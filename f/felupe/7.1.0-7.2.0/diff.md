# Comparing `tmp/felupe-7.1.0.tar.gz` & `tmp/felupe-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "felupe-7.1.0.tar", last modified: Fri Apr 14 22:57:35 2023, max compression
+gzip compressed data, was "felupe-7.2.0.tar", last modified: Wed Apr 26 20:11:06 2023, max compression
```

## Comparing `felupe-7.1.0.tar` & `felupe-7.2.0.tar`

### file list

```diff
@@ -1,129 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:35.686366 felupe-7.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35081 2023-04-14 22:57:27.000000 felupe-7.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    48189 2023-04-14 22:57:35.682366 felupe-7.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-04-14 22:57:27.000000 felupe-7.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-14 22:57:27.000000 felupe-7.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 22:57:35.686366 felupe-7.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:35.670365 felupe-7.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:35.670365 felupe-7.1.0/src/felupe/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:35.674366 felupe-7.1.0/src/felupe/_assembly/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/_assembly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/_assembly/_axi.py
--rw-r--r--   0 runner    (1001) docker     (123)     6501 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/_assembly/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23823 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/_assembly/_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/_assembly/_mixed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:35.674366 felupe-7.1.0/src/felupe/_basis/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/_basis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/_basis/_basis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:35.674366 felupe-7.1.0/src/felupe/_field/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/_field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/_field/_axi.py
--rw-r--r--   0 runner    (1001) docker     (123)     9796 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/_field/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/_field/_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/_field/_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/_field/_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/_field/_planestrain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:35.674366 felupe-7.1.0/src/felupe/constitution/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/constitution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/constitution/_kinematics.py
--rw-r--r--   0 runner    (1001) docker     (123)    17288 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/constitution/_mixed.py
--rw-r--r--   0 runner    (1001) docker     (123)     9816 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/constitution/_models_hyperelasticity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/constitution/_models_hyperelasticity_ad.py
--rw-r--r--   0 runner    (1001) docker     (123)    17606 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/constitution/_models_linear_elasticity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/constitution/_models_pseudo_elasticity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/constitution/_user_materials.py
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/constitution/_user_materials_hyperelastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/constitution/_user_materials_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:35.674366 felupe-7.1.0/src/felupe/dof/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/dof/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/dof/_boundary.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/dof/_loadcase.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/dof/_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:35.678366 felupe-7.1.0/src/felupe/element/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/element/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/element/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13838 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/element/_hexahedron.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/element/_lagrange.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/element/_line.py
--rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/element/_quad.py
--rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/element/_tetra.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/element/_triangle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:35.678366 felupe-7.1.0/src/felupe/math/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/math/_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/math/_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/math/_spatial.py
--rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/math/_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:35.678366 felupe-7.1.0/src/felupe/mechanics/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mechanics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mechanics/_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mechanics/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mechanics/_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mechanics/_multipoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mechanics/_pointload.py
--rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mechanics/_solidbody.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mechanics/_solidbody_gravity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mechanics/_solidbody_incompressible.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mechanics/_solidbody_pressure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mechanics/_step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:35.678366 felupe-7.1.0/src/felupe/mesh/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mesh/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mesh/_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     9293 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mesh/_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mesh/_discrete_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mesh/_dual.py
--rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mesh/_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mesh/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7272 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mesh/_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mesh/_read.py
--rw-r--r--   0 runner    (1001) docker     (123)    15966 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/mesh/_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:35.678366 felupe-7.1.0/src/felupe/quadrature/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/quadrature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/quadrature/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/quadrature/_gausslegendre.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/quadrature/_tetra.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/quadrature/_triangle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:35.682366 felupe-7.1.0/src/felupe/region/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/region/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13133 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/region/_boundary.py
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/region/_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/region/_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:35.682366 felupe-7.1.0/src/felupe/solve/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/solve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/solve/_solve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:35.682366 felupe-7.1.0/src/felupe/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8132 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/tools/_newton.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/tools/_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/tools/_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/tools/_save.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-14 22:57:27.000000 felupe-7.1.0/src/felupe/tools/_solve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:35.670365 felupe-7.1.0/src/felupe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    48189 2023-04-14 22:57:35.000000 felupe-7.1.0/src/felupe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-14 22:57:35.000000 felupe-7.1.0/src/felupe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 22:57:35.000000 felupe-7.1.0/src/felupe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-14 22:57:35.000000 felupe-7.1.0/src/felupe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 22:57:35.000000 felupe-7.1.0/src/felupe.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 22:57:35.682366 felupe-7.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-14 22:57:27.000000 felupe-7.1.0/tests/test_basis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-14 22:57:27.000000 felupe-7.1.0/tests/test_bilinearform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-14 22:57:27.000000 felupe-7.1.0/tests/test_composite.py
--rw-r--r--   0 runner    (1001) docker     (123)    12252 2023-04-14 22:57:27.000000 felupe-7.1.0/tests/test_constitution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-04-14 22:57:27.000000 felupe-7.1.0/tests/test_dof.py
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-04-14 22:57:27.000000 felupe-7.1.0/tests/test_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-04-14 22:57:27.000000 felupe-7.1.0/tests/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-04-14 22:57:27.000000 felupe-7.1.0/tests/test_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-04-14 22:57:27.000000 felupe-7.1.0/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-14 22:57:27.000000 felupe-7.1.0/tests/test_math.py
--rw-r--r--   0 runner    (1001) docker     (123)    12303 2023-04-14 22:57:27.000000 felupe-7.1.0/tests/test_mechanics.py
--rw-r--r--   0 runner    (1001) docker     (123)    11591 2023-04-14 22:57:27.000000 felupe-7.1.0/tests/test_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-04-14 22:57:27.000000 felupe-7.1.0/tests/test_mpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-04-14 22:57:27.000000 felupe-7.1.0/tests/test_planestrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-04-14 22:57:27.000000 felupe-7.1.0/tests/test_quadrature.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-04-14 22:57:27.000000 felupe-7.1.0/tests/test_readme.py
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-04-14 22:57:27.000000 felupe-7.1.0/tests/test_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-14 22:57:27.000000 felupe-7.1.0/tests/test_solve.py
--rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-04-14 22:57:27.000000 felupe-7.1.0/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:11:06.463003 felupe-7.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35081 2023-04-26 20:10:50.000000 felupe-7.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    49641 2023-04-26 20:11:06.463003 felupe-7.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-04-26 20:10:50.000000 felupe-7.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-26 20:10:50.000000 felupe-7.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 20:11:06.463003 felupe-7.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:11:06.447003 felupe-7.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:11:06.451003 felupe-7.2.0/src/felupe/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:11:06.451003 felupe-7.2.0/src/felupe/_assembly/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/_assembly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/_assembly/_axi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/_assembly/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23268 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/_assembly/_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/_assembly/_mixed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:11:06.451003 felupe-7.2.0/src/felupe/_basis/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/_basis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/_basis/_basis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:11:06.451003 felupe-7.2.0/src/felupe/_field/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/_field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/_field/_axi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/_field/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/_field/_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/_field/_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/_field/_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/_field/_planestrain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:11:06.451003 felupe-7.2.0/src/felupe/constitution/
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/constitution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/constitution/_kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17327 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/constitution/_mixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9596 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/constitution/_models_hyperelasticity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/constitution/_models_hyperelasticity_ad.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17201 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/constitution/_models_linear_elasticity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/constitution/_models_pseudo_elasticity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/constitution/_user_materials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/constitution/_user_materials_hyperelastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/constitution/_user_materials_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:11:06.455003 felupe-7.2.0/src/felupe/dof/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/dof/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/dof/_boundary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/dof/_loadcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/dof/_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:11:06.455003 felupe-7.2.0/src/felupe/element/
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/element/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/element/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13451 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/element/_hexahedron.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/element/_lagrange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/element/_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/element/_quad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/element/_tetra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/element/_triangle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:11:06.455003 felupe-7.2.0/src/felupe/math/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/math/_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/math/_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/math/_spatial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/math/_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:11:06.455003 felupe-7.2.0/src/felupe/mechanics/
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/mechanics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/mechanics/_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/mechanics/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/mechanics/_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/mechanics/_multipoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/mechanics/_pointload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/mechanics/_solidbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/mechanics/_solidbody_gravity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7118 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/mechanics/_solidbody_incompressible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/mechanics/_solidbody_pressure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/mechanics/_step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:11:06.459003 felupe-7.2.0/src/felupe/mesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/mesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/mesh/_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/mesh/_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/mesh/_discrete_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/mesh/_dual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/mesh/_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/mesh/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/mesh/_line_rectangle_cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/mesh/_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/mesh/_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15579 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/mesh/_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:11:06.459003 felupe-7.2.0/src/felupe/quadrature/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/quadrature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/quadrature/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/quadrature/_gausslegendre.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/quadrature/_tetra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/quadrature/_triangle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:11:06.459003 felupe-7.2.0/src/felupe/region/
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/region/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12824 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/region/_boundary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/region/_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/region/_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:11:06.459003 felupe-7.2.0/src/felupe/solve/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/solve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/solve/_solve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:11:06.459003 felupe-7.2.0/src/felupe/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/tools/_newton.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11397 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/tools/_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/tools/_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/tools/_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/tools/_save.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-26 20:10:50.000000 felupe-7.2.0/src/felupe/tools/_solve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:11:06.451003 felupe-7.2.0/src/felupe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    49641 2023-04-26 20:11:06.000000 felupe-7.2.0/src/felupe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-26 20:11:06.000000 felupe-7.2.0/src/felupe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 20:11:06.000000 felupe-7.2.0/src/felupe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-26 20:11:06.000000 felupe-7.2.0/src/felupe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 20:11:06.000000 felupe-7.2.0/src/felupe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:11:06.463003 felupe-7.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-26 20:10:50.000000 felupe-7.2.0/tests/test_basis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-26 20:10:50.000000 felupe-7.2.0/tests/test_bilinearform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-26 20:10:50.000000 felupe-7.2.0/tests/test_composite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12252 2023-04-26 20:10:50.000000 felupe-7.2.0/tests/test_constitution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-04-26 20:10:50.000000 felupe-7.2.0/tests/test_dof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-04-26 20:10:50.000000 felupe-7.2.0/tests/test_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-04-26 20:10:50.000000 felupe-7.2.0/tests/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-04-26 20:10:50.000000 felupe-7.2.0/tests/test_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-04-26 20:10:50.000000 felupe-7.2.0/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-04-26 20:10:50.000000 felupe-7.2.0/tests/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12303 2023-04-26 20:10:50.000000 felupe-7.2.0/tests/test_mechanics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11591 2023-04-26 20:10:50.000000 felupe-7.2.0/tests/test_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-04-26 20:10:50.000000 felupe-7.2.0/tests/test_mpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-04-26 20:10:50.000000 felupe-7.2.0/tests/test_planestrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-04-26 20:10:50.000000 felupe-7.2.0/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-04-26 20:10:50.000000 felupe-7.2.0/tests/test_quadrature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-04-26 20:10:50.000000 felupe-7.2.0/tests/test_readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-04-26 20:10:50.000000 felupe-7.2.0/tests/test_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-26 20:10:50.000000 felupe-7.2.0/tests/test_solve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-04-26 20:10:50.000000 felupe-7.2.0/tests/test_tools.py
```

### Comparing `felupe-7.1.0/LICENSE` & `felupe-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `felupe-7.1.0/PKG-INFO` & `felupe-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: felupe
-Version: 7.1.0
+Version: 7.2.0
 Summary: Finite Element Analysis
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -700,70 +700,86 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: all
 License-File: LICENSE
 
-# 🔍 FElupe - Finite Element Analysis
+# 🔍 FElupe
 
-[![PyPI version shields.io](https://img.shields.io/pypi/v/felupe.svg)](https://pypi.python.org/pypi/felupe/) [![Documentation Status](https://readthedocs.org/projects/felupe/badge/?version=latest)](https://felupe.readthedocs.io/en/latest/?badge=latest) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) ![Made with love in Graz (Austria)](https://img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20in-Graz%20(Austria)-0c674a) [![codecov](https://codecov.io/gh/adtzlr/felupe/branch/main/graph/badge.svg?token=J2QP6Y6LVH)](https://codecov.io/gh/adtzlr/felupe) [![DOI](https://zenodo.org/badge/360657894.svg)](https://zenodo.org/badge/latestdoi/360657894) ![Codestyle black](https://img.shields.io/badge/code%20style-black-black) ![GitHub Repo stars](https://img.shields.io/github/stars/adtzlr/felupe?logo=github) ![PyPI - Downloads](https://img.shields.io/pypi/dm/felupe)
+[![PyPI version shields.io](https://img.shields.io/pypi/v/felupe.svg)](https://pypi.python.org/pypi/felupe/) [![Documentation Status](https://readthedocs.org/projects/felupe/badge/?version=latest)](https://felupe.readthedocs.io/en/latest/?badge=latest) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) ![Made with love in Graz (Austria)](https://img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20in-Graz%20(Austria)-0c674a) [![codecov](https://codecov.io/gh/adtzlr/felupe/branch/main/graph/badge.svg?token=J2QP6Y6LVH)](https://codecov.io/gh/adtzlr/felupe) [![DOI](https://zenodo.org/badge/360657894.svg)](https://zenodo.org/badge/latestdoi/360657894) ![Codestyle black](https://img.shields.io/badge/code%20style-black-black) ![GitHub Repo stars](https://img.shields.io/github/stars/adtzlr/felupe?logo=github) ![PyPI - Downloads](https://img.shields.io/pypi/dm/felupe) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/adtzlr/felupe/HEAD) [![lite-badge](https://jupyterlite.rtfd.io/en/latest/_static/badge.svg)](https://adtzlr.github.io/felupe-web/lab?path=01_Getting+Started.ipynb) <a target="_blank" href="https://colab.research.google.com/github/adtzlr/felupe-web/blob/main/content/01_Getting%20Started.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
+
+> Finite Element Analysis
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/adtzlr/felupe/main/docs/_static/logo_light.svg" height="120px"/> <a href="https://felupe.readthedocs.io/en/latest/examples/rubberspring.html"><img src="https://user-images.githubusercontent.com/5793153/230604246-5a416081-6777-4f33-afdf-efdb51338722.png" height="120px"/></a> <a href="https://felupe.readthedocs.io/en/latest/examples/platewithhole.html"><img src="https://user-images.githubusercontent.com/5793153/230604587-42e3e339-e08c-4cc8-8000-f7046a8d95df.png" height="120px"/></a>
 </p>
 
 FElupe is a Python 3.7+ finite element analysis package focussing on the formulation and numerical solution of nonlinear problems in continuum mechanics of solid bodies. Its name is a combination of FE (finite element) and the german word *Lupe* (magnifying glass) as a synonym for getting an insight how a finite element analysis code looks like under the hood.
 
 # Installation
 Install Python, fire up a terminal and run
 
 ```shell
 pip install felupe[all]
 ```
 
-where `[all]` installs all optional dependencies. By default, FElupe depends on `numpy` and `scipy`. In order to make use of all features of FElupe, it is suggested to install all optional dependencies (`einsumt`, `h5py`, `matplotlib`, `meshio` and `tensortrax`).
+where `[all]` installs all optional dependencies. By default, FElupe depends on `numpy`, `scipy` and `tensortrax`. In order to make use of all features of FElupe, it is suggested to install all optional dependencies (`einsumt`, `h5py`, `matplotlib`, `meshio` and `pyvista`).
 
 # Getting Started
-A quarter model of a solid cube with hyperelastic material behaviour is subjected to a uniaxial elongation applied at a clamped end-face. This involves the creation of a mesh, a region as well as a displacement field (encapsulated in a field container). Furthermore, the boundary conditions are created by a template for a uniaxial loadcase. An isotropic pseudo-elastic Ogden-Roxburgh Mullins-softening model formulation in combination with an isotropic hyperelastic Neo-Hookean material formulation is applied on a nearly-incompressible solid body. A step generates the consecutive substep-movements of a given boundary condition. The step is further added to a list of steps of a job (here, a characteristic-curve job is used). During evaluation, each substep of each step is solved by an iterative Newton-Rhapson procedure. The solution is exported after each completed substep as a time-series XDMF file. For more details beside this high-level code snippet, please have a look at the [documentation](https://felupe.readthedocs.io/en/latest/?badge=latest).
+This tutorial covers the essential high-level parts of creating and solving problems with FElupe. As an introductory example, a quarter model of a solid cube with hyperelastic material behaviour is subjected to a uniaxial elongation applied at a clamped end-face. 
+
+First, let’s import FElupe and create a meshed cube out of hexahedron cells with 6 points per axis. A numeric region, pre-defined for hexahedrons, is created on the mesh. A vector-valued displacement field is initiated on the region. Next, a field container is created on top of this field. 
+
+A uniaxial load case is applied on the displacement field stored inside the field container. This involves setting up symmetry planes as well as the absolute value of the prescribed displacement at the mesh-points on the right-end face of the cube. The right-end face is *clamped*: only displacements in direction *x* are allowed. The dict of boundary conditions for this pre-defined load case are returned as `boundaries` and the partitioned degrees of freedom as well as the external displacements are stored within the returned dict `loadcase`. 
+
+An isotropic pseudo-elastic Ogden-Roxburgh Mullins-softening model formulation in combination with an isotropic hyperelastic Neo-Hookean material formulation is applied on the displacement field of a nearly-incompressible solid body. 
+
+A step generates the consecutive substep-movements of a given boundary condition. The step is further added to a list of steps of a job (here, a characteristic-curve job is used). During evaluation, each substep of each step is solved by an iterative Newton-Rhapson procedure. The solution is exported after each completed substep as a time-series XDMF file. Finally, the result of the last completed substep is plotted.
+
+For more details beside this high-level code snippet, please have a look at the [documentation](https://felupe.readthedocs.io/en/latest/?badge=latest).
 
 ```python
 import felupe as fem
 
 # create a hexahedron-region on a cube
-mesh = fem.Cube(n=11)
+mesh = fem.Cube(n=6)
 region = fem.RegionHexahedron(mesh)
 
 # add a field container (with a vector-valued displacement field)
 field = fem.FieldContainer([fem.Field(region, dim=3)])
 
 # apply a uniaxial elongation on the cube
-boundaries = fem.dof.uniaxial(field, clamped=True)[0]
+boundaries, loadcase = fem.dof.uniaxial(field, clamped=True)
 
 # define the constitutive material behaviour
 # and create a nearly-incompressible (u,p,J - formulation) solid body
 umat = fem.OgdenRoxburgh(material=fem.NeoHooke(mu=1), r=3, m=1, beta=0)
 solid = fem.SolidBodyNearlyIncompressible(umat, field, bulk=5000)
 
 # prepare a step with substeps
-move = fem.math.linsteps([0, 2, 0], num=10)
+move = fem.math.linsteps([0, 1, 0, 1, 2, 1], num=5)
 step = fem.Step(items=[solid], ramp={boundaries["move"]: move}, boundaries=boundaries)
 
 # add the step to a job, evaluate all substeps and create a plot
 job = fem.CharacteristicCurve(steps=[step], boundary=boundaries["move"])
 job.evaluate(filename="result.xdmf")
 fig, ax = job.plot(
     xlabel="Displacement $u$ in mm $\longrightarrow$",
     ylabel="Normal Force $F$ in N $\longrightarrow$",
 )
