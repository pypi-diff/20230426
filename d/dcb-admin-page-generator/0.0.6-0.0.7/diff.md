# Comparing `tmp/dcb_admin_page_generator-0.0.6.tar.gz` & `tmp/dcb_admin_page_generator-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcb_admin_page_generator-0.0.6.tar", last modified: Fri Apr 14 02:29:23 2023, max compression
+gzip compressed data, was "dcb_admin_page_generator-0.0.7.tar", last modified: Wed Apr 26 06:02:59 2023, max compression
```

## Comparing `dcb_admin_page_generator-0.0.6.tar` & `dcb_admin_page_generator-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 02:29:23.010128 dcb_admin_page_generator-0.0.6/
--rw-rw-rw-   0        0        0     1088 2023-04-12 01:46:29.000000 dcb_admin_page_generator-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      664 2023-04-14 02:29:23.009131 dcb_admin_page_generator-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-04-11 07:24:11.000000 dcb_admin_page_generator-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 02:29:22.952305 dcb_admin_page_generator-0.0.6/dcb_admin_page_generator/
--rw-rw-rw-   0        0        0       25 2023-03-30 02:20:19.000000 dcb_admin_page_generator-0.0.6/dcb_admin_page_generator/__init__.py
--rw-rw-rw-   0        0        0     6617 2023-04-14 02:07:21.000000 dcb_admin_page_generator-0.0.6/dcb_admin_page_generator/config.py
--rw-rw-rw-   0        0        0     3005 2023-04-14 02:16:54.000000 dcb_admin_page_generator-0.0.6/dcb_admin_page_generator/main.py
--rw-rw-rw-   0        0        0    10139 2023-04-11 08:45:36.000000 dcb_admin_page_generator-0.0.6/dcb_admin_page_generator/page_class.py
-drwxrwxrwx   0        0        0        0 2023-04-14 02:29:23.008134 dcb_admin_page_generator-0.0.6/dcb_admin_page_generator/template/
--rw-rw-rw-   0        0        0        0 2023-04-11 07:48:27.000000 dcb_admin_page_generator-0.0.6/dcb_admin_page_generator/template/__init__.py
--rw-rw-rw-   0        0        0     2531 2023-04-11 07:12:32.000000 dcb_admin_page_generator-0.0.6/dcb_admin_page_generator/template/add_or_edit.vue
--rw-rw-rw-   0        0        0     2258 2023-04-11 07:11:16.000000 dcb_admin_page_generator-0.0.6/dcb_admin_page_generator/template/dialog_add_or_edit.vue
--rw-rw-rw-   0        0        0     2762 2023-04-11 07:10:16.000000 dcb_admin_page_generator-0.0.6/dcb_admin_page_generator/template/dialog_list.vue
--rw-rw-rw-   0        0        0     5529 2023-04-06 07:21:58.000000 dcb_admin_page_generator-0.0.6/dcb_admin_page_generator/template/index.vue
-drwxrwxrwx   0        0        0        0 2023-04-14 02:29:22.958289 dcb_admin_page_generator-0.0.6/dcb_admin_page_generator.egg-info/
--rw-rw-rw-   0        0        0      664 2023-04-14 02:29:22.000000 dcb_admin_page_generator-0.0.6/dcb_admin_page_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      609 2023-04-14 02:29:22.000000 dcb_admin_page_generator-0.0.6/dcb_admin_page_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 02:29:22.000000 dcb_admin_page_generator-0.0.6/dcb_admin_page_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-04-14 02:29:22.000000 dcb_admin_page_generator-0.0.6/dcb_admin_page_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 02:29:23.010128 dcb_admin_page_generator-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      695 2023-04-14 02:29:12.000000 dcb_admin_page_generator-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 06:02:59.057579 dcb_admin_page_generator-0.0.7/
+-rw-rw-rw-   0        0        0     1088 2023-04-12 01:46:29.000000 dcb_admin_page_generator-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      664 2023-04-26 06:02:59.056583 dcb_admin_page_generator-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-04-11 07:24:11.000000 dcb_admin_page_generator-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 06:02:58.982779 dcb_admin_page_generator-0.0.7/dcb_admin_page_generator/
+-rw-rw-rw-   0        0        0       25 2023-03-30 02:20:19.000000 dcb_admin_page_generator-0.0.7/dcb_admin_page_generator/__init__.py
+-rw-rw-rw-   0        0        0     7175 2023-04-23 02:09:19.000000 dcb_admin_page_generator-0.0.7/dcb_admin_page_generator/common_class.py
+-rw-rw-rw-   0        0        0     6617 2023-04-14 02:07:21.000000 dcb_admin_page_generator-0.0.7/dcb_admin_page_generator/config.py
+-rw-rw-rw-   0        0        0     1391 2023-04-17 07:55:32.000000 dcb_admin_page_generator-0.0.7/dcb_admin_page_generator/funcs.py
+-rw-rw-rw-   0        0        0     2823 2023-04-18 01:37:05.000000 dcb_admin_page_generator-0.0.7/dcb_admin_page_generator/main.py
+-rw-rw-rw-   0        0        0     6847 2023-04-24 02:15:01.000000 dcb_admin_page_generator-0.0.7/dcb_admin_page_generator/page_class.py
+drwxrwxrwx   0        0        0        0 2023-04-26 06:02:59.046610 dcb_admin_page_generator-0.0.7/dcb_admin_page_generator/template/
+-rw-rw-rw-   0        0        0        0 2023-04-11 07:48:27.000000 dcb_admin_page_generator-0.0.7/dcb_admin_page_generator/template/__init__.py
+-rw-rw-rw-   0        0        0     2531 2023-04-11 07:12:32.000000 dcb_admin_page_generator-0.0.7/dcb_admin_page_generator/template/add_or_edit.vue
+-rw-rw-rw-   0        0        0     2258 2023-04-11 07:11:16.000000 dcb_admin_page_generator-0.0.7/dcb_admin_page_generator/template/dialog_add_or_edit.vue
+-rw-rw-rw-   0        0        0     4014 2023-04-24 02:15:01.000000 dcb_admin_page_generator-0.0.7/dcb_admin_page_generator/template/dialog_list.vue
+-rw-rw-rw-   0        0        0     3848 2023-04-24 02:11:19.000000 dcb_admin_page_generator-0.0.7/dcb_admin_page_generator/template/list.vue
+drwxrwxrwx   0        0        0        0 2023-04-26 06:02:58.988763 dcb_admin_page_generator-0.0.7/dcb_admin_page_generator.egg-info/
+-rw-rw-rw-   0        0        0      664 2023-04-26 06:02:58.000000 dcb_admin_page_generator-0.0.7/dcb_admin_page_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      683 2023-04-26 06:02:58.000000 dcb_admin_page_generator-0.0.7/dcb_admin_page_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 06:02:58.000000 dcb_admin_page_generator-0.0.7/dcb_admin_page_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-04-26 06:02:58.000000 dcb_admin_page_generator-0.0.7/dcb_admin_page_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 06:02:59.057579 dcb_admin_page_generator-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      695 2023-04-26 06:02:49.000000 dcb_admin_page_generator-0.0.7/setup.py
```

### Comparing `dcb_admin_page_generator-0.0.6/LICENSE` & `dcb_admin_page_generator-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dcb_admin_page_generator-0.0.6/PKG-INFO` & `dcb_admin_page_generator-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcb_admin_page_generator
-Version: 0.0.6
+Version: 0.0.7
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: wyz
 Author-email: 846630116@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dcb_admin_page_generator-0.0.6/dcb_admin_page_generator/config.py` & `dcb_admin_page_generator-0.0.7/dcb_admin_page_generator/config.py`

 * *Files identical despite different names*

### Comparing `dcb_admin_page_generator-0.0.6/dcb_admin_page_generator/main.py` & `dcb_admin_page_generator-0.0.7/dcb_admin_page_generator/main.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,50 @@
 import json
 from .page_class import *
