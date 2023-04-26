# Comparing `tmp/virtualpdu-0.3.6.tar.gz` & `tmp/virtualpdu-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/virtualpdu-0.3.6.tar", last modified: Tue Mar  7 13:49:24 2017, max compression
+gzip compressed data, was "virtualpdu-1.0.0.tar", last modified: Tue Apr 25 14:40:54 2023, max compression
```

## Comparing `virtualpdu-0.3.6.tar` & `virtualpdu-1.0.0.tar`

### file list

```diff
@@ -1,93 +1,96 @@
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-07 13:49:24.000000 virtualpdu-0.3.6/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)       17 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/babel.cfg
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     1182 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/.travis.yml
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     1384 2017-03-07 13:49:24.000000 virtualpdu-0.3.6/setup.cfg
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      621 2017-03-07 13:49:23.000000 virtualpdu-0.3.6/AUTHORS
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      654 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/CONTRIBUTING.rst
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      511 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/test-requirements.txt
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)    10143 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/LICENSE
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)       89 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/.mailmap
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-07 13:49:24.000000 virtualpdu-0.3.6/releasenotes/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-07 13:49:24.000000 virtualpdu-0.3.6/releasenotes/source/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-07 13:49:24.000000 virtualpdu-0.3.6/releasenotes/source/_static/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        0 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/releasenotes/source/_static/.placeholder
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     8944 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/releasenotes/source/conf.py
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      112 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/releasenotes/source/unreleased.rst
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-07 13:49:24.000000 virtualpdu-0.3.6/releasenotes/source/_templates/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        0 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      161 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/releasenotes/source/index.rst
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-07 13:49:24.000000 virtualpdu-0.3.6/releasenotes/notes/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        0 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/releasenotes/notes/.placeholder
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-07 13:49:24.000000 virtualpdu-0.3.6/virtualpdu/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     3908 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/virtualpdu/main.py
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-07 13:49:24.000000 virtualpdu-0.3.6/virtualpdu/pdu/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     1962 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/virtualpdu/pdu/baytech_mrp27.py
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     4266 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/virtualpdu/pdu/__init__.py
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     6259 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/virtualpdu/pdu/pysnmp_handler.py
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     3860 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/virtualpdu/pdu/apc_rackpdu.py
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     2619 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/virtualpdu/core.py
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-07 13:49:24.000000 virtualpdu-0.3.6/virtualpdu/tests/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-07 13:49:24.000000 virtualpdu-0.3.6/virtualpdu/tests/integration/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     5726 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/virtualpdu/tests/integration/test_entrypoint.py
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-07 13:49:24.000000 virtualpdu-0.3.6/virtualpdu/tests/integration/pdu/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     2626 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/virtualpdu/tests/integration/pdu/test_baytech_mrp27.py
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     2141 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/virtualpdu/tests/integration/pdu/test_pdu.py
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     4487 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/virtualpdu/tests/integration/pdu/test_pysnmp_handler.py
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     2699 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/virtualpdu/tests/integration/pdu/__init__.py
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     2591 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/virtualpdu/tests/integration/pdu/test_apc_rackpdu.py
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        0 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/virtualpdu/tests/integration/__init__.py
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-07 13:49:24.000000 virtualpdu-0.3.6/virtualpdu/tests/integration/drivers/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     2030 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/virtualpdu/tests/integration/drivers/test_libvirt_driver.py
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        0 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/virtualpdu/tests/integration/drivers/__init__.py
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     4045 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/virtualpdu/tests/integration/test_core_integration.py
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     3052 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/virtualpdu/tests/snmp_error_indications.py
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      794 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/virtualpdu/tests/base.py
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-07 13:49:24.000000 virtualpdu-0.3.6/virtualpdu/tests/unit/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     3400 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/virtualpdu/tests/unit/test_transitive_state.py
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-07 13:49:24.000000 virtualpdu-0.3.6/virtualpdu/tests/unit/pdu/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      805 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/virtualpdu/tests/unit/pdu/test_base_pdu.py
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     2270 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/virtualpdu/tests/unit/pdu/test_baytech_mrp27.py
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        0 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/virtualpdu/tests/unit/pdu/__init__.py
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     2843 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/virtualpdu/tests/unit/pdu/base_pdu_test_cases.py
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     4373 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/virtualpdu/tests/unit/pdu/test_apc_rackpdu.py
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     3598 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/virtualpdu/tests/unit/test_core.py
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     3225 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/virtualpdu/tests/unit/test_main.py
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        0 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/virtualpdu/tests/unit/__init__.py
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-07 13:49:24.000000 virtualpdu-0.3.6/virtualpdu/tests/unit/drivers/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     8065 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/virtualpdu/tests/unit/drivers/test_libvirt_driver.py
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     1114 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/virtualpdu/tests/unit/drivers/test_driver.py
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        0 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/virtualpdu/tests/unit/drivers/__init__.py
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     5767 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/virtualpdu/tests/unit/test_snmp_client.py
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        0 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/virtualpdu/tests/__init__.py
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     2684 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/virtualpdu/tests/snmp_client.py
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      666 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/virtualpdu/__init__.py
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-07 13:49:24.000000 virtualpdu-0.3.6/virtualpdu/drivers/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     2810 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/virtualpdu/drivers/libvirt_driver.py
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      896 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/virtualpdu/drivers/__init__.py
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)       94 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/MANIFEST.in
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      451 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/README.rst
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      319 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/.testr.conf
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      162 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/HACKING.rst
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-07 13:49:24.000000 virtualpdu-0.3.6/virtualpdu.egg-info/
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        1 2017-03-07 13:49:20.000000 virtualpdu-0.3.6/virtualpdu.egg-info/not-zip-safe
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)       11 2017-03-07 13:49:23.000000 virtualpdu-0.3.6/virtualpdu.egg-info/top_level.txt
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)       46 2017-03-07 13:49:23.000000 virtualpdu-0.3.6/virtualpdu.egg-info/pbr.json
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)       53 2017-03-07 13:49:23.000000 virtualpdu-0.3.6/virtualpdu.egg-info/entry_points.txt
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     2258 2017-03-07 13:49:24.000000 virtualpdu-0.3.6/virtualpdu.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)        1 2017-03-07 13:49:23.000000 virtualpdu-0.3.6/virtualpdu.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     1408 2017-03-07 13:49:23.000000 virtualpdu-0.3.6/virtualpdu.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)       74 2017-03-07 13:49:23.000000 virtualpdu-0.3.6/virtualpdu.egg-info/requires.txt
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      985 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/tox.ini
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      326 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/requirements.txt
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     1408 2017-03-07 13:49:24.000000 virtualpdu-0.3.6/PKG-INFO
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     1023 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/setup.py
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-07 13:49:24.000000 virtualpdu-0.3.6/doc/
-drwxrwxr-x   0 jenkins   (3000) jenkins   (3001)        0 2017-03-07 13:49:24.000000 virtualpdu-0.3.6/doc/source/
--rwxrwxr-x   0 jenkins   (3000) jenkins   (3001)     2458 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/doc/source/conf.py
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      199 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/doc/source/installation.rst
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)       30 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/doc/source/readme.rst
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)       75 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/doc/source/contributing.rst
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)       81 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/doc/source/usage.rst
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      503 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/doc/source/index.rst
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)      101 2017-03-07 13:47:59.000000 virtualpdu-0.3.6/.coveragerc
--rw-rw-r--   0 jenkins   (3000) jenkins   (3001)     1876 2017-03-07 13:49:23.000000 virtualpdu-0.3.6/ChangeLog
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-25 14:40:54.600228 virtualpdu-1.0.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      766 2023-04-25 14:40:54.000000 virtualpdu-1.0.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      654 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2566 2023-04-25 14:40:54.000000 virtualpdu-1.0.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1504 2023-04-25 14:40:54.600228 virtualpdu-1.0.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-25 14:40:54.592229 virtualpdu-1.0.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      501 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/doc/example.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-25 14:40:54.592229 virtualpdu-1.0.0/doc/source/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2386 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/doc/source/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      503 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/doc/source/installation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/doc/source/readme.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/doc/source/usage.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-25 14:40:54.588229 virtualpdu-1.0.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-25 14:40:54.596228 virtualpdu-1.0.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/releasenotes/notes/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-25 14:40:54.596228 virtualpdu-1.0.0/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-25 14:40:54.596228 virtualpdu-1.0.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-25 14:40:54.596228 virtualpdu-1.0.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8926 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1167 2023-04-25 14:40:54.600228 virtualpdu-1.0.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      364 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3039 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-25 14:40:54.596228 virtualpdu-1.0.0/virtualpdu/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      666 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/virtualpdu/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2619 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/virtualpdu/core.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-25 14:40:54.596228 virtualpdu-1.0.0/virtualpdu/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      896 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/virtualpdu/drivers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2810 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/virtualpdu/drivers/libvirt_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5827 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/virtualpdu/main.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-25 14:40:54.596228 virtualpdu-1.0.0/virtualpdu/pdu/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4266 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/virtualpdu/pdu/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3860 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/virtualpdu/pdu/apc_rackpdu.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1962 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/virtualpdu/pdu/baytech_mrp27.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10042 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/virtualpdu/pdu/pysnmp_handler.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-25 14:40:54.596228 virtualpdu-1.0.0/virtualpdu/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/virtualpdu/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      794 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/virtualpdu/tests/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-25 14:40:54.596228 virtualpdu-1.0.0/virtualpdu/tests/integration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/virtualpdu/tests/integration/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-25 14:40:54.596228 virtualpdu-1.0.0/virtualpdu/tests/integration/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/virtualpdu/tests/integration/drivers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2030 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/virtualpdu/tests/integration/drivers/test_libvirt_driver.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-25 14:40:54.600228 virtualpdu-1.0.0/virtualpdu/tests/integration/pdu/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2783 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/virtualpdu/tests/integration/pdu/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2591 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/virtualpdu/tests/integration/pdu/test_apc_rackpdu.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2626 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/virtualpdu/tests/integration/pdu/test_baytech_mrp27.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2144 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/virtualpdu/tests/integration/pdu/test_pdu.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7641 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/virtualpdu/tests/integration/pdu/test_pysnmp_handler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3941 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/virtualpdu/tests/integration/test_core_integration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5766 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/virtualpdu/tests/integration/test_entrypoint.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4280 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/virtualpdu/tests/snmp_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3215 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/virtualpdu/tests/snmp_error_indications.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-25 14:40:54.600228 virtualpdu-1.0.0/virtualpdu/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1308 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/virtualpdu/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-25 14:40:54.600228 virtualpdu-1.0.0/virtualpdu/tests/unit/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/virtualpdu/tests/unit/drivers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1114 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/virtualpdu/tests/unit/drivers/test_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7905 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/virtualpdu/tests/unit/drivers/test_libvirt_driver.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-25 14:40:54.600228 virtualpdu-1.0.0/virtualpdu/tests/unit/pdu/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/virtualpdu/tests/unit/pdu/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2842 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/virtualpdu/tests/unit/pdu/base_pdu_test_cases.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4375 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/virtualpdu/tests/unit/pdu/test_apc_rackpdu.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/virtualpdu/tests/unit/pdu/test_base_pdu.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2272 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/virtualpdu/tests/unit/pdu/test_baytech_mrp27.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3603 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/virtualpdu/tests/unit/test_core.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3225 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/virtualpdu/tests/unit/test_main.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7940 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/virtualpdu/tests/unit/test_pysnmp_handler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5975 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/virtualpdu/tests/unit/test_snmp_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3404 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/virtualpdu/tests/unit/test_transitive_state.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-25 14:40:54.596228 virtualpdu-1.0.0/virtualpdu.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1504 2023-04-25 14:40:54.000000 virtualpdu-1.0.0/virtualpdu.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2357 2023-04-25 14:40:54.000000 virtualpdu-1.0.0/virtualpdu.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-04-25 14:40:54.000000 virtualpdu-1.0.0/virtualpdu.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2023-04-25 14:40:54.000000 virtualpdu-1.0.0/virtualpdu.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-04-25 14:40:54.000000 virtualpdu-1.0.0/virtualpdu.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-04-25 14:40:54.000000 virtualpdu-1.0.0/virtualpdu.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       50 2023-04-25 14:40:54.000000 virtualpdu-1.0.0/virtualpdu.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2023-04-25 14:40:54.000000 virtualpdu-1.0.0/virtualpdu.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-25 14:40:54.600228 virtualpdu-1.0.0/zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      356 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/zuul.d/project.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      514 2023-04-25 14:40:28.000000 virtualpdu-1.0.0/zuul.d/virtualpdu-jobs.yaml
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `virtualpdu-0.3.6/setup.cfg` & `virtualpdu-1.0.0/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 [metadata]
 name = virtualpdu
 summary = VirtualPDU is a service for simulating virtual power distribution outlets (PDUs).
-description-file = 
+description_file = 
 	README.rst
 author = OpenStack
-author-email = openstack-dev@lists.openstack.org
-home-page = http://www.openstack.org/
+author_email = openstack-discuss@lists.openstack.org
+home_page = https://opendev.org/x/virtualpdu
+python_requires = >=3.8
 classifier = 
 	Environment :: OpenStack
 	Intended Audience :: Information Technology
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: Apache Software License
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python
-	Programming Language :: Python :: 2
-	Programming Language :: Python :: 2.7
+	Programming Language :: Python :: Implementation :: CPython
+	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.3
-	Programming Language :: Python :: 3.4
+	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 
 [files]
 packages = 
 	virtualpdu
 
 [entry_points]
 console_scripts = 
@@ -31,28 +33,14 @@
 source-dir = doc/source
 build-dir = doc/build
 all_files = 1
 
 [upload_sphinx]
 upload-dir = doc/build/html
 
-[compile_catalog]
-directory = virtualpdu/locale
-domain = virtualpdu
-
-[update_catalog]
-domain = virtualpdu
-output_dir = virtualpdu/locale
-input_file = virtualpdu/locale/virtualpdu.pot
-
-[extract_messages]
-keywords = _ gettext ngettext l_ lazy_gettext
-mapping_file = babel.cfg
-output_file = virtualpdu/locale/virtualpdu.pot
-
 [build_releasenotes]
 all_files = 1
 build-dir = releasenotes/build
 source-dir = releasenotes/source
 
 [egg_info]
 tag_build =
```

