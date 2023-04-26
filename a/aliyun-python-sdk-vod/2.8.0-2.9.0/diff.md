# Comparing `tmp/aliyun-python-sdk-vod-2.8.0.tar.gz` & `tmp/aliyun-python-sdk-vod-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-vod-2.8.0.tar", last modified: Thu Dec  7 08:09:48 2017, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-vod-2.9.0.tar", last modified: Thu Dec 21 11:03:44 2017, max compression
```

## Comparing `aliyun-python-sdk-vod-2.8.0.tar` & `aliyun-python-sdk-vod-2.9.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 jenkins    (504) jenkins    (503)        0 2017-12-07 08:09:48.000000 aliyun-python-sdk-vod-2.8.0/
-drwxr-xr-x   0 jenkins    (504) jenkins    (503)        0 2017-12-07 08:09:48.000000 aliyun-python-sdk-vod-2.8.0/aliyun_python_sdk_vod.egg-info/
--rw-r--r--   0 jenkins    (504) jenkins    (503)     3456 2017-12-07 08:09:48.000000 aliyun-python-sdk-vod-2.8.0/aliyun_python_sdk_vod.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (504) jenkins    (503)       13 2017-12-07 08:09:48.000000 aliyun-python-sdk-vod-2.8.0/aliyun_python_sdk_vod.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (504) jenkins    (503)        1 2017-12-07 08:09:48.000000 aliyun-python-sdk-vod-2.8.0/aliyun_python_sdk_vod.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1321 2017-12-07 08:09:48.000000 aliyun-python-sdk-vod-2.8.0/aliyun_python_sdk_vod.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (504) jenkins    (503)       30 2017-12-07 08:09:48.000000 aliyun-python-sdk-vod-2.8.0/aliyun_python_sdk_vod.egg-info/requires.txt
--rw-r--r--   0 jenkins    (504) jenkins    (503)     1321 2017-12-07 08:09:48.000000 aliyun-python-sdk-vod-2.8.0/PKG-INFO
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2586 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/setup.py
--rw-r--r--   0 jenkins    (504) jenkins    (503)       38 2017-12-07 08:09:48.000000 aliyun-python-sdk-vod-2.8.0/setup.cfg
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)        0 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/MANIFEST.in
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)      351 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/README.rst
-drwxr-xr-x   0 jenkins    (504) jenkins    (503)        0 2017-12-07 08:09:48.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)       21 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/__init__.py
-drwxr-xr-x   0 jenkins    (504) jenkins    (503)        0 2017-12-07 08:09:48.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)        0 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/__init__.py
-drwxr-xr-x   0 jenkins    (504) jenkins    (503)        0 2017-12-07 08:09:48.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2336 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/SubmitAIJobRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     1882 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/GetVideoInfoRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2198 2017-10-13 04:14:52.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/GetCategoriesRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     1886 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/DeleteCategoryRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2358 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/SubmitAIVideoTerrorismRecogJobRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2106 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/SetEditingProjectMaterialsRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2764 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/SubmitSnapshotJobRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2310 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/SubmitAIVideoCategoryJobRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2556 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/UpdateEditingProjectRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)        0 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/__init__.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2474 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/UpdateVideoInfoRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     1876 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/ListAIJobRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     1992 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/ListAIVideoCategoryJobRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2302 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/SubmitAIVideoSummaryJobRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2384 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/ProduceEditingProjectVideoRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     1708 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/DeleteVideoRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2086 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/GetVideoPlayAuthRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     3190 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/GetPlayInfoRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     1882 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/GetImageInfoRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2554 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/GetVideoPlayInfoRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2064 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/GetEditingProjectMaterialsRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2372 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/CreateUploadImageRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2040 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/ListAIVideoTerrorismRecogJobRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2000 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/ListAIVideoPornRecogJobRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2384 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/AddEditingProjectRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     1890 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/GetMezzanineInfoRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2046 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/UpdateCategoryRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     1968 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/ListAIVideoCoverJobRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     1984 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/ListAIVideoSummaryJobRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2816 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/SearchEditingProjectRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     1976 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/ListAIVideoCensorJobRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2700 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/DescribeCdnDomainLogsRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     1716 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/RefreshUploadVideoRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     1868 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/GetVideoConfigRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2934 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/DescribeDomainFlowDataRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     1922 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/DeleteEditingProjectRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2274 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/GetCDNStatisSumRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     1746 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/GetMessageCallbackRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2268 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/GetOSSStatisRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     1912 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/ListAIASRJobRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     1732 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/CreateOrderRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2294 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/SubmitAIVideoCensorJobRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     1852 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/DeleteStreamRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     1738 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/OpenVodServiceRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2318 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/SubmitAIVideoPornRecogJobRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     3320 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/CreateUploadVideoRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2286 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/SubmitAIVideoCoverJobRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2622 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/GetVideoListRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2230 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/SubmitAIASRJobRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2494 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/SetMessageCallbackRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2932 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/DescribeDomainBpsDataRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2052 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/AddCategoryRequest.py
--rwxr-xr-x   0 jenkins    (504) jenkins    (503)     1910 2017-12-06 14:02:30.000000 aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/GetEditingProjectRequest.py
+drwxr-xr-x   0 jenkins    (504) jenkins    (503)        0 2017-12-21 11:03:44.000000 aliyun-python-sdk-vod-2.9.0/
+drwxr-xr-x   0 jenkins    (504) jenkins    (503)        0 2017-12-21 11:03:44.000000 aliyun-python-sdk-vod-2.9.0/aliyun_python_sdk_vod.egg-info/
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     3464 2017-12-21 11:03:44.000000 aliyun-python-sdk-vod-2.9.0/aliyun_python_sdk_vod.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (504) jenkins    (503)       13 2017-12-21 11:03:44.000000 aliyun-python-sdk-vod-2.9.0/aliyun_python_sdk_vod.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (504) jenkins    (503)        1 2017-12-21 11:03:44.000000 aliyun-python-sdk-vod-2.9.0/aliyun_python_sdk_vod.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1321 2017-12-21 11:03:44.000000 aliyun-python-sdk-vod-2.9.0/aliyun_python_sdk_vod.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (504) jenkins    (503)       30 2017-12-21 11:03:44.000000 aliyun-python-sdk-vod-2.9.0/aliyun_python_sdk_vod.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (504) jenkins    (503)     1321 2017-12-21 11:03:44.000000 aliyun-python-sdk-vod-2.9.0/PKG-INFO
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2586 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/setup.py
+-rw-r--r--   0 jenkins    (504) jenkins    (503)       38 2017-12-21 11:03:44.000000 aliyun-python-sdk-vod-2.9.0/setup.cfg
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)        0 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/MANIFEST.in
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)      351 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/README.rst
+drwxr-xr-x   0 jenkins    (504) jenkins    (503)        0 2017-12-21 11:03:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)       21 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/__init__.py
+drwxr-xr-x   0 jenkins    (504) jenkins    (503)        0 2017-12-21 11:03:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)        0 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/__init__.py
+drwxr-xr-x   0 jenkins    (504) jenkins    (503)        0 2017-12-21 11:03:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2342 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/SubmitAIJobRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     1888 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/GetVideoInfoRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2198 2017-10-13 04:14:52.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/GetCategoriesRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     1708 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/DeleteCategoryRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2364 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/SubmitAIVideoTerrorismRecogJobRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2112 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/SetEditingProjectMaterialsRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2770 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/SubmitSnapshotJobRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2316 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/SubmitAIVideoCategoryJobRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2562 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/UpdateEditingProjectRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)        0 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/__init__.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2480 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/UpdateVideoInfoRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     1882 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/ListAIJobRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     1998 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/ListAIVideoCategoryJobRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2308 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/SubmitAIVideoSummaryJobRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2390 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/ProduceEditingProjectVideoRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     1714 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/DeleteVideoRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2092 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/GetVideoPlayAuthRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     3196 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/GetPlayInfoRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     1888 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/GetImageInfoRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2560 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/GetVideoPlayInfoRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2070 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/GetEditingProjectMaterialsRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2378 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/CreateUploadImageRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2046 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/ListAIVideoTerrorismRecogJobRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2006 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/ListAIVideoPornRecogJobRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2390 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/AddEditingProjectRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     1896 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/GetMezzanineInfoRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     1868 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/UpdateCategoryRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     1974 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/ListAIVideoCoverJobRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     1990 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/ListAIVideoSummaryJobRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2822 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/SearchEditingProjectRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     1982 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/ListAIVideoCensorJobRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2706 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/DescribeCdnDomainLogsRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     1722 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/RefreshUploadVideoRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     1874 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/GetVideoConfigRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2940 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/DescribeDomainFlowDataRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     1928 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/DeleteEditingProjectRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2280 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/GetCDNStatisSumRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     1752 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/GetMessageCallbackRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2274 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/GetOSSStatisRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     1918 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/ListAIASRJobRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2300 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/SubmitAIVideoCensorJobRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     1858 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/DeleteStreamRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     1744 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/OpenVodServiceRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2324 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/SubmitAIVideoPornRecogJobRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     3326 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/CreateUploadVideoRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2292 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/SubmitAIVideoCoverJobRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     3010 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/ListLiveRecordVideoRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2628 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/GetVideoListRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2236 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/SubmitAIASRJobRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2500 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/SetMessageCallbackRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     2938 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/DescribeDomainBpsDataRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     1874 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/AddCategoryRequest.py
+-rwxr-xr-x   0 jenkins    (504) jenkins    (503)     1916 2017-12-21 08:23:44.000000 aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/GetEditingProjectRequest.py
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyun_python_sdk_vod.egg-info/SOURCES.txt` & `aliyun-python-sdk-vod-2.9.0/aliyun_python_sdk_vod.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 aliyun_python_sdk_vod.egg-info/dependency_links.txt
 aliyun_python_sdk_vod.egg-info/requires.txt
 aliyun_python_sdk_vod.egg-info/top_level.txt
 aliyunsdkvod/__init__.py
 aliyunsdkvod/request/__init__.py
 aliyunsdkvod/request/v20170321/AddCategoryRequest.py
 aliyunsdkvod/request/v20170321/AddEditingProjectRequest.py
