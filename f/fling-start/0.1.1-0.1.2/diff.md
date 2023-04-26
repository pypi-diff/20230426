# Comparing `tmp/fling_start-0.1.1.tar.gz` & `tmp/fling_start-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fling_start-0.1.1.tar", max compression
+gzip compressed data, was "fling_start-0.1.2.tar", max compression
```

## Comparing `fling_start-0.1.1.tar` & `fling_start-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      156 2023-04-26 00:22:00.443542 fling_start-0.1.1/README.md
--rw-r--r--   0        0        0        6 2023-04-26 00:16:54.664591 fling_start-0.1.1/VERSION
--rw-r--r--   0        0        0        0 2023-04-19 21:06:07.644598 fling_start-0.1.1/fling/__init__.py
--rw-r--r--   0        0        0      427 2023-04-26 01:56:02.255573 fling_start-0.1.1/fling/start.py
--rw-r--r--   0        0        0      358 2023-04-26 17:21:34.844210 fling_start-0.1.1/fling/static/start/styles.css
--rw-r--r--   0        0        0     9044 2023-04-26 17:33:01.291206 fling_start-0.1.1/fling/templates/start/index.html
--rw-r--r--   0        0        0      823 2023-04-20 00:30:35.165486 fling_start-0.1.1/fling/templates/start/x3d.html
--rw-r--r--   0        0        0      600 2023-04-26 01:54:48.722071 fling_start-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      613 1970-01-01 00:00:00.000000 fling_start-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      156 2023-04-26 00:22:00.443542 fling_start-0.1.2/README.md
+-rw-r--r--   0        0        0        6 2023-04-26 18:25:30.486564 fling_start-0.1.2/VERSION
+-rw-r--r--   0        0        0        0 2023-04-19 21:06:07.644598 fling_start-0.1.2/fling/__init__.py
+-rw-r--r--   0        0        0      427 2023-04-26 01:56:02.255573 fling_start-0.1.2/fling/start.py
+-rw-r--r--   0        0        0      456 2023-04-26 18:23:34.476329 fling_start-0.1.2/fling/static/start/styles.css
+-rw-r--r--   0        0        0     8363 2023-04-26 18:24:38.168476 fling_start-0.1.2/fling/templates/start/index.html
+-rw-r--r--   0        0        0      823 2023-04-20 00:30:35.165486 fling_start-0.1.2/fling/templates/start/x3d.html
+-rw-r--r--   0        0        0      600 2023-04-26 18:25:20.474919 fling_start-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      613 1970-01-01 00:00:00.000000 fling_start-0.1.2/PKG-INFO
```

### Comparing `fling_start-0.1.1/fling/templates/start/index.html` & `fling_start-0.1.2/fling/templates/start/index.html`

 * *Files 7% similar despite different names*

```diff
@@ -20,32 +20,31 @@
         You are using an <strong>outdated</strong> browser. Please <a href="#">upgrade your browser</a> to
         improve your experience.
       </p>
     <![endif]-->
 
   <div class="stacked">
     <div id="loading">
-      <svg height="100%" width="100%" viewBox="0 0 800 388">
+      <svg height="100%" width="100%" viewBox="-250 -250 250 250">
         <defs>
           <filter id="blur">
             <feDropShadow dx="10" dy="10" stdDeviation="2">
-              <animate attributeName="stdDeviation" values="2 0; 0 2; 2 0; 0 2; 2 0; " dur="10s"
-                repeatCount="indefinite" fill="freeze" />
+              <animate attributeName="stdDeviation" values="2 0; 0 2; 2 0; 0 2; 2 0; " dur="10s" repeatCount="indefinite" fill="freeze" />
               <animate attributeName="dx" values="0;5;0;-5;0" dur="10s" repeatCount="indefinite" fill="freeze" />
               <animate attributeName="dy" values="5;0;-5;0;5" dur="10s" repeatCount="indefinite" fill="freeze" />
             </feDropShadow>
           </filter>
-          <path
+          <!-- <path
             d="M 400.372 49.999 C 323.997 50.539 274.407 85.548 275.005 181.908 C 275.603 278.243 353.793 299.809 402.037 299.991 C 450.181 300.17 524.341 279.245 524.992 183.114 C 525.663 84.284 481.094 49.427 400.372 49.999 Z"
-            id="circlepath3"></path>
+            id="circlepath3"></path> -->
           <path d="M 0 0 A 50 50 0 0 1 -50 50 A 50 50 0 0 1 -100 0 A 50 50 0 0 1 -50 -50 A 50 50 0 0 1 0 0 Z"
             id="circlepath4"></path>
 
           <filter id="loading-shader" color-interpolation-filters="sRGB" filterUnits="userSpaceOnUse"