### Comparing `virtualpdu-0.3.6/AUTHORS` & `virtualpdu-1.0.0/AUTHORS`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,20 @@
+Arundhati Surpur <arundhati@nectechnologies.in>
 Félix Bouliane <fbouliane@internap.com>
 Félix Bouliane <felixbouliane@hotmail.com>
+Ilya Etingof <etingof@gmail.com>
+Jay Faulkner <jay@jvf.cc>
 Jonathan Provost <jprovost.sh@gmail.com>
 Jonathan Provost <jprovost@internap.com>
 Marc Aubry <maubry@internap.com>
 Martin Roy <lindycoder@gmail.com>
 Mathieu Mitchell <mat128@gmail.com>
 Mathieu Mitchell <mmitchell@iweb.com>
 Maxime Dupuis <webf0x@hotmail.com>
 Philippe Godin <godp1301@gmail.com>
+Riccardo Pittau <elfosardo@gmail.com>
 Wajdi Al-Hawari <w.hawari@gmail.com>
 Wajdi Al-Hawari <wajdi@Wajdis-MacBook-Pro.local>
 Wajdi Al-Hawari <walhawari@iweb.com>
 mdupuis <mdupuis@internap.com>
 srobert <srobert@internap.com>
 stephanerobert <stephanerobert@users.noreply.github.com>
