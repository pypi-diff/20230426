# Comparing `tmp/litestar-2.0.0a4.tar.gz` & `tmp/litestar-2.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litestar-2.0.0a4.tar", max compression
+gzip compressed data, was "litestar-2.0.0a5.tar", max compression
```

## Comparing `litestar-2.0.0a4.tar` & `litestar-2.0.0a5.tar`

### file list

```diff
@@ -1,273 +1,292 @@
--rw-r--r--   0        0        0     1092 2023-04-11 16:09:54.380440 litestar-2.0.0a4/LICENSE
--rw-r--r--   0        0        0    48376 2023-04-11 16:09:54.380440 litestar-2.0.0a4/README.md
--rw-r--r--   0        0        0      744 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/__init__.py
--rw-r--r--   0        0        0      103 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/__main__.py
--rw-r--r--   0        0        0       77 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_asgi/__init__.py
--rw-r--r--   0        0        0     8644 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_asgi/asgi_router.py
--rw-r--r--   0        0        0      349 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_asgi/routing_trie/__init__.py
--rw-r--r--   0        0        0     7823 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_asgi/routing_trie/mapping.py
--rw-r--r--   0        0        0     5938 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_asgi/routing_trie/traversal.py
--rw-r--r--   0        0        0     2598 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_asgi/routing_trie/types.py
--rw-r--r--   0        0        0     1267 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_asgi/routing_trie/validate.py
--rw-r--r--   0        0        0     1528 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_asgi/utils.py
--rw-r--r--   0        0        0       66 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_kwargs/__init__.py
--rw-r--r--   0        0        0     3868 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_kwargs/cleanup.py
--rw-r--r--   0        0        0     4245 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_kwargs/dependencies.py
--rw-r--r--   0        0        0    14489 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_kwargs/extractors.py
--rw-r--r--   0        0        0    20815 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_kwargs/kwargs_model.py
--rw-r--r--   0        0        0     2759 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_kwargs/parameter_definition.py
--rw-r--r--   0        0        0        0 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_layers/__init__.py
--rw-r--r--   0        0        0     1288 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_layers/utils.py
--rw-r--r--   0        0        0     5935 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_multipart.py
--rw-r--r--   0        0        0        0 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_openapi/__init__.py
--rw-r--r--   0        0        0    10155 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_openapi/parameters.py
--rw-r--r--   0        0        0     5490 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_openapi/path_item.py
--rw-r--r--   0        0        0     1237 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_openapi/request_body.py
--rw-r--r--   0        0        0    10005 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_openapi/responses.py
--rw-r--r--   0        0        0       64 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_openapi/schema_generation/__init__.py
--rw-r--r--   0        0        0     7120 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_openapi/schema_generation/constrained_fields.py
--rw-r--r--   0        0        0     2093 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_openapi/schema_generation/examples.py
--rw-r--r--   0        0        0    28352 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_openapi/schema_generation/schema.py
--rw-r--r--   0        0        0      524 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_openapi/schema_generation/utils.py
--rw-r--r--   0        0        0        0 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_openapi/typescript_converter/__init__.py
--rw-r--r--   0        0        0    10970 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_openapi/typescript_converter/converter.py
--rw-r--r--   0        0        0     5242 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_openapi/typescript_converter/schema_parsing.py
--rw-r--r--   0        0        0     7685 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_openapi/typescript_converter/types.py
--rw-r--r--   0        0        0     1483 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_openapi/utils.py
--rw-r--r--   0        0        0     2465 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_parsers.py
--rw-r--r--   0        0        0      182 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_signature/__init__.py
--rw-r--r--   0        0        0     5995 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_signature/field.py
--rw-r--r--   0        0        0       64 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_signature/models/__init__.py
--rw-r--r--   0        0        0    12635 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_signature/models/attrs_signature_model.py
--rw-r--r--   0        0        0     3982 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_signature/models/base.py
--rw-r--r--   0        0        0     7456 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_signature/models/pydantic_signature_model.py
--rw-r--r--   0        0        0     8714 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/_signature/utils.py
--rw-r--r--   0        0        0    38796 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/app.py
--rw-r--r--   0        0        0     2200 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/background_tasks.py
--rw-r--r--   0        0        0        0 2023-04-11 16:09:54.400437 litestar-2.0.0a4/litestar/cli/__init__.py
--rw-r--r--   0        0        0    11820 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/cli/_utils.py
--rw-r--r--   0        0        0        0 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/cli/commands/__init__.py
--rw-r--r--   0        0        0     4553 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/cli/commands/core.py
--rw-r--r--   0        0        0     2365 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/cli/commands/schema.py
--rw-r--r--   0        0        0     2224 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/cli/commands/sessions.py
--rw-r--r--   0        0        0      807 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/cli/main.py
--rw-r--r--   0        0        0        0 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/config/__init__.py
--rw-r--r--   0        0        0     1747 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/config/allowed_hosts.py
--rw-r--r--   0        0        0    12358 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/config/app.py
--rw-r--r--   0        0        0     2742 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/config/compression.py
--rw-r--r--   0        0        0     5177 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/config/cors.py
--rw-r--r--   0        0        0     1771 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/config/csrf.py
--rw-r--r--   0        0        0     1991 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/config/response_cache.py
--rw-r--r--   0        0        0     1922 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/connection/__init__.py
--rw-r--r--   0        0        0    10838 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/connection/base.py
--rw-r--r--   0        0        0     7698 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/connection/request.py
--rw-r--r--   0        0        0     9005 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/connection/websocket.py
--rw-r--r--   0        0        0     1098 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/constants.py
--rw-r--r--   0        0        0        0 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/htmx/__init__.py
--rw-r--r--   0        0        0     4917 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/htmx/_utils.py
--rw-r--r--   0        0        0     4051 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/htmx/request.py
--rw-r--r--   0        0        0     8349 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/htmx/response.py
--rw-r--r--   0        0        0     1261 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/htmx/types.py
--rw-r--r--   0        0        0     2557 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/jinja.py
--rw-r--r--   0        0        0      521 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/jwt/__init__.py
--rw-r--r--   0        0        0    28720 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/jwt/jwt_auth.py
--rw-r--r--   0        0        0     3978 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/jwt/jwt_token.py
--rw-r--r--   0        0        0     6970 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/jwt/middleware.py
--rw-r--r--   0        0        0     3916 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/mako.py
--rw-r--r--   0        0        0        0 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/msgspec/__init__.py
--rw-r--r--   0        0        0      180 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/opentelemetry/__init__.py
--rw-r--r--   0        0        0      845 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/opentelemetry/_utils.py
--rw-r--r--   0        0        0     4206 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/opentelemetry/config.py
--rw-r--r--   0        0        0     2212 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/opentelemetry/middleware.py
--rw-r--r--   0        0        0     4044 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/piccolo_orm.py
--rw-r--r--   0        0        0        0 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/pydantic/__init__.py
--rw-r--r--   0        0        0      280 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/repository/__init__.py
--rw-r--r--   0        0        0     9079 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/repository/abc.py
--rw-r--r--   0        0        0      328 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/repository/exceptions.py
--rw-r--r--   0        0        0     1162 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/repository/filters.py
--rw-r--r--   0        0        0        0 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/repository/testing/__init__.py
--rw-r--r--   0        0        0    12484 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/repository/testing/generic_mock_repository.py
--rw-r--r--   0        0        0        0 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     3460 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/sqlalchemy/base.py
--rw-r--r--   0        0        0        0 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/sqlalchemy/dto.py
--rw-r--r--   0        0        0      390 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/sqlalchemy/init_plugin/__init__.py
--rw-r--r--   0        0        0      458 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/sqlalchemy/init_plugin/config/__init__.py
--rw-r--r--   0        0        0     3602 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/sqlalchemy/init_plugin/config/asyncio.py
--rw-r--r--   0        0        0    11308 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/sqlalchemy/init_plugin/config/common.py
--rw-r--r--   0        0        0    11499 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/sqlalchemy/init_plugin/config/engine.py
--rw-r--r--   0        0        0     2849 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/sqlalchemy/init_plugin/config/sync.py
--rw-r--r--   0        0        0     1527 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/sqlalchemy/init_plugin/plugin.py
--rw-r--r--   0        0        0    19731 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/sqlalchemy/repository.py
--rw-r--r--   0        0        0        0 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/sqlalchemy_1/__init__.py
--rw-r--r--   0        0        0    13770 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/sqlalchemy_1/config.py
--rw-r--r--   0        0        0    19447 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/sqlalchemy_1/plugin.py
--rw-r--r--   0        0        0     1319 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/sqlalchemy_1/types.py
--rw-r--r--   0        0        0     6071 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/contrib/tortoise_orm.py
--rw-r--r--   0        0        0     9559 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/controller.py
--rw-r--r--   0        0        0    16462 2023-04-11 16:09:54.404437 litestar-2.0.0a4/litestar/data_extractors.py
--rw-r--r--   0        0        0      883 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/datastructures/__init__.py
--rw-r--r--   0        0        0     3757 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/datastructures/cookie.py
--rw-r--r--   0        0        0    17316 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/datastructures/headers.py
--rw-r--r--   0        0        0     2977 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/datastructures/multi_dicts.py
--rw-r--r--   0        0        0     5027 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/datastructures/response_header.py
--rw-r--r--   0        0        0     9302 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/datastructures/state.py
--rw-r--r--   0        0        0     3360 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/datastructures/upload_file.py
--rw-r--r--   0        0        0     7273 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/datastructures/url.py
--rw-r--r--   0        0        0     2386 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/di.py
--rw-r--r--   0        0        0        0 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/dto/__init__.py
--rw-r--r--   0        0        0      337 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/dto/exceptions.py
--rw-r--r--   0        0        0     2484 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/dto/interface.py
--rw-r--r--   0        0        0     1728 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/enums.py
--rw-r--r--   0        0        0      201 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/events/__init__.py
--rw-r--r--   0        0        0     4597 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/events/emitter.py
--rw-r--r--   0        0        0     1305 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/events/listener.py
--rw-r--r--   0        0        0     1142 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/exceptions/__init__.py
--rw-r--r--   0        0        0     1608 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/exceptions/base_exceptions.py
--rw-r--r--   0        0        0     4629 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/exceptions/http_exceptions.py
--rw-r--r--   0        0        0     1351 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/exceptions/websocket_exceptions.py
--rw-r--r--   0        0        0     5350 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/file_system.py
--rw-r--r--   0        0        0      559 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/handlers/__init__.py
--rw-r--r--   0        0        0     3877 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/handlers/asgi_handlers.py
--rw-r--r--   0        0        0    16350 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/handlers/base.py
--rw-r--r--   0        0        0      263 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/handlers/http_handlers/__init__.py
--rw-r--r--   0        0        0     9280 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/handlers/http_handlers/_utils.py
--rw-r--r--   0        0        0    25419 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/handlers/http_handlers/base.py
--rw-r--r--   0        0        0    60867 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/handlers/http_handlers/decorators.py
--rw-r--r--   0        0        0    16602 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/handlers/websocket_handlers.py
--rw-r--r--   0        0        0      147 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/logging/__init__.py
--rw-r--r--   0        0        0      569 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/logging/_utils.py
--rw-r--r--   0        0        0    12050 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/logging/config.py
--rw-r--r--   0        0        0     1129 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/logging/picologging.py
--rw-r--r--   0        0        0      860 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/logging/standard.py
--rw-r--r--   0        0        0      385 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/__init__.py
--rw-r--r--   0        0        0     2081 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/_utils.py
--rw-r--r--   0        0        0     2973 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/allowed_hosts.py
--rw-r--r--   0        0        0     3436 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/authentication.py
--rw-r--r--   0        0        0     5302 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/base.py
--rw-r--r--   0        0        0     8367 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/compression.py
--rw-r--r--   0        0        0     2573 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/cors.py
--rw-r--r--   0        0        0     6474 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/csrf.py
--rw-r--r--   0        0        0      124 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/exceptions/__init__.py
--rw-r--r--   0        0        0     7191 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/exceptions/_debug_response.py
--rw-r--r--   0        0        0     9006 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/exceptions/middleware.py
--rw-r--r--   0        0        0      398 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/exceptions/templates/body.html
--rw-r--r--   0        0        0      344 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/exceptions/templates/frame.html
--rw-r--r--   0        0        0      920 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/exceptions/templates/scripts.js
--rw-r--r--   0        0        0     1830 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/exceptions/templates/styles.css
--rw-r--r--   0        0        0    13393 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/logging.py
--rw-r--r--   0        0        0    10821 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/rate_limit.py
--rw-r--r--   0        0        0       70 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/session/__init__.py
--rw-r--r--   0        0        0     7961 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/session/base.py
--rw-r--r--   0        0        0    10387 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/session/client_side.py
--rw-r--r--   0        0        0     8580 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/middleware/session/server_side.py
--rw-r--r--   0        0        0      231 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/openapi/__init__.py
--rw-r--r--   0        0        0     5226 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/openapi/config.py
--rw-r--r--   0        0        0    16449 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/openapi/controller.py
--rw-r--r--   0        0        0      898 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/openapi/datastructures.py
--rw-r--r--   0        0        0     1691 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/openapi/spec/__init__.py
--rw-r--r--   0        0        0     1648 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/openapi/spec/base.py
--rw-r--r--   0        0        0      961 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/openapi/spec/callback.py
--rw-r--r--   0        0        0     2936 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/openapi/spec/components.py
--rw-r--r--   0        0        0      592 2023-04-11 16:09:54.408436 litestar-2.0.0a4/litestar/openapi/spec/contact.py
--rw-r--r--   0        0        0      950 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/discriminator.py
--rw-r--r--   0        0        0     3290 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/encoding.py
--rw-r--r--   0        0        0      974 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/enums.py
--rw-r--r--   0        0        0     1168 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/example.py
--rw-r--r--   0        0        0      614 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/external_documentation.py
--rw-r--r--   0        0        0     5669 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/header.py
--rw-r--r--   0        0        0     1413 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/info.py
--rw-r--r--   0        0        0      752 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/license.py
--rw-r--r--   0        0        0     2876 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/link.py
--rw-r--r--   0        0        0     1882 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/media_type.py
--rw-r--r--   0        0        0     1195 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/oauth_flow.py
--rw-r--r--   0        0        0      897 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/oauth_flows.py
--rw-r--r--   0        0        0     4218 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/open_api.py
--rw-r--r--   0        0        0     4842 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/operation.py
--rw-r--r--   0        0        0     6242 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/parameter.py
--rw-r--r--   0        0        0     3245 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/path_item.py
--rw-r--r--   0        0        0     1255 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/paths.py
--rw-r--r--   0        0        0     1351 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/reference.py
--rw-r--r--   0        0        0     1095 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/request_body.py
--rw-r--r--   0        0        0     1854 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/response.py
--rw-r--r--   0        0        0     2367 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/responses.py
--rw-r--r--   0        0        0    34574 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/schema.py
--rw-r--r--   0        0        0     1686 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/security_requirement.py
--rw-r--r--   0        0        0     2690 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/security_scheme.py
--rw-r--r--   0        0        0     1077 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/server.py
--rw-r--r--   0        0        0     1171 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/server_variable.py
--rw-r--r--   0        0        0      923 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/tag.py
--rw-r--r--   0        0        0     1702 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/openapi/spec/xml.py
--rw-r--r--   0        0        0    10984 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/pagination.py
--rw-r--r--   0        0        0    16805 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/params.py
--rw-r--r--   0        0        0     7102 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/partial.py
--rw-r--r--   0        0        0     7209 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/plugins.py
--rw-r--r--   0        0        0        0 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/py.typed
--rw-r--r--   0        0        0      278 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/response/__init__.py
--rw-r--r--   0        0        0    12185 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/response/base.py
--rw-r--r--   0        0        0     8954 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/response/file.py
--rw-r--r--   0        0        0     2952 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/response/redirect.py
--rw-r--r--   0        0        0     4893 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/response/streaming.py
--rw-r--r--   0        0        0     2994 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/response/template.py
--rw-r--r--   0        0        0    14975 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/response_containers.py
--rw-r--r--   0        0        0    15028 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/router.py
--rw-r--r--   0        0        0      191 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/routes/__init__.py
--rw-r--r--   0        0        0     1763 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/routes/asgi.py
--rw-r--r--   0        0        0     6443 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/routes/base.py
--rw-r--r--   0        0        0    13384 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/routes/http.py
--rw-r--r--   0        0        0     3058 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/routes/websocket.py
--rw-r--r--   0        0        0       97 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/security/__init__.py
--rw-r--r--   0        0        0     7165 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/security/base.py
--rw-r--r--   0        0        0      188 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/security/session_auth/__init__.py
--rw-r--r--   0        0        0     5602 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/security/session_auth/auth.py
--rw-r--r--   0        0        0     4941 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/security/session_auth/middleware.py
--rw-r--r--   0        0        0     6606 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/serialization.py
--rw-r--r--   0        0        0      158 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/static_files/__init__.py
--rw-r--r--   0        0        0     5019 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/static_files/base.py
--rw-r--r--   0        0        0     3582 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/static_files/config.py
--rw-r--r--   0        0        0     9536 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/status_codes.py
--rw-r--r--   0        0        0        0 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/stores/__init__.py
--rw-r--r--   0        0        0     4377 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/stores/base.py
--rw-r--r--   0        0        0     5425 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/stores/file.py
--rw-r--r--   0        0        0     3625 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/stores/memory.py
--rw-r--r--   0        0        0     6231 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/stores/redis.py
--rw-r--r--   0        0        0     2233 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/stores/registry.py
--rw-r--r--   0        0        0      204 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/template/__init__.py
--rw-r--r--   0        0        0     4113 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/template/base.py
--rw-r--r--   0        0        0     1894 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/template/config.py
--rw-r--r--   0        0        0      581 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/testing/__init__.py
--rw-r--r--   0        0        0     1816 2023-04-11 16:09:54.412436 litestar-2.0.0a4/litestar/testing/client/__init__.py
--rw-r--r--   0        0        0    17450 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/testing/client/async_client.py
--rw-r--r--   0        0        0     5132 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/testing/client/base.py
--rw-r--r--   0        0        0    19556 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/testing/client/sync_client.py
--rw-r--r--   0        0        0    31465 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/testing/helpers.py
--rw-r--r--   0        0        0     2534 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/testing/life_span_handler.py
--rw-r--r--   0        0        0    21905 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/testing/request_factory.py
--rw-r--r--   0        0        0     8094 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/testing/transport.py
--rw-r--r--   0        0        0     6943 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/testing/websocket_test_session.py
--rw-r--r--   0        0        0     4105 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/types/__init__.py
--rw-r--r--   0        0        0     8697 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/types/asgi_types.py
--rw-r--r--   0        0        0      453 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/types/builtin_types.py
--rw-r--r--   0        0        0     2291 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/types/callable_types.py
--rw-r--r--   0        0        0     1645 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/types/composite_types.py
--rw-r--r--   0        0        0      183 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/types/empty.py
--rw-r--r--   0        0        0     2662 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/types/file_types.py
--rw-r--r--   0        0        0      344 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/types/helper_types.py
--rw-r--r--   0        0        0     1487 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/types/internal_types.py
--rw-r--r--   0        0        0     2607 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/types/protocols.py
--rw-r--r--   0        0        0     1820 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/types/serialization.py
--rw-r--r--   0        0        0     1906 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/utils/__init__.py
--rw-r--r--   0        0        0      729 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/utils/compat.py
--rw-r--r--   0        0        0     3449 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/utils/dataclass.py
--rw-r--r--   0        0        0     3520 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/utils/deprecation.py
--rw-r--r--   0        0        0     1483 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/utils/helpers.py
--rw-r--r--   0        0        0      723 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/utils/path.py
--rw-r--r--   0        0        0    10438 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/utils/predicates.py
--rw-r--r--   0        0        0     2720 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/utils/scope.py
--rw-r--r--   0        0        0     1003 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/utils/sequence.py
--rw-r--r--   0        0        0    10889 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/utils/signature.py
--rw-r--r--   0        0        0     5337 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/utils/sync.py
--rw-r--r--   0        0        0     6405 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/utils/typing.py
--rw-r--r--   0        0        0     1921 2023-04-11 16:09:54.416435 litestar-2.0.0a4/litestar/utils/version.py
--rw-r--r--   0        0        0     9282 2023-04-11 16:09:54.416435 litestar-2.0.0a4/pyproject.toml
--rw-r--r--   0        0        0    51743 1970-01-01 00:00:00.000000 litestar-2.0.0a4/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-04-26 13:40:53.109600 litestar-2.0.0a5/LICENSE
+-rw-r--r--   0        0        0    49290 2023-04-26 13:40:53.109600 litestar-2.0.0a5/README.md
+-rw-r--r--   0        0        0      744 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/__init__.py
+-rw-r--r--   0        0        0      103 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/__main__.py
+-rw-r--r--   0        0        0       77 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_asgi/__init__.py
+-rw-r--r--   0        0        0     8632 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_asgi/asgi_router.py
+-rw-r--r--   0        0        0      349 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_asgi/routing_trie/__init__.py
+-rw-r--r--   0        0        0     7823 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_asgi/routing_trie/mapping.py
+-rw-r--r--   0        0        0     5938 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_asgi/routing_trie/traversal.py
+-rw-r--r--   0        0        0     2598 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_asgi/routing_trie/types.py
+-rw-r--r--   0        0        0     1267 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_asgi/routing_trie/validate.py
+-rw-r--r--   0        0        0     1528 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_asgi/utils.py
+-rw-r--r--   0        0        0       66 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_kwargs/__init__.py
+-rw-r--r--   0        0        0     3868 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_kwargs/cleanup.py
+-rw-r--r--   0        0        0     4239 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_kwargs/dependencies.py
+-rw-r--r--   0        0        0    14907 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_kwargs/extractors.py
+-rw-r--r--   0        0        0    20450 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_kwargs/kwargs_model.py
+-rw-r--r--   0        0        0     2759 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_kwargs/parameter_definition.py
+-rw-r--r--   0        0        0        0 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_layers/__init__.py
+-rw-r--r--   0        0        0     1288 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_layers/utils.py
+-rw-r--r--   0        0        0     5935 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_multipart.py
+-rw-r--r--   0        0        0        0 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_openapi/__init__.py
+-rw-r--r--   0        0        0    10117 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_openapi/parameters.py
+-rw-r--r--   0        0        0     5525 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_openapi/path_item.py
+-rw-r--r--   0        0        0     1476 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_openapi/request_body.py
+-rw-r--r--   0        0        0    10196 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_openapi/responses.py
+-rw-r--r--   0        0        0       64 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_openapi/schema_generation/__init__.py
+-rw-r--r--   0        0        0     7074 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_openapi/schema_generation/constrained_fields.py
+-rw-r--r--   0        0        0     2104 2023-04-26 13:40:53.129600 litestar-2.0.0a5/litestar/_openapi/schema_generation/examples.py
+-rw-r--r--   0        0        0    31705 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/_openapi/schema_generation/schema.py
+-rw-r--r--   0        0        0      524 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/_openapi/schema_generation/utils.py
+-rw-r--r--   0        0        0        0 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/_openapi/typescript_converter/__init__.py
+-rw-r--r--   0        0        0    10970 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/_openapi/typescript_converter/converter.py
+-rw-r--r--   0        0        0     5240 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/_openapi/typescript_converter/schema_parsing.py
+-rw-r--r--   0        0        0     7685 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/_openapi/typescript_converter/types.py
+-rw-r--r--   0        0        0     1464 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/_openapi/utils.py
+-rw-r--r--   0        0        0     2338 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/_parsers.py
+-rw-r--r--   0        0        0      182 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/_signature/__init__.py
+-rw-r--r--   0        0        0     5995 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/_signature/field.py
+-rw-r--r--   0        0        0       64 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/_signature/models/__init__.py
+-rw-r--r--   0        0        0    13178 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/_signature/models/attrs_signature_model.py
+-rw-r--r--   0        0        0     3736 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/_signature/models/base.py
+-rw-r--r--   0        0        0     6680 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/_signature/models/pydantic_signature_model.py
+-rw-r--r--   0        0        0     6510 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/_signature/utils.py
+-rw-r--r--   0        0        0    35419 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/app.py
+-rw-r--r--   0        0        0     2200 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/background_tasks.py
+-rw-r--r--   0        0        0        0 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/cli/__init__.py
+-rw-r--r--   0        0        0    11640 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/cli/_utils.py
+-rw-r--r--   0        0        0        0 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/cli/commands/__init__.py
+-rw-r--r--   0        0        0     4553 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/cli/commands/core.py
+-rw-r--r--   0        0        0     2365 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/cli/commands/schema.py
+-rw-r--r--   0        0        0     2224 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/cli/commands/sessions.py
+-rw-r--r--   0        0        0      807 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/cli/main.py
+-rw-r--r--   0        0        0        0 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/config/__init__.py
+-rw-r--r--   0        0        0     1747 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/config/allowed_hosts.py
+-rw-r--r--   0        0        0    12358 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/config/app.py
+-rw-r--r--   0        0        0     2742 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/config/compression.py
+-rw-r--r--   0        0        0     5177 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/config/cors.py
+-rw-r--r--   0        0        0     1771 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/config/csrf.py
+-rw-r--r--   0        0        0     1991 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/config/response_cache.py
+-rw-r--r--   0        0        0     1922 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/connection/__init__.py
+-rw-r--r--   0        0        0    10832 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/connection/base.py
+-rw-r--r--   0        0        0     7698 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/connection/request.py
+-rw-r--r--   0        0        0     8999 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/connection/websocket.py
+-rw-r--r--   0        0        0     1098 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/constants.py
+-rw-r--r--   0        0        0        0 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/htmx/__init__.py
+-rw-r--r--   0        0        0     4917 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/htmx/_utils.py
+-rw-r--r--   0        0        0     4051 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/htmx/request.py
+-rw-r--r--   0        0        0     8324 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/htmx/response.py
+-rw-r--r--   0        0        0     1261 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/htmx/types.py
+-rw-r--r--   0        0        0     2557 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/jinja.py
+-rw-r--r--   0        0        0      521 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/jwt/__init__.py
+-rw-r--r--   0        0        0    28720 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/jwt/jwt_auth.py
+-rw-r--r--   0        0        0     3978 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/jwt/jwt_token.py
+-rw-r--r--   0        0        0     6970 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/jwt/middleware.py
+-rw-r--r--   0        0        0     3916 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/mako.py
+-rw-r--r--   0        0        0        0 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/msgspec/__init__.py
+-rw-r--r--   0        0        0      180 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/opentelemetry/__init__.py
+-rw-r--r--   0        0        0      845 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/opentelemetry/_utils.py
+-rw-r--r--   0        0        0     4206 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/opentelemetry/config.py
+-rw-r--r--   0        0        0     2206 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/opentelemetry/middleware.py
+-rw-r--r--   0        0        0        0 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/pydantic/__init__.py
+-rw-r--r--   0        0        0      290 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/repository/__init__.py
+-rw-r--r--   0        0        0     9259 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/repository/abc.py
+-rw-r--r--   0        0        0      328 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/repository/exceptions.py
+-rw-r--r--   0        0        0     1785 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/repository/filters.py
+-rw-r--r--   0        0        0        0 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/repository/testing/__init__.py
+-rw-r--r--   0        0        0    13409 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/repository/testing/generic_mock_repository.py
+-rw-r--r--   0        0        0        0 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     3984 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/sqlalchemy/base.py
+-rw-r--r--   0        0        0     3431 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/sqlalchemy/dto.py
+-rw-r--r--   0        0        0      742 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/sqlalchemy/plugins/__init__.py
+-rw-r--r--   0        0        0      319 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/sqlalchemy/plugins/_slots_base.py
+-rw-r--r--   0        0        0      504 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/sqlalchemy/plugins/init/__init__.py
+-rw-r--r--   0        0        0      458 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/sqlalchemy/plugins/init/config/__init__.py
+-rw-r--r--   0        0        0     3602 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py
+-rw-r--r--   0        0        0    11308 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/sqlalchemy/plugins/init/config/common.py
+-rw-r--r--   0        0        0    11500 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/sqlalchemy/plugins/init/config/engine.py
+-rw-r--r--   0        0        0     2849 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/sqlalchemy/plugins/init/config/sync.py
+-rw-r--r--   0        0        0     1600 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/sqlalchemy/plugins/init/plugin.py
+-rw-r--r--   0        0        0     1447 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/sqlalchemy/plugins/serialization.py
+-rw-r--r--   0        0        0    21853 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/sqlalchemy/repository.py
+-rw-r--r--   0        0        0     1856 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/contrib/sqlalchemy/types.py
+-rw-r--r--   0        0        0     9559 2023-04-26 13:40:53.133600 litestar-2.0.0a5/litestar/controller.py
+-rw-r--r--   0        0        0    16460 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/data_extractors.py
+-rw-r--r--   0        0        0      883 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/datastructures/__init__.py
+-rw-r--r--   0        0        0     3757 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/datastructures/cookie.py
+-rw-r--r--   0        0        0    17316 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/datastructures/headers.py
+-rw-r--r--   0        0        0     2977 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/datastructures/multi_dicts.py
+-rw-r--r--   0        0        0     5027 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/datastructures/response_header.py
+-rw-r--r--   0        0        0     9302 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/datastructures/state.py
+-rw-r--r--   0        0        0     3360 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/datastructures/upload_file.py
+-rw-r--r--   0        0        0     7273 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/datastructures/url.py
+-rw-r--r--   0        0        0     2386 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/di.py
+-rw-r--r--   0        0        0        0 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/__init__.py
+-rw-r--r--   0        0        0      337 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/exceptions.py
+-rw-r--r--   0        0        0      188 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/factory/__init__.py
+-rw-r--r--   0        0        0    11610 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/factory/abc.py
+-rw-r--r--   0        0        0      245 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/factory/backends/__init__.py
+-rw-r--r--   0        0        0     4354 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/factory/backends/abc.py
+-rw-r--r--   0        0        0        0 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/factory/backends/msgspec/__init__.py
+-rw-r--r--   0        0        0     2427 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/factory/backends/msgspec/backend.py
+-rw-r--r--   0        0        0     7436 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/factory/backends/msgspec/utils.py
+-rw-r--r--   0        0        0        0 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/factory/backends/pydantic/__init__.py
+-rw-r--r--   0        0        0     2187 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/factory/backends/pydantic/backend.py
+-rw-r--r--   0        0        0     4163 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/factory/backends/pydantic/utils.py
+-rw-r--r--   0        0        0      866 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/factory/backends/utils.py
+-rw-r--r--   0        0        0      658 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/factory/config.py
+-rw-r--r--   0        0        0      313 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/factory/exc.py
+-rw-r--r--   0        0        0     1269 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/factory/field.py
+-rw-r--r--   0        0        0     2201 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/factory/stdlib/dataclass.py
+-rw-r--r--   0        0        0     2374 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/factory/types.py
+-rw-r--r--   0        0        0     1594 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/factory/utils.py
+-rw-r--r--   0        0        0     4368 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/interface.py
+-rw-r--r--   0        0        0      309 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/dto/types.py
+-rw-r--r--   0        0        0     1728 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/enums.py
+-rw-r--r--   0        0        0      201 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/events/__init__.py
+-rw-r--r--   0        0        0     4597 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/events/emitter.py
+-rw-r--r--   0        0        0     1305 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/events/listener.py
+-rw-r--r--   0        0        0     1142 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/exceptions/__init__.py
+-rw-r--r--   0        0        0     1621 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/exceptions/base_exceptions.py
+-rw-r--r--   0        0        0     4629 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/exceptions/http_exceptions.py
+-rw-r--r--   0        0        0     1351 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/exceptions/websocket_exceptions.py
+-rw-r--r--   0        0        0     5330 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/file_system.py
+-rw-r--r--   0        0        0      559 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/handlers/__init__.py
+-rw-r--r--   0        0        0     3877 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/handlers/asgi_handlers.py
+-rw-r--r--   0        0        0    20202 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/handlers/base.py
+-rw-r--r--   0        0        0      263 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/handlers/http_handlers/__init__.py
+-rw-r--r--   0        0        0     8104 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/handlers/http_handlers/_utils.py
+-rw-r--r--   0        0        0    25662 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/handlers/http_handlers/base.py
+-rw-r--r--   0        0        0    60867 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/handlers/http_handlers/decorators.py
+-rw-r--r--   0        0        0      340 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/handlers/websocket_handlers/__init__.py
+-rw-r--r--   0        0        0     6502 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/handlers/websocket_handlers/_utils.py
+-rw-r--r--   0        0        0    12896 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/handlers/websocket_handlers/listener.py
+-rw-r--r--   0        0        0     3619 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/handlers/websocket_handlers/route_handler.py
+-rw-r--r--   0        0        0      147 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/logging/__init__.py
+-rw-r--r--   0        0        0      569 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/logging/_utils.py
+-rw-r--r--   0        0        0    12050 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/logging/config.py
+-rw-r--r--   0        0        0     1129 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/logging/picologging.py
+-rw-r--r--   0        0        0      860 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/logging/standard.py
+-rw-r--r--   0        0        0      385 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/__init__.py
+-rw-r--r--   0        0        0     2081 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/_utils.py
+-rw-r--r--   0        0        0     2967 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/allowed_hosts.py
+-rw-r--r--   0        0        0     3430 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/authentication.py
+-rw-r--r--   0        0        0     5284 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/base.py
+-rw-r--r--   0        0        0     8359 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/compression.py
+-rw-r--r--   0        0        0     2565 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/cors.py
+-rw-r--r--   0        0        0     6466 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/csrf.py
+-rw-r--r--   0        0        0      124 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/exceptions/__init__.py
+-rw-r--r--   0        0        0     7191 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/exceptions/_debug_response.py
+-rw-r--r--   0        0        0     8990 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/exceptions/middleware.py
+-rw-r--r--   0        0        0      398 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/exceptions/templates/body.html
+-rw-r--r--   0        0        0      344 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/exceptions/templates/frame.html
+-rw-r--r--   0        0        0      920 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/exceptions/templates/scripts.js
+-rw-r--r--   0        0        0     1830 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/exceptions/templates/styles.css
+-rw-r--r--   0        0        0    13372 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/logging.py
+-rw-r--r--   0        0        0    10811 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/rate_limit.py
+-rw-r--r--   0        0        0       70 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/session/__init__.py
+-rw-r--r--   0        0        0     7935 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/session/base.py
+-rw-r--r--   0        0        0    10365 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/session/client_side.py
+-rw-r--r--   0        0        0     8558 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/middleware/session/server_side.py
+-rw-r--r--   0        0        0      231 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/openapi/__init__.py
+-rw-r--r--   0        0        0     5226 2023-04-26 13:40:53.137600 litestar-2.0.0a5/litestar/openapi/config.py
+-rw-r--r--   0        0        0    16443 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/controller.py
+-rw-r--r--   0        0        0      898 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/datastructures.py
+-rw-r--r--   0        0        0     1691 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/__init__.py
+-rw-r--r--   0        0        0     1648 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/base.py
+-rw-r--r--   0        0        0      961 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/callback.py
+-rw-r--r--   0        0        0     2936 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/components.py
+-rw-r--r--   0        0        0      592 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/contact.py
+-rw-r--r--   0        0        0      950 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/discriminator.py
+-rw-r--r--   0        0        0     3290 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/encoding.py
+-rw-r--r--   0        0        0      974 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/enums.py
+-rw-r--r--   0        0        0     1168 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/example.py
+-rw-r--r--   0        0        0      614 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/external_documentation.py
+-rw-r--r--   0        0        0     5669 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/header.py
+-rw-r--r--   0        0        0     1413 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/info.py
+-rw-r--r--   0        0        0      752 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/license.py
+-rw-r--r--   0        0        0     2876 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/link.py
+-rw-r--r--   0        0        0     1882 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/media_type.py
+-rw-r--r--   0        0        0     1195 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/oauth_flow.py
+-rw-r--r--   0        0        0      897 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/oauth_flows.py
+-rw-r--r--   0        0        0     4218 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/open_api.py
+-rw-r--r--   0        0        0     4842 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/operation.py
+-rw-r--r--   0        0        0     6242 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/parameter.py
+-rw-r--r--   0        0        0     3245 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/path_item.py
+-rw-r--r--   0        0        0     1255 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/paths.py
+-rw-r--r--   0        0        0     1351 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/reference.py
+-rw-r--r--   0        0        0     1095 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/request_body.py
+-rw-r--r--   0        0        0     1854 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/response.py
+-rw-r--r--   0        0        0     2367 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/responses.py
+-rw-r--r--   0        0        0    34574 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/schema.py
+-rw-r--r--   0        0        0     1686 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/security_requirement.py
+-rw-r--r--   0        0        0     2690 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/security_scheme.py
+-rw-r--r--   0        0        0     1077 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/server.py
+-rw-r--r--   0        0        0     1171 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/server_variable.py
+-rw-r--r--   0        0        0      923 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/tag.py
+-rw-r--r--   0        0        0     1702 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/openapi/spec/xml.py
+-rw-r--r--   0        0        0    10984 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/pagination.py
+-rw-r--r--   0        0        0    16805 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/params.py
+-rw-r--r--   0        0        0     7100 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/partial.py
+-rw-r--r--   0        0        0     3926 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/plugins.py
+-rw-r--r--   0        0        0        0 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/py.typed
+-rw-r--r--   0        0        0      278 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/response/__init__.py
+-rw-r--r--   0        0        0    12173 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/response/base.py
+-rw-r--r--   0        0        0     9225 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/response/file.py
+-rw-r--r--   0        0        0     2952 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/response/redirect.py
+-rw-r--r--   0        0        0     4883 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/response/streaming.py
+-rw-r--r--   0        0        0     2994 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/response/template.py
+-rw-r--r--   0        0        0    14975 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/response_containers.py
+-rw-r--r--   0        0        0    15028 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/router.py
+-rw-r--r--   0        0        0      191 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/routes/__init__.py
+-rw-r--r--   0        0        0     1757 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/routes/asgi.py
+-rw-r--r--   0        0        0     6437 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/routes/base.py
+-rw-r--r--   0        0        0    13254 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/routes/http.py
+-rw-r--r--   0        0        0     3052 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/routes/websocket.py
+-rw-r--r--   0        0        0       97 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/security/__init__.py
+-rw-r--r--   0        0        0     7165 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/security/base.py
+-rw-r--r--   0        0        0      188 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/security/session_auth/__init__.py
+-rw-r--r--   0        0        0     5602 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/security/session_auth/auth.py
+-rw-r--r--   0        0        0     4933 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/security/session_auth/middleware.py
+-rw-r--r--   0        0        0     7355 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/serialization.py
+-rw-r--r--   0        0        0      158 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/static_files/__init__.py
+-rw-r--r--   0        0        0     5019 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/static_files/base.py
+-rw-r--r--   0        0        0     3582 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/static_files/config.py
+-rw-r--r--   0        0        0     9536 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/status_codes.py
+-rw-r--r--   0        0        0        0 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/stores/__init__.py
+-rw-r--r--   0        0        0     4377 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/stores/base.py
+-rw-r--r--   0        0        0     5425 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/stores/file.py
+-rw-r--r--   0        0        0     3625 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/stores/memory.py
+-rw-r--r--   0        0        0     6231 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/stores/redis.py
+-rw-r--r--   0        0        0     2233 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/stores/registry.py
+-rw-r--r--   0        0        0      204 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/template/__init__.py
+-rw-r--r--   0        0        0     4113 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/template/base.py
+-rw-r--r--   0        0        0     1894 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/template/config.py
+-rw-r--r--   0        0        0      581 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/testing/__init__.py
+-rw-r--r--   0        0        0     1816 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/testing/client/__init__.py
+-rw-r--r--   0        0        0    17445 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/testing/client/async_client.py
+-rw-r--r--   0        0        0     5132 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/testing/client/base.py
+-rw-r--r--   0        0        0    19555 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/testing/client/sync_client.py
+-rw-r--r--   0        0        0    31473 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/testing/helpers.py
+-rw-r--r--   0        0        0     2532 2023-04-26 13:40:53.141600 litestar-2.0.0a5/litestar/testing/life_span_handler.py
+-rw-r--r--   0        0        0    21905 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/testing/request_factory.py
+-rw-r--r--   0        0        0     8086 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/testing/transport.py
+-rw-r--r--   0        0        0     6939 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/testing/websocket_test_session.py
+-rw-r--r--   0        0        0     4105 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/types/__init__.py
+-rw-r--r--   0        0        0     8697 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/types/asgi_types.py
+-rw-r--r--   0        0        0      453 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/types/builtin_types.py
+-rw-r--r--   0        0        0     2291 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/types/callable_types.py
+-rw-r--r--   0        0        0     1645 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/types/composite_types.py
+-rw-r--r--   0        0        0      183 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/types/empty.py
+-rw-r--r--   0        0        0     2662 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/types/file_types.py
+-rw-r--r--   0        0        0      344 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/types/helper_types.py
+-rw-r--r--   0        0        0     1720 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/types/internal_types.py
+-rw-r--r--   0        0        0     2607 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/types/protocols.py
+-rw-r--r--   0        0        0     1820 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/types/serialization.py
+-rw-r--r--   0        0        0     1906 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/utils/__init__.py
+-rw-r--r--   0        0        0      729 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/utils/compat.py
+-rw-r--r--   0        0        0     3578 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/utils/dataclass.py
+-rw-r--r--   0        0        0     3520 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/utils/deprecation.py
+-rw-r--r--   0        0        0     1483 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/utils/helpers.py
+-rw-r--r--   0        0        0      723 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/utils/path.py
+-rw-r--r--   0        0        0    10434 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/utils/predicates.py
+-rw-r--r--   0        0        0     2720 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/utils/scope.py
+-rw-r--r--   0        0        0     1003 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/utils/sequence.py
+-rw-r--r--   0        0        0    13407 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/utils/signature.py
+-rw-r--r--   0        0        0     5337 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/utils/sync.py
+-rw-r--r--   0        0        0     6405 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/utils/typing.py
+-rw-r--r--   0        0        0     1921 2023-04-26 13:40:53.145600 litestar-2.0.0a5/litestar/utils/version.py
+-rw-r--r--   0        0        0     9638 2023-04-26 13:40:53.145600 litestar-2.0.0a5/pyproject.toml
+-rw-r--r--   0        0        0    52838 1970-01-01 00:00:00.000000 litestar-2.0.0a5/PKG-INFO
```

### Comparing `litestar-2.0.0a4/LICENSE` & `litestar-2.0.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/README.md` & `litestar-2.0.0a5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)
 [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)
 [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)
 [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)
 
 <!-- prettier-ignore-start -->
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-95-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-97-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 <!-- prettier-ignore-end -->
 
-[![Reddit](https://img.shields.io/reddit/subreddit-subscribers/litestar?label=r%2FLitestar&logo=reddit)](https://reddit.com/r/litestar-api)
+[![Reddit](https://img.shields.io/reddit/subreddit-subscribers/litestarapi?label=r%2FLitestar&logo=reddit)](https://reddit.com/r/litestarapi)
 [![Discord](https://img.shields.io/discord/919193495116337154?color=blue&label=chat%20on%20discord&logo=discord)](https://discord.gg/X3FJqy8d2j)
 [![Matrix](https://img.shields.io/badge/%5Bm%5D%20chat%20on%20Matrix-bridged-blue)](https://matrix.to/#/#litestar:matrix.org)
 [![Medium](https://img.shields.io/badge/Medium-12100E?style=flat&logo=medium&logoColor=white)](https://blog.litestar.dev)
 
 </div>
 
 # Starlite → Litestar
@@ -354,15 +354,15 @@
       <td align="center" valign="top" width="14.28%"><a href="http://mookrs.com"><img src="https://avatars.githubusercontent.com/u/985439?v=4?s=100" width="100px;" alt="mookrs"/><br /><sub><b>mookrs</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=mookrs" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://mike.depalatis.net"><img src="https://avatars.githubusercontent.com/u/2805515?v=4?s=100" width="100px;" alt="Mike DePalatis"/><br /><sub><b>Mike DePalatis</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=mivade" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/pemocarlo"><img src="https://avatars.githubusercontent.com/u/7297323?v=4?s=100" width="100px;" alt="Carlos Alberto Pérez-Molano"/><br /><sub><b>Carlos Alberto Pérez-Molano</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=pemocarlo" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://www.bestcryptocodes.com"><img src="https://avatars.githubusercontent.com/u/114229148?v=4?s=100" width="100px;" alt="ThinksFast"/><br /><sub><b>ThinksFast</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=ThinksFast" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/litestar/commits?author=ThinksFast" title="Documentation">📖</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/ottermata"><img src="https://avatars.githubusercontent.com/u/9451844?v=4?s=100" width="100px;" alt="Christopher Krause"/><br /><sub><b>Christopher Krause</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=ottermata" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="http://www.kylesmith.me"><img src="https://avatars.githubusercontent.com/u/1161424?v=4?s=100" width="100px;" alt="Kyle Smith"/><br /><sub><b>Kyle Smith</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=smithk86" title="Code">💻</a> <a href="https://github.com/litestar-org/litestar/commits?author=smithk86" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="http://www.kylesmith.me"><img src="https://avatars.githubusercontent.com/u/1161424?v=4?s=100" width="100px;" alt="Kyle Smith"/><br /><sub><b>Kyle Smith</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=smithk86" title="Code">💻</a> <a href="https://github.com/litestar-org/litestar/commits?author=smithk86" title="Documentation">📖</a> <a href="https://github.com/litestar-org/litestar/issues?q=author%3Asmithk86" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/scott2b"><img src="https://avatars.githubusercontent.com/u/307713?v=4?s=100" width="100px;" alt="Scott Bradley"/><br /><sub><b>Scott Bradley</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/issues?q=author%3Ascott2b" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://www.linkedin.com/in/srikanthccv/"><img src="https://avatars.githubusercontent.com/u/22846633?v=4?s=100" width="100px;" alt="Srikanth Chekuri"/><br /><sub><b>Srikanth Chekuri</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=srikanthccv" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/litestar/commits?author=srikanthccv" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://lonelyviking.com"><img src="https://avatars.githubusercontent.com/u/78952809?v=4?s=100" width="100px;" alt="Michael Bosch"/><br /><sub><b>Michael Bosch</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=LonelyVikingMichael" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/sssssss340"><img src="https://avatars.githubusercontent.com/u/8406195?v=4?s=100" width="100px;" alt="sssssss340"/><br /><sub><b>sssssss340</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/issues?q=author%3Asssssss340" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/ste-pool"><img src="https://avatars.githubusercontent.com/u/17198460?v=4?s=100" width="100px;" alt="ste-pool"/><br /><sub><b>ste-pool</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=ste-pool" title="Code">💻</a> <a href="#infra-ste-pool" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a></td>
     </tr>
     <tr>
@@ -398,18 +398,20 @@
       <td align="center" valign="top" width="14.28%"><a href="https://gh.arielle.codes"><img src="https://avatars.githubusercontent.com/u/71233171?v=4?s=100" width="100px;" alt="arl"/><br /><sub><b>arl</b></sub></a><br /><a href="#maintenance-onerandomusername" title="Maintenance">🚧</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Galdanwing"><img src="https://avatars.githubusercontent.com/u/29492757?v=4?s=100" width="100px;" alt="Antoine van der Horst"/><br /><sub><b>Antoine van der Horst</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=Galdanwing" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://nick.groenen.me"><img src="https://avatars.githubusercontent.com/u/145285?v=4?s=100" width="100px;" alt="Nick Groenen"/><br /><sub><b>Nick Groenen</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=zoni" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/giorgiovilardo"><img src="https://avatars.githubusercontent.com/u/56472600?v=4?s=100" width="100px;" alt="Giorgio Vilardo"/><br /><sub><b>Giorgio Vilardo</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=giorgiovilardo" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/bollwyvl"><img src="https://avatars.githubusercontent.com/u/45380?v=4?s=100" width="100px;" alt="Nicholas Bollweg"/><br /><sub><b>Nicholas Bollweg</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=bollwyvl" title="Code">💻</a></td>
     </tr>
     <tr>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/tompin82"><img src="https://avatars.githubusercontent.com/u/47041409?v=4?s=100" width="100px;" alt="Tomas Jonsson"/><br /><sub><b>Tomas Jonsson</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=tompin82" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/tompin82"><img src="https://avatars.githubusercontent.com/u/47041409?v=4?s=100" width="100px;" alt="Tomas Jonsson"/><br /><sub><b>Tomas Jonsson</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=tompin82" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/litestar/commits?author=tompin82" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://www.linkedin.com/in/khiem-doan/"><img src="https://avatars.githubusercontent.com/u/15646249?v=4?s=100" width="100px;" alt="Khiem Doan"/><br /><sub><b>Khiem Doan</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=khiemdoan" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/kedod"><img src="https://avatars.githubusercontent.com/u/35638715?v=4?s=100" width="100px;" alt="kedod"/><br /><sub><b>kedod</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=kedod" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/sonpro1296"><img src="https://avatars.githubusercontent.com/u/17319142?v=4?s=100" width="100px;" alt="sonpro1296"/><br /><sub><b>sonpro1296</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=sonpro1296" title="Code">💻</a> <a href="https://github.com/litestar-org/litestar/commits?author=sonpro1296" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://patrickarmengol.com"><img src="https://avatars.githubusercontent.com/u/42473149?v=4?s=100" width="100px;" alt="Patrick Armengol"/><br /><sub><b>Patrick Armengol</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=patrickarmengol" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://sanderwegter.nl"><img src="https://avatars.githubusercontent.com/u/7465799?v=4?s=100" width="100px;" alt="Sander"/><br /><sub><b>Sander</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=SanderWegter" title="Documentation">📖</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

### Comparing `litestar-2.0.0a4/litestar/__init__.py` & `litestar-2.0.0a5/litestar/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/_asgi/asgi_router.py` & `litestar-2.0.0a5/litestar/_asgi/asgi_router.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         self._plain_routes: set[str] = set()
         self._registered_routes: set[HTTPRoute | WebSocketRoute | ASGIRoute] = set()
         self.app = app
         self.root_route_map_node: RouteTrieNode = create_node()
         self.route_handler_index: dict[str, RouteHandlerType] = {}
         self.route_mapping: dict[str, list[BaseRoute]] = defaultdict(list)
 
-    async def __call__(self, scope: "Scope", receive: "Receive", send: "Send") -> None:
+    async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
         """ASGI callable.
 
         The main entry point to the Router class.
         """
         scope.setdefault("path_params", {})
         normalized_path = normalize_path(scope["path"])
         asgi_app, scope["route_handler"], scope["path"], scope["path_params"] = self.handle_routing(
@@ -119,15 +119,15 @@
                 raise ImproperlyConfiguredException(
                     f"route handler names must be unique - {handler.name} is not unique."
                 )
             identifier = handler.name or str(handler)
             self.route_mapping[identifier].append(route)
             self.route_handler_index[identifier] = handler
 
-    async def _call_lifespan_handler(self, handler: "LifeSpanHandler") -> None:
+    async def _call_lifespan_handler(self, handler: LifeSpanHandler) -> None:
         """Determine whether the lifecycle handler expects an argument, and if so pass the `app.state` to it. If the
         handler is an async function, await the return.
 
         Args:
             handler: sync or async callable that may or may not have an argument.
         """
         async_callable = AsyncCallable(handler)  # type: ignore
@@ -154,15 +154,15 @@
             self._store_handler_to_route_mapping(route)
             self._registered_routes.add(route)
 
         validate_node(node=self.root_route_map_node)
         if self._mount_routes:
             self._mount_paths_regex = re.compile("|".join(sorted(set(self._mount_routes))))  # pyright: ignore
 
-    async def lifespan(self, receive: "LifeSpanReceive", send: "LifeSpanSend") -> None:
+    async def lifespan(self, receive: LifeSpanReceive, send: LifeSpanSend) -> None:
         """Handle the ASGI "lifespan" event on application startup and shutdown.
 
         Args:
             receive: The ASGI receive function.
             send: The ASGI send function.
 
         Returns:
```

### Comparing `litestar-2.0.0a4/litestar/_asgi/routing_trie/mapping.py` & `litestar-2.0.0a5/litestar/_asgi/routing_trie/mapping.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/_asgi/routing_trie/traversal.py` & `litestar-2.0.0a5/litestar/_asgi/routing_trie/traversal.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/_asgi/routing_trie/types.py` & `litestar-2.0.0a5/litestar/_asgi/routing_trie/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/_asgi/routing_trie/validate.py` & `litestar-2.0.0a5/litestar/_asgi/routing_trie/validate.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/_asgi/utils.py` & `litestar-2.0.0a5/litestar/_asgi/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/_kwargs/cleanup.py` & `litestar-2.0.0a5/litestar/_kwargs/cleanup.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/_kwargs/dependencies.py` & `litestar-2.0.0a5/litestar/_kwargs/dependencies.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,18 +37,18 @@
         return other is self or (isinstance(other, self.__class__) and other.key == self.key)
 
     def __hash__(self) -> int:
         return hash(self.key)
 
 
 async def resolve_dependency(
-    dependency: "Dependency",
-    connection: "ASGIConnection",
+    dependency: Dependency,
+    connection: ASGIConnection,
     kwargs: dict[str, Any],
-    cleanup_group: "DependencyCleanupGroup",
+    cleanup_group: DependencyCleanupGroup,
 ) -> None:
     """Resolve a given instance of :class:`Dependency <litestar._kwargs.Dependency>`.
 
     All required sub dependencies must already
     be resolved into the kwargs. The result of the dependency will be stored in the kwargs.
 
     Args:
```

### Comparing `litestar-2.0.0a4/litestar/_kwargs/extractors.py` & `litestar-2.0.0a5/litestar/_kwargs/extractors.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 from litestar._multipart import parse_multipart_form
 from litestar._parsers import (
     parse_headers,
     parse_query_string,
     parse_url_encoded_form_data,
 )
 from litestar.datastructures.upload_file import UploadFile
-from litestar.dto.interface import DTOInterface
+from litestar.dto.interface import ConnectionContext
 from litestar.enums import ParamType, RequestEncodingType
 from litestar.exceptions import ValidationException
 from litestar.params import BodyKwarg
 from litestar.types import Empty
 
 if TYPE_CHECKING:
     from litestar._kwargs import KwargsModel
     from litestar._kwargs.parameter_definition import ParameterDefinition
     from litestar._signature.field import SignatureField
     from litestar.connection import ASGIConnection, Request
-    from litestar.utils.signature import ParsedParameter
+    from litestar.dto.interface import DTOInterface
 
 __all__ = (
     "body_extractor",
     "cookies_extractor",
     "create_connection_value_extractor",
     "create_data_extractor",
     "create_multipart_extractor",
@@ -284,31 +284,32 @@
     Returns:
         The MessagePack value.
     """
     return await connection.msgpack()
 
 
 def create_multipart_extractor(
-    signature_field: SignatureField, is_data_optional: bool
+    signature_field: SignatureField, is_data_optional: bool, dto_type: type[DTOInterface] | None
 ) -> Callable[[ASGIConnection[Any, Any, Any, Any]], Coroutine[Any, Any, Any]]:
     """Create a multipart form-data extractor.
 
     Args:
         signature_field: A SignatureField instance.
         is_data_optional: Boolean dictating whether the field is optional.
+        dto_type: The DTO type, if configured for handler.
 
     Returns:
         An extractor function.
     """
     body_kwarg_multipart_form_part_limit: int | None = None
     if signature_field.kwarg_model and isinstance(signature_field.kwarg_model, BodyKwarg):
         body_kwarg_multipart_form_part_limit = signature_field.kwarg_model.multipart_form_part_limit
 
     async def extract_multipart(
-        connection: "Request[Any, Any, Any]",
+        connection: Request[Any, Any, Any],
     ) -> Any:
         multipart_form_part_limit = (
             body_kwarg_multipart_form_part_limit
             if body_kwarg_multipart_form_part_limit is not None
             else connection.app.multipart_form_part_limit
         )
         connection.scope["_form"] = form_values = (  # type: ignore[typeddict-unknown-key]
@@ -322,40 +323,55 @@
         )
 
         if signature_field.is_non_string_sequence:
             return list(form_values.values())
         if signature_field.is_simple_type and signature_field.field_type is UploadFile and form_values:
             return [v for v in form_values.values() if isinstance(v, UploadFile)][0]
 
-        return form_values if form_values or not is_data_optional else None
+        if not form_values and is_data_optional:
+            return None
+
+        if dto_type:
+            ctx = ConnectionContext.from_connection(connection)
+            return dto_type(ctx).builtins_to_data_type(form_values)
+
+        return form_values
 
     return cast("Callable[[ASGIConnection[Any, Any, Any, Any]], Coroutine[Any, Any, Any]]", extract_multipart)
 
 
 def create_url_encoded_data_extractor(
-    is_data_optional: bool,
+    is_data_optional: bool, dto_type: type[DTOInterface] | None
 ) -> Callable[[ASGIConnection[Any, Any, Any, Any]], Coroutine[Any, Any, Any]]:
     """Create extractor for url encoded form-data.
 
     Args:
         is_data_optional: Boolean dictating whether the field is optional.
+        dto_type: The DTO type, if configured for handler.
 
     Returns:
         An extractor function.
     """
 
     async def extract_url_encoded_extractor(
-        connection: "Request[Any, Any, Any]",
+        connection: Request[Any, Any, Any],
     ) -> Any:
         connection.scope["_form"] = form_values = (  # type: ignore[typeddict-unknown-key]
             connection.scope["_form"]  # type: ignore[typeddict-item]
             if "_form" in connection.scope
             else parse_url_encoded_form_data(await connection.body())
         )
-        return form_values if form_values or not is_data_optional else None
+        if not form_values and is_data_optional:
+            return None
+
+        if dto_type:
+            ctx = ConnectionContext.from_connection(connection)
+            return dto_type(ctx).builtins_to_data_type(form_values)
+
+        return form_values
 
     return cast(
         "Callable[[ASGIConnection[Any, Any, Any, Any]], Coroutine[Any, Any, Any]]", extract_url_encoded_extractor
     )
 
 
 def create_data_extractor(kwargs_model: KwargsModel) -> Callable[[dict[str, Any], ASGIConnection], None]:
@@ -365,29 +381,32 @@
         kwargs_model: The KwargsModel instance.
 
     Returns:
         An extractor for the request's body.
     """
 
     if kwargs_model.expected_form_data:
-        media_type, signature_field = kwargs_model.expected_form_data
+        media_type, signature_field, dto_type = kwargs_model.expected_form_data
 
         if media_type == RequestEncodingType.MULTI_PART:
             data_extractor = create_multipart_extractor(
                 signature_field=signature_field,
                 is_data_optional=kwargs_model.is_data_optional,
+                dto_type=dto_type,
             )
         else:
-            data_extractor = create_url_encoded_data_extractor(is_data_optional=kwargs_model.is_data_optional)
+            data_extractor = create_url_encoded_data_extractor(
+                is_data_optional=kwargs_model.is_data_optional, dto_type=dto_type
+            )
     elif kwargs_model.expected_msgpack_data:
         data_extractor = cast(
             "Callable[[ASGIConnection[Any, Any, Any, Any]], Coroutine[Any, Any, Any]]", msgpack_extractor
         )
     elif kwargs_model.expected_dto_data:
-        data_extractor = create_dto_extractor(*kwargs_model.expected_dto_data)
+        data_extractor = create_dto_extractor(kwargs_model.expected_dto_data)
     else:
         data_extractor = cast(
             "Callable[[ASGIConnection[Any, Any, Any, Any]], Coroutine[Any, Any, Any]]", json_extractor
         )
 
     def extractor(
         values: dict[str, Any],
@@ -395,27 +414,23 @@
     ) -> None:
         values["data"] = data_extractor(connection)
 
     return extractor
 
 
 def create_dto_extractor(
-    parsed_parameter: ParsedParameter, dto_type: type[DTOInterface]
+    dto_type: type[DTOInterface],
 ) -> Callable[[ASGIConnection[Any, Any, Any, Any]], Coroutine[Any, Any, Any]]:
     """Create a DTO data extractor.
 
     Args:
-        parsed_parameter: :class:`ParsedParameter` instance representing the ``"data"`` kwarg.
         dto_type: The :class:`DTOInterface` subclass.
 
     Returns:
         An extractor function.
     """
-    is_dto_annotated = parsed_parameter.parsed_type.is_subclass_of(DTOInterface)
 
     async def dto_extractor(connection: Request[Any, Any, Any]) -> Any:
-        dto = await dto_type.from_connection(connection)
-        if is_dto_annotated:
-            return dto
-        return dto.to_data_type()
+        ctx = ConnectionContext.from_connection(connection)
+        return dto_type(ctx).bytes_to_data_type(await connection.body())
 
     return dto_extractor  # type:ignore[return-value]
```

### Comparing `litestar-2.0.0a4/litestar/_kwargs/kwargs_model.py` & `litestar-2.0.0a5/litestar/_kwargs/kwargs_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,26 +28,26 @@
     ParameterDefinition,
     create_parameter_definition,
     merge_parameter_sets,
 )
 from litestar._signature import SignatureModel, get_signature_model
 from litestar._signature.field import SignatureField
 from litestar.constants import RESERVED_KWARGS
-from litestar.dto.interface import DTOInterface
 from litestar.enums import ParamType, RequestEncodingType
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.params import BodyKwarg, ParameterKwarg
 
 __all__ = ("KwargsModel",)
 
 
 if TYPE_CHECKING:
     from litestar.connection import ASGIConnection
     from litestar.di import Provide
-    from litestar.utils.signature import ParsedParameter, ParsedSignature
+    from litestar.dto.interface import DTOInterface
+    from litestar.utils.signature import ParsedSignature
 
 
 class KwargsModel:
     """Model required kwargs for a given RouteHandler and its dependencies.
 
     This is done once and is memoized during application bootstrap, ensuring minimal runtime overhead.
     """
@@ -68,17 +68,17 @@
         "sequence_query_parameter_names",
     )
 
     def __init__(
         self,
         *,
         expected_cookie_params: set[ParameterDefinition],
-        expected_dto_data: tuple[ParsedParameter, type[DTOInterface]] | None,
+        expected_dto_data: type[DTOInterface] | None,
         expected_dependencies: set[Dependency],
-        expected_form_data: tuple[RequestEncodingType | str, SignatureField] | None,
+        expected_form_data: tuple[RequestEncodingType | str, SignatureField, type[DTOInterface] | None] | None,
         expected_msgpack_data: SignatureField | None,
         expected_header_params: set[ParameterDefinition],
         expected_path_params: set[ParameterDefinition],
         expected_query_params: set[ParameterDefinition],
         expected_reserved_kwargs: set[str],
         sequence_query_parameter_names: set[str],
         is_data_optional: bool,
@@ -298,42 +298,32 @@
         expected_reserved_kwargs = {field_name for field_name in signature_fields if field_name in RESERVED_KWARGS}
         expected_path_parameters = {p for p in param_definitions if p.param_type == ParamType.PATH}
         expected_header_parameters = {p for p in param_definitions if p.param_type == ParamType.HEADER}
         expected_cookie_parameters = {p for p in param_definitions if p.param_type == ParamType.COOKIE}
         expected_query_parameters = {p for p in param_definitions if p.param_type == ParamType.QUERY}
         sequence_query_parameter_names = {p.field_alias for p in expected_query_parameters if p.is_sequence}
 
-        expected_form_data: tuple[RequestEncodingType | str, SignatureField] | None = None
+        expected_form_data: tuple[RequestEncodingType | str, SignatureField, type[DTOInterface] | None] | None = None
         expected_msgpack_data: SignatureField | None = None
-        expected_dto_data: tuple[ParsedParameter, type[DTOInterface]] | None = None
+        expected_dto_data: type[DTOInterface] | None = None
 
         data_signature_field = signature_fields.get("data")
 
         media_type: RequestEncodingType | str | None = None
         if data_signature_field and isinstance(data_signature_field.kwarg_model, BodyKwarg):
             media_type = data_signature_field.kwarg_model.media_type
 
-        if data_signature_field and media_type:
-            if media_type in (
-                RequestEncodingType.MULTI_PART,
-                RequestEncodingType.URL_ENCODED,
-            ):
-                expected_form_data = (media_type, data_signature_field)
-
+        if data_signature_field:
+            if media_type in (RequestEncodingType.MULTI_PART, RequestEncodingType.URL_ENCODED):
+                expected_form_data = (media_type, data_signature_field, data_dto)
+            elif data_dto:
+                expected_dto_data = data_dto
             elif media_type == RequestEncodingType.MESSAGEPACK:
                 expected_msgpack_data = data_signature_field
 
-        elif data_signature_field:
-            parsed_parameter = parsed_signature.parameters["data"]
-            parsed_type = parsed_parameter.parsed_type
-            if parsed_type.is_subclass_of(DTOInterface):
-                expected_dto_data = (parsed_parameter, parsed_type.annotation)
-            elif data_dto:
-                expected_dto_data = (parsed_parameter, data_dto)
-
         for dependency in expected_dependencies:
             dependency_kwargs_model = cls.create_for_signature_model(
                 signature_model=get_signature_model(dependency.provide),
                 parsed_signature=parsed_signature,
                 dependencies=dependencies,
                 path_parameters=path_parameters,
                 layered_parameters=layered_parameters,
@@ -389,17 +379,15 @@
         output: dict[str, Any] = {}
 
         for extractor in self.extractors:
             extractor(output, connection)
 
         return output
 
-    async def resolve_dependencies(
-        self, connection: "ASGIConnection", kwargs: dict[str, Any]
-    ) -> "DependencyCleanupGroup":
+    async def resolve_dependencies(self, connection: ASGIConnection, kwargs: dict[str, Any]) -> DependencyCleanupGroup:
         """Resolve all dependencies into the kwargs, recursively.
 
         Args:
             connection: An instance of :class:`Request <litestar.connection.Request>` or
                 :class:`WebSocket <litestar.connection.WebSocket>`.
             kwargs: Kwargs to pass to dependencies.
         """
@@ -425,25 +413,25 @@
             provide=provide,
             dependencies=[cls._create_dependency_graph(key=k, dependencies=dependencies) for k in sub_dependency_keys],
         )
 
     @classmethod
     def _validate_dependency_data(
         cls,
-        expected_form_data: tuple[RequestEncodingType | str, SignatureField] | None,
+        expected_form_data: tuple[RequestEncodingType | str, SignatureField, type[DTOInterface] | None] | None,
         dependency_kwargs_model: KwargsModel,
     ) -> None:
         """Validate that the 'data' kwarg is compatible across dependencies."""
         if bool(expected_form_data) != bool(dependency_kwargs_model.expected_form_data):
             raise ImproperlyConfiguredException(
                 "Dependencies have incompatible 'data' kwarg types: one expects JSON and the other expects form-data"
             )
         if expected_form_data and dependency_kwargs_model.expected_form_data:
-            local_media_type, _ = expected_form_data
-            dependency_media_type, _ = dependency_kwargs_model.expected_form_data
+            local_media_type = expected_form_data[0]
+            dependency_media_type = dependency_kwargs_model.expected_form_data[0]
             if local_media_type != dependency_media_type:
                 raise ImproperlyConfiguredException(
                     "Dependencies have incompatible form-data encoding: one expects url-encoded and the other expects multi-part"
                 )
 
     @classmethod
     def _validate_raw_kwargs(
```

### Comparing `litestar-2.0.0a4/litestar/_kwargs/parameter_definition.py` & `litestar-2.0.0a5/litestar/_kwargs/parameter_definition.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/_layers/utils.py` & `litestar-2.0.0a5/litestar/_layers/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/_multipart.py` & `litestar-2.0.0a5/litestar/_multipart.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/_openapi/parameters.py` & `litestar-2.0.0a5/litestar/_openapi/parameters.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,16 +26,16 @@
     from litestar.handlers.base import BaseRouteHandler
     from litestar.openapi.spec import Reference
     from litestar.types import Dependencies
     from litestar.types.internal_types import PathParameterDefinition
 
 
 def create_path_parameter_schema(
-    path_parameter: "PathParameterDefinition",
-    field: "SignatureField",
+    path_parameter: PathParameterDefinition,
+    field: SignatureField,
     generate_examples: bool,
     schemas: dict[str, Schema],
 ) -> Schema | Reference:
     """Create a path parameter from the given path_param definition."""
     return create_schema(
         field=SignatureField(
             children=None,
@@ -55,15 +55,15 @@
     """Facilitates conditional deduplication of parameters.
 
     If multiple parameters with the same name are produced for a handler, the condition is ignored if the two
     ``Parameter`` instances are the same (the first is retained and any duplicates are ignored). If the ``Parameter``
     instances are not the same, an exception is raised.
     """
 
-    def __init__(self, route_handler: "BaseRouteHandler") -> None:
+    def __init__(self, route_handler: BaseRouteHandler) -> None:
         """Initialize ``ParameterCollection``.
 
         Args:
             route_handler: Associated route handler
         """
         self.route_handler = route_handler
         self._parameters: dict[str, Parameter] = {}
@@ -92,19 +92,19 @@
 
     def list(self) -> list[Parameter]:
         """Return a list of all ``Parameter``'s in the collection."""
         return list(self._parameters.values())
 
 
 def create_parameter(
-    signature_field: "SignatureField",
+    signature_field: SignatureField,
     parameter_name: str,
-    path_parameters: tuple["PathParameterDefinition", ...],
+    path_parameters: tuple[PathParameterDefinition, ...],
     generate_examples: bool,
-    schemas: dict[str, "Schema"],
+    schemas: dict[str, Schema],
 ) -> Parameter:
     """Create an OpenAPI Parameter instance."""
     result: Schema | Reference | None = None
     kwargs_model = signature_field.kwarg_model if isinstance(signature_field.kwarg_model, ParameterKwarg) else None
 
     if any(path_param.name == parameter_name for path_param in path_parameters):
         param_in = ParamType.PATH
@@ -139,20 +139,20 @@
         required=is_required,
         schema=result,
     )
 
 
 def get_recursive_handler_parameters(
     field_name: str,
-    signature_field: "SignatureField",
-    dependencies: "Dependencies",
-    route_handler: "BaseRouteHandler",
-    path_parameters: tuple["PathParameterDefinition", ...],
+    signature_field: SignatureField,
+    dependencies: Dependencies,
+    route_handler: BaseRouteHandler,
+    path_parameters: tuple[PathParameterDefinition, ...],
     generate_examples: bool,
-    schemas: dict[str, "Schema"],
+    schemas: dict[str, Schema],
 ) -> list[Parameter]:
     """Create and return parameters for a handler.
 
     If the provided field is not a dependency, a normal parameter is created and returned as a list, otherwise
     `create_parameter_for_handler()` is called to generate parameters for the dependency.
     """
 
@@ -170,19 +170,19 @@
     return create_parameter_for_handler(
         route_handler, dependency_fields, path_parameters, generate_examples, schemas=schemas
     )
 
 
 def get_layered_parameter(
     field_name: str,
-    signature_field: "SignatureField",
-    layered_parameters: dict[str, "SignatureField"],
-    path_parameters: tuple["PathParameterDefinition", ...],
+    signature_field: SignatureField,
+    layered_parameters: dict[str, SignatureField],
+    path_parameters: tuple[PathParameterDefinition, ...],
     generate_examples: bool,
-    schemas: dict[str, "Schema"],
+    schemas: dict[str, Schema],
 ) -> Parameter:
     """Create a layered parameter for a given signature model field.
 
     Layer info is extracted from the provided ``layered_parameters`` dict and set as the field's ``field_info`` attribute.
     """
     layer_field = layered_parameters[field_name]
 
@@ -207,19 +207,19 @@
         parameter_name=parameter_name,
         path_parameters=path_parameters,
         schemas=schemas,
     )
 
 
 def create_parameter_for_handler(
-    route_handler: "BaseRouteHandler",
-    handler_fields: dict[str, "SignatureField"],
-    path_parameters: tuple["PathParameterDefinition", ...],
+    route_handler: BaseRouteHandler,
+    handler_fields: dict[str, SignatureField],
+    path_parameters: tuple[PathParameterDefinition, ...],
     generate_examples: bool,
-    schemas: dict[str, "Schema"],
+    schemas: dict[str, Schema],
 ) -> list[Parameter]:
     """Create a list of path/query/header Parameter models for the given PathHandler."""
     parameters = ParameterCollection(route_handler=route_handler)
     dependencies = route_handler.resolve_dependencies()
 
     layered_parameters = route_handler.resolve_layered_parameters()
```

### Comparing `litestar-2.0.0a4/litestar/_openapi/path_item.py` & `litestar-2.0.0a5/litestar/_openapi/path_item.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     from litestar.handlers.http_handlers import HTTPRouteHandler
     from litestar.openapi.spec import Schema, SecurityRequirement
     from litestar.plugins import OpenAPISchemaPluginProtocol
     from litestar.routes import HTTPRoute
     from litestar.types.callable_types import OperationIDCreator
 
 
-def get_description_for_handler(route_handler: "HTTPRouteHandler", use_handler_docstrings: bool) -> str | None:
+def get_description_for_handler(route_handler: HTTPRouteHandler, use_handler_docstrings: bool) -> str | None:
     """Produce the operation description for a route handler, either by using the description value if provided,
 
     or the docstring - if config is enabled.
 
     Args:
         route_handler: A route handler instance.
         use_handler_docstrings: If ``True`` and `route_handler.description`` is ``None` returns docstring of wrapped
@@ -39,40 +39,40 @@
     if handler_description is None and use_handler_docstrings:
         fn = unwrap_partial(route_handler.fn.value)
         return cleandoc(fn.__doc__) if fn.__doc__ else None
     return handler_description
 
 
 def extract_layered_values(
-    route_handler: "HTTPRouteHandler",
+    route_handler: HTTPRouteHandler,
 ) -> tuple[list[str] | None, list[dict[str, list[str]]] | None]:
     """Extract the tags and security values from the route handler layers.
 
     Args:
         route_handler: A Route Handler instance.
 
     Returns:
         A tuple of optional lists.
     """
     tags: list[str] = []
-    security: list["SecurityRequirement"] = []
+    security: list[SecurityRequirement] = []
     for layer in route_handler.ownership_layers:
         if layer.tags:
             tags.extend(layer.tags)
         if layer.security:
             security.extend(layer.security)
     return sorted(set(tags)) if tags else None, security or None
 
 
 def create_path_item(
     create_examples: bool,
-    operation_id_creator: "OperationIDCreator",
-    plugins: list["OpenAPISchemaPluginProtocol"],
-    route: "HTTPRoute",
-    schemas: dict[str, "Schema"],
+    operation_id_creator: OperationIDCreator,
+    plugins: list[OpenAPISchemaPluginProtocol],
+    route: HTTPRoute,
+    schemas: dict[str, Schema],
     use_handler_docstrings: bool,
 ) -> tuple[PathItem, list[str]]:
     """Create a PathItem for the given route parsing all http_methods into Operation Models.
 
     Args:
         create_examples: Whether to auto-generate examples.
         operation_id_creator: A function to generate operation ids.
@@ -103,14 +103,15 @@
                 or None
             )
             raises_validation_error = bool("data" in handler_fields or path_item.parameters or parameters)
 
             request_body = None
             if "data" in handler_fields:
                 request_body = create_request_body(
+                    route_handler=route_handler,
                     field=handler_fields["data"],
                     generate_examples=create_examples,
                     plugins=plugins,
                     schemas=schemas,
                 )
             operation_id = route_handler.operation_id or operation_id_creator(
                 route_handler, http_method, route.path_components
```

### Comparing `litestar-2.0.0a4/litestar/_openapi/request_body.py` & `litestar-2.0.0a5/litestar/_openapi/request_body.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,24 +9,30 @@
 from litestar.params import BodyKwarg
 
 __all__ = ("create_request_body",)
 
 
 if TYPE_CHECKING:
     from litestar._signature.field import SignatureField
+    from litestar.handlers import BaseRouteHandler
     from litestar.openapi.spec import Schema
     from litestar.plugins import OpenAPISchemaPluginProtocol
 
 
 def create_request_body(
-    field: "SignatureField",
+    route_handler: BaseRouteHandler,
+    field: SignatureField,
     generate_examples: bool,
-    plugins: list["OpenAPISchemaPluginProtocol"],
-    schemas: dict[str, "Schema"],
+    plugins: list[OpenAPISchemaPluginProtocol],
+    schemas: dict[str, Schema],
 ) -> RequestBody | None:
     """Create a RequestBody model for the given RouteHandler or return None."""
     media_type: RequestEncodingType | str = RequestEncodingType.JSON
     if isinstance(field.kwarg_model, BodyKwarg) and field.kwarg_model.media_type:
         media_type = field.kwarg_model.media_type
 
-    schema = create_schema(field=field, generate_examples=generate_examples, plugins=plugins, schemas=schemas)
+    if dto := route_handler.resolve_dto():
+        schema = dto.create_openapi_schema("data", str(route_handler), generate_examples, schemas)
+    else:
+        schema = create_schema(field=field, generate_examples=generate_examples, plugins=plugins, schemas=schemas)
+
     return RequestBody(required=True, content={media_type: OpenAPIMediaType(schema=schema)})
```

### Comparing `litestar-2.0.0a4/litestar/_openapi/responses.py` & `litestar-2.0.0a5/litestar/_openapi/responses.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,34 +43,34 @@
 
 
 def pascal_case_to_text(string: str) -> str:
     """Given a 'PascalCased' string, return its split form- 'Pascal Cased'."""
     return " ".join(re.split(CAPITAL_LETTERS_PATTERN, string)).strip()
 
 
-def create_cookie_schema(cookie: "Cookie") -> Schema:
+def create_cookie_schema(cookie: Cookie) -> Schema:
     """Given a Cookie instance, return its corresponding OpenAPI schema.
 
     Args:
         cookie: Cookie
 
     Returns:
         Schema
     """
     cookie_copy = copy(cookie)
     cookie_copy.value = "<string>"
     value = cookie_copy.to_header(header="")
     return Schema(description=cookie.description or "", example=value)
 
 
-def create_success_response(
-    route_handler: "HTTPRouteHandler",
+def create_success_response(  # noqa: C901
+    route_handler: HTTPRouteHandler,
     generate_examples: bool,
-    plugins: list["OpenAPISchemaPluginProtocol"],
-    schemas: dict[str, "Schema"],
+    plugins: list[OpenAPISchemaPluginProtocol],
+    schemas: dict[str, Schema],
 ) -> OpenAPIResponse:
     """Create the schema for a success response."""
     return_annotation = route_handler.parsed_fn_signature.return_type.annotation
     default_descriptions: dict[Any, str] = {
         Stream: "Stream Response",
         Redirect: "Redirect Response",
         File: "File Download",
@@ -84,20 +84,23 @@
     if return_annotation not in {Signature.empty, None, NoneType, Redirect, File, Stream}:
         if return_annotation is Template:
             return_annotation = str
             route_handler.media_type = get_enum_string_value(MediaType.HTML)
         elif is_class_and_subclass(get_origin(return_annotation), LitestarResponse):
             return_annotation = get_args(return_annotation)[0] or Any
 
-        result = create_schema(
-            field=SignatureField.create(field_type=return_annotation),
-            generate_examples=generate_examples,
-            plugins=plugins,
-            schemas=schemas,
-        )
+        if dto := route_handler.resolve_return_dto():
+            result = dto.create_openapi_schema("return", str(route_handler), generate_examples, schemas)
+        else:
+            result = create_schema(
+                field=SignatureField.create(field_type=return_annotation),
+                generate_examples=generate_examples,
+                plugins=plugins,
+                schemas=schemas,
+            )
 
         schema = result if isinstance(result, Schema) else schemas[result.value]
 
         schema.content_encoding = route_handler.content_encoding
         schema.content_media_type = route_handler.content_media_type
 
         response = OpenAPIResponse(
@@ -210,17 +213,17 @@
         yield str(status_code), OpenAPIResponse(
             description=HTTPStatus(status_code).description,
             content={MediaType.JSON: OpenAPIMediaType(schema=schema)},
         )
 
 
 def create_additional_responses(
-    route_handler: "HTTPRouteHandler",
-    plugins: list["OpenAPISchemaPluginProtocol"],
-    schemas: dict[str, "Schema"],
+    route_handler: HTTPRouteHandler,
+    plugins: list[OpenAPISchemaPluginProtocol],
+    schemas: dict[str, Schema],
 ) -> Iterator[tuple[str, OpenAPIResponse]]:
     """Create the schema for additional responses, if any."""
     if not route_handler.responses:
         return
 
     for status_code, additional_response in route_handler.responses.items():
         schema = create_schema(
@@ -232,19 +235,19 @@
         yield str(status_code), OpenAPIResponse(
             description=additional_response.description,
             content={additional_response.media_type: OpenAPIMediaType(schema=schema)},
         )
 
 
 def create_responses(
-    route_handler: "HTTPRouteHandler",
+    route_handler: HTTPRouteHandler,
     raises_validation_error: bool,
     generate_examples: bool,
-    plugins: list["OpenAPISchemaPluginProtocol"],
-    schemas: dict[str, "Schema"],
+    plugins: list[OpenAPISchemaPluginProtocol],
+    schemas: dict[str, Schema],
 ) -> Responses | None:
     """Create a Response model embedded in a `Responses` dictionary for the given RouteHandler or return None."""
 
     responses: Responses = {
         str(route_handler.status_code): create_success_response(
             generate_examples=generate_examples, plugins=plugins, route_handler=route_handler, schemas=schemas
         ),
```

### Comparing `litestar-2.0.0a4/litestar/_openapi/schema_generation/constrained_fields.py` & `litestar-2.0.0a5/litestar/_openapi/schema_generation/constrained_fields.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     "create_date_constrained_field_schema",
     "create_numerical_constrained_field_schema",
     "create_string_constrained_field_schema",
 )
 
 
 def create_numerical_constrained_field_schema(
-    field_type: type["ConstrainedFloat"] | type["ConstrainedInt"] | type["ConstrainedDecimal"],
+    field_type: type[ConstrainedFloat] | type[ConstrainedInt] | type[ConstrainedDecimal],
 ) -> Schema:
     """Create Schema from Constrained Int/Float/Decimal field."""
     schema = Schema(type=OpenAPIType.INTEGER if issubclass(field_type, int) else OpenAPIType.NUMBER)
     if field_type.le is not None:
         schema.maximum = float(field_type.le)
     if field_type.lt is not None:
         schema.exclusive_maximum = float(field_type.lt)
@@ -62,46 +62,46 @@
     if field_type.gt is not None:
         schema.exclusive_minimum = float(field_type.gt)
     if field_type.multiple_of is not None:
         schema.multiple_of = float(field_type.multiple_of)
     return schema
 
 
-def create_date_constrained_field_schema(field_type: type["ConstrainedDate"]) -> Schema:
+def create_date_constrained_field_schema(field_type: type[ConstrainedDate]) -> Schema:
     """Create Schema from Constrained Date Field."""
     schema = Schema(type=OpenAPIType.STRING, format=OpenAPIFormat.DATE)
     if field_type.le is not None:
         schema.maximum = float(datetime.combine(field_type.le, datetime.min.time()).timestamp())
     if field_type.lt is not None:
         schema.exclusive_maximum = float(datetime.combine(field_type.lt, datetime.min.time()).timestamp())
     if field_type.ge is not None:
         schema.minimum = float(datetime.combine(field_type.ge, datetime.min.time()).timestamp())
     if field_type.gt is not None:
         schema.exclusive_minimum = float(datetime.combine(field_type.gt, datetime.min.time()).timestamp())
     return schema
 
 
-def create_string_constrained_field_schema(field_type: type["ConstrainedStr"] | type["ConstrainedBytes"]) -> Schema:
+def create_string_constrained_field_schema(field_type: type[ConstrainedStr] | type[ConstrainedBytes]) -> Schema:
     """Create Schema from Constrained Str/Bytes field."""
     schema = Schema(type=OpenAPIType.STRING)
     if field_type.min_length:
         schema.min_length = field_type.min_length
     if field_type.max_length:
         schema.max_length = field_type.max_length
     if hasattr(field_type, "regex") and isinstance(field_type.regex, Pattern):
         schema.pattern = field_type.regex.pattern
     if field_type.to_lower:
         schema.description = "must be in lower case"
     return schema
 
 
 def create_collection_constrained_field_schema(
-    field_type: type["ConstrainedList"] | type["ConstrainedSet"] | type["ConstrainedFrozenSet"],
-    children: tuple["SignatureField", ...] | None,
-    plugins: list["OpenAPISchemaPluginProtocol"],
+    field_type: type[ConstrainedList] | type[ConstrainedSet] | type[ConstrainedFrozenSet],
+    children: tuple[SignatureField, ...] | None,
+    plugins: list[OpenAPISchemaPluginProtocol],
     schemas: dict[str, Schema],
 ) -> Schema:
     """Create Schema from Constrained List/Set field.
 
     Args:
         field_type: A constrained field type.
         children: Any child fields.
@@ -140,27 +140,27 @@
             plugins=plugins,
             schemas=schemas,
         )
     return schema
 
 
 def create_constrained_field_schema(
-    field_type: type["ConstrainedBytes"]
-    | type["ConstrainedDate"]
-    | type["ConstrainedDecimal"]
-    | type["ConstrainedFloat"]
-    | type["ConstrainedFrozenSet"]
-    | type["ConstrainedInt"]
-    | type["ConstrainedList"]
-    | type["ConstrainedSet"]
-    | type["ConstrainedStr"],
-    children: tuple["SignatureField", ...] | None,
-    plugins: list["OpenAPISchemaPluginProtocol"],
+    field_type: type[ConstrainedBytes]
+    | type[ConstrainedDate]
+    | type[ConstrainedDecimal]
+    | type[ConstrainedFloat]
+    | type[ConstrainedFrozenSet]
+    | type[ConstrainedInt]
+    | type[ConstrainedList]
+    | type[ConstrainedSet]
+    | type[ConstrainedStr],
+    children: tuple[SignatureField, ...] | None,
+    plugins: list[OpenAPISchemaPluginProtocol],
     schemas: dict[str, Schema],
-) -> "Schema":
+) -> Schema:
     """Create Schema for Pydantic Constrained fields (created using constr(), conint() and so forth, or by subclassing
     Constrained*)
 
     Args:
         field_type: A constrained field type.
         children: Any children.
         plugins: A list of plugins.
```

### Comparing `litestar-2.0.0a4/litestar/_openapi/schema_generation/examples.py` & `litestar-2.0.0a5/litestar/_openapi/schema_generation/examples.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,25 +33,25 @@
         value = [_normalize_example_value(v) for v in value]
     if isinstance(value, dict):
         for k, v in value.items():
             value[k] = _normalize_example_value(v)
     return value
 
 
-def _create_field_meta(field: "SignatureField") -> FieldMeta:
+def _create_field_meta(field: SignatureField) -> FieldMeta:
     return FieldMeta(
         name=field.name,
         annotation=field.field_type,
-        constant=field.is_const,
+        constraints={"constant": field.is_const},
         default=field.default_value if field.default_value is not Empty else Null,
         children=[_create_field_meta(child) for child in field.children] if field.children else None,
     )
 
 
-def create_examples_for_field(field: "SignatureField") -> list["Example"]:
+def create_examples_for_field(field: SignatureField) -> list[Example]:
     """Create an OpenAPI Example instance.
 
     Args:
         field: A signature field.
 
     Returns:
         A list including a single example.
```

### Comparing `litestar-2.0.0a4/litestar/_openapi/schema_generation/schema.py` & `litestar-2.0.0a5/litestar/_openapi/schema_generation/schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 from collections import deque
 from copy import copy
 from dataclasses import MISSING, fields
 from datetime import date, datetime, time, timedelta
 from enum import EnumMeta
-from inspect import getdoc
 from ipaddress import IPv4Address, IPv4Interface, IPv4Network, IPv6Address, IPv6Interface, IPv6Network
 from pathlib import Path
 from typing import (
     TYPE_CHECKING,
     Any,
     DefaultDict,
     Deque,
@@ -27,14 +26,15 @@
     Set,
     Tuple,
     cast,
 )
 from uuid import UUID
 
 from _decimal import Decimal
+from msgspec.structs import fields as msgspec_struct_fields
 from typing_extensions import get_args, get_type_hints
 
 from litestar._openapi.schema_generation.constrained_fields import (
     create_constrained_field_schema,
 )
 from litestar._openapi.schema_generation.examples import create_examples_for_field
 from litestar._openapi.schema_generation.utils import sort_schemas_and_references
@@ -45,22 +45,27 @@
 from litestar.openapi.spec import Reference
 from litestar.openapi.spec.enums import OpenAPIFormat, OpenAPIType
 from litestar.openapi.spec.schema import Schema, SchemaDataContainer
 from litestar.pagination import ClassicPagination, CursorPagination, OffsetPagination
 from litestar.serialization import encode_json
 from litestar.types import DataclassProtocol, Empty, TypedDictClass
 from litestar.utils.predicates import (
+    is_attrs_class,
     is_dataclass_class,
+    is_optional_union,
     is_pydantic_constrained_field,
     is_pydantic_model_class,
+    is_struct_class,
     is_typed_dict,
 )
 from litestar.utils.typing import get_origin_or_inner_type, make_non_optional_union
 
 if TYPE_CHECKING:
+    from msgspec import Struct
+
     from litestar.plugins import OpenAPISchemaPluginProtocol
 
     try:
         from pydantic import (
             BaseModel,
             ConstrainedBytes,
             ConstrainedDate,
@@ -80,14 +85,18 @@
         ConstrainedFloat = Any  # type: ignore
         ConstrainedFrozenSet = Any  # type: ignore
         ConstrainedInt = Any  # type: ignore
         ConstrainedList = Any  # type: ignore
         ConstrainedSet = Any  # type: ignore
         ConstrainedStr = Any  # type: ignore
 
+    try:
+        from attrs import AttrsInstance
+    except ImportError:
+        AttrsInstance = Any  # type: ignore
 try:
     import pydantic
 
     PYDANTIC_TYPE_MAP: dict[type[Any] | None | Any, Schema] = {
         pydantic.UUID1: Schema(
             type=OpenAPIType.STRING,
             format=OpenAPIFormat.UUID,
@@ -325,17 +334,17 @@
     if isinstance(annotation, EnumMeta):
         return create_enum_schema(annotation)
 
     return None
 
 
 def create_schema_for_optional_field(
-    field: "SignatureField",
+    field: SignatureField,
     generate_examples: bool,
-    plugins: list["OpenAPISchemaPluginProtocol"],
+    plugins: list[OpenAPISchemaPluginProtocol],
     schemas: dict[str, Schema],
 ) -> Schema:
     """Create a Schema for an optional SignatureField.
 
     Args:
         field: A signature field instance.
         generate_examples: Whether to generate examples if none are given.
@@ -366,17 +375,17 @@
             Schema(type=OpenAPIType.NULL),
             *result,
         ]
     )
 
 
 def create_schema_for_union_field(
-    field: "SignatureField",
+    field: SignatureField,
     generate_examples: bool,
-    plugins: list["OpenAPISchemaPluginProtocol"],
+    plugins: list[OpenAPISchemaPluginProtocol],
     schemas: dict[str, Schema],
 ) -> Schema:
     """Create a Schema for a union SignatureField.
 
     Args:
         field: A signature field instance.
         generate_examples: Whether to generate examples if none are given.
@@ -393,17 +402,17 @@
                 for sub_field in field.children or []
             ]
         )
     )
 
 
 def create_schema_for_object_type(
-    field: "SignatureField",
+    field: SignatureField,
     generate_examples: bool,
-    plugins: list["OpenAPISchemaPluginProtocol"],
+    plugins: list[OpenAPISchemaPluginProtocol],
     schemas: dict[str, Schema],
 ) -> Schema:
     """Create schema for object types (dict, Mapping, list, Sequence etc.) types.
 
     Args:
         field: A signature field instance.
         generate_examples: Whether to generate examples if none are given.
@@ -435,19 +444,19 @@
         f"This can occur if a user-defined generic type is resolved as a parameter. If '{field.name}' should "
         "not be documented as a parameter, annotate it using the `Dependency` function, e.g., "
         f"`{field.name}: ... = Dependency(...)`."
     )
 
 
 def create_schema_for_builtin_generics(
-    field: "SignatureField",
+    field: SignatureField,
     generate_examples: bool,
-    plugins: list["OpenAPISchemaPluginProtocol"],
+    plugins: list[OpenAPISchemaPluginProtocol],
     schemas: dict[str, Schema],
-) -> "Schema":
+) -> Schema:
     """Handle builtin generic types.
 
     Args:
         field: A signature field instance.
         generate_examples: Whether to generate examples if none are given.
         plugins: A list of plugins.
         schemas: A mapping of namespaces to schemas - this mapping is used in the OA components section.
@@ -517,120 +526,210 @@
         },
     )
 
 
 def create_schema_for_pydantic_model(
     field_type: type[BaseModel],
     generate_examples: bool,
-    plugins: list["OpenAPISchemaPluginProtocol"],
+    plugins: list[OpenAPISchemaPluginProtocol],
     schemas: dict[str, Schema],
 ) -> Schema:
     """Create a schema object for a given pydantic model class.
 
     Args:
         field_type: A pydantic model class.
         generate_examples: Whether to generate examples if none are given.
         plugins: A list of plugins.
         schemas: A mapping of namespaces to schemas - this mapping is used in the OA components section.
 
     Returns:
         A schema instance.
     """
-    field_type_hints = get_type_hints(field_type, include_extras=False)
+
+    field_type_hints = get_type_hints(field_type)
     return Schema(
-        required=[field.alias or field.name for field in field_type.__fields__.values() if field.required],
+        required=sorted([field.alias or field.name for field in field_type.__fields__.values() if field.required]),
         properties={
             (f.alias or f.name): create_schema(
                 field=SignatureField.create(field_type=field_type_hints[f.name], name=f.alias or f.name),
                 generate_examples=generate_examples,
                 plugins=plugins,
                 schemas=schemas,
             )
             for f in field_type.__fields__.values()
         },
         type=OpenAPIType.OBJECT,
         title=_get_type_schema_name(field_type),
-        description=getdoc(field_type) or None,
+    )
+
+
+def create_schema_for_attrs_class(
+    field_type: type[AttrsInstance],
+    generate_examples: bool,
+    plugins: list[OpenAPISchemaPluginProtocol],
+    schemas: dict[str, Schema],
+) -> Schema:
+    """Create a schema object for a given attrs class.
+
+    Args:
+        field_type: An attrs class.
+        generate_examples: Whether to generate examples if none are given.
+        plugins: A list of plugins.
+        schemas: A mapping of namespaces to schemas - this mapping is used in the OA components section.
+
+    Returns:
+        A schema instance.
+    """
+    from attr import NOTHING
+    from attrs import fields_dict
+
+    field_type_hints = get_type_hints(field_type)
+    return Schema(
+        required=sorted(
+            [
+                field_name
+                for field_name, attribute in fields_dict(field_type).items()
+                if attribute.default is NOTHING and not is_optional_union(field_type_hints[field_name])
+            ]
+        ),
+        properties={
+            k: create_schema(
+                field=SignatureField.create(field_type=v, name=k),
+                generate_examples=generate_examples,
+                plugins=plugins,
+                schemas=schemas,
+            )
+            for k, v in field_type_hints.items()
+        },
+        type=OpenAPIType.OBJECT,
+        title=_get_type_schema_name(field_type),
+    )
+
+
+def create_schema_for_struct_class(
+    field_type: type[Struct],
+    generate_examples: bool,
+    plugins: list[OpenAPISchemaPluginProtocol],
+    schemas: dict[str, Schema],
+) -> Schema:
+    """Create a schema object for a given msgspec.Struct class.
+
+    Args:
+        field_type: A msgspec.Struct class.
+        generate_examples: Whether to generate examples if none are given.
+        plugins: A list of plugins.
+        schemas: A mapping of namespaces to schemas - this mapping is used in the OA components section.
+
+    Returns:
+        A schema instance.
+    """
+
+    return Schema(
+        required=sorted(
+            [
+                field.encode_name
+                for field in msgspec_struct_fields(field_type)
+                if field.required and not is_optional_union(field.type)
+            ]
+        ),
+        properties={
+            field.encode_name: create_schema(
+                field=SignatureField.create(field_type=field.type, name=field.encode_name),
+                generate_examples=generate_examples,
+                plugins=plugins,
+                schemas=schemas,
+            )
+            for field in msgspec_struct_fields(field_type)
+        },
+        type=OpenAPIType.OBJECT,
+        title=_get_type_schema_name(field_type),
     )
 
 
 def create_schema_for_dataclass(
     field_type: type[DataclassProtocol],
     generate_examples: bool,
-    plugins: list["OpenAPISchemaPluginProtocol"],
+    plugins: list[OpenAPISchemaPluginProtocol],
     schemas: dict[str, Schema],
 ) -> Schema:
     """Create a schema object for a given dataclass class.
 
     Args:
         field_type: A dataclass class.
         generate_examples: Whether to generate examples if none are given.
         plugins: A list of plugins.
         schemas: A mapping of namespaces to schemas - this mapping is used in the OA components section.
 
     Returns:
         A schema instance.
     """
+    field_type_hints = get_type_hints(field_type)
     return Schema(
-        required=[
-            field.name for field in fields(field_type) if field.default is MISSING and field.default_factory is MISSING
-        ],
+        required=sorted(
+            [
+                field.name
+                for field in fields(field_type)
+                if (
+                    field.default is MISSING
+                    and field.default_factory is MISSING
+                    and not is_optional_union(field_type_hints[field.name])
+                )
+            ]
+        ),
         properties={
             k: create_schema(
                 field=SignatureField.create(field_type=v, name=k),
                 generate_examples=generate_examples,
                 plugins=plugins,
                 schemas=schemas,
             )
-            for k, v in get_type_hints(field_type, include_extras=False).items()
+            for k, v in field_type_hints.items()
         },
         type=OpenAPIType.OBJECT,
         title=_get_type_schema_name(field_type),
-        description=getdoc(field_type) or None,
     )
 
 
 def create_schema_for_typed_dict(
     field_type: TypedDictClass,
     generate_examples: bool,
-    plugins: list["OpenAPISchemaPluginProtocol"],
+    plugins: list[OpenAPISchemaPluginProtocol],
     schemas: dict[str, Schema],
 ) -> Schema:
     """Create a schema object for a given typed dict.
 
     Args:
         field_type: A typed-dict class.
         generate_examples: Whether to generate examples if none are given.
         plugins: A list of plugins.
         schemas: A mapping of namespaces to schemas - this mapping is used in the OA components section.
 
     Returns:
         A schema instance.
     """
     return Schema(
-        required=list(getattr(field_type, "__required_keys__", [])),
+        required=sorted(getattr(field_type, "__required_keys__", [])),
         properties={
             k: create_schema(
                 field=SignatureField.create(field_type=v, name=k),
                 generate_examples=generate_examples,
                 plugins=plugins,
                 schemas=schemas,
             )
-            for k, v in get_type_hints(field_type, include_extras=False).items()
+            for k, v in get_type_hints(field_type).items()
         },
         type=OpenAPIType.OBJECT,
         title=_get_type_schema_name(field_type),
-        description=getdoc(field_type) or None,
     )
 
 
 def create_schema_for_plugin(
-    field: "SignatureField",
+    field: SignatureField,
     generate_examples: bool,
-    plugins: list["OpenAPISchemaPluginProtocol"],
+    plugins: list[OpenAPISchemaPluginProtocol],
     schemas: dict[str, Schema],
     plugin: OpenAPISchemaPluginProtocol,
 ) -> Schema | Reference:
     """Create a schema using a plugin.
 
     Args:
         field: A signature field instance.
@@ -657,15 +756,15 @@
             plugins=plugins,
             schemas=schemas,
         )
     return schema  # pragma: no cover
 
 
 def _process_schema_result(
-    field: "SignatureField",
+    field: SignatureField,
     schema: Schema,
     generate_examples: bool,
     schemas: dict[str, Schema],
 ) -> Schema | Reference:
     if field.kwarg_model and field.is_const and not field.is_empty and schema.const is None:
         schema.const = field.default_value
 
@@ -690,17 +789,17 @@
             )
         schemas[schema.title] = schema
         return Reference(ref=f"#/components/schemas/{schema.title}")
     return schema
 
 
 def create_schema(
-    field: "SignatureField",
+    field: SignatureField,
     generate_examples: bool,
-    plugins: list["OpenAPISchemaPluginProtocol"],
+    plugins: list[OpenAPISchemaPluginProtocol],
     schemas: dict[str, Schema],
 ) -> Schema | Reference:
     """Create a Schema for a given SignatureField.
 
     Args:
         field: A signature field instance.
         generate_examples: Whether to generate examples if none are given.
@@ -721,14 +820,24 @@
         )
 
     elif is_pydantic_model_class(annotation=field.field_type):
         result = create_schema_for_pydantic_model(
             field_type=field.field_type, generate_examples=generate_examples, plugins=plugins, schemas=schemas
         )
 
+    elif is_attrs_class(annotation=field.field_type):
+        result = create_schema_for_attrs_class(
+            field_type=field.field_type, generate_examples=generate_examples, plugins=plugins, schemas=schemas
+        )
+
+    elif is_struct_class(annotation=field.field_type):
+        result = create_schema_for_struct_class(
+            field_type=field.field_type, generate_examples=generate_examples, plugins=plugins, schemas=schemas
+        )
+
     elif is_dataclass_class(annotation=field.field_type):
         result = create_schema_for_dataclass(
             field_type=field.field_type, generate_examples=generate_examples, plugins=plugins, schemas=schemas
         )
 
     elif is_typed_dict(annotation=field.field_type):
         result = create_schema_for_typed_dict(
```

### Comparing `litestar-2.0.0a4/litestar/_openapi/schema_generation/utils.py` & `litestar-2.0.0a5/litestar/_openapi/schema_generation/utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/_openapi/typescript_converter/converter.py` & `litestar-2.0.0a5/litestar/_openapi/typescript_converter/converter.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/_openapi/typescript_converter/schema_parsing.py` & `litestar-2.0.0a5/litestar/_openapi/typescript_converter/schema_parsing.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     if allow_quoted:
         if allowed_key_re.fullmatch(value):
             return value
         return f'"{value}"'
     return invalid_namespace_re.sub("", value)
 
 
-def is_schema_value(value: Any) -> "TypeGuard[Schema]":
+def is_schema_value(value: Any) -> TypeGuard[Schema]:
     """Typeguard for a schema value.
 
     Args:
         value: An arbitrary value
 
     Returns:
         A typeguard boolean dictating whether the passed in value is a Schema.
```

### Comparing `litestar-2.0.0a4/litestar/_openapi/typescript_converter/types.py` & `litestar-2.0.0a5/litestar/_openapi/typescript_converter/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/_openapi/utils.py` & `litestar-2.0.0a5/litestar/_openapi/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from __future__ import annotations
 
 import re
-from typing import TYPE_CHECKING, Union
+from typing import TYPE_CHECKING
 
 from litestar.types.internal_types import PathParameterDefinition
 
 if TYPE_CHECKING:
     from litestar.handlers.http_handlers import HTTPRouteHandler
     from litestar.types import Method
 
 
 __all__ = ("default_operation_id_creator",)
 
 SEPARATORS_CLEANUP_PATTERN = re.compile(r"[!#$%&'*+\-.^_`|~:]+")
 
 
 def default_operation_id_creator(
-    route_handler: "HTTPRouteHandler",
-    http_method: "Method",
-    path_components: list[Union[str, "PathParameterDefinition"]],
+    route_handler: HTTPRouteHandler,
+    http_method: Method,
+    path_components: list[str | PathParameterDefinition],
 ) -> str:
     """Create a unique 'operationId' for an OpenAPI PathItem entry.
 
     Args:
         route_handler: The HTTP Route Handler instance.
         http_method: The HTTP method for the given PathItem.
         path_components: A list of path components.
```

### Comparing `litestar-2.0.0a4/litestar/_parsers.py` & `litestar-2.0.0a5/litestar/_parsers.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,16 +30,15 @@
 
     Args:
         query_string: A query string.
 
     Returns:
         A tuple of key value pairs.
     """
-    _bools = {"true": True, "false": False, "True": True, "False": False}
-    return tuple((k, v if v not in _bools else _bools[v]) for k, v in fast_parse_query_string(query_string, "&"))
+    return tuple(fast_parse_query_string(query_string, "&"))
 
 
 @lru_cache(1024)
 def parse_cookie_string(cookie_string: str) -> dict[str, str]:
     """Parse a cookie string into a dictionary of values.
 
     Args:
```

### Comparing `litestar-2.0.0a4/litestar/_signature/field.py` & `litestar-2.0.0a5/litestar/_signature/field.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/_signature/models/attrs_signature_model.py` & `litestar-2.0.0a5/litestar/_signature/models/attrs_signature_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,16 +11,14 @@
     Any,
     Callable,
     cast,
 )
 from uuid import UUID
 
 from _decimal import Decimal
-from dateutil.parser import parse
-from pytimeparse.timeparse import timeparse
 from typing_extensions import get_args
 
 from litestar._signature.field import SignatureField
 from litestar._signature.models.base import ErrorMessage, SignatureModel
 from litestar.connection import ASGIConnection, Request, WebSocket
 from litestar.datastructures import ImmutableState, MultiDict, State, UploadFile
 from litestar.exceptions import MissingDependencyException
@@ -31,23 +29,33 @@
 from litestar.utils.typing import get_origin_or_inner_type, make_non_optional_union, unwrap_union
 
 try:
     import attr
     import attrs
     import cattrs
 except ImportError as e:
-    raise MissingDependencyException("attrs is not installed") from e
+    raise MissingDependencyException("attrs") from e
+
+try:
+    from dateutil.parser import parse
+except ImportError as e:
+    raise MissingDependencyException("python-dateutil", "attrs") from e
+
+try:
+    from pytimeparse.timeparse import timeparse
+except ImportError as e:
+    raise MissingDependencyException("pytimeparse", "attrs") from e
 
 if TYPE_CHECKING:
-    from litestar.plugins import PluginMapping
     from litestar.utils.signature import ParsedSignature
 
-key_re = re.compile("@ attribute (.*)|'(.*)'")
-
 __all__ = ("AttrsSignatureModel",)
+key_re = re.compile("@ attribute (.*)|'(.*)'")
+TRUE_SET = {"1", "true", "on", "t", "y", "yes"}
+FALSE_SET = {"0", "false", "off", "f", "n", "no"}
 
 try:
     import pydantic
 
     def _structure_base_model(value: Any, cls: type[pydantic.BaseModel]) -> pydantic.BaseModel:
         if isinstance(value, pydantic.BaseModel):
             return value
@@ -64,14 +72,30 @@
     return value
 
 
 def _pass_through_unstructure_hook(value: Any) -> Any:
     return value
 
 
+def _structure_bool(value: Any, _: type[bool]) -> bool:
+    if isinstance(value, bytes):
+        value = value.decode("utf-8").lower()
+
+    if isinstance(value, str):
+        value = value.lower()
+
+    if value == 0 or value in FALSE_SET:
+        return False
+
+    if value == 1 or value in TRUE_SET:
+        return True
+
+    raise ValueError(f"Cannot convert {value} to bool")
+
+
 def _structure_datetime(value: Any, cls: type[datetime]) -> datetime:
     if isinstance(value, datetime):
         return value
 
     try:
         return cls.fromtimestamp(float(value), tz=timezone.utc)
     except (ValueError, TypeError):
@@ -81,15 +105,15 @@
 
 
 def _structure_date(value: Any, cls: type[date]) -> date:
     if isinstance(value, date) and not isinstance(value, datetime):
         return value
 
     if isinstance(value, (float, int, Decimal)):
-        return cls.fromtimestamp(float(value))
+        return datetime.fromtimestamp(float(value), tz=timezone.utc).date()
 
     dt = _structure_datetime(value=value, cls=datetime)
     return cls(year=dt.year, month=dt.month, day=dt.day)
 
 
 def _structure_time(value: Any, cls: type[time]) -> time:
     if isinstance(value, time):
@@ -140,14 +164,15 @@
     (MultiDict, _structure_multidict),
     (PurePath, _structure_path),
     (Request, _pass_through_structure_hook),
     (State, _pass_through_structure_hook),
     (UUID, _structure_uuid),
     (UploadFile, _pass_through_structure_hook),
     (WebSocket, _pass_through_structure_hook),
+    (bool, _structure_bool),
     (date, _structure_date),
     (datetime, _structure_datetime),
     (str, _structure_str),
     (time, _structure_time),
     (timedelta, _structure_timedelta),
     *pydantic_hooks,
 ]
@@ -207,15 +232,15 @@
 
     Args:
         e: An ExceptionGroup - which is a py3.11 feature. We use hasattr instead of instance checks to avoid installing this.
 
     Returns:
         A list of normalized exception messages.
     """
-    messages: "list[ErrorMessage]" = []
+    messages: list[ErrorMessage] = []
     if hasattr(e, "exceptions"):
         for exc in cast("list[Exception]", e.exceptions):
             if hasattr(exc, "exceptions"):  # pragma: no cover
                 # cattrs raises an exception group, where each exception can potentially be an exception group.
                 # this case is not reproducible in any of our tests - and frankly I have no idea when it would occur,
                 # so this clause is defensive programming only.
                 messages.extend(_extract_exceptions(exc))
@@ -290,15 +315,14 @@
 
     @classmethod
     def create(
         cls,
         fn_name: str,
         fn_module: str | None,
         parsed_signature: ParsedSignature,
-        field_plugin_mappings: dict[str, PluginMapping],
         dependency_names: set[str],
         type_overrides: dict[str, Any],
     ) -> type[SignatureModel]:
         attributes: dict[str, Any] = {}
 
         for parameter in parsed_signature.parameters.values():
             annotation = type_overrides.get(parameter.name, parameter.parsed_type.annotation)
@@ -337,11 +361,10 @@
             f"{fn_name}_signature_model",
             attrs=attributes,
             bases=(AttrsSignatureModel,),
             slots=True,
             kw_only=True,
         )
         model.return_annotation = parsed_signature.return_type.annotation  # pyright: ignore
-        model.field_plugin_mappings = field_plugin_mappings  # pyright: ignore
         model.dependency_name_set = dependency_names  # pyright: ignore
         model.populate_signature_fields()  # pyright: ignore
         return model
```

### Comparing `litestar-2.0.0a4/litestar/_signature/models/base.py` & `litestar-2.0.0a5/litestar/_signature/models/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,30 +5,28 @@
 
 from litestar.enums import ScopeType
 from litestar.exceptions import InternalServerException, ValidationException
 
 if TYPE_CHECKING:
     from litestar._signature.field import SignatureField
     from litestar.connection import ASGIConnection
-    from litestar.plugins import PluginMapping
     from litestar.utils.signature import ParsedSignature
 
 __all__ = ("SignatureModel",)
 
 
 class ErrorMessage(TypedDict):
     key: str
     message: str
 
 
 class SignatureModel(ABC):
     """Base model for Signature modelling."""
 
     dependency_name_set: ClassVar[set[str]]
-    field_plugin_mappings: ClassVar[dict[str, PluginMapping]]
     return_annotation: ClassVar[Any]
     fields: ClassVar[dict[str, SignatureField]]
 
     @classmethod
     def _create_exception(cls, connection: ASGIConnection, messages: list[ErrorMessage]) -> Exception:
         """Create an exception class - either a ValidationException or an InternalServerException, depending on whether
             the failure is in client provided values or injected dependencies.
@@ -89,25 +87,23 @@
     @classmethod
     @abstractmethod
     def create(
         cls,
         fn_name: str,
         fn_module: str | None,
         parsed_signature: ParsedSignature,
-        field_plugin_mappings: dict[str, PluginMapping],
         dependency_names: set[str],
         type_overrides: dict[str, Any],
     ) -> type[SignatureModel]:
         """Create a SignatureModel.
 
         Args:
             fn_name: Name of the callable.
             fn_module: Name of the function's module, if any.
             parsed_signature: A parsed signature.
-            field_plugin_mappings: A mapping of field names to plugin mappings.
             dependency_names: A set of dependency names.
             type_overrides: A dictionary of type overrides, either will override a parameter type with a type derived
                 from a plugin, or set the type to ``Any`` if validation should be skipped for the parameter.
 
         Returns:
             The created SignatureModel.
         """
```

### Comparing `litestar-2.0.0a4/litestar/_signature/models/pydantic_signature_model.py` & `litestar-2.0.0a5/litestar/_signature/models/pydantic_signature_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from litestar.constants import UNDEFINED_SENTINELS
 from litestar.params import BodyKwarg, DependencyKwarg, ParameterKwarg
 from litestar.types import Empty
 from litestar.utils.predicates import is_pydantic_constrained_field
 
 if TYPE_CHECKING:
     from litestar.connection import ASGIConnection
-    from litestar.plugins import PluginMapping
     from litestar.utils.signature import ParsedSignature
 
 __all__ = ("PydanticSignatureModel",)
 
 
 class PydanticSignatureModel(SignatureModel, BaseModel):
     """Model that represents a function signature that uses a pydantic specific type or types."""
@@ -49,35 +48,20 @@
             raise cls._create_exception(
                 messages=[{"key": str(exc["loc"][-1]), "message": exc["msg"]} for exc in e.errors()],
                 connection=connection,
             ) from e
 
         return signature.to_dict()
 
-    def _resolve_field_value(self, key: str) -> Any:
-        """Return value using key mapping, if available.
-
-        Args:
-            key: A field name.
-
-        Returns:
-            The plugin value, if available.
-        """
-        value = self.__getattribute__(key)
-        mapping = self.field_plugin_mappings.get(key)
-        return mapping.get_model_instance_for_value(value) if mapping else value
-
     def to_dict(self) -> dict[str, Any]:
         """Normalize access to the signature model's dictionary method, because different backends use different methods
         for this.
 
         Returns: A dictionary of string keyed values.
         """
-        if self.field_plugin_mappings:
-            return {key: self._resolve_field_value(key) for key in self.__fields__}
         return {key: self.__getattribute__(key) for key in self.__fields__}
 
     @classmethod
     def signature_field_from_model_field(cls, model_field: ModelField) -> SignatureField:
         """Create a SignatureField instance from a pydantic ModelField.
 
         Args:
@@ -124,25 +108,23 @@
 
     @classmethod
     def create(
         cls,
         fn_name: str,
         fn_module: str | None,
         parsed_signature: ParsedSignature,
-        field_plugin_mappings: dict[str, PluginMapping],
         dependency_names: set[str],
         type_overrides: dict[str, Any],
     ) -> type[PydanticSignatureModel]:
         """Create a pydantic based SignatureModel.
 
         Args:
             fn_name: Name of the callable.
             fn_module: Name of the function's module, if any.
             parsed_signature: A ParsedSignature instance.
-            field_plugin_mappings: A mapping of field names to plugin mappings.
             dependency_names: A set of dependency names.
             type_overrides: A dictionary of type overrides, either will override a parameter type with a type derived
                 from a plugin, or set the type to ``Any`` if validation should be skipped for the parameter.
 
         Returns:
             The created PydanticSignatureModel.
         """
@@ -181,11 +163,10 @@
         model: type[PydanticSignatureModel] = create_model(  # type: ignore
             f"{fn_name}_signature_model",
             __base__=PydanticSignatureModel,
             __module__=fn_module or "pydantic.main",
             **field_definitions,
         )
         model.return_annotation = parsed_signature.return_type.annotation
-        model.field_plugin_mappings = field_plugin_mappings
         model.dependency_name_set = dependency_names
         model.populate_signature_fields()
         return model
```

### Comparing `litestar-2.0.0a4/litestar/app.py` & `litestar-2.0.0a5/litestar/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 from __future__ import annotations
 
 import logging
 from datetime import date, datetime, time, timedelta
-from functools import partial
 from itertools import chain
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Literal, Mapping, Sequence, cast
 
 from typing_extensions import Self, TypedDict
 
 from litestar._asgi import ASGIRouter
 from litestar._asgi.utils import get_route_handlers, wrap_in_exception_handler
 from litestar._openapi.path_item import create_path_item
-from litestar._signature import create_signature_model
 from litestar.config.allowed_hosts import AllowedHostsConfig
 from litestar.config.app import AppConfig
 from litestar.config.response_cache import ResponseCacheConfig
 from litestar.connection import Request, WebSocket
 from litestar.constants import OPENAPI_NOT_INITIALIZED
 from litestar.datastructures.state import State
 from litestar.events.emitter import BaseEventEmitterBackend, SimpleEventEmitter
 from litestar.exceptions import (
     ImproperlyConfiguredException,
     NoRouteMatchFoundException,
 )
-from litestar.handlers.http_handlers import HTTPRouteHandler
 from litestar.logging.config import LoggingConfig, get_logger_placeholder
 from litestar.middleware.cors import CORSMiddleware
 from litestar.openapi.config import OpenAPIConfig
 from litestar.openapi.spec.components import Components
 from litestar.plugins import (
     InitPluginProtocol,
     OpenAPISchemaPluginProtocol,
@@ -38,31 +35,26 @@
 from litestar.routes import ASGIRoute, HTTPRoute, WebSocketRoute
 from litestar.static_files.base import StaticFiles
 from litestar.stores.registry import StoreRegistry
 from litestar.types import Empty
 from litestar.types.internal_types import PathParameterDefinition
 from litestar.utils import (
     as_async_callable_list,
-    async_partial,
-    is_async_callable,
     join_paths,
     unique,
 )
 from litestar.utils.dataclass import extract_dataclass_items
-from litestar.utils.helpers import unwrap_partial
-from litestar.utils.signature import ParsedSignature
 
 if TYPE_CHECKING:
     from litestar.config.compression import CompressionConfig
     from litestar.config.cors import CORSConfig
     from litestar.config.csrf import CSRFConfig
     from litestar.datastructures import CacheControlHeader, ETag, ResponseHeader
     from litestar.dto.interface import DTOInterface
     from litestar.events.listener import EventListener
-    from litestar.handlers.base import BaseRouteHandler
     from litestar.logging.config import BaseLoggingConfig
     from litestar.openapi.spec import SecurityRequirement
     from litestar.openapi.spec.open_api import OpenAPI
     from litestar.plugins import PluginProtocol
     from litestar.static_files.config import StaticFilesConfig
     from litestar.stores.base import Store
     from litestar.template.config import TemplateConfig
@@ -148,24 +140,24 @@
         "cors_config",
         "csrf_config",
         "event_emitter",
         "get_logger",
         "logger",
         "logging_config",
         "multipart_form_part_limit",
-        "signature_namespace",
         "on_shutdown",
         "on_startup",
         "openapi_config",
         "openapi_schema_plugins",
         "preferred_validation_backend",
         "request_class",
         "response_cache_config",
         "route_map",
         "serialization_plugins",
+        "signature_namespace",
         "state",
         "static_files_config",
         "stores",
         "template_engine",
         "websocket_class",
     )
 
@@ -537,17 +529,15 @@
         """
         routes = super().register(value=value)
 
         for route in routes:
             route_handlers = get_route_handlers(route)
 
             for route_handler in route_handlers:
-                route_handler.on_registration()
-                self._set_runtime_callables(route_handler=route_handler)
-                self._create_handler_signature_model(route_handler=route_handler)
+                route_handler.on_registration(self)
 
             if isinstance(route, HTTPRoute):
                 route.create_handler_map()
 
             elif isinstance(route, WebSocketRoute):
                 route.handler_parameter_model = route.create_handler_kwargs_model(route.route_handler)
 
@@ -659,15 +649,15 @@
     def url_for_static_asset(self, name: str, file_path: str) -> str:
         """Receives a static files handler name, an asset file path and returns resolved url path to the asset.
 
         Examples:
             .. code-block: python
 
                 from litestar import Litestar
-                from litestar.config.static_files import StaticFilesConfig
+                from litestar.static_files.config import StaticFilesConfig
 
                 app = Litestar(
                     static_files_config=[StaticFilesConfig(directories=["css"], path="/static/css")]
                 )
 
                 path = app.url_for_static_asset("css", "main.css")
 
@@ -716,84 +706,27 @@
         if self.cors_config:
             asgi_handler = CORSMiddleware(app=asgi_handler, config=self.cors_config)
 
         return wrap_in_exception_handler(
             debug=self.debug, app=asgi_handler, exception_handlers=self.exception_handlers or {}
         )
 
-    @staticmethod
-    def _set_runtime_callables(route_handler: BaseRouteHandler) -> None:
-        """Optimize the ``route_handler.fn`` and any ``provider.dependency`` callables for runtime by doing the following:
-
-        1. ensure that the ``self`` argument is preserved by binding it using partial.
-        2. ensure sync functions are wrapped in AsyncCallable for sync_to_thread handlers.
-
-        Args:
-            route_handler: A route handler to process.
-
-        Returns:
-            None
-        """
-        from litestar.controller import Controller
-
-        if isinstance(route_handler.owner, Controller) and not hasattr(route_handler.fn.value, "func"):
-            route_handler.fn.value = partial(route_handler.fn.value, route_handler.owner)
-
-        if isinstance(route_handler, HTTPRouteHandler):
-            route_handler.has_sync_callable = False
-            if not is_async_callable(route_handler.fn.value):
-                if route_handler.sync_to_thread:
-                    route_handler.fn.value = async_partial(route_handler.fn.value)
-                else:
-                    route_handler.has_sync_callable = True
-
-        for provider in route_handler.resolve_dependencies().values():
-            if not is_async_callable(provider.dependency.value):
-                provider.has_sync_callable = False
-                if provider.sync_to_thread:
-                    provider.dependency.value = async_partial(provider.dependency.value)
-                else:
-                    provider.has_sync_callable = True
-
-    def _create_handler_signature_model(self, route_handler: BaseRouteHandler) -> None:
-        """Create function signature models for all route handler functions and provider dependencies."""
-        if not route_handler.signature_model:
-            route_handler.signature_model = create_signature_model(
-                dependency_name_set=route_handler.dependency_name_set,
-                fn=cast("AnyCallable", route_handler.fn.value),
-                plugins=self.serialization_plugins,
-                preferred_validation_backend=self.preferred_validation_backend,
-                parsed_signature=route_handler.parsed_fn_signature,
-            )
-
-        for provider in route_handler.resolve_dependencies().values():
-            if not getattr(provider, "signature_model", None):
-                provider.signature_model = create_signature_model(
-                    dependency_name_set=route_handler.dependency_name_set,
-                    fn=provider.dependency.value,
-                    plugins=self.serialization_plugins,
-                    preferred_validation_backend=self.preferred_validation_backend,
-                    parsed_signature=ParsedSignature.from_fn(
-                        unwrap_partial(provider.dependency.value), route_handler.resolve_signature_namespace()
-                    ),
-                )
-
     def _wrap_send(self, send: Send, scope: Scope) -> Send:
         """Wrap the ASGI send and handles any 'before send' hooks.
 
         Args:
             send: The ASGI send function.
             scope: The ASGI scope.
 
         Returns:
             An ASGI send function.
         """
         if self.before_send:
 
-            async def wrapped_send(message: "Message") -> None:
+            async def wrapped_send(message: Message) -> None:
                 for hook in self.before_send:
                     await hook(message, self.state, scope)
                 await send(message)
 
             return wrapped_send
         return send
```

### Comparing `litestar-2.0.0a4/litestar/background_tasks.py` & `litestar-2.0.0a5/litestar/background_tasks.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/cli/_utils.py` & `litestar-2.0.0a5/litestar/cli/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -328,18 +328,14 @@
         for static_files in static_files_configs:
             static_files_info.append(
                 f"path=[yellow]{static_files.path}[/] dirs=[yellow]{', '.join(map(str, static_files.directories))}[/] "
                 f"html_mode={_format_is_enabled(static_files.html_mode)}",
             )
         table.add_row("Static files", "\n".join(static_files_info))
 
-    if app.serialization_plugins:
-        plugin_names = [type(plugin).__name__ for plugin in app.serialization_plugins]
-        table.add_row("Plugins", ", ".join(plugin_names))
-
     middlewares = []
     for middleware in app.middleware:
         updated_middleware = middleware.middleware if isinstance(middleware, DefineMiddleware) else middleware
         middlewares.append(get_name(updated_middleware))
     if middlewares:
         table.add_row("Middlewares", ", ".join(middlewares))
```

### Comparing `litestar-2.0.0a4/litestar/cli/commands/core.py` & `litestar-2.0.0a5/litestar/cli/commands/core.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/cli/commands/schema.py` & `litestar-2.0.0a5/litestar/cli/commands/schema.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/cli/commands/sessions.py` & `litestar-2.0.0a5/litestar/cli/commands/sessions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/cli/main.py` & `litestar-2.0.0a5/litestar/cli/main.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/config/allowed_hosts.py` & `litestar-2.0.0a5/litestar/config/allowed_hosts.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/config/app.py` & `litestar-2.0.0a5/litestar/config/app.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/config/compression.py` & `litestar-2.0.0a5/litestar/config/compression.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/config/cors.py` & `litestar-2.0.0a5/litestar/config/cors.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/config/csrf.py` & `litestar-2.0.0a5/litestar/config/csrf.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/config/response_cache.py` & `litestar-2.0.0a5/litestar/config/response_cache.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/connection/__init__.py` & `litestar-2.0.0a5/litestar/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/connection/base.py` & `litestar-2.0.0a5/litestar/connection/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,26 +25,26 @@
 
 UserT = TypeVar("UserT")
 AuthT = TypeVar("AuthT")
 HandlerT = TypeVar("HandlerT")
 StateT = TypeVar("StateT", bound=State)
 
 
-async def empty_receive() -> "NoReturn":  # pragma: no cover
+async def empty_receive() -> NoReturn:  # pragma: no cover
     """Raise a ``RuntimeError``.
 
     Serves as a placeholder ``send`` function.
 
     Raises:
         RuntimeError
     """
     raise RuntimeError()
 
 
-async def empty_send(_: "Message") -> "NoReturn":  # pragma: no cover
+async def empty_send(_: Message) -> NoReturn:  # pragma: no cover
     """Raise a ``RuntimeError``.
 
     Serves as a placeholder ``send`` function.
 
     Args:
         _: An ASGI message
```

### Comparing `litestar-2.0.0a4/litestar/connection/request.py` & `litestar-2.0.0a5/litestar/connection/request.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/connection/websocket.py` & `litestar-2.0.0a5/litestar/connection/websocket.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         Args:
             receive: The ASGI receive function.
 
         Returns:
             An ASGI receive function.
         """
 
-        async def wrapped_receive() -> "ReceiveMessage":
+        async def wrapped_receive() -> ReceiveMessage:
             if self.connection_state == "disconnect":
                 raise WebSocketException(detail=DISCONNECT_MESSAGE)
             message = await receive()
             if message["type"] == "websocket.connect":
                 self.connection_state = "connect"
             elif message["type"] == "websocket.receive":
                 self.connection_state = "receive"
@@ -89,15 +89,15 @@
         Args:
             send: The ASGI send function.
 
         Returns:
             An ASGI send function.
         """
 
-        async def wrapped_send(message: "Message") -> None:
+        async def wrapped_send(message: Message) -> None:
             if self.connection_state == "disconnect":
                 raise WebSocketDisconnect(detail=DISCONNECT_MESSAGE)  # pragma: no cover
             await send(message)
 
         return wrapped_send
 
     async def accept(
@@ -264,15 +264,15 @@
         await self.send_data(data=data, mode="binary", encoding=encoding)
 
     async def send_json(
         self,
         data: Any,
         mode: Literal["text", "binary"] = "text",
         encoding: str = "utf-8",
-        serializer: "Serializer" = default_serializer,
+        serializer: Serializer = default_serializer,
     ) -> None:
         """Send data as JSON.
 
         Args:
             data: A value to serialize.
             mode: Either ``text`` or ``binary``.
             encoding: Encoding to use for binary data.
```

### Comparing `litestar-2.0.0a4/litestar/constants.py` & `litestar-2.0.0a5/litestar/constants.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/contrib/htmx/_utils.py` & `litestar-2.0.0a5/litestar/contrib/htmx/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/contrib/htmx/request.py` & `litestar-2.0.0a5/litestar/contrib/htmx/request.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/contrib/htmx/response.py` & `litestar-2.0.0a5/litestar/contrib/htmx/response.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,16 +226,12 @@
 
         hx_headers: dict[str, Any] = get_headers(
             hx_headers=HtmxHeaderType(
                 push_url=self.push_url, re_swap=self.re_swap, re_target=self.re_target, trigger_event=event
             )
         )
 
-        template = Template(
-            name=self.name,
-            background=self.background,
-            encoding=self.encoding,
-        )
+        template = Template(name=self.name, background=self.background, context=self.context, encoding=self.encoding)
 
         return template.to_response(
             headers=hx_headers, media_type=media_type, app=app, status_code=status_code, request=request
         )
```

### Comparing `litestar-2.0.0a4/litestar/contrib/htmx/types.py` & `litestar-2.0.0a5/litestar/contrib/htmx/types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/contrib/jinja.py` & `litestar-2.0.0a5/litestar/contrib/jinja.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/contrib/jwt/__init__.py` & `litestar-2.0.0a5/litestar/contrib/jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/contrib/jwt/jwt_auth.py` & `litestar-2.0.0a5/litestar/contrib/jwt/jwt_auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/contrib/jwt/jwt_token.py` & `litestar-2.0.0a5/litestar/contrib/jwt/jwt_token.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/contrib/jwt/middleware.py` & `litestar-2.0.0a5/litestar/contrib/jwt/middleware.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/contrib/mako.py` & `litestar-2.0.0a5/litestar/contrib/mako.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/contrib/opentelemetry/_utils.py` & `litestar-2.0.0a5/litestar/contrib/opentelemetry/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/contrib/opentelemetry/config.py` & `litestar-2.0.0a5/litestar/contrib/opentelemetry/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/contrib/opentelemetry/middleware.py` & `litestar-2.0.0a5/litestar/contrib/opentelemetry/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             excluded_urls=get_excluded_urls(config.exclude_urls_env_key),
             meter=config.meter,
             meter_provider=config.meter_provider,
             server_request_hook=config.server_request_hook_handler,
             tracer_provider=config.tracer_provider,
         )
 
-    async def __call__(self, scope: "Scope", receive: "Receive", send: "Send") -> None:
+    async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
         """ASGI callable.
 
         Args:
             scope: The ASGI connection scope.
             receive: The ASGI receive function.
             send: The ASGI send function.
```

### Comparing `litestar-2.0.0a4/litestar/contrib/repository/abc.py` & `litestar-2.0.0a5/litestar/contrib/repository/abc.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 from typing import TYPE_CHECKING, Any, Generic, TypeVar
 
 from .exceptions import NotFoundError
 
 if TYPE_CHECKING:
     from typing_extensions import TypeAlias
 
-    from .filters import BeforeAfter, CollectionFilter, LimitOffset
+    from .filters import BeforeAfter, CollectionFilter, LimitOffset, OrderBy, SearchFilter
 
-__all__ = ("AbstractRepository", "FilterTypes")
+__all__ = ("AbstractAsyncRepository", "FilterTypes")
 
 T = TypeVar("T")
-RepoT = TypeVar("RepoT", bound="AbstractRepository")
+RepoT = TypeVar("RepoT", bound="AbstractAsyncRepository")
 CollectionT = TypeVar("CollectionT")
 
-FilterTypes: TypeAlias = "BeforeAfter | CollectionFilter[Any] | LimitOffset"
+FilterTypes: TypeAlias = "BeforeAfter | CollectionFilter[Any] | LimitOffset | OrderBy | SearchFilter"
 """Aggregate type alias of the types supported for collection filtering."""
 
 
-class AbstractRepository(Generic[T], metaclass=ABCMeta):
+class AbstractAsyncRepository(Generic[T], metaclass=ABCMeta):
     """Interface for persistent data interaction."""
 
     model_type: type[T]
     """Type of object represented by the repository."""
     id_attribute = "id"
     """Name of the primary identifying attribute on :attr:`model_type`."""
 
@@ -156,30 +156,30 @@
         """
 
     @abstractmethod
     async def update(self, data: T) -> T:
         """Update instance with the attribute values present on ``data``.
 
         Args:
-            data: An instance that should have a value for :attr:`id_attribute <AbstractRepository.id_attribute>` that exists in the
+            data: An instance that should have a value for :attr:`id_attribute <AbstractAsyncRepository.id_attribute>` that exists in the
                 collection.
 
         Returns:
             The updated instance.
 
         Raises:
             NotFoundError: If no instance found with same identifier as ``data``.
         """
 
     @abstractmethod
-    async def update_many(self, data: "list[T]") -> list[T]:
+    async def update_many(self, data: list[T]) -> list[T]:
         """Update multiple instances with the attribute values present on instances in ``data``.
 
         Args:
-            data: A list of instance that should have a value for :attr:`id_attribute <AbstractRepository.id_attribute>` that exists in the
+            data: A list of instance that should have a value for :attr:`id_attribute <AbstractAsyncRepository.id_attribute>` that exists in the
                 collection.
 
         Returns:
             a list of the updated instances.
 
         Raises:
             NotFoundError: If no instance found with same identifier as ``data``.
@@ -191,15 +191,15 @@
 
         Updates instance with the attribute values present on ``data``, or creates a new instance if
         one doesn't exist.
 
         Args:
             data: Instance to update existing, or be created. Identifier used to determine if an
                 existing instance exists is the value of an attribute on ``data`` named as value of
-                :attr:`id_attribute <AbstractRepository.id_attribute>`.
+                :attr:`id_attribute <AbstractAsyncRepository.id_attribute>`.
 
         Returns:
             The updated or created instance.
 
         Raises:
             NotFoundError: If no instance found with same identifier as ``data``.
         """
@@ -213,72 +213,76 @@
             **kwargs: Instance attribute value filters.
 
         Returns:
             a tuple containing The list of instances, after filtering applied, and a count of records returned by query, ignoring pagination.
         """
 
     @abstractmethod
-    async def list(self, *filters: FilterTypes, **kwargs: Any) -> "list[T]":
+    async def list(self, *filters: FilterTypes, **kwargs: Any) -> list[T]:
         """Get a list of instances, optionally filtered.
 
         Args:
-            *filters: Types for specific filtering operations.
+            *filters: filters for specific filtering operations
             **kwargs: Instance attribute value filters.
 
         Returns:
-            The list of instances, after filtering applied.
+            The list of instances, after filtering applied
         """
 
     @abstractmethod
     def filter_collection_by_kwargs(self, collection: CollectionT, /, **kwargs: Any) -> CollectionT:
         """Filter the collection by kwargs.
 
         Has ``AND`` semantics where multiple kwargs name/value pairs are provided.
 
         Args:
-            collection: the collection to be filtered
+            collection: the objects to be filtered
             **kwargs: key/value pairs such that objects remaining in the collection after filtering
                 have the property that their attribute named ``key`` has value equal to ``value``.
 
+
+        Returns:
+            The filtered objects
+
         Raises:
-            RepositoryError: if a named attribute doesn't exist on :attr:`model_type <AbstractRepository.model_type>`.
+            RepositoryError: if a named attribute doesn't exist on :attr:`model_type <AbstractAsyncRepository.model_type>`.
         """
 
     @staticmethod
     def check_not_found(item_or_none: T | None) -> T:
         """Raise :class:`NotFoundError` if ``item_or_none`` is ``None``.
 
         Args:
-            item_or_none: Item to be tested for existence.
+            item_or_none: Item (:class:`T <T>`) to be tested for existence.
 
         Returns:
             The item, if it exists.
         """
         if item_or_none is None:
             raise NotFoundError("No item found when one was expected")
         return item_or_none
 
     @classmethod
-    def get_id_attribute_value(cls, item: T) -> Any:
-        """Get value of attribute named as :attr:`id_attribute <AbstractRepository.id_attribute>` on ``item``.
+    def get_id_attribute_value(cls, item: T | type[T]) -> Any:
+        """Get value of attribute named as :attr:`id_attribute <AbstractAsyncRepository.id_attribute>` on ``item``.
 
         Args:
-            item: Anything that should have an attribute named as :attr:`id_attribute <AbstractRepository.id_attribute>` value.
+            item: Anything that should have an attribute named as :attr:`id_attribute <AbstractAsyncRepository.id_attribute>` value.
 
         Returns:
-            The value of attribute on ``item`` named as :attr:`id_attribute <AbstractRepository.id_attribute>`.
+            The value of attribute on ``item`` named as :attr:`id_attribute <AbstractAsyncRepository.id_attribute>`.
         """
         return getattr(item, cls.id_attribute)
 
     @classmethod
     def set_id_attribute_value(cls, item_id: Any, item: T) -> T:
         """Return the ``item`` after the ID is set to the appropriate attribute.
 
         Args:
             item_id: Value of ID to be set on instance
-            item: Anything that should have an attribute named as :attr:`id_attribute <AbstractRepository.id_attribute>` value.
+            item: Anything that should have an attribute named as :attr:`id_attribute <AbstractAsyncRepository.id_attribute>` value.
 
         Returns:
-            Item with ``item_id`` set to :attr:`id_attribute <AbstractRepository.id_attribute>`
+            Item with ``item_id`` set to :attr:`id_attribute <AbstractAsyncRepository.id_attribute>`
         """
         setattr(item, cls.id_attribute, item_id)
         return item
```

### Comparing `litestar-2.0.0a4/litestar/contrib/repository/filters.py` & `litestar-2.0.0a5/litestar/contrib/repository/filters.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 """Collection filter datastructures."""
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, Generic, TypeVar
+from typing import TYPE_CHECKING, Generic, Literal, TypeVar
 
 if TYPE_CHECKING:
     from collections import abc
     from datetime import datetime
 
 T = TypeVar("T")
 
-__all__ = (
-    "BeforeAfter",
-    "CollectionFilter",
-    "LimitOffset",
-)
+__all__ = ["BeforeAfter", "CollectionFilter", "LimitOffset", "OrderBy", "SearchFilter"]
 
 
 @dataclass
 class BeforeAfter:
     """Data required to filter a query on a ``datetime`` column."""
 
     field_name: str
@@ -43,7 +39,29 @@
 class LimitOffset:
     """Data required to add limit/offset filtering to a query."""
 
     limit: int
     """Value for ``LIMIT`` clause of query."""
     offset: int
     """Value for ``OFFSET`` clause of query."""
+
+
+@dataclass
+class OrderBy(Generic[T]):
+    """Data required to construct a ``ORDER BY ...`` clause."""
+
+    field_name: str
+    """Name of the model attribute to sort on."""
+    sort_order: Literal["asc", "desc"]
+    """Sort ascending or descending"""
+
+
+@dataclass
+class SearchFilter(Generic[T]):
+    """Data required to construct a ``WHERE field_name LIKE '%' || :value || '%'`` clause."""
+
+    field_name: str
+    """Name of the model attribute to sort on."""
+    value: str
+    """Values for ``LIKE`` clause."""
+    ignore_case: bool | None = False
+    """Should the search be case insensitive."""
```

### Comparing `litestar-2.0.0a4/litestar/contrib/repository/testing/generic_mock_repository.py` & `litestar-2.0.0a5/litestar/contrib/repository/testing/generic_mock_repository.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,39 +4,40 @@
 """
 from __future__ import annotations
 
 from datetime import datetime, timezone, tzinfo
 from typing import TYPE_CHECKING, Generic, Protocol, TypeVar
 from uuid import uuid4
 
-from litestar.contrib.repository.abc import AbstractRepository
+from litestar.contrib.repository.abc import AbstractAsyncRepository
 from litestar.contrib.repository.exceptions import ConflictError, RepositoryError
 
 if TYPE_CHECKING:
     from collections.abc import Callable, Hashable, Iterable, MutableMapping
     from typing import Any
 
     from litestar.contrib.repository import FilterTypes
 
 ModelT = TypeVar("ModelT", bound="HasID")
-MockRepoT = TypeVar("MockRepoT", bound="GenericMockRepository")
+MockRepoT = TypeVar("MockRepoT", bound="GenericAsyncMockRepository")
 
 
 class HasID(Protocol):
     id: Any
 
 
-class GenericMockRepository(AbstractRepository[ModelT], Generic[ModelT]):
+class GenericAsyncMockRepository(AbstractAsyncRepository[ModelT], Generic[ModelT]):
     """A repository implementation for tests.
 
     Uses a :class:`dict` for storage.
     """
 
     collection: MutableMapping[Hashable, ModelT]
     model_type: type[ModelT]
+    match_fields: list[str] | str | None = None
 
     _model_has_created: bool
     _model_has_updated: bool
 
     def __init__(
         self, id_factory: Callable[[], Any] = uuid4, tz: tzinfo = timezone.utc, allow_ids_on_add: bool = False, **_: Any
     ) -> None:
@@ -175,26 +176,43 @@
             The retrieved instance.
 
         Raises:
             NotFoundError: If no instance found identified by ``item_id``.
         """
         return self._find_or_raise_not_found(item_id)
 
-    async def get_or_create(self, **kwargs: Any) -> tuple[ModelT, bool]:
+    async def get_or_create(self, match_fields: list[str] | str | None = None, **kwargs: Any) -> tuple[ModelT, bool]:
         """Get instance identified by ``kwargs`` or create if it doesn't exist.
 
         Args:
+            match_fields: a list of keys to use to match the existing model.  When empty, all fields are matched.
             **kwargs: Identifier of the instance to be retrieved.
 
         Returns:
             a tuple that includes the instance and whether it needed to be created.
 
         """
-        existing = await self.get_one_or_none(**kwargs)
+        match_fields = match_fields if match_fields else self.match_fields
+        if isinstance(match_fields, str):
+            match_fields = [match_fields]
+        if match_fields:
+            match_filter = {
+                field_name: field_value
+                for field_name in match_fields
+                if (field_value := kwargs.get(field_name)) is not None
+            }
+        else:
+            match_filter = kwargs
+        existing = await self.get_one_or_none(**match_filter)
         if existing:
+            for field_name, new_field_value in kwargs.items():
+                field = getattr(existing, field_name, None)
+                if field and field != new_field_value:
+                    setattr(existing, field_name, new_field_value)
+
             return existing, False
         return await self.add(self.model_type(**kwargs)), True
 
     async def get_one(self, **kwargs: Any) -> ModelT:
         """Get instance identified by query filters.
 
         Args:
@@ -233,15 +251,15 @@
         """
         return len(await self.list(*filters, **kwargs))
 
     async def update(self, data: ModelT) -> ModelT:
         """Update instance with the attribute values present on ``data``.
 
         Args:
-            data: An instance that should have a value for :attr:`id_attribute <GenericMockRepository.id_attribute>` that exists in the
+            data: An instance that should have a value for :attr:`id_attribute <AsyncGenericMockRepository.id_attribute>` that exists in the
                 collection.
 
         Returns:
             The updated instance.
 
         Raises:
             NotFoundError: If no instance found with same identifier as ``data``.
@@ -254,15 +272,15 @@
             setattr(item, key, val)
         return item
 
     async def update_many(self, data: list[ModelT]) -> list[ModelT]:
         """Update instances with the attribute values present on ``data``.
 
         Args:
-            data: A list of instances that should have a value for :attr:`id_attribute <GenericMockRepository.id_attribute>`
+            data: A list of instances that should have a value for :attr:`id_attribute <AsyncGenericMockRepository.id_attribute>`
                 that exists in the collection.
 
         Returns:
             The updated instances.
 
         Raises:
             NotFoundError: If no instance found with same identifier as ``data``.
@@ -282,15 +300,15 @@
 
         Updates instance with the attribute values present on ``data``, or creates a new instance if
         one doesn't exist.
 
         Args:
             data: Instance to update existing, or be created. Identifier used to determine if an
                 existing instance exists is the value of an attribute on `data` named as value of
-                :attr:`id_attribute <GenericMockRepository.id_attribute>`.
+                :attr:`id_attribute <AsyncGenericMockRepository.id_attribute>`.
 
         Returns:
             The updated or created instance.
 
         Raises:
             NotFoundError: If no instance found with same identifier as ``data``.
         """
@@ -311,15 +329,15 @@
             **kwargs: Instance attribute value filters.
 
         Returns:
             List of instances, and count of records returned by query, ignoring pagination.
         """
         return await self.list(*filters, **kwargs), await self.count(*filters, **kwargs)
 
-    async def list(self, *filters: "FilterTypes", **kwargs: Any) -> list[ModelT]:
+    async def list(self, *filters: FilterTypes, **kwargs: Any) -> list[ModelT]:
         """Get a list of instances, optionally filtered.
 
         Args:
             *filters: Types for specific filtering operations.
             **kwargs: Instance attribute value filters.
 
         Returns:
```

### Comparing `litestar-2.0.0a4/litestar/contrib/sqlalchemy/base.py` & `litestar-2.0.0a5/litestar/contrib/sqlalchemy/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 """Application ORM configuration."""
 from __future__ import annotations
 
 import re
 from datetime import datetime
-from typing import Any, TypeVar
+from typing import TYPE_CHECKING, Any, ClassVar, Protocol, TypeVar, runtime_checkable
 from uuid import UUID, uuid4
 
 from pydantic import AnyHttpUrl, AnyUrl, EmailStr
-from sqlalchemy import JSON, MetaData, String, Uuid
+from sqlalchemy import MetaData, String
 from sqlalchemy.event import listens_for
 from sqlalchemy.orm import (
     DeclarativeBase,
     Mapped,
     Session,
     declarative_mixin,
     declared_attr,
     mapped_column,
     registry,
 )
 
+from .types import GUID, JSON
+
+if TYPE_CHECKING:
+    from sqlalchemy.sql import FromClause
+
 __all__ = ("AuditBase", "AuditColumns", "Base", "CommonTableAttributes", "UUIDPrimaryKey", "touch_updated_timestamp")
 
 
 BaseT = TypeVar("BaseT", bound="Base")
 
 convention = {
     "ix": "ix_%(column_0_label)s",
@@ -47,14 +52,30 @@
             session.
     """
     for instance in session.dirty:
         if hasattr(instance, "updated"):
             instance.updated = datetime.now()  # noqa: DTZ005
 
 
+@runtime_checkable
+class ModelProtocol(Protocol):
+    """The base SQLAlchemy model protocol."""
+
+    __table__: FromClause
+    __name__: ClassVar[str]
+
+    def to_dict(self, exclude: set[str] | None = None) -> dict[str, Any]:
+        """Convert model to dictionary.
+
+        Returns:
+            dict[str, Any]: A dict representation of the model
+        """
+        ...
+
+
 @declarative_mixin
 class UUIDPrimaryKey:
     """UUID Primary Key Field Mixin."""
 
     __abstract__ = True
 
     id: Mapped[UUID] = mapped_column(default=uuid4, primary_key=True)
@@ -74,16 +95,16 @@
 
 
 @declarative_mixin
 class CommonTableAttributes:
     """Common attributes for SQLALchemy tables."""
 
     __abstract__ = True
-    __name__: str
-    __table__: Any
+    __name__: ClassVar[str]
+    __table__: FromClause
 
     # noinspection PyMethodParameters
     @declared_attr.directive
     def __tablename__(cls) -> str:  # pylint: disable=no-self-argument
         """Infer table name from class name."""
         regexp = re.compile("((?<=[a-z0-9])[A-Z]|(?!^)[A-Z](?=[a-z]))")
         return regexp.sub(r"_\1", cls.__name__).lower()
@@ -97,15 +118,15 @@
         exclude = set(exclude) if exclude else set()
         return {field.name: getattr(self, field.name) for field in self.__table__.columns if field.name not in exclude}
 
 
 meta = MetaData(naming_convention=convention)
 orm_registry = registry(
     metadata=meta,
-    type_annotation_map={UUID: Uuid, EmailStr: String, AnyUrl: String, AnyHttpUrl: String, dict: JSON},
+    type_annotation_map={UUID: GUID, EmailStr: String, AnyUrl: String, AnyHttpUrl: String, dict: JSON},
 )
 
 
 class Base(CommonTableAttributes, UUIDPrimaryKey, DeclarativeBase):
     """Base for all SQLAlchemy declarative models."""
 
     registry = orm_registry
```

### Comparing `litestar-2.0.0a4/litestar/contrib/sqlalchemy/init_plugin/config/asyncio.py` & `litestar-2.0.0a5/litestar/contrib/sqlalchemy/plugins/init/config/asyncio.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/contrib/sqlalchemy/init_plugin/config/common.py` & `litestar-2.0.0a5/litestar/contrib/sqlalchemy/plugins/init/config/common.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/contrib/sqlalchemy/init_plugin/config/engine.py` & `litestar-2.0.0a5/litestar/contrib/sqlalchemy/plugins/init/config/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     label_length: int | None | EmptyType = Empty
     """Optional integer value which limits the size of dynamically generated column labels to that many characters. If
     less than 6, labels are generated as “_(counter)”. If ``None``, the value of ``dialect.max_identifier_length``,
     which may be affected via the
     :attr:`create_engine.max_identifier_length parameter <sqlalchemy.create_engine.params.max_identifier_length>`, is
     used instead. The value of
     :attr:`create_engine.label_length <sqlalchemy.create_engine.params.label_length>` may not be larger than that of
-    :attr:`create_engine.max_identfier_length <sqlalchemy.create_engine.params.max_identifier_length>`."""
+    :attr:`create_engine.max_identifier_length <sqlalchemy.create_engine.params.max_identifier_length>`."""
     logging_name: str | EmptyType = Empty
     """String identifier which will be used within the “name” field of logging records generated within the
     “sqlalchemy.engine” logger. Defaults to a hexstring of the object`s id."""
     max_identifier_length: int | None | EmptyType = Empty
     """Override the max_identifier_length determined by the dialect. if ``None`` or ``0``, has no effect. This is the
     database`s configured maximum number of characters that may be used in a SQL identifier such as a table name, column
     name, or label name. All dialects determine this value automatically, however in the case of a new database version
```

### Comparing `litestar-2.0.0a4/litestar/contrib/sqlalchemy/init_plugin/config/sync.py` & `litestar-2.0.0a5/litestar/contrib/sqlalchemy/plugins/init/config/sync.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/contrib/sqlalchemy/init_plugin/plugin.py` & `litestar-2.0.0a5/litestar/contrib/sqlalchemy/plugins/init/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
+from litestar.contrib.sqlalchemy.plugins import _slots_base
 from litestar.di import Provide
 from litestar.plugins import InitPluginProtocol
 
 if TYPE_CHECKING:
     from litestar.config.app import AppConfig
 
     from .config import SQLAlchemyAsyncConfig, SQLAlchemySyncConfig
 
 __all__ = ("SQLAlchemyInitPlugin",)
 
 
-class SQLAlchemyInitPlugin(InitPluginProtocol):
+class SQLAlchemyInitPlugin(InitPluginProtocol, _slots_base.SlotsBase):
     """SQLAlchemy application lifecycle configuration."""
 
-    __slots__ = ("_config",)
+    __slots__ = ()
 
     def __init__(self, config: SQLAlchemyAsyncConfig | SQLAlchemySyncConfig) -> None:
         """Initialize ``SQLAlchemyPlugin``.
 
         Args:
             config: configure DB connection and hook handlers and dependencies.
         """
```

### Comparing `litestar-2.0.0a4/litestar/contrib/sqlalchemy/repository.py` & `litestar-2.0.0a5/litestar/contrib/sqlalchemy/repository.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,40 +4,43 @@
 from contextlib import contextmanager
 from typing import TYPE_CHECKING, Any, Generic, Literal, Tuple, TypeVar, cast
 
 from sqlalchemy import Select, delete, over, select, text, update
 from sqlalchemy import func as sql_func
 from sqlalchemy.exc import IntegrityError, SQLAlchemyError
 
-from litestar.contrib.repository.abc import AbstractRepository
+from litestar.contrib.repository.abc import AbstractAsyncRepository
 from litestar.contrib.repository.exceptions import ConflictError, RepositoryError
 from litestar.contrib.repository.filters import (
     BeforeAfter,
     CollectionFilter,
     LimitOffset,
+    OrderBy,
+    SearchFilter,
 )
 
 if TYPE_CHECKING:
     from collections import abc
     from datetime import datetime
 
     from sqlalchemy.engine import Result
     from sqlalchemy.ext.asyncio import AsyncSession
 
     from litestar.contrib.repository import FilterTypes
-    from litestar.contrib.sqlalchemy import base
+
+    from . import base
 
 __all__ = (
-    "SQLAlchemyRepository",
+    "SQLAlchemyAsyncRepository",
     "ModelT",
 )
 
 T = TypeVar("T")
-ModelT = TypeVar("ModelT", bound="base.Base | base.AuditBase")
-SQLARepoT = TypeVar("SQLARepoT", bound="SQLAlchemyRepository")
+ModelT = TypeVar("ModelT", bound="base.ModelProtocol")
+SQLARepoT = TypeVar("SQLARepoT", bound="SQLAlchemyAsyncRepository")
 SelectT = TypeVar("SelectT", bound="Select[Any]")
 RowT = TypeVar("RowT", bound=Tuple[Any, ...])
 
 
 @contextmanager
 def wrap_sqlalchemy_exception() -> Any:
     """Do something within context to raise a `RepositoryError` chained
@@ -55,31 +58,31 @@
         yield
     except IntegrityError as exc:
         raise ConflictError from exc
     except SQLAlchemyError as exc:
         raise RepositoryError(f"An exception occurred: {exc}") from exc
 
 
-class SQLAlchemyRepository(AbstractRepository[ModelT], Generic[ModelT]):
+class SQLAlchemyAsyncRepository(AbstractAsyncRepository[ModelT], Generic[ModelT]):
     """SQLAlchemy based implementation of the repository interface."""
 
-    def __init__(
-        self, *, session: AsyncSession, base_select: Select[tuple[ModelT]] | None = None, **kwargs: Any
-    ) -> None:
+    match_fields: list[str] | str | None = None
+
+    def __init__(self, *, statement: Select[tuple[ModelT]] | None = None, session: AsyncSession, **kwargs: Any) -> None:
         """Repository pattern for SQLAlchemy models.
 
         Args:
+            statement: To facilitate customization of the underlying select query.
             session: Session managing the unit-of-work for the operation.
-            base_select: To facilitate customization of the underlying select query.
             **kwargs: Additional arguments.
 
         """
         super().__init__(**kwargs)
         self.session = session
-        self.statement = base_select if base_select is not None else select(self.model_type)
+        self.statement = statement if statement is not None else select(self.model_type)
 
     async def add(self, data: ModelT) -> ModelT:
         """Add `data` to the collection.
 
         Args:
             data: Instance to be added to the collection.
 
@@ -107,24 +110,24 @@
             self.session.add_all(data)
             await self.session.flush()
             for datum in data:
                 self.session.expunge(datum)
             return data
 
     async def delete(self, item_id: Any) -> ModelT:
-        """Delete instance identified by `item_id`.
+        """Delete instance identified by ``item_id``.
 
         Args:
             item_id: Identifier of instance to be deleted.
 
         Returns:
             The deleted instance.
 
         Raises:
-            NotFoundError: If no instance found identified by `item_id`.
+            NotFoundError: If no instance found identified by ``item_id``.
         """
         with wrap_sqlalchemy_exception():
             instance = await self.get(item_id)
             await self.session.delete(instance)
             await self.session.flush()
             self.session.expunge(instance)
             return instance
@@ -189,15 +192,15 @@
         Returns:
             The retrieved instance.
 
         Raises:
             NotFoundError: If no instance found identified by `item_id`.
         """
         with wrap_sqlalchemy_exception():
-            statement = kwargs.pop("base_select", self.statement)
+            statement = kwargs.pop("statement", self.statement)
             statement = self._filter_select_by_kwargs(statement=statement, **{self.id_attribute: item_id})
             instance = (await self._execute(statement)).scalar_one_or_none()
             instance = self.check_not_found(instance)
             self.session.expunge(instance)
             return instance
 
     async def get_one(self, **kwargs: Any) -> ModelT:
@@ -209,15 +212,15 @@
         Returns:
             The retrieved instance.
 
         Raises:
             NotFoundError: If no instance found identified by `item_id`.
         """
         with wrap_sqlalchemy_exception():
-            statement = kwargs.pop("base_select", self.statement)
+            statement = kwargs.pop("statement", self.statement)
             statement = self._filter_select_by_kwargs(statement=statement, **kwargs)
             instance = (await self._execute(statement)).scalar_one_or_none()
             instance = self.check_not_found(instance)
             self.session.expunge(instance)
             return instance
 
     async def get_one_or_none(self, **kwargs: Any) -> ModelT | None:
@@ -226,50 +229,70 @@
         Args:
             **kwargs: Identifier of the instance to be retrieved.
 
         Returns:
             The retrieved instance or None
         """
         with wrap_sqlalchemy_exception():
-            statement = kwargs.pop("base_select", self.statement)
+            statement = kwargs.pop("statement", self.statement)
             statement = self._filter_select_by_kwargs(statement=statement, **kwargs)
             instance = (await self._execute(statement)).scalar_one_or_none()
             if instance:
                 self.session.expunge(instance)
             return instance  # type: ignore
 
-    async def get_or_create(self, **kwargs: Any) -> tuple[ModelT, bool]:
+    async def get_or_create(
+        self, match_fields: list[str] | str | None = None, upsert: bool = True, **kwargs: Any
+    ) -> tuple[ModelT, bool]:
         """Get instance identified by ``kwargs`` or create if it doesn't exist.
 
         Args:
+            match_fields: a list of keys to use to match the existing model.  When empty, all fields are matched.
+            upsert: When using match_fields and actual model values differ from `kwargs`, perform an update operation on the model.
             **kwargs: Identifier of the instance to be retrieved.
 
         Returns:
-            a tuple that includes the instance and whether or not it needed to be created.
+            a tuple that includes the instance and whether or not it needed to be created.  When using match_fields and actual model values differ from `kwargs`, the model value will be updated.
         """
-        existing = await self.get_one_or_none(**kwargs)
-        if existing:
-            return existing, False
-        return await self.add(self.model_type(**kwargs)), True  # type: ignore[arg-type]
+        match_fields = match_fields if match_fields else self.match_fields
+        if isinstance(match_fields, str):
+            match_fields = [match_fields]
+        if match_fields:
+            match_filter = {
+                field_name: kwargs.get(field_name, None)
+                for field_name in match_fields
+                if kwargs.get(field_name, None) is not None
+            }
+        else:
+            match_filter = kwargs
+        existing = await self.get_one_or_none(**match_filter)
+        if not existing:
+            return await self.add(self.model_type(**kwargs)), True
+        if upsert:
+            for field_name, new_field_value in kwargs.items():
+                field = getattr(existing, field_name, None)
+                if field and field != new_field_value:
+                    setattr(existing, field_name, new_field_value)
+            if existing in self.session.dirty:
+                return (await self.update(existing)), False
+        return existing, False
 
     async def count(self, *filters: FilterTypes, **kwargs: Any) -> int:
         """Get the count of records returned by a query.
 
         Args:
             *filters: Types for specific filtering operations.
             **kwargs: Instance attribute value filters.
 
         Returns:
             Count of records returned by query, ignoring pagination.
         """
-        statement = kwargs.pop("base_select", self.statement)
+        statement = kwargs.pop("statement", self.statement)
         statement = statement.with_only_columns(
-            sql_func.count(
-                self.model_type.id,
-            ),
+            sql_func.count(self.get_id_attribute_value(self.model_type)),
             maintain_column_froms=True,
         ).order_by(None)
         statement = self._apply_filters(*filters, apply_pagination=False, statement=statement)
         statement = self._filter_select_by_kwargs(statement, **kwargs)
         results = await self._execute(statement)
         return results.scalar_one()  # type: ignore
 
@@ -344,22 +367,16 @@
         Args:
             *filters: Types for specific filtering operations.
             **kwargs: Instance attribute value filters.
 
         Returns:
             Count of records returned by query, ignoring pagination.
         """
-        statement = kwargs.pop("base_select", self.statement)
-        statement = statement.add_columns(
-            over(
-                sql_func.count(
-                    self.model_type.id,
-                ),
-            )
-        )
+        statement = kwargs.pop("statement", self.statement)
+        statement = statement.add_columns(over(sql_func.count(self.get_id_attribute_value(self.model_type))))
         statement = self._apply_filters(*filters, statement=statement)
         statement = self._filter_select_by_kwargs(statement, **kwargs)
         with wrap_sqlalchemy_exception():
             result = await self._execute(statement)
             count: int = 0
             instances: list[ModelT] = []
             for i, (instance, count_value) in enumerate(result):
@@ -375,15 +392,15 @@
         Args:
             *filters: Types for specific filtering operations.
             **kwargs: Instance attribute value filters.
 
         Returns:
             The list of instances, after filtering applied.
         """
-        statement = kwargs.pop("base_select", self.statement)
+        statement = kwargs.pop("statement", self.statement)
         statement = self._apply_filters(*filters, statement=statement)
         statement = self._filter_select_by_kwargs(statement, **kwargs)
 
         with wrap_sqlalchemy_exception():
             result = await self._execute(statement)
             instances = list(result.scalars())
             for instance in instances:
@@ -489,14 +506,20 @@
                     statement = self._apply_limit_offset_pagination(filter_.limit, filter_.offset, statement=statement)
             elif isinstance(filter_, BeforeAfter):
                 statement = self._filter_on_datetime_field(
                     filter_.field_name, filter_.before, filter_.after, statement=statement
                 )
             elif isinstance(filter_, CollectionFilter):
                 statement = self._filter_in_collection(filter_.field_name, filter_.values, statement=statement)
+            elif isinstance(filter_, OrderBy):
+                statement = self._order_by(statement, filter_.field_name, sort_desc=bool(filter_.sort_order == "desc"))
+            elif isinstance(filter_, SearchFilter):
+                statement = self._filter_by_like(
+                    statement, filter_.field_name, value=filter_.value, ignore_case=bool(filter_.ignore_case)
+                )
             else:
                 raise RepositoryError(f"Unexpected filter: {filter_}")
         return statement
 
     def _filter_in_collection(self, field_name: str, values: abc.Collection[Any], statement: SelectT) -> SelectT:
         if not values:
             return statement
@@ -512,7 +535,16 @@
             statement = statement.where(field > before)
         return statement
 
     def _filter_select_by_kwargs(self, statement: SelectT, **kwargs: Any) -> SelectT:
         for key, val in kwargs.items():
             statement = statement.where(getattr(self.model_type, key) == val)
         return statement
+
+    def _filter_by_like(self, statement: SelectT, field_name: str, value: str, ignore_case: bool) -> SelectT:
+        field = getattr(self.model_type, field_name)
+        search_text = f"%{value}%"
+        return statement.where(field.ilike(search_text) if ignore_case else field.like(search_text))
+
+    def _order_by(self, statement: SelectT, field_name: str, sort_desc: bool = False) -> SelectT:
+        field = getattr(self.model_type, field_name)
+        return statement.order_by(field.desc() if sort_desc else field.asc())
```

### Comparing `litestar-2.0.0a4/litestar/contrib/sqlalchemy_1/config.py` & `litestar-2.0.0a5/litestar/logging/config.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,336 +1,340 @@
 from __future__ import annotations
 
+from abc import ABC, abstractmethod
 from dataclasses import asdict, dataclass, field
+from importlib.util import find_spec
+from logging import INFO
 from typing import TYPE_CHECKING, Any, Callable, Literal, cast
 
 from litestar.exceptions import ImproperlyConfiguredException, MissingDependencyException
-from litestar.logging.config import BaseLoggingConfig, LoggingConfig
-from litestar.serialization import decode_json, encode_json
-from litestar.utils import AsyncCallable
+from litestar.serialization import encode_json
 
-try:
-    import sqlalchemy  # noqa: F401
-except ImportError as e:
-    raise MissingDependencyException("sqlalchemy") from e
-
-from sqlalchemy import create_engine
-from sqlalchemy.ext.asyncio import AsyncEngine, AsyncSession, create_async_engine
-from sqlalchemy.orm import Query, Session, sessionmaker
-
-__all__ = ("SQLAlchemyConfig", "SQLAlchemyEngineConfig", "SQLAlchemySessionConfig")
+__all__ = ("BaseLoggingConfig", "LoggingConfig", "StructLoggingConfig")
 
 
 if TYPE_CHECKING:
-    from sqlalchemy.engine import Engine
-    from sqlalchemy.future import Engine as FutureEngine
-    from sqlalchemy.pool import Pool
-
-    from litestar.datastructures.state import State
-    from litestar.types import BeforeMessageSendHookHandler, Message, Scope
+    from typing import NoReturn
 
-    from .types import SessionMakerInstanceProtocol, SessionMakerTypeProtocol
+    # these imports are duplicated on purpose so sphinx autodoc can find and link them
+    from structlog.types import BindableLogger, Processor, WrappedLogger
 
-IsolationLevel = Literal["AUTOCOMMIT", "READ COMMITTED", "READ UNCOMMITTED", "REPEATABLE READ", "SERIALIZABLE"]
+    from litestar.types import Logger, Scope
+    from litestar.types.callable_types import ExceptionLoggingHandler, GetLogger
 
-SESSION_SCOPE_KEY = "_sql_alchemy_db_session"
-SESSION_TERMINUS_ASGI_EVENTS = {"http.response.start", "http.disconnect", "websocket.disconnect", "websocket.close"}
 
+try:
+    from structlog.types import BindableLogger, Processor, WrappedLogger  # noqa: F811
+except ImportError:
+    BindableLogger = Any  # type: ignore
+    Processor = Any  # type: ignore
+    WrappedLogger = Any  # type: ignore
+
+
+default_handlers: dict[str, dict[str, Any]] = {
+    "console": {
+        "class": "logging.StreamHandler",
+        "level": "DEBUG",
+        "formatter": "standard",
+    },
+    "queue_listener": {
+        "class": "litestar.logging.standard.QueueListenerHandler",
+        "level": "DEBUG",
+        "formatter": "standard",
+    },
+}
+
+default_picologging_handlers: dict[str, dict[str, Any]] = {
+    "console": {
+        "class": "picologging.StreamHandler",
+        "level": "DEBUG",
+        "formatter": "standard",
+    },
+    "queue_listener": {
+        "class": "litestar.logging.picologging.QueueListenerHandler",
+        "level": "DEBUG",
+        "formatter": "standard",
+    },
+}
+
+
+def get_logger_placeholder(_: str) -> NoReturn:  # pragma: no cover
+    """Raise: An :class:`ImproperlyConfiguredException <.exceptions.ImproperlyConfiguredException>`"""
+    raise ImproperlyConfiguredException(
+        "cannot call '.get_logger' without passing 'logging_config' to the Litestar constructor first"
+    )
 
-def serializer(value: Any) -> str:
-    """Serialize JSON field values.
 
-    Args:
-        value: Any json serializable value.
+def _get_default_handlers() -> dict[str, dict[str, Any]]:
+    """Return the default logging handlers for the config.
 
     Returns:
-        JSON string.
+        A dictionary of logging handlers
     """
-    return encode_json(value).decode("utf-8")
+    if find_spec("picologging"):
+        return default_picologging_handlers
+    return default_handlers
 
 
-async def default_before_send_handler(message: "Message", _: "State", scope: "Scope") -> None:
-    """Handle closing and cleaning up sessions before sending.
+def _default_exception_logging_handler_factory(
+    is_struct_logger: bool, traceback_line_limit: int
+) -> ExceptionLoggingHandler:
+    """Create an exception logging handler function.
 
     Args:
-        message: ASGI-``Message``
-        _: A ``State`` (not used)
-        scope: An ASGI-``Scope``
+        is_struct_logger: Whether the logger is a structlog instance.
+        traceback_line_limit: Maximal number of lines to log from the
+            traceback.
 
     Returns:
-        None
+        An exception logging handler.
     """
-    session = cast("Session | AsyncSession | None", scope.get(SESSION_SCOPE_KEY))
-    if session and message["type"] in SESSION_TERMINUS_ASGI_EVENTS:
-        if isinstance(session, AsyncSession):
-            await session.close()
+
+    def _default_exception_logging_handler(logger: Logger, scope: Scope, tb: list[str]) -> None:
+        # we limit the length of the stack trace to 20 lines.
+        first_line = tb.pop(0)
+
+        if is_struct_logger:
+            logger.exception(
+                "uncaught exception",
+                connection_type=scope["type"],
+                path=scope["path"],
+                traceback="".join(tb[-traceback_line_limit:]),
+            )
         else:
-            session.close()
-        del scope[SESSION_SCOPE_KEY]  # type: ignore
+            stack_trace = first_line + "".join(tb[-traceback_line_limit:])
+            logger.exception(
+                "exception raised on %s connection to route %s\n\n%s", scope["type"], scope["path"], stack_trace
+            )
 
+    return _default_exception_logging_handler
 
-@dataclass
-class SQLAlchemySessionConfig:
-    """Configuration for a SQLAlchemy-Session."""
 
-    autocommit: bool | None = field(default=None)
-    autoflush: bool | None = field(default=None)
-    bind: Any | None = field(default=None)
-    binds: Any | None = field(default=None)
-    enable_baked_queries: bool | None = field(default=None)
-    expire_on_commit: bool = field(default=False)
-    future: bool | None = field(default=None)
-    info: dict[str, Any] | None = field(default=None)
-    query_cls: type[Query] | None = field(default=None)
-    twophase: bool | None = field(default=None)
+class BaseLoggingConfig(ABC):  # pragma: no cover
+    """Abstract class that should be extended by logging configs."""
 
+    __slots__ = ("log_exceptions", "traceback_line_limit", "exception_logging_handler")
 
-@dataclass
-class SQLAlchemyEngineConfig:
-    """Configuration for SQLAlchemy's :class`Engine <sqlalchemy.engine.Engine>`.
+    log_exceptions: Literal["always", "debug", "never"]
+    """Should exceptions be logged, defaults to log exceptions when ``app.debug == True``'"""
+    traceback_line_limit: int
+    """Max number of lines to print for exception traceback"""
+    exception_logging_handler: ExceptionLoggingHandler | None
+    """Handler function for logging exceptions."""
 
-    For details see: https://docs.sqlalchemy.org/en/14/core/engines.html
-    """
+    @abstractmethod
+    def configure(self) -> GetLogger:
+        """Return logger with the given configuration.
 
-    connect_args: dict[str, Any] | None = field(default=None)
-    echo: bool | None = field(default=None)
-    echo_pool: bool | None = field(default=None)
-    enable_from_linting: bool | None = field(default=None)
-    future: bool = field(default=True)
-    hide_parameters: bool | None = field(default=None)
-    isolation_level: IsolationLevel | None = field(default=None)
-    json_deserializer: Callable[[str], Any] = field(default=decode_json)
-    json_serializer: Callable[[Any], str] = field(default=serializer)
-    label_length: int | None = field(default=None)
-    listeners: Any = field(default=None)
-    logging_level: int | str | None = field(default=None)
-    logging_name: str | None = field(default=None)
-    max_identifier_length: int | None = field(default=None)
-    max_overflow: int | None = field(default=None)
-    module: Any = field(default=None)
-    paramstyle: Literal["qmark", "numeric", "named", "format", "pyformat"] | None = field(default=None)
-    plugins: list[str] | None = field(default=None)
-    pool: Pool | None = field(default=None)
-    pool_logging_name: str | None = field(default=None)
-    pool_pre_ping: bool | None = field(default=None)
-    pool_recycle: int | None = field(default=None)
-    pool_reset_on_return: Literal["rollback", "commit"] | None = field(default=None)
-    pool_size: int | None = field(default=None)
-    pool_timeout: int | None = field(default=None)
-    pool_use_lifo: bool | None = field(default=None)
-    poolclass: type[Pool] | None = field(default=None)
-    query_cache_size: int | None = field(default=None)
-    strategy: str | None = field(default=None)
+        Returns:
+            A 'logging.getLogger' like function.
+        """
+        raise NotImplementedError("abstract method")
 
 
 @dataclass
-class SQLAlchemyConfig:
-    """Configuration for SQLAlchemy's :class:`sessionmaker <sqlalchemy.orm.sessionmaker>`.
-
-    For details see: https://docs.sqlalchemy.org/en/14/orm/session_api.html
-    """
-
-    connection_string: str | None = field(default=None)
-    """Database connection string in one of the formats supported by SQLAlchemy.
-
-    Notes:
-        - For async connections, the connection string must include the correct async prefix.
-          e.g. ``'postgresql+asyncpg://...'`` instead of ``'postgresql://'``, and for sync connections its the opposite.
-
-    """
-    use_async_engine: bool = field(default=True)
-    """Dictate whether the engine created is an async connection or not.
+class LoggingConfig(BaseLoggingConfig):
+    """Configuration class for standard logging.
 
     Notes:
-        - This option must correlate to the type of ``connection_string``. That is, an async connection string required an
-          async connection and vice versa.
-
+        - If 'picologging' is installed it will be used by default.
     """
-    create_async_engine_callable: Callable[[str], AsyncEngine] = field(default=create_async_engine)
-    """Callable that creates an :class:`AsyncEngine <sqlalchemy.ext.asyncio.AsyncEngine>` instance or instance of its
-    subclass.
-    """
-    create_engine_callable: Callable[[str], Engine | FutureEngine] = field(default=create_engine)
-    """Callable that creates an :class:`Engine <sqlalchemy.engine.Engine>` or ``FutureEngine`` instance or instance of its
-    subclass."""
-    dependency_key: str = field(default="db_session")
-    """Key to use for the dependency injection of database sessions."""
-    engine_app_state_key: str = field(default="db_engine")
-    """Key under which to store the SQLAlchemy engine in the application :class:`State <.datastructures.State>`
-    instance.
-    """
-    engine_config: SQLAlchemyEngineConfig = field(default_factory=SQLAlchemyEngineConfig)
-    """Configuration for the SQLAlchemy engine.
 
-    The configuration options are documented in the SQLAlchemy documentation.
-    """
-    set_json_serializers: bool = field(default=True)
-    """A boolean flag dictating whether to set ``msgspec`` based serializer/deserializer functions.
+    version: Literal[1] = field(default=1)
+    """The only valid value at present is 1."""
+    incremental: bool = field(default=False)
+    """Whether the configuration is to be interpreted as incremental to the existing configuration.
 
     Notes:
-        - Some databases or some versions of some databases do not have a JSON column type. E.g. some older versions of
-          SQLite for example. In this case this flag should be false or an error will be raised by SQLAlchemy.
-
+        - This option is ignored for 'picologging'
     """
-    session_class: type[Session] | type[AsyncSession] | None = field(default=None)
-    """The session class to use.
+    disable_existing_loggers: bool = field(default=False)
+    """Whether any existing non-root loggers are to be disabled."""
+    filters: dict[str, dict[str, Any]] | None = field(default=None)
+    """A dict in which each key is a filter id and each value is a dict describing how to configure the corresponding
+    Filter instance.
+    """
+    propagate: bool = field(default=True)
+    """If messages must propagate to handlers higher up the logger hierarchy from this logger."""
+    formatters: dict[str, dict[str, Any]] = field(
+        default_factory=lambda: {
+            "standard": {"format": "%(levelname)s - %(asctime)s - %(name)s - %(module)s - %(message)s"}
+        }
+    )
+    handlers: dict[str, dict[str, Any]] = field(default_factory=_get_default_handlers)
+    """A dict in which each key is a handler id and each value is a dict describing how to configure the corresponding
+    Handler instance.
+    """
+    loggers: dict[str, dict[str, Any]] = field(
+        default_factory=lambda: {
+            "litestar": {"level": "INFO", "handlers": ["queue_listener"], "propagate": False},
+        }
+    )
+    """A dict in which each key is a logger name and each value is a dict describing how to configure the corresponding
+    Logger instance.
+    """
+    root: dict[str, dict[str, Any] | list[Any] | str] = field(
+        default_factory=lambda: {
+            "handlers": ["queue_listener"],
+            "level": "INFO",
+        }
+    )
+    """This will be the configuration for the root logger.
 
-    If not set, the session class will default to :class:`sqlalchemy.orm.Session` for sync connections and
-    :class:`sqlalchemy.ext.asyncio.AsyncSession` for async ones.
+    Processing of the configuration will be as for any logger, except that the propagate setting will not be applicable.
     """
-    session_config: SQLAlchemySessionConfig = field(default_factory=SQLAlchemySessionConfig)
-    """Configuration options for the ``sessionmaker``.
+    log_exceptions: Literal["always", "debug", "never"] = field(default="debug")
+    """Should exceptions be logged, defaults to log exceptions when 'app.debug == True'"""
+    traceback_line_limit: int = field(default=20)
+    """Max number of lines to print for exception traceback"""
+    exception_logging_handler: ExceptionLoggingHandler | None = field(default=None)
+    """Handler function for logging exceptions."""
 
-    The configuration options are documented in the SQLAlchemy documentation.
-    """
-    session_maker_class: type[SessionMakerTypeProtocol] = field(default=sessionmaker)
-    """Sessionmaker class to use."""
-    session_maker_app_state_key: str = field(default="session_maker_class")
-    """Key under which to store the SQLAlchemy ``sessionmaker`` in the application
-    :class:`State <.datastructures.State>` instance.
-    """
-    session_maker_instance: SessionMakerInstanceProtocol | None = field(default=None)
-    """Optional sessionmaker to use.
+    def __post_init__(self) -> None:
+        if "queue_listener" not in self.handlers:
+            self.handlers["queue_listener"] = _get_default_handlers()["queue_listener"]
 
-    If set, the plugin will use the provided instance rather than instantiate a sessionmaker.
-    """
-    engine_instance: Engine | FutureEngine | AsyncEngine | None = field(default=None)
-    """Optional engine to use.
+        if "litestar" not in self.loggers:
+            self.loggers["litestar"] = {
+                "level": "INFO",
+                "handlers": ["queue_listener"],
+                "propagate": False,
+            }
 
-    If set, the plugin will use the provided instance rather than instantiate an engine.
-    """
-    before_send_handler: BeforeMessageSendHookHandler = field(default=default_before_send_handler)
-    """Handler to call before the ASGI message is sent.
+        if self.log_exceptions != "never" and self.exception_logging_handler is None:
+            self.exception_logging_handler = _default_exception_logging_handler_factory(
+                is_struct_logger=False, traceback_line_limit=self.traceback_line_limit
+            )
 
-    The handler should handle closing the session stored in the ASGI scope, if its still open, and committing and
-    uncommitted data.
-    """
+    def configure(self) -> GetLogger:
+        """Return logger with the given configuration.
 
-    def __post_init__(self) -> None:
-        if self.connection_string is None and self.engine_instance is None:
-            raise ImproperlyConfiguredException("One of 'connection_string' or 'engine_instance' must be provided.")
+        Returns:
+            A 'logging.getLogger' like function.
+        """
 
-        if self.connection_string is not None and self.engine_instance is not None:
-            raise ImproperlyConfiguredException("Only one of 'connection_string' or 'engine_instance' can be provided.")
+        if "picologging" in str(encode_json(self.handlers)):
+            try:
+                import picologging  # noqa: F401
+            except ImportError as e:
+                raise MissingDependencyException("picologging") from e
 
-        self.before_send_handler = AsyncCallable(self.before_send_handler)  # type: ignore
+            from picologging import config, getLogger
 
-    @property
-    def engine_config_dict(self) -> dict[str, Any]:
-        """Return the engine configuration as a dict.
+            values = {k: v for k, v in asdict(self).items() if v is not None and k != "incremental"}
+        else:
+            from logging import config, getLogger  # type: ignore[no-redef, assignment]
 
-        Returns:
-            A string keyed dict of config kwargs for the SQLAlchemy ``create_engine`` function.
-        """
-        engine_excluded_fields: set[str] = {"future", "logging_level"} if self.use_async_engine else {"logging_level"}
+            values = {k: v for k, v in asdict(self).items() if v is not None}
 
-        if not self.set_json_serializers:
-            engine_excluded_fields.update({"json_deserializer", "json_serializer"})
+        config.dictConfig(values)
+        return cast("Callable[[str], Logger]", getLogger)
 
-        return {
-            k: v for k, v in asdict(self.engine_config).items() if v is not None and k not in engine_excluded_fields
-        }
 
-    @property
-    def engine(self) -> Engine | FutureEngine | AsyncEngine:
-        """Return an engine. If none exists yet, create one.
+def default_structlog_processors() -> list[Processor] | None:  # pyright: ignore
+    """Set the default processors for structlog.
 
-        Returns:
-            Getter that returns the engine instance used by the plugin.
-        """
-        if not self.engine_instance:
-            create_engine_callable = (
-                self.create_async_engine_callable if self.use_async_engine else self.create_engine_callable
-            )
-            self.engine_instance = create_engine_callable(
-                self.connection_string, **self.engine_config_dict  # type:ignore[arg-type]
-            )
-        return cast("Engine | FutureEngine | AsyncEngine", self.engine_instance)
+    Returns:
+        An optional list of processors.
+    """
+    try:
+        import structlog
 
-    @property
-    def session_maker(self) -> sessionmaker:
-        """Get a sessionmaker. If none exists yet, create one.
+        return [
+            structlog.contextvars.merge_contextvars,
+            structlog.processors.add_log_level,
+            structlog.processors.format_exc_info,
+            structlog.processors.TimeStamper(fmt="iso"),
+            structlog.processors.JSONRenderer(serializer=encode_json),
+        ]
+    except ImportError:  # pragma: no cover
+        return None
 
-        Returns:
-            Getter that returns the session_maker instance used by the plugin.
-        """
-        if not self.session_maker_instance:
-            session_maker_kwargs = {
-                k: v
-                for k, v in asdict(self.session_config).items()
-                if v is not None and ((self.use_async_engine and k != "future") or not self.use_async_engine)
-            }
-            session_class = self.session_class or (AsyncSession if self.use_async_engine else Session)
-            self.session_maker_instance = self.session_maker_class(
-                self.engine, class_=session_class, **session_maker_kwargs
-            )
-        return cast("sessionmaker", self.session_maker_instance)
 
-    def create_db_session_dependency(self, state: State, scope: Scope) -> Union[Session, AsyncSession]:  # noqa: F821
-        """Create a session instance.
+def default_wrapper_class() -> type[BindableLogger] | None:  # pyright: ignore
+    """Set the default wrapper class for structlog.
 
-        Args:
-            state: The ``Litestar.state`` instance.
-            scope: The current connection's scope.
+    Returns:
+        An optional wrapper class.
+    """
 
-        Returns:
-            A session instance T.
-        """
-        session = scope.get(SESSION_SCOPE_KEY)
-        if not session:
-            session_maker = cast("sessionmaker", state[self.session_maker_app_state_key])
-            session = scope[SESSION_SCOPE_KEY] = session_maker()  # type: ignore
-        return cast("Session | AsyncSession", session)
+    try:
+        import structlog
 
-    def update_app_state(self, state: State) -> None:
-        """Create a DB engine and stores it in the application state.
+        return structlog.make_filtering_bound_logger(INFO)
+    except ImportError:  # pragma: no cover
+        return None
 
-        Args:
-            state: The ``Litestar.state`` instance.
 
-        Returns:
-            None
-        """
+def default_logger_factory() -> Callable[..., WrappedLogger] | None:
+    """Set the default logger factory for structlog.
 
-        state[self.engine_app_state_key] = self.engine
-        state[self.session_maker_app_state_key] = self.session_maker
+    Returns:
+        An optional logger factory.
+    """
+    try:
+        import structlog
 
-    async def on_shutdown(self, state: State) -> None:
-        """Disposes of the SQLAlchemy engine.
+        return structlog.BytesLoggerFactory()
+    except ImportError:  # pragma: no cover
+        return None
 
-        Args:
-            state: The ``Litestar.state`` instance.
 
-        Returns:
-            None
-        """
-        engine = cast("Engine | AsyncEngine", state[self.engine_app_state_key])
-        if isinstance(engine, AsyncEngine):
-            await engine.dispose()
-        else:
-            engine.dispose()
-        del state[self.engine_app_state_key]
+@dataclass
+class StructLoggingConfig(BaseLoggingConfig):
+    """Configuration class for structlog.
+
+    Notes:
+        - requires ``structlog`` to be installed.
+    """
 
-    def config_sql_alchemy_logging(self, logging_config: BaseLoggingConfig | None) -> None:
-        """Add the SQLAlchemy loggers to the logging config.
+    processors: list[Processor] | None = field(default_factory=default_structlog_processors)  # pyright: ignore
+    """Iterable of structlog logging processors."""
+    wrapper_class: type[BindableLogger] | None = field(default_factory=default_wrapper_class)  # pyright: ignore
+    """Structlog bindable logger."""
+    context_class: dict[str, Any] | None = None
+    """Context class (a 'contextvar' context) for the logger."""
+    logger_factory: Callable[..., WrappedLogger] | None = field(default_factory=default_logger_factory)
+    """Logger factory to use."""
+    cache_logger_on_first_use: bool = field(default=True)
+    """Whether to cache the logger configuration and reuse."""
+    log_exceptions: Literal["always", "debug", "never"] = field(default="debug")
+    """Should exceptions be logged, defaults to log exceptions when 'app.debug == True'"""
+    traceback_line_limit: int = field(default=20)
+    """Max number of lines to print for exception traceback"""
+    exception_logging_handler: ExceptionLoggingHandler | None = field(default=None)
+    """Handler function for logging exceptions."""
 
-        Notes:
-            - Currently only works with :class:`LoggingConfig <.logging.config.LoggingConfig>`.
+    def __post_init__(self) -> None:
+        if self.log_exceptions != "never" and self.exception_logging_handler is None:
+            self.exception_logging_handler = _default_exception_logging_handler_factory(
+                is_struct_logger=True, traceback_line_limit=self.traceback_line_limit
+            )
 
-        Args:
-            logging_config: Logging config.
+    def configure(self) -> GetLogger:
+        """Return logger with the given configuration.
 
         Returns:
-            None.
+            A 'logging.getLogger' like function.
         """
-        if isinstance(logging_config, LoggingConfig):
-            logger_settings = {
-                "level": self.engine_config.logging_level or "WARNING",
-                "handlers": logging_config.loggers["litestar"]["handlers"],
+        try:
+            import structlog  # noqa: F401
+        except ImportError as e:
+            raise MissingDependencyException("structlog") from e
+
+        from structlog import configure, get_logger
+
+        # we now configure structlog
+        configure(
+            **{
+                k: v
+                for k, v in asdict(self).items()
+                if k
+                not in (
+                    "standard_lib_logging_config",
+                    "log_exceptions",
+                    "traceback_line_limit",
+                    "exception_logging_handler",
+                )
             }
-            for logger in (
-                "sqlalchemy",
-                self.engine_config.logging_name or "sqlalchemy.engine",
-                self.engine_config.pool_logging_name or "sqlalchemy.pool",
-            ):
-                if logger not in logging_config.loggers:
-                    logging_config.loggers[logger] = logger_settings
+        )
+        return get_logger
```

### Comparing `litestar-2.0.0a4/litestar/controller.py` & `litestar-2.0.0a5/litestar/controller.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/data_extractors.py` & `litestar-2.0.0a5/litestar/data_extractors.py`

 * *Files 0% similar despite different names*

```diff
@@ -250,15 +250,15 @@
             request: A :class:`Request <litestar.connection.Request>` instance.
 
         Returns:
             A tuple containing the request's parsed 'Content-Type' header.
         """
         return request.content_type
 
-    async def extract_body(self, request: "Request[Any, Any, Any]") -> Any:
+    async def extract_body(self, request: Request[Any, Any, Any]) -> Any:
         """Extract the body from an ``ASGIConnection``
 
         Args:
             request: A :class:`Request <litestar.connection.Request>` instance.
 
         Returns:
             Either the parsed request body or the raw byte-string.
```

### Comparing `litestar-2.0.0a4/litestar/datastructures/__init__.py` & `litestar-2.0.0a5/litestar/datastructures/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/datastructures/cookie.py` & `litestar-2.0.0a5/litestar/datastructures/cookie.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/datastructures/headers.py` & `litestar-2.0.0a5/litestar/datastructures/headers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/datastructures/multi_dicts.py` & `litestar-2.0.0a5/litestar/datastructures/multi_dicts.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/datastructures/response_header.py` & `litestar-2.0.0a5/litestar/datastructures/response_header.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/datastructures/state.py` & `litestar-2.0.0a5/litestar/datastructures/state.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/datastructures/upload_file.py` & `litestar-2.0.0a5/litestar/datastructures/upload_file.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/datastructures/url.py` & `litestar-2.0.0a5/litestar/datastructures/url.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/di.py` & `litestar-2.0.0a5/litestar/di.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/enums.py` & `litestar-2.0.0a5/litestar/enums.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/events/emitter.py` & `litestar-2.0.0a5/litestar/events/emitter.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/events/listener.py` & `litestar-2.0.0a5/litestar/events/listener.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/exceptions/__init__.py` & `litestar-2.0.0a5/litestar/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/exceptions/base_exceptions.py` & `litestar-2.0.0a5/litestar/exceptions/base_exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             return f"{self.__class__.__name__} - {self.detail}"
         return self.__class__.__name__
 
     def __str__(self) -> str:
         return " ".join(self.args).strip()
 
 
-class MissingDependencyException(LitestarException):
+class MissingDependencyException(LitestarException, ImportError):
     """Missing optional dependency.
 
     This exception is raised only when a module depends on a dependency that has not been installed.
     """
 
     def __init__(self, package: str, install_package: str | None = None) -> None:
         super().__init__(
```

### Comparing `litestar-2.0.0a4/litestar/exceptions/http_exceptions.py` & `litestar-2.0.0a5/litestar/exceptions/http_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/exceptions/websocket_exceptions.py` & `litestar-2.0.0a5/litestar/exceptions/websocket_exceptions.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/file_system.py` & `litestar-2.0.0a5/litestar/file_system.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,28 +21,28 @@
     from litestar.types import PathType
     from litestar.types.file_types import FileInfo
 
 
 class BaseLocalFileSystem(FileSystemProtocol):
     """Base class for a local file system."""
 
-    async def info(self, path: "PathType", **kwargs: Any) -> "FileInfo":
+    async def info(self, path: PathType, **kwargs: Any) -> FileInfo:
         """Retrieve information about a given file path.
 
         Args:
             path: A file path.
             **kwargs: Any additional kwargs.
 
         Returns:
             A dictionary of file info.
         """
         result = await Path(path).stat()
         return await FileSystemAdapter.parse_stat_result(path=path, result=result)
 
-    async def open(self, file: "PathType", mode: str, buffering: int = -1) -> AsyncFile[AnyStr]:
+    async def open(self, file: PathType, mode: str, buffering: int = -1) -> AsyncFile[AnyStr]:
         """Return a file-like object from the filesystem.
 
         Notes:
             - The return value must be a context-manager
 
         Args:
             file: Path to the target file.
@@ -59,15 +59,15 @@
         """Initialize an adapter from a given ``file_system``
 
         Args:
             file_system: A filesystem class adhering to the :class:`FileSystemProtocol <litestar.types.FileSystemProtocol>`
         """
         self.file_system = file_system
 
-    async def info(self, path: "PathType") -> "FileInfo":
+    async def info(self, path: PathType) -> FileInfo:
         """Proxies the call to the underlying FS Spec's ``info`` method, ensuring it's done in an async fashion and with
         strong typing.
 
         Args:
             path: A file path to load the info for.
 
         Returns:
@@ -85,16 +85,16 @@
         except PermissionError as e:
             raise NotAuthorizedException(f"failed to read {path} due to missing permissions") from e
         except OSError as e:  # pragma: no cover
             raise InternalServerException from e
 
     async def open(
         self,
-        file: "PathType",
-        mode: "OpenBinaryMode" = "rb",
+        file: PathType,
+        mode: OpenBinaryMode = "rb",
         buffering: int = -1,
     ) -> AsyncFile[bytes]:
         """Return a file-like object from the filesystem.
 
         Notes:
             - The return value must function correctly in a context ``with`` block.
 
@@ -116,15 +116,15 @@
             return AsyncFile(await run_sync(self.file_system.open, file, mode, buffering))  # type: ignore
         except PermissionError as e:
             raise NotAuthorizedException(f"failed to open {file} due to missing permissions") from e
         except OSError as e:
             raise InternalServerException from e
 
     @staticmethod
-    async def parse_stat_result(path: "PathType", result: "stat_result") -> "FileInfo":
+    async def parse_stat_result(path: PathType, result: stat_result) -> FileInfo:
         """Convert a ``stat_result`` instance into a ``FileInfo``.
 
         Args:
             path: The file path for which the :func:`stat_result <os.stat_result>` is provided.
             result: The :func:`stat_result <os.stat_result>` instance.
 
         Returns:
```

### Comparing `litestar-2.0.0a4/litestar/handlers/__init__.py` & `litestar-2.0.0a5/litestar/handlers/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from .asgi_handlers import ASGIRouteHandler, asgi
 from .base import BaseRouteHandler
 from .http_handlers import HTTPRouteHandler, delete, get, head, patch, post, put, route
 from .websocket_handlers import WebsocketListener, WebsocketRouteHandler, websocket, websocket_listener
 
 __all__ = (
-    "asgi",
     "ASGIRouteHandler",
     "BaseRouteHandler",
+    "HTTPRouteHandler",
+    "WebsocketListener",
+    "WebsocketRouteHandler",
+    "asgi",
     "delete",
     "get",
     "head",
-    "HTTPRouteHandler",
     "patch",
     "post",
     "put",
     "route",
     "websocket",
     "websocket_listener",
-    "WebsocketListener",
-    "WebsocketRouteHandler",
 )
```

### Comparing `litestar-2.0.0a4/litestar/handlers/asgi_handlers.py` & `litestar-2.0.0a5/litestar/handlers/asgi_handlers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/handlers/base.py` & `litestar-2.0.0a5/litestar/handlers/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 from __future__ import annotations
 
 from copy import copy
+from functools import partial
 from typing import TYPE_CHECKING, Any, Generic, Mapping, Sequence, TypeVar, cast
 
+from litestar._signature import create_signature_model
 from litestar._signature.field import SignatureField
-from litestar.dto.interface import DTOInterface
+from litestar.dto.interface import HandlerContext
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.types import Dependencies, Empty, ExceptionHandlersMap, Guard, Middleware, TypeEncodersMap
-from litestar.utils import AsyncCallable, Ref, get_name, normalize_path
+from litestar.utils import AsyncCallable, Ref, async_partial, get_name, is_async_callable, normalize_path
 from litestar.utils.helpers import unwrap_partial
-from litestar.utils.signature import ParsedSignature
+from litestar.utils.signature import ParsedSignature, infer_request_encoding_from_parameter
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
+    from litestar import Litestar
     from litestar._signature.models import SignatureModel
     from litestar.connection import ASGIConnection
     from litestar.controller import Controller
     from litestar.di import Provide
+    from litestar.dto.interface import DTOInterface
     from litestar.params import ParameterKwarg
+    from litestar.plugins import SerializationPluginProtocol
     from litestar.router import Router
-    from litestar.types import AsyncAnyCallable, ExceptionHandler
+    from litestar.types import AnyCallable, AsyncAnyCallable, ExceptionHandler
     from litestar.types.composite_types import MaybePartial
     from litestar.types.empty import EmptyType
 
 __all__ = ("BaseRouteHandler",)
 
 T = TypeVar("T", bound="BaseRouteHandler")
 
@@ -333,57 +338,130 @@
                 for layer in self.ownership_layers
                 if (layer_dto_type := layer.return_dto) is not Empty
             ]
             self._resolved_return_dto = return_dtos[-1] if return_dtos else self.resolve_dto()
 
         return cast("type[DTOInterface] | None", self._resolved_return_dto)
 
+    def _set_dto(self, dto: type[DTOInterface]) -> None:
+        """Set the dto for the handler.
+
+        Args:
+            dto: The :class:`DTO type <.dto.interface.DTOInterface>` to set.
+        """
+        self._resolved_dto = dto
+
+    def _set_return_dto(self, dto: type[DTOInterface]) -> None:
+        """Set the return_dto for the handler.
+
+        Args:
+            dto: The :class:`DTO type <.dto.interface.DTOInterface>` to set.
+        """
+        self._resolved_return_dto = dto
+
     def _init_handler_dtos(self) -> None:
         """Initialize the data and return DTOs for the handler."""
-        data_parameter = self.parsed_fn_signature.parameters.get("data")
-        if data_parameter:
-            parameter_type = data_parameter.parsed_type
-            dto = parameter_type.annotation if parameter_type.is_subclass_of(DTOInterface) else self.resolve_dto()
-            if dto:
-                dto.on_registration(parameter_type.annotation, self)
-
-        return_type = self.parsed_fn_signature.return_type
-        if return_type.annotation is not Empty:
-            return_dto = (
-                return_type.annotation if return_type.is_subclass_of(DTOInterface) else self.resolve_return_dto()
+        if (dto := self.resolve_dto()) and (data_parameter := self.parsed_fn_signature.parameters.get("data")):
+            dto.on_registration(
+                HandlerContext(
+                    "data", str(self), data_parameter.parsed_type, infer_request_encoding_from_parameter(data_parameter)
+                )
             )
-            if return_dto:
-                return_dto.on_registration(return_type.annotation, self)
 
-    async def authorize_connection(self, connection: "ASGIConnection") -> None:
+        if return_dto := self.resolve_return_dto():
+            return_dto.on_registration(HandlerContext("return", str(self), self.parsed_fn_signature.return_type))
+
+    async def authorize_connection(self, connection: ASGIConnection) -> None:
         """Ensure the connection is authorized by running all the route guards in scope."""
         for guard in self.resolve_guards():
             await guard(connection, copy(self))  # type: ignore
 
     @staticmethod
     def _validate_dependency_is_unique(dependencies: dict[str, Provide], key: str, provider: Provide) -> None:
         """Validate that a given provider has not been already defined under a different key."""
         for dependency_key, value in dependencies.items():
             if provider == value:
                 raise ImproperlyConfiguredException(
                     f"Provider for key {key} is already defined under the different key {dependency_key}. "
                     f"If you wish to override a provider, it must have the same key."
                 )
 
-    def on_registration(self) -> None:
+    def on_registration(self, app: Litestar) -> None:
         """Called once per handler when the app object is instantiated."""
         self._validate_handler_function()
+        self._handle_serialization_plugins(app.serialization_plugins)
+        self._init_handler_dtos()
+        self._set_runtime_callables()
+        self._create_signature_model(app)
+        self._create_provider_signature_models(app)
         self.resolve_guards()
         self.resolve_middleware()
         self.resolve_opts()
-        self._init_handler_dtos()
 
     def _validate_handler_function(self) -> None:
         """Validate the route handler function once set by inspecting its return annotations."""
 
+    def _set_runtime_callables(self) -> None:
+        """Optimize the ``route_handler.fn`` and any ``provider.dependency`` callables for runtime by doing the following:
+
+        1. ensure that the ``self`` argument is preserved by binding it using partial.
+        2. ensure sync functions are wrapped in AsyncCallable for sync_to_thread handlers.
+        """
+        from litestar.controller import Controller
+
+        if isinstance(self.owner, Controller) and not hasattr(self.fn.value, "func"):
+            self.fn.value = partial(self.fn.value, self.owner)
+
+        for provider in self.resolve_dependencies().values():
+            if not is_async_callable(provider.dependency.value):
+                provider.has_sync_callable = False
+                if provider.sync_to_thread:
+                    provider.dependency.value = async_partial(provider.dependency.value)
+                else:
+                    provider.has_sync_callable = True
+
+    def _create_signature_model(self, app: Litestar) -> None:
+        """Create signature model for handler function."""
+        if not self.signature_model:
+            self.signature_model = create_signature_model(
+                dependency_name_set=self.dependency_name_set,
+                fn=cast("AnyCallable", self.fn.value),
+                preferred_validation_backend=app.preferred_validation_backend,
+                parsed_signature=self.parsed_fn_signature,
+            )
+
+    def _create_provider_signature_models(self, app: Litestar) -> None:
+        """Create signature models for dependency providers."""
+        for provider in self.resolve_dependencies().values():
+            if not getattr(provider, "signature_model", None):
+                provider.signature_model = create_signature_model(
+                    dependency_name_set=self.dependency_name_set,
+                    fn=provider.dependency.value,
+                    preferred_validation_backend=app.preferred_validation_backend,
+                    parsed_signature=ParsedSignature.from_fn(
+                        unwrap_partial(provider.dependency.value), self.resolve_signature_namespace()
+                    ),
+                )
+
+    def _handle_serialization_plugins(self, plugins: list[SerializationPluginProtocol]) -> None:
+        """Handle the serialization plugins for the handler."""
+        # must do the return dto first, otherwise it will resolve to the same as the data dto
+        if self.resolve_return_dto() is None:
+            return_type = self.parsed_fn_signature.return_type
+            for plugin in plugins:
+                if plugin.supports_type(return_type):
+                    self._set_return_dto(plugin.create_dto_for_type(return_type))
+                    break
+
+        if (data_param := self.parsed_fn_signature.parameters.get("data")) and self.resolve_dto() is None:
+            for plugin in plugins:
+                if plugin.supports_type(data_param.parsed_type):
+                    self._set_dto(plugin.create_dto_for_type(data_param.parsed_type))
+                    break
+
     def __str__(self) -> str:
         """Return a unique identifier for the route handler.
 
         Returns:
             A string
         """
         target: type[AsyncAnyCallable] | AsyncAnyCallable
```

### Comparing `litestar-2.0.0a4/litestar/handlers/http_handlers/_utils.py` & `litestar-2.0.0a5/litestar/handlers/http_handlers/_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 from __future__ import annotations
 
 from functools import lru_cache
 from inspect import isawaitable
 from typing import TYPE_CHECKING, Any, Sequence, cast
 
-from litestar.dto.interface import DTOInterface
+from litestar.dto.interface import ConnectionContext
 from litestar.enums import HttpMethod
 from litestar.exceptions import ValidationException
-from litestar.plugins import get_plugin_for_value
 from litestar.status_codes import HTTP_200_OK, HTTP_201_CREATED, HTTP_204_NO_CONTENT
-from litestar.utils import is_async_callable
 
 if TYPE_CHECKING:
     from litestar.app import Litestar
     from litestar.background_tasks import BackgroundTask, BackgroundTasks
     from litestar.connection import Request
     from litestar.datastructures import Cookie, ResponseHeader
-    from litestar.plugins import SerializationPluginProtocol
+    from litestar.dto.interface import DTOInterface
     from litestar.response import Response
     from litestar.response_containers import ResponseContainer
     from litestar.types import (
         AfterRequestHookHandler,
         ASGIApp,
         AsyncAnyCallable,
         Method,
@@ -33,15 +31,14 @@
     "create_generic_asgi_response_handler",
     "create_response_container_handler",
     "create_response_handler",
     "filter_cookies",
     "get_default_status_code",
     "normalize_headers",
     "normalize_http_method",
-    "normalize_response_data",
 )
 
 
 def create_data_handler(
     after_request: AfterRequestHookHandler | None,
     background: BackgroundTask | BackgroundTasks | None,
     cookies: frozenset[Cookie],
@@ -69,15 +66,15 @@
     """
     normalized_headers = [
         (name.lower().encode("latin-1"), value.encode("latin-1")) for name, value in normalize_headers(headers).items()
     ]
     cookie_headers = [cookie.to_encoded_header() for cookie in cookies if not cookie.documentation_only]
     raw_headers = [*normalized_headers, *cookie_headers]
 
-    async def create_response(data: Any) -> "ASGIApp":
+    async def create_response(data: Any) -> ASGIApp:
         response = response_class(
             background=background,
             content=data,
             media_type=media_type,
             status_code=status_code,
             type_encoders=type_encoders,
         )
@@ -86,28 +83,24 @@
         if after_request:
             return await after_request(response)  # type: ignore
 
         return response
 
     async def handler(
         data: Any,
-        plugins: list["SerializationPluginProtocol"],
         return_dto: type[DTOInterface] | None,
         request: Request[Any, Any, Any],
         **kwargs: Any,
-    ) -> "ASGIApp":
+    ) -> ASGIApp:
         if isawaitable(data):
             data = await data
 
-        if isinstance(data, DTOInterface):
-            data = data.to_encodable_type(request=request)
-        elif return_dto:
-            data = return_dto.from_data(data=data).to_encodable_type(request=request)
-        elif plugins:
-            data = await normalize_response_data(data=data, plugins=plugins)
+        if return_dto:
+            ctx = ConnectionContext.from_connection(request)
+            data = return_dto(ctx).data_to_encodable_type(data)
 
         return await create_response(data=data)
 
     return handler
 
 
 def filter_cookies(local_cookies: frozenset[Cookie], layered_cookies: frozenset[Cookie]) -> list[Cookie]:
@@ -133,15 +126,15 @@
         after_request: An after request handler.
         cookies: A set of pre-defined cookies.
 
     Returns:
         A handler function.
     """
 
-    async def handler(data: "ASGIApp", **kwargs: Any) -> "ASGIApp":
+    async def handler(data: ASGIApp, **kwargs: Any) -> ASGIApp:
         if hasattr(data, "set_cookie"):
             for cookie in cookies:
                 data.set_cookie(**cookie.dict)
         return await after_request(data) if after_request else data  # type: ignore
 
     return handler
 
@@ -160,38 +153,14 @@
         header.name: cast("str", header.value)  # we know value to be a string at this point because we validate it
         # that it's not None when initializing a header with documentation_only=True
         for header in headers
         if not header.documentation_only
     }
 
 
-async def normalize_response_data(data: Any, plugins: list["SerializationPluginProtocol"]) -> Any:
-    """Normalize the response's data by awaiting any async values and resolving plugins.
-
-    Args:
-        data: An arbitrary value
-        plugins: A list of :class:`plugins <litestar.plugins.base.SerializationPluginProtocol>`
-    Returns:
-        Value for the response body
-    """
-
-    plugin = get_plugin_for_value(value=data, plugins=plugins)
-    if not plugin:
-        return data
-
-    if is_async_callable(plugin.to_dict):
-        if isinstance(data, (list, tuple)):
-            return [await plugin.to_dict(datum) for datum in data]
-        return await plugin.to_dict(data)
-
-    if isinstance(data, (list, tuple)):
-        return [plugin.to_dict(datum) for datum in data]
-    return plugin.to_dict(data)
-
-
 def create_response_container_handler(
     after_request: AfterRequestHookHandler | None,
     cookies: frozenset[Cookie],
     headers: frozenset[ResponseHeader],
     media_type: str,
     status_code: int,
 ) -> AsyncAnyCallable:
@@ -205,15 +174,15 @@
         status_code: The response status code.
 
     Returns:
         A handler function.
     """
     normalized_headers = normalize_headers(headers)
 
-    async def handler(data: ResponseContainer, app: Litestar, request: Request, **kwargs: Any) -> "ASGIApp":
+    async def handler(data: ResponseContainer, app: Litestar, request: Request, **kwargs: Any) -> ASGIApp:
         response = data.to_response(
             app=app,
             headers={**normalized_headers, **data.headers},
             status_code=status_code,
             media_type=data.media_type or media_type,
             request=request,
         )
@@ -233,15 +202,15 @@
         after_request: An after request handler.
         cookies: A set of pre-defined cookies.
 
     Returns:
         A handler function.
     """
 
-    async def handler(data: Response, **kwargs: Any) -> "ASGIApp":
+    async def handler(data: Response, **kwargs: Any) -> ASGIApp:
         data.cookies = filter_cookies(frozenset(data.cookies), cookies)
         return await after_request(data) if after_request else data  # type: ignore
 
     return handler
 
 
 def normalize_http_method(http_methods: HttpMethod | Method | Sequence[HttpMethod | Method]) -> set[Method]:
```

### Comparing `litestar-2.0.0a4/litestar/handlers/http_handlers/base.py` & `litestar-2.0.0a5/litestar/handlers/http_handlers/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,30 +40,29 @@
     Middleware,
     ResponseCookies,
     ResponseHeaders,
     ResponseType,
     TypeEncodersMap,
 )
 from litestar.types.builtin_types import NoneType
-from litestar.utils import AsyncCallable, is_async_callable
+from litestar.utils import AsyncCallable, async_partial, is_async_callable
 
 if TYPE_CHECKING:
     from typing import Any, Awaitable, Callable, Sequence
 
     from litestar.app import Litestar
     from litestar.background_tasks import BackgroundTask, BackgroundTasks
     from litestar.config.response_cache import CACHE_FOREVER
     from litestar.connection import Request
     from litestar.datastructures import CacheControlHeader, ETag
     from litestar.datastructures.headers import Header
     from litestar.di import Provide
     from litestar.dto.interface import DTOInterface
     from litestar.openapi.datastructures import ResponseSpec
     from litestar.openapi.spec import SecurityRequirement
-    from litestar.plugins import SerializationPluginProtocol
     from litestar.types import MaybePartial  # noqa: F401
 
 
 __all__ = ("HTTPRouteHandler", "route")
 
 
 class ResponseHandlerMap(TypedDict):
@@ -446,34 +445,31 @@
         return cast(
             "Callable[[Any], Awaitable[ASGIApp]]",
             self._response_handler_mapping["response_type_handler"]
             if is_response_type_data
             else self._response_handler_mapping["default_handler"],
         )
 
-    async def to_response(
-        self, app: Litestar, data: Any, plugins: list["SerializationPluginProtocol"], request: Request
-    ) -> ASGIApp:
+    async def to_response(self, app: Litestar, data: Any, request: Request) -> ASGIApp:
         """Return a :class:`Response <.response.Response>` from the handler by resolving and calling it.
 
         Args:
             app: The :class:`Litestar <litestar.app.Litestar>` app instance
             data: Either an instance of a :class:`ResponseContainer <.response_containers.ResponseContainer>`,
                 a Response instance or an arbitrary value.
-            plugins: An optional mapping of plugins
             request: A :class:`Request <.connection.Request>` instance
 
         Returns:
             A Response instance
         """
         response_handler = self.get_response_handler(is_response_type_data=isinstance(data, Response))
-        return await response_handler(app=app, data=data, plugins=plugins, request=request, return_dto=self.resolve_return_dto())  # type: ignore
+        return await response_handler(app=app, data=data, request=request, return_dto=self.resolve_return_dto())  # type: ignore
 
-    def on_registration(self) -> None:
-        super().on_registration()
+    def on_registration(self, app: Litestar) -> None:
+        super().on_registration(app)
         if before_request := self.resolve_before_request():
             before_request.set_parsed_signature(self.resolve_signature_namespace())
         self.resolve_after_response()
 
     def _validate_handler_function(self) -> None:
         """Validate the route handler function once it is set by inspecting its return annotations."""
         super()._validate_handler_function()
@@ -504,9 +500,19 @@
 
         if "socket" in self.parsed_fn_signature.parameters:
             raise ImproperlyConfiguredException("The 'socket' kwarg is not supported with http handlers")
 
         if "data" in self.parsed_fn_signature.parameters and "GET" in self.http_methods:
             raise ImproperlyConfiguredException("'data' kwarg is unsupported for 'GET' request handlers")
 
+    def _set_runtime_callables(self) -> None:
+        """Set the runtime callables for the route handler."""
+        super()._set_runtime_callables()
+        self.has_sync_callable = False
+        if not is_async_callable(self.fn.value):
+            if self.sync_to_thread:
+                self.fn.value = async_partial(self.fn.value)
+            else:
+                self.has_sync_callable = True
+
 
 route = HTTPRouteHandler
```

### Comparing `litestar-2.0.0a4/litestar/handlers/http_handlers/decorators.py` & `litestar-2.0.0a5/litestar/handlers/http_handlers/decorators.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/handlers/websocket_handlers.py` & `litestar-2.0.0a5/litestar/router.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,352 +1,313 @@
 from __future__ import annotations
 
-import inspect
-from abc import ABC, abstractmethod
-from functools import partial
-from typing import TYPE_CHECKING, Callable, Coroutine
-
-from msgspec.json import Encoder as JsonEncoder
-
-from litestar.exceptions import ImproperlyConfiguredException, WebSocketDisconnect
-from litestar.handlers.base import BaseRouteHandler
-from litestar.serialization import decode_json, default_serializer
-from litestar.types.builtin_types import NoneType
+from collections import defaultdict
+from copy import copy
+from typing import TYPE_CHECKING, Any, DefaultDict, Mapping, Sequence, cast
+
+from litestar._layers.utils import narrow_response_cookies, narrow_response_headers
+from litestar.controller import Controller
+from litestar.exceptions import ImproperlyConfiguredException
+from litestar.handlers.asgi_handlers import ASGIRouteHandler
+from litestar.handlers.http_handlers import HTTPRouteHandler
+from litestar.handlers.websocket_handlers import WebsocketListener, WebsocketRouteHandler
+from litestar.routes import ASGIRoute, HTTPRoute, WebSocketRoute
 from litestar.types.empty import Empty
-from litestar.utils import AsyncCallable, is_async_callable
-from litestar.utils.signature import ParsedSignature
+from litestar.utils import find_index, is_class_and_subclass, join_paths, normalize_path, unique
+from litestar.utils.sync import AsyncCallable
 
-__all__ = ("WebsocketRouteHandler", "websocket", "websocket_listener", "WebsocketListener")
+__all__ = ("Router",)
 
-if TYPE_CHECKING:
-    from typing import Any, Mapping
 
-    from litestar.connection import WebSocket
+if TYPE_CHECKING:
+    from litestar.datastructures import CacheControlHeader, ETag
+    from litestar.di import Provide
     from litestar.dto.interface import DTOInterface
+    from litestar.openapi.spec import SecurityRequirement
+    from litestar.routes import BaseRoute
     from litestar.types import (
-        AnyCallable,
-        Dependencies,
-        EmptyType,
-        ExceptionHandler,
+        AfterRequestHookHandler,
+        AfterResponseHookHandler,
+        BeforeRequestHookHandler,
+        ControllerRouterHandler,
+        ExceptionHandlersMap,
         Guard,
-        MaybePartial,  # noqa: F401
         Middleware,
-        SyncOrAsyncUnion,
+        ParametersMap,
+        ResponseCookies,
+        ResponseType,
+        RouteHandlerMapItem,
+        RouteHandlerType,
         TypeEncodersMap,
     )
-    from litestar.types.asgi_types import WebSocketMode
+    from litestar.types.composite_types import ResponseHeaders
+    from litestar.types.empty import EmptyType
 
 
-class WebsocketRouteHandler(BaseRouteHandler["WebsocketRouteHandler"]):
-    """Websocket route handler decorator.
+class Router:
+    """The Litestar Router class.
 
-    Use this decorator to decorate websocket handler functions.
+    A Router instance is used to group controller, routers and route handler functions under a shared path fragment
     """
 
-    __slots__ = ()
+    __slots__ = (
+        "after_request",
+        "after_response",
+        "before_request",
+        "cache_control",
+        "dependencies",
+        "dto",
+        "etag",
+        "exception_handlers",
+        "guards",
+        "middleware",
+        "opt",
+        "owner",
+        "parameters",
+        "path",
+        "registered_route_handler_ids",
+        "response_class",
+        "response_cookies",
+        "response_headers",
+        "return_dto",
+        "routes",
+        "security",
+        "signature_namespace",
+        "tags",
+        "type_encoders",
+    )
 
     def __init__(
         self,
-        path: str | None | list[str] | None = None,
+        path: str,
         *,
-        dependencies: Dependencies | None = None,
+        after_request: AfterRequestHookHandler | None = None,
+        after_response: AfterResponseHookHandler | None = None,
+        before_request: BeforeRequestHookHandler | None = None,
+        cache_control: CacheControlHeader | None = None,
+        dependencies: Mapping[str, Provide] | None = None,
         dto: type[DTOInterface] | None | EmptyType = Empty,
-        exception_handlers: dict[int | type[Exception], ExceptionHandler] | None = None,
-        guards: list[Guard] | None = None,
-        middleware: list[Middleware] | None = None,
-        name: str | None = None,
-        opt: dict[str, Any] | None = None,
+        etag: ETag | None = None,
+        exception_handlers: ExceptionHandlersMap | None = None,
+        guards: Sequence[Guard] | None = None,
+        middleware: Sequence[Middleware] | None = None,
+        opt: Mapping[str, Any] | None = None,
+        parameters: ParametersMap | None = None,
+        response_class: ResponseType | None = None,
+        response_cookies: ResponseCookies | None = None,
+        response_headers: ResponseHeaders | None = None,
         return_dto: type[DTOInterface] | None | EmptyType = Empty,
+        route_handlers: Sequence[ControllerRouterHandler],
+        security: Sequence[SecurityRequirement] | None = None,
         signature_namespace: Mapping[str, Any] | None = None,
-        **kwargs: Any,
+        tags: Sequence[str] | None = None,
+        type_encoders: TypeEncodersMap | None = None,
     ) -> None:
-        """Initialize ``WebsocketRouteHandler``
+        """Initialize a ``Router``.
 
         Args:
-            path: A path fragment for the route handler function or a sequence of path fragments. If not given defaults
-                to ``/``
-            dependencies: A string keyed mapping of dependency :class:`Provider <.di.Provide>` instances.
+            after_request: A sync or async function executed before a :class:`Request <.connection.Request>` is passed
+                to any route handler. If this function returns a value, the request will not reach the route handler,
+                and instead this value will be used.
+            after_response: A sync or async function called after the response has been awaited. It receives the
+                :class:`Request <.connection.Request>` object and should not return any values.
+            before_request: A sync or async function called immediately before calling the route handler. Receives
+                the :class:`litestar.connection.Request` instance and any non-``None`` return value is used for the
+                response, bypassing the route handler.
+            cache_control: A ``cache-control`` header of type
+                :class:`CacheControlHeader <.datastructures.CacheControlHeader>` to add to route handlers of
+                this router. Can be overridden by route handlers.
+            dependencies: A string keyed mapping of dependency :class:`Provide <.di.Provide>` instances.
             dto: :class:`DTOInterface <.dto.interface.DTOInterface>` to use for (de)serializing and
                 validation of request data.
+            etag: An ``etag`` header of type :class:`ETag <.datastructures.ETag>` to add to route handlers of this app.
             exception_handlers: A mapping of status codes and/or exception types to handler functions.
-            guards: A sequence of :class:`Guard <.types.Guard>` callables.
-            middleware: A sequence of :class:`Middleware <.types.Middleware>`.
-            name: A string identifying the route handler.
-            opt: A string keyed mapping of arbitrary values that can be accessed in :class:`Guards <.types.Guard>` or
+            guards: A sequence of :data:`Guard <.types.Guard>` callables.
+            middleware: A sequence of :data:`Middleware <.types.Middleware>`.
+            opt: A string keyed mapping of arbitrary values that can be accessed in :data:`Guards <.types.Guard>` or
                 wherever you have access to :class:`Request <.connection.Request>` or
-                :class:`ASGI Scope <.types.Scope>`.
+                :data:`ASGI Scope <.types.Scope>`.
+            parameters: A mapping of :func:`Parameter <.params.Parameter>` definitions available to all application
+                paths.
+            path: A path fragment that is prefixed to all route handlers, controllers and other routers associated
+                with the router instance.
+            response_class: A custom subclass of :class:`Response <.response.Response>` to be used as the default for
+                all route handlers, controllers and other routers associated with the router instance.
+            response_cookies: A sequence of :class:`Cookie <.datastructures.Cookie>` instances.
+            response_headers: A string keyed mapping of :class:`ResponseHeader <.datastructures.ResponseHeader>`
+                instances.
             return_dto: :class:`DTOInterface <.dto.interface.DTOInterface>` to use for serializing
                 outbound response data.
+            route_handlers: A required sequence of route handlers, which can include instances of
+                :class:`Router <.router.Router>`, subclasses of :class:`Controller <.controller.Controller>` or any
+                function decorated by the route handler decorators.
+            security: A sequence of dicts that will be added to the schema of all route handlers in the application.
+                See :data:`SecurityRequirement <.openapi.spec.SecurityRequirement>`
+                for details.
             signature_namespace: A mapping of names to types for use in forward reference resolution during signature modelling.
+            tags: A sequence of string tags that will be appended to the schema of all route handlers under the
+                application.
             type_encoders: A mapping of types to callables that transform them into types supported for serialization.
-            **kwargs: Any additional kwarg - will be set in the opt dictionary.
         """
 
-        super().__init__(
-            path=path,
-            dto=dto,
-            dependencies=dependencies,
-            exception_handlers=exception_handlers,
-            guards=guards,
-            middleware=middleware,
-            name=name,
-            opt=opt,
-            return_dto=return_dto,
-            signature_namespace=signature_namespace,
-            **kwargs,
-        )
+        self.after_request = AsyncCallable(after_request) if after_request else None  # type: ignore[arg-type]
+        self.after_response = AsyncCallable(after_response) if after_response else None
+        self.before_request = AsyncCallable(before_request) if before_request else None
+        self.cache_control = cache_control
+        self.dto = dto
+        self.etag = etag
+        self.dependencies = dict(dependencies or {})
+        self.exception_handlers = dict(exception_handlers or {})
+        self.guards = list(guards or [])
+        self.middleware = list(middleware or [])
+        self.opt = dict(opt or {})
+        self.owner: Router | None = None
+        self.parameters = dict(parameters or {})
+        self.path = normalize_path(path)
+        self.response_class = response_class
+        self.response_cookies = narrow_response_cookies(response_cookies)
+        self.response_headers = narrow_response_headers(response_headers)
+        self.return_dto = return_dto
+        self.routes: list[HTTPRoute | ASGIRoute | WebSocketRoute] = []
+        self.security = list(security or [])
+        self.signature_namespace = signature_namespace or {}
+        self.tags = list(tags or [])
+        self.registered_route_handler_ids: set[int] = set()
+        self.type_encoders = dict(type_encoders) if type_encoders is not None else None
 
-    def _validate_handler_function(self) -> None:
-        """Validate the route handler function once it's set by inspecting its return annotations."""
-        super()._validate_handler_function()
-
-        if not self.parsed_fn_signature.return_type.is_subclass_of(NoneType):
-            raise ImproperlyConfiguredException("Websocket handler functions should return 'None'")
-        if "socket" not in self.parsed_fn_signature.parameters:
-            raise ImproperlyConfiguredException("Websocket handlers must set a 'socket' kwarg")
-        for param in ("request", "body", "data"):
-            if param in self.parsed_fn_signature.parameters:
-                raise ImproperlyConfiguredException(f"The {param} kwarg is not supported with websocket handlers")
-        if not is_async_callable(self.fn.value):
-            raise ImproperlyConfiguredException("Functions decorated with 'websocket' must be async functions")
-
-
-websocket = WebsocketRouteHandler
-
-
-class websocket_listener(WebsocketRouteHandler):
-    """A websocket listener that automatically accepts a connection, handles disconnects,
-    invokes a callback function every time new data is received and sends any data
-    returned
-    """
+        for route_handler in route_handlers or []:
+            self.register(value=route_handler)
 
-    def __init__(
-        self,
-        path: str | None | list[str] | None = None,
-        *,
-        dependencies: Dependencies | None = None,
-        exception_handlers: dict[int | type[Exception], ExceptionHandler] | None = None,
-        guards: list[Guard] | None = None,
-        middleware: list[Middleware] | None = None,
-        receive_mode: WebSocketMode = "text",
-        send_mode: WebSocketMode = "text",
-        name: str | None = None,
-        on_accept: Callable[[WebSocket], SyncOrAsyncUnion[None]] | None = None,
-        on_disconnect: Callable[[WebSocket], SyncOrAsyncUnion[None]] | None = None,
-        opt: dict[str, Any] | None = None,
-        signature_namespace: Mapping[str, Any] | None = None,
-        type_encoders: TypeEncodersMap | None = None,
-        **kwargs: Any,
-    ) -> None:
-        """Initialize ``WebsocketRouteHandler``
+    def register(self, value: ControllerRouterHandler) -> list[BaseRoute]:
+        """Register a Controller, Route instance or RouteHandler on the router.
 
         Args:
-            path: A path fragment for the route handler function or a sequence of path fragments. If not given defaults
-                to ``/``
-            dependencies: A string keyed mapping of dependency :class:`Provider <.di.Provide>` instances.
-            exception_handlers: A mapping of status codes and/or exception types to handler functions.
-            guards: A sequence of :class:`Guard <.types.Guard>` callables.
-            middleware: A sequence of :class:`Middleware <.types.Middleware>`.
-            receive_mode: Websocket mode to receive data in, either `text` or `binary`.
-            send_mode: Websocket mode to receive data in, either `text` or `binary`.
-            name: A string identifying the route handler.
-            on_accept: Callback invoked after a connection has been accepted, receiving the
-                :class:`WebSocket <.connection.WebSocket>` instance as its only argument
-            on_disconnect: Callback invoked after a connection has been closed, receiving the
-                :class:`WebSocket <.connection.WebSocket>` instance as its only argument
-            opt: A string keyed mapping of arbitrary values that can be accessed in :class:`Guards <.types.Guard>` or
-                wherever you have access to :class:`Request <.connection.Request>` or
-                :class:`ASGI Scope <.types.Scope>`.
-            signature_namespace: A mapping of names to types for use in forward reference resolution during signature
-                modelling.
-            type_encoders: A mapping of types to callables that transform them into types supported for serialization.
-            **kwargs: Any additional kwarg - will be set in the opt dictionary.
-        """
-        self._receive_mode = receive_mode
-        self._send_mode = send_mode
-        self._on_accept = AsyncCallable(on_accept) if on_accept else None
-        self._on_disconnect = AsyncCallable(on_disconnect) if on_disconnect else None
-        self.type_encoders = type_encoders
-
-        super().__init__(
-            path=path,
-            dependencies=dependencies,
-            exception_handlers=exception_handlers,
-            guards=guards,
-            middleware=middleware,
-            name=name,
-            opt=opt,
-            signature_namespace=signature_namespace,
-            **kwargs,
-        )
-
-    def _validate_handler_function(self) -> None:
-        """Validate the route handler function once it's set by inspecting its return annotations."""
-        # since none of the validation rules of WebsocketRouteHandler apply here, this is let empty. Validation of the
-        # user supplied method happens at init time of this handler instead in __call__
-
-    def _create_listener_fn(  # noqa: C901
-        self,
-        *,
-        wants_receive_type: Any,
-        can_send_data: bool,
-        should_encode_to_json: bool,
-        pass_socket: bool,
-        callback: AsyncCallable,
-    ) -> Callable[..., Coroutine[None, None, None]]:
-        json_encoder = JsonEncoder(enc_hook=partial(default_serializer, type_encoders=self.resolve_type_encoders()))
-
-        async def handle_receive(socket: WebSocket) -> Any:
-            received_data = await socket.receive_data(mode=self._receive_mode)  # pyright: ignore
-            if wants_receive_type is str:
-                if isinstance(received_data, bytes):
-                    received_data = received_data.decode("utf-8")
-            elif wants_receive_type is bytes:
-                if isinstance(received_data, str):
-                    received_data = received_data.encode("utf-8")
-            else:
-                received_data = decode_json(received_data)
-            return received_data
-
-        async def handle_send(socket: WebSocket, data_to_send: Any) -> None:
-            if should_encode_to_json:
-                data_to_send = json_encoder.encode(data_to_send)
-
-            await socket.send_data(data_to_send, self._send_mode)  # pyright: ignore
-
-        async def listener_fn(socket: WebSocket, **kwargs: Any) -> None:
-            await socket.accept()
-            if self._on_accept:
-                await self._on_accept(socket)
-            if pass_socket:
-                kwargs["socket"] = socket
-            while True:
-                try:
-                    received_data = await handle_receive(socket)
-                    data_to_send = await callback(data=received_data, **kwargs)
-                    if can_send_data:
-                        await handle_send(socket, data_to_send)
-                except WebSocketDisconnect:
-                    if self._on_disconnect:
-                        await self._on_disconnect(socket)
-                    break
-
-        return listener_fn
-
-    @staticmethod
-    def _update_listener_fn_signature(listener_fn: Callable, callback_signature: inspect.Signature) -> None:
-        # make our listener_fn look like the callback, so we get a correct signature model
-
-        new_params = [p for p in callback_signature.parameters.values() if p.name not in {"data"}]
-        if "socket" not in callback_signature.parameters:
-            new_params.append(
-                inspect.Parameter(name="socket", kind=inspect.Parameter.KEYWORD_ONLY, annotation="WebSocket")
-            )
-        new_signature = callback_signature.replace(parameters=new_params)
-        listener_fn.__signature__ = new_signature  # type: ignore[attr-defined]
-        listener_fn.__annotations__ = {p.name: p.annotation for p in new_signature.parameters.values()}
-
-    def __call__(self, listener_callback: AnyCallable) -> websocket_listener:
-        listener_callback_signature = ParsedSignature.from_fn(listener_callback, self.resolve_signature_namespace())
-
-        if "data" not in listener_callback_signature.parameters:
-            raise ImproperlyConfiguredException("Websocket listeners must accept a 'data' parameter")
-        for param in ("request", "body"):
-            if param in listener_callback_signature.parameters:
-                raise ImproperlyConfiguredException(f"The {param} kwarg is not supported with websocket listeners")
-
-        listener_callback = AsyncCallable(listener_callback)
-
-        should_encode_to_json = not (
-            listener_callback_signature.return_type.is_subclass_of((str, bytes))
-            or (
-                listener_callback_signature.return_type.is_optional
-                and listener_callback_signature.return_type.has_inner_subclass_of((str, bytes))
-            )
-        )
-        can_send_data = not listener_callback_signature.return_type.is_subclass_of(NoneType)
-        pass_socket = "socket" in listener_callback_signature.parameters
-
-        listener_fn = self._create_listener_fn(
-            callback=listener_callback,
-            can_send_data=can_send_data,
-            should_encode_to_json=should_encode_to_json,
-            wants_receive_type=listener_callback_signature.parameters["data"].annotation,
-            pass_socket=pass_socket,
-        )
-        self._update_listener_fn_signature(listener_fn, listener_callback_signature.original_signature)
-
-        return super().__call__(listener_fn)
+            value: a subclass or instance of Controller, an instance of :class:`Router` or a function/method that has
+                been decorated by any of the routing decorators, e.g. :class:`get <.handlers.get>`,
+                :class:`post <.handlers.post>`.
 
+        Returns:
+            Collection of handlers added to the router.
+        """
+        validated_value = self._validate_registration_value(value)
 
-class WebsocketListener(ABC):
-    path: str | None | list[str] | None = None
-    """A path fragment for the route handler function or a sequence of path fragments. If not given defaults to ``/``"""
-    dependencies: Dependencies | None = None
-    """A string keyed mapping of dependency :class:`Provider <.di.Provide>` instances."""
-    dto: type[DTOInterface] | None | EmptyType = Empty
-    """:class:`DTOInterface <.dto.interface.DTOInterface>` to use for (de)serializing and validation of request data"""
-    exception_handlers: dict[int | type[Exception], ExceptionHandler] | None = None
-    """A mapping of status codes and/or exception types to handler functions."""
-    guards: list[Guard] | None = None
-    """A sequence of :class:`Guard <.types.Guard>` callables."""
-    middleware: list[Middleware] | None = None
-    """A sequence of :class:`Middleware <.types.Middleware>`."""
-    receive_mode: WebSocketMode = "text"
-    """Websocket mode to receive data in, either `text` or `binary`."""
-    send_mode: WebSocketMode = "text"
-    """Websocket mode to send data in, either `text` or `binary`."""
-    name: str | None = None
-    """A string identifying the route handler."""
-    opt: dict[str, Any] | None = None
-    """
-    A string keyed mapping of arbitrary values that can be accessed in :class:`Guards <.types.Guard>` or wherever you
-    have access to :class:`Request <.connection.Request>` or :class:`ASGI Scope <.types.Scope>`.
-    """
-    return_dto: type[DTOInterface] | None | EmptyType = Empty
-    """:class:`DTOInterface <.dto.interface.DTOInterface>` to use for serializing outbound response data."""
-    signature_namespace: Mapping[str, Any] | None = None
-    """
-    A mapping of names to types for use in forward reference resolution during signature modelling.
-    """
-    type_encoders: TypeEncodersMap | None = None
-    """
-    type_encoders: A mapping of types to callables that transform them into types supported for serialization.
-    """
+        routes: list[BaseRoute] = []
 
-    def __init__(self) -> None:
-        self._handler = websocket_listener(
-            dependencies=self.dependencies,
-            dto=self.dto,
-            exception_handlers=self.exception_handlers,
-            guards=self.guards,
-            middleware=self.middleware,
-            send_mode=self.send_mode,
-            receive_mode=self.receive_mode,
-            name=self.name,
-            on_accept=self.on_accept,
-            on_disconnect=self.on_disconnect,
-            opt=self.opt,
-            path=self.path,
-            return_dto=self.return_dto,
-            signature_namespace=self.signature_namespace,
-            type_encoders=self.type_encoders,
-        )(self.on_receive)
-
-    def on_accept(self, socket: WebSocket) -> SyncOrAsyncUnion[None]:  # noqa: B027
-        """Called after a WebSocket connection has been accepted"""
-
-    @abstractmethod
-    def on_receive(self, *args: Any, **kwargs: Any) -> Any:
-        """Called after data has been received from the WebSocket.
-
-        This should take a ``data`` argument, receiving the processed WebSocket data,
-        and can additionally include handler dependencies such as ``state``, or other
-        regular dependencies.
+        for route_path, handlers_map in self.get_route_handler_map(value=validated_value).items():
+            path = join_paths([self.path, route_path])
+            if http_handlers := unique(
+                [handler for handler in handlers_map.values() if isinstance(handler, HTTPRouteHandler)]
+            ):
+                if existing_handlers := unique(
+                    [
+                        handler
+                        for handler in self.route_handler_method_map.get(path, {}).values()
+                        if isinstance(handler, HTTPRouteHandler)
+                    ]
+                ):
+                    http_handlers.extend(existing_handlers)
+                    existing_route_index = find_index(self.routes, lambda x: x.path == path)  # noqa: B023
+
+                    if existing_route_index == -1:  # pragma: no cover
+                        raise ImproperlyConfiguredException("unable to find_index existing route index")
+
+                    route: WebSocketRoute | ASGIRoute | HTTPRoute = HTTPRoute(
+                        path=path,
+                        route_handlers=http_handlers,
+                    )
+                    self.routes[existing_route_index] = route
+                else:
+                    route = HTTPRoute(path=path, route_handlers=http_handlers)
+                    self.routes.append(route)
+                routes.append(route)
+
+            if websocket_handler := handlers_map.get("websocket"):
+                route = WebSocketRoute(path=path, route_handler=cast("WebsocketRouteHandler", websocket_handler))
+                self.routes.append(route)
+                routes.append(route)
+
+            if asgi_handler := handlers_map.get("asgi"):
+                route = ASGIRoute(path=path, route_handler=cast("ASGIRouteHandler", asgi_handler))
+                self.routes.append(route)
+                routes.append(route)
+
+        return routes
+
+    @property
+    def route_handler_method_map(self) -> dict[str, RouteHandlerMapItem]:
+        """Map route paths to :class:`RouteHandlerMapItem <litestar.types.internal_typ es.RouteHandlerMapItem>`
 
-        Data returned from this function will be serialized and sent via the socket
-        according to handler configuration.
+        Returns:
+             A dictionary mapping paths to route handlers
         """
-        raise NotImplementedError
-
-    def on_disconnect(self, socket: WebSocket) -> SyncOrAsyncUnion[None]:  # noqa: B027
-        """Called after a WebSocket connection has been disconnected"""
+        route_map: dict[str, RouteHandlerMapItem] = defaultdict(dict)
+        for route in self.routes:
+            if isinstance(route, HTTPRoute):
+                for route_handler in route.route_handlers:
+                    for method in route_handler.http_methods:
+                        route_map[route.path][method] = route_handler
+            else:
+                route_map[route.path][
+                    "websocket" if isinstance(route, WebSocketRoute) else "asgi"
+                ] = route.route_handler
+        return route_map
+
+    @classmethod
+    def get_route_handler_map(
+        cls,
+        value: Controller | RouteHandlerType | Router,
+    ) -> dict[str, RouteHandlerMapItem]:
+        """Map route handlers to HTTP methods."""
+        if isinstance(value, Router):
+            return value.route_handler_method_map
+
+        if isinstance(value, (HTTPRouteHandler, ASGIRouteHandler, WebsocketRouteHandler)):
+            copied_value = copy(value)
+            if isinstance(value, HTTPRouteHandler):
+                return {path: {http_method: copied_value for http_method in value.http_methods} for path in value.paths}
+
+            return {
+                path: {"websocket" if isinstance(value, WebsocketRouteHandler) else "asgi": copied_value}
+                for path in value.paths
+            }
+
+        handlers_map: DefaultDict[str, RouteHandlerMapItem] = defaultdict(dict)
+        for route_handler in value.get_route_handlers():
+            for handler_path in route_handler.paths:
+                path = join_paths([value.path, handler_path]) if handler_path else value.path
+                if isinstance(route_handler, HTTPRouteHandler):
+                    for http_method in route_handler.http_methods:
+                        handlers_map[path][http_method] = route_handler
+                else:
+                    handlers_map[path][
+                        "websocket" if isinstance(route_handler, WebsocketRouteHandler) else "asgi"
+                    ] = cast("WebsocketRouteHandler | ASGIRouteHandler", route_handler)
+
+        return handlers_map
+
+    def _validate_registration_value(self, value: ControllerRouterHandler) -> Controller | RouteHandlerType | Router:
+        """Ensure values passed to the register method are supported."""
+        if is_class_and_subclass(value, Controller):
+            return value(owner=self)
+
+        # this narrows down to an ABC, but we assume a non-abstract subclass of the ABC superclass
+        if is_class_and_subclass(value, WebsocketListener):  # type: ignore[type-abstract]
+            return value()._handler  # pyright: ignore
+
+        if isinstance(value, Router):
+            if value.owner:
+                raise ImproperlyConfiguredException(f"Router with path {value.path} has already been registered")
+            if value is self:
+                raise ImproperlyConfiguredException("Cannot register a router on itself")
+
+            value.owner = self
+            return value
+
+        if isinstance(value, (ASGIRouteHandler, HTTPRouteHandler, WebsocketRouteHandler)):
+            value.owner = self
+            return value
+
+        raise ImproperlyConfiguredException(
+            "Unsupported value passed to `Router.register`. "
+            "If you passed in a function or method, "
+            "make sure to decorate it first with one of the routing decorators"
+        )
```

### Comparing `litestar-2.0.0a4/litestar/logging/_utils.py` & `litestar-2.0.0a5/litestar/logging/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/logging/picologging.py` & `litestar-2.0.0a5/litestar/logging/picologging.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/logging/standard.py` & `litestar-2.0.0a5/litestar/logging/standard.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/middleware/_utils.py` & `litestar-2.0.0a5/litestar/middleware/_utils.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/middleware/allowed_hosts.py` & `litestar-2.0.0a5/litestar/middleware/allowed_hosts.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         if config.www_redirect:
             redirect_domains: set[str] = {
                 host.replace("www.", "") for host in config.allowed_hosts if host.startswith("www.")
             }
             if redirect_domains:
                 self.redirect_domains = re.compile("|".join(sorted(redirect_domains)))  # pyright: ignore
 
-    async def __call__(self, scope: "Scope", receive: "Receive", send: "Send") -> None:
+    async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
         """ASGI callable.
 
         Args:
             scope: The ASGI connection scope.
             receive: The ASGI receive function.
             send: The ASGI send function.
```

### Comparing `litestar-2.0.0a4/litestar/middleware/authentication.py` & `litestar-2.0.0a5/litestar/middleware/authentication.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             scopes: ASGI scopes processed by the authentication middleware.
         """
         self.app = app
         self.scopes = scopes or {ScopeType.HTTP, ScopeType.WEBSOCKET}
         self.exclude_opt_key = exclude_from_auth_key
         self.exclude = build_exclude_path_pattern(exclude=exclude)
 
-    async def __call__(self, scope: "Scope", receive: "Receive", send: "Send") -> None:
+    async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
         """ASGI callable.
 
         Args:
             scope: The ASGI connection scope.
             receive: The ASGI receive function.
             send: The ASGI send function.
```

### Comparing `litestar-2.0.0a4/litestar/middleware/base.py` & `litestar-2.0.0a5/litestar/middleware/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 class MiddlewareProtocol(Protocol):  # pragma: no cover
     """Abstract middleware protocol."""
 
     __slots__ = ("app",)
 
     app: ASGIApp
 
-    async def __call__(self, scope: "Scope", receive: "Receive", send: "Send") -> None:
+    async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
         """Execute the ASGI middleware.
 
         Called by the previous middleware in the stack if a response is not awaited prior.
 
         Upon completion, middleware should call the next ASGI handler and await it - or await a response created in its
         closure.
 
@@ -113,30 +113,30 @@
 
     @classmethod
     def __init_subclass__(cls, **kwargs: Any) -> None:
         super().__init_subclass__(**kwargs)
 
         original__call__ = cls.__call__
 
-        async def wrapped_call(self: AbstractMiddleware, scope: "Scope", receive: "Receive", send: "Send") -> None:
+        async def wrapped_call(self: AbstractMiddleware, scope: Scope, receive: Receive, send: Send) -> None:
             if should_bypass_middleware(
                 scope=scope,
                 scopes=self.scopes,
                 exclude_path_pattern=self.exclude_pattern,
                 exclude_opt_key=self.exclude_opt_key,
             ):
                 await self.app(scope, receive, send)
             else:
                 await original__call__(self, scope, receive, send)
 
         # https://github.com/python/mypy/issues/2427#issuecomment-384229898
         setattr(cls, "__call__", wrapped_call)
 
     @abstractmethod
-    async def __call__(self, scope: "Scope", receive: "Receive", send: "Send") -> None:
+    async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
         """Execute the ASGI middleware.
 
         Called by the previous middleware in the stack if a response is not awaited prior.
 
         Upon completion, middleware should call the next ASGI handler and await it - or await a response created in its
         closure.
```

### Comparing `litestar-2.0.0a4/litestar/middleware/compression.py` & `litestar-2.0.0a5/litestar/middleware/compression.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
             config: An instance of CompressionConfig.
         """
         super().__init__(
             app=app, exclude=config.exclude, exclude_opt_key=config.exclude_opt_key, scopes={ScopeType.HTTP}
         )
         self.config = config
 
-    async def __call__(self, scope: "Scope", receive: "Receive", send: "Send") -> None:
+    async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
         """ASGI callable.
 
         Args:
             scope: The ASGI connection scope.
             receive: The ASGI receive function.
             send: The ASGI send function.
 
@@ -172,15 +172,15 @@
 
         buffer = BytesIO()
         facade = CompressionFacade(buffer=buffer, compression_encoding=compression_encoding, config=self.config)
 
         initial_message = Ref[Optional["HTTPResponseStartEvent"]](None)
         started = Ref[bool](False)
 
-        async def send_wrapper(message: "Message") -> None:
+        async def send_wrapper(message: Message) -> None:
             """Handle and compresses the HTTP Message with brotli.
 
             Args:
                 message (Message): An ASGI Message.
             """
 
             if message["type"] == "http.response.start":
```

### Comparing `litestar-2.0.0a4/litestar/middleware/cors.py` & `litestar-2.0.0a5/litestar/middleware/cors.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         Args:
             app: The ``next`` ASGI app to call.
             config: An instance of :class:`CORSConfig <litestar.config.cors.CORSConfig>`
         """
         super().__init__(app=app, scopes={ScopeType.HTTP})
         self.config = config
 
-    async def __call__(self, scope: "Scope", receive: "Receive", send: "Send") -> None:
+    async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
         """ASGI callable.
 
         Args:
             scope: The ASGI connection scope.
             receive: The ASGI receive function.
             send: The ASGI send function.
 
@@ -56,15 +56,15 @@
             origin: The value of the ``Origin`` header.
             send: The ASGI send function.
 
         Returns:
             An ASGI send function.
         """
 
-        async def wrapped_send(message: "Message") -> None:
+        async def wrapped_send(message: Message) -> None:
             if message["type"] == "http.response.start":
                 message.setdefault("headers", [])
                 headers = MutableScopeHeaders.from_message(message=message)
                 headers.update(self.config.simple_headers)
 
                 if (self.config.is_allow_all_origins and has_cookie) or (
                     not self.config.is_allow_all_origins and self.config.is_origin_allowed(origin=origin)
```

### Comparing `litestar-2.0.0a4/litestar/middleware/csrf.py` & `litestar-2.0.0a5/litestar/middleware/csrf.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
             app: The ``next`` ASGI app to call.
             config: The CSRFConfig instance.
         """
         self.app = app
         self.config = config
         self.exclude = build_exclude_path_pattern(exclude=config.exclude)
 
-    async def __call__(self, scope: "Scope", receive: "Receive", send: "Send") -> None:
+    async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
         """ASGI callable.
 
         Args:
             scope: The ASGI connection scope.
             receive: The ASGI receive function.
             send: The ASGI send function.
 
@@ -131,15 +131,15 @@
             send: The ASGI send function.
             csrf_cookie: CSRF cookie.
 
         Returns:
             An ASGI send function.
         """
 
-        async def send_wrapper(message: "Message") -> None:
+        async def send_wrapper(message: Message) -> None:
             """Send function that wraps the original send to inject a cookie.
 
             Args:
                 message: An ASGI ``Message``
 
             Returns:
                 None
```

### Comparing `litestar-2.0.0a4/litestar/middleware/exceptions/_debug_response.py` & `litestar-2.0.0a5/litestar/middleware/exceptions/_debug_response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/middleware/exceptions/middleware.py` & `litestar-2.0.0a5/litestar/middleware/exceptions/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,15 @@
             debug: Whether ``debug`` mode is enabled
             exception_handlers: A dictionary mapping status codes and/or exception types to handler functions.
         """
         self.app = app
         self.exception_handlers = exception_handlers
         self.debug = debug
 
-    async def __call__(self, scope: "Scope", receive: "Receive", send: "Send") -> None:
+    async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
         """ASGI-callable.
 
         Args:
             scope: The ASGI connection scope.
             receive: The ASGI receive function.
             send: The ASGI send function.
 
@@ -160,15 +160,15 @@
                 await self.handle_request_exception(
                     litestar_app=litestar_app, scope=scope, receive=receive, send=send, exc=e
                 )
             else:
                 await self.handle_websocket_exception(send=send, exc=e)
 
     async def handle_request_exception(
-        self, litestar_app: "Litestar", scope: "Scope", receive: "Receive", send: "Send", exc: Exception
+        self, litestar_app: Litestar, scope: Scope, receive: Receive, send: Send, exc: Exception
     ) -> None:
         """Handle exception raised inside 'http' scope routes.
 
         Args:
             litestar_app: The litestar app instance.
             scope: The ASGI connection scope.
             receive: The ASGI receive function.
@@ -185,15 +185,15 @@
             send = cors_middleware.send_wrapper(send=send, origin=origin, has_cookie="cookie" in headers)
 
         exception_handler = get_exception_handler(self.exception_handlers, exc) or self.default_http_exception_handler
         response = exception_handler(Request(scope=scope, receive=receive, send=send), exc)
         await response(scope=scope, receive=receive, send=send)
 
     @staticmethod
-    async def handle_websocket_exception(send: "Send", exc: Exception) -> None:
+    async def handle_websocket_exception(send: Send, exc: Exception) -> None:
         """Handle exception raised inside 'websocket' scope routes.
 
         Args:
             send: The ASGI send function.
             exc: The caught exception.
 
         Returns:
```

### Comparing `litestar-2.0.0a4/litestar/middleware/exceptions/templates/scripts.js` & `litestar-2.0.0a5/litestar/middleware/exceptions/templates/scripts.js`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/middleware/exceptions/templates/styles.css` & `litestar-2.0.0a5/litestar/middleware/exceptions/templates/styles.css`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/middleware/logging.py` & `litestar-2.0.0a5/litestar/middleware/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
             extract_body="body" in self.config.response_log_fields,
             extract_headers="headers" in self.config.response_log_fields,
             extract_status_code="status_code" in self.config.response_log_fields,
             obfuscate_cookies=self.config.response_cookies_to_obfuscate,
             obfuscate_headers=self.config.response_headers_to_obfuscate,
         )
 
-    async def __call__(self, scope: "Scope", receive: "Receive", send: "Send") -> None:
+    async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
         """ASGI callable.
 
         Args:
             scope: The ASGI connection scope.
             receive: The ASGI receive function.
             send: The ASGI send function.
 
@@ -112,15 +112,15 @@
             send = self.create_send_wrapper(scope=scope, send=send)
 
         if self.config.request_log_fields:
             await self.log_request(scope=scope, receive=receive)
 
         await self.app(scope, receive, send)
 
-    async def log_request(self, scope: "Scope", receive: "Receive") -> None:
+    async def log_request(self, scope: Scope, receive: Receive) -> None:
         """Extract request data and log the message.
 
         Args:
             scope: The ASGI connection scope.
             receive: ASGI receive callable
 
         Returns:
@@ -161,15 +161,15 @@
     def _serialize_value(self, serializer: Serializer | None, value: Any) -> Any:
         if not self.is_struct_logger and isinstance(value, (dict, list, tuple, set)):
             value = encode_json(value, serializer)
         if isinstance(value, bytes):
             return value.decode("utf-8")
         return value
 
-    async def extract_request_data(self, request: "Request") -> dict[str, Any]:
+    async def extract_request_data(self, request: Request) -> dict[str, Any]:
         """Create a dictionary of values for the message.
 
         Args:
             request: A :class:`Request <litestar.connection.Request>` instance.
 
         Returns:
             An dict.
@@ -220,15 +220,15 @@
             scope: The ASGI connection scope.
             send: The ASGI send function.
 
         Returns:
             An ASGI send function.
         """
 
-        async def send_wrapper(message: "Message") -> None:
+        async def send_wrapper(message: Message) -> None:
             if message["type"] == HTTP_RESPONSE_START:
                 set_litestar_scope_state(scope, HTTP_RESPONSE_START, message)
             elif message["type"] == HTTP_RESPONSE_BODY:
                 set_litestar_scope_state(scope, HTTP_RESPONSE_BODY, message)
                 self.log_response(scope=scope)
             await send(message)
 
@@ -336,15 +336,15 @@
     def middleware(self) -> DefineMiddleware:
         """Use this property to insert the config into a middleware list on one of the application layers.
 
         Examples:
             .. code-block: python
 
                 from litestar import Litestar, Request, get
-                from litestar.config.logging import LoggingConfig
+                from litestar.logging import LoggingConfig
                 from litestar.middleware.logging import LoggingMiddlewareConfig
 
                 logging_config = LoggingConfig()
 
                 logging_middleware_config = LoggingMiddlewareConfig()
 
                 @get("/")
```

### Comparing `litestar-2.0.0a4/litestar/middleware/rate_limit.py` & `litestar-2.0.0a5/litestar/middleware/rate_limit.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             app=app, exclude=config.exclude, exclude_opt_key=config.exclude_opt_key, scopes={ScopeType.HTTP}
         )
         self.check_throttle_handler = cast("Callable[[Request], Awaitable[bool]] | None", config.check_throttle_handler)
         self.config = config
         self.max_requests: int = config.rate_limit[1]
         self.unit: DurationUnit = config.rate_limit[0]
 
-    async def __call__(self, scope: "Scope", receive: "Receive", send: "Send") -> None:
+    async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
         """ASGI callable.
 
         Args:
             scope: The ASGI connection scope.
             receive: The ASGI receive function.
             send: The ASGI send function.
 
@@ -94,15 +94,15 @@
             send: The ASGI send function.
             cache_object: A StorageObject instance.
 
         Returns:
             Send wrapper callable.
         """
 
-        async def send_wrapper(message: "Message") -> None:
+        async def send_wrapper(message: Message) -> None:
             """Wrap the ASGI ``Send`` callable.
 
             Args:
                 message: An ASGI ``Message``
 
             Returns:
                 None
@@ -170,15 +170,15 @@
 
         Returns:
             None
         """
         cache_object.history = [int(time()), *cache_object.history]
         await store.set(key, encode_json(cache_object), expires_in=DURATION_VALUES[self.unit])
 
-    async def should_check_request(self, request: "Request[Any, Any, Any]") -> bool:
+    async def should_check_request(self, request: Request[Any, Any, Any]) -> bool:
         """Return a boolean indicating if a request should be checked for rate limiting.
 
         Args:
             request: A :class:`Request <.connection.Request>` instance.
 
         Returns:
             Boolean dictating whether the request should be checked for rate-limiting.
```

### Comparing `litestar-2.0.0a4/litestar/middleware/session/base.py` & `litestar-2.0.0a5/litestar/middleware/session/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,17 +142,15 @@
 
         Returns:
             Deserialized data as a dictionary
         """
         return cast("dict[str, Any]", decode_json(data))
 
     @abstractmethod
-    async def store_in_message(
-        self, scope_session: "ScopeSession", message: "Message", connection: ASGIConnection
-    ) -> None:
+    async def store_in_message(self, scope_session: ScopeSession, message: Message, connection: ASGIConnection) -> None:
         """Store the necessary information in the outgoing ``Message``
 
         Args:
             scope_session: Current session to store
             message: Outgoing send-message
             connection: Originating ASGIConnection containing the scope
 
@@ -203,15 +201,15 @@
         Args:
             connection: ASGIConnection
 
         Returns:
             None
         """
 
-        async def wrapped_send(message: "Message") -> None:
+        async def wrapped_send(message: Message) -> None:
             """Wrap the ``send`` function.
 
             Declared in local scope to make use of closure values.
 
             Args:
                 message: An ASGI message.
 
@@ -225,15 +223,15 @@
             scope_session = connection.scope.get("session")
 
             await self.backend.store_in_message(scope_session, message, connection)
             await connection.send(message)
 
         return wrapped_send
 
-    async def __call__(self, scope: "Scope", receive: "Receive", send: "Send") -> None:
+    async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
         """ASGI-callable.
 
         Args:
             scope: The ASGI connection scope.
             receive: The ASGI receive function.
             send: The ASGI send function.
```

### Comparing `litestar-2.0.0a4/litestar/middleware/session/client_side.py` & `litestar-2.0.0a5/litestar/middleware/session/client_side.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,17 +122,15 @@
                 value=datum.decode("utf-8"),
                 key=f"{self.config.key}-{i}",
                 **cookie_params,
             )
             for i, datum in enumerate(data)
         ]
 
-    async def store_in_message(
-        self, scope_session: "ScopeSession", message: "Message", connection: "ASGIConnection"
-    ) -> None:
+    async def store_in_message(self, scope_session: ScopeSession, message: Message, connection: ASGIConnection) -> None:
         """Store data from ``scope_session`` in ``Message`` in the form of cookies. If the contents of ``scope_session``
         are too large to fit a single cookie, it will be split across several cookies, following the naming scheme of
         ``<cookie key>-<n>``. If the session is empty or shrinks, cookies will be cleared by setting their value to
         ``"null"``
 
         Args:
             scope_session: Current session to store
@@ -175,15 +173,15 @@
                 )
             )
             headers.add(
                 "Set-Cookie",
                 Cookie(value="null", key=cookie_key, expires=0, **cookie_params).to_header(header=""),
             )
 
-    async def load_from_connection(self, connection: "ASGIConnection") -> dict[str, Any]:
+    async def load_from_connection(self, connection: ASGIConnection) -> dict[str, Any]:
         """Load session data from a connection's session-cookies and return it as a dictionary.
 
         Args:
             connection: Originating ASGIConnection
 
         Returns:
             The session data
```

### Comparing `litestar-2.0.0a4/litestar/middleware/session/server_side.py` & `litestar-2.0.0a5/litestar/middleware/session/server_side.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,17 +82,15 @@
         n=:attr:`session_id_bytes <ServerSideSessionConfig.session_id_bytes>` random bytes.
 
         Returns:
             A session-ID
         """
         return secrets.token_hex(self.config.session_id_bytes)
 
-    async def store_in_message(
-        self, scope_session: "ScopeSession", message: "Message", connection: "ASGIConnection"
-    ) -> None:
+    async def store_in_message(self, scope_session: ScopeSession, message: Message, connection: ASGIConnection) -> None:
         """Store the necessary information in the outgoing ``Message`` by setting a cookie containing the session-ID.
 
         If the session is empty, a null-cookie will be set. Otherwise, the serialised
         data will be stored using :meth:`set <ServerSideSessionBackend.set>`, under the current session-id. If no session-ID
         exists, a new ID will be generated using :meth:`generate_session_id <ServerSideSessionBackend.generate_session_id>`.
 
         Args:
@@ -119,15 +117,15 @@
                 Cookie(value="null", key=self.config.key, expires=0, **cookie_params).to_header(header=""),
             )
         else:
             serialised_data = self.serialize_data(scope_session, scope)
             await self.set(session_id=session_id, data=serialised_data, store=store)
             headers["Set-Cookie"] = Cookie(value=session_id, key=self.config.key, **cookie_params).to_header(header="")
 
-    async def load_from_connection(self, connection: "ASGIConnection") -> dict[str, Any]:
+    async def load_from_connection(self, connection: ASGIConnection) -> dict[str, Any]:
         """Load session data from a connection and return it as a dictionary to be used in the current application
         scope.
 
         The session-ID will be gathered from a cookie with the key set in
         :attr:`BaseBackendConfig.key`. If a cookie is found, its value will be used as the session-ID and data associated
         with this ID will be loaded using :meth:`get <ServerSideSessionBackend.get>`.
         If no cookie was found or no data was loaded from the store, this will return an
```

### Comparing `litestar-2.0.0a4/litestar/openapi/config.py` & `litestar-2.0.0a5/litestar/openapi/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/openapi/controller.py` & `litestar-2.0.0a5/litestar/openapi/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     from litestar.connection.request import Request
     from litestar.openapi.spec.open_api import OpenAPI
 
 
 class OpenAPISchemaResponse(Response):
     """Response class for OpenAPI Schemas."""
 
-    def render(self, content: "OpenAPI") -> bytes:
+    def render(self, content: OpenAPI) -> bytes:
         """Handle rendering of schema into the correct format - either YAML or JSON.
 
         Args:
             content: The :class:`OpenAPI <litestar.openapi.spec.open_api.OpenAPI>` instance to render.
 
         Returns:
             Rendered bytes.
@@ -89,26 +89,26 @@
     _dumped_modified_schema: str = ""
     # set the dto types to `None` to ensure that if a dto is supplied at the application layer, they don't apply to
     # this controller.
     dto = None
     return_dto = None
 
     @staticmethod
-    def get_schema_from_request(request: Request) -> "OpenAPI":
+    def get_schema_from_request(request: Request) -> OpenAPI:
         """Return the OpenAPI pydantic model from the request instance.
 
         Args:
             request: A :class:`Litestar <.connection.Request>` instance.
 
         Returns:
             An :class:`OpenAPI <litestar.openapi.spec.open_api.OpenAPI>` instance.
         """
         return request.app.openapi_schema
 
-    def should_serve_endpoint(self, request: "Request") -> bool:
+    def should_serve_endpoint(self, request: Request) -> bool:
         """Verify that the requested path is within the enabled endpoints in the openapi_config.
 
         Args:
             request: To be tested if endpoint enabled.
 
         Returns:
             A boolean.
```

### Comparing `litestar-2.0.0a4/litestar/openapi/datastructures.py` & `litestar-2.0.0a5/litestar/openapi/datastructures.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/openapi/spec/__init__.py` & `litestar-2.0.0a5/litestar/openapi/spec/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/openapi/spec/base.py` & `litestar-2.0.0a5/litestar/openapi/spec/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/openapi/spec/callback.py` & `litestar-2.0.0a5/litestar/openapi/spec/callback.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/openapi/spec/components.py` & `litestar-2.0.0a5/litestar/openapi/spec/components.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/openapi/spec/contact.py` & `litestar-2.0.0a5/litestar/openapi/spec/contact.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/openapi/spec/discriminator.py` & `litestar-2.0.0a5/litestar/openapi/spec/discriminator.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/openapi/spec/encoding.py` & `litestar-2.0.0a5/litestar/openapi/spec/encoding.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/openapi/spec/enums.py` & `litestar-2.0.0a5/litestar/openapi/spec/enums.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/openapi/spec/example.py` & `litestar-2.0.0a5/litestar/openapi/spec/example.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/openapi/spec/external_documentation.py` & `litestar-2.0.0a5/litestar/openapi/spec/external_documentation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/openapi/spec/header.py` & `litestar-2.0.0a5/litestar/openapi/spec/header.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/openapi/spec/info.py` & `litestar-2.0.0a5/litestar/openapi/spec/info.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/openapi/spec/license.py` & `litestar-2.0.0a5/litestar/openapi/spec/license.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/openapi/spec/link.py` & `litestar-2.0.0a5/litestar/openapi/spec/link.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/openapi/spec/media_type.py` & `litestar-2.0.0a5/litestar/openapi/spec/media_type.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/openapi/spec/oauth_flow.py` & `litestar-2.0.0a5/litestar/openapi/spec/oauth_flow.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/openapi/spec/oauth_flows.py` & `litestar-2.0.0a5/litestar/openapi/spec/oauth_flows.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/openapi/spec/open_api.py` & `litestar-2.0.0a5/litestar/openapi/spec/open_api.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/openapi/spec/operation.py` & `litestar-2.0.0a5/litestar/openapi/spec/operation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/openapi/spec/parameter.py` & `litestar-2.0.0a5/litestar/openapi/spec/parameter.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/openapi/spec/path_item.py` & `litestar-2.0.0a5/litestar/openapi/spec/path_item.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/openapi/spec/paths.py` & `litestar-2.0.0a5/litestar/openapi/spec/paths.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/openapi/spec/reference.py` & `litestar-2.0.0a5/litestar/openapi/spec/reference.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/openapi/spec/request_body.py` & `litestar-2.0.0a5/litestar/openapi/spec/request_body.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/openapi/spec/response.py` & `litestar-2.0.0a5/litestar/openapi/spec/response.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/openapi/spec/responses.py` & `litestar-2.0.0a5/litestar/openapi/spec/responses.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/openapi/spec/schema.py` & `litestar-2.0.0a5/litestar/openapi/spec/schema.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/openapi/spec/security_requirement.py` & `litestar-2.0.0a5/litestar/openapi/spec/security_requirement.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/openapi/spec/security_scheme.py` & `litestar-2.0.0a5/litestar/openapi/spec/security_scheme.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/openapi/spec/server.py` & `litestar-2.0.0a5/litestar/openapi/spec/server.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/openapi/spec/server_variable.py` & `litestar-2.0.0a5/litestar/openapi/spec/server_variable.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/openapi/spec/tag.py` & `litestar-2.0.0a5/litestar/openapi/spec/tag.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/openapi/spec/xml.py` & `litestar-2.0.0a5/litestar/openapi/spec/xml.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/pagination.py` & `litestar-2.0.0a5/litestar/pagination.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/params.py` & `litestar-2.0.0a5/litestar/params.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/partial.py` & `litestar-2.0.0a5/litestar/partial.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         cls._models[item] = make_dataclass(
             cls_name=_create_partial_type_name(item),
             fields=field_definitions,
             bases=(item,),
         )
 
     @classmethod
-    def _create_partial_typeddict(cls, item: "TypedDictClass") -> None:
+    def _create_partial_typeddict(cls, item: TypedDictClass) -> None:
         """Receives a typeddict class and creates a new type with all attributes ``Optional``.
 
         Args:
             item: A :class:`TypedDict <typing.TypeDict>` class.
         """
         field_definitions: dict[str, Any] = {}
         for field_name, field_type in _extract_type_hints(item):
```

### Comparing `litestar-2.0.0a4/litestar/response/base.py` & `litestar-2.0.0a5/litestar/response/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,15 +288,15 @@
 
         Returns:
             None
         """
         if self.background is not None:
             await self.background()
 
-    async def start_response(self, send: "Send") -> None:
+    async def start_response(self, send: Send) -> None:
         """Emit the start event of the response. This event includes the headers and status codes.
 
         Args:
             send: The ASGI send function.
 
         Returns:
             None
@@ -312,15 +312,15 @@
             "type": "http.response.start",
             "status": self.status_code,
             "headers": encoded_headers,
         }
 
         await send(event)
 
-    async def send_body(self, send: "Send", receive: "Receive") -> None:
+    async def send_body(self, send: Send, receive: Receive) -> None:
         """Emit the response body.
 
         Args:
             send: The ASGI send function.
             receive: The ASGI receive function.
 
         Notes:
@@ -328,15 +328,15 @@
 
         Returns:
             None
         """
         event: HTTPResponseBodyEvent = {"type": "http.response.body", "body": self.body, "more_body": False}
         await send(event)
 
-    async def __call__(self, scope: "Scope", receive: "Receive", send: "Send") -> None:
+    async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
         """ASGI callable of the ``Response``.
 
         Args:
             scope: The ASGI connection scope.
             receive: The ASGI receive function.
             send: The ASGI send function.
```

### Comparing `litestar-2.0.0a4/litestar/response/file.py` & `litestar-2.0.0a5/litestar/response/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from email.utils import formatdate
 from inspect import iscoroutine
-from mimetypes import guess_type
+from mimetypes import encodings_map, guess_type
 from typing import TYPE_CHECKING, Any, AsyncGenerator, Coroutine, Literal, cast
 from urllib.parse import quote
 from zlib import adler32
 
 from litestar.constants import ONE_MEGABYTE
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.file_system import BaseLocalFileSystem, FileSystemAdapter
@@ -24,17 +24,20 @@
 
     from litestar.background_tasks import BackgroundTask, BackgroundTasks
     from litestar.datastructures.headers import ETag
     from litestar.enums import MediaType
     from litestar.types import HTTPResponseBodyEvent, PathType, Receive, ResponseCookies, Send
     from litestar.types.file_types import FileInfo, FileSystemProtocol
 
+# brotli not supported in 'mimetypes.encodings_map' until py 3.9.
+encodings_map[".br"] = "br"
+
 
 async def async_file_iterator(
-    file_path: "PathType", chunk_size: int, adapter: "FileSystemAdapter"
+    file_path: PathType, chunk_size: int, adapter: FileSystemAdapter
 ) -> AsyncGenerator[bytes, None]:
     """Return an async that asynchronously reads a file and yields its chunks.
 
     Args:
         file_path: A path to a file.
         chunk_size: The chunk file to use.
         adapter: File system adapter class.
@@ -121,16 +124,19 @@
                 generated.
             file_system: An implementation of the :class:`FileSystemProtocol <.types.FileSystemProtocol>`. If provided
                 it will be used to load the file.
             file_info: The output of calling :meth:`file_system.info <types.FileSystemProtocol.info>`, equivalent to
                 providing an :class:`os.stat_result`.
         """
         if not media_type:
-            mimetype, _ = guess_type(filename) if filename else (None, None)
+            mimetype, content_encoding = guess_type(filename) if filename else (None, None)
             media_type = mimetype or "application/octet-stream"
+            if content_encoding is not None:
+                headers = headers or {}
+                headers.update({"content-encoding": content_encoding})
 
         self.chunk_size = chunk_size
         self.content_disposition_type = content_disposition_type
         self.etag = etag
         self.file_path = path
         self.filename = filename or ""
         self.adapter = FileSystemAdapter(file_system or BaseLocalFileSystem())
@@ -174,15 +180,15 @@
             Returns the value of :attr:`stat_result.st_size <os.stat_result.st_size>` to populate the ``Content-Length``
                 header.
         """
         if isinstance(self.file_info, dict):
             return self.file_info["size"]
         return 0
 
-    async def send_body(self, send: "Send", receive: "Receive") -> None:
+    async def send_body(self, send: Send, receive: Receive) -> None:
         """Emit a stream of events correlating with the response body.
 
         Args:
             send: The ASGI send function.
             receive: The ASGI receive function.
 
         Returns:
@@ -196,15 +202,15 @@
             body_event: HTTPResponseBodyEvent = {
                 "type": "http.response.body",
                 "body": await file.read(),
                 "more_body": False,
             }
             await send(body_event)
 
-    async def start_response(self, send: "Send") -> None:
+    async def start_response(self, send: Send) -> None:
         """Emit the start event of the response. This event includes the headers and status codes.
 
         Args:
             send: The ASGI send function.
 
         Returns:
             None
```

### Comparing `litestar-2.0.0a4/litestar/response/redirect.py` & `litestar-2.0.0a5/litestar/response/redirect.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/response/streaming.py` & `litestar-2.0.0a5/litestar/response/streaming.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             status_code=status_code,
             is_head_response=is_head_response,
         )
         self.iterator: AsyncIterable[str | bytes] | AsyncGenerator[str | bytes, None] = (
             content if isinstance(content, (AsyncIterable, AsyncIterator)) else AsyncIteratorWrapper(content)
         )
 
-    async def _listen_for_disconnect(self, cancel_scope: "CancelScope", receive: "Receive") -> None:
+    async def _listen_for_disconnect(self, cancel_scope: CancelScope, receive: Receive) -> None:
         """Listen for a cancellation message, and if received - call cancel on the cancel scope.
 
         Args:
             cancel_scope: A task group cancel scope instance.
             receive: The ASGI receive function.
 
         Returns:
@@ -88,15 +88,15 @@
             if message["type"] == "http.disconnect":
                 # despite the IDE warning, this is not a coroutine because anyio 3+ changed this.
                 # therefore make sure not to await this.
                 cancel_scope.cancel()
             else:
                 await self._listen_for_disconnect(cancel_scope=cancel_scope, receive=receive)
 
-    async def _stream(self, send: "Send") -> None:
+    async def _stream(self, send: Send) -> None:
         """Send the chunks from the iterator as a stream of ASGI 'http.response.body' events.
 
         Args:
             send: The ASGI Send function.
 
         Returns:
             None
@@ -107,15 +107,15 @@
                 "body": chunk if isinstance(chunk, bytes) else chunk.encode(self.encoding),
                 "more_body": True,
             }
             await send(stream_event)
         terminus_event: HTTPResponseBodyEvent = {"type": "http.response.body", "body": b"", "more_body": False}
         await send(terminus_event)
 
-    async def send_body(self, send: "Send", receive: "Receive") -> None:
+    async def send_body(self, send: Send, receive: Receive) -> None:
         """Emit a stream of events correlating with the response body.
 
         Args:
             send: The ASGI send function.
             receive: The ASGI receive function.
 
         Returns:
```

### Comparing `litestar-2.0.0a4/litestar/response/template.py` & `litestar-2.0.0a5/litestar/response/template.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/response_containers.py` & `litestar-2.0.0a5/litestar/response_containers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/routes/asgi.py` & `litestar-2.0.0a5/litestar/routes/asgi.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         self.route_handler = route_handler
         super().__init__(
             path=path,
             scope_type=ScopeType.ASGI,
             handler_names=[unwrap_partial(route_handler.handler_name)],
         )
 
-    async def handle(self, scope: "Scope", receive: "Receive", send: "Send") -> None:
+    async def handle(self, scope: Scope, receive: Receive, send: Send) -> None:
         """ASGI app that authorizes the connection and then awaits the handler function.
 
         Args:
             scope: The ASGI connection scope.
             receive: The ASGI receive function.
             send: The ASGI send function.
```

### Comparing `litestar-2.0.0a4/litestar/routes/base.py` & `litestar-2.0.0a5/litestar/routes/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
             component for component in self.path_components if isinstance(component, PathParameterDefinition)
         )
         self.handler_names = handler_names
         self.scope_type = scope_type
         self.methods = set(methods or [])
 
     @abstractmethod
-    async def handle(self, scope: "Scope", receive: "Receive", send: "Send") -> None:  # pragma: no cover
+    async def handle(self, scope: Scope, receive: Receive, send: Send) -> None:  # pragma: no cover
         """ASGI App of the route.
 
         Args:
             scope: The ASGI connection scope.
             receive: The ASGI receive function.
             send: The ASGI send function.
```

### Comparing `litestar-2.0.0a4/litestar/routes/http.py` & `litestar-2.0.0a5/litestar/routes/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         super().__init__(
             methods=methods,
             path=path,
             scope_type=ScopeType.HTTP,
             handler_names=[route_handler.handler_name for route_handler in self.route_handlers],
         )
 
-    async def handle(self, scope: "HTTPScope", receive: "Receive", send: "Send") -> None:  # type: ignore[override]
+    async def handle(self, scope: HTTPScope, receive: Receive, send: Send) -> None:  # type: ignore[override]
         """ASGI app that creates a Request from the passed in args, determines which handler function to call and then
         handles the call.
 
         Args:
             scope: The ASGI connection scope.
             receive: The ASGI receive function.
             send: The ASGI send function.
@@ -97,19 +97,19 @@
                     raise ImproperlyConfiguredException(
                         f"Handler already registered for path {self.path!r} and http method {http_method}"
                     )
                 self.route_handler_map[http_method] = (route_handler, kwargs_model)
 
     async def _get_response_for_request(
         self,
-        scope: "Scope",
+        scope: Scope,
         request: Request[Any, Any, Any],
-        route_handler: "HTTPRouteHandler",
-        parameter_model: "KwargsModel",
-    ) -> "ASGIApp":
+        route_handler: HTTPRouteHandler,
+        parameter_model: KwargsModel,
+    ) -> ASGIApp:
         """Return a response for the request.
 
         If caching is enabled and a response exist in the cache, the cached response will be returned.
         If caching is enabled and a response does not exist in the cache, the newly created
         response will be cached.
 
         Args:
@@ -136,16 +136,16 @@
                 request=request,
                 route_handler=route_handler,
             )
 
         return response
 
     async def _call_handler_function(
-        self, scope: "Scope", request: Request, parameter_model: "KwargsModel", route_handler: "HTTPRouteHandler"
-    ) -> "ASGIApp":
+        self, scope: Scope, request: Request, parameter_model: KwargsModel, route_handler: HTTPRouteHandler
+    ) -> ASGIApp:
         """Call the before request handlers, retrieve any data required for the route handler, and call the route
         handler's ``to_response`` method.
 
         This is wrapped in a try except block - and if an exception is raised,
         it tries to pass it to an appropriate exception handler - if defined.
         """
         response_data: Any = None
@@ -155,30 +155,25 @@
             response_data = await before_request_handler(request)
 
         if not response_data:
             response_data, cleanup_group = await self._get_response_data(
                 route_handler=route_handler, parameter_model=parameter_model, request=request
             )
 
-        response: ASGIApp = await route_handler.to_response(
-            app=scope["app"],
-            data=response_data,
-            plugins=request.app.serialization_plugins,
-            request=request,
-        )
+        response: ASGIApp = await route_handler.to_response(app=scope["app"], data=response_data, request=request)
 
         if cleanup_group:
             await cleanup_group.cleanup()
 
         return response
 
     @staticmethod
     async def _get_response_data(
-        route_handler: "HTTPRouteHandler", parameter_model: "KwargsModel", request: Request
-    ) -> tuple[Any, "DependencyCleanupGroup" | None]:
+        route_handler: HTTPRouteHandler, parameter_model: KwargsModel, request: Request
+    ) -> tuple[Any, DependencyCleanupGroup | None]:
         """Determine what kwargs are required for the given route handler's ``fn`` and calls it."""
         parsed_kwargs: dict[str, Any] = {}
         cleanup_group: DependencyCleanupGroup | None = None
 
         if parameter_model.has_kwargs and route_handler.signature_model:
             kwargs = parameter_model.to_kwargs(connection=request)
```

### Comparing `litestar-2.0.0a4/litestar/routes/websocket.py` & `litestar-2.0.0a5/litestar/routes/websocket.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
         super().__init__(
             path=path,
             scope_type=ScopeType.WEBSOCKET,
             handler_names=[route_handler.handler_name],
         )
 
-    async def handle(self, scope: "WebSocketScope", receive: "Receive", send: "Send") -> None:  # type: ignore[override]
+    async def handle(self, scope: WebSocketScope, receive: Receive, send: Send) -> None:  # type: ignore[override]
         """ASGI app that creates a WebSocket from the passed in args, and then awaits the handler function.
 
         Args:
             scope: The ASGI connection scope.
             receive: The ASGI receive function.
             send: The ASGI send function.
```

### Comparing `litestar-2.0.0a4/litestar/security/base.py` & `litestar-2.0.0a5/litestar/security/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/security/session_auth/auth.py` & `litestar-2.0.0a5/litestar/security/session_auth/auth.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/security/session_auth/middleware.py` & `litestar-2.0.0a5/litestar/security/session_auth/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             app: An ASGIApp, this value is the next ASGI handler to call in the middleware stack.
             config: An instance of SessionAuth.
         """
         self.app = app
         self.config = config
         self.has_wrapped_middleware = False
 
-    async def __call__(self, scope: "Scope", receive: "Receive", send: "Send") -> None:
+    async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
         """Handle creating a middleware stack and calling it.
 
         Args:
             scope: The ASGI connection scope.
             receive: The ASGI receive function.
             send: The ASGI send function.
 
@@ -89,15 +89,15 @@
             exclude_opt_key: An identifier to use on routes to disable authentication and authorization checks for a particular route.
             scopes: ASGI scopes processed by the authentication middleware.
             retrieve_user_handler: Callable that receives the ``session`` value from the authentication middleware and returns a ``user`` value.
         """
         super().__init__(app=app, exclude=exclude, exclude_from_auth_key=exclude_opt_key, scopes=scopes)
         self.retrieve_user_handler = retrieve_user_handler
 
-    async def authenticate_request(self, connection: "ASGIConnection[Any, Any, Any, Any]") -> AuthenticationResult:
+    async def authenticate_request(self, connection: ASGIConnection[Any, Any, Any, Any]) -> AuthenticationResult:
         """Authenticate an incoming connection.
 
         Args:
             connection: An :class:`ASGIConnection <.connection.ASGIConnection>` instance.
 
         Raises:
             NotAuthorizedException: if session data is empty or user is not found.
```

### Comparing `litestar-2.0.0a4/litestar/serialization.py` & `litestar-2.0.0a5/litestar/serialization.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,23 +23,31 @@
     NameEmail,
     SecretField,
     StrictBool,
 )
 from pydantic.color import Color
 from pydantic.json import decimal_encoder
 
+from litestar.enums import MediaType
 from litestar.exceptions import SerializationException
 from litestar.types import Empty
 
-__all__ = ("dec_hook", "decode_json", "decode_msgpack", "default_serializer", "encode_json", "encode_msgpack")
-
-
 if TYPE_CHECKING:
     from litestar.types import TypeEncodersMap
 
+__all__ = (
+    "dec_hook",
+    "decode_json",
+    "decode_media_type",
+    "decode_msgpack",
+    "default_serializer",
+    "encode_json",
+    "encode_msgpack",
+)
+
 T = TypeVar("T")
 
 
 def _enc_base_model(model: BaseModel) -> Any:
     return model.dict()
 
 
@@ -236,7 +244,30 @@
     """
     try:
         if type_ is Empty:
             return _msgspec_msgpack_decoder.decode(raw)
         return msgspec.msgpack.decode(raw, dec_hook=dec_hook, type=type_)
     except msgspec.DecodeError as msgspec_error:
         raise SerializationException(str(msgspec_error)) from msgspec_error
+
+
+def decode_media_type(raw: bytes, media_type: MediaType | str, type_: Any) -> Any:
+    """Decode a raw value into an object.
+
+    Args:
+        raw: Value to decode
+        media_type: Media type of the value
+        type_: An optional type to decode the data into
+
+    Returns:
+        An object
+
+    Raises:
+        SerializationException: If error decoding ``raw`` or ``media_type`` unsupported.
+    """
+    if media_type == MediaType.JSON:
+        return decode_json(raw, type_=type_)
+
+    if media_type == MediaType.MESSAGEPACK:
+        return decode_msgpack(raw, type_=type_)
+
+    raise SerializationException(f"Unsupported media type: '{media_type}'")
```

### Comparing `litestar-2.0.0a4/litestar/static_files/base.py` & `litestar-2.0.0a5/litestar/static_files/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/static_files/config.py` & `litestar-2.0.0a5/litestar/static_files/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/status_codes.py` & `litestar-2.0.0a5/litestar/status_codes.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/stores/base.py` & `litestar-2.0.0a5/litestar/stores/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/stores/file.py` & `litestar-2.0.0a5/litestar/stores/file.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/stores/memory.py` & `litestar-2.0.0a5/litestar/stores/memory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/stores/redis.py` & `litestar-2.0.0a5/litestar/stores/redis.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/stores/registry.py` & `litestar-2.0.0a5/litestar/stores/registry.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/template/base.py` & `litestar-2.0.0a5/litestar/template/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/template/config.py` & `litestar-2.0.0a5/litestar/template/config.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/testing/__init__.py` & `litestar-2.0.0a5/litestar/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/testing/client/__init__.py` & `litestar-2.0.0a5/litestar/testing/client/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/testing/client/async_client.py` & `litestar-2.0.0a5/litestar/testing/client/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     from litestar.middleware.session.base import BaseBackendConfig
 
 
 T = TypeVar("T", bound=ASGIApp)
 
 
-class AsyncTestClient(AsyncClient, BaseTestClient, Generic[T]):  # type: ignore [misc]
+class AsyncTestClient(AsyncClient, BaseTestClient, Generic[T]):  # type: ignore[misc]
     lifespan_handler: LifeSpanHandler
     exit_stack: AsyncExitStack
 
     def __init__(
         self,
         app: T,
         base_url: str = "http://testserver.local",
@@ -79,15 +79,15 @@
             transport=TestClientTransport(  # type: ignore [arg-type]
                 client=self,
                 raise_server_exceptions=raise_server_exceptions,
                 root_path=root_path,
             ),
         )
 
-    async def __aenter__(self) -> "AsyncTestClient[T]":
+    async def __aenter__(self) -> AsyncTestClient[T]:
         async with AsyncExitStack() as stack:
             self.blocking_portal = portal = stack.enter_context(self.portal())
             self.lifespan_handler = LifeSpanHandler(client=self)
 
             @stack.callback
             def reset_portal() -> None:
                 delattr(self, "blocking_portal")
@@ -154,15 +154,15 @@
             follow_redirects=follow_redirects,
             timeout=timeout,
             extensions=extensions,
         )
 
     async def get(  # type: ignore [override]
         self,
-        url: "URLTypes",
+        url: URLTypes,
         *,
         params: QueryParamTypes | None = None,
         headers: HeaderTypes | None = None,
         cookies: CookieTypes | None = None,
         auth: AuthTypes | UseClientDefault = USE_CLIENT_DEFAULT,
         follow_redirects: bool | UseClientDefault = USE_CLIENT_DEFAULT,
         timeout: TimeoutTypes | UseClientDefault = USE_CLIENT_DEFAULT,
```

### Comparing `litestar-2.0.0a4/litestar/testing/client/base.py` & `litestar-2.0.0a5/litestar/testing/client/base.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/testing/client/sync_client.py` & `litestar-2.0.0a5/litestar/testing/client/sync_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     from litestar.testing.websocket_test_session import WebSocketTestSession
     from litestar.types.helper_types import OptionalSequence
 
 
 T = TypeVar("T", bound=ASGIApp)
 
 
-class TestClient(Client, BaseTestClient, Generic[T]):  # type: ignore [misc]
+class TestClient(Client, BaseTestClient, Generic[T]):  # type: ignore[misc]
     lifespan_handler: LifeSpanHandler
     exit_stack: ExitStack
 
     def __init__(
         self,
         app: T,
         base_url: str = "http://testserver.local",
```

### Comparing `litestar-2.0.0a4/litestar/testing/helpers.py` & `litestar-2.0.0a5/litestar/testing/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     on_app_init: OptionalSequence[OnAppInitHandler] = None,
     on_shutdown: OptionalSequence[LifeSpanHandler] = None,
     on_startup: OptionalSequence[LifeSpanHandler] = None,
     openapi_config: OpenAPIConfig | None = DEFAULT_OPENAPI_CONFIG,
     opt: Mapping[str, Any] | None = None,
     parameters: ParametersMap | None = None,
     plugins: OptionalSequence[PluginProtocol] = None,
-    preferred_validation_backend: Literal["pydantic", "attrs"] = "attrs",
+    preferred_validation_backend: Literal["pydantic", "attrs"] | None = None,
     raise_server_exceptions: bool = True,
     request_class: type[Request] | None = None,
     response_cache_config: ResponseCacheConfig | None = None,
     response_class: ResponseType | None = None,
     response_cookies: ResponseCookies | None = None,
     response_headers: OptionalSequence[ResponseHeader] = None,
     return_dto: type[DTOInterface] | None | EmptyType = Empty,
@@ -338,15 +338,15 @@
     on_app_init: OptionalSequence[OnAppInitHandler] = None,
     on_shutdown: OptionalSequence[LifeSpanHandler] = None,
     on_startup: OptionalSequence[LifeSpanHandler] = None,
     openapi_config: OpenAPIConfig | None = DEFAULT_OPENAPI_CONFIG,
     opt: Mapping[str, Any] | None = None,
     parameters: ParametersMap | None = None,
     plugins: OptionalSequence[PluginProtocol] = None,
-    preferred_validation_backend: Literal["pydantic", "attrs"] = "attrs",
+    preferred_validation_backend: Literal["pydantic", "attrs"] | None = None,
     raise_server_exceptions: bool = True,
     request_class: type[Request] | None = None,
     response_cache_config: ResponseCacheConfig | None = None,
     response_class: ResponseType | None = None,
     response_cookies: ResponseCookies | None = None,
     response_headers: OptionalSequence[ResponseHeader] = None,
     return_dto: type[DTOInterface] | None | EmptyType = Empty,
```

### Comparing `litestar-2.0.0a4/litestar/testing/life_span_handler.py` & `litestar-2.0.0a5/litestar/testing/life_span_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         self.stream_send = StapledObjectStream[Optional["LifeSpanSendMessage"]](*create_memory_object_stream(inf))
         self.stream_receive = StapledObjectStream["LifeSpanReceiveMessage"](*create_memory_object_stream(inf))
 
         with self.client.portal() as portal:
             self.task = portal.start_task_soon(self.lifespan)
             portal.call(self.wait_startup)
 
-    async def receive(self) -> "LifeSpanSendMessage":
+    async def receive(self) -> LifeSpanSendMessage:
         message = await self.stream_send.receive()
         if message is None:
             self.task.result()
         return cast("LifeSpanSendMessage", message)
 
     async def wait_startup(self) -> None:
         event: LifeSpanStartupEvent = {"type": "lifespan.startup"}
```

### Comparing `litestar-2.0.0a4/litestar/testing/request_factory.py` & `litestar-2.0.0a5/litestar/testing/request_factory.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/testing/transport.py` & `litestar-2.0.0a5/litestar/testing/transport.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     ) -> None:
         self.client = client
         self.raise_server_exceptions = raise_server_exceptions
         self.root_path = root_path
 
     @staticmethod
     def create_receive(request: Request, context: SendReceiveContext) -> Receive:
-        async def receive() -> "ReceiveMessage":
+        async def receive() -> ReceiveMessage:
             if context["request_complete"]:
                 if not context["response_complete"].is_set():
                     await context["response_complete"].wait()
                 disconnect_event: HTTPDisconnectEvent = {"type": "http.disconnect"}
                 return disconnect_event
 
             body = cast("Union[bytes, str, GeneratorType]", (request.read() or b""))
@@ -78,15 +78,15 @@
                 request_event["body"] = body if isinstance(body, bytes) else body.encode("utf-8")
             return request_event
 
         return receive
 
     @staticmethod
     def create_send(request: Request, context: SendReceiveContext) -> Send:
-        async def send(message: "Message") -> None:
+        async def send(message: Message) -> None:
             if message["type"] == "http.response.start":
                 assert not context[  # noqa: S101
                     "response_started"
                 ], 'Received multiple "http.response.start" messages.'
                 context["raw_kwargs"]["status_code"] = message["status"]
                 context["raw_kwargs"]["headers"] = [
                     (k.decode("utf-8"), v.decode("utf-8")) for k, v in message.get("headers", [])
@@ -189,9 +189,9 @@
 
             stream = ByteStream(raw_kwargs.pop("stream", BytesIO()).read())
             response = Response(**raw_kwargs, stream=stream, request=request)
             setattr(response, "template", context["template"])
             setattr(response, "context", context["context"])
             return response
 
-    async def handle_async_request(self, request: "Request") -> "Response":
+    async def handle_async_request(self, request: Request) -> Response:
         return self.handle_request(request=request)
```

### Comparing `litestar-2.0.0a4/litestar/testing/websocket_test_session.py` & `litestar-2.0.0a5/litestar/testing/websocket_test_session.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,20 +66,20 @@
             message = self.send_queue.get()
             if isinstance(message, BaseException):
                 raise message
 
     async def do_asgi_call(self) -> None:
         """The sub-thread in which the websocket session runs."""
 
-        async def receive() -> "WebSocketReceiveMessage":
+        async def receive() -> WebSocketReceiveMessage:
             while self.receive_queue.empty():
                 await sleep(0)
             return self.receive_queue.get()
 
-        async def send(message: "WebSocketSendMessage") -> None:
+        async def send(message: WebSocketSendMessage) -> None:
             if message["type"] == "websocket.accept":
                 headers = message.get("headers", [])
                 if headers:
                     headers_list = list(self.scope["headers"])
                     headers_list.extend(headers)
                     self.scope["headers"] = headers_list
                 subprotocols = cast("str | None", message.get("subprotocols"))
```

### Comparing `litestar-2.0.0a4/litestar/types/__init__.py` & `litestar-2.0.0a5/litestar/types/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/types/asgi_types.py` & `litestar-2.0.0a5/litestar/types/asgi_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/types/callable_types.py` & `litestar-2.0.0a5/litestar/types/callable_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/types/composite_types.py` & `litestar-2.0.0a5/litestar/types/composite_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/types/file_types.py` & `litestar-2.0.0a5/litestar/types/file_types.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/types/internal_types.py` & `litestar-2.0.0a5/litestar/types/internal_types.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,43 +6,50 @@
     Literal,
     NamedTuple,
     Optional,
     Type,
     Union,
 )
 
+from typing_extensions import TypeAlias
+
 from litestar.types import Method
 
 __all__ = (
+    "AnyConnection",
     "PathParameterDefinition",
     "ControllerRouterHandler",
+    "PathParameterDefinition",
     "ReservedKwargs",
     "ResponseType",
     "RouteHandlerMapItem",
     "RouteHandlerType",
 )
 
 
 if TYPE_CHECKING:
     from litestar.app import Litestar
+    from litestar.connection import ASGIConnection
     from litestar.controller import Controller
     from litestar.handlers.asgi_handlers import ASGIRouteHandler
     from litestar.handlers.http_handlers import HTTPRouteHandler
     from litestar.handlers.websocket_handlers import WebsocketRouteHandler
     from litestar.response import Response
     from litestar.router import Router
 else:
     Litestar = Any
+    ASGIConnection = Any
     ASGIRouteHandler = Any
     WebsocketRouteHandler = Any
     HTTPRouteHandler = Any
     Response = Any
     Controller = Any
     Router = Any
 
+AnyConnection: TypeAlias = "ASGIConnection[Any, Any, Any, Any]"
 ReservedKwargs = Literal["request", "socket", "headers", "query", "cookies", "state", "data"]
 LitestarType = Litestar
 RouteHandlerType = Union[HTTPRouteHandler, WebsocketRouteHandler, ASGIRouteHandler]
 ResponseType = Type[Response]
 ControllerRouterHandler = Union[Type[Controller], RouteHandlerType, Router, Callable[..., Any]]
 RouteHandlerMapItem = Dict[Union[Method, Literal["websocket", "asgi"]], RouteHandlerType]
```

### Comparing `litestar-2.0.0a4/litestar/types/protocols.py` & `litestar-2.0.0a5/litestar/types/protocols.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/types/serialization.py` & `litestar-2.0.0a5/litestar/types/serialization.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/utils/__init__.py` & `litestar-2.0.0a5/litestar/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/utils/compat.py` & `litestar-2.0.0a5/litestar/utils/compat.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/utils/dataclass.py` & `litestar-2.0.0a5/litestar/utils/dataclass.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,30 +76,33 @@
     Returns:
         A tuple of key/value pairs.
     """
     dataclass_fields = extract_dataclass_fields(dt, exclude_none, exclude_empty, include, exclude)
     return tuple((field.name, getattr(dt, field.name)) for field in dataclass_fields)
 
 
-def simple_asdict(obj: DataclassProtocol, exclude_none: bool = False, exclude_empty: bool = False) -> dict[str, Any]:
+def simple_asdict(
+    obj: DataclassProtocol, exclude_none: bool = False, exclude_empty: bool = False, convert_nested: bool = True
+) -> dict[str, Any]:
     """Convert a dataclass to a dictionary.
 
     This method has important differences to the standard library version:
     - it does not deepcopy values
     - it does not recurse into collections
 
     Args:
         obj: A dataclass instance.
         exclude_none: Whether to exclude None values.
         exclude_empty: Whether to exclude Empty values.
+        convert_nested: Whether to recursively convert nested dataclasses.
 
     Returns:
         A dictionary of key/value pairs.
     """
     ret = {}
     for field in extract_dataclass_fields(obj, exclude_none, exclude_empty):
         value = getattr(obj, field.name)
-        if isinstance(value, DataclassProtocol):
+        if isinstance(value, DataclassProtocol) and convert_nested:
             ret[field.name] = simple_asdict(value, exclude_none, exclude_empty)
         else:
             ret[field.name] = getattr(obj, field.name)
     return ret
```

### Comparing `litestar-2.0.0a4/litestar/utils/deprecation.py` & `litestar-2.0.0a5/litestar/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/utils/helpers.py` & `litestar-2.0.0a5/litestar/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/utils/path.py` & `litestar-2.0.0a5/litestar/utils/path.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/utils/predicates.py` & `litestar-2.0.0a5/litestar/utils/predicates.py`

 * *Files 1% similar despite different names*

```diff
@@ -239,29 +239,29 @@
 
     Returns:
         ``True`` if instance or type of ``TypedDict``.
     """
     return is_typeddict(annotation)
 
 
-def is_pydantic_model_class(annotation: Any) -> "TypeGuard[type[pydantic.BaseModel]]":  # pyright: ignore
+def is_pydantic_model_class(annotation: Any) -> TypeGuard[type[pydantic.BaseModel]]:  # pyright: ignore
     """Given a type annotation determine if the annotation is a subclass of pydantic's BaseModel.
 
     Args:
         annotation: A type.
 
     Returns:
         A typeguard determining whether the type is :data:`BaseModel pydantic.BaseModel>`.
     """
     if pydantic is not Empty:  # type: ignore[comparison-overlap]
         return is_class_and_subclass(annotation, pydantic.BaseModel)  # pyright: ignore
     return False  # pragma: no cover
 
 
-def is_pydantic_model_instance(annotation: Any) -> "TypeGuard[pydantic.BaseModel]":  # pyright: ignore
+def is_pydantic_model_instance(annotation: Any) -> TypeGuard[pydantic.BaseModel]:  # pyright: ignore
     """Given a type annotation determine if the annotation is an instance of pydantic's BaseModel.
 
     Args:
         annotation: A type.
 
     Returns:
         A typeguard determining whether the type is :data:`BaseModel pydantic.BaseModel>`.
```

### Comparing `litestar-2.0.0a4/litestar/utils/scope.py` & `litestar-2.0.0a5/litestar/utils/scope.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/utils/sequence.py` & `litestar-2.0.0a5/litestar/utils/sequence.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/utils/signature.py` & `litestar-2.0.0a5/litestar/utils/signature.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from __future__ import annotations
 
 import sys
 import typing
 from dataclasses import dataclass
 from inspect import Parameter, Signature, getmembers, isclass, ismethod
 from itertools import chain
-from typing import Any, AnyStr, Collection, Union
+from typing import Any, AnyStr, Collection, ForwardRef, TypeVar, Union
 
-from typing_extensions import Annotated, NotRequired, Required, get_args, get_origin, get_type_hints
+from typing_extensions import Annotated, NotRequired, Required, Self, get_args, get_origin, get_type_hints
 
 from litestar import connection, datastructures, types
 from litestar.datastructures import ImmutableState
+from litestar.enums import RequestEncodingType
 from litestar.exceptions import ImproperlyConfiguredException
 from litestar.params import BodyKwarg, DependencyKwarg, ParameterKwarg
 from litestar.types import AnyCallable, Empty
 from litestar.types.builtin_types import UNION_TYPES, NoneType
 from litestar.utils.typing import get_safe_generic_origin, unwrap_annotation
 
 _GLOBAL_NAMES = {
@@ -26,29 +27,37 @@
     and namespace in chain(types.__all__, connection.__all__, datastructures.__all__)  # pyright: ignore
 }
 """A mapping of names used for handler signature forward-ref resolution.
 
 This allows users to include these names within an `if TYPE_CHECKING:` block in their handler module.
 """
 
-__all__ = ("get_fn_type_hints", "ParsedType", "ParsedParameter", "ParsedSignature")
+__all__ = (
+    "get_fn_type_hints",
+    "ParsedType",
+    "ParsedParameter",
+    "ParsedSignature",
+    "infer_request_encoding_from_parameter",
+)
 
 
 def get_fn_type_hints(fn: Any, namespace: dict[str, Any] | None = None) -> dict[str, Any]:
     """Resolve type hints for ``fn``.
 
     Args:
         fn: Callable that is being inspected
         namespace: Extra names for resolution of forward references.
 
     Returns:
         Mapping of names to types.
     """
     fn_to_inspect: Any = fn
 
+    module_name = fn_to_inspect.__module__
+
     if isclass(fn_to_inspect):
         fn_to_inspect = fn_to_inspect.__init__
 
     # detect objects that are not functions and that have a `__call__` method
     if callable(fn_to_inspect) and ismethod(fn_to_inspect.__call__):
         fn_to_inspect = fn_to_inspect.__call__
 
@@ -57,21 +66,21 @@
         fn_to_inspect = fn_to_inspect.__func__
 
     # Order important. If a litestar name has been overridden in the function module, we want
     # to use that instead of the litestar one.
     namespace = {
         **_GLOBAL_NAMES,
         **vars(typing),
-        **vars(sys.modules[fn_to_inspect.__module__]),
+        **vars(sys.modules[module_name]),
         **(namespace or {}),
     }
     return get_type_hints(fn_to_inspect, globalns=namespace, include_extras=True)
 
 
-@dataclass(frozen=True)
+@dataclass(frozen=True, init=False)
 class ParsedType:
     """Represents a type annotation."""
 
     __slots__ = (
         "raw",
         "annotation",
         "origin",
@@ -104,18 +113,67 @@
     """An equivalent type to ``origin`` that can be safely used as a generic type across all supported Python versions.
 
     This is to serve safely rebuilding a generic outer type with different args at runtime.
     """
     inner_types: tuple[ParsedType, ...]
     """The type's generic args parsed as ``ParsedType``, if applicable."""
 
+    def __init__(self, annotation: Any) -> None:
+        """Initialize ParsedType.
+
+        Args:
+            annotation: The type annotation. This should be extracted from the return of
+                ``get_type_hints(..., include_extras=True)`` so that forward references are resolved and recursive
+                ``Annotated`` types are flattened.
+
+        Returns:
+            ParsedType
+        """
+        unwrapped, metadata, wrappers = unwrap_annotation(annotation)
+        origin = get_origin(unwrapped)
+        args = get_args(unwrapped)
+        object.__setattr__(self, "raw", annotation)
+        object.__setattr__(self, "annotation", unwrapped)
+        object.__setattr__(self, "origin", origin)
+        object.__setattr__(self, "args", args)
+        object.__setattr__(self, "metadata", metadata)
+        object.__setattr__(self, "is_annotated", Annotated in wrappers)
+        object.__setattr__(self, "is_required", Required in wrappers)
+        object.__setattr__(self, "is_not_required", NotRequired in wrappers)
+        object.__setattr__(self, "safe_generic_origin", get_safe_generic_origin(origin))
+        object.__setattr__(self, "inner_types", tuple(ParsedType(arg) for arg in args))
+
+    def __eq__(self, other: Any) -> bool:
+        if not isinstance(other, ParsedType):
+            return False
+
+        if self.origin:
+            return bool(self.origin == other.origin and self.inner_types == other.inner_types)
+
+        return bool(self.annotation == other.annotation)
+
+    @property
+    def is_forward_ref(self) -> bool:
+        """Whether the annotation is a forward reference or not."""
+        return isinstance(self.annotation, (str, ForwardRef))
+
+    @property
+    def is_type_var(self) -> bool:
+        """Whether the annotation is a TypeVar or not."""
+        return isinstance(self.annotation, TypeVar)
+
+    @property
+    def is_union(self) -> bool:
+        """Whether the annotation is a union type or not."""
+        return self.origin in UNION_TYPES
+
     @property
     def is_optional(self) -> bool:
         """Whether the annotation is Optional or not."""
-        return bool(self.origin in UNION_TYPES and NoneType in self.args)
+        return bool(self.is_union and NoneType in self.args)
 
     @property
     def is_collection(self) -> bool:
         """Whether the annotation is a collection type or not."""
         return bool(self.origin and self.origin is not Union and issubclass(self.origin, Collection))
 
     def is_subclass_of(self, cl: type[Any] | tuple[type[Any], ...]) -> bool:
@@ -130,56 +188,27 @@
         Returns:
             Whether the annotation is a subtype of the given type(s).
         """
         if self.origin:
             return self.origin not in UNION_TYPES and issubclass(self.origin, cl)
         if self.annotation is AnyStr:
             return issubclass(str, cl) or issubclass(bytes, cl)
-        return self.annotation is not Any and issubclass(self.annotation, cl)
+        return self.annotation is not Any and not self.is_type_var and issubclass(self.annotation, cl)
 
     def has_inner_subclass_of(self, cl: type[Any] | tuple[type[Any], ...]) -> bool:
         """Whether any generic args are a subclass of the given type.
 
         Args:
             cl: The type to check, or tuple of types. Passed as 2nd argument to ``issubclass()``.
 
         Returns:
             Whether any of the type's generic args are a subclass of the given type.
         """
         return any(t.is_subclass_of(cl) for t in self.inner_types)
 
-    @classmethod
-    def from_annotation(cls, annotation: Any) -> ParsedType:
-        """Initialize ParsedType.
-
-        Args:
-            annotation: The type annotation. This should be extracted from the return of
-                ``get_type_hints(..., include_extras=True)`` so that forward references are resolved and recursive
-                ``Annotated`` types are flattened.
-
-        Returns:
-            ParsedType
-        """
-        unwrapped, metadata, wrappers = unwrap_annotation(annotation)
-
-        origin = get_origin(unwrapped)
-        args = get_args(unwrapped)
-        return ParsedType(
-            raw=annotation,
-            annotation=unwrapped,
-            origin=origin,
-            args=args,
-            metadata=metadata,
-            is_annotated=Annotated in wrappers,
-            is_required=Required in wrappers,
-            is_not_required=NotRequired in wrappers,
-            safe_generic_origin=get_safe_generic_origin(origin),
-            inner_types=tuple(cls.from_annotation(arg) for arg in args),
-        )
-
 
 @dataclass(frozen=True)
 class ParsedParameter:
     """Represents the parameters of a callable."""
 
     __slots__ = (
         "name",
@@ -242,15 +271,15 @@
                 "It must be typed to a subclass of `litestar.datastructures.ImmutableState` or "
                 "`litestar.datastructures.State`."
             )
 
         return ParsedParameter(
             name=parameter.name,
             default=Empty if parameter.default is Signature.empty else parameter.default,
-            parsed_type=ParsedType.from_annotation(annotation),
+            parsed_type=ParsedType(annotation),
         )
 
 
 @dataclass(frozen=True)
 class ParsedSignature:
     """Parsed signature.
 
@@ -265,30 +294,70 @@
     """A mapping of parameter names to ParsedSignatureParameter instances."""
     return_type: ParsedType
     """The return annotation of the callable."""
     original_signature: Signature
     """The raw signature as returned by :func:`inspect.signature`"""
 
     @classmethod
-    def from_fn(cls, fn: AnyCallable, signature_namespace: dict[str, Any]) -> ParsedSignature:
-        """Parse a function signature into data used for the generation of a signature model.
+    def from_fn(cls, fn: AnyCallable, signature_namespace: dict[str, Any]) -> Self:
+        """Parse a function signature.
 
         Args:
-            fn: A callable.
+            fn: Any callable.
             signature_namespace: mapping of names to types for forward reference resolution
 
         Returns:
             ParsedSignature
         """
         signature = Signature.from_callable(fn)
         fn_type_hints = get_fn_type_hints(fn, namespace=signature_namespace)
 
         parameters = (
             ParsedParameter.from_parameter(parameter=parameter, fn_type_hints=fn_type_hints)
             for name, parameter in signature.parameters.items()
             if name not in ("self", "cls")
         )
-        return ParsedSignature(
+        return cls(
             parameters={p.name: p for p in parameters},
-            return_type=ParsedType.from_annotation(fn_type_hints.get("return", Empty)),
+            return_type=ParsedType(fn_type_hints.get("return", Empty)),
             original_signature=signature,
         )
+
+    @classmethod
+    def from_signature(cls, signature: Signature, signature_namespace: dict[str, Any]) -> Self:
+        """Parse an :class:`inspect.Signature` instance.
+
+        Python's `get_type_hints()` function does not support parsing signatures directly, so we need to create a dummy
+        function to pass to it. Maybe there's a better way to do this, but this does work.
+
+        Args:
+            signature: An :class:`inspect.Signature` instance.
+            signature_namespace: mapping of names to types for forward reference resolution
+
+        Returns:
+            ParsedSignature
+        """
+
+        def fn() -> None:
+            ...
+
+        fn.__signature__ = signature  # type:ignore[attr-defined]
+        fn.__annotations__ = {p.name: p.annotation for p in signature.parameters.values()}
+        return cls.from_fn(fn, signature_namespace)
+
+
+def infer_request_encoding_from_parameter(param: ParsedParameter) -> RequestEncodingType | str:
+    """Infer the request encoding type from a parsed type.
+
+    Args:
+        param: The parsed parameter to infer the request encoding type from.
+
+    Returns:
+        The inferred request encoding type.
+    """
+    if param.has_default and isinstance(param.default, BodyKwarg):
+        return param.default.media_type
+    if param.parsed_type.metadata:
+        for item in param.parsed_type.metadata:
+            if isinstance(item, BodyKwarg):
+                return item.media_type
+    return RequestEncodingType.JSON
```

### Comparing `litestar-2.0.0a4/litestar/utils/sync.py` & `litestar-2.0.0a5/litestar/utils/sync.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/utils/typing.py` & `litestar-2.0.0a5/litestar/utils/typing.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/litestar/utils/version.py` & `litestar-2.0.0a5/litestar/utils/version.py`

 * *Files identical despite different names*

### Comparing `litestar-2.0.0a4/pyproject.toml` & `litestar-2.0.0a5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "litestar"
-version = "2.0.0alpha4"
+version = "2.0.0alpha5"
 description = "Performant, light and flexible ASGI API Framework"
 authors = [
     "Na'aman Hirschfeld <nhirschfeld@gmail.com>",
     "Peter Schutt <peter.github@proton.me>",
     "Cody Fincher <cody.fincher@gmail.com>",
     "Janek Nouvertné <provinzkraut@posteo.de>",
 ]
@@ -65,28 +65,30 @@
 jinja2 = { version = ">=3.1.2", optional = true }
 jsbeautifier = { version = "*", optional = true }
 mako = { version = ">=1.2.4", optional = true }
 msgspec = "*"
 multidict = ">=6.0.2"
 opentelemetry-instrumentation-asgi = { version = "*", optional = true }
 picologging = { version = "*", optional = true }
-polyfactory = {version = ">=2.0.0a1", allow-prereleases = true}
+polyfactory = ">=2"
 pydantic = "<2"
 python-dateutil = { version = "*", optional = true }
 python-jose = { version = "*", optional = true }
 pytimeparse = { version = "*", optional = true }
 pyyaml = "*"
 redis = { version = ">=4.4.4,!=4.5.0,!=4.5.1,!=4.5.2,!=4.5.3", optional = true, extras = ["hiredis"] }
 rich = { version = ">=13.0.0", optional = true }
 sqlalchemy = { version = ">=2.0.4", optional = true }
 structlog = { version = "*", optional = true }
 typing-extensions = "*"
+uvicorn = {extras = ["standard"], version = "^0.21.1", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 aiosqlite = "*"
+asyncmy = "*"
 asyncpg = "*"
 attrs = "*"
 beautifulsoup4 = "*"
 brotli = "*"
 cattrs = "*"
 click = "*"
 cryptography = "*"
@@ -145,44 +147,51 @@
 cryptography = ["cryptography"]
 jinja = ["jinja2"]
 jwt = ["python-jose", "cryptography"]
 opentelemetry = ["opentelemetry-instrumentation-asgi"]
 picologging = ["picologging"]
 redis = ["redis"]
 sqlalchemy = ["sqlalchemy", "alembic"]
-standard = ["click", "jinja2", "jsbeautifier", "rich"]
+standard = ["click", "jinja2", "jsbeautifier", "rich", "uvicorn"]
 structlog = ["structlog"]
 tortoise-orm = ["tortoise-orm"]
 
 full = [
+    "alembic",
+    "attrs",
     "brotli",
+    "cattrs",
     "click",
     "cryptography",
     "jinja2",
     "jsbeautifier",
     "opentelemetry-instrumentation-asgi",
-    "picologging",
+    "python-dateutill",
     "python-jose",
+    "pytimeparse",
     "redis",
     "rich",
+    "sqlalchemy",
     "structlog",
-    "tortoise-orm",
+    "uvicorn",
 ]
 
 [tool.poetry.scripts]
 litestar = { callable = "litestar:__main__", extras = ["cli"] }
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
 include = '\.pyi?$'
 
+[tool.codespell]
+ignore-words-list = "selectin"
 
 [tool.coverage.run]
 omit = ["*/tests/*", "litestar/contrib/sqlalchemy_1/*"]
 
 [tool.coverage.report]
 exclude_lines = [
     'pragma: no cover',
@@ -196,22 +205,27 @@
 [tool.pytest.ini_options]
 addopts = "--ignore=examples"
 asyncio_mode = "auto"
 filterwarnings = [
     "ignore::trio.TrioDeprecationWarning:anyio._backends._trio*:164",
     "ignore::DeprecationWarning:pkg_resources:2803",
 ]
+markers = [
+    "sqlalchemy_asyncmy: SQLAlchemy MySQL (asyncmy) Tests",
+    "sqlalchemy_asyncpg: SQLAlchemy Postgres (asyncpg) Tests"
+]
 
 [tool.pyright]
 include = ["litestar", "tests", "examples"]
 exclude = [
     "examples/plugins/sqlalchemy_plugin",
     "litestar/contrib/sqlalchemy_1",
     "litestar/openapi",
     "litestar/plugins",
+    "tests/contrib/sqlalchemy/test_dto.py",
     "tests/contrib/sqlalchemy_1",
     "tests/openapi",
     "tests/plugins",
 ]
 
 [tool.slotscheck]
 strict-imports = false
@@ -265,15 +279,14 @@
     "D105",  # pydocstyle - missing docstring in magic method
     "D106",  # pydocstyle - missing docstring in public nested class
     "D107",  # pydocstyle - missing docstring in __init__
     "D202",  # pydocstyle - no blank lines allowed after function docstring
     "D205",  # pydocstyle - 1 blank line required between summary line and description
     "D415",  # pydocstyle - first line should end with a period, question mark, or exclamation point
     "E501",  # pycodestyle line too long, handled by black
-    "UP037", # pyupgrade - removes quotes from type annotation
 ]
 line-length = 120
 src = ["litestar", "tests", "docs/examples"]
 target-version = "py38"
 
 [tool.ruff.pydocstyle]
 convention = "google"
@@ -343,10 +356,11 @@
     "TCH",
     "TRY",
 ]
 "docs/**/*.*" = ["S", "B", "DTZ", "A", "TCH", "ERA", "D", "RET"]
 "docs/examples/**" = ["T201"]
 "litestar/exceptions/*.*" = ["N818"]
 "litestar/handlers/**/*.*" = ["N801"]
+"litestar/_openapi/schema_generation/schema.py" = ["C901"]
 "litestar/params.py" = ["N802"]
 "test_apps/**/*.*" = ["D", "TRY", "EM", "S", "PTH"]
 "tools/**/*.*" = ["D", "ARG", "EM", "TRY", "G", "FBT"]
```

### Comparing `litestar-2.0.0a4/PKG-INFO` & `litestar-2.0.0a5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litestar
-Version: 2.0.0a4
+Version: 2.0.0a5
 Summary: Performant, light and flexible ASGI API Framework
 Home-page: https://litestar.dev/
 License: MIT
 Keywords: api,rest,http,asgi,pydantic,litestar,starlite,framework,websocket,litestar
 Author: Na'aman Hirschfeld
 Author-email: nhirschfeld@gmail.com
 Maintainer: Na'aman Hirschfeld
@@ -39,42 +39,43 @@
 Provides-Extra: opentelemetry
 Provides-Extra: picologging
 Provides-Extra: redis
 Provides-Extra: sqlalchemy
 Provides-Extra: standard
 Provides-Extra: structlog
 Provides-Extra: tortoise-orm
-Requires-Dist: alembic ; extra == "sqlalchemy"
+Requires-Dist: alembic ; extra == "sqlalchemy" or extra == "full"
 Requires-Dist: anyio (>=3)
-Requires-Dist: attrs ; extra == "attrs"
+Requires-Dist: attrs ; extra == "attrs" or extra == "full"
 Requires-Dist: brotli ; extra == "brotli" or extra == "full"
-Requires-Dist: cattrs ; extra == "attrs"
+Requires-Dist: cattrs ; extra == "attrs" or extra == "full"
 Requires-Dist: click ; extra == "cli" or extra == "standard" or extra == "full"
 Requires-Dist: cryptography ; extra == "cryptography" or extra == "jwt" or extra == "full"
 Requires-Dist: fast-query-parsers
 Requires-Dist: httpx (>=0.22)
 Requires-Dist: importlib-metadata ; python_version < "3.10"
 Requires-Dist: jinja2 (>=3.1.2) ; extra == "jinja" or extra == "standard" or extra == "full"
 Requires-Dist: jsbeautifier ; extra == "cli" or extra == "standard" or extra == "full"
 Requires-Dist: mako (>=1.2.4)
 Requires-Dist: msgspec
 Requires-Dist: multidict (>=6.0.2)
 Requires-Dist: opentelemetry-instrumentation-asgi ; extra == "opentelemetry" or extra == "full"
-Requires-Dist: picologging ; extra == "picologging" or extra == "full"
-Requires-Dist: polyfactory (>=2.0.0a1)
+Requires-Dist: picologging ; extra == "picologging"
+Requires-Dist: polyfactory (>=2)
 Requires-Dist: pydantic (<2)
 Requires-Dist: python-dateutil ; extra == "attrs"
 Requires-Dist: python-jose ; extra == "jwt" or extra == "full"
-Requires-Dist: pytimeparse ; extra == "attrs"
+Requires-Dist: pytimeparse ; extra == "attrs" or extra == "full"
 Requires-Dist: pyyaml
 Requires-Dist: redis[hiredis] (>=4.4.4,!=4.5.0,!=4.5.1,!=4.5.2,!=4.5.3) ; extra == "redis" or extra == "full"
 Requires-Dist: rich (>=13.0.0) ; extra == "cli" or extra == "standard" or extra == "full"
-Requires-Dist: sqlalchemy (>=2.0.4) ; extra == "sqlalchemy"
+Requires-Dist: sqlalchemy (>=2.0.4) ; extra == "sqlalchemy" or extra == "full"
 Requires-Dist: structlog ; extra == "structlog" or extra == "full"
 Requires-Dist: typing-extensions
+Requires-Dist: uvicorn[standard] (>=0.21.1,<0.22.0) ; extra == "cli" or extra == "standard" or extra == "full"
 Project-URL: Documentation, https://docs.litestar.dev/
 Project-URL: Repository, https://github.com/litestar-org/litestar
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable -->
 <p align="center">
   <img src="artwork/banner-light.svg#gh-light-mode-only" alt="Litestar Logo - Light" width="100%" height="auto" />
@@ -93,19 +94,19 @@
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)
 [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)
 [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)
 [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_litestar&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_litestar)
 
 <!-- prettier-ignore-start -->
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-95-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-97-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 <!-- prettier-ignore-end -->
 
-[![Reddit](https://img.shields.io/reddit/subreddit-subscribers/litestar?label=r%2FLitestar&logo=reddit)](https://reddit.com/r/litestar-api)
+[![Reddit](https://img.shields.io/reddit/subreddit-subscribers/litestarapi?label=r%2FLitestar&logo=reddit)](https://reddit.com/r/litestarapi)
 [![Discord](https://img.shields.io/discord/919193495116337154?color=blue&label=chat%20on%20discord&logo=discord)](https://discord.gg/X3FJqy8d2j)
 [![Matrix](https://img.shields.io/badge/%5Bm%5D%20chat%20on%20Matrix-bridged-blue)](https://matrix.to/#/#litestar:matrix.org)
 [![Medium](https://img.shields.io/badge/Medium-12100E?style=flat&logo=medium&logoColor=white)](https://blog.litestar.dev)
 
 </div>
 
 # Starlite → Litestar
@@ -431,15 +432,15 @@
       <td align="center" valign="top" width="14.28%"><a href="http://mookrs.com"><img src="https://avatars.githubusercontent.com/u/985439?v=4?s=100" width="100px;" alt="mookrs"/><br /><sub><b>mookrs</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=mookrs" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://mike.depalatis.net"><img src="https://avatars.githubusercontent.com/u/2805515?v=4?s=100" width="100px;" alt="Mike DePalatis"/><br /><sub><b>Mike DePalatis</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=mivade" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/pemocarlo"><img src="https://avatars.githubusercontent.com/u/7297323?v=4?s=100" width="100px;" alt="Carlos Alberto Pérez-Molano"/><br /><sub><b>Carlos Alberto Pérez-Molano</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=pemocarlo" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://www.bestcryptocodes.com"><img src="https://avatars.githubusercontent.com/u/114229148?v=4?s=100" width="100px;" alt="ThinksFast"/><br /><sub><b>ThinksFast</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=ThinksFast" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/litestar/commits?author=ThinksFast" title="Documentation">📖</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/ottermata"><img src="https://avatars.githubusercontent.com/u/9451844?v=4?s=100" width="100px;" alt="Christopher Krause"/><br /><sub><b>Christopher Krause</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=ottermata" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="http://www.kylesmith.me"><img src="https://avatars.githubusercontent.com/u/1161424?v=4?s=100" width="100px;" alt="Kyle Smith"/><br /><sub><b>Kyle Smith</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=smithk86" title="Code">💻</a> <a href="https://github.com/litestar-org/litestar/commits?author=smithk86" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="http://www.kylesmith.me"><img src="https://avatars.githubusercontent.com/u/1161424?v=4?s=100" width="100px;" alt="Kyle Smith"/><br /><sub><b>Kyle Smith</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=smithk86" title="Code">💻</a> <a href="https://github.com/litestar-org/litestar/commits?author=smithk86" title="Documentation">📖</a> <a href="https://github.com/litestar-org/litestar/issues?q=author%3Asmithk86" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/scott2b"><img src="https://avatars.githubusercontent.com/u/307713?v=4?s=100" width="100px;" alt="Scott Bradley"/><br /><sub><b>Scott Bradley</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/issues?q=author%3Ascott2b" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://www.linkedin.com/in/srikanthccv/"><img src="https://avatars.githubusercontent.com/u/22846633?v=4?s=100" width="100px;" alt="Srikanth Chekuri"/><br /><sub><b>Srikanth Chekuri</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=srikanthccv" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/litestar/commits?author=srikanthccv" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://lonelyviking.com"><img src="https://avatars.githubusercontent.com/u/78952809?v=4?s=100" width="100px;" alt="Michael Bosch"/><br /><sub><b>Michael Bosch</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=LonelyVikingMichael" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/sssssss340"><img src="https://avatars.githubusercontent.com/u/8406195?v=4?s=100" width="100px;" alt="sssssss340"/><br /><sub><b>sssssss340</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/issues?q=author%3Asssssss340" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/ste-pool"><img src="https://avatars.githubusercontent.com/u/17198460?v=4?s=100" width="100px;" alt="ste-pool"/><br /><sub><b>ste-pool</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=ste-pool" title="Code">💻</a> <a href="#infra-ste-pool" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a></td>
     </tr>
     <tr>
@@ -475,18 +476,20 @@
       <td align="center" valign="top" width="14.28%"><a href="https://gh.arielle.codes"><img src="https://avatars.githubusercontent.com/u/71233171?v=4?s=100" width="100px;" alt="arl"/><br /><sub><b>arl</b></sub></a><br /><a href="#maintenance-onerandomusername" title="Maintenance">🚧</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Galdanwing"><img src="https://avatars.githubusercontent.com/u/29492757?v=4?s=100" width="100px;" alt="Antoine van der Horst"/><br /><sub><b>Antoine van der Horst</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=Galdanwing" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://nick.groenen.me"><img src="https://avatars.githubusercontent.com/u/145285?v=4?s=100" width="100px;" alt="Nick Groenen"/><br /><sub><b>Nick Groenen</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=zoni" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/giorgiovilardo"><img src="https://avatars.githubusercontent.com/u/56472600?v=4?s=100" width="100px;" alt="Giorgio Vilardo"/><br /><sub><b>Giorgio Vilardo</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=giorgiovilardo" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/bollwyvl"><img src="https://avatars.githubusercontent.com/u/45380?v=4?s=100" width="100px;" alt="Nicholas Bollweg"/><br /><sub><b>Nicholas Bollweg</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=bollwyvl" title="Code">💻</a></td>
     </tr>
     <tr>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/tompin82"><img src="https://avatars.githubusercontent.com/u/47041409?v=4?s=100" width="100px;" alt="Tomas Jonsson"/><br /><sub><b>Tomas Jonsson</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=tompin82" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/tompin82"><img src="https://avatars.githubusercontent.com/u/47041409?v=4?s=100" width="100px;" alt="Tomas Jonsson"/><br /><sub><b>Tomas Jonsson</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=tompin82" title="Tests">⚠️</a> <a href="https://github.com/litestar-org/litestar/commits?author=tompin82" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://www.linkedin.com/in/khiem-doan/"><img src="https://avatars.githubusercontent.com/u/15646249?v=4?s=100" width="100px;" alt="Khiem Doan"/><br /><sub><b>Khiem Doan</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=khiemdoan" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/kedod"><img src="https://avatars.githubusercontent.com/u/35638715?v=4?s=100" width="100px;" alt="kedod"/><br /><sub><b>kedod</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=kedod" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/sonpro1296"><img src="https://avatars.githubusercontent.com/u/17319142?v=4?s=100" width="100px;" alt="sonpro1296"/><br /><sub><b>sonpro1296</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=sonpro1296" title="Code">💻</a> <a href="https://github.com/litestar-org/litestar/commits?author=sonpro1296" title="Tests">⚠️</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://patrickarmengol.com"><img src="https://avatars.githubusercontent.com/u/42473149?v=4?s=100" width="100px;" alt="Patrick Armengol"/><br /><sub><b>Patrick Armengol</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=patrickarmengol" title="Documentation">📖</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://sanderwegter.nl"><img src="https://avatars.githubusercontent.com/u/7465799?v=4?s=100" width="100px;" alt="Sander"/><br /><sub><b>Sander</b></sub></a><br /><a href="https://github.com/litestar-org/litestar/commits?author=SanderWegter" title="Documentation">📖</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

