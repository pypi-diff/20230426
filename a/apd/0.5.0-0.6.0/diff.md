# Comparing `tmp/apd-0.5.0.tar.gz` & `tmp/apd-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apd-0.5.0.tar", last modified: Fri Apr 14 13:31:01 2023, max compression
+gzip compressed data, was "apd-0.6.0.tar", last modified: Wed Apr 26 10:40:20 2023, max compression
```

## Comparing `apd-0.5.0.tar` & `apd-0.6.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 13:31:01.384000 apd-0.5.0/
--rw-r--r--   0 root         (0) root         (0)     2075 2023-04-14 13:30:38.000000 apd-0.5.0/.gitignore
--rw-r--r--   0 root         (0) root         (0)     2001 2023-04-14 13:30:38.000000 apd-0.5.0/.gitlab-ci.yml
--rw-r--r--   0 root         (0) root         (0)     1066 2023-04-14 13:30:38.000000 apd-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)      596 2023-04-14 13:30:38.000000 apd-0.5.0/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)    35149 2023-04-14 13:30:38.000000 apd-0.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4204 2023-04-14 13:31:01.384000 apd-0.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3786 2023-04-14 13:30:38.000000 apd-0.5.0/README.rst
--rw-r--r--   0 root         (0) root         (0)      572 2023-04-14 13:30:38.000000 apd-0.5.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1329 2023-04-14 13:31:01.384000 apd-0.5.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 13:31:01.372000 apd-0.5.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 13:31:01.376000 apd-0.5.0/src/apd/
--rw-r--r--   0 root         (0) root         (0)     1196 2023-04-14 13:30:38.000000 apd-0.5.0/src/apd/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15871 2023-04-14 13:30:38.000000 apd-0.5.0/src/apd/analysis_data.py
--rw-r--r--   0 root         (0) root         (0)    13854 2023-04-14 13:30:38.000000 apd-0.5.0/src/apd/ap_info.py
--rw-r--r--   0 root         (0) root         (0)     6433 2023-04-14 13:30:38.000000 apd-0.5.0/src/apd/authentication.py
--rw-r--r--   0 root         (0) root         (0)    15411 2023-04-14 13:30:38.000000 apd-0.5.0/src/apd/command.py
--rw-r--r--   0 root         (0) root         (0)     2489 2023-04-14 13:30:38.000000 apd-0.5.0/src/apd/data_cache.py
--rw-r--r--   0 root         (0) root         (0)     3648 2023-04-14 13:30:38.000000 apd-0.5.0/src/apd/eos.py
--rw-r--r--   0 root         (0) root         (0)      921 2023-04-14 13:30:38.000000 apd-0.5.0/src/apd/rich_console.py
--rw-r--r--   0 root         (0) root         (0)     3057 2023-04-14 13:30:38.000000 apd-0.5.0/src/apd/snakemake.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 13:31:01.376000 apd-0.5.0/src/apd.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4204 2023-04-14 13:31:01.000000 apd-0.5.0/src/apd.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      739 2023-04-14 13:31:01.000000 apd-0.5.0/src/apd.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 13:31:01.000000 apd-0.5.0/src/apd.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      354 2023-04-14 13:31:01.000000 apd-0.5.0/src/apd.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-04-14 13:31:01.000000 apd-0.5.0/src/apd.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-04-14 13:31:01.000000 apd-0.5.0/src/apd.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 13:31:01.376000 apd-0.5.0/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 13:31:01.372000 apd-0.5.0/tests/cache-dir/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 13:31:01.380000 apd-0.5.0/tests/cache-dir/b2oc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 13:31:01.384000 apd-0.5.0/tests/cache-dir/b2oc/b02dkpi/
--rw-r--r--   0 root         (0) root         (0)   157583 2023-04-14 13:30:38.000000 apd-0.5.0/tests/cache-dir/b2oc/b02dkpi/tags.json
--rw-r--r--   0 root         (0) root         (0)  2657491 2023-04-14 13:30:38.000000 apd-0.5.0/tests/cache-dir/b2oc/b02dkpi.json
--rw-r--r--   0 root         (0) root         (0)     3197 2023-04-14 13:30:38.000000 apd-0.5.0/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 13:31:01.384000 apd-0.5.0/tests/data/
--rw-r--r--   0 root         (0) root         (0)    22577 2023-04-14 13:30:38.000000 apd-0.5.0/tests/data/rds_ap_info.json
--rw-r--r--   0 root         (0) root         (0)    22577 2023-04-14 13:30:38.000000 apd-0.5.0/tests/data/rds_ap_info_2versions.json
--rw-r--r--   0 root         (0) root         (0)     4225 2023-04-14 13:30:38.000000 apd-0.5.0/tests/test_analysis_data.py
--rw-r--r--   0 root         (0) root         (0)     4633 2023-04-14 13:30:38.000000 apd-0.5.0/tests/test_ap_info.py
--rw-r--r--   0 root         (0) root         (0)     9296 2023-04-14 13:30:38.000000 apd-0.5.0/tests/test_b2oc.py
--rw-r--r--   0 root         (0) root         (0)     2201 2023-04-14 13:30:38.000000 apd-0.5.0/tests/test_data_cache.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:40:20.384000 apd-0.6.0/
+-rw-r--r--   0 root         (0) root         (0)     2075 2023-04-26 10:39:57.000000 apd-0.6.0/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     2001 2023-04-26 10:39:57.000000 apd-0.6.0/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)     1066 2023-04-26 10:39:57.000000 apd-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      596 2023-04-26 10:39:57.000000 apd-0.6.0/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-04-26 10:39:57.000000 apd-0.6.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2850 2023-04-26 10:40:20.384000 apd-0.6.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2432 2023-04-26 10:39:57.000000 apd-0.6.0/README.rst
+-rw-r--r--   0 root         (0) root         (0)      572 2023-04-26 10:39:57.000000 apd-0.6.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1329 2023-04-26 10:40:20.384000 apd-0.6.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:40:20.372000 apd-0.6.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:40:20.376000 apd-0.6.0/src/apd/
+-rw-r--r--   0 root         (0) root         (0)     1453 2023-04-26 10:39:57.000000 apd-0.6.0/src/apd/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16999 2023-04-26 10:39:57.000000 apd-0.6.0/src/apd/analysis_data.py
+-rw-r--r--   0 root         (0) root         (0)    15796 2023-04-26 10:39:57.000000 apd-0.6.0/src/apd/ap_info.py
+-rw-r--r--   0 root         (0) root         (0)     6433 2023-04-26 10:39:57.000000 apd-0.6.0/src/apd/authentication.py
+-rw-r--r--   0 root         (0) root         (0)    13676 2023-04-26 10:39:57.000000 apd-0.6.0/src/apd/command.py
+-rw-r--r--   0 root         (0) root         (0)     2475 2023-04-26 10:39:57.000000 apd-0.6.0/src/apd/data_cache.py
+-rw-r--r--   0 root         (0) root         (0)     3648 2023-04-26 10:39:57.000000 apd-0.6.0/src/apd/eos.py
+-rw-r--r--   0 root         (0) root         (0)      921 2023-04-26 10:39:57.000000 apd-0.6.0/src/apd/rich_console.py
+-rw-r--r--   0 root         (0) root         (0)     3057 2023-04-26 10:39:57.000000 apd-0.6.0/src/apd/snakemake.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:40:20.376000 apd-0.6.0/src/apd.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2850 2023-04-26 10:40:20.000000 apd-0.6.0/src/apd.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      739 2023-04-26 10:40:20.000000 apd-0.6.0/src/apd.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 10:40:20.000000 apd-0.6.0/src/apd.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      354 2023-04-26 10:40:20.000000 apd-0.6.0/src/apd.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-04-26 10:40:20.000000 apd-0.6.0/src/apd.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-26 10:40:20.000000 apd-0.6.0/src/apd.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:40:20.376000 apd-0.6.0/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:40:20.372000 apd-0.6.0/tests/cache-dir/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:40:20.376000 apd-0.6.0/tests/cache-dir/b2oc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:40:20.380000 apd-0.6.0/tests/cache-dir/b2oc/b02dkpi/
+-rw-r--r--   0 root         (0) root         (0)   157583 2023-04-26 10:39:57.000000 apd-0.6.0/tests/cache-dir/b2oc/b02dkpi/tags.json
+-rw-r--r--   0 root         (0) root         (0)  2657491 2023-04-26 10:39:57.000000 apd-0.6.0/tests/cache-dir/b2oc/b02dkpi.json
+-rw-r--r--   0 root         (0) root         (0)     3272 2023-04-26 10:39:57.000000 apd-0.6.0/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 10:40:20.384000 apd-0.6.0/tests/data/
+-rw-r--r--   0 root         (0) root         (0)    22577 2023-04-26 10:39:57.000000 apd-0.6.0/tests/data/rds_ap_info.json
+-rw-r--r--   0 root         (0) root         (0)    22577 2023-04-26 10:39:57.000000 apd-0.6.0/tests/data/rds_ap_info_2versions.json
+-rw-r--r--   0 root         (0) root         (0)     4692 2023-04-26 10:39:57.000000 apd-0.6.0/tests/test_analysis_data.py
+-rw-r--r--   0 root         (0) root         (0)     4633 2023-04-26 10:39:57.000000 apd-0.6.0/tests/test_ap_info.py
+-rw-r--r--   0 root         (0) root         (0)     7490 2023-04-26 10:39:57.000000 apd-0.6.0/tests/test_b2oc.py
+-rw-r--r--   0 root         (0) root         (0)     2201 2023-04-26 10:39:57.000000 apd-0.6.0/tests/test_data_cache.py
```

### Comparing `apd-0.5.0/.gitignore` & `apd-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `apd-0.5.0/.gitlab-ci.yml` & `apd-0.6.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `apd-0.5.0/.pre-commit-config.yaml` & `apd-0.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `apd-0.5.0/CONTRIBUTING.md` & `apd-0.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `apd-0.5.0/LICENSE` & `apd-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `apd-0.5.0/pyproject.toml` & `apd-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apd-0.5.0/setup.cfg` & `apd-0.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `apd-0.5.0/src/apd/analysis_data.py` & `apd-0.6.0/src/apd/analysis_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,69 +1,132 @@
 ###############################################################################
