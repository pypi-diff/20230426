# Comparing `tmp/pytest_jupyterhub-0.0.1.dev0.tar.gz` & `tmp/pytest_jupyterhub-0.1.0.tar.gz`

## Comparing `pytest_jupyterhub-0.0.1.dev0.tar` & `pytest_jupyterhub-0.1.0.tar`

### file list

```diff
@@ -1,32 +1,34 @@
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.0.1.dev0/.flake8
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.0.1.dev0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.0.1.dev0/.readthedocs.yaml
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.0.1.dev0/CONTRIBUTING.md
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.0.1.dev0/MANIFEST.in
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.0.1.dev0/.github/dependabot.yaml
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.0.1.dev0/.github/workflows/test.yml
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.0.1.dev0/docs/Makefile
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.0.1.dev0/docs/make.bat
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.0.1.dev0/docs/requirements.txt
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.0.1.dev0/docs/source/changelog.md
--rw-r--r--   0        0        0     3775 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.0.1.dev0/docs/source/conf.py
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.0.1.dev0/docs/source/fixtures.md
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.0.1.dev0/docs/source/index.md
--rw-r--r--   0        0        0     4555 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.0.1.dev0/docs/source/_static/images/logo/favicon.ico
--rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.0.1.dev0/docs/source/_static/images/logo/logo.png
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.0.1.dev0/docs/source/contributing/docs.md
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.0.1.dev0/docs/source/contributing/index.md
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.0.1.dev0/docs/source/contributing/setup.md
--rw-r--r--   0        0        0     5443 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.0.1.dev0/docs/source/contributing/tests.md
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.0.1.dev0/docs/source/plugins/index.md
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.0.1.dev0/docs/source/plugins/jupyterhub_spawners.md
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.0.1.dev0/pytest_jupyterhub/__init__.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.0.1.dev0/pytest_jupyterhub/_version.py
--rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.0.1.dev0/pytest_jupyterhub/jupyterhub_spawners.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.0.1.dev0/tests/__init__.py
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.0.1.dev0/tests/test_jupyterhub_spawners.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.0.1.dev0/.gitignore
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.0.1.dev0/LICENSE
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.0.1.dev0/README.md
--rw-r--r--   0        0        0     3460 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.0.1.dev0/pyproject.toml
--rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.0.1.dev0/PKG-INFO
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.1.0/.flake8
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.1.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.1.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.1.0/MANIFEST.in
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.1.0/RELEASE.md
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.1.0/.github/dependabot.yaml
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.1.0/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.1.0/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.1.0/docs/Makefile
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.1.0/docs/make.bat
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.1.0/docs/requirements.txt
+-rw-r--r--   0        0        0     5441 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.1.0/docs/source/changelog.md
+-rw-r--r--   0        0        0     3775 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.1.0/docs/source/conf.py
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.1.0/docs/source/fixtures.md
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.1.0/docs/source/index.md
+-rw-r--r--   0        0        0     4555 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.1.0/docs/source/_static/images/logo/favicon.ico
+-rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.1.0/docs/source/_static/images/logo/logo.png
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.1.0/docs/source/contributing/docs.md
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.1.0/docs/source/contributing/index.md
+-rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.1.0/docs/source/contributing/setup.md
+-rw-r--r--   0        0        0     5443 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.1.0/docs/source/contributing/tests.md
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.1.0/docs/source/plugins/index.md
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.1.0/docs/source/plugins/jupyterhub_spawners.md
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.1.0/pytest_jupyterhub/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.1.0/pytest_jupyterhub/_version.py
+-rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.1.0/pytest_jupyterhub/jupyterhub_spawners.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.1.0/tests/test_jupyterhub_spawners.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.1.0/LICENSE
+-rw-r--r--   0        0        0     5165 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.1.0/README.md
+-rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     7813 2020-02-02 00:00:00.000000 pytest_jupyterhub-0.1.0/PKG-INFO
```

### Comparing `pytest_jupyterhub-0.0.1.dev0/.pre-commit-config.yaml` & `pytest_jupyterhub-0.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pytest_jupyterhub-0.0.1.dev0/.github/dependabot.yaml` & `pytest_jupyterhub-0.1.0/.github/dependabot.yaml`

 * *Files identical despite different names*

