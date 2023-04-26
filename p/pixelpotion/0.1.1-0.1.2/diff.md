# Comparing `tmp/pixelpotion-0.1.1.tar.gz` & `tmp/pixelpotion-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\git\pixel-potion\dist\.tmp-2bxmq28o\pixelpotion-0.1.1.tar", last modified: Wed Apr 26 09:19:24 2023, max compression
+gzip compressed data, was "D:\git\pixel-potion\dist\.tmp-xvmpfbbo\pixelpotion-0.1.2.tar", last modified: Wed Apr 26 09:47:46 2023, max compression
```

## Comparing `pixelpotion-0.1.1.tar` & `pixelpotion-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 09:19:24.270456 pixelpotion-0.1.1/
--rw-rw-rw-   0        0        0     2241 2023-04-26 09:19:24.269481 pixelpotion-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1523 2023-04-26 03:30:45.000000 pixelpotion-0.1.1/README.md
--rw-rw-rw-   0        0        0     1608 2023-04-26 09:05:56.000000 pixelpotion-0.1.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-26 09:19:24.247032 pixelpotion-0.1.1/pixelpotion/
--rw-rw-rw-   0        0        0        0 2023-04-25 08:39:56.000000 pixelpotion-0.1.1/pixelpotion/__init__.py
--rw-rw-rw-   0        0        0     2255 2023-04-26 03:34:31.000000 pixelpotion-0.1.1/pixelpotion/cli.py
--rw-rw-rw-   0        0        0     1707 2023-04-26 08:34:43.000000 pixelpotion-0.1.1/pixelpotion/convert.py
--rw-rw-rw-   0        0        0      733 2023-04-26 08:34:56.000000 pixelpotion-0.1.1/pixelpotion/split_frames.py
--rw-rw-rw-   0        0        0        0 2023-04-25 08:40:29.000000 pixelpotion-0.1.1/pixelpotion/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-26 09:19:24.264600 pixelpotion-0.1.1/pixelpotion.egg-info/
--rw-rw-rw-   0        0        0     2241 2023-04-26 09:19:24.000000 pixelpotion-0.1.1/pixelpotion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      420 2023-04-26 09:19:24.000000 pixelpotion-0.1.1/pixelpotion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 09:19:24.000000 pixelpotion-0.1.1/pixelpotion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-04-26 09:19:24.000000 pixelpotion-0.1.1/pixelpotion.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-04-26 09:19:24.000000 pixelpotion-0.1.1/pixelpotion.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-26 09:19:24.000000 pixelpotion-0.1.1/pixelpotion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-26 09:19:24.270456 pixelpotion-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      935 2023-04-26 09:16:28.000000 pixelpotion-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 09:19:24.268503 pixelpotion-0.1.1/tests/
--rw-rw-rw-   0        0        0        0 2023-04-26 03:38:00.000000 pixelpotion-0.1.1/tests/__init__.py
--rw-rw-rw-   0        0        0     2354 2023-04-26 08:22:42.000000 pixelpotion-0.1.1/tests/test_convert.py
--rw-rw-rw-   0        0        0     1862 2023-04-26 07:46:40.000000 pixelpotion-0.1.1/tests/test_gif_split.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:47:46.141850 pixelpotion-0.1.2/
+-rw-rw-rw-   0        0        0     2647 2023-04-26 09:47:46.140874 pixelpotion-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1805 2023-04-26 09:45:35.000000 pixelpotion-0.1.2/README.md
+-rw-rw-rw-   0        0        0     1988 2023-04-26 09:47:00.000000 pixelpotion-0.1.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-26 09:47:46.115501 pixelpotion-0.1.2/pixelpotion/
+-rw-rw-rw-   0        0        0        0 2023-04-25 08:39:56.000000 pixelpotion-0.1.2/pixelpotion/__init__.py
+-rw-rw-rw-   0        0        0     2255 2023-04-26 03:34:31.000000 pixelpotion-0.1.2/pixelpotion/cli.py
+-rw-rw-rw-   0        0        0     1707 2023-04-26 08:34:43.000000 pixelpotion-0.1.2/pixelpotion/convert.py
+-rw-rw-rw-   0        0        0      733 2023-04-26 08:34:56.000000 pixelpotion-0.1.2/pixelpotion/split_frames.py
+-rw-rw-rw-   0        0        0        0 2023-04-25 08:40:29.000000 pixelpotion-0.1.2/pixelpotion/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:47:46.135994 pixelpotion-0.1.2/pixelpotion.egg-info/
+-rw-rw-rw-   0        0        0     2647 2023-04-26 09:47:46.000000 pixelpotion-0.1.2/pixelpotion.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2023-04-26 09:47:46.000000 pixelpotion-0.1.2/pixelpotion.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 09:47:46.000000 pixelpotion-0.1.2/pixelpotion.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-04-26 09:47:46.000000 pixelpotion-0.1.2/pixelpotion.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-04-26 09:47:46.000000 pixelpotion-0.1.2/pixelpotion.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-26 09:47:46.000000 pixelpotion-0.1.2/pixelpotion.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 09:47:46.141850 pixelpotion-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      935 2023-04-26 09:47:30.000000 pixelpotion-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:47:46.139898 pixelpotion-0.1.2/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-26 03:38:00.000000 pixelpotion-0.1.2/tests/__init__.py
+-rw-rw-rw-   0        0        0     2354 2023-04-26 08:22:42.000000 pixelpotion-0.1.2/tests/test_convert.py
+-rw-rw-rw-   0        0        0     1862 2023-04-26 07:46:40.000000 pixelpotion-0.1.2/tests/test_gif_split.py
```

### Comparing `pixelpotion-0.1.1/PKG-INFO` & `pixelpotion-0.1.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixelpotion
-Version: 0.1.1
+Version: 0.1.2
 Summary: An open-source image processing tool based on the Pillow
 Home-page: https://github.com/mjhxyz/pixelpotion
 Author: Mao
 Author-email: mjhxyz@foxmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -31,32 +31,56 @@
 -  Save processed images to disk
 
 Installation
 ============
 
 PixelPotion can be installed via pip:
 
