# Comparing `tmp/langdash-0.0.3.dev2.tar.gz` & `tmp/langdash-0.0.4.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langdash-0.0.3.dev2.tar", last modified: Wed May 31 00:51:49 2023, max compression
+gzip compressed data, was "langdash-0.0.4.dev1.tar", last modified: Wed May 31 21:24:12 2023, max compression
```

## Comparing `langdash-0.0.3.dev2.tar` & `langdash-0.0.4.dev1.tar`

### file list

```diff
@@ -1,257 +1,36 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.662254 langdash-0.0.3.dev2/
--rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-0.0.3.dev2/LICENSE.txt
--rw-rw-r--   0 user      (1000) user      (1000)     3436 2023-05-31 00:51:49.662254 langdash-0.0.3.dev2/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     2670 2023-05-30 08:29:06.000000 langdash-0.0.3.dev2/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.590252 langdash-0.0.3.dev2/langdash/
--rw-rw-r--   0 user      (1000) user      (1000)       31 2023-05-25 22:58:46.000000 langdash-0.0.3.dev2/langdash/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3596 2023-05-30 19:46:43.000000 langdash-0.0.3.dev2/langdash/_langdash.py
--rw-rw-r--   0 user      (1000) user      (1000)    16507 2023-05-30 22:12:14.000000 langdash-0.0.3.dev2/langdash/chains.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.594252 langdash-0.0.3.dev2/langdash/classify/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-0.0.3.dev2/langdash/classify/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1780 2023-05-28 17:07:24.000000 langdash-0.0.3.dev2/langdash/classify/token_qa.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.586251 langdash-0.0.3.dev2/langdash/extern/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.598252 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/
--rw-rw-r--   0 user      (1000) user      (1000)    16349 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeCache.txt
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.598252 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.602252 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/
--rw-r--r--   0 user      (1000) user      (1000)     2441 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeCCompiler.cmake
--rw-r--r--   0 user      (1000) user      (1000)     5439 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeCXXCompiler.cmake
--rwxrwxr-x   0 user      (1000) user      (1000)    15968 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeDetermineCompilerABI_C.bin
--rwxrwxr-x   0 user      (1000) user      (1000)    15992 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeDetermineCompilerABI_CXX.bin
--rw-r--r--   0 user      (1000) user      (1000)      402 2023-05-25 00:05:29.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeSystem.cmake
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.602252 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdC/
--rw-rw-r--   0 user      (1000) user      (1000)    24853 2023-05-25 00:05:29.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdC/CMakeCCompilerId.c
--rwxrwxr-x   0 user      (1000) user      (1000)    16088 2023-05-25 00:05:29.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdC/a.out
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.602252 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdCXX/
--rw-rw-r--   0 user      (1000) user      (1000)    24597 2023-05-25 00:05:29.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdCXX/CMakeCXXCompilerId.cpp
--rwxrwxr-x   0 user      (1000) user      (1000)    16096 2023-05-25 00:05:29.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdCXX/a.out
--rw-rw-r--   0 user      (1000) user      (1000)      706 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/CMakeDirectoryInformation.cmake
--rw-rw-r--   0 user      (1000) user      (1000)    50084 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/CMakeOutput.log
--rw-rw-r--   0 user      (1000) user      (1000)     7911 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/Makefile.cmake
--rw-rw-r--   0 user      (1000) user      (1000)     9844 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/Makefile2
--rw-rw-r--   0 user      (1000) user      (1000)     3155 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/TargetDirectories.txt
--rw-rw-r--   0 user      (1000) user      (1000)       85 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/cmake.check_cache
--rw-rw-r--   0 user      (1000) user      (1000)        2 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/progress.marks
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.602252 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/
--rw-rw-r--   0 user      (1000) user      (1000)      692 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/DependInfo.cmake
--rw-rw-r--   0 user      (1000) user      (1000)     4674 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/build.make
--rw-rw-r--   0 user      (1000) user      (1000)      276 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/cmake_clean.cmake
--rw-rw-r--   0 user      (1000) user      (1000)      107 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/compiler_depend.make
--rw-rw-r--   0 user      (1000) user      (1000)      111 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/compiler_depend.ts
--rw-rw-r--   0 user      (1000) user      (1000)       88 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/depend.make
--rw-rw-r--   0 user      (1000) user      (1000)      679 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/flags.make
--rw-rw-r--   0 user      (1000) user      (1000)      133 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/link.txt
--rw-rw-r--   0 user      (1000) user      (1000)       43 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/progress.make
--rw-rw-r--   0 user      (1000) user      (1000)   101576 2023-05-25 00:05:37.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/rwkv.cpp.o
--rw-rw-r--   0 user      (1000) user      (1000)    11910 2023-05-25 00:05:37.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/rwkv.cpp.o.d
--rw-rw-r--   0 user      (1000) user      (1000)     6908 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)      376 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/CTestTestfile.cmake
--rw-rw-r--   0 user      (1000) user      (1000)     1338 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/FILE_FORMAT.md
--rw-rw-r--   0 user      (1000) user      (1000)     1067 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)     8978 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/Makefile
--rw-rw-r--   0 user      (1000) user      (1000)     6412 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.606252 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)   165600 2023-05-25 00:05:38.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/bin/test_ggml_basics
--rwxrwxr-x   0 user      (1000) user      (1000)    16728 2023-05-25 00:05:38.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/bin/test_tiny_rwkv
--rw-rw-r--   0 user      (1000) user      (1000)     2013 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/cmake_install.cmake
--rw-rw-r--   0 user      (1000) user      (1000)     3799 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/compile_commands.json
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.606252 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.606252 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/CMakeFiles/
--rw-rw-r--   0 user      (1000) user      (1000)      706 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/CMakeFiles/CMakeDirectoryInformation.cmake
--rw-rw-r--   0 user      (1000) user      (1000)        2 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/CMakeFiles/progress.marks
--rw-rw-r--   0 user      (1000) user      (1000)     2552 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)     1072 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)     7013 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/Makefile
--rw-rw-r--   0 user      (1000) user      (1000)     3707 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.606252 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/cmake/
--rw-rw-r--   0 user      (1000) user      (1000)     2037 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/cmake/BuildTypes.cmake
--rw-rw-r--   0 user      (1000) user      (1000)      717 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/cmake/GitVars.cmake
--rw-rw-r--   0 user      (1000) user      (1000)     1496 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/cmake_install.cmake
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.606252 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/
--rw-rw-r--   0 user      (1000) user      (1000)      433 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)     8583 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/common-ggml.cpp
--rw-rw-r--   0 user      (1000) user      (1000)      410 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/common-ggml.h
--rw-rw-r--   0 user      (1000) user      (1000)    15664 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/common.cpp
--rw-rw-r--   0 user      (1000) user      (1000)     3311 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/common.h
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.610252 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/
--rw-rw-r--   0 user      (1000) user      (1000)      319 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)     6201 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/README.md
--rw-rw-r--   0 user      (1000) user      (1000)     3490 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/convert-h5-to-ggml.py
--rw-rw-r--   0 user      (1000) user      (1000)    28339 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/main.cpp
--rw-rw-r--   0 user      (1000) user      (1000)     5200 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/quantize.cpp
--rw-rw-r--   0 user      (1000) user      (1000)   241358 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/dr_wav.h
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.610252 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/
--rw-rw-r--   0 user      (1000) user      (1000)      311 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)     6370 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/README.md
--rw-rw-r--   0 user      (1000) user      (1000)     6313 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/convert-cerebras-to-ggml.py
--rw-rw-r--   0 user      (1000) user      (1000)     4873 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/convert-ckpt-to-ggml.py
--rw-rw-r--   0 user      (1000) user      (1000)     6436 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/convert-h5-to-ggml.py
--rwxrwxr-x   0 user      (1000) user      (1000)     1752 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/download-ggml-model.sh
--rwxrwxr-x   0 user      (1000) user      (1000)     1117 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/download-model.sh
--rw-rw-r--   0 user      (1000) user      (1000)    29187 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/main.cpp
--rw-rw-r--   0 user      (1000) user      (1000)     5467 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/quantize.cpp
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.614252 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/
--rw-rw-r--   0 user      (1000) user      (1000)      311 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)    11108 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/README.md
--rw-rw-r--   0 user      (1000) user      (1000)     5509 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/convert-h5-to-ggml.py
--rwxrwxr-x   0 user      (1000) user      (1000)     1728 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/download-ggml-model.sh
--rwxrwxr-x   0 user      (1000) user      (1000)      571 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/download-model.sh
--rw-rw-r--   0 user      (1000) user      (1000)    25782 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/main.cpp
--rw-rw-r--   0 user      (1000) user      (1000)     5469 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/quantize.cpp
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.614252 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/
--rw-rw-r--   0 user      (1000) user      (1000)      133 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)     3689 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/README.md
--rw-rw-r--   0 user      (1000) user      (1000)     1491 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/convert-h5-to-ggml.py
--rw-rw-r--   0 user      (1000) user      (1000)     7679 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/main.cpp
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.586251 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/models/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.618252 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/models/mnist/
--rw-rw-r--   0 user      (1000) user      (1000)  1591571 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/models/mnist/mnist_model.state_dict
--rw-rw-r--   0 user      (1000) user      (1000)  7840016 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/models/mnist/t10k-images.idx3-ubyte
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.626253 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/stablelm/
--rw-rw-r--   0 user      (1000) user      (1000)      323 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/stablelm/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)     4755 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/stablelm/README.md
--rw-rw-r--   0 user      (1000) user      (1000)     3490 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/stablelm/convert-h5-to-ggml.py
--rw-rw-r--   0 user      (1000) user      (1000)    27316 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/stablelm/main.cpp
--rw-rw-r--   0 user      (1000) user      (1000)     5200 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/stablelm/quantize.cpp
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.630253 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/
--rw-rw-r--   0 user      (1000) user      (1000)      501 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)      718 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/README.md
--rw-rw-r--   0 user      (1000) user      (1000)     9506 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/convert-pt-to-ggml.py
--rw-rw-r--   0 user      (1000) user      (1000)    36271 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/main.cpp
--rw-rw-r--   0 user      (1000) user      (1000)     7693 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/quantize.cpp
--rw-rw-r--   0 user      (1000) user      (1000)   184690 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/whisper.cpp
--rw-rw-r--   0 user      (1000) user      (1000)    23750 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/whisper.h
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.586251 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/include/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.630253 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/include/ggml/
--rw-rw-r--   0 user      (1000) user      (1000)    31202 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/include/ggml/ggml.h
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.630253 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/scripts/
--rwxrwxr-x   0 user      (1000) user      (1000)      323 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/scripts/sync-llama.sh
--rwxrwxr-x   0 user      (1000) user      (1000)      921 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/scripts/sync-whisper.sh
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.630253 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.634253 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/
--rw-rw-r--   0 user      (1000) user      (1000)      706 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/CMakeDirectoryInformation.cmake
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.634253 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/
--rw-rw-r--   0 user      (1000) user      (1000)      597 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/DependInfo.cmake
--rw-rw-r--   0 user      (1000) user      (1000)     5420 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/build.make
--rw-rw-r--   0 user      (1000) user      (1000)      269 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/cmake_clean.cmake
--rw-rw-r--   0 user      (1000) user      (1000)       36 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/cmake_clean_target.cmake
--rw-rw-r--   0 user      (1000) user      (1000)      107 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/compiler_depend.make
--rw-rw-r--   0 user      (1000) user      (1000)      111 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/compiler_depend.ts
--rw-rw-r--   0 user      (1000) user      (1000)       88 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/depend.make
--rw-rw-r--   0 user      (1000) user      (1000)     1057 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/flags.make
--rw-rw-r--   0 user      (1000) user      (1000)   201672 2023-05-25 00:05:35.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/ggml.c.o
--rw-rw-r--   0 user      (1000) user      (1000)    10631 2023-05-25 00:05:35.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/ggml.c.o.d
--rw-rw-r--   0 user      (1000) user      (1000)       80 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/link.txt
--rw-rw-r--   0 user      (1000) user      (1000)       43 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/progress.make
--rw-rw-r--   0 user      (1000) user      (1000)        2 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/progress.marks
--rw-rw-r--   0 user      (1000) user      (1000)     8040 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)     8522 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/Makefile
--rw-rw-r--   0 user      (1000) user      (1000)     1573 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/cmake_install.cmake
--rw-rw-r--   0 user      (1000) user      (1000)    24594 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/ggml-cuda.cu
--rw-rw-r--   0 user      (1000) user      (1000)      638 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/ggml-cuda.h
--rw-rw-r--   0 user      (1000) user      (1000)    13447 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/ggml-opencl.c
--rw-rw-r--   0 user      (1000) user      (1000)      639 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/ggml-opencl.h
--rw-rw-r--   0 user      (1000) user      (1000)   428283 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/ggml.c
--rw-rw-r--   0 user      (1000) user      (1000)   205118 2023-05-25 00:05:35.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/src/libggml.a
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.638253 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/
--rw-rw-r--   0 user      (1000) user      (1000)     9198 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)     6569 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-blas0.c
--rw-rw-r--   0 user      (1000) user      (1000)    11463 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-grad0.c
--rw-rw-r--   0 user      (1000) user      (1000)    10265 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-mul-mat0.c
--rw-rw-r--   0 user      (1000) user      (1000)     9003 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-mul-mat1.c
--rw-rw-r--   0 user      (1000) user      (1000)    91837 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-mul-mat2.c
--rw-rw-r--   0 user      (1000) user      (1000)     5141 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-svd0.c
--rw-rw-r--   0 user      (1000) user      (1000)     3157 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-vec0.c
--rw-rw-r--   0 user      (1000) user      (1000)    21179 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-vec1.c
--rw-rw-r--   0 user      (1000) user      (1000)     7310 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-vec2.c
--rw-rw-r--   0 user      (1000) user      (1000)     1182 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/test0.c
--rw-rw-r--   0 user      (1000) user      (1000)    15073 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/test1.c
--rw-rw-r--   0 user      (1000) user      (1000)     5703 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/test2.c
--rw-rw-r--   0 user      (1000) user      (1000)     2841 2023-05-25 00:05:22.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/ggml/tests/test3.c
--rwxrwxr-x   0 user      (1000) user      (1000)   243024 2023-05-25 00:05:38.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/librwkv.so
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.646253 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/
--rw-rw-r--   0 user      (1000) user      (1000)  2467981 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/20B_tokenizer.json
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.646253 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/__pycache__/
--rw-rw-r--   0 user      (1000) user      (1000)     4174 2023-05-25 00:05:38.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/__pycache__/rwkv_cpp_model.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)     6921 2023-05-25 00:05:39.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/__pycache__/rwkv_cpp_shared_library.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)     8813 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/chat_with_bot.py
--rw-rw-r--   0 user      (1000) user      (1000)     3320 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/convert_pytorch_to_ggml.py
--rw-rw-r--   0 user      (1000) user      (1000)     1463 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/convert_pytorch_to_ggml.test.py
--rw-rw-r--   0 user      (1000) user      (1000)     2380 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/generate_completions.py
--rw-rw-r--   0 user      (1000) user      (1000)     3886 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/measure_pexplexity.py
--rw-rw-r--   0 user      (1000) user      (1000)     5833 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/merge_lora_into_ggml.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.646253 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/
--rw-rw-r--   0 user      (1000) user      (1000)      947 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/Chinese-Chat.json
--rw-rw-r--   0 user      (1000) user      (1000)      139 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/Chinese-QA.json
--rw-rw-r--   0 user      (1000) user      (1000)     1095 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/English-Chat.json
--rw-rw-r--   0 user      (1000) user      (1000)      764 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/English-QA.json
--rw-rw-r--   0 user      (1000) user      (1000)     1433 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/Japanese-Chat.json
--rw-rw-r--   0 user      (1000) user      (1000)      979 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/Japanese-QA.json
--rw-rw-r--   0 user      (1000) user      (1000)     1106 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/quantize.py
--rw-rw-r--   0 user      (1000) user      (1000)       23 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/requirements.txt
--rw-rw-r--   0 user      (1000) user      (1000)     4359 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/rwkv_cpp_model.py
--rw-rw-r--   0 user      (1000) user      (1000)     7528 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/rwkv_cpp_shared_library.py
--rw-rw-r--   0 user      (1000) user      (1000)     1255 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv/sampling.py
--rw-rw-r--   0 user      (1000) user      (1000)    39641 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv.cpp
--rw-rw-r--   0 user      (1000) user      (1000)     4691 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/rwkv.h
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.650254 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.654254 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/
--rw-rw-r--   0 user      (1000) user      (1000)      706 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/CMakeDirectoryInformation.cmake
--rw-rw-r--   0 user      (1000) user      (1000)        2 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/progress.marks
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.658254 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/
--rw-rw-r--   0 user      (1000) user      (1000)      871 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/DependInfo.cmake
--rw-rw-r--   0 user      (1000) user      (1000)     5923 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/build.make
--rw-rw-r--   0 user      (1000) user      (1000)      359 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/cmake_clean.cmake
--rw-rw-r--   0 user      (1000) user      (1000)      119 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/compiler_depend.make
--rw-rw-r--   0 user      (1000) user      (1000)      123 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/compiler_depend.ts
--rw-rw-r--   0 user      (1000) user      (1000)      100 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/depend.make
--rw-rw-r--   0 user      (1000) user      (1000)      670 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/flags.make
--rw-rw-r--   0 user      (1000) user      (1000)      224 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/link.txt
--rw-rw-r--   0 user      (1000) user      (1000)       43 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/progress.make
--rw-rw-r--   0 user      (1000) user      (1000)     5152 2023-05-25 00:05:38.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/test_ggml_basics.c.o
--rw-rw-r--   0 user      (1000) user      (1000)     3717 2023-05-25 00:05:38.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/test_ggml_basics.c.o.d
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.662254 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/
--rw-rw-r--   0 user      (1000) user      (1000)      861 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/DependInfo.cmake
--rw-rw-r--   0 user      (1000) user      (1000)     5799 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/build.make
--rw-rw-r--   0 user      (1000) user      (1000)      345 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/cmake_clean.cmake
--rw-rw-r--   0 user      (1000) user      (1000)      117 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/compiler_depend.make
--rw-rw-r--   0 user      (1000) user      (1000)      121 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/compiler_depend.ts
--rw-rw-r--   0 user      (1000) user      (1000)       98 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/depend.make
--rw-rw-r--   0 user      (1000) user      (1000)      670 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/flags.make
--rw-rw-r--   0 user      (1000) user      (1000)      218 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/link.txt
--rw-rw-r--   0 user      (1000) user      (1000)       43 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/progress.make
--rw-rw-r--   0 user      (1000) user      (1000)     9816 2023-05-25 00:05:38.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/test_tiny_rwkv.c.o
--rw-rw-r--   0 user      (1000) user      (1000)     4064 2023-05-25 00:05:38.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/test_tiny_rwkv.c.o.d
--rw-rw-r--   0 user      (1000) user      (1000)      577 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)     1309 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/CTestTestfile.cmake
--rw-rw-r--   0 user      (1000) user      (1000)    10760 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/Makefile
--rw-rw-r--   0 user      (1000) user      (1000)     1292 2023-05-25 00:05:30.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/cmake_install.cmake
--rw-rw-r--   0 user      (1000) user      (1000)     1024 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/expected_logits.bin
--rw-rw-r--   0 user      (1000) user      (1000)     1724 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/test_ggml_basics.c
--rw-rw-r--   0 user      (1000) user      (1000)     5039 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/test_tiny_rwkv.c
--rw-rw-r--   0 user      (1000) user      (1000)  1338429 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/tiny-rwkv-660K-FP16.bin
--rw-rw-r--   0 user      (1000) user      (1000)  2649149 2023-05-25 00:04:50.000000 langdash-0.0.3.dev2/langdash/extern/rwkv.cpp/tests/tiny-rwkv-660K-FP32.bin
--rw-rw-r--   0 user      (1000) user      (1000)      217 2023-05-30 08:12:32.000000 langdash-0.0.3.dev2/langdash/infer.py
--rw-rw-r--   0 user      (1000) user      (1000)     1209 2023-05-30 19:56:33.000000 langdash-0.0.3.dev2/langdash/llm.py
--rw-rw-r--   0 user      (1000) user      (1000)     7101 2023-05-30 20:56:47.000000 langdash-0.0.3.dev2/langdash/llm_session.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.594252 langdash-0.0.3.dev2/langdash/models/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:36.000000 langdash-0.0.3.dev2/langdash/models/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      624 2023-05-25 22:58:44.000000 langdash-0.0.3.dev2/langdash/models/mock.py
--rw-rw-r--   0 user      (1000) user      (1000)     6964 2023-05-30 22:08:25.000000 langdash-0.0.3.dev2/langdash/models/rwkvcpp.py
--rw-rw-r--   0 user      (1000) user      (1000)      840 2023-05-29 18:14:56.000000 langdash-0.0.3.dev2/langdash/models/sentence_transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     6051 2023-05-30 22:02:01.000000 langdash-0.0.3.dev2/langdash/models/transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)      259 2023-05-25 22:58:46.000000 langdash-0.0.3.dev2/langdash/response.py
--rw-rw-r--   0 user      (1000) user      (1000)     2154 2023-05-30 19:25:05.000000 langdash-0.0.3.dev2/langdash/sampling.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.594252 langdash-0.0.3.dev2/langdash/search/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-0.0.3.dev2/langdash/search/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      840 2023-05-29 19:25:03.000000 langdash-0.0.3.dev2/langdash/search/embedding_search.py
--rw-rw-r--   0 user      (1000) user      (1000)      260 2023-05-27 05:17:38.000000 langdash-0.0.3.dev2/langdash/search/engine.py
--rw-rw-r--   0 user      (1000) user      (1000)     2391 2023-05-28 22:28:07.000000 langdash-0.0.3.dev2/langdash/search/multichoice_search.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:51:49.594252 langdash-0.0.3.dev2/langdash.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     3436 2023-05-31 00:51:49.000000 langdash-0.0.3.dev2/langdash.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    12207 2023-05-31 00:51:49.000000 langdash-0.0.3.dev2/langdash.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-31 00:51:49.000000 langdash-0.0.3.dev2/langdash.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      124 2023-05-31 00:51:49.000000 langdash-0.0.3.dev2/langdash.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        9 2023-05-31 00:51:49.000000 langdash-0.0.3.dev2/langdash.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-05-31 00:51:49.662254 langdash-0.0.3.dev2/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1282 2023-05-31 00:50:47.000000 langdash-0.0.3.dev2/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 21:24:12.502655 langdash-0.0.4.dev1/
+-rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-0.0.4.dev1/LICENSE.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       35 2023-05-31 17:16:19.000000 langdash-0.0.4.dev1/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)     3484 2023-05-31 21:24:12.502655 langdash-0.0.4.dev1/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     2670 2023-05-30 08:29:06.000000 langdash-0.0.4.dev1/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 21:24:12.502655 langdash-0.0.4.dev1/langdash/
+-rw-rw-r--   0 user      (1000) user      (1000)       66 2023-05-31 20:08:48.000000 langdash-0.0.4.dev1/langdash/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    17611 2023-05-31 19:50:04.000000 langdash-0.0.4.dev1/langdash/chains.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 21:24:12.498655 langdash-0.0.4.dev1/langdash/classify/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-0.0.4.dev1/langdash/classify/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1780 2023-05-28 17:07:24.000000 langdash-0.0.4.dev1/langdash/classify/token_qa.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4126 2023-05-31 20:08:59.000000 langdash-0.0.4.dev1/langdash/core.py
+-rw-rw-r--   0 user      (1000) user      (1000)      690 2023-05-31 17:39:51.000000 langdash-0.0.4.dev1/langdash/infer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1223 2023-05-31 17:04:37.000000 langdash-0.0.4.dev1/langdash/llm.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7520 2023-05-31 19:52:12.000000 langdash-0.0.4.dev1/langdash/llm_session.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 21:24:12.498655 langdash-0.0.4.dev1/langdash/models/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:36.000000 langdash-0.0.4.dev1/langdash/models/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      682 2023-05-31 21:23:49.000000 langdash-0.0.4.dev1/langdash/models/mock.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7041 2023-05-31 20:11:04.000000 langdash-0.0.4.dev1/langdash/models/rwkvcpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)      958 2023-05-31 20:11:54.000000 langdash-0.0.4.dev1/langdash/models/sentence_transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6134 2023-05-31 20:11:31.000000 langdash-0.0.4.dev1/langdash/models/transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)      835 2023-05-31 17:40:54.000000 langdash-0.0.4.dev1/langdash/response.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2436 2023-05-31 17:34:53.000000 langdash-0.0.4.dev1/langdash/sampling.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 21:24:12.502655 langdash-0.0.4.dev1/langdash/search/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-0.0.4.dev1/langdash/search/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      840 2023-05-29 19:25:03.000000 langdash-0.0.4.dev1/langdash/search/embedding_search.py
+-rw-rw-r--   0 user      (1000) user      (1000)      260 2023-05-27 05:17:38.000000 langdash-0.0.4.dev1/langdash/search/engine.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2391 2023-05-28 22:28:07.000000 langdash-0.0.4.dev1/langdash/search/multichoice_search.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 21:24:12.502655 langdash-0.0.4.dev1/langdash.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     3484 2023-05-31 21:24:12.000000 langdash-0.0.4.dev1/langdash.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1214 2023-05-31 21:24:12.000000 langdash-0.0.4.dev1/langdash.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-31 21:24:12.000000 langdash-0.0.4.dev1/langdash.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      124 2023-05-31 21:24:12.000000 langdash-0.0.4.dev1/langdash.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        9 2023-05-31 21:24:12.000000 langdash-0.0.4.dev1/langdash.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-05-31 21:24:12.502655 langdash-0.0.4.dev1/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1405 2023-05-31 20:04:55.000000 langdash-0.0.4.dev1/setup.py
```

### Comparing `langdash-0.0.3.dev2/LICENSE.txt` & `langdash-0.0.4.dev1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev2/PKG-INFO` & `langdash-0.0.4.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 0.0.3.dev2
+Version: 0.0.4.dev1
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: embeddings
 Provides-Extra: rwkvcpp
 Provides-Extra: transformers
 Provides-Extra: sentence_transformers
