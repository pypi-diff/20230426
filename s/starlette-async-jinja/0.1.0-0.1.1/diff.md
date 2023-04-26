# Comparing `tmp/starlette_async_jinja-0.1.0.tar.gz` & `tmp/starlette_async_jinja-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starlette_async_jinja-0.1.0.tar", last modified: Sun Apr 16 04:09:20 2023, max compression
+gzip compressed data, was "starlette_async_jinja-0.1.1.tar", last modified: Wed Apr 26 17:40:13 2023, max compression
```

## Comparing `starlette_async_jinja-0.1.0.tar` & `starlette_async_jinja-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,5 @@
--rw-r--r--   0        0        0      284 2023-04-16 04:08:28.506884 starlette_async_jinja-0.1.0/README.md
--rw-r--r--   0        0        0     1117 2023-04-16 04:09:20.174436 starlette_async_jinja-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        4 2023-04-16 01:42:22.107238 starlette_async_jinja-0.1.0/starlette_async_jinja/__init__.py
--rw-r--r--   0        0        0     1297 2023-04-16 01:49:37.625240 starlette_async_jinja-0.1.0/starlette_async_jinja/bccache.py
--rw-r--r--   0        0        0     5079 2023-04-16 01:42:22.123633 starlette_async_jinja-0.1.0/starlette_async_jinja/compiler.py
--rw-r--r--   0        0        0     1789 2023-04-16 01:49:37.640539 starlette_async_jinja-0.1.0/starlette_async_jinja/environment.py
--rw-r--r--   0        0        0     1735 2023-04-16 01:49:37.632571 starlette_async_jinja-0.1.0/starlette_async_jinja/loaders.py
--rw-r--r--   0        0        0     3420 2023-04-16 01:49:37.616807 starlette_async_jinja-0.1.0/starlette_async_jinja/responses.py
--rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 starlette_async_jinja-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      282 2023-04-26 14:31:29.295695 starlette_async_jinja-0.1.1/README.md
+-rw-r--r--   0        0        0     1174 2023-04-26 17:40:13.118620 starlette_async_jinja-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      420 2023-04-22 16:45:22.461705 starlette_async_jinja-0.1.1/starlette_async_jinja/__init__.py
+-rw-r--r--   0        0        0     3753 2023-04-26 17:38:29.008338 starlette_async_jinja-0.1.1/starlette_async_jinja/responses.py
+-rw-r--r--   0        0        0      776 1970-01-01 00:00:00.000000 starlette_async_jinja-0.1.1/PKG-INFO
```

### Comparing `starlette_async_jinja-0.1.0/starlette_async_jinja/responses.py` & `starlette_async_jinja-0.1.1/starlette_async_jinja/responses.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,97 +1,106 @@
-import typing as t
 import os
+import typing as t
 
+from acb.adapters import AsyncEnvironment
 from jinja2.environment import Template
+from msgspec import json
 from starlette.background import BackgroundTask
 from starlette.requests import Request
 from starlette.responses import HTMLResponse
+from starlette.responses import JSONResponse
 from starlette.templating import Jinja2Templates
 from starlette.templating import pass_context
 from starlette.types import Receive
 from starlette.types import Scope
 from starlette.types import Send
-from environment import AsyncEnvironment
 
 
-class _TemplateResponse(HTMLResponse):
+class JsonResponse(JSONResponse):
+    async def render(self, content: str) -> bytes:
+        return json.encode(content)
+
+
+class _AsyncTemplateResponse(HTMLResponse):
     def __init__(
         self,
-        template: t.Any,
-        context: dict,
+        template: Template,
+        context: dict[str, str],
         content: str,
         status_code: int = 200,
         headers: t.Optional[t.Mapping[str, str]] = None,
         media_type: t.Optional[str] = None,
         background: t.Optional[BackgroundTask] = None,
-    ):
+    ) -> None:
         self.template = template
         self.context = context
         super().__init__(content, status_code, headers, media_type, background)
 
     async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
-        request = self.context.get("request", {})
-        extensions = request.get("extensions", {})
+        request: str | dict = self.context.get("request", {})
+        extensions: dict[str, str] = request.get("extensions", {})
         if "http.response.debug" in extensions:
             await send(
                 {
                     "type": "http.response.debug",
                     "info": {"template": self.template, "context": self.context},
                 }
             )
         await super().__call__(scope, receive, send)
 
 
 class AsyncJinja2Templates(Jinja2Templates):
     def __init__(
         self,
-        directory: t.Union[str, os.PathLike],
+        directory: str | os.PathLike,
         context_processors: t.Optional[
             t.List[t.Callable[[Request], t.Dict[str, t.Any]]]
         ] = None,
         **env_options: t.Any,
-    ):
+    ) -> None:
         super().__init__(directory, **env_options)
         self.env_options = env_options
         self.context_processors = context_processors or []
         self.env = self._create_env(directory, **env_options)
 
     def _create_env(
-        self, directory: t.Union[str, os.PathLike], **env_options: t.Any
+        self, directory: str | os.PathLike, **env_options: dict[str, str] | bool
     ) -> "AsyncEnvironment":
         @pass_context
-        def url_for(context: dict, name: str, **path_params: t.Any) -> str:
+        def url_for(
+            context: dict[str, t.Any], name: str, **path_params: dict[str, str | bool]
+        ) -> str:
             request = context["request"]
             return request.url_for(name, **path_params)
 
         env_options.setdefault("autoescape", True)
         env = AsyncEnvironment(**env_options)
         env.globals["url_for"] = url_for
         return env
 
     async def get_template(self, name: str) -> "Template":
         return await self.env.get_template(name)
 
-    async def TemplateResponse(
+    async def AsyncTemplateResponse(
         self,
         name: str,
-        context: dict,
+        context: dict[str, str],
         status_code: int = 200,
         headers: t.Optional[t.Mapping[str, str]] = None,
         media_type: t.Optional[str] = None,
         background: t.Optional[BackgroundTask] = None,
-    ) -> _TemplateResponse:
+    ) -> "_AsyncTemplateResponse":
         if "request" not in context:
             raise ValueError('context must include a "request" key')
         request = t.cast(Request, context["request"])
         for context_processor in self.context_processors:
             context.update(context_processor(request))
         template = await self.get_template(name)
         content = await template.render_async(context)
-        return _TemplateResponse(
+        return _AsyncTemplateResponse(
             template,
             context,
             content,
             status_code=status_code,
             headers=headers,
             media_type=media_type,
             background=background,
```