-# (c) Copyright 2021-2022 for the benefit of the LHCb Collaboration           #
+# (c) Copyright 2021-2023 for the benefit of the LHCb Collaboration           #
 #                                                                             #
 # This software is distributed under the terms of the GNU General Public      #
 # Licence version 3 (GPL Version 3), copied verbatim in the file "COPYING".   #
 #                                                                             #
 # In applying this licence, CERN does not waive the privileges and immunities #
 # granted to it by virtue of its status as an Intergovernmental Organization  #
 # or submit itself to any jurisdiction.                                       #
 ###############################################################################
+"""Interface to the Analysis Production data.
 
+Provides:
+    * the get_analysis_data method, the principal way to lookup AP info. It returns
+    and AnalysisData class.
+    * the AnalysisData class, which allows querying information about Analysis Productions
+
+"""
 import copy
 import itertools
 import logging
 import os
+from pathlib import Path
 
 from apd.ap_info import (
+    InvalidCacheError,
     SampleCollection,
-    check_tag_in_list,
-    fetch_ap_info,
+    cache_ap_info,
+    check_tag_value_possible,
     iterable,
     load_ap_info,
     safe_casefold,
 )
 from apd.data_cache import DataCache
 
 logger = logging.getLogger("apd")
 
 APD_METADATA_CACHE_DIR = "APD_METADATA_CACHE_DIR"
 APD_METADATA_LIFETIME = "APD_METADATA_LIFETIME"
+APD_METADATA_LIFETIME_DEFAULT = 600
 APD_DATA_CACHE_DIR = "APD_DATA_CACHE_DIR"
 
 
+def _load_and_setup_cache(
+    cache_dir, working_group, analysis, ap_date=None, api_url="https://lbap.app.cern.ch"
+):
+    """Utility function that checks whether the data for the Analysis
+    is cached already and does it if needed."""
+    env_cache = os.environ.get(APD_METADATA_CACHE_DIR)
+    if not cache_dir:
+        if env_cache:
+            cache_dir = env_cache
+        else:
+            cache_dir = Path.home() / ".cache" / "apd"
+        logger.debug("Cache directory not set, using %s", cache_dir)
+    samples = None
+    try:
+        lifetime = os.environ.get(APD_METADATA_LIFETIME, APD_METADATA_LIFETIME_DEFAULT)
+        samples, _ = load_ap_info(
+            cache_dir,
+            working_group,
+            analysis,
+            ap_date=ap_date,
+            maxlifetime=lifetime,
+        )
+    except FileNotFoundError:
+        logger.debug(
+            "Caching information for %s/%s to %s for time %s",
+            working_group,
+            analysis,
+            cache_dir,
+            ap_date,
+        )
+        samples = cache_ap_info(
+            cache_dir, working_group, analysis, ap_date=ap_date, api_url=api_url
+        )
+    except InvalidCacheError:
+        logger.debug(
+            "Invalid cache. reloading information for %s/%s to %s for time %s",
+            working_group,
+            analysis,
+            cache_dir,
+            ap_date,
+        )
+        samples = cache_ap_info(
+            cache_dir, working_group, analysis, ap_date=ap_date, api_url=api_url
+        )
+    assert samples is not None
+    return samples
+
+
 def _validate_tags(tags, default_tags=None, available_tags=None):
     """Method that checks the dictionary of tag names, values that should be used
     to filter the data accordingly.
 
-     - Special cases are handled: tags "name" and "version" as well as "data" and "mc"
-        (which are converted to a "config" value).
-     - tag values cannot be None
-     - tag values cannot be of type bytes
-     - int tag values are converted to string
+    Note:
+        - Special cases are handled: tags "name" and "version" as well as "data" and "mc"
+          (which are converted to a "config" value).
+        - Tag values cannot be None.
+        - Tag values cannot be of type bytes.
+        - Int tag values are converted to string.
+
+    Args:
+        tags (dict): the dictionary of tags to be validated.
+        default_tags (dict, optional): provide default tags. Defaults to None.
+        available_tags (list, optional): provide a list of available tags. Defaults to None.
+
+    Raises:
+        ValueError: see the Note above.
+        TypeError: see the Note above.
+
+    Returns:
+        dict: the validated tags.
     """
 
     # Merging the default tags with the ones passed
     effective_tags = tags
     if default_tags:
         for t, v in default_tags.items():
             if t not in effective_tags:
                 effective_tags[t] = v
 
     # Final dict that will be returned
     cleaned = {}
 
