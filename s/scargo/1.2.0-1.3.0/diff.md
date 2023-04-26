# Comparing `tmp/scargo-1.2.0.tar.gz` & `tmp/scargo-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scargo-1.2.0.tar", last modified: Wed Apr 12 09:37:03 2023, max compression
+gzip compressed data, was "scargo-1.3.0.tar", last modified: Wed Apr 26 11:29:19 2023, max compression
```

## Comparing `scargo-1.2.0.tar` & `scargo-1.3.0.tar`

### file list

```diff
@@ -1,94 +1,95 @@
--rw-r--r--   0        0        0     4508 2023-04-12 09:36:58.133182 scargo-1.2.0/CODE-OF-CONDUCT.md
--rw-r--r--   0        0        0     1066 2023-04-12 09:36:58.133182 scargo-1.2.0/LICENSE
--rw-r--r--   0        0        0     2527 2023-04-12 09:36:58.133182 scargo-1.2.0/README.md
--rw-r--r--   0        0        0     2567 2023-04-12 09:36:58.257181 scargo-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      108 2023-04-12 09:36:58.257181 scargo-1.2.0/scargo/__init__.py
--rwxr-xr-x   0        0        0    19839 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/certs/certGen.sh
--rwxr-xr-x   0        0        0     4914 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/certs/generateAllCertificates.sh
--rw-r--r--   0        0        0     3967 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/certs/openssl_device_intermediate_ca.cnf
--rw-r--r--   0        0        0     3957 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/certs/openssl_root_ca.cnf
--rw-r--r--   0        0        0      914 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/clang_utils.py
--rw-r--r--   0        0        0    12538 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/cli.py
--rw-r--r--   0        0        0       86 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/commands/__init__.py
--rw-r--r--   0        0        0     1588 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/commands/build.py
--rw-r--r--   0        0        0    11335 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/commands/check.py
--rw-r--r--   0        0        0     1153 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/commands/clean.py
--rw-r--r--   0        0        0     4227 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/commands/debug.py
--rw-r--r--   0        0        0     3417 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/commands/doc.py
--rw-r--r--   0        0        0     3274 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/commands/docker.py
--rw-r--r--   0        0        0     1124 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/commands/fix.py
--rw-r--r--   0        0        0     3235 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/commands/flash.py
--rw-r--r--   0        0        0     6711 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/commands/gen.py
--rw-r--r--   0        0        0     3302 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/commands/new.py
--rw-r--r--   0        0        0     3352 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/commands/publish.py
--rw-r--r--   0        0        0     1688 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/commands/run.py
--rw-r--r--   0        0        0     3180 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/commands/test.py
--rw-r--r--   0        0        0     4361 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/commands/update.py
--rw-r--r--   0        0        0      228 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/commands/version.py
--rw-r--r--   0        0        0     6458 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/config.py
--rw-r--r--   0        0        0     2403 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/config_utils.py
--rw-r--r--   0        0        0     2185 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/docker_utils.py
--rw-r--r--   0        0        0       86 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/__init__.py
--rw-r--r--   0        0        0     1669 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/base_gen.py
--rw-r--r--   0        0        0      441 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/cicd_gen.py
--rw-r--r--   0        0        0      395 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/cmake_gen.py
--rw-r--r--   0        0        0      569 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/conan_gen.py
--rw-r--r--   0        0        0     2520 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/cpp_gen.py
--rw-r--r--   0        0        0     3186 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/docker_gen.py
--rw-r--r--   0        0        0     1115 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/env_gen.py
--rwxr-xr-x   0        0        0     5093 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/mock_gen.py
--rw-r--r--   0        0        0       86 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/mock_utils/__init__.py
--rw-r--r--   0        0        0     1663 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/mock_utils/cmake_utils.py
--rw-r--r--   0        0        0     2396 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/mock_utils/data_classes.py
--rw-r--r--   0        0        0      454 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/readme_gen.py
--rw-r--r--   0        0        0     4832 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/.gitlab-ci.yml.j2
--rw-r--r--   0        0        0     1580 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/CMakeLists.txt.j2
--rw-r--r--   0        0        0     4275 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/README.md.j2
--rw-r--r--   0        0        0     1693 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/conan/conanfile.py.j2
--rw-r--r--   0        0        0     1464 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/conan/conanfiletest.j2
--rw-r--r--   0        0        0      150 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/cpp/cmake-src-esp32.j2
--rw-r--r--   0        0        0     2415 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/cpp/cmake-src-stm32.j2
--rw-r--r--   0        0        0      886 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/cpp/cmake-src-x86.j2
--rw-r--r--   0        0        0      181 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/cpp/lib.cpp.j2
--rw-r--r--   0        0        0      213 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/cpp/lib.h.j2
--rw-r--r--   0        0        0      715 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/cpp/main.cpp.j2
--rw-r--r--   0        0        0      159 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/docker/Dockerfile-custom.j2
--rw-r--r--   0        0        0     2290 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/docker/Dockerfile-esp32.j2
--rw-r--r--   0        0        0     1251 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/docker/Dockerfile-stm32.j2
--rw-r--r--   0        0        0      236 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/docker/Dockerfile-x86.j2
--rw-r--r--   0        0        0     2348 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/docker/Dockerfile.j2
--rw-r--r--   0        0        0      158 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/docker/devcontainer.json.j2
--rw-r--r--   0        0        0     1000 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/docker/docker-compose.yaml.j2
--rw-r--r--   0        0        0      287 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/docker/env.txt.j2
--rw-r--r--   0        0        0       22 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/docker/stm32.cfg.j2
--rw-r--r--   0        0        0      294 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/esp32.cmake.j2
--rw-r--r--   0        0        0       39 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/mock/.clang-format
--rw-r--r--   0        0        0      475 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/mock/CMakeLists.txt
--rw-r--r--   0        0        0     1300 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/mock/class_interface.h.j2
--rw-r--r--   0        0        0     1058 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/mock/class_mock.cpp.j2
--rw-r--r--   0        0        0      697 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/mock/class_mock.h.j2
--rw-r--r--   0        0        0      510 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/project.cmake.j2
--rw-r--r--   0        0        0     2194 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/scargo.toml.j2
--rw-r--r--   0        0        0      802 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/stm32.cmake.j2
--rw-r--r--   0        0        0       91 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/tests/CMakeLists-it.txt.j2
--rw-r--r--   0        0        0      100 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/tests/CMakeLists-mocks.txt.j2
--rw-r--r--   0        0        0     1079 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/tests/CMakeLists-test.txt.j2
--rw-r--r--   0        0        0       84 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/tests/CMakeLists-ut.txt.j2
--rw-r--r--   0        0        0      326 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/tests/static_mock/CMakeLists.txt
--rw-r--r--   0        0        0     1046 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/tests/static_mock/static_mock.h
--rw-r--r--   0        0        0       39 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/ut/.clang-format
--rw-r--r--   0        0        0      575 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/ut/CMakeLists.txt.j2
--rw-r--r--   0        0        0      703 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/ut/ut.cpp.j2
--rw-r--r--   0        0        0      213 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/templates/x86.cmake.j2
--rw-r--r--   0        0        0     1698 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/tests_gen.py
--rw-r--r--   0        0        0      579 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/toml_gen.py
--rw-r--r--   0        0        0     6757 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/file_generators/ut_gen.py
--rw-r--r--   0        0        0      640 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/global_values.py
--rw-r--r--   0        0        0     2044 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/logger.py
--rw-r--r--   0        0        0     1144 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/path_utils.py
--rw-r--r--   0        0        0     2953 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/templates/.clang-format
--rw-r--r--   0        0        0     8780 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/templates/.clang-tidy
--rw-r--r--   0        0        0     2361 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/templates/.gitignore
--rw-r--r--   0        0        0     1066 2023-04-12 09:36:58.261181 scargo-1.2.0/scargo/templates/LICENSE
--rw-r--r--   0        0        0      515 2023-04-12 09:36:58.261181 scargo-1.2.0/setup.cfg
--rw-r--r--   0        0        0     5218 1970-01-01 00:00:00.000000 scargo-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     4508 2023-04-26 11:29:12.279526 scargo-1.3.0/CODE-OF-CONDUCT.md
+-rw-r--r--   0        0        0     1066 2023-04-26 11:29:12.283526 scargo-1.3.0/LICENSE
+-rw-r--r--   0        0        0     2488 2023-04-26 11:29:12.283526 scargo-1.3.0/README.md
+-rw-r--r--   0        0        0     2748 2023-04-26 11:29:12.419527 scargo-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      108 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/__init__.py
+-rwxr-xr-x   0        0        0    19839 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/certs/certGen.sh
+-rwxr-xr-x   0        0        0     4914 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/certs/generateAllCertificates.sh
+-rw-r--r--   0        0        0     3967 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/certs/openssl_device_intermediate_ca.cnf
+-rw-r--r--   0        0        0     3957 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/certs/openssl_root_ca.cnf
+-rw-r--r--   0        0        0      698 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/clang_utils.py
+-rw-r--r--   0        0        0    12631 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/cli.py
+-rw-r--r--   0        0        0       86 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/commands/__init__.py
+-rw-r--r--   0        0        0     1596 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/commands/build.py
+-rw-r--r--   0        0        0    12127 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/commands/check.py
+-rw-r--r--   0        0        0     1142 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/commands/clean.py
+-rw-r--r--   0        0        0     4205 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/commands/debug.py
+-rw-r--r--   0        0        0     3402 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/commands/doc.py
+-rw-r--r--   0        0        0     3382 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/commands/docker.py
+-rw-r--r--   0        0        0     1124 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/commands/fix.py
+-rw-r--r--   0        0        0     3226 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/commands/flash.py
+-rw-r--r--   0        0        0     6677 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/commands/gen.py
+-rw-r--r--   0        0        0     3319 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/commands/new.py
+-rw-r--r--   0        0        0     3405 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/commands/publish.py
+-rw-r--r--   0        0        0     1688 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/commands/run.py
+-rw-r--r--   0        0        0     3327 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/commands/test.py
+-rw-r--r--   0        0        0     4432 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/commands/update.py
+-rw-r--r--   0        0        0      228 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/commands/version.py
+-rw-r--r--   0        0        0     6578 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/config.py
+-rw-r--r--   0        0        0     2127 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/config_utils.py
+-rw-r--r--   0        0        0     2174 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/docker_utils.py
+-rw-r--r--   0        0        0       86 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/file_generators/__init__.py
+-rw-r--r--   0        0        0     1658 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/file_generators/base_gen.py
+-rw-r--r--   0        0        0      441 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/file_generators/cicd_gen.py
+-rw-r--r--   0        0        0       86 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/file_generators/clang_parser/__init__.py
+-rw-r--r--   0        0        0     2251 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/file_generators/clang_parser/data_classes.py
+-rw-r--r--   0        0        0     1197 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/file_generators/clang_parser/header_parser.py
+-rw-r--r--   0        0        0     2133 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/file_generators/clang_parser/params_extractor.py
+-rw-r--r--   0        0        0      395 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/file_generators/cmake_gen.py
+-rw-r--r--   0        0        0      569 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/file_generators/conan_gen.py
+-rw-r--r--   0        0        0     2468 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/file_generators/cpp_gen.py
+-rw-r--r--   0        0        0     3186 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/file_generators/docker_gen.py
+-rw-r--r--   0        0        0     1115 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/file_generators/env_gen.py
+-rwxr-xr-x   0        0        0     1607 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/file_generators/mock_gen.py
+-rw-r--r--   0        0        0      454 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/file_generators/readme_gen.py
+-rw-r--r--   0        0        0     4834 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/file_generators/templates/.gitlab-ci.yml.j2
+-rw-r--r--   0        0        0     1580 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/file_generators/templates/CMakeLists.txt.j2
+-rw-r--r--   0        0        0     4275 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/file_generators/templates/README.md.j2
+-rw-r--r--   0        0        0     1693 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/file_generators/templates/conan/conanfile.py.j2
+-rw-r--r--   0        0        0     1464 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/file_generators/templates/conan/conanfiletest.j2
+-rw-r--r--   0        0        0      150 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/file_generators/templates/cpp/cmake-src-esp32.j2
+-rw-r--r--   0        0        0     2423 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/file_generators/templates/cpp/cmake-src-stm32.j2
+-rw-r--r--   0        0        0      886 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/file_generators/templates/cpp/cmake-src-x86.j2
+-rw-r--r--   0        0        0      181 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/file_generators/templates/cpp/lib.cpp.j2
+-rw-r--r--   0        0        0      213 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/file_generators/templates/cpp/lib.h.j2
+-rw-r--r--   0        0        0      715 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/file_generators/templates/cpp/main.cpp.j2
+-rw-r--r--   0        0        0      159 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/file_generators/templates/docker/Dockerfile-custom.j2
+-rw-r--r--   0        0        0     2067 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/file_generators/templates/docker/Dockerfile-esp32.j2
+-rw-r--r--   0        0        0      754 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/file_generators/templates/docker/Dockerfile-stm32.j2
+-rw-r--r--   0        0        0       49 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/file_generators/templates/docker/Dockerfile-x86.j2
+-rw-r--r--   0        0        0     2359 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/file_generators/templates/docker/Dockerfile.j2
+-rw-r--r--   0        0        0      158 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/file_generators/templates/docker/devcontainer.json.j2
+-rw-r--r--   0        0        0     1000 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/file_generators/templates/docker/docker-compose.yaml.j2
+-rw-r--r--   0        0        0      287 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/file_generators/templates/docker/env.txt.j2
+-rw-r--r--   0        0        0       22 2023-04-26 11:29:12.419527 scargo-1.3.0/scargo/file_generators/templates/docker/stm32.cfg.j2
+-rw-r--r--   0        0        0      294 2023-04-26 11:29:12.423527 scargo-1.3.0/scargo/file_generators/templates/esp32.cmake.j2
+-rw-r--r--   0        0        0       39 2023-04-26 11:29:12.423527 scargo-1.3.0/scargo/file_generators/templates/mock/.clang-format
+-rw-r--r--   0        0        0      475 2023-04-26 11:29:12.423527 scargo-1.3.0/scargo/file_generators/templates/mock/CMakeLists.txt
+-rw-r--r--   0        0        0      594 2023-04-26 11:29:12.423527 scargo-1.3.0/scargo/file_generators/templates/mock/class_interface.h.j2
+-rw-r--r--   0        0        0      835 2023-04-26 11:29:12.423527 scargo-1.3.0/scargo/file_generators/templates/mock/class_mock.cpp.j2
+-rw-r--r--   0        0        0      697 2023-04-26 11:29:12.423527 scargo-1.3.0/scargo/file_generators/templates/mock/class_mock.h.j2
+-rw-r--r--   0        0        0      510 2023-04-26 11:29:12.423527 scargo-1.3.0/scargo/file_generators/templates/project.cmake.j2
+-rw-r--r--   0        0        0     2194 2023-04-26 11:29:12.423527 scargo-1.3.0/scargo/file_generators/templates/scargo.toml.j2
+-rw-r--r--   0        0        0      802 2023-04-26 11:29:12.423527 scargo-1.3.0/scargo/file_generators/templates/stm32.cmake.j2
+-rw-r--r--   0        0        0       91 2023-04-26 11:29:12.423527 scargo-1.3.0/scargo/file_generators/templates/tests/CMakeLists-it.txt.j2
+-rw-r--r--   0        0        0      100 2023-04-26 11:29:12.423527 scargo-1.3.0/scargo/file_generators/templates/tests/CMakeLists-mocks.txt.j2
+-rw-r--r--   0        0        0     1079 2023-04-26 11:29:12.423527 scargo-1.3.0/scargo/file_generators/templates/tests/CMakeLists-test.txt.j2
+-rw-r--r--   0        0        0       84 2023-04-26 11:29:12.423527 scargo-1.3.0/scargo/file_generators/templates/tests/CMakeLists-ut.txt.j2
+-rw-r--r--   0        0        0      326 2023-04-26 11:29:12.423527 scargo-1.3.0/scargo/file_generators/templates/tests/static_mock/CMakeLists.txt
+-rw-r--r--   0        0        0     1046 2023-04-26 11:29:12.423527 scargo-1.3.0/scargo/file_generators/templates/tests/static_mock/static_mock.h
+-rw-r--r--   0        0        0       39 2023-04-26 11:29:12.423527 scargo-1.3.0/scargo/file_generators/templates/ut/.clang-format
+-rw-r--r--   0        0        0      575 2023-04-26 11:29:12.423527 scargo-1.3.0/scargo/file_generators/templates/ut/CMakeLists.txt.j2
+-rw-r--r--   0        0        0      719 2023-04-26 11:29:12.423527 scargo-1.3.0/scargo/file_generators/templates/ut/ut.cpp.j2
+-rw-r--r--   0        0        0      213 2023-04-26 11:29:12.423527 scargo-1.3.0/scargo/file_generators/templates/x86.cmake.j2
+-rw-r--r--   0        0        0     1597 2023-04-26 11:29:12.423527 scargo-1.3.0/scargo/file_generators/tests_gen.py
+-rw-r--r--   0        0        0      560 2023-04-26 11:29:12.423527 scargo-1.3.0/scargo/file_generators/toml_gen.py
+-rw-r--r--   0        0        0     5357 2023-04-26 11:29:12.423527 scargo-1.3.0/scargo/file_generators/ut_gen.py
+-rw-r--r--   0        0        0      629 2023-04-26 11:29:12.423527 scargo-1.3.0/scargo/global_values.py
+-rw-r--r--   0        0        0     2044 2023-04-26 11:29:12.423527 scargo-1.3.0/scargo/logger.py
+-rw-r--r--   0        0        0     1137 2023-04-26 11:29:12.423527 scargo-1.3.0/scargo/path_utils.py
+-rw-r--r--   0        0        0     2953 2023-04-26 11:29:12.423527 scargo-1.3.0/scargo/templates/.clang-format
+-rw-r--r--   0        0        0     8780 2023-04-26 11:29:12.423527 scargo-1.3.0/scargo/templates/.clang-tidy
+-rw-r--r--   0        0        0     2361 2023-04-26 11:29:12.423527 scargo-1.3.0/scargo/templates/.gitignore
+-rw-r--r--   0        0        0     1066 2023-04-26 11:29:12.423527 scargo-1.3.0/scargo/templates/LICENSE
+-rw-r--r--   0        0        0      519 2023-04-26 11:29:12.423527 scargo-1.3.0/setup.cfg
+-rw-r--r--   0        0        0     5229 1970-01-01 00:00:00.000000 scargo-1.3.0/PKG-INFO
```

### Comparing `scargo-1.2.0/CODE-OF-CONDUCT.md` & `scargo-1.3.0/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `scargo-1.2.0/LICENSE` & `scargo-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scargo-1.2.0/README.md` & `scargo-1.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 - python3
 
 ## Working natively (not recommended, a lot of env setup)
 Base:
 
 - python >= 3.8
 - cmake >= 3.24.2
-- cppcheck bzr lib32z1 clang clang-format clang-tidy valgrind gcovr doxygen curl libcurl4-openssl-dev libcmocka0 libcmocka-dev
+- cppcheck lib32z1 clang clang-format clang-tidy gcovr doxygen libcmocka0 libcmocka-dev
 - lizard
 
 Depending on the architecture:
 
 - compiler (e.g. gcc-arm-none-eabi-9-2020-q2-update gcc-arm-none-eabi)
 - flashing tools
 - uC HAL and dependent files
```

