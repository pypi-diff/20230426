# Comparing `tmp/tidy3d-2.1.0.tar.gz` & `tmp/tidy3d-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidy3d-2.1.0.tar", last modified: Tue Apr 18 20:46:11 2023, max compression
+gzip compressed data, was "tidy3d-2.1.1.tar", last modified: Tue Apr 25 18:27:59 2023, max compression
```

## Comparing `tidy3d-2.1.0.tar` & `tidy3d-2.1.1.tar`

### file list

```diff
@@ -1,193 +1,193 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.198248 tidy3d-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-04-18 20:45:52.000000 tidy3d-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-18 20:45:52.000000 tidy3d-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-04-18 20:46:11.198248 tidy3d-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-04-18 20:45:52.000000 tidy3d-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-18 20:45:52.000000 tidy3d-2.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.174246 tidy3d-2.1.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-18 20:45:52.000000 tidy3d-2.1.0/requirements/basic.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-18 20:45:52.000000 tidy3d-2.1.0/requirements/core.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-18 20:45:52.000000 tidy3d-2.1.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-18 20:45:52.000000 tidy3d-2.1.0/requirements/gdspy.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-18 20:45:52.000000 tidy3d-2.1.0/requirements/gdstk.txt
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-18 20:45:52.000000 tidy3d-2.1.0/requirements/jax.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-18 20:45:52.000000 tidy3d-2.1.0/requirements/trimesh.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-18 20:45:52.000000 tidy3d-2.1.0/requirements/web.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-18 20:45:52.000000 tidy3d-2.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 20:46:11.198248 tidy3d-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-18 20:45:52.000000 tidy3d-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.174246 tidy3d-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.174246 tidy3d-2.1.0/tests/_test_local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/_test_local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/_test_local/_test_adjoint_performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/_test_local/_test_data_performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/_test_local/_test_fit_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/_test_local/_test_plugins_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/_test_local/_test_web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.178246 tidy3d-2.1.0/tests/test_components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_components/test_IO.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_components/test_apodization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_components/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_components/test_boundaries.py
--rw-r--r--   0 runner    (1001) docker     (123)    10844 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_components/test_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_components/test_field_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19253 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_components/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_components/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_components/test_grid_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_components/test_medium.py
--rw-r--r--   0 runner    (1001) docker     (123)    22157 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_components/test_meshgenerate.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_components/test_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_components/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    21134 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_components/test_sidewall.py
--rw-r--r--   0 runner    (1001) docker     (123)    49798 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_components/test_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_components/test_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_components/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_components/test_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.178246 tidy3d-2.1.0/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_data/test_data_arrays.py
--rw-r--r--   0 runner    (1001) docker     (123)    19395 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_data/test_monitor_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_data/test_sim_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.178246 tidy3d-2.1.0/tests/test_package/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_package/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_package/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_package/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_package/test_make_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_package/test_material_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_package/test_parametric_variants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.178246 tidy3d-2.1.0/tests/test_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25771 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_plugins/test_adjoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    12530 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_plugins/test_component_modeler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_plugins/test_dispersion_fitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_plugins/test_mode_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_plugins/test_polyslab.py
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_plugins/test_resonance_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_plugins/test_waveguide.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.182247 tidy3d-2.1.0/tests/test_web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_web/mock_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_web/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_web/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_web/test_material_fitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_web/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_web/test_tidy3d_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_web/test_tidy3d_material_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_web/test_tidy3d_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    15992 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/test_web/test_webapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    15225 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.182247 tidy3d-2.1.0/tidy3d/
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.186247 tidy3d-2.1.0/tidy3d/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/apodization.py
--rw-r--r--   0 runner    (1001) docker     (123)    23162 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    23749 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/boundary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.186247 tidy3d-2.1.0/tidy3d/components/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13878 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/data/data_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    14266 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    77646 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/data/monitor_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    27869 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/data/sim_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    35154 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/field_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)   146855 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.186247 tidy3d-2.1.0/tidy3d/components/grid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14955 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/grid/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    23735 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/grid/grid_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    47455 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/grid/mesher.py
--rw-r--r--   0 runner    (1001) docker     (123)    57298 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/medium.py
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    29507 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)   115895 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    32922 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/components/viz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.186247 tidy3d-2.1.0/tidy3d/material_library/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/material_library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62029 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/material_library/material_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/material_library/material_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    15029 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/material_library/parametric_materials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.186247 tidy3d-2.1.0/tidy3d/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.190247 tidy3d-2.1.0/tidy3d/plugins/adjoint/
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/adjoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.190247 tidy3d-2.1.0/tidy3d/plugins/adjoint/components/
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/adjoint/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/adjoint/components/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.190247 tidy3d-2.1.0/tidy3d/plugins/adjoint/components/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/adjoint/components/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7791 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/adjoint/components/data/data_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/adjoint/components/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12145 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/adjoint/components/data/monitor_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/adjoint/components/data/sim_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    18360 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/adjoint/components/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/adjoint/components/medium.py
--rw-r--r--   0 runner    (1001) docker     (123)    12607 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/adjoint/components/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/adjoint/components/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/adjoint/components/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/adjoint/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.190247 tidy3d-2.1.0/tidy3d/plugins/dispersion/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/dispersion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23663 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/dispersion/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/dispersion/fit_web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.190247 tidy3d-2.1.0/tidy3d/plugins/mode/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/mode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/mode/derivatives.py
--rw-r--r--   0 runner    (1001) docker     (123)    25011 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/mode/mode_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    24731 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/mode/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/mode/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.190247 tidy3d-2.1.0/tidy3d/plugins/polyslab/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/polyslab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/polyslab/polyslab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.190247 tidy3d-2.1.0/tidy3d/plugins/resonance/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/resonance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/resonance/resonance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.194247 tidy3d-2.1.0/tidy3d/plugins/smatrix/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/smatrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19999 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/smatrix/smatrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.194247 tidy3d-2.1.0/tidy3d/plugins/waveguide/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/waveguide/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35573 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/plugins/waveguide/rectangular_dielectric.py
--rw-r--r--   0 runner    (1001) docker     (123)    10884 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/updater.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.194247 tidy3d-2.1.0/tidy3d/web/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/asynchronous.py
--rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)   275233 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/cacert.pem
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.198248 tidy3d-2.1.0/tidy3d/web/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/cli/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/cli/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/cli/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    19165 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/http_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/httputils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/material_fitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/material_libray.py
--rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/s3utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15194 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/simulation_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    21709 2023-04-18 20:45:52.000000 tidy3d-2.1.0/tidy3d/web/webapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:11.182247 tidy3d-2.1.0/tidy3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-04-18 20:46:11.000000 tidy3d-2.1.0/tidy3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-04-18 20:46:11.000000 tidy3d-2.1.0/tidy3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:46:11.000000 tidy3d-2.1.0/tidy3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-18 20:46:11.000000 tidy3d-2.1.0/tidy3d.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-18 20:46:11.000000 tidy3d-2.1.0/tidy3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-18 20:46:11.000000 tidy3d-2.1.0/tidy3d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.092064 tidy3d-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-04-25 18:27:42.000000 tidy3d-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-25 18:27:42.000000 tidy3d-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-04-25 18:27:59.092064 tidy3d-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-04-25 18:27:42.000000 tidy3d-2.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-25 18:27:42.000000 tidy3d-2.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.060063 tidy3d-2.1.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-25 18:27:42.000000 tidy3d-2.1.1/requirements/basic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-25 18:27:42.000000 tidy3d-2.1.1/requirements/core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-25 18:27:42.000000 tidy3d-2.1.1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-25 18:27:42.000000 tidy3d-2.1.1/requirements/gdspy.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-25 18:27:42.000000 tidy3d-2.1.1/requirements/gdstk.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-25 18:27:42.000000 tidy3d-2.1.1/requirements/jax.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-25 18:27:42.000000 tidy3d-2.1.1/requirements/trimesh.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-25 18:27:42.000000 tidy3d-2.1.1/requirements/web.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-25 18:27:42.000000 tidy3d-2.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 18:27:59.092064 tidy3d-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-25 18:27:42.000000 tidy3d-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.060063 tidy3d-2.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.060063 tidy3d-2.1.1/tests/_test_local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/_test_local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/_test_local/_test_adjoint_performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/_test_local/_test_data_performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/_test_local/_test_fit_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/_test_local/_test_plugins_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/_test_local/_test_web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.064063 tidy3d-2.1.1/tests/test_components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_components/test_IO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_components/test_apodization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_components/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_components/test_boundaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10844 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_components/test_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_components/test_field_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19253 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_components/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_components/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_components/test_grid_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_components/test_medium.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22157 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_components/test_meshgenerate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_components/test_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_components/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21134 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_components/test_sidewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49787 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_components/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_components/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_components/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_components/test_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.064063 tidy3d-2.1.1/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_data/test_data_arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19395 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_data/test_monitor_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12848 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_data/test_sim_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.068063 tidy3d-2.1.1/tests/test_package/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_package/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_package/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_package/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_package/test_make_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_package/test_material_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_package/test_parametric_variants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.068063 tidy3d-2.1.1/tests/test_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25771 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_plugins/test_adjoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12530 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_plugins/test_component_modeler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_plugins/test_dispersion_fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_plugins/test_mode_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_plugins/test_polyslab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_plugins/test_resonance_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_plugins/test_waveguide.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.072064 tidy3d-2.1.1/tests/test_web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_web/mock_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_web/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_web/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_web/test_material_fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_web/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_web/test_tidy3d_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_web/test_tidy3d_material_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_web/test_tidy3d_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15990 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/test_web/test_webapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15225 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.072064 tidy3d-2.1.1/tidy3d/
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.076063 tidy3d-2.1.1/tidy3d/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/apodization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23177 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23749 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/boundary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.080064 tidy3d-2.1.1/tidy3d/components/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13878 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/data/data_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14266 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77646 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/data/monitor_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27869 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/data/sim_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35154 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/field_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)   146851 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.080064 tidy3d-2.1.1/tidy3d/components/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14955 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/grid/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23735 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/grid/grid_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47455 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/grid/mesher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57298 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/medium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29507 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115912 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32922 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/components/viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.080064 tidy3d-2.1.1/tidy3d/material_library/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/material_library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62029 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/material_library/material_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/material_library/material_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15029 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/material_library/parametric_materials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.080064 tidy3d-2.1.1/tidy3d/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.080064 tidy3d-2.1.1/tidy3d/plugins/adjoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/adjoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.084064 tidy3d-2.1.1/tidy3d/plugins/adjoint/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/adjoint/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/adjoint/components/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.084064 tidy3d-2.1.1/tidy3d/plugins/adjoint/components/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/adjoint/components/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7791 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/adjoint/components/data/data_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/adjoint/components/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12145 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/adjoint/components/data/monitor_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/adjoint/components/data/sim_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18360 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/adjoint/components/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/adjoint/components/medium.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12607 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/adjoint/components/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/adjoint/components/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/adjoint/components/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/adjoint/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.084064 tidy3d-2.1.1/tidy3d/plugins/dispersion/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/dispersion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23663 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/dispersion/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/dispersion/fit_web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.084064 tidy3d-2.1.1/tidy3d/plugins/mode/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/mode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/mode/derivatives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25011 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/mode/mode_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24731 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/mode/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/mode/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.084064 tidy3d-2.1.1/tidy3d/plugins/polyslab/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/polyslab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/polyslab/polyslab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.084064 tidy3d-2.1.1/tidy3d/plugins/resonance/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/resonance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/resonance/resonance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.084064 tidy3d-2.1.1/tidy3d/plugins/smatrix/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/smatrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19999 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/smatrix/smatrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.084064 tidy3d-2.1.1/tidy3d/plugins/waveguide/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/waveguide/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35573 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/plugins/waveguide/rectangular_dielectric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10884 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.092064 tidy3d-2.1.1/tidy3d/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/asynchronous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)   275233 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/cacert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.092064 tidy3d-2.1.1/tidy3d/web/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/cli/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/cli/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/cli/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19165 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/http_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/httputils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/material_fitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/material_libray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/s3utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15189 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/simulation_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21709 2023-04-25 18:27:42.000000 tidy3d-2.1.1/tidy3d/web/webapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:27:59.072064 tidy3d-2.1.1/tidy3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-04-25 18:27:59.000000 tidy3d-2.1.1/tidy3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-04-25 18:27:59.000000 tidy3d-2.1.1/tidy3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 18:27:59.000000 tidy3d-2.1.1/tidy3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-25 18:27:59.000000 tidy3d-2.1.1/tidy3d.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-25 18:27:59.000000 tidy3d-2.1.1/tidy3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-25 18:27:59.000000 tidy3d-2.1.1/tidy3d.egg-info/top_level.txt
```

### Comparing `tidy3d-2.1.0/LICENSE` & `tidy3d-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/PKG-INFO` & `tidy3d-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidy3d
-Version: 2.1.0
+Version: 2.1.1
 Summary: A fast FDTD solver
 Home-page: https://github.com/flexcompute/tidy3d
 Author: Tyler Hughes
 Author-email: tyler@flexcompute.com
 Project-URL: Bug Tracker, https://github.com/flexcompute/tidy3d/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidy3d-2.1.0/README.md` & `tidy3d-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/setup.py` & `tidy3d-2.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/_test_local/_test_adjoint_performance.py` & `tidy3d-2.1.1/tests/_test_local/_test_adjoint_performance.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/_test_local/_test_data_performance.py` & `tidy3d-2.1.1/tests/_test_local/_test_data_performance.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/_test_local/_test_fit_web.py` & `tidy3d-2.1.1/tests/_test_local/_test_fit_web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/_test_local/_test_plugins_web.py` & `tidy3d-2.1.1/tests/_test_local/_test_plugins_web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/_test_local/_test_web.py` & `tidy3d-2.1.1/tests/_test_local/_test_web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/test_components/test_IO.py` & `tidy3d-2.1.1/tests/test_components/test_IO.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/test_components/test_apodization.py` & `tidy3d-2.1.1/tests/test_components/test_apodization.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/test_components/test_base.py` & `tidy3d-2.1.1/tests/test_components/test_base.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/test_components/test_boundaries.py` & `tidy3d-2.1.1/tests/test_components/test_boundaries.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/test_components/test_custom.py` & `tidy3d-2.1.1/tests/test_components/test_custom.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/test_components/test_field_projection.py` & `tidy3d-2.1.1/tests/test_components/test_field_projection.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/test_components/test_geometry.py` & `tidy3d-2.1.1/tests/test_components/test_geometry.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/test_components/test_grid.py` & `tidy3d-2.1.1/tests/test_components/test_grid.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/test_components/test_grid_spec.py` & `tidy3d-2.1.1/tests/test_components/test_grid_spec.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/test_components/test_medium.py` & `tidy3d-2.1.1/tests/test_components/test_medium.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/test_components/test_meshgenerate.py` & `tidy3d-2.1.1/tests/test_components/test_meshgenerate.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/test_components/test_mode.py` & `tidy3d-2.1.1/tests/test_components/test_mode.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/test_components/test_monitor.py` & `tidy3d-2.1.1/tests/test_components/test_monitor.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/test_components/test_sidewall.py` & `tidy3d-2.1.1/tests/test_components/test_sidewall.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/test_components/test_simulation.py` & `tidy3d-2.1.1/tests/test_components/test_simulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -882,20 +882,18 @@
 
     assert_log_level(log_capture, log_level)
 
 
 @pytest.mark.parametrize(
     "box_length,absorb_type,log_level",
     [
-        (0, "PML", "INFO"),
-        (0.5, "PML", "INFO"),
-        (1, "PML", "INFO"),
-        (1.5, "PML", "WARNING"),
-        (1.5, "absorber", "INFO"),
-        (5.0, "PML", "INFO"),
+        (0, "PML", None),
+        (1, "PML", "WARNING"),
+        (1.5, "absorber", None),
+        (2.0, "PML", None),
     ],
 )
 def test_sim_validate_structure_bounds_pml(log_capture, box_length, absorb_type, log_level):
     """Make sure we warn if structure bounds are within the PML exactly to simulation edges."""
 
     boundary = td.PML() if absorb_type == "PML" else td.Absorber()
 
