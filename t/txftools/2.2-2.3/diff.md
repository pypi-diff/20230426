# Comparing `tmp/txftools-2.2.tar.gz` & `tmp/txftools-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "txftools-2.2.tar", last modified: Fri Apr 21 01:44:32 2023, max compression
+gzip compressed data, was "txftools-2.3.tar", last modified: Wed Apr 26 02:05:26 2023, max compression
```

## Comparing `txftools-2.2.tar` & `txftools-2.3.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 01:44:32.419455 txftools-2.2/
--rw-rw-rw-   0        0        0    11558 2022-06-13 09:28:44.000000 txftools-2.2/LICENSE
--rw-rw-rw-   0        0        0      427 2023-04-21 01:44:32.419455 txftools-2.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-21 01:44:32.419455 txftools-2.2/setup.cfg
--rw-rw-rw-   0        0        0      902 2023-04-21 01:44:11.000000 txftools-2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 01:44:32.403497 txftools-2.2/txftools/
--rw-rw-rw-   0        0        0     1205 2022-06-13 09:15:25.000000 txftools-2.2/txftools/__init__.py
--rw-rw-rw-   0        0        0     5239 2022-06-16 02:50:15.000000 txftools-2.2/txftools/currency_sorted.py
--rw-rw-rw-   0        0        0     9164 2023-04-21 01:42:35.000000 txftools-2.2/txftools/encryption.py
--rw-rw-rw-   0        0        0     4690 2022-07-07 11:11:56.000000 txftools-2.2/txftools/execute_redis.py
--rw-rw-rw-   0        0        0    23966 2023-01-14 06:53:46.000000 txftools-2.2/txftools/format_data.py
--rw-rw-rw-   0        0        0     4800 2022-11-21 03:28:29.000000 txftools-2.2/txftools/lazy_test.py
--rw-rw-rw-   0        0        0     4383 2022-05-24 01:50:39.000000 txftools-2.2/txftools/province.py
--rw-rw-rw-   0        0        0     3534 2022-07-01 09:43:55.000000 txftools-2.2/txftools/send_emals.py
--rw-rw-rw-   0        0        0     6673 2022-06-30 05:08:18.000000 txftools-2.2/txftools/ssh_online.py
--rw-rw-rw-   0        0        0    13082 2022-07-15 05:24:00.000000 txftools-2.2/txftools/timer.py
-drwxrwxrwx   0        0        0        0 2023-04-21 01:44:32.418458 txftools-2.2/txftools.egg-info/
--rw-rw-rw-   0        0        0      427 2023-04-21 01:44:32.000000 txftools-2.2/txftools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      431 2023-04-21 01:44:32.000000 txftools-2.2/txftools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 01:44:32.000000 txftools-2.2/txftools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-21 01:44:32.000000 txftools-2.2/txftools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-21 01:44:32.000000 txftools-2.2/txftools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2022-07-25 12:19:26.000000 txftools-2.2/txftools.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-04-26 02:05:26.126616 txftools-2.3/
+-rw-rw-rw-   0        0        0    11558 2022-06-13 09:28:44.000000 txftools-2.3/LICENSE
+-rw-rw-rw-   0        0        0      427 2023-04-26 02:05:26.125619 txftools-2.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-26 02:05:26.126616 txftools-2.3/setup.cfg
+-rw-rw-rw-   0        0        0      902 2023-04-26 02:04:56.000000 txftools-2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 02:05:26.111655 txftools-2.3/txftools/
+-rw-rw-rw-   0        0        0     1205 2022-06-13 09:15:25.000000 txftools-2.3/txftools/__init__.py
+-rw-rw-rw-   0        0        0     5239 2022-06-16 02:50:15.000000 txftools-2.3/txftools/currency_sorted.py
+-rw-rw-rw-   0        0        0    21033 2023-04-26 02:01:19.000000 txftools-2.3/txftools/encryption.py
+-rw-rw-rw-   0        0        0     4690 2022-07-07 11:11:56.000000 txftools-2.3/txftools/execute_redis.py
+-rw-rw-rw-   0        0        0    23966 2023-01-14 06:53:46.000000 txftools-2.3/txftools/format_data.py
+-rw-rw-rw-   0        0        0     4800 2022-11-21 03:28:29.000000 txftools-2.3/txftools/lazy_test.py
+-rw-rw-rw-   0        0        0      514 2023-04-22 06:18:06.000000 txftools-2.3/txftools/pipfile_lock_requirements.py
+-rw-rw-rw-   0        0        0     4383 2022-05-24 01:50:39.000000 txftools-2.3/txftools/province.py
+-rw-rw-rw-   0        0        0     3534 2022-07-01 09:43:55.000000 txftools-2.3/txftools/send_emals.py
+-rw-rw-rw-   0        0        0     6673 2022-06-30 05:08:18.000000 txftools-2.3/txftools/ssh_online.py
+-rw-rw-rw-   0        0        0    13181 2023-04-26 02:04:13.000000 txftools-2.3/txftools/timer.py
+drwxrwxrwx   0        0        0        0 2023-04-26 02:05:26.125619 txftools-2.3/txftools.egg-info/
+-rw-rw-rw-   0        0        0      427 2023-04-26 02:05:26.000000 txftools-2.3/txftools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      469 2023-04-26 02:05:26.000000 txftools-2.3/txftools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 02:05:26.000000 txftools-2.3/txftools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-26 02:05:26.000000 txftools-2.3/txftools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-26 02:05:26.000000 txftools-2.3/txftools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2022-07-25 12:19:26.000000 txftools-2.3/txftools.egg-info/zip-safe
```

### Comparing `txftools-2.2/LICENSE` & `txftools-2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `txftools-2.2/setup.py` & `txftools-2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding:utf-8 -*-
 from setuptools import setup, find_packages
 
 setup(name='txftools',  # 名字
-      version='2.2',  # 版本
+      version='2.3',  # 版本
       long_description_content_type="text/markdown",
       long_description='README',
       description='django response middleware',  # 简介一般我们放在readme.md
       classifiers=[
           'Programming Language :: Python',  # python
           'Intended Audience :: Developers',  # 受众人
           'Operating System :: OS Independent',  # 系统
```