-TODO
+.. code:: bash
+
+   pip install pixelpotion
 
 Usage
 =====
 
 PixelPotion can be used via the command line interface. Here are some
 examples:
 
+**Original image:** |original|
+
+**Resize to 100x100:**
+
 .. code:: bash
 
    # Resize an image to 400x400 pixels
-   pixelpotion resize input.png output.png --width 400 --height 400
+   pp resize input.png output.png --width 100 --height 100
 
-   # Crop an image to 200x200 pixels
-   pp convert -f tmp/test.png -t png -w 200 -he 100 -q 300 -o tmp/out.png
+.. figure:: https://img.mjhxyz.top/outpu.png
+   :alt: 100x100
+
+   100x100
+
+**Crop to 200x100 JPEG:**
+
+.. code:: bash
+
+   # Crop an image to 200x100 pixels
+   pp convert -f input.png -o outpu.jpg -t jpg --width 200 --height 100
+
+.. figure:: https://img.mjhxyz.top/outpu.jpg
+   :alt: 200x100
+
+   200x100
+
+**Extract first frame of animated GIF:**
+
+.. code:: bash
 
    # Extract the first frame of an animated GIF
-   pp gif split -f C:\Users\mjhxy\Desktop\input.gif -o tmp -p qq
+   pp gif split -f input.gif -o tmp -p frame
 
 For a full list of available commands and options, please refer to the
 Command Line Interface Documentation in the project wiki(TODO).
 
 API
 ---
 
@@ -71,7 +95,9 @@
 contribute, please read the Contributing Guide and submit a pull
 request(TODO).
 
 License
 -------
 
 PixelPotion is licensed under the MIT License.
+
+.. |original| image:: https://img.mjhxyz.top/00008-624526612.png
```

### Comparing `pixelpotion-0.1.1/README.md` & `pixelpotion-0.1.2/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,88 @@
-# PixelPotion
-PixelPotion is a command line tool based on Pillow for easy processing of PNG, JPG, and GIF images. It provides a simple and intuitive interface for performing common image operations such as resizing, cropping, and retrieving GIF frames.
+PixelPotion
+===========
 
-## Features
+PixelPotion is a command line tool based on Pillow for easy processing
+of PNG, JPG, and GIF images. It provides a simple and intuitive
+interface for performing common image operations such as resizing,
+cropping, and retrieving GIF frames.
+
+Features
+--------
+
+-  Supports PNG, JPG, and GIF image formats
+-  ``Resize`` images to a specified width and height
+-  ``Crop`` images to a specified size and position
+-  ``Retrieve`` individual frames from animated GIFs
+-  Save processed images to disk
 
-- Supports PNG, JPG, and GIF image formats
-- `Resize` images to a specified width and height
-- `Crop` images to a specified size and position
-- `Retrieve` individual frames from animated GIFs
-- Save processed images to disk
+Installation
+============
 
-# Installation
 PixelPotion can be installed via pip:
 
-TODO
+.. code:: bash
 
-# Usage
-PixelPotion can be used via the command line interface. Here are some examples:
+   pip install pixelpotion
 
-```bash
-# Resize an image to 400x400 pixels
-pixelpotion resize input.png output.png --width 400 --height 400
+Usage
+=====
 
-# Crop an image to 200x200 pixels
-pp convert -f tmp/test.png -t png -w 200 -he 100 -q 300 -o tmp/out.png
+PixelPotion can be used via the command line interface. Here are some
+examples:
 
-# Extract the first frame of an animated GIF
-pp gif split -f C:\Users\mjhxy\Desktop\input.gif -o tmp -p qq
-```
+**Original image:** |original|
 
-For a full list of available commands and options, please refer to the Command Line Interface Documentation in the project wiki(TODO).
+**Resize to 100x100:**
 
-## API
+.. code:: bash
 
-PixelPotion is built on top of the popular Pillow library and extends its functionality. For more information on the API, please refer to the API Documentation in the project wiki(TODO).
+   # Resize an image to 400x400 pixels
+   pp resize input.png output.png --width 100 --height 100
 