@@ -907,17 +905,18 @@
     box = td.Structure(
         geometry=td.Box(size=(box_length, 0.5, 0.5), center=(0, 0, 0)),
         medium=td.Medium(permittivity=2),
     )
     sim = td.Simulation(
         size=(1, 1, 1),
         structures=[box],
+        grid_spec=td.GridSpec.auto(wavelength=0.001),
         sources=[src],
         run_time=1e-12,
-        boundary_spec=td.BoundarySpec.all_sides(boundary=boundary),
+        boundary_spec=td.BoundarySpec.pml(x=True, y=False, z=False),
     )
 
     assert_log_level(log_capture, log_level)
 
 
 def test_num_mediums():
     """Make sure we error if too many mediums supplied."""
```

### Comparing `tidy3d-2.1.0/tests/test_components/test_source.py` & `tidy3d-2.1.1/tests/test_components/test_source.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/test_components/test_types.py` & `tidy3d-2.1.1/tests/test_components/test_types.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/test_data/test_data_arrays.py` & `tidy3d-2.1.1/tests/test_data/test_data_arrays.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/test_data/test_monitor_data.py` & `tidy3d-2.1.1/tests/test_data/test_monitor_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/test_data/test_sim_data.py` & `tidy3d-2.1.1/tests/test_data/test_sim_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/test_package/test_config.py` & `tidy3d-2.1.1/tests/test_package/test_config.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/test_package/test_log.py` & `tidy3d-2.1.1/tests/test_package/test_log.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/test_package/test_make_script.py` & `tidy3d-2.1.1/tests/test_package/test_make_script.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/test_package/test_material_library.py` & `tidy3d-2.1.1/tests/test_package/test_material_library.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/test_package/test_parametric_variants.py` & `tidy3d-2.1.1/tests/test_package/test_parametric_variants.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/test_plugins/test_adjoint.py` & `tidy3d-2.1.1/tests/test_plugins/test_adjoint.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/test_plugins/test_component_modeler.py` & `tidy3d-2.1.1/tests/test_plugins/test_component_modeler.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/test_plugins/test_dispersion_fitter.py` & `tidy3d-2.1.1/tests/test_plugins/test_dispersion_fitter.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/test_plugins/test_mode_solver.py` & `tidy3d-2.1.1/tests/test_plugins/test_mode_solver.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/test_plugins/test_polyslab.py` & `tidy3d-2.1.1/tests/test_plugins/test_polyslab.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/test_plugins/test_resonance_finder.py` & `tidy3d-2.1.1/tests/test_plugins/test_resonance_finder.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/test_plugins/test_waveguide.py` & `tidy3d-2.1.1/tests/test_plugins/test_waveguide.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/test_web/test_auth.py` & `tidy3d-2.1.1/tests/test_web/test_auth.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/test_web/test_cli.py` & `tidy3d-2.1.1/tests/test_web/test_cli.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/test_web/test_material_fitter.py` & `tidy3d-2.1.1/tests/test_web/test_material_fitter.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/test_web/test_tidy3d_folder.py` & `tidy3d-2.1.1/tests/test_web/test_tidy3d_folder.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/test_web/test_tidy3d_material_library.py` & `tidy3d-2.1.1/tests/test_web/test_tidy3d_material_library.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tests/test_web/test_tidy3d_task.py` & `tidy3d-2.1.1/tests/test_web/test_tidy3d_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
         match=[matchers.query_param_matcher({"projectName": "test folder2"})],
         json={"data": {"projectId": "1234", "projectName": "test folder2"}},
         status=200,
     )
     responses.add(
         responses.POST,
         f"{Env.current.web_api_endpoint}/tidy3d/projects/1234/tasks",
-        match=[matchers.json_params_matcher({"taskName": "test task", "call_back_url": None})],
+        match=[matchers.json_params_matcher({"taskName": "test task", "callbackUrl": None})],
         json={
             "data": {
                 "taskId": "1234",
                 "taskName": "test task",
                 "createdAt": "2022-01-01T00:00:00.000Z",
             }
         },
@@ -163,15 +163,15 @@
         match=[matchers.query_param_matcher({"projectName": "test folder1"})],
         json={"data": {"projectId": "1234", "projectName": "test folder1"}},
         status=200,
     )
     responses.add(
         responses.POST,
         f"{Env.current.web_api_endpoint}/tidy3d/projects/1234/tasks",
-        match=[matchers.json_params_matcher({"taskName": "test task", "call_back_url": None})],
+        match=[matchers.json_params_matcher({"taskName": "test task", "callbackUrl": None})],
         json={
             "data": {
                 "taskId": "1234",
                 "taskName": "test task",
                 "createdAt": "2022-01-01T00:00:00.000Z",
             }
         },
```

### Comparing `tidy3d-2.1.0/tests/test_web/test_webapi.py` & `tidy3d-2.1.1/tests/test_web/test_webapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         json={"data": {"projectId": TASK_ID, "projectName": PROJECT_NAME}},
         status=200,
     )
 
     responses.add(
         responses.POST,
         f"{Env.current.web_api_endpoint}/tidy3d/projects/{TASK_ID}/tasks",
-        match=[matchers.json_params_matcher({"taskName": TASK_NAME, "call_back_url": None})],
+        match=[matchers.json_params_matcher({"taskName": TASK_NAME, "callbackUrl": None})],
         json={
             "data": {
                 "taskId": TASK_ID,
                 "taskName": TASK_NAME,
                 "createdAt": CREATED_AT,
             }
         },
```

### Comparing `tidy3d-2.1.0/tests/utils.py` & `tidy3d-2.1.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/__init__.py` & `tidy3d-2.1.1/tidy3d/__init__.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/__main__.py` & `tidy3d-2.1.1/tidy3d/__main__.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/components/apodization.py` & `tidy3d-2.1.1/tidy3d/components/apodization.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/components/base.py` & `tidy3d-2.1.1/tidy3d/components/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -466,15 +466,15 @@
             Path to a group inside the file to selectively load a sub-element of the model only.
             Starting `/` is optional.
         **parse_obj_kwargs
             Keyword arguments passed to pydantic's ``parse_obj`` method.
 
         Example
         -------
-        >>> simulation.to_hdf5(fname='folder/sim.hdf5') # doctest: +SKIP
+        >>> simulation = Simulation.from_file(fname='folder/sim.hdf5') # doctest: +SKIP
         """
 
         group_path = cls._construct_group_path(group_path)
         model_dict = cls.dict_from_hdf5(fname=fname, group_path=group_path)
         return cls.parse_obj(model_dict, **parse_obj_kwargs)
 
     def to_hdf5(self, fname: str) -> None:
```

### Comparing `tidy3d-2.1.0/tidy3d/components/boundary.py` & `tidy3d-2.1.1/tidy3d/components/boundary.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/components/data/data_array.py` & `tidy3d-2.1.1/tidy3d/components/data/data_array.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/components/data/dataset.py` & `tidy3d-2.1.1/tidy3d/components/data/dataset.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/components/data/monitor_data.py` & `tidy3d-2.1.1/tidy3d/components/data/monitor_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/components/data/sim_data.py` & `tidy3d-2.1.1/tidy3d/components/data/sim_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/components/field_projection.py` & `tidy3d-2.1.1/tidy3d/components/field_projection.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/components/geometry.py` & `tidy3d-2.1.1/tidy3d/components/geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,15 +164,15 @@
         is_inside[inds_inside] = self.inside(*coords_3d)
         return is_inside
 
     @abstractmethod
     def intersections_plane(
         self, x: float = None, y: float = None, z: float = None
     ) -> List[Shapely]:
-        """Returns list of shapely geoemtries at plane specified by one non-None value of x,y,z.
+        """Returns list of shapely geomtries at plane specified by one non-None value of x,y,z.
 
         Parameters
         ----------
         x : float = None
             Position of plane in x direction, only one of x,y,z can be specified to define plane.
         y : float = None
             Position of plane in y direction, only one of x,y,z can be specified to define plane.
@@ -184,15 +184,15 @@
         List[shapely.geometry.base.BaseGeometry]
             List of 2D shapes that intersect plane.
             For more details refer to
             `Shapely's Documentaton <https://shapely.readthedocs.io/en/stable/project.html>`_.
         """
 
     def intersections_2dbox(self, plane: Box) -> List[Shapely]:
-        """Returns list of shapely geoemtries representing the intersections of the geometry with
+        """Returns list of shapely geomtries representing the intersections of the geometry with
         a 2D box.
 
         Returns
         -------
         List[shapely.geometry.base.BaseGeometry]
             List of 2D shapes that intersect plane.
             For more details refer to
@@ -3587,15 +3587,15 @@
         if self.mesh_dataset is None:
             return ((-inf, -inf, -inf), (inf, inf, inf))
         return self.trimesh.bounds
 
     def intersections_plane(
         self, x: float = None, y: float = None, z: float = None
     ) -> List[Shapely]:
-        """Returns list of shapely geoemtries at plane specified by one non-None value of x,y,z.
+        """Returns list of shapely geomtries at plane specified by one non-None value of x,y,z.
 
         Parameters
         ----------
         x : float = None
             Position of plane in x direction, only one of x,y,z can be specified to define plane.
         y : float = None
             Position of plane in y direction, only one of x,y,z can be specified to define plane.
@@ -3758,15 +3758,15 @@
         )
 
         return rmin, rmax
 
     def intersections_plane(
         self, x: float = None, y: float = None, z: float = None
     ) -> List[Shapely]:
-        """Returns list of shapely geoemtries at plane specified by one non-None value of x,y,z.
+        """Returns list of shapely geomtries at plane specified by one non-None value of x,y,z.
 
         Parameters
         ----------
         x : float = None
             Position of plane in x direction, only one of x,y,z can be specified to define plane.
         y : float = None
             Position of plane in y direction, only one of x,y,z can be specified to define plane.
```

### Comparing `tidy3d-2.1.0/tidy3d/components/grid/grid.py` & `tidy3d-2.1.1/tidy3d/components/grid/grid.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/components/grid/grid_spec.py` & `tidy3d-2.1.1/tidy3d/components/grid/grid_spec.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/components/grid/mesher.py` & `tidy3d-2.1.1/tidy3d/components/grid/mesher.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/components/medium.py` & `tidy3d-2.1.1/tidy3d/components/medium.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/components/mode.py` & `tidy3d-2.1.1/tidy3d/components/mode.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/components/monitor.py` & `tidy3d-2.1.1/tidy3d/components/monitor.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/components/simulation.py` & `tidy3d-2.1.1/tidy3d/components/simulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
     )
 
     symmetry: Tuple[Symmetry, Symmetry, Symmetry] = pydantic.Field(
         (0, 0, 0),
         title="Symmetries",
         description="Tuple of integers defining reflection symmetry across a plane "
         "bisecting the simulation domain normal to the x-, y-, and z-axis "
-        "at the simulation center of each axis, respectvely. "
+        "at the simulation center of each axis, respectively. "
         "Each element can be ``0`` (no symmetry), ``1`` (even, i.e. 'PMC' symmetry) or "
         "``-1`` (odd, i.e. 'PEC' symmetry). "
         "Note that the vectorial nature of the fields must be taken into account to correctly "
         "determine the symmetry value.",
     )
 
     structures: Tuple[Structure, ...] = pydantic.Field(
@@ -553,18 +553,18 @@
                 if np.any(freqs < fmin_med) or np.any(freqs > fmax_med):
                     if medium_index == 0:
                         medium_str = "The simulation background medium"
                     else:
                         medium_str = f"The medium associated with structures[{medium_index-1}]"
 
                     log.warning(
-                        f"{medium_str}has a frequency range: ({fmin_med:2e}, {fmax_med:2e}) "
-                        "(Hz)that does not fully cover the frequencies contained in "
+                        f"{medium_str} has a frequency range: ({fmin_med:2e}, {fmax_med:2e}) "
+                        "(Hz) that does not fully cover the frequencies contained in "
                         f"monitors[{monitor_index}]. "
-                        "This can cause innacuracies in the recorded results."
+                        "This can cause inaccuracies in the recorded results."
                     )
 
         return val
 
     @pydantic.validator("monitors", always=True)
     def _warn_monitor_simulation_frequency_range(cls, val, values):
         """Warn if any DFT monitors have frequencies outside of the simulation frequency range."""
@@ -736,15 +736,15 @@
                         log.warning(
                             f"The grid step in {key} has a value of {grid_spec.dl:.4f} (um)"
                             ", which was detected as being large when compared to the "
                             f"central wavelength of sources[{source_index}] "
                             f"within the simulation medium "
                             f"associated with structures[{medium_index + 1}], given by "
                             f"{lambda_min:.4f} (um). "
-                            "To avoid inaccuracies, it is reccomended the grid size is reduced. "
+                            "To avoid inaccuracies, it is recommended the grid size is reduced. "
                             f"Skipping check for structure indexes > {medium_index + 1}."
                         )
                         return val
                         # TODO: warn about custom grid spec
 
         return val
 
@@ -802,17 +802,18 @@
         """Call validators taking z`self` that get run after init."""
         self._validate_no_structures_pml()
         self._validate_tfsf_nonuniform_grid()
 
     def _validate_no_structures_pml(self) -> None:
         """Ensure no structures terminate / have bounds inside of PML."""
 
-        pml_thicks = self.pml_thicknesses
+        pml_thicks = np.array(self.pml_thicknesses).T
         sim_bounds = self.bounds
         bound_spec = self.boundary_spec.to_list
+
         for i, structure in enumerate(self.structures):
             geo_bounds = structure.geometry.bounds
             for sim_bound, geo_bound, pml_thick, bound_dim, pm_val in zip(
                 sim_bounds, geo_bounds, pml_thicks, bound_spec, (-1, 1)
             ):
                 for sim_pos, geo_pos, pml, bound_edge in zip(
                     sim_bound, geo_bound, pml_thick, bound_dim
@@ -860,15 +861,15 @@
 
                 # check if all the grid sizes are sufficiently unequal
                 if not np.all(np.isclose(sizes_in_tfsf, sizes_in_tfsf[0])):
                     log.warning(
                         f"The grid is nonuniform along the '{'xyz'[ind]}' axis, which may lead "
                         "to sub-optimal cancellation of the incident field in the scattered-field "
                         "region for the total-field scattered-field (TFSF) source "
-                        f"'{source.name}'. For best results, we recomended ensuring a uniform "
+                        f"'{source.name}'. For best results, we recommended ensuring a uniform "
                         "grid in both directions tangential to the TFSF injection axis, "
                         f"'{'xyz'[source.injection_axis]}'. "
                     )
 
     """ Pre submit validation (before web.upload()) """
 
     def validate_pre_upload(self) -> None:
```

### Comparing `tidy3d-2.1.0/tidy3d/components/source.py` & `tidy3d-2.1.1/tidy3d/components/source.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/components/structure.py` & `tidy3d-2.1.1/tidy3d/components/structure.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/components/types.py` & `tidy3d-2.1.1/tidy3d/components/types.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/components/validators.py` & `tidy3d-2.1.1/tidy3d/components/validators.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/components/viz.py` & `tidy3d-2.1.1/tidy3d/components/viz.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/config.py` & `tidy3d-2.1.1/tidy3d/config.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/constants.py` & `tidy3d-2.1.1/tidy3d/constants.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/exceptions.py` & `tidy3d-2.1.1/tidy3d/exceptions.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/log.py` & `tidy3d-2.1.1/tidy3d/log.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/material_library/material_library.py` & `tidy3d-2.1.1/tidy3d/material_library/material_library.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/material_library/material_reference.py` & `tidy3d-2.1.1/tidy3d/material_library/material_reference.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/material_library/parametric_materials.py` & `tidy3d-2.1.1/tidy3d/material_library/parametric_materials.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/plugins/adjoint/__init__.py` & `tidy3d-2.1.1/tidy3d/plugins/adjoint/__init__.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/plugins/adjoint/components/base.py` & `tidy3d-2.1.1/tidy3d/plugins/adjoint/components/base.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/plugins/adjoint/components/data/data_array.py` & `tidy3d-2.1.1/tidy3d/plugins/adjoint/components/data/data_array.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/plugins/adjoint/components/data/dataset.py` & `tidy3d-2.1.1/tidy3d/plugins/adjoint/components/data/dataset.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/plugins/adjoint/components/data/monitor_data.py` & `tidy3d-2.1.1/tidy3d/plugins/adjoint/components/data/monitor_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/plugins/adjoint/components/data/sim_data.py` & `tidy3d-2.1.1/tidy3d/plugins/adjoint/components/data/sim_data.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/plugins/adjoint/components/geometry.py` & `tidy3d-2.1.1/tidy3d/plugins/adjoint/components/geometry.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/plugins/adjoint/components/medium.py` & `tidy3d-2.1.1/tidy3d/plugins/adjoint/components/medium.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/plugins/adjoint/components/simulation.py` & `tidy3d-2.1.1/tidy3d/plugins/adjoint/components/simulation.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/plugins/adjoint/components/structure.py` & `tidy3d-2.1.1/tidy3d/plugins/adjoint/components/structure.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/plugins/adjoint/components/types.py` & `tidy3d-2.1.1/tidy3d/plugins/adjoint/components/types.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/plugins/adjoint/web.py` & `tidy3d-2.1.1/tidy3d/plugins/adjoint/web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/plugins/dispersion/fit.py` & `tidy3d-2.1.1/tidy3d/plugins/dispersion/fit.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/plugins/dispersion/fit_web.py` & `tidy3d-2.1.1/tidy3d/plugins/dispersion/fit_web.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/plugins/mode/derivatives.py` & `tidy3d-2.1.1/tidy3d/plugins/mode/derivatives.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/plugins/mode/mode_solver.py` & `tidy3d-2.1.1/tidy3d/plugins/mode/mode_solver.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/plugins/mode/solver.py` & `tidy3d-2.1.1/tidy3d/plugins/mode/solver.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/plugins/mode/transforms.py` & `tidy3d-2.1.1/tidy3d/plugins/mode/transforms.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/plugins/polyslab/polyslab.py` & `tidy3d-2.1.1/tidy3d/plugins/polyslab/polyslab.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/plugins/resonance/resonance.py` & `tidy3d-2.1.1/tidy3d/plugins/resonance/resonance.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/plugins/smatrix/smatrix.py` & `tidy3d-2.1.1/tidy3d/plugins/smatrix/smatrix.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/plugins/waveguide/rectangular_dielectric.py` & `tidy3d-2.1.1/tidy3d/plugins/waveguide/rectangular_dielectric.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/updater.py` & `tidy3d-2.1.1/tidy3d/updater.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/web/asynchronous.py` & `tidy3d-2.1.1/tidy3d/web/asynchronous.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/web/auth.py` & `tidy3d-2.1.1/tidy3d/web/auth.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/web/cacert.pem` & `tidy3d-2.1.1/tidy3d/web/cacert.pem`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/web/cli/app.py` & `tidy3d-2.1.1/tidy3d/web/cli/app.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/web/cli/migrate.py` & `tidy3d-2.1.1/tidy3d/web/cli/migrate.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/web/config.py` & `tidy3d-2.1.1/tidy3d/web/config.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/web/container.py` & `tidy3d-2.1.1/tidy3d/web/container.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/web/environment.py` & `tidy3d-2.1.1/tidy3d/web/environment.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/web/http_management.py` & `tidy3d-2.1.1/tidy3d/web/http_management.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from os.path import expanduser
 from enum import Enum
 
 import requests
 import toml
 
 from .environment import Env
+from ..exceptions import WebError
 from ..version import __version__
 
 SIMCLOUD_APIKEY = "SIMCLOUD_APIKEY"
 
 
 class ResponseCodes(Enum):
     """HTTP response codes to handle individually."""
@@ -70,18 +71,21 @@
     @wraps(func)
     def wrapper(*args, **kwargs):
         """The wrapper function."""
 
         # Extend some capabilities of func
         resp = func(*args, **kwargs)
 
-        if resp.status_code == ResponseCodes.NOT_FOUND.value:
-            return None
-
-        resp.raise_for_status()
+        if resp.status_code != ResponseCodes.OK.value:
+            if resp.status_code == ResponseCodes.NOT_FOUND.value:
+                return None
+            json_resp = resp.json()
+            if "error" in json_resp.keys():
+                raise WebError(json_resp["error"])
+            resp.raise_for_status()
 
         if not resp.text:
             return None
         result = resp.json()
         return result.get("data") if "data" in result else result
 
     return wrapper
```

### Comparing `tidy3d-2.1.0/tidy3d/web/httputils.py` & `tidy3d-2.1.1/tidy3d/web/httputils.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/web/material_fitter.py` & `tidy3d-2.1.1/tidy3d/web/material_fitter.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/web/material_libray.py` & `tidy3d-2.1.1/tidy3d/web/material_libray.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/web/s3utils.py` & `tidy3d-2.1.1/tidy3d/web/s3utils.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/web/simulation_task.py` & `tidy3d-2.1.1/tidy3d/web/simulation_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,29 +167,29 @@
                 "the 'adjoint.run' function to run JaxSimulations."
             )
         return values
 
     # pylint: disable=arguments-differ
     @classmethod
     def create(
-        cls, simulation: Simulation, task_name: str, folder_name="default", call_back_url=None
+        cls, simulation: Simulation, task_name: str, folder_name="default", callback_url=None
     ) -> SimulationTask:
         """Create a new task on the server.
 
         Parameters
         ----------
         simulation: :class".Simulation"
             The :class:`.Simulation` will be uploaded to server in the submitting phase.
             If Simulation is too large to fit into memory, pass None to this parameter
             and use :meth:`.simulationTask.upload_file` instead.
         task_name: str
             The name of the task.
         folder_name: str,
             The name of the folder to store the task. Default is "default".
-        call_back_url: str
+        callback_url: str
             Http PUT url to receive simulation finish event. The body content is a json file with
             fields ``{'id', 'status', 'name', 'workUnit', 'solverVersion'}``.
 
         Returns
         -------
         :class:`SimulationTask`
             :class:`SimulationTask` object containing info about status, size,
@@ -200,15 +200,15 @@
             folder = Folder.get(folder_name)
         if not folder:
             folder = Folder.create(folder_name)
         FOLDER_CACHE[folder_name] = folder
 
         resp = http.post(
             f"tidy3d/projects/{folder.folder_id}/tasks",
-            {"taskName": task_name, "call_back_url": call_back_url},
+            {"taskName": task_name, "callbackUrl": callback_url},
         )
 
         return SimulationTask(**resp, simulation=simulation, folder=folder)
 
     # pylint: disable=arguments-differ
     @classmethod
     def get(cls, task_id: str) -> SimulationTask:
```

### Comparing `tidy3d-2.1.0/tidy3d/web/task.py` & `tidy3d-2.1.1/tidy3d/web/task.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/web/types.py` & `tidy3d-2.1.1/tidy3d/web/types.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d/web/webapi.py` & `tidy3d-2.1.1/tidy3d/web/webapi.py`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d.egg-info/PKG-INFO` & `tidy3d-2.1.1/tidy3d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidy3d
-Version: 2.1.0
+Version: 2.1.1
 Summary: A fast FDTD solver
 Home-page: https://github.com/flexcompute/tidy3d
 Author: Tyler Hughes
 Author-email: tyler@flexcompute.com
 Project-URL: Bug Tracker, https://github.com/flexcompute/tidy3d/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tidy3d-2.1.0/tidy3d.egg-info/SOURCES.txt` & `tidy3d-2.1.1/tidy3d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tidy3d-2.1.0/tidy3d.egg-info/requires.txt` & `tidy3d-2.1.1/tidy3d.egg-info/requires.txt`

 * *Files identical despite different names*

