# Comparing `tmp/pyransame-0.0.3.tar.gz` & `tmp/pyransame-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyransame-0.0.3.tar", last modified: Sat Apr 15 11:54:14 2023, max compression
+gzip compressed data, was "pyransame-0.0.4.tar", last modified: Wed Apr 26 16:22:29 2023, max compression
```

## Comparing `pyransame-0.0.3.tar` & `pyransame-0.0.4.tar`

### file list

```diff
@@ -1,36 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:54:14.727579 pyransame-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:54:14.727579 pyransame-0.0.3/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-15 11:54:02.000000 pyransame-0.0.3/.devcontainer/devcontainer.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      208 2023-04-15 11:54:02.000000 pyransame-0.0.3/.devcontainer/oncreatecommand.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:54:14.723579 pyransame-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:54:14.727579 pyransame-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-15 11:54:02.000000 pyransame-0.0.3/.github/workflows/pages_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-15 11:54:02.000000 pyransame-0.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-15 11:54:02.000000 pyransame-0.0.3/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-15 11:54:02.000000 pyransame-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-15 11:54:02.000000 pyransame-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-15 11:54:14.727579 pyransame-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-15 11:54:02.000000 pyransame-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:54:14.727579 pyransame-0.0.3/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-15 11:54:02.000000 pyransame-0.0.3/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-15 11:54:02.000000 pyransame-0.0.3/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-04-15 11:54:02.000000 pyransame-0.0.3/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-15 11:54:02.000000 pyransame-0.0.3/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-15 11:54:02.000000 pyransame-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-15 11:54:02.000000 pyransame-0.0.3/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-15 11:54:02.000000 pyransame-0.0.3/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 11:54:14.727579 pyransame-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:54:14.723579 pyransame-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:54:14.727579 pyransame-0.0.3/src/pyransame/
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-15 11:54:02.000000 pyransame-0.0.3/src/pyransame/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-15 11:54:14.000000 pyransame-0.0.3/src/pyransame/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-15 11:54:02.000000 pyransame-0.0.3/src/pyransame/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:54:14.727579 pyransame-0.0.3/src/pyransame.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-15 11:54:14.000000 pyransame-0.0.3/src/pyransame.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-15 11:54:14.000000 pyransame-0.0.3/src/pyransame.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 11:54:14.000000 pyransame-0.0.3/src/pyransame.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-15 11:54:14.000000 pyransame-0.0.3/src/pyransame.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-15 11:54:14.000000 pyransame-0.0.3/src/pyransame.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 11:54:14.727579 pyransame-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-04-15 11:54:02.000000 pyransame-0.0.3/tests/test_random_surface_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-15 11:54:02.000000 pyransame-0.0.3/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:22:29.287916 pyransame-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:22:29.283916 pyransame-0.0.4/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-26 16:22:15.000000 pyransame-0.0.4/.devcontainer/devcontainer.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      253 2023-04-26 16:22:15.000000 pyransame-0.0.4/.devcontainer/oncreatecommand.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:22:29.283916 pyransame-0.0.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-26 16:22:15.000000 pyransame-0.0.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:22:29.283916 pyransame-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-26 16:22:15.000000 pyransame-0.0.4/.github/workflows/pages_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-26 16:22:15.000000 pyransame-0.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-26 16:22:15.000000 pyransame-0.0.4/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-26 16:22:15.000000 pyransame-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-26 16:22:15.000000 pyransame-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-26 16:22:15.000000 pyransame-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-26 16:22:29.287916 pyransame-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-26 16:22:15.000000 pyransame-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:22:29.283916 pyransame-0.0.4/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-26 16:22:15.000000 pyransame-0.0.4/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:22:29.283916 pyransame-0.0.4/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   146735 2023-04-26 16:22:15.000000 pyransame-0.0.4/doc/_static/surface_sampling.png
+-rw-r--r--   0 runner    (1001) docker     (123)   183927 2023-04-26 16:22:15.000000 pyransame-0.0.4/doc/_static/volume_sampling.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-26 16:22:15.000000 pyransame-0.0.4/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-04-26 16:22:15.000000 pyransame-0.0.4/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-26 16:22:15.000000 pyransame-0.0.4/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-26 16:22:15.000000 pyransame-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-26 16:22:15.000000 pyransame-0.0.4/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-26 16:22:15.000000 pyransame-0.0.4/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 16:22:29.287916 pyransame-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:22:29.279915 pyransame-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:22:29.283916 pyransame-0.0.4/src/pyransame/
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-04-26 16:22:15.000000 pyransame-0.0.4/src/pyransame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-26 16:22:29.000000 pyransame-0.0.4/src/pyransame/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-04-26 16:22:15.000000 pyransame-0.0.4/src/pyransame/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:22:29.287916 pyransame-0.0.4/src/pyransame.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-26 16:22:29.000000 pyransame-0.0.4/src/pyransame.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-26 16:22:29.000000 pyransame-0.0.4/src/pyransame.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:22:29.000000 pyransame-0.0.4/src/pyransame.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-26 16:22:29.000000 pyransame-0.0.4/src/pyransame.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 16:22:29.000000 pyransame-0.0.4/src/pyransame.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:22:29.287916 pyransame-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-26 16:22:15.000000 pyransame-0.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-04-26 16:22:15.000000 pyransame-0.0.4/tests/test_random_surface_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-26 16:22:15.000000 pyransame-0.0.4/tests/test_random_volume_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-04-26 16:22:15.000000 pyransame-0.0.4/tests/test_util.py
```

### Comparing `pyransame-0.0.3/.github/workflows/pages_publish.yml` & `pyransame-0.0.4/.github/workflows/pages_publish.yml`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,15 @@
           pip install vtk-osmesa --extra-index-url https://gitlab.kitware.com/api/v4/projects/13/packages/pypi/simple
       - name: Build documentation
         run: make -C doc html
       - name: Upload artifact
         uses: actions/upload-pages-artifact@v1
         with:
           path: doc/_build/html
-  
+
   # Deployment job
   deploy:
     environment:
       name: github-pages
       url: ${{ steps.deployment.outputs.page_url }}
     runs-on: ubuntu-latest
     needs: build
```

