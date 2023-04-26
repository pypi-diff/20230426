# Comparing `tmp/tusuan-0.0.4.tar.gz` & `tmp/tusuan-0.0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tusuan-0.0.4.tar", last modified: Sun Apr 23 09:24:19 2023, max compression
+gzip compressed data, was "tusuan-0.0.4.1.tar", last modified: Tue Apr 25 16:51:10 2023, max compression
```

## Comparing `tusuan-0.0.4.tar` & `tusuan-0.0.4.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-04-23 09:24:19.484348 tusuan-0.0.4/
--rw-r--r--   0 xiangyang   (501) staff       (20)      172 2022-12-29 07:25:59.000000 tusuan-0.0.4/MANIFEST.in
--rw-r--r--   0 xiangyang   (501) staff       (20)      563 2023-04-23 09:24:19.484232 tusuan-0.0.4/PKG-INFO
--rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-03-29 03:34:53.000000 tusuan-0.0.4/README.md
--rw-r--r--   0 xiangyang   (501) staff       (20)       81 2023-04-23 09:24:18.000000 tusuan-0.0.4/requirements.txt
--rw-r--r--   0 xiangyang   (501) staff       (20)       38 2023-04-23 09:24:19.484399 tusuan-0.0.4/setup.cfg
--rw-r--r--   0 xiangyang   (501) staff       (20)     1587 2023-04-21 17:22:54.000000 tusuan-0.0.4/setup.py
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-04-23 09:24:19.483019 tusuan-0.0.4/tusuan/
--rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-03-29 03:37:06.000000 tusuan-0.0.4/tusuan/__init__.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     1099 2023-03-15 10:31:32.000000 tusuan-0.0.4/tusuan/file_function.py
--rw-r--r--   0 xiangyang   (501) staff       (20)       40 2023-03-29 03:39:48.000000 tusuan-0.0.4/tusuan/hello.py
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-04-23 09:24:19.484088 tusuan-0.0.4/tusuan/image_video_utils/
--rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-03-29 17:21:56.000000 tusuan-0.0.4/tusuan/image_video_utils/__init__.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     2132 2023-04-21 16:34:53.000000 tusuan-0.0.4/tusuan/image_video_utils/cropper.py
--rw-r--r--   0 xiangyang   (501) staff       (20)      819 2023-03-29 17:22:55.000000 tusuan-0.0.4/tusuan/image_video_utils/display.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     1329 2023-04-07 04:48:17.000000 tusuan-0.0.4/tusuan/image_video_utils/image_visual_selector.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     3341 2023-04-21 17:20:22.000000 tusuan-0.0.4/tusuan/image_video_utils/readers.py
--rw-r--r--   0 xiangyang   (501) staff       (20)     1974 2023-04-21 17:19:04.000000 tusuan-0.0.4/tusuan/image_video_utils/writers.py
--rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-04-21 16:44:19.000000 tusuan-0.0.4/tusuan/path_utils.py
-drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-04-23 09:24:19.483493 tusuan-0.0.4/tusuan.egg-info/
--rw-r--r--   0 xiangyang   (501) staff       (20)      563 2023-04-23 09:24:19.000000 tusuan-0.0.4/tusuan.egg-info/PKG-INFO
--rw-r--r--   0 xiangyang   (501) staff       (20)      507 2023-04-23 09:24:19.000000 tusuan-0.0.4/tusuan.egg-info/SOURCES.txt
--rw-r--r--   0 xiangyang   (501) staff       (20)        1 2023-04-23 09:24:19.000000 tusuan-0.0.4/tusuan.egg-info/dependency_links.txt
--rw-r--r--   0 xiangyang   (501) staff       (20)       81 2023-04-23 09:24:19.000000 tusuan-0.0.4/tusuan.egg-info/requires.txt
--rw-r--r--   0 xiangyang   (501) staff       (20)        7 2023-04-23 09:24:19.000000 tusuan-0.0.4/tusuan.egg-info/top_level.txt
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-04-25 16:51:10.759826 tusuan-0.0.4.1/
+-rw-r--r--   0 xiangyang   (501) staff       (20)      172 2022-12-29 07:25:59.000000 tusuan-0.0.4.1/MANIFEST.in
+-rw-r--r--   0 xiangyang   (501) staff       (20)      565 2023-04-25 16:51:10.759698 tusuan-0.0.4.1/PKG-INFO
+-rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-03-29 03:34:53.000000 tusuan-0.0.4.1/README.md
+-rw-r--r--   0 xiangyang   (501) staff       (20)       81 2023-04-25 16:51:10.000000 tusuan-0.0.4.1/requirements.txt
+-rw-r--r--   0 xiangyang   (501) staff       (20)       38 2023-04-25 16:51:10.759870 tusuan-0.0.4.1/setup.cfg
+-rw-r--r--   0 xiangyang   (501) staff       (20)     1634 2023-04-25 16:50:57.000000 tusuan-0.0.4.1/setup.py
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-04-25 16:51:10.758425 tusuan-0.0.4.1/tusuan/
+-rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-03-29 03:37:06.000000 tusuan-0.0.4.1/tusuan/__init__.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     1099 2023-03-15 10:31:32.000000 tusuan-0.0.4.1/tusuan/file_function.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)       40 2023-03-29 03:39:48.000000 tusuan-0.0.4.1/tusuan/hello.py
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-04-25 16:51:10.759539 tusuan-0.0.4.1/tusuan/image_video_utils/
+-rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-03-29 17:21:56.000000 tusuan-0.0.4.1/tusuan/image_video_utils/__init__.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     2132 2023-04-21 16:34:53.000000 tusuan-0.0.4.1/tusuan/image_video_utils/cropper.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)      819 2023-03-29 17:22:55.000000 tusuan-0.0.4.1/tusuan/image_video_utils/display.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     1329 2023-04-07 04:48:17.000000 tusuan-0.0.4.1/tusuan/image_video_utils/image_visual_selector.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     3591 2023-04-25 16:48:57.000000 tusuan-0.0.4.1/tusuan/image_video_utils/readers.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)     2213 2023-04-25 16:49:11.000000 tusuan-0.0.4.1/tusuan/image_video_utils/writers.py
+-rw-r--r--   0 xiangyang   (501) staff       (20)        0 2023-04-21 16:44:19.000000 tusuan-0.0.4.1/tusuan/path_utils.py
+drwxr-xr-x   0 xiangyang   (501) staff       (20)        0 2023-04-25 16:51:10.758903 tusuan-0.0.4.1/tusuan.egg-info/
+-rw-r--r--   0 xiangyang   (501) staff       (20)      565 2023-04-25 16:51:10.000000 tusuan-0.0.4.1/tusuan.egg-info/PKG-INFO
+-rw-r--r--   0 xiangyang   (501) staff       (20)      507 2023-04-25 16:51:10.000000 tusuan-0.0.4.1/tusuan.egg-info/SOURCES.txt
+-rw-r--r--   0 xiangyang   (501) staff       (20)        1 2023-04-25 16:51:10.000000 tusuan-0.0.4.1/tusuan.egg-info/dependency_links.txt
+-rw-r--r--   0 xiangyang   (501) staff       (20)       81 2023-04-25 16:51:10.000000 tusuan-0.0.4.1/tusuan.egg-info/requires.txt
+-rw-r--r--   0 xiangyang   (501) staff       (20)        7 2023-04-25 16:51:10.000000 tusuan-0.0.4.1/tusuan.egg-info/top_level.txt
```

### Comparing `tusuan-0.0.4/PKG-INFO` & `tusuan-0.0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tusuan
-Version: 0.0.4
+Version: 0.0.4.1
 Summary: useful functions.
 Home-page: https://github.com/tusuan
 Author: tusuan
 Author-email: btk@qq.com
 License: MIT
 Keywords: tusuan
 Platform: UNKNOWN
