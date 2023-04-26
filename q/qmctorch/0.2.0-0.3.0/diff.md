# Comparing `tmp/qmctorch-0.2.0.tar.gz` & `tmp/qmctorch-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/nico/QMCTorch/dist/tmpk0l104n3/qmctorch-0.2.0.tar", last modified: Wed Jun 16 17:02:50 2021, max compression
+gzip compressed data, was "/home/nico/QMCTorch/dist/.tmp-wbk7uea6/qmctorch-0.3.0.tar", last modified: Wed Apr 26 15:00:54 2023, max compression
```

## Comparing `qmctorch-0.2.0.tar` & `qmctorch-0.3.0.tar`

### file list

```diff
@@ -1,180 +1,180 @@
-drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2021-06-16 17:02:50.766533 qmctorch-0.2.0/
--rw-rw-r--   0 nico      (1000) nico      (1000)    11359 2021-03-19 12:51:47.000000 qmctorch-0.2.0/LICENSE
--rw-rw-r--   0 nico      (1000) nico      (1000)       35 2021-03-19 12:51:47.000000 qmctorch-0.2.0/MANIFEST.in
--rw-rw-r--   0 nico      (1000) nico      (1000)       55 2021-03-19 12:51:47.000000 qmctorch-0.2.0/NOTICE
--rw-rw-r--   0 nico      (1000) nico      (1000)     1972 2021-06-16 17:02:50.766533 qmctorch-0.2.0/PKG-INFO
--rw-rw-r--   0 nico      (1000) nico      (1000)     1156 2021-03-19 12:51:47.000000 qmctorch-0.2.0/README.md
-drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2021-06-16 17:02:50.754533 qmctorch-0.2.0/bin/
--rwxrwxr-x   0 nico      (1000) nico      (1000)     1530 2021-06-16 16:49:19.000000 qmctorch-0.2.0/bin/qmctorch
-drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2021-06-16 17:02:50.754533 qmctorch-0.2.0/qmctorch/
--rw-rw-r--   0 nico      (1000) nico      (1000)      534 2021-03-19 12:51:47.000000 qmctorch-0.2.0/qmctorch/__init__.py
--rw-rw-r--   0 nico      (1000) nico      (1000)       22 2021-06-16 16:55:37.000000 qmctorch-0.2.0/qmctorch/__version__.py
-drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2021-06-16 17:02:50.754533 qmctorch-0.2.0/qmctorch/sampler/
--rw-rw-r--   0 nico      (1000) nico      (1000)      266 2021-03-19 12:51:47.000000 qmctorch-0.2.0/qmctorch/sampler/__init__.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     6404 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/sampler/generalized_metropolis.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     5325 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/sampler/hamiltonian.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     9680 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/sampler/metropolis.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     2158 2021-03-19 12:51:47.000000 qmctorch-0.2.0/qmctorch/sampler/sampler_base.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     4967 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/sampler/walkers.py
-drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2021-06-16 17:02:50.754533 qmctorch-0.2.0/qmctorch/scf/
--rw-rw-r--   0 nico      (1000) nico      (1000)       55 2021-03-19 12:51:47.000000 qmctorch-0.2.0/qmctorch/scf/__init__.py
-drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2021-06-16 17:02:50.754533 qmctorch-0.2.0/qmctorch/scf/calculator/
--rw-rw-r--   0 nico      (1000) nico      (1000)      176 2021-03-19 12:51:47.000000 qmctorch-0.2.0/qmctorch/scf/calculator/__init__.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     6976 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/scf/calculator/adf.py
--rw-rw-r--   0 nico      (1000) nico      (1000)      968 2021-03-19 12:51:47.000000 qmctorch-0.2.0/qmctorch/scf/calculator/calculator_base.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     5554 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/scf/calculator/pyscf.py
--rw-rw-r--   0 nico      (1000) nico      (1000)    13028 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/scf/molecule.py
-drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2021-06-16 17:02:50.754533 qmctorch-0.2.0/qmctorch/solver/
--rw-rw-r--   0 nico      (1000) nico      (1000)      251 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/solver/__init__.py
--rw-rw-r--   0 nico      (1000) nico      (1000)    17060 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/solver/solver_base.py
--rw-rw-r--   0 nico      (1000) nico      (1000)    16319 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/solver/solver_slater_jastrow.py
--rw-rw-r--   0 nico      (1000) nico      (1000)    10045 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/solver/solver_slater_jastrow_horovod.py
-drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2021-06-16 17:02:50.758533 qmctorch-0.2.0/qmctorch/utils/
--rw-rw-r--   0 nico      (1000) nico      (1000)     1529 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/utils/__init__.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     1900 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/utils/algebra_utils.py
--rw-rw-r--   0 nico      (1000) nico      (1000)    12585 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/utils/hdf5_utils.py
--rw-rw-r--   0 nico      (1000) nico      (1000)    12151 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/utils/interpolate.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     7419 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/utils/plot_data.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     1770 2021-03-19 12:51:47.000000 qmctorch-0.2.0/qmctorch/utils/stat_utils.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     7580 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/utils/torch_utils.py
-drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2021-06-16 17:02:50.758533 qmctorch-0.2.0/qmctorch/wavefunction/
--rw-rw-r--   0 nico      (1000) nico      (1000)      529 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/__init__.py
-drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2021-06-16 17:02:50.758533 qmctorch-0.2.0/qmctorch/wavefunction/jastrows/
--rw-rw-r--   0 nico      (1000) nico      (1000)        0 2021-06-14 16:21:28.000000 qmctorch-0.2.0/qmctorch/wavefunction/jastrows/__init__.py
-drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2021-06-16 17:02:50.758533 qmctorch-0.2.0/qmctorch/wavefunction/jastrows/distance/
--rw-rw-r--   0 nico      (1000) nico      (1000)      126 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/jastrows/distance/__init__.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     6572 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/jastrows/distance/electron_electron_distance.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     4932 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/jastrows/distance/electron_nuclei_distance.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     2072 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/jastrows/distance/scaling.py
-drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2021-06-16 17:02:50.758533 qmctorch-0.2.0/qmctorch/wavefunction/jastrows/elec_elec/
--rw-rw-r--   0 nico      (1000) nico      (1000)        0 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/jastrows/elec_elec/__init__.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     9691 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/jastrows/elec_elec/jastrow_factor_electron_electron.py
-drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2021-06-16 17:02:50.758533 qmctorch-0.2.0/qmctorch/wavefunction/jastrows/elec_elec/kernels/
--rw-rw-r--   0 nico      (1000) nico      (1000)      280 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/jastrows/elec_elec/kernels/__init__.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     3241 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/jastrows/elec_elec/kernels/fully_connected_jastrow_kernel.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     4499 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/jastrows/elec_elec/kernels/jastrow_kernel_electron_electron_base.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     4756 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/jastrows/elec_elec/kernels/pade_jastrow_kernel.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     9216 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/jastrows/elec_elec/kernels/pade_jastrow_polynomial_kernel.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     5158 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/jastrows/elec_elec/orbital_dependent_jastrow_kernel.py
-drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2021-06-16 17:02:50.758533 qmctorch-0.2.0/qmctorch/wavefunction/jastrows/elec_elec_nuclei/
--rw-rw-r--   0 nico      (1000) nico      (1000)        0 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/jastrows/elec_elec_nuclei/__init__.py
--rw-rw-r--   0 nico      (1000) nico      (1000)    14483 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/jastrows/elec_elec_nuclei/jastrow_factor_electron_electron_nuclei.py
-drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2021-06-16 17:02:50.758533 qmctorch-0.2.0/qmctorch/wavefunction/jastrows/elec_elec_nuclei/kernels/
--rw-rw-r--   0 nico      (1000) nico      (1000)      232 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/jastrows/elec_elec_nuclei/kernels/__init__.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     3095 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/jastrows/elec_elec_nuclei/kernels/boys_handy_jastrow_kernel.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     1438 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/jastrows/elec_elec_nuclei/kernels/fully_connected_jastrow_kernel.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     3127 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/jastrows/elec_elec_nuclei/kernels/jastrow_kernel_electron_electron_nuclei_base.py
-drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2021-06-16 17:02:50.758533 qmctorch-0.2.0/qmctorch/wavefunction/jastrows/elec_nuclei/
--rw-rw-r--   0 nico      (1000) nico      (1000)        0 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/jastrows/elec_nuclei/__init__.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     5188 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/jastrows/elec_nuclei/jastrow_factor_electron_nuclei.py
-drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2021-06-16 17:02:50.758533 qmctorch-0.2.0/qmctorch/wavefunction/jastrows/elec_nuclei/kernels/
--rw-rw-r--   0 nico      (1000) nico      (1000)      204 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/jastrows/elec_nuclei/kernels/__init__.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     1826 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/jastrows/elec_nuclei/kernels/fully_connected_jastrow_kernel.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     4636 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/jastrows/elec_nuclei/kernels/jastrow_kernel_electron_nuclei_base.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     3992 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/jastrows/elec_nuclei/kernels/pade_jastrow_kernel.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     8331 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/jastrows/jastrow_factor_combined_terms.py
-drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2021-06-16 17:02:50.758533 qmctorch-0.2.0/qmctorch/wavefunction/orbitals/
--rw-rw-r--   0 nico      (1000) nico      (1000)        0 2021-03-19 12:51:47.000000 qmctorch-0.2.0/qmctorch/wavefunction/orbitals/__init__.py
--rw-rw-r--   0 nico      (1000) nico      (1000)    23039 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/orbitals/atomic_orbitals.py
--rw-rw-r--   0 nico      (1000) nico      (1000)    12450 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/orbitals/atomic_orbitals_backflow.py
--rw-rw-r--   0 nico      (1000) nico      (1000)    12847 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/orbitals/atomic_orbitals_orbital_dependent_backflow.py
-drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2021-06-16 17:02:50.758533 qmctorch-0.2.0/qmctorch/wavefunction/orbitals/backflow/
--rw-rw-r--   0 nico      (1000) nico      (1000)        0 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/orbitals/backflow/__init__.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     8584 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/orbitals/backflow/backflow_transformation.py
-drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2021-06-16 17:02:50.758533 qmctorch-0.2.0/qmctorch/wavefunction/orbitals/backflow/kernels/
--rw-rw-r--   0 nico      (1000) nico      (1000)      377 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/orbitals/backflow/kernels/__init__.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     1085 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/orbitals/backflow/kernels/backflow_kernel_autodiff_inverse.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     3315 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/orbitals/backflow/kernels/backflow_kernel_base.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     1192 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/orbitals/backflow/kernels/backflow_kernel_fully_connected.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     2220 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/orbitals/backflow/kernels/backflow_kernel_inverse.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     1060 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/orbitals/backflow/kernels/backflow_kernel_power_sum.py
--rw-rw-r--   0 nico      (1000) nico      (1000)      756 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/orbitals/backflow/kernels/backflow_kernel_square.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     1767 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/orbitals/backflow/orbital_dependent_backflow_kernel.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     9184 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/orbitals/backflow/orbital_dependent_backflow_transformation.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     4722 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/orbitals/norm_orbital.py
--rw-rw-r--   0 nico      (1000) nico      (1000)    12843 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/orbitals/radial_functions.py
--rw-rw-r--   0 nico      (1000) nico      (1000)    20956 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/orbitals/spherical_harmonics.py
-drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2021-06-16 17:02:50.758533 qmctorch-0.2.0/qmctorch/wavefunction/pooling/
--rw-rw-r--   0 nico      (1000) nico      (1000)        0 2021-03-19 12:51:47.000000 qmctorch-0.2.0/qmctorch/wavefunction/pooling/__init__.py
--rw-rw-r--   0 nico      (1000) nico      (1000)    12258 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/pooling/orbital_configurations.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     5208 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/pooling/orbital_projector.py
--rw-rw-r--   0 nico      (1000) nico      (1000)    24519 2021-03-19 12:51:47.000000 qmctorch-0.2.0/qmctorch/wavefunction/pooling/slater_pooling.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     2799 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/slater_combined_jastrow.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     9477 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/slater_combined_jastrow_backflow.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     9042 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/slater_jastrow.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     8704 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/slater_jastrow_backflow.py
--rw-rw-r--   0 nico      (1000) nico      (1000)    12410 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/slater_jastrow_base.py
--rw-rw-r--   0 nico      (1000) nico      (1000)    11914 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/slater_orbital_dependent_jastrow.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     7969 2021-06-16 16:49:19.000000 qmctorch-0.2.0/qmctorch/wavefunction/wf_base.py
-drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2021-06-16 17:02:50.754533 qmctorch-0.2.0/qmctorch.egg-info/
--rw-rw-r--   0 nico      (1000) nico      (1000)     1972 2021-06-16 17:02:50.000000 qmctorch-0.2.0/qmctorch.egg-info/PKG-INFO
--rw-rw-r--   0 nico      (1000) nico      (1000)     7078 2021-06-16 17:02:50.000000 qmctorch-0.2.0/qmctorch.egg-info/SOURCES.txt
--rw-rw-r--   0 nico      (1000) nico      (1000)        1 2021-06-16 17:02:50.000000 qmctorch-0.2.0/qmctorch.egg-info/dependency_links.txt
--rw-rw-r--   0 nico      (1000) nico      (1000)        1 2021-03-19 12:59:49.000000 qmctorch-0.2.0/qmctorch.egg-info/not-zip-safe
--rw-rw-r--   0 nico      (1000) nico      (1000)      198 2021-06-16 17:02:50.000000 qmctorch-0.2.0/qmctorch.egg-info/requires.txt
--rw-rw-r--   0 nico      (1000) nico      (1000)       25 2021-06-16 17:02:50.000000 qmctorch-0.2.0/qmctorch.egg-info/top_level.txt
--rw-rw-r--   0 nico      (1000) nico      (1000)      294 2021-06-16 17:02:50.766533 qmctorch-0.2.0/setup.cfg
--rw-rw-r--   0 nico      (1000) nico      (1000)     1857 2021-06-16 17:01:33.000000 qmctorch-0.2.0/setup.py
-drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2021-06-16 17:02:50.762533 qmctorch-0.2.0/tests/
--rw-rw-r--   0 nico      (1000) nico      (1000)        0 2021-03-19 12:51:47.000000 qmctorch-0.2.0/tests/__init__.py
--rw-rw-r--   0 nico      (1000) nico      (1000)      284 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/path_utils.py
-drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2021-06-16 17:02:50.762533 qmctorch-0.2.0/tests/sampler/
--rw-rw-r--   0 nico      (1000) nico      (1000)        0 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/sampler/__init__.py
--rw-rw-r--   0 nico      (1000) nico      (1000)      498 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/sampler/test_generalized_metropolis.py
--rw-rw-r--   0 nico      (1000) nico      (1000)      502 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/sampler/test_hamiltonian.py
--rw-rw-r--   0 nico      (1000) nico      (1000)      693 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/sampler/test_metropolis.py
--rw-rw-r--   0 nico      (1000) nico      (1000)      589 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/sampler/test_sampler_base.py
--rw-rw-r--   0 nico      (1000) nico      (1000)      854 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/sampler/test_walker.py
-drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2021-06-16 17:02:50.762533 qmctorch-0.2.0/tests/scf/
--rw-rw-r--   0 nico      (1000) nico      (1000)        0 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/scf/__init__.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     1418 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/scf/test_gto2sto_fit.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     1513 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/scf/test_molecule.py
-drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2021-06-16 17:02:50.762533 qmctorch-0.2.0/tests/solver/
--rw-rw-r--   0 nico      (1000) nico      (1000)        0 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/solver/__init__.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     5565 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/solver/test_h2.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     2685 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/solver/test_h2_adf.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     2645 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/solver/test_h2_adf_jacobi.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     4397 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/solver/test_h2_correlated.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     2408 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/solver/test_h2_stats.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     2537 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/solver/test_lih.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     3021 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/solver/test_lih_adf_backflow.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     3070 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/solver/test_lih_correlated.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     2814 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/solver/test_lih_generic_jastrow.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     3066 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/solver/test_lih_pyscf_backflow.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     6523 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/solver/test_lih_pyscf_compare_backflow.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     3294 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/solver/test_lih_pyscf_generic_backflow.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     3065 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/solver/test_lih_pyscf_orbital_dependent_backflow.py
-drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2021-06-16 17:02:50.762533 qmctorch-0.2.0/tests/wavefunction/
--rw-rw-r--   0 nico      (1000) nico      (1000)        0 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/wavefunction/__init__.py
-drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2021-06-16 17:02:50.762533 qmctorch-0.2.0/tests/wavefunction/orbitals/
--rw-rw-r--   0 nico      (1000) nico      (1000)        0 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/wavefunction/orbitals/__init__.py
--rw-rw-r--   0 nico      (1000) nico      (1000)       87 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/wavefunction/orbitals/second_derivative.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     3700 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/wavefunction/orbitals/test_ao_derivatives_adf.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     4409 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/wavefunction/orbitals/test_ao_derivatives_pyscf.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     3165 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/wavefunction/orbitals/test_ao_values_adf.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     2277 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/wavefunction/orbitals/test_ao_values_pyscf.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     4041 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/wavefunction/orbitals/test_backflow_ao_derivatives_pyscf.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     4028 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/wavefunction/orbitals/test_cartesian_harmonics.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     5414 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/wavefunction/orbitals/test_cartesian_harmonics_adf.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     2941 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/wavefunction/orbitals/test_mo_values_adf.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     1522 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/wavefunction/orbitals/test_norm.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     4385 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/wavefunction/orbitals/test_orbital_dependent_backflow_ao_derivatives_pyscf.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     4997 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/wavefunction/orbitals/test_radial_functions.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     5822 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/wavefunction/orbitals/test_radial_gto.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     5918 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/wavefunction/orbitals/test_radial_sto.py
--rw-rw-r--   0 nico      (1000) nico      (1000)      797 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/wavefunction/orbitals/test_spherical_harmonics.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     4168 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/wavefunction/test_compare_slaterjastrow_backflow.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     4251 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/wavefunction/test_compare_slaterjastrow_orbital_dependent_backflow.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     7775 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/wavefunction/test_slater_orbital_dependent_jastrow.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     6416 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/wavefunction/test_slatercombinedjastrow.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     6331 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/wavefunction/test_slatercombinedjastrow_backflow.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     5389 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/wavefunction/test_slaterjastrow.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     5671 2021-06-16 17:00:51.000000 qmctorch-0.2.0/tests/wavefunction/test_slaterjastrow_backflow.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     6510 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/wavefunction/test_slaterjastrow_cas.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     2229 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/wavefunction/test_slaterjastrow_ee_cusp.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     5199 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/wavefunction/test_slaterjastrow_generic.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     5907 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests/wavefunction/test_slaterjastrow_orbital_dependent_backflow.py
-drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2021-06-16 17:02:50.766533 qmctorch-0.2.0/tests_hvd/
--rw-rw-r--   0 nico      (1000) nico      (1000)        0 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests_hvd/__init__.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     4339 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests_hvd/test_h2_hvd.py
--rw-rw-r--   0 nico      (1000) nico      (1000)      579 2021-06-16 16:49:20.000000 qmctorch-0.2.0/tests_hvd/test_hvd.py
+drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2023-04-26 15:00:54.613762 qmctorch-0.3.0/
+-rw-rw-r--   0 nico      (1000) nico      (1000)    11347 2023-04-20 12:42:06.000000 qmctorch-0.3.0/LICENSE
+-rw-rw-r--   0 nico      (1000) nico      (1000)       35 2023-04-20 12:42:06.000000 qmctorch-0.3.0/MANIFEST.in
+-rw-rw-r--   0 nico      (1000) nico      (1000)       55 2023-04-20 12:42:06.000000 qmctorch-0.3.0/NOTICE
+-rw-rw-r--   0 nico      (1000) nico      (1000)     1952 2023-04-26 15:00:54.613762 qmctorch-0.3.0/PKG-INFO
+-rw-rw-r--   0 nico      (1000) nico      (1000)     1156 2023-04-20 12:42:06.000000 qmctorch-0.3.0/README.md
+drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2023-04-26 15:00:54.593752 qmctorch-0.3.0/bin/
+-rwxrwxr-x   0 nico      (1000) nico      (1000)     1513 2023-04-26 14:58:28.000000 qmctorch-0.3.0/bin/qmctorch
+drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2023-04-26 15:00:54.593752 qmctorch-0.3.0/qmctorch/
+-rw-rw-r--   0 nico      (1000) nico      (1000)      534 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/__init__.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)       22 2023-04-26 14:58:29.000000 qmctorch-0.3.0/qmctorch/__version__.py
+drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2023-04-26 15:00:54.597754 qmctorch-0.3.0/qmctorch/sampler/
+-rw-rw-r--   0 nico      (1000) nico      (1000)      266 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/sampler/__init__.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     6404 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/sampler/generalized_metropolis.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     5325 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/sampler/hamiltonian.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     9684 2023-04-26 14:58:29.000000 qmctorch-0.3.0/qmctorch/sampler/metropolis.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     2158 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/sampler/sampler_base.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     4967 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/sampler/walkers.py
+drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2023-04-26 15:00:54.597754 qmctorch-0.3.0/qmctorch/scf/
+-rw-rw-r--   0 nico      (1000) nico      (1000)       55 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/scf/__init__.py
+drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2023-04-26 15:00:54.597754 qmctorch-0.3.0/qmctorch/scf/calculator/
+-rw-rw-r--   0 nico      (1000) nico      (1000)      216 2023-04-26 14:58:29.000000 qmctorch-0.3.0/qmctorch/scf/calculator/__init__.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     9192 2023-04-26 14:58:29.000000 qmctorch-0.3.0/qmctorch/scf/calculator/adf.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)      933 2023-04-26 14:58:29.000000 qmctorch-0.3.0/qmctorch/scf/calculator/calculator_base.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     5554 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/scf/calculator/pyscf.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)    13603 2023-04-26 14:58:29.000000 qmctorch-0.3.0/qmctorch/scf/molecule.py
+drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2023-04-26 15:00:54.597754 qmctorch-0.3.0/qmctorch/solver/
+-rw-rw-r--   0 nico      (1000) nico      (1000)      157 2023-04-26 14:58:29.000000 qmctorch-0.3.0/qmctorch/solver/__init__.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)    16306 2023-04-26 14:58:29.000000 qmctorch-0.3.0/qmctorch/solver/solver.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)    17118 2023-04-26 14:58:29.000000 qmctorch-0.3.0/qmctorch/solver/solver_base.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     9987 2023-04-26 14:58:29.000000 qmctorch-0.3.0/qmctorch/solver/solver_mpi.py
+drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2023-04-26 15:00:54.597754 qmctorch-0.3.0/qmctorch/utils/
+-rw-rw-r--   0 nico      (1000) nico      (1000)     1529 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/utils/__init__.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     1900 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/utils/algebra_utils.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)    12729 2023-04-26 14:58:29.000000 qmctorch-0.3.0/qmctorch/utils/hdf5_utils.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)    12151 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/utils/interpolate.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     7058 2023-04-26 14:58:29.000000 qmctorch-0.3.0/qmctorch/utils/plot_data.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     1770 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/utils/stat_utils.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     7569 2023-04-26 14:58:29.000000 qmctorch-0.3.0/qmctorch/utils/torch_utils.py
+drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2023-04-26 15:00:54.597754 qmctorch-0.3.0/qmctorch/wavefunction/
+-rw-rw-r--   0 nico      (1000) nico      (1000)      529 2023-04-26 14:58:29.000000 qmctorch-0.3.0/qmctorch/wavefunction/__init__.py
+drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2023-04-26 15:00:54.597754 qmctorch-0.3.0/qmctorch/wavefunction/jastrows/
+-rw-rw-r--   0 nico      (1000) nico      (1000)        0 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/jastrows/__init__.py
+drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2023-04-26 15:00:54.601756 qmctorch-0.3.0/qmctorch/wavefunction/jastrows/distance/
+-rw-rw-r--   0 nico      (1000) nico      (1000)      126 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/jastrows/distance/__init__.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     6572 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/jastrows/distance/electron_electron_distance.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     4932 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/jastrows/distance/electron_nuclei_distance.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     2072 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/jastrows/distance/scaling.py
+drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2023-04-26 15:00:54.601756 qmctorch-0.3.0/qmctorch/wavefunction/jastrows/elec_elec/
+-rw-rw-r--   0 nico      (1000) nico      (1000)        0 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/jastrows/elec_elec/__init__.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     9691 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/jastrows/elec_elec/jastrow_factor_electron_electron.py
+drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2023-04-26 15:00:54.601756 qmctorch-0.3.0/qmctorch/wavefunction/jastrows/elec_elec/kernels/
+-rw-rw-r--   0 nico      (1000) nico      (1000)      280 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/jastrows/elec_elec/kernels/__init__.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     3241 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/jastrows/elec_elec/kernels/fully_connected_jastrow_kernel.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     4499 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/jastrows/elec_elec/kernels/jastrow_kernel_electron_electron_base.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     4756 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/jastrows/elec_elec/kernels/pade_jastrow_kernel.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     9216 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/jastrows/elec_elec/kernels/pade_jastrow_polynomial_kernel.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     5158 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/jastrows/elec_elec/orbital_dependent_jastrow_kernel.py
+drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2023-04-26 15:00:54.601756 qmctorch-0.3.0/qmctorch/wavefunction/jastrows/elec_elec_nuclei/
+-rw-rw-r--   0 nico      (1000) nico      (1000)        0 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/jastrows/elec_elec_nuclei/__init__.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)    14483 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/jastrows/elec_elec_nuclei/jastrow_factor_electron_electron_nuclei.py
+drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2023-04-26 15:00:54.601756 qmctorch-0.3.0/qmctorch/wavefunction/jastrows/elec_elec_nuclei/kernels/
+-rw-rw-r--   0 nico      (1000) nico      (1000)      232 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/jastrows/elec_elec_nuclei/kernels/__init__.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     3095 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/jastrows/elec_elec_nuclei/kernels/boys_handy_jastrow_kernel.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     1438 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/jastrows/elec_elec_nuclei/kernels/fully_connected_jastrow_kernel.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     3127 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/jastrows/elec_elec_nuclei/kernels/jastrow_kernel_electron_electron_nuclei_base.py
+drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2023-04-26 15:00:54.601756 qmctorch-0.3.0/qmctorch/wavefunction/jastrows/elec_nuclei/
+-rw-rw-r--   0 nico      (1000) nico      (1000)        0 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/jastrows/elec_nuclei/__init__.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     5188 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/jastrows/elec_nuclei/jastrow_factor_electron_nuclei.py
+drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2023-04-26 15:00:54.601756 qmctorch-0.3.0/qmctorch/wavefunction/jastrows/elec_nuclei/kernels/
+-rw-rw-r--   0 nico      (1000) nico      (1000)      204 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/jastrows/elec_nuclei/kernels/__init__.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     1826 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/jastrows/elec_nuclei/kernels/fully_connected_jastrow_kernel.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     4636 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/jastrows/elec_nuclei/kernels/jastrow_kernel_electron_nuclei_base.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     3992 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/jastrows/elec_nuclei/kernels/pade_jastrow_kernel.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     8331 2023-04-25 09:27:11.000000 qmctorch-0.3.0/qmctorch/wavefunction/jastrows/jastrow_factor_combined_terms.py
+drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2023-04-26 15:00:54.601756 qmctorch-0.3.0/qmctorch/wavefunction/orbitals/
+-rw-rw-r--   0 nico      (1000) nico      (1000)        0 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/orbitals/__init__.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)    23039 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/orbitals/atomic_orbitals.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)    12450 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/orbitals/atomic_orbitals_backflow.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)    12847 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/orbitals/atomic_orbitals_orbital_dependent_backflow.py
+drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2023-04-26 15:00:54.605758 qmctorch-0.3.0/qmctorch/wavefunction/orbitals/backflow/
+-rw-rw-r--   0 nico      (1000) nico      (1000)        0 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/orbitals/backflow/__init__.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     8584 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/orbitals/backflow/backflow_transformation.py
+drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2023-04-26 15:00:54.605758 qmctorch-0.3.0/qmctorch/wavefunction/orbitals/backflow/kernels/
+-rw-rw-r--   0 nico      (1000) nico      (1000)      377 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/orbitals/backflow/kernels/__init__.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     1085 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/orbitals/backflow/kernels/backflow_kernel_autodiff_inverse.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     3315 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/orbitals/backflow/kernels/backflow_kernel_base.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     1192 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/orbitals/backflow/kernels/backflow_kernel_fully_connected.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     2220 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/orbitals/backflow/kernels/backflow_kernel_inverse.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     1060 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/orbitals/backflow/kernels/backflow_kernel_power_sum.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)      756 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/orbitals/backflow/kernels/backflow_kernel_square.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     1767 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/orbitals/backflow/orbital_dependent_backflow_kernel.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     9184 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/orbitals/backflow/orbital_dependent_backflow_transformation.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     4722 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/orbitals/norm_orbital.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)    12843 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/orbitals/radial_functions.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)    20956 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/orbitals/spherical_harmonics.py
+drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2023-04-26 15:00:54.605758 qmctorch-0.3.0/qmctorch/wavefunction/pooling/
+-rw-rw-r--   0 nico      (1000) nico      (1000)        0 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/pooling/__init__.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)    12258 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/pooling/orbital_configurations.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     5208 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/pooling/orbital_projector.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)    24519 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/pooling/slater_pooling.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     3950 2023-04-26 14:58:29.000000 qmctorch-0.3.0/qmctorch/wavefunction/slater_combined_jastrow.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)    11173 2023-04-26 14:58:29.000000 qmctorch-0.3.0/qmctorch/wavefunction/slater_combined_jastrow_backflow.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)    10041 2023-04-26 14:58:29.000000 qmctorch-0.3.0/qmctorch/wavefunction/slater_jastrow.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)    10232 2023-04-26 14:58:29.000000 qmctorch-0.3.0/qmctorch/wavefunction/slater_jastrow_backflow.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)    12710 2023-04-26 14:58:29.000000 qmctorch-0.3.0/qmctorch/wavefunction/slater_jastrow_base.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)    13080 2023-04-26 14:58:29.000000 qmctorch-0.3.0/qmctorch/wavefunction/slater_orbital_dependent_jastrow.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     7969 2023-04-20 12:42:06.000000 qmctorch-0.3.0/qmctorch/wavefunction/wf_base.py
+drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2023-04-26 15:00:54.593752 qmctorch-0.3.0/qmctorch.egg-info/
+-rw-rw-r--   0 nico      (1000) nico      (1000)     1952 2023-04-26 15:00:54.000000 qmctorch-0.3.0/qmctorch.egg-info/PKG-INFO
+-rw-rw-r--   0 nico      (1000) nico      (1000)     7044 2023-04-26 15:00:54.000000 qmctorch-0.3.0/qmctorch.egg-info/SOURCES.txt
+-rw-rw-r--   0 nico      (1000) nico      (1000)        1 2023-04-26 15:00:54.000000 qmctorch-0.3.0/qmctorch.egg-info/dependency_links.txt
+-rw-rw-r--   0 nico      (1000) nico      (1000)        1 2023-04-20 13:02:50.000000 qmctorch-0.3.0/qmctorch.egg-info/not-zip-safe
+-rw-rw-r--   0 nico      (1000) nico      (1000)      215 2023-04-26 15:00:54.000000 qmctorch-0.3.0/qmctorch.egg-info/requires.txt
+-rw-rw-r--   0 nico      (1000) nico      (1000)       25 2023-04-26 15:00:54.000000 qmctorch-0.3.0/qmctorch.egg-info/top_level.txt
+-rw-rw-r--   0 nico      (1000) nico      (1000)      294 2023-04-26 15:00:54.613762 qmctorch-0.3.0/setup.cfg
+-rw-rw-r--   0 nico      (1000) nico      (1000)     1779 2023-04-26 14:58:29.000000 qmctorch-0.3.0/setup.py
+drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2023-04-26 15:00:54.605758 qmctorch-0.3.0/tests/
+-rw-rw-r--   0 nico      (1000) nico      (1000)        0 2023-04-20 12:42:06.000000 qmctorch-0.3.0/tests/__init__.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)      284 2023-04-20 12:42:06.000000 qmctorch-0.3.0/tests/path_utils.py
+drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2023-04-26 15:00:54.605758 qmctorch-0.3.0/tests/sampler/
+-rw-rw-r--   0 nico      (1000) nico      (1000)        0 2023-04-20 12:42:06.000000 qmctorch-0.3.0/tests/sampler/__init__.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)      498 2023-04-20 12:42:06.000000 qmctorch-0.3.0/tests/sampler/test_generalized_metropolis.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)      502 2023-04-20 12:42:06.000000 qmctorch-0.3.0/tests/sampler/test_hamiltonian.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)      693 2023-04-20 12:42:06.000000 qmctorch-0.3.0/tests/sampler/test_metropolis.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)      589 2023-04-20 12:42:06.000000 qmctorch-0.3.0/tests/sampler/test_sampler_base.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)      854 2023-04-20 12:42:06.000000 qmctorch-0.3.0/tests/sampler/test_walker.py
+drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2023-04-26 15:00:54.605758 qmctorch-0.3.0/tests/scf/
+-rw-rw-r--   0 nico      (1000) nico      (1000)        0 2023-04-20 12:42:06.000000 qmctorch-0.3.0/tests/scf/__init__.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     1418 2023-04-20 12:42:06.000000 qmctorch-0.3.0/tests/scf/test_gto2sto_fit.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     1513 2023-04-20 12:42:06.000000 qmctorch-0.3.0/tests/scf/test_molecule.py
+drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2023-04-26 15:00:54.609760 qmctorch-0.3.0/tests/solver/
+-rw-rw-r--   0 nico      (1000) nico      (1000)        0 2023-04-20 12:42:06.000000 qmctorch-0.3.0/tests/solver/__init__.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     5539 2023-04-26 14:58:29.000000 qmctorch-0.3.0/tests/solver/test_h2.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     2659 2023-04-26 14:58:29.000000 qmctorch-0.3.0/tests/solver/test_h2_adf.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     2619 2023-04-26 14:58:29.000000 qmctorch-0.3.0/tests/solver/test_h2_adf_jacobi.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     4371 2023-04-26 14:58:29.000000 qmctorch-0.3.0/tests/solver/test_h2_correlated.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     2382 2023-04-26 14:58:29.000000 qmctorch-0.3.0/tests/solver/test_h2_stats.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     2511 2023-04-26 14:58:29.000000 qmctorch-0.3.0/tests/solver/test_lih.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     2995 2023-04-26 14:58:29.000000 qmctorch-0.3.0/tests/solver/test_lih_adf_backflow.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     3044 2023-04-26 14:58:29.000000 qmctorch-0.3.0/tests/solver/test_lih_correlated.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     2788 2023-04-26 14:58:29.000000 qmctorch-0.3.0/tests/solver/test_lih_generic_jastrow.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     3040 2023-04-26 14:58:29.000000 qmctorch-0.3.0/tests/solver/test_lih_pyscf_backflow.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     6484 2023-04-26 14:58:29.000000 qmctorch-0.3.0/tests/solver/test_lih_pyscf_compare_backflow.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     3268 2023-04-26 14:58:29.000000 qmctorch-0.3.0/tests/solver/test_lih_pyscf_generic_backflow.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     3039 2023-04-26 14:58:29.000000 qmctorch-0.3.0/tests/solver/test_lih_pyscf_orbital_dependent_backflow.py
+drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2023-04-26 15:00:54.609760 qmctorch-0.3.0/tests/wavefunction/
+-rw-rw-r--   0 nico      (1000) nico      (1000)        0 2023-04-20 12:42:06.000000 qmctorch-0.3.0/tests/wavefunction/__init__.py
+drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2023-04-26 15:00:54.613762 qmctorch-0.3.0/tests/wavefunction/orbitals/
+-rw-rw-r--   0 nico      (1000) nico      (1000)        0 2023-04-20 12:42:06.000000 qmctorch-0.3.0/tests/wavefunction/orbitals/__init__.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)       87 2023-04-20 12:42:06.000000 qmctorch-0.3.0/tests/wavefunction/orbitals/second_derivative.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     3700 2023-04-20 12:42:06.000000 qmctorch-0.3.0/tests/wavefunction/orbitals/test_ao_derivatives_adf.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     4409 2023-04-20 12:42:06.000000 qmctorch-0.3.0/tests/wavefunction/orbitals/test_ao_derivatives_pyscf.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     3165 2023-04-20 12:42:06.000000 qmctorch-0.3.0/tests/wavefunction/orbitals/test_ao_values_adf.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     2277 2023-04-20 12:42:06.000000 qmctorch-0.3.0/tests/wavefunction/orbitals/test_ao_values_pyscf.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     4041 2023-04-20 12:42:06.000000 qmctorch-0.3.0/tests/wavefunction/orbitals/test_backflow_ao_derivatives_pyscf.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     4028 2023-04-20 12:42:06.000000 qmctorch-0.3.0/tests/wavefunction/orbitals/test_cartesian_harmonics.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     5414 2023-04-20 12:42:06.000000 qmctorch-0.3.0/tests/wavefunction/orbitals/test_cartesian_harmonics_adf.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     2941 2023-04-20 12:42:06.000000 qmctorch-0.3.0/tests/wavefunction/orbitals/test_mo_values_adf.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     1522 2023-04-20 12:42:06.000000 qmctorch-0.3.0/tests/wavefunction/orbitals/test_norm.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     4385 2023-04-20 12:42:06.000000 qmctorch-0.3.0/tests/wavefunction/orbitals/test_orbital_dependent_backflow_ao_derivatives_pyscf.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     4997 2023-04-20 12:42:06.000000 qmctorch-0.3.0/tests/wavefunction/orbitals/test_radial_functions.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     5822 2023-04-20 12:42:06.000000 qmctorch-0.3.0/tests/wavefunction/orbitals/test_radial_gto.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     5918 2023-04-20 12:42:06.000000 qmctorch-0.3.0/tests/wavefunction/orbitals/test_radial_sto.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)      797 2023-04-20 12:42:06.000000 qmctorch-0.3.0/tests/wavefunction/orbitals/test_spherical_harmonics.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     4168 2023-04-20 12:42:06.000000 qmctorch-0.3.0/tests/wavefunction/test_compare_slaterjastrow_backflow.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     4251 2023-04-20 12:42:06.000000 qmctorch-0.3.0/tests/wavefunction/test_compare_slaterjastrow_orbital_dependent_backflow.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     7775 2023-04-20 12:42:06.000000 qmctorch-0.3.0/tests/wavefunction/test_slater_orbital_dependent_jastrow.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     6416 2023-04-26 14:58:29.000000 qmctorch-0.3.0/tests/wavefunction/test_slatercombinedjastrow.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     6331 2023-04-26 14:58:29.000000 qmctorch-0.3.0/tests/wavefunction/test_slatercombinedjastrow_backflow.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     5389 2023-04-20 12:42:06.000000 qmctorch-0.3.0/tests/wavefunction/test_slaterjastrow.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     5671 2023-04-20 12:42:06.000000 qmctorch-0.3.0/tests/wavefunction/test_slaterjastrow_backflow.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     6510 2023-04-20 12:42:06.000000 qmctorch-0.3.0/tests/wavefunction/test_slaterjastrow_cas.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     2229 2023-04-20 12:42:06.000000 qmctorch-0.3.0/tests/wavefunction/test_slaterjastrow_ee_cusp.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     5199 2023-04-20 12:42:06.000000 qmctorch-0.3.0/tests/wavefunction/test_slaterjastrow_generic.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     5907 2023-04-20 12:42:06.000000 qmctorch-0.3.0/tests/wavefunction/test_slaterjastrow_orbital_dependent_backflow.py
+drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2023-04-26 15:00:54.613762 qmctorch-0.3.0/tests_hvd/
+-rw-rw-r--   0 nico      (1000) nico      (1000)        0 2023-04-20 12:42:06.000000 qmctorch-0.3.0/tests_hvd/__init__.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     4305 2023-04-26 14:58:29.000000 qmctorch-0.3.0/tests_hvd/test_h2_hvd.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)      579 2023-04-20 12:42:06.000000 qmctorch-0.3.0/tests_hvd/test_hvd.py
```

### Comparing `qmctorch-0.2.0/LICENSE` & `qmctorch-0.3.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [yyy] [name of copyright owner]
+   Copyright 2022 Nicolas Renaud
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `qmctorch-0.2.0/PKG-INFO` & `qmctorch-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: qmctorch
-Version: 0.2.0
+Version: 0.3.0
 Summary: Pytorch Implementation of Quantum Monte Carlo
 Home-page: https://github.com/NLESC-JCER/QMCTorch
 Author: ['Nicolas Renaud', 'Felipe Zapata']
 Author-email: n.renaud@esciencecenter.nl
 License: Apache Software License 2.0
 Keywords: qmctorch
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering :: Chemistry
@@ -42,9 +41,7 @@
 https://qmctorch.readthedocs.io/en/latest/intro.html
 
 
 ## Disclaimer
 QMCTorch is currently under developmement and most likely won't behave as expected 
 
 
-
-
```

