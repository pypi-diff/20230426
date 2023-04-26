# Comparing `tmp/twopilabs-sense-x1000-0.6.3.tar.gz` & `tmp/twopilabs-sense-x1000-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/builds/devel/products/tahiti/tahiti-software/python/twopilabs-sense-x1000/dist/.tmp-jpgb7a4e/twopilabs-sense-x1000-0.6.3.tar", last modified: Tue Apr  4 15:06:19 2023, max compression
+gzip compressed data, was "/builds/devel/products/tahiti/tahiti-software/python/twopilabs-sense-x1000/dist/.tmp-80z8x1bi/twopilabs-sense-x1000-0.6.4.tar", last modified: Tue Apr 25 14:58:34 2023, max compression
```

## Comparing `twopilabs-sense-x1000-0.6.3.tar` & `twopilabs-sense-x1000-0.6.4.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 15:06:19.000000 twopilabs-sense-x1000-0.6.3/
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      922 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     7652 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      809 2023-04-04 15:06:19.000000 twopilabs-sense-x1000-0.6.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      184 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 15:06:19.000000 twopilabs-sense-x1000-0.6.3/docs/
--rw-rw-rw-   0 root         (0) root         (0)      634 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 15:06:19.000000 twopilabs-sense-x1000-0.6.3/docs/_images/
--rw-rw-rw-   0 root         (0) root         (0)    52074 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/docs/_images/examples-fast-plot-screenshot.png
--rw-rw-rw-   0 root         (0) root         (0)    48716 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/docs/_images/examples-hdf5-record-screenshot.png
--rw-rw-rw-   0 root         (0) root         (0)   425392 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/docs/_images/examples-live-plot-screenshot.png
--rw-rw-rw-   0 root         (0) root         (0)    58587 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/docs/_images/examples-range-doppler-screenshot.png
--rw-rw-rw-   0 root         (0) root         (0)     2995 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     2499 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/docs/configuring.rst
--rw-rw-rw-   0 root         (0) root         (0)     6058 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/docs/controlling.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 15:06:19.000000 twopilabs-sense-x1000-0.6.3/docs/examples/
--rw-rw-rw-   0 root         (0) root         (0)     1620 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/docs/examples/examples.rst
--rw-rw-rw-   0 root         (0) root         (0)      347 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/docs/examples/fast-plot.rst
--rw-rw-rw-   0 root         (0) root         (0)      836 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/docs/examples/hdf5-recorder.rst
--rw-rw-rw-   0 root         (0) root         (0)      342 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/docs/examples/live-plot.rst
--rw-rw-rw-   0 root         (0) root         (0)      557 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/docs/examples/range-doppler.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 15:06:19.000000 twopilabs-sense-x1000-0.6.3/docs/extensions/
--rw-rw-rw-   0 root         (0) root         (0)      977 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/docs/extensions/source.py
--rw-rw-rw-   0 root         (0) root         (0)      772 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     3402 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/docs/introduction.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 15:06:19.000000 twopilabs-sense-x1000-0.6.3/docs/reference/
--rw-rw-rw-   0 root         (0) root         (0)      426 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/docs/reference/sense.x1000.rst
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/docs/reference/sense.x1000.scpi_calc.rst
--rw-rw-rw-   0 root         (0) root         (0)      144 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/docs/reference/sense.x1000.scpi_control.rst
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/docs/reference/sense.x1000.scpi_core.rst
--rw-rw-rw-   0 root         (0) root         (0)      146 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/docs/reference/sense.x1000.scpi_initiate.rst
--rw-rw-rw-   0 root         (0) root         (0)      140 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/docs/reference/sense.x1000.scpi_memory.rst
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/docs/reference/sense.x1000.scpi_sense.rst
--rw-rw-rw-   0 root         (0) root         (0)      140 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/docs/reference/sense.x1000.scpi_system.rst
--rw-rw-rw-   0 root         (0) root         (0)      143 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/docs/reference/sense.x1000.scpi_trigger.rst
--rw-rw-rw-   0 root         (0) root         (0)      139 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/docs/reference/sense.x1000.x1000.rst
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/docs/reference/sense.x1000.x1000_base.rst
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/docs/reference/sense.x1000.x1000_scpi.rst
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 15:06:19.000000 twopilabs-sense-x1000-0.6.3/examples/
--rw-rw-rw-   0 root         (0) root         (0)      223 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/examples/environment.yml
--rwxrwxrwx   0 root         (0) root         (0)    21804 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/examples/fast-plot.py
--rw-rw-rw-   0 root         (0) root         (0)      913 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/examples/fast-plot.spec
--rwxrwxrwx   0 root         (0) root         (0)     2557 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/examples/fw-upgrade.py
--rwxrwxrwx   0 root         (0) root         (0)     8479 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/examples/hdf5-record.py
--rwxrwxrwx   0 root         (0) root         (0)     7983 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/examples/hdf5-replay.py
--rwxrwxrwx   0 root         (0) root         (0)    11766 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/examples/live-plot.py
--rw-rw-rw-   0 root         (0) root         (0)      913 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/examples/live-plot.spec
--rwxrwxrwx   0 root         (0) root         (0)    13267 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/examples/range-doppler.py
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/examples/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      766 2023-04-04 15:06:19.000000 twopilabs-sense-x1000-0.6.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 15:06:19.000000 twopilabs-sense-x1000-0.6.3/twopilabs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 15:06:19.000000 twopilabs-sense-x1000-0.6.3/twopilabs/sense/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 15:06:19.000000 twopilabs-sense-x1000-0.6.3/twopilabs/sense/x1000/
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/twopilabs/sense/x1000/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      900 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/twopilabs/sense/x1000/scpi_calc.py
--rw-rw-rw-   0 root         (0) root         (0)    22317 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/twopilabs/sense/x1000/scpi_control.py
--rw-rw-rw-   0 root         (0) root         (0)     2045 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/twopilabs/sense/x1000/scpi_core.py
--rw-rw-rw-   0 root         (0) root         (0)      876 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/twopilabs/sense/x1000/scpi_initiate.py
--rw-rw-rw-   0 root         (0) root         (0)     2442 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/twopilabs/sense/x1000/scpi_memory.py
--rw-rw-rw-   0 root         (0) root         (0)     8124 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/twopilabs/sense/x1000/scpi_sense.py
--rw-rw-rw-   0 root         (0) root         (0)    11079 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/twopilabs/sense/x1000/scpi_system.py
--rw-rw-rw-   0 root         (0) root         (0)     2248 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/twopilabs/sense/x1000/scpi_trigger.py
--rw-rw-rw-   0 root         (0) root         (0)     1954 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/twopilabs/sense/x1000/x1000.py
--rw-rw-rw-   0 root         (0) root         (0)    45066 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/twopilabs/sense/x1000/x1000_base.py
--rw-rw-rw-   0 root         (0) root         (0)     2818 2023-04-04 15:05:04.000000 twopilabs-sense-x1000-0.6.3/twopilabs/sense/x1000/x1000_scpi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 15:06:19.000000 twopilabs-sense-x1000-0.6.3/twopilabs_sense_x1000.egg-info/
--rw-r--r--   0 root         (0) root         (0)      809 2023-04-04 15:06:18.000000 twopilabs-sense-x1000-0.6.3/twopilabs_sense_x1000.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1963 2023-04-04 15:06:19.000000 twopilabs-sense-x1000-0.6.3/twopilabs_sense_x1000.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-04 15:06:18.000000 twopilabs-sense-x1000-0.6.3/twopilabs_sense_x1000.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       41 2023-04-04 15:06:18.000000 twopilabs-sense-x1000-0.6.3/twopilabs_sense_x1000.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-04 15:06:18.000000 twopilabs-sense-x1000-0.6.3/twopilabs_sense_x1000.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 14:58:34.000000 twopilabs-sense-x1000-0.6.4/
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      922 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      809 2023-04-25 14:58:34.000000 twopilabs-sense-x1000-0.6.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      184 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 14:58:34.000000 twopilabs-sense-x1000-0.6.4/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      634 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 14:58:34.000000 twopilabs-sense-x1000-0.6.4/docs/_images/
+-rw-rw-rw-   0 root         (0) root         (0)    52074 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/docs/_images/examples-fast-plot-screenshot.png
+-rw-rw-rw-   0 root         (0) root         (0)    48716 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/docs/_images/examples-hdf5-record-screenshot.png
+-rw-rw-rw-   0 root         (0) root         (0)   425392 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/docs/_images/examples-live-plot-screenshot.png
+-rw-rw-rw-   0 root         (0) root         (0)    58587 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/docs/_images/examples-range-doppler-screenshot.png
+-rw-rw-rw-   0 root         (0) root         (0)     2995 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2499 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/docs/configuring.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6058 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/docs/controlling.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 14:58:34.000000 twopilabs-sense-x1000-0.6.4/docs/examples/
+-rw-rw-rw-   0 root         (0) root         (0)     1620 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/docs/examples/examples.rst
+-rw-rw-rw-   0 root         (0) root         (0)      347 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/docs/examples/fast-plot.rst
+-rw-rw-rw-   0 root         (0) root         (0)      836 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/docs/examples/hdf5-recorder.rst
+-rw-rw-rw-   0 root         (0) root         (0)      342 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/docs/examples/live-plot.rst
+-rw-rw-rw-   0 root         (0) root         (0)      557 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/docs/examples/range-doppler.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 14:58:34.000000 twopilabs-sense-x1000-0.6.4/docs/extensions/
+-rw-rw-rw-   0 root         (0) root         (0)      977 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/docs/extensions/source.py
+-rw-rw-rw-   0 root         (0) root         (0)      772 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3402 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/docs/introduction.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 14:58:34.000000 twopilabs-sense-x1000-0.6.4/docs/reference/
+-rw-rw-rw-   0 root         (0) root         (0)      426 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/docs/reference/sense.x1000.rst
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/docs/reference/sense.x1000.scpi_calc.rst
+-rw-rw-rw-   0 root         (0) root         (0)      144 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/docs/reference/sense.x1000.scpi_control.rst
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/docs/reference/sense.x1000.scpi_core.rst
+-rw-rw-rw-   0 root         (0) root         (0)      146 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/docs/reference/sense.x1000.scpi_initiate.rst
+-rw-rw-rw-   0 root         (0) root         (0)      140 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/docs/reference/sense.x1000.scpi_memory.rst
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/docs/reference/sense.x1000.scpi_sense.rst
+-rw-rw-rw-   0 root         (0) root         (0)      140 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/docs/reference/sense.x1000.scpi_system.rst
+-rw-rw-rw-   0 root         (0) root         (0)      143 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/docs/reference/sense.x1000.scpi_trigger.rst
+-rw-rw-rw-   0 root         (0) root         (0)      139 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/docs/reference/sense.x1000.x1000.rst
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/docs/reference/sense.x1000.x1000_base.rst
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/docs/reference/sense.x1000.x1000_scpi.rst
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 14:58:34.000000 twopilabs-sense-x1000-0.6.4/examples/
+-rw-rw-rw-   0 root         (0) root         (0)      223 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/examples/environment.yml
+-rwxrwxrwx   0 root         (0) root         (0)    21804 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/examples/fast-plot.py
+-rw-rw-rw-   0 root         (0) root         (0)      913 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/examples/fast-plot.spec
+-rwxrwxrwx   0 root         (0) root         (0)     2557 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/examples/fw-upgrade.py
+-rwxrwxrwx   0 root         (0) root         (0)     8479 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/examples/hdf5-record.py
+-rwxrwxrwx   0 root         (0) root         (0)     7983 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/examples/hdf5-replay.py
+-rwxrwxrwx   0 root         (0) root         (0)    11766 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/examples/live-plot.py
+-rw-rw-rw-   0 root         (0) root         (0)      913 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/examples/live-plot.spec
+-rwxrwxrwx   0 root         (0) root         (0)    13267 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/examples/range-doppler.py
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/examples/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      766 2023-04-25 14:58:34.000000 twopilabs-sense-x1000-0.6.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 14:58:34.000000 twopilabs-sense-x1000-0.6.4/twopilabs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 14:58:34.000000 twopilabs-sense-x1000-0.6.4/twopilabs/sense/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 14:58:34.000000 twopilabs-sense-x1000-0.6.4/twopilabs/sense/x1000/
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/twopilabs/sense/x1000/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      900 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/twopilabs/sense/x1000/scpi_calc.py
+-rw-rw-rw-   0 root         (0) root         (0)    23485 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/twopilabs/sense/x1000/scpi_control.py
+-rw-rw-rw-   0 root         (0) root         (0)     2045 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/twopilabs/sense/x1000/scpi_core.py
+-rw-rw-rw-   0 root         (0) root         (0)      876 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/twopilabs/sense/x1000/scpi_initiate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2442 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/twopilabs/sense/x1000/scpi_memory.py
+-rw-rw-rw-   0 root         (0) root         (0)     8124 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/twopilabs/sense/x1000/scpi_sense.py
+-rw-rw-rw-   0 root         (0) root         (0)    11079 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/twopilabs/sense/x1000/scpi_system.py
+-rw-rw-rw-   0 root         (0) root         (0)     2248 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/twopilabs/sense/x1000/scpi_trigger.py
+-rw-rw-rw-   0 root         (0) root         (0)     1954 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/twopilabs/sense/x1000/x1000.py
+-rw-rw-rw-   0 root         (0) root         (0)    45279 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/twopilabs/sense/x1000/x1000_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2818 2023-04-25 14:57:22.000000 twopilabs-sense-x1000-0.6.4/twopilabs/sense/x1000/x1000_scpi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 14:58:34.000000 twopilabs-sense-x1000-0.6.4/twopilabs_sense_x1000.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      809 2023-04-25 14:58:34.000000 twopilabs-sense-x1000-0.6.4/twopilabs_sense_x1000.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1963 2023-04-25 14:58:34.000000 twopilabs-sense-x1000-0.6.4/twopilabs_sense_x1000.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 14:58:34.000000 twopilabs-sense-x1000-0.6.4/twopilabs_sense_x1000.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2023-04-25 14:58:34.000000 twopilabs-sense-x1000-0.6.4/twopilabs_sense_x1000.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-25 14:58:34.000000 twopilabs-sense-x1000-0.6.4/twopilabs_sense_x1000.egg-info/top_level.txt
```

### Comparing `twopilabs-sense-x1000-0.6.3/.gitlab-ci.yml` & `twopilabs-sense-x1000-0.6.4/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.6.3/LICENSE` & `twopilabs-sense-x1000-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.6.3/PKG-INFO` & `twopilabs-sense-x1000-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twopilabs-sense-x1000
-Version: 0.6.3
+Version: 0.6.4
 Summary: Official 2πSENSE X1000 series hardware control library
 Home-page: https://www.2pi-labs.com
 Author: 2pi-Labs GmbH
 Author-email: opensource@2pi-labs.com
 License: LGPLv3
 Project-URL: Documentation, https://2pi-labs.gitlab.io/python/twopilabs-sense-x1000
 Project-URL: Source, https://gitlab.com/2pi-labs/python/twopilabs-sense-x1000