### Comparing `pyransame-0.0.3/.github/workflows/python-publish.yml` & `pyransame-0.0.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pyransame-0.0.3/.github/workflows/test.yml` & `pyransame-0.0.4/.github/workflows/test.yml`

 * *Files 10% similar despite different names*

```diff
@@ -22,11 +22,13 @@
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install -r requirements-test.txt
     - name: Install package
-      run: python -m pip install .
+      run: python -m pip install -e .
     - name: Test with pytest
       run: |
-        pytest tests
+        pytest tests --cov=src/pyransame --durations=10
+    - name: Upload coverage reports to Codecov
+      uses: codecov/codecov-action@v3
```

### Comparing `pyransame-0.0.3/.gitignore` & `pyransame-0.0.4/.gitignore`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -157,8 +157,8 @@
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
 .vscode
-_version.py
+_version.py
```

### Comparing `pyransame-0.0.3/LICENSE` & `pyransame-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyransame-0.0.3/doc/Makefile` & `pyransame-0.0.4/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pyransame-0.0.3/doc/conf.py` & `pyransame-0.0.4/doc/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,39 +3,40 @@
 # For the full list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 
-project = 'pyransame'
-copyright = '2023, Matthew Flamm'
-author = 'Matthew Flamm'
+project = "pyransame"
+copyright = "2023, Matthew Flamm"
+author = "Matthew Flamm"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
-    'sphinx.ext.autosummary',
-    'pyvista.ext.plot_directive',
-    ]
-
-templates_path = ['_templates']
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+    "numpydoc",
+    "sphinx.ext.autosummary",
+    "pyvista.ext.plot_directive",
+]
 
+templates_path = ["_templates"]
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
-html_theme = 'pydata_sphinx_theme'
-html_static_path = ['_static']
+html_theme = "pydata_sphinx_theme"
+html_static_path = ["_static"]
 
 import pyvista
