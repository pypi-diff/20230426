# Comparing `tmp/azure-containerregistry-1.1.0b3.zip` & `tmp/azure-containerregistry-1.1.0b4.zip`

## zipinfo {}

```diff
@@ -1,95 +1,96 @@
-Zip file size: 147880 bytes, number of entries: 93
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-05 01:42 azure-containerregistry-1.1.0b3/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-05 01:42 azure-containerregistry-1.1.0b3/azure/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-05 01:42 azure-containerregistry-1.1.0b3/tests/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-05 01:42 azure-containerregistry-1.1.0b3/samples/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-05 01:42 azure-containerregistry-1.1.0b3/azure_containerregistry.egg-info/
--rw-rw-r--  2.0 unx       38 b- defN 23-Apr-05 01:42 azure-containerregistry-1.1.0b3/setup.cfg
--rw-rw-r--  2.0 unx    11022 b- defN 23-Apr-05 01:42 azure-containerregistry-1.1.0b3/PKG-INFO
--rw-rw-r--  2.0 unx     1073 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/LICENSE
--rw-rw-r--  2.0 unx      161 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/MANIFEST.in
--rw-rw-r--  2.0 unx     4159 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/CHANGELOG.md
--rw-rw-r--  2.0 unx     4279 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/TROUBLESHOOTING.md
--rw-rw-r--  2.0 unx     2312 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/setup.py
--rw-rw-r--  2.0 unx       86 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/pyproject.toml
--rw-rw-r--  2.0 unx     9999 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/README.md
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-05 01:42 azure-containerregistry-1.1.0b3/azure/containerregistry/
--rw-rw-r--  2.0 unx       81 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-05 01:42 azure-containerregistry-1.1.0b3/azure/containerregistry/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-05 01:42 azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/
--rw-rw-r--  2.0 unx     2887 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/azure/containerregistry/_anonymous_exchange_client.py
--rw-rw-r--  2.0 unx     4474 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/azure/containerregistry/_helpers.py
--rw-rw-r--  2.0 unx    47251 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/azure/containerregistry/_container_registry_client.py
--rw-rw-r--  2.0 unx     1216 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/azure/containerregistry/__init__.py
--rw-rw-r--  2.0 unx    11997 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/azure/containerregistry/_models.py
--rw-rw-r--  2.0 unx     4273 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/azure/containerregistry/_exchange_client.py
--rw-rw-r--  2.0 unx      248 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/azure/containerregistry/_user_agent.py
--rw-rw-r--  2.0 unx      172 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/azure/containerregistry/_version.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/azure/containerregistry/py.typed
--rw-rw-r--  2.0 unx     2883 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/azure/containerregistry/_base_client.py
--rw-rw-r--  2.0 unx     2504 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/azure/containerregistry/_download_stream.py
--rw-rw-r--  2.0 unx     3862 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/azure/containerregistry/_authentication_policy.py
--rw-rw-r--  2.0 unx      675 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/azure/containerregistry/aio/__init__.py
--rw-rw-r--  2.0 unx     4382 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/azure/containerregistry/aio/_async_exchange_client.py
--rw-rw-r--  2.0 unx    44655 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/azure/containerregistry/aio/_async_container_registry_client.py
--rw-rw-r--  2.0 unx     2667 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/azure/containerregistry/aio/_async_download_stream.py
--rw-rw-r--  2.0 unx     3963 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/azure/containerregistry/aio/_async_authentication_policy.py
--rw-rw-r--  2.0 unx     3244 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/azure/containerregistry/aio/_async_base_client.py
--rw-rw-r--  2.0 unx     3207 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/azure/containerregistry/aio/_async_anonymous_exchange_client.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-05 01:42 azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/models/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-05 01:42 azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-05 01:42 azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/aio/
--rw-rw-r--  2.0 unx      722 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/__init__.py
--rw-rw-r--  2.0 unx     1369 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/_vendor.py
--rw-rw-r--  2.0 unx     1530 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/_patch.py
--rw-rw-r--  2.0 unx     3326 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/_configuration.py
--rw-rw-r--  2.0 unx    78836 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/_serialization.py
--rw-rw-r--  2.0 unx     4629 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/_client.py
--rw-rw-r--  2.0 unx     2960 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/models/_enums.py
--rw-rw-r--  2.0 unx     3412 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/models/__init__.py
--rw-rw-r--  2.0 unx    64464 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/models/_models.py
--rw-rw-r--  2.0 unx      791 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/models/_patch.py
--rw-rw-r--  2.0 unx      870 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/operations/__init__.py
--rw-rw-r--  2.0 unx    10862 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/operations/_patch.py
--rw-rw-r--  2.0 unx   102001 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/operations/_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-05 01:42 azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/aio/operations/
--rw-rw-r--  2.0 unx      722 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/aio/__init__.py
--rw-rw-r--  2.0 unx      845 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/aio/_vendor.py
--rw-rw-r--  2.0 unx     1530 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/aio/_patch.py
--rw-rw-r--  2.0 unx     3368 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/aio/_configuration.py
--rw-rw-r--  2.0 unx     4778 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/aio/_client.py
--rw-rw-r--  2.0 unx      870 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/aio/operations/__init__.py
--rw-rw-r--  2.0 unx     8679 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/aio/operations/_patch.py
--rw-rw-r--  2.0 unx    80597 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/aio/operations/_operations.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-05 01:42 azure-containerregistry-1.1.0b3/tests/perfstress_tests/
--rw-rw-r--  2.0 unx     2145 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/tests/asynctestcase.py
--rw-rw-r--  2.0 unx    25792 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/tests/test_container_registry_client_async.py
--rw-rw-r--  2.0 unx     9002 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/tests/test_anon_access.py
--rw-rw-r--  2.0 unx     1743 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/tests/conftest.py
--rw-rw-r--  2.0 unx     8558 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/tests/testcase.py
--rw-rw-r--  2.0 unx    28203 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/tests/test_container_registry_client.py
--rw-rw-r--  2.0 unx      505 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/tests/preparer.py
--rw-rw-r--  2.0 unx      290 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/tests/constants.py
--rw-rw-r--  2.0 unx     9393 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/tests/test_anon_access_async.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/tests/perfstress_tests/__init__.py
--rw-rw-r--  2.0 unx     1162 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/tests/perfstress_tests/list_repositories.py
--rw-rw-r--  2.0 unx     1235 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/tests/perfstress_tests/list_artifacts.py
--rw-rw-r--  2.0 unx     2745 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/samples/sample_delete_tags.py
--rw-rw-r--  2.0 unx     3136 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/samples/sample_delete_images.py
--rw-rw-r--  2.0 unx     2940 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/samples/sample_delete_tags_async.py
--rw-rw-r--  2.0 unx     3314 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/samples/sample_delete_images_async.py
--rw-rw-r--  2.0 unx     3246 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/samples/sample_hello_world.py
--rw-rw-r--  2.0 unx     2566 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/samples/sample_list_tags.py
--rw-rw-r--  2.0 unx     4767 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/samples/sample_upload_download_manifest.py
--rw-rw-r--  2.0 unx     4356 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/samples/utilities.py
--rw-rw-r--  2.0 unx     3120 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/samples/sample_set_image_properties_async.py
--rw-rw-r--  2.0 unx     2694 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/samples/sample_list_tags_async.py
--rw-rw-r--  2.0 unx     4514 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/samples/README.md
--rw-rw-r--  2.0 unx     3000 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/samples/sample_set_image_properties.py
--rw-rw-r--  2.0 unx     3388 b- defN 23-Apr-05 01:41 azure-containerregistry-1.1.0b3/samples/sample_hello_world_async.py
--rw-rw-r--  2.0 unx    11022 b- defN 23-Apr-05 01:42 azure-containerregistry-1.1.0b3/azure_containerregistry.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx        1 b- defN 23-Apr-05 01:42 azure-containerregistry-1.1.0b3/azure_containerregistry.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx       41 b- defN 23-Apr-05 01:42 azure-containerregistry-1.1.0b3/azure_containerregistry.egg-info/requires.txt
--rw-rw-r--  2.0 unx     3134 b- defN 23-Apr-05 01:42 azure-containerregistry-1.1.0b3/azure_containerregistry.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx        6 b- defN 23-Apr-05 01:42 azure-containerregistry-1.1.0b3/azure_containerregistry.egg-info/top_level.txt
-93 files, 700949 bytes uncompressed, 128010 bytes compressed:  81.7%
+Zip file size: 153094 bytes, number of entries: 94
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-26 00:32 azure-containerregistry-1.1.0b4/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-26 00:32 azure-containerregistry-1.1.0b4/tests/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-26 00:32 azure-containerregistry-1.1.0b4/azure/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-26 00:32 azure-containerregistry-1.1.0b4/samples/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-26 00:32 azure-containerregistry-1.1.0b4/azure_containerregistry.egg-info/
+-rw-rw-r--  2.0 unx     2312 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/setup.py
+-rw-rw-r--  2.0 unx       38 b- defN 23-Apr-26 00:32 azure-containerregistry-1.1.0b4/setup.cfg
+-rw-rw-r--  2.0 unx      161 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/MANIFEST.in
+-rw-rw-r--  2.0 unx       86 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/pyproject.toml
+-rw-rw-r--  2.0 unx     4713 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/CHANGELOG.md
+-rw-rw-r--  2.0 unx    11022 b- defN 23-Apr-26 00:32 azure-containerregistry-1.1.0b4/PKG-INFO
+-rw-rw-r--  2.0 unx     4279 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/TROUBLESHOOTING.md
+-rw-rw-r--  2.0 unx     1073 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/LICENSE
+-rw-rw-r--  2.0 unx     9999 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/README.md
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-26 00:32 azure-containerregistry-1.1.0b4/tests/perfstress_tests/
+-rw-rw-r--  2.0 unx     7543 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/tests/testcase.py
+-rw-rw-r--  2.0 unx     1743 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/tests/conftest.py
+-rw-rw-r--  2.0 unx    39478 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/tests/test_container_registry_client.py
+-rw-rw-r--  2.0 unx     9393 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/tests/test_anon_access_async.py
+-rw-rw-r--  2.0 unx     3121 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/tests/asynctestcase.py
+-rw-rw-r--  2.0 unx     9002 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/tests/test_anon_access.py
+-rw-rw-r--  2.0 unx      290 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/tests/constants.py
+-rw-rw-r--  2.0 unx      505 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/tests/preparer.py
+-rw-rw-r--  2.0 unx    41494 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/tests/test_container_registry_client_async.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/tests/perfstress_tests/__init__.py
+-rw-rw-r--  2.0 unx     1235 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/tests/perfstress_tests/list_artifacts.py
+-rw-rw-r--  2.0 unx     1162 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/tests/perfstress_tests/list_repositories.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-26 00:32 azure-containerregistry-1.1.0b4/azure/containerregistry/
+-rw-rw-r--  2.0 unx       81 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-26 00:32 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-26 00:32 azure-containerregistry-1.1.0b4/azure/containerregistry/aio/
+-rw-rw-r--  2.0 unx     2504 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_download_stream.py
+-rw-rw-r--  2.0 unx     1206 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/__init__.py
+-rw-rw-r--  2.0 unx     4273 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_exchange_client.py
+-rw-rw-r--  2.0 unx    11863 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_models.py
+-rw-rw-r--  2.0 unx     2883 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_base_client.py
+-rw-rw-r--  2.0 unx     3862 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_authentication_policy.py
+-rw-rw-r--  2.0 unx      248 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_user_agent.py
+-rw-rw-r--  2.0 unx    47682 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_container_registry_client.py
+-rw-rw-r--  2.0 unx     2887 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_anonymous_exchange_client.py
+-rw-rw-r--  2.0 unx      172 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_version.py
+-rw-rw-r--  2.0 unx     4717 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_helpers.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/py.typed
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-26 00:32 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-26 00:32 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-26 00:32 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/operations/
+-rw-rw-r--  2.0 unx     4629 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/_client.py
+-rw-rw-r--  2.0 unx      722 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/__init__.py
+-rw-rw-r--  2.0 unx     3326 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/_configuration.py
+-rw-rw-r--  2.0 unx     1530 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/_patch.py
+-rw-rw-r--  2.0 unx     1369 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/_vendor.py
+-rw-rw-r--  2.0 unx    78836 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/_serialization.py
+-rw-rw-r--  2.0 unx     3412 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/models/__init__.py
+-rw-rw-r--  2.0 unx    64438 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/models/_models.py
+-rw-rw-r--  2.0 unx      791 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/models/_patch.py
+-rw-rw-r--  2.0 unx     2960 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/models/_enums.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-26 00:32 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/operations/
+-rw-rw-r--  2.0 unx     4778 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/_client.py
+-rw-rw-r--  2.0 unx      722 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/__init__.py
+-rw-rw-r--  2.0 unx     3368 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/_configuration.py
+-rw-rw-r--  2.0 unx     1530 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/_patch.py
+-rw-rw-r--  2.0 unx      845 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/_vendor.py
+-rw-rw-r--  2.0 unx      870 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx     8679 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx    80761 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/operations/_operations.py
+-rw-rw-r--  2.0 unx      870 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/operations/__init__.py
+-rw-rw-r--  2.0 unx    10863 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/operations/_patch.py
+-rw-rw-r--  2.0 unx   103037 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/operations/_operations.py
+-rw-rw-r--  2.0 unx    49024 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/aio/_async_container_registry_client.py
+-rw-rw-r--  2.0 unx     3963 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/aio/_async_authentication_policy.py
+-rw-rw-r--  2.0 unx     3207 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/aio/_async_anonymous_exchange_client.py
+-rw-rw-r--  2.0 unx      675 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/aio/__init__.py
+-rw-rw-r--  2.0 unx     2667 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/aio/_async_download_stream.py
+-rw-rw-r--  2.0 unx     4382 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/aio/_async_exchange_client.py
+-rw-rw-r--  2.0 unx     3244 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/aio/_async_base_client.py
+-rw-rw-r--  2.0 unx     6940 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/samples/sample_set_get_image_async.py
+-rw-rw-r--  2.0 unx     3000 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/samples/sample_set_image_properties.py
+-rw-rw-r--  2.0 unx     3314 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/samples/sample_delete_images_async.py
+-rw-rw-r--  2.0 unx     2566 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/samples/sample_list_tags.py
+-rw-rw-r--  2.0 unx     2694 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/samples/sample_list_tags_async.py
+-rw-rw-r--  2.0 unx     3246 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/samples/sample_hello_world.py
+-rw-rw-r--  2.0 unx     6689 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/samples/sample_set_get_image.py
+-rw-rw-r--  2.0 unx     4356 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/samples/utilities.py
+-rw-rw-r--  2.0 unx     2745 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/samples/sample_delete_tags.py
+-rw-rw-r--  2.0 unx     3136 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/samples/sample_delete_images.py
+-rw-rw-r--  2.0 unx     3388 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/samples/sample_hello_world_async.py
+-rw-rw-r--  2.0 unx     2940 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/samples/sample_delete_tags_async.py
+-rw-rw-r--  2.0 unx     4698 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/samples/README.md
+-rw-rw-r--  2.0 unx     3120 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/samples/sample_set_image_properties_async.py
+-rw-rw-r--  2.0 unx       41 b- defN 23-Apr-26 00:32 azure-containerregistry-1.1.0b4/azure_containerregistry.egg-info/requires.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Apr-26 00:32 azure-containerregistry-1.1.0b4/azure_containerregistry.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx        6 b- defN 23-Apr-26 00:32 azure-containerregistry-1.1.0b4/azure_containerregistry.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx    11022 b- defN 23-Apr-26 00:32 azure-containerregistry-1.1.0b4/azure_containerregistry.egg-info/PKG-INFO
+-rw-rw-r--  2.0 unx     3161 b- defN 23-Apr-26 00:32 azure-containerregistry-1.1.0b4/azure_containerregistry.egg-info/SOURCES.txt
+94 files, 743588 bytes uncompressed, 133032 bytes compressed:  82.1%
```