### Comparing `qmctorch-0.2.0/README.md` & `qmctorch-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/bin/qmctorch` & `qmctorch-0.3.0/bin/qmctorch`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 import os
 import argparse
 
 
-dist_solvers = ['SolverSlaterJastrowHorovod']
+dist_solvers = ['SolverMPI']
 
 
 def check_file(fname):
     """Check if any distributed solver is imported."""
 
     with open(fname, 'r') as f:
         data = f.readlines()
```

### Comparing `qmctorch-0.2.0/qmctorch/__init__.py` & `qmctorch-0.3.0/qmctorch/__init__.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/sampler/generalized_metropolis.py` & `qmctorch-0.3.0/qmctorch/sampler/generalized_metropolis.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/sampler/hamiltonian.py` & `qmctorch-0.3.0/qmctorch/sampler/hamiltonian.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/sampler/metropolis.py` & `qmctorch-0.3.0/qmctorch/sampler/metropolis.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,26 +23,26 @@
         """Metropolis Hasting generator
 
         Args:
             nwalkers (int, optional): Number of walkers. Defaults to 100.
             nstep (int, optional): Number of steps. Defaults to 1000.
             step_size (int, optional): length of the step. Defaults to 0.2.
             nelec (int, optional): total number of electrons. Defaults to 1.
-            ntherm (int, optional): number of mc step to thermalize. Defaults to -1, i.e. keep ponly last position
+            ntherm (int, optional): number of mc step to thermalize. Defaults to -1, i.e. keep only the last position
             ndecor (int, optional): number of mc step for decorelation. Defauts to 1.
             ndim (int, optional): total number of dimension. Defaults to 3.
             init (dict, optional): method to init the positions of the walkers. See Molecule.domain()
 
             move (dict, optional): method to move the electrons. default('all-elec','normal') \n
                                    'type':
                                         'one-elec': move a single electron per iteration \n
                                         'all-elec': move all electrons at the same time \n
                                         'all-elec-iter': move all electrons by iterating through single elec moves \n
                                     'proba' :
-                                        'uniform': uniform ina cube \n
+                                        'uniform': uniform in a cube \n
                                         'normal': gussian in a sphere \n
             cuda (bool, optional): turn CUDA ON/OFF. Defaults to False.
 
 
         Examples::
             >>> mol = Molecule('h2.xyz')
             >>> wf = SlaterJastrow(mol)
```

### Comparing `qmctorch-0.2.0/qmctorch/sampler/sampler_base.py` & `qmctorch-0.3.0/qmctorch/sampler/sampler_base.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/sampler/walkers.py` & `qmctorch-0.3.0/qmctorch/sampler/walkers.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/scf/calculator/calculator_base.py` & `qmctorch-0.3.0/qmctorch/scf/calculator/calculator_base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from types import SimpleNamespace
-
 import numpy as np
 
 
 class CalculatorBase:
     def __init__(self, atoms, atom_coords, basis, scf, units, molname, calcname, savefile):
 
         self.atoms = atoms
```

### Comparing `qmctorch-0.2.0/qmctorch/scf/calculator/pyscf.py` & `qmctorch-0.3.0/qmctorch/scf/calculator/pyscf.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/scf/molecule.py` & `qmctorch-0.3.0/qmctorch/scf/molecule.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,49 @@
 import os
 import math
 import numpy as np
 from mendeleev import element
 from types import SimpleNamespace
-from mpi4py import MPI
 import h5py
-
-from .calculator.adf import CalculatorADF
-from .calculator.pyscf import CalculatorPySCF
+from mpi4py import MPI
+from .calculator import CalculatorADF, CalculatorPySCF, CalculatorADF2019
 
 from ..utils import dump_to_hdf5, load_from_hdf5, bytes2str
 from .. import log
 
 
 class Molecule:
 
-    def __init__(self, atom=None, calculator='adf',
-                 scf='hf', basis='dzp', unit='bohr',
+    def __init__(self, atom=None, calculator='pyscf',
+                 scf='hf', basis='sto-3g', unit='bohr',
                  name=None, load=None, save_scf_file=False,
                  redo_scf=False, rank=0):
         """Create a molecule in QMCTorch
 
         Args:
             atom (str or None, optional): defines the atoms and their positions. Defaults to None.
