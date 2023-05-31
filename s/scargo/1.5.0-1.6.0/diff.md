# Comparing `tmp/scargo-1.5.0.tar.gz` & `tmp/scargo-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scargo-1.5.0.tar", last modified: Fri May 19 06:46:32 2023, max compression
+gzip compressed data, was "scargo-1.6.0.tar", last modified: Wed May 31 13:51:20 2023, max compression
```

## Comparing `scargo-1.5.0.tar` & `scargo-1.6.0.tar`

### file list

```diff
@@ -1,95 +1,95 @@
--rw-r--r--   0        0        0     4508 2023-05-19 06:46:27.278807 scargo-1.5.0/CODE-OF-CONDUCT.md
--rw-r--r--   0        0        0     1066 2023-05-19 06:46:27.278807 scargo-1.5.0/LICENSE
--rw-r--r--   0        0        0     2488 2023-05-19 06:46:27.278807 scargo-1.5.0/README.md
--rw-r--r--   0        0        0     2748 2023-05-19 06:46:27.406804 scargo-1.5.0/pyproject.toml
--rw-r--r--   0        0        0      108 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/__init__.py
--rwxr-xr-x   0        0        0    19734 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/certs/certGen.sh
--rwxr-xr-x   0        0        0     5226 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/certs/generateAllCertificates.sh
--rw-r--r--   0        0        0     3967 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/certs/openssl_device_intermediate_ca.cnf
--rw-r--r--   0        0        0     3957 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/certs/openssl_root_ca.cnf
--rw-r--r--   0        0        0      698 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/clang_utils.py
--rw-r--r--   0        0        0    12706 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/cli.py
--rw-r--r--   0        0        0       86 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/commands/__init__.py
--rw-r--r--   0        0        0     1738 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/commands/build.py
--rw-r--r--   0        0        0    12212 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/commands/check.py
--rw-r--r--   0        0        0     1142 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/commands/clean.py
--rw-r--r--   0        0        0     4343 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/commands/debug.py
--rw-r--r--   0        0        0     3402 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/commands/doc.py
--rw-r--r--   0        0        0     3369 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/commands/docker.py
--rw-r--r--   0        0        0     1124 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/commands/fix.py
--rw-r--r--   0        0        0     3927 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/commands/flash.py
--rw-r--r--   0        0        0     6677 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/commands/gen.py
--rw-r--r--   0        0        0     2857 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/commands/new.py
--rw-r--r--   0        0        0     3405 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/commands/publish.py
--rw-r--r--   0        0        0     1688 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/commands/run.py
--rw-r--r--   0        0        0     3347 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/commands/test.py
--rw-r--r--   0        0        0     4419 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/commands/update.py
--rw-r--r--   0        0        0      228 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/commands/version.py
--rw-r--r--   0        0        0     6707 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/config.py
--rw-r--r--   0        0        0     2255 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/config_utils.py
--rw-r--r--   0        0        0     2174 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/docker_utils.py
--rw-r--r--   0        0        0       86 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/file_generators/__init__.py
--rw-r--r--   0        0        0     1658 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/file_generators/base_gen.py
--rw-r--r--   0        0        0      441 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/file_generators/cicd_gen.py
--rw-r--r--   0        0        0       86 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/file_generators/clang_parser/__init__.py
--rw-r--r--   0        0        0     2251 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/file_generators/clang_parser/data_classes.py
--rw-r--r--   0        0        0     1197 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/file_generators/clang_parser/header_parser.py
--rw-r--r--   0        0        0     2348 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/file_generators/clang_parser/params_extractor.py
--rw-r--r--   0        0        0      395 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/file_generators/cmake_gen.py
--rw-r--r--   0        0        0      569 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/file_generators/conan_gen.py
--rw-r--r--   0        0        0     2468 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/file_generators/cpp_gen.py
--rw-r--r--   0        0        0     3186 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/file_generators/docker_gen.py
--rw-r--r--   0        0        0     1115 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/file_generators/env_gen.py
--rwxr-xr-x   0        0        0     1607 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/file_generators/mock_gen.py
--rw-r--r--   0        0        0      454 2023-05-19 06:46:27.406804 scargo-1.5.0/scargo/file_generators/readme_gen.py
--rw-r--r--   0        0        0     4834 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/.gitlab-ci.yml.j2
--rw-r--r--   0        0        0     1580 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/CMakeLists.txt.j2
--rw-r--r--   0        0        0     4275 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/README.md.j2
--rw-r--r--   0        0        0     1693 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/conan/conanfile.py.j2
--rw-r--r--   0        0        0     1464 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/conan/conanfiletest.j2
--rw-r--r--   0        0        0      150 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/cpp/cmake-src-esp32.j2
--rw-r--r--   0        0        0     2423 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/cpp/cmake-src-stm32.j2
--rw-r--r--   0        0        0      886 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/cpp/cmake-src-x86.j2
--rw-r--r--   0        0        0      181 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/cpp/lib.cpp.j2
--rw-r--r--   0        0        0      213 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/cpp/lib.h.j2
--rw-r--r--   0        0        0      715 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/cpp/main.cpp.j2
--rw-r--r--   0        0        0      159 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/docker/Dockerfile-custom.j2
--rw-r--r--   0        0        0     2067 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/docker/Dockerfile-esp32.j2
--rw-r--r--   0        0        0      754 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/docker/Dockerfile-stm32.j2
--rw-r--r--   0        0        0       49 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/docker/Dockerfile-x86.j2
--rw-r--r--   0        0        0     2359 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/docker/Dockerfile.j2
--rw-r--r--   0        0        0      158 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/docker/devcontainer.json.j2
--rw-r--r--   0        0        0     1000 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/docker/docker-compose.yaml.j2
--rw-r--r--   0        0        0      287 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/docker/env.txt.j2
--rw-r--r--   0        0        0       22 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/docker/stm32.cfg.j2
--rw-r--r--   0        0        0      294 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/esp32.cmake.j2
--rw-r--r--   0        0        0       39 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/mock/.clang-format
--rw-r--r--   0        0        0      475 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/mock/CMakeLists.txt
--rw-r--r--   0        0        0      594 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/mock/class_interface.h.j2
--rw-r--r--   0        0        0      835 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/mock/class_mock.cpp.j2
--rw-r--r--   0        0        0      697 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/mock/class_mock.h.j2
--rw-r--r--   0        0        0      510 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/project.cmake.j2
--rw-r--r--   0        0        0     2228 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/scargo.toml.j2
--rw-r--r--   0        0        0      802 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/stm32.cmake.j2
--rw-r--r--   0        0        0       91 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/tests/CMakeLists-it.txt.j2
--rw-r--r--   0        0        0      100 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/tests/CMakeLists-mocks.txt.j2
--rw-r--r--   0        0        0     1079 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/tests/CMakeLists-test.txt.j2
--rw-r--r--   0        0        0       84 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/tests/CMakeLists-ut.txt.j2
--rw-r--r--   0        0        0      326 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/tests/static_mock/CMakeLists.txt
--rw-r--r--   0        0        0     1046 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/tests/static_mock/static_mock.h
--rw-r--r--   0        0        0       39 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/ut/.clang-format
--rw-r--r--   0        0        0      575 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/ut/CMakeLists.txt.j2
--rw-r--r--   0        0        0      719 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/ut/ut.cpp.j2
--rw-r--r--   0        0        0      213 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/templates/x86.cmake.j2
--rw-r--r--   0        0        0     1597 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/tests_gen.py
--rw-r--r--   0        0        0      550 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/toml_gen.py
--rw-r--r--   0        0        0     5357 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/file_generators/ut_gen.py
--rw-r--r--   0        0        0      629 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/global_values.py
--rw-r--r--   0        0        0     2044 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/logger.py
--rw-r--r--   0        0        0     1137 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/path_utils.py
--rw-r--r--   0        0        0     2953 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/templates/.clang-format
--rw-r--r--   0        0        0     8780 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/templates/.clang-tidy
--rw-r--r--   0        0        0     2361 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/templates/.gitignore
--rw-r--r--   0        0        0     1066 2023-05-19 06:46:27.410804 scargo-1.5.0/scargo/templates/LICENSE
--rw-r--r--   0        0        0      519 2023-05-19 06:46:27.410804 scargo-1.5.0/setup.cfg
--rw-r--r--   0        0        0     5229 1970-01-01 00:00:00.000000 scargo-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     4508 2023-05-31 13:51:14.577332 scargo-1.6.0/CODE-OF-CONDUCT.md
+-rw-r--r--   0        0        0     1066 2023-05-31 13:51:14.577332 scargo-1.6.0/LICENSE
+-rw-r--r--   0        0        0     2494 2023-05-31 13:51:14.581332 scargo-1.6.0/README.md
+-rw-r--r--   0        0        0     2748 2023-05-31 13:51:14.589332 scargo-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0      108 2023-05-31 13:51:14.589332 scargo-1.6.0/scargo/__init__.py
+-rwxr-xr-x   0        0        0    19734 2023-05-31 13:51:14.589332 scargo-1.6.0/scargo/certs/certGen.sh
+-rwxr-xr-x   0        0        0     5226 2023-05-31 13:51:14.589332 scargo-1.6.0/scargo/certs/generateAllCertificates.sh
+-rw-r--r--   0        0        0     3967 2023-05-31 13:51:14.589332 scargo-1.6.0/scargo/certs/openssl_device_intermediate_ca.cnf
+-rw-r--r--   0        0        0     3957 2023-05-31 13:51:14.589332 scargo-1.6.0/scargo/certs/openssl_root_ca.cnf
+-rw-r--r--   0        0        0      698 2023-05-31 13:51:14.589332 scargo-1.6.0/scargo/clang_utils.py
+-rw-r--r--   0        0        0    12830 2023-05-31 13:51:14.589332 scargo-1.6.0/scargo/cli.py
+-rw-r--r--   0        0        0       86 2023-05-31 13:51:14.589332 scargo-1.6.0/scargo/commands/__init__.py
+-rw-r--r--   0        0        0     1738 2023-05-31 13:51:14.589332 scargo-1.6.0/scargo/commands/build.py
+-rw-r--r--   0        0        0    12319 2023-05-31 13:51:14.589332 scargo-1.6.0/scargo/commands/check.py
+-rw-r--r--   0        0        0     1142 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/commands/clean.py
+-rw-r--r--   0        0        0     4168 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/commands/debug.py
+-rw-r--r--   0        0        0     3402 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/commands/doc.py
+-rw-r--r--   0        0        0     3286 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/commands/docker.py
+-rw-r--r--   0        0        0     1124 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/commands/fix.py
+-rw-r--r--   0        0        0     3835 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/commands/flash.py
+-rw-r--r--   0        0        0     6677 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/commands/gen.py
+-rw-r--r--   0        0        0     2857 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/commands/new.py
+-rw-r--r--   0        0        0     3405 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/commands/publish.py
+-rw-r--r--   0        0        0     1688 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/commands/run.py
+-rw-r--r--   0        0        0     3651 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/commands/test.py
+-rw-r--r--   0        0        0     4419 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/commands/update.py
+-rw-r--r--   0        0        0      228 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/commands/version.py
+-rw-r--r--   0        0        0     6707 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/config.py
+-rw-r--r--   0        0        0     2255 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/config_utils.py
+-rw-r--r--   0        0        0     2174 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/docker_utils.py
+-rw-r--r--   0        0        0       86 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/__init__.py
+-rw-r--r--   0        0        0     1658 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/base_gen.py
+-rw-r--r--   0        0        0      441 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/cicd_gen.py
+-rw-r--r--   0        0        0       86 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/clang_parser/__init__.py
+-rw-r--r--   0        0        0     2251 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/clang_parser/data_classes.py
+-rw-r--r--   0        0        0     1197 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/clang_parser/header_parser.py
+-rw-r--r--   0        0        0     2385 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/clang_parser/params_extractor.py
+-rw-r--r--   0        0        0      395 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/cmake_gen.py
+-rw-r--r--   0        0        0      569 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/conan_gen.py
+-rw-r--r--   0        0        0     2468 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/cpp_gen.py
+-rw-r--r--   0        0        0     3186 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/docker_gen.py
+-rw-r--r--   0        0        0     1115 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/env_gen.py
+-rwxr-xr-x   0        0        0     1607 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/mock_gen.py
+-rw-r--r--   0        0        0      454 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/readme_gen.py
+-rw-r--r--   0        0        0     4834 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/.gitlab-ci.yml.j2
+-rw-r--r--   0        0        0     1580 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/CMakeLists.txt.j2
+-rw-r--r--   0        0        0     4275 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/README.md.j2
+-rw-r--r--   0        0        0     1693 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/conan/conanfile.py.j2
+-rw-r--r--   0        0        0     1464 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/conan/conanfiletest.j2
+-rw-r--r--   0        0        0      150 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/cpp/cmake-src-esp32.j2
+-rw-r--r--   0        0        0     2423 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/cpp/cmake-src-stm32.j2
+-rw-r--r--   0        0        0      886 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/cpp/cmake-src-x86.j2
+-rw-r--r--   0        0        0      181 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/cpp/lib.cpp.j2
+-rw-r--r--   0        0        0      213 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/cpp/lib.h.j2
+-rw-r--r--   0        0        0      715 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/cpp/main.cpp.j2
+-rw-r--r--   0        0        0      159 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/docker/Dockerfile-custom.j2
+-rw-r--r--   0        0        0     2128 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/docker/Dockerfile-esp32.j2
+-rw-r--r--   0        0        0      754 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/docker/Dockerfile-stm32.j2
+-rw-r--r--   0        0        0       49 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/docker/Dockerfile-x86.j2
+-rw-r--r--   0        0        0     2363 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/docker/Dockerfile.j2
+-rw-r--r--   0        0        0      158 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/docker/devcontainer.json.j2
+-rw-r--r--   0        0        0     1000 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/docker/docker-compose.yaml.j2
+-rw-r--r--   0        0        0      287 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/docker/env.txt.j2
+-rw-r--r--   0        0        0       22 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/docker/stm32.cfg.j2
+-rw-r--r--   0        0        0      294 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/esp32.cmake.j2
+-rw-r--r--   0        0        0       39 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/mock/.clang-format
+-rw-r--r--   0        0        0      475 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/mock/CMakeLists.txt
+-rw-r--r--   0        0        0      594 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/mock/class_interface.h.j2
+-rw-r--r--   0        0        0      835 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/mock/class_mock.cpp.j2
+-rw-r--r--   0        0        0      697 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/mock/class_mock.h.j2
+-rw-r--r--   0        0        0      510 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/project.cmake.j2
+-rw-r--r--   0        0        0     2228 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/scargo.toml.j2
+-rw-r--r--   0        0        0      802 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/stm32.cmake.j2
+-rw-r--r--   0        0        0       91 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/tests/CMakeLists-it.txt.j2
+-rw-r--r--   0        0        0      100 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/tests/CMakeLists-mocks.txt.j2
+-rw-r--r--   0        0        0     1079 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/tests/CMakeLists-test.txt.j2
+-rw-r--r--   0        0        0       84 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/tests/CMakeLists-ut.txt.j2
+-rw-r--r--   0        0        0      326 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/tests/static_mock/CMakeLists.txt
+-rw-r--r--   0        0        0     1046 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/tests/static_mock/static_mock.h
+-rw-r--r--   0        0        0       39 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/ut/.clang-format
+-rw-r--r--   0        0        0      575 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/ut/CMakeLists.txt.j2
+-rw-r--r--   0        0        0      716 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/ut/ut.cpp.j2
+-rw-r--r--   0        0        0      213 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/templates/x86.cmake.j2
+-rw-r--r--   0        0        0     1597 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/tests_gen.py
+-rw-r--r--   0        0        0      550 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/toml_gen.py
+-rw-r--r--   0        0        0     5357 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/file_generators/ut_gen.py
+-rw-r--r--   0        0        0      629 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/global_values.py
+-rw-r--r--   0        0        0     2044 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/logger.py
+-rw-r--r--   0        0        0     1137 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/path_utils.py
+-rw-r--r--   0        0        0     2953 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/templates/.clang-format
+-rw-r--r--   0        0        0     8780 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/templates/.clang-tidy
+-rw-r--r--   0        0        0     2361 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/templates/.gitignore
+-rw-r--r--   0        0        0     1066 2023-05-31 13:51:14.593332 scargo-1.6.0/scargo/templates/LICENSE
+-rw-r--r--   0        0        0      519 2023-05-31 13:51:14.593332 scargo-1.6.0/setup.cfg
+-rw-r--r--   0        0        0     5235 1970-01-01 00:00:00.000000 scargo-1.6.0/PKG-INFO
```

### Comparing `scargo-1.5.0/CODE-OF-CONDUCT.md` & `scargo-1.6.0/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/LICENSE` & `scargo-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/README.md` & `scargo-1.6.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # Installation
 Scargo is available on [pypi](https://pypi.org/project/scargo/), so you can install it with pip:
 
 ```pip install scargo```
 
 # Working with scargo
 You can find all information on how to work with scargo on official documentation webpage: https://spyro-soft.github.io/scargo/index.html
-![Scargo flow gif](https://raw.githubusercontent.com/Spyro-Soft/scargo/develop/docs/source/_static/scargo_flow_docker.gif)
+![Scargo flow animation](https://raw.githubusercontent.com/Spyro-Soft/scargo/develop/docs/source/_static/scargo_flow_docker.svg)
 
 # Project dependencies
 ## Working with docker (recommended)
 - docker
 - docker-compose
 - pip
 - python3
```

### Comparing `scargo-1.5.0/pyproject.toml` & `scargo-1.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/certs/certGen.sh` & `scargo-1.6.0/scargo/certs/certGen.sh`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/certs/generateAllCertificates.sh` & `scargo-1.6.0/scargo/certs/generateAllCertificates.sh`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/certs/openssl_device_intermediate_ca.cnf` & `scargo-1.6.0/scargo/certs/openssl_device_intermediate_ca.cnf`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/certs/openssl_root_ca.cnf` & `scargo-1.6.0/scargo/certs/openssl_root_ca.cnf`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/clang_utils.py` & `scargo-1.6.0/scargo/clang_utils.py`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/cli.py` & `scargo-1.6.0/scargo/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -403,20 +403,23 @@
 ###############################################################################
 
 
 @cli.command()
 def test(
     verbose: bool = Option(False, "--verbose", "-v", help="Verbose mode."),
     profile: str = Option("Debug", "--profile", help="CMake profile to use"),
+    detailed_coverage: bool = Option(
+        False, help="Generate detailed coverage HTML files"
+    ),
     base_dir: Optional[Path] = BASE_DIR_OPTION,
 ) -> None:
     """Compile and run all tests in directory `test`."""
     if base_dir:
         os.chdir(base_dir)
-    scargo_test(verbose, profile)
+    scargo_test(verbose, profile, detailed_coverage)
 
 
 ###############################################################################
 
 
 @cli.command()
 def update(
```

### Comparing `scargo-1.5.0/scargo/commands/build.py` & `scargo-1.6.0/scargo/commands/build.py`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/commands/check.py` & `scargo-1.6.0/scargo/commands/check.py`

 * *Files 1% similar despite different names*

```diff
@@ -308,14 +308,16 @@
                     ["idf.py", "clang-check"],
                     stdout=subprocess.DEVNULL,
                     stderr=subprocess.DEVNULL,
                     check=False,
                 )
         if file_path.suffix == ".h":
             cmd.extend(["--", "-x", "c++"])
+        if "--" not in cmd and self._config.project.target.family != "esp32":
+            cmd.append("--")
         try:
             subprocess.check_output(cmd)
         except subprocess.CalledProcessError as e:
             if self._verbose:
                 logger.info(e.output.decode())
             else:
                 logger.warning("clang-tidy found error in file %s", file_path)
```

### Comparing `scargo-1.5.0/scargo/commands/clean.py` & `scargo-1.6.0/scargo/commands/clean.py`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/commands/debug.py` & `scargo-1.6.0/scargo/commands/debug.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,20 +27,15 @@
         if self._target.family not in self.SUPPORTED_TARGETS:
             logger.error("Debugging currently not supported for %s", self._target)
             logger.info(
                 "Scargo currently supports debug for %s", self.SUPPORTED_TARGETS
             )
             sys.exit(1)
 
-        bin_name = config.project.bin_name
-        bin_path = bin_path or (self._get_bin_path(bin_name) if bin_name else None)
-        if not bin_path:
-            logger.error("No bin_name in config")
-            sys.exit(1)
-        self._bin_path = bin_path
+        self._bin_path = bin_path or self._get_bin_path(config.project.name.lower())
         if not self._bin_path.exists():
             logger.error("Binary %s does not exist", self._bin_path)
             logger.info("Did you run scargo build --profile Debug?")
             sys.exit(1)
 
         if self._target.family == "stm32":
             stm32_config = config.get_stm32_config()
```

### Comparing `scargo-1.5.0/scargo/commands/doc.py` & `scargo-1.6.0/scargo/commands/doc.py`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/commands/docker.py` & `scargo-1.6.0/scargo/commands/docker.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,15 +68,14 @@
     if command:
         cmd.extend(["bash", "-c", command])
 
     try:
         subprocess.run(cmd, cwd=docker_path, check=True)
         logger.info("Stop docker environment.")
     except subprocess.CalledProcessError:
-        logger.error("Run docker fail.")
         sys.exit(1)
 
 
 def scargo_docker_exec(docker_opts: List[str]) -> None:
     """
     Exec docker
 
@@ -103,15 +102,14 @@
 
     bash_command = ["bash"]
     cmd = ["docker", "exec", "-it", *docker_opts, newest_container[0].id, *bash_command]
     try:
         subprocess.run(cmd, check=True)
         logger.info("Stop exec docker environment.")
     except subprocess.CalledProcessError:
-        logger.error("Exec docker fail.")
         sys.exit(1)
 
 
 def _get_docker_path(project_path: Path) -> Path:
     # do not rebuild dockers in the docker
     if Path("/.dockerenv").exists():
         logger.error("Cannot used docker command inside the docker container.")
```

### Comparing `scargo-1.5.0/scargo/commands/fix.py` & `scargo-1.6.0/scargo/commands/fix.py`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/commands/flash.py` & `scargo-1.6.0/scargo/commands/flash.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,20 +89,21 @@
 def flash_stm32(
     config: Config,
     flash_profile: str = "Debug",
     erase_memory: bool = True,
     port: Optional[str] = None,
 ) -> None:
     project_path = config.project_root
-    bin_name = config.project.bin_name
-    if not bin_name:
-        logger.error("No bin_name in config!")
-        sys.exit(1)
-    bin_name = bin_name.lower()
-    bin_path = project_path / "build" / flash_profile / "bin" / f"{bin_name}.bin"
+    bin_path = (
+        project_path
+        / "build"
+        / flash_profile
+        / "bin"
+        / f"{config.project.name.lower()}.bin"
+    )
 
     flash_start = hex(config.get_stm32_config().flash_start)
 
     if not bin_path.exists():
         logger.error("%s does not exist", bin_path)
         logger.info("Did you run scargo build --profile %s", flash_profile)
     elif not flash_start:
```

### Comparing `scargo-1.5.0/scargo/commands/gen.py` & `scargo-1.6.0/scargo/commands/gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/commands/new.py` & `scargo-1.6.0/scargo/commands/new.py`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/commands/publish.py` & `scargo-1.6.0/scargo/commands/publish.py`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/commands/run.py` & `scargo-1.6.0/scargo/commands/run.py`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/commands/test.py` & `scargo-1.6.0/scargo/commands/test.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,19 +11,22 @@
 from scargo.config import Config
 from scargo.config_utils import prepare_config
 from scargo.logger import get_logger
 
 logger = get_logger()
 
 
-def scargo_test(verbose: bool, profile: str = "Debug") -> None:
+def scargo_test(
+    verbose: bool, profile: str = "Debug", detailed_coverage: bool = False
+) -> None:
     """
     Run test
     :param bool verbose: if verbose
     :param str profile: CMake profile to use
+    :param bool detailed_coverage: Generate detailed coverage HTML files
     """
     config = prepare_config()
 
     test_dir_name = "tests"
     project_dir = config.project_root
     tests_src_dir = project_dir / test_dir_name
     test_build_dir = project_dir / "build" / test_dir_name
@@ -57,39 +60,45 @@
             cwd=project_dir,
         )
     except subprocess.CalledProcessError:
         logger.error("Failed to build tests.")
         sys.exit(1)
 
     # run ut
-    run_ut(config, verbose, test_build_dir)
+    run_ut(config, verbose, test_build_dir, detailed_coverage)
 
 
-def run_ut(config: Config, verbose: bool, cwd: Path) -> None:
+def run_ut(config: Config, verbose: bool, cwd: Path, detailed_coverage: bool) -> None:
     # Run tests.
     cmd: List[Union[str, Path]] = ["ctest"]
 
     if verbose:
         cmd.append("--verbose")
     try:
         # Using `subprocess.run` because tests can fail,
         # and we do not want Python to throw exception.
         subprocess.run(cmd, cwd=cwd, check=False)
 
+        output_option = (
+            "--html-details=ut-coverage.details.html"
+            if detailed_coverage
+            else "--html=ut-coverage.html"
+        )
+
         # Run code coverage.
         cmd = [
             "gcovr",
             "-r",
             "ut",
             ".",
             "-f",
             config.source_dir_path,
-            "--html",
-            "ut-coverage.html",
+            output_option,
         ]
+        print(cmd)
 
         gcov_executable = config.tests.gcov_executable
 
         if gcov_executable != "":
             cmd.extend(["--gcov-executable", gcov_executable])
 
         subprocess.check_call(cmd, cwd=cwd)
@@ -114,16 +123,15 @@
     cmd = [
         "gcovr",
         "-r",
         "it",
         ".",
         "--txt",
         "it-coverage.txt",
-        "--html",
-        "it-coverage.html",
+        "--html=it-coverage.html",
     ]
 
     gcov_executable = config.tests.gcov_executable
 
     if gcov_executable != "":
         cmd.extend(["--gcov-executable", gcov_executable])
```

### Comparing `scargo-1.5.0/scargo/commands/update.py` & `scargo-1.6.0/scargo/commands/update.py`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/config.py` & `scargo-1.6.0/scargo/config.py`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/config_utils.py` & `scargo-1.6.0/scargo/config_utils.py`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/docker_utils.py` & `scargo-1.6.0/scargo/docker_utils.py`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/file_generators/base_gen.py` & `scargo-1.6.0/scargo/file_generators/base_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/file_generators/clang_parser/data_classes.py` & `scargo-1.6.0/scargo/file_generators/clang_parser/data_classes.py`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/file_generators/clang_parser/header_parser.py` & `scargo-1.6.0/scargo/file_generators/clang_parser/header_parser.py`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/file_generators/clang_parser/params_extractor.py` & `scargo-1.6.0/scargo/file_generators/clang_parser/params_extractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,17 @@
         and descendant.location.file.name == filename  # type: ignore[attr-defined]
     ]
 
 
 def extract_classes(cursor: Cursor, filename: str) -> List[ClassDescriptor]:
     return [
         ClassDescriptor(
-            cursor.spelling, f"Mock{cursor.spelling}", _extract_cxx_methods(cursor)
+            descendant.spelling,
+            f"Mock{descendant.spelling}",
+            _extract_cxx_methods(descendant),
         )
         for descendant in cursor.walk_preorder()
         if descendant.kind == CursorKind.CLASS_DECL
         and descendant.location.file.name == filename  # type: ignore[attr-defined]
     ]
```

### Comparing `scargo-1.5.0/scargo/file_generators/conan_gen.py` & `scargo-1.6.0/scargo/file_generators/conan_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/file_generators/cpp_gen.py` & `scargo-1.6.0/scargo/file_generators/cpp_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/file_generators/docker_gen.py` & `scargo-1.6.0/scargo/file_generators/docker_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/file_generators/env_gen.py` & `scargo-1.6.0/scargo/file_generators/env_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/file_generators/mock_gen.py` & `scargo-1.6.0/scargo/file_generators/mock_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/file_generators/templates/.gitlab-ci.yml.j2` & `scargo-1.6.0/scargo/file_generators/templates/.gitlab-ci.yml.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/file_generators/templates/CMakeLists.txt.j2` & `scargo-1.6.0/scargo/file_generators/templates/CMakeLists.txt.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/file_generators/templates/README.md.j2` & `scargo-1.6.0/scargo/file_generators/templates/README.md.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/file_generators/templates/conan/conanfile.py.j2` & `scargo-1.6.0/scargo/file_generators/templates/conan/conanfile.py.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/file_generators/templates/conan/conanfiletest.j2` & `scargo-1.6.0/scargo/file_generators/templates/conan/conanfiletest.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/file_generators/templates/cpp/cmake-src-stm32.j2` & `scargo-1.6.0/scargo/file_generators/templates/cpp/cmake-src-stm32.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/file_generators/templates/cpp/cmake-src-x86.j2` & `scargo-1.6.0/scargo/file_generators/templates/cpp/cmake-src-x86.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/file_generators/templates/cpp/main.cpp.j2` & `scargo-1.6.0/scargo/file_generators/templates/cpp/main.cpp.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/file_generators/templates/docker/Dockerfile-esp32.j2` & `scargo-1.6.0/scargo/file_generators/templates/docker/Dockerfile-esp32.j2`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # esp-idf dependencies, https://docs.espressif.com/projects/esp-idf/en/latest/esp32/get-started/linux-macos-setup.html
-RUN apt update --fix-missing && apt -y --no-install-recommends install git wget flex bison gperf python3 python3-venv cmake ninja-build ccache libffi-dev libssl-dev dfu-util libusb-1.0-0 \
+# libpython2.7 required by xtensa-esp32-elf-gdb
+RUN apt update --fix-missing && apt -y --no-install-recommends install git wget flex bison gperf python3 python3-venv cmake ninja-build ccache libffi-dev libssl-dev dfu-util libusb-1.0-0 libpython2.7 \
     curl openocd && \
     rm -rf /var/lib/apt/lists/*
 
 ARG ESPRESSIF_IDF_TAG="v4.4.3"
 ARG ESPRESSIF_IDF_VERSION="${ESPRESSIF_IDF_TAG}"
 ARG ESPRESSIF_IDF_PATH="/opt/esp-idf"
 ARG ESPRESSIF_IDF_REPO_URL="https://github.com/espressif/esp-idf.git"
```

### Comparing `scargo-1.5.0/scargo/file_generators/templates/docker/Dockerfile-stm32.j2` & `scargo-1.6.0/scargo/file_generators/templates/docker/Dockerfile-stm32.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/file_generators/templates/docker/Dockerfile.j2` & `scargo-1.6.0/scargo/file_generators/templates/docker/Dockerfile.j2`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     apt -y install sudo && \
     rm -rf /var/lib/apt/lists/* && \
     update-alternatives --install /usr/bin/python python /usr/bin/python3 1
 
 FROM base AS cpp
 
 RUN apt update --fix-missing && apt -y --no-install-recommends install cppcheck lib32z1 \
-    make cmake clang clang-format clang-tidy gcovr doxygen libcmocka0 libcmocka-dev && \
+    make cmake clang clang-format clang-tidy gcovr doxygen libcmocka0 libcmocka-dev gdb && \
     rm -rf /var/lib/apt/lists/*
 
 FROM cpp AS {{ project.target.family }}
 {% include 'docker/Dockerfile-' + project.target.family + '.j2' %}
 
 WORKDIR /opt
```

### Comparing `scargo-1.5.0/scargo/file_generators/templates/docker/docker-compose.yaml.j2` & `scargo-1.6.0/scargo/file_generators/templates/docker/docker-compose.yaml.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/file_generators/templates/mock/class_interface.h.j2` & `scargo-1.6.0/scargo/file_generators/templates/mock/class_interface.h.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/file_generators/templates/mock/class_mock.cpp.j2` & `scargo-1.6.0/scargo/file_generators/templates/mock/class_mock.cpp.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/file_generators/templates/mock/class_mock.h.j2` & `scargo-1.6.0/scargo/file_generators/templates/mock/class_mock.h.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/file_generators/templates/scargo.toml.j2` & `scargo-1.6.0/scargo/file_generators/templates/scargo.toml.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/file_generators/templates/stm32.cmake.j2` & `scargo-1.6.0/scargo/file_generators/templates/stm32.cmake.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/file_generators/templates/tests/CMakeLists-test.txt.j2` & `scargo-1.6.0/scargo/file_generators/templates/tests/CMakeLists-test.txt.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/file_generators/templates/tests/static_mock/static_mock.h` & `scargo-1.6.0/scargo/file_generators/templates/tests/static_mock/static_mock.h`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/file_generators/templates/ut/CMakeLists.txt.j2` & `scargo-1.6.0/scargo/file_generators/templates/ut/CMakeLists.txt.j2`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/file_generators/templates/ut/ut.cpp.j2` & `scargo-1.6.0/scargo/file_generators/templates/ut/ut.cpp.j2`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
  */
 
 #include <gtest/gtest.h>
 #include <memory>
 {% for inc in header.includes %}
 #include "{{inc.name}}"
 {% endfor %}
-// #include "{{header.name}}"
+#include "{{header.name}}"
 
 {% if header.namespaces %}
 {% for namespace in header.namespaces %}
 using namespace {{namespace.name}};
 {% endfor %}
 {% endif %}
 using namespace ::testing;
```

### Comparing `scargo-1.5.0/scargo/file_generators/tests_gen.py` & `scargo-1.6.0/scargo/file_generators/tests_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/file_generators/toml_gen.py` & `scargo-1.6.0/scargo/file_generators/toml_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/file_generators/ut_gen.py` & `scargo-1.6.0/scargo/file_generators/ut_gen.py`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/global_values.py` & `scargo-1.6.0/scargo/global_values.py`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/logger.py` & `scargo-1.6.0/scargo/logger.py`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/path_utils.py` & `scargo-1.6.0/scargo/path_utils.py`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/templates/.clang-format` & `scargo-1.6.0/scargo/templates/.clang-format`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/templates/.clang-tidy` & `scargo-1.6.0/scargo/templates/.clang-tidy`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/templates/.gitignore` & `scargo-1.6.0/scargo/templates/.gitignore`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/scargo/templates/LICENSE` & `scargo-1.6.0/scargo/templates/LICENSE`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/setup.cfg` & `scargo-1.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `scargo-1.5.0/PKG-INFO` & `scargo-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scargo
-Version: 1.5.0
+Version: 1.6.0
 Summary: C/C++ package and software development life cycle manager inspired by RUST cargo idea.
 Keywords: scargo,Package manager,C++
 Author-email: "Spyrosoft Solutions S.A." <aak@spyro-soft.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -86,15 +86,15 @@
 # Installation
 Scargo is available on [pypi](https://pypi.org/project/scargo/), so you can install it with pip:
 
 ```pip install scargo```
 
 # Working with scargo
 You can find all information on how to work with scargo on official documentation webpage: https://spyro-soft.github.io/scargo/index.html
-![Scargo flow gif](https://raw.githubusercontent.com/Spyro-Soft/scargo/develop/docs/source/_static/scargo_flow_docker.gif)
+![Scargo flow animation](https://raw.githubusercontent.com/Spyro-Soft/scargo/develop/docs/source/_static/scargo_flow_docker.svg)
 
 # Project dependencies
 ## Working with docker (recommended)
 - docker
 - docker-compose
 - pip
 - python3
```