## zipnote {}

```diff
@@ -1,280 +1,283 @@
-Filename: azure-containerregistry-1.1.0b3/
+Filename: azure-containerregistry-1.1.0b4/
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/
+Filename: azure-containerregistry-1.1.0b4/tests/
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/tests/
+Filename: azure-containerregistry-1.1.0b4/azure/
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/samples/
+Filename: azure-containerregistry-1.1.0b4/samples/
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure_containerregistry.egg-info/
+Filename: azure-containerregistry-1.1.0b4/azure_containerregistry.egg-info/
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/setup.cfg
+Filename: azure-containerregistry-1.1.0b4/setup.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/PKG-INFO
+Filename: azure-containerregistry-1.1.0b4/setup.cfg
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/LICENSE
+Filename: azure-containerregistry-1.1.0b4/MANIFEST.in
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/MANIFEST.in
+Filename: azure-containerregistry-1.1.0b4/pyproject.toml
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/CHANGELOG.md
+Filename: azure-containerregistry-1.1.0b4/CHANGELOG.md
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/TROUBLESHOOTING.md
+Filename: azure-containerregistry-1.1.0b4/PKG-INFO
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/setup.py
+Filename: azure-containerregistry-1.1.0b4/TROUBLESHOOTING.md
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/pyproject.toml
+Filename: azure-containerregistry-1.1.0b4/LICENSE
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/README.md
+Filename: azure-containerregistry-1.1.0b4/README.md
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/
+Filename: azure-containerregistry-1.1.0b4/tests/perfstress_tests/
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/__init__.py
+Filename: azure-containerregistry-1.1.0b4/tests/testcase.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/aio/
+Filename: azure-containerregistry-1.1.0b4/tests/conftest.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/
+Filename: azure-containerregistry-1.1.0b4/tests/test_container_registry_client.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/_anonymous_exchange_client.py
+Filename: azure-containerregistry-1.1.0b4/tests/test_anon_access_async.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/_helpers.py
+Filename: azure-containerregistry-1.1.0b4/tests/asynctestcase.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/_container_registry_client.py
+Filename: azure-containerregistry-1.1.0b4/tests/test_anon_access.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/__init__.py
+Filename: azure-containerregistry-1.1.0b4/tests/constants.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/_models.py
+Filename: azure-containerregistry-1.1.0b4/tests/preparer.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/_exchange_client.py
+Filename: azure-containerregistry-1.1.0b4/tests/test_container_registry_client_async.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/_user_agent.py
+Filename: azure-containerregistry-1.1.0b4/tests/perfstress_tests/__init__.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/_version.py
+Filename: azure-containerregistry-1.1.0b4/tests/perfstress_tests/list_artifacts.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/py.typed
+Filename: azure-containerregistry-1.1.0b4/tests/perfstress_tests/list_repositories.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/_base_client.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/_download_stream.py
+Filename: azure-containerregistry-1.1.0b4/azure/__init__.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/_authentication_policy.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/aio/__init__.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/aio/
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/aio/_async_exchange_client.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_download_stream.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/aio/_async_container_registry_client.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/__init__.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/aio/_async_download_stream.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_exchange_client.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/aio/_async_authentication_policy.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_models.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/aio/_async_base_client.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_base_client.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/aio/_async_anonymous_exchange_client.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_authentication_policy.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/models/
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_user_agent.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/operations/
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_container_registry_client.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/aio/
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_anonymous_exchange_client.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/__init__.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_version.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/_vendor.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_helpers.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/_patch.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/py.typed
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/_configuration.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/models/
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/_serialization.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/_client.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/operations/
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/models/_enums.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/_client.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/models/__init__.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/__init__.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/models/_models.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/_configuration.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/models/_patch.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/_patch.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/operations/__init__.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/_vendor.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/operations/_patch.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/_serialization.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/operations/_operations.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/models/__init__.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/aio/operations/
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/models/_models.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/aio/__init__.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/models/_patch.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/aio/_vendor.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/models/_enums.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/aio/_patch.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/operations/
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/aio/_configuration.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/_client.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/aio/_client.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/__init__.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/aio/operations/__init__.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/_configuration.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/aio/operations/_patch.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/_patch.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/aio/operations/_operations.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/_vendor.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/tests/perfstress_tests/
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/tests/asynctestcase.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/tests/test_container_registry_client_async.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/operations/_operations.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/tests/test_anon_access.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/operations/__init__.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/tests/conftest.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/operations/_patch.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/tests/testcase.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/operations/_operations.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/tests/test_container_registry_client.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/aio/_async_container_registry_client.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/tests/preparer.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/aio/_async_authentication_policy.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/tests/constants.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/aio/_async_anonymous_exchange_client.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/tests/test_anon_access_async.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/aio/__init__.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/tests/perfstress_tests/__init__.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/aio/_async_download_stream.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/tests/perfstress_tests/list_repositories.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/aio/_async_exchange_client.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/tests/perfstress_tests/list_artifacts.py
+Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/aio/_async_base_client.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/samples/sample_delete_tags.py
+Filename: azure-containerregistry-1.1.0b4/samples/sample_set_get_image_async.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/samples/sample_delete_images.py
+Filename: azure-containerregistry-1.1.0b4/samples/sample_set_image_properties.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/samples/sample_delete_tags_async.py
+Filename: azure-containerregistry-1.1.0b4/samples/sample_delete_images_async.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/samples/sample_delete_images_async.py
+Filename: azure-containerregistry-1.1.0b4/samples/sample_list_tags.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/samples/sample_hello_world.py
+Filename: azure-containerregistry-1.1.0b4/samples/sample_list_tags_async.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/samples/sample_list_tags.py
+Filename: azure-containerregistry-1.1.0b4/samples/sample_hello_world.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/samples/sample_upload_download_manifest.py
+Filename: azure-containerregistry-1.1.0b4/samples/sample_set_get_image.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/samples/utilities.py
+Filename: azure-containerregistry-1.1.0b4/samples/utilities.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/samples/sample_set_image_properties_async.py
+Filename: azure-containerregistry-1.1.0b4/samples/sample_delete_tags.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/samples/sample_list_tags_async.py
+Filename: azure-containerregistry-1.1.0b4/samples/sample_delete_images.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/samples/README.md
+Filename: azure-containerregistry-1.1.0b4/samples/sample_hello_world_async.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/samples/sample_set_image_properties.py
+Filename: azure-containerregistry-1.1.0b4/samples/sample_delete_tags_async.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/samples/sample_hello_world_async.py
+Filename: azure-containerregistry-1.1.0b4/samples/README.md
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure_containerregistry.egg-info/PKG-INFO
+Filename: azure-containerregistry-1.1.0b4/samples/sample_set_image_properties_async.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure_containerregistry.egg-info/dependency_links.txt
+Filename: azure-containerregistry-1.1.0b4/azure_containerregistry.egg-info/requires.txt
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure_containerregistry.egg-info/requires.txt
+Filename: azure-containerregistry-1.1.0b4/azure_containerregistry.egg-info/dependency_links.txt
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure_containerregistry.egg-info/SOURCES.txt
+Filename: azure-containerregistry-1.1.0b4/azure_containerregistry.egg-info/top_level.txt
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b3/azure_containerregistry.egg-info/top_level.txt
+Filename: azure-containerregistry-1.1.0b4/azure_containerregistry.egg-info/PKG-INFO
+Comment: 
+
+Filename: azure-containerregistry-1.1.0b4/azure_containerregistry.egg-info/SOURCES.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-containerregistry-1.1.0b3/PKG-INFO` & `azure-containerregistry-1.1.0b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-containerregistry
-Version: 1.1.0b3
+Version: 1.1.0b4
 Summary: Microsoft Azure Azure Container Registry Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azuresdkengsysadmins@microsoft.com
 License: MIT License
 Project-URL: Bug Reports, https://github.com/Azure/azure-sdk-for-python/issues
 Project-URL: Source, https://github.com/Azure/azure-sdk-python
```

## Comparing `azure-containerregistry-1.1.0b3/LICENSE` & `azure-containerregistry-1.1.0b4/LICENSE`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b3/CHANGELOG.md` & `azure-containerregistry-1.1.0b4/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,21 @@
 # Release History
 
+## 1.1.0b4 (2023-04-25)
+
+### Features Added
+- Added an optional kwarg `media_type` in `set_manifest()` to enable uploading image manifests of any type.
+
+### Breaking Changes
+- Renamed `upload_manifest()` to `set_manifest()`, and changed to consume manifest in `JSON` instead of `OCIManifest` type.
+- Renamed `download_manifest()` to `get_manifest()`, and changed it's return type from `DownloadManifestResult` to `GetManifestResult`.
+
+### Other Changes
+- Changed the default audience to `"https://containerregistry.azure.net"` which works for all clouds.
+
 ## 1.1.0b3 (2023-04-04)
 
 ### Features Added
 - Supported uploading and downding large OCI artifact blobs in synchronous and asynchronous `ContainerRegistryClient`.
 - Published model `DownloadManifestResult`, `DownloadBlobStream` and `AsyncDownloadBlobStream`.
 
 ### Breaking Changes
@@ -50,15 +62,15 @@
 - Python 2.7 is no longer supported. Please use Python version 3.6 or later.
 
 ## 1.0.0b7 (2021-11-19)
 
 ### Features Added
 
 - Updated the supported rest api version to be the stable "2021-07-01".
-  - Removed the property `teleport_enabled` in `RepositoryProperties`.
+- Removed the property `teleport_enabled` in `RepositoryProperties`.
 
 ## 1.0.0b6 (2021-09-08)
 
 ### Breaking Changes
 
 - Removed `credential_scopes` keyword.
 - Added `audience` keyword, which allows customers to select from available audiences or provide their own audience string. This keyword is required when creating a client.
```

## Comparing `azure-containerregistry-1.1.0b3/TROUBLESHOOTING.md` & `azure-containerregistry-1.1.0b4/TROUBLESHOOTING.md`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b3/setup.py` & `azure-containerregistry-1.1.0b4/setup.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b3/README.md` & `azure-containerregistry-1.1.0b4/README.md`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b3/azure/containerregistry/_anonymous_exchange_client.py` & `azure-containerregistry-1.1.0b4/azure/containerregistry/_anonymous_exchange_client.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b3/azure/containerregistry/_helpers.py` & `azure-containerregistry-1.1.0b4/azure/containerregistry/_helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,34 +4,46 @@
 # Licensed under the MIT License.
 # ------------------------------------
 import base64
 import hashlib
 import re
 import time
 import json
-from typing import List, Dict, IO, Optional
-from io import BytesIO
+from typing import Any, List, Dict, MutableMapping, IO, Optional, Union
 from urllib.parse import urlparse
-
 from azure.core.exceptions import ServiceRequestError
 from azure.core.pipeline import PipelineRequest
-from ._generated.models import OCIManifest
+
+JSON = MutableMapping[str, Any]
 
 BEARER = "Bearer"
 AUTHENTICATION_CHALLENGE_PARAMS_PATTERN = re.compile('(?:(\\w+)="([^""]*)")+')
 SUPPORTED_API_VERSIONS = [
     "2019-08-15-preview",
     "2021-07-01"
 ]
-OCI_MANIFEST_MEDIA_TYPE = "application/vnd.oci.image.manifest.v1+json"
 DEFAULT_CHUNK_SIZE = 4 * 1024 * 1024 # 4MB
 
-# Public cloud audience
-AZURE_RESOURCE_MANAGER_PUBLIC_CLOUD = "https://management.azure.com"
+# The default audience used for all clouds when audience is not set
+DEFAULT_AUDIENCE = "https://containerregistry.azure.net"
 
+# Known manifest media types
+OCI_IMAGE_MANIFEST = "application/vnd.oci.image.manifest.v1+json"
+DOCKER_MANIFEST = "application/vnd.docker.distribution.manifest.v2+json"
+
+SUPPORTED_MANIFEST_MEDIA_TYPES = ", ".join(
+    [
+        "*/*",
+        OCI_IMAGE_MANIFEST,
+        DOCKER_MANIFEST,
+        "application/vnd.oci.image.index.v1+json",
+        "application/vnd.docker.distribution.manifest.list.v2+json",
+        "application/vnd.cncf.oras.artifact.manifest.v1+json"
+    ]
+)
 
 def _is_tag(tag_or_digest: str) -> bool:
     tag = tag_or_digest.split(":")
     return not (len(tag) == 2 and tag[0].startswith("sha"))
 
 def _clean(matches: List[str]) -> None:
     """This method removes empty strings and commas from the regex matching of the Challenge header"""
@@ -111,26 +123,19 @@
             value += "=" * padding
         byte_value = base64.b64decode(value).decode("utf-8")
         web_token = json.loads(byte_value)
         return web_token.get("exp", time.time())
 
     return time.time()
 
-def _serialize_manifest(manifest: OCIManifest) -> IO:
-    data = json.dumps(manifest.serialize()).encode('utf-8')
-    return BytesIO(data)
-
-def _deserialize_manifest(data: IO) -> OCIManifest:
-    data.seek(0)
-    value = data.read()
-    data.seek(0)
-    return OCIManifest.deserialize(json.loads(value.decode()))
-
-def _compute_digest(data: IO) -> str:
-    data.seek(0)
-    value = data.read()
-    data.seek(0)
+def _compute_digest(data: Union[IO[bytes], bytes]) -> str:
+    if isinstance(data, bytes):
+        value = data
+    else:
+        data.seek(0)
+        value = data.read()
+        data.seek(0)
     return "sha256:" + hashlib.sha256(value).hexdigest()
 
-def _validate_digest(data: IO, digest: str) -> bool:
-    data_digest = _compute_digest(data)
-    return data_digest == digest
+def _validate_digest(data: Union[IO[bytes], bytes], expected_digest: str) -> bool:
+    digest = _compute_digest(data)
+    return digest == expected_digest
```

## Comparing `azure-containerregistry-1.1.0b3/azure/containerregistry/_container_registry_client.py` & `azure-containerregistry-1.1.0b4/azure/containerregistry/_container_registry_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,52 +2,55 @@
 # ------------------------------------
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 # ------------------------------------
 # pylint: disable=too-many-lines
 import functools
 import hashlib
