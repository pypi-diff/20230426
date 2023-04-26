# Comparing `tmp/wagtail_reoako-1.0.0.tar.gz` & `tmp/wagtail_reoako-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_reoako-1.0.0.tar", last modified: Thu Aug 12 02:41:35 2021, max compression
+gzip compressed data, was "dist/wagtail_reoako-1.1.0.tar", last modified: Wed Apr 26 00:32:17 2023, max compression
```

## Comparing `wagtail_reoako-1.0.0.tar` & `wagtail_reoako-1.1.0.tar`

### file list

```diff
@@ -1,28 +1,45 @@
-drwxr-xr-x   0 pathorsley   (503) staff       (20)        0 2021-08-12 02:41:35.977876 wagtail_reoako-1.0.0/
--rw-r--r--   0 pathorsley   (503) staff       (20)      117 2021-08-11 22:08:31.000000 wagtail_reoako-1.0.0/LICENSE
--rw-r--r--   0 pathorsley   (503) staff       (20)       87 2021-08-12 02:30:02.000000 wagtail_reoako-1.0.0/MANIFEST.in
--rw-r--r--   0 pathorsley   (503) staff       (20)     1792 2021-08-12 02:41:35.978107 wagtail_reoako-1.0.0/PKG-INFO
--rw-r--r--   0 pathorsley   (503) staff       (20)      729 2021-08-12 02:30:02.000000 wagtail_reoako-1.0.0/README.md
--rw-r--r--   0 pathorsley   (503) staff       (20)      779 2021-08-12 02:41:35.979642 wagtail_reoako-1.0.0/setup.cfg
--rw-r--r--   0 pathorsley   (503) staff       (20)      902 2021-08-12 02:30:02.000000 wagtail_reoako-1.0.0/setup.py
-drwxr-xr-x   0 pathorsley   (503) staff       (20)        0 2021-08-12 02:41:35.968867 wagtail_reoako-1.0.0/wagtail_reoako/
--rw-r--r--   0 pathorsley   (503) staff       (20)       85 2021-08-12 02:30:02.000000 wagtail_reoako-1.0.0/wagtail_reoako/__init__.py
--rw-r--r--   0 pathorsley   (503) staff       (20)      137 2021-08-12 02:30:02.000000 wagtail_reoako-1.0.0/wagtail_reoako/apps.py
--rw-r--r--   0 pathorsley   (503) staff       (20)     1361 2021-08-12 02:30:02.000000 wagtail_reoako-1.0.0/wagtail_reoako/reoako_client.py
-drwxr-xr-x   0 pathorsley   (503) staff       (20)        0 2021-08-12 02:41:35.948352 wagtail_reoako-1.0.0/wagtail_reoako/static/
-drwxr-xr-x   0 pathorsley   (503) staff       (20)        0 2021-08-12 02:41:35.948561 wagtail_reoako-1.0.0/wagtail_reoako/static/wagtail_reoako/
-drwxr-xr-x   0 pathorsley   (503) staff       (20)        0 2021-08-12 02:41:35.972991 wagtail_reoako-1.0.0/wagtail_reoako/static/wagtail_reoako/js/
--rw-r--r--   0 pathorsley   (503) staff       (20)     5998 2021-08-12 02:41:35.000000 wagtail_reoako-1.0.0/wagtail_reoako/static/wagtail_reoako/js/reoako.js
-drwxr-xr-x   0 pathorsley   (503) staff       (20)        0 2021-08-12 02:41:35.948970 wagtail_reoako-1.0.0/wagtail_reoako/templates/
-drwxr-xr-x   0 pathorsley   (503) staff       (20)        0 2021-08-12 02:41:35.977006 wagtail_reoako-1.0.0/wagtail_reoako/templates/wagtail_reoako/
--rw-r--r--   0 pathorsley   (503) staff       (20)      503 2021-08-12 02:30:02.000000 wagtail_reoako-1.0.0/wagtail_reoako/templates/wagtail_reoako/_ajax_results.html
--rw-r--r--   0 pathorsley   (503) staff       (20)     1726 2021-08-12 02:30:02.000000 wagtail_reoako-1.0.0/wagtail_reoako/templates/wagtail_reoako/_results.html
--rw-r--r--   0 pathorsley   (503) staff       (20)      331 2021-08-12 02:30:02.000000 wagtail_reoako-1.0.0/wagtail_reoako/templates/wagtail_reoako/reoako.html
--rw-r--r--   0 pathorsley   (503) staff       (20)      372 2021-08-12 02:30:02.000000 wagtail_reoako-1.0.0/wagtail_reoako/urls.py
--rw-r--r--   0 pathorsley   (503) staff       (20)     1468 2021-08-12 02:30:02.000000 wagtail_reoako-1.0.0/wagtail_reoako/views.py
--rw-r--r--   0 pathorsley   (503) staff       (20)     3052 2021-08-12 02:30:02.000000 wagtail_reoako-1.0.0/wagtail_reoako/wagtail_hooks.py
-drwxr-xr-x   0 pathorsley   (503) staff       (20)        0 2021-08-12 02:41:35.972138 wagtail_reoako-1.0.0/wagtail_reoako.egg-info/
--rw-r--r--   0 pathorsley   (503) staff       (20)     1792 2021-08-12 02:41:35.000000 wagtail_reoako-1.0.0/wagtail_reoako.egg-info/PKG-INFO
--rw-r--r--   0 pathorsley   (503) staff       (20)      576 2021-08-12 02:41:35.000000 wagtail_reoako-1.0.0/wagtail_reoako.egg-info/SOURCES.txt
--rw-r--r--   0 pathorsley   (503) staff       (20)        1 2021-08-12 02:41:35.000000 wagtail_reoako-1.0.0/wagtail_reoako.egg-info/dependency_links.txt
--rw-r--r--   0 pathorsley   (503) staff       (20)       15 2021-08-12 02:41:35.000000 wagtail_reoako-1.0.0/wagtail_reoako.egg-info/top_level.txt
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-26 00:32:17.367293 wagtail_reoako-1.1.0/
+-rw-r--r--   0 richardblake   (502) staff       (20)      638 2023-04-26 00:24:51.000000 wagtail_reoako-1.1.0/CHANGELOG.txt
+-rw-r--r--   0 richardblake   (502) staff       (20)     1968 2023-04-26 00:24:51.000000 wagtail_reoako-1.1.0/DEV_README.md
+-rw-r--r--   0 richardblake   (502) staff       (20)      117 2023-04-18 00:59:11.000000 wagtail_reoako-1.1.0/LICENSE
+-rw-r--r--   0 richardblake   (502) staff       (20)      184 2023-04-26 00:28:17.000000 wagtail_reoako-1.1.0/MANIFEST.in
+-rw-r--r--   0 richardblake   (502) staff       (20)     2685 2023-04-26 00:32:17.367536 wagtail_reoako-1.1.0/PKG-INFO
+-rw-r--r--   0 richardblake   (502) staff       (20)     1482 2023-04-26 00:24:51.000000 wagtail_reoako-1.1.0/README.md
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-26 00:32:17.347917 wagtail_reoako-1.1.0/build_test/
+-rw-r--r--   0 richardblake   (502) staff       (20)       58 2023-04-26 00:24:51.000000 wagtail_reoako-1.1.0/build_test/__init__.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      192 2023-04-26 00:24:51.000000 wagtail_reoako-1.1.0/build_test/apps.py
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-26 00:32:17.351348 wagtail_reoako-1.1.0/build_test/migrations/
+-rw-r--r--   0 richardblake   (502) staff       (20)      651 2023-04-26 00:24:51.000000 wagtail_reoako-1.1.0/build_test/migrations/0001_initial.py
+-rw-r--r--   0 richardblake   (502) staff       (20)     1720 2023-04-26 00:24:51.000000 wagtail_reoako-1.1.0/build_test/migrations/0002_create_homepage.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      621 2023-04-26 00:24:51.000000 wagtail_reoako-1.1.0/build_test/migrations/0003_add_rich_text_field_to_homepage.py
+-rw-r--r--   0 richardblake   (502) staff       (20)        0 2023-04-26 00:24:51.000000 wagtail_reoako-1.1.0/build_test/migrations/__init__.py
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-26 00:32:17.352482 wagtail_reoako-1.1.0/build_test/models/
+-rw-r--r--   0 richardblake   (502) staff       (20)       32 2023-04-26 00:24:51.000000 wagtail_reoako-1.1.0/build_test/models/__init__.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      705 2023-04-26 00:24:51.000000 wagtail_reoako-1.1.0/build_test/models/home_page.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      994 2023-04-26 00:24:51.000000 wagtail_reoako-1.1.0/build_test/urls.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      454 2023-04-26 00:24:51.000000 wagtail_reoako-1.1.0/build_test/wsgi.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      288 2023-04-26 00:24:51.000000 wagtail_reoako-1.1.0/pyproject.toml
+-rw-r--r--   0 richardblake   (502) staff       (20)      842 2023-04-26 00:32:17.368530 wagtail_reoako-1.1.0/setup.cfg
+-rw-r--r--   0 richardblake   (502) staff       (20)      902 2023-04-24 11:46:31.000000 wagtail_reoako-1.1.0/setup.py
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-26 00:32:17.359110 wagtail_reoako-1.1.0/wagtail_reoako/
+-rw-r--r--   0 richardblake   (502) staff       (20)       85 2023-04-26 00:24:51.000000 wagtail_reoako-1.1.0/wagtail_reoako/__init__.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      137 2023-04-18 00:59:11.000000 wagtail_reoako-1.1.0/wagtail_reoako/apps.py
+-rw-r--r--   0 richardblake   (502) staff       (20)     1361 2023-04-18 00:59:11.000000 wagtail_reoako-1.1.0/wagtail_reoako/reoako_client.py
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-26 00:32:17.338122 wagtail_reoako-1.1.0/wagtail_reoako/static/
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-26 00:32:17.338265 wagtail_reoako-1.1.0/wagtail_reoako/static/wagtail_reoako/
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-26 00:32:17.363155 wagtail_reoako-1.1.0/wagtail_reoako/static/wagtail_reoako/js/
+-rw-r--r--   0 richardblake   (502) staff       (20)     6810 2023-04-26 00:32:17.000000 wagtail_reoako-1.1.0/wagtail_reoako/static/wagtail_reoako/js/reoako.js
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-26 00:32:17.338696 wagtail_reoako-1.1.0/wagtail_reoako/templates/
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-26 00:32:17.366600 wagtail_reoako-1.1.0/wagtail_reoako/templates/wagtail_reoako/
+-rw-r--r--   0 richardblake   (502) staff       (20)      503 2023-04-18 00:59:11.000000 wagtail_reoako-1.1.0/wagtail_reoako/templates/wagtail_reoako/_ajax_results.html
+-rw-r--r--   0 richardblake   (502) staff       (20)     1733 2023-04-26 00:24:51.000000 wagtail_reoako-1.1.0/wagtail_reoako/templates/wagtail_reoako/_results.html
+-rw-r--r--   0 richardblake   (502) staff       (20)      340 2023-04-26 00:24:51.000000 wagtail_reoako-1.1.0/wagtail_reoako/templates/wagtail_reoako/reoako.html
+-rw-r--r--   0 richardblake   (502) staff       (20)      651 2023-04-26 00:24:51.000000 wagtail_reoako-1.1.0/wagtail_reoako/templates/wagtail_reoako/reoako_icon.svg
+-rw-r--r--   0 richardblake   (502) staff       (20)      372 2023-04-18 00:59:11.000000 wagtail_reoako-1.1.0/wagtail_reoako/urls.py
+-rw-r--r--   0 richardblake   (502) staff       (20)     1468 2023-04-18 00:59:11.000000 wagtail_reoako-1.1.0/wagtail_reoako/views.py
+-rw-r--r--   0 richardblake   (502) staff       (20)     2642 2023-04-26 00:24:51.000000 wagtail_reoako-1.1.0/wagtail_reoako/wagtail_hooks.py
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-26 00:32:17.362582 wagtail_reoako-1.1.0/wagtail_reoako.egg-info/
+-rw-r--r--   0 richardblake   (502) staff       (20)     2685 2023-04-26 00:32:17.000000 wagtail_reoako-1.1.0/wagtail_reoako.egg-info/PKG-INFO
+-rw-r--r--   0 richardblake   (502) staff       (20)      996 2023-04-26 00:32:17.000000 wagtail_reoako-1.1.0/wagtail_reoako.egg-info/SOURCES.txt
+-rw-r--r--   0 richardblake   (502) staff       (20)        1 2023-04-26 00:32:17.000000 wagtail_reoako-1.1.0/wagtail_reoako.egg-info/dependency_links.txt
+-rw-r--r--   0 richardblake   (502) staff       (20)       15 2023-04-26 00:32:17.000000 wagtail_reoako-1.1.0/wagtail_reoako.egg-info/top_level.txt
```

### Comparing `wagtail_reoako-1.0.0/setup.cfg` & `wagtail_reoako-1.1.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 [metadata]
 name = wagtail_reoako
 description_file = README.md
 description = Reoako translator for wagtail draftail editor
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = octavenz
-author_email = support@octave.nz
+author_email = support@reoako.nz
 license = UNLICENSED
 classifiers = 
 	Development Status :: 3 - Alpha
 	Environment :: Web Environment
 	Intended Audience :: Developers
 	License :: OSI Approved :: BSD License
 	Framework :: Django
 	Framework :: Wagtail
 	Framework :: Wagtail :: 2
