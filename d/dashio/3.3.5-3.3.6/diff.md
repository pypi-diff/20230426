# Comparing `tmp/dashio-3.3.5.tar.gz` & `tmp/dashio-3.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dashio-3.3.5.tar", last modified: Wed Apr 19 06:24:43 2023, max compression
+gzip compressed data, was "dashio-3.3.6.tar", last modified: Wed Apr 26 04:43:05 2023, max compression
```

## Comparing `dashio-3.3.5.tar` & `dashio-3.3.6.tar`

### file list

```diff
@@ -1,84 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:24:43.550700 dashio-3.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-19 06:24:29.000000 dashio-3.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-04-19 06:24:43.550700 dashio-3.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-04-19 06:24:29.000000 dashio-3.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:24:43.534699 dashio-3.3.5/dashio/
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21460 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/action_station.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:24:43.534699 dashio-3.3.5/dashio/action_station_services/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/action_station_services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/action_station_services/action_station_service_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/action_station_services/as_servicel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/action_station_services/clock_servicel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/action_station_services/modbus_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/action_station_services/task_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/action_station_services/timer_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    16621 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/bleconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12852 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/dashconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)    22685 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:24:43.542700 dashio-3.3.5/dashio/iotcontrol/
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/alarm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/audio_visual_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/button_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    10583 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/color_picker.py
--rw-r--r--   0 runner    (1001) docker     (123)    14418 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/control.py
--rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/device_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     8762 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/dial.py
--rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/event_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/knob.py
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/label.py
--rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/ring_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    10443 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/slider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/textbox.py
--rw-r--r--   0 runner    (1001) docker     (123)    12106 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/iotcontrol/time_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9629 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/mqttconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/serialconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)    13036 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/tcpconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/zeroconf_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-04-19 06:24:29.000000 dashio-3.3.5/dashio/zmqconnection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:24:43.534699 dashio-3.3.5/dashio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-04-19 06:24:43.000000 dashio-3.3.5/dashio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-19 06:24:43.000000 dashio-3.3.5/dashio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 06:24:43.000000 dashio-3.3.5/dashio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 06:24:43.000000 dashio-3.3.5/dashio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-19 06:24:43.000000 dashio-3.3.5/dashio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 06:24:43.000000 dashio-3.3.5/dashio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-19 06:24:29.000000 dashio-3.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-19 06:24:43.550700 dashio-3.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-19 06:24:29.000000 dashio-3.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 06:24:43.550700 dashio-3.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_alarm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_button.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_button_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_control.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_dashconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_dashdevice.py
--rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_device_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_dial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_event_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_knob.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_mqttconntection.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_slider.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_tcpconnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_textbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_time_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 06:24:29.000000 dashio-3.3.5/tests/test_zqmconnection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 04:43:05.631092 dashio-3.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-26 04:42:55.000000 dashio-3.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-04-26 04:43:05.631092 dashio-3.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-04-26 04:42:55.000000 dashio-3.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 04:43:05.623092 dashio-3.3.6/dashio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21460 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/action_station.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 04:43:05.627092 dashio-3.3.6/dashio/action_station_services/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/action_station_services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/action_station_services/action_station_service_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/action_station_services/as_servicel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/action_station_services/clock_servicel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/action_station_services/modbus_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/action_station_services/task_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/action_station_services/timer_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16621 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/bleconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12853 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/dashconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22685 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 04:43:05.627092 dashio-3.3.6/dashio/iotcontrol/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/alarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/audio_visual_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/button_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10583 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/color_picker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14404 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/device_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8762 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/dial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/event_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/knob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/ring_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10443 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/textbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12106 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/iotcontrol/time_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/mqttconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/serialconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13036 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/tcpconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/zeroconf_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-04-26 04:42:55.000000 dashio-3.3.6/dashio/zmqconnection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 04:43:05.627092 dashio-3.3.6/dashio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-04-26 04:43:05.000000 dashio-3.3.6/dashio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-26 04:43:05.000000 dashio-3.3.6/dashio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 04:43:05.000000 dashio-3.3.6/dashio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 04:43:05.000000 dashio-3.3.6/dashio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-26 04:43:05.000000 dashio-3.3.6/dashio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 04:43:05.000000 dashio-3.3.6/dashio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-26 04:42:55.000000 dashio-3.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-26 04:43:05.631092 dashio-3.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-26 04:42:55.000000 dashio-3.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 04:43:05.631092 dashio-3.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_alarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_button_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_dashconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_dashdevice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_device_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_dial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_event_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_knob.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_mqttconntection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_tcpconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_textbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_time_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 04:42:55.000000 dashio-3.3.6/tests/test_zqmconnection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 04:43:05.631092 dashio-3.3.6/utilities/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1313 2023-04-26 04:42:55.000000 dashio-3.3.6/utilities/c64_decode
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1709 2023-04-26 04:42:55.000000 dashio-3.3.6/utilities/c64_encode
```

### Comparing `dashio-3.3.5/LICENSE` & `dashio-3.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/PKG-INFO` & `dashio-3.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dashio
-Version: 3.3.5
+Version: 3.3.6
 Summary: DashIO interface library
 Home-page: https://dashio.io
 Download-URL: https://github.com/dashio-connect/python-dashio
 Author: James Boulton
 Author-email: james@dashio.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `dashio-3.3.5/README.md` & `dashio-3.3.6/README.md`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/dashio/__init__.py` & `dashio-3.3.6/dashio/__init__.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/dashio/action_station.py` & `dashio-3.3.6/dashio/action_station.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/dashio/action_station_services/action_station_service_config.py` & `dashio-3.3.6/dashio/action_station_services/action_station_service_config.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/dashio/action_station_services/as_servicel.py` & `dashio-3.3.6/dashio/action_station_services/as_servicel.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/dashio/action_station_services/clock_servicel.py` & `dashio-3.3.6/dashio/action_station_services/clock_servicel.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/dashio/action_station_services/modbus_service.py` & `dashio-3.3.6/dashio/action_station_services/modbus_service.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/dashio/action_station_services/task_service.py` & `dashio-3.3.6/dashio/action_station_services/task_service.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/dashio/action_station_services/timer_service.py` & `dashio-3.3.6/dashio/action_station_services/timer_service.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/dashio/bleconnection.py` & `dashio-3.3.6/dashio/bleconnection.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/dashio/constants.py` & `dashio-3.3.6/dashio/constants.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/dashio/dashconnection.py` & `dashio-3.3.6/dashio/dashconnection.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 import paho.mqtt.client as mqtt
 import shortuuid
 import zmq
 
 from .constants import CONNECTION_PUB_URL
 from .iotcontrol.enums import ConnectionState
 
