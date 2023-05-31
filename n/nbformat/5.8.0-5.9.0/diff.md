# Comparing `tmp/nbformat-5.8.0.tar.gz` & `tmp/nbformat-5.9.0.tar.gz`

## Comparing `nbformat-5.8.0.tar` & `nbformat-5.9.0.tar`

### file list

```diff
@@ -1,130 +1,129 @@
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 nbformat-5.8.0/.git-blame-ignore-revs
--rw-r--r--   0        0        0    10806 2020-02-02 00:00:00.000000 nbformat-5.8.0/.mailmap
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 nbformat-5.8.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 nbformat-5.8.0/.readthedocs.yaml
--rw-r--r--   0        0        0    13125 2020-02-02 00:00:00.000000 nbformat-5.8.0/CHANGELOG.md
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 nbformat-5.8.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 nbformat-5.8.0/README.md
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 nbformat-5.8.0/RELEASING.md
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 nbformat-5.8.0/codecov.yml
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 nbformat-5.8.0/index.js
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 nbformat-5.8.0/package.json
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 nbformat-5.8.0/.github/dependabot.yml
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 nbformat-5.8.0/.github/scripts/create_npmrc.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 nbformat-5.8.0/.github/scripts/parse_ref.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nbformat-5.8.0/.github/workflows/enforce-label.yml
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 nbformat-5.8.0/.github/workflows/prep-release.yml
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 nbformat-5.8.0/.github/workflows/publish-release.yml
--rw-r--r--   0        0        0     4692 2020-02-02 00:00:00.000000 nbformat-5.8.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0     7417 2020-02-02 00:00:00.000000 nbformat-5.8.0/docs/Makefile
--rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 nbformat-5.8.0/docs/api.rst
--rw-r--r--   0        0        0    10122 2020-02-02 00:00:00.000000 nbformat-5.8.0/docs/conf.py
--rw-r--r--   0        0        0    15210 2020-02-02 00:00:00.000000 nbformat-5.8.0/docs/format_description.rst
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 nbformat-5.8.0/docs/index.rst
--rw-r--r--   0        0        0     7248 2020-02-02 00:00:00.000000 nbformat-5.8.0/docs/make.bat
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 nbformat-5.8.0/docs/markup.rst
--rw-r--r--   0        0        0     6198 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/__init__.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/_imports.py
--rw-r--r--   0        0        0    11260 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/_struct.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/_version.py
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/converter.py
--rw-r--r--   0        0        0     6104 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/current.py
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/json_compat.py
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/notebooknode.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/py.typed
--rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/reader.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/sentinel.py
--rw-r--r--   0        0        0    20875 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/sign.py
--rw-r--r--   0        0        0    22580 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/validator.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/warnings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/corpus/__init__.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/corpus/words.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/corpus/tests/__init__.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/corpus/tests/test_words.py
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/v1/__init__.py
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/v1/convert.py
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/v1/nbbase.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/v1/nbjson.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/v1/rwbase.py
--rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/v2/__init__.py
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/v2/convert.py
--rw-r--r--   0        0        0     5551 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/v2/nbbase.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/v2/nbjson.py
--rw-r--r--   0        0        0     5599 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/v2/nbpy.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/v2/nbxml.py
--rw-r--r--   0        0        0     5829 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/v2/rwbase.py
--rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/v3/__init__.py
--rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/v3/convert.py
--rw-r--r--   0        0        0     7379 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/v3/nbbase.py
--rw-r--r--   0        0        0    12198 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/v3/nbformat.v3.schema.json
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/v3/nbjson.py
--rw-r--r--   0        0        0     7980 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/v3/nbpy.py
--rw-r--r--   0        0        0     6297 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/v3/rwbase.py
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/v4/__init__.py
--rw-r--r--   0        0        0     9459 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/v4/convert.py
--rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/v4/nbbase.py
--rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/v4/nbformat.v4.0.schema.json
--rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/v4/nbformat.v4.1.schema.json
--rw-r--r--   0        0        0    12838 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/v4/nbformat.v4.2.schema.json
--rw-r--r--   0        0        0    14000 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/v4/nbformat.v4.3.schema.json
--rw-r--r--   0        0        0    15703 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/v4/nbformat.v4.4.schema.json
--rw-r--r--   0        0        0    16104 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/v4/nbformat.v4.5.schema.json
--rw-r--r--   0        0        0    16104 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/v4/nbformat.v4.schema.json
--rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/v4/nbjson.py
--rw-r--r--   0        0        0     4258 2020-02-02 00:00:00.000000 nbformat-5.8.0/nbformat/v4/rwbase.py
--rwxr-xr-x   0        0        0      163 2020-02-02 00:00:00.000000 nbformat-5.8.0/scripts/jupyter-trust
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/__init__.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/base.py
--rw-r--r--   0        0        0    17365 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/invalid.ipynb
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/invalid_cell_id.ipynb
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/invalid_unique_cell_id.ipynb
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/many_tracebacks.ipynb
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/no_min_version.ipynb
--rw-r--r--   0        0        0    46130 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/test2.ipynb
--rw-r--r--   0        0        0    15875 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/test3.ipynb
--rw-r--r--   0        0        0    15843 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/test3_no_metadata.ipynb
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/test3_no_min_version.ipynb
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/test3_no_worksheets.ipynb
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/test3_worksheet_with_no_cells.ipynb
--rw-r--r--   0        0        0    16074 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/test4.5.ipynb
--rw-r--r--   0        0        0    17400 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/test4.ipynb
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/test4custom.ipynb
--rw-r--r--   0        0        0    17485 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/test4docinfo.ipynb
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/test4jupyter_metadata.ipynb
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/test4jupyter_metadata_timings.ipynb
--rw-r--r--   0        0        0    18282 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/test4plus.ipynb
--rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/test_api.py
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/test_convert.py
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/test_nbformat.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/test_reader.py
--rw-r--r--   0        0        0     9310 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/test_sign.py
--rw-r--r--   0        0        0    11973 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/test_validator.py
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/v4_5_invalid_metadata.ipynb
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/v4_5_no_cell_id.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/v1/__init__.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/v1/nbexamples.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/v1/test_json.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/v1/test_nbbase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/v2/__init__.py
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/v2/nbexamples.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/v2/test_json.py
--rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/v2/test_nbbase.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/v2/test_nbpy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/v3/__init__.py
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/v3/formattest.py
--rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/v3/nbexamples.py
--rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/v3/test_json.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/v3/test_misc.py
--rw-r--r--   0        0        0     6005 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/v3/test_nbbase.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/v3/test_nbpy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/v4/__init__.py
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/v4/formattest.py
--rw-r--r--   0        0        0     3717 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/v4/nbexamples.py
--rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/v4/test_convert.py
--rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/v4/test_json.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/v4/test_nbbase.py
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 nbformat-5.8.0/tests/v4/test_validate.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 nbformat-5.8.0/.gitignore
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 nbformat-5.8.0/LICENSE
--rw-r--r--   0        0        0     5456 2020-02-02 00:00:00.000000 nbformat-5.8.0/pyproject.toml
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 nbformat-5.8.0/PKG-INFO
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 nbformat-5.9.0/.git-blame-ignore-revs
+-rw-r--r--   0        0        0    10806 2020-02-02 00:00:00.000000 nbformat-5.9.0/.mailmap
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 nbformat-5.9.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nbformat-5.9.0/.readthedocs.yaml
+-rw-r--r--   0        0        0    14259 2020-02-02 00:00:00.000000 nbformat-5.9.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 nbformat-5.9.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 nbformat-5.9.0/README.md
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 nbformat-5.9.0/RELEASING.md
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 nbformat-5.9.0/index.js
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 nbformat-5.9.0/package.json
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 nbformat-5.9.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 nbformat-5.9.0/.github/scripts/create_npmrc.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 nbformat-5.9.0/.github/scripts/parse_ref.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nbformat-5.9.0/.github/workflows/enforce-label.yml
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 nbformat-5.9.0/.github/workflows/prep-release.yml
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 nbformat-5.9.0/.github/workflows/publish-release.yml
+-rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 nbformat-5.9.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     7417 2020-02-02 00:00:00.000000 nbformat-5.9.0/docs/Makefile
+-rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 nbformat-5.9.0/docs/api.rst
+-rw-r--r--   0        0        0    10122 2020-02-02 00:00:00.000000 nbformat-5.9.0/docs/conf.py
+-rw-r--r--   0        0        0    15210 2020-02-02 00:00:00.000000 nbformat-5.9.0/docs/format_description.rst
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 nbformat-5.9.0/docs/index.rst
+-rw-r--r--   0        0        0     7248 2020-02-02 00:00:00.000000 nbformat-5.9.0/docs/make.bat
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 nbformat-5.9.0/docs/markup.rst
+-rw-r--r--   0        0        0     6198 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/__init__.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/_imports.py
+-rw-r--r--   0        0        0    11260 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/_struct.py
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/_version.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/converter.py
+-rw-r--r--   0        0        0     6145 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/current.py
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/json_compat.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/notebooknode.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/py.typed
+-rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/reader.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/sentinel.py
+-rw-r--r--   0        0        0    21475 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/sign.py
+-rw-r--r--   0        0        0    22578 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/validator.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/warnings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/corpus/__init__.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/corpus/words.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/corpus/tests/__init__.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/corpus/tests/test_words.py
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/v1/__init__.py
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/v1/convert.py
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/v1/nbbase.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/v1/nbjson.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/v1/rwbase.py
+-rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/v2/__init__.py
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/v2/convert.py
+-rw-r--r--   0        0        0     5551 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/v2/nbbase.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/v2/nbjson.py
+-rw-r--r--   0        0        0     5607 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/v2/nbpy.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/v2/nbxml.py
+-rw-r--r--   0        0        0     5829 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/v2/rwbase.py
+-rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/v3/__init__.py
+-rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/v3/convert.py
+-rw-r--r--   0        0        0     7379 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/v3/nbbase.py
+-rw-r--r--   0        0        0    12198 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/v3/nbformat.v3.schema.json
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/v3/nbjson.py
+-rw-r--r--   0        0        0     7996 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/v3/nbpy.py
+-rw-r--r--   0        0        0     6297 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/v3/rwbase.py
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/v4/__init__.py
+-rw-r--r--   0        0        0     9459 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/v4/convert.py
+-rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/v4/nbbase.py
+-rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/v4/nbformat.v4.0.schema.json
+-rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/v4/nbformat.v4.1.schema.json
+-rw-r--r--   0        0        0    12838 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/v4/nbformat.v4.2.schema.json
+-rw-r--r--   0        0        0    14000 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/v4/nbformat.v4.3.schema.json
+-rw-r--r--   0        0        0    15703 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/v4/nbformat.v4.4.schema.json
+-rw-r--r--   0        0        0    16104 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/v4/nbformat.v4.5.schema.json
+-rw-r--r--   0        0        0    16104 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/v4/nbformat.v4.schema.json
+-rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/v4/nbjson.py
+-rw-r--r--   0        0        0     4258 2020-02-02 00:00:00.000000 nbformat-5.9.0/nbformat/v4/rwbase.py
+-rwxr-xr-x   0        0        0      163 2020-02-02 00:00:00.000000 nbformat-5.9.0/scripts/jupyter-trust
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/__init__.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/base.py
+-rw-r--r--   0        0        0    17365 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/invalid.ipynb
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/invalid_cell_id.ipynb
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/invalid_unique_cell_id.ipynb
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/many_tracebacks.ipynb
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/no_min_version.ipynb
+-rw-r--r--   0        0        0    46130 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/test2.ipynb
+-rw-r--r--   0        0        0    15875 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/test3.ipynb
+-rw-r--r--   0        0        0    15843 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/test3_no_metadata.ipynb
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/test3_no_min_version.ipynb
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/test3_no_worksheets.ipynb
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/test3_worksheet_with_no_cells.ipynb
+-rw-r--r--   0        0        0    16074 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/test4.5.ipynb
+-rw-r--r--   0        0        0    17400 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/test4.ipynb
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/test4custom.ipynb
+-rw-r--r--   0        0        0    17485 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/test4docinfo.ipynb
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/test4jupyter_metadata.ipynb
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/test4jupyter_metadata_timings.ipynb
+-rw-r--r--   0        0        0    18282 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/test4plus.ipynb
+-rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/test_api.py
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/test_convert.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/test_nbformat.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/test_reader.py
+-rw-r--r--   0        0        0     9318 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/test_sign.py
+-rw-r--r--   0        0        0    11973 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/test_validator.py
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/v4_5_invalid_metadata.ipynb
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/v4_5_no_cell_id.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/v1/__init__.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/v1/nbexamples.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/v1/test_json.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/v1/test_nbbase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/v2/__init__.py
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/v2/nbexamples.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/v2/test_json.py
+-rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/v2/test_nbbase.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/v2/test_nbpy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/v3/__init__.py
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/v3/formattest.py
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/v3/nbexamples.py
+-rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/v3/test_json.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/v3/test_misc.py
+-rw-r--r--   0        0        0     6005 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/v3/test_nbbase.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/v3/test_nbpy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/v4/__init__.py
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/v4/formattest.py
+-rw-r--r--   0        0        0     3717 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/v4/nbexamples.py
+-rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/v4/test_convert.py
+-rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/v4/test_json.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/v4/test_nbbase.py
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 nbformat-5.9.0/tests/v4/test_validate.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 nbformat-5.9.0/.gitignore
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 nbformat-5.9.0/LICENSE
+-rw-r--r--   0        0        0     5547 2020-02-02 00:00:00.000000 nbformat-5.9.0/pyproject.toml
+-rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 nbformat-5.9.0/PKG-INFO
```

