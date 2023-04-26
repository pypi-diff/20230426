# Comparing `tmp/tritony-0.0.8.tar.gz` & `tmp/tritony-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tritony-0.0.8.tar", last modified: Wed Oct  5 11:43:05 2022, max compression
+gzip compressed data, was "tritony-0.0.9.tar", last modified: Wed Apr 26 04:31:33 2023, max compression
```

## Comparing `tritony-0.0.8.tar` & `tritony-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxr-xr-x   0 Arthurk    (501) staff       (20)        0 2022-10-05 11:43:05.874414 tritony-0.0.8/
--rw-r--r--   0 Arthurk    (501) staff       (20)     1542 2022-10-05 11:29:44.000000 tritony-0.0.8/LICENSE
--rw-r--r--   0 Arthurk    (501) staff       (20)     2191 2022-10-05 11:43:05.874180 tritony-0.0.8/PKG-INFO
--rw-r--r--   0 Arthurk    (501) staff       (20)      958 2022-07-27 03:53:27.000000 tritony-0.0.8/README.md
--rw-r--r--   0 Arthurk    (501) staff       (20)       38 2022-10-05 11:43:05.874494 tritony-0.0.8/setup.cfg
--rw-r--r--   0 Arthurk    (501) staff       (20)     2176 2022-10-05 11:41:50.000000 tritony-0.0.8/setup.py
-drwxr-xr-x   0 Arthurk    (501) staff       (20)        0 2022-10-05 11:43:05.872393 tritony-0.0.8/tritony/
--rw-r--r--   0 Arthurk    (501) staff       (20)      175 2022-08-08 04:32:47.000000 tritony-0.0.8/tritony/__init__.py
--rw-r--r--   0 Arthurk    (501) staff       (20)     4351 2022-07-27 03:53:27.000000 tritony-0.0.8/tritony/helpers.py
--rw-r--r--   0 Arthurk    (501) staff       (20)    12118 2022-09-22 09:35:17.000000 tritony-0.0.8/tritony/tools.py
--rw-r--r--   0 Arthurk    (501) staff       (20)       22 2022-10-05 11:42:32.000000 tritony-0.0.8/tritony/version.py
-drwxr-xr-x   0 Arthurk    (501) staff       (20)        0 2022-10-05 11:43:05.873847 tritony-0.0.8/tritony.egg-info/
--rw-r--r--   0 Arthurk    (501) staff       (20)     2191 2022-10-05 11:43:05.000000 tritony-0.0.8/tritony.egg-info/PKG-INFO
--rw-r--r--   0 Arthurk    (501) staff       (20)      285 2022-10-05 11:43:05.000000 tritony-0.0.8/tritony.egg-info/SOURCES.txt
--rw-r--r--   0 Arthurk    (501) staff       (20)        1 2022-10-05 11:43:05.000000 tritony-0.0.8/tritony.egg-info/dependency_links.txt
--rw-r--r--   0 Arthurk    (501) staff       (20)        1 2022-09-22 08:26:02.000000 tritony-0.0.8/tritony.egg-info/not-zip-safe
--rw-r--r--   0 Arthurk    (501) staff       (20)      103 2022-10-05 11:43:05.000000 tritony-0.0.8/tritony.egg-info/requires.txt
--rw-r--r--   0 Arthurk    (501) staff       (20)        8 2022-10-05 11:43:05.000000 tritony-0.0.8/tritony.egg-info/top_level.txt
+drwxrwxr-x   0 arthur    (1015) arthur    (1015)        0 2023-04-26 04:31:31.532234 tritony-0.0.9/
+-rw-rw-r--   0 arthur    (1015) arthur    (1015)     1542 2022-11-29 08:41:27.000000 tritony-0.0.9/LICENSE
+-rw-rw-r--   0 arthur    (1015) arthur    (1015)     3953 2023-04-26 04:31:31.533234 tritony-0.0.9/PKG-INFO
+-rw-rw-r--   0 arthur    (1015) arthur    (1015)     2506 2023-04-26 04:30:43.000000 tritony-0.0.9/README.md
+-rw-rw-r--   0 arthur    (1015) arthur    (1015)      116 2023-04-26 04:30:43.000000 tritony-0.0.9/pyproject.toml
+-rw-rw-r--   0 arthur    (1015) arthur    (1015)     2042 2023-04-26 04:31:31.535234 tritony-0.0.9/setup.cfg
+-rw-rw-r--   0 arthur    (1015) arthur    (1015)       69 2023-04-26 04:30:43.000000 tritony-0.0.9/setup.py
+drwxrwxr-x   0 arthur    (1015) arthur    (1015)        0 2023-04-26 04:31:31.517234 tritony-0.0.9/tests/
+-rw-rw-r--   0 arthur    (1015) arthur    (1015)     1883 2023-04-26 04:30:43.000000 tritony-0.0.9/tests/test_connect.py
+-rw-rw-r--   0 arthur    (1015) arthur    (1015)      961 2023-04-26 04:30:43.000000 tritony-0.0.9/tests/test_model_call.py
+drwxrwxr-x   0 arthur    (1015) arthur    (1015)        0 2023-04-26 04:31:31.523234 tritony-0.0.9/tritony/
+-rw-rw-r--   0 arthur    (1015) arthur    (1015)      175 2022-10-26 06:17:08.000000 tritony-0.0.9/tritony/__init__.py
+-rw-rw-r--   0 arthur    (1015) arthur    (1015)     3681 2023-04-26 04:30:43.000000 tritony-0.0.9/tritony/helpers.py
+-rw-rw-r--   0 arthur    (1015) arthur    (1015)    12122 2023-04-26 04:30:43.000000 tritony-0.0.9/tritony/tools.py
+-rw-rw-r--   0 arthur    (1015) arthur    (1015)       22 2023-04-26 04:30:43.000000 tritony-0.0.9/tritony/version.py
+drwxrwxr-x   0 arthur    (1015) arthur    (1015)        0 2023-04-26 04:31:31.531234 tritony-0.0.9/tritony.egg-info/
+-rw-rw-r--   0 arthur    (1015) arthur    (1015)     3953 2023-04-26 04:31:31.000000 tritony-0.0.9/tritony.egg-info/PKG-INFO
+-rw-rw-r--   0 arthur    (1015) arthur    (1015)      357 2023-04-26 04:31:31.000000 tritony-0.0.9/tritony.egg-info/SOURCES.txt
+-rw-rw-r--   0 arthur    (1015) arthur    (1015)        1 2023-04-26 04:31:31.000000 tritony-0.0.9/tritony.egg-info/dependency_links.txt
+-rw-rw-r--   0 arthur    (1015) arthur    (1015)        1 2023-04-26 04:31:31.000000 tritony-0.0.9/tritony.egg-info/not-zip-safe
+-rw-rw-r--   0 arthur    (1015) arthur    (1015)      183 2023-04-26 04:31:31.000000 tritony-0.0.9/tritony.egg-info/requires.txt
+-rw-rw-r--   0 arthur    (1015) arthur    (1015)        8 2023-04-26 04:31:31.000000 tritony-0.0.9/tritony.egg-info/top_level.txt
```

### Comparing `tritony-0.0.8/LICENSE` & `tritony-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tritony-0.0.8/tritony/tools.py` & `tritony-0.0.9/tritony/tools.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import asyncio
 import functools
 import itertools
 import logging
 import os
 import time
 from concurrent.futures import ThreadPoolExecutor