### Comparing `scargo-1.2.0/pyproject.toml` & `scargo-1.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dynamic = ["version"]
 keywords = ["scargo", "Package manager", "C++"]
 dependencies = [
-    "clang==14.0",
+    "clang==16.0.1.1",
     "cmake==3.25.2",
     "coloredlogs==15.0.1",
     "conan==1.59.0",
     "docker==6.0.1",
     "esptool==4.5.1",
     "jinja2==3.1.2",
     "libclang==16.0.0",
@@ -42,33 +42,34 @@
     "toml==0.10.2",
     "tomlkit==0.11.6",
     "typer==0.7.0",
 ]
 
 [project.optional-dependencies]
 dev = [
-    "allure-pytest",
     "black",
     "coverage~=6.0",
     "flake8>=3.2.0",
     "flit==3.8.0",
     "gcovr>=5.2",
     "isort==5.11.4",
+    "matplotlib",
     "mypy==1.0.1",
     "pre-commit",
     "pyclean==2.2.0",
     "pyelftools",
+    "pyfakefs",
     "PyInstaller",
     "pylint",
     "pytest-bdd",
     "pytest-cov",
     "pytest-mock",
     "pytest-subprocess",
     "pytest",
-    "types-clang",
+    "types-clang==0.14.3",
     "types-toml",
     "unittest-xml-reporting",
 ]
 doc = [
     "recommonmark",
     "sphinx-rtd-theme==1.1.1",
     "Sphinx",
@@ -107,7 +108,15 @@
 [[tool.mypy.overrides]]
 module = "coloredlogs"
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = "docker"
 ignore_missing_imports = true
+
+[[tool.mypy.overrides]]
+module = "matplotlib.*"
+ignore_missing_imports = true
+
+[[tool.mypy.overrides]]
+module = "pyfakefs.*"
+ignore_missing_imports = true
```

### Comparing `scargo-1.2.0/scargo/certs/certGen.sh` & `scargo-1.3.0/scargo/certs/certGen.sh`

 * *Files identical despite different names*

### Comparing `scargo-1.2.0/scargo/certs/generateAllCertificates.sh` & `scargo-1.3.0/scargo/certs/generateAllCertificates.sh`

 * *Files identical despite different names*

### Comparing `scargo-1.2.0/scargo/certs/openssl_device_intermediate_ca.cnf` & `scargo-1.3.0/scargo/certs/openssl_device_intermediate_ca.cnf`

 * *Files identical despite different names*

### Comparing `scargo-1.2.0/scargo/certs/openssl_root_ca.cnf` & `scargo-1.3.0/scargo/certs/openssl_root_ca.cnf`

 * *Files identical despite different names*

### Comparing `scargo-1.2.0/scargo/cli.py` & `scargo-1.3.0/scargo/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,15 +351,15 @@
         name,
         bin_name,
         lib_name,
         Target.get_target_by_id(target.value),
         create_docker,
         git,
     )
