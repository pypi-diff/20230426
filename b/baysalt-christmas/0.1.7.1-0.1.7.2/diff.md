# Comparing `tmp/baysalt_christmas-0.1.7.1.tar.gz` & `tmp/baysalt_christmas-0.1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baysalt_christmas-0.1.7.1.tar", last modified: Mon Apr 24 06:23:05 2023, max compression
+gzip compressed data, was "baysalt_christmas-0.1.7.2.tar", last modified: Wed Apr 26 03:44:06 2023, max compression
```

## Comparing `baysalt_christmas-0.1.7.1.tar` & `baysalt_christmas-0.1.7.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-04-24 06:23:05.209130 baysalt_christmas-0.1.7.1/
--rw-r--r--   0 christmas   (501) staff       (20)    10244 2023-04-19 08:43:20.000000 baysalt_christmas-0.1.7.1/.DS_Store
--rw-r--r--   0 christmas   (501) staff       (20)      117 2023-03-25 19:22:27.000000 baysalt_christmas-0.1.7.1/MANIFEST.in
--rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-04-24 06:23:05.208877 baysalt_christmas-0.1.7.1/PKG-INFO
--rw-r--r--   0 christmas   (501) staff       (20)     3732 2023-03-29 03:30:38.000000 baysalt_christmas-0.1.7.1/README.md
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-04-24 06:23:05.199684 baysalt_christmas-0.1.7.1/baysalt_christmas.egg-info/
--rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-04-24 06:23:05.000000 baysalt_christmas-0.1.7.1/baysalt_christmas.egg-info/PKG-INFO
--rw-r--r--   0 christmas   (501) staff       (20)      729 2023-04-24 06:23:05.000000 baysalt_christmas-0.1.7.1/baysalt_christmas.egg-info/SOURCES.txt
--rw-r--r--   0 christmas   (501) staff       (20)        1 2023-04-24 06:23:05.000000 baysalt_christmas-0.1.7.1/baysalt_christmas.egg-info/dependency_links.txt
--rw-r--r--   0 christmas   (501) staff       (20)       21 2023-04-24 06:23:05.000000 baysalt_christmas-0.1.7.1/baysalt_christmas.egg-info/requires.txt
--rw-r--r--   0 christmas   (501) staff       (20)       10 2023-04-24 06:23:05.000000 baysalt_christmas-0.1.7.1/baysalt_christmas.egg-info/top_level.txt
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-04-24 06:23:05.202355 baysalt_christmas-0.1.7.1/christmas/
--rw-r--r--   0 christmas   (501) staff       (20)    20394 2023-04-24 06:22:46.000000 baysalt_christmas-0.1.7.1/christmas/Blogging.py
--rw-r--r--   0 christmas   (501) staff       (20)     1895 2023-03-25 02:55:02.000000 baysalt_christmas-0.1.7.1/christmas/S_DateTime.py
--rw-r--r--   0 christmas   (501) staff       (20)      445 2023-04-23 12:43:18.000000 baysalt_christmas-0.1.7.1/christmas/__init__.py
--rw-r--r--   0 christmas   (501) staff       (20)     4526 2023-04-24 06:14:31.000000 baysalt_christmas-0.1.7.1/christmas/commonCode.py
--rw-r--r--   0 christmas   (501) staff       (20)     1638 2023-04-12 07:23:55.000000 baysalt_christmas-0.1.7.1/christmas/cprintf.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-04-24 06:23:05.206308 baysalt_christmas-0.1.7.1/christmas/mncPy/
--rw-r--r--   0 christmas   (501) staff       (20)     1203 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.7.1/christmas/mncPy/.gitignore
--rw-r--r--   0 christmas   (501) staff       (20)    35149 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.7.1/christmas/mncPy/LICENSE
--rw-r--r--   0 christmas   (501) staff       (20)      239 2023-03-03 08:53:41.000000 baysalt_christmas-0.1.7.1/christmas/mncPy/__init__.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-04-24 06:23:05.208418 baysalt_christmas-0.1.7.1/christmas/mncPy/__pycache__/
--rw-r--r--   0 christmas   (501) staff       (20)      228 2023-03-26 18:28:05.000000 baysalt_christmas-0.1.7.1/christmas/mncPy/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)     8964 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.7.1/christmas/mncPy/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)     3411 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.7.1/christmas/mncPy/__pycache__/compress.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)    12920 2023-03-09 13:49:40.000000 baysalt_christmas-0.1.7.1/christmas/mncPy/common.py
--rw-r--r--   0 christmas   (501) staff       (20)     4347 2023-03-09 14:00:22.000000 baysalt_christmas-0.1.7.1/christmas/mncPy/compress.py
--rw-r--r--   0 christmas   (501) staff       (20)     3554 2023-03-29 02:58:20.000000 baysalt_christmas-0.1.7.1/christmas/processBar.py
--rw-r--r--   0 christmas   (501) staff       (20)     3473 2023-04-13 06:21:12.000000 baysalt_christmas-0.1.7.1/christmas/read_conf.py
--rw-r--r--   0 christmas   (501) staff       (20)     1506 2022-12-07 09:44:40.000000 baysalt_christmas-0.1.7.1/christmas/server_info.py
--rw-r--r--   0 christmas   (501) staff       (20)      456 2023-03-25 18:44:30.000000 baysalt_christmas-0.1.7.1/run_twine.py
--rw-r--r--   0 christmas   (501) staff       (20)       38 2023-04-24 06:23:05.209215 baysalt_christmas-0.1.7.1/setup.cfg
--rw-r--r--   0 christmas   (501) staff       (20)      796 2023-04-24 06:23:01.000000 baysalt_christmas-0.1.7.1/setup.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-04-26 03:44:06.938433 baysalt_christmas-0.1.7.2/
+-rw-r--r--   0 christmas   (501) staff       (20)    10244 2023-04-19 08:43:20.000000 baysalt_christmas-0.1.7.2/.DS_Store
+-rw-r--r--   0 christmas   (501) staff       (20)      117 2023-03-25 19:22:27.000000 baysalt_christmas-0.1.7.2/MANIFEST.in
+-rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-04-26 03:44:06.938308 baysalt_christmas-0.1.7.2/PKG-INFO
+-rw-r--r--   0 christmas   (501) staff       (20)     3732 2023-03-29 03:30:38.000000 baysalt_christmas-0.1.7.2/README.md
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-04-26 03:44:06.932340 baysalt_christmas-0.1.7.2/baysalt_christmas.egg-info/
+-rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-04-26 03:44:06.000000 baysalt_christmas-0.1.7.2/baysalt_christmas.egg-info/PKG-INFO
+-rw-r--r--   0 christmas   (501) staff       (20)      729 2023-04-26 03:44:06.000000 baysalt_christmas-0.1.7.2/baysalt_christmas.egg-info/SOURCES.txt
+-rw-r--r--   0 christmas   (501) staff       (20)        1 2023-04-26 03:44:06.000000 baysalt_christmas-0.1.7.2/baysalt_christmas.egg-info/dependency_links.txt
+-rw-r--r--   0 christmas   (501) staff       (20)       30 2023-04-26 03:44:06.000000 baysalt_christmas-0.1.7.2/baysalt_christmas.egg-info/requires.txt
+-rw-r--r--   0 christmas   (501) staff       (20)       10 2023-04-26 03:44:06.000000 baysalt_christmas-0.1.7.2/baysalt_christmas.egg-info/top_level.txt
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-04-26 03:44:06.934481 baysalt_christmas-0.1.7.2/christmas/
+-rw-r--r--   0 christmas   (501) staff       (20)    20519 2023-04-26 03:41:40.000000 baysalt_christmas-0.1.7.2/christmas/Blogging.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1895 2023-03-25 02:55:02.000000 baysalt_christmas-0.1.7.2/christmas/S_DateTime.py
+-rw-r--r--   0 christmas   (501) staff       (20)      445 2023-04-23 12:43:18.000000 baysalt_christmas-0.1.7.2/christmas/__init__.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4526 2023-04-24 06:14:31.000000 baysalt_christmas-0.1.7.2/christmas/commonCode.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1638 2023-04-12 07:23:55.000000 baysalt_christmas-0.1.7.2/christmas/cprintf.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-04-26 03:44:06.935982 baysalt_christmas-0.1.7.2/christmas/mncPy/
+-rw-r--r--   0 christmas   (501) staff       (20)     1203 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.7.2/christmas/mncPy/.gitignore
+-rw-r--r--   0 christmas   (501) staff       (20)    35149 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.7.2/christmas/mncPy/LICENSE
+-rw-r--r--   0 christmas   (501) staff       (20)      239 2023-03-03 08:53:41.000000 baysalt_christmas-0.1.7.2/christmas/mncPy/__init__.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-04-26 03:44:06.937952 baysalt_christmas-0.1.7.2/christmas/mncPy/__pycache__/
+-rw-r--r--   0 christmas   (501) staff       (20)      228 2023-03-26 18:28:05.000000 baysalt_christmas-0.1.7.2/christmas/mncPy/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)     8964 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.7.2/christmas/mncPy/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)     3411 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.7.2/christmas/mncPy/__pycache__/compress.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)    12920 2023-03-09 13:49:40.000000 baysalt_christmas-0.1.7.2/christmas/mncPy/common.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4347 2023-03-09 14:00:22.000000 baysalt_christmas-0.1.7.2/christmas/mncPy/compress.py
+-rw-r--r--   0 christmas   (501) staff       (20)     3554 2023-03-29 02:58:20.000000 baysalt_christmas-0.1.7.2/christmas/processBar.py
+-rw-r--r--   0 christmas   (501) staff       (20)     3473 2023-04-13 06:21:12.000000 baysalt_christmas-0.1.7.2/christmas/read_conf.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1506 2022-12-07 09:44:40.000000 baysalt_christmas-0.1.7.2/christmas/server_info.py
+-rw-r--r--   0 christmas   (501) staff       (20)      456 2023-03-25 18:44:30.000000 baysalt_christmas-0.1.7.2/run_twine.py
+-rw-r--r--   0 christmas   (501) staff       (20)       38 2023-04-26 03:44:06.938481 baysalt_christmas-0.1.7.2/setup.cfg
+-rw-r--r--   0 christmas   (501) staff       (20)      796 2023-04-26 03:44:02.000000 baysalt_christmas-0.1.7.2/setup.py
```

### Comparing `baysalt_christmas-0.1.7.1/.DS_Store` & `baysalt_christmas-0.1.7.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.1/PKG-INFO` & `baysalt_christmas-0.1.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baysalt_christmas
-Version: 0.1.7.1
+Version: 0.1.7.2
 Summary: Some simple tools for Christmas
 Author: Christmas
 Author-email: 273519355@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `baysalt_christmas-0.1.7.1/README.md` & `baysalt_christmas-0.1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.1/baysalt_christmas.egg-info/PKG-INFO` & `baysalt_christmas-0.1.7.2/baysalt_christmas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baysalt-christmas
-Version: 0.1.7.1
+Version: 0.1.7.2
 Summary: Some simple tools for Christmas
 Author: Christmas
 Author-email: 273519355@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `baysalt_christmas-0.1.7.1/baysalt_christmas.egg-info/SOURCES.txt` & `baysalt_christmas-0.1.7.2/baysalt_christmas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.1/christmas/Blogging.py` & `baysalt_christmas-0.1.7.2/christmas/Blogging.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             self.PARA_DEFAULT['debug_log_filename'] = f'{self.logfile_name}_debug.log'
             self.PARA_DEFAULT['info_log_filename'] = f'{self.logfile_name}_info.log'
             self.PARA_DEFAULT['warning_log_filename'] = f'{self.logfile_name}_warning.log'
             self.PARA_DEFAULT['error_log_filename'] = f'{self.logfile_name}_error.log'
             self.PARA_DEFAULT['critical_log_filename'] = f'{self.logfile_name}_critical.log'
         
         self.PARA = self.PARA_DEFAULT