```

### Comparing `twopilabs-sense-x1000-0.6.3/docs/Makefile` & `twopilabs-sense-x1000-0.6.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.6.3/docs/_images/examples-fast-plot-screenshot.png` & `twopilabs-sense-x1000-0.6.4/docs/_images/examples-fast-plot-screenshot.png`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.6.3/docs/_images/examples-hdf5-record-screenshot.png` & `twopilabs-sense-x1000-0.6.4/docs/_images/examples-hdf5-record-screenshot.png`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.6.3/docs/_images/examples-live-plot-screenshot.png` & `twopilabs-sense-x1000-0.6.4/docs/_images/examples-live-plot-screenshot.png`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.6.3/docs/_images/examples-range-doppler-screenshot.png` & `twopilabs-sense-x1000-0.6.4/docs/_images/examples-range-doppler-screenshot.png`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.6.3/docs/conf.py` & `twopilabs-sense-x1000-0.6.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.6.3/docs/configuring.rst` & `twopilabs-sense-x1000-0.6.4/docs/configuring.rst`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.6.3/docs/controlling.rst` & `twopilabs-sense-x1000-0.6.4/docs/controlling.rst`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.6.3/docs/examples/examples.rst` & `twopilabs-sense-x1000-0.6.4/docs/examples/examples.rst`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.6.3/docs/examples/hdf5-recorder.rst` & `twopilabs-sense-x1000-0.6.4/docs/examples/hdf5-recorder.rst`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.6.3/docs/examples/range-doppler.rst` & `twopilabs-sense-x1000-0.6.4/docs/examples/range-doppler.rst`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.6.3/docs/extensions/source.py` & `twopilabs-sense-x1000-0.6.4/docs/extensions/source.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.6.3/docs/index.rst` & `twopilabs-sense-x1000-0.6.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.6.3/docs/introduction.rst` & `twopilabs-sense-x1000-0.6.4/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.6.3/examples/fast-plot.py` & `twopilabs-sense-x1000-0.6.4/examples/fast-plot.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.6.3/examples/fast-plot.spec` & `twopilabs-sense-x1000-0.6.4/examples/fast-plot.spec`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.6.3/examples/fw-upgrade.py` & `twopilabs-sense-x1000-0.6.4/examples/fw-upgrade.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.6.3/examples/hdf5-record.py` & `twopilabs-sense-x1000-0.6.4/examples/hdf5-record.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.6.3/examples/hdf5-replay.py` & `twopilabs-sense-x1000-0.6.4/examples/hdf5-replay.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.6.3/examples/live-plot.py` & `twopilabs-sense-x1000-0.6.4/examples/live-plot.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.6.3/examples/live-plot.spec` & `twopilabs-sense-x1000-0.6.4/examples/live-plot.spec`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.6.3/examples/range-doppler.py` & `twopilabs-sense-x1000-0.6.4/examples/range-doppler.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.6.3/setup.cfg` & `twopilabs-sense-x1000-0.6.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.6.3/twopilabs/sense/x1000/scpi_calc.py` & `twopilabs-sense-x1000-0.6.4/twopilabs/sense/x1000/scpi_calc.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.6.3/twopilabs/sense/x1000/scpi_control.py` & `twopilabs-sense-x1000-0.6.4/twopilabs/sense/x1000/scpi_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,14 +216,38 @@
         else:
             coupling = SenseX1000Base.ChannelCoupling[self.device.execute(
                 f'CONTROL:RADAR:FRONTEND:CHANNEL{chan_idx:d}:COUPLING?', result=ScpiChars).as_string()]
 
         self.device.raise_error()
         return coupling
 
+    def radar_processing_offset_length(self, chan_idx: int = 0) -> int:
+        """returns the processing offset table length"""
+        length = self.device.execute(f'CONTROL:RADAR:PROCESSING:OFFSET{chan_idx:d}:LENGTH?', result=ScpiNumber).as_int()
+        self.device.raise_error()
+
+        return length
+
+    def radar_processing_offset_blocksize(self, chan_idx: int = 0) -> int:
+        """returns the processing offset table block size"""
+        blocksize = self.device.execute(f'CONTROL:RADAR:PROCESSING:OFFSET{chan_idx:d}:BSIZE?', result=ScpiNumber).as_int()
+        self.device.raise_error()
+
+        return blocksize
+
+    def radar_processing_offset_data(self, address: int, block: Optional[bytes] = None, chan_idx: int = 0) -> bytes:
+        """sets/gets radar processing offset table data"""
+        if block is not None:
+            self.device.execute(f'CONTROL:RADAR:PROCESSING:OFFSET{chan_idx:d}:DATA {address:d},', param=ScpiArbBlock(block))
+        else:
+            block = self.device.execute(f'CONTROL:RADAR:PROCESSING:OFFSET{chan_idx:d}:DATA? {address:d}', result=ScpiArbBlock).as_bytes()
+        self.device.raise_error()
+
+        return block
+
     def gpio_input_state(self, input_idx: Optional[int] = None) -> bool:
         """"Returns the current state of the given input port"""
         onoff = self.device.execute(f'CONTROL:GPIO:IN{input_idx or ""}:STATE?', result=ScpiBool).as_bool()
         self.device.raise_error()
 
         return onoff
```

