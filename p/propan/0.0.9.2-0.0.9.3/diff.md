# Comparing `tmp/propan-0.0.9.2.tar.gz` & `tmp/propan-0.0.9.3.tar.gz`

## Comparing `propan-0.0.9.2.tar` & `propan-0.0.9.3.tar`

### file list

```diff
@@ -1,77 +1,87 @@
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 propan-0.0.9.2/CONTRIBUTING.md
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.0.9.2/SECURITY.md
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.0.9.2/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 propan-0.0.9.2/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.0.9.2/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 propan-0.0.9.2/.github/workflows/tests.yml
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/1_basic_usage.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/2_specific_exchange.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/3_lifespan_events.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/4_cli_attributes_promotion.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/5_publishing.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/6_arguments_casting.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/7_handler_errors_processing.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/dependencies/1_dependency_injection.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/dependencies/2_dependency_declaration.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/dependencies/3_dependency_aliases.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/dependencies/4_dependency_deep_aliases.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/dependencies/5_dependency_nesting.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/dependencies/6_dependecy_calling.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/dependencies/7_annotated.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/http_frameworks_integrations/aiohttp.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/http_frameworks_integrations/blacksheep.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/http_frameworks_integrations/falcon.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/http_frameworks_integrations/fastapi.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/http_frameworks_integrations/quart.py
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/http_frameworks_integrations/sanic.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 propan-0.0.9.2/examples/http_frameworks_integrations/tornado.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/__about__.py
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/__main__.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/annotations.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/brokers/__init__.py
--rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/brokers/push_back_watcher.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/brokers/model/__init__.py
--rw-r--r--   0        0        0     5915 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/brokers/model/broker_usecase.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/brokers/model/schemas.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/brokers/nats/__init__.py
--rw-r--r--   0        0        0     4847 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/brokers/nats/nats_broker.py
--rw-r--r--   0        0        0     5155 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/brokers/nats/nats_broker.pyi
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/brokers/nats/nats_js_broker.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/brokers/nats/schemas.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/brokers/rabbit/__init__.py
--rw-r--r--   0        0        0     8922 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/brokers/rabbit/rabbit_broker.py
--rw-r--r--   0        0        0     5835 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/brokers/rabbit/rabbit_broker.pyi
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/brokers/rabbit/schemas.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/cli/__init__.py
--rw-r--r--   0        0        0     3357 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/cli/app.py
--rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/cli/main.py
--rw-r--r--   0        0        0     5897 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/cli/startproject.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/cli/supervisors/__init__.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/cli/supervisors/basereload.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/cli/supervisors/multiprocess.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/cli/supervisors/utils.py
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/cli/supervisors/watchfiles.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/cli/utils/__init__.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/cli/utils/imports.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/cli/utils/logs.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/cli/utils/parser.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/log/__init__.py
--rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/log/formatter.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/log/logging.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/utils/__init__.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/utils/classes.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/utils/functions.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/utils/context/__init__.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/utils/context/main.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 propan-0.0.9.2/propan/utils/context/types.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.0.9.2/scripts/lint.sh
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.0.9.2/scripts/publish.sh
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.0.9.2/scripts/test-cov.sh
--rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.0.9.2/scripts/test.sh
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 propan-0.0.9.2/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.0.9.2/LICENSE
--rw-r--r--   0        0        0    10123 2020-02-02 00:00:00.000000 propan-0.0.9.2/README.md
--rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 propan-0.0.9.2/pyproject.toml
--rw-r--r--   0        0        0    13341 2020-02-02 00:00:00.000000 propan-0.0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 propan-0.0.9.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 propan-0.0.9.3/SECURITY.md
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.0.9.3/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 propan-0.0.9.3/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 propan-0.0.9.3/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 propan-0.0.9.3/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/1_basic_usage.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/2_specific_exchange.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/3_lifespan_events.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/4_cli_attributes_promotion.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/5_publishing.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/6_arguments_casting.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/7_handler_errors_processing.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/8_rpc_over_mq.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/9_noblocking_callbacks.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/dependencies/1_dependency_injection.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/dependencies/2_dependency_declaration.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/dependencies/3_dependency_aliases.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/dependencies/4_dependency_deep_aliases.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/dependencies/5_dependency_nesting.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/dependencies/6_dependecy_calling.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/dependencies/7_annotated.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/http_frameworks_integrations/aiohttp.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/http_frameworks_integrations/blacksheep.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/http_frameworks_integrations/falcon.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/http_frameworks_integrations/fastapi.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/http_frameworks_integrations/native_fastapi.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/http_frameworks_integrations/quart.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/http_frameworks_integrations/sanic.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 propan-0.0.9.3/examples/http_frameworks_integrations/tornado.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/__about__.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/__main__.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/annotations.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/brokers/__init__.py
+-rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/brokers/push_back_watcher.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/brokers/model/__init__.py
+-rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/brokers/model/broker_usecase.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/brokers/model/schemas.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/brokers/nats/__init__.py
+-rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/brokers/nats/nats_broker.py
+-rw-r--r--   0        0        0     5216 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/brokers/nats/nats_broker.pyi
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/brokers/nats/nats_js_broker.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/brokers/nats/schemas.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/brokers/rabbit/__init__.py
+-rw-r--r--   0        0        0    10843 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/brokers/rabbit/rabbit_broker.py
+-rw-r--r--   0        0        0     6795 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/brokers/rabbit/rabbit_broker.pyi
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/brokers/rabbit/schemas.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/cli/__init__.py
+-rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/cli/app.py
+-rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/cli/main.py
+-rw-r--r--   0        0        0     5928 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/cli/startproject.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/cli/supervisors/__init__.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/cli/supervisors/basereload.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/cli/supervisors/multiprocess.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/cli/supervisors/utils.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/cli/supervisors/watchfiles.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/cli/utils/__init__.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/cli/utils/imports.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/cli/utils/logs.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/cli/utils/parser.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/fastapi/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/fastapi/core/__init__.py
+-rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/fastapi/core/route.py
+-rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/fastapi/core/router.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/fastapi/rabbit/__init__.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/fastapi/rabbit/rabbit_router.py
+-rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/fastapi/rabbit/rabbit_router.pyi
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/log/__init__.py
+-rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/log/formatter.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/log/logging.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/utils/__init__.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/utils/classes.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/utils/functions.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/utils/context/__init__.py
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/utils/context/main.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 propan-0.0.9.3/propan/utils/context/types.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 propan-0.0.9.3/scripts/lint.sh
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 propan-0.0.9.3/scripts/publish.sh
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 propan-0.0.9.3/scripts/test-cov.sh
+-rwxr-xr-x   0        0        0       27 2020-02-02 00:00:00.000000 propan-0.0.9.3/scripts/test.sh
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 propan-0.0.9.3/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 propan-0.0.9.3/LICENSE
+-rw-r--r--   0        0        0    10913 2020-02-02 00:00:00.000000 propan-0.0.9.3/README.md
+-rw-r--r--   0        0        0     4995 2020-02-02 00:00:00.000000 propan-0.0.9.3/pyproject.toml
+-rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 propan-0.0.9.3/PKG-INFO
```

### Comparing `propan-0.0.9.2/CONTRIBUTING.md` & `propan-0.0.9.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.2/SECURITY.md` & `propan-0.0.9.3/SECURITY.md`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.2/.github/workflows/documentation.yml` & `propan-0.0.9.3/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.2/.github/workflows/publish_coverage.yml` & `propan-0.0.9.3/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.2/.github/workflows/publish_pypi.yml` & `propan-0.0.9.3/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.2/.github/workflows/tests.yml` & `propan-0.0.9.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.2/examples/3_lifespan_events.py` & `propan-0.0.9.3/examples/3_lifespan_events.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.2/examples/4_cli_attributes_promotion.py` & `propan-0.0.9.3/examples/4_cli_attributes_promotion.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,23 +11,24 @@
 ... env=.env
 "=" is required
 
 Or you can pass a boolean flags
 ... --use-smth  # passes as use_smth=True
 ... --no-use-smth  # passes as use_smth=False
 """
-from propan import Context, PropanApp, RabbitBroker
 from pydantic import BaseSettings
 
+from propan import Context, PropanApp, RabbitBroker
+
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
 app = PropanApp(broker)
 
 
 class Settings(BaseSettings):
     ...
 
 
 @app.on_startup
 async def setup_later(env: str, context: Context):
     settings = Settings(_env_file=env)
-    context.set_context("settings", settings)
+    context.set_global("settings", settings)
```

### Comparing `propan-0.0.9.2/examples/6_arguments_casting.py` & `propan-0.0.9.3/examples/6_arguments_casting.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 """
 Propan has @apply_types decorator to cast incoming function
 arguments to type according their type annotation.
 
 If you doesn't create broker as `RabbitBroker(apply_types=False)`,
 all broker handlers are wrapped by @apply_types by default.
 """
-from propan import PropanApp, RabbitBroker, apply_types
 from pydantic import BaseModel
 
+from propan import PropanApp, RabbitBroker, apply_types
+
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
 app = PropanApp(broker)
 
 
 class SimpleMessage(BaseModel):
     key: int
 
 
 @app.on_startup
 async def publish(broker: RabbitBroker):
-    await broker.publish_message("123", queue="test")
-    await broker.publish_message(SimpleMessage(key=123).dict(), queue="test2")
+    await broker.publish("123", queue="test")
+    await broker.publish(SimpleMessage(key=123).dict(), queue="test2")
 
 
 @broker.handle("test")
 async def base_handler(body: int):
     assert body == 123
     assert _nested_call(body)
```

### Comparing `propan-0.0.9.2/examples/7_handler_errors_processing.py` & `propan-0.0.9.3/examples/7_handler_errors_processing.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.2/examples/dependencies/1_dependency_injection.py` & `propan-0.0.9.3/examples/dependencies/1_dependency_injection.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,11 +20,11 @@
 async def base_handler(
     body: dict,
     app: App,
     broker: Rabbit,
     context: ContextRepo,
     logger: Logger,
     message: RabbitMessage,
-    not_found_field=Context(required=False),
+    not_found_field=Context(default=None),
 ):
     assert not_found_field is None
     assert broker is rabbit_broker
```

### Comparing `propan-0.0.9.2/examples/dependencies/2_dependency_declaration.py` & `propan-0.0.9.3/examples/dependencies/2_dependency_declaration.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,13 +10,13 @@
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
 app = PropanApp(broker)
 
 
 @app.on_startup
 def setup(context: ContextRepo):
-    context.set_context("my_dependency", True)
+    context.set_global("my_dependency", True)
 
 
 @broker.handle("test")
 async def base_handler(body: dict, my_dependency: bool = Context()):
     assert my_dependency is True
```

### Comparing `propan-0.0.9.2/examples/dependencies/4_dependency_deep_aliases.py` & `propan-0.0.9.3/examples/dependencies/4_dependency_deep_aliases.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Alias is able to provide access to specific attributes of dependency
 """