```

### Comparing `langdash-0.0.3.dev2/README.md` & `langdash-0.0.4.dev1/README.md`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev2/langdash/_langdash.py` & `langdash-0.0.4.dev1/langdash/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 from langdash.llm import LLM
 from langdash.llm_session import LLMSession, T_LLM
 from langdash.chains import LDChain, LDText, LDFormatArg, LDArg, LDReturns, LDChoice
 
 T_ModelInternal = TypeVar("T_ModelInternal")
 
 class Langdash:
+  """
+  Core Langdash instance.
+  """
   _models: Dict[str, LLM]
   
   def __init__(self):
     self._models = {}
     self._cached_models = {}
   
   def get_model_internal(self,
@@ -23,44 +26,51 @@
     return self._cached_models[model]
   
   def register_model(self, name: str, model: LLM):
     """
     Register a new language model to the Langdash instance.
     
     Args:
-      name: The name of the model.
-      model: The LLM object.
+      name (str): The name of the model.
+      model (LLM): The LLM object.
     """
     if name in self._models:
       raise KeyError(f"model '{name}' already exists")
     self._models[name] = model
     
   def session_for_model(self, model: str, **kwargs) -> LLMSession:
     """
     Create a new session for a given model.
     
     Args:
-      model: The name of the model to be used.
+      model (str): The name of the model to be used.
+      default_infer_args (InferArgs): Default inference arguments.
+      track_called_chains (bool): Whether or not to track the nodes called in each chain. Defaults to `True`.
+      token_healing (bool): Whether or not to heal tokens.
+      global_args (LDNodeArgs): Global arguments which can be read by every chain.
     
     Returns:
-      The session object.
+      (LLMSession) The session object.
     """
     return self._models[model].session(ld=self, **kwargs)
       
   def chain(self, *args, **kwargs) -> LDChain:
     """
     Chain a list of nodes together.
 
     Args:
-      nodes: A list of nodes to chain.
-      args: A dictionary of argument types for the chain function.
-      returns: A dictionary of return value types for the chain function.
+      nodes (List[Union["LDNode", str]]):
+        A list of nodes or constant text nodes (represented by strings) to chain together.
+      args (TypeDict):
+        A dictionary of argument types for the chain function.
+      returns (TypeDict):
+        A dictionary of return value types for the chain function.
 
     Returns:
-      The chain of nodes.
+      (LDChain) The chain of nodes.
     """
     return LDChain(self, *args, **kwargs)
     
   def text(self, *args, **kwargs):
     """
     Creates a raw text node.
```