-    scargo_update(Path(SCARGO_DEFAULT_CONFIG_FILE).absolute())
+    scargo_update(Path(name, SCARGO_DEFAULT_CONFIG_FILE).absolute())
 
 
 ###############################################################################
 
 
 @cli.command()
 def publish(
@@ -401,20 +401,21 @@
 
 ###############################################################################
 
 
 @cli.command()
 def test(
     verbose: bool = Option(False, "--verbose", "-v", help="Verbose mode."),
+    profile: str = Option("Debug", "--profile", help="CMake profile to use"),
     base_dir: Optional[Path] = BASE_DIR_OPTION,
 ) -> None:
     """Compile and run all tests in directory `test`."""
     if base_dir:
         os.chdir(base_dir)
-    scargo_test(verbose)
+    scargo_test(verbose, profile)
 
 
 ###############################################################################
 
 
 @cli.command()
 def update(
```

### Comparing `scargo-1.2.0/scargo/commands/build.py` & `scargo-1.3.0/scargo/commands/build.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         sys.exit(1)
 
     build_dir = Path(project_dir, "build", profile)
     build_dir.mkdir(parents=True, exist_ok=True)
 
     conan_clean_remote()
 
-    conan_add_remote(project_dir)
+    conan_add_remote(project_dir, config)
     conan_add_conancenter()
 
     try:
         subprocess.check_call(
             ["conan", "install", ".", "-if", build_dir],
             cwd=project_dir,
         )
```

### Comparing `scargo-1.2.0/scargo/commands/check.py` & `scargo-1.3.0/scargo/commands/check.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,16 +72,28 @@
             CopyrightChecker,
             CppcheckChecker,
             CyclomaticChecker,
             PragmaChecker,
             TodoChecker,
         ]
 
+    problem_counts = []
     for checker_class in checkers:
-        checker_class(config, verbose=verbose).check()
+        problem_count = checker_class(config, verbose=verbose).check()
+        problem_counts.append((checker_class, problem_count))
+    if len(checkers) > 1:
+        logger.info("Summary:")
+        if any(count > 0 for _, count in problem_counts):
+            for checker_class, problem_count in problem_counts:
+                logger.info(
+                    f"{checker_class.check_name}: {problem_count} problems found"
+                )
+            sys.exit(1)
+        else:
+            logger.info("No problems found!")
 
 
 class CheckResult(NamedTuple):
     problems_found: int
     fix: bool = True
 
 
@@ -93,23 +105,24 @@
     def __init__(
         self, config: Config, fix_errors: bool = False, verbose: bool = False
     ) -> None:
         self._config = config
         self._fix_errors = fix_errors
         self._verbose = verbose
 
-    def check(self) -> None:
+    def check(self) -> int:
         logger.info(f"Starting {self.check_name} check...")
         error_count = self.check_files()
         self.report(error_count)
+        return error_count
 
     def check_files(self) -> int:
         error_counter = 0
         for file_path in find_files(
-            Path(self._config.project.target.source_dir),
+            self._config.source_dir_path,
             ("*.h", "*.hpp") if self.headers_only else ("*.h", "*.hpp", "*.c", "*.cpp"),
             self.get_exclude_patterns(),
         ):
             result = self.check_file(file_path)
             error_counter += result.problems_found
             if (
                 result.problems_found > 0
@@ -125,15 +138,14 @@
         problem_count = self.format_problem_count(count)
         if self._fix_errors and self.can_fix:
             logger.info(f"Finished {self.check_name} check. Fixed {problem_count}.")
         else:
             logger.info(f"Finished {self.check_name} check. Found {problem_count}.")
             if count > 0:
                 logger.error(f"{self.check_name} check fail!")
-                sys.exit(1)
 
     @staticmethod
     def format_problem_count(count: int) -> str:
         return f"problems in {count} files"
 
     def get_exclude_patterns(self) -> List[str]:
         return [*self._config.check.exclude, *self.get_check_config().exclude]
@@ -157,15 +169,15 @@
     can_fix = True
 
     def check_file(self, file_path: Path) -> CheckResult:
         with open(file_path, encoding="utf-8") as file:
             for line in file.readlines():
                 if "#pragma once" in line:
                     return CheckResult(0)
-        logger.warning("Missing pragma in %s", file_path)
+        logger.warning("Missing '#pragma once' in %s", file_path)
         return CheckResult(1)
 
     def fix_file(self, file_path: Path) -> None:
         with open(file_path, encoding="utf-8") as file:
             old = file.read()
 
         with open(file_path, "w", encoding="utf-8") as file:
@@ -178,43 +190,55 @@
     check_name = "copyright"
     can_fix = True
 
     def __init__(self, config: Config, fix_errors: bool = False, verbose: bool = False):
         super().__init__(config, fix_errors, verbose)
         self.copyright_desc = self.get_check_config().description or ""
 
-    def check(self) -> None:
+    def check(self) -> int:
         if not self.copyright_desc:
-            logger.warning("No copyrights in defined in toml")
-            return
-        super().check()
+            logger.warning(
+                "No copyright line defined in scargo.toml at check.copyright.description"
+            )
+            return 0
+        return super().check()
+
+    def __get_copyright_lines(self) -> List[str]:
+        return (
+            ["//\n"]
+            + [f"// {el}\n" for el in self.copyright_desc.split("\n")]
+            + ["//\n"]
+        )
 
     def check_file(self, file_path: Path) -> CheckResult:
+        copyright_lines = self.__get_copyright_lines()
+
         with open(file_path, encoding="utf-8") as file:
-            for line in file.readlines():
-                if self.copyright_desc in line:
-                    return CheckResult(problems_found=0)
-                if "copyright" in line.lower():
-                    logger.warning(
-                        "Incorrect and not excluded copyright in %s", file_path
-                    )
-                    return CheckResult(problems_found=1, fix=False)
-        logger.info("Missing copyright in %s.", file_path)
+            file_lines = file.readlines()
+
+            for line_no, line in enumerate(file_lines[: -(len(copyright_lines) - 1)]):
+                if line == copyright_lines[0]:
+                    if all(
+                        line_from_file == line_from_copyrights
+                        for line_from_file, line_from_copyrights in zip(
+                            file_lines[line_no:], copyright_lines
+                        )
+                    ):
+                        return CheckResult(problems_found=0)
+
+        logger.warning("Missing copyright line in %s.", file_path)
         return CheckResult(problems_found=1)
 
     def fix_file(self, file_path: Path) -> None:
         with open(file_path, encoding="utf-8") as file:
             old = file.read()
 
         with open(file_path, "w", encoding="utf-8") as file:
-            file.write("//\n")
-            for line in self.copyright_desc.split("\n"):
-                if line != "":
-                    file.write(f"// {line}\n")
-            file.write("//\n")
+            for line in self.__get_copyright_lines():
+                file.write(line)
             file.write("\n")
             file.write(old)
 
 
 class TodoChecker(CheckerFixer):
     check_name = "todo"
 
@@ -308,42 +332,40 @@
             yield file_path
 
 
 class CyclomaticChecker(CheckerFixer):
     check_name = "cyclomatic"
 
     def check_files(self) -> int:
-        source_dir = self._config.project.target.source_dir
-
-        cmd = ["lizard", source_dir, "-C", "25", "-w"]
+        cmd = ["lizard", str(self._config.source_dir_path), "-C", "25", "-w"]
 
         for exclude_pattern in self.get_exclude_patterns():
             cmd.extend(["--exclude", exclude_pattern])
         try:
             subprocess.check_call(cmd)
         except subprocess.CalledProcessError:
-            logger.error(f"ERROR: Check {self.check_name} fail")
+            logger.error(f"{self.check_name} fail!")
         return 0
 
     def report(self, count: int) -> None:
         logger.info(f"Finished {self.check_name} check.")
 
     def check_file(self, file_path: Path) -> CheckResult:
         raise NotImplementedError
 
 
 class CppcheckChecker(CheckerFixer):
     check_name = "cppcheck"
 
     def check_files(self) -> int:
-        cmd = "cppcheck --enable=all --suppress=missingIncludeSystem src/ main/"
+        cmd = "cppcheck --enable=all --suppress=missingIncludeSystem --inline-suppr src/ main/"
         try:
             subprocess.check_call(cmd, shell=True)
         except subprocess.CalledProcessError:
-            logger.error(f"{self.check_name} fail")
+            logger.error(f"{self.check_name} fail!")
         return 0
 
     def report(self, count: int) -> None:
         logger.info(f"Finished {self.check_name} check.")
 
     def check_file(self, file_path: Path) -> CheckResult:
         raise NotImplementedError
```

### Comparing `scargo-1.2.0/scargo/commands/clean.py` & `scargo-1.3.0/scargo/commands/clean.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 logger = get_logger()
 
 
 def _case_insensitive_find_dir(source_dir: Path, dirname: str) -> Optional[Path]:
     if source_dir and source_dir.exists():
         for child in source_dir.iterdir():
             if child.name.lower() == dirname.lower():
-                return child.absolute()
+                return child
     return None
 
 
 def scargo_clean() -> None:
     """Clean project dir from unnecessary files"""
 
     config = get_scargo_config_or_exit()
```

### Comparing `scargo-1.2.0/scargo/commands/debug.py` & `scargo-1.3.0/scargo/commands/debug.py`

 * *Files 13% similar despite different names*

```diff
@@ -102,17 +102,17 @@
             "-f",
             "board/esp-wroom-32.cfg",
         ]
         self._debug_embedded(openocd_args, "xtensa-esp32-elf-gdb")
 
     def _get_bin_path(self, bin_name: str) -> Path:
         if self._target.family == "esp32":
-            bin_path = Path(self._project_root, "build/Debug", bin_name).absolute()
+            bin_path = Path(self._project_root, "build/Debug", bin_name)
         else:
-            bin_path = Path(self._project_root, "build/Debug/bin", bin_name).absolute()
+            bin_path = Path(self._project_root, "build/Debug/bin", bin_name)
         if self._target.family in ("stm32", "esp32") and bin_path.suffix != "elf":
             bin_path = bin_path.with_suffix(".elf")
         return bin_path
 
 
 def scargo_debug(bin_path: Optional[Path]) -> None:
     config = prepare_config(run_in_docker=False)
```

### Comparing `scargo-1.2.0/scargo/commands/doc.py` & `scargo-1.3.0/scargo/commands/doc.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,65 +2,66 @@
 # @copyright Copyright (C) 2023 SpyroSoft Solutions S.A. All rights reserved.
 # #
 
 """Create project documentation"""
 import subprocess
 import sys
 from pathlib import Path
+from typing import Iterable
 
 import typer
 
 from scargo.config import Config
 from scargo.config_utils import prepare_config
 from scargo.logger import get_logger
 from scargo.path_utils import find_program_path
 
 logger = get_logger()
 
 
 class _ScargoGenDoc:
     EXCLUDE_LIST = ["build"]
 
-    def __init__(self, config: Config, doxygen_path: Path, doc_dir_path: Path):
+    def __init__(self, config: Config, doc_dir_path: Path):
         self._config = config
-        self._doxygen_path = doxygen_path
         self._doc_dir_path = doc_dir_path
 
     def create_default_doxyfile(self) -> None:
         """Create default doxyfile"""
         subprocess.check_call("doxygen -g", shell=True, cwd=self._doc_dir_path)
 
     def update_doxyfile(self) -> None:
         """Update Doxyfile configuration according specified values"""
+        doxyfile_path = self._doc_dir_path / "Doxyfile"
+        with doxyfile_path.open(encoding="utf-8") as doxyfile:
+            doxyfile_lines = doxyfile.readlines()
+
+        with doxyfile_path.open("w", encoding="utf-8") as doxyfile:
+            doxyfile.writelines(self.adjust_doxyfile_lines(doxyfile_lines))
+
+    def adjust_doxyfile_lines(self, lines: Iterable[str]) -> Iterable[str]:
         project_name = self._config.project.name
         project_path = self._config.project_root
         exclude = " ".join(
             f"{project_path}/{dir}"
             for dir in self.EXCLUDE_LIST + self._config.doc.exclude
         )
-
         doxy_values = {
             "PROJECT_NAME": f'"{project_name}"',
             "EXTRACT_ALL": "YES",
             "INPUT": project_path,
             "RECURSIVE": "YES",
             "EXCLUDE_PATTERNS": exclude,
             "GENERATE_LATEX": "NO",
         }
-
-        doxyfile_path = self._doc_dir_path / "Doxyfile"
-        with doxyfile_path.open(encoding="utf-8") as doxyfile:
-            rewrite_file = doxyfile.readlines()
-            for i, line in enumerate(rewrite_file):
-                for key, value in doxy_values.items():
-                    if line.startswith(f"{key} "):
-                        rewrite_file[i] = f"{key.ljust(23)}= {value}\n"
-
-        with doxyfile_path.open("w", encoding="utf-8") as doxyfile:
-            doxyfile.writelines(rewrite_file)
+        for line in lines:
+            key = line.split(" ", 1)[0]
+            if key in doxy_values:
+                yield f"{key.ljust(23)}= {doxy_values[key]}\n"
+            yield line
 
     def generate_doxygen(self) -> None:
         """Generate doxygen according to doxyfile"""
         subprocess.check_call("doxygen", shell=True, cwd=self._doc_dir_path)
 
 
 def _open_doc(doc_dir_path: Path) -> None:
@@ -85,22 +86,21 @@
     """
     config = prepare_config()
     doc_dir_path = config.project_root / "build/doc"
     if open_doc:
         _open_doc(doc_dir_path)
         sys.exit(0)
 
-    doxygen_path = find_program_path("doxygen")
-    if not doxygen_path:
+    if not find_program_path("doxygen"):
         logger.error("Doxygen not installed or not in PATH environment variable")
         sys.exit(1)
 
     doc_dir_path.mkdir(parents=True, exist_ok=True)
 
     try:
-        scargo_doc_gen = _ScargoGenDoc(config, doxygen_path, doc_dir_path)
+        scargo_doc_gen = _ScargoGenDoc(config, doc_dir_path)
         scargo_doc_gen.create_default_doxyfile()
         scargo_doc_gen.update_doxyfile()
         scargo_doc_gen.generate_doxygen()
 
     except subprocess.CalledProcessError:
         logger.error("Fail to create project documentation")
```

### Comparing `scargo-1.2.0/scargo/commands/docker.py` & `scargo-1.3.0/scargo/commands/docker.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,25 +12,29 @@
 
 from scargo.config_utils import get_scargo_config_or_exit
 from scargo.logger import get_logger
 
 logger = get_logger()
 
 
-def scargo_docker_build(docker_opts: Sequence[str]) -> None:
+def scargo_docker_build(
+    docker_opts: Sequence[str], project_root: Optional[Path] = None
+) -> None:
     """
     Build docker
 
     :param docker_opts: additional docker options
+    :param project_root
     :raises CalledProcessError: if docker build fail
     """
     logger.debug("Build docker environment.")
 
-    config = get_scargo_config_or_exit()
-    docker_path = _get_docker_path(config.project_root)
+    if not project_root:
+        project_root = get_scargo_config_or_exit().project_root
+    docker_path = _get_docker_path(project_root)
 
     try:
         subprocess.run(
             ["docker-compose", "build", *docker_opts], cwd=docker_path, check=True
         )
         logger.info("Initialize docker environment.")
     except subprocess.CalledProcessError:
```

### Comparing `scargo-1.2.0/scargo/commands/fix.py` & `scargo-1.3.0/scargo/commands/fix.py`

 * *Files identical despite different names*

### Comparing `scargo-1.2.0/scargo/commands/flash.py` & `scargo-1.3.0/scargo/commands/flash.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # #
 # @copyright Copyright (C) 2023 SpyroSoft Solutions S.A. All rights reserved.
 # #
 
 import subprocess
 import sys
-from pathlib import Path
 from typing import Optional
 
 from scargo.config import Config
 from scargo.config_utils import prepare_config
 from scargo.logger import get_logger
 
 logger = get_logger()
@@ -52,15 +51,15 @@
                 "--partition-name=ota_0",
                 f"--input={app_path}",
             ]
             if port:
                 command.append(f"--port={port}")
             subprocess.check_call(command, cwd=project_path)
         elif fs:
-            fs_path = Path("build") / "spiffs.bin"
+            fs_path = config.project_root / "build" / "spiffs.bin"
             command = [
                 "parttool.py",
                 "write_partition",
                 "--partition-name=spiffs",
                 f"--input={fs_path}",
             ]
             if port:
```

### Comparing `scargo-1.2.0/scargo/commands/gen.py` & `scargo-1.3.0/scargo/commands/gen.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     if gen_ut:
         generate_ut(gen_ut, config)
 
     if gen_mock:
         if gen_mock.suffix not in (".h", ".hpp"):
             logger.error("Not a header file. Please chose .h or .hpp file.")
             sys.exit(1)
-        if generate_mocks(gen_mock, config.project.target.source_dir, config):
+        if generate_mocks(gen_mock, config):
             logger.info(f"Generated: {gen_mock}")
         else:
             logger.info(f"Skipping: {gen_mock}")
 
     if certs:
         generate_certs(
             certs, certs_mode, certs_input, certs_passwd, config.project_root
```

### Comparing `scargo-1.2.0/scargo/commands/new.py` & `scargo-1.3.0/scargo/commands/new.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # #
 # @copyright Copyright (C) 2023 SpyroSoft Solutions S.A. All rights reserved.
 # #
 
 """Create new project"""
-import os
 import re
 import subprocess
 import sys
 from pathlib import Path
 from typing import Optional, Tuple
 
 from scargo import __version__
@@ -49,50 +48,50 @@
         sys.exit(1)
 
     # If neither binary target nor library target is specified then create a
     # binary target named same as the project name.
     if not bin_name and not lib_name:
         bin_name = name  # One item tuple.
 
+    project_dir = Path(name)
     try:
-        project_dir = Path(name)
         project_dir.mkdir()
-        os.chdir(project_dir)
     except FileExistsError:
         logger.error("Provided project name: %s already exist.", name)
         sys.exit(1)
 
     build_env = get_build_env(create_docker)
 
     cc, cflags, cxx, cxxflags = get_cc_config(target)
+    toml_path = project_dir / SCARGO_DEFAULT_CONFIG_FILE
     generate_toml(
-        SCARGO_DEFAULT_CONFIG_FILE,
+        toml_path,
         project_name=name,
         target=target,
         build_env=build_env,
         cc=cc,
         cxx=cxx,
         cflags=cflags,
         cxxflags=cxxflags,
         version=__version__,
         docker_image_tag=f"{name.lower()}-dev:1.0",
         lib_name=lib_name,
         bin_name=bin_name,
     )
 
-    config = get_scargo_config_or_exit(Path("scargo.toml"))
+    config = get_scargo_config_or_exit(toml_path)
     generate_cpp(config)
 
-    test_dir = "tests"
+    test_dir = project_dir / "tests"
     Path(test_dir, "mocks").mkdir(parents=True)
     Path(test_dir, "ut").mkdir(parents=True)
     Path(test_dir, "it").mkdir(parents=True)
 
     if git:
-        subprocess.check_call("git init -q", shell=True)
+        subprocess.check_call("git init -q", shell=True, cwd=project_dir)
         logger.info("Initialized git repo")
 
 
 def get_cc_config(target: Target) -> Tuple[str, str, str, str]:
     """
     Get c configuration base on architecture
```

### Comparing `scargo-1.2.0/scargo/commands/publish.py` & `scargo-1.3.0/scargo/commands/publish.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 """Publish conan package into repository"""
 import os
 import subprocess
 import sys
 from pathlib import Path
 
+from scargo.config import Config
 from scargo.config_utils import prepare_config
 from scargo.logger import get_logger
 
 logger = get_logger()
 
 
 def scargo_publish(repo: str) -> None:
@@ -25,15 +26,15 @@
     config = prepare_config()
     project_path = config.project_root
     project_config = config.project
     project_name = project_config.name
     version = project_config.version
 
     conan_clean_remote()
-    conan_add_remote(project_path)
+    conan_add_remote(project_path, config)
     conan_add_conancenter()
 
     # Export package
     try:
         subprocess.check_call(
             "conan export-pkg . -f",
             cwd=project_path,
@@ -57,22 +58,22 @@
             cwd=project_path,
         )
     except subprocess.CalledProcessError:
         logger.error("Unable to publish package")
         sys.exit(1)
 
 
-def conan_add_remote(project_path: Path) -> None:
+def conan_add_remote(project_path: Path, config: Config) -> None:
     """
     Add conan remote repository
 
     :param Path project_path: path to project
+    :param Config config:
     :return: None
     """
-    config = prepare_config()
     conan_repo = config.conan.repo
     for repo_name, repo_url in conan_repo.items():
         try:
             subprocess.check_call(
                 ["conan", "remote", "add", repo_name, repo_url],
                 cwd=project_path,
             )
```

### Comparing `scargo-1.2.0/scargo/commands/run.py` & `scargo-1.3.0/scargo/commands/run.py`

 * *Files identical despite different names*

### Comparing `scargo-1.2.0/scargo/commands/test.py` & `scargo-1.3.0/scargo/commands/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,18 +11,19 @@
 from scargo.config import Config
 from scargo.config_utils import prepare_config
 from scargo.logger import get_logger
 
 logger = get_logger()
 
 
-def scargo_test(verbose: bool) -> None:
+def scargo_test(verbose: bool, profile: str = "Debug") -> None:
     """
     Run test
     :param bool verbose: if verbose
+    :param str profile: CMake profile to use
     """
     config = prepare_config()
 
     test_dir_name = "tests"
     project_dir = config.project_root
     tests_src_dir = project_dir / test_dir_name
     test_build_dir = project_dir / "build" / test_dir_name
@@ -41,16 +42,19 @@
     try:
         # Run CMake and build tests.
         subprocess.check_call(
             ["conan", "install", tests_src_dir, "-if", test_build_dir],
             cwd=project_dir,
         )
         subprocess.check_call(
-            ["conan", "build", tests_src_dir, "-bf", test_build_dir],
-            cwd=project_dir,
+            ["cmake", f"-DCMAKE_BUILD_TYPE={profile}", tests_src_dir],
+            cwd=test_build_dir,
+        )
+        subprocess.check_call(
+            "cmake --build . --parallel", shell=True, cwd=test_build_dir
         )
     except subprocess.CalledProcessError:
         logger.error("Failed to build tests.")
         sys.exit(1)
 
     # run ut
     run_ut(config, verbose, test_build_dir)
@@ -70,15 +74,15 @@
         # Run code coverage.
         cmd = [
             "gcovr",
             "-r",
             "ut",
             ".",
             "-f",
-            config.project_root.joinpath(config.project.target.source_dir),
+            config.source_dir_path,
             "--html",
             "ut-coverage.html",
         ]
 
         gcov_executable = config.tests.gcov_executable
 
         if gcov_executable != "":
```

### Comparing `scargo-1.2.0/scargo/commands/update.py` & `scargo-1.3.0/scargo/commands/update.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """Update project"""
 import shutil
 import subprocess
 import sys
 from pathlib import Path
 
 from scargo.commands.docker import scargo_docker_build
-from scargo.config_utils import check_scargo_version, get_scargo_config_or_exit
+from scargo.config_utils import add_version_to_scargo_lock, get_scargo_config_or_exit
 from scargo.file_generators.cicd_gen import generate_cicd
 from scargo.file_generators.cmake_gen import generate_cmake
 from scargo.file_generators.conan_gen import generate_conanfile
 from scargo.file_generators.docker_gen import generate_docker_compose
 from scargo.file_generators.env_gen import generate_env
 from scargo.file_generators.readme_gen import generate_readme
 from scargo.file_generators.tests_gen import generate_tests
@@ -55,30 +55,30 @@
         )
         sys.exit(1)
 
     # Copy templates project files to repo directory
     copy_file_if_not_exists(project_path)
 
     # Copy config file and create lock file.
