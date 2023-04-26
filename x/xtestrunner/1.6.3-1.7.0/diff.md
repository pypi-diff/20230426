# Comparing `tmp/xtestrunner-1.6.3.tar.gz` & `tmp/xtestrunner-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtestrunner-1.6.3.tar", max compression
+gzip compressed data, was "xtestrunner-1.7.0.tar", max compression
```

## Comparing `xtestrunner-1.6.3.tar` & `xtestrunner-1.7.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11567 2022-03-16 14:28:26.157468 xtestrunner-1.6.3/LICENSE
--rw-r--r--   0        0        0     1160 2023-04-07 16:05:03.752586 xtestrunner-1.6.3/pyproject.toml
--rw-r--r--   0        0        0     2342 2023-03-06 16:55:59.681328 xtestrunner-1.6.3/README.md
--rw-r--r--   0        0        0     2107 2023-04-07 16:00:47.363977 xtestrunner-1.6.3/XTestRunner/__init__.py
--rw-r--r--   0        0        0     4300 2022-11-23 16:26:28.416349 xtestrunner-1.6.3/XTestRunner/_dingtalk.py
--rw-r--r--   0        0        0     3571 2023-04-05 03:32:24.218179 xtestrunner-1.6.3/XTestRunner/_email.py
--rw-r--r--   0        0        0     4944 2022-11-23 16:33:04.007983 xtestrunner-1.6.3/XTestRunner/_feishu.py
--rw-r--r--   0        0        0     4251 2023-03-06 16:55:59.684323 xtestrunner-1.6.3/XTestRunner/_weixin.py
--rw-r--r--   0        0        0      875 2022-04-07 16:13:07.194649 xtestrunner-1.6.3/XTestRunner/config.py
--rw-r--r--   0        0        0        0 2022-03-05 09:43:21.583035 xtestrunner-1.6.3/XTestRunner/html/__init__.py
--rw-r--r--   0        0        0     9995 2023-04-07 15:55:51.680155 xtestrunner-1.6.3/XTestRunner/html/heading-en.html
--rw-r--r--   0        0        0     9998 2022-05-07 13:53:25.628656 xtestrunner-1.6.3/XTestRunner/html/heading-zh-CN.html
--rw-r--r--   0        0        0     4431 2022-04-12 14:37:36.417747 xtestrunner-1.6.3/XTestRunner/html/mail.html
--rw-r--r--   0        0        0      442 2022-04-12 14:45:26.407074 xtestrunner-1.6.3/XTestRunner/html/notice_tmp.md
--rw-r--r--   0        0        0     2549 2023-03-06 16:55:59.685323 xtestrunner-1.6.3/XTestRunner/html/report-en.html
--rw-r--r--   0        0        0     2555 2023-03-06 16:55:59.686323 xtestrunner-1.6.3/XTestRunner/html/report-zh-CN.html
--rw-r--r--   0        0        0     5455 2023-03-11 15:34:52.855357 xtestrunner-1.6.3/XTestRunner/html/stylesheet.html
--rw-r--r--   0        0        0     8300 2023-04-07 15:55:51.682151 xtestrunner-1.6.3/XTestRunner/html/template.html
--rw-r--r--   0        0        0        0 2022-03-11 14:28:55.560239 xtestrunner-1.6.3/XTestRunner/htmlrunner/__init__.py
--rw-r--r--   0        0        0     8914 2023-04-05 03:32:24.219167 xtestrunner-1.6.3/XTestRunner/htmlrunner/result.py
--rw-r--r--   0        0        0    19457 2023-03-11 15:30:19.410914 xtestrunner-1.6.3/XTestRunner/htmlrunner/runner.py
--rw-r--r--   0        0        0      478 2022-03-11 15:11:22.626827 xtestrunner-1.6.3/XTestRunner/version.py
--rw-r--r--   0        0        0        0 2022-03-08 14:19:54.668807 xtestrunner-1.6.3/XTestRunner/xmlrunner/__init__.py
--rw-r--r--   0        0        0    26732 2023-03-11 16:23:55.295699 xtestrunner-1.6.3/XTestRunner/xmlrunner/result.py
--rw-r--r--   0        0        0     5587 2023-03-06 16:55:59.691323 xtestrunner-1.6.3/XTestRunner/xmlrunner/runner.py
--rw-r--r--   0        0        0     3679 1970-01-01 00:00:00.000000 xtestrunner-1.6.3/PKG-INFO
+-rw-r--r--   0        0        0    11567 2022-03-16 14:28:26.157468 xtestrunner-1.7.0/LICENSE
+-rw-r--r--   0        0        0     1160 2023-04-25 16:27:22.800263 xtestrunner-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2342 2023-03-06 16:55:59.681328 xtestrunner-1.7.0/README.md
+-rw-r--r--   0        0        0     2107 2023-04-25 16:25:31.621688 xtestrunner-1.7.0/XTestRunner/__init__.py
+-rw-r--r--   0        0        0     4300 2022-11-23 16:26:28.416349 xtestrunner-1.7.0/XTestRunner/_dingtalk.py
+-rw-r--r--   0        0        0     3571 2023-04-05 03:32:24.218179 xtestrunner-1.7.0/XTestRunner/_email.py
+-rw-r--r--   0        0        0     4944 2022-11-23 16:33:04.007983 xtestrunner-1.7.0/XTestRunner/_feishu.py
+-rw-r--r--   0        0        0     4251 2023-03-06 16:55:59.684323 xtestrunner-1.7.0/XTestRunner/_weixin.py
+-rw-r--r--   0        0        0      875 2022-04-07 16:13:07.194649 xtestrunner-1.7.0/XTestRunner/config.py
+-rw-r--r--   0        0        0        0 2022-03-05 09:43:21.583035 xtestrunner-1.7.0/XTestRunner/html/__init__.py
+-rw-r--r--   0        0        0     8195 2023-04-25 16:05:13.857047 xtestrunner-1.7.0/XTestRunner/html/heading-en.html
+-rw-r--r--   0        0        0     8199 2023-04-25 16:05:13.858021 xtestrunner-1.7.0/XTestRunner/html/heading-zh-CN.html
+-rw-r--r--   0        0        0     3788 2023-04-25 16:05:13.859010 xtestrunner-1.7.0/XTestRunner/html/mail.html
+-rw-r--r--   0        0        0      442 2022-04-12 14:45:26.407074 xtestrunner-1.7.0/XTestRunner/html/notice_tmp.md
+-rw-r--r--   0        0        0     2372 2023-04-25 16:05:13.861021 xtestrunner-1.7.0/XTestRunner/html/report-en.html
+-rw-r--r--   0        0        0     2378 2023-04-25 16:05:13.862033 xtestrunner-1.7.0/XTestRunner/html/report-zh-CN.html
+-rw-r--r--   0        0        0     4761 2023-04-25 16:05:13.863034 xtestrunner-1.7.0/XTestRunner/html/stylesheet.html
+-rw-r--r--   0        0        0     8585 2023-04-25 16:20:11.366324 xtestrunner-1.7.0/XTestRunner/html/template.html
+-rw-r--r--   0        0        0        0 2022-03-11 14:28:55.560239 xtestrunner-1.7.0/XTestRunner/htmlrunner/__init__.py
+-rw-r--r--   0        0        0     8914 2023-04-05 03:32:24.219167 xtestrunner-1.7.0/XTestRunner/htmlrunner/result.py
+-rw-r--r--   0        0        0    19457 2023-03-11 15:30:19.410914 xtestrunner-1.7.0/XTestRunner/htmlrunner/runner.py
+-rw-r--r--   0        0        0      478 2022-03-11 15:11:22.626827 xtestrunner-1.7.0/XTestRunner/version.py
+-rw-r--r--   0        0        0        0 2022-03-08 14:19:54.668807 xtestrunner-1.7.0/XTestRunner/xmlrunner/__init__.py
+-rw-r--r--   0        0        0    26732 2023-03-11 16:23:55.295699 xtestrunner-1.7.0/XTestRunner/xmlrunner/result.py
+-rw-r--r--   0        0        0     5587 2023-03-06 16:55:59.691323 xtestrunner-1.7.0/XTestRunner/xmlrunner/runner.py
+-rw-r--r--   0        0        0     3679 1970-01-01 00:00:00.000000 xtestrunner-1.7.0/PKG-INFO
```

### Comparing `xtestrunner-1.6.3/LICENSE` & `xtestrunner-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.6.3/pyproject.toml` & `xtestrunner-1.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "XTestRunner"
-version = "1.6.3"
+version = "1.7.0"
 description = "Modern style test report based on unittest framework."
 authors = ["bugmaster <fnngj@126.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/seldomQA/XTestRunner/"
 repository = "https://github.com/seldomQA/XTestRunner/"
 classifiers = [
```

### Comparing `xtestrunner-1.6.3/README.md` & `xtestrunner-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.6.3/XTestRunner/__init__.py` & `xtestrunner-1.7.0/XTestRunner/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,10 +38,10 @@
 from ._feishu import FeiShu
 from ._weixin import Weinxin
 from .config import label
 
 
 __author__ = "bugmaster"
 
-__version__ = "1.6.3"
+__version__ = "1.7.0"
 
 __description__ = "Unittest-based HTML test report."
```

### Comparing `xtestrunner-1.6.3/XTestRunner/_dingtalk.py` & `xtestrunner-1.7.0/XTestRunner/_dingtalk.py`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.6.3/XTestRunner/_email.py` & `xtestrunner-1.7.0/XTestRunner/_email.py`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.6.3/XTestRunner/_feishu.py` & `xtestrunner-1.7.0/XTestRunner/_feishu.py`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.6.3/XTestRunner/_weixin.py` & `xtestrunner-1.7.0/XTestRunner/_weixin.py`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.6.3/XTestRunner/config.py` & `xtestrunner-1.7.0/XTestRunner/config.py`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.6.3/XTestRunner/html/heading-en.html` & `xtestrunner-1.7.0/XTestRunner/html/heading-zh-CN.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,169 +1,177 @@
-<nav class="navbar navbar-light position-lg-sticky top-lg-0 d-none d-lg-block overlap-10 flex-none bg-white border-bottom px-0 py-3" id="topbar">
-    <div class="container-fluid">
-        <div class="hstack gap-2">
-            <a href="https://github.com/SeldomQA/XTestRunner">
-                <img src="http://img.itest.info/XTestRunner_logo.jpg" style="height: 2.25rem;">
-            </a>
-        </div>
-        <div class="navbar-user d-none d-sm-block">
-            <div class="hstack gap-3 ms-4">
-                <h3 style="float: right;"> {{ title }} </h3>
-            </div>
-        </div>
+<nav
+  class="navbar navbar-light position-lg-sticky top-lg-0 d-none d-lg-block overlap-10 flex-none bg-white border-bottom px-0 py-3"
+  id="topbar">
+  <div class="container-fluid">
+    <div class="hstack gap-2">
+      <a href="https://github.com/SeldomQA/XTestRunner">
+        <img src="http://img.itest.info/XTestRunner_logo.jpg" style="height: 2.25rem;">
+      </a>
     </div>
+    <div class="navbar-user d-none d-sm-block">
+      <div class="hstack gap-3 ms-4">
+        <h3 style="float: right;"> {{ title }} </h3>
+      </div>
+    </div>
+  </div>
 </nav>
 
 <div id="headContainer" class="container-fluid mm-active">
-    <div class="row">
-        <div class="col-12 col-lg-5 col-xl-4 d-flex" style="float:left">
-            <div class='card flex-fill'>
-                <div class="card-header">
-                    <div class="d-flex align-items-center">
-                        <h5 class="mb-0">Overview</h5>
-                    </div>
-                </div>
-                <div class="card-body py-0 position-relative scrollable-y" style="max-height:300px">
-                    <div class="list-group list-group-flush">
-                        <div class="list-group-item px-0 position-relative hstack flex-wrap head-list">
-                            <div class="flex-1">
-                                <div class="d-flex align-items-center mb-1">Tester</div>
-                                <div class="d-flex align-items-center">
-                                    <div class="text-sm text-muted line-clamp-1 me-auto">{{tester}}</div>
-                                </div>
-                            </div>
-                        </div>
-                        <div class="list-group-item px-0 position-relative hstack flex-wrap head-list">
-                            <div class="flex-1">
-                                <div class="d-flex align-items-center mb-1">Start time - End time</div>
-                                <div class="d-flex align-items-center">
-                                    <div class="text-sm text-muted line-clamp-1 me-auto">{{ start_time }} - {{ end_time }}</div>
-                                </div>
-                            </div>
-                        </div>
-                        <div class="list-group-item px-0 position-relative hstack flex-wrap head-list">
-                            <div class="flex-1">
-                                <div class="d-flex align-items-center mb-1">Duration</div>
-                                <div class="d-flex align-items-center">
-                                    <div class="text-sm text-muted line-clamp-1 me-auto">{{duration}}</div>
-                                </div>
-                            </div>
-                        </div>
-                        <div class="list-group-item px-0 position-relative hstack flex-wrap head-list">
-                            <div class="flex-1">
-                                <div class="d-flex align-items-center mb-1">Status</div>
-                                <div class="d-flex align-items-center">
-                                    <div class="text-sm text-muted line-clamp-1 me-auto">
-                                        <span class="badge badge-pill bg-soft-success text-success me-2">Passed:{{p_number}}</span>
-                                        <span class="badge badge-pill bg-soft-warning text-warning me-2">Failed:{{f_number}}</span>
-                                        <span class="badge badge-pill bg-soft-danger text-danger me-2">Errors:{{e_number}}</span>
-                                        <span class="badge badge-pill bg-soft-secondary text-secondary me-2">Skipped:{{s_number}}</span>
-                                    </div>
-                                </div>
-                            </div>
-                        </div>
-                        <div class="list-group-item px-0 position-relative hstack flex-wrap" style="padding-top: 5px;">
-                            <div class="flex-1">
-                                <div class="d-flex align-items-center mb-1">Description</div>
-                                <div class="d-flex align-items-center">
-                                    <div class="text-sm text-muted me-auto">{{description}}</div>
-                                </div>
-                            </div>
-                        </div>
-                    </div>
+  <div class="row">
+    <!-- Overview data -->
+    <div class="col-12 col-lg-5 col-xl-3 d-flex" style="float:left">
+      <div class='card flex-fill'>
+        <div class="card-header">
+          <div class="d-flex align-items-center">
+            <h5 class="mb-0" id="overview">概述</h5>
+          </div>
+        </div>
+        <div class="card-body py-0 position-relative scrollable-y" style="max-height:300px">
+          <div class="list-group list-group-flush">
+            <div class="list-group-item px-0 position-relative hstack flex-wrap head-list">
+              <div class="flex-1">
+                <div class="d-flex align-items-center mb-1">👨‍🔧 测试人员</div>
+                <div class="d-flex align-items-center">
+                  <div class="text-sm text-muted line-clamp-1 me-auto">{{tester}}</div>
+                </div>
+              </div>
+            </div>
+            <div class="list-group-item px-0 position-relative hstack flex-wrap head-list">
+              <div class="flex-1">
+                <div class="d-flex align-items-center mb-1">🕒 开始时间</div>
+                <div class="d-flex align-items-center">
+                  <div class="text-sm text-muted line-clamp-1 me-auto">{{ start_time }}</div>
+                </div>
+              </div>
+            </div>
+            <div class="list-group-item px-0 position-relative hstack flex-wrap head-list">
+              <div class="flex-1">
+                <div class="d-flex align-items-center mb-1">🕘 结束时间</div>
+                <div class="d-flex align-items-center">
+                  <div class="text-sm text-muted line-clamp-1 me-auto">{{ end_time }}</div>
+                </div>
+              </div>
+            </div>
+            <div class="list-group-item px-0 position-relative hstack flex-wrap head-list">
+              <div class="flex-1">
+                <div class="d-flex align-items-center mb-1">⌛ 运行时长</div>
+                <div class="d-flex align-items-center">
+                  <div class="text-sm text-muted line-clamp-1 me-auto">{{duration}}</div>
+                </div>
+              </div>
+            </div>
+            <div class="list-group-item px-0 position-relative hstack flex-wrap" style="padding-top: 5px;">
+              <div class="flex-1">
+                <div class="d-flex align-items-center mb-1">ℹ️ 描述</div>
+                <div class="d-flex align-items-center">
+                  <div class="text-sm text-muted me-auto">{{description}}</div>
                 </div>
+              </div>
             </div>
+          </div>
         </div>
-
-        <div style="width: 20%">
-            <div class="card" style="height: 45%;">
-                <div class="card-body">
-                    <div class="row">
-                        <div class="col"><span class="h6 font-semibold text-muted text-sm d-block mb-2">Passed</span>
-                            <span class="h3 font-bold mb-0">{{p_number}}</span>
-                        </div>
-                        <div class="col-auto">
-                            <div class="icon icon-shape bg-success text-white text-lg rounded-circle">P</div>
-                        </div>
-                    </div>
-                    <div class="mt-2 mb-0 text-sm">
-                        <span class="badge badge-pill bg-soft-success text-success me-2">{{p_percent}}</span>
-                        <span class="text-nowrap text-xs text-muted">Pass rate</span>
-                    </div>
-                    <div class="d-flex align-items-center">
-                        <div class="progress" style="width:70%; margin-top: 5px;">
-                            <div class="progress-bar bg-success" role="progressbar" aria-valuenow="83" aria-valuemin="0"
-                                aria-valuemax="100" style="width:{{p_percent}}"></div>
-                        </div>
-                    </div>
-                </div>
+      </div>
+    </div>
+    <!-- passed & failed -->
+    <div style="width: 20%">
+      <div class="card" style="height: 45%;">
+        <div class="card-body">
+          <div class="row">
+            <div class="col"><span class="h6 font-semibold text-muted text-sm d-block mb-2">通过</span>
+              <span class="h3 font-bold mb-0" id="p_number">{{p_number}}</span>
+            </div>
+            <div class="col-auto">
+              <div class="icon icon-shape bg-success text-white text-lg rounded-circle">P</div>
+            </div>
+          </div>
+          <div class="mt-2 mb-0 text-sm">
+            <span class="badge badge-pill bg-soft-warning text-success me-2">{{p_percent}}</span>
+            <span class="text-nowrap text-xs text-muted">通过率</span>
+          </div>
+          <div class="d-flex align-items-center">
+            <div class="progress" style="width:70%; margin-top: 5px;">
+              <div class="progress-bar bg-success" role="progressbar" aria-valuenow="83" aria-valuemin="0"
+                aria-valuemax="100" style="width:{{p_percent}}"></div>
             </div>
-            <div class="card" style="height: 45%; top: 10%;">
-                <div class="card-body">
-                    <div class="row">
-                        <div class="col"><span class="h6 font-semibold text-muted text-sm d-block mb-2">Failed</span>
-                            <span class="h3 font-bold mb-0">{{f_number}}</span></div>
-                        <div class="col-auto">
-                            <div class="icon icon-shape bg-warning text-white text-lg rounded-circle">F</div>
-                        </div>
-                    </div>
-                    <div class="mt-2 mb-0 text-sm">
-                        <span class="badge badge-pill bg-soft-warning text-warning me-2">{{f_percent}}</span>
-                        <span class="text-nowrap text-xs text-muted">Failure rate</span>
-                    </div>
-                    <div class="d-flex align-items-center">
-                        <div class="progress" style="width:70%; margin-top: 5px;">
-                            <div class="progress-bar bg-warning" role="progressbar" aria-valuenow="83" aria-valuemin="0"
-                                aria-valuemax="100" style="width:{{f_percent}}"></div>
-                        </div>
-                    </div>
-                </div>
+          </div>
+        </div>
+      </div>
+      <div class="card" style="height: 45%; top: 10%;">
+        <div class="card-body">
+          <div class="row">
+            <div class="col"><span class="h6 font-semibold text-muted text-sm d-block mb-2">失败</span>
+              <span class="h3 font-bold mb-0" id="f_number">{{f_number}}</span>
+            </div>
+            <div class="col-auto">
+              <div class="icon icon-shape bg-warning text-white text-lg rounded-circle">F</div>
+            </div>
+          </div>
+          <div class="mt-2 mb-0 text-sm">
+            <span class="badge badge-pill bg-soft-warning text-warning me-2">{{f_percent}}</span>
+            <span class="text-nowrap text-xs text-muted">失败率</span>
+          </div>
+          <div class="d-flex align-items-center">
+            <div class="progress" style="width:70%; margin-top: 5px;">
+              <div class="progress-bar bg-warning" role="progressbar" aria-valuenow="83" aria-valuemin="0"
+                aria-valuemax="100" style="width:{{f_percent}}"></div>
             </div>
+          </div>
         </div>
-        <div style="width: 20%">
-            <div class="card" style="height: 45%;">
-                <div class="card-body">
-                    <div class="row">
-                        <div class="col"><span class="h6 font-semibold text-muted text-sm d-block mb-2">Errors</span>
-                            <span class="h3 font-bold mb-0">{{e_number}}</span></div>
-                        <div class="col-auto">
-                            <div class="icon icon-shape bg-danger text-white text-lg rounded-circle">E</div>
-                        </div>
-                    </div>
-                    <div class="mt-2 mb-0 text-sm">
-                        <span class="badge badge-pill bg-soft-danger text-danger me-2">{{e_percent}}</span>
-                        <span class="text-nowrap text-xs text-muted">Error rate</span>
-                    </div>
-                    <div class="d-flex align-items-center">
-                        <div class="progress" style="width:70%; margin-top: 5px;">
-                            <div class="progress-bar bg-danger" role="progressbar" aria-valuenow="83" aria-valuemin="0"
-                                aria-valuemax="100" style="width:{{e_percent}}"></div>
-                        </div>
-                    </div>
-                </div>
+      </div>
+    </div>
+    <!-- error & skipped -->
+    <div style="width: 20%">
+      <div class="card" style="height: 45%;">
+        <div class="card-body">
+          <div class="row">
+            <div class="col"><span class="h6 font-semibold text-muted text-sm d-block mb-2">错误</span>
+              <span class="h3 font-bold mb-0" id="e_number">{{e_number}}</span>
+            </div>
+            <div class="col-auto">
+              <div class="icon icon-shape bg-danger text-white text-lg rounded-circle">E</div>
+            </div>
+          </div>
+          <div class="mt-2 mb-0 text-sm">
+            <span class="badge badge-pill bg-soft-danger text-danger me-2">{{e_percent}}</span>
+            <span class="text-nowrap text-xs text-muted">错误率</span>
+          </div>
+          <div class="d-flex align-items-center">
+            <div class="progress" style="width:70%; margin-top: 5px;">
+              <div class="progress-bar bg-danger" role="progressbar" aria-valuenow="83" aria-valuemin="0"
+                aria-valuemax="100" style="width:{{e_percent}}"></div>
             </div>
-            <div class="card" style="height: 45%; top: 10%;">
-                <div class="card-body">
-                    <div class="row">
-                        <div class="col">
-                            <span class="h6 font-semibold text-muted text-sm d-block mb-2">Skipped</span>
-                            <span class="h3 font-bold mb-0">{{s_number}}</span>
-                        </div>
-                        <div class="col-auto">
-                            <div class="icon icon-shape bg-secondary text-white text-lg rounded-circle">S</div>
-                        </div>
-                    </div>
-                    <div class="mt-2 mb-0 text-sm">
-                        <span class="badge badge-pill bg-soft-secondary text-secondary me-2">{{s_percent}}</span>
-                        <span class="text-nowrap text-xs text-muted">Skip rate</span>
-                    </div>
-                    <div class="d-flex align-items-center">
-                        <div class="progress" style="width:70%; margin-top: 5px;">
-                            <div class="progress-bar bg-secondary" role="progressbar" aria-valuenow="83" aria-valuemin="0"
-                                aria-valuemax="100" style="width:{{s_percent}}"></div>
-                        </div>
-                    </div>
-                </div>
+          </div>
+        </div>
+      </div>
+      <div class="card" style="height: 45%; top: 10%;">
+        <div class="card-body">
+          <div class="row">
+            <div class="col">
+              <span class="h6 font-semibold text-muted text-sm d-block mb-2">跳过</span>
+              <span class="h3 font-bold mb-0" id="s_number">{{s_number}}</span>
+            </div>
+            <div class="col-auto">
+              <div class="icon icon-shape bg-secondary text-white text-lg rounded-circle">S</div>
+            </div>
+          </div>
+          <div class="mt-2 mb-0 text-sm">
+            <span class="badge badge-pill bg-soft-secondary text-secondary me-2">{{s_percent}}</span>
+            <span class="text-nowrap text-xs text-muted">跳过率</span>
+          </div>
+          <div class="d-flex align-items-center">
+            <div class="progress" style="width:70%; margin-top: 5px;">
+              <div class="progress-bar bg-secondary" role="progressbar" aria-valuenow="83" aria-valuemin="0"
+                aria-valuemax="100" style="width:{{s_percent}}"></div>
             </div>
+          </div>
+        </div>
+      </div>
+    </div>
+    <!-- history data -->
+    <div class="col-12 col-lg-5 col-xl-4 d-flex" style="float:right">
+      <div class='card flex-fill'>
+        <div id="echartElement" class="apex-charts" data-colors="#42d29d,#44badc" style="height:420px; padding:10px;">
         </div>
+      </div>
     </div>
-</div>
+  </div>
+</div>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,26 +1,25 @@
 [http://img.itest.info/XTestRunner_logo.jpg]
 **** {{ title }} ****
-** Overview **
-Tester
+** æ¦è¿° **
+ð¨âð§ æµè¯äººå
 {{tester}}
-Start time - End time
-{{ start_time }} - {{ end_time }}
-Duration
+ð å¼å§æ¶é´
+{{ start_time }}
+ð ç»ææ¶é´
+{{ end_time }}
+â è¿è¡æ¶é¿
 {{duration}}
-Status
-Passed:{{p_number}} Failed:{{f_number}} Errors:{{e_number}} Skipped:{
-{s_number}}
-Description
+â¹ï¸ æè¿°
 {{description}}
-Passed {{p_number}}
+éè¿ {{p_number}}
 P
-{{p_percent}} Pass rate
-Failed {{f_number}}
+{{p_percent}} éè¿ç
+å¤±è´¥ {{f_number}}
 F
-{{f_percent}} Failure rate
-Errors {{e_number}}
+{{f_percent}} å¤±è´¥ç
+éè¯¯ {{e_number}}
 E
-{{e_percent}} Error rate
-Skipped {{s_number}}
+{{e_percent}} éè¯¯ç
+è·³è¿ {{s_number}}
 S
-{{s_percent}} Skip rate
+{{s_percent}} è·³è¿ç
```

### Comparing `xtestrunner-1.6.3/XTestRunner/html/heading-zh-CN.html` & `xtestrunner-1.7.0/XTestRunner/html/heading-en.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,169 +1,177 @@
-<nav class="navbar navbar-light position-lg-sticky top-lg-0 d-none d-lg-block overlap-10 flex-none bg-white border-bottom px-0 py-3" id="topbar">
-    <div class="container-fluid">
-        <div class="hstack gap-2">
-            <a href="https://github.com/SeldomQA/XTestRunner">
-                <img src="http://img.itest.info/XTestRunner_logo.jpg" style="height: 2.25rem;">
-            </a>
-        </div>
-        <div class="navbar-user d-none d-sm-block">
-            <div class="hstack gap-3 ms-4">
-                <h3 style="float: right;"> {{ title }} </h3>
-            </div>
-        </div>
+<nav
+  class="navbar navbar-light position-lg-sticky top-lg-0 d-none d-lg-block overlap-10 flex-none bg-white border-bottom px-0 py-3"
+  id="topbar">
+  <div class="container-fluid">
+    <div class="hstack gap-2">
+      <a href="https://github.com/SeldomQA/XTestRunner">
+        <img src="http://img.itest.info/XTestRunner_logo.jpg" style="height: 2.25rem;">
+      </a>
     </div>
+    <div class="navbar-user d-none d-sm-block">
+      <div class="hstack gap-3 ms-4">
+        <h3 style="float: right;"> {{ title }} </h3>
+      </div>
+    </div>
+  </div>
 </nav>
 
 <div id="headContainer" class="container-fluid mm-active">
-    <div class="row">
-        <div class="col-12 col-lg-5 col-xl-4 d-flex" style="float:left">
-            <div class='card flex-fill'>
-                <div class="card-header">
-                    <div class="d-flex align-items-center">
-                        <h5 class="mb-0">概述</h5>
-                    </div>
-                </div>
-                <div class="card-body py-0 position-relative scrollable-y" style="max-height:300px">
-                    <div class="list-group list-group-flush">
-                        <div class="list-group-item px-0 position-relative hstack flex-wrap head-list">
-                            <div class="flex-1">
-                                <div class="d-flex align-items-center mb-1">测试人员</div>
-                                <div class="d-flex align-items-center">
-                                    <div class="text-sm text-muted line-clamp-1 me-auto">{{tester}}</div>
-                                </div>
-                            </div>
-                        </div>
-                        <div class="list-group-item px-0 position-relative hstack flex-wrap head-list">
-                            <div class="flex-1">
-                                <div class="d-flex align-items-center mb-1">开始时间 - 结束时间</div>
-                                <div class="d-flex align-items-center">
-                                    <div class="text-sm text-muted line-clamp-1 me-auto">{{ start_time }} - {{ end_time }}</div>
-                                </div>
-                            </div>
-                        </div>
-                        <div class="list-group-item px-0 position-relative hstack flex-wrap head-list">
-                            <div class="flex-1">
-                                <div class="d-flex align-items-center mb-1">运行时长</div>
-                                <div class="d-flex align-items-center">
-                                    <div class="text-sm text-muted line-clamp-1 me-auto">{{duration}}</div>
-                                </div>
-                            </div>
-                        </div>
-                        <div class="list-group-item px-0 position-relative hstack flex-wrap head-list">
-                            <div class="flex-1">
-                                <div class="d-flex align-items-center mb-1">统计</div>
-                                <div class="d-flex align-items-center">
-                                    <div class="text-sm text-muted line-clamp-1 me-auto">
-                                        <span class="badge badge-pill bg-soft-success text-success me-2">通过:{{p_number}}</span>
-                                        <span class="badge badge-pill bg-soft-warning text-warning me-2">失败:{{f_number}}</span>
-                                        <span class="badge badge-pill bg-soft-danger text-danger me-2">错误:{{e_number}}</span>
-                                        <span class="badge badge-pill bg-soft-secondary text-secondary me-2">跳过:{{s_number}}</span>
-                                    </div>
-                                </div>
-                            </div>
-                        </div>
-                        <div class="list-group-item px-0 position-relative hstack flex-wrap" style="padding-top: 5px;">
-                            <div class="flex-1">
-                                <div class="d-flex align-items-center mb-1">描述</div>
-                                <div class="d-flex align-items-center">
-                                    <div class="text-sm text-muted me-auto">{{description}}</div>
-                                </div>
-                            </div>
-                        </div>
-                    </div>
+  <div class="row">
+    <!-- Overview data -->
+    <div class="col-12 col-lg-5 col-xl-3 d-flex" style="float:left">
+      <div class='card flex-fill'>
+        <div class="card-header">
+          <div class="d-flex align-items-center">
+            <h5 class="mb-0" id="overview">Overview</h5>
+          </div>
+        </div>
+        <div class="card-body py-0 position-relative scrollable-y" style="max-height:300px">
+          <div class="list-group list-group-flush">
+            <div class="list-group-item px-0 position-relative hstack flex-wrap head-list">
+              <div class="flex-1">
+                <div class="d-flex align-items-center mb-1">👨‍🔧 Tester</div>
+                <div class="d-flex align-items-center">
+                  <div class="text-sm text-muted line-clamp-1 me-auto">{{tester}}</div>
+                </div>
+              </div>
+            </div>
+            <div class="list-group-item px-0 position-relative hstack flex-wrap head-list">
+              <div class="flex-1">
+                <div class="d-flex align-items-center mb-1">🕒 Start time</div>
+                <div class="d-flex align-items-center">
+                  <div class="text-sm text-muted line-clamp-1 me-auto">{{ start_time }}</div>
+                </div>
+              </div>
+            </div>
+            <div class="list-group-item px-0 position-relative hstack flex-wrap head-list">
+              <div class="flex-1">
+                <div class="d-flex align-items-center mb-1">🕘 End time</div>
+                <div class="d-flex align-items-center">
+                  <div class="text-sm text-muted line-clamp-1 me-auto">{{ end_time }}</div>
+                </div>
+              </div>
+            </div>
+            <div class="list-group-item px-0 position-relative hstack flex-wrap head-list">
+              <div class="flex-1">
+                <div class="d-flex align-items-center mb-1">⌛ Duration</div>
+                <div class="d-flex align-items-center">
+                  <div class="text-sm text-muted line-clamp-1 me-auto">{{duration}}</div>
+                </div>
+              </div>
+            </div>
+            <div class="list-group-item px-0 position-relative hstack flex-wrap" style="padding-top: 5px;">
+              <div class="flex-1">
+                <div class="d-flex align-items-center mb-1">ℹ️ Description</div>
+                <div class="d-flex align-items-center">
+                  <div class="text-sm text-muted me-auto">{{description}}</div>
                 </div>
+              </div>
             </div>
+          </div>
         </div>
-
-        <div style="width: 20%">
-            <div class="card" style="height: 45%;">
-                <div class="card-body">
-                    <div class="row">
-                        <div class="col"><span class="h6 font-semibold text-muted text-sm d-block mb-2">通过</span>
-                            <span class="h3 font-bold mb-0">{{p_number}}</span>
-                        </div>
-                        <div class="col-auto">
-                            <div class="icon icon-shape bg-success text-white text-lg rounded-circle">P</div>
-                        </div>
-                    </div>
-                    <div class="mt-2 mb-0 text-sm">
-                        <span class="badge badge-pill bg-soft-warning text-success me-2">{{p_percent}}</span>
-                        <span class="text-nowrap text-xs text-muted">通过率</span>
-                    </div>
-                    <div class="d-flex align-items-center">
-                        <div class="progress" style="width:70%; margin-top: 5px;">
-                            <div class="progress-bar bg-success" role="progressbar" aria-valuenow="83" aria-valuemin="0"
-                                aria-valuemax="100" style="width:{{p_percent}}"></div>
-                        </div>
-                    </div>
-                </div>
+      </div>
+    </div>
+    <!-- passed & failed -->
+    <div style="width: 20%">
+      <div class="card" style="height: 45%;">
+        <div class="card-body">
+          <div class="row">
+            <div class="col"><span class="h6 font-semibold text-muted text-sm d-block mb-2">Passed</span>
+              <span class="h3 font-bold mb-0" id="p_number">{{p_number}}</span>
+            </div>
+            <div class="col-auto">
+              <div class="icon icon-shape bg-success text-white text-lg rounded-circle">P</div>
+            </div>
+          </div>
+          <div class="mt-2 mb-0 text-sm">
+            <span class="badge badge-pill bg-soft-success text-success me-2">{{p_percent}}</span>
+            <span class="text-nowrap text-xs text-muted">Pass rate</span>
+          </div>
+          <div class="d-flex align-items-center">
+            <div class="progress" style="width:70%; margin-top: 5px;">
+              <div class="progress-bar bg-success" role="progressbar" aria-valuenow="83" aria-valuemin="0"
+                aria-valuemax="100" style="width:{{p_percent}}"></div>
             </div>
-            <div class="card" style="height: 45%; top: 10%;">
-                <div class="card-body">
-                    <div class="row">
-                        <div class="col"><span class="h6 font-semibold text-muted text-sm d-block mb-2">失败</span>
-                            <span class="h3 font-bold mb-0">{{f_number}}</span></div>
-                        <div class="col-auto">
-                            <div class="icon icon-shape bg-warning text-white text-lg rounded-circle">F</div>
-                        </div>
-                    </div>
-                    <div class="mt-2 mb-0 text-sm">
-                        <span class="badge badge-pill bg-soft-warning text-warning me-2">{{f_percent}}</span>
-                        <span class="text-nowrap text-xs text-muted">失败率</span>
-                    </div>
-                    <div class="d-flex align-items-center">
-                        <div class="progress" style="width:70%; margin-top: 5px;">
-                            <div class="progress-bar bg-warning" role="progressbar" aria-valuenow="83" aria-valuemin="0"
-                                aria-valuemax="100" style="width:{{f_percent}}"></div>
-                        </div>
-                    </div>
-                </div>
+          </div>
+        </div>
+      </div>
+      <div class="card" style="height: 45%; top: 10%;">
+        <div class="card-body">
+          <div class="row">
+            <div class="col"><span class="h6 font-semibold text-muted text-sm d-block mb-2">Failed</span>
+              <span class="h3 font-bold mb-0" id="f_number">{{f_number}}</span>
+            </div>
+            <div class="col-auto">
+              <div class="icon icon-shape bg-warning text-white text-lg rounded-circle">F</div>
+            </div>
+          </div>
+          <div class="mt-2 mb-0 text-sm">
+            <span class="badge badge-pill bg-soft-warning text-warning me-2">{{f_percent}}</span>
+            <span class="text-nowrap text-xs text-muted">Failure rate</span>
+          </div>
+          <div class="d-flex align-items-center">
+            <div class="progress" style="width:70%; margin-top: 5px;">
+              <div class="progress-bar bg-warning" role="progressbar" aria-valuenow="83" aria-valuemin="0"
+                aria-valuemax="100" style="width:{{f_percent}}"></div>
             </div>
+          </div>
         </div>
-        <div style="width: 20%">
-            <div class="card" style="height: 45%;">
-                <div class="card-body">
-                    <div class="row">
-                        <div class="col"><span class="h6 font-semibold text-muted text-sm d-block mb-2">错误</span>
-                            <span class="h3 font-bold mb-0">{{e_number}}</span></div>
-                        <div class="col-auto">
-                            <div class="icon icon-shape bg-danger text-white text-lg rounded-circle">E</div>
-                        </div>
-                    </div>
-                    <div class="mt-2 mb-0 text-sm">
-                        <span class="badge badge-pill bg-soft-danger text-danger me-2">{{e_percent}}</span>
-                        <span class="text-nowrap text-xs text-muted">错误率</span>
-                    </div>
-                    <div class="d-flex align-items-center">
-                        <div class="progress" style="width:70%; margin-top: 5px;">
-                            <div class="progress-bar bg-danger" role="progressbar" aria-valuenow="83" aria-valuemin="0"
-                                aria-valuemax="100" style="width:{{e_percent}}"></div>
-                        </div>
-                    </div>
-                </div>
+      </div>
+    </div>
+    <!-- error & skipped -->
+    <div style="width: 20%">
+      <div class="card" style="height: 45%;">
+        <div class="card-body">
+          <div class="row">
+            <div class="col"><span class="h6 font-semibold text-muted text-sm d-block mb-2">Errors</span>
+              <span class="h3 font-bold mb-0" id="e_number">{{e_number}}</span>
+            </div>
+            <div class="col-auto">
+              <div class="icon icon-shape bg-danger text-white text-lg rounded-circle">E</div>
+            </div>
+          </div>
+          <div class="mt-2 mb-0 text-sm">
+            <span class="badge badge-pill bg-soft-danger text-danger me-2">{{e_percent}}</span>
+            <span class="text-nowrap text-xs text-muted">Error rate</span>
+          </div>
+          <div class="d-flex align-items-center">
+            <div class="progress" style="width:70%; margin-top: 5px;">
+              <div class="progress-bar bg-danger" role="progressbar" aria-valuenow="83" aria-valuemin="0"
+                aria-valuemax="100" style="width:{{e_percent}}"></div>
             </div>
-            <div class="card" style="height: 45%; top: 10%;">
-                <div class="card-body">
-                    <div class="row">
-                        <div class="col">
-                            <span class="h6 font-semibold text-muted text-sm d-block mb-2">跳过</span>
-                            <span class="h3 font-bold mb-0">{{s_number}}</span>
-                        </div>
-                        <div class="col-auto">
-                            <div class="icon icon-shape bg-secondary text-white text-lg rounded-circle">S</div>
-                        </div>
-                    </div>
-                    <div class="mt-2 mb-0 text-sm">
-                        <span class="badge badge-pill bg-soft-secondary text-secondary me-2">{{s_percent}}</span>
-                        <span class="text-nowrap text-xs text-muted">跳过率</span>
-                    </div>
-                    <div class="d-flex align-items-center">
-                        <div class="progress" style="width:70%; margin-top: 5px;">
-                            <div class="progress-bar bg-secondary" role="progressbar" aria-valuenow="83" aria-valuemin="0"
-                                aria-valuemax="100" style="width:{{s_percent}}"></div>
-                        </div>
-                    </div>
-                </div>
+          </div>
+        </div>
+      </div>
+      <div class="card" style="height: 45%; top: 10%;">
+        <div class="card-body">
+          <div class="row">
+            <div class="col">
+              <span class="h6 font-semibold text-muted text-sm d-block mb-2">Skipped</span>
+              <span class="h3 font-bold mb-0" id="s_number">{{s_number}}</span>
+            </div>
+            <div class="col-auto">
+              <div class="icon icon-shape bg-secondary text-white text-lg rounded-circle">S</div>
+            </div>
+          </div>
+          <div class="mt-2 mb-0 text-sm">
+            <span class="badge badge-pill bg-soft-secondary text-secondary me-2">{{s_percent}}</span>
+            <span class="text-nowrap text-xs text-muted">Skip rate</span>
+          </div>
+          <div class="d-flex align-items-center">
+            <div class="progress" style="width:70%; margin-top: 5px;">
+              <div class="progress-bar bg-secondary" role="progressbar" aria-valuenow="83" aria-valuemin="0"
+                aria-valuemax="100" style="width:{{s_percent}}"></div>
             </div>
+          </div>
+        </div>
+      </div>
+    </div>
+    <!-- history data -->
+    <div class="col-12 col-lg-5 col-xl-4 d-flex" style="float:right">
+      <div class='card flex-fill'>
+        <div id="echartElement" class="apex-charts" data-colors="#42d29d,#44badc" style="height:420px; padding:10px;">
         </div>
+      </div>
     </div>
-</div>
+  </div>
+</div>
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
 [http://img.itest.info/XTestRunner_logo.jpg]
 **** {{ title }} ****
-** æ¦è¿° **
-æµè¯äººå
+** Overview **
+ð¨âð§ Tester
 {{tester}}
-å¼å§æ¶é´ - ç»ææ¶é´
-{{ start_time }} - {{ end_time }}
-è¿è¡æ¶é¿
+ð Start time
+{{ start_time }}
+ð End time
+{{ end_time }}
+â Duration
 {{duration}}
-ç»è®¡
-éè¿:{{p_number}} å¤±è´¥:{{f_number}} éè¯¯:{{e_number}} è·³è¿:{{s_number}}
-æè¿°
+â¹ï¸ Description
 {{description}}
-éè¿ {{p_number}}
+Passed {{p_number}}
 P
-{{p_percent}} éè¿ç
-å¤±è´¥ {{f_number}}
+{{p_percent}} Pass rate
+Failed {{f_number}}
 F
-{{f_percent}} å¤±è´¥ç
-éè¯¯ {{e_number}}
+{{f_percent}} Failure rate
+Errors {{e_number}}
 E
-{{e_percent}} éè¯¯ç
-è·³è¿ {{s_number}}
+{{e_percent}} Error rate
+Skipped {{s_number}}
 S
-{{s_percent}} è·³è¿ç
+{{s_percent}} Skip rate
```

### Comparing `xtestrunner-1.6.3/XTestRunner/html/mail.html` & `xtestrunner-1.7.0/XTestRunner/html/mail.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,122 +1,121 @@
-<div width="50%" cellpadding="0" cellspacing="0"
-    style="font-family: 'Helvetica Neue',Helvetica,Arial,sans-serif;
+<div width="50%" cellpadding="0" cellspacing="0" style="font-family: 'Helvetica Neue',Helvetica,Arial,sans-serif;
         box-sizing: border-box;
         display: inline-block;
         font-size: 14px;
         overflow: hidden;
         border-radius: 7px;
         margin: 0;
         border: 1px solid #e9e9e9;
         width: 50%;
         background-color: #f5f9fc;">
-        <div style="font-size: 16px;
+  <div style="font-size: 16px;
             vertical-align: top;
             color: #fff;
             background-color: #8957ff;
             padding: 20px;">
-            <span style="margin-top:20px;display:block"> XTestRunner Test Report </span>
-        </div>
-    <div style="margin-top: 30px;
+    <span style="margin-top:20px;display:block"> XTestRunner Test Report </span>
+  </div>
+  <div style="margin-top: 30px;
         margin-left: 20px;
         margin-right: 20px;
         margin-bottom: 30px;">
-        <table width="100%" cellpadding="0" cellspacing="0" style="font-size:14px;margin:0">
-            <tbody>
-            <tr>
-                <td style="padding:0 0 20px; width: 25%;">
-                    标题:
-                </td>
-                <td style="padding:0 0 20px; width: 25%;">
-                    {{ mail_title }}
-                </td>
-                 <td style="padding:0 0 20px; width: 25%;">
-                    测试人员:
-                </td>
-                <td style="padding:0 0 20px; width: 25%;">
-                    {{ mail_tester }}
-                </td>
-            </tr>
-            <tr>
-                <td style="padding:0 0 20px; width: 25%;">
-                    开始时间:
-                </td>
-                <td style="padding:0 0 20px; width: 25%;">
-                    {{ start_time }}
-                </td>
-                 <td style="padding:0 0 20px; width: 25%;">
-                    结束时间:
-                </td>
-                <td style="padding:0 0 20px; width: 25%;">
-                    {{ end_time }}
-                </td>
-            </tr>
-            <tr>
-                <td style="padding:0 0 20px; width: 25%;">
-                    运行时长:
-                </td>
-                <td style="padding:0 0 20px; width: 25%;">
-                    {{ duration }}
-                </td>
-                <td style="padding:0 0 20px; width: 25%;"></td>
-                <td style="padding:0 0 20px; width: 25%;"></td>
-            </tr>
-            <tr>
-                <td style="padding:0 0 20px; width: 25%;">
-                    通过用例:
-                </td>
-                <td style="padding:0 0 20px; width: 25%;">
-                    {{ mail_pass }}
-                </td>
-                <td style="padding:0 0 20px; width: 25%;">
-                    通过率:
-                </td>
-                <td style="padding:0 0 20px; width: 25%;">
-                    {{ pass_rate }}
-                </td>
-            </tr>
-            <tr>
-                <td style="padding:0 0 20px; width: 25%;">
-                    失败用例: 
-                </td>
-                <td style="padding:0 0 20px; width: 25%;">
-                    {{ mail_fail }}
-                </td>
-                <td style="padding:0 0 20px; width: 25%;">
-                    失败率:
-                </td>
-                <td style="padding:0 0 20px; width: 25%;">
-                    {{ failure_rate }}
-                </td>
-            </tr>
-            <tr>
-                <td style="padding:0 0 20px; width: 25%;">
-                    错误用例:
-                </td>
-                <td style="padding:0 0 20px; width: 25%;">
-                    {{ mail_error }}
-                </td>
-                <td style="padding:0 0 20px; width: 25%;">
-                    错误率:
-                </td>
-                <td style="padding:0 0 20px; width: 25%;">
-                    {{ error_rate }}
-                </td>
-            </tr>
-            <tr>
-                <td style="padding:0 0 20px; width: 25%;">
-                    跳过用例: 
-                </td>
-                <td style="padding:0 0 20px; width: 25%;">
-                    {{ mail_skip }}
-                </td>
-                <td style="padding:0 0 20px; width: 25%;">
-                    跳过率:
-                </td>
-                <td style="padding:0 0 20px; width: 25%;">
-                    {{ skip_rate }}
-                </td>
-            </tr>
-            </tbody>
-        </table>
-    </div>
-</div>
+    <table width="100%" cellpadding="0" cellspacing="0" style="font-size:14px;margin:0">
+      <tbody>
+        <tr>
+          <td style="padding:0 0 20px; width: 25%;">
+            标题:
+          </td>
+          <td style="padding:0 0 20px; width: 25%;">
+            {{ mail_title }}
+          </td>
+          <td style="padding:0 0 20px; width: 25%;">
+            测试人员:
+          </td>
+          <td style="padding:0 0 20px; width: 25%;">
+            {{ mail_tester }}
+          </td>
+        </tr>
+        <tr>
+          <td style="padding:0 0 20px; width: 25%;">
+            开始时间:
+          </td>
+          <td style="padding:0 0 20px; width: 25%;">
+            {{ start_time }}
+          </td>
+          <td style="padding:0 0 20px; width: 25%;">
+            结束时间:
+          </td>
+          <td style="padding:0 0 20px; width: 25%;">
+            {{ end_time }}
+          </td>
+        </tr>
+        <tr>
+          <td style="padding:0 0 20px; width: 25%;">
+            运行时长:
+          </td>
+          <td style="padding:0 0 20px; width: 25%;">
+            {{ duration }}
+          </td>
+          <td style="padding:0 0 20px; width: 25%;"></td>
+          <td style="padding:0 0 20px; width: 25%;"></td>
+        </tr>
+        <tr>
+          <td style="padding:0 0 20px; width: 25%;">
+            通过用例:
+          </td>
+          <td style="padding:0 0 20px; width: 25%;">
+            {{ mail_pass }}
+          </td>
+          <td style="padding:0 0 20px; width: 25%;">
+            通过率:
+          </td>
+          <td style="padding:0 0 20px; width: 25%;">
+            {{ pass_rate }}
+          </td>
+        </tr>
+        <tr>
+          <td style="padding:0 0 20px; width: 25%;">
+            失败用例:
+          </td>
+          <td style="padding:0 0 20px; width: 25%;">
+            {{ mail_fail }}
+          </td>
+          <td style="padding:0 0 20px; width: 25%;">
+            失败率:
+          </td>
+          <td style="padding:0 0 20px; width: 25%;">
+            {{ failure_rate }}
+          </td>
+        </tr>
+        <tr>
+          <td style="padding:0 0 20px; width: 25%;">
+            错误用例:
+          </td>
+          <td style="padding:0 0 20px; width: 25%;">
+            {{ mail_error }}
+          </td>
+          <td style="padding:0 0 20px; width: 25%;">
+            错误率:
+          </td>
+          <td style="padding:0 0 20px; width: 25%;">
+            {{ error_rate }}
+          </td>
+        </tr>
+        <tr>
+          <td style="padding:0 0 20px; width: 25%;">
+            跳过用例:
+          </td>
+          <td style="padding:0 0 20px; width: 25%;">
+            {{ mail_skip }}
+          </td>
+          <td style="padding:0 0 20px; width: 25%;">
+            跳过率:
+          </td>
+          <td style="padding:0 0 20px; width: 25%;">
+            {{ skip_rate }}
+          </td>
+        </tr>
+      </tbody>
+    </table>
+  </div>
+</div>
```

### Comparing `xtestrunner-1.6.3/XTestRunner/html/report-en.html` & `xtestrunner-1.7.0/XTestRunner/html/report-en.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,54 @@
-
 <div id="resultContainer" class="card">
-    <div class="card-header border-bottom">
-        <span style="float: left;">
-            <h5 class="mb-0">Result</h5>
-        </span>
-        <span style="float: right;">
-            <a href='javascript:showCase(0, {{ channel }})' class="btn btn-dark btn-sm">Summary</a>
-            <a href='javascript:showCase(1, {{ channel }})' class="btn btn-success btn-sm">Pass</a>
-            <a href='javascript:showCase(2, {{ channel }})' class="btn btn-warning btn-sm">Failed</a>
-            <a href='javascript:showCase(3, {{ channel }})' class="btn btn-danger btn-sm">Error</a>
-            <a href='javascript:showCase(4, {{ channel }})' class="btn btn-secondary btn-sm">Skip</a>
-            <a href='javascript:showCase(5, {{ channel }})' class="btn btn-info btn-sm">All</a>
-        </span>
-    </div>
-    <div class="table-responsive">
-        <table class="table table-hover table-nowrap">
-            <thead class="table-light">
-                <tr>
-                    <th scope="col">Test Group/Test Case</th>
-                    <th scope="col">Description</th>
-                    <th scope="col">Duration</th>
-                    <th scope="col">Count</th>
-                    <th scope="col">Pass</th>
-                    <th scope="col">Fail</th>
-                    <th scope="col">Error</th>
-                    <th scope="col">View</th>
-                    <th scope="col">Screenshots</th>
-                </tr>
-            </thead>
-            <tbody>
-                {{ test_list }}
-            </tbody>
-        </table>
-    </div>
-    <div class="card-footer border-0 py-5">
-        <span class="text-muted text-sm">Cases Total:
-            <button type="button" class="btn btn-sm bg-dark bg-opacity-20 bg-opacity-100-hover text-dark text-white-hover">{{ count }}</button> =
-            <button type="button" class="btn btn-sm bg-success bg-opacity-20 bg-opacity-100-hover text-success text-white-hover">{{ Pass }}</button> +
-            <button type="button" class="btn btn-sm bg-warning bg-opacity-20 bg-opacity-100-hover text-warning text-white-hover">{{ fail }}</button> +
-            <button type="button" class="btn btn-sm bg-danger bg-opacity-20 bg-opacity-100-hover text-danger text-white-hover">{{ error }}</button> +
-            <button type="button" class="btn btn-sm bg-secondary bg-opacity-20 bg-opacity-100-hover text-secondary text-white-hover">{{ skip }}</button>
-        </span>
-    </div>
+  <div class="card-header border-bottom">
+    <span style="float: left;">
+      <h5 class="mb-0">Result</h5>
+    </span>
+    <span style="float: right;">
+      <a href='javascript:showCase(0, {{ channel }})' class="btn btn-dark btn-sm">Summary</a>
+      <a href='javascript:showCase(1, {{ channel }})' class="btn btn-success btn-sm">Pass</a>
+      <a href='javascript:showCase(2, {{ channel }})' class="btn btn-warning btn-sm">Failed</a>
+      <a href='javascript:showCase(3, {{ channel }})' class="btn btn-danger btn-sm">Error</a>
+      <a href='javascript:showCase(4, {{ channel }})' class="btn btn-secondary btn-sm">Skip</a>
+      <a href='javascript:showCase(5, {{ channel }})' class="btn btn-info btn-sm">All</a>
+    </span>
+  </div>
+  <div class="table-responsive">
+    <table class="table table-hover table-nowrap">
+      <thead class="table-light">
+        <tr>
+          <th scope="col">Test Group/Test Case</th>
+          <th scope="col">Description</th>
+          <th scope="col">Duration</th>
+          <th scope="col">Count</th>
+          <th scope="col">Pass</th>
+          <th scope="col">Fail</th>
+          <th scope="col">Error</th>
+          <th scope="col">View</th>
+          <th scope="col">Screenshots</th>
+        </tr>
+      </thead>
+      <tbody>
+        {{ test_list }}
+      </tbody>
+    </table>
+  </div>
+  <div class="card-footer border-0 py-5">
+    <span class="text-muted text-sm">Cases Total:
+      <button type="button" class="btn btn-sm bg-dark bg-opacity-20 bg-opacity-100-hover text-dark text-white-hover">{{
+        count }}</button> =
+      <button type="button"
+        class="btn btn-sm bg-success bg-opacity-20 bg-opacity-100-hover text-success text-white-hover">{{ Pass
+        }}</button> +
+      <button type="button"
+        class="btn btn-sm bg-warning bg-opacity-20 bg-opacity-100-hover text-warning text-white-hover">{{ fail
+        }}</button> +
+      <button type="button"
+        class="btn btn-sm bg-danger bg-opacity-20 bg-opacity-100-hover text-danger text-white-hover">{{ error
+        }}</button> +
+      <button type="button"
+        class="btn btn-sm bg-secondary bg-opacity-20 bg-opacity-100-hover text-secondary text-white-hover">{{ skip
+        }}</button>
+    </span>
+  </div>
 </div>
-<div style="height:120px"></div>
+<div style="height:120px"></div>
```

### Comparing `xtestrunner-1.6.3/XTestRunner/html/report-zh-CN.html` & `xtestrunner-1.7.0/XTestRunner/html/report-zh-CN.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,54 @@
-
 <div id="resultContainer" class="card">
-    <div class="card-header border-bottom">
-        <span style="float: left;">
-            <h5 class="mb-0">结果</h5>
-        </span>
-        <span style="float: right;">
-            <a href='javascript:showCase(0, {{ channel }})' class="btn btn-dark btn-sm">摘要</a>
-            <a href='javascript:showCase(1, {{ channel }})' class="btn btn-success btn-sm">通过</a>
-            <a href='javascript:showCase(2, {{ channel }})' class="btn btn-warning btn-sm">失败</a>
-            <a href='javascript:showCase(3, {{ channel }})' class="btn btn-danger btn-sm">错误</a>
-            <a href='javascript:showCase(4, {{ channel }})' class="btn btn-secondary btn-sm">跳过</a>
-            <a href='javascript:showCase(5, {{ channel }})' class="btn btn-info btn-sm">所有</a>
-        </span>
-    </div>
-    <div class="table-responsive">
-        <table class="table table-hover table-nowrap">
-            <thead class="table-light">
-                <tr>
-                    <th scope="col">测试类/测试用例</th>
-                    <th scope="col">描述</th>
-                    <th scope="col">时长</th>
-                    <th scope="col">执行</th>
-                    <th scope="col">通过</th>
-                    <th scope="col">失败</th>
-                    <th scope="col">错误</th>
-                    <th scope="col">查看</th>
-                    <th scope="col">截图</th>
-                </tr>
-            </thead>
-            <tbody>
-                {{ test_list }}
-            </tbody>
-        </table>
-    </div>
-    <div class="card-footer border-0 py-5">
-        <span class="text-muted text-sm">用例总数:
-            <button type="button" class="btn btn-sm bg-dark bg-opacity-20 bg-opacity-100-hover text-dark text-white-hover">{{ count }}</button> =
-            <button type="button" class="btn btn-sm bg-success bg-opacity-20 bg-opacity-100-hover text-success text-white-hover">{{ Pass }}</button> +
-            <button type="button" class="btn btn-sm bg-warning bg-opacity-20 bg-opacity-100-hover text-warning text-white-hover">{{ fail }}</button> +
-            <button type="button" class="btn btn-sm bg-danger bg-opacity-20 bg-opacity-100-hover text-danger text-white-hover">{{ error }}</button> +
-            <button type="button" class="btn btn-sm bg-secondary bg-opacity-20 bg-opacity-100-hover text-secondary text-white-hover">{{ skip }}</button>
-        </span>
-    </div>
+  <div class="card-header border-bottom">
+    <span style="float: left;">
+      <h5 class="mb-0">结果</h5>
+    </span>
+    <span style="float: right;">
+      <a href='javascript:showCase(0, {{ channel }})' class="btn btn-dark btn-sm">摘要</a>
+      <a href='javascript:showCase(1, {{ channel }})' class="btn btn-success btn-sm">通过</a>
+      <a href='javascript:showCase(2, {{ channel }})' class="btn btn-warning btn-sm">失败</a>
+      <a href='javascript:showCase(3, {{ channel }})' class="btn btn-danger btn-sm">错误</a>
+      <a href='javascript:showCase(4, {{ channel }})' class="btn btn-secondary btn-sm">跳过</a>
+      <a href='javascript:showCase(5, {{ channel }})' class="btn btn-info btn-sm">所有</a>
+    </span>
+  </div>
+  <div class="table-responsive">
+    <table class="table table-hover table-nowrap">
+      <thead class="table-light">
+        <tr>
+          <th scope="col">测试类/测试用例</th>
+          <th scope="col">描述</th>
+          <th scope="col">时长</th>
+          <th scope="col">执行</th>
+          <th scope="col">通过</th>
+          <th scope="col">失败</th>
+          <th scope="col">错误</th>
+          <th scope="col">查看</th>
+          <th scope="col">截图</th>
+        </tr>
+      </thead>
+      <tbody>
+        {{ test_list }}
+      </tbody>
+    </table>
+  </div>
+  <div class="card-footer border-0 py-5">
+    <span class="text-muted text-sm">用例总数:
+      <button type="button" class="btn btn-sm bg-dark bg-opacity-20 bg-opacity-100-hover text-dark text-white-hover">{{
+        count }}</button> =
+      <button type="button"
+        class="btn btn-sm bg-success bg-opacity-20 bg-opacity-100-hover text-success text-white-hover">{{ Pass
+        }}</button> +
+      <button type="button"
+        class="btn btn-sm bg-warning bg-opacity-20 bg-opacity-100-hover text-warning text-white-hover">{{ fail
+        }}</button> +
+      <button type="button"
+        class="btn btn-sm bg-danger bg-opacity-20 bg-opacity-100-hover text-danger text-white-hover">{{ error
+        }}</button> +
+      <button type="button"
+        class="btn btn-sm bg-secondary bg-opacity-20 bg-opacity-100-hover text-secondary text-white-hover">{{ skip
+        }}</button>
+    </span>
+  </div>
 </div>
-<div style="height:120px"></div>
+<div style="height:120px"></div>
```

### Comparing `xtestrunner-1.6.3/XTestRunner/html/stylesheet.html` & `xtestrunner-1.7.0/XTestRunner/html/stylesheet.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,267 +1,265 @@
 <style type="text/css" media="screen">
-    body {
-        font-family: verdana, arial, helvetica, sans-serif;
-        font-size: 80%;
-    }
-
-    table {
-        font-size: 100%;
-    }
-
-    .table td {
-        white-space: inherit !important;
-    }
-
-    /* -- heading ---------------------------------------------------------------------- */
-    h1 {
-        font-size: 16pt;
-        color: gray;
-    }
-
-    pre {
-        background-color: #eef2f7;
-        padding-top: 10px;
-        text-align: left;
-        max-height: 600px;
-        overflow: auto;
-    }
-
-    ::-webkit-scrollbar {
-        width: 6px;
-        height: 6px;
-        background-color: #F5F5F5;
-    }
-
-    ::-webkit-scrollbar-track {
-        -webkit-box-shadow: inset 0 0 6px rgba(0,0,0,0.3);
-        border-radius: 10px;
-        background-color: rgba(114,124,245,.25);
-    }
-
-    ::-webkit-scrollbar-thumb {
-        border-radius: 10px;
-        -webkit-box-shadow: inset 0 0 6px rgba(0,0,0,.3);
-        background-color: #6c757d;
-    }
-
-    .heading {
-        margin-top: 20px;
-        margin-bottom: 1ex;
-        margin-left: 10px;
-        margin-right: 10px;
-        width: 23%;
-        float: left;
-        padding-top: 10px;
-        padding-left: 10px;
-        padding-bottom: 10px;
-        padding-right: 10px;
-        box-shadow: 0px 0px 5px #000;
-    }
-
-    .heading .attribute {
-        margin-top: 1ex;
-        margin-bottom: 0;
-    }
-
-    .heading .description {
-        margin-top: 4ex;
-        margin-bottom: 6ex;
-    }
-
-    /* -- css div popup ------------------------------------------------------------------------ */
-
-    a.popup_link:hover {
-        color: red;
-    }
-
-    .log_window {
-        max-width: 70%;
-        max-height: 70%;
-    }
-
-    /* -- report ------------------------------------------------------------------------ */
-    .show_detail_line {
-        margin-left: 10px;
-        margin-top: 30px;
-        margin-bottom: 20px;
-    }
-
-    .show_detail_button {
-        margin-top: 3ex;
-        margin-bottom: 1ex;
-        margin-left: 10px;
-        text-align: right;
-        margin-right: 15px;
-    }
-
-    .header_row {
-        font-weight: bold;
-        color: #606060;
-        border-top-width: 10px;
-        border-color: #d6e9c6;
-        font-size: 15px;
-    }
-
-    .total_row {
-        font-weight: bold;
-        background-color: #dee2e6;
-    }
-
-    .passClass {
-        background-color: #ccf5e7;
-    }
-
-    .failClass {
-        background-color: #ffe8cc;
-    }
-
-    .errorClass {
-        background-color: #ffd6e0;
-    }
-
-    .skipClass {
-        background-color: #e7eaf0;
-    }
-
-    .passCase {
-        color: #00CC88;
-        font-weight: bold;
-    }
-
-    .failCase {
-        color: #FF8C00;
-        font-weight: bold;
-    }
-
-    .errorCase {
-        color: #FF3366;
-        font-weight: bold;
-    }
-
-    .skipCase {
-        color: #525f7f;
-        font-weight: bold;
-    }
-
-    .hiddenRow {
-        display: none;
-    }
-
-    .caseStatistics {
-        width: 46%
-    }
-
-    .none {
-        color: #009900
-    }
-
-    .testcase {
-        margin-left: 2em;
-    }
-
-    /* -- chars ---------------------------------------------------------------------- */
-    .testChars {
-        width: 900px;
-        margin-left: 0px;
-    }
-
-    .error-color {
-        color: #fff;
-        background-color: #f44455;
-        border-color: #f44455;
-    }
-
-    .pass-color {
-        color: #fff;
-        background-color: #5fc27e;
-        border-color: #5fc27e;
-    }
-
-    .fail-color {
-        color: #fff;
-        background-color: #fcc100;
-        border-color: #fcc100;
-    }
-
-    .skip-color {
-        color: #fff;
-        background-color: #6c757d;
-        border-color: #6c757d;
-    }
-
-    /* -- screenshots ---------------------------------------------------------------------- */
-    .img {
-        border-collapse: collapse;
-        max-width: 100%;
-        max-height: 100%;
-        object-fit: contain;
-        position: absolute;
-        top: 0;
-        left: 0;
-        bottom: 0;
-        right: 0;
-        margin: auto;
-    }
-
-    .img-card {
-        height: 600px;
-        width:800px;
-        background-color: #e7eaf0;
-    }
-
-    .img-circle {
-        height: 20px;
-        border-radius: 12px;
-        background-color: red;
-        padding-left: 13px;
-        margin: 0 auto;
-        position: relative;
-        top: -40px;
-        background-color: rgba(1, 150, 0, 0.3);
-    }
-
-    .img-circle font {
-        border: 1px solid white;
-        width: 11px;
-        height: 11px;
-        border-radius: 50%;
-        margin-right: 9px;
-        margin-top: 4px;
-        display: block;
-        float: left;
-        background-color: white;
-    }
-
-    .close-shots {
-        position: absolute;
-        top: 5px;
-        right: 5px;
-        z-index: 99;
-    }
-
-    .footer {
-        height: 50px;
-        width: 100%;
-        position: fixed;
-        bottom: 0;
-    }
-
-    #headContainer {
-        margin-top: 20px;
-        margin-bottom: 20px;
-        padding-left: 30px;
-        padding-right: 30px;
-    }
-
-    .head-list {
-        padding-top: 5px;
-        padding-bottom: 5px;
-    }
-
-    #resultContainer {
-        margin-left: 30px;
-        margin-right: 30px;
-    }
-
-
-</style>
+  body {
+    font-family: verdana, arial, helvetica, sans-serif;
+    font-size: 80%;
+  }
+
+  table {
+    font-size: 100%;
+  }
+
+  .table td {
+    white-space: inherit !important;
+  }
+
+  /* -- heading ---------------------------------------------------------------------- */
+  h1 {
+    font-size: 16pt;
+    color: gray;
+  }
+
+  pre {
+    background-color: #eef2f7;
+    padding-top: 10px;
+    text-align: left;
+    max-height: 600px;
+    overflow: auto;
+  }
+
+  ::-webkit-scrollbar {
+    width: 6px;
+    height: 6px;
+    background-color: #F5F5F5;
+  }
+
+  ::-webkit-scrollbar-track {
+    -webkit-box-shadow: inset 0 0 6px rgba(0, 0, 0, 0.3);
+    border-radius: 10px;
+    background-color: rgba(114, 124, 245, .25);
+  }
+
+  ::-webkit-scrollbar-thumb {
+    border-radius: 10px;
+    -webkit-box-shadow: inset 0 0 6px rgba(0, 0, 0, .3);
+    background-color: #6c757d;
+  }
+
+  .heading {
+    margin-top: 20px;
+    margin-bottom: 1ex;
+    margin-left: 10px;
+    margin-right: 10px;
+    width: 23%;
+    float: left;
+    padding-top: 10px;
+    padding-left: 10px;
+    padding-bottom: 10px;
+    padding-right: 10px;
+    box-shadow: 0px 0px 5px #000;
+  }
+
+  .heading .attribute {
+    margin-top: 1ex;
+    margin-bottom: 0;
+  }
+
+  .heading .description {
+    margin-top: 4ex;
+    margin-bottom: 6ex;
+  }
+
+  /* -- css div popup ------------------------------------------------------------------------ */
+
+  a.popup_link:hover {
+    color: red;
+  }
+
+  .log_window {
+    max-width: 70%;
+    max-height: 70%;
+  }
+
+  /* -- report ------------------------------------------------------------------------ */
+  .show_detail_line {
+    margin-left: 10px;
+    margin-top: 30px;
+    margin-bottom: 20px;
+  }
+
+  .show_detail_button {
+    margin-top: 3ex;
+    margin-bottom: 1ex;
+    margin-left: 10px;
+    text-align: right;
+    margin-right: 15px;
+  }
+
+  .header_row {
+    font-weight: bold;
+    color: #606060;
+    border-top-width: 10px;
+    border-color: #d6e9c6;
+    font-size: 15px;
+  }
+
+  .total_row {
+    font-weight: bold;
+    background-color: #dee2e6;
+  }
+
+  .passClass {
+    background-color: #ccf5e7;
+  }
+
+  .failClass {
+    background-color: #ffe8cc;
+  }
+
+  .errorClass {
+    background-color: #ffd6e0;
+  }
+
+  .skipClass {
+    background-color: #e7eaf0;
+  }
+
+  .passCase {
+    color: #00CC88;
+    font-weight: bold;
+  }
+
+  .failCase {
+    color: #FF8C00;
+    font-weight: bold;
+  }
+
+  .errorCase {
+    color: #FF3366;
+    font-weight: bold;
+  }
+
+  .skipCase {
+    color: #525f7f;
+    font-weight: bold;
+  }
+
+  .hiddenRow {
+    display: none;
+  }
+
+  .caseStatistics {
+    width: 46%
+  }
+
+  .none {
+    color: #009900
+  }
+
+  .testcase {
+    margin-left: 2em;
+  }
+
+  /* -- chars ---------------------------------------------------------------------- */
+  .testChars {
+    width: 900px;
+    margin-left: 0px;
+  }
+
+  .error-color {
+    color: #fff;
+    background-color: #f44455;
+    border-color: #f44455;
+  }
+
+  .pass-color {
+    color: #fff;
+    background-color: #5fc27e;
+    border-color: #5fc27e;
+  }
+
+  .fail-color {
+    color: #fff;
+    background-color: #fcc100;
+    border-color: #fcc100;
+  }
+
+  .skip-color {
+    color: #fff;
+    background-color: #6c757d;
+    border-color: #6c757d;
+  }
+
+  /* -- screenshots ---------------------------------------------------------------------- */
+  .img {
+    border-collapse: collapse;
+    max-width: 100%;
+    max-height: 100%;
+    object-fit: contain;
+    position: absolute;
+    top: 0;
+    left: 0;
+    bottom: 0;
+    right: 0;
+    margin: auto;
+  }
+
+  .img-card {
+    height: 600px;
+    width: 800px;
+    background-color: #e7eaf0;
+  }
+
+  .img-circle {
+    height: 20px;
+    border-radius: 12px;
+    background-color: red;
+    padding-left: 13px;
+    margin: 0 auto;
+    position: relative;
+    top: -40px;
+    background-color: rgba(1, 150, 0, 0.3);
+  }
+
+  .img-circle font {
+    border: 1px solid white;
+    width: 11px;
+    height: 11px;
+    border-radius: 50%;
+    margin-right: 9px;
+    margin-top: 4px;
+    display: block;
+    float: left;
+    background-color: white;
+  }
+
+  .close-shots {
+    position: absolute;
+    top: 5px;
+    right: 5px;
+    z-index: 99;
+  }
+
+  .footer {
+    height: 50px;
+    width: 100%;
+    position: fixed;
+    bottom: 0;
+  }
+
+  #headContainer {
+    margin-top: 20px;
+    margin-bottom: 20px;
+    padding-left: 30px;
+    padding-right: 30px;
+  }
+
+  .head-list {
+    padding-top: 5px;
+    padding-bottom: 5px;
+  }
+
+  #resultContainer {
+    margin-left: 30px;
+    margin-right: 30px;
+  }
+</style>
```

#### html2text {}

```diff
@@ -1 +0,0 @@
-
```

### Comparing `xtestrunner-1.6.3/XTestRunner/htmlrunner/result.py` & `xtestrunner-1.7.0/XTestRunner/htmlrunner/result.py`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.6.3/XTestRunner/htmlrunner/runner.py` & `xtestrunner-1.7.0/XTestRunner/htmlrunner/runner.py`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.6.3/XTestRunner/xmlrunner/result.py` & `xtestrunner-1.7.0/XTestRunner/xmlrunner/result.py`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.6.3/XTestRunner/xmlrunner/runner.py` & `xtestrunner-1.7.0/XTestRunner/xmlrunner/runner.py`

 * *Files identical despite different names*

### Comparing `xtestrunner-1.6.3/PKG-INFO` & `xtestrunner-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtestrunner
-Version: 1.6.3
+Version: 1.7.0
 Summary: Modern style test report based on unittest framework.
 Home-page: https://github.com/seldomQA/XTestRunner/
 License: Apache-2.0
 Author: bugmaster
 Author-email: fnngj@126.com
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
```