```

### Comparing `tusuan-0.0.4/setup.py` & `tusuan-0.0.4.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from read import read
 from setuptools import setup, find_packages
 
 setup(name='tusuan',  # 包名
       python_requires='>=3.8.0',  # python环境
-      version='0.0.4',  # 包的版本
+      version='0.0.4.1',  # 包的版本
       description="useful functions.",  # 包简介，显示在PyPI上
 
       long_description=read('README.md'),  # 读取的Readme文档内容，一整块字符串
       long_description_content_type="text/markdown",  # 指定包文档格式为markdown
 
       author="tusuan",  # 作者相关信息
       author_email='btk@qq.com',
       url='https://github.com/tusuan',
 
       # 指定包信息，还可以用find_packages()函数  # find_packages(where="./", include=["tusuan*"]),
       # packages=["tusuan",
       #           "tusuan.image_video_utils"],
-      packages=find_packages(where="./", include=["tusuan*"]),
+      packages=find_packages(where=".", include=["tusuan*"]),
       install_requires=read('requirements.txt').splitlines(),  # 指定需要安装的依赖, 需要是一个列表
 
       include_package_data=True,  # 不知道做啥的
       license="MIT",
       keywords=['tusuan'],
       classifiers=[  # 一些网站的分类信息，方便用户检索
           'Intended Audience :: Developers',
@@ -32,8 +32,10 @@
       ])
 
 """
 pipreqs ./ --encoding=utf8 --force --mode no-pin
 python3 setup.py sdist 
 twine upload --repository tusuan@testpypi dist/*
 pip install -i https://test.pypi.org/simple/ -U tusuan
+
+twine upload --repository tusuan@pypi dist/*
 """