-            primitiveUnits="userSpaceOnUse" width="200vw" height="200vh" x="-50vw" y="-50vh">
+            primitiveUnits="userSpaceOnUse" width="300%" height="200%" x="-500" y="-500" > <!-- width="200vw" height="200vh" x="-50vw" y="-50vh" -->
             <feSpecularLighting id="specLighting" result="specOut" specularExponent="500" specularConstant="0.5"
               lighting-color="#bb99bb">
               <fePointLight id="point-light" x="0" y="75" z="1000" />
             </feSpecularLighting>
             <animate xlink:href="#point-light" id="anim-dialiate" attributeName="x" values="-10; 810; -10" dur="10s"
               repeatCount="indefinite" />
             <animate xlink:href="#point-light" id="anim-dialiate" attributeName="y" values="50; 350; 50" dur="12s"
@@ -55,93 +54,86 @@
             <animate xlink:href="#specLighting" attributeName="lighting-color" values="#bb99bb; red; black; #bb99bb"
               dur="18s" repeatCount="indefinite" />
             <animate xlink:href="#specLighting" attributeName="specularConstant" values="0.5;0.1;0.5" dur="10s"
               repeatCount="indefinite" fill="freeze" />
             <feComposite in="SourceGraphic" in2="specOut" operator="arithmetic" k1="0" k2="1" k3="1" k4="0" />
           </filter>
         </defs>
-        <g filter="url(#loading-shader)" x="0" y="0" width="100%" height="100%">
-          <rect id="stage" x="-400" y="-200" width="200vw" height="200vh" style="fill:#888899">
-            <animate attributeName="fill" values="grey; light grey; light blue; pink; grey" begin="3s" dur="10s"
+        <g id="shadedgroup" width="100%" height="100%">
+          <rect id="stage" width="300%" height="300%" x="-500" y="-500">
+            <animate attributeName="fill" values="grey; light-grey; light-blue; pink; grey" begin="3s" dur="10s"
               repeatCount="indefinite" />
           </rect>
-          <g width="100%" height="100%">
+          <g width="100%" height="100%" transform="translate(-70, -125)">
 
             <!-- <animateMotion dur="40s" repeatCount="indefinite">
               <mpath xlink:href="#circlepath3" />
             </animateMotion> -->
-            <animateTransform attributeName="transform" type="scale" values="0.8 0.8; 1 1; 0.9 0.9; 0.8 0.8;" dur="10s"
-              repeatCount="indefinite" />
-            <animateTransform attributeName="transform" type="translate" values="-50 200; 450 200; 450 200; 950 200;"
+            <!-- <animateTransform attributeName="transform" type="scale" values="0.8 0.8; 1 1; 0.9 0.9; 0.8 0.8;" dur="10s"
+              repeatCount="indefinite" /> -->
+            <!-- <animateTransform attributeName="transform" type="translate" values="-50 50%; 45% 50%; 55% 50%; 120% 50%;"
               dur="10s" keyTimes="0; 0.2; 0.8; 1" keySplines="0.1 0.8 0.2 1; 0.5 0 0.5 1; 0.5 0 0 1" calcMode="spline"
-              repeatCount="indefinite" />
+              repeatCount="indefinite" /> -->
             <!-- <animateTransform
       attributeName="transform"
       type="skewX"
       
       values="0; 5; 10; 15; 15; 10; 5; 0; -5; -10; -15; -15; -10; -5; 0;"
       dur="15s"
       repeatCount="indefinite" /> -->
             <circle class="loadingCircle" r="20">
-              <animateMotion dur="5.6s" repeatCount="indefinite" begin="0" keyTimes="0;  0.4; 1"
-                keySplines="0.1 0.1 0.1 0.1; 0.1 0.1 0.1 0.1;" calcMode="spline">
+              <animateMotion dur="5.6s" repeatCount="indefinite" begin="0">
                 <mpath xlink:href="#circlepath4" />
               </animateMotion>
               <animate attributeName="fill" values="red; orange; yellow; green; blue; indigo; violet; red;" begin="1.5s"
                 dur="10s" repeatCount="indefinite" />
               <animate attributeName="r" values="16;20;20;16" dur="5s" repeatCount="indefinite" />
             </circle>
             <circle class="loadingCircle" r="20">
-              <animateMotion dur="5.6s" begin="0.8s" repeatCount="indefinite" keyTimes="0;  0.5; 1"
-                keySplines="0.1 0.1 0.1 0.1; 0.1 0.1 0.1 0.1;" calcMode="spline">
+              <animateMotion dur="5.6s" begin="0.8s" repeatCount="indefinite">
                 <mpath xlink:href="#circlepath4" />
               </animateMotion>
               <animate attributeName="r" values="16;20;20;16" dur="5s" repeatCount="indefinite" />
               <animate attributeName="fill" values="red; orange; yellow; green; blue; indigo; violet; red;" begin="1.2s"
                 dur="10s" repeatCount="indefinite" />
             </circle>
             <circle class="loadingCircle" r="20">