+import json
 from io import BytesIO
-from typing import Any, Dict, IO, Optional, overload, Union, cast, Tuple
+from typing import Any, Dict, IO, Optional, overload, Union, cast, Tuple, MutableMapping
 
 from azure.core.credentials import TokenCredential
 from azure.core.exceptions import (
     ClientAuthenticationError,
     ResourceNotFoundError,
     ResourceExistsError,
     HttpResponseError,
     map_error,
 )
 from azure.core.paging import ItemPaged
 from azure.core.pipeline import PipelineResponse
 from azure.core.tracing.decorator import distributed_trace
 
 from ._base_client import ContainerRegistryBaseClient
-from ._generated.models import AcrErrors, OCIManifest, ManifestWrapper
+from ._generated.models import AcrErrors
 from ._download_stream import DownloadBlobStream
 from ._helpers import (
     _compute_digest,
     _is_tag,
     _parse_next_link,
-    _serialize_manifest,
     _validate_digest,
-    OCI_MANIFEST_MEDIA_TYPE,
     SUPPORTED_API_VERSIONS,
-    AZURE_RESOURCE_MANAGER_PUBLIC_CLOUD,
+    OCI_IMAGE_MANIFEST,
+    SUPPORTED_MANIFEST_MEDIA_TYPES,
+    DEFAULT_AUDIENCE,
     DEFAULT_CHUNK_SIZE,
 )
 from ._models import (
     RepositoryProperties,
     ArtifactTagProperties,
     ArtifactManifestProperties,
-    DownloadManifestResult,
+    GetManifestResult,
 )
 
-def _return_response_and_deserialized(pipeline_response, deserialized, _):
-    return pipeline_response, deserialized
+JSON = MutableMapping[str, Any]
+
+def _return_response(pipeline_response, _, __):
+    return pipeline_response
 
 def _return_response_and_headers(pipeline_response, _, response_headers):
     return pipeline_response, response_headers
 
 def _return_response_headers(_, __, response_headers):
     return response_headers
 
@@ -55,28 +58,28 @@
 class ContainerRegistryClient(ContainerRegistryBaseClient):
     def __init__(
         self,
         endpoint: str,
         credential: Optional[TokenCredential] = None,
         *,
         api_version: Optional[str] = None,
-        audience: str = AZURE_RESOURCE_MANAGER_PUBLIC_CLOUD,
+        audience: str = DEFAULT_AUDIENCE,
         **kwargs
     ) -> None:
         """Create a ContainerRegistryClient from an ACR endpoint and a credential.
 
         :param str endpoint: An ACR endpoint.
         :param credential: The credential with which to authenticate. This should be None in anonymous access.
         :type credential: ~azure.core.credentials.TokenCredential or None
         :keyword api_version: API Version. The default value is "2021-07-01". Note that overriding this default value
          may result in unsupported behavior.
         :paramtype api_version: str
         :keyword audience: URL to use for credential authentication with AAD. Its value could be
             "https://management.azure.com", "https://management.chinacloudapi.cn" or
-            "https://management.usgovcloudapi.net". The default value is "https://management.azure.com".
+            "https://management.usgovcloudapi.net". The default value is "https://containerregistry.azure.net".
         :paramtype audience: str
         :returns: None
         :rtype: None
         :raises ValueError: If the provided api_version keyword-only argument isn't supported.
 
         .. admonition:: Example:
 
@@ -855,57 +858,103 @@
         return RepositoryProperties._from_generated(  # pylint: disable=protected-access
             self._client.container_registry.update_properties(
                 repository, value=properties._to_generated(), **kwargs  # pylint: disable=protected-access
             )
         )
 
     @distributed_trace
-    def upload_manifest(
-        self, repository: str, manifest: Union[OCIManifest, IO], *, tag: Optional[str] = None, **kwargs
+    def set_manifest(
+        self,
+        repository: str,
+        manifest: Union[JSON, IO[bytes]],
+        *,
+        tag: Optional[str] = None,
+        media_type: str = OCI_IMAGE_MANIFEST,
+        **kwargs
     ) -> str:
-        """Upload a manifest for an OCI artifact.
+        """Set a manifest for an artifact.
 
-        :param str repository: Name of the repository.
-        :param manifest: The manifest to upload. Note: This must be a seekable stream.
-        :type manifest: ~azure.containerregistry.models.OCIManifest or IO
+        :param str repository: Name of the repository
+        :param manifest: The manifest to set. It can be a JSON formatted dict or seekable stream.
+        :type manifest: dict or IO
         :keyword tag: Tag of the manifest.
         :paramtype tag: str or None
-        :returns: The digest of the uploaded manifest, calculated by the registry.
+        :keyword media_type: The media type of the manifest. If not specified, this value will be set to
+            a default value of "application/vnd.oci.image.manifest.v1+json". Note: the current known media types are:
+            "application/vnd.oci.image.manifest.v1+json", and "application/vnd.docker.distribution.manifest.v2+json".
+        :paramtype media_type: str
+        :returns: The digest of the set manifest, calculated by the registry.
         :rtype: str
         :raises ValueError: If the parameter repository or manifest is None,
-            or the digest in the response does not match the digest of the uploaded manifest.
+            or the digest in the response does not match the digest of the set manifest.
         """
         try:
-            if isinstance(manifest, OCIManifest):
-                data = _serialize_manifest(manifest)
+            data: IO[bytes]
+            if isinstance(manifest, MutableMapping):
+                data = BytesIO(json.dumps(manifest).encode())
             else:
                 data = manifest
             tag_or_digest = tag
             if tag_or_digest is None:
                 tag_or_digest = _compute_digest(data)
 
             response_headers = self._client.container_registry.create_manifest(
                 name=repository,
                 reference=tag_or_digest,
                 payload=data,
-                content_type=OCI_MANIFEST_MEDIA_TYPE,
-                headers={"Accept": OCI_MANIFEST_MEDIA_TYPE},
+                content_type=media_type,
                 cls=_return_response_headers,
                 **kwargs
             )
             digest = response_headers['Docker-Content-Digest']
             if not _validate_digest(data, digest):
-                raise ValueError("The digest in the response does not match the digest of the uploaded manifest.")
+                raise ValueError("The server-computed digest does not match the client-computed digest.")
         except Exception as e:
             if repository is None or manifest is None:
                 raise ValueError("The parameter repository and manifest cannot be None.") from e
             raise
         return digest
 
     @distributed_trace
+    def get_manifest(self, repository: str, tag_or_digest: str, **kwargs) -> GetManifestResult:
+        """Get the manifest for an artifact.
+
+        :param str repository: Name of the repository.
+        :param str tag_or_digest: The tag or digest of the manifest to get.
+            When digest is provided, will use this digest to compare with the one calculated by the response payload.
+            When tag is provided, will use the digest in response headers to compare.
+        :returns: GetManifestResult
+        :rtype: ~azure.containerregistry.GetManifestResult
+        :raises ValueError: If the requested digest does not match the digest of the received manifest.
+        """
+        response = cast(
+            PipelineResponse,
+            self._client.container_registry.get_manifest(
+                name=repository,
+                reference=tag_or_digest,
+                accept=SUPPORTED_MANIFEST_MEDIA_TYPES,
+                cls=_return_response,
+                **kwargs
+            )
+        )
+        media_type = response.http_response.headers['Content-Type']
+        manifest_bytes = response.http_response.read()
+        manifest_json = response.http_response.json()
+        if tag_or_digest.startswith("sha256:"):
+            digest = tag_or_digest
+            if not _validate_digest(manifest_bytes, digest):
+                raise ValueError("The requested digest does not match the digest of the received manifest.")
+        else:
+            digest = response.http_response.headers['Docker-Content-Digest']
+            if not _validate_digest(manifest_bytes, digest):
+                raise ValueError("The server-computed digest does not match the client-computed digest.")
+
+        return GetManifestResult(digest=digest, manifest=manifest_json, media_type=media_type)
+
+    @distributed_trace
     def upload_blob(self, repository: str, data: IO[bytes], **kwargs) -> Tuple[str, int]:
         """Upload an artifact blob.
 
         :param str repository: Name of the repository.
         :param data: The blob to upload. Note: This must be a seekable stream.
         :type data: IO
         :returns: The digest and size in bytes of the uploaded blob.
@@ -945,48 +994,15 @@
                 cls=_return_response_headers,
                 **kwargs
             ))
             location = response_headers['Location']
             hasher.update(buffer)
             buffer = data.read(DEFAULT_CHUNK_SIZE)
             blob_size += len(buffer)
-        return "sha256:" + hasher.hexdigest(), location, blob_size
-
-    @distributed_trace
-    def download_manifest(self, repository: str, tag_or_digest: str, **kwargs) -> DownloadManifestResult:
-        """Download the manifest for an OCI artifact.
-
-        :param str repository: Name of the repository.
-        :param str tag_or_digest: The tag or digest of the manifest to download.
-            When digest is provided, will use this digest to compare with the one calculated by the response payload.
-            When tag is provided, will use the digest in response headers to compare.
-        :returns: DownloadManifestResult
-        :rtype: ~azure.containerregistry.DownloadManifestResult
-        :raises ValueError: If the requested digest does not match the digest of the received manifest.
-        """
-        response, manifest_wrapper = cast(
-            Tuple[PipelineResponse, ManifestWrapper],
-            self._client.container_registry.get_manifest(
-                name=repository,
-                reference=tag_or_digest,
-                headers={"Accept": OCI_MANIFEST_MEDIA_TYPE},
-                cls=_return_response_and_deserialized,
-                **kwargs
-            )
-        )
-        manifest = OCIManifest.deserialize(cast(ManifestWrapper, manifest_wrapper).serialize())
-        manifest_stream = _serialize_manifest(manifest)
-        if tag_or_digest.startswith("sha256:"):
-            digest = tag_or_digest
-        else:
-            digest = response.http_response.headers['Docker-Content-Digest']
-        if not _validate_digest(manifest_stream, digest):
-            raise ValueError("The requested digest does not match the digest of the received manifest.")
-
-        return DownloadManifestResult(digest=digest, data=manifest_stream, manifest=manifest)
+        return f"sha256:{hasher.hexdigest()}", location, blob_size
 
     @distributed_trace
     def download_blob(self, repository: str, digest: str, **kwargs) -> DownloadBlobStream:
         """Download a blob that is part of an artifact to a stream.
 
         :param str repository: Name of the repository.
         :param str digest: The digest of the blob to download.
```

## Comparing `azure-containerregistry-1.1.0b3/azure/containerregistry/__init__.py` & `azure-containerregistry-1.1.0b4/azure/containerregistry/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 )
 from ._models import (
     ArtifactArchitecture,
     ArtifactOperatingSystem,
     ArtifactManifestProperties,
     RepositoryProperties,
     ArtifactTagProperties,
-    DownloadManifestResult,
+    GetManifestResult,
 )
 from ._download_stream import DownloadBlobStream
 from ._version import VERSION
 
 __version__ = VERSION
 
 __all__ = [
@@ -29,10 +29,10 @@
     "ArtifactOperatingSystem",
     "ContainerRegistryClient",
     "ArtifactManifestOrder",
     "ArtifactManifestProperties",
     "RepositoryProperties",
     "ArtifactTagOrder",
     "ArtifactTagProperties",
-    "DownloadManifestResult",
+    "GetManifestResult",
     "DownloadBlobStream",
 ]
```

## Comparing `azure-containerregistry-1.1.0b3/azure/containerregistry/_models.py` & `azure-containerregistry-1.1.0b4/azure/containerregistry/_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 # ------------------------------------
 import warnings
 from datetime import datetime
 from enum import Enum
 from typing import List
 
 from azure.core import CaseInsensitiveEnumMeta
-
 from ._generated.models import (
     ContainerRepositoryProperties as GeneratedRepositoryProperties,
     RepositoryWriteableProperties,
     TagWriteableProperties,
     TagAttributesBase,
     ManifestWriteableProperties,
     ManifestAttributesBase,
@@ -301,21 +300,19 @@
         return self._name
 
     @property
     def repository_name(self) -> str:
         return self._repository_name
 
 
-class DownloadManifestResult(object):
-    """The result from downloading a manifest from the registry.
+class GetManifestResult(object):
+    """The get manifest result.
 
-    :ivar manifest: The OCI manifest that was downloaded.
-    :vartype manifest: ~azure.containerregistry.models.OCIManifest
-    :ivar data: The manifest stream that was downloaded.
-    :vartype data: IO
+    :ivar dict manifest: The manifest JSON.
+    :ivar str media_type: The manifest's media type.
     :ivar str digest: The manifest's digest, calculated by the registry.
     """
 
     def __init__(self, **kwargs):
         self.manifest = kwargs.get("manifest")
-        self.data = kwargs.get("data")
+        self.media_type = kwargs.get("media_type")
         self.digest = kwargs.get("digest")
```

## Comparing `azure-containerregistry-1.1.0b3/azure/containerregistry/_exchange_client.py` & `azure-containerregistry-1.1.0b4/azure/containerregistry/_exchange_client.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b3/azure/containerregistry/_base_client.py` & `azure-containerregistry-1.1.0b4/azure/containerregistry/_base_client.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b3/azure/containerregistry/_download_stream.py` & `azure-containerregistry-1.1.0b4/azure/containerregistry/_download_stream.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b3/azure/containerregistry/_authentication_policy.py` & `azure-containerregistry-1.1.0b4/azure/containerregistry/_authentication_policy.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b3/azure/containerregistry/aio/__init__.py` & `azure-containerregistry-1.1.0b4/azure/containerregistry/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b3/azure/containerregistry/aio/_async_exchange_client.py` & `azure-containerregistry-1.1.0b4/azure/containerregistry/aio/_async_exchange_client.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b3/azure/containerregistry/aio/_async_container_registry_client.py` & `azure-containerregistry-1.1.0b4/azure/containerregistry/aio/_async_container_registry_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 # ------------------------------------
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 # ------------------------------------
 # pylint: disable=too-many-lines
 import functools
 import hashlib
+import json
 from io import BytesIO
-from typing import Any, Dict, IO, Optional, overload, Union, cast, Tuple
+from typing import Any, Dict, IO, Optional, overload, Union, cast, Tuple, MutableMapping
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.credentials_async import AsyncTokenCredential
 from azure.core.exceptions import (
     ClientAuthenticationError,
     ResourceExistsError,
     ResourceNotFoundError,
@@ -20,24 +21,34 @@
 )
 from azure.core.pipeline import PipelineResponse
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.tracing.decorator_async import distributed_trace_async
 
 from ._async_base_client import ContainerRegistryBaseClient
 from ._async_download_stream import AsyncDownloadBlobStream
-from .._container_registry_client import _return_response_headers, _return_response_and_headers
+from .._container_registry_client import (
+    _return_response_headers,
+    _return_response_and_headers,
+    _return_response,
+)
 from .._generated.models import AcrErrors
 from .._helpers import (
+    _compute_digest,
     _is_tag,
     _parse_next_link,
+    _validate_digest,
     SUPPORTED_API_VERSIONS,
-    AZURE_RESOURCE_MANAGER_PUBLIC_CLOUD,
+    OCI_IMAGE_MANIFEST,
+    SUPPORTED_MANIFEST_MEDIA_TYPES,
+    DEFAULT_AUDIENCE,
     DEFAULT_CHUNK_SIZE,
 )
-from .._models import RepositoryProperties, ArtifactManifestProperties, ArtifactTagProperties
+from .._models import RepositoryProperties, ArtifactManifestProperties, ArtifactTagProperties, GetManifestResult
+
+JSON = MutableMapping[str, Any]
 
 
 class _UnclosableBytesIO(BytesIO):
     def close(self):
         pass
 
     def manual_close(self):
@@ -47,28 +58,28 @@
 class ContainerRegistryClient(ContainerRegistryBaseClient):
     def __init__(
         self,
         endpoint: str,
         credential: Optional[AsyncTokenCredential] = None,
         *,
         api_version: Optional[str] = None,
-        audience: str = AZURE_RESOURCE_MANAGER_PUBLIC_CLOUD,
+        audience: str = DEFAULT_AUDIENCE,
         **kwargs
     ) -> None:
         """Create a ContainerRegistryClient from an ACR endpoint and a credential.
 
         :param str endpoint: An ACR endpoint.
         :param credential: The credential with which to authenticate. This should be None in anonymous access.
         :type credential: ~azure.core.credentials_async.AsyncTokenCredential or None
         :keyword api_version: API Version. The default value is "2021-07-01". Note that overriding this default value
             may result in unsupported behavior.
         :paramtype api_version: str
         :keyword audience: URL to use for credential authentication with AAD. Its value could be
             "https://management.azure.com", "https://management.chinacloudapi.cn" or
-            "https://management.usgovcloudapi.net". The default value is "https://management.azure.com".
+            "https://management.usgovcloudapi.net". The default value is "https://containerregistry.azure.net".
         :paramtype audience: str
         :returns: None
         :rtype: None
         :raises ValueError: If the provided api_version keyword-only argument isn't supported.
 
         .. admonition:: Example:
 
@@ -857,14 +868,102 @@
         )
         return ArtifactTagProperties._from_generated(  # pylint: disable=protected-access
             tag_attributes.tag, # type: ignore
             repository=repository
         )
 
     @distributed_trace_async
