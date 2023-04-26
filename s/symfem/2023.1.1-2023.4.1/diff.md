# Comparing `tmp/symfem-2023.1.1.tar.gz` & `tmp/symfem-2023.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symfem-2023.1.1.tar", last modified: Wed Jan  4 09:18:57 2023, max compression
+gzip compressed data, was "symfem-2023.4.1.tar", last modified: Wed Apr 26 17:07:49 2023, max compression
```

## Comparing `symfem-2023.1.1.tar` & `symfem-2023.4.1.tar`

### file list

```diff
@@ -1,101 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 09:18:57.928435 symfem-2023.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-01-04 09:18:52.000000 symfem-2023.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13311 2023-01-04 09:18:57.928435 symfem-2023.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12893 2023-01-04 09:18:57.000000 symfem-2023.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-01-04 09:18:57.928435 symfem-2023.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-01-04 09:18:52.000000 symfem-2023.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 09:18:57.920435 symfem-2023.1.1/symfem/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/basis_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/create.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 09:18:57.924435 symfem-2023.1.1/symfem/elements/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/_guzman_neilan_tetrahedron.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/_guzman_neilan_triangle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/abf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/ac.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/argyris.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/aw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/bddm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/bdfm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/bdm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/bell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/bernardi_raugel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/bernstein.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/bfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/bubble.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/conforming_crouzeix_raviart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/crouzeix_raviart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/direct_serendipity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/dpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12904 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/dual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/fortin_soulie.py
--rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/guzman_neilan.py
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/hct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/hermite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/hhj.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/huang_zhang.py
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/kmv.py
--rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/lagrange.py
--rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/lagrange_prism.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/lagrange_pyramid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/morley.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/morley_wang_xu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/mtw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/nedelec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/nedelec_prism.py
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/p1_iso_p2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/q.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/rannacher_turek.py
--rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/regge.py
--rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/rhct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/rt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/serendipity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/taylor.py
--rw-r--r--   0 runner    (1001) docker     (123)    14666 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/tnt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/transition.py
--rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/trimmed_serendipity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/elements/wu_xu.py
--rw-r--r--   0 runner    (1001) docker     (123)    33501 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/finite_element.py
--rw-r--r--   0 runner    (1001) docker     (123)    57827 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/functionals.py
--rw-r--r--   0 runner    (1001) docker     (123)    54369 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/moments.py
--rw-r--r--   0 runner    (1001) docker     (123)    19862 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/piecewise_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    33258 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    42378 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/polynomials.py
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/quadrature.py
--rw-r--r--   0 runner    (1001) docker     (123)    72868 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/references.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/symbols.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-01-04 09:18:52.000000 symfem-2023.1.1/symfem/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 09:18:57.920435 symfem-2023.1.1/symfem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13311 2023-01-04 09:18:57.000000 symfem-2023.1.1/symfem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-01-04 09:18:57.000000 symfem-2023.1.1/symfem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-04 09:18:57.000000 symfem-2023.1.1/symfem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-01-04 09:18:57.000000 symfem-2023.1.1/symfem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-04 09:18:57.000000 symfem-2023.1.1/symfem.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 09:18:57.924435 symfem-2023.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-04 09:18:52.000000 symfem-2023.1.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-01-04 09:18:52.000000 symfem-2023.1.1/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-01-04 09:18:52.000000 symfem-2023.1.1/test/test_against_basix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-01-04 09:18:52.000000 symfem-2023.1.1/test/test_against_computed_by_hand.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-01-04 09:18:52.000000 symfem-2023.1.1/test/test_arnold_winther.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-01-04 09:18:52.000000 symfem-2023.1.1/test/test_bernstein.py
--rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-01-04 09:18:52.000000 symfem-2023.1.1/test/test_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-01-04 09:18:52.000000 symfem-2023.1.1/test/test_dof_descriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-01-04 09:18:52.000000 symfem-2023.1.1/test/test_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-01-04 09:18:52.000000 symfem-2023.1.1/test/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-01-04 09:18:52.000000 symfem-2023.1.1/test/test_guzman_neilan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-01-04 09:18:52.000000 symfem-2023.1.1/test/test_hct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-01-04 09:18:52.000000 symfem-2023.1.1/test/test_nedelec.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-01-04 09:18:52.000000 symfem-2023.1.1/test/test_p1_iso_p2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-01-04 09:18:52.000000 symfem-2023.1.1/test/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-01-04 09:18:52.000000 symfem-2023.1.1/test/test_polynomials.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-01-04 09:18:52.000000 symfem-2023.1.1/test/test_quadrature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-01-04 09:18:52.000000 symfem-2023.1.1/test/test_references.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-01-04 09:18:52.000000 symfem-2023.1.1/test/test_reorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-01-04 09:18:52.000000 symfem-2023.1.1/test/test_stiffness_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-01-04 09:18:52.000000 symfem-2023.1.1/test/test_tensor_product.py
--rw-r--r--   0 runner    (1001) docker     (123)     9479 2023-01-04 09:18:52.000000 symfem-2023.1.1/test/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:49.263639 symfem-2023.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-26 17:07:26.000000 symfem-2023.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13871 2023-04-26 17:07:49.263639 symfem-2023.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13453 2023-04-26 17:07:49.000000 symfem-2023.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-26 17:07:49.267639 symfem-2023.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-26 17:07:26.000000 symfem-2023.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:49.243639 symfem-2023.4.1/symfem/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10850 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/basis_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/create.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:49.259639 symfem-2023.4.1/symfem/elements/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/_guzman_neilan_tetrahedron.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/_guzman_neilan_triangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/abf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/ac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/argyris.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/aw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/bddm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/bdfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/bdm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/bell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/bernardi_raugel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/bernstein.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/bfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/bubble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/conforming_crouzeix_raviart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/crouzeix_raviart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/direct_serendipity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/dpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/dual.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/enriched_galerkin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/fortin_soulie.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/guzman_neilan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/hct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/hermite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/hhj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/huang_zhang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/kmv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/lagrange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5003 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/lagrange_prism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/lagrange_pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/morley.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/morley_wang_xu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/mtw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/nedelec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/nedelec_prism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/p1_iso_p2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/q.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/rannacher_turek.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/regge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/rhct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/rt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/serendipity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/taylor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14666 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/tnt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/transition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/trimmed_serendipity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/vector_enriched_galerkin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/elements/wu_xu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38368 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/finite_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57827 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/functionals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55195 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/moments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20147 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/piecewise_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33258 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42389 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/polynomials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/quadrature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77252 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/references.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/symbols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-26 17:07:26.000000 symfem-2023.4.1/symfem/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:49.243639 symfem-2023.4.1/symfem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13871 2023-04-26 17:07:49.000000 symfem-2023.4.1/symfem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-26 17:07:49.000000 symfem-2023.4.1/symfem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 17:07:49.000000 symfem-2023.4.1/symfem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-26 17:07:49.000000 symfem-2023.4.1/symfem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 17:07:49.000000 symfem-2023.4.1/symfem.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:07:49.263639 symfem-2023.4.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7140 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/test_against_basix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/test_against_computed_by_hand.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/test_arnold_winther.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/test_bernstein.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/test_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/test_dof_descriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/test_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/test_guzman_neilan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/test_hct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/test_nedelec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/test_p1_iso_p2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/test_polynomials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/test_quadrature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/test_references.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/test_reorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/test_stiffness_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/test_tensor_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9802 2023-04-26 17:07:26.000000 symfem-2023.4.1/test/utils.py
```

### Comparing `symfem-2023.1.1/LICENSE` & `symfem-2023.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/PKG-INFO` & `symfem-2023.4.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symfem
-Version: 2023.1.1
+Version: 2023.4.1
 Summary: a symbolic finite element definition library
 Home-page: https://github.com/mscroggs/symfem
 Author: Matthew Scroggs
 Author-email: symfem@mscroggs.co.uk
 Maintainer-email: symfem@mscroggs.co.uk
 License: MIT
 Description-Content-Type: text/markdown
