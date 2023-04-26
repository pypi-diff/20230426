# Comparing `tmp/pointclass-0.4.tar.gz` & `tmp/pointclass-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pointclass-0.4.tar", last modified: Tue Apr 25 16:20:06 2023, max compression
+gzip compressed data, was "pointclass-0.5.tar", last modified: Tue Apr 25 16:27:13 2023, max compression
```

## Comparing `pointclass-0.4.tar` & `pointclass-0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 16:20:06.807290 pointclass-0.4/
--rw-rw-rw-   0        0        0      177 2023-04-25 16:20:05.868831 pointclass-0.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-25 10:31:30.000000 pointclass-0.4/licence.txt.txt
-drwxrwxrwx   0        0        0        0 2023-04-25 16:20:05.828439 pointclass-0.4/pointclass/
--rw-rw-rw-   0        0        0      563 2023-04-25 10:59:19.000000 pointclass-0.4/pointclass/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 16:20:05.866621 pointclass-0.4/pointclass.egg-info/
--rw-rw-rw-   0        0        0      177 2023-04-25 16:20:05.000000 pointclass-0.4/pointclass.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      184 2023-04-25 16:20:05.000000 pointclass-0.4/pointclass.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 16:20:05.000000 pointclass-0.4/pointclass.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-25 16:20:05.000000 pointclass-0.4/pointclass.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 16:20:06.823134 pointclass-0.4/setup.cfg
--rw-rw-rw-   0        0        0      247 2023-04-25 16:19:19.000000 pointclass-0.4/setup1.py
+drwxrwxrwx   0        0        0        0 2023-04-25 16:27:13.770138 pointclass-0.5/
+-rw-rw-rw-   0        0        0      177 2023-04-25 16:27:13.766144 pointclass-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-25 10:31:30.000000 pointclass-0.5/licence.txt.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 16:27:13.745335 pointclass-0.5/pointclass/
+-rw-rw-rw-   0        0        0      569 2023-04-25 16:26:49.000000 pointclass-0.5/pointclass/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 16:27:13.765148 pointclass-0.5/pointclass.egg-info/
+-rw-rw-rw-   0        0        0      177 2023-04-25 16:27:13.000000 pointclass-0.5/pointclass.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      184 2023-04-25 16:27:13.000000 pointclass-0.5/pointclass.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 16:27:13.000000 pointclass-0.5/pointclass.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-25 16:27:13.000000 pointclass-0.5/pointclass.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 16:27:13.770138 pointclass-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      247 2023-04-25 16:27:05.000000 pointclass-0.5/setup1.py
```

### Comparing `pointclass-0.4/pointclass/__init__.py` & `pointclass-0.5/pointclass/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,8 +13,9 @@
     def __mult__(self,p):
         return(self.x * p.x,self.y * p.y)
     def __eq__(self,p):
          return(self.x==p.x,self.y==p.y)
     def __repro__():
         return "point(self.x,self.y)"
     def distance(p1,p2):
-        return math.hypot(p2.x-p1.x,p2.y-p1.y)
+        return math.hypot(p2.x-p1.x,p2.y-p1.y)
+
```