+    async def set_manifest(
+        self,
+        repository: str,
+        manifest: Union[JSON, IO[bytes]],
+        *,
+        tag: Optional[str] = None,
+        media_type: str = OCI_IMAGE_MANIFEST,
+        **kwargs
+    ) -> str:
+        """Set a manifest for an artifact.
+
+        :param str repository: Name of the repository
+        :param manifest: The manifest to set. It can be a JSON formatted dict or seekable stream.
+        :type manifest: dict or IO
+        :keyword tag: Tag of the manifest.
+        :paramtype tag: str or None
+        :keyword media_type: The media type of the manifest. If not specified, this value will be set to
+            a default value of "application/vnd.oci.image.manifest.v1+json". Note: the current known media types are:
+            "application/vnd.oci.image.manifest.v1+json", and "application/vnd.docker.distribution.manifest.v2+json".
+        :paramtype media_type: str
+        :returns: The digest of the set manifest, calculated by the registry.
+        :rtype: str
+        :raises ValueError: If the parameter repository or manifest is None,
+            or the digest in the response does not match the digest of the set manifest.
+        """
+        try:
+            if isinstance(manifest, MutableMapping):
+                data = _UnclosableBytesIO(json.dumps(manifest).encode())
+            else:
+                data = _UnclosableBytesIO(manifest.read())
+            tag_or_digest = tag
+            if tag_or_digest is None:
+                tag_or_digest = _compute_digest(data)
+
+            response_headers = await self._client.container_registry.create_manifest(
+                name=repository,
+                reference=tag_or_digest,
+                payload=data,
+                content_type=media_type,
+                cls=_return_response_headers,
+                **kwargs
+            )
+            digest = response_headers['Docker-Content-Digest']
+            if not _validate_digest(data, digest):
+                raise ValueError("The server-computed digest does not match the client-computed digest.")
+        except Exception as e:
+            if repository is None or manifest is None:
+                raise ValueError("The parameter repository and manifest cannot be None.") from e
+            raise
+        return digest
+
+    @distributed_trace_async
+    async def get_manifest(self, repository: str, tag_or_digest: str, **kwargs) -> GetManifestResult:
+        """Get the manifest for an artifact.
+
+        :param str repository: Name of the repository.
+        :param str tag_or_digest: The tag or digest of the manifest to get.
+            When digest is provided, will use this digest to compare with the one calculated by the response payload.
+            When tag is provided, will use the digest in response headers to compare.
+        :returns: GetManifestResult
+        :rtype: ~azure.containerregistry.GetManifestResult
+        :raises ValueError: If the requested digest does not match the digest of the received manifest.
+        """
+        response = cast(
+            PipelineResponse,
+            await self._client.container_registry.get_manifest(
+                name=repository,
+                reference=tag_or_digest,
+                accept=SUPPORTED_MANIFEST_MEDIA_TYPES,
+                cls=_return_response,
+                **kwargs
+            )
+        )
+        media_type = response.http_response.headers['Content-Type']
+        manifest_bytes = await response.http_response.read()
+        manifest_json = response.http_response.json()
+        if tag_or_digest.startswith("sha256:"):
+            digest = tag_or_digest
+            if not _validate_digest(manifest_bytes, digest):
+                raise ValueError("The requested digest does not match the digest of the received manifest.")
+        else:
+            digest = response.http_response.headers['Docker-Content-Digest']
+            if not _validate_digest(manifest_bytes, digest):
+                raise ValueError("The server-computed digest does not match the client-computed digest.")
+
+        return GetManifestResult(digest=digest, manifest=manifest_json, media_type=media_type)
+
+    @distributed_trace_async
     async def upload_blob(self, repository: str, data: IO[bytes], **kwargs) -> Tuple[str, int]:
         """Upload an artifact blob.
 
         :param str repository: Name of the repository.
         :param data: The blob to upload. Note: This must be a seekable stream.
         :type data: IO
         :returns: The digest and size in bytes of the uploaded blob.
@@ -894,33 +993,32 @@
             if repository is None or data is None:
                 raise ValueError("The parameter repository and data cannot be None.") from e
             raise
         return complete_upload_response_headers['Docker-Content-Digest'], blob_size
 
     async def _upload_blob_chunk(self, location: str, data: IO[bytes], **kwargs) -> Tuple[str, str, int]:
         hasher = hashlib.sha256()
-        blob_size = 0
         buffer = data.read(DEFAULT_CHUNK_SIZE)
-
+        blob_size = len(buffer)
         while len(buffer) > 0:
             try:
                 buffer_stream = _UnclosableBytesIO(buffer)
                 response_headers = cast(
                     Dict[str, str],
                     await self._client.container_registry_blob.upload_chunk(
                         location,
                         buffer_stream,
                         cls=_return_response_headers,
                         **kwargs
                     )
                 )
-                blob_size += len(buffer)
-                hasher.update(buffer)
                 location = response_headers['Location']
+                hasher.update(buffer)
                 buffer = data.read(DEFAULT_CHUNK_SIZE)
+                blob_size += len(buffer)
             finally:
                 buffer_stream.manual_close()
 
         return f"sha256:{hasher.hexdigest()}", location, blob_size
 
     @distributed_trace_async
     async def download_blob(self, repository: str, digest: str, **kwargs) -> AsyncDownloadBlobStream:
```

## Comparing `azure-containerregistry-1.1.0b3/azure/containerregistry/aio/_async_download_stream.py` & `azure-containerregistry-1.1.0b4/azure/containerregistry/aio/_async_download_stream.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b3/azure/containerregistry/aio/_async_authentication_policy.py` & `azure-containerregistry-1.1.0b4/azure/containerregistry/aio/_async_authentication_policy.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b3/azure/containerregistry/aio/_async_base_client.py` & `azure-containerregistry-1.1.0b4/azure/containerregistry/aio/_async_base_client.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b3/azure/containerregistry/aio/_async_anonymous_exchange_client.py` & `azure-containerregistry-1.1.0b4/azure/containerregistry/aio/_async_anonymous_exchange_client.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/__init__.py` & `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.4, generator: @autorest/python@6.4.6)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.4, generator: @autorest/python@6.4.9)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._client import ContainerRegistry
 
 try:
     from ._patch import __all__ as _patch_all
```

## Comparing `azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/_vendor.py` & `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/_vendor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.4, generator: @autorest/python@6.4.6)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.4, generator: @autorest/python@6.4.9)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import List, cast
 
 
 def _format_url_section(template, **kwargs):
```

## Comparing `azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/_patch.py` & `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/_configuration.py` & `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.4, generator: @autorest/python@6.4.6)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.4, generator: @autorest/python@6.4.9)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any, TYPE_CHECKING
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
```

## Comparing `azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/_serialization.py` & `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/_serialization.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/_client.py` & `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.4, generator: @autorest/python@6.4.6)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.4, generator: @autorest/python@6.4.9)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
 from typing import Any, TYPE_CHECKING
 
 from azure.core import PipelineClient
```

## Comparing `azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/models/_enums.py` & `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/models/_enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.4, generator: @autorest/python@6.4.6)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.4, generator: @autorest/python@6.4.9)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from enum import Enum
 from azure.core import CaseInsensitiveEnumMeta
```

## Comparing `azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/models/__init__.py` & `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.4, generator: @autorest/python@6.4.6)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.4, generator: @autorest/python@6.4.9)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._models import AcrAccessToken
 from ._models import AcrErrorInfo
 from ._models import AcrErrors
 from ._models import AcrRefreshToken
```

## Comparing `azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/models/_models.py` & `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/models/_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding=utf-8
 # pylint: disable=too-many-lines
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.4, generator: @autorest/python@6.4.6)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.4, generator: @autorest/python@6.4.9)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 import datetime
 import sys
 from typing import Any, Dict, List, Optional, TYPE_CHECKING, Union
 
@@ -1077,58 +1077,57 @@
         :paramtype annotations: ~container_registry.models.Annotations
         """
         super().__init__(schema_version=schema_version, **kwargs)
         self.manifests = manifests
         self.annotations = annotations
 
 
-class OCIManifest(_serialization.Model):
+class OCIManifest(Manifest):
     """Returns the requested OCI Manifest file.
 
+    :ivar schema_version: Schema version.
+    :vartype schema_version: int
     :ivar config: V2 image config descriptor.
     :vartype config: ~container_registry.models.Descriptor
     :ivar layers: List of V2 image layer information.
     :vartype layers: list[~container_registry.models.Descriptor]
     :ivar annotations: Additional information provided through arbitrary metadata.
     :vartype annotations: ~container_registry.models.Annotations
-    :ivar schema_version: Schema version.
-    :vartype schema_version: int
     """
 
     _attribute_map = {
+        "schema_version": {"key": "schemaVersion", "type": "int"},
         "config": {"key": "config", "type": "Descriptor"},
         "layers": {"key": "layers", "type": "[Descriptor]"},
         "annotations": {"key": "annotations", "type": "Annotations"},
-        "schema_version": {"key": "schemaVersion", "type": "int"},
     }
 
     def __init__(
         self,
         *,
+        schema_version: Optional[int] = None,
         config: Optional["_models.Descriptor"] = None,
         layers: Optional[List["_models.Descriptor"]] = None,
         annotations: Optional["_models.Annotations"] = None,
-        schema_version: Optional[int] = None,
         **kwargs: Any
     ) -> None:
         """
+        :keyword schema_version: Schema version.
+        :paramtype schema_version: int
         :keyword config: V2 image config descriptor.
         :paramtype config: ~container_registry.models.Descriptor
         :keyword layers: List of V2 image layer information.
         :paramtype layers: list[~container_registry.models.Descriptor]
         :keyword annotations: Additional information provided through arbitrary metadata.
         :paramtype annotations: ~container_registry.models.Annotations
-        :keyword schema_version: Schema version.
-        :paramtype schema_version: int
         """
-        super().__init__(**kwargs)
+        super().__init__(schema_version=schema_version, **kwargs)
         self.config = config
         self.layers = layers
         self.annotations = annotations
