# Comparing `tmp/langdash-0.0.2.dev2.tar.gz` & `tmp/langdash-0.0.3.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langdash-0.0.2.dev2.tar", last modified: Tue May 30 15:34:23 2023, max compression
+gzip compressed data, was "langdash-0.0.3.dev1.tar", last modified: Wed May 31 00:48:39 2023, max compression
```

## Comparing `langdash-0.0.2.dev2.tar` & `langdash-0.0.3.dev1.tar`

### file list

```diff
@@ -1,257 +1,257 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.284158 langdash-0.0.2.dev2/
--rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-0.0.2.dev2/LICENSE.txt
--rw-rw-r--   0 user      (1000) user      (1000)     3436 2023-05-30 15:34:23.284158 langdash-0.0.2.dev2/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     2670 2023-05-30 08:29:06.000000 langdash-0.0.2.dev2/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.176167 langdash-0.0.2.dev2/langdash/
--rw-rw-r--   0 user      (1000) user      (1000)       31 2023-05-25 22:58:46.000000 langdash-0.0.2.dev2/langdash/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3129 2023-05-30 08:35:04.000000 langdash-0.0.2.dev2/langdash/_langdash.py
--rw-rw-r--   0 user      (1000) user      (1000)    14626 2023-05-30 08:35:25.000000 langdash-0.0.2.dev2/langdash/chains.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.176167 langdash-0.0.2.dev2/langdash/classify/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-0.0.2.dev2/langdash/classify/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1780 2023-05-28 17:07:24.000000 langdash-0.0.2.dev2/langdash/classify/token_qa.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.168168 langdash-0.0.2.dev2/langdash/extern/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.184167 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/
--rw-rw-r--   0 user      (1000) user      (1000)    16349 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeCache.txt
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.184167 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.188166 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/
--rw-r--r--   0 user      (1000) user      (1000)     2441 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeCCompiler.cmake
--rw-r--r--   0 user      (1000) user      (1000)     5439 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeCXXCompiler.cmake
--rwxrwxr-x   0 user      (1000) user      (1000)    15968 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeDetermineCompilerABI_C.bin
--rwxrwxr-x   0 user      (1000) user      (1000)    15992 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeDetermineCompilerABI_CXX.bin
--rw-r--r--   0 user      (1000) user      (1000)      402 2023-05-25 00:05:29.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeSystem.cmake
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.188166 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdC/
--rw-rw-r--   0 user      (1000) user      (1000)    24853 2023-05-25 00:05:29.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdC/CMakeCCompilerId.c
--rwxrwxr-x   0 user      (1000) user      (1000)    16088 2023-05-25 00:05:29.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdC/a.out
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.188166 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdCXX/
--rw-rw-r--   0 user      (1000) user      (1000)    24597 2023-05-25 00:05:29.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdCXX/CMakeCXXCompilerId.cpp
--rwxrwxr-x   0 user      (1000) user      (1000)    16096 2023-05-25 00:05:29.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdCXX/a.out
--rw-rw-r--   0 user      (1000) user      (1000)      706 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/CMakeDirectoryInformation.cmake
--rw-rw-r--   0 user      (1000) user      (1000)    50084 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/CMakeOutput.log
--rw-rw-r--   0 user      (1000) user      (1000)     7911 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/Makefile.cmake
--rw-rw-r--   0 user      (1000) user      (1000)     9844 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/Makefile2
--rw-rw-r--   0 user      (1000) user      (1000)     3155 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/TargetDirectories.txt
--rw-rw-r--   0 user      (1000) user      (1000)       85 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/cmake.check_cache
--rw-rw-r--   0 user      (1000) user      (1000)        2 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/progress.marks
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.192166 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/
--rw-rw-r--   0 user      (1000) user      (1000)      692 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/DependInfo.cmake
--rw-rw-r--   0 user      (1000) user      (1000)     4674 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/build.make
--rw-rw-r--   0 user      (1000) user      (1000)      276 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/cmake_clean.cmake
--rw-rw-r--   0 user      (1000) user      (1000)      107 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/compiler_depend.make
--rw-rw-r--   0 user      (1000) user      (1000)      111 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/compiler_depend.ts
--rw-rw-r--   0 user      (1000) user      (1000)       88 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/depend.make
--rw-rw-r--   0 user      (1000) user      (1000)      679 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/flags.make
--rw-rw-r--   0 user      (1000) user      (1000)      133 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/link.txt
--rw-rw-r--   0 user      (1000) user      (1000)       43 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/progress.make
--rw-rw-r--   0 user      (1000) user      (1000)   101576 2023-05-25 00:05:37.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/rwkv.cpp.o
--rw-rw-r--   0 user      (1000) user      (1000)    11910 2023-05-25 00:05:37.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/rwkv.cpp.o.d
--rw-rw-r--   0 user      (1000) user      (1000)     6908 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)      376 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CTestTestfile.cmake
--rw-rw-r--   0 user      (1000) user      (1000)     1338 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/FILE_FORMAT.md
--rw-rw-r--   0 user      (1000) user      (1000)     1067 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)     8978 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/Makefile
--rw-rw-r--   0 user      (1000) user      (1000)     6412 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.196166 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)   165600 2023-05-25 00:05:38.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/bin/test_ggml_basics
--rwxrwxr-x   0 user      (1000) user      (1000)    16728 2023-05-25 00:05:38.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/bin/test_tiny_rwkv
--rw-rw-r--   0 user      (1000) user      (1000)     2013 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/cmake_install.cmake
--rw-rw-r--   0 user      (1000) user      (1000)     3799 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/compile_commands.json
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.196166 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.196166 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/CMakeFiles/
--rw-rw-r--   0 user      (1000) user      (1000)      706 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/CMakeFiles/CMakeDirectoryInformation.cmake
--rw-rw-r--   0 user      (1000) user      (1000)        2 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/CMakeFiles/progress.marks
--rw-rw-r--   0 user      (1000) user      (1000)     2552 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)     1072 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)     7013 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/Makefile
--rw-rw-r--   0 user      (1000) user      (1000)     3707 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.196166 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/cmake/
--rw-rw-r--   0 user      (1000) user      (1000)     2037 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/cmake/BuildTypes.cmake
--rw-rw-r--   0 user      (1000) user      (1000)      717 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/cmake/GitVars.cmake
--rw-rw-r--   0 user      (1000) user      (1000)     1496 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/cmake_install.cmake
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.200165 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/
--rw-rw-r--   0 user      (1000) user      (1000)      433 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)     8583 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/common-ggml.cpp
--rw-rw-r--   0 user      (1000) user      (1000)      410 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/common-ggml.h
--rw-rw-r--   0 user      (1000) user      (1000)    15664 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/common.cpp
--rw-rw-r--   0 user      (1000) user      (1000)     3311 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/common.h
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.200165 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/
--rw-rw-r--   0 user      (1000) user      (1000)      319 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)     6201 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/README.md
--rw-rw-r--   0 user      (1000) user      (1000)     3490 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/convert-h5-to-ggml.py
--rw-rw-r--   0 user      (1000) user      (1000)    28339 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/main.cpp
--rw-rw-r--   0 user      (1000) user      (1000)     5200 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/quantize.cpp
--rw-rw-r--   0 user      (1000) user      (1000)   241358 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/dr_wav.h
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.204165 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/
--rw-rw-r--   0 user      (1000) user      (1000)      311 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)     6370 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/README.md
--rw-rw-r--   0 user      (1000) user      (1000)     6313 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/convert-cerebras-to-ggml.py
--rw-rw-r--   0 user      (1000) user      (1000)     4873 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/convert-ckpt-to-ggml.py
--rw-rw-r--   0 user      (1000) user      (1000)     6436 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/convert-h5-to-ggml.py
--rwxrwxr-x   0 user      (1000) user      (1000)     1752 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/download-ggml-model.sh
--rwxrwxr-x   0 user      (1000) user      (1000)     1117 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/download-model.sh
--rw-rw-r--   0 user      (1000) user      (1000)    29187 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/main.cpp
--rw-rw-r--   0 user      (1000) user      (1000)     5467 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/quantize.cpp
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.204165 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/
--rw-rw-r--   0 user      (1000) user      (1000)      311 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)    11108 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/README.md
--rw-rw-r--   0 user      (1000) user      (1000)     5509 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/convert-h5-to-ggml.py
--rwxrwxr-x   0 user      (1000) user      (1000)     1728 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/download-ggml-model.sh
--rwxrwxr-x   0 user      (1000) user      (1000)      571 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/download-model.sh
--rw-rw-r--   0 user      (1000) user      (1000)    25782 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/main.cpp
--rw-rw-r--   0 user      (1000) user      (1000)     5469 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/quantize.cpp
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.208165 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/
--rw-rw-r--   0 user      (1000) user      (1000)      133 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)     3689 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/README.md
--rw-rw-r--   0 user      (1000) user      (1000)     1491 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/convert-h5-to-ggml.py
--rw-rw-r--   0 user      (1000) user      (1000)     7679 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/main.cpp
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.172168 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/models/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.212164 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/models/mnist/
--rw-rw-r--   0 user      (1000) user      (1000)  1591571 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/models/mnist/mnist_model.state_dict
--rw-rw-r--   0 user      (1000) user      (1000)  7840016 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/models/mnist/t10k-images.idx3-ubyte
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.232163 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/stablelm/
--rw-rw-r--   0 user      (1000) user      (1000)      323 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/stablelm/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)     4755 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/stablelm/README.md
--rw-rw-r--   0 user      (1000) user      (1000)     3490 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/stablelm/convert-h5-to-ggml.py
--rw-rw-r--   0 user      (1000) user      (1000)    27316 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/stablelm/main.cpp
--rw-rw-r--   0 user      (1000) user      (1000)     5200 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/stablelm/quantize.cpp
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.236162 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/
--rw-rw-r--   0 user      (1000) user      (1000)      501 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)      718 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/README.md
--rw-rw-r--   0 user      (1000) user      (1000)     9506 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/convert-pt-to-ggml.py
--rw-rw-r--   0 user      (1000) user      (1000)    36271 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/main.cpp
--rw-rw-r--   0 user      (1000) user      (1000)     7693 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/quantize.cpp
--rw-rw-r--   0 user      (1000) user      (1000)   184690 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/whisper.cpp
--rw-rw-r--   0 user      (1000) user      (1000)    23750 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/whisper.h
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.172168 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/include/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.236162 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/include/ggml/
--rw-rw-r--   0 user      (1000) user      (1000)    31202 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/include/ggml/ggml.h
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.236162 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/scripts/
--rwxrwxr-x   0 user      (1000) user      (1000)      323 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/scripts/sync-llama.sh
--rwxrwxr-x   0 user      (1000) user      (1000)      921 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/scripts/sync-whisper.sh
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.240162 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.240162 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/
--rw-rw-r--   0 user      (1000) user      (1000)      706 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/CMakeDirectoryInformation.cmake
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.244161 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/
--rw-rw-r--   0 user      (1000) user      (1000)      597 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/DependInfo.cmake
--rw-rw-r--   0 user      (1000) user      (1000)     5420 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/build.make
--rw-rw-r--   0 user      (1000) user      (1000)      269 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/cmake_clean.cmake
--rw-rw-r--   0 user      (1000) user      (1000)       36 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/cmake_clean_target.cmake
--rw-rw-r--   0 user      (1000) user      (1000)      107 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/compiler_depend.make
--rw-rw-r--   0 user      (1000) user      (1000)      111 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/compiler_depend.ts
--rw-rw-r--   0 user      (1000) user      (1000)       88 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/depend.make
--rw-rw-r--   0 user      (1000) user      (1000)     1057 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/flags.make
--rw-rw-r--   0 user      (1000) user      (1000)   201672 2023-05-25 00:05:35.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/ggml.c.o
--rw-rw-r--   0 user      (1000) user      (1000)    10631 2023-05-25 00:05:35.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/ggml.c.o.d
--rw-rw-r--   0 user      (1000) user      (1000)       80 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/link.txt
--rw-rw-r--   0 user      (1000) user      (1000)       43 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/progress.make
--rw-rw-r--   0 user      (1000) user      (1000)        2 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/progress.marks
--rw-rw-r--   0 user      (1000) user      (1000)     8040 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)     8522 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/Makefile
--rw-rw-r--   0 user      (1000) user      (1000)     1573 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/cmake_install.cmake
--rw-rw-r--   0 user      (1000) user      (1000)    24594 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/ggml-cuda.cu
--rw-rw-r--   0 user      (1000) user      (1000)      638 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/ggml-cuda.h
--rw-rw-r--   0 user      (1000) user      (1000)    13447 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/ggml-opencl.c
--rw-rw-r--   0 user      (1000) user      (1000)      639 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/ggml-opencl.h
--rw-rw-r--   0 user      (1000) user      (1000)   428283 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/ggml.c
--rw-rw-r--   0 user      (1000) user      (1000)   205118 2023-05-25 00:05:35.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/libggml.a
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.252161 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/
--rw-rw-r--   0 user      (1000) user      (1000)     9198 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)     6569 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-blas0.c
--rw-rw-r--   0 user      (1000) user      (1000)    11463 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-grad0.c
--rw-rw-r--   0 user      (1000) user      (1000)    10265 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-mul-mat0.c
--rw-rw-r--   0 user      (1000) user      (1000)     9003 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-mul-mat1.c
--rw-rw-r--   0 user      (1000) user      (1000)    91837 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-mul-mat2.c
--rw-rw-r--   0 user      (1000) user      (1000)     5141 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-svd0.c
--rw-rw-r--   0 user      (1000) user      (1000)     3157 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-vec0.c
--rw-rw-r--   0 user      (1000) user      (1000)    21179 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-vec1.c
--rw-rw-r--   0 user      (1000) user      (1000)     7310 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-vec2.c
--rw-rw-r--   0 user      (1000) user      (1000)     1182 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test0.c
--rw-rw-r--   0 user      (1000) user      (1000)    15073 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test1.c
--rw-rw-r--   0 user      (1000) user      (1000)     5703 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test2.c
--rw-rw-r--   0 user      (1000) user      (1000)     2841 2023-05-25 00:05:22.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test3.c
--rwxrwxr-x   0 user      (1000) user      (1000)   243024 2023-05-25 00:05:38.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/librwkv.so
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.260160 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/
--rw-rw-r--   0 user      (1000) user      (1000)  2467981 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/20B_tokenizer.json
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.264160 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/__pycache__/
--rw-rw-r--   0 user      (1000) user      (1000)     4174 2023-05-25 00:05:38.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/__pycache__/rwkv_cpp_model.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)     6921 2023-05-25 00:05:39.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/__pycache__/rwkv_cpp_shared_library.cpython-310.pyc
--rw-rw-r--   0 user      (1000) user      (1000)     8813 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/chat_with_bot.py
--rw-rw-r--   0 user      (1000) user      (1000)     3320 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/convert_pytorch_to_ggml.py
--rw-rw-r--   0 user      (1000) user      (1000)     1463 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/convert_pytorch_to_ggml.test.py
--rw-rw-r--   0 user      (1000) user      (1000)     2380 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/generate_completions.py
--rw-rw-r--   0 user      (1000) user      (1000)     3886 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/measure_pexplexity.py
--rw-rw-r--   0 user      (1000) user      (1000)     5833 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/merge_lora_into_ggml.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.264160 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/
--rw-rw-r--   0 user      (1000) user      (1000)      947 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/Chinese-Chat.json
--rw-rw-r--   0 user      (1000) user      (1000)      139 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/Chinese-QA.json
--rw-rw-r--   0 user      (1000) user      (1000)     1095 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/English-Chat.json
--rw-rw-r--   0 user      (1000) user      (1000)      764 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/English-QA.json
--rw-rw-r--   0 user      (1000) user      (1000)     1433 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/Japanese-Chat.json
--rw-rw-r--   0 user      (1000) user      (1000)      979 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/Japanese-QA.json
--rw-rw-r--   0 user      (1000) user      (1000)     1106 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/quantize.py
--rw-rw-r--   0 user      (1000) user      (1000)       23 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/requirements.txt
--rw-rw-r--   0 user      (1000) user      (1000)     4359 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/rwkv_cpp_model.py
--rw-rw-r--   0 user      (1000) user      (1000)     7528 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/rwkv_cpp_shared_library.py
--rw-rw-r--   0 user      (1000) user      (1000)     1255 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/sampling.py
--rw-rw-r--   0 user      (1000) user      (1000)    39641 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv.cpp
--rw-rw-r--   0 user      (1000) user      (1000)     4691 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv.h
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.272159 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.280158 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/
--rw-rw-r--   0 user      (1000) user      (1000)      706 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/CMakeDirectoryInformation.cmake
--rw-rw-r--   0 user      (1000) user      (1000)        2 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/progress.marks
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.280158 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/
--rw-rw-r--   0 user      (1000) user      (1000)      871 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/DependInfo.cmake
--rw-rw-r--   0 user      (1000) user      (1000)     5923 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/build.make
--rw-rw-r--   0 user      (1000) user      (1000)      359 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/cmake_clean.cmake
--rw-rw-r--   0 user      (1000) user      (1000)      119 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/compiler_depend.make
--rw-rw-r--   0 user      (1000) user      (1000)      123 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/compiler_depend.ts
--rw-rw-r--   0 user      (1000) user      (1000)      100 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/depend.make
--rw-rw-r--   0 user      (1000) user      (1000)      670 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/flags.make
--rw-rw-r--   0 user      (1000) user      (1000)      224 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/link.txt
--rw-rw-r--   0 user      (1000) user      (1000)       43 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/progress.make
--rw-rw-r--   0 user      (1000) user      (1000)     5152 2023-05-25 00:05:38.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/test_ggml_basics.c.o
--rw-rw-r--   0 user      (1000) user      (1000)     3717 2023-05-25 00:05:38.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/test_ggml_basics.c.o.d
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.284158 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/
--rw-rw-r--   0 user      (1000) user      (1000)      861 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/DependInfo.cmake
--rw-rw-r--   0 user      (1000) user      (1000)     5799 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/build.make
--rw-rw-r--   0 user      (1000) user      (1000)      345 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/cmake_clean.cmake
--rw-rw-r--   0 user      (1000) user      (1000)      117 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/compiler_depend.make
--rw-rw-r--   0 user      (1000) user      (1000)      121 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/compiler_depend.ts
--rw-rw-r--   0 user      (1000) user      (1000)       98 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/depend.make
--rw-rw-r--   0 user      (1000) user      (1000)      670 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/flags.make
--rw-rw-r--   0 user      (1000) user      (1000)      218 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/link.txt
--rw-rw-r--   0 user      (1000) user      (1000)       43 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/progress.make
--rw-rw-r--   0 user      (1000) user      (1000)     9816 2023-05-25 00:05:38.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/test_tiny_rwkv.c.o
--rw-rw-r--   0 user      (1000) user      (1000)     4064 2023-05-25 00:05:38.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/test_tiny_rwkv.c.o.d
--rw-rw-r--   0 user      (1000) user      (1000)      577 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeLists.txt
--rw-rw-r--   0 user      (1000) user      (1000)     1309 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CTestTestfile.cmake
--rw-rw-r--   0 user      (1000) user      (1000)    10760 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/Makefile
--rw-rw-r--   0 user      (1000) user      (1000)     1292 2023-05-25 00:05:30.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/cmake_install.cmake
--rw-rw-r--   0 user      (1000) user      (1000)     1024 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/expected_logits.bin
--rw-rw-r--   0 user      (1000) user      (1000)     1724 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/test_ggml_basics.c
--rw-rw-r--   0 user      (1000) user      (1000)     5039 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/test_tiny_rwkv.c
--rw-rw-r--   0 user      (1000) user      (1000)  1338429 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/tiny-rwkv-660K-FP16.bin
--rw-rw-r--   0 user      (1000) user      (1000)  2649149 2023-05-25 00:04:50.000000 langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/tiny-rwkv-660K-FP32.bin
--rw-rw-r--   0 user      (1000) user      (1000)      217 2023-05-30 08:12:32.000000 langdash-0.0.2.dev2/langdash/infer.py
--rw-rw-r--   0 user      (1000) user      (1000)     1212 2023-05-30 08:27:52.000000 langdash-0.0.2.dev2/langdash/llm.py
--rw-rw-r--   0 user      (1000) user      (1000)     6466 2023-05-30 08:56:47.000000 langdash-0.0.2.dev2/langdash/llm_session.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.176167 langdash-0.0.2.dev2/langdash/models/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:36.000000 langdash-0.0.2.dev2/langdash/models/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      624 2023-05-25 22:58:44.000000 langdash-0.0.2.dev2/langdash/models/mock.py
--rw-rw-r--   0 user      (1000) user      (1000)     6967 2023-05-30 08:14:45.000000 langdash-0.0.2.dev2/langdash/models/rwkvcpp.py
--rw-rw-r--   0 user      (1000) user      (1000)      840 2023-05-29 18:14:56.000000 langdash-0.0.2.dev2/langdash/models/sentence_transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)     6066 2023-05-30 08:16:06.000000 langdash-0.0.2.dev2/langdash/models/transformers.py
--rw-rw-r--   0 user      (1000) user      (1000)      259 2023-05-25 22:58:46.000000 langdash-0.0.2.dev2/langdash/response.py
--rw-rw-r--   0 user      (1000) user      (1000)     2156 2023-05-27 04:12:41.000000 langdash-0.0.2.dev2/langdash/sampling.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.176167 langdash-0.0.2.dev2/langdash/search/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-0.0.2.dev2/langdash/search/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      840 2023-05-29 19:25:03.000000 langdash-0.0.2.dev2/langdash/search/embedding_search.py
--rw-rw-r--   0 user      (1000) user      (1000)      260 2023-05-27 05:17:38.000000 langdash-0.0.2.dev2/langdash/search/engine.py
--rw-rw-r--   0 user      (1000) user      (1000)     2391 2023-05-28 22:28:07.000000 langdash-0.0.2.dev2/langdash/search/multichoice_search.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-30 15:34:23.180167 langdash-0.0.2.dev2/langdash.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     3436 2023-05-30 15:34:23.000000 langdash-0.0.2.dev2/langdash.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    12207 2023-05-30 15:34:23.000000 langdash-0.0.2.dev2/langdash.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-30 15:34:23.000000 langdash-0.0.2.dev2/langdash.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      124 2023-05-30 15:34:23.000000 langdash-0.0.2.dev2/langdash.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        9 2023-05-30 15:34:23.000000 langdash-0.0.2.dev2/langdash.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-05-30 15:34:23.284158 langdash-0.0.2.dev2/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1262 2023-05-30 15:33:03.000000 langdash-0.0.2.dev2/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.712409 langdash-0.0.3.dev1/
+-rw-rw-r--   0 user      (1000) user      (1000)    10786 2023-05-30 02:56:17.000000 langdash-0.0.3.dev1/LICENSE.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     3436 2023-05-31 00:48:39.712409 langdash-0.0.3.dev1/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     2670 2023-05-30 08:29:06.000000 langdash-0.0.3.dev1/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.628407 langdash-0.0.3.dev1/langdash/
+-rw-rw-r--   0 user      (1000) user      (1000)       31 2023-05-25 22:58:46.000000 langdash-0.0.3.dev1/langdash/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3596 2023-05-30 19:46:43.000000 langdash-0.0.3.dev1/langdash/_langdash.py
+-rw-rw-r--   0 user      (1000) user      (1000)    16507 2023-05-30 22:12:14.000000 langdash-0.0.3.dev1/langdash/chains.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.628407 langdash-0.0.3.dev1/langdash/classify/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:31.000000 langdash-0.0.3.dev1/langdash/classify/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1780 2023-05-28 17:07:24.000000 langdash-0.0.3.dev1/langdash/classify/token_qa.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.620406 langdash-0.0.3.dev1/langdash/extern/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.636407 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/
+-rw-rw-r--   0 user      (1000) user      (1000)    16349 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeCache.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.636407 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.636407 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/
+-rw-r--r--   0 user      (1000) user      (1000)     2441 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeCCompiler.cmake
+-rw-r--r--   0 user      (1000) user      (1000)     5439 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeCXXCompiler.cmake
+-rwxrwxr-x   0 user      (1000) user      (1000)    15968 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeDetermineCompilerABI_C.bin
+-rwxrwxr-x   0 user      (1000) user      (1000)    15992 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeDetermineCompilerABI_CXX.bin
+-rw-r--r--   0 user      (1000) user      (1000)      402 2023-05-25 00:05:29.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeSystem.cmake
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.636407 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdC/
+-rw-rw-r--   0 user      (1000) user      (1000)    24853 2023-05-25 00:05:29.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdC/CMakeCCompilerId.c
+-rwxrwxr-x   0 user      (1000) user      (1000)    16088 2023-05-25 00:05:29.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdC/a.out
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.640407 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdCXX/
+-rw-rw-r--   0 user      (1000) user      (1000)    24597 2023-05-25 00:05:29.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdCXX/CMakeCXXCompilerId.cpp
+-rwxrwxr-x   0 user      (1000) user      (1000)    16096 2023-05-25 00:05:29.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdCXX/a.out
+-rw-rw-r--   0 user      (1000) user      (1000)      706 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/CMakeDirectoryInformation.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)    50084 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/CMakeOutput.log
+-rw-rw-r--   0 user      (1000) user      (1000)     7911 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/Makefile.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)     9844 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/Makefile2
+-rw-rw-r--   0 user      (1000) user      (1000)     3155 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/TargetDirectories.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       85 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/cmake.check_cache
+-rw-rw-r--   0 user      (1000) user      (1000)        2 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/progress.marks
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.640407 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/
+-rw-rw-r--   0 user      (1000) user      (1000)      692 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/DependInfo.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)     4674 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/build.make
+-rw-rw-r--   0 user      (1000) user      (1000)      276 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/cmake_clean.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)      107 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/compiler_depend.make
+-rw-rw-r--   0 user      (1000) user      (1000)      111 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/compiler_depend.ts
+-rw-rw-r--   0 user      (1000) user      (1000)       88 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/depend.make
+-rw-rw-r--   0 user      (1000) user      (1000)      679 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/flags.make
+-rw-rw-r--   0 user      (1000) user      (1000)      133 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/link.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       43 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/progress.make
+-rw-rw-r--   0 user      (1000) user      (1000)   101576 2023-05-25 00:05:37.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/rwkv.cpp.o
+-rw-rw-r--   0 user      (1000) user      (1000)    11910 2023-05-25 00:05:37.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/rwkv.cpp.o.d
+-rw-rw-r--   0 user      (1000) user      (1000)     6908 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeLists.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      376 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CTestTestfile.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)     1338 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/FILE_FORMAT.md
+-rw-rw-r--   0 user      (1000) user      (1000)     1067 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)     8978 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/Makefile
+-rw-rw-r--   0 user      (1000) user      (1000)     6412 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.640407 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)   165600 2023-05-25 00:05:38.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/bin/test_ggml_basics
+-rwxrwxr-x   0 user      (1000) user      (1000)    16728 2023-05-25 00:05:38.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/bin/test_tiny_rwkv
+-rw-rw-r--   0 user      (1000) user      (1000)     2013 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/cmake_install.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)     3799 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/compile_commands.json
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.644407 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.644407 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/CMakeFiles/
+-rw-rw-r--   0 user      (1000) user      (1000)      706 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/CMakeFiles/CMakeDirectoryInformation.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)        2 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/CMakeFiles/progress.marks
+-rw-rw-r--   0 user      (1000) user      (1000)     2552 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/CMakeLists.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     1072 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)     7013 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/Makefile
+-rw-rw-r--   0 user      (1000) user      (1000)     3707 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.644407 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/cmake/
+-rw-rw-r--   0 user      (1000) user      (1000)     2037 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/cmake/BuildTypes.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)      717 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/cmake/GitVars.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)     1496 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/cmake_install.cmake
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.644407 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/
+-rw-rw-r--   0 user      (1000) user      (1000)      433 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/CMakeLists.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     8583 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/common-ggml.cpp
+-rw-rw-r--   0 user      (1000) user      (1000)      410 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/common-ggml.h
+-rw-rw-r--   0 user      (1000) user      (1000)    15664 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/common.cpp
+-rw-rw-r--   0 user      (1000) user      (1000)     3311 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/common.h
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.644407 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/
+-rw-rw-r--   0 user      (1000) user      (1000)      319 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/CMakeLists.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     6201 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)     3490 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/convert-h5-to-ggml.py
+-rw-rw-r--   0 user      (1000) user      (1000)    28339 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/main.cpp
+-rw-rw-r--   0 user      (1000) user      (1000)     5200 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/quantize.cpp
+-rw-rw-r--   0 user      (1000) user      (1000)   241358 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/dr_wav.h
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.648407 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/
+-rw-rw-r--   0 user      (1000) user      (1000)      311 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/CMakeLists.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     6370 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)     6313 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/convert-cerebras-to-ggml.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4873 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/convert-ckpt-to-ggml.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6436 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/convert-h5-to-ggml.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     1752 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/download-ggml-model.sh
+-rwxrwxr-x   0 user      (1000) user      (1000)     1117 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/download-model.sh
+-rw-rw-r--   0 user      (1000) user      (1000)    29187 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/main.cpp
+-rw-rw-r--   0 user      (1000) user      (1000)     5467 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/quantize.cpp
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.648407 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/
+-rw-rw-r--   0 user      (1000) user      (1000)      311 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/CMakeLists.txt
+-rw-rw-r--   0 user      (1000) user      (1000)    11108 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)     5509 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/convert-h5-to-ggml.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     1728 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/download-ggml-model.sh
+-rwxrwxr-x   0 user      (1000) user      (1000)      571 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/download-model.sh
+-rw-rw-r--   0 user      (1000) user      (1000)    25782 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/main.cpp
+-rw-rw-r--   0 user      (1000) user      (1000)     5469 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/quantize.cpp
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.648407 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/
+-rw-rw-r--   0 user      (1000) user      (1000)      133 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/CMakeLists.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     3689 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)     1491 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/convert-h5-to-ggml.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7679 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/main.cpp
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.624406 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/models/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.652407 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/models/mnist/
+-rw-rw-r--   0 user      (1000) user      (1000)  1591571 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/models/mnist/mnist_model.state_dict
+-rw-rw-r--   0 user      (1000) user      (1000)  7840016 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/models/mnist/t10k-images.idx3-ubyte
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.668408 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/stablelm/
+-rw-rw-r--   0 user      (1000) user      (1000)      323 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/stablelm/CMakeLists.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     4755 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/stablelm/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)     3490 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/stablelm/convert-h5-to-ggml.py
+-rw-rw-r--   0 user      (1000) user      (1000)    27316 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/stablelm/main.cpp
+-rw-rw-r--   0 user      (1000) user      (1000)     5200 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/stablelm/quantize.cpp
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.672408 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/
+-rw-rw-r--   0 user      (1000) user      (1000)      501 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/CMakeLists.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      718 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)     9506 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/convert-pt-to-ggml.py
+-rw-rw-r--   0 user      (1000) user      (1000)    36271 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/main.cpp
+-rw-rw-r--   0 user      (1000) user      (1000)     7693 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/quantize.cpp
+-rw-rw-r--   0 user      (1000) user      (1000)   184690 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/whisper.cpp
+-rw-rw-r--   0 user      (1000) user      (1000)    23750 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/whisper.h
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.624406 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/include/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.672408 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/include/ggml/
+-rw-rw-r--   0 user      (1000) user      (1000)    31202 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/include/ggml/ggml.h
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.672408 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/scripts/
+-rwxrwxr-x   0 user      (1000) user      (1000)      323 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/scripts/sync-llama.sh
+-rwxrwxr-x   0 user      (1000) user      (1000)      921 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/scripts/sync-whisper.sh
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.676408 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.676408 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/
+-rw-rw-r--   0 user      (1000) user      (1000)      706 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/CMakeDirectoryInformation.cmake
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.680408 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/
+-rw-rw-r--   0 user      (1000) user      (1000)      597 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/DependInfo.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)     5420 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/build.make
+-rw-rw-r--   0 user      (1000) user      (1000)      269 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/cmake_clean.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)       36 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/cmake_clean_target.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)      107 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/compiler_depend.make
+-rw-rw-r--   0 user      (1000) user      (1000)      111 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/compiler_depend.ts
+-rw-rw-r--   0 user      (1000) user      (1000)       88 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/depend.make
+-rw-rw-r--   0 user      (1000) user      (1000)     1057 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/flags.make
+-rw-rw-r--   0 user      (1000) user      (1000)   201672 2023-05-25 00:05:35.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/ggml.c.o
+-rw-rw-r--   0 user      (1000) user      (1000)    10631 2023-05-25 00:05:35.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/ggml.c.o.d
+-rw-rw-r--   0 user      (1000) user      (1000)       80 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/link.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       43 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/progress.make
+-rw-rw-r--   0 user      (1000) user      (1000)        2 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/progress.marks
+-rw-rw-r--   0 user      (1000) user      (1000)     8040 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeLists.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     8522 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/Makefile
+-rw-rw-r--   0 user      (1000) user      (1000)     1573 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/cmake_install.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)    24594 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/ggml-cuda.cu
+-rw-rw-r--   0 user      (1000) user      (1000)      638 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/ggml-cuda.h
+-rw-rw-r--   0 user      (1000) user      (1000)    13447 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/ggml-opencl.c
+-rw-rw-r--   0 user      (1000) user      (1000)      639 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/ggml-opencl.h
+-rw-rw-r--   0 user      (1000) user      (1000)   428283 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/ggml.c
+-rw-rw-r--   0 user      (1000) user      (1000)   205118 2023-05-25 00:05:35.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/libggml.a
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.684408 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/
+-rw-rw-r--   0 user      (1000) user      (1000)     9198 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/CMakeLists.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     6569 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-blas0.c
+-rw-rw-r--   0 user      (1000) user      (1000)    11463 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-grad0.c
+-rw-rw-r--   0 user      (1000) user      (1000)    10265 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-mul-mat0.c
+-rw-rw-r--   0 user      (1000) user      (1000)     9003 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-mul-mat1.c
+-rw-rw-r--   0 user      (1000) user      (1000)    91837 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-mul-mat2.c
+-rw-rw-r--   0 user      (1000) user      (1000)     5141 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-svd0.c
+-rw-rw-r--   0 user      (1000) user      (1000)     3157 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-vec0.c
+-rw-rw-r--   0 user      (1000) user      (1000)    21179 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-vec1.c
+-rw-rw-r--   0 user      (1000) user      (1000)     7310 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-vec2.c
+-rw-rw-r--   0 user      (1000) user      (1000)     1182 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test0.c
+-rw-rw-r--   0 user      (1000) user      (1000)    15073 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test1.c
+-rw-rw-r--   0 user      (1000) user      (1000)     5703 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test2.c
+-rw-rw-r--   0 user      (1000) user      (1000)     2841 2023-05-25 00:05:22.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test3.c
+-rwxrwxr-x   0 user      (1000) user      (1000)   243024 2023-05-25 00:05:38.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/librwkv.so
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.688408 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/
+-rw-rw-r--   0 user      (1000) user      (1000)  2467981 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/20B_tokenizer.json
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.692408 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/__pycache__/
+-rw-rw-r--   0 user      (1000) user      (1000)     4174 2023-05-25 00:05:38.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/__pycache__/rwkv_cpp_model.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)     6921 2023-05-25 00:05:39.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/__pycache__/rwkv_cpp_shared_library.cpython-310.pyc
+-rw-rw-r--   0 user      (1000) user      (1000)     8813 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/chat_with_bot.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3320 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/convert_pytorch_to_ggml.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1463 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/convert_pytorch_to_ggml.test.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2380 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/generate_completions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3886 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/measure_pexplexity.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5833 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/merge_lora_into_ggml.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.692408 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/prompt/
+-rw-rw-r--   0 user      (1000) user      (1000)      947 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/prompt/Chinese-Chat.json
+-rw-rw-r--   0 user      (1000) user      (1000)      139 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/prompt/Chinese-QA.json
+-rw-rw-r--   0 user      (1000) user      (1000)     1095 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/prompt/English-Chat.json
+-rw-rw-r--   0 user      (1000) user      (1000)      764 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/prompt/English-QA.json
+-rw-rw-r--   0 user      (1000) user      (1000)     1433 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/prompt/Japanese-Chat.json
+-rw-rw-r--   0 user      (1000) user      (1000)      979 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/prompt/Japanese-QA.json
+-rw-rw-r--   0 user      (1000) user      (1000)     1106 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/quantize.py
+-rw-rw-r--   0 user      (1000) user      (1000)       23 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/requirements.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     4359 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/rwkv_cpp_model.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7528 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/rwkv_cpp_shared_library.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1255 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/sampling.py
+-rw-rw-r--   0 user      (1000) user      (1000)    39641 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv.cpp
+-rw-rw-r--   0 user      (1000) user      (1000)     4691 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv.h
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.696409 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.704409 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/
+-rw-rw-r--   0 user      (1000) user      (1000)      706 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/CMakeDirectoryInformation.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)        2 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/progress.marks
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.708409 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/
+-rw-rw-r--   0 user      (1000) user      (1000)      871 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/DependInfo.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)     5923 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/build.make
+-rw-rw-r--   0 user      (1000) user      (1000)      359 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/cmake_clean.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)      119 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/compiler_depend.make
+-rw-rw-r--   0 user      (1000) user      (1000)      123 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/compiler_depend.ts
+-rw-rw-r--   0 user      (1000) user      (1000)      100 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/depend.make
+-rw-rw-r--   0 user      (1000) user      (1000)      670 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/flags.make
+-rw-rw-r--   0 user      (1000) user      (1000)      224 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/link.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       43 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/progress.make
+-rw-rw-r--   0 user      (1000) user      (1000)     5152 2023-05-25 00:05:38.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/test_ggml_basics.c.o
+-rw-rw-r--   0 user      (1000) user      (1000)     3717 2023-05-25 00:05:38.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/test_ggml_basics.c.o.d
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.712409 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/
+-rw-rw-r--   0 user      (1000) user      (1000)      861 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/DependInfo.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)     5799 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/build.make
+-rw-rw-r--   0 user      (1000) user      (1000)      345 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/cmake_clean.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)      117 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/compiler_depend.make
+-rw-rw-r--   0 user      (1000) user      (1000)      121 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/compiler_depend.ts
+-rw-rw-r--   0 user      (1000) user      (1000)       98 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/depend.make
+-rw-rw-r--   0 user      (1000) user      (1000)      670 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/flags.make
+-rw-rw-r--   0 user      (1000) user      (1000)      218 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/link.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       43 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/progress.make
+-rw-rw-r--   0 user      (1000) user      (1000)     9816 2023-05-25 00:05:38.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/test_tiny_rwkv.c.o
+-rw-rw-r--   0 user      (1000) user      (1000)     4064 2023-05-25 00:05:38.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/test_tiny_rwkv.c.o.d
+-rw-rw-r--   0 user      (1000) user      (1000)      577 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeLists.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     1309 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CTestTestfile.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)    10760 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/Makefile
+-rw-rw-r--   0 user      (1000) user      (1000)     1292 2023-05-25 00:05:30.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/cmake_install.cmake
+-rw-rw-r--   0 user      (1000) user      (1000)     1024 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/expected_logits.bin
+-rw-rw-r--   0 user      (1000) user      (1000)     1724 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/test_ggml_basics.c
+-rw-rw-r--   0 user      (1000) user      (1000)     5039 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/test_tiny_rwkv.c
+-rw-rw-r--   0 user      (1000) user      (1000)  1338429 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/tiny-rwkv-660K-FP16.bin
+-rw-rw-r--   0 user      (1000) user      (1000)  2649149 2023-05-25 00:04:50.000000 langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/tiny-rwkv-660K-FP32.bin
+-rw-rw-r--   0 user      (1000) user      (1000)      217 2023-05-30 08:12:32.000000 langdash-0.0.3.dev1/langdash/infer.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1209 2023-05-30 19:56:33.000000 langdash-0.0.3.dev1/langdash/llm.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7101 2023-05-30 20:56:47.000000 langdash-0.0.3.dev1/langdash/llm_session.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.628407 langdash-0.0.3.dev1/langdash/models/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:36.000000 langdash-0.0.3.dev1/langdash/models/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      624 2023-05-25 22:58:44.000000 langdash-0.0.3.dev1/langdash/models/mock.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6964 2023-05-30 22:08:25.000000 langdash-0.0.3.dev1/langdash/models/rwkvcpp.py
+-rw-rw-r--   0 user      (1000) user      (1000)      840 2023-05-29 18:14:56.000000 langdash-0.0.3.dev1/langdash/models/sentence_transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6051 2023-05-30 22:02:01.000000 langdash-0.0.3.dev1/langdash/models/transformers.py
+-rw-rw-r--   0 user      (1000) user      (1000)      259 2023-05-25 22:58:46.000000 langdash-0.0.3.dev1/langdash/response.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2154 2023-05-30 19:25:05.000000 langdash-0.0.3.dev1/langdash/sampling.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.632407 langdash-0.0.3.dev1/langdash/search/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-05-30 02:28:40.000000 langdash-0.0.3.dev1/langdash/search/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      840 2023-05-29 19:25:03.000000 langdash-0.0.3.dev1/langdash/search/embedding_search.py
+-rw-rw-r--   0 user      (1000) user      (1000)      260 2023-05-27 05:17:38.000000 langdash-0.0.3.dev1/langdash/search/engine.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2391 2023-05-28 22:28:07.000000 langdash-0.0.3.dev1/langdash/search/multichoice_search.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-05-31 00:48:39.632407 langdash-0.0.3.dev1/langdash.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     3436 2023-05-31 00:48:39.000000 langdash-0.0.3.dev1/langdash.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    12207 2023-05-31 00:48:39.000000 langdash-0.0.3.dev1/langdash.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-05-31 00:48:39.000000 langdash-0.0.3.dev1/langdash.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      124 2023-05-31 00:48:39.000000 langdash-0.0.3.dev1/langdash.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        9 2023-05-31 00:48:39.000000 langdash-0.0.3.dev1/langdash.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-05-31 00:48:39.712409 langdash-0.0.3.dev1/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1262 2023-05-31 00:47:19.000000 langdash-0.0.3.dev1/setup.py
```

### Comparing `langdash-0.0.2.dev2/LICENSE.txt` & `langdash-0.0.3.dev1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/PKG-INFO` & `langdash-0.0.3.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 0.0.2.dev2
+Version: 0.0.3.dev1
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `langdash-0.0.2.dev2/README.md` & `langdash-0.0.3.dev1/README.md`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/_langdash.py` & `langdash-0.0.3.dev1/langdash/_langdash.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import gc
 from typing import Dict, Callable, TypeVar
 from langdash.llm import LLM
 from langdash.llm_session import LLMSession, T_LLM