+                - At1 x y z; At2 x y z ... : Provide the atomic coordinate directly
+                - <file>.xyz : provide the path to an .xyz file containing the atomic coordinates 
             calculator (str, optional): selet scf calculator. Defaults to 'adf'.
+                - pyscf : PySCF calculator
+                - adf : ADF2020+ calculator
+                - adf2019 : ADF2019 calculatori
             scf (str, optional): select scf level of theory. Defaults to 'hf'.
+                - hf : perform a Hatree-Fock calculation to obtain the molecular orbital coefficients
+                - dft : perform a density functional theory using the local density approximation
             basis (str, optional): select the basis set. Defaults to 'dzp'.
-            unit (str, optional): units of the coordinates. Defaults to 'bohr'.
+            unit (str, optional): units of the coordinates; 'bohr' or 'angs'. Defaults to 'bohr'.
             name (str or None, optional): name of the molecule. Defaults to None.
             load (str or None, optional): path to a hdf5 file to load. Defaults to None.
             save_scf_file (bool, optional): save the scf file (when applicable) Defaults to False
             redo_scf (bool, optional): if true ignore existing hdf5 file and redo the scf calculation
             rank (int, optional): Rank of the process. Defaults to 0.
 
         Examples:
-            >>> from qmctorch.wavefunction import Molecule
+            >>> from qmctorch.scf import Molecule
             >>> mol = Molecule(atom='H 0 0 0; H 0 0 1', unit='angs',
             ...                calculator='adf', basis='dzp')
         """
 
         self.atom_coords = []
         self.atomic_nelec = []
         self.atomic_number = []
@@ -95,15 +100,16 @@
                              file=self.hdf5file)
                     self.basis = self._load_basis()
 
                 # perform the scf calculation
                 else:
                     log.info('  Running scf  calculation')
 
-                    calc = {'adf': CalculatorADF,
+                    calc = {'adf2019': CalculatorADF2019,
+                            'adf': CalculatorADF,
                             'pyscf': CalculatorPySCF}[calculator]
 
                     self.calculator = calc(self.atoms,
                                            self.atom_coords,
                                            basis,
                                            self.scf_level,
                                            self.unit,
```

### Comparing `qmctorch-0.2.0/qmctorch/solver/solver_base.py` & `qmctorch-0.3.0/qmctorch/solver/solver_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,21 +196,23 @@
 
             # store any other defined method
             elif hasattr(self.wf, obs):
                 func = self.wf.__getattribute__(obs)
                 data = func(pos)
                 if isinstance(data, torch.Tensor):
                     data = data.cpu().detach().numpy()
-                    if (ibatch is None) or (ibatch == 0):
-                        self.observable.__getattribute__(
-                            obs).append(data)
-                    else:
-                        self.observable.__getattribute__(
-                            obs)[-1] = np.append(self.observable.__getattribute__(
-                                obs)[-1], data)
+                if isinstance(data, list):
+                    data = np.array(data)
+                if (ibatch is None) or (ibatch == 0):
+                    self.observable.__getattribute__(
+                        obs).append(data)
+                else:
+                    self.observable.__getattribute__(
+                        obs)[-1] = np.append(self.observable.__getattribute__(
+                            obs)[-1], data)
 
     def print_observable(self, cumulative_loss, verbose=False):
         """Print the observalbe to csreen
 
         Args:
             cumulative_loss (float): current loss value
             verbose (bool, optional): print all the observables. Defaults to False
