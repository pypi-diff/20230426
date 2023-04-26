# Comparing `tmp/dogpile.cache-1.1.8.tar.gz` & `tmp/dogpile.cache-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dogpile.cache-1.1.8.tar", last modified: Fri Jul  8 17:57:28 2022, max compression
+gzip compressed data, was "dogpile.cache-1.2.0.tar", last modified: Wed Apr 26 15:47:54 2023, max compression
```

## Comparing `dogpile.cache-1.1.8.tar` & `dogpile.cache-1.2.0.tar`

### file list

```diff
@@ -1,135 +1,131 @@
-drwxrwxr-x   0 classic   (1000) classic   (1000)        0 2022-07-08 17:57:28.758220 dogpile.cache-1.1.8/
--rw-rw-r--   0 classic   (1000) classic   (1000)     1059 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/LICENSE
--rw-rw-r--   0 classic   (1000) classic   (1000)      343 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/MANIFEST.in
--rw-rw-r--   0 classic   (1000) classic   (1000)     4915 2022-07-08 17:57:28.758220 dogpile.cache-1.1.8/PKG-INFO
--rw-rw-r--   0 classic   (1000) classic   (1000)     4176 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/README.rst
-drwxrwxr-x   0 classic   (1000) classic   (1000)        0 2022-07-08 17:57:28.751220 dogpile.cache-1.1.8/docs/
-drwxrwxr-x   0 classic   (1000) classic   (1000)        0 2022-07-08 17:57:28.752220 dogpile.cache-1.1.8/docs/_sources/
--rw-rw-r--   0 classic   (1000) classic   (1000)     1587 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/docs/_sources/api.rst.txt
--rw-rw-r--   0 classic   (1000) classic   (1000)    38753 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/docs/_sources/changelog.rst.txt
--rw-rw-r--   0 classic   (1000) classic   (1000)    10222 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/docs/_sources/core_usage.rst.txt
--rw-rw-r--   0 classic   (1000) classic   (1000)      769 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/docs/_sources/front.rst.txt
--rw-rw-r--   0 classic   (1000) classic   (1000)     1215 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/docs/_sources/index.rst.txt
--rw-rw-r--   0 classic   (1000) classic   (1000)     9296 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/docs/_sources/recipes.rst.txt
--rw-rw-r--   0 classic   (1000) classic   (1000)    11625 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/docs/_sources/usage.rst.txt
-drwxrwxr-x   0 classic   (1000) classic   (1000)        0 2022-07-08 17:57:28.754220 dogpile.cache-1.1.8/docs/_static/
--rw-rw-r--   0 classic   (1000) classic   (1000)     4418 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/docs/_static/_sphinx_javascript_frameworks_compat.js
--rw-rw-r--   0 classic   (1000) classic   (1000)    15205 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/docs/_static/basic.css
--rw-rw-r--   0 classic   (1000) classic   (1000)      107 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/docs/_static/changelog.css
--rw-rw-r--   0 classic   (1000) classic   (1000)     8171 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/docs/_static/doctools.js
--rw-rw-r--   0 classic   (1000) classic   (1000)      421 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/docs/_static/documentation_options.js
--rw-rw-r--   0 classic   (1000) classic   (1000)      286 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/docs/_static/file.png
--rw-rw-r--   0 classic   (1000) classic   (1000)   288580 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/docs/_static/jquery-3.6.0.js
--rw-rw-r--   0 classic   (1000) classic   (1000)    89501 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/docs/_static/jquery.js
--rw-rw-r--   0 classic   (1000) classic   (1000)     4758 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/docs/_static/language_data.js
--rw-rw-r--   0 classic   (1000) classic   (1000)       90 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/docs/_static/minus.png
--rw-rw-r--   0 classic   (1000) classic   (1000)     4180 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/docs/_static/nature.css
--rw-rw-r--   0 classic   (1000) classic   (1000)      343 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/docs/_static/nature_override.css
--rw-rw-r--   0 classic   (1000) classic   (1000)       90 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/docs/_static/plus.png
--rw-rw-r--   0 classic   (1000) classic   (1000)     4846 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/docs/_static/pygments.css
--rw-rw-r--   0 classic   (1000) classic   (1000)    17088 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/docs/_static/searchtools.js
--rw-rw-r--   0 classic   (1000) classic   (1000)        0 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/docs/_static/site_custom_css.css
--rw-rw-r--   0 classic   (1000) classic   (1000)      204 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/docs/_static/sphinx_paramlinks.css
--rw-rw-r--   0 classic   (1000) classic   (1000)    68420 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/docs/_static/underscore-1.13.1.js
--rw-rw-r--   0 classic   (1000) classic   (1000)    19530 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/docs/_static/underscore.js
--rw-rw-r--   0 classic   (1000) classic   (1000)   443085 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/docs/api.html
-drwxrwxr-x   0 classic   (1000) classic   (1000)        0 2022-07-08 17:57:28.755220 dogpile.cache-1.1.8/docs/build/
--rw-rw-r--   0 classic   (1000) classic   (1000)     3373 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/docs/build/Makefile
-drwxrwxr-x   0 classic   (1000) classic   (1000)        0 2022-07-08 17:57:28.755220 dogpile.cache-1.1.8/docs/build/_static/
--rw-rw-r--   0 classic   (1000) classic   (1000)      343 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/docs/build/_static/nature_override.css
--rw-rw-r--   0 classic   (1000) classic   (1000)        0 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/docs/build/_static/site_custom_css.css
-drwxrwxr-x   0 classic   (1000) classic   (1000)        0 2022-07-08 17:57:28.755220 dogpile.cache-1.1.8/docs/build/_templates/
--rw-rw-r--   0 classic   (1000) classic   (1000)        0 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/docs/build/_templates/site_custom_sidebars.html
--rw-rw-r--   0 classic   (1000) classic   (1000)     1587 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/docs/build/api.rst
--rw-rw-r--   0 classic   (1000) classic   (1000)      266 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/docs/build/builder.py
--rw-------   0 classic   (1000) classic   (1000)    38753 2022-07-08 17:57:24.000000 dogpile.cache-1.1.8/docs/build/changelog.rst
--rw-rw-r--   0 classic   (1000) classic   (1000)     7408 2022-07-08 17:57:24.000000 dogpile.cache-1.1.8/docs/build/conf.py
--rw-rw-r--   0 classic   (1000) classic   (1000)    10222 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/docs/build/core_usage.rst
--rw-rw-r--   0 classic   (1000) classic   (1000)      769 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/docs/build/front.rst
--rw-rw-r--   0 classic   (1000) classic   (1000)     1215 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/docs/build/index.rst
--rw-rw-r--   0 classic   (1000) classic   (1000)     9296 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/docs/build/recipes.rst
--rw-rw-r--   0 classic   (1000) classic   (1000)      178 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/docs/build/requirements.txt
-drwxrwxr-x   0 classic   (1000) classic   (1000)        0 2022-07-08 17:57:28.755220 dogpile.cache-1.1.8/docs/build/unreleased/
--rw-rw-r--   0 classic   (1000) classic   (1000)      410 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/docs/build/unreleased/README.txt
--rw-rw-r--   0 classic   (1000) classic   (1000)    11625 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/docs/build/usage.rst
--rw-rw-r--   0 classic   (1000) classic   (1000)   131016 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/docs/changelog.html
--rw-rw-r--   0 classic   (1000) classic   (1000)    28546 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/docs/core_usage.html
--rw-rw-r--   0 classic   (1000) classic   (1000)     6610 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/docs/front.html
--rw-rw-r--   0 classic   (1000) classic   (1000)    67485 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/docs/genindex.html
--rw-rw-r--   0 classic   (1000) classic   (1000)    14915 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/docs/index.html
--rw-rw-r--   0 classic   (1000) classic   (1000)     6074 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/docs/py-modindex.html
--rw-rw-r--   0 classic   (1000) classic   (1000)    32494 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/docs/recipes.html
--rw-rw-r--   0 classic   (1000) classic   (1000)     3625 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/docs/search.html
--rw-rw-r--   0 classic   (1000) classic   (1000)    47480 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/docs/searchindex.js
--rw-rw-r--   0 classic   (1000) classic   (1000)   110635 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/docs/usage.html
-drwxrwxr-x   0 classic   (1000) classic   (1000)        0 2022-07-08 17:57:28.747220 dogpile.cache-1.1.8/dogpile/
--rw-rw-r--   0 classic   (1000) classic   (1000)      106 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/dogpile/__init__.py
-drwxrwxr-x   0 classic   (1000) classic   (1000)        0 2022-07-08 17:57:28.748220 dogpile.cache-1.1.8/dogpile/cache/
--rw-rw-r--   0 classic   (1000) classic   (1000)      180 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/dogpile/cache/__init__.py
--rw-rw-r--   0 classic   (1000) classic   (1000)    16696 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/dogpile/cache/api.py
-drwxrwxr-x   0 classic   (1000) classic   (1000)        0 2022-07-08 17:57:28.749220 dogpile.cache-1.1.8/dogpile/cache/backends/
--rw-rw-r--   0 classic   (1000) classic   (1000)     1197 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/dogpile/cache/backends/__init__.py
--rw-rw-r--   0 classic   (1000) classic   (1000)    13749 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/dogpile/cache/backends/file.py
--rw-rw-r--   0 classic   (1000) classic   (1000)    20835 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/dogpile/cache/backends/memcached.py
--rw-rw-r--   0 classic   (1000) classic   (1000)     3030 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/dogpile/cache/backends/memory.py
--rw-rw-r--   0 classic   (1000) classic   (1000)     1167 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/dogpile/cache/backends/null.py
--rw-rw-r--   0 classic   (1000) classic   (1000)    11764 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/dogpile/cache/backends/redis.py
--rw-rw-r--   0 classic   (1000) classic   (1000)      601 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/dogpile/cache/exception.py
-drwxrwxr-x   0 classic   (1000) classic   (1000)        0 2022-07-08 17:57:28.749220 dogpile.cache-1.1.8/dogpile/cache/plugins/
--rw-rw-r--   0 classic   (1000) classic   (1000)        0 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/dogpile/cache/plugins/__init__.py
--rw-rw-r--   0 classic   (1000) classic   (1000)     2964 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/dogpile/cache/plugins/mako_cache.py
--rw-rw-r--   0 classic   (1000) classic   (1000)     3610 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/dogpile/cache/proxy.py
--rw-rw-r--   0 classic   (1000) classic   (1000)    67760 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/dogpile/cache/region.py
--rw-rw-r--   0 classic   (1000) classic   (1000)     5418 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/dogpile/cache/util.py
--rw-rw-r--   0 classic   (1000) classic   (1000)      565 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/dogpile/core.py
--rw-rw-r--   0 classic   (1000) classic   (1000)     7077 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/dogpile/lock.py
-drwxrwxr-x   0 classic   (1000) classic   (1000)        0 2022-07-08 17:57:28.749220 dogpile.cache-1.1.8/dogpile/util/
--rw-rw-r--   0 classic   (1000) classic   (1000)      339 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/dogpile/util/__init__.py
--rw-rw-r--   0 classic   (1000) classic   (1000)     1735 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/dogpile/util/compat.py
--rw-rw-r--   0 classic   (1000) classic   (1000)     4479 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/dogpile/util/langhelpers.py
--rw-rw-r--   0 classic   (1000) classic   (1000)     2801 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/dogpile/util/nameregistry.py
--rw-rw-r--   0 classic   (1000) classic   (1000)     4532 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/dogpile/util/readwrite_lock.py
-drwxrwxr-x   0 classic   (1000) classic   (1000)        0 2022-07-08 17:57:28.756220 dogpile.cache-1.1.8/dogpile.cache.egg-info/
--rw-rw-r--   0 classic   (1000) classic   (1000)     4915 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/dogpile.cache.egg-info/PKG-INFO
--rw-rw-r--   0 classic   (1000) classic   (1000)     3066 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/dogpile.cache.egg-info/SOURCES.txt
--rw-rw-r--   0 classic   (1000) classic   (1000)        1 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/dogpile.cache.egg-info/dependency_links.txt
--rw-rw-r--   0 classic   (1000) classic   (1000)       74 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/dogpile.cache.egg-info/entry_points.txt
--rw-rw-r--   0 classic   (1000) classic   (1000)        1 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/dogpile.cache.egg-info/not-zip-safe
--rw-rw-r--   0 classic   (1000) classic   (1000)       34 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/dogpile.cache.egg-info/requires.txt
--rw-rw-r--   0 classic   (1000) classic   (1000)        8 2022-07-08 17:57:28.000000 dogpile.cache-1.1.8/dogpile.cache.egg-info/top_level.txt
--rw-rw-r--   0 classic   (1000) classic   (1000)      838 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/hash_port.py
--rw-rw-r--   0 classic   (1000) classic   (1000)      513 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/log_tests.ini
--rw-rw-r--   0 classic   (1000) classic   (1000)     1595 2022-07-08 17:57:28.759220 dogpile.cache-1.1.8/setup.cfg
--rw-rw-r--   0 classic   (1000) classic   (1000)      558 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/setup.py
-drwxrwxr-x   0 classic   (1000) classic   (1000)        0 2022-07-08 17:57:28.756220 dogpile.cache-1.1.8/tests/
--rw-rw-r--   0 classic   (1000) classic   (1000)        0 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/tests/__init__.py
-drwxrwxr-x   0 classic   (1000) classic   (1000)        0 2022-07-08 17:57:28.757220 dogpile.cache-1.1.8/tests/cache/
--rw-rw-r--   0 classic   (1000) classic   (1000)      870 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/tests/cache/__init__.py
--rw-rw-r--   0 classic   (1000) classic   (1000)    16355 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/tests/cache/_fixtures.py
-drwxrwxr-x   0 classic   (1000) classic   (1000)        0 2022-07-08 17:57:28.757220 dogpile.cache-1.1.8/tests/cache/plugins/
--rw-rw-r--   0 classic   (1000) classic   (1000)        0 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/tests/cache/plugins/__init__.py
--rw-rw-r--   0 classic   (1000) classic   (1000)     1389 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/tests/cache/plugins/test_mako_cache.py
--rw-rw-r--   0 classic   (1000) classic   (1000)     2972 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/tests/cache/test_dbm_backend.py
--rw-rw-r--   0 classic   (1000) classic   (1000)    18860 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/tests/cache/test_decorator.py
--rw-rw-r--   0 classic   (1000) classic   (1000)      405 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/tests/cache/test_mako.py
--rw-rw-r--   0 classic   (1000) classic   (1000)    16050 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/tests/cache/test_memcached_backend.py
--rw-rw-r--   0 classic   (1000) classic   (1000)      361 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/tests/cache/test_memory_backend.py
--rw-rw-r--   0 classic   (1000) classic   (1000)     1934 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/tests/cache/test_null_backend.py
--rw-rw-r--   0 classic   (1000) classic   (1000)     6693 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/tests/cache/test_redis_backend.py
--rw-rw-r--   0 classic   (1000) classic   (1000)     3468 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/tests/cache/test_redis_sentinel_backend.py
--rw-rw-r--   0 classic   (1000) classic   (1000)    32235 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/tests/cache/test_region.py
--rw-rw-r--   0 classic   (1000) classic   (1000)      769 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/tests/conftest.py
--rw-rw-r--   0 classic   (1000) classic   (1000)      552 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/tests/test_backgrounding.py
--rw-rw-r--   0 classic   (1000) classic   (1000)    10397 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/tests/test_lock.py
--rw-rw-r--   0 classic   (1000) classic   (1000)      893 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/tests/test_utils.py
-drwxrwxr-x   0 classic   (1000) classic   (1000)        0 2022-07-08 17:57:28.758220 dogpile.cache-1.1.8/tests/tls/
--rw-rw-r--   0 classic   (1000) classic   (1000)     2354 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/tests/tls/ca-root.crt
--rw-rw-r--   0 classic   (1000) classic   (1000)     2354 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/tests/tls/client-ca-root.crt
--rw-rw-r--   0 classic   (1000) classic   (1000)     1692 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/tests/tls/client.crt
--rw-rw-r--   0 classic   (1000) classic   (1000)     1679 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/tests/tls/client.key
--rw-rw-r--   0 classic   (1000) classic   (1000)     1675 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/tests/tls/server.key
--rw-rw-r--   0 classic   (1000) classic   (1000)     4021 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/tests/tls/server_chain.pem
-drwxrwxr-x   0 classic   (1000) classic   (1000)        0 2022-07-08 17:57:28.758220 dogpile.cache-1.1.8/tests/util/
--rw-rw-r--   0 classic   (1000) classic   (1000)        0 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/tests/util/__init__.py
--rw-rw-r--   0 classic   (1000) classic   (1000)     1535 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/tests/util/test_nameregistry.py
--rw-rw-r--   0 classic   (1000) classic   (1000)     2401 2022-07-08 17:57:15.000000 dogpile.cache-1.1.8/tox.ini
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:54.441534 dogpile.cache-1.2.0/
+-rw-r--r--   0 classic   (1000) classic   (1000)     1059 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/LICENSE
+-rw-r--r--   0 classic   (1000) classic   (1000)      343 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/MANIFEST.in
+-rw-r--r--   0 classic   (1000) classic   (1000)     4895 2023-04-26 15:47:54.441534 dogpile.cache-1.2.0/PKG-INFO
+-rw-r--r--   0 classic   (1000) classic   (1000)     4176 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/README.rst
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:54.428534 dogpile.cache-1.2.0/docs/
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:54.430534 dogpile.cache-1.2.0/docs/_sources/
+-rw-r--r--   0 classic   (1000) classic   (1000)     1587 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_sources/api.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)    39402 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_sources/changelog.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)    10222 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_sources/core_usage.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)      769 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_sources/front.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)     1215 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_sources/index.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)     9296 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_sources/recipes.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)    11625 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_sources/usage.rst.txt
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:54.433534 dogpile.cache-1.2.0/docs/_static/
+-rw-r--r--   0 classic   (1000) classic   (1000)    14813 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_static/basic.css
+-rw-r--r--   0 classic   (1000) classic   (1000)      107 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_static/changelog.css
+-rw-r--r--   0 classic   (1000) classic   (1000)     4472 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_static/doctools.js
+-rw-r--r--   0 classic   (1000) classic   (1000)      420 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_static/documentation_options.js
+-rw-r--r--   0 classic   (1000) classic   (1000)      286 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_static/file.png
+-rw-r--r--   0 classic   (1000) classic   (1000)     4758 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_static/language_data.js
+-rw-r--r--   0 classic   (1000) classic   (1000)       90 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_static/minus.png
+-rw-r--r--   0 classic   (1000) classic   (1000)     4208 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_static/nature.css
+-rw-r--r--   0 classic   (1000) classic   (1000)      343 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_static/nature_override.css
+-rw-r--r--   0 classic   (1000) classic   (1000)       90 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_static/plus.png
+-rw-r--r--   0 classic   (1000) classic   (1000)     4846 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_static/pygments.css
+-rw-r--r--   0 classic   (1000) classic   (1000)    18215 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_static/searchtools.js
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_static/site_custom_css.css
+-rw-r--r--   0 classic   (1000) classic   (1000)     4712 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_static/sphinx_highlight.js
+-rw-r--r--   0 classic   (1000) classic   (1000)      204 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/_static/sphinx_paramlinks.css
+-rw-r--r--   0 classic   (1000) classic   (1000)   480795 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/api.html
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:54.435534 dogpile.cache-1.2.0/docs/build/
+-rw-r--r--   0 classic   (1000) classic   (1000)     3373 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/docs/build/Makefile
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:54.435534 dogpile.cache-1.2.0/docs/build/_static/
+-rw-r--r--   0 classic   (1000) classic   (1000)      343 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/docs/build/_static/nature_override.css
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/docs/build/_static/site_custom_css.css
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:54.435534 dogpile.cache-1.2.0/docs/build/_templates/
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/docs/build/_templates/site_custom_sidebars.html
+-rw-r--r--   0 classic   (1000) classic   (1000)     1587 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/docs/build/api.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)      266 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/docs/build/builder.py
+-rw-------   0 classic   (1000) classic   (1000)    39402 2023-04-26 15:47:49.000000 dogpile.cache-1.2.0/docs/build/changelog.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)     7408 2023-04-26 15:47:49.000000 dogpile.cache-1.2.0/docs/build/conf.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    10222 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/docs/build/core_usage.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)      769 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/docs/build/front.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)     1215 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/docs/build/index.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)     9296 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/docs/build/recipes.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)      178 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/docs/build/requirements.txt
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:54.435534 dogpile.cache-1.2.0/docs/build/unreleased/
+-rw-r--r--   0 classic   (1000) classic   (1000)      410 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/docs/build/unreleased/README.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)    11625 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/docs/build/usage.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)   132742 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/changelog.html
+-rw-r--r--   0 classic   (1000) classic   (1000)    28474 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/core_usage.html
+-rw-r--r--   0 classic   (1000) classic   (1000)     6492 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/front.html
+-rw-r--r--   0 classic   (1000) classic   (1000)    67476 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/genindex.html
+-rw-r--r--   0 classic   (1000) classic   (1000)    14900 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/index.html
+-rw-r--r--   0 classic   (1000) classic   (1000)     5958 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/py-modindex.html
+-rw-r--r--   0 classic   (1000) classic   (1000)    32468 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/recipes.html
+-rw-r--r--   0 classic   (1000) classic   (1000)     3509 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/search.html
+-rw-r--r--   0 classic   (1000) classic   (1000)    74849 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/searchindex.js
+-rw-r--r--   0 classic   (1000) classic   (1000)   111861 2023-04-26 15:47:53.000000 dogpile.cache-1.2.0/docs/usage.html
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:54.421533 dogpile.cache-1.2.0/dogpile/
+-rw-r--r--   0 classic   (1000) classic   (1000)      106 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/__init__.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:54.422534 dogpile.cache-1.2.0/dogpile/cache/
+-rw-r--r--   0 classic   (1000) classic   (1000)      180 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/cache/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    16890 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/cache/api.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:54.423534 dogpile.cache-1.2.0/dogpile/cache/backends/
+-rw-r--r--   0 classic   (1000) classic   (1000)     1197 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/cache/backends/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    13749 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/cache/backends/file.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    20835 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/cache/backends/memcached.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     3030 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/cache/backends/memory.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     1167 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/cache/backends/null.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    11764 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/cache/backends/redis.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      601 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/cache/exception.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:54.424533 dogpile.cache-1.2.0/dogpile/cache/plugins/
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/cache/plugins/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     2964 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/cache/plugins/mako_cache.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     3610 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/cache/proxy.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    68481 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/cache/region.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     5418 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/cache/util.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      565 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/core.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     7077 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/lock.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:54.425534 dogpile.cache-1.2.0/dogpile/util/
+-rw-r--r--   0 classic   (1000) classic   (1000)      339 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/util/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     1735 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/util/compat.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     4479 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/util/langhelpers.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     2801 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/util/nameregistry.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     4532 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/dogpile/util/readwrite_lock.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:54.437534 dogpile.cache-1.2.0/dogpile.cache.egg-info/
+-rw-r--r--   0 classic   (1000) classic   (1000)     4895 2023-04-26 15:47:54.000000 dogpile.cache-1.2.0/dogpile.cache.egg-info/PKG-INFO
+-rw-r--r--   0 classic   (1000) classic   (1000)     2933 2023-04-26 15:47:54.000000 dogpile.cache-1.2.0/dogpile.cache.egg-info/SOURCES.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)        1 2023-04-26 15:47:54.000000 dogpile.cache-1.2.0/dogpile.cache.egg-info/dependency_links.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)       73 2023-04-26 15:47:54.000000 dogpile.cache-1.2.0/dogpile.cache.egg-info/entry_points.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)        1 2023-04-26 15:47:54.000000 dogpile.cache-1.2.0/dogpile.cache.egg-info/not-zip-safe
+-rw-r--r--   0 classic   (1000) classic   (1000)       34 2023-04-26 15:47:54.000000 dogpile.cache-1.2.0/dogpile.cache.egg-info/requires.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)        8 2023-04-26 15:47:54.000000 dogpile.cache-1.2.0/dogpile.cache.egg-info/top_level.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)      838 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/hash_port.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      513 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/log_tests.ini
+-rw-r--r--   0 classic   (1000) classic   (1000)     1595 2023-04-26 15:47:54.442534 dogpile.cache-1.2.0/setup.cfg
+-rw-r--r--   0 classic   (1000) classic   (1000)      558 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/setup.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:54.437534 dogpile.cache-1.2.0/tests/
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/__init__.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:54.439534 dogpile.cache-1.2.0/tests/cache/
+-rw-r--r--   0 classic   (1000) classic   (1000)      870 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/cache/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    16896 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/cache/_fixtures.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:54.439534 dogpile.cache-1.2.0/tests/cache/plugins/
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/cache/plugins/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     1389 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/cache/plugins/test_mako_cache.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     2972 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/cache/test_dbm_backend.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    18860 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/cache/test_decorator.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      405 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/cache/test_mako.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    16050 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/cache/test_memcached_backend.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      361 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/cache/test_memory_backend.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     1934 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/cache/test_null_backend.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     6693 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/cache/test_redis_backend.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     3468 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/cache/test_redis_sentinel_backend.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    32235 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/cache/test_region.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      769 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/conftest.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      552 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/test_backgrounding.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    10397 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/test_lock.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      893 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/test_utils.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:54.440534 dogpile.cache-1.2.0/tests/tls/
+-rw-r--r--   0 classic   (1000) classic   (1000)     2354 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/tls/ca-root.crt
+-rw-r--r--   0 classic   (1000) classic   (1000)     2354 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/tls/client-ca-root.crt
+-rw-r--r--   0 classic   (1000) classic   (1000)     1692 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/tls/client.crt
+-rw-r--r--   0 classic   (1000) classic   (1000)     1679 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/tls/client.key
+-rw-r--r--   0 classic   (1000) classic   (1000)     1675 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/tls/server.key
+-rw-r--r--   0 classic   (1000) classic   (1000)     4021 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/tls/server_chain.pem
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:54.441534 dogpile.cache-1.2.0/tests/util/
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/util/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     1535 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tests/util/test_nameregistry.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     2401 2023-04-26 15:47:38.000000 dogpile.cache-1.2.0/tox.ini
```

### Comparing `dogpile.cache-1.1.8/LICENSE` & `dogpile.cache-1.2.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2005-2022 Michael Bayer.
+Copyright 2005-2023 Michael Bayer.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
 so, subject to the following conditions:
```

### Comparing `dogpile.cache-1.1.8/PKG-INFO` & `dogpile.cache-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: dogpile.cache
-Version: 1.1.8
+Version: 1.2.0
 Summary: A caching front-end based on the Dogpile lock.
 Home-page: https://github.com/sqlalchemy/dogpile.cache
 Author: Mike Bayer
 Author-email: mike_mp@zzzcomputing.com
 License: MIT
 Project-URL: Documentation, https://dogpilecache.sqlalchemy.org
 Project-URL: Issue Tracker, https://github.com/sqlalchemy/dogpile.cache/
 Keywords: caching
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
@@ -107,9 +106,7 @@
 `Code of Conduct <https://www.sqlalchemy.org/codeofconduct.html>`_.
 
 License
 -------
 
 Dogpile is distributed under the `MIT license
 <https://opensource.org/licenses/MIT>`_.
-
-
```

### Comparing `dogpile.cache-1.1.8/README.rst` & `dogpile.cache-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/docs/_sources/api.rst.txt` & `dogpile.cache-1.2.0/docs/_sources/api.rst.txt`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/docs/_sources/changelog.rst.txt` & `dogpile.cache-1.2.0/docs/_sources/changelog.rst.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,28 @@
 =========
 Changelog
 =========
 
 .. changelog::
+    :version: 1.2.0
+    :released: Wed Apr 26 2023
+
+    .. change::
+        :tags: feature, region
+        :tickets: 236
+
+        Added new construct :class:`.api.CantDeserializeException` which can be
+        raised by user-defined deserializer functions which would be passed to
+        :paramref:`.CacheRegion.deserializer`, to indicate a cache value that can't
+        be deserialized and therefore should be regenerated. This can allow an
+        application that's been updated to gracefully re-cache old items that were
+        persisted from a previous version of the application. Pull request courtesy
+        Simon Hewitt.
+
+.. changelog::
     :version: 1.1.8
     :released: Fri Jul 8 2022
 
     .. change::
         :tags: bug, memcached
         :tickets: 223, 228
```

### Comparing `dogpile.cache-1.1.8/docs/_sources/core_usage.rst.txt` & `dogpile.cache-1.2.0/docs/_sources/core_usage.rst.txt`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/docs/_sources/front.rst.txt` & `dogpile.cache-1.2.0/docs/_sources/front.rst.txt`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/docs/_sources/index.rst.txt` & `dogpile.cache-1.2.0/docs/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/docs/_sources/recipes.rst.txt` & `dogpile.cache-1.2.0/docs/_sources/recipes.rst.txt`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/docs/_sources/usage.rst.txt` & `dogpile.cache-1.2.0/docs/_sources/usage.rst.txt`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/docs/_static/basic.css` & `dogpile.cache-1.2.0/docs/_static/basic.css`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 /*
  * basic.css
  * ~~~~~~~~~
  *
  * Sphinx stylesheet -- basic theme.
  *
- * :copyright: Copyright 2007-2022 by the Sphinx team, see AUTHORS.
+ * :copyright: Copyright 2007-2023 by the Sphinx team, see AUTHORS.
  * :license: BSD, see LICENSE for details.
  *
  */
 
 /* -- main layout ----------------------------------------------------------- */
 
 div.clearer {
@@ -232,24 +232,14 @@
     -webkit-hyphens: auto;
     hyphens: auto;
 }
 
 a.headerlink {
     visibility: hidden;
 }
-a.brackets:before,
-span.brackets > a:before{
-    content: "[";
-}
-
-a.brackets:after,
-span.brackets > a:after {
-    content: "]";
-}
-
 
 h1:hover > a.headerlink,
 h2:hover > a.headerlink,
 h3:hover > a.headerlink,
 h4:hover > a.headerlink,
 h5:hover > a.headerlink,
 h6:hover > a.headerlink,
@@ -330,19 +320,25 @@
     clear: right;
     overflow-x: auto;
 }
 
 p.sidebar-title {
     font-weight: bold;
 }
+
+nav.contents,
+aside.topic,
 div.admonition, div.topic, blockquote {
     clear: left;
 }
 
 /* -- topics ---------------------------------------------------------------- */
+
+nav.contents,
+aside.topic,
 div.topic {
     border: 1px solid #ccc;
     padding: 7px;
     margin: 10px 0 10px 0;
 }
 
 p.topic-title {
@@ -373,21 +369,25 @@
     margin-top: 25px;
 }
 
 /* -- content of sidebars/topics/admonitions -------------------------------- */
 
 div.sidebar > :last-child,
 aside.sidebar > :last-child,
+nav.contents > :last-child,
+aside.topic > :last-child,
 div.topic > :last-child,
 div.admonition > :last-child {
     margin-bottom: 0;
 }
 
 div.sidebar::after,
 aside.sidebar::after,
+nav.contents::after,
+aside.topic::after,
 div.topic::after,
 div.admonition::after,
 blockquote::after {
     display: block;
     content: '';
     clear: both;
 }
@@ -605,33 +605,14 @@
 }
 
 ol.simple p,
 ul.simple p {
     margin-bottom: 0;
 }
 
-/* Docutils 0.17 and older (footnotes & citations) */
-dl.footnote > dt,
-dl.citation > dt {
-    float: left;
-    margin-right: 0.5em;
-}
-
-dl.footnote > dd,
-dl.citation > dd {
-    margin-bottom: 0em;
-}
-
-dl.footnote > dd:after,
-dl.citation > dd:after {
-    content: "";
-    clear: both;
-}
-
-/* Docutils 0.18+ (footnotes & citations) */
 aside.footnote > span,
 div.citation > span {
     float: left;
 }
 aside.footnote > span:last-of-type,
 div.citation > span:last-of-type {
   padding-right: 0.5em;
@@ -648,32 +629,26 @@
 }
 aside.footnote > p:last-of-type:after,
 div.citation > p:last-of-type:after {
     content: "";
     clear: both;
 }
 
-/* Footnotes & citations ends */
-
 dl.field-list {
     display: grid;
     grid-template-columns: fit-content(30%) auto;
 }
 
 dl.field-list > dt {
     font-weight: bold;
     word-break: break-word;
     padding-left: 0.5em;
     padding-right: 5px;
 }
 
-dl.field-list > dt:after {
-    content: ":";
-}
-
 dl.field-list > dd {
     padding-left: 0.5em;
     margin-top: 0em;
     margin-left: 0em;
     margin-bottom: 0em;
 }
```

### Comparing `dogpile.cache-1.1.8/docs/_static/language_data.js` & `dogpile.cache-1.2.0/docs/_static/language_data.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 /*
  * language_data.js
  * ~~~~~~~~~~~~~~~~
  *
  * This script contains the language-specific data used by searchtools.js,
  * namely the list of stopwords, stemmer, scorer and splitter.
  *
- * :copyright: Copyright 2007-2022 by the Sphinx team, see AUTHORS.
+ * :copyright: Copyright 2007-2023 by the Sphinx team, see AUTHORS.
  * :license: BSD, see LICENSE for details.
  *
  */
 
 var stopwords = ["a", "and", "are", "as", "at", "be", "but", "by", "for", "if", "in", "into", "is", "it", "near", "no", "not", "of", "on", "or", "such", "that", "the", "their", "then", "there", "these", "they", "this", "to", "was", "will", "with"];
```

### Comparing `dogpile.cache-1.1.8/docs/_static/nature.css` & `dogpile.cache-1.2.0/docs/_static/nature.css`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 /*
  * nature.css_t
  * ~~~~~~~~~~~~
  *
  * Sphinx stylesheet -- nature theme.
  *
- * :copyright: Copyright 2007-2022 by the Sphinx team, see AUTHORS.
+ * :copyright: Copyright 2007-2023 by the Sphinx team, see AUTHORS.
  * :license: BSD, see LICENSE for details.
  *
  */
 
 @import url("basic.css");
 
 /* -- page layout ----------------------------------------------------------- */
@@ -189,14 +189,17 @@
     border: 1px solid #ccc;
 }
 
 div.seealso {
     background-color: #ffc;
     border: 1px solid #ff6;
 }
+
+nav.contents,
+aside.topic,
 div.topic {
     background-color: #eee;
 }
 
 div.warning {
     background-color: #ffe4e4;
     border: 1px solid #f66;
```

### Comparing `dogpile.cache-1.1.8/docs/_static/pygments.css` & `dogpile.cache-1.2.0/docs/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/docs/_static/searchtools.js` & `dogpile.cache-1.2.0/docs/_static/searchtools.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 /*
  * searchtools.js
  * ~~~~~~~~~~~~~~~~
  *
  * Sphinx JavaScript utilities for the full-text search.
  *
- * :copyright: Copyright 2007-2022 by the Sphinx team, see AUTHORS.
+ * :copyright: Copyright 2007-2023 by the Sphinx team, see AUTHORS.
  * :license: BSD, see LICENSE for details.
  *
  */
 "use strict";
 
 /**
  * Simple result scoring code.
@@ -53,22 +53,22 @@
 
 /**
  * See https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_Expressions#escaping
  */
 const _escapeRegExp = (string) =>
     string.replace(/[.*+\-?^${}()|[\]\\]/g, "\\$&"); // $& means the whole matched string
 
-const _displayItem = (item, highlightTerms, searchTerms) => {
+const _displayItem = (item, searchTerms) => {
     const docBuilder = DOCUMENTATION_OPTIONS.BUILDER;
     const docUrlRoot = DOCUMENTATION_OPTIONS.URL_ROOT;
     const docFileSuffix = DOCUMENTATION_OPTIONS.FILE_SUFFIX;
     const docLinkSuffix = DOCUMENTATION_OPTIONS.LINK_SUFFIX;
     const showSearchSummary = DOCUMENTATION_OPTIONS.SHOW_SEARCH_SUMMARY;
 
-    const [docName, title, anchor, descr] = item;
+    const [docName, title, anchor, descr, score, _filename] = item;
 
     let listItem = document.createElement("li");
     let requestUrl;
     let linkUrl;
     if (docBuilder === "dirhtml") {
         // dirhtml builder
         let dirname = docName + "/";
@@ -78,29 +78,28 @@
         requestUrl = docUrlRoot + dirname;
         linkUrl = requestUrl;
     } else {
         // normal html builders
         requestUrl = docUrlRoot + docName + docFileSuffix;
         linkUrl = docName + docLinkSuffix;
     }
-    const params = new URLSearchParams();
-    params.set("highlight", [...highlightTerms].join(" "));
     let linkEl = listItem.appendChild(document.createElement("a"));
-    linkEl.href = linkUrl + "?" + params.toString() + anchor;
+    linkEl.href = linkUrl + anchor;
+    linkEl.dataset.score = score;
     linkEl.innerHTML = title;
     if (descr)
-        listItem.appendChild(document.createElement("span")).innerText =
+        listItem.appendChild(document.createElement("span")).innerHTML =
         " (" + descr + ")";
     else if (showSearchSummary)
         fetch(requestUrl)
         .then((responseData) => responseData.text())
         .then((data) => {
             if (data)
                 listItem.appendChild(
-                    Search.makeSearchSummary(data, searchTerms, highlightTerms)
+                    Search.makeSearchSummary(data, searchTerms)
                 );
         });
     Search.output.appendChild(listItem);
 };
 const _finishSearch = (resultCount) => {
     Search.stopPulse();
     Search.title.innerText = _("Search Results");
@@ -112,23 +111,22 @@
         Search.status.innerText = _(
             `Search finished, found ${resultCount} page(s) matching the search query.`
         );
 };
 const _displayNextItem = (
     results,
     resultCount,
-    highlightTerms,
     searchTerms
 ) => {
     // results left, load the summary and display it
     // this is intended to be dynamic (don't sub resultsCount)
     if (results.length) {
-        _displayItem(results.pop(), highlightTerms, searchTerms);
+        _displayItem(results.pop(), searchTerms);
         setTimeout(
-            () => _displayNextItem(results, resultCount, highlightTerms, searchTerms),
+            () => _displayNextItem(results, resultCount, searchTerms),
             5
         );
     }
     // search finished, update title and status message
     else _finishSearch(resultCount);
 };
 
@@ -151,18 +149,18 @@
  */
 const Search = {
     _index: null,
     _queued_query: null,
     _pulse_status: -1,
 
     htmlToText: (htmlString) => {
-        const htmlElement = document
-            .createRange()
-            .createContextualFragment(htmlString);
-        _removeChildren(htmlElement.querySelectorAll(".headerlink"));
+        const htmlElement = new DOMParser().parseFromString(htmlString, 'text/html');
+        htmlElement.querySelectorAll(".headerlink").forEach((el) => {
+            el.remove()
+        });
         const docContent = htmlElement.querySelector('[role="main"]');
         if (docContent !== undefined) return docContent.textContent;
         console.warn(
             "Content block not found. Sphinx search tries to obtain it via '[role=main]'. Could you check your theme or template."
         );
         return "";
     },
@@ -235,14 +233,20 @@
         else Search.deferQuery(query);
     },
 
     /**
      * execute search (requires search index to be loaded)
      */
     query: (query) => {
+        const filenames = Search._index.filenames;
+        const docNames = Search._index.docnames;
+        const titles = Search._index.titles;
+        const allTitles = Search._index.alltitles;
+        const indexEntries = Search._index.indexentries;
+
         // stem the search terms and add them to the correct list
         const stemmer = new Stemmer();
         const searchTerms = new Set();
         const excludedTerms = new Set();
         const highlightTerms = new Set();
         const objectTerms = new Set(splitQuery(query.toLowerCase().trim()));
         splitQuery(query.trim()).forEach((queryTerm) => {
@@ -262,22 +266,60 @@
             if (word[0] === "-") excludedTerms.add(word.substr(1));
             else {
                 searchTerms.add(word);
                 highlightTerms.add(queryTermLower);
             }
         });
 
+        if (SPHINX_HIGHLIGHT_ENABLED) { // set in sphinx_highlight.js
+            localStorage.setItem("sphinx_highlight_terms", [...highlightTerms].join(" "))
+        }
+
         // console.debug("SEARCH: searching for:");
         // console.info("required: ", [...searchTerms]);
         // console.info("excluded: ", [...excludedTerms]);
 
         // array of [docname, title, anchor, descr, score, filename]
         let results = [];
         _removeChildren(document.getElementById("search-progress"));
 
+        const queryLower = query.toLowerCase();
+        for (const [title, foundTitles] of Object.entries(allTitles)) {
+            if (title.toLowerCase().includes(queryLower) && (queryLower.length >= title.length / 2)) {
+                for (const [file, id] of foundTitles) {
+                    let score = Math.round(100 * queryLower.length / title.length)
+                    results.push([
+                        docNames[file],
+                        titles[file] !== title ? `${titles[file]} > ${title}` : title,
+                        id !== null ? "#" + id : "",
+                        null,
+                        score,
+                        filenames[file],
+                    ]);
+                }
+            }
+        }
+
+        // search for explicit entries in index directives
+        for (const [entry, foundEntries] of Object.entries(indexEntries)) {
+            if (entry.includes(queryLower) && (queryLower.length >= entry.length / 2)) {
+                for (const [file, id] of foundEntries) {
+                    let score = Math.round(100 * queryLower.length / entry.length)
+                    results.push([
+                        docNames[file],
+                        titles[file],
+                        id ? "#" + id : "",
+                        null,
+                        score,
+                        filenames[file],
+                    ]);
+                }
+            }
+        }
+
         // lookup as object
         objectTerms.forEach((term) =>
             results.push(...Search.performObjectSearch(term, objectTerms))
         );
 
         // lookup as search terms in fulltext
         results.push(...Search.performTermsSearch(searchTerms, excludedTerms));
@@ -316,15 +358,15 @@
         results = results.reverse();
 
         // for debugging
         //Search.lastresults = results.slice();  // a copy
         // console.info("search results:", Search.lastresults);
 
         // print the results
-        _displayNextItem(results, results.length, highlightTerms, searchTerms);
+        _displayNextItem(results, results.length, searchTerms);
     },
 
     /**
      * search for object names
      */
     performObjectSearch: (object, objectTerms) => {
         const filenames = Search._index.filenames;
@@ -397,16 +439,16 @@
     /**
      * search for full-text terms in the index
      */
     performTermsSearch: (searchTerms, excludedTerms) => {
         // prepare search
         const terms = Search._index.terms;
         const titleTerms = Search._index.titleterms;
-        const docNames = Search._index.docnames;
         const filenames = Search._index.filenames;
+        const docNames = Search._index.docnames;
         const titles = Search._index.titles;
 
         const scoreMap = new Map();
         const fileMap = new Map();
 
         // perform the search on the required terms
         searchTerms.forEach((word) => {
@@ -504,37 +546,32 @@
         }
         return results;
     },
 
     /**
      * helper function to return a node containing the
      * search summary for a given text. keywords is a list
-     * of stemmed words, highlightWords is the list of normal, unstemmed
-     * words. the first one is used to find the occurrence, the
-     * latter for highlighting it.
+     * of stemmed words.
      */
-    makeSearchSummary: (htmlText, keywords, highlightWords) => {
-        const text = Search.htmlToText(htmlText).toLowerCase();
+    makeSearchSummary: (htmlText, keywords) => {
+        const text = Search.htmlToText(htmlText);
         if (text === "") return null;
 
+        const textLower = text.toLowerCase();
         const actualStartPosition = [...keywords]
-            .map((k) => text.indexOf(k.toLowerCase()))
+            .map((k) => textLower.indexOf(k.toLowerCase()))
             .filter((i) => i > -1)
             .slice(-1)[0];
         const startWithContext = Math.max(actualStartPosition - 120, 0);
 
         const top = startWithContext === 0 ? "" : "...";
         const tail = startWithContext + 240 < text.length ? "..." : "";
 
-        let summary = document.createElement("div");
+        let summary = document.createElement("p");
         summary.classList.add("context");
-        summary.innerText = top + text.substr(startWithContext, 240).trim() + tail;
-
-        highlightWords.forEach((highlightWord) =>
-            _highlightText(summary, highlightWord, "highlighted")
-        );
+        summary.textContent = top + text.substr(startWithContext, 240).trim() + tail;
 
         return summary;
     },
 };
 
 _ready(Search.init);
```

### Comparing `dogpile.cache-1.1.8/docs/api.html` & `dogpile.cache-1.2.0/docs/api.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>API &#8212; dogpile.cache 1.1.8 documentation</title>
+    <title>API &#8212; dogpile.cache 1.2.0 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
-    <script src="_static/jquery.js"></script>
-    <script src="_static/underscore.js"></script>
-    <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
     <script src="_static/doctools.js"></script>
+    <script src="_static/sphinx_highlight.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Changelog" href="changelog.html" />
     <link rel="prev" title="dogpile Core" href="core_usage.html" /> 
   </head><body>
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
@@ -32,15 +30,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="changelog.html" title="Changelog"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="core_usage.html" title="dogpile Core"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.1.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.0 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">API</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -48,19 +46,19 @@
             
   <section id="api">
 <h1>API<a class="headerlink" href="#api" title="Permalink to this heading">¶</a></h1>
 <section id="module-dogpile.cache.region">
 <span id="region"></span><h2>Region<a class="headerlink" href="#module-dogpile.cache.region" title="Permalink to this heading">¶</a></h2>
 <dl class="py class">
 <dt class="sig sig-object py" id="dogpile.cache.region.CacheRegion">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">dogpile.cache.region.</span></span><span class="sig-name descname"><span class="pre">CacheRegion</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="pre">name:</span> <span class="pre">~typing.Optional[str]</span> <span class="pre">=</span> <span class="pre">None,</span> <span class="pre">function_key_generator:</span> <span class="pre">~typing.Callable[[...],</span> <span class="pre">~typing.Callable[[...],</span> <span class="pre">str]]</span> <span class="pre">=</span> <span class="pre">&lt;function</span> <span class="pre">function_key_generator&gt;,</span> <span class="pre">function_multi_key_generator:</span> <span class="pre">~typing.Callable[[...],</span> <span class="pre">~typing.Callable[[...],</span> <span class="pre">~typing.Sequence[str]]]</span> <span class="pre">=</span> <span class="pre">&lt;function</span> <span class="pre">function_multi_key_generator&gt;,</span> <span class="pre">key_mangler:</span> <span class="pre">~typing.Optional[~typing.Callable[[str],</span> <span class="pre">str]]</span> <span class="pre">=</span> <span class="pre">None,</span> <span class="pre">serializer:</span> <span class="pre">~typing.Optional[~typing.Callable[[~typing.Any],</span> <span class="pre">bytes]]</span> <span class="pre">=</span> <span class="pre">None,</span> <span class="pre">deserializer:</span> <span class="pre">~typing.Optional[~typing.Callable[[bytes],</span> <span class="pre">~typing.Any]]</span> <span class="pre">=</span> <span class="pre">None,</span> <span class="pre">async_creation_runner:</span> <span class="pre">~typing.Optional[~typing.Callable[[~dogpile.cache.region.CacheRegion,</span> <span class="pre">str,</span> <span class="pre">~typing.Callable[[],</span> <span class="pre">~typing.Any],</span> <span class="pre">~dogpile.cache.api.CacheMutex],</span> <span class="pre">None]]</span> <span class="pre">=</span> <span class="pre">None</span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.region.CacheRegion" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">dogpile.cache.region.</span></span><span class="sig-name descname"><span class="pre">CacheRegion</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="pre">name:</span> <span class="pre">str</span> <span class="pre">|</span> <span class="pre">None</span> <span class="pre">=</span> <span class="pre">None,</span> <span class="pre">function_key_generator:</span> <span class="pre">~typing.Callable[[...],</span> <span class="pre">~typing.Callable[[...],</span> <span class="pre">str]]</span> <span class="pre">=</span> <span class="pre">&lt;function</span> <span class="pre">function_key_generator&gt;,</span> <span class="pre">function_multi_key_generator:</span> <span class="pre">~typing.Callable[[...],</span> <span class="pre">~typing.Callable[[...],</span> <span class="pre">~typing.Sequence[str]]]</span> <span class="pre">=</span> <span class="pre">&lt;function</span> <span class="pre">function_multi_key_generator&gt;,</span> <span class="pre">key_mangler:</span> <span class="pre">~typing.Callable[[str],</span> <span class="pre">str]</span> <span class="pre">|</span> <span class="pre">None</span> <span class="pre">=</span> <span class="pre">None,</span> <span class="pre">serializer:</span> <span class="pre">~typing.Callable[[~typing.Any],</span> <span class="pre">bytes]</span> <span class="pre">|</span> <span class="pre">None</span> <span class="pre">=</span> <span class="pre">None,</span> <span class="pre">deserializer:</span> <span class="pre">~typing.Callable[[bytes],</span> <span class="pre">~typing.Any]</span> <span class="pre">|</span> <span class="pre">None</span> <span class="pre">=</span> <span class="pre">None,</span> <span class="pre">async_creation_runner:</span> <span class="pre">~typing.Callable[[~dogpile.cache.region.CacheRegion,</span> <span class="pre">str,</span> <span class="pre">~typing.Callable[[],</span> <span class="pre">~typing.Any],</span> <span class="pre">~dogpile.cache.api.CacheMutex],</span> <span class="pre">None]</span> <span class="pre">|</span> <span class="pre">None</span> <span class="pre">=</span> <span class="pre">None</span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.region.CacheRegion" title="Permalink to this definition">¶</a></dt>
 <dd><p>Bases: <code class="xref py py-class docutils literal notranslate"><span class="pre">object</span></code></p>
 <p>A front end to a particular cache backend.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.params.name"></span><strong>name</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.params.name">¶</a> – Optional, a string name for the region.
 This isn’t used internally
 but can be accessed via the <code class="docutils literal notranslate"><span class="pre">.name</span></code> parameter, helpful
 for configuring a region from a config file.</p></li>
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.params.function_key_generator"></span><strong>function_key_generator</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.params.function_key_generator">¶</a> – <p>Optional.  A
 function that will produce a “cache key” given
@@ -149,16 +147,26 @@
 <p><span class="versionmodified added">New in version 1.1.0.</span></p>
 </div>
 </p></li>
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.params.deserializer"></span><strong>deserializer</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.params.deserializer">¶</a> – <p>function which will be applied to all values returned
 by the backend.  Defaults to <code class="docutils literal notranslate"><span class="pre">None</span></code>, in which case the
 deserializer recommended by the backend will be used.   Typical
 deserializers include <code class="docutils literal notranslate"><span class="pre">pickle.dumps</span></code> and <code class="docutils literal notranslate"><span class="pre">json.dumps</span></code>.</p>
+<p>Deserializers can raise a <a class="reference internal" href="#dogpile.cache.api.CantDeserializeException" title="dogpile.cache.api.CantDeserializeException"><code class="xref py py-class docutils literal notranslate"><span class="pre">api.CantDeserializeException</span></code></a> if they
+are unable to deserialize the value from the backend, indicating
+deserialization failed and that caching should proceed to re-generate
+a value.  This allows an application that has been updated to gracefully
+re-cache old items which were persisted by a previous version of the
+application and can no longer be successfully deserialized.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.0.</span></p>
+<p><span class="versionmodified added">New in version 1.1.0: </span>added “deserializer” parameter</p>
+</div>
+<div class="versionadded">
+<p><span class="versionmodified added">New in version 1.2.0: </span>added support for
+<a class="reference internal" href="#dogpile.cache.api.CantDeserializeException" title="dogpile.cache.api.CantDeserializeException"><code class="xref py py-class docutils literal notranslate"><span class="pre">api.CantDeserializeException</span></code></a></p>
 </div>
 </p></li>
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.params.async_creation_runner"></span><strong>async_creation_runner</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.params.async_creation_runner">¶</a> – <p>A callable that, when specified,
 will be passed to and called by dogpile.lock when
 there is a stale value present in the cache.  It will be passed the
 mutex and is responsible releasing that mutex when finished.
 This can be used to defer the computation of expensive creator
@@ -166,15 +174,15 @@
 background thread, a long-running queue, or a task manager system
 like Celery.</p>
 <p>For a specific example using async_creation_runner, new values can
 be created in a background thread like so:</p>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="kn">import</span> <span class="nn">threading</span>
 
 <span class="k">def</span> <span class="nf">async_creation_runner</span><span class="p">(</span><span class="n">cache</span><span class="p">,</span> <span class="n">somekey</span><span class="p">,</span> <span class="n">creator</span><span class="p">,</span> <span class="n">mutex</span><span class="p">):</span>
-    <span class="sd">&#39;&#39;&#39; Used by dogpile.core:Lock when appropriate  &#39;&#39;&#39;</span>
+<span class="w">    </span><span class="sd">&#39;&#39;&#39; Used by dogpile.core:Lock when appropriate  &#39;&#39;&#39;</span>
     <span class="k">def</span> <span class="nf">runner</span><span class="p">():</span>
         <span class="k">try</span><span class="p">:</span>
             <span class="n">value</span> <span class="o">=</span> <span class="n">creator</span><span class="p">()</span>
             <span class="n">cache</span><span class="o">.</span><span class="n">set</span><span class="p">(</span><span class="n">somekey</span><span class="p">,</span> <span class="n">value</span><span class="p">)</span>
         <span class="k">finally</span><span class="p">:</span>
             <span class="n">mutex</span><span class="o">.</span><span class="n">release</span><span class="p">()</span>
 
@@ -219,15 +227,15 @@
 <div class="versionadded">
 <p><span class="versionmodified added">New in version 0.6.6.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.region.CacheRegion.cache_multi_on_arguments">
-<span class="sig-name descname"><span class="pre">cache_multi_on_arguments</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="pre">namespace:</span> <span class="pre">~typing.Optional[str]</span> <span class="pre">=</span> <span class="pre">None,</span> <span class="pre">expiration_time:</span> <span class="pre">~typing.Optional[~typing.Union[float,</span> <span class="pre">~typing.Callable[[],</span> <span class="pre">float]]]</span> <span class="pre">=</span> <span class="pre">None,</span> <span class="pre">should_cache_fn:</span> <span class="pre">~typing.Optional[~typing.Callable[[~typing.Any],</span> <span class="pre">bool]]</span> <span class="pre">=</span> <span class="pre">None,</span> <span class="pre">asdict:</span> <span class="pre">bool</span> <span class="pre">=</span> <span class="pre">False,</span> <span class="pre">to_str:</span> <span class="pre">~typing.Callable[[~typing.Any],</span> <span class="pre">str]</span> <span class="pre">=</span> <span class="pre">&lt;class</span> <span class="pre">'str'&gt;,</span> <span class="pre">function_multi_key_generator:</span> <span class="pre">~typing.Optional[~typing.Callable[[...],</span> <span class="pre">~typing.Callable[[...],</span> <span class="pre">~typing.Sequence[str]]]]</span> <span class="pre">=</span> <span class="pre">None</span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">...</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">...</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Mapping</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#dogpile.cache.region.CacheRegion.cache_multi_on_arguments" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">cache_multi_on_arguments</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="pre">namespace:</span> <span class="pre">str</span> <span class="pre">|</span> <span class="pre">None</span> <span class="pre">=</span> <span class="pre">None,</span> <span class="pre">expiration_time:</span> <span class="pre">float</span> <span class="pre">|</span> <span class="pre">~typing.Callable[[],</span> <span class="pre">float]</span> <span class="pre">|</span> <span class="pre">None</span> <span class="pre">=</span> <span class="pre">None,</span> <span class="pre">should_cache_fn:</span> <span class="pre">~typing.Callable[[~typing.Any],</span> <span class="pre">bool]</span> <span class="pre">|</span> <span class="pre">None</span> <span class="pre">=</span> <span class="pre">None,</span> <span class="pre">asdict:</span> <span class="pre">bool</span> <span class="pre">=</span> <span class="pre">False,</span> <span class="pre">to_str:</span> <span class="pre">~typing.Callable[[~typing.Any],</span> <span class="pre">str]</span> <span class="pre">=</span> <span class="pre">&lt;class</span> <span class="pre">'str'&gt;,</span> <span class="pre">function_multi_key_generator:</span> <span class="pre">~typing.Callable[[...],</span> <span class="pre">~typing.Callable[[...],</span> <span class="pre">~typing.Sequence[str]]]</span> <span class="pre">|</span> <span class="pre">None</span> <span class="pre">=</span> <span class="pre">None</span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">...</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">...</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">Mapping</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#dogpile.cache.region.CacheRegion.cache_multi_on_arguments" title="Permalink to this definition">¶</a></dt>
 <dd><p>A function decorator that will cache multiple return
 values from the function using a sequence of keys derived from the
 function itself and the arguments passed to it.</p>
 <p>This method is the “multiple key” analogue to the
 <a class="reference internal" href="#dogpile.cache.region.CacheRegion.cache_on_arguments" title="dogpile.cache.region.CacheRegion.cache_on_arguments"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.cache_on_arguments()</span></code></a> method.</p>
 <p>Example:</p>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="nd">@someregion</span><span class="o">.</span><span class="n">cache_multi_on_arguments</span><span class="p">()</span>
@@ -288,15 +296,15 @@
 <p><span class="versionmodified added">New in version 0.5.3: </span>Added <code class="docutils literal notranslate"><span class="pre">get()</span></code> method to decorated
 function.</p>
 </div>
 <p>Parameters passed to <a class="reference internal" href="#dogpile.cache.region.CacheRegion.cache_multi_on_arguments" title="dogpile.cache.region.CacheRegion.cache_multi_on_arguments"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.cache_multi_on_arguments()</span></code></a>
 have the same meaning as those passed to
 <a class="reference internal" href="#dogpile.cache.region.CacheRegion.cache_on_arguments" title="dogpile.cache.region.CacheRegion.cache_on_arguments"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.cache_on_arguments()</span></code></a>.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.cache_multi_on_arguments.params.namespace"></span><strong>namespace</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.cache_multi_on_arguments.params.namespace">¶</a> – optional string argument which will be
 established as part of each cache key.</p></li>
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.cache_multi_on_arguments.params.expiration_time"></span><strong>expiration_time</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.cache_multi_on_arguments.params.expiration_time">¶</a> – if not None, will override the normal
 expiration time.  May be passed as an integer or a
 callable.</p></li>
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.cache_multi_on_arguments.params.should_cache_fn"></span><strong>should_cache_fn</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.cache_multi_on_arguments.params.should_cache_fn">¶</a> – passed to
@@ -321,15 +329,15 @@
 </ul>
 </dd>
 </dl>
 <div class="versionadded">
 <p><span class="versionmodified added">New in version 0.5.0.</span></p>
 </div>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.region.CacheRegion.cache_multi_on_arguments.params.function_multi_key_generator"></span><strong>function_multi_key_generator</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.cache_multi_on_arguments.params.function_multi_key_generator">¶</a> – <p>a function that will produce a
 list of keys. This function will supersede the one configured on the
 <a class="reference internal" href="#dogpile.cache.region.CacheRegion" title="dogpile.cache.region.CacheRegion"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheRegion</span></code></a> itself.</p>
 <div class="versionadded">
 <p><span class="versionmodified added">New in version 0.5.5.</span></p>
 </div>
 </p>
@@ -340,15 +348,15 @@
 <p><a class="reference internal" href="#dogpile.cache.region.CacheRegion.cache_on_arguments" title="dogpile.cache.region.CacheRegion.cache_on_arguments"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.cache_on_arguments()</span></code></a></p>
 <p><a class="reference internal" href="#dogpile.cache.region.CacheRegion.get_or_create_multi" title="dogpile.cache.region.CacheRegion.get_or_create_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get_or_create_multi()</span></code></a></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.region.CacheRegion.cache_on_arguments">
-<span class="sig-name descname"><span class="pre">cache_on_arguments</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="pre">namespace:</span> <span class="pre">~typing.Optional[str]</span> <span class="pre">=</span> <span class="pre">None,</span> <span class="pre">expiration_time:</span> <span class="pre">~typing.Optional[~typing.Union[float,</span> <span class="pre">~typing.Callable[[],</span> <span class="pre">float]]]</span> <span class="pre">=</span> <span class="pre">None,</span> <span class="pre">should_cache_fn:</span> <span class="pre">~typing.Optional[~typing.Callable[[~typing.Any],</span> <span class="pre">bool]]</span> <span class="pre">=</span> <span class="pre">None,</span> <span class="pre">to_str:</span> <span class="pre">~typing.Callable[[~typing.Any],</span> <span class="pre">str]</span> <span class="pre">=</span> <span class="pre">&lt;class</span> <span class="pre">'str'&gt;,</span> <span class="pre">function_key_generator:</span> <span class="pre">~typing.Optional[~typing.Callable[[...],</span> <span class="pre">~typing.Callable[[...],</span> <span class="pre">str]]]</span> <span class="pre">=</span> <span class="pre">None</span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">...</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">...</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#dogpile.cache.region.CacheRegion.cache_on_arguments" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">cache_on_arguments</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="pre">namespace:</span> <span class="pre">str</span> <span class="pre">|</span> <span class="pre">None</span> <span class="pre">=</span> <span class="pre">None,</span> <span class="pre">expiration_time:</span> <span class="pre">float</span> <span class="pre">|</span> <span class="pre">~typing.Callable[[],</span> <span class="pre">float]</span> <span class="pre">|</span> <span class="pre">None</span> <span class="pre">=</span> <span class="pre">None,</span> <span class="pre">should_cache_fn:</span> <span class="pre">~typing.Callable[[~typing.Any],</span> <span class="pre">bool]</span> <span class="pre">|</span> <span class="pre">None</span> <span class="pre">=</span> <span class="pre">None,</span> <span class="pre">to_str:</span> <span class="pre">~typing.Callable[[~typing.Any],</span> <span class="pre">str]</span> <span class="pre">=</span> <span class="pre">&lt;class</span> <span class="pre">'str'&gt;,</span> <span class="pre">function_key_generator:</span> <span class="pre">~typing.Callable[[...],</span> <span class="pre">~typing.Callable[[...],</span> <span class="pre">str]]</span> <span class="pre">|</span> <span class="pre">None</span> <span class="pre">=</span> <span class="pre">None</span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">...</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">...</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#dogpile.cache.region.CacheRegion.cache_on_arguments" title="Permalink to this definition">¶</a></dt>
 <dd><p>A function decorator that will cache the return
 value of the function using a key derived from the
 function itself and its arguments.</p>
 <p>The decorator internally makes use of the
 <a class="reference internal" href="#dogpile.cache.region.CacheRegion.get_or_create" title="dogpile.cache.region.CacheRegion.get_or_create"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get_or_create()</span></code></a> method to access the
 cache and conditionally call the function.  See that
 method for additional behavioral details.</p>
@@ -468,15 +476,15 @@
 by the decorator before it becomes an instance method.</p>
 <p>The function key generation can be entirely replaced
 on a per-region basis using the <code class="docutils literal notranslate"><span class="pre">function_key_generator</span></code>
 argument present on <a class="reference internal" href="#dogpile.cache.region.make_region" title="dogpile.cache.region.make_region"><code class="xref py py-func docutils literal notranslate"><span class="pre">make_region()</span></code></a> and
 <a class="reference internal" href="#dogpile.cache.region.CacheRegion" title="dogpile.cache.region.CacheRegion"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheRegion</span></code></a>. If defaults to
 <a class="reference internal" href="#dogpile.cache.util.function_key_generator" title="dogpile.cache.util.function_key_generator"><code class="xref py py-func docutils literal notranslate"><span class="pre">function_key_generator()</span></code></a>.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.cache_on_arguments.params.namespace"></span><strong>namespace</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.cache_on_arguments.params.namespace">¶</a> – optional string argument which will be
 established as part of the cache key.   This may be needed
 to disambiguate functions of the same name within the same
 source file, such as those
 associated with classes - note that the decorator itself
 can’t see the parent class on a function as the class is
@@ -510,20 +518,20 @@
 <p><a class="reference internal" href="#dogpile.cache.region.CacheRegion.cache_multi_on_arguments" title="dogpile.cache.region.CacheRegion.cache_multi_on_arguments"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.cache_multi_on_arguments()</span></code></a></p>
 <p><a class="reference internal" href="#dogpile.cache.region.CacheRegion.get_or_create" title="dogpile.cache.region.CacheRegion.get_or_create"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get_or_create()</span></code></a></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.region.CacheRegion.configure">
-<span class="sig-name descname"><span class="pre">configure</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">backend</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">expiration_time</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><span class="pre">float</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">timedelta</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">arguments</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Mapping</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">_config_argument_dict</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Mapping</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">_config_prefix</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">wrap</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><span class="pre">ProxyBackend</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Type</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><span class="pre">ProxyBackend</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">()</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">replace_existing_backend</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">region_invalidator</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#dogpile.cache.region.RegionInvalidationStrategy" title="dogpile.cache.region.RegionInvalidationStrategy"><span class="pre">RegionInvalidationStrategy</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#dogpile.cache.region.CacheRegion" title="dogpile.cache.region.CacheRegion"><span class="pre">CacheRegion</span></a></span></span><a class="headerlink" href="#dogpile.cache.region.CacheRegion.configure" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">configure</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">backend</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">expiration_time</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">timedelta</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">arguments</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Mapping</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">_config_argument_dict</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Mapping</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">_config_prefix</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">wrap</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><span class="pre">ProxyBackend</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">Type</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><span class="pre">ProxyBackend</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">()</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">replace_existing_backend</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">region_invalidator</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#dogpile.cache.region.RegionInvalidationStrategy" title="dogpile.cache.region.RegionInvalidationStrategy"><span class="pre">RegionInvalidationStrategy</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#dogpile.cache.region.CacheRegion" title="dogpile.cache.region.CacheRegion"><span class="pre">CacheRegion</span></a></span></span><a class="headerlink" href="#dogpile.cache.region.CacheRegion.configure" title="Permalink to this definition">¶</a></dt>
 <dd><p>Configure a <a class="reference internal" href="#dogpile.cache.region.CacheRegion" title="dogpile.cache.region.CacheRegion"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheRegion</span></code></a>.</p>
 <p>The <a class="reference internal" href="#dogpile.cache.region.CacheRegion" title="dogpile.cache.region.CacheRegion"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheRegion</span></code></a> itself
 is returned.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.configure.params.backend"></span><strong>backend</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.configure.params.backend">¶</a> – Required.  This is the name of the
 <a class="reference internal" href="#dogpile.cache.api.CacheBackend" title="dogpile.cache.api.CacheBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheBackend</span></code></a> to use, and is resolved by loading
 the class from the <code class="docutils literal notranslate"><span class="pre">dogpile.cache</span></code> entrypoint.</p></li>
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.configure.params.expiration_time"></span><strong>expiration_time</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.configure.params.expiration_time">¶</a> – <p>Optional.  The expiration time passed
 to the dogpile system.  May be passed as an integer number
 of seconds, or as a <code class="docutils literal notranslate"><span class="pre">datetime.timedelta</span></code> value.</p>
@@ -640,15 +648,15 @@
 Passing the flag <code class="docutils literal notranslate"><span class="pre">ignore_expiration=True</span></code> bypasses
 the invalidation time check.</p>
 <div class="versionadded">
 <p><span class="versionmodified added">New in version 0.3.0: </span>Support for the <a class="reference internal" href="#dogpile.cache.region.CacheRegion.invalidate" title="dogpile.cache.region.CacheRegion.invalidate"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.invalidate()</span></code></a>
 method.</p>
 </div>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.get.params.key"></span><strong>key</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.get.params.key">¶</a> – Key to be retrieved. While it’s typical for a key to be a
 string, it is ultimately passed directly down to the cache backend,
 before being optionally processed by the key_mangler function, so can
 be of any type recognized by the backend or by the key_mangler
 function, if present.</p></li>
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.get.params.expiration_time"></span><strong>expiration_time</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.get.params.expiration_time">¶</a> – <p>Optional expiration time value
@@ -717,15 +725,15 @@
 <div class="versionadded">
 <p><span class="versionmodified added">New in version 0.5.0.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.region.CacheRegion.get_or_create">
-<span class="sig-name descname"><span class="pre">get_or_create</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">creator</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">...</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">expiration_time</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">float</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">should_cache_fn</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">creator_args</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Tuple</span><span class="p"><span class="pre">[</span></span><span class="pre">Any</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Mapping</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Any</span></span></span><a class="headerlink" href="#dogpile.cache.region.CacheRegion.get_or_create" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">get_or_create</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">creator</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">...</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">expiration_time</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">should_cache_fn</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">creator_args</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Tuple</span><span class="p"><span class="pre">[</span></span><span class="pre">Any</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Mapping</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Any</span></span></span><a class="headerlink" href="#dogpile.cache.region.CacheRegion.get_or_create" title="Permalink to this definition">¶</a></dt>
 <dd><p>Return a cached value based on the given key.</p>
 <p>If the value does not exist or is considered to be expired
 based on its creation time, the given
 creation function may or may not be used to recreate the value
 and persist the newly generated value in the cache.</p>
 <p>Whether or not the function is used depends on if the
 <em>dogpile lock</em> can be acquired or not.  If it can’t, it means
@@ -742,15 +750,15 @@
 lock to generate a new value, or will wait
 until the lock is released to return the new value.</p>
 <div class="versionchanged">
 <p><span class="versionmodified changed">Changed in version 0.3.0: </span>The value is unconditionally regenerated if the creation
 time is older than the last call to <a class="reference internal" href="#dogpile.cache.region.CacheRegion.invalidate" title="dogpile.cache.region.CacheRegion.invalidate"><code class="xref py py-meth docutils literal notranslate"><span class="pre">invalidate()</span></code></a>.</p>
 </div>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.get_or_create.params.key"></span><strong>key</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.get_or_create.params.key">¶</a> – Key to be retrieved. While it’s typical for a key to be a
 string, it is ultimately passed directly down to the cache backend,
 before being optionally processed by the key_mangler function, so can
 be of any type recognized by the backend or by the key_mangler
 function, if present.</p></li>
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.get_or_create.params.creator"></span><strong>creator</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.get_or_create.params.creator">¶</a> – function which creates a new value.</p></li>
@@ -804,15 +812,15 @@
 <p><a class="reference internal" href="#dogpile.cache.region.CacheRegion.get_or_create_multi" title="dogpile.cache.region.CacheRegion.get_or_create_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get_or_create_multi()</span></code></a> - multiple key/value
 version</p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.region.CacheRegion.get_or_create_multi">
-<span class="sig-name descname"><span class="pre">get_or_create_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">keys</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">creator</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">expiration_time</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">float</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">should_cache_fn</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#dogpile.cache.region.CacheRegion.get_or_create_multi" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">get_or_create_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">keys</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">creator</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">expiration_time</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">should_cache_fn</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#dogpile.cache.region.CacheRegion.get_or_create_multi" title="Permalink to this definition">¶</a></dt>
 <dd><p>Return a sequence of cached values based on a sequence of keys.</p>
 <p>The behavior for generation of values based on keys corresponds
 to that of <code class="xref py py-meth docutils literal notranslate"><span class="pre">Region.get_or_create()</span></code>, with the exception that
 the <code class="docutils literal notranslate"><span class="pre">creator()</span></code> function may be asked to generate any subset of
 the given keys.   The list of keys to be generated is passed to
 <code class="docutils literal notranslate"><span class="pre">creator()</span></code>, and <code class="docutils literal notranslate"><span class="pre">creator()</span></code> should return the generated values
 as a sequence corresponding to the order of the keys.</p>
@@ -822,15 +830,15 @@
 <p>If you are using a <a class="reference internal" href="#dogpile.cache.api.CacheBackend" title="dogpile.cache.api.CacheBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheBackend</span></code></a> or <a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">ProxyBackend</span></code></a>
 that modifies values, take note this function invokes
 <code class="docutils literal notranslate"><span class="pre">.set_multi()</span></code> for newly generated values using the same values it
 returns to the calling function. A correct implementation of
 <code class="docutils literal notranslate"><span class="pre">.set_multi()</span></code> will not modify values in-place on the submitted
 <code class="docutils literal notranslate"><span class="pre">mapping</span></code> dict.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.get_or_create_multi.params.keys"></span><strong>keys</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.get_or_create_multi.params.keys">¶</a> – Sequence of keys to be retrieved.</p></li>
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.get_or_create_multi.params.creator"></span><strong>creator</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.get_or_create_multi.params.creator">¶</a> – function which accepts a sequence of keys and
 returns a sequence of new values.</p></li>
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.get_or_create_multi.params.expiration_time"></span><strong>expiration_time</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.get_or_create_multi.params.expiration_time">¶</a> – optional expiration time which will override
 the expiration time already configured on this <a class="reference internal" href="#dogpile.cache.region.CacheRegion" title="dogpile.cache.region.CacheRegion"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheRegion</span></code></a>
 if not None.   To set no expiration, use the value -1.</p></li>
@@ -886,15 +894,15 @@
 “old” value until the new one is available.</p>
 <p>Usage of “soft” invalidation requires that the region or the method
 is given a non-None expiration time.</p>
 <div class="versionadded">
 <p><span class="versionmodified added">New in version 0.3.0.</span></p>
 </div>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.region.CacheRegion.invalidate.params.hard"></span><strong>hard</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.invalidate.params.hard">¶</a> – <p>if True, cache values will all require immediate
 regeneration; dogpile logic won’t be used.  If False, the
 creation time of existing values will be pushed back before
 the expiration time so that a return+regen will be invoked.</p>
 <div class="versionadded">
 <p><span class="versionmodified added">New in version 0.5.1.</span></p>
 </div>
@@ -933,15 +941,15 @@
 <dt class="sig sig-object py" id="dogpile.cache.region.CacheRegion.set_multi">
 <span class="sig-name descname"><span class="pre">set_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">mapping</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Mapping</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#dogpile.cache.region.CacheRegion.set_multi" title="Permalink to this definition">¶</a></dt>
 <dd><p>Place new values in the cache under the given keys.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.region.CacheRegion.wrap">
-<span class="sig-name descname"><span class="pre">wrap</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">proxy</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><span class="pre">ProxyBackend</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Type</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><span class="pre">ProxyBackend</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#dogpile.cache.region.CacheRegion.wrap" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">wrap</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">proxy</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><span class="pre">ProxyBackend</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">Type</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><span class="pre">ProxyBackend</span></a><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#dogpile.cache.region.CacheRegion.wrap" title="Permalink to this definition">¶</a></dt>
 <dd><p>Takes a ProxyBackend instance or class and wraps the
 attached backend.</p>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
@@ -959,64 +967,64 @@
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.region.DefaultInvalidationStrategy.is_hard_invalidated">
 <span class="sig-name descname"><span class="pre">is_hard_invalidated</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">timestamp</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">bool</span></span></span><a class="headerlink" href="#dogpile.cache.region.DefaultInvalidationStrategy.is_hard_invalidated" title="Permalink to this definition">¶</a></dt>
 <dd><p>Check timestamp to determine if it was hard invalidated.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Returns</dt>
+<dt class="field-odd">Returns<span class="colon">:</span></dt>
 <dd class="field-odd"><p>Boolean. True if <code class="docutils literal notranslate"><span class="pre">timestamp</span></code> is older than
 the last region invalidation time and region is invalidated
 in hard mode.</p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.region.DefaultInvalidationStrategy.is_invalidated">
 <span class="sig-name descname"><span class="pre">is_invalidated</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">timestamp</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">bool</span></span></span><a class="headerlink" href="#dogpile.cache.region.DefaultInvalidationStrategy.is_invalidated" title="Permalink to this definition">¶</a></dt>
 <dd><p>Check timestamp to determine if it was invalidated.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Returns</dt>
+<dt class="field-odd">Returns<span class="colon">:</span></dt>
 <dd class="field-odd"><p>Boolean. True if <code class="docutils literal notranslate"><span class="pre">timestamp</span></code> is older than
 the last region invalidation time.</p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.region.DefaultInvalidationStrategy.is_soft_invalidated">
 <span class="sig-name descname"><span class="pre">is_soft_invalidated</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">timestamp</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">bool</span></span></span><a class="headerlink" href="#dogpile.cache.region.DefaultInvalidationStrategy.is_soft_invalidated" title="Permalink to this definition">¶</a></dt>
 <dd><p>Check timestamp to determine if it was soft invalidated.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Returns</dt>
+<dt class="field-odd">Returns<span class="colon">:</span></dt>
 <dd class="field-odd"><p>Boolean. True if <code class="docutils literal notranslate"><span class="pre">timestamp</span></code> is older than
 the last region invalidation time and region is invalidated
 in soft mode.</p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.region.DefaultInvalidationStrategy.was_hard_invalidated">
 <span class="sig-name descname"><span class="pre">was_hard_invalidated</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">bool</span></span></span><a class="headerlink" href="#dogpile.cache.region.DefaultInvalidationStrategy.was_hard_invalidated" title="Permalink to this definition">¶</a></dt>
 <dd><p>Indicate the region was invalidated in hard mode.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Returns</dt>
+<dt class="field-odd">Returns<span class="colon">:</span></dt>
 <dd class="field-odd"><p>Boolean. True if region was invalidated in hard mode.</p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.region.DefaultInvalidationStrategy.was_soft_invalidated">
 <span class="sig-name descname"><span class="pre">was_soft_invalidated</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">bool</span></span></span><a class="headerlink" href="#dogpile.cache.region.DefaultInvalidationStrategy.was_soft_invalidated" title="Permalink to this definition">¶</a></dt>
 <dd><p>Indicate the region was invalidated in soft mode.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Returns</dt>
+<dt class="field-odd">Returns<span class="colon">:</span></dt>
 <dd class="field-odd"><p>Boolean. True if region was invalidated in soft mode.</p>
 </dd>
 </dl>
 </dd></dl>
 
 </dd></dl>
 
@@ -1103,64 +1111,64 @@
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.region.RegionInvalidationStrategy.is_hard_invalidated">
 <span class="sig-name descname"><span class="pre">is_hard_invalidated</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">timestamp</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">bool</span></span></span><a class="headerlink" href="#dogpile.cache.region.RegionInvalidationStrategy.is_hard_invalidated" title="Permalink to this definition">¶</a></dt>
 <dd><p>Check timestamp to determine if it was hard invalidated.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Returns</dt>
+<dt class="field-odd">Returns<span class="colon">:</span></dt>
 <dd class="field-odd"><p>Boolean. True if <code class="docutils literal notranslate"><span class="pre">timestamp</span></code> is older than
 the last region invalidation time and region is invalidated
 in hard mode.</p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.region.RegionInvalidationStrategy.is_invalidated">
 <span class="sig-name descname"><span class="pre">is_invalidated</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">timestamp</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">bool</span></span></span><a class="headerlink" href="#dogpile.cache.region.RegionInvalidationStrategy.is_invalidated" title="Permalink to this definition">¶</a></dt>
 <dd><p>Check timestamp to determine if it was invalidated.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Returns</dt>
+<dt class="field-odd">Returns<span class="colon">:</span></dt>
 <dd class="field-odd"><p>Boolean. True if <code class="docutils literal notranslate"><span class="pre">timestamp</span></code> is older than
 the last region invalidation time.</p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.region.RegionInvalidationStrategy.is_soft_invalidated">
 <span class="sig-name descname"><span class="pre">is_soft_invalidated</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">timestamp</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">bool</span></span></span><a class="headerlink" href="#dogpile.cache.region.RegionInvalidationStrategy.is_soft_invalidated" title="Permalink to this definition">¶</a></dt>
 <dd><p>Check timestamp to determine if it was soft invalidated.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Returns</dt>
+<dt class="field-odd">Returns<span class="colon">:</span></dt>
 <dd class="field-odd"><p>Boolean. True if <code class="docutils literal notranslate"><span class="pre">timestamp</span></code> is older than
 the last region invalidation time and region is invalidated
 in soft mode.</p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.region.RegionInvalidationStrategy.was_hard_invalidated">
 <span class="sig-name descname"><span class="pre">was_hard_invalidated</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">bool</span></span></span><a class="headerlink" href="#dogpile.cache.region.RegionInvalidationStrategy.was_hard_invalidated" title="Permalink to this definition">¶</a></dt>
 <dd><p>Indicate the region was invalidated in hard mode.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Returns</dt>
+<dt class="field-odd">Returns<span class="colon">:</span></dt>
 <dd class="field-odd"><p>Boolean. True if region was invalidated in hard mode.</p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.region.RegionInvalidationStrategy.was_soft_invalidated">
 <span class="sig-name descname"><span class="pre">was_soft_invalidated</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">bool</span></span></span><a class="headerlink" href="#dogpile.cache.region.RegionInvalidationStrategy.was_soft_invalidated" title="Permalink to this definition">¶</a></dt>
 <dd><p>Indicate the region was invalidated in soft mode.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Returns</dt>
+<dt class="field-odd">Returns<span class="colon">:</span></dt>
 <dd class="field-odd"><p>Boolean. True if region was invalidated in soft mode.</p>
 </dd>
 </dl>
 </dd></dl>
 
 </dd></dl>
 
@@ -1213,57 +1221,57 @@
 <a class="reference internal" href="#dogpile.cache.api.BytesBackend.set_serialized" title="dogpile.cache.api.BytesBackend.set_serialized"><code class="xref py py-meth docutils literal notranslate"><span class="pre">BytesBackend.set_serialized()</span></code></a>,
 <a class="reference internal" href="#dogpile.cache.api.BytesBackend.set_serialized_multi" title="dogpile.cache.api.BytesBackend.set_serialized_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">BytesBackend.set_serialized_multi()</span></code></a>.</p>
 <div class="versionadded">
 <p><span class="versionmodified added">New in version 1.1.</span></p>
 </div>
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.api.BytesBackend.get_serialized">
-<span class="sig-name descname"><span class="pre">get_serialized</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><span class="pre">bytes</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference internal" href="#dogpile.cache.api.NoValue" title="dogpile.cache.api.NoValue"><span class="pre">NoValue</span></a><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#dogpile.cache.api.BytesBackend.get_serialized" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">get_serialized</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">bytes</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference internal" href="#dogpile.cache.api.NoValue" title="dogpile.cache.api.NoValue"><span class="pre">NoValue</span></a></span></span><a class="headerlink" href="#dogpile.cache.api.BytesBackend.get_serialized" title="Permalink to this definition">¶</a></dt>
 <dd><p>Retrieve a serialized value from the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.api.BytesBackend.get_serialized.params.key"></span><strong>key</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.api.BytesBackend.get_serialized.params.key">¶</a> – String key that was passed to the <a class="reference internal" href="#dogpile.cache.region.CacheRegion.get" title="dogpile.cache.region.CacheRegion.get"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get()</span></code></a>
 method, which will also be processed by the “key mangling” function
 if one was present.</p>
 </dd>
-<dt class="field-even">Returns</dt>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>a bytes object, or <a class="reference internal" href="#dogpile.cache.api.NO_VALUE" title="dogpile.cache.api.NO_VALUE"><code class="xref py py-data docutils literal notranslate"><span class="pre">NO_VALUE</span></code></a>
 constant if not present.</p>
 </dd>
 </dl>
 <div class="versionadded">
 <p><span class="versionmodified added">New in version 1.1.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.api.BytesBackend.get_serialized_multi">
-<span class="sig-name descname"><span class="pre">get_serialized_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">keys</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><span class="pre">bytes</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference internal" href="#dogpile.cache.api.NoValue" title="dogpile.cache.api.NoValue"><span class="pre">NoValue</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#dogpile.cache.api.BytesBackend.get_serialized_multi" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">get_serialized_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">keys</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">bytes</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference internal" href="#dogpile.cache.api.NoValue" title="dogpile.cache.api.NoValue"><span class="pre">NoValue</span></a><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#dogpile.cache.api.BytesBackend.get_serialized_multi" title="Permalink to this definition">¶</a></dt>
 <dd><p>Retrieve multiple serialized values from the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.api.BytesBackend.get_serialized_multi.params.keys"></span><strong>keys</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.api.BytesBackend.get_serialized_multi.params.keys">¶</a> – sequence of string keys that was passed to the
 <a class="reference internal" href="#dogpile.cache.region.CacheRegion.get_multi" title="dogpile.cache.region.CacheRegion.get_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get_multi()</span></code></a> method, which will also be processed
 by the “key mangling” function if one was present.</p>
 </dd>
-<dt class="field-even">Returns</dt>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>list of bytes objects</p>
 </dd>
 </dl>
 <div class="versionadded">
 <p><span class="versionmodified added">New in version 1.1.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.api.BytesBackend.set_serialized">
 <span class="sig-name descname"><span class="pre">set_serialized</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">value</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bytes</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#dogpile.cache.api.BytesBackend.set_serialized" title="Permalink to this definition">¶</a></dt>
 <dd><p>Set a serialized value in the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="dogpile.cache.api.BytesBackend.set_serialized.params.key"></span><strong>key</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.api.BytesBackend.set_serialized.params.key">¶</a> – String key that was passed to the <a class="reference internal" href="#dogpile.cache.region.CacheRegion.set" title="dogpile.cache.region.CacheRegion.set"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.set()</span></code></a>
 method, which will also be processed by the “key mangling” function
 if one was present.</p></li>
 <li><p><span class="target" id="dogpile.cache.api.BytesBackend.set_serialized.params.value"></span><strong>value</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.api.BytesBackend.set_serialized.params.value">¶</a> – a bytes object to be stored.</p></li>
 </ul>
 </dd>
@@ -1274,15 +1282,15 @@
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.api.BytesBackend.set_serialized_multi">
 <span class="sig-name descname"><span class="pre">set_serialized_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">mapping</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Mapping</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">bytes</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#dogpile.cache.api.BytesBackend.set_serialized_multi" title="Permalink to this definition">¶</a></dt>
 <dd><p>Set multiple serialized values in the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.api.BytesBackend.set_serialized_multi.params.mapping"></span><strong>mapping</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.api.BytesBackend.set_serialized_multi.params.mapping">¶</a> – a dict in which the key will be whatever was passed to
 the <a class="reference internal" href="#dogpile.cache.region.CacheRegion.set_multi" title="dogpile.cache.region.CacheRegion.set_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.set_multi()</span></code></a> method, processed by the “key
 mangling” function, if any.</p>
 </dd>
 </dl>
 <p>When implementing a new <a class="reference internal" href="#dogpile.cache.api.CacheBackend" title="dogpile.cache.api.CacheBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheBackend</span></code></a> or cutomizing via
 <a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">ProxyBackend</span></code></a>, be aware that when this method is invoked by
@@ -1307,15 +1315,15 @@
 backend.   For backends in which the value that’s stored is ultimately
 a stream of bytes, the <a class="reference internal" href="#dogpile.cache.api.BytesBackend" title="dogpile.cache.api.BytesBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">BytesBackend</span></code></a> should be used.</p>
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.api.CacheBackend.delete">
 <span class="sig-name descname"><span class="pre">delete</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#dogpile.cache.api.CacheBackend.delete" title="Permalink to this definition">¶</a></dt>
 <dd><p>Delete a value from the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.api.CacheBackend.delete.params.key"></span><strong>key</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.api.CacheBackend.delete.params.key">¶</a> – String key that was passed to the
 <a class="reference internal" href="#dogpile.cache.region.CacheRegion.delete" title="dogpile.cache.region.CacheRegion.delete"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.delete()</span></code></a>
 method, which will also be processed by the “key mangling” function
 if one was present.</p>
 </dd>
 </dl>
 <p>The behavior here should be idempotent,
@@ -1325,15 +1333,15 @@
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.api.CacheBackend.delete_multi">
 <span class="sig-name descname"><span class="pre">delete_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">keys</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#dogpile.cache.api.CacheBackend.delete_multi" title="Permalink to this definition">¶</a></dt>
 <dd><p>Delete multiple values from the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.api.CacheBackend.delete_multi.params.keys"></span><strong>keys</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.api.CacheBackend.delete_multi.params.keys">¶</a> – sequence of string keys that was passed to the
 <a class="reference internal" href="#dogpile.cache.region.CacheRegion.delete_multi" title="dogpile.cache.region.CacheRegion.delete_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.delete_multi()</span></code></a> method, which will also be processed
 by the “key mangling” function if one was present.</p>
 </dd>
 </dl>
 <p>The behavior here should be idempotent,
 that is, can be called any number of times
@@ -1342,48 +1350,48 @@
 <div class="versionadded">
 <p><span class="versionmodified added">New in version 0.5.0.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="dogpile.cache.api.CacheBackend.deserializer">
-<span class="sig-name descname"><span class="pre">deserializer</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><span class="pre">None</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="pre">bytes</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></em><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">None</span></em><a class="headerlink" href="#dogpile.cache.api.CacheBackend.deserializer" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">deserializer</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">None</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="pre">bytes</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span></em><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">None</span></em><a class="headerlink" href="#dogpile.cache.api.CacheBackend.deserializer" title="Permalink to this definition">¶</a></dt>
 <dd><p>deserializer function that will be used by default if not overridden
 by the region.</p>
 <div class="versionadded">
 <p><span class="versionmodified added">New in version 1.1.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.api.CacheBackend.get">
-<span class="sig-name descname"><span class="pre">get</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><span class="pre">CachedValue</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference internal" href="#dogpile.cache.api.NoValue" title="dogpile.cache.api.NoValue"><span class="pre">NoValue</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">bytes</span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#dogpile.cache.api.CacheBackend.get" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">get</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><span class="pre">CachedValue</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference internal" href="#dogpile.cache.api.NoValue" title="dogpile.cache.api.NoValue"><span class="pre">NoValue</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">bytes</span></span></span><a class="headerlink" href="#dogpile.cache.api.CacheBackend.get" title="Permalink to this definition">¶</a></dt>
 <dd><p>Retrieve an optionally serialized value from the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.api.CacheBackend.get.params.key"></span><strong>key</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.api.CacheBackend.get.params.key">¶</a> – String key that was passed to the <a class="reference internal" href="#dogpile.cache.region.CacheRegion.get" title="dogpile.cache.region.CacheRegion.get"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get()</span></code></a>
 method, which will also be processed by the “key mangling” function
 if one was present.</p>
 </dd>
-<dt class="field-even">Returns</dt>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>the Python object that corresponds to
 what was established via the <a class="reference internal" href="#dogpile.cache.api.CacheBackend.set" title="dogpile.cache.api.CacheBackend.set"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.set()</span></code></a> method,
 or the <a class="reference internal" href="#dogpile.cache.api.NO_VALUE" title="dogpile.cache.api.NO_VALUE"><code class="xref py py-data docutils literal notranslate"><span class="pre">NO_VALUE</span></code></a> constant if not present.</p>
 </dd>
 </dl>
 <p>If a serializer is in use, this method will only be called if the
 <a class="reference internal" href="#dogpile.cache.api.CacheBackend.get_serialized" title="dogpile.cache.api.CacheBackend.get_serialized"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.get_serialized()</span></code></a> method is not overridden.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.api.CacheBackend.get_multi">
-<span class="sig-name descname"><span class="pre">get_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">keys</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><span class="pre">CachedValue</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference internal" href="#dogpile.cache.api.NoValue" title="dogpile.cache.api.NoValue"><span class="pre">NoValue</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">bytes</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#dogpile.cache.api.CacheBackend.get_multi" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">get_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">keys</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><span class="pre">CachedValue</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference internal" href="#dogpile.cache.api.NoValue" title="dogpile.cache.api.NoValue"><span class="pre">NoValue</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">bytes</span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#dogpile.cache.api.CacheBackend.get_multi" title="Permalink to this definition">¶</a></dt>
 <dd><p>Retrieve multiple optionally serialized values from the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.api.CacheBackend.get_multi.params.keys"></span><strong>keys</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.api.CacheBackend.get_multi.params.keys">¶</a> – sequence of string keys that was passed to the
 <a class="reference internal" href="#dogpile.cache.region.CacheRegion.get_multi" title="dogpile.cache.region.CacheRegion.get_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get_multi()</span></code></a> method, which will also be processed
 by the “key mangling” function if one was present.</p>
 </dd>
 </dl>
 <dl class="simple">
 <dt>:return a list of values as would be returned</dt><dd><p>individually via the <a class="reference internal" href="#dogpile.cache.api.CacheBackend.get" title="dogpile.cache.api.CacheBackend.get"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.get()</span></code></a> method, corresponding
@@ -1395,15 +1403,15 @@
 <div class="versionadded">
 <p><span class="versionmodified added">New in version 0.5.0.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.api.CacheBackend.get_mutex">
-<span class="sig-name descname"><span class="pre">get_mutex</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#dogpile.cache.api.CacheMutex" title="dogpile.cache.api.CacheMutex"><span class="pre">CacheMutex</span></a><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#dogpile.cache.api.CacheBackend.get_mutex" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">get_mutex</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#dogpile.cache.api.CacheMutex" title="dogpile.cache.api.CacheMutex"><span class="pre">CacheMutex</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span></span><a class="headerlink" href="#dogpile.cache.api.CacheBackend.get_mutex" title="Permalink to this definition">¶</a></dt>
 <dd><p>Return an optional mutexing object for the given key.</p>
 <p>This object need only provide an <code class="docutils literal notranslate"><span class="pre">acquire()</span></code>
 and <code class="docutils literal notranslate"><span class="pre">release()</span></code> method.</p>
 <p>May return <code class="docutils literal notranslate"><span class="pre">None</span></code>, in which case the dogpile
 lock will use a regular <code class="docutils literal notranslate"><span class="pre">threading.Lock</span></code>
 object to mutex concurrent threads for
 value creation.   The default implementation
@@ -1424,23 +1432,23 @@
 can be used as a means of throttling the total
 number of value recreation operations that may
 proceed at one time.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.api.CacheBackend.get_serialized">
-<span class="sig-name descname"><span class="pre">get_serialized</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><span class="pre">bytes</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference internal" href="#dogpile.cache.api.NoValue" title="dogpile.cache.api.NoValue"><span class="pre">NoValue</span></a><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#dogpile.cache.api.CacheBackend.get_serialized" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">get_serialized</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">bytes</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference internal" href="#dogpile.cache.api.NoValue" title="dogpile.cache.api.NoValue"><span class="pre">NoValue</span></a></span></span><a class="headerlink" href="#dogpile.cache.api.CacheBackend.get_serialized" title="Permalink to this definition">¶</a></dt>
 <dd><p>Retrieve a serialized value from the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.api.CacheBackend.get_serialized.params.key"></span><strong>key</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.api.CacheBackend.get_serialized.params.key">¶</a> – String key that was passed to the <a class="reference internal" href="#dogpile.cache.region.CacheRegion.get" title="dogpile.cache.region.CacheRegion.get"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get()</span></code></a>
 method, which will also be processed by the “key mangling” function
 if one was present.</p>
 </dd>
-<dt class="field-even">Returns</dt>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>a bytes object, or <a class="reference internal" href="#dogpile.cache.api.NO_VALUE" title="dogpile.cache.api.NO_VALUE"><code class="xref py py-data docutils literal notranslate"><span class="pre">NO_VALUE</span></code></a>
 constant if not present.</p>
 </dd>
 </dl>
 <p>The default implementation of this method for <a class="reference internal" href="#dogpile.cache.api.CacheBackend" title="dogpile.cache.api.CacheBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheBackend</span></code></a>
 returns the value of the <a class="reference internal" href="#dogpile.cache.api.CacheBackend.get" title="dogpile.cache.api.CacheBackend.get"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.get()</span></code></a> method.</p>
 <div class="versionadded">
@@ -1450,23 +1458,23 @@
 <p class="admonition-title">See also</p>
 <p><a class="reference internal" href="#dogpile.cache.api.BytesBackend" title="dogpile.cache.api.BytesBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">BytesBackend</span></code></a></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.api.CacheBackend.get_serialized_multi">
-<span class="sig-name descname"><span class="pre">get_serialized_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">keys</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><span class="pre">bytes</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference internal" href="#dogpile.cache.api.NoValue" title="dogpile.cache.api.NoValue"><span class="pre">NoValue</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#dogpile.cache.api.CacheBackend.get_serialized_multi" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">get_serialized_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">keys</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">bytes</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference internal" href="#dogpile.cache.api.NoValue" title="dogpile.cache.api.NoValue"><span class="pre">NoValue</span></a><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#dogpile.cache.api.CacheBackend.get_serialized_multi" title="Permalink to this definition">¶</a></dt>
 <dd><p>Retrieve multiple serialized values from the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.api.CacheBackend.get_serialized_multi.params.keys"></span><strong>keys</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.api.CacheBackend.get_serialized_multi.params.keys">¶</a> – sequence of string keys that was passed to the
 <a class="reference internal" href="#dogpile.cache.region.CacheRegion.get_multi" title="dogpile.cache.region.CacheRegion.get_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get_multi()</span></code></a> method, which will also be processed
 by the “key mangling” function if one was present.</p>
 </dd>
-<dt class="field-even">Returns</dt>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>list of bytes objects</p>
 </dd>
 </dl>
 <p>The default implementation of this method for <a class="reference internal" href="#dogpile.cache.api.CacheBackend" title="dogpile.cache.api.CacheBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheBackend</span></code></a>
 returns the value of the <a class="reference internal" href="#dogpile.cache.api.CacheBackend.get_multi" title="dogpile.cache.api.CacheBackend.get_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.get_multi()</span></code></a> method.</p>
 <div class="versionadded">
 <p><span class="versionmodified added">New in version 1.1.</span></p>
@@ -1475,36 +1483,36 @@
 <p class="admonition-title">See also</p>
 <p><a class="reference internal" href="#dogpile.cache.api.BytesBackend" title="dogpile.cache.api.BytesBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">BytesBackend</span></code></a></p>
 </div>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="dogpile.cache.api.CacheBackend.key_mangler">
-<span class="sig-name descname"><span class="pre">key_mangler</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></em><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">None</span></em><a class="headerlink" href="#dogpile.cache.api.CacheBackend.key_mangler" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">key_mangler</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></em><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">None</span></em><a class="headerlink" href="#dogpile.cache.api.CacheBackend.key_mangler" title="Permalink to this definition">¶</a></dt>
 <dd><p>Key mangling function.</p>
 <p>May be None, or otherwise declared
 as an ordinary instance method.</p>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="dogpile.cache.api.CacheBackend.serializer">
-<span class="sig-name descname"><span class="pre">serializer</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><span class="pre">None</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">bytes</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></em><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">None</span></em><a class="headerlink" href="#dogpile.cache.api.CacheBackend.serializer" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">serializer</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">None</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">bytes</span><span class="p"><span class="pre">]</span></span></em><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">None</span></em><a class="headerlink" href="#dogpile.cache.api.CacheBackend.serializer" title="Permalink to this definition">¶</a></dt>
 <dd><p>Serializer function that will be used by default if not overridden
 by the region.</p>
 <div class="versionadded">
 <p><span class="versionmodified added">New in version 1.1.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.api.CacheBackend.set">
-<span class="sig-name descname"><span class="pre">set</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">value</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><span class="pre">CachedValue</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">bytes</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#dogpile.cache.api.CacheBackend.set" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">set</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">value</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><span class="pre">CachedValue</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">bytes</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#dogpile.cache.api.CacheBackend.set" title="Permalink to this definition">¶</a></dt>
 <dd><p>Set an optionally serialized value in the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="dogpile.cache.api.CacheBackend.set.params.key"></span><strong>key</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.api.CacheBackend.set.params.key">¶</a> – String key that was passed to the <a class="reference internal" href="#dogpile.cache.region.CacheRegion.set" title="dogpile.cache.region.CacheRegion.set"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.set()</span></code></a>
 method, which will also be processed by the “key mangling” function
 if one was present.</p></li>
 <li><p><span class="target" id="dogpile.cache.api.CacheBackend.set.params.value"></span><strong>value</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.api.CacheBackend.set.params.value">¶</a> – The optionally serialized <a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><code class="xref py py-class docutils literal notranslate"><span class="pre">CachedValue</span></code></a> object.
 May be an instance of <a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><code class="xref py py-class docutils literal notranslate"><span class="pre">CachedValue</span></code></a> or a bytes object
 depending on if a serializer is in use with the region and if the
@@ -1516,18 +1524,18 @@
 <p class="admonition-title">See also</p>
 <p><a class="reference internal" href="#dogpile.cache.api.CacheBackend.set_serialized" title="dogpile.cache.api.CacheBackend.set_serialized"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.set_serialized()</span></code></a></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.api.CacheBackend.set_multi">
-<span class="sig-name descname"><span class="pre">set_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">mapping</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Mapping</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><span class="pre">CachedValue</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">bytes</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#dogpile.cache.api.CacheBackend.set_multi" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">set_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">mapping</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Mapping</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><span class="pre">CachedValue</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">bytes</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#dogpile.cache.api.CacheBackend.set_multi" title="Permalink to this definition">¶</a></dt>
 <dd><p>Set multiple values in the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.api.CacheBackend.set_multi.params.mapping"></span><strong>mapping</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.api.CacheBackend.set_multi.params.mapping">¶</a> – a dict in which the key will be whatever was passed to
 the <a class="reference internal" href="#dogpile.cache.region.CacheRegion.set_multi" title="dogpile.cache.region.CacheRegion.set_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.set_multi()</span></code></a> method, processed by the “key
 mangling” function, if any.</p>
 </dd>
 </dl>
 <p>When implementing a new <a class="reference internal" href="#dogpile.cache.api.CacheBackend" title="dogpile.cache.api.CacheBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheBackend</span></code></a> or cutomizing via
 <a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">ProxyBackend</span></code></a>, be aware that when this method is invoked by
@@ -1544,15 +1552,15 @@
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.api.CacheBackend.set_serialized">
 <span class="sig-name descname"><span class="pre">set_serialized</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">value</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bytes</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#dogpile.cache.api.CacheBackend.set_serialized" title="Permalink to this definition">¶</a></dt>
 <dd><p>Set a serialized value in the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="dogpile.cache.api.CacheBackend.set_serialized.params.key"></span><strong>key</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.api.CacheBackend.set_serialized.params.key">¶</a> – String key that was passed to the <a class="reference internal" href="#dogpile.cache.region.CacheRegion.set" title="dogpile.cache.region.CacheRegion.set"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.set()</span></code></a>
 method, which will also be processed by the “key mangling” function
 if one was present.</p></li>
 <li><p><span class="target" id="dogpile.cache.api.CacheBackend.set_serialized.params.value"></span><strong>value</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.api.CacheBackend.set_serialized.params.value">¶</a> – a bytes object to be stored.</p></li>
 </ul>
 </dd>
@@ -1569,15 +1577,15 @@
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.api.CacheBackend.set_serialized_multi">
 <span class="sig-name descname"><span class="pre">set_serialized_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">mapping</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Mapping</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">bytes</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#dogpile.cache.api.CacheBackend.set_serialized_multi" title="Permalink to this definition">¶</a></dt>
 <dd><p>Set multiple serialized values in the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.api.CacheBackend.set_serialized_multi.params.mapping"></span><strong>mapping</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.api.CacheBackend.set_serialized_multi.params.mapping">¶</a> – a dict in which the key will be whatever was passed to
 the <a class="reference internal" href="#dogpile.cache.region.CacheRegion.set_multi" title="dogpile.cache.region.CacheRegion.set_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.set_multi()</span></code></a> method, processed by the “key
 mangling” function, if any.</p>
 </dd>
 </dl>
 <p>When implementing a new <a class="reference internal" href="#dogpile.cache.api.CacheBackend" title="dogpile.cache.api.CacheBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheBackend</span></code></a> or cutomizing via
 <a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">ProxyBackend</span></code></a>, be aware that when this method is invoked by
@@ -1615,30 +1623,30 @@
 returns this locking object.</p>
 </div>
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.api.CacheMutex.acquire">
 <em class="property"><span class="pre">abstract</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">acquire</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">wait</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">True</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">bool</span></span></span><a class="headerlink" href="#dogpile.cache.api.CacheMutex.acquire" title="Permalink to this definition">¶</a></dt>
 <dd><p>Acquire the mutex.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.api.CacheMutex.acquire.params.wait"></span><strong>wait</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.api.CacheMutex.acquire.params.wait">¶</a> – if True, block until available, else return True/False
 immediately.</p>
 </dd>
-<dt class="field-even">Returns</dt>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>True if the lock succeeded.</p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.api.CacheMutex.locked">
 <em class="property"><span class="pre">abstract</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">locked</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">bool</span></span></span><a class="headerlink" href="#dogpile.cache.api.CacheMutex.locked" title="Permalink to this definition">¶</a></dt>
 <dd><p>Check if the mutex was acquired.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Returns</dt>
+<dt class="field-odd">Returns<span class="colon">:</span></dt>
 <dd class="field-odd"><p>true if the lock is acquired.</p>
 </dd>
 </dl>
 <div class="versionadded">
 <p><span class="versionmodified added">New in version 1.1.2.</span></p>
 </div>
 </dd></dl>
@@ -1678,14 +1686,25 @@
 <dt class="sig sig-object py" id="dogpile.cache.api.CachedValue.payload">
 <span class="sig-name descname"><span class="pre">payload</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">Any</span></em><a class="headerlink" href="#dogpile.cache.api.CachedValue.payload" title="Permalink to this definition">¶</a></dt>
 <dd><p>Alias for field number 0</p>
 </dd></dl>
 
 </dd></dl>
 
+<dl class="py exception">
+<dt class="sig sig-object py" id="dogpile.cache.api.CantDeserializeException">
+<em class="property"><span class="pre">exception</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">dogpile.cache.api.</span></span><span class="sig-name descname"><span class="pre">CantDeserializeException</span></span><a class="headerlink" href="#dogpile.cache.api.CantDeserializeException" title="Permalink to this definition">¶</a></dt>
+<dd><p>Bases: <code class="xref py py-class docutils literal notranslate"><span class="pre">Exception</span></code></p>
+<p>Exception indicating deserialization failed, and that caching
+should proceed to re-generate a value</p>
+<div class="versionadded">
+<p><span class="versionmodified added">New in version 1.2.0.</span></p>
+</div>
+</dd></dl>
+
 <dl class="py attribute">
 <dt class="sig sig-object py" id="dogpile.cache.api.KeyType">
 <span class="sig-prename descclassname"><span class="pre">dogpile.cache.api.</span></span><span class="sig-name descname"><span class="pre">KeyType</span></span><a class="headerlink" href="#dogpile.cache.api.KeyType" title="Permalink to this definition">¶</a></dt>
 <dd><p>A cache key.</p>
 </dd></dl>
 
 <dl class="py data">
@@ -1721,14 +1740,15 @@
 <span id="backends"></span><h2>Backends<a class="headerlink" href="#module-dogpile.cache.backends.memory" title="Permalink to this heading">¶</a></h2>
 <section id="memory-backends">
 <h3>Memory Backends<a class="headerlink" href="#memory-backends" title="Permalink to this heading">¶</a></h3>
 <p>Provides simple dictionary-based backends.</p>
 <p>The two backends are <a class="reference internal" href="#dogpile.cache.backends.memory.MemoryBackend" title="dogpile.cache.backends.memory.MemoryBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">MemoryBackend</span></code></a> and <a class="reference internal" href="#dogpile.cache.backends.memory.MemoryPickleBackend" title="dogpile.cache.backends.memory.MemoryPickleBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">MemoryPickleBackend</span></code></a>;
 the latter applies a serialization step to cached values while the former
 places the value as given into the dictionary.</p>
+</section>
 <dl class="py class">
 <dt class="sig sig-object py" id="dogpile.cache.backends.memory.MemoryBackend">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">dogpile.cache.backends.memory.</span></span><span class="sig-name descname"><span class="pre">MemoryBackend</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">arguments</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.memory.MemoryBackend" title="Permalink to this definition">¶</a></dt>
 <dd><p>Bases: <a class="reference internal" href="#dogpile.cache.api.CacheBackend" title="dogpile.cache.api.CacheBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheBackend</span></code></a></p>
 <p>A backend that uses a plain dictionary.</p>
 <p>There is no size management, and values which
 are placed into the dictionary will remain
@@ -1757,15 +1777,15 @@
 </pre></div>
 </div>
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.memory.MemoryBackend.delete">
 <span class="sig-name descname"><span class="pre">delete</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.memory.MemoryBackend.delete" title="Permalink to this definition">¶</a></dt>
 <dd><p>Delete a value from the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.backends.memory.MemoryBackend.delete.params.key"></span><strong>key</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.memory.MemoryBackend.delete.params.key">¶</a> – String key that was passed to the
 <a class="reference internal" href="#dogpile.cache.region.CacheRegion.delete" title="dogpile.cache.region.CacheRegion.delete"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.delete()</span></code></a>
 method, which will also be processed by the “key mangling” function
 if one was present.</p>
 </dd>
 </dl>
 <p>The behavior here should be idempotent,
@@ -1775,15 +1795,15 @@
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.memory.MemoryBackend.delete_multi">
 <span class="sig-name descname"><span class="pre">delete_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">keys</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.memory.MemoryBackend.delete_multi" title="Permalink to this definition">¶</a></dt>
 <dd><p>Delete multiple values from the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.backends.memory.MemoryBackend.delete_multi.params.keys"></span><strong>keys</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.memory.MemoryBackend.delete_multi.params.keys">¶</a> – sequence of string keys that was passed to the
 <a class="reference internal" href="#dogpile.cache.region.CacheRegion.delete_multi" title="dogpile.cache.region.CacheRegion.delete_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.delete_multi()</span></code></a> method, which will also be processed
 by the “key mangling” function if one was present.</p>
 </dd>
 </dl>
 <p>The behavior here should be idempotent,
 that is, can be called any number of times
@@ -1795,35 +1815,35 @@
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.memory.MemoryBackend.get">
 <span class="sig-name descname"><span class="pre">get</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.memory.MemoryBackend.get" title="Permalink to this definition">¶</a></dt>
 <dd><p>Retrieve an optionally serialized value from the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.backends.memory.MemoryBackend.get.params.key"></span><strong>key</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.memory.MemoryBackend.get.params.key">¶</a> – String key that was passed to the <a class="reference internal" href="#dogpile.cache.region.CacheRegion.get" title="dogpile.cache.region.CacheRegion.get"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get()</span></code></a>
 method, which will also be processed by the “key mangling” function
 if one was present.</p>
 </dd>
-<dt class="field-even">Returns</dt>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>the Python object that corresponds to
 what was established via the <a class="reference internal" href="#dogpile.cache.api.CacheBackend.set" title="dogpile.cache.api.CacheBackend.set"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.set()</span></code></a> method,
 or the <a class="reference internal" href="#dogpile.cache.api.NO_VALUE" title="dogpile.cache.api.NO_VALUE"><code class="xref py py-data docutils literal notranslate"><span class="pre">NO_VALUE</span></code></a> constant if not present.</p>
 </dd>
 </dl>
 <p>If a serializer is in use, this method will only be called if the
 <a class="reference internal" href="#dogpile.cache.api.CacheBackend.get_serialized" title="dogpile.cache.api.CacheBackend.get_serialized"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.get_serialized()</span></code></a> method is not overridden.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.memory.MemoryBackend.get_multi">
 <span class="sig-name descname"><span class="pre">get_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">keys</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.memory.MemoryBackend.get_multi" title="Permalink to this definition">¶</a></dt>
 <dd><p>Retrieve multiple optionally serialized values from the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.backends.memory.MemoryBackend.get_multi.params.keys"></span><strong>keys</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.memory.MemoryBackend.get_multi.params.keys">¶</a> – sequence of string keys that was passed to the
 <a class="reference internal" href="#dogpile.cache.region.CacheRegion.get_multi" title="dogpile.cache.region.CacheRegion.get_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get_multi()</span></code></a> method, which will also be processed
 by the “key mangling” function if one was present.</p>
 </dd>
 </dl>
 <dl class="simple">
 <dt>:return a list of values as would be returned</dt><dd><p>individually via the <a class="reference internal" href="#dogpile.cache.api.CacheBackend.get" title="dogpile.cache.api.CacheBackend.get"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.get()</span></code></a> method, corresponding
@@ -1838,15 +1858,15 @@
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.memory.MemoryBackend.set">
 <span class="sig-name descname"><span class="pre">set</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">value</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.memory.MemoryBackend.set" title="Permalink to this definition">¶</a></dt>
 <dd><p>Set an optionally serialized value in the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="dogpile.cache.backends.memory.MemoryBackend.set.params.key"></span><strong>key</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.memory.MemoryBackend.set.params.key">¶</a> – String key that was passed to the <a class="reference internal" href="#dogpile.cache.region.CacheRegion.set" title="dogpile.cache.region.CacheRegion.set"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.set()</span></code></a>
 method, which will also be processed by the “key mangling” function
 if one was present.</p></li>
 <li><p><span class="target" id="dogpile.cache.backends.memory.MemoryBackend.set.params.value"></span><strong>value</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.memory.MemoryBackend.set.params.value">¶</a> – The optionally serialized <a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><code class="xref py py-class docutils literal notranslate"><span class="pre">CachedValue</span></code></a> object.
 May be an instance of <a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><code class="xref py py-class docutils literal notranslate"><span class="pre">CachedValue</span></code></a> or a bytes object
 depending on if a serializer is in use with the region and if the
@@ -1861,15 +1881,15 @@
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.memory.MemoryBackend.set_multi">
 <span class="sig-name descname"><span class="pre">set_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">mapping</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.memory.MemoryBackend.set_multi" title="Permalink to this definition">¶</a></dt>
 <dd><p>Set multiple values in the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.backends.memory.MemoryBackend.set_multi.params.mapping"></span><strong>mapping</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.memory.MemoryBackend.set_multi.params.mapping">¶</a> – a dict in which the key will be whatever was passed to
 the <a class="reference internal" href="#dogpile.cache.region.CacheRegion.set_multi" title="dogpile.cache.region.CacheRegion.set_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.set_multi()</span></code></a> method, processed by the “key
 mangling” function, if any.</p>
 </dd>
 </dl>
 <p>When implementing a new <a class="reference internal" href="#dogpile.cache.api.CacheBackend" title="dogpile.cache.api.CacheBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheBackend</span></code></a> or cutomizing via
 <a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">ProxyBackend</span></code></a>, be aware that when this method is invoked by
@@ -1915,18 +1935,18 @@
 either <code class="docutils literal notranslate"><span class="pre">cPickle</span></code> or <code class="docutils literal notranslate"><span class="pre">pickle</span></code> and specifying <code class="docutils literal notranslate"><span class="pre">HIGHEST_PROTOCOL</span></code>
 upon serialize.</p>
 <div class="versionadded">
 <p><span class="versionmodified added">New in version 0.5.3.</span></p>
 </div>
 </dd></dl>
 
-</section>
 <span class="target" id="module-dogpile.cache.backends.memcached"></span><section id="memcached-backends">
 <h3>Memcached Backends<a class="headerlink" href="#memcached-backends" title="Permalink to this heading">¶</a></h3>
 <p>Provides backends for talking to <a class="reference external" href="http://memcached.org">memcached</a>.</p>
+</section>
 <dl class="py class">
 <dt class="sig sig-object py" id="dogpile.cache.backends.memcached.BMemcachedBackend">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">dogpile.cache.backends.memcached.</span></span><span class="sig-name descname"><span class="pre">BMemcachedBackend</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">arguments</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.memcached.BMemcachedBackend" title="Permalink to this definition">¶</a></dt>
 <dd><p>Bases: <a class="reference internal" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend" title="dogpile.cache.backends.memcached.GenericMemcachedBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">GenericMemcachedBackend</span></code></a></p>
 <p>A backend for the
 <a class="reference external" href="https://github.com/jaysonsantos/python-binary-memcached">python-binary-memcached</a>
 memcached client.</p>
@@ -1965,15 +1985,15 @@
 </pre></div>
 </div>
 <p>For advanced ways to configure TLS creating a more complex
 tls_context visit <a class="reference external" href="https://docs.python.org/3/library/ssl.html">https://docs.python.org/3/library/ssl.html</a></p>
 <p>Arguments which can be passed to the <code class="docutils literal notranslate"><span class="pre">arguments</span></code>
 dictionary include:</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="dogpile.cache.backends.memcached.BMemcachedBackend.params.username"></span><strong>username</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.memcached.BMemcachedBackend.params.username">¶</a> – optional username, will be used for
 SASL authentication.</p></li>
 <li><p><span class="target" id="dogpile.cache.backends.memcached.BMemcachedBackend.params.password"></span><strong>password</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.memcached.BMemcachedBackend.params.password">¶</a> – optional password, will be used for
 SASL authentication.</p></li>
 <li><p><span class="target" id="dogpile.cache.backends.memcached.BMemcachedBackend.params.tls_context"></span><strong>tls_context</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.memcached.BMemcachedBackend.params.tls_context">¶</a> – <p>optional TLS context, will be used for
 TLS connections.</p>
@@ -1996,15 +2016,15 @@
 <dt class="sig sig-object py" id="dogpile.cache.backends.memcached.GenericMemcachedBackend">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">dogpile.cache.backends.memcached.</span></span><span class="sig-name descname"><span class="pre">GenericMemcachedBackend</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">arguments</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend" title="Permalink to this definition">¶</a></dt>
 <dd><p>Bases: <a class="reference internal" href="#dogpile.cache.api.CacheBackend" title="dogpile.cache.api.CacheBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheBackend</span></code></a></p>
 <p>Base class for memcached backends.</p>
 <p>This base class accepts a number of paramters
 common to all backends.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="dogpile.cache.backends.memcached.GenericMemcachedBackend.params.url"></span><strong>url</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend.params.url">¶</a> – the string URL to connect to.  Can be a single
 string or a list of strings.  This is the only argument
 that’s required.</p></li>
 <li><p><span class="target" id="dogpile.cache.backends.memcached.GenericMemcachedBackend.params.distributed_lock"></span><strong>distributed_lock</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend.params.distributed_lock">¶</a> – boolean, when True, will use a
 memcached-lock as the dogpile lock (see <a class="reference internal" href="#dogpile.cache.backends.memcached.MemcachedLock" title="dogpile.cache.backends.memcached.MemcachedLock"><code class="xref py py-class docutils literal notranslate"><span class="pre">MemcachedLock</span></code></a>).
 Use this when multiple
@@ -2059,15 +2079,15 @@
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.memcached.GenericMemcachedBackend.delete">
 <span class="sig-name descname"><span class="pre">delete</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend.delete" title="Permalink to this definition">¶</a></dt>
 <dd><p>Delete a value from the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.backends.memcached.GenericMemcachedBackend.delete.params.key"></span><strong>key</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend.delete.params.key">¶</a> – String key that was passed to the
 <a class="reference internal" href="#dogpile.cache.region.CacheRegion.delete" title="dogpile.cache.region.CacheRegion.delete"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.delete()</span></code></a>
 method, which will also be processed by the “key mangling” function
 if one was present.</p>
 </dd>
 </dl>
 <p>The behavior here should be idempotent,
@@ -2077,15 +2097,15 @@
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.memcached.GenericMemcachedBackend.delete_multi">
 <span class="sig-name descname"><span class="pre">delete_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">keys</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend.delete_multi" title="Permalink to this definition">¶</a></dt>
 <dd><p>Delete multiple values from the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.backends.memcached.GenericMemcachedBackend.delete_multi.params.keys"></span><strong>keys</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend.delete_multi.params.keys">¶</a> – sequence of string keys that was passed to the
 <a class="reference internal" href="#dogpile.cache.region.CacheRegion.delete_multi" title="dogpile.cache.region.CacheRegion.delete_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.delete_multi()</span></code></a> method, which will also be processed
 by the “key mangling” function if one was present.</p>
 </dd>
 </dl>
 <p>The behavior here should be idempotent,
 that is, can be called any number of times
@@ -2094,48 +2114,48 @@
 <div class="versionadded">
 <p><span class="versionmodified added">New in version 0.5.0.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="dogpile.cache.backends.memcached.GenericMemcachedBackend.deserializer">
-<span class="sig-name descname"><span class="pre">deserializer</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><span class="pre">None</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Deserializer</span><span class="p"><span class="pre">]</span></span></em><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">None</span></em><a class="headerlink" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend.deserializer" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">deserializer</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">None</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">Deserializer</span></em><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">None</span></em><a class="headerlink" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend.deserializer" title="Permalink to this definition">¶</a></dt>
 <dd><p>deserializer function that will be used by default if not overridden
 by the region.</p>
 <div class="versionadded">
 <p><span class="versionmodified added">New in version 1.1.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.memcached.GenericMemcachedBackend.get">
 <span class="sig-name descname"><span class="pre">get</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend.get" title="Permalink to this definition">¶</a></dt>
 <dd><p>Retrieve an optionally serialized value from the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.backends.memcached.GenericMemcachedBackend.get.params.key"></span><strong>key</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend.get.params.key">¶</a> – String key that was passed to the <a class="reference internal" href="#dogpile.cache.region.CacheRegion.get" title="dogpile.cache.region.CacheRegion.get"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get()</span></code></a>
 method, which will also be processed by the “key mangling” function
 if one was present.</p>
 </dd>
-<dt class="field-even">Returns</dt>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>the Python object that corresponds to
 what was established via the <a class="reference internal" href="#dogpile.cache.api.CacheBackend.set" title="dogpile.cache.api.CacheBackend.set"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.set()</span></code></a> method,
 or the <a class="reference internal" href="#dogpile.cache.api.NO_VALUE" title="dogpile.cache.api.NO_VALUE"><code class="xref py py-data docutils literal notranslate"><span class="pre">NO_VALUE</span></code></a> constant if not present.</p>
 </dd>
 </dl>
 <p>If a serializer is in use, this method will only be called if the
 <a class="reference internal" href="#dogpile.cache.api.CacheBackend.get_serialized" title="dogpile.cache.api.CacheBackend.get_serialized"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.get_serialized()</span></code></a> method is not overridden.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.memcached.GenericMemcachedBackend.get_multi">
 <span class="sig-name descname"><span class="pre">get_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">keys</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend.get_multi" title="Permalink to this definition">¶</a></dt>
 <dd><p>Retrieve multiple optionally serialized values from the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.backends.memcached.GenericMemcachedBackend.get_multi.params.keys"></span><strong>keys</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend.get_multi.params.keys">¶</a> – sequence of string keys that was passed to the
 <a class="reference internal" href="#dogpile.cache.region.CacheRegion.get_multi" title="dogpile.cache.region.CacheRegion.get_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get_multi()</span></code></a> method, which will also be processed
 by the “key mangling” function if one was present.</p>
 </dd>
 </dl>
 <dl class="simple">
 <dt>:return a list of values as would be returned</dt><dd><p>individually via the <a class="reference internal" href="#dogpile.cache.api.CacheBackend.get" title="dogpile.cache.api.CacheBackend.get"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.get()</span></code></a> method, corresponding
@@ -2176,28 +2196,28 @@
 can be used as a means of throttling the total
 number of value recreation operations that may
 proceed at one time.</p>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="dogpile.cache.backends.memcached.GenericMemcachedBackend.serializer">
-<span class="sig-name descname"><span class="pre">serializer</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><span class="pre">None</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Serializer</span><span class="p"><span class="pre">]</span></span></em><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">None</span></em><a class="headerlink" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend.serializer" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">serializer</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">None</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">Serializer</span></em><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">None</span></em><a class="headerlink" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend.serializer" title="Permalink to this definition">¶</a></dt>
 <dd><p>Serializer function that will be used by default if not overridden
 by the region.</p>
 <div class="versionadded">
 <p><span class="versionmodified added">New in version 1.1.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.memcached.GenericMemcachedBackend.set">
 <span class="sig-name descname"><span class="pre">set</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">value</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend.set" title="Permalink to this definition">¶</a></dt>
 <dd><p>Set an optionally serialized value in the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="dogpile.cache.backends.memcached.GenericMemcachedBackend.set.params.key"></span><strong>key</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend.set.params.key">¶</a> – String key that was passed to the <a class="reference internal" href="#dogpile.cache.region.CacheRegion.set" title="dogpile.cache.region.CacheRegion.set"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.set()</span></code></a>
 method, which will also be processed by the “key mangling” function
 if one was present.</p></li>
 <li><p><span class="target" id="dogpile.cache.backends.memcached.GenericMemcachedBackend.set.params.value"></span><strong>value</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend.set.params.value">¶</a> – The optionally serialized <a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><code class="xref py py-class docutils literal notranslate"><span class="pre">CachedValue</span></code></a> object.
 May be an instance of <a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><code class="xref py py-class docutils literal notranslate"><span class="pre">CachedValue</span></code></a> or a bytes object
 depending on if a serializer is in use with the region and if the
@@ -2219,15 +2239,15 @@
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.memcached.GenericMemcachedBackend.set_multi">
 <span class="sig-name descname"><span class="pre">set_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">mapping</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend.set_multi" title="Permalink to this definition">¶</a></dt>
 <dd><p>Set multiple values in the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.backends.memcached.GenericMemcachedBackend.set_multi.params.mapping"></span><strong>mapping</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend.set_multi.params.mapping">¶</a> – a dict in which the key will be whatever was passed to
 the <a class="reference internal" href="#dogpile.cache.region.CacheRegion.set_multi" title="dogpile.cache.region.CacheRegion.set_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.set_multi()</span></code></a> method, processed by the “key
 mangling” function, if any.</p>
 </dd>
 </dl>
 <p>When implementing a new <a class="reference internal" href="#dogpile.cache.api.CacheBackend" title="dogpile.cache.api.CacheBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheBackend</span></code></a> or cutomizing via
 <a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">ProxyBackend</span></code></a>, be aware that when this method is invoked by
@@ -2261,15 +2281,15 @@
     <span class="n">arguments</span> <span class="o">=</span> <span class="p">{</span>
         <span class="s1">&#39;url&#39;</span><span class="p">:</span><span class="s2">&quot;127.0.0.1:11211&quot;</span>
     <span class="p">}</span>
 <span class="p">)</span>
 </pre></div>
 </div>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="dogpile.cache.backends.memcached.MemcachedBackend.params.dead_retry"></span><strong>dead_retry</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.memcached.MemcachedBackend.params.dead_retry">¶</a> – <p>Number of seconds memcached server is considered dead
 before it is tried again. Will be passed to <code class="docutils literal notranslate"><span class="pre">memcache.Client</span></code>
 as the <code class="docutils literal notranslate"><span class="pre">dead_retry</span></code> parameter.</p>
 <div class="versionchanged">
 <p><span class="versionmodified changed">Changed in version 1.1.8: </span>Moved the <code class="docutils literal notranslate"><span class="pre">dead_retry</span></code> argument which was
 erroneously added to “set_parameters” to
@@ -2321,15 +2341,15 @@
 <p>dogpile.cache uses the <code class="docutils literal notranslate"><span class="pre">HashClient</span></code> from pymemcache in order to reduce
 API differences when compared to other memcached client drivers.
 This allows the user to provide a single server or a list of memcached
 servers.</p>
 <p>Arguments which can be passed to the <code class="docutils literal notranslate"><span class="pre">arguments</span></code>
 dictionary include:</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="dogpile.cache.backends.memcached.PyMemcacheBackend.params.tls_context"></span><strong>tls_context</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.memcached.PyMemcacheBackend.params.tls_context">¶</a> – <p>optional TLS context, will be used for
 TLS connections.</p>
 <p>A typical configuration using tls_context:</p>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="kn">import</span> <span class="nn">ssl</span>
 <span class="kn">from</span> <span class="nn">dogpile.cache</span> <span class="kn">import</span> <span class="n">make_region</span>
 
@@ -2474,32 +2494,32 @@
 <span class="p">)</span>
 </pre></div>
 </div>
 <p>Arguments accepted here include those of
 <a class="reference internal" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend" title="dogpile.cache.backends.memcached.GenericMemcachedBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">GenericMemcachedBackend</span></code></a>, as well as
 those below.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="dogpile.cache.backends.memcached.PylibmcBackend.params.binary"></span><strong>binary</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.memcached.PylibmcBackend.params.binary">¶</a> – sets the <code class="docutils literal notranslate"><span class="pre">binary</span></code> flag understood by
 <code class="docutils literal notranslate"><span class="pre">pylibmc.Client</span></code>.</p></li>
 <li><p><span class="target" id="dogpile.cache.backends.memcached.PylibmcBackend.params.behaviors"></span><strong>behaviors</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.memcached.PylibmcBackend.params.behaviors">¶</a> – a dictionary which will be passed to
 <code class="docutils literal notranslate"><span class="pre">pylibmc.Client</span></code> as the <code class="docutils literal notranslate"><span class="pre">behaviors</span></code> parameter.</p></li>
 <li><p><span class="target" id="dogpile.cache.backends.memcached.PylibmcBackend.params.min_compress_len"></span><strong>min_compress_len</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.memcached.PylibmcBackend.params.min_compress_len">¶</a> – Integer, will be passed as the
 <code class="docutils literal notranslate"><span class="pre">min_compress_len</span></code> parameter to the <code class="docutils literal notranslate"><span class="pre">pylibmc.Client.set</span></code>
 method.</p></li>
 </ul>
 </dd>
 </dl>
 </dd></dl>
 
-</section>
 <span class="target" id="module-dogpile.cache.backends.redis"></span><section id="redis-backends">
 <h3>Redis Backends<a class="headerlink" href="#redis-backends" title="Permalink to this heading">¶</a></h3>
 <p>Provides backends for talking to <a class="reference external" href="http://redis.io">Redis</a>.</p>
+</section>
 <dl class="py class">
 <dt class="sig sig-object py" id="dogpile.cache.backends.redis.RedisBackend">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">dogpile.cache.backends.redis.</span></span><span class="sig-name descname"><span class="pre">RedisBackend</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">arguments</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.redis.RedisBackend" title="Permalink to this definition">¶</a></dt>
 <dd><p>Bases: <a class="reference internal" href="#dogpile.cache.api.BytesBackend" title="dogpile.cache.api.BytesBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">BytesBackend</span></code></a></p>
 <p>A <a class="reference external" href="http://redis.io/">Redis</a> backend, using the
 <a class="reference external" href="http://pypi.python.org/pypi/redis/">redis-py</a> backend.</p>
 <p>Example configuration:</p>
@@ -2516,15 +2536,15 @@
         <span class="s1">&#39;thread_local_lock&#39;</span><span class="p">:</span> <span class="kc">False</span>
         <span class="p">}</span>
 <span class="p">)</span>
 </pre></div>
 </div>
 <p>Arguments accepted in the arguments dictionary:</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="dogpile.cache.backends.redis.RedisBackend.params.url"></span><strong>url</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.redis.RedisBackend.params.url">¶</a> – string. If provided, will override separate host/port/db
 params.  The format is that accepted by <code class="docutils literal notranslate"><span class="pre">StrictRedis.from_url()</span></code>.</p></li>
 <li><p><span class="target" id="dogpile.cache.backends.redis.RedisBackend.params.host"></span><strong>host</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.redis.RedisBackend.params.host">¶</a> – string, default is <code class="docutils literal notranslate"><span class="pre">localhost</span></code>.</p></li>
 <li><p><span class="target" id="dogpile.cache.backends.redis.RedisBackend.params.password"></span><strong>password</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.redis.RedisBackend.params.password">¶</a> – string, default is no password.</p></li>
 <li><p><span class="target" id="dogpile.cache.backends.redis.RedisBackend.params.port"></span><strong>port</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.redis.RedisBackend.params.port">¶</a> – integer, default is <code class="docutils literal notranslate"><span class="pre">6379</span></code>.</p></li>
 <li><p><span class="target" id="dogpile.cache.backends.redis.RedisBackend.params.db"></span><strong>db</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.redis.RedisBackend.params.db">¶</a> – integer, default is <code class="docutils literal notranslate"><span class="pre">0</span></code>.</p></li>
@@ -2565,15 +2585,15 @@
 </dd>
 </dl>
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.redis.RedisBackend.delete">
 <span class="sig-name descname"><span class="pre">delete</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.redis.RedisBackend.delete" title="Permalink to this definition">¶</a></dt>
 <dd><p>Delete a value from the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.backends.redis.RedisBackend.delete.params.key"></span><strong>key</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.redis.RedisBackend.delete.params.key">¶</a> – String key that was passed to the
 <a class="reference internal" href="#dogpile.cache.region.CacheRegion.delete" title="dogpile.cache.region.CacheRegion.delete"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.delete()</span></code></a>
 method, which will also be processed by the “key mangling” function
 if one was present.</p>
 </dd>
 </dl>
 <p>The behavior here should be idempotent,
@@ -2583,15 +2603,15 @@
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.redis.RedisBackend.delete_multi">
 <span class="sig-name descname"><span class="pre">delete_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">keys</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.redis.RedisBackend.delete_multi" title="Permalink to this definition">¶</a></dt>
 <dd><p>Delete multiple values from the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.backends.redis.RedisBackend.delete_multi.params.keys"></span><strong>keys</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.redis.RedisBackend.delete_multi.params.keys">¶</a> – sequence of string keys that was passed to the
 <a class="reference internal" href="#dogpile.cache.region.CacheRegion.delete_multi" title="dogpile.cache.region.CacheRegion.delete_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.delete_multi()</span></code></a> method, which will also be processed
 by the “key mangling” function if one was present.</p>
 </dd>
 </dl>
 <p>The behavior here should be idempotent,
 that is, can be called any number of times
@@ -2632,54 +2652,54 @@
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.redis.RedisBackend.get_serialized">
 <span class="sig-name descname"><span class="pre">get_serialized</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.redis.RedisBackend.get_serialized" title="Permalink to this definition">¶</a></dt>
 <dd><p>Retrieve a serialized value from the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.backends.redis.RedisBackend.get_serialized.params.key"></span><strong>key</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.redis.RedisBackend.get_serialized.params.key">¶</a> – String key that was passed to the <a class="reference internal" href="#dogpile.cache.region.CacheRegion.get" title="dogpile.cache.region.CacheRegion.get"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get()</span></code></a>
 method, which will also be processed by the “key mangling” function
 if one was present.</p>
 </dd>
-<dt class="field-even">Returns</dt>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>a bytes object, or <a class="reference internal" href="#dogpile.cache.api.NO_VALUE" title="dogpile.cache.api.NO_VALUE"><code class="xref py py-data docutils literal notranslate"><span class="pre">NO_VALUE</span></code></a>
 constant if not present.</p>
 </dd>
 </dl>
 <div class="versionadded">
 <p><span class="versionmodified added">New in version 1.1.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.redis.RedisBackend.get_serialized_multi">
 <span class="sig-name descname"><span class="pre">get_serialized_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">keys</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.redis.RedisBackend.get_serialized_multi" title="Permalink to this definition">¶</a></dt>
 <dd><p>Retrieve multiple serialized values from the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.backends.redis.RedisBackend.get_serialized_multi.params.keys"></span><strong>keys</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.redis.RedisBackend.get_serialized_multi.params.keys">¶</a> – sequence of string keys that was passed to the
 <a class="reference internal" href="#dogpile.cache.region.CacheRegion.get_multi" title="dogpile.cache.region.CacheRegion.get_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get_multi()</span></code></a> method, which will also be processed
 by the “key mangling” function if one was present.</p>
 </dd>
-<dt class="field-even">Returns</dt>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>list of bytes objects</p>
 </dd>
 </dl>
 <div class="versionadded">
 <p><span class="versionmodified added">New in version 1.1.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.redis.RedisBackend.set_serialized">
 <span class="sig-name descname"><span class="pre">set_serialized</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">value</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.redis.RedisBackend.set_serialized" title="Permalink to this definition">¶</a></dt>
 <dd><p>Set a serialized value in the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="dogpile.cache.backends.redis.RedisBackend.set_serialized.params.key"></span><strong>key</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.redis.RedisBackend.set_serialized.params.key">¶</a> – String key that was passed to the <a class="reference internal" href="#dogpile.cache.region.CacheRegion.set" title="dogpile.cache.region.CacheRegion.set"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.set()</span></code></a>
 method, which will also be processed by the “key mangling” function
 if one was present.</p></li>
 <li><p><span class="target" id="dogpile.cache.backends.redis.RedisBackend.set_serialized.params.value"></span><strong>value</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.redis.RedisBackend.set_serialized.params.value">¶</a> – a bytes object to be stored.</p></li>
 </ul>
 </dd>
@@ -2690,15 +2710,15 @@
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.redis.RedisBackend.set_serialized_multi">
 <span class="sig-name descname"><span class="pre">set_serialized_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">mapping</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.redis.RedisBackend.set_serialized_multi" title="Permalink to this definition">¶</a></dt>
 <dd><p>Set multiple serialized values in the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.backends.redis.RedisBackend.set_serialized_multi.params.mapping"></span><strong>mapping</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.redis.RedisBackend.set_serialized_multi.params.mapping">¶</a> – a dict in which the key will be whatever was passed to
 the <a class="reference internal" href="#dogpile.cache.region.CacheRegion.set_multi" title="dogpile.cache.region.CacheRegion.set_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.set_multi()</span></code></a> method, processed by the “key
 mangling” function, if any.</p>
 </dd>
 </dl>
 <p>When implementing a new <a class="reference internal" href="#dogpile.cache.api.CacheBackend" title="dogpile.cache.api.CacheBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheBackend</span></code></a> or cutomizing via
 <a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">ProxyBackend</span></code></a>, be aware that when this method is invoked by
@@ -2740,15 +2760,15 @@
         <span class="s1">&#39;thread_local_lock&#39;</span><span class="p">:</span> <span class="kc">False</span>
     <span class="p">}</span>
 <span class="p">)</span>
 </pre></div>
 </div>
 <p>Arguments accepted in the arguments dictionary:</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="dogpile.cache.backends.redis.RedisSentinelBackend.params.db"></span><strong>db</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.redis.RedisSentinelBackend.params.db">¶</a> – integer, default is <code class="docutils literal notranslate"><span class="pre">0</span></code>.</p></li>
 <li><p><span class="target" id="dogpile.cache.backends.redis.RedisSentinelBackend.params.redis_expiration_time"></span><strong>redis_expiration_time</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.redis.RedisSentinelBackend.params.redis_expiration_time">¶</a> – integer, number of seconds after setting
 a value that Redis should expire it.  This should be larger than dogpile’s
 cache expiration.  By default no expiration is set.</p></li>
 <li><p><span class="target" id="dogpile.cache.backends.redis.RedisSentinelBackend.params.distributed_lock"></span><strong>distributed_lock</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.redis.RedisSentinelBackend.params.distributed_lock">¶</a> – boolean, when True, will use a
 redis-lock as the dogpile lock. Use this when multiple processes will be
@@ -2781,18 +2801,18 @@
 asynchronous runners, as they run in a different thread than the one
 used to create the lock.</p></li>
 </ul>
 </dd>
 </dl>
 </dd></dl>
 
-</section>
 <span class="target" id="module-dogpile.cache.backends.file"></span><section id="file-backends">
 <h3>File Backends<a class="headerlink" href="#file-backends" title="Permalink to this heading">¶</a></h3>
 <p>Provides backends that deal with local filesystem access.</p>
+</section>
 <dl class="py class">
 <dt class="sig sig-object py" id="dogpile.cache.backends.file.AbstractFileLock">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">dogpile.cache.backends.file.</span></span><span class="sig-name descname"><span class="pre">AbstractFileLock</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">filename</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.file.AbstractFileLock" title="Permalink to this definition">¶</a></dt>
 <dd><p>Bases: <code class="xref py py-class docutils literal notranslate"><span class="pre">object</span></code></p>
 <p>Coordinate read/write access to a file.</p>
 <p>typically is a file-based lock but doesn’t necessarily have to be.</p>
 <p>The default implementation here is <a class="reference internal" href="#dogpile.cache.backends.file.FileLock" title="dogpile.cache.backends.file.FileLock"><code class="xref py py-class docutils literal notranslate"><span class="pre">FileLock</span></code></a>.</p>
@@ -2930,15 +2950,15 @@
 key is problematic, since it’s not generally safe to
 delete lockfiles as the application runs, implying an
 unlimited number of key-based files would need to be
 created and never deleted.</p>
 <p>Parameters to the <code class="docutils literal notranslate"><span class="pre">arguments</span></code> dictionary are
 below.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="dogpile.cache.backends.file.DBMBackend.params.filename"></span><strong>filename</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.file.DBMBackend.params.filename">¶</a> – path of the filename in which to
 create the DBM file.  Note that some dbm backends
 will change this name to have additional suffixes.</p></li>
 <li><p><span class="target" id="dogpile.cache.backends.file.DBMBackend.params.rw_lockfile"></span><strong>rw_lockfile</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.file.DBMBackend.params.rw_lockfile">¶</a> – the name of the file to use for
 read/write locking.  If omitted, a default name
 is used by appending the suffix “.rw.lock” to the
@@ -3001,15 +3021,15 @@
 </dd>
 </dl>
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.file.DBMBackend.delete">
 <span class="sig-name descname"><span class="pre">delete</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.file.DBMBackend.delete" title="Permalink to this definition">¶</a></dt>
 <dd><p>Delete a value from the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.backends.file.DBMBackend.delete.params.key"></span><strong>key</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.file.DBMBackend.delete.params.key">¶</a> – String key that was passed to the
 <a class="reference internal" href="#dogpile.cache.region.CacheRegion.delete" title="dogpile.cache.region.CacheRegion.delete"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.delete()</span></code></a>
 method, which will also be processed by the “key mangling” function
 if one was present.</p>
 </dd>
 </dl>
 <p>The behavior here should be idempotent,
@@ -3019,15 +3039,15 @@
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.file.DBMBackend.delete_multi">
 <span class="sig-name descname"><span class="pre">delete_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">keys</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.file.DBMBackend.delete_multi" title="Permalink to this definition">¶</a></dt>
 <dd><p>Delete multiple values from the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.backends.file.DBMBackend.delete_multi.params.keys"></span><strong>keys</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.file.DBMBackend.delete_multi.params.keys">¶</a> – sequence of string keys that was passed to the
 <a class="reference internal" href="#dogpile.cache.region.CacheRegion.delete_multi" title="dogpile.cache.region.CacheRegion.delete_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.delete_multi()</span></code></a> method, which will also be processed
 by the “key mangling” function if one was present.</p>
 </dd>
 </dl>
 <p>The behavior here should be idempotent,
 that is, can be called any number of times
@@ -3068,54 +3088,54 @@
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.file.DBMBackend.get_serialized">
 <span class="sig-name descname"><span class="pre">get_serialized</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.file.DBMBackend.get_serialized" title="Permalink to this definition">¶</a></dt>
 <dd><p>Retrieve a serialized value from the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.backends.file.DBMBackend.get_serialized.params.key"></span><strong>key</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.file.DBMBackend.get_serialized.params.key">¶</a> – String key that was passed to the <a class="reference internal" href="#dogpile.cache.region.CacheRegion.get" title="dogpile.cache.region.CacheRegion.get"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get()</span></code></a>
 method, which will also be processed by the “key mangling” function
 if one was present.</p>
 </dd>
-<dt class="field-even">Returns</dt>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>a bytes object, or <a class="reference internal" href="#dogpile.cache.api.NO_VALUE" title="dogpile.cache.api.NO_VALUE"><code class="xref py py-data docutils literal notranslate"><span class="pre">NO_VALUE</span></code></a>
 constant if not present.</p>
 </dd>
 </dl>
 <div class="versionadded">
 <p><span class="versionmodified added">New in version 1.1.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.file.DBMBackend.get_serialized_multi">
 <span class="sig-name descname"><span class="pre">get_serialized_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">keys</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.file.DBMBackend.get_serialized_multi" title="Permalink to this definition">¶</a></dt>
 <dd><p>Retrieve multiple serialized values from the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.backends.file.DBMBackend.get_serialized_multi.params.keys"></span><strong>keys</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.file.DBMBackend.get_serialized_multi.params.keys">¶</a> – sequence of string keys that was passed to the
 <a class="reference internal" href="#dogpile.cache.region.CacheRegion.get_multi" title="dogpile.cache.region.CacheRegion.get_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get_multi()</span></code></a> method, which will also be processed
 by the “key mangling” function if one was present.</p>
 </dd>
-<dt class="field-even">Returns</dt>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>list of bytes objects</p>
 </dd>
 </dl>
 <div class="versionadded">
 <p><span class="versionmodified added">New in version 1.1.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.file.DBMBackend.set_serialized">
 <span class="sig-name descname"><span class="pre">set_serialized</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">value</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.file.DBMBackend.set_serialized" title="Permalink to this definition">¶</a></dt>
 <dd><p>Set a serialized value in the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="dogpile.cache.backends.file.DBMBackend.set_serialized.params.key"></span><strong>key</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.file.DBMBackend.set_serialized.params.key">¶</a> – String key that was passed to the <a class="reference internal" href="#dogpile.cache.region.CacheRegion.set" title="dogpile.cache.region.CacheRegion.set"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.set()</span></code></a>
 method, which will also be processed by the “key mangling” function
 if one was present.</p></li>
 <li><p><span class="target" id="dogpile.cache.backends.file.DBMBackend.set_serialized.params.value"></span><strong>value</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.file.DBMBackend.set_serialized.params.value">¶</a> – a bytes object to be stored.</p></li>
 </ul>
 </dd>
@@ -3126,15 +3146,15 @@
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.file.DBMBackend.set_serialized_multi">
 <span class="sig-name descname"><span class="pre">set_serialized_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">mapping</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.file.DBMBackend.set_serialized_multi" title="Permalink to this definition">¶</a></dt>
 <dd><p>Set multiple serialized values in the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.backends.file.DBMBackend.set_serialized_multi.params.mapping"></span><strong>mapping</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.file.DBMBackend.set_serialized_multi.params.mapping">¶</a> – a dict in which the key will be whatever was passed to
 the <a class="reference internal" href="#dogpile.cache.region.CacheRegion.set_multi" title="dogpile.cache.region.CacheRegion.set_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.set_multi()</span></code></a> method, processed by the “key
 mangling” function, if any.</p>
 </dd>
 </dl>
 <p>When implementing a new <a class="reference internal" href="#dogpile.cache.api.CacheBackend" title="dogpile.cache.api.CacheBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheBackend</span></code></a> or cutomizing via
 <a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">ProxyBackend</span></code></a>, be aware that when this method is invoked by
@@ -3193,23 +3213,23 @@
 <dd><p>Release a ‘writer’ lock.</p>
 <p>Raises <code class="docutils literal notranslate"><span class="pre">NotImplementedError</span></code> by default, must be
 implemented by subclasses.</p>
 </dd></dl>
 
 </dd></dl>
 
-</section>
 <span class="target" id="module-dogpile.cache.proxy"></span><section id="proxy-backends">
 <h3>Proxy Backends<a class="headerlink" href="#proxy-backends" title="Permalink to this heading">¶</a></h3>
 <p>Provides a utility and a decorator class that allow for modifying the behavior
 of different backends without altering the class itself or having to extend the
 base backend.</p>
 <div class="versionadded">
 <p><span class="versionmodified added">New in version 0.5.0: </span>Added support for the <a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">ProxyBackend</span></code></a> class.</p>
 </div>
+</section>
 <dl class="py class">
 <dt class="sig sig-object py" id="dogpile.cache.proxy.ProxyBackend">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">dogpile.cache.proxy.</span></span><span class="sig-name descname"><span class="pre">ProxyBackend</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">arg</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">kw</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.proxy.ProxyBackend" title="Permalink to this definition">¶</a></dt>
 <dd><p>Bases: <a class="reference internal" href="#dogpile.cache.api.CacheBackend" title="dogpile.cache.api.CacheBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheBackend</span></code></a></p>
 <p>A decorator class for altering the functionality of backends.</p>
 <p>Basic usage:</p>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="kn">from</span> <span class="nn">dogpile.cache</span> <span class="kn">import</span> <span class="n">make_region</span>
@@ -3249,15 +3269,15 @@
 <p><span class="versionmodified added">New in version 0.5.0.</span></p>
 </div>
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.proxy.ProxyBackend.delete">
 <span class="sig-name descname"><span class="pre">delete</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#dogpile.cache.proxy.ProxyBackend.delete" title="Permalink to this definition">¶</a></dt>
 <dd><p>Delete a value from the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.proxy.ProxyBackend.delete.params.key"></span><strong>key</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.proxy.ProxyBackend.delete.params.key">¶</a> – String key that was passed to the
 <a class="reference internal" href="#dogpile.cache.region.CacheRegion.delete" title="dogpile.cache.region.CacheRegion.delete"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.delete()</span></code></a>
 method, which will also be processed by the “key mangling” function
 if one was present.</p>
 </dd>
 </dl>
 <p>The behavior here should be idempotent,
@@ -3267,15 +3287,15 @@
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.proxy.ProxyBackend.delete_multi">
 <span class="sig-name descname"><span class="pre">delete_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">keys</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#dogpile.cache.proxy.ProxyBackend.delete_multi" title="Permalink to this definition">¶</a></dt>
 <dd><p>Delete multiple values from the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.proxy.ProxyBackend.delete_multi.params.keys"></span><strong>keys</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.proxy.ProxyBackend.delete_multi.params.keys">¶</a> – sequence of string keys that was passed to the
 <a class="reference internal" href="#dogpile.cache.region.CacheRegion.delete_multi" title="dogpile.cache.region.CacheRegion.delete_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.delete_multi()</span></code></a> method, which will also be processed
 by the “key mangling” function if one was present.</p>
 </dd>
 </dl>
 <p>The behavior here should be idempotent,
 that is, can be called any number of times
@@ -3284,38 +3304,38 @@
 <div class="versionadded">
 <p><span class="versionmodified added">New in version 0.5.0.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.proxy.ProxyBackend.get">
-<span class="sig-name descname"><span class="pre">get</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><span class="pre">CachedValue</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference internal" href="#dogpile.cache.api.NoValue" title="dogpile.cache.api.NoValue"><span class="pre">NoValue</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">bytes</span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#dogpile.cache.proxy.ProxyBackend.get" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">get</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><span class="pre">CachedValue</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference internal" href="#dogpile.cache.api.NoValue" title="dogpile.cache.api.NoValue"><span class="pre">NoValue</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">bytes</span></span></span><a class="headerlink" href="#dogpile.cache.proxy.ProxyBackend.get" title="Permalink to this definition">¶</a></dt>
 <dd><p>Retrieve an optionally serialized value from the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.proxy.ProxyBackend.get.params.key"></span><strong>key</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.proxy.ProxyBackend.get.params.key">¶</a> – String key that was passed to the <a class="reference internal" href="#dogpile.cache.region.CacheRegion.get" title="dogpile.cache.region.CacheRegion.get"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get()</span></code></a>
 method, which will also be processed by the “key mangling” function
 if one was present.</p>
 </dd>
-<dt class="field-even">Returns</dt>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>the Python object that corresponds to
 what was established via the <a class="reference internal" href="#dogpile.cache.api.CacheBackend.set" title="dogpile.cache.api.CacheBackend.set"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.set()</span></code></a> method,
 or the <a class="reference internal" href="#dogpile.cache.api.NO_VALUE" title="dogpile.cache.api.NO_VALUE"><code class="xref py py-data docutils literal notranslate"><span class="pre">NO_VALUE</span></code></a> constant if not present.</p>
 </dd>
 </dl>
 <p>If a serializer is in use, this method will only be called if the
 <a class="reference internal" href="#dogpile.cache.api.CacheBackend.get_serialized" title="dogpile.cache.api.CacheBackend.get_serialized"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.get_serialized()</span></code></a> method is not overridden.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.proxy.ProxyBackend.get_multi">
-<span class="sig-name descname"><span class="pre">get_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">keys</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><span class="pre">CachedValue</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference internal" href="#dogpile.cache.api.NoValue" title="dogpile.cache.api.NoValue"><span class="pre">NoValue</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">bytes</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#dogpile.cache.proxy.ProxyBackend.get_multi" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">get_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">keys</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><span class="pre">CachedValue</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference internal" href="#dogpile.cache.api.NoValue" title="dogpile.cache.api.NoValue"><span class="pre">NoValue</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">bytes</span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#dogpile.cache.proxy.ProxyBackend.get_multi" title="Permalink to this definition">¶</a></dt>
 <dd><p>Retrieve multiple optionally serialized values from the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.proxy.ProxyBackend.get_multi.params.keys"></span><strong>keys</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.proxy.ProxyBackend.get_multi.params.keys">¶</a> – sequence of string keys that was passed to the
 <a class="reference internal" href="#dogpile.cache.region.CacheRegion.get_multi" title="dogpile.cache.region.CacheRegion.get_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get_multi()</span></code></a> method, which will also be processed
 by the “key mangling” function if one was present.</p>
 </dd>
 </dl>
 <dl class="simple">
 <dt>:return a list of values as would be returned</dt><dd><p>individually via the <a class="reference internal" href="#dogpile.cache.api.CacheBackend.get" title="dogpile.cache.api.CacheBackend.get"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.get()</span></code></a> method, corresponding
@@ -3327,15 +3347,15 @@
 <div class="versionadded">
 <p><span class="versionmodified added">New in version 0.5.0.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.proxy.ProxyBackend.get_mutex">
-<span class="sig-name descname"><span class="pre">get_mutex</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#dogpile.cache.api.CacheMutex" title="dogpile.cache.api.CacheMutex"><span class="pre">CacheMutex</span></a><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#dogpile.cache.proxy.ProxyBackend.get_mutex" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">get_mutex</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#dogpile.cache.api.CacheMutex" title="dogpile.cache.api.CacheMutex"><span class="pre">CacheMutex</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span></span><a class="headerlink" href="#dogpile.cache.proxy.ProxyBackend.get_mutex" title="Permalink to this definition">¶</a></dt>
 <dd><p>Return an optional mutexing object for the given key.</p>
 <p>This object need only provide an <code class="docutils literal notranslate"><span class="pre">acquire()</span></code>
 and <code class="docutils literal notranslate"><span class="pre">release()</span></code> method.</p>
 <p>May return <code class="docutils literal notranslate"><span class="pre">None</span></code>, in which case the dogpile
 lock will use a regular <code class="docutils literal notranslate"><span class="pre">threading.Lock</span></code>
 object to mutex concurrent threads for
 value creation.   The default implementation
@@ -3356,23 +3376,23 @@
 can be used as a means of throttling the total
 number of value recreation operations that may
 proceed at one time.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.proxy.ProxyBackend.get_serialized">
-<span class="sig-name descname"><span class="pre">get_serialized</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><span class="pre">bytes</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference internal" href="#dogpile.cache.api.NoValue" title="dogpile.cache.api.NoValue"><span class="pre">NoValue</span></a><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#dogpile.cache.proxy.ProxyBackend.get_serialized" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">get_serialized</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">bytes</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference internal" href="#dogpile.cache.api.NoValue" title="dogpile.cache.api.NoValue"><span class="pre">NoValue</span></a></span></span><a class="headerlink" href="#dogpile.cache.proxy.ProxyBackend.get_serialized" title="Permalink to this definition">¶</a></dt>
 <dd><p>Retrieve a serialized value from the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.proxy.ProxyBackend.get_serialized.params.key"></span><strong>key</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.proxy.ProxyBackend.get_serialized.params.key">¶</a> – String key that was passed to the <a class="reference internal" href="#dogpile.cache.region.CacheRegion.get" title="dogpile.cache.region.CacheRegion.get"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get()</span></code></a>
 method, which will also be processed by the “key mangling” function
 if one was present.</p>
 </dd>
-<dt class="field-even">Returns</dt>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>a bytes object, or <a class="reference internal" href="#dogpile.cache.api.NO_VALUE" title="dogpile.cache.api.NO_VALUE"><code class="xref py py-data docutils literal notranslate"><span class="pre">NO_VALUE</span></code></a>
 constant if not present.</p>
 </dd>
 </dl>
 <p>The default implementation of this method for <a class="reference internal" href="#dogpile.cache.api.CacheBackend" title="dogpile.cache.api.CacheBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheBackend</span></code></a>
 returns the value of the <a class="reference internal" href="#dogpile.cache.api.CacheBackend.get" title="dogpile.cache.api.CacheBackend.get"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.get()</span></code></a> method.</p>
 <div class="versionadded">
@@ -3382,23 +3402,23 @@
 <p class="admonition-title">See also</p>
 <p><a class="reference internal" href="#dogpile.cache.api.BytesBackend" title="dogpile.cache.api.BytesBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">BytesBackend</span></code></a></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.proxy.ProxyBackend.get_serialized_multi">
-<span class="sig-name descname"><span class="pre">get_serialized_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">keys</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><span class="pre">bytes</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference internal" href="#dogpile.cache.api.NoValue" title="dogpile.cache.api.NoValue"><span class="pre">NoValue</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#dogpile.cache.proxy.ProxyBackend.get_serialized_multi" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">get_serialized_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">keys</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">bytes</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference internal" href="#dogpile.cache.api.NoValue" title="dogpile.cache.api.NoValue"><span class="pre">NoValue</span></a><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#dogpile.cache.proxy.ProxyBackend.get_serialized_multi" title="Permalink to this definition">¶</a></dt>
 <dd><p>Retrieve multiple serialized values from the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.proxy.ProxyBackend.get_serialized_multi.params.keys"></span><strong>keys</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.proxy.ProxyBackend.get_serialized_multi.params.keys">¶</a> – sequence of string keys that was passed to the
 <a class="reference internal" href="#dogpile.cache.region.CacheRegion.get_multi" title="dogpile.cache.region.CacheRegion.get_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get_multi()</span></code></a> method, which will also be processed
 by the “key mangling” function if one was present.</p>
 </dd>
-<dt class="field-even">Returns</dt>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>list of bytes objects</p>
 </dd>
 </dl>
 <p>The default implementation of this method for <a class="reference internal" href="#dogpile.cache.api.CacheBackend" title="dogpile.cache.api.CacheBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheBackend</span></code></a>
 returns the value of the <a class="reference internal" href="#dogpile.cache.api.CacheBackend.get_multi" title="dogpile.cache.api.CacheBackend.get_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.get_multi()</span></code></a> method.</p>
 <div class="versionadded">
 <p><span class="versionmodified added">New in version 1.1.</span></p>
@@ -3407,18 +3427,18 @@
 <p class="admonition-title">See also</p>
 <p><a class="reference internal" href="#dogpile.cache.api.BytesBackend" title="dogpile.cache.api.BytesBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">BytesBackend</span></code></a></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.proxy.ProxyBackend.set">
-<span class="sig-name descname"><span class="pre">set</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">value</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><span class="pre">CachedValue</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">bytes</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#dogpile.cache.proxy.ProxyBackend.set" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">set</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">value</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><span class="pre">CachedValue</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">bytes</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#dogpile.cache.proxy.ProxyBackend.set" title="Permalink to this definition">¶</a></dt>
 <dd><p>Set an optionally serialized value in the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="dogpile.cache.proxy.ProxyBackend.set.params.key"></span><strong>key</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.proxy.ProxyBackend.set.params.key">¶</a> – String key that was passed to the <a class="reference internal" href="#dogpile.cache.region.CacheRegion.set" title="dogpile.cache.region.CacheRegion.set"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.set()</span></code></a>
 method, which will also be processed by the “key mangling” function
 if one was present.</p></li>
 <li><p><span class="target" id="dogpile.cache.proxy.ProxyBackend.set.params.value"></span><strong>value</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.proxy.ProxyBackend.set.params.value">¶</a> – The optionally serialized <a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><code class="xref py py-class docutils literal notranslate"><span class="pre">CachedValue</span></code></a> object.
 May be an instance of <a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><code class="xref py py-class docutils literal notranslate"><span class="pre">CachedValue</span></code></a> or a bytes object
 depending on if a serializer is in use with the region and if the
@@ -3430,18 +3450,18 @@
 <p class="admonition-title">See also</p>
 <p><a class="reference internal" href="#dogpile.cache.api.CacheBackend.set_serialized" title="dogpile.cache.api.CacheBackend.set_serialized"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.set_serialized()</span></code></a></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.proxy.ProxyBackend.set_multi">
-<span class="sig-name descname"><span class="pre">set_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">mapping</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Mapping</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><span class="pre">CachedValue</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">bytes</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#dogpile.cache.proxy.ProxyBackend.set_multi" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">set_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">mapping</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Mapping</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><span class="pre">CachedValue</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">bytes</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#dogpile.cache.proxy.ProxyBackend.set_multi" title="Permalink to this definition">¶</a></dt>
 <dd><p>Set multiple values in the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.proxy.ProxyBackend.set_multi.params.mapping"></span><strong>mapping</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.proxy.ProxyBackend.set_multi.params.mapping">¶</a> – a dict in which the key will be whatever was passed to
 the <a class="reference internal" href="#dogpile.cache.region.CacheRegion.set_multi" title="dogpile.cache.region.CacheRegion.set_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.set_multi()</span></code></a> method, processed by the “key
 mangling” function, if any.</p>
 </dd>
 </dl>
 <p>When implementing a new <a class="reference internal" href="#dogpile.cache.api.CacheBackend" title="dogpile.cache.api.CacheBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheBackend</span></code></a> or cutomizing via
 <a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">ProxyBackend</span></code></a>, be aware that when this method is invoked by
@@ -3458,15 +3478,15 @@
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.proxy.ProxyBackend.set_serialized">
 <span class="sig-name descname"><span class="pre">set_serialized</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">value</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bytes</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#dogpile.cache.proxy.ProxyBackend.set_serialized" title="Permalink to this definition">¶</a></dt>
 <dd><p>Set a serialized value in the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="dogpile.cache.proxy.ProxyBackend.set_serialized.params.key"></span><strong>key</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.proxy.ProxyBackend.set_serialized.params.key">¶</a> – String key that was passed to the <a class="reference internal" href="#dogpile.cache.region.CacheRegion.set" title="dogpile.cache.region.CacheRegion.set"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.set()</span></code></a>
 method, which will also be processed by the “key mangling” function
 if one was present.</p></li>
 <li><p><span class="target" id="dogpile.cache.proxy.ProxyBackend.set_serialized.params.value"></span><strong>value</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.proxy.ProxyBackend.set_serialized.params.value">¶</a> – a bytes object to be stored.</p></li>
 </ul>
 </dd>
@@ -3483,15 +3503,15 @@
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.proxy.ProxyBackend.set_serialized_multi">
 <span class="sig-name descname"><span class="pre">set_serialized_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">mapping</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Mapping</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">bytes</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#dogpile.cache.proxy.ProxyBackend.set_serialized_multi" title="Permalink to this definition">¶</a></dt>
 <dd><p>Set multiple serialized values in the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.proxy.ProxyBackend.set_serialized_multi.params.mapping"></span><strong>mapping</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.proxy.ProxyBackend.set_serialized_multi.params.mapping">¶</a> – a dict in which the key will be whatever was passed to
 the <a class="reference internal" href="#dogpile.cache.region.CacheRegion.set_multi" title="dogpile.cache.region.CacheRegion.set_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.set_multi()</span></code></a> method, processed by the “key
 mangling” function, if any.</p>
 </dd>
 </dl>
 <p>When implementing a new <a class="reference internal" href="#dogpile.cache.api.CacheBackend" title="dogpile.cache.api.CacheBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheBackend</span></code></a> or cutomizing via
 <a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">ProxyBackend</span></code></a>, be aware that when this method is invoked by
@@ -3517,23 +3537,23 @@
 <dd><p>Take a backend as an argument and setup the self.proxied property.
 Return an object that be used as a backend by a <a class="reference internal" href="#dogpile.cache.region.CacheRegion" title="dogpile.cache.region.CacheRegion"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheRegion</span></code></a>
 object.</p>
 </dd></dl>
 
 </dd></dl>
 
-</section>
 <span class="target" id="module-dogpile.cache.backends.null"></span><section id="null-backend">
 <h3>Null Backend<a class="headerlink" href="#null-backend" title="Permalink to this heading">¶</a></h3>
 <p>The Null backend does not do any caching at all.  It can be
 used to test behavior without caching, or as a means of disabling
 caching for a region that is otherwise used normally.</p>
 <div class="versionadded">
 <p><span class="versionmodified added">New in version 0.5.4.</span></p>
 </div>
+</section>
 <dl class="py class">
 <dt class="sig sig-object py" id="dogpile.cache.backends.null.NullBackend">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">dogpile.cache.backends.null.</span></span><span class="sig-name descname"><span class="pre">NullBackend</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">arguments</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.null.NullBackend" title="Permalink to this definition">¶</a></dt>
 <dd><p>Bases: <a class="reference internal" href="#dogpile.cache.api.CacheBackend" title="dogpile.cache.api.CacheBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheBackend</span></code></a></p>
 <p>A “null” backend that effectively disables all cache operations.</p>
 <p>Basic usage:</p>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="kn">from</span> <span class="nn">dogpile.cache</span> <span class="kn">import</span> <span class="n">make_region</span>
@@ -3544,15 +3564,15 @@
 </pre></div>
 </div>
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.null.NullBackend.delete">
 <span class="sig-name descname"><span class="pre">delete</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.null.NullBackend.delete" title="Permalink to this definition">¶</a></dt>
 <dd><p>Delete a value from the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.backends.null.NullBackend.delete.params.key"></span><strong>key</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.null.NullBackend.delete.params.key">¶</a> – String key that was passed to the
 <a class="reference internal" href="#dogpile.cache.region.CacheRegion.delete" title="dogpile.cache.region.CacheRegion.delete"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.delete()</span></code></a>
 method, which will also be processed by the “key mangling” function
 if one was present.</p>
 </dd>
 </dl>
 <p>The behavior here should be idempotent,
@@ -3562,15 +3582,15 @@
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.null.NullBackend.delete_multi">
 <span class="sig-name descname"><span class="pre">delete_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">keys</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.null.NullBackend.delete_multi" title="Permalink to this definition">¶</a></dt>
 <dd><p>Delete multiple values from the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.backends.null.NullBackend.delete_multi.params.keys"></span><strong>keys</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.null.NullBackend.delete_multi.params.keys">¶</a> – sequence of string keys that was passed to the
 <a class="reference internal" href="#dogpile.cache.region.CacheRegion.delete_multi" title="dogpile.cache.region.CacheRegion.delete_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.delete_multi()</span></code></a> method, which will also be processed
 by the “key mangling” function if one was present.</p>
 </dd>
 </dl>
 <p>The behavior here should be idempotent,
 that is, can be called any number of times
@@ -3582,35 +3602,35 @@
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.null.NullBackend.get">
 <span class="sig-name descname"><span class="pre">get</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.null.NullBackend.get" title="Permalink to this definition">¶</a></dt>
 <dd><p>Retrieve an optionally serialized value from the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.backends.null.NullBackend.get.params.key"></span><strong>key</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.null.NullBackend.get.params.key">¶</a> – String key that was passed to the <a class="reference internal" href="#dogpile.cache.region.CacheRegion.get" title="dogpile.cache.region.CacheRegion.get"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get()</span></code></a>
 method, which will also be processed by the “key mangling” function
 if one was present.</p>
 </dd>
-<dt class="field-even">Returns</dt>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>the Python object that corresponds to
 what was established via the <a class="reference internal" href="#dogpile.cache.api.CacheBackend.set" title="dogpile.cache.api.CacheBackend.set"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.set()</span></code></a> method,
 or the <a class="reference internal" href="#dogpile.cache.api.NO_VALUE" title="dogpile.cache.api.NO_VALUE"><code class="xref py py-data docutils literal notranslate"><span class="pre">NO_VALUE</span></code></a> constant if not present.</p>
 </dd>
 </dl>
 <p>If a serializer is in use, this method will only be called if the
 <a class="reference internal" href="#dogpile.cache.api.CacheBackend.get_serialized" title="dogpile.cache.api.CacheBackend.get_serialized"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.get_serialized()</span></code></a> method is not overridden.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.null.NullBackend.get_multi">
 <span class="sig-name descname"><span class="pre">get_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">keys</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.null.NullBackend.get_multi" title="Permalink to this definition">¶</a></dt>
 <dd><p>Retrieve multiple optionally serialized values from the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.backends.null.NullBackend.get_multi.params.keys"></span><strong>keys</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.null.NullBackend.get_multi.params.keys">¶</a> – sequence of string keys that was passed to the
 <a class="reference internal" href="#dogpile.cache.region.CacheRegion.get_multi" title="dogpile.cache.region.CacheRegion.get_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get_multi()</span></code></a> method, which will also be processed
 by the “key mangling” function if one was present.</p>
 </dd>
 </dl>
 <dl class="simple">
 <dt>:return a list of values as would be returned</dt><dd><p>individually via the <a class="reference internal" href="#dogpile.cache.api.CacheBackend.get" title="dogpile.cache.api.CacheBackend.get"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.get()</span></code></a> method, corresponding
@@ -3654,15 +3674,15 @@
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.null.NullBackend.set">
 <span class="sig-name descname"><span class="pre">set</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">value</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.null.NullBackend.set" title="Permalink to this definition">¶</a></dt>
 <dd><p>Set an optionally serialized value in the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="dogpile.cache.backends.null.NullBackend.set.params.key"></span><strong>key</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.null.NullBackend.set.params.key">¶</a> – String key that was passed to the <a class="reference internal" href="#dogpile.cache.region.CacheRegion.set" title="dogpile.cache.region.CacheRegion.set"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.set()</span></code></a>
 method, which will also be processed by the “key mangling” function
 if one was present.</p></li>
 <li><p><span class="target" id="dogpile.cache.backends.null.NullBackend.set.params.value"></span><strong>value</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.null.NullBackend.set.params.value">¶</a> – The optionally serialized <a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><code class="xref py py-class docutils literal notranslate"><span class="pre">CachedValue</span></code></a> object.
 May be an instance of <a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><code class="xref py py-class docutils literal notranslate"><span class="pre">CachedValue</span></code></a> or a bytes object
 depending on if a serializer is in use with the region and if the
@@ -3677,15 +3697,15 @@
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.null.NullBackend.set_multi">
 <span class="sig-name descname"><span class="pre">set_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">mapping</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.null.NullBackend.set_multi" title="Permalink to this definition">¶</a></dt>
 <dd><p>Set multiple values in the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.backends.null.NullBackend.set_multi.params.mapping"></span><strong>mapping</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.null.NullBackend.set_multi.params.mapping">¶</a> – a dict in which the key will be whatever was passed to
 the <a class="reference internal" href="#dogpile.cache.region.CacheRegion.set_multi" title="dogpile.cache.region.CacheRegion.set_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.set_multi()</span></code></a> method, processed by the “key
 mangling” function, if any.</p>
 </dd>
 </dl>
 <p>When implementing a new <a class="reference internal" href="#dogpile.cache.api.CacheBackend" title="dogpile.cache.api.CacheBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheBackend</span></code></a> or cutomizing via
 <a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">ProxyBackend</span></code></a>, be aware that when this method is invoked by
@@ -3700,15 +3720,14 @@
 <p><span class="versionmodified added">New in version 0.5.0.</span></p>
 </div>
 </dd></dl>
 
 </dd></dl>
 
 </section>
-</section>
 <section id="module-dogpile.cache.exception">
 <span id="exceptions"></span><h2>Exceptions<a class="headerlink" href="#module-dogpile.cache.exception" title="Permalink to this heading">¶</a></h2>
 <p>Exception classes for dogpile.cache.</p>
 <dl class="py exception">
 <dt class="sig sig-object py" id="dogpile.cache.exception.DogpileCacheException">
 <em class="property"><span class="pre">exception</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">dogpile.cache.exception.</span></span><span class="sig-name descname"><span class="pre">DogpileCacheException</span></span><a class="headerlink" href="#dogpile.cache.exception.DogpileCacheException" title="Permalink to this definition">¶</a></dt>
 <dd><p>Bases: <code class="xref py py-class docutils literal notranslate"><span class="pre">Exception</span></code></p>
@@ -3785,25 +3804,26 @@
 argument  on any Mako tag which accepts it, in conjunction with the
 name of the desired region as the <code class="docutils literal notranslate"><span class="pre">cache_region</span></code> argument:</p>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="o">&lt;%</span><span class="k">def</span> <span class="nf">name</span><span class="o">=</span><span class="s2">&quot;mysection()&quot;</span> <span class="n">cached</span><span class="o">=</span><span class="s2">&quot;True&quot;</span> <span class="n">cache_region</span><span class="o">=</span><span class="s2">&quot;memcached&quot;</span><span class="o">&gt;</span>
     <span class="n">some</span> <span class="n">content</span> <span class="n">that</span><span class="s1">&#39;s cached</span>
 <span class="o">&lt;/%</span><span class="n">def</span><span class="o">&gt;</span>
 </pre></div>
 </div>
+</section>
 <dl class="py class">
 <dt class="sig sig-object py" id="dogpile.cache.plugins.mako_cache.MakoPlugin">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">dogpile.cache.plugins.mako_cache.</span></span><span class="sig-name descname"><span class="pre">MakoPlugin</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">cache</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.plugins.mako_cache.MakoPlugin" title="Permalink to this definition">¶</a></dt>
 <dd><p>Bases: <code class="xref py py-class docutils literal notranslate"><span class="pre">CacheImpl</span></code></p>
 <p>A Mako <code class="docutils literal notranslate"><span class="pre">CacheImpl</span></code> which talks to dogpile.cache.</p>
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.plugins.mako_cache.MakoPlugin.get">
 <span class="sig-name descname"><span class="pre">get</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">kw</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.plugins.mako_cache.MakoPlugin.get" title="Permalink to this definition">¶</a></dt>
 <dd><p>Retrieve a value from the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="dogpile.cache.plugins.mako_cache.MakoPlugin.get.params.key"></span><strong>key</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.plugins.mako_cache.MakoPlugin.get.params.key">¶</a> – the value’s key.</p></li>
 <li><p><span class="target" id="dogpile.cache.plugins.mako_cache.MakoPlugin.get.params.**kw"></span><strong>**kw</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.plugins.mako_cache.MakoPlugin.get.params.**kw">¶</a> – cache configuration arguments.</p></li>
 </ul>
 </dd>
 </dl>
 </dd></dl>
@@ -3815,15 +3835,15 @@
 to generate a new value.</p>
 <p>This function <em>must</em> return a value, either from
 the cache, or via the given creation function.
 If the creation function is called, the newly
 created value should be populated into the cache
 under the given key before being returned.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="dogpile.cache.plugins.mako_cache.MakoPlugin.get_or_create.params.key"></span><strong>key</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.plugins.mako_cache.MakoPlugin.get_or_create.params.key">¶</a> – the value’s key.</p></li>
 <li><p><span class="target" id="dogpile.cache.plugins.mako_cache.MakoPlugin.get_or_create.params.creation_function"></span><strong>creation_function</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.plugins.mako_cache.MakoPlugin.get_or_create.params.creation_function">¶</a> – function that when called generates
 a new value.</p></li>
 <li><p><span class="target" id="dogpile.cache.plugins.mako_cache.MakoPlugin.get_or_create.params.**kw"></span><strong>**kw</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.plugins.mako_cache.MakoPlugin.get_or_create.params.**kw">¶</a> – cache configuration arguments.</p></li>
 </ul>
 </dd>
@@ -3831,27 +3851,26 @@
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.plugins.mako_cache.MakoPlugin.invalidate">
 <span class="sig-name descname"><span class="pre">invalidate</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">kw</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.plugins.mako_cache.MakoPlugin.invalidate" title="Permalink to this definition">¶</a></dt>
 <dd><p>Invalidate a value in the cache.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="dogpile.cache.plugins.mako_cache.MakoPlugin.invalidate.params.key"></span><strong>key</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.plugins.mako_cache.MakoPlugin.invalidate.params.key">¶</a> – the value’s key.</p></li>
 <li><p><span class="target" id="dogpile.cache.plugins.mako_cache.MakoPlugin.invalidate.params.**kw"></span><strong>**kw</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.plugins.mako_cache.MakoPlugin.invalidate.params.**kw">¶</a> – cache configuration arguments.</p></li>
 </ul>
 </dd>
 </dl>
 </dd></dl>
 
 </dd></dl>
 
 </section>
-</section>
 <section id="utilities">
 <h2>Utilities<a class="headerlink" href="#utilities" title="Permalink to this heading">¶</a></h2>
 <dl class="py function">
 <dt class="sig sig-object py" id="dogpile.cache.util.function_key_generator">
 <span class="sig-prename descclassname"><span class="pre">dogpile.cache.util.</span></span><span class="sig-name descname"><span class="pre">function_key_generator</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">namespace</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">fn</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">to_str=&lt;class</span> <span class="pre">'str'&gt;</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.util.function_key_generator" title="Permalink to this definition">¶</a></dt>
 <dd><p>Return a function that generates a string
 key, based on a given function as well as
@@ -3910,15 +3929,15 @@
 <dd><p>Dogpile lock class.</p>
 <p>Provides an interface around an arbitrary mutex
 that allows one thread/process to be elected as
 the creator of a new value, while other threads/processes
 continue to return the previous version
 of that value.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="dogpile.Lock.params.mutex"></span><strong>mutex</strong><a class="paramlink headerlink reference internal" href="#dogpile.Lock.params.mutex">¶</a> – A mutex object that provides <code class="docutils literal notranslate"><span class="pre">acquire()</span></code>
 and <code class="docutils literal notranslate"><span class="pre">release()</span></code> methods.</p></li>
 <li><p><span class="target" id="dogpile.Lock.params.creator"></span><strong>creator</strong><a class="paramlink headerlink reference internal" href="#dogpile.Lock.params.creator">¶</a> – Callable which returns a tuple of the form
 (new_value, creation_time).  “new_value” should be a newly
 generated value representing completed state.  “creation_time”
 should be a floating point time value which is relative
@@ -4016,26 +4035,26 @@
 <code class="docutils literal notranslate"><span class="pre">MyFoo</span></code> will be called once, passing the
 identifier <code class="docutils literal notranslate"><span class="pre">foo1</span></code> as the argument.</p>
 <p>When thread 1 and thread 2 both complete or
 otherwise delete references to <code class="docutils literal notranslate"><span class="pre">my_foo</span></code>, the
 object is <em>removed</em> from the <a class="reference internal" href="#dogpile.util.NameRegistry" title="dogpile.util.NameRegistry"><code class="xref py py-class docutils literal notranslate"><span class="pre">NameRegistry</span></code></a> as
 a result of Python garbage collection.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.util.NameRegistry.params.creator"></span><strong>creator</strong><a class="paramlink headerlink reference internal" href="#dogpile.util.NameRegistry.params.creator">¶</a> – A function that will create a new
 value, given the identifier passed to the <a class="reference internal" href="#dogpile.util.NameRegistry.get" title="dogpile.util.NameRegistry.get"><code class="xref py py-meth docutils literal notranslate"><span class="pre">NameRegistry.get()</span></code></a>
 method.</p>
 </dd>
 </dl>
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.util.NameRegistry.get">
 <span class="sig-name descname"><span class="pre">get</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">identifier</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">args</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Any</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">kw</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Any</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Any</span></span></span><a class="headerlink" href="#dogpile.util.NameRegistry.get" title="Permalink to this definition">¶</a></dt>
 <dd><p>Get and possibly create the value.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="dogpile.util.NameRegistry.get.params.identifier"></span><strong>identifier</strong><a class="paramlink headerlink reference internal" href="#dogpile.util.NameRegistry.get.params.identifier">¶</a> – Hash key for the value.
 If the creation function is called, this identifier
 will also be passed to the creation function.</p></li>
 <li><p><span class="target" id="dogpile.util.NameRegistry.get.params.**kw"></span><strong>**kw</strong><a class="paramlink headerlink reference internal" href="#dogpile.util.NameRegistry.get.params.**kw">¶</a> (<em>*args</em><em>,</em>) – Additional arguments which will
 also be passed to the creation function if it is
 called.</p></li>
@@ -4056,32 +4075,252 @@
       </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
         <div class="sphinxsidebarwrapper">
   <div>
     <h3><a href="index.html">Table of Contents</a></h3>
     <ul>
 <li><a class="reference internal" href="#">API</a><ul>
-<li><a class="reference internal" href="#module-dogpile.cache.region">Region</a></li>
-<li><a class="reference internal" href="#backend-api">Backend API</a></li>
+<li><a class="reference internal" href="#module-dogpile.cache.region">Region</a><ul>
+<li><a class="reference internal" href="#dogpile.cache.region.CacheRegion"><code class="docutils literal notranslate"><span class="pre">CacheRegion</span></code></a><ul>
+<li><a class="reference internal" href="#dogpile.cache.region.CacheRegion.actual_backend"><code class="docutils literal notranslate"><span class="pre">CacheRegion.actual_backend</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.region.CacheRegion.cache_multi_on_arguments"><code class="docutils literal notranslate"><span class="pre">CacheRegion.cache_multi_on_arguments()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.region.CacheRegion.cache_on_arguments"><code class="docutils literal notranslate"><span class="pre">CacheRegion.cache_on_arguments()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.region.CacheRegion.configure"><code class="docutils literal notranslate"><span class="pre">CacheRegion.configure()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.region.CacheRegion.configure_from_config"><code class="docutils literal notranslate"><span class="pre">CacheRegion.configure_from_config()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.region.CacheRegion.delete"><code class="docutils literal notranslate"><span class="pre">CacheRegion.delete()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.region.CacheRegion.delete_multi"><code class="docutils literal notranslate"><span class="pre">CacheRegion.delete_multi()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.region.CacheRegion.get"><code class="docutils literal notranslate"><span class="pre">CacheRegion.get()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.region.CacheRegion.get_multi"><code class="docutils literal notranslate"><span class="pre">CacheRegion.get_multi()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.region.CacheRegion.get_or_create"><code class="docutils literal notranslate"><span class="pre">CacheRegion.get_or_create()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.region.CacheRegion.get_or_create_multi"><code class="docutils literal notranslate"><span class="pre">CacheRegion.get_or_create_multi()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.region.CacheRegion.invalidate"><code class="docutils literal notranslate"><span class="pre">CacheRegion.invalidate()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.region.CacheRegion.is_configured"><code class="docutils literal notranslate"><span class="pre">CacheRegion.is_configured</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.region.CacheRegion.key_is_locked"><code class="docutils literal notranslate"><span class="pre">CacheRegion.key_is_locked()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.region.CacheRegion.set"><code class="docutils literal notranslate"><span class="pre">CacheRegion.set()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.region.CacheRegion.set_multi"><code class="docutils literal notranslate"><span class="pre">CacheRegion.set_multi()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.region.CacheRegion.wrap"><code class="docutils literal notranslate"><span class="pre">CacheRegion.wrap()</span></code></a></li>
+</ul>
+</li>
+<li><a class="reference internal" href="#dogpile.cache.region.DefaultInvalidationStrategy"><code class="docutils literal notranslate"><span class="pre">DefaultInvalidationStrategy</span></code></a><ul>
+<li><a class="reference internal" href="#dogpile.cache.region.DefaultInvalidationStrategy.invalidate"><code class="docutils literal notranslate"><span class="pre">DefaultInvalidationStrategy.invalidate()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.region.DefaultInvalidationStrategy.is_hard_invalidated"><code class="docutils literal notranslate"><span class="pre">DefaultInvalidationStrategy.is_hard_invalidated()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.region.DefaultInvalidationStrategy.is_invalidated"><code class="docutils literal notranslate"><span class="pre">DefaultInvalidationStrategy.is_invalidated()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.region.DefaultInvalidationStrategy.is_soft_invalidated"><code class="docutils literal notranslate"><span class="pre">DefaultInvalidationStrategy.is_soft_invalidated()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.region.DefaultInvalidationStrategy.was_hard_invalidated"><code class="docutils literal notranslate"><span class="pre">DefaultInvalidationStrategy.was_hard_invalidated()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.region.DefaultInvalidationStrategy.was_soft_invalidated"><code class="docutils literal notranslate"><span class="pre">DefaultInvalidationStrategy.was_soft_invalidated()</span></code></a></li>
+</ul>
+</li>
+<li><a class="reference internal" href="#dogpile.cache.region.RegionInvalidationStrategy"><code class="docutils literal notranslate"><span class="pre">RegionInvalidationStrategy</span></code></a><ul>
+<li><a class="reference internal" href="#dogpile.cache.region.RegionInvalidationStrategy.invalidate"><code class="docutils literal notranslate"><span class="pre">RegionInvalidationStrategy.invalidate()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.region.RegionInvalidationStrategy.is_hard_invalidated"><code class="docutils literal notranslate"><span class="pre">RegionInvalidationStrategy.is_hard_invalidated()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.region.RegionInvalidationStrategy.is_invalidated"><code class="docutils literal notranslate"><span class="pre">RegionInvalidationStrategy.is_invalidated()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.region.RegionInvalidationStrategy.is_soft_invalidated"><code class="docutils literal notranslate"><span class="pre">RegionInvalidationStrategy.is_soft_invalidated()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.region.RegionInvalidationStrategy.was_hard_invalidated"><code class="docutils literal notranslate"><span class="pre">RegionInvalidationStrategy.was_hard_invalidated()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.region.RegionInvalidationStrategy.was_soft_invalidated"><code class="docutils literal notranslate"><span class="pre">RegionInvalidationStrategy.was_soft_invalidated()</span></code></a></li>
+</ul>
+</li>
+<li><a class="reference internal" href="#dogpile.cache.region.make_region"><code class="docutils literal notranslate"><span class="pre">make_region()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.region.value_version"><code class="docutils literal notranslate"><span class="pre">value_version</span></code></a></li>
+</ul>
+</li>
+<li><a class="reference internal" href="#backend-api">Backend API</a><ul>
+<li><a class="reference internal" href="#dogpile.cache.api.BackendFormatted"><code class="docutils literal notranslate"><span class="pre">BackendFormatted</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.api.BackendSetType"><code class="docutils literal notranslate"><span class="pre">BackendSetType</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.api.BytesBackend"><code class="docutils literal notranslate"><span class="pre">BytesBackend</span></code></a><ul>
+<li><a class="reference internal" href="#dogpile.cache.api.BytesBackend.get_serialized"><code class="docutils literal notranslate"><span class="pre">BytesBackend.get_serialized()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.api.BytesBackend.get_serialized_multi"><code class="docutils literal notranslate"><span class="pre">BytesBackend.get_serialized_multi()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.api.BytesBackend.set_serialized"><code class="docutils literal notranslate"><span class="pre">BytesBackend.set_serialized()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.api.BytesBackend.set_serialized_multi"><code class="docutils literal notranslate"><span class="pre">BytesBackend.set_serialized_multi()</span></code></a></li>
+</ul>
+</li>
+<li><a class="reference internal" href="#dogpile.cache.api.CacheBackend"><code class="docutils literal notranslate"><span class="pre">CacheBackend</span></code></a><ul>
+<li><a class="reference internal" href="#dogpile.cache.api.CacheBackend.delete"><code class="docutils literal notranslate"><span class="pre">CacheBackend.delete()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.api.CacheBackend.delete_multi"><code class="docutils literal notranslate"><span class="pre">CacheBackend.delete_multi()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.api.CacheBackend.deserializer"><code class="docutils literal notranslate"><span class="pre">CacheBackend.deserializer</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.api.CacheBackend.get"><code class="docutils literal notranslate"><span class="pre">CacheBackend.get()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.api.CacheBackend.get_multi"><code class="docutils literal notranslate"><span class="pre">CacheBackend.get_multi()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.api.CacheBackend.get_mutex"><code class="docutils literal notranslate"><span class="pre">CacheBackend.get_mutex()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.api.CacheBackend.get_serialized"><code class="docutils literal notranslate"><span class="pre">CacheBackend.get_serialized()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.api.CacheBackend.get_serialized_multi"><code class="docutils literal notranslate"><span class="pre">CacheBackend.get_serialized_multi()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.api.CacheBackend.key_mangler"><code class="docutils literal notranslate"><span class="pre">CacheBackend.key_mangler</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.api.CacheBackend.serializer"><code class="docutils literal notranslate"><span class="pre">CacheBackend.serializer</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.api.CacheBackend.set"><code class="docutils literal notranslate"><span class="pre">CacheBackend.set()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.api.CacheBackend.set_multi"><code class="docutils literal notranslate"><span class="pre">CacheBackend.set_multi()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.api.CacheBackend.set_serialized"><code class="docutils literal notranslate"><span class="pre">CacheBackend.set_serialized()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.api.CacheBackend.set_serialized_multi"><code class="docutils literal notranslate"><span class="pre">CacheBackend.set_serialized_multi()</span></code></a></li>
+</ul>
+</li>
+<li><a class="reference internal" href="#dogpile.cache.api.CacheMutex"><code class="docutils literal notranslate"><span class="pre">CacheMutex</span></code></a><ul>
+<li><a class="reference internal" href="#dogpile.cache.api.CacheMutex.acquire"><code class="docutils literal notranslate"><span class="pre">CacheMutex.acquire()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.api.CacheMutex.locked"><code class="docutils literal notranslate"><span class="pre">CacheMutex.locked()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.api.CacheMutex.release"><code class="docutils literal notranslate"><span class="pre">CacheMutex.release()</span></code></a></li>
+</ul>
+</li>
+<li><a class="reference internal" href="#dogpile.cache.api.CacheReturnType"><code class="docutils literal notranslate"><span class="pre">CacheReturnType</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.api.CachedValue"><code class="docutils literal notranslate"><span class="pre">CachedValue</span></code></a><ul>
+<li><a class="reference internal" href="#dogpile.cache.api.CachedValue.metadata"><code class="docutils literal notranslate"><span class="pre">CachedValue.metadata</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.api.CachedValue.payload"><code class="docutils literal notranslate"><span class="pre">CachedValue.payload</span></code></a></li>
+</ul>
+</li>
+<li><a class="reference internal" href="#dogpile.cache.api.CantDeserializeException"><code class="docutils literal notranslate"><span class="pre">CantDeserializeException</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.api.KeyType"><code class="docutils literal notranslate"><span class="pre">KeyType</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.api.NO_VALUE"><code class="docutils literal notranslate"><span class="pre">NO_VALUE</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.api.NoValue"><code class="docutils literal notranslate"><span class="pre">NoValue</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.api.SerializedReturnType"><code class="docutils literal notranslate"><span class="pre">SerializedReturnType</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.api.ValuePayload"><code class="docutils literal notranslate"><span class="pre">ValuePayload</span></code></a></li>
+</ul>
+</li>
 <li><a class="reference internal" href="#module-dogpile.cache.backends.memory">Backends</a><ul>
 <li><a class="reference internal" href="#memory-backends">Memory Backends</a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.memory.MemoryBackend"><code class="docutils literal notranslate"><span class="pre">MemoryBackend</span></code></a><ul>
+<li><a class="reference internal" href="#dogpile.cache.backends.memory.MemoryBackend.delete"><code class="docutils literal notranslate"><span class="pre">MemoryBackend.delete()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.memory.MemoryBackend.delete_multi"><code class="docutils literal notranslate"><span class="pre">MemoryBackend.delete_multi()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.memory.MemoryBackend.get"><code class="docutils literal notranslate"><span class="pre">MemoryBackend.get()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.memory.MemoryBackend.get_multi"><code class="docutils literal notranslate"><span class="pre">MemoryBackend.get_multi()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.memory.MemoryBackend.set"><code class="docutils literal notranslate"><span class="pre">MemoryBackend.set()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.memory.MemoryBackend.set_multi"><code class="docutils literal notranslate"><span class="pre">MemoryBackend.set_multi()</span></code></a></li>
+</ul>
+</li>
+<li><a class="reference internal" href="#dogpile.cache.backends.memory.MemoryPickleBackend"><code class="docutils literal notranslate"><span class="pre">MemoryPickleBackend</span></code></a></li>
 <li><a class="reference internal" href="#memcached-backends">Memcached Backends</a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.memcached.BMemcachedBackend"><code class="docutils literal notranslate"><span class="pre">BMemcachedBackend</span></code></a><ul>
+<li><a class="reference internal" href="#dogpile.cache.backends.memcached.BMemcachedBackend.delete_multi"><code class="docutils literal notranslate"><span class="pre">BMemcachedBackend.delete_multi()</span></code></a></li>
+</ul>
+</li>
+<li><a class="reference internal" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend"><code class="docutils literal notranslate"><span class="pre">GenericMemcachedBackend</span></code></a><ul>
+<li><a class="reference internal" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend.client"><code class="docutils literal notranslate"><span class="pre">GenericMemcachedBackend.client</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend.delete"><code class="docutils literal notranslate"><span class="pre">GenericMemcachedBackend.delete()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend.delete_multi"><code class="docutils literal notranslate"><span class="pre">GenericMemcachedBackend.delete_multi()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend.deserializer"><code class="docutils literal notranslate"><span class="pre">GenericMemcachedBackend.deserializer</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend.get"><code class="docutils literal notranslate"><span class="pre">GenericMemcachedBackend.get()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend.get_multi"><code class="docutils literal notranslate"><span class="pre">GenericMemcachedBackend.get_multi()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend.get_mutex"><code class="docutils literal notranslate"><span class="pre">GenericMemcachedBackend.get_mutex()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend.serializer"><code class="docutils literal notranslate"><span class="pre">GenericMemcachedBackend.serializer</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend.set"><code class="docutils literal notranslate"><span class="pre">GenericMemcachedBackend.set()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend.set_arguments"><code class="docutils literal notranslate"><span class="pre">GenericMemcachedBackend.set_arguments</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend.set_multi"><code class="docutils literal notranslate"><span class="pre">GenericMemcachedBackend.set_multi()</span></code></a></li>
+</ul>
+</li>
+<li><a class="reference internal" href="#dogpile.cache.backends.memcached.MemcachedBackend"><code class="docutils literal notranslate"><span class="pre">MemcachedBackend</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.memcached.MemcachedLock"><code class="docutils literal notranslate"><span class="pre">MemcachedLock</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.memcached.PyMemcacheBackend"><code class="docutils literal notranslate"><span class="pre">PyMemcacheBackend</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.memcached.PylibmcBackend"><code class="docutils literal notranslate"><span class="pre">PylibmcBackend</span></code></a></li>
 <li><a class="reference internal" href="#redis-backends">Redis Backends</a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.redis.RedisBackend"><code class="docutils literal notranslate"><span class="pre">RedisBackend</span></code></a><ul>
+<li><a class="reference internal" href="#dogpile.cache.backends.redis.RedisBackend.delete"><code class="docutils literal notranslate"><span class="pre">RedisBackend.delete()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.redis.RedisBackend.delete_multi"><code class="docutils literal notranslate"><span class="pre">RedisBackend.delete_multi()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.redis.RedisBackend.get_mutex"><code class="docutils literal notranslate"><span class="pre">RedisBackend.get_mutex()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.redis.RedisBackend.get_serialized"><code class="docutils literal notranslate"><span class="pre">RedisBackend.get_serialized()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.redis.RedisBackend.get_serialized_multi"><code class="docutils literal notranslate"><span class="pre">RedisBackend.get_serialized_multi()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.redis.RedisBackend.set_serialized"><code class="docutils literal notranslate"><span class="pre">RedisBackend.set_serialized()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.redis.RedisBackend.set_serialized_multi"><code class="docutils literal notranslate"><span class="pre">RedisBackend.set_serialized_multi()</span></code></a></li>
+</ul>
+</li>
+<li><a class="reference internal" href="#dogpile.cache.backends.redis.RedisSentinelBackend"><code class="docutils literal notranslate"><span class="pre">RedisSentinelBackend</span></code></a></li>
 <li><a class="reference internal" href="#file-backends">File Backends</a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.file.AbstractFileLock"><code class="docutils literal notranslate"><span class="pre">AbstractFileLock</span></code></a><ul>
+<li><a class="reference internal" href="#dogpile.cache.backends.file.AbstractFileLock.acquire"><code class="docutils literal notranslate"><span class="pre">AbstractFileLock.acquire()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.file.AbstractFileLock.acquire_read_lock"><code class="docutils literal notranslate"><span class="pre">AbstractFileLock.acquire_read_lock()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.file.AbstractFileLock.acquire_write_lock"><code class="docutils literal notranslate"><span class="pre">AbstractFileLock.acquire_write_lock()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.file.AbstractFileLock.is_open"><code class="docutils literal notranslate"><span class="pre">AbstractFileLock.is_open</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.file.AbstractFileLock.read"><code class="docutils literal notranslate"><span class="pre">AbstractFileLock.read()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.file.AbstractFileLock.release"><code class="docutils literal notranslate"><span class="pre">AbstractFileLock.release()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.file.AbstractFileLock.release_read_lock"><code class="docutils literal notranslate"><span class="pre">AbstractFileLock.release_read_lock()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.file.AbstractFileLock.release_write_lock"><code class="docutils literal notranslate"><span class="pre">AbstractFileLock.release_write_lock()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.file.AbstractFileLock.write"><code class="docutils literal notranslate"><span class="pre">AbstractFileLock.write()</span></code></a></li>
+</ul>
+</li>
+<li><a class="reference internal" href="#dogpile.cache.backends.file.DBMBackend"><code class="docutils literal notranslate"><span class="pre">DBMBackend</span></code></a><ul>
+<li><a class="reference internal" href="#dogpile.cache.backends.file.DBMBackend.delete"><code class="docutils literal notranslate"><span class="pre">DBMBackend.delete()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.file.DBMBackend.delete_multi"><code class="docutils literal notranslate"><span class="pre">DBMBackend.delete_multi()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.file.DBMBackend.get_mutex"><code class="docutils literal notranslate"><span class="pre">DBMBackend.get_mutex()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.file.DBMBackend.get_serialized"><code class="docutils literal notranslate"><span class="pre">DBMBackend.get_serialized()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.file.DBMBackend.get_serialized_multi"><code class="docutils literal notranslate"><span class="pre">DBMBackend.get_serialized_multi()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.file.DBMBackend.set_serialized"><code class="docutils literal notranslate"><span class="pre">DBMBackend.set_serialized()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.file.DBMBackend.set_serialized_multi"><code class="docutils literal notranslate"><span class="pre">DBMBackend.set_serialized_multi()</span></code></a></li>
+</ul>
+</li>
+<li><a class="reference internal" href="#dogpile.cache.backends.file.FileLock"><code class="docutils literal notranslate"><span class="pre">FileLock</span></code></a><ul>
+<li><a class="reference internal" href="#dogpile.cache.backends.file.FileLock.acquire_read_lock"><code class="docutils literal notranslate"><span class="pre">FileLock.acquire_read_lock()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.file.FileLock.acquire_write_lock"><code class="docutils literal notranslate"><span class="pre">FileLock.acquire_write_lock()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.file.FileLock.is_open"><code class="docutils literal notranslate"><span class="pre">FileLock.is_open</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.file.FileLock.release_read_lock"><code class="docutils literal notranslate"><span class="pre">FileLock.release_read_lock()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.file.FileLock.release_write_lock"><code class="docutils literal notranslate"><span class="pre">FileLock.release_write_lock()</span></code></a></li>
+</ul>
+</li>
 <li><a class="reference internal" href="#proxy-backends">Proxy Backends</a></li>
+<li><a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend"><code class="docutils literal notranslate"><span class="pre">ProxyBackend</span></code></a><ul>
+<li><a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend.delete"><code class="docutils literal notranslate"><span class="pre">ProxyBackend.delete()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend.delete_multi"><code class="docutils literal notranslate"><span class="pre">ProxyBackend.delete_multi()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend.get"><code class="docutils literal notranslate"><span class="pre">ProxyBackend.get()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend.get_multi"><code class="docutils literal notranslate"><span class="pre">ProxyBackend.get_multi()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend.get_mutex"><code class="docutils literal notranslate"><span class="pre">ProxyBackend.get_mutex()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend.get_serialized"><code class="docutils literal notranslate"><span class="pre">ProxyBackend.get_serialized()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend.get_serialized_multi"><code class="docutils literal notranslate"><span class="pre">ProxyBackend.get_serialized_multi()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend.set"><code class="docutils literal notranslate"><span class="pre">ProxyBackend.set()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend.set_multi"><code class="docutils literal notranslate"><span class="pre">ProxyBackend.set_multi()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend.set_serialized"><code class="docutils literal notranslate"><span class="pre">ProxyBackend.set_serialized()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend.set_serialized_multi"><code class="docutils literal notranslate"><span class="pre">ProxyBackend.set_serialized_multi()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend.wrap"><code class="docutils literal notranslate"><span class="pre">ProxyBackend.wrap()</span></code></a></li>
+</ul>
+</li>
 <li><a class="reference internal" href="#null-backend">Null Backend</a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.null.NullBackend"><code class="docutils literal notranslate"><span class="pre">NullBackend</span></code></a><ul>
+<li><a class="reference internal" href="#dogpile.cache.backends.null.NullBackend.delete"><code class="docutils literal notranslate"><span class="pre">NullBackend.delete()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.null.NullBackend.delete_multi"><code class="docutils literal notranslate"><span class="pre">NullBackend.delete_multi()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.null.NullBackend.get"><code class="docutils literal notranslate"><span class="pre">NullBackend.get()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.null.NullBackend.get_multi"><code class="docutils literal notranslate"><span class="pre">NullBackend.get_multi()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.null.NullBackend.get_mutex"><code class="docutils literal notranslate"><span class="pre">NullBackend.get_mutex()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.null.NullBackend.set"><code class="docutils literal notranslate"><span class="pre">NullBackend.set()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.backends.null.NullBackend.set_multi"><code class="docutils literal notranslate"><span class="pre">NullBackend.set_multi()</span></code></a></li>
+</ul>
+</li>
+</ul>
+</li>
+<li><a class="reference internal" href="#module-dogpile.cache.exception">Exceptions</a><ul>
+<li><a class="reference internal" href="#dogpile.cache.exception.DogpileCacheException"><code class="docutils literal notranslate"><span class="pre">DogpileCacheException</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.exception.PluginNotFound"><code class="docutils literal notranslate"><span class="pre">PluginNotFound</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.exception.RegionAlreadyConfigured"><code class="docutils literal notranslate"><span class="pre">RegionAlreadyConfigured</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.exception.RegionNotConfigured"><code class="docutils literal notranslate"><span class="pre">RegionNotConfigured</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.exception.ValidationError"><code class="docutils literal notranslate"><span class="pre">ValidationError</span></code></a></li>
 </ul>
 </li>
-<li><a class="reference internal" href="#module-dogpile.cache.exception">Exceptions</a></li>
 <li><a class="reference internal" href="#module-dogpile.cache.plugins.mako_cache">Plugins</a><ul>
 <li><a class="reference internal" href="#mako-integration">Mako Integration</a></li>
+<li><a class="reference internal" href="#dogpile.cache.plugins.mako_cache.MakoPlugin"><code class="docutils literal notranslate"><span class="pre">MakoPlugin</span></code></a><ul>
+<li><a class="reference internal" href="#dogpile.cache.plugins.mako_cache.MakoPlugin.get"><code class="docutils literal notranslate"><span class="pre">MakoPlugin.get()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.plugins.mako_cache.MakoPlugin.get_or_create"><code class="docutils literal notranslate"><span class="pre">MakoPlugin.get_or_create()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.plugins.mako_cache.MakoPlugin.invalidate"><code class="docutils literal notranslate"><span class="pre">MakoPlugin.invalidate()</span></code></a></li>
+</ul>
+</li>
+</ul>
+</li>
+<li><a class="reference internal" href="#utilities">Utilities</a><ul>
+<li><a class="reference internal" href="#dogpile.cache.util.function_key_generator"><code class="docutils literal notranslate"><span class="pre">function_key_generator()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.util.kwarg_function_key_generator"><code class="docutils literal notranslate"><span class="pre">kwarg_function_key_generator()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.util.sha1_mangle_key"><code class="docutils literal notranslate"><span class="pre">sha1_mangle_key()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.cache.util.length_conditional_mangler"><code class="docutils literal notranslate"><span class="pre">length_conditional_mangler()</span></code></a></li>
+</ul>
+</li>
+<li><a class="reference internal" href="#dogpile-core">dogpile Core</a><ul>
+<li><a class="reference internal" href="#dogpile.Lock"><code class="docutils literal notranslate"><span class="pre">Lock</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.NeedRegenerationException"><code class="docutils literal notranslate"><span class="pre">NeedRegenerationException</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.util.ReadWriteMutex"><code class="docutils literal notranslate"><span class="pre">ReadWriteMutex</span></code></a><ul>
+<li><a class="reference internal" href="#dogpile.util.ReadWriteMutex.acquire_read_lock"><code class="docutils literal notranslate"><span class="pre">ReadWriteMutex.acquire_read_lock()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.util.ReadWriteMutex.acquire_write_lock"><code class="docutils literal notranslate"><span class="pre">ReadWriteMutex.acquire_write_lock()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.util.ReadWriteMutex.release_read_lock"><code class="docutils literal notranslate"><span class="pre">ReadWriteMutex.release_read_lock()</span></code></a></li>
+<li><a class="reference internal" href="#dogpile.util.ReadWriteMutex.release_write_lock"><code class="docutils literal notranslate"><span class="pre">ReadWriteMutex.release_write_lock()</span></code></a></li>
+</ul>
+</li>
+<li><a class="reference internal" href="#dogpile.util.NameRegistry"><code class="docutils literal notranslate"><span class="pre">NameRegistry</span></code></a><ul>
+<li><a class="reference internal" href="#dogpile.util.NameRegistry.get"><code class="docutils literal notranslate"><span class="pre">NameRegistry.get()</span></code></a></li>
+</ul>
+</li>
 </ul>
 </li>
-<li><a class="reference internal" href="#utilities">Utilities</a></li>
-<li><a class="reference internal" href="#dogpile-core">dogpile Core</a></li>
 </ul>
 </li>
 </ul>
 
   </div>
 <div id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
@@ -4118,17 +4357,17 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="changelog.html" title="Changelog"
              >next</a> |</li>
         <li class="right" >
           <a href="core_usage.html" title="dogpile Core"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.1.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.0 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">API</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2011-2022 Mike Bayer.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 5.0.2.
+        &#169; Copyright 2011-2023 Mike Bayer.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.2.1.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -8,45 +8,43 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * dogpile.cache_1.1.8_documentation »
+    * dogpile.cache_1.2.0_documentation »
     * API
 ****** APIÂ¶ ******
 ***** RegionÂ¶ *****
-  classdogpile.cache.region.CacheRegion(name: ~typing.Optional[str] = None,
+  classdogpile.cache.region.CacheRegion(name: str | None = None,
   function_key_generator: ~typing.Callable[[...], ~typing.Callable[[...], str]]
   = <function function_key_generator>, function_multi_key_generator:
   ~typing.Callable[[...], ~typing.Callable[[...], ~typing.Sequence[str]]] =
-  <function function_multi_key_generator>, key_mangler: ~typing.Optional
-  [~typing.Callable[[str], str]] = None, serializer: ~typing.Optional
-  [~typing.Callable[[~typing.Any], bytes]] = None, deserializer:
-  ~typing.Optional[~typing.Callable[[bytes], ~typing.Any]] = None,
-  async_creation_runner: ~typing.Optional[~typing.Callable[
-  [~dogpile.cache.region.CacheRegion, str, ~typing.Callable[[], ~typing.Any],
-  ~dogpile.cache.api.CacheMutex], None]] = None)Â¶
+  <function function_multi_key_generator>, key_mangler: ~typing.Callable[[str],
+  str] | None = None, serializer: ~typing.Callable[[~typing.Any], bytes] | None
+  = None, deserializer: ~typing.Callable[[bytes], ~typing.Any] | None = None,
+  async_creation_runner: ~typing.Callable[[~dogpile.cache.region.CacheRegion,
+  str, ~typing.Callable[[], ~typing.Any], ~dogpile.cache.api.CacheMutex], None]
+  | None = None)Â¶
       Bases: object
       A front end to a particular cache backend.
         propertyactual_backendÂ¶
             Return the ultimate backend underneath any proxies.
             The backend might be the result of one or more proxy.wrap
             applications. If so, derive the actual underlying backend.
             New in version 0.6.6.
-        cache_multi_on_arguments(namespace: ~typing.Optional[str] = None,
-        expiration_time: ~typing.Optional[~typing.Union[float, ~typing.Callable
-        [[], float]]] = None, should_cache_fn: ~typing.Optional
-        [~typing.Callable[[~typing.Any], bool]] = None, asdict: bool = False,
-        to_str: ~typing.Callable[[~typing.Any], str] = <class 'str'>,
-        function_multi_key_generator: ~typing.Optional[~typing.Callable[[...],
-        ~typing.Callable[[...], ~typing.Sequence[str]]]] = None) &#x2192;
-        Callable[[Callable[[...], Sequence[Any]]], Callable[[...], Union
-        [Sequence[Any], Mapping[str, Any]]]]Â¶
+        cache_multi_on_arguments(namespace: str | None = None, expiration_time:
+        float | ~typing.Callable[[], float] | None = None, should_cache_fn:
+        ~typing.Callable[[~typing.Any], bool] | None = None, asdict: bool =
+        False, to_str: ~typing.Callable[[~typing.Any], str] = <class 'str'>,
+        function_multi_key_generator: ~typing.Callable[[...], ~typing.Callable[
+        [...], ~typing.Sequence[str]]] | None = None) &#x2192; Callable[
+        [Callable[[...], Sequence[Any]]], Callable[[...], Sequence[Any] |
+        Mapping[str, Any]]]Â¶
             A function decorator that will cache multiple return values from
             the function using a sequence of keys derived from the function
             itself and the arguments passed to it.
             This method is the âmultiple keyâ analogue to the
             CacheRegion.cache_on_arguments() method.
             Example:
             @someregion.cache_multi_on_arguments()
@@ -94,22 +92,21 @@
             Parameters passed to CacheRegion.cache_multi_on_arguments() have
             the same meaning as those passed to CacheRegion.cache_on_arguments
             ().
             New in version 0.5.0.
             See also
             CacheRegion.cache_on_arguments()
             CacheRegion.get_or_create_multi()
-        cache_on_arguments(namespace: ~typing.Optional[str] = None,
-        expiration_time: ~typing.Optional[~typing.Union[float, ~typing.Callable
-        [[], float]]] = None, should_cache_fn: ~typing.Optional
-        [~typing.Callable[[~typing.Any], bool]] = None, to_str:
+        cache_on_arguments(namespace: str | None = None, expiration_time: float
+        | ~typing.Callable[[], float] | None = None, should_cache_fn:
+        ~typing.Callable[[~typing.Any], bool] | None = None, to_str:
         ~typing.Callable[[~typing.Any], str] = <class 'str'>,
-        function_key_generator: ~typing.Optional[~typing.Callable[[...],
-        ~typing.Callable[[...], str]]] = None) &#x2192; Callable[[Callable[
-        [...], Any]], Callable[[...], Any]]Â¶
+        function_key_generator: ~typing.Callable[[...], ~typing.Callable[[...],
+        str]] | None = None) &#x2192; Callable[[Callable[[...], Any]], Callable
+        [[...], Any]]Â¶
             A function decorator that will cache the return value of the
             function using a key derived from the function itself and its
             arguments.
             The decorator internally makes use of the CacheRegion.get_or_create
             () method to access the cache and conditionally call the function.
             See that method for additional behavioral details.
             E.g.:
@@ -189,21 +186,20 @@
             The function key generation can be entirely replaced on a per-
             region basis using the function_key_generator argument present on
             make_region() and CacheRegion. If defaults to
             function_key_generator().
             See also
             CacheRegion.cache_multi_on_arguments()
             CacheRegion.get_or_create()
-        configure(backend: str, expiration_time: Optional[Union[float,
-        timedelta]] = None, arguments: Optional[Mapping[str, Any]] = None,
-        _config_argument_dict: Optional[Mapping[str, Any]] = None,
-        _config_prefix: Optional[str] = None, wrap: Sequence[Union
-        [ProxyBackend, Type[ProxyBackend]]] = (), replace_existing_backend:
-        bool = False, region_invalidator: Optional[RegionInvalidationStrategy]
-        = None) &#x2192; CacheRegionÂ¶
+        configure(backend: str, expiration_time: float | timedelta | None =
+        None, arguments: Mapping[str, Any] | None = None,
+        _config_argument_dict: Mapping[str, Any] | None = None, _config_prefix:
+        str | None = None, wrap: Sequence[ProxyBackend | Type[ProxyBackend]] =
+        (), replace_existing_backend: bool = False, region_invalidator:
+        RegionInvalidationStrategy | None = None) &#x2192; CacheRegionÂ¶
             Configure a CacheRegion.
             The CacheRegion itself is returned.
         configure_from_config(config_dict, prefix)Â¶
             Configure from a configuration dictionary and a prefix.
             Example:
             local_region = make_region()
             memcached_region = make_region()
@@ -274,17 +270,17 @@
             argument, is tested against the creation time of the retrieved
             value versus the current time (as reported by time.time()). If
             stale, the cached value is ignored and the NO_VALUE token is
             returned. Passing the flag ignore_expiration=True bypasses the
             expiration time check.
             New in version 0.5.0.
         get_or_create(key: str, creator: Callable[[...], Any], expiration_time:
-        Optional[float] = None, should_cache_fn: Optional[Callable[[Any],
-        bool]] = None, creator_args: Optional[Tuple[Any, Mapping[str, Any]]] =
-        None) &#x2192; AnyÂ¶
+        float | None = None, should_cache_fn: Callable[[Any], bool] | None =
+        None, creator_args: Tuple[Any, Mapping[str, Any]] | None = None)
+        &#x2192; AnyÂ¶
             Return a cached value based on the given key.
             If the value does not exist or is considered to be expired based on
             its creation time, the given creation function may or may not be
             used to recreate the value and persist the newly generated value in
             the cache.
             Whether or not the function is used depends on if the dogpile lock
             can be acquired or not. If it canât, it means a different thread
@@ -302,31 +298,31 @@
             if the creation time is older than the last call to invalidate().
             See also
             CacheRegion.get()
             CacheRegion.cache_on_arguments() - applies get_or_create() to any
             function using a decorator.
             CacheRegion.get_or_create_multi() - multiple key/value version
         get_or_create_multi(keys: Sequence[str], creator: Callable[[], Any],
-        expiration_time: Optional[float] = None, should_cache_fn: Optional
-        [Callable[[Any], bool]] = None) &#x2192; Sequence[Any]Â¶
+        expiration_time: float | None = None, should_cache_fn: Callable[[Any],
+        bool] | None = None) &#x2192; Sequence[Any]Â¶
             Return a sequence of cached values based on a sequence of keys.
             The behavior for generation of values based on keys corresponds to
             that of Region.get_or_create(), with the exception that the creator
             () function may be asked to generate any subset of the given keys.
             The list of keys to be generated is passed to creator(), and
             creator() should return the generated values as a sequence
             corresponding to the order of the keys.
             The method uses the same approach as Region.get_multi() and
             Region.set_multi() to get and set values from the backend.
             If you are using a CacheBackend or ProxyBackend that modifies
             values, take note this function invokes .set_multi() for newly
             generated values using the same values it returns to the calling
             function. A correct implementation of .set_multi() will not modify
             values in-place on the submitted mapping dict.
-              Parameters
+              Parameters:
                       * keysÂ¶ â Sequence of keys to be retrieved.
                       * creatorÂ¶ â function which accepts a sequence of keys
                         and returns a sequence of new values.
                       * expiration_timeÂ¶ â optional expiration time which
                         will override the expiration time already configured on
                         this CacheRegion if not None. To set no expiration, use
                         the value -1.
@@ -374,46 +370,46 @@
             Return True if a particular cache key is currently being generated
             within the dogpile lock.
             New in version 1.1.2.
         set(key: str, value: Any) &#x2192; NoneÂ¶
             Place a new value in the cache under the given key.
         set_multi(mapping: Mapping[str, Any]) &#x2192; NoneÂ¶
             Place new values in the cache under the given keys.
-        wrap(proxy: Union[ProxyBackend, Type[ProxyBackend]]) &#x2192; NoneÂ¶
+        wrap(proxy: ProxyBackend | Type[ProxyBackend]) &#x2192; NoneÂ¶
             Takes a ProxyBackend instance or class and wraps the attached
             backend.
   classdogpile.cache.region.DefaultInvalidationStrategyÂ¶
       Bases: RegionInvalidationStrategy
         invalidate(hard: bool = True) &#x2192; NoneÂ¶
             Region invalidation.
             CacheRegion propagated call. The default invalidation system works
             by setting a current timestamp (using time.time()) to consider all
             older timestamps effectively invalidated.
         is_hard_invalidated(timestamp: float) &#x2192; boolÂ¶
             Check timestamp to determine if it was hard invalidated.
-              Returns
+              Returns:
                   Boolean. True if timestamp is older than the last region
                   invalidation time and region is invalidated in hard mode.
         is_invalidated(timestamp: float) &#x2192; boolÂ¶
             Check timestamp to determine if it was invalidated.
-              Returns
+              Returns:
                   Boolean. True if timestamp is older than the last region
                   invalidation time.
         is_soft_invalidated(timestamp: float) &#x2192; boolÂ¶
             Check timestamp to determine if it was soft invalidated.
-              Returns
+              Returns:
                   Boolean. True if timestamp is older than the last region
                   invalidation time and region is invalidated in soft mode.
         was_hard_invalidated() &#x2192; boolÂ¶
             Indicate the region was invalidated in hard mode.
-              Returns
+              Returns:
                   Boolean. True if region was invalidated in hard mode.
         was_soft_invalidated() &#x2192; boolÂ¶
             Indicate the region was invalidated in soft mode.
-              Returns
+              Returns:
                   Boolean. True if region was invalidated in soft mode.
   classdogpile.cache.region.RegionInvalidationStrategyÂ¶
       Bases: object
       Region invalidation strategy interface
       Implement this interface and pass implementation instance to
       CacheRegion.configure() to override default region invalidation.
       Example:
@@ -473,34 +469,34 @@
         invalidate(hard: bool = True) &#x2192; NoneÂ¶
             Region invalidation.
             CacheRegion propagated call. The default invalidation system works
             by setting a current timestamp (using time.time()) to consider all
             older timestamps effectively invalidated.
         is_hard_invalidated(timestamp: float) &#x2192; boolÂ¶
             Check timestamp to determine if it was hard invalidated.
-              Returns
+              Returns:
                   Boolean. True if timestamp is older than the last region
                   invalidation time and region is invalidated in hard mode.
         is_invalidated(timestamp: float) &#x2192; boolÂ¶
             Check timestamp to determine if it was invalidated.
-              Returns
+              Returns:
                   Boolean. True if timestamp is older than the last region
                   invalidation time.
         is_soft_invalidated(timestamp: float) &#x2192; boolÂ¶
             Check timestamp to determine if it was soft invalidated.
-              Returns
+              Returns:
                   Boolean. True if timestamp is older than the last region
                   invalidation time and region is invalidated in soft mode.
         was_hard_invalidated() &#x2192; boolÂ¶
             Indicate the region was invalidated in hard mode.
-              Returns
+              Returns:
                   Boolean. True if region was invalidated in hard mode.
         was_soft_invalidated() &#x2192; boolÂ¶
             Indicate the region was invalidated in soft mode.
-              Returns
+              Returns:
                   Boolean. True if region was invalidated in soft mode.
   dogpile.cache.region.make_region(*arg: Any, **kw: Any) &#x2192; CacheRegionÂ¶
       Instantiate a new CacheRegion.
       Currently, make_region() is a passthrough to CacheRegion. See that class
       for constructor arguments.
   dogpile.cache.region.value_version= 2Â¶
       An integer placed in the CachedValue so that new versions of
@@ -521,44 +517,44 @@
       Bases: DefaultSerialization, CacheBackend
       A cache backend that receives and returns series of bytes.
       This backend only supports the âserializedâ form of values;
       subclasses should implement BytesBackend.get_serialized(),
       BytesBackend.get_serialized_multi(), BytesBackend.set_serialized(),
       BytesBackend.set_serialized_multi().
       New in version 1.1.
-        get_serialized(key: str) &#x2192; Union[bytes, NoValue]Â¶
+        get_serialized(key: str) &#x2192; bytes | NoValueÂ¶
             Retrieve a serialized value from the cache.
-              Parameters
+              Parameters:
                   keyÂ¶ â String key that was passed to the CacheRegion.get()
                   method, which will also be processed by the âkey
                   manglingâ function if one was present.
-              Returns
+              Returns:
                   a bytes object, or NO_VALUE constant if not present.
             New in version 1.1.
-        get_serialized_multi(keys: Sequence[str]) &#x2192; Sequence[Union
-        [bytes, NoValue]]Â¶
+        get_serialized_multi(keys: Sequence[str]) &#x2192; Sequence[bytes |
+        NoValue]Â¶
             Retrieve multiple serialized values from the cache.
-              Parameters
+              Parameters:
                   keysÂ¶ â sequence of string keys that was passed to the
                   CacheRegion.get_multi() method, which will also be processed
                   by the âkey manglingâ function if one was present.
-              Returns
+              Returns:
                   list of bytes objects
             New in version 1.1.
         set_serialized(key: str, value: bytes) &#x2192; NoneÂ¶
             Set a serialized value in the cache.
-              Parameters
+              Parameters:
                       * keyÂ¶ â String key that was passed to the
                         CacheRegion.set() method, which will also be processed
                         by the âkey manglingâ function if one was present.
                       * valueÂ¶ â a bytes object to be stored.
             New in version 1.1.
         set_serialized_multi(mapping: Mapping[str, bytes]) &#x2192; NoneÂ¶
             Set multiple serialized values in the cache.
-              Parameters
+              Parameters:
                   mappingÂ¶ â a dict in which the key will be whatever was
                   passed to the CacheRegion.set_multi() method, processed by
                   the âkey manglingâ function, if any.
             When implementing a new CacheBackend or cutomizing via
             ProxyBackend, be aware that when this method is invoked by
             Region.get_or_create_multi(), the mapping values are the same ones
             returned to the upstream caller. If the subclass alters the values
@@ -570,60 +566,60 @@
       Bases: object
       Base class for backend implementations.
       Backends which set and get Python object values should subclass this
       backend. For backends in which the value thatâs stored is ultimately a
       stream of bytes, the BytesBackend should be used.
         delete(key: str) &#x2192; NoneÂ¶
             Delete a value from the cache.
-              Parameters
+              Parameters:
                   keyÂ¶ â String key that was passed to the
                   CacheRegion.delete() method, which will also be processed by
                   the âkey manglingâ function if one was present.
             The behavior here should be idempotent, that is, can be called any
             number of times regardless of whether or not the key exists.
         delete_multi(keys: Sequence[str]) &#x2192; NoneÂ¶
             Delete multiple values from the cache.
-              Parameters
+              Parameters:
                   keysÂ¶ â sequence of string keys that was passed to the
                   CacheRegion.delete_multi() method, which will also be
                   processed by the âkey manglingâ function if one was
                   present.
             The behavior here should be idempotent, that is, can be called any
             number of times regardless of whether or not the key exists.
             New in version 0.5.0.
-        deserializer: Union[None, Callable[[bytes], Any]]= NoneÂ¶
+        deserializer: None | Callable[[bytes], Any]= NoneÂ¶
             deserializer function that will be used by default if not
             overridden by the region.
             New in version 1.1.
-        get(key: str) &#x2192; Union[CachedValue, NoValue, bytes]Â¶
+        get(key: str) &#x2192; CachedValue | NoValue | bytesÂ¶
             Retrieve an optionally serialized value from the cache.
-              Parameters
+              Parameters:
                   keyÂ¶ â String key that was passed to the CacheRegion.get()
                   method, which will also be processed by the âkey
                   manglingâ function if one was present.
-              Returns
+              Returns:
                   the Python object that corresponds to what was established
                   via the CacheBackend.set() method, or the NO_VALUE constant
                   if not present.
             If a serializer is in use, this method will only be called if the
             CacheBackend.get_serialized() method is not overridden.
-        get_multi(keys: Sequence[str]) &#x2192; Sequence[Union[CachedValue,
-        NoValue, bytes]]Â¶
+        get_multi(keys: Sequence[str]) &#x2192; Sequence[CachedValue | NoValue
+        | bytes]Â¶
             Retrieve multiple optionally serialized values from the cache.
-              Parameters
+              Parameters:
                   keysÂ¶ â sequence of string keys that was passed to the
                   CacheRegion.get_multi() method, which will also be processed
                   by the âkey manglingâ function if one was present.
               :return a list of values as would be returned
                   individually via the CacheBackend.get() method, corresponding
                   to the list of keys given.
             If a serializer is in use, this method will only be called if the
             CacheBackend.get_serialized_multi() method is not overridden.
             New in version 0.5.0.
-        get_mutex(key: str) &#x2192; Optional[CacheMutex]Â¶
+        get_mutex(key: str) &#x2192; CacheMutex | NoneÂ¶
             Return an optional mutexing object for the given key.
             This object need only provide an acquire() and release() method.
             May return None, in which case the dogpile lock will use a regular
             threading.Lock object to mutex concurrent threads for value
             creation. The default implementation returns None.
             Different backends may want to provide various kinds of âmutexâ
             objects, such as those which link to lock files, distributed
@@ -632,65 +628,64 @@
             A mutex that takes the key into account will allow multiple
             regenerate operations across keys to proceed simultaneously, while
             a mutex that does not will serialize regenerate operations to just
             one at a time across all keys in the region. The latter approach,
             or a variant that involves a modulus of the given keyâs hash
             value, can be used as a means of throttling the total number of
             value recreation operations that may proceed at one time.
-        get_serialized(key: str) &#x2192; Union[bytes, NoValue]Â¶
+        get_serialized(key: str) &#x2192; bytes | NoValueÂ¶
             Retrieve a serialized value from the cache.
-              Parameters
+              Parameters:
                   keyÂ¶ â String key that was passed to the CacheRegion.get()
                   method, which will also be processed by the âkey
                   manglingâ function if one was present.
-              Returns
+              Returns:
                   a bytes object, or NO_VALUE constant if not present.
             The default implementation of this method for CacheBackend returns
             the value of the CacheBackend.get() method.
             New in version 1.1.
             See also
             BytesBackend
-        get_serialized_multi(keys: Sequence[str]) &#x2192; Sequence[Union
-        [bytes, NoValue]]Â¶
+        get_serialized_multi(keys: Sequence[str]) &#x2192; Sequence[bytes |
+        NoValue]Â¶
             Retrieve multiple serialized values from the cache.
-              Parameters
+              Parameters:
                   keysÂ¶ â sequence of string keys that was passed to the
                   CacheRegion.get_multi() method, which will also be processed
                   by the âkey manglingâ function if one was present.
-              Returns
+              Returns:
                   list of bytes objects
             The default implementation of this method for CacheBackend returns
             the value of the CacheBackend.get_multi() method.
             New in version 1.1.
             See also
             BytesBackend
-        key_mangler: Optional[Callable[[str], str]]= NoneÂ¶
+        key_mangler: Callable[[str], str] | None= NoneÂ¶
             Key mangling function.
             May be None, or otherwise declared as an ordinary instance method.
-        serializer: Union[None, Callable[[Any], bytes]]= NoneÂ¶
+        serializer: None | Callable[[Any], bytes]= NoneÂ¶
             Serializer function that will be used by default if not overridden
             by the region.
             New in version 1.1.
-        set(key: str, value: Union[CachedValue, bytes]) &#x2192; NoneÂ¶
+        set(key: str, value: CachedValue | bytes) &#x2192; NoneÂ¶
             Set an optionally serialized value in the cache.
-              Parameters
+              Parameters:
                       * keyÂ¶ â String key that was passed to the
                         CacheRegion.set() method, which will also be processed
                         by the âkey manglingâ function if one was present.
                       * valueÂ¶ â The optionally serialized CachedValue
                         object. May be an instance of CachedValue or a bytes
                         object depending on if a serializer is in use with the
                         region and if the CacheBackend.set_serialized() method
                         is not overridden.
             See also
             CacheBackend.set_serialized()
-        set_multi(mapping: Mapping[str, Union[CachedValue, bytes]]) &#x2192;
-        NoneÂ¶
+        set_multi(mapping: Mapping[str, CachedValue | bytes]) &#x2192; NoneÂ¶
             Set multiple values in the cache.
-              Parameters
+              Parameters:
                   mappingÂ¶ â a dict in which the key will be whatever was
                   passed to the CacheRegion.set_multi() method, processed by
                   the âkey manglingâ function, if any.
             When implementing a new CacheBackend or cutomizing via
             ProxyBackend, be aware that when this method is invoked by
             Region.get_or_create_multi(), the mapping values are the same ones
             returned to the upstream caller. If the subclass alters the values
@@ -698,27 +693,27 @@
             â that will have the undesirable effect of modifying the returned
             values as well.
             If a serializer is in use, this method will only be called if the
             CacheBackend.set_serialized_multi() method is not overridden.
             New in version 0.5.0.
         set_serialized(key: str, value: bytes) &#x2192; NoneÂ¶
             Set a serialized value in the cache.
-              Parameters
+              Parameters:
                       * keyÂ¶ â String key that was passed to the
                         CacheRegion.set() method, which will also be processed
                         by the âkey manglingâ function if one was present.
                       * valueÂ¶ â a bytes object to be stored.
             The default implementation of this method for CacheBackend calls
             upon the CacheBackend.set() method.
             New in version 1.1.
             See also
             BytesBackend
         set_serialized_multi(mapping: Mapping[str, bytes]) &#x2192; NoneÂ¶
             Set multiple serialized values in the cache.
-              Parameters
+              Parameters:
                   mappingÂ¶ â a dict in which the key will be whatever was
                   passed to the CacheRegion.set_multi() method, processed by
                   the âkey manglingâ function, if any.
             When implementing a new CacheBackend or cutomizing via
             ProxyBackend, be aware that when this method is invoked by
             Region.get_or_create_multi(), the mapping values are the same ones
             returned to the upstream caller. If the subclass alters the values
@@ -737,22 +732,22 @@
       methods may be used.
       New in version 1.1.
       See also
       CacheBackend.get_mutex() - the backend method that optionally returns
       this locking object.
         abstractacquire(wait: bool = True) &#x2192; boolÂ¶
             Acquire the mutex.
-              Parameters
+              Parameters:
                   waitÂ¶ â if True, block until available, else return True/
                   False immediately.
-              Returns
+              Returns:
                   True if the lock succeeded.
         abstractlocked() &#x2192; boolÂ¶
             Check if the mutex was acquired.
-              Returns
+              Returns:
                   true if the lock is acquired.
             New in version 1.1.2.
         abstractrelease() &#x2192; NoneÂ¶
             Release the mutex.
   dogpile.cache.api.CacheReturnTypeÂ¶
       The non-serialized form of what may be returned from a backend get
       method.
@@ -763,14 +758,19 @@
       Represent a value stored in the cache.
       CachedValue is a two-tuple of (payload, metadata), where metadata is
       dogpile.cacheâs tracking information ( currently the creation time).
         metadata: Mapping[str, Any]Â¶
             Alias for field number 1
         payload: AnyÂ¶
             Alias for field number 0
+  exceptiondogpile.cache.api.CantDeserializeExceptionÂ¶
+      Bases: Exception
+      Exception indicating deserialization failed, and that caching should
+      proceed to re-generate a value
+      New in version 1.2.0.
   dogpile.cache.api.KeyTypeÂ¶
       A cache key.
   dogpile.cache.api.NO_VALUE= <dogpile.cache.api.NoValue object>Â¶
       Value returned from get() that describes a key not present.
   classdogpile.cache.api.NoValueÂ¶
       Bases: object
       Describe a missing cache value.
@@ -807,70 +807,70 @@
           'dogpile.cache.memory',
           arguments={
               "cache_dict":my_dictionary
           }
       )
         delete(key)Â¶
             Delete a value from the cache.
-              Parameters
+              Parameters:
                   keyÂ¶ â String key that was passed to the
                   CacheRegion.delete() method, which will also be processed by
                   the âkey manglingâ function if one was present.
             The behavior here should be idempotent, that is, can be called any
             number of times regardless of whether or not the key exists.
         delete_multi(keys)Â¶
             Delete multiple values from the cache.
-              Parameters
+              Parameters:
                   keysÂ¶ â sequence of string keys that was passed to the
                   CacheRegion.delete_multi() method, which will also be
                   processed by the âkey manglingâ function if one was
                   present.
             The behavior here should be idempotent, that is, can be called any
             number of times regardless of whether or not the key exists.
             New in version 0.5.0.
         get(key)Â¶
             Retrieve an optionally serialized value from the cache.
-              Parameters
+              Parameters:
                   keyÂ¶ â String key that was passed to the CacheRegion.get()
                   method, which will also be processed by the âkey
                   manglingâ function if one was present.
-              Returns
+              Returns:
                   the Python object that corresponds to what was established
                   via the CacheBackend.set() method, or the NO_VALUE constant
                   if not present.
             If a serializer is in use, this method will only be called if the
             CacheBackend.get_serialized() method is not overridden.
         get_multi(keys)Â¶
             Retrieve multiple optionally serialized values from the cache.
-              Parameters
+              Parameters:
                   keysÂ¶ â sequence of string keys that was passed to the
                   CacheRegion.get_multi() method, which will also be processed
                   by the âkey manglingâ function if one was present.
               :return a list of values as would be returned
                   individually via the CacheBackend.get() method, corresponding
                   to the list of keys given.
             If a serializer is in use, this method will only be called if the
             CacheBackend.get_serialized_multi() method is not overridden.
             New in version 0.5.0.
         set(key, value)Â¶
             Set an optionally serialized value in the cache.
-              Parameters
+              Parameters:
                       * keyÂ¶ â String key that was passed to the
                         CacheRegion.set() method, which will also be processed
                         by the âkey manglingâ function if one was present.
                       * valueÂ¶ â The optionally serialized CachedValue
                         object. May be an instance of CachedValue or a bytes
                         object depending on if a serializer is in use with the
                         region and if the CacheBackend.set_serialized() method
                         is not overridden.
             See also
             CacheBackend.set_serialized()
         set_multi(mapping)Â¶
             Set multiple values in the cache.
-              Parameters
+              Parameters:
                   mappingÂ¶ â a dict in which the key will be whatever was
                   passed to the CacheRegion.set_multi() method, processed by
                   the âkey manglingâ function, if any.
             When implementing a new CacheBackend or cutomizing via
             ProxyBackend, be aware that when this method is invoked by
             Region.get_or_create_multi(), the mapping values are the same ones
             returned to the upstream caller. If the subclass alters the values
@@ -899,15 +899,14 @@
       performance hit in doing so as that of other backends; in this way the
       MemoryPickleBackend performance is somewhere in between that of the pure
       MemoryBackend and the remote server oriented backends such as that of
       Memcached or Redis.
       Pickle behavior here is the same as that of the Redis backend, using
       either cPickle or pickle and specifying HIGHEST_PROTOCOL upon serialize.
       New in version 0.5.3.
-
 **** Memcached BackendsÂ¶ ****
 Provides backends for talking to memcached.
   classdogpile.cache.backends.memcached.BMemcachedBackend(arguments)Â¶
       Bases: GenericMemcachedBackend
       A backend for the python-binary-memcached memcached client.
       This is a pure Python memcached client which includes security features
       like SASL and SSL/TLS.
@@ -956,49 +955,49 @@
       with a particular thread when that thread ends.
         propertyclientÂ¶
             Return the memcached client.
             This uses a threading.local by default as it appears most modern
             memcached libs arenât inherently threadsafe.
         delete(key)Â¶
             Delete a value from the cache.
-              Parameters
+              Parameters:
                   keyÂ¶ â String key that was passed to the
                   CacheRegion.delete() method, which will also be processed by
                   the âkey manglingâ function if one was present.
             The behavior here should be idempotent, that is, can be called any
             number of times regardless of whether or not the key exists.
         delete_multi(keys)Â¶
             Delete multiple values from the cache.
-              Parameters
+              Parameters:
                   keysÂ¶ â sequence of string keys that was passed to the
                   CacheRegion.delete_multi() method, which will also be
                   processed by the âkey manglingâ function if one was
                   present.
             The behavior here should be idempotent, that is, can be called any
             number of times regardless of whether or not the key exists.
             New in version 0.5.0.
-        deserializer: Union[None, Deserializer]= NoneÂ¶
+        deserializer: None | Deserializer= NoneÂ¶
             deserializer function that will be used by default if not
             overridden by the region.
             New in version 1.1.
         get(key)Â¶
             Retrieve an optionally serialized value from the cache.
-              Parameters
+              Parameters:
                   keyÂ¶ â String key that was passed to the CacheRegion.get()
                   method, which will also be processed by the âkey
                   manglingâ function if one was present.
-              Returns
+              Returns:
                   the Python object that corresponds to what was established
                   via the CacheBackend.set() method, or the NO_VALUE constant
                   if not present.
             If a serializer is in use, this method will only be called if the
             CacheBackend.get_serialized() method is not overridden.
         get_multi(keys)Â¶
             Retrieve multiple optionally serialized values from the cache.
-              Parameters
+              Parameters:
                   keysÂ¶ â sequence of string keys that was passed to the
                   CacheRegion.get_multi() method, which will also be processed
                   by the âkey manglingâ function if one was present.
               :return a list of values as would be returned
                   individually via the CacheBackend.get() method, corresponding
                   to the list of keys given.
             If a serializer is in use, this method will only be called if the
@@ -1017,36 +1016,36 @@
             A mutex that takes the key into account will allow multiple
             regenerate operations across keys to proceed simultaneously, while
             a mutex that does not will serialize regenerate operations to just
             one at a time across all keys in the region. The latter approach,
             or a variant that involves a modulus of the given keyâs hash
             value, can be used as a means of throttling the total number of
             value recreation operations that may proceed at one time.
-        serializer: Union[None, Serializer]= NoneÂ¶
+        serializer: None | Serializer= NoneÂ¶
             Serializer function that will be used by default if not overridden
             by the region.
             New in version 1.1.
         set(key, value)Â¶
             Set an optionally serialized value in the cache.
-              Parameters
+              Parameters:
                       * keyÂ¶ â String key that was passed to the
                         CacheRegion.set() method, which will also be processed
                         by the âkey manglingâ function if one was present.
                       * valueÂ¶ â The optionally serialized CachedValue
                         object. May be an instance of CachedValue or a bytes
                         object depending on if a serializer is in use with the
                         region and if the CacheBackend.set_serialized() method
                         is not overridden.
             See also
             CacheBackend.set_serialized()
         set_arguments: Mapping[str, Any]= {}Â¶
             Additional arguments which will be passed to the set() method.
         set_multi(mapping)Â¶
             Set multiple values in the cache.
-              Parameters
+              Parameters:
                   mappingÂ¶ â a dict in which the key will be whatever was
                   passed to the CacheRegion.set_multi() method, processed by
                   the âkey manglingâ function, if any.
             When implementing a new CacheBackend or cutomizing via
             ProxyBackend, be aware that when this method is invoked by
             Region.get_or_create_multi(), the mapping values are the same ones
             returned to the upstream caller. If the subclass alters the values
@@ -1104,22 +1103,21 @@
               'url':["127.0.0.1"],
               'binary':True,
               'behaviors':{"tcp_nodelay": True,"ketama":True}
           }
       )
       Arguments accepted here include those of GenericMemcachedBackend, as well
       as those below.
-        Parameters
+        Parameters:
                 * binaryÂ¶ â sets the binary flag understood by
                   pylibmc.Client.
                 * behaviorsÂ¶ â a dictionary which will be passed to
                   pylibmc.Client as the behaviors parameter.
                 * min_compress_lenÂ¶ â Integer, will be passed as the
                   min_compress_len parameter to the pylibmc.Client.set method.
-
 **** Redis BackendsÂ¶ ****
 Provides backends for talking to Redis.
   classdogpile.cache.backends.redis.RedisBackend(arguments)Â¶
       Bases: BytesBackend
       A Redis backend, using the redis-py backend.
       Example configuration:
       from dogpile.cache import make_region
@@ -1134,23 +1132,23 @@
               'distributed_lock': True,
               'thread_local_lock': False
               }
       )
       Arguments accepted in the arguments dictionary:
         delete(key)Â¶
             Delete a value from the cache.
-              Parameters
+              Parameters:
                   keyÂ¶ â String key that was passed to the
                   CacheRegion.delete() method, which will also be processed by
                   the âkey manglingâ function if one was present.
             The behavior here should be idempotent, that is, can be called any
             number of times regardless of whether or not the key exists.
         delete_multi(keys)Â¶
             Delete multiple values from the cache.
-              Parameters
+              Parameters:
                   keysÂ¶ â sequence of string keys that was passed to the
                   CacheRegion.delete_multi() method, which will also be
                   processed by the âkey manglingâ function if one was
                   present.
             The behavior here should be idempotent, that is, can be called any
             number of times regardless of whether or not the key exists.
             New in version 0.5.0.
@@ -1169,41 +1167,41 @@
             a mutex that does not will serialize regenerate operations to just
             one at a time across all keys in the region. The latter approach,
             or a variant that involves a modulus of the given keyâs hash
             value, can be used as a means of throttling the total number of
             value recreation operations that may proceed at one time.
         get_serialized(key)Â¶
             Retrieve a serialized value from the cache.
-              Parameters
+              Parameters:
                   keyÂ¶ â String key that was passed to the CacheRegion.get()
                   method, which will also be processed by the âkey
                   manglingâ function if one was present.
-              Returns
+              Returns:
                   a bytes object, or NO_VALUE constant if not present.
             New in version 1.1.
         get_serialized_multi(keys)Â¶
             Retrieve multiple serialized values from the cache.
-              Parameters
+              Parameters:
                   keysÂ¶ â sequence of string keys that was passed to the
                   CacheRegion.get_multi() method, which will also be processed
                   by the âkey manglingâ function if one was present.
-              Returns
+              Returns:
                   list of bytes objects
             New in version 1.1.
         set_serialized(key, value)Â¶
             Set a serialized value in the cache.
-              Parameters
+              Parameters:
                       * keyÂ¶ â String key that was passed to the
                         CacheRegion.set() method, which will also be processed
                         by the âkey manglingâ function if one was present.
                       * valueÂ¶ â a bytes object to be stored.
             New in version 1.1.
         set_serialized_multi(mapping)Â¶
             Set multiple serialized values in the cache.
-              Parameters
+              Parameters:
                   mappingÂ¶ â a dict in which the key will be whatever was
                   passed to the CacheRegion.set_multi() method, processed by
                   the âkey manglingâ function, if any.
             When implementing a new CacheBackend or cutomizing via
             ProxyBackend, be aware that when this method is invoked by
             Region.get_or_create_multi(), the mapping values are the same ones
             returned to the upstream caller. If the subclass alters the values
@@ -1229,15 +1227,15 @@
               'db': 0,
               'redis_expiration_time': 60*60*2,   # 2 hours
               'distributed_lock': True,
               'thread_local_lock': False
           }
       )
       Arguments accepted in the arguments dictionary:
-        Parameters
+        Parameters:
                 * dbÂ¶ â integer, default is 0.
                 * redis_expiration_timeÂ¶ â integer, number of seconds after
                   setting a value that Redis should expire it. This should be
                   larger than dogpileâs cache expiration. By default no
                   expiration is set.
                 * distributed_lockÂ¶ â boolean, when True, will use a redis-
                   lock as the dogpile lock. Use this when multiple processes
@@ -1265,15 +1263,14 @@
                 * lock_sleepÂ¶ â integer, number of seconds to sleep when
                   failed to acquire a lock. This argument is only valid when
                   distributed_lock is True.
                 * thread_local_lockÂ¶ â bool, whether a thread-local Redis
                   lock object should be used. This is the default, but is not
                   compatible with asynchronous runners, as they run in a
                   different thread than the one used to create the lock.
-
 **** File BackendsÂ¶ ****
 Provides backends that deal with local filesystem access.
   classdogpile.cache.backends.file.AbstractFileLock(filename)Â¶
       Bases: object
       Coordinate read/write access to a file.
       typically is a file-based lock but doesnât necessarily have to be.
       The default implementation here is FileLock.
@@ -1360,23 +1357,23 @@
       uniquely corresponds to the key is problematic, since itâs not
       generally safe to delete lockfiles as the application runs, implying an
       unlimited number of key-based files would need to be created and never
       deleted.
       Parameters to the arguments dictionary are below.
         delete(key)Â¶
             Delete a value from the cache.
-              Parameters
+              Parameters:
                   keyÂ¶ â String key that was passed to the
                   CacheRegion.delete() method, which will also be processed by
                   the âkey manglingâ function if one was present.
             The behavior here should be idempotent, that is, can be called any
             number of times regardless of whether or not the key exists.
         delete_multi(keys)Â¶
             Delete multiple values from the cache.
-              Parameters
+              Parameters:
                   keysÂ¶ â sequence of string keys that was passed to the
                   CacheRegion.delete_multi() method, which will also be
                   processed by the âkey manglingâ function if one was
                   present.
             The behavior here should be idempotent, that is, can be called any
             number of times regardless of whether or not the key exists.
             New in version 0.5.0.
@@ -1395,41 +1392,41 @@
             a mutex that does not will serialize regenerate operations to just
             one at a time across all keys in the region. The latter approach,
             or a variant that involves a modulus of the given keyâs hash
             value, can be used as a means of throttling the total number of
             value recreation operations that may proceed at one time.
         get_serialized(key)Â¶
             Retrieve a serialized value from the cache.
-              Parameters
+              Parameters:
                   keyÂ¶ â String key that was passed to the CacheRegion.get()
                   method, which will also be processed by the âkey
                   manglingâ function if one was present.
-              Returns
+              Returns:
                   a bytes object, or NO_VALUE constant if not present.
             New in version 1.1.
         get_serialized_multi(keys)Â¶
             Retrieve multiple serialized values from the cache.
-              Parameters
+              Parameters:
                   keysÂ¶ â sequence of string keys that was passed to the
                   CacheRegion.get_multi() method, which will also be processed
                   by the âkey manglingâ function if one was present.
-              Returns
+              Returns:
                   list of bytes objects
             New in version 1.1.
         set_serialized(key, value)Â¶
             Set a serialized value in the cache.
-              Parameters
+              Parameters:
                       * keyÂ¶ â String key that was passed to the
                         CacheRegion.set() method, which will also be processed
                         by the âkey manglingâ function if one was present.
                       * valueÂ¶ â a bytes object to be stored.
             New in version 1.1.
         set_serialized_multi(mapping)Â¶
             Set multiple serialized values in the cache.
-              Parameters
+              Parameters:
                   mappingÂ¶ â a dict in which the key will be whatever was
                   passed to the CacheRegion.set_multi() method, processed by
                   the âkey manglingâ function, if any.
             When implementing a new CacheBackend or cutomizing via
             ProxyBackend, be aware that when this method is invoked by
             Region.get_or_create_multi(), the mapping values are the same ones
             returned to the upstream caller. If the subclass alters the values
@@ -1455,15 +1452,14 @@
             Release a âreaderâ lock.
             Raises NotImplementedError by default, must be implemented by
             subclasses.
         release_write_lock()Â¶
             Release a âwriterâ lock.
             Raises NotImplementedError by default, must be implemented by
             subclasses.
-
 **** Proxy BackendsÂ¶ ****
 Provides a utility and a decorator class that allow for modifying the behavior
 of different backends without altering the class itself or having to extend the
 base backend.
 New in version 0.5.0: Added support for the ProxyBackend class.
   classdogpile.cache.proxy.ProxyBackend(*arg, **kw)Â¶
       Bases: CacheBackend
@@ -1497,56 +1493,56 @@
       )
       Classes that extend ProxyBackend can be stacked together. The .proxied
       property will always point to either the concrete backend instance or the
       next proxy in the chain that a method can be delegated towards.
       New in version 0.5.0.
         delete(key: str) &#x2192; NoneÂ¶
             Delete a value from the cache.
-              Parameters
+              Parameters:
                   keyÂ¶ â String key that was passed to the
                   CacheRegion.delete() method, which will also be processed by
                   the âkey manglingâ function if one was present.
             The behavior here should be idempotent, that is, can be called any
             number of times regardless of whether or not the key exists.
         delete_multi(keys: Sequence[str]) &#x2192; NoneÂ¶
             Delete multiple values from the cache.
-              Parameters
+              Parameters:
                   keysÂ¶ â sequence of string keys that was passed to the
                   CacheRegion.delete_multi() method, which will also be
                   processed by the âkey manglingâ function if one was
                   present.
             The behavior here should be idempotent, that is, can be called any
             number of times regardless of whether or not the key exists.
             New in version 0.5.0.
-        get(key: str) &#x2192; Union[CachedValue, NoValue, bytes]Â¶
+        get(key: str) &#x2192; CachedValue | NoValue | bytesÂ¶
             Retrieve an optionally serialized value from the cache.
-              Parameters
+              Parameters:
                   keyÂ¶ â String key that was passed to the CacheRegion.get()
                   method, which will also be processed by the âkey
                   manglingâ function if one was present.
-              Returns
+              Returns:
                   the Python object that corresponds to what was established
                   via the CacheBackend.set() method, or the NO_VALUE constant
                   if not present.
             If a serializer is in use, this method will only be called if the
             CacheBackend.get_serialized() method is not overridden.
-        get_multi(keys: Sequence[str]) &#x2192; Sequence[Union[CachedValue,
-        NoValue, bytes]]Â¶
+        get_multi(keys: Sequence[str]) &#x2192; Sequence[CachedValue | NoValue
+        | bytes]Â¶
             Retrieve multiple optionally serialized values from the cache.
-              Parameters
+              Parameters:
                   keysÂ¶ â sequence of string keys that was passed to the
                   CacheRegion.get_multi() method, which will also be processed
                   by the âkey manglingâ function if one was present.
               :return a list of values as would be returned
                   individually via the CacheBackend.get() method, corresponding
                   to the list of keys given.
             If a serializer is in use, this method will only be called if the
             CacheBackend.get_serialized_multi() method is not overridden.
             New in version 0.5.0.
-        get_mutex(key: str) &#x2192; Optional[CacheMutex]Â¶
+        get_mutex(key: str) &#x2192; CacheMutex | NoneÂ¶
             Return an optional mutexing object for the given key.
             This object need only provide an acquire() and release() method.
             May return None, in which case the dogpile lock will use a regular
             threading.Lock object to mutex concurrent threads for value
             creation. The default implementation returns None.
             Different backends may want to provide various kinds of âmutexâ
             objects, such as those which link to lock files, distributed
@@ -1555,58 +1551,57 @@
             A mutex that takes the key into account will allow multiple
             regenerate operations across keys to proceed simultaneously, while
             a mutex that does not will serialize regenerate operations to just
             one at a time across all keys in the region. The latter approach,
             or a variant that involves a modulus of the given keyâs hash
             value, can be used as a means of throttling the total number of
             value recreation operations that may proceed at one time.
-        get_serialized(key: str) &#x2192; Union[bytes, NoValue]Â¶
+        get_serialized(key: str) &#x2192; bytes | NoValueÂ¶
             Retrieve a serialized value from the cache.
-              Parameters
+              Parameters:
                   keyÂ¶ â String key that was passed to the CacheRegion.get()
                   method, which will also be processed by the âkey
                   manglingâ function if one was present.
-              Returns
+              Returns:
                   a bytes object, or NO_VALUE constant if not present.
             The default implementation of this method for CacheBackend returns
             the value of the CacheBackend.get() method.
             New in version 1.1.
             See also
             BytesBackend
-        get_serialized_multi(keys: Sequence[str]) &#x2192; Sequence[Union
-        [bytes, NoValue]]Â¶
+        get_serialized_multi(keys: Sequence[str]) &#x2192; Sequence[bytes |
+        NoValue]Â¶
             Retrieve multiple serialized values from the cache.
-              Parameters
+              Parameters:
                   keysÂ¶ â sequence of string keys that was passed to the
                   CacheRegion.get_multi() method, which will also be processed
                   by the âkey manglingâ function if one was present.
-              Returns
+              Returns:
                   list of bytes objects
             The default implementation of this method for CacheBackend returns
             the value of the CacheBackend.get_multi() method.
             New in version 1.1.
             See also
             BytesBackend
-        set(key: str, value: Union[CachedValue, bytes]) &#x2192; NoneÂ¶
+        set(key: str, value: CachedValue | bytes) &#x2192; NoneÂ¶
             Set an optionally serialized value in the cache.
-              Parameters
+              Parameters:
                       * keyÂ¶ â String key that was passed to the
                         CacheRegion.set() method, which will also be processed
                         by the âkey manglingâ function if one was present.
                       * valueÂ¶ â The optionally serialized CachedValue
                         object. May be an instance of CachedValue or a bytes
                         object depending on if a serializer is in use with the
                         region and if the CacheBackend.set_serialized() method
                         is not overridden.
             See also
             CacheBackend.set_serialized()
-        set_multi(mapping: Mapping[str, Union[CachedValue, bytes]]) &#x2192;
-        NoneÂ¶
+        set_multi(mapping: Mapping[str, CachedValue | bytes]) &#x2192; NoneÂ¶
             Set multiple values in the cache.
-              Parameters
+              Parameters:
                   mappingÂ¶ â a dict in which the key will be whatever was
                   passed to the CacheRegion.set_multi() method, processed by
                   the âkey manglingâ function, if any.
             When implementing a new CacheBackend or cutomizing via
             ProxyBackend, be aware that when this method is invoked by
             Region.get_or_create_multi(), the mapping values are the same ones
             returned to the upstream caller. If the subclass alters the values
@@ -1614,27 +1609,27 @@
             â that will have the undesirable effect of modifying the returned
             values as well.
             If a serializer is in use, this method will only be called if the
             CacheBackend.set_serialized_multi() method is not overridden.
             New in version 0.5.0.
         set_serialized(key: str, value: bytes) &#x2192; NoneÂ¶
             Set a serialized value in the cache.
-              Parameters
+              Parameters:
                       * keyÂ¶ â String key that was passed to the
                         CacheRegion.set() method, which will also be processed
                         by the âkey manglingâ function if one was present.
                       * valueÂ¶ â a bytes object to be stored.
             The default implementation of this method for CacheBackend calls
             upon the CacheBackend.set() method.
             New in version 1.1.
             See also
             BytesBackend
         set_serialized_multi(mapping: Mapping[str, bytes]) &#x2192; NoneÂ¶
             Set multiple serialized values in the cache.
-              Parameters
+              Parameters:
                   mappingÂ¶ â a dict in which the key will be whatever was
                   passed to the CacheRegion.set_multi() method, processed by
                   the âkey manglingâ function, if any.
             When implementing a new CacheBackend or cutomizing via
             ProxyBackend, be aware that when this method is invoked by
             Region.get_or_create_multi(), the mapping values are the same ones
             returned to the upstream caller. If the subclass alters the values
@@ -1645,15 +1640,14 @@
             The default implementation of this method for CacheBackend calls
             upon the CacheBackend.set_multi() method.
             See also
             BytesBackend
         wrap(backend: CacheBackend) &#x2192; ProxyBackendÂ¶
             Take a backend as an argument and setup the self.proxied property.
             Return an object that be used as a backend by a CacheRegion object.
-
 **** Null BackendÂ¶ ****
 The Null backend does not do any caching at all. It can be used to test
 behavior without caching, or as a means of disabling caching for a region that
 is otherwise used normally.
 New in version 0.5.4.
   classdogpile.cache.backends.null.NullBackend(arguments)Â¶
       Bases: CacheBackend
@@ -1662,45 +1656,45 @@
       from dogpile.cache import make_region
 
       region = make_region().configure(
           'dogpile.cache.null'
       )
         delete(key)Â¶
             Delete a value from the cache.
-              Parameters
+              Parameters:
                   keyÂ¶ â String key that was passed to the
                   CacheRegion.delete() method, which will also be processed by
                   the âkey manglingâ function if one was present.
             The behavior here should be idempotent, that is, can be called any
             number of times regardless of whether or not the key exists.
         delete_multi(keys)Â¶
             Delete multiple values from the cache.
-              Parameters
+              Parameters:
                   keysÂ¶ â sequence of string keys that was passed to the
                   CacheRegion.delete_multi() method, which will also be
                   processed by the âkey manglingâ function if one was
                   present.
             The behavior here should be idempotent, that is, can be called any
             number of times regardless of whether or not the key exists.
             New in version 0.5.0.
         get(key)Â¶
             Retrieve an optionally serialized value from the cache.
-              Parameters
+              Parameters:
                   keyÂ¶ â String key that was passed to the CacheRegion.get()
                   method, which will also be processed by the âkey
                   manglingâ function if one was present.
-              Returns
+              Returns:
                   the Python object that corresponds to what was established
                   via the CacheBackend.set() method, or the NO_VALUE constant
                   if not present.
             If a serializer is in use, this method will only be called if the
             CacheBackend.get_serialized() method is not overridden.
         get_multi(keys)Â¶
             Retrieve multiple optionally serialized values from the cache.
-              Parameters
+              Parameters:
                   keysÂ¶ â sequence of string keys that was passed to the
                   CacheRegion.get_multi() method, which will also be processed
                   by the âkey manglingâ function if one was present.
               :return a list of values as would be returned
                   individually via the CacheBackend.get() method, corresponding
                   to the list of keys given.
             If a serializer is in use, this method will only be called if the
@@ -1721,28 +1715,28 @@
             a mutex that does not will serialize regenerate operations to just
             one at a time across all keys in the region. The latter approach,
             or a variant that involves a modulus of the given keyâs hash
             value, can be used as a means of throttling the total number of
             value recreation operations that may proceed at one time.
         set(key, value)Â¶
             Set an optionally serialized value in the cache.
-              Parameters
+              Parameters:
                       * keyÂ¶ â String key that was passed to the
                         CacheRegion.set() method, which will also be processed
                         by the âkey manglingâ function if one was present.
                       * valueÂ¶ â The optionally serialized CachedValue
                         object. May be an instance of CachedValue or a bytes
                         object depending on if a serializer is in use with the
                         region and if the CacheBackend.set_serialized() method
                         is not overridden.
             See also
             CacheBackend.set_serialized()
         set_multi(mapping)Â¶
             Set multiple values in the cache.
-              Parameters
+              Parameters:
                   mappingÂ¶ â a dict in which the key will be whatever was
                   passed to the CacheRegion.set_multi() method, processed by
                   the âkey manglingâ function, if any.
             When implementing a new CacheBackend or cutomizing via
             ProxyBackend, be aware that when this method is invoked by
             Region.get_or_create_multi(), the mapping values are the same ones
             returned to the upstream caller. If the subclass alters the values
@@ -1807,32 +1801,32 @@
     some content that's cached
 </%def>
   classdogpile.cache.plugins.mako_cache.MakoPlugin(cache)Â¶
       Bases: CacheImpl
       A Mako CacheImpl which talks to dogpile.cache.
         get(key, **kw)Â¶
             Retrieve a value from the cache.
-              Parameters
+              Parameters:
                       * keyÂ¶ â the valueâs key.
                       * **kwÂ¶ â cache configuration arguments.
         get_or_create(key, creation_function, **kw)Â¶
             Retrieve a value from the cache, using the given creation function
             to generate a new value.
             This function must return a value, either from the cache, or via
             the given creation function. If the creation function is called,
             the newly created value should be populated into the cache under
             the given key before being returned.
-              Parameters
+              Parameters:
                       * keyÂ¶ â the valueâs key.
                       * creation_functionÂ¶ â function that when called
                         generates a new value.
                       * **kwÂ¶ â cache configuration arguments.
         invalidate(key, **kw)Â¶
             Invalidate a value in the cache.
-              Parameters
+              Parameters:
                       * keyÂ¶ â the valueâs key.
                       * **kwÂ¶ â cache configuration arguments.
 
 ***** UtilitiesÂ¶ *****
   dogpile.cache.util.function_key_generator(namespace, fn, to_str=<class
   'str'>)Â¶
       Return a function that generates a string key, based on a given function
@@ -1863,15 +1857,15 @@
 ***** dogpile CoreÂ¶ *****
   classdogpile.Lock(mutex, creator, value_and_created_fn, expiretime,
   async_creator=None)Â¶
       Dogpile lock class.
       Provides an interface around an arbitrary mutex that allows one thread/
       process to be elected as the creator of a new value, while other threads/
       processes continue to return the previous version of that value.
-        Parameters
+        Parameters:
                 * mutexÂ¶ â A mutex object that provides acquire() and
                   release() methods.
                 * creatorÂ¶ â Callable which returns a tuple of the form
                   (new_value, creation_time). ânew_valueâ should be a newly
                   generated value representing completed state.
                   âcreation_timeâ should be a floating point time value
                   which is relative to Pythonâs time.time() call,
@@ -1930,50 +1924,222 @@
       my_foo = registry.get("foo1")
       Above, my_foo in both thread #1 and #2 will be the same object. The
       constructor for MyFoo will be called once, passing the identifier foo1 as
       the argument.
       When thread 1 and thread 2 both complete or otherwise delete references
       to my_foo, the object is removed from the NameRegistry as a result of
       Python garbage collection.
-        Parameters
+        Parameters:
             creatorÂ¶ â A function that will create a new value, given the
             identifier passed to the NameRegistry.get() method.
         get(identifier: str, *args: Any, **kw: Any) &#x2192; AnyÂ¶
             Get and possibly create the value.
-              Parameters
+              Parameters:
                       * identifierÂ¶ â Hash key for the value. If the
                         creation function is called, this identifier will also
                         be passed to the creation function.
                       * **kwÂ¶ (*args,) â Additional arguments which will
                         also be passed to the creation function if it is
                         called.
 
 **** Table_of_Contents ****
     * API
           o Region
+                # CacheRegion
+                      # CacheRegion.actual_backend
+                      # CacheRegion.cache_multi_on_arguments()
+                      # CacheRegion.cache_on_arguments()
+                      # CacheRegion.configure()
+                      # CacheRegion.configure_from_config()
+                      # CacheRegion.delete()
+                      # CacheRegion.delete_multi()
+                      # CacheRegion.get()
+                      # CacheRegion.get_multi()
+                      # CacheRegion.get_or_create()
+                      # CacheRegion.get_or_create_multi()
+                      # CacheRegion.invalidate()
+                      # CacheRegion.is_configured
+                      # CacheRegion.key_is_locked()
+                      # CacheRegion.set()
+                      # CacheRegion.set_multi()
+                      # CacheRegion.wrap()
+                # DefaultInvalidationStrategy
+                      # DefaultInvalidationStrategy.invalidate()
+                      # DefaultInvalidationStrategy.is_hard_invalidated()
+                      # DefaultInvalidationStrategy.is_invalidated()
+                      # DefaultInvalidationStrategy.is_soft_invalidated()
+                      # DefaultInvalidationStrategy.was_hard_invalidated()
+                      # DefaultInvalidationStrategy.was_soft_invalidated()
+                # RegionInvalidationStrategy
+                      # RegionInvalidationStrategy.invalidate()
+                      # RegionInvalidationStrategy.is_hard_invalidated()
+                      # RegionInvalidationStrategy.is_invalidated()
+                      # RegionInvalidationStrategy.is_soft_invalidated()
+                      # RegionInvalidationStrategy.was_hard_invalidated()
+                      # RegionInvalidationStrategy.was_soft_invalidated()
+                # make_region()
+                # value_version
           o Backend_API
+                # BackendFormatted
+                # BackendSetType
+                # BytesBackend
+                      # BytesBackend.get_serialized()
+                      # BytesBackend.get_serialized_multi()
+                      # BytesBackend.set_serialized()
+                      # BytesBackend.set_serialized_multi()
+                # CacheBackend
+                      # CacheBackend.delete()
+                      # CacheBackend.delete_multi()
+                      # CacheBackend.deserializer
+                      # CacheBackend.get()
+                      # CacheBackend.get_multi()
+                      # CacheBackend.get_mutex()
+                      # CacheBackend.get_serialized()
+                      # CacheBackend.get_serialized_multi()
+                      # CacheBackend.key_mangler
+                      # CacheBackend.serializer
+                      # CacheBackend.set()
+                      # CacheBackend.set_multi()
+                      # CacheBackend.set_serialized()
+                      # CacheBackend.set_serialized_multi()
+                # CacheMutex
+                      # CacheMutex.acquire()
+                      # CacheMutex.locked()
+                      # CacheMutex.release()
+                # CacheReturnType
+                # CachedValue
+                      # CachedValue.metadata
+                      # CachedValue.payload
+                # CantDeserializeException
+                # KeyType
+                # NO_VALUE
+                # NoValue
+                # SerializedReturnType
+                # ValuePayload
           o Backends
                 # Memory_Backends
+                # MemoryBackend
+                      # MemoryBackend.delete()
+                      # MemoryBackend.delete_multi()
+                      # MemoryBackend.get()
+                      # MemoryBackend.get_multi()
+                      # MemoryBackend.set()
+                      # MemoryBackend.set_multi()
+                # MemoryPickleBackend
                 # Memcached_Backends
+                # BMemcachedBackend
+                      # BMemcachedBackend.delete_multi()
+                # GenericMemcachedBackend
+                      # GenericMemcachedBackend.client
+                      # GenericMemcachedBackend.delete()
+                      # GenericMemcachedBackend.delete_multi()
+                      # GenericMemcachedBackend.deserializer
+                      # GenericMemcachedBackend.get()
+                      # GenericMemcachedBackend.get_multi()
+                      # GenericMemcachedBackend.get_mutex()
+                      # GenericMemcachedBackend.serializer
+                      # GenericMemcachedBackend.set()
+                      # GenericMemcachedBackend.set_arguments
+                      # GenericMemcachedBackend.set_multi()
+                # MemcachedBackend
+                # MemcachedLock
+                # PyMemcacheBackend
+                # PylibmcBackend
                 # Redis_Backends
+                # RedisBackend
+                      # RedisBackend.delete()
+                      # RedisBackend.delete_multi()
+                      # RedisBackend.get_mutex()
+                      # RedisBackend.get_serialized()
+                      # RedisBackend.get_serialized_multi()
+                      # RedisBackend.set_serialized()
+                      # RedisBackend.set_serialized_multi()
+                # RedisSentinelBackend
                 # File_Backends
+                # AbstractFileLock
+                      # AbstractFileLock.acquire()
+                      # AbstractFileLock.acquire_read_lock()
+                      # AbstractFileLock.acquire_write_lock()
+                      # AbstractFileLock.is_open
+                      # AbstractFileLock.read()
+                      # AbstractFileLock.release()
+                      # AbstractFileLock.release_read_lock()
+                      # AbstractFileLock.release_write_lock()
+                      # AbstractFileLock.write()
+                # DBMBackend
+                      # DBMBackend.delete()
+                      # DBMBackend.delete_multi()
+                      # DBMBackend.get_mutex()
+                      # DBMBackend.get_serialized()
+                      # DBMBackend.get_serialized_multi()
+                      # DBMBackend.set_serialized()
+                      # DBMBackend.set_serialized_multi()
+                # FileLock
+                      # FileLock.acquire_read_lock()
+                      # FileLock.acquire_write_lock()
+                      # FileLock.is_open
+                      # FileLock.release_read_lock()
+                      # FileLock.release_write_lock()
                 # Proxy_Backends
+                # ProxyBackend
+                      # ProxyBackend.delete()
+                      # ProxyBackend.delete_multi()
+                      # ProxyBackend.get()
+                      # ProxyBackend.get_multi()
+                      # ProxyBackend.get_mutex()
+                      # ProxyBackend.get_serialized()
+                      # ProxyBackend.get_serialized_multi()
+                      # ProxyBackend.set()
+                      # ProxyBackend.set_multi()
+                      # ProxyBackend.set_serialized()
+                      # ProxyBackend.set_serialized_multi()
+                      # ProxyBackend.wrap()
                 # Null_Backend
+                # NullBackend
+                      # NullBackend.delete()
+                      # NullBackend.delete_multi()
+                      # NullBackend.get()
+                      # NullBackend.get_multi()
+                      # NullBackend.get_mutex()
+                      # NullBackend.set()
+                      # NullBackend.set_multi()
           o Exceptions
+                # DogpileCacheException
+                # PluginNotFound
+                # RegionAlreadyConfigured
+                # RegionNotConfigured
+                # ValidationError
           o Plugins
                 # Mako_Integration
+                # MakoPlugin
+                      # MakoPlugin.get()
+                      # MakoPlugin.get_or_create()
+                      # MakoPlugin.invalidate()
           o Utilities
+                # function_key_generator()
+                # kwarg_function_key_generator()
+                # sha1_mangle_key()
+                # length_conditional_mangler()
           o dogpile_Core
+                # Lock
+                # NeedRegenerationException
+                # ReadWriteMutex
+                      # ReadWriteMutex.acquire_read_lock()
+                      # ReadWriteMutex.acquire_write_lock()
+                      # ReadWriteMutex.release_read_lock()
+                      # ReadWriteMutex.release_write_lock()
+                # NameRegistry
+                      # NameRegistry.get()
 **** Quick search ****
 [q                   ] [Go]
 *** Previous topic ***
 dogpile_Core
 *** Next topic ***
 Changelog
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * dogpile.cache_1.1.8_documentation »
+    * dogpile.cache_1.2.0_documentation »
     * API
-© Copyright 2011-2022 Mike Bayer. Created using Sphinx 5.0.2.
+© Copyright 2011-2023 Mike Bayer. Created using Sphinx 6.2.1.
```

### Comparing `dogpile.cache-1.1.8/docs/build/Makefile` & `dogpile.cache-1.2.0/docs/build/Makefile`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/docs/build/api.rst` & `dogpile.cache-1.2.0/docs/build/api.rst`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/docs/build/changelog.rst` & `dogpile.cache-1.2.0/docs/build/changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,28 @@
 =========
 Changelog
 =========
 
 .. changelog::
+    :version: 1.2.0
+    :released: Wed Apr 26 2023
+
+    .. change::
+        :tags: feature, region
+        :tickets: 236
+
+        Added new construct :class:`.api.CantDeserializeException` which can be
+        raised by user-defined deserializer functions which would be passed to
+        :paramref:`.CacheRegion.deserializer`, to indicate a cache value that can't
+        be deserialized and therefore should be regenerated. This can allow an
+        application that's been updated to gracefully re-cache old items that were
+        persisted from a previous version of the application. Pull request courtesy
+        Simon Hewitt.
+
+.. changelog::
     :version: 1.1.8
     :released: Fri Jul 8 2022
 
     .. change::
         :tags: bug, memcached
         :tickets: 223, 228
```

### Comparing `dogpile.cache-1.1.8/docs/build/conf.py` & `dogpile.cache-1.2.0/docs/build/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,24 +61,24 @@
 # source_encoding = 'utf-8'
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "dogpile.cache"
-copyright = "2011-2022 Mike Bayer"
+copyright = "2011-2023 Mike Bayer"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = dogpile.__version__
 # The full version, including alpha/beta/rc tags.
-release = "1.1.8"
+release = "1.2.0"
 
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
 
 # There are two options for replacing |today|: either, you set today to some
```

### Comparing `dogpile.cache-1.1.8/docs/build/core_usage.rst` & `dogpile.cache-1.2.0/docs/build/core_usage.rst`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/docs/build/front.rst` & `dogpile.cache-1.2.0/docs/build/front.rst`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/docs/build/index.rst` & `dogpile.cache-1.2.0/docs/build/index.rst`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/docs/build/recipes.rst` & `dogpile.cache-1.2.0/docs/build/recipes.rst`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/docs/build/usage.rst` & `dogpile.cache-1.2.0/docs/build/usage.rst`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/docs/changelog.html` & `dogpile.cache-1.2.0/docs/changelog.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Changelog &#8212; dogpile.cache 1.1.8 documentation</title>
+    <title>Changelog &#8212; dogpile.cache 1.2.0 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
-    <script src="_static/jquery.js"></script>
-    <script src="_static/underscore.js"></script>
-    <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
     <script src="_static/doctools.js"></script>
+    <script src="_static/sphinx_highlight.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="prev" title="API" href="api.html" /> 
   </head><body>
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
@@ -28,26 +26,44 @@
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="api.html" title="API"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.1.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.0 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Changelog</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body" role="main">
             
   <section id="changelog">
 <h1>Changelog<a class="headerlink" href="#changelog" title="Permalink to this heading">¶</a></h1>
+<section id="change-1.2.0">
+<h2 class="release-version">1.2.0<a class="headerlink" href="#change-1.2.0" title="Permalink to this heading">¶</a></h2>
+Released: Wed Apr 26 2023<section id="change-1.2.0-feature">
+<h3>feature<a class="headerlink" href="#change-1.2.0-feature" title="Permalink to this heading">¶</a></h3>
+<ul class="simple">
+<li><p class="caption" id="change-1.2.0-0"><span class="target" id="change-cb55fd53c03c5bae407507cf0cd7453c"><strong>[feature] [region]</strong> <a class="changelog-reference headerlink reference internal" href="#change-cb55fd53c03c5bae407507cf0cd7453c">¶</a></span><p>Added new construct <a class="reference internal" href="api.html#dogpile.cache.api.CantDeserializeException" title="dogpile.cache.api.CantDeserializeException"><code class="xref py py-class docutils literal notranslate"><span class="pre">api.CantDeserializeException</span></code></a> which can be
+raised by user-defined deserializer functions which would be passed to
+<a class="reference internal" href="api.html#dogpile.cache.region.CacheRegion.params.deserializer" title="dogpile.cache.region.CacheRegion"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">CacheRegion.deserializer</span></code></a>, to indicate a cache value that can’t
+be deserialized and therefore should be regenerated. This can allow an
+application that’s been updated to gracefully re-cache old items that were
+persisted from a previous version of the application. Pull request courtesy
+Simon Hewitt.</p>
+<p>References: <a class="reference external" href="https://github.com/sqlalchemy/dogpile.cache/issues/236">#236</a></p>
+</p>
+</li>
+</ul>
+</section>
+</section>
 <section id="change-1.1.8">
 <h2 class="release-version">1.1.8<a class="headerlink" href="#change-1.1.8" title="Permalink to this heading">¶</a></h2>
 Released: Fri Jul 8 2022<section id="change-1.1.8-bug">
 <h3>bug<a class="headerlink" href="#change-1.1.8-bug" title="Permalink to this heading">¶</a></h3>
 <ul class="simple">
 <li><p class="caption" id="change-1.1.8-0"><span class="target" id="change-c483ce3cfcd3295d554300227c723cca"><strong>[bug] [memcached]</strong> <a class="changelog-reference headerlink reference internal" href="#change-c483ce3cfcd3295d554300227c723cca">¶</a></span><p>Moved the <code class="xref py py-paramref docutils literal notranslate"><span class="pre">MemcacheArgs.dead_retry</span></code> argument and the
 <code class="xref py py-paramref docutils literal notranslate"><span class="pre">MemcacheArgs.socket_timeout</span></code> argument which were
@@ -1337,14 +1353,18 @@
       </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
         <div class="sphinxsidebarwrapper">
   <div>
     <h3><a href="index.html">Table of Contents</a></h3>
     <ul>
 <li><a class="reference internal" href="#">Changelog</a><ul>
+<li><a class="reference internal" href="#change-1.2.0">1.2.0</a><ul>
+<li><a class="reference internal" href="#change-1.2.0-feature">feature</a></li>
+</ul>
+</li>
 <li><a class="reference internal" href="#change-1.1.8">1.1.8</a><ul>
 <li><a class="reference internal" href="#change-1.1.8-bug">bug</a></li>
 </ul>
 </li>
 <li><a class="reference internal" href="#change-1.1.7">1.1.7</a><ul>
 <li><a class="reference internal" href="#change-1.1.7-usecase">usecase</a></li>
 </ul>
@@ -1560,17 +1580,17 @@
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="api.html" title="API"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.1.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.0 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Changelog</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2011-2022 Mike Bayer.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 5.0.2.
+        &#169; Copyright 2011-2023 Mike Bayer.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.2.1.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -6,17 +6,30 @@
 
 
 
 **** Navigation ****
     * index
     * modules |
     * previous |
-    * dogpile.cache_1.1.8_documentation »
+    * dogpile.cache_1.2.0_documentation »
     * Changelog
 ****** ChangelogÂ¶ ******
+***** 1.2.0Â¶ *****
+Released: Wed Apr 26 2023
+**** featureÂ¶ ****
+    * [feature] [region] Â¶
+      Added new construct api.CantDeserializeException which can be raised by
+      user-defined deserializer functions which would be passed to
+      CacheRegion.deserializer, to indicate a cache value that canât be
+      deserialized and therefore should be regenerated. This can allow an
+      application thatâs been updated to gracefully re-cache old items that
+      were persisted from a previous version of the application. Pull request
+      courtesy Simon Hewitt.
+      References: #236
+
 ***** 1.1.8Â¶ *****
 Released: Fri Jul 8 2022
 **** bugÂ¶ ****
     * [bug] [memcached] Â¶
       Moved the MemcacheArgs.dead_retry argument and the
       MemcacheArgs.socket_timeout argument which were erroneously added to the
       âset_parametersâ, where they have no effect, to be part of the
@@ -827,14 +840,16 @@
     * [no_tags] Â¶
       Initial release.
 [no_tags] Â¶
 Includes a pylibmc backend and a plain dictionary backend.
 
 **** Table_of_Contents ****
     * Changelog
+          o 1.2.0
+                # feature
           o 1.1.8
                 # bug
           o 1.1.7
                 # usecase
           o 1.1.6
                 # usecase
                 # bug
@@ -942,10 +957,10 @@
 [q                   ] [Go]
 *** Previous topic ***
 API
 **** Navigation ****
     * index
     * modules |
     * previous |
-    * dogpile.cache_1.1.8_documentation »
+    * dogpile.cache_1.2.0_documentation »
     * Changelog
-© Copyright 2011-2022 Mike Bayer. Created using Sphinx 5.0.2.
+© Copyright 2011-2023 Mike Bayer. Created using Sphinx 6.2.1.
```

### Comparing `dogpile.cache-1.1.8/docs/core_usage.html` & `dogpile.cache-1.2.0/docs/core_usage.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>dogpile Core &#8212; dogpile.cache 1.1.8 documentation</title>
+    <title>dogpile Core &#8212; dogpile.cache 1.2.0 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
-    <script src="_static/jquery.js"></script>
-    <script src="_static/underscore.js"></script>
-    <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
     <script src="_static/doctools.js"></script>
+    <script src="_static/sphinx_highlight.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="API" href="api.html" />
     <link rel="prev" title="Recipes" href="recipes.html" /> 
   </head><body>
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
@@ -32,15 +30,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="api.html" title="API"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="recipes.html" title="Recipes"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.1.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.0 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">dogpile Core</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -167,15 +165,15 @@
 <span class="kn">import</span> <span class="nn">threading</span>
 <span class="kn">import</span> <span class="nn">time</span>
 <span class="kn">from</span> <span class="nn">dogpile</span> <span class="kn">import</span> <span class="n">Lock</span><span class="p">,</span> <span class="n">NeedRegenerationException</span>
 
 <span class="n">mc_pool</span> <span class="o">=</span> <span class="n">pylibmc</span><span class="o">.</span><span class="n">ThreadMappedPool</span><span class="p">(</span><span class="n">pylibmc</span><span class="o">.</span><span class="n">Client</span><span class="p">(</span><span class="s2">&quot;localhost&quot;</span><span class="p">))</span>
 
 <span class="k">def</span> <span class="nf">cached</span><span class="p">(</span><span class="n">key</span><span class="p">,</span> <span class="n">expiration_time</span><span class="p">):</span>
-    <span class="sd">&quot;&quot;&quot;A decorator that will cache the return value of a function</span>
+<span class="w">    </span><span class="sd">&quot;&quot;&quot;A decorator that will cache the return value of a function</span>
 <span class="sd">    in memcached given a key.&quot;&quot;&quot;</span>
 
     <span class="n">mutex</span> <span class="o">=</span> <span class="n">threading</span><span class="o">.</span><span class="n">Lock</span><span class="p">()</span>
 
     <span class="k">def</span> <span class="nf">get_value</span><span class="p">():</span>
          <span class="k">with</span> <span class="n">mc_pool</span><span class="o">.</span><span class="n">reserve</span><span class="p">()</span> <span class="k">as</span> <span class="n">mc</span><span class="p">:</span>
             <span class="n">value_plus_time</span> <span class="o">=</span> <span class="n">mc</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">key</span><span class="p">)</span>
@@ -237,15 +235,15 @@
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="kn">import</span> <span class="nn">lockfile</span>
 <span class="kn">import</span> <span class="nn">os</span>
 <span class="kn">from</span> <span class="nn">hashlib</span> <span class="kn">import</span> <span class="n">sha1</span>
 
 <span class="c1"># ... other imports and setup from the previous example</span>
 
 <span class="k">def</span> <span class="nf">cached</span><span class="p">(</span><span class="n">key</span><span class="p">,</span> <span class="n">expiration_time</span><span class="p">):</span>
-    <span class="sd">&quot;&quot;&quot;A decorator that will cache the return value of a function</span>
+<span class="w">    </span><span class="sd">&quot;&quot;&quot;A decorator that will cache the return value of a function</span>
 <span class="sd">    in memcached given a key.&quot;&quot;&quot;</span>
 
     <span class="n">lock_path</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="s2">&quot;/tmp&quot;</span><span class="p">,</span> <span class="s2">&quot;</span><span class="si">%s</span><span class="s2">.lock&quot;</span> <span class="o">%</span> <span class="n">sha1</span><span class="p">(</span><span class="n">key</span><span class="p">)</span><span class="o">.</span><span class="n">hexdigest</span><span class="p">())</span>
 
     <span class="c1"># ... get_value() from the previous example goes here</span>
 
     <span class="k">def</span> <span class="nf">decorate</span><span class="p">(</span><span class="n">fn</span><span class="p">):</span>
@@ -330,17 +328,17 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="api.html" title="API"
              >next</a> |</li>
         <li class="right" >
           <a href="recipes.html" title="Recipes"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.1.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.0 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">dogpile Core</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2011-2022 Mike Bayer.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 5.0.2.
+        &#169; Copyright 2011-2023 Mike Bayer.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.2.1.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -8,15 +8,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * dogpile.cache_1.1.8_documentation »
+    * dogpile.cache_1.2.0_documentation »
     * dogpile Core
 ****** dogpile CoreÂ¶ ******
 dogpile provides a locking interface around a âvalue creationâ and âvalue
 retrievalâ pair of functions.
 Changed in version 0.6.0: The dogpile package encapsulates the functionality
 that was previously provided by the separate dogpile.core package.
 The primary interface is the Lock object, which provides for the invocation of
@@ -235,10 +235,10 @@
 *** Next topic ***
 API
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * dogpile.cache_1.1.8_documentation »
+    * dogpile.cache_1.2.0_documentation »
     * dogpile Core
-© Copyright 2011-2022 Mike Bayer. Created using Sphinx 5.0.2.
+© Copyright 2011-2023 Mike Bayer. Created using Sphinx 6.2.1.
```

### Comparing `dogpile.cache-1.1.8/docs/front.html` & `dogpile.cache-1.2.0/docs/front.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Front Matter &#8212; dogpile.cache 1.1.8 documentation</title>
+    <title>Front Matter &#8212; dogpile.cache 1.2.0 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
-    <script src="_static/jquery.js"></script>
-    <script src="_static/underscore.js"></script>
-    <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
     <script src="_static/doctools.js"></script>
+    <script src="_static/sphinx_highlight.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Usage Guide" href="usage.html" />
     <link rel="prev" title="Welcome to dogpile.cache’s documentation!" href="index.html" /> 
   </head><body>
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
@@ -32,15 +30,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="usage.html" title="Usage Guide"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="index.html" title="Welcome to dogpile.cache’s documentation!"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.1.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.0 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Front Matter</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -123,17 +121,17 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="usage.html" title="Usage Guide"
              >next</a> |</li>
         <li class="right" >
           <a href="index.html" title="Welcome to dogpile.cache’s documentation!"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.1.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.0 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Front Matter</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2011-2022 Mike Bayer.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 5.0.2.
+        &#169; Copyright 2011-2023 Mike Bayer.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.2.1.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -8,15 +8,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * dogpile.cache_1.1.8_documentation »
+    * dogpile.cache_1.2.0_documentation »
     * Front Matter
 ****** Front MatterÂ¶ ******
 Information about the dogpile.cache project.
 ***** Project HomepageÂ¶ *****
 dogpile.cache is hosted on GitHub at https://github.com/sqlalchemy/
 dogpile.cache.
 Releases and project status are available on Pypi at https://pypi.python.org/
@@ -45,10 +45,10 @@
 *** Next topic ***
 Usage_Guide
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * dogpile.cache_1.1.8_documentation »
+    * dogpile.cache_1.2.0_documentation »
     * Front Matter
-© Copyright 2011-2022 Mike Bayer. Created using Sphinx 5.0.2.
+© Copyright 2011-2023 Mike Bayer. Created using Sphinx 6.2.1.
```

### Comparing `dogpile.cache-1.1.8/docs/genindex.html` & `dogpile.cache-1.2.0/docs/genindex.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Index &#8212; dogpile.cache 1.1.8 documentation</title>
+    <title>Index &#8212; dogpile.cache 1.2.0 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
-    <script src="_static/jquery.js"></script>
-    <script src="_static/underscore.js"></script>
-    <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
     <script src="_static/doctools.js"></script>
+    <script src="_static/sphinx_highlight.js"></script>
     <link rel="index" title="Index" href="#" />
     <link rel="search" title="Search" href="search.html" /> 
   </head><body>
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="#" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.1.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.0 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Index</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -157,14 +155,16 @@
 </li>
       <li><a href="api.html#dogpile.cache.api.CacheMutex">CacheMutex (class in dogpile.cache.api)</a>
 </li>
       <li><a href="api.html#dogpile.cache.region.CacheRegion">CacheRegion (class in dogpile.cache.region)</a>
 </li>
       <li><a href="api.html#dogpile.cache.api.CacheReturnType">CacheReturnType (in module dogpile.cache.api)</a>
 </li>
+      <li><a href="api.html#dogpile.cache.api.CantDeserializeException">CantDeserializeException</a>
+</li>
       <li><a href="api.html#dogpile.cache.backends.memcached.GenericMemcachedBackend.client">client (dogpile.cache.backends.memcached.GenericMemcachedBackend property)</a>
 </li>
       <li><a href="api.html#dogpile.cache.region.CacheRegion.configure">configure() (dogpile.cache.region.CacheRegion method)</a>
 </li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="api.html#dogpile.cache.region.CacheRegion.configure_from_config">configure_from_config() (dogpile.cache.region.CacheRegion method)</a>
@@ -1136,17 +1136,17 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="#" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.1.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.0 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Index</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2011-2022 Mike Bayer.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 5.0.2.
+        &#169; Copyright 2011-2023 Mike Bayer.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.2.1.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * dogpile.cache_1.1.8_documentation »
+    * dogpile.cache_1.2.0_documentation »
     * Index
 ****** Index ******
 Symbols | A | B | C | D | E | F | G | H | I | K | L | M | N | P | R | S | T | U
 | V | W
 ***** Symbols *****
     * **kw_(dogpile.cache.plugins.mako_cache.MakoPlugin.get_parameter)
           o (dogpile.cache.plugins.mako_cache.MakoPlugin.get_or_create
@@ -54,19 +54,19 @@
     * cache_on_arguments()_(dogpile.cache.region.CacheRegion                parameter)
       method)                                                       * connection_pool_(dogpile.cache.backends.redis.RedisBackend
     * CacheBackend_(class_in_dogpile.cache.api)                       parameter)
     * CachedValue_(class_in_dogpile.cache.api)                      * creation_function_
     * CacheMutex_(class_in_dogpile.cache.api)                         (dogpile.cache.plugins.mako_cache.MakoPlugin.get_or_create
     * CacheRegion_(class_in_dogpile.cache.region)                     parameter)
     * CacheReturnType_(in_module_dogpile.cache.api)                 * creator_(dogpile.cache.region.CacheRegion.get_or_create
-    * client_                                                         parameter), [1]
-      (dogpile.cache.backends.memcached.GenericMemcachedBackend           o (dogpile.cache.region.CacheRegion.get_or_create_multi
-      property)                                                             parameter)
-    * configure()_(dogpile.cache.region.CacheRegion_method)               o (dogpile.Lock_parameter)
-                                                                          o (dogpile.util.NameRegistry_parameter)
+    * CantDeserializeException                                        parameter), [1]
+    * client_                                                             o (dogpile.cache.region.CacheRegion.get_or_create_multi
+      (dogpile.cache.backends.memcached.GenericMemcachedBackend             parameter)
+      property)                                                           o (dogpile.Lock_parameter)
+    * configure()_(dogpile.cache.region.CacheRegion_method)               o (dogpile.util.NameRegistry_parameter)
                                                                     * creator_args_
                                                                       (dogpile.cache.region.CacheRegion.get_or_create_parameter),
                                                                       [1]
 ***** D *****
     * db_(dogpile.cache.backends.redis.RedisBackend_parameter)
           o (dogpile.cache.backends.redis.RedisSentinelBackend            * distributed_lock_
             parameter)                                                      (dogpile.cache.backends.memcached.GenericMemcachedBackend
@@ -370,10 +370,10 @@
           o (dogpile.cache.region.RegionInvalidationStrategy       method)
             method)
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
-    * dogpile.cache_1.1.8_documentation »
+    * dogpile.cache_1.2.0_documentation »
     * Index
-© Copyright 2011-2022 Mike Bayer. Created using Sphinx 5.0.2.
+© Copyright 2011-2023 Mike Bayer. Created using Sphinx 6.2.1.
```

### Comparing `dogpile.cache-1.1.8/docs/index.html` & `dogpile.cache-1.2.0/docs/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Welcome to dogpile.cache’s documentation! &#8212; dogpile.cache 1.1.8 documentation</title>
+    <title>Welcome to dogpile.cache’s documentation! &#8212; dogpile.cache 1.2.0 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
-    <script src="_static/jquery.js"></script>
-    <script src="_static/underscore.js"></script>
-    <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
     <script src="_static/doctools.js"></script>
+    <script src="_static/sphinx_highlight.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Front Matter" href="front.html" /> 
   </head><body>
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
@@ -28,15 +26,15 @@
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="front.html" title="Front Matter"
              accesskey="N">next</a> |</li>
-        <li class="nav-item nav-item-0"><a href="#">dogpile.cache 1.1.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="#">dogpile.cache 1.2.0 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Welcome to dogpile.cache’s documentation!</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -95,14 +93,15 @@
 <li class="toctree-l2"><a class="reference internal" href="api.html#module-dogpile.cache.exception">Exceptions</a></li>
 <li class="toctree-l2"><a class="reference internal" href="api.html#module-dogpile.cache.plugins.mako_cache">Plugins</a></li>
 <li class="toctree-l2"><a class="reference internal" href="api.html#utilities">Utilities</a></li>
 <li class="toctree-l2"><a class="reference internal" href="api.html#dogpile-core">dogpile Core</a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="changelog.html">Changelog</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="changelog.html#change-1.2.0">1.2.0</a></li>
 <li class="toctree-l2"><a class="reference internal" href="changelog.html#change-1.1.8">1.1.8</a></li>
 <li class="toctree-l2"><a class="reference internal" href="changelog.html#change-1.1.7">1.1.7</a></li>
 <li class="toctree-l2"><a class="reference internal" href="changelog.html#change-1.1.6">1.1.6</a></li>
 <li class="toctree-l2"><a class="reference internal" href="changelog.html#change-1.1.5">1.1.5</a></li>
 <li class="toctree-l2"><a class="reference internal" href="changelog.html#change-1.1.4">1.1.4</a></li>
 <li class="toctree-l2"><a class="reference internal" href="changelog.html#change-1.1.3">1.1.3</a></li>
 <li class="toctree-l2"><a class="reference internal" href="changelog.html#change-1.1.2">1.1.2</a></li>
@@ -205,17 +204,17 @@
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="front.html" title="Front Matter"
              >next</a> |</li>
-        <li class="nav-item nav-item-0"><a href="#">dogpile.cache 1.1.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="#">dogpile.cache 1.2.0 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Welcome to dogpile.cache’s documentation!</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2011-2022 Mike Bayer.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 5.0.2.
+        &#169; Copyright 2011-2023 Mike Bayer.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.2.1.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -6,15 +6,15 @@
 
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
-    * dogpile.cache_1.1.8_documentation »
+    * dogpile.cache_1.2.0_documentation »
     * Welcome to dogpile.cacheâs documentation!
 ****** Welcome to dogpile.cacheâs documentation!Â¶ ******
 Dogpile consists of two subsystems, one building on top of the other.
 dogpile provides the concept of a âdogpile lockâ, a control structure which
 allows a single thread of execution to be selected as the âcreatorâ of some
 resource, while allowing other threads of execution to refer to the previous
 version of this resource as the creation proceeds; if there is no previous
@@ -52,14 +52,15 @@
           o Backend_API
           o Backends
           o Exceptions
           o Plugins
           o Utilities
           o dogpile_Core
     * Changelog
+          o 1.2.0
           o 1.1.8
           o 1.1.7
           o 1.1.6
           o 1.1.5
           o 1.1.4
           o 1.1.3
           o 1.1.2
@@ -116,10 +117,10 @@
 [q                   ] [Go]
 *** Next topic ***
 Front_Matter
 **** Navigation ****
     * index
     * modules |
     * next |
-    * dogpile.cache_1.1.8_documentation »
+    * dogpile.cache_1.2.0_documentation »
     * Welcome to dogpile.cacheâs documentation!
-© Copyright 2011-2022 Mike Bayer. Created using Sphinx 5.0.2.
+© Copyright 2011-2023 Mike Bayer. Created using Sphinx 6.2.1.
```

### Comparing `dogpile.cache-1.1.8/docs/py-modindex.html` & `dogpile.cache-1.2.0/docs/py-modindex.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Python Module Index &#8212; dogpile.cache 1.1.8 documentation</title>
+    <title>Python Module Index &#8212; dogpile.cache 1.2.0 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
-    <script src="_static/jquery.js"></script>
-    <script src="_static/underscore.js"></script>
-    <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
     <script src="_static/doctools.js"></script>
+    <script src="_static/sphinx_highlight.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
  
 
 
   </head><body>
     <div class="related" role="navigation" aria-label="related navigation">
@@ -26,15 +24,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="#" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.1.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.0 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Python Module Index</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -135,17 +133,17 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="#" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.1.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.0 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Python Module Index</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2011-2022 Mike Bayer.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 5.0.2.
+        &#169; Copyright 2011-2023 Mike Bayer.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.2.1.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * dogpile.cache_1.1.8_documentation »
+    * dogpile.cache_1.2.0_documentation »
     * Python Module Index
 ****** Python Module Index ******
 d
      
     d
 [-] dogpile
         dogpile.cache.api
@@ -26,10 +26,10 @@
         dogpile.cache.proxy
         dogpile.cache.region
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
-    * dogpile.cache_1.1.8_documentation »
+    * dogpile.cache_1.2.0_documentation »
     * Python Module Index
-© Copyright 2011-2022 Mike Bayer. Created using Sphinx 5.0.2.
+© Copyright 2011-2023 Mike Bayer. Created using Sphinx 6.2.1.
```

### Comparing `dogpile.cache-1.1.8/docs/recipes.html` & `dogpile.cache-1.2.0/docs/recipes.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Recipes &#8212; dogpile.cache 1.1.8 documentation</title>
+    <title>Recipes &#8212; dogpile.cache 1.2.0 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
-    <script src="_static/jquery.js"></script>
-    <script src="_static/underscore.js"></script>
-    <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
     <script src="_static/doctools.js"></script>
+    <script src="_static/sphinx_highlight.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="dogpile Core" href="core_usage.html" />
     <link rel="prev" title="Usage Guide" href="usage.html" /> 
   </head><body>
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
@@ -32,15 +30,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="core_usage.html" title="dogpile Core"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="usage.html" title="Usage Guide"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.1.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.0 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Recipes</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -147,15 +145,15 @@
 a system such as the <a class="reference internal" href="api.html#dogpile.cache.region.CacheRegion.params.async_creation_runner" title="dogpile.cache.region.CacheRegion"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">CacheRegion.async_creation_runner</span></code></a>.
 However, an expedient approach for smaller use cases is to link cache refresh
 operations to the ORM session’s commit, as below:</p>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="kn">from</span> <span class="nn">sqlalchemy</span> <span class="kn">import</span> <span class="n">event</span>
 <span class="kn">from</span> <span class="nn">sqlalchemy.orm</span> <span class="kn">import</span> <span class="n">Session</span>
 
 <span class="k">def</span> <span class="nf">cache_refresh</span><span class="p">(</span><span class="n">session</span><span class="p">,</span> <span class="n">refresher</span><span class="p">,</span> <span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">):</span>
-    <span class="sd">&quot;&quot;&quot;</span>
+<span class="w">    </span><span class="sd">&quot;&quot;&quot;</span>
 <span class="sd">    Refresh the functions cache data in a new thread. Starts refreshing only</span>
 <span class="sd">    after the session was committed so all database data is available.</span>
 <span class="sd">    &quot;&quot;&quot;</span>
     <span class="k">assert</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">session</span><span class="p">,</span> <span class="n">Session</span><span class="p">),</span> \
         <span class="s2">&quot;Need a session, not a sessionmaker or scoped_session&quot;</span>
 
     <span class="nd">@event</span><span class="o">.</span><span class="n">listens_for</span><span class="p">(</span><span class="n">session</span><span class="p">,</span> <span class="s2">&quot;after_commit&quot;</span><span class="p">)</span>
@@ -220,15 +218,15 @@
 inherits from <code class="docutils literal notranslate"><span class="pre">_EncodedProxy</span></code> and  implements the necessary <code class="docutils literal notranslate"><span class="pre">value_decode</span></code>
 and <code class="docutils literal notranslate"><span class="pre">value_encode</span></code> functions.</p>
 <p>Encoded ProxyBackend Example:</p>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="kn">from</span> <span class="nn">dogpile.cache.proxy</span> <span class="kn">import</span> <span class="n">ProxyBackend</span>
 <span class="kn">import</span> <span class="nn">msgpack</span>
 
 <span class="k">class</span> <span class="nc">_EncodedProxy</span><span class="p">(</span><span class="n">ProxyBackend</span><span class="p">):</span>
-    <span class="sd">&quot;&quot;&quot;base class for building value-mangling proxies&quot;&quot;&quot;</span>
+<span class="w">    </span><span class="sd">&quot;&quot;&quot;base class for building value-mangling proxies&quot;&quot;&quot;</span>
 
     <span class="k">def</span> <span class="nf">value_decode</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">):</span>
         <span class="k">raise</span> <span class="ne">NotImplementedError</span><span class="p">(</span><span class="s2">&quot;override me&quot;</span><span class="p">)</span>
 
     <span class="k">def</span> <span class="nf">value_encode</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">value</span><span class="p">):</span>
         <span class="k">raise</span> <span class="ne">NotImplementedError</span><span class="p">(</span><span class="s2">&quot;override me&quot;</span><span class="p">)</span>
 
@@ -237,15 +235,15 @@
         <span class="bp">self</span><span class="o">.</span><span class="n">proxied</span><span class="o">.</span><span class="n">set</span><span class="p">(</span><span class="n">k</span><span class="p">,</span> <span class="n">v</span><span class="p">)</span>
 
     <span class="k">def</span> <span class="nf">get</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">key</span><span class="p">):</span>
         <span class="n">v</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">proxied</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">key</span><span class="p">)</span>
         <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">value_decode</span><span class="p">(</span><span class="n">v</span><span class="p">)</span>
 
     <span class="k">def</span> <span class="nf">set_multi</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">mapping</span><span class="p">):</span>
-        <span class="sd">&quot;&quot;&quot;encode to a new dict to preserve unencoded values in-place when</span>
+<span class="w">        </span><span class="sd">&quot;&quot;&quot;encode to a new dict to preserve unencoded values in-place when</span>
 <span class="sd">           called by `get_or_create_multi`</span>
 <span class="sd">           &quot;&quot;&quot;</span>
         <span class="n">mapping_set</span> <span class="o">=</span> <span class="p">{}</span>
         <span class="k">for</span> <span class="p">(</span><span class="n">k</span><span class="p">,</span> <span class="n">v</span><span class="p">)</span> <span class="ow">in</span> <span class="n">mapping</span><span class="o">.</span><span class="n">iteritems</span><span class="p">():</span>
             <span class="n">mapping_set</span><span class="p">[</span><span class="n">k</span><span class="p">]</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">value_encode</span><span class="p">(</span><span class="n">v</span><span class="p">)</span>
         <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">proxied</span><span class="o">.</span><span class="n">set_multi</span><span class="p">(</span><span class="n">mapping_set</span><span class="p">)</span>
 
@@ -257,15 +255,15 @@
                 <span class="n">translated</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">value_decode</span><span class="p">(</span><span class="n">record</span><span class="p">))</span>
             <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
                 <span class="k">raise</span>
         <span class="k">return</span> <span class="n">translated</span>
 
 
 <span class="k">class</span> <span class="nc">MsgpackProxy</span><span class="p">(</span><span class="n">_EncodedProxy</span><span class="p">):</span>
-    <span class="sd">&quot;&quot;&quot;custom decode/encode for value mangling&quot;&quot;&quot;</span>
+<span class="w">    </span><span class="sd">&quot;&quot;&quot;custom decode/encode for value mangling&quot;&quot;&quot;</span>
 
     <span class="k">def</span> <span class="nf">value_decode</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">v</span><span class="p">):</span>
         <span class="k">if</span> <span class="ow">not</span> <span class="n">v</span> <span class="ow">or</span> <span class="n">v</span> <span class="ow">is</span> <span class="n">NO_VALUE</span><span class="p">:</span>
             <span class="k">return</span> <span class="n">NO_VALUE</span>
         <span class="c1"># you probably want to specify a custom decoder via `object_hook`</span>
         <span class="n">v</span> <span class="o">=</span> <span class="n">msgpack</span><span class="o">.</span><span class="n">unpackb</span><span class="p">(</span><span class="n">payload</span><span class="p">,</span> <span class="n">encoding</span><span class="o">=</span><span class="s2">&quot;utf-8&quot;</span><span class="p">)</span>
         <span class="k">return</span> <span class="n">CachedValue</span><span class="p">(</span><span class="o">*</span><span class="n">v</span><span class="p">)</span>
@@ -344,17 +342,17 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="core_usage.html" title="dogpile Core"
              >next</a> |</li>
         <li class="right" >
           <a href="usage.html" title="Usage Guide"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.1.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.0 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Recipes</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2011-2022 Mike Bayer.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 5.0.2.
+        &#169; Copyright 2011-2023 Mike Bayer.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.2.1.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -8,15 +8,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * dogpile.cache_1.1.8_documentation »
+    * dogpile.cache_1.2.0_documentation »
     * Recipes
 ****** RecipesÂ¶ ******
 ***** Invalidating a group of related keysÂ¶ *****
 This recipe presents a way to track the cache keys related to a particular
 region, for the purposes of invalidating a series of keys that relate to a
 particular id.
 Three cached functions, user_fn_one(), user_fn_two(), user_fn_three() each
@@ -248,10 +248,10 @@
 *** Next topic ***
 dogpile_Core
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * dogpile.cache_1.1.8_documentation »
+    * dogpile.cache_1.2.0_documentation »
     * Recipes
-© Copyright 2011-2022 Mike Bayer. Created using Sphinx 5.0.2.
+© Copyright 2011-2023 Mike Bayer. Created using Sphinx 6.2.1.
```

### Comparing `dogpile.cache-1.1.8/docs/search.html` & `dogpile.cache-1.2.0/docs/search.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Search &#8212; dogpile.cache 1.1.8 documentation</title>
+    <title>Search &#8212; dogpile.cache 1.2.0 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
-    <script src="_static/jquery.js"></script>
-    <script src="_static/underscore.js"></script>
-    <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
     <script src="_static/doctools.js"></script>
+    <script src="_static/sphinx_highlight.js"></script>
     <script src="_static/searchtools.js"></script>
     <script src="_static/language_data.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="#" />
   <script src="searchindex.js" defer></script>
    
 
@@ -29,15 +27,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.1.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.0 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Search</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -89,17 +87,17 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.1.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.0 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Search</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2011-2022 Mike Bayer.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 5.0.2.
+        &#169; Copyright 2011-2023 Mike Bayer.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.2.1.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -4,19 +4,19 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * dogpile.cache_1.1.8_documentation »
+    * dogpile.cache_1.2.0_documentation »
     * Search
 ****** Search ******
 Please activate JavaScript to enable the search functionality.
 Searching for multiple words only shows matches that contain all words.
 [q                   ] [search]
 **** Navigation ****
     * index
     * modules |
-    * dogpile.cache_1.1.8_documentation »
+    * dogpile.cache_1.2.0_documentation »
     * Search
-© Copyright 2011-2022 Mike Bayer. Created using Sphinx 5.0.2.
+© Copyright 2011-2023 Mike Bayer. Created using Sphinx 6.2.1.
```

### Comparing `dogpile.cache-1.1.8/docs/usage.html` & `dogpile.cache-1.2.0/docs/usage.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Usage Guide &#8212; dogpile.cache 1.1.8 documentation</title>
+    <title>Usage Guide &#8212; dogpile.cache 1.2.0 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
-    <script src="_static/jquery.js"></script>
-    <script src="_static/underscore.js"></script>
-    <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
     <script src="_static/doctools.js"></script>
+    <script src="_static/sphinx_highlight.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Recipes" href="recipes.html" />
     <link rel="prev" title="Front Matter" href="front.html" /> 
   </head><body>
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
@@ -32,15 +30,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="recipes.html" title="Recipes"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="front.html" title="Front Matter"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.1.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.0 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Usage Guide</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -123,18 +121,18 @@
 to the pylibmc module.</p>
 </section>
 <section id="region-configuration">
 <h2>Region Configuration<a class="headerlink" href="#region-configuration" title="Permalink to this heading">¶</a></h2>
 <p>The <a class="reference internal" href="api.html#dogpile.cache.region.make_region" title="dogpile.cache.region.make_region"><code class="xref py py-func docutils literal notranslate"><span class="pre">make_region()</span></code></a> function currently calls the <a class="reference internal" href="api.html#dogpile.cache.region.CacheRegion" title="dogpile.cache.region.CacheRegion"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheRegion</span></code></a> constructor directly.</p>
 <dl class="py class">
 <dt class="sig sig-object py">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">dogpile.cache.region.</span></span><span class="sig-name descname"><span class="pre">CacheRegion</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="pre">name:</span> <span class="pre">~typing.Optional[str]</span> <span class="pre">=</span> <span class="pre">None,</span> <span class="pre">function_key_generator:</span> <span class="pre">~typing.Callable[[...],</span> <span class="pre">~typing.Callable[[...],</span> <span class="pre">str]]</span> <span class="pre">=</span> <span class="pre">&lt;function</span> <span class="pre">function_key_generator&gt;,</span> <span class="pre">function_multi_key_generator:</span> <span class="pre">~typing.Callable[[...],</span> <span class="pre">~typing.Callable[[...],</span> <span class="pre">~typing.Sequence[str]]]</span> <span class="pre">=</span> <span class="pre">&lt;function</span> <span class="pre">function_multi_key_generator&gt;,</span> <span class="pre">key_mangler:</span> <span class="pre">~typing.Optional[~typing.Callable[[str],</span> <span class="pre">str]]</span> <span class="pre">=</span> <span class="pre">None,</span> <span class="pre">serializer:</span> <span class="pre">~typing.Optional[~typing.Callable[[~typing.Any],</span> <span class="pre">bytes]]</span> <span class="pre">=</span> <span class="pre">None,</span> <span class="pre">deserializer:</span> <span class="pre">~typing.Optional[~typing.Callable[[bytes],</span> <span class="pre">~typing.Any]]</span> <span class="pre">=</span> <span class="pre">None,</span> <span class="pre">async_creation_runner:</span> <span class="pre">~typing.Optional[~typing.Callable[[~dogpile.cache.region.CacheRegion,</span> <span class="pre">str,</span> <span class="pre">~typing.Callable[[],</span> <span class="pre">~typing.Any],</span> <span class="pre">~dogpile.cache.api.CacheMutex],</span> <span class="pre">None]]</span> <span class="pre">=</span> <span class="pre">None</span></em><span class="sig-paren">)</span></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">dogpile.cache.region.</span></span><span class="sig-name descname"><span class="pre">CacheRegion</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="pre">name:</span> <span class="pre">str</span> <span class="pre">|</span> <span class="pre">None</span> <span class="pre">=</span> <span class="pre">None,</span> <span class="pre">function_key_generator:</span> <span class="pre">~typing.Callable[[...],</span> <span class="pre">~typing.Callable[[...],</span> <span class="pre">str]]</span> <span class="pre">=</span> <span class="pre">&lt;function</span> <span class="pre">function_key_generator&gt;,</span> <span class="pre">function_multi_key_generator:</span> <span class="pre">~typing.Callable[[...],</span> <span class="pre">~typing.Callable[[...],</span> <span class="pre">~typing.Sequence[str]]]</span> <span class="pre">=</span> <span class="pre">&lt;function</span> <span class="pre">function_multi_key_generator&gt;,</span> <span class="pre">key_mangler:</span> <span class="pre">~typing.Callable[[str],</span> <span class="pre">str]</span> <span class="pre">|</span> <span class="pre">None</span> <span class="pre">=</span> <span class="pre">None,</span> <span class="pre">serializer:</span> <span class="pre">~typing.Callable[[~typing.Any],</span> <span class="pre">bytes]</span> <span class="pre">|</span> <span class="pre">None</span> <span class="pre">=</span> <span class="pre">None,</span> <span class="pre">deserializer:</span> <span class="pre">~typing.Callable[[bytes],</span> <span class="pre">~typing.Any]</span> <span class="pre">|</span> <span class="pre">None</span> <span class="pre">=</span> <span class="pre">None,</span> <span class="pre">async_creation_runner:</span> <span class="pre">~typing.Callable[[~dogpile.cache.region.CacheRegion,</span> <span class="pre">str,</span> <span class="pre">~typing.Callable[[],</span> <span class="pre">~typing.Any],</span> <span class="pre">~dogpile.cache.api.CacheMutex],</span> <span class="pre">None]</span> <span class="pre">|</span> <span class="pre">None</span> <span class="pre">=</span> <span class="pre">None</span></em><span class="sig-paren">)</span></dt>
 <dd><p>A front end to a particular cache backend.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.params.name"></span><strong>name</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.params.name">¶</a> – Optional, a string name for the region.
 This isn’t used internally
 but can be accessed via the <code class="docutils literal notranslate"><span class="pre">.name</span></code> parameter, helpful
 for configuring a region from a config file.</p></li>
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.params.function_key_generator"></span><strong>function_key_generator</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.params.function_key_generator">¶</a> – <p>Optional.  A
 function that will produce a “cache key” given
@@ -223,16 +221,26 @@
 <p><span class="versionmodified added">New in version 1.1.0.</span></p>
 </div>
 </p></li>
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.params.deserializer"></span><strong>deserializer</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.params.deserializer">¶</a> – <p>function which will be applied to all values returned
 by the backend.  Defaults to <code class="docutils literal notranslate"><span class="pre">None</span></code>, in which case the
 deserializer recommended by the backend will be used.   Typical
 deserializers include <code class="docutils literal notranslate"><span class="pre">pickle.dumps</span></code> and <code class="docutils literal notranslate"><span class="pre">json.dumps</span></code>.</p>
+<p>Deserializers can raise a <a class="reference internal" href="api.html#dogpile.cache.api.CantDeserializeException" title="dogpile.cache.api.CantDeserializeException"><code class="xref py py-class docutils literal notranslate"><span class="pre">api.CantDeserializeException</span></code></a> if they
+are unable to deserialize the value from the backend, indicating
+deserialization failed and that caching should proceed to re-generate
+a value.  This allows an application that has been updated to gracefully
+re-cache old items which were persisted by a previous version of the
+application and can no longer be successfully deserialized.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.0.</span></p>
+<p><span class="versionmodified added">New in version 1.1.0: </span>added “deserializer” parameter</p>
+</div>
+<div class="versionadded">
+<p><span class="versionmodified added">New in version 1.2.0: </span>added support for
+<a class="reference internal" href="api.html#dogpile.cache.api.CantDeserializeException" title="dogpile.cache.api.CantDeserializeException"><code class="xref py py-class docutils literal notranslate"><span class="pre">api.CantDeserializeException</span></code></a></p>
 </div>
 </p></li>
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.params.async_creation_runner"></span><strong>async_creation_runner</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.params.async_creation_runner">¶</a> – <p>A callable that, when specified,
 will be passed to and called by dogpile.lock when
 there is a stale value present in the cache.  It will be passed the
 mutex and is responsible releasing that mutex when finished.
 This can be used to defer the computation of expensive creator
@@ -240,15 +248,15 @@
 background thread, a long-running queue, or a task manager system
 like Celery.</p>
 <p>For a specific example using async_creation_runner, new values can
 be created in a background thread like so:</p>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="kn">import</span> <span class="nn">threading</span>
 
 <span class="k">def</span> <span class="nf">async_creation_runner</span><span class="p">(</span><span class="n">cache</span><span class="p">,</span> <span class="n">somekey</span><span class="p">,</span> <span class="n">creator</span><span class="p">,</span> <span class="n">mutex</span><span class="p">):</span>
-    <span class="sd">&#39;&#39;&#39; Used by dogpile.core:Lock when appropriate  &#39;&#39;&#39;</span>
+<span class="w">    </span><span class="sd">&#39;&#39;&#39; Used by dogpile.core:Lock when appropriate  &#39;&#39;&#39;</span>
     <span class="k">def</span> <span class="nf">runner</span><span class="p">():</span>
         <span class="k">try</span><span class="p">:</span>
             <span class="n">value</span> <span class="o">=</span> <span class="n">creator</span><span class="p">()</span>
             <span class="n">cache</span><span class="o">.</span><span class="n">set</span><span class="p">(</span><span class="n">somekey</span><span class="p">,</span> <span class="n">value</span><span class="p">)</span>
         <span class="k">finally</span><span class="p">:</span>
             <span class="n">mutex</span><span class="o">.</span><span class="n">release</span><span class="p">()</span>
 
@@ -287,20 +295,20 @@
 </dd></dl>
 
 <p>One you have a <a class="reference internal" href="api.html#dogpile.cache.region.CacheRegion" title="dogpile.cache.region.CacheRegion"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheRegion</span></code></a>, the <a class="reference internal" href="api.html#dogpile.cache.region.CacheRegion.cache_on_arguments" title="dogpile.cache.region.CacheRegion.cache_on_arguments"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.cache_on_arguments()</span></code></a> method can
 be used to decorate functions, but the cache itself can’t be used until
 <a class="reference internal" href="api.html#dogpile.cache.region.CacheRegion.configure" title="dogpile.cache.region.CacheRegion.configure"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.configure()</span></code></a> is called.  The interface for that method is as follows:</p>
 <dl class="py method">
 <dt class="sig sig-object py">
-<span class="sig-prename descclassname"><span class="pre">CacheRegion.</span></span><span class="sig-name descname"><span class="pre">configure</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">backend</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">expiration_time</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><span class="pre">float</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">timedelta</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">arguments</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Mapping</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">_config_argument_dict</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Mapping</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">_config_prefix</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">wrap</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">Union</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="api.html#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><span class="pre">ProxyBackend</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Type</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="api.html#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><span class="pre">ProxyBackend</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">()</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">replace_existing_backend</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">region_invalidator</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="api.html#dogpile.cache.region.RegionInvalidationStrategy" title="dogpile.cache.region.RegionInvalidationStrategy"><span class="pre">RegionInvalidationStrategy</span></a><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="api.html#dogpile.cache.region.CacheRegion" title="dogpile.cache.region.CacheRegion"><span class="pre">CacheRegion</span></a></span></span></dt>
+<span class="sig-prename descclassname"><span class="pre">CacheRegion.</span></span><span class="sig-name descname"><span class="pre">configure</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">backend</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">expiration_time</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">timedelta</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">arguments</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Mapping</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">_config_argument_dict</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Mapping</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">_config_prefix</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">wrap</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="api.html#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><span class="pre">ProxyBackend</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">Type</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="api.html#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><span class="pre">ProxyBackend</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">()</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">replace_existing_backend</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">region_invalidator</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="api.html#dogpile.cache.region.RegionInvalidationStrategy" title="dogpile.cache.region.RegionInvalidationStrategy"><span class="pre">RegionInvalidationStrategy</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="api.html#dogpile.cache.region.CacheRegion" title="dogpile.cache.region.CacheRegion"><span class="pre">CacheRegion</span></a></span></span></dt>
 <dd><p>Configure a <a class="reference internal" href="api.html#dogpile.cache.region.CacheRegion" title="dogpile.cache.region.CacheRegion"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheRegion</span></code></a>.</p>
 <p>The <a class="reference internal" href="api.html#dogpile.cache.region.CacheRegion" title="dogpile.cache.region.CacheRegion"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheRegion</span></code></a> itself
 is returned.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.configure.params.backend"></span><strong>backend</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.configure.params.backend">¶</a> – Required.  This is the name of the
 <a class="reference internal" href="api.html#dogpile.cache.api.CacheBackend" title="dogpile.cache.api.CacheBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheBackend</span></code></a> to use, and is resolved by loading
 the class from the <code class="docutils literal notranslate"><span class="pre">dogpile.cache</span></code> entrypoint.</p></li>
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.configure.params.expiration_time"></span><strong>expiration_time</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.configure.params.expiration_time">¶</a> – <p>Optional.  The expiration time passed
 to the dogpile system.  May be passed as an integer number
 of seconds, or as a <code class="docutils literal notranslate"><span class="pre">datetime.timedelta</span></code> value.</p>
@@ -405,15 +413,15 @@
 Passing the flag <code class="docutils literal notranslate"><span class="pre">ignore_expiration=True</span></code> bypasses
 the invalidation time check.</p>
 <div class="versionadded">
 <p><span class="versionmodified added">New in version 0.3.0: </span>Support for the <a class="reference internal" href="api.html#dogpile.cache.region.CacheRegion.invalidate" title="dogpile.cache.region.CacheRegion.invalidate"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.invalidate()</span></code></a>
 method.</p>
 </div>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.get.params.key"></span><strong>key</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.get.params.key">¶</a> – Key to be retrieved. While it’s typical for a key to be a
 string, it is ultimately passed directly down to the cache backend,
 before being optionally processed by the key_mangler function, so can
 be of any type recognized by the backend or by the key_mangler
 function, if present.</p></li>
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.get.params.expiration_time"></span><strong>expiration_time</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.get.params.expiration_time">¶</a> – <p>Optional expiration time value
@@ -450,15 +458,15 @@
 <p><a class="reference internal" href="api.html#dogpile.cache.region.CacheRegion.set" title="dogpile.cache.region.CacheRegion.set"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.set()</span></code></a></p>
 <p><a class="reference internal" href="api.html#dogpile.cache.region.CacheRegion.delete" title="dogpile.cache.region.CacheRegion.delete"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.delete()</span></code></a></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py">
-<span class="sig-prename descclassname"><span class="pre">CacheRegion.</span></span><span class="sig-name descname"><span class="pre">get_or_create</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">creator</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">...</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">expiration_time</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">float</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">should_cache_fn</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">creator_args</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Tuple</span><span class="p"><span class="pre">[</span></span><span class="pre">Any</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Mapping</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Any</span></span></span></dt>
+<span class="sig-prename descclassname"><span class="pre">CacheRegion.</span></span><span class="sig-name descname"><span class="pre">get_or_create</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">creator</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">...</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">expiration_time</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">should_cache_fn</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">creator_args</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Tuple</span><span class="p"><span class="pre">[</span></span><span class="pre">Any</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Mapping</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Any</span></span></span></dt>
 <dd><p>Return a cached value based on the given key.</p>
 <p>If the value does not exist or is considered to be expired
 based on its creation time, the given
 creation function may or may not be used to recreate the value
 and persist the newly generated value in the cache.</p>
 <p>Whether or not the function is used depends on if the
 <em>dogpile lock</em> can be acquired or not.  If it can’t, it means
@@ -475,15 +483,15 @@
 lock to generate a new value, or will wait
 until the lock is released to return the new value.</p>
 <div class="versionchanged">
 <p><span class="versionmodified changed">Changed in version 0.3.0: </span>The value is unconditionally regenerated if the creation
 time is older than the last call to <a class="reference internal" href="api.html#dogpile.cache.region.CacheRegion.invalidate" title="dogpile.cache.region.CacheRegion.invalidate"><code class="xref py py-meth docutils literal notranslate"><span class="pre">invalidate()</span></code></a>.</p>
 </div>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.get_or_create.params.key"></span><strong>key</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.get_or_create.params.key">¶</a> – Key to be retrieved. While it’s typical for a key to be a
 string, it is ultimately passed directly down to the cache backend,
 before being optionally processed by the key_mangler function, so can
 be of any type recognized by the backend or by the key_mangler
 function, if present.</p></li>
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.get_or_create.params.creator"></span><strong>creator</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.get_or_create.params.creator">¶</a> – function which creates a new value.</p></li>
@@ -551,15 +559,15 @@
 <dd><p>Remove a value from the cache.</p>
 <p>This operation is idempotent (can be called multiple times, or on a
 non-existent key, safely)</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py">
-<span class="sig-prename descclassname"><span class="pre">CacheRegion.</span></span><span class="sig-name descname"><span class="pre">cache_on_arguments</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="pre">namespace:</span> <span class="pre">~typing.Optional[str]</span> <span class="pre">=</span> <span class="pre">None,</span> <span class="pre">expiration_time:</span> <span class="pre">~typing.Optional[~typing.Union[float,</span> <span class="pre">~typing.Callable[[],</span> <span class="pre">float]]]</span> <span class="pre">=</span> <span class="pre">None,</span> <span class="pre">should_cache_fn:</span> <span class="pre">~typing.Optional[~typing.Callable[[~typing.Any],</span> <span class="pre">bool]]</span> <span class="pre">=</span> <span class="pre">None,</span> <span class="pre">to_str:</span> <span class="pre">~typing.Callable[[~typing.Any],</span> <span class="pre">str]</span> <span class="pre">=</span> <span class="pre">&lt;class</span> <span class="pre">'str'&gt;,</span> <span class="pre">function_key_generator:</span> <span class="pre">~typing.Optional[~typing.Callable[[...],</span> <span class="pre">~typing.Callable[[...],</span> <span class="pre">str]]]</span> <span class="pre">=</span> <span class="pre">None</span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">...</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">...</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></span></dt>
+<span class="sig-prename descclassname"><span class="pre">CacheRegion.</span></span><span class="sig-name descname"><span class="pre">cache_on_arguments</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="pre">namespace:</span> <span class="pre">str</span> <span class="pre">|</span> <span class="pre">None</span> <span class="pre">=</span> <span class="pre">None,</span> <span class="pre">expiration_time:</span> <span class="pre">float</span> <span class="pre">|</span> <span class="pre">~typing.Callable[[],</span> <span class="pre">float]</span> <span class="pre">|</span> <span class="pre">None</span> <span class="pre">=</span> <span class="pre">None,</span> <span class="pre">should_cache_fn:</span> <span class="pre">~typing.Callable[[~typing.Any],</span> <span class="pre">bool]</span> <span class="pre">|</span> <span class="pre">None</span> <span class="pre">=</span> <span class="pre">None,</span> <span class="pre">to_str:</span> <span class="pre">~typing.Callable[[~typing.Any],</span> <span class="pre">str]</span> <span class="pre">=</span> <span class="pre">&lt;class</span> <span class="pre">'str'&gt;,</span> <span class="pre">function_key_generator:</span> <span class="pre">~typing.Callable[[...],</span> <span class="pre">~typing.Callable[[...],</span> <span class="pre">str]]</span> <span class="pre">|</span> <span class="pre">None</span> <span class="pre">=</span> <span class="pre">None</span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">...</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">...</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></span></dt>
 <dd><p>A function decorator that will cache the return
 value of the function using a key derived from the
 function itself and its arguments.</p>
 <p>The decorator internally makes use of the
 <a class="reference internal" href="api.html#dogpile.cache.region.CacheRegion.get_or_create" title="dogpile.cache.region.CacheRegion.get_or_create"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get_or_create()</span></code></a> method to access the
 cache and conditionally call the function.  See that
 method for additional behavioral details.</p>
@@ -679,15 +687,15 @@
 by the decorator before it becomes an instance method.</p>
 <p>The function key generation can be entirely replaced
 on a per-region basis using the <code class="docutils literal notranslate"><span class="pre">function_key_generator</span></code>
 argument present on <a class="reference internal" href="api.html#dogpile.cache.region.make_region" title="dogpile.cache.region.make_region"><code class="xref py py-func docutils literal notranslate"><span class="pre">make_region()</span></code></a> and
 <a class="reference internal" href="api.html#dogpile.cache.region.CacheRegion" title="dogpile.cache.region.CacheRegion"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheRegion</span></code></a>. If defaults to
 <a class="reference internal" href="api.html#dogpile.cache.util.function_key_generator" title="dogpile.cache.util.function_key_generator"><code class="xref py py-func docutils literal notranslate"><span class="pre">function_key_generator()</span></code></a>.</p>
 <dl class="field-list simple">
-<dt class="field-odd">Parameters</dt>
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.cache_on_arguments.params.namespace"></span><strong>namespace</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.cache_on_arguments.params.namespace">¶</a> – optional string argument which will be
 established as part of the cache key.   This may be needed
 to disambiguate functions of the same name within the same
 source file, such as those
 associated with classes - note that the decorator itself
 can’t see the parent class on a function as the class is
@@ -939,17 +947,17 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="recipes.html" title="Recipes"
              >next</a> |</li>
         <li class="right" >
           <a href="front.html" title="Front Matter"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.1.8 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.2.0 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Usage Guide</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
-        &#169; Copyright 2011-2022 Mike Bayer.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 5.0.2.
+        &#169; Copyright 2011-2023 Mike Bayer.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.2.1.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -8,15 +8,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * dogpile.cache_1.1.8_documentation »
+    * dogpile.cache_1.2.0_documentation »
     * Usage Guide
 ****** Usage GuideÂ¶ ******
 ***** OverviewÂ¶ *****
 At the time of this writing, popular key/value servers include Memcached, Redis
 and many others. While these tools all have different usage focuses, they all
 have in common that the storage model is based on the retrieval of a value
 based on a key; as such, they are all potentially suitable for caching,
@@ -83,35 +83,34 @@
 is the expiration time passed to the Dogpile lock, and arguments, which are
 arguments used directly by the backend - in this case we are using arguments
 that are passed directly to the pylibmc module.
 
 ***** Region ConfigurationÂ¶ *****
 The make_region() function currently calls the CacheRegion constructor
 directly.
-  classdogpile.cache.region.CacheRegion(name: ~typing.Optional[str] = None,
+  classdogpile.cache.region.CacheRegion(name: str | None = None,
   function_key_generator: ~typing.Callable[[...], ~typing.Callable[[...], str]]
   = <function function_key_generator>, function_multi_key_generator:
   ~typing.Callable[[...], ~typing.Callable[[...], ~typing.Sequence[str]]] =
-  <function function_multi_key_generator>, key_mangler: ~typing.Optional
-  [~typing.Callable[[str], str]] = None, serializer: ~typing.Optional
-  [~typing.Callable[[~typing.Any], bytes]] = None, deserializer:
-  ~typing.Optional[~typing.Callable[[bytes], ~typing.Any]] = None,
-  async_creation_runner: ~typing.Optional[~typing.Callable[
-  [~dogpile.cache.region.CacheRegion, str, ~typing.Callable[[], ~typing.Any],
-  ~dogpile.cache.api.CacheMutex], None]] = None)
+  <function function_multi_key_generator>, key_mangler: ~typing.Callable[[str],
+  str] | None = None, serializer: ~typing.Callable[[~typing.Any], bytes] | None
+  = None, deserializer: ~typing.Callable[[bytes], ~typing.Any] | None = None,
+  async_creation_runner: ~typing.Callable[[~dogpile.cache.region.CacheRegion,
+  str, ~typing.Callable[[], ~typing.Any], ~dogpile.cache.api.CacheMutex], None]
+  | None = None)
       A front end to a particular cache backend.
 One you have a CacheRegion, the CacheRegion.cache_on_arguments() method can be
 used to decorate functions, but the cache itself canât be used until
 CacheRegion.configure() is called. The interface for that method is as follows:
-  CacheRegion.configure(backend: str, expiration_time: Optional[Union[float,
-  timedelta]] = None, arguments: Optional[Mapping[str, Any]] = None,
-  _config_argument_dict: Optional[Mapping[str, Any]] = None, _config_prefix:
-  Optional[str] = None, wrap: Sequence[Union[ProxyBackend, Type[ProxyBackend]]]
-  = (), replace_existing_backend: bool = False, region_invalidator: Optional
-  [RegionInvalidationStrategy] = None) &#x2192; CacheRegion
+  CacheRegion.configure(backend: str, expiration_time: float | timedelta | None
+  = None, arguments: Mapping[str, Any] | None = None, _config_argument_dict:
+  Mapping[str, Any] | None = None, _config_prefix: str | None = None, wrap:
+  Sequence[ProxyBackend | Type[ProxyBackend]] = (), replace_existing_backend:
+  bool = False, region_invalidator: RegionInvalidationStrategy | None = None)
+  &#x2192; CacheRegion
       Configure a CacheRegion.
       The CacheRegion itself is returned.
 The CacheRegion can also be configured from a dictionary, using the
 CacheRegion.configure_from_config() method:
   CacheRegion.configure_from_config(config_dict, prefix)
       Configure from a configuration dictionary and a prefix.
       Example:
@@ -157,17 +156,17 @@
       New in version 0.3.0: Support for the CacheRegion.invalidate() method.
       See also
       CacheRegion.get_multi()
       CacheRegion.get_or_create()
       CacheRegion.set()
       CacheRegion.delete()
   CacheRegion.get_or_create(key: str, creator: Callable[[...], Any],
-  expiration_time: Optional[float] = None, should_cache_fn: Optional[Callable[
-  [Any], bool]] = None, creator_args: Optional[Tuple[Any, Mapping[str, Any]]] =
-  None) &#x2192; Any
+  expiration_time: float | None = None, should_cache_fn: Callable[[Any], bool]
+  | None = None, creator_args: Tuple[Any, Mapping[str, Any]] | None = None)
+  &#x2192; Any
       Return a cached value based on the given key.
       If the value does not exist or is considered to be expired based on its
       creation time, the given creation function may or may not be used to
       recreate the value and persist the newly generated value in the cache.
       Whether or not the function is used depends on if the dogpile lock can be
       acquired or not. If it canât, it means a different thread or process is
       already running a creation function for this key against the cache. When
@@ -189,21 +188,20 @@
       CacheRegion.get_or_create_multi() - multiple key/value version
   CacheRegion.set(key: str, value: Any) &#x2192; None
       Place a new value in the cache under the given key.
   CacheRegion.delete(key: str) &#x2192; None
       Remove a value from the cache.
       This operation is idempotent (can be called multiple times, or on a non-
       existent key, safely)
-  CacheRegion.cache_on_arguments(namespace: ~typing.Optional[str] = None,
-  expiration_time: ~typing.Optional[~typing.Union[float, ~typing.Callable[[],
-  float]]] = None, should_cache_fn: ~typing.Optional[~typing.Callable[
-  [~typing.Any], bool]] = None, to_str: ~typing.Callable[[~typing.Any], str] =
-  <class 'str'>, function_key_generator: ~typing.Optional[~typing.Callable[
-  [...], ~typing.Callable[[...], str]]] = None) &#x2192; Callable[[Callable[
-  [...], Any]], Callable[[...], Any]]
+  CacheRegion.cache_on_arguments(namespace: str | None = None, expiration_time:
+  float | ~typing.Callable[[], float] | None = None, should_cache_fn:
+  ~typing.Callable[[~typing.Any], bool] | None = None, to_str: ~typing.Callable
+  [[~typing.Any], str] = <class 'str'>, function_key_generator:
+  ~typing.Callable[[...], ~typing.Callable[[...], str]] | None = None) &#x2192;
+  Callable[[Callable[[...], Any]], Callable[[...], Any]]
       A function decorator that will cache the return value of the function
       using a key derived from the function itself and its arguments.
       The decorator internally makes use of the CacheRegion.get_or_create()
       method to access the cache and conditionally call the function. See that
       method for additional behavioral details.
       E.g.:
       @someregion.cache_on_arguments()
@@ -430,10 +428,10 @@
 *** Next topic ***
 Recipes
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * dogpile.cache_1.1.8_documentation »
+    * dogpile.cache_1.2.0_documentation »
     * Usage Guide
-© Copyright 2011-2022 Mike Bayer. Created using Sphinx 5.0.2.
+© Copyright 2011-2023 Mike Bayer. Created using Sphinx 6.2.1.
```

### Comparing `dogpile.cache-1.1.8/dogpile/cache/api.py` & `dogpile.cache-1.2.0/dogpile/cache/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,14 +47,23 @@
 
 
 KeyManglerType = Callable[[KeyType], KeyType]
 Serializer = Callable[[ValuePayload], bytes]
 Deserializer = Callable[[bytes], ValuePayload]
 
 
+class CantDeserializeException(Exception):
+    """Exception indicating deserialization failed, and that caching
+    should proceed to re-generate a value
+
+    .. versionadded:: 1.2.0
+
+    """
+
+
 class CacheMutex(abc.ABC):
     """Describes a mutexing object with acquire and release methods.
 
     This is an abstract base class; any object that has acquire/release
     methods may be used.
 
     .. versionadded:: 1.1
```

### Comparing `dogpile.cache-1.1.8/dogpile/cache/backends/__init__.py` & `dogpile.cache-1.2.0/dogpile/cache/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/dogpile/cache/backends/file.py` & `dogpile.cache-1.2.0/dogpile/cache/backends/file.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/dogpile/cache/backends/memcached.py` & `dogpile.cache-1.2.0/dogpile/cache/backends/memcached.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/dogpile/cache/backends/memory.py` & `dogpile.cache-1.2.0/dogpile/cache/backends/memory.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/dogpile/cache/backends/null.py` & `dogpile.cache-1.2.0/dogpile/cache/backends/null.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/dogpile/cache/backends/redis.py` & `dogpile.cache-1.2.0/dogpile/cache/backends/redis.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/dogpile/cache/exception.py` & `dogpile.cache-1.2.0/dogpile/cache/exception.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/dogpile/cache/plugins/mako_cache.py` & `dogpile.cache-1.2.0/dogpile/cache/plugins/mako_cache.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/dogpile/cache/proxy.py` & `dogpile.cache-1.2.0/dogpile/cache/proxy.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/dogpile/cache/region.py` & `dogpile.cache-1.2.0/dogpile/cache/region.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 from . import exception
 from .api import BackendArguments
 from .api import BackendFormatted
 from .api import CachedValue
 from .api import CacheMutex
 from .api import CacheReturnType
+from .api import CantDeserializeException
 from .api import KeyType
 from .api import MetaDataType
 from .api import NO_VALUE
 from .api import SerializedReturnType
 from .api import Serializer
 from .api import ValuePayload
 from .backends import _backend_loader
@@ -324,15 +325,25 @@
      .. versionadded:: 1.1.0
 
     :param deserializer: function which will be applied to all values returned
      by the backend.  Defaults to ``None``, in which case the
      deserializer recommended by the backend will be used.   Typical
      deserializers include ``pickle.dumps`` and ``json.dumps``.
 
-     .. versionadded:: 1.1.0
+     Deserializers can raise a :class:`.api.CantDeserializeException` if they
+     are unable to deserialize the value from the backend, indicating
+     deserialization failed and that caching should proceed to re-generate
+     a value.  This allows an application that has been updated to gracefully
+     re-cache old items which were persisted by a previous version of the
+     application and can no longer be successfully deserialized.
+
+     .. versionadded:: 1.1.0 added "deserializer" parameter
+
+     .. versionadded:: 1.2.0 added support for
+        :class:`.api.CantDeserializeException`
 
     :param async_creation_runner:  A callable that, when specified,
      will be passed to and called by dogpile.lock when
      there is a stale value present in the cache.  It will be passed the
      mutex and is responsible releasing that mutex when finished.
      This can be used to defer the computation of expensive creator
      functions to later points in the future by way of, for example, a
@@ -1215,16 +1226,20 @@
             return NO_VALUE
 
         assert self.deserializer
         byte_value = cast(bytes, value)
 
         bytes_metadata, _, bytes_payload = byte_value.partition(b"|")
         metadata = json.loads(bytes_metadata)
-        payload = self.deserializer(bytes_payload)
-        return CachedValue(payload, metadata)
+        try:
+            payload = self.deserializer(bytes_payload)
+        except CantDeserializeException:
+            return NO_VALUE
+        else:
+            return CachedValue(payload, metadata)
 
     def _serialize_cached_value_elements(
         self, payload: ValuePayload, metadata: MetaDataType
     ) -> bytes:
         serializer = cast(Serializer, self.serializer)
 
         return b"%b|%b" % (
@@ -1243,15 +1258,16 @@
         """
         if metadata is None:
             metadata = self._gen_metadata()
 
         return self._serialize_cached_value_elements(payload, metadata)
 
     def _serialized_cached_value(self, value: CachedValue) -> BackendFormatted:
-        """Return a backend formatted representation of a :class:`.CachedValue`.
+        """Return a backend formatted representation of a
+        :class:`.CachedValue`.
 
         If a serializer is in use then this will return a string representation
         with the value formatted by the serializer.
 
         """
 
         assert self.serializer
```

### Comparing `dogpile.cache-1.1.8/dogpile/cache/util.py` & `dogpile.cache-1.2.0/dogpile/cache/util.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/dogpile/core.py` & `dogpile.cache-1.2.0/dogpile/core.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/dogpile/lock.py` & `dogpile.cache-1.2.0/dogpile/lock.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/dogpile/util/compat.py` & `dogpile.cache-1.2.0/dogpile/util/compat.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/dogpile/util/langhelpers.py` & `dogpile.cache-1.2.0/dogpile/util/langhelpers.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/dogpile/util/nameregistry.py` & `dogpile.cache-1.2.0/dogpile/util/nameregistry.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/dogpile/util/readwrite_lock.py` & `dogpile.cache-1.2.0/dogpile/util/readwrite_lock.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/dogpile.cache.egg-info/PKG-INFO` & `dogpile.cache-1.2.0/dogpile.cache.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: dogpile.cache
-Version: 1.1.8
+Version: 1.2.0
 Summary: A caching front-end based on the Dogpile lock.
 Home-page: https://github.com/sqlalchemy/dogpile.cache
 Author: Mike Bayer
 Author-email: mike_mp@zzzcomputing.com
 License: MIT
 Project-URL: Documentation, https://dogpilecache.sqlalchemy.org
 Project-URL: Issue Tracker, https://github.com/sqlalchemy/dogpile.cache/
 Keywords: caching
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
@@ -107,9 +106,7 @@
 `Code of Conduct <https://www.sqlalchemy.org/codeofconduct.html>`_.
 
 License
 -------
 
 Dogpile is distributed under the `MIT license
 <https://opensource.org/licenses/MIT>`_.
-
-
```

### Comparing `dogpile.cache-1.1.8/dogpile.cache.egg-info/SOURCES.txt` & `dogpile.cache-1.2.0/dogpile.cache.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -42,33 +42,29 @@
 docs/_sources/api.rst.txt
 docs/_sources/changelog.rst.txt
 docs/_sources/core_usage.rst.txt
 docs/_sources/front.rst.txt
 docs/_sources/index.rst.txt
 docs/_sources/recipes.rst.txt
 docs/_sources/usage.rst.txt
-docs/_static/_sphinx_javascript_frameworks_compat.js
 docs/_static/basic.css
 docs/_static/changelog.css
 docs/_static/doctools.js
 docs/_static/documentation_options.js
 docs/_static/file.png
-docs/_static/jquery-3.6.0.js
-docs/_static/jquery.js
 docs/_static/language_data.js
 docs/_static/minus.png
 docs/_static/nature.css
 docs/_static/nature_override.css
 docs/_static/plus.png
 docs/_static/pygments.css
 docs/_static/searchtools.js
 docs/_static/site_custom_css.css
+docs/_static/sphinx_highlight.js
 docs/_static/sphinx_paramlinks.css
-docs/_static/underscore-1.13.1.js
-docs/_static/underscore.js
 docs/build/Makefile
 docs/build/api.rst
 docs/build/builder.py
 docs/build/changelog.rst
 docs/build/conf.py
 docs/build/core_usage.rst
 docs/build/front.rst
```

### Comparing `dogpile.cache-1.1.8/hash_port.py` & `dogpile.cache-1.2.0/hash_port.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/log_tests.ini` & `dogpile.cache-1.2.0/log_tests.ini`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/setup.cfg` & `dogpile.cache-1.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/setup.py` & `dogpile.cache-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/tests/cache/__init__.py` & `dogpile.cache-1.2.0/tests/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/tests/cache/_fixtures.py` & `dogpile.cache-1.2.0/tests/cache/_fixtures.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 import pytest
 
 from dogpile.cache import CacheRegion
 from dogpile.cache import register_backend
 from dogpile.cache.api import CacheBackend
 from dogpile.cache.api import CacheMutex
+from dogpile.cache.api import CantDeserializeException
 from dogpile.cache.api import NO_VALUE
 from dogpile.cache.region import _backend_loader
 from . import assert_raises_message
 from . import eq_
 
 
 class _GenericBackendFixture(object):
@@ -376,22 +377,39 @@
             raise Exception("boom")
 
         assert_raises_message(
             Exception, "boom", reg.get_or_create, "some_key", boom
         )
 
 
+def raise_cant_deserialize_exception(v):
+    raise CantDeserializeException()
+
+
 class _GenericSerializerTest(TestCase):
     # Inheriting from this class will make test cases
     # use these serialization arguments
     region_args = {
         "serializer": lambda v: json.dumps(v).encode("ascii"),
         "deserializer": json.loads,
     }
 
+    def test_serializer_cant_deserialize(self):
+        region = self._region(
+            region_args={
+                "serializer": self.region_args["serializer"],
+                "deserializer": raise_cant_deserialize_exception,
+            }
+        )
+
+        value = {"foo": ["bar", 1, False, None]}
+        region.set("k", value)
+        asserted = region.get("k")
+        eq_(asserted, NO_VALUE)
+
     def test_uses_serializer(self):
         region = self._region()
 
         backend = region.backend
         value = {"foo": ["bar", 1, False, None]}
         region.set("k", value)
```

### Comparing `dogpile.cache-1.1.8/tests/cache/plugins/test_mako_cache.py` & `dogpile.cache-1.2.0/tests/cache/plugins/test_mako_cache.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/tests/cache/test_dbm_backend.py` & `dogpile.cache-1.2.0/tests/cache/test_dbm_backend.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/tests/cache/test_decorator.py` & `dogpile.cache-1.2.0/tests/cache/test_decorator.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/tests/cache/test_memcached_backend.py` & `dogpile.cache-1.2.0/tests/cache/test_memcached_backend.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/tests/cache/test_null_backend.py` & `dogpile.cache-1.2.0/tests/cache/test_null_backend.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/tests/cache/test_redis_backend.py` & `dogpile.cache-1.2.0/tests/cache/test_redis_backend.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/tests/cache/test_redis_sentinel_backend.py` & `dogpile.cache-1.2.0/tests/cache/test_redis_sentinel_backend.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/tests/cache/test_region.py` & `dogpile.cache-1.2.0/tests/cache/test_region.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/tests/conftest.py` & `dogpile.cache-1.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/tests/test_backgrounding.py` & `dogpile.cache-1.2.0/tests/test_backgrounding.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/tests/test_lock.py` & `dogpile.cache-1.2.0/tests/test_lock.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/tests/test_utils.py` & `dogpile.cache-1.2.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/tests/tls/ca-root.crt` & `dogpile.cache-1.2.0/tests/tls/ca-root.crt`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/tests/tls/client-ca-root.crt` & `dogpile.cache-1.2.0/tests/tls/client-ca-root.crt`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/tests/tls/client.crt` & `dogpile.cache-1.2.0/tests/tls/client.crt`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/tests/tls/client.key` & `dogpile.cache-1.2.0/tests/tls/client.key`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/tests/tls/server.key` & `dogpile.cache-1.2.0/tests/tls/server.key`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/tests/tls/server_chain.pem` & `dogpile.cache-1.2.0/tests/tls/server_chain.pem`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/tests/util/test_nameregistry.py` & `dogpile.cache-1.2.0/tests/util/test_nameregistry.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.1.8/tox.ini` & `dogpile.cache-1.2.0/tox.ini`

 * *Files identical despite different names*

