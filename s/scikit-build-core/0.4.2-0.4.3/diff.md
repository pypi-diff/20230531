# Comparing `tmp/scikit_build_core-0.4.2.tar.gz` & `tmp/scikit_build_core-0.4.3.tar.gz`

## Comparing `scikit_build_core-0.4.2.tar` & `scikit_build_core-0.4.3.tar`

### file list

```diff
@@ -1,237 +1,237 @@
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/.git_archival.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/.gitattributes
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/.packit.yaml
--rw-r--r--   0        0        0     3313 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/.readthedocs.yml
--rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/noxfile.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/.distro/packit.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/.distro/python-scikit-build-core.rpmlintrc
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/.distro/python-scikit-build-core.spec
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/.distro/.fmf/version
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/.distro/plans/main.fmf.dist-git
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/.distro/plans/rpmlint.fmf
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/.distro/plans/smoke.fmf
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/.distro/tests/rpmlint.fmf
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/.distro/tests/smoke.fmf
--rw-r--r--   0        0        0     9536 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/.github/codecov.yml
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/.github/matchers/pylint.json
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/.github/workflows/cd.yml
--rw-r--r--   0        0        0     6827 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0    14714 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/docs/changelog.md
--rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/docs/cmakelists.md
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/docs/conf.py
--rw-r--r--   0        0        0    12487 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/docs/configuration.md
--rw-r--r--   0        0        0     9062 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/docs/getting_started.md
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/docs/index.md
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/docs/api/scikit_build_core.build.rst
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/docs/api/scikit_build_core.builder.rst
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/docs/api/scikit_build_core.file_api.model.rst
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/docs/api/scikit_build_core.file_api.rst
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/docs/api/scikit_build_core.metadata.rst
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/docs/api/scikit_build_core.resources.find_python.rst
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/docs/api/scikit_build_core.resources.rst
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/docs/api/scikit_build_core.rst
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/docs/api/scikit_build_core.settings.rst
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/docs/api/scikit_build_core.setuptools.rst
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/docs/examples/getting_started/test.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/docs/examples/getting_started/abi3/CMakeLists.txt
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/docs/examples/getting_started/abi3/example.c
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/docs/examples/getting_started/abi3/pyproject.toml
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/docs/examples/getting_started/c/CMakeLists.txt
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/docs/examples/getting_started/c/example.c
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/docs/examples/getting_started/c/pyproject.toml
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/docs/examples/getting_started/cython/CMakeLists.txt
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/docs/examples/getting_started/cython/example.pyx
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/docs/examples/getting_started/cython/pyproject.toml
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/docs/examples/getting_started/fortran/CMakeLists.txt
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/docs/examples/getting_started/fortran/example.f
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/docs/examples/getting_started/fortran/pyproject.toml
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/docs/examples/getting_started/pybind11/CMakeLists.txt
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/docs/examples/getting_started/pybind11/example.cpp
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/docs/examples/getting_started/pybind11/pyproject.toml
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/docs/examples/getting_started/swig/CMakeLists.txt
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/docs/examples/getting_started/swig/example.c
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/docs/examples/getting_started/swig/example.i
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/docs/examples/getting_started/swig/pyproject.toml
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/__init__.py
--rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/_logging.py
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/_shutil.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/_version.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/_version.pyi
--rw-r--r--   0        0        0     8594 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/cmake.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/errors.py
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/program_search.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/py.typed
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/_compat/__init__.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/_compat/builtins.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/_compat/tomllib.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/_compat/typing.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/_compat/importlib/__init__.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/_compat/importlib/metadata.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/_compat/importlib/resources.py
--rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/build/__init__.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/build/_file_processor.py
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/build/_init.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/build/_pathutil.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/build/_scripts.py
--rw-r--r--   0        0        0     7806 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/build/_wheelfile.py
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/build/sdist.py
--rw-r--r--   0        0        0     9832 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/build/wheel.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/builder/__init__.py
--rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/builder/builder.py
--rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/builder/generator.py
--rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/builder/get_requires.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/builder/macos.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/builder/sysconfig.py
--rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/builder/wheel_tag.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/file_api/__init__.py
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/file_api/_cattrs_converter.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/file_api/query.py
--rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/file_api/reply.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/file_api/model/__init__.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/file_api/model/cache.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/file_api/model/cmakefiles.py
--rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/file_api/model/codemodel.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/file_api/model/common.py
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/file_api/model/directory.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/file_api/model/index.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/file_api/model/toolchains.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/metadata/__init__.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/metadata/fancy_pypi_readme.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/metadata/setuptools_scm.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/resources/__init__.py
--rw-r--r--   0        0        0     3773 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/resources/_editable_redirect.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/resources/known_wheels.toml
--rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/resources/find_python/Copyright.txt
--rw-r--r--   0        0        0    23174 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake
--rw-r--r--   0        0        0    22536 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/resources/find_python/FindPython.cmake
--rw-r--r--   0        0        0    19036 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/resources/find_python/FindPython3.cmake
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/resources/find_python/__init__.py
--rw-r--r--   0        0        0   198528 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/resources/find_python/FindPython/Support.cmake
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/settings/__init__.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/settings/_load_provider.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/settings/metadata.py
--rw-r--r--   0        0        0     5642 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/settings/skbuild_model.py
--rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/settings/skbuild_read_settings.py
--rw-r--r--   0        0        0    16489 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/settings/sources.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/setuptools/__init__.py
--rw-r--r--   0        0        0     7759 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/setuptools/build_cmake.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/setuptools/build_meta.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/src/scikit_build_core/setuptools/wrapper.py
--rw-r--r--   0        0        0     9343 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/conftest.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/constraints.txt
--rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/test_builder.py
--rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/test_cmake_config.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/test_custom_modules.py
--rw-r--r--   0        0        0     8426 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/test_dynamic_metadata.py
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/test_fileapi.py
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/test_fortran.py
--rw-r--r--   0        0        0    15811 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/test_generator_default.py
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/test_get_requires.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/test_logging.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/test_module_dir.py
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/test_name_main.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/test_prepare_metadata.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/test_process_scripts.py
--rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/test_program_search.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/test_pyproject_abi3.py
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/test_pyproject_extra_dirs.py
--rw-r--r--   0        0        0     8248 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/test_pyproject_pep517.py
--rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/test_pyproject_pep518.py
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/test_pyproject_pep660.py
--rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/test_settings.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/test_setuptools_abi3.py
--rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/test_setuptools_pep517.py
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/test_setuptools_pep518.py
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/test_simple_pure.py
--rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/test_simplest_c.py
--rw-r--r--   0        0        0    12743 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/test_skbuild_settings.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/test_wheelfile_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/api/simple_pure/.cmake/api/v1/query/cache-v2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/api/simple_pure/.cmake/api/v1/query/cmakeFiles-v1
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/api/simple_pure/.cmake/api/v1/query/codemodel-v2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/api/simple_pure/.cmake/api/v1/query/toolchains-v1
--rw-r--r--   0        0        0    20671 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json
--rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/abi3_pyproject_ext/CMakeLists.txt
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/abi3_pyproject_ext/abi3_example.c
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/abi3_pyproject_ext/pyproject.toml
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/abi3_setuptools_ext/CMakeLists.txt
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/abi3_setuptools_ext/abi3_example.c
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/abi3_setuptools_ext/pyproject.toml
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/abi3_setuptools_ext/setup.cfg
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/abi3_setuptools_ext/setup.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/custom_cmake/CMakeLists.txt
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/custom_cmake/pyproject.toml
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/custom_cmake/extern/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/__init__.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/ExampleInclude.cmake
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/__init__.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/ExamplePkgConfig.cmake
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/__init__.py
--rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/custom_cmake/scripts/script1
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/dynamic_metadata/CMakeLists.txt
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/dynamic_metadata/dual_project.toml
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/dynamic_metadata/faulty_dual_project.toml
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/dynamic_metadata/faulty_project.toml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/dynamic_metadata/local_pyproject.toml
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/dynamic_metadata/plugin_project.toml
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/dynamic_metadata/pyproject.toml
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/dynamic_metadata/warn_project.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/dynamic_metadata/plugins/local/version/__init__.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/dynamic_metadata/plugins/local/version/nested/__init__.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/dynamic_metadata/src/module.c
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/dynamic_metadata/src/dynamic/__init__.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/filepath_pure/CMakeLists.txt
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/filepath_pure/pyproject.toml
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/fortran_example/CMakeLists.txt
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/fortran_example/fib1.f
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/fortran_example/pyproject.toml
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/mixed_setuptools/CMakeLists.txt
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/mixed_setuptools/pyproject.toml
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/mixed_setuptools/setup.cfg
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/mixed_setuptools/setup.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/mixed_setuptools/src/main.cpp
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/mixed_setuptools/src/mixed_setuptools/__init__.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/mixed_setuptools/src/mixed_setuptools/_core.pyi
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/simple_pure/CMakeLists.txt
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/simple_pure/simple_pure.cpp
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/simple_pyproject_ext/CMakeLists.txt
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/simple_pyproject_ext/LICENSE
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/simple_pyproject_ext/pyproject.toml
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/simple_pyproject_ext/src/main.cpp
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/simple_pyproject_source_dir/LICENSE
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/simple_pyproject_source_dir/pyproject.toml
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/simple_pyproject_source_dir/src/CMakeLists.txt
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/simple_pyproject_source_dir/src/main.cpp
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/simple_setuptools_ext/CMakeLists.txt
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/simple_setuptools_ext/LICENSE
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/simple_setuptools_ext/pyproject.toml
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/simple_setuptools_ext/setup.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/simple_setuptools_ext/src/main.cpp
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/simplest_c/.gitignore
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/simplest_c/CMakeLists.txt
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/simplest_c/pyproject.toml
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/simplest_c/src/module.c
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/simplest_c/src/not_a_package/simple.txt
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/simplest_c/src/simplest/__init__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/simplest_c/src/simplest/_module.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/simplest_c/src/simplest/artifact_ignored.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/simplest_c/src/simplest/data.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/simplest_c/src/simplest/excluded.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/simplest_c/src/simplest/ignored.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/simplest_c/src/simplest/ignored_included.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/tests/packages/simplest_c/src/simplest/sdist_only.txt
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/.gitignore
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/LICENSE
--rw-r--r--   0        0        0     9702 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/README.md
--rw-r--r--   0        0        0     8424 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/pyproject.toml
--rw-r--r--   0        0        0    12650 2020-02-02 00:00:00.000000 scikit_build_core-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.git_archival.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.gitattributes
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.packit.yaml
+-rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.readthedocs.yml
+-rw-r--r--   0        0        0     5786 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/noxfile.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.distro/packit.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.distro/python-scikit-build-core.rpmlintrc
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.distro/python-scikit-build-core.spec
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.distro/.fmf/version
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.distro/plans/main.fmf.dist-git
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.distro/plans/rpmlint.fmf
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.distro/plans/smoke.fmf
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.distro/tests/rpmlint.fmf
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.distro/tests/smoke.fmf
+-rw-r--r--   0        0        0     9969 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.github/codecov.yml
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     6827 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0    15372 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/changelog.md
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/cmakelists.md
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/conf.py
+-rw-r--r--   0        0        0    12730 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/configuration.md
+-rw-r--r--   0        0        0     9062 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/getting_started.md
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/index.md
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/api/scikit_build_core.build.rst
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/api/scikit_build_core.builder.rst
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/api/scikit_build_core.file_api.model.rst
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/api/scikit_build_core.file_api.rst
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/api/scikit_build_core.metadata.rst
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/api/scikit_build_core.resources.find_python.rst
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/api/scikit_build_core.resources.rst
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/api/scikit_build_core.rst
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/api/scikit_build_core.settings.rst
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/api/scikit_build_core.setuptools.rst
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/examples/getting_started/test.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/examples/getting_started/abi3/CMakeLists.txt
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/examples/getting_started/abi3/example.c
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/examples/getting_started/abi3/pyproject.toml
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/examples/getting_started/c/CMakeLists.txt
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/examples/getting_started/c/example.c
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/examples/getting_started/c/pyproject.toml
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/examples/getting_started/cython/CMakeLists.txt
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/examples/getting_started/cython/example.pyx
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/examples/getting_started/cython/pyproject.toml
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/examples/getting_started/fortran/CMakeLists.txt
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/examples/getting_started/fortran/example.f
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/examples/getting_started/fortran/pyproject.toml
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/examples/getting_started/pybind11/CMakeLists.txt
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/examples/getting_started/pybind11/example.cpp
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/examples/getting_started/pybind11/pyproject.toml
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/examples/getting_started/swig/CMakeLists.txt
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/examples/getting_started/swig/example.c
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/examples/getting_started/swig/example.i
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/docs/examples/getting_started/swig/pyproject.toml
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/__init__.py
+-rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/_logging.py
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/_shutil.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/_version.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/_version.pyi
+-rw-r--r--   0        0        0     8594 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/cmake.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/errors.py
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/program_search.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/py.typed
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/_compat/__init__.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/_compat/builtins.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/_compat/tomllib.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/_compat/typing.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/_compat/importlib/__init__.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/_compat/importlib/metadata.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/_compat/importlib/resources.py
+-rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/build/__init__.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/build/_file_processor.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/build/_init.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/build/_pathutil.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/build/_scripts.py
+-rw-r--r--   0        0        0     8169 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/build/_wheelfile.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/build/sdist.py
+-rw-r--r--   0        0        0     9882 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/build/wheel.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/builder/__init__.py
+-rw-r--r--   0        0        0     7574 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/builder/builder.py
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/builder/generator.py
+-rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/builder/get_requires.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/builder/macos.py
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/builder/sysconfig.py
+-rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/builder/wheel_tag.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/file_api/__init__.py
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/file_api/_cattrs_converter.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/file_api/query.py
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/file_api/reply.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/file_api/model/__init__.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/file_api/model/cache.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/file_api/model/cmakefiles.py
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/file_api/model/codemodel.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/file_api/model/common.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/file_api/model/directory.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/file_api/model/index.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/file_api/model/toolchains.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/metadata/__init__.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/metadata/fancy_pypi_readme.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/metadata/setuptools_scm.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/resources/__init__.py
+-rw-r--r--   0        0        0     3773 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/resources/_editable_redirect.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/resources/known_wheels.toml
+-rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/resources/find_python/Copyright.txt
+-rw-r--r--   0        0        0    23174 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake
+-rw-r--r--   0        0        0    22536 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/resources/find_python/FindPython.cmake
+-rw-r--r--   0        0        0    19036 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/resources/find_python/FindPython3.cmake
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/resources/find_python/__init__.py
+-rw-r--r--   0        0        0   198528 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/resources/find_python/FindPython/Support.cmake
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/settings/__init__.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/settings/_load_provider.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/settings/metadata.py
+-rw-r--r--   0        0        0     5642 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/settings/skbuild_model.py
+-rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/settings/skbuild_read_settings.py
+-rw-r--r--   0        0        0    18214 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/settings/sources.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/setuptools/__init__.py
+-rw-r--r--   0        0        0     7759 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/setuptools/build_cmake.py
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/setuptools/build_meta.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/src/scikit_build_core/setuptools/wrapper.py
+-rw-r--r--   0        0        0     9343 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/conftest.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/constraints.txt
+-rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_builder.py
+-rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_cmake_config.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_custom_modules.py
+-rw-r--r--   0        0        0     8426 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_dynamic_metadata.py
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_fileapi.py
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_fortran.py
+-rw-r--r--   0        0        0    15811 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_generator_default.py
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_get_requires.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_logging.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_module_dir.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_name_main.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_prepare_metadata.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_process_scripts.py
+-rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_program_search.py
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_pyproject_abi3.py
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_pyproject_extra_dirs.py
+-rw-r--r--   0        0        0     8248 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_pyproject_pep517.py
+-rw-r--r--   0        0        0     4572 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_pyproject_pep518.py
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_pyproject_pep660.py
+-rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_settings.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_setuptools_abi3.py
+-rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_setuptools_pep517.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_setuptools_pep518.py
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_simple_pure.py
+-rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_simplest_c.py
+-rw-r--r--   0        0        0    12743 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_skbuild_settings.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/test_wheelfile_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/api/simple_pure/.cmake/api/v1/query/cache-v2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/api/simple_pure/.cmake/api/v1/query/cmakeFiles-v1
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/api/simple_pure/.cmake/api/v1/query/codemodel-v2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/api/simple_pure/.cmake/api/v1/query/toolchains-v1
+-rw-r--r--   0        0        0    20671 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json
+-rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/abi3_pyproject_ext/CMakeLists.txt
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/abi3_pyproject_ext/abi3_example.c
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/abi3_pyproject_ext/pyproject.toml
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/abi3_setuptools_ext/CMakeLists.txt
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/abi3_setuptools_ext/abi3_example.c
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/abi3_setuptools_ext/pyproject.toml
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/abi3_setuptools_ext/setup.cfg
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/abi3_setuptools_ext/setup.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/custom_cmake/CMakeLists.txt
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/custom_cmake/pyproject.toml
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/custom_cmake/extern/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/__init__.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/ExampleInclude.cmake
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/__init__.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/ExamplePkgConfig.cmake
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/__init__.py
+-rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/custom_cmake/scripts/script1
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/dynamic_metadata/CMakeLists.txt
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/dynamic_metadata/dual_project.toml
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/dynamic_metadata/faulty_dual_project.toml
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/dynamic_metadata/faulty_project.toml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/dynamic_metadata/local_pyproject.toml
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/dynamic_metadata/plugin_project.toml
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/dynamic_metadata/pyproject.toml
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/dynamic_metadata/warn_project.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/dynamic_metadata/plugins/local/version/__init__.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/dynamic_metadata/plugins/local/version/nested/__init__.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/dynamic_metadata/src/module.c
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/dynamic_metadata/src/dynamic/__init__.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/filepath_pure/CMakeLists.txt
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/filepath_pure/pyproject.toml
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/fortran_example/CMakeLists.txt
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/fortran_example/fib1.f
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/fortran_example/pyproject.toml
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/mixed_setuptools/CMakeLists.txt
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/mixed_setuptools/pyproject.toml
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/mixed_setuptools/setup.cfg
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/mixed_setuptools/setup.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/mixed_setuptools/src/main.cpp
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/mixed_setuptools/src/mixed_setuptools/__init__.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/mixed_setuptools/src/mixed_setuptools/_core.pyi
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simple_pure/CMakeLists.txt
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simple_pure/simple_pure.cpp
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simple_pyproject_ext/CMakeLists.txt
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simple_pyproject_ext/LICENSE
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simple_pyproject_ext/pyproject.toml
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simple_pyproject_ext/src/main.cpp
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simple_pyproject_source_dir/LICENSE
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simple_pyproject_source_dir/pyproject.toml
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simple_pyproject_source_dir/src/CMakeLists.txt
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simple_pyproject_source_dir/src/main.cpp
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simple_setuptools_ext/CMakeLists.txt
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simple_setuptools_ext/LICENSE
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simple_setuptools_ext/pyproject.toml
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simple_setuptools_ext/setup.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simple_setuptools_ext/src/main.cpp
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simplest_c/.gitignore
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simplest_c/CMakeLists.txt
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simplest_c/pyproject.toml
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simplest_c/src/module.c
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simplest_c/src/not_a_package/simple.txt
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simplest_c/src/simplest/__init__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simplest_c/src/simplest/_module.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simplest_c/src/simplest/artifact_ignored.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simplest_c/src/simplest/data.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simplest_c/src/simplest/excluded.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simplest_c/src/simplest/ignored.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simplest_c/src/simplest/ignored_included.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/tests/packages/simplest_c/src/simplest/sdist_only.txt
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/.gitignore
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/LICENSE
+-rw-r--r--   0        0        0    10748 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/README.md
+-rw-r--r--   0        0        0     8587 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0    13747 2020-02-02 00:00:00.000000 scikit_build_core-0.4.3/PKG-INFO
```