+
 class DashControl():
     """Class to stare dash connection info
     """
     def get_state(self) -> str:
         """Not used by this class as its a CFG only control
         """
         return ""
```

### Comparing `dashio-3.3.5/dashio/device.py` & `dashio-3.3.6/dashio/device.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/dashio/iotcontrol/__init__.py` & `dashio-3.3.6/dashio/iotcontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/dashio/iotcontrol/alarm.py` & `dashio-3.3.6/dashio/iotcontrol/alarm.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/dashio/iotcontrol/audio_visual_display.py` & `dashio-3.3.6/dashio/iotcontrol/audio_visual_display.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/dashio/iotcontrol/button.py` & `dashio-3.3.6/dashio/iotcontrol/button.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,14 +73,15 @@
             _get_color(cfg_dict.get("offColor", 'red')),
             cfg_dict.get("text", ""),
             ControlPosition(cfg_dict["xPositionRatio"], cfg_dict["yPositionRatio"], cfg_dict["widthRatio"], cfg_dict["heightRatio"])
         )
         tmp_cls.parent_id = cfg_dict["parentID"]
         return tmp_cls
 
+
 class Button(Control):
     """A Button control.
 
     Attributes
     ----------
     control_id : str
         An unique control identity string. The control identity string must be a unique string for each control per device
```

### Comparing `dashio-3.3.5/dashio/iotcontrol/button_group.py` & `dashio-3.3.6/dashio/iotcontrol/button_group.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/dashio/iotcontrol/chart.py` & `dashio-3.3.6/dashio/iotcontrol/chart.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/dashio/iotcontrol/color_picker.py` & `dashio-3.3.6/dashio/iotcontrol/color_picker.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/dashio/iotcontrol/control.py` & `dashio-3.3.6/dashio/iotcontrol/control.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 import json
-import logging
+
 from ..constants import BAD_CHARS
 from .enums import ColorPickerStyle, DeviceViewStyle, DialNumberPosition, DirectionStyle, ChartXAxisLabelsStyle,\
     Keyboard, KnobStyle, Precision, TextAlignment, TitlePosition, Icon, Color, TextFormat, LabelStyle, SliderBarStyle,\
     DialStyle, TimeGraphPositionOfKey, ButtonStyle, ButtonGroupStyle, MenuStyle
 from .event import Event
```

### Comparing `dashio-3.3.5/dashio/iotcontrol/device_view.py` & `dashio-3.3.6/dashio/iotcontrol/device_view.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/dashio/iotcontrol/dial.py` & `dashio-3.3.6/dashio/iotcontrol/dial.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/dashio/iotcontrol/direction.py` & `dashio-3.3.6/dashio/iotcontrol/direction.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/dashio/iotcontrol/enums.py` & `dashio-3.3.6/dashio/iotcontrol/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,14 @@
 
 class Icon(Enum):
     """
     All the Icons
     """
     NONE = "None"
     DOT = "Dot"
-    PAD = "Pad"
     UP = "Up"
     DOWN = "Down"
     LEFT = "Left"
     RIGHT = "Right"
     UP_LEFT = "Up Left"
     DOWN_LEFT = "Down Left"
     DOWN_RIGHT = "Down Right"
```

### Comparing `dashio-3.3.5/dashio/iotcontrol/event.py` & `dashio-3.3.6/dashio/iotcontrol/event.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/dashio/iotcontrol/event_log.py` & `dashio-3.3.6/dashio/iotcontrol/event_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 import dateutil.parser
 from ..constants import BAD_CHARS
 from .control import Control, ControlPosition, ControlConfig, _get_title_position
 from .enums import Color, TitlePosition
 from .ring_buffer import RingBuffer
 from .event import Event
 
+
 class EventData:
     """Event log data point
     """
     def __init__(self, lines: str, color=Color.WHITE):
         """EventLog data point
 
         Parameters