+	Framework :: Wagtail :: 3
+	Framework :: Wagtail :: 4
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Topic :: Internet :: WWW/HTTP
 	Topic :: Internet :: WWW/HTTP :: Site Management
 
 [options]
 include_package_data = true
-packages = find:
+packages = wagtail_reoako
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `wagtail_reoako-1.0.0/setup.py` & `wagtail_reoako-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `wagtail_reoako-1.0.0/wagtail_reoako/reoako_client.py` & `wagtail_reoako-1.1.0/wagtail_reoako/reoako_client.py`

 * *Files identical despite different names*

### Comparing `wagtail_reoako-1.0.0/wagtail_reoako/static/wagtail_reoako/js/reoako.js` & `wagtail_reoako-1.1.0/wagtail_reoako/static/wagtail_reoako/js/reoako.js`

 * *Files 24% similar despite different names*

#### js-beautify {}

```diff
@@ -1,83 +1,83 @@
 ! function(t) {
     var e = {};
 
-    function n(o) {
-        if (e[o]) return e[o].exports;
-        var r = e[o] = {
-            i: o,
+    function o(n) {
+        if (e[n]) return e[n].exports;
+        var r = e[n] = {
+            i: n,
             l: !1,
             exports: {}
         };
-        return t[o].call(r.exports, r, r.exports, n), r.l = !0, r.exports
+        return t[n].call(r.exports, r, r.exports, o), r.l = !0, r.exports
     }
-    n.m = t, n.c = e, n.d = function(t, e, o) {
-        n.o(t, e) || Object.defineProperty(t, e, {
+    o.m = t, o.c = e, o.d = function(t, e, n) {
+        o.o(t, e) || Object.defineProperty(t, e, {
             enumerable: !0,
-            get: o
+            get: n
         })
-    }, n.r = function(t) {
+    }, o.r = function(t) {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(t, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(t, "__esModule", {
             value: !0
         })
-    }, n.t = function(t, e) {
-        if (1 & e && (t = n(t)), 8 & e) return t;
+    }, o.t = function(t, e) {
+        if (1 & e && (t = o(t)), 8 & e) return t;
         if (4 & e && "object" == typeof t && t && t.__esModule) return t;
-        var o = Object.create(null);
-        if (n.r(o), Object.defineProperty(o, "default", {
+        var n = Object.create(null);
+        if (o.r(n), Object.defineProperty(n, "default", {
                 enumerable: !0,
                 value: t
             }), 2 & e && "string" != typeof t)
-            for (var r in t) n.d(o, r, function(e) {
+            for (var r in t) o.d(n, r, function(e) {
                 return t[e]
             }.bind(null, r));
-        return o
-    }, n.n = function(t) {
+        return n
+    }, o.n = function(t) {
         var e = t && t.__esModule ? function() {
             return t.default
         } : function() {
             return t
         };
-        return n.d(e, "a", e), e
-    }, n.o = function(t, e) {
+        return o.d(e, "a", e), e
+    }, o.o = function(t, e) {
         return Object.prototype.hasOwnProperty.call(t, e)
-    }, n.p = "", n(n.s = 0)
-}([function(t, e, n) {
+    }, o.p = "", o(o.s = 0)
+}([function(t, e, o) {
     "use strict";
     (function(t) {
         function e(t) {
             return (e = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(t) {
                 return typeof t
             } : function(t) {
                 return t && "function" == typeof Symbol && t.constructor === Symbol && t !== Symbol.prototype ? "symbol" : typeof t
             })(t)
         }
-        var o = n(2);
+        var n = o(2);
 
         function r() {
             return (r = Object.assign || function(t) {
                 for (var e = 1; e < arguments.length; e++) {
-                    var n = arguments[e];
-                    for (var o in n) Object.prototype.hasOwnProperty.call(n, o) && (t[o] = n[o])
+                    var o = arguments[e];
+                    for (var n in o) Object.prototype.hasOwnProperty.call(o, n) && (t[n] = o[n])
                 }
                 return t
             }).apply(this, arguments)
         }
 
         function i(t, e) {
-            for (var n = 0; n < e.length; n++) {
-                var o = e[n];
-                o.enumerable = o.enumerable || !1, o.configurable = !0, "value" in o && (o.writable = !0), Object.defineProperty(t, o.key, o)
+            for (var o = 0; o < e.length; o++) {
+                var n = e[o];
+                n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(t, n.key, n)
             }
         }
 
-        function u(t, e) {
-            return (u = Object.setPrototypeOf || function(t, e) {
+        function a(t, e) {
+            return (a = Object.setPrototypeOf || function(t, e) {
                 return t.__proto__ = e, t
             })(t, e)
         }
 
         function c(t) {
             var e = function() {
                 if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
@@ -86,120 +86,160 @@
                 try {
                     return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
                 } catch (t) {
                     return !1
                 }
             }();
             return function() {
-                var n, o = f(t);
+                var o, n = f(t);
                 if (e) {
                     var r = f(this).constructor;
-                    n = Reflect.construct(o, arguments, r)
-                } else n = o.apply(this, arguments);
-                return a(this, n)
+                    o = Reflect.construct(n, arguments, r)
+                } else o = n.apply(this, arguments);
+                return u(this, o)
             }
         }
 
-        function a(t, n) {
-            return !n || "object" !== e(n) && "function" != typeof n ? l(t) : n
+        function u(t, o) {
+            return !o || "object" !== e(o) && "function" != typeof o ? l(t) : o
         }
 
         function l(t) {
             if (void 0 === t) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
             return t
         }
 
         function f(t) {
             return (f = Object.setPrototypeOf ? Object.getPrototypeOf : function(t) {
                 return t.__proto__ || Object.getPrototypeOf(t)
             })(t)
         }
         var s = window.React,
-            p = window.draftail,
-            y = window.DraftJS.Modifier,
-            d = window.DraftJS.EditorState,
-            b = window.$,
-            h = function(e) {
+            d = window.draftail,
+            p = window.DraftJS.Modifier,
+            y = window.DraftJS.EditorState,
+            h = window.$,
+            b = function(e) {
                 ! function(t, e) {
                     if ("function" != typeof e && null !== e) throw new TypeError("Super expression must either be null or a function");
                     t.prototype = Object.create(e && e.prototype, {
                         constructor: {
                             value: t,
                             writable: !0,
                             configurable: !0
                         }
-                    }), e && u(t, e)
+                    }), e && a(t, e)
                 }(s, e);
-                var n, r, a, f = c(s);
+                var o, r, u, f = c(s);
 
                 function s(t) {
                     var e;
                     return function(t, e) {
                         if (!(t instanceof e)) throw new TypeError("Cannot call a class as a function")
                     }(this, s), (e = f.call(this, t)).onChosen = e.onChosen.bind(l(e)), e.onClose = e.onClose.bind(l(e)), e
                 }
-                return n = s, (r = [{
+                return o = s, (r = [{
+                    key: "browseApi",
+                    value: function(t, e) {
+                        var o = h(".reoako-search-results", t.body).html();
+                        t.ajaxifyForm(h("form.search-form", t.body));
+                        var n, r = h("form.search-form", t.body).attr("action");
+
+                        function i() {
+                            var e = h("#id_q", t.body).val();
+                            return "" !== e ? n = h.ajax({
+                                url: r,
+                                data: {
+                                    q: e
+                                },
+                                success: function(e) {
+                                    n = null, h(".reoako-search-results", t.body).html(e), h(".reoako-search-results a.reoako-choose-word", t.body).on("click", (function() {
+                                        var e = h(this).data();
+                                        return t.respond("wordChosen", e), t.close(), !1
+                                    }))
+                                },
+                                error: function() {
+                                    n = null
+                                }
+                            }) : (h(".reoako-search-results", t.body).html(o), a()), !1
+                        }
+
+                        function a() {
+                            h("a.reoako-choose-word", t.body).on("click", (function() {
+                                var e = h(this).data();
+                                return t.respond("wordChosen", e), t.close(), !1
+                            }))
+                        }
+                        h("#id_q", t.body).on("input", (function() {
+                            n && n.abort(), clearTimeout(h.data(this, "timer"));
+                            var t = setTimeout(i, 200);
+                            h(this).data("timer", t)
+                        })), a()
+                    }
+                }, {
                     key: "componentWillMount",
                     value: function() {
                         var e = this.props,
-                            n = e.onClose,
+                            o = e.onClose,
                             r = e.editorState;
-                        b(document.body).on("hidden.bs.modal", this.onClose), this.workflow = t.ModalWorkflow({
+                        h(document.body).on("hidden.bs.modal", this.onClose);
+                        var i = this;
+                        this.workflow = t.ModalWorkflow({
                             url: "/admin/reoako-modal/",
                             onload: {
-                                browse: function(e, n) {
-                                    var i = b(".search-form #id_q", e.body);
-                                    i.attr("autocomplete", "off"), t.PAGE_CHOOSER_MODAL_ONLOAD_HANDLERS.browse(e, n);
-                                    var u = (0, o.getSelectionText)(r);
-                                    u && i.val(u).trigger("input"), setTimeout((function() {
-                                        return i.eq(0).focus()
+                                browse: function(t, e) {
+                                    var o = h(".search-form #id_q", t.body);
+                                    o.attr("autocomplete", "off"), i.browseApi(t, e);
+                                    var a = (0, n.getSelectionText)(r);
+                                    a && o.val(a).trigger("input"), setTimeout((function() {
+                                        return o.eq(0).focus()
                                     }), 600)
                                 }
                             },
                             responses: {
-                                pageChosen: this.onChosen
+                                wordChosen: this.onChosen
                             },
                             onError: function(t) {
-                                console.log(t), n()
+                                o()
                             }
                         })
                     }
                 }, {
                     key: "componentWillUnmount",
                     value: function() {
-                        this.workflow = null, b(document.body).off("hidden.bs.modal", this.onClose)
+                        this.workflow = null, h(document.body).off("hidden.bs.modal", this.onClose)
                     }
                 }, {
                     key: "onChosen",
                     value: function(t) {
                         var e = this.props,
-                            n = e.editorState,
-                            o = e.entityType,
+                            o = e.editorState,
+                            n = e.entityType,
                             r = e.onComplete,
-                            i = n.getSelection(),
-                            u = t.reoakoTranslation,
-                            c = n.getCurrentContent(),
-                            a = c.createEntity(o.type, "MUTABLE", t).getLastCreatedEntityKey(),
-                            l = y.replaceText(c, i, u, null, a);
-                        r(d.push(n, l, "insert-characters"))
+                            i = o.getSelection(),
+                            a = t.reoakoTranslation,
+                            c = o.getCurrentContent(),
+                            u = c.createEntity(n.type, "MUTABLE", t).getLastCreatedEntityKey(),
+                            l = p.replaceText(c, i, a, null, u);
+                        r(y.push(o, l, "insert-characters"))
                     }
                 }, {
                     key: "onClose",
                     value: function() {
                         var t = this.props.onClose;
                         t()
                     }
                 }, {
                     key: "render",
                     value: function() {
                         return null
                     }
-                }]) && i(n.prototype, r), a && i(n, a), s
+                }]) && i(o.prototype, r), u && i(o, u), s
             }(s.Component),
-            g = s.createElement("svg", {
+            v = s.createElement("svg", {
                 version: "1.1",
                 xmlns: "http://www.w3.org/2000/svg",
                 viewBox: "0, 0, 1024, 1024",
                 width: "1em",
                 height: "1em",
                 style: {
                     verticalAlign: "middle",
@@ -207,66 +247,66 @@
                 }
             }, s.createElement("path", {
                 d: "M18.2822 114.286C18.2822 68.8406 55.1228 32 100.568 32H923.425C968.87 32 1005.71 68.8406 1005.71 114.286V813.714C1005.71 859.159 968.87 896 923.425 896H622.845L536.183 996.068C523.422 1010.8 500.564 1010.8 487.804 996.068L401.142 896H100.568C55.1228 896 18.2822 859.159 18.2822 813.714V672H443.593V524H443.59V430H443.593V301.438H509.406C565.752 301.438 593.024 325.719 593.024 370.344C593.024 414.75 565.752 437.062 509.856 437.062H444.59V513.188H514.815L602.265 672H710L611.957 497.875C664.472 476 693.547 431.594 693.547 370.344C693.547 281.312 632.918 224 528.113 224H346V671H18.2822V114.286Z",
                 fill: "currentColor"
             }));
         window.draftail.registerPlugin({
             type: "REOAKO",
-            source: h,
+            source: b,
             decorator: function(t) {
                 var e = t.entityKey,
-                    n = t.contentState,
-                    o = t.children,
-                    i = n.getEntity(e).getData();
-                return s.createElement(p.TooltipEntity, r({}, t, {
+                    o = t.contentState,
+                    n = t.children,
+                    i = o.getEntity(e).getData();
+                return s.createElement(d.TooltipEntity, r({}, t, {
                     label: "".concat(i.reoakoTranslation, " (").concat(i.reoakoHeadword, ")"),
-                    icon: g
-                }), o)
+                    icon: v
+                }), n)
             }
         })
-    }).call(this, n(1))
+    }).call(this, o(1))
 }, function(t, e) {
-    var n;
-    n = function() {
+    var o;
+    o = function() {
         return this
     }();
     try {
-        n = n || new Function("return this")()
+        o = o || new Function("return this")()
     } catch (t) {
-        "object" == typeof window && (n = window)
+        "object" == typeof window && (o = window)
     }
-    t.exports = n
-}, function(t, e, n) {
+    t.exports = o
+}, function(t, e, o) {
     "use strict";
     Object.defineProperty(e, "__esModule", {
         value: !0
     }), e.getSelectionText = void 0;
     e.getSelectionText = function(t) {
         var e = t.getSelection(),
-            n = e.getAnchorOffset(),
-            o = e.getFocusOffset(),
+            o = e.getAnchorOffset(),
+            n = e.getFocusOffset(),
             r = function(t) {
                 var e = t.getSelection(),
-                    n = t.getCurrentContent(),
-                    o = e.getStartKey(),
+                    o = t.getCurrentContent(),
+                    n = e.getStartKey(),
                     r = e.getEndKey(),
-                    i = n.getBlockMap();
+                    i = o.getBlockMap();
                 return i.toSeq().skipUntil((function(t, e) {
-                    return e === o
+                    return e === n
                 })).takeUntil((function(t, e) {
                     return e === r
                 })).concat([
                     [r, i.get(r)]
                 ]).toList()
             }(t);
         if (e.getIsBackward()) {
-            var i = n;
-            n = o, o = i
+            var i = o;
+            o = n, n = i
         }
-        for (var u = "", c = 0; c < r.size; c += 1) {
-            var a = 0 === c ? n : 0,
-                l = c === r.size - 1 ? o : r.get(c).getText().length;
-            u += r.get(c).getText().slice(a, l)
+        for (var a = "", c = 0; c < r.size; c += 1) {
+            var u = 0 === c ? o : 0,
+                l = c === r.size - 1 ? n : r.get(c).getText().length;
+            a += r.get(c).getText().slice(u, l)
         }
-        return u
+        return a
     }
 }]);
```

### Comparing `wagtail_reoako-1.0.0/wagtail_reoako/templates/wagtail_reoako/_results.html` & `wagtail_reoako-1.1.0/wagtail_reoako/templates/wagtail_reoako/_results.html`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         {% if results %}
             {% for result in results %}
                 {% for translation in result.translations %}
                     <tr data-page-title="{{ page.get_admin_display_title }}">
                         <td class='title'>
                             <div class="title-wrapper">
                                 <a
-                                    class="choose-page"
+                                    class="reoako-choose-word"
                                     href="#{{ translation.slug }}"
                                     data-reoako-id="{{ translation.slug }}"
                                     data-reoako-headword="{{ result.headword }}"
                                     data-reoako-translation="{{ translation.mi }}"
                                 >
                                     <strong>{{ translation.mi }}</strong>
                                     <br />
```

### Comparing `wagtail_reoako-1.0.0/wagtail_reoako/views.py` & `wagtail_reoako-1.1.0/wagtail_reoako/views.py`

 * *Files identical despite different names*

### Comparing `wagtail_reoako-1.0.0/wagtail_reoako/wagtail_hooks.py` & `wagtail_reoako-1.1.0/wagtail_reoako/wagtail_hooks.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,31 @@
+from pkg_resources import parse_version
 from draftjs_exporter.dom import DOM
 
 import wagtail.admin.rich_text.editors.draftail.features as draftail_features
 
-from wagtail.core import hooks
+from wagtail import __version__ as WAGTAIL_VERSION
+
+if parse_version(WAGTAIL_VERSION) < parse_version('3.0'):
+    from wagtail.core import hooks
+else:
+    from wagtail import hooks
+
 from wagtail.admin.rich_text.converters.html_to_contentstate import InlineEntityElementHandler
 
 from .urls import urlpatterns
 
-
 @hooks.register('register_admin_urls')
 def wagtail_reoako_urls():
     return urlpatterns
 
+@hooks.register("register_icons")
+def register_icons(icons):
+    return icons + ['wagtail_reoako/reoako_icon.svg']
+
 
 def reoako_entity_decorator(props):
     """
     Draft.js ContentState to database HTML.
     Converts the reoako entities into a span tag.
 
     TODO:
@@ -54,25 +64,15 @@
     feature_name = 'reoako'
     type_ = 'REOAKO'
 
     control = {
         'type': type_,
         'label': '',
         'description': 'Reoako',
-        'icon': [
-            '''
-            M18.2822 114.286C18.2822 68.8406 55.1228 32 100.568 32H923.425C968.87 32 1005.71 
-            68.8406 1005.71 114.286V813.714C1005.71 859.159 968.87 896 923.425 896H622.845L536.183 
-            996.068C523.422 1010.8 500.564 1010.8 487.804 996.068L401.142 896H100.568C55.1228 896 18.2822 
-            859.159 18.2822 813.714V672H443.593V524H443.59V430H443.593V301.438H509.406C565.752 301.438 
-            593.024 325.719 593.024 370.344C593.024 414.75 565.752 437.062 509.856 
-            437.062H444.59V513.188H514.815L602.265 672H710L611.957 497.875C664.472 476 693.547 431.594 
-            693.547 370.344C693.547 281.312 632.918 224 528.113 224H346V671H18.2822V114.286Z
-            '''
-        ],
+        'icon': 'reoako_icon',
     }
 
     features.register_editor_plugin(
         'draftail', feature_name, draftail_features.EntityFeature(
             control,
             js=['wagtail_reoako/js/reoako.js'],
         )
```