### Comparing `scikit_build_core-0.4.2/.packit.yaml` & `scikit_build_core-0.4.3/.packit.yaml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/.pre-commit-config.yaml` & `scikit_build_core-0.4.3/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, scss, javascript, json]
         args: [--prose-wrap=always]
         exclude: "^tests"
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.267
+    rev: v0.0.270
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.3.0
     hooks:
@@ -82,15 +82,15 @@
           - ninja
           - packaging
           - pyproject_metadata
           - pytest
           - rich
           - setuptools-scm
           - tomli
-          - types-setuptools>=67.6.0.5
+          - types-setuptools>=67.8
 
   - repo: https://github.com/henryiii/check-sdist
     rev: "v0.1.2"
     hooks:
       - id: check-sdist
         args: [--inject-junk]
         additional_dependencies:
```

### Comparing `scikit_build_core-0.4.2/noxfile.py` & `scikit_build_core-0.4.3/noxfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,17 @@
         extra.append("cmake")
     if shutil.which("ninja") is None:
         extra.append("ninja")
     if (3, 8) <= sys.version_info < (3, 12):
         extra.append("numpy")
 
     install_arg = "-e.[test,cov]" if "--cov" in posargs else "-e.[test]"
+    if "--cov" in posargs:
+        posargs.append("--cov-config=pyproject.toml")
+
     session.install(install_arg, *extra, *install_args)
     session.run("pytest", *run_args, *posargs, env=env)
 
 
 @nox.session
 def tests(session: nox.Session) -> None:
     """
@@ -147,15 +150,15 @@
     # (requires tomli, so allowing access to system-site-packages)
 
     if sys.version_info < (3, 11):
         import tomli as tomllib
     else:
         import tomllib
 
-    parser = argparse.ArgumentParser()
+    parser = argparse.ArgumentParser(prog=f"{Path(sys.argv[0]).name} -s downstream")
     parser.add_argument("project", help="A project to build")
     parser.add_argument("--subdir", help="A subdirectory to build")
     args, remaining = parser.parse_known_args(session.posargs)
 
     tmp_dir = Path(session.create_tmp())
     proj_dir = tmp_dir / "_".join(args.project.split("/"))
```

### Comparing `scikit_build_core-0.4.2/.distro/python-scikit-build-core.spec` & `scikit_build_core-0.4.3/.distro/python-scikit-build-core.spec`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/.github/CONTRIBUTING.md` & `scikit_build_core-0.4.3/.github/CONTRIBUTING.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+# Testing a project with a branch / main
+
+If you are testing a downstream project, you can use a branch of
+scikit-build-core like this:
+
+```toml
+[build-system]
+requires = ["scikit-build-core @ git+https://github.com/scikit-build/scikit-build-core@main"]
+build-backend = "scikit_build_core.build"
+```
+
+Or you can build your project from the scikit-build-core source with nox:
+
+```bash
+nox -s downstream -- https://github.com/...
+```
+
 # Setting up for development
 
 See the [Scikit-HEP Developer introduction][skhep-dev-intro] for a detailed
 description of best practices for developing packages.
 
 [skhep-dev-intro]: https://scikit-hep.org/developer/intro
```

### Comparing `scikit_build_core-0.4.2/.github/matchers/pylint.json` & `scikit_build_core-0.4.3/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/.github/workflows/cd.yml` & `scikit_build_core-0.4.3/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/.github/workflows/ci.yml` & `scikit_build_core-0.4.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/docs/changelog.md` & `scikit_build_core-0.4.3/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,28 @@
 # Changelog
 
+## Version 0.4.3
+
+This adds support for CPython 3.12.0b1, and improves Stable ABI / Limited API
+support (supported by an upcoming nanobind for Python 3.12). An editable install
+fix allows running from any directory.
+
+Fixes:
+
+- Allow CMake to detect if limited API is targeted by @henryiii in #333 and #342
+- Make abi3 support conditional on Python version by @henryiii in #344
+- Windows path correction for 3.12.0b1 by @henryiii in #346
+- Editable path needs to be absolute by @henryiii in #345
+
+Other:
+
+- Add 3.12.0b1 by @henryiii in #341
+- Refactor settings by @henryiii in #338
+- Document that `CMAKE_ARGS` supports space separators by @henryiii in #339
+
 ## Version 0.4.2
 
 This is a quick followup to LICENSE file handing to closer match the current
 draft of [PEP 639](https://peps.python.org/pep-0639). It also removes the
 automatic optional Rich logging, which doesn't work well with Pip's subprocess
 piping, being cropped to a very narrow width regardless of terminal size.
```

### Comparing `scikit_build_core-0.4.2/docs/cmakelists.md` & `scikit_build_core-0.4.3/docs/cmakelists.md`

 * *Files 24% similar despite different names*

```diff
@@ -19,22 +19,28 @@
 
 You always want to find at least `Interpreter` and the "Module" component of the
 "Development" package. You do not want to find the entire "Development" package,
 as that include "Embed" component, which is not always present and is not
 related to making Python extension modules.
 
 If you are making a Limited ABI / Stable API package, you'll need the
-`Development.SABIModule` component instead.
+`Development.SABIModule` component instead. You can use the
+`SKBUILD_LIMITED_API` variable to check to see if it was requested.
+
+If you want to use the old, deprecated FindPythonInterp and FindPythonLibs
+instead, you can. Though it should be noted that FindPythonLibs requires a trick
+to make it work properly if a Python library is not preset (like in manylinux):
+you have to set `PYTHON_LIBRARY` to something (doesn't matter what) to make it
+succeed.
 
 ## Finding other packages
 
 Scikit-build-core includes the site-packages directory in CMake's search path,
 so packages can provide a find package config with a name matching the package
-name - such as the `pybind11` package. Later versions of scikit-build core will
-include a design for package to provide arbitrary CMake code.
+name - such as the `pybind11` package.
 
 Third party packages can declare entry-points `cmake.module` and `cmake.prefix`,
 and the specified module will be added to `CMAKE_PREFIX_PATH` and
 `CMAKE_MODULE_PATH`, respectively. Currently, the key is not used, but
 eventually there might be a way to request or exclude certain entry-points by
 key.
 
@@ -57,11 +63,26 @@
 - `${SKBUILD_HEADERS_DIR}`: The header directory. Anything in here gets
   installed to Python's header directory.
 - `${SKBUILD_SCRIPTS_DIR}`: The scripts directory. Anything placed in here will
   go to `bin` (Unix) or `Scripts` (Windows).
 - `${SKBUILD_NULL_DIR}`: Anything installed here will not be placed in the
   wheel.
 
+## Limited API / Stable ABI
+
+You can activate the limited ABI by setting When you do that,
+`${SKBUILD_SABI_COMPONENT}` will be set to `Development.SABIModule` if you can
+target this (new enough CPython), and will remain an empty string otherwise
+(PyPy). This allows the following idiom:
+
+```cmake
+find_package(Python REQUIRED COMPONENTS Interpreter Development.Module ${SKBUILD_SABI_COMPONENT})
+```
+
+This will add this only if scikit-build-core is driving the compilation and is
+targeting ABI3. If you want to support limited ABI from outside
+scikit-build-core, look into the `OPTIONAL_COMPONENTS` flag for `find_package`.
+
 ## Future additions
 
-Scikit-build-core does not include helpers for Fortran or Cython like
-scikit-build classic yet. These will be carefully reimagined soon.
+Scikit-build-core does not include helpers for F2Py or Cython like scikit-build
+classic yet. These will be carefully reimagined soon.
```

### Comparing `scikit_build_core-0.4.2/docs/conf.py` & `scikit_build_core-0.4.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/docs/configuration.md` & `scikit_build_core-0.4.3/docs/configuration.md`

 * *Files 2% similar despite different names*

```diff
@@ -194,14 +194,18 @@
 the wheel tags for the version you support:
 
 ```toml
 [tool.scikit-build]
 wheel.py-api = "cp37"
 ```
 
+Scikit-build-core will only target ABI3 if the version of Python is equal to or
+newer than the one you set. `${SKBUILD_SABI_COMPONENT}` is set to
+`Development.SABIModule` when targeting ABI3, and is an empty string otherwise.
+
 If you are not using CPython at all, you can specify any version of Python is
 fine:
 
 ```toml
 [tool.scikit-build]
 wheel.py.api = "py3"
 ```
@@ -322,16 +326,17 @@
 ```yaml
 SKBUILD_CMAKE_DEFINES: SOME_DEFINE=ON
 ```
 
 ````
 
 You can also manually specify the exact cmake args. Beyond the normal
-`SKBUILD_CMAKE_ARGS`, the `CMAKE_ARGS` environment variable is also supported
-(with some filtering for options scikit-build-core doesn't support overriding).
+`SKBUILD_CMAKE_ARGS`, the `CMAKE_ARGS` space-separated environment variable is
+also supported (with some filtering for options scikit-build-core doesn't
+support overriding).
 
 ````{tab} pyproject.toml
 
 ```toml
 [tool.scikit-build]
 cmake.args = ["-DSOME_DEFINE=ON", "-DOTHER=OFF"]
 ```
@@ -371,15 +376,15 @@
 
 `````
 
 ````{tab} Environment
 
 ```yaml
 SKBUILD_CMAKE_ARGS: -DSOME_DEFINE=ON;-DOTHER=OFF
-CMAKE_ARGS: -DSOME_DEFINE=ON;-DOTHER=OFF
+CMAKE_ARGS: -DSOME_DEFINE=ON -DOTHER=OFF
 ```
 
 ````
 
 ## Dynamic metadata
 
 Scikit-build-core 0.3.0 supports dynamic metadata with two built-in plugins.
```

### Comparing `scikit_build_core-0.4.2/docs/getting_started.md` & `scikit_build_core-0.4.3/docs/getting_started.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/docs/index.md` & `scikit_build_core-0.4.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/docs/api/scikit_build_core.build.rst` & `scikit_build_core-0.4.3/docs/api/scikit_build_core.build.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/docs/api/scikit_build_core.builder.rst` & `scikit_build_core-0.4.3/docs/api/scikit_build_core.builder.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/docs/api/scikit_build_core.file_api.model.rst` & `scikit_build_core-0.4.3/docs/api/scikit_build_core.file_api.model.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/docs/api/scikit_build_core.file_api.rst` & `scikit_build_core-0.4.3/docs/api/scikit_build_core.file_api.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/docs/api/scikit_build_core.metadata.rst` & `scikit_build_core-0.4.3/docs/api/scikit_build_core.metadata.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/docs/api/scikit_build_core.rst` & `scikit_build_core-0.4.3/docs/api/scikit_build_core.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/docs/api/scikit_build_core.settings.rst` & `scikit_build_core-0.4.3/docs/api/scikit_build_core.settings.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/docs/api/scikit_build_core.setuptools.rst` & `scikit_build_core-0.4.3/docs/api/scikit_build_core.setuptools.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/docs/examples/getting_started/abi3/example.c` & `scikit_build_core-0.4.3/docs/examples/getting_started/abi3/example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/docs/examples/getting_started/c/example.c` & `scikit_build_core-0.4.3/docs/examples/getting_started/c/example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/docs/examples/getting_started/cython/CMakeLists.txt` & `scikit_build_core-0.4.3/docs/examples/getting_started/cython/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/docs/examples/getting_started/fortran/CMakeLists.txt` & `scikit_build_core-0.4.3/docs/examples/getting_started/fortran/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/docs/examples/getting_started/swig/CMakeLists.txt` & `scikit_build_core-0.4.3/docs/examples/getting_started/swig/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/_logging.py` & `scikit_build_core-0.4.3/src/scikit_build_core/_logging.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/_shutil.py` & `scikit_build_core-0.4.3/src/scikit_build_core/_shutil.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/cmake.py` & `scikit_build_core-0.4.3/src/scikit_build_core/cmake.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/errors.py` & `scikit_build_core-0.4.3/src/scikit_build_core/errors.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/program_search.py` & `scikit_build_core-0.4.3/src/scikit_build_core/program_search.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/_compat/typing.py` & `scikit_build_core-0.4.3/src/scikit_build_core/_compat/typing.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/_compat/importlib/metadata.py` & `scikit_build_core-0.4.3/src/scikit_build_core/_compat/importlib/metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/build/__init__.py` & `scikit_build_core-0.4.3/src/scikit_build_core/build/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/build/_file_processor.py` & `scikit_build_core-0.4.3/src/scikit_build_core/build/_file_processor.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/build/_init.py` & `scikit_build_core-0.4.3/src/scikit_build_core/build/_init.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/build/_pathutil.py` & `scikit_build_core-0.4.3/src/scikit_build_core/build/_pathutil.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/build/_scripts.py` & `scikit_build_core-0.4.3/src/scikit_build_core/build/_scripts.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/build/_wheelfile.py` & `scikit_build_core-0.4.3/src/scikit_build_core/build/_wheelfile.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import os
 import stat
 import time
 import zipfile
 from collections.abc import Mapping, Set
 from email.message import Message
 from email.policy import EmailPolicy
-from pathlib import Path, PurePosixPath
+from pathlib import Path
 from zipfile import ZipInfo
 
 import packaging.utils
 from packaging.tags import Tag
 from packaging.utils import BuildTag
 from pyproject_metadata import StandardMetadata
 
@@ -68,16 +68,16 @@
     """A general tool for writing wheels. Designed to look a little like ZipFile."""
 
     metadata: StandardMetadata
     folder: Path
     tags: Set[Tag]
     wheel_metadata = WheelMetadata(root_is_purelib=False)
     buildver: str = ""
-    zipfile: zipfile.ZipFile | None = None
     license_files: Mapping[Path, bytes] = dataclasses.field(default_factory=dict)
+    _zipfile: zipfile.ZipFile | None = None
 
     @property
     def name_ver(self) -> str:
         name = packaging.utils.canonicalize_name(self.metadata.name).replace("-", "_")
         # replace - with _ as a local version separator
         version = str(self.metadata.version).replace("-", "_")
         return f"{name}-{version}"
@@ -151,60 +151,73 @@
         for key, path in plans.items():
             for filename in sorted(path.glob("**/*")):
                 is_in_dist_info = any(x.endswith(".dist-info") for x in filename.parts)
                 is_python_cache = filename.suffix in {".pyc", ".pyo"}
                 if filename.is_file() and not is_in_dist_info and not is_python_cache:
                     relpath = filename.relative_to(path)
                     target = Path(data_dir) / key / relpath if key else relpath
-                    # Zipfiles require Posix paths for the arcname
-                    self.write(str(filename), str(PurePosixPath(target)))
+                    self.write(str(filename), str(target))
 
         dist_info_contents = self.dist_info_contents()
         for key, data in dist_info_contents.items():
             self.writestr(f"{self.dist_info}/{key}", data)
 
     def write(self, filename: str, arcname: str | None = None) -> None:
-        """Write a file to the archive."""
+        """Write a file to the archive. Paths are normalized to Posix paths."""
 
         with Path(filename).open("rb") as f:
             st = os.fstat(f.fileno())
             data = f.read()
-        zinfo = ZipInfo(arcname or str(filename), date_time=self.timestamp(st.st_mtime))
+
+        # Zipfiles require Posix paths for the arcname
+        zinfo = ZipInfo(
+            (arcname or filename).replace("\\", "/"),
+            date_time=self.timestamp(st.st_mtime),
+        )
         zinfo.compress_type = zipfile.ZIP_DEFLATED
         zinfo.external_attr = (stat.S_IMODE(st.st_mode) | stat.S_IFMT(st.st_mode)) << 16
         self.writestr(zinfo, data)
 
     def writestr(self, zinfo_or_arcname: str | ZipInfo, data: bytes) -> None:
         """Write bytes (not strings) to the archive."""
         assert isinstance(data, bytes)
-        assert self.zipfile is not None
+        assert self._zipfile is not None
         if isinstance(zinfo_or_arcname, zipfile.ZipInfo):
             zinfo = zinfo_or_arcname
         else:
-            zinfo = zipfile.ZipInfo(zinfo_or_arcname, date_time=self.timestamp())
+            zinfo = zipfile.ZipInfo(
+                zinfo_or_arcname.replace("\\", "/"),
+                date_time=self.timestamp(),
+            )
             zinfo.compress_type = zipfile.ZIP_DEFLATED
             zinfo.external_attr = (0o664 | stat.S_IFREG) << 16
-        self.zipfile.writestr(zinfo, data)
+        assert (
+            "\\" not in zinfo.filename
+        ), f"\\ not supported in zip; got {zinfo.filename!r}"
+        self._zipfile.writestr(zinfo, data)
 
     def __enter__(self) -> Self:
         if not self.wheelpath.parent.exists():
             self.wheelpath.parent.mkdir(parents=True)
 
-        self.zipfile = zipfile.ZipFile(
+        self._zipfile = zipfile.ZipFile(
             self.wheelpath, "w", compression=zipfile.ZIP_DEFLATED
         )
         return self
 
     def __exit__(self, *args: object) -> None:
-        assert self.zipfile is not None
+        assert self._zipfile is not None
         record = f"{self.dist_info}/RECORD"
         data = io.StringIO()
         writer = csv.writer(data, delimiter=",", quotechar='"', lineterminator="\n")
-        for member in self.zipfile.infolist():
-            with self.zipfile.open(member) as f:
+        for member in self._zipfile.infolist():
+            assert (
+                "\\" not in member.filename
+            ), f"Invalid zip contents: {member.filename}"
+            with self._zipfile.open(member) as f:
                 member_data = f.read()
             sha = _b64encode(hashlib.sha256(member_data).digest()).decode("ascii")
             writer.writerow((member.filename, f"sha256={sha}", member.file_size))
         writer.writerow((record, "", ""))
         self.writestr(record, data.getvalue().encode("utf-8"))
-        self.zipfile.close()
-        self.zipfile = None
+        self._zipfile.close()
+        self._zipfile = None
```

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/build/sdist.py` & `scikit_build_core-0.4.3/src/scikit_build_core/build/sdist.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/build/wheel.py` & `scikit_build_core-0.4.3/src/scikit_build_core/build/wheel.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,15 +250,17 @@
                     path_to_module(v.relative_to(wheel_dirs["platlib"])): str(
                         v.relative_to(wheel_dirs["platlib"])
                     )
                     for v in scantree(wheel_dirs["platlib"])
                 }
                 editable_py = resources / "_editable_redirect.py"
                 editable_txt = editable_py.read_text(encoding="utf-8")
-                reload_dir = os.fspath(build_dir) if settings.build_dir else None
+                reload_dir = (
+                    os.fspath(build_dir.resolve()) if settings.build_dir else None
+                )
                 editable_txt += f"\n\ninstall({modules!r}, {installed!r}, {reload_dir!r}, {settings.editable.rebuild!r}, {settings.editable.verbose!r})\n"
 
                 wheel.writestr(
                     f"_{normalized_name}_editable.py",
                     editable_txt.encode("utf-8"),
                 )
                 wheel.writestr(
```

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/builder/builder.py` & `scikit_build_core-0.4.3/src/scikit_build_core/builder/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,27 +111,31 @@
             logger.debug("FindPython backport activated at {}", fp_dir)
 
         local_def = set_environment_for_gen(
             self.config.cmake, self.config.env, self.settings.ninja
         )
         cmake_defines.update(local_def)
 
-        cache_config: dict[str, str | Path] = {
+        cache_config: dict[str, str | Path | bool] = {
             "SKBUILD": "2",
             "SKBUILD_CORE_VERSION": __version__,
         }
 
         if name is not None:
             canonical_name = name.replace("-", "_").replace(".", "_")
             cache_config["SKBUILD_PROJECT_NAME"] = canonical_name
         if version is not None:
             cache_config["SKBUILD_PROJECT_VERSION"] = str(version)
 
         if limited_abi is None:
-            limited_abi = self.settings.wheel.py_api.startswith("cp3")
+            if self.settings.wheel.py_api.startswith("cp3"):
+                target_minor_version = int(self.settings.wheel.py_api[3:])
+                limited_abi = target_minor_version >= sys.version_info.minor
+            else:
+                limited_abi = False
 
         python_library = get_python_library(self.config.env, abi3=limited_abi)
         python_include_dir = get_python_include_dir()
 
         # Classic Find Python
         cache_config["PYTHON_EXECUTABLE"] = sys.executable
         cache_config["PYTHON_INCLUDE_DIR"] = python_include_dir
@@ -162,14 +166,19 @@
 
                 ext_suffix = distutils.sysconfig.get_config_var("EXT_SUFFIX")
             else:
                 ext_suffix = sysconfig.get_config_var("EXT_SUFFIX")
             assert isinstance(ext_suffix, str)
             cache_config["SKBUILD_SOABI"] = ext_suffix.rsplit(".", 1)[0].lstrip(".")
 
+        # Allow CMakeLists to detect this is supposed to be a limited ABI build
+        cache_config["SKBUILD_SABI_COMPONENT"] = (
+            "Development.SABIModule" if limited_abi else ""
+        )
+
         if cache_entries:
             cache_config.update(cache_entries)
 
         self.config.init_cache(cache_config)
 
         if sys.platform.startswith("darwin"):
             # Cross-compile support for macOS - respect ARCHFLAGS if set
```

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/builder/generator.py` & `scikit_build_core-0.4.3/src/scikit_build_core/builder/generator.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/builder/get_requires.py` & `scikit_build_core-0.4.3/src/scikit_build_core/builder/get_requires.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/builder/macos.py` & `scikit_build_core-0.4.3/src/scikit_build_core/builder/macos.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/builder/sysconfig.py` & `scikit_build_core-0.4.3/src/scikit_build_core/builder/sysconfig.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/builder/wheel_tag.py` & `scikit_build_core-0.4.3/src/scikit_build_core/builder/wheel_tag.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/file_api/_cattrs_converter.py` & `scikit_build_core-0.4.3/src/scikit_build_core/file_api/_cattrs_converter.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/file_api/query.py` & `scikit_build_core-0.4.3/src/scikit_build_core/file_api/query.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/file_api/reply.py` & `scikit_build_core-0.4.3/src/scikit_build_core/file_api/reply.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/file_api/model/codemodel.py` & `scikit_build_core-0.4.3/src/scikit_build_core/file_api/model/codemodel.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/file_api/model/directory.py` & `scikit_build_core-0.4.3/src/scikit_build_core/file_api/model/directory.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/file_api/model/index.py` & `scikit_build_core-0.4.3/src/scikit_build_core/file_api/model/index.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/file_api/model/toolchains.py` & `scikit_build_core-0.4.3/src/scikit_build_core/file_api/model/toolchains.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/metadata/fancy_pypi_readme.py` & `scikit_build_core-0.4.3/src/scikit_build_core/metadata/fancy_pypi_readme.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/metadata/setuptools_scm.py` & `scikit_build_core-0.4.3/src/scikit_build_core/metadata/setuptools_scm.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/resources/_editable_redirect.py` & `scikit_build_core-0.4.3/src/scikit_build_core/resources/_editable_redirect.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/resources/known_wheels.toml` & `scikit_build_core-0.4.3/src/scikit_build_core/resources/known_wheels.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/resources/find_python/Copyright.txt` & `scikit_build_core-0.4.3/src/scikit_build_core/resources/find_python/Copyright.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake` & `scikit_build_core-0.4.3/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake` & `scikit_build_core-0.4.3/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/resources/find_python/FindPython.cmake` & `scikit_build_core-0.4.3/src/scikit_build_core/resources/find_python/FindPython.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/resources/find_python/FindPython3.cmake` & `scikit_build_core-0.4.3/src/scikit_build_core/resources/find_python/FindPython3.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/resources/find_python/FindPython/Support.cmake` & `scikit_build_core-0.4.3/src/scikit_build_core/resources/find_python/FindPython/Support.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/settings/_load_provider.py` & `scikit_build_core-0.4.3/src/scikit_build_core/settings/_load_provider.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/settings/metadata.py` & `scikit_build_core-0.4.3/src/scikit_build_core/settings/metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/settings/skbuild_model.py` & `scikit_build_core-0.4.3/src/scikit_build_core/settings/skbuild_model.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/settings/skbuild_read_settings.py` & `scikit_build_core-0.4.3/src/scikit_build_core/settings/skbuild_read_settings.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/settings/sources.py` & `scikit_build_core-0.4.3/src/scikit_build_core/settings/sources.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,43 @@
+"""
+This is the configuration tooling for scikit-build-core. This is build around
+the :class:`Source` Protocol. Sources are created with some input (like a toml
+file for the :class:`TOMLSource`). Sources also usually have some prefix (like
+``tool.scikit-build``) as well. The :class:`SourceChain` holds a collection of
+Sources, and is the primary way to use them.
+
+An end user interacts with :class:`SourceChain` via ``.convert_target``, which
+takes a Dataclass class and returns an instance with fields populated.
+
+Example of usage::
+
+    sources = SourceChain(TOMLSource("tool", "mypackage", settings=pyproject_dict), ...)
+    settings = sources.convert_target(SomeSettingsModel)
+
+    unrecognized_options = list(source.unrecognized_options(SomeSettingsModel)
+
+
+Naming conventions:
+
+- ``model`` is the complete Dataclass.
+- ``target`` is the type to convert a single item to.
+- ``settings`` is the input data source (unless it already has a name, like
+  ``env``).
+- ``options`` are the names of the items in the ``model``, formatted in the
+  style of the current Source.
+- ``fields`` are the tuple of strings describing a nested field in the
+  ``model``.
+"""
+
+
 from __future__ import annotations
 
 import dataclasses
 import os
+import typing
 from collections.abc import Generator, Iterator, Mapping, Sequence
 from typing import Any, TypeVar, Union
 
 from .._compat.builtins import ExceptionGroup
 from .._compat.typing import Protocol, runtime_checkable
 
 T = TypeVar("T")
@@ -13,24 +45,24 @@
 __all__ = ["Source", "SourceChain", "ConfSource", "EnvSource", "TOMLSource"]
 
 
 def __dir__() -> list[str]:
     return __all__
 
 
-def _dig_strict(dict_: Mapping[str, Any], *names: str) -> Any:
+def _dig_strict(__dict: Mapping[str, Any], *names: str) -> Any:
     for name in names:
-        dict_ = dict_[name]
-    return dict_
+        __dict = __dict[name]
+    return __dict
 
 
-def _dig_not_strict(dict_: Mapping[str, Any], *names: str) -> Any:
+def _dig_not_strict(__dict: Mapping[str, Any], *names: str) -> Any:
     for name in names:
-        dict_ = dict_.get(name, {})
-    return dict_
+        __dict = __dict.get(name, {})
+    return __dict
 
 
 def _dig_fields(__opt: Any, *names: str) -> Any:
     for name in names:
         fields = dataclasses.fields(__opt)
         types = [x.type for x in fields if x.name == name]
         if len(types) != 1:
@@ -49,15 +81,16 @@
     @property
     def __args__(self) -> list[Any]:
         ...
 
 
 def _process_union(target: type[Any]) -> Any:
     """
-    Selects the non-None item in an Optional or Optional-like Union. Passes through non-Unions.
+    Selects the non-None item in an Optional or Optional-like Union. Passes
+    through non-Unions.
     """
 
     if (
         not isinstance(target, TypeLike)
         or not hasattr(target, "__origin__")
         or target.__origin__ is not Union
     ):
@@ -73,75 +106,92 @@
 
     msg = "Only Unions with None supported"
     raise AssertionError(msg)
 
 
 def _get_target_raw_type(target: type[Any]) -> type[Any]:
     """
-    Takes a type like Optional[str] and returns str,
-    or Optional[Dict[str, int]] and returns dict.
+    Takes a type like ``Optional[str]`` and returns str,
+    or ``Optional[Dict[str, int]]`` and returns dict.
     """
 
     target = _process_union(target)
     # The hasattr is required for Python 3.7, though not quite sure why
     if isinstance(target, TypeLike) and hasattr(target, "__origin__"):
         return target.__origin__
     return target
 
 
-def _get_inner_type(target: type[Any]) -> type[Any]:
+def _get_inner_type(__target: type[Any]) -> type[Any]:
     """
-    Takes a types like List[str] and returns str,
-    or Dict[str, int] and returns int.
+    Takes a types like ``List[str]`` and returns str,
+    or ``Dict[str, int]`` and returns int.
     """
 
-    raw_target = _get_target_raw_type(target)
-    target = _process_union(target)
+    raw_target = _get_target_raw_type(__target)
+    target = _process_union(__target)
     if raw_target == list:
-        assert isinstance(target, TypeLike)
+        assert isinstance(__target, TypeLike)
         return target.__args__[0]
     if raw_target == dict:
-        assert isinstance(target, TypeLike)
+        assert isinstance(__target, TypeLike)
         return target.__args__[1]
     msg = f"Expected a list or dict, got {target!r}"
     raise AssertionError(msg)
 
 
-def _nested_dataclass_to_names(target: type[Any], *inner: str) -> Iterator[list[str]]:
+def _nested_dataclass_to_names(__target: type[Any], *inner: str) -> Iterator[list[str]]:
     """
-    Yields each entry, like ("a", "b", "c") for a.b.c
+    Yields each entry, like ``("a", "b", "c")`` for ``a.b.c``.
     """
 
-    if dataclasses.is_dataclass(target):
-        for field in dataclasses.fields(target):
+    if dataclasses.is_dataclass(__target):
+        for field in dataclasses.fields(__target):
             yield from _nested_dataclass_to_names(field.type, *inner, field.name)
     else:
         yield list(inner)
 
 
 class Source(Protocol):
     def has_item(self, *fields: str, is_dict: bool) -> bool:
         """
-        Check if the source contains a chain of fields. For example, fields =
-        [Field(name="a"), Field(name="b")] will check if the source contains the
-        key "a.b".
+        Check if the source contains a chain of fields. For example, ``fields =
+        [Field(name="a"), Field(name="b")]`` will check if the source contains the
+        key "a.b". ``is_dict`` should be set if it can be nested.
         """
         ...
 
     def get_item(self, *fields: str, is_dict: bool) -> Any:
+        """
+        Select an item from a chain of fields. Raises KeyError if
+        the there is no item. ``is_dict`` should be set if it can be nested.
+        """
         ...
 
     @classmethod
     def convert(cls, item: Any, target: type[Any]) -> object:
+        """
+        Convert an ``item`` from the base representation of the source's source
+        into a ``target`` type. Raises TypeError if the conversion fails.
+        """
         ...
 
     def unrecognized_options(self, options: object) -> Generator[str, None, None]:
+        """
+        Given a model, produce an iterator of all unrecognized option names.
+        Empty iterator if this can't be computed for the source (like for
+        environment variables).
+        """
         ...
 
     def all_option_names(self, target: type[Any]) -> Iterator[str]:
+        """
+        Given a model, produce a list of all possible names (used for producing
+        suggestions).
+        """
         ...
 
 
 class EnvSource:
     """
     This is a source using environment variables.
     """
@@ -181,15 +231,15 @@
         if raw_target is bool:
             result = item.strip().lower() not in {"0", "false", "off", "no", ""}
             return result
 
         if callable(raw_target):
             return raw_target(item)
         msg = f"Can't convert target {target}"
-        raise AssertionError(msg)
+        raise TypeError(msg)
 
     def unrecognized_options(
         self, options: object  # noqa: ARG002
     ) -> Generator[str, None, None]:
         yield from ()
 
     def all_option_names(self, target: type[Any]) -> Iterator[str]:
@@ -290,15 +340,15 @@
             raise TypeError(msg)
         if raw_target is bool:
             result = item.strip().lower() not in {"0", "false", "off", "no", ""}
             return result
         if callable(raw_target):
             return raw_target(item)
         msg = f"Can't convert target {target}"
-        raise AssertionError(msg)
+        raise TypeError(msg)
 
     def unrecognized_options(self, options: object) -> Generator[str, None, None]:
         if not self.verify:
             return
         for keystr in self.settings:
             keys = keystr.replace("-", "_").split(".")[len(self.prefixes) :]
             try:
@@ -359,15 +409,15 @@
                 raise TypeError(msg)
             return {k: cls.convert(v, _get_inner_type(target)) for k, v in item.items()}
         if raw_target == Any:
             return item
         if callable(raw_target):
             return raw_target(item)
         msg = f"Can't convert target {target}"
-        raise AssertionError(msg)
+        raise TypeError(msg)
 
     def unrecognized_options(self, options: object) -> Generator[str, None, None]:
         yield from _unrecognized_dict(self.settings, options, self.prefixes)
 
     def all_option_names(self, target: type[Any]) -> Iterator[str]:
         for names in _nested_dataclass_to_names(target):
             dash_names = [name.replace("_", "-") for name in names]
@@ -393,19 +443,14 @@
     def get_item(self, *fields: str, is_dict: bool) -> Any:
         for source in self.sources:
             if source.has_item(*fields, is_dict=is_dict):
                 return source.get_item(*fields, is_dict=is_dict)
         msg = f"{fields!r} not found in any source"
         raise KeyError(msg)
 
-    @classmethod
-    def convert(cls, item: Any, target: type[T]) -> T:  # noqa: ARG003
-        msg = "SourceChain cannot convert items, use the result from has_item"
-        raise NotImplementedError(msg)
-
     def convert_target(self, target: type[T], *prefixes: str) -> T:
         """
         Given a dataclass type, create an object of that dataclass filled
         with the values in the sources.
         """
 
         errors = []
@@ -463,10 +508,12 @@
 
         return target(**prep)
 
     def unrecognized_options(self, options: object) -> Generator[str, None, None]:
         for source in self.sources:
             yield from source.unrecognized_options(options)
 
-    def all_option_names(self, target: type[Any]) -> Iterator[str]:
-        for source in self.sources:
-            yield from source.all_option_names(target)
+
+if typing.TYPE_CHECKING:
+    _: Source = typing.cast(EnvSource, None)
+    _ = typing.cast(ConfSource, None)
+    _ = typing.cast(TOMLSource, None)
```

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/setuptools/build_cmake.py` & `scikit_build_core-0.4.3/src/scikit_build_core/setuptools/build_cmake.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/setuptools/build_meta.py` & `scikit_build_core-0.4.3/src/scikit_build_core/setuptools/build_meta.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from setuptools.build_meta import (
     build_sdist,
     build_wheel,
     prepare_metadata_for_build_wheel,
 )
 
 if hasattr(setuptools.build_meta, "build_editable"):
-    from setuptools.build_meta import build_editable  # type: ignore[attr-defined]
+    from setuptools.build_meta import build_editable
 
 if hasattr(setuptools.build_meta, "prepare_metadata_for_build_editable"):
-    from setuptools.build_meta import (  # type: ignore[attr-defined]
+    from setuptools.build_meta import (
         prepare_metadata_for_build_editable,
     )
 
 
 __all__ = [
     "build_editable",
     "build_sdist",
@@ -59,11 +59,11 @@
 
     def get_requires_for_build_editable(
         config_settings: dict[str, str | list[str]] | None = None
     ) -> list[str]:
         from ..builder.get_requires import GetRequires
 
         requires = GetRequires(config_settings)
-        setuptools_reqs = setuptools.build_meta.get_requires_for_build_editable(  # type: ignore[attr-defined]
+        setuptools_reqs = setuptools.build_meta.get_requires_for_build_editable(
             config_settings
         )
         return [*setuptools_reqs, *requires.cmake(), *requires.ninja()]
```

### Comparing `scikit_build_core-0.4.2/src/scikit_build_core/setuptools/wrapper.py` & `scikit_build_core-0.4.3/src/scikit_build_core/setuptools/wrapper.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/conftest.py` & `scikit_build_core-0.4.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/test_builder.py` & `scikit_build_core-0.4.3/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/test_cmake_config.py` & `scikit_build_core-0.4.3/tests/test_cmake_config.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/test_dynamic_metadata.py` & `scikit_build_core-0.4.3/tests/test_dynamic_metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/test_fileapi.py` & `scikit_build_core-0.4.3/tests/test_fileapi.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/test_fortran.py` & `scikit_build_core-0.4.3/tests/test_fortran.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/test_generator_default.py` & `scikit_build_core-0.4.3/tests/test_generator_default.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/test_get_requires.py` & `scikit_build_core-0.4.3/tests/test_get_requires.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/test_module_dir.py` & `scikit_build_core-0.4.3/tests/test_module_dir.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/test_name_main.py` & `scikit_build_core-0.4.3/tests/test_name_main.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/test_prepare_metadata.py` & `scikit_build_core-0.4.3/tests/test_prepare_metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/test_process_scripts.py` & `scikit_build_core-0.4.3/tests/test_process_scripts.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/test_program_search.py` & `scikit_build_core-0.4.3/tests/test_program_search.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/test_pyproject_abi3.py` & `scikit_build_core-0.4.3/tests/test_pyproject_abi3.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/test_pyproject_extra_dirs.py` & `scikit_build_core-0.4.3/tests/test_pyproject_extra_dirs.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/test_pyproject_pep517.py` & `scikit_build_core-0.4.3/tests/test_pyproject_pep517.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/test_pyproject_pep518.py` & `scikit_build_core-0.4.3/tests/test_pyproject_pep518.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/test_pyproject_pep660.py` & `scikit_build_core-0.4.3/tests/test_pyproject_pep660.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/test_settings.py` & `scikit_build_core-0.4.3/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/test_setuptools_abi3.py` & `scikit_build_core-0.4.3/tests/test_setuptools_abi3.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/test_setuptools_pep517.py` & `scikit_build_core-0.4.3/tests/test_setuptools_pep517.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/test_setuptools_pep518.py` & `scikit_build_core-0.4.3/tests/test_setuptools_pep518.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/test_simple_pure.py` & `scikit_build_core-0.4.3/tests/test_simple_pure.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/test_simplest_c.py` & `scikit_build_core-0.4.3/tests/test_simplest_c.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/test_skbuild_settings.py` & `scikit_build_core-0.4.3/tests/test_skbuild_settings.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/test_wheelfile_utils.py` & `scikit_build_core-0.4.3/tests/test_wheelfile_utils.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json` & `scikit_build_core-0.4.3/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json` & `scikit_build_core-0.4.3/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json` & `scikit_build_core-0.4.3/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json` & `scikit_build_core-0.4.3/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json` & `scikit_build_core-0.4.3/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json` & `scikit_build_core-0.4.3/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json` & `scikit_build_core-0.4.3/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/packages/abi3_pyproject_ext/abi3_example.c` & `scikit_build_core-0.4.3/tests/packages/abi3_pyproject_ext/abi3_example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/packages/abi3_setuptools_ext/abi3_example.c` & `scikit_build_core-0.4.3/tests/packages/abi3_setuptools_ext/abi3_example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/packages/dynamic_metadata/plugin_project.toml` & `scikit_build_core-0.4.3/tests/packages/dynamic_metadata/plugin_project.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/packages/dynamic_metadata/src/module.c` & `scikit_build_core-0.4.3/tests/packages/dynamic_metadata/src/module.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/packages/filepath_pure/CMakeLists.txt` & `scikit_build_core-0.4.3/tests/packages/filepath_pure/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/packages/fortran_example/CMakeLists.txt` & `scikit_build_core-0.4.3/tests/packages/fortran_example/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/packages/mixed_setuptools/CMakeLists.txt` & `scikit_build_core-0.4.3/tests/packages/mixed_setuptools/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/packages/simple_pyproject_ext/LICENSE` & `scikit_build_core-0.4.3/tests/packages/simple_pyproject_ext/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/packages/simple_pyproject_ext/src/main.cpp` & `scikit_build_core-0.4.3/tests/packages/simple_pyproject_ext/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/packages/simple_pyproject_source_dir/LICENSE` & `scikit_build_core-0.4.3/tests/packages/simple_pyproject_source_dir/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/packages/simple_pyproject_source_dir/src/main.cpp` & `scikit_build_core-0.4.3/tests/packages/simple_pyproject_source_dir/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/packages/simple_setuptools_ext/LICENSE` & `scikit_build_core-0.4.3/tests/packages/simple_setuptools_ext/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/packages/simple_setuptools_ext/src/main.cpp` & `scikit_build_core-0.4.3/tests/packages/simple_setuptools_ext/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/packages/simplest_c/CMakeLists.txt` & `scikit_build_core-0.4.3/tests/packages/simplest_c/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/tests/packages/simplest_c/src/module.c` & `scikit_build_core-0.4.3/tests/packages/simplest_c/src/module.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/.gitignore` & `scikit_build_core-0.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/LICENSE` & `scikit_build_core-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.2/README.md` & `scikit_build_core-0.4.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # scikit-build-core
 
 [![Documentation Status][rtd-badge]][rtd-link]
+[![GitHub Discussion][github-discussions-badge]][github-discussions-link]
 
 [![Actions Status][actions-badge]][actions-link]
-[![Code style: black][black-badge]][black-link]
 [![codecov][codecov-badge]][codecov-link]
-[![GitHub Discussion][github-discussions-badge]][github-discussions-link]
 
 [![PyPI version][pypi-version]][pypi-link]
 [![Conda-Forge][conda-badge]][conda-link]
 [![PyPI platforms][pypi-platforms]][pypi-link]
 
 <!-- Not implemented yet
 [![Gitter][gitter-badge]][gitter-link]
@@ -207,14 +206,32 @@
 # List dynamic metadata fields and hook locations in this table
 ```
 
 Most CMake environment variables should be supported, and `CMAKE_ARGS` can be
 used to set extra CMake args. `ARCHFLAGS` is used to specify macOS universal2 or
 cross-compiles, just like setuptools.
 
+## Other projects for building
+
+Scikit-build-core is a binary build backend. There are also other binary build
+backends:
+
+- [py-build-cmake][]: A different attempt at a standards compliant builder for
+  CMake. Strong focus on cross-compilation. Uses Flit internals.
+- [meson-python][]: A meson-based build backend; has some maintainer overlap
+  with scikit-build-core.
+- [maturin][]: A build backend for Rust projects, using Cargo.
+- [enscons][]: A SCons based backend, not very actively developed (it predates
+  all the others in modern standard support!)
+
+If you don't need a binary build, you don't need to use a binary build backend!
+There are some very good Python build backends; we recommend [hatchling][] as a
+good balance between good defaults for beginners and good support for advanced
+use cases. This is the tool scikit-build-core itself uses.
+
 ## Acknowledgements
 
 Support for this work was provided by NSF cooperative agreement [OAC-2209877][].
 
 <!-- prettier-ignore-start -->
 [actions-badge]:            https://github.com/scikit-build/scikit-build-core/workflows/CI/badge.svg
 [actions-link]:             https://github.com/scikit-build/scikit-build-core/actions
@@ -230,8 +247,12 @@
 [codecov-link]:             https://codecov.io/gh/scikit-build/scikit-build-core
 [pypi-link]:                https://pypi.org/project/scikit-build-core/
 [pypi-platforms]:           https://img.shields.io/pypi/pyversions/scikit-build-core
 [pypi-version]:             https://badge.fury.io/py/scikit-build-core.svg
 [rtd-badge]:                https://readthedocs.org/projects/scikit-build-core/badge/?version=latest
 [rtd-link]:                 https://scikit-build-core.readthedocs.io/en/latest/?badge=latest
 [OAC-2209877]:              https://www.nsf.gov/awardsearch/showAward?AWD_ID=2209877&HistoricalAwards=false
+[hatchling]:                https://hatch.pypa.io/latest
+[maturin]:                  https://www.maturin.rs
+[enscons]:                  https://pypi.org/project/enscons
+[py-build-cmake]:           https://tttapa.github.io/py-build-cmake
 <!-- prettier-ignore-end -->
```

### Comparing `scikit_build_core-0.4.2/pyproject.toml` & `scikit_build_core-0.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Development Status :: 4 - Beta",
     "Typing :: Typed",
 ]
 
 dynamic = ["version"]
 
 dependencies = [
@@ -101,14 +102,15 @@
 addopts = ["-ra", "--strict-markers", "--strict-config"]
 xfail_strict = true
 filterwarnings = [
     "error",
     "ignore:pkg_resources is deprecated as an API:DeprecationWarning",  # Caused by wheel in tests
     "ignore:Config variable '.*' is unset, Python ABI tag may be incorrect:RuntimeWarning",
     "ignore:onerror argument is deprecated, use onexc instead:DeprecationWarning",  # Caused by wheel and Python 3.12
+    "ignore:(ast.Str|Attribute s|ast.NameConstant|ast.Num) is deprecated:DeprecationWarning:_pytest",  # Python 3.12
 ]
 log_cli_level = "info"
 testpaths = ["tests"]
 markers = [
     "broken_on_urct: Broken for now due to lib not found",
     "compile: Compiles code",
     "configure: Configures CMake code",
```

### Comparing `scikit_build_core-0.4.2/PKG-INFO` & `scikit_build_core-0.4.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit_build_core
-Version: 0.4.2
+Version: 0.4.3
 Summary: Build backend for CMake based projects
 Project-URL: Homepage, https://github.com/scikit-build/scikit-build-core
 Project-URL: Documentation, https://scikit-build-core.readthedocs.io
 Project-URL: Discussions, https://github.com/orgs/scikit-build/discussions
 Project-URL: Issues, https://github.com/scikit-build/scikit-build-core/issues
 Project-URL: Changelog, https://scikit-build-core.readthedocs.io/en/latest/changelog.html
 Author-email: Henry Schreiner <henryfs@princeton.edu>
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Requires-Dist: exceptiongroup; python_version < '3.11'
 Requires-Dist: importlib-metadata; python_version < '3.8'
 Requires-Dist: importlib-resources>=1.3; python_version < '3.9'
@@ -61,19 +62,18 @@
 Requires-Dist: setuptools; extra == 'test'
 Requires-Dist: wheel; extra == 'test'
 Description-Content-Type: text/markdown
 
 # scikit-build-core
 
 [![Documentation Status][rtd-badge]][rtd-link]
+[![GitHub Discussion][github-discussions-badge]][github-discussions-link]
 
 [![Actions Status][actions-badge]][actions-link]
-[![Code style: black][black-badge]][black-link]
 [![codecov][codecov-badge]][codecov-link]
-[![GitHub Discussion][github-discussions-badge]][github-discussions-link]
 
 [![PyPI version][pypi-version]][pypi-link]
 [![Conda-Forge][conda-badge]][conda-link]
 [![PyPI platforms][pypi-platforms]][pypi-link]
 
 <!-- Not implemented yet
 [![Gitter][gitter-badge]][gitter-link]
@@ -271,14 +271,32 @@
 # List dynamic metadata fields and hook locations in this table
 ```
 
 Most CMake environment variables should be supported, and `CMAKE_ARGS` can be
 used to set extra CMake args. `ARCHFLAGS` is used to specify macOS universal2 or
 cross-compiles, just like setuptools.
 
+## Other projects for building
+
+Scikit-build-core is a binary build backend. There are also other binary build
+backends:
+
+- [py-build-cmake][]: A different attempt at a standards compliant builder for
+  CMake. Strong focus on cross-compilation. Uses Flit internals.
+- [meson-python][]: A meson-based build backend; has some maintainer overlap
+  with scikit-build-core.
+- [maturin][]: A build backend for Rust projects, using Cargo.
+- [enscons][]: A SCons based backend, not very actively developed (it predates
+  all the others in modern standard support!)
+
+If you don't need a binary build, you don't need to use a binary build backend!
+There are some very good Python build backends; we recommend [hatchling][] as a
+good balance between good defaults for beginners and good support for advanced
+use cases. This is the tool scikit-build-core itself uses.
+
 ## Acknowledgements
 
 Support for this work was provided by NSF cooperative agreement [OAC-2209877][].
 
 <!-- prettier-ignore-start -->
 [actions-badge]:            https://github.com/scikit-build/scikit-build-core/workflows/CI/badge.svg
 [actions-link]:             https://github.com/scikit-build/scikit-build-core/actions
@@ -294,8 +312,12 @@
 [codecov-link]:             https://codecov.io/gh/scikit-build/scikit-build-core
 [pypi-link]:                https://pypi.org/project/scikit-build-core/
 [pypi-platforms]:           https://img.shields.io/pypi/pyversions/scikit-build-core
 [pypi-version]:             https://badge.fury.io/py/scikit-build-core.svg
 [rtd-badge]:                https://readthedocs.org/projects/scikit-build-core/badge/?version=latest
 [rtd-link]:                 https://scikit-build-core.readthedocs.io/en/latest/?badge=latest
 [OAC-2209877]:              https://www.nsf.gov/awardsearch/showAward?AWD_ID=2209877&HistoricalAwards=false
+[hatchling]:                https://hatch.pypa.io/latest
+[maturin]:                  https://www.maturin.rs
+[enscons]:                  https://pypi.org/project/enscons
+[py-build-cmake]:           https://tttapa.github.io/py-build-cmake
 <!-- prettier-ignore-end -->
```