-        self.schema_version = schema_version
 
 
 class Paths108HwamOauth2ExchangePostRequestbodyContentApplicationXWwwFormUrlencodedSchema(_serialization.Model):
     """Paths108HwamOauth2ExchangePostRequestbodyContentApplicationXWwwFormUrlencodedSchema.
 
     All required parameters must be populated in order to send to Azure.
```

## Comparing `azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/models/_patch.py` & `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/operations/__init__.py` & `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/operations/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.4, generator: @autorest/python@6.4.6)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.4, generator: @autorest/python@6.4.9)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._operations import ContainerRegistryOperations
 from ._operations import ContainerRegistryBlobOperations
 from ._operations import AuthenticationOperations
```

## Comparing `azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/operations/_patch.py` & `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/operations/_patch.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 # fmt: off
 
 
 
+
 def build_exchange_aad_access_token_for_acr_refresh_token_request(
     **kwargs  # type: Any
 ):
     # type: (...) -> HttpRequest
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
```

## Comparing `azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/operations/_operations.py` & `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/operations/_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # pylint: disable=too-many-lines
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.4, generator: @autorest/python@6.4.6)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.4, generator: @autorest/python@6.4.9)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
+from io import IOBase
 from typing import Any, Callable, Dict, IO, Iterable, Iterator, Optional, TypeVar, Union, overload
 import urllib.parse
 
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
@@ -29,49 +30,52 @@
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
-def build_container_registry_check_docker_v2_support_request(**kwargs: Any) -> HttpRequest:
+def build_container_registry_check_docker_v2_support_request(  # pylint: disable=name-too-long
+    **kwargs: Any,
+) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/v2/"
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
 
 
-def build_container_registry_get_manifest_request(name: str, reference: str, **kwargs: Any) -> HttpRequest:
+def build_container_registry_get_manifest_request(  # pylint: disable=name-too-long
+    name: str, reference: str, *, accept: Optional[str] = None, **kwargs: Any
+) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
-    accept = _headers.pop("Accept", "application/json")
-
     # Construct URL
     _url = "/v2/{name}/manifests/{reference}"
     path_format_arguments = {
         "name": _SERIALIZER.url("name", name, "str"),
         "reference": _SERIALIZER.url("reference", reference, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
     # Construct headers
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+    if accept is not None:
+        _headers["accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
 
 
-def build_container_registry_create_manifest_request(
+def build_container_registry_create_manifest_request(  # pylint: disable=name-too-long
     name: str, reference: str, *, content: IO, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
@@ -88,15 +92,17 @@
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="PUT", url=_url, headers=_headers, content=content, **kwargs)
 
 
-def build_container_registry_delete_manifest_request(name: str, reference: str, **kwargs: Any) -> HttpRequest:
+def build_container_registry_delete_manifest_request(  # pylint: disable=name-too-long
+    name: str, reference: str, **kwargs: Any
+) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/v2/{name}/manifests/{reference}"
     path_format_arguments = {
@@ -108,15 +114,15 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="DELETE", url=_url, headers=_headers, **kwargs)
 
 
-def build_container_registry_get_repositories_request(
+def build_container_registry_get_repositories_request(  # pylint: disable=name-too-long
     *, last: Optional[str] = None, n: Optional[int] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2021-07-01"))
     accept = _headers.pop("Accept", "application/json")
@@ -133,15 +139,17 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_container_registry_get_properties_request(name: str, **kwargs: Any) -> HttpRequest:
+def build_container_registry_get_properties_request(  # pylint: disable=name-too-long
+    name: str, **kwargs: Any
+) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2021-07-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
@@ -157,15 +165,17 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_container_registry_delete_repository_request(name: str, **kwargs: Any) -> HttpRequest:
+def build_container_registry_delete_repository_request(  # pylint: disable=name-too-long
+    name: str, **kwargs: Any
+) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2021-07-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
@@ -181,15 +191,17 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="DELETE", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_container_registry_update_properties_request(name: str, **kwargs: Any) -> HttpRequest:
+def build_container_registry_update_properties_request(  # pylint: disable=name-too-long
+    name: str, **kwargs: Any
+) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2021-07-01"))
     accept = _headers.pop("Accept", "application/json")
 
@@ -208,22 +220,22 @@
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="PATCH", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_container_registry_get_tags_request(
+def build_container_registry_get_tags_request(  # pylint: disable=name-too-long
     name: str,
     *,
     last: Optional[str] = None,
     n: Optional[int] = None,
     orderby: Optional[str] = None,
     digest: Optional[str] = None,
-    **kwargs: Any
+    **kwargs: Any,
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2021-07-01"))
     accept = _headers.pop("Accept", "application/json")
 
@@ -248,15 +260,17 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_container_registry_get_tag_properties_request(name: str, reference: str, **kwargs: Any) -> HttpRequest:
+def build_container_registry_get_tag_properties_request(  # pylint: disable=name-too-long
+    name: str, reference: str, **kwargs: Any
+) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2021-07-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
@@ -273,15 +287,17 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_container_registry_update_tag_attributes_request(name: str, reference: str, **kwargs: Any) -> HttpRequest:
+def build_container_registry_update_tag_attributes_request(  # pylint: disable=name-too-long
+    name: str, reference: str, **kwargs: Any
+) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2021-07-01"))
     accept = _headers.pop("Accept", "application/json")
 
@@ -301,15 +317,17 @@
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="PATCH", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_container_registry_delete_tag_request(name: str, reference: str, **kwargs: Any) -> HttpRequest:
+def build_container_registry_delete_tag_request(  # pylint: disable=name-too-long
+    name: str, reference: str, **kwargs: Any
+) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2021-07-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
@@ -326,15 +344,15 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="DELETE", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_container_registry_get_manifests_request(
+def build_container_registry_get_manifests_request(  # pylint: disable=name-too-long
     name: str, *, last: Optional[str] = None, n: Optional[int] = None, orderby: Optional[str] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2021-07-01"))
     accept = _headers.pop("Accept", "application/json")
@@ -358,15 +376,17 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_container_registry_get_manifest_properties_request(name: str, digest: str, **kwargs: Any) -> HttpRequest:
+def build_container_registry_get_manifest_properties_request(  # pylint: disable=name-too-long
+    name: str, digest: str, **kwargs: Any
+) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2021-07-01"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
@@ -383,15 +403,17 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_container_registry_update_manifest_properties_request(name: str, digest: str, **kwargs: Any) -> HttpRequest:
+def build_container_registry_update_manifest_properties_request(  # pylint: disable=name-too-long
+    name: str, digest: str, **kwargs: Any
+) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2021-07-01"))
     accept = _headers.pop("Accept", "application/json")
 
@@ -411,15 +433,17 @@
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="PATCH", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_container_registry_blob_get_blob_request(name: str, digest: str, **kwargs: Any) -> HttpRequest:
+def build_container_registry_blob_get_blob_request(  # pylint: disable=name-too-long
+    name: str, digest: str, **kwargs: Any
+) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     accept = _headers.pop("Accept", "application/octet-stream")
 
     # Construct URL
     _url = "/v2/{name}/blobs/{digest}"
     path_format_arguments = {
@@ -431,15 +455,17 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
 
 
-def build_container_registry_blob_check_blob_exists_request(name: str, digest: str, **kwargs: Any) -> HttpRequest:
+def build_container_registry_blob_check_blob_exists_request(  # pylint: disable=name-too-long
+    name: str, digest: str, **kwargs: Any
+) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/v2/{name}/blobs/{digest}"
     path_format_arguments = {
@@ -451,35 +477,34 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="HEAD", url=_url, headers=_headers, **kwargs)
 
 
-def build_container_registry_blob_delete_blob_request(name: str, digest: str, **kwargs: Any) -> HttpRequest:
+def build_container_registry_blob_delete_blob_request(  # pylint: disable=name-too-long
+    name: str, digest: str, **kwargs: Any
+) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     accept = _headers.pop("Accept", "application/octet-stream")
 
     # Construct URL
     _url = "/v2/{name}/blobs/{digest}"
     path_format_arguments = {
         "name": _SERIALIZER.url("name", name, "str"),
         "digest": _SERIALIZER.url("digest", digest, "str"),
     }
 
     _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
 
-    # Construct headers
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="DELETE", url=_url, headers=_headers, **kwargs)
+    return HttpRequest(method="DELETE", url=_url, **kwargs)
 
 
-def build_container_registry_blob_mount_blob_request(
+def build_container_registry_blob_mount_blob_request(  # pylint: disable=name-too-long
     name: str, *, from_parameter: str, mount: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     accept = _headers.pop("Accept", "application/json")
 
@@ -497,15 +522,17 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="POST", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_container_registry_blob_get_upload_status_request(next_link: str, **kwargs: Any) -> HttpRequest:
+def build_container_registry_blob_get_upload_status_request(  # pylint: disable=name-too-long
+    next_link: str, **kwargs: Any
+) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/{nextBlobUuidLink}"
     path_format_arguments = {
@@ -516,15 +543,17 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
 
 
-def build_container_registry_blob_upload_chunk_request(next_link: str, *, content: IO, **kwargs: Any) -> HttpRequest:
+def build_container_registry_blob_upload_chunk_request(  # pylint: disable=name-too-long
+    next_link: str, *, content: IO, **kwargs: Any
+) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/{nextBlobUuidLink}"
@@ -538,15 +567,15 @@
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="PATCH", url=_url, headers=_headers, content=content, **kwargs)
 
 
-def build_container_registry_blob_complete_upload_request(
+def build_container_registry_blob_complete_upload_request(  # pylint: disable=name-too-long
     next_link: str, *, digest: str, content: Optional[IO] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
@@ -566,15 +595,17 @@
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="PUT", url=_url, params=_params, headers=_headers, content=content, **kwargs)
 
 
-def build_container_registry_blob_cancel_upload_request(next_link: str, **kwargs: Any) -> HttpRequest:
+def build_container_registry_blob_cancel_upload_request(  # pylint: disable=name-too-long
+    next_link: str, **kwargs: Any
+) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/{nextBlobUuidLink}"
     path_format_arguments = {
@@ -585,15 +616,17 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="DELETE", url=_url, headers=_headers, **kwargs)
 
 
-def build_container_registry_blob_start_upload_request(name: str, **kwargs: Any) -> HttpRequest:
+def build_container_registry_blob_start_upload_request(  # pylint: disable=name-too-long
+    name: str, **kwargs: Any
+) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = "/v2/{name}/blobs/uploads/"
     path_format_arguments = {
@@ -604,15 +637,15 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
 
 
-def build_container_registry_blob_get_chunk_request(
+def build_container_registry_blob_get_chunk_request(  # pylint: disable=name-too-long
     name: str, digest: str, *, range_header: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     accept = _headers.pop("Accept", "application/octet-stream")
 
     # Construct URL
@@ -627,15 +660,15 @@
     # Construct headers
     _headers["Range"] = _SERIALIZER.header("range_header", range_header, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
 
 
-def build_container_registry_blob_check_chunk_exists_request(
+def build_container_registry_blob_check_chunk_exists_request(  # pylint: disable=name-too-long
     name: str, digest: str, *, range_header: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
@@ -715,68 +748,74 @@
             error = self._deserialize.failsafe_deserialize(_models.AcrErrors, pipeline_response)
             raise HttpResponseError(response=response, model=error)
 
         if cls:
             return cls(pipeline_response, None, {})
 
     @distributed_trace
-    def get_manifest(self, name: str, reference: str, **kwargs: Any) -> _models.ManifestWrapper:
+    def get_manifest(
+        self, name: str, reference: str, *, accept: Optional[str] = None, **kwargs: Any
+    ) -> Iterator[bytes]:
         """Get the manifest identified by ``name`` and ``reference`` where ``reference`` can be a tag or
         digest.
 
         :param name: Name of the image (including the namespace). Required.
         :type name: str
         :param reference: A tag or a digest, pointing to a specific image. Required.
         :type reference: str
-        :return: ManifestWrapper
-        :rtype: ~container_registry.models.ManifestWrapper
+        :keyword accept: Accept header string delimited by comma. For example,
+         application/vnd.docker.distribution.manifest.v2+json. Default value is None.
+        :paramtype accept: str
+        :return: Iterator of the response bytes
+        :rtype: Iterator[bytes]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
-        cls: ClsType[_models.ManifestWrapper] = kwargs.pop("cls", None)
+        cls: ClsType[Iterator[bytes]] = kwargs.pop("cls", None)
 
         request = build_container_registry_get_manifest_request(
             name=name,
             reference=reference,
+            accept=accept,
             headers=_headers,
             params=_params,
         )
         path_format_arguments = {
             "url": self._serialize.url("self._config.url", self._config.url, "str", skip_quote=True),
         }
         request.url = self._client.format_url(request.url, **path_format_arguments)
 
-        _stream = False
+        _stream = True
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
             request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.AcrErrors, pipeline_response)
             raise HttpResponseError(response=response, model=error)
 
-        deserialized = self._deserialize("ManifestWrapper", pipeline_response)
+        deserialized = response.iter_bytes()
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
+        return deserialized  # type: ignore
 
     @distributed_trace
     def create_manifest(self, name: str, reference: str, payload: IO, **kwargs: Any) -> Any:
         """Put the manifest identified by ``name`` and ``reference`` where ``reference`` can be a tag or
         digest.
 
         :param name: Name of the image (including the namespace). Required.
@@ -1093,15 +1132,15 @@
     @overload
     def update_properties(
         self,
         name: str,
         value: Optional[_models.RepositoryWriteableProperties] = None,
         *,
         content_type: str = "application/json",
-        **kwargs: Any
+        **kwargs: Any,
     ) -> _models.ContainerRepositoryProperties:
         """Update the attribute identified by ``name`` where ``reference`` is the name of the repository.
 
         :param name: Name of the image (including the namespace). Required.
         :type name: str
         :param value: Repository attribute value. Default value is None.
         :type value: ~container_registry.models.RepositoryWriteableProperties
@@ -1162,15 +1201,15 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ContainerRepositoryProperties] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(value, (IO, bytes)):
+        if isinstance(value, (IOBase, bytes)):
             _content = value
         else:
             if value is not None:
                 _json = self._serialize.body(value, "RepositoryWriteableProperties")
             else:
                 _json = None
 
@@ -1212,15 +1251,15 @@
         self,
         name: str,
         *,
         last: Optional[str] = None,
         n: Optional[int] = None,
         orderby: Optional[str] = None,
         digest: Optional[str] = None,
-        **kwargs: Any
+        **kwargs: Any,
     ) -> Iterable["_models.TagAttributesBase"]:
         """List tags of a repository.
 
         :param name: Name of the image (including the namespace). Required.
         :type name: str
         :keyword last: Query parameter for the last item in previous query. Result set will include
          values lexically after last. Default value is None.
@@ -1373,15 +1412,15 @@
     def update_tag_attributes(
         self,
         name: str,
         reference: str,
         value: Optional[_models.TagWriteableProperties] = None,
         *,
         content_type: str = "application/json",
-        **kwargs: Any
+        **kwargs: Any,
     ) -> _models.ArtifactTagProperties:
         """Update tag attributes.
 
         :param name: Name of the image (including the namespace). Required.
         :type name: str
         :param reference: Tag name. Required.
         :type reference: str
@@ -1399,15 +1438,15 @@
     def update_tag_attributes(
         self,
         name: str,
         reference: str,
         value: Optional[IO] = None,
         *,
         content_type: str = "application/json",
-        **kwargs: Any
+        **kwargs: Any,
     ) -> _models.ArtifactTagProperties:
         """Update tag attributes.
 
         :param name: Name of the image (including the namespace). Required.
         :type name: str
         :param reference: Tag name. Required.
         :type reference: str
@@ -1423,15 +1462,15 @@
 
     @distributed_trace
     def update_tag_attributes(
         self,
         name: str,
         reference: str,
         value: Optional[Union[_models.TagWriteableProperties, IO]] = None,
-        **kwargs: Any
+        **kwargs: Any,
     ) -> _models.ArtifactTagProperties:
         """Update tag attributes.
 
         :param name: Name of the image (including the namespace). Required.
         :type name: str
         :param reference: Tag name. Required.
         :type reference: str
@@ -1458,15 +1497,15 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ArtifactTagProperties] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(value, (IO, bytes)):
+        if isinstance(value, (IOBase, bytes)):
             _content = value
         else:
             if value is not None:
                 _json = self._serialize.body(value, "TagWriteableProperties")
             else:
                 _json = None
 
@@ -1562,15 +1601,15 @@
     def get_manifests(
         self,
         name: str,
         *,
         last: Optional[str] = None,
         n: Optional[int] = None,
         orderby: Optional[str] = None,
-        **kwargs: Any
+        **kwargs: Any,
     ) -> Iterable["_models.ManifestAttributesBase"]:
         """List manifests of a repository.
 
         :param name: Name of the image (including the namespace). Required.
         :type name: str
         :keyword last: Query parameter for the last item in previous query. Result set will include
          values lexically after last. Default value is None.
@@ -1720,15 +1759,15 @@
     def update_manifest_properties(
         self,
         name: str,
         digest: str,
         value: Optional[_models.ManifestWriteableProperties] = None,
         *,
         content_type: str = "application/json",
-        **kwargs: Any
+        **kwargs: Any,
     ) -> _models.ArtifactManifestProperties:
         """Update properties of a manifest.
 
         :param name: Name of the image (including the namespace). Required.
         :type name: str
         :param digest: Digest of a BLOB. Required.
         :type digest: str