-    shutil.copyfile(config_file_path, project_path / SCARGO_LOCK_FILE)
+    lock_path = project_path / SCARGO_LOCK_FILE
+    shutil.copyfile(config_file_path, lock_path)
     ###########################################################################
-    config = get_scargo_config_or_exit()
-    check_scargo_version(config)
+    add_version_to_scargo_lock(lock_path)
     project_config = config.project
     target = project_config.target
 
     # Copy docker env files to repo directory
     generate_docker_compose(docker_path, config)
     generate_env(docker_path, config)
 
     generate_cmake(config)
     generate_conanfile(config)
 
     if target.family == "esp32":
-        Path(target.source_dir, "fs").mkdir(parents=True, exist_ok=True)
+        Path(config.source_dir_path, "fs").mkdir(parents=True, exist_ok=True)
         with open(Path(project_path, "version.txt"), "w", encoding="utf-8") as out:
             out.write(project_config.version)
         with open(Path(project_path, "partitions.csv"), "w", encoding="utf-8") as out:
             out.write(
                 "# ESP-IDF Partition Table\n# Name,   Type, SubType, Offset,  Size, Flags\n"
             )
             partitions = config.get_esp32_config().partitions
@@ -87,21 +87,24 @@
             out.write("\n")
 
     generate_cicd(config=config)
     generate_tests(config)
     generate_readme(config)
 
     # do not rebuild dockers in the docker
