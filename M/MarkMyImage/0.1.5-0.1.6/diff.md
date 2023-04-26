# Comparing `tmp/MarkMyImage-0.1.5.tar.gz` & `tmp/MarkMyImage-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MarkMyImage-0.1.5.tar", last modified: Wed Apr 26 11:14:18 2023, max compression
+gzip compressed data, was "MarkMyImage-0.1.6.tar", last modified: Wed Apr 26 11:22:31 2023, max compression
```

## Comparing `MarkMyImage-0.1.5.tar` & `MarkMyImage-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 alatas    (1001) alatas    (1001)        0 2023-04-26 11:14:18.125583 MarkMyImage-0.1.5/
-drwxrwxr-x   0 alatas    (1001) alatas    (1001)        0 2023-04-26 11:14:18.121583 MarkMyImage-0.1.5/MarkMyImage/
--rw-rw-r--   0 alatas    (1001) alatas    (1001)     3425 2023-04-26 11:14:07.000000 MarkMyImage-0.1.5/MarkMyImage/__init__.py
-drwxrwxr-x   0 alatas    (1001) alatas    (1001)        0 2023-04-26 11:14:18.125583 MarkMyImage-0.1.5/MarkMyImage.egg-info/
--rw-rw-r--   0 alatas    (1001) alatas    (1001)     2215 2023-04-26 11:14:18.000000 MarkMyImage-0.1.5/MarkMyImage.egg-info/PKG-INFO
--rw-rw-r--   0 alatas    (1001) alatas    (1001)      254 2023-04-26 11:14:18.000000 MarkMyImage-0.1.5/MarkMyImage.egg-info/SOURCES.txt
--rw-rw-r--   0 alatas    (1001) alatas    (1001)        1 2023-04-26 11:14:18.000000 MarkMyImage-0.1.5/MarkMyImage.egg-info/dependency_links.txt
--rw-rw-r--   0 alatas    (1001) alatas    (1001)       41 2023-04-26 11:14:18.000000 MarkMyImage-0.1.5/MarkMyImage.egg-info/entry_points.txt
--rw-rw-r--   0 alatas    (1001) alatas    (1001)        7 2023-04-26 11:14:18.000000 MarkMyImage-0.1.5/MarkMyImage.egg-info/requires.txt
--rw-rw-r--   0 alatas    (1001) alatas    (1001)       12 2023-04-26 11:14:18.000000 MarkMyImage-0.1.5/MarkMyImage.egg-info/top_level.txt
--rw-rw-r--   0 alatas    (1001) alatas    (1001)     2215 2023-04-26 11:14:18.125583 MarkMyImage-0.1.5/PKG-INFO
--rw-rw-r--   0 alatas    (1001) alatas    (1001)     1602 2023-04-26 09:00:08.000000 MarkMyImage-0.1.5/README.md
--rw-rw-r--   0 alatas    (1001) alatas    (1001)       38 2023-04-26 11:14:18.125583 MarkMyImage-0.1.5/setup.cfg
--rw-rw-r--   0 alatas    (1001) alatas    (1001)     1003 2023-04-26 11:14:15.000000 MarkMyImage-0.1.5/setup.py
+drwxrwxr-x   0 alatas    (1001) alatas    (1001)        0 2023-04-26 11:22:31.852615 MarkMyImage-0.1.6/
+drwxrwxr-x   0 alatas    (1001) alatas    (1001)        0 2023-04-26 11:22:31.852615 MarkMyImage-0.1.6/MarkMyImage/
+-rw-rw-r--   0 alatas    (1001) alatas    (1001)     3575 2023-04-26 11:22:16.000000 MarkMyImage-0.1.6/MarkMyImage/__init__.py
+drwxrwxr-x   0 alatas    (1001) alatas    (1001)        0 2023-04-26 11:22:31.852615 MarkMyImage-0.1.6/MarkMyImage.egg-info/
+-rw-rw-r--   0 alatas    (1001) alatas    (1001)     2215 2023-04-26 11:22:31.000000 MarkMyImage-0.1.6/MarkMyImage.egg-info/PKG-INFO
+-rw-rw-r--   0 alatas    (1001) alatas    (1001)      254 2023-04-26 11:22:31.000000 MarkMyImage-0.1.6/MarkMyImage.egg-info/SOURCES.txt
+-rw-rw-r--   0 alatas    (1001) alatas    (1001)        1 2023-04-26 11:22:31.000000 MarkMyImage-0.1.6/MarkMyImage.egg-info/dependency_links.txt
+-rw-rw-r--   0 alatas    (1001) alatas    (1001)       41 2023-04-26 11:22:31.000000 MarkMyImage-0.1.6/MarkMyImage.egg-info/entry_points.txt
+-rw-rw-r--   0 alatas    (1001) alatas    (1001)        7 2023-04-26 11:22:31.000000 MarkMyImage-0.1.6/MarkMyImage.egg-info/requires.txt
+-rw-rw-r--   0 alatas    (1001) alatas    (1001)       12 2023-04-26 11:22:31.000000 MarkMyImage-0.1.6/MarkMyImage.egg-info/top_level.txt
+-rw-rw-r--   0 alatas    (1001) alatas    (1001)     2215 2023-04-26 11:22:31.852615 MarkMyImage-0.1.6/PKG-INFO
+-rw-rw-r--   0 alatas    (1001) alatas    (1001)     1602 2023-04-26 09:00:08.000000 MarkMyImage-0.1.6/README.md
+-rw-rw-r--   0 alatas    (1001) alatas    (1001)       38 2023-04-26 11:22:31.852615 MarkMyImage-0.1.6/setup.cfg
+-rw-rw-r--   0 alatas    (1001) alatas    (1001)     1003 2023-04-26 11:22:26.000000 MarkMyImage-0.1.6/setup.py
```

### Comparing `MarkMyImage-0.1.5/MarkMyImage/__init__.py` & `MarkMyImage-0.1.6/MarkMyImage/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,17 @@
         new_size = (int(watermark.width * ratio), int(watermark.height * ratio))
         resized_watermark = watermark.resize(new_size, Image.ANTIALIAS)
 
         # Rotate the logo
         rotated_watermark = resized_watermark.rotate(rotation_angle, expand=True, resample=Image.BICUBIC)
 
         x, y = position
