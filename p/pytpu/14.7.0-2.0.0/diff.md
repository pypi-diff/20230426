# Comparing `tmp/pytpu-14.7.0.tar.gz` & `tmp/pytpu-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytpu-14.7.0.tar", last modified: Tue Apr 11 18:52:34 2023, max compression
+gzip compressed data, was "dist/pytpu-2.0.0.tar", last modified: Wed Apr 26 11:03:38 2023, max compression
```

## Comparing `pytpu-14.7.0.tar` & `pytpu-2.0.0.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-11 18:52:34.318198 pytpu-14.7.0/
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)       41 2023-04-11 18:51:16.000000 pytpu-14.7.0/MANIFEST.in
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     4262 2023-04-11 18:52:34.318198 pytpu-14.7.0/PKG-INFO
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     3131 2023-04-11 18:51:16.000000 pytpu-14.7.0/README.md
-drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-11 18:52:34.314198 pytpu-14.7.0/pytpu/
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      600 2023-04-11 18:51:16.000000 pytpu-14.7.0/pytpu/__init__.py
-drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-11 18:52:34.318198 pytpu-14.7.0/pytpu/pytpu/
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      695 2023-04-11 18:51:16.000000 pytpu-14.7.0/pytpu/pytpu/__init__.py
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)    12138 2023-04-11 18:51:16.000000 pytpu-14.7.0/pytpu/pytpu/libtpu_bindings.py
-drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-11 18:52:34.318198 pytpu-14.7.0/pytpu/scripts/
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-11 18:51:16.000000 pytpu-14.7.0/pytpu/scripts/__init__.py
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     2258 2023-04-11 18:51:16.000000 pytpu-14.7.0/pytpu/scripts/pyrun_tpu_cli.py
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      810 2023-04-11 18:51:16.000000 pytpu-14.7.0/pytpu/scripts/run_get_fps.py
-drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-11 18:52:34.318198 pytpu-14.7.0/pytpu/tools/
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      119 2023-04-11 18:51:16.000000 pytpu-14.7.0/pytpu/tools/__init__.py
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     5134 2023-04-11 18:51:16.000000 pytpu-14.7.0/pytpu/tools/get_fps.py
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     6860 2023-04-11 18:51:16.000000 pytpu-14.7.0/pytpu/tools/helpers.py
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     7808 2023-04-11 18:51:16.000000 pytpu-14.7.0/pytpu/tools/tpu_runner.py
-drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-11 18:52:34.318198 pytpu-14.7.0/pytpu.egg-info/
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     4262 2023-04-11 18:52:34.000000 pytpu-14.7.0/pytpu.egg-info/PKG-INFO
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      489 2023-04-11 18:52:34.000000 pytpu-14.7.0/pytpu.egg-info/SOURCES.txt
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)        1 2023-04-11 18:52:34.000000 pytpu-14.7.0/pytpu.egg-info/dependency_links.txt
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      109 2023-04-11 18:52:34.000000 pytpu-14.7.0/pytpu.egg-info/entry_points.txt
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)        1 2023-04-11 18:52:34.000000 pytpu-14.7.0/pytpu.egg-info/not-zip-safe
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      197 2023-04-11 18:52:34.000000 pytpu-14.7.0/pytpu.egg-info/requires.txt
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)        6 2023-04-11 18:52:34.000000 pytpu-14.7.0/pytpu.egg-info/top_level.txt
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)       38 2023-04-11 18:52:34.318198 pytpu-14.7.0/setup.cfg
--rwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)     1531 2023-04-11 18:52:34.000000 pytpu-14.7.0/setup.py
+drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-26 11:03:38.272816 pytpu-2.0.0/
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)       41 2023-04-26 11:02:53.000000 pytpu-2.0.0/MANIFEST.in
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     4264 2023-04-26 11:03:38.272816 pytpu-2.0.0/PKG-INFO
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     3137 2023-04-26 11:02:53.000000 pytpu-2.0.0/README.md
+drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-26 11:03:38.268815 pytpu-2.0.0/pytpu/
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      255 2023-04-26 11:02:53.000000 pytpu-2.0.0/pytpu/__init__.py
+drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-26 11:03:38.268815 pytpu-2.0.0/pytpu/pytpu/
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      306 2023-04-26 11:02:53.000000 pytpu-2.0.0/pytpu/pytpu/__init__.py
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     5047 2023-04-26 11:02:53.000000 pytpu-2.0.0/pytpu/pytpu/converter_to_raw.py
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)    14101 2023-04-26 11:02:53.000000 pytpu-2.0.0/pytpu/pytpu/libtpu_bindings.py
+drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-26 11:03:38.268815 pytpu-2.0.0/pytpu/scripts/
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-26 11:02:53.000000 pytpu-2.0.0/pytpu/scripts/__init__.py
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     2352 2023-04-26 11:02:53.000000 pytpu-2.0.0/pytpu/scripts/pyrun_tpu_cli.py
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      834 2023-04-26 11:02:53.000000 pytpu-2.0.0/pytpu/scripts/run_get_fps.py
+drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-26 11:03:38.272816 pytpu-2.0.0/pytpu/tools/
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      123 2023-04-26 11:02:53.000000 pytpu-2.0.0/pytpu/tools/__init__.py
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     3919 2023-04-26 11:02:53.000000 pytpu-2.0.0/pytpu/tools/get_fps.py
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     6073 2023-04-26 11:02:53.000000 pytpu-2.0.0/pytpu/tools/helpers.py
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     2896 2023-04-26 11:02:53.000000 pytpu-2.0.0/pytpu/tools/lenet5_processing.py
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     3758 2023-04-26 11:02:53.000000 pytpu-2.0.0/pytpu/tools/resnet50_processing.py
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     7094 2023-04-26 11:02:53.000000 pytpu-2.0.0/pytpu/tools/tpu_runner.py
+drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-26 11:03:38.268815 pytpu-2.0.0/pytpu.egg-info/
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     4264 2023-04-26 11:03:38.000000 pytpu-2.0.0/pytpu.egg-info/PKG-INFO
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      589 2023-04-26 11:03:38.000000 pytpu-2.0.0/pytpu.egg-info/SOURCES.txt
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)        1 2023-04-26 11:03:38.000000 pytpu-2.0.0/pytpu.egg-info/dependency_links.txt
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      109 2023-04-26 11:03:38.000000 pytpu-2.0.0/pytpu.egg-info/entry_points.txt
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)        1 2023-04-26 11:03:38.000000 pytpu-2.0.0/pytpu.egg-info/not-zip-safe
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)       84 2023-04-26 11:03:38.000000 pytpu-2.0.0/pytpu.egg-info/requires.txt
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)        6 2023-04-26 11:03:38.000000 pytpu-2.0.0/pytpu.egg-info/top_level.txt
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)       38 2023-04-26 11:03:38.272816 pytpu-2.0.0/setup.cfg
+-rwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)      970 2023-04-26 11:03:38.000000 pytpu-2.0.0/setup.py
```

### Comparing `pytpu-14.7.0/PKG-INFO` & `pytpu-2.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pytpu
-Version: 14.7.0
+Version: 2.0.0
 Summary: TPU Python API
 Home-page: http://git.mmp.iva-tech.ru/tpu_sw/iva_tpu_sdk