### Comparing `langdash-0.0.3.dev2/langdash/chains.py` & `langdash-0.0.4.dev1/langdash/chains.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,20 +18,28 @@
 LDNodeGenerator = Generator[Response, None, None]
 LDNodeArgs = Dict[str, Any]
 LDNodeArgsFrozen = FrozenSet[Tuple[str, Any]]
 TypeDict = Dict[str, Type]
 
 @dataclass(frozen=True)
 class CalledChain:
+  """
+  Data class used to store info about nodes previously called.
+  
+  Attributes:
+    node: Node object
+    args: Arguments passed to the node (for LDFormatArg)
+    tokens_used: Number of tokens the node used (either number of tokens injected, or generated)
+  """
   node: "LDNode"
   args: LDNodeArgs
   tokens_used: int
 
 class LDChain:
-  
+  """ Class used to represent language chains """
   def __init__(
     self,
     ld: "Langdash",
     nodes: List[Union["LDNode", str]],
     args: TypeDict = {},
     returns: TypeDict = {},
   ):
@@ -42,15 +50,15 @@
     self._nodes = self._preprocess_nodes(nodes)
   
   def cached(self, model: str, **model_kwargs) -> "LDChainCached":
     """
     Cache the chain for a specific model
     
     Args:
-      model: The model name
+      model (str): The model name
       
     Returns:
       The cached chain
     """
     return LDChainCached(
       model=model,
       model_kwargs=model_kwargs,
@@ -129,27 +137,31 @@
   def _load_session(self, ctx: Union[str, "LLMGenerationSession"]) -> "LLMGenerationSession":
     from langdash.llm_session import LLMGenerationSession
     if isinstance(ctx, LLMGenerationSession):
       return ctx
     else:
       return self._ld.session_for_model(ctx)
   
-  def _stream(self, session: "LLMGenerationSession", args: LDNodeArgs):
+  def _stream(self, session: "LLMGenerationSession", args: LDNodeArgs) \
+    -> Generator[Response, None, None]:
     for node in self._node_pass(session, args):
       if isinstance(node, Union[LDReturns, LDChoice]):
         yield RespReturns(key=node._returns)
       yield from node(session, args)
   
-  def stream(self, ctx: Union[str, "LLMGenerationSession"], **kwargs):
+  def stream(self, ctx: Union[str, "LLMGenerationSession"], **kwargs) \
+    -> Generator[Response, None, None]:
     """
     Stream data generated from the LLM within the specified session.
     
     Args:
-        session: The LLM generation session.
-        args: The arguments to pass to generation.
+      session (Union[str, "LLMGenerationSession"]):
+        The name of the model, or an existing LLM generation session.
+      args (LDNodeArgs):
+        Arguments to pass to the chain. This will be used by any argument or format nodes.
     """
     return self._stream(session=self._load_session(ctx), **kwargs)
   
   def _call(
     self,
     session: "LLMGenerationSession",
     args: LDNodeArgs = {},
@@ -171,25 +183,25 @@
     return result
   
   def call(self, ctx: Union[str, "LLMGenerationSession"], **kwargs):
     """
     Returns data generated from the LLM within the specified session.
     
     Args:
-      ctx:
-        The LLM generation session, or the model name.
-      args:
-        The arguments to pass to generation.
-      return_session:
+      ctx (Union[str, "LLMGenerationSession"]):
+        The name of the model, or an existing LLM generation session.
+      args (LDNodeArgs):
+        Arguments to pass to the chain. This will be used by any argument or format nodes.
+      return_session (bool):
         Whether or not to return the generation session after generation.
-      set_global_args:
+      set_global_args (bool):
         Whether or not to set current arguments as global arguments.
     
     Returns:
-      The result, or a tuple with (result, session).
+      (LDResult) The result, or a tuple with (result, session).
     """
     return self._call(session=self._load_session(ctx), **kwargs)
 
 @dataclass
 class LDChainCacheState:
   state: "LLMState"
   skip_nodes: int
@@ -328,32 +340,38 @@
   def call(self, **kwargs):
     return super()._call(session=self._load_session(args=kwargs.get("args")), **kwargs)
 
 @dataclass
 class LDResult:
   """
   Class for storing the results of inference.
+  
+  Attributes:
+    returns: Mapping of return keys to return values
+    prompt_tokens: Number of tokens injected to the language model
+    completion_tokens: Number of tokens generated by the language model
   """
+  
   returns: Dict[str, Any]
   prompt_tokens: int
   completion_tokens: int
   
   def __init__(self):
     self.returns = {}
     self.prompt_tokens = 0
     self.completion_tokens = 0
     
   def update_results(self, key: str, cast_function, generator: LDNodeGenerator):
     """
     Update the results with the given key.
     
     Args:
-      key: The key of the language model.
+      key (str): The key of the language model.
       cast_function: The function to cast the results.
-      generator: Node generator that runs to get the results.
+      generator (LDNodeGenerator): Node generator that runs to get the results.
     """
     text = ""
     for resp in generator:
       if isinstance(resp, RespInfer):
         text = resp.running_infer
         self.completion_tokens += 1
       else:
@@ -361,56 +379,60 @@
     self.returns[key] = cast_function(text)
   
   def update_stats(self, generator: LDNodeGenerator):
     """
     Update the stats of the result, given a node generator.
     
     Args:
-      generator: Node generator to get the results.
+      generator (LDNodeGenerator): Node generator to get the results.
     """
     for resp in generator:
       if isinstance(resp, RespInject):
         self.prompt_tokens += resp.tokens_counter
       else:
         continue
 
 class LDNode:
+  """ Base class for langdash nodes. """
   def __init__(self, ld: "Langdash"):
     self._ld = ld
     
   def __call__(self, session: "LLMGenerationSession", args: LDNodeArgs) -> LDNodeGenerator:
     raise NotImplementedError("__call__")
   
 class LDText(LDNode):
+  """ Constant text node """
   
   def __init__(self, ld: "Langdash", text: str):
     super().__init__(ld)
     self._text = text
     
   def __repr__(self):
     return f"<Text>\n{self._text}\n</Text>"
   
   def __call__(self, session: "LLMGenerationSession", args: LDNodeArgs) -> LDNodeGenerator:
     tokens_counter = session.inject(self._text)
     yield RespInject(tokens_counter=tokens_counter)
   
 class LDFormatArg(LDNode):
+  """ Format argument node """
   
   def __init__(self, ld: "Langdash", text: str):
     super().__init__(ld)
     self._text = text
   
   def __repr__(self):
     return f"<FormatArgs>\n{self._text}\n</FormatArgs>"
   
   def __call__(self, session: "LLMGenerationSession", args: LDNodeArgs) -> LDNodeGenerator:
     tokens_counter = session.inject(self._text.format(globals=session.global_args, **args))
     yield RespInject(tokens_counter=tokens_counter)
 
 class LDArg(LDNode):
+  """ Argument node """
   
   def __init__(self, ld: "Langdash",
                arg: str,
                padleft: str = "",
                padright: str = ""):
     super().__init__(ld)
     self._arg = arg
@@ -428,14 +450,15 @@
     else:
       s += str(session.global_args[self._arg])
     s += self._padright
     tokens_counter = session.inject(s)
     yield RespInject(tokens_counter=tokens_counter)
   
 class LDReturns(LDNode):
+  """ Return node """
   
   def __init__(self, ld: "Langdash",
                returns: str,
                end: Optional[Union[str, int]],
                padleft: Optional[str] = None,
                inference_args: Optional[InferArgs] = None):
     super().__init__(ld)
@@ -451,14 +474,15 @@
     for i, respinfer in enumerate(session.infer(end=self._end, args=self._inference_args)):
       if i == 0:
         if self._padleft is not None and respinfer.tokstr.startswith(self._padleft):
           respinfer.tokstr = respinfer.tokstr[len(self._padleft):]
       yield respinfer
       
 class LDChoice(LDNode):
+  """ Choice node """
   
   def __init__(self, ld: "Langdash",
                returns: str,
                choices: List[str],
                padleft: str = "",
                padright: str = ""):
     super().__init__(ld)
```

### Comparing `langdash-0.0.3.dev2/langdash/classify/token_qa.py` & `langdash-0.0.4.dev1/langdash/classify/token_qa.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev2/langdash/llm.py` & `langdash-0.0.4.dev1/langdash/llm.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,13 +37,13 @@
 
   def get_capability(self) -> LLMCapability:
     """
     Returns the capability of the language model.
     """
     return LLMCapability.Generative
 
-class EmbeddingLLM(LLM):
+class EmbeddingLLM(LLM[T_LLMSession]):
   """
   A language model class for generating embeddings.
   """
   def get_capability(self) -> LLMCapability:
     return LLMCapability.Embedding
```

### Comparing `langdash-0.0.3.dev2/langdash/llm_session.py` & `langdash-0.0.4.dev1/langdash/llm_session.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,14 +23,16 @@
   """
   pass
 
 T_LLM = TypeVar('T_LLM', bound=LLM)
 T_LLMState = TypeVar("T_LLMState", bound=LLMState)
 
 class LLMGenerationSession(LLMSession, Generic[T_LLM, T_LLMState]):
+  """ Generation session for a language model. """
+  
   def __init__(self,
                llm: T_LLM,
                ld: "Langdash",
                default_infer_args: InferArgs = InferArgs(),
                track_called_chains: bool = True,
                token_healing: bool = True,
                global_args: LDNodeArgs = {}):
@@ -45,15 +47,15 @@
     self.tokens_counter = 0
     
   def set_state(self, state: Optional[T_LLMState]):
     """
     Set the state of the language model.
 
     Args:
-      state:
+      state (Optional[T_LLMState]):
         The state of the language model, or None to clear the state.
     """
     raise NotImplementedError("set_state")
   
   def clone_state(self) -> T_LLMState:
     """
     Clone the current state of the language model.
@@ -86,19 +88,19 @@
       self.called_chains.append(CalledChain(node=node, args=args, tokens_used=tokens_used))
   
   def tokenize(self, text: str, add_special_tokens: bool = False) -> List[int]:
     """
     Tokenize the given text into a list of tokens.
 
     Args:
-      text: The text to tokenize.
-      add_special_tokens: Whether to add special tokens to the output.
+      text (str): The text to tokenize.
+      add_special_tokens (bool): Whether to add special tokens to the output.
 
     Returns:
-      The list of tokens.
+      (List[int]) The list of tokens.
     """
     raise NotImplementedError("tokenize")
   
   def decode(self, tokids: List[int]) -> str:
     raise NotImplementedError("decode")
   
   def next_token_probs(self) -> List[float]:
@@ -115,30 +117,35 @@
   def infer(self,
             end: Optional[Union[str, int]],
             args: Optional[InferArgs] = None) -> Generator[RespInfer, None, None]:
     """
     Infer the next token from the input sequence.
 
     Args:
-      end: The end of the input sequence.
-      args: Additional arguments to pass to the inference function.
+      end (Optional[Union[str, int]]):
+        The end of the output sequence.
+        If set to None, the output sequence will be generated until the maximum number of tokens is reached.
+      args (Optional[InferArgs]):
+        Optionak inference parameters.
         
     Returns:
       Inference response
     """
     if not args:
       args = self.default_infer_args
     yield from self._infer(end, args)
     
   def inject(self, text: Union[str, int], add_special_tokens: bool = False) -> int:
     raise NotImplementedError("inject")
 
 T_Logits = TypeVar('T_Logits')
 
 class LLMGenerationSessionForRawText(LLMGenerationSession, Generic[T_LLM, T_LLMState, T_Logits]):
+  """ Generation session for a language model that processes raw text. """
+  
   _logits: Optional[T_Logits]
   _next_token: Optional[Tuple[int, str]]
   
   def _eval(self, tokid: int) -> T_Logits:
     raise NotImplementedError("_eval")
   
   def _next_token_probs(self):
@@ -207,14 +214,16 @@
       num_toks += len(input_ids)
 
     return num_toks
 
 T_Embedding = TypeVar('T_Embedding')
 
 class LLMEmbeddingSession(LLMSession, Generic[T_LLM, T_Embedding]):
+  """ Session for a language model that outputs an embedding for raw text. """
+  
   def __init__(self,
                llm: T_LLM,
                ld: "Langdash"):
     self._ld = ld
     self.llm = llm
     
   def embedding_size(self) -> int:
@@ -224,13 +233,13 @@
     raise NotImplementedError("embedding_size")
     
   def infer(self, text: str) -> T_Embedding:
     """
     Infer the embedding of a text.
     
     Args:
-      text: The text to be embedded.
+      text (str): The text to be embedded.
       
     Returns:
       The embedding vector of the text.
     """
     raise NotImplementedError("infer")
```

### Comparing `langdash-0.0.3.dev2/langdash/models/rwkvcpp.py` & `langdash-0.0.4.dev1/langdash/models/rwkvcpp.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,18 @@
 @dataclass
 class RWKVCppState(LLMState):
   _logits: Optional[torch.Tensor] = None
   _state: Optional[torch.Tensor] = None
   _next_token: Optional[Tuple[int, str]] = None
 
 class RWKVCppSession(LLMGenerationSessionForRawText["RWKVCppModel", RWKVCppState, torch.Tensor]):
+  """
+  Session for rwkv.cpp model.
+  """
+  
   _rwkv: rwkv_cpp_model.RWKVModel
   _tokenizer: tokenizers.Tokenizer
   
   def __init__(self, *args, **kwargs):
     super().__init__(*args, **kwargs)
     
     def load_model(llm: RWKVCppModel):
@@ -196,14 +200,18 @@
         yield RespInfer(tokid=tokid, tokstr=tokstr, running_infer=generated)
         
       self._logits, self._state = self._rwkv.eval(tokid, self._state)
     
     yield RespInfer(tokid=0, tokstr="", running_infer=generated)
 
 class RWKVCppModel(LLM[RWKVCppSession]):
+  """
+  rwkv.cpp model
+  """
+  
   Session = RWKVCppSession
   
   def __init__(self, model_path: str, tokenizer_path: Optional[str] = None):
     """
     Creates a template for the RWKV language model (using the rwkv.cpp library).
     
     Args:
```

### Comparing `langdash-0.0.3.dev2/langdash/models/sentence_transformers.py` & `langdash-0.0.4.dev1/langdash/models/sentence_transformers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from sentence_transformers import SentenceTransformer
 import torch
 from langdash.llm import EmbeddingLLM
 from langdash.llm_session import LLMEmbeddingSession
 
 class SentenceTransformersSession(LLMEmbeddingSession["SentenceTransformersModel", torch.Tensor]):
+  """
+  Session for sentence_transformers embedding model.
+  """
   def __init__(self, *args, **kwargs):
     super().__init__(*args, **kwargs)
       
     self._model = self._ld.get_model_internal(
       self.llm,
       lambda llm: SentenceTransformer(llm._model_name)
     )
@@ -15,11 +18,14 @@
   def embedding_size(self) -> int:
     return self._model.get_sentence_embedding_dimension()
   
   def infer(self, text: str) -> torch.Tensor:
     return self._model.encode([text])
 
 class SentenceTransformersModel(EmbeddingLLM[SentenceTransformersSession]):
+  """
+  sentence_transformers embedding model.
+  """
   Session = SentenceTransformersSession
 
   def __init__(self, model_name: str):
     self._model_name = model_name
```

### Comparing `langdash-0.0.3.dev2/langdash/models/transformers.py` & `langdash-0.0.4.dev1/langdash/models/transformers.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,18 @@
 @dataclass
 class TransformersState(LLMState):
   _logits: Optional[torch.Tensor] = None
   _past_key_values: Any = None
   _next_token: Optional[Tuple[int, str]] = None
 
 class TransformersSession(LLMGenerationSessionForRawText["TransformersModel", TransformersState, torch.Tensor]):
+  """
+  Session for transformers model.
+  """
+  
   _next_token: Optional[Tuple[int, str]]
   
   def __init__(self, *args, **kwargs):
     super().__init__(*args, **kwargs)
     
     def load_model(llm: TransformersModel):
       model = transformers.AutoModelForCausalLM.from_pretrained(llm._model_name)
@@ -159,14 +163,17 @@
         yield RespInfer(tokid=tokid, tokstr=tokstr, running_infer=generated)
       
       self._logits = self._eval(tokid)
     
     yield RespInfer(tokid=0, tokstr="", running_infer=generated)
 
 class TransformersModel(LLM[TransformersSession]):
+  """
+  transformers model.
+  """
   Session = TransformersSession
   
   def __init__(self, model_name: str, tokenizer_name: Optional[str] = None):
     """
     Creates a template for a language model powered by the transformers library.
     
     Args:
```

### Comparing `langdash-0.0.3.dev2/langdash/sampling.py` & `langdash-0.0.4.dev1/langdash/sampling.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from typing import List
 from langdash.infer import InferArgs
 
 import torch
 from torch.nn import functional as F
 
 @torch.jit.script
-def sample_top_p(logits: torch.Tensor, top_p: float) -> torch.Tensor:
+def _sample_top_p(logits: torch.Tensor, top_p: float) -> torch.Tensor:
   assert 0.0 <= top_p <= 1.0, "top_p must be in [0.0, 1.0]"
   probs = F.softmax(logits, dim=-1)
   sorted_probs = torch.sort(probs, descending=True)[0]
   cumulative_probs = torch.cumsum(sorted_probs, dim=-1)
   cutoff = float(sorted_probs[torch.argmax((cumulative_probs > top_p).long())])
   probs[probs < cutoff] = 0
   return probs
 
 @torch.jit.script
-def sample_typical(logits: torch.Tensor, mass: float) -> torch.Tensor:
+def _sample_typical(logits: torch.Tensor, mass: float) -> torch.Tensor:
   # https://github.com/huggingface/transformers/compare/main...cimeister:typicalsampling:typical-pr
   assert 0.0 <= mass <= 1.0, "typical mass must be in [0.0, 1.0]"
   
   probs = F.softmax(logits, dim=-1)
   normalized = -torch.log(probs)
   ent = torch.nansum(normalized * probs, dim=-1, keepdim=True)
   
@@ -28,15 +28,15 @@
   sorted_logits = logits.gather(-1, sorted_indices)
   cumulative_probs = sorted_logits.softmax(dim=-1).cumsum(dim=-1)
   
   I = (cumulative_probs < mass).sum()
   probs[shifted_scores > sorted_scores[I]] = 0.
   return probs
 
-def output_probs(
+def _output_probs(
   logits: torch.FloatTensor,
   args: InferArgs,
   ctx: List[int]
 ) -> torch.Tensor:
   # apply repetition penalty
   if args.rep_penalty != 1.0:
     rep_penalty = args.rep_penalty
@@ -46,22 +46,33 @@
         logits[tok] *= rep_penalty
       else:
         logits[tok] /= rep_penalty
   
   # probabilities
   if args.typical_mass > 0.0:
     # typical
-    probs = sample_typical(logits, args.typical_mass)
+    probs = _sample_typical(logits, args.typical_mass)
   else:
     # top-p
-    probs = sample_top_p(logits, args.top_p)
+    probs = _sample_top_p(logits, args.top_p)
   
   # apply temperature
   if args.temperature != 0.0:
     probs = probs.pow(1.0 / args.temperature)
     
   return probs
 
 def sample(*args, **kwargs) -> int:
-  probs = output_probs(*args, **kwargs)
+  """
+  Sample from a distribution of tokens specified by *logits*.
+  
+  Args:
+    logits (torch.FloatTensor): Logits to sample from.
+    args (InferArgs): Sampling arguments.
+    ctx (List[int]): List of current tokens generated.
+  
+  Returns:
+    The token generated.
+  """
+  probs = _output_probs(*args, **kwargs)
   return int(torch.multinomial(probs, num_samples=1)[0])
```

### Comparing `langdash-0.0.3.dev2/langdash/search/embedding_search.py` & `langdash-0.0.4.dev1/langdash/search/embedding_search.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev2/langdash/search/multichoice_search.py` & `langdash-0.0.4.dev1/langdash/search/multichoice_search.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.3.dev2/langdash.egg-info/PKG-INFO` & `langdash-0.0.4.dev1/langdash.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 0.0.3.dev2
+Version: 0.0.4.dev1
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: embeddings
 Provides-Extra: rwkvcpp
 Provides-Extra: transformers
 Provides-Extra: sentence_transformers
```

