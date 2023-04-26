# Comparing `tmp/qrisp-0.0.14.tar.gz` & `tmp/qrisp-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qrisp-0.0.14.tar", last modified: Mon Apr 24 16:44:01 2023, max compression
+gzip compressed data, was "qrisp-0.0.15.tar", last modified: Wed Apr 26 12:26:13 2023, max compression
```

## Comparing `qrisp-0.0.14.tar` & `qrisp-0.0.15.tar`

### file list

```diff
@@ -1,164 +1,164 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 16:44:01.151008 qrisp-0.0.14/
--rw-rw-rw-   0        0        0    14474 2023-04-24 14:39:30.000000 qrisp-0.0.14/LICENSE
--rw-rw-rw-   0        0        0      638 2023-04-24 16:44:01.152073 qrisp-0.0.14/PKG-INFO
--rw-rw-rw-   0        0        0       48 2022-05-11 14:39:01.000000 qrisp-0.0.14/README.md
--rw-rw-rw-   0        0        0      108 2023-04-24 15:55:10.000000 qrisp-0.0.14/pyproject.toml
--rw-rw-rw-   0        0        0      582 2023-04-24 16:44:01.154795 qrisp-0.0.14/setup.cfg
--rw-rw-rw-   0        0        0     1668 2023-04-24 16:35:17.000000 qrisp-0.0.14/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 16:44:00.400086 qrisp-0.0.14/src/
-drwxrwxrwx   0        0        0        0 2023-04-24 16:44:00.437885 qrisp-0.0.14/src/qrisp/
--rw-rw-rw-   0        0        0      705 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 16:44:00.491400 qrisp-0.0.14/src/qrisp/arithmetic/
--rw-rw-rw-   0        0        0    32545 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/arithmetic/SBP_arithmetic.py
--rw-rw-rw-   0        0        0      703 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/arithmetic/__init__.py
--rw-rw-rw-   0        0        0     7316 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/arithmetic/comparisons.py
--rw-rw-rw-   0        0        0     5362 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/arithmetic/incrementation.py
--rw-rw-rw-   0        0        0    26506 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/arithmetic/matrix_multiplication.py
--rw-rw-rw-   0        0        0     3293 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/arithmetic/poly_tools.py
--rw-rw-rw-   0        0        0    11029 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/arithmetic/ripple_carry_adder.py
--rw-rw-rw-   0        0        0    16515 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/arithmetic/ripple_division.py
--rw-rw-rw-   0        0        0     1154 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/arithmetic/ripple_mult.py
-drwxrwxrwx   0        0        0        0 2023-04-24 16:44:00.572321 qrisp-0.0.14/src/qrisp/circuit/
--rw-rw-rw-   0        0        0      745 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/circuit/__init__.py
--rw-rw-rw-   0        0        0     1227 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/circuit/clbit.py
--rw-rw-rw-   0        0        0     5927 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/circuit/controlled_operations.py
--rw-rw-rw-   0        0        0     3764 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/circuit/instruction.py
--rw-rw-rw-   0        0        0      504 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/circuit/library.py
--rw-rw-rw-   0        0        0    20068 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/circuit/multi_cx.py
--rw-rw-rw-   0        0        0    28034 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/circuit/operation.py
--rw-rw-rw-   0        0        0    68556 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/circuit/quantum_circuit.py
--rw-rw-rw-   0        0        0     1463 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/circuit/qubit.py
--rw-rw-rw-   0        0        0     5362 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/circuit/standard_operations.py
--rw-rw-rw-   0        0        0     5445 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/circuit/transpiler.py
--rw-rw-rw-   0        0        0     4163 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/circuit/transpiler_old.py
-drwxrwxrwx   0        0        0        0 2023-04-24 16:44:00.612022 qrisp-0.0.14/src/qrisp/core/
--rw-rw-rw-   0        0        0      774 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/core/__init__.py
--rw-rw-rw-   0        0        0    34327 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/core/compilation.py
--rw-rw-rw-   0        0        0    38436 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/core/library.py
--rw-rw-rw-   0        0        0    33412 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/core/quantum_array.py
--rw-rw-rw-   0        0        0     9283 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/core/quantum_dictionary.py
--rw-rw-rw-   0        0        0    41602 2023-04-24 14:38:09.000000 qrisp-0.0.14/src/qrisp/core/quantum_session.py
--rw-rw-rw-   0        0        0    48724 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/core/quantum_variable.py
--rw-rw-rw-   0        0        0    13770 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/core/session_merging_tools.py
--rw-rw-rw-   0        0        0      641 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/default_backend.py
-drwxrwxrwx   0        0        0        0 2023-04-24 16:44:00.645149 qrisp-0.0.14/src/qrisp/environments/
--rw-rw-rw-   0        0        0     6672 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/environments/GMS_environment.py
--rw-rw-rw-   0        0        0      791 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/environments/__init__.py
--rw-rw-rw-   0        0        0    11053 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/environments/control_environment.py
--rw-rw-rw-   0        0        0     5685 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/environments/gate_wrap_environment.py
--rw-rw-rw-   0        0        0    26529 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/environments/quantum_conditionals.py
--rw-rw-rw-   0        0        0    15427 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/environments/quantum_environments.py
--rw-rw-rw-   0        0        0    20105 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/environments/quantum_inversion.py
--rw-rw-rw-   0        0        0     3996 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/environments/temp_var_environment.py
-drwxrwxrwx   0        0        0        0 2023-04-24 16:44:00.653200 qrisp-0.0.14/src/qrisp/grover/
--rw-rw-rw-   0        0        0      451 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/grover/__init__.py
--rw-rw-rw-   0        0        0    12647 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/grover/grover_tools.py
-drwxrwxrwx   0        0        0        0 2023-04-24 16:44:00.666116 qrisp-0.0.14/src/qrisp/interface/
--rw-rw-rw-   0        0        0      672 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/interface/__init__.py
--rw-rw-rw-   0        0        0     8119 2023-04-24 14:42:14.000000 qrisp-0.0.14/src/qrisp/interface/backends.py
--rw-rw-rw-   0        0        0    13257 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/interface/circuit_converter.py
-drwxrwxrwx   0        0        0        0 2023-04-24 16:44:00.681822 qrisp-0.0.14/src/qrisp/interface/openapi_interface/
--rw-rw-rw-   0        0        0      857 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/interface/openapi_interface/__init__.py
--rw-rw-rw-   0        0        0     1528 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/interface/openapi_interface/backend_client.py
--rw-rw-rw-   0        0        0     3921 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/interface/openapi_interface/backend_server.py
--rw-rw-rw-   0        0        0     1099 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/interface/openapi_interface/interface_types.py
-drwxrwxrwx   0        0        0        0 2023-04-24 16:44:00.702680 qrisp-0.0.14/src/qrisp/interface/thrift_interface/
--rw-rw-rw-   0        0        0      624 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/interface/thrift_interface/__init__.py
--rw-rw-rw-   0        0        0     3394 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/interface/thrift_interface/backend_client.py
--rw-rw-rw-   0        0        0     5835 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/interface/thrift_interface/backend_server.py
-drwxrwxrwx   0        0        0        0 2023-04-24 16:44:00.720441 qrisp-0.0.14/src/qrisp/interface/thrift_interface/codegen/
--rw-rw-rw-   0        0        0    15394 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/interface/thrift_interface/codegen/BackendService.py
--rw-rw-rw-   0        0        0      463 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/interface/thrift_interface/codegen/__init__.py
--rw-rw-rw-   0        0        0      790 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/interface/thrift_interface/codegen/constants.py
--rw-rw-rw-   0        0        0    26149 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/interface/thrift_interface/codegen/ttypes.py
--rw-rw-rw-   0        0        0      963 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/interface/thrift_interface/interface_types.py
--rw-rw-rw-   0        0        0     1692 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/interface/thrift_interface/stoppable_thrift_server.py
-drwxrwxrwx   0        0        0        0 2023-04-24 16:44:00.732851 qrisp-0.0.14/src/qrisp/iterators/
--rw-rw-rw-   0        0        0      479 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/iterators/__init__.py
--rw-rw-rw-   0        0        0     3967 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/iterators/qrange.py
-drwxrwxrwx   0        0        0        0 2023-04-24 16:44:00.751437 qrisp-0.0.14/src/qrisp/logic_synthesis/
--rw-rw-rw-   0        0        0      592 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/logic_synthesis/__init__.py
--rw-rw-rw-   0        0        0    19768 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/logic_synthesis/gray_synthesis.py
--rw-rw-rw-   0        0        0     2768 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/logic_synthesis/pprm_synthesis.py
--rw-rw-rw-   0        0        0    15620 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/logic_synthesis/truth_tables.py
-drwxrwxrwx   0        0        0        0 2023-04-24 16:44:00.785070 qrisp-0.0.14/src/qrisp/misc/
--rw-rw-rw-   0        0        0    17646 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/misc/GMS_tools.py
--rw-rw-rw-   0        0        0      488 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/misc/__init__.py
--rw-rw-rw-   0        0        0     4076 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/misc/depth_reduction.py
--rw-rw-rw-   0        0        0    60365 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/misc/utility.py
-drwxrwxrwx   0        0        0        0 2023-04-24 16:44:00.806667 qrisp-0.0.14/src/qrisp/qtypes/
--rw-rw-rw-   0        0        0      607 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/qtypes/__init__.py
--rw-rw-rw-   0        0        0     6385 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/qtypes/quantum_bool.py
--rw-rw-rw-   0        0        0     2239 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/qtypes/quantum_char.py
--rw-rw-rw-   0        0        0    31986 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/qtypes/quantum_float.py
--rw-rw-rw-   0        0        0     4976 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/qtypes/quantum_string.py
-drwxrwxrwx   0        0        0        0 2023-04-24 16:44:00.827009 qrisp-0.0.14/src/qrisp/quantum_network/
--rw-rw-rw-   0        0        0      624 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/quantum_network/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 16:44:00.830020 qrisp-0.0.14/src/qrisp/quantum_network/interface/
--rw-rw-rw-   0        0        0      410 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/quantum_network/interface/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 16:44:00.852466 qrisp-0.0.14/src/qrisp/quantum_network/interface/codegen/
--rw-rw-rw-   0        0        0    52890 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/quantum_network/interface/codegen/QuantumNetworkService.py
--rw-rw-rw-   0        0        0      470 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/quantum_network/interface/codegen/__init__.py
--rw-rw-rw-   0        0        0      790 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/quantum_network/interface/codegen/constants.py
--rw-rw-rw-   0        0        0    21148 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/quantum_network/interface/codegen/ttypes.py
--rw-rw-rw-   0        0        0     1360 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/quantum_network/interface_connection_example.py
--rw-rw-rw-   0        0        0    13558 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/quantum_network/qn_client.py
--rw-rw-rw-   0        0        0     5590 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/quantum_network/qn_server.py
--rw-rw-rw-   0        0        0     5722 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/quantum_network/qn_simulator_server.py
--rw-rw-rw-   0        0        0     6907 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/quantum_network/quantum_network_session.py
-drwxrwxrwx   0        0        0        0 2023-04-24 16:44:00.907316 qrisp-0.0.14/src/qrisp/simulator/
--rw-rw-rw-   0        0        0      786 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/simulator/__init__.py
--rw-rw-rw-   0        0        0     8518 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/simulator/bi_array_helper.py
--rw-rw-rw-   0        0        0    49714 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/simulator/bi_arrays.py
--rw-rw-rw-   0        0        0    49650 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/simulator/bi_arrays_new.py
--rw-rw-rw-   0        0        0    26922 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/simulator/circuit_preprocessing.py
--rw-rw-rw-   0        0        0    13881 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/simulator/circuit_reordering.py
--rw-rw-rw-   0        0        0     7995 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/simulator/impure_quantum_state.py
--rw-rw-rw-   0        0        0      493 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/simulator/numerics_config.py
--rw-rw-rw-   0        0        0     6077 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/simulator/quantum_state.py
--rw-rw-rw-   0        0        0    13850 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/simulator/simulator.py
--rw-rw-rw-   0        0        0     7462 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/simulator/tensor_factor.py
--rw-rw-rw-   0        0        0    11761 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/simulator/unitary_management.py
-drwxrwxrwx   0        0        0        0 2023-04-24 16:44:00.923748 qrisp-0.0.14/src/qrisp/uncomputation/
--rw-rw-rw-   0        0        0      549 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/uncomputation/__init__.py
--rw-rw-rw-   0        0        0     6180 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/uncomputation/type_checker.py
--rw-rw-rw-   0        0        0     4430 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/uncomputation/uncomputation.py
--rw-rw-rw-   0        0        0    11617 2023-04-24 14:36:50.000000 qrisp-0.0.14/src/qrisp/uncomputation/unqomp.py
-drwxrwxrwx   0        0        0        0 2023-04-24 16:44:00.455999 qrisp-0.0.14/src/qrisp.egg-info/
--rw-rw-rw-   0        0        0      638 2023-04-24 16:44:00.000000 qrisp-0.0.14/src/qrisp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5228 2023-04-24 16:44:00.000000 qrisp-0.0.14/src/qrisp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 16:44:00.000000 qrisp-0.0.14/src/qrisp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2023-04-24 16:44:00.000000 qrisp-0.0.14/src/qrisp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-24 16:44:00.000000 qrisp-0.0.14/src/qrisp.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-24 16:44:01.146129 qrisp-0.0.14/tests/
--rw-rw-rw-   0        0        0     1121 2023-04-24 14:36:50.000000 qrisp-0.0.14/tests/test_GMS_environment_example.py
--rw-rw-rw-   0        0        0     1475 2023-04-24 14:36:50.000000 qrisp-0.0.14/tests/test_GXX_converter_example.py
--rw-rw-rw-   0        0        0     2190 2023-04-24 14:36:50.000000 qrisp-0.0.14/tests/test_GXX_gates_example.py
--rw-rw-rw-   0        0        0     3035 2023-04-24 14:36:50.000000 qrisp-0.0.14/tests/test_GZZ_gates_example.py
--rw-rw-rw-   0        0        0     2476 2023-04-24 14:36:50.000000 qrisp-0.0.14/tests/test_abstract_parameters.py
--rw-rw-rw-   0        0        0      940 2023-04-24 14:36:50.000000 qrisp-0.0.14/tests/test_array_entry_manipulation.py
--rw-rw-rw-   0        0        0     4149 2023-04-24 14:36:50.000000 qrisp-0.0.14/tests/test_comparisons.py
--rw-rw-rw-   0        0        0     3442 2023-04-24 14:36:50.000000 qrisp-0.0.14/tests/test_conditional_environments_example.py
--rw-rw-rw-   0        0        0     3037 2023-04-24 14:36:50.000000 qrisp-0.0.14/tests/test_controlled_gates.py
--rw-rw-rw-   0        0        0     4231 2023-04-24 14:36:50.000000 qrisp-0.0.14/tests/test_diagonal_hamiltonian_application.py
--rw-rw-rw-   0        0        0     1603 2023-04-24 14:36:50.000000 qrisp-0.0.14/tests/test_gray_synthesis_example.py
--rw-rw-rw-   0        0        0     3848 2023-04-24 14:36:50.000000 qrisp-0.0.14/tests/test_grovers_algorithm.py
--rw-rw-rw-   0        0        0      675 2023-04-24 14:36:50.000000 qrisp-0.0.14/tests/test_hello_world.py
--rw-rw-rw-   0        0        0     1693 2023-04-24 14:36:50.000000 qrisp-0.0.14/tests/test_inpl_matrix_multiplication_example.py
--rw-rw-rw-   0        0        0     1569 2023-04-24 14:36:50.000000 qrisp-0.0.14/tests/test_interface.py
--rw-rw-rw-   0        0        0      973 2023-04-24 14:36:50.000000 qrisp-0.0.14/tests/test_loops.py
--rw-rw-rw-   0        0        0     2058 2023-04-24 14:36:50.000000 qrisp-0.0.14/tests/test_matrix_multiplication_example.py
--rw-rw-rw-   0        0        0     2420 2023-04-24 14:36:50.000000 qrisp-0.0.14/tests/test_mcx.py
--rw-rw-rw-   0        0        0      670 2023-04-24 14:36:50.000000 qrisp-0.0.14/tests/test_measurement_reduction.py
--rw-rw-rw-   0        0        0      663 2023-04-24 14:36:50.000000 qrisp-0.0.14/tests/test_outcome_array.py
--rw-rw-rw-   0        0        0     1894 2023-04-24 14:36:50.000000 qrisp-0.0.14/tests/test_qiskit_backend_client.py
--rw-rw-rw-   0        0        0      806 2023-04-24 14:36:50.000000 qrisp-0.0.14/tests/test_qompiler.py
--rw-rw-rw-   0        0        0     3087 2023-04-24 14:36:50.000000 qrisp-0.0.14/tests/test_quantum_arithmetic.py
--rw-rw-rw-   0        0        0     2912 2023-04-24 14:36:50.000000 qrisp-0.0.14/tests/test_quantum_dictionary.py
--rw-rw-rw-   0        0        0     1047 2023-04-24 14:36:50.000000 qrisp-0.0.14/tests/test_quantum_division.py
--rw-rw-rw-   0        0        0     4896 2023-04-24 14:36:50.000000 qrisp-0.0.14/tests/test_quantum_teleportation.py
--rw-rw-rw-   0        0        0     1236 2023-04-24 14:36:50.000000 qrisp-0.0.14/tests/test_state_preparation.py
--rw-rw-rw-   0        0        0      958 2023-04-24 14:36:50.000000 qrisp-0.0.14/tests/test_string_test.py
--rw-rw-rw-   0        0        0     5218 2023-04-24 14:36:50.000000 qrisp-0.0.14/tests/test_uncomputation_example.py
--rw-rw-rw-   0        0        0     1600 2023-04-24 14:36:50.000000 qrisp-0.0.14/tests/test_unitary_calculation.py
--rw-rw-rw-   0        0        0     4023 2023-04-24 14:36:50.000000 qrisp-0.0.14/tests/tests_doc_examples.py
+drwxrwxrwx   0        0        0        0 2023-04-26 12:26:13.577317 qrisp-0.0.15/
+-rw-rw-rw-   0        0        0    14474 2023-04-24 14:39:30.000000 qrisp-0.0.15/LICENSE
+-rw-rw-rw-   0        0        0      638 2023-04-26 12:26:13.577317 qrisp-0.0.15/PKG-INFO
+-rw-rw-rw-   0        0        0       48 2022-05-11 14:39:01.000000 qrisp-0.0.15/README.md
+-rw-rw-rw-   0        0        0      108 2023-04-24 15:55:10.000000 qrisp-0.0.15/pyproject.toml
+-rw-rw-rw-   0        0        0      588 2023-04-26 12:26:13.580676 qrisp-0.0.15/setup.cfg
+-rw-rw-rw-   0        0        0     1668 2023-04-24 16:35:17.000000 qrisp-0.0.15/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 12:26:13.022115 qrisp-0.0.15/src/
+drwxrwxrwx   0        0        0        0 2023-04-26 12:26:13.058523 qrisp-0.0.15/src/qrisp/
+-rw-rw-rw-   0        0        0      705 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 12:26:13.106862 qrisp-0.0.15/src/qrisp/arithmetic/
+-rw-rw-rw-   0        0        0    33345 2023-04-25 09:24:44.000000 qrisp-0.0.15/src/qrisp/arithmetic/SBP_arithmetic.py
+-rw-rw-rw-   0        0        0      703 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/arithmetic/__init__.py
+-rw-rw-rw-   0        0        0     7316 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/arithmetic/comparisons.py
+-rw-rw-rw-   0        0        0     5374 2023-04-24 21:55:24.000000 qrisp-0.0.15/src/qrisp/arithmetic/incrementation.py
+-rw-rw-rw-   0        0        0    26518 2023-04-24 21:55:26.000000 qrisp-0.0.15/src/qrisp/arithmetic/matrix_multiplication.py
+-rw-rw-rw-   0        0        0     3293 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/arithmetic/poly_tools.py
+-rw-rw-rw-   0        0        0    11041 2023-04-24 21:55:24.000000 qrisp-0.0.15/src/qrisp/arithmetic/ripple_carry_adder.py
+-rw-rw-rw-   0        0        0    16527 2023-04-24 21:55:00.000000 qrisp-0.0.15/src/qrisp/arithmetic/ripple_division.py
+-rw-rw-rw-   0        0        0     1166 2023-04-24 21:55:25.000000 qrisp-0.0.15/src/qrisp/arithmetic/ripple_mult.py
+drwxrwxrwx   0        0        0        0 2023-04-26 12:26:13.148966 qrisp-0.0.15/src/qrisp/circuit/
+-rw-rw-rw-   0        0        0      745 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/circuit/__init__.py
+-rw-rw-rw-   0        0        0     1239 2023-04-24 21:55:26.000000 qrisp-0.0.15/src/qrisp/circuit/clbit.py
+-rw-rw-rw-   0        0        0     5939 2023-04-24 21:55:25.000000 qrisp-0.0.15/src/qrisp/circuit/controlled_operations.py
+-rw-rw-rw-   0        0        0     3776 2023-04-24 21:55:28.000000 qrisp-0.0.15/src/qrisp/circuit/instruction.py
+-rw-rw-rw-   0        0        0      504 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/circuit/library.py
+-rw-rw-rw-   0        0        0    20068 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/circuit/multi_cx.py
+-rw-rw-rw-   0        0        0    28263 2023-04-25 11:57:49.000000 qrisp-0.0.15/src/qrisp/circuit/operation.py
+-rw-rw-rw-   0        0        0    68568 2023-04-25 12:05:38.000000 qrisp-0.0.15/src/qrisp/circuit/quantum_circuit.py
+-rw-rw-rw-   0        0        0     1532 2023-04-25 09:12:59.000000 qrisp-0.0.15/src/qrisp/circuit/qubit.py
+-rw-rw-rw-   0        0        0     5374 2023-04-24 21:55:25.000000 qrisp-0.0.15/src/qrisp/circuit/standard_operations.py
+-rw-rw-rw-   0        0        0     5457 2023-04-24 21:55:11.000000 qrisp-0.0.15/src/qrisp/circuit/transpiler.py
+-rw-rw-rw-   0        0        0     4163 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/circuit/transpiler_old.py
+drwxrwxrwx   0        0        0        0 2023-04-26 12:26:13.184730 qrisp-0.0.15/src/qrisp/core/
+-rw-rw-rw-   0        0        0      774 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/core/__init__.py
+-rw-rw-rw-   0        0        0    34329 2023-04-25 12:10:42.000000 qrisp-0.0.15/src/qrisp/core/compilation.py
+-rw-rw-rw-   0        0        0    38448 2023-04-24 21:55:23.000000 qrisp-0.0.15/src/qrisp/core/library.py
+-rw-rw-rw-   0        0        0    33439 2023-04-26 12:08:04.000000 qrisp-0.0.15/src/qrisp/core/quantum_array.py
+-rw-rw-rw-   0        0        0     9295 2023-04-24 21:55:25.000000 qrisp-0.0.15/src/qrisp/core/quantum_dictionary.py
+-rw-rw-rw-   0        0        0    41602 2023-04-24 14:38:09.000000 qrisp-0.0.15/src/qrisp/core/quantum_session.py
+-rw-rw-rw-   0        0        0    48739 2023-04-25 09:14:41.000000 qrisp-0.0.15/src/qrisp/core/quantum_variable.py
+-rw-rw-rw-   0        0        0    13782 2023-04-24 21:55:23.000000 qrisp-0.0.15/src/qrisp/core/session_merging_tools.py
+-rw-rw-rw-   0        0        0      641 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/default_backend.py
+drwxrwxrwx   0        0        0        0 2023-04-26 12:26:13.215287 qrisp-0.0.15/src/qrisp/environments/
+-rw-rw-rw-   0        0        0     6672 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/environments/GMS_environment.py
+-rw-rw-rw-   0        0        0      791 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/environments/__init__.py
+-rw-rw-rw-   0        0        0    11065 2023-04-24 21:55:22.000000 qrisp-0.0.15/src/qrisp/environments/control_environment.py
+-rw-rw-rw-   0        0        0     5697 2023-04-24 21:54:35.000000 qrisp-0.0.15/src/qrisp/environments/gate_wrap_environment.py
+-rw-rw-rw-   0        0        0    26541 2023-04-24 21:55:22.000000 qrisp-0.0.15/src/qrisp/environments/quantum_conditionals.py
+-rw-rw-rw-   0        0        0    15439 2023-04-24 21:54:42.000000 qrisp-0.0.15/src/qrisp/environments/quantum_environments.py
+-rw-rw-rw-   0        0        0    20117 2023-04-24 21:55:26.000000 qrisp-0.0.15/src/qrisp/environments/quantum_inversion.py
+-rw-rw-rw-   0        0        0     4008 2023-04-24 21:55:24.000000 qrisp-0.0.15/src/qrisp/environments/temp_var_environment.py
+drwxrwxrwx   0        0        0        0 2023-04-26 12:26:13.223271 qrisp-0.0.15/src/qrisp/grover/
+-rw-rw-rw-   0        0        0      451 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/grover/__init__.py
+-rw-rw-rw-   0        0        0    12659 2023-04-24 21:55:23.000000 qrisp-0.0.15/src/qrisp/grover/grover_tools.py
+drwxrwxrwx   0        0        0        0 2023-04-26 12:26:13.232409 qrisp-0.0.15/src/qrisp/interface/
+-rw-rw-rw-   0        0        0      672 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/interface/__init__.py
+-rw-rw-rw-   0        0        0     8119 2023-04-24 14:42:14.000000 qrisp-0.0.15/src/qrisp/interface/backends.py
+-rw-rw-rw-   0        0        0    13273 2023-04-25 11:46:06.000000 qrisp-0.0.15/src/qrisp/interface/circuit_converter.py
+drwxrwxrwx   0        0        0        0 2023-04-26 12:26:13.246842 qrisp-0.0.15/src/qrisp/interface/openapi_interface/
+-rw-rw-rw-   0        0        0      857 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/interface/openapi_interface/__init__.py
+-rw-rw-rw-   0        0        0     1528 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/interface/openapi_interface/backend_client.py
+-rw-rw-rw-   0        0        0     3921 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/interface/openapi_interface/backend_server.py
+-rw-rw-rw-   0        0        0     1099 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/interface/openapi_interface/interface_types.py
+drwxrwxrwx   0        0        0        0 2023-04-26 12:26:13.263807 qrisp-0.0.15/src/qrisp/interface/thrift_interface/
+-rw-rw-rw-   0        0        0      624 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/interface/thrift_interface/__init__.py
+-rw-rw-rw-   0        0        0     3406 2023-04-24 21:54:39.000000 qrisp-0.0.15/src/qrisp/interface/thrift_interface/backend_client.py
+-rw-rw-rw-   0        0        0     5847 2023-04-24 21:55:24.000000 qrisp-0.0.15/src/qrisp/interface/thrift_interface/backend_server.py
+drwxrwxrwx   0        0        0        0 2023-04-26 12:26:13.279033 qrisp-0.0.15/src/qrisp/interface/thrift_interface/codegen/
+-rw-rw-rw-   0        0        0    15406 2023-04-24 21:55:28.000000 qrisp-0.0.15/src/qrisp/interface/thrift_interface/codegen/BackendService.py
+-rw-rw-rw-   0        0        0      463 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/interface/thrift_interface/codegen/__init__.py
+-rw-rw-rw-   0        0        0      790 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/interface/thrift_interface/codegen/constants.py
+-rw-rw-rw-   0        0        0    26161 2023-04-24 21:55:24.000000 qrisp-0.0.15/src/qrisp/interface/thrift_interface/codegen/ttypes.py
+-rw-rw-rw-   0        0        0      975 2023-04-24 21:55:24.000000 qrisp-0.0.15/src/qrisp/interface/thrift_interface/interface_types.py
+-rw-rw-rw-   0        0        0     1692 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/interface/thrift_interface/stoppable_thrift_server.py
+drwxrwxrwx   0        0        0        0 2023-04-26 12:26:13.286498 qrisp-0.0.15/src/qrisp/iterators/
+-rw-rw-rw-   0        0        0      479 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/iterators/__init__.py
+-rw-rw-rw-   0        0        0     3967 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/iterators/qrange.py
+drwxrwxrwx   0        0        0        0 2023-04-26 12:26:13.302563 qrisp-0.0.15/src/qrisp/logic_synthesis/
+-rw-rw-rw-   0        0        0      592 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/logic_synthesis/__init__.py
+-rw-rw-rw-   0        0        0    19780 2023-04-24 21:55:25.000000 qrisp-0.0.15/src/qrisp/logic_synthesis/gray_synthesis.py
+-rw-rw-rw-   0        0        0     2768 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/logic_synthesis/pprm_synthesis.py
+-rw-rw-rw-   0        0        0    15620 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/logic_synthesis/truth_tables.py
+drwxrwxrwx   0        0        0        0 2023-04-26 12:26:13.317921 qrisp-0.0.15/src/qrisp/misc/
+-rw-rw-rw-   0        0        0    17658 2023-04-24 21:55:27.000000 qrisp-0.0.15/src/qrisp/misc/GMS_tools.py
+-rw-rw-rw-   0        0        0      488 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/misc/__init__.py
+-rw-rw-rw-   0        0        0     4076 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/misc/depth_reduction.py
+-rw-rw-rw-   0        0        0    60377 2023-04-24 21:55:24.000000 qrisp-0.0.15/src/qrisp/misc/utility.py
+drwxrwxrwx   0        0        0        0 2023-04-26 12:26:13.340210 qrisp-0.0.15/src/qrisp/qtypes/
+-rw-rw-rw-   0        0        0      607 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/qtypes/__init__.py
+-rw-rw-rw-   0        0        0     6397 2023-04-24 21:55:22.000000 qrisp-0.0.15/src/qrisp/qtypes/quantum_bool.py
+-rw-rw-rw-   0        0        0     2239 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/qtypes/quantum_char.py
+-rw-rw-rw-   0        0        0    28131 2023-04-25 09:38:48.000000 qrisp-0.0.15/src/qrisp/qtypes/quantum_float.py
+-rw-rw-rw-   0        0        0     4976 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/qtypes/quantum_string.py
+drwxrwxrwx   0        0        0        0 2023-04-26 12:26:13.361545 qrisp-0.0.15/src/qrisp/quantum_network/
+-rw-rw-rw-   0        0        0      624 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/quantum_network/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 12:26:13.364508 qrisp-0.0.15/src/qrisp/quantum_network/interface/
+-rw-rw-rw-   0        0        0      410 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/quantum_network/interface/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 12:26:13.383691 qrisp-0.0.15/src/qrisp/quantum_network/interface/codegen/
+-rw-rw-rw-   0        0        0    52890 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/quantum_network/interface/codegen/QuantumNetworkService.py
+-rw-rw-rw-   0        0        0      470 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/quantum_network/interface/codegen/__init__.py
+-rw-rw-rw-   0        0        0      790 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/quantum_network/interface/codegen/constants.py
+-rw-rw-rw-   0        0        0    21148 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/quantum_network/interface/codegen/ttypes.py
+-rw-rw-rw-   0        0        0     1360 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/quantum_network/interface_connection_example.py
+-rw-rw-rw-   0        0        0    13570 2023-04-24 21:54:51.000000 qrisp-0.0.15/src/qrisp/quantum_network/qn_client.py
+-rw-rw-rw-   0        0        0     5602 2023-04-24 21:54:54.000000 qrisp-0.0.15/src/qrisp/quantum_network/qn_server.py
+-rw-rw-rw-   0        0        0     5722 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/quantum_network/qn_simulator_server.py
+-rw-rw-rw-   0        0        0     6919 2023-04-24 21:54:48.000000 qrisp-0.0.15/src/qrisp/quantum_network/quantum_network_session.py
+drwxrwxrwx   0        0        0        0 2023-04-26 12:26:13.435127 qrisp-0.0.15/src/qrisp/simulator/
+-rw-rw-rw-   0        0        0      786 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/simulator/__init__.py
+-rw-rw-rw-   0        0        0     8518 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/simulator/bi_array_helper.py
+-rw-rw-rw-   0        0        0    49714 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/simulator/bi_arrays.py
+-rw-rw-rw-   0        0        0    49650 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/simulator/bi_arrays_new.py
+-rw-rw-rw-   0        0        0    26922 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/simulator/circuit_preprocessing.py
+-rw-rw-rw-   0        0        0    13881 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/simulator/circuit_reordering.py
+-rw-rw-rw-   0        0        0     7995 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/simulator/impure_quantum_state.py
+-rw-rw-rw-   0        0        0      493 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/simulator/numerics_config.py
+-rw-rw-rw-   0        0        0     6077 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/simulator/quantum_state.py
+-rw-rw-rw-   0        0        0    13911 2023-04-25 09:18:14.000000 qrisp-0.0.15/src/qrisp/simulator/simulator.py
+-rw-rw-rw-   0        0        0     7462 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/simulator/tensor_factor.py
+-rw-rw-rw-   0        0        0    11761 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/simulator/unitary_management.py
+drwxrwxrwx   0        0        0        0 2023-04-26 12:26:13.452091 qrisp-0.0.15/src/qrisp/uncomputation/
+-rw-rw-rw-   0        0        0      549 2023-04-24 14:36:50.000000 qrisp-0.0.15/src/qrisp/uncomputation/__init__.py
+-rw-rw-rw-   0        0        0     6192 2023-04-24 21:55:25.000000 qrisp-0.0.15/src/qrisp/uncomputation/type_checker.py
+-rw-rw-rw-   0        0        0     4442 2023-04-24 21:55:24.000000 qrisp-0.0.15/src/qrisp/uncomputation/uncomputation.py
+-rw-rw-rw-   0        0        0    11629 2023-04-24 21:55:25.000000 qrisp-0.0.15/src/qrisp/uncomputation/unqomp.py
+drwxrwxrwx   0        0        0        0 2023-04-26 12:26:13.074266 qrisp-0.0.15/src/qrisp.egg-info/
+-rw-rw-rw-   0        0        0      638 2023-04-26 12:26:12.000000 qrisp-0.0.15/src/qrisp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5228 2023-04-26 12:26:13.000000 qrisp-0.0.15/src/qrisp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 12:26:12.000000 qrisp-0.0.15/src/qrisp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      116 2023-04-26 12:26:12.000000 qrisp-0.0.15/src/qrisp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-26 12:26:12.000000 qrisp-0.0.15/src/qrisp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 12:26:13.573076 qrisp-0.0.15/tests/
+-rw-rw-rw-   0        0        0     1121 2023-04-24 14:36:50.000000 qrisp-0.0.15/tests/test_GMS_environment_example.py
+-rw-rw-rw-   0        0        0     1475 2023-04-24 14:36:50.000000 qrisp-0.0.15/tests/test_GXX_converter_example.py
+-rw-rw-rw-   0        0        0     2202 2023-04-24 21:55:27.000000 qrisp-0.0.15/tests/test_GXX_gates_example.py
+-rw-rw-rw-   0        0        0     3047 2023-04-24 21:55:27.000000 qrisp-0.0.15/tests/test_GZZ_gates_example.py
+-rw-rw-rw-   0        0        0     2476 2023-04-24 14:36:50.000000 qrisp-0.0.15/tests/test_abstract_parameters.py
+-rw-rw-rw-   0        0        0      940 2023-04-24 14:36:50.000000 qrisp-0.0.15/tests/test_array_entry_manipulation.py
+-rw-rw-rw-   0        0        0     4149 2023-04-24 14:36:50.000000 qrisp-0.0.15/tests/test_comparisons.py
+-rw-rw-rw-   0        0        0     3442 2023-04-24 14:36:50.000000 qrisp-0.0.15/tests/test_conditional_environments_example.py
+-rw-rw-rw-   0        0        0     3037 2023-04-24 14:36:50.000000 qrisp-0.0.15/tests/test_controlled_gates.py
+-rw-rw-rw-   0        0        0     4231 2023-04-24 14:36:50.000000 qrisp-0.0.15/tests/test_diagonal_hamiltonian_application.py
+-rw-rw-rw-   0        0        0     1603 2023-04-24 14:36:50.000000 qrisp-0.0.15/tests/test_gray_synthesis_example.py
+-rw-rw-rw-   0        0        0     3848 2023-04-24 14:36:50.000000 qrisp-0.0.15/tests/test_grovers_algorithm.py
+-rw-rw-rw-   0        0        0      675 2023-04-24 14:36:50.000000 qrisp-0.0.15/tests/test_hello_world.py
+-rw-rw-rw-   0        0        0     1693 2023-04-24 14:36:50.000000 qrisp-0.0.15/tests/test_inpl_matrix_multiplication_example.py
+-rw-rw-rw-   0        0        0     1569 2023-04-24 14:36:50.000000 qrisp-0.0.15/tests/test_interface.py
+-rw-rw-rw-   0        0        0      973 2023-04-24 14:36:50.000000 qrisp-0.0.15/tests/test_loops.py
+-rw-rw-rw-   0        0        0     2058 2023-04-24 14:36:50.000000 qrisp-0.0.15/tests/test_matrix_multiplication_example.py
+-rw-rw-rw-   0        0        0     2432 2023-04-24 21:55:26.000000 qrisp-0.0.15/tests/test_mcx.py
+-rw-rw-rw-   0        0        0      682 2023-04-24 21:55:27.000000 qrisp-0.0.15/tests/test_measurement_reduction.py
+-rw-rw-rw-   0        0        0      663 2023-04-24 14:36:50.000000 qrisp-0.0.15/tests/test_outcome_array.py
+-rw-rw-rw-   0        0        0     1894 2023-04-24 14:36:50.000000 qrisp-0.0.15/tests/test_qiskit_backend_client.py
+-rw-rw-rw-   0        0        0      806 2023-04-24 14:36:50.000000 qrisp-0.0.15/tests/test_qompiler.py
+-rw-rw-rw-   0        0        0     3099 2023-04-24 21:55:05.000000 qrisp-0.0.15/tests/test_quantum_arithmetic.py
+-rw-rw-rw-   0        0        0     2912 2023-04-24 14:36:50.000000 qrisp-0.0.15/tests/test_quantum_dictionary.py
+-rw-rw-rw-   0        0        0     1047 2023-04-24 14:36:50.000000 qrisp-0.0.15/tests/test_quantum_division.py
+-rw-rw-rw-   0        0        0     4896 2023-04-24 14:36:50.000000 qrisp-0.0.15/tests/test_quantum_teleportation.py
+-rw-rw-rw-   0        0        0     1236 2023-04-24 14:36:50.000000 qrisp-0.0.15/tests/test_state_preparation.py
+-rw-rw-rw-   0        0        0      958 2023-04-24 14:36:50.000000 qrisp-0.0.15/tests/test_string_test.py
+-rw-rw-rw-   0        0        0     5218 2023-04-24 14:36:50.000000 qrisp-0.0.15/tests/test_uncomputation_example.py
+-rw-rw-rw-   0        0        0     1600 2023-04-24 14:36:50.000000 qrisp-0.0.15/tests/test_unitary_calculation.py
+-rw-rw-rw-   0        0        0     4023 2023-04-24 14:36:50.000000 qrisp-0.0.15/tests/tests_doc_examples.py
```

### Comparing `qrisp-0.0.14/LICENSE` & `qrisp-0.0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/PKG-INFO` & `qrisp-0.0.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qrisp
-Version: 0.0.14
+Version: 0.0.15
 Summary: Qrisp - A high level language for gate-based quantum computing
 Home-page: https://github.com/pypa/sampleproject
 Author: Raphael Seidel
 Author-email: raphael.seidel@fokus.fraunhofer.de
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)
```

### Comparing `qrisp-0.0.14/setup.cfg` & `qrisp-0.0.15/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2071 7269 7370 0d0a 7665 7273 696f   = qrisp..versio
-00000020: 6e20 3d20 302e 302e 3134 0d0a 6175 7468  n = 0.0.14..auth
+00000020: 6e20 3d20 302e 302e 3135 0d0a 6175 7468  n = 0.0.15..auth
 00000030: 6f72 203d 2052 6170 6861 656c 2053 6569  or = Raphael Sei
 00000040: 6465 6c0d 0a61 7574 686f 725f 656d 6169  del..author_emai
 00000050: 6c20 3d20 7261 7068 6165 6c2e 7365 6964  l = raphael.seid
 00000060: 656c 4066 6f6b 7573 2e66 7261 756e 686f  el@fokus.fraunho
 00000070: 6665 722e 6465 0d0a 6465 7363 7269 7074  fer.de..descript
 00000080: 696f 6e20 3d20 4120 736d 616c 6c20 6578  ion = A small ex
 00000090: 616d 706c 6520 7061 636b 6167 650d 0a6c  ample package..l
 000000a0: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
 000000b0: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
 000000c0: 640d 0a6c 6f6e 675f 6465 7363 7269 7074  d..long_descript
 000000d0: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
 000000e0: 203d 2074 6578 742f 6d61 726b 646f 776e   = text/markdown
 000000f0: 0d0a 7572 6c20 3d20 6874 7470 733a 2f2f  ..url = https://
