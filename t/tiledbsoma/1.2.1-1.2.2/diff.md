# Comparing `tmp/tiledbsoma-1.2.1.tar.gz` & `tmp/tiledbsoma-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiledbsoma-1.2.1.tar", last modified: Tue Mar 28 13:30:29 2023, max compression
+gzip compressed data, was "tiledbsoma-1.2.2.tar", last modified: Wed Apr 26 00:03:44 2023, max compression
```

## Comparing `tiledbsoma-1.2.1.tar` & `tiledbsoma-1.2.2.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:30:29.535375 tiledbsoma-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-03-28 13:30:26.000000 tiledbsoma-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     5023 2023-03-28 13:30:29.535375 tiledbsoma-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3066 2023-03-28 13:30:26.000000 tiledbsoma-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-03-28 13:30:28.000000 tiledbsoma-1.2.1/RELEASE-VERSION
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:30:29.519375 tiledbsoma-1.2.1/dist_links/
--rw-r--r--   0 runner    (1001) docker     (122)      508 2023-03-28 13:30:26.000000 tiledbsoma-1.2.1/dist_links/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:30:29.519375 tiledbsoma-1.2.1/dist_links/libtiledbsoma/
--rw-r--r--   0 runner    (1001) docker     (122)     9356 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4058 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:30:29.519375 tiledbsoma-1.2.1/dist_links/libtiledbsoma/cmake/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:30:29.523375 tiledbsoma-1.2.1/dist_links/libtiledbsoma/cmake/Modules/
--rw-r--r--   0 runner    (1001) docker     (122)     2893 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/cmake/Modules/CheckAVX2Support.cmake
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/cmake/Modules/FindCatch_EP.cmake
--rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/cmake/Modules/FindClangTools.cmake
--rw-r--r--   0 runner    (1001) docker     (122)     4894 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/cmake/Modules/FindSpdlog_EP.cmake
--rw-r--r--   0 runner    (1001) docker     (122)     5746 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/cmake/Modules/FindTileDB_EP.cmake
--rw-r--r--   0 runner    (1001) docker     (122)     3643 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/cmake/Modules/TileDBCommon.cmake
--rw-r--r--   0 runner    (1001) docker     (122)     4906 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/cmake/Superbuild.cmake
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:30:29.523375 tiledbsoma-1.2.1/dist_links/libtiledbsoma/cmake/inputs/
--rw-r--r--   0 runner    (1001) docker     (122)      724 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/cmake/inputs/Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (122)      467 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/cmake/inputs/tiledbsoma.pc.in
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:30:29.523375 tiledbsoma-1.2.1/dist_links/libtiledbsoma/cmake/patches/
--rw-r--r--   0 runner    (1001) docker     (122)      736 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/cmake/patches/spdlog.patch
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:30:29.523375 tiledbsoma-1.2.1/dist_links/libtiledbsoma/doc/
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/doc/README.md
--rw-r--r--   0 runner    (1001) docker     (122)    36556 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/doc/reader.svg
--rw-r--r--   0 runner    (1001) docker     (122)     2198 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/doc/reader.uml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:30:29.523375 tiledbsoma-1.2.1/dist_links/libtiledbsoma/external/
--rw-r--r--   0 runner    (1001) docker     (122)     2774 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/external/.clang-format
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:30:29.515375 tiledbsoma-1.2.1/dist_links/libtiledbsoma/external/include/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:30:29.527375 tiledbsoma-1.2.1/dist_links/libtiledbsoma/external/include/span/
--rw-r--r--   0 runner    (1001) docker     (122)    17276 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/external/include/span/span.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:30:29.527375 tiledbsoma-1.2.1/dist_links/libtiledbsoma/external/include/thread_pool/
--rw-r--r--   0 runner    (1001) docker     (122)     7148 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/external/include/thread_pool/producer_consumer_queue.h
--rw-r--r--   0 runner    (1001) docker     (122)    17772 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/external/include/thread_pool/status.h
--rw-r--r--   0 runner    (1001) docker     (122)     5561 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/external/include/thread_pool/thread_pool.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:30:29.515375 tiledbsoma-1.2.1/dist_links/libtiledbsoma/external/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:30:29.527375 tiledbsoma-1.2.1/dist_links/libtiledbsoma/external/src/thread_pool/
--rw-r--r--   0 runner    (1001) docker     (122)     3092 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/external/src/thread_pool/status.cc
--rw-r--r--   0 runner    (1001) docker     (122)     6700 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/external/src/thread_pool/thread_pool.cc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:30:29.515375 tiledbsoma-1.2.1/dist_links/libtiledbsoma/include/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:30:29.531375 tiledbsoma-1.2.1/dist_links/libtiledbsoma/include/tiledbsoma/
--rw-r--r--   0 runner    (1001) docker     (122)     3767 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/include/tiledbsoma/array_buffers.h
--rw-r--r--   0 runner    (1001) docker     (122)     7215 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/include/tiledbsoma/arrow_adapter.h
--rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/include/tiledbsoma/carrow.h
--rw-r--r--   0 runner    (1001) docker     (122)     7819 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/include/tiledbsoma/column_buffer.h
--rw-r--r--   0 runner    (1001) docker     (122)     1885 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/include/tiledbsoma/common.h
--rw-r--r--   0 runner    (1001) docker     (122)     2959 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/include/tiledbsoma/logger_public.h
--rw-r--r--   0 runner    (1001) docker     (122)    10187 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/include/tiledbsoma/managed_query.h
--rw-r--r--   0 runner    (1001) docker     (122)    11719 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/include/tiledbsoma/soma_array_reader.h
--rw-r--r--   0 runner    (1001) docker     (122)     2367 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/include/tiledbsoma/spdlog_with_R.h
--rw-r--r--   0 runner    (1001) docker     (122)     1765 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/include/tiledbsoma/stats.h
--rw-r--r--   0 runner    (1001) docker     (122)     1660 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/include/tiledbsoma/tiledbsoma
--rw-r--r--   0 runner    (1001) docker     (122)     2219 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/include/tiledbsoma/util.h
--rw-r--r--   0 runner    (1001) docker     (122)     1728 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/include/tiledbsoma/version.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:30:29.531375 tiledbsoma-1.2.1/dist_links/libtiledbsoma/src/
--rw-r--r--   0 runner    (1001) docker     (122)     9518 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4147 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/src/cli.cc
--rw-r--r--   0 runner    (1001) docker     (122)     7895 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/src/column_buffer.cc
--rw-r--r--   0 runner    (1001) docker     (122)     7087 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/src/logger.cc
--rw-r--r--   0 runner    (1001) docker     (122)     7934 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/src/logger.h
--rw-r--r--   0 runner    (1001) docker     (122)     7133 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/src/managed_query.cc
--rw-r--r--   0 runner    (1001) docker     (122)    13037 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/src/soma_array_reader.cc
--rw-r--r--   0 runner    (1001) docker     (122)     1689 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/src/stats.cc
--rw-r--r--   0 runner    (1001) docker     (122)     2329 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/src/util.cc
--rw-r--r--   0 runner    (1001) docker     (122)     1941 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/src/version.cc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:30:29.531375 tiledbsoma-1.2.1/dist_links/libtiledbsoma/test/
--rw-r--r--   0 runner    (1001) docker     (122)     2235 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)     6525 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/test/test_query_condition.py
--rw-r--r--   0 runner    (1001) docker     (122)     4038 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/test/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (122)     7879 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/test/test_soma_array_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)     3081 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/test/unit_column_buffer.cc
--rw-r--r--   0 runner    (1001) docker     (122)     5649 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/test/unit_managed_query.cc
--rw-r--r--   0 runner    (1001) docker     (122)     8829 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/test/unit_soma_array_reader.cc
--rw-r--r--   0 runner    (1001) docker     (122)    15705 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/libtiledbsoma/test/unit_thread_pool.cc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:30:29.531375 tiledbsoma-1.2.1/dist_links/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/scripts/README.md
--rwxr-xr-x   0 runner    (1001) docker     (122)     2811 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/scripts/bld
--rwxr-xr-x   0 runner    (1001) docker     (122)     1339 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/scripts/run-clang-format.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      821 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/scripts/show-versions.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3483 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/dist_links/scripts/update-tiledb-version.py
--rw-r--r--   0 runner    (1001) docker     (122)      498 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-28 13:30:29.535375 tiledbsoma-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     9712 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:30:29.519375 tiledbsoma-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:30:29.535375 tiledbsoma-1.2.1/src/tiledbsoma/
--rw-r--r--   0 runner    (1001) docker     (122)     5322 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/src/tiledbsoma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6363 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/src/tiledbsoma/_arrow_types.py
--rw-r--r--   0 runner    (1001) docker     (122)    26853 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/src/tiledbsoma/_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     7018 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/src/tiledbsoma/_common_nd_array.py
--rw-r--r--   0 runner    (1001) docker     (122)      345 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/src/tiledbsoma/_constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    33379 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/src/tiledbsoma/_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (122)     6797 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/src/tiledbsoma/_dense_nd_array.py
--rw-r--r--   0 runner    (1001) docker     (122)     1550 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/src/tiledbsoma/_exception.py
--rw-r--r--   0 runner    (1001) docker     (122)     1281 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/src/tiledbsoma/_experiment.py
--rw-r--r--   0 runner    (1001) docker     (122)     6712 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/src/tiledbsoma/_factory.py
--rw-r--r--   0 runner    (1001) docker     (122)     4436 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/src/tiledbsoma/_funcs.py
--rw-r--r--   0 runner    (1001) docker     (122)     1767 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/src/tiledbsoma/_general_utilities.py
--rw-r--r--   0 runner    (1001) docker     (122)     2550 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/src/tiledbsoma/_measurement.py
--rw-r--r--   0 runner    (1001) docker     (122)    16305 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/src/tiledbsoma/_query_condition.py
--rw-r--r--   0 runner    (1001) docker     (122)     2504 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/src/tiledbsoma/_read_iters.py
--rw-r--r--   0 runner    (1001) docker     (122)    11771 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/src/tiledbsoma/_sparse_nd_array.py
--rw-r--r--   0 runner    (1001) docker     (122)    12280 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/src/tiledbsoma/_tdb_handles.py
--rw-r--r--   0 runner    (1001) docker     (122)     6964 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/src/tiledbsoma/_tiledb_array.py
--rw-r--r--   0 runner    (1001) docker     (122)     9232 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/src/tiledbsoma/_tiledb_object.py
--rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/src/tiledbsoma/_types.py
--rw-r--r--   0 runner    (1001) docker     (122)     9107 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/src/tiledbsoma/_util.py
--rw-r--r--   0 runner    (1001) docker     (122)     3079 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/src/tiledbsoma/eta.py
--rw-r--r--   0 runner    (1001) docker     (122)     1492 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/src/tiledbsoma/experiment_query.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:30:29.535375 tiledbsoma-1.2.1/src/tiledbsoma/io/
--rw-r--r--   0 runner    (1001) docker     (122)      319 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/src/tiledbsoma/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3529 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/src/tiledbsoma/io/conversions.py
--rw-r--r--   0 runner    (1001) docker     (122)    48234 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/src/tiledbsoma/io/ingest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1995 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/src/tiledbsoma/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:30:29.535375 tiledbsoma-1.2.1/src/tiledbsoma/options/
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/src/tiledbsoma/options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3939 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/src/tiledbsoma/options/_soma_tiledb_context.py
--rw-r--r--   0 runner    (1001) docker     (122)     4892 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/src/tiledbsoma/options/_tiledb_create_options.py
--rw-r--r--   0 runner    (1001) docker     (122)    26675 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/src/tiledbsoma/pytiledbsoma.cc
--rw-r--r--   0 runner    (1001) docker     (122)     7781 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/src/tiledbsoma/query_condition.cc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 13:30:29.535375 tiledbsoma-1.2.1/src/tiledbsoma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5023 2023-03-28 13:30:29.000000 tiledbsoma-1.2.1/src/tiledbsoma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4264 2023-03-28 13:30:29.000000 tiledbsoma-1.2.1/src/tiledbsoma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-28 13:30:29.000000 tiledbsoma-1.2.1/src/tiledbsoma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-28 13:30:29.000000 tiledbsoma-1.2.1/src/tiledbsoma.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      182 2023-03-28 13:30:29.000000 tiledbsoma-1.2.1/src/tiledbsoma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-03-28 13:30:29.000000 tiledbsoma-1.2.1/src/tiledbsoma.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4659 2023-03-28 13:30:27.000000 tiledbsoma-1.2.1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.890294 tiledbsoma-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-04-26 00:03:40.000000 tiledbsoma-1.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-04-26 00:03:44.890294 tiledbsoma-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3123 2023-04-26 00:03:40.000000 tiledbsoma-1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-04-26 00:03:42.000000 tiledbsoma-1.2.2/RELEASE-VERSION
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.882294 tiledbsoma-1.2.2/dist_links/
+-rw-r--r--   0 runner    (1001) docker     (122)      508 2023-04-26 00:03:40.000000 tiledbsoma-1.2.2/dist_links/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.882294 tiledbsoma-1.2.2/dist_links/libtiledbsoma/
+-rw-r--r--   0 runner    (1001) docker     (122)     9437 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4058 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.882294 tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.882294 tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/Modules/
+-rw-r--r--   0 runner    (1001) docker     (122)     2893 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/Modules/CheckAVX2Support.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)      937 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/Modules/FindCatch_EP.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/Modules/FindClangTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     4894 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/Modules/FindSpdlog_EP.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     6323 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/Modules/FindTileDB_EP.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     3643 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/Modules/TileDBCommon.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     5203 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/Superbuild.cmake
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.882294 tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/inputs/
+-rw-r--r--   0 runner    (1001) docker     (122)      724 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/inputs/Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (122)      467 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/inputs/tiledbsoma.pc.in
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.882294 tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/patches/
+-rw-r--r--   0 runner    (1001) docker     (122)      736 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/patches/spdlog.patch
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.882294 tiledbsoma-1.2.2/dist_links/libtiledbsoma/doc/
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/doc/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)    36556 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/doc/reader.svg
+-rw-r--r--   0 runner    (1001) docker     (122)     2198 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/doc/reader.uml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.882294 tiledbsoma-1.2.2/dist_links/libtiledbsoma/external/
+-rw-r--r--   0 runner    (1001) docker     (122)     2774 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/external/.clang-format
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.878294 tiledbsoma-1.2.2/dist_links/libtiledbsoma/external/include/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.882294 tiledbsoma-1.2.2/dist_links/libtiledbsoma/external/include/span/
+-rw-r--r--   0 runner    (1001) docker     (122)    17276 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/external/include/span/span.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.882294 tiledbsoma-1.2.2/dist_links/libtiledbsoma/external/include/thread_pool/
+-rw-r--r--   0 runner    (1001) docker     (122)     7148 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/external/include/thread_pool/producer_consumer_queue.h
+-rw-r--r--   0 runner    (1001) docker     (122)    17772 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/external/include/thread_pool/status.h
+-rw-r--r--   0 runner    (1001) docker     (122)     5561 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/external/include/thread_pool/thread_pool.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.878294 tiledbsoma-1.2.2/dist_links/libtiledbsoma/external/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.882294 tiledbsoma-1.2.2/dist_links/libtiledbsoma/external/src/thread_pool/
+-rw-r--r--   0 runner    (1001) docker     (122)     3092 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/external/src/thread_pool/status.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     6700 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/external/src/thread_pool/thread_pool.cc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.878294 tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.882294 tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/
+-rw-r--r--   0 runner    (1001) docker     (122)     3767 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/array_buffers.h
+-rw-r--r--   0 runner    (1001) docker     (122)     7215 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/arrow_adapter.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/carrow.h
+-rw-r--r--   0 runner    (1001) docker     (122)     7819 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/column_buffer.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1885 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/common.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2959 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/logger_public.h
+-rw-r--r--   0 runner    (1001) docker     (122)    10187 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/managed_query.h
+-rw-r--r--   0 runner    (1001) docker     (122)    11753 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/soma_array_reader.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2367 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/spdlog_with_R.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1765 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/stats.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1660 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/tiledbsoma
+-rw-r--r--   0 runner    (1001) docker     (122)     2219 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/util.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1728 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/version.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.886294 tiledbsoma-1.2.2/dist_links/libtiledbsoma/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     9518 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4147 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/src/cli.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     7895 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/src/column_buffer.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     7087 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/src/logger.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     7934 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/src/logger.h
+-rw-r--r--   0 runner    (1001) docker     (122)     7133 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/src/managed_query.cc
+-rw-r--r--   0 runner    (1001) docker     (122)    13037 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/src/soma_array_reader.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     1689 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/src/stats.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     2329 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/src/util.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     1811 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/src/version.cc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.886294 tiledbsoma-1.2.2/dist_links/libtiledbsoma/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     2235 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     6525 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/test/test_query_condition.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4038 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/test/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7879 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/test/test_soma_array_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3081 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/test/unit_column_buffer.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     5649 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/test/unit_managed_query.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     8829 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/test/unit_soma_array_reader.cc
+-rw-r--r--   0 runner    (1001) docker     (122)    15705 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/libtiledbsoma/test/unit_thread_pool.cc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.886294 tiledbsoma-1.2.2/dist_links/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/scripts/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2811 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/scripts/bld
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1339 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/scripts/run-clang-format.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      821 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/scripts/show-versions.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3483 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/dist_links/scripts/update-tiledb-version.py
+-rw-r--r--   0 runner    (1001) docker     (122)      498 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-26 00:03:44.890294 tiledbsoma-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)    10989 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.878294 tiledbsoma-1.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.890294 tiledbsoma-1.2.2/src/tiledbsoma/
+-rw-r--r--   0 runner    (1001) docker     (122)     5322 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6363 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/_arrow_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26853 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6993 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/_common_nd_array.py
+-rw-r--r--   0 runner    (1001) docker     (122)      345 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33545 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6863 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/_dense_nd_array.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1550 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/_exception.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1660 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6712 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4436 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1767 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/_general_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2550 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16305 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/_query_condition.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2504 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/_read_iters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11747 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/_sparse_nd_array.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12161 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/_tdb_handles.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6964 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/_tiledb_array.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9229 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/_tiledb_object.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1499 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9107 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/_util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3079 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/eta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1492 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/experiment_query.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.890294 tiledbsoma-1.2.2/src/tiledbsoma/io/
+-rw-r--r--   0 runner    (1001) docker     (122)      319 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3529 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/io/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    53522 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/io/ingest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1995 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.890294 tiledbsoma-1.2.2/src/tiledbsoma/options/
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4049 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/options/_soma_tiledb_context.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5098 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/options/_tiledb_create_options.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26675 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/pytiledbsoma.cc
+-rw-r--r--   0 runner    (1001) docker     (122)     7781 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/src/tiledbsoma/query_condition.cc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:03:44.890294 tiledbsoma-1.2.2/src/tiledbsoma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5056 2023-04-26 00:03:44.000000 tiledbsoma-1.2.2/src/tiledbsoma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4264 2023-04-26 00:03:44.000000 tiledbsoma-1.2.2/src/tiledbsoma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 00:03:44.000000 tiledbsoma-1.2.2/src/tiledbsoma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 00:03:44.000000 tiledbsoma-1.2.2/src/tiledbsoma.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      323 2023-04-26 00:03:44.000000 tiledbsoma-1.2.2/src/tiledbsoma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-26 00:03:44.000000 tiledbsoma-1.2.2/src/tiledbsoma.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4659 2023-04-26 00:03:41.000000 tiledbsoma-1.2.2/version.py
```

### Comparing `tiledbsoma-1.2.1/PKG-INFO` & `tiledbsoma-1.2.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,31 @@
 Metadata-Version: 2.1
 Name: tiledbsoma
