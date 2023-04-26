# Comparing `tmp/scrape_schema-0.0.8.tar.gz` & `tmp/scrape_schema-0.0.9.tar.gz`

## Comparing `scrape_schema-0.0.8.tar` & `scrape_schema-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 scrape_schema-0.0.8/scrape_schema/__init__.py
--rw-r--r--   0        0        0    19469 2020-02-02 00:00:00.000000 scrape_schema-0.0.8/scrape_schema/base.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 scrape_schema-0.0.8/scrape_schema/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scrape_schema-0.0.8/scrape_schema/callbacks/__init__.py
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 scrape_schema-0.0.8/scrape_schema/callbacks/slax.py
--rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 scrape_schema-0.0.8/scrape_schema/callbacks/soup.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 scrape_schema-0.0.8/scrape_schema/factory/__init__.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 scrape_schema-0.0.8/scrape_schema/fields/__init__.py
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 scrape_schema-0.0.8/scrape_schema/fields/nested.py
--rw-r--r--   0        0        0     6111 2020-02-02 00:00:00.000000 scrape_schema-0.0.8/scrape_schema/fields/regex.py
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 scrape_schema-0.0.8/scrape_schema/fields/slax.py
--rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 scrape_schema-0.0.8/scrape_schema/fields/soup.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scrape_schema-0.0.8/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 scrape_schema-0.0.8/LICENSE
--rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 scrape_schema-0.0.8/README.md
--rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 scrape_schema-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     5166 2020-02-02 00:00:00.000000 scrape_schema-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 scrape_schema-0.0.9/scrape_schema/__init__.py
+-rw-r--r--   0        0        0    20490 2020-02-02 00:00:00.000000 scrape_schema-0.0.9/scrape_schema/base.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 scrape_schema-0.0.9/scrape_schema/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scrape_schema-0.0.9/scrape_schema/callbacks/__init__.py
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 scrape_schema-0.0.9/scrape_schema/callbacks/slax.py
+-rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 scrape_schema-0.0.9/scrape_schema/callbacks/soup.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 scrape_schema-0.0.9/scrape_schema/factory/__init__.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 scrape_schema-0.0.9/scrape_schema/fields/__init__.py
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 scrape_schema-0.0.9/scrape_schema/fields/nested.py
+-rw-r--r--   0        0        0     6111 2020-02-02 00:00:00.000000 scrape_schema-0.0.9/scrape_schema/fields/regex.py
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 scrape_schema-0.0.9/scrape_schema/fields/slax.py
+-rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 scrape_schema-0.0.9/scrape_schema/fields/soup.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scrape_schema-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 scrape_schema-0.0.9/LICENSE
+-rw-r--r--   0        0        0     3665 2020-02-02 00:00:00.000000 scrape_schema-0.0.9/README.md
+-rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 scrape_schema-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 scrape_schema-0.0.9/PKG-INFO
```

### Comparing `scrape_schema-0.0.8/scrape_schema/base.py` & `scrape_schema-0.0.9/scrape_schema/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,32 +211,52 @@
 
     def extract(self, markup: MARKUP_TYPE, *, type_: Optional[Type] = None) -> Any:
         """parse markup without BaseSchema Instance
 
         :param markup: string target
         :param type_: optional type for type-casting
         """
-        # TODO add logging
+        logger.info(
+            "%s[%s] start extract value. Field attrs: factory=%s, callback=%s, filter_=%s, default=%s",
+            self.__class__.__name__,
+            self.Config.parser or "str",
+            repr(self.factory),
+            repr(self.callback),
+            repr(self.filter_),
+            self.default,
+        )
         if self.Config.parser and not isinstance(markup, self.Config.parser):
             raise TypeError(
-                f"markup in `{self.__class__.__name__}` "
+                f"Markup in `{self.__class__.__name__}` "
                 f"should be `{self.Config.parser.__name__}`,"
                 f"not {type(markup).__name__}"
             )
         value = self._parse(markup)
         if not value:
+            logger.debug(
+                "%s.extract value not found, set default `%s` value",
+                self.__class__.__name__,
+                self.default)
             value = self.default
         if self._is_iterable_and_not_string_value(value):
+            if self.filter_:
+                logger.debug(
+                    "%s.extract `filter_(%s)`", self.__class__.__name__, value)
             value = self._filter(value)
         if self.callback:
+            logger.debug(
+                "%s.extract `callback(%s)`", self.__class__.__name__, value)
             value = self._callback(value)
         if self.factory:
+            logger.debug(
+                "%s.extract `factory(%s)`", self.__class__.__name__, value)
             value = self._factory(value)
         elif type_:
             value = self._cast_type(type_, value)