-aliyunsdkvod/request/v20170321/CreateOrderRequest.py
 aliyunsdkvod/request/v20170321/CreateUploadImageRequest.py
 aliyunsdkvod/request/v20170321/CreateUploadVideoRequest.py
 aliyunsdkvod/request/v20170321/DeleteCategoryRequest.py
 aliyunsdkvod/request/v20170321/DeleteEditingProjectRequest.py
 aliyunsdkvod/request/v20170321/DeleteStreamRequest.py
 aliyunsdkvod/request/v20170321/DeleteVideoRequest.py
 aliyunsdkvod/request/v20170321/DescribeCdnDomainLogsRequest.py
@@ -38,14 +37,15 @@
 aliyunsdkvod/request/v20170321/ListAIJobRequest.py
 aliyunsdkvod/request/v20170321/ListAIVideoCategoryJobRequest.py
 aliyunsdkvod/request/v20170321/ListAIVideoCensorJobRequest.py
 aliyunsdkvod/request/v20170321/ListAIVideoCoverJobRequest.py
 aliyunsdkvod/request/v20170321/ListAIVideoPornRecogJobRequest.py
 aliyunsdkvod/request/v20170321/ListAIVideoSummaryJobRequest.py
 aliyunsdkvod/request/v20170321/ListAIVideoTerrorismRecogJobRequest.py