@@ -16,18 +18,18 @@
 from tritonclient.grpc import _get_inference_request as grpc_get_inference_request
 from tritonclient.utils import InferenceServerException
 
 from tritony import ASYNC_TASKS
 from tritony.helpers import (
     COMPRESSION_ALGORITHM_MAP,
     TritonClientFlag,
+    TritonModelSpec,
     TritonProtocol,
     get_triton_client,
     init_triton_client,
-    prepare_triton_flag,
 )
 
 logger = logging.getLogger(__name__)
 
 TRITON_LOAD_DELAY = float(os.environ.get("TRITON_LOAD_DELAY", 3))
 TRITON_BACKOFF_COEFF = float(os.environ.get("TRITON_BACKOFF_COEFF", 0.2))
 TRITON_RETRIES = int(os.environ.get("TRITON_RETRIES", 5))
@@ -58,29 +60,30 @@
 
 
 async def send_request_async(
     inference_client,
     data_queue,
     done_event,
     triton_client: Union[grpcclient.InferenceServerClient, httpclient.InferenceServerClient],
+    model_spec: TritonModelSpec,
 ):
     ret = []
     while True:
         data = asyncio.create_task(data_queue.get())
         done = asyncio.create_task(done_event.wait())
         d, _ = await asyncio.wait({data, done}, return_when=asyncio.FIRST_COMPLETED)
         idx, batch_data = None, None
         if data in d:
             idx, batch_data = data.result()
         elif done in d:
             return ret
         try:
             a_pred = await request_async(
                 inference_client.flag.protocol,
-                inference_client.build_triton_input(batch_data),
+                inference_client.build_triton_input(batch_data, model_spec),
                 triton_client,
                 timeout=inference_client.client_timeout,
                 compression=inference_client.flag.compression_algorithm,
             )
         except InferenceServerException as triton_error:
             handel_triton_error(triton_error)
         ret.append((idx, a_pred))