-## Contributing
+.. figure:: https://img.mjhxyz.top/outpu.png
+   :alt: 100x100
 
-Contributions to PixelPotion are always welcome! If you'd like to contribute, please read the Contributing Guide and submit a pull request(TODO).
+   100x100
 
-## License
+**Crop to 200x100 JPEG:**
 
-PixelPotion is licensed under the MIT License.
+.. code:: bash
+
+   # Crop an image to 200x100 pixels
+   pp convert -f input.png -o outpu.jpg -t jpg --width 200 --height 100
+
+.. figure:: https://img.mjhxyz.top/outpu.jpg
+   :alt: 200x100
+
+   200x100
+
+**Extract first frame of animated GIF:**
+
+.. code:: bash
+
+   # Extract the first frame of an animated GIF
+   pp gif split -f input.gif -o tmp -p frame
+
+For a full list of available commands and options, please refer to the
+Command Line Interface Documentation in the project wiki(TODO).
+
+API
+---
+
+PixelPotion is built on top of the popular Pillow library and extends
+its functionality. For more information on the API, please refer to the
+API Documentation in the project wiki(TODO).
+
+Contributing
+------------
+
+Contributions to PixelPotion are always welcome! If you’d like to
+contribute, please read the Contributing Guide and submit a pull
+request(TODO).
+
+License
+-------
+
+PixelPotion is licensed under the MIT License.
+
+.. |original| image:: https://img.mjhxyz.top/00008-624526612.png
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pixelpotion-0.1.1/pixelpotion/cli.py` & `pixelpotion-0.1.2/pixelpotion/cli.py`

 * *Files identical despite different names*

### Comparing `pixelpotion-0.1.1/pixelpotion/convert.py` & `pixelpotion-0.1.2/pixelpotion/convert.py`

 * *Files identical despite different names*

### Comparing `pixelpotion-0.1.1/pixelpotion/split_frames.py` & `pixelpotion-0.1.2/pixelpotion/split_frames.py`

 * *Files identical despite different names*

### Comparing `pixelpotion-0.1.1/pixelpotion.egg-info/PKG-INFO` & `pixelpotion-0.1.2/pixelpotion.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixelpotion
-Version: 0.1.1
+Version: 0.1.2
 Summary: An open-source image processing tool based on the Pillow
 Home-page: https://github.com/mjhxyz/pixelpotion
 Author: Mao
 Author-email: mjhxyz@foxmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -31,32 +31,56 @@
 -  Save processed images to disk
 
 Installation
 ============
 
 PixelPotion can be installed via pip:
 
-TODO
+.. code:: bash
+
+   pip install pixelpotion
 
 Usage
 =====
 
 PixelPotion can be used via the command line interface. Here are some
 examples:
 
+**Original image:** |original|
+
+**Resize to 100x100:**
+
 .. code:: bash
 
    # Resize an image to 400x400 pixels
-   pixelpotion resize input.png output.png --width 400 --height 400
+   pp resize input.png output.png --width 100 --height 100
 
-   # Crop an image to 200x200 pixels
-   pp convert -f tmp/test.png -t png -w 200 -he 100 -q 300 -o tmp/out.png
+.. figure:: https://img.mjhxyz.top/outpu.png
+   :alt: 100x100
+
+   100x100
+
+**Crop to 200x100 JPEG:**
+
+.. code:: bash
+
+   # Crop an image to 200x100 pixels
+   pp convert -f input.png -o outpu.jpg -t jpg --width 200 --height 100
+
+.. figure:: https://img.mjhxyz.top/outpu.jpg
+   :alt: 200x100
+
+   200x100
+
+**Extract first frame of animated GIF:**
+
+.. code:: bash
 
    # Extract the first frame of an animated GIF
-   pp gif split -f C:\Users\mjhxy\Desktop\input.gif -o tmp -p qq
+   pp gif split -f input.gif -o tmp -p frame
 
 For a full list of available commands and options, please refer to the
 Command Line Interface Documentation in the project wiki(TODO).
 
 API
 ---
 
@@ -71,7 +95,9 @@
 contribute, please read the Contributing Guide and submit a pull
 request(TODO).
 
 License
 -------
 
 PixelPotion is licensed under the MIT License.
+
+.. |original| image:: https://img.mjhxyz.top/00008-624526612.png
```

### Comparing `pixelpotion-0.1.1/setup.py` & `pixelpotion-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.rst', 'r') as f:
     long_description = f.read()
 
 setup(
     name="pixelpotion",
-    version="0.1.1",
+    version="0.1.2",
     description="An open-source image processing tool based on the Pillow",
     long_description=long_description,
     author="Mao",
     author_email="mjhxyz@foxmail.com",
     url="https://github.com/mjhxyz/pixelpotion",
     packages=find_packages(),
     classifiers=[
```

### Comparing `pixelpotion-0.1.1/tests/test_convert.py` & `pixelpotion-0.1.2/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `pixelpotion-0.1.1/tests/test_gif_split.py` & `pixelpotion-0.1.2/tests/test_gif_split.py`

 * *Files identical despite different names*