+aliyunsdkvod/request/v20170321/ListLiveRecordVideoRequest.py
 aliyunsdkvod/request/v20170321/OpenVodServiceRequest.py
 aliyunsdkvod/request/v20170321/ProduceEditingProjectVideoRequest.py
 aliyunsdkvod/request/v20170321/RefreshUploadVideoRequest.py
 aliyunsdkvod/request/v20170321/SearchEditingProjectRequest.py
 aliyunsdkvod/request/v20170321/SetEditingProjectMaterialsRequest.py
 aliyunsdkvod/request/v20170321/SetMessageCallbackRequest.py
 aliyunsdkvod/request/v20170321/SubmitAIASRJobRequest.py
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyun_python_sdk_vod.egg-info/PKG-INFO` & `aliyun-python-sdk-vod-2.9.0/aliyun_python_sdk_vod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-vod
-Version: 2.8.0
+Version: 2.9.0
 Summary: The vod module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: aliyun-python-sdk-vod
         This is the vod module of Aliyun Python SDK.
```

### Comparing `aliyun-python-sdk-vod-2.8.0/PKG-INFO` & `aliyun-python-sdk-vod-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-vod
-Version: 2.8.0
+Version: 2.9.0
 Summary: The vod module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: aliyun-python-sdk-vod
         This is the vod module of Aliyun Python SDK.