-from .config import template_data
+from .funcs import *
 
 
-def deal_yapi(configuration, file_path,yapi_type):
-    # print('file_path', file_path)
-    yapi_url = input('请输入获取数据链接的YapiURL(默认配置直接敲回车)')
-    if yapi_url:
-        id_dict = get_id(yapi_url, configuration)
-        resp = requests.get(f'{configuration["serverUrl"]}{configuration["getInfoPath"]}', params=id_dict)
-        resp_text = json.loads(resp.text)
-    else:
-        resp_text = template_data[yapi_type]
-    # print('resp_text', resp_text)
-    resp_query_path = resp_text["data"]["query_path"]
-    resp_body = json.loads(resp_text["data"]["res_body"])
-    resp_body_other = json.loads(resp_text["data"]["req_body_other"])
-    return resp_query_path, resp_body['properties'], resp_body_other['properties']
-    # else:
-
-
-def generate_page_list(configuration, generator_title, file_path, need_dialog=False):
-    resp_query_path, resp_body, resp_body_other = deal_yapi(configuration, file_path,'list')
-    resp_body = resp_body['data']['properties']['list']['items']['properties']
-    return GenerateList(generator_title, resp_query_path, resp_body_other, resp_body, f'{"dialog_" if need_dialog else ""}list')
-
-
-def generate_page_add(configuration, generator_title, file_path, need_dialog=False):
-    resp_query_path, resp_body, resp_body_other = deal_yapi(configuration, file_path,'add')
-    return GenerateAdd(generator_title, resp_query_path, resp_body_other, resp_body, f'{"dialog_" if need_dialog else ""}add')
+def generate_page_list(configuration, generator_title, file_path, generator_type):
+    # generate_config = deal_yapi(configuration, 'list')
+    # generate_config = {**generate_config, 'generator_title': generator_title,
+    #                    'object_type': f'{"dialog_" if need_dialog else "" }list', 'file_path': file_path,
+    #                    'resp_body': generate_config['resp_body']['data']['properties']['list']['items']['properties']
+    #                    }
+    return GenerateList(configuration, generator_title, file_path, generator_type)
 
 
-def generator(config, generator_title, generator_type, file_path):
+def generate_page_add(configuration, generator_title, file_path, generator_type):
+    # generate_config = deal_yapi(configuration, 'add')
+    # generate_config = {**generate_config, 'generator_title': generator_title, 'file_path': file_path,
+    #                    'object_type': f'{"dialog_" if need_dialog else ""}add'}
+    return GenerateAdd(configuration, generator_title, file_path, generator_type)
+
+
+def generator(config):
     # page_type = input('请输入想要生成的Page Type(list,add,form,dialog_list,dialog_add,dialog_form)')
