# Comparing `tmp/FImdlp-0.9.3.tar.gz` & `tmp/FImdlp-0.9.4.macosx-13-arm64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FImdlp-0.9.3.tar", last modified: Wed Feb 22 10:57:25 2023, max compression
+gzip compressed data, was "FImdlp-0.9.4.macosx-13-arm64.tar", last modified: Tue Apr 25 16:07:48 2023, max compression
```

## Comparing `FImdlp-0.9.3.tar` & `FImdlp-0.9.4.macosx-13-arm64.tar`

### file list

```diff
@@ -1,31 +1,40 @@
-drwxr-xr-x   0 rmontanana   (501) staff       (20)        0 2023-02-22 10:57:25.684501 FImdlp-0.9.3/
--rw-r--r--   0 rmontanana   (501) staff       (20)     1069 2022-12-13 15:41:55.000000 FImdlp-0.9.3/LICENSE
--rw-r--r--   0 rmontanana   (501) staff       (20)      126 2023-02-22 10:24:42.000000 FImdlp-0.9.3/MANIFEST.in
--rw-r--r--   0 rmontanana   (501) staff       (20)     2446 2023-02-22 10:57:25.684153 FImdlp-0.9.3/PKG-INFO
--rw-r--r--   0 rmontanana   (501) staff       (20)     1638 2022-12-22 18:41:18.000000 FImdlp-0.9.3/README.md
--rw-r--r--   0 rmontanana   (501) staff       (20)     1393 2022-12-23 10:10:29.000000 FImdlp-0.9.3/pyproject.toml
--rw-r--r--   0 rmontanana   (501) staff       (20)       38 2023-02-22 10:57:25.684618 FImdlp-0.9.3/setup.cfg
--rw-r--r--   0 rmontanana   (501) staff       (20)      615 2023-02-22 09:56:29.000000 FImdlp-0.9.3/setup.py
-drwxr-xr-x   0 rmontanana   (501) staff       (20)        0 2023-02-22 10:57:25.673926 FImdlp-0.9.3/src/
-drwxr-xr-x   0 rmontanana   (501) staff       (20)        0 2023-02-22 10:57:25.677014 FImdlp-0.9.3/src/FImdlp.egg-info/
--rw-r--r--   0 rmontanana   (501) staff       (20)     2446 2023-02-22 10:57:25.000000 FImdlp-0.9.3/src/FImdlp.egg-info/PKG-INFO
--rw-r--r--   0 rmontanana   (501) staff       (20)      541 2023-02-22 10:57:25.000000 FImdlp-0.9.3/src/FImdlp.egg-info/SOURCES.txt
--rw-r--r--   0 rmontanana   (501) staff       (20)        1 2023-02-22 10:57:25.000000 FImdlp-0.9.3/src/FImdlp.egg-info/dependency_links.txt
--rw-r--r--   0 rmontanana   (501) staff       (20)       26 2023-02-22 10:57:25.000000 FImdlp-0.9.3/src/FImdlp.egg-info/requires.txt
--rw-r--r--   0 rmontanana   (501) staff       (20)       15 2023-02-22 10:57:25.000000 FImdlp-0.9.3/src/FImdlp.egg-info/top_level.txt
-drwxr-xr-x   0 rmontanana   (501) staff       (20)        0 2023-02-22 10:57:25.679579 FImdlp-0.9.3/src/cppmdlp/
--rw-r--r--   0 rmontanana   (501) staff       (20)     5794 2023-02-22 10:56:09.000000 FImdlp-0.9.3/src/cppmdlp/CPPFImdlp.cpp
--rw-r--r--   0 rmontanana   (501) staff       (20)      775 2023-02-22 09:14:12.000000 FImdlp-0.9.3/src/cppmdlp/CPPFImdlp.h
--rw-r--r--   0 rmontanana   (501) staff       (20)     2263 2023-02-22 09:14:12.000000 FImdlp-0.9.3/src/cppmdlp/Metrics.cpp
--rw-r--r--   0 rmontanana   (501) staff       (20)      515 2023-02-20 18:19:36.000000 FImdlp-0.9.3/src/cppmdlp/Metrics.h
--rw-r--r--   0 rmontanana   (501) staff       (20)      444 2023-02-22 09:14:12.000000 FImdlp-0.9.3/src/cppmdlp/typesFImdlp.h
-drwxr-xr-x   0 rmontanana   (501) staff       (20)        0 2023-02-22 10:57:25.682474 FImdlp-0.9.3/src/fimdlp/
--rw-r--r--   0 rmontanana   (501) staff       (20)      454 2023-02-22 09:56:29.000000 FImdlp-0.9.3/src/fimdlp/Factorize.cpp
--rw-r--r--   0 rmontanana   (501) staff       (20)      195 2023-02-22 09:56:29.000000 FImdlp-0.9.3/src/fimdlp/Factorize.h
--rw-r--r--   0 rmontanana   (501) staff       (20)       68 2023-02-22 09:56:29.000000 FImdlp-0.9.3/src/fimdlp/__init__.py
--rw-r--r--   0 rmontanana   (501) staff       (20)       22 2023-02-22 09:56:29.000000 FImdlp-0.9.3/src/fimdlp/_version.py
--rw-r--r--   0 rmontanana   (501) staff       (20)     1021 2023-02-22 09:56:29.000000 FImdlp-0.9.3/src/fimdlp/cfimdlp.pyx
--rw-r--r--   0 rmontanana   (501) staff       (20)     8455 2023-02-22 09:56:29.000000 FImdlp-0.9.3/src/fimdlp/mdlp.py
-drwxr-xr-x   0 rmontanana   (501) staff       (20)        0 2023-02-22 10:57:25.683323 FImdlp-0.9.3/src/fimdlp/tests/
--rw-r--r--   0 rmontanana   (501) staff       (20)     7904 2023-02-22 10:53:28.000000 FImdlp-0.9.3/src/fimdlp/tests/FImdlp_test.py
--rw-r--r--   0 rmontanana   (501) staff       (20)       36 2022-12-13 15:41:55.000000 FImdlp-0.9.3/src/fimdlp/tests/__init__.py
+drwxr-xr-x   0 rmontanana   (501) staff       (20)        0 2023-04-25 16:07:48.545446 ./
+drwxr-xr-x   0 rmontanana   (501) staff       (20)        0 2023-04-25 16:07:48.545494 ./Users/
+drwxr-xr-x   0 rmontanana   (501) staff       (20)        0 2023-04-25 16:07:48.545543 ./Users/rmontanana/
+drwxr-xr-x   0 rmontanana   (501) staff       (20)        0 2023-04-25 16:07:48.545608 ./Users/rmontanana/.virtualenvs/
+drwxr-xr-x   0 rmontanana   (501) staff       (20)        0 2023-04-25 16:07:48.545655 ./Users/rmontanana/.virtualenvs/310/
+drwxr-xr-x   0 rmontanana   (501) staff       (20)        0 2023-04-25 16:07:48.545702 ./Users/rmontanana/.virtualenvs/310/lib/
+drwxr-xr-x   0 rmontanana   (501) staff       (20)        0 2023-04-25 16:07:48.545750 ./Users/rmontanana/.virtualenvs/310/lib/python3.10/
+drwxr-xr-x   0 rmontanana   (501) staff       (20)        0 2023-04-25 16:07:48.555156 ./Users/rmontanana/.virtualenvs/310/lib/python3.10/site-packages/
+drwxr-xr-x   0 rmontanana   (501) staff       (20)        0 2023-04-25 16:07:48.555884 ./Users/rmontanana/.virtualenvs/310/lib/python3.10/site-packages/FImdlp-0.9.4-py3.10.egg-info/
+-rw-r--r--   0 rmontanana   (501) staff       (20)     2642 2023-04-25 16:07:48.529878 ./Users/rmontanana/.virtualenvs/310/lib/python3.10/site-packages/FImdlp-0.9.4-py3.10.egg-info/PKG-INFO
+-rw-r--r--   0 rmontanana   (501) staff       (20)      589 2023-04-25 16:07:48.535742 ./Users/rmontanana/.virtualenvs/310/lib/python3.10/site-packages/FImdlp-0.9.4-py3.10.egg-info/SOURCES.txt
+-rw-r--r--   0 rmontanana   (501) staff       (20)        1 2023-04-25 16:07:48.530040 ./Users/rmontanana/.virtualenvs/310/lib/python3.10/site-packages/FImdlp-0.9.4-py3.10.egg-info/dependency_links.txt
+-rw-r--r--   0 rmontanana   (501) staff       (20)       26 2023-04-25 16:07:48.530188 ./Users/rmontanana/.virtualenvs/310/lib/python3.10/site-packages/FImdlp-0.9.4-py3.10.egg-info/requires.txt
+-rw-r--r--   0 rmontanana   (501) staff       (20)       15 2023-04-25 16:07:48.530278 ./Users/rmontanana/.virtualenvs/310/lib/python3.10/site-packages/FImdlp-0.9.4-py3.10.egg-info/top_level.txt
+drwxr-xr-x   0 rmontanana   (501) staff       (20)        0 2023-04-25 16:07:48.546443 ./Users/rmontanana/.virtualenvs/310/lib/python3.10/site-packages/cppmdlp/
+-rw-r--r--   0 rmontanana   (501) staff       (20)     7725 2023-04-25 08:55:42.000000 ./Users/rmontanana/.virtualenvs/310/lib/python3.10/site-packages/cppmdlp/CPPFImdlp.cpp
+-rw-r--r--   0 rmontanana   (501) staff       (20)     1284 2023-04-25 08:55:42.000000 ./Users/rmontanana/.virtualenvs/310/lib/python3.10/site-packages/cppmdlp/CPPFImdlp.h
+-rw-r--r--   0 rmontanana   (501) staff       (20)     2468 2023-04-25 08:55:42.000000 ./Users/rmontanana/.virtualenvs/310/lib/python3.10/site-packages/cppmdlp/Metrics.cpp
+-rw-r--r--   0 rmontanana   (501) staff       (20)      558 2023-04-25 08:55:42.000000 ./Users/rmontanana/.virtualenvs/310/lib/python3.10/site-packages/cppmdlp/Metrics.h
+-rw-r--r--   0 rmontanana   (501) staff       (20)      445 2023-04-11 17:30:57.000000 ./Users/rmontanana/.virtualenvs/310/lib/python3.10/site-packages/cppmdlp/typesFImdlp.h
+drwxr-xr-x   0 rmontanana   (501) staff       (20)        0 2023-04-25 16:07:48.548659 ./Users/rmontanana/.virtualenvs/310/lib/python3.10/site-packages/fimdlp/
+-rw-r--r--   0 rmontanana   (501) staff       (20)     3114 2023-04-25 16:05:42.000000 ./Users/rmontanana/.virtualenvs/310/lib/python3.10/site-packages/fimdlp/ArffFiles.cpp
+-rw-r--r--   0 rmontanana   (501) staff       (20)      765 2023-04-25 16:05:42.000000 ./Users/rmontanana/.virtualenvs/310/lib/python3.10/site-packages/fimdlp/ArffFiles.h
+-rw-r--r--   0 rmontanana   (501) staff       (20)      461 2023-04-25 16:05:42.000000 ./Users/rmontanana/.virtualenvs/310/lib/python3.10/site-packages/fimdlp/Factorize.cpp
+-rw-r--r--   0 rmontanana   (501) staff       (20)      195 2023-02-24 16:22:35.000000 ./Users/rmontanana/.virtualenvs/310/lib/python3.10/site-packages/fimdlp/Factorize.h
+-rw-r--r--   0 rmontanana   (501) staff       (20)       68 2023-02-24 16:22:35.000000 ./Users/rmontanana/.virtualenvs/310/lib/python3.10/site-packages/fimdlp/__init__.py
+drwxr-xr-x   0 rmontanana   (501) staff       (20)        0 2023-04-25 16:07:48.552486 ./Users/rmontanana/.virtualenvs/310/lib/python3.10/site-packages/fimdlp/__pycache__/
+-rw-r--r--   0 rmontanana   (501) staff       (20)      247 2023-04-25 16:07:48.551539 ./Users/rmontanana/.virtualenvs/310/lib/python3.10/site-packages/fimdlp/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 rmontanana   (501) staff       (20)      196 2023-04-25 16:07:48.548778 ./Users/rmontanana/.virtualenvs/310/lib/python3.10/site-packages/fimdlp/__pycache__/_version.cpython-310.pyc
+-rw-r--r--   0 rmontanana   (501) staff       (20)     8148 2023-04-25 16:07:48.552442 ./Users/rmontanana/.virtualenvs/310/lib/python3.10/site-packages/fimdlp/__pycache__/mdlp.cpython-310.pyc
+-rw-r--r--   0 rmontanana   (501) staff       (20)       22 2023-04-25 16:05:42.000000 ./Users/rmontanana/.virtualenvs/310/lib/python3.10/site-packages/fimdlp/_version.py
+-rw-r--r--   0 rmontanana   (501) staff       (20)     2585 2023-04-25 16:05:42.000000 ./Users/rmontanana/.virtualenvs/310/lib/python3.10/site-packages/fimdlp/cfimdlp.pyx
+-rwxr-xr-x   0 rmontanana   (501) staff       (20)   150972 2023-04-25 16:07:27.000000 ./Users/rmontanana/.virtualenvs/310/lib/python3.10/site-packages/fimdlp/cppfimdlp.cpython-310-darwin.so
+-rw-r--r--   0 rmontanana   (501) staff       (20)     9615 2023-04-25 16:05:42.000000 ./Users/rmontanana/.virtualenvs/310/lib/python3.10/site-packages/fimdlp/mdlp.py
+drwxr-xr-x   0 rmontanana   (501) staff       (20)        0 2023-04-25 16:07:48.549024 ./Users/rmontanana/.virtualenvs/310/lib/python3.10/site-packages/fimdlp/tests/
+-rw-r--r--   0 rmontanana   (501) staff       (20)    12663 2023-04-25 16:05:42.000000 ./Users/rmontanana/.virtualenvs/310/lib/python3.10/site-packages/fimdlp/tests/FImdlp_test.py
+-rw-r--r--   0 rmontanana   (501) staff       (20)       36 2023-02-24 16:22:35.000000 ./Users/rmontanana/.virtualenvs/310/lib/python3.10/site-packages/fimdlp/tests/__init__.py
+drwxr-xr-x   0 rmontanana   (501) staff       (20)        0 2023-04-25 16:07:48.551326 ./Users/rmontanana/.virtualenvs/310/lib/python3.10/site-packages/fimdlp/tests/__pycache__/
+-rw-r--r--   0 rmontanana   (501) staff       (20)    11799 2023-04-25 16:07:48.551237 ./Users/rmontanana/.virtualenvs/310/lib/python3.10/site-packages/fimdlp/tests/__pycache__/FImdlp_test.cpython-310.pyc
+-rw-r--r--   0 rmontanana   (501) staff       (20)      227 2023-04-25 16:07:48.549123 ./Users/rmontanana/.virtualenvs/310/lib/python3.10/site-packages/fimdlp/tests/__pycache__/__init__.cpython-310.pyc
```

### Comparing `FImdlp-0.9.3/PKG-INFO` & `./Users/rmontanana/.virtualenvs/310/lib/python3.10/site-packages/FImdlp-0.9.4-py3.10.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: FImdlp
-Version: 0.9.3
+Version: 0.9.4
 Author-email: Ricardo Montañana <ricardo.montanana@alu.uclm.es>
 Project-URL: Home, https://github.com/doctorado-ml/FImdlp
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Base, https://github.com/rmontanana/mdlp
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FImdlp
 [![CI](https://github.com/Doctorado-ML/FImdlp/actions/workflows/main.yml/badge.svg)](https://github.com/Doctorado-ML/FImdlp/actions/workflows/main.yml)
 [![CodeQL](https://github.com/Doctorado-ML/FImdlp/actions/workflows/codeql.yml/badge.svg)](https://github.com/Doctorado-ML/FImdlp/actions/workflows/codeql.yml)
@@ -42,21 +44,24 @@
 ## Build and usage sample
 
 ### Python sample
 
 ```bash
 pip install -e .
 python samples/sample.py iris  
-python samples/sample.py iris --alternative
+python samples/sample.py iris -c 2
 python samples/sample.py -h # for more options
 ```
 
 ### C++ sample
 
 ```bash
 cd samples
-mkdir build
+cmake -B build
 cd build
-cmake ..
 make
-./sample iris
+./sample -f iris -c 2
+./sample -h
 ```
+
+### Based on
+[https://github.com/rmontanana/mdlp](https://github.com/rmontanana/mdlp)
```

### Comparing `FImdlp-0.9.3/src/FImdlp.egg-info/SOURCES.txt` & `./Users/rmontanana/.virtualenvs/310/lib/python3.10/site-packages/FImdlp-0.9.4-py3.10.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 src/FImdlp.egg-info/requires.txt
 src/FImdlp.egg-info/top_level.txt
 src/cppmdlp/CPPFImdlp.cpp
 src/cppmdlp/CPPFImdlp.h
 src/cppmdlp/Metrics.cpp
 src/cppmdlp/Metrics.h
 src/cppmdlp/typesFImdlp.h
+src/fimdlp/ArffFiles.cpp
+src/fimdlp/ArffFiles.h
 src/fimdlp/Factorize.cpp
 src/fimdlp/Factorize.h
 src/fimdlp/__init__.py
 src/fimdlp/_version.py
 src/fimdlp/cfimdlp.pyx
 src/fimdlp/mdlp.py
 src/fimdlp/tests/FImdlp_test.py
```

### Comparing `FImdlp-0.9.3/src/cppmdlp/CPPFImdlp.cpp` & `./Users/rmontanana/.virtualenvs/310/lib/python3.10/site-packages/cppmdlp/CPPFImdlp.cpp`

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,81 @@
 #include <numeric>
 #include <algorithm>
 #include <set>
 #include <cmath>
-#include <limits>
 #include "CPPFImdlp.h"
 #include "Metrics.h"
 
 namespace mdlp {
 
-    CPPFImdlp::CPPFImdlp(): indices(indices_t()), X(samples_t()), y(labels_t()),
-        metrics(Metrics(y, indices))
+    CPPFImdlp::CPPFImdlp(size_t min_length_, int max_depth_, float proposed): min_length(min_length_),
+        max_depth(max_depth_),
+        proposed_cuts(proposed)
     {
     }
+
+    CPPFImdlp::CPPFImdlp() = default;
+
     CPPFImdlp::~CPPFImdlp() = default;
 
-    CPPFImdlp& CPPFImdlp::fit(samples_t& X_, labels_t& y_)
+    size_t CPPFImdlp::compute_max_num_cut_points() const
+    {
+        // Set the actual maximum number of cut points as a number or as a percentage of the number of samples
+        if (proposed_cuts == 0) {
+            return numeric_limits<size_t>::max();
+        }
+        if (proposed_cuts < 0 || proposed_cuts > static_cast<float>(X.size())) {
+            throw invalid_argument("wrong proposed num_cuts value");
+        }
+        if (proposed_cuts < 1)
+            return static_cast<size_t>(round(static_cast<float>(X.size()) * proposed_cuts));
+        return static_cast<size_t>(proposed_cuts);
+    }
+
+    void CPPFImdlp::fit(samples_t& X_, labels_t& y_)
     {
         X = X_;
         y = y_;
+        num_cut_points = compute_max_num_cut_points();
+        depth = 0;
         cutPoints.clear();
         if (X.size() != y.size()) {
             throw invalid_argument("X and y must have the same size");
         }
         if (X.empty() || y.empty()) {
             throw invalid_argument("X and y must have at least one element");
         }
+        if (min_length < 3) {
+            throw invalid_argument("min_length must be greater than 2");
+        }
+        if (max_depth < 1) {
+            throw invalid_argument("max_depth must be greater than 0");
+        }
         indices = sortIndices(X_, y_);
         metrics.setData(y, indices);
-        computeCutPoints(0, X.size());
-        return *this;
+        computeCutPoints(0, X.size(), 1);
+        sort(cutPoints.begin(), cutPoints.end());
+        if (num_cut_points > 0) {
+            // Select the best (with lower entropy) cut points
+            while (cutPoints.size() > num_cut_points) {
+                resizeCutPoints();
+            }
+        }
     }
 
     pair<precision_t, size_t> CPPFImdlp::valueCutPoint(size_t start, size_t cut, size_t end)
     {
-        size_t n, m, idxPrev = cut - 1 >= start ? cut - 1 : cut;
+        size_t n;
+        size_t m;
+        size_t idxPrev = cut - 1 >= start ? cut - 1 : cut;
         size_t idxNext = cut + 1 < end ? cut + 1 : cut;
-        bool backWall; // true if duplicates reach begining of the interval
-        precision_t previous, actual, next;
+        bool backWall; // true if duplicates reach beginning of the interval
+        precision_t previous;
+        precision_t actual;
+        precision_t next;
         previous = X[indices[idxPrev]];
         actual = X[indices[cut]];
         next = X[indices[idxNext]];
         // definition 2 of the paper => X[t-1] < X[t]
         // get the first equal value of X in the interval
         while (idxPrev > start && actual == previous) {
             previous = X[indices[--idxPrev]];
@@ -56,106 +91,121 @@
         m = idxNext - cut - 1;
         // Decide which values to use
         cut = cut + (backWall ? m + 1 : -n);
         actual = X[indices[cut]];
         return { (actual + previous) / 2, cut };
     }
 
-    void CPPFImdlp::computeCutPoints(size_t start, size_t end)
+    void CPPFImdlp::computeCutPoints(size_t start, size_t end, int depth_)
     {
         size_t cut;
         pair<precision_t, size_t> result;
-        if (end - start < 3)
+        // Check if the interval length and the depth are Ok
+        if (end - start < min_length || depth_ > max_depth)
             return;
+        depth = depth_ > depth ? depth_ : depth;
         cut = getCandidate(start, end);
         if (cut == numeric_limits<size_t>::max())
             return;
         if (mdlp(start, cut, end)) {
             result = valueCutPoint(start, cut, end);
             cut = result.second;
             cutPoints.push_back(result.first);
-            computeCutPoints(start, cut);
-            computeCutPoints(cut, end);
+            computeCutPoints(start, cut, depth_ + 1);
+            computeCutPoints(cut, end, depth_ + 1);
         }
     }
 
     size_t CPPFImdlp::getCandidate(size_t start, size_t end)
     {
         /* Definition 1: A binary discretization for A is determined by selecting the cut point TA for which
         E(A, TA; S) is minimal amongst all the candidate cut points. */
-        size_t candidate = numeric_limits<size_t>::max(), elements = end - start;
+        size_t candidate = numeric_limits<size_t>::max();
+        size_t elements = end - start;
         bool sameValues = true;
-        precision_t entropy_left, entropy_right, minEntropy;
+        precision_t entropy_left;
+        precision_t entropy_right;
+        precision_t minEntropy;
         // Check if all the values of the variable in the interval are the same
         for (size_t idx = start + 1; idx < end; idx++) {
             if (X[indices[idx]] != X[indices[start]]) {
                 sameValues = false;
                 break;
             }
         }
         if (sameValues)
             return candidate;
         minEntropy = metrics.entropy(start, end);
         for (size_t idx = start + 1; idx < end; idx++) {
             // Cutpoints are always on boundaries (definition 2)
             if (y[indices[idx]] == y[indices[idx - 1]])
                 continue;
-            entropy_left = precision_t(idx - start) / elements * metrics.entropy(start, idx);
-            entropy_right = precision_t(end - idx) / elements * metrics.entropy(idx, end);
+            entropy_left = precision_t(idx - start) / static_cast<precision_t>(elements) * metrics.entropy(start, idx);
+            entropy_right = precision_t(end - idx) / static_cast<precision_t>(elements) * metrics.entropy(idx, end);
             if (entropy_left + entropy_right < minEntropy) {
                 minEntropy = entropy_left + entropy_right;
                 candidate = idx;
             }
         }
         return candidate;
     }
 
     bool CPPFImdlp::mdlp(size_t start, size_t cut, size_t end)
     {
-        int k, k1, k2;
-        precision_t ig, delta;
-        precision_t ent, ent1, ent2;
+        int k;
+        int k1;
+        int k2;
+        precision_t ig;
+        precision_t delta;
+        precision_t ent;
+        precision_t ent1;
+        precision_t ent2;
         auto N = precision_t(end - start);
-        if (N < 2) {
-            return false;
-        }
         k = metrics.computeNumClasses(start, end);
         k1 = metrics.computeNumClasses(start, cut);
         k2 = metrics.computeNumClasses(cut, end);
         ent = metrics.entropy(start, end);
         ent1 = metrics.entropy(start, cut);
         ent2 = metrics.entropy(cut, end);
         ig = metrics.informationGain(start, cut, end);
-        delta = log2(pow(3, precision_t(k)) - 2) -
-            (precision_t(k) * ent - precision_t(k1) * ent1 - precision_t(k2) * ent2);
+        delta = static_cast<precision_t>(log2(pow(3, precision_t(k)) - 2) -
+            (precision_t(k) * ent - precision_t(k1) * ent1 - precision_t(k2) * ent2));
         precision_t term = 1 / N * (log2(N - 1) + delta);
         return ig > term;
     }
 
     // Argsort from https://stackoverflow.com/questions/1577475/c-sorting-and-keeping-track-of-indexes
     indices_t CPPFImdlp::sortIndices(samples_t& X_, labels_t& y_)
     {
         indices_t idx(X_.size());
         iota(idx.begin(), idx.end(), 0);
-        for (size_t i = 0; i < X_.size(); i++)
-            stable_sort(idx.begin(), idx.end(), [&X_, &y_](size_t i1, size_t i2) {
+        stable_sort(idx.begin(), idx.end(), [&X_, &y_](size_t i1, size_t i2) {
             if (X_[i1] == X_[i2])
                 return y_[i1] < y_[i2];
             else
                 return X_[i1] < X_[i2];
-                });
+            });
         return idx;
     }
 
-    cutPoints_t CPPFImdlp::getCutPoints()
+    void CPPFImdlp::resizeCutPoints()
     {
-        // Remove duplicates and sort
-        cutPoints_t output(cutPoints.size());
-        set<precision_t> s;
-        unsigned size = cutPoints.size();
-        for (unsigned i = 0; i < size; i++)
-            s.insert(cutPoints[i]);
-        output.assign(s.begin(), s.end());
-        sort(output.begin(), output.end());
-        return output;
+        //Compute entropy of each of the whole cutpoint set and discards the biggest value
+        precision_t maxEntropy = 0;
+        precision_t entropy;
+        size_t maxEntropyIdx = 0;
+        size_t begin = 0;
+        size_t end;
+        for (size_t idx = 0; idx < cutPoints.size(); idx++) {
+            end = begin;
+            while (X[indices[end]] < cutPoints[idx] && end < X.size())
+                end++;
+            entropy = metrics.entropy(begin, end);
+            if (entropy > maxEntropy) {
+                maxEntropy = entropy;
+                maxEntropyIdx = idx;
+            }
+            begin = end;
+        }
+        cutPoints.erase(cutPoints.begin() + static_cast<long>(maxEntropyIdx));
     }
 }
```

### Comparing `FImdlp-0.9.3/src/cppmdlp/Metrics.cpp` & `./Users/rmontanana/.virtualenvs/310/lib/python3.10/site-packages/cppmdlp/Metrics.cpp`

 * *Files 24% similar despite different names*

```diff
@@ -1,65 +1,78 @@
 #include "Metrics.h"
 #include <set>
 #include <cmath>
+
 using namespace std;
 namespace mdlp {
-    Metrics::Metrics(labels_t& y_, indices_t& indices_): y(y_), indices(indices_), numClasses(computeNumClasses(0, indices.size())), entropyCache(cacheEnt_t()), igCache(cacheIg_t())
+    Metrics::Metrics(labels_t& y_, indices_t& indices_): y(y_), indices(indices_),
+        numClasses(computeNumClasses(0, indices.size()))
     {
     }
+
     int Metrics::computeNumClasses(size_t start, size_t end)
     {
         set<int> nClasses;
         for (auto i = start; i < end; ++i) {
             nClasses.insert(y[indices[i]]);
         }
-        return nClasses.size();
+        return static_cast<int>(nClasses.size());
     }
-    void Metrics::setData(labels_t& y_, indices_t& indices_)
+
+    void Metrics::setData(const labels_t& y_, const indices_t& indices_)
     {
         indices = indices_;
         y = y_;
         numClasses = computeNumClasses(0, indices.size());
         entropyCache.clear();
         igCache.clear();
     }
+
     precision_t Metrics::entropy(size_t start, size_t end)
     {
-        precision_t p, ventropy = 0;
+        precision_t p;
+        precision_t ventropy = 0;
         int nElements = 0;
         labels_t counts(numClasses + 1, 0);
         if (end - start < 2)
             return 0;
         if (entropyCache.find({ start, end }) != entropyCache.end()) {
             return entropyCache[{start, end}];
         }
         for (auto i = &indices[start]; i != &indices[end]; ++i) {
             counts[y[*i]]++;
             nElements++;
         }
         for (auto count : counts) {
             if (count > 0) {
-                p = (precision_t)count / nElements;
+                p = static_cast<precision_t>(count) / static_cast<precision_t>(nElements);
                 ventropy -= p * log2(p);
             }
         }
         entropyCache[{start, end}] = ventropy;
         return ventropy;
     }
+
     precision_t Metrics::informationGain(size_t start, size_t cut, size_t end)
     {
         precision_t iGain;
-        precision_t entropyInterval, entropyLeft, entropyRight;
-        int nElementsLeft = cut - start, nElementsRight = end - cut;
-        int nElements = end - start;
+        precision_t entropyInterval;
+        precision_t entropyLeft;
+        precision_t entropyRight;
+        size_t nElementsLeft = cut - start;
+        size_t nElementsRight = end - cut;
+        size_t nElements = end - start;
         if (igCache.find(make_tuple(start, cut, end)) != igCache.end()) {
             return igCache[make_tuple(start, cut, end)];
         }
         entropyInterval = entropy(start, end);
         entropyLeft = entropy(start, cut);
         entropyRight = entropy(cut, end);
-        iGain = entropyInterval - ((precision_t)nElementsLeft * entropyLeft + (precision_t)nElementsRight * entropyRight) / nElements;
+        iGain = entropyInterval -
+            (static_cast<precision_t>(nElementsLeft) * entropyLeft +
+                static_cast<precision_t>(nElementsRight) * entropyRight) /
+            static_cast<precision_t>(nElements);
         igCache[make_tuple(start, cut, end)] = iGain;
         return iGain;
     }
 
 }
```

### Comparing `FImdlp-0.9.3/src/cppmdlp/Metrics.h` & `./Users/rmontanana/.virtualenvs/310/lib/python3.10/site-packages/cppmdlp/Metrics.h`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 #ifndef CCMETRICS_H
 #define CCMETRICS_H
+
 #include "typesFImdlp.h"
+
 namespace mdlp {
     class Metrics {
     protected:
         labels_t& y;
         indices_t& indices;
         int numClasses;
-        cacheEnt_t entropyCache;
-        cacheIg_t igCache;
+        cacheEnt_t entropyCache = cacheEnt_t();
+        cacheIg_t igCache = cacheIg_t();
     public:
         Metrics(labels_t&, indices_t&);
-        void setData(labels_t&, indices_t&);
+        void setData(const labels_t&, const indices_t&);
         int computeNumClasses(size_t, size_t);
         precision_t entropy(size_t, size_t);
         precision_t informationGain(size_t, size_t, size_t);
     };
 }
 #endif
```

### Comparing `FImdlp-0.9.3/src/fimdlp/mdlp.py` & `./Users/rmontanana/.virtualenvs/310/lib/python3.10/site-packages/fimdlp/mdlp.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,29 +2,36 @@
 from .cppfimdlp import CFImdlp, factorize
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.utils.multiclass import unique_labels
 from sklearn.utils.validation import check_X_y, check_array, check_is_fitted
 from joblib import Parallel, delayed
 from ._version import __version__
 
-# from ._version import __version__
-
 
 class FImdlp(TransformerMixin, BaseEstimator):
-    def __init__(self, n_jobs=-1):
+    def __init__(self, n_jobs=-1, min_length=3, max_depth=1e6, max_cuts=0):
         self.n_jobs = n_jobs
+        self.min_length = min_length
+        self.max_depth = max_depth
+        self.max_cuts = max_cuts
 
     """Fayyad - Irani MDLP discretization algorithm based implementation.
 
     Parameters
     ----------
     n_jobs : int, default=-1
         The number of jobs to run in parallel. :meth:`fit` and
         :meth:`transform`, are parallelized over the features. ``-1`` means
         using all cores available.
+    min_length: int, default=3
+        The minimum length of an interval to be considered to be discretized.
+    max_depth: int, default=1e6
+        The maximum depth of the discretization process.
+    max_cuts: float, default=0
+        The maximum number of cut points to be computed for each feature.
 
     Attributes
     ----------
     n_features_in_ : int
         The number of features of the data passed to :meth:`fit`.
     discretizer_ : list
         The list of discretizers, one for each feature.
@@ -91,25 +98,36 @@
         """
         X, y = self._check_args(
             X, y, expected_args=["features"], kwargs=kwargs
         )
         self._update_params(X, y)
         self.X_ = X
         self.y_ = y
+        self.efective_min_length_ = (
+            self.min_length
+            if self.min_length > 1
+            else int(self.min_length * X.shape[0])
+        )
         self.discretizer_ = [None] * self.n_features_in_
         self.cut_points_ = [None] * self.n_features_in_
         Parallel(n_jobs=self.n_jobs, prefer="threads")(
             delayed(self._fit_discretizer)(feature)
             for feature in range(self.n_features_in_)
         )
+        # target of every feature. Start with -1 => y (see join_fit)
+        self.target_ = [-1] * self.n_features_in_
         return self
 
     def _fit_discretizer(self, feature):
         if feature in self.features_:
-            self.discretizer_[feature] = CFImdlp()
+            self.discretizer_[feature] = CFImdlp(
+                min_length=self.efective_min_length_,
+                max_depth=self.max_depth,
+                max_cuts=self.max_cuts,
+            )
             self.discretizer_[feature].fit(self.X_[:, feature], self.y_)
             self.cut_points_[feature] = self.discretizer_[
                 feature
             ].get_cut_points()
         else:
             self.discretizer_[feature] = None
             self.cut_points_[feature] = []
@@ -228,17 +246,25 @@
                     f"{self.n_features_in_})"
                 )
         if target < 0 or target >= self.n_features_in_:
             raise ValueError(
                 f"Target {target} not in range [0, {self.n_features_in_})"
             )
         if target in features:
-            raise ValueError("Target cannot in features to join")
+            raise ValueError("Target cannot be in features to join")
         y_join = [
             f"{str(item_y)}{''.join([str(x) for x in items_x])}".encode()
             for item_y, items_x in zip(self.y_, data[:, features])
         ]
+        # Store in target_ the features used with class to discretize target
+        self.target_[target] = features + [-1]
         self.y_join_ = y_join
         self.discretizer_[target].fit(self.X_[:, target], factorize(y_join))
         self.cut_points_[target] = self.discretizer_[target].get_cut_points()
         # return the discretized target variable with the new cut points
         return np.searchsorted(self.cut_points_[target], self.X_[:, target])
+
+    def get_depths(self):
+        res = [0] * self.n_features_in_
+        for feature in self.features_:
+            res[feature] = self.discretizer_[feature].get_depth()
+        return res
```

### Comparing `FImdlp-0.9.3/src/fimdlp/tests/FImdlp_test.py` & `./Users/rmontanana/.virtualenvs/310/lib/python3.10/site-packages/fimdlp/tests/FImdlp_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,61 @@
 import unittest
 import sklearn
 import numpy as np
 from sklearn.datasets import load_iris
 from sklearn.utils.estimator_checks import check_estimator
-from ..cppfimdlp import CFImdlp, factorize
+from ..cppfimdlp import CFImdlp, factorize, CArffFiles
 from ..mdlp import FImdlp
 from .. import __version__
 
-# from .._version import __version__
-
 
 class FImdlpTest(unittest.TestCase):
+    delta = 1e-6  # same tolerance as in C++ code
+
     def test_version(self):
         clf = FImdlp()
         self.assertEqual(
             clf.get_version(),
             f"{__version__}({CFImdlp().get_version().decode()})",
         )
 
+    def test_minimum_mdlp_version(self):
+        mdlp_version = tuple(
+            int(c) for c in CFImdlp().get_version().decode().split(".")[0:3]
+        )
+        minimum_mdlp_version = (1, 1, 2)
+        self.assertTrue(mdlp_version >= minimum_mdlp_version)
+
     def test_init(self):
         clf = FImdlp()
         self.assertEqual(-1, clf.n_jobs)
-        clf = FImdlp(n_jobs=7)
+        self.assertEqual(3, clf.min_length)
+        self.assertEqual(1e6, clf.max_depth)
+        clf = FImdlp(n_jobs=7, min_length=24, max_depth=17)
         self.assertEqual(7, clf.n_jobs)
+        self.assertEqual(24, clf.min_length)
+        self.assertEqual(17, clf.max_depth)
 
     def test_fit_definitive(self):
         clf = FImdlp()
         X, y = load_iris(return_X_y=True)
         clf.fit(X, y)
         self.assertEqual(clf.n_features_in_, 4)
         self.assertTrue(np.array_equal(X, clf.X_))
         self.assertTrue(np.array_equal(y, clf.y_))
         expected = [
-            [5.449999809265137, 5.75],
-            [2.75, 2.8499999046325684, 2.95, 3.05, 3.3499999046325684],
-            [2.45, 4.75, 5.050000190734863],
+            [5.45, 5.75],
+            [2.75, 2.85, 2.95, 3.05, 3.35],
+            [2.45, 4.75, 5.05],
             [0.8, 1.75],
         ]
         computed = clf.get_cut_points()
         for item_computed, item_expected in zip(computed, expected):
             for x_, y_ in zip(item_computed, item_expected):
-                self.assertAlmostEqual(x_, y_)
+                self.assertAlmostEqual(x_, y_, delta=self.delta)
         self.assertListEqual([0, 1, 2, 3], clf.features_)
         clf.fit(X, y, features=[0, 2, 3])
         self.assertListEqual([0, 2, 3], clf.features_)
 
     def test_fit_Errors(self):
         clf = FImdlp()
         with self.assertRaises(ValueError):
@@ -128,30 +139,40 @@
             b"f8",
         ]
         expected = [0, 1, 2, 3, 4, 5, 6, 1, 1, 7, 8]
         computed = factorize(source)
         self.assertListEqual(expected, computed)
 
     def test_join_fit(self):
-        y = np.array([b"f0", b"f0", b"f2", b"f3", b"f4"])
+        y = np.array([b"f0", b"f0", b"f2", b"f3", b"f3", b"f4", b"f4"])
         x = np.array(
             [
-                [0, 1, 2, 3, 4],
-                [0, 1, 2, 3, 4],
-                [1, 2, 3, 4, 5],
-                [2, 3, 4, 5, 6],
-                [3, 4, 5, 6, 7],
+                [0, 1, 2, 3, 4, 5],
+                [0, 2, 2, 3, 4, 5],
+                [1, 2, 3, 4, 5, 5],
+                [2, 3, 4, 5, 6, 6],
+                [3, 4, 5, 6, 7, 7],
+                [1, 2, 2, 3, 5, 7],
+                [1, 3, 4, 4, 4, 7],
             ]
         )
-        expected = [0, 0, 1, 2, 2]
+        expected = [0, 1, 1, 2, 2, 1, 2]
         clf = FImdlp()
         clf.fit(x, factorize(y))
-        computed = clf.join_fit([0, 2], 1, x)
+        computed = clf.join_fit([0, 2, 3, 4], 1, x)
         self.assertListEqual(computed.tolist(), expected)
-        expected_y = [b"002", b"002", b"113", b"224", b"335"]
+        expected_y = [
+            b"00234",
+            b"00234",
+            b"11345",
+            b"22456",
+            b"23567",
+            b"31235",
+            b"31444",
+        ]
         self.assertListEqual(expected_y, clf.y_join_)
 
     def test_join_fit_error(self):
         y = np.array([b"f0", b"f0", b"f2", b"f3", b"f4"])
         x = np.array(
             [
                 [0, 1, 2, 3, 4],
@@ -188,27 +209,37 @@
             str(exception.exception),
             "Target 5 not in range [0, 5)",
         )
         with self.assertRaises(ValueError) as exception:
             clf.join_fit([0, 2], 2, x)
         self.assertEqual(
             str(exception.exception),
-            "Target cannot in features to join",
+            "Target cannot be in features to join",
         )
 
     def test_factorize(self):
         y = np.array([b"f0", b"f0", b"f2", b"f3", b"f4"])
         clf = FImdlp()
         computed = clf.factorize(y)
         self.assertListEqual([0, 0, 1, 2, 3], computed)
         y = [b"f4", b"f0", b"f0", b"f2", b"f3"]
         clf = FImdlp()
         computed = clf.factorize(y)
         self.assertListEqual([0, 1, 1, 2, 3], computed)
 
+    def test_join_fit_info(self):
+        clf = FImdlp()
+        X, y = load_iris(return_X_y=True)
+        clf.fit(X, y)
+        clf.join_fit([0, 2], 1, X)
+        clf.join_fit([0, 3], 2, X)
+        clf.join_fit([1, 2], 3, X)
+        expected = [-1, [0, 2, -1], [0, 3, -1], [1, 2, -1]]
+        self.assertListEqual(expected, clf.target_)
+
     @staticmethod
     def test_sklearn_transformer():
         for check, test in check_estimator(FImdlp(), generate_only=True):
             test(check)
 
     def test_states_feature(self):
         clf = FImdlp()
@@ -223,7 +254,114 @@
             )
 
     def test_states_no_feature(self):
         clf = FImdlp()
         X, y = load_iris(return_X_y=True)
         clf.fit(X, y)
         self.assertIsNone(clf.get_states_feature(4))
+
+    def test_MaxDepth(self):
+        clf = FImdlp(max_depth=1)
+        X, y = load_iris(return_X_y=True)
+        clf.fit(X, y)
+        expected_cutpoints = [
+            [5.45],
+            [3.35],
+            [2.45],
+            [0.8],
+        ]
+        expected_depths = [1] * 4
+        self.assertListEqual(expected_depths, clf.get_depths())
+        for expected, computed in zip(
+            expected_cutpoints, clf.get_cut_points()
+        ):
+            for e, c in zip(expected, computed):
+                self.assertAlmostEqual(e, c, delta=self.delta)
+
+    def test_MinLength(self):
+        clf = FImdlp(min_length=75)
+        X, y = load_iris(return_X_y=True)
+        clf.fit(X, y)
+        expected_cutpoints = [
+            [5.45, 5.75],
+            [2.85, 3.35],
+            [2.45, 4.75],
+            [0.8, 1.75],
+        ]
+        expected_depths = [3, 2, 2, 2]
+        self.assertListEqual(expected_depths, clf.get_depths())
+        for expected, computed in zip(
+            expected_cutpoints, clf.get_cut_points()
+        ):
+            for e, c in zip(expected, computed):
+                self.assertAlmostEqual(e, c, delta=self.delta)
+
+    def test_MinLengthMaxDepth(self):
+        clf = FImdlp(min_length=75, max_depth=2)
+        X, y = load_iris(return_X_y=True)
+        clf.fit(X, y)
+        expected_cutpoints = [
+            [5.45, 5.75],
+            [2.85, 3.35],
+            [2.45, 4.75],
+            [0.8, 1.75],
+        ]
+        expected_depths = [2, 2, 2, 2]
+        self.assertListEqual(expected_depths, clf.get_depths())
+        for expected, computed in zip(
+            expected_cutpoints, clf.get_cut_points()
+        ):
+            for e, c in zip(expected, computed):
+                self.assertAlmostEqual(e, c, delta=self.delta)
+
+    def test_max_cuts(self):
+        clf = FImdlp(max_cuts=1)
+        X, y = load_iris(return_X_y=True)
+        clf.fit(X, y)
+        expected_cutpoints = [
+            [5.45],
+            [2.85],
+            [2.45],
+            [0.8],
+        ]
+        expected_depths = [3, 5, 4, 3]
+        self.assertListEqual(expected_depths, clf.get_depths())
+        for expected, computed in zip(
+            expected_cutpoints, clf.get_cut_points()
+        ):
+            for e, c in zip(expected, computed):
+                self.assertAlmostEqual(e, c, delta=self.delta)
+
+    def test_ArffFiles(self):
+        loader = CArffFiles()
+        loader.load(b"src/cppmdlp/tests/datasets/iris.arff")
+        X = loader.get_X()
+        y = loader.get_y()
+        expected = [
+            (b"sepallength", b"REAL"),
+            (b"sepalwidth", b"REAL"),
+            (b"petallength", b"REAL"),
+            (b"petalwidth", b"REAL"),
+        ]
+        self.assertListEqual(loader.get_attributes(), expected)
+        self.assertListEqual(y[:10], [0, 0, 0, 0, 0, 0, 0, 0, 0, 0])
+        expected = [
+            b"5.1,3.5,1.4,0.2,Iris-setosa",
+            b"4.9,3.0,1.4,0.2,Iris-setosa",
+            b"4.7,3.2,1.3,0.2,Iris-setosa",
+            b"4.6,3.1,1.5,0.2,Iris-setosa",
+            b"5.0,3.6,1.4,0.2,Iris-setosa",
+            b"5.4,3.9,1.7,0.4,Iris-setosa",
+            b"4.6,3.4,1.4,0.3,Iris-setosa",
+            b"5.0,3.4,1.5,0.2,Iris-setosa",
+            b"4.4,2.9,1.4,0.2,Iris-setosa",
+            b"4.9,3.1,1.5,0.1,Iris-setosa",
+        ]
+        self.assertListEqual(loader.get_lines()[:10], expected)
+        expected_X = [
+            [5.0999999, 3.5, 1.39999998, 0.2],
+            [4.9000001, 3, 1.39999998, 0.2],
+            [4.69999981, 3.20000005, 1.29999995, 0.2],
+        ]
+        for computed, expected in zip(X[:3].tolist(), expected_X):
+            for c, e in zip(computed, expected):
+                self.assertAlmostEqual(c, e, delta=self.delta)
```

