# Comparing `tmp/powerapi-2.0.2.tar.gz` & `tmp/powerapi-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powerapi-2.0.2.tar", last modified: Fri Mar 31 08:51:10 2023, max compression
+gzip compressed data, was "powerapi-2.0.3.tar", last modified: Tue Apr 25 14:42:30 2023, max compression
```

## Comparing `powerapi-2.0.2.tar` & `powerapi-2.0.3.tar`

### file list

```diff
@@ -1,118 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:51:10.929235 powerapi-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-03-31 08:50:59.000000 powerapi-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-03-31 08:51:10.929235 powerapi-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-03-31 08:50:59.000000 powerapi-2.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:51:10.917235 powerapi-2.0.2/powerapi/
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:51:10.917235 powerapi-2.0.2/powerapi/actor/
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/actor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12570 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/actor/actor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10444 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/actor/socket_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/actor/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/actor/supervisor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:51:10.917235 powerapi-2.0.2/powerapi/backend_supervisor/
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/backend_supervisor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/backend_supervisor/backend_supervisor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:51:10.917235 powerapi-2.0.2/powerapi/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9696 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/cli/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/cli/config_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15835 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/cli/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18117 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/cli/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    16954 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/cli/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:51:10.921234 powerapi-2.0.2/powerapi/database/
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/database/base_db.py
--rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/database/csvdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/database/direct_prometheus_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/database/file_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/database/influxdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/database/influxdb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/database/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/database/opentsdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/database/prometheus_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/database/socket_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/database/virtiofs_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:51:10.921234 powerapi-2.0.2/powerapi/dispatch_rule/
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/dispatch_rule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/dispatch_rule/dispatch_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/dispatch_rule/hwpc_dispatch_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/dispatch_rule/power_dispatch_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/dispatch_rule/procfs_dispatch_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/dispatch_rule/simple_dispatch_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:51:10.921234 powerapi-2.0.2/powerapi/dispatcher/
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/dispatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/dispatcher/blocking_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     7479 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/dispatcher/dispatcher_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/dispatcher/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/dispatcher/route_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:51:10.921234 powerapi-2.0.2/powerapi/dispatcher/simple/
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/dispatcher/simple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/dispatcher/simple/simple_dispatcher_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/dispatcher/simple/simple_dispatcher_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:51:10.921234 powerapi-2.0.2/powerapi/filter/
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/filter/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:51:10.921234 powerapi-2.0.2/powerapi/formula/
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/formula/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/formula/abstract_cpu_dram_formula.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:51:10.921234 powerapi-2.0.2/powerapi/formula/dummy/
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/formula/dummy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/formula/dummy/dummy_formula_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/formula/dummy/dummy_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/formula/formula_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/formula/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:51:10.921234 powerapi-2.0.2/powerapi/formula/simple/
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/formula/simple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/formula/simple/simple_formula_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/formula/simple/simple_handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:51:10.925235 powerapi-2.0.2/powerapi/handler/
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/handler/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/handler/poison_pill_message_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/handler/start_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:51:10.925235 powerapi-2.0.2/powerapi/puller/
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/puller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7647 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/puller/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/puller/puller_actor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:51:10.925235 powerapi-2.0.2/powerapi/puller/simple/
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/puller/simple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/puller/simple/simple_puller_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/puller/simple/simple_puller_handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:51:10.925235 powerapi-2.0.2/powerapi/pusher/
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/pusher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/pusher/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/pusher/pusher_actor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:51:10.925235 powerapi-2.0.2/powerapi/pusher/simple/
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/pusher/simple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/pusher/simple/simple_pusher_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/pusher/simple/simple_pusher_handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:51:10.925235 powerapi-2.0.2/powerapi/report/
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/report/control_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/report/formula_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/report/hwpc_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/report/power_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/report/procfs_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/report/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:51:10.925235 powerapi-2.0.2/powerapi/report_modifier/
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/report_modifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/report_modifier/libvirt_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/report_modifier/report_modifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:51:10.929235 powerapi-2.0.2/powerapi/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/utils/json_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/utils/stat_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/utils/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/utils/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-03-31 08:50:59.000000 powerapi-2.0.2/powerapi/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:51:10.917235 powerapi-2.0.2/powerapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-03-31 08:51:10.000000 powerapi-2.0.2/powerapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-03-31 08:51:10.000000 powerapi-2.0.2/powerapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 08:51:10.000000 powerapi-2.0.2/powerapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-03-31 08:51:10.000000 powerapi-2.0.2/powerapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-31 08:51:10.000000 powerapi-2.0.2/powerapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-03-31 08:50:59.000000 powerapi-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 08:51:10.929235 powerapi-2.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.830734 powerapi-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-25 14:42:12.000000 powerapi-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-04-25 14:42:30.830734 powerapi-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-04-25 14:42:12.000000 powerapi-2.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.810734 powerapi-2.0.3/powerapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.810734 powerapi-2.0.3/powerapi/actor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/actor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12489 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/actor/actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10444 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/actor/socket_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/actor/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/actor/supervisor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.810734 powerapi-2.0.3/powerapi/backend_supervisor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/backend_supervisor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/backend_supervisor/backend_supervisor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.814734 powerapi-2.0.3/powerapi/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9696 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/cli/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/cli/config_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15911 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/cli/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18117 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/cli/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16954 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/cli/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.818734 powerapi-2.0.3/powerapi/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/database/base_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/database/csvdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/database/direct_prometheus_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/database/file_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/database/influxdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/database/influxdb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/database/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/database/opentsdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/database/prometheus_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/database/socket_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/database/virtiofs_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.818734 powerapi-2.0.3/powerapi/dispatch_rule/
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/dispatch_rule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/dispatch_rule/dispatch_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/dispatch_rule/hwpc_dispatch_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/dispatch_rule/power_dispatch_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/dispatch_rule/procfs_dispatch_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/dispatch_rule/simple_dispatch_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.818734 powerapi-2.0.3/powerapi/dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/dispatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/dispatcher/blocking_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7479 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/dispatcher/dispatcher_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/dispatcher/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/dispatcher/route_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.818734 powerapi-2.0.3/powerapi/dispatcher/simple/
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/dispatcher/simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/dispatcher/simple/simple_dispatcher_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/dispatcher/simple/simple_dispatcher_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.822734 powerapi-2.0.3/powerapi/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/filter/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.822734 powerapi-2.0.3/powerapi/formula/
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/formula/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/formula/abstract_cpu_dram_formula.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/formula/formula_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/formula/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.822734 powerapi-2.0.3/powerapi/formula/simple/
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/formula/simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/formula/simple/simple_formula_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/formula/simple/simple_handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.822734 powerapi-2.0.3/powerapi/handler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/handler/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/handler/poison_pill_message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/handler/start_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.822734 powerapi-2.0.3/powerapi/puller/
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/puller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/puller/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/puller/puller_actor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.822734 powerapi-2.0.3/powerapi/puller/simple/
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/puller/simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/puller/simple/simple_puller_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/puller/simple/simple_puller_handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.826734 powerapi-2.0.3/powerapi/pusher/
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/pusher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/pusher/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/pusher/pusher_actor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.826734 powerapi-2.0.3/powerapi/pusher/simple/
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/pusher/simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/pusher/simple/simple_pusher_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/pusher/simple/simple_pusher_handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.826734 powerapi-2.0.3/powerapi/report/
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/report/control_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/report/formula_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/report/hwpc_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/report/power_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/report/procfs_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/report/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.826734 powerapi-2.0.3/powerapi/report_modifier/
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/report_modifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/report_modifier/libvirt_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/report_modifier/report_modifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.826734 powerapi-2.0.3/powerapi/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/utils/json_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/utils/stat_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/utils/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/utils/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-25 14:42:12.000000 powerapi-2.0.3/powerapi/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:42:30.810734 powerapi-2.0.3/powerapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-04-25 14:42:30.000000 powerapi-2.0.3/powerapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-04-25 14:42:30.000000 powerapi-2.0.3/powerapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:42:30.000000 powerapi-2.0.3/powerapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-25 14:42:30.000000 powerapi-2.0.3/powerapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-25 14:42:30.000000 powerapi-2.0.3/powerapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-25 14:42:12.000000 powerapi-2.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 14:42:30.830734 powerapi-2.0.3/setup.cfg
```

### Comparing `powerapi-2.0.2/LICENSE` & `powerapi-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/PKG-INFO` & `powerapi-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powerapi
-Version: 2.0.2
+Version: 2.0.3
 Summary: PowerAPI is a middleware toolkit for building software-defined power meters.
 Author-email: PowerAPI Staff <powerapi-staff@inria.fr>
 License: BSD-3-Clause
 Project-URL: homepage, https://powerapi.org
 Project-URL: documentation, https://powerapi.readthedocs.org
 Project-URL: repository, https://github.com/powerapi-ng/powerapi
 Keywords: powerapi,energy,power-meter,green-computing
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: powerapi Version: 2.0.2 Summary: PowerAPI is a
+Metadata-Version: 2.1 Name: powerapi Version: 2.0.3 Summary: PowerAPI is a
 middleware toolkit for building software-defined power meters. Author-email:
 PowerAPI Staff
 inria.fr> License: BSD-3-Clause Project-URL: homepage, https://powerapi.org
 Project-URL: documentation, https://powerapi.readthedocs.org Project-URL:
 repository, https://github.com/powerapi-ng/powerapi Keywords:
 powerapi,energy,power-meter,green-computing Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `powerapi-2.0.2/README.md` & `powerapi-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/__init__.py` & `powerapi-2.0.3/powerapi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "2.0.2"
+__version__ = "2.0.3"
```