-from langdash.chains import LDChain, LDText, LDFormatArg, LDArg, LDReturns
+from langdash.chains import LDChain, LDText, LDFormatArg, LDArg, LDReturns, LDChoice
 
 T_ModelInternal = TypeVar("T_ModelInternal")
 
 class Langdash:
   _models: Dict[str, LLM]
   
   def __init__(self):
@@ -114,7 +114,25 @@
       inference_args:
         The inference arguments for the function.
 
     Returns:
       The return node.
     """
     return LDReturns(self, *args, **kwargs)
+
+  def choice(self, *args, **kwargs):
+    """
+    Creates a new choice node with the specified choices, and returns to the .
+    
+    Args:
+      returns: The name of the return value.
+      choices: List of choice strings
+      padleft:
+        Left padding for every choice string.
+      padright:
+        Right padding for every choice string.
+    
+    Returns:
+      The newly created choice node.
+    """
+    return LDChoice(self, *args, **kwargs)
+
```

### Comparing `langdash-0.0.2.dev2/langdash/chains.py` & `langdash-0.0.3.dev1/langdash/chains.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from dataclasses import dataclass
 from collections import OrderedDict
 from typing import Generator, Dict, Any, List, Union, Optional, Type, Tuple, FrozenSet, TYPE_CHECKING
 import re
+import random
 
 from langdash.response import Response, RespInfer, RespInject, RespReturns
 from langdash.infer import InferArgs
 
 if TYPE_CHECKING:
   from langdash._langdash import Langdash
   from langdash.llm_session import LLMGenerationSession, LLMState
@@ -130,15 +131,15 @@
     if isinstance(ctx, LLMGenerationSession):
       return ctx
     else:
       return self._ld.session_for_model(ctx)
   
   def _stream(self, session: "LLMGenerationSession", args: LDNodeArgs):
     for node in self._node_pass(session, args):
-      if isinstance(node, LDReturns):
+      if isinstance(node, Union[LDReturns, LDChoice]):
         yield RespReturns(key=node._returns)
       yield from node(session, args)
   
   def stream(self, ctx: Union[str, "LLMGenerationSession"], **kwargs):
     """
     Stream data generated from the LLM within the specified session.
     