### Comparing `twopilabs-sense-x1000-0.6.3/twopilabs/sense/x1000/scpi_core.py` & `twopilabs-sense-x1000-0.6.4/twopilabs/sense/x1000/scpi_core.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.6.3/twopilabs/sense/x1000/scpi_initiate.py` & `twopilabs-sense-x1000-0.6.4/twopilabs/sense/x1000/scpi_initiate.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.6.3/twopilabs/sense/x1000/scpi_memory.py` & `twopilabs-sense-x1000-0.6.4/twopilabs/sense/x1000/scpi_memory.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.6.3/twopilabs/sense/x1000/scpi_sense.py` & `twopilabs-sense-x1000-0.6.4/twopilabs/sense/x1000/scpi_sense.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.6.3/twopilabs/sense/x1000/scpi_system.py` & `twopilabs-sense-x1000-0.6.4/twopilabs/sense/x1000/scpi_system.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.6.3/twopilabs/sense/x1000/scpi_trigger.py` & `twopilabs-sense-x1000-0.6.4/twopilabs/sense/x1000/scpi_trigger.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.6.3/twopilabs/sense/x1000/x1000.py` & `twopilabs-sense-x1000-0.6.4/twopilabs/sense/x1000/x1000.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.6.3/twopilabs/sense/x1000/x1000_base.py` & `twopilabs-sense-x1000-0.6.4/twopilabs/sense/x1000/x1000_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -915,14 +915,17 @@
                 raise RuntimeError("This feature requires the h5py library to be installed.")
 
             if isinstance(parent, str):
                 # When string is given as parent, treat it as a filename
                 parent = h5py.File(parent, 'r')
 
             # This raises an exception if 'name' cannot be found in parent