@@ -1746,15 +1785,15 @@
     def update_manifest_properties(
         self,
         name: str,
         digest: str,
         value: Optional[IO] = None,
         *,
         content_type: str = "application/json",
-        **kwargs: Any
+        **kwargs: Any,
     ) -> _models.ArtifactManifestProperties:
         """Update properties of a manifest.
 
         :param name: Name of the image (including the namespace). Required.
         :type name: str
         :param digest: Digest of a BLOB. Required.
         :type digest: str
@@ -1770,15 +1809,15 @@
 
     @distributed_trace
     def update_manifest_properties(
         self,
         name: str,
         digest: str,
         value: Optional[Union[_models.ManifestWriteableProperties, IO]] = None,
-        **kwargs: Any
+        **kwargs: Any,
     ) -> _models.ArtifactManifestProperties:
         """Update properties of a manifest.
 
         :param name: Name of the image (including the namespace). Required.
         :type name: str
         :param digest: Digest of a BLOB. Required.
         :type digest: str
@@ -1805,15 +1844,15 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ArtifactManifestProperties] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(value, (IO, bytes)):
+        if isinstance(value, (IOBase, bytes)):
             _content = value
         else:
             if value is not None:
                 _json = self._serialize.body(value, "ManifestWriteableProperties")
             else:
                 _json = None
 
@@ -1996,50 +2035,52 @@
         if response.status_code == 307:
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)
 
     @distributed_trace
-    def delete_blob(self, name: str, digest: str, **kwargs: Any) -> Iterator[bytes]:
+    def delete_blob(  # pylint: disable=inconsistent-return-statements
+        self, name: str, digest: str, **kwargs: Any
+    ) -> None:
         """Removes an already uploaded blob.
 
         :param name: Name of the image (including the namespace). Required.
         :type name: str
         :param digest: Digest of a BLOB. Required.
         :type digest: str
-        :return: Iterator of the response bytes
-        :rtype: Iterator[bytes]
+        :return: None
+        :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
-        cls: ClsType[Iterator[bytes]] = kwargs.pop("cls", None)
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_container_registry_blob_delete_blob_request(
             name=name,
             digest=digest,
             headers=_headers,
             params=_params,
         )
         path_format_arguments = {
             "url": self._serialize.url("self._config.url", self._config.url, "str", skip_quote=True),
         }
         request.url = self._client.format_url(request.url, **path_format_arguments)
 
-        _stream = True
+        _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
             request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [202]:
@@ -2047,20 +2088,16 @@
             raise HttpResponseError(response=response)
 
         response_headers = {}
         response_headers["Docker-Content-Digest"] = self._deserialize(
             "str", response.headers.get("Docker-Content-Digest")
         )
 
-        deserialized = response.iter_bytes()
-
         if cls:
-            return cls(pipeline_response, deserialized, response_headers)  # type: ignore
-
-        return deserialized  # type: ignore
+            return cls(pipeline_response, None, response_headers)
 
     @distributed_trace
     def mount_blob(  # pylint: disable=inconsistent-return-statements
         self, name: str, *, from_parameter: str, mount: str, **kwargs: Any
     ) -> None:
         """Mount a blob identified by the ``mount`` parameter from another repository.
```

## Comparing `azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/aio/__init__.py` & `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.4, generator: @autorest/python@6.4.6)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.4, generator: @autorest/python@6.4.9)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._client import ContainerRegistry
 
 try:
     from ._patch import __all__ as _patch_all
```

## Comparing `azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/aio/_vendor.py` & `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/_vendor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.4, generator: @autorest/python@6.4.6)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.4, generator: @autorest/python@6.4.9)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 
 def raise_if_not_implemented(cls, abstract_methods):
     not_implemented = [f for f in abstract_methods if not callable(getattr(cls, f, None))]
     if not_implemented:
```

## Comparing `azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/aio/_patch.py` & `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/aio/_configuration.py` & `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.4, generator: @autorest/python@6.4.6)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.4, generator: @autorest/python@6.4.9)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any, TYPE_CHECKING
 
 from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
```

## Comparing `azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/aio/_client.py` & `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.4, generator: @autorest/python@6.4.6)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.4, generator: @autorest/python@6.4.9)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
 from typing import Any, Awaitable, TYPE_CHECKING
 
 from azure.core import AsyncPipelineClient
```

## Comparing `azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/aio/operations/__init__.py` & `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/operations/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.4, generator: @autorest/python@6.4.6)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.4, generator: @autorest/python@6.4.9)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._operations import ContainerRegistryOperations
 from ._operations import ContainerRegistryBlobOperations
 from ._operations import AuthenticationOperations
```

## Comparing `azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/aio/operations/_patch.py` & `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b3/azure/containerregistry/_generated/aio/operations/_operations.py` & `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/operations/_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # pylint: disable=too-many-lines
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.4, generator: @autorest/python@6.4.6)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.4, generator: @autorest/python@6.4.9)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
+from io import IOBase
 from typing import Any, AsyncIterable, AsyncIterator, Callable, Dict, IO, Optional, TypeVar, Union, overload
 import urllib.parse
 
 from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
@@ -119,68 +120,74 @@
             error = self._deserialize.failsafe_deserialize(_models.AcrErrors, pipeline_response)
             raise HttpResponseError(response=response, model=error)
 
         if cls:
             return cls(pipeline_response, None, {})
 
     @distributed_trace_async
-    async def get_manifest(self, name: str, reference: str, **kwargs: Any) -> _models.ManifestWrapper:
+    async def get_manifest(
+        self, name: str, reference: str, *, accept: Optional[str] = None, **kwargs: Any
+    ) -> AsyncIterator[bytes]:
         """Get the manifest identified by ``name`` and ``reference`` where ``reference`` can be a tag or
         digest.
 
         :param name: Name of the image (including the namespace). Required.
         :type name: str
         :param reference: A tag or a digest, pointing to a specific image. Required.
         :type reference: str
-        :return: ManifestWrapper
-        :rtype: ~container_registry.models.ManifestWrapper
+        :keyword accept: Accept header string delimited by comma. For example,
+         application/vnd.docker.distribution.manifest.v2+json. Default value is None.
+        :paramtype accept: str
+        :return: Async iterator of the response bytes
+        :rtype: AsyncIterator[bytes]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
-        cls: ClsType[_models.ManifestWrapper] = kwargs.pop("cls", None)
+        cls: ClsType[AsyncIterator[bytes]] = kwargs.pop("cls", None)
 
         request = build_container_registry_get_manifest_request(
             name=name,
             reference=reference,
+            accept=accept,
             headers=_headers,
             params=_params,
         )
         path_format_arguments = {
             "url": self._serialize.url("self._config.url", self._config.url, "str", skip_quote=True),
         }
         request.url = self._client.format_url(request.url, **path_format_arguments)
 
-        _stream = False
+        _stream = True
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
             request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.AcrErrors, pipeline_response)
             raise HttpResponseError(response=response, model=error)
 
-        deserialized = self._deserialize("ManifestWrapper", pipeline_response)
+        deserialized = response.iter_bytes()
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
+        return deserialized  # type: ignore
 
     @distributed_trace_async
     async def create_manifest(self, name: str, reference: str, payload: IO, **kwargs: Any) -> Any:
         """Put the manifest identified by ``name`` and ``reference`` where ``reference`` can be a tag or
         digest.
 
         :param name: Name of the image (including the namespace). Required.
@@ -570,15 +577,15 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ContainerRepositoryProperties] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(value, (IO, bytes)):
+        if isinstance(value, (IOBase, bytes)):
             _content = value
         else:
             if value is not None:
                 _json = self._serialize.body(value, "RepositoryWriteableProperties")
             else:
                 _json = None
 
@@ -866,15 +873,15 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ArtifactTagProperties] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(value, (IO, bytes)):
+        if isinstance(value, (IOBase, bytes)):
             _content = value
         else:
             if value is not None:
                 _json = self._serialize.body(value, "TagWriteableProperties")
             else:
                 _json = None
 
@@ -1216,15 +1223,15 @@
 
         content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
         cls: ClsType[_models.ArtifactManifestProperties] = kwargs.pop("cls", None)
 
         content_type = content_type or "application/json"
         _json = None
         _content = None
-        if isinstance(value, (IO, bytes)):
+        if isinstance(value, (IOBase, bytes)):
             _content = value
         else:
             if value is not None:
                 _json = self._serialize.body(value, "ManifestWriteableProperties")
             else:
                 _json = None
 
@@ -1407,50 +1414,52 @@
         if response.status_code == 307:
             response_headers["Location"] = self._deserialize("str", response.headers.get("Location"))
 
         if cls:
             return cls(pipeline_response, None, response_headers)
 
     @distributed_trace_async
-    async def delete_blob(self, name: str, digest: str, **kwargs: Any) -> AsyncIterator[bytes]:
+    async def delete_blob(  # pylint: disable=inconsistent-return-statements
+        self, name: str, digest: str, **kwargs: Any
+    ) -> None:
         """Removes an already uploaded blob.
 
         :param name: Name of the image (including the namespace). Required.
         :type name: str
         :param digest: Digest of a BLOB. Required.
         :type digest: str
-        :return: Async iterator of the response bytes
-        :rtype: AsyncIterator[bytes]
+        :return: None
+        :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
-        cls: ClsType[AsyncIterator[bytes]] = kwargs.pop("cls", None)
+        cls: ClsType[None] = kwargs.pop("cls", None)
 
         request = build_container_registry_blob_delete_blob_request(
             name=name,
             digest=digest,
             headers=_headers,
             params=_params,
         )
         path_format_arguments = {
             "url": self._serialize.url("self._config.url", self._config.url, "str", skip_quote=True),
         }
         request.url = self._client.format_url(request.url, **path_format_arguments)
 
-        _stream = True
+        _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
             request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [202]:
@@ -1458,20 +1467,16 @@
             raise HttpResponseError(response=response)
 
         response_headers = {}
         response_headers["Docker-Content-Digest"] = self._deserialize(
             "str", response.headers.get("Docker-Content-Digest")
         )
 
-        deserialized = response.iter_bytes()
-
         if cls:
-            return cls(pipeline_response, deserialized, response_headers)  # type: ignore
-
-        return deserialized  # type: ignore
+            return cls(pipeline_response, None, response_headers)
 
     @distributed_trace_async
     async def mount_blob(  # pylint: disable=inconsistent-return-statements
         self, name: str, *, from_parameter: str, mount: str, **kwargs: Any
     ) -> None:
         """Mount a blob identified by the ``mount`` parameter from another repository.
```

## Comparing `azure-containerregistry-1.1.0b3/tests/asynctestcase.py` & `azure-containerregistry-1.1.0b4/tests/perfstress_tests/list_artifacts.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,31 @@
-# coding=utf-8
 # ------------------------------------
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 # ------------------------------------
-import logging
-import os
+from azure_devtools.perfstress_tests import PerfStressTest
+from azure.containerregistry import ContainerRegistryClient
+from azure.containerregistry.aio import ContainerRegistryClient as AsyncContainerRegistryClient
 
-from azure.containerregistry.aio import ContainerRegistryClient
 
-from azure.core.credentials import AccessToken
-from azure.identity.aio import DefaultAzureCredential, ClientSecretCredential
-from azure.identity import AzureAuthorityHosts
-
-from testcase import ContainerRegistryTestClass, get_audience, get_authority
-
-logger = logging.getLogger()
-
-
-class AsyncFakeTokenCredential(object):
-    """Protocol for classes able to provide OAuth tokens.
-    :param str scopes: Lets you specify the type of access needed.
-    """
-
-    def __init__(self):
-        self.token = AccessToken("YOU SHALL NOT PASS", 0)
-
-    async def get_token(self, *args):
-        return self.token
-
-
-class AsyncContainerRegistryTestClass(ContainerRegistryTestClass):
-    def get_credential(self, authority=None, **kwargs):
-        if self.is_live:
-            if authority != AzureAuthorityHosts.AZURE_PUBLIC_CLOUD:
-                return ClientSecretCredential(
-                    tenant_id=os.environ["CONTAINERREGISTRY_TENANT_ID"],
-                    client_id=os.environ["CONTAINERREGISTRY_CLIENT_ID"],
-                    client_secret=os.environ["CONTAINERREGISTRY_CLIENT_SECRET"],
-                    authority=authority
-                )
-            return DefaultAzureCredential(**kwargs)
-        return AsyncFakeTokenCredential()
-
-    def create_registry_client(self, endpoint, **kwargs):
-        authority = get_authority(endpoint)
-        audience = kwargs.pop("audience", None)
-        if not audience:
-            audience = get_audience(authority)
-        credential = self.get_credential(authority=authority)
-        return ContainerRegistryClient(endpoint=endpoint, credential=credential, audience=audience, **kwargs)
-
-    def create_anon_client(self, endpoint, **kwargs):
-        authority = get_authority(endpoint)
-        audience = get_audience(authority)
-        return ContainerRegistryClient(endpoint=endpoint, credential=None, audience=audience, **kwargs)
+class ListArtifactsTest(PerfStressTest):
+
+    def __init__(self, arguments):
+        super().__init__(arguments)
+
+        endpoint = self.get_from_env("CONTAINERREGISTRY_ANONREGISTRY_ENDPOINT")
+        audience = "https://management.azure.com"
+        self.anon_client = ContainerRegistryClient(endpoint=endpoint, credential=None, audience=audience)
+        self.async_anon_client = AsyncContainerRegistryClient(endpoint=endpoint, credential=None, audience=audience)       
+        self.repository = "node"
+
+    async def close(self):
+        await self.async_anon_client.close()
+        await super().close()
+
+    def run_sync(self):
+        for _ in self.anon_client.list_manifest_properties(self.repository):
+            pass
+
+    async def run_async(self):
+        async for _ in self.async_anon_client.list_manifest_properties(self.repository):
+            pass
```

## Comparing `azure-containerregistry-1.1.0b3/tests/test_anon_access.py` & `azure-containerregistry-1.1.0b4/tests/test_anon_access.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b3/tests/conftest.py` & `azure-containerregistry-1.1.0b4/tests/conftest.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b3/tests/testcase.py` & `azure-containerregistry-1.1.0b4/tests/testcase.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 # Licensed under the MIT License.
 # ------------------------------------
 import logging
 import os
 import pytest
 
 from azure.containerregistry import ContainerRegistryClient
-from azure.containerregistry._helpers import _is_tag, AZURE_RESOURCE_MANAGER_PUBLIC_CLOUD
-from azure.containerregistry._generated.models import Annotations, Descriptor, OCIManifest
+from azure.containerregistry._helpers import _is_tag
 
 from azure.mgmt.containerregistry import ContainerRegistryManagementClient
 from azure.mgmt.containerregistry.models import ImportImageParameters, ImportSource, ImportMode
 from azure.identity import DefaultAzureCredential, AzureAuthorityHosts, ClientSecretCredential
 
 from devtools_testutils import AzureRecordedTestCase, is_live, FakeTokenCredential
 
@@ -64,54 +63,37 @@
 
     def assert_all_properties(self, properties, value):
         assert properties.can_delete == value
         assert properties.can_read == value
         assert properties.can_write == value
         assert properties.can_list == value
 