```

### Comparing `virtualpdu-0.3.6/CONTRIBUTING.rst` & `virtualpdu-1.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `virtualpdu-0.3.6/LICENSE` & `virtualpdu-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `virtualpdu-0.3.6/releasenotes/source/conf.py` & `virtualpdu-1.0.0/releasenotes/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 # If your documentation needs a minimal Sphinx version, state it here.
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
-    'oslosphinx',
     'reno.sphinxext',
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix of source filenames.
```

### Comparing `virtualpdu-0.3.6/virtualpdu/pdu/baytech_mrp27.py` & `virtualpdu-1.0.0/virtualpdu/pdu/baytech_mrp27.py`

 * *Files identical despite different names*

### Comparing `virtualpdu-0.3.6/virtualpdu/pdu/__init__.py` & `virtualpdu-1.0.0/virtualpdu/pdu/__init__.py`

 * *Files identical despite different names*

### Comparing `virtualpdu-0.3.6/virtualpdu/pdu/apc_rackpdu.py` & `virtualpdu-1.0.0/virtualpdu/pdu/apc_rackpdu.py`

 * *Files identical despite different names*

### Comparing `virtualpdu-0.3.6/virtualpdu/core.py` & `virtualpdu-1.0.0/virtualpdu/core.py`

 * *Files identical despite different names*

### Comparing `virtualpdu-0.3.6/virtualpdu/tests/integration/test_entrypoint.py` & `virtualpdu-1.0.0/virtualpdu/tests/integration/test_entrypoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,54 +7,57 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+import os
 import signal
 import subprocess
 import sys
 import tempfile
 import threading
 
