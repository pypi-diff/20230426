# Comparing `tmp/colomoto_jupyter-0.8.5.tar.gz` & `tmp/colomoto_jupyter-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colomoto_jupyter-0.8.5.tar", last modified: Fri Apr  7 21:52:20 2023, max compression
+gzip compressed data, was "colomoto_jupyter-0.8.6.tar", last modified: Wed Apr 26 10:33:42 2023, max compression
```

## Comparing `colomoto_jupyter-0.8.5.tar` & `colomoto_jupyter-0.8.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:52:20.987387 colomoto_jupyter-0.8.5/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-07 21:52:20.987387 colomoto_jupyter-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/cellcollective.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:52:20.987387 colomoto_jupyter-0.8.5/colomoto/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/colomoto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/colomoto/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    26534 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/colomoto/minibn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/colomoto/modelchecking.py
--rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/colomoto/setup_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/colomoto/temporal_logics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/colomoto/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:52:20.987387 colomoto_jupyter-0.8.5/colomoto_jupyter/
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/colomoto_jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/colomoto_jupyter/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/colomoto_jupyter/formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/colomoto_jupyter/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    11789 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/colomoto_jupyter/jupyter_ext.js
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/colomoto_jupyter/sessionfiles.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/colomoto_jupyter/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/colomoto_jupyter/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/colomoto_jupyter/widget_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/colomoto_jupyter/wui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:52:20.987387 colomoto_jupyter-0.8.5/colomoto_jupyter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-07 21:52:20.000000 colomoto_jupyter-0.8.5/colomoto_jupyter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-07 21:52:20.000000 colomoto_jupyter-0.8.5/colomoto_jupyter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 21:52:20.000000 colomoto_jupyter-0.8.5/colomoto_jupyter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-07 21:52:20.000000 colomoto_jupyter-0.8.5/colomoto_jupyter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-07 21:52:20.000000 colomoto_jupyter-0.8.5/colomoto_jupyter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/espresso_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/itstools.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/itstools_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/nusmv.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-07 21:52:12.000000 colomoto_jupyter-0.8.5/nusmv_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 21:52:20.987387 colomoto_jupyter-0.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-07 21:52:13.000000 colomoto_jupyter-0.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:33:42.358047 colomoto_jupyter-0.8.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-26 10:33:42.358047 colomoto_jupyter-0.8.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/cellcollective.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:33:42.354047 colomoto_jupyter-0.8.6/colomoto/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/colomoto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/colomoto/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27199 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/colomoto/minibn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/colomoto/modelchecking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/colomoto/setup_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/colomoto/temporal_logics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/colomoto/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:33:42.358047 colomoto_jupyter-0.8.6/colomoto_jupyter/
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/colomoto_jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/colomoto_jupyter/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/colomoto_jupyter/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/colomoto_jupyter/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11789 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/colomoto_jupyter/jupyter_ext.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/colomoto_jupyter/sessionfiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/colomoto_jupyter/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/colomoto_jupyter/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/colomoto_jupyter/widget_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/colomoto_jupyter/wui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:33:42.358047 colomoto_jupyter-0.8.6/colomoto_jupyter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-26 10:33:42.000000 colomoto_jupyter-0.8.6/colomoto_jupyter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-26 10:33:42.000000 colomoto_jupyter-0.8.6/colomoto_jupyter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 10:33:42.000000 colomoto_jupyter-0.8.6/colomoto_jupyter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-26 10:33:42.000000 colomoto_jupyter-0.8.6/colomoto_jupyter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-26 10:33:42.000000 colomoto_jupyter-0.8.6/colomoto_jupyter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/espresso_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/itstools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/itstools_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/nusmv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/nusmv_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 10:33:42.358047 colomoto_jupyter-0.8.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-26 10:33:31.000000 colomoto_jupyter-0.8.6/setup.py
```

### Comparing `colomoto_jupyter-0.8.5/PKG-INFO` & `colomoto_jupyter-0.8.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colomoto_jupyter
-Version: 0.8.5
+Version: 0.8.6
 Summary: CoLoMoTo helper functions for Juypter integration
 Home-page: https://github.com/colomoto/colomoto-jupyter
 Author: Loïc Paulevé
 Author-email: loic.pauleve@ens-cachan.org
 License: LGPL v3+/CeCILL-C
 Keywords: jupyter,computational systems biology
 Classifier: Intended Audience :: Science/Research