-    def assert_manifest(self, manifest, expected):
-        assert manifest is not None
-        assert manifest.schema_version == expected.schema_version
-        assert manifest.config is not None
-        assert_manifest_config_or_layer_properties(manifest.config, expected.config)
-        assert manifest.layers is not None
-        assert len(manifest.layers) == len(expected.layers)
-        count = 0
-        for layer in manifest.layers:
-            assert_manifest_config_or_layer_properties(layer, expected.layers[count])
-            count += 1
-
     def create_fully_qualified_reference(self, registry, repository, digest):
         return f"{registry}/{repository}{':' if _is_tag(digest) else '@'}{digest.split(':')[-1]}"
 
     def is_public_endpoint(self, endpoint):
         return ".azurecr.io" in endpoint
     
-    def create_oci_manifest(self):
-        config1 = Descriptor(
-            media_type="application/vnd.acme.rocket.config",
-            digest="sha256:d25b42d3dbad5361ed2d909624d899e7254a822c9a632b582ebd3a44f9b0dbc8",
-            size=171
-        )
-        config2 = Descriptor(
-            media_type="application/vnd.oci.image.layer.v1.tar",
-            digest="sha256:654b93f61054e4ce90ed203bb8d556a6200d5f906cf3eca0620738d6dc18cbed",
-            size=28,
-            annotations=Annotations(name="artifact.txt")
-        )
-        return OCIManifest(config=config1, schema_version=2, layers=[config2])
-    
-    def upload_manifest_prerequisites(self, repo, client):
+    def upload_oci_manifest_prerequisites(self, repo, client):
         layer = "654b93f61054e4ce90ed203bb8d556a6200d5f906cf3eca0620738d6dc18cbed"
         config = "config.json"
         base_path = os.path.join(self.get_test_directory(), "data", "oci_artifact")
         # upload config
         client.upload_blob(repo, open(os.path.join(base_path, config), "rb"))
         # upload layers
         client.upload_blob(repo, open(os.path.join(base_path, layer), "rb"))
+    
+    def upload_docker_manifest_prerequisites(self, repo, client):
+        layer = "2db29710123e3e53a794f2694094b9b4338aa9ee5c40b930cb8063a1be392c54"
+        config = "config.json"
+        base_path = os.path.join(self.get_test_directory(), "data", "docker_artifact")
+        # upload config
+        client.upload_blob(repo, open(os.path.join(base_path, config), "rb"))
+        # upload layers
+        client.upload_blob(repo, open(os.path.join(base_path, layer), "rb"))
 
     def get_test_directory(self):
         return os.path.join(os.getcwd(), "tests")
 
 
 def get_authority(endpoint: str) -> str:
     if ".azurecr.io" in endpoint:
@@ -124,15 +106,15 @@
         logger.warning("US Gov Authority")
         return AzureAuthorityHosts.AZURE_GOVERNMENT
     raise ValueError(f"Endpoint ({endpoint}) could not be understood")
 
 def get_audience(authority: str) -> str:
     if authority == AzureAuthorityHosts.AZURE_PUBLIC_CLOUD:
         logger.warning("Public cloud auth audience")
-        return AZURE_RESOURCE_MANAGER_PUBLIC_CLOUD
+        return "https://management.azure.com"
     if authority == AzureAuthorityHosts.AZURE_CHINA:
         logger.warning("China cloud auth audience")
         return "https://management.chinacloudapi.cn"
     if authority == AzureAuthorityHosts.AZURE_GOVERNMENT:
         logger.warning("US Gov cloud auth audience")
         return "https://management.usgovcloudapi.net"
 
@@ -194,12 +176,7 @@
     ]
     for repo, tag in zip(repos, tags):
         try:
             import_image(authority, repo, tag)
             import_image(authority_anon, repo, tag, is_anonymous=True)
         except Exception as e:
             print(e)
-
-def assert_manifest_config_or_layer_properties(value, expected):
-    assert value.media_type == expected.media_type
-    assert value.digest == expected.digest
-    assert value.size == expected.size
```

## Comparing `azure-containerregistry-1.1.0b3/tests/test_container_registry_client.py` & `azure-containerregistry-1.1.0b4/tests/test_container_registry_client.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 # ------------------------------------
 import os
 import pytest
 import six
 import hashlib
+import json
 from datetime import datetime
 from io import BytesIO
 from azure.containerregistry import (
     RepositoryProperties,
     ArtifactManifestProperties,
     ArtifactManifestOrder,
     ArtifactTagProperties,
     ArtifactTagOrder,
     ContainerRegistryClient,
 )
-from azure.containerregistry._helpers import _serialize_manifest, DEFAULT_CHUNK_SIZE
-from azure.core.exceptions import ResourceNotFoundError, ClientAuthenticationError
+from azure.containerregistry._helpers import DOCKER_MANIFEST, OCI_IMAGE_MANIFEST, DEFAULT_CHUNK_SIZE
+from azure.core.exceptions import ResourceNotFoundError, ClientAuthenticationError, HttpResponseError
 from azure.core.paging import ItemPaged
 from azure.identity import AzureAuthorityHosts
 from testcase import ContainerRegistryTestClass, get_authority, get_audience
 from constants import HELLO_WORLD, ALPINE, BUSYBOX, DOES_NOT_EXIST
 from preparer import acr_preparer
 from devtools_testutils import recorded_by_proxy
 
@@ -446,110 +447,318 @@
             properties = client.get_repository_properties(ALPINE)
             
             with pytest.warns(DeprecationWarning):
                 last_udpated_on = properties.last_udpated_on
             last_updated_on = properties.last_updated_on
             assert last_udpated_on == last_updated_on
 
+    # Live only, as test proxy now cannot handle spaces correctly
+    # issue: https://github.com/Azure/azure-sdk-tools/issues/5968
+    @pytest.mark.live_test_only
     @acr_preparer()
     @recorded_by_proxy
-    def test_upload_oci_manifest(self, containerregistry_endpoint):
+    def test_set_oci_manifest_json(self, containerregistry_endpoint):
         repo = self.get_resource_name("repo")
-        manifest = self.create_oci_manifest()
+        path = os.path.join(self.get_test_directory(), "data", "oci_artifact", "manifest.json")
         with self.create_registry_client(containerregistry_endpoint) as client:
-            self.upload_manifest_prerequisites(repo, client)
+            self.upload_oci_manifest_prerequisites(repo, client)
 
-            # Act
-            digest = client.upload_manifest(repo, manifest)
+            with open(path, "rb") as manifest_stream:
+                manifest_json = json.loads(manifest_stream.read().decode())
+                with pytest.raises(HttpResponseError):
+                    client.set_manifest(repo, manifest_json, media_type=DOCKER_MANIFEST)
+                digest = client.set_manifest(repo, manifest_json)
 
-            # Assert
-            response = client.download_manifest(repo, digest)
-            assert response.data.tell() == 0
-            self.assert_manifest(response.manifest, manifest)
+            response = client.get_manifest(repo, digest)
+            assert response.media_type == OCI_IMAGE_MANIFEST
 
-            # Cleanup
+            client.delete_manifest(repo, digest)
             client.delete_repository(repo)
 
+    # Live only, as test proxy now cannot handle spaces correctly
+    # issue: https://github.com/Azure/azure-sdk-tools/issues/5968
+    @pytest.mark.live_test_only
     @acr_preparer()
     @recorded_by_proxy
-    def test_upload_oci_manifest_stream(self, containerregistry_endpoint):
+    def test_set_oci_manifest_json_with_tag(self, containerregistry_endpoint):
         repo = self.get_resource_name("repo")
-        manifest = self.create_oci_manifest()
-        manifest_stream = _serialize_manifest(manifest)
+        tag = "v1"
+        path = os.path.join(self.get_test_directory(), "data", "oci_artifact", "manifest.json")
         with self.create_registry_client(containerregistry_endpoint) as client:
-            self.upload_manifest_prerequisites(repo, client)
+            self.upload_oci_manifest_prerequisites(repo, client)
+            
+            with open(path, "rb") as manifest_stream:
+                manifest_json = json.loads(manifest_stream.read().decode())
+                with pytest.raises(HttpResponseError):
+                    client.set_manifest(repo, manifest_json, tag=tag, media_type=DOCKER_MANIFEST)
+                digest = client.set_manifest(repo, manifest_json, tag=tag)
+            
+            response = client.get_manifest(repo, tag)
+            assert response.media_type == OCI_IMAGE_MANIFEST
 
-            # Act
-            digest = client.upload_manifest(repo, manifest_stream)
+            tags = client.get_manifest_properties(repo, digest).tags
+            assert len(tags) == 1
+            assert tags[0] == tag
 
-            # Assert
-            response = client.download_manifest(repo, digest)
-            assert response.data.tell() == 0
-            self.assert_manifest(response.manifest, manifest)
+            client.delete_manifest(repo, digest)
+            client.delete_repository(repo)
+    
+    # Live only, as test proxy now cannot handle spaces correctly
+    # issue: https://github.com/Azure/azure-sdk-tools/issues/5968
+    @pytest.mark.live_test_only
+    @acr_preparer()
+    @recorded_by_proxy
+    def test_set_oci_manifest_stream(self, containerregistry_endpoint):
+        repo = self.get_resource_name("repo")
+        path = os.path.join(self.get_test_directory(), "data", "oci_artifact", "manifest.json")
+        with self.create_registry_client(containerregistry_endpoint) as client:
+            self.upload_oci_manifest_prerequisites(repo, client)
 
-            # Cleanup
+            with open(path, "rb") as manifest_stream:
+                with pytest.raises(HttpResponseError):
+                    client.set_manifest(repo, manifest_stream, media_type=DOCKER_MANIFEST)
+                manifest_stream.seek(0)
+                digest = client.set_manifest(repo, manifest_stream)
+
+            response = client.get_manifest(repo, digest)
+            assert response.media_type == OCI_IMAGE_MANIFEST
+
+            client.delete_manifest(repo, digest)
+            client.delete_repository(repo)
+
+    @acr_preparer()
+    @recorded_by_proxy
+    def test_set_oci_manifest_stream_without_spaces(self, containerregistry_endpoint):
+        repo = self.get_resource_name("repo")
+        # Reading data from a no space file to make this test pass in playback as test proxy cannot handle spaces correctly
+        # issue: https://github.com/Azure/azure-sdk-tools/issues/5968
+        path = os.path.join(self.get_test_directory(), "data", "oci_artifact", "manifest_without_spaces.json")
+        with self.create_registry_client(containerregistry_endpoint) as client:
+            self.upload_oci_manifest_prerequisites(repo, client)
+
+            with open(path, "rb") as manifest_stream:
+                with pytest.raises(HttpResponseError):
+                    client.set_manifest(repo, manifest_stream, media_type=DOCKER_MANIFEST)
+                manifest_stream.seek(0)
+                digest = client.set_manifest(repo, manifest_stream)
+
+            response = client.get_manifest(repo, digest)
+            assert response.media_type == OCI_IMAGE_MANIFEST
+
+            client.delete_manifest(repo, digest)
             client.delete_repository(repo)
 
+    # Live only, as test proxy now cannot handle spaces correctly
+    # issue: https://github.com/Azure/azure-sdk-tools/issues/5968
+    @pytest.mark.live_test_only
     @acr_preparer()
     @recorded_by_proxy
-    def test_upload_oci_manifest_with_tag(self, containerregistry_endpoint):
+    def test_set_oci_manifest_stream_with_tag(self, containerregistry_endpoint):
         repo = self.get_resource_name("repo")
         tag = "v1"
-        manifest = self.create_oci_manifest()
+        path = os.path.join(self.get_test_directory(), "data", "oci_artifact", "manifest.json")
         with self.create_registry_client(containerregistry_endpoint) as client:
-            self.upload_manifest_prerequisites(repo, client)
+            self.upload_oci_manifest_prerequisites(repo, client)
             
-            # Act
-            digest = client.upload_manifest(repo, manifest, tag=tag)
+            with open(path, "rb") as manifest_stream:
+                with pytest.raises(HttpResponseError):
+                    client.set_manifest(repo, manifest_stream, tag=tag, media_type=DOCKER_MANIFEST)
+                manifest_stream.seek(0)
+                digest = client.set_manifest(repo, manifest_stream, tag=tag)
             
-            # Assert
-            response = client.download_manifest(repo, digest)
-            assert response.data.tell() == 0
-            self.assert_manifest(response.manifest, manifest)
-
-            response = client.download_manifest(repo, tag)
-            assert response.digest == digest
-            assert response.data.tell() == 0
-            self.assert_manifest(response.manifest, manifest)
+            response = client.get_manifest(repo, tag)
+            assert response.media_type == OCI_IMAGE_MANIFEST
+            
+            tags = client.get_manifest_properties(repo, digest).tags
+            assert len(tags) == 1
+            assert tags[0] == tag
 
+            client.delete_manifest(repo, digest)
+            client.delete_repository(repo)
+    
+    @acr_preparer()
+    @recorded_by_proxy
+    def test_set_oci_manifest_stream_without_spaces_with_tag(self, containerregistry_endpoint):
+        repo = self.get_resource_name("repo")
+        tag = "v1"
+        # Reading data from a no space file to make this test pass in playback as test proxy cannot handle spaces correctly
+        # issue: https://github.com/Azure/azure-sdk-tools/issues/5968
+        path = os.path.join(self.get_test_directory(), "data", "oci_artifact", "manifest_without_spaces.json")
+        with self.create_registry_client(containerregistry_endpoint) as client:
+            self.upload_oci_manifest_prerequisites(repo, client)
+            
+            with open(path, "rb") as manifest_stream:
+                with pytest.raises(HttpResponseError):
+                    client.set_manifest(repo, manifest_stream, tag=tag, media_type=DOCKER_MANIFEST)
+                manifest_stream.seek(0)
+                digest = client.set_manifest(repo, manifest_stream, tag=tag)
+            
+            response = client.get_manifest(repo, tag)
+            assert response.media_type == OCI_IMAGE_MANIFEST
+            
             tags = client.get_manifest_properties(repo, digest).tags
             assert len(tags) == 1
             assert tags[0] == tag
 
-            # Cleanup
+            client.delete_manifest(repo, digest)
+            client.delete_repository(repo)
+    
+    # Live only, as test proxy now cannot handle spaces correctly
+    # issue: https://github.com/Azure/azure-sdk-tools/issues/5968
+    @pytest.mark.live_test_only
+    @acr_preparer()
+    @recorded_by_proxy
+    def test_set_docker_manifest_stream(self, containerregistry_endpoint):
+        repo = "library/hello-world"
+        path = os.path.join(self.get_test_directory(), "data", "docker_artifact", "manifest.json")
+        with self.create_registry_client(containerregistry_endpoint) as client:
+            self.upload_docker_manifest_prerequisites(repo, client)
+
+            with open(path, "rb") as manifest_stream:
+                with pytest.raises(HttpResponseError):
+                    # It fails as the default media type is oci image manifest media type
+                    client.set_manifest(repo, manifest_stream)
+                manifest_stream.seek(0)
+                digest = client.set_manifest(repo, manifest_stream, media_type=DOCKER_MANIFEST)
+
+            response = client.get_manifest(repo, digest)
+            assert response.media_type == DOCKER_MANIFEST
+
+            client.delete_manifest(repo, digest)
             client.delete_repository(repo)