### Comparing `txftools-2.2/txftools/__init__.py` & `txftools-2.3/txftools/__init__.py`

 * *Files identical despite different names*

### Comparing `txftools-2.2/txftools/currency_sorted.py` & `txftools-2.3/txftools/currency_sorted.py`

 * *Files identical despite different names*

### Comparing `txftools-2.2/txftools/execute_redis.py` & `txftools-2.3/txftools/execute_redis.py`

 * *Files identical despite different names*

### Comparing `txftools-2.2/txftools/format_data.py` & `txftools-2.3/txftools/format_data.py`

 * *Files identical despite different names*

### Comparing `txftools-2.2/txftools/lazy_test.py` & `txftools-2.3/txftools/lazy_test.py`

 * *Files identical despite different names*

### Comparing `txftools-2.2/txftools/province.py` & `txftools-2.3/txftools/province.py`

 * *Files identical despite different names*

### Comparing `txftools-2.2/txftools/send_emals.py` & `txftools-2.3/txftools/send_emals.py`

 * *Files identical despite different names*

### Comparing `txftools-2.2/txftools/ssh_online.py` & `txftools-2.3/txftools/ssh_online.py`

 * *Files identical despite different names*

### Comparing `txftools-2.2/txftools/timer.py` & `txftools-2.3/txftools/timer.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,14 +77,15 @@
         # 星期几(0,6  0代表周1)， 本月共几天  int
         _, self.month_len = calendar.monthrange(self.year, self.month)
         self.this_week = datetime.date(self.year, self.month, self.day).weekday()
         # 季度
         self.quarter = (self.month - 1) // 3 + 1
         # 字符串时间
         self.str_date = self.this_time.strftime('%Y-%m-%d')
+        self.str_date_hms = self.this_time.strftime('%Y-%m-%d %H:%M:%S')
 
     def time_type(self, date_time=None, dtype=None):
         """
         return
         1 '2022-02-28 10:24:56'
         2 datetime.datetime(2022, 2, 28, 10, 24, 56, 221989)
         """
@@ -357,11 +358,12 @@
         s = s.split('-')[0]
         e = e.split('-')[0]
         return range(s, e + 1)
 
 
 if __name__ == '__main__':
 
-    # c = CustomBasicDateTime(this_time='2022-07-12')
+    c = CustomBasicDateTime(this_time='2022-07-12')
     # print(c.this_week)
+    print(c.str_date_hms)
     pass
```