```

### Comparing `colomoto_jupyter-0.8.5/README.md` & `colomoto_jupyter-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.5/cellcollective.py` & `colomoto_jupyter-0.8.6/cellcollective.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.5/colomoto/helpers.py` & `colomoto_jupyter-0.8.6/colomoto/helpers.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.5/colomoto/minibn.py` & `colomoto_jupyter-0.8.6/colomoto/minibn.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,36 +15,36 @@
 from colomoto.types import HypercubeCollection
 from colomoto_jupyter import import_colomoto_tool
 from colomoto_jupyter.io import ensure_localfile
 from colomoto_jupyter.sessionfiles import new_output_file
 from colomoto_jupyter import IN_IPYTHON, jupyter_setup
 
 import boolean
+import boolean.boolean as bpy
 
 re_nonword = re.compile(r"\W", flags=re.A)
 
 if IN_IPYTHON:
     jupyter_setup("minibn", label="miniBN")
 
-class NOT(boolean.NOT):
+class NOT(bpy.NOT):
     def __init__(self, *args):
         super().__init__(*args)
         self.operator = "!"
 
-import boolean.boolean as bpy
-
 class _TRUE(bpy._TRUE):
     def __call__(self, **kw):
         return self if not kw else True
 
-
 class _FALSE(bpy._FALSE):
     def __call__(self, **kw):
         return self if not kw else False
 