@@ -154,15 +155,15 @@
     args: LDNodeArgs = {},
     return_session: bool = False,
     set_global_args: bool = False,
   ) -> Union["LDResult", Tuple["LDResult", "LLMGenerationSession"]]:
     result = LDResult()
     for node in self._node_pass(session, args):
       generator = node(session, args)
-      if isinstance(node, LDReturns):
+      if isinstance(node, (LDReturns, LDChoice)):
         returns = node._returns
         result.update_results(returns, self._returns[returns], generator)
       else:
         result.update_stats(generator)
     if return_session:
       if set_global_args:
         session.global_args = args
@@ -297,14 +298,15 @@
       text_node = self._nodes[0]
       assert isinstance(text_node, LDText)
       session.inject(text_node._text)
       
       self._set_state_cache(
         frozenset(),
         LDChainCacheState(state=session.clone_state(), skip_nodes=1))
+      self._skip_nodes = 1
       
       return session
     
     if args is None:
       old_state_cache = self._get_state_cache(frozenset())
       self._skip_nodes = old_state_cache.skip_nodes
       session.set_state(old_state_cache.state)
@@ -359,15 +361,15 @@
     self.returns[key] = cast_function(text)
   
   def update_stats(self, generator: LDNodeGenerator):
     """
     Update the stats of the result, given a node generator.
     
     Args:
-      generator: Node generator that runs to get the results.
+      generator: Node generator to get the results.
     """
     for resp in generator:
       if isinstance(resp, RespInject):
         self.prompt_tokens += resp.tokens_counter
       else:
         continue
 