-import os
 from pysnmp.entity.rfc3413.oneliner import cmdgen
 from retrying import retry
 
 from virtualpdu.pdu import apc_rackpdu
 from virtualpdu.pdu.apc_rackpdu import APCRackPDUOutletControl
 from virtualpdu.tests import base
 from virtualpdu.tests import snmp_client
 
 TEST_CONFIG = """[global]
 libvirt_uri=test:///default
 
 [my_pdu]
 listen_address=127.0.0.1
 listen_port=9998
+snmp_versions=1
 community=public
 ports=5:test
 
 [my_second_pdu]
 listen_address=127.0.0.1
 listen_port=9997
+snmp_versions=1
 community=public
 ports=2:test
 """
 
 
 class TestEntryPointIntegration(base.TestCase):
     def test_entry_point_works(self):
         p = subprocess.Popen([
             sys.executable, _get_entry_point_path('virtualpdu')],
             stderr=subprocess.PIPE
         )
         stdout, stderr = p.communicate()
-        self.assertEqual(
+        self.assertIn(
             b'Missing configuration file as first parameter.\n',
             stderr)
         self.assertEqual(1, p.returncode)
 
     def test_config(self):
         with tempfile.NamedTemporaryFile() as f:
             f.write(bytearray(TEST_CONFIG, encoding='utf-8'))
@@ -157,15 +160,15 @@
 
 
 def _turn_off_outlet(community, listen_address, outlet, port):
     outlet_oid = apc_rackpdu.rPDU_outlet_control_outlet_command + (outlet,)
     snmp_client_ = snmp_client.SnmpClient(cmdgen,
                                           listen_address,
                                           port,
-                                          community,
+                                          community=community,
                                           timeout=1,
                                           retries=1)
 
     snmp_client_.set(outlet_oid, APCRackPDUOutletControl.states.IMMEDIATE_OFF)
 
 
 def _get_entry_point_path(entry_point):
```

### Comparing `virtualpdu-0.3.6/virtualpdu/tests/integration/pdu/test_baytech_mrp27.py` & `virtualpdu-1.0.0/virtualpdu/tests/integration/pdu/test_baytech_mrp27.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
 from virtualpdu import core
 from virtualpdu.pdu.baytech_mrp27 import BaytechMRP27PDU
 from virtualpdu.pdu.baytech_mrp27 import BaytechMRP27PDUOutletControl
-
 from virtualpdu.tests.integration.pdu import PDUTestCase
 
 
 class TestBaytechMRP27PDU(PDUTestCase):
     pdu_class = BaytechMRP27PDU
     outlet_control_class = BaytechMRP27PDUOutletControl
```

### Comparing `virtualpdu-0.3.6/virtualpdu/tests/integration/pdu/test_pdu.py` & `virtualpdu-1.0.0/virtualpdu/tests/integration/pdu/test_pdu.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,19 +24,19 @@
 
 
 class TestPDU(PDUTestCase):
     pdu_class = pdu.PDU
     outlet_control_class = pdu.PDUOutletControl
 
     def test_get_unknown_oid(self):
-        self.assertRaises(RequestTimedOut,
-                          self.snmp_get, enterprises + (42,))
+        self.assertEqual(NoSuchInstance(''),
+                         self.snmp_get(enterprises + (42,)))
 
     def test_set_unknown_oid(self):
-        self.assertEqual(NoSuchInstance(),
+        self.assertEqual(NoSuchInstance(''),
                          self.snmp_set(enterprises + (42,), univ.Integer(7)))
 
     def test_get_valid_oid_wrong_community(self):
         self.core_mock.get_pdu_outlet_state.return_value = core.POWER_ON
         self.pdu.oid_mapping[enterprises + (88, 1)] = \
             pdu.PDUOutletControl(pdu_name=self.pdu.name,
                                  outlet_number=1,
```

### Comparing `virtualpdu-0.3.6/virtualpdu/tests/integration/pdu/__init__.py` & `virtualpdu-1.0.0/virtualpdu/tests/integration/pdu/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from mock import mock
-from pysnmp.entity.rfc3413.oneliner import cmdgen
 import random
+from unittest import mock
+
+from pysnmp.entity.rfc3413.oneliner import cmdgen
 
 from virtualpdu.pdu import pysnmp_handler
 from virtualpdu.tests import base
 from virtualpdu.tests import snmp_client
 
 
 class PDUTestCase(base.TestCase):
@@ -30,41 +31,42 @@
         self.community = 'test1212'
         self.core_mock = mock.Mock()
         self.pdu = self.pdu_class(name='test_pdu', core=self.core_mock)
         self.pdu_test_harness = pysnmp_handler.SNMPPDUHarness(
             self.pdu,
             '127.0.0.1',
             random.randint(20000, 30000),
-            self.community)
+            snmp_versions=['1', '2c'],
+            community=self.community)
         self.pdu_test_harness.start()
 
     def tearDown(self):
         self.pdu_test_harness.stop()
         super(PDUTestCase, self).tearDown()
 
     def snmp_get(self, oid, community=None):
         s = snmp_client.SnmpClient(cmdgen,
                                    self.pdu_test_harness.listen_address,
                                    self.pdu_test_harness.listen_port,
-                                   community or self.community,
+                                   community=community or self.community,
                                    timeout=1,
                                    retries=1)
         return s.get_one(oid)
 
     def snmp_get_next(self, oid, community=None):
         s = snmp_client.SnmpClient(cmdgen,
                                    self.pdu_test_harness.listen_address,
                                    self.pdu_test_harness.listen_port,
-                                   community or self.community,
+                                   community=community or self.community,
                                    timeout=1,
                                    retries=1)
         return s.get_next(oid)
 
     def snmp_set(self, oid, value, community=None):
         s = snmp_client.SnmpClient(cmdgen,
                                    self.pdu_test_harness.listen_address,
                                    self.pdu_test_harness.listen_port,
-                                   community or self.community,
+                                   community=community or self.community,
                                    timeout=1,
                                    retries=1)
 
         return s.set(oid, value)
```

### Comparing `virtualpdu-0.3.6/virtualpdu/tests/integration/pdu/test_apc_rackpdu.py` & `virtualpdu-1.0.0/virtualpdu/tests/integration/pdu/test_apc_rackpdu.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
 from virtualpdu import core
 from virtualpdu.pdu.apc_rackpdu import APCRackPDU
 from virtualpdu.pdu.apc_rackpdu import APCRackPDUOutletControl
-
 from virtualpdu.tests.integration.pdu import PDUTestCase
 
 
 class TestAPCRackPDU(PDUTestCase):
     pdu_class = APCRackPDU
     outlet_control_class = APCRackPDUOutletControl
```

### Comparing `virtualpdu-0.3.6/virtualpdu/tests/integration/drivers/test_libvirt_driver.py` & `virtualpdu-1.0.0/virtualpdu/tests/integration/drivers/test_libvirt_driver.py`

 * *Files identical despite different names*

### Comparing `virtualpdu-0.3.6/virtualpdu/tests/integration/test_core_integration.py` & `virtualpdu-1.0.0/virtualpdu/tests/integration/test_core_integration.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import random
 import time
 
 from pysnmp.entity.rfc3413.oneliner import cmdgen
+
 from virtualpdu import core
 from virtualpdu import drivers
 from virtualpdu.drivers import libvirt_driver
 from virtualpdu.pdu import apc_rackpdu
 from virtualpdu.pdu import pysnmp_handler
 from virtualpdu.tests import base
 from virtualpdu.tests import snmp_client
@@ -43,24 +44,24 @@
         super(TestCoreIntegration, self).tearDown()
 
     def get_harness_client(self, pdu_):
         listen_address = '127.0.0.1'
         port = random.randint(20000, 30000)
         community = 'public'
 
-        self.pdu_test_harness = pysnmp_handler.SNMPPDUHarness(pdu_,
-                                                              listen_address,
-                                                              port,
-                                                              community)
+        self.pdu_test_harness = pysnmp_handler.SNMPPDUHarness(
+            pdu_, listen_address, port,
+            snmp_versions=['1', '2c'], community=community
+        )
         self.pdu_test_harness.start()
 
         return snmp_client.SnmpClient(cmdgen,
                                       listen_address,
                                       port,
-                                      community,
+                                      community=community,
                                       timeout=1,
                                       retries=1)
 
     def test_set_pdu_outlet_command_on_power_off(self):
         pdu = apc_rackpdu.APCRackPDU('my_pdu', self.core)
         snmp_client_ = self.get_harness_client(pdu)
```

### Comparing `virtualpdu-0.3.6/virtualpdu/tests/snmp_error_indications.py` & `virtualpdu-1.0.0/virtualpdu/tests/snmp_error_indications.py`

 * *Files 3% similar despite different names*

```diff
@@ -171,7 +171,19 @@
 
 class SNMPApplicationError(SNMPErrorIndication):
     pass
 
 
 class OidNotIncreasing(SNMPApplicationError):
     pass
+
+
+class ReportPduReceived(SNMPErrorIndication):
+    pass
+
+
+class UnknownUserName(SNMPErrorIndication):
+    pass
+
+
+class WrongDigest(SNMPErrorIndication):
+    pass
```

### Comparing `virtualpdu-0.3.6/virtualpdu/tests/base.py` & `virtualpdu-1.0.0/virtualpdu/tests/base.py`

 * *Files identical despite different names*

### Comparing `virtualpdu-0.3.6/virtualpdu/tests/unit/test_transitive_state.py` & `virtualpdu-1.0.0/virtualpdu/tests/unit/test_transitive_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import threading
+from unittest import mock
 
-from mock import mock
 from virtualpdu import core
 from virtualpdu import drivers
 from virtualpdu.tests import base
 
 
 class TestTransitiveState(base.TestCase):
     def setUp(self):
```

### Comparing `virtualpdu-0.3.6/virtualpdu/tests/unit/pdu/test_base_pdu.py` & `virtualpdu-1.0.0/virtualpdu/tests/unit/pdu/test_base_pdu.py`

 * *Files identical despite different names*

### Comparing `virtualpdu-0.3.6/virtualpdu/tests/unit/pdu/test_baytech_mrp27.py` & `virtualpdu-1.0.0/virtualpdu/tests/unit/pdu/test_baytech_mrp27.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
 from pyasn1.type import univ
+
 from virtualpdu.pdu import baytech_mrp27
 from virtualpdu.pdu import sysDescr
 from virtualpdu.pdu import sysObjectID
 from virtualpdu.tests import base
 from virtualpdu.tests.unit.pdu.base_pdu_test_cases import BasePDUTests
```

### Comparing `virtualpdu-0.3.6/virtualpdu/tests/unit/pdu/base_pdu_test_cases.py` & `virtualpdu-1.0.0/virtualpdu/tests/unit/pdu/base_pdu_test_cases.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,28 +7,30 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from cached_property import cached_property
-from mock import mock
+
+import functools
+from unittest import mock
+
 from virtualpdu import core
 
 
 class BasePDUTests(object):
     pdu_class = None
     outlet_control_oid = None
 
-    @cached_property
+    @functools.cached_property
     def core_mock(self):
         return mock.Mock()
 
-    @cached_property
+    @functools.cached_property
     def pdu(self):
         return self.pdu_class(name='my_pdu', core=self.core_mock)
 
     def test_power_on_notifies_core(self):
         outlet_control = self.pdu.oid_mapping[self.outlet_control_oid]
         outlet_control.value = \
             outlet_control.states.from_core(core.POWER_ON)
```

### Comparing `virtualpdu-0.3.6/virtualpdu/tests/unit/pdu/test_apc_rackpdu.py` & `virtualpdu-1.0.0/virtualpdu/tests/unit/pdu/test_apc_rackpdu.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
 from pyasn1.type import univ
+
 from virtualpdu import core
 from virtualpdu.pdu import apc_rackpdu
 from virtualpdu.pdu import sysDescr
 from virtualpdu.pdu import sysObjectID
 from virtualpdu.tests import base
 from virtualpdu.tests.unit.pdu.base_pdu_test_cases import BasePDUTests
```

### Comparing `virtualpdu-0.3.6/virtualpdu/tests/unit/test_core.py` & `virtualpdu-1.0.0/virtualpdu/tests/unit/test_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
 import time
+from unittest import mock
 
-from mock import mock
 from virtualpdu import core
 from virtualpdu import drivers
 from virtualpdu.tests import base
 
 
 class TestCore(base.TestCase):
     def setUp(self):
```

### Comparing `virtualpdu-0.3.6/virtualpdu/tests/unit/test_main.py` & `virtualpdu-1.0.0/virtualpdu/tests/unit/test_main.py`

 * *Files identical despite different names*

### Comparing `virtualpdu-0.3.6/virtualpdu/tests/unit/drivers/test_libvirt_driver.py` & `virtualpdu-1.0.0/virtualpdu/tests/unit/drivers/test_libvirt_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from unittest import mock
+
 import libvirt
-from mock import mock
 
 from virtualpdu import drivers
 from virtualpdu.drivers import libvirt_driver
 from virtualpdu.tests import base
 
 DOMAIN_ALREADY_RUNNING = "internal error: Domain '{}' is already running"
 DOMAIN_NOT_RUNNING = "Requested operation is not valid: domain is not running"
@@ -113,40 +114,37 @@
         connection_mock.lookupByName.assert_called_with('domainA')
         domain_mock.isActive.assert_called_with()
         connection_mock.close.assert_called_with()
 
     def test_get_power_state_domain_not_found(self, mock_open):
         connection_mock = mock.Mock()
         connection_mock.lookupByName.side_effect = \
-            libvirt.libvirtError('virDomainLookupByName() failed',
-                                 conn=connection_mock)
+            libvirt.libvirtError('virDomainLookupByName() failed')
         mock_open.return_value = connection_mock
 
         self.assertRaises(drivers.DeviceNotFound,
                           self.driver.get_power_state, 'domainA')
 
         connection_mock.close.assert_called_with()
 
     def test_power_on_domain_not_found(self, mock_open):
         connection_mock = mock.Mock()
         connection_mock.lookupByName.side_effect = \
-            libvirt.libvirtError('virDomainLookupByName() failed',
-                                 conn=connection_mock)
+            libvirt.libvirtError('virDomainLookupByName() failed')
         mock_open.return_value = connection_mock
 
         self.assertRaises(drivers.DeviceNotFound,
                           self.driver.power_on, 'domainA')
 
         connection_mock.close.assert_called_with()
 
     def test_power_off_domain_not_found(self, mock_open):
         connection_mock = mock.Mock()
         connection_mock.lookupByName.side_effect = \
-            libvirt.libvirtError('virDomainLookupByName() failed',
-                                 conn=connection_mock)
+            libvirt.libvirtError('virDomainLookupByName() failed')
         mock_open.return_value = connection_mock
 
         self.assertRaises(drivers.DeviceNotFound,
                           self.driver.power_off, 'domainA')
 
         connection_mock.close.assert_called_with()
```

### Comparing `virtualpdu-0.3.6/virtualpdu/tests/unit/drivers/test_driver.py` & `virtualpdu-1.0.0/virtualpdu/tests/unit/drivers/test_driver.py`

 * *Files identical despite different names*

### Comparing `virtualpdu-0.3.6/virtualpdu/tests/unit/test_snmp_client.py` & `virtualpdu-1.0.0/virtualpdu/tests/unit/test_snmp_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,19 +8,22 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from mock import mock
-from mock import sentinel
+from unittest import mock
+from unittest.mock import sentinel
+
 from pysnmp.proto import errind
 from pysnmp.proto.errind import ErrorIndication
 from pysnmp.proto.rfc1905 import NoSuchInstance
+import testtools
+
 from virtualpdu.tests import base
 from virtualpdu.tests import snmp_client
 from virtualpdu.tests import snmp_error_indications
 
 
 class TestSnmpClient(base.TestCase):
     def setUp(self):
@@ -73,72 +76,74 @@
         self.assertEqual('42 thousands', value)
 
         self.oneliner_cmdgen.UdpTransportTarget\
             .assert_called_with((sentinel.hostname, sentinel.port),
                                 timeout=sentinel.timeout,
                                 retries=sentinel.retries)
         self.oneliner_cmdgen.CommunityData\
-            .assert_called_with(sentinel.community)
+            .assert_called_with(sentinel.community, mpModel=0)
         self.command_generator_mock.getCmd.assert_called_with(
             sentinel.community_data,
             sentinel.udp_transport_target,
-            oid
+            oid, contextEngineId=None, contextName=''
         )
 
     def test_get_with_all_possible_error_indications(self):
         oid = (1, 3, 6)
         for class_name, error_indication in self.all_error_indications:
             self.command_generator_mock.getCmd.return_value = \
                 (error_indication, 0, 0, [])
 
             exception_class = snmp_error_indications.__dict__.get(class_name)
 
-            self.assertRaises(exception_class,
-                              self.snmp_client.get_one, oid)
+            with testtools.ExpectedException(exception_class):
+                self.snmp_client.get_one(oid)
 
     def test_set(self):
         oid = (1, 3, 6)
         self.command_generator_mock.setCmd.return_value = \
             (None, 0, 0, [(oid, '43 thousands')])
         value = self.snmp_client.set(oid, '43 thousands')
 
         self.assertEqual('43 thousands', value)
 
         self.oneliner_cmdgen.UdpTransportTarget\
             .assert_called_with((sentinel.hostname, sentinel.port),
                                 timeout=sentinel.timeout,
                                 retries=sentinel.retries)
         self.oneliner_cmdgen.CommunityData\
-            .assert_called_with(sentinel.community)
+            .assert_called_with(sentinel.community, mpModel=0)
         self.command_generator_mock.setCmd.assert_called_with(
             sentinel.community_data,
             sentinel.udp_transport_target,
-            (oid, '43 thousands')
+            (oid, '43 thousands'),
+            contextEngineId=None, contextName=''
         )
 
     def test_set_no_such_instance(self):
         oid = (1, 3, 6)
         self.command_generator_mock.setCmd.return_value = \
-            (None, 0, 0, [(oid, NoSuchInstance())])
+            (None, 0, 0, [(oid, NoSuchInstance(''))])
         value = self.snmp_client.set(oid, '43 thousands')
 
-        self.assertEqual(NoSuchInstance(), value)
+        self.assertEqual(NoSuchInstance(''), value)
 
         self.oneliner_cmdgen.UdpTransportTarget \
             .assert_called_with((sentinel.hostname, sentinel.port),
                                 timeout=sentinel.timeout,
                                 retries=sentinel.retries)
 
         self.oneliner_cmdgen.CommunityData \
-            .assert_called_with(sentinel.community)
+            .assert_called_with(sentinel.community, mpModel=0)
 
         self.command_generator_mock.setCmd.assert_called_with(
             sentinel.community_data,
             sentinel.udp_transport_target,
-            (oid, '43 thousands')
+            (oid, '43 thousands'),
+            contextEngineId=None, contextName=''
         )
 
     def test_set_with_all_possible_error_indications(self):
         oid = (1, 3, 6)
         for class_name, error_indication in self.all_error_indications:
             self.command_generator_mock.setCmd.return_value = \
                 (error_indication, 0, 0, [])
```

### Comparing `virtualpdu-0.3.6/virtualpdu/__init__.py` & `virtualpdu-1.0.0/virtualpdu/__init__.py`

 * *Files identical despite different names*

### Comparing `virtualpdu-0.3.6/virtualpdu/drivers/libvirt_driver.py` & `virtualpdu-1.0.0/virtualpdu/drivers/libvirt_driver.py`

 * *Files identical despite different names*

### Comparing `virtualpdu-0.3.6/virtualpdu/drivers/__init__.py` & `virtualpdu-1.0.0/virtualpdu/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `virtualpdu-0.3.6/virtualpdu.egg-info/SOURCES.txt` & `virtualpdu-1.0.0/virtualpdu.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 .coveragerc
-.mailmap
-.testr.conf
-.travis.yml
+.stestr.conf
 AUTHORS
 CONTRIBUTING.rst
 ChangeLog
 HACKING.rst
 LICENSE
-MANIFEST.in
 README.rst
-babel.cfg
+bindep.txt
 requirements.txt
 setup.cfg
 setup.py
 test-requirements.txt
 tox.ini
+doc/example.ini
+doc/requirements.txt
 doc/source/conf.py
 doc/source/contributing.rst
 doc/source/index.rst
 doc/source/installation.rst
 doc/source/readme.rst
 doc/source/usage.rst
 releasenotes/notes/.placeholder
@@ -57,17 +56,20 @@
 virtualpdu/tests/integration/pdu/test_apc_rackpdu.py
 virtualpdu/tests/integration/pdu/test_baytech_mrp27.py
 virtualpdu/tests/integration/pdu/test_pdu.py
 virtualpdu/tests/integration/pdu/test_pysnmp_handler.py
 virtualpdu/tests/unit/__init__.py
 virtualpdu/tests/unit/test_core.py
 virtualpdu/tests/unit/test_main.py
+virtualpdu/tests/unit/test_pysnmp_handler.py
 virtualpdu/tests/unit/test_snmp_client.py
 virtualpdu/tests/unit/test_transitive_state.py
 virtualpdu/tests/unit/drivers/__init__.py
 virtualpdu/tests/unit/drivers/test_driver.py
 virtualpdu/tests/unit/drivers/test_libvirt_driver.py
 virtualpdu/tests/unit/pdu/__init__.py
 virtualpdu/tests/unit/pdu/base_pdu_test_cases.py
 virtualpdu/tests/unit/pdu/test_apc_rackpdu.py
 virtualpdu/tests/unit/pdu/test_base_pdu.py
-virtualpdu/tests/unit/pdu/test_baytech_mrp27.py
+virtualpdu/tests/unit/pdu/test_baytech_mrp27.py
+zuul.d/project.yaml
+zuul.d/virtualpdu-jobs.yaml
```

### Comparing `virtualpdu-0.3.6/virtualpdu.egg-info/PKG-INFO` & `virtualpdu-1.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,37 @@
-Metadata-Version: 1.1
+Metadata-Version: 1.2
 Name: virtualpdu
-Version: 0.3.6
+Version: 1.0.0
 Summary: VirtualPDU is a service for simulating virtual power distribution outlets (PDUs).
-Home-page: http://www.openstack.org/
+Home-page: https://opendev.org/x/virtualpdu
 Author: OpenStack
-Author-email: openstack-dev@lists.openstack.org
+Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ===============================
         virtualpdu
         ===============================
         
         VirtualPDU is a service for simulating virtual power distribution outlets
         (PDUs).
         
-        virtualpdu is licensed under the Apache License like the rest of OpenStack.
+        This software is intended for CI and development use only. Please do not run
+        VirtualPDU in a production environment for any reason.
         
         * Free software: Apache license, Version 2.0
-        * Documentation: http://docs.openstack.org/developer/virtualpdu
-        * Source: http://git.openstack.org/cgit/openstack/virtualpdu
+        * Source: http://opendev.org/openstack/virtualpdu
         * Bugs: http://bugs.launchpad.net/virtualpdu
         
         
 Platform: UNKNOWN
 Classifier: Environment :: OpenStack
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8
```

### Comparing `virtualpdu-0.3.6/PKG-INFO` & `virtualpdu-1.0.0/virtualpdu.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,37 @@
-Metadata-Version: 1.1
+Metadata-Version: 1.2
 Name: virtualpdu
-Version: 0.3.6
+Version: 1.0.0
 Summary: VirtualPDU is a service for simulating virtual power distribution outlets (PDUs).
-Home-page: http://www.openstack.org/
+Home-page: https://opendev.org/x/virtualpdu
 Author: OpenStack
-Author-email: openstack-dev@lists.openstack.org
+Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ===============================
         virtualpdu
         ===============================
         
         VirtualPDU is a service for simulating virtual power distribution outlets
         (PDUs).
         
-        virtualpdu is licensed under the Apache License like the rest of OpenStack.
+        This software is intended for CI and development use only. Please do not run
+        VirtualPDU in a production environment for any reason.
         
         * Free software: Apache license, Version 2.0
-        * Documentation: http://docs.openstack.org/developer/virtualpdu
-        * Source: http://git.openstack.org/cgit/openstack/virtualpdu
+        * Source: http://opendev.org/openstack/virtualpdu
         * Bugs: http://bugs.launchpad.net/virtualpdu
         
         
 Platform: UNKNOWN
 Classifier: Environment :: OpenStack
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8
```

### Comparing `virtualpdu-0.3.6/doc/source/conf.py` & `virtualpdu-1.0.0/doc/source/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
@@ -18,16 +17,14 @@
 sys.path.insert(0, os.path.abspath('../..'))
 # -- General configuration ----------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = [
     'sphinx.ext.autodoc',
-    #'sphinx.ext.intersphinx',
-    'oslosphinx'
 ]
 
 # autodoc generation is a bit aggressive and a nuisance when doing heavy
 # text edit cycles.
 # execute "export SPHINX_DEBUG=1" in your terminal to disable
 
 # The suffix of source filenames.
```

### Comparing `virtualpdu-0.3.6/ChangeLog` & `virtualpdu-1.0.0/ChangeLog`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,32 @@
 CHANGES
 =======
 
+1.0.0
+-----
+
+* Update pep8 deps - hacking to 6.0.0
+* Add doc8 test to pep8
+* Remove useless config files
+* Remove ignore F811 flake8 rule
+* Fix gitreview; Minor update to readme
+* Remove all related translation config from setup.cfg
+* Follow up for migration to Python 3
+* Move virtualpdu to Python 3
+* OpenDev Migration Patch
+* added SNMPv3 support
+* SNMP agent rebased on the high-level pysnmp API
+* fix uninitialized ASN.1 objects use
+* Add test for the pysnmp handler
+* Drop MANIFEST.in - it's not needed by pbr
+* There is no documentation for virtualpdu
+* Add link to docker container in readme
+* Removes unnecessary utf-8 encoding
+* Add errors that were added with pysnmp 4.3.6
+
 0.3.6
 -----
 
 * Updating pyasn1 and pysnmp<5.0.0,>=4.3.4
 
 0.3.5
 -----
@@ -27,15 +49,15 @@
 -----
 
 * Add support for custom PDU outlet count
 
 0.3.1
 -----
 
-* Store POWER_ON state when performing a REBOOT
+* Store POWER\_ON state when performing a REBOOT
 * Make sure virtualpdu is tested on py27,34,35
 * Fix PEP8
 
 0.3.0
 -----
 
 * Taking executor out of the context
@@ -63,15 +85,15 @@
 * Add Baytech MRP27 support
 * Outlet's default power state is now configurable
 
 0.1.0
 -----
 
 * Handle SIGINT correctly on Python 2.7
-* Support listen_address in config instead of listen_host
+* Support listen\_address in config instead of listen\_host
 * Adding Updated Tox
 * Creating Main Application Wrapper
 
 0.0.4
 -----
 
 * Permission Issues with PyPi. Trying again
@@ -86,15 +108,15 @@
 
 * Supporting PyPi Upload Via Travis
 * Introduce the virtualpdu entry point
 * Using the Power States Defined in The Core
 * Implementation of the Core for VPDU
 * Fixing intermittent unit test failures
 * Adding Explicit Tests for Power State
-* Introduce get_power_state for drivers
+* Introduce get\_power\_state for drivers
 * Ensure APCRackPDU instanciation does not update core
 * Introduce power distribution units SNMP agents
 * Rename device providers to drivers
 * Introduce libvirt device provider
 * Disable pypy tox target
 * Introduce travis configuration using tox-travis
 * Initial Cookiecutter Commit
```