+            if not isinstance(parent[name], h5py.Group) or 'acquisition_data' not in parent[name].keys():
+                raise TypeError(f'\'{parent[name].name}\' does not seem to be a loadable AcqData object')
+
             group = parent[name]
             acq_data = group['acquisition_data']
 
             if 'header' not in acq_data.attrs:
                 raise ValueError(f'{group} is missing acquisition header information')
 
             # Deserialize the header
```

### Comparing `twopilabs-sense-x1000-0.6.3/twopilabs/sense/x1000/x1000_scpi.py` & `twopilabs-sense-x1000-0.6.4/twopilabs/sense/x1000/x1000_scpi.py`

 * *Files identical despite different names*

### Comparing `twopilabs-sense-x1000-0.6.3/twopilabs_sense_x1000.egg-info/PKG-INFO` & `twopilabs-sense-x1000-0.6.4/twopilabs_sense_x1000.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twopilabs-sense-x1000
-Version: 0.6.3
+Version: 0.6.4
 Summary: Official 2πSENSE X1000 series hardware control library
 Home-page: https://www.2pi-labs.com
 Author: 2pi-Labs GmbH
 Author-email: opensource@2pi-labs.com
 License: LGPLv3
 Project-URL: Documentation, https://2pi-labs.gitlab.io/python/twopilabs-sense-x1000
 Project-URL: Source, https://gitlab.com/2pi-labs/python/twopilabs-sense-x1000
```

### Comparing `twopilabs-sense-x1000-0.6.3/twopilabs_sense_x1000.egg-info/SOURCES.txt` & `twopilabs-sense-x1000-0.6.4/twopilabs_sense_x1000.egg-info/SOURCES.txt`

 * *Files identical despite different names*