```

### Comparing `tusuan-0.0.4/tusuan/file_function.py` & `tusuan-0.0.4.1/tusuan/file_function.py`

 * *Files identical despite different names*

### Comparing `tusuan-0.0.4/tusuan/image_video_utils/cropper.py` & `tusuan-0.0.4.1/tusuan/image_video_utils/cropper.py`

 * *Files identical despite different names*

### Comparing `tusuan-0.0.4/tusuan/image_video_utils/display.py` & `tusuan-0.0.4.1/tusuan/image_video_utils/display.py`

 * *Files identical despite different names*

### Comparing `tusuan-0.0.4/tusuan/image_video_utils/image_visual_selector.py` & `tusuan-0.0.4.1/tusuan/image_video_utils/image_visual_selector.py`

 * *Files identical despite different names*

### Comparing `tusuan-0.0.4/tusuan/image_video_utils/readers.py` & `tusuan-0.0.4.1/tusuan/image_video_utils/readers.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,33 +15,35 @@
     with Image.open(image_path) as img:
         # 获取图像尺寸
         width, height = img.size
 
     return height, width
 
 
-def read_image(image_path, grey: bool = False, to_rgb: bool = False):
+def read_image(image_path, grey: bool = False, resize=None, to_rgb: bool = False):
     """
     读取图像函数
 
     :param image_path: 图像路径
     :param grey: 是否将图像转换为灰度图像，默认为False
+    :param resize: (h, w)，默认为None
     :param to_rgb: 是否将图像转换为RGB格式，默认为True
     :return: 读取到的图像数组
     """
     if grey:
         # 读取灰度图像
         image = cv2.imread(image_path, cv2.IMREAD_GRAYSCALE)
     else:
         # 读取彩色图像
         image = cv2.imread(image_path)
         if to_rgb:
             # 将BGR格式转换为RGB格式
             image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
-
+    if resize:
+        image = cv2.resize(image, resize)
     return image
 
 
 def get_video_info(video_path):
     """
     获取帧速率、帧数、宽度和高度
     :param video_path: 视频文件地址
@@ -63,22 +65,23 @@
     # 释放VideoCapture对象
     cap.release()
 
     # 返回帧数、宽度、高度和帧速率
     return frames_count, fps, height, width
 
 
-def read_video(video_path, stop: int = sys.maxsize, step: int = 1, to_rgb=False):
+def read_video(video_path, stop: int = sys.maxsize, step: int = 1, *, resize=None, to_rgb=False):
     """
     这个函数可以读取视频文件，并返回指定范围内的帧。
 
     :param video_path: 视频文件路径
     :param start: 要读取的起始帧索引（默认为 0）
     :param stop: 要读取的结束帧索引（默认为 sys.maxsize，即读取所有帧）
     :param step: 读取帧的步长（默认为 1）