@@ -404,34 +406,32 @@
     tokens_counter = session.inject(self._text.format(globals=session.global_args, **args))
     yield RespInject(tokens_counter=tokens_counter)
 
 class LDArg(LDNode):
   
   def __init__(self, ld: "Langdash",
                arg: str,
-               padleft: Optional[str] = None,
-               padright: Optional[str] = None):
+               padleft: str = "",
+               padright: str = ""):
     super().__init__(ld)
     self._arg = arg
     self._padleft = padleft
     self._padright = padright
   
   def __repr__(self):
     return f"<Arg arg={self._arg}>"
   
   def __call__(self, session: "LLMGenerationSession", args: LDNodeArgs) -> LDNodeGenerator:
     s =  ""
-    if self._padleft is not None:
-      s += self._padleft
+    s += self._padleft
     if self._arg in args:
       s += str(args[self._arg])
     else:
       s += str(session.global_args[self._arg])
-    if self._padright is not None:
-      s += self._padright
+    s += self._padright
     tokens_counter = session.inject(s)
     yield RespInject(tokens_counter=tokens_counter)
   
 class LDReturns(LDNode):
   
   def __init__(self, ld: "Langdash",
                returns: str,
@@ -449,8 +449,65 @@
   
   def __call__(self, session: "LLMGenerationSession", args: LDNodeArgs) -> LDNodeGenerator:
     for i, respinfer in enumerate(session.infer(end=self._end, args=self._inference_args)):
       if i == 0:
         if self._padleft is not None and respinfer.tokstr.startswith(self._padleft):
           respinfer.tokstr = respinfer.tokstr[len(self._padleft):]
       yield respinfer
-      
+      
+class LDChoice(LDNode):
+  
+  def __init__(self, ld: "Langdash",
+               returns: str,
+               choices: List[str],
+               padleft: str = "",
+               padright: str = ""):
+    super().__init__(ld)
+    self._returns = returns
+    self._choices = choices
+    self._padleft = padleft
+    self._padright = padright
+    self._choices_preprocessed = [
+      f"{self._padleft}{choice}{self._padright}" for choice in self._choices
+    ]
+    
+  def __repr__(self):
+    return f"<Choices {self._returns}>"
+  
+  def __call__(self, session: "LLMGenerationSession", args: LDNodeArgs) -> LDNodeGenerator:
+    from langdash.llm_session import LLMGenerationSessionForRawText
+    
+    tokids = [-1] * len(self._choices_preprocessed)
+    has_multiple_tokens = False
+    
+    heal_padleft: Optional[str] = None
+    if session.token_healing and \
+      isinstance(session, LLMGenerationSessionForRawText) and \
+      session._next_token is not None:
+      heal_padleft = session._next_token[1]
+      session._next_token = None
+    
+    for i, text in enumerate(self._choices_preprocessed):
+      if heal_padleft is not None:
+        text_tokids = session.tokenize(heal_padleft + text)
+      else:
+        text_tokids = session.tokenize(text)
+      if len(text_tokids) > 1:
+        has_multiple_tokens = True
+        break
+      tokids[i] = text_tokids[0]
+      
+    if has_multiple_tokens:
+      # TODO: handle multiple tokens
+      raise NotImplementedError("handle multiple tokens not implemented")
+    else:
+      probs = session.next_token_probs()
+      weights = [probs[tokid] for tokid in tokids]
+      inject_idx = random.choices(range(len(self._choices)), weights=weights)[0]
+      tokid_inject = tokids[inject_idx]
+      session.inject(tokid_inject)
+      yield RespInfer(
+        tokid=tokid_inject,
+        tokstr=self._choices[inject_idx],
+        running_infer=self._choices[inject_idx],
+      )
+
```

### Comparing `langdash-0.0.2.dev2/langdash/classify/token_qa.py` & `langdash-0.0.3.dev1/langdash/classify/token_qa.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeCache.txt` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeCache.txt`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeCCompiler.cmake` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeCCompiler.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeCXXCompiler.cmake` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeCXXCompiler.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeDetermineCompilerABI_C.bin` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeDetermineCompilerABI_C.bin`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeDetermineCompilerABI_CXX.bin` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CMakeDetermineCompilerABI_CXX.bin`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdC/CMakeCCompilerId.c` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdC/CMakeCCompilerId.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdC/a.out` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdC/a.out`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdCXX/CMakeCXXCompilerId.cpp` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdCXX/CMakeCXXCompilerId.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdCXX/a.out` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/3.22.1/CompilerIdCXX/a.out`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/CMakeDirectoryInformation.cmake` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/CMakeDirectoryInformation.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/CMakeOutput.log` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/CMakeOutput.log`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/Makefile.cmake` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/Makefile.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/Makefile2` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/Makefile2`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/TargetDirectories.txt` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/TargetDirectories.txt`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/DependInfo.cmake` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/DependInfo.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/build.make` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/build.make`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/flags.make` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/flags.make`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/rwkv.cpp.o` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/rwkv.cpp.o`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/rwkv.cpp.o.d` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeFiles/rwkv.dir/rwkv.cpp.o.d`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/CMakeLists.txt` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/FILE_FORMAT.md` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/FILE_FORMAT.md`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/LICENSE` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/LICENSE`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/Makefile` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/Makefile`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/README.md` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/README.md`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/bin/test_ggml_basics` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/bin/test_ggml_basics`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/bin/test_tiny_rwkv` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/bin/test_tiny_rwkv`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/cmake_install.cmake` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/cmake_install.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/compile_commands.json` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/compile_commands.json`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/CMakeFiles/CMakeDirectoryInformation.cmake` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/CMakeFiles/CMakeDirectoryInformation.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/CMakeLists.txt` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/LICENSE` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/LICENSE`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/Makefile` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/Makefile`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/README.md` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/README.md`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/cmake/BuildTypes.cmake` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/cmake/BuildTypes.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/cmake/GitVars.cmake` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/cmake/GitVars.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/cmake_install.cmake` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/cmake_install.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/common-ggml.cpp` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/common-ggml.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/common.cpp` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/common.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/common.h` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/common.h`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/README.md` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/README.md`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/convert-h5-to-ggml.py` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/convert-h5-to-ggml.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/main.cpp` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/main.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/quantize.cpp` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/dolly-v2/quantize.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/dr_wav.h` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/dr_wav.h`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/README.md` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/README.md`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/convert-cerebras-to-ggml.py` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/convert-cerebras-to-ggml.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/convert-ckpt-to-ggml.py` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/convert-ckpt-to-ggml.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/convert-h5-to-ggml.py` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/convert-h5-to-ggml.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/download-ggml-model.sh` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/download-ggml-model.sh`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/download-model.sh` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/download-model.sh`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/main.cpp` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/main.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/quantize.cpp` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-2/quantize.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/README.md` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/README.md`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/convert-h5-to-ggml.py` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/convert-h5-to-ggml.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/download-ggml-model.sh` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/download-ggml-model.sh`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/download-model.sh` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/download-model.sh`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/main.cpp` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/main.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/quantize.cpp` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/gpt-j/quantize.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/README.md` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/README.md`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/convert-h5-to-ggml.py` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/convert-h5-to-ggml.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/main.cpp` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/main.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/models/mnist/mnist_model.state_dict` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/models/mnist/mnist_model.state_dict`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/mnist/models/mnist/t10k-images.idx3-ubyte` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/mnist/models/mnist/t10k-images.idx3-ubyte`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/stablelm/README.md` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/stablelm/README.md`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/stablelm/convert-h5-to-ggml.py` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/stablelm/convert-h5-to-ggml.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/stablelm/main.cpp` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/stablelm/main.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/stablelm/quantize.cpp` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/stablelm/quantize.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/README.md` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/README.md`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/convert-pt-to-ggml.py` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/convert-pt-to-ggml.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/main.cpp` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/main.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/quantize.cpp` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/quantize.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/whisper.cpp` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/whisper.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/examples/whisper/whisper.h` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/examples/whisper/whisper.h`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/include/ggml/ggml.h` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/include/ggml/ggml.h`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/scripts/sync-whisper.sh` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/scripts/sync-whisper.sh`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/CMakeDirectoryInformation.cmake` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/CMakeDirectoryInformation.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/DependInfo.cmake` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/DependInfo.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/build.make` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/build.make`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/flags.make` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/flags.make`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/ggml.c.o` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/ggml.c.o`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/ggml.c.o.d` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeFiles/ggml.dir/ggml.c.o.d`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/CMakeLists.txt` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/Makefile` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/Makefile`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/cmake_install.cmake` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/cmake_install.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/ggml-cuda.cu` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/ggml-cuda.cu`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/ggml-cuda.h` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/ggml-cuda.h`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/ggml-opencl.c` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/ggml-opencl.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/ggml-opencl.h` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/ggml-opencl.h`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/ggml.c` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/ggml.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/src/libggml.a` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/src/libggml.a`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/CMakeLists.txt` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-blas0.c` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-blas0.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-grad0.c` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-grad0.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-mul-mat0.c` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-mul-mat0.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-mul-mat1.c` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-mul-mat1.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-mul-mat2.c` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-mul-mat2.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-svd0.c` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-svd0.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-vec0.c` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-vec0.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-vec1.c` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-vec1.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test-vec2.c` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test-vec2.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test0.c` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test0.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test1.c` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test1.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test2.c` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test2.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/ggml/tests/test3.c` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/ggml/tests/test3.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/librwkv.so` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/librwkv.so`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/20B_tokenizer.json` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/20B_tokenizer.json`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/__pycache__/rwkv_cpp_model.cpython-310.pyc` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/__pycache__/rwkv_cpp_model.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/__pycache__/rwkv_cpp_shared_library.cpython-310.pyc` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/__pycache__/rwkv_cpp_shared_library.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/chat_with_bot.py` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/chat_with_bot.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/convert_pytorch_to_ggml.py` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/convert_pytorch_to_ggml.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/convert_pytorch_to_ggml.test.py` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/convert_pytorch_to_ggml.test.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/generate_completions.py` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/generate_completions.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/measure_pexplexity.py` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/measure_pexplexity.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/merge_lora_into_ggml.py` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/merge_lora_into_ggml.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/Chinese-Chat.json` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/prompt/Chinese-Chat.json`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/English-Chat.json` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/prompt/English-Chat.json`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/English-QA.json` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/prompt/English-QA.json`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/Japanese-Chat.json` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/prompt/Japanese-Chat.json`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/prompt/Japanese-QA.json` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/prompt/Japanese-QA.json`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/quantize.py` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/quantize.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/rwkv_cpp_model.py` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/rwkv_cpp_model.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/rwkv_cpp_shared_library.py` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/rwkv_cpp_shared_library.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv/sampling.py` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv/sampling.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv.cpp` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv.cpp`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/rwkv.h` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/rwkv.h`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/CMakeDirectoryInformation.cmake` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/CMakeDirectoryInformation.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/DependInfo.cmake` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/DependInfo.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/build.make` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/build.make`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/flags.make` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/flags.make`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/test_ggml_basics.c.o` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/test_ggml_basics.c.o`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/test_ggml_basics.c.o.d` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_ggml_basics.dir/test_ggml_basics.c.o.d`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/DependInfo.cmake` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/DependInfo.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/build.make` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/build.make`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/flags.make` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/flags.make`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/test_tiny_rwkv.c.o` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/test_tiny_rwkv.c.o`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/test_tiny_rwkv.c.o.d` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeFiles/test_tiny_rwkv.dir/test_tiny_rwkv.c.o.d`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CMakeLists.txt` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/CTestTestfile.cmake` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/CTestTestfile.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/Makefile` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/Makefile`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/cmake_install.cmake` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/cmake_install.cmake`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/expected_logits.bin` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/expected_logits.bin`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/test_ggml_basics.c` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/test_ggml_basics.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/test_tiny_rwkv.c` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/test_tiny_rwkv.c`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/tiny-rwkv-660K-FP16.bin` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/tiny-rwkv-660K-FP16.bin`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/extern/rwkv.cpp/tests/tiny-rwkv-660K-FP32.bin` & `langdash-0.0.3.dev1/langdash/extern/rwkv.cpp/tests/tiny-rwkv-660K-FP32.bin`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/llm.py` & `langdash-0.0.3.dev1/langdash/llm.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 class LLM(Generic[T_LLMSession]):
   """
   A language model class for inference.
   """
   Session: Type[T_LLMSession]
   
   def session(self, *args, **kwargs) -> T_LLMSession:
-     """
+    """
     Create a new session for the given model.
     
     Args:
       default_infer_args (dict):
         Default arguments for the default inference engine.
       track_called_chains (bool):
         Whether to track called chains.
@@ -30,15 +30,15 @@
       global_args (dict):
         Global arguments for the session.
 
     Returns:
       A new session object.
     """
     return self.__class__.Session(llm=self, *args, **kwargs)
-  
+
   def get_capability(self) -> LLMCapability:
     """
     Returns the capability of the language model.
     """
     return LLMCapability.Generative
 
 class EmbeddingLLM(LLM):
```

### Comparing `langdash-0.0.2.dev2/langdash/llm_session.py` & `langdash-0.0.3.dev1/langdash/llm_session.py`

 * *Files 7% similar despite different names*

```diff
@@ -94,15 +94,18 @@
       add_special_tokens: Whether to add special tokens to the output.
 
     Returns:
       The list of tokens.
     """
     raise NotImplementedError("tokenize")
   
-  def next_token_probs(self) -> Sequence[float]:
+  def decode(self, tokids: List[int]) -> str:
+    raise NotImplementedError("decode")
+  
+  def next_token_probs(self) -> List[float]:
     """
     Returns the probabilities for next token.
     """
     raise NotImplementedError("next_token_probs")
   
   def _infer(self,
             end: Optional[Union[str, int]],
@@ -122,65 +125,82 @@
     Returns:
       Inference response
     """
     if not args:
       args = self.default_infer_args
     yield from self._infer(end, args)
     
-  def inject(self, text: str, add_special_tokens: bool = False) -> int:
+  def inject(self, text: Union[str, int], add_special_tokens: bool = False) -> int:
     raise NotImplementedError("inject")
 
 T_Logits = TypeVar('T_Logits')
 
 class LLMGenerationSessionForRawText(LLMGenerationSession, Generic[T_LLM, T_LLMState, T_Logits]):
   _logits: Optional[T_Logits]
   _next_token: Optional[Tuple[int, str]]
   
   def _eval(self, tokid: int) -> T_Logits:
     raise NotImplementedError("_eval")
   
-  def _token_to_str(self, tokid: int) -> str:
-    raise NotImplementedError("_token_to_str")
-  
-  def _heal_token(self, tok_a: int, tok_b: int) -> str:
-    return self._token_to_str(tok_a) + self._token_to_str(tok_b)
+  def _next_token_probs(self):
+    raise NotImplementedError("_next_token_probs")
   
-  def inject(self, text: str, add_special_tokens: bool = False) -> int:
-    input_ids = self.tokenize(text, add_special_tokens=add_special_tokens)
+  def flush_token(self):
+    """
+    Flushes the previous token into the language model if healing is enabled.
+    
+    **Warning:** unexpected behavior if the previous token is a "boundary" token
+    like spaces.
+    """
+    if self._next_token is None:
+      return
+    self.inject(self._next_token[0])
+    self._next_token = None
+  
+  def next_token_probs(self, *args, **kwargs) -> List[float]:
+    assert self._next_token is None, "token healing must be disabled or flush_token() must be called"
+    probs = self._next_token_probs(*args, **kwargs)
+    return list(map(float, probs))
+  
+  def inject(self, text: Union[str, int], add_special_tokens: bool = False) -> int:
+    if isinstance(text, str):
+      input_ids = self.tokenize(text, add_special_tokens=add_special_tokens)
+    else:
+      input_ids = [text]
     if not input_ids:
       return 0
     
     num_toks = 0
       
     if self.token_healing:
       init_offset = 0
       if self._next_token is not None:
         tokid, tokstr = self._next_token
-        healed_str = self._heal_token(tokid, input_ids[0])
+        healed_str = self.decode([tokid, input_ids[0]])
         healed_tokens = self.tokenize(healed_str, add_special_tokens=add_special_tokens)
         
         if len(input_ids) == 1:
           if len(healed_tokens) == 1:
             self._next_token = (healed_tokens[0], healed_str)
             return 1
           else:
             # handle rare case where 1 input token maps to 2 or more "healed" tokens
             for tokid in healed_tokens[:-1]:
               self._logits = self._eval(tokid)
-            self._next_token = (healed_tokens[-1], self._token_to_str(healed_tokens[-1]))
+            self._next_token = (healed_tokens[-1], self.decode(healed_tokens[-1:]))
             return len(healed_tokens) - 1
         else:
           for tokid in healed_tokens:
             self._logits = self._eval(tokid)
           init_offset = 1
         
       for tokid in input_ids[init_offset:-1]:
         self._logits = self._eval(tokid)
       num_toks += len(input_ids) - init_offset - 1
-      self._next_token = (input_ids[-1], self._token_to_str(input_ids[-1]))
+      self._next_token = (input_ids[-1], self.decode(input_ids[-1:]))
     else:
       if self._next_token is not None:
         tokid, tokstr = self._next_token
         self._eval(tokid)
         num_toks += 1
       for tokid in input_ids:
         self._logits = self._eval(tokid)
@@ -202,13 +222,15 @@
     Returns the embedding size of the model.
     """
     raise NotImplementedError("embedding_size")
     
   def infer(self, text: str) -> T_Embedding:
     """
     Infer the embedding of a text.
+    
     Args:
       text: The text to be embedded.
+      
     Returns:
-      The embedding of the text.
+      The embedding vector of the text.
     """
     raise NotImplementedError("infer")
```

### Comparing `langdash-0.0.2.dev2/langdash/models/mock.py` & `langdash-0.0.3.dev1/langdash/models/mock.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/models/rwkvcpp.py` & `langdash-0.0.3.dev1/langdash/models/rwkvcpp.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,17 +105,14 @@
     self._logits, self._state = None, None
     self._next_token = None
   
   def _eval(self, tokid: int) -> torch.Tensor:
     self._logits, self._state = self._rwkv.eval(tokid, self._state)
     return self._logits
   
-  def _token_to_str(self, tokid: int) -> str:
-    return self._tokenizer.id_to_token(tokid)
-  
   def set_state(self, state: Optional[RWKVCppState]):
     if state is None:
       self._logits, self._state = None, None
       self._next_token = None
     else:
       self._logits = copy.deepcopy(state._logits)
       self._state = copy.deepcopy(state._state)
@@ -127,15 +124,18 @@
       _state = copy.deepcopy(self._state),
       _next_token = self._next_token,
     )
 
   def tokenize(self, text: str, add_special_tokens: bool = False) -> List[int]:
     return self._tokenizer.encode(text, add_special_tokens=add_special_tokens).ids
   
