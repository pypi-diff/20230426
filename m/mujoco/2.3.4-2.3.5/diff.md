# Comparing `tmp/mujoco-2.3.4.tar.gz` & `tmp/mujoco-2.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mujoco-2.3.4.tar", last modified: Thu Apr 20 15:58:50 2023, max compression
+gzip compressed data, was "mujoco-2.3.5.tar", last modified: Tue Apr 25 14:29:14 2023, max compression
```

## Comparing `mujoco-2.3.4.tar` & `mujoco-2.3.5.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-04-20 15:58:50.590985 mujoco-2.3.4/
--rw-r--r--   0 jenkins    (502) staff       (20)    11358 2023-04-20 15:58:50.000000 mujoco-2.3.4/LICENSE
--rw-r--r--   0 jenkins    (502) staff       (20)    31030 2023-04-20 15:58:50.000000 mujoco-2.3.4/LICENSES_THIRD_PARTY.md
--rw-r--r--   0 jenkins    (502) staff       (20)      179 2023-04-20 15:58:50.000000 mujoco-2.3.4/MANIFEST.in
--rw-r--r--   0 jenkins    (502) staff       (20)    34948 2023-04-20 15:58:50.590834 mujoco-2.3.4/PKG-INFO
--rw-r--r--   0 jenkins    (502) staff       (20)     2987 2023-04-20 15:58:50.000000 mujoco-2.3.4/README.md
-drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-04-20 15:58:50.578605 mujoco-2.3.4/cmake/
--rw-r--r--   0 jenkins    (502) staff       (20)     1740 2023-04-20 15:58:50.000000 mujoco-2.3.4/cmake/CheckAvxSupport.cmake
--rw-r--r--   0 jenkins    (502) staff       (20)     4747 2023-04-20 15:58:50.000000 mujoco-2.3.4/cmake/FindOrFetch.cmake
--rw-r--r--   0 jenkins    (502) staff       (20)     8371 2023-04-20 15:58:50.000000 mujoco-2.3.4/cmake/MujocoDependencies.cmake
--rw-r--r--   0 jenkins    (502) staff       (20)     1242 2023-04-20 15:58:50.000000 mujoco-2.3.4/cmake/MujocoHarden.cmake
--rw-r--r--   0 jenkins    (502) staff       (20)     2302 2023-04-20 15:58:50.000000 mujoco-2.3.4/cmake/MujocoLinkOptions.cmake
--rw-r--r--   0 jenkins    (502) staff       (20)     1568 2023-04-20 15:58:50.000000 mujoco-2.3.4/cmake/MujocoMacOS.cmake
--rw-r--r--   0 jenkins    (502) staff       (20)     3918 2023-04-20 15:58:50.000000 mujoco-2.3.4/cmake/MujocoOptions.cmake
--rw-r--r--   0 jenkins    (502) staff       (20)     2164 2023-04-20 15:58:50.000000 mujoco-2.3.4/cmake/ShellTests.cmake
--rw-r--r--   0 jenkins    (502) staff       (20)     5676 2023-04-20 15:58:50.000000 mujoco-2.3.4/cmake/TargetAddRpath.cmake
-drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-04-20 15:58:50.583046 mujoco-2.3.4/mujoco/
--rw-r--r--   0 jenkins    (502) staff       (20)    13113 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/CMakeLists.txt
--rw-r--r--   0 jenkins    (502) staff       (20)     2446 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/__init__.py
--rw-r--r--   0 jenkins    (502) staff       (20)    46477 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/bindings_test.py
--rw-r--r--   0 jenkins    (502) staff       (20)    13444 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/callbacks.cc
-drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-04-20 15:58:50.584213 mujoco-2.3.4/mujoco/cgl/
--rw-r--r--   0 jenkins    (502) staff       (20)     2271 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/cgl/__init__.py
--rw-r--r--   0 jenkins    (502) staff       (20)     5204 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/cgl/cgl.py
--rw-r--r--   0 jenkins    (502) staff       (20)     2366 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/constants.cc
-drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-04-20 15:58:50.584564 mujoco-2.3.4/mujoco/egl/
--rw-r--r--   0 jenkins    (502) staff       (20)     4764 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/egl/__init__.py
--rw-r--r--   0 jenkins    (502) staff       (20)     2783 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/egl/egl_ext.py
--rw-r--r--   0 jenkins    (502) staff       (20)    30507 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/enum_traits.h
--rw-r--r--   0 jenkins    (502) staff       (20)     4704 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/enums.cc
--rw-r--r--   0 jenkins    (502) staff       (20)      885 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/errors.cc
--rw-r--r--   0 jenkins    (502) staff       (20)     7747 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/errors.h
--rw-r--r--   0 jenkins    (502) staff       (20)   121911 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/function_traits.h
--rw-r--r--   0 jenkins    (502) staff       (20)    46647 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/functions.cc
--rw-r--r--   0 jenkins    (502) staff       (20)     7964 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/functions.h
--rw-r--r--   0 jenkins    (502) staff       (20)     1849 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/gl_context.py
-drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-04-20 15:58:50.584727 mujoco-2.3.4/mujoco/glfw/
--rw-r--r--   0 jenkins    (502) staff       (20)     1403 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/glfw/__init__.py
--rw-r--r--   0 jenkins    (502) staff       (20)    20668 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/indexer_xmacro.h
--rw-r--r--   0 jenkins    (502) staff       (20)    15911 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/indexers.cc
--rw-r--r--   0 jenkins    (502) staff       (20)     7177 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/indexers.h
--rw-r--r--   0 jenkins    (502) staff       (20)     3474 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/mjdata_meta.h
-drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-04-20 15:58:50.585700 mujoco-2.3.4/mujoco/mjpython/
--rw-r--r--   0 jenkins    (502) staff       (20)     1113 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/mjpython/Info.plist
--rw-r--r--   0 jenkins    (502) staff       (20)   432307 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/mjpython/mjpython.icns
--rw-r--r--   0 jenkins    (502) staff       (20)    12145 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/mjpython/mjpython.mm
--rw-r--r--   0 jenkins    (502) staff       (20)     2286 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/mjpython/mjpython.py
-drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-04-20 15:58:50.585899 mujoco-2.3.4/mujoco/osmesa/
--rw-r--r--   0 jenkins    (502) staff       (20)     2556 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/osmesa/__init__.py
--rw-r--r--   0 jenkins    (502) staff       (20)     1962 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/raw.h
--rw-r--r--   0 jenkins    (502) staff       (20)     8709 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/render.cc
--rw-r--r--   0 jenkins    (502) staff       (20)     3822 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/render_test.py
--rw-r--r--   0 jenkins    (502) staff       (20)     8993 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/renderer.py
--rw-r--r--   0 jenkins    (502) staff       (20)     3655 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/renderer_test.py
--rw-r--r--   0 jenkins    (502) staff       (20)     9004 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/rollout.cc
--rw-r--r--   0 jenkins    (502) staff       (20)     7793 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/rollout.py
--rw-r--r--   0 jenkins    (502) staff       (20)    18173 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/rollout_test.py
--rw-r--r--   0 jenkins    (502) staff       (20)     2318 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/serialization.h
-drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-04-20 15:58:50.588367 mujoco-2.3.4/mujoco/simulate/
--rw-r--r--   0 jenkins    (502) staff       (20)     9588 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/simulate/CMakeLists.txt
--rw-r--r--   0 jenkins    (502) staff       (20)     3337 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/simulate/array_safety.h
-drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-04-20 15:58:50.588790 mujoco-2.3.4/mujoco/simulate/cmake/
--rw-r--r--   0 jenkins    (502) staff       (20)     2635 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/simulate/cmake/SimulateDependencies.cmake
--rw-r--r--   0 jenkins    (502) staff       (20)     3918 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/simulate/cmake/SimulateOptions.cmake
--rw-r--r--   0 jenkins    (502) staff       (20)     7725 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/simulate/glfw_adapter.cc
--rw-r--r--   0 jenkins    (502) staff       (20)     2489 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/simulate/glfw_adapter.h
--rw-r--r--   0 jenkins    (502) staff       (20)     1487 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/simulate/glfw_corevideo.h
--rw-r--r--   0 jenkins    (502) staff       (20)     2530 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/simulate/glfw_corevideo.mm
--rw-r--r--   0 jenkins    (502) staff       (20)     4395 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/simulate/glfw_dispatch.cc
--rw-r--r--   0 jenkins    (502) staff       (20)     2884 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/simulate/glfw_dispatch.h
--rw-r--r--   0 jenkins    (502) staff       (20)     1656 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/simulate/macos_gui.mm
--rw-r--r--   0 jenkins    (502) staff       (20)    14318 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/simulate/main.cc
--rw-r--r--   0 jenkins    (502) staff       (20)     6095 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/simulate/platform_ui_adapter.cc
--rw-r--r--   0 jenkins    (502) staff       (20)     3319 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/simulate/platform_ui_adapter.h
--rw-r--r--   0 jenkins    (502) staff       (20)    74967 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/simulate/simulate.cc
--rw-r--r--   0 jenkins    (502) staff       (20)     8972 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/simulate/simulate.h
--rw-r--r--   0 jenkins    (502) staff       (20)     6913 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/simulate.cc
--rw-r--r--   0 jenkins    (502) staff       (20)    71425 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/structs.cc
--rw-r--r--   0 jenkins    (502) staff       (20)    31352 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/structs.h
-drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-04-20 15:58:50.590577 mujoco-2.3.4/mujoco/util/
--rw-r--r--   0 jenkins    (502) staff       (20)     3288 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/util/CMakeLists.txt
--rw-r--r--   0 jenkins    (502) staff       (20)     4893 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/util/array_traits.h
--rw-r--r--   0 jenkins    (502) staff       (20)     2516 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/util/array_traits_test.cc
--rw-r--r--   0 jenkins    (502) staff       (20)     2426 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/util/crossplatform.h
--rw-r--r--   0 jenkins    (502) staff       (20)     4146 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/util/func_traits.h
--rw-r--r--   0 jenkins    (502) staff       (20)     4013 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/util/func_traits_test.cc
--rw-r--r--   0 jenkins    (502) staff       (20)     7119 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/util/func_wrap.h
--rw-r--r--   0 jenkins    (502) staff       (20)     2944 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/util/func_wrap_test.cc
--rw-r--r--   0 jenkins    (502) staff       (20)     5690 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/util/tuple_tools.h
--rw-r--r--   0 jenkins    (502) staff       (20)     1945 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/util/tuple_tools_test.cc
--rw-r--r--   0 jenkins    (502) staff       (20)    12239 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/viewer.py
--rw-r--r--   0 jenkins    (502) staff       (20)      979 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco/viewer_test.py
-drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-04-20 15:58:50.583879 mujoco-2.3.4/mujoco.egg-info/
--rw-r--r--   0 jenkins    (502) staff       (20)    34948 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (502) staff       (20)     2130 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (502) staff       (20)        1 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (502) staff       (20)       28 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco.egg-info/requires.txt
--rw-r--r--   0 jenkins    (502) staff       (20)        7 2023-04-20 15:58:50.000000 mujoco-2.3.4/mujoco.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (502) staff       (20)       38 2023-04-20 15:58:50.591013 mujoco-2.3.4/setup.cfg
--rw-r--r--   0 jenkins    (502) staff       (20)    14305 2023-04-20 15:58:50.000000 mujoco-2.3.4/setup.py
+drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-04-25 14:29:14.160325 mujoco-2.3.5/
+-rw-r--r--   0 jenkins    (502) staff       (20)    11358 2023-04-25 14:29:14.000000 mujoco-2.3.5/LICENSE
+-rw-r--r--   0 jenkins    (502) staff       (20)    31030 2023-04-25 14:29:13.000000 mujoco-2.3.5/LICENSES_THIRD_PARTY.md
+-rw-r--r--   0 jenkins    (502) staff       (20)      179 2023-04-25 14:29:13.000000 mujoco-2.3.5/MANIFEST.in
+-rw-r--r--   0 jenkins    (502) staff       (20)    34948 2023-04-25 14:29:14.160187 mujoco-2.3.5/PKG-INFO
+-rw-r--r--   0 jenkins    (502) staff       (20)     2987 2023-04-25 14:29:13.000000 mujoco-2.3.5/README.md
+drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-04-25 14:29:14.151831 mujoco-2.3.5/cmake/
+-rw-r--r--   0 jenkins    (502) staff       (20)     1740 2023-04-25 14:29:14.000000 mujoco-2.3.5/cmake/CheckAvxSupport.cmake
+-rw-r--r--   0 jenkins    (502) staff       (20)     4747 2023-04-25 14:29:14.000000 mujoco-2.3.5/cmake/FindOrFetch.cmake
+-rw-r--r--   0 jenkins    (502) staff       (20)     8371 2023-04-25 14:29:14.000000 mujoco-2.3.5/cmake/MujocoDependencies.cmake
+-rw-r--r--   0 jenkins    (502) staff       (20)     1242 2023-04-25 14:29:14.000000 mujoco-2.3.5/cmake/MujocoHarden.cmake
+-rw-r--r--   0 jenkins    (502) staff       (20)     2302 2023-04-25 14:29:14.000000 mujoco-2.3.5/cmake/MujocoLinkOptions.cmake
+-rw-r--r--   0 jenkins    (502) staff       (20)     1568 2023-04-25 14:29:14.000000 mujoco-2.3.5/cmake/MujocoMacOS.cmake
+-rw-r--r--   0 jenkins    (502) staff       (20)     3918 2023-04-25 14:29:14.000000 mujoco-2.3.5/cmake/MujocoOptions.cmake
+-rw-r--r--   0 jenkins    (502) staff       (20)     2164 2023-04-25 14:29:14.000000 mujoco-2.3.5/cmake/ShellTests.cmake
+-rw-r--r--   0 jenkins    (502) staff       (20)     5676 2023-04-25 14:29:14.000000 mujoco-2.3.5/cmake/TargetAddRpath.cmake
+drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-04-25 14:29:14.155315 mujoco-2.3.5/mujoco/
+-rw-r--r--   0 jenkins    (502) staff       (20)    13113 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/CMakeLists.txt
+-rw-r--r--   0 jenkins    (502) staff       (20)     2446 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/__init__.py
+-rw-r--r--   0 jenkins    (502) staff       (20)    46477 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/bindings_test.py
+-rw-r--r--   0 jenkins    (502) staff       (20)    13444 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/callbacks.cc
+drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-04-25 14:29:14.156060 mujoco-2.3.5/mujoco/cgl/
+-rw-r--r--   0 jenkins    (502) staff       (20)     2271 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/cgl/__init__.py
+-rw-r--r--   0 jenkins    (502) staff       (20)     5204 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/cgl/cgl.py
+-rw-r--r--   0 jenkins    (502) staff       (20)     2366 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/constants.cc
+drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-04-25 14:29:14.156273 mujoco-2.3.5/mujoco/egl/
+-rw-r--r--   0 jenkins    (502) staff       (20)     4764 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/egl/__init__.py
+-rw-r--r--   0 jenkins    (502) staff       (20)     2783 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/egl/egl_ext.py
+-rw-r--r--   0 jenkins    (502) staff       (20)    30507 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/enum_traits.h
+-rw-r--r--   0 jenkins    (502) staff       (20)     4704 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/enums.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)      885 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/errors.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)     7747 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/errors.h
+-rw-r--r--   0 jenkins    (502) staff       (20)   121937 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco/function_traits.h
+-rw-r--r--   0 jenkins    (502) staff       (20)    46647 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/functions.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)     7964 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/functions.h
+-rw-r--r--   0 jenkins    (502) staff       (20)     1849 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/gl_context.py
+drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-04-25 14:29:14.156372 mujoco-2.3.5/mujoco/glfw/
+-rw-r--r--   0 jenkins    (502) staff       (20)     1403 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/glfw/__init__.py
+-rw-r--r--   0 jenkins    (502) staff       (20)    20668 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/indexer_xmacro.h
+-rw-r--r--   0 jenkins    (502) staff       (20)    15911 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/indexers.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)     7177 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/indexers.h
+-rw-r--r--   0 jenkins    (502) staff       (20)     3474 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/mjdata_meta.h
+drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-04-25 14:29:14.157000 mujoco-2.3.5/mujoco/mjpython/
+-rw-r--r--   0 jenkins    (502) staff       (20)     1113 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/mjpython/Info.plist
+-rw-r--r--   0 jenkins    (502) staff       (20)   432307 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/mjpython/mjpython.icns
+-rw-r--r--   0 jenkins    (502) staff       (20)    12145 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/mjpython/mjpython.mm
+-rw-r--r--   0 jenkins    (502) staff       (20)     2286 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/mjpython/mjpython.py
+drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-04-25 14:29:14.157104 mujoco-2.3.5/mujoco/osmesa/
+-rw-r--r--   0 jenkins    (502) staff       (20)     2556 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/osmesa/__init__.py
+-rw-r--r--   0 jenkins    (502) staff       (20)     1962 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/raw.h
+-rw-r--r--   0 jenkins    (502) staff       (20)     8709 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/render.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)     3822 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/render_test.py
+-rw-r--r--   0 jenkins    (502) staff       (20)     8993 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/renderer.py
+-rw-r--r--   0 jenkins    (502) staff       (20)     3655 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/renderer_test.py
+-rw-r--r--   0 jenkins    (502) staff       (20)     9004 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/rollout.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)     7793 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/rollout.py
+-rw-r--r--   0 jenkins    (502) staff       (20)    18173 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/rollout_test.py
+-rw-r--r--   0 jenkins    (502) staff       (20)     2318 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/serialization.h
+drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-04-25 14:29:14.158600 mujoco-2.3.5/mujoco/simulate/
+-rw-r--r--   0 jenkins    (502) staff       (20)     9588 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco/simulate/CMakeLists.txt
+-rw-r--r--   0 jenkins    (502) staff       (20)     3337 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco/simulate/array_safety.h
+drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-04-25 14:29:14.158815 mujoco-2.3.5/mujoco/simulate/cmake/
+-rw-r--r--   0 jenkins    (502) staff       (20)     2635 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco/simulate/cmake/SimulateDependencies.cmake
+-rw-r--r--   0 jenkins    (502) staff       (20)     3918 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco/simulate/cmake/SimulateOptions.cmake
+-rw-r--r--   0 jenkins    (502) staff       (20)     7725 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco/simulate/glfw_adapter.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)     2489 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco/simulate/glfw_adapter.h
+-rw-r--r--   0 jenkins    (502) staff       (20)     1487 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco/simulate/glfw_corevideo.h
+-rw-r--r--   0 jenkins    (502) staff       (20)     2530 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco/simulate/glfw_corevideo.mm
+-rw-r--r--   0 jenkins    (502) staff       (20)     4395 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco/simulate/glfw_dispatch.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)     2884 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco/simulate/glfw_dispatch.h
+-rw-r--r--   0 jenkins    (502) staff       (20)     1656 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco/simulate/macos_gui.mm
+-rw-r--r--   0 jenkins    (502) staff       (20)    14318 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco/simulate/main.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)     6095 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco/simulate/platform_ui_adapter.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)     3319 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco/simulate/platform_ui_adapter.h
+-rw-r--r--   0 jenkins    (502) staff       (20)    74787 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco/simulate/simulate.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)     8995 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco/simulate/simulate.h
+-rw-r--r--   0 jenkins    (502) staff       (20)     6913 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/simulate.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)    71425 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/structs.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)    31352 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/structs.h
+drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-04-25 14:29:14.159995 mujoco-2.3.5/mujoco/util/
+-rw-r--r--   0 jenkins    (502) staff       (20)     3288 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/util/CMakeLists.txt
+-rw-r--r--   0 jenkins    (502) staff       (20)     4893 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/util/array_traits.h
+-rw-r--r--   0 jenkins    (502) staff       (20)     2516 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/util/array_traits_test.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)     2426 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/util/crossplatform.h
+-rw-r--r--   0 jenkins    (502) staff       (20)     4146 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/util/func_traits.h
+-rw-r--r--   0 jenkins    (502) staff       (20)     4013 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/util/func_traits_test.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)     7119 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/util/func_wrap.h
+-rw-r--r--   0 jenkins    (502) staff       (20)     2944 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/util/func_wrap_test.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)     5690 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/util/tuple_tools.h
+-rw-r--r--   0 jenkins    (502) staff       (20)     1945 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/util/tuple_tools_test.cc
+-rw-r--r--   0 jenkins    (502) staff       (20)    12239 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/viewer.py
+-rw-r--r--   0 jenkins    (502) staff       (20)      979 2023-04-25 14:29:13.000000 mujoco-2.3.5/mujoco/viewer_test.py
+drwxr-xr-x   0 jenkins    (502) staff       (20)        0 2023-04-25 14:29:14.155863 mujoco-2.3.5/mujoco.egg-info/
+-rw-r--r--   0 jenkins    (502) staff       (20)    34948 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (502) staff       (20)     2130 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (502) staff       (20)        1 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (502) staff       (20)       28 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (502) staff       (20)        7 2023-04-25 14:29:14.000000 mujoco-2.3.5/mujoco.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (502) staff       (20)       38 2023-04-25 14:29:14.160359 mujoco-2.3.5/setup.cfg
+-rw-r--r--   0 jenkins    (502) staff       (20)    14305 2023-04-25 14:29:13.000000 mujoco-2.3.5/setup.py
```

### Comparing `mujoco-2.3.4/LICENSE` & `mujoco-2.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/LICENSES_THIRD_PARTY.md` & `mujoco-2.3.5/LICENSES_THIRD_PARTY.md`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/PKG-INFO` & `mujoco-2.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mujoco
-Version: 2.3.4
+Version: 2.3.5
 Summary: MuJoCo Physics Simulator
 Home-page: https://github.com/deepmind/mujoco
 Author: DeepMind
 Author-email: mujoco@deepmind.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `mujoco-2.3.4/README.md` & `mujoco-2.3.5/README.md`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/cmake/CheckAvxSupport.cmake` & `mujoco-2.3.5/cmake/CheckAvxSupport.cmake`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/cmake/FindOrFetch.cmake` & `mujoco-2.3.5/cmake/FindOrFetch.cmake`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/cmake/MujocoDependencies.cmake` & `mujoco-2.3.5/cmake/MujocoDependencies.cmake`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/cmake/MujocoHarden.cmake` & `mujoco-2.3.5/cmake/MujocoHarden.cmake`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/cmake/MujocoLinkOptions.cmake` & `mujoco-2.3.5/cmake/MujocoLinkOptions.cmake`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/cmake/MujocoMacOS.cmake` & `mujoco-2.3.5/cmake/MujocoMacOS.cmake`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/cmake/MujocoOptions.cmake` & `mujoco-2.3.5/cmake/MujocoOptions.cmake`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/cmake/ShellTests.cmake` & `mujoco-2.3.5/cmake/ShellTests.cmake`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/cmake/TargetAddRpath.cmake` & `mujoco-2.3.5/cmake/TargetAddRpath.cmake`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/CMakeLists.txt` & `mujoco-2.3.5/mujoco/CMakeLists.txt`

 * *Files 0% similar despite different names*

```diff
@@ -80,23 +80,23 @@
     # On macOS, check if we are using mujoco.framework first.
     # Framework headers are searched differently from normal headers.
     # We need to use -F instead of the usual target_include_directories.
     find_path(MUJOCO_FRAMEWORK mujoco.Framework HINTS ${MUJOCO_FRAMEWORK_DIR})
     if(MUJOCO_FRAMEWORK)
       message("MuJoCo framework is at ${MUJOCO_FRAMEWORK}/mujoco.framework")
       set(MUJOCO_LIBRARY
-          ${MUJOCO_FRAMEWORK}/mujoco.framework/Versions/A/libmujoco.2.3.4.dylib
+          ${MUJOCO_FRAMEWORK}/mujoco.framework/Versions/A/libmujoco.2.3.5.dylib
       )
       target_compile_options(mujoco INTERFACE -F${MUJOCO_FRAMEWORK})
     endif()
   endif()
 
   if(NOT MUJOCO_FRAMEWORK)
     find_library(
-      MUJOCO_LIBRARY mujoco mujoco.2.3.4 HINTS ${MUJOCO_LIBRARY_DIR} REQUIRED
+      MUJOCO_LIBRARY mujoco mujoco.2.3.5 HINTS ${MUJOCO_LIBRARY_DIR} REQUIRED
     )
     find_path(MUJOCO_INCLUDE mujoco/mujoco.h HINTS ${MUJOCO_INCLUDE_DIR} REQUIRED)
     message("MuJoCo is at ${MUJOCO_LIBRARY}")
     message("MuJoCo headers are at ${MUJOCO_INCLUDE}")
     target_include_directories(mujoco INTERFACE "${MUJOCO_INCLUDE}")
   endif()