-    # name and version are special tags in our case, we check their validity
-    if "name" in effective_tags:
-        raise ValueError("name is not a supported tag in AnalysisData objects")
-
-    version = effective_tags.get("version", None)
-    if version and iterable(version):
-        raise ValueError("version argument doesn't support iterables")
-
     # Special handling for the data and mc tags to avoid having to
     # use the config tag
     # The config tag is set according to the following table:
     #
     # | mc\data |    True    |    False   |      None      |
     # |:-------:|:----------:|:----------:|:--------------:|
     # |   True  | ValueError |     mc     |       mc       |
@@ -108,23 +171,25 @@
         if t in ["data", "mc"]:
             continue
         if v is None:
             raise TypeError(f"{t} value is None")
         if isinstance(v, bytes):
             raise TypeError(f"{t} value is of type {type(v)}")
         if available_tags is not None:
-            check_tag_in_list(t, available_tags)
+            # NB this raises an exception if the tag is not in the list
+            # or if the value does not match any samples
+            check_tag_value_possible(t, v, available_tags)
         if isinstance(v, int) and not isinstance(v, bool):
             cleaned[t] = str(v)
         else:
             cleaned[t] = v
     return cleaned
 
 
-def sample_check(samples, tags):
+def _sample_check(samples, tags):
     """Filter the SampleCollection and check that we have the
     samples that we expect"""
 
     # Fixing the dict to make sure each item is a list
     ltags = {}
     dimensions = tags.keys()
     for tag, value in tags.items():
@@ -154,27 +219,33 @@
     for coordinate, sample_count in hist.items():
         if sample_count != 1:
             logger.debug("Error %d samples for %s", sample_count, {str(coordinate)})
             errors.append((dict(zip(dimensions, coordinate)), sample_count))
     return errors
 
 
+# Map contains AnalysisData objects already loaded
 __analysis_map = {}
 
 
 def get_analysis_data(
     working_group,
     analysis,
     metadata_cache=None,
     data_cache=None,
     api_url="https://lbap.app.cern.ch",
     ap_date=None,
     **kwargs,
 ):
-    """Cache with the same process"""
+    """Main method to get analysis production information.
+
+    Gets the AnalysisData information from the same process if possible.
+    If not loaded already, it loads it from the cache disk and if not present or valid,
+    fetches from the REST API.
+    """
     key = (working_group, analysis, ap_date)
     if key in __analysis_map:
         # As we keep an instance for each WG/Analysis, we need to copy and apply our own defaults
         ad = copy.deepcopy(__analysis_map[key])
         ad.data_cache = data_cache
         ad.default_tags = _validate_tags(kwargs)
         return ad
@@ -219,195 +290,165 @@
     ):
         """
         Constructor that configures the can either fetch the data from the AP service or load from a local cache.
 
         Analysis Production tags can be specified as keyword arguments
         to specify the data to be analyzed.
         """
-        self.working_group = working_group
-        self.analysis = analysis
+        self._working_group = working_group
+        self._analysis = analysis
+
+        #  self._samples is a SampleCollection filled in with the values
+        # Only for internal use as the default filters are NOT applied
+        self._samples = None
 
-        #  self.samples is a SampleCollection filled in with the values
-        metadata_cache = metadata_cache or os.environ.get(APD_METADATA_CACHE_DIR, "")
-        need_clean_fetch = False
+        # Special case when the metadata cache is passed directly as
+        # a SampleCollection
         if metadata_cache:
             if isinstance(metadata_cache, SampleCollection):
                 logger.debug("Using SampleCollection passed to constructor")
-                self.samples = metadata_cache
-            else:
-                logger.debug("Using metadata cache %s", metadata_cache)
-                try:
-                    self.samples, _ = load_ap_info(
-                        metadata_cache, working_group, analysis, ap_date=ap_date
-                    )
-                except FileNotFoundError:
-                    logger.debug(
-                        "Could not find cache in %s, loading from remote",
-                        metadata_cache,
-                    )
-                    need_clean_fetch = True
+                self._samples = metadata_cache
         else:
-            logger.debug(
-                "No cache set, fetching Analysis Production data from %s", api_url
+            # We use the env variable if it is set
+            envcache = os.environ.get(APD_METADATA_CACHE_DIR, None)
+            if envcache:
+                metadata_cache = envcache
+
+        if self._samples is None:
+            # In this case the metadata cache was not a SampleCollection or
+            # not set at all, set setup the cache
+            self._samples = _load_and_setup_cache(
+                metadata_cache, working_group, analysis, ap_date, api_url=api_url
             )
-            need_clean_fetch = True
 
-        if need_clean_fetch:
-            self.samples = fetch_ap_info(
-                working_group, analysis, None, api_url, ap_date=ap_date
-            )
-
-        self.available_tags = self.samples.available_tags()
+        self._available_tags = self._samples.available_tags()
 
-        # Tags is a list of tags that can be used to restrict the samples that will be used
-        self.default_tags = _validate_tags(kwargs, available_tags=self.available_tags)
+        # "available_tags" is a list of tags that can be used to restrict the samples that will be used
+        self._default_tags = _validate_tags(kwargs, available_tags=self._available_tags)
 
         # Now dealing with data cache
         data_cache = data_cache or os.environ.get(APD_DATA_CACHE_DIR, None)
         if isinstance(data_cache, str):
-            self.data_cache = DataCache(data_cache)
+            self._data_cache = DataCache(data_cache)
         else:
-            self.data_cache = data_cache
+            self._data_cache = data_cache
 
     def __call__(
         self,
         *,
-        version=None,
-        name=None,
         return_pfns=True,
         check_data=True,
         use_local_cache=True,
         showmax=10,
         **tags,
     ):
         # pylint: disable-msg=too-many-locals
         """Main method that returns the dataset info.
         The normal behaviour is to return the PFNs for the samples but setting
         return_pfns to false returns the SampleCollection"""
 
-        # Cannot mix data from 2 versions in the same dataset
-        if not version:
-            version = self.default_tags.get("version", None)
-
-        if iterable(version):
-            raise ValueError("version argument doesn't support iterables")
-
         # Establishing the list of samples to run on
-        samples = self.samples
+        samples = self._samples
 
-        if name:
-            if version:
-                # No need to apply other tags, this specifies explicitly a specific dataset
-                # We return it straight away
-                logger.debug("Filtering for version/name %s/%s", name, version)
-                samples = samples.filter("version", version)
-                if len(samples) == 0:
-                    raise KeyError(f"No version {version}")
-                samples = samples.filter("name", name)
-                if len(samples) == 0:
-                    raise KeyError(f"No name {name}")
-            else:
-                # We check whether a version was specified in the default tags
-                samples = samples.filter("name", name)
-                if len(samples) != 1:
-                    raise ValueError(
-                        f"{len(samples)} matching {name}, should be exactly 1"
-                    )
-        else:
-            # Merge the current tags with the default passed to the constructor
-            # and check that they are consistent
-            effective_tags = _validate_tags(
-                tags, self.default_tags, self.available_tags
-            )
-
-            if version:
-                effective_tags["version"] = version
+        # Merge the current tags with the default passed to the constructor
+        # and check that they are consistent
+        effective_tags = _validate_tags(tags, self._default_tags, self._available_tags)
+
+        for tagname, tagvalue in effective_tags.items():
+            logger.debug("Filtering for %s = %s", tagname, tagvalue)
+
+        # Applying the filters in one go
+        samples = samples.filter(**effective_tags)
+        logger.debug("Matched %d samples", len(samples))
+
+        # Filter samples and check that we have what we expect
+        if check_data:
+            errors = _sample_check(samples, effective_tags)
+            if len(errors) > 0:
+                error_txt = f"{len(errors)} problem(s) found\n"
+                for etags, ecount in errors:
+                    if etags:
+                        error_txt += f"{str(etags)}: "
 
-            for tagname, tagvalue in effective_tags.items():
-                logger.debug("Filtering for %s = %s", tagname, tagvalue)
-
-            # Applying the filters in one go
-            samples = samples.filter(**effective_tags)
-            logger.debug("Matched %d samples", len(samples))
-
-            # Filter samples and check that we have what we expect
-            if check_data:
-                errors = sample_check(samples, effective_tags)
-                if len(errors) > 0:
-                    error_txt = f"{len(errors)} problem(s) found\n"
-                    for etags, ecount in errors:
-                        if etags:
-                            error_txt += f"{str(etags)}: "
+                    if ecount > 0:
                         error_txt += f"{ecount} samples for the same configuration found, this is ambiguous:"
-                        if ecount > 0:
-                            error_txt += (
-                                f"(only the first {showmax} samples printed)"
-                                if (ecount > showmax)
-                                else ""
-                            )
-                            match_list = [
-                                str(m)
-                                for m in itertools.islice(
-                                    samples.filter(**etags).itertags(), 0, showmax
-                                )
-                            ]
-                            error_txt += "".join(
-                                ["\n" + " " * 5 + str(m) for m in match_list]
+                        error_txt += (
+                            f"(only the first {showmax} samples printed)"
+                            if (ecount > showmax)
+                            else ""
+                        )
+                        match_list = [
+                            str(m)
+                            for m in itertools.islice(
+                                samples.filter(**etags).itertags(), 0, showmax
                             )
-                    logger.debug("Error loading data: %s", error_txt)
-                    raise ValueError("Error loading data: " + error_txt)
+                        ]
+                        error_txt += "".join(
+                            ["\n" + " " * 5 + str(m) for m in match_list]
+                        )
+                    else:
+                        error_txt += "No matching sample found"
+                logger.debug("Error loading data: %s", error_txt)
+                raise ValueError("Error loading data: " + error_txt)
 
         if return_pfns:
             if use_local_cache:
                 return self._transform_pfns(samples.PFNs())
             return samples.PFNs()
 
         return samples
 
     def _transform_pfns(self, pfns):
         """Method to return PFNs, useful as it can be overriden in inheriting classes"""
-        if not self.data_cache:
+        if not self._data_cache:
             return pfns
-        return [self.data_cache(pfn) for pfn in pfns]
+        return [self._data_cache(pfn) for pfn in pfns]
 
     def __str__(self):
-        txt = f"AnalysisProductions: {self.working_group} / {self.analysis}\n"
-        txt += str(self.samples)
+        """User friendly representation of the AnalysisData instance."""
+        txt = f"AnalysisProductions: {self._working_group} / {self._analysis}\n"
+        txt += str(self._samples)
         return txt
 
     def __repr__(self):
-        return f"<AnalysisData: WG={self.analysis}, analysis={self.working_group}, n_samples={len(self.samples)}>"
+        """String representation of the AnalysisData instance."""
+        return f"<AnalysisData: WG={self._analysis}, analysis={self._working_group}, n_samples={len(self._samples)}>"
 
     def summary(self, tags: list = None) -> dict:
-        """prepares a summary of the Analysis Production info"""
+        """Prepares a summary of the Analysis Production info."""
 
         # Deal with the tags first
         tag_summary = {}
         if tags:
             for tag in tags:
-                if tag in self.available_tags:
+                if tag in self._available_tags:
                     try:
-                        values = sorted(self.available_tags[tag])
+                        values = sorted(self._available_tags[tag])
                     except TypeError as exc:
                         raise ValueError(
                             f"Could not sort the values for tag ({tag}). Please check that the values are sensible.\n"
                         ) from exc
-                    values = list(self.available_tags[tag])
+                    values = list(self._available_tags[tag])
                     tag_summary[tag] = values
                 else:
                     raise ValueError(
-                        f"Requested tag ({tag}) not valid for the given production (wg: {self.working_group}, analysis: {self.analysis})!"
+                        f"Requested tag ({tag}) not valid for the given production (wg: {self._working_group}, analysis: {self._analysis})!"
                     )
         else:
-            tag_summary = dict(self.available_tags)
+            tag_summary = dict(self._available_tags)
 
         summary = {}
         summary["tags"] = tag_summary
 
         # If we specify the tags to be list, we assume the general information should not be printed
         if not tags:
-            summary["analysis"] = self.analysis
-            summary["working_group"] = self.working_group
-            summary["Number_of_files"] = self.samples.file_count()
-            summary["Bytecount"] = self.samples.byte_count()
+            summary["analysis"] = self._analysis
+            summary["working_group"] = self._working_group
+            summary["Number_of_files"] = self._samples.file_count()
+            summary["Bytecount"] = self._samples.byte_count()
 
         return summary
+
+    def all_samples(self):
+        """Returns all the samples in this Analysis Production.
+        i.e. without filtering by the default tags"""
+        return self._samples
```

### Comparing `apd-0.5.0/src/apd/ap_info.py` & `apd-0.6.0/src/apd/ap_info.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,17 +4,21 @@
 # This software is distributed under the terms of the GNU General Public      #
 # Licence version 3 (GPL Version 3), copied verbatim in the file "COPYING".   #
 #                                                                             #
 # In applying this licence, CERN does not waive the privileges and immunities #
 # granted to it by virtue of its status as an Intergovernmental Organization  #
 # or submit itself to any jurisdiction.                                       #
 ###############################################################################
-#
-# Tool to load and interpret information from the AnalysisProductions data endpoint
-#
+"""Internal tools to load and interpret information from the AnalysisProductions data endpoint.
+
+This modules contains the retrieve the data from the AnalysisProductions endpoint
+(with the APDataDownloader class). It returns JSON that can be loaded into a
+SamplesCollection instance.
+
+"""
 import collections.abc
 import difflib
 import itertools
 import json
 import logging
 import math
 import os
@@ -28,44 +32,71 @@
 from .authentication import get_auth_headers
 from .eos import auth
 
 logger = logging.getLogger("apd")
 
 
 def iterable(arg):
-    """Version of Iterable that excludes str"""
+    """Version of Iterable that excludes str."""
     return isinstance(arg, collections.abc.Iterable) and not isinstance(
         arg, (str, bytes)
     )
 
 
 def safe_casefold(a):
-    """casefold that can be called on any type, does nothing on non str"""
+    """Casefold that can be called on any type, does nothing on non str."""
     if isinstance(a, str):
         return a.casefold()
     return a
 
 
-def check_tag_in_list(tag, tag_list):
-    """Check if the tag exists in the list of whether there is one close enough"""
+def check_tag_value_possible(tag, values, available_tags):
+    """Check if the `tag` exists in the in the `available_tags` of similar name,
+    in the sense of `difflib.get_close_matches`. If yes, also check that
+    the value is one of the existing tags values for that tag
+    """
+    tag_list = [t.lower() for t in available_tags.keys()]
+    tag = safe_casefold(tag)
     if tag not in tag_list:
         msg = f"Tag {tag} unknown."
         closest = difflib.get_close_matches(tag, tag_list, n=1)
         if closest:
             msg += f" Did you mean {closest[0]} ?"
         msg += f"\nAvailable tags: {', '.join(tag_list)}"
         raise ValueError(msg)
+    # Now we now the tag exists, checking the value is in the samples
+    # We can have either a value or a list passed, we always
+    # transform to a list to simplify processing
+    if not iterable(values):
+        values = [safe_casefold(str(values))]
+    else:
+        values = [safe_casefold(str(v)) for v in values]
+    for value in values:
+        possible_values = available_tags[tag]
+        if not iterable(possible_values):
+            possible_values = [possible_values]
+        possible_values = [safe_casefold(v) for v in possible_values]
+        if value not in possible_values:
+            msg = f"No sample for tag {tag}={value}"
+            closest = difflib.get_close_matches(value, possible_values, n=1)
+            if closest:
+                msg += f" Did you mean {closest[0]} ?"
+            msg += f"\nAvailable values for {tag}: {', '.join(possible_values)}"
+            raise ValueError(msg)
 
 
 class InvalidCacheError(Exception):
     """Exception to signal that the AP info cache is invalid"""
 
 
 class APDataDownloader:
+    """Utility class that fetches the Analysis Production information."""
+
     def __init__(self, api_url="https://lbap.app.cern.ch"):
+        """Constructor defaulting to the production URL for lbap."""
         self.api_url = api_url
         self.token = None
 
     def _get_kwargs(self):
         return {"timeout": 120, **get_auth_headers()}
 
     def get_ap_info(self, working_group, analysis, ap_date=None):
@@ -127,15 +158,15 @@
             return f
     raise FileNotFoundError(f"{filename} in {mydir}")
 
 
 def _analysis_files(
     cache_dir, working_group, analysis, ap_date, find_case_insensitive=False
 ):
-    """Utils to compose the name of the cache files"""
+    """Utils to compose the name of the cache files."""
     cache_dir = Path(cache_dir)
     cache_dir = (cache_dir / "archives" / ap_date) if ap_date else cache_dir
     wgdir = cache_dir / working_group
     anadir = wgdir / analysis
     datafile = wgdir / f"{analysis}.json"
     tagsfile = anadir / "tags.json"
     cacheinfofile = wgdir / f"{analysis}_cacheinfo.json"
@@ -172,15 +203,15 @@
         current_info[READ] = datetime.now().isoformat()
     temp_path = cacheinfofile.parent / (cacheinfofile.name + secrets.token_urlsafe())
     temp_path.write_text(json.dumps(current_info))
     os.rename(temp_path, cacheinfofile)
     return current_info
 
 
-def get_cache_age(cacheinfo):
+def _get_cache_age(cacheinfo):
     """Return the number of seconds since the cache was last modified"""
     modif_str = cacheinfo.get(MODIFY, None)
     if not modif_str:
         return math.inf
     mtime = datetime.fromisoformat(modif_str)
     delta = datetime.now() - mtime
     return delta.total_seconds()
@@ -190,15 +221,15 @@
     cache_dir,
     working_group,
     analysis,
     loader=None,
     api_url="https://lbap.app.cern.ch",
     ap_date=None,
 ):
-    """Fetch the AP info and cache it locally"""
+    """Fetch the AP info and cache it locally."""
     datafile, tagsfile, cacheinfofile = _analysis_files(
         cache_dir, working_group, analysis, ap_date
     )
     samples = fetch_ap_info(working_group, analysis, loader, api_url, ap_date)
     datafile.write_text(json.dumps(samples.info))
     tagsfile.write_text(json.dumps(samples.tags))
     _update_cache_info(cacheinfofile, True, True)
@@ -210,20 +241,23 @@
     # We want a case insensitive lookup
     datafile, tagsfile, cacheinfofile = _analysis_files(
         cache_dir, working_group, analysis, ap_date, True
     )
     data = json.loads(datafile.read_text())
     tags = json.loads(tagsfile.read_text())
     cacheinfo = _update_cache_info(cacheinfofile, False, True)
-    cache_age = get_cache_age(cacheinfo)
-
+    cache_age = _get_cache_age(cacheinfo)
+    logger.debug("cache_age: %s vs maxlife: %s", cache_age, maxlifetime)
     # If we have specified a maxlifetime, we return an exception
     # if the cache is too old
     if maxlifetime:
-        if cache_age > float(maxlifetime):
+        if float(maxlifetime) >= 0 and cache_age > float(maxlifetime):
+            logger.debug(
+                "cache_too or no caching: %s vs maxlife: %s", cache_age, maxlifetime
+            )
             raise InvalidCacheError(f"Cache too old ({cache_age}s > {maxlifetime}s)")
 
     return SampleCollection(data, tags), cacheinfo
 
 
 def load_ap_info_from_single_file(filename):
     """Load the API info from a cache file (ONLY FOR TESTS)"""
@@ -243,14 +277,15 @@
     """Class wrapping the AnalysisProduction metadata."""
 
     def __init__(self, info=None, tags=None):
         self.info = info if info else []
         self.tags = tags if tags else {}
 
     def __len__(self):
+        """Returns the lenght of the samples list."""
         return len(self.info)
 
     def _sampleTags(self, sample):
         """Method exposing the tags for a given sample/dataset
         We take the dictionary passed in the tag list and add the version and name"""
         sid = str(sample["sample_id"])
         tags = self.tags[sid]
@@ -259,27 +294,30 @@
         # AP is rerun
         tags["version"] = sample["version"]
         tags["name"] = sample["name"]
         tags["state"] = sample["state"]
         return tags
 
     def __repr__(self):
+        """Create a string representation of the samples."""
         return "\n".join(
             [
                 f"{s['name']} {s['version']} files:{len(s['lfns'])} bytes:{s['total_bytes']/(1024*1024*1024):.1f} GiB | "
                 + str(self._sampleTags(s))
                 for s in self.info
             ]
         )
 
     def __iter__(self):
+        """Iterate on the samples in the info member."""
         for s in self.info:
             yield s
 
     def itertags(self):
+        """Iterate on all the tags present in all the samples."""
         for s in self.info:
             yield self._sampleTags(s)
 
     def filter(self, *args, **tags):
         """
         Filter the requests according to the tag value passed in parameter
         """
@@ -288,16 +326,14 @@
         if (len(args) != 0) and len(args) != 2:
             raise ValueError(
                 "filter method takes two positional arguments or keyword arguments"
             )
 
         def _compare_tag(sample, ftag, fvalue):
             """Utility method than handles specific tags, but not iterables"""
-            sampleTags = self._sampleTags(sample)
-            check_tag_in_list(ftag, sampleTags.keys())
             return safe_casefold(self._sampleTags(sample).get(ftag)) == safe_casefold(
                 fvalue
             )
 
         def _filter1(samples, ftag, fvalue):
             logger.debug("filtering samples for %s:%s", ftag, fvalue)
             if callable(fvalue):
@@ -346,14 +382,15 @@
         """Collects total bytecount"""
         count = 0
         for sample in self.info:
             count += len(sample["lfns"].keys())
         return count
 
     def __or__(self, samples):
+        """Logical or between two SampleCollections."""
         info = self.info + samples.info
         tags = {**(self.tags), **(samples.tags)}
         return SampleCollection(info, tags)
 
     def available_tags(self):
         """returns a superset of all tags used in the samples of the collection"""
         available_tags = defaultdict(set)
@@ -374,15 +411,16 @@
             for t in tags:
                 row.append(sample_tags.get(t, None))
             values.append(row)
         return values
 
     def groupby(self, tags=None):
         """Tool that takes the samples and groups them by the tags specified.
-        If no list of tags is specified, then the existing ones are used"""
+        If no list of tags is specified, then the existing ones are used.
+        """
 
         report = self.report()
         header = report[0]
         data = report[1:]
         if not tags:
             tags = list(self.available_tags().keys())
         else:
```

### Comparing `apd-0.5.0/src/apd/authentication.py` & `apd-0.6.0/src/apd/authentication.py`

 * *Files identical despite different names*

### Comparing `apd-0.5.0/src/apd/command.py` & `apd-0.6.0/src/apd/command.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,28 +12,21 @@
 # The command line tools use the click and click-log packages for easier development
 #
 import json
 import logging
 import os
 import sys
 import tempfile
-from pathlib import Path
 
 import click
 import click_log
 import requests
 
-from .analysis_data import (
-    APD_DATA_CACHE_DIR,
-    APD_METADATA_CACHE_DIR,
-    APD_METADATA_LIFETIME,
-    AnalysisData,
-    get_analysis_data,
-)
-from .ap_info import InvalidCacheError, cache_ap_info, load_ap_info
+from .analysis_data import APD_DATA_CACHE_DIR, APD_METADATA_CACHE_DIR, get_analysis_data
+from .ap_info import cache_ap_info
 from .authentication import get_auth_headers, logout
 from .data_cache import DataCache
 from .rich_console import console, error_console
 
 logger = logging.getLogger("apd")
 click_log.basic_config(logger)
 
@@ -69,50 +62,14 @@
     # your format
     error_console.print(f"{exception_type.__name__}: {exception}")
 
 
 sys.excepthook = exception_handler
 
 
-def setup_cache(cache_dir, working_group, analysis, ap_date=None):
-    """Utility function that checks whether the data for the Analysis
-    is cached already and does it if needed."""
-    if not cache_dir:
-        cache_dir = Path.home() / ".cache" / "apd"
-        logger.debug("Cache directory not set, using %s", cache_dir)
-    try:
-        lifetime = os.environ.get(APD_METADATA_LIFETIME, None)
-        load_ap_info(
-            cache_dir,
-            working_group,
-            analysis,
-            ap_date=ap_date,
-            maxlifetime=lifetime,
-        )
-    except FileNotFoundError:
-        logger.debug(
-            "Caching information for %s/%s to %s for time %s",
-            working_group,
-            analysis,
-            cache_dir,
-            ap_date,
-        )
-        cache_ap_info(cache_dir, working_group, analysis, ap_date=ap_date)
-    except InvalidCacheError:
-        logger.debug(
-            "Invalid cache. reloading information for %s/%s to %s for time %s",
-            working_group,
-            analysis,
-            cache_dir,
-            ap_date,
-        )
-        cache_ap_info(cache_dir, working_group, analysis, ap_date=ap_date)
-    return cache_dir
-
-
 def _process_common_tags(eventtype, datatype, polarity, config, name, version):
     """Util to simplify the parsing of common tags"""
     filter_tags = {}
     if name is not None:
         filter_tags["name"] = name
     if version is not None:
         filter_tags["version"] = version
@@ -161,15 +118,15 @@
 @click.argument("analysis")
 @click.option("--date", default=None, help="analysis date in ISO 8601 format")
 @click_log.simple_verbosity_option(logger)
 @common_docstr()
 def cmd_cache_ap_info(cache_dir, working_group, analysis, date):
     """Cache the metadata for analysis production specified."""
     logger.debug(
-        "Caching information for %s/%s to %s for time %s",
+        "Caching %s/%s to %s for time %s",
         working_group,
         analysis,
         cache_dir,
         date,
     )
     cache_ap_info(cache_dir, working_group, analysis, ap_date=date)
 
@@ -219,16 +176,14 @@
     name,
     version,
     date,
 ):
     """List the PFNs for the analysis, matching the tags specified.
     This command checks that the arguments are not ambiguous."""
 
-    cache_dir = setup_cache(cache_dir, working_group, analysis, date)
-
     # Loading the data and filtering/displaying
     datasets = get_analysis_data(
         working_group, analysis, metadata_cache=cache_dir, ap_date=date
     )
     filter_tags = _process_common_tags(
         eventtype, datatype, polarity, config, name, version
     )
@@ -282,17 +237,14 @@
     name,
     version,
     date,
 ):
     """List the samples for the analysis, matching the tags specified.
     This command does not check whether the data set in unambiguous"""
 
-    # Dealing with the cache
-    cache_dir = setup_cache(cache_dir, working_group, analysis, date)
-
     # Loading the data and filtering/displaying
     datasets = get_analysis_data(
         working_group, analysis, metadata_cache=cache_dir, ap_date=date
     )
     filter_tags = filter_tags = _process_common_tags(
         eventtype, datatype, polarity, config, name, version
     )
@@ -319,38 +271,35 @@
     default=None,
     help="Column list (comma separated) by which the dataset should be grouped (or 'all')",
 )
 @click_log.simple_verbosity_option(logger)
 def cmd_dump_info(working_group, analysis, cache_dir, output, groupby):
     """Dump the known information about a specific analysis"""
 
-    # Dealing with the cache
-    setup_cache(cache_dir, working_group, analysis)
-
     # Loading the data first
-    datasets = AnalysisData(working_group, analysis, metadata_cache=cache_dir)
+    datasets = get_analysis_data(working_group, analysis, metadata_cache=cache_dir)
 
     # Checking whether we need to group the data...
     if groupby:
         groupby_tags = [t.strip().lower() for t in groupby.split(",")]
         # Special case where we use all the tags available except name and version
         if "all" in groupby_tags:
             groupby_tags = None
 
-        groups = datasets.samples.groupby(groupby_tags)
+        groups = datasets.all_samples().groupby(groupby_tags)
         if output:
             with open(output, "w") as f:
                 json.dump({str(k): v for k, v in groups.items()}, f)
         else:
             for k, v in groups.items():
                 print(",".join(k))
                 for line in v:
                     print(" " * 8 + str(line))
     else:
-        report = datasets.samples.report()
+        report = datasets.all_samples().report()
         # gets the report as CSV in this case, not JSON
         report_str = "\n".join(([",".join([str(e) for e in line]) for line in report]))
         if output:
             with open(output, "w") as f:
                 f.write(report_str)
         else:
             print(report_str)
@@ -358,15 +307,15 @@
 
 @click.command()
 @click.argument("working_group")
 @click.argument("analysis")
 @click.option(
     "--cache_dir",
     default=os.environ.get(APD_METADATA_CACHE_DIR, None),
-    help="Specify location of the cached analysis data files",
+    help="Specify location of the cached analysis metadata",
 )
 @click.option(
     "--tag",
     default=None,
     help="Tag for which the values should be listed",
     multiple=True,
 )
@@ -377,16 +326,14 @@
     working_group,
     analysis,
     cache_dir,
     tag,
     date,
 ):
     """Print a summary of the information available about the specified analysis."""
-    # Dealing with the cache
-    cache_dir = setup_cache(cache_dir, working_group, analysis, date)
 
     # Loading the dataset and displaying its summary
     datasets = get_analysis_data(
         working_group, analysis, metadata_cache=cache_dir, ap_date=date
     )
     datasets = get_analysis_data(
         working_group, analysis, metadata_cache=cache_dir, ap_date=date
@@ -404,15 +351,15 @@
     "--cache_dir",
     default=os.environ.get("APD_METADATA_CACHE_DIR", None),
     help="Specify location of the cache for the analysis metadata",
 )
 @click.option(
     "--data_cache_dir",
     default=os.environ.get(APD_DATA_CACHE_DIR, None),
-    help="Specify location of the cache for the analysis metadata",
+    help="Specify location where a copy of the files will be kept",
 )
 @click.option(
     "-n",
     "--dry-run",
     type=bool,
     default=False,
     is_flag=True,
@@ -457,15 +404,14 @@
     name,
     version,
     date,
 ):
     """Cache the files for the analysis locally, matching the tags specified.
     This command checks that the arguments are not ambiguous."""
     # pylint: disable-msg=too-many-locals
-    cache_dir = setup_cache(cache_dir, working_group, analysis, date)
 
     if not data_cache_dir:
         raise ValueError("Please specify the location of the data cache")
     data_cache = DataCache(data_cache_dir)
     # Loading the data and filtering/displaying
     datasets = get_analysis_data(
         working_group, analysis, metadata_cache=cache_dir, ap_date=date
```

### Comparing `apd-0.5.0/src/apd/data_cache.py` & `apd-0.6.0/src/apd/data_cache.py`

 * *Files 9% similar despite different names*

```diff
@@ -49,9 +49,9 @@
             return remote
         return str(local) if local.exists() else remote
 
     def copy_locally(self, remote):
         local = self.remote_to_local(remote)
         local.parent.mkdir(parents=True, exist_ok=True)
         cmd = ["xrdcp", "--silent", str(remote), str(local)]
-        result = subprocess.run(cmd, check=True, timeout=1000)
+        result = subprocess.run(cmd, check=True)
         return result
```

### Comparing `apd-0.5.0/src/apd/eos.py` & `apd-0.6.0/src/apd/eos.py`

 * *Files identical despite different names*

### Comparing `apd-0.5.0/src/apd/rich_console.py` & `apd-0.6.0/src/apd/rich_console.py`

 * *Files identical despite different names*

### Comparing `apd-0.5.0/src/apd/snakemake.py` & `apd-0.6.0/src/apd/snakemake.py`

 * *Files identical despite different names*

### Comparing `apd-0.5.0/src/apd.egg-info/SOURCES.txt` & `apd-0.6.0/src/apd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apd-0.5.0/tests/cache-dir/b2oc/b02dkpi/tags.json` & `apd-0.6.0/tests/cache-dir/b2oc/b02dkpi/tags.json`

 * *Files identical despite different names*

### Comparing `apd-0.5.0/tests/cache-dir/b2oc/b02dkpi.json` & `apd-0.6.0/tests/cache-dir/b2oc/b02dkpi.json`

 * *Files identical despite different names*

### Comparing `apd-0.5.0/tests/conftest.py` & `apd-0.6.0/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import json
 import os
 from pathlib import Path
 
 import pytest
 import responses
 
-from apd.analysis_data import APD_METADATA_CACHE_DIR
+from apd.analysis_data import APD_METADATA_CACHE_DIR, APD_METADATA_LIFETIME
 from apd.ap_info import cache_ap_info, load_ap_info_from_single_file
 
 DATA_DIR = Path(__file__).parent / "data"
 APINFO_PATHS = DATA_DIR / "rds_ap_info.json"
 APINFO_MULTIPLEVERSIONS_PATHS = DATA_DIR / "rds_ap_info_2versions.json"
 
 
@@ -92,8 +92,9 @@
     os.makedirs(cachedir)
     yield cachedir
 
 
 @pytest.fixture
 def apd_cache(monkeypatch):
     monkeypatch.setenv(APD_METADATA_CACHE_DIR, str(Path(__file__).parent / "cache-dir"))
+    monkeypatch.setenv(APD_METADATA_LIFETIME, "-1")
     yield
```

### Comparing `apd-0.5.0/tests/data/rds_ap_info.json` & `apd-0.6.0/tests/data/rds_ap_info.json`

 * *Files identical despite different names*

### Comparing `apd-0.5.0/tests/data/rds_ap_info_2versions.json` & `apd-0.6.0/tests/data/rds_ap_info_2versions.json`

 * *Files identical despite different names*

### Comparing `apd-0.5.0/tests/test_analysis_data.py` & `apd-0.6.0/tests/test_analysis_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 ###############################################################################
-# (c) Copyright 2021 CERN for the benefit of the LHCb Collaboration           #
+# (c) Copyright 2021-2023 CERN for the benefit of the LHCb Collaboration      #
 #                                                                             #
 # This software is distributed under the terms of the GNU General Public      #
 # Licence version 3 (GPL Version 3), copied verbatim in the file "COPYING".   #
 #                                                                             #
 # In applying this licence, CERN does not waive the privileges and immunities #
 # granted to it by virtue of its status as an Intergovernmental Organization  #
 # or submit itself to any jurisdiction.                                       #
 ###############################################################################
+import logging
+
 import pytest
 
 from apd import AnalysisData
-from apd.analysis_data import APD_METADATA_CACHE_DIR, sample_check
+from apd.analysis_data import (
+    APD_METADATA_CACHE_DIR,
+    APD_METADATA_LIFETIME,
+    _sample_check,
+)
 
 
 def test_fromcache(apinfo_cache):
     datasets = AnalysisData("SL", "RDs", metadata_cache=apinfo_cache)
     assert len(datasets(datatype="2012", polarity=["magup", "magdown"])) == 11
     assert len(datasets(datatype=["2012", "2016"], polarity=["magup", "magdown"])) == 25
     assert len(datasets(datatype=["2012", "2016"], polarity="magdown")) == 12
 
 
 def test_fromendpoint(monkeypatch, mocked_responses):
+    logger = logging.getLogger("apd")
+    logger.setLevel(logging.DEBUG)
     monkeypatch.setenv(APD_METADATA_CACHE_DIR, "")
+    monkeypatch.setenv(APD_METADATA_LIFETIME, "0")
     datasets = AnalysisData("SL", "RDs")
     assert len(datasets(datatype="2012", polarity=["magup", "magdown"])) == 11
     assert len(datasets(datatype=["2012", "2016"], polarity=["magup", "magdown"])) == 25
     assert len(datasets(datatype=["2012", "2016"], polarity="magdown")) == 12
 
 
 def test_withversionandname(apinfo_cache):
@@ -49,28 +58,28 @@
 def test_sample_check_badinput(apinfo_multipleversions):
     tags = {"datatype": ["2012", "2016"], "polarity": "magdown"}
     samples = apinfo_multipleversions
     with pytest.raises(
         KeyError,
         match="Encountered sample with tags.*which does not match filtering criteria",
     ):
-        sample_check(samples, tags)
+        _sample_check(samples, tags)
 
 
 def test_sample_check(apinfo_multipleversions):
     tags = {"datatype": ["2012", "2016"], "polarity": "magdown"}
     samples = apinfo_multipleversions.filter(**tags)
-    errors = sample_check(samples, tags)
+    errors = _sample_check(samples, tags)
     assert len(errors) == 0
 
 
 def test_sample_check_error(apinfo_multipleversions):
     tags = {"datatype": ["2012", "2018"], "polarity": "magup"}
     samples = apinfo_multipleversions.filter(**tags)
-    errors = sample_check(samples, tags)
+    errors = _sample_check(samples, tags)
     assert len(errors) == 1
 
 
 def test_sample_check_load_dataset_error(apinfo_multipleversions):
     with pytest.raises(ValueError):
         datasets = AnalysisData(
             "SL",
@@ -96,7 +105,14 @@
         datasets(badtag="novalue")
 
 
 def test_badtag_constructor(apinfo_cache):
     """In case we specify a tag that does not exist an exception should be thrown"""
     with pytest.raises(ValueError):
         AnalysisData("SL", "RDs", metadata_cache=apinfo_cache, badtag="novalue")
+
+
+def test_badtagvalue_constructor(apinfo_cache):
+    """In case we specify a tag with a value which does not exist, we should raise
+    and exception in that case"""
+    with pytest.raises(ValueError):
+        AnalysisData("SL", "RDs", metadata_cache=apinfo_cache, datatype="2032")
```

### Comparing `apd-0.5.0/tests/test_ap_info.py` & `apd-0.6.0/tests/test_ap_info.py`

 * *Files identical despite different names*

### Comparing `apd-0.5.0/tests/test_b2oc.py` & `apd-0.6.0/tests/test_b2oc.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,20 +22,14 @@
 
     pfns = datasets(version="v0r0p2518507", name="2018_15164022_magup")
     assert len(pfns) == 6
 
     pfns = datasets(version="v0r0p2970193", name="2018_15164022_magup")
     assert len(pfns) == 1 and "00145075_00000001" in pfns[0]
 
-    with pytest.raises(ValueError, match="version argument doesn't support iterables"):
-        datasets(version=["v0r0p2518507", "v0r0p2970193"], name="2018_15164022_magup")
-
-    with pytest.raises(ValueError, match="version argument doesn't support iterables"):
-        datasets(version={"v0r0p2518507", "v0r0p2970193"}, name="2018_15164022_magup")
-
     pfns = set(
         datasets(
             version="v0r0p2970193",
             name=["2018_15164022_magup", "2018_15164022_magdown"],
         )
     )
 
@@ -54,42 +48,14 @@
         datasets(
             version="v0r0p2970193",
             name={"2018_15164022_magup", "2018_15164022_magdown"},
         )
     )
 
 
-def test_defaults_version(apd_cache):
-    datasets = AnalysisData("b2oc", "b02dkpi", version="v0r0p2518507")
-    pfns = datasets(name="2018_15164022_magup")
-    assert len(pfns) == 6
-
-    datasets = AnalysisData("b2oc", "b02dkpi", version="v0r0p2970193")
-    pfns = datasets(name="2018_15164022_magup")
-    assert len(pfns) == 1 and "00145075_00000001" in pfns[0]
-
-    with pytest.raises(ValueError, match="version argument doesn't support iterables"):
-        AnalysisData("b2oc", "b02dkpi", version=["v0r0p2518507", "v0r0p2970193"])
-    with pytest.raises(ValueError, match="version argument doesn't support iterables"):
-        AnalysisData("b2oc", "b02dkpi", version={"v0r0p2518507", "v0r0p2970193"})
-
-
-def test_defaults_name(apd_cache):
-    with pytest.raises(
-        ValueError, match="name is not a supported tag in AnalysisData objects"
-    ):
-        AnalysisData(
-            "b2oc", "b02dkpi", version="v0r0p2518507", name="2018_15164022_magup"
-        )
-    with pytest.raises(
-        ValueError, match="name is not a supported tag in AnalysisData objects"
-    ):
-        AnalysisData("b2oc", "b02dkpi", name="2018_15164022_magup")
-
-
 def test_defaults_tag_override(apd_cache):
     datasets = AnalysisData(
         "b2oc", "b02dkpi", datatype=2018, polarity=["magup", "magdown"]
     )
 
     pfns = datasets(datatype="2011", eventtype="11164047", polarity="magdown")
     assert len(pfns) == 5 and all("00128098_0000" in x for x in pfns)
@@ -167,17 +133,15 @@
     )
 
     with pytest.raises(
         ValueError, match=r"Error loading data: 4 problem\(s\) found"
     ):  # TODO: This should be more specific
         datasets(datatype=["2012", "2011"], polarity=["magup", "magdown"])
 
-    with pytest.raises(
-        ValueError, match=r"Error loading data: 2 problem\(s\) found"
-    ):  # TODO: This should be more specific
+    with pytest.raises(ValueError, match=r"No sample for tag polarity=magoff.*"):
         datasets(datatype=["2015", "2016"], polarity=["magoff"])
 
     pfns = datasets(datatype=["2015", "2016"], polarity=["magup", "magdown"], mc=False)
     assert len(pfns) == 519 and all(
         any(
             y in x for y in ["00121802_00", "00121816_00", "00121814_00", "00121794_00"]
         )
@@ -202,39 +166,35 @@
             datatype=["2015", "2016"],
             polarity=["magup", "magdown"],
             data=False,
             mc=False,
         )
 
 
-def test_missing_by_name(apd_cache):
-    datasets = AnalysisData("b2oc", "b02dkpi")
-    with pytest.raises(KeyError):
-        datasets(version="i-do-no-exist", name="2018_15164022_magup")
-    with pytest.raises(KeyError):
-        datasets(version="v0r0p2970193", name="i-do-not-exist")
-
-
-def test_missing_by_tags(apd_cache):
-    datasets = AnalysisData("b2oc", "b02dkpi")
-    with pytest.raises(KeyError):
-        datasets(version="i-do-no-exist", name="2018_15164022_magup")
-    with pytest.raises(KeyError):
-        datasets(version="v0r0p2970193", name="i-do-not-exist")
-
-
 def test_analysis_case_sensitivity(apd_cache):
     datasets = AnalysisData("b2oc", "b02dkpi")
-    assert len(datasets.samples) == 1694
-    assert len(AnalysisData("B2OC", "B02DKPI").samples) == 1694
+    assert len(datasets._samples) == 1694
+    assert len(AnalysisData("B2OC", "B02DKPI")._samples) == 1694
 
     pfns = datasets(version="v0r0p2970193", name="2018_15164022_magup")
     assert len(pfns) == 1 and "00145075_00000001" in pfns[0]
 
     pfns = datasets(version="V0R0P2970193", name="2018_15164022_MAGUP")
     assert len(pfns) == 1 and "00145075_00000001" in pfns[0]
 
 
 def test_name_case_sensitivity(apd_cache):
     datasets = AnalysisData("b2oc", "b02dkpi")
     pfns = datasets(version="v0r0p2970193", name="2018_15164022_MAGUP")
     assert len(pfns) == 1 and "00145075_00000001" in pfns[0]
+
+
+def test_unknown_tag_value(apd_cache):
+    datasets = AnalysisData("b2oc", "b02dkpi")
+
+    with pytest.raises(ValueError, match="No sample for tag datatype=2032.*"):
+        datasets(
+            datatype=["2032"],
+            polarity=["magup", "magdown"],
+            eventtype="11164047",
+            mc=True,
+        )
```

### Comparing `apd-0.5.0/tests/test_data_cache.py` & `apd-0.6.0/tests/test_data_cache.py`

 * *Files identical despite different names*