### Comparing `pytest_jupyterhub-0.0.1.dev0/.github/workflows/test.yml` & `pytest_jupyterhub-0.1.0/.github/workflows/test.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 on:
   pull_request:
     paths-ignore:
       - "docs/**"
       - "**.md"
       - "**.rst"
       - ".github/workflows/*"
-      - "!.github/workflows/test.yml"
+      - "!.github/workflows/test.yaml"
   push:
     paths-ignore:
       - "docs/**"
       - "**.md"
       - "**.rst"
       - ".github/workflows/*"
-      - "!.github/workflows/test.yml"
+      - "!.github/workflows/test.yaml"
     branches-ignore:
       - "pre-commit-ci-update-config"
   workflow_dispatch:
 
 permissions:
   contents: read
 
@@ -49,15 +49,15 @@
         uses: actions/setup-node@v3
         with:
           node-version: "14"
 
       - name: Install Javascript dependencies
         run: |
           npm install
-          npm install -g configurable-http-proxy yarn
+          npm install -g configurable-http-proxy
           npm list
 
       - name: Install Python ${{ matrix.python}}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
 
@@ -67,10 +67,9 @@
           pip install -e ".[test]"
           pip freeze
 
       - name: Run the tests
         run: |
           pytest -v --cov=pytest_jupyterhub tests
 
-      # - name: Submit codecov report
-      #   run: |
-      #     codecov
+      - name: Submit codecov report
+        uses: codecov/codecov-action@v3
```

### Comparing `pytest_jupyterhub-0.0.1.dev0/docs/Makefile` & `pytest_jupyterhub-0.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pytest_jupyterhub-0.0.1.dev0/docs/make.bat` & `pytest_jupyterhub-0.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pytest_jupyterhub-0.0.1.dev0/docs/source/conf.py` & `pytest_jupyterhub-0.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pytest_jupyterhub-0.0.1.dev0/docs/source/fixtures.md` & `pytest_jupyterhub-0.1.0/docs/source/fixtures.md`

 * *Files identical despite different names*

### Comparing `pytest_jupyterhub-0.0.1.dev0/docs/source/index.md` & `pytest_jupyterhub-0.1.0/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `pytest_jupyterhub-0.0.1.dev0/docs/source/_static/images/logo/favicon.ico` & `pytest_jupyterhub-0.1.0/docs/source/_static/images/logo/favicon.ico`

 * *Files identical despite different names*

### Comparing `pytest_jupyterhub-0.0.1.dev0/docs/source/_static/images/logo/logo.png` & `pytest_jupyterhub-0.1.0/docs/source/_static/images/logo/logo.png`

 * *Files identical despite different names*

### Comparing `pytest_jupyterhub-0.0.1.dev0/docs/source/contributing/docs.md` & `pytest_jupyterhub-0.1.0/docs/source/contributing/docs.md`

 * *Files identical despite different names*

### Comparing `pytest_jupyterhub-0.0.1.dev0/docs/source/contributing/index.md` & `pytest_jupyterhub-0.1.0/docs/source/contributing/index.md`

 * *Files identical despite different names*

### Comparing `pytest_jupyterhub-0.0.1.dev0/docs/source/contributing/setup.md` & `pytest_jupyterhub-0.1.0/docs/source/contributing/setup.md`

 * *Files 24% similar despite different names*

