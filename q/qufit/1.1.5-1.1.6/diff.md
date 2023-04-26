# Comparing `tmp/qufit-1.1.5.tar.gz` & `tmp/qufit-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qufit-1.1.5.tar", last modified: Tue Apr 25 14:57:40 2023, max compression
+gzip compressed data, was "qufit-1.1.6.tar", last modified: Tue Apr 25 15:02:08 2023, max compression
```

## Comparing `qufit-1.1.5.tar` & `qufit-1.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 14:57:40.242327 qufit-1.1.5/
--rw-rw-rw-   0        0        0      820 2023-04-25 14:57:40.241330 qufit-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      331 2022-11-06 13:08:56.000000 qufit-1.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 14:57:40.220384 qufit-1.1.5/qufit/
--rw-rw-rw-   0        0        0       16 2022-11-06 12:49:07.000000 qufit-1.1.5/qufit/__init__.py
--rw-rw-rw-   0        0        0    26238 2023-04-25 14:57:06.000000 qufit-1.1.5/qufit/dataTools.py
--rw-rw-rw-   0        0        0     3907 2022-09-21 03:02:11.000000 qufit-1.1.5/qufit/opt.py
--rw-rw-rw-   0        0        0    59941 2023-04-24 07:03:24.000000 qufit-1.1.5/qufit/optimize.py
-drwxrwxrwx   0        0        0        0 2023-04-25 14:57:40.238336 qufit-1.1.5/qufit.egg-info/
--rw-rw-rw-   0        0        0      820 2023-04-25 14:57:40.000000 qufit-1.1.5/qufit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-04-25 14:57:40.000000 qufit-1.1.5/qufit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 14:57:40.000000 qufit-1.1.5/qufit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-25 14:57:40.000000 qufit-1.1.5/qufit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 14:57:40.242327 qufit-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0      707 2023-04-25 14:57:18.000000 qufit-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 15:02:08.703328 qufit-1.1.6/
+-rw-rw-rw-   0        0        0      820 2023-04-25 15:02:08.702331 qufit-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2022-11-06 13:08:56.000000 qufit-1.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 15:02:08.684380 qufit-1.1.6/qufit/
+-rw-rw-rw-   0        0        0       16 2022-11-06 12:49:07.000000 qufit-1.1.6/qufit/__init__.py
+-rw-rw-rw-   0        0        0    26246 2023-04-25 15:01:15.000000 qufit-1.1.6/qufit/dataTools.py
+-rw-rw-rw-   0        0        0     3907 2022-09-21 03:02:11.000000 qufit-1.1.6/qufit/opt.py
+-rw-rw-rw-   0        0        0    59941 2023-04-24 07:03:24.000000 qufit-1.1.6/qufit/optimize.py
+drwxrwxrwx   0        0        0        0 2023-04-25 15:02:08.701338 qufit-1.1.6/qufit.egg-info/
+-rw-rw-rw-   0        0        0      820 2023-04-25 15:02:08.000000 qufit-1.1.6/qufit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-04-25 15:02:08.000000 qufit-1.1.6/qufit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 15:02:08.000000 qufit-1.1.6/qufit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-25 15:02:08.000000 qufit-1.1.6/qufit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 15:02:08.703328 qufit-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      707 2023-04-25 15:01:52.000000 qufit-1.1.6/setup.py
```

### Comparing `qufit-1.1.5/PKG-INFO` & `qufit-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qufit
-Version: 1.1.5
+Version: 1.1.6
 Summary: 本模块包括了超导量子计算实验中常用模型的拟合函数于数据处理方法。
 Home-page: https://pypi.org/
 Author: 赵寿宽(sk zhao)
 Author-email: 2396776980@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `qufit-1.1.5/qufit/dataTools.py` & `qufit-1.1.6/qufit/dataTools.py`

 * *Files 1% similar despite different names*

```diff
@@ -310,16 +310,16 @@
         plt.close()
 
 def cutCircle(info_c0,info_c1,data):
         # print(data.shape)
         # data0, data1 = data[0,:], data[1,:]
         c0, r0 = info_c0[0], info_c0[1]
         c1, r1 = info_c1[0], info_c1[1]
-        s0 = (data.real-c0[0])**2+(data.imag-c0[1])**2
-        s1 = (data.real-c1[0])**2+(data.imag-c1[1])**2
+        s0 = (data.real-c0.real)**2+(data.imag-c0.imag)**2
+        s1 = (data.real-c1.real)**2+(data.imag-c1.imag)**2
         # idx = ((np.abs(s0)<r0**2) +  (np.abs(s1)<r1**2))
         s1_cut = (s1<r1**2)*1
         s0_cut = (s0<r0**2)*1
         num0 = np.count_nonzero(s0_cut)
         num1 = np.count_nonzero(s1_cut)
         print(num0)
         num0 /= (num0+num1)
```

### Comparing `qufit-1.1.5/qufit/opt.py` & `qufit-1.1.6/qufit/opt.py`

 * *Files identical despite different names*

### Comparing `qufit-1.1.5/qufit/optimize.py` & `qufit-1.1.6/qufit/optimize.py`

 * *Files identical despite different names*

### Comparing `qufit-1.1.5/qufit.egg-info/PKG-INFO` & `qufit-1.1.6/qufit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qufit
-Version: 1.1.5
+Version: 1.1.6
 Summary: 本模块包括了超导量子计算实验中常用模型的拟合函数于数据处理方法。
 Home-page: https://pypi.org/
 Author: 赵寿宽(sk zhao)
 Author-email: 2396776980@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `qufit-1.1.5/setup.py` & `qufit-1.1.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="qufit",
-    version="1.1.5",
+    version="1.1.6",
     author="赵寿宽(sk zhao)",
     author_email="2396776980@qq.com",
     description="本模块包括了超导量子计算实验中常用模型的拟合函数于数据处理方法。",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://pypi.org/",
     packages=setuptools.find_packages(),
```