+    file_path = get_user_input('输入生成目标路径(不填生成在当前根页面)')
+    file_path = file_path + "/" if file_path else ""
+
+    generator_title = get_user_input('请输入生成页面标题(必填)')
+    generator_type = get_user_input('请输入想要生成的Page Type(1、list 2、add 3、dialog_list 4、dialog_add)')
+
     page_dict = {'1': 'list', 'list': 'list',
                  '2': 'add', 'add': 'add',
                  '3': 'dialog_list', 'dialog_list': 'dialog_list',
                  '4': 'dialog_add', 'dialog_add': 'dialog_add'}
     generator_type = page_dict[generator_type]
 
     if generator_type == 'list':
-        return generate_page_list(config, generator_title, file_path)
+        return generate_page_list(config, generator_title, file_path, generator_type)
     elif generator_type == 'add':
-        return generate_page_add(config, generator_title, file_path)
+        return generate_page_add(config, generator_title, file_path, generator_type)
     elif generator_type == 'dialog_list':
-        return generate_page_list(config, generator_title, file_path, need_dialog=True)
+        return generate_page_list(config, generator_title, file_path, generator_type)
     elif generator_type == 'dialog_add':
-        return generate_page_add(config, generator_title, file_path, need_dialog=True)
+        return generate_page_add(config, generator_title, file_path, generator_type)
 
 
 # if __name__ == '__main__':
     # from config import defineConfig as temp_cfg
     # target_file_path = input('输入生成目标路径')
     # page_title = input('请输入生成页面标题')
     # page_type = input('请输入想要生成的Page Type(1、list 2、add 3、dialog_list 4、dialog_add)')
```

### Comparing `dcb_admin_page_generator-0.0.6/dcb_admin_page_generator/template/add_or_edit.vue` & `dcb_admin_page_generator-0.0.7/dcb_admin_page_generator/template/add_or_edit.vue`

 * *Files identical despite different names*

### Comparing `dcb_admin_page_generator-0.0.6/dcb_admin_page_generator/template/dialog_add_or_edit.vue` & `dcb_admin_page_generator-0.0.7/dcb_admin_page_generator/template/dialog_add_or_edit.vue`

 * *Files identical despite different names*

### Comparing `dcb_admin_page_generator-0.0.6/dcb_admin_page_generator.egg-info/PKG-INFO` & `dcb_admin_page_generator-0.0.7/dcb_admin_page_generator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcb-admin-page-generator
-Version: 0.0.6
+Version: 0.0.7
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: wyz
 Author-email: 846630116@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dcb_admin_page_generator-0.0.6/dcb_admin_page_generator.egg-info/SOURCES.txt` & `dcb_admin_page_generator-0.0.7/dcb_admin_page_generator.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 LICENSE
 README.md
 setup.py
 dcb_admin_page_generator/__init__.py
+dcb_admin_page_generator/common_class.py
 dcb_admin_page_generator/config.py
+dcb_admin_page_generator/funcs.py
 dcb_admin_page_generator/main.py
 dcb_admin_page_generator/page_class.py
 dcb_admin_page_generator.egg-info/PKG-INFO
 dcb_admin_page_generator.egg-info/SOURCES.txt
 dcb_admin_page_generator.egg-info/dependency_links.txt
 dcb_admin_page_generator.egg-info/top_level.txt
 dcb_admin_page_generator/template/__init__.py
 dcb_admin_page_generator/template/add_or_edit.vue
 dcb_admin_page_generator/template/dialog_add_or_edit.vue
 dcb_admin_page_generator/template/dialog_list.vue
-dcb_admin_page_generator/template/index.vue
+dcb_admin_page_generator/template/list.vue
```

### Comparing `dcb_admin_page_generator-0.0.6/setup.py` & `dcb_admin_page_generator-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dcb_admin_page_generator",
-    version="0.0.6",
+    version="0.0.7",
     author="wyz",
     author_email="846630116@qq.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(exclude=['ceshi', 'config']),
```