```

### Comparing `aliyun-python-sdk-vod-2.8.0/setup.py` & `aliyun-python-sdk-vod-2.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/SubmitAIJobRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/SubmitAIJobRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class SubmitAIJobRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'SubmitAIJob')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'SubmitAIJob','vod')
 
 	def get_UserData(self):
 		return self.get_query_params().get('UserData')
 
 	def set_UserData(self,UserData):
 		self.add_query_param('UserData',UserData)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/GetVideoInfoRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/GetVideoInfoRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class GetVideoInfoRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'GetVideoInfo')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'GetVideoInfo','vod')
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/GetCategoriesRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/GetCategoriesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/DeleteCategoryRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/DeleteCategoryRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class DeleteCategoryRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'DeleteCategory')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'DeleteCategory','vod')
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
 
@@ -37,18 +37,12 @@
 
 	def get_CateId(self):
 		return self.get_query_params().get('CateId')
 
 	def set_CateId(self,CateId):
 		self.add_query_param('CateId',CateId)
 
-	def get_OwnerAccount(self):
-		return self.get_query_params().get('OwnerAccount')
-
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
 	def get_OwnerId(self):
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self,OwnerId):
 		self.add_query_param('OwnerId',OwnerId)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/SubmitAIVideoTerrorismRecogJobRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/SubmitAIVideoTerrorismRecogJobRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class SubmitAIVideoTerrorismRecogJobRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'SubmitAIVideoTerrorismRecogJob')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'SubmitAIVideoTerrorismRecogJob','vod')
 
 	def get_UserData(self):
 		return self.get_query_params().get('UserData')
 
 	def set_UserData(self,UserData):
 		self.add_query_param('UserData',UserData)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/SetEditingProjectMaterialsRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/SetEditingProjectMaterialsRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class SetEditingProjectMaterialsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'SetEditingProjectMaterials')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'SetEditingProjectMaterials','vod')
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/SubmitSnapshotJobRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/SubmitSnapshotJobRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class SubmitSnapshotJobRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'SubmitSnapshotJob')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'SubmitSnapshotJob','vod')
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/SubmitAIVideoCategoryJobRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/SubmitAIVideoCategoryJobRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class SubmitAIVideoCategoryJobRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'SubmitAIVideoCategoryJob')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'SubmitAIVideoCategoryJob','vod')
 
 	def get_AIVideoCategoryConfig(self):
 		return self.get_query_params().get('AIVideoCategoryConfig')
 
 	def set_AIVideoCategoryConfig(self,AIVideoCategoryConfig):
 		self.add_query_param('AIVideoCategoryConfig',AIVideoCategoryConfig)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/UpdateEditingProjectRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/UpdateEditingProjectRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class UpdateEditingProjectRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'UpdateEditingProject')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'UpdateEditingProject','vod')
 
 	def get_CoverURL(self):
 		return self.get_query_params().get('CoverURL')
 
 	def set_CoverURL(self,CoverURL):
 		self.add_query_param('CoverURL',CoverURL)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/UpdateVideoInfoRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/UpdateVideoInfoRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class UpdateVideoInfoRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'UpdateVideoInfo')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'UpdateVideoInfo','vod')
 
 	def get_CoverURL(self):
 		return self.get_query_params().get('CoverURL')
 
 	def set_CoverURL(self,CoverURL):
 		self.add_query_param('CoverURL',CoverURL)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/ListAIJobRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/ListAIJobRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class ListAIJobRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'ListAIJob')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'ListAIJob','vod')
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/ListAIVideoCategoryJobRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/ListAIVideoCategoryJobRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class ListAIVideoCategoryJobRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'ListAIVideoCategoryJob')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'ListAIVideoCategoryJob','vod')
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/SubmitAIVideoSummaryJobRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/SubmitAIVideoSummaryJobRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class SubmitAIVideoSummaryJobRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'SubmitAIVideoSummaryJob')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'SubmitAIVideoSummaryJob','vod')
 
 	def get_UserData(self):
 		return self.get_query_params().get('UserData')
 
 	def set_UserData(self,UserData):
 		self.add_query_param('UserData',UserData)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/ProduceEditingProjectVideoRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/ProduceEditingProjectVideoRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class ProduceEditingProjectVideoRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'ProduceEditingProjectVideo')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'ProduceEditingProjectVideo','vod')
 
 	def get_CoverURL(self):
 		return self.get_query_params().get('CoverURL')
 
 	def set_CoverURL(self,CoverURL):
 		self.add_query_param('CoverURL',CoverURL)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/DeleteVideoRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/DeleteVideoRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class DeleteVideoRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'DeleteVideo')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'DeleteVideo','vod')
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/GetVideoPlayAuthRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/GetVideoPlayAuthRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class GetVideoPlayAuthRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'GetVideoPlayAuth')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'GetVideoPlayAuth','vod')
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/GetPlayInfoRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/GetPlayInfoRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class GetPlayInfoRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'GetPlayInfo')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'GetPlayInfo','vod')
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/GetImageInfoRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/GetImageInfoRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class GetImageInfoRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'GetImageInfo')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'GetImageInfo','vod')
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/GetVideoPlayInfoRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/GetVideoPlayInfoRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class GetVideoPlayInfoRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'GetVideoPlayInfo')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'GetVideoPlayInfo','vod')
 
 	def get_SignVersion(self):
 		return self.get_query_params().get('SignVersion')
 
 	def set_SignVersion(self,SignVersion):
 		self.add_query_param('SignVersion',SignVersion)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/GetEditingProjectMaterialsRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/GetEditingProjectMaterialsRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class GetEditingProjectMaterialsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'GetEditingProjectMaterials')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'GetEditingProjectMaterials','vod')
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/CreateUploadImageRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/CreateUploadImageRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class CreateUploadImageRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'CreateUploadImage')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'CreateUploadImage','vod')
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/ListAIVideoTerrorismRecogJobRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/ListAIVideoTerrorismRecogJobRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class ListAIVideoTerrorismRecogJobRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'ListAIVideoTerrorismRecogJob')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'ListAIVideoTerrorismRecogJob','vod')
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/ListAIVideoPornRecogJobRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/ListAIVideoPornRecogJobRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class ListAIVideoPornRecogJobRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'ListAIVideoPornRecogJob')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'ListAIVideoPornRecogJob','vod')
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/AddEditingProjectRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/AddEditingProjectRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class AddEditingProjectRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'AddEditingProject')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'AddEditingProject','vod')
 
 	def get_CoverURL(self):
 		return self.get_query_params().get('CoverURL')
 
 	def set_CoverURL(self,CoverURL):
 		self.add_query_param('CoverURL',CoverURL)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/GetMezzanineInfoRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/GetMezzanineInfoRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class GetMezzanineInfoRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'GetMezzanineInfo')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'GetMezzanineInfo','vod')
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/UpdateCategoryRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/UpdateCategoryRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class UpdateCategoryRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'UpdateCategory')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'UpdateCategory','vod')
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
 