-  def next_token_probs(self) -> torch.Tensor:
+  def decode(self, tokids: List[int]) -> str:
+    return self._tokenizer.decode(tokids)
+  
+  def _next_token_probs(self) -> torch.Tensor:
     if self._next_token is None:
       if self._logits is None:
         raise ValueError("cannot predict next probability for empty input")
       logits = self._logits
     else:
       logits, _ = self._rwkv.eval(self._next_token[0], self._state)
     return torch.nn.functional.softmax(logits, dim=-1)
```

### Comparing `langdash-0.0.2.dev2/langdash/models/sentence_transformers.py` & `langdash-0.0.3.dev1/langdash/models/sentence_transformers.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/models/transformers.py` & `langdash-0.0.3.dev1/langdash/models/transformers.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,18 +29,18 @@
       tokenizer = transformers.AutoTokenizer.from_pretrained(llm._tokenizer_name)
       return model, tokenizer
       
     self._model, self._tokenizer = self._ld.get_model_internal(self.llm, load_model)
     
     if isinstance(
       self._tokenizer,
-      Union[
+      (
         transformers.GPT2Tokenizer,
         transformers.GPT2TokenizerFast
-      ]
+      )
     ):
       self._space_token = "\u0120"
       self._buffered_token_head = set(
         v for k, v in self._tokenizer.get_vocab().items() if "\u0122" in k
       )
     else:
       self._space_token = " "