```

### Comparing `dashio-3.3.5/dashio/iotcontrol/knob.py` & `dashio-3.3.6/dashio/iotcontrol/knob.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/dashio/iotcontrol/label.py` & `dashio-3.3.6/dashio/iotcontrol/label.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/dashio/iotcontrol/map.py` & `dashio-3.3.6/dashio/iotcontrol/map.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 import json
 
 from ..constants import BAD_CHARS
 from .control import Control, ControlPosition, ControlConfig, _get_title_position
 from .enums import TitlePosition, Color
 from .event import Event
 
+
 class MapLocation:
     """
     A json version of a map location.
     """
     def __init__(self, latitude: str, longitude: str, average_speed=None, peak_speed=None, course=None, altitude=None, distance=None):
         """MapLocation
```

### Comparing `dashio-3.3.5/dashio/iotcontrol/menu.py` & `dashio-3.3.6/dashio/iotcontrol/menu.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/dashio/iotcontrol/ring_buffer.py` & `dashio-3.3.6/dashio/iotcontrol/ring_buffer.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/dashio/iotcontrol/selector.py` & `dashio-3.3.6/dashio/iotcontrol/selector.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/dashio/iotcontrol/slider.py` & `dashio-3.3.6/dashio/iotcontrol/slider.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/dashio/iotcontrol/textbox.py` & `dashio-3.3.6/dashio/iotcontrol/textbox.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/dashio/iotcontrol/time_graph.py` & `dashio-3.3.6/dashio/iotcontrol/time_graph.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/dashio/ip.py` & `dashio-3.3.6/dashio/ip.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/dashio/load_config.py` & `dashio-3.3.6/dashio/load_config.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/dashio/mqttconnection.py` & `dashio-3.3.6/dashio/mqttconnection.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 import shortuuid
 import zmq
 
 from .constants import CONNECTION_PUB_URL
 
 from .iotcontrol.enums import ConnectionState
 
+
 class MQTTConnection(threading.Thread):
     """Setups and manages a connection thread to the MQTT Server."""
 
     def _on_connect(self, client, userdata, flags, msg):
         if msg == 0:
             self._connection_state = ConnectionState.CONNECTED
             for device_id in self._device_id_list:
```

### Comparing `dashio-3.3.5/dashio/serialconnection.py` & `dashio-3.3.6/dashio/serialconnection.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/dashio/tcpconnection.py` & `dashio-3.3.6/dashio/tcpconnection.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/dashio/zeroconf_service.py` & `dashio-3.3.6/dashio/zeroconf_service.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/dashio/zmqconnection.py` & `dashio-3.3.6/dashio/zmqconnection.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/dashio.egg-info/PKG-INFO` & `dashio-3.3.6/dashio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dashio
-Version: 3.3.5
+Version: 3.3.6
 Summary: DashIO interface library
 Home-page: https://dashio.io
 Download-URL: https://github.com/dashio-connect/python-dashio
 Author: James Boulton
 Author-email: james@dashio.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `dashio-3.3.5/dashio.egg-info/SOURCES.txt` & `dashio-3.3.6/dashio.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -70,8 +70,10 @@
 tests/test_menu.py
 tests/test_mqttconntection.py
 tests/test_selector.py
 tests/test_slider.py
 tests/test_tcpconnection.py
 tests/test_textbox.py
 tests/test_time_graph.py
-tests/test_zqmconnection.py
+tests/test_zqmconnection.py
+utilities/c64_decode
+utilities/c64_encode
```

### Comparing `dashio-3.3.5/setup.cfg` & `dashio-3.3.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/tests/test_button.py` & `dashio-3.3.6/tests/test_button.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,13 +32,13 @@
     def test_button_set_text(self):
         test_control = Button("BUTTONID")
         test_control.text = "HELLO"
         self.assertEqual(test_control.get_state(), '\t{device_id}\tBTTN\tBUTTONID\tOFF\tNone\tHELLO\n', "text Should be Hello")
 
     def test_button_text_icon(self):
         test_control = Button("BUTTONID")
-        test_control.send_button(ButtonState.ON, Icon.PAD, "HELLO")
-        self.assertEqual(test_control.get_state(), '\t{device_id}\tBTTN\tBUTTONID\tON\tPad\tHELLO\n', "icon Should be Pad")
+        test_control.send_button(ButtonState.ON, Icon.SQUARE, "HELLO")
+        self.assertEqual(test_control.get_state(), '\t{device_id}\tBTTN\tBUTTONID\tON\tSquare\tHELLO\n', "icon Should be Square")
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `dashio-3.3.5/tests/test_button_group.py` & `dashio-3.3.6/tests/test_button_group.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/tests/test_chart.py` & `dashio-3.3.6/tests/test_chart.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/tests/test_dashdevice.py` & `dashio-3.3.6/tests/test_dashdevice.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/tests/test_device_view.py` & `dashio-3.3.6/tests/test_device_view.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/tests/test_dial.py` & `dashio-3.3.6/tests/test_dial.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/tests/test_direction.py` & `dashio-3.3.6/tests/test_direction.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/tests/test_event_log.py` & `dashio-3.3.6/tests/test_event_log.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/tests/test_knob.py` & `dashio-3.3.6/tests/test_knob.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/tests/test_label.py` & `dashio-3.3.6/tests/test_label.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/tests/test_map.py` & `dashio-3.3.6/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/tests/test_menu.py` & `dashio-3.3.6/tests/test_menu.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/tests/test_selector.py` & `dashio-3.3.6/tests/test_selector.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/tests/test_slider.py` & `dashio-3.3.6/tests/test_slider.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/tests/test_textbox.py` & `dashio-3.3.6/tests/test_textbox.py`

 * *Files identical despite different names*

### Comparing `dashio-3.3.5/tests/test_time_graph.py` & `dashio-3.3.6/tests/test_time_graph.py`

 * *Files identical despite different names*