-        self.console()
+        self.console
     
     def setup_Blog(self, **kwargs):
         
         self.PARA.update(kwargs)
         self.maxBytes = self.PARA['maxBytes']
         self.backupCount = self.PARA['backupCount']
         self.colors_config = self.PARA['colors_config']
@@ -270,14 +270,16 @@
             self.__write_random_log(level=logging.INFO, _level_log_name=self.info_log_filename)
         if self.switch_write_warning_log:
             self.__write_random_log(level=logging.WARNING, _level_log_name=self.warning_log_filename)
         if self.switch_write_error_log:
             self.__write_random_log(level=logging.ERROR, _level_log_name=self.error_log_filename)
         if self.switch_write_critical_log:
             self.__write_random_log(level=logging.CRITICAL, _level_log_name=self.critical_log_filename)
+            
+        # 如果console被执行了一次，那么删除之前的执行结果，重新执行
         return self.logger
     
     def __write_all_log(self):
         all_logger_handler = self.__init_logger_handler(self.__all_log_path, Rotating=self.Rotating, when=self.when,
                                                         interval=self.interval)  # 收集所有日志文件
         self.__set_log_formatter(all_logger_handler)  # 设置日志输出格式-all日志文件
         self.__set_log_handler(all_logger_handler, level=logging.DEBUG)  # 设置handler级别并添加到logger收集器
