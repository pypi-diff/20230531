# Comparing `tmp/langdash-0.0.3.dev1.tar.gz` & `tmp/langdash-0.0.3.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langdash-0.0.3.dev1.tar", last modified: Wed May 31 00:48:39 2023, max compression
+gzip compressed data, was "langdash-0.0.3.dev2.tar", last modified: Wed May 31 00:51:49 2023, max compression
```

## Comparing `langdash-0.0.3.dev1.tar` & `langdash-0.0.3.dev2.tar`

### file list

```diff
@@ -1,257 +1,257 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.712409 langdash-0.0.3.dev1/
--rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-0.0.3.dev1/LICENSE.txt
--rw-rw-r--   0 user      (1000) user      (1000)     3436 2023-05-31 00:48:39.712409 langdash-0.0.3.dev1/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     2670 2023-05-30 08:29:06.000000 langdash-0.0.3.dev1/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.628407 langdash-0.0.3.dev1/langdash/
--rw-rw-r--   0 user      (1000) user      (1000)       31 2023-05-25 22:58:46.000000 langdash-0.0.3.dev1/langdash/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3596 2023-05-30 19:46:43.000000 langdash-0.0.3.dev1/langdash/_langdash.py
--rw-rw-r--   0 user      (1000) user      (1000)    16507 2023-05-30 22:12:14.000000 langdash-0.0.3.dev1/langdash/chains.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.628407 langdash-0.0.3.dev1/langdash/classify/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-0.0.3.dev1/langdash/classify/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1780 2023-05-28 17:07:24.000000 langdash-0.0.3.dev1/langdash/classify/token_qa.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.620406 langdash-0.0.3.dev1/langdash/extern/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.636407 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/
--rw-rw-r--   0 user      (1000) user      (1000)    16349 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeCache.txt
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.636407 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.636407 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/
--rw-r--r--   0 user      (1000) user      (1000)     2441 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeCCompiler.cmake
--rw-r--r--   0 user      (1000) user      (1000)     5439 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeCXXCompiler.cmake
--rwxrwxr-x   0 user      (1000) user      (1000)    15968 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeDetermineCompilerABI_C.bin
--rwxrwxr-x   0 user      (1000) user      (1000)    15992 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeDetermineCompilerABI_CXX.bin
--rw-r--r--   0 user      (1000) user      (1000)      402 2023-05-25 00:05:29.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeSystem.cmake
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.636407 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdC/
--rw-rw-r--   0 user      (1000) user      (1000)    24853 2023-05-25 00:05:29.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdC/CMakeCCompilerId.c
--rwxrwxr-x   0 user      (1000) user      (1000)    16088 2023-05-25 00:05:29.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdC/a.out
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.640407 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdCXX/
--rw-rw-r--   0 user      (1000) user      (1000)    24597 2023-05-25 00:05:29.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdCXX/CMakeCXXCompilerId.cpp
--rwxrwxr-x   0 user      (1000) user      (1000)    16096 2023-05-25 00:05:29.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdCXX/a.out
--rw-rw-r--   0 user      (1000) user      (1000)      706 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/CMakeDirectoryInformation.cmake
--rw-rw-r--   0 user      (1000) user      (1000)    50084 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/CMakeOutput.log
--rw-rw-r--   0 user      (1000) user      (1000)     7911 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/Makefile.cmake
--rw-rw-r--   0 user      (1000) user      (1000)     9844 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/Makefile2
--rw-rw-r--   0 user      (1000) user      (1000)     3155 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/TargetDirectories.txt
--rw-rw-r--   0 user      (1000) user      (1000)       85 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/cmake.check_cache
--rw-rw-r--   0 user      (1000) user      (1000)        2 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/progress.marks
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.640407 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/
--rw-rw-r--   0 user      (1000) user      (1000)      692 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/DependInfo.cmake
--rw-rw-r--   0 user      (1000) user      (1000)     4674 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/build.make
--rw-rw-r--   0 user      (1000) user      (1000)      276 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/cmake_clean.cmake
--rw-rw-r--   0 user      (1000) user      (1000)      107 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/compiler_depend.make
--rw-rw-r--   0 user      (1000) user      (1000)      111 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/compiler_depend.ts
--rw-rw-r--   0 user      (1000) user      (1000)       88 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/depend.make
--rw-rw-r--   0 user      (1000) user      (1000)      679 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/flags.make
--rw-rw-r--   0 user      (1000) user      (1000)      133 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/link.txt
--rw-rw-r--   0 user      (1000) user      (1000)       43 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/progress.make
--rw-rw-r--   0 user      (1000) user      (1000)   101576 2023-05-25 00:05:37.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/rwkv.cpp.o
--rw-rw-r--   0 user      (1000) user      (1000)    11910 2023-05-25 00:05:37.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/rwkv.cpp.o.d
--rw-rw-r--   0 user      (1000) user      (1000)     6908 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)      376 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CTestTestfile.cmake
--rw-rw-r--   0 user      (1000) user      (1000)     1338 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/FILE_FORMAT.md
--rw-rw-r--   0 user      (1000) user      (1000)     1067 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)     8978 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/Makefile
--rw-rw-r--   0 user      (1000) user      (1000)     6412 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.640407 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)   165600 2023-05-25 00:05:38.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/bin/test_ggml_basics
--rwxrwxr-x   0 user      (1000) user      (1000)    16728 2023-05-25 00:05:38.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/bin/test_tiny_rwkv
--rw-rw-r--   0 user      (1000) user      (1000)     2013 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/cmake_install.cmake
--rw-rw-r--   0 user      (1000) user      (1000)     3799 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/compile_commands.json
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.644407 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.644407 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/CMakeFiles/
--rw-rw-r--   0 user      (1000) user      (1000)      706 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/CMakeFiles/CMakeDirectoryInformation.cmake
--rw-rw-r--   0 user      (1000) user      (1000)        2 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/CMakeFiles/progress.marks
--rw-rw-r--   0 user      (1000) user      (1000)     2552 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)     1072 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)     7013 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/Makefile
--rw-rw-r--   0 user      (1000) user      (1000)     3707 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.644407 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/cmake/
--rw-rw-r--   0 user      (1000) user      (1000)     2037 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/cmake/BuildTypes.cmake
--rw-rw-r--   0 user      (1000) user      (1000)      717 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/cmake/GitVars.cmake
--rw-rw-r--   0 user      (1000) user      (1000)     1496 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/cmake_install.cmake
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.644407 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/
--rw-rw-r--   0 user      (1000) user      (1000)      433 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)     8583 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/common-ggml.cpp
--rw-rw-r--   0 user      (1000) user      (1000)      410 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/common-ggml.h
--rw-rw-r--   0 user      (1000) user      (1000)    15664 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/common.cpp
--rw-rw-r--   0 user      (1000) user      (1000)     3311 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/common.h
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.644407 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/
--rw-rw-r--   0 user      (1000) user      (1000)      319 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)     6201 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/README.md
--rw-rw-r--   0 user      (1000) user      (1000)     3490 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/convert-h5-to-ggml.py
--rw-rw-r--   0 user      (1000) user      (1000)    28339 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/main.cpp
--rw-rw-r--   0 user      (1000) user      (1000)     5200 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/quantize.cpp
--rw-rw-r--   0 user      (1000) user      (1000)   241358 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/dr_wav.h
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.648407 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/
--rw-rw-r--   0 user      (1000) user      (1000)      311 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)     6370 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/README.md
--rw-rw-r--   0 user      (1000) user      (1000)     6313 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/convert-cerebras-to-ggml.py
--rw-rw-r--   0 user      (1000) user      (1000)     4873 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/convert-ckpt-to-ggml.py
--rw-rw-r--   0 user      (1000) user      (1000)     6436 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/convert-h5-to-ggml.py
--rwxrwxr-x   0 user      (1000) user      (1000)     1752 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/download-ggml-model.sh
--rwxrwxr-x   0 user      (1000) user      (1000)     1117 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/download-model.sh
--rw-rw-r--   0 user      (1000) user      (1000)    29187 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/main.cpp
--rw-rw-r--   0 user      (1000) user      (1000)     5467 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/quantize.cpp
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.648407 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/
--rw-rw-r--   0 user      (1000) user      (1000)      311 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)    11108 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/README.md
--rw-rw-r--   0 user      (1000) user      (1000)     5509 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/convert-h5-to-ggml.py
--rwxrwxr-x   0 user      (1000) user      (1000)     1728 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/download-ggml-model.sh
--rwxrwxr-x   0 user      (1000) user      (1000)      571 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/download-model.sh
--rw-rw-r--   0 user      (1000) user      (1000)    25782 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/main.cpp
--rw-rw-r--   0 user      (1000) user      (1000)     5469 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/quantize.cpp
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.648407 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/
--rw-rw-r--   0 user      (1000) user      (1000)      133 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)     3689 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/README.md
--rw-rw-r--   0 user      (1000) user      (1000)     1491 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/convert-h5-to-ggml.py
--rw-rw-r--   0 user      (1000) user      (1000)     7679 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/main.cpp
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.624406 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/models/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.652407 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/models/mnist/
--rw-rw-r--   0 user      (1000) user      (1000)  1591571 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/models/mnist/mnist_model.state_dict
--rw-rw-r--   0 user      (1000) user      (1000)  7840016 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/models/mnist/t10k-images.idx3-ubyte
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.668408 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/stablelm/
--rw-rw-r--   0 user      (1000) user      (1000)      323 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/stablelm/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)     4755 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/stablelm/README.md
--rw-rw-r--   0 user      (1000) user      (1000)     3490 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/stablelm/convert-h5-to-ggml.py
--rw-rw-r--   0 user      (1000) user      (1000)    27316 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/stablelm/main.cpp
--rw-rw-r--   0 user      (1000) user      (1000)     5200 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/stablelm/quantize.cpp
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.672408 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/
--rw-rw-r--   0 user      (1000) user      (1000)      501 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)      718 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/README.md
--rw-rw-r--   0 user      (1000) user      (1000)     9506 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/convert-pt-to-ggml.py
--rw-rw-r--   0 user      (1000) user      (1000)    36271 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/main.cpp
--rw-rw-r--   0 user      (1000) user      (1000)     7693 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/quantize.cpp
--rw-rw-r--   0 user      (1000) user      (1000)   184690 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/whisper.cpp
--rw-rw-r--   0 user      (1000) user      (1000)    23750 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/whisper.h
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.624406 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/include/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.672408 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/include/ggml/
--rw-rw-r--   0 user      (1000) user      (1000)    31202 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/include/ggml/ggml.h
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.672408 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/scripts/
--rwxrwxr-x   0 user      (1000) user      (1000)      323 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/scripts/sync-llama.sh
--rwxrwxr-x   0 user      (1000) user      (1000)      921 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/scripts/sync-whisper.sh
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.676408 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.676408 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/
--rw-rw-r--   0 user      (1000) user      (1000)      706 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/CMakeDirectoryInformation.cmake
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.680408 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/
--rw-rw-r--   0 user      (1000) user      (1000)      597 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/DependInfo.cmake
--rw-rw-r--   0 user      (1000) user      (1000)     5420 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/build.make
--rw-rw-r--   0 user      (1000) user      (1000)      269 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/cmake_clean.cmake
--rw-rw-r--   0 user      (1000) user      (1000)       36 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/cmake_clean_target.cmake
--rw-rw-r--   0 user      (1000) user      (1000)      107 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/compiler_depend.make
--rw-rw-r--   0 user      (1000) user      (1000)      111 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/compiler_depend.ts
--rw-rw-r--   0 user      (1000) user      (1000)       88 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/depend.make
--rw-rw-r--   0 user      (1000) user      (1000)     1057 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/flags.make
--rw-rw-r--   0 user      (1000) user      (1000)   201672 2023-05-25 00:05:35.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/ggml.c.o
--rw-rw-r--   0 user      (1000) user      (1000)    10631 2023-05-25 00:05:35.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/ggml.c.o.d
--rw-rw-r--   0 user      (1000) user      (1000)       80 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/link.txt
--rw-rw-r--   0 user      (1000) user      (1000)       43 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/progress.make
--rw-rw-r--   0 user      (1000) user      (1000)        2 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/progress.marks
--rw-rw-r--   0 user      (1000) user      (1000)     8040 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)     8522 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/Makefile
--rw-rw-r--   0 user      (1000) user      (1000)     1573 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/cmake_install.cmake
--rw-rw-r--   0 user      (1000) user      (1000)    24594 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/ggml-cuda.cu
--rw-rw-r--   0 user      (1000) user      (1000)      638 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/ggml-cuda.h
--rw-rw-r--   0 user      (1000) user      (1000)    13447 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/ggml-opencl.c
--rw-rw-r--   0 user      (1000) user      (1000)      639 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/ggml-opencl.h
--rw-rw-r--   0 user      (1000) user      (1000)   428283 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/ggml.c
--rw-rw-r--   0 user      (1000) user      (1000)   205118 2023-05-25 00:05:35.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/libggml.a
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.684408 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/
--rw-rw-r--   0 user      (1000) user      (1000)     9198 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)     6569 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-blas0.c
--rw-rw-r--   0 user      (1000) user      (1000)    11463 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-grad0.c
--rw-rw-r--   0 user      (1000) user      (1000)    10265 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-mul-mat0.c
--rw-rw-r--   0 user      (1000) user      (1000)     9003 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-mul-mat1.c
--rw-rw-r--   0 user      (1000) user      (1000)    91837 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-mul-mat2.c
--rw-rw-r--   0 user      (1000) user      (1000)     5141 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-svd0.c
--rw-rw-r--   0 user      (1000) user      (1000)     3157 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-vec0.c
--rw-rw-r--   0 user      (1000) user      (1000)    21179 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-vec1.c
--rw-rw-r--   0 user      (1000) user      (1000)     7310 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-vec2.c
--rw-rw-r--   0 user      (1000) user      (1000)     1182 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test0.c
--rw-rw-r--   0 user      (1000) user      (1000)    15073 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test1.c
--rw-rw-r--   0 user      (1000) user      (1000)     5703 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test2.c
--rw-rw-r--   0 user      (1000) user      (1000)     2841 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test3.c
--rwxrwxr-x   0 user      (1000) user      (1000)   243024 2023-05-25 00:05:38.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/librwkv.so
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.688408 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/
--rw-rw-r--   0 user      (1000) user      (1000)  2467981 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/20B_tokenizer.json
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.692408 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/__pycache__/
--rw-rw-r--   0 user      (1000) user      (1000)     4174 2023-05-25 00:05:38.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/__pycache__/rwkv_cpp_model.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)     6921 2023-05-25 00:05:39.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/__pycache__/rwkv_cpp_shared_library.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)     8813 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/chat_with_bot.py
--rw-rw-r--   0 user      (1000) user      (1000)     3320 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/convert_pytorch_to_ggml.py
--rw-rw-r--   0 user      (1000) user      (1000)     1463 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/convert_pytorch_to_ggml.test.py
--rw-rw-r--   0 user      (1000) user      (1000)     2380 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/generate_completions.py
--rw-rw-r--   0 user      (1000) user      (1000)     3886 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/measure_pexplexity.py
--rw-rw-r--   0 user      (1000) user      (1000)     5833 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/merge_lora_into_ggml.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.692408 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/prompt/
--rw-rw-r--   0 user      (1000) user      (1000)      947 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/prompt/Chinese-Chat.json
--rw-rw-r--   0 user      (1000) user      (1000)      139 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/prompt/Chinese-QA.json
--rw-rw-r--   0 user      (1000) user      (1000)     1095 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/prompt/English-Chat.json
--rw-rw-r--   0 user      (1000) user      (1000)      764 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/prompt/English-QA.json
--rw-rw-r--   0 user      (1000) user      (1000)     1433 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/prompt/Japanese-Chat.json
--rw-rw-r--   0 user      (1000) user      (1000)      979 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/prompt/Japanese-QA.json
--rw-rw-r--   0 user      (1000) user      (1000)     1106 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/quantize.py
--rw-rw-r--   0 user      (1000) user      (1000)       23 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/requirements.txt
--rw-rw-r--   0 user      (1000) user      (1000)     4359 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/rwkv_cpp_model.py
--rw-rw-r--   0 user      (1000) user      (1000)     7528 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/rwkv_cpp_shared_library.py
--rw-rw-r--   0 user      (1000) user      (1000)     1255 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/sampling.py
--rw-rw-r--   0 user      (1000) user      (1000)    39641 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv.cpp
--rw-rw-r--   0 user      (1000) user      (1000)     4691 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv.h
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.696409 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.704409 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/
--rw-rw-r--   0 user      (1000) user      (1000)      706 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/CMakeDirectoryInformation.cmake
--rw-rw-r--   0 user      (1000) user      (1000)        2 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/progress.marks
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.708409 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/
--rw-rw-r--   0 user      (1000) user      (1000)      871 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/DependInfo.cmake
--rw-rw-r--   0 user      (1000) user      (1000)     5923 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/build.make
--rw-rw-r--   0 user      (1000) user      (1000)      359 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/cmake_clean.cmake
--rw-rw-r--   0 user      (1000) user      (1000)      119 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/compiler_depend.make
--rw-rw-r--   0 user      (1000) user      (1000)      123 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/compiler_depend.ts
--rw-rw-r--   0 user      (1000) user      (1000)      100 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/depend.make
--rw-rw-r--   0 user      (1000) user      (1000)      670 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/flags.make
--rw-rw-r--   0 user      (1000) user      (1000)      224 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/link.txt
--rw-rw-r--   0 user      (1000) user      (1000)       43 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/progress.make
--rw-rw-r--   0 user      (1000) user      (1000)     5152 2023-05-25 00:05:38.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/test_ggml_basics.c.o
--rw-rw-r--   0 user      (1000) user      (1000)     3717 2023-05-25 00:05:38.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/test_ggml_basics.c.o.d
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.712409 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/
--rw-rw-r--   0 user      (1000) user      (1000)      861 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/DependInfo.cmake
--rw-rw-r--   0 user      (1000) user      (1000)     5799 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/build.make
--rw-rw-r--   0 user      (1000) user      (1000)      345 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/cmake_clean.cmake
--rw-rw-r--   0 user      (1000) user      (1000)      117 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/compiler_depend.make
--rw-rw-r--   0 user      (1000) user      (1000)      121 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/compiler_depend.ts
--rw-rw-r--   0 user      (1000) user      (1000)       98 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/depend.make
--rw-rw-r--   0 user      (1000) user      (1000)      670 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/flags.make
--rw-rw-r--   0 user      (1000) user      (1000)      218 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/link.txt
--rw-rw-r--   0 user      (1000) user      (1000)       43 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/progress.make
--rw-rw-r--   0 user      (1000) user      (1000)     9816 2023-05-25 00:05:38.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/test_tiny_rwkv.c.o
--rw-rw-r--   0 user      (1000) user      (1000)     4064 2023-05-25 00:05:38.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/test_tiny_rwkv.c.o.d
--rw-rw-r--   0 user      (1000) user      (1000)      577 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)     1309 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CTestTestfile.cmake
--rw-rw-r--   0 user      (1000) user      (1000)    10760 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/Makefile
--rw-rw-r--   0 user      (1000) user      (1000)     1292 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/cmake_install.cmake
--rw-rw-r--   0 user      (1000) user      (1000)     1024 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/expected_logits.bin
--rw-rw-r--   0 user      (1000) user      (1000)     1724 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/test_ggml_basics.c
--rw-rw-r--   0 user      (1000) user      (1000)     5039 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/test_tiny_rwkv.c
--rw-rw-r--   0 user      (1000) user      (1000)  1338429 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/tiny-rwkv-660K-FP16.bin
--rw-rw-r--   0 user      (1000) user      (1000)  2649149 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/tiny-rwkv-660K-FP32.bin
--rw-rw-r--   0 user      (1000) user      (1000)      217 2023-05-30 08:12:32.000000 langdash-0.0.3.dev1/langdash/infer.py
--rw-rw-r--   0 user      (1000) user      (1000)     1209 2023-05-30 19:56:33.000000 langdash-0.0.3.dev1/langdash/llm.py
--rw-rw-r--   0 user      (1000) user      (1000)     7101 2023-05-30 20:56:47.000000 langdash-0.0.3.dev1/langdash/llm_session.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.628407 langdash-0.0.3.dev1/langdash/models/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:36.000000 langdash-0.0.3.dev1/langdash/models/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      624 2023-05-25 22:58:44.000000 langdash-0.0.3.dev1/langdash/models/mock.py
--rw-rw-r--   0 user      (1000) user      (1000)     6964 2023-05-30 22:08:25.000000 langdash-0.0.3.dev1/langdash/models/rwkvcpp.py
--rw-rw-r--   0 user      (1000) user      (1000)      840 2023-05-29 18:14:56.000000 langdash-0.0.3.dev1/langdash/models/sentence_transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     6051 2023-05-30 22:02:01.000000 langdash-0.0.3.dev1/langdash/models/transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)      259 2023-05-25 22:58:46.000000 langdash-0.0.3.dev1/langdash/response.py
--rw-rw-r--   0 user      (1000) user      (1000)     2154 2023-05-30 19:25:05.000000 langdash-0.0.3.dev1/langdash/sampling.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.632407 langdash-0.0.3.dev1/langdash/search/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-0.0.3.dev1/langdash/search/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      840 2023-05-29 19:25:03.000000 langdash-0.0.3.dev1/langdash/search/embedding_search.py
--rw-rw-r--   0 user      (1000) user      (1000)      260 2023-05-27 05:17:38.000000 langdash-0.0.3.dev1/langdash/search/engine.py
--rw-rw-r--   0 user      (1000) user      (1000)     2391 2023-05-28 22:28:07.000000 langdash-0.0.3.dev1/langdash/search/multichoice_search.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.632407 langdash-0.0.3.dev1/langdash.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     3436 2023-05-31 00:48:39.000000 langdash-0.0.3.dev1/langdash.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    12207 2023-05-31 00:48:39.000000 langdash-0.0.3.dev1/langdash.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-31 00:48:39.000000 langdash-0.0.3.dev1/langdash.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      124 2023-05-31 00:48:39.000000 langdash-0.0.3.dev1/langdash.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        9 2023-05-31 00:48:39.000000 langdash-0.0.3.dev1/langdash.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-05-31 00:48:39.712409 langdash-0.0.3.dev1/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1262 2023-05-31 00:47:19.000000 langdash-0.0.3.dev1/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.662254 langdash-0.0.3.dev2/
+-rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-0.0.3.dev2/LICENSE.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     3436 2023-05-31 00:51:49.662254 langdash-0.0.3.dev2/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     2670 2023-05-30 08:29:06.000000 langdash-0.0.3.dev2/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.590252 langdash-0.0.3.dev2/langdash/
+-rw-rw-r--   0 user      (1000) user      (1000)       31 2023-05-25 22:58:46.000000 langdash-0.0.3.dev2/langdash/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3596 2023-05-30 19:46:43.000000 langdash-0.0.3.dev2/langdash/_langdash.py
+-rw-rw-r--   0 user      (1000) user      (1000)    16507 2023-05-30 22:12:14.000000 langdash-0.0.3.dev2/langdash/chains.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.594252 langdash-0.0.3.dev2/langdash/classify/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-0.0.3.dev2/langdash/classify/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1780 2023-05-28 17:07:24.000000 langdash-0.0.3.dev2/langdash/classify/token_qa.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.586251 langdash-0.0.3.dev2/langdash/extern/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.598252 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/
+-rw-rw-r--   0 user      (1000) user      (1000)    16349 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeCache.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.598252 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.602252 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/
+-rw-r--r--   0 user      (1000) user      (1000)     2441 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeCCompiler.cmake
+-rw-r--r--   0 user      (1000) user      (1000)     5439 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeCXXCompiler.cmake
+-rwxrwxr-x   0 user      (1000) user      (1000)    15968 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeDetermineCompilerABI_C.bin
+-rwxrwxr-x   0 user      (1000) user      (1000)    15992 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeDetermineCompilerABI_CXX.bin
+-rw-r--r--   0 user      (1000) user      (1000)      402 2023-05-25 00:05:29.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeSystem.cmake
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.602252 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdC/
+-rw-rw-r--   0 user      (1000) user      (1000)    24853 2023-05-25 00:05:29.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdC/CMakeCCompilerId.c
+-rwxrwxr-x   0 user      (1000) user      (1000)    16088 2023-05-25 00:05:29.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdC/a.out
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.602252 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdCXX/
+-rw-rw-r--   0 user      (1000) user      (1000)    24597 2023-05-25 00:05:29.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdCXX/CMakeCXXCompilerId.cpp
+-rwxrwxr-x   0 user      (1000) user      (1000)    16096 2023-05-25 00:05:29.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdCXX/a.out
+-rw-rw-r--   0 user      (1000) user      (1000)      706 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/CMakeDirectoryInformation.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)    50084 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/CMakeOutput.log
+-rw-rw-r--   0 user      (1000) user      (1000)     7911 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/Makefile.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)     9844 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/Makefile2
+-rw-rw-r--   0 user      (1000) user      (1000)     3155 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/TargetDirectories.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       85 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/cmake.check_cache
+-rw-rw-r--   0 user      (1000) user      (1000)        2 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/progress.marks
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.602252 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/
+-rw-rw-r--   0 user      (1000) user      (1000)      692 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/DependInfo.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)     4674 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/build.make
+-rw-rw-r--   0 user      (1000) user      (1000)      276 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/cmake_clean.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)      107 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/compiler_depend.make
+-rw-rw-r--   0 user      (1000) user      (1000)      111 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/compiler_depend.ts
+-rw-rw-r--   0 user      (1000) user      (1000)       88 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/depend.make
+-rw-rw-r--   0 user      (1000) user      (1000)      679 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/flags.make
+-rw-rw-r--   0 user      (1000) user      (1000)      133 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/link.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       43 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/progress.make
+-rw-rw-r--   0 user      (1000) user      (1000)   101576 2023-05-25 00:05:37.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/rwkv.cpp.o
+-rw-rw-r--   0 user      (1000) user      (1000)    11910 2023-05-25 00:05:37.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/rwkv.cpp.o.d
+-rw-rw-r--   0 user      (1000) user      (1000)     6908 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeLists.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      376 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CTestTestfile.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)     1338 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/FILE_FORMAT.md
+-rw-rw-r--   0 user      (1000) user      (1000)     1067 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)     8978 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/Makefile
+-rw-rw-r--   0 user      (1000) user      (1000)     6412 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.606252 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)   165600 2023-05-25 00:05:38.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/bin/test_ggml_basics
+-rwxrwxr-x   0 user      (1000) user      (1000)    16728 2023-05-25 00:05:38.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/bin/test_tiny_rwkv
+-rw-rw-r--   0 user      (1000) user      (1000)     2013 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/cmake_install.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)     3799 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/compile_commands.json
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.606252 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.606252 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/CMakeFiles/
+-rw-rw-r--   0 user      (1000) user      (1000)      706 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/CMakeFiles/CMakeDirectoryInformation.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)        2 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/CMakeFiles/progress.marks
+-rw-rw-r--   0 user      (1000) user      (1000)     2552 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/CMakeLists.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     1072 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)     7013 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/Makefile
+-rw-rw-r--   0 user      (1000) user      (1000)     3707 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.606252 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/cmake/
+-rw-rw-r--   0 user      (1000) user      (1000)     2037 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/cmake/BuildTypes.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)      717 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/cmake/GitVars.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)     1496 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/cmake_install.cmake
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.606252 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/
+-rw-rw-r--   0 user      (1000) user      (1000)      433 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/CMakeLists.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     8583 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/common-ggml.cpp
+-rw-rw-r--   0 user      (1000) user      (1000)      410 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/common-ggml.h
+-rw-rw-r--   0 user      (1000) user      (1000)    15664 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/common.cpp
+-rw-rw-r--   0 user      (1000) user      (1000)     3311 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/common.h
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.610252 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/
+-rw-rw-r--   0 user      (1000) user      (1000)      319 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/CMakeLists.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     6201 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)     3490 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/convert-h5-to-ggml.py
+-rw-rw-r--   0 user      (1000) user      (1000)    28339 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/main.cpp
+-rw-rw-r--   0 user      (1000) user      (1000)     5200 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/quantize.cpp
+-rw-rw-r--   0 user      (1000) user      (1000)   241358 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/dr_wav.h
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.610252 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/
+-rw-rw-r--   0 user      (1000) user      (1000)      311 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/CMakeLists.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     6370 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)     6313 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/convert-cerebras-to-ggml.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4873 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/convert-ckpt-to-ggml.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6436 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/convert-h5-to-ggml.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     1752 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/download-ggml-model.sh
+-rwxrwxr-x   0 user      (1000) user      (1000)     1117 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/download-model.sh
+-rw-rw-r--   0 user      (1000) user      (1000)    29187 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/main.cpp
+-rw-rw-r--   0 user      (1000) user      (1000)     5467 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/quantize.cpp
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.614252 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/
+-rw-rw-r--   0 user      (1000) user      (1000)      311 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/CMakeLists.txt
+-rw-rw-r--   0 user      (1000) user      (1000)    11108 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)     5509 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/convert-h5-to-ggml.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     1728 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/download-ggml-model.sh
+-rwxrwxr-x   0 user      (1000) user      (1000)      571 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/download-model.sh
+-rw-rw-r--   0 user      (1000) user      (1000)    25782 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/main.cpp
+-rw-rw-r--   0 user      (1000) user      (1000)     5469 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/quantize.cpp
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.614252 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/
+-rw-rw-r--   0 user      (1000) user      (1000)      133 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/CMakeLists.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     3689 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)     1491 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/convert-h5-to-ggml.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7679 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/main.cpp
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.586251 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/models/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.618252 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/models/mnist/
+-rw-rw-r--   0 user      (1000) user      (1000)  1591571 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/models/mnist/mnist_model.state_dict
+-rw-rw-r--   0 user      (1000) user      (1000)  7840016 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/models/mnist/t10k-images.idx3-ubyte
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.626253 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/stablelm/
+-rw-rw-r--   0 user      (1000) user      (1000)      323 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/stablelm/CMakeLists.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     4755 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/stablelm/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)     3490 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/stablelm/convert-h5-to-ggml.py
+-rw-rw-r--   0 user      (1000) user      (1000)    27316 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/stablelm/main.cpp
+-rw-rw-r--   0 user      (1000) user      (1000)     5200 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/stablelm/quantize.cpp
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.630253 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/
+-rw-rw-r--   0 user      (1000) user      (1000)      501 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/CMakeLists.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      718 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)     9506 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/convert-pt-to-ggml.py
+-rw-rw-r--   0 user      (1000) user      (1000)    36271 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/main.cpp
+-rw-rw-r--   0 user      (1000) user      (1000)     7693 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/quantize.cpp
+-rw-rw-r--   0 user      (1000) user      (1000)   184690 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/whisper.cpp
+-rw-rw-r--   0 user      (1000) user      (1000)    23750 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/whisper.h
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.586251 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/include/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.630253 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/include/ggml/
+-rw-rw-r--   0 user      (1000) user      (1000)    31202 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/include/ggml/ggml.h
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.630253 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/scripts/
+-rwxrwxr-x   0 user      (1000) user      (1000)      323 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/scripts/sync-llama.sh
+-rwxrwxr-x   0 user      (1000) user      (1000)      921 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/scripts/sync-whisper.sh
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.630253 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.634253 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/
+-rw-rw-r--   0 user      (1000) user      (1000)      706 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/CMakeDirectoryInformation.cmake
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.634253 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/
+-rw-rw-r--   0 user      (1000) user      (1000)      597 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/DependInfo.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)     5420 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/build.make
+-rw-rw-r--   0 user      (1000) user      (1000)      269 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/cmake_clean.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)       36 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/cmake_clean_target.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)      107 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/compiler_depend.make
+-rw-rw-r--   0 user      (1000) user      (1000)      111 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/compiler_depend.ts
+-rw-rw-r--   0 user      (1000) user      (1000)       88 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/depend.make
+-rw-rw-r--   0 user      (1000) user      (1000)     1057 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/flags.make
+-rw-rw-r--   0 user      (1000) user      (1000)   201672 2023-05-25 00:05:35.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/ggml.c.o
+-rw-rw-r--   0 user      (1000) user      (1000)    10631 2023-05-25 00:05:35.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/ggml.c.o.d
+-rw-rw-r--   0 user      (1000) user      (1000)       80 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/link.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       43 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/progress.make
+-rw-rw-r--   0 user      (1000) user      (1000)        2 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/progress.marks
+-rw-rw-r--   0 user      (1000) user      (1000)     8040 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeLists.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     8522 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/Makefile
+-rw-rw-r--   0 user      (1000) user      (1000)     1573 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/cmake_install.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)    24594 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/ggml-cuda.cu
+-rw-rw-r--   0 user      (1000) user      (1000)      638 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/ggml-cuda.h
+-rw-rw-r--   0 user      (1000) user      (1000)    13447 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/ggml-opencl.c
+-rw-rw-r--   0 user      (1000) user      (1000)      639 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/ggml-opencl.h
+-rw-rw-r--   0 user      (1000) user      (1000)   428283 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/ggml.c
+-rw-rw-r--   0 user      (1000) user      (1000)   205118 2023-05-25 00:05:35.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/libggml.a
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.638253 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/
+-rw-rw-r--   0 user      (1000) user      (1000)     9198 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/CMakeLists.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     6569 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-blas0.c
+-rw-rw-r--   0 user      (1000) user      (1000)    11463 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-grad0.c
+-rw-rw-r--   0 user      (1000) user      (1000)    10265 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-mul-mat0.c
+-rw-rw-r--   0 user      (1000) user      (1000)     9003 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-mul-mat1.c
+-rw-rw-r--   0 user      (1000) user      (1000)    91837 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-mul-mat2.c
+-rw-rw-r--   0 user      (1000) user      (1000)     5141 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-svd0.c
+-rw-rw-r--   0 user      (1000) user      (1000)     3157 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-vec0.c
+-rw-rw-r--   0 user      (1000) user      (1000)    21179 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-vec1.c
+-rw-rw-r--   0 user      (1000) user      (1000)     7310 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-vec2.c
+-rw-rw-r--   0 user      (1000) user      (1000)     1182 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/test0.c
+-rw-rw-r--   0 user      (1000) user      (1000)    15073 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/test1.c
+-rw-rw-r--   0 user      (1000) user      (1000)     5703 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/test2.c
+-rw-rw-r--   0 user      (1000) user      (1000)     2841 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/test3.c
+-rwxrwxr-x   0 user      (1000) user      (1000)   243024 2023-05-25 00:05:38.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/librwkv.so
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.646253 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/
+-rw-rw-r--   0 user      (1000) user      (1000)  2467981 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/20B_tokenizer.json
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.646253 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/__pycache__/
+-rw-rw-r--   0 user      (1000) user      (1000)     4174 2023-05-25 00:05:38.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/__pycache__/rwkv_cpp_model.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)     6921 2023-05-25 00:05:39.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/__pycache__/rwkv_cpp_shared_library.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)     8813 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/chat_with_bot.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3320 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/convert_pytorch_to_ggml.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1463 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/convert_pytorch_to_ggml.test.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2380 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/generate_completions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3886 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/measure_pexplexity.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5833 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/merge_lora_into_ggml.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.646253 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/
+-rw-rw-r--   0 user      (1000) user      (1000)      947 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/Chinese-Chat.json
+-rw-rw-r--   0 user      (1000) user      (1000)      139 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/Chinese-QA.json
+-rw-rw-r--   0 user      (1000) user      (1000)     1095 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/English-Chat.json
+-rw-rw-r--   0 user      (1000) user      (1000)      764 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/English-QA.json
+-rw-rw-r--   0 user      (1000) user      (1000)     1433 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/Japanese-Chat.json
+-rw-rw-r--   0 user      (1000) user      (1000)      979 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/Japanese-QA.json
+-rw-rw-r--   0 user      (1000) user      (1000)     1106 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/quantize.py
+-rw-rw-r--   0 user      (1000) user      (1000)       23 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/requirements.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     4359 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/rwkv_cpp_model.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7528 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/rwkv_cpp_shared_library.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1255 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/sampling.py
+-rw-rw-r--   0 user      (1000) user      (1000)    39641 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv.cpp
+-rw-rw-r--   0 user      (1000) user      (1000)     4691 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv.h
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.650254 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.654254 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/
+-rw-rw-r--   0 user      (1000) user      (1000)      706 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/CMakeDirectoryInformation.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)        2 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/progress.marks
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.658254 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/
+-rw-rw-r--   0 user      (1000) user      (1000)      871 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/DependInfo.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)     5923 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/build.make
+-rw-rw-r--   0 user      (1000) user      (1000)      359 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/cmake_clean.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)      119 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/compiler_depend.make
+-rw-rw-r--   0 user      (1000) user      (1000)      123 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/compiler_depend.ts
+-rw-rw-r--   0 user      (1000) user      (1000)      100 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/depend.make
+-rw-rw-r--   0 user      (1000) user      (1000)      670 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/flags.make
+-rw-rw-r--   0 user      (1000) user      (1000)      224 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/link.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       43 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/progress.make
+-rw-rw-r--   0 user      (1000) user      (1000)     5152 2023-05-25 00:05:38.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/test_ggml_basics.c.o
+-rw-rw-r--   0 user      (1000) user      (1000)     3717 2023-05-25 00:05:38.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/test_ggml_basics.c.o.d
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.662254 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/
+-rw-rw-r--   0 user      (1000) user      (1000)      861 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/DependInfo.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)     5799 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/build.make
+-rw-rw-r--   0 user      (1000) user      (1000)      345 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/cmake_clean.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)      117 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/compiler_depend.make
+-rw-rw-r--   0 user      (1000) user      (1000)      121 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/compiler_depend.ts
+-rw-rw-r--   0 user      (1000) user      (1000)       98 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/depend.make
+-rw-rw-r--   0 user      (1000) user      (1000)      670 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/flags.make
+-rw-rw-r--   0 user      (1000) user      (1000)      218 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/link.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       43 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/progress.make
+-rw-rw-r--   0 user      (1000) user      (1000)     9816 2023-05-25 00:05:38.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/test_tiny_rwkv.c.o
+-rw-rw-r--   0 user      (1000) user      (1000)     4064 2023-05-25 00:05:38.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/test_tiny_rwkv.c.o.d
+-rw-rw-r--   0 user      (1000) user      (1000)      577 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeLists.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     1309 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CTestTestfile.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)    10760 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/Makefile
+-rw-rw-r--   0 user      (1000) user      (1000)     1292 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/cmake_install.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)     1024 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/expected_logits.bin
+-rw-rw-r--   0 user      (1000) user      (1000)     1724 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/test_ggml_basics.c
+-rw-rw-r--   0 user      (1000) user      (1000)     5039 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/test_tiny_rwkv.c
+-rw-rw-r--   0 user      (1000) user      (1000)  1338429 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/tiny-rwkv-660K-FP16.bin
+-rw-rw-r--   0 user      (1000) user      (1000)  2649149 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/tiny-rwkv-660K-FP32.bin
+-rw-rw-r--   0 user      (1000) user      (1000)      217 2023-05-30 08:12:32.000000 langdash-0.0.3.dev2/langdash/infer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1209 2023-05-30 19:56:33.000000 langdash-0.0.3.dev2/langdash/llm.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7101 2023-05-30 20:56:47.000000 langdash-0.0.3.dev2/langdash/llm_session.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.594252 langdash-0.0.3.dev2/langdash/models/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:36.000000 langdash-0.0.3.dev2/langdash/models/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      624 2023-05-25 22:58:44.000000 langdash-0.0.3.dev2/langdash/models/mock.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6964 2023-05-30 22:08:25.000000 langdash-0.0.3.dev2/langdash/models/rwkvcpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)      840 2023-05-29 18:14:56.000000 langdash-0.0.3.dev2/langdash/models/sentence_transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6051 2023-05-30 22:02:01.000000 langdash-0.0.3.dev2/langdash/models/transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)      259 2023-05-25 22:58:46.000000 langdash-0.0.3.dev2/langdash/response.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2154 2023-05-30 19:25:05.000000 langdash-0.0.3.dev2/langdash/sampling.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.594252 langdash-0.0.3.dev2/langdash/search/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-0.0.3.dev2/langdash/search/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      840 2023-05-29 19:25:03.000000 langdash-0.0.3.dev2/langdash/search/embedding_search.py
+-rw-rw-r--   0 user      (1000) user      (1000)      260 2023-05-27 05:17:38.000000 langdash-0.0.3.dev2/langdash/search/engine.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2391 2023-05-28 22:28:07.000000 langdash-0.0.3.dev2/langdash/search/multichoice_search.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.594252 langdash-0.0.3.dev2/langdash.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     3436 2023-05-31 00:51:49.000000 langdash-0.0.3.dev2/langdash.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    12207 2023-05-31 00:51:49.000000 langdash-0.0.3.dev2/langdash.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-31 00:51:49.000000 langdash-0.0.3.dev2/langdash.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      124 2023-05-31 00:51:49.000000 langdash-0.0.3.dev2/langdash.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        9 2023-05-31 00:51:49.000000 langdash-0.0.3.dev2/langdash.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-05-31 00:51:49.662254 langdash-0.0.3.dev2/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1282 2023-05-31 00:50:47.000000 langdash-0.0.3.dev2/setup.py
```

### Comparing `langdash-0.0.3.dev1/LICENSE.txt` & `langdash-0.0.3.dev2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/PKG-INFO` & `langdash-0.0.3.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 0.0.3.dev1
+Version: 0.0.3.dev2
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `langdash-0.0.3.dev1/README.md` & `langdash-0.0.3.dev2/README.md`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/_langdash.py` & `langdash-0.0.3.dev2/langdash/_langdash.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/chains.py` & `langdash-0.0.3.dev2/langdash/chains.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/classify/token_qa.py` & `langdash-0.0.3.dev2/langdash/classify/token_qa.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeCache.txt` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeCache.txt`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeCCompiler.cmake` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeCCompiler.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeCXXCompiler.cmake` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeCXXCompiler.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeDetermineCompilerABI_C.bin` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeDetermineCompilerABI_C.bin`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeDetermineCompilerABI_CXX.bin` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeDetermineCompilerABI_CXX.bin`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdC/CMakeCCompilerId.c` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdC/CMakeCCompilerId.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdC/a.out` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdC/a.out`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdCXX/CMakeCXXCompilerId.cpp` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdCXX/CMakeCXXCompilerId.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdCXX/a.out` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdCXX/a.out`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/CMakeDirectoryInformation.cmake` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/CMakeDirectoryInformation.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/CMakeOutput.log` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/CMakeOutput.log`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/Makefile.cmake` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/Makefile.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/Makefile2` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/Makefile2`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/TargetDirectories.txt` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/TargetDirectories.txt`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/DependInfo.cmake` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/DependInfo.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/build.make` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/build.make`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/flags.make` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/flags.make`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/rwkv.cpp.o` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/rwkv.cpp.o`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/rwkv.cpp.o.d` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/rwkv.cpp.o.d`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeLists.txt` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/FILE_FORMAT.md` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/FILE_FORMAT.md`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/LICENSE` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/LICENSE`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/Makefile` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/Makefile`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/README.md` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/README.md`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/bin/test_ggml_basics` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/bin/test_ggml_basics`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/bin/test_tiny_rwkv` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/bin/test_tiny_rwkv`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/cmake_install.cmake` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/cmake_install.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/compile_commands.json` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/compile_commands.json`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/CMakeFiles/CMakeDirectoryInformation.cmake` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/CMakeFiles/CMakeDirectoryInformation.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/CMakeLists.txt` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/LICENSE` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/LICENSE`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/Makefile` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/Makefile`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/README.md` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/README.md`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/cmake/BuildTypes.cmake` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/cmake/BuildTypes.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/cmake/GitVars.cmake` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/cmake/GitVars.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/cmake_install.cmake` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/cmake_install.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/common-ggml.cpp` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/common-ggml.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/common.cpp` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/common.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/common.h` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/common.h`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/README.md` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/README.md`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/convert-h5-to-ggml.py` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/convert-h5-to-ggml.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/main.cpp` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/main.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/quantize.cpp` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/quantize.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/dr_wav.h` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/dr_wav.h`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/README.md` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/README.md`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/convert-cerebras-to-ggml.py` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/convert-cerebras-to-ggml.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/convert-ckpt-to-ggml.py` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/convert-ckpt-to-ggml.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/convert-h5-to-ggml.py` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/convert-h5-to-ggml.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/download-ggml-model.sh` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/download-ggml-model.sh`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/download-model.sh` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/download-model.sh`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/main.cpp` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/main.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/quantize.cpp` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/quantize.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/README.md` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/README.md`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/convert-h5-to-ggml.py` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/convert-h5-to-ggml.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/download-ggml-model.sh` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/download-ggml-model.sh`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/download-model.sh` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/download-model.sh`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/main.cpp` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/main.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/quantize.cpp` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/quantize.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/README.md` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/README.md`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/convert-h5-to-ggml.py` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/convert-h5-to-ggml.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/main.cpp` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/main.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/models/mnist/mnist_model.state_dict` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/models/mnist/mnist_model.state_dict`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/models/mnist/t10k-images.idx3-ubyte` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/models/mnist/t10k-images.idx3-ubyte`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/stablelm/README.md` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/stablelm/README.md`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/stablelm/convert-h5-to-ggml.py` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/stablelm/convert-h5-to-ggml.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/stablelm/main.cpp` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/stablelm/main.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/stablelm/quantize.cpp` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/stablelm/quantize.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/README.md` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/README.md`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/convert-pt-to-ggml.py` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/convert-pt-to-ggml.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/main.cpp` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/main.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/quantize.cpp` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/quantize.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/whisper.cpp` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/whisper.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/whisper.h` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/whisper.h`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/include/ggml/ggml.h` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/include/ggml/ggml.h`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/scripts/sync-whisper.sh` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/scripts/sync-whisper.sh`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/CMakeDirectoryInformation.cmake` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/CMakeDirectoryInformation.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/DependInfo.cmake` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/DependInfo.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/build.make` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/build.make`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/flags.make` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/flags.make`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/ggml.c.o` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/ggml.c.o`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/ggml.c.o.d` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/ggml.c.o.d`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeLists.txt` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/Makefile` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/Makefile`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/cmake_install.cmake` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/cmake_install.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/ggml-cuda.cu` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/ggml-cuda.cu`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/ggml-cuda.h` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/ggml-cuda.h`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/ggml-opencl.c` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/ggml-opencl.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/ggml-opencl.h` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/ggml-opencl.h`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/ggml.c` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/ggml.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/libggml.a` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/libggml.a`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/CMakeLists.txt` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-blas0.c` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-blas0.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-grad0.c` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-grad0.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-mul-mat0.c` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-mul-mat0.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-mul-mat1.c` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-mul-mat1.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-mul-mat2.c` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-mul-mat2.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-svd0.c` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-svd0.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-vec0.c` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-vec0.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-vec1.c` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-vec1.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-vec2.c` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-vec2.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test0.c` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/test0.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test1.c` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/test1.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test2.c` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/test2.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test3.c` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/test3.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/librwkv.so` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/librwkv.so`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/20B_tokenizer.json` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/20B_tokenizer.json`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/__pycache__/rwkv_cpp_model.cpython-310.pyc` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/__pycache__/rwkv_cpp_model.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/__pycache__/rwkv_cpp_shared_library.cpython-310.pyc` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/__pycache__/rwkv_cpp_shared_library.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/chat_with_bot.py` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/chat_with_bot.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/convert_pytorch_to_ggml.py` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/convert_pytorch_to_ggml.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/convert_pytorch_to_ggml.test.py` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/convert_pytorch_to_ggml.test.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/generate_completions.py` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/generate_completions.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/measure_pexplexity.py` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/measure_pexplexity.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/merge_lora_into_ggml.py` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/merge_lora_into_ggml.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/prompt/Chinese-Chat.json` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/Chinese-Chat.json`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/prompt/English-Chat.json` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/English-Chat.json`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/prompt/English-QA.json` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/English-QA.json`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/prompt/Japanese-Chat.json` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/Japanese-Chat.json`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/prompt/Japanese-QA.json` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/Japanese-QA.json`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/quantize.py` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/quantize.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/rwkv_cpp_model.py` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/rwkv_cpp_model.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/rwkv_cpp_shared_library.py` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/rwkv_cpp_shared_library.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/sampling.py` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/sampling.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv.cpp` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv.h` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv.h`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/CMakeDirectoryInformation.cmake` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/CMakeDirectoryInformation.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/DependInfo.cmake` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/DependInfo.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/build.make` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/build.make`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/flags.make` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/flags.make`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/test_ggml_basics.c.o` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/test_ggml_basics.c.o`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/test_ggml_basics.c.o.d` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/test_ggml_basics.c.o.d`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/DependInfo.cmake` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/DependInfo.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/build.make` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/build.make`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/flags.make` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/flags.make`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/test_tiny_rwkv.c.o` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/test_tiny_rwkv.c.o`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/test_tiny_rwkv.c.o.d` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/test_tiny_rwkv.c.o.d`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeLists.txt` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CTestTestfile.cmake` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CTestTestfile.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/Makefile` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/Makefile`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/cmake_install.cmake` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/cmake_install.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/expected_logits.bin` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/expected_logits.bin`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/test_ggml_basics.c` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/test_ggml_basics.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/test_tiny_rwkv.c` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/test_tiny_rwkv.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/tiny-rwkv-660K-FP16.bin` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/tiny-rwkv-660K-FP16.bin`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/tiny-rwkv-660K-FP32.bin` & `langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/tiny-rwkv-660K-FP32.bin`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/llm.py` & `langdash-0.0.3.dev2/langdash/llm.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/llm_session.py` & `langdash-0.0.3.dev2/langdash/llm_session.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/models/mock.py` & `langdash-0.0.3.dev2/langdash/models/mock.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/models/rwkvcpp.py` & `langdash-0.0.3.dev2/langdash/models/rwkvcpp.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/models/sentence_transformers.py` & `langdash-0.0.3.dev2/langdash/models/sentence_transformers.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/models/transformers.py` & `langdash-0.0.3.dev2/langdash/models/transformers.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/sampling.py` & `langdash-0.0.3.dev2/langdash/sampling.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/search/embedding_search.py` & `langdash-0.0.3.dev2/langdash/search/embedding_search.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash/search/multichoice_search.py` & `langdash-0.0.3.dev2/langdash/search/multichoice_search.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/langdash.egg-info/PKG-INFO` & `langdash-0.0.3.dev2/langdash.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 0.0.3.dev1
+Version: 0.0.3.dev2
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `langdash-0.0.3.dev1/langdash.egg-info/SOURCES.txt` & `langdash-0.0.3.dev2/langdash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev1/setup.py` & `langdash-0.0.3.dev2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='langdash',
-    version='0.0.3.dev1',
+    version='0.0.3.dev2',
     description='A simple library for interfacing with language models.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Nana Mochizuki',
     author_email='nana@mysymphony.jp.net',
     url='https://git.mysymphony.jp.net/nana/langdash',
     classifiers=[
@@ -21,15 +21,15 @@
       'Programming Language :: Python :: 3.8',
     ],
     project_urls={
       'Source': 'https://git.mysymphony.jp.net/nana/langdash',
     },
     # requirements
     python_requires='>=3.8',
-    packages=find_packages(include=['langdash', 'langdash.*']),
+    packages=find_packages(include=['langdash', 'langdash.*'], exclude=['extern']),
     install_requires=[
       'torch',
     ],
     extras_require={
       # Modules
       "embeddings": ["faiss"],
```