@@ -450,15 +452,15 @@
             f.write('\n')
         f.close()
 
     def run(self, nepoch, batchsize=None, loss='variance'):
         raise NotImplementedError()
 
     def log_data(self):
-        """Log basi information about the sampler."""
+        """Log basic information about the sampler."""
 
         log.info('')
         log.info(' QMC Solver ')
 
         if self.wf is not None:
             log.info(
                 '  WaveFunction        : {0}', self.wf.__class__.__name__)
```

### Comparing `qmctorch-0.2.0/qmctorch/solver/solver_slater_jastrow.py` & `qmctorch-0.3.0/qmctorch/solver/solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
                             OrthoReg, add_group_attr,
                             dump_to_hdf5)
 
 from .. import log
 from .solver_base import SolverBase
 
 
-class SolverSlaterJastrow(SolverBase):
+class Solver(SolverBase):
 
     def __init__(self, wf=None, sampler=None, optimizer=None,
                  scheduler=None, output=None, rank=0):
         """Basic QMC solver
 
         Args:
             wf (qmctorch.WaveFunction, optional): wave function. Defaults to None.
@@ -387,15 +387,15 @@
         # compute local gradients
         self.opt.zero_grad()
         loss.backward()
 
         return loss, eloc
 
     def evaluate_grad_manual(self, lpos):
-        """Evaluate the gradient using low variance express
+        """Evaluate the gradient using low variance expression
 
         Args:
             lpos ([type]): [description]
 
         Args:
             lpos (torch.tensor): sampling points
 
@@ -409,17 +409,17 @@
             no_grad_eloc = False
 
         if self.wf.jastrow.requires_autograd:
             no_grad_eloc = False
 
         if self.loss.method in ['energy', 'weighted-energy']:
 
-            ''' Get the gradient of the total energy
-            dE/dk = < (dpsi/dk)/psi (E_L - <E_L >) >
-            '''
+            # Get the gradient of the total energy
+            # dE/dk = < (dpsi/dk)/psi (E_L - <E_L >) >
+            
 
             # compute local energy and wf values
             _, eloc = self.loss(lpos, no_grad=no_grad_eloc)
             psi = self.wf(lpos)
             norm = 1. / len(psi)
 
             # evaluate the prefactor of the grads
```

### Comparing `qmctorch-0.2.0/qmctorch/solver/solver_slater_jastrow_horovod.py` & `qmctorch-0.3.0/qmctorch/solver/solver_mpi.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 import torch
 from torch.utils.data import DataLoader
 
 from qmctorch.utils import (DataSet, Loss, OrthoReg, add_group_attr,
                             dump_to_hdf5)
 
 from .. import log
-from .solver_slater_jastrow import SolverSlaterJastrow
+from .solver import Solver
 
 try:
     import horovod.torch as hvd
 except ModuleNotFoundError:
     pass
 
 
 def logd(rank, *args):
     if rank == 0:
         log.info(*args)
 
 
-class SolverSlaterJastrowHorovod(SolverSlaterJastrow):
+class SolverMPI(Solver):
 
     def __init__(self, wf=None, sampler=None, optimizer=None,
                  scheduler=None, output=None, rank=0):
         """Distributed QMC solver
 
         Args:
             wf (qmctorch.WaveFunction, optional): wave function. Defaults to None.
```

### Comparing `qmctorch-0.2.0/qmctorch/utils/__init__.py` & `qmctorch-0.3.0/qmctorch/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/utils/algebra_utils.py` & `qmctorch-0.3.0/qmctorch/utils/algebra_utils.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/utils/hdf5_utils.py` & `qmctorch-0.3.0/qmctorch/utils/hdf5_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 import numpy as np
 import torch
 
 from .. import log
 
 
 def print_insert_error(obj, obj_name):
+    print(obj_name, obj)
     log.critical('Issue inserting data {0} of type {type}',
                  obj_name, type=str(type(obj)))
 
 
 def print_insert_type_error(obj, obj_name):
     log.critical('Issue inserting type of data {0}} ({type}})' %
                  obj_name, type=str(type(obj)))
-
-
+    
 def print_load_error(grp):
     log.critical('Issue loading {grp}', grp=grp)
 
 
 def load_from_hdf5(obj, fname, obj_name):
     """Load the content of an hdf5 file in an object.
 
@@ -205,14 +205,15 @@
             for child_name in get_children_names(obj):
                 child_obj = get_child_object(obj, child_name)
                 insert_object(child_obj,  own_grp, child_name)
 
         except Exception as inst:
             print(type(inst))
             print(inst)
+            
             print_insert_error(obj, obj_name)
 
     # if something went wrong anyway
     else:
         log.critical(
             ' Warning : Object {obj} already exists in {parent}', obj=obj_name, parent=parent_grp)
         log.critical(
@@ -243,15 +244,16 @@
         insert_fn = lookup_insert[type(obj)]
     except KeyError:
         insert_fn = insert_default
 
     try:
         insert_fn(obj, parent_grp, obj_name)
         # insert_type(obj, parent_grp, obj_name)
-    except:
+    except Exception as expt_message:
+        print(expt_message)
         print_insert_error(obj, obj_name)
 
 
 def insert_type(obj, parent_grp, obj_name):
     """Insert the content of the type object in an attribute
 
     Arguments:
@@ -284,18 +286,21 @@
     """funtion to insert a list as a dataset
 
     Arguments:
         obj {object} -- object to save
         parent_grp {hdf5 group} -- group where to dump
         obj_name {str} -- name of the object
     """
-    np.warnings.filterwarnings(
-        'ignore', category=np.VisibleDeprecationWarning)
+
+    
     try:
-        parent_grp.create_dataset(obj_name, data=obj)
+        if np.all([isinstance(el,torch.Tensor) for el in obj]):
+            obj = [el.numpy() for el in obj]
+            
+        parent_grp.create_dataset(obj_name, data=np.array(obj))
     except:
         for il, l in enumerate(obj):
             try:
                 insert_object(l, parent_grp, obj_name+'_'+str(il))
             except:
                 print_insert_error(obj, obj_name)
```

### Comparing `qmctorch-0.2.0/qmctorch/utils/interpolate.py` & `qmctorch-0.3.0/qmctorch/utils/interpolate.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/utils/plot_data.py` & `qmctorch-0.3.0/qmctorch/utils/plot_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -54,61 +54,51 @@
         obs_dict (SimpleNamespace): namespace of observable
         obsname (str): name (key) of the desired observable
     """
 
     fig = plt.figure()
     ax = fig.add_subplot(111)
 
-    data = np.array(observable.models.best[obsname]).flatten()
+    data = np.array(observable.__dict__[obsname]).squeeze()
     epoch = np.arange(len(data))
     ax.plot(epoch, data, color='#144477')
 
-    if obsname + '.grad' in observable.__dict__.keys():
-        data = np.array(observable.__getattribute__(
-            obsname + '.grad')).flatten()
-        ax2 = ax.twinx()
-        ax2.plot(epoch, data, color='blue')
-        ax2.set_ylabel('gradient', color='blue')
-        ax2.tick_params(axis='y', labelcolor='blue')
-
     plt.show()
 
 
 def plot_walkers_traj(eloc, walkers='mean'):
     """Plot the trajectory of all the individual walkers
 
     Args:
         obs (SimpleNamespace): Namespace of the observables
         walkers (int, str, optional): all, mean or index of a given walker Defaults to 'all'
     """
     nstep, nwalkers = eloc.shape
-
     celoc = np.cumsum(eloc, axis=0).T
     celoc /= np.arange(1, nstep + 1)
 
-    var_decor = np.sqrt(np.var(np.mean(celoc, axis=1)))
-    var = np.sqrt(np.var(celoc, axis=1) / (nstep - 1))
-
     if walkers is not None:
-        # plt.subplot(1, 2, 1)
 
         if walkers == 'all':
             plt.plot(eloc, 'o', alpha=1 / nwalkers, c='grey')
             cmap = cm.hot(np.linspace(0, 1, nwalkers))
             for i in range(nwalkers):
                 plt.plot(celoc.T[:, i], color=cmap[i])
 
         elif walkers == 'mean':
             plt.plot(eloc, 'o', alpha=1 / nwalkers, c='grey')
-            plt.plot(np.mean(celoc.T, axis=1), linewidth=5)
-
+            emean = np.mean(celoc.T, axis=1)
+            emin = emean.min()
+            emax = emean.max()
+            delta = emax-emin
+            plt.plot(emean, linewidth=5)
+            plt.ylim(emin-0.25*delta,emax+0.25*delta)
         else:
-            plt.plot(eloc[walkers, :], 'o',
-                     alpha=1 / nwalkers, c='grey')
-            plt.plot(celoc.T[traj_index, :])
+            raise ValueError('walkers argument must be all or mean')
+        
         plt.grid()
         plt.xlabel('Monte Carlo Steps')
         plt.ylabel('Energy (Hartree)')
 
     plt.show()
```

### Comparing `qmctorch-0.2.0/qmctorch/utils/stat_utils.py` & `qmctorch-0.3.0/qmctorch/utils/stat_utils.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/utils/torch_utils.py` & `qmctorch-0.3.0/qmctorch/utils/torch_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import torch
 from torch import nn
-from torch.autograd import grad
+from torch.autograd import grad, Variable
 from torch.utils.data import Dataset
 
 
 def set_torch_double_precision():
     """Set the default precision to double for all torch tensors."""
     torch.set_default_dtype = torch.float64
     torch.set_default_tensor_type(torch.DoubleTensor)
@@ -131,23 +131,22 @@
 
 class Loss(nn.Module):
 
     def __init__(
             self,
             wf,
             method='energy',
-            clip=False,
-            no_weight=False):
+            clip=False):
         """Defines the loss to use during the optimization
 
         Arguments:
             wf {WaveFunction} -- wave function object used
 
         Keyword Arguments:
-            method {str} -- method to use  (default: {'variance'})
+            method {str} -- method to use  (default: {'energy'})
                             (energy, variance, weighted-energy,
                             weighted-variance)
             clip {bool} -- clip the values that are +/- % sigma away from
                            the mean (default: {False})
         """
 
         super(Loss, self).__init__()
@@ -192,15 +191,15 @@
             # compute local eneergies
             local_energies = self.wf.local_energy(pos)
 
             # mask the energies if necessary
             mask = self.get_clipping_mask(local_energies)
 
             # sampling_weight
-            weight = self.get_sampling_weights(deactivate_weight)
+            weight = self.get_sampling_weights(pos, deactivate_weight)
 
             # compute the loss
             loss = self.loss_fn((weight * local_energies)[mask])
 
         return loss, local_energies
 
     @staticmethod
@@ -229,15 +228,15 @@
                 local_energies > emin)
         else:
             mask = torch.ones_like(
                 local_energies).type(torch.bool)
 
         return mask
 
-    def get_sampling_weights(self, deactivate_weight):
+    def get_sampling_weights(self, pos, deactivate_weight):
         """Get the weight needed when resampling is not
             done at every step
         """
 
         local_use_weight = self.use_weight * \
             (not deactivate_weight)
```

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/jastrows/distance/electron_electron_distance.py` & `qmctorch-0.3.0/qmctorch/wavefunction/jastrows/distance/electron_electron_distance.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/jastrows/distance/electron_nuclei_distance.py` & `qmctorch-0.3.0/qmctorch/wavefunction/jastrows/distance/electron_nuclei_distance.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/jastrows/distance/scaling.py` & `qmctorch-0.3.0/qmctorch/wavefunction/jastrows/distance/scaling.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/jastrows/elec_elec/jastrow_factor_electron_electron.py` & `qmctorch-0.3.0/qmctorch/wavefunction/jastrows/elec_elec/jastrow_factor_electron_electron.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/jastrows/elec_elec/kernels/fully_connected_jastrow_kernel.py` & `qmctorch-0.3.0/qmctorch/wavefunction/jastrows/elec_elec/kernels/fully_connected_jastrow_kernel.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/jastrows/elec_elec/kernels/jastrow_kernel_electron_electron_base.py` & `qmctorch-0.3.0/qmctorch/wavefunction/jastrows/elec_elec/kernels/jastrow_kernel_electron_electron_base.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/jastrows/elec_elec/kernels/pade_jastrow_kernel.py` & `qmctorch-0.3.0/qmctorch/wavefunction/jastrows/elec_elec/kernels/pade_jastrow_kernel.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/jastrows/elec_elec/kernels/pade_jastrow_polynomial_kernel.py` & `qmctorch-0.3.0/qmctorch/wavefunction/jastrows/elec_elec/kernels/pade_jastrow_polynomial_kernel.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/jastrows/elec_elec/orbital_dependent_jastrow_kernel.py` & `qmctorch-0.3.0/qmctorch/wavefunction/jastrows/elec_elec/orbital_dependent_jastrow_kernel.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/jastrows/elec_elec_nuclei/jastrow_factor_electron_electron_nuclei.py` & `qmctorch-0.3.0/qmctorch/wavefunction/jastrows/elec_elec_nuclei/jastrow_factor_electron_electron_nuclei.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/jastrows/elec_elec_nuclei/kernels/boys_handy_jastrow_kernel.py` & `qmctorch-0.3.0/qmctorch/wavefunction/jastrows/elec_elec_nuclei/kernels/boys_handy_jastrow_kernel.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/jastrows/elec_elec_nuclei/kernels/fully_connected_jastrow_kernel.py` & `qmctorch-0.3.0/qmctorch/wavefunction/jastrows/elec_elec_nuclei/kernels/fully_connected_jastrow_kernel.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/jastrows/elec_elec_nuclei/kernels/jastrow_kernel_electron_electron_nuclei_base.py` & `qmctorch-0.3.0/qmctorch/wavefunction/jastrows/elec_elec_nuclei/kernels/jastrow_kernel_electron_electron_nuclei_base.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/jastrows/elec_nuclei/jastrow_factor_electron_nuclei.py` & `qmctorch-0.3.0/qmctorch/wavefunction/jastrows/elec_nuclei/jastrow_factor_electron_nuclei.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/jastrows/elec_nuclei/kernels/fully_connected_jastrow_kernel.py` & `qmctorch-0.3.0/qmctorch/wavefunction/jastrows/elec_nuclei/kernels/fully_connected_jastrow_kernel.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/jastrows/elec_nuclei/kernels/jastrow_kernel_electron_nuclei_base.py` & `qmctorch-0.3.0/qmctorch/wavefunction/jastrows/elec_nuclei/kernels/jastrow_kernel_electron_nuclei_base.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/jastrows/elec_nuclei/kernels/pade_jastrow_kernel.py` & `qmctorch-0.3.0/qmctorch/wavefunction/jastrows/elec_nuclei/kernels/pade_jastrow_kernel.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/jastrows/jastrow_factor_combined_terms.py` & `qmctorch-0.3.0/qmctorch/wavefunction/jastrows/jastrow_factor_combined_terms.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/orbitals/atomic_orbitals.py` & `qmctorch-0.3.0/qmctorch/wavefunction/orbitals/atomic_orbitals.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/orbitals/atomic_orbitals_backflow.py` & `qmctorch-0.3.0/qmctorch/wavefunction/orbitals/atomic_orbitals_backflow.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/orbitals/atomic_orbitals_orbital_dependent_backflow.py` & `qmctorch-0.3.0/qmctorch/wavefunction/orbitals/atomic_orbitals_orbital_dependent_backflow.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/orbitals/backflow/backflow_transformation.py` & `qmctorch-0.3.0/qmctorch/wavefunction/orbitals/backflow/backflow_transformation.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/orbitals/backflow/kernels/backflow_kernel_autodiff_inverse.py` & `qmctorch-0.3.0/qmctorch/wavefunction/orbitals/backflow/kernels/backflow_kernel_autodiff_inverse.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/orbitals/backflow/kernels/backflow_kernel_base.py` & `qmctorch-0.3.0/qmctorch/wavefunction/orbitals/backflow/kernels/backflow_kernel_base.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/orbitals/backflow/kernels/backflow_kernel_fully_connected.py` & `qmctorch-0.3.0/qmctorch/wavefunction/orbitals/backflow/kernels/backflow_kernel_fully_connected.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/orbitals/backflow/kernels/backflow_kernel_inverse.py` & `qmctorch-0.3.0/qmctorch/wavefunction/orbitals/backflow/kernels/backflow_kernel_inverse.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/orbitals/backflow/kernels/backflow_kernel_power_sum.py` & `qmctorch-0.3.0/qmctorch/wavefunction/orbitals/backflow/kernels/backflow_kernel_power_sum.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/orbitals/backflow/kernels/backflow_kernel_square.py` & `qmctorch-0.3.0/qmctorch/wavefunction/orbitals/backflow/kernels/backflow_kernel_square.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/orbitals/backflow/orbital_dependent_backflow_kernel.py` & `qmctorch-0.3.0/qmctorch/wavefunction/orbitals/backflow/orbital_dependent_backflow_kernel.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/orbitals/backflow/orbital_dependent_backflow_transformation.py` & `qmctorch-0.3.0/qmctorch/wavefunction/orbitals/backflow/orbital_dependent_backflow_transformation.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/orbitals/norm_orbital.py` & `qmctorch-0.3.0/qmctorch/wavefunction/orbitals/norm_orbital.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/orbitals/radial_functions.py` & `qmctorch-0.3.0/qmctorch/wavefunction/orbitals/radial_functions.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/orbitals/spherical_harmonics.py` & `qmctorch-0.3.0/qmctorch/wavefunction/orbitals/spherical_harmonics.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/pooling/orbital_configurations.py` & `qmctorch-0.3.0/qmctorch/wavefunction/pooling/orbital_configurations.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/pooling/orbital_projector.py` & `qmctorch-0.3.0/qmctorch/wavefunction/pooling/orbital_projector.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/pooling/slater_pooling.py` & `qmctorch-0.3.0/qmctorch/wavefunction/pooling/slater_pooling.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/slater_combined_jastrow_backflow.py` & `qmctorch-0.3.0/qmctorch/wavefunction/slater_jastrow_backflow.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,95 +1,103 @@
 
 
-import numpy as np
 import torch
-from .slater_jastrow import SlaterJastrow
 
+from torch import nn
 import operator
 
-from .jastrows.elec_elec.kernels.pade_jastrow_kernel import PadeJastrowKernel as PadeJastrowKernelElecElec
-from .jastrows.jastrow_factor_combined_terms import JastrowFactorCombinedTerms
-from .jastrows.elec_nuclei.kernels.pade_jastrow_kernel import PadeJastrowKernel as PadeJastrowKernelElecNuc
-
+from .. import log
 
 from .orbitals.atomic_orbitals_backflow import AtomicOrbitalsBackFlow
 from .orbitals.atomic_orbitals_orbital_dependent_backflow import AtomicOrbitalsOrbitalDependentBackFlow
+from .slater_jastrow_base import SlaterJastrowBase
 from .orbitals.backflow.kernels import BackFlowKernelInverse
+from .jastrows.elec_elec.kernels.pade_jastrow_kernel import PadeJastrowKernel
+from .jastrows.elec_elec.jastrow_factor_electron_electron import JastrowFactorElectronElectron
 
 
-class SlaterCombinedJastrowBackflow(SlaterJastrow):
+class SlaterJastrowBackFlow(SlaterJastrowBase):
 
     def __init__(self, mol, configs='ground_state',
                  kinetic='jacobi',
-                 jastrow_kernel={
-                     'ee': PadeJastrowKernelElecElec,
-                     'en': PadeJastrowKernelElecNuc,
-                     'een': None},
-                 jastrow_kernel_kwargs={
-                     'ee': {},
-                     'en': {},
-                     'een': {}},
+                 jastrow_kernel=PadeJastrowKernel,
+                 jastrow_kernel_kwargs={},
                  backflow_kernel=BackFlowKernelInverse,
                  backflow_kernel_kwargs={},
                  orbital_dependent_backflow=False,
                  cuda=False,
                  include_all_mo=True):
-        """Implementation of the QMC Network.
+        """Slater Jastrow wave function with electron-electron Jastrow factor and backflow
+
+        .. math::
+            \\Psi(R_{at}, r) = J(r)\\sum_n c_n D^\\uparrow_n(q^\\uparrow)D^\\downarrow_n(q^\\downarrow)
+
+        with
+
+        .. math::
+            J(r) = \\exp\\left( K_{ee}(r) \\right)
+        
+        with K, a kernel function depending only on the electron-eletron distances, and
+
+        .. math::
+            q(r_i) = r_i + \\sum){j\\neq i} K_{BF}(r_{ij})(r_i-r_j)
 
+        is a backflow transformation defined by the kernel K_{BF}. Note that different transformation
+        can be used for different orbital via the `orbital_dependent_backflow` option.
+
+        Args:
         Args:
-            mol (qmc.wavefunction.Molecule): a molecule object
+            mol (Molecule): a QMCTorch molecule object
             configs (str, optional): defines the CI configurations to be used. Defaults to 'ground_state'.
+                - ground_state : only the ground state determinant in the wave function
+                - single(n,m) : only single excitation with n electrons and m orbitals 
+                - single_double(n,m) : single and double excitation with n electrons and m orbitals
+                - cas(n, m) : all possible configuration using n eletrons and m orbitals                   
             kinetic (str, optional): method to compute the kinetic energy. Defaults to 'jacobi'.
-            jastrow_kernel (dict, optional) : dictionary of jastrow kernels classes
-            jastrow_kernel_kwargs (dict, optional) : dictionary of keywords arguments for the jastrow kernel contructor
-            backflow_kernel (BackFlowKernelBase, optional) : kernel function of the backflow transformation
+                - jacobi : use the Jacobi formula to compute the kinetic energy 
+                - auto : use automatic differentiation to compute the kinetic energy
+            jastrow_kernel (JastrowKernelBase, optional) : Class that computes the jastrow kernels
+            jastrow_kernel_kwargs (dict, optional) : keyword arguments for the jastrow kernel contructor
+            backflow_kernel (BackFlowKernelBase, optional) : kernel function of the backflow transformation. 
+                - By default an inverse kernel K(r_{ij}) = w/r_{ij} is used
             backflow_kernel_kwargs (dict, optional) : keyword arguments for the backflow kernel contructor
+            orbital_dependent_backflow (bool, optional) : every orbital has a different transformation if True. Default to False 
             cuda (bool, optional): turns GPU ON/OFF  Defaults to False.
             include_all_mo (bool, optional): include either all molecular orbitals or only the ones that are
                                              popualted in the configs. Defaults to False
+    
         Examples::
+            >>> from qmctorch.scf import Molecule
+            >>> from qmctorch.wavefunction import SlaterJastrowBackFlow
             >>> mol = Molecule('h2o.xyz', calculator='adf', basis = 'dzp')
-            >>> wf = SlaterJastrow(mol, configs='cas(2,2)')
+            >>> wf = SlaterJastrowBackFlow(mol, configs='cas(2,2)')
         """
 
-        super().__init__(mol, configs, kinetic, None, {}, cuda, include_all_mo)
+        super().__init__(mol, configs, kinetic, cuda, include_all_mo)
 
         # process the backflow transformation
         if orbital_dependent_backflow:
             self.ao = AtomicOrbitalsOrbitalDependentBackFlow(
                 mol, backflow_kernel, backflow_kernel_kwargs, cuda)
         else:
             self.ao = AtomicOrbitalsBackFlow(
                 mol, backflow_kernel, backflow_kernel_kwargs, cuda)
 
-        if self.cuda:
-            self.ao = self.ao.to(self.device)
-
         # process the Jastrow
-        if jastrow_kernel is not None:
-
-            for k in ['ee', 'en', 'een']:
-                if k not in jastrow_kernel.keys():
-                    jastrow_kernel[k] = None
-                if k not in jastrow_kernel_kwargs.keys():
-                    jastrow_kernel_kwargs[k] = None
+        self.jastrow = JastrowFactorElectronElectron(
+            self.mol.nup, self.mol.ndown, jastrow_kernel,
+            kernel_kwargs=jastrow_kernel_kwargs, cuda=cuda)
 
+        if jastrow_kernel is not None:
             self.use_jastrow = True
-            self.jastrow_type = 'JastrowFactorCombinedTerms'
+            self.jastrow_type = jastrow_kernel.__name__
 
-            self.jastrow = JastrowFactorCombinedTerms(
-                self.mol.nup, self.mol.ndown,
-                torch.as_tensor(self.mol.atom_coords),
-                jastrow_kernel=jastrow_kernel,
-                jastrow_kernel_kwargs=jastrow_kernel_kwargs,
-                cuda=cuda)
-
-            if self.cuda:
-                for term in self.jastrow.jastrow_terms:
-                    term = term.to(self.device)
+        if self.cuda:
+            self.jastrow = self.jastrow.to(self.device)
+            self.ao = self.ao.to(self.device)
 
         self.log_data()
 
     def forward(self, x, ao=None):
         """computes the value of the wave function for the sampling points
 
         .. math::
@@ -151,19 +159,19 @@
             [type]: [description]
         """
 
         ao = self.ao(x, derivative=derivative, sum_grad=sum_grad)
         return self.ao2mo(ao)
 
     def kinetic_energy_jacobi(self, x,  **kwargs):
-        r"""Compute the value of the kinetic enery using the Jacobi Formula.
+        """Compute the value of the kinetic enery using the Jacobi Formula.
 
 
         .. math::