+from pydantic import BaseSettings, Field
+
 from propan import Context, PropanApp, RabbitBroker
 from propan.annotations import ContextRepo
-from pydantic import BaseSettings, Field
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
 app = PropanApp(broker)
 
 KEY = "my-secret-key"
 
@@ -15,13 +16,13 @@
 class Settings(BaseSettings):
     key: str = Field("")
 
 
 @app.on_startup
 async def setup(context: ContextRepo):
     settings = Settings(key=KEY)
-    context.set_context("settings", settings)
+    context.set_global("settings", settings)
 
 
 @app.on_startup
 def setup_later(key: str = Context("settings.key")):
     assert key is KEY
```

### Comparing `propan-0.0.9.2/examples/dependencies/5_dependency_nesting.py` & `propan-0.0.9.3/examples/dependencies/5_dependency_nesting.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.2/examples/dependencies/6_dependecy_calling.py` & `propan-0.0.9.3/examples/dependencies/6_dependecy_calling.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.2/examples/dependencies/7_annotated.py` & `propan-0.0.9.3/examples/dependencies/7_annotated.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 With Python 3.10+ you can use
 typing.Annotated class as a shortcut to Depends and Alias
 """
 import logging
 
-from propan import Context, Depends, PropanApp, RabbitBroker, apply_types
 from typing_extensions import Annotated
 
+from propan import Context, Depends, PropanApp, RabbitBroker, apply_types
+
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
 app = PropanApp(broker)
 
 Logger = Annotated[logging.Logger, Context("broker.logger")]
```

### Comparing `propan-0.0.9.2/examples/http_frameworks_integrations/aiohttp.py` & `propan-0.0.9.3/examples/http_frameworks_integrations/aiohttp.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 You can use Propan MQBrokers without PropanApp
 Just start and stop them whenever you want
 """
 from aiohttp import web
+
 from propan import RabbitBroker
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
 
 @broker.handle("test")
 async def base_handler(body):
```

### Comparing `propan-0.0.9.2/examples/http_frameworks_integrations/blacksheep.py` & `propan-0.0.9.3/examples/http_frameworks_integrations/blacksheep.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 You can use Propan MQBrokers without PropanApp
 Just start and stop them whenever you want
 """
 from blacksheep import Application
+
 from propan import RabbitBroker
 
 app = Application()
 
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
```

### Comparing `propan-0.0.9.2/examples/http_frameworks_integrations/falcon.py` & `propan-0.0.9.3/examples/http_frameworks_integrations/falcon.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 You can use Propan MQBrokers without PropanApp
 Just start and stop them whenever you want
 """
 import falcon
 import falcon.asgi
+
 from propan import RabbitBroker
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
 
 @broker.handle("test")
 async def base_handler(body):
```

### Comparing `propan-0.0.9.2/examples/http_frameworks_integrations/fastapi.py` & `propan-0.0.9.3/examples/http_frameworks_integrations/fastapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 You can use Propan MQBrokers without PropanApp
 Just start and stop them whenever you want
 """
 from contextlib import asynccontextmanager
 
 from fastapi import FastAPI
+
 from propan import RabbitBroker
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
 app = FastAPI()
```

### Comparing `propan-0.0.9.2/examples/http_frameworks_integrations/quart.py` & `propan-0.0.9.3/examples/http_frameworks_integrations/quart.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 You can use Propan MQBrokers without PropanApp
 Just start and stop them whenever you want
 """
-from propan import RabbitBroker
 from quart import Quart
 
+from propan import RabbitBroker
+
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
 app = Quart(__name__)
 
 
 @broker.handle("test")
 async def base_handler(body):
```

### Comparing `propan-0.0.9.2/examples/http_frameworks_integrations/sanic.py` & `propan-0.0.9.3/examples/http_frameworks_integrations/sanic.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 You can use Propan MQBrokers without PropanApp
 Just start and stop them whenever you want
 """
-from propan import RabbitBroker
 from sanic import Sanic
 from sanic.response import text
 
+from propan import RabbitBroker
+
 app = Sanic("MyHelloWorldApp")
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
 
 @broker.handle("test")
 async def base_handler(body):
     print(body)
```

### Comparing `propan-0.0.9.2/examples/http_frameworks_integrations/tornado.py` & `propan-0.0.9.3/examples/http_frameworks_integrations/tornado.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 You can use Propan MQBrokers without PropanApp
 Just start and stop them whenever you want
 """
 import asyncio
 
 import tornado.web
+
 from propan import RabbitBroker
 
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
 
 
 @broker.handle("test")
 async def base_handler(body):
```

### Comparing `propan-0.0.9.2/propan/__init__.py` & `propan-0.0.9.3/propan/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 from propan.cli.app import *  # noqa: F403
 from propan.log import *  # noqa: F403
 from propan.utils import *  # noqa: F403
 
 try:
     from propan.brokers.rabbit import RabbitBroker
 except Exception:
-    pass
+    RabbitBroker = None  # type: ignore
 
 try:
     from propan.brokers.nats import NatsBroker
 except Exception:
-    pass
+    NatsBroker = None  # type: ignore
 
 assert any((RabbitBroker, NatsBroker)), (
     "You should specify using broker!\n"
     "Install it using one of the following commands:\n"
     'pip install "propan[async-rabbit]"\n'
     'pip install "propan[async-nats]"\n'
 )
```

### Comparing `propan-0.0.9.2/propan/annotations.py` & `propan-0.0.9.3/propan/annotations.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 import logging
 
+from typing_extensions import Annotated
+
 from propan.cli.app import PropanApp
 from propan.utils.context import Context as ContextField
 from propan.utils.context import ContextRepo as CR
-from typing_extensions import Annotated
 
 Logger = Annotated[logging.Logger, ContextField("logger")]
 App = Annotated[PropanApp, ContextField("app")]
 ContextRepo = Annotated[CR, ContextField("context")]
 
-RabbitBroker = NatsBroker = RabbitMessage = NatsMessage = None
 
 try:
     import aio_pika
+
     from propan.brokers.rabbit import RabbitBroker as RB
 
     RabbitBroker = Annotated[RB, ContextField("broker")]
     RabbitMessage = Annotated[aio_pika.message.IncomingMessage, ContextField("message")]
 except Exception:
-    pass
+    RabbitBroker = RabbitMessage = None  # type: ignore
 
 try:
     from nats.aio.msg import Msg
+
     from propan.brokers.nats import NatsBroker as NB
 
     NatsBroker = Annotated[NB, ContextField("broker")]
     NatsMessage = Annotated[Msg, ContextField("message")]
 except Exception:
-    pass
+    NatsBroker = NatsMessage = None  # type: ignore
 
 assert any(
     (
         all((RabbitBroker, RabbitMessage)),
         all((NatsBroker, NatsMessage)),
     )
 ), (
```

### Comparing `propan-0.0.9.2/propan/brokers/push_back_watcher.py` & `propan-0.0.9.3/propan/brokers/push_back_watcher.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.2/propan/brokers/model/broker_usecase.py` & `propan-0.0.9.3/propan/brokers/model/broker_usecase.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 import logging
 from abc import ABC, abstractmethod
 from functools import wraps
 from time import perf_counter
-from typing import Any, Callable, Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 from propan.brokers.push_back_watcher import (
     BaseWatcher,
     FakePushBackWatcher,
     PushBackWatcher,
 )
 from propan.log import access_logger
-from propan.types import DecodedMessage, DecoratedCallable, Wrapper
-from propan.utils import apply_types
-from propan.utils.context import context
-from propan.utils.context import message as message_context
-from propan.utils.functions import call_or_await
+from propan.types import (
+    AnyCallable,
+    DecodedMessage,
+    DecoratedAsync,
+    DecoratedCallable,
+    Wrapper,
+)
+from propan.utils import apply_types, context
+from propan.utils.functions import to_async
 
 
 class BrokerUsecase(ABC):
     logger: Optional[logging.Logger]
     log_level: int
     handlers: List[Any]
     _connection: Any
@@ -28,42 +32,50 @@
         self,
         *args: Any,
         apply_types: bool = True,
         logger: Optional[logging.Logger] = access_logger,
         log_level: int = logging.INFO,
         log_fmt: str = "%(asctime)s %(levelname)s - %(message)s",
         **kwargs: Any,
-    ):
+    ) -> None:
         self.logger = logger
         self.log_level = log_level
         self._fmt = log_fmt
 
         self._connection = None
         self._is_apply_types = apply_types
         self.handlers = []
 
         self._connection_args = args
         self._connection_kwargs = kwargs
 