-Author: Alexey Antipin
-Author-email: a.antipin@iva-tech.ru
+Author: IVA-Tech
+Author-email: info@iva-tech.ru
 License: UNKNOWN
 Description: # IVA TPU Python API
         ## Main entities
         ### TPUDevice
         TPUDevice is a device handle
         
         ### TPUProgram
@@ -23,36 +23,37 @@
         program = TPUProgram("program.tpu", config)
         ```
         
         ### TPUInference
         TPUInference contains input/output data
         
         ## Example
+        
         ```python
         import asyncio
         import numpy as np
         from iva_tpu import TPUDevice, TPUProgram, TPUInference
         
         from iva_applications.resnet50 import image_to_tensor
         from iva_applications.imagenet import tpu_tensor_to_classes
         from PIL import Image
         
         image = Image.open('ILSVRC2012_val_00000045.JPEG')
         tensor = image_to_tensor(image)
         
         device = TPUDevice()
-        program = TPUProgram("resnet50.tpu") #default TPUProgramInfo is totally fine
+        program = TPUProgram("resnet50.tpu")  # default TPUProgramInfo is totally fine
         device.load_program(program)
         inference = TPUInference(program)
         inference.load([tensor])
-        status_future = device.load_inference(inference)  # device returns future for inference status
+        status_future = device._load_inference(inference)  # device returns future for inference status
         event_loop = asyncio.get_event_loop()
         status = event_loop.run_until_complete(status_future)
-        assert status.is_success # check that there is no errors during inference
-        output = inference.get() # get results
+        assert status.is_success  # check that there is no errors during inference
+        output = inference.get()  # get results
         tpu_tensor_to_classes(output[0], top=1)
         ```
         
         ## TPU Dictionary interface
         ```
         ...
         program = TPUProgram("resnet50.tpu")
```

### Comparing `pytpu-14.7.0/README.md` & `pytpu-2.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -15,36 +15,37 @@
 program = TPUProgram("program.tpu", config)
 ```
 
 ### TPUInference
 TPUInference contains input/output data
 
 ## Example
+
 ```python
 import asyncio
 import numpy as np
 from iva_tpu import TPUDevice, TPUProgram, TPUInference
 
 from iva_applications.resnet50 import image_to_tensor
 from iva_applications.imagenet import tpu_tensor_to_classes
 from PIL import Image
 
 image = Image.open('ILSVRC2012_val_00000045.JPEG')
 tensor = image_to_tensor(image)
 
 device = TPUDevice()
-program = TPUProgram("resnet50.tpu") #default TPUProgramInfo is totally fine
+program = TPUProgram("resnet50.tpu")  # default TPUProgramInfo is totally fine
 device.load_program(program)
 inference = TPUInference(program)
 inference.load([tensor])
-status_future = device.load_inference(inference)  # device returns future for inference status
+status_future = device._load_inference(inference)  # device returns future for inference status
 event_loop = asyncio.get_event_loop()
 status = event_loop.run_until_complete(status_future)
-assert status.is_success # check that there is no errors during inference
-output = inference.get() # get results
+assert status.is_success  # check that there is no errors during inference
+output = inference.get()  # get results
 tpu_tensor_to_classes(output[0], top=1)
 ```
 
 ## TPU Dictionary interface
 ```
 ...
 program = TPUProgram("resnet50.tpu")
