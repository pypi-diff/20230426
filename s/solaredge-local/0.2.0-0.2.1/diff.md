# Comparing `tmp/solaredge_local-0.2.0.tar.gz` & `tmp/solaredge_local-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/solaredge_local-0.2.0.tar", last modified: Fri May 24 13:16:19 2019, max compression
+gzip compressed data, was "solaredge_local-0.2.1.tar", last modified: Wed Apr 26 15:08:52 2023, max compression
```

## Comparing `solaredge_local-0.2.0.tar` & `solaredge_local-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 drob      (1000) drob      (1000)        0 2019-05-24 13:16:19.000000 solaredge_local-0.2.0/
--rw-r--r--   0 drob      (1000) drob      (1000)     9205 2019-05-24 13:16:19.000000 solaredge_local-0.2.0/PKG-INFO
--rw-r--r--   0 drob      (1000) drob      (1000)     7525 2019-05-24 13:10:03.000000 solaredge_local-0.2.0/README.md
--rw-r--r--   0 drob      (1000) drob      (1000)       38 2019-05-24 13:16:19.000000 solaredge_local-0.2.0/setup.cfg
--rw-r--r--   0 drob      (1000) drob      (1000)     1357 2019-05-24 13:14:44.000000 solaredge_local-0.2.0/setup.py
-drwxr-xr-x   0 drob      (1000) drob      (1000)        0 2019-05-24 13:16:19.000000 solaredge_local-0.2.0/solaredge_local/
--rw-rw-r--   0 drob      (1000) drob      (1000)       49 2019-04-01 00:15:01.000000 solaredge_local-0.2.0/solaredge_local/__init__.py
--rw-r--r--   0 drob      (1000) drob      (1000)    11981 2019-05-24 13:10:03.000000 solaredge_local-0.2.0/solaredge_local/information_pb2.py
--rw-r--r--   0 drob      (1000) drob      (1000)    34211 2019-05-22 12:57:30.000000 solaredge_local-0.2.0/solaredge_local/maintenance_pb2.py
--rw-r--r--   0 drob      (1000) drob      (1000)    77718 2019-05-24 13:10:03.000000 solaredge_local-0.2.0/solaredge_local/powercontrol_pb2.py
--rw-r--r--   0 drob      (1000) drob      (1000)      664 2019-05-24 13:10:03.000000 solaredge_local-0.2.0/solaredge_local/solaredge.py
--rw-r--r--   0 drob      (1000) drob      (1000)    42571 2019-05-22 12:57:30.000000 solaredge_local-0.2.0/solaredge_local/status_pb2.py
-drwxr-xr-x   0 drob      (1000) drob      (1000)        0 2019-05-24 13:16:19.000000 solaredge_local-0.2.0/solaredge_local.egg-info/
--rw-rw-r--   0 drob      (1000) drob      (1000)     9205 2019-05-24 13:16:18.000000 solaredge_local-0.2.0/solaredge_local.egg-info/PKG-INFO
--rw-rw-r--   0 drob      (1000) drob      (1000)      405 2019-05-24 13:16:19.000000 solaredge_local-0.2.0/solaredge_local.egg-info/SOURCES.txt
--rw-rw-r--   0 drob      (1000) drob      (1000)        1 2019-05-24 13:16:18.000000 solaredge_local-0.2.0/solaredge_local.egg-info/dependency_links.txt
--rw-rw-r--   0 drob      (1000) drob      (1000)       23 2019-05-24 13:16:18.000000 solaredge_local-0.2.0/solaredge_local.egg-info/requires.txt
--rw-rw-r--   0 drob      (1000) drob      (1000)       16 2019-05-24 13:16:18.000000 solaredge_local-0.2.0/solaredge_local.egg-info/top_level.txt
+drwxrwxr-x   0 drob      (1000) drob      (1000)        0 2023-04-26 15:08:52.768911 solaredge_local-0.2.1/
+-rw-rw-r--   0 drob      (1000) drob      (1000)     8972 2023-04-26 15:08:52.768911 solaredge_local-0.2.1/PKG-INFO
+-rw-rw-r--   0 drob      (1000) drob      (1000)     8375 2023-04-26 14:20:16.000000 solaredge_local-0.2.1/README.md
+-rw-rw-r--   0 drob      (1000) drob      (1000)       38 2023-04-26 15:08:52.768911 solaredge_local-0.2.1/setup.cfg
+-rw-rw-r--   0 drob      (1000) drob      (1000)     1357 2023-04-26 14:33:57.000000 solaredge_local-0.2.1/setup.py
+drwxrwxr-x   0 drob      (1000) drob      (1000)        0 2023-04-26 15:08:52.768911 solaredge_local-0.2.1/solaredge_local/
+-rw-rw-r--   0 drob      (1000) drob      (1000)       49 2023-04-26 14:20:16.000000 solaredge_local-0.2.1/solaredge_local/__init__.py
+-rw-rw-r--   0 drob      (1000) drob      (1000)     2240 2023-04-26 14:20:16.000000 solaredge_local-0.2.1/solaredge_local/information_pb2.py
+-rw-rw-r--   0 drob      (1000) drob      (1000)     5145 2023-04-26 14:20:16.000000 solaredge_local-0.2.1/solaredge_local/maintenance_pb2.py
+-rw-rw-r--   0 drob      (1000) drob      (1000)    12142 2023-04-26 14:20:16.000000 solaredge_local-0.2.1/solaredge_local/powercontrol_pb2.py
+-rw-rw-r--   0 drob      (1000) drob      (1000)      664 2023-04-26 14:20:16.000000 solaredge_local-0.2.1/solaredge_local/solaredge.py
+-rw-rw-r--   0 drob      (1000) drob      (1000)     6161 2023-04-26 14:20:16.000000 solaredge_local-0.2.1/solaredge_local/status_pb2.py
+drwxrwxr-x   0 drob      (1000) drob      (1000)        0 2023-04-26 15:08:52.768911 solaredge_local-0.2.1/solaredge_local.egg-info/
+-rw-rw-r--   0 drob      (1000) drob      (1000)     8972 2023-04-26 15:08:52.000000 solaredge_local-0.2.1/solaredge_local.egg-info/PKG-INFO
+-rw-rw-r--   0 drob      (1000) drob      (1000)      405 2023-04-26 15:08:52.000000 solaredge_local-0.2.1/solaredge_local.egg-info/SOURCES.txt
+-rw-rw-r--   0 drob      (1000) drob      (1000)        1 2023-04-26 15:08:52.000000 solaredge_local-0.2.1/solaredge_local.egg-info/dependency_links.txt
+-rw-rw-r--   0 drob      (1000) drob      (1000)       23 2023-04-26 15:08:52.000000 solaredge_local-0.2.1/solaredge_local.egg-info/requires.txt
+-rw-rw-r--   0 drob      (1000) drob      (1000)       16 2023-04-26 15:08:52.000000 solaredge_local-0.2.1/solaredge_local.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `solaredge_local-0.2.0/PKG-INFO` & `solaredge_local-0.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,152 +1,161 @@
 Metadata-Version: 2.1
 Name: solaredge_local
-Version: 0.2.0
+Version: 0.2.1
 Summary: API wrapper to communicate locally with SolarEdge Inverters
 Home-page: https://github.com/drobtravels/solaredge-local
 Author: David Roberts
 Author-email: 
 License: MIT License
-Description: # SolarEdge Local
-        
-        The goal if this respository is to provide information about using the local API available on some solar edge inverters.  This is a WIP based on my observations and may contain inaccuracies.  Pull Requests or Issues are encouraged to correct any mistakes or add additonal informatoin.
-        
-        ### Relevant Models
-        
-        The local API is available on the [SExxxxH-US models with SetApp](https://www.solaredge.com/sites/default/files/se-hd-wave-single-phase-inverter-with-setapp-datasheet-na.pdf) as well as European three phase inverters SEXXK-XXXTXBXX4 models with SetApp like [SE3K-E10K](https://www.solaredge.com/sites/default/files/se-three-phase-inverter-setapp-ds.pdf), [SE12.5K-SE27.6K](https://www.solaredge.com/sites/default/files/se-three-phase-inverter-setapp-datasheet.pdf) and [SE33.3K](https://www.solaredge.com/sites/default/files/se-three-phase-inverter-for-277-480-grid-setapp-datasheet.pdf).
-        Please check carefully the datasheets if in the section "Additional Features", sub-section "Inverter Commissioning" is present the following line "With the SetApp mobile application using built-in Wi-Fi access point for local connection".
-        
-        More inforation on SeeApp could be found [here](https://www.solaredge.com/us/products/installer-tools/setapp). These models have no LED screen and are provisioned ONLY via a phone app during commissioning.
-        Check also the [SetApp FAQ](https://www.solaredge.com/sites/default/files/solaredge-setapp-faqs-eng.pdf) for more info.
-        For convenience it is reported here one Q&A:
-        
-        > Q: Can the new app be used for already installed inverters?
-        >
-        > A: Only SolarEdge inverters with a new communication board (no display) can be activated or configured via SetApp.
-        
-        Reportedly, these new inverters have a CPU number starting with 04.
-        
-        You can check by finding the IP address of your inverter and visiting it in a browser.  If it supports the local API, you'll see the SolarEdge logo and a "Commissioning" menu.
-        
-        If you do not have the local API available, see [this repository](https://github.com/jbuehl/solaredge) as an alternative.
-        
-        ### Using the Python wrapper
-        
-        For convinience, a python API wrapper, [solaredge_local](https://pypi.org/project/solaredge-local/) is available.  **Only python 3 is supported**
-        
-        To install: `pip install solaredge-local`
-        
-        To use:
-        
-        ```
-        from solaredge_local import SolarEdge
-        client = SolarEdge("http://<inverter ip address>")
-        client.get_status()  # Provides general energy and other overview information
-        client.get_maintenance() # Provides optimizer level information and other details
-        client.get_information() # Provides software versions and error log list.
-        client.get_power_control() # Provides power control information and other details.
-        ```
-        
-        ### API Endpoints
-        
-        * AppConfigs: "web/v1/app_configs"
-        * Region: "web/v1/region"
-        * Region_Country: "web/v1/region/country"
-        * Region_Language: "web/v1/region/language"
-        * Pairing: "web/v1/pairing"
-        * Pairing_Request: "web/v1/pairing/request"
-        * Communication: "web/v1/communication"
-        * Communication_Server: "web/v1/communication/server"
-        * Communication_Lan: "web/v1/communication/lan"
-        * Communication_Rs485_SlaveDetect: "web/v1/communication/rs485/<id>/slave_detect"
-        * Communication_Rs485_Protocol: "web/v1/communication/rs485/<id>/protocol"
-        * Communication_Rs485_DeviceId: "web/v1/communication/rs485/<id>/deviceid"
-        * Communication_Rs485_Modbus: "web/v1/communication/rs485/<id>/modbus"
-        * Communication_Rs485_Modbus_AddDevice: "web/v1/communication/rs485/<id>/modbus/add_device"
-        * Communication_Rs485_Modbus_RemoveDevice: "web/v1/communication/rs485/<id>/modbus/remove_device"
-        * Communication_Wifi: "web/v1/communication/wifi"
-        * Communication_Wifi_Wps: "web/v1/communication/wifi/wps"
-        * Communication_Wifi_Connect: "web/v1/communication/wifi/connect"
-        * Communication_Cellular: "web/v1/communication/cellular"
-        * Communication_Zigbee_Defaults: "web/v1/communication/zigbee/defaults"
-        * Communication_Zigbee_ModuleConfigs: "web/v1/communication/zigbee/module_configs"
-        * Communication_Zigbee_OpMode: "web/v1/communication/zigbee/op_mode"
-        * Communication_Gpio_Pri: "web/v1/communication/gpio/pri"
-        * Communication_ModbusTcp: "web/v1/communication/modbus_tcp"
-        * PowerControl: "web/v1/power_control"
-        * PowerControl_GridControl: "web/v1/power_control/grid_control"
-        * PowerControl_EnergyManager_LimitControl: "web/v1/power_control/energy_manager/limit_control"
-        * PowerControl_EnergyManager_EnergyControl: "web/v1/power_control/energy_manager/energy_control"
-        * PowerControl_EnergyManager_StorageControl: "web/v1/power_control/energy_manager/storage_control"
-        * PowerControl_ReactivePower: "web/v1/power_control/reactive_power"
-        * PowerControl_ActivePower: "web/v1/power_control/active_power"
-        * PowerControl_Wakeup: "web/v1/power_control/wakeup"
-        * PowerControl_Advanced: "web/v1/power_control/advanced"
-        * PowerControl_Reset: "web/v1/power_control/reset"
-        * PowerControl_Rrcr: "web/v1/power_control/rrcr"
-        * Maintenance: "web/v1/maintenance"
-        * Maintenance_DateTime: "web/v1/maintenance/date_and_time"
-        * Maintenance_ResetCounters: "web/v1/maintenance/reset_counters"
-        * Maintenance_ResetFactory: "web/v1/maintenance/reset_factory"
-        * Maintenance_Afci: "web/v1/maintenance/afci"
-        * Maintenance_AfciTest: "web/v1/maintenance/afci/test"
-        * Maintenance_Inverters_SelfTest: "web/v1/maintenance/inverters/<position>/self_test"
-        * Maintenance_Standby: "web/v1/maintenance/standby"
-        * Maintenance_GridProtectionLogin: "web/v1/maintenance/grid_protection/login"
-        * Maintenance_GridProtection: "web/v1/maintenance/grid_protection"
-        * Maintenance_UpgradeUsb: "web/v1/maintenance/fw_upgrade/usb"
-        * Information: "web/v1/information"
-        * Status: "web/v1/status"
-        * Status_ServerCommTest: "web/v1/status/server_comm_test"
-        
-        The Status endpoint appears to the most useful for realtime production data.
-        Optimizer level data is available from the maintenance API endpoint.
-        
-        
-        ## Using the API
-        
-        All endpoints I have explored so far appear to be a GET, and responses use [Protocol Buffers](https://developers.google.com/protocol-buffers/).  There is no authentication
-        
-        ### View Raw Response
-        
-        You can see the raw data by doing the following (assuming you have the protoocal buffers CLI tool installed)
-        
-        ```
-        curl -s http://<inverter ip>/web/v1/status | protoc --decode_raw
-        ```
-        
-        Many numbers appear to be 32 bit floating point.
-        
-        The proto definitions required to fully parse the responses are available in  javascript if you choose "view source" in the developer tools of your browser.
-        
-        ### View Parsed response
-        
-        If there is a corresponding `.proto` file in [message_types](/message_types), you can view the parsed response from the API.  Each proto file correspond to the name of an API endpoint. These are very much a WIP and may be incomplete.  These can be created by choosing "view source" in the developer tools of your browser, and searching for text like `proto.web_status.<apiNameInCamelCase>.toObject`
-        
-        Here is an example for the status API:
-        
-        ```
-        curl -s http://<inverter ip>/web/v1/status | protoc --decode Status message_types/status.proto
-        ```
-        
-        ### Updating Protocol Buffer response
-        
-        To add or change the Protocol Buffer defintions, please do the following
-        
-        1. Manually change the `message_types/*.proto` files as required
-        2. Test the file using `curl` as described in [View Parsed Response](#view-parsed-response)
-        3. Update the generated `*_pb2.py` files for each file changed by running a command like:
-        
-            ```
-            protoc -I=message_types --python_out=solaredge_local message_types/<filename_changed>.proto
-            ```
-        4. Commit the generated updates
-        
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
+
+# SolarEdge Local
+
+**Warning**
+
+Recent firmware versions disable local access.  Some units may continue to work, but many users are reporting it is no longer available.  See [this issue](https://github.com/jbuehl/solaredge/issues/124) and [this issue](https://github.com/drobtravels/solaredge-local/issues/24) for additional details.  Please check if you can access your inverter via a web browser before attempting to use this library.
+
+
+The goal if this respository is to provide information about using the local API available on some solar edge inverters.  This is a WIP based on my observations and may contain inaccuracies.  Pull Requests or Issues are encouraged to correct any mistakes or add additonal informatoin.
+
+### Relevant Models
+
+The fastest way to check your inverter will support this library and to enter the IP address of your inverter in the browser and see if the administration page is displayed.
+
+The local API is available for specific firmware versions running on [SExxxxH-US models with SetApp](https://www.solaredge.com/sites/default/files/se-hd-wave-single-phase-inverter-with-setapp-datasheet-na.pdf) as well as European three phase inverters SEXXK-XXXTXBXX4 models with SetApp like [SE3K-E10K](https://www.solaredge.com/sites/default/files/se-three-phase-inverter-setapp-ds.pdf), [SE12.5K-SE27.6K](https://www.solaredge.com/sites/default/files/se-three-phase-inverter-setapp-datasheet.pdf) and [SE33.3K](https://www.solaredge.com/sites/default/files/se-three-phase-inverter-for-277-480-grid-setapp-datasheet.pdf). Same goes for Australian inverters [SE2500H->SE10000H](https://www.solaredge.com/sites/default/files/se-single-phase-HD-wave-inverter-setapp-datasheet-aus.pdf). 
+Please check carefully the datasheets if in the section "Additional Features", sub-section "Inverter Commissioning" is present the following line "With the SetApp mobile application using built-in Wi-Fi access point for local connection".  You should 
+
+More inforation on SetApp could be found [here](https://www.solaredge.com/us/products/installer-tools/setapp). These models have no LED screen and are provisioned ONLY via a phone app during commissioning.
+Check also the [SetApp FAQ](https://www.solaredge.com/sites/default/files/solaredge-setapp-faqs-eng.pdf) for more info.
+For convenience it is reported here one Q&A:
+
+> Q: Can the new app be used for already installed inverters?
+>
+> A: Only SolarEdge inverters with a new communication board (no display) can be activated or configured via SetApp.
+
+These new inverters have a [CPU number](https://www.solaredge.com/setapp-inverters-firmware) starting with 04.
+
+You can check by finding the IP address of your inverter and visiting it in a browser.  If it supports the local API, you'll see the SolarEdge logo and a "Commissioning" menu.
+
+If you do not have the local API available, see [this repository](https://github.com/jbuehl/solaredge) as an alternative.
+
+### Using the Python wrapper
+
+For convinience, a python API wrapper, [solaredge_local](https://pypi.org/project/solaredge-local/) is available.  **Only python 3 is supported**
+
+To install: `pip3 install solaredge-local`
+
+To use:
+
+```
+from solaredge_local import SolarEdge
+client = SolarEdge("http://<inverter ip address>")
+client.get_status()  # Provides general energy and other overview information
+client.get_maintenance() # Provides optimizer level information and other details
+client.get_information() # Provides software versions and error log list.
+client.get_power_control() # Provides power control information and other details.
+```
+
+### API Endpoints
+
+* AppConfigs: "web/v1/app_configs"
+* Region: "web/v1/region"
+* Region_Country: "web/v1/region/country"
+* Region_Language: "web/v1/region/language"
+* Pairing: "web/v1/pairing"
+* Pairing_Request: "web/v1/pairing/request"
+* Communication: "web/v1/communication"
+* Communication_Server: "web/v1/communication/server"
+* Communication_Lan: "web/v1/communication/lan"
+* Communication_Rs485_SlaveDetect: "web/v1/communication/rs485/<id>/slave_detect"
+* Communication_Rs485_Protocol: "web/v1/communication/rs485/<id>/protocol"
+* Communication_Rs485_DeviceId: "web/v1/communication/rs485/<id>/deviceid"
+* Communication_Rs485_Modbus: "web/v1/communication/rs485/<id>/modbus"
+* Communication_Rs485_Modbus_AddDevice: "web/v1/communication/rs485/<id>/modbus/add_device"
+* Communication_Rs485_Modbus_RemoveDevice: "web/v1/communication/rs485/<id>/modbus/remove_device"
+* Communication_Wifi: "web/v1/communication/wifi"
+* Communication_Wifi_Wps: "web/v1/communication/wifi/wps"
+* Communication_Wifi_Connect: "web/v1/communication/wifi/connect"
+* Communication_Cellular: "web/v1/communication/cellular"
+* Communication_Zigbee_Defaults: "web/v1/communication/zigbee/defaults"
+* Communication_Zigbee_ModuleConfigs: "web/v1/communication/zigbee/module_configs"
+* Communication_Zigbee_OpMode: "web/v1/communication/zigbee/op_mode"
+* Communication_Gpio_Pri: "web/v1/communication/gpio/pri"
+* Communication_ModbusTcp: "web/v1/communication/modbus_tcp"
+* PowerControl: "web/v1/power_control"
+* PowerControl_GridControl: "web/v1/power_control/grid_control"
+* PowerControl_EnergyManager_LimitControl: "web/v1/power_control/energy_manager/limit_control"
+* PowerControl_EnergyManager_EnergyControl: "web/v1/power_control/energy_manager/energy_control"
+* PowerControl_EnergyManager_StorageControl: "web/v1/power_control/energy_manager/storage_control"
+* PowerControl_ReactivePower: "web/v1/power_control/reactive_power"
+* PowerControl_ActivePower: "web/v1/power_control/active_power"
+* PowerControl_Wakeup: "web/v1/power_control/wakeup"
+* PowerControl_Advanced: "web/v1/power_control/advanced"
+* PowerControl_Reset: "web/v1/power_control/reset"
+* PowerControl_Rrcr: "web/v1/power_control/rrcr"
+* Maintenance: "web/v1/maintenance"
+* Maintenance_DateTime: "web/v1/maintenance/date_and_time"
+* Maintenance_ResetCounters: "web/v1/maintenance/reset_counters"
+* Maintenance_ResetFactory: "web/v1/maintenance/reset_factory"
+* Maintenance_Afci: "web/v1/maintenance/afci"
+* Maintenance_AfciTest: "web/v1/maintenance/afci/test"
+* Maintenance_Inverters_SelfTest: "web/v1/maintenance/inverters/<position>/self_test"
+* Maintenance_Standby: "web/v1/maintenance/standby"
+* Maintenance_GridProtectionLogin: "web/v1/maintenance/grid_protection/login"
+* Maintenance_GridProtection: "web/v1/maintenance/grid_protection"
+* Maintenance_UpgradeUsb: "web/v1/maintenance/fw_upgrade/usb"
+* Information: "web/v1/information"
+* Status: "web/v1/status"
+* Status_ServerCommTest: "web/v1/status/server_comm_test"
+
+The Status endpoint appears to the most useful for realtime production data.
+Optimizer level data is available from the Maintenance API endpoint.
+
+
+## Using the API
+
+All endpoints I have explored so far appear to be a GET, and responses use [Protocol Buffers](https://developers.google.com/protocol-buffers/).  There is no authentication.
+
+### View Raw Response
+
+You can see the raw data by doing the following (assuming you have the protoocal buffers CLI tool installed)
+
+```
+curl -s http://<inverter ip>/web/v1/status | protoc --decode_raw
+```
+
+Many numbers appear to be 32 bit floating point.
+
+The proto definitions required to fully parse the responses are available in  javascript if you choose "view source" in the developer tools of your browser.
+
+### View Parsed response
+
+If there is a corresponding `.proto` file in [message_types](/message_types), you can view the parsed response from the API.  Each proto file correspond to the name of an API endpoint. These are very much a WIP and may be incomplete.  These can be created by choosing "view source" in the developer tools of your browser, and searching for text like `proto.web_status.<apiNameInCamelCase>.toObject`
+
+Here is an example for the status API:
+
+```
+curl -s http://<inverter ip>/web/v1/status | protoc --decode Status message_types/status.proto
+```
+
+### Updating Protocol Buffer response
+
+To add or change the Protocol Buffer defintions, please do the following
+
+1. Manually change the `message_types/*.proto` files as required
+2. Test the file using `curl` as described in [View Parsed Response](#view-parsed-response)
+3. Update the generated `*_pb2.py` files for each file changed by running a command like:
+
+    ```
+    protoc -I=message_types --python_out=solaredge_local message_types/<filename_changed>.proto
+    ```
+4. Commit the generated updates
+
+
```

### Comparing `solaredge_local-0.2.0/README.md` & `solaredge_local-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 # SolarEdge Local
 
+**Warning**
+
+Recent firmware versions disable local access.  Some units may continue to work, but many users are reporting it is no longer available.  See [this issue](https://github.com/jbuehl/solaredge/issues/124) and [this issue](https://github.com/drobtravels/solaredge-local/issues/24) for additional details.  Please check if you can access your inverter via a web browser before attempting to use this library.
+
+
 The goal if this respository is to provide information about using the local API available on some solar edge inverters.  This is a WIP based on my observations and may contain inaccuracies.  Pull Requests or Issues are encouraged to correct any mistakes or add additonal informatoin.
 
 ### Relevant Models
 
-The local API is available on the [SExxxxH-US models with SetApp](https://www.solaredge.com/sites/default/files/se-hd-wave-single-phase-inverter-with-setapp-datasheet-na.pdf) as well as European three phase inverters SEXXK-XXXTXBXX4 models with SetApp like [SE3K-E10K](https://www.solaredge.com/sites/default/files/se-three-phase-inverter-setapp-ds.pdf), [SE12.5K-SE27.6K](https://www.solaredge.com/sites/default/files/se-three-phase-inverter-setapp-datasheet.pdf) and [SE33.3K](https://www.solaredge.com/sites/default/files/se-three-phase-inverter-for-277-480-grid-setapp-datasheet.pdf).
-Please check carefully the datasheets if in the section "Additional Features", sub-section "Inverter Commissioning" is present the following line "With the SetApp mobile application using built-in Wi-Fi access point for local connection".
+The fastest way to check your inverter will support this library and to enter the IP address of your inverter in the browser and see if the administration page is displayed.
+
+The local API is available for specific firmware versions running on [SExxxxH-US models with SetApp](https://www.solaredge.com/sites/default/files/se-hd-wave-single-phase-inverter-with-setapp-datasheet-na.pdf) as well as European three phase inverters SEXXK-XXXTXBXX4 models with SetApp like [SE3K-E10K](https://www.solaredge.com/sites/default/files/se-three-phase-inverter-setapp-ds.pdf), [SE12.5K-SE27.6K](https://www.solaredge.com/sites/default/files/se-three-phase-inverter-setapp-datasheet.pdf) and [SE33.3K](https://www.solaredge.com/sites/default/files/se-three-phase-inverter-for-277-480-grid-setapp-datasheet.pdf). Same goes for Australian inverters [SE2500H->SE10000H](https://www.solaredge.com/sites/default/files/se-single-phase-HD-wave-inverter-setapp-datasheet-aus.pdf). 
+Please check carefully the datasheets if in the section "Additional Features", sub-section "Inverter Commissioning" is present the following line "With the SetApp mobile application using built-in Wi-Fi access point for local connection".  You should 
 
-More inforation on SeeApp could be found [here](https://www.solaredge.com/us/products/installer-tools/setapp). These models have no LED screen and are provisioned ONLY via a phone app during commissioning.
+More inforation on SetApp could be found [here](https://www.solaredge.com/us/products/installer-tools/setapp). These models have no LED screen and are provisioned ONLY via a phone app during commissioning.
 Check also the [SetApp FAQ](https://www.solaredge.com/sites/default/files/solaredge-setapp-faqs-eng.pdf) for more info.
 For convenience it is reported here one Q&A:
 
 > Q: Can the new app be used for already installed inverters?
 >
 > A: Only SolarEdge inverters with a new communication board (no display) can be activated or configured via SetApp.
 
-Reportedly, these new inverters have a CPU number starting with 04.
+These new inverters have a [CPU number](https://www.solaredge.com/setapp-inverters-firmware) starting with 04.
 
 You can check by finding the IP address of your inverter and visiting it in a browser.  If it supports the local API, you'll see the SolarEdge logo and a "Commissioning" menu.
 
 If you do not have the local API available, see [this repository](https://github.com/jbuehl/solaredge) as an alternative.
 
 ### Using the Python wrapper
 
 For convinience, a python API wrapper, [solaredge_local](https://pypi.org/project/solaredge-local/) is available.  **Only python 3 is supported**
 
-To install: `pip install solaredge-local`
+To install: `pip3 install solaredge-local`
 
 To use:
 
 ```
 from solaredge_local import SolarEdge
 client = SolarEdge("http://<inverter ip address>")
 client.get_status()  # Provides general energy and other overview information
@@ -87,20 +94,20 @@
 * Maintenance_GridProtection: "web/v1/maintenance/grid_protection"
 * Maintenance_UpgradeUsb: "web/v1/maintenance/fw_upgrade/usb"
 * Information: "web/v1/information"
 * Status: "web/v1/status"
 * Status_ServerCommTest: "web/v1/status/server_comm_test"
 
 The Status endpoint appears to the most useful for realtime production data.
-Optimizer level data is available from the maintenance API endpoint.
+Optimizer level data is available from the Maintenance API endpoint.
 
 
 ## Using the API
 
-All endpoints I have explored so far appear to be a GET, and responses use [Protocol Buffers](https://developers.google.com/protocol-buffers/).  There is no authentication
+All endpoints I have explored so far appear to be a GET, and responses use [Protocol Buffers](https://developers.google.com/protocol-buffers/).  There is no authentication.
 
 ### View Raw Response
 
 You can see the raw data by doing the following (assuming you have the protoocal buffers CLI tool installed)
 
 ```
 curl -s http://<inverter ip>/web/v1/status | protoc --decode_raw
```

### Comparing `solaredge_local-0.2.0/setup.py` & `solaredge_local-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
             buf.append(f.read())
     return sep.join(buf)
 
 long_description = read('README.md')
 
 setup(
     name='solaredge_local',
-    version="0.2.0",
+    version="0.2.1",
     url='https://github.com/drobtravels/solaredge-local',
     license='MIT License',
     author='David Roberts',
     author_email="",
     description='API wrapper to communicate locally with SolarEdge Inverters',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `solaredge_local-0.2.0/solaredge_local/solaredge.py` & `solaredge_local-0.2.1/solaredge_local/solaredge.py`

 * *Files identical despite different names*

### Comparing `solaredge_local-0.2.0/solaredge_local.egg-info/PKG-INFO` & `solaredge_local-0.2.1/solaredge_local.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,152 +1,161 @@
 Metadata-Version: 2.1
 Name: solaredge-local
-Version: 0.2.0
+Version: 0.2.1
 Summary: API wrapper to communicate locally with SolarEdge Inverters
 Home-page: https://github.com/drobtravels/solaredge-local
 Author: David Roberts
 Author-email: 
 License: MIT License
-Description: # SolarEdge Local
-        
-        The goal if this respository is to provide information about using the local API available on some solar edge inverters.  This is a WIP based on my observations and may contain inaccuracies.  Pull Requests or Issues are encouraged to correct any mistakes or add additonal informatoin.
-        
-        ### Relevant Models
-        
-        The local API is available on the [SExxxxH-US models with SetApp](https://www.solaredge.com/sites/default/files/se-hd-wave-single-phase-inverter-with-setapp-datasheet-na.pdf) as well as European three phase inverters SEXXK-XXXTXBXX4 models with SetApp like [SE3K-E10K](https://www.solaredge.com/sites/default/files/se-three-phase-inverter-setapp-ds.pdf), [SE12.5K-SE27.6K](https://www.solaredge.com/sites/default/files/se-three-phase-inverter-setapp-datasheet.pdf) and [SE33.3K](https://www.solaredge.com/sites/default/files/se-three-phase-inverter-for-277-480-grid-setapp-datasheet.pdf).
-        Please check carefully the datasheets if in the section "Additional Features", sub-section "Inverter Commissioning" is present the following line "With the SetApp mobile application using built-in Wi-Fi access point for local connection".
-        
-        More inforation on SeeApp could be found [here](https://www.solaredge.com/us/products/installer-tools/setapp). These models have no LED screen and are provisioned ONLY via a phone app during commissioning.
-        Check also the [SetApp FAQ](https://www.solaredge.com/sites/default/files/solaredge-setapp-faqs-eng.pdf) for more info.
-        For convenience it is reported here one Q&A:
-        
-        > Q: Can the new app be used for already installed inverters?
-        >
-        > A: Only SolarEdge inverters with a new communication board (no display) can be activated or configured via SetApp.
-        
-        Reportedly, these new inverters have a CPU number starting with 04.
-        
-        You can check by finding the IP address of your inverter and visiting it in a browser.  If it supports the local API, you'll see the SolarEdge logo and a "Commissioning" menu.
-        
-        If you do not have the local API available, see [this repository](https://github.com/jbuehl/solaredge) as an alternative.
-        
-        ### Using the Python wrapper
-        
-        For convinience, a python API wrapper, [solaredge_local](https://pypi.org/project/solaredge-local/) is available.  **Only python 3 is supported**
-        
-        To install: `pip install solaredge-local`
-        
-        To use:
-        
-        ```
-        from solaredge_local import SolarEdge
-        client = SolarEdge("http://<inverter ip address>")
-        client.get_status()  # Provides general energy and other overview information
-        client.get_maintenance() # Provides optimizer level information and other details
-        client.get_information() # Provides software versions and error log list.
-        client.get_power_control() # Provides power control information and other details.
-        ```
-        
-        ### API Endpoints
-        
-        * AppConfigs: "web/v1/app_configs"
-        * Region: "web/v1/region"
-        * Region_Country: "web/v1/region/country"
-        * Region_Language: "web/v1/region/language"
-        * Pairing: "web/v1/pairing"
-        * Pairing_Request: "web/v1/pairing/request"
-        * Communication: "web/v1/communication"
-        * Communication_Server: "web/v1/communication/server"
-        * Communication_Lan: "web/v1/communication/lan"
-        * Communication_Rs485_SlaveDetect: "web/v1/communication/rs485/<id>/slave_detect"
-        * Communication_Rs485_Protocol: "web/v1/communication/rs485/<id>/protocol"
-        * Communication_Rs485_DeviceId: "web/v1/communication/rs485/<id>/deviceid"
-        * Communication_Rs485_Modbus: "web/v1/communication/rs485/<id>/modbus"
-        * Communication_Rs485_Modbus_AddDevice: "web/v1/communication/rs485/<id>/modbus/add_device"
-        * Communication_Rs485_Modbus_RemoveDevice: "web/v1/communication/rs485/<id>/modbus/remove_device"
-        * Communication_Wifi: "web/v1/communication/wifi"
-        * Communication_Wifi_Wps: "web/v1/communication/wifi/wps"
-        * Communication_Wifi_Connect: "web/v1/communication/wifi/connect"
-        * Communication_Cellular: "web/v1/communication/cellular"
-        * Communication_Zigbee_Defaults: "web/v1/communication/zigbee/defaults"
-        * Communication_Zigbee_ModuleConfigs: "web/v1/communication/zigbee/module_configs"
-        * Communication_Zigbee_OpMode: "web/v1/communication/zigbee/op_mode"
-        * Communication_Gpio_Pri: "web/v1/communication/gpio/pri"
-        * Communication_ModbusTcp: "web/v1/communication/modbus_tcp"
-        * PowerControl: "web/v1/power_control"
-        * PowerControl_GridControl: "web/v1/power_control/grid_control"
-        * PowerControl_EnergyManager_LimitControl: "web/v1/power_control/energy_manager/limit_control"
-        * PowerControl_EnergyManager_EnergyControl: "web/v1/power_control/energy_manager/energy_control"
-        * PowerControl_EnergyManager_StorageControl: "web/v1/power_control/energy_manager/storage_control"
-        * PowerControl_ReactivePower: "web/v1/power_control/reactive_power"
-        * PowerControl_ActivePower: "web/v1/power_control/active_power"
-        * PowerControl_Wakeup: "web/v1/power_control/wakeup"
-        * PowerControl_Advanced: "web/v1/power_control/advanced"
-        * PowerControl_Reset: "web/v1/power_control/reset"
-        * PowerControl_Rrcr: "web/v1/power_control/rrcr"
-        * Maintenance: "web/v1/maintenance"
-        * Maintenance_DateTime: "web/v1/maintenance/date_and_time"
-        * Maintenance_ResetCounters: "web/v1/maintenance/reset_counters"
-        * Maintenance_ResetFactory: "web/v1/maintenance/reset_factory"
-        * Maintenance_Afci: "web/v1/maintenance/afci"
-        * Maintenance_AfciTest: "web/v1/maintenance/afci/test"
-        * Maintenance_Inverters_SelfTest: "web/v1/maintenance/inverters/<position>/self_test"
-        * Maintenance_Standby: "web/v1/maintenance/standby"
-        * Maintenance_GridProtectionLogin: "web/v1/maintenance/grid_protection/login"
-        * Maintenance_GridProtection: "web/v1/maintenance/grid_protection"
-        * Maintenance_UpgradeUsb: "web/v1/maintenance/fw_upgrade/usb"
-        * Information: "web/v1/information"
-        * Status: "web/v1/status"
-        * Status_ServerCommTest: "web/v1/status/server_comm_test"
-        
-        The Status endpoint appears to the most useful for realtime production data.
-        Optimizer level data is available from the maintenance API endpoint.
-        
-        
-        ## Using the API
-        
-        All endpoints I have explored so far appear to be a GET, and responses use [Protocol Buffers](https://developers.google.com/protocol-buffers/).  There is no authentication
-        
-        ### View Raw Response
-        
-        You can see the raw data by doing the following (assuming you have the protoocal buffers CLI tool installed)
-        
-        ```
-        curl -s http://<inverter ip>/web/v1/status | protoc --decode_raw
-        ```
-        
-        Many numbers appear to be 32 bit floating point.
-        
-        The proto definitions required to fully parse the responses are available in  javascript if you choose "view source" in the developer tools of your browser.
-        
-        ### View Parsed response
-        
-        If there is a corresponding `.proto` file in [message_types](/message_types), you can view the parsed response from the API.  Each proto file correspond to the name of an API endpoint. These are very much a WIP and may be incomplete.  These can be created by choosing "view source" in the developer tools of your browser, and searching for text like `proto.web_status.<apiNameInCamelCase>.toObject`
-        
-        Here is an example for the status API:
-        
-        ```
-        curl -s http://<inverter ip>/web/v1/status | protoc --decode Status message_types/status.proto
-        ```
-        
-        ### Updating Protocol Buffer response
-        
-        To add or change the Protocol Buffer defintions, please do the following
-        
-        1. Manually change the `message_types/*.proto` files as required
-        2. Test the file using `curl` as described in [View Parsed Response](#view-parsed-response)
-        3. Update the generated `*_pb2.py` files for each file changed by running a command like:
-        
-            ```
-            protoc -I=message_types --python_out=solaredge_local message_types/<filename_changed>.proto
-            ```
-        4. Commit the generated updates
-        
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
+
+# SolarEdge Local
+
+**Warning**
+
+Recent firmware versions disable local access.  Some units may continue to work, but many users are reporting it is no longer available.  See [this issue](https://github.com/jbuehl/solaredge/issues/124) and [this issue](https://github.com/drobtravels/solaredge-local/issues/24) for additional details.  Please check if you can access your inverter via a web browser before attempting to use this library.
+
+
+The goal if this respository is to provide information about using the local API available on some solar edge inverters.  This is a WIP based on my observations and may contain inaccuracies.  Pull Requests or Issues are encouraged to correct any mistakes or add additonal informatoin.
+
+### Relevant Models
+
+The fastest way to check your inverter will support this library and to enter the IP address of your inverter in the browser and see if the administration page is displayed.
+
+The local API is available for specific firmware versions running on [SExxxxH-US models with SetApp](https://www.solaredge.com/sites/default/files/se-hd-wave-single-phase-inverter-with-setapp-datasheet-na.pdf) as well as European three phase inverters SEXXK-XXXTXBXX4 models with SetApp like [SE3K-E10K](https://www.solaredge.com/sites/default/files/se-three-phase-inverter-setapp-ds.pdf), [SE12.5K-SE27.6K](https://www.solaredge.com/sites/default/files/se-three-phase-inverter-setapp-datasheet.pdf) and [SE33.3K](https://www.solaredge.com/sites/default/files/se-three-phase-inverter-for-277-480-grid-setapp-datasheet.pdf). Same goes for Australian inverters [SE2500H->SE10000H](https://www.solaredge.com/sites/default/files/se-single-phase-HD-wave-inverter-setapp-datasheet-aus.pdf). 
+Please check carefully the datasheets if in the section "Additional Features", sub-section "Inverter Commissioning" is present the following line "With the SetApp mobile application using built-in Wi-Fi access point for local connection".  You should 
+
+More inforation on SetApp could be found [here](https://www.solaredge.com/us/products/installer-tools/setapp). These models have no LED screen and are provisioned ONLY via a phone app during commissioning.
+Check also the [SetApp FAQ](https://www.solaredge.com/sites/default/files/solaredge-setapp-faqs-eng.pdf) for more info.
+For convenience it is reported here one Q&A:
+
+> Q: Can the new app be used for already installed inverters?
+>
+> A: Only SolarEdge inverters with a new communication board (no display) can be activated or configured via SetApp.
+
+These new inverters have a [CPU number](https://www.solaredge.com/setapp-inverters-firmware) starting with 04.
+
+You can check by finding the IP address of your inverter and visiting it in a browser.  If it supports the local API, you'll see the SolarEdge logo and a "Commissioning" menu.
+
+If you do not have the local API available, see [this repository](https://github.com/jbuehl/solaredge) as an alternative.
+
+### Using the Python wrapper
+
+For convinience, a python API wrapper, [solaredge_local](https://pypi.org/project/solaredge-local/) is available.  **Only python 3 is supported**
+
+To install: `pip3 install solaredge-local`
+
+To use:
+
+```
+from solaredge_local import SolarEdge
+client = SolarEdge("http://<inverter ip address>")
+client.get_status()  # Provides general energy and other overview information
+client.get_maintenance() # Provides optimizer level information and other details
+client.get_information() # Provides software versions and error log list.
+client.get_power_control() # Provides power control information and other details.
+```
+
+### API Endpoints
+
+* AppConfigs: "web/v1/app_configs"
+* Region: "web/v1/region"
+* Region_Country: "web/v1/region/country"
+* Region_Language: "web/v1/region/language"
+* Pairing: "web/v1/pairing"
+* Pairing_Request: "web/v1/pairing/request"
+* Communication: "web/v1/communication"
+* Communication_Server: "web/v1/communication/server"
+* Communication_Lan: "web/v1/communication/lan"
+* Communication_Rs485_SlaveDetect: "web/v1/communication/rs485/<id>/slave_detect"
+* Communication_Rs485_Protocol: "web/v1/communication/rs485/<id>/protocol"
+* Communication_Rs485_DeviceId: "web/v1/communication/rs485/<id>/deviceid"
+* Communication_Rs485_Modbus: "web/v1/communication/rs485/<id>/modbus"
+* Communication_Rs485_Modbus_AddDevice: "web/v1/communication/rs485/<id>/modbus/add_device"
+* Communication_Rs485_Modbus_RemoveDevice: "web/v1/communication/rs485/<id>/modbus/remove_device"
+* Communication_Wifi: "web/v1/communication/wifi"
+* Communication_Wifi_Wps: "web/v1/communication/wifi/wps"
+* Communication_Wifi_Connect: "web/v1/communication/wifi/connect"
+* Communication_Cellular: "web/v1/communication/cellular"
+* Communication_Zigbee_Defaults: "web/v1/communication/zigbee/defaults"
+* Communication_Zigbee_ModuleConfigs: "web/v1/communication/zigbee/module_configs"
+* Communication_Zigbee_OpMode: "web/v1/communication/zigbee/op_mode"
+* Communication_Gpio_Pri: "web/v1/communication/gpio/pri"
+* Communication_ModbusTcp: "web/v1/communication/modbus_tcp"
+* PowerControl: "web/v1/power_control"
+* PowerControl_GridControl: "web/v1/power_control/grid_control"
+* PowerControl_EnergyManager_LimitControl: "web/v1/power_control/energy_manager/limit_control"
+* PowerControl_EnergyManager_EnergyControl: "web/v1/power_control/energy_manager/energy_control"
+* PowerControl_EnergyManager_StorageControl: "web/v1/power_control/energy_manager/storage_control"
+* PowerControl_ReactivePower: "web/v1/power_control/reactive_power"
+* PowerControl_ActivePower: "web/v1/power_control/active_power"
+* PowerControl_Wakeup: "web/v1/power_control/wakeup"
+* PowerControl_Advanced: "web/v1/power_control/advanced"
+* PowerControl_Reset: "web/v1/power_control/reset"
+* PowerControl_Rrcr: "web/v1/power_control/rrcr"
+* Maintenance: "web/v1/maintenance"
+* Maintenance_DateTime: "web/v1/maintenance/date_and_time"
+* Maintenance_ResetCounters: "web/v1/maintenance/reset_counters"
+* Maintenance_ResetFactory: "web/v1/maintenance/reset_factory"
+* Maintenance_Afci: "web/v1/maintenance/afci"
+* Maintenance_AfciTest: "web/v1/maintenance/afci/test"
+* Maintenance_Inverters_SelfTest: "web/v1/maintenance/inverters/<position>/self_test"
+* Maintenance_Standby: "web/v1/maintenance/standby"
+* Maintenance_GridProtectionLogin: "web/v1/maintenance/grid_protection/login"
+* Maintenance_GridProtection: "web/v1/maintenance/grid_protection"
+* Maintenance_UpgradeUsb: "web/v1/maintenance/fw_upgrade/usb"
+* Information: "web/v1/information"
+* Status: "web/v1/status"
+* Status_ServerCommTest: "web/v1/status/server_comm_test"
+
+The Status endpoint appears to the most useful for realtime production data.
+Optimizer level data is available from the Maintenance API endpoint.
+
+
+## Using the API
+
+All endpoints I have explored so far appear to be a GET, and responses use [Protocol Buffers](https://developers.google.com/protocol-buffers/).  There is no authentication.
+
+### View Raw Response
+
+You can see the raw data by doing the following (assuming you have the protoocal buffers CLI tool installed)
+
+```
+curl -s http://<inverter ip>/web/v1/status | protoc --decode_raw
+```
+
+Many numbers appear to be 32 bit floating point.
+
+The proto definitions required to fully parse the responses are available in  javascript if you choose "view source" in the developer tools of your browser.
+
+### View Parsed response
+
+If there is a corresponding `.proto` file in [message_types](/message_types), you can view the parsed response from the API.  Each proto file correspond to the name of an API endpoint. These are very much a WIP and may be incomplete.  These can be created by choosing "view source" in the developer tools of your browser, and searching for text like `proto.web_status.<apiNameInCamelCase>.toObject`
+
+Here is an example for the status API:
+
+```
+curl -s http://<inverter ip>/web/v1/status | protoc --decode Status message_types/status.proto
+```
+
+### Updating Protocol Buffer response
+
+To add or change the Protocol Buffer defintions, please do the following
+
+1. Manually change the `message_types/*.proto` files as required
+2. Test the file using `curl` as described in [View Parsed Response](#view-parsed-response)
+3. Update the generated `*_pb2.py` files for each file changed by running a command like:
+
+    ```
+    protoc -I=message_types --python_out=solaredge_local message_types/<filename_changed>.proto
+    ```
+4. Commit the generated updates
+
+
```