-        context.set_context("logger", logger)
-        context.set_context("broker", self)
+        context.set_global("logger", logger)
+        context.set_global("broker", self)
 
     async def connect(self, *args: Any, **kwargs: Any) -> Any:
         if self._connection is None:
             _args = args or self._connection_args
             _kwargs = kwargs or self._connection_kwargs
             self._connection = await self._connect(*_args, **_kwargs)
             return self._connection
 
     @abstractmethod
     async def _connect(self, *args: Any, **kwargs: Any) -> Any:
         raise NotImplementedError()
 
     @abstractmethod
-    async def publish_message(self, message: Any, *args: Any, **kwargs: Any) -> Any:
+    async def publish(
+        self,
+        message: Any,
+        *args: Any,
+        callback: bool = False,
+        callback_timeout: Optional[float] = None,
+        raise_timeout: bool = False,
+        **kwargs: Any,
+    ) -> Any:
         raise NotImplementedError()
 
     @abstractmethod
     async def close(self) -> None:
         raise NotImplementedError()
 
     @abstractmethod
@@ -86,92 +98,99 @@
 
     @abstractmethod
     def handle(
         self,
         *broker_args: Any,
         retry: Union[bool, int] = False,
         **broker_kwargs: Any,
-    ) -> Callable[[DecoratedCallable], None]:
+    ) -> Wrapper:
         raise NotImplementedError()
 
     @property
     def fmt(self) -> str:
         return self._fmt
 
     def _init_logger(self, logger: logging.Logger) -> None:
         for handler in logger.handlers:
             formatter = handler.formatter
             if formatter is not None:
-                if getattr(formatter, "use_colors", None) is not None:
-                    kwargs = {"use_colors": formatter.use_colors}
+                use_colors = getattr(formatter, "use_colors", None)
+                if use_colors is not None:
+                    kwargs = {"use_colors": use_colors}
                 else:
                     kwargs = {}
                 handler.setFormatter(type(formatter)(self.fmt, **kwargs))
 
     async def __aenter__(self) -> "BrokerUsecase":
         await self.connect()
         return self
 
     async def __aexit__(self, *args: Any, **kwargs: Any) -> None:
         await self.close()
 
     def _wrap_handler(
-        self, func: DecoratedCallable, retry: Union[bool, int], **broker_args: Any
-    ) -> DecoratedCallable:
+        self, func: AnyCallable, retry: Union[bool, int], **broker_args: Any
+    ) -> DecoratedAsync:
+        func = to_async(func)
+
         if self._is_apply_types is True:
             func = apply_types(func)
 
         if self.logger is not None:
             func = self._log_execution(self.logger, **broker_args)(func)
 
         func = self._wrap_decode_message(func)
 
         func = self._process_message(func, _get_watcher(self.logger, retry))
 
         func = _set_message_context(func)
 
+        func = suppress(func)
+
         return func
 
-    def _wrap_decode_message(self, func: DecoratedCallable) -> Wrapper:
+    def _wrap_decode_message(self, func: AnyCallable) -> DecoratedCallable:
         @wraps(func)
         async def wrapper(message: Any) -> Any:
             return await func(await self._decode_message(message))
 
         return wrapper
 
-    def _log_execution(
-        self, logger: logging.Logger, **broker_args: Any
-    ) -> Callable[[DecoratedCallable], Wrapper]:
-        def decor(func: DecoratedCallable) -> Wrapper:
+    def _log_execution(self, logger: logging.Logger, **broker_args: Any) -> Wrapper:
+        def decor(func: AnyCallable) -> DecoratedCallable:
             @wraps(func)
             async def wrapper(*args: Any, **kwargs: Any) -> Any:
-                message = message_context.get()
+                message = context.get("message")
 
                 start = perf_counter()
 
-                self._get_log_context(message=message, **broker_args)
-                logger.log(self.log_level, "Received")
+                log_context = self._get_log_context(message=message, **broker_args)
 
-                try:
-                    r = await call_or_await(func, *args, **kwargs)
-                except Exception as e:
-                    logger.error(repr(e))
-                else:
-                    logger.log(
-                        self.log_level, f"Processed by {(perf_counter() - start):.4f}"
-                    )
-                    return r
+                with context.scope("log_context", log_context):
+                    logger.log(self.log_level, "Received")
+
+                    try:
+                        r = await func(*args, **kwargs)
+                    except Exception as e:
+                        logger.error(repr(e))
+                        raise e
+                    else:
+                        logger.log(
+                            self.log_level,
+                            f"Processed by {(perf_counter() - start):.4f}",
+                        )
+                        return r
 
             return wrapper
 
         return decor
 
     def _log(self, message: str, log_level: Optional[int] = None) -> None:
         if self.logger is not None:
-            self.logger.log(message, log_level or self.log_level)
+            self.logger.log(level=(log_level or self.log_level), msg=message)
 
 
 def _get_watcher(
     logger: Optional[logging.Logger], try_number: Union[bool, int] = True
 ) -> Optional[BaseWatcher]:
     watcher: Optional[BaseWatcher]
     if try_number is True:
@@ -179,14 +198,25 @@
     elif try_number is False:
         watcher = None
     else:
         watcher = PushBackWatcher(logger=logger, max_tries=try_number)
     return watcher
 
 
-def _set_message_context(func: DecoratedCallable) -> Wrapper:
+def _set_message_context(func: AnyCallable) -> DecoratedCallable:
+    @wraps(func)
+    async def wrapper(message: Any) -> Any:
+        with context.scope("message", message):
+            return await func(message)
+
+    return wrapper
+
+
+def suppress(func: AnyCallable) -> DecoratedCallable:
     @wraps(func)
     async def wrapper(message: Any) -> Any:
-        message_context.set(message)
-        return await func(message)
+        try:
+            return await func(message)
+        except Exception:
+            pass
 
     return wrapper
```

### Comparing `propan-0.0.9.2/propan/brokers/model/schemas.py` & `propan-0.0.9.3/propan/brokers/model/schemas.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.2/propan/brokers/nats/nats_broker.py` & `propan-0.0.9.3/propan/brokers/nats/nats_broker.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 from functools import wraps
 from typing import Any, Callable, Dict, List, Optional, Union
 from uuid import uuid4
 
 import nats
 from nats.aio.client import Client
 from nats.aio.msg import Msg
+
 from propan.brokers.model import BrokerUsecase, ContentTypes
 from propan.brokers.nats.schemas import Handler
 from propan.brokers.push_back_watcher import BaseWatcher
-from propan.types import DecoratedCallable
-from propan.utils.context.main import log_context
+from propan.types import AnyDict, DecoratedCallable
 
 
 class NatsBroker(BrokerUsecase):
     handlers: List[Handler]
     _connection: Optional[Client]
 
     __max_queue_len: int
     __max_subject_len: int
 
-    def __init__(self, *args: Any, log_fmt: Optional[str] = None, **kwargs: Any):
+    def __init__(self, *args: Any, log_fmt: Optional[str] = None, **kwargs: AnyDict):
         super().__init__(*args, log_fmt=log_fmt, **kwargs)
 
         self._connection = None
 
         self.__max_queue_len = 0
         self.__max_subject_len = 4
 
@@ -53,14 +53,16 @@
                         f"`{queue}` queue"
                     )
 
             func = parent._wrap_handler(func, retry, queue=queue, subject=subject)
             handler = Handler(callback=func, subject=subject, queue=queue)
             self.handlers.append(handler)
 
+            return func
+
         return wrapper
 
     async def start(self) -> None:
         await super().start()
 
         for handler in self.handlers:
             func = handler.callback
@@ -68,15 +70,15 @@
             if self.logger:
                 self._get_log_context(None, handler.subject, handler.queue)
                 self.logger.info(f"`{func.__name__}` waiting for messages")
 
             sub = await self._connection.subscribe(handler.subject, cb=func)
             handler.subscription = sub
 