-Version: 1.2.1
+Version: 1.2.2
 Summary: Python API for efficient storage and retrieval of single-cell data using TileDB
 Home-page: https://github.com/single-cell-data/TileDB-SOMA/tree/main/apis/python
 Author: TileDB, Inc.
 Author-email: help@tiledb.io
 Maintainer: TileDB, Inc.
 Maintainer-email: help@tiledb.io
 License: MIT
 Description: # Overview
         
-        This is a Python implementation of the [Unified Single-cell Data Model](https://github.com/single-cell-data/SOMA).
-        
-        This branch, `main`, implements the [updated specfication](https://github.com/single-cell-data/SOMA/blob/main/abstract_specification.md).  Please also see the `main-old` branch which implements the [original specification](https://github.com/single-cell-data/TileDB-SOMA/blob/main-old/spec/specification.md).
+        This is a Python implementation of the [SOMA API specification](https://github.com/single-cell-data/SOMA/blob/main/abstract_specification.md) for interacting with the [Unified Single-cell Data Model](https://github.com/single-cell-data/SOMA).
         
         # Installation
         
         ## Using pip
         
-        This code is hosted at [PyPI](https://pypi.org/project/tiledbsoma/), so you can do
+        This code is hosted at [PyPI](https://pypi.org/project/tiledbsoma/), so you can install using `pip`:
         
         ```shell
         $ python -m pip install tiledbsoma
-        # or
-        $ python -m pip install --pre tiledbsoma
         ```
         
-        Without `--pre` you will get version 0.1.* (the `main-old` branch); with `--pre`, you will get 0.5.0a* (the `main` branch).
-        
         To install a specific version:
         
         ```shell
         $ python -m pip install git+https://github.com/single-cell-data/TileDB-SOMA.git@0.0.6#subdirectory=apis/python
         ```
         
         To update to the latest version:
@@ -43,14 +37,15 @@
         ## From source
         
         * This requires [`tiledb`](https://github.com/TileDB-Inc/TileDB-Py) (see [./setup.cfg](setup.cfg) for version), in addition to other dependencies in [setup.cfg](./setup.cfg).
         * Clone [this repo](https://github.com/single-cell-data/TileDB-SOMA)
         * `cd` into your checkout and then `cd apis/python`
         * `python -m pip install .`
         * Or, if you wish to modify the code and run it, `python -m pip install -v -e .`
+        * If the TileDB and TileDB-SOMA libraries are locally installed to a custom directory, such as `/usr/local`, set the path with environment variables `TILEDB_PATH` and `TILEDBSOMA_PATH`, `TILEDB_PATH=/usr/local python -m pip install -v -e .`
         * Optionally, if you prefer, you can run that inside `venv`:
           ```shell
           $ python -m venv venv
           $ . ./venv/bin/activate
           $ python -m pip install -v -e .
           ```
         * In either case:
@@ -60,15 +55,15 @@
         
         # Status
         
         Please see [https://github.com/single-cell-data/TileDB-SOMA/issues](https://github.com/single-cell-data/TileDB-SOMA/issues).
         
         # `platform_config` format
         
-        When accessing SOMA APIs, TileDB-specific settings can be configured with the `platform_config` parameter.
+        When accessing SOMA APIs, TileDB-specific settings can be configured with the [`platform_config`](https://github.com/single-cell-data/SOMA/blob/main/abstract_specification.md#platform-specific-configuration) parameter.
         The options accepted by TileDB SOMA are described here, using [TypeScript interface syntax](https://www.typescriptlang.org/docs/handbook/2/objects.html):
         
         ```typescript
         interface PlatformConfig {
           tiledb?: TDBConfig;
         }
         
@@ -112,14 +107,16 @@
         }
         ```
         
         # Information for developers
         
         Please see the [TileDB-SOMA wiki](https://github.com/single-cell-data/TileDB-SOMA/wiki).
         
+        <!-- temp for readthedocs testing -->
+        
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Operating System :: Unix
```

### Comparing `tiledbsoma-1.2.1/README.md` & `tiledbsoma-1.2.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 # Overview
 
-This is a Python implementation of the [Unified Single-cell Data Model](https://github.com/single-cell-data/SOMA).
-
-This branch, `main`, implements the [updated specfication](https://github.com/single-cell-data/SOMA/blob/main/abstract_specification.md).  Please also see the `main-old` branch which implements the [original specification](https://github.com/single-cell-data/TileDB-SOMA/blob/main-old/spec/specification.md).
+This is a Python implementation of the [SOMA API specification](https://github.com/single-cell-data/SOMA/blob/main/abstract_specification.md) for interacting with the [Unified Single-cell Data Model](https://github.com/single-cell-data/SOMA).
 
 # Installation
 
 ## Using pip
 
-This code is hosted at [PyPI](https://pypi.org/project/tiledbsoma/), so you can do
+This code is hosted at [PyPI](https://pypi.org/project/tiledbsoma/), so you can install using `pip`:
 
 ```shell
 $ python -m pip install tiledbsoma
-# or
-$ python -m pip install --pre tiledbsoma
 ```
 
-Without `--pre` you will get version 0.1.* (the `main-old` branch); with `--pre`, you will get 0.5.0a* (the `main` branch).
-
 To install a specific version:
 
 ```shell
 $ python -m pip install git+https://github.com/single-cell-data/TileDB-SOMA.git@0.0.6#subdirectory=apis/python
 ```
 
 To update to the latest version:
@@ -33,14 +27,15 @@
 ## From source
 
 * This requires [`tiledb`](https://github.com/TileDB-Inc/TileDB-Py) (see [./setup.cfg](setup.cfg) for version), in addition to other dependencies in [setup.cfg](./setup.cfg).
 * Clone [this repo](https://github.com/single-cell-data/TileDB-SOMA)
 * `cd` into your checkout and then `cd apis/python`
 * `python -m pip install .`
 * Or, if you wish to modify the code and run it, `python -m pip install -v -e .`
+* If the TileDB and TileDB-SOMA libraries are locally installed to a custom directory, such as `/usr/local`, set the path with environment variables `TILEDB_PATH` and `TILEDBSOMA_PATH`, `TILEDB_PATH=/usr/local python -m pip install -v -e .`
 * Optionally, if you prefer, you can run that inside `venv`:
   ```shell
   $ python -m venv venv
   $ . ./venv/bin/activate
   $ python -m pip install -v -e .
   ```
 * In either case:
@@ -50,15 +45,15 @@
 
 # Status
 
 Please see [https://github.com/single-cell-data/TileDB-SOMA/issues](https://github.com/single-cell-data/TileDB-SOMA/issues).
 
 # `platform_config` format
 
-When accessing SOMA APIs, TileDB-specific settings can be configured with the `platform_config` parameter.
+When accessing SOMA APIs, TileDB-specific settings can be configured with the [`platform_config`](https://github.com/single-cell-data/SOMA/blob/main/abstract_specification.md#platform-specific-configuration) parameter.
 The options accepted by TileDB SOMA are described here, using [TypeScript interface syntax](https://www.typescriptlang.org/docs/handbook/2/objects.html):
 
 ```typescript
 interface PlatformConfig {
   tiledb?: TDBConfig;
 }
 
@@ -101,7 +96,9 @@
   [kwarg: string]: any;
 }
 ```
 
 # Information for developers
 
 Please see the [TileDB-SOMA wiki](https://github.com/single-cell-data/TileDB-SOMA/wiki).
+
+<!-- temp for readthedocs testing -->
```

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/CMakeLists.txt` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,16 @@
 # TileDB BUILD Options
 # NOTE: TileDB Embedded version is controlled in cmake/Modules/FindTileDB_EP.cmake
 option(TILEDB_S3 "Enables S3/minio support using aws-cpp-sdk" ON)
 option(TILEDB_AZURE "Enables Azure Storage support using azure-storage-cpp" ON)
 option(TILEDB_GCS "Enables GCS Storage support using google-cloud-cpp" OFF)
 option(TILEDB_HDFS "Enables HDFS support using the official Hadoop JNI bindings" OFF)
 option(TILEDB_WERROR "Enables the -Werror flag during compilation." OFF)
-option(TILEDB_SERIALIZATION "If true, enables building with support for query serialization" OFF)
+option(TILEDB_SERIALIZATION "If true, enables building with support for query serialization" ON)
+option(TILEDB_VERBOSE "If true, sets default logging to verbose for TileDB" OFF)
 option(OVERRIDE_INSTALL_PREFIX "Ignores the setting of CMAKE_INSTALL_PREFIX and sets a default prefix" ON)
 option(ENABLE_ARROW_EXPORT "Installs an extra header for exporting in-memory results with Apache Arrow" ON)
 option(TILEDB_LOG_OUTPUT_ON_FAILURE "If true, print error logs if dependency sub-project build fails" ON)
 
 # NOTE: TILEDBSOMA_BUILD_R is added to INHERITED_CMAKE_ARGS in Superbuild.cmake
 # so the option is forwarded to the non-superbuild
 if(TILEDBSOMA_BUILD_R)
@@ -240,8 +241,8 @@
 # Regular build
 # ###########################################################
 add_subdirectory(src)
 
 if(TILEDBSOMA_ENABLE_TESTING)
   enable_testing()
   add_subdirectory(test)
-endif()
+endif()
```

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/README.md` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/README.md`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/cmake/Modules/CheckAVX2Support.cmake` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/Modules/CheckAVX2Support.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/cmake/Modules/FindClangTools.cmake` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/Modules/FindClangTools.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/cmake/Modules/FindSpdlog_EP.cmake` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/Modules/FindSpdlog_EP.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/cmake/Modules/FindTileDB_EP.cmake` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/Modules/FindTileDB_EP.cmake`

 * *Files 8% similar despite different names*

```diff
@@ -54,28 +54,28 @@
     # loaded by the Python and R tiledbsoma packages. Those packages -also- use TileDB-Py and
     # TileDB-R, each of which links their own 'copy' of TileDB Embedded, whose version we don't
     # control here. Ideally the TileDB Embedded versions should match! The show_package_versions()
     # helper function in each package can help to diagnose any mismatch.
     # NB When updating the pinned URLs here, please also update in file apis/r/tools/get_tarball.R
     if(DOWNLOAD_TILEDB_PREBUILT)
         if (WIN32) # Windows
-          SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.15.0/tiledb-windows-x86_64-2.15.0-1fb59c4.zip")
-          SET(DOWNLOAD_SHA1 "aeea7b08acffd2e907956ad31b3230f329c8e2f2")
+          SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.15.1/tiledb-windows-x86_64-2.15.1-432d4c2.zip")
+          SET(DOWNLOAD_SHA1 "7235a3bc0b5675ed83762a4290d99c6ff9db285f")
         elseif(APPLE) # OSX
 
           if (CMAKE_OSX_ARCHITECTURES STREQUAL x86_64 OR CMAKE_SYSTEM_PROCESSOR MATCHES "(x86_64)|(AMD64|amd64)|(^i.86$)")
-            SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.15.0/tiledb-macos-x86_64-2.15.0-1fb59c4.tar.gz")
-            SET(DOWNLOAD_SHA1 "e0a6cb63a87d07223ea1fe1e85add1157485039a")
+            SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.15.1/tiledb-macos-x86_64-2.15.1-432d4c2.tar.gz")
+            SET(DOWNLOAD_SHA1 "f5986f5a85912147e2b839e0968963df6c540688")
           elseif (CMAKE_OSX_ARCHITECTURES STREQUAL arm64 OR CMAKE_SYSTEM_PROCESSOR MATCHES "^aarch64" OR CMAKE_SYSTEM_PROCESSOR MATCHES "^arm")
-            SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.15.0/tiledb-macos-arm64-2.15.0-1fb59c4.tar.gz")
-            SET(DOWNLOAD_SHA1 "9cfdc7c783a0e9dc660d2da79c459c4792c42192")
+            SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.15.1/tiledb-macos-arm64-2.15.1-432d4c2.tar.gz")
+            SET(DOWNLOAD_SHA1 "6abb30f9dd7371d5a06a273008179bd57d691e36")
           endif()
         else() # Linux
-          SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.15.0/tiledb-linux-x86_64-2.15.0-1fb59c4.tar.gz")
-          SET(DOWNLOAD_SHA1 "d848984df361bf1dff1ace09cb7ac1c516c6cb87")
+          SET(DOWNLOAD_URL "https://github.com/TileDB-Inc/TileDB/releases/download/2.15.1/tiledb-linux-x86_64-2.15.1-432d4c2.tar.gz")
+          SET(DOWNLOAD_SHA1 "9b705af26007b193800f0382c343d421a8b59003")
         endif()
 
         ExternalProject_Add(ep_tiledb
                 PREFIX "externals"
                 URL ${DOWNLOAD_URL}
                 URL_HASH SHA1=${DOWNLOAD_SHA1}
                 CONFIGURE_COMMAND ""
@@ -89,25 +89,36 @@
                 LOG_CONFIGURE FALSE
                 LOG_BUILD FALSE
                 LOG_INSTALL FALSE
                 )
     else() # Build from source
         ExternalProject_Add(ep_tiledb
           PREFIX "externals"
-          URL "https://github.com/TileDB-Inc/TileDB/archive/2.15.0.zip"
-          URL_HASH SHA1=b281debe6799c635ab8c2984496ebe1f473a56d9
+          URL "https://github.com/TileDB-Inc/TileDB/archive/2.15.1.zip"
+          URL_HASH SHA1=8bb70f7534297b184d23b216b1097fdde40829df
           DOWNLOAD_NAME "tiledb.zip"
           CMAKE_ARGS
             -DCMAKE_INSTALL_PREFIX=${EP_INSTALL_PREFIX}
             -DCMAKE_PREFIX_PATH=${EP_INSTALL_PREFIX}
             -DTILEDB_S3=${TILEDB_S3}
-            -DTILEDB_VERBOSE=ON
-            -DTILEDB_SERIALIZATION=ON
+            -DTILEDB_AZURE=${TILEDB_AZURE}
+            -DTILEDB_GCS=${TILEDB_GCS}
+            -DTILEDB_HDFS=${TILEDB_HDFS}
+            -DTILEDB_SERIALIZATION=${TILEDB_SERIALIZATION}
+            -DTILEDB_WERROR=${TILEDB_WERROR}
+            -DTILEDB_VERBOSE=${TILEDB_VERBOSE}
             -DTILEDB_TESTS=OFF
             -DCMAKE_BUILD_TYPE=${CMAKE_BUILD_TYPE}
+            -DCMAKE_OSX_ARCHITECTURES=${CMAKE_OSX_ARCHITECTURES}
+            -DCMAKE_C_FLAGS=${CMAKE_C_FLAGS}
+            -DCMAKE_CXX_FLAGS=${CMAKE_CXX_FLAGS}
+            -DCMAKE_CXX_COMPILER=${CMAKE_CXX_COMPILER}
+            -DCMAKE_C_COMPILER=${CMAKE_C_COMPILER}
+            -DCMAKE_TOOLCHAIN_FILE=${CMAKE_TOOLCHAIN_FILE}
+            -DCMAKE_POSITION_INDEPENDENT_CODE=ON
           UPDATE_COMMAND ""
           INSTALL_COMMAND
             ${CMAKE_COMMAND} --build . --target install-tiledb
           LOG_DOWNLOAD TRUE
           LOG_CONFIGURE TRUE
           LOG_BUILD TRUE
           LOG_INSTALL TRUE
```

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/cmake/Modules/TileDBCommon.cmake` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/Modules/TileDBCommon.cmake`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/cmake/Superbuild.cmake` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/Superbuild.cmake`

 * *Files 8% similar despite different names*

```diff
@@ -45,30 +45,37 @@
 set(EXTERNAL_PROJECTS)
 
 # Forward any additional CMake args to the non-superbuild.
 set(INHERITED_CMAKE_ARGS
   -DCMAKE_INSTALL_PREFIX=${CMAKE_INSTALL_PREFIX}
   -DCMAKE_PREFIX_PATH=${CMAKE_PREFIX_PATH}
   -DCMAKE_BUILD_TYPE=${CMAKE_BUILD_TYPE}
+  -DCMAKE_C_FLAGS=${CMAKE_C_FLAGS}
+  -DCMAKE_CXX_FLAGS=${CMAKE_CXX_FLAGS}
+  -DCMAKE_CXX_STANDARD=${CMAKE_CXX_STANDARD}
+  -DCMAKE_CXX_COMPILER=${CMAKE_CXX_COMPILER}
+  -DCMAKE_C_COMPILER=${CMAKE_C_COMPILER}
   -DEP_BASE=${EP_BASE}
   -DFORCE_BUILD_TILEDB=${FORCE_BUILD_TILEDB}
   -DTILEDB_S3=${TILEDB_S3}
   -DTILEDB_AZURE=${TILEDB_AZURe}
   -DTILEDB_GCS=${TILEDB_GCS}
   -DTILEDB_HDFS=${TILEDB_HDFS}
   -DTILEDB_SERIALIZATION=${TILEDB_SERIALIZATION}
   -DTILEDB_WERROR=${TILEDB_WERROR}
+  -DTILEDB_VERBOSE=${TILEDB_VERBOSE}
   -DTileDB_DIR=${TileDB_DIR}
   -DSANITIZER=${SANITIZER}
   -DENABLE_ARROW_EXPORT=${ENABLE_ARROW_EXPORT}
   -DOVERRIDE_INSTALL_PREFIX=${OVERRIDE_INSTALL_PREFIX}
   -DTILEDBSOMA_BUILD_R=${TILEDBSOMA_BUILD_R}
   -DTILEDBSOMA_BUILD_STATIC=${TILEDBSOMA_BUILD_STATIC}
   -DTILEDBSOMA_BUILD_CLI=${TILEDBSOMA_BUILD_CLI}
   -DTILEDBSOMA_ENABLE_TESTING=${TILEDBSOMA_ENABLE_TESTING}
+  -DCMAKE_OSX_ARCHITECTURES=${CMAKE_OSX_ARCHITECTURES}
 )
 
 ############################################################
 # Set up external projects for dependencies
 ############################################################
 
 # These includes modify the EXTERNAL_PROJECTS variable.
```

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/cmake/inputs/Config.cmake.in` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/inputs/Config.cmake.in`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/cmake/patches/spdlog.patch` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/cmake/patches/spdlog.patch`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/doc/reader.svg` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/doc/reader.svg`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/doc/reader.uml` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/doc/reader.uml`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/external/.clang-format` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/external/.clang-format`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/external/include/span/span.hpp` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/external/include/span/span.hpp`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/external/include/thread_pool/producer_consumer_queue.h` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/external/include/thread_pool/producer_consumer_queue.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/external/include/thread_pool/status.h` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/external/include/thread_pool/status.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/external/include/thread_pool/thread_pool.h` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/external/include/thread_pool/thread_pool.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/external/src/thread_pool/status.cc` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/external/src/thread_pool/status.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/external/src/thread_pool/thread_pool.cc` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/external/src/thread_pool/thread_pool.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/include/tiledbsoma/array_buffers.h` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/array_buffers.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/include/tiledbsoma/arrow_adapter.h` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/arrow_adapter.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/include/tiledbsoma/carrow.h` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/carrow.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/include/tiledbsoma/column_buffer.h` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/column_buffer.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/include/tiledbsoma/common.h` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/common.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/include/tiledbsoma/logger_public.h` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/logger_public.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/include/tiledbsoma/managed_query.h` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/managed_query.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/include/tiledbsoma/soma_array_reader.h` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/soma_array_reader.h`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,16 @@
  * THE SOFTWARE.
  *
  * @section DESCRIPTION
  *
  *   This declares the SOMAArrayReader
  */
 
-#ifndef SOMA_READER
-#define SOMA_READER
+#ifndef SOMA_ARRAY_READER
+#define SOMA_ARRAY_READER
 
 #include <stdexcept>  // for windows: error C2039: 'runtime_error': is not a member of 'std'
 
 #include <future>
 
 #include <tiledb/tiledb>
 
@@ -370,8 +370,8 @@
 
     // Unoptimized method for computing nnz() (issue `count_cells` query)
     uint64_t nnz_slow();
 };
 
 }  // namespace tiledbsoma
 
-#endif
+#endif  // SOMA_ARRAY_READER
```

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/include/tiledbsoma/spdlog_with_R.h` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/spdlog_with_R.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/include/tiledbsoma/stats.h` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/stats.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/include/tiledbsoma/tiledbsoma` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/tiledbsoma`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/include/tiledbsoma/util.h` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/util.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/include/tiledbsoma/version.h` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/include/tiledbsoma/version.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/src/CMakeLists.txt` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/src/cli.cc` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/src/cli.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/src/column_buffer.cc` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/src/column_buffer.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/src/logger.cc` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/src/logger.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/src/logger.h` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/src/logger.h`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/src/managed_query.cc` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/src/managed_query.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/src/soma_array_reader.cc` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/src/soma_array_reader.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/src/stats.cc` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/src/stats.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/src/util.cc` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/src/util.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/src/version.cc` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/src/version.cc`

 * *Files 16% similar despite different names*

```diff
@@ -30,27 +30,20 @@
  * This exposes the version of the TileDB Embedded library in use.
  */
 
 #include "tiledbsoma/version.h"
 #include <tiledb/tiledb>
 #include "tiledbsoma/logger_public.h"
 
-#ifdef BUILD_COMMIT_HASH
-#define VERSION BUILD_COMMIT_HASH
-#else
-#define VERSION "dev"
-#endif
-
 namespace tiledbsoma::version {
 
 std::string as_string() {
     int major, minor, patch;
     tiledb_version(&major, &minor, &patch);
-    return fmt::format(
-        "libtiledbsoma={};libtiledb={}.{}.{}", VERSION, major, minor, patch);
+    return fmt::format("libtiledb={}.{}.{}", major, minor, patch);
 }
 
 std::tuple<int, int, int> embedded_version_triple() {
     int major, minor, patch;
     tiledb_version(&major, &minor, &patch);
     return std::make_tuple(major, minor, patch);
 }
```

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/test/CMakeLists.txt` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/test/test_query_condition.py` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/test/test_query_condition.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/test/test_simple.py` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/test/test_simple.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/test/test_soma_array_reader.py` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/test/test_soma_array_reader.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/test/unit_column_buffer.cc` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/test/unit_column_buffer.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/test/unit_managed_query.cc` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/test/unit_managed_query.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/test/unit_soma_array_reader.cc` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/test/unit_soma_array_reader.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/libtiledbsoma/test/unit_thread_pool.cc` & `tiledbsoma-1.2.2/dist_links/libtiledbsoma/test/unit_thread_pool.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/scripts/bld` & `tiledbsoma-1.2.2/dist_links/scripts/bld`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/scripts/run-clang-format.sh` & `tiledbsoma-1.2.2/dist_links/scripts/run-clang-format.sh`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/scripts/show-versions.py` & `tiledbsoma-1.2.2/dist_links/scripts/show-versions.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/dist_links/scripts/update-tiledb-version.py` & `tiledbsoma-1.2.2/dist_links/scripts/update-tiledb-version.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/setup.py` & `tiledbsoma-1.2.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -36,32 +36,44 @@
     from setuptools import Extension as Pybind11Extension
 
 this_dir = pathlib.Path(__file__).parent.absolute()
 sys.path.insert(0, str(this_dir))
 
 import version  # noqa E402
 
+# tiledb_dir and libtiledbsoma_dir may be specified by either environment variable
+# or command-line argument. If both are provided, the latter wins.
+
+tiledb_dir: Optional[pathlib.Path] = None
 libtiledbsoma_dir: Optional[pathlib.Path] = None
 
+tiledb_dir = pathlib.Path(os.environ.get("TILEDB_PATH", this_dir))
+libtiledbsoma_dir = os.environ.get("TILEDBSOMA_PATH", None)
+
 args = sys.argv[:]
 for arg in args:
     start, eq, last = arg.partition("=")
+    if (start, eq) == ("--tiledb", "="):
+        tiledb_dir = pathlib.Path(last)
+        sys.argv.remove(arg)
     if (start, eq) == ("--libtiledbsoma", "="):
         libtiledbsoma_dir = pathlib.Path(last)
         sys.argv.remove(arg)
 
 if libtiledbsoma_dir is None:
     scripts_dir = this_dir / "dist_links" / "scripts"
 
     if scripts_dir.is_symlink():
         # in git source tree
         libtiledbsoma_dir = this_dir.parent.parent / "dist"
     else:
         # in extracted sdist, with libtiledbsoma copied into dist_links/
         libtiledbsoma_dir = this_dir / "dist_links" / "dist"
+else:
+    libtiledbsoma_dir = pathlib.Path(libtiledbsoma_dir)
 
 
 def get_libtiledbsoma_library_name():
     """
     :return: List of TileDB shared library names.
     """
     if os.name == "posix":
@@ -175,32 +187,39 @@
     "dist_links/libtiledbsoma/external/include",
     "../../build/externals/install/include",
     str(libtiledbsoma_dir / "include"),
     str(
         "./src/tiledbsoma"
     ),  # since pytiledbsoma.cc does #include of query_condition.cc
     str(libtiledbsoma_dir.parent / "build/externals/install/include"),
+    str(tiledb_dir / "include"),
 ]
 
 LIB_DIRS = [
     str(libtiledbsoma_dir / "lib"),
+    str(tiledb_dir / "lib"),
 ]
 CXX_FLAGS = [
     f'-Wl,-rpath,{str(libtiledbsoma_dir / "lib")}',
+    f'-Wl,-rpath,{str(tiledb_dir / "lib")}',
 ]
 if sys.platform == "darwin":
     CXX_FLAGS.append("-mmacosx-version-min=10.14")
 
 if os.name == "posix" and sys.platform != "darwin":
     LIB_DIRS.append(str(libtiledbsoma_dir / "lib" / "x86_64-linux-gnu"))
     LIB_DIRS.append(str(libtiledbsoma_dir / "lib64"))
+    LIB_DIRS.append(str(tiledb_dir / "lib" / "x86_64-linux-gnu"))
+    LIB_DIRS.append(str(tiledb_dir / "lib64"))
     CXX_FLAGS.append(
         f'-Wl,-rpath,{str(libtiledbsoma_dir / "lib" / "x86_64-linux-gnu")}'
     )
     CXX_FLAGS.append(f'-Wl,-rpath,{str(libtiledbsoma_dir / "lib64")}')
+    CXX_FLAGS.append(f'-Wl,-rpath,{str(tiledb_dir / "lib" / "x86_64-linux-gnu")}')
+    CXX_FLAGS.append(f'-Wl,-rpath,{str(tiledb_dir / "lib64")}')
 
 # ----------------------------------------------------------------
 # Don't use `if __name__ == "__main__":` as the `python_requires` must
 # be at top level, outside any if-block
 # https://github.com/pypa/cibuildwheel/blob/7c4bbf8cb31d856a0fe547faf8edf165cd48ce74/cibuildwheel/projectfiles.py#L41-L46
 
 setuptools.setup(
@@ -243,24 +262,31 @@
             extra_compile_args=["-std=c++17"] + CXX_FLAGS,
             language="c++",
         )
     ],
     zip_safe=False,
     setup_requires=["pybind11"],
     install_requires=[
-        "anndata",
+        # Needed for Python 3.7 which anndata 0.9 doesn't support but we do
+        "anndata < 0.9; python_version<'3.8'",
+        "anndata; python_version>='3.8'",
         "attrs>=22.2",
         # Pinning numba & its particular numpy constraints:
         # The old pip solver (<=2020) doesn't deal with the transitive
         # requirements (scanpy -> numba -> numpy) properly resulting in broken
         # installation of incompatible numpy>=1.24. Issue #1051
         # These pins can be removed either when there's a new numba release
         # with less-particular numpy version constraints, or if we decide we no
         # longer need to support the old pip solver (default on ubuntu 20.04).
-        "numba==0.56.4",
+        #
+        # Also: numba doesn't support Python 3.11 until 0.57.0rc1.
+        # It' not preferable to pin to an RC dependency, so we only do this
+        # when we must, which is for 3.11.
+        "numba==0.56.4; python_version<'3.11'",
+        "numba==0.57.0rc1; python_version=='3.11'",
         "numpy>=1.18,<1.24",
         "pandas",
         "pyarrow>=9.0.0",
         "scanpy>=1.9.2",
         "scipy",
         "somacore==1.0.1",
         "tiledb==0.21.*",
```

### Comparing `tiledbsoma-1.2.1/src/tiledbsoma/__init__.py` & `tiledbsoma-1.2.2/src/tiledbsoma/__init__.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/src/tiledbsoma/_arrow_types.py` & `tiledbsoma-1.2.2/src/tiledbsoma/_arrow_types.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/src/tiledbsoma/_collection.py` & `tiledbsoma-1.2.2/src/tiledbsoma/_collection.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/src/tiledbsoma/_common_nd_array.py` & `tiledbsoma-1.2.2/src/tiledbsoma/_common_nd_array.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,18 +173,18 @@
 
         # TODO: accept more TileDB array-schema options from create_options
         # https://github.com/single-cell-data/TileDB-SOMA/issues/876
         return tiledb.ArraySchema(
             domain=dom,
             attrs=attrs,
             sparse=is_sparse,
-            allows_duplicates=create_options.get("allows_duplicates", False),
+            allows_duplicates=create_options.allows_duplicates(),
             offsets_filters=create_options.offsets_filters(),
             validity_filters=create_options.validity_filters(),
-            capacity=create_options.get("capacity", 100000),
+            capacity=create_options.capacity(),
             tile_order=tile_order,
             cell_order=cell_order,
             ctx=context.tiledb_ctx,
         )
 
     @classmethod
     def _dim_capacity_and_extent(
```

### Comparing `tiledbsoma-1.2.1/src/tiledbsoma/_dataframe.py` & `tiledbsoma-1.2.2/src/tiledbsoma/_dataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,15 +149,15 @@
             domain:
                 An optional sequence of tuples specifying the domain of each
                 index column. Each tuple should be a pair consisting of the minimum and
                 maximum values storable in the index column. For example, if there is a
                 single int64-valued index column, then ``domain`` might be ``[(100,
                 200)]`` to indicate that values between 100 and 200, inclusive, can be
                 stored in that column.  If provided, this sequence must have the same
-                length as `index_column_names`, and the index-column domain will be as
+                length as ``index_column_names``, and the index-column domain will be as
                 specified.  If omitted entirely, or if ``None`` in a given dimension,
                 the corresponding index-column domain will use the minimum and maximum
                 possible values for the column's datatype.  This makes a
                 :class:`DataFrame` growable.
             platform_config:
                 Platform-specific options used to create this
                 DataFrame, provided via ``{"tiledb": {"create": ...}}`` nested keys.
@@ -246,24 +246,24 @@
         Lifecycle:
             Experimental.
         """
         return self._tiledb_domain()
 
     @property
     def count(self) -> int:
-        """Returns the number of rows in the dataframe. Same as `len(df)`.
+        """Returns the number of rows in the dataframe. Same as ``len(df)``.
 
         Lifecycle:
             Experimental.
         """
         self._check_open_read()
         return cast(int, self._soma_reader().nnz())
 
     def __len__(self) -> int:
-        """Returns the number of rows in the dataframe. Same as `df.count`."""
+        """Returns the number of rows in the dataframe. Same as ``df.count``."""
         return self.count
 
     def read(
         self,
         coords: options.SparseDFCoords = (),
         column_names: Optional[Sequence[str]] = None,
         *,
@@ -311,19 +311,19 @@
             Acceptable ways to index:
 
             * A sequence of coordinates is accepted, one per dimension.
             * Sequence length must be <= number of dimensions.
             * If the sequence contains missing coordinates (length less than number of dimensions),
               then ``slice(None)`` -- i.e. no constraint -- is assumed for the missing dimensions.
             * Per-dimension, explicitly specified coordinates can be one of: None, a value, a
-              list/ndarray/paarray/etc of values, a slice, etc.
+              list/``numpy.ndarray``/``pyarrow.Array``/etc of values, a slice, etc.
             * Slices are doubly inclusive: ``slice(2,4)`` means [2,3,4] not [2,3].
               Slice steps are not supported.
-              Slices can be ``slice(None)``, meaning select all in that dimension, but may not be half-specified:
-              ``slice(2,None)`` and ``slice(None,4)`` are both unsupported.
+              Slices can be ``slice(None)``, meaning select all in that dimension, and may be half-specified,
+              e.g.  ``slice(2,None)`` or ``slice(None,4)``.
             * Negative indexing is unsupported.
 
         Lifecycle:
             Experimental.
         """
         del batch_size, platform_config  # Currently unused.
         _util.check_unpartitioned(partitions)
@@ -355,17 +355,17 @@
         """Writes an `Arrow table <https://arrow.apache.org/docs/python/generated/pyarrow.Table.html>`_
         to the persistent object. As duplicate index values are not allowed, index values already
         present in the object are overwritten
         and new index values are added.
 
         Args:
             values:
-                An Arrow table containing all columns, including
-                the index columns. The schema for the values must match
-                the schema for the :class:`DataFrame`.
+                An `Arrow table <https://arrow.apache.org/docs/python/generated/pyarrow.Table.html>`_
+                containing all columns, including the index columns. The schema for the values must
+                match the schema for the :class:`DataFrame`.
 
         Raises:
             TypeError:
                 If the ``values`` parameter is an unsupported type.
             ValueError:
                 If the ``values`` parameter is an empty table.
             SOMAError:
@@ -707,37 +707,39 @@
             ),
         )
         dims.append(dim)
 
     dom = tiledb.Domain(dims, ctx=context.tiledb_ctx)
 
     attrs = []
+    metadata = schema.metadata or {}
     for attr_name in schema.names:
         if attr_name in index_column_names:
             continue
         attr = tiledb.Attr(
             name=attr_name,
             dtype=_arrow_types.tiledb_type_from_arrow_type(
                 schema.field(attr_name).type
             ),
+            nullable=metadata.get(attr_name.encode("utf-8")) == b"nullable",
             filters=tiledb_create_options.attr_filters(attr_name, ["ZstdFilter"]),
             ctx=context.tiledb_ctx,
         )
         attrs.append(attr)
 
     cell_order, tile_order = tiledb_create_options.cell_tile_orders()
 
     return tiledb.ArraySchema(
         domain=dom,
         attrs=attrs,
         sparse=True,
-        allows_duplicates=tiledb_create_options.get("allows_duplicates", False),
+        allows_duplicates=tiledb_create_options.allows_duplicates(),
         offsets_filters=tiledb_create_options.offsets_filters(),
         validity_filters=tiledb_create_options.validity_filters(),
-        capacity=tiledb_create_options.get("capacity", 100000),
+        capacity=tiledb_create_options.capacity(),
         cell_order=cell_order,
         # As of TileDB core 2.8.2, we cannot consolidate string-indexed sparse arrays with
         # col-major tile order: so we write ``X`` with row-major tile order.
         tile_order=tile_order,
         ctx=context.tiledb_ctx,
     )
```

### Comparing `tiledbsoma-1.2.1/src/tiledbsoma/_dense_nd_array.py` & `tiledbsoma-1.2.2/src/tiledbsoma/_dense_nd_array.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,16 +22,17 @@
 
 
 class DenseNDArray(NDArray, somacore.DenseNDArray):
     """:class:`DenseNDArray` is a dense, N-dimensional array, with offset (zero-based)
     integer indexing on each dimension. :class:`DenseNDArray` has a user-defined
     schema, which includes:
 
-    * The element type, expressed as an Arrow type, indicating the type of data
-      contained within the array.
+    * The element type, expressed as an
+      `Arrow type <https://arrow.apache.org/docs/python/api/datatypes.html>`_
+      indicating the type of data contained within the array.
     * The shape of the array, i.e., the number of dimensions and the length of
       each dimension.
 
     All dimensions must have a positive, non-zero length, and there must be 1
     or more dimensions.
 
     Where explicitly referenced in the API, the dimensions are named
```

### Comparing `tiledbsoma-1.2.1/src/tiledbsoma/_exception.py` & `tiledbsoma-1.2.2/src/tiledbsoma/_exception.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/src/tiledbsoma/_experiment.py` & `tiledbsoma-1.2.2/src/tiledbsoma/_experiment.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,19 +2,22 @@
 # Copyright (c) 2021-2023 TileDB, Inc.
 #
 # Licensed under the MIT License.
 
 """Implementation of a SOMA Experiment.
 """
 
+from typing import Any
+
 from somacore import experiment
 
 from ._collection import Collection, CollectionBase
 from ._dataframe import DataFrame
 from ._measurement import Measurement
+from ._tdb_handles import Wrapper
 from ._tiledb_object import AnyTileDBObject
 
 
 class Experiment(
     CollectionBase[AnyTileDBObject],
     experiment.Experiment[  # type: ignore[type-var]
         DataFrame,
@@ -40,7 +43,14 @@
 
     __slots__ = ()
 
     _subclass_constrained_soma_types = {
         "obs": ("SOMADataFrame",),
         "ms": ("SOMACollection",),
     }
+
+    @classmethod
+    def _set_create_metadata(cls, handle: Wrapper[Any]) -> None:
+        # Root SOMA objects include a `dataset_type` entry to allow the
+        # TileDB Cloud UI to detect that they are SOMA datasets.
+        handle.metadata["dataset_type"] = "soma"
+        return super()._set_create_metadata(handle)
```

### Comparing `tiledbsoma-1.2.1/src/tiledbsoma/_factory.py` & `tiledbsoma-1.2.2/src/tiledbsoma/_factory.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/src/tiledbsoma/_funcs.py` & `tiledbsoma-1.2.2/src/tiledbsoma/_funcs.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/src/tiledbsoma/_general_utilities.py` & `tiledbsoma-1.2.2/src/tiledbsoma/_general_utilities.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/src/tiledbsoma/_measurement.py` & `tiledbsoma-1.2.2/src/tiledbsoma/_measurement.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/src/tiledbsoma/_query_condition.py` & `tiledbsoma-1.2.2/src/tiledbsoma/_query_condition.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/src/tiledbsoma/_read_iters.py` & `tiledbsoma-1.2.2/src/tiledbsoma/_read_iters.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/src/tiledbsoma/_sparse_nd_array.py` & `tiledbsoma-1.2.2/src/tiledbsoma/_sparse_nd_array.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,24 +101,24 @@
         coords: options.SparseNDCoords = (),
         *,
         result_order: options.ResultOrderStr = options.ResultOrder.AUTO,
         batch_size: options.BatchSize = _UNBATCHED,
         partitions: Optional[options.ReadPartitions] = None,
         platform_config: Optional[PlatformConfig] = None,
     ) -> "SparseNDArrayRead":
-        """Reads a user-defined slice of the SparseNDArray.
+        """Reads a user-defined slice of the :class:`SparseNDArray`.
 
         Args:
             coords:
                 A per-dimension tuple of scalar, slice, sequence of scalar or
                 `Arrow IntegerArray <https://arrow.apache.org/docs/python/generated/pyarrow.IntegerArray.html>`_
-                defining the region to read.  (Arrow arrays currently unimplemented.)
+                defining the region to read.
 
         Returns:
-            A SparseNDArrayRead to access result iterators in various formats.
+            A :class:`SparseNDArrayRead` to access result iterators in various formats.
 
         Raises:
             SOMAError:
                 If the object is not open for reading.
 
         Lifecycle:
             Experimental.
@@ -128,19 +128,19 @@
 
             * A sequence of coordinates is accepted, one per dimension.
             * Sequence length must be <= number of dimensions.
             * If the sequence contains missing coordinates (length < number of dimensions),
               then ``slice(None)`` -- i.e. no constraint -- is assumed for the
               remaining dimensions.
             * Per-dimension, explicitly specified coordinates can be one of:
-              None, a value, a list/ndarray/paarray/etc of values, a slice, etc.
+              None, a value, a list/``numpy.ndarray``/``pyarrow.Array``/etc of values, a slice, etc.
             * Slices are doubly inclusive: ``slice(2,4)`` means [2,3,4] not [2,3].
               Slice steps can only be +1. Slices can be ``slice(None)``, meaning
-              select all in that dimension, but may not be half-specified:
-              ``slice(2,None)`` and ``slice(None,4)`` are both unsupported.
+              select all in that dimension, and may be half-specified, e.g.
+              ``slice(2,None)`` or ``slice(None,4)``.
             * Negative indexing is unsupported.
         """
         del batch_size, platform_config  # Currently unused.
         self._check_open_read()
         _util.check_unpartitioned(partitions)
 
         schema = self._handle.schema
```

### Comparing `tiledbsoma-1.2.1/src/tiledbsoma/_tdb_handles.py` & `tiledbsoma-1.2.2/src/tiledbsoma/_tdb_handles.py`

 * *Files 3% similar despite different names*

```diff
@@ -216,32 +216,27 @@
     def _opener(
         cls,
         uri: str,
         mode: options.OpenMode,
         context: SOMATileDBContext,
         timestamp: int,
     ) -> tiledb.Group:
-        return tiledb.Group(
-            uri, mode, ctx=_group_timestamp_ctx(context.tiledb_ctx, timestamp)
-        )
+        # We want to do open-group-at-timestamp.
+        ctx = context.tiledb_ctx
+        cfgdict = context.tiledb_ctx.config().dict()
+        cfgdict["sm.group.timestamp_end"] = timestamp
+        return tiledb.Group(uri, mode, ctx=ctx, config=tiledb.Config(cfgdict))
 
     def _do_initial_reads(self, reader: tiledb.Group) -> None:
         super()._do_initial_reads(reader)
         self.initial_contents = {
             o.name: GroupEntry.from_object(o) for o in reader if o.name is not None
         }
 
 
-def _group_timestamp_ctx(ctx: tiledb.Ctx, timestamp: int) -> tiledb.Ctx:
-    """Builds a TileDB context to open groups at the given timestamp."""
-    group_cfg = ctx.config().dict()
-    group_cfg["sm.group.timestamp_end"] = timestamp
-    return tiledb.Ctx(group_cfg)
-
-
 class _DictMod(enum.Enum):
     """State machine to keep track of modifications to a dictionary.
 
     This whole thing is a hack to allow users to treat the metadata dict
     like an actual dictionary because tiledb currently does not support multiple
     modifications to the same key (e.g., add-then-delete a metadata entry has
     undesired results) [sc-25089].
```

### Comparing `tiledbsoma-1.2.1/src/tiledbsoma/_tiledb_array.py` & `tiledbsoma-1.2.2/src/tiledbsoma/_tiledb_array.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/src/tiledbsoma/_tiledb_object.py` & `tiledbsoma-1.2.2/src/tiledbsoma/_tiledb_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,15 +261,15 @@
                 return md_type.lower() == cls.soma_type.lower()
         except (SOMAError, tiledb.cc.TileDBError):
             return False
 
     @classmethod
     def _set_create_metadata(cls, handle: _tdb_handles.AnyWrapper) -> None:
         """Sets the necessary metadata on a newly-created TileDB object."""
-        handle.writer.meta.update(
+        handle.metadata.update(
             {
                 _constants.SOMA_OBJECT_TYPE_METADATA_KEY: cls.soma_type,
                 _constants.SOMA_ENCODING_VERSION_METADATA_KEY: _constants.SOMA_ENCODING_VERSION,
             }
         )
         # Semi-hack: flush the metadata immediately upon creation so that the
         # backing storage isn't half-created (i.e., there is a tiledb object
```

### Comparing `tiledbsoma-1.2.1/src/tiledbsoma/_types.py` & `tiledbsoma-1.2.2/src/tiledbsoma/_types.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/src/tiledbsoma/_util.py` & `tiledbsoma-1.2.2/src/tiledbsoma/_util.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/src/tiledbsoma/eta.py` & `tiledbsoma-1.2.2/src/tiledbsoma/eta.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/src/tiledbsoma/experiment_query.py` & `tiledbsoma-1.2.2/src/tiledbsoma/experiment_query.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/src/tiledbsoma/io/conversions.py` & `tiledbsoma-1.2.2/src/tiledbsoma/io/conversions.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/src/tiledbsoma/io/ingest.py` & `tiledbsoma-1.2.2/src/tiledbsoma/io/ingest.py`

 * *Files 11% similar despite different names*

```diff
@@ -91,16 +91,15 @@
         experiment_uri: The experiment to create or update.
 
         input_path: A path to an input H5AD file.
 
         measurement_name: The name of the measurement to store data in.
 
         ingest_mode: The ingestion type to perform:
-            - ``write``: Writes all data, creating new layers
-              if the SOMA already exists.
+            - ``write``: Writes all data, creating new layers if the SOMA already exists.
             - ``resume``: Adds data to an existing SOMA, skipping writing data
               that was previously written. Useful for continuing after a partial
               or interrupted ingestion operation.
             - ``schema_only``: Creates groups and the array schema, without
               writing any data to the array. Useful to prepare for appending
               multiple H5AD files to a single SOMA.
 
@@ -155,15 +154,15 @@
     *,
     context: Optional[SOMATileDBContext] = None,
     platform_config: Optional[PlatformConfig] = None,
     ingest_mode: IngestMode = "write",
     use_relative_uri: Optional[bool] = None,
     X_kind: Union[Type[SparseNDArray], Type[DenseNDArray]] = SparseNDArray,
 ) -> str:
-    """Writes an anndata object to a :class:`Experiment`.
+    """Writes an `AnnData <https://anndata.readthedocs.io/>`_ object to an :class:`Experiment`.
 
     Measurement data is stored in a :class:`Measurement` in the experiment's
     ``ms`` field, with the key provided by ``measurement_name``. Data elements
     are available at the standard fields (``var``, ``X``, etc.). Unstructured
     data from ``uns`` is partially supported (structured arrays and non-numeric
     NDArrays are skipped), and is available at the measurement's ``uns`` key
     (i.e., at ``your_experiment.ms[measurement_name]["uns"]``).
@@ -172,16 +171,15 @@
         experiment_uri: The experiment to create or update.
 
         input_path: A path to an input H5AD file.
 
         measurement_name: The name of the measurement to store data in.
 
         ingest_mode: The ingestion type to perform:
-            - ``write``: Writes all data, creating new layers
-              if the SOMA already exists.
+            - ``write``: Writes all data, creating new layers if the SOMA already exists.
             - ``resume``: Adds data to an existing SOMA, skipping writing data
               that was previously written. Useful for continuing after a partial
               or interrupted ingestion operation.
             - ``schema_only``: Creates groups and the array schema, without
               writing any data to the array. Useful to prepare for appending
               multiple H5AD files to a single SOMA.
 
@@ -216,70 +214,84 @@
 
     logging.log_io(None, _util.format_elapsed(s, "FINISH DECATEGORICALIZING"))
 
     s = _util.get_start_stamp()
     logging.log_io(None, f"START  WRITING {experiment_uri}")
 
     # Must be done first, to create the parent directory.
-    experiment = _create_or_open_coll(Experiment, experiment_uri, ingest_mode)
+    experiment = _create_or_open_coll(
+        Experiment, experiment_uri, ingest_mode, context=context
+    )
 
     # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
     # OBS
     df_uri = _util.uri_joinpath(experiment.uri, "obs")
     with _write_dataframe(
         df_uri,
         conversions.decategoricalize_obs_or_var(anndata.obs),
         id_column_name="obs_id",
         platform_config=platform_config,
+        context=context,
         ingest_mode=ingest_mode,
     ) as obs:
         _maybe_set(experiment, "obs", obs, use_relative_uri=use_relative_uri)
 
     # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
     # MS
     with _create_or_open_coll(
-        Collection[Measurement], _util.uri_joinpath(experiment.uri, "ms"), ingest_mode
+        Collection[Measurement],
+        _util.uri_joinpath(experiment.uri, "ms"),
+        ingest_mode,
+        context=context,
     ) as ms:
         _maybe_set(experiment, "ms", ms, use_relative_uri=use_relative_uri)
 
         # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
         # MS/meas
         with _create_or_open_coll(
-            Measurement, f"{experiment.ms.uri}/{measurement_name}", ingest_mode
+            Measurement,
+            f"{experiment.ms.uri}/{measurement_name}",
+            ingest_mode,
+            context=context,
         ) as measurement:
             _maybe_set(
                 ms, measurement_name, measurement, use_relative_uri=use_relative_uri
             )
 
             # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
             # ms/meas/uns
             _maybe_ingest_uns(
                 measurement,
                 anndata.uns,
                 platform_config,
+                context,
                 ingest_mode,
                 use_relative_uri=use_relative_uri,
             )
 
             # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
             # MS/meas/VAR
             with _write_dataframe(
                 _util.uri_joinpath(measurement.uri, "var"),
                 conversions.decategoricalize_obs_or_var(anndata.var),
                 id_column_name="var_id",
                 platform_config=platform_config,
+                context=context,
                 ingest_mode=ingest_mode,
             ) as var:
                 _maybe_set(measurement, "var", var, use_relative_uri=use_relative_uri)
 
             # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
             # MS/meas/X/DATA
 
             with _create_or_open_coll(
-                Collection, _util.uri_joinpath(measurement.uri, "X"), ingest_mode
+                Collection,
+                _util.uri_joinpath(measurement.uri, "X"),
+                ingest_mode,
+                context=context,
             ) as x:
                 _maybe_set(measurement, "X", x, use_relative_uri=use_relative_uri)
 
                 # Since we did ``anndata = ad.read_h5ad(path_to_h5ad, "r")`` with the "r":
                 # * If we do ``anndata.X[:]`` we're loading all of a CSR/CSC/etc into memory.
                 # * If we do ``anndata.X`` we're getting a pageable object which can be loaded
                 #   chunkwise into memory.
@@ -287,114 +299,129 @@
 
                 with create_from_matrix(
                     X_kind,
                     _util.uri_joinpath(measurement.X.uri, "data"),
                     anndata.X,
                     platform_config,
                     ingest_mode,
+                    context,
                 ) as data:
                     _maybe_set(x, "data", data, use_relative_uri=use_relative_uri)
 
                 # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
                 # MS/meas/OBSM,VARM,OBSP,VARP
                 if len(anndata.obsm.keys()) > 0:  # do not create an empty collection
                     with _create_or_open_coll(
                         Collection,
                         _util.uri_joinpath(measurement.uri, "obsm"),
                         ingest_mode,
+                        context=context,
                     ) as obsm:
                         _maybe_set(
                             measurement, "obsm", obsm, use_relative_uri=use_relative_uri
                         )
                         for key in anndata.obsm.keys():
                             with create_from_matrix(
-                                DenseNDArray,
+                                # TODO (https://github.com/single-cell-data/TileDB-SOMA/issues/1245):
+                                # consider a use-dense flag at the tiledbsoma.io API
+                                # DenseNDArray,
+                                SparseNDArray,
                                 _util.uri_joinpath(measurement.obsm.uri, key),
                                 conversions.to_tiledb_supported_array_type(
                                     anndata.obsm[key]
                                 ),
                                 platform_config,
                                 ingest_mode,
+                                context=context,
                             ) as arr:
                                 _maybe_set(
                                     obsm, key, arr, use_relative_uri=use_relative_uri
                                 )
                             arr.close()
                     measurement.obsm.close()
 
                 if len(anndata.varm.keys()) > 0:  # do not create an empty collection
                     with _create_or_open_coll(
                         Collection,
                         _util.uri_joinpath(measurement.uri, "varm"),
                         ingest_mode,
+                        context=context,
                     ) as varm:
                         _maybe_set(
                             measurement, "varm", varm, use_relative_uri=use_relative_uri
                         )
                         for key in anndata.varm.keys():
                             with create_from_matrix(
-                                DenseNDArray,
+                                # TODO (https://github.com/single-cell-data/TileDB-SOMA/issues/1245):
+                                # consider a use-dense flag at the tiledbsoma.io API
+                                # DenseNDArray,
+                                SparseNDArray,
                                 _util.uri_joinpath(measurement.varm.uri, key),
                                 conversions.to_tiledb_supported_array_type(
                                     anndata.varm[key]
                                 ),
                                 platform_config,
                                 ingest_mode,
+                                context=context,
                             ) as darr:
                                 _maybe_set(
                                     varm,
                                     key,
                                     darr,
                                     use_relative_uri=use_relative_uri,
                                 )
 
                 if len(anndata.obsp.keys()) > 0:  # do not create an empty collection
                     with _create_or_open_coll(
                         Collection,
                         _util.uri_joinpath(measurement.uri, "obsp"),
                         ingest_mode,
+                        context=context,
                     ) as obsp:
                         _maybe_set(
                             measurement, "obsp", obsp, use_relative_uri=use_relative_uri
                         )
                         for key in anndata.obsp.keys():
                             with create_from_matrix(
                                 SparseNDArray,
                                 _util.uri_joinpath(measurement.obsp.uri, key),
                                 conversions.to_tiledb_supported_array_type(
                                     anndata.obsp[key]
                                 ),
                                 platform_config,
                                 ingest_mode,
+                                context=context,
                             ) as sarr:
                                 _maybe_set(
                                     obsp,
                                     key,
                                     sarr,
                                     use_relative_uri=use_relative_uri,
                                 )
 
                 if len(anndata.varp.keys()) > 0:  # do not create an empty collection
                     with _create_or_open_coll(
                         Collection,
                         _util.uri_joinpath(measurement.uri, "varp"),
                         ingest_mode,
+                        context=context,
                     ) as varp:
                         _maybe_set(
                             measurement, "varp", varp, use_relative_uri=use_relative_uri
                         )
                         for key in anndata.varp.keys():
                             with create_from_matrix(
                                 SparseNDArray,
                                 _util.uri_joinpath(measurement.varp.uri, key),
                                 conversions.to_tiledb_supported_array_type(
                                     anndata.varp[key]
                                 ),
                                 platform_config,
                                 ingest_mode,
+                                context=context,
                             ) as sarr:
                                 _maybe_set(
                                     varp,
                                     key,
                                     sarr,
                                     use_relative_uri=use_relative_uri,
                                 )
@@ -402,54 +429,58 @@
                 # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
                 # MS/RAW
                 if anndata.raw is not None:
                     with _create_or_open_coll(
                         Measurement,
                         _util.uri_joinpath(experiment.ms.uri, "raw"),
                         ingest_mode,
+                        context=context,
                     ) as raw_measurement:
                         _maybe_set(
                             ms,
                             "raw",
                             raw_measurement,
                             use_relative_uri=use_relative_uri,
                         )
 
                         with _write_dataframe(
                             _util.uri_joinpath(raw_measurement.uri, "var"),
                             conversions.decategoricalize_obs_or_var(anndata.raw.var),
                             id_column_name="var_id",
                             platform_config=platform_config,
+                            context=context,
                             ingest_mode=ingest_mode,
                         ) as var:
                             _maybe_set(
                                 raw_measurement,
                                 "var",
                                 var,
                                 use_relative_uri=use_relative_uri,
                             )
 
                         with _create_or_open_coll(
                             Collection,
                             _util.uri_joinpath(raw_measurement.uri, "X"),
                             ingest_mode,
+                            context=context,
                         ) as rm_x:
                             _maybe_set(
                                 raw_measurement,
                                 "X",
                                 rm_x,
                                 use_relative_uri=use_relative_uri,
                             )
 
                             with create_from_matrix(
                                 SparseNDArray,
                                 _util.uri_joinpath(raw_measurement.X.uri, "data"),
                                 anndata.raw.X,
                                 platform_config,
                                 ingest_mode,
+                                context=context,
                             ) as rm_x_data:
                                 _maybe_set(
                                     rm_x,
                                     "data",
                                     rm_x_data,
                                     use_relative_uri=use_relative_uri,
                                 )
@@ -475,76 +506,105 @@
     except SOMAError:
         # This is already a member of the collection.
         pass
 
 
 @overload
 def _create_or_open_coll(
-    cls: Type[Experiment], uri: str, ingest_mode: str
+    cls: Type[Experiment],
+    uri: str,
+    ingest_mode: str,
+    context: Optional[SOMATileDBContext],
 ) -> Experiment:
     ...
 
 
 @overload
 def _create_or_open_coll(
-    cls: Type[Measurement], uri: str, ingest_mode: str
+    cls: Type[Measurement],
+    uri: str,
+    ingest_mode: str,
+    context: Optional[SOMATileDBContext],
 ) -> Measurement:
     ...
 
 
 @overload
 def _create_or_open_coll(
-    cls: Type[Collection[_TDBO]], uri: str, ingest_mode: str
+    cls: Type[Collection[_TDBO]],
+    uri: str,
+    ingest_mode: str,
+    context: Optional[SOMATileDBContext],
 ) -> Collection[_TDBO]:
     ...
 
 
 @typeguard_ignore
-def _create_or_open_coll(cls: Type[Any], uri: str, ingest_mode: str) -> Any:
+def _create_or_open_coll(
+    cls: Type[Any], uri: str, ingest_mode: str, context: Optional[SOMATileDBContext]
+) -> Any:
     try:
-        thing = cls.open(uri, "w")
+        thing = cls.open(uri, "w", context=context)
     except DoesNotExistError:
         # This is always OK. Make a new one.
-        return cls.create(uri)
+        return cls.create(uri, context=context)
     # It already exists. Are we resuming?
     if ingest_mode == "resume":
         return thing
     raise SOMAError(f"{uri} already exists")
 
 
 def _write_dataframe(
     df_uri: str,
     df: pd.DataFrame,
     id_column_name: Optional[str],
     platform_config: Optional[PlatformConfig] = None,
+    context: Optional[SOMATileDBContext] = None,
     ingest_mode: IngestMode = "write",
 ) -> DataFrame:
     s = _util.get_start_stamp()
     logging.log_io(None, f"START  WRITING {df_uri}")
 
     df[SOMA_JOINID] = np.asarray(range(len(df)), dtype=np.int64)
 
     df.reset_index(inplace=True)
     if id_column_name is not None:
         df.rename(columns={"index": id_column_name}, inplace=True)
     df.set_index(SOMA_JOINID, inplace=True)
 
     # Categoricals are not yet well supported, so we must flatten
+    # Also replace Numpy/Pandas-style nulls with Arrow-style nulls
+    null_fields = set()
     for k in df:
         if df[k].dtype == "category":
             df[k] = df[k].astype(df[k].cat.categories.dtype)
+        if df[k].isnull().any():
+            if df[k].isnull().all():
+                df[k] = pa.nulls(df.shape[0], pa.infer_type(df[k]))
+            else:
+                df[k].where(
+                    df[k].notnull(),
+                    pd.Series(pa.nulls(df[k].isnull().sum(), pa.infer_type(df[k]))),
+                    inplace=True,
+                )
+            null_fields.add(k)
     arrow_table = pa.Table.from_pandas(df)
+    if null_fields:
+        md = arrow_table.schema.metadata
+        md.update(dict.fromkeys(null_fields, "nullable"))
+        arrow_table = arrow_table.replace_schema_metadata(md)
 
     try:
-        soma_df = _factory.open(df_uri, "w", soma_type=DataFrame)
+        soma_df = _factory.open(df_uri, "w", soma_type=DataFrame, context=context)
     except DoesNotExistError:
         soma_df = DataFrame.create(
             df_uri,
             schema=arrow_table.schema,
             platform_config=platform_config,
+            context=context,
         )
     else:
         if ingest_mode == "resume":
             storage_ned = _read_nonempty_domain(soma_df)
             dim_range = ((int(df.index.min()), int(df.index.max())),)
             if _chunk_is_contained_in(dim_range, storage_ned):
                 logging.log_io(
@@ -573,14 +633,15 @@
 @typeguard_ignore
 def create_from_matrix(
     cls: Type[_NDArr],
     uri: str,
     matrix: Union[Matrix, h5py.Dataset],
     platform_config: Optional[PlatformConfig] = None,
     ingest_mode: IngestMode = "write",
+    context: Optional[SOMATileDBContext] = None,
 ) -> _NDArr:
     """
     Create and populate the ``soma_matrix`` from the contents of ``matrix``.
 
     Lifecycle:
         Experimental.
     """
@@ -588,23 +649,26 @@
     if len(matrix.shape) != 2:
         raise ValueError(f"expected matrix.shape == 2; got {matrix.shape}")
 
     s = _util.get_start_stamp()
     logging.log_io(None, f"START  WRITING {uri}")
 
     try:
-        soma_ndarray = cls.open(uri, "w", platform_config=platform_config)
+        soma_ndarray = cls.open(
+            uri, "w", platform_config=platform_config, context=context
+        )
     except DoesNotExistError:
         # A SparseNDArray must be appendable in soma.io.
         shape = [None for _ in matrix.shape] if cls.is_sparse else matrix.shape
         soma_ndarray = cls.create(
             uri,
             type=pa.from_numpy_dtype(matrix.dtype),
             shape=shape,
             platform_config=platform_config,
+            context=context,
         )
     else:
         if ingest_mode != "resume":
             raise SOMAError(f"{soma_ndarray.uri} already exists")
 
     if ingest_mode == "schema_only":
         logging.log_io(
@@ -621,23 +685,25 @@
     if isinstance(soma_ndarray, DenseNDArray):
         _write_matrix_to_denseNDArray(
             soma_ndarray,
             matrix,
             tiledb_create_options=TileDBCreateOptions.from_platform_config(
                 platform_config
             ),
+            context=context,
             ingest_mode=ingest_mode,
         )
     elif isinstance(soma_ndarray, SparseNDArray):  # SOMASparseNDArray
         _write_matrix_to_sparseNDArray(
             soma_ndarray,
             matrix,
             tiledb_create_options=TileDBCreateOptions.from_platform_config(
                 platform_config
             ),
+            context=context,
             ingest_mode=ingest_mode,
         )
     else:
         raise TypeError(f"unknown array type {type(soma_ndarray)}")
 
     logging.log_io(
         f"Wrote   {soma_ndarray.uri}",
@@ -679,14 +745,15 @@
     measurement_name: str,
     collection_name: str,
     matrix_name: str,
     # E.g. a scipy.csr_matrix from scanpy analysis:
     matrix_data: Union[Matrix, h5py.Dataset],
     ingest_mode: IngestMode = "write",
     use_relative_uri: Optional[bool] = None,
+    context: Optional[SOMATileDBContext] = None,
 ) -> None:
     """This is useful for adding X/obsp/varm/etc data, for example from
     `Scanpy <https://scanpy.readthedocs.io/>`_'s ``scanpy.pp.normalize_total``,
     ``scanpy.pp.log1p``, etc.
 
     Use ``ingest_mode="resume"`` to not error out if the schema already exists.
 
@@ -694,34 +761,42 @@
         Experimental.
     """
     with exp.ms[measurement_name] as meas:
         if collection_name in meas:
             coll = cast(Collection[RawHandle], meas[collection_name])
         else:
             coll = _create_or_open_coll(
-                Collection, f"{meas.uri}/{collection_name}", ingest_mode
+                Collection,
+                f"{meas.uri}/{collection_name}",
+                ingest_mode,
+                context=context,
             )
             _maybe_set(meas, collection_name, coll, use_relative_uri=use_relative_uri)
         with coll:
             uri = f"{coll.uri}/{matrix_name}"
             with create_from_matrix(
-                SparseNDArray, uri, matrix_data, ingest_mode=ingest_mode
+                SparseNDArray,
+                uri,
+                matrix_data,
+                ingest_mode=ingest_mode,
+                context=context,
             ) as sparse_nd_array:
                 _maybe_set(
                     coll,
                     matrix_name,
                     sparse_nd_array,
                     use_relative_uri=use_relative_uri,
                 )
 
 
 def _write_matrix_to_denseNDArray(
     soma_ndarray: DenseNDArray,
     matrix: Union[Matrix, h5py.Dataset],
     tiledb_create_options: TileDBCreateOptions,
+    context: Optional[SOMATileDBContext],
     ingest_mode: IngestMode,
 ) -> None:
     """Write a matrix to an empty DenseNDArray"""
 
     # There is a chunk-by-chunk already-done check for resume mode, below.
     # This full-matrix-level check here might seem redundant, but in fact it's important:
     # * By checking input bounds against storage NED here, we can see if the entire matrix
@@ -862,14 +937,17 @@
         sum_nnz += matrix[tuple(coords)].nnz
         if sum_nnz > goal_chunk_nnz:
             break
         if count > max_rows:
             break
         chunk_size += 1
 
+    if sum_nnz == 0:  # completely empty sparse array (corner case)
+        return 1
+
     if sum_nnz > goal_chunk_nnz:
         return chunk_size
 
     # Solve the equation:
     #
     # sum_nnz              count
     # -------          =  -------
@@ -880,14 +958,15 @@
     return chunk_size
 
 
 def _write_matrix_to_sparseNDArray(
     soma_ndarray: SparseNDArray,
     matrix: Matrix,
     tiledb_create_options: TileDBCreateOptions,
+    context: Optional[SOMATileDBContext],
     ingest_mode: IngestMode,
 ) -> None:
     """Write a matrix to an empty DenseNDArray"""
 
     def _coo_to_table(mat_coo: sp.coo_matrix, axis: int = 0, base: int = 0) -> pa.Table:
         pydict = {
             "soma_data": mat_coo.data,
@@ -1054,63 +1133,80 @@
     return True
 
 
 def _maybe_ingest_uns(
     m: Measurement,
     uns: Mapping[str, object],
     platform_config: Optional[PlatformConfig],
+    context: Optional[SOMATileDBContext],
     ingest_mode: IngestMode,
     *,
     use_relative_uri: Optional[bool],
 ) -> None:
     # Don't try to ingest an empty uns.
     if not uns:
         return
     _ingest_uns_dict(
-        m, "uns", uns, platform_config, ingest_mode, use_relative_uri=use_relative_uri
+        m,
+        "uns",
+        uns,
+        platform_config,
+        context,
+        ingest_mode,
+        use_relative_uri=use_relative_uri,
     )
 
 
 def _ingest_uns_dict(
     parent: AnyTileDBCollection,
     parent_key: str,
     dct: Mapping[str, object],
     platform_config: Optional[PlatformConfig],
+    context: Optional[SOMATileDBContext],
     ingest_mode: IngestMode,
     *,
     use_relative_uri: Optional[bool],
 ) -> None:
     with _create_or_open_coll(
-        Collection, _util.uri_joinpath(parent.uri, parent_key), ingest_mode
+        Collection,
+        _util.uri_joinpath(parent.uri, parent_key),
+        ingest_mode,
+        context=context,
     ) as coll:
         _maybe_set(parent, parent_key, coll, use_relative_uri=use_relative_uri)
         coll.metadata["soma_tiledbsoma_type"] = "uns"
         for key, value in dct.items():
-            if isinstance(value, (np.str_, int, float, str)):
+            if isinstance(value, np.generic):
+                # This is some kind of numpy scalar value. Metadata entries
+                # only accept native Python types, so unwrap it.
+                value = value.item()
+            if isinstance(value, (int, float, str)):
                 # Primitives get set on the metadata.
                 coll.metadata[key] = value
                 continue
             if isinstance(value, Mapping):
                 # Mappings are represented as sub-dictionaries.
                 _ingest_uns_dict(
                     coll,
                     key,
                     value,
                     platform_config,
+                    context,
                     ingest_mode,
                     use_relative_uri=use_relative_uri,
                 )
                 continue
             if isinstance(value, pd.DataFrame):
                 with _write_dataframe(
                     _util.uri_joinpath(coll.uri, key),
                     value,
                     None,
                     platform_config,
-                    ingest_mode,
+                    context=context,
+                    ingest_mode=ingest_mode,
                 ) as df:
                     _maybe_set(coll, key, df, use_relative_uri=use_relative_uri)
                 continue
             if isinstance(value, list) or "numpy" in str(type(value)):
                 value = np.asarray(value)
             if isinstance(value, np.ndarray):
                 if value.dtype.names is not None:
@@ -1123,14 +1219,15 @@
                     continue
 
                 _ingest_uns_ndarray(
                     coll,
                     key,
                     value,
                     platform_config,
+                    context=context,
                     use_relative_uri=use_relative_uri,
                 )
             else:
                 msg = (
                     f"Skipped {coll.uri}[{key!r}]"
                     f" (uns object): unrecognized type {type(value)}"
                 )
@@ -1140,14 +1237,15 @@
 
 
 def _ingest_uns_ndarray(
     coll: AnyTileDBCollection,
     key: str,
     value: NPNDArray,
     platform_config: Optional[PlatformConfig],
+    context: Optional[SOMATileDBContext],
     *,
     use_relative_uri: Optional[bool],
 ) -> None:
     arr_uri = _util.uri_joinpath(coll.uri, key)
     try:
         pa_dtype = pa.from_numpy_dtype(value.dtype)
     except pa.ArrowNotImplementedError:
@@ -1161,18 +1259,23 @@
         soma_arr = _factory.open(arr_uri, "w", soma_type=DenseNDArray)
     except DoesNotExistError:
         soma_arr = DenseNDArray.create(
             arr_uri,
             type=pa_dtype,
             shape=value.shape,
             platform_config=platform_config,
+            context=context,
         )
     with soma_arr:
         _maybe_set(coll, key, soma_arr, use_relative_uri=use_relative_uri)
-        soma_arr.write((), pa.Tensor.from_numpy(value), platform_config=platform_config)
+        soma_arr.write(
+            (),
+            pa.Tensor.from_numpy(value),
+            platform_config=platform_config,
+        )
     msg = f"Wrote   {soma_arr.uri} (uns ndarray)"
 
 
 # ----------------------------------------------------------------
 def to_h5ad(
     experiment: Experiment,
     h5ad_path: Path,
@@ -1213,18 +1316,18 @@
     var_id_name: str = "var_id",
     X_layer_name: str = "data",
 ) -> ad.AnnData:
     """Converts the experiment group to `AnnData <https://anndata.readthedocs.io/>`_
     format. Choice of matrix formats is following what we often see in input
     ``.h5ad`` files:
 
-    * X as ``scipy.sparse.csr_matrix``
-    * obs,var as ``pandas.dataframe``
-    * obsm,varm arrays as ``numpy.ndarray``
-    * obsp,varp arrays as ``scipy.sparse.csr_matrix``
+    * ``X`` as ``scipy.sparse.csr_matrix``
+    * ``obs``,``var`` as ``pandas.dataframe``
+    * ``obsm``,``varm`` arrays as ``numpy.ndarray``
+    * ``obsp``,``varp`` arrays as ``scipy.sparse.csr_matrix``
 
     Lifecycle:
         Experimental.
     """
 
     s = _util.get_start_stamp()
     logging.log_io(None, "START  Experiment.to_anndata")
@@ -1273,27 +1376,61 @@
 
     obsm = {}
     if "obsm" in measurement:
         for key in measurement.obsm.keys():
             shape = measurement.obsm[key].shape
             if len(shape) != 2:
                 raise ValueError(f"expected shape == 2; got {shape}")
-            matrix = measurement.obsm[key].read((slice(None),) * len(shape)).to_numpy()
-            # The spelling ``sp.csr_array`` is more idiomatic but doesn't exist until Python 3.8
-            obsm[key] = sp.csr_matrix(matrix)
+            if isinstance(measurement.obsm[key], DenseNDArray):
+                matrix = measurement.obsm[key].read().to_numpy()
+                # The spelling ``sp.csr_array`` is more idiomatic but doesn't exist until Python 3.8
+                obsm[key] = matrix
+            else:
+                # obsp is nobs x nobs.
+                # obsm is nobs x some number -- number of PCA components, etc.
+                matrix = measurement.obsm[key].read().tables().concat().to_pandas()
+                nobs_times_width, coo_column_count = matrix.shape
+                if coo_column_count != 3:
+                    raise SOMAError(
+                        f"internal error: expect COO width of 3; got {coo_column_count}"
+                    )
+                if nobs_times_width % nobs != 0:
+                    raise SOMAError(
+                        f"internal error: encountered non-rectangular obsm[{key}]: {nobs} does not divide {nobs_times_width}"
+                    )
+                obsm[key] = conversions.csr_from_tiledb_df(
+                    matrix, nobs, nobs_times_width // nobs
+                ).toarray()
 
     varm = {}
     if "varm" in measurement:
         for key in measurement.varm.keys():
             shape = measurement.varm[key].shape
             if len(shape) != 2:
                 raise ValueError(f"expected shape == 2; got {shape}")
-            matrix = measurement.varm[key].read((slice(None),) * len(shape)).to_numpy()
-            # The spelling ``sp.csr_array`` is more idiomatic but doesn't exist until Python 3.8
-            varm[key] = sp.csr_matrix(matrix)
+            if isinstance(measurement.varm[key], DenseNDArray):
+                matrix = measurement.varm[key].read().to_numpy()
+                # The spelling ``sp.csr_array`` is more idiomatic but doesn't exist until Python 3.8
+                varm[key] = matrix
+            else:
+                # varp is nvar x nvar.
+                # varm is nvar x some number -- number of PCs, etc.
+                matrix = measurement.varm[key].read().tables().concat().to_pandas()
+                nvar_times_width, coo_column_count = matrix.shape
+                if coo_column_count != 3:
+                    raise SOMAError(
+                        f"internal error: expect COO width of 3; got {coo_column_count}"
+                    )
+                if nvar_times_width % nvar != 0:
+                    raise SOMAError(
+                        f"internal error: encountered non-rectangular varm[{key}]: {nvar} does not divide {nvar_times_width}"
+                    )
+                varm[key] = conversions.csr_from_tiledb_df(
+                    matrix, nvar, nvar_times_width // nvar
+                ).toarray()
 
     obsp = {}
     if "obsp" in measurement:
         for key in measurement.obsp.keys():
             matrix = measurement.obsp[key].read().tables().concat().to_pandas()
             obsp[key] = conversions.csr_from_tiledb_df(matrix, nobs, nobs)
```

### Comparing `tiledbsoma-1.2.1/src/tiledbsoma/logging.py` & `tiledbsoma-1.2.2/src/tiledbsoma/logging.py`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/src/tiledbsoma/options/_soma_tiledb_context.py` & `tiledbsoma-1.2.2/src/tiledbsoma/options/_soma_tiledb_context.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,17 +83,17 @@
     def replace(
         self, *, tiledb_config: Optional[Dict[str, Any]] = None, **changes: Any
     ) -> Self:
         """Create a copy of the context, merging changes.
 
         Args:
             tiledb_config:
-                A dictionary of parameters for tiledb.Config().
+                A dictionary of parameters for `tiledb.Config() <https://tiledb-inc-tiledb.readthedocs-hosted.com/projects/tiledb-py/en/stable/python-api.html#config>`_.
             changes:
-                Any other parameters will be passed to the class __init__.
+                Any other parameters will be passed to the class ``__init__``.
 
         Lifecycle:
             Experimental.
 
         Examples:
             >>> context.replace(timestamp=0)
```

### Comparing `tiledbsoma-1.2.1/src/tiledbsoma/options/_tiledb_create_options.py` & `tiledbsoma-1.2.2/src/tiledbsoma/options/_tiledb_create_options.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,18 +25,19 @@
 DEFAULT_OFFSET_FILTERS = (
     "DoubleDeltaFilter",
     "BitWidthReductionFilter",
     "ZstdFilter",
 )
 DEFAULT_VALIDITY_FILTERS = None
 DEFAULT_TILE_EXTENT = 2048
+DEFAULT_CAPACITY = 100000
+DEFAULT_ALLOWS_DUPLICATES = False
+
 # TODO: pending further work on
 #  https://github.com/single-cell-data/TileDB-SOMA/issues/27
-# DEFAULT_OBS_EXTENT = 256
-# DEFAULT_VAR_EXTENT = 2048
 # DEFAULT_X_CAPACITY = 100000
 # DEFAULT_MAX_THREAD_POOL_WORKERS = 8
 
 StrOrMap = Union[str, Mapping[str, Any]]
 
 
 @attrs.define(frozen=True)
@@ -68,14 +69,20 @@
 
     def write_X_chunked(self) -> bool:
         return self.get("write_X_chunked", DEFAULT_WRITE_X_CHUNKED)
 
     def goal_chunk_nnz(self) -> int:
         return self.get("goal_chunk_nnz", DEFAULT_GOAL_CHUNK_NNZ)
 
+    def capacity(self) -> int:
+        return self.get("capacity", DEFAULT_CAPACITY)
+
+    def allows_duplicates(self) -> bool:
+        return self.get("allows_duplicates", DEFAULT_ALLOWS_DUPLICATES)
+
     def offsets_filters(
         self,
         default: Sequence[StrOrMap] = DEFAULT_OFFSET_FILTERS,
     ) -> Sequence[tiledb.Filter]:
         return _build_filters(self.get("offsets_filters", default))
 
     def validity_filters(
```

### Comparing `tiledbsoma-1.2.1/src/tiledbsoma/pytiledbsoma.cc` & `tiledbsoma-1.2.2/src/tiledbsoma/pytiledbsoma.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/src/tiledbsoma/query_condition.cc` & `tiledbsoma-1.2.2/src/tiledbsoma/query_condition.cc`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/src/tiledbsoma.egg-info/PKG-INFO` & `tiledbsoma-1.2.2/src/tiledbsoma.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,31 @@
 Metadata-Version: 2.1
 Name: tiledbsoma
-Version: 1.2.1
+Version: 1.2.2
 Summary: Python API for efficient storage and retrieval of single-cell data using TileDB
 Home-page: https://github.com/single-cell-data/TileDB-SOMA/tree/main/apis/python
 Author: TileDB, Inc.
 Author-email: help@tiledb.io
 Maintainer: TileDB, Inc.
 Maintainer-email: help@tiledb.io
 License: MIT
 Description: # Overview
         
-        This is a Python implementation of the [Unified Single-cell Data Model](https://github.com/single-cell-data/SOMA).
-        
-        This branch, `main`, implements the [updated specfication](https://github.com/single-cell-data/SOMA/blob/main/abstract_specification.md).  Please also see the `main-old` branch which implements the [original specification](https://github.com/single-cell-data/TileDB-SOMA/blob/main-old/spec/specification.md).
+        This is a Python implementation of the [SOMA API specification](https://github.com/single-cell-data/SOMA/blob/main/abstract_specification.md) for interacting with the [Unified Single-cell Data Model](https://github.com/single-cell-data/SOMA).
         
         # Installation
         
         ## Using pip
         
-        This code is hosted at [PyPI](https://pypi.org/project/tiledbsoma/), so you can do
+        This code is hosted at [PyPI](https://pypi.org/project/tiledbsoma/), so you can install using `pip`:
         
         ```shell
         $ python -m pip install tiledbsoma
-        # or
-        $ python -m pip install --pre tiledbsoma
         ```
         
-        Without `--pre` you will get version 0.1.* (the `main-old` branch); with `--pre`, you will get 0.5.0a* (the `main` branch).
-        
         To install a specific version:
         
         ```shell
         $ python -m pip install git+https://github.com/single-cell-data/TileDB-SOMA.git@0.0.6#subdirectory=apis/python
         ```
         
         To update to the latest version:
@@ -43,14 +37,15 @@
         ## From source
         
         * This requires [`tiledb`](https://github.com/TileDB-Inc/TileDB-Py) (see [./setup.cfg](setup.cfg) for version), in addition to other dependencies in [setup.cfg](./setup.cfg).
         * Clone [this repo](https://github.com/single-cell-data/TileDB-SOMA)
         * `cd` into your checkout and then `cd apis/python`
         * `python -m pip install .`
         * Or, if you wish to modify the code and run it, `python -m pip install -v -e .`
+        * If the TileDB and TileDB-SOMA libraries are locally installed to a custom directory, such as `/usr/local`, set the path with environment variables `TILEDB_PATH` and `TILEDBSOMA_PATH`, `TILEDB_PATH=/usr/local python -m pip install -v -e .`
         * Optionally, if you prefer, you can run that inside `venv`:
           ```shell
           $ python -m venv venv
           $ . ./venv/bin/activate
           $ python -m pip install -v -e .
           ```
         * In either case:
@@ -60,15 +55,15 @@
         
         # Status
         
         Please see [https://github.com/single-cell-data/TileDB-SOMA/issues](https://github.com/single-cell-data/TileDB-SOMA/issues).
         
         # `platform_config` format
         
-        When accessing SOMA APIs, TileDB-specific settings can be configured with the `platform_config` parameter.
+        When accessing SOMA APIs, TileDB-specific settings can be configured with the [`platform_config`](https://github.com/single-cell-data/SOMA/blob/main/abstract_specification.md#platform-specific-configuration) parameter.
         The options accepted by TileDB SOMA are described here, using [TypeScript interface syntax](https://www.typescriptlang.org/docs/handbook/2/objects.html):
         
         ```typescript
         interface PlatformConfig {
           tiledb?: TDBConfig;
         }
         
@@ -112,14 +107,16 @@
         }
         ```
         
         # Information for developers
         
         Please see the [TileDB-SOMA wiki](https://github.com/single-cell-data/TileDB-SOMA/wiki).
         
+        <!-- temp for readthedocs testing -->
+        
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Operating System :: Unix
```

### Comparing `tiledbsoma-1.2.1/src/tiledbsoma.egg-info/SOURCES.txt` & `tiledbsoma-1.2.2/src/tiledbsoma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tiledbsoma-1.2.1/version.py` & `tiledbsoma-1.2.2/version.py`

 * *Files identical despite different names*