@@ -99,14 +102,16 @@
 @retry((InferenceServerException, grpc.RpcError), tries=TRITON_RETRIES, delay=TRITON_BACKOFF_COEFF, backoff=2)
 async def request_async(protocol: TritonProtocol, model_input: Dict, triton_client, timeout: int, compression: str):
     st = time.time()
 
     if protocol == TritonProtocol.grpc:
         loop = asyncio.get_running_loop()
 
+        if "parameters" in grpc_get_inference_request.__code__.co_varnames:
+            model_input["parameters"] = None
         request = grpc_get_inference_request(
             **model_input,
             priority=0,
             timeout=timeout,
             sequence_id=0,
             sequence_start=False,
             sequence_end=False,
@@ -125,203 +130,174 @@
 
     ed = time.time()
     logger.debug(f"{model_input['model_name']} {model_input['inputs'][0].shape()} elapsed: {ed - st:.3f}")
 
     return [result.as_numpy(outputs.name()) for outputs in model_input["outputs"]]
 
 
-def worker_parse_args(parser):
-    parser.add_argument(
-        "-v",
-        "--verbose",
-        action="store_true",
-        required=False,
-        default=False,
-        help="Enable verbose output",
-    )
-    parser.add_argument(
-        "-a",
-        "--async",
-        dest="async_set",
-        action="store_true",
-        required=False,
-        default=False,
-        help="Use asynchronous inference API",
-    )
-    parser.add_argument(
-        "--streaming",
-        action="store_true",
-        required=False,
-        default=False,
-        help="Use streaming inference API. " + "The flag is only available with gRPC protocol.",
-    )
-    parser.add_argument("-m", "--model-name", type=str, required=True, help="Name of model")
-    parser.add_argument(
-        "-x",
-        "--model-version",
-        type=str,
-        required=False,
-        default="",
-        help="Version of model. Default is to use latest version.",
-    )
-    parser.add_argument(
-        "-b",
-        "--batch-size",
-        type=int,
-        required=False,
-        default=64,
-        help="Batch size. Default is 1.",
-    )
-    parser.add_argument(
-        "-u",
-        "--url",
-        type=str,
-        required=False,
-        default="localhost:8000",
-        help="Inference server URL. Default is localhost:8000.",
-    )
-    parser.add_argument(
-        "-i",
-        "--protocol",
-        type=str,
-        required=False,
-        default="HTTP",
-        help="Protocol (HTTP/gRPC) used to communicate with " + "the inference service. Default is HTTP.",
-    )
-
-
 class InferenceClient:
     @classmethod
     def create_with(
         cls,
         model: str,
         url: str,
         input_dims: int = 2,
+        model_version: str = "1",
         protocol: str = "grpc",
         run_async: bool = True,
         concurrency: int = ASYNC_TASKS,
         secure: bool = False,
         compression_algorithm: Optional[str] = None,
     ):
         return cls(
-            prepare_triton_flag(
-                model_name=model,
+            TritonClientFlag(
                 url=url,
-                input_dims=input_dims,
+                model_name=model,
+                model_version=model_version,
                 protocol=protocol,
-                run_async=run_async,
+                async_set=run_async,
                 concurrency=concurrency,
+                input_dims=input_dims,
                 compression_algorithm=compression_algorithm,
                 ssl=secure,
             )
         )
 
     def __init__(self, flag: TritonClientFlag):
         self.__version__ = 1
 
         self.flag = flag
-        if self.flag.protocol is TritonProtocol.grpc:
-            self.triton_client: grpcclient.InferenceServerClient = init_triton_client(self.flag)
-        else:
-            self.triton_client: httpclient.InferenceServerClient = init_triton_client(self.flag)
-        self._renew_triton_client()
-
+        self.model_specs = {}
         self.is_async = self.flag.async_set
         self.client_timeout = TRITON_CLIENT_TIMEOUT
+        self._triton_client = None
 
         self.output_kwargs = {}
         self.sent_count = 0
         self.processed_count = 0
 
+    @property
+    def triton_client(self):
+        if self.flag.protocol is TritonProtocol.grpc:
+            self._triton_client: grpcclient.InferenceServerClient = init_triton_client(self.flag)
+        else:
+            self._triton_client: httpclient.InferenceServerClient = init_triton_client(self.flag)
+        self._renew_triton_client(self._triton_client)
+        return self._triton_client
+
     def __del__(self):
-        if self.flag.protocol is TritonProtocol.grpc and self.flag.streaming and hasattr(self, "triton_client"):
-            self.triton_client.stop_stream()
+        # Not supporting streaming
+        # if self.flag.protocol is TritonProtocol.grpc and self.flag.streaming and hasattr(self, "triton_client"):
+        #     self.triton_client.stop_stream()
+        pass
 
     @retry((InferenceServerException, grpc.RpcError), tries=TRITON_RETRIES, delay=TRITON_LOAD_DELAY, backoff=2)
-    def _renew_triton_client(self):
-        self.triton_client.is_server_live()
-        self.triton_client.is_server_ready()
-        self.triton_client.is_model_ready(self.flag.model_name)
-        (
-            self.max_batch_size,
-            self.input_name_list,
-            self.output_name_list,
-            self.dtype_list,
-        ) = get_triton_client(self.triton_client, self.flag)
+    def _renew_triton_client(self, triton_client, model_name: str | None = None, model_version: str | None = None):
+        if not model_name:
+            model_name = self.flag.model_name
+        if not model_version:
+            model_version = self.flag.model_version
+
+        triton_client.is_server_live()
+        triton_client.is_server_ready()
+        triton_client.is_model_ready(model_name, model_version)
+
+        (max_batch_size, input_name_list, output_name_list, dtype_list,) = get_triton_client(
+            triton_client, model_name=model_name, model_version=model_version, protocol=self.flag.protocol
+        )
+
+        self.model_specs[(model_name, model_version)] = TritonModelSpec(
+            name=model_name,
+            max_batch_size=max_batch_size,
+            input_name=input_name_list,
+            input_dtype=dtype_list,
+            output_name=output_name_list,
+        )
 
     def _get_request_id(self):
         self.sent_count += 1
         return self.sent_count
 
-    def __call__(self, sequences_or_dict: Union[List[Any], Dict[str, List[Any]]]):
-        if self.triton_client is None:
-            self._renew_triton_client()
+    def __call__(
+        self,
+        sequences_or_dict: Union[List[Any], Dict[str, List[Any]]],
+        model_name: str | None = None,
+        model_version: str | None = None,
+    ):
+        if model_name is None:
+            model_name = self.flag.model_name
+        if model_version is None:
+            model_version = self.flag.model_version
+        if (model_name, model_version) not in self.model_specs:
+            self._renew_triton_client(self.triton_client, model_name, model_version)
+
+        model_spec = self.model_specs[(model_name, model_version)]
 
         if type(sequences_or_dict) in [list, np.ndarray]:
             sequences_list = [sequences_or_dict]
         elif type(sequences_or_dict) is dict:
-            sequences_list = [sequences_or_dict[input_name] for input_name in self.input_name_list]
+            sequences_list = [sequences_or_dict[input_name] for input_name in model_spec.input_name]
 
-        return self._call_async(sequences_list)
+        return self._call_async(sequences_list, model_spec=model_spec)
 
-    def build_triton_input(self, _input_list: List[np.array]):
+    def build_triton_input(self, _input_list: List[np.array], model_spec: TritonModelSpec):
         if self.flag.protocol is TritonProtocol.grpc:
             client = grpcclient
         else:
             client = httpclient
         infer_input_list = []
-        for _input, _input_name, _dtype in zip(_input_list, self.input_name_list, self.dtype_list):
+        for _input, _input_name, _dtype in zip(_input_list, model_spec.input_name, model_spec.input_dtype):
             infer_input = client.InferInput(_input_name, _input.shape, _dtype)
             infer_input.set_data_from_numpy(_input)
             infer_input_list.append(infer_input)
 
         infer_requested_output = [
-            client.InferRequestedOutput(output_name, **self.output_kwargs) for output_name in self.output_name_list
+            client.InferRequestedOutput(output_name, **self.output_kwargs) for output_name in model_spec.output_name
         ]
 
         request_id = self._get_request_id()
         request_input = dict(
-            model_name=self.flag.model_name,
+            model_name=model_spec.name,
             inputs=infer_input_list,
             request_id=str(request_id),
-            model_version=self.flag.model_version,
+            model_version=model_spec.model_version,
             outputs=infer_requested_output,
         )
 
         return request_input
 
-    def _call_async(self, data: List[np.ndarray]) -> Optional[np.ndarray]:
-        async_result = asyncio.run(self._call_async_item(data=data))
+    def _call_async(self, data: List[np.ndarray], model_spec: TritonModelSpec) -> Optional[np.ndarray]:
+        async_result = asyncio.run(self._call_async_item(data=data, model_spec=model_spec))
 
         if isinstance(async_result, Exception):
             raise async_result
 
         return async_result
 
-    async def _call_async_item(self, data: List[np.ndarray]):
+    async def _call_async_item(self, data: List[np.ndarray], model_spec: TritonModelSpec):
         current_grpc_async_tasks = []
 
         try:
             data_queue = asyncio.Queue(maxsize=ASYNC_TASKS)
             done_event = asyncio.Event()
 
-            generator = asyncio.create_task(data_generator(data, self.max_batch_size, data_queue, done_event))
+            generator = asyncio.create_task(data_generator(data, model_spec.max_batch_size, data_queue, done_event))
             current_grpc_async_tasks.append(generator)
 
             predict_tasks = [
-                asyncio.create_task(send_request_async(self, data_queue, done_event, self.triton_client))
+                asyncio.create_task(send_request_async(self, data_queue, done_event, self.triton_client, model_spec))
                 for idx in range(ASYNC_TASKS)
             ]
             current_grpc_async_tasks.extend(predict_tasks)
 
             ret = await asyncio.gather(*predict_tasks, generator, data_queue.join())
             ret = sorted(itertools.chain(*ret[:ASYNC_TASKS]))
             result_by_req_id = [output_result_list for req_id, output_result_list in ret]
 
-            if self.max_batch_size == 0:
+            if model_spec.max_batch_size == 0:
                 result_by_output_name = list(zip(*result_by_req_id))
             else:
                 result_by_output_name = list(map(lambda ll: np.concatenate(ll, axis=0), zip(*result_by_req_id)))
 
             if len(result_by_output_name) == 1:
                 result_by_output_name = result_by_output_name[0]
```