+        logger.info("%s.extract return `%s[%s]`", self.__class__.__name__, value, type(value).__name__)
         return value
 
     def __call__(self, instance: BaseSchema, name: str, markup: MARKUP_TYPE) -> Any:
         logger.info(
             "`%s.%s[%s]`. Field attrs: factory=%s, callback=%s, filter_=%s, default=%s",
             instance.__class__.__name__,
             name,
@@ -276,14 +296,15 @@
         if self.factory:
             value = self._factory(value)
             logger.debug(
                 "factory `%s.%s = %s`", instance.__class__.__name__, name, value
             )
         else:
             value = self._typing(instance, name, value)
+        logger.info(r"finish parse value %s.%s = %s")
         return value
 
     def _filter(self, value: T) -> Any:
         """filter parsed value by filter_ function, if it passed
 
         :param value: list or dict value. dict filter by values
         :return: filtered value
@@ -550,15 +571,16 @@
 
     @classmethod
     def from_kwargs(cls, **kwargs) -> Self:
         """Create new class without parse markup and fields
 
         :param kwargs: any keyword arguments
         """
-        kwargs.pop("parse_markup")
+        if kwargs.get("parse_markup"):
+            kwargs.pop("parse_markup")
 
         return cls("", parse_markup=False, **kwargs)
 
     @staticmethod
     def _to_dict(value: BaseSchema | list | dict):
         if isinstance(value, BaseSchema):
             return value.dict()
```

### Comparing `scrape_schema-0.0.8/scrape_schema/callbacks/slax.py` & `scrape_schema-0.0.9/scrape_schema/callbacks/slax.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.8/scrape_schema/callbacks/soup.py` & `scrape_schema-0.0.9/scrape_schema/callbacks/soup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """build-in callbacks for fields.soup"""
+from __future__ import annotations
 import re
 from typing import Any, Callable, Optional
 
 from bs4 import BeautifulSoup, Tag
 
 RE_TAG_NAME = re.compile(r"<(\w+)")
 RE_TAG_ATTRS = re.compile(r'(?P<name>[\w_\-:.]+)="(?P<value>[\w_\-:.]+)"')
@@ -28,25 +29,27 @@
                 old, new, count
             )
         return tag
 
     return wrapper
 
 
-def element_to_dict(element: str) -> dict[str, str | dict]:
+def element_to_dict(element: str) -> dict[str, str | dict[str, str | list[str]]]:
     """Convert string element to dict
 
     Example:
         <p> -> {"name": "p", "attrs":{}}
         <a id="1", class="thing"> -> {"name": "a", "attrs": {"id": "1", "class": "thing"}}
     """
     if not (match := RE_TAG_NAME.search(element)):
-        raise TypeError(f"Element `{element}` is not HTML tag")
+        raise TypeError(f"Element `{element}` is not valid HTML tag")
     tag_name = match.group(1)
     attrs = dict(RE_TAG_ATTRS.findall(element))
+    if (klass := attrs.get("class")) and len(klass.split(" ")) != 1:
+        attrs["class"] = klass.split(" ")
     return {"name": tag_name, "attrs": attrs}
 
 
 def get_text(
     separator: str = "", strip: bool = False
 ) -> Callable[[Tag | Any], str | Any]:
     """get text from bs4.Tag
```

### Comparing `scrape_schema-0.0.8/scrape_schema/fields/nested.py` & `scrape_schema-0.0.9/scrape_schema/fields/nested.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.8/scrape_schema/fields/regex.py` & `scrape_schema-0.0.9/scrape_schema/fields/regex.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.8/scrape_schema/fields/slax.py` & `scrape_schema-0.0.9/scrape_schema/fields/slax.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.8/scrape_schema/fields/soup.py` & `scrape_schema-0.0.9/scrape_schema/fields/soup.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.8/.gitignore` & `scrape_schema-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.8/LICENSE` & `scrape_schema-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.8/README.md` & `scrape_schema-0.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -10,41 +10,50 @@
 or the complete absence of the **API interfaces** and decrease lines of code
 
 Also structuring, data serialization and use as an intermediate layer 
 for third-party serialization libraries: json, dataclasses, pydantic, etc
 
 _____
 # Features
-* Partial support type-casting from annotations (str, int, float, bool, list, dict)
-* Optional success-attempts parse values checker
-* Factory functions for convert values
-* Filter functions for filter a founded values
-* Optional checking the success of getting the value from the field
+* partial support type-casting from annotations (str, int, float, bool, list, dict, Optional)
+* converting parsed values using callbacks, filters, factories
+* logging to quickly find problems in getting values
+* optional success-attempts parse values checker from fields objects
+* decrease code lines for your parsers
+* standardization, modularity* of structures-parsers
+
+*If you usage schema-structures and they are separated from the logic of getting the text
+(stdout output, HTTP requests, etc)
 ____
-# Build-in backends parsers support:
-* re
-* bs4
-* selectolax(Modest)
-* parsel (TODO)
+# Build-in libraries parsers support:
+- [x] re
+- [x] bs4
+- [x] selectolax(Modest)
+- [ ] parsel
+- [ ] lxml
+- [ ] selenium
+- [ ] playwright
 ____
 # Install
 
-zero dependencies (regex, nested fields)
+zero dependencies: regex, nested fields (and typing_extension if python < 3.11)
 ```shell
 pip install scrape-schema
 ```
+
 add bs4 fields
 ```shell
 pip install scrape-schema[bs4]
 ```
 
 add selectolax fields
 ```shell
 pip install scrape-schema[selectolax]
 ```
+
 add all fields
 ```shell
 pip install scrape-schema[all]
 ```
 ____
 # Example
 ```python
@@ -60,15 +69,14 @@
 -bar:20
 lorem upsum dolor
 192.168.0.1
 """
 
 
 class Schema(BaseSchema):
-    status: str = "OK"
     ipv4: Annotated[str, ReMatch(r"(\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})")]
     max_digit: Annotated[int, ReMatchList(r"(\d+)",
                                           callback=int,                                      
                                           factory=max)]
     failed_value: Annotated[bool, ReMatchList(r"(ora)", default=False)]
     digits: Annotated[list[int], ReMatchList(r"(\d+)")]
     digits_float: Annotated[list[float], ReMatchList(r"(\d+)", 
@@ -96,15 +104,15 @@
 In this project, logging to the `DEBUG` level is enabled by default. 
 
 To set up logger, you can get it by the name `"scrape_schema"`
 ```python
 import logging
 
 logger = logging.getLogger("scrape_schema")
-logger.setLevel(logging.WARNING)
+logger.setLevel(logging.ERROR)
 ...
 ```
 
 See more [examples](examples) and [documentation](https://scrape-schema.readthedocs.io/en/latest/) 
 for get more information/examples
 ____
 This project is licensed under the terms of the MIT license.
```

### Comparing `scrape_schema-0.0.8/pyproject.toml` & `scrape_schema-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.8/PKG-INFO` & `scrape_schema-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrape-schema
-Version: 0.0.8
+Version: 0.0.9
 Summary: A library for converting any text (xml, html, plain text, stdout, etc) to python datatypes
 Project-URL: Documentation, https://github.com/vypivshiy/scrape-schema#readme
 Project-URL: Issues, https://github.com/vypivshiy/scrape-schema/issues
 Project-URL: Source, https://github.com/vypivshiy/scrape-schema
 Project-URL: Examples, https://github.com/vypivshiy/scrape-schema/examples
 Author: vypivshiy
 License-Expression: MIT
@@ -53,41 +53,50 @@
 or the complete absence of the **API interfaces** and decrease lines of code
 
 Also structuring, data serialization and use as an intermediate layer 
 for third-party serialization libraries: json, dataclasses, pydantic, etc
 
 _____
 # Features
-* Partial support type-casting from annotations (str, int, float, bool, list, dict)
-* Optional success-attempts parse values checker
-* Factory functions for convert values
-* Filter functions for filter a founded values
-* Optional checking the success of getting the value from the field
+* partial support type-casting from annotations (str, int, float, bool, list, dict, Optional)
+* converting parsed values using callbacks, filters, factories
+* logging to quickly find problems in getting values
+* optional success-attempts parse values checker from fields objects
+* decrease code lines for your parsers
+* standardization, modularity* of structures-parsers
+
+*If you usage schema-structures and they are separated from the logic of getting the text
+(stdout output, HTTP requests, etc)
 ____
-# Build-in backends parsers support:
-* re
-* bs4
-* selectolax(Modest)
-* parsel (TODO)
+# Build-in libraries parsers support:
+- [x] re
+- [x] bs4
+- [x] selectolax(Modest)
+- [ ] parsel
+- [ ] lxml
+- [ ] selenium
+- [ ] playwright
 ____
 # Install
 
-zero dependencies (regex, nested fields)
+zero dependencies: regex, nested fields (and typing_extension if python < 3.11)
 ```shell
 pip install scrape-schema
 ```
+
 add bs4 fields
 ```shell
 pip install scrape-schema[bs4]
 ```
 
 add selectolax fields
 ```shell
 pip install scrape-schema[selectolax]
 ```
+
 add all fields
 ```shell
 pip install scrape-schema[all]
 ```
 ____
 # Example
 ```python
@@ -103,15 +112,14 @@
 -bar:20
 lorem upsum dolor
 192.168.0.1
 """
 
 
 class Schema(BaseSchema):
-    status: str = "OK"
     ipv4: Annotated[str, ReMatch(r"(\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})")]
     max_digit: Annotated[int, ReMatchList(r"(\d+)",
                                           callback=int,                                      
                                           factory=max)]
     failed_value: Annotated[bool, ReMatchList(r"(ora)", default=False)]
     digits: Annotated[list[int], ReMatchList(r"(\d+)")]
     digits_float: Annotated[list[float], ReMatchList(r"(\d+)", 
@@ -139,15 +147,15 @@
 In this project, logging to the `DEBUG` level is enabled by default. 
 
 To set up logger, you can get it by the name `"scrape_schema"`
 ```python
 import logging
 
 logger = logging.getLogger("scrape_schema")
-logger.setLevel(logging.WARNING)
+logger.setLevel(logging.ERROR)
 ...
 ```
 
 See more [examples](examples) and [documentation](https://scrape-schema.readthedocs.io/en/latest/) 
 for get more information/examples
 ____
 This project is licensed under the terms of the MIT license.
```