@@ -37,20 +37,14 @@
 
 	def get_CateId(self):
 		return self.get_query_params().get('CateId')
 
 	def set_CateId(self,CateId):
 		self.add_query_param('CateId',CateId)
 
-	def get_OwnerAccount(self):
-		return self.get_query_params().get('OwnerAccount')
-
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
 	def get_OwnerId(self):
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self,OwnerId):
 		self.add_query_param('OwnerId',OwnerId)
 
 	def get_CateName(self):
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/ListAIVideoCoverJobRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/ListAIVideoCoverJobRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class ListAIVideoCoverJobRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'ListAIVideoCoverJob')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'ListAIVideoCoverJob','vod')
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/ListAIVideoSummaryJobRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/ListAIVideoSummaryJobRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class ListAIVideoSummaryJobRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'ListAIVideoSummaryJob')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'ListAIVideoSummaryJob','vod')
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/SearchEditingProjectRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/SearchEditingProjectRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class SearchEditingProjectRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'SearchEditingProject')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'SearchEditingProject','vod')
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/ListAIVideoCensorJobRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/ListAIVideoCensorJobRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class ListAIVideoCensorJobRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'ListAIVideoCensorJob')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'ListAIVideoCensorJob','vod')
 
 	def get_AIVideoCensorJobIds(self):
 		return self.get_query_params().get('AIVideoCensorJobIds')
 
 	def set_AIVideoCensorJobIds(self,AIVideoCensorJobIds):
 		self.add_query_param('AIVideoCensorJobIds',AIVideoCensorJobIds)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/DescribeCdnDomainLogsRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/DescribeCdnDomainLogsRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class DescribeCdnDomainLogsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'DescribeCdnDomainLogs')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'DescribeCdnDomainLogs','vod')
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/RefreshUploadVideoRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/RefreshUploadVideoRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class RefreshUploadVideoRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'RefreshUploadVideo')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'RefreshUploadVideo','vod')
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/GetVideoConfigRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/GetVideoConfigRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class GetVideoConfigRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'GetVideoConfig')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'GetVideoConfig','vod')
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/DescribeDomainFlowDataRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/DescribeDomainFlowDataRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class DescribeDomainFlowDataRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'DescribeDomainFlowData')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'DescribeDomainFlowData','vod')
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/DeleteEditingProjectRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/DeleteEditingProjectRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class DeleteEditingProjectRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'DeleteEditingProject')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'DeleteEditingProject','vod')
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/GetCDNStatisSumRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/GetCDNStatisSumRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class GetCDNStatisSumRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'GetCDNStatisSum')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'GetCDNStatisSum','vod')
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/GetMessageCallbackRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/GetMessageCallbackRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class GetMessageCallbackRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'GetMessageCallback')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'GetMessageCallback','vod')
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/GetOSSStatisRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/GetOSSStatisRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class GetOSSStatisRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'GetOSSStatis')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'GetOSSStatis','vod')
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/ListAIASRJobRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/ListAIASRJobRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class ListAIASRJobRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'ListAIASRJob')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'ListAIASRJob','vod')
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/CreateOrderRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/AddCategoryRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,35 +14,41 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
-class CreateOrderRequest(RpcRequest):
+class AddCategoryRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'CreateOrder')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'AddCategory','vod')
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
 
 	def get_ResourceOwnerAccount(self):
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
 		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
 
