# Comparing `tmp/pixivSpiderCreatedByHanXu-0.0.5.tar.gz` & `tmp/pixivSpiderCreatedByHanXu-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixivSpiderCreatedByHanXu-0.0.5.tar", last modified: Wed Apr 26 05:21:31 2023, max compression
+gzip compressed data, was "pixivSpiderCreatedByHanXu-0.0.6.tar", last modified: Wed Apr 26 10:28:32 2023, max compression
```

## Comparing `pixivSpiderCreatedByHanXu-0.0.5.tar` & `pixivSpiderCreatedByHanXu-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 05:21:31.018286 pixivSpiderCreatedByHanXu-0.0.5/
--rw-rw-rw-   0        0        0     1090 2023-04-26 04:32:32.000000 pixivSpiderCreatedByHanXu-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     2818 2023-04-26 05:21:31.018286 pixivSpiderCreatedByHanXu-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1845 2023-04-26 04:32:32.000000 pixivSpiderCreatedByHanXu-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 05:21:30.994285 pixivSpiderCreatedByHanXu-0.0.5/pixivSpiderCreatedByHanXu/
--rw-rw-rw-   0        0        0    11199 2023-04-26 05:17:54.000000 pixivSpiderCreatedByHanXu-0.0.5/pixivSpiderCreatedByHanXu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 05:21:31.015301 pixivSpiderCreatedByHanXu-0.0.5/pixivSpiderCreatedByHanXu.egg-info/
--rw-rw-rw-   0        0        0     2818 2023-04-26 05:21:30.000000 pixivSpiderCreatedByHanXu-0.0.5/pixivSpiderCreatedByHanXu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2023-04-26 05:21:30.000000 pixivSpiderCreatedByHanXu-0.0.5/pixivSpiderCreatedByHanXu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 05:21:30.000000 pixivSpiderCreatedByHanXu-0.0.5/pixivSpiderCreatedByHanXu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-26 05:21:30.000000 pixivSpiderCreatedByHanXu-0.0.5/pixivSpiderCreatedByHanXu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-04-26 05:21:30.000000 pixivSpiderCreatedByHanXu-0.0.5/pixivSpiderCreatedByHanXu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-26 05:21:31.018286 pixivSpiderCreatedByHanXu-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     4308 2023-04-26 05:21:07.000000 pixivSpiderCreatedByHanXu-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 05:21:31.017285 pixivSpiderCreatedByHanXu-0.0.5/tests/
--rw-rw-rw-   0        0        0      991 2023-04-26 04:58:28.000000 pixivSpiderCreatedByHanXu-0.0.5/tests/test.py
--rw-rw-rw-   0        0        0       83 2023-04-26 05:08:41.000000 pixivSpiderCreatedByHanXu-0.0.5/tests/test2.py
+drwxrwxrwx   0        0        0        0 2023-04-26 10:28:32.374349 pixivSpiderCreatedByHanXu-0.0.6/
+-rw-rw-rw-   0        0        0     1090 2023-04-26 10:08:28.000000 pixivSpiderCreatedByHanXu-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     2818 2023-04-26 10:28:32.374349 pixivSpiderCreatedByHanXu-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1845 2023-04-26 10:08:28.000000 pixivSpiderCreatedByHanXu-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 10:28:32.360945 pixivSpiderCreatedByHanXu-0.0.6/pixivSpiderCreatedByHanXu/
+-rw-rw-rw-   0        0        0    11319 2023-04-26 10:23:15.000000 pixivSpiderCreatedByHanXu-0.0.6/pixivSpiderCreatedByHanXu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 10:28:32.370946 pixivSpiderCreatedByHanXu-0.0.6/pixivSpiderCreatedByHanXu.egg-info/
+-rw-rw-rw-   0        0        0     2818 2023-04-26 10:28:32.000000 pixivSpiderCreatedByHanXu-0.0.6/pixivSpiderCreatedByHanXu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2023-04-26 10:28:32.000000 pixivSpiderCreatedByHanXu-0.0.6/pixivSpiderCreatedByHanXu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 10:28:32.000000 pixivSpiderCreatedByHanXu-0.0.6/pixivSpiderCreatedByHanXu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-26 10:28:32.000000 pixivSpiderCreatedByHanXu-0.0.6/pixivSpiderCreatedByHanXu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-04-26 10:28:32.000000 pixivSpiderCreatedByHanXu-0.0.6/pixivSpiderCreatedByHanXu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 10:28:32.374349 pixivSpiderCreatedByHanXu-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     4308 2023-04-26 10:28:29.000000 pixivSpiderCreatedByHanXu-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 10:28:32.373340 pixivSpiderCreatedByHanXu-0.0.6/tests/
+-rw-rw-rw-   0        0        0      991 2023-04-26 10:08:28.000000 pixivSpiderCreatedByHanXu-0.0.6/tests/test.py
+-rw-rw-rw-   0        0        0       83 2023-04-26 10:08:28.000000 pixivSpiderCreatedByHanXu-0.0.6/tests/test2.py
```

### Comparing `pixivSpiderCreatedByHanXu-0.0.5/LICENSE` & `pixivSpiderCreatedByHanXu-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pixivSpiderCreatedByHanXu-0.0.5/PKG-INFO` & `pixivSpiderCreatedByHanXu-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixivSpiderCreatedByHanXu
-Version: 0.0.5
+Version: 0.0.6
 Summary: This package can crawl the images at pixiv in two ways.
 Home-page: https://gitee.com/UnderTurrets/pixiv-spider
 Author: Han Xu
 Author-email: 736946693@qq.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `pixivSpiderCreatedByHanXu-0.0.5/README.md` & `pixivSpiderCreatedByHanXu-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pixivSpiderCreatedByHanXu-0.0.5/pixivSpiderCreatedByHanXu/__init__.py` & `pixivSpiderCreatedByHanXu-0.0.6/pixivSpiderCreatedByHanXu/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,22 @@
 import urllib.error
 def percentage(a,b,c):
     '''''
     a:已经下载的数据块
     b:数据块的大小
     c:远程文件的大小
    '''
-    per = a * b / c
+    per = 100.0 * a * b / c
     if per > 100 :
         per = 100
-    print ("{:.2%}".format(per),end=" ")
+    print ('%.2f%%' % per,end="~")
+    return
+
+
+
 opener = urllib.request.build_opener()
 opener.addheaders = [('User-Agent','Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36 Edg/112.0.1722.48'),
                      ("referer", "https://www.pixiv.net/"),]
 urllib.request.install_opener(opener)
 
 class pixiv_spider():
     def __init__(self):
@@ -175,17 +179,19 @@
         for img_url in images_urls:
             # 定义一个flag用于判断下载图片是否异常
             flag = True
             image_path=""
             try:
                 image_path = self.path + str(m) + img_url[img_url.rfind("."):]
                 urllib.request.urlretrieve(url=img_url,filename=image_path,reporthook=percentage)
+                print()
+                print("第{}张图片的URL是:\n{}".format(m, img_url))
                 print('**********第' + str(m) + '张图片下载完成********')
                 print("保存于:\n{}".format(image_path))
-                print("第{}张图片的URL是:\n{}".format(m, img_url))
+                print()
                 continue
 
             except urllib.error.HTTPError:
                 if (img_url[-3:] == "jpg"):
                     stable_url_png = img_url[:-3] + "png"
                     del img_url
                     img_url = stable_url_png
@@ -193,17 +199,19 @@
                 elif (img_url[-3:] == "png"):
                     stable_url_jpg = img_url[:-3] + "jpg"
                     del img_url
                     img_url = stable_url_jpg
 
                 image_path = self.path + str(m) + img_url[img_url.rfind("."):]
                 urllib.request.urlretrieve(url=img_url,filename=image_path,reporthook=percentage)
+                print()
+                print("第{}张图片的URL是:\n{}".format(m, img_url))
                 print('**********第' + str(m) + '张图片下载完成********')
                 print("保存于:\n{}".format(image_path))
-                print("第{}张图片的URL是:\n{}".format(m, img_url))
+                print()
                 continue
 
             except BaseException as error:
                 print(error)
                 print("There are some problems with the url:{}".format(img_url))
                 continue
```