```

### Comparing `pytpu-14.7.0/pytpu/scripts/pyrun_tpu_cli.py` & `pytpu-2.0.0/pytpu/scripts/pyrun_tpu_cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-import argparse
-import logging
-import os
-from pytpu.tools.helpers import get_io_from_bin
-from pytpu.tools.tpu_runner import TpuRunner
-# from pytpu.tools.pyrun_tpu import pyrun_tpu
-
-LOGGER = logging.getLogger(__name__)
-
-
-def main():
-    parser = argparse.ArgumentParser(prog='pyrun_tpu',
-                                     description='Python command line tool to run tpu programs')
-
-    parser.add_argument('-p', nargs='?', help='Path to the program.tpu', type=str)
-    parser.add_argument('-i', nargs='?', help='Inputs binary files path', type=str, default='')
-    parser.add_argument('-o', nargs='?', help='Save output binary files path', type=str, default='')
-    parser.add_argument('-t', nargs='?', help='Enable execution time calculation', type=str)
-    parser.add_argument('-debug', help='Enable DEBUG messages', action='store_true')
-    parser.add_argument('-pyproc', action='store_true', help='Enable python pre- and post-processing')
-
-    args = parser.parse_args()
-
-    if args.debug:
-        log_level = logging.DEBUG
-    else:
-        log_level = logging.INFO
-    logging.basicConfig(level=log_level)
-    LOGGER.info(f'Use logging level: {log_level}')
-
-    if args.i is None:
-        LOGGER.info('WARNING: no input files are set')
-        inputs = []
-    else:
-        inputs = args.i.split(',')
-    input_data, _ = get_io_from_bin(args.p, inputs, 'inputs')
-
-    runner = TpuRunner(program_path=args.p,
-                       loop=None,
-                       sync=False,
-                       pyprocessing=args.pyproc)
-    output_data = runner(input_data)
-    # output_data = pyrun_tpu(args.p, input_data)
-
-    # Write outputs to binary files
-    if args.o is None:
-        LOGGER.info('WARNING: no output files are set to store the results')
-    else:
-        output_files = args.o.split(',')
-        _, output_names = get_io_from_bin(args.p, None, 'outputs')
-        for idx, name in enumerate(output_names):
-            if not os.path.exists(os.path.dirname(output_files[idx])):
-                os.makedirs(os.path.dirname(output_files[idx]))
-            with open(output_files[idx], 'wb') as io_file:
-                io_file.write(output_data[name].tobytes())
-                LOGGER.info(f'Writing output {name} to {output_files[idx]}')
+# import argparse
+# import logging
+# import os
+# from pytpu.tools.helpers import get_io_from_bin
+# from pytpu.tools.tpu_runner import TpuRunner
+# # from pytpu.tools.pyrun_tpu import pyrun_tpu
+
+# LOGGER = logging.getLogger(__name__)
+
+
+# def main():
+#     parser = argparse.ArgumentParser(prog='pyrun_tpu',
+#                                      description='Python command line tool to run tpu programs')
+
+#     parser.add_argument('-p', nargs='?', help='Path to the program.tpu', type=str)
+#     parser.add_argument('-i', nargs='?', help='Inputs binary files path', type=str, default='')
+#     parser.add_argument('-o', nargs='?', help='Save output binary files path', type=str, default='')
+#     parser.add_argument('-t', nargs='?', help='Enable execution time calculation', type=str)
+#     parser.add_argument('-debug', help='Enable DEBUG messages', action='store_true')
+#     parser.add_argument('-pyproc', action='store_true', help='Enable python pre- and post-processing')
+
+#     args = parser.parse_args()
+
+#     if args.debug:
+#         log_level = logging.DEBUG
+#     else:
+#         log_level = logging.INFO
+#     logging.basicConfig(level=log_level)
+#     LOGGER.info(f'Use logging level: {log_level}')
+
+#     if args.i is None:
+#         LOGGER.info('WARNING: no input files are set')
+#         inputs = []
+#     else:
+#         inputs = args.i.split(',')
+#     input_data, _ = get_io_from_bin(args.p, inputs, 'inputs')
+
+#     runner = TpuRunner(program_path=args.p,
+#                        loop=None,
+#                        sync=False,
+#                        pyprocessing=args.pyproc)
+#     output_data = runner(input_data)
+#     # output_data = pyrun_tpu(args.p, input_data)
+
+#     # Write outputs to binary files
+#     if args.o is None:
+#         LOGGER.info('WARNING: no output files are set to store the results')
+#     else:
+#         output_files = args.o.split(',')
+#         _, output_names = get_io_from_bin(args.p, None, 'outputs')
+#         for idx, name in enumerate(output_names):
+#             if not os.path.exists(os.path.dirname(output_files[idx])):
+#                 os.makedirs(os.path.dirname(output_files[idx]))
+#             with open(output_files[idx], 'wb') as io_file:
+#                 io_file.write(output_data[name].tobytes())
+#                 LOGGER.info(f'Writing output {name} to {output_files[idx]}')
```

### Comparing `pytpu-14.7.0/pytpu/scripts/run_get_fps.py` & `pytpu-2.0.0/pytpu/scripts/run_get_fps.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import argparse
-from pytpu.tools import get_fps
+# import argparse
+# from pytpu.tools import get_fps
 
 
-def main():
-    parser = argparse.ArgumentParser(prog='run_get_fps',
-                                     description='TPU performance measurement tool')
+# def main():
+#     parser = argparse.ArgumentParser(prog='run_get_fps',
+#                                      description='TPU performance measurement tool')
 