### Comparing `powerapi-2.0.2/powerapi/actor/__init__.py` & `powerapi-2.0.3/powerapi/actor/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/actor/actor.py` & `powerapi-2.0.3/powerapi/actor/actor.py`

 * *Files 2% similar despite different names*

```diff
@@ -264,17 +264,14 @@
         self.socket_interface.send_control(msg)
         self.logger.debug('send control [' + str(msg) + '] to Actor ' + self.name)
 
     def receive_control(self, timeout=None):
         """
         Receive a message from this actor on the control canal
         """
-        if timeout is None:
-            timeout = self.socket_interface.timeout
-
         msg = self.socket_interface.receive_control(timeout)
         self.logger.debug('Actor ' + self.name + ' receive control : [' + str(msg) + ']')
         return msg
 
     def send_data(self, msg):
         """
         Send a msg to this actor using the data canal
```

### Comparing `powerapi-2.0.2/powerapi/actor/socket_interface.py` & `powerapi-2.0.3/powerapi/actor/socket_interface.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/actor/state.py` & `powerapi-2.0.3/powerapi/actor/state.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/actor/supervisor.py` & `powerapi-2.0.3/powerapi/actor/supervisor.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/backend_supervisor/__init__.py` & `powerapi-2.0.3/powerapi/backend_supervisor/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/backend_supervisor/backend_supervisor.py` & `powerapi-2.0.3/powerapi/backend_supervisor/backend_supervisor.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/cli/__init__.py` & `powerapi-2.0.3/powerapi/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/cli/config_parser.py` & `powerapi-2.0.3/powerapi/cli/config_parser.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/cli/config_validator.py` & `powerapi-2.0.3/powerapi/cli/config_validator.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/cli/generator.py` & `powerapi-2.0.3/powerapi/cli/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 import sys
 from typing import Dict, Type
 
 from powerapi.actor import Actor
 from powerapi.database.influxdb2 import InfluxDB2
 from powerapi.exception import PowerAPIException
 from powerapi.filter import Filter
-from powerapi.report import HWPCReport, PowerReport, ControlReport, ProcfsReport, Report
+from powerapi.report import HWPCReport, PowerReport, ControlReport, ProcfsReport, Report, FormulaReport
 from powerapi.database import MongoDB, CsvDB, InfluxDB, OpenTSDB, SocketDB, PrometheusDB, DirectPrometheusDB, \
     VirtioFSDB, FileDB
 from powerapi.puller import PullerActor
 from powerapi.pusher import PusherActor
 
 from powerapi.report_modifier.libvirt_mapper import LibvirtMapper
 from powerapi.puller.simple.simple_puller_actor import SimplePullerActor