@@ -75,21 +75,21 @@
       torch.IntTensor([tokid]),
       past_key_values=self._past_key_values,
       use_cache=True
     )
     self._past_key_values = outputs.past_key_values
     return outputs.logits[-1]
   
-  def _token_to_str(self, tokid: int) -> str:
-    return self._tokenizer.convert_ids_to_tokens(tokid)
+  def decode(self, tokids: List[int]) -> str:
+    return self._tokenizer.decode(tokids)
   
   def tokenize(self, text: str, add_special_tokens: bool = False) -> List[int]:
-    return list(self._tokenizer.encode(text, add_special_tokens=add_special_tokens))
+    return self._tokenizer.encode(text, add_special_tokens=add_special_tokens).tolist()
   
-  def next_token_probs(self) -> torch.Tensor:
+  def _next_token_probs(self) -> torch.Tensor:
     if self._next_token is None:
       if self._logits is None:
         raise ValueError("cannot predict next probability for empty input")
       logits = self._logits
     else:
       logits = self._model.forward(
         torch.IntTensor([self._next_token[0]]),
```

### Comparing `langdash-0.0.2.dev2/langdash/sampling.py` & `langdash-0.0.3.dev1/langdash/sampling.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,12 +56,12 @@
     probs = sample_top_p(logits, args.top_p)
   
   # apply temperature
   if args.temperature != 0.0:
     probs = probs.pow(1.0 / args.temperature)
     
   return probs
-  
+
 def sample(*args, **kwargs) -> int:
   probs = output_probs(*args, **kwargs)
   return int(torch.multinomial(probs, num_samples=1)[0])
```

### Comparing `langdash-0.0.2.dev2/langdash/search/embedding_search.py` & `langdash-0.0.3.dev1/langdash/search/embedding_search.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash/search/multichoice_search.py` & `langdash-0.0.3.dev1/langdash/search/multichoice_search.py`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/langdash.egg-info/PKG-INFO` & `langdash-0.0.3.dev1/langdash.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langdash
-Version: 0.0.2.dev2
+Version: 0.0.3.dev1
 Summary: A simple library for interfacing with language models.
 Home-page: https://git.mysymphony.jp.net/nana/langdash
 Author: Nana Mochizuki
 Author-email: nana@mysymphony.jp.net
 Project-URL: Source, https://git.mysymphony.jp.net/nana/langdash
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `langdash-0.0.2.dev2/langdash.egg-info/SOURCES.txt` & `langdash-0.0.3.dev1/langdash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langdash-0.0.2.dev2/setup.py` & `langdash-0.0.3.dev1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='langdash',
-    version='0.0.2.dev2',
+    version='0.0.3.dev1',
     description='A simple library for interfacing with language models.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Nana Mochizuki',
     author_email='nana@mysymphony.jp.net',
     url='https://git.mysymphony.jp.net/nana/langdash',
     classifiers=[
```