+
+# visualize the results
+view = fem.View(field)
+view.plot("Principal Values of Logarithmic Strain").show()
 ```
 
-https://user-images.githubusercontent.com/5793153/200951381-ea310e54-7623-4dd1-a55f-a28f9055063f.mp4
+![curve](https://user-images.githubusercontent.com/5793153/234382805-d9a56108-9dd7-4f57-a029-571a5a2486a4.svg)
 
-<img src="https://raw.githubusercontent.com/adtzlr/felupe/main/docs/_static/readme_characteristic_curve.svg" width="600px"/>
+![cube](https://user-images.githubusercontent.com/5793153/234405093-2f5201c1-3bba-46ee-bd91-af87813609d9.png)
 
 # Documentation
 The documentation is located [here](https://felupe.readthedocs.io/en/latest/?badge=latest).
 
 # Extension Packages
 The capabilities of FElupe may be enhanced with extension packages created by the community.
```

### Comparing `felupe-7.1.0/README.md` & `felupe-7.2.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,63 +1,79 @@
-# 🔍 FElupe - Finite Element Analysis
+# 🔍 FElupe
 
-[![PyPI version shields.io](https://img.shields.io/pypi/v/felupe.svg)](https://pypi.python.org/pypi/felupe/) [![Documentation Status](https://readthedocs.org/projects/felupe/badge/?version=latest)](https://felupe.readthedocs.io/en/latest/?badge=latest) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) ![Made with love in Graz (Austria)](https://img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20in-Graz%20(Austria)-0c674a) [![codecov](https://codecov.io/gh/adtzlr/felupe/branch/main/graph/badge.svg?token=J2QP6Y6LVH)](https://codecov.io/gh/adtzlr/felupe) [![DOI](https://zenodo.org/badge/360657894.svg)](https://zenodo.org/badge/latestdoi/360657894) ![Codestyle black](https://img.shields.io/badge/code%20style-black-black) ![GitHub Repo stars](https://img.shields.io/github/stars/adtzlr/felupe?logo=github) ![PyPI - Downloads](https://img.shields.io/pypi/dm/felupe)
+[![PyPI version shields.io](https://img.shields.io/pypi/v/felupe.svg)](https://pypi.python.org/pypi/felupe/) [![Documentation Status](https://readthedocs.org/projects/felupe/badge/?version=latest)](https://felupe.readthedocs.io/en/latest/?badge=latest) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) ![Made with love in Graz (Austria)](https://img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20in-Graz%20(Austria)-0c674a) [![codecov](https://codecov.io/gh/adtzlr/felupe/branch/main/graph/badge.svg?token=J2QP6Y6LVH)](https://codecov.io/gh/adtzlr/felupe) [![DOI](https://zenodo.org/badge/360657894.svg)](https://zenodo.org/badge/latestdoi/360657894) ![Codestyle black](https://img.shields.io/badge/code%20style-black-black) ![GitHub Repo stars](https://img.shields.io/github/stars/adtzlr/felupe?logo=github) ![PyPI - Downloads](https://img.shields.io/pypi/dm/felupe) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/adtzlr/felupe/HEAD) [![lite-badge](https://jupyterlite.rtfd.io/en/latest/_static/badge.svg)](https://adtzlr.github.io/felupe-web/lab?path=01_Getting+Started.ipynb) <a target="_blank" href="https://colab.research.google.com/github/adtzlr/felupe-web/blob/main/content/01_Getting%20Started.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
+
+> Finite Element Analysis
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/adtzlr/felupe/main/docs/_static/logo_light.svg" height="120px"/> <a href="https://felupe.readthedocs.io/en/latest/examples/rubberspring.html"><img src="https://user-images.githubusercontent.com/5793153/230604246-5a416081-6777-4f33-afdf-efdb51338722.png" height="120px"/></a> <a href="https://felupe.readthedocs.io/en/latest/examples/platewithhole.html"><img src="https://user-images.githubusercontent.com/5793153/230604587-42e3e339-e08c-4cc8-8000-f7046a8d95df.png" height="120px"/></a>
 </p>
 
 FElupe is a Python 3.7+ finite element analysis package focussing on the formulation and numerical solution of nonlinear problems in continuum mechanics of solid bodies. Its name is a combination of FE (finite element) and the german word *Lupe* (magnifying glass) as a synonym for getting an insight how a finite element analysis code looks like under the hood.
 
 # Installation
 Install Python, fire up a terminal and run
 
 ```shell
 pip install felupe[all]
 ```
 
-where `[all]` installs all optional dependencies. By default, FElupe depends on `numpy` and `scipy`. In order to make use of all features of FElupe, it is suggested to install all optional dependencies (`einsumt`, `h5py`, `matplotlib`, `meshio` and `tensortrax`).
+where `[all]` installs all optional dependencies. By default, FElupe depends on `numpy`, `scipy` and `tensortrax`. In order to make use of all features of FElupe, it is suggested to install all optional dependencies (`einsumt`, `h5py`, `matplotlib`, `meshio` and `pyvista`).
 
 # Getting Started
-A quarter model of a solid cube with hyperelastic material behaviour is subjected to a uniaxial elongation applied at a clamped end-face. This involves the creation of a mesh, a region as well as a displacement field (encapsulated in a field container). Furthermore, the boundary conditions are created by a template for a uniaxial loadcase. An isotropic pseudo-elastic Ogden-Roxburgh Mullins-softening model formulation in combination with an isotropic hyperelastic Neo-Hookean material formulation is applied on a nearly-incompressible solid body. A step generates the consecutive substep-movements of a given boundary condition. The step is further added to a list of steps of a job (here, a characteristic-curve job is used). During evaluation, each substep of each step is solved by an iterative Newton-Rhapson procedure. The solution is exported after each completed substep as a time-series XDMF file. For more details beside this high-level code snippet, please have a look at the [documentation](https://felupe.readthedocs.io/en/latest/?badge=latest).
+This tutorial covers the essential high-level parts of creating and solving problems with FElupe. As an introductory example, a quarter model of a solid cube with hyperelastic material behaviour is subjected to a uniaxial elongation applied at a clamped end-face. 
+
+First, let’s import FElupe and create a meshed cube out of hexahedron cells with 6 points per axis. A numeric region, pre-defined for hexahedrons, is created on the mesh. A vector-valued displacement field is initiated on the region. Next, a field container is created on top of this field. 
+
+A uniaxial load case is applied on the displacement field stored inside the field container. This involves setting up symmetry planes as well as the absolute value of the prescribed displacement at the mesh-points on the right-end face of the cube. The right-end face is *clamped*: only displacements in direction *x* are allowed. The dict of boundary conditions for this pre-defined load case are returned as `boundaries` and the partitioned degrees of freedom as well as the external displacements are stored within the returned dict `loadcase`. 
+
+An isotropic pseudo-elastic Ogden-Roxburgh Mullins-softening model formulation in combination with an isotropic hyperelastic Neo-Hookean material formulation is applied on the displacement field of a nearly-incompressible solid body. 
+
+A step generates the consecutive substep-movements of a given boundary condition. The step is further added to a list of steps of a job (here, a characteristic-curve job is used). During evaluation, each substep of each step is solved by an iterative Newton-Rhapson procedure. The solution is exported after each completed substep as a time-series XDMF file. Finally, the result of the last completed substep is plotted.
+
+For more details beside this high-level code snippet, please have a look at the [documentation](https://felupe.readthedocs.io/en/latest/?badge=latest).
 
 ```python
 import felupe as fem
 
 # create a hexahedron-region on a cube
-mesh = fem.Cube(n=11)
+mesh = fem.Cube(n=6)
 region = fem.RegionHexahedron(mesh)
 
 # add a field container (with a vector-valued displacement field)
 field = fem.FieldContainer([fem.Field(region, dim=3)])
 
 # apply a uniaxial elongation on the cube
-boundaries = fem.dof.uniaxial(field, clamped=True)[0]
+boundaries, loadcase = fem.dof.uniaxial(field, clamped=True)
 
 # define the constitutive material behaviour
 # and create a nearly-incompressible (u,p,J - formulation) solid body
 umat = fem.OgdenRoxburgh(material=fem.NeoHooke(mu=1), r=3, m=1, beta=0)
 solid = fem.SolidBodyNearlyIncompressible(umat, field, bulk=5000)
 
 # prepare a step with substeps
-move = fem.math.linsteps([0, 2, 0], num=10)
+move = fem.math.linsteps([0, 1, 0, 1, 2, 1], num=5)
 step = fem.Step(items=[solid], ramp={boundaries["move"]: move}, boundaries=boundaries)
 
 # add the step to a job, evaluate all substeps and create a plot
 job = fem.CharacteristicCurve(steps=[step], boundary=boundaries["move"])
 job.evaluate(filename="result.xdmf")
 fig, ax = job.plot(
     xlabel="Displacement $u$ in mm $\longrightarrow$",
     ylabel="Normal Force $F$ in N $\longrightarrow$",
 )
+
+# visualize the results
+view = fem.View(field)
+view.plot("Principal Values of Logarithmic Strain").show()
 ```
 
-https://user-images.githubusercontent.com/5793153/200951381-ea310e54-7623-4dd1-a55f-a28f9055063f.mp4
+![curve](https://user-images.githubusercontent.com/5793153/234382805-d9a56108-9dd7-4f57-a029-571a5a2486a4.svg)
 
-<img src="https://raw.githubusercontent.com/adtzlr/felupe/main/docs/_static/readme_characteristic_curve.svg" width="600px"/>
+![cube](https://user-images.githubusercontent.com/5793153/234405093-2f5201c1-3bba-46ee-bd91-af87813609d9.png)
 
 # Documentation
 The documentation is located [here](https://felupe.readthedocs.io/en/latest/?badge=latest).
 
 # Extension Packages
 The capabilities of FElupe may be enhanced with extension packages created by the community.
```

#### html2text {}

```diff
@@ -1,81 +1,98 @@
-# ð FElupe - Finite Element Analysis [![PyPI version shields.io](https://
-img.shields.io/pypi/v/felupe.svg)](https://pypi.python.org/pypi/felupe/) [!
-[Documentation Status](https://readthedocs.org/projects/felupe/badge/
-?version=latest)](https://felupe.readthedocs.io/en/latest/?badge=latest) [!
-[License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https:/
-/www.gnu.org/licenses/gpl-3.0) ![Made with love in Graz (Austria)](https://
-img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20in-Graz%20(Austria)-
-0c674a) [![codecov](https://codecov.io/gh/adtzlr/felupe/branch/main/graph/
+# ð FElupe [![PyPI version shields.io](https://img.shields.io/pypi/v/
+felupe.svg)](https://pypi.python.org/pypi/felupe/) [![Documentation Status]
+(https://readthedocs.org/projects/felupe/badge/?version=latest)](https://
+felupe.readthedocs.io/en/latest/?badge=latest) [![License: GPL v3](https://
+img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-
+3.0) ![Made with love in Graz (Austria)](https://img.shields.io/badge/
+Made%20with%20%E2%9D%A4%EF%B8%8F%20in-Graz%20(Austria)-0c674a) [![codecov]
+(https://codecov.io/gh/adtzlr/felupe/branch/main/graph/
 badge.svg?token=J2QP6Y6LVH)](https://codecov.io/gh/adtzlr/felupe) [![DOI]
 (https://zenodo.org/badge/360657894.svg)](https://zenodo.org/badge/latestdoi/
 360657894) ![Codestyle black](https://img.shields.io/badge/code%20style-black-
 black) ![GitHub Repo stars](https://img.shields.io/github/stars/adtzlr/
 felupe?logo=github) ![PyPI - Downloads](https://img.shields.io/pypi/dm/felupe)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/
+adtzlr/felupe/HEAD) [![lite-badge](https://jupyterlite.rtfd.io/en/latest/
+_static/badge.svg)](https://adtzlr.github.io/felupe-web/
+lab?path=01_Getting+Started.ipynb) [Open_In_Colab] > Finite Element Analysis
       [https://raw.githubusercontent.com/adtzlr/felupe/main/docs/_static/
  logo_light.svg] [https://user-images.githubusercontent.com/5793153/230604246-
            5a416081-6777-4f33-afdf-efdb51338722.png] [https://user-
     images.githubusercontent.com/5793153/230604587-42e3e339-e08c-4cc8-8000-
                                f7046a8d95df.png]
 FElupe is a Python 3.7+ finite element analysis package focussing on the
 formulation and numerical solution of nonlinear problems in continuum mechanics
 of solid bodies. Its name is a combination of FE (finite element) and the
 german word *Lupe* (magnifying glass) as a synonym for getting an insight how a
 finite element analysis code looks like under the hood. # Installation Install
 Python, fire up a terminal and run ```shell pip install felupe[all] ``` where `
 [all]` installs all optional dependencies. By default, FElupe depends on
-`numpy` and `scipy`. In order to make use of all features of FElupe, it is
-suggested to install all optional dependencies (`einsumt`, `h5py`,
-`matplotlib`, `meshio` and `tensortrax`). # Getting Started A quarter model of
-a solid cube with hyperelastic material behaviour is subjected to a uniaxial
-elongation applied at a clamped end-face. This involves the creation of a mesh,
-a region as well as a displacement field (encapsulated in a field container).
-Furthermore, the boundary conditions are created by a template for a uniaxial
-loadcase. An isotropic pseudo-elastic Ogden-Roxburgh Mullins-softening model
+`numpy`, `scipy` and `tensortrax`. In order to make use of all features of
+FElupe, it is suggested to install all optional dependencies (`einsumt`,
+`h5py`, `matplotlib`, `meshio` and `pyvista`). # Getting Started This tutorial
+covers the essential high-level parts of creating and solving problems with
+FElupe. As an introductory example, a quarter model of a solid cube with
+hyperelastic material behaviour is subjected to a uniaxial elongation applied
+at a clamped end-face. First, letâs import FElupe and create a meshed cube
+out of hexahedron cells with 6 points per axis. A numeric region, pre-defined
+for hexahedrons, is created on the mesh. A vector-valued displacement field is
+initiated on the region. Next, a field container is created on top of this
+field. A uniaxial load case is applied on the displacement field stored inside
+the field container. This involves setting up symmetry planes as well as the
+absolute value of the prescribed displacement at the mesh-points on the right-
+end face of the cube. The right-end face is *clamped*: only displacements in
+direction *x* are allowed. The dict of boundary conditions for this pre-defined
+load case are returned as `boundaries` and the partitioned degrees of freedom
+as well as the external displacements are stored within the returned dict
+`loadcase`. An isotropic pseudo-elastic Ogden-Roxburgh Mullins-softening model
 formulation in combination with an isotropic hyperelastic Neo-Hookean material
-formulation is applied on a nearly-incompressible solid body. A step generates
-the consecutive substep-movements of a given boundary condition. The step is
-further added to a list of steps of a job (here, a characteristic-curve job is
-used). During evaluation, each substep of each step is solved by an iterative
-Newton-Rhapson procedure. The solution is exported after each completed substep
-as a time-series XDMF file. For more details beside this high-level code
-snippet, please have a look at the [documentation](https://
+formulation is applied on the displacement field of a nearly-incompressible
+solid body. A step generates the consecutive substep-movements of a given
+boundary condition. The step is further added to a list of steps of a job
+(here, a characteristic-curve job is used). During evaluation, each substep of
+each step is solved by an iterative Newton-Rhapson procedure. The solution is
+exported after each completed substep as a time-series XDMF file. Finally, the
+result of the last completed substep is plotted. For more details beside this
+high-level code snippet, please have a look at the [documentation](https://
 felupe.readthedocs.io/en/latest/?badge=latest). ```python import felupe as fem
-# create a hexahedron-region on a cube mesh = fem.Cube(n=11) region =
+# create a hexahedron-region on a cube mesh = fem.Cube(n=6) region =
 fem.RegionHexahedron(mesh) # add a field container (with a vector-valued
 displacement field) field = fem.FieldContainer([fem.Field(region, dim=3)]) #
-apply a uniaxial elongation on the cube boundaries = fem.dof.uniaxial(field,
-clamped=True)[0] # define the constitutive material behaviour # and create a
-nearly-incompressible (u,p,J - formulation) solid body umat = fem.OgdenRoxburgh
-(material=fem.NeoHooke(mu=1), r=3, m=1, beta=0) solid =
+apply a uniaxial elongation on the cube boundaries, loadcase = fem.dof.uniaxial
+(field, clamped=True) # define the constitutive material behaviour # and create
+a nearly-incompressible (u,p,J - formulation) solid body umat =
+fem.OgdenRoxburgh(material=fem.NeoHooke(mu=1), r=3, m=1, beta=0) solid =
 fem.SolidBodyNearlyIncompressible(umat, field, bulk=5000) # prepare a step with
-substeps move = fem.math.linsteps([0, 2, 0], num=10) step = fem.Step(items=
-[solid], ramp={boundaries["move"]: move}, boundaries=boundaries) # add the step
-to a job, evaluate all substeps and create a plot job = fem.CharacteristicCurve
-(steps=[step], boundary=boundaries["move"]) job.evaluate
+substeps move = fem.math.linsteps([0, 1, 0, 1, 2, 1], num=5) step = fem.Step
+(items=[solid], ramp={boundaries["move"]: move}, boundaries=boundaries) # add
+the step to a job, evaluate all substeps and create a plot job =
+fem.CharacteristicCurve(steps=[step], boundary=boundaries["move"]) job.evaluate
 (filename="result.xdmf") fig, ax = job.plot( xlabel="Displacement $u$ in mm
-$\longrightarrow$", ylabel="Normal Force $F$ in N $\longrightarrow$", ) ```
-https://user-images.githubusercontent.com/5793153/200951381-ea310e54-7623-4dd1-
-a55f-a28f9055063f.mp4 [https://raw.githubusercontent.com/adtzlr/felupe/main/
-docs/_static/readme_characteristic_curve.svg] # Documentation The documentation
-is located [here](https://felupe.readthedocs.io/en/latest/?badge=latest). #
-Extension Packages The capabilities of FElupe may be enhanced with extension
-packages created by the community. | **Package** | **Description** | **Link** |
-|:-----------:|:-------------------------------------------------------:|:-----
---------------------------------:| | tensortrax | Math on (Hyper-Dual) Tensors
-with Trailing Axes | https://github.com/adtzlr/tensortrax | | matADi | Material
-Definition with Automatic Differentiation (AD) | https://github.com/adtzlr/
-matadi | | FEplot | A visualization tool for FElupe | https://github.com/
-ZAARAOUI999/feplot | # Changelog All notable changes to this project will be
-documented in [this file](CHANGELOG.md). The format is based on [Keep a
-Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to
-[Semantic Versioning](https://semver.org/spec/v2.0.0.html). # License FElupe -
-finite element analysis (C) 2023 Andreas Dutzler, Graz (Austria). This program
-is free software: you can redistribute it and/or modify it under the terms of
-the GNU General Public License as published by the Free Software Foundation,
-either version 3 of the License, or (at your option) any later version. This
-program is distributed in the hope that it will be useful, but WITHOUT ANY
-WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
-PARTICULAR PURPOSE. See the GNU General Public License for more details. You
-should have received a copy of the GNU General Public License along with this
-program. If not, see
+$\longrightarrow$", ylabel="Normal Force $F$ in N $\longrightarrow$", ) #
+visualize the results view = fem.View(field) view.plot("Principal Values of
+Logarithmic Strain").show() ``` ![curve](https://user-
+images.githubusercontent.com/5793153/234382805-d9a56108-9dd7-4f57-a029-
+571a5a2486a4.svg) ![cube](https://user-images.githubusercontent.com/5793153/
+234405093-2f5201c1-3bba-46ee-bd91-af87813609d9.png) # Documentation The
+documentation is located [here](https://felupe.readthedocs.io/en/latest/
+?badge=latest). # Extension Packages The capabilities of FElupe may be enhanced
+with extension packages created by the community. | **Package** |
+**Description** | **Link** | |:-----------:|:----------------------------------
+---------------------:|:-------------------------------------:| | tensortrax |
+Math on (Hyper-Dual) Tensors with Trailing Axes | https://github.com/adtzlr/
+tensortrax | | matADi | Material Definition with Automatic Differentiation (AD)
+| https://github.com/adtzlr/matadi | | FEplot | A visualization tool for FElupe
+| https://github.com/ZAARAOUI999/feplot | # Changelog All notable changes to
+this project will be documented in [this file](CHANGELOG.md). The format is
+based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this
+project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
+# License FElupe - finite element analysis (C) 2023 Andreas Dutzler, Graz
+(Austria). This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by the Free
+Software Foundation, either version 3 of the License, or (at your option) any
+later version. This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY
+or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for
+more details. You should have received a copy of the GNU General Public License
+along with this program. If not, see
 www.gnu.org/licenses/>.
```

### Comparing `felupe-7.1.0/pyproject.toml` & `felupe-7.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -40,28 +40,31 @@
   "Topic :: Utilities"
 ]
 dynamic = ["version"]
 requires-python = ">=3.7"
 dependencies = [
   "numpy",
   "scipy",
+  "tensortrax",
 ]
 
 [project.optional-dependencies]
 test = [
     "h5py",
     "matplotlib",
     "meshio",
+    "pyvista",
     "tensortrax",
 ]
 all = [
     "einsumt",
     "h5py",
     "matplotlib",
     "meshio",
+    "pyvista",
     "tensortrax",
 ]
 
 [tool.setuptools.dynamic]
 version = {attr = "felupe.__about__.__version__"}
 
 [project.urls]
```

### Comparing `felupe-7.1.0/src/felupe/_assembly/_axi.py` & `felupe-7.2.0/src/felupe/_assembly/_axi.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 
 from .._field._axi import FieldAxisymmetric
 from .._field._base import Field
 from ._base import IntegralForm
```

### Comparing `felupe-7.1.0/src/felupe/_assembly/_base.py` & `felupe-7.2.0/src/felupe/_assembly/_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 
 try:
     from einsumt import einsumt
 except ModuleNotFoundError:
```

### Comparing `felupe-7.1.0/src/felupe/_assembly/_form.py` & `felupe-7.2.0/src/felupe/_assembly/_form.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,30 @@
 # -*- coding: utf-8 -*-
 """
-Created on Tue Jan  4 17:26:08 2022
+This file is part of FElupe.
 
-@author: adutz
-"""
-# -*- coding: utf-8 -*-
-"""
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
-
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 from threading import Thread
 
 import numpy as np
 
-from .._basis import Basis, BasisMixed
-from .._field import Field
-from .._field import FieldContainer as FieldMixed
+from .._basis import BasisMixed
 from ._base import IntegralForm
 from ._mixed import IntegralFormMixed
 
 
 class LinearForm:
     r"""A linear form object with methods for integration and assembly of
     vectors.
@@ -536,16 +519,16 @@
         Flag to use the gradient of ``u``.
     dx : ndarray or None, optional (default is None)
         Array with (numerical) differential volumes.
     args : tuple, optional (default is ())
         Tuple with initial optional weakform-arguments. May be updated during
         integration / assembly.
     kwargs : dict, optional (default is {})
-        Dictionary with initial optional weakform-keyword-arguments. May be updated during
-        integration / assembly.
+        Dictionary with initial optional weakform-keyword-arguments. May be updated
+        during integration / assembly.
     parallel : bool, optional (default is False)
         Flag to activate parallel (threaded) basis evaluation.
 
     """
 
     def __init__(
         self,
```

### Comparing `felupe-7.1.0/src/felupe/_assembly/_mixed.py` & `felupe-7.2.0/src/felupe/_assembly/_mixed.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 from scipy.sparse import bmat, vstack
 
 from .._field._axi import FieldAxisymmetric
 from .._field._base import Field
```

### Comparing `felupe-7.1.0/src/felupe/_basis/_basis.py` & `felupe-7.2.0/src/felupe/_basis/_basis.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 
 try:
     from einsumt import einsumt
 except ModuleNotFoundError:
```

### Comparing `felupe-7.1.0/src/felupe/_field/_axi.py` & `felupe-7.2.0/src/felupe/_field/_planestrain.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,83 +1,61 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 
 from ..math import sym as symmetric
 from ._base import Field
 
 
-class FieldAxisymmetric(Field):
-    r"""A axisymmetric Field on points of a two-dimensional
+class FieldPlaneStrain(Field):
+    r"""A plane strain Field on points of a two-dimensional
     `region` with dimension `dim` (default is 2) and initial point
     `values` (default is 0).
-    
-    * component 1 =  axial component
-    * component 2 = radial component
-    
-    ..  code-block::
-        
-         x_2 (radial direction)
-        
-          ^
-          |        _
-          |       / \
-        --|-----------------> x_1 (axial rotation axis)
-                  \_^
-    
+
     This is a modified :class:`Field` class in which the radial coordinates
     are evaluated at the numeric integration points. The :meth:`grad`-method is
     modified in such a way that it does not only contain the in-plane
     2d-gradient but also the circumferential stretch as shown in Eq.(1).
-    
+
     ..  code-block::
 
-                    |  dudX(2d) :   0   |
-        dudX(axi) = | ..................|                  (1)
-                    |     0     : u_r/R |
+                            |  dudX(2d) :   0   |
+        dudX(planestrain) = | ..................|                  (1)
+                            |     0     :   0   |
 
     Attributes
     ----------
     region : Region
         The region on which the field will be created.
     dim : int (default is 2)
         The dimension of the field.
     values : float (default is 0.0) or array
         A single value for all components of the field or an array of
         shape (region.mesh.npoints, dim)`.
 
     """
 
     def __init__(self, region, dim=2, values=0):
-        """A continous axisymmetric Field on points of a two-dimensional
+        """A plane strain Field on points of a two-dimensional
         `region` with dimension `dim` (default is 2) and initial point
         `values` (default is 0).
 
         Attributes
         ----------
         region : Region
             The region on which the field will be created.
@@ -87,21 +65,14 @@
             A single value for all components of the field or an array of
             shape (region.mesh.npoints, dim)`.
         """
 
         # init base Field
         super().__init__(region, dim=dim, values=values)
 
-        # create scalar-valued field of radial point values
-        self.scalar = Field(region, dim=1, values=region.mesh.points[:, 1])
-
-        # interpolate radial point values to integration points of each cell
-        # in the region
-        self.radius = self.scalar.interpolate()
-
     def _interpolate_2d(self):
         """Interpolate 2D field values at points and evaluate them at the
         integration points of all cells in the region."""
 
         # interpolated field values "aI"
         # evaluated at quadrature point "p"
         # for cell "c"
@@ -150,17 +121,17 @@
         """3D-gradient as partial derivative of field values at points w.r.t.
         the undeformed coordinates, evaluated at the integration points of all
         cells in the region. Optionally, the symmetric part of the gradient is
         returned.
 
         ..  code-block::
 
-                        |  dudX(2d) :   0   |
-            dudX(axi) = | ..................|
-                        |     0     : u_r/R |
+                                |  dudX(2d) :   0   |
+            dudX(planestrain) = | ..................|
+                                |     0     :   0   |
 
         Arguments
         ---------
         sym : bool, optional (default is False)
             Calculate the symmetric part of the gradient.
 
         Returns
@@ -170,11 +141,8 @@
             w.r.t. undeformed coordinates, evaluated at the integration points
             of all cells in the region.
         """
 
         # extend dimension of in-plane 2d-gradient
         g = np.pad(self._grad_2d(sym=sym), ((0, 1), (0, 1), (0, 0), (0, 0)))
 
-        # set dudX_33 = u_r / R
-        g[-1, -1] = self.interpolate()[1] / self.radius
-
         return g
```

### Comparing `felupe-7.1.0/src/felupe/_field/_base.py` & `felupe-7.2.0/src/felupe/_field/_base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 from copy import deepcopy
 
 import numpy as np
 
 from ..math import identity
```

### Comparing `felupe-7.1.0/src/felupe/_field/_container.py` & `felupe-7.2.0/src/felupe/_field/_container.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,23 @@
+# -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 from copy import deepcopy
 
 import numpy as np
```

### Comparing `felupe-7.1.0/src/felupe/_field/_fields.py` & `felupe-7.2.0/src/felupe/_field/_fields.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,23 @@
+# -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 from ..region._templates import (
     RegionBiQuadraticQuad,
     RegionConstantHexahedron,
     RegionConstantQuad,
     RegionHexahedron,
```

### Comparing `felupe-7.1.0/src/felupe/_field/_indices.py` & `felupe-7.2.0/tests/test_basis.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,9 @@
 # -*- coding: utf-8 -*-
 """
-Created on Thu Apr 29 18:29:15 2021
-
-@author: adutz
-"""
-# -*- coding: utf-8 -*-
-"""
  _______  _______  ___      __   __  _______  _______ 
 |       ||       ||   |    |  | |  ||       ||       |
 |    ___||    ___||   |    |  | |  ||    _  ||    ___|
 |   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
 |    ___||    ___||   |___ |       ||    ___||    ___|
 |   |    |   |___ |       ||       ||   |    |   |___ 
 |___|    |_______||_______||_______||___|    |_______|
@@ -28,17 +22,55 @@
 
 You should have received a copy of the GNU General Public License
 along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
 
 """
 
 import numpy as np
+import pytest
+
+import felupe as fe
+
+
+def pre(dim):
+
+    m = fe.Cube(n=3)
+    r = fe.RegionHexahedron(m)
+    u = fe.FieldContainer([fe.Field(r, dim=dim)])
+    return r, u
+
+
+def pre_constant(dim):
+
+    m = fe.Cube(n=3)
+    r = fe.RegionConstantHexahedron(m)
+    u = fe.FieldContainer([fe.Field(r, dim=dim)])
+    return r, u
+
+
+def test_basis():
+
+    for parallel in [False, True]:
+
+        r, u = pre(dim=3)
+        b = fe.Basis(u, parallel=parallel)
+
+        assert b[0].grad is not None
+
+        r, u = pre(dim=1)
+        b = fe.Basis(u, parallel=parallel)
+
+        assert b[0].grad is not None
+
+        r, u = pre_constant(dim=3)
+        b = fe.Basis(u, parallel=parallel)
+
+        assert b[0].grad is None
+
+        r, u = pre_constant(dim=1)
+        b = fe.Basis(u, parallel=parallel)
+
+        assert b[0].grad is None
 
 
-class Indices:
-    def __init__(self, eai, ai, region, dim):
-        """Indices for cell "e", point "a" and component "i"."""
-
-        self.eai = eai
-        self.ai = ai
-        self.dof = np.arange(region.mesh.npoints * dim).reshape(-1, dim)
-        self.shape = (region.mesh.npoints * dim, 1)
+if __name__ == "__main__":
+    test_basis()
```

### Comparing `felupe-7.1.0/src/felupe/_field/_planestrain.py` & `felupe-7.2.0/src/felupe/_field/_axi.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,70 +1,74 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 
 from ..math import sym as symmetric
 from ._base import Field
 
 
-class FieldPlaneStrain(Field):
-    r"""A plane strain Field on points of a two-dimensional
+class FieldAxisymmetric(Field):
+    r"""A axisymmetric Field on points of a two-dimensional
     `region` with dimension `dim` (default is 2) and initial point
     `values` (default is 0).
 
+    * component 1 =  axial component
+    * component 2 = radial component
+
+    ..  code-block::
+
+         x_2 (radial direction)
+
+          ^
+          |        _
+          |       / \
+        --|-----------------> x_1 (axial rotation axis)
+                  \_^
+
     This is a modified :class:`Field` class in which the radial coordinates
     are evaluated at the numeric integration points. The :meth:`grad`-method is
     modified in such a way that it does not only contain the in-plane
     2d-gradient but also the circumferential stretch as shown in Eq.(1).
 
     ..  code-block::
 
-                            |  dudX(2d) :   0   |
-        dudX(planestrain) = | ..................|                  (1)
-                            |     0     :   0   |
+                    |  dudX(2d) :   0   |
+        dudX(axi) = | ..................|                  (1)
+                    |     0     : u_r/R |
 
     Attributes
     ----------
     region : Region
         The region on which the field will be created.
     dim : int (default is 2)
         The dimension of the field.
     values : float (default is 0.0) or array
         A single value for all components of the field or an array of
         shape (region.mesh.npoints, dim)`.
 
     """
 
     def __init__(self, region, dim=2, values=0):
-        """A plane strain Field on points of a two-dimensional
+        """A continous axisymmetric Field on points of a two-dimensional
         `region` with dimension `dim` (default is 2) and initial point
         `values` (default is 0).
 
         Attributes
         ----------
         region : Region
             The region on which the field will be created.
@@ -74,14 +78,21 @@
             A single value for all components of the field or an array of
             shape (region.mesh.npoints, dim)`.
         """
 
         # init base Field
         super().__init__(region, dim=dim, values=values)
 
+        # create scalar-valued field of radial point values
+        self.scalar = Field(region, dim=1, values=region.mesh.points[:, 1])
+
+        # interpolate radial point values to integration points of each cell
+        # in the region
+        self.radius = self.scalar.interpolate()
+
     def _interpolate_2d(self):
         """Interpolate 2D field values at points and evaluate them at the
         integration points of all cells in the region."""
 
         # interpolated field values "aI"
         # evaluated at quadrature point "p"
         # for cell "c"
@@ -130,17 +141,17 @@
         """3D-gradient as partial derivative of field values at points w.r.t.
         the undeformed coordinates, evaluated at the integration points of all
         cells in the region. Optionally, the symmetric part of the gradient is
         returned.
 
         ..  code-block::
 
-                                |  dudX(2d) :   0   |
-            dudX(planestrain) = | ..................|
-                                |     0     :   0   |
+                        |  dudX(2d) :   0   |
+            dudX(axi) = | ..................|
+                        |     0     : u_r/R |
 
         Arguments
         ---------
         sym : bool, optional (default is False)
             Calculate the symmetric part of the gradient.
 
         Returns
@@ -150,8 +161,11 @@
             w.r.t. undeformed coordinates, evaluated at the integration points
             of all cells in the region.
         """
 
         # extend dimension of in-plane 2d-gradient
         g = np.pad(self._grad_2d(sym=sym), ((0, 1), (0, 1), (0, 0), (0, 0)))
 
+        # set dudX_33 = u_r / R
+        g[-1, -1] = self.interpolate()[1] / self.radius
+
         return g
```

### Comparing `felupe-7.1.0/src/felupe/constitution/_kinematics.py` & `felupe-7.2.0/src/felupe/constitution/_kinematics.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 
 try:
     from einsumt import einsumt
 except ModuleNotFoundError:
@@ -42,15 +33,16 @@
 
        d\boldsymbol{x} = \boldsymbol{F} d\boldsymbol{X}
 
     Gradient:
 
     .. math::
 
-       \frac{\partial \boldsymbol{F}}{\partial \boldsymbol{F}} = \boldsymbol{I} \overset{ik}{\otimes} \boldsymbol{I}
+       \frac{\partial \boldsymbol{F}}{\partial \boldsymbol{F}} =
+       \boldsymbol{I} \overset{ik}{\otimes} \boldsymbol{I}
     """
 
     def __init__(self, parallel=False):
         self.parallel = parallel
 
     def function(self, extract):
         """Line change.
@@ -99,15 +91,17 @@
 
        d\boldsymbol{a} = J \boldsymbol{F}^{-T} d\boldsymbol{A}
 
     Gradient:
 
     .. math::
 
-       \frac{\partial J \boldsymbol{F}^{-T}}{\partial \boldsymbol{F}} = J \left( \boldsymbol{F}^{-T} \otimes \boldsymbol{F}^{-T} - \boldsymbol{F}^{-T} \overset{il}{\otimes} \boldsymbol{F}^{-T} \right)
+       \frac{\partial J \boldsymbol{F}^{-T}}{\partial \boldsymbol{F}} =
+       J \left( \boldsymbol{F}^{-T} \otimes \boldsymbol{F}^{-T}
+       - \boldsymbol{F}^{-T} \overset{il}{\otimes} \boldsymbol{F}^{-T} \right)
 
     """
 
     def __init__(self, parallel=False):
         self.parallel = parallel
 
     def function(self, extract, N=None, parallel=None):
@@ -134,15 +128,15 @@
 
         if parallel is None:
             parallel = self.parallel
 
         if N is None:
             return [Fs]
         else:
-            return [dot(Fs, N, parallel=parallel)]
+            return [dot(Fs, N, mode=(2, 1), parallel=parallel)]
 
     def gradient(self, extract, N=None, parallel=None):
         """Gradient of area change.
 
         Arguments
         ---------
         extract : list of ndarray
@@ -188,15 +182,17 @@
 
     Gradient and hessian (equivalent to gradient of area change):
 
     .. math::
 
        \frac{\partial J}{\partial \boldsymbol{F}} &= J \boldsymbol{F}^{-T}
 
-       \frac{\partial^2 J}{\partial \boldsymbol{F}\ \partial \boldsymbol{F}} &= J \left( \boldsymbol{F}^{-T} \otimes \boldsymbol{F}^{-T} - \boldsymbol{F}^{-T} \overset{il}{\otimes} \boldsymbol{F}^{-T} \right)
+       \frac{\partial^2 J}{\partial \boldsymbol{F}\ \partial \boldsymbol{F}} &=
+       J \left( \boldsymbol{F}^{-T} \otimes \boldsymbol{F}^{-T} -
+       \boldsymbol{F}^{-T} \overset{il}{\otimes} \boldsymbol{F}^{-T} \right)
 
     """
 
     def __init__(self, parallel=False):
         self.parallel = parallel
 
     def function(self, extract):
```

### Comparing `felupe-7.1.0/src/felupe/constitution/_mixed.py` & `felupe-7.2.0/src/felupe/constitution/_mixed.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 
 from ..math import cdya_ik, cdya_il, ddot, det, dya, identity, inv, transpose
 
 
@@ -44,83 +35,128 @@
     energy density function in terms of a determinant-modified deformation
     gradient and an additional control equation.
 
     ..  math::
 
         \Pi &= \Pi_{int} + \Pi_{ext}
 
-        \Pi_{int} &= \int_V \psi(\boldsymbol{F}) \ dV \qquad \rightarrow \qquad \Pi_{int}(\boldsymbol{u},p,J) = \int_V \psi(\overline{\boldsymbol{F}}) \ dV + \int_V p (J-\overline{J}) \ dV
+        \Pi_{int} &= \int_V \psi(\boldsymbol{F}) \ dV \qquad \rightarrow
+        \qquad \Pi_{int}(\boldsymbol{u},p,J) = \int_V \psi(\overline{\boldsymbol{F}})
+        \ dV + \int_V p (J-\overline{J}) \ dV
 
-        \overline{\boldsymbol{F}} &= \left(\frac{\overline{J}}{J}\right)^{1/3} \boldsymbol{F}
+        \overline{\boldsymbol{F}} &=
+        \left(\frac{\overline{J}}{J}\right)^{1/3} \boldsymbol{F}
 
     The variations of the total potential energy w.r.t.
     :math:`(\boldsymbol{u},p,J)` lead to the following expressions. We denote
     first partial derivatives as :math:`\boldsymbol{f}_{(\bullet)}` and second
     partial derivatives as :math:`\boldsymbol{A}_{(\bullet,\bullet)}`.
 
     ..  math::
 
-        \delta_{\boldsymbol{u}} \Pi_{int} &= \int_V \boldsymbol{f}_{\boldsymbol{u}} : \delta \boldsymbol{F} \ dV = \int_V \left( \frac{\partial \psi}{\partial \overline{\boldsymbol{F}}} : \frac{\partial \overline{\boldsymbol{F}}}{\partial \boldsymbol{F}} + p J \boldsymbol{F}^{-T} \right) : \delta \boldsymbol{F} \ dV
-
-        \delta_{p} \Pi_{int} &= \int_V f_{p} \ \delta p \ dV = \int_V (J - \overline{J}) \ \delta p \ dV
-
-        \delta_{\overline{J}} \Pi_{int} &= \int_V f_{\overline{J}} \ \delta \overline{J} \ dV = \int_V \left( \frac{\partial \psi}{\partial \overline{\boldsymbol{F}}} : \frac{\partial \overline{\boldsymbol{F}}}{\partial \overline{J}} - p \right) : \delta \overline{J} \ dV
+        \delta_{\boldsymbol{u}} \Pi_{int} &= \int_V \boldsymbol{f}_{\boldsymbol{u}} :
+        \delta \boldsymbol{F} \ dV = \int_V \left( \frac{\partial \psi}
+        {\partial \overline{\boldsymbol{F}}} : \frac{\partial \overline{\boldsymbol{F}}}
+        {\partial \boldsymbol{F}} + p J \boldsymbol{F}^{-T} \right) :
+        \delta \boldsymbol{F} \ dV
+
+        \delta_{p} \Pi_{int} &= \int_V f_{p} \ \delta p \ dV =
+        \int_V (J - \overline{J}) \ \delta p \ dV
+
+        \delta_{\overline{J}} \Pi_{int} &= \int_V f_{\overline{J}} \ \delta \overline{J}
+        \ dV = \int_V \left( \frac{\partial \psi}{\partial \overline{\boldsymbol{F}}} :
+        \frac{\partial \overline{\boldsymbol{F}}}{\partial \overline{J}} - p \right) :
+        \delta \overline{J} \ dV
 
     The projection tensors from the variations lead the following results.
 
     ..  math::
 
-        \frac{\partial \overline{\boldsymbol{F}}}{\partial \boldsymbol{F}} &= \left(\frac{\overline{J}}{J}\right)^{1/3} \left( \boldsymbol{I} \overset{ik}{\odot} \boldsymbol{I} - \frac{1}{3} \boldsymbol{F} \otimes \boldsymbol{F}^{-T} \right)
+        \frac{\partial \overline{\boldsymbol{F}}}{\partial \boldsymbol{F}} &=
+        \left(\frac{\overline{J}}{J}\right)^{1/3} \left( \boldsymbol{I}
+        \overset{ik}{\odot} \boldsymbol{I} - \frac{1}{3} \boldsymbol{F} \otimes
+        \boldsymbol{F}^{-T} \right)
 
-        \frac{\partial \overline{\boldsymbol{F}}}{\partial \overline{J}} &= \frac{1}{3 \overline{J}} \overline{\boldsymbol{F}}
+        \frac{\partial \overline{\boldsymbol{F}}}{\partial \overline{J}} &=
+        \frac{1}{3 \overline{J}} \overline{\boldsymbol{F}}
 
     The double-dot products from the variations are now evaluated.
 
     ..  math::
 
-        \overline{\boldsymbol{P}} &= \frac{\partial \psi}{\partial \overline{\boldsymbol{F}}} = \overline{\overline{\boldsymbol{P}}} - \frac{1}{3} \left(  \overline{\overline{\boldsymbol{P}}} : \boldsymbol{F} \right) \boldsymbol{F}^{-T} \qquad \text{with} \qquad \overline{\overline{\boldsymbol{P}}} = \left(\frac{\overline{J}}{J}\right)^{1/3} \frac{\partial \psi}{\partial \overline{\boldsymbol{F}}}
-
-        \frac{\partial \psi}{\partial \overline{\boldsymbol{F}}} : \frac{1}{3 \overline{J}} \overline{\boldsymbol{F}} &= \frac{1}{3 \overline{J}} \overline{\overline{\boldsymbol{P}}} : \boldsymbol{F}
+        \overline{\boldsymbol{P}} &= \frac{\partial \psi}{\partial
+        \overline{\boldsymbol{F}}} = \overline{\overline{\boldsymbol{P}}} - \frac{1}{3}
+        \left(  \overline{\overline{\boldsymbol{P}}} : \boldsymbol{F} \right)
+        \boldsymbol{F}^{-T} \qquad \text{with} \qquad
+        \overline{\overline{\boldsymbol{P}}} = \left(\frac{\overline{J}}{J}\right)^{1/3}
+        \frac{\partial \psi}{\partial \overline{\boldsymbol{F}}}
+
+        \frac{\partial \psi}{\partial \overline{\boldsymbol{F}}} :
+        \frac{1}{3 \overline{J}} \overline{\boldsymbol{F}} &= \frac{1}{3 \overline{J}}
+        \overline{\overline{\boldsymbol{P}}} : \boldsymbol{F}
 
     We now have three formulas; one for the first Piola Kirchhoff stress and
     two additional control equations.
 
     ..  math::
 
-        \boldsymbol{f}_{\boldsymbol{u}} (= \boldsymbol{P}) &= \overline{\overline{\boldsymbol{P}}} - \frac{1}{3} \left(  \overline{\overline{\boldsymbol{P}}} : \boldsymbol{F} \right) \boldsymbol{F}^{-T}
+        \boldsymbol{f}_{\boldsymbol{u}} (= \boldsymbol{P}) &=
+        \overline{\overline{\boldsymbol{P}}} - \frac{1}{3} \left(
+        \overline{\overline{\boldsymbol{P}}} : \boldsymbol{F} \right)
+        \boldsymbol{F}^{-T}
 
         f_p &= J - \overline{J}
 
-        f_{\overline{J}} &=  \frac{1}{3 \overline{J}} \left( \overline{\overline{\boldsymbol{P}}} : \boldsymbol{F} \right) - p
+        f_{\overline{J}} &=  \frac{1}{3 \overline{J}} \left(
+        \overline{\overline{\boldsymbol{P}}} : \boldsymbol{F} \right) - p
 
     A linearization of the above formulas gives six equations (only results are
     given here).
 
     ..  math::
 
-        \mathbb{A}_{\boldsymbol{u},\boldsymbol{u}} &=  \overline{\overline{\mathbb{A}}} + \frac{1}{9} \left(  \boldsymbol{F} : \overline{\overline{\mathbb{A}}} : \boldsymbol{F} \right) \boldsymbol{F}^{-T} \otimes \boldsymbol{F}^{-T} - \frac{1}{3} \left( \boldsymbol{F}^{-T} \otimes \left( \overline{\overline{\boldsymbol{P}}} + \boldsymbol{F} : \overline{\overline{\mathbb{A}}} \right) + \left( \overline{\overline{\boldsymbol{P}}} + \overline{\overline{\mathbb{A}}} : \boldsymbol{F} \right) \otimes \boldsymbol{F}^{-T} \right)
-
-        &+\left( p J + \frac{1}{9} \overline{\overline{\boldsymbol{P}}} : \boldsymbol{F} \right) \boldsymbol{F}^{-T} \otimes \boldsymbol{F}^{-T} - \left( p J - \frac{1}{3} \overline{\overline{\boldsymbol{P}}} : \boldsymbol{F} \right) \boldsymbol{F}^{-T} \overset{il}{\odot} \boldsymbol{F}^{-T}
+        \mathbb{A}_{\boldsymbol{u},\boldsymbol{u}} &=  \overline{\overline{\mathbb{A}}}
+        + \frac{1}{9} \left(  \boldsymbol{F} : \overline{\overline{\mathbb{A}}} :
+        \boldsymbol{F} \right) \boldsymbol{F}^{-T} \otimes \boldsymbol{F}^{-T} -
+        \frac{1}{3} \left( \boldsymbol{F}^{-T} \otimes \left(
+        \overline{\overline{\boldsymbol{P}}} + \boldsymbol{F} :
+        \overline{\overline{\mathbb{A}}} \right) + \left(
+        \overline{\overline{\boldsymbol{P}}} + \overline{\overline{\mathbb{A}}} :
+        \boldsymbol{F} \right) \otimes \boldsymbol{F}^{-T} \right)
+
+        &+\left( p J + \frac{1}{9} \overline{\overline{\boldsymbol{P}}} : \boldsymbol{F}
+        \right) \boldsymbol{F}^{-T} \otimes \boldsymbol{F}^{-T} - \left( p J -
+        \frac{1}{3} \overline{\overline{\boldsymbol{P}}} : \boldsymbol{F} \right)
+        \boldsymbol{F}^{-T} \overset{il}{\odot} \boldsymbol{F}^{-T}
 
         A_{p,p} &= 0
 
-        A_{\overline{J},\overline{J}} &= \frac{1}{9 \overline{J}^2} \left( \boldsymbol{F} : \overline{\overline{\mathbb{A}}} : \boldsymbol{F} \right) - 2 \left( \overline{\overline{\boldsymbol{P}}} : \boldsymbol{F} \right)
-
-        \boldsymbol{A}_{\boldsymbol{u},p} &= \boldsymbol{A}_{p, \boldsymbol{u}} = J \boldsymbol{F}^{-T}
-
-        \boldsymbol{A}_{\boldsymbol{u},\overline{J}} &= \boldsymbol{A}_{\overline{J}, \boldsymbol{u}} = \frac{1}{3 \overline{J}} \left( \boldsymbol{P}' + \boldsymbol{F} : \overline{\overline{\mathbb{A}}} - \frac{1}{3} \left( \boldsymbol{F} : \overline{\overline{\mathbb{A}}} : \boldsymbol{F} \right) \boldsymbol{F}^{-T} \right)
+        A_{\overline{J},\overline{J}} &= \frac{1}{9 \overline{J}^2} \left(
+        \boldsymbol{F} : \overline{\overline{\mathbb{A}}} : \boldsymbol{F} \right) -
+        2 \left( \overline{\overline{\boldsymbol{P}}} : \boldsymbol{F} \right)
+
+        \boldsymbol{A}_{\boldsymbol{u},p} &= \boldsymbol{A}_{p, \boldsymbol{u}} =
+        J \boldsymbol{F}^{-T}
+
+        \boldsymbol{A}_{\boldsymbol{u},\overline{J}} &= \boldsymbol{A}_{\overline{J},
+        \boldsymbol{u}} = \frac{1}{3 \overline{J}} \left( \boldsymbol{P}' +
+        \boldsymbol{F} : \overline{\overline{\mathbb{A}}} - \frac{1}{3} \left(
+        \boldsymbol{F} : \overline{\overline{\mathbb{A}}} : \boldsymbol{F} \right)
+        \boldsymbol{F}^{-T} \right)
 
         A_{p,\overline{J}} &= A_{\overline{J}, p} = -1
 
 
     with
 
     ..  math::
 
-        \overline{\overline{\mathbb{A}}} = \left(\frac{\overline{J}}{J}\right)^{1/3} \frac{\partial^2 \psi}{\partial \overline{\boldsymbol{F}} \partial \overline{\boldsymbol{F}}} \left(\frac{\overline{J}}{J}\right)^{1/3}
+        \overline{\overline{\mathbb{A}}} = \left(\frac{\overline{J}}{J}\right)^{1/3}
+        \frac{\partial^2 \psi}{\partial \overline{\boldsymbol{F}} \partial
+        \overline{\boldsymbol{F}}} \left(\frac{\overline{J}}{J}\right)^{1/3}
 
     as well as
 
     ..  math::
 
         \boldsymbol{P}' = \boldsymbol{P} - p J \boldsymbol{F}^{-T}
 
@@ -264,15 +300,15 @@
         [F, p, J], statevars = x[:3], x[-1]
 
         self.detF = det(F)
         self.iFT = transpose(inv(F))
         self.Fb = (J / self.detF) ** (1 / 3) * F
         self.Pb, statevars_new = self.fun_P([self.Fb, statevars])
         self.Pbb = (J / self.detF) ** (1 / 3) * self.Pb
-        self.PbbF = ddot(self.Pbb, F, parallel=self.parallel)
+        self.PbbF = ddot(self.Pbb, F, mode=(2, 2), parallel=self.parallel)
 
         return [
             self._gradient_u(F, p, J),
             self._gradient_p(F, p, J),
             self._gradient_J(F, p, J),
             statevars_new,
         ]
@@ -322,18 +358,18 @@
         self.eye = identity(F)
         self.P4 = cdya_ik(self.eye, self.eye, parallel=self.parallel) - 1 / 3 * dya(
             F, self.iFT, parallel=self.parallel
         )
         self.A4b = self.fun_A([self.Fb, statevars])[0]
         self.A4bb = (J / self.detF) ** (2 / 3) * self.A4b
 
-        self.PbbF = ddot(self.Pbb, F, parallel=self.parallel)
-        self.FA4bb = ddot(F, self.A4bb, parallel=self.parallel)
-        self.A4bbF = ddot(self.A4bb, F, parallel=self.parallel)
-        self.FA4bbF = ddot(F, self.A4bbF, parallel=self.parallel)
+        self.PbbF = ddot(self.Pbb, F, mode=(2, 2), parallel=self.parallel)
+        self.FA4bb = ddot(F, self.A4bb, mode=(2, 4), parallel=self.parallel)
+        self.A4bbF = ddot(self.A4bb, F, mode=(4, 2), parallel=self.parallel)
+        self.FA4bbF = ddot(F, self.A4bbF, mode=(2, 2), parallel=self.parallel)
 
         return [
             self._hessian_uu(F, p, J),
             self._hessian_up(F, p, J),
             self._hessian_uJ(F, p, J),
             self._hessian_pp(F, p, J),
             self._hessian_pJ(F, p, J),
```

### Comparing `felupe-7.1.0/src/felupe/constitution/_models_hyperelasticity.py` & `felupe-7.2.0/src/felupe/constitution/_models_hyperelasticity.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 
 from ..math import (
     cdya_ik,
     cdya_il,
@@ -54,15 +45,16 @@
     energy function is defined on the determinant of the deformation
     gradient.
 
     .. math::
 
         \psi &= \hat{\psi}(\hat{\boldsymbol{C}}) + U(J)
 
-        \hat\psi(\hat{\boldsymbol{C}}) &= \frac{\mu}{2} (\text{tr}(\hat{\boldsymbol{C}}) - 3)
+        \hat\psi(\hat{\boldsymbol{C}}) &= \frac{\mu}{2}
+        (\text{tr}(\hat{\boldsymbol{C}}) - 3)
 
     with
 
     .. math::
 
        J &= \text{det}(\boldsymbol{F})
 
@@ -81,72 +73,95 @@
     of the strain energy density function. The hessian of the strain
     energy density function enables the corresponding elasticity tensor.
 
     .. math::
 
        \boldsymbol{P} &= \frac{\partial \psi}{\partial \boldsymbol{F}}
 
-       \mathbb{A} &= \frac{\partial^2 \psi}{\partial \boldsymbol{F}\ \partial \boldsymbol{F}}
+       \mathbb{A} &= \frac{\partial^2 \psi}{\partial \boldsymbol{F}\ \partial
+       \boldsymbol{F}}
 
     A chain rule application leads to the following expression for the stress tensor.
-    It is formulated as a sum of the **physical**-deviatoric (not the mathematical deviator!) and the physical-hydrostatic stress tensors.
+    It is formulated as a sum of the **physical**-deviatoric (not the mathematical
+    deviator!) and the physical-hydrostatic stress tensors.
 
     .. math::
 
        \boldsymbol{P} &= \boldsymbol{P}' + \boldsymbol{P}_U
 
-       \boldsymbol{P}' &= \frac{\partial \hat{\psi}}{\partial \hat{\boldsymbol{F}}} : \frac{\partial \hat{\boldsymbol{F}}}{\partial \boldsymbol{F}} = \bar{\boldsymbol{P}} - \frac{1}{3} (\bar{\boldsymbol{P}} : \boldsymbol{F}) \boldsymbol{F}^{-T}
+       \boldsymbol{P}' &= \frac{\partial \hat{\psi}}{\partial \hat{\boldsymbol{F}}} :
+       \frac{\partial \hat{\boldsymbol{F}}}{\partial \boldsymbol{F}} =
+       \bar{\boldsymbol{P}} - \frac{1}{3} (\bar{\boldsymbol{P}} : \boldsymbol{F})
+       \boldsymbol{F}^{-T}
 
-       \boldsymbol{P}_U &= \frac{\partial U(J)}{\partial J} \frac{\partial J}{\partial \boldsymbol{F}} = U'(J) J \boldsymbol{F}^{-T}
+       \boldsymbol{P}_U &= \frac{\partial U(J)}{\partial J} \frac{\partial J}{\partial
+       \boldsymbol{F}} = U'(J) J \boldsymbol{F}^{-T}
 
     with
 
     .. math::
 
-       \frac{\partial \hat{\boldsymbol{F}}}{\partial \boldsymbol{F}} &= J^{-1/3} \left( \boldsymbol{I} \overset{ik}{\otimes} \boldsymbol{I} - \frac{1}{3} \boldsymbol{F} \otimes \boldsymbol{F}^{-T} \right)
+       \frac{\partial \hat{\boldsymbol{F}}}{\partial \boldsymbol{F}} &= J^{-1/3} \left(
+       \boldsymbol{I} \overset{ik}{\otimes} \boldsymbol{I} - \frac{1}{3} \boldsymbol{F}
+       \otimes \boldsymbol{F}^{-T} \right)
 
        \frac{\partial J}{\partial \boldsymbol{F}} &= J \boldsymbol{F}^{-T}
 
-       \bar{\boldsymbol{P}} &= J^{-1/3} \frac{\partial \hat{\psi}}{\partial \hat{\boldsymbol{F}}}
+       \bar{\boldsymbol{P}} &= J^{-1/3} \frac{\partial \hat{\psi}}{\partial
+       \hat{\boldsymbol{F}}}
 
     With the above partial derivatives the first Piola-Kirchhoff stress
     tensor of the Neo-Hookean material model takes the following form.
 
     .. math::
 
-       \boldsymbol{P} = \mu J^{-2/3} \left( \boldsymbol{F} - \frac{1}{3} (\boldsymbol{F} : \boldsymbol{F}) \boldsymbol{F}^{-T} \right) + K (J - 1) J \boldsymbol{F}^{-T}
+       \boldsymbol{P} = \mu J^{-2/3} \left( \boldsymbol{F} - \frac{1}{3} (
+       \boldsymbol{F} : \boldsymbol{F}) \boldsymbol{F}^{-T} \right) + K (J - 1) J
+       \boldsymbol{F}^{-T}
 
     Again, a chain rule application leads to an expression for the elasticity tensor.
 
     .. math::
 
        \mathbb{A} &= \mathbb{A}' + \mathbb{A}_{U}
 
-       \mathbb{A}' &= \bar{\mathbb{A}} - \frac{1}{3} \left( (\bar{\mathbb{A}} : \boldsymbol{F}) \otimes \boldsymbol{F}^{-T} + \boldsymbol{F}^{-T} \otimes (\boldsymbol{F} : \bar{\mathbb{A}}) \right ) + \frac{1}{9} (\boldsymbol{F} : \bar{\mathbb{A}} : \boldsymbol{F}) \boldsymbol{F}^{-T} \otimes \boldsymbol{F}^{-T}
-
-       \mathbb{A}_{U} &= (U''(J) J + U'(J)) J \boldsymbol{F}^{-T} \otimes \boldsymbol{F}^{-T} - U'(J) J \boldsymbol{F}^{-T} \overset{il}{\otimes} \boldsymbol{F}^{-T}
+       \mathbb{A}' &= \bar{\mathbb{A}} - \frac{1}{3} \left( (\bar{\mathbb{A}} :
+       \boldsymbol{F}) \otimes \boldsymbol{F}^{-T} + \boldsymbol{F}^{-T} \otimes
+       (\boldsymbol{F} : \bar{\mathbb{A}}) \right ) + \frac{1}{9} (\boldsymbol{F} :
+       \bar{\mathbb{A}} : \boldsymbol{F}) \boldsymbol{F}^{-T} \otimes
+       \boldsymbol{F}^{-T}
+
+       \mathbb{A}_{U} &= (U''(J) J + U'(J)) J \boldsymbol{F}^{-T} \otimes
+       \boldsymbol{F}^{-T} - U'(J) J \boldsymbol{F}^{-T} \overset{il}{\otimes}
+       \boldsymbol{F}^{-T}
 
     with
 
     .. math::
 
-       \bar{\mathbb{A}} = J^{-1/3} \frac{\partial^2 \hat\psi}{\partial \hat{\boldsymbol{F}}\ \partial \hat{\boldsymbol{F}}} J^{-1/3}
+       \bar{\mathbb{A}} = J^{-1/3} \frac{\partial^2 \hat\psi}{\partial
+       \hat{\boldsymbol{F}}\ \partial \hat{\boldsymbol{F}}} J^{-1/3}
 
     With the above partial derivatives the (physical-deviatoric and
     -hydrostatic) parts of the elasticity tensor associated
     to the first Piola-Kirchhoff stress tensor of the Neo-Hookean
     material model takes the following form.
 
     .. math::
 
        \mathbb{A} &= \mathbb{A}' + \mathbb{A}_{U}
 
-       \mathbb{A}' &= J^{-2/3} \left(\boldsymbol{I} \overset{ik}{\otimes} \boldsymbol{I} - \frac{1}{3} \left( \boldsymbol{F} \otimes \boldsymbol{F}^{-T} + \boldsymbol{F}^{-T} \otimes \boldsymbol{F} \right ) + \frac{1}{9} (\boldsymbol{F} : \boldsymbol{F}) \boldsymbol{F}^{-T} \otimes \boldsymbol{F}^{-T} \right)
-
-       \mathbb{A}_{U} &= K J \left( (2J - 1) \boldsymbol{F}^{-T} \otimes \boldsymbol{F}^{-T} - (J - 1) \boldsymbol{F}^{-T} \overset{il}{\otimes} \boldsymbol{F}^{-T} \right)
+       \mathbb{A}' &= J^{-2/3} \left(\boldsymbol{I} \overset{ik}{\otimes} \boldsymbol{I}
+       - \frac{1}{3} \left( \boldsymbol{F} \otimes \boldsymbol{F}^{-T} +
+       \boldsymbol{F}^{-T} \otimes \boldsymbol{F} \right ) + \frac{1}{9} (\boldsymbol{F}
+       : \boldsymbol{F}) \boldsymbol{F}^{-T} \otimes \boldsymbol{F}^{-T} \right)
+
+       \mathbb{A}_{U} &= K J \left( (2J - 1) \boldsymbol{F}^{-T} \otimes
+       \boldsymbol{F}^{-T} - (J - 1) \boldsymbol{F}^{-T} \overset{il}{\otimes}
+       \boldsymbol{F}^{-T} \right)
 
 
     Arguments
     ---------
     mu : float
         Shear modulus
     bulk : float
```

### Comparing `felupe-7.1.0/src/felupe/constitution/_models_hyperelasticity_ad.py` & `felupe-7.2.0/src/felupe/constitution/_models_hyperelasticity_ad.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,28 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 from functools import wraps
 
 import numpy as np
-import tensortrax as tr
 from tensortrax.math import log, sqrt
 from tensortrax.math import sum as sum1
 from tensortrax.math import trace
 from tensortrax.math._linalg import det, eigvalsh, inv
 from tensortrax.math._special import from_triu_1d, triu_1d
 
 
@@ -45,15 +35,16 @@
         return fun(det(C) ** (-1 / 3) * C, *args, **kwargs)
 
     return apply_iso
 
 
 def saint_venant_kirchhoff(C, mu, lmbda):
     """Strain energy function of the Saint Venant-Kirchhoff material formulation.
-    Here, ``I1`` and ``I2`` are strain invariants of the Green-Lagrange strain tensor."""
+    Here, ``I1`` and ``I2`` are strain invariants of the Green-Lagrange strain tensor.
+    """
     I1 = trace(C) / 2 - 3 / 2
     I2 = trace(C @ C) / 4 - trace(C) / 2 + 3 / 4
     return mu * I2 + lmbda * I1**2 / 2
 
 
 def neo_hooke(C, mu):
     "Strain energy function of the Neo-Hookean material formulation."
@@ -120,19 +111,19 @@
 
 
 def van_der_waals(C, mu, limit, a, beta):
     "Strain energy function of the Van der Waals material formulation."
     J3 = det(C) ** (-1 / 3)
     I1 = J3 * trace(C)
     I2 = J3 * (trace(C) ** 2 - trace(C @ C)) / 2
-    I = (1 - beta) * I1 + beta * I2
-    I.x[np.isclose(I.x, 3)] += 1e-8
-    eta = sqrt((I - 3) / (limit**2 - 3))
+    Im = (1 - beta) * I1 + beta * I2
+    Im.x[np.isclose(Im.x, 3)] += 1e-8
+    eta = sqrt((Im - 3) / (limit**2 - 3))
     return mu * (
-        -(limit**2 - 3) * (log(1 - eta) + eta) - 2 / 3 * a * ((I - 3) / 2) ** (3 / 2)
+        -(limit**2 - 3) * (log(1 - eta) + eta) - 2 / 3 * a * ((Im - 3) / 2) ** (3 / 2)
     )
 
 
 @isochoric_volumetric_split
 def finite_strain_viscoelastic(C, Cin, mu, eta, dtime):
     "Finite strain viscoelastic material formulation."
```

### Comparing `felupe-7.1.0/src/felupe/constitution/_models_linear_elasticity.py` & `felupe-7.2.0/src/felupe/constitution/_models_linear_elasticity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,28 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 
-from ..math import (
-    cdya,
-    cdya_ik,
-    cdya_il,
-    ddot,
-    det,
-    dot,
-    dya,
-    identity,
-    inv,
-    trace,
-    transpose,
-)
+from ..math import cdya, dya, identity, trace, transpose
 
 
 def lame_converter(E, nu):
     """Convert material parameters to first and second Lamé - constants.
 
     Arguments
     ---------
@@ -94,15 +73,17 @@
             2 \varepsilon_{31}
         \end{bmatrix}
 
     with the strain tensor
 
     ..  math::
 
-        \boldsymbol{\varepsilon} = \frac{1}{2} \left( \frac{\partial \boldsymbol{u}}{\partial \boldsymbol{X}} + \left( \frac{\partial \boldsymbol{u}}{\partial \boldsymbol{X}} \right)^T \right)
+        \boldsymbol{\varepsilon} = \frac{1}{2} \left( \frac{\partial \boldsymbol{u}}
+        {\partial \boldsymbol{X}} + \left( \frac{\partial \boldsymbol{u}}
+        {\partial \boldsymbol{X}} \right)^T \right)
 
 
     Arguments
     ---------
     E : float
         Young's modulus.
     nu : float
@@ -220,23 +201,28 @@
 
 
 class LinearElasticTensorNotation:
     r"""Isotropic linear-elastic material formulation.
 
     ..  math::
 
-        \boldsymbol{\sigma} &= 2 \mu \ \boldsymbol{\varepsilon} + \gamma \ \text{tr}(\boldsymbol{\varepsilon}) \ \boldsymbol{I}
+        \boldsymbol{\sigma} &= 2 \mu \ \boldsymbol{\varepsilon} + \gamma \
+        \text{tr}(\boldsymbol{\varepsilon}) \ \boldsymbol{I}
 
-        \frac{\boldsymbol{\partial \sigma}}{\partial \boldsymbol{\varepsilon}} &= 2 \mu \ \boldsymbol{I} \odot \boldsymbol{I} + \gamma \ \boldsymbol{I} \otimes \boldsymbol{I}
+        \frac{\boldsymbol{\partial \sigma}}{\partial \boldsymbol{\varepsilon}} &=
+        2 \mu \ \boldsymbol{I} \odot \boldsymbol{I} + \gamma \ \boldsymbol{I} \otimes
+        \boldsymbol{I}
 
     with the strain tensor
 
     ..  math::
 
-        \boldsymbol{\varepsilon} = \frac{1}{2} \left( \frac{\partial \boldsymbol{u}}{\partial \boldsymbol{X}} + \left( \frac{\partial \boldsymbol{u}}{\partial \boldsymbol{X}} \right)^T \right)
+        \boldsymbol{\varepsilon} = \frac{1}{2} \left( \frac{\partial \boldsymbol{u}}
+        {\partial \boldsymbol{X}} + \left( \frac{\partial \boldsymbol{u}}
+        {\partial \boldsymbol{X}} \right)^T \right)
 
 
     Arguments
     ---------
     E : float
         Young's modulus.
     nu : float
@@ -321,21 +307,21 @@
 
         if E is None:
             E = self.E
 
         if nu is None:
             nu = self.nu
 
-        I = identity(dim=3, shape=shape)
+        eye = identity(dim=3, shape=shape)
 
         # convert to lame constants
         gamma, mu = lame_converter(E, nu)
 
-        elast = 2 * mu * cdya(I, I, parallel=self.parallel) + gamma * dya(
-            I, I, parallel=self.parallel
+        elast = 2 * mu * cdya(eye, eye, parallel=self.parallel) + gamma * dya(
+            eye, eye, parallel=self.parallel
         )
 
         return [elast]
 
 
 class LinearElasticPlaneStrain:
     """Plane-strain isotropic linear-elastic material formulation.
```

### Comparing `felupe-7.1.0/src/felupe/constitution/_models_pseudo_elasticity.py` & `felupe-7.2.0/src/felupe/constitution/_models_pseudo_elasticity.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,50 +1,44 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 
 from ..math import dya
 
 
 class OgdenRoxburgh:
     r"""A Pseudo-Elastic material formulation for an isotropic treatment of the
     load-history dependent Mullins-softening of rubber-like materials.
 
     ..  math::
 
-        \eta(W, W_{max}) &= 1 - \frac{1}{r} erf\left( \frac{W_{max} - W}{m + \beta~W_{max}} \right)
+        \eta(W, W_{max}) &= 1 - \frac{1}{r} erf\left( \frac{W_{max} - W}
+        {m + \beta~W_{max}} \right)
 
         \boldsymbol{P} &= \eta \frac{\partial \psi}{\partial \boldsymbol{F}}
 
-        \mathbb{A} &= \frac{\partial^2 \psi}{\partial \boldsymbol{F} \partial \boldsymbol{F}} + \frac{\partial \eta}{\partial \psi} \frac{\partial \psi}{\partial \boldsymbol{F}} \otimes \frac{\partial \psi}{\partial \boldsymbol{F}}
+        \mathbb{A} &= \frac{\partial^2 \psi}{\partial \boldsymbol{F} \partial
+        \boldsymbol{F}} + \frac{\partial \eta}{\partial \psi} \frac{\partial \psi}
+        {\partial \boldsymbol{F}} \otimes \frac{\partial \psi}{\partial \boldsymbol{F}}
 
     """
 
     def __init__(self, material, r, m, beta):
 
         # isotropic hyperelastic material formulation
         self.material = material
```

### Comparing `felupe-7.1.0/src/felupe/constitution/_user_materials.py` & `felupe-7.2.0/src/felupe/constitution/_user_materials.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 
 from ..math import identity, ravel, reshape, sym
 from ._models_linear_elasticity import lame_converter
 from ._user_materials_models import linear_elastic_plastic_isotropic_hardening
```

### Comparing `felupe-7.1.0/src/felupe/constitution/_user_materials_hyperelastic.py` & `felupe-7.2.0/src/felupe/constitution/_user_materials_hyperelastic.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 import tensortrax as tr
 
 from ..math import cdya_ik, dot, transpose
 from ._user_materials import UserMaterial
```

### Comparing `felupe-7.1.0/src/felupe/constitution/_user_materials_models.py` & `felupe-7.2.0/src/felupe/constitution/_user_materials_models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 
 from ..math import cdya_ik, ddot, dya, identity, sqrt, trace
 
 
@@ -56,23 +47,23 @@
     λ : float
         First Lamé-constant.
     μ : float
         Second Lamé-constant (shear modulus).
     """
 
     # change of stress due to change of strain
-    I = identity(dim=3, shape=(1, 1))
-    dσ = 2 * μ * dε + λ * trace(dε) * I
+    eye = identity(dim=3, shape=(1, 1))
+    dσ = 2 * μ * dε + λ * trace(dε) * eye
 
     # update stress
     σ = σn + dσ
 
     # evaluate elasticity tensor
     if kwargs["tangent"]:
-        dσdε = 2 * μ * cdya_ik(I, I) + λ * dya(I, I)
+        dσdε = 2 * μ * cdya_ik(eye, eye) + λ * dya(eye, eye)
     else:
         dσdε = None
 
     # update state variables (not used here)
     ζ = ζn
 
     return dσdε, σ, ζ
@@ -116,15 +107,16 @@
 
             εp = εpn + dγ n
 
             α = αn + sqrt(2 / 3) dγ
 
             Algorithmic consistent tangent modulus:
 
-            dσdε = dσdε - 2μ / (1 + K / 3μ) n ⊗ n - 2μ dγ / ||s|| ((2μ 1 ⊙ 1 - 1/3 1 ⊗ 1) - 2μ n ⊗ n)
+            dσdε = dσdε - 2μ / (1 + K / 3μ) n ⊗ n
+                 - 2μ dγ / ||s|| ((2μ 1 ⊙ 1 - 1/3 1 ⊗ 1) - 2μ n ⊗ n)
 
     Arguments
     ---------
     dε : ndarray
         Strain increment.
     εn : ndarray
         Old strain tensor.
@@ -138,26 +130,26 @@
         Second Lamé-constant (shear modulus).
     σy : float
         Initial yield stress.
     K : float
         Isotropic hardening modulus.
     """
 
-    I = identity(dε)
+    eye = identity(dε)
 
     # elasticity tensor
     if kwargs["tangent"]:
-        dσdε = λ * dya(I, I) + 2 * μ * cdya_ik(I, I)
+        dσdε = λ * dya(eye, eye) + 2 * μ * cdya_ik(eye, eye)
     else:
         dσdε = None
 
     # elastic hypothetic (trial) stress and deviatoric stress
-    dσ = 2 * μ * dε + λ * trace(dε) * I
+    dσ = 2 * μ * dε + λ * trace(dε) * eye
     σ = σn + dσ
-    s = σ - 1 / 3 * trace(σ) * I
+    s = σ - 1 / 3 * trace(σ) * eye
 
     # unpack old state variables
     α, εp = ζn
 
     # hypothetic (trial) yield function
     norm_s = sqrt(ddot(s, s))
     f = norm_s - sqrt(2 / 3) * (σy + K * α)
@@ -183,15 +175,18 @@
             dσdε[..., mask] = (
                 dσdε
                 - 2 * μ / (1 + K / (3 * μ)) * dya(n, n)
                 - 2
                 * μ
                 * dγ
                 / norm_s
-                * (2 * μ * (cdya_ik(I, I) - 1 / 3 * dya(I, I)) - 2 * μ * dya(n, n))
+                * (
+                    2 * μ * (cdya_ik(eye, eye) - 1 / 3 * dya(eye, eye))
+                    - 2 * μ * dya(n, n)
+                )
             )[..., mask]
 
         # update list of state variables
         ζ[0][..., mask] = α[..., mask]
         ζ[1][..., mask] = εp[..., mask]
 
     return dσdε, σ, ζ
```

### Comparing `felupe-7.1.0/src/felupe/dof/_boundary.py` & `felupe-7.2.0/src/felupe/dof/_boundary.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 
 
 class Boundary:
     "A Boundary as a collection of prescribed degrees of freedom."
```

### Comparing `felupe-7.1.0/src/felupe/dof/_loadcase.py` & `felupe-7.2.0/src/felupe/dof/_loadcase.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 
 from ._boundary import Boundary
 from ._tools import apply, partition
```

### Comparing `felupe-7.1.0/src/felupe/element/_hexahedron.py` & `felupe-7.2.0/src/felupe/element/_hexahedron.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 
 from ._base import Element
 from ._lagrange import ArbitraryOrderLagrange
```

### Comparing `felupe-7.1.0/src/felupe/element/_lagrange.py` & `felupe-7.2.0/src/felupe/element/_lagrange.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 from copy import deepcopy as copy
 from string import ascii_lowercase as alphabet
 
 import numpy as np
 from scipy.special import factorial
```

### Comparing `felupe-7.1.0/src/felupe/element/_quad.py` & `felupe-7.2.0/src/felupe/element/_quad.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 
 from ._base import Element
 from ._lagrange import ArbitraryOrderLagrange
```

### Comparing `felupe-7.1.0/src/felupe/element/_tetra.py` & `felupe-7.2.0/src/felupe/element/_tetra.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 
 from ._base import Element
```

### Comparing `felupe-7.1.0/src/felupe/element/_triangle.py` & `felupe-7.2.0/src/felupe/element/_triangle.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 
 from ._base import Element
```

### Comparing `felupe-7.1.0/src/felupe/math/_math.py` & `felupe-7.2.0/tests/test_bilinearform.py`

 * *Files 27% similar despite different names*

```diff
@@ -21,36 +21,82 @@
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
 
 """
 
-import numpy as np
+import pytest
 
+import felupe as fe
+from felupe.math import ddot, dot, dya
 
-def linsteps(points, num=10, endpoint=True):
 
-    points = np.array(points).ravel()
-    start = points[:-1]
-    end = points[1:]
-    num = np.array([num]).ravel()
+def lform(v, w):
+    return dot(w, v)
 
-    if len(num) == 1:
-        num = np.tile(num, max(1, len(start)))
 
-    num = np.pad(num, (0, max(0, len(start) - len(num))), mode="edge")
+def lform_grad(v, F):
+    return ddot(F, v)
 
-    steplist = [
-        np.linspace(a, b, n, endpoint=False) for a, b, n in zip(start, end, num)
-    ]
-    if len(steplist) > 0:
-        steps = np.concatenate(
-            [np.linspace(a, b, n, endpoint=False) for a, b, n in zip(start, end, num)]
-        )
-    else:
-        steps = np.array([])
 
-    if endpoint:
-        steps = np.append(steps, points[-1])
+def lformu(v, F, p):
+    return ddot(F, v)
 
-    return steps
+
+def lformp(q, F, p):
+    return dot(p, q)
+
+
+def bform(v, u, w):
+    return dot(w, v) * dot(w, u)
+
+
+def bform_grad(v, u, F):
+    return ddot(F, v) * ddot(F, u)
+
+
+def a_uu(v, u, F, p):
+    return ddot(u, ddot(dya(F, F), v))
+
+
+def a_up(v, r, F, p):
+    return dot(p, r) * ddot(F, v)
+
+
+def a_pp(q, r, F, p):
+    return dot(p, q) * dot(r, p)
+
+
+def pre(dim):
+
+    mesh = fe.Cube(n=3)
+    region = fe.RegionHexahedron(mesh)
+    region0 = fe.RegionConstantHexahedron(mesh.dual(points_per_cell=1))
+    u = fe.Field(region, dim=3)
+    p = fe.Field(region0)
+    up = fe.FieldContainer([u, p])
+
+    return up
+
+
+def test_form_decorator():
+
+    field = pre(dim=3)
+    F, p = field.extract()
+    b = fe.Basis(field)
+
+    @fe.Form(v=field, u=field, grad_v=(True, False), grad_u=(True, False))
+    def a():
+        return (a_uu, a_up, a_pp)
+
+    M = a.assemble(field, field, args=(F, p))
+
+    @fe.Form(v=field, grad_v=(True, False))
+    def L():
+        return (lformu, lformp)
+
+    s = L.assemble(field, args=(F, p))
+
+
+if __name__ == "__main__":
+    test_form_decorator()
```

### Comparing `felupe-7.1.0/src/felupe/math/_spatial.py` & `felupe-7.2.0/src/felupe/math/_spatial.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 
 
 def rotation_matrix(alpha_deg, dim=3, axis=0):
     """Rotation matrix with given rotation axis and dimension (2d or 3d).
```

### Comparing `felupe-7.1.0/src/felupe/math/_tensor.py` & `felupe-7.2.0/src/felupe/math/_tensor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,47 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 
 try:
     from einsumt import einsumt
 except ModuleNotFoundError:
     from numpy import einsum as einsumt
 
 
 def identity(A=None, dim=None, shape=None):
     "Identity according to matrix A with optional specified dim."
     if A is not None:
-        dimA, g, e = A.shape[-3:]
+        dimA = A.shape[0]
+        shapeA = A.shape[2:]
         if dim is None:
             dim = dimA
-    else:
-        g, e = shape
-    return np.tile(np.eye(dim), (g, e, 1, 1)).transpose([2, 3, 0, 1])
+        if shape is None:
+            shape = shapeA
+
+    ones = (1,) * len(shape)
+    eye = np.eye(dim).reshape(dim, dim, *ones)
+
+    return np.ascontiguousarray(np.broadcast_to(eye, (dim, dim, *shape)))
 
 
 def sym(A):
     "Symmetric part of matrix A."
     return (A + transpose(A)) / 2
 
 
@@ -135,26 +131,26 @@
 def cof(A):
     "Cofactor matrix of A (as a wrapper for the inverse of A)."
     return transpose(inv(A, determinant=1.0))
 
 
 def eig(A, eig=np.linalg.eig):
     "Eigenvalues and -vectors of matrix A."
-    wA, vA = eig(A.transpose([2, 3, 0, 1]))
-    return wA.transpose([2, 0, 1]), vA.transpose([2, 3, 0, 1])
+    wA, vA = eig(A.T)
+    return wA.T, vA.T
 
 
 def eigh(A):
     "Eigenvalues and -vectors of a symmetric matrix A."
     return eig(A, eig=np.linalg.eigh)
 
 
 def eigvals(A, shear=False, eig=np.linalg.eig):
     "Eigenvalues (and optional principal shear values) of a matrix A."
-    wA = eig(A.transpose([2, 3, 0, 1]))[0].transpose([2, 0, 1])
+    wA = eig(A.T)[0].T
     if shear:
         dim = wA.shape[0]
         if dim == 3:
             ij = [(1, 0), (2, 0), (2, 1)]
         elif dim == 2:
             ij = [(1, 0)]
         dwA = np.array([wA[i] - wA[j] for i, j in ij])
@@ -167,15 +163,15 @@
     "Eigenvalues (and optional principal shear values) of a symmetric matrix A."
     return eigvals(A, shear=shear, eig=np.linalg.eigh)
 
 
 def transpose(A, mode=1):
     "Transpose (mode=1) or major-transpose (mode=2) of matrix A."
     if mode == 1:
-        return A.transpose([1, 0, 2, 3])
+        return np.einsum("ij...->ji...", A)
     elif mode == 2:
         return np.einsum("ijkl...->klij...", A)
     else:
         raise ValueError("Unknown value of mode.")
 
 
 def majortranspose(A):
@@ -213,68 +209,68 @@
 def cross(a, b):
     "Cross product of two vectors a and b."
     return np.einsum(
         "...i->i...", np.cross(np.einsum("i...->...i", a), np.einsum("i...->...i", b))
     )
 
 
-def dot(A, B, n=2, parallel=False):
+def dot(A, B, mode=(2, 2), parallel=False):
     "Dot-product of A and B with inputs of n trailing axes.."
 
     if parallel:
         einsum = einsumt
     else:
         einsum = np.einsum
 
-    if len(A.shape) == 2 + n and len(B.shape) == 2 + n:
+    if mode == (2, 2):
         return einsum("ik...,kj...->ij...", A, B)
 
-    elif len(A.shape) == 1 + n and len(B.shape) == 1 + n:
+    elif mode == (1, 1):
         return einsum("i...,i...->...", A, B)
 
-    elif len(A.shape) == 4 + n and len(B.shape) == 4 + n:
+    elif mode == (4, 4):
         return einsum("ijkp...,plmn...->ijklmn...", A, B)
 
-    elif len(A.shape) == 2 + n and len(B.shape) == 1 + n:
+    elif mode == (2, 1):
         return einsum("ij...,j...->i...", A, B)
 
-    elif len(A.shape) == 1 + n and len(B.shape) == 2 + n:
+    elif mode == (1, 2):
         return einsum("i...,ij...->j...", A, B)
 
-    elif len(A.shape) == 4 + n and len(B.shape) == 1 + n:
+    elif mode == (4, 1):
         return einsum("ijkl...,l...->ijk...", A, B)
 
-    elif len(A.shape) == 1 + n and len(B.shape) == 4 + n:
+    elif mode == (1, 4):
         return einsum("i...,ijkl...->jkl...", A, B)
 
-    elif len(A.shape) == 2 + n and len(B.shape) == 4 + n:
+    elif mode == (2, 4):
         return einsum("im...,mjkl...->ijkl...", A, B)
 
-    elif len(A.shape) == 4 + n and len(B.shape) == 2 + n:
+    elif mode == (4, 2):
         return einsum("ijkm...,ml...->ijkl...", A, B)
 
     else:
         raise TypeError("Unknown shape of A and B.")
 
 
-def ddot(A, B, n=2, parallel=False):
+def ddot(A, B, mode=(2, 2), parallel=False):
     "Double-Dot-product of A and B with inputs of `n` trailing axes."
 
     if parallel:
         einsum = einsumt
     else:
         einsum = np.einsum
 
-    if len(A.shape) == 2 + n and len(B.shape) == 2 + n:
+    if mode == (2, 2):
         return einsum("ij...,ij...->...", A, B)
-    elif len(A.shape) == 2 + n and len(B.shape) == 4 + n:
+    elif mode == (2, 4):
         return einsum("ij...,ijkl...->kl...", A, B)
-    elif len(A.shape) == 4 + n and len(B.shape) == 2 + n:
+    elif mode == (4, 2):
         return einsum("ijkl...,kl...->ij...", A, B)
-    elif len(A.shape) == 4 + n and len(B.shape) == 4 + n:
+    elif mode == (4, 4):
         return einsum("ijkl...,klmn...->ijmn...", A, B)
     else:
         raise TypeError("Unknown shape of A and B.")
 
 
 def tovoigt(A, strain=False):
     "Convert (3, 3) tensor to (6, ) voigt notation."
```

### Comparing `felupe-7.1.0/src/felupe/mechanics/_curve.py` & `felupe-7.2.0/src/felupe/mechanics/_curve.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,27 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 
-from ..dof import Boundary
 from ..tools import force
 from ._job import Job
 
 
 class CharacteristicCurve(Job):
     def __init__(
         self,
@@ -77,15 +67,15 @@
         fig=None,
         ax=None,
         items=None,
         **kwargs
     ):
         if self.res is None:
             raise ValueError(
-                "Job results are empty. Run `job.evaluate()` and call `job.plot()` again."
+                "Results are empty. Run `job.evaluate()` and call `job.plot()` again."
             )
 
         import matplotlib.pyplot as plt
 
         if x is None:
             x = self.x
         if y is None:
```

### Comparing `felupe-7.1.0/src/felupe/mechanics/_helpers.py` & `felupe-7.2.0/src/felupe/mechanics/_helpers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,24 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
-
 import numpy as np
 
 from .._assembly import IntegralFormMixed
 from .._field import FieldAxisymmetric
 from ..constitution import AreaChange
 from ..math import det
```

### Comparing `felupe-7.1.0/src/felupe/mechanics/_job.py` & `felupe-7.2.0/src/felupe/mechanics/_job.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,66 +1,57 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
-
-This file is part of felupe.
+This file is part of FElupe.
 
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 from platform import architecture, machine, platform
 
 import numpy as np
 
 from ..__about__ import __version__ as version
 from ..math import dot, eigh, eigvalsh, tovoigt, transpose
 
 
-def displacement(substep):
+def displacement(field, substep=None):
     "Displacement Vector"
-    u = substep.x[0].values
+    u = field[0].values
     return np.pad(u, ((0, 0), (0, 3 - u.shape[1])))
 
 
-def deformation_gradient(substep):
+def deformation_gradient(field, substep=None):
     "Deformation Gradient"
-    F = substep.x[0].extract()
+    F = field[0].extract()
     return [F.mean(-2).transpose([2, 0, 1])]
 
 
-def log_strain_principal(substep):
+def log_strain_principal(field, substep=None):
     "Principal Values of Logarithmic Strain"
-    u = substep.x[0]
+    u = field[0]
     F = u.extract()
     stretch = np.sqrt(eigvalsh(dot(transpose(F), F)))[::-1]
     strain = np.log(stretch).mean(-2)
     return [strain.T]
 
 
-def log_strain(substep):
+def log_strain(field, substep=None):
     "Lagrangian Logarithmic Strain Tensor"
-    u = substep.x[0]
+    u = field[0]
     F = u.extract()
     w, v = eigh(dot(transpose(F), F))
     stretch = np.sqrt(w)
     strain = np.einsum("a...,ia...,ja...->ij...", np.log(stretch), v, v)
     return [tovoigt(strain.mean(-2), True).T]
 
 
@@ -72,20 +63,23 @@
         steps,
         callback=lambda stepnumber, substepnumber, substep: None,
         filename=None,
     ):
         self.steps = steps
         self.nsteps = len(steps)
         self.callback = callback
+        self.timetrack = []
 
     def _write(self, writer, time, substep, point_data, cell_data):
+        field = substep.x
+        kwargs = dict(field=field, substep=substep)
         writer.write_data(
             time,
-            point_data={key: value(substep) for key, value in point_data.items()},
-            cell_data={key: value(substep) for key, value in cell_data.items()},
+            point_data={key: value(**kwargs) for key, value in point_data.items()},
+            cell_data={key: value(**kwargs) for key, value in cell_data.items()},
         )
 
     def evaluate(
         self,
         filename=None,
         mesh=None,
         point_data=None,
@@ -96,31 +90,31 @@
         parallel=False,
         **kwargs,
     ):
 
         if verbose:
             print(
                 f"""
- _______  _______  ___      __   __  _______  _______ 
+ _______  _______  ___      __   __  _______  _______
 |       ||       ||   |    |  | |  ||       ||       |
 |    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
+|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___
 |    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
+|   |    |   |___ |       ||       ||   |    |   |___
 |___|    |_______||_______||_______||___|    |_______|
 FElupe Version {version} ({platform(terse=True)} {machine()} {architecture()[0]})
 
 """
             )
 
             print("Run Job")
             print("=======\n")
 
         if parallel:
-            if not "kwargs" in kwargs.keys():
+            if "kwargs" not in kwargs.keys():
                 kwargs["kwargs"] = {}
             kwargs["kwargs"]["parallel"] = True
 
         if filename is not None:
             from meshio.xdmf import TimeSeriesWriter
 
             if mesh is None:
@@ -180,14 +174,15 @@
                     self.callback(j, i, substep)
 
                     # update x0 after each completed substep
                     if "x0" in kwargs.keys():
                         kwargs["x0"].link(substep.x)
 
                     if filename is not None:
+                        self.timetrack.append(increment)
                         self._write(
                             writer=writer,
                             time=increment,
                             substep=substep,
                             point_data={**pdata, **point_data},
                             cell_data={**cdata, **cell_data},
                         )
```

### Comparing `felupe-7.1.0/src/felupe/mechanics/_pointload.py` & `felupe-7.2.0/src/felupe/mechanics/_pointload.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 from scipy.sparse import csr_matrix
 
 from ._helpers import Assemble, Results
```

### Comparing `felupe-7.1.0/src/felupe/mechanics/_solidbody.py` & `felupe-7.2.0/src/felupe/mechanics/_solidbody.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 
 from .._assembly import IntegralFormMixed
 from ..constitution import AreaChange
 from ..math import det, dot, transpose
```

### Comparing `felupe-7.1.0/src/felupe/mechanics/_solidbody_gravity.py` & `felupe-7.2.0/src/felupe/mechanics/_solidbody_gravity.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,29 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 from scipy.sparse import csr_matrix
 
 from .._assembly import IntegralFormMixed
-from ..constitution import AreaChange
 from ._helpers import Assemble, Results
 
 
 class SolidBodyGravity:
     "A SolidBody with methods for the assembly of sparse vectors/matrices."
 
     def __init__(self, field, gravity, density):
```

### Comparing `felupe-7.1.0/src/felupe/mechanics/_solidbody_incompressible.py` & `felupe-7.2.0/src/felupe/mechanics/_solidbody_incompressible.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 
 from .._assembly import IntegralFormMixed
 from .._field import FieldAxisymmetric
 from ..constitution import AreaChange
@@ -165,15 +156,15 @@
         v = self.results.state.v()
         J = self.results.state.J
         p = self.results.state.p
 
         du = (u - u0)[field.region.mesh.cells].transpose([1, 2, 0])
 
         # change of state variables due to change of displacement field
-        dJ = ddot(h, du, n=1) / self.V + (v / self.V - J)
+        dJ = ddot(h, du, mode=(2, 2)) / self.V + (v / self.V - J)
         dp = self.bulk * (dJ + J - 1) - p
 
         self.field = field
         self.results.kinematics = self.results.state.F = self.field.extract()
 
         # update state variables
         self.results.state.p = p + dp
```

### Comparing `felupe-7.1.0/src/felupe/mechanics/_solidbody_pressure.py` & `felupe-7.2.0/src/felupe/mechanics/_solidbody_pressure.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 from .._assembly import IntegralFormMixed
 from ..constitution import AreaChange
 from ._helpers import Assemble, Results
```

### Comparing `felupe-7.1.0/src/felupe/mesh/_container.py` & `felupe-7.2.0/src/felupe/mesh/_container.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 from copy import deepcopy
 
 import numpy as np
 
 from ._mesh import Mesh
```

### Comparing `felupe-7.1.0/src/felupe/mesh/_convert.py` & `felupe-7.2.0/src/felupe/mesh/_convert.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,27 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 
-from ._discrete_geometry import DiscreteGeometry
 from ._helpers import mesh_or_data
 
 
 @mesh_or_data
 def convert(
     points,
     cells,
@@ -162,38 +152,38 @@
         i = [0, 0, 0, 1]
         j = [1, 1, 2, 2]
         k = [2, 3, 3, 3]
 
         faces_to_stack = cells[:, i], cells[:, j], cells[:, k]
 
     elif "quad" in cell_type:
-        # k-th edge is (i[k], j[k], k[k], l[k])
+        # k-th edge is (i[k], j[k], k[k], m[k])
         i = [
             0,
         ]
         j = [
             1,
         ]
         k = [
             2,
         ]
-        l = [
+        m = [
             3,
         ]
 
-        faces_to_stack = cells[:, i], cells[:, j], cells[:, k], cells[:, l]
+        faces_to_stack = cells[:, i], cells[:, j], cells[:, k], cells[:, m]
 
     elif "hexahedron" in cell_type:
         # k-th edge is (i[k], j[k], k[k], l[k])
         i = [0, 1, 1, 2, 0, 4]
         j = [3, 2, 0, 3, 1, 5]
         k = [7, 6, 4, 7, 2, 6]
-        l = [4, 5, 5, 6, 3, 7]
+        m = [4, 5, 5, 6, 3, 7]
 
-        faces_to_stack = cells[:, i], cells[:, j], cells[:, k], cells[:, l]
+        faces_to_stack = cells[:, i], cells[:, j], cells[:, k], cells[:, m]
 
     # sort points of edges
     faces = np.sort(np.dstack(faces_to_stack).reshape(-1, len(faces_to_stack)), axis=1)
 
     # obtain unique edges and inverse mapping
     faces_unique, inverse = np.unique(faces, False, True, False, 0)
```

### Comparing `felupe-7.1.0/src/felupe/mesh/_discrete_geometry.py` & `felupe-7.2.0/src/felupe/mesh/_discrete_geometry.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 
 
 class DiscreteGeometry:
     """A discrete geometry with points, cells and optional a specified cell type.
@@ -34,15 +25,16 @@
     Parameters
     ----------
     points : ndarray
         Point coordinates.
     cells : ndarray
         Point-connectivity of cells.
     cell_type : str or None, optional
-        An optional string in VTK-convention that specifies the cell type (default is None). Necessary when a discrete geometry is saved to a file.
+        An optional string in VTK-convention that specifies the cell type (default is
+        None). Necessary when a discrete geometry is saved to a file.
 
     Attributes
     ----------
     points : ndarray
         Point coordinates.
     cells : ndarray
         Point-connectivity of cells.
```

### Comparing `felupe-7.1.0/src/felupe/mesh/_geometry.py` & `felupe-7.2.0/src/felupe/mesh/_geometry.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,28 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 
-from ._base import cube_hexa, line_line, rectangle_quad
+from ._line_rectangle_cube import cube_hexa, line_line, rectangle_quad
 from ._mesh import Mesh
 
 
 class Line(Mesh):
     def __init__(self, a=0, b=1, n=2):
         self.a = a
         self.b = b
```

### Comparing `felupe-7.1.0/src/felupe/mesh/_helpers.py` & `felupe-7.2.0/src/felupe/mesh/_helpers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 from functools import wraps
 
 
 def mesh_or_data(meshfun):
     """If a ``DiscreteGeometry`` is passed to a mesh function, extract ``points`` and
```

### Comparing `felupe-7.1.0/src/felupe/mesh/_mesh.py` & `felupe-7.2.0/src/felupe/mesh/_mesh.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 from copy import deepcopy
 from functools import wraps
 
 import numpy as np
 
@@ -65,15 +56,16 @@
     Parameters
     ----------
     points : ndarray
         Point coordinates.
     cells : ndarray
         Point-connectivity of cells.
     cell_type : str or None, optional
-        An optional string in VTK-convention that specifies the cell type (default is None). Necessary when a mesh is saved to a file.
+        An optional string in VTK-convention that specifies the cell type (default is
+        None). Necessary when a mesh is saved to a file.
 
     Attributes
     ----------
     points : ndarray
         Point coordinates.
     cells : ndarray
         Point-connectivity of cells.
@@ -102,15 +94,16 @@
     def __str__(self):
         return self.__repr__()
 
     def disconnect(self, points_per_cell=None, calc_points=True):
         """Return a new instance of a Mesh with disconnected cells. Optionally, the
         points-per-cell may be specified (must be lower or equal the number of points-
         per-cell of the original Mesh). If the Mesh is to be used as a *dual* Mesh, then
-        the point-coordinates do not have to be re-created because they are not used."""
+        the point-coordinates do not have to be re-created because they are not used.
+        """
 
         return self.dual(
             points_per_cell=points_per_cell,
             disconnect=True,
             calc_points=calc_points,
             offset=0,
             npoints=None,
```

### Comparing `felupe-7.1.0/src/felupe/mesh/_read.py` & `felupe-7.2.0/tests/test_solve.py`

 * *Files 26% similar despite different names*

```diff
@@ -23,39 +23,55 @@
 You should have received a copy of the GNU General Public License
 along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
 
 """
 
 import numpy as np
 
-from ._container import MeshContainer
-from ._mesh import Mesh
+import felupe as fe
 
 
-def read(
-    filename, file_format=None, cellblock=None, dim=None, merge=False, decimals=None
-):
-    "Read a mesh-file using meshio and create a felupe mesh-container."
+def test_solve():
 
-    from meshio import read as meshio_read
+    m = fe.Cube(n=3)
+    e = fe.Hexahedron()
+    q = fe.GaussLegendre(1, 3)
+    r = fe.Region(m, e, q)
+    u = fe.Field(r, dim=3)
+    v = fe.FieldContainer([u])
 
-    m = meshio_read(filename=filename, file_format=file_format)
+    W = fe.constitution.NeoHooke(1, 3)
 
-    if dim is None:
-        dim = m.points.shape[1]
+    F = v.extract()
+    P = W.gradient(F)[:-1]
+    A = W.hessian(F)
 
-    points = m.points[:, :dim]
+    b = fe.dof.symmetry(u)
+    dof0, dof1 = fe.dof.partition(v, b)
 
-    if cellblock is None:
-        cellblock = slice(None)
+    ext0 = fe.dof.apply(v, b, dof0)
 
-    cells = m.cells[cellblock]
+    L = fe.IntegralForm(P, v, r.dV)
+    a = fe.IntegralForm(A, v, r.dV, v)
 
-    if not isinstance(cells, list):
-        cells = [cells]
+    b = L.assemble().toarray()[:, 0]
+    A = a.assemble()
 
-    if len(cells) > 0:
-        meshes = [Mesh(points, c.data, c.type) for c in cells]
-    else:
-        meshes = [Mesh(points, np.zeros((0, 0), dtype=int), None)]
+    system = fe.solve.partition(v, A, dof1, dof0)
 
-    return MeshContainer(meshes, merge=merge, decimals=decimals)
+    du = fe.solve.solve(*system)
+    assert np.allclose(du, 0)
+
+    du = fe.solve.solve(*system, ext0)
+    assert np.allclose(du, 0)
+
+    system = fe.solve.partition(v, A, dof1, dof0, b)
+
+    du = fe.solve.solve(*system)
+    assert np.allclose(du, 0)
+
+    du = fe.solve.solve(*system, ext0)
+    assert np.allclose(du, 0)
+
+
+if __name__ == "__main__":
+    test_solve()
```

### Comparing `felupe-7.1.0/src/felupe/mesh/_tools.py` & `felupe-7.2.0/src/felupe/mesh/_tools.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 
 from ..math import rotation_matrix
 from ._helpers import mesh_or_data
 
@@ -473,31 +464,31 @@
 
         # tets out of a hex
         # mode ... no. of diagional through hex-point 6.
         if mode == 0:
             i = [0, 0, 0, 0, 2]
             j = [1, 2, 2, 5, 7]
             k = [2, 7, 3, 7, 5]
-            l = [5, 5, 7, 4, 6]
+            m = [5, 5, 7, 4, 6]
 
         elif mode == 3:
             i = [0, 0, 0, 0, 1, 1]
             j = [2, 3, 7, 5, 5, 6]
             k = [3, 7, 4, 6, 6, 2]
-            l = [6, 6, 6, 4, 0, 0]
+            m = [6, 6, 6, 4, 0, 0]
 
         else:
             raise NotImplementedError(f"Mode {mode} not implemented.")
 
         cells_new = np.dstack(
             (
                 cells[:, i],
                 cells[:, j],
                 cells[:, k],
-                cells[:, l],
+                cells[:, m],
             )
         )
 
         cell_type_new = "tetra"
 
     cells_new = cells_new.reshape(-1, cells_new.shape[-1])
```

### Comparing `felupe-7.1.0/src/felupe/quadrature/_gausslegendre.py` & `felupe-7.2.0/src/felupe/quadrature/_gausslegendre.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 from string import ascii_lowercase
 
 import numpy as np
 
 from . import Scheme
```

### Comparing `felupe-7.1.0/src/felupe/region/__init__.py` & `felupe-7.2.0/src/felupe/region/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,7 +19,33 @@
     RegionTetra,
     RegionTetraMINI,
     RegionTriangle,
     RegionTriangleMINI,
     RegionTriQuadraticHexahedron,
     RegionTriQuadraticHexahedronBoundary,
 )
+
+__all__ = [
+    "RegionBoundary",
+    "Region",
+    "RegionBiQuadraticQuad",
+    "RegionBiQuadraticQuadBoundary",
+    "RegionConstantHexahedron",
+    "RegionConstantQuad",
+    "RegionHexahedron",
+    "RegionHexahedronBoundary",
+    "RegionLagrange",
+    "RegionQuad",
+    "RegionQuadBoundary",
+    "RegionQuadraticHexahedron",
+    "RegionQuadraticHexahedronBoundary",
+    "RegionQuadraticQuad",
+    "RegionQuadraticQuadBoundary",
+    "RegionQuadraticTetra",
+    "RegionQuadraticTriangle",
+    "RegionTetra",
+    "RegionTetraMINI",
+    "RegionTriangle",
+    "RegionTriangleMINI",
+    "RegionTriQuadraticHexahedron",
+    "RegionTriQuadraticHexahedronBoundary",
+]
```

### Comparing `felupe-7.1.0/src/felupe/region/_boundary.py` & `felupe-7.2.0/src/felupe/region/_boundary.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 
 from ..math import cross
 from ..mesh import Mesh
 from ._region import Region
@@ -46,21 +37,21 @@
         )
     )
 
     # complementary edges for the creation of "boundary" quads
     # (rotated quads with 1st edge as n-th edge of one original quad)
     t = [1, 0, 3, 2]
     k = np.array(i)[t]
-    l = np.array(j)[t]
+    m = np.array(j)[t]
 
     cells = np.dstack(
         (
             cells_faces,
             mesh.cells[:, k],
-            mesh.cells[:, l],
+            mesh.cells[:, m],
         )
     )
 
     return cells, cells_faces
 
 
 def boundary_cells_quad8(mesh):
@@ -118,22 +109,22 @@
 def boundary_cells_hexahedron(mesh):
     "Convert the cells array of a hex mesh into a boundary cells array."
 
     # faces (boundary) of a hexahedron
     i = [0, 2, 1, 3, 0, 5]
     j = [3, 1, 0, 2, 1, 4]
     k = [7, 5, 4, 6, 2, 7]
-    l = [4, 6, 5, 7, 3, 6]
+    r = [4, 6, 5, 7, 3, 6]
 
     cells_faces = np.dstack(
         (
             mesh.cells[:, i],
             mesh.cells[:, j],
             mesh.cells[:, k],
-            mesh.cells[:, l],
+            mesh.cells[:, r],
         )
     )
 
     # complementary faces for the creation of "boundary" hexahedrons
     # (6 rotated hexahedrons with 1st face as n-th face of
     #  one original hexahedron)
     m = [1, 3, 2, 0, 4, 1]
@@ -159,23 +150,23 @@
 
     cells_hexahedron, cells_faces_hexahedron = boundary_cells_hexahedron(mesh)
 
     # midpoints on edges of faces (boundary) of a hexahedron
     i = [11, 9, 8, 10, 8, 12]
     j = [19, 17, 16, 18, 9, 15]
     k = [15, 13, 12, 14, 10, 14]
-    l = [16, 18, 17, 19, 11, 13]
+    v = [16, 18, 17, 19, 11, 13]
 
     cells_faces = np.dstack(
         (
             cells_faces_hexahedron,
             mesh.cells[:, i],
             mesh.cells[:, j],
             mesh.cells[:, k],
-            mesh.cells[:, l],
+            mesh.cells[:, v],
         )
     )
 
     # complementary faces for the creation of "boundary" hexahedrons
     # (6 rotated hexahedrons with 1st face as n-th face of
     #  one original hexahedron)
     m = [9, 11, 10, 8, 12, 8]
@@ -190,15 +181,15 @@
 
     cells = np.dstack(
         (
             cells_hexahedron,
             mesh.cells[:, i],
             mesh.cells[:, j],
             mesh.cells[:, k],
-            mesh.cells[:, l],
+            mesh.cells[:, v],
             mesh.cells[:, m],
             mesh.cells[:, n],
             mesh.cells[:, p],
             mesh.cells[:, q],
             mesh.cells[:, r],
             mesh.cells[:, s],
             mesh.cells[:, t],
@@ -225,26 +216,26 @@
     )
 
     # complementary faces for the creation of "boundary" hexahedrons
     # (6 rotated hexahedrons with 1st face as n-th face of
     #  one original hexahedron)
     j = [22, 23, 21, 20, 20, 21]
     k = [23, 22, 20, 21, 21, 20]
-    l = [24, 25, 24, 25, 22, 23]
+    r = [24, 25, 24, 25, 22, 23]
     m = [25, 24, 25, 24, 23, 22]
     n = [20, 21, 22, 23, 24, 25]
     p = [21, 20, 23, 22, 25, 24]
     q = [26, 26, 26, 26, 26, 26]
 
     cells = np.dstack(
         (
             cells_hexahedron20,
             mesh.cells[:, j],
             mesh.cells[:, k],
-            mesh.cells[:, l],
+            mesh.cells[:, r],
             mesh.cells[:, m],
             mesh.cells[:, n],
             mesh.cells[:, p],
             mesh.cells[:, q],
         )
     )
 
@@ -258,15 +249,16 @@
     functions are evaluated at all integration points of each cell in the region
     if the optional gradient argument is True.
 
     .. math::
 
        \frac{\partial X^I}{\partial r^J} &= X_a^I \frac{\partial h_a}{\partial r^J}
 
-       \frac{\partial h_a}{\partial X^J} &= \frac{\partial h_a}{\partial r^I} \frac{\partial r^I}{\partial X^J}
+       \frac{\partial h_a}{\partial X^J} &= \frac{\partial h_a}{\partial r^I}
+       \frac{\partial r^I}{\partial X^J}
 
        dV &= \det\left(\frac{\partial X^I}{\partial r^J}\right) w
 
 
     Parameters
     ----------
     mesh : Mesh
@@ -289,29 +281,38 @@
     mesh : Mesh
         A mesh with points and cells.
     element : Finite element
         The finite element formulation to be applied on the cells.
     quadrature: Quadrature scheme
         An element-compatible numeric integration scheme with points and weights.
     h : ndarray
-        Element shape function array ``h_ap`` of shape function ``a`` evaluated at quadrature point ``p``.
+        Element shape function array ``h_ap`` of shape function ``a`` evaluated at
+        quadrature point ``p``.
     dhdr : ndarray
-        Partial derivative of element shape function array ``dhdr_aJp`` with shape function ``a`` w.r.t. natural element coordinate ``J`` evaluated at quadrature point ``p`` for every cell ``c`` (geometric gradient or **Jacobian** transformation between ``X`` and ``r``).
+        Partial derivative of element shape function array ``dhdr_aJp`` with shape
+        function ``a`` w.r.t. natural element coordinate ``J`` evaluated at quadrature
+        point ``p`` for every cell ``c`` (geometric gradient or **Jacobian**
+        transformation between ``X`` and ``r``).
     dXdr : ndarray
-        Geometric gradient ``dXdr_IJpc`` as partial derivative of undeformed coordinate ``I`` w.r.t. natural element coordinate ``J`` evaluated at quadrature point ``p`` for every cell ``c`` (geometric gradient or **Jacobian** transformation between ``X`` and ``r``).
+        Geometric gradient ``dXdr_IJpc`` as partial derivative of undeformed coordinate
+        ``I`` w.r.t. natural element coordinate ``J`` evaluated at quadrature point
+        ``p`` for every cell ``c`` (geometric gradient or **Jacobian** transformation
+        between ``X`` and ``r``).
     drdX : ndarray
         Inverse of dXdr.
     dA : ndarray
         Numeric *Differential area vectors*.
     normals : ndarray
         Area unit normal vectors.
     dV : ndarray
         Numeric *Differential volume element* as norm of *Differential area vectors*.
     dhdX : ndarray
-        Partial derivative of element shape functions ``dhdX_aJpc`` of shape function ``a`` w.r.t. undeformed coordinate ``J`` evaluated at quadrature point ``p`` for every cell ``c``.
+        Partial derivative of element shape functions ``dhdX_aJpc`` of shape function
+        ``a`` w.r.t. undeformed coordinate ``J`` evaluated at quadrature point ``p`` for
+        every cell ``c``.
     """
 
     def __init__(
         self,
         mesh,
         element,
         quadrature,
@@ -364,15 +365,15 @@
             self._selection = self._selection[
                 np.all(np.isin(cells_faces[self._selection], point_selection), axis=1)
             ]
 
         # get cell-faces and cells on boundary (unique cell-faces with one count)
         cells_on_boundary = cells[self._selection]
 
-        ## create mesh on boundary
+        # create mesh on boundary
         mesh_boundary_cells = mesh.copy()
         mesh_boundary_cells.update(cells_on_boundary)
         self.mesh = mesh_boundary_cells
         self.mesh.cells_faces = cells_faces[self._selection]
 
         # init region and faces
         super().__init__(mesh_boundary_cells, element, quadrature, grad=grad)
```

### Comparing `felupe-7.1.0/src/felupe/region/_templates.py` & `felupe-7.2.0/src/felupe/region/_templates.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,25 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
-import numpy as np
-
 from ..element import (
     ArbitraryOrderLagrange,
     BiQuadraticQuad,
     ConstantHexahedron,
     ConstantQuad,
     Hexahedron,
     Quad,
```

### Comparing `felupe-7.1.0/src/felupe/tools/_newton.py` & `felupe-7.2.0/src/felupe/tools/_newton.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import inspect
 from time import perf_counter
 
 import numpy as np
 from scipy.sparse import csr_matrix
@@ -57,15 +48,14 @@
     [item.field.link(x) for item in items]
 
     # init vector with shape from global field
     shape = (np.sum(x.fieldsizes), 1)
     vector = csr_matrix(shape)
 
     for body in items:
-
         # assemble vector
         r = body.assemble.vector(field=body.field, **kwargs)
 
         # check and reshape vector
         if r.shape != shape:
             r.resize(*shape)
 
@@ -82,15 +72,14 @@
     kwargs = {"parallel": parallel}
 
     # init matrix with shape from global field
     shape = (np.sum(x.fieldsizes), np.sum(x.fieldsizes))
     matrix = csr_matrix(shape)
 
     for body in items:
-
         # assemble matrix
         K = body.assemble.matrix(**kwargs)
 
         # check and reshape matrix
         if K.shape != matrix.shape:
             K.resize(*shape)
 
@@ -135,15 +124,17 @@
 
     return dx
 
 
 def check(dx, x, f, xtol, ftol, dof1=None, dof0=None, items=None, eps=1e-3):
     "Check result."
 
-    sumnorm = lambda x: np.sum(norm(x))
+    def sumnorm(x):
+        return np.sum(norm(x))
+
     xnorm = sumnorm(dx)
 
     if dof1 is None:
         dof1 = slice(None)
 
     if dof0 is None:
         dof0 = slice(0, 0)
@@ -207,15 +198,16 @@
          x = xn + dx                                       (6)
 
     Eq.(5) and Eq.(6) are repeated until `check(dx, x, f)` returns `True`.
 
     """
 
     if verbose:
-        runtime = [perf_counter()]
+        runtimes = [perf_counter()]
+        soltimes = []
 
     if x0 is not None:
         # take x0
         x = x0
 
     else:
         # obtain field of first body
@@ -236,38 +228,37 @@
         print("=====================")
         print()
         print("| # | norm(fun) |  norm(dx) |")
         print("|---|-----------|-----------|")
 
     # iteration loop
     for iteration in range(maxiter):
-
         # evaluate jacobian at unknowns "x"
         if items is not None:
             K = jac_items(items, x, *args, **kwargs)
         else:
             K = jac(x, *args, **kwargs)
 
         # create keyword-arguments for solving the linear system
         keys = ["x", "dof1", "dof0", "ext0", "solver"]
         values = [x, dof1, dof0, ext0, solver]
 
         for key, value in zip(keys, values):
-
             if key in sig.parameters:
                 kwargs_solve[key] = value
 
         # solve linear system and update solution
         if verbose:
-            soltime = [perf_counter()]
+            soltime_start = perf_counter()
 
         dx = solve(K, -f, **kwargs_solve)
 
         if verbose:
-            soltime.append(perf_counter())
+            soltime_end = perf_counter()
+            soltimes.append([soltime_start, soltime_end])
 
         x = update(x, dx)
 
         # evaluate function at unknowns "x"
         if items is not None:
             f = fun_items(items, x, *args, **kwargs)
         else:
@@ -289,14 +280,16 @@
 
     if 1 + iteration == maxiter and not success:
         raise ValueError("Maximum number of iterations reached (not converged).\n")
 
     Res = Result(x=x, fun=f, success=success, iterations=1 + iteration)
 
     if verbose:
-        runtime.append(perf_counter())
+        runtimes.append(perf_counter())
+        runtime = np.diff(runtimes)
+        soltime = np.diff(soltimes).sum()
         print(
             "\nConverged in %d iterations (Assembly: %1.4g s, Solve: %1.4g s).\n"
-            % (iteration + 1, np.diff(runtime) - np.diff(soltime), np.diff(soltime))
+            % (iteration + 1, runtime - soltime, soltime)
         )
 
     return Res
```

### Comparing `felupe-7.1.0/src/felupe/tools/_project.py` & `felupe-7.2.0/src/felupe/tools/_project.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 from scipy.sparse import csr_matrix as sparsematrix
 
 from .._field import Field
 from ..region import Region
```

### Comparing `felupe-7.1.0/src/felupe/tools/_save.py` & `felupe-7.2.0/src/felupe/tools/_save.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # -*- coding: utf-8 -*-
 """
- _______  _______  ___      __   __  _______  _______ 
-|       ||       ||   |    |  | |  ||       ||       |
-|    ___||    ___||   |    |  | |  ||    _  ||    ___|
-|   |___ |   |___ |   |    |  |_|  ||   |_| ||   |___ 
-|    ___||    ___||   |___ |       ||    ___||    ___|
-|   |    |   |___ |       ||       ||   |    |   |___ 
-|___|    |_______||_______||_______||___|    |_______|
+This file is part of FElupe.
 
-This file is part of felupe.
-
-Felupe is free software: you can redistribute it and/or modify
+FElupe is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
-Felupe is distributed in the hope that it will be useful,
+FElupe is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with Felupe.  If not, see <http://www.gnu.org/licenses/>.
-
+along with FElupe.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import numpy as np
 
 from ..math import det, dot, eigvalsh, transpose
 from . import topoints
```

### Comparing `felupe-7.1.0/src/felupe.egg-info/PKG-INFO` & `felupe-7.2.0/src/felupe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: felupe
-Version: 7.1.0
+Version: 7.2.0
 Summary: Finite Element Analysis
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -700,70 +700,86 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: all
 License-File: LICENSE
 
-# 🔍 FElupe - Finite Element Analysis
+# 🔍 FElupe
 
-[![PyPI version shields.io](https://img.shields.io/pypi/v/felupe.svg)](https://pypi.python.org/pypi/felupe/) [![Documentation Status](https://readthedocs.org/projects/felupe/badge/?version=latest)](https://felupe.readthedocs.io/en/latest/?badge=latest) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) ![Made with love in Graz (Austria)](https://img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20in-Graz%20(Austria)-0c674a) [![codecov](https://codecov.io/gh/adtzlr/felupe/branch/main/graph/badge.svg?token=J2QP6Y6LVH)](https://codecov.io/gh/adtzlr/felupe) [![DOI](https://zenodo.org/badge/360657894.svg)](https://zenodo.org/badge/latestdoi/360657894) ![Codestyle black](https://img.shields.io/badge/code%20style-black-black) ![GitHub Repo stars](https://img.shields.io/github/stars/adtzlr/felupe?logo=github) ![PyPI - Downloads](https://img.shields.io/pypi/dm/felupe)
+[![PyPI version shields.io](https://img.shields.io/pypi/v/felupe.svg)](https://pypi.python.org/pypi/felupe/) [![Documentation Status](https://readthedocs.org/projects/felupe/badge/?version=latest)](https://felupe.readthedocs.io/en/latest/?badge=latest) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) ![Made with love in Graz (Austria)](https://img.shields.io/badge/Made%20with%20%E2%9D%A4%EF%B8%8F%20in-Graz%20(Austria)-0c674a) [![codecov](https://codecov.io/gh/adtzlr/felupe/branch/main/graph/badge.svg?token=J2QP6Y6LVH)](https://codecov.io/gh/adtzlr/felupe) [![DOI](https://zenodo.org/badge/360657894.svg)](https://zenodo.org/badge/latestdoi/360657894) ![Codestyle black](https://img.shields.io/badge/code%20style-black-black) ![GitHub Repo stars](https://img.shields.io/github/stars/adtzlr/felupe?logo=github) ![PyPI - Downloads](https://img.shields.io/pypi/dm/felupe) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/adtzlr/felupe/HEAD) [![lite-badge](https://jupyterlite.rtfd.io/en/latest/_static/badge.svg)](https://adtzlr.github.io/felupe-web/lab?path=01_Getting+Started.ipynb) <a target="_blank" href="https://colab.research.google.com/github/adtzlr/felupe-web/blob/main/content/01_Getting%20Started.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
+
+> Finite Element Analysis
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/adtzlr/felupe/main/docs/_static/logo_light.svg" height="120px"/> <a href="https://felupe.readthedocs.io/en/latest/examples/rubberspring.html"><img src="https://user-images.githubusercontent.com/5793153/230604246-5a416081-6777-4f33-afdf-efdb51338722.png" height="120px"/></a> <a href="https://felupe.readthedocs.io/en/latest/examples/platewithhole.html"><img src="https://user-images.githubusercontent.com/5793153/230604587-42e3e339-e08c-4cc8-8000-f7046a8d95df.png" height="120px"/></a>
 </p>
 
 FElupe is a Python 3.7+ finite element analysis package focussing on the formulation and numerical solution of nonlinear problems in continuum mechanics of solid bodies. Its name is a combination of FE (finite element) and the german word *Lupe* (magnifying glass) as a synonym for getting an insight how a finite element analysis code looks like under the hood.
 
 # Installation
 Install Python, fire up a terminal and run
 
 ```shell
 pip install felupe[all]
 ```
 
-where `[all]` installs all optional dependencies. By default, FElupe depends on `numpy` and `scipy`. In order to make use of all features of FElupe, it is suggested to install all optional dependencies (`einsumt`, `h5py`, `matplotlib`, `meshio` and `tensortrax`).
+where `[all]` installs all optional dependencies. By default, FElupe depends on `numpy`, `scipy` and `tensortrax`. In order to make use of all features of FElupe, it is suggested to install all optional dependencies (`einsumt`, `h5py`, `matplotlib`, `meshio` and `pyvista`).
 
 # Getting Started
-A quarter model of a solid cube with hyperelastic material behaviour is subjected to a uniaxial elongation applied at a clamped end-face. This involves the creation of a mesh, a region as well as a displacement field (encapsulated in a field container). Furthermore, the boundary conditions are created by a template for a uniaxial loadcase. An isotropic pseudo-elastic Ogden-Roxburgh Mullins-softening model formulation in combination with an isotropic hyperelastic Neo-Hookean material formulation is applied on a nearly-incompressible solid body. A step generates the consecutive substep-movements of a given boundary condition. The step is further added to a list of steps of a job (here, a characteristic-curve job is used). During evaluation, each substep of each step is solved by an iterative Newton-Rhapson procedure. The solution is exported after each completed substep as a time-series XDMF file. For more details beside this high-level code snippet, please have a look at the [documentation](https://felupe.readthedocs.io/en/latest/?badge=latest).
+This tutorial covers the essential high-level parts of creating and solving problems with FElupe. As an introductory example, a quarter model of a solid cube with hyperelastic material behaviour is subjected to a uniaxial elongation applied at a clamped end-face. 
+
+First, let’s import FElupe and create a meshed cube out of hexahedron cells with 6 points per axis. A numeric region, pre-defined for hexahedrons, is created on the mesh. A vector-valued displacement field is initiated on the region. Next, a field container is created on top of this field. 
+
+A uniaxial load case is applied on the displacement field stored inside the field container. This involves setting up symmetry planes as well as the absolute value of the prescribed displacement at the mesh-points on the right-end face of the cube. The right-end face is *clamped*: only displacements in direction *x* are allowed. The dict of boundary conditions for this pre-defined load case are returned as `boundaries` and the partitioned degrees of freedom as well as the external displacements are stored within the returned dict `loadcase`. 
+
+An isotropic pseudo-elastic Ogden-Roxburgh Mullins-softening model formulation in combination with an isotropic hyperelastic Neo-Hookean material formulation is applied on the displacement field of a nearly-incompressible solid body. 
+
+A step generates the consecutive substep-movements of a given boundary condition. The step is further added to a list of steps of a job (here, a characteristic-curve job is used). During evaluation, each substep of each step is solved by an iterative Newton-Rhapson procedure. The solution is exported after each completed substep as a time-series XDMF file. Finally, the result of the last completed substep is plotted.
+
+For more details beside this high-level code snippet, please have a look at the [documentation](https://felupe.readthedocs.io/en/latest/?badge=latest).
 
 ```python
 import felupe as fem
 
 # create a hexahedron-region on a cube
-mesh = fem.Cube(n=11)
+mesh = fem.Cube(n=6)
 region = fem.RegionHexahedron(mesh)
 
 # add a field container (with a vector-valued displacement field)
 field = fem.FieldContainer([fem.Field(region, dim=3)])
 
 # apply a uniaxial elongation on the cube
-boundaries = fem.dof.uniaxial(field, clamped=True)[0]
+boundaries, loadcase = fem.dof.uniaxial(field, clamped=True)
 
 # define the constitutive material behaviour
 # and create a nearly-incompressible (u,p,J - formulation) solid body
 umat = fem.OgdenRoxburgh(material=fem.NeoHooke(mu=1), r=3, m=1, beta=0)
 solid = fem.SolidBodyNearlyIncompressible(umat, field, bulk=5000)
 
 # prepare a step with substeps
-move = fem.math.linsteps([0, 2, 0], num=10)
+move = fem.math.linsteps([0, 1, 0, 1, 2, 1], num=5)
 step = fem.Step(items=[solid], ramp={boundaries["move"]: move}, boundaries=boundaries)
 
 # add the step to a job, evaluate all substeps and create a plot
 job = fem.CharacteristicCurve(steps=[step], boundary=boundaries["move"])
 job.evaluate(filename="result.xdmf")
 fig, ax = job.plot(
     xlabel="Displacement $u$ in mm $\longrightarrow$",
     ylabel="Normal Force $F$ in N $\longrightarrow$",
 )
+
+# visualize the results
+view = fem.View(field)
+view.plot("Principal Values of Logarithmic Strain").show()
 ```
 
-https://user-images.githubusercontent.com/5793153/200951381-ea310e54-7623-4dd1-a55f-a28f9055063f.mp4
+![curve](https://user-images.githubusercontent.com/5793153/234382805-d9a56108-9dd7-4f57-a029-571a5a2486a4.svg)
 
-<img src="https://raw.githubusercontent.com/adtzlr/felupe/main/docs/_static/readme_characteristic_curve.svg" width="600px"/>
+![cube](https://user-images.githubusercontent.com/5793153/234405093-2f5201c1-3bba-46ee-bd91-af87813609d9.png)
 
 # Documentation
 The documentation is located [here](https://felupe.readthedocs.io/en/latest/?badge=latest).
 
 # Extension Packages
 The capabilities of FElupe may be enhanced with extension packages created by the community.
```

### Comparing `felupe-7.1.0/src/felupe.egg-info/SOURCES.txt` & `felupe-7.2.0/src/felupe.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -57,21 +57,21 @@
 src/felupe/mechanics/_pointload.py
 src/felupe/mechanics/_solidbody.py
 src/felupe/mechanics/_solidbody_gravity.py
 src/felupe/mechanics/_solidbody_incompressible.py
 src/felupe/mechanics/_solidbody_pressure.py
 src/felupe/mechanics/_step.py
 src/felupe/mesh/__init__.py
-src/felupe/mesh/_base.py
 src/felupe/mesh/_container.py
 src/felupe/mesh/_convert.py
 src/felupe/mesh/_discrete_geometry.py
 src/felupe/mesh/_dual.py
 src/felupe/mesh/_geometry.py
 src/felupe/mesh/_helpers.py
+src/felupe/mesh/_line_rectangle_cube.py
 src/felupe/mesh/_mesh.py
 src/felupe/mesh/_read.py
 src/felupe/mesh/_tools.py
 src/felupe/quadrature/__init__.py
 src/felupe/quadrature/_base.py
 src/felupe/quadrature/_gausslegendre.py
 src/felupe/quadrature/_tetra.py
@@ -80,14 +80,15 @@
 src/felupe/region/_boundary.py
 src/felupe/region/_region.py
 src/felupe/region/_templates.py
 src/felupe/solve/__init__.py
 src/felupe/solve/_solve.py
 src/felupe/tools/__init__.py
 src/felupe/tools/_newton.py
+src/felupe/tools/_plot.py
 src/felupe/tools/_post.py
 src/felupe/tools/_project.py
 src/felupe/tools/_save.py
 src/felupe/tools/_solve.py
 tests/test_basis.py
 tests/test_bilinearform.py
 tests/test_composite.py
@@ -98,12 +99,13 @@
 tests/test_form.py
 tests/test_job.py
 tests/test_math.py
 tests/test_mechanics.py
 tests/test_mesh.py
 tests/test_mpc.py
 tests/test_planestrain.py
+tests/test_plot.py
 tests/test_quadrature.py
 tests/test_readme.py
 tests/test_region.py
 tests/test_solve.py
 tests/test_tools.py
```

### Comparing `felupe-7.1.0/tests/test_composite.py` & `felupe-7.2.0/tests/test_composite.py`

 * *Files identical despite different names*

### Comparing `felupe-7.1.0/tests/test_constitution.py` & `felupe-7.2.0/tests/test_constitution.py`

 * *Files identical despite different names*

### Comparing `felupe-7.1.0/tests/test_dof.py` & `felupe-7.2.0/tests/test_dof.py`

 * *Files identical despite different names*

### Comparing `felupe-7.1.0/tests/test_element.py` & `felupe-7.2.0/tests/test_element.py`

 * *Files identical despite different names*

### Comparing `felupe-7.1.0/tests/test_field.py` & `felupe-7.2.0/tests/test_field.py`

 * *Files identical despite different names*

### Comparing `felupe-7.1.0/tests/test_form.py` & `felupe-7.2.0/tests/test_form.py`

 * *Files identical despite different names*

### Comparing `felupe-7.1.0/tests/test_job.py` & `felupe-7.2.0/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `felupe-7.1.0/tests/test_math.py` & `felupe-7.2.0/tests/test_math.py`

 * *Files 10% similar despite different names*

```diff
@@ -72,47 +72,45 @@
 
     with pytest.raises(ValueError):
         fe.math.dya(a, a, mode=3)
 
     fe.math.sym(H)
 
     fe.math.dot(C, C)
-    fe.math.dot(C, A)
-    fe.math.dot(A, C)
+    fe.math.dot(C, A, mode=(2, 4))
+    fe.math.dot(A, C, mode=(4, 2))
 
     fe.math.transpose(F, mode=1)
     fe.math.transpose(A, mode=2)
 
     with pytest.raises(ValueError):
         fe.math.transpose(F, mode=3)
 
     with pytest.raises(TypeError):
-        fe.math.dot(C, B)
+        fe.math.dot(C, B, mode=(2, 3))
+        fe.math.dot(B, C, mode=(3, 2))
 
-    with pytest.raises(TypeError):
-        fe.math.dot(B, C)
-
-    assert fe.math.dot(C, a).shape == (3, 8, 200)
-    assert fe.math.dot(a, C).shape == (3, 8, 200)
-    assert fe.math.dot(a, a).shape == (8, 200)
-
-    assert fe.math.dot(a, A).shape == (3, 3, 3, 8, 200)
-    assert fe.math.dot(A, a).shape == (3, 3, 3, 8, 200)
-    assert fe.math.dot(A, A).shape == (3, 3, 3, 3, 3, 3, 8, 200)
-
-    assert fe.math.ddot(C, C).shape == (8, 200)
-    assert fe.math.ddot(C, A).shape == (3, 3, 8, 200)
-    assert fe.math.ddot(A, C).shape == (3, 3, 8, 200)
+    assert fe.math.dot(C, a, mode=(2, 1)).shape == (3, 8, 200)
+    assert fe.math.dot(a, C, mode=(1, 2)).shape == (3, 8, 200)
+    assert fe.math.dot(a, a, mode=(1, 1)).shape == (8, 200)
+
+    assert fe.math.dot(a, A, mode=(1, 4)).shape == (3, 3, 3, 8, 200)
+    assert fe.math.dot(A, a, mode=(4, 1)).shape == (3, 3, 3, 8, 200)
+    assert fe.math.dot(A, A, mode=(4, 4)).shape == (3, 3, 3, 3, 3, 3, 8, 200)
+
+    assert fe.math.ddot(C, C, mode=(2, 2)).shape == (8, 200)
+    assert fe.math.ddot(C, A, mode=(2, 4)).shape == (3, 3, 8, 200)
+    assert fe.math.ddot(A, C, mode=(4, 2)).shape == (3, 3, 8, 200)
 
-    assert fe.math.ddot(A, A).shape == (3, 3, 3, 3, 8, 200)
+    assert fe.math.ddot(A, A, mode=(4, 4)).shape == (3, 3, 3, 3, 8, 200)
 
     with pytest.raises(TypeError):
-        fe.math.ddot(A, B)
-        fe.math.ddot(B, B)
-        fe.math.ddot(C, B)
+        fe.math.ddot(A, B, mode=(4, 3))
+        fe.math.ddot(B, B, mode=(3, 3))
+        fe.math.ddot(C, B, mode=(2, 3))
 
     detC = fe.math.det(C)
     fe.math.det(C[:2, :2])
     fe.math.det(C[:1, :1])
 
     fe.math.inv(C)
     fe.math.inv(C[:2, :2])
```

### Comparing `felupe-7.1.0/tests/test_mechanics.py` & `felupe-7.2.0/tests/test_mechanics.py`

 * *Files identical despite different names*

### Comparing `felupe-7.1.0/tests/test_mesh.py` & `felupe-7.2.0/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `felupe-7.1.0/tests/test_mpc.py` & `felupe-7.2.0/tests/test_mpc.py`

 * *Files identical despite different names*

### Comparing `felupe-7.1.0/tests/test_planestrain.py` & `felupe-7.2.0/tests/test_planestrain.py`

 * *Files identical despite different names*

### Comparing `felupe-7.1.0/tests/test_quadrature.py` & `felupe-7.2.0/tests/test_quadrature.py`

 * *Files identical despite different names*

### Comparing `felupe-7.1.0/tests/test_readme.py` & `felupe-7.2.0/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `felupe-7.1.0/tests/test_region.py` & `felupe-7.2.0/tests/test_region.py`

 * *Files identical despite different names*

### Comparing `felupe-7.1.0/tests/test_tools.py` & `felupe-7.2.0/tests/test_tools.py`

 * *Files identical despite different names*