+    :param resize: (h, w)，默认为None
     :param to_rgb: 是否转化为RGB图像（默认为 False，保持和cv2返回结果一致）
     :return: 读取成功返回一个代表对应帧所组成的numpy数组，读取失败返回None
     """
     cap = cv2.VideoCapture(video_path)
 
     if not cap.isOpened():
         return None
@@ -95,14 +98,16 @@
     for i in range(stop):
         # 只选取其中符合特定步长的帧
         if i % step == 0:
             ret, frame = cap.read()
             if ret:
                 if to_rgb:
                     frame = cv2.cvtColor(frame, cv2.COLOR_BGR2RGB)
+                if resize:
+                    frame = cv2.resize(frame, resize)
                 video.append(frame)
         else:
             ret = cap.grab()
 
         if not ret:
             break
```

### Comparing `tusuan-0.0.4/tusuan/image_video_utils/writers.py` & `tusuan-0.0.4.1/tusuan/image_video_utils/writers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,60 @@
 import cv2
 import einops
 import numpy
 
 
-def write_image(image: numpy.ndarray, filename: str, rgb_to_bgr=False) -> None:
+def write_image(image: numpy.ndarray, filename: str, *, resize=None, rgb_to_bgr=False) -> None:
     """
     将图像写入文件。
     :param image: numpy.array, 输入图像。
     :param filename: str, 输出文件名。
+    :param resize: (h, w)，默认为None
     :param rgb_to_bgr: False
     :return: 默认False。
     """
     if rgb_to_bgr:
         image = cv2.cvtColor(image, cv2.COLOR_RGB2BGR)
+    if resize:
+        image = cv2.resize(image, resize)
     cv2.imwrite(filename, image)
 
     print(filename, "written")
 
 
-def write_video(video: numpy.ndarray, filename: str, fps: int = 30, rgb_to_bgr=False) -> None:
+def write_video(video: numpy.ndarray, filename: str, *, fps: int = 30, resize=None, rgb_to_bgr=False) -> None:
     """
     将cv2读取的维度格式FHWC（frame_count, height, width, channel_count）视频帧写入文件。
     如果缺少channel_count维度，则会repeat补上。
     函数接受一个视频帧、一个输出文件名和一个视频帧率（默认为30帧/秒），
 
     使用OpenCV的VideoWriter函数创建视频写入对象，然后逐帧将视频写入文件。
     最后，释放视频写入对象。注意，为了使写入的视频具有更好的兼容性，我们选择了MP4编码格式。
 
     :param video: numpy.array, 输入视频帧。
     :param filename: str, 输出文件名。
     :param fps: int, 输出视频帧率。
+    :param resize: (h, w)，默认为None
     :param rgb_to_bgr: 默认False。
     :return: None
     """
     video = numpy.array(video, dtype=numpy.uint16)
     if video.ndim == 4:
         frame_count, height, width, channel_count = video.shape
     elif video.ndim == 3:
         video = einops.repeat(video, "f h w -> f h w c", c=3)
         frame_count, height, width, channel_count = video.shape
 
     fourcc = cv2.VideoWriter_fourcc(*"mp4v")  # 定义输出视频编码格式
+
     writer = cv2.VideoWriter(filename, fourcc, fps, (width, height))  # 创建视频写入对象
 
     for frame in video:
         if rgb_to_bgr:
             frame = cv2.cvtColor(frame, cv2.COLOR_RGB2BGR)
+        if resize:
+            frame = cv2.resize(frame, resize)
         writer.write(frame)  # 逐帧写入视频
 
     writer.release()  # 释放视频写入对象
 
     print(filename, "written")
```

### Comparing `tusuan-0.0.4/tusuan.egg-info/PKG-INFO` & `tusuan-0.0.4.1/tusuan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tusuan
-Version: 0.0.4
+Version: 0.0.4.1
 Summary: useful functions.
 Home-page: https://github.com/tusuan
 Author: tusuan
 Author-email: btk@qq.com
 License: MIT
 Keywords: tusuan
 Platform: UNKNOWN
```