+        if x == 0 and y == 0:
+            x = (img.width - rotated_watermark.width) // 2
+            y = (img.height - rotated_watermark.height) // 2
         img.paste(rotated_watermark, (x, y, x + rotated_watermark.width, y + rotated_watermark.height), rotated_watermark)
         img.save(os.path.join(output_folder, item))
         logging.info(f'Saved watermarked image to: {os.path.join(output_folder, item)}')
 
 def main():
     parser = argparse.ArgumentParser(description="Add a watermark to all images in a folder.")
     parser.add_argument("input_folder", help="Path to the input image folder.")
```

### Comparing `MarkMyImage-0.1.5/MarkMyImage.egg-info/PKG-INFO` & `MarkMyImage-0.1.6/MarkMyImage.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MarkMyImage
-Version: 0.1.5
+Version: 0.1.6
 Summary: Add a watermark to all images in a folder.
 Author: Lomezno
 Author-email: dbwspain@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `MarkMyImage-0.1.5/PKG-INFO` & `MarkMyImage-0.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MarkMyImage
-Version: 0.1.5
+Version: 0.1.6
 Summary: Add a watermark to all images in a folder.
 Author: Lomezno
 Author-email: dbwspain@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `MarkMyImage-0.1.5/README.md` & `MarkMyImage-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `MarkMyImage-0.1.5/setup.py` & `MarkMyImage-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="MarkMyImage",
-    version="0.1.5",
+    version="0.1.6",
     description="Add a watermark to all images in a folder.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Lomezno",
     author_email="dbwspain@gmail.com",
     packages=find_packages(),
     install_requires=["Pillow"],
```