-             \\frac{\Delta (J(R) \Psi(R))}{ J(R) \Psi(R)} = \\frac{\\Delta J(R)}{J(R}
+             \\frac{\\Delta (J(R) \\Psi(R))}{ J(R) \\Psi(R)} = \\frac{\\Delta J(R)}{J(R)}
                                                           + 2 \\frac{\\nabla J(R)}{J(R)} \\frac{\\nabla \\Psi(R)}{\\Psi(R)}
                                                           + \\frac{\\Delta \\Psi(R)}{\\Psi(R)}
 
         The lapacian of the determinental part is computed via
 
         .. math::
             \\Delta_i \\Psi(R) \\sum_n c_n ( \\frac{\\Delta_i D_n^{u}}{D_n^{u}} +
```

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/slater_jastrow.py` & `qmctorch-0.3.0/qmctorch/wavefunction/slater_jastrow.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,26 +12,44 @@
 
     def __init__(self, mol, configs='ground_state',
                  kinetic='jacobi',
                  jastrow_kernel=PadeJastrowKernel,
                  jastrow_kernel_kwargs={},
                  cuda=False,
                  include_all_mo=True):
-        """Implementation of the QMC Network.
+        """Slater Jastrow wave function with electron-electron Jastrow factor
+
+        .. math::
+            \\Psi(R_{at}, r) = J(r)\\sum_n c_n D^\\uparrow_n(r^\\uparrow)D^\\downarrow_n(r^\\downarrow)
+
+        with
+
+        .. math::
+            J(r) = \\exp\\left( K_{ee}(r) \\right)
+
+        with K, a kernel function depending only on the electron-eletron distances 
 
         Args:
-            mol (qmc.wavefunction.Molecule): a molecule object
+            mol (Molecule): a QMCTorch molecule object
             configs (str, optional): defines the CI configurations to be used. Defaults to 'ground_state'.
+                - ground_state : only the ground state determinant in the wave function
+                - single(n,m) : only single excitation with n electrons and m orbitals 
+                - single_double(n,m) : single and double excitation with n electrons and m orbitals
+                - cas(n, m) : all possible configuration using n eletrons and m orbitals                   
             kinetic (str, optional): method to compute the kinetic energy. Defaults to 'jacobi'.
+                - jacobi : use the Jacobi formula to compute the kinetic energy 
+                - auto : use automatic differentiation to compute the kinetic energy
             jastrow_kernel (JastrowKernelBase, optional) : Class that computes the jastrow kernels
             jastrow_kernel_kwargs (dict, optional) : keyword arguments for the jastrow kernel contructor
-            cuda (bool, optional): turns GPU ON/OFF  Defaults to False.
+            cuda (bool, optional): turns GPU ON/OFF  Defaults to Fals   e.
             include_all_mo (bool, optional): include either all molecular orbitals or only the ones that are
                                              popualted in the configs. Defaults to False
         Examples::
+            >>> from qmctorch.scf import Molecule
+            >>> from qmctorch.wavefunction import SlaterJastrow
             >>> mol = Molecule('h2o.xyz', calculator='adf', basis = 'dzp')
             >>> wf = SlaterJastrow(mol, configs='cas(2,2)')
         """
 
         super().__init__(mol, configs, kinetic, cuda, include_all_mo)
 
         # process the Jastrow
@@ -48,15 +66,15 @@
 
         self.log_data()
 
     def forward(self, x, ao=None):
         """computes the value of the wave function for the sampling points
 
         .. math::
-            \\Psi(R) =  \\sum_{n} c_n J(R) D^{u}_n(r^u) \\times D^{d}_n(r^d)
+            \\Psi(R) =  J(R) \\sum_{n} c_n  D^{u}_n(r^u) \\times D^{d}_n(r^d)
 
         Args:
             x (torch.tensor): sampling points (Nbatch, 3*Nelec)
             ao (torch.tensor, optional): values of the atomic orbitals (Nbatch, Nelec, Nao)
 
         Returns:
             torch.tensor: values of the wave functions at each sampling point (Nbatch, 1)
@@ -106,29 +124,30 @@
 
         Returns:
             torch.tensor -- MO matrix [nbatch, nelec, nmo]
         """
         return self.mo(self.mo_scf(self.ao(x, derivative=derivative)))
 
     def kinetic_energy_jacobi(self, x, **kwargs):
-        r"""Compute the value of the kinetic enery using the Jacobi Formula.
+        """Compute the value of the kinetic enery using the Jacobi Formula.
         C. Filippi, Simple Formalism for Efficient Derivatives .
 
         .. math::
-             \\frac{\Delta \\Psi(R)}{ \\Psi(R)} = \\Psi(R)^{-1} \\sum_n c_n (\\frac{\\Delta D_n^u}{D_n^u} + \\frac{\\Delta D_n^d}{D_n^d}) D_n^u D_n^d
+            \\frac{\Delta \\Psi(R)}{\\Psi(R)} = \\Psi(R)^{-1} \\sum_n c_n (\\frac{\Delta D_n^u}{D_n^u} + \\frac{\Delta D_n^d}{D_n^d}) D_n^u D_n^d
 
         We compute the laplacian of the determinants through the Jacobi formula
 
         .. math::
-            \\frac{\\Delta det(A)}{det(A)} = Tr(A^{-1} \\Delta A)
+            \\frac{\\Delta \\det(A)}{\\det(A)} = Tr(A^{-1} \\Delta A)
 
-        Here A = J(R) phi and therefore :
+        Here :math:`A = J(R) \\phi` and therefore :
 
         .. math::
             \\Delta A = (\\Delta J) D + 2 \\nabla J \\nabla D + (\\Delta D) J
+
         Args:
             x (torch.tensor): sampling points (Nbatch, 3*Nelec)
 
         Returns:
             torch.tensor: values of the kinetic energy at each sampling points
         """
 
@@ -146,15 +165,15 @@
         C. Filippi, Simple Formalism for Efficient Derivatives.
 
         .. math::
              \\frac{K(R)}{\Psi(R)} = Tr(A^{-1} B_{grad})
 
         The gradients of the wave function
 
-        .. math:
+        .. math::
             \\Psi(R) = J(R) \\sum_n c_n D^{u}_n D^{d}_n = J(R) \\Sigma
 
         are computed following
 
         .. math::
             \\nabla \\Psi(R) = \\left( \\nabla J(R) \\right) \\Sigma + J(R) \\left(\\nabla \Sigma \\right)
 
@@ -164,15 +183,15 @@
 
             \\nabla \\Sigma =  \\sum_n c_n (\\frac{\\nabla D^u_n}{D^u_n} + \\frac{\\nabla D^d_n}{D^d_n}) D^u_n D^d_n
 
         that we compute with the Jacobi formula as:
 
         .. math::
 
-            \\nabla \\Sigma =  \\sum_n c_n (Tr( (D^u_n)^-1 \\nabla D^u_n) + Tr( (D^d_n)^-1 \\nabla D^d_n)) D^u_n D^d_n
+            \\nabla \\Sigma =  \\sum_n c_n (Tr( (D^u_n)^{-1} \\nabla D^u_n) + Tr( (D^d_n)^{-1} \\nabla D^d_n)) D^u_n D^d_n
 
         Args:
             x (torch.tensor): sampling points (Nbatch, 3*Nelec)
             pdf (bool, optional) : if true compute the grads of the density
 
         Returns:
             torch.tensor: values of the gradients wrt the walker pos at each sampling points
```

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/slater_jastrow_backflow.py` & `qmctorch-0.3.0/qmctorch/wavefunction/slater_combined_jastrow_backflow.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,75 +1,124 @@
 
 
+import numpy as np
 import torch
+from .slater_jastrow import SlaterJastrow
 
-from torch import nn
 import operator
 
-from .. import log
+from .jastrows.elec_elec.kernels.pade_jastrow_kernel import PadeJastrowKernel as PadeJastrowKernelElecElec
+from .jastrows.jastrow_factor_combined_terms import JastrowFactorCombinedTerms
+from .jastrows.elec_nuclei.kernels.pade_jastrow_kernel import PadeJastrowKernel as PadeJastrowKernelElecNuc
+
 
 from .orbitals.atomic_orbitals_backflow import AtomicOrbitalsBackFlow
 from .orbitals.atomic_orbitals_orbital_dependent_backflow import AtomicOrbitalsOrbitalDependentBackFlow
-from .slater_jastrow_base import SlaterJastrowBase
 from .orbitals.backflow.kernels import BackFlowKernelInverse
-from .jastrows.elec_elec.kernels.pade_jastrow_kernel import PadeJastrowKernel
-from .jastrows.elec_elec.jastrow_factor_electron_electron import JastrowFactorElectronElectron
 
 
-class SlaterJastrowBackFlow(SlaterJastrowBase):
+class SlaterManyBodyJastrowBackflow(SlaterJastrow):
 
     def __init__(self, mol, configs='ground_state',
                  kinetic='jacobi',
-                 jastrow_kernel=PadeJastrowKernel,
-                 jastrow_kernel_kwargs={},
+                 jastrow_kernel={
+                     'ee': PadeJastrowKernelElecElec,
+                     'en': PadeJastrowKernelElecNuc,
+                     'een': None},
+                 jastrow_kernel_kwargs={
+                     'ee': {},
+                     'en': {},
+                     'een': {}},
                  backflow_kernel=BackFlowKernelInverse,
                  backflow_kernel_kwargs={},
                  orbital_dependent_backflow=False,
                  cuda=False,
                  include_all_mo=True):
-        """Implementation of the QMC Network.
+        """Slater Jastrow wave function with many-body Jastrow factor and backflow
+
+        .. math::
+            \\Psi(R_{at}, r) = J(R_{at}, r)\\sum_n c_n D^\\uparrow_n(q^\\uparrow)D^\\downarrow_n(q^\\downarrow)
+
+        with
+
+        .. math::
+            J(r) = \\exp\\left( K_{ee}(r) + K_{en}(R_{at},r) + K_{een}(R_{at}, r) \\right)    
+
+        with the different kernels representing electron-electron, electron-nuclei and electron-electron-nuclei terms and
+
+        .. math::
+            q(r_i) = r_i + \\sum){j\\neq i} K_{BF}(r_{ij})(r_i-r_j)
+
+        is a backflow transformation defined by the kernel K_{BF}. Note that different transformation
+        can be used for different orbital via the `orbital_dependent_backflow` option.
 
         Args:
-            mol (qmc.wavefunction.Molecule): a molecule object
+        Args:
+            mol (Molecule): a QMCTorch molecule object
             configs (str, optional): defines the CI configurations to be used. Defaults to 'ground_state'.
+                - ground_state : only the ground state determinant in the wave function
+                - single(n,m) : only single excitation with n electrons and m orbitals 
+                - single_double(n,m) : single and double excitation with n electrons and m orbitals
+                - cas(n, m) : all possible configuration using n eletrons and m orbitals                   
             kinetic (str, optional): method to compute the kinetic energy. Defaults to 'jacobi'.
-            jastrow_kernel (JastrowKernelBase, optional) : Class that computes the jastrow kernels
-            jastrow_kernel_kwargs (dict, optional) : keyword arguments for the jastrow kernel contructor
-            backflow_kernel (BackFlowKernelBase, optional) : kernel function of the backflow transformation
+                - jacobi : use the Jacobi formula to compute the kinetic energy 
+                - auto : use automatic differentiation to compute the kinetic energy
+            jastrow_kernel (dict, optional) : different Jastrow kernels for the different terms. 
+                By default only electron-electron and electron-nuclei terms are used
+            jastrow_kernel_kwargs (dict, optional) : keyword arguments for the jastrow kernels contructor
+            backflow_kernel (BackFlowKernelBase, optional) : kernel function of the backflow transformation. 
+                - By default an inverse kernel K(r_{ij}) = w/r_{ij} is used
             backflow_kernel_kwargs (dict, optional) : keyword arguments for the backflow kernel contructor
+            orbital_dependent_backflow (bool, optional) : every orbital has a different transformation if True. Default to False 
             cuda (bool, optional): turns GPU ON/OFF  Defaults to False.
             include_all_mo (bool, optional): include either all molecular orbitals or only the ones that are
                                              popualted in the configs. Defaults to False
+    
         Examples::
+            >>> from qmctorch.scf import Molecule
+            >>> from qmctorch.wavefunction import SlaterManyBodyJastrowBackflow
             >>> mol = Molecule('h2o.xyz', calculator='adf', basis = 'dzp')
-            >>> wf = SlaterJastrow(mol, configs='cas(2,2)')
+            >>> wf = SlaterManyBodyJastrowBackflow(mol, configs='cas(2,2)')
         """
 
-        super().__init__(mol, configs, kinetic, cuda, include_all_mo)
+        super().__init__(mol, configs, kinetic, None, {}, cuda, include_all_mo)
 
         # process the backflow transformation
         if orbital_dependent_backflow:
             self.ao = AtomicOrbitalsOrbitalDependentBackFlow(
                 mol, backflow_kernel, backflow_kernel_kwargs, cuda)
         else:
             self.ao = AtomicOrbitalsBackFlow(
                 mol, backflow_kernel, backflow_kernel_kwargs, cuda)
 
-        # process the Jastrow
-        self.jastrow = JastrowFactorElectronElectron(
-            self.mol.nup, self.mol.ndown, jastrow_kernel,
-            kernel_kwargs=jastrow_kernel_kwargs, cuda=cuda)
+        if self.cuda:
+            self.ao = self.ao.to(self.device)
 
+        # process the Jastrow
         if jastrow_kernel is not None:
+
+            for k in ['ee', 'en', 'een']:
+                if k not in jastrow_kernel.keys():
+                    jastrow_kernel[k] = None
+                if k not in jastrow_kernel_kwargs.keys():
+                    jastrow_kernel_kwargs[k] = None
+
             self.use_jastrow = True
-            self.jastrow_type = jastrow_kernel.__name__
+            self.jastrow_type = 'JastrowFactorCombinedTerms'
 
-        if self.cuda:
-            self.jastrow = self.jastrow.to(self.device)
-            self.ao = self.ao.to(self.device)
+            self.jastrow = JastrowFactorCombinedTerms(
+                self.mol.nup, self.mol.ndown,
+                torch.as_tensor(self.mol.atom_coords),
+                jastrow_kernel=jastrow_kernel,
+                jastrow_kernel_kwargs=jastrow_kernel_kwargs,
+                cuda=cuda)
+
+            if self.cuda:
+                for term in self.jastrow.jastrow_terms:
+                    term = term.to(self.device)
 
         self.log_data()
 
     def forward(self, x, ao=None):
         """computes the value of the wave function for the sampling points
 
         .. math::
```

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/slater_jastrow_base.py` & `qmctorch-0.3.0/qmctorch/wavefunction/slater_jastrow_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,24 +21,26 @@
                  configs='ground_state',
                  kinetic='jacobi',
                  cuda=False,
                  include_all_mo=True):
         """Implementation of the QMC Network.
 
         Args:
-            mol (qmc.wavefunction.Molecule): a molecule object
+            mol (Molecule): a QMCTorch molecule object
             configs (str, optional): defines the CI configurations to be used. Defaults to 'ground_state'.
+                - ground_state : only the ground state determinant in the wave function
+                - single(n,m) : only single excitation with n electrons and m orbitals 
+                - single_double(n,m) : single and double excitation with n electrons and m orbitals
+                - cas(n, m) : all possible configuration using n eletrons and m orbitals                   
             kinetic (str, optional): method to compute the kinetic energy. Defaults to 'jacobi'.
-            use_jastrow (bool, optional): turn jastrow factor ON/OFF. Defaults to True.
+                - jacobi : use the Jacobi formula to compute the kinetic energy 
+                - auto : use automatic differentiation to compute the kinetic energy
             cuda (bool, optional): turns GPU ON/OFF  Defaults to False.
             include_all_mo (bool, optional): include either all molecular orbitals or only the ones that are
                                              popualted in the configs. Defaults to False
-        Examples::
-            >>> mol = Molecule('h2o.xyz', calculator='adf', basis = 'dzp')
-            >>> wf = SlaterJastrow(mol, configs='cas(2,2)')
         """
 
         super(SlaterJastrowBase, self).__init__(
             mol.nelec, 3, kinetic, cuda)
 
         # check for cuda
         if not torch.cuda.is_available and self.cuda:
@@ -290,19 +292,19 @@
 
         Returns:
             torch.tensor -- MO matrix [nbatch, nelec, nmo]
         """
         raise NotImplementedError('Implement a get_mo_vals method')
 
     def kinetic_energy_jacobi(self, x,  **kwargs):
-        r"""Compute the value of the kinetic enery using the Jacobi Formula.
+        """Compute the value of the kinetic enery using the Jacobi Formula.
         C. Filippi, Simple Formalism for Efficient Derivatives .
 
         .. math::
-             \\frac{K(R)}{\Psi(R)} = Tr(A^{-1} B_{kin})
+             \\frac{K(R)}{\\Psi(R)} = Tr(A^{-1} B_{kin})
 
         Args:
             x (torch.tensor): sampling points (Nbatch, 3*Nelec)
 
         Returns:
             torch.tensor: values of the kinetic energy at each sampling points
         """
```

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/slater_orbital_dependent_jastrow.py` & `qmctorch-0.3.0/qmctorch/wavefunction/slater_orbital_dependent_jastrow.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,27 +11,44 @@
     def __init__(self, mol,
                  configs='ground_state',
                  kinetic='jacobi',
                  jastrow_kernel=PadeJastrowKernel,
                  jastrow_kernel_kwargs={},
                  cuda=False,
                  include_all_mo=True):
-        """Implementation of the QMC Network.
+        """Slater Jastrow Wave function with an orbital dependent Electron-Electron Jastrow Factor
+
+        .. math::
+            \\Psi(R_{at}, r) = \\sum_n c_n D^\\uparrow_n(r^\\uparrow)D^\\downarrow_n(r^\\downarrow)
+
+        where each molecular orbital of the determinants is multiplied with a different electron-electron Jastrow
+
+        .. math::
+            \\phi_i(r) \\rightarrow J_i(r) \\phi_i(r) 
 
         Args:
-            mol (qmc.wavefunction.Molecule): a molecule object
+            mol (Molecule): a QMCTorch molecule object
             configs (str, optional): defines the CI configurations to be used. Defaults to 'ground_state'.
+                - ground_state : only the ground state determinant in the wave function
+                - single(n,m) : only single excitation with n electrons and m orbitals 
+                - single_double(n,m) : single and double excitation with n electrons and m orbitals
+                - cas(n, m) : all possible configuration using n eletrons and m orbitals                   
             kinetic (str, optional): method to compute the kinetic energy. Defaults to 'jacobi'.
-            use_jastrow (bool, optional): turn jastrow factor ON/OFF. Defaults to True.
+                - jacobi : use the Jacobi formula to compute the kinetic energy 
+                - auto : use automatic differentiation to compute the kinetic energy
+            jastrow_kernel (JastrowKernelBase, optional) : Class that computes the jastrow kernels
+            jastrow_kernel_kwargs (dict, optional) : keyword arguments for the jastrow kernel contructor
             cuda (bool, optional): turns GPU ON/OFF  Defaults to False.
             include_all_mo (bool, optional): include either all molecular orbitals or only the ones that are
                                              popualted in the configs. Defaults to False
         Examples::
+            >>> from qmctorch.scf import Molecule
+            >>> from qmctorch.wavefunction import SlaterOrbitalDependentJastrow
             >>> mol = Molecule('h2o.xyz', calculator='adf', basis = 'dzp')
-            >>> wf = SlaterJastrow(mol, configs='cas(2,2)')
+            >>> wf = SlaterOrbitalDependentJastrow(mol, configs='cas(2,2)')
         """
 
         if jastrow_kernel is None:
             raise ValueError(
                 'Orbital dependent Jastrow factor requires a valid jastrow kernel.')
 
         super().__init__(mol, configs, kinetic, cuda, include_all_mo)
@@ -191,19 +208,20 @@
             djast_dmo = (djast * dmo).sum(-1)
             d2jast_mo = d2jast.sum(1).unsqueeze(1) * mo
 
             # assemble kin op
             return jast_d2mo + 2 * djast_dmo + d2jast_mo
 
     def kinetic_energy_jacobi(self, x,  **kwargs):
-        r"""Compute the value of the kinetic enery using the Jacobi Formula.
+        """Compute the value of the kinetic enery using the Jacobi Formula.
         C. Filippi, Simple Formalism for Efficient Derivatives .
 
         .. math::
-             \\frac{K(R)}{\Psi(R)} = Tr(A^{-1} B_{kin})
+
+             \\frac{K(R)}{\\Psi(R)} = Tr(A^{-1} B_{kin})
 
         Args:
             x (torch.tensor): sampling points (Nbatch, 3*Nelec)
 
         Returns:
             torch.tensor: values of the kinetic energy at each sampling points
         """
```

### Comparing `qmctorch-0.2.0/qmctorch/wavefunction/wf_base.py` & `qmctorch-0.3.0/qmctorch/wavefunction/wf_base.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/qmctorch.egg-info/PKG-INFO` & `qmctorch-0.3.0/qmctorch.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: qmctorch
-Version: 0.2.0
+Version: 0.3.0
 Summary: Pytorch Implementation of Quantum Monte Carlo
 Home-page: https://github.com/NLESC-JCER/QMCTorch
 Author: ['Nicolas Renaud', 'Felipe Zapata']
 Author-email: n.renaud@esciencecenter.nl
 License: Apache Software License 2.0
 Keywords: qmctorch
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Scientific/Engineering :: Chemistry
@@ -42,9 +41,7 @@
 https://qmctorch.readthedocs.io/en/latest/intro.html
 
 
 ## Disclaimer
 QMCTorch is currently under developmement and most likely won't behave as expected 
 
 
-
-
```

### Comparing `qmctorch-0.2.0/qmctorch.egg-info/SOURCES.txt` & `qmctorch-0.3.0/qmctorch.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 qmctorch/scf/__init__.py
 qmctorch/scf/molecule.py
 qmctorch/scf/calculator/__init__.py
 qmctorch/scf/calculator/adf.py
 qmctorch/scf/calculator/calculator_base.py
 qmctorch/scf/calculator/pyscf.py
 qmctorch/solver/__init__.py
+qmctorch/solver/solver.py
 qmctorch/solver/solver_base.py
-qmctorch/solver/solver_slater_jastrow.py
-qmctorch/solver/solver_slater_jastrow_horovod.py
+qmctorch/solver/solver_mpi.py
 qmctorch/utils/__init__.py
 qmctorch/utils/algebra_utils.py
 qmctorch/utils/hdf5_utils.py
 qmctorch/utils/interpolate.py
 qmctorch/utils/plot_data.py
 qmctorch/utils/stat_utils.py
 qmctorch/utils/torch_utils.py
```

### Comparing `qmctorch-0.2.0/setup.py` & `qmctorch-0.3.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,19 +37,17 @@
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Topic :: Scientific/Engineering :: Chemistry'
     ],
     test_suite='tests',
     install_requires=['matplotlib', 'numpy', 'argparse',
-                      'scipy', 'tqdm', 'torch',
-                      # 'plams@git+https://github.com/SCM-NV/PLAMS@master',
-                      'plams',
+                      'scipy', 'tqdm', 'torch', 'plams',
                       'pyscf', 'mendeleev', 'twiggy', 'mpi4py'],
 
     extras_require={
-        'hpc': ['horovod'],
-        'doc': ['recommonmark', 'sphinx', 'sphinx_rtd_theme'],
+        'hpc': ['horovod==0.27.0'],
+        'doc': ['recommonmark', 'sphinx', 'sphinx_rtd_theme', 'nbsphinx'],
         'test': ['pytest', 'pytest-runner',
                  'coverage', 'coveralls', 'pycodestyle'],
     }
 )
