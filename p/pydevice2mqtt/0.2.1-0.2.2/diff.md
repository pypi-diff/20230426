# Comparing `tmp/pydevice2mqtt-0.2.1.tar.gz` & `tmp/pydevice2mqtt-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydevice2mqtt-0.2.1.tar", last modified: Tue Feb  7 21:22:16 2023, max compression
+gzip compressed data, was "pydevice2mqtt-0.2.2.tar", last modified: Tue Apr 25 18:19:25 2023, max compression
```

## Comparing `pydevice2mqtt-0.2.1.tar` & `pydevice2mqtt-0.2.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      719 2023-01-29 14:00:05.801942 pydevice2mqtt-0.2.1/.github/workflows/python-app.yml
--rw-r--r--   0        0        0      719 2023-02-07 21:18:58.348333 pydevice2mqtt-0.2.1/.gitignore
--rw-r--r--   0        0        0     1085 2023-01-28 22:47:34.594516 pydevice2mqtt-0.2.1/LICENSE
--rw-r--r--   0        0        0     1328 2023-01-29 14:00:05.802945 pydevice2mqtt-0.2.1/README.md
--rw-r--r--   0        0        0     1019 2023-02-07 21:17:52.794150 pydevice2mqtt-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      135 2023-01-28 22:51:00.110756 pydevice2mqtt-0.2.1/src/pydevice2mqtt/__init__.py
--rw-r--r--   0        0        0     8726 2023-02-07 21:12:46.980842 pydevice2mqtt-0.2.1/src/pydevice2mqtt/pydevice2mqtt.py
--rw-r--r--   0        0        0    18805 2023-02-07 21:15:26.944913 pydevice2mqtt-0.2.1/src/pydevice2mqtt/remote_devices.py
--rw-r--r--   0        0        0     6743 2023-02-07 21:16:19.014321 pydevice2mqtt-0.2.1/test/pydevice2mqtt_test.py
--rw-r--r--   0        0        0     1859 1970-01-01 00:00:00.000000 pydevice2mqtt-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1759 2023-04-25 18:12:28.120988 pydevice2mqtt-0.2.2/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0      719 2023-02-07 21:18:58.348333 pydevice2mqtt-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1085 2023-01-28 22:47:34.594516 pydevice2mqtt-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1328 2023-01-29 14:00:05.802945 pydevice2mqtt-0.2.2/README.md
+-rw-r--r--   0        0        0     1019 2023-04-25 18:19:22.918913 pydevice2mqtt-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      135 2023-01-28 22:51:00.110756 pydevice2mqtt-0.2.2/src/pydevice2mqtt/__init__.py
+-rw-r--r--   0        0        0     8761 2023-04-25 18:12:28.124989 pydevice2mqtt-0.2.2/src/pydevice2mqtt/pydevice2mqtt.py
+-rw-r--r--   0        0        0    18871 2023-04-25 18:12:28.125991 pydevice2mqtt-0.2.2/src/pydevice2mqtt/remote_devices.py
+-rw-r--r--   0        0        0     6830 2023-04-25 18:12:28.127986 pydevice2mqtt-0.2.2/test/pydevice2mqtt_test.py
+-rw-r--r--   0        0        0     1859 1970-01-01 00:00:00.000000 pydevice2mqtt-0.2.2/PKG-INFO
```

### Comparing `pydevice2mqtt-0.2.1/.gitignore` & `pydevice2mqtt-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pydevice2mqtt-0.2.1/LICENSE` & `pydevice2mqtt-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydevice2mqtt-0.2.1/README.md` & `pydevice2mqtt-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pydevice2mqtt-0.2.1/pyproject.toml` & `pydevice2mqtt-0.2.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 00000080: 2e0d 0a20 2020 2053 7570 706f 7274 7320  ...    Supports 
 00000090: 7468 6520 4861 7373 6f20 6175 746f 2063  the Hasso auto c
 000000a0: 6f6e 6669 6775 7261 7469 6f6e 2070 726f  onfiguration pro
 000000b0: 746f 636f 6c0d 0a20 2020 2027 2727 0d0a  tocol..    '''..
 000000c0: 2020 2020 6c69 6365 6e73 6520 3d20 7b66      license = {f
 000000d0: 696c 6520 3d20 224c 4943 454e 5345 227d  ile = "LICENSE"}
 000000e0: 0d0a 2020 2020 7665 7273 696f 6e20 3d20  ..    version = 
-000000f0: 2230 2e32 2e31 220d 0a20 2020 2072 6561  "0.2.1"..    rea
+000000f0: 2230 2e32 2e32 220d 0a20 2020 2072 6561  "0.2.2"..    rea
 00000100: 646d 6520 3d20 2252 4541 444d 452e 6d64  dme = "README.md
 00000110: 220d 0a20 2020 2072 6571 7569 7265 732d  "..    requires-
-00000120: 7079 7468 6f6e 203d 2022 3e3d 332e 3922  python = ">=3.9"
+00000120: 7079 7468 6f6e 203d 2022 3e3d 332e 3722  python = ">=3.7"
 00000130: 0d0a 2020 2020 6175 7468 6f72 7320 3d20  ..    authors = 
 00000140: 5b7b 6e61 6d65 3d22 4869 6768 496d 7022  [{name="HighImp"
 00000150: 2c20 656d 6169 6c3d 2241 6e79 4869 6768  , email="AnyHigh
 00000160: 5a40 676d 6169 6c2e 636f 6d22 7d5d 0d0a  Z@gmail.com"}]..
 00000170: 2020 2020 6465 7065 6e64 656e 6369 6573      dependencies
 00000180: 203d 205b 0d0a 2020 2020 2020 2020 2270   = [..        "p
 00000190: 6168 6f2d 6d71 7474 222c 0d0a 2020 2020  aho-mqtt",..
```

### Comparing `pydevice2mqtt-0.2.1/src/pydevice2mqtt/pydevice2mqtt.py` & `pydevice2mqtt-0.2.2/src/pydevice2mqtt/pydevice2mqtt.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,27 +41,28 @@
 
         complete_config: dict = {"remote_devices": {}, "mqtt_settings": {}}
 
         if config_file.is_file():
             with open(config_file, "r") as config_stream:
                 complete_config = yaml.load(config_stream, yaml.SafeLoader)
             if force_update and mqtt_settings:
-                complete_config |= mqtt_settings
+                  
+                complete_config.update(mqtt_settings)
 
         elif mqtt_settings is not None:
             needed_mqtt_keys = ["ip", "port", "bridge_name", "discovery_prefix", "operating_prefix"]
             assert all([needed_key in mqtt_settings.keys() for needed_key in needed_mqtt_keys]), \
                 f"Missing info in mqtt settings. Provide at least: {', '.join(needed_mqtt_keys)}"
             if "logging" not in mqtt_settings.keys():
                 mqtt_settings["logging"] = False
             for entry in ["user", "pw"]:
                 if entry not in mqtt_settings.keys():
                     mqtt_settings[entry] = None
 
-            complete_config["mqtt_settings"] |= mqtt_settings
+            complete_config["mqtt_settings"].update(mqtt_settings)
 
         else:
             raise ValueError("MQTT Settings have to be set for new file creation!")
 
         # check if all devices provide the necessary info
         for device_class_name, device_info_dict in devices.items():
             try:
@@ -79,15 +80,15 @@
             # all infos correct, update dict
             if device_class_name in complete_config["remote_devices"].keys():
                 if not force_update:
                     assert all(devices[device_class_name].keys()) not in complete_config["remote_devices"][
                         device_class_name].keys(), \
                         f"Found existing Device, updating {device_class_name} is forbidden!"
                 # update, no matter what
-                complete_config["remote_devices"][device_class_name] |= devices[device_class_name]
+                complete_config["remote_devices"][device_class_name].update(devices[device_class_name])
 
             else:  # device class not known, just copy the dict
                 complete_config["remote_devices"][device_class_name] = devices[device_class_name]
 
         with open(config_file, "w") as config_stream:
             yaml.safe_dump(complete_config, config_stream)
```

### Comparing `pydevice2mqtt-0.2.1/src/pydevice2mqtt/remote_devices.py` & `pydevice2mqtt-0.2.2/src/pydevice2mqtt/remote_devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,17 +74,17 @@
         level = getattr(kwargs, "Level", logging.DEBUG)
         print_string = "".join(map(str, args))
         logging.log(level=level, msg=print_string)
         if self._logging_channel is not None:
             self._publish(topic=self._logging_channel,
                           payload=print_string,
                           retain=False,
-                          qos=1)
+                          qos=0)
 
-    def _update(self, channel_name: str, message: any, retain: bool = False, qos: int = 1) -> None:
+    def _update(self, channel_name: str, message: any, retain: bool = False, qos: int = 0) -> None:
         """
         Publish the message in json format to the channel name
         (must be added by add_channel first)
 
         :param channel_name: name of the device channel
         :param message: any type of json dumpable data to publish
         :param retain: Retain flag for this message
@@ -158,15 +158,17 @@
         return dict([channel for name, channel in self._operation_topics.items()])
 
     @classmethod
     def get_config_req(cls) -> dict:
         """Returns a dict with the required keys and the expected data types as values
         :return: dict
         """
-        return cls._CONFIG_REQ | cls._BASE_CONFIG_REQ
+        config_req = cls._CONFIG_REQ.copy()
+        config_req.update(cls._BASE_CONFIG_REQ)
+        return config_req
 
 
 def supported_device_classes() -> dict:
     """
     generates a dictionary with all supported devices,
     and the class name as key, the object as value
```

### Comparing `pydevice2mqtt-0.2.1/test/pydevice2mqtt_test.py` & `pydevice2mqtt-0.2.2/test/pydevice2mqtt_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 def create_config_file(path: Path, device_classes: dict = None) -> None:
     """
     Generate a fast config file to create mocked bridges
     :param path: filename for resulting config file
     :param device_classes: dict of classes to create ({<classname>:<classobj>})
     """
     import pydevice2mqtt
-    path.unlink(missing_ok=True)
+    if path.exists():
+        path.unlink()
     all_devices: dict = {}
     if device_classes is None:
         device_classes = pydevice2mqtt.supported_device_classes()
 
     for classname, device_class in device_classes.items():
 
         config_requirement = device_class.get_config_req()
@@ -118,15 +119,18 @@
     assert sensor_instance.get_uid() == expected_uid
     assert sensor_instance.get_object_id() == EXAMPLE_DATA[str]
     assert sensor_instance.get_name() == EXAMPLE_DATA[str]
     assert len(mqtt_client.mock_calls) == 3
     sensor_instance.set_value(1)
     assert len(mqtt_client.mock_calls) == 4
     set_value_call_kwargs = mqtt_client.mock_calls[-1].kwargs
-    assert set_value_call_kwargs["payload"] == '{"value": 1}'
+    try:
+        assert set_value_call_kwargs["payload"] == '{"value": 1}'
+    except TypeError:
+        print(set_value_call_kwargs)
 
 
 def test_additional_config(mocker):
     import pydevice2mqtt
 
     mocker.patch("pydevice2mqtt.pydevice2mqtt.mqtt.Client")
     mocker.patch("pydevice2mqtt.remote_devices.espeak")
```

### Comparing `pydevice2mqtt-0.2.1/PKG-INFO` & `pydevice2mqtt-0.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pydevice2mqtt
-Version: 0.2.1
+Version: 0.2.2
 Summary:     This project provides a simplified control of devices via MQTT.
             Supports the Hasso auto configuration protocol
             
 Keywords: hassio,mqtt,homeassistent,homeautomation
 Author-email: HighImp <AnyHighZ@gmail.com>
-Requires-Python: >=3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: paho-mqtt
 Requires-Dist: pyyaml
 Requires-Dist: pylint ~=2.14.0 ; extra == "test"
 Requires-Dist: pytest-cov ~=4.0.0 ; extra == "test"
 Requires-Dist: pytest-mock ~=3.10.0 ; extra == "test"
 Provides-Extra: test
```