-    if target.family == "stm32" and not Path("third-party/stm32-cmake").is_dir():
+    if (
+        target.family == "stm32"
+        and not Path(config.project_root, "third-party/stm32-cmake").is_dir()
+    ):
         subprocess.run("conan source .", shell=True, cwd=project_path, check=True)
 
     if project_config.build_env == SCARGO_DOCKER_ENV:
         if not Path(project_path, ".dockerenv").exists():
             if not pull_docker_image(docker_path):
-                scargo_docker_build([])
+                scargo_docker_build([], config.project_root)
         else:
             logger.warning("Cannot run docker inside docker")
 
 
 def pull_docker_image(docker_path: Path) -> bool:
     logger.info("Pulling the image from docker registry...")
     try:
```

### Comparing `scargo-1.2.0/scargo/config.py` & `scargo-1.3.0/scargo/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,18 @@
     )
     docker_compose: "DockerComposeConfig" = Field(
         default_factory=lambda: DockerComposeConfig(),  # pylint: disable=unnecessary-lambda
         alias="docker-compose",
     )
     project_root: Path
 
+    @property
+    def source_dir_path(self) -> Path:
+        return self.project_root / self.project.target.source_dir
+
     def get_stm32_config(self) -> "Stm32Config":
         if not self.stm32:
             raise ConfigError("No [stm32] section in config")
         return self.stm32
 
     def get_esp32_config(self) -> "Esp32Config":
         if not self.esp32:
```

### Comparing `scargo-1.2.0/scargo/config_utils.py` & `scargo-1.3.0/scargo/config_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -52,30 +52,22 @@
     """
     Check scargo version
 
     :param Config config: project configuration
     :return: None
     """
     version_lock = config.scargo.version
-    if not version_lock:
-        add_version_to_scargo_lock()
-    elif __version__ != version_lock:
+    if __version__ != version_lock:
         logger.warning("Warning: scargo package is different then in lock file")
         logger.info("Run scargo update")
 
 
-def add_version_to_scargo_lock() -> None:
+def add_version_to_scargo_lock(scargo_lock: Path) -> None:
     """
     :return: project configuration as dict
     """
-    scargo_lock = get_config_file_path(SCARGO_LOCK_FILE)
-    if not scargo_lock:
-        logger.error("ERROR: File `%s` does not exist.", SCARGO_LOCK_FILE)
-        logger.info("Did you run `scargo update`?")
-        sys.exit(1)
-
     with open(scargo_lock, encoding="utf-8") as scargo_lock_file:
         config = tomlkit.load(scargo_lock_file)
 
     config.setdefault("scargo", tomlkit.table())["version"] = __version__
     with open(scargo_lock, "w", encoding="utf-8") as scargo_lock_file:
         tomlkit.dump(config, scargo_lock_file)