-    parser.add_argument('program', nargs='?', help='Path to the program.tpu', type=str)
-    parser.add_argument('-raw', nargs='?', help='Enable RAW mode without pre- and post-processing (default = False)',
-                        type=int, default=False)
-    parser.add_argument('-n_queries', nargs='?', help='Number of queries (default = 1000)', type=int, default=1000)
-    parser.add_argument('-n_proc', nargs='?', help='Number of processes (default = 4)', type=int, default=4)
+#     parser.add_argument('program', nargs='?', help='Path to the program.tpu', type=str)
+#     parser.add_argument('-raw', nargs='?', help='Enable RAW mode without pre- and post-processing (default = False)',
+#                         type=int, default=False)
+#     parser.add_argument('-n_queries', nargs='?', help='Number of queries (default = 1000)', type=int, default=1000)
+#     parser.add_argument('-n_proc', nargs='?', help='Number of processes (default = 4)', type=int, default=4)
 
-    args = parser.parse_args()
+#     args = parser.parse_args()
 
-    get_fps(args.program, raw=bool(args.raw), n_queries=args.n_queries, n_proc=args.n_proc)
+#     get_fps(args.program, raw=bool(args.raw), n_queries=args.n_queries, n_proc=args.n_proc)
```

### Comparing `pytpu-14.7.0/pytpu/tools/helpers.py` & `pytpu-2.0.0/pytpu/tools/helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,83 +1,56 @@
 import copy
 import logging
 import os
 import re
 import shutil
 import tempfile
-import json 
+import json
 from typing import Any
 from typing import Dict
 from typing import List
-from typing import Optional
 from typing import TYPE_CHECKING
-from typing import Tuple
+# from typing import Tuple
 from zipfile import ZipFile
 
 import numpy as np
 
-from tpu_tlm_is.base import TpuParameters
-from tpu_tlm_is.base import get_hw_params
-from tpu_tlm_is.base.number_types import STR_TO_NUMPY
+# from tpu_tlm_is.base import TpuParameters
+# from tpu_tlm_is.base import get_hw_params
+# from tpu_tlm_is.base.number_types import STR_TO_NUMPY
 
 
 if TYPE_CHECKING:
-    from ..pytpu import TPUProgram
+    pass
 
 __all__ = [
     'get_tpu_devices',
-    'get_tpu_parameters',
+    # 'get_tpu_parameters',
     'STR_TO_BYTES',
     'STR_TO_DTYPE',
     'to_raw',
     'to_nhwc_program',
-    'input_metadata',
-    'output_metadata',
-    'convert_from_uint8_to_user_dtype',
 ]
 
 LOGGER = logging.getLogger(__name__)
 
 
 def get_tpu_devices() -> List[str]:
     return [os.path.join('/dev', f) for f in os.listdir('/dev') if re.match(r'tpu.', f) and len(f) == 4]
 
 