-              <animateMotion dur="5.6s" begin="1.6s" keyTimes="0;  0.5; 1"
-                keySplines="0.1 0.1 0.1 0.1; 0.1 0.1 0.1 0.1;" calcMode="spline" repeatCount="indefinite">
+              <animateMotion dur="5.6s" begin="1.6s" repeatCount="indefinite">
                 <mpath xlink:href="#circlepath4" />
               </animateMotion>
               <animate attributeName="r" values="16;20;20;16" dur="5s" repeatCount="indefinite" />
               <animate attributeName="fill" values="red; orange; yellow; green; blue; indigo; violet; red;" begin="0.9s"
                 dur="10s" repeatCount="indefinite" />
             </circle>
             <circle class="loadingCircle" r="20">
-              <animateMotion dur="5.6s" begin="2.4s" keyTimes="0;  0.5; 1" keySplines="0.1 0.1 0.1 0.1; 0.1 0.1 0.1 0.1;"
-                calcMode="spline" repeatCount="indefinite">
+              <animateMotion dur="5.6s" begin="2.4s" repeatCount="indefinite">
                 <mpath xlink:href="#circlepath4" />
               </animateMotion>
               <animate attributeName="r" values="16;20;20;16" dur="5s" repeatCount="indefinite" />
               <animate attributeName="fill" values="red; orange; yellow; green; blue; indigo; violet; red;" begin="0.6s"
                 dur="10s" repeatCount="indefinite" />
             </circle>
             <circle class="loadingCircle" r="20">
-              <animateMotion id="circle4motion" dur="5.6s" begin="3.2s" keyTimes="0;  0.5; 1"
-                keySplines="0.1 0.1 0.1 0.1; 0.1 0.1 0.1 0.1;" calcMode="spline" fill="freeze" repeatCount="indefinite">
+              <animateMotion id="circle4motion" dur="5.6s" begin="3.2s" fill="freeze" repeatCount="indefinite">
                 <mpath xlink:href="#circlepath4" />
               </animateMotion>
               <animate attributeName="r" values="16;20;20;16" dur="5s" repeatCount="indefinite" />
               <animate attributeName="fill" values="red; orange; yellow; green; blue; indigo; violet; red;" begin="0.3s"
                 dur="10s" repeatCount="indefinite" />
             </circle>
             <circle class="loadingCircle" r="20">
-              <animateMotion id="circle4motion" dur="5.6s" begin="4.0s" keyTimes="0;  0.5; 1"
-                keySplines="0.1 0.1 0.1 0.1; 0.1 0.1 0.1 0.1;" calcMode="spline" fill="freeze" repeatCount="indefinite">
+              <animateMotion id="circle4motion" dur="5.6s" begin="4.0s" fill="freeze" repeatCount="indefinite">
                 <mpath xlink:href="#circlepath4" />
               </animateMotion>
               <animate attributeName="r" values="16;20;20;16" dur="5s" repeatCount="indefinite" />
               <animate attributeName="fill" values="red; orange; yellow; green; blue; indigo; violet; red;" begin="0s"
                 dur="10s" repeatCount="indefinite" />
             </circle>
             <circle class="loadingCircle" r="20">
-              <animateMotion id="circle4motion" dur="5.6s" begin="4.8s" keyTimes="0;  0.5; 1"
-                keySplines="0.1 0.1 0.1 0.1; 0.1 0.1 0.1 0.1;" calcMode="spline" calcMode="spline" fill="freeze" repeatCount="indefinite">
+              <animateMotion id="circle4motion" dur="5.6s" begin="4.8s" fill="freeze" repeatCount="indefinite">
                 <mpath xlink:href="#circlepath4" />
               </animateMotion>
               <animate attributeName="r" values="16;20;20;16" dur="5s" repeatCount="indefinite" />
               <animate attributeName="fill" values="red; orange; yellow; green; blue; indigo; violet; red;"
                 begin="-0.2s" dur="10s" repeatCount="indefinite" />
             </circle>
           </g>
```

### Comparing `fling_start-0.1.1/fling/templates/start/x3d.html` & `fling_start-0.1.2/fling/templates/start/x3d.html`

 * *Files identical despite different names*

### Comparing `fling_start-0.1.1/pyproject.toml` & `fling_start-0.1.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "fling-start"
-version = "0.1.1"
+version = "0.1.2"
 description = "Side Project Management from the command line"
 authors = [
     "Joshua McKenty <jmckenty@gmail.com>",
     "Anouk Ruhaak <anoukruhaak@gmail.com>",
 ]
 readme = "README.md"
 include = [{ path = "VERSION" }, { path = "README.md" },
```

### Comparing `fling_start-0.1.1/PKG-INFO` & `fling_start-0.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fling-start
-Version: 0.1.1
+Version: 0.1.2
 Summary: Side Project Management from the command line
 Author: Joshua McKenty
 Author-email: jmckenty@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