```diff
@@ -6,14 +6,20 @@
 
 The [JupyterHub Pytest Plugin](https://github.com/jupyterhub/pytest-jupyterhub) uses [JupyterHub](https://github.com/jupyterhub/jupyterhub) which can only run on macOS or Linux operating systems. If you are using Windows, we recommend using [VirtualBox](https://virtualbox.org) or a similar system to run [Ubuntu Linux](https://ubuntu.com) for development.
 
 ### Install Python
 
 The JupyterHub Pytest Plugin is written in the [Python](https://python.org) programming language and requires you have at least version 3.8 installed locally. If you haven’t installed Python before, the recommended way to install it is to use [Miniforge](https://github.com/conda-forge/miniforge#download).
 
+### Install nodejs
+
+[NodeJS 12+](https://nodejs.org/en/) is required for building some JavaScript components. `configurable-http-proxy`, the default proxy implementation for JupyterHub, is written in Javascript. If you have not installed NodeJS before, we recommend installing it in the `miniconda` environment you set up for Python. You can do so with `conda install nodejs`.
+
+Many in the Jupyter community use \[`nvm`\](<https://github.com/nvm-sh/nvm>) to managing node dependencies.
+
 ### Install git
 
 The JupyterHub Pytest Plugin uses [Git](https://git-scm.com) & [GitHub](https://github.com) for development & collaboration. You need to [install git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) to work on the JupyterHub Pytest Plugin. We also recommend getting a free account on GitHub.com.
 
 ## Setting up a development install
 
 When developing Pytest JupyterHub, you would need to make changes and be able to instantly test the changes. To achieve that, a developer install is required.
@@ -29,28 +35,57 @@
 1. Clone the [Pytest JupyterHub](https://github.com/jupyterhub/pytest-jupyterhub) repository to your computer.
 
    ```bash
    git clone https://github.com/jupyterhub/pytest-jupyterhub.git
    cd pytest-jupyterhub
    ```
 
-2. Make sure the `python` you installed is available to you on the command line.
+2. Make sure the `python` and `npm` you installed are available to you on the command line.
 
    ```bash
    python -V
    ```
 
    This should return a version number greater than or equal to 3.8.
 
-3. Install an editable version of Pytest-JupyterHub and its requirements for development and testing.
+   ```bash
+   npm -v
+   ```
+
+   This should return a version number greater than or equal to 5.0.
+
+3. Install `configurable-http-proxy` (required to run and test the default JupyterHub configuration):
+
+   ```bash
+   npm install -g configurable-http-proxy
+   ```
+
+   If you get an error that says `Error: EACCES: permission denied`, you might need to prefix the command with `sudo`.
+   `sudo` may be required to perform a system-wide install.
+   If you do not have access to sudo, you may instead run the following commands:
+
+   ```bash
+   npm install configurable-http-proxy
+   export PATH=$PATH:$(pwd)/node_modules/.bin
+   ```
+
+   The second line needs to be run every time you open a new terminal.
+
+   If you are using conda you can instead run:
+
+   ```bash
+   conda install configurable-http-proxy
+   ```
+
+4. Install an editable version of Pytest-JupyterHub and its requirements for development and testing.
 
    ```bash
    python3 -m pip install --editable ".[test]"
    ```
 
-4. You are now good to go! Run the tests to confirm all required dependencies have been installed correctly.
+5. You are now good to go! Run the tests to confirm all required dependencies have been installed correctly.
 
    ```bash
    pytest -v --cov=pytest_jupyterhub tests
    ```
 
 Happy Coding! :)
```

### Comparing `pytest_jupyterhub-0.0.1.dev0/docs/source/contributing/tests.md` & `pytest_jupyterhub-0.1.0/docs/source/contributing/tests.md`

 * *Files identical despite different names*

### Comparing `pytest_jupyterhub-0.0.1.dev0/docs/source/plugins/index.md` & `pytest_jupyterhub-0.1.0/docs/source/plugins/index.md`

 * *Files identical despite different names*

### Comparing `pytest_jupyterhub-0.0.1.dev0/pytest_jupyterhub/jupyterhub_spawners.py` & `pytest_jupyterhub-0.1.0/pytest_jupyterhub/jupyterhub_spawners.py`

 * *Files identical despite different names*

### Comparing `pytest_jupyterhub-0.0.1.dev0/tests/test_jupyterhub_spawners.py` & `pytest_jupyterhub-0.1.0/tests/test_jupyterhub_spawners.py`

 * *Files identical despite different names*

### Comparing `pytest_jupyterhub-0.0.1.dev0/.gitignore` & `pytest_jupyterhub-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_jupyterhub-0.0.1.dev0/LICENSE` & `pytest_jupyterhub-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_jupyterhub-0.0.1.dev0/pyproject.toml` & `pytest_jupyterhub-0.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 #
 # ref: https://github.com/your-tools/tbump#readme
 #
 [tool.tbump]
 github_url = "https://github.com/jupyterhub/pytest-jupyterhub"
 
 [tool.tbump.version]
-current = "0.0.1.dev0"
+current = "0.1.0"
 regex = '''
     (?P<major>\d+)
     \.
     (?P<minor>\d+)
     \.
     (?P<patch>\d+)
     (?P<pre>((a|b|rc)\d+)|)
```