### Comparing `pixivSpiderCreatedByHanXu-0.0.5/pixivSpiderCreatedByHanXu.egg-info/PKG-INFO` & `pixivSpiderCreatedByHanXu-0.0.6/pixivSpiderCreatedByHanXu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixivSpiderCreatedByHanXu
-Version: 0.0.5
+Version: 0.0.6
 Summary: This package can crawl the images at pixiv in two ways.
 Home-page: https://gitee.com/UnderTurrets/pixiv-spider
 Author: Han Xu
 Author-email: 736946693@qq.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `pixivSpiderCreatedByHanXu-0.0.5/setup.py` & `pixivSpiderCreatedByHanXu-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
     ],
 
     #如果上传时出现ERROR：The user '' isn't allowed to upload to project ''，换个名字，长一点无所谓，不能跟别人重复
     name="pixivSpiderCreatedByHanXu",
-    version="0.0.5",
+    version="0.0.6",
     author="Han Xu",
     author_email="736946693@qq.com",
     description="This package can crawl the images at pixiv in two ways.",
 
     long_description=long_description,
     #README.md文本的格式，如果希望使用markdown语言就需要下面这句话
     long_description_content_type="text/markdown",
```

### Comparing `pixivSpiderCreatedByHanXu-0.0.5/tests/test.py` & `pixivSpiderCreatedByHanXu-0.0.6/tests/test.py`

 * *Files identical despite different names*