```

### Comparing `scargo-1.2.0/scargo/docker_utils.py` & `scargo-1.3.0/scargo/docker_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     :param dict project_config: project configuration
     :param Path project_path: path to project root
     :return: None
     """
     build_env = project_config.build_env
     if build_env != SCARGO_DOCKER_ENV or Path("/.dockerenv").exists():
         return
-    relative_path = Path.cwd().absolute().relative_to(project_path)
+    relative_path = Path.cwd().relative_to(project_path)
     path_in_docker = Path("/workspace", relative_path)
 
     cmd_args = sys.argv[1:]
 
     entrypoint = ""
     if project_config.target.family == "esp32":
         entrypoint = "/opt/esp/entrypoint.sh"
```

### Comparing `scargo-1.2.0/scargo/file_generators/base_gen.py` & `scargo-1.3.0/scargo/file_generators/base_gen.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,8 +48,8 @@
     output_path.write_text(content, encoding="utf-8")
 
     logger.info("Generated %s", output_path)
 
 
 def _is_file_excluded(output_path: Path, project_path: Path, config: Config) -> bool:
     exclude_list = config.scargo.update_exclude
-    return str(output_path.absolute().relative_to(project_path)) in exclude_list
+    return str(output_path.relative_to(project_path)) in exclude_list
```

### Comparing `scargo-1.2.0/scargo/file_generators/conan_gen.py` & `scargo-1.3.0/scargo/file_generators/conan_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.2.0/scargo/file_generators/cpp_gen.py` & `scargo-1.3.0/scargo/file_generators/cpp_gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # #
 # @copyright Copyright (C) 2023 SpyroSoft Solutions S.A. All rights reserved.
 # #
-from pathlib import Path
 from typing import Any, Dict
 
 from scargo.config import Config
 from scargo.file_generators.base_gen import create_file_from_template
 
 
 class _CppTemplateGen:
     """
     This class is a container cpp files creation with multilayer approach
     """
 
     def __init__(self, config: Config) -> None:
         self._config = config
-        self._src_dir = Path(config.project.target.source_dir).absolute()
+        self._src_dir = config.source_dir_path
 
     def _generate_bin(self, bin_name: str) -> None:
         """Function which creates main.cpp file using jinja"""
         self._create_file_from_template(
             "cpp/main.cpp.j2",
             f"{bin_name.lower()}.cpp",
             template_params={
```

### Comparing `scargo-1.2.0/scargo/file_generators/docker_gen.py` & `scargo-1.3.0/scargo/file_generators/docker_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.2.0/scargo/file_generators/env_gen.py` & `scargo-1.3.0/scargo/file_generators/env_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.2.0/scargo/file_generators/mock_utils/data_classes.py` & `scargo-1.3.0/scargo/file_generators/clang_parser/data_classes.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # #
 # @copyright Copyright (C) 2023 SpyroSoft Solutions S.A. All rights reserved.
 # #
-from typing import Any, List, Sequence
+from typing import List, Sequence
 
 
 class ArgumentDescriptor:
     """Describes a function argument"""
 
     def __init__(self, name: str, data_type: str):
         self.name = name
         self.data_type = data_type
 
 
-class MockFunctionDescriptor:
+class FunctionDescriptor:
     """Contains function name and types"""
 
     def __init__(
         self,
         name: str,
         return_type: str,
         specifiers: Sequence[str],
@@ -46,34 +46,40 @@
     def get_arg_types(self) -> str:
         for arg in self.arguments:
             if arg.data_type == "void":
                 return " "
         return ", ".join(arg.data_type for arg in self.arguments)
 
 
-class MockClassDescriptor:
+class ClassDescriptor:
     """Contains class names and function definitions"""
 
-    def __init__(self, name: str, mock_name: str):
+    def __init__(self, name: str, mock_name: str, methods: List[FunctionDescriptor]):
         self.name = name
         self.mock_name = mock_name
-        self.methods: List[MockFunctionDescriptor] = []
-        self.constructors: List[str] = []  # this is never set to anything else
-        self.destructor = ""  # this is never set to anything else
+        self.methods: List[FunctionDescriptor] = methods
 
 
-class MockNamespaceDescriptor:
+class NamespaceDescriptor:
+    def __init__(self, name: str):
+        self.name = name
+
+
+class IncludeDescriptor:
     def __init__(self, name: str):
         self.name = name
 
 
 class HeaderDescriptor:
     """Parsed header definitions"""
 
-    def __init__(self, name: str, **kwargs: Any):
+    def __init__(
+        self,
+        name: str,
+        classes: List[ClassDescriptor],
+        namespaces: List[NamespaceDescriptor],
+        includes: List[IncludeDescriptor],
+    ):
         self.name = name
-        self.directives = kwargs.get("directives", [])
-        self.includes = kwargs.get("includes", [])
-        self.classes = kwargs.get("classes", [])
-        self.one_line_classes = kwargs.get("one_line_classes", [])
-        self.namespaces = kwargs.get("namespaces", [])
-        self.c_style_header = kwargs.get("c_style_header", False)
+        self.classes = classes
+        self.namespaces = namespaces
+        self.includes = includes
```

### Comparing `scargo-1.2.0/scargo/file_generators/templates/.gitlab-ci.yml.j2` & `scargo-1.3.0/scargo/file_generators/templates/.gitlab-ci.yml.j2`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
   stage: test
   extends: .merge_request
   allow_failure: true
   script:
     - scargo test
   artifacts:
     paths:
-      - build/doc/ut_coverage_html
+      - build/tests/ut-coverage.html
 
 #______________________________________________________________________________________________CLANG_FORMAT
 clang format:
   stage: check
   extends: .merge_request
   allow_failure: false
   script:
```

### Comparing `scargo-1.2.0/scargo/file_generators/templates/CMakeLists.txt.j2` & `scargo-1.3.0/scargo/file_generators/templates/CMakeLists.txt.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.2.0/scargo/file_generators/templates/README.md.j2` & `scargo-1.3.0/scargo/file_generators/templates/README.md.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.2.0/scargo/file_generators/templates/conan/conanfile.py.j2` & `scargo-1.3.0/scargo/file_generators/templates/conan/conanfile.py.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.2.0/scargo/file_generators/templates/conan/conanfiletest.j2` & `scargo-1.3.0/scargo/file_generators/templates/conan/conanfiletest.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.2.0/scargo/file_generators/templates/cpp/cmake-src-stm32.j2` & `scargo-1.3.0/scargo/file_generators/templates/cpp/cmake-src-stm32.j2`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 stm32_fetch_cmsis(${STM32_FAMILY})
 # stm32_fetch_hal(${STM32_FAMILY})
 
 find_package(CMSIS COMPONENTS STM32${STM32_FAMILY} REQUIRED)
 # find_package(HAL COMPONENTS STM32${STM32_FAMILY} REQUIRED)
-# set(CMAKE_INCLUDE_CURRENT_DIR TRUE)
+set(CMAKE_INCLUDE_CURRENT_DIR TRUE)
 
 STRING(TOLOWER ${STM32_FAMILY} STM32_FAMILY_LOWER)
 SET(HAL_CONFIG_FILE ${CMAKE_CURRENT_SOURCE_DIR}/stm32${STM32_FAMILY_LOWER}xx_hal_conf.h)
-if(NOT EXISTS HAL_CONFIG_FILE AND DEFINED STM32_HAL_${STM32_FAMILY}_PATH)
-    set(HAL_CONFIG_FILE_TEMPLATE ${STM32_HAL_L4_PATH}/Inc/stm32${STM32_FAMILY_LOWER}xx_hal_conf_template.h)
+if(NOT EXISTS ${HAL_CONFIG_FILE} AND DEFINED STM32_HAL_${STM32_FAMILY}_PATH)
+    set(HAL_CONFIG_FILE_TEMPLATE ${STM32_HAL_${FAMILY}_PATH}/Inc/stm32${STM32_FAMILY_LOWER}xx_hal_conf_template.h)
     configure_file(${HAL_CONFIG_FILE_TEMPLATE} ${HAL_CONFIG_FILE} COPYONLY)
 else()
 set(HAL_CONFIG_FILE "")
 endif()
 
 
 {% if  config.project.bin_name %}
```

### Comparing `scargo-1.2.0/scargo/file_generators/templates/cpp/cmake-src-x86.j2` & `scargo-1.3.0/scargo/file_generators/templates/cpp/cmake-src-x86.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.2.0/scargo/file_generators/templates/cpp/main.cpp.j2` & `scargo-1.3.0/scargo/file_generators/templates/cpp/main.cpp.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.2.0/scargo/file_generators/templates/docker/Dockerfile-esp32.j2` & `scargo-1.3.0/scargo/file_generators/templates/docker/Dockerfile-esp32.j2`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-RUN  apt -y install flex bison gperf python3-setuptools ninja-build ccache libffi-dev libssl-dev dfu-util libusb-1.0-0
+# esp-idf dependencies, https://docs.espressif.com/projects/esp-idf/en/latest/esp32/get-started/linux-macos-setup.html
+RUN apt update --fix-missing && apt -y --no-install-recommends install git wget flex bison gperf python3 python3-venv cmake ninja-build ccache libffi-dev libssl-dev dfu-util libusb-1.0-0 \
+    curl openocd && \
+    rm -rf /var/lib/apt/lists/*
 
 ARG ESPRESSIF_IDF_TAG="v4.4.3"
 ARG ESPRESSIF_IDF_VERSION="${ESPRESSIF_IDF_TAG}"
 ARG ESPRESSIF_IDF_PATH="/opt/esp-idf"
 ARG ESPRESSIF_IDF_REPO_URL="https://github.com/espressif/esp-idf.git"
 ARG ESPRESSIF_TOOLS_PATH="/root/.espressif"
 ARG RUN_CLANG_TIDY_SCRIPT_URL="https://raw.githubusercontent.com/llvm/llvm-project/llvmorg-16.0.0/clang-tools-extra/clang-tidy/tool/run-clang-tidy.py"
@@ -12,24 +15,15 @@
 WORKDIR /opt
 
 RUN umask 0002 && git clone --single-branch --branch ${ESPRESSIF_IDF_VERSION} --recursive ${ESPRESSIF_IDF_REPO_URL} ${ESPRESSIF_IDF_PATH}
 RUN umask 0002 && ${ESPRESSIF_IDF_PATH}/install.sh
 RUN umask 0002 && ${ESPRESSIF_IDF_PATH}/tools/idf_tools.py install xtensa-clang
 
 RUN curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash && \
-    apt-get update && \
-    apt-get install -y ca-certificates curl apt-transport-https lsb-release gnupg && \
-    curl -sL https://packages.microsoft.com/keys/microsoft.asc | \
-    gpg --dearmor | \
-    tee /etc/apt/trusted.gpg.d/microsoft.gpg > /dev/null && \
-    AZ_REPO=$(lsb_release -cs) && \
-    echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ $AZ_REPO main" | \
-    tee /etc/apt/sources.list.d/azure-cli.list && \
-    apt-get update && \
-    apt-get install azure-cli
+    rm -rf /var/lib/apt/lists/*
 
 ENV LC_ALL=C
 
 RUN umask 0002 && mkdir /opt/esp/ && echo '#!/usr/bin/env bash\n\
 \n\
 set -e\n\
 \n\
```

### Comparing `scargo-1.2.0/scargo/file_generators/templates/docker/Dockerfile.j2` & `scargo-1.3.0/scargo/file_generators/templates/docker/Dockerfile.j2`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,25 @@
 
 ARG DOCKER_IMAGE_ROOT=ubuntu:20.04
 FROM ${DOCKER_IMAGE_ROOT} as base
 
 ENV DEBIAN_FRONTEND noninteractive
 
 RUN apt update --fix-missing && \
-    apt -y install python3.8 python3.8-venv python3-pip \
-    binutils git wget \
-    scons build-essential pkg-config \
-    unzip graphviz nano vim && \
+    apt -y install --no-install-recommends python3 python3-pip \
+    git build-essential pkg-config graphviz && \
     apt -y install sudo && \
-    update-alternatives --install /usr/bin/python python /usr/bin/python3 1 && \
-    update-alternatives --install /usr/bin/pip pip /usr/bin/pip3 1
+    rm -rf /var/lib/apt/lists/* && \
+    update-alternatives --install /usr/bin/python python /usr/bin/python3 1
 
 FROM base AS cpp
 
-RUN apt -y install cppcheck bzr lib32z1 \
-    clang clang-format clang-tidy valgrind \
-    gcovr doxygen curl libcurl4-openssl-dev \
-    libcmocka0 libcmocka-dev plantuml
+RUN apt update --fix-missing && apt -y --no-install-recommends install cppcheck lib32z1 \
+    make cmake clang clang-format clang-tidy gcovr doxygen libcmocka0 libcmocka-dev && \
+    rm -rf /var/lib/apt/lists/*
 
 FROM cpp AS {{ project.target.family }}
 {% include 'docker/Dockerfile-' + project.target.family + '.j2' %}
 
 WORKDIR /opt
 
 FROM {{ project.target.family }} AS custom_{{ project.name }}
@@ -43,15 +40,16 @@
 ARG CONAN_PASSWORD
 ENV CONAN_LOGIN_USERNAME=${CONAN_LOGIN_USERNAME}
 ENV CONAN_PASSWORD=${CONAN_PASSWORD}
 
 WORKDIR /opt
 
 # configure ssh
-RUN apt install -y openssh-server ssh-askpass && apt install -y rsync grsync && \
+RUN apt update --fix-missing && apt install -y --no-install-recommends openssh-server && \
+    rm -rf /var/lib/apt/lists/* && \
     ssh-keygen -A && mkdir -p /run/sshd && \
     echo "Port $SSH_PORT" >> /etc/ssh/sshd_config
 
 EXPOSE $SSH_PORT
 
 RUN printf "\n\nADDING USER $USER_NAME TO SUDOERS - DEV ENV ONLY!\n\n" >&2 && \
     apt -y install sudo && \
```

### Comparing `scargo-1.2.0/scargo/file_generators/templates/docker/docker-compose.yaml.j2` & `scargo-1.3.0/scargo/file_generators/templates/docker/docker-compose.yaml.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.2.0/scargo/file_generators/templates/mock/class_mock.h.j2` & `scargo-1.3.0/scargo/file_generators/templates/mock/class_mock.h.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.2.0/scargo/file_generators/templates/scargo.toml.j2` & `scargo-1.3.0/scargo/file_generators/templates/scargo.toml.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.2.0/scargo/file_generators/templates/stm32.cmake.j2` & `scargo-1.3.0/scargo/file_generators/templates/stm32.cmake.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.2.0/scargo/file_generators/templates/tests/CMakeLists-test.txt.j2` & `scargo-1.3.0/scargo/file_generators/templates/tests/CMakeLists-test.txt.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.2.0/scargo/file_generators/templates/tests/static_mock/static_mock.h` & `scargo-1.3.0/scargo/file_generators/templates/tests/static_mock/static_mock.h`

 * *Files identical despite different names*

### Comparing `scargo-1.2.0/scargo/file_generators/templates/ut/CMakeLists.txt.j2` & `scargo-1.3.0/scargo/file_generators/templates/ut/CMakeLists.txt.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.2.0/scargo/file_generators/templates/ut/ut.cpp.j2` & `scargo-1.3.0/scargo/file_generators/templates/ut/ut.cpp.j2`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 /**
  * @copyright Copyright (C) 2022 Spyrosoft Solutions. All rights reserved.
  */
 
 #include <gtest/gtest.h>
 #include <memory>
 {% for inc in header.includes %}
-// #include {{inc}}
+#include "{{inc.name}}"
 {% endfor %}
 // #include "{{header.name}}"
 
 {% if header.namespaces %}
 {% for namespace in header.namespaces %}
-// using namespace {{namespace}};
+using namespace {{namespace.name}};
 {% endfor %}
 {% endif %}
 using namespace ::testing;
 
 {% if header.classes %}
 {% for cls in header.classes %}
-class {{cls}}Test : public Test
+class {{cls.name}}Test : public Test
 {
 public:
     void SetUp() override
     {
     }
 
     void TearDown() override
@@ -30,12 +30,12 @@
     }
 };
 {% endfor %}
 {% endif %}
 
 {% if header.classes %}
 {% for cls in header.classes %}
-TEST_F({{cls}}Test, exampleTest)
+TEST_F({{cls.name}}Test, exampleTest)
 {
 }
 {% endfor %}
 {% endif %}
```

### Comparing `scargo-1.2.0/scargo/file_generators/tests_gen.py` & `scargo-1.3.0/scargo/file_generators/tests_gen.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,13 +40,10 @@
     )
 
     for template, output_path in gen_once_file_list:
         create_file_from_template(
             template,
             output_path,
             overwrite=False,
-            template_params={
-                "target": config.project.target,
-                "tests": config.tests,
-            },
+            template_params={},
             config=config,
         )
```

### Comparing `scargo-1.2.0/scargo/file_generators/toml_gen.py` & `scargo-1.3.0/scargo/file_generators/toml_gen.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,15 @@
 """Generate toml for scargo project"""
 from pathlib import Path
 from typing import Any
 
 from scargo.file_generators.base_gen import write_template
 
 
-def generate_toml(output_file_path: str, **values: Any) -> None:
+def generate_toml(output_file_path: Path, **values: Any) -> None:
     """_summary_
 
     Args:
         output_file_path (String): path to the output .env file
         **values (Dict): dict contains all necessary values for toml
     """
-    write_template(
-        Path(output_file_path), "scargo.toml.j2", template_params={"data": values}
-    )
+    write_template(output_file_path, "scargo.toml.j2", template_params={"data": values})
```

### Comparing `scargo-1.2.0/scargo/file_generators/ut_gen.py` & `scargo-1.3.0/scargo/file_generators/ut_gen.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,21 @@
 # #
 # @copyright Copyright (C) 2023 SpyroSoft Solutions S.A. All rights reserved.
 # #
-
-import re
 from pathlib import Path
 from typing import List, Sequence
 
 from scargo.config import Config
 from scargo.file_generators.base_gen import create_file_from_template
-from scargo.file_generators.mock_utils.cmake_utils import add_subdirs_to_cmake
+from scargo.file_generators.clang_parser.header_parser import parse_file
 
 HEADER_EXTENSIONS = (".h", ".hpp")
 SRC_EXTENSIONS = (".c", ".cpp")
 
 
-class HeaderDescriptor:
-    """
-    This class is a container for names, includes, classes and namespaces
-    which are parsed from the header file. This information is then passed
-    to generate unit tests.
-    """
-
-    def __init__(
-        self, name: str, includes: List[str], classes: List[str], namespaces: List[str]
-    ) -> None:
-        self.name = name
-        self.includes = includes
-        self.classes = classes
-        self.namespaces = namespaces
-
-
 class _UnitTestsGen:
     def __init__(self, config: Config):
         self._config = config
         self._project_path = config.project_root
         self._ut_dir = self._project_path / "tests/ut"
 
     def generate_tests(self, input_path: Path, overwrite: bool) -> None:
@@ -61,45 +43,48 @@
     ) -> None:
         """Generates unit test source file
 
         :param Path input_file_path: Path to src file
         :param Path output_file_path: Path to unit test file
         :param bool overwrite: overwrite if exists
         """
-        header_descriptor = self._parse_header_file(input_file_path)
+        header_descriptor = parse_file(input_file_path)
         create_file_from_template(
             "ut/ut.cpp.j2",
             output_file_path,
             overwrite=overwrite,
             template_params={"header": header_descriptor},
             config=self._config,
         )
 
     def _generate_cmake(self, src_dir_path: Path, ut_dir_path: Path) -> None:
         """Generate CMakeLists for unit tests
 
         :param Path src_dir_path: Source directory for which tests are being generated
         :param Path ut_dir_path: Directory of generated unit tests
         """
-        add_subdirs_to_cmake(ut_dir_path.relative_to(self._project_path))
+        cmake_dir_path = ut_dir_path
+        while cmake_dir_path != self._ut_dir:
+            add_ut_dir_to_parent_cmake(cmake_dir_path)
+            cmake_dir_path = cmake_dir_path.parent
 
         ut_name = self._get_cmake_tests_name(ut_dir_path)
         ut_files = [
             p.name for p in self._get_paths_with_ext(ut_dir_path, SRC_EXTENSIONS)
         ]
 
         # Exclude main from srcs to test
         main_cpp = (
             f"{self._config.project.bin_name}.cpp"
             if self._config.project.bin_name
             else None
         )
 
         src_files = [
-            p.absolute().relative_to(self._project_path.absolute())
+            p.relative_to(self._project_path)
             for p in self._get_paths_with_ext(src_dir_path, SRC_EXTENSIONS)
             if p.name != main_cpp
         ]
 
         create_file_from_template(
             "ut/CMakeLists.txt.j2",
             ut_dir_path / "CMakeLists.txt",
@@ -114,73 +99,50 @@
 
     def _get_unit_test_path(self, input_src_path: Path) -> Path:
         """Return output path for unit test
 
         :param Path input_src_path: Source path
         :return Path: output path for unit test
         """
-        input_src_path = input_src_path.absolute()
-        relative_to_src = input_src_path.relative_to(
-            self._project_path.absolute() / self._config.project.target.source_dir
-        )
+        relative_to_src = input_src_path.relative_to(self._config.source_dir_path)
         return Path(self._ut_dir, relative_to_src).with_name(
             f"ut_{input_src_path.stem}.cpp"
         )
 
     def _get_cmake_tests_name(self, test_dir_path: Path) -> str:
         """Get tests name for cmake
 
         :param Path test_dir_path: Path to test dir
         :return str: tests name for cmake
         """
-        test_dir_path = test_dir_path.absolute()
-        relative_path = test_dir_path.relative_to(self._project_path.absolute())
+        relative_path = test_dir_path.relative_to(self._project_path)
         return "_".join(relative_path.parts)
 
     @staticmethod
-    def _get_namespace(line: str) -> str:
-        if line.startswith("namespace"):
-            namespace = line.split(" ")[1]
-        elif line.startswith("using namespace"):
-            namespace = line.split(" ")[2]
-        else:
-            raise ValueError(f"No 'namespace' found in line: '{line}'")
-
-        last_char = namespace[-1]
-        if last_char in ("{", ";"):
-            return namespace[0:-1]
-
-        return namespace
-
-    @staticmethod
-    def _parse_header_file(header_path: Path) -> HeaderDescriptor:
-        namespaces = []
-        classes = []
-        includes = []
-
-        # open header file to parse the header name and class name
-        with open(header_path, encoding="utf-8") as header:
-            for line in header:
-                line = line.strip()
-                if line.startswith("#include"):
-                    includes.append(line.split(" ")[1])
-                elif line.startswith("namespace") or line.startswith("using namespace"):
-                    namespaces.append(_UnitTestsGen._get_namespace(line))
-                elif line.startswith("class"):
-                    class_regex = re.compile(r"^([a-z]+)(\s[a-zA-Z\d]+)")
-                    temp = class_regex.search(line)
-                    if temp:
-                        classes.append(temp.group(2).lstrip())
-                elif line.startswith('extern "C"'):
-                    class_name = "".join([w.capitalize() for w in header_path.stem])
-                    classes.append(class_name)
-
-        return HeaderDescriptor(str(header_path), namespaces, classes, includes)
-
-    @staticmethod
     def _get_paths_with_ext(workdir: Path, extensions: Sequence[str]) -> List[Path]:
         return [child for child in workdir.iterdir() if child.suffix in extensions]
 
 
+COPYRIGHT = """# #
+# Copyright (C) 2022 Spyrosoft Solutions. All rights reserved.
+# #\n\n"""
+
+
+def add_ut_dir_to_parent_cmake(ut_dir_path: Path) -> None:
+    # if CMakelists doesn't exist create it in parent dir
+    parent_dir = ut_dir_path.parent
+    cmake_list_path = parent_dir / "CMakeLists.txt"
+    if not cmake_list_path.exists():
+        with cmake_list_path.open("w", encoding="utf-8") as file:
+            file.write(COPYRIGHT)
+    # check if ut_dir_path exists in CMakeLists
+    # if not add it
+    with cmake_list_path.open("r+", encoding="utf-8") as file:
+        cmake_text = file.read()
+        add_subdirectory_clause = f"\nadd_subdirectory({ut_dir_path.name})"
+        if add_subdirectory_clause not in cmake_text:
+            file.write(add_subdirectory_clause)
+
+
 def generate_ut(input_path: Path, config: Config, force: bool = False) -> None:
     ut_gen = _UnitTestsGen(config)
     ut_gen.generate_tests(input_path, force)