```

### Comparing `mujoco-2.3.4/mujoco/__init__.py` & `mujoco-2.3.5/mujoco/__init__.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/bindings_test.py` & `mujoco-2.3.5/mujoco/bindings_test.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/callbacks.cc` & `mujoco-2.3.5/mujoco/callbacks.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/cgl/__init__.py` & `mujoco-2.3.5/mujoco/cgl/__init__.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/cgl/cgl.py` & `mujoco-2.3.5/mujoco/cgl/cgl.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/constants.cc` & `mujoco-2.3.5/mujoco/constants.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/egl/__init__.py` & `mujoco-2.3.5/mujoco/egl/__init__.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/egl/egl_ext.py` & `mujoco-2.3.5/mujoco/egl/egl_ext.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/enum_traits.h` & `mujoco-2.3.5/mujoco/enum_traits.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/enums.cc` & `mujoco-2.3.5/mujoco/enums.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/errors.cc` & `mujoco-2.3.5/mujoco/errors.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/errors.h` & `mujoco-2.3.5/mujoco/errors.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/function_traits.h` & `mujoco-2.3.5/mujoco/function_traits.h`

 * *Files 0% similar despite different names*

```diff
@@ -1682,16 +1682,16 @@
     return ::mjv_freeSceneState;
   }
 };
 
 struct mjv_updateSceneState {
   static constexpr char name[] = "mjv_updateSceneState";
   static constexpr char doc[] = "Update a scene state from model and data.";
-  using type = void (const mjModel *, mjData *, mjvSceneState *);
-  static constexpr auto param_names = std::make_tuple("m", "d", "scnstate");
+  using type = void (const mjModel *, mjData *, const mjvOption *, mjvSceneState *);
+  static constexpr auto param_names = std::make_tuple("m", "d", "opt", "scnstate");
 
   MUJOCO_ALWAYS_INLINE static type& GetFunc() {
     return ::mjv_updateSceneState;
   }
 };
 
 struct mjv_addGeoms {
```

### Comparing `mujoco-2.3.4/mujoco/functions.cc` & `mujoco-2.3.5/mujoco/functions.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/functions.h` & `mujoco-2.3.5/mujoco/functions.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/gl_context.py` & `mujoco-2.3.5/mujoco/gl_context.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/glfw/__init__.py` & `mujoco-2.3.5/mujoco/glfw/__init__.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/indexer_xmacro.h` & `mujoco-2.3.5/mujoco/indexer_xmacro.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/indexers.cc` & `mujoco-2.3.5/mujoco/indexers.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/indexers.h` & `mujoco-2.3.5/mujoco/indexers.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/mjdata_meta.h` & `mujoco-2.3.5/mujoco/mjdata_meta.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/mjpython/Info.plist` & `mujoco-2.3.5/mujoco/mjpython/Info.plist`

 * *Files 15% similar despite different names*

#### Comparing `mujoco-2.3.4/mujoco/mjpython/Info.plist` & `mujoco-2.3.5/mujoco/mjpython/Info.plist`

```diff
@@ -5,21 +5,21 @@
 <plist version="1.0">
   <dict>
     <key>CFBundleName</key>
     <string>mjpython</string>
     <key>CFBundleIdentifier</key>
     <string>org.mujoco.mjpython</string>
     <key>CFBundleVersion</key>
-    <string>2.3.4</string>
+    <string>2.3.5</string>
     <key>CFBundleGetInfoString</key>
-    <string>2.3.4</string>
+    <string>2.3.5</string>
     <key>CFBundleLongVersionString</key>
-    <string>2.3.4</string>
+    <string>2.3.5</string>
     <key>CFBundleShortVersionString</key>
-    <string>2.3.4</string>
+    <string>2.3.5</string>
     <key>CFBundleExecutable</key>
     <string>mjpython</string>
     <key>CFBundleIconFile</key>
     <string>mjpython.icns</string>
     <key>CFBundlePackageType</key>
     <string>APPL</string>
     <key>NSHumanReadableCopyright</key>
```

### Comparing `mujoco-2.3.4/mujoco/mjpython/mjpython.icns` & `mujoco-2.3.5/mujoco/mjpython/mjpython.icns`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/mjpython/mjpython.mm` & `mujoco-2.3.5/mujoco/mjpython/mjpython.mm`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/mjpython/mjpython.py` & `mujoco-2.3.5/mujoco/mjpython/mjpython.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/osmesa/__init__.py` & `mujoco-2.3.5/mujoco/osmesa/__init__.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/raw.h` & `mujoco-2.3.5/mujoco/raw.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/render.cc` & `mujoco-2.3.5/mujoco/render.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/render_test.py` & `mujoco-2.3.5/mujoco/render_test.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/renderer.py` & `mujoco-2.3.5/mujoco/renderer.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/renderer_test.py` & `mujoco-2.3.5/mujoco/renderer_test.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/rollout.cc` & `mujoco-2.3.5/mujoco/rollout.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/rollout.py` & `mujoco-2.3.5/mujoco/rollout.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/rollout_test.py` & `mujoco-2.3.5/mujoco/rollout_test.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/serialization.h` & `mujoco-2.3.5/mujoco/serialization.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/simulate/CMakeLists.txt` & `mujoco-2.3.5/mujoco/simulate/CMakeLists.txt`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 set(MUJOCO_DEP_VERSION_lodepng
     b4ed2cd7ecf61d29076169b49199371456d4f90b
     CACHE STRING "Version of `lodepng` to be fetched."
 )
 
 project(
   mujoco_simulate
-  VERSION 2.3.4
+  VERSION 2.3.5
   DESCRIPTION "MuJoCo simulate binaries"
   HOMEPAGE_URL "https://mujoco.org"
 )
 
 enable_language(C)
 enable_language(CXX)
 if(APPLE)
```

### Comparing `mujoco-2.3.4/mujoco/simulate/array_safety.h` & `mujoco-2.3.5/mujoco/simulate/array_safety.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/simulate/cmake/SimulateDependencies.cmake` & `mujoco-2.3.5/mujoco/simulate/cmake/SimulateDependencies.cmake`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/simulate/cmake/SimulateOptions.cmake` & `mujoco-2.3.5/mujoco/simulate/cmake/SimulateOptions.cmake`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/simulate/glfw_adapter.cc` & `mujoco-2.3.5/mujoco/simulate/glfw_adapter.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/simulate/glfw_adapter.h` & `mujoco-2.3.5/mujoco/simulate/glfw_adapter.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/simulate/glfw_corevideo.h` & `mujoco-2.3.5/mujoco/simulate/glfw_corevideo.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/simulate/glfw_corevideo.mm` & `mujoco-2.3.5/mujoco/simulate/glfw_corevideo.mm`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/simulate/glfw_dispatch.cc` & `mujoco-2.3.5/mujoco/simulate/glfw_dispatch.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/simulate/glfw_dispatch.h` & `mujoco-2.3.5/mujoco/simulate/glfw_dispatch.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/simulate/macos_gui.mm` & `mujoco-2.3.5/mujoco/simulate/macos_gui.mm`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/simulate/main.cc` & `mujoco-2.3.5/mujoco/simulate/main.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/simulate/platform_ui_adapter.cc` & `mujoco-2.3.5/mujoco/simulate/platform_ui_adapter.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/simulate/platform_ui_adapter.h` & `mujoco-2.3.5/mujoco/simulate/platform_ui_adapter.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/simulate/simulate.cc` & `mujoco-2.3.5/mujoco/simulate/simulate.cc`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 #include "simulate.h"
 
 #include <atomic>
 #include <chrono>
 #include <cstdio>
 #include <cstring>
 #include <memory>
+#include <optional>
 #include <ratio>
 #include <string>
 #include <type_traits>
 #include <utility>
 
 #include "lodepng.h"
 #include <mujoco/mjdata.h>
@@ -49,34 +50,25 @@
 namespace mj = ::mujoco;
 namespace mju = ::mujoco::sample_util;
 
 using Seconds = std::chrono::duration<double>;
 using Milliseconds = std::chrono::duration<double, std::milli>;
 
 template <typename T>
-inline bool ScalarsDiffer(const T& a, const T& b) {
-  return a != b;
-}
-
-template <typename T, int N>
-inline bool ArraysDiffer(const T (&a)[N], const T (&b)[N]) {
-  for (int i = 0; i < N; ++i) {
-    if (a[i] != b[i]) {
-      return true;
-    }
-  }
-  return false;
-}
-
-template <typename T>
-inline bool Differ(const T& a, const T& b) {
+inline bool IsDifferent(const T& a, const T& b) {
   if constexpr (std::is_array_v<T>) {
-    return ArraysDiffer(a, b);
+    static_assert(std::rank_v<T> == 1);
+    for (int i = 0; i < std::extent_v<T>; ++i) {
+      if (a[i] != b[i]) {
+        return true;
+      }
+    }
+    return false;
   } else {
-    return ScalarsDiffer(a, b);
+    return a != b;
   }
 }
 
 template <typename T>
 inline void CopyScalar(T& dst, const T& src) {
   dst = src;
 }
@@ -1028,31 +1020,40 @@
   sim->platform_ui->SetClipboardString(clipboard);
 }
 
 // update UI 0 when MuJoCo structures change (except for joint sliders)
 void UpdateSettings(mj::Simulate* sim, const mjModel* m) {
   // physics flags
   for (int i=0; i<mjNDISABLE; i++) {
-    sim->disable[i] = ((m->opt.disableflags & (1<<i)) !=0);
+    int new_value = ((m->opt.disableflags & (1<<i)) !=0);
+    if (sim->disable[i] != new_value) {
+      sim->disable[i] = new_value;
+      sim->pending_.ui_update_physics = true;
+    }
   }
   for (int i=0; i<mjNENABLE; i++) {
-    sim->enable[i] = ((m->opt.enableflags & (1<<i)) !=0);
+    int new_value = ((m->opt.enableflags & (1<<i)) !=0);
+    if (sim->enable[i] != new_value) {
+      sim->enable[i] = new_value;
+      sim->pending_.ui_update_physics = true;
+    }
   }
 
   // camera
+  int old_camera = sim->camera;
   if (sim->cam.type==mjCAMERA_FIXED) {
     sim->camera = 2 + sim->cam.fixedcamid;
   } else if (sim->cam.type==mjCAMERA_TRACKING) {
     sim->camera = 1;
   } else {
     sim->camera = 0;
   }
-
-  // update UI
-  sim->pending_.full_ui_update = true;
+  if (old_camera != sim->camera) {
+    sim->pending_.ui_update_rendering = true;
+  }
 }
 
 // Compute suitable font scale.
 int ComputeFontScale(const mj::PlatformUIAdapter& platform_ui) {
   // compute framebuffer-to-window ratio
   auto [buf_width, buf_height] = platform_ui.GetFramebufferSize();
   auto [win_width, win_height] = platform_ui.GetWindowSize();
@@ -1553,15 +1554,14 @@
 void Simulate::Sync() {
   if (!m_) {
     return;
   }
 
   bool update_profiler = this->profiler && (this->run || !this->m_);
   bool update_sensor = this->sensor && (this->run || !this->m_);
-  bool update_settings = false;
 
   for (int i = 0; i < m_->njnt; ++i) {
     std::optional<std::pair<mjtNum, mjtNum>> range;
     if (m_->jnt_limited[i]) {
       range.emplace(m_->jnt_range[2*i], m_->jnt_range[2*i + 1]);
     }
     if (jnt_range_[i] != range) {
@@ -1603,19 +1603,19 @@
       pending_.ui_update_ctrl = true;
       ctrl_prev_[i] = ctrl_[i];
     }
   }
 
   if (!fully_managed_) {
     // synchronize m_->opt with changes made via the UI
-  #define X(name)                                             \
-    if (Differ(scnstate_.model.opt.name, mjopt_prev_.name)) { \
-      pending_.ui_update_physics = true;                      \
-      Copy(m_->opt.name, scnstate_.model.opt.name);           \
-    }
+#define X(name)                                                  \
+  if (IsDifferent(scnstate_.model.opt.name, mjopt_prev_.name)) { \
+    pending_.ui_update_physics = true;                           \
+    Copy(m_->opt.name, scnstate_.model.opt.name);                \
+  }
 
     X(timestep);
     X(apirate);
     X(impratio);
     X(tolerance);
     X(noslip_tolerance);
     X(mpr_tolerance);
@@ -1677,21 +1677,19 @@
   }
 
   if (pending_.reset) {
     mj_resetData(m_, d_);
     mj_forward(m_, d_);
     update_profiler = true;
     update_sensor = true;
-    update_settings = true;
     pending_.reset = false;
   }
 
   if (pending_.align) {
     AlignAndScaleView(this, m_);
-    update_settings = true;
     pending_.align = false;
   }
 
   if (pending_.copy_pose) {
     CopyPose(this, m_, d_);
     pending_.copy_pose = false;
   }
@@ -1705,15 +1703,14 @@
     mju_copy(d_->mocap_pos, m_->key_mpos + i*3*m_->nmocap, 3*m_->nmocap);
     mju_copy(d_->mocap_quat, m_->key_mquat + i*4*m_->nmocap,
               4*m_->nmocap);
     mju_copy(d_->ctrl, m_->key_ctrl + i*m_->nu, m_->nu);
     mj_forward(m_, d_);
     update_profiler = true;
     update_sensor = true;
-    update_settings = true;
     pending_.load_key = false;
   }
 
   if (pending_.save_key) {
     int i = this->key;
     m_->key_time[i] = d_->time;
     mju_copy(m_->key_qpos + i*m_->nq, d_->qpos, m_->nq);
@@ -1770,16 +1767,15 @@
         // mujoco camera
         this->cam.type = mjCAMERA_TRACKING;
         this->cam.trackbodyid = selbody;
         this->cam.fixedcamid = -1;
 
         // UI camera
         this->camera = 1;
-        mjui_update(SECT_RENDERING, -1, &this->ui0, &pending_.select_state,
-                    &this->platform_ui->mjr_context());
+        pending_.ui_update_rendering = true;
       }
     }
 
     // set body selection
     else {
       if (selbody>=0) {
         // record selection
@@ -1798,31 +1794,33 @@
     pending_.select = false;
   }
 
   // update scene
   if (fully_managed_) {
     mjv_updateScene(m_, d_, &this->opt, &this->pert, &this->cam, mjCAT_ALL, &this->scn);
   } else {
-    mjv_updateSceneState(m_, d_, &scnstate_);
+    mjv_updateSceneState(m_, d_, &this->opt, &scnstate_);
     mjopt_prev_ = scnstate_.model.opt;
     warn_vgeomfull_prev_ = scnstate_.data.warning[mjWARN_VGEOMFULL].number;
   }
 
+  // update settings
+  UpdateSettings(this, m_);
+
   // update watch
   if (this->ui0_enable && this->ui0.sect[SECT_WATCH].state) {
     UpdateWatch(this, m_, d_);
   }
 
   // update info text
   if (this->info) {
     UpdateInfoText(this, m_, d_, this->info_title, this->info_content);
   }
   if (update_profiler) { UpdateProfiler(this, m_, d_); }
   if (update_sensor) { UpdateSensor(this, m_, d_); }
-  if (update_settings) { UpdateSettings(this, m_); }
 
   // clear timers once profiler info has been copied
   ClearTimers(d_);
 
   if (this->run || !this->fully_managed_) {
     // clear old perturbations, apply new
     mju_zero(d_->xfrc_applied, 6*m_->nbody);
@@ -1954,15 +1952,15 @@
   }
 
   // update scene
   if (fully_managed_) {
     mjv_updateScene(this->mnew_, this->dnew_,
                     &this->opt, &this->pert, &this->cam, mjCAT_ALL, &this->scn);
   } else {
-    mjv_updateSceneState(this->mnew_, this->dnew_, &this->scnstate_);
+    mjv_updateSceneState(this->mnew_, this->dnew_, &this->opt, &this->scnstate_);
   }
 
   // set window title to model name
   if (this->mnew_->names) {
     char title[200] = "MuJoCo : ";
     mju::strcat_arr(title, this->mnew_->names);
     platform_ui->SetWindowTitle(title);
@@ -2053,72 +2051,70 @@
     // finalize
     this->platform_ui->SwapBuffers();
 
     return;
   }
 
   // update UI sections from last sync
-  if (pending_.full_ui_update) {
-    mjui_update(-1, -1, &this->ui0, &this->uistate, &this->platform_ui->mjr_context());
-    mjui_update(-1, -1, &this->ui1, &this->uistate, &this->platform_ui->mjr_context());
-    pending_.full_ui_update = false;
-    pending_.ui_update_physics = false;
-    pending_.ui_update_joint = false;
-    pending_.ui_update_ctrl = false;
-  } else {
-    if (this->ui0_enable && this->ui0.sect[SECT_WATCH].state) {
-      mjui_update(SECT_WATCH, -1, &this->ui0, &this->uistate, &this->platform_ui->mjr_context());
-    }
+  if (this->ui0_enable && this->ui0.sect[SECT_WATCH].state) {
+    mjui_update(SECT_WATCH, -1, &this->ui0, &this->uistate, &this->platform_ui->mjr_context());
+  }
 
-    if (pending_.ui_update_physics) {
-      if (this->ui0_enable && this->ui0.sect[SECT_PHYSICS].state) {
-        mjui_update(SECT_PHYSICS, -1, &this->ui0, &this->uistate, &this->platform_ui->mjr_context());
-      }
-      pending_.ui_update_physics = false;
+  if (pending_.ui_update_physics) {
+    if (this->ui0_enable && this->ui0.sect[SECT_PHYSICS].state) {
+      mjui_update(SECT_PHYSICS, -1, &this->ui0, &this->uistate, &this->platform_ui->mjr_context());
     }
+    pending_.ui_update_physics = false;
+  }
 
-    if (!fully_managed_) {
-      if (this->ui0_enable && this->ui0.sect[SECT_RENDERING].state &&
-          (cam_prev_.type != cam.type ||
-           cam_prev_.fixedcamid != cam.fixedcamid ||
-           cam_prev_.trackbodyid != cam.trackbodyid ||
-           opt_prev_.label != opt.label || opt_prev_.frame != opt.frame ||
-           Differ(opt_prev_.flags, opt.flags))) {
-        mjui_update(SECT_RENDERING, -1, &this->ui0, &this->uistate,
-                    &this->platform_ui->mjr_context());
-      }
+  if (!fully_managed_) {
+    if (this->ui0_enable && this->ui0.sect[SECT_RENDERING].state &&
+        (cam_prev_.type != cam.type ||
+         cam_prev_.fixedcamid != cam.fixedcamid ||
+         cam_prev_.trackbodyid != cam.trackbodyid ||
+         opt_prev_.label != opt.label || opt_prev_.frame != opt.frame ||
+         IsDifferent(opt_prev_.flags, opt.flags))) {
+      pending_.ui_update_rendering = true;
+    }
+
+    if (this->ui0_enable && this->ui0.sect[SECT_RENDERING].state &&
+        (IsDifferent(opt_prev_.geomgroup, opt.geomgroup) ||
+         IsDifferent(opt_prev_.sitegroup, opt.sitegroup) ||
+         IsDifferent(opt_prev_.jointgroup, opt.jointgroup) ||
+         IsDifferent(opt_prev_.tendongroup, opt.tendongroup) ||
+         IsDifferent(opt_prev_.actuatorgroup, opt.actuatorgroup) ||
+         IsDifferent(opt_prev_.skingroup, opt.skingroup))) {
+      mjui_update(SECT_GROUP, -1, &this->ui0, &this->uistate,
+                  &this->platform_ui->mjr_context());
+    }
 
-      if (this->ui0_enable && this->ui0.sect[SECT_RENDERING].state &&
-          (Differ(opt_prev_.geomgroup, opt.geomgroup) ||
-           Differ(opt_prev_.sitegroup, opt.sitegroup) ||
-           Differ(opt_prev_.jointgroup, opt.jointgroup) ||
-           Differ(opt_prev_.tendongroup, opt.tendongroup) ||
-           Differ(opt_prev_.actuatorgroup, opt.actuatorgroup) ||
-           Differ(opt_prev_.skingroup, opt.skingroup))) {
-        mjui_update(SECT_GROUP, -1, &this->ui0, &this->uistate,
-                    &this->platform_ui->mjr_context());
-      }
+    opt_prev_ = opt;
+    cam_prev_ = cam;
+  }
 
-      opt_prev_ = opt;
-      cam_prev_ = cam;
+  if (pending_.ui_update_rendering) {
+    if (this->ui0_enable && this->ui0.sect[SECT_RENDERING].state) {
+      mjui_update(SECT_RENDERING, -1, &this->ui0, &this->uistate,
+                  &this->platform_ui->mjr_context());
     }
+    pending_.ui_update_rendering = false;
+  }
 
-    if (pending_.ui_update_joint) {
-      if (this->ui1_enable && this->ui1.sect[SECT_JOINT].state) {
-        mjui_update(SECT_JOINT, -1, &this->ui1, &this->uistate, &this->platform_ui->mjr_context());
-      }
-      pending_.ui_update_joint = false;
+  if (pending_.ui_update_joint) {
+    if (this->ui1_enable && this->ui1.sect[SECT_JOINT].state) {
+      mjui_update(SECT_JOINT, -1, &this->ui1, &this->uistate, &this->platform_ui->mjr_context());
     }
+    pending_.ui_update_joint = false;
+  }
 
-    if (pending_.ui_update_ctrl) {
-      if (this->ui1_enable && this->ui1.sect[SECT_CONTROL].state) {
-        mjui_update(SECT_CONTROL, -1, &this->ui1, &this->uistate, &this->platform_ui->mjr_context());
-      }
-      pending_.ui_update_ctrl = false;
+  if (pending_.ui_update_ctrl) {
+    if (this->ui1_enable && this->ui1.sect[SECT_CONTROL].state) {
+      mjui_update(SECT_CONTROL, -1, &this->ui1, &this->uistate, &this->platform_ui->mjr_context());
     }
+    pending_.ui_update_ctrl = false;
   }
 
   // render scene
   mjr_render(rect, &this->scn, &this->platform_ui->mjr_context());
 
   // show last loading error
   if (this->load_error[0]) {
@@ -2340,12 +2336,14 @@
       fps_ = frames_ / interval;
       frames_ = 0;
     }
   }
 
   if (fully_managed_){
     mjv_freeScene(&this->scn);
+  } else {
+    mjv_freeSceneState(&scnstate_);
   }
 
   this->exitrequest.store(2);
 }
 }  // namespace mujoco
```

### Comparing `mujoco-2.3.4/mujoco/simulate/simulate.h` & `mujoco-2.3.5/mujoco/simulate/simulate.h`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 #include <atomic>
 #include <chrono>
 #include <condition_variable>
 #include <memory>
 #include <mutex>
 #include <optional>
 #include <ratio>
+#include <string>
 #include <utility>
 #include <vector>
 
 #include <mujoco/mjui.h>
 #include <mujoco/mujoco.h>
 #include "platform_ui_adapter.h"
 
@@ -123,16 +124,16 @@
     bool copy_pose;
     bool load_key;
     bool save_key;
     bool zero_ctrl;
     int newperturb;
     bool select;
     mjuiState select_state;
-    bool full_ui_update;
     bool ui_update_physics;
+    bool ui_update_rendering;
     bool ui_update_joint;
     bool ui_update_ctrl;
   } pending_ = {};
 
   SimulateMutex mtx;
   std::condition_variable_any cond_loadrequest;
```

### Comparing `mujoco-2.3.4/mujoco/simulate.cc` & `mujoco-2.3.5/mujoco/simulate.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/structs.cc` & `mujoco-2.3.5/mujoco/structs.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/structs.h` & `mujoco-2.3.5/mujoco/structs.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/util/CMakeLists.txt` & `mujoco-2.3.5/mujoco/util/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/util/array_traits.h` & `mujoco-2.3.5/mujoco/util/array_traits.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/util/array_traits_test.cc` & `mujoco-2.3.5/mujoco/util/array_traits_test.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/util/crossplatform.h` & `mujoco-2.3.5/mujoco/util/crossplatform.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/util/func_traits.h` & `mujoco-2.3.5/mujoco/util/func_traits.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/util/func_traits_test.cc` & `mujoco-2.3.5/mujoco/util/func_traits_test.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/util/func_wrap.h` & `mujoco-2.3.5/mujoco/util/func_wrap.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/util/func_wrap_test.cc` & `mujoco-2.3.5/mujoco/util/func_wrap_test.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/util/tuple_tools.h` & `mujoco-2.3.5/mujoco/util/tuple_tools.h`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/util/tuple_tools_test.cc` & `mujoco-2.3.5/mujoco/util/tuple_tools_test.cc`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/viewer.py` & `mujoco-2.3.5/mujoco/viewer.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco/viewer_test.py` & `mujoco-2.3.5/mujoco/viewer_test.py`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/mujoco.egg-info/PKG-INFO` & `mujoco-2.3.5/mujoco.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mujoco
-Version: 2.3.4
+Version: 2.3.5
 Summary: MuJoCo Physics Simulator
 Home-page: https://github.com/deepmind/mujoco
 Author: DeepMind
 Author-email: mujoco@deepmind.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `mujoco-2.3.4/mujoco.egg-info/SOURCES.txt` & `mujoco-2.3.5/mujoco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mujoco-2.3.4/setup.py` & `mujoco-2.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 import setuptools
 from setuptools import find_packages
 from setuptools import setup
 from setuptools.command import build_ext
 from setuptools.command import install_scripts
 
-__version__ = '2.3.4'
+__version__ = '2.3.5'
 
 MUJOCO_CMAKE = 'MUJOCO_CMAKE'
 MUJOCO_CMAKE_ARGS = 'MUJOCO_CMAKE_ARGS'
 MUJOCO_PATH = 'MUJOCO_PATH'
 MUJOCO_PLUGIN_PATH = 'MUJOCO_PLUGIN_PATH'
 
 EXT_PREFIX = 'mujoco.'
```