@@ -412,8 +414,9 @@
     log1.logger.info("这是日志信息")
     log1.logger.warning("这是警告信息")
     log1.logger.error("这是错误日志信息")
     log1.logger.critical("这是严重级别信息")
 
 
 if __name__ == '__main__':
-    example_Blog_simple()
+    # example_Blog_simple()
+    example_Blog()
```

### Comparing `baysalt_christmas-0.1.7.1/christmas/S_DateTime.py` & `baysalt_christmas-0.1.7.2/christmas/S_DateTime.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.1/christmas/commonCode.py` & `baysalt_christmas-0.1.7.2/christmas/commonCode.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.1/christmas/cprintf.py` & `baysalt_christmas-0.1.7.2/christmas/cprintf.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.1/christmas/mncPy/.gitignore` & `baysalt_christmas-0.1.7.2/christmas/mncPy/.gitignore`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.1/christmas/mncPy/LICENSE` & `baysalt_christmas-0.1.7.2/christmas/mncPy/LICENSE`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.1/christmas/mncPy/__pycache__/common.cpython-39.pyc` & `baysalt_christmas-0.1.7.2/christmas/mncPy/__pycache__/common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.1/christmas/mncPy/__pycache__/compress.cpython-39.pyc` & `baysalt_christmas-0.1.7.2/christmas/mncPy/__pycache__/compress.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.1/christmas/mncPy/common.py` & `baysalt_christmas-0.1.7.2/christmas/mncPy/common.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.1/christmas/mncPy/compress.py` & `baysalt_christmas-0.1.7.2/christmas/mncPy/compress.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.1/christmas/processBar.py` & `baysalt_christmas-0.1.7.2/christmas/processBar.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.1/christmas/read_conf.py` & `baysalt_christmas-0.1.7.2/christmas/read_conf.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.1/christmas/server_info.py` & `baysalt_christmas-0.1.7.2/christmas/server_info.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.1/setup.py` & `baysalt_christmas-0.1.7.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="baysalt_christmas",
-    version="0.1.7.1",
+    version="0.1.7.2",
     author="Christmas",
     author_email="273519355@qq.com",
     description="Some simple tools for Christmas",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     include_package_data=True,
@@ -20,12 +20,12 @@
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     install_requires=[
         'numpy',
         'netCDF4',
         'xarray',
-        # 'mpi4py',
+        'colorlog',
     ],
 )
 # python3 setup.py sdist bdist_wheel
 # twine upload dist/*
```