+
 pyvista.OFF_SCREEN = True
 
 pyvista.set_plot_theme("document")
 pyvista.global_theme.window_size = [1024, 768]
 pyvista.global_theme.font.size = 22
 pyvista.global_theme.font.label_size = 22
 pyvista.global_theme.font.title_size = 22
-pyvista.global_theme.return_cpos = False
+pyvista.global_theme.return_cpos = False
```

### Comparing `pyransame-0.0.3/doc/make.bat` & `pyransame-0.0.4/doc/make.bat`

 * *Files identical despite different names*

### Comparing `pyransame-0.0.3/pyproject.toml` & `pyransame-0.0.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -23,7 +23,13 @@
 
 [tool.setuptools_scm]
 write_to = "src/pyransame/_version.py"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 namespaces = false
+
+[tool.isort]
+profile = "black"
+
+[tool.pytest.ini_options]
+testpaths = ["tests"]
```

### Comparing `pyransame-0.0.3/src/pyransame.egg-info/SOURCES.txt` & `pyransame-0.0.4/src/pyransame.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 .gitignore
+.pre-commit-config.yaml
 LICENSE
 README.md
 pyproject.toml
 requirements-doc.txt
 requirements-test.txt
 .devcontainer/devcontainer.json
 .devcontainer/oncreatecommand.sh
+.github/dependabot.yml
 .github/workflows/pages_publish.yml
 .github/workflows/python-publish.yml
 .github/workflows/test.yml
 doc/Makefile
 doc/conf.py
 doc/index.rst
 doc/make.bat
+doc/_static/surface_sampling.png
+doc/_static/volume_sampling.png
 src/pyransame/__init__.py
 src/pyransame/_version.py
 src/pyransame/util.py
 src/pyransame.egg-info/PKG-INFO
 src/pyransame.egg-info/SOURCES.txt
 src/pyransame.egg-info/dependency_links.txt
 src/pyransame.egg-info/requires.txt
 src/pyransame.egg-info/top_level.txt
+tests/__init__.py
 tests/test_random_surface_points.py
+tests/test_random_volume_points.py
 tests/test_util.py
```

### Comparing `pyransame-0.0.3/tests/test_random_surface_points.py` & `pyransame-0.0.4/tests/test_random_surface_points.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,93 +1,119 @@
 """Tests for random_surface_points."""
 import numpy as np
 import pyvista as pv
+
 import pyransame
 
 
 def test_square_plane():
     mesh = pv.Plane()
-    points = pyransame.random_surface_points(mesh, 100000)
-    assert points.shape == (100000, 3)
+    points = pyransame.random_surface_points(mesh, 200000)
+    assert points.shape == (200000, 3)
     assert isinstance(points, np.ndarray)
     assert np.allclose(points.mean(axis=0), (0.0, 0.0, 0.0), rtol=5e-3, atol=5e-3)
 
 
+def test_small_sample():
+    mesh = pv.Plane()
+    points = pyransame.random_surface_points(mesh, 2)
+    assert points.shape == (2, 3)
+    assert isinstance(points, np.ndarray)
+
+
 def test_nonuniform_cell_size():
     mesh = pv.Plane(i_resolution=1, j_resolution=3)
 
     # make mesh nonuniform, but still centered at (0,0,0)
-    mesh.points = np.array([
-        [1, -1, 0.0],
-        [-1, -1, 0],
-        [1, 0, 0],
-        [-1, 0, 0],
-        [1, 0.5, 0],
-        [-1, 0.5, 0],
-        [1, 1, 0],
-        [-1, 1, 0],
-    ])
+    # points not numbered the same as inside each cell
+    mesh.points = np.array(
+        [
+            [1, -1, 0.0],
+            [-1, -1, 0],
+            [1, 0, 0],
+            [-1, 0, 0],
+            [1, 0.5, 0],
+            [-1, 0.5, 0],
+            [1, 1, 0],
+            [-1, 1, 0],
+        ]
+    )
 
-    points = pyransame.random_surface_points(mesh, 100000)
+    points = pyransame.random_surface_points(mesh, 200000)
     assert np.allclose(points.mean(axis=0), (0.0, 0.0, 0.0), rtol=5e-3, atol=5e-3)
 