@@ -192,14 +192,15 @@
 class DBActorGenerator(SimpleGenerator):
     """
     ActorGenerator that initialise the start message with a database from config
     """
 
     def __init__(self, component_group_name: str):
         SimpleGenerator.__init__(self, component_group_name)
+        self.report_classes['FormulaReport'] = FormulaReport
         self.report_classes['ControlReport'] = ControlReport
         self.report_classes['ProcfsReport'] = ProcfsReport
 
         self.db_factory = {
             'mongodb': lambda db_config: MongoDB(db_config['model'], db_config['uri'], db_config['db'],
                                                  db_config['collection']),
             'socket': lambda db_config: SocketDB(db_config['model'], db_config['port']),
```

### Comparing `powerapi-2.0.2/powerapi/cli/parser.py` & `powerapi-2.0.3/powerapi/cli/parser.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/cli/tools.py` & `powerapi-2.0.3/powerapi/cli/tools.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/database/__init__.py` & `powerapi-2.0.3/powerapi/database/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/database/base_db.py` & `powerapi-2.0.3/powerapi/database/base_db.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/database/csvdb.py` & `powerapi-2.0.3/powerapi/database/csvdb.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/database/direct_prometheus_db.py` & `powerapi-2.0.3/powerapi/database/direct_prometheus_db.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/database/file_db.py` & `powerapi-2.0.3/powerapi/database/file_db.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/database/influxdb.py` & `powerapi-2.0.3/powerapi/database/influxdb.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/database/influxdb2.py` & `powerapi-2.0.3/powerapi/database/influxdb2.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/database/mongodb.py` & `powerapi-2.0.3/powerapi/database/mongodb.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/database/opentsdb.py` & `powerapi-2.0.3/powerapi/database/opentsdb.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/database/prometheus_db.py` & `powerapi-2.0.3/powerapi/database/prometheus_db.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/database/socket_db.py` & `powerapi-2.0.3/powerapi/database/socket_db.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/database/virtiofs_db.py` & `powerapi-2.0.3/powerapi/database/virtiofs_db.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/dispatch_rule/__init__.py` & `powerapi-2.0.3/powerapi/dispatch_rule/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/dispatch_rule/dispatch_rule.py` & `powerapi-2.0.3/powerapi/dispatch_rule/dispatch_rule.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/dispatch_rule/hwpc_dispatch_rule.py` & `powerapi-2.0.3/powerapi/dispatch_rule/hwpc_dispatch_rule.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/dispatch_rule/power_dispatch_rule.py` & `powerapi-2.0.3/powerapi/dispatch_rule/power_dispatch_rule.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/dispatch_rule/procfs_dispatch_rule.py` & `powerapi-2.0.3/powerapi/dispatch_rule/procfs_dispatch_rule.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/dispatch_rule/simple_dispatch_rule.py` & `powerapi-2.0.3/powerapi/dispatch_rule/simple_dispatch_rule.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/dispatcher/__init__.py` & `powerapi-2.0.3/powerapi/dispatcher/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/dispatcher/blocking_detector.py` & `powerapi-2.0.3/powerapi/dispatcher/blocking_detector.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/dispatcher/dispatcher_actor.py` & `powerapi-2.0.3/powerapi/dispatcher/dispatcher_actor.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/dispatcher/handlers.py` & `powerapi-2.0.3/powerapi/dispatcher/handlers.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/dispatcher/route_table.py` & `powerapi-2.0.3/powerapi/dispatcher/route_table.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/dispatcher/simple/__init__.py` & `powerapi-2.0.3/powerapi/dispatcher/simple/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/dispatcher/simple/simple_dispatcher_actor.py` & `powerapi-2.0.3/powerapi/dispatcher/simple/simple_dispatcher_actor.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/dispatcher/simple/simple_dispatcher_handlers.py` & `powerapi-2.0.3/powerapi/dispatcher/simple/simple_dispatcher_handlers.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/exception.py` & `powerapi-2.0.3/powerapi/exception.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/filter/__init__.py` & `powerapi-2.0.3/powerapi/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/filter/filter.py` & `powerapi-2.0.3/powerapi/filter/filter.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/formula/__init__.py` & `powerapi-2.0.3/powerapi/formula/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,10 +25,9 @@
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from powerapi.formula.handlers import FormulaPoisonPillMessageHandler
 from powerapi.formula.abstract_cpu_dram_formula import AbstractCpuDramFormula
-from powerapi.formula.dummy.dummy_formula_actor import DummyFormulaActor
 from powerapi.formula.formula_actor import FormulaActor, FormulaState
 from powerapi.formula.simple.simple_formula_actor import SimpleFormulaActor
```

### Comparing `powerapi-2.0.2/powerapi/formula/abstract_cpu_dram_formula.py` & `powerapi-2.0.3/powerapi/formula/abstract_cpu_dram_formula.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/formula/dummy/__init__.py` & `powerapi-2.0.3/powerapi/formula/simple/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-from powerapi.formula.dummy.dummy_formula_actor import DummyFormulaActor, DummyFormulaState
+from powerapi.formula.simple.simple_formula_actor import SimpleFormulaActor
```

### Comparing `powerapi-2.0.2/powerapi/formula/dummy/dummy_formula_actor.py` & `powerapi-2.0.3/powerapi/formula/formula_actor.py`

 * *Files 21% similar despite different names*

```diff
@@ -24,60 +24,69 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import logging
-from typing import Dict, Any
+import re
 
-from powerapi.actor import Actor
+from typing import Dict
 
-from powerapi.handler import StartHandler
-from powerapi.report import Report
-from powerapi.message import PoisonPillMessage, StartMessage
+from powerapi.actor import Actor, State
+from powerapi.pusher import PusherActor
 
-from powerapi.formula.abstract_cpu_dram_formula import AbstractCpuDramFormula, AbstractCpuDramFormulaState
-from powerapi.formula.handlers import FormulaPoisonPillMessageHandler
-from powerapi.formula.dummy.dummy_handlers import ReportHandler
 
-
-class DummyFormulaState(AbstractCpuDramFormulaState):
+class FormulaState(State):
     """
-    Formula values with configurable sleeping time for dummy formula
+    Initialize a new Formula actor state.
+    :param actor: Actor linked to the state
+    :param pushers: Pushers available for the actor
+    :param metadata: Metadata related to the state
     """
 
-    def __init__(self, actor: Actor, pushers: Dict[str, Actor], metadata: Dict[str, Any], socket: str, core: str,
-                 sleep_time: int):
-        AbstractCpuDramFormulaState.__init__(self, actor, pushers, metadata, socket, core)
-        self.sleep_time = sleep_time
+    def __init__(self, actor, pushers, metadata):
+        super().__init__(actor)
+        self.pushers = pushers
+        self.metadata = metadata
 
 
-class DummyFormulaActor(AbstractCpuDramFormula):
+class FormulaActor(Actor):
     """
-    A fake Formula that simulate data processing by waiting 1s and send a
-    power report containing 42
+    Abstract actor class used to implement formula actor that compute power consumption of a device from Reports
     """
 
-    def __init__(self, name, pushers, socket, core, level_logger=logging.WARNING, sleep_time=0, timeout=None):
+    def __init__(self, name, pushers: Dict[str, PusherActor], level_logger=logging.WARNING, timeout=None):
         """
-        Initialize a new Dummy Formula actor.
+        Initialize a new Formula actor.
         :param name: Actor name
         :param pushers: Pusher actors
-        :param socket:
-        :param core:
         :param level_logger: Level of the logger
         :param timeout: Time in millisecond to wait for a message before calling the timeout handler
         """
-        AbstractCpuDramFormula.__init__(self, name, pushers, socket, core, level_logger, timeout)
+        Actor.__init__(self, name, level_logger, timeout)
+
+        self.formula_metadata = self._extract_formula_metadata(name)
+        self.state = FormulaState(self, pushers, self.formula_metadata)
+
+    @staticmethod
+    def _extract_formula_metadata(formula_name):
+        metadata_str = re.findall(r'\'([\w_]*)\'', formula_name)
+
+        metadata = {}
+
+        if len(metadata_str) >= 2:
+            metadata['sensor'] = metadata_str[1]
+
+        if len(metadata_str) >= 3:
+            metadata['socket'] = int(metadata_str[2])
 
-        #: (powerapi.State): Basic state of the Formula.
-        self.state = DummyFormulaState(self, pushers, self.formula_metadata, socket, core, sleep_time)
+        if len(metadata_str) >= 4:
+            metadata['core'] = int(metadata_str[3])
+        return metadata
 
     def setup(self):
         """
-        Initialize Handler
+        Setup the Formula actor.
         """
-        AbstractCpuDramFormula.setup(self)
-        self.add_handler(PoisonPillMessage, FormulaPoisonPillMessageHandler(self.state))
-        self.add_handler(Report, ReportHandler(self.state))
-        self.add_handler(StartMessage, StartHandler(self.state))
+        for _, pusher in self.state.pushers.items():
+            pusher.connect_data()
```

### Comparing `powerapi-2.0.2/powerapi/formula/dummy/dummy_handlers.py` & `powerapi-2.0.3/powerapi/formula/simple/simple_handlers.py`

 * *Files 22% similar despite different names*

```diff
@@ -23,45 +23,34 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-import time
-
 from powerapi.handler import Handler
-from powerapi.report import PowerReport
 
 
 class ReportHandler(Handler):
     """
     Basic handler behaviour for a kind of Report
     """
 
     def _estimate(self, report):
         """
         Method that estimate the power consumption from an input report
         :param report: Input Report
-        :return: List of PowerReport
+        :return: List of Input Report
         """
-        socket_id = self.state.socket if self.state.socket is not None else -1
-
-        metadata = report.metadata
-
-        metadata['formula_name'] = self.state.actor.name
-        metadata['socket'] = socket_id
-
-        result_msg = PowerReport(timestamp=report.timestamp, sensor=report.sensor, target=report.target, power=42,
-                                 metadata=metadata)
-        return [result_msg]
+        self.state.actor.logger.debug('received message ' + str(report))
+        return [report]
 
     def handle(self, msg):
         """
         Process a report and send the result to the pusher actor
         :param powerapi.Report msg:  Received message
         """
-        time.sleep(self.state.sleep_time)
         results = self._estimate(msg)
         for _, actor_pusher in self.state.pushers.items():
             for result in results:
                 actor_pusher.send_data(result)
+                self.state.actor.logger.debug('sent message ' + str(result) + ' to ' + str(actor_pusher))
```

### Comparing `powerapi-2.0.2/powerapi/formula/formula_actor.py` & `powerapi-2.0.3/powerapi/handler/start_handler.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Copyright (c) 2022, INRIA
-# Copyright (c) 2022, University of Lille
+# Copyright (c) 2018, INRIA
+# Copyright (c) 2018, University of Lille
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # * Redistributions of source code must retain the above copyright notice, this
 #   list of conditions and the following disclaimer.
@@ -23,70 +23,41 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-import logging
-import re
+from powerapi.message import OKMessage, StartMessage, ErrorMessage
+from .handler import Handler
 
-from typing import Dict
 
-from powerapi.actor import Actor, State
-from powerapi.pusher import PusherActor
-
-
-class FormulaState(State):
+class StartHandler(Handler):
     """
-    Initialize a new Formula actor state.
-    :param actor: Actor linked to the state
-    :param pushers: Pushers available for the actor
-    :param metadata: Metadata related to the state
+    Initialize the received state
     """
 
-    def __init__(self, actor, pushers, metadata):
-        super().__init__(actor)
-        self.pushers = pushers
-        self.metadata = metadata
-
-
-class FormulaActor(Actor):
-    """
-    Abstract actor class used to implement formula actor that compute power consumption of a device from Reports
-    """
-
-    def __init__(self, name, pushers: Dict[str, PusherActor], level_logger=logging.WARNING, timeout=None):
-        """
-        Initialize a new Formula actor.
-        :param name: Actor name
-        :param pushers: Pusher actors
-        :param level_logger: Level of the logger
-        :param timeout: Time in millisecond to wait for a message before calling the timeout handler
+    def handle(self, msg):
         """
-        Actor.__init__(self, name, level_logger, timeout)
-
-        self.formula_metadata = self._extract_formula_metadata(name)
-        self.state = FormulaState(self, pushers, self.formula_metadata)
+        Allow to initialize the state of the actor, then reply to the control
+        socket.
 
-    @staticmethod
-    def _extract_formula_metadata(formula_name):
-        metadata_str = re.findall(r'\'([\w_]*)\'', formula_name)
-
-        metadata = {}
+        :param powerapi.StartMessage msg: Message that initialize the actor
+        """
+        if self.state.initialized:
+            self.state.actor.send_control(
+                ErrorMessage(self.state.actor.name, 'Actor already initialized'))
+            return
 
-        if len(metadata_str) >= 2:
-            metadata['sensor'] = metadata_str[1]
+        if not isinstance(msg, StartMessage):
+            return
 
-        if len(metadata_str) >= 3:
-            metadata['socket'] = int(metadata_str[2])
+        self.initialization()
 
-        if len(metadata_str) >= 4:
-            metadata['core'] = int(metadata_str[3])
-        return metadata
+        if self.state.alive:
+            self.state.initialized = True
+            self.state.actor.send_control(OKMessage(self.state.actor.name))
 
-    def setup(self):
+    def initialization(self):
         """
-        Setup the Formula actor.
+        Abstract method that initialize the actor after receiving a start msg
         """
-        for _, pusher in self.state.pushers.items():
-            pusher.connect_data()
```

### Comparing `powerapi-2.0.2/powerapi/formula/handlers.py` & `powerapi-2.0.3/powerapi/formula/handlers.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/formula/simple/__init__.py` & `powerapi-2.0.3/powerapi/utils/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Copyright (c) 2022, INRIA
-# Copyright (c) 2022, University of Lille
+# Copyright (c) 2021, INRIA
+# Copyright (c) 2021, University of Lille
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # * Redistributions of source code must retain the above copyright notice, this
 #   list of conditions and the following disclaimer.
@@ -23,8 +23,11 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-from powerapi.formula.simple.simple_formula_actor import SimpleFormulaActor
+from powerapi.utils.utils import timestamp_to_datetime, datetime_to_timestamp, dict_merge
+from powerapi.utils.tree import Tree
+from powerapi.utils.stat_buffer import StatBuffer
+from .json_stream import JsonStream
```

### Comparing `powerapi-2.0.2/powerapi/formula/simple/simple_formula_actor.py` & `powerapi-2.0.3/powerapi/formula/simple/simple_formula_actor.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/formula/simple/simple_handlers.py` & `powerapi-2.0.3/powerapi/handler/poison_pill_message_handler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Copyright (c) 2022, INRIA
-# Copyright (c) 2022, University of Lille
+# Copyright (c) 2018, INRIA
+# Copyright (c) 2018, University of Lille
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # * Redistributions of source code must retain the above copyright notice, this
 #   list of conditions and the following disclaimer.
@@ -23,34 +23,54 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-from powerapi.handler import Handler
+from powerapi.message import UnknownMessageTypeException, PoisonPillMessage
+from .handler import Handler
 
 
-class ReportHandler(Handler):
+class PoisonPillMessageHandler(Handler):
     """
-    Basic handler behaviour for a kind of Report
+    Generic handler for PoisonPillMessage
     """
 
-    def _estimate(self, report):
+    def teardown(self, soft=False):
         """
-        Method that estimate the power consumption from an input report
-        :param report: Input Report
-        :return: List of Input Report
+        function called before terminating the actor process
+        could be redefined
         """
-        self.state.actor.logger.debug('received message ' + str(report))
-        return [report]
+
+    def handle_msg(self, msg):
+        """
+        Handle the given message
+        :param msg: The message to handle
+        """
+        Handler.delegate_message_handling(self, msg)
+
+    def _empty_mail_box(self):
+        print(str(self.state.actor.name) + " empty mail box")
+        while True:
+            self.state.actor.socket_interface.timeout = 0.1
+            msg = self.state.actor.socket_interface.receive()
+
+            if msg is not None:
+                self.handle_msg(msg)
+            else:
+                return
 
     def handle(self, msg):
         """
-        Process a report and send the result to the pusher actor
-        :param powerapi.Report msg:  Received message
+        Set the :attr:`alive <powerapi.actor.state.State.alive>`
+        attribute of the actor state to False
+
+        :param Object msg: the message received by the actor
         """
-        results = self._estimate(msg)
-        for _, actor_pusher in self.state.pushers.items():
-            for result in results:
-                actor_pusher.send_data(result)
-                self.state.actor.logger.debug('sent message ' + str(result) + ' to ' + str(actor_pusher))
+        if not isinstance(msg, PoisonPillMessage):
+            raise UnknownMessageTypeException(type(msg))
+
+        if msg.is_soft:
+            self._empty_mail_box()
+        self.teardown(soft=msg.is_soft)
+        self.state.alive = False
```

### Comparing `powerapi-2.0.2/powerapi/handler/__init__.py` & `powerapi-2.0.3/powerapi/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/handler/handler.py` & `powerapi-2.0.3/powerapi/handler/handler.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/handler/poison_pill_message_handler.py` & `powerapi-2.0.3/powerapi/report_modifier/libvirt_mapper.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Copyright (c) 2018, INRIA
-# Copyright (c) 2018, University of Lille
+# Copyright (c) 2021, INRIA
+# Copyright (c) 2021, University of Lille
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # * Redistributions of source code must retain the above copyright notice, this
 #   list of conditions and the following disclaimer.
@@ -11,66 +11,58 @@
 # * Redistributions in binary form must reproduce the above copyright notice,
 #   this list of conditions and the following disclaimer in the documentation
 #   and/or other materials provided with the distribution.
 #
 # * Neither the name of the copyright holder nor the names of its
 #   contributors may be used to endorse or promote products derived from
 #   this software without specific prior written permission.
-#
+
 # THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
 # AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
 # IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-from powerapi.message import UnknownMessageTypeException, PoisonPillMessage
-from .handler import Handler
+import re
+import logging
+
+try:
+    from libvirt import openReadOnly, libvirtError
+except ImportError:
+    logging.getLogger().info("libvirt-python is not installed.")
+
+    class LibvirtException(Exception):
+        """"""
+        def __init__(self, _):
+            Exception.__init__(self)
+
+    libvirtError = LibvirtException
+    openReadOnly = None
+
+from powerapi.report_modifier.report_modifier import ReportModifier
 
 
-class PoisonPillMessageHandler(Handler):
+class LibvirtMapper(ReportModifier):
     """
-    Generic handler for PoisonPillMessage
+    Report modifier which modifi target with libvirt id by open stak uuid
     """
 
-    def teardown(self, soft=False):
-        """
-        function called before terminating the actor process
-        could be redefined
-        """
-
-    def handle_msg(self, msg):
-        """
-        Handle the given message
-        :param msg: The message to handle
-        """
-        Handler.delegate_message_handling(self, msg)
-
-    def _empty_mail_box(self):
-        print(str(self.state.actor.name) + " empty mail box")
-        while True:
-            self.state.actor.socket_interface.timeout = 0.1
-            msg = self.state.actor.socket_interface.receive()
-
-            if msg is not None:
-                self.handle_msg(msg)
-            else:
-                return
-
-    def handle(self, msg):
-        """
-        Set the :attr:`alive <powerapi.actor.state.State.alive>`
-        attribute of the actor state to False
-
-        :param Object msg: the message received by the actor
-        """
-        if not isinstance(msg, PoisonPillMessage):
-            raise UnknownMessageTypeException(type(msg))
-
-        if msg.is_soft:
-            self._empty_mail_box()
-        self.teardown(soft=msg.is_soft)
-        self.state.alive = False
+    def __init__(self, uri: str, regexp: str):
+        self.regexp = re.compile(regexp)
+        daemon_uri = None if uri == '' else uri
+        self.libvirt = openReadOnly(daemon_uri)
+
+    def modify_report(self, report):
+        result = re.match(self.regexp, report.target)
+        if result is not None:
+            domain_name = result.groups(0)[0]
+            try:
+                domain = self.libvirt.lookupByName(domain_name)
+                report.metadata["domain_id"] = domain.UUIDString()
+            except libvirtError:
+                pass
+        return report
```

### Comparing `powerapi-2.0.2/powerapi/handler/start_handler.py` & `powerapi-2.0.3/powerapi/report_modifier/report_modifier.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Copyright (c) 2018, INRIA
-# Copyright (c) 2018, University of Lille
+# Copyright (c) 2021, INRIA
+# Copyright (c) 2021, University of Lille
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # * Redistributions of source code must retain the above copyright notice, this
 #   list of conditions and the following disclaimer.
@@ -11,53 +11,31 @@
 # * Redistributions in binary form must reproduce the above copyright notice,
 #   this list of conditions and the following disclaimer in the documentation
 #   and/or other materials provided with the distribution.
 #
 # * Neither the name of the copyright holder nor the names of its
 #   contributors may be used to endorse or promote products derived from
 #   this software without specific prior written permission.
-#
+
 # THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
 # AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
 # IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-from powerapi.message import OKMessage, StartMessage, ErrorMessage
-from .handler import Handler
+from powerapi.report import Report
 
 
-class StartHandler(Handler):
+class ReportModifier:
     """
-    Initialize the received state
+    Abstract class for object used by puller to modify reports before sending them to dispatcher
     """
-
-    def handle(self, msg):
-        """
-        Allow to initialize the state of the actor, then reply to the control
-        socket.
-
-        :param powerapi.StartMessage msg: Message that initialize the actor
-        """
-        if self.state.initialized:
-            self.state.actor.send_control(
-                ErrorMessage(self.state.actor.name, 'Actor already initialized'))
-            return
-
-        if not isinstance(msg, StartMessage):
-            return
-
-        self.initialization()
-
-        if self.state.alive:
-            self.state.initialized = True
-            self.state.actor.send_control(OKMessage(self.state.actor.name))
-
-    def initialization(self):
+    def modify_report(self, report: Report) -> Report:
         """
-        Abstract method that initialize the actor after receiving a start msg
+        modify the given report
         """
+        raise NotImplementedError()
```

### Comparing `powerapi-2.0.2/powerapi/message.py` & `powerapi-2.0.3/powerapi/message.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/puller/__init__.py` & `powerapi-2.0.3/powerapi/puller/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/puller/handlers.py` & `powerapi-2.0.3/powerapi/puller/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,15 +197,15 @@
         Initialize the database and connect all dispatcher to the
         socket_interface
         """
         db_puller_thread = DBPullerThread(self.state, self.timeout, self)
         db_puller_thread.start()
 
         while self.state.alive:
-            msg = self.state.actor.receive_control(0.1)
+            msg = self.state.actor.receive_control(self.timeout)
             if msg is not None:
                 self.handle_internal_msg(msg)
 
     def _database_connection(self):
         try:
             if not self.state.asynchrone:
                 self.state.database.connect()
```

### Comparing `powerapi-2.0.2/powerapi/puller/puller_actor.py` & `powerapi-2.0.3/powerapi/puller/puller_actor.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
     A Puller allows to handle the reading of a database and to dispatch report
     to many Dispatcher depending on some rules.
     """
 
     def __init__(self, name, database, report_filter, report_model, stream_mode=False, report_modifier_list=[],
                  level_logger=logging.WARNING,
-                 timeout=0, timeout_puller=100):
+                 timeout=5000, timeout_puller=100):
         """
         :param str name: Actor name.
         :param BaseDB database: Allow to interact with a Database.
         :param Filter report_filter: Filter of the Puller.
         :param int level_logger: Define the level of the logger
         :param int tiemout_puller: (require stream mode) time (in ms) between two database reading
         :param bool asynchrone: use asynchrone driver
@@ -116,8 +116,8 @@
         self.low_exception += database.exceptions
 
     def setup(self):
         """
         Define StartMessage handler and PoisonPillMessage handler
         """
         self.add_handler(PoisonPillMessage, PullerPoisonPillMessageHandler(self.state))
-        self.add_handler(StartMessage, PullerStartHandler(self.state, 0.1))
+        self.add_handler(StartMessage, PullerStartHandler(self.state, self.socket_interface.timeout))
```

### Comparing `powerapi-2.0.2/powerapi/puller/simple/__init__.py` & `powerapi-2.0.3/powerapi/puller/simple/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/puller/simple/simple_puller_actor.py` & `powerapi-2.0.3/powerapi/puller/simple/simple_puller_actor.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
+import logging
 from typing import Type
 
 from powerapi.actor import Actor, State
 from powerapi.message import StartMessage, \
     SimplePullerSendReportsMessage, PoisonPillMessage
 from powerapi.puller import PullerPoisonPillMessageHandler
 from powerapi.puller.simple.simple_puller_handlers import SimplePullerHandler, SimplePullerStartHandler
@@ -61,23 +61,24 @@
 
 
 class SimplePullerActor(Actor):
     """
     Simple Actor that generated a given number of messages of a given type
     """
 
-    def __init__(self, name: str, number_of_reports_to_send: int, report_type_to_send: Type[Report], report_filter):
+    def __init__(self, name: str, number_of_reports_to_send: int, report_type_to_send: Type[Report], report_filter,
+                 level_logger: int = logging.WARNING):
         """
         Create an actor with the given information
         :param str name: The actor's name
         :param int number_of_reports_to_send: Number of reports to send
         :param Report report_type_to_send: Report type to be sent
         :param Filter report_filter: Filters and the associated dispatchers and rules
         """
-        Actor.__init__(self, name)
+        Actor.__init__(self, name, level_logger=level_logger)
         self.state = SimplePullerState(self, number_of_reports_to_send, report_type_to_send, report_filter)
 
     def setup(self):
         """
         Defines StartMessage handler, PoisonPillMessage handler and SimplePullerSendReportsMessage handler
         """
         self.add_handler(StartMessage, SimplePullerStartHandler(self.state))
```

### Comparing `powerapi-2.0.2/powerapi/puller/simple/simple_puller_handlers.py` & `powerapi-2.0.3/powerapi/puller/simple/simple_puller_handlers.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/pusher/__init__.py` & `powerapi-2.0.3/powerapi/pusher/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/pusher/handlers.py` & `powerapi-2.0.3/powerapi/pusher/handlers.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/pusher/pusher_actor.py` & `powerapi-2.0.3/powerapi/pusher/pusher_actor.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/pusher/simple/__init__.py` & `powerapi-2.0.3/powerapi/pusher/simple/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/pusher/simple/simple_pusher_actor.py` & `powerapi-2.0.3/powerapi/pusher/simple/simple_pusher_actor.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+import logging
+
+from multiprocessing import Value
 
 from powerapi.actor import Actor, State
 from powerapi.handler import PoisonPillMessageHandler
 from powerapi.message import StartMessage, \
     GetReceivedReportsSimplePusherMessage, PoisonPillMessage
 from powerapi.pusher.simple.simple_pusher_handlers import SimplePusherStartHandler, SimplePusherHandler, \
     SimplePusherGetReceivedReportsHandler
@@ -48,25 +51,26 @@
         """
         :param Actor actor: The actor related to the state
         :param int number_of_reports_to_store: Number of reports to store
         """
         State.__init__(self, actor)
         self.number_of_reports_to_store = number_of_reports_to_store
         self.reports = []
+        self.alive = Value('i', 1)
 
 
 class SimplePusherActor(Actor):
     """
     PusherActor class
 
     The Pusher allows to save Report sent by Formula.
     """
 
-    def __init__(self, name: str, number_of_reports_to_store: int):
-        Actor.__init__(self, name)
+    def __init__(self, name: str, number_of_reports_to_store: int, level_logger: int = logging.WARNING):
+        Actor.__init__(self, name=name, level_logger=level_logger)
         self.state = SimplePusherState(self, number_of_reports_to_store)
 
     def setup(self):
         """
         Defines StartMessage handler, PoisonPillMessage handler, PowerReport handler and HWPCReport handler
         """
         self.add_handler(StartMessage, SimplePusherStartHandler(self.state))
```

### Comparing `powerapi-2.0.2/powerapi/pusher/simple/simple_pusher_handlers.py` & `powerapi-2.0.3/powerapi/pusher/simple/simple_pusher_handlers.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         """
         The reception of a Report makes actor to store it and stop itself if required
         """
         # When receiving a Report save it to the list of reports
         self.state.actor.logger.debug('received message ' + str(report))
         self.save_report(report)
         self.state.actor.logger.debug(str(report) + ' saved to list')
-
+        self.state.actor.logger.debug("reports saved :" + str(len(self.state.reports)))
         self.stop_actor_if_required()
 
     def save_report(self, report: Report):
         """
         Saves the received report in a list
         :param report: Report to be saved
         """
@@ -74,16 +74,16 @@
 
     def stop_actor_if_required(self):
         """
         Stops the actor system if number_of_reports_to_store is reached
         """
         if len(self.state.reports) >= self.state.number_of_reports_to_store:
             self.state.actor.logger.debug("reports saved :" + str(len(self.state.reports)))
-            print("reports saved :" + str(len(self.state.reports)))
             self.state.actor.send_control(PoisonPillMessage(sender_name='system'))
+            self.state.alive = 0
             self.state.actor.logger.debug("exit request sent")
 
 
 class SimplePusherGetReceivedReportsHandler(Handler):
     """
     Handler for GetReceivedReports
     """
```

### Comparing `powerapi-2.0.2/powerapi/report/__init__.py` & `powerapi-2.0.3/powerapi/report/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/report/control_report.py` & `powerapi-2.0.3/powerapi/report/control_report.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/report/formula_report.py` & `powerapi-2.0.3/powerapi/report/formula_report.py`

 * *Files 27% similar despite different names*

```diff
@@ -25,41 +25,79 @@
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from __future__ import annotations
 
+import json
 from datetime import datetime
-from typing import Dict, Any
+from typing import Dict, Any, List
 
-from powerapi.report.report import Report
+from powerapi.report.report import Report, CSV_HEADER_COMMON
+
+CSV_HEADER_FORMULA_REPORT = CSV_HEADER_COMMON + ['metadata']
 
 
 class FormulaReport(Report):
     """
     FormulaReport stores information about a formula.
     This is useful to gather information about a running formula in order to debug or compute statistics.
     """
 
     def __init__(self, timestamp: datetime, sensor: str, target: str, metadata: Dict[str, Any]):
         """
-        Initialize a Power report using the given parameters.
+        Initialize a Formula report using the given parameters.
         :param timestamp: Report timestamp
         :param sensor: Sensor name
         :param target: Target name
-        :param metadata: Metadata values, can be anything that add useful information
+        :param metadata: Metadata values, can be anything but should be json serializable
         """
         Report.__init__(self, timestamp, sensor, target)
         self.metadata = metadata
 
     def __repr__(self) -> str:
-        return 'FormulaReport(%s, %s, %s, %s)' % (self.timestamp, self.sensor, self.target, self.metadata)
+        return f'FormulaReport({self.timestamp}, {self.sensor}, {self.target}, {self.metadata})'
+
+    @staticmethod
+    def to_csv_lines(report: FormulaReport, **_) -> (List[str], Dict[str, Any]):
+        """
+        Convert a Formula report into a csv line.
+        :param report: Formula report that will be converted
+        :return: Tuple containing the csv header and the csv lines
+        """
+
+        line = {
+            'timestamp': int(datetime.timestamp(report.timestamp) * 1000),
+            'sensor': report.sensor,
+            'target': report.target,
+            'metadata': json.dumps(report.metadata)
+        }
+
+        return CSV_HEADER_FORMULA_REPORT, {'FormulaReport': [line]}
+
+    @staticmethod
+    def to_mongodb(report: FormulaReport) -> Dict[str, Any]:
+        """
+        Convert a Formula report into a json document that can be stored into mongodb.
+        :return: a dictionary, that can be stored into a mongodb
+        """
+        return FormulaReport.to_json(report)
 
     @staticmethod
-    def deserialize(data: Dict) -> FormulaReport:
+    def to_influxdb(report: FormulaReport, **_) -> Dict[str, Any]:
         """
-        Generate a report using the given data.
-        :param data: Dictionary containing the report attributes
-        :return: The Formula report initialized with the given data
+        Convert a Formula report into a dict that can be stored into influxdb.
+        param report: Formula report that will be converted
+        :return: a dictionary, that can be stored into influxdb
         """
-        return FormulaReport(data['timestamp'], data['sensor'], data['target'], data['metadata'])
+        document = {
+            'measurement': 'formula_report',
+            'tags': {
+                'sensor': report.sensor,
+                'target': report.target,
+            },
+            'time': int(datetime.timestamp(report.timestamp) * 1000),
+            'fields': report.metadata
+        }
+
+        return document
```

### Comparing `powerapi-2.0.2/powerapi/report/hwpc_report.py` & `powerapi-2.0.3/powerapi/report/hwpc_report.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/report/power_report.py` & `powerapi-2.0.3/powerapi/report/power_report.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/report/procfs_report.py` & `powerapi-2.0.3/powerapi/report/procfs_report.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/report/report.py` & `powerapi-2.0.3/powerapi/report/report.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/report_modifier/__init__.py` & `powerapi-2.0.3/powerapi/report_modifier/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/utils/json_stream.py` & `powerapi-2.0.3/powerapi/utils/json_stream.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/utils/stat_buffer.py` & `powerapi-2.0.3/powerapi/utils/stat_buffer.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/utils/sync.py` & `powerapi-2.0.3/powerapi/utils/sync.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/utils/tree.py` & `powerapi-2.0.3/powerapi/utils/tree.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi/utils/utils.py` & `powerapi-2.0.3/powerapi/utils/utils.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/powerapi.egg-info/PKG-INFO` & `powerapi-2.0.3/powerapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powerapi
-Version: 2.0.2
+Version: 2.0.3
 Summary: PowerAPI is a middleware toolkit for building software-defined power meters.
 Author-email: PowerAPI Staff <powerapi-staff@inria.fr>
 License: BSD-3-Clause
 Project-URL: homepage, https://powerapi.org
 Project-URL: documentation, https://powerapi.readthedocs.org
 Project-URL: repository, https://github.com/powerapi-ng/powerapi
 Keywords: powerapi,energy,power-meter,green-computing
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: powerapi Version: 2.0.2 Summary: PowerAPI is a
+Metadata-Version: 2.1 Name: powerapi Version: 2.0.3 Summary: PowerAPI is a
 middleware toolkit for building software-defined power meters. Author-email:
 PowerAPI Staff
 inria.fr> License: BSD-3-Clause Project-URL: homepage, https://powerapi.org
 Project-URL: documentation, https://powerapi.readthedocs.org Project-URL:
 repository, https://github.com/powerapi-ng/powerapi Keywords:
 powerapi,energy,power-meter,green-computing Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

### Comparing `powerapi-2.0.2/powerapi.egg-info/SOURCES.txt` & `powerapi-2.0.3/powerapi.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -50,17 +50,14 @@
 powerapi/dispatcher/simple/simple_dispatcher_handlers.py
 powerapi/filter/__init__.py
 powerapi/filter/filter.py
 powerapi/formula/__init__.py
 powerapi/formula/abstract_cpu_dram_formula.py
 powerapi/formula/formula_actor.py
 powerapi/formula/handlers.py
-powerapi/formula/dummy/__init__.py
-powerapi/formula/dummy/dummy_formula_actor.py
-powerapi/formula/dummy/dummy_handlers.py
 powerapi/formula/simple/__init__.py
 powerapi/formula/simple/simple_formula_actor.py
 powerapi/formula/simple/simple_handlers.py
 powerapi/handler/__init__.py
 powerapi/handler/handler.py
 powerapi/handler/poison_pill_message_handler.py
 powerapi/handler/start_handler.py
```

### Comparing `powerapi-2.0.2/powerapi.egg-info/requires.txt` & `powerapi-2.0.3/powerapi.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `powerapi-2.0.2/pyproject.toml` & `powerapi-2.0.3/pyproject.toml`

 * *Files identical despite different names*