-00000100: 6769 7468 7562 2e63 6f6d 2f70 7970 612f  github.com/pypa/
-00000110: 7361 6d70 6c65 7072 6f6a 6563 740d 0a70  sampleproject..p
-00000120: 726f 6a65 6374 5f75 726c 7320 3d20 0d0a  roject_urls = ..
-00000130: 0942 7567 2054 7261 636b 6572 203d 2068  .Bug Tracker = h
-00000140: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000150: 6d2f 7079 7061 2f73 616d 706c 6570 726f  m/pypa/samplepro
-00000160: 6a65 6374 2f69 7373 7565 730d 0a0d 0a5b  ject/issues....[
-00000170: 6f70 7469 6f6e 735d 0d0a 7061 636b 6167  options]..packag
-00000180: 655f 6469 7220 3d20 0d0a 093d 7372 630d  e_dir = ...=src.
-00000190: 0a70 6163 6b61 6765 7320 3d20 6669 6e64  .packages = find
-000001a0: 3a0d 0a70 7974 686f 6e5f 7265 7175 6972  :..python_requir
-000001b0: 6573 203d 203e 3d33 2e38 0d0a 0d0a 5b6f  es = >=3.8....[o
-000001c0: 7074 696f 6e73 2e70 6163 6b61 6765 732e  ptions.packages.
-000001d0: 6669 6e64 5d0d 0a77 6865 7265 203d 2073  find]..where = s
-000001e0: 7263 0d0a 0d0a 5b74 6f6f 6c3a 7079 7465  rc....[tool:pyte
-000001f0: 7374 5d0d 0a74 6573 7470 6174 6873 203d  st]..testpaths =
-00000200: 202e 2f74 6573 7473 0d0a 7079 7468 6f6e   ./tests..python
-00000210: 7061 7468 203d 202e 0d0a 0d0a 5b65 6767  path = .....[egg
-00000220: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
-00000230: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
-00000240: 2030 0d0a 0d0a                            0....
+00000100: 6769 7468 7562 2e63 6f6d 2f66 7261 756e  github.com/fraun
+00000110: 686f 6665 7266 6f6b 7573 2f51 7269 7370  hoferfokus/Qrisp
+00000120: 0d0a 7072 6f6a 6563 745f 7572 6c73 203d  ..project_urls =
+00000130: 200d 0a09 4275 6720 5472 6163 6b65 7220   ...Bug Tracker 
+00000140: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
+00000150: 2e63 6f6d 2f66 7261 756e 686f 6665 7266  .com/fraunhoferf
+00000160: 6f6b 7573 2f51 7269 7370 2f69 7373 7565  okus/Qrisp/issue
+00000170: 730d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  s....[options]..
+00000180: 7061 636b 6167 655f 6469 7220 3d20 0d0a  package_dir = ..
+00000190: 093d 7372 630d 0a70 6163 6b61 6765 7320  .=src..packages 
+000001a0: 3d20 6669 6e64 3a0d 0a70 7974 686f 6e5f  = find:..python_
+000001b0: 7265 7175 6972 6573 203d 203e 3d33 2e38  requires = >=3.8
+000001c0: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
+000001d0: 6b61 6765 732e 6669 6e64 5d0d 0a77 6865  kages.find]..whe
+000001e0: 7265 203d 2073 7263 0d0a 0d0a 5b74 6f6f  re = src....[too
+000001f0: 6c3a 7079 7465 7374 5d0d 0a74 6573 7470  l:pytest]..testp
+00000200: 6174 6873 203d 202e 2f74 6573 7473 0d0a  aths = ./tests..
+00000210: 7079 7468 6f6e 7061 7468 203d 202e 0d0a  pythonpath = ...
+00000220: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
+00000230: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
+00000240: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
```

### Comparing `qrisp-0.0.14/setup.py` & `qrisp-0.0.15/setup.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/__init__.py` & `qrisp-0.0.15/src/qrisp/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/arithmetic/SBP_arithmetic.py` & `qrisp-0.0.15/src/qrisp/arithmetic/SBP_arithmetic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 
 import sympy as sp
 import numpy as np
 from qrisp.core import QuantumVariable, QuantumArray
 from qrisp.misc import gate_wrap
 from qrisp.arithmetic.poly_tools import (
     get_ordered_symbol_list,
@@ -856,14 +856,38 @@
     # Perform exponent shifts
 
     x.exp_shift(x_exp)
     y.exp_shift(y_exp)
 
     return output_qf
 
+#Wrapper for choosing the best multiplication algorithm
+def q_mult(factor_1, factor_2, target = None, method = "auto"):
+    
+    if method == "auto":
+        
+        if factor_1.reg == factor_2.reg:
+            return q_mult(factor_1, factor_2, target, method = "sbp")
+        else:
+            return q_mult(factor_1, factor_2, target, method = "hybrid")
+
+    elif method == "sbp":
+        
+        from qrisp.qtypes.quantum_float import create_output_qf
+        if target is None:
+            target = create_output_qf([factor_1, factor_2], op = "mul")
+        
+        sbp_mult(factor_1, factor_2, target)
+        return target
+    
+    elif method == "hybrid":
+        from qrisp.arithmetic import hybrid_mult
+        return hybrid_mult(factor_1, factor_2)
+
+
 
 def QFT_inpl_mult(qv, inplace_mult = 1):
     
     from qrisp.misc import is_inv
     
     
     qv = list(qv)
```

### Comparing `qrisp-0.0.14/src/qrisp/arithmetic/__init__.py` & `qrisp-0.0.15/src/qrisp/arithmetic/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/arithmetic/comparisons.py` & `qrisp-0.0.15/src/qrisp/arithmetic/comparisons.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/arithmetic/incrementation.py` & `qrisp-0.0.15/src/qrisp/arithmetic/incrementation.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 
 from qrisp.misc import gate_wrap
 from qrisp import x, QuantumVariable
 
 
 @gate_wrap(is_qfree=True)
 def increment(qf, amount):
```

### Comparing `qrisp-0.0.14/src/qrisp/arithmetic/matrix_multiplication.py` & `qrisp-0.0.15/src/qrisp/arithmetic/matrix_multiplication.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 
 
 import sympy as sp
 
 from qrisp.arithmetic.SBP_arithmetic import hybrid_mult, polynomial_encoder
 from qrisp import QuantumArray, p, z
 from qrisp.qtypes import QuantumFloat
```

### Comparing `qrisp-0.0.14/src/qrisp/arithmetic/poly_tools.py` & `qrisp-0.0.15/src/qrisp/arithmetic/poly_tools.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/arithmetic/ripple_carry_adder.py` & `qrisp-0.0.15/src/qrisp/arithmetic/ripple_carry_adder.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 
 import numpy as np
 
 # Implementation of the modular Cuccaro-Adder https://arxiv.org/pdf/quant-ph/0410184.pdf
 # Has complexity O(log(N)) (Fourier-Adding has O(log(N)^2))
 
 from qrisp import QuantumCircuit
```

### Comparing `qrisp-0.0.14/src/qrisp/arithmetic/ripple_division.py` & `qrisp-0.0.15/src/qrisp/arithmetic/ripple_division.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 from qrisp import x, gate_wrap
 
 
 @gate_wrap(is_qfree=True, permeability="args")
 def q_int_div(numerator, divisor, adder="cuccaro", n=None, log_output=True):
     # This function performs integer division based on the following algorithm
     # Which is a reformulation of the division algorithm presented in
```

### Comparing `qrisp-0.0.14/src/qrisp/arithmetic/ripple_mult.py` & `qrisp-0.0.15/src/qrisp/arithmetic/ripple_mult.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 
 from qrisp import x, cx
 from qrisp.arithmetic import inpl_add
 from qrisp.arithmetic import create_output_qf
 
 
 def ripple_mult(factor_1, factor_2):
```

### Comparing `qrisp-0.0.14/src/qrisp/circuit/__init__.py` & `qrisp-0.0.15/src/qrisp/circuit/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/circuit/clbit.py` & `qrisp-0.0.15/src/qrisp/circuit/clbit.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 
 
 class Clbit:
     """
     This class represents classical bits. Classical bits are created by supplying the
     identifier string.
```

### Comparing `qrisp-0.0.14/src/qrisp/circuit/controlled_operations.py` & `qrisp-0.0.15/src/qrisp/circuit/controlled_operations.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 
 from qrisp.circuit import QuantumCircuit
 from qrisp.circuit import Qubit, XGate
 
 
 # This function takes a circuit and turns it into it's controlled version
 def multi_controlled_circuit(
```

### Comparing `qrisp-0.0.14/src/qrisp/circuit/instruction.py` & `qrisp-0.0.15/src/qrisp/circuit/instruction.py`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 
 
 class Instruction:
     """
     This class combines Operation objects with their operands (ie. qubits and classical
     bits). The data attribut of the QuantumCircuit class consists of a list of
     Instructions.
```

### Comparing `qrisp-0.0.14/src/qrisp/circuit/multi_cx.py` & `qrisp-0.0.15/src/qrisp/circuit/multi_cx.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/circuit/operation.py` & `qrisp-0.0.15/src/qrisp/circuit/operation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 
 import copy
 
 import numpy as np
 from sympy.core.expr import Expr
 
 
@@ -751,21 +751,28 @@
         if res.is_qfree is not None:
             res.is_qfree = bool(self.is_qfree)
 
         res.permeability = dict(self.permeability)
 
         return res
 
-    def substitute(self, subs_dic):
+    def bind_parameters(self, subs_dic):
         from copy import copy
 
         res = copy(self)
         if not isinstance(self.definition, type(None)):
-            res.definition = self.definition.substitute(subs_dic)
-        res.base_operation = self.base_operation.substitute(subs_dic)
+            res.definition = self.definition.bind_parameters(subs_dic)
+        res.base_operation = self.base_operation.bind_parameters(subs_dic)
+        
+        res.params = []
+        for p in self.params:
+            if p in subs_dic:
+                res.params.append(subs_dic[p])
+            else:
+                res.params.append(p)
 
         return res
 
 
 # Class to describe controlled operation
 # Very simlar to phase tolerant operations but with a more specifix naming
 # convention, inversion algorithm and unitary generation algorithm
```

### Comparing `qrisp-0.0.14/src/qrisp/circuit/quantum_circuit.py` & `qrisp-0.0.15/src/qrisp/circuit/quantum_circuit.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 
 from qrisp.circuit import Operation, Clbit, Qubit, Instruction
 
 import numpy as np
 import sympy
 import qrisp.circuit.standard_operations as ops
```

### Comparing `qrisp-0.0.14/src/qrisp/circuit/qubit.py` & `qrisp-0.0.15/src/qrisp/circuit/qubit.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 class Qubit:
     """
     This class describes qubits. Qubits are created by supplying the identifier string.
     
     Attributes
     ----------
     identifier : str
@@ -33,14 +33,16 @@
               ┌───┐
     alphonse: ┤ X ├
               └───┘
     
 
     """
     def __init__(self, identifier):
+        if identifier == "qb_[127]":
+            raise
         self.identifier = identifier
         self.hash_value = id(self)
         self.lock = False
         self.perm_lock = False
         
     def __str__(self):
         return self.identifier
```

### Comparing `qrisp-0.0.14/src/qrisp/circuit/standard_operations.py` & `qrisp-0.0.15/src/qrisp/circuit/standard_operations.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 
 # This file uses the gate constructor from operation.py to define
 # some standard operations
 
 import types
 from qrisp.circuit import PauliGate, U3Gate
 from qrisp.circuit.operation import Operation
```

### Comparing `qrisp-0.0.14/src/qrisp/circuit/transpiler.py` & `qrisp-0.0.15/src/qrisp/circuit/transpiler.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 
 
 import numpy as np
 from qrisp.circuit.operation import PTControlledOperation, ControlledOperation
 from qrisp.circuit.instruction import Instruction
 from qrisp.circuit.operation import Operation
 from qrisp.circuit.quantum_circuit import fast_append
```

### Comparing `qrisp-0.0.14/src/qrisp/circuit/transpiler_old.py` & `qrisp-0.0.15/src/qrisp/circuit/transpiler_old.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/core/__init__.py` & `qrisp-0.0.15/src/qrisp/core/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/core/compilation.py` & `qrisp-0.0.15/src/qrisp/core/compilation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 
 import numpy as np
 import networkx as nx
 from numba import njit, prange
 
 from qrisp.circuit import QuantumCircuit, Qubit, PTControlledOperation, ControlledOperation, transpile, QubitAlloc, Instruction, fast_append
 from qrisp.misc import get_depth_dic, retarget_instructions, reduce_depth
@@ -97,15 +97,15 @@
         transpiled_qc = transpile(qc, transpile_predicate = reordering_transpile_predicate)
         reordered_qc = reorder_qc(transpiled_qc)
         
         #Transpile logic synthesis
         reordered_qc = transpile(reordered_qc, transpile_predicate = lambda op : not (isinstance(op, PTControlledOperation) and op.base_operation.name in ["x"]))
         
         # We combine adjacent single qubit gates
-        if not reordered_qc.abstract_params:
+        if not qs.abstract_params:
             reordered_qc = combine_single_qubit_gates(reordered_qc)
         
         #We now determine the amount of Qubits the circuit will need    
         required_qubits = 0
         max_required_qubits = 0
         
         for instr in reordered_qc.data:
```

### Comparing `qrisp-0.0.14/src/qrisp/core/library.py` & `qrisp-0.0.15/src/qrisp/core/library.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 
 import qrisp.circuit.standard_operations as std_ops
 import numpy as np
 from qrisp.core import recursive_qs_search
 
 def append_operation(operation, qubits = [], clbits = []):
```

### Comparing `qrisp-0.0.14/src/qrisp/core/quantum_array.py` & `qrisp-0.0.15/src/qrisp/core/quantum_array.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 
 from itertools import product
 import copy
 from qrisp.core import QuantumVariable
 from qrisp.misc import bin_rep, int_encoder
 from qrisp.circuit import transpile
 
@@ -90,15 +90,15 @@
     >>> q_array_2[:] = np.eye(2)
     >>> print(q_array_2)
     {OutcomeArray([[1., 0.],
                    [0., 1.]]): 1.0}
     
     **Quantum indexing**
     
-    QuantumArrays can be dereferenced by :ref:`QuantumFloats`. This returns a :ref:`QuantumEnvironment` in which the corresponding entry is avaliable as a QuantumVariable. ::
+    QuantumArrays can be dereferenced by :ref:`QuantumFloats <QuantumFloat>`. This returns a :ref:`QuantumEnvironment` in which the corresponding entry is avaliable as a QuantumVariable. ::
         
         from qrisp import QuantumBool, QuantumArray, QuantumFloat, h, multi_measurement
     
         q_array = QuantumArray(QuantumBool(), shape = (4,4))
         index_0 = QuantumFloat(2)
         index_1 = QuantumFloat(2)
```

### Comparing `qrisp-0.0.14/src/qrisp/core/quantum_dictionary.py` & `qrisp-0.0.15/src/qrisp/core/quantum_dictionary.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 import numpy as np
 from qrisp.core import recursive_qv_search, QuantumVariable
 from qrisp.misc import custom_qv, bin_rep, int_as_array, gate_wrap
 import itertools
 from qrisp.logic_synthesis import TruthTable
```

### Comparing `qrisp-0.0.14/src/qrisp/core/quantum_session.py` & `qrisp-0.0.15/src/qrisp/core/quantum_session.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/core/quantum_variable.py` & `qrisp-0.0.15/src/qrisp/core/quantum_variable.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 
 import copy
 import weakref
 
 import numpy as np
 import matplotlib.pyplot as plt
 
@@ -734,15 +734,15 @@
             raise Exception("Tried to reduce QuantumVariable by invalid qubits")
 
 
         #Find Qubits to be cleared        
         for i in range(len(qubits)):
             for j in range(self.size):
                 if self.reg[j] == qubits[i]:
-                    self.reg[j].identifier = "qb_" + str(self.qs.qubit_index_counter)
+                    self.reg[j].identifier = "qb_" + str(self.qs.qubit_index_counter[0])
                     self.qs.qubit_index_counter += 1
                     self.reg.pop(j)
                     break
         
         self.qs.clear_qubits(qubits, verify)
         #Adjust variable size
         self.size -= len(qubits)
```

### Comparing `qrisp-0.0.14/src/qrisp/core/session_merging_tools.py` & `qrisp-0.0.15/src/qrisp/core/session_merging_tools.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 import weakref
 
 
 #This module contains the necessary tools to merge QuantumSessions
 
 #Due to the interplay with QuantumEnvironments and the behavior
 #that QuantumEnvironments automatically detect QuantumSessions that operated
```

### Comparing `qrisp-0.0.14/src/qrisp/default_backend.py` & `qrisp-0.0.15/src/qrisp/default_backend.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/environments/GMS_environment.py` & `qrisp-0.0.15/src/qrisp/environments/GMS_environment.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/environments/__init__.py` & `qrisp-0.0.15/src/qrisp/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/environments/control_environment.py` & `qrisp-0.0.15/src/qrisp/environments/control_environment.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 
 from qrisp.environments import QuantumEnvironment
 from qrisp.core.library import mcx, x, p, rz
 from qrisp.core.session_merging_tools import merge
 from qrisp.misc import perm_lock, perm_unlock
 from qrisp.circuit.qubit import Qubit
```

### Comparing `qrisp-0.0.14/src/qrisp/environments/gate_wrap_environment.py` & `qrisp-0.0.15/src/qrisp/environments/gate_wrap_environment.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 
 from qrisp.environments import QuantumEnvironment
 from qrisp.circuit import QuantumCircuit
 
 
 class GateWrapEnvironment(QuantumEnvironment):
     """
```

### Comparing `qrisp-0.0.14/src/qrisp/environments/quantum_conditionals.py` & `qrisp-0.0.15/src/qrisp/environments/quantum_conditionals.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 from qrisp.environments.quantum_environments import QuantumEnvironment
 from qrisp.environments.quantum_inversion import invert
 from qrisp.misc import (
     perm_lock,
     perm_unlock,
     unlock,
     redirect_qfunction,
```

### Comparing `qrisp-0.0.14/src/qrisp/environments/quantum_environments.py` & `qrisp-0.0.15/src/qrisp/environments/quantum_environments.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 
 # Abstract class to describe environments
 # The idea is to start dumping the circuit data into a container
 # (the .env_data attribute) once the environment is entered.
 # Meanwhile, the original data of the session is stored in the .original_data attribute.
 # The dumping is ended when the environment is left or a child environment is entered.
 # The child environment will append itself into the container, once it is left.
```

### Comparing `qrisp-0.0.14/src/qrisp/environments/quantum_inversion.py` & `qrisp-0.0.15/src/qrisp/environments/quantum_inversion.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 
 
 from qrisp.environments.quantum_environments import QuantumEnvironment
 from qrisp.circuit import QubitAlloc, QubitDealloc
 
 
 # Environment inheritor where the environment content is appended as the inverse
```

### Comparing `qrisp-0.0.14/src/qrisp/environments/temp_var_environment.py` & `qrisp-0.0.15/src/qrisp/environments/temp_var_environment.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 
 from qrisp.environments.quantum_inversion import invert
 from qrisp.environments.quantum_environments import QuantumEnvironment
 from qrisp.core.session_merging_tools import merge
 from qrisp.misc import lock, unlock
 from qrisp.core.quantum_variable import QuantumVariable
```

### Comparing `qrisp-0.0.14/src/qrisp/grover/grover_tools.py` & `qrisp-0.0.15/src/qrisp/grover/grover_tools.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 
 import numpy as np
 from qrisp import gate_wrap, h, x, gphase, mcz, mcp, QuantumVariable, QuantumArray
 
 
 # Applies the grover diffuser onto the (list of) quantum variable input_object
 def diffuser(input_object, phase = np.pi):
```

### Comparing `qrisp-0.0.14/src/qrisp/interface/__init__.py` & `qrisp-0.0.15/src/qrisp/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/interface/backends.py` & `qrisp-0.0.15/src/qrisp/interface/backends.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/interface/circuit_converter.py` & `qrisp-0.0.15/src/qrisp/interface/circuit_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 
 from qrisp.misc import bin_rep
 
 def convert_circuit(qc, target_api = "thrift", transpile = True):
 
     
     if transpile or target_api == "open_api":
@@ -154,15 +154,14 @@
     
     from qrisp.circuit import ControlledOperation
     for i in range(len(qc.data)):
         op = qc.data[i].op
         
         params = list(op.params)
         
-        
         #Prepare qiskit qubits
         qubit_list = [bit_dic[qubit.identifier] for qubit in qc.data[i].qubits]
         clbit_list = [bit_dic[clbit.identifier] for clbit in qc.data[i].clbits]
         
         if hasattr(op, "global_phase"):
             qiskit_qc.global_phase += op.global_phase
         
@@ -194,14 +193,15 @@
             else:
                 qiskit_ins = qsk_gates.YGate().control()
         
         elif issubclass(op.__class__, ControlledOperation):
             
             
             base_name = op.base_operation.name
+            
             if len(base_name) == 1:
                 base_name = base_name.upper()
             
             if op.base_operation.definition:
                 
                 qiskit_definition = convert_to_qiskit(op.base_operation.definition)
                 base_gate = qiskit_definition.to_gate()
```

### Comparing `qrisp-0.0.14/src/qrisp/interface/openapi_interface/__init__.py` & `qrisp-0.0.15/src/qrisp/interface/openapi_interface/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/interface/openapi_interface/backend_client.py` & `qrisp-0.0.15/src/qrisp/interface/openapi_interface/backend_client.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/interface/openapi_interface/backend_server.py` & `qrisp-0.0.15/src/qrisp/interface/openapi_interface/backend_server.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/interface/openapi_interface/interface_types.py` & `qrisp-0.0.15/src/qrisp/interface/openapi_interface/interface_types.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/interface/thrift_interface/__init__.py` & `qrisp-0.0.15/src/qrisp/interface/thrift_interface/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/interface/thrift_interface/backend_client.py` & `qrisp-0.0.15/src/qrisp/interface/thrift_interface/backend_client.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 
 import sys
 
 from qrisp.interface.circuit_converter import convert_circuit
 from qrisp.interface.thrift_interface.codegen import BackendService
```

### Comparing `qrisp-0.0.14/src/qrisp/interface/thrift_interface/backend_server.py` & `qrisp-0.0.15/src/qrisp/interface/thrift_interface/backend_server.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 
 import threading
 
 from thrift.transport import TSocket
 from thrift.transport import TTransport
 from thrift.protocol import TBinaryProtocol
 from qrisp.interface.thrift_interface.stoppable_thrift_server import StoppableThriftServer
```

### Comparing `qrisp-0.0.14/src/qrisp/interface/thrift_interface/codegen/BackendService.py` & `qrisp-0.0.15/src/qrisp/interface/thrift_interface/codegen/BackendService.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 #
 # Autogenerated by Thrift Compiler (0.15.0)
 #
 # DO NOT EDIT UNLESS YOU ARE SURE THAT YOU KNOW WHAT YOU ARE DOING
 #
 #  options string: py
 #
```

### Comparing `qrisp-0.0.14/src/qrisp/interface/thrift_interface/codegen/constants.py` & `qrisp-0.0.15/src/qrisp/interface/thrift_interface/codegen/constants.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/interface/thrift_interface/codegen/ttypes.py` & `qrisp-0.0.15/src/qrisp/interface/thrift_interface/codegen/ttypes.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 #
 # Autogenerated by Thrift Compiler (0.15.0)
 #
 # DO NOT EDIT UNLESS YOU ARE SURE THAT YOU KNOW WHAT YOU ARE DOING
 #
 #  options string: py
 #
```

### Comparing `qrisp-0.0.14/src/qrisp/interface/thrift_interface/interface_types.py` & `qrisp-0.0.15/src/qrisp/interface/thrift_interface/interface_types.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 
 from qrisp.interface.thrift_interface.codegen.ttypes import Qubit as PortableQubit
 from qrisp.interface.thrift_interface.codegen.ttypes import QuantumCircuit as PortableQuantumCircuit
 from qrisp.interface.thrift_interface.codegen.ttypes import Operation as PortableOperation
 from qrisp.interface.thrift_interface.codegen.ttypes import Instruction as PortableInstruction
 from qrisp.interface.thrift_interface.codegen.ttypes import Clbit as PortableClbit
 from qrisp.interface.thrift_interface.codegen.ttypes import ConnectivityEdge, BackendStatus
```

### Comparing `qrisp-0.0.14/src/qrisp/interface/thrift_interface/stoppable_thrift_server.py` & `qrisp-0.0.15/src/qrisp/interface/thrift_interface/stoppable_thrift_server.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/iterators/qrange.py` & `qrisp-0.0.15/src/qrisp/iterators/qrange.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/logic_synthesis/__init__.py` & `qrisp-0.0.15/src/qrisp/logic_synthesis/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/logic_synthesis/gray_synthesis.py` & `qrisp-0.0.15/src/qrisp/logic_synthesis/gray_synthesis.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 import numpy as np
 from qrisp.misc import int_as_array, int_encoder, array_as_int, gate_wrap
 import sympy as sp
 
 use_gray_code = False
 try:
     from ffht import fht as fwht
```

### Comparing `qrisp-0.0.14/src/qrisp/logic_synthesis/pprm_synthesis.py` & `qrisp-0.0.15/src/qrisp/logic_synthesis/pprm_synthesis.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/logic_synthesis/truth_tables.py` & `qrisp-0.0.15/src/qrisp/logic_synthesis/truth_tables.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/misc/GMS_tools.py` & `qrisp-0.0.15/src/qrisp/misc/GMS_tools.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 
 import numpy as np
 from qrisp.circuit import Operation
 
 
 class GXX_wrapper(Operation):
```

### Comparing `qrisp-0.0.14/src/qrisp/misc/depth_reduction.py` & `qrisp-0.0.15/src/qrisp/misc/depth_reduction.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/misc/utility.py` & `qrisp-0.0.15/src/qrisp/misc/utility.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 
 import traceback
 
 import numpy as np
 import sympy
 
 def bin_rep(n, bits):
```

### Comparing `qrisp-0.0.14/src/qrisp/qtypes/__init__.py` & `qrisp-0.0.15/src/qrisp/qtypes/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/qtypes/quantum_bool.py` & `qrisp-0.0.15/src/qrisp/qtypes/quantum_bool.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 
 from qrisp.core.quantum_variable import QuantumVariable
 from qrisp.environments import control
 import sys
 class QuantumBool(QuantumVariable):
     """
     QuantumBools are the quantum type, which represents boolean truth values.
```

### Comparing `qrisp-0.0.14/src/qrisp/qtypes/quantum_char.py` & `qrisp-0.0.15/src/qrisp/qtypes/quantum_char.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/qtypes/quantum_float.py` & `qrisp-0.0.15/src/qrisp/qtypes/quantum_float.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 
 from qrisp.core import QuantumVariable
 import numpy as np
 import sympy as sp
 from qrisp.misc import gate_wrap
-from qrisp.arithmetic import polynomial_encoder, lt, gt, leq, geq, eq, neq, inpl_mult, sbp_add
+from qrisp.arithmetic import polynomial_encoder, lt, gt, leq, geq, eq, neq, inpl_mult, sbp_add, q_mult
 
 def signed_int_iso(x, n):
     if int(x) < -2**n or int(x) >= 2**n:
         raise Exception("Applying signed integer isomorphism resulted in overflow")
     
     if x >= 0:
         return x%2**n
@@ -59,29 +59,29 @@
     This subclass of :ref:`QuantumVariable` can represent floating point numbers (signed and unsigned) up to an arbitrary precision.
     
     The technical details of the employed arithmetic can be found in this `article <https://ieeexplore.ieee.org/document/9815035>`_. 
     
     To create a QuantumFloat we call the constructor:
     
     >>> from qrisp import QuantumFloat
-    >>> qf_0 = QuantumFloat(3, -1, signed = False)
+    >>> a = QuantumFloat(3, -1, signed = False)
     
     Here, the 3 indicates the amount of mantissa qubits and the -1 indicates the exponent.
     
     For unsigned QuantumFloats, the decoder function is given by
     
     .. math::
         
         f_{k}(i) = i2^{k}
     
     Where $k$ is the exponent.
     
     We can check which values can be represented:
     
-    >>> for i in range(2**qf_0.size): print(qf_0.decoder(i))
+    >>> for i in range(2**a.size): print(a.decoder(i))
     0.0
     0.5
     1.0
     1.5
     2.0
     2.5
     3.0
@@ -96,16 +96,16 @@
         f_{k}^{n}(i) = \begin{cases} i2^{k} & \text{if } i < 2^n \\ (i - 2^{n+1})2^k & \text{else} \end{cases}
     
     Where $k$ is again, the exponent and $n$ is the mantissa size.
     
     
     Another example:
     
-    >>> qf_1 = QuantumFloat(2, -2, signed = True)
-    >>> for i in range(2**qf_1.size): print(qf_1.decoder(i))
+    >>> b = QuantumFloat(2, -2, signed = True)
+    >>> for i in range(2**b.size): print(b.decoder(i))
     0.0
     0.25
     0.5
     0.75
     -1.0
     -0.75
     -0.5
@@ -116,141 +116,141 @@
     
     **Arithmetic**
     
     Many operations known from classical arithmetic work for QuantumFloats in infix notation.
     
     Addition:
     
-    >>> qf_0[:] = 1.5
-    >>> qf_1[:] = 0.25
-    >>> qf_3 = qf_0 + qf_1
-    >>> print(qf_3)
+    >>> a[:] = 1.5
+    >>> b[:] = 0.25
+    >>> c = a + b
+    >>> print(c)
     {1.75: 1.0}
     
     Subtraction:
     
-    >>> qf_4 = qf_0 - qf_3
-    >>> print(qf_4)
+    >>> d = a - c
+    >>> print(d)
     {-0.25: 1.0}
     
     Multiplication:
-        
-    >>> qf_5 = qf_4 * qf_1
-    >>> print(qf_5)
+    
+    >>> e = d * b
+    >>> print(e)
     {-0.0625: 1.0}
     
     And even division:
         
-    >>> qf_6 = QuantumFloat(3)
-    >>> qf_7 = QuantumFloat(3)
-    >>> qf_6[:] = 7
-    >>> qf_7[:] = 2
-    >>> qf_8 = qf_6/qf_7
-    >>> print(qf_8)
+    >>> a = QuantumFloat(3)
+    >>> b = QuantumFloat(3)
+    >>> a[:] = 7
+    >>> b[:] = 2
+    >>> c = a/b
+    >>> print(c)
     {3.5: 1.0}
     
     Floor division:
         
-    >>> qf_9 = qf_6//qf_7
-    >>> print(qf_9)
+    >>> d = a//b
+    >>> print(d)
     {3.0: 1.0}
     
     Inversion:
     
-    >>> qf_10 = QuantumFloat(3, -1)
-    >>> qf_10[:] = 3.5
-    >>> qf_11 = qf_10**-1
-    >>> print(qf_11)
+    >>> a = QuantumFloat(3, -1)
+    >>> a[:] = 3.5
+    >>> b= a**-1
+    >>> print(b)
     {0.25: 1.0}
     
     Note that the latter is only an approximate result. This is because in many cases, the results of division can not be stored in a finite amount of qubits, forcing us to approximate.
     To get a better approximation we can use the :meth:`q_div <qrisp.q_div>` and :meth:`qf_inversion <qrisp.qf_inversion>` functions and specify the precision:
     
     >>> from qrisp import q_div, qf_inversion
-    >>> qf_12 = QuantumFloat(3)
-    >>> qf_12[:] = 1
-    >>> qf_13 = QuantumFloat(3)
-    >>> qf_13[:] = 7
-    >>> qf_14 = q_div(qf_12, qf_13, prec = 6)
-    >>> print(qf_14)
+    >>> a = QuantumFloat(3)
+    >>> a[:] = 1
+    >>> b = QuantumFloat(3)
+    >>> b[:] = 7
+    >>> c = q_div(a, b, prec = 6)
+    >>> print(c)
     {0.140625: 1.0}
     
     Comparing with the classical result (0.1428571428):
     
     >>> 1/7 - 0.140625
     0.002232142857142849
     
     We see that the result is inside the expected precision of $2^{-6} =  0.015625$.
     
     
     **In-place Operations**
     
     Further supported operations are inplace addition, subtraction (with both classical and quantum values):
         
-    >>> qf_15 = QuantumFloat(4, signed = True)
-    >>> qf_15[:] = 4
-    >>> qf_16 = QuantumFloat(4)
-    >>> qf_16[:] = 3
-    >>> qf_15 += qf_16
-    >>> print(qf_15)
+    >>> a = QuantumFloat(4, signed = True)
+    >>> a[:] = 4
+    >>> b = QuantumFloat(4)
+    >>> b[:] = 3
+    >>> a += b
+    >>> print(a)
     {7: 1.0}
-    >>> qf_15 -= 2
-    >>> print(qf_15)
+    >>> a -= 2
+    >>> print(a)
     {5: 1.0}
     
     .. warning::
         Additions that would result in overflow, raise no errors. Instead the additions are performed `modular <https://en.wikipedia.org/wiki/Modular_arithmetic>`_.
         
-        >>> a = QuantumFloat(3)
-        >>> a += 9
-        >>> print(a)
+        >>> c = QuantumFloat(3)
+        >>> c += 9
+        >>> print(c)
         {1: 1.0}
     
     For inplace multiplications, only classical integers are allowed:
     
-    >>> qf_15 *= -3
-    >>> print(qf_15)
+    >>> a *= -3
+    >>> print(a)
     {-15: 1.0}
     
     .. note::
         In-place multiplications can change the mantissa size to prevent overflow errors. If you want to prevent this behavior, look into :meth:`inpl_mult <qrisp.inpl_mult>`.
         
-        >>> qf.qf_15.size
+        >>> a.size
         7
     
     **Bitshifts**
     
     Bitshifts can be executed for free (ie. not requiring any quantum gates). We can either use the :meth:`exp_shift <qrisp.QuantumFloat.exp_shift>` method or use the infix operators. Note that the bitshifts work in-place.
     
     
-    >>> qf_15.exp_shift(3)
-    >>> print(qf_15)
-    {40: 1.0}
-    >>> qf_15 >> 5
-    >>> print(qf_15)
-    {1.25: 1.0}
+    >>> a.exp_shift(3)
+    >>> print(a)
+    {-120: 1.0}
+    >>> a >> 5
+    >>> print(a)
+    {-3.75: 1.0}
     
     **Comparisons**
     
     QuantumFloats can be compared to Python floats using the established operators. The return values are :ref:`QuantumBools <QuantumBool>`:
         
     >>> from qrisp import h
-    >>> qf_16 = QuantumFloat(4)
-    >>> h(qf_16[2])
-    >>> print(qf_16)
+    >>> a = QuantumFloat(4)
+    >>> h(a[2])
+    >>> print(a)
     {0: 0.5, 4: 0.5}
-    >>> comparison_qbl_0 = (qf_16 < 4 )
+    >>> comparison_qbl_0 = (a < 4 )
     >>> print(comparison_qbl_0)
     {False: 0.5, True: 0.5}
 
     Comparison to other QuantumFloats also works:
         
-    >>> qf_17 = QuantumFloat(3)
-    >>> qf_17[:] = 4
-    >>> comparison_qbl_1 = (qf_17 == qf_16)
+    >>> b = QuantumFloat(3)
+    >>> b[:] = 4
+    >>> comparison_qbl_1 = (a == b)
     >>> comparison_qbl_1.qs.statevector()
     sqrt(2)*(|0>*|True>*|4>*|False> + |4>*|False>*|4>*|True>)/2
     
     The first tensor factor containing a boolean value is corresponding to ``comparison_qbl_0`` and the second one is ``comparison_qbl_1``.
     
     """
     
@@ -297,16 +297,14 @@
     #     if self.signed:
     #         res = int(signed_int_iso(i/2**self.exponent, self.size-1))
     #     else:
     #         res =  int(i/2**self.exponent)
             
     #     return res
         
-        
-    
     def sb_poly(self, m = 0):
         """
         Returns the semi-boolean polynomial of this `QuantumFloat` where `m` specifies the image extension parameter.
         
         For the technical details we refer to: https://ieeexplore.ieee.org/document/9815035
         
 
@@ -764,43 +762,14 @@
         {0.5: 1.0}
 
         """
         decoder_values = np.array([self.decoder(i) for i in range(2**self.size)])
         
         return decoder_values[np.argmin(np.abs(decoder_values - x))]
         
-
-
-from qrisp.misc import gate_wrap
-
-def q_mult(factor_1, factor_2, target = None, method = "auto"):
-    
-    if method == "auto":
-        
-        if factor_1.reg == factor_2.reg:
-            return q_mult(factor_1, factor_2, target, method = "sbp")
-        else:
-            return q_mult(factor_1, factor_2, target, method = "hybrid")
-
-    elif method == "sbp":
-        
-        from qrisp import sbp_mult, merge
-        if target is None:
-            target = create_output_qf([factor_1, factor_2], op = "mul")
-        
-        merge([target, factor_1, factor_2])
-        
-        
-        sbp_mult(factor_1, factor_2, target)
-        return target
-    
-    elif method == "hybrid":
-        from qrisp.arithmetic import hybrid_mult
-        return hybrid_mult(factor_1, factor_2)
-
 def create_output_qf(operands, op):
     
     if isinstance(op, sp.core.expr.Expr):
         from qrisp.arithmetic.poly_tools import expr_to_list
         
         expr_list = expr_to_list(op)
         
@@ -917,115 +886,7 @@
         if qf1_sign_list[i] > max(qf2_sign_list) and qf2.signed:
             qs.cx(qf2[-1], qf1[i])
     
     #Copy the sign bit
     if qf2.signed:
         qs.cx(qf2[-1], qf1[-1])
 
-
-
-
-# @adaptive_condition
-# def less_than(qf_0, qf_1):
-#     lt_qbl = QuantumBool()
-#     if qf_0.signed:
-#         qf_0 -= qf_1
-#         cx(qf_1[-1], lt_qbl)
-#         # The last qubit holds the sign of the QuantumFloat
-#         qf_0 += qf_1
-#         return lt_qbl
-#     else:
-#         temp_qf = qf_0 - qf_1
-#         cx(temp_qf[-1], lt_qbl)
-#         return lt_qbl
-
-# @adaptive_condition
-# def greater_than(qf_0, qf_1):
-#     gt_qbl = QuantumBool()
-#     if qf_0.signed:
-#         qf_1 -= qf_0
-#         # The last qubit holds the sign of the QuantumFloat
-#         cx(qf_1[-1], gt_qbl)
-#         qf_1 += qf_0
-#         return gt_qbl
-#     else:
-#         temp_qf = qf_1 - qf_0
-#         cx(temp_qf[-1], gt_qbl)
-#         return gt_qbl
-
-# @adaptive_condition
-# def less_than_or_equal(qf_0, qf_1):
-#     leq_qbl = QuantumBool()
-#     if qf_0.signed:
-#         qf_1 -= qf_0
-#         # The last qubit holds the sign of the QuantumFloat
-#         cx(qf_0[-1], leq_qbl)
-#         qf_1 += qf_0
-#         leq_qbl.flip()
-#         return leq_qbl
-#     else:
-#         temp_qf = qf_1 - qf_0
-        
-#         cx(temp_qf[-1], leq_qbl)
-#         leq_qbl.flip()
-#         return leq_qbl
-
-# @adaptive_condition
-# def greater_than_or_equal(qf_0, qf_1):
-#     geq_qbl = QuantumBool()
-#     if hasattr(qf_0, 'signed') and qf_0.signed:
-#         qf_0 -= qf_1
-#         # The last qubit holds the sign of the QuantumFloat
-#         cx(qf_0[-1], geq_qbl)
-#         qf_0 += qf_1
-#         geq_qbl.flip()
-#         return geq_qbl
-#     else:
-#         temp_qf = qf_0 - qf_1
-#         cx(temp_qf[-1], geq_qbl)
-#         geq_qbl.flip()
-#         return geq_qbl
-
-
-# #TO-DO implement without arithmetic?
-# @adaptive_condition
-# def equal(qf_0, qf_1):
-    
-#     eq_qbl = QuantumBool()
-    
-#     if isinstance(qf_1, QuantumFloat):
-#         if not qf_0.signed and not qf_1.signed:
-#             if qf_0.exponent > qf_1.exponent:
-#                 qf_0, qf_1 = qf_1, qf_0
-                
-#             min_sig = qf_0.mshape[0]
-#             max_sig = max(qf_0.mshape[1], qf_1.mshape[1])
-            
-#             temp_qf = QuantumFloat(max_sig - min_sig)
-            
-#             cx(qf_0, temp_qf[:qf_0.size])
-#             cx(qf_1, temp_qf[-qf_1.size:])
-            
-#             mcx(temp_qf, eq_qbl, ctrl_state = 0)
-            
-#             return eq_qbl
-        
-#     temp_qf = qf_0 - qf_1
-        
-#     mcx(temp_qf, eq_qbl, ctrl_state = 0)
-    
-#     return eq_qbl
-
-# @adaptive_condition
-# def always_true():
-#     qbl = QuantumBool()
-#     qbl.flip()
-#     return qbl
-
-# @adaptive_condition
-# def always_false():
-#     from qrisp import QuantumBool
-#     qbl = QuantumBool()
-#     return qbl
-
-
-
```

### Comparing `qrisp-0.0.14/src/qrisp/qtypes/quantum_string.py` & `qrisp-0.0.15/src/qrisp/qtypes/quantum_string.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/quantum_network/__init__.py` & `qrisp-0.0.15/src/qrisp/quantum_network/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/quantum_network/interface/codegen/QuantumNetworkService.py` & `qrisp-0.0.15/src/qrisp/quantum_network/interface/codegen/QuantumNetworkService.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/quantum_network/interface/codegen/constants.py` & `qrisp-0.0.15/src/qrisp/quantum_network/interface/codegen/constants.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/quantum_network/interface/codegen/ttypes.py` & `qrisp-0.0.15/src/qrisp/quantum_network/interface/codegen/ttypes.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/quantum_network/interface_connection_example.py` & `qrisp-0.0.15/src/qrisp/quantum_network/interface_connection_example.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/quantum_network/qn_client.py` & `qrisp-0.0.15/src/qrisp/quantum_network/qn_client.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 
 from qrisp.interface.circuit_converter import convert_circuit
 from qrisp.quantum_network.interface.codegen import QuantumNetworkService
 from qrisp.quantum_network.interface.codegen.ttypes import Message
 from qrisp.interface import PortableQubit
 from qrisp import Qubit
```

### Comparing `qrisp-0.0.14/src/qrisp/quantum_network/qn_server.py` & `qrisp-0.0.15/src/qrisp/quantum_network/qn_server.py`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 
 import threading
 
 from thrift.transport import TSocket
 from thrift.transport import TTransport
 from thrift.protocol import TBinaryProtocol
 from thrift.server import TServer, TNonblockingServer
```

### Comparing `qrisp-0.0.14/src/qrisp/quantum_network/qn_simulator_server.py` & `qrisp-0.0.15/src/qrisp/quantum_network/qn_simulator_server.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/quantum_network/quantum_network_session.py` & `qrisp-0.0.15/src/qrisp/quantum_network/quantum_network_session.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 from qrisp.circuit import QuantumCircuit, transpile, QubitAlloc, QubitDealloc
 from qrisp import QuantumSession, QuantumFloat, QuantumChar, QuantumBool, merge
 from qrisp.quantum_network import QuantumNetworkClient
 import numpy as np
 
 class QuantumNetworkSession(QuantumSession):
     """
```

### Comparing `qrisp-0.0.14/src/qrisp/simulator/__init__.py` & `qrisp-0.0.15/src/qrisp/simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/simulator/bi_array_helper.py` & `qrisp-0.0.15/src/qrisp/simulator/bi_array_helper.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/simulator/bi_arrays.py` & `qrisp-0.0.15/src/qrisp/simulator/bi_arrays.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/simulator/bi_arrays_new.py` & `qrisp-0.0.15/src/qrisp/simulator/bi_arrays_new.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/simulator/circuit_preprocessing.py` & `qrisp-0.0.15/src/qrisp/simulator/circuit_preprocessing.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/simulator/circuit_reordering.py` & `qrisp-0.0.15/src/qrisp/simulator/circuit_reordering.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/simulator/impure_quantum_state.py` & `qrisp-0.0.15/src/qrisp/simulator/impure_quantum_state.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/simulator/quantum_state.py` & `qrisp-0.0.15/src/qrisp/simulator/quantum_state.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/simulator/simulator.py` & `qrisp-0.0.15/src/qrisp/simulator/simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 def run(qc, shots, token = "", iqs = None, insert_reset = True):
     
     #This command enables fast appending. Fast appending means that the .append method of the QuantumCircuit
     #class checks much less validity conditions and is also less tolerant regarding inputs.
     
     print(f"Simulating {len(qc.qubits)} qubits..", end = "\r")
     
-    
     with fast_append():
         
         #We convert the circuit which is given with portable objects to a qrisp circuit
         qc = convert_circuit(qc, "qrisp", transpile = True)
         
         
         #Count the amount of measurements (we can stop the simulation after all measurements are performed)
@@ -130,15 +129,16 @@
             if measurement_counter == measurement_amount:
                 break
         
         progress_bar.close()
         
         LINE_UP = '\033[1A'
         LINE_CLEAR = '\x1b[2K'
-        print(LINE_CLEAR, end=LINE_UP)
+        print(LINE_CLEAR, end= "\r")
+        # print(LINE_UP, end = "")
         
         
         #Prepare result dictionary
         #The iqs object contains the outcome bitstrings in the attribute .outcome_list and the probablities in .cl_prob
         #In order to ensure qiskit compatibility, we reverse the bitstrings
         res = {}
         for i in range(len(iqs.cl_prob)):
@@ -227,15 +227,16 @@
         
         res = qs.eval().tensor_array.to_array()
         
         progress_bar.close()
         
         LINE_UP = '\033[1A'
         LINE_CLEAR = '\x1b[2K'
-        print(LINE_CLEAR, end=LINE_UP)
+        print(LINE_CLEAR, end= "\r")
+        # print(LINE_UP, end = "")
         
         
         
         #Deactivate the fast append mode
         QuantumCircuit.fast_append = False
         
         return res
```

### Comparing `qrisp-0.0.14/src/qrisp/simulator/tensor_factor.py` & `qrisp-0.0.15/src/qrisp/simulator/tensor_factor.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/simulator/unitary_management.py` & `qrisp-0.0.15/src/qrisp/simulator/unitary_management.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/uncomputation/__init__.py` & `qrisp-0.0.15/src/qrisp/uncomputation/__init__.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/src/qrisp/uncomputation/type_checker.py` & `qrisp-0.0.15/src/qrisp/uncomputation/type_checker.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 import numpy as np
 
 #Checks if a gate is permeable on a set of qubits
 #Permeable means that the gate has the form
 # U = \sum_{x = 0}^{2^n} |x><x| U_x
 #where the braket expression represents the qubits
 #of the list "qubit_indices"
```

### Comparing `qrisp-0.0.14/src/qrisp/uncomputation/uncomputation.py` & `qrisp-0.0.15/src/qrisp/uncomputation/uncomputation.py`

 * *Ordering differences only*

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 
 import numpy as np
 
 def auto_uncompute(*args, recompute = False):
     if len(args):
         return auto_uncompute_inner(args[0])
     else:
```

### Comparing `qrisp-0.0.14/src/qrisp/uncomputation/unqomp.py` & `qrisp-0.0.15/src/qrisp/uncomputation/unqomp.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 
 from networkx import DiGraph
 import networkx as nx
 from qrisp.uncomputation.type_checker import is_permeable, is_qfree
 from qrisp.circuit import ControlledOperation, PTControlledOperation, QubitDealloc, QubitAlloc, Instruction, QuantumCircuit
 from qrisp.logic_synthesis import LogicSynthGate
```

### Comparing `qrisp-0.0.14/src/qrisp.egg-info/PKG-INFO` & `qrisp-0.0.15/src/qrisp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qrisp
-Version: 0.0.14
+Version: 0.0.15
 Summary: Qrisp - A high level language for gate-based quantum computing
 Home-page: https://github.com/pypa/sampleproject
 Author: Raphael Seidel
 Author-email: raphael.seidel@fokus.fraunhofer.de
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Eclipse Public License 2.0 (EPL-2.0)
```

### Comparing `qrisp-0.0.14/src/qrisp.egg-info/SOURCES.txt` & `qrisp-0.0.15/src/qrisp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/tests/test_GMS_environment_example.py` & `qrisp-0.0.15/tests/test_GMS_environment_example.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/tests/test_GXX_converter_example.py` & `qrisp-0.0.15/tests/test_GXX_converter_example.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/tests/test_GXX_gates_example.py` & `qrisp-0.0.15/tests/test_GXX_gates_example.py`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 # Created by ann81984 at 05.05.2022
 import pytest
 import numpy as np
 
 from qrisp import QuantumSession, QuantumVariable
 from qrisp.misc.GMS_tools import gms_multi_cx_fan_out, gms_multi_cx_fan_in, gms_multi_cp_gate, gms_multi_cp_gate_mono_phase, GXX_wrapper
 from qrisp import x
```

### Comparing `qrisp-0.0.14/tests/test_GZZ_gates_example.py` & `qrisp-0.0.15/tests/test_GZZ_gates_example.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 # Created by ann81984 at 05.05.2022
 import pytest
 import numpy as np
 
 from qrisp import QuantumSession, QuantumVariable, QuantumCircuit
 from qrisp.misc.GMS_tools import gms_multi_cx_fan_out, gms_multi_cx_fan_in, gms_multi_cp_gate, \
     gms_multi_cp_gate_mono_phase, GXX_wrapper, GZZ_converter
```

### Comparing `qrisp-0.0.14/tests/test_abstract_parameters.py` & `qrisp-0.0.15/tests/test_abstract_parameters.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/tests/test_array_entry_manipulation.py` & `qrisp-0.0.15/tests/test_array_entry_manipulation.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/tests/test_comparisons.py` & `qrisp-0.0.15/tests/test_comparisons.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/tests/test_conditional_environments_example.py` & `qrisp-0.0.15/tests/test_conditional_environments_example.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/tests/test_controlled_gates.py` & `qrisp-0.0.15/tests/test_controlled_gates.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/tests/test_diagonal_hamiltonian_application.py` & `qrisp-0.0.15/tests/test_diagonal_hamiltonian_application.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/tests/test_gray_synthesis_example.py` & `qrisp-0.0.15/tests/test_gray_synthesis_example.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/tests/test_grovers_algorithm.py` & `qrisp-0.0.15/tests/test_grovers_algorithm.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/tests/test_hello_world.py` & `qrisp-0.0.15/tests/test_hello_world.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/tests/test_inpl_matrix_multiplication_example.py` & `qrisp-0.0.15/tests/test_inpl_matrix_multiplication_example.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/tests/test_interface.py` & `qrisp-0.0.15/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/tests/test_loops.py` & `qrisp-0.0.15/tests/test_loops.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/tests/test_matrix_multiplication_example.py` & `qrisp-0.0.15/tests/test_matrix_multiplication_example.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/tests/test_mcx.py` & `qrisp-0.0.15/tests/test_mcx.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 
 def test_mcx():
     
     from qrisp import h, mcx, QuantumVariable, multi_measurement, bin_rep
     import numpy as np
     def test_mcx_inner(n, ctrl_state, method, test_phase = True, num_ancilla = 0):
```

### Comparing `qrisp-0.0.14/tests/test_measurement_reduction.py` & `qrisp-0.0.15/tests/test_outcome_array.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 * which is available at https://www.eclipse.org/legal/epl-2.0/
 *
 * SPDX-License-Identifier: EPL-2.0
 **********************************************************************/
 """
 
 
-from qrisp import QuantumFloat, h
-
-def test_measurement_reduction():
+def outome_array_hashing_test():
+    from qrisp import OutcomeArray
+    import numpy as np
     
-    qf = QuantumFloat(4)
-    h(qf)
-    qbls = []
-    for i in range(100):
-        qbls.append(qf == 2)
-
-    assert qbls[50].get_measurement() == {False: 0.9375, True: 0.0625}
+    test = OutcomeArray(np.eye(3))
+    
+    test_dic = {test : 1}
+    
+    test_dic[str(np.eye(3))]
+    
+    assert str(np.eye(3)) == str(test)
```

### Comparing `qrisp-0.0.14/tests/test_qiskit_backend_client.py` & `qrisp-0.0.15/tests/test_qiskit_backend_client.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/tests/test_qompiler.py` & `qrisp-0.0.15/tests/test_qompiler.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/tests/test_quantum_arithmetic.py` & `qrisp-0.0.15/tests/test_quantum_arithmetic.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""
-/*********************************************************************
-* Copyright (c) 2023 the Qrisp Authors
-*
-* This program and the accompanying materials are made
-* available under the terms of the Eclipse Public License 2.0
-* which is available at https://www.eclipse.org/legal/epl-2.0/
-*
-* SPDX-License-Identifier: EPL-2.0
-**********************************************************************/
-"""
-
+"""
+/*********************************************************************
+* Copyright (c) 2023 the Qrisp Authors
+*
+* This program and the accompanying materials are made
+* available under the terms of the Eclipse Public License 2.0
+* which is available at https://www.eclipse.org/legal/epl-2.0/
+*
+* SPDX-License-Identifier: EPL-2.0
+**********************************************************************/
+"""
+
 
 def test_quantum_arithmetic():
     
     import numpy as np
     from qrisp import h, multi_measurement, q_div, QuantumFloat
     def test_arithmetic_helper(qf_0, qf_1, operation):
```

### Comparing `qrisp-0.0.14/tests/test_quantum_dictionary.py` & `qrisp-0.0.15/tests/test_quantum_dictionary.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/tests/test_quantum_division.py` & `qrisp-0.0.15/tests/test_quantum_division.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/tests/test_quantum_teleportation.py` & `qrisp-0.0.15/tests/test_quantum_teleportation.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/tests/test_state_preparation.py` & `qrisp-0.0.15/tests/test_state_preparation.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/tests/test_string_test.py` & `qrisp-0.0.15/tests/test_string_test.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/tests/test_uncomputation_example.py` & `qrisp-0.0.15/tests/test_uncomputation_example.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/tests/test_unitary_calculation.py` & `qrisp-0.0.15/tests/test_unitary_calculation.py`

 * *Files identical despite different names*

### Comparing `qrisp-0.0.14/tests/tests_doc_examples.py` & `qrisp-0.0.15/tests/tests_doc_examples.py`

 * *Files identical despite different names*