-def input_metadata(program):
-    metadata = json.loads(program.info())
-    # return dict(*metadata['inputs']['1'].values())
-    return metadata['inputs']['1']
-
-
-def output_metadata(program):
-    metadata = json.loads(program.info())
-    # return dict(*metadata['outputs']['2'].values())
-    return metadata['outputs']['2']
-
-
-def convert_from_uint8_to_user_dtype(data, user_dtype):
-    if 'int' in user_dtype:
-        return data.view(user_dtype)
-    elif 'float16' == user_dtype:
-        return data.view(np.uint16).view(user_dtype)
-    elif 'float32' == user_dtype:
-        return data.view(np.uint32).view(user_dtype)
-    else:
-        raise AssertionError(f'{user_dtype} as user_dtype does not support!')
-
-
-def get_tpu_parameters(hw_par: Dict[str, Any]) -> TpuParameters:
-    if hw_par['cache_word_len'] == 128 and hw_par['ddr_word_len'] == 32:
-        return get_hw_params('128x128').tpu_parameters
-    if hw_par['cache_word_len'] == 64 and hw_par['ddr_word_len'] == 16:
-        return get_hw_params('64x64').tpu_parameters
-    if hw_par['cache_word_len'] == 64 and hw_par['ddr_word_len'] == 64:
-        return get_hw_params('64x64_fpga').tpu_parameters
-
-    raise NotImplementedError('Translation of such platform does not supported!')
+# def get_tpu_parameters(hw_par: Dict[str, Any]) -> TpuParameters:
+#     if hw_par['cache_word_len'] == 128 and hw_par['ddr_word_len'] == 32:
+#         return get_hw_params('128x128').tpu_parameters
+#     if hw_par['cache_word_len'] == 64 and hw_par['ddr_word_len'] == 16:
+#         return get_hw_params('64x64').tpu_parameters
+#     if hw_par['cache_word_len'] == 64 and hw_par['ddr_word_len'] == 64:
+#         return get_hw_params('64x64_fpga').tpu_parameters
+#
+#     raise NotImplementedError('Translation of such platform does not supported!')
 
 
 def _to_raw_old(io_: Dict[str, Any], name: str) -> Dict[str, Any]:
     LOGGER.debug(f'IO description: {io_}')
 
     size = io_['size']
     io_out = {
@@ -176,35 +149,35 @@
 
         with tempfile.NamedTemporaryFile() as temp_file:
             shutil.make_archive(temp_file.name, 'zip', tempdir)
             os.rename(temp_file.name + '.zip', store_path)
             LOGGER.debug(f'NHWC program saved to {store_path}')
 
 
-def get_io_from_bin(program_path: str, io_path: str, io_type: str
-                    ) -> Tuple[Dict[str, np.ndarray], List[str]]:
-    with tempfile.TemporaryDirectory() as tempdir:
-        with ZipFile(program_path, 'r') as zip_obj:
-            zip_obj.extractall(tempdir)
-
-        with open(os.path.join(tempdir, 'metadata.json'), 'r', encoding='utf8') as metadata_file:
-            metadata = json.load(metadata_file)
-
-    io_data = {}
-    io_names = []
-    for _, region in metadata[io_type].items():
-        for name, io_ in region.items():
-            io_names.append(name)
-            _path = os.path.join(io_path, io_type, name.replace('/', '_') + '.bin')
-            with open(_path, 'r') as io_file:
-                tmp = np.fromfile(io_file, STR_TO_NUMPY[io_.get('user_dtype', 'int8')])
-                io_data[name] = tmp.reshape(io_.get('user_shape', (1, -1)))
-                LOGGER.debug(f'Read {io_type} from files: {name}, {io_data[name].shape}, {io_data[name].dtype}')
+# def get_io_from_bin(program_path: str, io_path: str, io_type: str
+#                     ) -> Tuple[Dict[str, np.ndarray], List[str]]:
+#     with tempfile.TemporaryDirectory() as tempdir:
+#         with ZipFile(program_path, 'r') as zip_obj:
+#             zip_obj.extractall(tempdir)
+
+#         with open(os.path.join(tempdir, 'metadata.json'), 'r', encoding='utf8') as metadata_file:
+#             metadata = json.load(metadata_file)
+
+#     io_data = {}
+#     io_names = []
+#     for _, region in metadata[io_type].items():
+#         for name, io_ in region.items():
+#             io_names.append(name)
+#             _path = os.path.join(io_path, io_type, name.replace('/', '_') + '.bin')
+#             with open(_path, 'r') as io_file:
+#                 tmp = np.fromfile(io_file, STR_TO_NUMPY[io_.get('user_dtype', 'int8')])
+#                 io_data[name] = tmp.reshape(io_.get('user_shape', (1, -1)))
+#                 LOGGER.debug(f'Read {io_type} from files: {name}, {io_data[name].shape}, {io_data[name].dtype}')
 
-    return io_data, io_names
+#     return io_data, io_names
 
 
 STR_TO_DTYPE = {
     'int8': np.int8,
     'float16': np.float16,
     'float32': np.float32,
 }
```

### Comparing `pytpu-14.7.0/pytpu/tools/tpu_runner.py` & `pytpu-2.0.0/pytpu/tools/tpu_runner.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,199 +1,177 @@
-import asyncio
-import json
-import logging
-import os
-import shutil
-import tempfile
-
-from math import ceil
-from typing import Any
-from typing import Dict
-from typing import Tuple
-from zipfile import ZipFile
-
-import numpy as np
-
-from tpu_tlm_is.base import TensorDescription
-from tpu_tlm_is.base.number_types import UserNumberType
-from tpu_tlm_is.base.number_types import TpuNumberType
-from tpu_tlm_is.base.number_types import STR_TO_USER_NUMBER_TYPE
-from tpu_tlm_is.base.number_types import STR_TO_TPU_NUMBER_TYPE
-from tpu_tlm_is.models.iotools import post_process
-from tpu_tlm_is.models.iotools import pre_process
-from pytpu.pytpu import TPUDevice, TPUProgram, TPUInference  # type: ignore
-from pytpu.pytpu import TPUProcessingMode
-from pytpu.pytpu import load_inference
-from pytpu.pytpu import get_inference
-from pytpu.pytpu import submit_inference
-from ..tools.helpers import get_tpu_devices
-from ..tools.helpers import get_tpu_parameters
-from ..tools.helpers import to_raw
-
-
-__all__ = [
-    'TpuRunner',
-]
-
-LOGGER = logging.getLogger(__name__)
-_SUFFIX = ':0'
-
-
-def _get_tensor_description(io_: Dict[str, Any], cwl: int) -> TensorDescription:
-    if 'user_shape' in io_.keys():
-        LOGGER.debug('Generate NON-RAW descriptions')
-        return TensorDescription(
-            user_shape_mask=tuple(tuple([True, ] * abs(p[0]) + [False, ] * s + [True, ] * abs(p[1])
-                                  for p, s in zip(io_['padding'], io_['user_shape']))),
-            user_order=io_['user_order'],
-            user_dtype=STR_TO_USER_NUMBER_TYPE[io_['user_dtype']],
-            tpu_shape=io_['tpu_shape'],
-            tpu_order=io_['tpu_order'],
-            tpu_dtype=STR_TO_TPU_NUMBER_TYPE[io_['tpu_dtype']],
-            scales=tuple([float(s) for s in io_['scales']]),
-            anchor=io_['anchor'],
-        )
-    else:
-        LOGGER.debug('Generate RAW descriptions')
-        return TensorDescription(
-            user_shape_mask=((False, ), tuple([False, ] * int(io_['size'])), ),
-            user_order=('N', 'C', ),
-            user_dtype=UserNumberType.INT8,
-            tpu_shape=(1, ceil(int(io_['size']) / cwl), np.minimum(cwl, int(io_['size']))),
-            tpu_order=('N', 'C', 'B'),
-            tpu_dtype=TpuNumberType.INT8,
-            scales=(1.0, ),
-        )
-
-
-def _tensor_as_node(node: Dict[str, np.ndarray]) -> Tuple[Dict[str, np.ndarray], bool]:
-    node_tensor = {}
-    _len_suffix = len(_SUFFIX)
-    flag_suffix = False
-    for key, data in node.items():
-        if key[-_len_suffix:] == _SUFFIX:
-            node_tensor[key[:-_len_suffix]] = data
-            flag_suffix = True
-        else:
-            node_tensor[key] = data
-    return node_tensor, flag_suffix
-
-
-def _node_as_tensor(node: Dict[str, np.ndarray]) -> Dict[str, np.ndarray]:
-    node_tensor = {}
-    _len_suffix = len(_SUFFIX)
-    for key, data in node.items():
-        if key[-_len_suffix:] == _SUFFIX:
-            node_tensor[key] = data
-        else:
-            node_tensor[key + _SUFFIX] = data
-
-    return node_tensor
-
-
-class TpuRunner:
-    """Runner for IVA TPU."""
-
-    def __init__(self, program_path: str, device_name: str = None, loop: Any = None, sync: bool = False, pyprocessing: bool = False) -> None:
-
-        LOGGER.debug(f'Init TpuRunner with program: {program_path}')
-
-        self._pyprocessing = pyprocessing
-        self._sync = sync
-        self._loop = loop if loop else asyncio.get_event_loop()
-
-        tpu_devices = get_tpu_devices()
-        if len(tpu_devices) < 1:
-            raise EnvironmentError('No TPU devices found')
-        
-        # import ipdb; ipdb.set_trace()
-        if device_name is None:
-        # device_num = int(list(filter(str.isdigit, tpu_devices[0]))[0])
-            self._device = TPUDevice(tpu_devices[0].encode('utf-8'))
-        else:
-            full_name = [name for name in tpu_devices if device_name in name]
-            assert len(full_name) == 1, f'More than one device selected: {full_name}'
-            assert full_name[0] in tpu_devices, f'No such device: {device_name}'
-            self._device = TPUDevice(full_name[0].encode('utf-8'))
-        
-        if self._device.init() != 0:
-            print('\n\nDevice error: {}\n'.format(self._device.get_error().decode('utf-8')))
-
-        if pyprocessing:
-            with tempfile.TemporaryDirectory() as tempdir:
-                with ZipFile(program_path, 'r') as zip_obj:
-                    zip_obj.extractall(tempdir)
-
-                with open(os.path.join(tempdir, 'metadata.json'), 'r') as metadata_file:
-                    metadata = json.load(metadata_file)
-
-                tpu_par = get_tpu_parameters(metadata['hardware_parameters'])
-
-                tensor_descriptions: Dict[str, TensorDescription] = dict()
-                for _, region in metadata['inputs'].items():
-                    for name, io_ in region.items():
-                        tensor_descriptions[name] = _get_tensor_description(io_, tpu_par.cache_word_length)
-                        LOGGER.debug(f'Input: {name}, {[len(s) for s in tensor_descriptions[name].user_shape_mask]}, '
-                                     f'{tensor_descriptions[name].user_dtype}')
-
-                for _, region in metadata['outputs'].items():
-                    for name, io_ in region.items():
-                        tensor_descriptions[name] = _get_tensor_description(io_, tpu_par.cache_word_length)
-
-                with open(os.path.join(tempdir, 'metadata.json'), 'w') as metadata_file:
-                    raw_metadata = to_raw(metadata)
-                    json.dump(raw_metadata, metadata_file)
-
-                with tempfile.NamedTemporaryFile() as temp_file:
-                    program_path = os.path.join(tempdir, 'program_raw.tpu')
-                    shutil.make_archive(temp_file.name, 'zip', tempdir)
-                    os.rename(temp_file.name + '.zip', program_path)
-                    LOGGER.debug(f'Raw program saved to {program_path}')
-
-                self._tpu_par = tpu_par
-                self._tensor_descriptions = tensor_descriptions
-        
-        self._program = TPUProgram(program_path.encode('utf-8'))
-        self._device.load_program(self._program)
-
-        if not bool(self._program.is_valid()):
-            print('\n\nProgram Error: {}\n'.format(self._program.get_error().decode('utf-8')))
-
-    def __call__(self, input_data: Dict[str, np.ndarray]) -> Dict[str, np.ndarray]:
-        """
-        Run inference using IVA TPU.
-
-        Parameters
-        ----------
-        input_data
-            Dict with input tensors for inference
-
-        """
-
-        input_data, flag_suffix = _tensor_as_node(input_data)
-        
-        if self._pyprocessing:
-            mode = TPUProcessingMode.kRaw.value
-            input_data = pre_process(self._tpu_par, input_data, self._tensor_descriptions)
-            # Convert to raw program format
-            input_data = {n: v.reshape((1, -1)).view(np.int8) for n, v in input_data.items()}
-        else:
-            mode = TPUProcessingMode.kFull.value
-
-        inference = TPUInference(self._program)
-        tpu_input_buf, tpu_output_buf, ctx = load_inference(input_data, self._program)
-        
-        inference.set_inputs(tpu_input_buf)
-        inference.set_outputs(tpu_output_buf)
-
-        if self._sync:
-            self._device.run_inference(inference, mode)
-        else:
-            status_future = submit_inference(self._device, self._program, inference, tpu_output_buf, mode)
-            self._loop.run_until_complete(status_future)
-        output_data = get_inference(self._program, tpu_output_buf, ctx, as_dict=True)
-        if self._pyprocessing:
-            output_data = post_process(self._tpu_par, output_data, self._tensor_descriptions)
-        if flag_suffix:
-            output_data = _node_as_tensor(output_data)
-
-        return output_data
+# import asyncio
+# import json
+# import logging
+# import os
+# import shutil
+# import tempfile
+#
+# from math import ceil
+# from typing import Any
+# from typing import Dict
+# from typing import Tuple
+# from zipfile import ZipFile
+#
+# import numpy as np
+#
+# from tpu_tlm_is.base import TensorDescription
+# from tpu_tlm_is.base.number_types import UserNumberType
+# from tpu_tlm_is.base.number_types import TpuNumberType
+# from tpu_tlm_is.base.number_types import STR_TO_USER_NUMBER_TYPE
+# from tpu_tlm_is.base.number_types import STR_TO_TPU_NUMBER_TYPE
+# from tpu_tlm_is.models.iotools import post_process
+# from tpu_tlm_is.models.iotools import pre_process
+# from pytpu.pytpu import TPUDevice, TPUProgram, TPUInference, TPU  # type: ignore
+# from pytpu.pytpu import TPUProcessingMode
+# from pytpu.pytpu import load_inference
+# from pytpu.pytpu import get_inference
+# from pytpu.pytpu import submit_inference
+# from ..tools.helpers import get_tpu_devices
+# from ..tools.helpers import get_tpu_parameters
+# from ..tools.helpers import to_raw
+#
+#
+# __all__ = [
+#     'TpuRunner',
+# ]
+#
+# LOGGER = logging.getLogger(__name__)
+# _SUFFIX = ':0'
+#
+#
+# def _get_tensor_description(io_: Dict[str, Any], cwl: int) -> TensorDescription:
+#     if 'user_shape' in io_.keys():
+#         LOGGER.debug('Generate NON-RAW descriptions')
+#         return TensorDescription(
+#             user_shape_mask=tuple(tuple([True, ] * abs(p[0]) + [False, ] * s + [True, ] * abs(p[1])
+#                                   for p, s in zip(io_['padding'], io_['user_shape']))),
+#             user_order=io_['user_order'],
+#             user_dtype=STR_TO_USER_NUMBER_TYPE[io_['user_dtype']],
+#             tpu_shape=io_['tpu_shape'],
+#             tpu_order=io_['tpu_order'],
+#             tpu_dtype=STR_TO_TPU_NUMBER_TYPE[io_['tpu_dtype']],
+#             scales=tuple([float(s) for s in io_['scales']]),
+#             anchor=io_['anchor'],
+#         )
+#     else:
+#         LOGGER.debug('Generate RAW descriptions')
+#         return TensorDescription(
+#             user_shape_mask=((False, ), tuple([False, ] * int(io_['size'])), ),
+#             user_order=('N', 'C', ),
+#             user_dtype=UserNumberType.INT8,
+#             tpu_shape=(1, ceil(int(io_['size']) / cwl), np.minimum(cwl, int(io_['size']))),
+#             tpu_order=('N', 'C', 'B'),
+#             tpu_dtype=TpuNumberType.INT8,
+#             scales=(1.0, ),
+#         )
+#
+#
+# def _tensor_as_node(node: Dict[str, np.ndarray]) -> Tuple[Dict[str, np.ndarray], bool]:
+#     node_tensor = {}
+#     _len_suffix = len(_SUFFIX)
+#     flag_suffix = False
+#     for key, data in node.items():
+#         if key[-_len_suffix:] == _SUFFIX:
+#             node_tensor[key[:-_len_suffix]] = data
+#             flag_suffix = True
+#         else:
+#             node_tensor[key] = data
+#     return node_tensor, flag_suffix
+#
+#
+# def _node_as_tensor(node: Dict[str, np.ndarray]) -> Dict[str, np.ndarray]:
+#     node_tensor = {}
+#     _len_suffix = len(_SUFFIX)
+#     for key, data in node.items():
+#         if key[-_len_suffix:] == _SUFFIX:
+#             node_tensor[key] = data
+#         else:
+#             node_tensor[key + _SUFFIX] = data
+#
+#     return node_tensor
+#
+#
+# class TpuRunner:
+#     def __init__(self, program_path):
+#         self.program_path = program_path
+#         self._tpu_par = None
+#         self._tensor_descriptions = None
+#
+#     def __enter__(self):
+#         dev_name = TPU.list_devices()[0] # first device
+#         self.device = TPU.get_device(dev_name)
+#         self.program = TPU.get_program(self.program_path)
+#         self.device.load_program(self.program)
+#         self.program.device = self.device
+#         return self
+#
+#     def __exit__(self, exc_type, exc_value, traceback):
+#         self.program.close()
+#         self.device.close()
+#
+#     def __call__(self, input_data: Dict[str, np.ndarray]) -> Dict[str, np.ndarray]:
+#         input_data, flag_suffix = _tensor_as_node(input_data)
+#         with self.program.inference() as inference:
+#             output_data = inference.sync(input_data)
+#             if flag_suffix:
+#                 output_data = _node_as_tensor(output_data)
+#
+#         return output_data
+#
+#     # pyprocessing
+#     def create_raw_programe(self):
+#         with tempfile.TemporaryDirectory() as tempdir:
+#             with ZipFile(self.program_path, 'r') as zip_obj:
+#                 zip_obj.extractall(tempdir)
+#
+#             with open(os.path.join(tempdir, 'metadata.json'), 'r') as metadata_file:
+#                 metadata = json.load(metadata_file)
+#
+#             tpu_par = get_tpu_parameters(metadata['hardware_parameters'])
+#
+#             tensor_descriptions: Dict[str, TensorDescription] = dict()
+#             for _, region in metadata['inputs'].items():
+#                 for name, io_ in region.items():
+#                     tensor_descriptions[name] = _get_tensor_description(io_, tpu_par.cache_word_length)
+#                     LOGGER.debug(f'Input: {name}, {[len(s) for s in tensor_descriptions[name].user_shape_mask]}, '
+#                                  f'{tensor_descriptions[name].user_dtype}')
+#
+#             for _, region in metadata['outputs'].items():
+#                 for name, io_ in region.items():
+#                     tensor_descriptions[name] = _get_tensor_description(io_, tpu_par.cache_word_length)
+#
+#             with open(os.path.join(tempdir, 'metadata.json'), 'w') as metadata_file:
+#                 raw_metadata = to_raw(metadata)
+#                 json.dump(raw_metadata, metadata_file)
+#
+#             with tempfile.NamedTemporaryFile() as temp_file:
+#                 self.program_path = os.path.join(tempdir, 'program_raw.tpu')
+#                 shutil.make_archive(temp_file.name, 'zip', tempdir)
+#                 os.rename(temp_file.name + '.zip', self.program_path)
+#                 LOGGER.debug(f'Raw program saved to {self.program_path}')
+#
+#             self._tpu_par = tpu_par
+#             self._tensor_descriptions = tensor_descriptions
+#
+#     def run_with_pyprocessing(self, input_data: Dict[str, np.ndarray]) -> Dict[str, np.ndarray]:
+#         self.create_raw_programe()
+#
+#         input_data, flag_suffix = _tensor_as_node(input_data)
+#         mode = TPUProcessingMode.kRaw.value
+#         input_data = pre_process(self._tpu_par, input_data, self._tensor_descriptions)
+#
+#         # Convert to raw program format
+#         input_data = {n: v.reshape((1, -1)).view(np.int8) for n, v in input_data.items()}
+#
+#         with self.program.inference() as inference:
+#             tpu_input_buf, tpu_output_buf, ctx = load_inference(input_data, self.program)
+#             inference.set_inputs(tpu_input_buf)
+#             inference.set_outputs(tpu_output_buf)
+#             self.device.run_inference(inference, mode)
+#             output_data = get_inference(self.program, tpu_output_buf, ctx, as_dict=True)
+#             output_data = post_process(self._tpu_par, output_data, self._tensor_descriptions)
+#
+#             if flag_suffix:
+#                 output_data = _node_as_tensor(output_data)
+#
+#             return output_data
+#
```

### Comparing `pytpu-14.7.0/pytpu.egg-info/PKG-INFO` & `pytpu-2.0.0/pytpu.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pytpu
-Version: 14.7.0
+Version: 2.0.0
 Summary: TPU Python API
 Home-page: http://git.mmp.iva-tech.ru/tpu_sw/iva_tpu_sdk
-Author: Alexey Antipin
-Author-email: a.antipin@iva-tech.ru
+Author: IVA-Tech
+Author-email: info@iva-tech.ru
 License: UNKNOWN
 Description: # IVA TPU Python API
         ## Main entities
         ### TPUDevice
         TPUDevice is a device handle
         
         ### TPUProgram
@@ -23,36 +23,37 @@
         program = TPUProgram("program.tpu", config)
         ```
         
         ### TPUInference
         TPUInference contains input/output data
         
         ## Example
+        
         ```python
         import asyncio
         import numpy as np
         from iva_tpu import TPUDevice, TPUProgram, TPUInference
         
         from iva_applications.resnet50 import image_to_tensor
         from iva_applications.imagenet import tpu_tensor_to_classes
         from PIL import Image
         
         image = Image.open('ILSVRC2012_val_00000045.JPEG')
         tensor = image_to_tensor(image)
         
         device = TPUDevice()
-        program = TPUProgram("resnet50.tpu") #default TPUProgramInfo is totally fine
+        program = TPUProgram("resnet50.tpu")  # default TPUProgramInfo is totally fine
         device.load_program(program)
         inference = TPUInference(program)
         inference.load([tensor])
-        status_future = device.load_inference(inference)  # device returns future for inference status
+        status_future = device._load_inference(inference)  # device returns future for inference status
         event_loop = asyncio.get_event_loop()
         status = event_loop.run_until_complete(status_future)
-        assert status.is_success # check that there is no errors during inference
-        output = inference.get() # get results
+        assert status.is_success  # check that there is no errors during inference
+        output = inference.get()  # get results
         tpu_tensor_to_classes(output[0], top=1)
         ```
         
         ## TPU Dictionary interface
         ```
         ...
         program = TPUProgram("resnet50.tpu")
```