+def is_constant(f):
+    return isinstance(f, (bpy._TRUE,bpy._FALSE))
 
 class BaseNetwork(dict):
     def __init__(self, data=None, Symbol_class=boolean.Symbol,
             allowed_in_name=('.','_',':','-'), **kwargs):
         super().__init__()
         self.ba = boolean.BooleanAlgebra(NOT_class=NOT,
             TRUE_class=_TRUE,
@@ -303,21 +303,28 @@
                 left = line[:sep].strip()
                 right = line[sep+2:].strip()
             if header is None and (left, right) == ("targets", "factors"):
                 header = True
                 continue
             self[left] = self.ba.parse(right)
 
-    def simplify(self):
-        bn = copy.copy(self)
+    def simplify(self, in_place=False, suspect_dnf=True):
+        """
+        if in_place, modifies the network in place, otherwise works on a copy
+        returns it.
+        if suspect_dnf, try harder simplifications for functions that are in DNF and have literals with
+        opposite signs in clauses (will make CNF and DNF transformations).
+        """
+        bn = self if in_place else copy.copy(self)
         for a, f in bn.items():
             f = f.simplify()
-            f = simplify_dnf(self.ba, f)
+            if suspect_dnf:
+                f = simplify_dnf(self.ba, f)
             bn[a] = f
-        return bn
+        return bn if not in_place else None
 
     def as_dnf(self):
         def make_lit(l):
             if isinstance(l, self.ba.NOT):
                 return (l.args[0].obj, False)
             else:
                 return (l.obj, True)
@@ -370,34 +377,35 @@
                     sign = 1
                 influences.add((b,a,sign))
         for (b, a, sign) in influences:
             ig.add_edge(b, a, sign=sign, label="+" if sign > 0 else "-")
         return ig
 
     def constants(self):
-        csttypes = [boolean.boolean._TRUE, boolean.boolean._FALSE]
-        return {i:f is self.ba.TRUE for i,f in self.items() \
-                if type(f) in csttypes}
+        return {i: f for i,f in self.items() if is_constant(f)}
 
     def propagate_constants(self):
-        csttypes = [boolean.boolean._TRUE, boolean.boolean._FALSE]
-        bn = self.copy()
-        csts = {i:f for i, f in bn.items() if type(f) in csttypes}
+        """
+        For each node having a constant function, replace references to that
+            node by the constant in the expression of all the other nodes.
+        Performs simple function simplification.
+        Modifies the Boolean network in-place.
+        The set of constant nodes can be accessed with the `constants()` method.
+        """
+        csts = {self.v(i): self.ba.TRUE if bool(f) else self.ba.FALSE
+                    for i, f in self.constants().items()}
         while csts:
             new_csts = {}
-            for a in bn.keys():
-                if a in csts:
-                    continue
-                bn.rewrite(a, csts)
-                if type(bn[a]) in csttypes:
-                    new_csts[a] = bn[a]
-            for a in csts:
-                del bn[a]
+            for a, fa, in self.items():
+                if not is_constant(fa):
+                    fa = fa.subs(csts).simplify()
+                    self[a] = fa
+                    if is_constant(fa):
+                        new_csts[self.v(a)] = fa
             csts = new_csts
-        return bn
 
     def to_pint(self):
         pypint = import_colomoto_tool("pypint")
         from pypint.converters import import_minibn
         return import_minibn(self)
 
     def to_pyboolnet(self):
```

### Comparing `colomoto_jupyter-0.8.5/colomoto/modelchecking.py` & `colomoto_jupyter-0.8.6/colomoto/modelchecking.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.5/colomoto/setup_helper.py` & `colomoto_jupyter-0.8.6/colomoto/setup_helper.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.5/colomoto/temporal_logics.py` & `colomoto_jupyter-0.8.6/colomoto/temporal_logics.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,17 +135,17 @@
                 return arg
             else:
                 return "{} ({})".format(op, arg)
         elif isinstance(e, BinaryOperator):
             right = to_its(e.right)
             left = to_its(e.left)
             if isinstance(e, And):
-                tmpl = "({}) && ({})"
+                tmpl = "({})&&({})"
             elif isinstance(e, Or):
-                tmpl = "({}) || ({})"
+                tmpl = "({})||({})"
             elif isinstance(e, If):
                 tmpl = "({}) -> ({})"
             elif isinstance(e, EU):
                 tmpl = "E(({}) U ({}))"
             elif isinstance(e, AU):
                 tmpl = "A(({}) U ({}))"
             return tmpl.format(left, right)
```

### Comparing `colomoto_jupyter-0.8.5/colomoto/types.py` & `colomoto_jupyter-0.8.6/colomoto/types.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.5/colomoto_jupyter/__init__.py` & `colomoto_jupyter-0.8.6/colomoto_jupyter/__init__.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.5/colomoto_jupyter/formatters.py` & `colomoto_jupyter-0.8.6/colomoto_jupyter/formatters.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.5/colomoto_jupyter/io.py` & `colomoto_jupyter-0.8.6/colomoto_jupyter/io.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.5/colomoto_jupyter/jupyter_ext.js` & `colomoto_jupyter-0.8.6/colomoto_jupyter/jupyter_ext.js`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.5/colomoto_jupyter/sessionfiles.py` & `colomoto_jupyter-0.8.6/colomoto_jupyter/sessionfiles.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.5/colomoto_jupyter/upload.py` & `colomoto_jupyter-0.8.6/colomoto_jupyter/upload.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.5/colomoto_jupyter/widget_utils.py` & `colomoto_jupyter-0.8.6/colomoto_jupyter/widget_utils.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.5/colomoto_jupyter/wui.py` & `colomoto_jupyter-0.8.6/colomoto_jupyter/wui.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.5/colomoto_jupyter.egg-info/PKG-INFO` & `colomoto_jupyter-0.8.6/colomoto_jupyter.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colomoto-jupyter
-Version: 0.8.5
+Version: 0.8.6
 Summary: CoLoMoTo helper functions for Juypter integration
 Home-page: https://github.com/colomoto/colomoto-jupyter
 Author: Loïc Paulevé
 Author-email: loic.pauleve@ens-cachan.org
 License: LGPL v3+/CeCILL-C
 Keywords: jupyter,computational systems biology
 Classifier: Intended Audience :: Science/Research
```

### Comparing `colomoto_jupyter-0.8.5/colomoto_jupyter.egg-info/SOURCES.txt` & `colomoto_jupyter-0.8.6/colomoto_jupyter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.5/itstools.py` & `colomoto_jupyter-0.8.6/itstools.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.5/nusmv.py` & `colomoto_jupyter-0.8.6/nusmv.py`

 * *Files identical despite different names*

### Comparing `colomoto_jupyter-0.8.5/setup.py` & `colomoto_jupyter-0.8.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf8 -*-
 
 from setuptools import setup, find_packages
 
 NAME = "colomoto_jupyter"
 
 setup(name=NAME,
-    version='0.8.5',
+    version='0.8.6',
     author = "Loïc Paulevé",
     author_email = "loic.pauleve@ens-cachan.org",
     url = "https://github.com/colomoto/colomoto-jupyter",
     description = "CoLoMoTo helper functions for Juypter integration",
     long_description = """
 Provides helper functions for integration in the CoLoMoTo Jupyter notebook.
```

