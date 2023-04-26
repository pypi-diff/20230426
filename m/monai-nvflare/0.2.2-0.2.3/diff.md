# Comparing `tmp/monai_nvflare-0.2.2-py3-none-any.whl.zip` & `tmp/monai_nvflare-0.2.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 11734 bytes, number of entries: 10
+Zip file size: 11654 bytes, number of entries: 10
 -rw-rw-r--  2.0 unx      842 b- defN 23-Apr-05 22:42 monai_nvflare/__init__.py
 -rw-rw-r--  2.0 unx    10186 b- defN 23-Apr-05 22:42 monai_nvflare/client_algo_executor.py
 -rw-rw-r--  2.0 unx     7394 b- defN 23-Apr-05 22:42 monai_nvflare/client_algo_statistics.py
--rw-rw-r--  2.0 unx     5077 b- defN 23-Apr-05 22:42 monai_nvflare/monai_bundle_persistor.py
+-rw-rw-r--  2.0 unx     4800 b- defN 23-Apr-24 23:59 monai_nvflare/monai_bundle_persistor.py
 -rw-rw-r--  2.0 unx     2145 b- defN 23-Apr-05 22:42 monai_nvflare/monai_data_stats_persistor.py
 -rw-rw-r--  2.0 unx      747 b- defN 23-Apr-05 22:42 monai_nvflare/utils.py
--rw-rw-r--  2.0 unx     2407 b- defN 23-Apr-07 02:03 monai_nvflare-0.2.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-07 02:03 monai_nvflare-0.2.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       14 b- defN 23-Apr-07 02:03 monai_nvflare-0.2.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      868 b- defN 23-Apr-07 02:03 monai_nvflare-0.2.2.dist-info/RECORD
-10 files, 29772 bytes uncompressed, 10238 bytes compressed:  65.6%
+-rw-rw-r--  2.0 unx     2410 b- defN 23-Apr-25 15:10 monai_nvflare-0.2.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-25 15:10 monai_nvflare-0.2.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       14 b- defN 23-Apr-25 15:10 monai_nvflare-0.2.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      868 b- defN 23-Apr-25 15:10 monai_nvflare-0.2.3.dist-info/RECORD
+10 files, 29498 bytes uncompressed, 10158 bytes compressed:  65.6%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: monai_nvflare/monai_data_stats_persistor.py
 Comment: 
 
 Filename: monai_nvflare/utils.py
 Comment: 
 
-Filename: monai_nvflare-0.2.2.dist-info/METADATA
+Filename: monai_nvflare-0.2.3.dist-info/METADATA
 Comment: 
 
-Filename: monai_nvflare-0.2.2.dist-info/WHEEL
+Filename: monai_nvflare-0.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: monai_nvflare-0.2.2.dist-info/top_level.txt
+Filename: monai_nvflare-0.2.3.dist-info/top_level.txt
 Comment: 
 
-Filename: monai_nvflare-0.2.2.dist-info/RECORD
+Filename: monai_nvflare-0.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## monai_nvflare/monai_bundle_persistor.py

```diff
@@ -12,16 +12,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 
 from monai.bundle import ConfigParser
 from monai.bundle.config_item import ConfigItem
-from monai.fl.client.monai_algo import check_bundle_config
-from monai.fl.utils.constants import RequiredBundleKeys
 
 from nvflare.apis.event_type import EventType
 from nvflare.apis.fl_constant import FLContextKey
 from nvflare.apis.fl_context import FLContext
 from nvflare.app_common.app_constant import DefaultCheckpointFileName
 from nvflare.app_opt.pt.file_model_persistor import PTFileModelPersistor
 
@@ -86,18 +84,14 @@
         self.train_parser = ConfigParser()
 
         # Read bundle config files
         app_root = fl_ctx.get_prop(FLContextKey.APP_ROOT)
         self.bundle_root = os.path.join(app_root, self.bundle_root)
 
         self.train_parser.read_config(os.path.join(self.bundle_root, self.config_train_filename))
-        check_bundle_config(self.train_parser)
-
-        # Override some config items
-        self.train_parser[RequiredBundleKeys.BUNDLE_ROOT] = self.bundle_root
 
         if self.source_ckpt_filename:
             self.source_ckpt_file_full_name = os.path.join(self.bundle_root, self.source_ckpt_filename)
 
     def _get_model(self, fl_ctx: FLContext):
         try:
             # Get network config
```

## Comparing `monai_nvflare-0.2.2.dist-info/METADATA` & `monai_nvflare-0.2.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: monai-nvflare
-Version: 0.2.2
+Version: 0.2.3
 Summary: MONAI NVIDIA FLARE integration
 Home-page: https://github.com/NVIDIA/NVFlare
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8,<3.11
 Description-Content-Type: text/markdown
-Requires-Dist: monai (>=1.1.0)
+Requires-Dist: monai (>=1.2.0rc5)
 Requires-Dist: nvflare (>=2.3.0)
 
 # MONAI Integration
 
 ## Objective
 Integration with [MONAI](https://monai.io/)'s federated learning capabilities.
```