-	def get_OwnerAccount(self):
-		return self.get_query_params().get('OwnerAccount')
-
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
 	def get_OwnerId(self):
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
+		self.add_query_param('OwnerId',OwnerId)
+
+	def get_ParentId(self):
+		return self.get_query_params().get('ParentId')
+
+	def set_ParentId(self,ParentId):
+		self.add_query_param('ParentId',ParentId)
+
+	def get_CateName(self):
+		return self.get_query_params().get('CateName')
+
+	def set_CateName(self,CateName):
+		self.add_query_param('CateName',CateName)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/SubmitAIVideoCensorJobRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/SubmitAIVideoCensorJobRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class SubmitAIVideoCensorJobRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'SubmitAIVideoCensorJob')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'SubmitAIVideoCensorJob','vod')
 
 	def get_UserData(self):
 		return self.get_query_params().get('UserData')
 
 	def set_UserData(self,UserData):
 		self.add_query_param('UserData',UserData)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/DeleteStreamRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/DeleteStreamRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class DeleteStreamRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'DeleteStream')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'DeleteStream','vod')
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/OpenVodServiceRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/OpenVodServiceRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class OpenVodServiceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'OpenVodService')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'OpenVodService','vod')
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/SubmitAIVideoPornRecogJobRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/SubmitAIVideoPornRecogJobRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class SubmitAIVideoPornRecogJobRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'SubmitAIVideoPornRecogJob')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'SubmitAIVideoPornRecogJob','vod')
 
 	def get_UserData(self):
 		return self.get_query_params().get('UserData')
 
 	def set_UserData(self,UserData):
 		self.add_query_param('UserData',UserData)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/CreateUploadVideoRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/CreateUploadVideoRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class CreateUploadVideoRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'CreateUploadVideo')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'CreateUploadVideo','vod')
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/SubmitAIVideoCoverJobRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/SubmitAIVideoCoverJobRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class SubmitAIVideoCoverJobRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'SubmitAIVideoCoverJob')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'SubmitAIVideoCoverJob','vod')
 
 	def get_UserData(self):
 		return self.get_query_params().get('UserData')
 
 	def set_UserData(self,UserData):
 		self.add_query_param('UserData',UserData)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/GetVideoListRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/GetVideoListRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class GetVideoListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'GetVideoList')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'GetVideoList','vod')
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/SubmitAIASRJobRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/SubmitAIASRJobRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class SubmitAIASRJobRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'SubmitAIASRJob')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'SubmitAIASRJob','vod')
 
 	def get_UserData(self):
 		return self.get_query_params().get('UserData')
 
 	def set_UserData(self,UserData):
 		self.add_query_param('UserData',UserData)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/SetMessageCallbackRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/SetMessageCallbackRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class SetMessageCallbackRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'SetMessageCallback')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'SetMessageCallback','vod')
 
 	def get_CallbackType(self):
 		return self.get_query_params().get('CallbackType')
 
 	def set_CallbackType(self,CallbackType):
 		self.add_query_param('CallbackType',CallbackType)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/DescribeDomainBpsDataRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/DescribeDomainBpsDataRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 class DescribeDomainBpsDataRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'DescribeDomainBpsData')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'DescribeDomainBpsData','vod')
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
```

### Comparing `aliyun-python-sdk-vod-2.8.0/aliyunsdkvod/request/v20170321/AddCategoryRequest.py` & `aliyun-python-sdk-vod-2.9.0/aliyunsdkvod/request/v20170321/GetEditingProjectRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
-class AddCategoryRequest(RpcRequest):
+class GetEditingProjectRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'vod', '2017-03-21', 'AddCategory')
+		RpcRequest.__init__(self, 'vod', '2017-03-21', 'GetEditingProject','vod')
 
 	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self,ResourceOwnerId):
 		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
 
@@ -43,18 +43,12 @@
 
 	def get_OwnerId(self):
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self,OwnerId):
 		self.add_query_param('OwnerId',OwnerId)
 
-	def get_ParentId(self):
-		return self.get_query_params().get('ParentId')
+	def get_ProjectId(self):
+		return self.get_query_params().get('ProjectId')
 
-	def set_ParentId(self,ParentId):
-		self.add_query_param('ParentId',ParentId)
-
-	def get_CateName(self):
-		return self.get_query_params().get('CateName')
-
-	def set_CateName(self,CateName):
-		self.add_query_param('CateName',CateName)
+	def set_ProjectId(self,ProjectId):
+		self.add_query_param('ProjectId',ProjectId)
```