+
 def test_nonuniform_cell_size_w_precomputed_areas():
     mesh = pv.Plane(i_resolution=1, j_resolution=3)
-    
+
     # make mesh nonuniform, but still centered at (0,0,0)
-    mesh.points = np.array([
-        [1, -1, 0.0],
-        [-1, -1, 0],
-        [1, 0, 0],
-        [-1, 0, 0],
-        [1, 0.5, 0],
-        [-1, 0.5, 0],
-        [1, 1, 0],
-        [-1, 1, 0],
-    ])
+    # points not numbered the same as inside each cell
+    mesh.points = np.array(
+        [
+            [1, -1, 0.0],
+            [-1, -1, 0],
+            [1, 0, 0],
+            [-1, 0, 0],
+            [1, 0.5, 0],
+            [-1, 0.5, 0],
+            [1, 1, 0],
+            [-1, 1, 0],
+        ]
+    )
     mesh = mesh.compute_cell_sizes(length=False, volume=False)
 
-    points = pyransame.random_surface_points(mesh, 100000)
+    points = pyransame.random_surface_points(mesh, 200000)
     assert np.allclose(points.mean(axis=0), (0.0, 0.0, 0.0), rtol=5e-3, atol=5e-3)
 
 
 def test_weights():
     mesh = pv.Plane(i_resolution=1, j_resolution=2)
-    
+
     # make mesh nonuniform, with 2nd cell half size
-    mesh.points = np.array([
-        [1, -1, 0.0],
-        [-1, -1, 0],
-        [1, 0, 0],
-        [-1, 0, 0],
-        [1, 0.5, 0],
-        [-1, 0.5, 0],
-    ])
+    # points not numbered the same as inside each cell
+    mesh.points = np.array(
+        [
+            [1, -1, 0.0],
+            [-1, -1, 0],
+            [1, 0, 0],
+            [-1, 0, 0],
+            [1, 0.5, 0],
+            [-1, 0.5, 0],
+        ]
+    )
 
     # 1/2 the number of points will have y>0 if no weighting is done
     # The expected y_mean will be -0.5 for points in cell 0 and 0.25 for piotns in cell 1
     # Therefore a weighting of 1:4 must be applied to have center be at y=0.0
 
     mesh.cell_data["weights"] = [1, 4]
 
-    points = pyransame.random_surface_points(mesh, 100000, "weights")
+    points = pyransame.random_surface_points(mesh, 200000, "weights")
     assert np.allclose(points.mean(axis=0), (0.0, 0.0, 0.0), rtol=5e-3, atol=5e-3)
 
+    mesh.cell_data.clear()
+    mesh.cell_data["other_str"] = [1, 4]
+
+    points = pyransame.random_surface_points(mesh, 200, "other_str")
+
 
 def test_weights_array():
     mesh = pv.Plane(i_resolution=1, j_resolution=2)
 
     # make mesh nonuniform, with 2nd cell half size
-    mesh.points = np.array([
-        [1, -1, 0.0],
-        [-1, -1, 0],
-        [1, 0, 0],
-        [-1, 0, 0],
-        [1, 0.5, 0],
-        [-1, 0.5, 0],
-    ])
+    # points not numbered the same as inside each cell
+    mesh.points = np.array(
+        [
+            [1, -1, 0.0],
+            [-1, -1, 0],
+            [1, 0, 0],
+            [-1, 0, 0],
+            [1, 0.5, 0],
+            [-1, 0.5, 0],
+        ]
+    )
 
     # 1/2 the number of points will have y>0 if no weighting is done
     # The expected y_mean will be -0.5 for points in cell 0 and 0.25 for piotns in cell 1
     # Therefore a weighting of 1:4 must be applied to have center be at y=0.0
-    points = pyransame.random_surface_points(mesh, 100000, [1, 4])
+    points = pyransame.random_surface_points(mesh, 200000, [1, 4])
     assert np.allclose(points.mean(axis=0), (0.0, 0.0, 0.0), rtol=5e-3, atol=5e-3)
```