@@ -156,14 +156,15 @@
 
 ![The numbering of a reference interval](https://raw.githubusercontent.com/mscroggs/symfem/main/img/interval_numbering.png)
 
 ### List of supported elements
 - Bernstein (alternative names: Bernstein-Bezier)
 - bubble
 - dPc
+- enriched Galerkin (alternative names: EG)
 - Hermite
 - Lagrange (alternative names: P)
 - Morley-Wang-Xu (alternative names: MWX)
 - serendipity (alternative names: S)
 - Taylor (alternative names: discontinuous Taylor)
 - vector Lagrange (alternative names: vP)
 - Wu-Xu
@@ -182,14 +183,16 @@
 - Brezzi-Douglas-Fortin-Marini (alternative names: BDFM)
 - Brezzi-Douglas-Marini (alternative names: BDM, N2div)
 - bubble
 - bubble enriched Lagrange
 - bubble enriched vector Lagrange
 - conforming Crouzeix-Raviart (alternative names: conforming CR)
 - Crouzeix-Raviart (alternative names: CR, Crouzeix-Falk, CF)
+- enriched Galerkin (alternative names: EG)
+- enriched vector Galerkin (alternative names: locking-free enriched Galerkin, LFEG)
 - Fortin-Soulie (alternative names: FS)
 - Guzman-Neilan
 - Hellan-Herrmann-Johnson (alternative names: HHJ)
 - Hermite
 - Hsieh-Clough-Tocher (alternative names: Clough-Tocher, HCT, CT)
 - Kong-Mulder-Veldhuizen (alternative names: KMV)
 - Lagrange (alternative names: P)
@@ -219,14 +222,16 @@
 - Arbogast-Correa (alternative names: AC, AC full, Arbogast-Correa full)
 - Arnold-Boffi-Falk (alternative names: ABF)
 - Bogner-Fox-Schmit (alternative names: BFS)
 - Brezzi-Douglas-Fortin-Marini (alternative names: BDFM)
 - bubble
 - direct serendipity
 - dPc
+- enriched Galerkin (alternative names: EG)
+- enriched vector Galerkin (alternative names: locking-free enriched Galerkin, LFEG)
 - Huang-Zhang (alternative names: HZ)
 - NCE (alternative names: RTCE, Qcurl, Nedelec, Ncurl)
 - NCF (alternative names: RTCF, Qdiv)
 - P1-iso-P2 (alternative names: P2-iso-P1, iso-P2 P1)
 - Q (alternative names: Lagrange, P)
 - Rannacher-Turek
 - Regge
@@ -249,14 +254,16 @@
 ### List of supported elements
 - Bernardi-Raugel
 - Bernstein (alternative names: Bernstein-Bezier)
 - Brezzi-Douglas-Fortin-Marini (alternative names: BDFM)
 - Brezzi-Douglas-Marini (alternative names: BDM, N2div)
 - bubble
 - Crouzeix-Raviart (alternative names: CR, Crouzeix-Falk, CF)
+- enriched Galerkin (alternative names: EG)
+- enriched vector Galerkin (alternative names: locking-free enriched Galerkin, LFEG)
 - Guzman-Neilan
 - Hermite
 - Kong-Mulder-Veldhuizen (alternative names: KMV)
 - Lagrange (alternative names: P)
 - Mardal-Tai-Winther (alternative names: MTW)
 - matrix Lagrange
 - Morley-Wang-Xu (alternative names: MWX)
@@ -276,14 +283,16 @@
 ![The numbering of a reference hexahedron](https://raw.githubusercontent.com/mscroggs/symfem/main/img/hexahedron_numbering.png)
 
 ### List of supported elements
 - Brezzi-Douglas-Duran-Fortin (alternative names: BDDF)
 - Brezzi-Douglas-Fortin-Marini (alternative names: BDFM)
 - bubble
 - dPc
+- enriched Galerkin (alternative names: EG)
+- enriched vector Galerkin (alternative names: locking-free enriched Galerkin, LFEG)
 - NCE (alternative names: RTCE, Qcurl, Nedelec, Ncurl)
 - NCF (alternative names: RTCF, Qdiv)
 - Q (alternative names: Lagrange, P)
 - Rannacher-Turek
 - Regge
 - serendipity (alternative names: S)
 - serendipity Hcurl (alternative names: Scurl, BDMCE, AAE)
```

### Comparing `symfem-2023.1.1/README.md` & `symfem-2023.4.1/symfem.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: symfem
+Version: 2023.4.1
+Summary: a symbolic finite element definition library
+Home-page: https://github.com/mscroggs/symfem
+Author: Matthew Scroggs
+Author-email: symfem@mscroggs.co.uk
+Maintainer-email: symfem@mscroggs.co.uk
+License: MIT
+Description-Content-Type: text/markdown
+Provides-Extra: style
+Provides-Extra: docs
+Provides-Extra: optional
+Provides-Extra: test
+License-File: LICENSE
+
 ![Symfem](https://raw.githubusercontent.com/mscroggs/symfem/main/logo/logo.png)
 
 |  | Badges |
 | --- | :---: |
 | Documentation | [![Documentation status](https://readthedocs.org/projects/symfem/badge/?version=latest)](https://symfem.readthedocs.io/en/latest/?badge=latest) |
 | Testing & coverage | [![Style checks](https://github.com/mscroggs/symfem/actions/workflows/style-checks.yml/badge.svg)](https://github.com/mscroggs/symfem/actions) [![Run tests](https://github.com/mscroggs/symfem/actions/workflows/run-tests.yml/badge.svg)](https://github.com/mscroggs/symfem/actions) [![Coverage Status](https://coveralls.io/repos/github/mscroggs/symfem/badge.svg?branch=main)](https://coveralls.io/github/mscroggs/symfem?branch=main) |
 | Packages | [![PyPI](https://img.shields.io/pypi/v/symfem?color=blue&label=PyPI&logo=pypi&logoColor=white)](https://pypi.org/project/symfem/) [![conda](https://anaconda.org/conda-forge/symfem/badges/version.svg)](https://anaconda.org/conda-forge/symfem) |
@@ -140,14 +156,15 @@
 
 ![The numbering of a reference interval](https://raw.githubusercontent.com/mscroggs/symfem/main/img/interval_numbering.png)
 
 ### List of supported elements
 - Bernstein (alternative names: Bernstein-Bezier)
 - bubble
 - dPc
+- enriched Galerkin (alternative names: EG)
 - Hermite
 - Lagrange (alternative names: P)
 - Morley-Wang-Xu (alternative names: MWX)
 - serendipity (alternative names: S)
 - Taylor (alternative names: discontinuous Taylor)
 - vector Lagrange (alternative names: vP)
 - Wu-Xu
@@ -166,14 +183,16 @@
 - Brezzi-Douglas-Fortin-Marini (alternative names: BDFM)
 - Brezzi-Douglas-Marini (alternative names: BDM, N2div)
 - bubble
 - bubble enriched Lagrange
 - bubble enriched vector Lagrange
 - conforming Crouzeix-Raviart (alternative names: conforming CR)
 - Crouzeix-Raviart (alternative names: CR, Crouzeix-Falk, CF)
+- enriched Galerkin (alternative names: EG)
+- enriched vector Galerkin (alternative names: locking-free enriched Galerkin, LFEG)
 - Fortin-Soulie (alternative names: FS)
 - Guzman-Neilan
 - Hellan-Herrmann-Johnson (alternative names: HHJ)
 - Hermite
 - Hsieh-Clough-Tocher (alternative names: Clough-Tocher, HCT, CT)
 - Kong-Mulder-Veldhuizen (alternative names: KMV)
 - Lagrange (alternative names: P)
@@ -203,14 +222,16 @@
 - Arbogast-Correa (alternative names: AC, AC full, Arbogast-Correa full)
 - Arnold-Boffi-Falk (alternative names: ABF)
 - Bogner-Fox-Schmit (alternative names: BFS)
 - Brezzi-Douglas-Fortin-Marini (alternative names: BDFM)
 - bubble
 - direct serendipity
 - dPc
+- enriched Galerkin (alternative names: EG)
+- enriched vector Galerkin (alternative names: locking-free enriched Galerkin, LFEG)
 - Huang-Zhang (alternative names: HZ)
 - NCE (alternative names: RTCE, Qcurl, Nedelec, Ncurl)
 - NCF (alternative names: RTCF, Qdiv)
 - P1-iso-P2 (alternative names: P2-iso-P1, iso-P2 P1)
 - Q (alternative names: Lagrange, P)
 - Rannacher-Turek
 - Regge
@@ -233,14 +254,16 @@
 ### List of supported elements
 - Bernardi-Raugel
 - Bernstein (alternative names: Bernstein-Bezier)
 - Brezzi-Douglas-Fortin-Marini (alternative names: BDFM)
 - Brezzi-Douglas-Marini (alternative names: BDM, N2div)
 - bubble
 - Crouzeix-Raviart (alternative names: CR, Crouzeix-Falk, CF)
+- enriched Galerkin (alternative names: EG)
+- enriched vector Galerkin (alternative names: locking-free enriched Galerkin, LFEG)
 - Guzman-Neilan
 - Hermite
 - Kong-Mulder-Veldhuizen (alternative names: KMV)
 - Lagrange (alternative names: P)
 - Mardal-Tai-Winther (alternative names: MTW)
 - matrix Lagrange
 - Morley-Wang-Xu (alternative names: MWX)
@@ -260,14 +283,16 @@
 ![The numbering of a reference hexahedron](https://raw.githubusercontent.com/mscroggs/symfem/main/img/hexahedron_numbering.png)
 
 ### List of supported elements
 - Brezzi-Douglas-Duran-Fortin (alternative names: BDDF)
 - Brezzi-Douglas-Fortin-Marini (alternative names: BDFM)
 - bubble
 - dPc
+- enriched Galerkin (alternative names: EG)
+- enriched vector Galerkin (alternative names: locking-free enriched Galerkin, LFEG)
 - NCE (alternative names: RTCE, Qcurl, Nedelec, Ncurl)
 - NCF (alternative names: RTCF, Qdiv)
 - Q (alternative names: Lagrange, P)
 - Rannacher-Turek
 - Regge
 - serendipity (alternative names: S)
 - serendipity Hcurl (alternative names: Scurl, BDMCE, AAE)
```

### Comparing `symfem-2023.1.1/setup.py` & `symfem-2023.4.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,34 +15,34 @@
         "(https://raw.githubusercontent.com/mscroggs/symfem/main/logo/logo.png)"
     ).replace(
         "(img/",
         "(https://raw.githubusercontent.com/mscroggs/symfem/main/img/")
 with open(os.path.join(os.path.dirname(os.path.realpath(__file__)), "README.md"), "w") as f:
     f.write(long_description)
 
-data_files = ["LICENSE", "README.md",
+data_files = [("", ["LICENSE", "README.md"]),
               ("test", ["test/__init__.py", "test/utils.py", "test/conftest.py"])]
 
 if __name__ == "__main__":
     setuptools.setup(
         name="symfem",
         description="a symbolic finite element definition library",
         long_description=long_description,
         long_description_content_type="text/markdown",
-        version="2023.1.1",
+        version="2023.4.1",
         author="Matthew Scroggs",
         license="MIT",
         author_email="symfem@mscroggs.co.uk",
         maintainer_email="symfem@mscroggs.co.uk",
         url="https://github.com/mscroggs/symfem",
         packages=["symfem", "symfem.elements"],
         package_data={"symfem": ["py.typed"]},
         include_package_data=True,
         data_files=data_files,
         install_requires=["sympy>=1.10"],
         extras_require={
             "style": ["flake8", "pydocstyle", "mypy", "isort"],
-            "docs": ["sphinx==5.0.2", "sphinx-autoapi"],
-            "optional": ["CairoSVG"],
+            "docs": ["sphinx", "sphinx-autoapi"],
+            "optional": ["CairoSVG>=2.6.0"],
             "test": ["pytest", "symfem[optional]", "numpy"],
         }
     )
```

### Comparing `symfem-2023.1.1/symfem/basis_functions.py` & `symfem-2023.4.1/symfem/basis_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from abc import abstractmethod
 
 import sympy
 
 from .functions import AnyFunction, FunctionInput, ScalarFunction, SympyFormat, ValuesToSubstitute
 from .geometry import PointType
 from .references import Reference
-from .symbols import AxisVariables, AxisVariablesNotSingle, t
+from .symbols import AxisVariables, AxisVariablesNotSingle, t, x
 
 
 class BasisFunction(AnyFunction):
     """A basis function of a finite element.
 
     This basis function can be used before the element's basis functions have been computed. When
     the explicit basis function is needed, only then will it be computed.
@@ -278,25 +278,29 @@
         """Compute the norm of the function.
 
         Returns:
             The norm
         """
         raise self.get_function().norm()
 
-    def integral(self, domain: Reference, vars: AxisVariablesNotSingle = t) -> AnyFunction:
+    def integral(
+        self, domain: Reference, vars: AxisVariablesNotSingle = x,
+        dummy_vars: AxisVariablesNotSingle = t
+    ) -> ScalarFunction:
         """Compute the integral of the function.
 
         Args:
-            domain: The domain to integrate over
-            vars: The variables to integrate over
+            domain: The domain of the integral
+            vars: The variables to integrate with respect to
+            dummy_vars: The dummy variables to use inside the integral
 
         Returns:
             The integral
         """
-        return self.get_function().integral(domain, vars)
+        return self.get_function().integral(domain, vars, dummy_vars)
 
     def subs(self, vars: AxisVariables, values: ValuesToSubstitute) -> BasisFunction:
         """Substitute values into the function.
 
         Args:
             vars: The variable(s) to substitute
             values: The value(s) to substitute
```

### Comparing `symfem-2023.1.1/symfem/create.py` & `symfem-2023.4.1/symfem/create.py`

 * *Files 7% similar despite different names*

```diff
@@ -162,15 +162,17 @@
                       TNT, tiniest tensor,
                       TNTcurl, tiniest tensor Hcurl,
                       TNTdiv, tiniest tensor Hdiv,
                       Arnold-Boffi-Falk, ABF,
                       Arbogast-Correa, AC, AC full, Arbogast-Correa full,
                       Rannacher-Turek,
                       P1-iso-P2, P2-iso-P1, iso-P2 P1,
-                      Huang-Zhang, HZ
+                      Huang-Zhang, HZ,
+                      enriched Galerkin, EG,
+                      enriched vector Galerkin, locking-free enriched Galerkin, LFEG
         order: The order of the element.
     """
     reference = create_reference(cell_type)
 
     if element_type in _elementmap:
         if reference.name not in _elementmap[element_type]:
             raise ValueError(f"{element_type} element cannot be created on a {reference.name}.")
```

### Comparing `symfem-2023.1.1/symfem/elements/_guzman_neilan_tetrahedron.py` & `symfem-2023.4.1/symfem/elements/_guzman_neilan_tetrahedron.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/_guzman_neilan_triangle.py` & `symfem-2023.4.1/symfem/elements/_guzman_neilan_triangle.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/abf.py` & `symfem-2023.4.1/symfem/elements/abf.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/ac.py` & `symfem-2023.4.1/symfem/elements/ac.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/argyris.py` & `symfem-2023.4.1/symfem/elements/argyris.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/aw.py` & `symfem-2023.4.1/symfem/elements/aw.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/bddm.py` & `symfem-2023.4.1/symfem/elements/bddm.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/bdfm.py` & `symfem-2023.4.1/symfem/elements/bdfm.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/bdm.py` & `symfem-2023.4.1/symfem/elements/bdm.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/bell.py` & `symfem-2023.4.1/symfem/elements/bell.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/bernardi_raugel.py` & `symfem-2023.4.1/symfem/elements/bernardi_raugel.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/bernstein.py` & `symfem-2023.4.1/symfem/elements/bernstein.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/bfs.py` & `symfem-2023.4.1/symfem/elements/bfs.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/bubble.py` & `symfem-2023.4.1/symfem/elements/bubble.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/conforming_crouzeix_raviart.py` & `symfem-2023.4.1/symfem/elements/conforming_crouzeix_raviart.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/crouzeix_raviart.py` & `symfem-2023.4.1/symfem/elements/crouzeix_raviart.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/direct_serendipity.py` & `symfem-2023.4.1/symfem/elements/direct_serendipity.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/dpc.py` & `symfem-2023.4.1/symfem/elements/dpc.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/dual.py` & `symfem-2023.4.1/symfem/elements/dual.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 import sympy
 
 from ..finite_element import FiniteElement
 from ..functions import AnyFunction, FunctionInput, VectorFunction
 from ..geometry import PointType, SetOfPoints, SetOfPointsInput
 from ..piecewise_functions import PiecewiseFunction
-from ..plotting import Picture, colors
 from ..references import DualPolygon
 
 
 class DualCiarletElement(FiniteElement):
     """Abstract barycentric finite element."""
 
     def __init__(
@@ -43,16 +42,16 @@
             dof_directions: The direction that each basis function is associated with
         """
         self.dual_coefficients = dual_coefficients
         self.fine_space = fine_space
         super().__init__(reference, order, len(dual_coefficients), domain_dim, range_dim,
                          range_shape=range_shape)
         self._basis_functions: typing.Union[typing.List[AnyFunction], None] = None
-        self.dof_entities = dof_entities
-        self.dof_directions = dof_directions
+        self._dof_entities = dof_entities
+        self._dof_directions = dof_directions
 
     def get_polynomial_basis(
         self, reshape: bool = True
     ) -> typing.List[AnyFunction]:
         """Get the symbolic polynomial basis for the element.
 
         Returns:
@@ -106,15 +105,15 @@
                             for a, b in zip(coeffs, sub_basis):
                                 assert isinstance(b, VectorFunction)
                                 sf_item += a * b[i]
                             sf_list.append(sf_item)
                         sub_fun = tuple(sf_list)
                     pieces[(v0, v1, v2)] = sub_fun
                 bfs.append(PiecewiseFunction(pieces, 2))
-            assert len(bfs) == len(self.dof_entities)
+            assert len(bfs) == len(self._dof_entities)
             self._basis_functions = bfs
 
         assert self._basis_functions is not None
         return self._basis_functions
 
     def entity_dofs(self, entity_dim: int, entity_number: int) -> typing.List[int]:
         """Get the numbers of the DOFs associated with the given entity.
@@ -123,19 +122,59 @@
             entity_dim: The dimension of the entity
             entity_number: The number of the entity
 
         Returns:
             The numbers of the DOFs associated with the entity
         """
         out = []
-        for i, e in enumerate(self.dof_entities):
+        for i, e in enumerate(self._dof_entities):
             if e == (entity_dim, entity_number):
                 out.append(i)
         return out
 
+    def dof_plot_positions(self) -> typing.List[PointType]:
+        """Get the points to plot each DOF at on a DOF diagram.
+
+        Returns:
+            The DOF positions
+        """
+        positions = []
+        for d, (dim, e_n) in enumerate(self._dof_entities):
+            if dim == 0:
+                positions.append(self.reference.vertices[e_n])
+            elif dim == 1:
+                positions.append(tuple((a + b) / 2 for a, b in zip(
+                    self.reference.vertices[self.reference.edges[e_n][0]],
+                    self.reference.vertices[self.reference.edges[e_n][1]],
+                )))
+            elif dim == 2:
+                positions.append(self.reference.midpoint())
+            else:
+                raise ValueError("Unsupported tdim")
+
+        return positions
+
+    def dof_directions(self) -> typing.List[typing.Union[PointType, None]]:
+        """Get the direction associated with each DOF.
+
+        Returns:
+            The DOF directions
+        """
+        if self._dof_directions is None:
+            return [None for d in self._dof_entities]
+        return list(self._dof_directions)
+
+    def dof_entities(self) -> typing.List[typing.Tuple[int, int]]:
+        """Get the entities that each DOF is associated with.
+
+        Returns:
+            The entities
+        """
+        return self._dof_entities
+
     def map_to_cell(
         self, vertices_in: SetOfPointsInput, basis:
         typing.Optional[typing.List[AnyFunction]] = None,
         forward_map: typing.Optional[PointType] = None,
         inverse_map: typing.Optional[PointType] = None
     ) -> typing.List[AnyFunction]:
         """Map the basis onto a cell using the appropriate mapping for the element.
@@ -147,55 +186,14 @@
             inverse_map: The map to the reference from the cell
 
         Returns:
             The basis functions mapped to the cell
         """
         raise NotImplementedError()
 
-    def plot_dof_diagram(
-        self, filename: typing.Union[str, typing.List[str]],
-        plot_options: typing.Dict[str, typing.Any] = {}, **kwargs: typing.Any
-    ):
-        """Plot a diagram showing the DOFs of the element.
-
-        Args:
-            filename: The file name
-            plot_options: Options for the plot
-            kwargs: Keyword arguments
-        """
-        img = Picture(**kwargs)
-
-        for entities in self.reference.z_ordered_entities():
-            for dim, e_n in entities:
-                if dim == 1:
-                    pts = tuple(self.reference.vertices[i] for i in self.reference.edges[e_n])
-                    img.add_line(pts[0], pts[1], colors.BLACK)
-
-            for dim, e_n in entities:
-                for d in self.entity_dofs(dim, e_n):
-                    if dim == 0:
-                        point = self.reference.vertices[e_n]
-                    elif dim == 1:
-                        point = tuple((a + b) / 2 for a, b in zip(
-                            self.reference.vertices[self.reference.edges[e_n][0]],
-                            self.reference.vertices[self.reference.edges[e_n][1]],
-                        ))
-                    elif dim == 2:
-                        point = self.reference.midpoint()
-                    else:
-                        raise ValueError("Unsupported tdim")
-
-                    if self.dof_directions is not None:
-                        direction = self.dof_directions[d]
-                        img.add_dof_arrow(point, direction, d, colors.entity(dim), False)
-                    else:
-                        img.add_dof_marker(point, d, colors.entity(dim))
-
-        img.save(filename, plot_options=plot_options)
-
 
 class Dual(DualCiarletElement):
     """Barycentric dual finite element."""
 
     def __init__(self, reference: DualPolygon, order: int):
         """Create the element.
 
@@ -215,25 +213,22 @@
             dual_coefficients = [
                 [[sympy.Rational(1, reference.number_of_triangles), 0, 0]
                  for i in range(2 * reference.number_of_triangles)]
                 for j in range(reference.number_of_triangles)
             ]
 
             for j in range(reference.number_of_triangles):
-                dual_coefficients[j][2 * j][2] = 1
-                dual_coefficients[j][2 * j + 1][1] = 1
-                dual_coefficients[j][2 * j - 1][2] = sympy.Rational(1, 2)
-                dual_coefficients[j][2 * j][1] = sympy.Rational(1, 2)
-                dual_coefficients[j][2 * j + 1][2] = sympy.Rational(1, 2)
-                if j + 1 == reference.number_of_triangles:
-                    dual_coefficients[j][0][1] = sympy.Rational(1, 2)
-                else:
-                    dual_coefficients[j][2 * j + 2][1] = sympy.Rational(1, 2)
+                dual_coefficients[j][2 * j - 1][2] = 1
+                dual_coefficients[j][2 * j][1] = 1
+                dual_coefficients[j][2 * j - 2][2] = sympy.Rational(1, 2)
+                dual_coefficients[j][2 * j - 1][1] = sympy.Rational(1, 2)
+                dual_coefficients[j][2 * j][2] = sympy.Rational(1, 2)
+                dual_coefficients[j][2 * j + 1][1] = sympy.Rational(1, 2)
 
-            dof_entities = [(1, i) for i in range(1, len(reference.vertices), 2)]
+            dof_entities = [(0, i) for i in range(0, len(reference.vertices), 2)]
 
             fine_space = "Lagrange"
 
         super().__init__(
             dual_coefficients, fine_space, reference, order, dof_entities, reference.tdim, 1
         )
```

### Comparing `symfem-2023.1.1/symfem/elements/fortin_soulie.py` & `symfem-2023.4.1/symfem/elements/fortin_soulie.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/guzman_neilan.py` & `symfem-2023.4.1/symfem/elements/guzman_neilan.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/hct.py` & `symfem-2023.4.1/symfem/elements/hct.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/hermite.py` & `symfem-2023.4.1/symfem/elements/hermite.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/hhj.py` & `symfem-2023.4.1/symfem/elements/hhj.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/huang_zhang.py` & `symfem-2023.4.1/symfem/elements/huang_zhang.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/kmv.py` & `symfem-2023.4.1/symfem/elements/kmv.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/lagrange.py` & `symfem-2023.4.1/symfem/elements/lagrange.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/lagrange_prism.py` & `symfem-2023.4.1/symfem/elements/lagrange_prism.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/lagrange_pyramid.py` & `symfem-2023.4.1/symfem/elements/lagrange_pyramid.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/morley.py` & `symfem-2023.4.1/symfem/elements/morley.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/morley_wang_xu.py` & `symfem-2023.4.1/symfem/elements/morley_wang_xu.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/mtw.py` & `symfem-2023.4.1/symfem/elements/mtw.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/nedelec.py` & `symfem-2023.4.1/symfem/elements/nedelec.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/nedelec_prism.py` & `symfem-2023.4.1/symfem/elements/nedelec_prism.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/p1_iso_p2.py` & `symfem-2023.4.1/symfem/elements/p1_iso_p2.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/q.py` & `symfem-2023.4.1/symfem/elements/q.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/rannacher_turek.py` & `symfem-2023.4.1/symfem/elements/rannacher_turek.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/regge.py` & `symfem-2023.4.1/symfem/elements/regge.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/rhct.py` & `symfem-2023.4.1/symfem/elements/rhct.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/rt.py` & `symfem-2023.4.1/symfem/elements/rt.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/serendipity.py` & `symfem-2023.4.1/symfem/elements/serendipity.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/taylor.py` & `symfem-2023.4.1/symfem/elements/taylor.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/tnt.py` & `symfem-2023.4.1/symfem/elements/tnt.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/transition.py` & `symfem-2023.4.1/symfem/elements/transition.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/trimmed_serendipity.py` & `symfem-2023.4.1/symfem/elements/trimmed_serendipity.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/elements/wu_xu.py` & `symfem-2023.4.1/symfem/elements/wu_xu.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/finite_element.py` & `symfem-2023.4.1/symfem/finite_element.py`

 * *Files 17% similar despite different names*

```diff
@@ -62,26 +62,87 @@
         self.domain_dim = domain_dim
         self.range_dim = range_dim
         self.range_shape = range_shape
         self._float_basis_functions = None
         self._value_scale = None
 
     @abstractmethod
+    def dof_plot_positions(self) -> typing.List[PointType]:
+        """Get the points to plot each DOF at on a DOF diagram.
+
+        Returns:
+            The DOF positions
+        """
+        pass
+
+    @abstractmethod
+    def dof_directions(self) -> typing.List[typing.Union[PointType, None]]:
+        """Get the direction associated with each DOF.
+
+        Returns:
+            The DOF directions
+        """
+        pass
+
+    @abstractmethod
+    def dof_entities(self) -> typing.List[typing.Tuple[int, int]]:
+        """Get the entities that each DOF is associated with.
+
+        Returns:
+            The entities
+        """
+        pass
+
     def plot_dof_diagram(
         self, filename: typing.Union[str, typing.List[str]],
         plot_options: typing.Dict[str, typing.Any] = {}, **kwargs: typing.Any
     ):
         """Plot a diagram showing the DOFs of the element.
 
         Args:
             filename: The file name
             plot_options: Options for the plot
             kwargs: Keyword arguments
         """
-        pass
+        img = Picture(**kwargs)
+
+        dof_positions = self.dof_plot_positions()
+        dof_directions = self.dof_directions()
+        dof_entities = self.dof_entities()
+
+        for entities in self.reference.z_ordered_entities():
+            for dim, e in entities:
+                if dim == 1:
+                    pts = tuple(self.reference.vertices[i] for i in self.reference.edges[e])
+                    img.add_line(pts[0], pts[1], colors.BLACK)
+                if dim == 2:
+                    pts = tuple(self.reference.vertices[i] for i in self.reference.faces[e])
+                    if len(pts) == 4:
+                        pts = (pts[0], pts[1], pts[3], pts[2])
+                    img.add_fill(pts, colors.WHITE, 0.5)
+
+            for dim, e in entities:
+                dofs = [(dof_positions[i], dof_directions[i], dof_entities[i], i)
+                        for i in self.entity_dofs(dim, e)]
+                dofs.sort(key=lambda d: img.z(d[0]))
+                for d in dofs:
+                    direction = d[1]
+                    if direction is not None:
+                        shifted = False
+                        for d2, p in enumerate(dof_positions):
+                            if d != d2 and d[0] == p:
+                                shifted = True
+                                break
+                        img.add_dof_arrow(d[0], direction, d[3],
+                                          colors.entity(d[2][0]), shifted)
+                    else:
+                        img.add_dof_marker(
+                            d[0], d[3], colors.entity(d[2][0]))
+
+        img.save(filename, plot_options=plot_options)
 
     @abstractmethod
     def entity_dofs(self, entity_dim: int, entity_number: int) -> typing.List[int]:
         """Get the numbers of the DOFs associated with the given entity.
 
         Args:
             entity_dim: The dimension of the entity
@@ -163,35 +224,42 @@
             self._float_basis_functions = [b.with_floats() for b in self.get_basis_functions()]
 
         assert self._float_basis_functions is not None
         points = parse_set_of_points_input(points_in)
         return [tuple(b.subs(x, p).as_sympy() for b in self._float_basis_functions) for p in points]
 
     def plot_basis_function(
-        self, n: int, filename: typing.Union[str, typing.List[str]], **kwargs: typing.Any
+        self, n: int, filename: typing.Union[str, typing.List[str]],
+        cell: typing.Optional[Reference] = None, **kwargs: typing.Any
     ):
         """Plot a diagram showing a basis function.
 
         Args:
             n: The basis function number
             filename: The file name
+            cell: The cell to push the basis function to and plot on
             kwargs: Keyword arguments
         """
         if self._value_scale is None:
             max_v = 0.0
             values = self.tabulate_basis_float(self.reference.make_lattice_float(6))
             for row in values:
                 assert isinstance(row, tuple)
                 for i in row:
                     max_v = max(max_v, float(parse_function_input(i).norm()))
             self._value_scale = 1 / sympy.Float(max_v)
 
-        f = self.get_basis_functions()[n]
         assert self._value_scale is not None
-        f.plot(self.reference, filename, None, None, None, n, self._value_scale, **kwargs)
+
+        if cell is None:
+            f = self.get_basis_functions()[n]
+            f.plot(self.reference, filename, None, None, None, n, self._value_scale, **kwargs)
+        else:
+            f = self.map_to_cell(cell.vertices)[n]
+            f.plot(cell, filename, None, None, None, n, self._value_scale, **kwargs)
 
     @abstractmethod
     def map_to_cell(
         self, vertices_in: SetOfPointsInput,
         basis: typing.Optional[typing.List[AnyFunction]] = None,
         forward_map: typing.Optional[PointType] = None,
         inverse_map: typing.Optional[PointType] = None
@@ -422,14 +490,38 @@
             entity_number: The number of the entity
 
         Returns:
             The numbers of the DOFs associated with the entity
         """
         return [i for i, j in enumerate(self.dofs) if j.entity == (entity_dim, entity_number)]
 
+    def dof_plot_positions(self) -> typing.List[PointType]:
+        """Get the points to plot each DOF at on a DOF diagram.
+
+        Returns:
+            The DOF positions
+        """
+        return [d.adjusted_dof_point() for d in self.dofs]
+
+    def dof_directions(self) -> typing.List[typing.Union[PointType, None]]:
+        """Get the direction associated with each DOF.
+
+        Returns:
+            The DOF directions
+        """
+        return [d.dof_direction() for d in self.dofs]
+
+    def dof_entities(self) -> typing.List[typing.Tuple[int, int]]:
+        """Get the entities that each DOF is associated with.
+
+        Returns:
+            The entities
+        """
+        return [d.entity for d in self.dofs]
+
     def get_polynomial_basis(self) -> typing.List[AnyFunction]:
         """Get the symbolic polynomial basis for the element.
 
         Returns:
             The polynomial basis
         """
         return self._basis
@@ -487,23 +579,28 @@
                 self._basis_functions = sfs
 
         assert isinstance(self._basis_functions, list)
 
         return self._basis_functions
 
     def plot_basis_function(
-        self, n: int, filename: typing.Union[str, typing.List[str]], **kwargs: typing.Any
+        self, n: int, filename: typing.Union[str, typing.List[str]],
+        cell: typing.Optional[Reference] = None, **kwargs: typing.Any
     ):
         """Plot a diagram showing a basis function.
 
         Args:
             n: The basis function number
             filename: The file name
+            cell: The cell to push the basis function to and plot on
             kwargs: Keyword arguments
         """
+        if cell is not None:
+            raise NotImplementedError()
+
         if self._value_scale is None:
             values = self.tabulate_basis_float(self.reference.make_lattice_float(6))
             max_v = 0.0
             for row in values:
                 assert isinstance(row, tuple)
                 for i in row:
                     max_v = max(max_v, float(parse_function_input(i).norm()))
@@ -511,64 +608,14 @@
 
         f = self.get_basis_functions()[n]
         d = self.dofs[n]
         assert self._value_scale is not None
         f.plot(self.reference, filename, d.dof_point(), d.dof_direction(), d.entity, n,
                self._value_scale, **kwargs)
 
-    def plot_dof_diagram(
-        self, filename: typing.Union[str, typing.List[str]],
-        plot_options: typing.Dict[str, typing.Any] = {}, **kwargs: typing.Any
-    ):
-        """Plot a diagram showing the DOFs of the element.
-
-        Args:
-            filename: The file name
-            plot_options: Options for the plot
-            kwargs: Keyword arguments
-        """
-        img = Picture(**kwargs)
-
-        dofs_by_subentity: typing.Dict[int, typing.Dict[int, ListOfFunctionals]] = {
-            i: {j: [] for j in range(self.reference.sub_entity_count(i))}
-            for i in range(self.reference.tdim + 1)}
-
-        for d in self.dofs:
-            dofs_by_subentity[d.entity[0]][d.entity[1]].append(d)
-
-        for entities in self.reference.z_ordered_entities():
-            for dim, e in entities:
-                if dim == 1:
-                    pts = tuple(self.reference.vertices[i] for i in self.reference.edges[e])
-                    img.add_line(pts[0], pts[1], colors.BLACK)
-                if dim == 2:
-                    pts = tuple(self.reference.vertices[i] for i in self.reference.faces[e])
-                    if len(pts) == 4:
-                        pts = (pts[0], pts[1], pts[3], pts[2])
-                    img.add_fill(pts, colors.WHITE, 0.5)
-
-            for dim, e in entities:
-                dofs = dofs_by_subentity[dim][e]
-                dofs.sort(key=lambda d: img.z(d.adjusted_dof_point()))
-                for d in dofs:
-                    direction = d.dof_direction()
-                    if direction is not None:
-                        shifted = False
-                        for d2 in self.dofs:
-                            if d != d2 and d.adjusted_dof_point() == d2.adjusted_dof_point():
-                                shifted = True
-                                break
-                        img.add_dof_arrow(d.adjusted_dof_point(), direction, self.dofs.index(d),
-                                          colors.entity(d.entity[0]), shifted)
-                    else:
-                        img.add_dof_marker(
-                            d.adjusted_dof_point(), self.dofs.index(d), colors.entity(d.entity[0]))
-
-        img.save(filename, plot_options=plot_options)
-
     def map_to_cell(
         self, vertices_in: SetOfPointsInput,
         basis: typing.Optional[typing.List[AnyFunction]] = None,
         forward_map: typing.Optional[PointType] = None,
         inverse_map: typing.Optional[PointType] = None
     ) -> typing.List[AnyFunction]:
         """Map the basis onto a cell using the appropriate mapping for the element.
@@ -661,15 +708,15 @@
     _basis_functions: typing.List[AnyFunction]
 
     def __init__(
         self, reference: Reference, order: int, basis_functions: typing.List[FunctionInput],
         basis_entities: typing.List[typing.Tuple[int, int]],
         domain_dim: int, range_dim: int, range_shape: typing.Optional[typing.Tuple[int, ...]] = None
     ):
-        """Create a Ciarlet element.
+        """Create a direct element.
 
         Args:
             reference: The reference cell
             order: The polynomial order
             basis_functions: The basis functions
             basis_entities: The entitiy each basis function is associated with
             domain_dim: The topological dimension of the cell
@@ -689,14 +736,78 @@
             entity_number: The number of the entity
 
         Returns:
             The numbers of the DOFs associated with the entity
         """
         return [i for i, j in enumerate(self._basis_entities) if j == (entity_dim, entity_number)]
 
+    def dof_plot_positions(self) -> typing.List[PointType]:
+        """Get the points to plot each DOF at on a DOF diagram.
+
+        Returns:
+            The DOF positions
+        """
+        positions = []
+        for n, (dim, e_n) in enumerate(self._basis_entities):
+            ed = self.entity_dofs(dim, e_n)
+            entity_n = ed.index(n)
+            dof_count = len(ed)
+            sub_ref = self.reference.sub_entity(dim, e_n)
+            if dim == 0:
+                assert entity_n == 0
+                positions.append(sub_ref.vertices[0])
+            elif dim == 1:
+                positions.append(tuple(
+                    o + sympy.Rational((entity_n + 1) * a, dof_count + 1)
+                    for o, a in zip(sub_ref.origin, *sub_ref.axes)))
+            elif dim == 2:
+                ne = 1
+                while ne * (ne + 1) // 2 < dof_count:
+                    ne += 1
+                i = 0
+                while entity_n >= ne - i:
+                    entity_n -= ne - i
+                    i += 1
+                positions.append(tuple(
+                    o + sympy.Rational((entity_n + 1) * a + (i + 1) * b, ne + 1)
+                    for o, a, b in zip(sub_ref.origin, *sub_ref.axes)))
+            elif dim == 3:
+                ne = 1
+                while ne * (ne + 1) * (ne + 2) // 6 < n:
+                    ne += 1
+                i = 0
+                while entity_n >= (ne - i) * (ne + 1 - i) // 2:
+                    entity_n -= (ne - i) * (ne + 1 - i) // 2
+                    i += 1
+                j = 0
+                while entity_n >= ne - j:
+                    entity_n -= ne - j
+                    j += 1
+                positions.append(tuple(
+                    o + sympy.Rational((entity_n + 1) * a + (j + 1) * b + (i + 1) * c, n + 1)
+                    for o, a, b, c in zip(sub_ref.origin, *sub_ref.axes)))
+
+        return positions
+
+    def dof_directions(self) -> typing.List[typing.Union[PointType, None]]:
+        """Get the direction associated with each DOF.
+
+        Returns:
+            The DOF directions
+        """
+        return [None for d in self._basis_entities]
+
+    def dof_entities(self) -> typing.List[typing.Tuple[int, int]]:
+        """Get the entities that each DOF is associated with.
+
+        Returns:
+            The entities
+        """
+        return self._basis_entities
+
     def get_basis_functions(
         self, use_tensor_factorisation: bool = False
     ) -> typing.List[AnyFunction]:
         """Get the basis functions of the element.
 
         Args:
             use_tensor_factorisation: Should a tensor factorisation be used?
@@ -732,78 +843,14 @@
         """Get the symbolic polynomial basis for the element.
 
         Returns:
             The polynomial basis
         """
         raise NotImplementedError()
 
-    def plot_dof_diagram(
-        self, filename: typing.Union[str, typing.List[str]],
-        plot_options: typing.Dict[str, typing.Any] = {}, **kwargs: typing.Any
-    ):
-        """Plot a diagram showing the DOFs of the element.
-
-        Args:
-            filename: The file name
-            plot_options: Options for the plot
-            kwargs: Keyword arguments
-        """
-        img = Picture(**kwargs)
-
-        dofs_by_subentity: typing.Dict[int, typing.Dict[int, typing.List[int]]] = {
-            i: {j: [] for j in range(self.reference.sub_entity_count(i))}
-            for i in range(self.reference.tdim + 1)}
-
-        for i, e in enumerate(self._basis_entities):
-            dofs_by_subentity[e[0]][e[1]].append(i)
-
-        for entities in self.reference.z_ordered_entities():
-            for dim, e_n in entities:
-                if dim == 1:
-                    pts = tuple(self.reference.vertices[i] for i in self.reference.edges[e_n])
-                    img.add_line(pts[0], pts[1], colors.BLACK)
-                if dim == 2:
-                    pts = tuple(self.reference.vertices[i] for i in self.reference.faces[e_n])
-                    if len(pts) == 4:
-                        pts = (pts[0], pts[1], pts[3], pts[2])
-                    img.add_fill(pts, colors.WHITE, 0.5)
-
-            for dim, e_n in entities:
-                n = len(dofs_by_subentity[dim][e_n])
-                if n > 0:
-                    sub_ref = self.reference.sub_entity(dim, e_n)
-                    points: typing.List[PointType] = []
-                    if dim == 0:
-                        assert n == 1
-                        points = [sub_ref.vertices[0]]
-                    elif dim == 1:
-                        points = [tuple(o + sympy.Rational(i * a, n + 1)
-                                        for o, a in zip(sub_ref.origin, *sub_ref.axes))
-                                  for i in range(1, n + 1)]
-                    elif dim == 2:
-                        ne = 1
-                        while ne * (ne + 1) // 2 < n:
-                            ne += 1
-                        points = [tuple(o + sympy.Rational(i * a + j * b, n + 1)
-                                        for o, a, b in zip(sub_ref.origin, *sub_ref.axes))
-                                  for i in range(1, ne + 1) for j in range(1, ne + 1 - i)]
-                    elif dim == 3:
-                        ne = 1
-                        while ne * (ne + 1) * (ne + 2) // 6 < n:
-                            ne += 1
-                        points = [tuple(o + sympy.Rational(i * a + j * b + k * c, n + 1)
-                                        for o, a, b, c in zip(sub_ref.origin, *sub_ref.axes))
-                                  for i in range(1, ne + 1) for j in range(1, ne + 1 - i)
-                                  for k in range(1, ne + 1 - i - j)]
-
-                    for p, d in zip(points, dofs_by_subentity[dim][e_n]):
-                        img.add_dof_marker(p, d, colors.entity(dim))
-
-        img.save(filename, plot_options=plot_options)
-
     def test(self):
         """Run tests for this element."""
         super().test()
         self.test_independence()
 
     def test_independence(self):
         """Test that the basis functions of this element are linearly independent."""
@@ -842,14 +889,149 @@
                     if t in fd:
                         mat[j][i] = fd[t]
         mat = sympy.Matrix(mat)
 
         assert mat.rank() == mat.rows
 
 
+class EnrichedElement(FiniteElement):
+    """Finite element defined directly."""
+
+    _basis_functions: typing.Optional[typing.List[AnyFunction]]
+
+    def __init__(
+        self, subelements: typing.List[FiniteElement],
+    ):
+        """Create an enriched element.
+
+        Args:
+            subelements: The sub elements
+        """
+        reference = subelements[0].reference
+        order = subelements[0].order
+        domain_dim = subelements[0].domain_dim
+        range_dim = subelements[0].range_dim
+        range_shape = subelements[0].range_shape
+        for e in subelements:
+            assert e.reference == reference
+            assert e.domain_dim == domain_dim
+            assert e.range_dim == range_dim
+            assert e.range_shape == range_shape
+        self._basis_functions = None
+        self._subelements = subelements
+
+        super().__init__(reference, order, sum(e.space_dim for e in subelements),
+                         domain_dim, range_dim, range_shape)
+
+    def entity_dofs(self, entity_dim: int, entity_number: int) -> typing.List[int]:
+        """Get the numbers of the DOFs associated with the given entity.
+
+        Args:
+            entity_dim: The dimension of the entity
+            entity_number: The number of the entity
+
+        Returns:
+            The numbers of the DOFs associated with the entity
+        """
+        start = 0
+        dofs = []
+        for e in self._subelements:
+            dofs += [start + i for i in e.entity_dofs(entity_dim, entity_number)]
+            start += e.space_dim
+        return dofs
+
+    def dof_plot_positions(self) -> typing.List[PointType]:
+        """Get the points to plot each DOF at on a DOF diagram.
+
+        Returns:
+            The DOF positions
+        """
+        positions = []
+        for e in self._subelements:
+            positions += e.dof_plot_positions()
+        return positions
+
+    def dof_directions(self) -> typing.List[typing.Union[PointType, None]]:
+        """Get the direction associated with each DOF.
+
+        Returns:
+            The DOF directions
+        """
+        positions = []
+        for e in self._subelements:
+            positions += e.dof_directions()
+        return positions
+
+    def dof_entities(self) -> typing.List[typing.Tuple[int, int]]:
+        """Get the entities that each DOF is associated with.
+
+        Returns:
+            The entities
+        """
+        positions = []
+        for e in self._subelements:
+            positions += e.dof_entities()
+        return positions
+
+    def get_basis_functions(
+        self, use_tensor_factorisation: bool = False
+    ) -> typing.List[AnyFunction]:
+        """Get the basis functions of the element.
+
+        Args:
+            use_tensor_factorisation: Should a tensor factorisation be used?
+
+        Returns:
+            The basis functions
+        """
+        if use_tensor_factorisation:
+            return self._get_basis_functions_tensor()
+
+        if self._basis_functions is None:
+            self._basis_functions = []
+            for e in self._subelements:
+                self._basis_functions += e.get_basis_functions()
+
+        return self._basis_functions
+
+    def map_to_cell(
+        self, vertices_in: SetOfPointsInput,
+        basis: typing.Optional[typing.List[AnyFunction]] = None,
+        forward_map: typing.Optional[PointType] = None,
+        inverse_map: typing.Optional[PointType] = None
+    ) -> typing.List[AnyFunction]:
+        """Map the basis onto a cell using the appropriate mapping for the element.
+
+        Args:
+            vertices_in: The vertices of the cell
+            basis: The basis functions
+            forward_map: The map from the reference to the cell
+            inverse_map: The map to the reference from the cell
+
+        Returns:
+            The basis functions mapped to the cell
+        """
+        out = []
+        for e in self._subelements:
+            out += e.map_to_cell(vertices_in, basis, forward_map, inverse_map)
+        return out
+
+    def get_polynomial_basis(self) -> typing.List[AnyFunction]:
+        """Get the symbolic polynomial basis for the element.
+
+        Returns:
+            The polynomial basis
+        """
+        raise NotImplementedError()
+
+    def test(self):
+        """Run tests for this element."""
+        super().test()
+
+
 class ElementBasisFunction(BasisFunction):
     """A basis function of a finite element."""
 
     def __init__(self, element: FiniteElement, n: int):
         """Create an element basis function.
 
         Args:
```

### Comparing `symfem-2023.1.1/symfem/functionals.py` & `symfem-2023.4.1/symfem/functionals.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/functions.py` & `symfem-2023.4.1/symfem/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -310,20 +310,24 @@
 
         Returns:
             The norm
         """
         pass
 
     @abstractmethod
-    def integral(self, domain: Reference, vars: AxisVariablesNotSingle = t):
+    def integral(
+        self, domain: Reference, vars: AxisVariablesNotSingle = x,
+        dummy_vars: AxisVariablesNotSingle = t
+    ) -> ScalarFunction:
         """Compute the integral of the function.
 
         Args:
             domain: The domain of the integral
             vars: The variables to integrate with respect to
+            dummy_vars: The dummy variables to use inside the integral
 
         Returns:
             The integral
         """
         pass
 
     @abstractmethod
@@ -404,24 +408,30 @@
 
         img = Picture(**kwargs)
 
         if dof_entity is not None and dof_entity[0] > 1:
             sub_e = reference.sub_entity(*dof_entity)
             img.add_fill([i + extra for i in sub_e.clockwise_vertices], colors.BLUE, 0.5)
 
-        for ze in reference.z_ordered_entities_extra_dim():
+        if self.is_scalar:
+            zentities = reference.z_ordered_entities_extra_dim()
+        else:
+            zentities = reference.z_ordered_entities()
+
+        for ze in zentities:
             for dim, entity in ze:
                 if dim == 1:
                     c = colors.GRAY
                     if dof_entity == (1, entity):
                         c = colors.BLUE
                     img.add_line(
                         reference.vertices[reference.edges[entity][0]] + extra,
                         reference.vertices[reference.edges[entity][1]] + extra, c)
 
+            for dim, entity in ze:
                 if dim == reference.tdim:
                     self.plot_values(reference, img, value_scale)
 
             if (dim, entity) in ze:
                 if dof_direction is not None:
                     assert dof_point is not None and dof_n is not None
                     img.add_dof_arrow(dof_point + extra, dof_direction + extra, dof_n,
@@ -748,30 +758,35 @@
         """Compute the norm of the function.
 
         Returns:
             The norm
         """
         return ScalarFunction(abs(self._f))
 
-    def integral(self, domain: Reference, vars: AxisVariablesNotSingle = t) -> ScalarFunction:
+    def integral(
+        self, domain: Reference, vars: AxisVariablesNotSingle = x,
+        dummy_vars: AxisVariablesNotSingle = t
+    ) -> ScalarFunction:
         """Compute the integral of the function.
 
         Args:
             domain: The domain of the integral
             vars: The variables to integrate with respect to
+            dummy_vars: The dummy variables to use inside the integral
 
         Returns:
             The integral
         """
-        limits = domain.integration_limits(vars)
-
+        limits = domain.integration_limits(dummy_vars)
         point = VectorFunction(domain.origin)
-        for ti, a in zip(t, domain.axes):
+        for ti, a in zip(dummy_vars, domain.axes):
             point += ti * VectorFunction(a)
-        out = self._f.subs(x, point)
+        out = self._f * 1
+        for v, p in zip(vars, point):
+            out = out.subs(v, p)
 
         if len(limits[0]) == 2:
             for i in limits:
                 assert len(i) == 2
                 out = out.subs(*i)
             return out
 
@@ -1149,20 +1164,24 @@
             The norm
         """
         a = sympy.Integer(0)
         for i in self._vec:
             a += i._f ** 2
         return ScalarFunction(sympy.sqrt(a))
 
-    def integral(self, domain: Reference, vars: AxisVariablesNotSingle = t):
+    def integral(
+        self, domain: Reference, vars: AxisVariablesNotSingle = x,
+        dummy_vars: AxisVariablesNotSingle = t
+    ) -> ScalarFunction:
         """Compute the integral of the function.
 
         Args:
             domain: The domain of the integral
             vars: The variables to integrate with respect to
+            dummy_vars: The dummy variables to use inside the integral
 
         Returns:
             The integral
         """
         raise NotImplementedError()
 
     def __iter__(self):
@@ -1577,20 +1596,24 @@
         """Compute the norm of the function.
 
         Returns:
             The norm
         """
         raise NotImplementedError()
 
-    def integral(self, domain: Reference, vars: AxisVariablesNotSingle = t):
+    def integral(
+        self, domain: Reference, vars: AxisVariablesNotSingle = x,
+        dummy_vars: AxisVariablesNotSingle = t
+    ) -> ScalarFunction:
         """Compute the integral of the function.
 
         Args:
             domain: The domain of the integral
             vars: The variables to integrate with respect to
+            dummy_vars: The dummy variables to use inside the integral
 
         Returns:
             The integral
         """
         raise NotImplementedError()
 
     def det(self) -> ScalarFunction:
```

### Comparing `symfem-2023.1.1/symfem/geometry.py` & `symfem-2023.4.1/symfem/geometry.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/mappings.py` & `symfem-2023.4.1/symfem/mappings.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/moments.py` & `symfem-2023.4.1/symfem/moments.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/piecewise_functions.py` & `symfem-2023.4.1/symfem/piecewise_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from __future__ import annotations
 
 import typing
 
 import sympy
 
-from .functions import (AnyFunction, FunctionInput, SympyFormat, ValuesToSubstitute, VectorFunction,
-                        _to_sympy_format, parse_function_input)
+from .functions import (AnyFunction, FunctionInput, ScalarFunction, SympyFormat, ValuesToSubstitute,
+                        VectorFunction, _to_sympy_format, parse_function_input)
 from .geometry import (PointType, SetOfPoints, SetOfPointsInput, parse_set_of_points_input,
                        point_in_quadrilateral, point_in_tetrahedron, point_in_triangle)
 from .references import Reference
 from .symbols import AxisVariables, AxisVariablesNotSingle, t, x
 
 
 class PiecewiseFunction(AnyFunction):
@@ -418,28 +418,35 @@
 
         Returns:
             The norm
         """
         return PiecewiseFunction(
             {shape: f.norm() for shape, f in self._pieces.items()}, self.tdim)
 
-    def integral(self, domain: Reference, vars: AxisVariablesNotSingle = t) -> AnyFunction:
+    def integral(
+        self, domain: Reference, vars: AxisVariablesNotSingle = x,
+        dummy_vars: AxisVariablesNotSingle = t
+    ) -> ScalarFunction:
         """Compute the integral of the function.
 
         Args:
             domain: The domain of the integral
             vars: The variables to integrate with respect to
+            dummy_vars: The dummy variables to use inside the integral
 
         Returns:
             The integral
         """
-        # TODO: Add check that the domain is a subset of one piece
-        # TODO: Add integral over multiple pieces
-        p = self.get_piece(domain.midpoint())
-        return p.integral(domain, vars)
+        result = ScalarFunction(0)
+        for shape, f in self._pieces.items():
+            ref = _piece_reference(self.tdim, shape)
+            sub_domain = ref.intersection(domain)
+            if sub_domain is not None:
+                result += f.integral(sub_domain, vars, dummy_vars)
+        return result
 
     def det(self) -> PiecewiseFunction:
         """Compute the determinant.
 
         Returns:
             The deteminant
         """
@@ -496,36 +503,41 @@
 
         Args:
             reference: The reference cell
             img: The image to plot on
             value_scale: The scale factor for the function values
             n: The number of points per side for plotting
         """
-        from .create import create_reference
         from .plotting import Picture
         assert isinstance(img, Picture)
 
         for shape, f in self._pieces.items():
-            if self.tdim == 2:
-                if len(shape) == 3:
-                    ref = create_reference("triangle", shape)
-                elif len(shape) == 4:
-                    ref = create_reference("quadrilateral", shape)
-                else:
-                    raise ValueError("Unsupported cell type")
-            elif self.tdim == 3:
-                if len(shape) == 4:
-                    ref = create_reference("tetrahedron", shape)
-                else:
-                    raise ValueError("Unsupported cell type")
-            else:
-                raise ValueError("Unsupported tdim")
+            ref = _piece_reference(self.tdim, shape)
             f.plot_values(ref, img, value_scale, n // 2)
 
     def with_floats(self) -> AnyFunction:
         """Return a version the function with floats as coefficients.
 
         Returns:
             A version the function with floats as coefficients
         """
         return PiecewiseFunction(
             {shape: f.with_floats() for shape, f in self._pieces.items()}, self.tdim)
+
+
+def _piece_reference(tdim, shape):
+    """Create a reference element for a single piece."""
+    from .create import create_reference
+    if tdim == 2:
+        if len(shape) == 3:
+            return create_reference("triangle", shape)
+        elif len(shape) == 4:
+            return create_reference("quadrilateral", shape)
+        else:
+            raise ValueError("Unsupported cell type")
+    elif tdim == 3:
+        if len(shape) == 4:
+            return create_reference("tetrahedron", shape)
+        else:
+            raise ValueError("Unsupported cell type")
+    else:
+        raise ValueError("Unsupported tdim")
```

### Comparing `symfem-2023.1.1/symfem/plotting.py` & `symfem-2023.4.1/symfem/plotting.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/polynomials.py` & `symfem-2023.4.1/symfem/polynomials.py`

 * *Files 0% similar despite different names*

```diff
@@ -1072,12 +1072,12 @@
     """
     from .create import create_reference
 
     poly = orthogonal_basis(cell, order, derivs, variables)
     ref = create_reference(cell)
     if variables is None:
         variables = x
-    norms = [sympy.sqrt((f ** 2).integral(ref, variables)) for f in poly[0]]
+    norms = [sympy.sqrt((f ** 2).integral(ref, dummy_vars=variables)) for f in poly[0]]
     for i, n in enumerate(norms):
         for j in range(len(poly)):
             poly[j][i] /= n
     return poly
```

### Comparing `symfem-2023.1.1/symfem/quadrature.py` & `symfem-2023.4.1/symfem/quadrature.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem/references.py` & `symfem-2023.4.1/symfem/references.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,57 @@
 
 LatticeWithLines = typing.Tuple[SetOfPoints, typing.List[typing.Tuple[int, int]]]
 IntLimits = typing.List[typing.Union[
     typing.Tuple[sympy.core.symbol.Symbol, sympy.core.expr.Expr, sympy.core.expr.Expr],
     typing.Tuple[sympy.core.symbol.Symbol, sympy.core.expr.Expr]]]
 
 
+def _which_side(vs: SetOfPoints, p: PointType, q: PointType) -> typing.Optional[int]:
+    """Check which side of a line or plane a set of points are.
+
+    Args:
+        vs: The set of points
+        p: A point on the line or plane
+        q: Another point on the line (2D) or the normal to the plane (3D)
+
+    Returns:
+        2 if the points are all to the left, 1 if the points are all to the left or on the line,
+        0 if the points are all on the line, -1 if the points are all to the right or on the line,
+        -1 if the points are all to the right, None if there are some points on either side.
+    """
+    sides = []
+    for v in vs:
+        if len(q) == 2:
+            cross = (v[0] - p[0]) * (q[1] - p[1]) - (v[1] - p[1]) * (q[0] - p[0])
+        elif len(q) == 3:
+            cross = (v[0] - p[0]) * q[0] + (v[1] - p[1]) * q[1] + (v[2] - p[2]) * q[2]
+        else:
+            return None
+        if cross == 0:
+            sides.append(0)
+        elif cross > 0:
+            sides.append(1)
+        else:
+            sides.append(-1)
+
+    if -1 in sides and 1 in sides:
+        return None
+    if 1 in sides:
+        if 0 in sides:
+            return 1
+        else:
+            return 2
+    if -1 in sides:
+        if 0 in sides:
+            return -1
+        else:
+            return -2
+    return 0
+
+
 def _vsub(v: PointTypeInput, w: PointTypeInput) -> PointType:
     """Subtract.
 
     Args:
         v: A vector
         w: A vector
 
@@ -151,14 +194,53 @@
         """Get list of vertices in clockwise order.
 
         Returns:
             A list of vertices
         """
         return self.vertices
 
+    def intersection(self, other: Reference) -> typing.Optional[Reference]:
+        """Get the intersection of two references.
+
+        Returns:
+            A reference element that is the intersection
+        """
+        if self.gdim != other.gdim:
+            raise ValueError("Incompatible cell dimensions")
+
+        for cell1, cell2 in [(self, other), (other, self)]:
+            try:
+                for v in cell1.vertices:
+                    if not cell2.contains(v):
+                        break
+                else:
+                    return cell1
+            except NotImplementedError:
+                pass
+        for cell1, cell2 in [(self, other), (other, self)]:
+            if cell1.gdim == 2:
+                for e in cell1.edges:
+                    p = cell1.vertices[e[0]]
+                    q = cell1.vertices[e[1]]
+                    dir1 = _which_side(cell1.vertices, p, q)
+                    dir2 = _which_side(cell2.vertices, p, q)
+                    if dir1 is not None and dir2 is not None and dir1 * dir2 < 0:
+                        return None
+            if cell1.gdim == 3:
+                for i in range(cell1.sub_entity_count(2)):
+                    face = cell1.sub_entity(2, i)
+                    p = face.midpoint()
+                    n = face.normal()
+                    dir1 = _which_side(cell1.vertices, p, n)
+                    dir2 = _which_side(cell2.vertices, p, n)
+                    if dir1 is not None and dir2 is not None and dir1 * dir2 < 0:
+                        return None
+
+        raise NotImplementedError("Intersection of these elements is not yet supported")
+
     @abstractmethod
     def default_reference(self) -> Reference:
         """Get the default reference for this cell type.
 
         Returns:
             The default reference
         """
@@ -1024,17 +1106,25 @@
 
         Args:
             point: The point
 
         Returns:
             Is the point contained in the reference?
         """
-        if self.vertices != self.reference_vertices:
-            raise NotImplementedError()
-        return 0 <= point[0] and 0 <= point[1] and sum(point) <= 1
+        if self.vertices == self.reference_vertices:
+            return 0 <= point[0] and 0 <= point[1] and sum(point) <= 1
+        elif self.gdim == 2:
+            po = _vsub(point, self.origin)
+            det = self.axes[0][0] * self.axes[1][1] - self.axes[0][1] * self.axes[1][0]
+            t0 = (self.axes[1][1] * po[0] - self.axes[1][0] * po[1]) / det
+            t1 = (self.axes[0][0] * po[1] - self.axes[0][1] * po[0]) / det
+            print(self.origin, self.axes, point)
+            print(t0, t1)
+            return 0 <= t0 and 0 <= t1 and t0 + t1 <= 1
+        raise NotImplementedError()
 
 
 class Tetrahedron(Reference):
     """A tetrahedron."""
 
     def __init__(self, vertices: SetOfPointsInput = ((0, 0, 0), (1, 0, 0), (0, 1, 0), (0, 0, 1))):
         """Create a tetrahedron.
@@ -1199,17 +1289,23 @@
 
         Args:
             point: The point
 
         Returns:
             Is the point contained in the reference?
         """
-        if self.vertices != self.reference_vertices:
-            raise NotImplementedError()
-        return 0 <= point[0] and 0 <= point[1] and 0 <= point[2] and sum(point) <= 1
+        if self.vertices == self.reference_vertices:
+            return 0 <= point[0] and 0 <= point[1] and 0 <= point[2] and sum(point) <= 1
+        else:
+            po = _vsub(point, self.origin)
+            minv = sympy.Matrix([[a[i] for a in self.axes] for i in range(3)]).inv()
+            t0 = (minv[0, 0] * po[0] + minv[0, 1] * po[1] + minv[0, 2] * po[2])
+            t1 = (minv[1, 0] * po[0] + minv[1, 1] * po[1] + minv[1, 2] * po[2])
+            t2 = (minv[2, 0] * po[0] + minv[2, 1] * po[1] + minv[2, 2] * po[2])
+            return 0 <= t0 and 0 <= t1 and 0 >= t2 and t0 + t1 + t2 <= 1
 
 
 class Quadrilateral(Reference):
     """A quadrilateral."""
 
     def __init__(self, vertices: SetOfPointsInput = ((0, 0), (1, 0), (0, 1), (1, 1))):
         """Create a quadrilateral.
@@ -2161,7 +2257,20 @@
             n: The number of points along each edge
 
         Returns:
             A lattice of points including the edges of the cell
             Pairs of point numbers that make a mesh of lines across the cell
         """
         raise NotImplementedError()
+
+    def z_ordered_entities_extra_dim(self) -> typing.List[typing.List[typing.Tuple[int, int]]]:
+        """Get the subentities in back-to-front plotting order when using an extra dimension.
+
+        Returns:
+            List of lists of subentity dimensions and numbers
+        """
+        N = 2 * self.number_of_triangles
+        n = (self.number_of_triangles + 1) // 2 * 2
+        return [
+            [(1, i) for i in range(n)] + [(0, i) for i in range(1, n)],
+            [(2, 0)] + [(1, i) for i in range(n, N)] + [(0, 0)] + [(0, i) for i in range(n, N)]
+        ]
```

### Comparing `symfem-2023.1.1/symfem/utils.py` & `symfem-2023.4.1/symfem/utils.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/symfem.egg-info/PKG-INFO` & `symfem-2023.4.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: symfem
-Version: 2023.1.1
-Summary: a symbolic finite element definition library
-Home-page: https://github.com/mscroggs/symfem
-Author: Matthew Scroggs
-Author-email: symfem@mscroggs.co.uk
-Maintainer-email: symfem@mscroggs.co.uk
-License: MIT
-Description-Content-Type: text/markdown
-Provides-Extra: style
-Provides-Extra: docs
-Provides-Extra: optional
-Provides-Extra: test
-License-File: LICENSE
-
 ![Symfem](https://raw.githubusercontent.com/mscroggs/symfem/main/logo/logo.png)
 
 |  | Badges |
 | --- | :---: |
 | Documentation | [![Documentation status](https://readthedocs.org/projects/symfem/badge/?version=latest)](https://symfem.readthedocs.io/en/latest/?badge=latest) |
 | Testing & coverage | [![Style checks](https://github.com/mscroggs/symfem/actions/workflows/style-checks.yml/badge.svg)](https://github.com/mscroggs/symfem/actions) [![Run tests](https://github.com/mscroggs/symfem/actions/workflows/run-tests.yml/badge.svg)](https://github.com/mscroggs/symfem/actions) [![Coverage Status](https://coveralls.io/repos/github/mscroggs/symfem/badge.svg?branch=main)](https://coveralls.io/github/mscroggs/symfem?branch=main) |
 | Packages | [![PyPI](https://img.shields.io/pypi/v/symfem?color=blue&label=PyPI&logo=pypi&logoColor=white)](https://pypi.org/project/symfem/) [![conda](https://anaconda.org/conda-forge/symfem/badges/version.svg)](https://anaconda.org/conda-forge/symfem) |
@@ -156,14 +140,15 @@
 
 ![The numbering of a reference interval](https://raw.githubusercontent.com/mscroggs/symfem/main/img/interval_numbering.png)
 
 ### List of supported elements
 - Bernstein (alternative names: Bernstein-Bezier)
 - bubble
 - dPc
+- enriched Galerkin (alternative names: EG)
 - Hermite
 - Lagrange (alternative names: P)
 - Morley-Wang-Xu (alternative names: MWX)
 - serendipity (alternative names: S)
 - Taylor (alternative names: discontinuous Taylor)
 - vector Lagrange (alternative names: vP)
 - Wu-Xu
@@ -182,14 +167,16 @@
 - Brezzi-Douglas-Fortin-Marini (alternative names: BDFM)
 - Brezzi-Douglas-Marini (alternative names: BDM, N2div)
 - bubble
 - bubble enriched Lagrange
 - bubble enriched vector Lagrange
 - conforming Crouzeix-Raviart (alternative names: conforming CR)
 - Crouzeix-Raviart (alternative names: CR, Crouzeix-Falk, CF)
+- enriched Galerkin (alternative names: EG)
+- enriched vector Galerkin (alternative names: locking-free enriched Galerkin, LFEG)
 - Fortin-Soulie (alternative names: FS)
 - Guzman-Neilan
 - Hellan-Herrmann-Johnson (alternative names: HHJ)
 - Hermite
 - Hsieh-Clough-Tocher (alternative names: Clough-Tocher, HCT, CT)
 - Kong-Mulder-Veldhuizen (alternative names: KMV)
 - Lagrange (alternative names: P)
@@ -219,14 +206,16 @@
 - Arbogast-Correa (alternative names: AC, AC full, Arbogast-Correa full)
 - Arnold-Boffi-Falk (alternative names: ABF)
 - Bogner-Fox-Schmit (alternative names: BFS)
 - Brezzi-Douglas-Fortin-Marini (alternative names: BDFM)
 - bubble
 - direct serendipity
 - dPc
+- enriched Galerkin (alternative names: EG)
+- enriched vector Galerkin (alternative names: locking-free enriched Galerkin, LFEG)
 - Huang-Zhang (alternative names: HZ)
 - NCE (alternative names: RTCE, Qcurl, Nedelec, Ncurl)
 - NCF (alternative names: RTCF, Qdiv)
 - P1-iso-P2 (alternative names: P2-iso-P1, iso-P2 P1)
 - Q (alternative names: Lagrange, P)
 - Rannacher-Turek
 - Regge
@@ -249,14 +238,16 @@
 ### List of supported elements
 - Bernardi-Raugel
 - Bernstein (alternative names: Bernstein-Bezier)
 - Brezzi-Douglas-Fortin-Marini (alternative names: BDFM)
 - Brezzi-Douglas-Marini (alternative names: BDM, N2div)
 - bubble
 - Crouzeix-Raviart (alternative names: CR, Crouzeix-Falk, CF)
+- enriched Galerkin (alternative names: EG)
+- enriched vector Galerkin (alternative names: locking-free enriched Galerkin, LFEG)
 - Guzman-Neilan
 - Hermite
 - Kong-Mulder-Veldhuizen (alternative names: KMV)
 - Lagrange (alternative names: P)
 - Mardal-Tai-Winther (alternative names: MTW)
 - matrix Lagrange
 - Morley-Wang-Xu (alternative names: MWX)
@@ -276,14 +267,16 @@
 ![The numbering of a reference hexahedron](https://raw.githubusercontent.com/mscroggs/symfem/main/img/hexahedron_numbering.png)
 
 ### List of supported elements
 - Brezzi-Douglas-Duran-Fortin (alternative names: BDDF)
 - Brezzi-Douglas-Fortin-Marini (alternative names: BDFM)
 - bubble
 - dPc
+- enriched Galerkin (alternative names: EG)
+- enriched vector Galerkin (alternative names: locking-free enriched Galerkin, LFEG)
 - NCE (alternative names: RTCE, Qcurl, Nedelec, Ncurl)
 - NCF (alternative names: RTCF, Qdiv)
 - Q (alternative names: Lagrange, P)
 - Rannacher-Turek
 - Regge
 - serendipity (alternative names: S)
 - serendipity Hcurl (alternative names: Scurl, BDMCE, AAE)
```

### Comparing `symfem-2023.1.1/symfem.egg-info/SOURCES.txt` & `symfem-2023.4.1/symfem.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 symfem/elements/bfs.py
 symfem/elements/bubble.py
 symfem/elements/conforming_crouzeix_raviart.py
 symfem/elements/crouzeix_raviart.py
 symfem/elements/direct_serendipity.py
 symfem/elements/dpc.py
 symfem/elements/dual.py
+symfem/elements/enriched_galerkin.py
 symfem/elements/fortin_soulie.py
 symfem/elements/guzman_neilan.py
 symfem/elements/hct.py
 symfem/elements/hermite.py
 symfem/elements/hhj.py
 symfem/elements/huang_zhang.py
 symfem/elements/kmv.py
@@ -66,14 +67,15 @@
 symfem/elements/rhct.py
 symfem/elements/rt.py
 symfem/elements/serendipity.py
 symfem/elements/taylor.py
 symfem/elements/tnt.py
 symfem/elements/transition.py
 symfem/elements/trimmed_serendipity.py
+symfem/elements/vector_enriched_galerkin.py
 symfem/elements/wu_xu.py
 test/__init__.py
 test/conftest.py
 test/test_against_basix.py
 test/test_against_computed_by_hand.py
 test/test_arnold_winther.py
 test/test_bernstein.py
```

### Comparing `symfem-2023.1.1/test/conftest.py` & `symfem-2023.4.1/test/conftest.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/test/test_against_basix.py` & `symfem-2023.4.1/test/test_against_basix.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,22 +127,26 @@
             import basix
         except ImportError:
             pytest.skip("Basix must be installed to run this test.")
 
     import numpy as np
 
     points = make_lattice(cell, 2)
-    parsed_args = []
+    parsed_args = [
+        basix.LagrangeVariant.unset,
+        basix.DPCVariant.unset,
+        False
+    ]
     for a in args:
         if a[0] == "LagrangeVariant":
-            parsed_args.append(basix.variants.string_to_lagrange_variant(a[1]))
+            parsed_args[0] = basix.variants.string_to_lagrange_variant(a[1])
         elif a[0] == "DPCVariant":
-            parsed_args.append(basix.variants.string_to_dpc_variant(a[1]))
+            parsed_args[1] = basix.variants.string_to_dpc_variant(a[1])
         elif a[0] == "bool":
-            parsed_args.append(a[1])
+            parsed_args[2] = a[1]
         else:
             raise ValueError(f"Unknown arg type: {a[0]}")
     space = basix.create_element(
         basix.finite_element.string_to_family(basix_type, cell),
         basix.cell.string_to_type(cell), order, *parsed_args)
     result = space.tabulate(0, points)[0]
```

### Comparing `symfem-2023.1.1/test/test_against_computed_by_hand.py` & `symfem-2023.4.1/test/test_against_computed_by_hand.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/test/test_bernstein.py` & `symfem-2023.4.1/test/test_bernstein.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/test/test_docs.py` & `symfem-2023.4.1/test/test_docs.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/test/test_dof_descriptions.py` & `symfem-2023.4.1/test/test_dof_descriptions.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/test/test_elements.py` & `symfem-2023.4.1/test/test_elements.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/test/test_functions.py` & `symfem-2023.4.1/test/test_functions.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/test/test_guzman_neilan.py` & `symfem-2023.4.1/test/test_guzman_neilan.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/test/test_hct.py` & `symfem-2023.4.1/test/test_hct.py`

 * *Files 14% similar despite different names*

```diff
@@ -74,7 +74,24 @@
         f1 = f.get_piece((half, 0)).diff(x[1]).subs(x[1], 0)
         f2 = f.get_piece((half, half))
         f2 = (f2.diff(x[0]) + f2.diff(x[1])).subs(x[1], 1 - x[0])
         f3 = f.get_piece((0, half)).diff(x[0]).subs(x[0], 0)
         assert f1.diff(x[0]).diff(x[0]) == 0
         assert f2.diff(x[0]).diff(x[0]) == 0
         assert f3.diff(x[1]).diff(x[1]) == 0
+
+
+def test_rhct_integral():
+    element = symfem.create_element("triangle", "rHCT", 3)
+    ref = element.reference
+    f1 = element.get_basis_function(1).directional_derivative((1, 0))
+    f2 = element.get_basis_function(6).directional_derivative((1, 0))
+    integrand = f1 * f2
+
+    third = sympy.Rational(1, 3)
+    expr = (f1*f2).pieces[((0, 1), (0, 0), (third, third))].as_sympy()
+    assert len((f1*f2).pieces) == 3
+    assert (f1*f2).pieces[((0, 0), (1, 0), (third, third))] == 0
+    assert (f1*f2).pieces[((1, 0), (0, 1), (third, third))] == 0
+
+    assert sympy.integrate(sympy.integrate(
+        expr, (x[1], x[0], 1 - 2 * x[0])), (x[0], 0, third)) == integrand.integral(ref, x)
```

### Comparing `symfem-2023.1.1/test/test_nedelec.py` & `symfem-2023.4.1/test/test_nedelec.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/test/test_p1_iso_p2.py` & `symfem-2023.4.1/test/test_p1_iso_p2.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/test/test_plotting.py` & `symfem-2023.4.1/test/test_plotting.py`

 * *Files 6% similar despite different names*

```diff
@@ -106,14 +106,27 @@
         e.plot_dof_diagram(os.path.join(
             folder, f"test_dof_diagrams_raviart_thomas-{reference}-{degree}.{ext}"))
     compile_tex(f"test_dof_diagrams_raviart_thomas-{reference}-{degree}.tex")
 
 
 @pytest.mark.parametrize("reference", [
     "interval", "triangle", "quadrilateral",
+    "tetrahedron", "hexahedron",
+])
+@pytest.mark.parametrize("degree", [1, 2])
+def test_dof_diagrams_eg(reference, degree):
+    e = symfem.create_element(reference, "EG", degree)
+    for ext in ["svg", "png", "tex"]:
+        e.plot_dof_diagram(os.path.join(
+            folder, f"test_dof_diagrams_eg-{reference}-{degree}.{ext}"))
+    compile_tex(f"test_dof_diagrams_eg-{reference}-{degree}.tex")
+
+
+@pytest.mark.parametrize("reference", [
+    "interval", "triangle", "quadrilateral",
 ])
 @pytest.mark.parametrize("degree", [0, 1, 2])
 def test_function_plots_lagrange(reference, degree):
     e = symfem.create_element(reference, "P", degree)
     for ext in ["svg", "png", "tex"]:
         e.plot_basis_function(0, os.path.join(
             folder, f"test_function_plots_lagrange-{reference}-{degree}.{ext}"))
@@ -174,14 +187,26 @@
         e.plot_basis_function(0, os.path.join(
             folder, f"test_function_plots_bc-{n}.{ext}"))
     compile_tex(f"test_function_plots_bc-{n}.tex")
 
 
 @pytest.mark.parametrize("reference", [
     "interval", "triangle", "quadrilateral",
+])
+@pytest.mark.parametrize("degree", [1, 2])
+def test_function_plots_eg(reference, degree):
+    e = symfem.create_element(reference, "EG", degree)
+    for ext in ["svg", "png", "tex"]:
+        e.plot_basis_function(0, os.path.join(
+            folder, f"test_function_plots_eg-{reference}-{degree}.{ext}"))
+    compile_tex(f"test_function_plots_eg-{reference}-{degree}.tex")
+
+
+@pytest.mark.parametrize("reference", [
+    "interval", "triangle", "quadrilateral",
     "tetrahedron", "hexahedron", "prism", "pyramid",
     "dual polygon(6)"
 ])
 def test_plot_reference(reference):
     r = symfem.create_reference(reference)
     rname = reference.replace("(", "").replace(")", "").replace(" ", "_")
     for ext in ["svg", "png", "tex"]:
```

### Comparing `symfem-2023.1.1/test/test_polynomials.py` & `symfem-2023.4.1/test/test_polynomials.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/test/test_quadrature.py` & `symfem-2023.4.1/test/test_quadrature.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/test/test_references.py` & `symfem-2023.4.1/test/test_references.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/test/test_reorder.py` & `symfem-2023.4.1/test/test_reorder.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/test/test_stiffness_matrix.py` & `symfem-2023.4.1/test/test_stiffness_matrix.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/test/test_tensor_product.py` & `symfem-2023.4.1/test/test_tensor_product.py`

 * *Files identical despite different names*

### Comparing `symfem-2023.1.1/test/utils.py` & `symfem-2023.4.1/test/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
         "serendipity": [({"variant": "equispaced"}, range(1, 6)),
                         ({"variant": "lobatto"}, range(1, 3))],
         "Hermite": [({}, [3])],
         "Bernstein": [({}, range(1, 4))],
         "Taylor": [({}, range(0, 5))],
         "Wu-Xu": [({}, [2])],
         "MWX": [({}, [1])],
+        "EG": [({}, range(1, 5))],
     },
     "triangle": {
         "P": [({"variant": "equispaced"}, range(5)), ({"variant": "lobatto"}, range(3))],
         "vP": [({"variant": "equispaced"}, range(5)), ({"variant": "lobatto"}, range(3))],
         "matrix Lagrange": [({"variant": "equispaced"}, range(3)),
                             ({"variant": "lobatto"}, range(3))],
         "symmetric matrix Lagrange": [
@@ -61,14 +62,16 @@
         "Wu-Xu": [({}, [3])],
         "transition": [({"edge_orders": [1, 1, 1], "variant": "equispaced"}, range(1, 6)),
                        ({"edge_orders": [2, 2, 1], "variant": "equispaced"}, range(1, 6)),
                        ({"edge_orders": [3, 3, 1], "variant": "equispaced"}, range(1, 6)),
                        ({"edge_orders": [3, 3, 2], "variant": "equispaced"}, range(1, 6)),
                        ({"edge_orders": [2, 2, 1], "variant": "lobatto"}, range(1, 3))],
         "P1-iso-P2": [({}, [1])],
+        "EG": [({}, range(1, 4))],
+        "LFEG": [({}, range(1, 4))],
     },
     "tetrahedron": {
         "P": [({"variant": "equispaced"}, range(3)), ({"variant": "lobatto"}, range(3))],
         "vP": [({"variant": "equispaced"}, range(3)), ({"variant": "lobatto"}, range(3))],
         "matrix Lagrange": [({"variant": "equispaced"}, range(2)),
                             ({"variant": "lobatto"}, range(3))],
         "symmetric matrix Lagrange": [({"variant": "equispaced"}, range(2)),
@@ -102,14 +105,16 @@
                          "variant": "equispaced"}, range(1, 5)),
                        ({"edge_orders": [3, 2, 1, 2, 1, 1], "face_orders": [1, 1, 1, 1],
                          "variant": "equispaced"}, range(1, 5)),
                        ({"edge_orders": [1, 1, 3, 1, 3, 1], "face_orders": [1, 1, 1, 1],
                          "variant": "equispaced"}, range(1, 5)),
                        ({"edge_orders": [1, 1, 2, 1, 2, 5], "face_orders": [3, 3, 2, 5],
                          "variant": "equispaced"}, range(1, 5))],
+        "EG": [({}, range(1, 3))],
+        "LFEG": [({}, range(1, 3))],
     },
     "quadrilateral": {
         "bubble": [({"variant": "equispaced"}, range(2, 4)), ({"variant": "lobatto"}, range(2, 4))],
         "Q": [({"variant": "equispaced"}, range(4)), ({"variant": "lobatto"}, range(3))],
         "vQ": [({"variant": "equispaced"}, range(4)), ({"variant": "lobatto"}, range(3))],
         "dPc": [({"variant": "equispaced"}, range(4)), ({"variant": "lobatto"}, range(3))],
         "vector dPc": [({"variant": "equispaced"}, range(4)), ({"variant": "lobatto"}, range(3))],
@@ -129,14 +134,16 @@
         "TNTdiv": [({"variant": "equispaced"}, range(1, 4))],
         "Regge": [({"variant": "integral"}, range(3))],
         "ABF": [({}, range(3))],
         "AC": [({}, range(4))],
         "Rannacher-Turek": [({}, [1])],
         "P1-iso-P2": [({}, [1])],
         "HZ": [({}, [2, 3, 4])],
+        "EG": [({}, range(1, 4))],
+        "LFEG": [({}, range(1, 4))],
     },
     "hexahedron": {
         "bubble": [({"variant": "equispaced"}, range(2, 4)), ({"variant": "lobatto"}, range(2, 4))],
         "Q": [({"variant": "equispaced"}, range(3)), ({"variant": "lobatto"}, range(3))],
         "vQ": [({"variant": "equispaced"}, range(3)), ({"variant": "lobatto"}, range(3))],
         "dPc": [({"variant": "equispaced"}, range(3)), ({"variant": "lobatto"}, range(3))],
         "vector dPc": [({"variant": "equispaced"}, range(3)), ({"variant": "lobatto"}, range(3))],
@@ -151,14 +158,16 @@
         "TScurl": [({"variant": "equispaced"}, range(1, 4))],
         "TSdiv": [({"variant": "equispaced"}, range(1, 4))],
         "TNT": [({"variant": "equispaced"}, range(1, 2))],
         "TNTcurl": [({"variant": "equispaced"}, range(1, 2))],
         "TNTdiv": [({"variant": "equispaced"}, range(1, 2))],
         "Regge": [({"variant": "integral"}, range(2))],
         "Rannacher-Turek": [({}, [1])],
+        "EG": [({}, range(1, 3))],
+        "LFEG": [({}, range(1, 3))],
     },
     "prism": {
         "Lagrange": [({"variant": "equispaced"}, range(4))],
         "Nedelec": [({"variant": "equispaced"}, range(1, 3))],
     },
     "pyramid": {
         "Lagrange": [({"variant": "equispaced"}, range(4))],
```