```

### Comparing `qmctorch-0.2.0/tests/sampler/test_metropolis.py` & `qmctorch-0.3.0/tests/sampler/test_metropolis.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/tests/sampler/test_sampler_base.py` & `qmctorch-0.3.0/tests/sampler/test_sampler_base.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/tests/sampler/test_walker.py` & `qmctorch-0.3.0/tests/sampler/test_walker.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/tests/scf/test_gto2sto_fit.py` & `qmctorch-0.3.0/tests/scf/test_gto2sto_fit.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/tests/scf/test_molecule.py` & `qmctorch-0.3.0/tests/scf/test_molecule.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/tests/solver/test_h2.py` & `qmctorch-0.3.0/tests/solver/test_h2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import unittest
 
 import numpy as np
 import torch
 import torch.optim as optim
 
 from qmctorch.sampler import Hamiltonian, Metropolis
-from qmctorch.solver import SolverSlaterJastrow
+from qmctorch.solver import Solver
 from qmctorch.utils import (plot_block, plot_blocking_energy,
                             plot_correlation_coefficient, plot_energy,
                             plot_integrated_autocorrelation_time,
                             plot_walkers_traj)
 from qmctorch.scf import Molecule
 from qmctorch.wavefunction import SlaterJastrow
 
@@ -58,15 +58,15 @@
             nelec=self.wf.nelec,
             init=self.mol.domain('normal'))
 
         # optimizer
         self.opt = optim.Adam(self.wf.parameters(), lr=0.01)
 
         # solver
-        self.solver = SolverSlaterJastrow(wf=self.wf, sampler=self.sampler,
+        self.solver = Solver(wf=self.wf, sampler=self.sampler,
                                           optimizer=self.opt)
 
         # ground state energy
         self.ground_state_energy = -1.16
 
         # ground state pos
         self.ground_state_pos = 0.69
```

### Comparing `qmctorch-0.2.0/tests/solver/test_h2_adf.py` & `qmctorch-0.3.0/tests/solver/test_h2_adf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import unittest
 
 import numpy as np
 import torch
 import torch.optim as optim
 
 from qmctorch.sampler import Metropolis
-from qmctorch.solver import SolverSlaterJastrow
+from qmctorch.solver import Solver
 from qmctorch.scf import Molecule
 from qmctorch.wavefunction import SlaterJastrow
 
 from ..path_utils import PATH_TEST
 
 
 class TestH2ADF(unittest.TestCase):
@@ -39,15 +39,15 @@
                 'type': 'all-elec',
                 'proba': 'normal'})
 
         # optimizer
         self.opt = optim.Adam(self.wf.parameters(), lr=0.01)
 
         # solver
-        self.solver = SolverSlaterJastrow(wf=self.wf, sampler=self.sampler,
+        self.solver = Solver(wf=self.wf, sampler=self.sampler,
                                           optimizer=self.opt)
 
         # ground state energy
         self.ground_state_energy = -1.16
 
         # ground state pos
         self.ground_state_pos = 0.69
```

### Comparing `qmctorch-0.2.0/tests/solver/test_h2_adf_jacobi.py` & `qmctorch-0.3.0/tests/solver/test_h2_adf_jacobi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import unittest
 
 import numpy as np
 import torch
 import torch.optim as optim
 
 from qmctorch.sampler import Metropolis
-from qmctorch.solver import SolverSlaterJastrow
+from qmctorch.solver import Solver
 from qmctorch.scf import Molecule
 from qmctorch.wavefunction import SlaterJastrow
 from ..path_utils import PATH_TEST
 
 
 class TestH2ADFJacobi(unittest.TestCase):
 
@@ -38,15 +38,15 @@
                 'type': 'all-elec',
                 'proba': 'normal'})
 
         # optimizer
         self.opt = optim.Adam(self.wf.parameters(), lr=0.01)
 
         # solver
-        self.solver = SolverSlaterJastrow(wf=self.wf, sampler=self.sampler,
+        self.solver = Solver(wf=self.wf, sampler=self.sampler,
                                           optimizer=self.opt)
 
         # ground state energy
         self.ground_state_energy = -1.16
 
         # ground state pos
         self.ground_state_pos = 0.69
```

### Comparing `qmctorch-0.2.0/tests/solver/test_h2_correlated.py` & `qmctorch-0.3.0/tests/solver/test_h2_correlated.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import numpy as np
 import torch
 import torch.optim as optim
 
 
 from qmctorch.sampler import Metropolis
-from qmctorch.solver import SolverSlaterJastrow
+from qmctorch.solver import Solver
 from qmctorch.utils import plot_energy
 
 
 from qmctorch.scf import Molecule
 from qmctorch.wavefunction import SlaterOrbitalDependentJastrow
 from qmctorch.utils import set_torch_double_precision
 from qmctorch.wavefunction.jastrows.elec_elec.kernels import FullyConnectedJastrowKernel
@@ -56,15 +56,15 @@
                 'type': 'all-elec',
                 'proba': 'normal'})
 
         # optimizer
         self.opt = optim.Adam(self.wf.parameters(), lr=0.01)
 
         # solver
-        self.solver = SolverSlaterJastrow(wf=self.wf, sampler=self.sampler,
+        self.solver = Solver(wf=self.wf, sampler=self.sampler,
                                           optimizer=self.opt)
 
         # ground state energy
         self.ground_state_energy = -1.16
 
         # ground state pos
         self.ground_state_pos = 0.69
```

### Comparing `qmctorch-0.2.0/tests/solver/test_h2_stats.py` & `qmctorch-0.3.0/tests/solver/test_h2_stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import unittest
 
 import numpy as np
 import torch
 import torch.optim as optim
 
 from qmctorch.sampler import Metropolis
-from qmctorch.solver import SolverSlaterJastrow
+from qmctorch.solver import Solver
 from qmctorch.utils import (plot_block, plot_blocking_energy,
                             plot_correlation_coefficient,
                             plot_integrated_autocorrelation_time,
                             plot_walkers_traj)
 from qmctorch.scf import Molecule
 from qmctorch.wavefunction import SlaterJastrow
 
@@ -53,15 +53,15 @@
                 'type': 'all-elec',
                 'proba': 'normal'})
 
         # optimizer
         self.opt = optim.Adam(self.wf.parameters(), lr=0.01)
 
         # solver
-        self.solver = SolverSlaterJastrow(wf=self.wf, sampler=self.sampler,
+        self.solver = Solver(wf=self.wf, sampler=self.sampler,
                                           optimizer=self.opt)
 
     def test_sampling_traj(self):
 
         pos = self.solver.sampler(self.solver.wf.pdf)
         obs = self.solver.sampling_traj(pos)
```

### Comparing `qmctorch-0.2.0/tests/solver/test_lih.py` & `qmctorch-0.3.0/tests/solver/test_lih.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import unittest
 
 import numpy as np
 import torch
 import torch.optim as optim
 
 from qmctorch.sampler import Metropolis
-from qmctorch.solver import SolverSlaterJastrow
+from qmctorch.solver import Solver
 from qmctorch.scf import Molecule
 from qmctorch.wavefunction import SlaterJastrow
 
 
 class TestLiH(unittest.TestCase):
 
     def setUp(self):
@@ -41,15 +41,15 @@
                 'type': 'all-elec',
                 'proba': 'normal'})
 
         # optimizer
         self.opt = optim.Adam(self.wf.parameters(), lr=0.01)
 
         # solver
-        self.solver = SolverSlaterJastrow(wf=self.wf, sampler=self.sampler,
+        self.solver = Solver(wf=self.wf, sampler=self.sampler,
                                           optimizer=self.opt)
 
     def test1_single_point(self):
 
         # sample and compute observables
         obs = self.solver.single_point()
         e, v = obs.energy, obs.variance
```

### Comparing `qmctorch-0.2.0/tests/solver/test_lih_adf_backflow.py` & `qmctorch-0.3.0/tests/solver/test_lih_adf_backflow.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import unittest
 
 import numpy as np
 import torch
 import torch.optim as optim
 
 from qmctorch.sampler import Metropolis
-from qmctorch.solver import SolverSlaterJastrow
+from qmctorch.solver import Solver
 from qmctorch.scf import Molecule
 from qmctorch.wavefunction import SlaterJastrowBackFlow
 from qmctorch.utils import set_torch_double_precision
 
 from ..path_utils import PATH_TEST
 
 
@@ -51,15 +51,15 @@
                 'type': 'all-elec',
                 'proba': 'normal'})
 
         # optimizer
         self.opt = optim.Adam(self.wf.parameters(), lr=0.01)
 
         # solver
-        self.solver = SolverSlaterJastrow(wf=self.wf, sampler=self.sampler,
+        self.solver = Solver(wf=self.wf, sampler=self.sampler,
                                           optimizer=self.opt)
 
         # artificial pos
         self.nbatch = 10
         self.pos = torch.as_tensor(np.random.rand(
             self.nbatch, self.wf.nelec*3))
         self.pos.requires_grad = True
```

### Comparing `qmctorch-0.2.0/tests/solver/test_lih_correlated.py` & `qmctorch-0.3.0/tests/solver/test_lih_correlated.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import unittest
 
 import numpy as np
 import torch
 import torch.optim as optim
 
 from qmctorch.sampler import Metropolis
-from qmctorch.solver import SolverSlaterJastrow
+from qmctorch.solver import Solver
 from qmctorch.scf import Molecule
 from qmctorch.wavefunction import SlaterOrbitalDependentJastrow
 from qmctorch.utils import set_torch_double_precision
 
 from ..path_utils import PATH_TEST
 
 
@@ -51,15 +51,15 @@
                 'type': 'all-elec',
                 'proba': 'normal'})
 
         # optimizer
         self.opt = optim.Adam(self.wf.parameters(), lr=0.01)
 
         # solver
-        self.solver = SolverSlaterJastrow(wf=self.wf,
+        self.solver = Solver(wf=self.wf,
                                           sampler=self.sampler,
                                           optimizer=self.opt)
 
         # artificial pos
         self.nbatch = 10
         self.pos = torch.as_tensor(np.random.rand(
             self.nbatch, self.wf.nelec*3))
```

### Comparing `qmctorch-0.2.0/tests/solver/test_lih_generic_jastrow.py` & `qmctorch-0.3.0/tests/solver/test_lih_generic_jastrow.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import unittest
 
 import numpy as np
 import torch
 import torch.optim as optim
 
 from qmctorch.sampler import Metropolis
-from qmctorch.solver import SolverSlaterJastrow
+from qmctorch.solver import Solver
 from qmctorch.scf import Molecule
 from qmctorch.wavefunction import SlaterJastrow
 from qmctorch.wavefunction.jastrows.elec_elec.kernels import FullyConnectedJastrowKernel
 from qmctorch.utils import set_torch_double_precision
 
 
 class TestLiH(unittest.TestCase):
@@ -45,15 +45,15 @@
                 'type': 'all-elec',
                 'proba': 'normal'})
 
         # optimizer
         self.opt = optim.Adam(self.wf.parameters(), lr=0.01)
 
         # solver
-        self.solver = SolverSlaterJastrow(wf=self.wf, sampler=self.sampler,
+        self.solver = Solver(wf=self.wf, sampler=self.sampler,
                                           optimizer=self.opt)
 
         # artificial pos
         self.nbatch = 10
         self.pos = torch.as_tensor(np.random.rand(
             self.nbatch, self.wf.nelec*3))
         self.pos.requires_grad = True
```

### Comparing `qmctorch-0.2.0/tests/solver/test_lih_pyscf_backflow.py` & `qmctorch-0.3.0/tests/solver/test_lih_pyscf_backflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import unittest
 
 import numpy as np
 import torch
 import torch.optim as optim
 
 from qmctorch.sampler import Metropolis
-from qmctorch.solver import SolverSlaterJastrow
+from qmctorch.solver import Solver
 from qmctorch.scf import Molecule
 from qmctorch.wavefunction import SlaterJastrowBackFlow
 from qmctorch.utils import set_torch_double_precision
 
 
 class TestLiHBackFlowPySCF(unittest.TestCase):
 
@@ -52,15 +52,15 @@
                 'type': 'all-elec',
                 'proba': 'normal'})
 
         # optimizer
         self.opt = optim.Adam(self.wf.parameters(), lr=0.01)
 
         # solver