### Comparing `nbformat-5.8.0/.mailmap` & `nbformat-5.9.0/.mailmap`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/.pre-commit-config.yaml` & `nbformat-5.9.0/.pre-commit-config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -16,27 +16,27 @@
       - id: check-toml
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: trailing-whitespace
 
   - repo: https://github.com/python-jsonschema/check-jsonschema
-    rev: 0.21.0
+    rev: 0.22.0
     hooks:
       - id: check-github-workflows
 
   - repo: https://github.com/executablebooks/mdformat
     rev: 0.7.16
     hooks:
       - id: mdformat
 
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.254
+    rev: v0.0.263
     hooks:
       - id: ruff
         args: ["--fix"]
         exclude: script
```

### Comparing `nbformat-5.8.0/CHANGELOG.md` & `nbformat-5.9.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,31 @@
 (changelog)=
 
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 5.9.0
+
+([Full Changelog](https://github.com/jupyter/nbformat/compare/v5.8.0...1b5e8e4e9af98f9c9b0843ba155b8756103d094d))
+
+### Maintenance and upkeep improvements
+
+- Support Python 3.12 [#363](https://github.com/jupyter/nbformat/pull/363) ([@blink1073](https://github.com/blink1073))
+- Use local coverage [#360](https://github.com/jupyter/nbformat/pull/360) ([@blink1073](https://github.com/blink1073))
+- Bump actions/checkout from 2 to 3 [#350](https://github.com/jupyter/nbformat/pull/350) ([@dependabot](https://github.com/dependabot))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyter/nbformat/graphs/contributors?from=2023-03-20&to=2023-05-31&type=c))
+
+[@blink1073](https://github.com/search?q=repo%3Ajupyter%2Fnbformat+involves%3Ablink1073+updated%3A2023-03-20..2023-05-31&type=Issues) | [@dependabot](https://github.com/search?q=repo%3Ajupyter%2Fnbformat+involves%3Adependabot+updated%3A2023-03-20..2023-05-31&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter%2Fnbformat+involves%3Apre-commit-ci+updated%3A2023-03-20..2023-05-31&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 5.8.0
 
 ([Full Changelog](https://github.com/jupyter/nbformat/compare/v5.7.3...85917af9c77beae326531e1923e0ec47725e590b))
 
 ### Enhancements made
 
 - Add strip_invalid_metadata argument to validator normalize method [#355](https://github.com/jupyter/nbformat/pull/355) ([@jonabc](https://github.com/jonabc))
@@ -25,16 +43,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyter/nbformat/graphs/contributors?from=2023-01-12&to=2023-03-20&type=c))
 
 [@blink1073](https://github.com/search?q=repo%3Ajupyter%2Fnbformat+involves%3Ablink1073+updated%3A2023-01-12..2023-03-20&type=Issues) | [@dcsaba89](https://github.com/search?q=repo%3Ajupyter%2Fnbformat+involves%3Adcsaba89+updated%3A2023-01-12..2023-03-20&type=Issues) | [@jonabc](https://github.com/search?q=repo%3Ajupyter%2Fnbformat+involves%3Ajonabc+updated%3A2023-01-12..2023-03-20&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter%2Fnbformat+involves%3Apre-commit-ci+updated%3A2023-01-12..2023-03-20&type=Issues) | [@rschroll](https://github.com/search?q=repo%3Ajupyter%2Fnbformat+involves%3Arschroll+updated%3A2023-01-12..2023-03-20&type=Issues) | [@westurner](https://github.com/search?q=repo%3Ajupyter%2Fnbformat+involves%3Awesturner+updated%3A2023-01-12..2023-03-20&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 5.7.3
 
 ([Full Changelog](https://github.com/jupyter/nbformat/compare/v5.7.2...1eefc29edff5da06f78c0087e7c06e644a6abcc9))
 
 ### Maintenance and upkeep improvements
 
 - Undeprecate validate(nb, relax_add_props=True) [#343](https://github.com/jupyter/nbformat/pull/343) ([@minrk](https://github.com/minrk))
```

### Comparing `nbformat-5.8.0/CONTRIBUTING.md` & `nbformat-5.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/README.md` & `nbformat-5.9.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # nbformat: Jupyter Notebook Format
 
-[![codecov.io](https://codecov.io/github/jupyter/nbformat/coverage.svg?branch=main)](https://codecov.io/github/jupyter/nbformat/coverage.svg?branch=main)
 ![CI Tests](https://github.com/jupyter/nbformat/workflows/Run%20tests/badge.svg)
 
 `nbformat` contains the reference implementation of the [Jupyter Notebook format],
 and Python APIs for working with notebooks.
 
 There is also a JSON Schema for nbformat versions >= 3.
```

### Comparing `nbformat-5.8.0/RELEASING.md` & `nbformat-5.9.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/package.json` & `nbformat-5.9.0/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {"'version'": "'5.9.0'"}*

```diff
@@ -17,9 +17,9 @@
     "license": "BSD-3-Clause",
     "main": "index.js",
     "name": "nbformat-schema",
     "repository": {
         "type": "git",
         "url": "git+https://github.com/jupyter/nbformat.git"
     },
-    "version": "5.8.0"
+    "version": "5.9.0"
 }
```

### Comparing `nbformat-5.8.0/.github/scripts/parse_ref.py` & `nbformat-5.9.0/.github/scripts/parse_ref.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,13 +21,13 @@
     current_ref: str
         The github reference string.
     """
     if not current_ref.startswith("refs/tags/"):
         raise Exception(f"Invalid ref `{current_ref}`!")  # noqa
 
     tag_name = current_ref.replace("refs/tags/", "")
-    print(tag_name)
+    print(tag_name)  # noqa
 
 
 if __name__ == "__main__":
     current_ref = os.environ.get("GITHUB_REF")
     parse_ref(current_ref)
```

### Comparing `nbformat-5.8.0/.github/workflows/prep-release.yml` & `nbformat-5.9.0/.github/workflows/prep-release.yml`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/.github/workflows/publish-release.yml` & `nbformat-5.9.0/.github/workflows/publish-release.yml`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/.github/workflows/tests.yml` & `nbformat-5.9.0/.github/workflows/tests.yml`

 * *Files 14% similar despite different names*

```diff
@@ -15,24 +15,24 @@
   tests:
     runs-on: ${{ matrix.os }}
     timeout-minutes: 20
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest, windows-latest, macos-latest]
-        python-version: ["3.7", "3.11"]
+        python-version: ["3.8", "3.11"]
         include:
           - os: windows-latest
             python-version: "3.9"
           - os: ubuntu-latest
             python-version: "pypy-3.8"
           - os: ubuntu-latest
-            python-version: "3.10"
+            python-version: "3.12.0-beta.1"
           - os: macos-latest
-            python-version: "3.8"
+            python-version: "3.10"
     steps:
       - uses: actions/checkout@v3
       - uses: jupyterlab/maintainer-tools/.github/actions/base-setup@v1
       - name: Run the tests
         if: ${{ !startsWith(matrix.python-version, 'pypy') && !startsWith(matrix.os, 'windows') }}
         run: |
           hatch run cov:test --cov-fail-under 75 || hatch run test:test --lf
@@ -40,19 +40,26 @@
         if: ${{ startsWith(matrix.python-version, 'pypy') }}
         run: |
           hatch run test:nowarn || hatch run test:nowarn --lf
       - name: Run the tests on windows
         if: ${{ startsWith(matrix.os, 'windows') }}
         run: |
           hatch run cov:nowarn || hatch run test:nowarn --lf
-      - name: Code coverage
-        run: |
-          pip install codecov coverage[toml]
-          codecov
       - run: hatch version 100.100.100
+      - uses: jupyterlab/maintainer-tools/.github/actions/upload-coverage@v1
+
+  coverage:
+    runs-on: ubuntu-latest
+    needs:
+      - tests
+    steps:
+      - uses: actions/checkout@v3
+      - uses: jupyterlab/maintainer-tools/.github/actions/report-coverage@v1
+        with:
+          fail_under: 77
 
   test_lint:
     name: Test Lint
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - uses: jupyterlab/maintainer-tools/.github/actions/base-setup@v1
@@ -72,44 +79,44 @@
         run: hatch run docs:build
 
   test_minimum_versions:
     name: Test Minimum Versions
     timeout-minutes: 20
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Base Setup
         uses: jupyterlab/maintainer-tools/.github/actions/base-setup@v1
         with:
           dependency_type: minimum
       - name: Run the unit tests
         run: |
           hatch run test:nowarn || hatch run test:nowarn --lf
 
   test_prereleases:
     name: Test Prereleases
     runs-on: ubuntu-latest
     timeout-minutes: 20
     steps:
       - name: Checkout
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
       - name: Base Setup
         uses: jupyterlab/maintainer-tools/.github/actions/base-setup@v1
         with:
           dependency_type: pre
       - name: Run the tests
         run: |
           hatch run test:nowarn || hatch run test:nowarn --lf
 
   make_sdist:
     name: Make SDist
     runs-on: ubuntu-latest
     timeout-minutes: 10
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - uses: jupyterlab/maintainer-tools/.github/actions/base-setup@v1
       - uses: jupyterlab/maintainer-tools/.github/actions/make-sdist@v1
 
   test_sdist:
     runs-on: ubuntu-latest
     needs: [make_sdist]
     name: Install from SDist and Test
@@ -143,15 +150,15 @@
       - uses: jupyterlab/maintainer-tools/.github/actions/check-links@v1
         with:
           ignore_glob: "tests/*.ipynb"
 
   tests_check: # This job does nothing and is only used for the branch protection
     if: always()
     needs:
-      - tests
+      - coverage
       - test_lint
       - docs
       - test_minimum_versions
       - test_prereleases
       - check_links
       - check_release
       - test_sdist
```

### Comparing `nbformat-5.8.0/docs/Makefile` & `nbformat-5.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/docs/api.rst` & `nbformat-5.9.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/docs/conf.py` & `nbformat-5.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/docs/format_description.rst` & `nbformat-5.9.0/docs/format_description.rst`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/docs/make.bat` & `nbformat-5.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/docs/markup.rst` & `nbformat-5.9.0/docs/markup.rst`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/nbformat/__init__.py` & `nbformat-5.9.0/nbformat/__init__.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/nbformat/_imports.py` & `nbformat-5.9.0/nbformat/_imports.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/nbformat/_struct.py` & `nbformat-5.9.0/nbformat/_struct.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/nbformat/_version.py` & `nbformat-5.9.0/nbformat/_version.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/nbformat/converter.py` & `nbformat-5.9.0/nbformat/converter.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/nbformat/current.py` & `nbformat-5.9.0/nbformat/current.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 warnings.warn(
     """nbformat.current is deprecated since before nbformat 3.0
 
 - use nbformat for read/write/validate public API
 - use nbformat.vX directly to composing notebooks of a particular version
 """,
     DeprecationWarning,
+    stacklevel=2,
 )
 
 __all__ = [
     "NotebookNode",
     "new_code_cell",
     "new_text_cell",
     "new_notebook",
@@ -84,15 +85,16 @@
 
     pass
 
 
 def _warn_format():
     warnings.warn(
         """Non-JSON file support in nbformat is deprecated since nbformat 1.0.
-    Use nbconvert to create files of other formats."""
+    Use nbconvert to create files of other formats.""",
+        stacklevel=2,
     )
 
 
 def parse_py(s, **kwargs):
     """Parse a string into a (nbformat, string) tuple."""
     nbf = current_nbformat
     nbm = current_nbformat_minor
```

### Comparing `nbformat-5.8.0/nbformat/json_compat.py` & `nbformat-5.9.0/nbformat/json_compat.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/nbformat/notebooknode.py` & `nbformat-5.9.0/nbformat/notebooknode.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/nbformat/reader.py` & `nbformat-5.9.0/nbformat/reader.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/nbformat/sentinel.py` & `nbformat-5.9.0/nbformat/sentinel.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/nbformat/sign.py` & `nbformat-5.9.0/nbformat/sign.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,27 @@
 from collections import OrderedDict
 from contextlib import contextmanager
 from datetime import datetime, timezone
 from hmac import HMAC
 
 try:
     import sqlite3
+
+    # Use adapters recommended by Python 3.12 stdlib docs.
+    # https://docs.python.org/3.12/library/sqlite3.html#default-adapters-and-converters-deprecated
+    def adapt_datetime_iso(val):
+        """Adapt datetime.datetime to timezone-naive ISO 8601 date."""
+        return val.isoformat()
+
+    def convert_datetime(val):
+        """Convert ISO 8601 datetime to datetime.datetime object."""
+        return datetime.fromisoformat(val.decode())
+
+    sqlite3.register_adapter(datetime, adapt_datetime_iso)
+    sqlite3.register_converter("datetime", convert_datetime)
 except ImportError:
     try:
         from pysqlite2 import dbapi2 as sqlite3  # type:ignore[no-redef]
     except ImportError:
         sqlite3 = None  # type:ignore[assignment]
 
 from base64 import encodebytes
@@ -592,29 +605,29 @@
         with open(notebook_path, encoding="utf8") as f:
             nb = read(f, NO_CONVERT)
         self.sign_notebook(nb, notebook_path)
 
     def sign_notebook(self, nb, notebook_path="<stdin>"):
         """Sign a notebook that's been loaded"""
         if self.notary.check_signature(nb):
-            print("Notebook already signed: %s" % notebook_path)
+            print("Notebook already signed: %s" % notebook_path)  # noqa
         else:
-            print("Signing notebook: %s" % notebook_path)
+            print("Signing notebook: %s" % notebook_path)  # noqa
             self.notary.sign(nb)
 
     def generate_new_key(self):
         """Generate a new notebook signature key"""
-        print("Generating new notebook key: %s" % self.notary.secret_file)
+        print("Generating new notebook key: %s" % self.notary.secret_file)  # noqa
         self.notary._write_secret_file(os.urandom(1024))
 
     def start(self):
         """Start the trust notebook app."""
         if self.reset:
             if os.path.exists(self.notary.db_file):
-                print("Removing trusted signature cache: %s" % self.notary.db_file)
+                print("Removing trusted signature cache: %s" % self.notary.db_file)  # noqa
                 os.remove(self.notary.db_file)
             self.generate_new_key()
             return
         if not self.extra_args:
             self.log.debug("Reading notebook from stdin")
             nb_s = sys.stdin.read()
             assert isinstance(nb_s, str)  # noqa
```

### Comparing `nbformat-5.8.0/nbformat/validator.py` & `nbformat-5.9.0/nbformat/validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,16 +198,15 @@
         error = self.original
         instance = _truncate_obj(error.instance)
 
         return "\n".join(
             [
                 error.message,
                 "",
-                "Failed validating %r in %s%s:"
-                % (
+                "Failed validating {!r} in {}{}:".format(
                     error.validator,
                     self.ref or "notebook",
                     _format_as_index(list(error.relative_schema_path)[:-1]),
                 ),
                 "",
                 "On instance%s:" % _format_as_index(error.relative_path),
                 pprint.pformat(instance, width=78),
@@ -520,15 +519,15 @@
             relax_add_props=relax_add_props,
             name="jsonschema",
         )
         return validator.iter_errors(nbdict, *args)
     return iter(errors)
 
 
-def _strip_invalida_metadata(
+def _strip_invalida_metadata(  # noqa
     nbdict: Any, version: int, version_minor: int, relax_add_props: bool
 ) -> int:
     """
     This function tries to extract metadata errors from the validator and fix
     them if necessary. This mostly mean stripping unknown keys from metadata
     fields, or removing metadata fields altogether.
```

### Comparing `nbformat-5.8.0/nbformat/warnings.py` & `nbformat-5.9.0/nbformat/warnings.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/nbformat/v1/__init__.py` & `nbformat-5.9.0/nbformat/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/nbformat/v1/convert.py` & `nbformat-5.9.0/nbformat/v1/convert.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/nbformat/v1/nbbase.py` & `nbformat-5.9.0/nbformat/v1/nbbase.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/nbformat/v1/nbjson.py` & `nbformat-5.9.0/nbformat/v1/nbjson.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/nbformat/v1/rwbase.py` & `nbformat-5.9.0/nbformat/v1/rwbase.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/nbformat/v2/__init__.py` & `nbformat-5.9.0/nbformat/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/nbformat/v2/convert.py` & `nbformat-5.9.0/nbformat/v2/convert.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/nbformat/v2/nbbase.py` & `nbformat-5.9.0/nbformat/v2/nbbase.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/nbformat/v2/nbjson.py` & `nbformat-5.9.0/nbformat/v2/nbjson.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/nbformat/v2/nbpy.py` & `nbformat-5.9.0/nbformat/v2/nbpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 class PyReader(NotebookReader):
     """A Python notebook reader."""
 
     def reads(self, s, **kwargs):
         """Convert a string to a notebook."""
         return self.to_notebook(s, **kwargs)
 
-    def to_notebook(self, s, **kwargs):
+    def to_notebook(self, s, **kwargs):  # noqa
         """Convert a string to a notebook."""
         lines = s.splitlines()
         cells = []
         cell_lines: List[str] = []
         state = "codecell"
         for line in lines:
             if line.startswith("# <nbformat>") or _encoding_declaration_re.match(line):
```

### Comparing `nbformat-5.8.0/nbformat/v2/nbxml.py` & `nbformat-5.9.0/nbformat/v2/nbxml.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/nbformat/v2/rwbase.py` & `nbformat-5.9.0/nbformat/v2/rwbase.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/nbformat/v3/__init__.py` & `nbformat-5.9.0/nbformat/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/nbformat/v3/convert.py` & `nbformat-5.9.0/nbformat/v3/convert.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/nbformat/v3/nbbase.py` & `nbformat-5.9.0/nbformat/v3/nbbase.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/nbformat/v3/nbformat.v3.schema.json` & `nbformat-5.9.0/nbformat/v3/nbformat.v3.schema.json`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/nbformat/v3/nbjson.py` & `nbformat-5.9.0/nbformat/v3/nbjson.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/nbformat/v3/nbpy.py` & `nbformat-5.9.0/nbformat/v3/nbpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             cell = self.new_cell(state, cell_lines)
             if cell is not None:
                 cells.append(cell)
         ws = new_worksheet(cells=cells)
         nb = new_notebook(worksheets=[ws])
         return nb
 
-    def new_cell(self, state, lines, **kwargs):
+    def new_cell(self, state, lines, **kwargs):  # noqa
         """Create a new cell."""
         if state == "codecell":
             input_ = "\n".join(lines)
             input_ = input_.strip("\n")
             if input_:
                 return new_code_cell(input=input_)
         elif state == "htmlcell":
@@ -163,15 +163,15 @@
             yield "\n".join(lines[starts[i] : starts[i + 1]]).strip("\n")
         yield "\n".join(lines[starts[-1] :]).strip("\n")
 
 
 class PyWriter(NotebookWriter):
     """A Python notebook writer."""
 
-    def writes(self, nb, **kwargs):
+    def writes(self, nb, **kwargs):  # noqa
         """Convert a notebook to a string."""
         lines = ["# -*- coding: utf-8 -*-"]
         lines.extend(
             [
                 "# <nbformat>%i.%i</nbformat>" % (nbformat, nbformat_minor),
                 "",
             ]
```

### Comparing `nbformat-5.8.0/nbformat/v3/rwbase.py` & `nbformat-5.9.0/nbformat/v3/rwbase.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/nbformat/v4/__init__.py` & `nbformat-5.9.0/nbformat/v4/__init__.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/nbformat/v4/convert.py` & `nbformat-5.9.0/nbformat/v4/convert.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/nbformat/v4/nbbase.py` & `nbformat-5.9.0/nbformat/v4/nbbase.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/nbformat/v4/nbformat.v4.0.schema.json` & `nbformat-5.9.0/nbformat/v4/nbformat.v4.0.schema.json`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/nbformat/v4/nbformat.v4.1.schema.json` & `nbformat-5.9.0/nbformat/v4/nbformat.v4.1.schema.json`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/nbformat/v4/nbformat.v4.2.schema.json` & `nbformat-5.9.0/nbformat/v4/nbformat.v4.2.schema.json`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/nbformat/v4/nbformat.v4.3.schema.json` & `nbformat-5.9.0/nbformat/v4/nbformat.v4.3.schema.json`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/nbformat/v4/nbformat.v4.4.schema.json` & `nbformat-5.9.0/nbformat/v4/nbformat.v4.4.schema.json`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/nbformat/v4/nbformat.v4.5.schema.json` & `nbformat-5.9.0/nbformat/v4/nbformat.v4.5.schema.json`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/nbformat/v4/nbformat.v4.schema.json` & `nbformat-5.9.0/nbformat/v4/nbformat.v4.schema.json`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/nbformat/v4/nbjson.py` & `nbformat-5.9.0/nbformat/v4/nbjson.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/nbformat/v4/rwbase.py` & `nbformat-5.9.0/nbformat/v4/rwbase.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/tests/invalid.ipynb` & `nbformat-5.9.0/tests/invalid.ipynb`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/tests/invalid_cell_id.ipynb` & `nbformat-5.9.0/tests/invalid_cell_id.ipynb`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/tests/invalid_unique_cell_id.ipynb` & `nbformat-5.9.0/tests/invalid_unique_cell_id.ipynb`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/tests/many_tracebacks.ipynb` & `nbformat-5.9.0/tests/many_tracebacks.ipynb`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/tests/test2.ipynb` & `nbformat-5.9.0/tests/test2.ipynb`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/tests/test3.ipynb` & `nbformat-5.9.0/tests/test3.ipynb`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/tests/test3_no_metadata.ipynb` & `nbformat-5.9.0/tests/test3_no_metadata.ipynb`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/tests/test4.5.ipynb` & `nbformat-5.9.0/tests/test4.5.ipynb`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/tests/test4.ipynb` & `nbformat-5.9.0/tests/test4.ipynb`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/tests/test4custom.ipynb` & `nbformat-5.9.0/tests/test4custom.ipynb`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/tests/test4docinfo.ipynb` & `nbformat-5.9.0/tests/test4docinfo.ipynb`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/tests/test4jupyter_metadata_timings.ipynb` & `nbformat-5.9.0/tests/test4jupyter_metadata_timings.ipynb`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/tests/test4plus.ipynb` & `nbformat-5.9.0/tests/test4plus.ipynb`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/tests/test_api.py` & `nbformat-5.9.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/tests/test_convert.py` & `nbformat-5.9.0/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/tests/test_nbformat.py` & `nbformat-5.9.0/tests/test_nbformat.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/tests/test_reader.py` & `nbformat-5.9.0/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/tests/test_sign.py` & `nbformat-5.9.0/tests/test_sign.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,15 @@
             self.assertNotIn("trusted", cell)
 
     def test_sign_stdin(self):
         def sign_stdin(nb):
             env = os.environ.copy()
             env["JUPYTER_DATA_DIR"] = self.data_dir
             p = Popen(
-                [sys.executable, "-m", "nbformat.sign", "--log-level=0"],
+                [sys.executable, "-m", "nbformat.sign", "--log-level=0"],  # noqa
                 stdin=PIPE,
                 stdout=PIPE,
                 env=env,
             )
             assert p.stdin is not None
             write(nb, codecs.getwriter("utf8")(p.stdin))
             p.stdin.close()
```

### Comparing `nbformat-5.8.0/tests/test_validator.py` & `nbformat-5.9.0/tests/test_validator.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/tests/v4_5_invalid_metadata.ipynb` & `nbformat-5.9.0/tests/v4_5_invalid_metadata.ipynb`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/tests/v4_5_no_cell_id.ipynb` & `nbformat-5.9.0/tests/v4_5_no_cell_id.ipynb`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/tests/v1/test_nbbase.py` & `nbformat-5.9.0/tests/v1/test_nbbase.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/tests/v2/nbexamples.py` & `nbformat-5.9.0/tests/v2/nbexamples.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/tests/v2/test_json.py` & `nbformat-5.9.0/tests/v2/test_json.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/tests/v2/test_nbbase.py` & `nbformat-5.9.0/tests/v2/test_nbbase.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/tests/v3/formattest.py` & `nbformat-5.9.0/tests/v3/formattest.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/tests/v3/nbexamples.py` & `nbformat-5.9.0/tests/v3/nbexamples.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/tests/v3/test_json.py` & `nbformat-5.9.0/tests/v3/test_json.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/tests/v3/test_misc.py` & `nbformat-5.9.0/tests/v3/test_misc.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/tests/v3/test_nbbase.py` & `nbformat-5.9.0/tests/v3/test_nbbase.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/tests/v3/test_nbpy.py` & `nbformat-5.9.0/tests/v3/test_nbpy.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/tests/v4/formattest.py` & `nbformat-5.9.0/tests/v4/formattest.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/tests/v4/nbexamples.py` & `nbformat-5.9.0/tests/v4/nbexamples.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/tests/v4/test_convert.py` & `nbformat-5.9.0/tests/v4/test_convert.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/tests/v4/test_json.py` & `nbformat-5.9.0/tests/v4/test_json.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/tests/v4/test_nbbase.py` & `nbformat-5.9.0/tests/v4/test_nbbase.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/tests/v4/test_validate.py` & `nbformat-5.9.0/tests/v4/test_validate.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/LICENSE` & `nbformat-5.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nbformat-5.8.0/pyproject.toml` & `nbformat-5.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -11,27 +11,25 @@
 classifiers = [
     "Intended Audience :: Developers",
     "Intended Audience :: System Administrators",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11"
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dependencies = [
     "fastjsonschema",
     "jsonschema>=2.6",
     "jupyter_core",
-    "traitlets>=5.1",
-    "importlib-metadata>=3.6;python_version<\"3.8\"",
+    "traitlets>=5.1"
 ]
 
 [[project.authors]]
 name = "Jupyter Development Team"
 email = "jupyter@googlegroups.com"
 
 [project.readme]
@@ -83,15 +81,15 @@
 [tool.hatch.envs.typing]
 features = ["test"]
 dependencies = ["mypy>=0.990"]
 [tool.hatch.envs.typing.scripts]
 test = "mypy --install-types --non-interactive {args:nbformat tests}"
 
 [tool.hatch.envs.lint]
-dependencies = ["black[jupyter]==23.1.0", "mdformat>0.7", "ruff==0.0.254"]
+dependencies = ["black[jupyter]==23.3.0", "mdformat>0.7", "ruff==0.0.263"]
 detached = true
 [tool.hatch.envs.lint.scripts]
 style = [
   "ruff {args:.}",
   "black --check --diff {args:.}",
   "mdformat --check {args:*.md}"
 ]
@@ -106,14 +104,16 @@
 testpaths = [
     "tests/",
 ]
 filterwarnings = [
     "error",
     "ignore:Using or importing the ABCs from 'collections':DeprecationWarning:jsonschema",
     "module:Jupyter is migrating its paths to use standard platformdirs:DeprecationWarning",
+    # ignore pytest warnings.
+    "ignore:::_pytest",
 ]
 
 [tool.coverage.report]
 exclude_lines = [
   "pragma: no cover",
   "def __repr__",
   "if self.debug:",
@@ -188,18 +188,24 @@
 # E402 Module level import not at top of file
 # T201 `print` found
 # B007 Loop control variable `i` not used within the loop body.
 # N802 Function name `assertIn` should be lowercase
 # RUF001 contains ambiguous unicode character '–' (did you mean '-'?)
 # S101 Use of `assert` detected
 # PLR2004 Magic value used in comparison
-"tests/*" = ["B011", "F841", "C408", "E402", "T201", "B007", "N802", "RUF001", "RUF002", "S101", "PLR2004"]
+# PLC1901 `cell.source == ""` can be simplified
+"tests/*" = ["B011", "F841", "C408", "E402", "T201", "B007", "N802", "RUF001", "RUF002", "S101", "PLR2004",
+             "PLC1901"]
 # F401 `nbxml.to_notebook` imported but unused
 "nbformat/*__init__.py" = ["F401"]
 
+[tool.coverage.run]
+relative_files = true
+source = ["nbformat"]
+
 [tool.interrogate]
 ignore-init-module=true
 ignore-private=true
 ignore-semiprivate=true
 ignore-property-decorators=true
 ignore-nested-functions=true
 ignore-nested-classes=true
```

### Comparing `nbformat-5.8.0/PKG-INFO` & `nbformat-5.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbformat
-Version: 5.8.0
+Version: 5.9.0
 Summary: The Jupyter Notebook format
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
         
         - Copyright (c) 2001-2015, IPython Development Team
         - Copyright (c) 2015-, Jupyter Development Team
@@ -39,22 +39,20 @@
 Keywords: Interactive,Interpreter,Shell,Web
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: fastjsonschema
-Requires-Dist: importlib-metadata>=3.6; python_version < '3.8'
 Requires-Dist: jsonschema>=2.6
 Requires-Dist: jupyter-core
 Requires-Dist: traitlets>=5.1
 Provides-Extra: docs
 Requires-Dist: myst-parser; extra == 'docs'
 Requires-Dist: pydata-sphinx-theme; extra == 'docs'
 Requires-Dist: sphinx; extra == 'docs'
```