```

### Comparing `scargo-1.2.0/scargo/global_values.py` & `scargo-1.3.0/scargo/global_values.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pathlib import Path
 
 DESCRIPTION = "C/C++ package and software development life cycle manager based on RUST cargo idea."
 
 SCARGO_PKG_PATH = (
     Path(pkgutil.get_loader("scargo").path).parent  # type: ignore[union-attr]
     if pkgutil.get_loader("scargo").path  # type: ignore[union-attr]
-    else Path(__file__).absolute().parent
+    else Path(__file__).parent
 )
 SCARGO_DEFAULT_BUILD_ENV = "docker"
 SCARGO_DOCKER_ENV = "docker"
 
 SCARGO_LOCK_FILE = "scargo.lock"
 SCARGO_DEFAULT_CONFIG_FILE = "scargo.toml"
 ENV_DEFAULT_NAME = ".env"
```

### Comparing `scargo-1.2.0/scargo/logger.py` & `scargo-1.3.0/scargo/logger.py`

 * *Files identical despite different names*

### Comparing `scargo-1.2.0/scargo/path_utils.py` & `scargo-1.3.0/scargo/path_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         cmd_output = subprocess.check_output([cmd, program_name])
     except subprocess.CalledProcessError:
         return None
     return Path(cmd_output.decode("utf-8").strip())
 
 
 def get_config_file_path(config_file_name: str) -> Optional[Path]:
-    current_path = Path().absolute()
+    current_path = Path.cwd()
     directories_to_check = [current_path] + list(current_path.parents)
     for directory in directories_to_check:
         if (directory / config_file_name).exists():
             return directory / config_file_name
     return None
```

### Comparing `scargo-1.2.0/scargo/templates/.clang-format` & `scargo-1.3.0/scargo/templates/.clang-format`

 * *Files identical despite different names*

### Comparing `scargo-1.2.0/scargo/templates/.clang-tidy` & `scargo-1.3.0/scargo/templates/.clang-tidy`

 * *Files identical despite different names*

### Comparing `scargo-1.2.0/scargo/templates/.gitignore` & `scargo-1.3.0/scargo/templates/.gitignore`

 * *Files identical despite different names*

### Comparing `scargo-1.2.0/scargo/templates/LICENSE` & `scargo-1.3.0/scargo/templates/LICENSE`

 * *Files identical despite different names*

### Comparing `scargo-1.2.0/setup.cfg` & `scargo-1.3.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [flake8]
 exclude = .git,__pycache__,.eggs,build
-ignore = W503,
+ignore = W503,E203
 
 per-file-ignores =
     # tests often manipulate sys.path before importing the main tools, so ignore import order violations
     test/*.py: E402,
 
     # ignore long lines - used for RS encoding pairs
     test/test_modules.py: E501,
```

### Comparing `scargo-1.2.0/PKG-INFO` & `scargo-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scargo
-Version: 1.2.0
+Version: 1.3.0
 Summary: C/C++ package and software development life cycle manager inspired by RUST cargo idea.
 Keywords: scargo,Package manager,C++
 Author-email: "Spyrosoft Solutions S.A." <aak@spyro-soft.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -14,47 +14,48 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: clang==14.0
+Requires-Dist: clang==16.0.1.1
 Requires-Dist: cmake==3.25.2
 Requires-Dist: coloredlogs==15.0.1
 Requires-Dist: conan==1.59.0
 Requires-Dist: docker==6.0.1
 Requires-Dist: esptool==4.5.1
 Requires-Dist: jinja2==3.1.2
 Requires-Dist: libclang==16.0.0
 Requires-Dist: lizard==1.17.10
 Requires-Dist: pydantic==1.10.6
 Requires-Dist: shellingham==1.5.0.post1
 Requires-Dist: toml==0.10.2
 Requires-Dist: tomlkit==0.11.6
 Requires-Dist: typer==0.7.0
-Requires-Dist: allure-pytest ; extra == "dev"
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: coverage~=6.0 ; extra == "dev"
 Requires-Dist: flake8>=3.2.0 ; extra == "dev"
 Requires-Dist: flit==3.8.0 ; extra == "dev"
 Requires-Dist: gcovr>=5.2 ; extra == "dev"
 Requires-Dist: isort==5.11.4 ; extra == "dev"
+Requires-Dist: matplotlib ; extra == "dev"
 Requires-Dist: mypy==1.0.1 ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: pyclean==2.2.0 ; extra == "dev"
 Requires-Dist: pyelftools ; extra == "dev"
+Requires-Dist: pyfakefs ; extra == "dev"
 Requires-Dist: PyInstaller ; extra == "dev"
 Requires-Dist: pylint ; extra == "dev"
 Requires-Dist: pytest-bdd ; extra == "dev"
 Requires-Dist: pytest-cov ; extra == "dev"
 Requires-Dist: pytest-mock ; extra == "dev"
 Requires-Dist: pytest-subprocess ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev"
-Requires-Dist: types-clang ; extra == "dev"
+Requires-Dist: types-clang==0.14.3 ; extra == "dev"
 Requires-Dist: types-toml ; extra == "dev"
 Requires-Dist: unittest-xml-reporting ; extra == "dev"
 Requires-Dist: recommonmark ; extra == "doc"
 Requires-Dist: sphinx-rtd-theme==1.1.1 ; extra == "doc"
 Requires-Dist: Sphinx ; extra == "doc"
 Requires-Dist: sphinxcontrib-plantuml==0.24.1 ; extra == "doc"
 Project-URL: Documentation, https://spyro-soft.github.io/scargo/index.html
@@ -99,15 +100,15 @@
 - python3
 
 ## Working natively (not recommended, a lot of env setup)
 Base:
 
 - python >= 3.8
 - cmake >= 3.24.2
-- cppcheck bzr lib32z1 clang clang-format clang-tidy valgrind gcovr doxygen curl libcurl4-openssl-dev libcmocka0 libcmocka-dev
+- cppcheck lib32z1 clang clang-format clang-tidy gcovr doxygen libcmocka0 libcmocka-dev
 - lizard
 
 Depending on the architecture:
 
 - compiler (e.g. gcc-arm-none-eabi-9-2020-q2-update gcc-arm-none-eabi)
 - flashing tools
 - uC HAL and dependent files
```