-        self.solver = SolverSlaterJastrow(wf=self.wf, sampler=self.sampler,
+        self.solver = Solver(wf=self.wf, sampler=self.sampler,
                                           optimizer=self.opt)
 
         # artificial pos
         self.nbatch = 10
         self.pos = torch.as_tensor(np.random.rand(
             self.nbatch, self.wf.nelec*3))
         self.pos.requires_grad = True
```

### Comparing `qmctorch-0.2.0/tests/solver/test_lih_pyscf_compare_backflow.py` & `qmctorch-0.3.0/tests/solver/test_lih_pyscf_compare_backflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import unittest
 
 import numpy as np
 import torch
 import torch.optim as optim
 
 from qmctorch.sampler import Metropolis
-from qmctorch.solver import SolverSlaterJastrow
+from qmctorch.solver import Solver
 from qmctorch.scf import Molecule
 from qmctorch.wavefunction import SlaterJastrowBackFlow, SlaterJastrow
 from qmctorch.utils import set_torch_double_precision
 
 
 def reset_generator():
     torch.manual_seed(0)
@@ -93,18 +93,18 @@
         reset_generator()
         self.opt = optim.Adam(self.wf.parameters(), lr=0.01)
 
         reset_generator()
         self.opt_ref = optim.Adam(self.wf_ref.parameters(), lr=0.01)
 
         # solver
-        self.solver_ref = SolverSlaterJastrow(wf=self.wf_ref, sampler=self.sampler_ref,
+        self.solver_ref = Solver(wf=self.wf_ref, sampler=self.sampler_ref,
                                               optimizer=self.opt_ref)
 
-        self.solver = SolverSlaterJastrow(wf=self.wf, sampler=self.sampler,
+        self.solver = Solver(wf=self.wf, sampler=self.sampler,
                                           optimizer=self.opt)
 
         # artificial pos
         self.nbatch = 10
         self.pos = torch.as_tensor(np.random.rand(
             self.nbatch, self.wf.nelec*3))
         self.pos.requires_grad = True
```

### Comparing `qmctorch-0.2.0/tests/solver/test_lih_pyscf_generic_backflow.py` & `qmctorch-0.3.0/tests/solver/test_lih_pyscf_orbital_dependent_backflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,18 @@
 import unittest
 
 import numpy as np
 import torch
 import torch.optim as optim
 
 from qmctorch.sampler import Metropolis
-from qmctorch.solver import SolverSlaterJastrow
+from qmctorch.solver import Solver
 from qmctorch.scf import Molecule
 from qmctorch.wavefunction import SlaterJastrowBackFlow
 from qmctorch.utils import set_torch_double_precision
-from qmctorch.wavefunction.orbitals.backflow.kernels import BackFlowKernelPowerSum
 
 
 class TestLiHBackFlowPySCF(unittest.TestCase):
 
     def setUp(self):
 
         torch.manual_seed(0)
@@ -27,16 +26,15 @@
             unit='bohr',
             calculator='pyscf',
             basis='sto-3g')
 
         # wave function
         self.wf = SlaterJastrowBackFlow(self.mol, kinetic='jacobi',
                                         configs='single_double(2,2)',
-                                        backflow_kernel=BackFlowKernelPowerSum,
-                                        orbital_dependent_backflow=False,
+                                        orbital_dependent_backflow=True,
                                         include_all_mo=True)
 
         # fc weights
         self.wf.fc.weight.data = torch.rand(self.wf.fc.weight.shape)
 
         # jastrow weights
         self.wf.jastrow.jastrow_kernel.weight.data = torch.rand(
@@ -54,15 +52,15 @@
                 'type': 'all-elec',
                 'proba': 'normal'})
 
         # optimizer
         self.opt = optim.Adam(self.wf.parameters(), lr=0.01)
 
         # solver
-        self.solver = SolverSlaterJastrow(wf=self.wf, sampler=self.sampler,
+        self.solver = Solver(wf=self.wf, sampler=self.sampler,
                                           optimizer=self.opt)
 
         # artificial pos
         self.nbatch = 10
         self.pos = torch.as_tensor(np.random.rand(
             self.nbatch, self.wf.nelec*3))
         self.pos.requires_grad = True
@@ -93,13 +91,11 @@
 
         self.solver.configure(track=['local_energy', 'parameters'],
                               loss='energy', grad='manual')
         obs = self.solver.run(5)
 
 
 if __name__ == "__main__":
-    unittest.main()
-    # t = TestLiHBackFlowPySCF()
-    # t.setUp()
-    # t.test_0_wavefunction()
-    # t.test1_single_point()
-    # # t.test3_wf_opt_grad_manual()
+    # unittest.main()
+    t = TestLiHBackFlowPySCF()
+    t.setUp()
+    t.test3_wf_opt_grad_manual()
```

### Comparing `qmctorch-0.2.0/tests/solver/test_lih_pyscf_orbital_dependent_backflow.py` & `qmctorch-0.3.0/tests/solver/test_lih_pyscf_generic_backflow.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 import unittest
 
 import numpy as np
 import torch
 import torch.optim as optim
 
 from qmctorch.sampler import Metropolis
-from qmctorch.solver import SolverSlaterJastrow
+from qmctorch.solver import Solver
 from qmctorch.scf import Molecule
 from qmctorch.wavefunction import SlaterJastrowBackFlow
 from qmctorch.utils import set_torch_double_precision
+from qmctorch.wavefunction.orbitals.backflow.kernels import BackFlowKernelPowerSum
 
 
 class TestLiHBackFlowPySCF(unittest.TestCase):
 
     def setUp(self):
 
         torch.manual_seed(0)
@@ -26,15 +27,16 @@
             unit='bohr',
             calculator='pyscf',
             basis='sto-3g')
 
         # wave function
         self.wf = SlaterJastrowBackFlow(self.mol, kinetic='jacobi',
                                         configs='single_double(2,2)',
-                                        orbital_dependent_backflow=True,
+                                        backflow_kernel=BackFlowKernelPowerSum,
+                                        orbital_dependent_backflow=False,
                                         include_all_mo=True)
 
         # fc weights
         self.wf.fc.weight.data = torch.rand(self.wf.fc.weight.shape)
 
         # jastrow weights
         self.wf.jastrow.jastrow_kernel.weight.data = torch.rand(
@@ -52,15 +54,15 @@
                 'type': 'all-elec',
                 'proba': 'normal'})
 
         # optimizer
         self.opt = optim.Adam(self.wf.parameters(), lr=0.01)
 
         # solver
-        self.solver = SolverSlaterJastrow(wf=self.wf, sampler=self.sampler,
+        self.solver = Solver(wf=self.wf, sampler=self.sampler,
                                           optimizer=self.opt)
 
         # artificial pos
         self.nbatch = 10
         self.pos = torch.as_tensor(np.random.rand(
             self.nbatch, self.wf.nelec*3))
         self.pos.requires_grad = True
@@ -91,11 +93,13 @@
 
         self.solver.configure(track=['local_energy', 'parameters'],
                               loss='energy', grad='manual')
         obs = self.solver.run(5)
 
 
 if __name__ == "__main__":
-    # unittest.main()
-    t = TestLiHBackFlowPySCF()
-    t.setUp()
-    t.test3_wf_opt_grad_manual()
+    unittest.main()
+    # t = TestLiHBackFlowPySCF()
+    # t.setUp()
+    # t.test_0_wavefunction()
+    # t.test1_single_point()
+    # # t.test3_wf_opt_grad_manual()
```

### Comparing `qmctorch-0.2.0/tests/wavefunction/orbitals/test_ao_derivatives_adf.py` & `qmctorch-0.3.0/tests/wavefunction/orbitals/test_ao_derivatives_adf.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/tests/wavefunction/orbitals/test_ao_derivatives_pyscf.py` & `qmctorch-0.3.0/tests/wavefunction/orbitals/test_ao_derivatives_pyscf.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/tests/wavefunction/orbitals/test_ao_values_adf.py` & `qmctorch-0.3.0/tests/wavefunction/orbitals/test_ao_values_adf.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/tests/wavefunction/orbitals/test_ao_values_pyscf.py` & `qmctorch-0.3.0/tests/wavefunction/orbitals/test_ao_values_pyscf.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/tests/wavefunction/orbitals/test_backflow_ao_derivatives_pyscf.py` & `qmctorch-0.3.0/tests/wavefunction/orbitals/test_backflow_ao_derivatives_pyscf.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/tests/wavefunction/orbitals/test_cartesian_harmonics.py` & `qmctorch-0.3.0/tests/wavefunction/orbitals/test_cartesian_harmonics.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/tests/wavefunction/orbitals/test_cartesian_harmonics_adf.py` & `qmctorch-0.3.0/tests/wavefunction/orbitals/test_cartesian_harmonics_adf.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/tests/wavefunction/orbitals/test_mo_values_adf.py` & `qmctorch-0.3.0/tests/wavefunction/orbitals/test_mo_values_adf.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/tests/wavefunction/orbitals/test_norm.py` & `qmctorch-0.3.0/tests/wavefunction/orbitals/test_norm.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/tests/wavefunction/orbitals/test_orbital_dependent_backflow_ao_derivatives_pyscf.py` & `qmctorch-0.3.0/tests/wavefunction/orbitals/test_orbital_dependent_backflow_ao_derivatives_pyscf.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/tests/wavefunction/orbitals/test_radial_functions.py` & `qmctorch-0.3.0/tests/wavefunction/orbitals/test_radial_functions.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/tests/wavefunction/orbitals/test_radial_gto.py` & `qmctorch-0.3.0/tests/wavefunction/orbitals/test_radial_gto.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/tests/wavefunction/orbitals/test_radial_sto.py` & `qmctorch-0.3.0/tests/wavefunction/orbitals/test_radial_sto.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/tests/wavefunction/orbitals/test_spherical_harmonics.py` & `qmctorch-0.3.0/tests/wavefunction/orbitals/test_spherical_harmonics.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/tests/wavefunction/test_compare_slaterjastrow_backflow.py` & `qmctorch-0.3.0/tests/wavefunction/test_compare_slaterjastrow_backflow.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/tests/wavefunction/test_compare_slaterjastrow_orbital_dependent_backflow.py` & `qmctorch-0.3.0/tests/wavefunction/test_compare_slaterjastrow_orbital_dependent_backflow.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/tests/wavefunction/test_slater_orbital_dependent_jastrow.py` & `qmctorch-0.3.0/tests/wavefunction/test_slater_orbital_dependent_jastrow.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/tests/wavefunction/test_slatercombinedjastrow.py` & `qmctorch-0.3.0/tests/wavefunction/test_slatercombinedjastrow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from qmctorch.scf import Molecule
-from qmctorch.wavefunction import SlaterCombinedJastrow
+from qmctorch.wavefunction import SlaterManyBodyJastrow
 from qmctorch.utils import set_torch_double_precision
 from qmctorch.wavefunction.jastrows.elec_nuclei.kernels import PadeJastrowKernel as PadeJastrowKernelElecNuc
 from qmctorch.wavefunction.jastrows.elec_elec.kernels import PadeJastrowKernel as PadeJastrowKernelElecElec
 from qmctorch.wavefunction.jastrows.elec_elec_nuclei.kernels import BoysHandyJastrowKernel, FullyConnectedJastrowKernel
 from torch.autograd import grad, gradcheck, Variable
 
 import numpy as np
@@ -50,15 +50,15 @@
         mol = Molecule(
             atom='Li 0 0 0; H 0 0 3.14',
             unit='bohr',
             calculator='pyscf',
             basis='sto-3g',
             redo_scf=True)
 
-        self.wf = SlaterCombinedJastrow(mol,
+        self.wf = SlaterManyBodyJastrow(mol,
                                         kinetic='auto',
                                         include_all_mo=False,
                                         configs='single_double(2,2)',
                                         jastrow_kernel={
                                             'ee': PadeJastrowKernelElecElec,
                                             'en': PadeJastrowKernelElecNuc,
                                             'een': BoysHandyJastrowKernel},
```

### Comparing `qmctorch-0.2.0/tests/wavefunction/test_slatercombinedjastrow_backflow.py` & `qmctorch-0.3.0/tests/wavefunction/test_slatercombinedjastrow_backflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from qmctorch.scf import Molecule
-from qmctorch.wavefunction import SlaterCombinedJastrowBackflow
+from qmctorch.wavefunction import SlaterManyBodyJastrowBackflow
 from qmctorch.utils import set_torch_double_precision
 from qmctorch.wavefunction.jastrows.elec_nuclei.kernels import PadeJastrowKernel as PadeJastrowKernelElecNuc
 from qmctorch.wavefunction.jastrows.elec_elec.kernels import PadeJastrowKernel as PadeJastrowKernelElecElec
 from qmctorch.wavefunction.jastrows.elec_elec_nuclei.kernels import BoysHandyJastrowKernel, FullyConnectedJastrowKernel
 from qmctorch.wavefunction.orbitals.backflow.kernels import BackFlowKernelInverse
 
 from torch.autograd import grad, gradcheck, Variable
@@ -52,15 +52,15 @@
         mol = Molecule(
             atom='Li 0 0 0; H 0 0 3.14',
             unit='bohr',
             calculator='pyscf',
             basis='sto-3g',
             redo_scf=True)
 
-        self.wf = SlaterCombinedJastrowBackflow(mol,
+        self.wf = SlaterManyBodyJastrowBackflow(mol,
                                                 kinetic='auto',
                                                 include_all_mo=False,
                                                 configs='single_double(2,2)',
                                                 jastrow_kernel={
                                                     'ee': PadeJastrowKernelElecElec,
                                                     'en': PadeJastrowKernelElecNuc,
                                                     'een': BoysHandyJastrowKernel},
```

### Comparing `qmctorch-0.2.0/tests/wavefunction/test_slaterjastrow.py` & `qmctorch-0.3.0/tests/wavefunction/test_slaterjastrow.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/tests/wavefunction/test_slaterjastrow_backflow.py` & `qmctorch-0.3.0/tests/wavefunction/test_slaterjastrow_backflow.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/tests/wavefunction/test_slaterjastrow_cas.py` & `qmctorch-0.3.0/tests/wavefunction/test_slaterjastrow_cas.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/tests/wavefunction/test_slaterjastrow_ee_cusp.py` & `qmctorch-0.3.0/tests/wavefunction/test_slaterjastrow_ee_cusp.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/tests/wavefunction/test_slaterjastrow_generic.py` & `qmctorch-0.3.0/tests/wavefunction/test_slaterjastrow_generic.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/tests/wavefunction/test_slaterjastrow_orbital_dependent_backflow.py` & `qmctorch-0.3.0/tests/wavefunction/test_slaterjastrow_orbital_dependent_backflow.py`

 * *Files identical despite different names*

### Comparing `qmctorch-0.2.0/tests_hvd/test_h2_hvd.py` & `qmctorch-0.3.0/tests_hvd/test_h2_hvd.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import numpy as np
 import torch
 import torch.optim as optim
 import horovod.torch as hvd
 from mpi4py import MPI
 
 from qmctorch.sampler import Metropolis
-from qmctorch.solver import SolverSlaterJastrowHorovod
+from qmctorch.solver import SolverMPI
 from qmctorch.scf import Molecule
 from qmctorch.wavefunction import SlaterJastrow
 from qmctorch.utils import set_torch_double_precision
 
 
 class TestH2Hvd(unittest.TestCase):
 
@@ -52,15 +52,15 @@
                 'type': 'all-elec',
                 'proba': 'normal'})
 
         # optimizer
         self.opt = optim.Adam(self.wf.parameters(), lr=0.01)
 
         # solver
-        self.solver = SolverSlaterJastrowHorovod(wf=self.wf, sampler=self.sampler,
+        self.solver = SolverMPI(wf=self.wf, sampler=self.sampler,
                                                  optimizer=self.opt, rank=hvd.rank())
 
         # ground state energy
         self.ground_state_energy = -1.16
 
         # ground state pos
         self.ground_state_pos = 0.69
```

### Comparing `qmctorch-0.2.0/tests_hvd/test_hvd.py` & `qmctorch-0.3.0/tests_hvd/test_hvd.py`

 * *Files identical despite different names*