-    async def publish_message(
+    async def publish(
         self, message: Union[str, Dict[str, Any]], subject: str, **publish_args: Any
     ) -> None:
         if self._connection is None:
             raise ValueError("NatsConnection not started yet")
 
         if isinstance(message, dict):
             message = json.dumps(message)
@@ -110,15 +112,14 @@
 
         context = {
             "subject": subject,
             "queue": queue,
             "message_id": message.message_id[:10] if message else "",
         }
 
-        log_context.set(context)
         return context
 
     @property
     def fmt(self) -> str:
         return self._fmt or (
             "%(asctime)s %(levelname)s - "
             f"%(subject)-{self.__max_subject_len}s | "
```

### Comparing `propan-0.0.9.2/propan/brokers/nats/nats_broker.pyi` & `propan-0.0.9.3/propan/brokers/nats/nats_broker.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 import ssl
-from typing import Any, Callable, Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 from nats.aio.client import (
     DEFAULT_CONNECT_TIMEOUT,
     DEFAULT_DRAIN_TIMEOUT,
     DEFAULT_INBOX_PREFIX,
     DEFAULT_MAX_FLUSHER_QUEUE_SIZE,
     DEFAULT_MAX_OUTSTANDING_PINGS,
@@ -16,19 +16,20 @@
     Client,
     Credentials,
     ErrorCallback,
     JWTCallback,
     SignatureCallback,
 )
 from nats.aio.msg import Msg
+
 from propan.brokers.model import BrokerUsecase
 from propan.brokers.nats.schemas import Handler
 from propan.brokers.push_back_watcher import BaseWatcher
 from propan.log import access_logger
-from propan.types import DecoratedCallable
+from propan.types import AnyDict, DecodedMessage, DecoratedCallable, Wrapper
 
 class NatsBroker(BrokerUsecase):
     logger: logging.Logger
     handlers: List[Handler] = []
     _connection: Optional[Client] = None
 
     def __init__(
@@ -100,29 +101,29 @@
         user_jwt_cb: Optional[JWTCallback] = None,
         user_credentials: Optional[Credentials] = None,
         nkeys_seed: Optional[str] = None,
         inbox_prefix: Union[str, bytes] = DEFAULT_INBOX_PREFIX,
         pending_size: int = DEFAULT_PENDING_SIZE,
         flush_timeout: Optional[float] = None,
     ) -> Client: ...
-    async def publish_message(
+    async def publish(  # type: ignore[override]
         self,
         message: Union[str, Dict[str, Any]],
         subject: str,
         reply: str = "",
         headers: Optional[Dict[str, str]] = None,
     ) -> None: ...
-    def handle(
+    def handle(  # type: ignore[override]
         self, subject: str, queue: str = "", *, retry: Union[bool, int] = False
-    ) -> Callable[[DecoratedCallable], None]: ...
+    ) -> Wrapper: ...
     async def __aenter__(self) -> "NatsBroker": ...
     async def _connect(self, *args: Any, **kwargs: Any) -> Client: ...
     async def close(self) -> None: ...
-    def _get_log_context(
-        self, message: Optional[Msg], subject: str, queue: str = "", **kwargs
+    def _get_log_context(  # type: ignore[override]
+        self, message: Optional[Msg], subject: str, queue: str = "", **kwargs: AnyDict
     ) -> Dict[str, Any]: ...
     @staticmethod
-    async def _decode_message(message: Msg) -> Union[str, dict]: ...
+    async def _decode_message(message: Msg) -> DecodedMessage: ...
     @staticmethod
     def _process_message(
         func: DecoratedCallable, watcher: Optional[BaseWatcher] = None
-    ) -> Callable[[Msg], Any]: ...
+    ) -> Wrapper: ...
```

### Comparing `propan-0.0.9.2/propan/brokers/nats/schemas.py` & `propan-0.0.9.3/propan/brokers/nats/schemas.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from dataclasses import dataclass
 from typing import Optional, Sequence
 
 from nats.aio.subscription import Subscription
 from nats.js.api import DEFAULT_PREFIX
-from propan.types import DecoratedCallable
 from pydantic import BaseModel
 
+from propan.types import DecoratedCallable
+
 
 @dataclass
 class Handler:
     callback: DecoratedCallable
     subject: str
     queue: str = ""
```

### Comparing `propan-0.0.9.2/propan/brokers/rabbit/rabbit_broker.pyi` & `propan-0.0.9.3/propan/brokers/rabbit/rabbit_broker.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 import logging
 from ssl import SSLContext
 from typing import Any, Dict, List, Optional, Union
 
 import aio_pika
 import aiormq
 from pamqp.common import FieldTable
+from pydantic import BaseModel
+from yarl import URL
+
 from propan.brokers.model import BrokerUsecase
 from propan.brokers.push_back_watcher import BaseWatcher
 from propan.brokers.rabbit.schemas import Handler, RabbitExchange, RabbitQueue
 from propan.log import access_logger
-from propan.types import DecodedMessage, DecoratedCallable, Wrapper
-from yarl import URL
+from propan.types import AnyDict, DecodedMessage, DecoratedCallable, Wrapper
 
 class RabbitBroker(BrokerUsecase):
     handlers: List[Handler]
     _connection: Optional[aio_pika.RobustConnection]
     _channel: Optional[aio_pika.RobustChannel]
 
     __max_queue_len: int
     __max_exchange_len: int
 
-    async def __init__(
+    def __init__(
         self,
         url: Union[str, URL, None] = None,
         host: str = "localhost",
         port: int = 5672,
         login: str = "guest",
         password: str = "guest",
         virtualhost: str = "/",
@@ -35,15 +37,15 @@
         client_properties: Optional[FieldTable] = None,
         *,
         logger: Optional[logging.Logger] = access_logger,
         log_level: int = logging.INFO,
         log_fmt: Optional[str] = None,
         apply_types: bool = True,
         consumers: Optional[int] = None,
-    ):
+    ) -> None:
         """
         URL string might be contain ssl parameters e.g.
         `amqps://user:pass@host//?ca_certs=ca.pem&certfile=crt.pem&keyfile=key.pem`
 
         :param client_properties: add custom client capability.
         :param url:
             RFC3986_ formatted broker address. When :class:`None`
@@ -94,26 +96,45 @@
         :param timeout: connection timeout in seconds
         :param ssl_context: ssl.SSLContext instance
 
         .. _RFC3986: https://goo.gl/MzgYAs
         .. _official Python documentation: https://goo.gl/pty9xA
         """
         ...
-    async def publish_message(
+    async def publish(  # type: ignore[override]
         self,
-        message: Union[aio_pika.Message, str, Dict[str, Any]],
+        message: Union[aio_pika.Message, str, Dict[str, Any], BaseModel] = "",
         queue: Union[RabbitQueue, str] = "",
         exchange: Union[RabbitExchange, str, None] = None,
         *,
+        # publish kwargs
         routing_key: str = "",
         mandatory: bool = True,
         immediate: bool = False,
         timeout: aio_pika.abc.TimeoutType = None,
+        # callback kwargs
+        callback: bool = False,
+        callback_timeout: Optional[float] = 30.0,
+        raise_timeout: bool = False,
+        # message kwargs
+        headers: Optional[aio_pika.abc.HeadersType] = None,
+        content_type: Optional[str] = None,
+        content_encoding: Optional[str] = None,
+        delivery_mode: Union[aio_pika.abc.DeliveryMode, int, None] = None,
+        priority: Optional[int] = None,
+        correlation_id: Optional[str] = None,
+        reply_to: Optional[str] = None,
+        expiration: Optional[aio_pika.abc.DateType] = None,
+        message_id: Optional[str] = None,
+        timestamp: Optional[aio_pika.abc.DateType] = None,
+        type: Optional[str] = None,
+        user_id: Optional[str] = None,
+        app_id: Optional[str] = None,
     ) -> Optional[aiormq.abc.ConfirmationFrameType]: ...
-    def handle(
+    def handle(  # type: ignore[override]
         self,
         queue: Union[str, RabbitQueue],
         exchange: Union[str, RabbitExchange, None] = None,
         *,
         retry: Union[bool, int] = False,
     ) -> Wrapper:
         """
@@ -127,20 +148,20 @@
     async def _decode_message(
         message: aio_pika.IncomingMessage,
     ) -> DecodedMessage: ...
     @staticmethod
     def _process_message(
         func: DecoratedCallable, watcher: Optional[BaseWatcher] = None
     ) -> DecoratedCallable: ...
-    def _get_log_context(
+    def _get_log_context(  # type: ignore[override]
         self,
         message: Optional[aio_pika.Message],
         queue: RabbitQueue,
         exchange: Optional[RabbitExchange] = None,
-        **kwrags,
+        **kwrags: AnyDict,
     ) -> Dict[str, Any]: ...
     async def _init_channel(self, max_consumers: Optional[int] = None) -> None: ...
     async def _init_handler(
         self, handler: Handler
     ) -> aio_pika.abc.AbstractRobustQueue: ...
     async def _init_queue(
         self, queue: RabbitQueue
```

### Comparing `propan-0.0.9.2/propan/brokers/rabbit/schemas.py` & `propan-0.0.9.3/propan/brokers/rabbit/schemas.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Any, Dict, Optional, Union
 
 from aio_pika.abc import ExchangeType, TimeoutType
+from pydantic import BaseModel, Field
+
 from propan.brokers.model.schemas import NameRequired, Queue
 from propan.types import DecoratedCallable
-from pydantic import BaseModel, Field
 
 __all__ = (
     "RabbitQueue",
     "RabbitExchange",
     "Handler",
     "ExchangeType",
 )
```

### Comparing `propan-0.0.9.2/propan/cli/app.py` & `propan-0.0.9.3/propan/cli/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,74 +1,78 @@
 import asyncio
 import logging
-from ctypes import Union
 from typing import Dict, List, Optional
 
 from anyio import create_memory_object_stream, create_task_group
 from anyio.streams.memory import MemoryObjectReceiveStream, MemoryObjectSendStream
+
 from propan.brokers.model.broker_usecase import BrokerUsecase
 from propan.cli.supervisors.utils import set_exit
+from propan.cli.utils.parser import SettingField
 from propan.log import logger
-from propan.types import DecoratedCallableNone
+from propan.types import AsyncFunc, DecoratedCallableNone, NoneCallable
 from propan.utils import apply_types, context
 from propan.utils.functions import to_async
 
 
 class PropanApp:
-    _on_startup_calling: List[DecoratedCallableNone]
-    _on_shutdown_calling: List[DecoratedCallableNone]
+    _on_startup_calling: List[AsyncFunc]
+    _on_shutdown_calling: List[AsyncFunc]
 
-    _stop_stream: Optional[MemoryObjectSendStream]
-    _receive_stream: Optional[MemoryObjectReceiveStream]
+    _stop_stream: Optional[MemoryObjectSendStream[bool]]
+    _receive_stream: Optional[MemoryObjectReceiveStream[bool]]
 
     def __init__(
         self,
         broker: Optional[BrokerUsecase] = None,
         logger: Optional[logging.Logger] = logger,
     ):
         self.broker = broker
         self.logger = logger
         self.context = context
-        context.set_context("app", self)
+        context.set_global("app", self)
 
         self._on_startup_calling = []
         self._on_shutdown_calling = []
         self._stop_stream = None
         self._receive_stream = None
-        self._command_line_options: Dict[str, Union[str, bool]] = {}
+        self._command_line_options: Dict[str, SettingField] = {}
 
     def set_broker(self, broker: BrokerUsecase) -> None:
         self.broker = broker
 
-    def on_startup(self, func: DecoratedCallableNone) -> DecoratedCallableNone:
-        self._on_startup_calling.append(apply_types(to_async(func)))
+    def on_startup(self, func: NoneCallable) -> DecoratedCallableNone:
+        f: AsyncFunc = apply_types(to_async(func))
+        self._on_startup_calling.append(f)
         return func
 
-    def on_shutdown(self, func: DecoratedCallableNone) -> DecoratedCallableNone:
-        self._on_shutdown_calling.append(apply_types(to_async(func)))
+    def on_shutdown(self, func: NoneCallable) -> DecoratedCallableNone:
+        f: AsyncFunc = apply_types(to_async(func))
+        self._on_shutdown_calling.append(f)
         return func
 
     async def run(self, log_level: int = logging.INFO) -> None:
         self._init_async_cycle()
         async with create_task_group() as tg:
-            set_exit(lambda *_: tg.start_soon(self._stop_stream.send, True))
+            set_exit(lambda *_: tg.start_soon(self.__exit, True))
             tg.start_soon(self._stop, log_level)
             tg.start_soon(self._start, log_level)
 
-    def _init_async_cycle(self):
+    def _init_async_cycle(self) -> None:
         self.loop = asyncio.get_event_loop()
         if not self._stop_stream and not self._receive_stream:
             self._stop_stream, self._receive_stream = create_memory_object_stream(1)
 
     async def _start(self, log_level: int = logging.INFO) -> None:
         self._log(log_level, "Propan app starting...")
         await self._startup()
         self._log(log_level, "Propan app started successfully! To exit press CTRL+C")
 
     async def _stop(self, log_level: int = logging.INFO) -> None:
+        assert self._receive_stream, "You should call `_init_async_cycle` first"
         await self._receive_stream.receive()
         self._log(log_level, "Propan app shutting down...")
         await self._shutdown()
         self._log(log_level, "Propan app shut down gracefully.")
 
     def _log(self, level: int, message: str) -> None:
         if self.logger is not None:
@@ -86,7 +90,11 @@
             self.broker is not None
             and getattr(self.broker, "_connection", False) is not False
         ):
             await self.broker.close()
 
         for func in self._on_shutdown_calling:
             await func()
+
+    async def __exit(self, flag: bool) -> None:
+        if self._stop_stream is not None:
+            await self._stop_stream.send(flag)
```

### Comparing `propan-0.0.9.2/propan/cli/main.py` & `propan-0.0.9.3/propan/cli/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import asyncio
 import logging
 import sys
 from pathlib import Path
-from typing import Dict, Optional, Union
+from typing import Dict, Optional
 
 import typer
+
 from propan.__about__ import __version__
 from propan.cli.app import PropanApp
 from propan.cli.utils.imports import get_app_path, import_object
 from propan.cli.utils.logs import LogLevels, set_log_level
-from propan.cli.utils.parser import parse_cli_args
+from propan.cli.utils.parser import SettingField, parse_cli_args
 from propan.log import logger
 
 cli = typer.Typer()
 
 
 def version_callback(version: bool) -> None:
     if version is True:
@@ -37,15 +38,15 @@
     version: Optional[bool] = typer.Option(
         False,
         "--version",
         callback=version_callback,
         is_eager=True,
         help="Show current platform, python and propan version",
     )
-):
+) -> None:
     """
     Generate, run and manage Propan apps to greater development experience
     """
 
 
 @cli.command()
 def create(appname: str) -> None:
@@ -96,21 +97,21 @@
 
     elif workers > 1:
         from propan.cli.supervisors.multiprocess import Multiprocess
 
         Multiprocess(target=_run, args=(*args, logging.DEBUG), workers=workers).run()
 
     else:
-        _run(*args)
+        _run(module=module, app=app, extra_options=extra)
 
 
 def _run(
     module: Path,
     app: str,
-    extra_options: Dict[str, Union[bool, str]],
+    extra_options: Dict[str, SettingField],
     log_level: int = logging.INFO,
 ) -> None:
     try:
         propan_app = import_object(module, app)
 
         if not isinstance(propan_app, PropanApp):
             raise ValueError(f"{propan_app} is not a PropanApp")
```

### Comparing `propan-0.0.9.2/propan/cli/startproject.py` & `propan-0.0.9.3/propan/cli/startproject.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from typing import Union
+from typing import Union, cast
 
 
 def create(project_dir: Path, version: str) -> Path:
     project_dir = _create_project_dir(project_dir, version)
     app_dir = _create_app_dir(project_dir / "app")
     _create_config_dir(app_dir / "config")
     _create_core_dir(app_dir / "core")
@@ -94,15 +94,15 @@
         "",
         "app = PropanApp(broker)",
         "",
         "",
         "@app.on_startup",
         "async def init_app(broker: RabbitBroker, env: Optional[str], context: Context):",
         "    settings = init_settings(env)",
-        '    context.set_context("settings", settings)',
+        '    context.set_global("settings", settings)',
         "",
         "    logger_level = logging.DEBUG if settings.debug else logging.INFO",
         "    app.logger.setLevel(logger_level)",
         "    broker.logger.setLevel(logger_level)",
         "",
         "    await broker.connect(url=settings.rabbit.url)",
         "",
@@ -209,14 +209,15 @@
     return apps_dir
 
 
 def _touch_dir(dir: Union[Path, str]) -> Path:
     if isinstance(dir, str) is True:
         dir = Path(dir).resolve()
 
+    dir = cast(Path, dir)
     if dir.exists() is False:
         dir.mkdir()
     return dir
 
 
 def _write_file(path: Path, *content: str) -> None:
     path.touch()
```

### Comparing `propan-0.0.9.2/propan/cli/supervisors/basereload.py` & `propan-0.0.9.3/propan/cli/supervisors/basereload.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.2/propan/cli/supervisors/multiprocess.py` & `propan-0.0.9.3/propan/cli/supervisors/multiprocess.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.2/propan/cli/supervisors/utils.py` & `propan-0.0.9.3/propan/cli/supervisors/utils.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.2/propan/cli/supervisors/watchfiles.py` & `propan-0.0.9.3/propan/cli/supervisors/watchfiles.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,45 @@
 from pathlib import Path
 from typing import Any, Optional, Sequence, Tuple, Union
 
 import watchfiles
+
 from propan.cli.supervisors.basereload import BaseReload
 from propan.log import logger
 from propan.types import DecoratedCallable
 
 
 class ExtendedFilter(watchfiles.PythonFilter):
+    ignore_dirs: Tuple[str, ...]
+
     def __init__(
         self,
         *,
         ignore_paths: Optional[Sequence[Union[str, Path]]] = None,
         extra_extensions: Sequence[str] = (),
     ) -> None:
         super().__init__(ignore_paths=ignore_paths, extra_extensions=extra_extensions)
         self.extensions = self.extensions + (".env", ".yaml")
-        self.ignore_dirs = self.ignore_dirs + ("venv", "env", ".ruff_cache", "htmlcov")
+        self.ignore_dirs = self.ignore_dirs + (
+            "venv",
+            "env",
+            ".github",
+            ".mypy_cache",
+            ".pytest_cache",
+            ".ruff_cache",
+        )
 
 
 class WatchReloader(BaseReload):
     def __init__(
         self,
         target: DecoratedCallable,
         args: Tuple[Any, ...],
         reload_dirs: Sequence[Union[Path, str]],
-        reload_delay: Optional[float] = 0.3,
+        reload_delay: float = 0.3,
     ) -> None:
         super().__init__(target, args, reload_delay)
         self.reloader_name = "WatchFiles"
         self.watcher = watchfiles.watch(
             *reload_dirs,
             step=int(reload_delay * 1000),
             watch_filter=ExtendedFilter(),
@@ -40,7 +50,8 @@
     def should_restart(self) -> bool:
         for changes in self.watcher:  # pragma: no branch
             if changes:  # pragma: no branch
                 unique_paths = {Path(c[1]).name for c in changes}
                 message = "WatchReloader detected file change in '%s'. Reloading..."
                 logger.info(message % tuple(unique_paths))
                 return True
+        return False  # pragma: no cover
```

### Comparing `propan-0.0.9.2/propan/cli/utils/imports.py` & `propan-0.0.9.3/propan/cli/utils/imports.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.2/propan/cli/utils/logs.py` & `propan-0.0.9.3/propan/cli/utils/logs.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.2/propan/log/formatter.py` & `propan-0.0.9.3/propan/log/formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import logging
 import sys
 from collections import defaultdict
 from typing import Callable, Optional
+from typing_extensions import Literal
 
 import click
-from propan.utils.context.main import log_context
+
+from propan.utils.context.main import context
 
 
 class ColourizedFormatter(logging.Formatter):
     level_name_colors: "defaultdict[str, Callable[[str], str]]" = defaultdict(
         lambda: str,
         **{
             str(logging.DEBUG): lambda level_name: click.style(
@@ -29,15 +31,15 @@
         },
     )
 
     def __init__(
         self,
         fmt: Optional[str] = None,
         datefmt: Optional[str] = None,
-        style: str = "%",
+        style: Literal["%", "{", "$"] = "%",
         use_colors: Optional[bool] = None,
     ):
         """
         Initialize the formatter with specified format strings.
 
         Initialize the formatter either with the specified format string, or a
         default as described above. Allow for specialized date formatting with
@@ -67,15 +69,15 @@
 
 class DefaultFormatter(ColourizedFormatter):
     pass
 
 
 class AccessFormatter(ColourizedFormatter):
     def formatMessage(self, record: logging.LogRecord) -> str:
-        context = log_context.get()
-        if context:  # pragma: no cover
-            record.__dict__.update(context)
+        c = context.get_local("log_context")
+        if c:  # pragma: no cover
+            record.__dict__.update(c)
         return super().formatMessage(record)
 
 
 def expand_log_field(field: str, symbols: int) -> str:
     return field + (" " * (symbols - len(field)))
```

### Comparing `propan-0.0.9.2/propan/log/logging.py` & `propan-0.0.9.3/propan/log/logging.py`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.2/propan/utils/context/types.py` & `propan-0.0.9.3/propan/utils/context/types.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,28 @@
+from inspect import _empty
 from typing import Any
 
 from fast_depends.library import CustomField
+
+from propan.types import AnyDict
 from propan.utils.context import context
 
 
 class Context(CustomField):
     def __init__(
-        self, real_name: str = "", *, cast: bool = False, required: bool = True
+        self, real_name: str = "", *, cast: bool = False, default: Any = _empty
     ):
         self.name = real_name
-        super().__init__(cast=cast, required=required)
+        self.default = default
+        super().__init__(cast=cast, required=(default is _empty))
 
-    def use(self, **kwargs):
+    def use(self, **kwargs: AnyDict) -> AnyDict:
         name = self.name or self.param_name
-        return {**kwargs, self.param_name: resolve_context(name)}
+        default = None if self.default is _empty else self.default
+        return {**kwargs, self.param_name: resolve_context(name) or default}
 
 
 def resolve_context(argument: str) -> Any:
     keys = argument.split(".")
 
     v = context.context.get(keys[0])
     for i in keys[1:]:
```

### Comparing `propan-0.0.9.2/LICENSE` & `propan-0.0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `propan-0.0.9.2/README.md` & `propan-0.0.9.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -35,27 +35,26 @@
 
 It is a modern, high-level framework on top of popular specific Python brokers libraries, based on [*pydantic*](https://docs.pydantic.dev/) and [*fastapi*](https://fastapi.tiangolo.com/ru/), [*pytest*](https://docs.pytest.org/en/7.3.x/) concepts.
 
 ---
 
 **Documentation**: <a href="https://lancetnik.github.io/Propan/" target="_blank">https://lancetnik.github.io/Propan/</a>
 
-**Sources**: <a href="https://github.com/Lancetnik/Propan/" target="_blank">https://github.com/Lancetnik/Propan/</a>
-
 ---
 
 ### The key features are
 
 * **Easy**: Designed to be easy to use and learn.
 * **Intuitive**: Great editor support. Autocompletion everywhere.
 * [**Dependencies management**](#dependencies): Minimize code duplication. Multiple features from each argument and parameter declaration.
 * [**Integrations**](#http-frameworks-integrations): **Propan** is ready to use in pair with [any HTTP framework](https://lancetnik.github.io/Propan/5_integrations/1_integrations-index/) you want
 * **MQ independent**: Single interface to popular MQ:
     * **NATS** (based on [nats-py](https://github.com/nats-io/nats.py)) 
-    * **RabbitMQ** (based on [aio-pika](https://aio-pika.readthedocs.io/en/latest/)) 
+    * **RabbitMQ** (based on [aio-pika](https://aio-pika.readthedocs.io/en/latest/))
+* [**RPC**](https://lancetnik.github.io/Propan/2_getting_started/4_broker/4_rpc/): The framework supports RPC requests over MQ, which will allow performing long operations on remote services asynchronously.
 * [**Greate to develop**](#cli-power): CLI tool provides great development experience:
     * framework-independent way to rule application environment
     * application code hot reloading
 
 ### Supported MQ brokers
 |              | async                                                   | sync                 |
 |--------------|:-------------------------------------------------------:|:--------------------:|
@@ -273,34 +272,64 @@
 
 Now you can enjoy a new development experience!
 
 ---
 
 ## HTTP Frameworks integrations
 
+### Any Framework
+
 You can use **Propan** `MQBrokers` without `PropanApp`.
 Just *start* and *stop* them according to your application lifespan.
 
 ```python
-from contextlib import asynccontextmanager
+from propan import NatsBroker
+from sanic import Sanic
 
-from fastapi import FastAPI
-from propan import RabbitBroker
+app = Sanic("MyHelloWorldApp")
+broker = NatsBroker("nats://localhost:4222")
 
-broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
-
-app = FastAPI()
+@broker.handle("test")
+async def base_handler(body):
+    print(body)
 
-@asynccontextmanager
-async def lifespan(app: FastAPI):
+@app.after_server_start
+async def start_broker(app, loop):
     await broker.start()
-    yield
+
+@app.after_server_stop
+async def stop_broker(app, loop):
     await broker.close()
+```
 
-@broker.handle("test")
-async def base_handler(body):
-    print(body)
+### FastAPI Plugin
+
+Also, **Propan** can be used as part of **FastAPI**.
+
+Just import a **PropanRouter** you need and declare the message handler
+using the `@event` decorator. This decorator is similar to the decorator `@handle` for the corresponding brokers.
+
+```python
+from fastapi import Depends, FastAPI
+from pydantic import BaseModel
+from propan.fastapi import RabbitRouter
+
+app = FastAPI()
+
+router = RabbitRouter("amqp://guest:guest@localhost:5672")
+
+class Incoming(BaseModel):
+    m: dict
+
+def call():
+    return True
+
+@router.event("test")
+async def hello(m: Incoming, d = Depends(call)) -> dict:
+    return { "response": "Hello, Propan!" }
+
+app.include_router(router)
 ```
 
 ## Examples
 
 To see more framework usages go to [**examples/**](https://github.com/Lancetnik/Propan/tree/main/examples)
```

### Comparing `propan-0.0.9.2/pyproject.toml` & `propan-0.0.9.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -125,39 +125,40 @@
 ]
 
 [tool.hatch.envs.test]
 features = [
   "test",
 ]
 
+[[tool.hatch.envs.test.matrix]]
+python = ["37", "38", "39", "310", "311"]
+
 [tool.hatch.envs.test.scripts]
 run = "pytest -q -m 'not slow'"
 run-all = "pytest -m 'all'"
 
-[[tool.hatch.envs.test.matrix]]
-python = ["37", "38", "39", "310", "311"]
-
 [tool.hatch.envs.test-last]
 python = "3.11"
 features = [
   "test",
 ]
 
 [tool.hatch.envs.test-last.scripts]
 run = "pytest -q -m 'not slow'"
 run-all = "pytest -v -m 'all'"
 cov = "bash ./scripts/test-cov.sh -v -m 'all'"
 
 [tool.mypy]
 strict = true
 ignore_missing_imports = true
+disallow_subclassing_any = true
 
 [tool.isort]
 profile = "black"
-known_third_party = ["propan", "pydantic", "aio-pika", "nats-py"]
+known_first_party = ["propan"]
 
 [tool.ruff]
 select = [
     "E",  # pycodestyle errors
     "W",  # pycodestyle warnings
     "F",  # pyflakes
     "I",  # isort
@@ -165,23 +166,20 @@
     "B",  # flake8-bugbear
 ]
 ignore = [
     "E501",  # line too long, handled by black
     "C901",  # too complex
 ]
 
-[tool.ruff.isort]
-known-third-party = ["propan", "pydantic", "aio-pika", "nats-py"]
-
 [tool.ruff.flake8-bugbear]
 extend-immutable-calls = [
-    "propan.Depends", "propan.Alias",
-    "propan.utils.Depends", "propan.utils.Alias",
-    "propan.utils.context.Depends", "propan.utils.context.Alias",
-    "typer.Argument", "typer.Option",
+    "propan.Depends", "propan.Context",
+    "propan.utils.Depends", "propan.utils.Context",
+    "propan.utils.context.Depends", "propan.utils.context.Context",
+    "typer.Argument", "typer.Option", "fastapi.Depends",
 ]
 
 [tool.pytest.ini_options]
 minversion = "7.0"
 addopts = "-q -m 'not slow'"
 testpaths = [
     "tests",
```

### Comparing `propan-0.0.9.2/PKG-INFO` & `propan-0.0.9.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propan
-Version: 0.0.9.2
+Version: 0.0.9.3
 Summary: Propan framework: the simplest way to work with a messaging queues
 Project-URL: Homepage, https://lancetnik.github.io/Propan/
 Project-URL: Documentation, https://lancetnik.github.io/Propan/
 Project-URL: Tracker, https://github.com/Lancetnik/Propan/issues
 Project-URL: Source, https://github.com/Lancetnik/Propan
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-Expression: MIT
@@ -105,27 +105,26 @@
 
 It is a modern, high-level framework on top of popular specific Python brokers libraries, based on [*pydantic*](https://docs.pydantic.dev/) and [*fastapi*](https://fastapi.tiangolo.com/ru/), [*pytest*](https://docs.pytest.org/en/7.3.x/) concepts.
 
 ---
 
 **Documentation**: <a href="https://lancetnik.github.io/Propan/" target="_blank">https://lancetnik.github.io/Propan/</a>
 
-**Sources**: <a href="https://github.com/Lancetnik/Propan/" target="_blank">https://github.com/Lancetnik/Propan/</a>
-
 ---
 
 ### The key features are
 
 * **Easy**: Designed to be easy to use and learn.
 * **Intuitive**: Great editor support. Autocompletion everywhere.
 * [**Dependencies management**](#dependencies): Minimize code duplication. Multiple features from each argument and parameter declaration.
 * [**Integrations**](#http-frameworks-integrations): **Propan** is ready to use in pair with [any HTTP framework](https://lancetnik.github.io/Propan/5_integrations/1_integrations-index/) you want
 * **MQ independent**: Single interface to popular MQ:
     * **NATS** (based on [nats-py](https://github.com/nats-io/nats.py)) 
-    * **RabbitMQ** (based on [aio-pika](https://aio-pika.readthedocs.io/en/latest/)) 
+    * **RabbitMQ** (based on [aio-pika](https://aio-pika.readthedocs.io/en/latest/))
+* [**RPC**](https://lancetnik.github.io/Propan/2_getting_started/4_broker/4_rpc/): The framework supports RPC requests over MQ, which will allow performing long operations on remote services asynchronously.
 * [**Greate to develop**](#cli-power): CLI tool provides great development experience:
     * framework-independent way to rule application environment
     * application code hot reloading
 
 ### Supported MQ brokers
 |              | async                                                   | sync                 |
 |--------------|:-------------------------------------------------------:|:--------------------:|
@@ -343,34 +342,64 @@
 
 Now you can enjoy a new development experience!
 
 ---
 
 ## HTTP Frameworks integrations
 
+### Any Framework
+
 You can use **Propan** `MQBrokers` without `PropanApp`.
 Just *start* and *stop* them according to your application lifespan.
 
 ```python
-from contextlib import asynccontextmanager
+from propan import NatsBroker
+from sanic import Sanic
 
-from fastapi import FastAPI
-from propan import RabbitBroker
+app = Sanic("MyHelloWorldApp")
+broker = NatsBroker("nats://localhost:4222")
 
-broker = RabbitBroker("amqp://guest:guest@localhost:5672/")
-
-app = FastAPI()
+@broker.handle("test")
+async def base_handler(body):
+    print(body)
 
-@asynccontextmanager
-async def lifespan(app: FastAPI):
+@app.after_server_start
+async def start_broker(app, loop):
     await broker.start()
-    yield
+
+@app.after_server_stop
+async def stop_broker(app, loop):
     await broker.close()
+```
 
-@broker.handle("test")
-async def base_handler(body):
-    print(body)
+### FastAPI Plugin
+
+Also, **Propan** can be used as part of **FastAPI**.
+
+Just import a **PropanRouter** you need and declare the message handler
+using the `@event` decorator. This decorator is similar to the decorator `@handle` for the corresponding brokers.
+
+```python
+from fastapi import Depends, FastAPI
+from pydantic import BaseModel
+from propan.fastapi import RabbitRouter
+
+app = FastAPI()
+
+router = RabbitRouter("amqp://guest:guest@localhost:5672")
+
+class Incoming(BaseModel):
+    m: dict
+
+def call():
+    return True
+
+@router.event("test")
+async def hello(m: Incoming, d = Depends(call)) -> dict:
+    return { "response": "Hello, Propan!" }
+
+app.include_router(router)
 ```
 
 ## Examples
 
 To see more framework usages go to [**examples/**](https://github.com/Lancetnik/Propan/tree/main/examples)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propan Version: 0.0.9.2 Summary: Propan framework:
+Metadata-Version: 2.1 Name: propan Version: 0.0.9.3 Summary: Propan framework:
 the simplest way to work with a messaging queues Project-URL: Homepage, https:/
 /lancetnik.github.io/Propan/ Project-URL: Documentation, https://
 lancetnik.github.io/Propan/ Project-URL: Tracker, https://github.com/Lancetnik/
 Propan/issues Project-URL: Source, https://github.com/Lancetnik/Propan Author-
 email: Pastukhov Nikita
 yandex.ru> License-Expression: MIT License-File: LICENSE Keywords:
 framework,message brokers,rabbitmq Classifier: Development Status :: 4 - Beta
@@ -49,80 +49,83 @@
 framework**. It's following by [*fastapi*](https://fastapi.tiangolo.com/ru/),
 simplify Message Brokers around code writing and provides a helpful development
 toolkit, which existed only in HTTP-frameworks world until now. It's designed
 to create reactive microservices around Messaging_Architecture. It is a modern,
 high-level framework on top of popular specific Python brokers libraries, based
 on [*pydantic*](https://docs.pydantic.dev/) and [*fastapi*](https://
 fastapi.tiangolo.com/ru/), [*pytest*](https://docs.pytest.org/en/7.3.x/
-) concepts. --- **Documentation**: https://lancetnik.github.io/Propan/
-**Sources**: https://github.com/Lancetnik/Propan/ --- ### The key features are
-* **Easy**: Designed to be easy to use and learn. * **Intuitive**: Great editor
-support. Autocompletion everywhere. * [**Dependencies management**]
-(#dependencies): Minimize code duplication. Multiple features from each
-argument and parameter declaration. * [**Integrations**](#http-frameworks-
-integrations): **Propan** is ready to use in pair with [any HTTP framework]
-(https://lancetnik.github.io/Propan/5_integrations/1_integrations-index/) you
-want * **MQ independent**: Single interface to popular MQ: * **NATS** (based on
-[nats-py](https://github.com/nats-io/nats.py)) * **RabbitMQ** (based on [aio-
-pika](https://aio-pika.readthedocs.io/en/latest/)) * [**Greate to develop**]
-(#cli-power): CLI tool provides great development experience: * framework-
-independent way to rule application environment * application code hot
-reloading ### Supported MQ brokers | | async | sync | |--------------|:--------
------------------------------------------------:|:--------------------:| |
-**RabbitMQ** | :heavy_check_mark: **stable** :heavy_check_mark: | :mag:
-planning :mag: | | **Nats** | :warning: **beta** :warning: | :mag: planning :
-mag: | | **NatsJS** | :hammer_and_wrench: **in progress** :hammer_and_wrench: |
-:mag: planning :mag: | | **MQTT** | :mag: planning :mag: | :mag: planning :mag:
-| | **REDIS** | :mag: planning :mag: | :mag: planning :mag: | | **Kafka** | :
-mag: planning :mag: | :mag: planning :mag: | | **SQS** | :mag: planning :mag: |
-:mag: planning :mag: | ### Community If you are interested in this project,
-please give me feedback by star or/and watch repository. If you have any
-questions or ideas about features to implement, welcome to [discussions](https:
-//github.com/Lancetnik/Propan/discussions) or public [telegram group](https://
-t.me/propan_python). --- ## Declarative? With declarative tools you should
-define **what you need to get**. With traditional imperative tools you should
-write **what you need to do**. Take a look at classic imperative tools, such as
-[aio-pika](https://aio-pika.readthedocs.io/en/latest/), [pika](https://
-pika.readthedocs.io/en/stable/), [nats-py](https://github.com/nats-io/nats.py),
-etc. This is the **Quickstart** with the *aio-pika*: ```python import asyncio
-import aio_pika async def main(): connection = await aio_pika.connect_robust
-( "amqp://guest:guest@127.0.0.1/" ) queue_name = "test_queue" async with
-connection: channel = await connection.channel() queue = await
-channel.declare_queue(queue_name) async with queue.iterator() as queue_iter:
-async for message in queue_iter: async with message.process(): print
-(message.body) asyncio.run(main()) ``` **aio-pika** is a really great tool with
-a really easy learning curve. But it's still imperative. You need to *connect*,
-declare *channel*, *queues*, *exchanges* by yourself. Also, you need to manage
-*connection*, *message*, *queue* context to avoid any troubles. It is not a bad
-way, but it can be easy. ```python from propan import PropanApp, RabbitBroker
+) concepts. --- **Documentation**: https://lancetnik.github.io/Propan/ --- ###
+The key features are * **Easy**: Designed to be easy to use and learn. *
+**Intuitive**: Great editor support. Autocompletion everywhere. *
+[**Dependencies management**](#dependencies): Minimize code duplication.
+Multiple features from each argument and parameter declaration. *
+[**Integrations**](#http-frameworks-integrations): **Propan** is ready to use
+in pair with [any HTTP framework](https://lancetnik.github.io/Propan/
+5_integrations/1_integrations-index/) you want * **MQ independent**: Single
+interface to popular MQ: * **NATS** (based on [nats-py](https://github.com/
+nats-io/nats.py)) * **RabbitMQ** (based on [aio-pika](https://aio-
+pika.readthedocs.io/en/latest/)) * [**RPC**](https://lancetnik.github.io/
+Propan/2_getting_started/4_broker/4_rpc/): The framework supports RPC requests
+over MQ, which will allow performing long operations on remote services
+asynchronously. * [**Greate to develop**](#cli-power): CLI tool provides great
+development experience: * framework-independent way to rule application
+environment * application code hot reloading ### Supported MQ brokers | | async
+| sync | |--------------|:-----------------------------------------------------
+--:|:--------------------:| | **RabbitMQ** | :heavy_check_mark: **stable** :
+heavy_check_mark: | :mag: planning :mag: | | **Nats** | :warning: **beta** :
+warning: | :mag: planning :mag: | | **NatsJS** | :hammer_and_wrench: **in
+progress** :hammer_and_wrench: | :mag: planning :mag: | | **MQTT** | :mag:
+planning :mag: | :mag: planning :mag: | | **REDIS** | :mag: planning :mag: | :
+mag: planning :mag: | | **Kafka** | :mag: planning :mag: | :mag: planning :mag:
+| | **SQS** | :mag: planning :mag: | :mag: planning :mag: | ### Community If
+you are interested in this project, please give me feedback by star or/and
+watch repository. If you have any questions or ideas about features to
+implement, welcome to [discussions](https://github.com/Lancetnik/Propan/
+discussions) or public [telegram group](https://t.me/propan_python). --- ##
+Declarative? With declarative tools you should define **what you need to get**.
+With traditional imperative tools you should write **what you need to do**.
+Take a look at classic imperative tools, such as [aio-pika](https://aio-
+pika.readthedocs.io/en/latest/), [pika](https://pika.readthedocs.io/en/stable/
+), [nats-py](https://github.com/nats-io/nats.py), etc. This is the
+**Quickstart** with the *aio-pika*: ```python import asyncio import aio_pika
+async def main(): connection = await aio_pika.connect_robust( "amqp://guest:
+guest@127.0.0.1/" ) queue_name = "test_queue" async with connection: channel =
+await connection.channel() queue = await channel.declare_queue(queue_name)
+async with queue.iterator() as queue_iter: async for message in queue_iter:
+async with message.process(): print(message.body) asyncio.run(main()) ```
+**aio-pika** is a really great tool with a really easy learning curve. But it's
+still imperative. You need to *connect*, declare *channel*, *queues*,
+*exchanges* by yourself. Also, you need to manage *connection*, *message*,
+*queue* context to avoid any troubles. It is not a bad way, but it can be easy.
+```python from propan import PropanApp, RabbitBroker broker = RabbitBroker
+("amqp://guest:guest@localhost:5672/") app = PropanApp(broker) @broker.handle
+("test_queue") async def base_handler(body): print(body) ``` This is the
+**Propan** declarative way to write the same code. That is so much easier,
+isn't it? --- ## Quickstart Install using `pip`: ```shell $ pip install "propan
+[async-rabbit]" # or $ pip install "propan[async-nats]" ``` ### Basic usage
+Create an application with the following code at `serve.py`: ```python from
+propan import PropanApp from propan import RabbitBroker # from propan import
+NatsBroker broker = RabbitBroker("amqp://guest:guest@localhost:5672/") # broker
+= NatsBroker("nats://localhost:4222") app = PropanApp(broker) @broker.handle
+("test") async def base_handler(body): '''Handle all default exchange messages
+with `test` routing key''' print(body) ``` And just run it: ```shell $ propan
+run serve:app ``` --- ## Type casting Propan uses `pydantic` to cast incoming
+function arguments to types according to their annotation. ```python from
+pydantic import BaseModel from propan import PropanApp, Context, RabbitBroker
 broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app = PropanApp
-(broker) @broker.handle("test_queue") async def base_handler(body): print(body)
-``` This is the **Propan** declarative way to write the same code. That is so
-much easier, isn't it? --- ## Quickstart Install using `pip`: ```shell $ pip
-install "propan[async-rabbit]" # or $ pip install "propan[async-nats]" ``` ###
-Basic usage Create an application with the following code at `serve.py`:
-```python from propan import PropanApp from propan import RabbitBroker # from
-propan import NatsBroker broker = RabbitBroker("amqp://guest:guest@localhost:
-5672/") # broker = NatsBroker("nats://localhost:4222") app = PropanApp(broker)
-@broker.handle("test") async def base_handler(body): '''Handle all default
-exchange messages with `test` routing key''' print(body) ``` And just run it:
-```shell $ propan run serve:app ``` --- ## Type casting Propan uses `pydantic`
-to cast incoming function arguments to types according to their annotation.
-```python from pydantic import BaseModel from propan import PropanApp, Context,
-RabbitBroker broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app =
-PropanApp(broker) class SimpleMessage(BaseModel): key: int @broker.handle
-("test2") async def second_handler(body: SimpleMessage): assert isinstance
-(body.key, int) ``` --- ## Dependencies **Propan** a has dependencies
-management policy close to `pytest fixtures`. You can specify in functions
-arguments which dependencies you would to use. Framework passes them from the
-global Context object. Already existed context fields are: *app*, *broker*,
-*context* (itself), *logger* and *message*. If you call not existing field,
-raises *pydantic.error_wrappers.ValidationError* value. But you can specify
-your own dependencies, call dependencies functions (like `Fastapi Depends`) and
-[more](https://github.com/Lancetnik/Propan/tree/main/examples/dependencies).
+(broker) class SimpleMessage(BaseModel): key: int @broker.handle("test2") async
+def second_handler(body: SimpleMessage): assert isinstance(body.key, int) ``` -
+-- ## Dependencies **Propan** a has dependencies management policy close to
+`pytest fixtures`. You can specify in functions arguments which dependencies
+you would to use. Framework passes them from the global Context object. Already
+existed context fields are: *app*, *broker*, *context* (itself), *logger* and
+*message*. If you call not existing field, raises
+*pydantic.error_wrappers.ValidationError* value. But you can specify your own
+dependencies, call dependencies functions (like `Fastapi Depends`) and [more]
+(https://github.com/Lancetnik/Propan/tree/main/examples/dependencies).
 ```python from logging import Logger import aio_pika from propan import
 PropanApp, Context, RabbitBroker rabbit_broker = RabbitBroker("amqp://guest:
 guest@localhost:5672/") app = PropanApp(rabbit_broker) @rabbit_broker.handle
 ("test") async def base_handler(body: dict, broker: RabbitBroker = Context()):
 assert broker is rabbit_broker ``` --- ## CLI power **Propan** has its own CLI
 tool that provided the following features: * project generation *
 multiprocessing workers * project hot reloading * custom command line arguments
@@ -135,16 +138,25 @@
 ContextRepo): settings = Settings(_env_file=env) context.set_context
 ("settings", settings) ``` ### Project template Also, **Propan CLI** is able to
 generate a production-ready application template: ```shell $ propan create
 [projectname] ``` *Notice: project template require* `pydantic[dotenv]`
 *installation.* Run the created project: ```shell # Run rabbimq first $ docker
 compose --file [projectname]/docker-compose.yaml up -d # Run project $ propan
 run [projectname].app.serve:app --env=.env --reload ``` Now you can enjoy a new
-development experience! --- ## HTTP Frameworks integrations You can use
-**Propan** `MQBrokers` without `PropanApp`. Just *start* and *stop* them
-according to your application lifespan. ```python from contextlib import
-asynccontextmanager from fastapi import FastAPI from propan import RabbitBroker
-broker = RabbitBroker("amqp://guest:guest@localhost:5672/") app = FastAPI()
-@asynccontextmanager async def lifespan(app: FastAPI): await broker.start()
-yield await broker.close() @broker.handle("test") async def base_handler(body):
-print(body) ``` ## Examples To see more framework usages go to [**examples/**]
+development experience! --- ## HTTP Frameworks integrations ### Any Framework
+You can use **Propan** `MQBrokers` without `PropanApp`. Just *start* and *stop*
+them according to your application lifespan. ```python from propan import
+NatsBroker from sanic import Sanic app = Sanic("MyHelloWorldApp") broker =
+NatsBroker("nats://localhost:4222") @broker.handle("test") async def
+base_handler(body): print(body) @app.after_server_start async def start_broker
+(app, loop): await broker.start() @app.after_server_stop async def stop_broker
+(app, loop): await broker.close() ``` ### FastAPI Plugin Also, **Propan** can
+be used as part of **FastAPI**. Just import a **PropanRouter** you need and
+declare the message handler using the `@event` decorator. This decorator is
+similar to the decorator `@handle` for the corresponding brokers. ```python
+from fastapi import Depends, FastAPI from pydantic import BaseModel from
+propan.fastapi import RabbitRouter app = FastAPI() router = RabbitRouter("amqp:
+//guest:guest@localhost:5672") class Incoming(BaseModel): m: dict def call():
+return True @router.event("test") async def hello(m: Incoming, d = Depends
+(call)) -> dict: return { "response": "Hello, Propan!" } app.include_router
+(router) ``` ## Examples To see more framework usages go to [**examples/**]
 (https://github.com/Lancetnik/Propan/tree/main/examples)
```