+    
+    @acr_preparer()
+    @recorded_by_proxy
+    def test_set_docker_manifest_stream_without_spaces(self, containerregistry_endpoint):
+        repo = "library/hello-world"
+        # Reading data from a no space file to make this test pass in playback as test proxy cannot handle spaces correctly
+        # issue: https://github.com/Azure/azure-sdk-tools/issues/5968
+        path = os.path.join(self.get_test_directory(), "data", "docker_artifact", "manifest_without_spaces.json")
+        with self.create_registry_client(containerregistry_endpoint) as client:
+            self.upload_docker_manifest_prerequisites(repo, client)
+
+            with open(path, "rb") as manifest_stream:
+                with pytest.raises(HttpResponseError):
+                    # It fails as the default media type is oci image manifest media type
+                    client.set_manifest(repo, manifest_stream)
+                manifest_stream.seek(0)
+                digest = client.set_manifest(repo, manifest_stream, media_type=DOCKER_MANIFEST)
 
+            response = client.get_manifest(repo, digest)
+            assert response.media_type == DOCKER_MANIFEST
+
+            client.delete_manifest(repo, digest)
+            client.delete_repository(repo)
+    
+    # Live only, as test proxy now cannot handle spaces correctly
+    # issue: https://github.com/Azure/azure-sdk-tools/issues/5968
+    @pytest.mark.live_test_only
     @acr_preparer()
     @recorded_by_proxy
-    def test_upload_oci_manifest_stream_with_tag(self, containerregistry_endpoint):
-        repo = self.get_resource_name("repo")
+    def test_set_docker_manifest_stream_with_tag(self, containerregistry_endpoint):
+        repo = "library/hello-world"
         tag = "v1"
-        manifest = self.create_oci_manifest()
-        manifest_stream = _serialize_manifest(manifest)
+        path = os.path.join(self.get_test_directory(), "data", "docker_artifact", "manifest.json")
         with self.create_registry_client(containerregistry_endpoint) as client:
-            self.upload_manifest_prerequisites(repo, client)
+            self.upload_docker_manifest_prerequisites(repo, client)
+
+            with open(path, "rb") as manifest_stream:
+                with pytest.raises(HttpResponseError):
+                    # It fails as the default media type is oci image manifest media type
+                    client.set_manifest(repo, manifest_stream, tag=tag)
+                digest = client.set_manifest(repo, manifest_stream, tag=tag, media_type=DOCKER_MANIFEST)
             
-            # Act
-            digest = client.upload_manifest(repo, manifest_stream, tag=tag)
+            response = client.get_manifest(repo, tag)
+            assert response.media_type == DOCKER_MANIFEST
+
+            tags = client.get_manifest_properties(repo, digest).tags
+            assert len(tags) == 1
+            assert tags[0] == tag
             
-            # Assert
-            response = client.download_manifest(repo, digest)
-            assert response.data.tell() == 0
-            self.assert_manifest(response.manifest, manifest)
-
-            response = client.download_manifest(repo, tag)
-            assert response.digest == digest
-            assert response.data.tell() == 0
-            self.assert_manifest(response.manifest, manifest)
+            client.delete_manifest(repo, digest)
+            client.delete_repository(repo)
+    
+    @acr_preparer()
+    @recorded_by_proxy
+    def test_set_docker_manifest_stream_without_spaces_with_tag(self, containerregistry_endpoint):
+        repo = "library/hello-world"
+        tag = "v1"
+        # Reading data from a no space file to make this test pass in playback as test proxy cannot handle spaces correctly
+        # issue: https://github.com/Azure/azure-sdk-tools/issues/5968
+        path = os.path.join(self.get_test_directory(), "data", "docker_artifact", "manifest_without_spaces.json")
+        with self.create_registry_client(containerregistry_endpoint) as client:
+            self.upload_docker_manifest_prerequisites(repo, client)
+
+            with open(path, "rb") as manifest_stream:
+                with pytest.raises(HttpResponseError):
+                    # It fails as the default media type is oci image manifest media type
+                    client.set_manifest(repo, manifest_stream, tag=tag)
+                digest = client.set_manifest(repo, manifest_stream, tag=tag, media_type=DOCKER_MANIFEST)
+            
+            response = client.get_manifest(repo, tag)
+            assert response.media_type == DOCKER_MANIFEST
 
             tags = client.get_manifest_properties(repo, digest).tags
             assert len(tags) == 1
             assert tags[0] == tag
+            
+            client.delete_manifest(repo, digest)
+            client.delete_repository(repo)
+    
+    # Live only, as test proxy now cannot handle spaces correctly
+    # issue: https://github.com/Azure/azure-sdk-tools/issues/5968
+    @pytest.mark.live_test_only
+    @acr_preparer()
+    @recorded_by_proxy
+    def test_set_docker_manifest_json(self, containerregistry_endpoint):
+        repo = "library/hello-world"
+        path = os.path.join(self.get_test_directory(), "data", "docker_artifact", "manifest.json")
+        with self.create_registry_client(containerregistry_endpoint) as client:
+            self.upload_docker_manifest_prerequisites(repo, client)
+
+            with open(path, "rb") as manifest_stream:
+                manifest_json = json.loads(manifest_stream.read().decode())
+                with pytest.raises(HttpResponseError):
+                    # It fails as the default media type is oci image manifest media type
+                    client.set_manifest(repo, manifest_json)
+                digest = client.set_manifest(repo, manifest_json, media_type=DOCKER_MANIFEST)
+            
+            response = client.get_manifest(repo, digest)
+            assert response.media_type == DOCKER_MANIFEST
 
-            # Cleanup
+            client.delete_manifest(repo, digest)
+            client.delete_repository(repo)
+    
+    # Live only, as test proxy now cannot handle spaces correctly
+    # issue: https://github.com/Azure/azure-sdk-tools/issues/5968
+    @pytest.mark.live_test_only
+    @acr_preparer()
+    @recorded_by_proxy
+    def test_set_docker_manifest_json_with_tag(self, containerregistry_endpoint):
+        repo = "library/hello-world"
+        tag = "v1"
+        path = os.path.join(self.get_test_directory(), "data", "docker_artifact", "manifest.json")
+        with self.create_registry_client(containerregistry_endpoint) as client:
+            self.upload_docker_manifest_prerequisites(repo, client)
+
+            with open(path, "rb") as manifest_stream:
+                manifest_json = json.loads(manifest_stream.read().decode())
+                with pytest.raises(HttpResponseError):
+                    # It fails as the default media type is oci image manifest media type
+                    client.set_manifest(repo, manifest_json, tag=tag)
+                digest = client.set_manifest(repo, manifest_json, tag=tag, media_type=DOCKER_MANIFEST)
+            
+            response = client.get_manifest(repo, tag)
+            assert response.media_type == DOCKER_MANIFEST
+
+            tags = client.get_manifest_properties(repo, digest).tags
+            assert len(tags) == 1
+            assert tags[0] == tag
+            
+            client.delete_manifest(repo, digest)
             client.delete_repository(repo)
 
     @acr_preparer()
     @recorded_by_proxy
     def test_upload_blob(self, containerregistry_endpoint):
         repo = self.get_resource_name("repo")
         blob = "654b93f61054e4ce90ed203bb8d556a6200d5f906cf3eca0620738d6dc18cbed"
@@ -619,39 +828,35 @@
             client.delete_blob(repo, digest)
 
     @acr_preparer()
     @recorded_by_proxy
     def test_set_audience(self, containerregistry_endpoint):
         authority = get_authority(containerregistry_endpoint)
         credential = self.get_credential(authority=authority)
-        valid_audience = get_audience(authority)
+        
+        with ContainerRegistryClient(endpoint=containerregistry_endpoint, credential=credential) as client:
+            for repo in client.list_repository_names():
+                pass
 
+        valid_audience = get_audience(authority)
         with ContainerRegistryClient(
             endpoint=containerregistry_endpoint, credential=credential, audience=valid_audience
         ) as client:
             for repo in client.list_repository_names():
                 pass
-        
-        with ContainerRegistryClient(endpoint=containerregistry_endpoint, credential=credential) as client:
-            if valid_audience == get_audience(AzureAuthorityHosts.AZURE_PUBLIC_CLOUD):
-                for repo in client.list_repository_names():
-                    pass
-                
-                invalid_audience = get_audience(AzureAuthorityHosts.AZURE_GOVERNMENT)
-                invalid_client = ContainerRegistryClient(
-                    endpoint=containerregistry_endpoint, credential=credential, audience=invalid_audience
-                )
-                with pytest.raises(ClientAuthenticationError):           
-                    for repo in invalid_client.list_repository_names():
-                        pass
-            else:
+
+        if valid_audience == get_audience(AzureAuthorityHosts.AZURE_PUBLIC_CLOUD):
+            invalid_audience = get_audience(AzureAuthorityHosts.AZURE_GOVERNMENT)
+            with ContainerRegistryClient(
+                endpoint=containerregistry_endpoint, credential=credential, audience=invalid_audience
+            ) as client:
                 with pytest.raises(ClientAuthenticationError):
                     for repo in client.list_repository_names():
                         pass
-    
+
     @acr_preparer()
     @recorded_by_proxy
     def test_list_tags_in_empty_repo(self, containerregistry_endpoint):
         with self.create_registry_client(containerregistry_endpoint) as client:
             # cleanup tags in ALPINE repo
             for tag in client.list_tag_properties(ALPINE):
                 client.delete_tag(ALPINE, tag.name)
```

## Comparing `azure-containerregistry-1.1.0b3/tests/test_anon_access_async.py` & `azure-containerregistry-1.1.0b4/tests/test_anon_access_async.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b3/tests/perfstress_tests/list_repositories.py` & `azure-containerregistry-1.1.0b4/tests/perfstress_tests/list_repositories.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b3/samples/sample_delete_tags.py` & `azure-containerregistry-1.1.0b4/samples/sample_delete_tags.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b3/samples/sample_delete_images.py` & `azure-containerregistry-1.1.0b4/samples/sample_delete_images.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b3/samples/sample_delete_tags_async.py` & `azure-containerregistry-1.1.0b4/samples/sample_delete_tags_async.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b3/samples/sample_delete_images_async.py` & `azure-containerregistry-1.1.0b4/samples/sample_delete_images_async.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b3/samples/sample_hello_world.py` & `azure-containerregistry-1.1.0b4/samples/sample_hello_world.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b3/samples/sample_list_tags.py` & `azure-containerregistry-1.1.0b4/samples/sample_list_tags.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b3/samples/utilities.py` & `azure-containerregistry-1.1.0b4/samples/utilities.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b3/samples/sample_set_image_properties_async.py` & `azure-containerregistry-1.1.0b4/samples/sample_set_image_properties_async.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b3/samples/sample_list_tags_async.py` & `azure-containerregistry-1.1.0b4/samples/sample_list_tags_async.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b3/samples/README.md` & `azure-containerregistry-1.1.0b4/samples/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 |**File Name**|**Description**|
 |-------------|---------------|
 |[sample_hello_world.py][hello_world] ([sample_hello_world_async.py][hello_world_async]) |Instantiate a `ContainerRegistryClient` object and iterating through the collection of tags in the repository with anonymous access |
 |[sample_delete_tags.py][delete_tags] ([sample_delete_tags_async.py][delete_tags_async]) | Delete tags from a repository |
 |[sample_delete_images.py][delete_images] ([sample_delete_images_async.py][delete_images_async]) | Delete images from a repository |
 |[sample_set_image_properties.py][set_image_properties] ([sample_set_image_properties_async.py][set_image_properties_async]) | Set read/write/delete properties on an image |
 |[sample_list_tags.py][list_tags] ([sample_list_tags_async.py][list_tags_async]) | List tags on an image with anonymous access |
-|[sample_upload_download_manifest.py][upload_download_manifest] | Upload and download an OCI manifest and blob to and from a repository |
+|[sample_set_get_image.py][set_get_image] ([sample_set_get_image_async.py][set_get_image_async]) | Set and get a manifest, and upload and download a blob to and from a repository |
 
 ### Prerequisites
 * Python 3.7 or later is required to use this package.
 * You need an [Azure subscription][azure_sub] and a [Container Registry account][container_registry_docs] to use this package.
 
 ## Setup
 
@@ -57,8 +57,9 @@
 [delete_tags_async]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/containerregistry/azure-containerregistry/samples/sample_delete_tags_async.py
 [delete_images]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/containerregistry/azure-containerregistry/samples/sample_delete_images.py
 [delete_images_async]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/containerregistry/azure-containerregistry/samples/sample_delete_images_async.py
 [set_image_properties]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/containerregistry/azure-containerregistry/samples/sample_set_image_properties.py
 [set_image_properties_async]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/containerregistry/azure-containerregistry/samples/sample_set_image_properties_async.py
 [list_tags]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/containerregistry/azure-containerregistry/samples/sample_list_tags.py
 [list_tags_async]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/containerregistry/azure-containerregistry/samples/sample_list_tags_async.py
-[upload_download_manifest]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/containerregistry/azure-containerregistry/samples/sample_upload_download_manifest.py
+[set_get_image]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/containerregistry/azure-containerregistry/samples/sample_set_get_image.py
+[set_get_image_async]: https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/containerregistry/azure-containerregistry/samples/sample_set_get_image_async.py
```

## Comparing `azure-containerregistry-1.1.0b3/samples/sample_set_image_properties.py` & `azure-containerregistry-1.1.0b4/samples/sample_set_image_properties.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b3/samples/sample_hello_world_async.py` & `azure-containerregistry-1.1.0b4/samples/sample_hello_world_async.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b3/azure_containerregistry.egg-info/PKG-INFO` & `azure-containerregistry-1.1.0b4/azure_containerregistry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-containerregistry
-Version: 1.1.0b3
+Version: 1.1.0b4
 Summary: Microsoft Azure Azure Container Registry Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azuresdkengsysadmins@microsoft.com
 License: MIT License
 Project-URL: Bug Reports, https://github.com/Azure/azure-sdk-for-python/issues
 Project-URL: Source, https://github.com/Azure/azure-sdk-python
```

## Comparing `azure-containerregistry-1.1.0b3/azure_containerregistry.egg-info/SOURCES.txt` & `azure-containerregistry-1.1.0b4/azure_containerregistry.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -56,17 +56,18 @@
 samples/sample_delete_images_async.py
 samples/sample_delete_tags.py
 samples/sample_delete_tags_async.py
 samples/sample_hello_world.py
 samples/sample_hello_world_async.py
 samples/sample_list_tags.py
 samples/sample_list_tags_async.py
+samples/sample_set_get_image.py
+samples/sample_set_get_image_async.py
 samples/sample_set_image_properties.py
 samples/sample_set_image_properties_async.py
-samples/sample_upload_download_manifest.py
 samples/utilities.py
 tests/asynctestcase.py
 tests/conftest.py
 tests/constants.py
 tests/preparer.py
 tests/test_anon_access.py
 tests/test_anon_access_async.py
```

