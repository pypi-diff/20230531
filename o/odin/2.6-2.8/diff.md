# Comparing `tmp/odin-2.6.tar.gz` & `tmp/odin-2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odin-2.6.tar", max compression
+gzip compressed data, was "odin-2.8.tar", max compression
```

## Comparing `odin-2.6.tar` & `odin-2.8.tar`

### file list

```diff
@@ -1,120 +1,121 @@
--rw-r--r--   0        0        0     1539 2023-03-29 12:55:55.994516 odin-2.6/LICENSE
--rw-r--r--   0        0        0     7879 2023-03-29 12:55:55.994516 odin-2.6/README.rst
--rw-r--r--   0        0        0     1817 2023-03-29 12:55:55.998516 odin-2.6/pyproject.toml
--rw-r--r--   0        0        0      718 2023-03-29 12:55:55.998516 odin-2.6/src/odin/__init__.py
--rw-r--r--   0        0        0     5355 2023-03-29 12:55:55.998516 odin-2.6/src/odin/adapters.py
--rw-r--r--   0        0        0     7305 2023-03-29 12:55:55.998516 odin-2.6/src/odin/annotated_resource/__init__.py
--rw-r--r--   0        0        0      518 2023-03-29 12:55:55.998516 odin-2.6/src/odin/annotated_resource/special_fields.py
--rw-r--r--   0        0        0      791 2023-03-29 12:55:55.998516 odin-2.6/src/odin/annotated_resource/type_aliases.py
--rw-r--r--   0        0        0     8540 2023-03-29 12:55:55.998516 odin-2.6/src/odin/annotated_resource/type_resolution.py
--rw-r--r--   0        0        0      376 2023-03-29 12:55:55.998516 odin-2.6/src/odin/bases.py
--rw-r--r--   0        0        0        0 2023-03-29 12:55:55.998516 odin-2.6/src/odin/codecs/__init__.py
--rw-r--r--   0        0        0    10542 2023-03-29 12:55:55.998516 odin-2.6/src/odin/codecs/csv_codec.py
--rw-r--r--   0        0        0     2497 2023-03-29 12:55:55.998516 odin-2.6/src/odin/codecs/dict_codec.py
--rw-r--r--   0        0        0     4536 2023-03-29 12:55:55.998516 odin-2.6/src/odin/codecs/json_codec.py
--rw-r--r--   0        0        0     4269 2023-03-29 12:55:55.998516 odin-2.6/src/odin/codecs/msgpack_codec.py
--rw-r--r--   0        0        0     5870 2023-03-29 12:55:55.998516 odin-2.6/src/odin/codecs/toml_codec.py
--rw-r--r--   0        0        0     3488 2023-03-29 12:55:55.998516 odin-2.6/src/odin/codecs/xml_codec.py
--rw-r--r--   0        0        0     3948 2023-03-29 12:55:55.998516 odin-2.6/src/odin/codecs/yaml_codec.py
--rw-r--r--   0        0        0     1181 2023-03-29 12:55:55.998516 odin-2.6/src/odin/compatibility.py
--rw-r--r--   0        0        0        0 2023-03-29 12:55:55.998516 odin-2.6/src/odin/contrib/__init__.py
--rw-r--r--   0        0        0      493 2023-03-29 12:55:55.998516 odin-2.6/src/odin/contrib/arrow/__init__.py
--rw-r--r--   0        0        0     1790 2023-03-29 12:55:55.998516 odin-2.6/src/odin/contrib/arrow/fields.py
--rw-r--r--   0        0        0      146 2023-03-29 12:55:55.998516 odin-2.6/src/odin/contrib/geo/__init__.py
--rw-r--r--   0        0        0     3776 2023-03-29 12:55:55.998516 odin-2.6/src/odin/contrib/geo/datatypes.py
--rw-r--r--   0        0        0     2321 2023-03-29 12:55:55.998516 odin-2.6/src/odin/contrib/geo/fields.py
--rw-r--r--   0        0        0      115 2023-03-29 12:55:55.998516 odin-2.6/src/odin/contrib/money/__init__.py
--rw-r--r--   0        0        0    18356 2023-03-29 12:55:55.998516 odin-2.6/src/odin/contrib/money/datatypes.py
--rw-r--r--   0        0        0     1498 2023-03-29 12:55:55.998516 odin-2.6/src/odin/contrib/money/fields.py
--rw-r--r--   0        0        0      222 2023-03-29 12:55:55.998516 odin-2.6/src/odin/contrib/pint/__init__.py
--rw-r--r--   0        0        0     2027 2023-03-29 12:55:55.998516 odin-2.6/src/odin/contrib/pint/fields.py
--rw-r--r--   0        0        0      235 2023-03-29 12:55:55.998516 odin-2.6/src/odin/contrib/pint/units.py
--rw-r--r--   0        0        0       80 2023-03-29 12:55:55.998516 odin-2.6/src/odin/contrib/rich/__init__.py
--rw-r--r--   0        0        0      631 2023-03-29 12:55:55.998516 odin-2.6/src/odin/contrib/rich/theme.py
--rw-r--r--   0        0        0     1721 2023-03-29 12:55:55.998516 odin-2.6/src/odin/contrib/rich/validation_tree.py
--rw-r--r--   0        0        0     6779 2023-03-29 12:55:55.998516 odin-2.6/src/odin/contrib/sphinx/__init__.py
--rw-r--r--   0        0        0     1353 2023-03-29 12:55:55.998516 odin-2.6/src/odin/contrib/swagger/__init__.py
--rw-r--r--   0        0        0     1183 2023-03-29 12:55:55.998516 odin-2.6/src/odin/datastructures.py
--rw-r--r--   0        0        0    10223 2023-03-29 12:55:55.998516 odin-2.6/src/odin/datetimeutil.py
--rw-r--r--   0        0        0     1624 2023-03-29 12:55:55.998516 odin-2.6/src/odin/decorators.py
--rw-r--r--   0        0        0     4800 2023-03-29 12:55:55.998516 odin-2.6/src/odin/exceptions.py
--rw-r--r--   0        0        0    32453 2023-03-29 12:55:55.998516 odin-2.6/src/odin/fields/__init__.py
--rw-r--r--   0        0        0     2078 2023-03-29 12:55:55.998516 odin-2.6/src/odin/fields/base.py
--rw-r--r--   0        0        0     7864 2023-03-29 12:55:55.998516 odin-2.6/src/odin/fields/composite.py
--rw-r--r--   0        0        0     4439 2023-03-29 12:55:55.998516 odin-2.6/src/odin/fields/virtual.py
--rw-r--r--   0        0        0     4426 2023-03-29 12:55:55.998516 odin-2.6/src/odin/filtering.py
--rw-r--r--   0        0        0     1849 2023-03-29 12:55:55.998516 odin-2.6/src/odin/helpers.py
--rw-r--r--   0        0        0    34197 2023-03-29 12:55:55.998516 odin-2.6/src/odin/mapping/__init__.py
--rw-r--r--   0        0        0     2359 2023-03-29 12:55:55.998516 odin-2.6/src/odin/mapping/helpers.py
--rw-r--r--   0        0        0     9084 2023-03-29 12:55:55.998516 odin-2.6/src/odin/proxy.py
--rw-r--r--   0        0        0        0 2023-03-29 12:55:55.998516 odin-2.6/src/odin/py.typed
--rw-r--r--   0        0        0     4773 2023-03-29 12:55:55.998516 odin-2.6/src/odin/registration.py
--rw-r--r--   0        0        0    27638 2023-03-29 12:55:55.998516 odin-2.6/src/odin/resources.py
--rw-r--r--   0        0        0     1562 2023-03-29 12:55:55.998516 odin-2.6/src/odin/serializers.py
--rw-r--r--   0        0        0     9514 2023-03-29 12:55:55.998516 odin-2.6/src/odin/traversal.py
--rw-r--r--   0        0        0     8922 2023-03-29 12:55:55.998516 odin-2.6/src/odin/utils/__init__.py
--rw-r--r--   0        0        0     3725 2023-03-29 12:55:55.998516 odin-2.6/src/odin/utils/ipv6.py
--rw-r--r--   0        0        0    10333 2023-03-29 12:55:55.998516 odin-2.6/src/odin/validators.py
--rw-r--r--   0        0        0        0 2023-03-29 12:55:55.998516 odin-2.6/tests/__init__.py
--rw-r--r--   0        0        0      581 2023-03-29 12:55:55.998516 odin-2.6/tests/_helpers.py
--rw-r--r--   0        0        0        0 2023-03-29 12:55:55.998516 odin-2.6/tests/annotated_resources/__init__.py
--rw-r--r--   0        0        0    12091 2023-03-29 12:55:55.998516 odin-2.6/tests/annotated_resources/test_type_resolution.py
--rw-r--r--   0        0        0      364 2023-03-29 12:55:55.998516 odin-2.6/tests/conftest.py
--rw-r--r--   0        0        0     1778 2023-03-29 12:55:55.998516 odin-2.6/tests/contrib/test_arrow_fields.py
--rw-r--r--   0        0        0     6022 2023-03-29 12:55:55.998516 odin-2.6/tests/contrib/test_geo_datatypes.py
--rw-r--r--   0        0        0     2796 2023-03-29 12:55:55.998516 odin-2.6/tests/contrib/test_geo_fields.py
--rw-r--r--   0        0        0     2293 2023-03-29 12:55:55.998516 odin-2.6/tests/contrib/test_geo_serialisation.py
--rw-r--r--   0        0        0     3324 2023-03-29 12:55:55.998516 odin-2.6/tests/contrib/test_money_datatypes.py
--rw-r--r--   0        0        0      762 2023-03-29 12:55:55.998516 odin-2.6/tests/contrib/test_money_fields.py
--rw-r--r--   0        0        0      941 2023-03-29 12:55:55.998516 odin-2.6/tests/contrib/test_money_serialisation.py
--rw-r--r--   0        0        0     1216 2023-03-29 12:55:55.998516 odin-2.6/tests/contrib/test_pint_fields.py
--rw-r--r--   0        0        0      433 2023-03-29 12:55:55.998516 odin-2.6/tests/contrib/test_sphinx.py
--rw-r--r--   0        0        0      301 2023-03-29 12:55:55.998516 odin-2.6/tests/fixtures/book-incorrect.toml
--rw-r--r--   0        0        0      720 2023-03-29 12:55:55.998516 odin-2.6/tests/fixtures/book-invalid.json
--rw-r--r--   0        0        0      303 2023-03-29 12:55:56.002516 odin-2.6/tests/fixtures/book-invalid.toml
--rw-r--r--   0        0        0      354 2023-03-29 12:55:56.002516 odin-2.6/tests/fixtures/book-invalid.yaml
--rw-r--r--   0        0        0      642 2023-03-29 12:55:56.002516 odin-2.6/tests/fixtures/book-valid.json
--rw-r--r--   0        0        0      325 2023-03-29 12:55:56.002516 odin-2.6/tests/fixtures/book-valid.toml
--rw-r--r--   0        0        0      453 2023-03-29 12:55:56.002516 odin-2.6/tests/fixtures/book-valid.xml
--rw-r--r--   0        0        0      357 2023-03-29 12:55:56.002516 odin-2.6/tests/fixtures/book-valid.yaml
--rw-r--r--   0        0        0      469 2023-03-29 12:55:56.002516 odin-2.6/tests/fixtures/library-header-alt-order.csv
--rw-r--r--   0        0        0      442 2023-03-29 12:55:56.002516 odin-2.6/tests/fixtures/library-invalid.csv
--rw-r--r--   0        0        0      441 2023-03-29 12:55:56.002516 odin-2.6/tests/fixtures/library-last-bad.csv
--rw-r--r--   0        0        0      441 2023-03-29 12:55:56.002516 odin-2.6/tests/fixtures/library-lower-header.csv
--rw-r--r--   0        0        0      389 2023-03-29 12:55:56.002516 odin-2.6/tests/fixtures/library-no-header.csv
--rw-r--r--   0        0        0      441 2023-03-29 12:55:56.002516 odin-2.6/tests/fixtures/library-valid.csv
--rw-r--r--   0        0        0     2543 2023-03-29 12:55:56.002516 odin-2.6/tests/fixtures/library.json
--rw-r--r--   0        0        0     1948 2023-03-29 12:55:56.002516 odin-2.6/tests/fixtures/library.yaml
--rw-r--r--   0        0        0     6148 2023-03-29 12:55:56.002516 odin-2.6/tests/resources.py
--rw-r--r--   0        0        0     2340 2023-03-29 12:55:56.002516 odin-2.6/tests/resources_annotated.py
--rw-r--r--   0        0        0     3925 2023-03-29 12:55:56.002516 odin-2.6/tests/test_adapters.py
--rw-r--r--   0        0        0     3125 2023-03-29 12:55:56.002516 odin-2.6/tests/test_annotated_resources.py
--rw-r--r--   0        0        0     7037 2023-03-29 12:55:56.002516 odin-2.6/tests/test_codec_csv.py
--rw-r--r--   0        0        0     3016 2023-03-29 12:55:56.002516 odin-2.6/tests/test_codec_dict.py
--rw-r--r--   0        0        0     2672 2023-03-29 12:55:56.002516 odin-2.6/tests/test_codec_json.py
--rw-r--r--   0        0        0     2688 2023-03-29 12:55:56.002516 odin-2.6/tests/test_codec_msgpack.py
--rw-r--r--   0        0        0     6254 2023-03-29 12:55:56.002516 odin-2.6/tests/test_codec_toml.py
--rw-r--r--   0        0        0     2156 2023-03-29 12:55:56.002516 odin-2.6/tests/test_codec_xml.py
--rw-r--r--   0        0        0     2227 2023-03-29 12:55:56.002516 odin-2.6/tests/test_codec_yaml.py
--rw-r--r--   0        0        0     1110 2023-03-29 12:55:56.002516 odin-2.6/tests/test_compatibility.py
--rw-r--r--   0        0        0     1793 2023-03-29 12:55:56.002516 odin-2.6/tests/test_datastructures.py
--rw-r--r--   0        0        0    11626 2023-03-29 12:55:56.002516 odin-2.6/tests/test_datetimeutil.py
--rw-r--r--   0        0        0     1069 2023-03-29 12:55:56.002516 odin-2.6/tests/test_decorators.py
--rw-r--r--   0        0        0     2072 2023-03-29 12:55:56.002516 odin-2.6/tests/test_exceptions.py
--rw-r--r--   0        0        0    48489 2023-03-29 12:55:56.002516 odin-2.6/tests/test_fields.py
--rw-r--r--   0        0        0     9825 2023-03-29 12:55:56.002516 odin-2.6/tests/test_fields_composite.py
--rw-r--r--   0        0        0     1028 2023-03-29 12:55:56.002516 odin-2.6/tests/test_fields_virtual.py
--rw-r--r--   0        0        0     4564 2023-03-29 12:55:56.002516 odin-2.6/tests/test_filtering.py
--rw-r--r--   0        0        0     1734 2023-03-29 12:55:56.002516 odin-2.6/tests/test_helpers.py
--rw-r--r--   0        0        0     2534 2023-03-29 12:55:56.002516 odin-2.6/tests/test_kitchensink.py
--rw-r--r--   0        0        0    20443 2023-03-29 12:55:56.002516 odin-2.6/tests/test_mapping.py
--rw-r--r--   0        0        0      962 2023-03-29 12:55:56.002516 odin-2.6/tests/test_mapping_helpers.py
--rw-r--r--   0        0        0     1374 2023-03-29 12:55:56.002516 odin-2.6/tests/test_polymorphic.py
--rw-r--r--   0        0        0     5058 2023-03-29 12:55:56.002516 odin-2.6/tests/test_proxy.py
--rw-r--r--   0        0        0     2903 2023-03-29 12:55:56.002516 odin-2.6/tests/test_resource_base.py
--rw-r--r--   0        0        0    11673 2023-03-29 12:55:56.002516 odin-2.6/tests/test_resources.py
--rw-r--r--   0        0        0     2222 2023-03-29 12:55:56.002516 odin-2.6/tests/test_serializers.py
--rw-r--r--   0        0        0    10418 2023-03-29 12:55:56.002516 odin-2.6/tests/test_traversal.py
--rw-r--r--   0        0        0     5859 2023-03-29 12:55:56.002516 odin-2.6/tests/test_utils.py
--rw-r--r--   0        0        0     7620 2023-03-29 12:55:56.002516 odin-2.6/tests/test_validators.py
--rw-r--r--   0        0        0     9735 1970-01-01 00:00:00.000000 odin-2.6/PKG-INFO
+-rw-r--r--   0        0        0     1539 2023-05-30 23:59:27.722059 odin-2.8/LICENSE
+-rw-r--r--   0        0        0     7879 2023-05-30 23:59:27.722059 odin-2.8/README.rst
+-rw-r--r--   0        0        0     2489 2023-05-30 23:59:27.722059 odin-2.8/pyproject.toml
+-rw-r--r--   0        0        0      718 2023-05-30 23:59:27.722059 odin-2.8/src/odin/__init__.py
+-rw-r--r--   0        0        0     5356 2023-05-30 23:59:27.722059 odin-2.8/src/odin/adapters.py
+-rw-r--r--   0        0        0     7306 2023-05-30 23:59:27.722059 odin-2.8/src/odin/annotated_resource/__init__.py
+-rw-r--r--   0        0        0      518 2023-05-30 23:59:27.722059 odin-2.8/src/odin/annotated_resource/special_fields.py
+-rw-r--r--   0        0        0      791 2023-05-30 23:59:27.722059 odin-2.8/src/odin/annotated_resource/type_aliases.py
+-rw-r--r--   0        0        0     8701 2023-05-30 23:59:27.722059 odin-2.8/src/odin/annotated_resource/type_resolution.py
+-rw-r--r--   0        0        0      376 2023-05-30 23:59:27.722059 odin-2.8/src/odin/bases.py
+-rw-r--r--   0        0        0        0 2023-05-30 23:59:27.722059 odin-2.8/src/odin/codecs/__init__.py
+-rw-r--r--   0        0        0    10541 2023-05-30 23:59:27.722059 odin-2.8/src/odin/codecs/csv_codec.py
+-rw-r--r--   0        0        0     2480 2023-05-30 23:59:27.722059 odin-2.8/src/odin/codecs/dict_codec.py
+-rw-r--r--   0        0        0     4547 2023-05-30 23:59:27.726059 odin-2.8/src/odin/codecs/json_codec.py
+-rw-r--r--   0        0        0     4264 2023-05-30 23:59:27.726059 odin-2.8/src/odin/codecs/msgpack_codec.py
+-rw-r--r--   0        0        0     5899 2023-05-30 23:59:27.726059 odin-2.8/src/odin/codecs/toml_codec.py
+-rw-r--r--   0        0        0     3115 2023-05-30 23:59:27.726059 odin-2.8/src/odin/codecs/xml_codec.py
+-rw-r--r--   0        0        0     3970 2023-05-30 23:59:27.726059 odin-2.8/src/odin/codecs/yaml_codec.py
+-rw-r--r--   0        0        0     1249 2023-05-30 23:59:27.726059 odin-2.8/src/odin/compatibility.py
+-rw-r--r--   0        0        0        0 2023-05-30 23:59:27.726059 odin-2.8/src/odin/contrib/__init__.py
+-rw-r--r--   0        0        0      503 2023-05-30 23:59:27.726059 odin-2.8/src/odin/contrib/arrow/__init__.py
+-rw-r--r--   0        0        0     1791 2023-05-30 23:59:27.726059 odin-2.8/src/odin/contrib/arrow/fields.py
+-rw-r--r--   0        0        0      146 2023-05-30 23:59:27.726059 odin-2.8/src/odin/contrib/geo/__init__.py
+-rw-r--r--   0        0        0     3765 2023-05-30 23:59:27.726059 odin-2.8/src/odin/contrib/geo/datatypes.py
+-rw-r--r--   0        0        0     2370 2023-05-30 23:59:27.726059 odin-2.8/src/odin/contrib/geo/fields.py
+-rw-r--r--   0        0        0      115 2023-05-30 23:59:27.726059 odin-2.8/src/odin/contrib/money/__init__.py
+-rw-r--r--   0        0        0    18131 2023-05-30 23:59:27.726059 odin-2.8/src/odin/contrib/money/datatypes.py
+-rw-r--r--   0        0        0     1585 2023-05-30 23:59:27.726059 odin-2.8/src/odin/contrib/money/fields.py
+-rw-r--r--   0        0        0      222 2023-05-30 23:59:27.726059 odin-2.8/src/odin/contrib/pint/__init__.py
+-rw-r--r--   0        0        0     2182 2023-05-30 23:59:27.726059 odin-2.8/src/odin/contrib/pint/fields.py
+-rw-r--r--   0        0        0      245 2023-05-30 23:59:27.726059 odin-2.8/src/odin/contrib/pint/units.py
+-rw-r--r--   0        0        0       80 2023-05-30 23:59:27.726059 odin-2.8/src/odin/contrib/rich/__init__.py
+-rw-r--r--   0        0        0      631 2023-05-30 23:59:27.726059 odin-2.8/src/odin/contrib/rich/theme.py
+-rw-r--r--   0        0        0     1662 2023-05-30 23:59:27.726059 odin-2.8/src/odin/contrib/rich/validation_tree.py
+-rw-r--r--   0        0        0     6787 2023-05-30 23:59:27.726059 odin-2.8/src/odin/contrib/sphinx/__init__.py
+-rw-r--r--   0        0        0     1309 2023-05-30 23:59:27.726059 odin-2.8/src/odin/contrib/swagger/__init__.py
+-rw-r--r--   0        0        0     1183 2023-05-30 23:59:27.726059 odin-2.8/src/odin/datastructures.py
+-rw-r--r--   0        0        0    10233 2023-05-30 23:59:27.726059 odin-2.8/src/odin/datetimeutil.py
+-rw-r--r--   0        0        0     1624 2023-05-30 23:59:27.726059 odin-2.8/src/odin/decorators.py
+-rw-r--r--   0        0        0     4800 2023-05-30 23:59:27.726059 odin-2.8/src/odin/exceptions.py
+-rw-r--r--   0        0        0    33799 2023-05-30 23:59:27.726059 odin-2.8/src/odin/fields/__init__.py
+-rw-r--r--   0        0        0     2078 2023-05-30 23:59:27.726059 odin-2.8/src/odin/fields/base.py
+-rw-r--r--   0        0        0     8102 2023-05-30 23:59:27.726059 odin-2.8/src/odin/fields/composite.py
+-rw-r--r--   0        0        0     4479 2023-05-30 23:59:27.726059 odin-2.8/src/odin/fields/virtual.py
+-rw-r--r--   0        0        0     4426 2023-05-30 23:59:27.726059 odin-2.8/src/odin/filtering.py
+-rw-r--r--   0        0        0     1849 2023-05-30 23:59:27.726059 odin-2.8/src/odin/helpers.py
+-rw-r--r--   0        0        0    34236 2023-05-30 23:59:27.726059 odin-2.8/src/odin/mapping/__init__.py
+-rw-r--r--   0        0        0     2359 2023-05-30 23:59:27.726059 odin-2.8/src/odin/mapping/helpers.py
+-rw-r--r--   0        0        0     8940 2023-05-30 23:59:27.726059 odin-2.8/src/odin/proxy.py
+-rw-r--r--   0        0        0        0 2023-05-30 23:59:27.726059 odin-2.8/src/odin/py.typed
+-rw-r--r--   0        0        0     4781 2023-05-30 23:59:27.726059 odin-2.8/src/odin/registration.py
+-rw-r--r--   0        0        0    27572 2023-05-30 23:59:27.726059 odin-2.8/src/odin/resources.py
+-rw-r--r--   0        0        0     1562 2023-05-30 23:59:27.726059 odin-2.8/src/odin/serializers.py
+-rw-r--r--   0        0        0     9572 2023-05-30 23:59:27.726059 odin-2.8/src/odin/traversal.py
+-rw-r--r--   0        0        0     8910 2023-05-30 23:59:27.726059 odin-2.8/src/odin/utils/__init__.py
+-rw-r--r--   0        0        0     3725 2023-05-30 23:59:27.726059 odin-2.8/src/odin/utils/ipv6.py
+-rw-r--r--   0        0        0    10342 2023-05-30 23:59:27.726059 odin-2.8/src/odin/validators.py
+-rw-r--r--   0        0        0        0 2023-05-30 23:59:27.726059 odin-2.8/tests/__init__.py
+-rw-r--r--   0        0        0      582 2023-05-30 23:59:27.726059 odin-2.8/tests/_helpers.py
+-rw-r--r--   0        0        0        0 2023-05-30 23:59:27.726059 odin-2.8/tests/annotated_resources/__init__.py
+-rw-r--r--   0        0        0    12091 2023-05-30 23:59:27.726059 odin-2.8/tests/annotated_resources/test_type_resolution.py
+-rw-r--r--   0        0        0      429 2023-05-30 23:59:27.726059 odin-2.8/tests/conftest.py
+-rw-r--r--   0        0        0     1779 2023-05-30 23:59:27.726059 odin-2.8/tests/contrib/test_arrow_fields.py
+-rw-r--r--   0        0        0     6023 2023-05-30 23:59:27.726059 odin-2.8/tests/contrib/test_geo_datatypes.py
+-rw-r--r--   0        0        0     2797 2023-05-30 23:59:27.726059 odin-2.8/tests/contrib/test_geo_fields.py
+-rw-r--r--   0        0        0     2293 2023-05-30 23:59:27.726059 odin-2.8/tests/contrib/test_geo_serialisation.py
+-rw-r--r--   0        0        0     3323 2023-05-30 23:59:27.726059 odin-2.8/tests/contrib/test_money_datatypes.py
+-rw-r--r--   0        0        0      733 2023-05-30 23:59:27.726059 odin-2.8/tests/contrib/test_money_fields.py
+-rw-r--r--   0        0        0      911 2023-05-30 23:59:27.726059 odin-2.8/tests/contrib/test_money_serialisation.py
+-rw-r--r--   0        0        0     1216 2023-05-30 23:59:27.726059 odin-2.8/tests/contrib/test_pint_fields.py
+-rw-r--r--   0        0        0      433 2023-05-30 23:59:27.726059 odin-2.8/tests/contrib/test_sphinx.py
+-rw-r--r--   0        0        0      301 2023-05-30 23:59:27.726059 odin-2.8/tests/fixtures/book-incorrect.toml
+-rw-r--r--   0        0        0      720 2023-05-30 23:59:27.726059 odin-2.8/tests/fixtures/book-invalid.json
+-rw-r--r--   0        0        0      303 2023-05-30 23:59:27.726059 odin-2.8/tests/fixtures/book-invalid.toml
+-rw-r--r--   0        0        0      354 2023-05-30 23:59:27.726059 odin-2.8/tests/fixtures/book-invalid.yaml
+-rw-r--r--   0        0        0      642 2023-05-30 23:59:27.726059 odin-2.8/tests/fixtures/book-valid.json
+-rw-r--r--   0        0        0      325 2023-05-30 23:59:27.726059 odin-2.8/tests/fixtures/book-valid.toml
+-rw-r--r--   0        0        0      453 2023-05-30 23:59:27.726059 odin-2.8/tests/fixtures/book-valid.xml
+-rw-r--r--   0        0        0      357 2023-05-30 23:59:27.726059 odin-2.8/tests/fixtures/book-valid.yaml
+-rw-r--r--   0        0        0      469 2023-05-30 23:59:27.726059 odin-2.8/tests/fixtures/library-header-alt-order.csv
+-rw-r--r--   0        0        0     2503 2023-05-30 23:59:27.726059 odin-2.8/tests/fixtures/library-invalid-nested.json
+-rw-r--r--   0        0        0      442 2023-05-30 23:59:27.726059 odin-2.8/tests/fixtures/library-invalid.csv
+-rw-r--r--   0        0        0      441 2023-05-30 23:59:27.726059 odin-2.8/tests/fixtures/library-last-bad.csv
+-rw-r--r--   0        0        0      441 2023-05-30 23:59:27.726059 odin-2.8/tests/fixtures/library-lower-header.csv
+-rw-r--r--   0        0        0      389 2023-05-30 23:59:27.726059 odin-2.8/tests/fixtures/library-no-header.csv
+-rw-r--r--   0        0        0      441 2023-05-30 23:59:27.726059 odin-2.8/tests/fixtures/library-valid.csv
+-rw-r--r--   0        0        0     2543 2023-05-30 23:59:27.726059 odin-2.8/tests/fixtures/library.json
+-rw-r--r--   0        0        0     1948 2023-05-30 23:59:27.726059 odin-2.8/tests/fixtures/library.yaml
+-rw-r--r--   0        0        0     6147 2023-05-30 23:59:27.726059 odin-2.8/tests/resources.py
+-rw-r--r--   0        0        0     2339 2023-05-30 23:59:27.726059 odin-2.8/tests/resources_annotated.py
+-rw-r--r--   0        0        0     3922 2023-05-30 23:59:27.726059 odin-2.8/tests/test_adapters.py
+-rw-r--r--   0        0        0     3124 2023-05-30 23:59:27.726059 odin-2.8/tests/test_annotated_resources.py
+-rw-r--r--   0        0        0     7033 2023-05-30 23:59:27.726059 odin-2.8/tests/test_codec_csv.py
+-rw-r--r--   0        0        0     3018 2023-05-30 23:59:27.726059 odin-2.8/tests/test_codec_dict.py
+-rw-r--r--   0        0        0     2673 2023-05-30 23:59:27.726059 odin-2.8/tests/test_codec_json.py
+-rw-r--r--   0        0        0     2689 2023-05-30 23:59:27.726059 odin-2.8/tests/test_codec_msgpack.py
+-rw-r--r--   0        0        0     6256 2023-05-30 23:59:27.726059 odin-2.8/tests/test_codec_toml.py
+-rw-r--r--   0        0        0     2157 2023-05-30 23:59:27.726059 odin-2.8/tests/test_codec_xml.py
+-rw-r--r--   0        0        0     2228 2023-05-30 23:59:27.726059 odin-2.8/tests/test_codec_yaml.py
+-rw-r--r--   0        0        0     1143 2023-05-30 23:59:27.726059 odin-2.8/tests/test_compatibility.py
+-rw-r--r--   0        0        0     1793 2023-05-30 23:59:27.726059 odin-2.8/tests/test_datastructures.py
+-rw-r--r--   0        0        0    11627 2023-05-30 23:59:27.726059 odin-2.8/tests/test_datetimeutil.py
+-rw-r--r--   0        0        0     1070 2023-05-30 23:59:27.726059 odin-2.8/tests/test_decorators.py
+-rw-r--r--   0        0        0     2072 2023-05-30 23:59:27.726059 odin-2.8/tests/test_exceptions.py
+-rw-r--r--   0        0        0    48478 2023-05-30 23:59:27.730059 odin-2.8/tests/test_fields.py
+-rw-r--r--   0        0        0     9825 2023-05-30 23:59:27.730059 odin-2.8/tests/test_fields_composite.py
+-rw-r--r--   0        0        0     1028 2023-05-30 23:59:27.730059 odin-2.8/tests/test_fields_virtual.py
+-rw-r--r--   0        0        0     4564 2023-05-30 23:59:27.730059 odin-2.8/tests/test_filtering.py
+-rw-r--r--   0        0        0     1735 2023-05-30 23:59:27.730059 odin-2.8/tests/test_helpers.py
+-rw-r--r--   0        0        0     3176 2023-05-30 23:59:27.730059 odin-2.8/tests/test_kitchensink.py
+-rw-r--r--   0        0        0    20443 2023-05-30 23:59:27.730059 odin-2.8/tests/test_mapping.py
+-rw-r--r--   0        0        0      963 2023-05-30 23:59:27.730059 odin-2.8/tests/test_mapping_helpers.py
+-rw-r--r--   0        0        0     1374 2023-05-30 23:59:27.730059 odin-2.8/tests/test_polymorphic.py
+-rw-r--r--   0        0        0     5058 2023-05-30 23:59:27.730059 odin-2.8/tests/test_proxy.py
+-rw-r--r--   0        0        0     2904 2023-05-30 23:59:27.730059 odin-2.8/tests/test_resource_base.py
+-rw-r--r--   0        0        0    11513 2023-05-30 23:59:27.730059 odin-2.8/tests/test_resources.py
+-rw-r--r--   0        0        0     2206 2023-05-30 23:59:27.730059 odin-2.8/tests/test_serializers.py
+-rw-r--r--   0        0        0    10433 2023-05-30 23:59:27.730059 odin-2.8/tests/test_traversal.py
+-rw-r--r--   0        0        0     5860 2023-05-30 23:59:27.730059 odin-2.8/tests/test_utils.py
+-rw-r--r--   0        0        0     7619 2023-05-30 23:59:27.730059 odin-2.8/tests/test_validators.py
+-rw-r--r--   0        0        0     9536 1970-01-01 00:00:00.000000 odin-2.8/PKG-INFO
```

### Comparing `odin-2.6/LICENSE` & `odin-2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `odin-2.6/README.rst` & `odin-2.8/README.rst`

 * *Files identical despite different names*

### Comparing `odin-2.6/src/odin/__init__.py` & `odin-2.8/src/odin/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Disable logging if an explicit handler is not added
 import logging
 
 logging.getLogger("odin.registration").addHandler(logging.NullHandler())
 
 from odin import exceptions  # noqa
+from odin.adapters import ResourceAdapter  # noqa
+from odin.annotated_resource import *  # noqa
+from odin.annotated_resource import type_aliases as types  # noqa
 from odin.fields import *  # noqa
 from odin.fields.composite import *  # noqa
 from odin.fields.virtual import *  # noqa
+from odin.helpers import *  # noqa
 from odin.mapping import *  # noqa
-from odin.resources import Resource  # noqa
-from odin.adapters import ResourceAdapter  # noqa
 from odin.proxy import ResourceProxy  # noqa
-from odin.annotated_resource import *  # noqa
-from odin.annotated_resource import type_aliases as types  # noqa
-from odin.helpers import *  # noqa
+from odin.resources import Resource  # noqa
 
 __authors__ = "Tim Savage <tim@savage.company>"
 __copyright__ = "Copyright (C) 2021 Tim Savage"
```

### Comparing `odin-2.6/src/odin/adapters.py` & `odin-2.8/src/odin/adapters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from functools import cached_property
+
 from odin.utils import field_iter_items, getmeta
 
 __all__ = ("ResourceAdapter",)
 
 
 class CurriedAdapter:
     """Curry wrapper for an Adapter to allow for pre-config of include/exclude and
```

### Comparing `odin-2.6/src/odin/annotated_resource/__init__.py` & `odin-2.8/src/odin/annotated_resource/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,26 +8,27 @@
 Annotated resources still utilise many of the existing classes eg
 ``ResourceBase``, ``ResourceOptions`` and all existing fields. Allowing
 existing code (eg Mappings, Codecs) including custom implementations to be
 utilised unchanged.
 
 """
 import copy
-from typing import Any, Dict, Tuple, Type, Optional, TypeVar, Iterable
+from typing import Any, Dict, Iterable, Optional, Tuple, Type, TypeVar
 
 from odin import registration
 from odin.fields import BaseField
 from odin.resources import (
-    ResourceBase,
-    ResourceOptions,
     DEFAULT_TYPE_FIELD,
     NotProvided,
+    ResourceBase,
+    ResourceOptions,
 )
-from .type_resolution import process_attribute, Options
+
 from ..exceptions import ResourceDefError
+from .type_resolution import Options, process_attribute
 
 __all__ = (
     "Options",
     "AnnotatedResourceType",
     "AnnotatedResource",
     "AResource",
 )
```

### Comparing `odin-2.6/src/odin/annotated_resource/special_fields.py` & `odin-2.8/src/odin/annotated_resource/special_fields.py`

 * *Files identical despite different names*

### Comparing `odin-2.6/src/odin/annotated_resource/type_aliases.py` & `odin-2.8/src/odin/annotated_resource/type_aliases.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Type aliases for string formatted types."""
-from typing import Callable, Union, Any, Sequence, Tuple
+from typing import Any, Callable, Sequence, Tuple, Union
 
 __all__ = (
     "Email",
     "IPv4",
     "IPv6",
     "IPv46",
     "Url",
```

### Comparing `odin-2.6/src/odin/annotated_resource/type_resolution.py` & `odin-2.8/src/odin/annotated_resource/type_resolution.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,71 @@
 """Methods for resolving types to fields."""
 import datetime
 import enum
 import pathlib
 import re
 import uuid
-from typing import Any, Sequence, Dict, Type, Union, get_origin, List, Final
+from typing import Any, Dict, Final, List, Sequence, Type, Union, get_origin
 
 try:
     # Handle the change in typing between 3.8 and later releases
-    from typing import T, KT, VT
+    from typing import KT, VT, T
 except ImportError:
     T = None
     KT = None
     VT = None
 
 import odin
-from .special_fields import AnyField
-from .type_aliases import Validator, Choices, Email, IPv4, IPv6, IPv46, Url
-from .. import ListOf, DictOf
+
 from ..exceptions import ResourceDefError
 from ..fields import (
     BaseField,
+    BooleanField,
+    DateField,
+    DateTimeField,
+    DictField,
+    EmailField,
     Field,
+    FloatField,
+    IntegerField,
+    IPv4Field,
+    IPv6Field,
+    IPv46Field,
+    ListField,
     NotProvided,
-    TypedListField,
+    PathField,
+    RegexField,
+    StringField,
+    TimeField,
     TypedDictField,
-    ListField,
-    DictField,
+    TypedListField,
+    UrlField,
+    UUIDField,
 )
+from ..fields.composite import DictOf, ListOf
 from ..fields.virtual import ConstantField
 from ..resources import ResourceBase
+from .special_fields import AnyField
+from .type_aliases import Choices, Email, IPv4, IPv6, IPv46, Url, Validator
 
 
 class Options:
     """Define options for a field"""
 
     __slots__ = (
         "field_type",
         "base_args",
         "field_args",
         "extra_args",
     )
 
     def __init__(
         self,
-        default: Any = odin.NotProvided,
-        field_type: Type[odin.BaseField] = None,
+        default: Any = NotProvided,
+        field_type: Type[BaseField] = None,
         *,
         verbose_name: str = None,
         verbose_name_plural: str = None,
         name: str = None,
         validators: Sequence[Validator] = None,
         choices: Choices = None,
         use_default_if_not_provided: bool = True,
@@ -108,31 +124,31 @@
                 raise
         raise ResourceDefError(
             f"Field type `{self.base_args.get('name', 'Unknown!')}` could not be resolved"
         )
 
 
 SIMPLE_TYPE_MAP = {
-    bool: odin.BooleanField,
-    datetime.date: odin.DateField,
-    datetime.datetime: odin.DateTimeField,
-    dict: odin.DictField,
-    Email: odin.EmailField,
-    float: odin.FloatField,
-    int: odin.IntegerField,
-    IPv4: odin.IPv4Field,
-    IPv6: odin.IPv6Field,
-    IPv46: odin.IPv46Field,
-    list: odin.ListField,
-    pathlib.Path: odin.PathField,
-    re.Pattern: odin.RegexField,
-    str: odin.StringField,
-    datetime.time: odin.TimeField,
-    Url: odin.UrlField,
-    uuid.UUID: odin.UUIDField,
+    bool: BooleanField,
+    datetime.date: DateField,
+    datetime.datetime: DateTimeField,
+    dict: DictField,
+    Email: EmailField,
+    float: FloatField,
+    int: IntegerField,
+    IPv4: IPv4Field,
+    IPv6: IPv6Field,
+    IPv46: IPv46Field,
+    list: ListField,
+    pathlib.Path: PathField,
+    re.Pattern: RegexField,
+    str: StringField,
+    datetime.time: TimeField,
+    Url: UrlField,
+    uuid.UUID: UUIDField,
     Any: AnyField,  # For Python 3.11
 }
 
 
 def _resolve_field_from_type(options: Options, type_: type):
     """Resolve a field from a basic type"""
     if field_type := SIMPLE_TYPE_MAP.get(type_, None):
@@ -219,15 +235,15 @@
             pass  # Resolve
 
     elif origin is Final:
         # Constant
         options.field_type = ConstantField
         value = options.field_args["default"]
         if value is NotProvided:
-            raise ResourceDefError(f"Final fields require a value")
+            raise ResourceDefError("Final fields require a value")
         options.base_args["value"] = value
         return
 
     elif issubclass(origin, List):
         return _resolve_list_from_sub_scripted_type(args, options)
 
     elif issubclass(origin, Dict):
```

### Comparing `odin-2.6/src/odin/codecs/csv_codec.py` & `odin-2.8/src/odin/codecs/csv_codec.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 
 """
 import csv
 from io import StringIO
 
 from odin import bases
 from odin.datastructures import CaseLessStringList
+from odin.exceptions import CodecDecodeError, ValidationError
 from odin.fields import NotProvided
 from odin.resources import create_resource_from_iter
 from odin.utils import getmeta, lazy_property
-from odin.exceptions import CodecDecodeError, ValidationError
 
 CONTENT_TYPE = "text/csv"
 
 
 class Reader(bases.TypedResourceIterable):
     """
     Customisable reader object.
@@ -97,15 +97,15 @@
         # Configure header
         if self.includes_header:
             self.header = self._read_header()
 
             # Handle strict fields
             if self.strict_fields and self.extra_field_names:
                 raise CodecDecodeError(
-                    "Extra unknown fields: {0}".format(",".join(self.extra_field_names))
+                    "Extra unknown fields: {}".format(",".join(self.extra_field_names))
                 )
 
         # Built in counters
         self.row_count = None
         self.error_count = None
 
     def __iter__(self):
```

### Comparing `odin-2.6/src/odin/codecs/dict_codec.py` & `odin-2.8/src/odin/codecs/dict_codec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-from odin import bases
-from odin import resources, ResourceAdapter
+from odin import ResourceAdapter, bases, resources
 from odin.utils import getmeta
 
-
 TYPE_SERIALIZERS = {}
 
 
 class OdinEncoder:
     def __init__(self, include_virtual_fields=True, include_type_field=True):
         self.include_virtual_fields = include_virtual_fields
         self.include_type_field = include_type_field
```

### Comparing `odin-2.6/src/odin/codecs/json_codec.py` & `odin-2.8/src/odin/codecs/json_codec.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import datetime
 import typing
 import uuid
 
-from odin import bases
-from odin import serializers, resources, ResourceAdapter
+from odin import ResourceAdapter, bases, resources, serializers
 from odin.exceptions import CodecDecodeError, CodecEncodeError
 from odin.utils import getmeta
 
 try:
     import simplejson as json
 except ImportError:
     import json
@@ -37,18 +36,21 @@
     def default(self, o):
         if isinstance(o, (resources.ResourceBase, ResourceAdapter)):
             meta = getmeta(o)
             obj = o.to_dict(self.include_virtual_fields)
             if self.include_type_field:
                 obj[meta.type_field] = meta.resource_name
             return obj
+
         elif isinstance(o, LIST_TYPES):
             return list(o)
+
         elif o.__class__ in JSON_TYPES:
             return JSON_TYPES[o.__class__](o)
+
         return super().default(o)
 
 
 def load(fp, resource=None, full_clean=True, default_to_not_supplied=False):
     """
     Load a from a JSON encoded file.
 
@@ -85,38 +87,38 @@
 
     """
     try:
         return resources.build_object_graph(
             json.loads(s), resource, full_clean, False, default_to_not_supplied
         )
     except (ValueError, TypeError) as ex:
-        raise CodecDecodeError(str(ex))
+        raise CodecDecodeError(str(ex)) from ex
 
 
 def dump(resource, fp, cls=OdinEncoder, **kwargs):
     """
     Dump to a JSON encoded file.
 
     :param resource: The root resource to dump to a JSON encoded file.
     :param cls: Encoder to use serializing to a string; default is the :py:class:`OdinEncoder`.
     :param fp: The file pointer that represents the output file.
 
     """
     try:
         json.dump(resource, fp, cls=cls, **kwargs)
     except ValueError as ex:
-        raise CodecEncodeError(str(ex))
+        raise CodecEncodeError(str(ex)) from ex
 
 
 def dumps(resource, cls=OdinEncoder, **kwargs):
     """
     Dump to a JSON encoded string.
 
     :param resource: The root resource to dump to a JSON encoded file.
     :param cls: Encoder to use serializing to a string; default is the :py:class:`OdinEncoder`.
     :returns: JSON encoded string.
 
     """
     try:
         return json.dumps(resource, cls=cls, **kwargs)
     except ValueError as ex:
-        raise CodecEncodeError(str(ex))
+        raise CodecEncodeError(str(ex)) from ex
```

### Comparing `odin-2.6/src/odin/codecs/msgpack_codec.py` & `odin-2.8/src/odin/codecs/msgpack_codec.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,19 @@
 from typing import TextIO
 
 try:
     import msgpack
 except ImportError:
     raise ImportError(
         "odin.codecs.msgpack_codec requires the 'msgpack-python' package."
-    )  # noqa
+    ) from None  # noqa
 
-from odin import bases
-from odin import serializers, resources, ResourceAdapter
+from odin import ResourceAdapter, bases, resources, serializers
 from odin.utils import getmeta
 
-
 TYPE_SERIALIZERS = {
     datetime.date: serializers.date_iso_format,
     datetime.time: serializers.time_iso_format,
     datetime.datetime: serializers.datetime_iso_format,
     uuid.UUID: str,
 }
 CONTENT_TYPE = "application/x-msgpack"
@@ -34,16 +32,18 @@
 
     def default(self, o):
         if isinstance(o, (resources.ResourceBase, ResourceAdapter)):
             meta = getmeta(o)
             obj = o.to_dict(self.include_virtual_fields)
             obj[meta.type_field] = meta.resource_name
             return obj
+
         elif isinstance(o, bases.ResourceIterable):
             return list(o)
+
         elif o.__class__ in TYPE_SERIALIZERS:
             return TYPE_SERIALIZERS[o.__class__](o)
 
 
 def load(
     fp: TextIO,
     resource: resources.ResourceBase = None,
```

### Comparing `odin-2.6/src/odin/codecs/toml_codec.py` & `odin-2.8/src/odin/codecs/toml_codec.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from typing import Union, Sequence, Dict, Optional, Type
+from typing import Dict, Optional, Sequence, Type, Union
 
-from odin import resources, ResourceAdapter
+from odin import ResourceAdapter, resources
 from odin.exceptions import CodecDecodeError
 from odin.resources import ResourceBase
 from odin.utils import getmeta
 
 try:
     import toml
 except ImportError:  # pragma: no cover
     raise ImportError(  # pragma: no cover
         "odin.codecs.toml_codec requires the 'toml' package."
-    )
+    ) from None
 
 
 TOML_TYPES = {}
 CONTENT_TYPE = "application/toml"
 
 
 def load(fp, resource=None, full_clean=True, default_to_not_supplied=False):
@@ -35,15 +35,16 @@
     :returns: A resource object or object graph of resources loaded from file.
 
     """
 
     try:
         data = toml.load(fp)
     except toml.TomlDecodeError as ex:
-        raise CodecDecodeError(str(ex))
+        raise CodecDecodeError(str(ex)) from ex
+
     return resources.build_object_graph(
         data,
         resource,
         full_clean,
         False,
         default_to_not_supplied,
     )
@@ -66,15 +67,16 @@
     :returns: A resource object or object graph of resources loaded from file.
 
     """
 
     try:
         data = toml.loads(s)
     except toml.TomlDecodeError as ex:
-        raise CodecDecodeError(str(ex))
+        raise CodecDecodeError(str(ex)) from ex
+
     return resources.build_object_graph(
         data,
         resource,
         full_clean,
         False,
         default_to_not_supplied,
     )
@@ -101,14 +103,15 @@
             resource_dict[meta.type_field] = meta.resource_name
         return resource_dict
 
     def dump_value(self, v):
         if isinstance(v, (ResourceBase, ResourceAdapter)):
             resource_dict = self.resource_to_dict(v)
             return self.dump_inline_table(resource_dict)
+
         if type(v) in TOML_TYPES:
             v = TOML_TYPES[type(v)](v)
         return super().dump_value(v)
 
 
 RT = Union[
     ResourceBase,
```

### Comparing `odin-2.6/src/odin/codecs/xml_codec.py` & `odin-2.8/src/odin/codecs/xml_codec.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,17 +15,16 @@
 
 """
 import datetime
 from io import StringIO
 from typing import TextIO
 from xml.sax import saxutils
 
-from odin import serializers, Resource
-from odin import fields
-from odin.fields import composite, StringField
+from odin import fields, serializers
+from odin.fields import StringField, composite
 from odin.utils import attribute_field_iter_items, element_field_iter_items, getmeta
 
 XML_TYPES = {
     datetime.date: serializers.date_iso_format,
     datetime.time: serializers.time_iso_format,
     datetime.datetime: serializers.datetime_iso_format,
 }
@@ -45,74 +44,61 @@
     else:
         return str(value)
 
 
 def dump(
     fp: TextIO,
     resource,  # type: Resource
-    line_ending="",  # type: str
+    line_ending: str = "",
 ):
     """
     Dump a resource to a file like object.
     :param fp: File pointer or file like object.
     :param resource: Resource to dump
     :param line_ending: End of line character to apply
     """
     meta = getmeta(resource)
 
     # Write container and any attributes
     attributes = "".join(
-        " {}={}".format(
-            f.name, saxutils.quoteattr(_serialize_to_string(v))
-        )  # Encode attributes
+        f" {f.name}={saxutils.quoteattr(_serialize_to_string(v))}"  # Encode attributes
         for f, v in attribute_field_iter_items(resource)
     )
-    fp.write("<{}{}>{}".format(meta.name, attributes, line_ending))
+    fp.write(f"<{meta.name}{attributes}>{line_ending}")
 
     # Write any element fields
     for field, value in element_field_iter_items(resource):
         if isinstance(field, composite.ListOf):
             if field.use_container:
-                fp.write("<{}>{}".format(field.name, line_ending))
+                fp.write(f"<{field.name}>{line_ending}")
             for v in value:
                 dump(fp, v, line_ending)
             if field.use_container:
-                fp.write("</{}>{}".format(field.name, line_ending))
+                fp.write(f"</{field.name}>{line_ending}")
 
         elif isinstance(field, composite.DictAs):
             if value is not None:
                 dump(fp, value, line_ending)
 
         elif isinstance(field, fields.ArrayField):
             for v in value:
                 fp.write(
-                    "<{}>{}</{}>{}".format(
-                        field.name, _serialize_to_string(v), field.name, line_ending
-                    )
+                    f"<{field.name}>{_serialize_to_string(v)}</{field.name}>{line_ending}"
                 )
 
         elif isinstance(field, TextField):
             if value is not None:
-                fp.write(
-                    "{}{}".format(
-                        saxutils.escape(_serialize_to_string(value)), line_ending
-                    )
-                )
+                fp.write(f"{saxutils.escape(_serialize_to_string(value))}{line_ending}")
 
         else:
             fp.write(
-                "<{}>{}</{}>{}".format(
-                    field.name,
-                    saxutils.escape(_serialize_to_string(value)),
-                    field.name,
-                    line_ending,
-                )
+                f"<{field.name}>{saxutils.escape(_serialize_to_string(value))}</{field.name}>{line_ending}"
             )
 
-    fp.write("</{}>{}".format(meta.name, line_ending))
+    fp.write(f"</{meta.name}>{line_ending}")
 
 
 def dumps(resource, **kwargs):
     """
     Dump a resource to a string.
 
     :param resource: Resource to dump
```

### Comparing `odin-2.6/src/odin/codecs/yaml_codec.py` & `odin-2.8/src/odin/codecs/yaml_codec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """Codec to load/save Yaml documents."""
-from typing import TextIO, Union
 from io import StringIO
+from typing import TextIO, Union
 
-from odin import bases
-from odin import resources, ResourceAdapter
+from odin import ResourceAdapter, bases, resources
 from odin.exceptions import CodecEncodeError
 from odin.utils import getmeta
 
 try:
     import yaml
 except ImportError:
     raise ImportError(  # pragma: no cover
         "odin.codecs.yaml_codec requires the 'pyyaml' package."
-    )
+    ) from None
 
 try:
-    from yaml import CSafeLoader as SafeLoader, CSafeDumper as SafeDumper
+    from yaml import CSafeDumper as SafeDumper
+    from yaml import CSafeLoader as SafeLoader
 except ImportError:
-    from yaml import SafeLoader, SafeDumper  # pragma: no cover
+    from yaml import SafeDumper, SafeLoader  # pragma: no cover
 
 
 YAML_TYPES = {}
 CONTENT_TYPE = "application/x-yaml"
 
 
 class OdinDumper(SafeDumper):
@@ -92,15 +92,15 @@
     :param dumper: Dumper to use serializing to a string; default is the :py:class:`OdinDumper`.
     :param fp: The file pointer that represents the output file.
 
     """
     try:
         yaml.dump(resource, fp, Dumper=dumper, **kwargs)
     except ValueError as ex:
-        raise CodecEncodeError(str(ex))
+        raise CodecEncodeError(str(ex)) from ex
 
 
 def dumps(resource: resources.ResourceBase, dumper=OdinDumper, **kwargs) -> str:
     """Dump to a YAML encoded string.
 
     :param resource: The root resource to dump to a YAML encoded file.
     :param dumper: Dumper to use serializing to a string; default is the :py:class:`OdinDumper`.
```

### Comparing `odin-2.6/src/odin/compatibility.py` & `odin-2.8/src/odin/compatibility.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,25 +17,27 @@
         if inspect.isclass(obj):
             old_init = obj.__init__
 
             def wrapped_init(*args, **kwargs):
                 warnings.warn(
                     f"{obj.__name__} is deprecated and scheduled for removal. {message}",
                     category=category,
+                    stacklevel=2,
                 )
                 return old_init(*args, **kwargs)
 
             obj.__init__ = wrapped_init
             return obj
 
         else:
 
             def wrapped_func(*args, **kwargs):
                 warnings.warn(
                     f"{obj.__name__} is deprecated and scheduled for removal. {message}",
                     category=category,
+                    stacklevel=2,
                 )
                 return obj(*args, **kwargs)
 
             return wrapped_func
 
     return wrap
```

### Comparing `odin-2.6/src/odin/contrib/arrow/fields.py` & `odin-2.8/src/odin/contrib/arrow/fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-import arrow
 import datetime
 
-from odin import exceptions, datetimeutil
+import arrow
+
+from odin import datetimeutil, exceptions
 from odin.fields import Field
 from odin.validators import EMPTY_VALUES
 
 __all__ = ("ArrowField",)
 
 
 class ArrowField(Field):
```

### Comparing `odin-2.6/src/odin/contrib/geo/datatypes.py` & `odin-2.8/src/odin/contrib/geo/datatypes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import math
+from typing import Tuple
 
 __all__ = ("latitude", "longitude", "latlng", "point")
 
-from typing import Tuple
-
 
-def to_dms(value, absolute=False):
-    # type: (float, bool) -> Tuple[float, float, float]
+def to_dms(value: float, absolute: bool = False) -> Tuple[float, float, float]:
     """
     Split a float value into DMS (degree, minute, second) parts
 
     :param value: Float value to split
     :param absolute: Obtain the absolute value
     :return: tuple containing DMS values
 
@@ -20,16 +18,15 @@
     degree = int(math.floor(value))
     value = (value - degree) * 60
     minute = int(math.floor(value))
     second = (value - minute) * 60
     return (-degree if invert else degree), minute, second
 
 
-def to_dm(value, absolute=False):
-    # type: (float, bool) -> Tuple[float, float]
+def to_dm(value: float, absolute: bool = False) -> Tuple[float, float]:
     """
     Split a float value into DM (degree, minute) parts
 
     :param value: Float value to split
     :param absolute: Obtain the absolute value
     :return: tuple containing DM values
 
@@ -61,15 +58,15 @@
     """
     A longitude value. A longitude is a value between -180.0 and 180.0.
     """
 
     def __new__(cls, x):
         lng = float.__new__(cls, x)
         if lng > 180.0 or lng < -180.0:
-            raise ValueError("not in range -180.0 -> 180.0: '{}'".format(x))
+            raise ValueError(f"not in range -180.0 -> 180.0: '{x}'")
         return lng
 
     def __str__(self):
         result = "{:03d}°{:02d}'{:02f}\"".format(*to_dms(self, True))
         return result + ("W" if self < 0 else "E")
 
 
@@ -81,15 +78,15 @@
     def __new__(cls, *args):
         # Unpack a tuple, list or latlng instance.
         if len(args) == 1 and isinstance(args[0], (tuple, list)):
             args = args[0]
         try:
             lat, lng = args
         except ValueError:
-            raise TypeError(f"latlng() takes 2 arguments ({len(args)} given)")
+            raise TypeError(f"latlng() takes 2 arguments ({len(args)} given)") from None
         return tuple.__new__(cls, (latitude(lat), longitude(lng)))
 
     @property
     def lat(self):
         return self[0]
 
     @property
@@ -125,15 +122,15 @@
         return self[1]
 
     @property
     def z(self):
         try:
             return self[2]
         except IndexError:
-            raise AttributeError("2D points do not include a z axis.")
+            raise AttributeError("2D points do not include a z axis.") from None
 
     @property
     def is_3d(self):
         return len(self) == 3
 
     def __repr__(self):
         return ("point({}, {}, {})" if self.is_3d else "point({}, {})").format(*self)
```

### Comparing `odin-2.6/src/odin/contrib/geo/fields.py` & `odin-2.8/src/odin/contrib/geo/fields.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,82 +1,91 @@
 from odin import exceptions
 from odin.fields import Field, ScalarField
 from odin.validators import EMPTY_VALUES
-from .datatypes import latitude, longitude, latlng, point
 
-__all__ = ('LatitudeField', 'LongitudeField', 'LatLngField', 'PointField')
+from .datatypes import latitude, latlng, longitude, point
+
+__all__ = ("LatitudeField", "LongitudeField", "LatLngField", "PointField")
 
 
 class LatitudeField(ScalarField):
     """
     Field that contains a latitude value.
     """
+
     default_error_messages = {
-        'invalid': "'%s' value must be a latitude.",
+        "invalid": "'%s' value must be a latitude.",
     }
     data_type_name = "Latitude"
 
     def to_python(self, value):
         if value in EMPTY_VALUES:
             return
         try:
             return latitude(value)
+
         except (ValueError, TypeError):
-            msg = self.error_messages['invalid'] % value
-            raise exceptions.ValidationError(msg)
+            msg = self.error_messages["invalid"] % value
+            raise exceptions.ValidationError(msg) from None
 
 
 class LongitudeField(ScalarField):
     """
     Field that contains a longitude value.
     """
+
     default_error_messages = {
-        'invalid': "'%s' value must be a longitude.",
+        "invalid": "'%s' value must be a longitude.",
     }
     data_type_name = "Longitude"
 
     def to_python(self, value):
         if value in EMPTY_VALUES:
             return
         try:
             return longitude(value)
+
         except (ValueError, TypeError):
-            msg = self.error_messages['invalid'] % value
-            raise exceptions.ValidationError(msg)
+            msg = self.error_messages["invalid"] % value
+            raise exceptions.ValidationError(msg) from None
 
 
 class LatLngField(Field):
     """
     Field that contains a lat/long pair.
     """
+
     default_error_messages = {
-        'invalid': "'%s' value must be a (latitude, longitude).",
+        "invalid": "'%s' value must be a (latitude, longitude).",
     }
     data_type_name = "LatLng"
 
     def to_python(self, value):
         if value in EMPTY_VALUES:
             return
         try:
             return latlng(value)
+
         except (ValueError, TypeError):
-            msg = self.error_messages['invalid'] % value
-            raise exceptions.ValidationError(msg)
+            msg = self.error_messages["invalid"] % value
+            raise exceptions.ValidationError(msg) from None
 
 
 class PointField(Field):
     """
     Field that contains a point in cartesian space. This can be either 2D (on a plain) or 3D (includes a z-axis).
     """
+
     default_error_messages = {
-        'invalid': "'%s' value must be a point in 2D or 3D cartesian space.",
+        "invalid": "'%s' value must be a point in 2D or 3D cartesian space.",
     }
     data_type_name = "Point"
 
     def to_python(self, value):
         if value in EMPTY_VALUES:
             return
         try:
             return point(value)
+
         except (ValueError, TypeError):
-            msg = self.error_messages['invalid'] % value
-            raise exceptions.ValidationError(msg)
+            msg = self.error_messages["invalid"] % value
+            raise exceptions.ValidationError(msg) from None
```

### Comparing `odin-2.6/src/odin/contrib/money/datatypes.py` & `odin-2.8/src/odin/contrib/money/datatypes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 import decimal
-
 from collections import namedtuple
 
 __all__ = ("Currency", "set_default_currency", "Amount", "NO_CURRENCY")
 
 
 class Currency(namedtuple("Currency", "code number name symbol precision")):
-    def __new__(cls, code, number, name="", symbol=u"", precision=2):
-        return super(Currency, cls).__new__(cls, code, number, name, symbol, precision)
+    def __new__(cls, code, number, name="", symbol="", precision=2):
+        return super().__new__(cls, code, number, name, symbol, precision)
 
     def __eq__(self, other):
         if isinstance(other, Currency):
             return self.code == other.code
         if isinstance(other, str):
             return self.code == other
         return NotImplemented
 
     def __repr__(self):
-        return "Currency({!r}, {!r})".format(self.code, self.number)
+        return f"Currency({self.code!r}, {self.number!r})"
 
     def __str__(self):
         if self.name:
-            return "{} - {}".format(self.name, self.code)
+            return f"{self.name} - {self.code}"
         else:
             return self.code
 
 
 CURRENCY = {}
 # XXX is the currency code for no currency in ISO 4217
 CURRENCY["XXX"] = DEFAULT_CURRENCY = NO_CURRENCY = Currency(
@@ -52,32 +51,32 @@
         if isinstance(value, (tuple, list)):
             if len(value) == 1:
                 value = value[0]
             elif len(value) == 2:
                 value, currency = value
             else:
                 raise ValueError(
-                    "expected tuple with a length of 1 or 2 got: {}".format(len(value))
+                    f"expected tuple with a length of 1 or 2 got: {len(value)}"
                 )
 
         if not isinstance(value, decimal.Decimal):
             try:
                 value = decimal.Decimal(value)
             except decimal.InvalidOperation:
                 raise ValueError(
-                    "value is not a valid numerical amount: {}".format(value)
-                )
+                    f"value is not a valid numerical amount: {value}"
+                ) from None
 
         if currency is None:
             currency = DEFAULT_CURRENCY
         elif isinstance(currency, str):
             currency = CURRENCY[currency.upper()]
         elif not isinstance(currency, Currency):
             raise TypeError(
-                "unable to convert value into a valid currency: {}".format(currency)
+                f"unable to convert value into a valid currency: {currency}"
             )
 
         return tuple.__new__(cls, (value, currency))
 
     # Type conversions
 
     def __float__(self):
@@ -220,15 +219,15 @@
 
         :param format_string:
         :return: formatted string
 
         """
         assert isinstance(format_string, str)
         return format_string.format(
-            value=("{{0:0.{:d}f}}".format(self.currency.precision)).format(self.value),
+            value=(f"{{0:0.{self.currency.precision:d}f}}").format(self.value),
             value_raw=self.value,
             currency=self.currency,
         )
 
     def assign_currency(self, currency):
         """
         Assign a currency if this amount currently has no currency assigned.
@@ -242,179 +241,179 @@
         if not self.is_naive:
             raise ValueError("This amount is already assigned a currency.")
         return Amount(self.value, CURRENCY[currency])
 
 
 # Currencies based off the latest ISO 4217 list of currencies
 # Updated: 2014-08-29
-CURRENCY["AED"] = Currency("AED", 784, "UAE Dirham", u"", 2)
-CURRENCY["AFN"] = Currency("AFN", 971, "Afghani", u"؋", 2)
-CURRENCY["ALL"] = Currency("ALL", 8, "Lek", u"", 2)
-CURRENCY["AMD"] = Currency("AMD", 51, "Armenian Dram", u"", 2)
-CURRENCY["ANG"] = Currency("ANG", 532, "Netherlands Antillean Guilder", u"ƒ", 2)
-CURRENCY["AOA"] = Currency("AOA", 973, "Kwanza", u"", 2)
-CURRENCY["ARS"] = Currency("ARS", 32, "Argentine Peso", u"$", 2)
-CURRENCY["AUD"] = Currency("AUD", 36, "Australian Dollar", u"$", 2)
-CURRENCY["AWG"] = Currency("AWG", 533, "Aruban Florin", u"ƒ", 2)
-CURRENCY["AZN"] = Currency("AZN", 944, "Azerbaijanian Manat", u"ман", 2)
-CURRENCY["BAM"] = Currency("BAM", 977, "Convertible Mark", u"KM", 2)
-CURRENCY["BBD"] = Currency("BBD", 52, "Barbados Dollar", u"$", 2)
-CURRENCY["BDT"] = Currency("BDT", 50, "Taka", u"", 2)
-CURRENCY["BGN"] = Currency("BGN", 975, "Bulgarian Lev", u"", 2)
-CURRENCY["BHD"] = Currency("BHD", 48, "Bahraini Dinar", u"", 3)
-CURRENCY["BIF"] = Currency("BIF", 108, "Burundi Franc", u"", 0)
-CURRENCY["BMD"] = Currency("BMD", 60, "Bermudian Dollar", u"", 2)
-CURRENCY["BND"] = Currency("BND", 96, "Brunei Dollar", u"$", 2)
-CURRENCY["BOB"] = Currency("BOB", 68, "Boliviano", u"", 2)
-CURRENCY["BOV"] = Currency("BOV", 984, "Mvdol", u"", 2)
-CURRENCY["BRL"] = Currency("BRL", 986, "Brazilian Real", u"", 2)
-CURRENCY["BSD"] = Currency("BSD", 44, "Bahamian Dollar", u"", 2)
-CURRENCY["BTN"] = Currency("BTN", 64, "Ngultrum", u"", 2)
-CURRENCY["BWP"] = Currency("BWP", 72, "Pula", u"P", 2)
-CURRENCY["BYR"] = Currency("BYR", 974, "Belarussian Ruble", u"p.", 0)
-CURRENCY["BZD"] = Currency("BZD", 84, "Belize Dollar", u"BZ$", 2)
-CURRENCY["CAD"] = Currency("CAD", 124, "Canadian Dollar", u"$", 2)
-CURRENCY["CDF"] = Currency("CDF", 976, "Congolese Franc", u"", 2)
-CURRENCY["CHE"] = Currency("CHE", 947, "WIR Euro", u"", 2)
-CURRENCY["CHF"] = Currency("CHF", 756, "Swiss Franc", u"CHF", 2)
-CURRENCY["CHW"] = Currency("CHW", 948, "WIR Franc", u"", 2)
-CURRENCY["CLF"] = Currency("CLF", 990, "Unidad de Fomento", u"", 4)
-CURRENCY["CLP"] = Currency("CLP", 152, "Chilean Peso", u"$", 0)
-CURRENCY["CNY"] = Currency("CNY", 156, "Yuan Renminbi", u"¥", 2)
-CURRENCY["COP"] = Currency("COP", 170, "Colombian Peso", u"$", 2)
-CURRENCY["COU"] = Currency("COU", 970, "Unidad de Valor Real", u"", 2)
-CURRENCY["CRC"] = Currency("CRC", 188, "Costa Rican Colon", u"₡", 2)
-CURRENCY["CUC"] = Currency("CUC", 931, "Peso Convertible", u"", 2)
-CURRENCY["CUP"] = Currency("CUP", 192, "Cuban Peso", u"₱", 2)
-CURRENCY["CVE"] = Currency("CVE", 132, "Cabo Verde Escudo", u"", 2)
-CURRENCY["CZK"] = Currency("CZK", 203, "Czech Koruna", u"Kč", 2)
-CURRENCY["DJF"] = Currency("DJF", 262, "Djibouti Franc", u"", 0)
-CURRENCY["DKK"] = Currency("DKK", 208, "Danish Krone", u"kr", 2)
-CURRENCY["DOP"] = Currency("DOP", 214, "Dominican Peso", u"RD$", 2)
-CURRENCY["DZD"] = Currency("DZD", 12, "Algerian Dinar", u"", 2)
-CURRENCY["EGP"] = Currency("EGP", 818, "Egyptian Pound", u"£", 2)
-CURRENCY["ERN"] = Currency("ERN", 232, "Nakfa", u"", 2)
-CURRENCY["ETB"] = Currency("ETB", 230, "Ethiopian Birr", u"", 2)
-CURRENCY["EUR"] = Currency("EUR", 978, "Euro", u"€", 2)
-CURRENCY["FJD"] = Currency("FJD", 242, "Fiji Dollar", u"$", 2)
-CURRENCY["FKP"] = Currency("FKP", 238, "Falkland Islands Pound", u"£", 2)
-CURRENCY["GBP"] = Currency("GBP", 826, "Pound Sterling", u"£", 2)
-CURRENCY["GEL"] = Currency("GEL", 981, "Lari", u"", 2)
-CURRENCY["GHS"] = Currency("GHS", 936, "Ghana Cedi", u"¢", 2)
-CURRENCY["GIP"] = Currency("GIP", 292, "Gibraltar Pound", u"£", 2)
-CURRENCY["GMD"] = Currency("GMD", 270, "Dalasi", u"", 2)
-CURRENCY["GNF"] = Currency("GNF", 324, "Guinea Franc", u"", 0)
-CURRENCY["GTQ"] = Currency("GTQ", 320, "Quetzal", u"Q", 2)
-CURRENCY["GYD"] = Currency("GYD", 328, "Guyana Dollar", u"$", 2)
-CURRENCY["HKD"] = Currency("HKD", 344, "Hong Kong Dollar", u"$", 2)
-CURRENCY["HNL"] = Currency("HNL", 340, "Lempira", u"L", 2)
-CURRENCY["HRK"] = Currency("HRK", 191, "Croatian Kuna", u"kn", 2)
-CURRENCY["HTG"] = Currency("HTG", 332, "Gourde", u"", 2)
-CURRENCY["HUF"] = Currency("HUF", 348, "Forint", u"Ft", 2)
-CURRENCY["IDR"] = Currency("IDR", 360, "Rupiah", u"Rp", 2)
-CURRENCY["ILS"] = Currency("ILS", 376, "New Israeli Sheqel", u"₪", 2)
-CURRENCY["INR"] = Currency("INR", 356, "Indian Rupee", u"₹", 2)
-CURRENCY["IQD"] = Currency("IQD", 368, "Iraqi Dinar", u"", 3)
-CURRENCY["IRR"] = Currency("IRR", 364, "Iranian Rial", u"﷼", 2)
-CURRENCY["ISK"] = Currency("ISK", 352, "Iceland Krona", u"kr", 0)
-CURRENCY["JMD"] = Currency("JMD", 388, "Jamaican Dollar", u"J$", 2)
-CURRENCY["JOD"] = Currency("JOD", 400, "Jordanian Dinar", u"", 3)
-CURRENCY["JPY"] = Currency("JPY", 392, "Yen", u"¥", 0)
-CURRENCY["KES"] = Currency("KES", 404, "Kenyan Shilling", u"", 2)
-CURRENCY["KGS"] = Currency("KGS", 417, "Som", u"лв", 2)
-CURRENCY["KHR"] = Currency("KHR", 116, "Riel", u"៛", 2)
-CURRENCY["KMF"] = Currency("KMF", 174, "Comoro Franc", u"", 0)
-CURRENCY["KPW"] = Currency("KPW", 408, "North Korean Won", u"₩", 2)
-CURRENCY["KRW"] = Currency("KRW", 410, "Won", u"₩", 0)
-CURRENCY["KWD"] = Currency("KWD", 414, "Kuwaiti Dinar", u"", 3)
-CURRENCY["KYD"] = Currency("KYD", 136, "Cayman Islands Dollar", u"$", 2)
-CURRENCY["KZT"] = Currency("KZT", 398, "Tenge", u"лв", 2)
-CURRENCY["LAK"] = Currency("LAK", 418, "Kip", u"₭", 2)
-CURRENCY["LBP"] = Currency("LBP", 422, "Lebanese Pound", u"£", 2)
-CURRENCY["LKR"] = Currency("LKR", 144, "Sri Lanka Rupee", u"₨", 2)
-CURRENCY["LRD"] = Currency("LRD", 430, "Liberian Dollar", u"$", 2)
-CURRENCY["LSL"] = Currency("LSL", 426, "Loti", u"", 2)
-CURRENCY["LTL"] = Currency("LTL", 440, "Lithuanian Litas", u"Lt", 2)
-CURRENCY["LYD"] = Currency("LYD", 434, "Libyan Dinar", u"", 3)
-CURRENCY["MAD"] = Currency("MAD", 504, "Moroccan Dirham", u"", 2)
-CURRENCY["MDL"] = Currency("MDL", 498, "Moldovan Leu", u"", 2)
-CURRENCY["MGA"] = Currency("MGA", 969, "Malagasy Ariary", u"", 2)
-CURRENCY["MKD"] = Currency("MKD", 807, "Denar", u"ден", 2)
-CURRENCY["MMK"] = Currency("MMK", 104, "Kyat", u"", 2)
-CURRENCY["MNT"] = Currency("MNT", 496, "Tugrik", u"₮", 2)
-CURRENCY["MOP"] = Currency("MOP", 446, "Pataca", u"", 2)
-CURRENCY["MRO"] = Currency("MRO", 478, "Ouguiya", u"", 2)
-CURRENCY["MUR"] = Currency("MUR", 480, "Mauritius Rupee", u"₨", 2)
-CURRENCY["MVR"] = Currency("MVR", 462, "Rufiyaa", u"", 2)
-CURRENCY["MWK"] = Currency("MWK", 454, "Kwacha", u"", 2)
-CURRENCY["MXN"] = Currency("MXN", 484, "Mexican Peso", u"$", 2)
-CURRENCY["MXV"] = Currency("MXV", 979, "Mexican Unidad de Inversion (UDI)", u"", 2)
-CURRENCY["MYR"] = Currency("MYR", 458, "Malaysian Ringgit", u"RM", 2)
-CURRENCY["MZN"] = Currency("MZN", 943, "Mozambique Metical", u"MT", 2)
-CURRENCY["NAD"] = Currency("NAD", 516, "Namibia Dollar", u"$", 2)
-CURRENCY["NGN"] = Currency("NGN", 566, "Naira", u"₦", 2)
-CURRENCY["NIO"] = Currency("NIO", 558, "Cordoba Oro", u"C$", 2)
-CURRENCY["NOK"] = Currency("NOK", 578, "Norwegian Krone", u"kr", 2)
-CURRENCY["NPR"] = Currency("NPR", 524, "Nepalese Rupee", u"₨", 2)
-CURRENCY["NZD"] = Currency("NZD", 554, "New Zealand Dollar", u"$", 2)
-CURRENCY["OMR"] = Currency("OMR", 512, "Rial Omani", u"﷼", 3)
-CURRENCY["PAB"] = Currency("PAB", 590, "Balboa", u"B/.", 2)
-CURRENCY["PEN"] = Currency("PEN", 604, "Nuevo Sol", u"S/.", 2)
-CURRENCY["PGK"] = Currency("PGK", 598, "Kina", u"", 2)
-CURRENCY["PHP"] = Currency("PHP", 608, "Philippine Peso", u"₱", 2)
-CURRENCY["PKR"] = Currency("PKR", 586, "Pakistan Rupee", u"₨", 2)
-CURRENCY["PLN"] = Currency("PLN", 985, "Zloty", u"zł", 2)
-CURRENCY["PYG"] = Currency("PYG", 600, "Guarani", u"Gs", 0)
-CURRENCY["QAR"] = Currency("QAR", 634, "Qatari Rial", u"﷼", 2)
-CURRENCY["RON"] = Currency("RON", 946, "New Romanian Leu", u"lei", 2)
-CURRENCY["RSD"] = Currency("RSD", 941, "Serbian Dinar", u"Дин.", 2)
-CURRENCY["RUB"] = Currency("RUB", 643, "Russian Ruble", u"руб", 2)
-CURRENCY["RWF"] = Currency("RWF", 646, "Rwanda Franc", u"", 0)
-CURRENCY["SAR"] = Currency("SAR", 682, "Saudi Riyal", u"", 2)
-CURRENCY["SBD"] = Currency("SBD", 90, "Solomon Islands Dollar", u"$", 2)
-CURRENCY["SCR"] = Currency("SCR", 690, "Seychelles Rupee", u"₨", 2)
-CURRENCY["SDG"] = Currency("SDG", 938, "Sudanese Pound", u"", 2)
-CURRENCY["SEK"] = Currency("SEK", 752, "Swedish Krona", u"kr", 2)
-CURRENCY["SGD"] = Currency("SGD", 702, "Singapore Dollar", u"$", 2)
-CURRENCY["SHP"] = Currency("SHP", 654, "Saint Helena Pound", u"£", 2)
-CURRENCY["SLL"] = Currency("SLL", 694, "Leone", u"", 2)
-CURRENCY["SOS"] = Currency("SOS", 706, "Somali Shilling", u"S", 2)
-CURRENCY["SRD"] = Currency("SRD", 968, "Surinam Dollar", u"$", 2)
-CURRENCY["SSP"] = Currency("SSP", 728, "South Sudanese Pound", u"", 2)
-CURRENCY["STD"] = Currency("STD", 678, "Dobra", u"", 2)
-CURRENCY["SVC"] = Currency("SVC", 222, "El Salvador Colon", u"$", 2)
-CURRENCY["SYP"] = Currency("SYP", 760, "Syrian Pound", u"£", 2)
-CURRENCY["SZL"] = Currency("SZL", 748, "Lilangeni", u"", 2)
-CURRENCY["THB"] = Currency("THB", 764, "Baht", u"฿", 2)
-CURRENCY["TJS"] = Currency("TJS", 972, "Somoni", u"", 2)
-CURRENCY["TMT"] = Currency("TMT", 934, "Turkmenistan New Manat", u"", 2)
-CURRENCY["TND"] = Currency("TND", 788, "Tunisian Dinar", u"", 3)
-CURRENCY["TOP"] = Currency("TOP", 776, "Pa’anga", u"", 2)
-CURRENCY["TRY"] = Currency("TRY", 949, "Turkish Lira", u"₤", 2)
-CURRENCY["TTD"] = Currency("TTD", 780, "Trinidad and Tobago Dollar", u"TT$", 2)
-CURRENCY["TWD"] = Currency("TWD", 901, "New Taiwan Dollar", u"NT$", 2)
-CURRENCY["TZS"] = Currency("TZS", 834, "Tanzanian Shilling", u"", 2)
-CURRENCY["UAH"] = Currency("UAH", 980, "Hryvnia", u"₴", 2)
-CURRENCY["UGX"] = Currency("UGX", 800, "Uganda Shilling", u"", 0)
-CURRENCY["USD"] = Currency("USD", 840, "US Dollar", u"$", 2)
-CURRENCY["USN"] = Currency("USN", 997, "US Dollar (Next day)", u"", 2)
+CURRENCY["AED"] = Currency("AED", 784, "UAE Dirham", "", 2)
+CURRENCY["AFN"] = Currency("AFN", 971, "Afghani", "؋", 2)
+CURRENCY["ALL"] = Currency("ALL", 8, "Lek", "", 2)
+CURRENCY["AMD"] = Currency("AMD", 51, "Armenian Dram", "", 2)
+CURRENCY["ANG"] = Currency("ANG", 532, "Netherlands Antillean Guilder", "ƒ", 2)
+CURRENCY["AOA"] = Currency("AOA", 973, "Kwanza", "", 2)
+CURRENCY["ARS"] = Currency("ARS", 32, "Argentine Peso", "$", 2)
+CURRENCY["AUD"] = Currency("AUD", 36, "Australian Dollar", "$", 2)
+CURRENCY["AWG"] = Currency("AWG", 533, "Aruban Florin", "ƒ", 2)
+CURRENCY["AZN"] = Currency("AZN", 944, "Azerbaijanian Manat", "ман", 2)
+CURRENCY["BAM"] = Currency("BAM", 977, "Convertible Mark", "KM", 2)
+CURRENCY["BBD"] = Currency("BBD", 52, "Barbados Dollar", "$", 2)
+CURRENCY["BDT"] = Currency("BDT", 50, "Taka", "", 2)
+CURRENCY["BGN"] = Currency("BGN", 975, "Bulgarian Lev", "", 2)
+CURRENCY["BHD"] = Currency("BHD", 48, "Bahraini Dinar", "", 3)
+CURRENCY["BIF"] = Currency("BIF", 108, "Burundi Franc", "", 0)
+CURRENCY["BMD"] = Currency("BMD", 60, "Bermudian Dollar", "", 2)
+CURRENCY["BND"] = Currency("BND", 96, "Brunei Dollar", "$", 2)
+CURRENCY["BOB"] = Currency("BOB", 68, "Boliviano", "", 2)
+CURRENCY["BOV"] = Currency("BOV", 984, "Mvdol", "", 2)
+CURRENCY["BRL"] = Currency("BRL", 986, "Brazilian Real", "", 2)
+CURRENCY["BSD"] = Currency("BSD", 44, "Bahamian Dollar", "", 2)
+CURRENCY["BTN"] = Currency("BTN", 64, "Ngultrum", "", 2)
+CURRENCY["BWP"] = Currency("BWP", 72, "Pula", "P", 2)
+CURRENCY["BYR"] = Currency("BYR", 974, "Belarussian Ruble", "p.", 0)
+CURRENCY["BZD"] = Currency("BZD", 84, "Belize Dollar", "BZ$", 2)
+CURRENCY["CAD"] = Currency("CAD", 124, "Canadian Dollar", "$", 2)
+CURRENCY["CDF"] = Currency("CDF", 976, "Congolese Franc", "", 2)
+CURRENCY["CHE"] = Currency("CHE", 947, "WIR Euro", "", 2)
+CURRENCY["CHF"] = Currency("CHF", 756, "Swiss Franc", "CHF", 2)
+CURRENCY["CHW"] = Currency("CHW", 948, "WIR Franc", "", 2)
+CURRENCY["CLF"] = Currency("CLF", 990, "Unidad de Fomento", "", 4)
+CURRENCY["CLP"] = Currency("CLP", 152, "Chilean Peso", "$", 0)
+CURRENCY["CNY"] = Currency("CNY", 156, "Yuan Renminbi", "¥", 2)
+CURRENCY["COP"] = Currency("COP", 170, "Colombian Peso", "$", 2)
+CURRENCY["COU"] = Currency("COU", 970, "Unidad de Valor Real", "", 2)
+CURRENCY["CRC"] = Currency("CRC", 188, "Costa Rican Colon", "₡", 2)
+CURRENCY["CUC"] = Currency("CUC", 931, "Peso Convertible", "", 2)
+CURRENCY["CUP"] = Currency("CUP", 192, "Cuban Peso", "₱", 2)
+CURRENCY["CVE"] = Currency("CVE", 132, "Cabo Verde Escudo", "", 2)
+CURRENCY["CZK"] = Currency("CZK", 203, "Czech Koruna", "Kč", 2)
+CURRENCY["DJF"] = Currency("DJF", 262, "Djibouti Franc", "", 0)
+CURRENCY["DKK"] = Currency("DKK", 208, "Danish Krone", "kr", 2)
+CURRENCY["DOP"] = Currency("DOP", 214, "Dominican Peso", "RD$", 2)
+CURRENCY["DZD"] = Currency("DZD", 12, "Algerian Dinar", "", 2)
+CURRENCY["EGP"] = Currency("EGP", 818, "Egyptian Pound", "£", 2)
+CURRENCY["ERN"] = Currency("ERN", 232, "Nakfa", "", 2)
+CURRENCY["ETB"] = Currency("ETB", 230, "Ethiopian Birr", "", 2)
+CURRENCY["EUR"] = Currency("EUR", 978, "Euro", "€", 2)
+CURRENCY["FJD"] = Currency("FJD", 242, "Fiji Dollar", "$", 2)
+CURRENCY["FKP"] = Currency("FKP", 238, "Falkland Islands Pound", "£", 2)
+CURRENCY["GBP"] = Currency("GBP", 826, "Pound Sterling", "£", 2)
+CURRENCY["GEL"] = Currency("GEL", 981, "Lari", "", 2)
+CURRENCY["GHS"] = Currency("GHS", 936, "Ghana Cedi", "¢", 2)
+CURRENCY["GIP"] = Currency("GIP", 292, "Gibraltar Pound", "£", 2)
+CURRENCY["GMD"] = Currency("GMD", 270, "Dalasi", "", 2)
+CURRENCY["GNF"] = Currency("GNF", 324, "Guinea Franc", "", 0)
+CURRENCY["GTQ"] = Currency("GTQ", 320, "Quetzal", "Q", 2)
+CURRENCY["GYD"] = Currency("GYD", 328, "Guyana Dollar", "$", 2)
+CURRENCY["HKD"] = Currency("HKD", 344, "Hong Kong Dollar", "$", 2)
+CURRENCY["HNL"] = Currency("HNL", 340, "Lempira", "L", 2)
+CURRENCY["HRK"] = Currency("HRK", 191, "Croatian Kuna", "kn", 2)
+CURRENCY["HTG"] = Currency("HTG", 332, "Gourde", "", 2)
+CURRENCY["HUF"] = Currency("HUF", 348, "Forint", "Ft", 2)
+CURRENCY["IDR"] = Currency("IDR", 360, "Rupiah", "Rp", 2)
+CURRENCY["ILS"] = Currency("ILS", 376, "New Israeli Sheqel", "₪", 2)
+CURRENCY["INR"] = Currency("INR", 356, "Indian Rupee", "₹", 2)
+CURRENCY["IQD"] = Currency("IQD", 368, "Iraqi Dinar", "", 3)
+CURRENCY["IRR"] = Currency("IRR", 364, "Iranian Rial", "﷼", 2)
+CURRENCY["ISK"] = Currency("ISK", 352, "Iceland Krona", "kr", 0)
+CURRENCY["JMD"] = Currency("JMD", 388, "Jamaican Dollar", "J$", 2)
+CURRENCY["JOD"] = Currency("JOD", 400, "Jordanian Dinar", "", 3)
+CURRENCY["JPY"] = Currency("JPY", 392, "Yen", "¥", 0)
+CURRENCY["KES"] = Currency("KES", 404, "Kenyan Shilling", "", 2)
+CURRENCY["KGS"] = Currency("KGS", 417, "Som", "лв", 2)
+CURRENCY["KHR"] = Currency("KHR", 116, "Riel", "៛", 2)
+CURRENCY["KMF"] = Currency("KMF", 174, "Comoro Franc", "", 0)
+CURRENCY["KPW"] = Currency("KPW", 408, "North Korean Won", "₩", 2)
+CURRENCY["KRW"] = Currency("KRW", 410, "Won", "₩", 0)
+CURRENCY["KWD"] = Currency("KWD", 414, "Kuwaiti Dinar", "", 3)
+CURRENCY["KYD"] = Currency("KYD", 136, "Cayman Islands Dollar", "$", 2)
+CURRENCY["KZT"] = Currency("KZT", 398, "Tenge", "лв", 2)
+CURRENCY["LAK"] = Currency("LAK", 418, "Kip", "₭", 2)
+CURRENCY["LBP"] = Currency("LBP", 422, "Lebanese Pound", "£", 2)
+CURRENCY["LKR"] = Currency("LKR", 144, "Sri Lanka Rupee", "₨", 2)
+CURRENCY["LRD"] = Currency("LRD", 430, "Liberian Dollar", "$", 2)
+CURRENCY["LSL"] = Currency("LSL", 426, "Loti", "", 2)
+CURRENCY["LTL"] = Currency("LTL", 440, "Lithuanian Litas", "Lt", 2)
+CURRENCY["LYD"] = Currency("LYD", 434, "Libyan Dinar", "", 3)
+CURRENCY["MAD"] = Currency("MAD", 504, "Moroccan Dirham", "", 2)
+CURRENCY["MDL"] = Currency("MDL", 498, "Moldovan Leu", "", 2)
+CURRENCY["MGA"] = Currency("MGA", 969, "Malagasy Ariary", "", 2)
+CURRENCY["MKD"] = Currency("MKD", 807, "Denar", "ден", 2)
+CURRENCY["MMK"] = Currency("MMK", 104, "Kyat", "", 2)
+CURRENCY["MNT"] = Currency("MNT", 496, "Tugrik", "₮", 2)
+CURRENCY["MOP"] = Currency("MOP", 446, "Pataca", "", 2)
+CURRENCY["MRO"] = Currency("MRO", 478, "Ouguiya", "", 2)
+CURRENCY["MUR"] = Currency("MUR", 480, "Mauritius Rupee", "₨", 2)
+CURRENCY["MVR"] = Currency("MVR", 462, "Rufiyaa", "", 2)
+CURRENCY["MWK"] = Currency("MWK", 454, "Kwacha", "", 2)
+CURRENCY["MXN"] = Currency("MXN", 484, "Mexican Peso", "$", 2)
+CURRENCY["MXV"] = Currency("MXV", 979, "Mexican Unidad de Inversion (UDI)", "", 2)
+CURRENCY["MYR"] = Currency("MYR", 458, "Malaysian Ringgit", "RM", 2)
+CURRENCY["MZN"] = Currency("MZN", 943, "Mozambique Metical", "MT", 2)
+CURRENCY["NAD"] = Currency("NAD", 516, "Namibia Dollar", "$", 2)
+CURRENCY["NGN"] = Currency("NGN", 566, "Naira", "₦", 2)
+CURRENCY["NIO"] = Currency("NIO", 558, "Cordoba Oro", "C$", 2)
+CURRENCY["NOK"] = Currency("NOK", 578, "Norwegian Krone", "kr", 2)
+CURRENCY["NPR"] = Currency("NPR", 524, "Nepalese Rupee", "₨", 2)
+CURRENCY["NZD"] = Currency("NZD", 554, "New Zealand Dollar", "$", 2)
+CURRENCY["OMR"] = Currency("OMR", 512, "Rial Omani", "﷼", 3)
+CURRENCY["PAB"] = Currency("PAB", 590, "Balboa", "B/.", 2)
+CURRENCY["PEN"] = Currency("PEN", 604, "Nuevo Sol", "S/.", 2)
+CURRENCY["PGK"] = Currency("PGK", 598, "Kina", "", 2)
+CURRENCY["PHP"] = Currency("PHP", 608, "Philippine Peso", "₱", 2)
+CURRENCY["PKR"] = Currency("PKR", 586, "Pakistan Rupee", "₨", 2)
+CURRENCY["PLN"] = Currency("PLN", 985, "Zloty", "zł", 2)
+CURRENCY["PYG"] = Currency("PYG", 600, "Guarani", "Gs", 0)
+CURRENCY["QAR"] = Currency("QAR", 634, "Qatari Rial", "﷼", 2)
+CURRENCY["RON"] = Currency("RON", 946, "New Romanian Leu", "lei", 2)
+CURRENCY["RSD"] = Currency("RSD", 941, "Serbian Dinar", "Дин.", 2)
+CURRENCY["RUB"] = Currency("RUB", 643, "Russian Ruble", "руб", 2)
+CURRENCY["RWF"] = Currency("RWF", 646, "Rwanda Franc", "", 0)
+CURRENCY["SAR"] = Currency("SAR", 682, "Saudi Riyal", "", 2)
+CURRENCY["SBD"] = Currency("SBD", 90, "Solomon Islands Dollar", "$", 2)
+CURRENCY["SCR"] = Currency("SCR", 690, "Seychelles Rupee", "₨", 2)
+CURRENCY["SDG"] = Currency("SDG", 938, "Sudanese Pound", "", 2)
+CURRENCY["SEK"] = Currency("SEK", 752, "Swedish Krona", "kr", 2)
+CURRENCY["SGD"] = Currency("SGD", 702, "Singapore Dollar", "$", 2)
+CURRENCY["SHP"] = Currency("SHP", 654, "Saint Helena Pound", "£", 2)
+CURRENCY["SLL"] = Currency("SLL", 694, "Leone", "", 2)
+CURRENCY["SOS"] = Currency("SOS", 706, "Somali Shilling", "S", 2)
+CURRENCY["SRD"] = Currency("SRD", 968, "Surinam Dollar", "$", 2)
+CURRENCY["SSP"] = Currency("SSP", 728, "South Sudanese Pound", "", 2)
+CURRENCY["STD"] = Currency("STD", 678, "Dobra", "", 2)
+CURRENCY["SVC"] = Currency("SVC", 222, "El Salvador Colon", "$", 2)
+CURRENCY["SYP"] = Currency("SYP", 760, "Syrian Pound", "£", 2)
+CURRENCY["SZL"] = Currency("SZL", 748, "Lilangeni", "", 2)
+CURRENCY["THB"] = Currency("THB", 764, "Baht", "฿", 2)
+CURRENCY["TJS"] = Currency("TJS", 972, "Somoni", "", 2)
+CURRENCY["TMT"] = Currency("TMT", 934, "Turkmenistan New Manat", "", 2)
+CURRENCY["TND"] = Currency("TND", 788, "Tunisian Dinar", "", 3)
+CURRENCY["TOP"] = Currency("TOP", 776, "Pa’anga", "", 2)
+CURRENCY["TRY"] = Currency("TRY", 949, "Turkish Lira", "₤", 2)
+CURRENCY["TTD"] = Currency("TTD", 780, "Trinidad and Tobago Dollar", "TT$", 2)
+CURRENCY["TWD"] = Currency("TWD", 901, "New Taiwan Dollar", "NT$", 2)
+CURRENCY["TZS"] = Currency("TZS", 834, "Tanzanian Shilling", "", 2)
+CURRENCY["UAH"] = Currency("UAH", 980, "Hryvnia", "₴", 2)
+CURRENCY["UGX"] = Currency("UGX", 800, "Uganda Shilling", "", 0)
+CURRENCY["USD"] = Currency("USD", 840, "US Dollar", "$", 2)
+CURRENCY["USN"] = Currency("USN", 997, "US Dollar (Next day)", "", 2)
 CURRENCY["UYI"] = Currency(
-    "UYI", 940, "Uruguay Peso en Unidades Indexadas (URUIURUI)", u"", 0
+    "UYI", 940, "Uruguay Peso en Unidades Indexadas (URUIURUI)", "", 0
 )
-CURRENCY["UYU"] = Currency("UYU", 858, "Peso Uruguayo", u"$U", 2)
-CURRENCY["UZS"] = Currency("UZS", 860, "Uzbekistan Sum", u"лв", 2)
-CURRENCY["VEF"] = Currency("VEF", 937, "Bolivar", u"Bs", 2)
-CURRENCY["VND"] = Currency("VND", 704, "Dong", u"₫", 0)
-CURRENCY["VUV"] = Currency("VUV", 548, "Vatu", u"", 0)
-CURRENCY["WST"] = Currency("WST", 882, "Tala", u"", 2)
-CURRENCY["XAF"] = Currency("XAF", 950, "CFA Franc BEAC", u"", 0)
-CURRENCY["XCD"] = Currency("XCD", 951, "East Caribbean Dollar", u"$", 2)
-CURRENCY["XOF"] = Currency("XOF", 952, "CFA Franc BCEAO", u"", 0)
-CURRENCY["XPF"] = Currency("XPF", 953, "CFP Franc", u"", 0)
-CURRENCY["XTS"] = Currency("XTS", 963, "Test currency", u"", 0)
-CURRENCY["YER"] = Currency("YER", 886, "Yemeni Rial", u"﷼", 2)
-CURRENCY["ZAR"] = Currency("ZAR", 710, "Rand", u"S", 2)
-CURRENCY["ZMW"] = Currency("ZMW", 967, "Zambian Kwacha", u"", 2)
-CURRENCY["ZWL"] = Currency("ZWL", 932, "Zimbabwe Dollar", u"Z$", 2)
+CURRENCY["UYU"] = Currency("UYU", 858, "Peso Uruguayo", "$U", 2)
+CURRENCY["UZS"] = Currency("UZS", 860, "Uzbekistan Sum", "лв", 2)
+CURRENCY["VEF"] = Currency("VEF", 937, "Bolivar", "Bs", 2)
+CURRENCY["VND"] = Currency("VND", 704, "Dong", "₫", 0)
+CURRENCY["VUV"] = Currency("VUV", 548, "Vatu", "", 0)
+CURRENCY["WST"] = Currency("WST", 882, "Tala", "", 2)
+CURRENCY["XAF"] = Currency("XAF", 950, "CFA Franc BEAC", "", 0)
+CURRENCY["XCD"] = Currency("XCD", 951, "East Caribbean Dollar", "$", 2)
+CURRENCY["XOF"] = Currency("XOF", 952, "CFA Franc BCEAO", "", 0)
+CURRENCY["XPF"] = Currency("XPF", 953, "CFP Franc", "", 0)
+CURRENCY["XTS"] = Currency("XTS", 963, "Test currency", "", 0)
+CURRENCY["YER"] = Currency("YER", 886, "Yemeni Rial", "﷼", 2)
+CURRENCY["ZAR"] = Currency("ZAR", 710, "Rand", "S", 2)
+CURRENCY["ZMW"] = Currency("ZMW", 967, "Zambian Kwacha", "", 2)
+CURRENCY["ZWL"] = Currency("ZWL", 932, "Zimbabwe Dollar", "Z$", 2)
 
 # Additional special case as BTC is not a "real" currency.
-CURRENCY["BTC"] = Currency("BTC", 0, "Bitcoin", u"฿", 4)
+CURRENCY["BTC"] = Currency("BTC", 0, "Bitcoin", "฿", 4)
```

### Comparing `odin-2.6/src/odin/contrib/money/fields.py` & `odin-2.8/src/odin/contrib/money/fields.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 from odin import exceptions
 from odin.fields import ScalarField
 from odin.validators import EMPTY_VALUES
+
 from .datatypes import Amount
 
 __all__ = ("AmountField",)
 
 
 class AmountField(ScalarField):
-    """
-    Field that contains a monetary amount (with an optional currency).
-    """
+    """Field that contains a monetary amount (with an optional currency)."""
 
     default_error_messages = {
         "invalid": "'%s' value must be a (amount, currency).",
         "invalid_currency": "'%s' currency is not supported.",
     }
     data_type_name = "Amount"
 
     def __init__(self, allowed_currencies=None, **kwargs):
-        super(AmountField, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.allowed_currencies = allowed_currencies
 
     def to_python(self, value):
+        """Convert value to an Amount."""
         if value in EMPTY_VALUES:
             return
         if isinstance(value, Amount):
             return value
 
         try:
             return Amount(value)
+
         except (ValueError, TypeError):
             msg = self.error_messages["invalid"] % value
-            raise exceptions.ValidationError(msg)
+            raise exceptions.ValidationError(msg) from None
 
     def validate(self, value):
-        super(AmountField, self).validate(value)
+        """Validate value."""
+        super().validate(value)
         if (
             self.allowed_currencies
             and (value not in EMPTY_VALUES)
             and (value.currency not in self.allowed_currencies)
         ):
             msg = self.error_messages["invalid_currency"] % str(value.currency)
             raise exceptions.ValidationError(msg)
 
     def prepare(self, value):
+        """Prepare value for serialization."""
         if value in EMPTY_VALUES:
             return
         return float(value), value.currency.code
```

### Comparing `odin-2.6/src/odin/contrib/pint/fields.py` & `odin-2.8/src/odin/contrib/pint/fields.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from abc import ABC
 
 from pint import errors
 
 from odin import exceptions
 from odin.fields import Field
 from odin.validators import EMPTY_VALUES
+
 from .units import registry
 
 __all__ = ("FloatField",)
 
 
 class PintField(Field, ABC):
+    """Base class for Pint fields."""
+
     def __init__(self, units: str, **kwargs):
         super().__init__(**kwargs)
 
         # Ensure we have valid units
         if units is None:
             raise ValueError("Units cannot be None")
         if isinstance(units, str):
@@ -35,31 +38,34 @@
             if isinstance(units, str):
                 units = registry[units]
             # Convert the magnitude and apply units
             value = self.to_magnitude(raw_value) * units
 
         try:
             return value.to(self.units)
-        except errors.DimensionalityError as de:
-            raise exceptions.ValidationError(de)
+        except errors.DimensionalityError as ex:
+            raise exceptions.ValidationError(str(ex)) from None
 
     def to_magnitude(self, value):
         raise NotImplementedError()
 
 
 class FloatField(PintField):
     default_error_messages = {
         "invalid": "'%s' value must be a float.",
     }
     data_type_name = "Float"
 
-    def to_magnitude(self, value):
+    def to_magnitude(self, value) -> float:
+        """Convert value to a float."""
         try:
             return float(value)
+
         except ValueError:
             msg = self.error_messages["invalid"] % value
-            raise exceptions.ValidationError(msg)
+            raise exceptions.ValidationError(msg) from None
 
     def to_python(self, value):
+        """Convert value to a float."""
         if value in EMPTY_VALUES:
             return None
         return self.to_quantity(value)
```

### Comparing `odin-2.6/src/odin/contrib/rich/theme.py` & `odin-2.8/src/odin/contrib/rich/theme.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Rich Theme definition."""
 from typing import Dict
 
 from rich import get_console
-from rich.theme import Theme
 from rich.style import Style
+from rich.theme import Theme
 
 ODIN_STYLES: Dict[str, Style] = {
     "odin.resource.name": Style(color="bright_cyan"),
     "odin.resource.error": Style(color="red", underline=True),
     "odin.field.name": Style(color="bright_blue"),
     "odin.field.error": Style(color="red", italic=True),
     "odin.field.type": Style(color="magenta"),
```

### Comparing `odin-2.6/src/odin/contrib/rich/validation_tree.py` & `odin-2.8/src/odin/contrib/rich/validation_tree.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 """Integration with Rich for nicer CLI's!"""
-from rich.text import Text
 from typing import Iterable, Union
 
 from rich.tree import Tree
 
-from odin.exceptions import ValidationError, NON_FIELD_ERRORS
-from .theme import odin_theme
+from odin.exceptions import NON_FIELD_ERRORS, ValidationError
 
 
 def _all_str(iterable: Iterable) -> bool:
     """Does the supplied iterable only contain strings."""
     return all(isinstance(item, str) for item in iterable)
 
 
 def _validation_error_to_tree(error_messages: Union[list, dict], tree: Tree):
     """Internal recursive method."""
 
     if isinstance(error_messages, dict):
         for name, value in error_messages.items():
-
             node = tree.add(
-                f"[odin.resource.name]+"
+                "[odin.resource.name]+"
                 if name == NON_FIELD_ERRORS
                 else f"[odin.field.name]{name}"
             )
 
             _validation_error_to_tree(value, node)
 
     elif isinstance(error_messages, list):
```

### Comparing `odin-2.6/src/odin/contrib/sphinx/__init__.py` & `odin-2.8/src/odin/contrib/sphinx/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Sphinx integration to document resources."""
-from typing import Tuple, Any
+from typing import Any, Tuple
 
 from sphinx.application import Sphinx
 from sphinx.ext.autodoc import (
     Documenter,
     ModuleLevelDocumenter,
-    bool_option,
     ObjectMembers,
+    bool_option,
 )
 from sphinx.util import logging
 
 import odin
 from odin.resources import ResourceBase
 from odin.utils import field_iter, getmeta
 
@@ -158,15 +158,15 @@
             # Calculate table column widths
             name_len = 4
             data_type_len = 9
             details_len = 7
             for name, data_type, details in data_table:
                 name_len = max(len(name), name_len)
                 data_type_len = max(len(data_type), data_type_len)
-                details_len = max(max(len(l) for l in details), details_len)
+                details_len = max(max(len(value) for value in details), details_len)
             name_len += 2  # Padding
             data_type_len += 2  # Padding
             details_len += 2  # Padding
 
             def add_separator(char="-"):
                 self.add_line(
                     f"+{char * name_len}+{char * data_type_len}+{char * details_len}+",
```

### Comparing `odin-2.6/src/odin/contrib/swagger/__init__.py` & `odin-2.8/src/odin/contrib/swagger/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,56 +1,51 @@
 """
 Tools for generating Swagger Specification from resources.
 """
-from odin.utils import getmeta
 from odin import fields
+from odin.utils import getmeta
 
 SWAGGER_SPEC_TYPE_MAPPING = {
-    fields.IntegerField: 'integer',
-    fields.FloatField: 'number',
-    fields.BooleanField: 'boolean',
+    fields.IntegerField: "integer",
+    fields.FloatField: "number",
+    fields.BooleanField: "boolean",
 }
 """
 Mapping of fields to Swagger types.
 """
 
 SWAGGER_SPEC_FORMAT_MAPPING = {
-    fields.StringField: '',
-    fields.IntegerField: 'int64',
-    fields.FloatField: 'float',
-    fields.BooleanField: '',
-    fields.DateField: 'date',
-    fields.DateTimeField: 'date-time',
-    fields.NaiveTimeField: 'date-time',
+    fields.StringField: "",
+    fields.IntegerField: "int64",
+    fields.FloatField: "float",
+    fields.BooleanField: "",
+    fields.DateField: "date",
+    fields.DateTimeField: "date-time",
+    fields.NaiveTimeField: "date-time",
 }
 """
 Mapping of fields to Swagger formats.
 """
 
 
 def generate_definition(resource):
     """
     Generate a `Swagger Definitions Object <http://swagger.io/specification/#definitionsObject>`_
     from a resource.
 
     """
     meta = getmeta(resource)
 
-    definition = {
-        'type': "object",
-        'properties': {}
-    }
+    definition = {"type": "object", "properties": {}}
 
     for field in meta.all_fields:
-        field_definition = {
-            'type': SWAGGER_SPEC_TYPE_MAPPING.get(field, 'string')
-        }
+        field_definition = {"type": SWAGGER_SPEC_TYPE_MAPPING.get(field, "string")}
 
         if field in SWAGGER_SPEC_FORMAT_MAPPING:
-            field_definition['format'] = SWAGGER_SPEC_FORMAT_MAPPING[field]
+            field_definition["format"] = SWAGGER_SPEC_FORMAT_MAPPING[field]
 
         if field.doc_text:
-            field_definition['description'] = field.doc_text
+            field_definition["description"] = field.doc_text
 
-        definition['properties'][field.name] = field_definition
+        definition["properties"][field.name] = field_definition
 
     return {meta.name: definition}
```

### Comparing `odin-2.6/src/odin/datastructures.py` & `odin-2.8/src/odin/datastructures.py`

 * *Files identical despite different names*

### Comparing `odin-2.6/src/odin/datetimeutil.py` & `odin-2.8/src/odin/datetimeutil.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 import re
 import time
-from email.utils import parsedate_tz as parse_http_datetime
 from email.utils import formatdate as format_http_datetime  # noqa
-from typing import Union, Type, Dict
+from email.utils import parsedate_tz as parse_http_datetime
+from typing import Dict, Type, Union
 
 
 class IgnoreTimezone:
     pass
 
 
 IgnorableTimezone = Union[datetime.tzinfo, Type[IgnoreTimezone]]
@@ -218,15 +218,15 @@
     """Parse a date in the string format defined in ISO 8601."""
     if not isinstance(date_string, str):
         raise ValueError("Expected string")
 
     try:
         return datetime.datetime.strptime(date_string, "%Y-%m-%d").date()
     except ValueError:
-        raise ValueError("Expected ISO 8601 formatted date string.")
+        raise ValueError("Expected ISO 8601 formatted date string.") from None
 
 
 def parse_iso_time_string(
     time_string: str, default_timezone: IgnorableTimezone = utc
 ) -> datetime.time:
     """Parse a time in the string format defined by ISO 8601."""
     if not isinstance(time_string, str):
```

### Comparing `odin-2.6/src/odin/decorators.py` & `odin-2.8/src/odin/decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Helpful decorators."""
-from typing import Dict, Any, Type, Callable, TypeVar, Union
+from typing import Any, Callable, Dict, Type, TypeVar, Union
 
-from odin.resources import build_object_graph, ResourceBase
+from odin.resources import ResourceBase, build_object_graph
 
 _F = TypeVar("_F", bound=Callable[..., Any])
 
 
 def returns_resource(
     func: _F = None,
     codec=None,
```

### Comparing `odin-2.6/src/odin/exceptions.py` & `odin-2.8/src/odin/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Exceptions raised by Odin."""
-from typing import Union, List, Dict, Final
+from typing import Dict, Final, List, Union
 
 from odin import registration
 
 NON_FIELD_ERRORS: Final[str] = "__all__"
 
 
 class ValidationError(Exception):
```

### Comparing `odin-2.6/src/odin/fields/__init__.py` & `odin-2.8/src/odin/fields/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import copy
 import datetime
 import enum
 import pathlib
 import re
 import uuid
 from functools import cached_property
-from typing import Sequence, Tuple, Any, TypeVar, Optional, Type, Dict
+from typing import Any, Dict, Optional, Sequence, Tuple, Type, TypeVar
 
-from odin import exceptions, datetimeutil, registration
+from odin import datetimeutil, exceptions, registration
 from odin.utils import getmeta
 from odin.validators import (
     EMPTY_VALUES,
     MaxLengthValidator,
-    MinValueValidator,
     MaxValueValidator,
-    validate_url,
+    MinValueValidator,
+    validate_email_address,
     validate_ipv4_address,
     validate_ipv6_address,
     validate_ipv46_address,
-    validate_email_address,
+    validate_url,
 )
+
 from .base import BaseField
 
 __all__ = (
     "NotProvided",
     "NotProvidedType",
     "BaseField",
     "Field",
@@ -239,14 +240,16 @@
 
     def value_to_object(self, obj, data):
         """Assign a value to an object."""
         setattr(obj, self.attname, data)
 
 
 class BooleanField(Field):
+    """Field that must contain a boolean value."""
+
     default_error_messages = {"invalid": "'%s' value must be either True or False."}
     true_strings = ("t", "true", "y", "yes", "on", "1", "✓")
     false_strings = ("f", "false", "n", "no", "off", "0")
     data_type_name = "Boolean"
 
     def to_python(self, value):
         if value is None:
@@ -302,14 +305,16 @@
         if not self.empty and value == "":
             raise exceptions.ValidationError(self.error_messages["null"])
 
         super().validate(value)
 
 
 class UrlField(StringField):
+    """Field that must create a URL."""
+
     data_type_name = "URL"
 
     def __init__(self, **options):
         options.setdefault("validators", []).append(validate_url)
         super().__init__(**options)
 
 
@@ -326,17 +331,18 @@
             self.validators.append(MaxValueValidator(max_value))
 
     def to_python(self, value):
         if value in self.empty_values:
             return
         try:
             return self.scalar_type(value)
+
         except (TypeError, ValueError):
             msg = self.error_messages["invalid"] % value
-            raise exceptions.ValidationError(msg)
+            raise exceptions.ValidationError(msg) from None
 
 
 class IntegerField(ScalarField):
     default_error_messages = {
         "invalid": "'%s' value must be a integer.",
     }
     data_type_name = "Integer"
@@ -626,14 +632,15 @@
             return datetime.datetime.fromtimestamp(int(value), tz=datetimeutil.utc)
         except ValueError:
             pass
         msg = self.error_messages["invalid"]
         raise exceptions.ValidationError(msg)
 
     def prepare(self, value):
+        """Prepare for value for serialisation"""
         if value in self.empty_values:
             return
         if isinstance(value, int):
             return int(value)
         if isinstance(value, datetime.datetime):
             return datetimeutil.to_timestamp(value)
 
@@ -655,17 +662,18 @@
 
     def to_python(self, value):
         if value is None:
             return value
         try:
             val = dict(value)
             return val
+
         except (TypeError, ValueError):
             msg = self.error_messages["invalid"]
-            raise exceptions.ValidationError(msg)
+            raise exceptions.ValidationError(msg) from None
 
 
 ObjectField = DictField
 
 
 class ListField(Field):
     default_error_messages = {
@@ -691,93 +699,95 @@
         raise exceptions.ValidationError(msg)
 
 
 ArrayField = ListField
 
 
 class TypedListField(ListField):
+    """Field that handles a list of a specific type."""
+
     @staticmethod
     def data_type_name(instance):
         type_name = instance.field.data_type_name
         if callable(type_name):
             type_name = type_name(instance.field)
         return f"List<{type_name}>"
 
     def __init__(self, field: Field, **options):
+        """Initialise the typed list field."""
         self.field = field
         super().__init__(**options)
 
     @property
     def choices_doc_text(self) -> Sequence[Tuple[Any, str]]:
+        """Generate choices for documentation purposes."""
         if self.choices:
             return self.choices
         if hasattr(self.field, "choices_doc_text"):
             return self.field.choices_doc_text
         return self.field.choices
 
     def to_python(self, value):
+        """Convert the value to a list of the specified type."""
         value = super().to_python(value)
         if not value:
             return value
 
         value_list = []
         errors = {}
         field_to_python = self.field.to_python
         for idx, item in enumerate(value):
             try:
                 value_list.append(field_to_python(item))
             except exceptions.ValidationError as ve:
-                errors[idx] = ve.error_messages
+                errors[str(idx)] = ve.error_messages
 
         if errors:
             raise exceptions.ValidationError(errors)
 
         return value_list
 
     def validate(self, value):
-        """
-        Validate each item against field
-        """
+        """Validate each item against field"""
         super().validate(value)
         if value:
             field_validate = self.field.validate
 
             errors = {}
             for idx, item in enumerate(value):
                 try:
                     field_validate(item)
                 except exceptions.ValidationError as ve:
-                    errors[idx] = ve.error_messages
+                    errors[str(idx)] = ve.error_messages
 
             if errors:
                 raise exceptions.ValidationError(errors)
 
         return value
 
     def run_validators(self, value):
-        """
-        Run validators against each item in the field
-        """
+        """Run validators against each item in the field"""
         super().run_validators(value)
         if value:
             field_run_validators = self.field.run_validators
 
             errors = {}
             for idx, item in enumerate(value):
                 try:
                     field_run_validators(item)
                 except exceptions.ValidationError as ve:
-                    errors[idx] = ve.error_messages
+                    errors[str(idx)] = ve.error_messages
 
             if errors:
                 raise exceptions.ValidationError(errors)
 
         return value
 
     def prepare(self, value):
+        """Prepare list for serialisation."""
         if isinstance(value, (tuple, list)):
             prepare = self.field.prepare
             return [prepare(i) for i in value]
         return value
 
 
 TypedArrayField = TypedListField
@@ -800,289 +810,296 @@
         if callable(key_type_name):
             key_type_name = key_type_name(instance.key_field)
 
         value_type_name = instance.value_field.data_type_name
         if callable(value_type_name):
             value_type_name = value_type_name(instance.value_field)
 
-        return "Dict<{0}, {1}>".format(key_type_name, value_type_name)
+        return f"Dict<{key_type_name}, {value_type_name}>"
 
     def __init__(self, value_field, key_field=StringField(), **options):
         self.key_field = key_field
         self.value_field = value_field
         super().__init__(**options)
 
     def to_python(self, value):
+        """Convert the value to a dict of the specified type."""
         value = super().to_python(value)
         if not value:
             return value
 
         value_dict = {}
         key_errors = []
         value_errors = {}
-        for key, value in value.items():
+        for key, val in value.items():
             try:
                 key = self.key_field.to_python(key)
             except exceptions.ValidationError as ve:
                 key_errors += ve.error_messages
 
-            # If we have key errors no point checking values any more.
+            # If we have key errors no point checking values.
             if key_errors:
                 continue
 
             try:
-                value_dict[key] = self.value_field.to_python(value)
+                value_dict[key] = self.value_field.to_python(val)
             except exceptions.ValidationError as ve:
                 value_errors[key] = ve.error_messages
 
         if key_errors:
             raise exceptions.ValidationError(key_errors)
         if value_errors:
             raise exceptions.ValidationError(value_errors)
 
         return value_dict
 
     def validate(self, value):
+        """Validate value."""
         super().validate(value)
 
         if value in self.empty_values:
             return
 
         key_errors = []
         value_errors = {}
-        for key, value in value.items():
+        for key, val in value.items():
             try:
                 self.key_field.validate(key)
             except exceptions.ValidationError as ve:
                 key_errors += ve.error_messages
 
-            # If we have key errors no point checking values any more.
+            # If we have key errors no point checking values
             if key_errors:
                 continue
 
             try:
-                self.value_field.validate(value)
+                self.value_field.validate(val)
+
             except exceptions.ValidationError as ve:
                 value_errors[key] = ve.error_messages
 
         if key_errors:
             raise exceptions.ValidationError(key_errors)
         if value_errors:
             raise exceptions.ValidationError(value_errors)
 
     def run_validators(self, value):
+        """Run validators against value."""
         super().run_validators(value)
 
         if value in self.empty_values:
             return
 
         key_errors = []
         value_errors = {}
-        for key, value in value.items():
+        for key, val in value.items():
             try:
                 key = self.key_field.run_validators(key)
             except exceptions.ValidationError as ve:
                 key_errors += ve.error_messages
 
-            # If we have key errors no point checking values any more.
+            # If we have key errors no point checking values.
             if key_errors:
                 continue
 
             try:
-                self.value_field.run_validators(value)
+                self.value_field.run_validators(val)
             except exceptions.ValidationError as ve:
                 value_errors[key] = ve.error_messages
 
         if key_errors:
             raise exceptions.ValidationError(key_errors)
         if value_errors:
             raise exceptions.ValidationError(value_errors)
 
+    def prepare(self, value):
+        """Prepare list for serialisation."""
+        if isinstance(value, dict):
+            prepare_key = self.key_field.prepare
+            prepare_value = self.value_field.prepare
+            return {prepare_key(k): prepare_value(v) for k, v in value.items()}
+        return value
+
 
 TypedObjectField = TypedDictField
 
 
 class EmailField(StringField):
-    """
-    An Email address.
+    """An Email address.
 
     Validates that a string represents a valid Email address.
-
     """
 
     data_type_name = "Email"
 
     def __init__(self, **options):
+        """Initialise the field."""
         options.setdefault("validators", []).append(validate_email_address)
         super().__init__(**options)
 
 
 class IPv4Field(StringField):
-    """
-    An IPv4 address.
+    """An IPv4 address.
 
     Validates that a string represents a valid IPv4 address format.
-
     """
 
     data_type_name = "IPv4"
 
     def __init__(self, **options):
+        """Initialise the field."""
         options.setdefault("validators", []).append(validate_ipv4_address)
         super().__init__(**options)
 
 
 class IPv6Field(StringField):
-    """
-    An IPv6 address.
+    """An IPv6 address.
 
     Validates that a string represents a valid IPv6 address format.
-
     """
 
     data_type_name = "IPv6"
 
     def __init__(self, **options):
+        """Initialise the field."""
         options.setdefault("validators", []).append(validate_ipv6_address)
         super().__init__(**options)
 
 
 class IPv46Field(StringField):
-    """
-    An IPv4 or IPv6 address.
+    """An IPv4 or IPv6 address.
 
     Validates that a string represents a valid IPv4 or IPv6 address format.
-
     """
 
     data_type_name = "IPv46"
 
     def __init__(self, **options):
+        """Initialise the field."""
         options.setdefault("validators", []).append(validate_ipv46_address)
         super().__init__(**options)
 
 
 class UUIDField(Field):
-    """
-    An universally unique identifier.
+    """An universally unique identifier.
 
     Validates that the string represents a universally unique identifier.
     """
 
     data_type_name = "UUID"
 
-    def __init__(self, **options):
-        super().__init__(**options)
-
     def to_python(self, value):
+        """Convert the value to a UUID."""
         if value is None:
             return
 
         if isinstance(value, uuid.UUID):
             return value
 
         elif isinstance(value, bytes):
             if len(value) == 16:
                 return uuid.UUID(bytes=value)
 
             try:
                 value = value.decode("utf-8")
             except UnicodeDecodeError as e:
-                raise exceptions.ValidationError(e.args[0], code="invalid")
+                raise exceptions.ValidationError(e.args[0], code="invalid") from None
 
         elif isinstance(value, int):
             try:
                 return uuid.UUID(int=value)
             except ValueError as e:
-                raise exceptions.ValidationError(e.args[0], code="invalid")
+                raise exceptions.ValidationError(e.args[0], code="invalid") from None
 
         elif isinstance(value, (tuple, list)):
             try:
                 return uuid.UUID(fields=value)
             except ValueError as e:
-                raise exceptions.ValidationError(e.args[0], code="invalid")
+                raise exceptions.ValidationError(e.args[0], code="invalid") from None
 
         elif not isinstance(value, str):
             value = str(value)
 
         try:
             return uuid.UUID(value)
         except ValueError as e:
-            raise exceptions.ValidationError(e.args[0], code="invalid")
+            raise exceptions.ValidationError(e.args[0], code="invalid") from None
 
 
 ET = TypeVar("ET", bound=enum.Enum)
 
 
 class EnumField(Field):
-    """
-    Field for handling Python enums.
-    """
+    """Field for handling Python enums."""
 
     data_type_name = "Enum"
 
     def __init__(self, enum_type: Type[ET], **options):
+        """Initialise the field."""
 
         # Generate choices structure from choices
         choices = options.pop("choices", None)
         options["choices"] = tuple((e, e.name) for e in choices or enum_type)
 
         super().__init__(**options)
         self.enum_type = enum_type
 
     @property
     def choices_doc_text(self):
-        """
-        Choices converted for documentation purposes.
-        """
+        """Choices converted for documentation purposes."""
         return tuple((v.value, n) for v, n in self.choices)
 
     def to_python(self, value) -> Optional[ET]:
+        """Convert the value to an enum."""
         if value is None:
             return
 
         # Attempt to convert
         try:
             return self.enum_type(value)
         except ValueError:
             # If value is an empty string return None
             # Do this check here to support enums that define an option using
             # an empty string.
             if value == "":
                 return
             raise exceptions.ValidationError(
                 self.error_messages["invalid_choice"] % value
-            )
+            ) from None
 
     def prepare(self, value: Optional[ET]):
+        """Prepare enum for serialisation."""
         if (value is not None) and isinstance(value, self.enum_type):
             return value.value
 
 
 class PathField(Field):
-    """
-    Field for handling Python Paths
-    """
+    """Field for handling Python Paths"""
 
     default_error_messages = {
         "invalid": "Value %s is not a valid path.",
     }
     data_type_name = "Path"
 
     def to_python(self, value) -> Optional[pathlib.Path]:
+        """Convert the value to a Path."""
         if value is None:
             return
 
         # Attempt to convert
         try:
             return pathlib.Path(value)
+
         except (ValueError, TypeError):
-            raise exceptions.ValidationError(self.error_messages["invalid"] % value)
+            raise exceptions.ValidationError(
+                self.error_messages["invalid"] % value
+            ) from None
 
     def prepare(self, value: Optional[str]):
+        """Prepare path for serialisation."""
         if isinstance(value, pathlib.Path):
             return value.as_posix()
 
 
 class RegexField(Field):
     """
     Field for handling regular expressions.
@@ -1095,22 +1112,28 @@
     default_error_messages = {
         "invalid": "Value '%s' is not a valid regular expression.",
         "syntax": "Value '%s' contains invalid syntax: %s.",
     }
     data_type_name = "Regex"
 
     def to_python(self, value) -> Optional[re.Pattern]:
+        """Convert the value to a regular expression."""
         if value is None:
             return
 
         try:
             return re.compile(value)
+
         except TypeError:
-            raise exceptions.ValidationError(self.error_messages["invalid"] % value)
+            raise exceptions.ValidationError(
+                self.error_messages["invalid"] % value
+            ) from None
+
         except re.error as ex:
             raise exceptions.ValidationError(
                 self.error_messages["syntax"] % (value, ex)
-            )
+            ) from None
 
     def prepare(self, value: Optional[re.Pattern]):
+        """Prepare regular expression for serialisation."""
         if isinstance(value, re.Pattern):
             return value.pattern
```

### Comparing `odin-2.6/src/odin/fields/base.py` & `odin-2.8/src/odin/fields/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Callable
+from typing import Callable, Optional
 
 
 class BaseField:
     """Base all field inherit from."""
 
     # These track each time an instance is created. Used to retain order.
     creation_counter = 0
```

### Comparing `odin-2.6/src/odin/fields/composite.py` & `odin-2.8/src/odin/fields/composite.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from odin import bases
-from odin import exceptions
-from odin.resources import create_resource_from_dict
+from typing import Any, Iterator, Tuple
+
+from odin import bases, exceptions
 from odin.fields import Field
+from odin.resources import create_resource_from_dict
 from odin.utils import value_in_choices
 from odin.validators import EMPTY_VALUES
 
 __all__ = (
     "CompositeField",
     "DictAs",
     "ObjectAs",
@@ -28,36 +29,36 @@
         :param use_container: Special flag for codecs that support containers or just multiple instances of a
             sub element (ie XML).
         :param empty: This collection can be empty
         :param options: Additional options passed to :py:class:`odin.fields.Field` super class.
 
         """
         if not hasattr(resource, "_meta"):
-            raise TypeError(
-                "{!r} is not a valid type for a related field.".format(resource)
-            )
+            raise TypeError(f"{resource!r} is not a valid type for a related field.")
         self.of = resource
         self.use_container = use_container
 
         if not options.get("null", False):
             options.setdefault("default", lambda: resource())
 
         super().__init__(**options)
 
     def to_python(self, value):
+        """Convert raw value to a python value."""
         if value is None:
             return None
         if isinstance(value, self.of):
             return value
         if isinstance(value, dict):
             return create_resource_from_dict(value, self.of, full_clean=False)
         msg = self.error_messages["invalid"] % self.of
         raise exceptions.ValidationError(msg)
 
     def validate(self, value):
+        """Validate the value."""
         super().validate(value)
         if value not in EMPTY_VALUES:
             value.full_clean()
 
     def item_iter_from_object(self, obj):
         """
         Return an iterator of items (resource, idx) from composite field.
@@ -75,17 +76,15 @@
         :param key:
         :return:
         """
         raise NotImplementedError()
 
 
 class DictAs(CompositeField):
-    """
-    Treat a dictionary as a Resource.
-    """
+    """Treat a dictionary as a Resource."""
 
     default_error_messages = {
         "invalid": "Must be a dict of type ``%r``.",
     }
     data_type_name = "Dict as"
 
     def item_iter_from_object(self, obj):
@@ -97,26 +96,25 @@
         pass  # Not required as keys are not used.
 
 
 ObjectAs = DictAs
 
 
 class ListOf(CompositeField):
-    """
-    List of resources.
-    """
+    """List of resources."""
 
     default_error_messages = {
         "invalid": "Must be a list of ``%r`` objects.",
         "null": "List cannot contain null entries.",
         "empty": "List cannot be empty",
     }
     data_type_name = "List of"
 
     def __init__(self, resource, empty=True, **options):
+        """Initialisation of a ListOf field."""
         options.setdefault("default", list)
         super().__init__(resource, **options)
         self.empty = empty
 
     @staticmethod
     def _process_list(value_list, method):
         values = []
@@ -131,14 +129,15 @@
 
         if errors:
             raise exceptions.ValidationError(errors)
 
         return values
 
     def to_python(self, value):
+        """Convert raw value to a python value."""
         if value is None:
             return None
         if isinstance(value, (list, bases.ResourceIterable)):
             super_to_python = super().to_python
 
             def process(val):
                 if val is None:
@@ -146,59 +145,54 @@
                 return super_to_python(val)
 
             return self._process_list(value, process)
         msg = self.error_messages["invalid"] % self.of
         raise exceptions.ValidationError(msg)
 
     def validate(self, value):
+        """Validate the value."""
         # Skip The direct super method and apply it to each list item.
         super(CompositeField, self).validate(value)  # noqa
         if value is not None:
-            super_validate = super(ListOf, self).validate
+            super_validate = super().validate
             self._process_list(value, super_validate)
 
         if (value is not None) and (not value) and (not self.empty):
             raise exceptions.ValidationError(self.error_messages["empty"])
 
     def __iter__(self):
-        # This does nothing but it does prevent inspections from complaining.
+        # This does nothing, but it does prevent inspections from complaining.
         return None  # NoQA
 
     def item_iter_from_object(self, obj):
         resources = self.value_from_object(obj)
         if resources:
-            for i in enumerate(resources):
-                yield i
+            yield from enumerate(resources)
 
     def key_to_python(self, key):
-        """
-        A to python method for the key value.
-        :param key:
-        :return:
-        """
+        """A to python method for the key value."""
         return int(key)
 
 
 ArrayOf = ListOf
 
 
 class DictOf(CompositeField):
-    """
-    Dictionary of resources.
-    """
+    """Dictionary of resources."""
 
     default_error_messages = {
         "invalid": "Must be a dict of ``%r`` objects.",
         "null": "Dict cannot contain null entries.",
         "empty": "List cannot be empty",
         "invalid_key": "Key %r is not a valid choice.",
     }
     data_type_name = "Dict of"
 
     def __init__(self, resource, empty=True, key_choices=None, **options):
+        """Initialise DictOf field."""
         options.setdefault("default", dict)
         super().__init__(resource, **options)
         self.empty = empty
         self.key_choices = key_choices
 
     def _process_dict(self, value_dict, method):
         values = {}
@@ -216,14 +210,15 @@
 
         if errors:
             raise exceptions.ValidationError(errors)
 
         return values
 
     def to_python(self, value):
+        """Convert raw value to a python type."""
         if value is None:
             return None
         if isinstance(value, dict):
             super_to_python = super().to_python
 
             def process(val):
                 if val is None:
@@ -233,33 +228,31 @@
                 return super_to_python(val)
 
             return self._process_dict(value, process)
         msg = self.error_messages["invalid"] % self.of
         raise exceptions.ValidationError(msg)
 
     def validate(self, value):
+        """Validate the value."""
         # Skip The direct super method and apply it to each list item.
         super(CompositeField, self).validate(value)  # noqa
         if value is not None:
             super_validate = super().validate
             self._process_dict(value, super_validate)
 
         if (value is not None) and (not value) and (not self.empty):
             raise exceptions.ValidationError(self.error_messages["empty"], code="empty")
 
     def __iter__(self):
         # This does nothing but it does prevent inspections from complaining.
         return None  # NoQA
 
-    def item_iter_from_object(self, obj):
+    def item_iter_from_object(self, obj) -> Iterator[Tuple[str, Any]]:
+        """Iterate object returning key/value pairs"""
         resources = self.value_from_object(obj)
         if resources:
             for key in sorted(resources):
                 yield key, resources[key]
 
     def key_to_python(self, key):
-        """
-        A to python method for the key value.
-        :param key:
-        :return:
-        """
+        """A to python method for the key value."""
         return key
```

### Comparing `odin-2.6/src/odin/fields/virtual.py` & `odin-2.8/src/odin/fields/virtual.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Callable, Union, Sequence
+from typing import Any, Callable, Sequence, Union
 
 from odin.utils import force_tuple, getmeta
 
 from .base import BaseField
 
 __all__ = (
     "ConstantField",
@@ -145,8 +145,10 @@
 
     def on_resource_ready(self):
         # Extract reference to fields
         meta = getmeta(self.resource)
         try:
             self._fields = tuple(meta.field_map[name] for name in self.field_names)
         except KeyError as ex:
-            raise AttributeError(f"Attribute {ex} not found on {self.resource!r}")
+            raise AttributeError(
+                f"Attribute {ex} not found on {self.resource!r}"
+            ) from None
```

### Comparing `odin-2.6/src/odin/filtering.py` & `odin-2.8/src/odin/filtering.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import abc
 import operator
-from typing import Callable, Iterable, Any, Sequence, Union
+from typing import Any, Callable, Iterable, Sequence, Union
 
 from .exceptions import InvalidPathError
 from .resources import ResourceBase
 from .traversal import TraversalPath
 
 
 class FilterAtom(abc.ABC):
```

### Comparing `odin-2.6/src/odin/helpers.py` & `odin-2.8/src/odin/helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Helpers
 ~~~~~~~
 
 A collection of useful convenience methods.
 """
 
-from typing import Union, List, Dict, DefaultDict
+from typing import DefaultDict, Dict, List, Union
 
 from odin import BaseField
 from odin.exceptions import NON_FIELD_ERRORS, ValidationError
 
 __all__ = ("ValidationErrorCollection",)
```

### Comparing `odin-2.6/src/odin/mapping/__init__.py` & `odin-2.8/src/odin/mapping/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """Mapping data between resources or other object types."""
 import abc
 from typing import (
-    TypeVar,
-    Union,
-    Sequence,
-    Optional,
-    Callable,
     Any,
-    NamedTuple,
+    Callable,
+    Dict,
     Iterable,
+    NamedTuple,
+    Optional,
+    Sequence,
     Type,
-    Dict,
+    TypeVar,
+    Union,
 )
 
 from odin import bases as base_types
 from odin import registration
-from odin.fields import NotProvided, Field
+from odin.exceptions import MappingExecutionError, MappingSetupError
+from odin.fields import Field, NotProvided
+from odin.fields.composite import DictAs, ListOf
+from odin.mapping.helpers import MapDictAs, MapListOf, NoOpMapper
 from odin.resources import ResourceBase
-from odin.fields.composite import ListOf, DictAs
-from odin.exceptions import MappingSetupError, MappingExecutionError
-from odin.mapping.helpers import MapListOf, MapDictAs, NoOpMapper
 from odin.utils import cached_property, getmeta
 
 __all__ = ("Mapping", "map_field", "map_list_field", "assign_field", "define", "assign")
 
 _V = TypeVar("_V")
 Action = Callable[[Any, "..."], Optional[Any]]
 BoundAction = Callable[["Mapping", Any, "..."], Optional[Any]]
@@ -212,21 +212,21 @@
 
         # Get field resolver objects
         try:
             from_fields = registration.get_field_resolver(from_obj).from_field_dict
         except KeyError:
             raise MappingSetupError(
                 f"`from_obj` {from_obj!r} does not have an attribute resolver defined."
-            )
+            ) from None
         try:
             to_fields = registration.get_field_resolver(to_obj).to_field_dict
         except KeyError:
             raise MappingSetupError(
                 f"`to_obj` {to_obj!r} does not have an attribute resolver defined."
-            )
+            ) from None
 
         def attr_mapping_to_mapping_rule(m, def_type, ref):
             """Parse, validate and normalise defined mapping rules so rules can be executed without having to perform
             checks during a mapping operation."""
             to_list = False
             bind = False
             skip_if_none = False
@@ -235,15 +235,15 @@
                 map_from, action, map_to, to_list, bind, skip_if_none = m
             except ValueError:
                 try:
                     map_from, action, map_to = m
                 except ValueError:
                     raise MappingSetupError(
                         f"Bad mapping definition `{m}` in {def_type} `{ref}`."
-                    )
+                    ) from None
 
             if map_from is None:
                 is_assignment = True
 
             if not is_assignment:
                 map_from = force_tuple(map_from)
                 for f in map_from:
@@ -296,16 +296,16 @@
             map_to = rule[2]
             if len(map_to) == 1 and map_to[0] in unmapped_fields:
                 unmapped_fields.remove(map_to[0])
 
         # Generate mapping rules.
         mapping_rules = []
 
-        # Check that from_obj is a sub_class (or same class) as any `parent.from_obj`. This is important for mapping
-        # sub class lists and resolving mappings.
+        # Check that from_obj is a sub_class (or same class) as any `parent.from_obj`.
+        # This is important for mapping subclass lists and resolving mappings.
         base_parents = [p for p in parents if hasattr(p, "_subs")]
         for p in base_parents:
             if not issubclass(from_obj, p.from_obj):
                 raise MappingSetupError(
                     "`from_obj` must be a subclass of `parent.from_obj`"
                 )
             if not issubclass(to_obj, p.to_obj):
@@ -326,15 +326,15 @@
 
         # Add custom mappings
         for attr in attrs.values():
             # Methods with a _mapping attribute have been decorated by either `map_field` or `map_list_field`
             # decorators.
             if hasattr(attr, "_mapping"):
                 mapping_rule = attr_mapping_to_mapping_rule(
-                    getattr(attr, "_mapping"), "custom mapping", attr
+                    attr._mapping, "custom mapping", attr
                 )
                 mapping_rules.append(mapping_rule)
                 remove_from_unmapped_fields(mapping_rule)
                 # Remove mapping
                 delattr(attr, "_mapping")
 
         # Add auto mapped fields that are yet to be mapped.
@@ -350,15 +350,15 @@
 
         # Create mapper instance
         mapper = super_new(mcs, name, bases, attrs)
         if register_mapping:
             registration.register_mapping(mapper)
             mapper = registration.get_mapping(from_obj, to_obj)
 
-            # Register mapping with parents mapping objects as a sub class.
+            # Register mapping with parents mapping objects as a subclass.
             for parent in base_parents:
                 parent._subs[from_obj] = mapper
 
         return mapper
 
     @classmethod
     def generate_auto_mapping(mcs, name, from_fields, to_fields):
@@ -440,16 +440,15 @@
     This is useful if context is volatile.
     """
 
     def __init__(self, *args, **kwargs):
         self.sequence = list(MappingResult(*args, **kwargs))
 
     def __iter__(self):
-        for item in self.sequence:
-            yield item
+        yield from self.sequence
 
 
 class CachingMappingResult(MappingResult):
     """Extends from the basic MappingResult to cache the results of a mapping operation and also provide methods and
     abilities available to a list (len, indexing). The results are only evaluated when requested.
     """
 
@@ -616,15 +615,17 @@
 
             try:
                 if bind:
                     to_values = action(self, *from_values)
                 else:
                     to_values = action(*from_values)
             except TypeError as ex:
-                raise MappingExecutionError(f"{ex} applying rule {mapping_rule}")
+                raise MappingExecutionError(
+                    f"{ex} applying rule {mapping_rule}"
+                ) from None
 
         if to_list:
             if isinstance(to_values, Iterable):
                 to_values = (list(to_values),)
         else:
             to_values = force_tuple(to_values)
```

### Comparing `odin-2.6/src/odin/mapping/helpers.py` & `odin-2.8/src/odin/mapping/helpers.py`

 * *Files identical despite different names*

### Comparing `odin-2.6/src/odin/proxy.py` & `odin-2.8/src/odin/proxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,43 +3,43 @@
 ~~~~~~~~~~~~~~
 
 The resource proxy is an object that provides an alternate interface to a shadowed Resource.
 
 This could be as a means of providing a summary object, or for adding additional properties.
 
 """
-from typing import List, Union, Optional
+from typing import Optional
 
 from odin import registration
 from odin.bases import TypedResourceIterable
-from odin.resources import ResourceOptions, ResourceBase
-from odin.utils import getmeta, filter_fields, lazy_property
+from odin.resources import ResourceBase, ResourceOptions
+from odin.utils import filter_fields, getmeta, lazy_property
 
-EMPTY = tuple()
+EMPTY = ()
 
 
 class FieldProxyDescriptor:
     """
     Descriptor to proxy field to underlying resource.
     """
 
     __slots__ = ("attname", "readonly")
 
     def __init__(self, readonly=False):
         self.attname: Optional[str] = None
         self.readonly = readonly
 
     def __get__(self, instance, owner):
-        shadow = getattr(instance, "_shadow")
+        shadow = instance._shadow
         return getattr(shadow, self.attname)
 
     def __set__(self, instance, value):
         if self.readonly:
             raise AttributeError("can't set attribute")
-        shadow = getattr(instance, "_shadow")
+        shadow = instance._shadow
         return setattr(shadow, self.attname, value)
 
     def contribute_to_class(self, cls, name):
         self.attname = name
         setattr(cls, name, self)
 
 
@@ -58,23 +58,23 @@
         "type_field",
         "key_field_name",
         "key_field_names",
         "field_sorting",
     )
 
     def __init__(self, meta):
-        super(ResourceProxyOptions, self).__init__(meta)
+        super().__init__(meta)
         self.resource = None
         self.shadow = None
         self.include = []
         self.exclude = []
         self.readonly = []
 
     def __repr__(self):
-        return "<Proxy of {!r}>".format(getmeta(self.resource))
+        return f"<Proxy of {getmeta(self.resource)!r}>"
 
     def contribute_to_class(self, cls, _):
         cls._meta = self
         cls_name = cls.__name__
         self.name = cls_name
         self.class_name = f"{cls.__module__}.{cls_name}"
 
@@ -144,15 +144,15 @@
         return tuple(f for f in self.fields if f.attname not in self.readonly)
 
 
 class ResourceProxyType(type):
     meta_options = ResourceProxyOptions
 
     def __new__(mcs, name, bases, attrs):
-        super_new = super(ResourceProxyType, mcs).__new__
+        super_new = super().__new__
 
         # attrs will never be empty for classes declared in the standard way
         # (ie. with the `class` keyword). This is quite robust.
         if name == "NewBase" and attrs == {}:
             return super_new(mcs, name, bases, attrs)
 
         parents = [
@@ -236,15 +236,15 @@
 class ResourceProxyIter(TypedResourceIterable):
     """
     Returned by `ResourceProxy.proxy` if an iterable is supplied.
     """
 
     def __init__(self, objects, resource_type):
         # type: (Union[List[ResourceBase]], ResourceProxyBase) -> None
-        super(ResourceProxyIter, self).__init__(resource_type)
+        super().__init__(resource_type)
         self.objects = objects
 
     def __iter__(self):
         resource_type = self.resource_type
         for obj in self.objects:
             yield resource_type.proxy(obj)
 
@@ -266,15 +266,15 @@
         meta = getmeta(self)
 
         # Get shadowed resource if supplied
         shadow = kwargs.pop("__resource", None)
         if shadow is None:
             # Create a new instance
             self._shadow = meta.resource()
-            super(ResourceProxyBase, self).__init__(*args, **kwargs)
+            super().__init__(*args, **kwargs)
         else:
             self._shadow = shadow
 
     def get_shadow(self):
         return self._shadow
```

### Comparing `odin-2.6/src/odin/registration.py` & `odin-2.8/src/odin/registration.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 def generate_mapping_cache_name(from_obj, to_obj):
     return f"{from_obj.__module__}.{from_obj.__name__} > {to_obj.__module__}.{to_obj.__name__}"
 
 
 class ResourceCache:
     # Use the Borg pattern to share state between all instances. Details at
     # http://aspn.activestate.com/ASPN/Cookbook/Python/Recipe/66531.
-    __shared_state = dict(
-        resources={},
-        mappings={},
-        field_resolvers=set(),
-        validation_error_handlers={},
-    )
+    __shared_state = {
+        "resources": {},
+        "mappings": {},
+        "field_resolvers": set(),
+        "validation_error_handlers": {},
+    }
 
     def __init__(self):
         self.__dict__ = self.__shared_state
 
     def register_resources(self, *resources):
         """
         Register a resource (or resources).
```

### Comparing `odin-2.6/src/odin/resources.py` & `odin-2.8/src/odin/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 import copy
 from typing import (
-    TypeVar,
-    Dict,
     Any,
-    Type,
+    Callable,
+    Dict,
+    List,
     Optional,
+    Sequence,
     Tuple,
+    Type,
+    TypeVar,
     Union,
-    Sequence,
-    List,
     cast,
-    Callable,
 )
 
-from odin import bases
-from odin import exceptions, registration
-from odin.exceptions import ValidationError, ResourceDefError
-from odin.fields import NotProvided, BaseField, Field, NotProvidedType
-from odin.utils import (
-    cached_property,
-    field_iter_items,
-    force_tuple,
-    getmeta,
-)
+from odin import bases, exceptions, registration
+from odin.exceptions import ResourceDefError, ValidationError
+from odin.fields import BaseField, Field, NotProvided, NotProvidedType
+from odin.utils import cached_property, field_iter_items, force_tuple, getmeta
 
 DEFAULT_TYPE_FIELD = "$"
 
 # Set of field names that cannot be used
 RESERVED_FIELD_NAMES = {
     "fields",  # Causes an infinite-recursion with clean_fields being a builtin method
 }
@@ -240,15 +234,15 @@
 
 class ResourceType(type):
     """Metaclass for all Resources."""
 
     meta_options = ResourceOptions
 
     def __new__(mcs, name, bases, attrs):
-        super_new = super(ResourceType, mcs).__new__
+        super_new = super().__new__
 
         # attrs will never be empty for classes declared in the standard way
         # (i.e. with the `class` keyword). This is quite robust.
         if name == "NewBase" and attrs == {}:
             return super_new(mcs, name, bases, attrs)
 
         parents = [
@@ -697,15 +691,15 @@
 
     :param d: dictionary of data.
     :param resource: A resource type, resource name or list of resources and names to use as the base for creating a
         resource. If a list is supplied the first item will be used if a resource type is not supplied; this could also
         be a parent(s) of any resource defined by the dict.
     :param full_clean: Perform a full clean as part of the creation.
     :param copy_dict: Use a copy of the input dictionary rather than destructively processing the input dict.
-    :param default_to_not_provided: If an value is not supplied keep the value as NOT_PROVIDED. This is used
+    :param default_to_not_provided: If a value is not supplied keep the value as NOT_PROVIDED. This is used
         to support merging an updated value.
     """
     if not isinstance(d, dict):
         raise TypeError("`d` must be a dict instance.")
 
     if copy_dict:
         d = d.copy()
@@ -728,15 +722,15 @@
             try:
                 value = f.to_python(value)
             except ValidationError as ve:
                 errors[f.name] = ve.error_messages
         attrs.append(value)
 
     # Stop if there are any errors
-    if errors:
+    if errors and full_clean:
         raise ValidationError(errors)
 
     # Create the new instance
     new_resource = resource_type(*attrs)
 
     if d:
         # If there are any extra attributes let the resource handle them
@@ -759,15 +753,15 @@
     """Generate an object graph from a dict
 
     :param d: Dictionary to build from
     :param resource: A resource type, resource name or list of resources and names to use as the base for creating a
         resource. If a list is supplied the first item will be used if a resource type is not supplied.
     :param full_clean: Perform a full clean once built; default is True
     :param copy_dict: Clone the dict before doing build; default is True
-    :param default_to_not_supplied: If an value is not supplied keep the value as NOT_PROVIDED. This is used
+    :param default_to_not_supplied: If a value is not supplied keep the value as NOT_PROVIDED. This is used
         to support merging an updated value.
     :raises ValidationError: During building of the object graph and issues discovered are raised as a ValidationError.
     """
     if isinstance(d, dict):
         return create_resource_from_dict(
             d, resource, full_clean, copy_dict, default_to_not_supplied
         )
@@ -786,9 +780,8 @@
 class ResourceIterable(bases.ResourceIterable):
     """Iterable that yields resources."""
 
     def __init__(self, sequence):
         self.sequence = sequence
 
     def __iter__(self):
-        for item in self.sequence:
-            yield item
+        yield from self.sequence
```

### Comparing `odin-2.6/src/odin/serializers.py` & `odin-2.8/src/odin/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import datetime
-from typing import Union, Callable, Any, Dict
+from typing import Any, Callable, Dict, Union
 
 from odin import datetimeutil
 from odin.compatibility import deprecated
 
 StringFormatter = Callable[[Any], str]
 STRING_TYPES: Dict[type, StringFormatter] = {}
```

### Comparing `odin-2.6/src/odin/traversal.py` & `odin-2.8/src/odin/traversal.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Traversal of a datastructure."""
 import itertools
-from typing import Union, Optional, NamedTuple, Sequence, cast, Iterable, List, Any
+from typing import Any, Iterable, List, NamedTuple, Optional, Sequence, Union, cast
 
 import odin
-from odin.exceptions import InvalidPathError, NoMatchError, MultipleMatchesError
+from odin.exceptions import InvalidPathError, MultipleMatchesError, NoMatchError
 from odin.resources import ResourceBase
 from odin.utils import getmeta
 
 
 class _NotSupplied:
     """Placeholder"""
 
@@ -80,28 +80,30 @@
     def extract_element(self, resource: ResourceBase) -> Any:
         """Extract an element from a resource instance"""
         key, value, attr = self
 
         try:
             field = getmeta(resource).field_map[attr]
         except KeyError:
-            raise InvalidPathError(self, f"Unknown field {attr!r}")
+            raise InvalidPathError(self, f"Unknown field {attr!r}") from None
         element = field.value_from_object(resource)
 
         if key is NotSupplied:
             # No additional lookup required
             return element
 
         elif value is NotSupplied:
             # Index or key into element
             key = cast(odin.CompositeField, field).key_to_python(key)
             try:
                 return element[key]
             except LookupError:
-                raise NoMatchError(self, f"Could not find index {key!r} in {field}.")
+                raise NoMatchError(
+                    self, f"Could not find index {key!r} in {field}."
+                ) from None
 
         else:
             # Filter elements
             if isinstance(element, dict):
                 element = element.values()
 
             values = tuple(r for r in element if getattr(r, key) == value)
```

### Comparing `odin-2.6/src/odin/utils/__init__.py` & `odin-2.8/src/odin/utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import re
 from typing import (
-    Iterable,
-    Tuple,
-    Union,
-    Set,
-    TypeVar,
-    Sequence,
     Any,
-    List,
     Dict,
+    Iterable,
     Iterator,
+    List,
     Optional,
+    Sequence,
+    Set,
+    Tuple,
+    TypeVar,
+    Union,
 )
 
 from odin.compatibility import deprecated
 
 _CAMEL_CASE_RE = re.compile(r"[A-Z]")
 _LOWER_UNDERSCORE_CASE_RE = re.compile(r"_([a-z])")
 _LOWER_DASH_CASE_RE = re.compile(r"-([a-z])")
@@ -158,15 +158,15 @@
 
     :param resource_or_instance: Resource or instance of a resource.
     :type resource_or_instance: Type[odin.resources.ResourceBase] | odin.resources.ResourceBase
     :return: Meta options class
     :rtype: odin.resources.ResourceOptions
 
     """
-    return getattr(resource_or_instance, "_meta")
+    return resource_or_instance._meta
 
 
 def field_iter(resource, include_virtual: bool = True) -> Iterator:
     """
     Return an iterator that yields fields from a resource.
 
     :param resource: Resource to iterate over.
```

### Comparing `odin-2.6/src/odin/utils/ipv6.py` & `odin-2.8/src/odin/utils/ipv6.py`

 * *Files identical despite different names*

### Comparing `odin-2.6/src/odin/validators.py` & `odin-2.8/src/odin/validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # This file is largely verbatim from the Django project, the wheel works well, no need to re-invent it.
 #
 # A note: to use validators from the Django project install the baldr package. Baldr is an integration between Odin and
 # the Django framework, the integration includes support for handling the Django version of the ValidationError
 # exception within Odin.
-from typing import Callable, Any, Union, TypeVar, Optional
-
 import re
+from typing import Any, Callable, Optional, TypeVar, Union
 
 from odin import exceptions
 from odin.utils.ipv6 import is_valid_ipv6_address
 
 EMPTY_VALUES = (None, "", [], (), {})
 
 
@@ -258,15 +257,15 @@
         validate_ipv4_address(value)
     except exceptions.ValidationError:
         try:
             validate_ipv6_address(value)
         except exceptions.ValidationError:
             raise exceptions.ValidationError(
                 "Enter a valid IPv4 or IPv6 address.", code="invalid"
-            )
+            ) from None
 
 
 class EmailValidator:
     """Validate is a valid email address format."""
 
     message = "Enter a valid email address."
     code = "invalid"
```

### Comparing `odin-2.6/tests/_helpers.py` & `odin-2.8/tests/_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+
 import pytest
 
 
 def assertJSONEqual(raw, expected_data, msg=None):
     """
     Assert that two JSON documents are the same.
     """
```

### Comparing `odin-2.6/tests/annotated_resources/test_type_resolution.py` & `odin-2.8/tests/annotated_resources/test_type_resolution.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import sys
-from typing import Optional, Union, List, Dict, Tuple, Any, Final
+from typing import Any, Dict, Final, List, Optional, Tuple, Union
 
 import pytest
 
 import odin
 from odin.annotated_resource import type_resolution
 from odin.annotated_resource.special_fields import AnyField
 
-from ..resources_annotated import From, Book
+from ..resources_annotated import Book, From
 
 
 class NonsenseField(odin.Field):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         raise TypeError("Nonsense!")
```

### Comparing `odin-2.6/tests/contrib/test_arrow_fields.py` & `odin-2.8/tests/contrib/test_arrow_fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-import arrow
 import datetime
+
+import arrow
 import pytest
 
 from odin.exceptions import ValidationError
 
 try:
     from odin.contrib.arrow.fields import ArrowField
 except ImportError:
```

### Comparing `odin-2.6/tests/contrib/test_geo_datatypes.py` & `odin-2.8/tests/contrib/test_geo_datatypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pytest
+
 from odin.contrib.geo import datatypes
 
 
 class TestDataTypes:
     def test_to_dms(self):
         # I am aware that round in python is not accurate but in this case I have calculated the test values
         # specifically so that the rounding will not effect the outcome of this test.
```

### Comparing `odin-2.6/tests/contrib/test_geo_fields.py` & `odin-2.8/tests/contrib/test_geo_fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pytest
-from odin.contrib.geo.datatypes import latitude, longitude, latlng, point
+
+from odin.contrib.geo.datatypes import latitude, latlng, longitude, point
 from odin.contrib.geo.fields import (
     LatitudeField,
-    LongitudeField,
     LatLngField,
+    LongitudeField,
     PointField,
 )
 from odin.exceptions import ValidationError
 
 
 class TestGeoFields:
     # LatitudeField ###########################################################
```

### Comparing `odin-2.6/tests/contrib/test_geo_serialisation.py` & `odin-2.8/tests/contrib/test_geo_serialisation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import odin
+from odin.codecs import json_codec
 from odin.contrib.geo import (
     LatitudeField,
-    LongitudeField,
     LatLngField,
+    LongitudeField,
     PointField,
     latitude,
-    longitude,
     latlng,
+    longitude,
     point,
 )
-from odin.codecs import json_codec
 
 
 class GeoResource(odin.Resource):
     class Meta:
         namespace = "odin.tests"
 
     lat_a = LatitudeField(null=True)
@@ -58,17 +58,17 @@
             '{"$": "odin.tests.GeoResource", '
             '"lat_a": null, "lat_b": 23.67, "lat_c": -23.67, '
             '"latlng_a": null, "latlng_b": [23.67, -123.56], '
             '"lng_a": null, "lng_b": 123.56, "lng_c": -123.56, '
             '"point_a": null, "point_b": [66.66, -33.33]}'
         )
 
-        assert None == resource.lat_a
+        assert None is resource.lat_a
         assert latitude(23.67) == resource.lat_b
         assert latitude(-23.67) == resource.lat_c
-        assert None == resource.lng_a
+        assert None is resource.lng_a
         assert longitude(123.56) == resource.lng_b
         assert longitude(-123.56) == resource.lng_c
-        assert None == resource.latlng_a
+        assert None is resource.latlng_a
         assert latlng(23.67, -123.56) == resource.latlng_b
-        assert None == resource.point_a
+        assert None is resource.point_a
         assert point(66.66, -33.33) == resource.point_b
```

### Comparing `odin-2.6/tests/contrib/test_money_datatypes.py` & `odin-2.8/tests/contrib/test_money_datatypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pytest
+
 from odin.contrib.money import datatypes
 
 a = datatypes.Amount(11)
 b = datatypes.Amount(22, "AUD")
 c = datatypes.Amount(33, "AUD")
 d = datatypes.Amount(44, "NZD")
 
@@ -17,15 +18,15 @@
         pytest.raises(TypeError, datatypes.Amount, None)
         pytest.raises(ValueError, datatypes.Amount, "abs")
         pytest.raises(TypeError, datatypes.Amount, 12, object())
         # Unknown currency
         pytest.raises(KeyError, datatypes.Amount, 12, "ZZZ")
         # From tuple
         assert "10.0000" == str(datatypes.Amount(("10",)))
-        assert "10.00 NZD", str(datatypes.Amount(("10" == "NZD")))
+        assert "10.00 NZD", str(datatypes.Amount("10" == "NZD"))
         pytest.raises(ValueError, datatypes.Amount, ("10", "NZD", "hmmm"))
 
     # These tests assume that the decimal library is correct.
 
     def test_amount_type_conversion(self):
         assert 12 == int(datatypes.Amount(12.345))
         assert 12.34 == float(datatypes.Amount(12.34))
```

### Comparing `odin-2.6/tests/contrib/test_money_fields.py` & `odin-2.8/tests/contrib/test_money_fields.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pytest
-from odin.contrib.money import AmountField
-from odin.contrib.money import Amount
+
+from odin.contrib.money import Amount, AmountField
 from odin.exceptions import ValidationError
 
 a = Amount(11)
 b = Amount(22, "AUD")
 c = Amount(33, "AUD")
 d = Amount(44, "NZD")
```

### Comparing `odin-2.6/tests/contrib/test_money_serialisation.py` & `odin-2.8/tests/contrib/test_money_serialisation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import odin
-from odin.contrib.money import AmountField
-from odin.contrib.money import Amount
 from odin.codecs import json_codec
+from odin.contrib.money import Amount, AmountField
 
 
 class AmountResource(odin.Resource):
     class Meta:
         namespace = "odin.tests"
 
     a = AmountField(null=True)
@@ -25,10 +24,10 @@
         )
 
     def test_deserialise(self):
         resource = json_codec.loads(
             '{"$": "odin.tests.AmountResource", "a": null, "b": 10, "c": [23.66, "AUD"]}'
         )
 
-        assert None == resource.a
+        assert None is resource.a
         assert Amount(10) == resource.b
         assert Amount(23.66, "AUD") == resource.c
```

### Comparing `odin-2.6/tests/contrib/test_pint_fields.py` & `odin-2.8/tests/contrib/test_pint_fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 
 from odin.exceptions import ValidationError
 
 try:
-    from odin.contrib.pint.fields import PintField, FloatField
+    from odin.contrib.pint.fields import FloatField, PintField
     from odin.contrib.pint.units import registry
 except ImportError:
     pass  # Pint is not available to pypy
 else:
 
     class TestPintFields:
         # PintField ###############################################################
```

### Comparing `odin-2.6/tests/fixtures/book-invalid.json` & `odin-2.8/tests/fixtures/book-invalid.json`

 * *Files identical despite different names*

### Comparing `odin-2.6/tests/fixtures/book-valid.json` & `odin-2.8/tests/fixtures/book-valid.json`

 * *Files identical despite different names*

### Comparing `odin-2.6/tests/fixtures/library.json` & `odin-2.8/tests/fixtures/library.json`

 * *Files identical despite different names*

### Comparing `odin-2.6/tests/fixtures/library.yaml` & `odin-2.8/tests/fixtures/library.yaml`

 * *Files identical despite different names*

### Comparing `odin-2.6/tests/resources.py` & `odin-2.8/tests/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import odin
 import enum
 
+import odin
 from odin.fields.virtual import CalculatedField
 from odin.mapping.helpers import sum_fields
 from odin.utils import snake_to_camel
 
 
 class Author(odin.Resource):
     name = odin.StringField()
@@ -231,9 +231,8 @@
         field_name_format = snake_to_camel
 
     full_name = odin.StringField()
     year_of_birth = odin.IntegerField()
 
 
 class InheritedCamelCaseResource(CamelCaseResource):
-
     email_address = odin.EmailField()
```

### Comparing `odin-2.6/tests/resources_annotated.py` & `odin-2.8/tests/resources_annotated.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,9 +107,8 @@
         field_name_format = snake_to_camel
 
     full_name: str
     year_of_birth: str
 
 
 class InheritedCamelCaseResource(CamelCaseResource):
-
     email_address: str
```

### Comparing `odin-2.6/tests/test_adapters.py` & `odin-2.8/tests/test_adapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from odin import adapters
 from odin.utils import field_iter_items
+
 from .resources import *
 
 
 class TestResourceOptionsAdapter:
     def test_repr(self):
         options = adapters.ResourceAdapter(Book())._meta
 
@@ -67,15 +68,15 @@
 
         assert "<ResourceAdapter: library.Book resource adapter>" == repr(target)
 
     def test_iter(self):
         book = Book(title="Foo", isbn="abc123", rrp=123.45, num_pages=10, fiction=True)
         target = adapters.ResourceAdapter(book)
 
-        actual = list((f.name, str(v)) for f, v in field_iter_items(target))
+        actual = [(f.name, str(v)) for f, v in field_iter_items(target)]
         assert [
             ("title", "Foo"),
             ("isbn", "abc123"),
             ("num_pages", "10"),
             ("rrp", "123.45"),
             ("fiction", "True"),
             ("genre", "None"),
```

### Comparing `odin-2.6/tests/test_annotated_resources.py` & `odin-2.8/tests/test_annotated_resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import datetime
 import json
 
 from odin.codecs import json_codec
 from odin.utils import getmeta, snake_to_camel
-
 from tests.resources_annotated import (
-    Book,
-    Publisher,
     Author,
-    Library,
+    Book,
     IdentifiableBook,
     InheritedCamelCaseResource,
+    Library,
+    Publisher,
 )
 
 
 class TestAnnotatedResourceType:
     def test_fields_are_identified_in_correct_order(self):
         meta = getmeta(Book)
```

### Comparing `odin-2.6/tests/test_codec_csv.py` & `odin-2.8/tests/test_codec_csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 from io import StringIO
 
 import pytest
+
 import odin
 import odin.exceptions
 from odin.codecs import csv_codec
 
 FIXTURE_PATH_ROOT = os.path.join(os.path.dirname(__file__), "fixtures")
 
 
@@ -47,23 +48,23 @@
 class TestReader:
     def open_fixture(self, file_name):
         return open(os.path.join(FIXTURE_PATH_ROOT, file_name))
 
     @pytest.mark.parametrize(
         "fixture options".split(),
         (
-            ("library-valid.csv", dict(includes_header=True)),
-            ("library-header-alt-order.csv", dict(includes_header=True)),
-            ("library-last-bad.csv", dict(includes_header=True)),
-            ("library-no-header.csv", dict(includes_header=False)),
+            ("library-valid.csv", {"includes_header": True}),
+            ("library-header-alt-order.csv", {"includes_header": True}),
+            ("library-last-bad.csv", {"includes_header": True}),
+            ("library-no-header.csv", {"includes_header": False}),
             (
                 "library-lower-header.csv",
-                dict(includes_header=True, ignore_header_case=True),
+                {"includes_header": True, "ignore_header_case": True},
             ),
-            ("library-valid.csv", dict(includes_header=True, strict_fields=True)),
+            ("library-valid.csv", {"includes_header": True, "strict_fields": True}),
         ),
     )
     def test_valid_libraries(self, fixture, options):
         with self.open_fixture(fixture) as f:
             target = csv_codec.reader(f, Book, **options)
             library = list(target)
         assert len(library) == 6
@@ -204,13 +205,13 @@
             target = csv_codec.reader(f, Book, includes_header=True)
             expected_library = list(target)
 
         temp_csv = os.path.join(str(tmpdir), "dump_test.csv")
         with open(temp_csv, "w") as f:
             csv_codec.dump(f, expected_library, include_header=True)
 
-        with open(temp_csv, "r") as f:
+        with open(temp_csv) as f:
             actual_library = list(csv_codec.reader(f, Book, includes_header=True))
 
         assert sorted(actual_library, key=lambda x: x.num_pages) == sorted(
             expected_library, key=lambda x: x.num_pages
         )
```

### Comparing `odin-2.6/tests/test_codec_dict.py` & `odin-2.8/tests/test_codec_dict.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import datetime
+
 from odin.codecs import dict_codec
+
 from .resources import *
 
 
 class TestDictCodec:
     def test_dump(self):
         in_resource = Book(
             title="Consider Phlebas",
```

### Comparing `odin-2.6/tests/test_codec_json.py` & `odin-2.8/tests/test_codec_json.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-import uuid
 import datetime
 import os
+import uuid
 from io import StringIO
 
 from odin.codecs import json_codec
+
 from .resources import *
 
 FIXTURE_PATH_ROOT = os.path.join(os.path.dirname(__file__), "fixtures")
 
 
 class TestJSONCodec:
     def test_dumps_and_loads(self):
```

### Comparing `odin-2.6/tests/test_codec_msgpack.py` & `odin-2.8/tests/test_codec_msgpack.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-import uuid
 import datetime
 import os
+import uuid
 from io import BytesIO
 
 from odin.codecs import msgpack_codec
+
 from .resources import *
 
 FIXTURE_PATH_ROOT = os.path.join(os.path.dirname(__file__), "fixtures")
 
 
 class TestMsgPackCodec:
     def test_dumps_and_loads(self):
```

### Comparing `odin-2.6/tests/test_codec_toml.py` & `odin-2.8/tests/test_codec_toml.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import datetime
 import os
 from io import StringIO
 
 import pytest
+
 from odin.codecs import toml_codec
 from odin.exceptions import CodecDecodeError, ValidationError
+
 from . import resources_annotated
 from .resources import *
 
 FIXTURE_PATH_ROOT = os.path.join(os.path.dirname(__file__), "fixtures")
 
 
 class CustomString:
```

### Comparing `odin-2.6/tests/test_codec_xml.py` & `odin-2.8/tests/test_codec_xml.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 from datetime import date
 
 from odin.codecs import xml_codec
+
 from .resources import *
 
 FIXTURE_PATH_ROOT = os.path.join(os.path.dirname(__file__), "fixtures")
 
 
 class Summary(odin.Resource):
     format = odin.StringField(is_attribute=True)
```

### Comparing `odin-2.6/tests/test_codec_yaml.py` & `odin-2.8/tests/test_codec_yaml.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import datetime
 import os
 from io import StringIO
 
 from odin.codecs import yaml_codec
+
 from .resources import *
 
 FIXTURE_PATH_ROOT = os.path.join(os.path.dirname(__file__), "fixtures")
 
 
 class TestYAMLCodec:
     def test_dumps_and_loads(self):
```

### Comparing `odin-2.6/tests/test_compatibility.py` & `odin-2.8/tests/test_compatibility.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 import warnings
+
 from odin.compatibility import deprecated
 
 
 class TestDeprecated:
     def test_function_deprecation_warning(self):
         @deprecated("No longer used.", category=UserWarning)
         def deprecated_function():
             pass
 
         with warnings.catch_warnings(record=True) as warning_log:
             deprecated_function()
 
         # Compare the message values
         assert [
-            str(m.message) for m in sorted(warning_log, key=lambda l: str(l.message))
+            str(m.message)
+            for m in sorted(warning_log, key=lambda log: str(log.message))
         ] == [
             "deprecated_function is deprecated and scheduled for removal. No longer used.",
         ]
 
     def test_class_deprecation_warning(self):
         @deprecated("No longer used.", category=UserWarning)
         class DeprecatedClass:
             pass
 
         with warnings.catch_warnings(record=True) as warning_log:
             DeprecatedClass()
 
         # Compare the message values
         assert [
-            str(m.message) for m in sorted(warning_log, key=lambda l: str(l.message))
+            str(m.message)
+            for m in sorted(warning_log, key=lambda log: str(log.message))
         ] == [
             "DeprecatedClass is deprecated and scheduled for removal. No longer used.",
         ]
```

### Comparing `odin-2.6/tests/test_datastructures.py` & `odin-2.8/tests/test_datastructures.py`

 * *Files identical despite different names*

### Comparing `odin-2.6/tests/test_datetimeutil.py` & `odin-2.8/tests/test_datetimeutil.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import pytest
 import datetime
 
+import pytest
+
 from odin import datetimeutil
 
 
 class TestTimezones:
     def test_fixed_timezone(self):
         target = datetimeutil.FixedTimezone.from_hours_minutes(10, 30)
```

### Comparing `odin-2.6/tests/test_decorators.py` & `odin-2.8/tests/test_decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pytest
 
 from odin import decorators
 from odin.codecs import json_codec
 from odin.exceptions import ValidationError
+
 from .resources import Author
 
 
 class TestDecorators:
     def test_returns_resource(self):
         @decorators.returns_resource(resource=Author)
         def test():
```

### Comparing `odin-2.6/tests/test_exceptions.py` & `odin-2.8/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `odin-2.6/tests/test_fields.py` & `odin-2.8/tests/test_fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-import pathlib
-import re
-
-import pytest
 import datetime
 import enum
+import pathlib
+import re
 import uuid
 from copy import deepcopy
 
+import pytest
+
 import odin
-from odin.fields import *
-from odin.fields import Field, TimeStampField, NotProvided
 from odin.datetimeutil import FixedTimezone
+from odin.exceptions import ValidationError
+from odin.fields import *
+from odin.fields import Field, NotProvided, TimeStampField
 from odin.fields.virtual import VirtualField
 from odin.validators import (
-    MinValueValidator,
-    MaxValueValidator,
     MaxLengthValidator,
-    RegexValidator,
+    MaxValueValidator,
     MinLengthValidator,
+    MinValueValidator,
+    RegexValidator,
 )
-from odin.exceptions import ValidationError
 
 utc = datetime.timezone.utc
 
 
 class ObjectValue:
     pass
 
@@ -162,15 +162,15 @@
         assert "321" == target.get_default()
 
     def test_value_from_object(self):
         target = FieldTest()
         target.set_attributes_from_name("test_name")
 
         an_obj = ObjectValue()
-        setattr(an_obj, "test_name", "test_value")
+        an_obj.test_name = "test_value"
 
         actual = target.value_from_object(an_obj)
         assert "test_value" == actual
 
     def test__repr(self):
         target = Field()
         assert "<odin.fields.Field>" == repr(target)
@@ -386,41 +386,41 @@
     # URLField ################################################################
 
     def test_urlfield_1(self):
         f = UrlField()
         assert "http://www.github.com" == f.clean("http://www.github.com")
         pytest.raises(ValidationError, f.clean, "eek")
         pytest.raises(ValidationError, f.clean, None)
-        assert f.max_length == None
+        assert f.max_length is None
         self.assert_validator_in(RegexValidator, f.validators)
 
     # IntegerField ############################################################
 
     def test_integerfield_1(self):
         f = IntegerField()
         pytest.raises(ValidationError, f.clean, None)
         pytest.raises(ValidationError, f.clean, "abc")
         assert 123 == f.clean(123)
         assert 123 == f.clean("123")
         assert 123 == f.clean(123.5)
-        assert None == f.min_value
+        assert None is f.min_value
         self.assert_validator_not_in(MinValueValidator, f.validators)
-        assert None == f.max_value
+        assert None is f.max_value
         self.assert_validator_not_in(MaxValueValidator, f.validators)
 
     def test_integerfield_2(self):
         f = IntegerField(null=True)
-        assert None == f.clean(None)
+        assert None is f.clean(None)
         pytest.raises(ValidationError, f.clean, "abc")
         assert 69 == f.clean(69)
         assert 69 == f.clean("69")
         assert 69 == f.clean(69.5)
-        assert None == f.min_value
+        assert None is f.min_value
         self.assert_validator_not_in(MinValueValidator, f.validators)
-        assert None == f.max_value
+        assert None is f.max_value
         self.assert_validator_not_in(MaxValueValidator, f.validators)
 
     def test_integerfield_3(self):
         f = IntegerField(min_value=50, max_value=100)
         pytest.raises(ValidationError, f.clean, None)
         pytest.raises(ValidationError, f.clean, "abc")
         assert 69 == f.clean(69)
@@ -440,29 +440,29 @@
     def test_floatfield_1(self):
         f = FloatField()
         pytest.raises(ValidationError, f.clean, None)
         pytest.raises(ValidationError, f.clean, "abc")
         assert 123 == f.clean(123)
         assert 123.5 == f.clean("123.5")
         assert 123.5 == f.clean(123.5)
-        assert None == f.min_value
+        assert None is f.min_value
         self.assert_validator_not_in(MinValueValidator, f.validators)
-        assert None == f.max_value
+        assert None is f.max_value
         self.assert_validator_not_in(MaxValueValidator, f.validators)
 
     def test_floatfield_2(self):
         f = FloatField(null=True)
         assert f.clean(None) is None
         pytest.raises(ValidationError, f.clean, "abc")
         assert 69 == f.clean(69)
         assert 69.5 == f.clean("69.5")
         assert 69.5 == f.clean(69.5)
-        assert None == f.min_value
+        assert None is f.min_value
         self.assert_validator_not_in(MinValueValidator, f.validators)
-        assert None == f.max_value
+        assert None is f.max_value
         self.assert_validator_not_in(MaxValueValidator, f.validators)
 
     def test_floatfield_3(self):
         f = FloatField(min_value=50.5, max_value=100.4)
         pytest.raises(ValidationError, f.clean, None)
         pytest.raises(ValidationError, f.clean, "abc")
         assert 69 == f.clean(69)
@@ -879,15 +879,15 @@
         assert [] == f.clean([])
         assert ["foo", "bar"], f.clean(["foo" == "bar"])
         assert ["foo", "bar", "$", "eek"], f.clean(["foo", "bar", "$" == "eek"])
         assert f.default == list
 
     def test_listfield__where_null_is_true(self):
         f = ListField(null=True)
-        assert None == f.clean(None)
+        assert None is f.clean(None)
         pytest.raises(ValidationError, f.clean, "abc")
         pytest.raises(ValidationError, f.clean, 123)
         assert [] == f.clean([])
         assert ["foo", "bar"], f.clean(["foo" == "bar"])
         assert ["foo", "bar", "$", "eek"], f.clean(["foo", "bar", "$" == "eek"])
 
     def test_listfield__validators_are_executed_on_empty(self):
@@ -966,15 +966,15 @@
         assert {} == f.clean({})
         pytest.raises(ValidationError, f.clean, {"foo": "bar"})
         assert {"foo": 1} == f.clean({"foo": 1})
 
     def test_typeddictfield_2(self):
         f = TypedDictField(IntegerField(), null=True)
         assert "Dict<String, Integer>" == f.data_type_name(f)
-        assert None == f.clean(None)
+        assert None is f.clean(None)
         pytest.raises(ValidationError, f.clean, "abc")
         pytest.raises(ValidationError, f.clean, 123)
         assert {} == f.clean({})
         pytest.raises(ValidationError, f.clean, {"foo": "bar"})
         assert {"foo": 1} == f.clean({"foo": 1})
 
     def test_typeddictfield_3(self):
```

### Comparing `odin-2.6/tests/test_fields_composite.py` & `odin-2.8/tests/test_fields_composite.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 
 import odin
 from odin.exceptions import ValidationError
-from odin.fields.composite import DictAs, ArrayOf, DictOf
+from odin.fields.composite import ArrayOf, DictAs, DictOf
 
 
 class ExampleResource(odin.Resource):
     name = odin.StringField()
 
 
 class TestFields:
```

### Comparing `odin-2.6/tests/test_fields_virtual.py` & `odin-2.8/tests/test_fields_virtual.py`

 * *Files identical despite different names*

### Comparing `odin-2.6/tests/test_filtering.py` & `odin-2.8/tests/test_filtering.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import pytest
 import os
 
+import pytest
+
 from odin import filtering
-from odin.traversal import TraversalPath
 from odin.codecs import json_codec
-
+from odin.traversal import TraversalPath
 
 # Open library fixture
 with open(os.path.join(os.path.dirname(__file__), "fixtures", "library.json")) as f:
     library = json_codec.load(f)
 
 first_book = TraversalPath.parse("books[0]").get_value(library)
```

### Comparing `odin-2.6/tests/test_helpers.py` & `odin-2.8/tests/test_helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pytest
 
 from odin import helpers
 from odin.exceptions import ValidationError
 from odin.utils import getmeta
+
 from .resources import Author
 
 
 class TestValidationErrorCollection:
     def test_messages__with_valid_message(self):
         target = helpers.ValidationErrorCollection()
```

### Comparing `odin-2.6/tests/test_mapping.py` & `odin-2.8/tests/test_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-import pytest
 import datetime
 
-from odin.exceptions import MappingSetupError, MappingExecutionError
+import pytest
+
+from odin.exceptions import MappingExecutionError, MappingSetupError
 from odin.fields import NotProvided
-from odin.mapping import MappingResult, FieldMapping
+from odin.mapping import FieldMapping, MappingResult
 from odin.mapping.helpers import MapDictAs, MapListOf, NoOpMapper
+
 from .resources import *
 
 
 class SimpleFromResource(odin.Resource):
     title = odin.StringField()
 
 
@@ -25,15 +27,15 @@
 class SimpleFromTo(odin.Mapping):
     from_obj = SimpleFromResource
     to_obj = SimpleToResource
 
     @odin.map_field(from_field="title")
     def title_count(self, value):
         if self.in_loop:
-            return "%s: %s" % (self.loop_idx, value)
+            return f"{self.loop_idx}: {value}"
         else:
             return value
 
 
 def assertMappingEquivalent(a, b):
     flat_a = sorted(str(i) for i in a)
     flat_b = sorted(str(i) for i in b)
@@ -521,16 +523,16 @@
 class TestSubClassMapping:
     """
     Test the concept of a sub class mapping ie
 
                 Resource A          -->         Mapping A-X         -->           Resource X
                     |                                |                                |
                _____|_____                      _____|_____                      _____|_____
-              /           \                    /           \                    /           \
-             /            \                   /            \                   /            \
+              /           \\                    /           \\                    /           \
+             /            \\                   /            \\                   /            \
         Resource B    Resource C         Mapping B-Y   Mapping C-Z        Resource Y    Resource Z
 
     Define a mapping that can handle a list of *Resource A* and *Resource B* objects being mapped by an abstract mapping
     *Mapping A-X* to the corresponding *Resource Y* and *Resource Z* objects.
 
     """
```

### Comparing `odin-2.6/tests/test_mapping_helpers.py` & `odin-2.8/tests/test_mapping_helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pytest
+
 from odin.mapping import helpers
 
 
 class TestMappingHelpers:
     def test_sum_fields(self):
         actual = helpers.sum_fields(22, 20)
```

### Comparing `odin-2.6/tests/test_polymorphic.py` & `odin-2.8/tests/test_polymorphic.py`

 * *Files identical despite different names*

### Comparing `odin-2.6/tests/test_proxy.py` & `odin-2.8/tests/test_proxy.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 
+from odin import proxy
 from odin.resources import create_resource_from_dict
 from odin.utils import getmeta
-from odin import proxy
 
 from .resources import Book, BookProxy
 
 
 class MockObject:
     def __init__(self, **kwargs):
         self.__dict__.update(kwargs)
```

### Comparing `odin-2.6/tests/test_resource_base.py` & `odin-2.8/tests/test_resource_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pytest
 
 import odin
+
 from . import resources
 
 
 class TestResourceBase:
     def test_virtual_fields(self):
         target = resources.FromResource()
```

### Comparing `odin-2.6/tests/test_resources.py` & `odin-2.8/tests/test_resources.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import pytest
 
 import odin
+from odin.exceptions import ResourceDefError, ValidationError
 from odin.fields import NotProvided
 from odin.resources import (
+    Resource,
     ResourceOptions,
     build_object_graph,
     create_resource_from_dict,
-    Resource,
 )
-from odin.exceptions import ValidationError, ResourceDefError
 from odin.utils import getmeta, snake_to_camel
-from .resources import Book, BookProxy, Library, Subscriber, InheritedCamelCaseResource
+
+from .resources import Book, BookProxy, InheritedCamelCaseResource, Library, Subscriber
 
 
 class Author(odin.Resource):
     name = odin.StringField()
     country = odin.StringField(null=True)
 
     def clean(self):
@@ -226,74 +227,68 @@
                 fields = odin.StringField()
 
 
 class TestConstructionMethods:
     def test_build_object_graph_empty_dict_no_clean(self):
         book = build_object_graph({}, Book, full_clean=False)
 
-        assert (
-            dict(
-                title=None,
-                isbn=None,
-                num_pages=None,
-                rrp=20.4,
-                fiction=None,
-                genre=None,
-                published=None,
-                authors=None,
-                publisher=None,
-            )
-            == book.to_dict()
-        )
+        assert {
+            "title": None,
+            "isbn": None,
+            "num_pages": None,
+            "rrp": 20.4,
+            "fiction": None,
+            "genre": None,
+            "published": None,
+            "authors": None,
+            "publisher": None,
+        } == book.to_dict()
 
     def test_build_object_graph_empty_dict(self):
         with pytest.raises(ValidationError) as ctx:
             build_object_graph({}, Book)
 
-        assert (
-            dict(
-                title=["This field cannot be null."],
-                isbn=["This field cannot be null."],
-                num_pages=["This field cannot be null."],
-                fiction=["This field cannot be null."],
-                genre=["This field cannot be null."],
-                published=["This field cannot be null."],
-                authors=["List cannot contain null entries."],
-            )
-            == ctx.value.error_messages
-        )
+        assert {
+            "title": ["This field cannot be null."],
+            "isbn": ["This field cannot be null."],
+            "num_pages": ["This field cannot be null."],
+            "fiction": ["This field cannot be null."],
+            "genre": ["This field cannot be null."],
+            "published": ["This field cannot be null."],
+            "authors": ["List cannot contain null entries."],
+        } == ctx.value.error_messages
 
     def test_build_object_graph_from_list(self):
         books = build_object_graph(
-            [dict(title="Book1"), dict(title="Book2")], Book, full_clean=False
+            [{"title": "Book1"}, {"title": "Book2"}], Book, full_clean=False
         )
 
         assert [
-            dict(
-                title="Book1",
-                isbn=None,
-                num_pages=None,
-                rrp=20.4,
-                fiction=None,
-                genre=None,
-                published=None,
-                authors=None,
-                publisher=None,
-            ),
-            dict(
-                title="Book2",
-                isbn=None,
-                num_pages=None,
-                rrp=20.4,
-                fiction=None,
-                genre=None,
-                published=None,
-                authors=None,
-                publisher=None,
-            ),
+            {
+                "title": "Book1",
+                "isbn": None,
+                "num_pages": None,
+                "rrp": 20.4,
+                "fiction": None,
+                "genre": None,
+                "published": None,
+                "authors": None,
+                "publisher": None,
+            },
+            {
+                "title": "Book2",
+                "isbn": None,
+                "num_pages": None,
+                "rrp": 20.4,
+                "fiction": None,
+                "genre": None,
+                "published": None,
+                "authors": None,
+                "publisher": None,
+            },
         ] == [book.to_dict() for book in books]
 
     def test_build_nested_objects(self):
         subscribers = [
             {"name": "John Smith", "address": "Oak Lane 1234"},
             {"name": "Johnny Smith", "address": "Oak Lane 1235"},
         ]
@@ -355,46 +350,40 @@
         book = create_resource_from_dict(
             {"title": "Foo", "num_pages": 42},
             Book,
             full_clean=False,
             default_to_not_provided=True,
         )
 
-        assert (
-            dict(
-                title="Foo",
-                isbn=NotProvided,
-                num_pages=42,
-                rrp=NotProvided,
-                fiction=NotProvided,
-                genre=NotProvided,
-                published=NotProvided,
-                authors=NotProvided,
-                publisher=NotProvided,
-            )
-            == book.to_dict()
-        )
+        assert {
+            "title": "Foo",
+            "isbn": NotProvided,
+            "num_pages": 42,
+            "rrp": NotProvided,
+            "fiction": NotProvided,
+            "genre": NotProvided,
+            "published": NotProvided,
+            "authors": NotProvided,
+            "publisher": NotProvided,
+        } == book.to_dict()
 
     def test_create_resource_from_dict__with_proxy(self):
         book = create_resource_from_dict(
             {"title": "Foo", "num_pages": 42, "rrp": 10000.99, "fiction": True},
             BookProxy,
             full_clean=False,
             default_to_not_provided=True,
         )
 
-        assert (
-            dict(
-                title="Foo",
-                isbn=NotProvided,
-                num_pages=42,
-                rrp=20.4,
-            )
-            == book.to_dict()
-        )
+        assert {
+            "title": "Foo",
+            "isbn": NotProvided,
+            "num_pages": 42,
+            "rrp": 20.4,
+        } == book.to_dict()
 
     def test_inheritance_of_meta_options(self):
         options = getmeta(InheritedCamelCaseResource)
 
         assert options.resource_name == "foo.bar.InheritedCamelCaseResource"
         assert options.field_name_format is snake_to_camel
```

### Comparing `odin-2.6/tests/test_serializers.py` & `odin-2.8/tests/test_serializers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import datetime
 
-from odin import datetimeutil
-from odin import serializers
+from odin import datetimeutil, serializers
 
 
 class TestSerializer:
     def test_date_iso_format(self):
         assert "2014-01-16" == serializers.date_iso_format(datetime.date(2014, 1, 16))
 
     def test_time_iso_format(self):
```

### Comparing `odin-2.6/tests/test_traversal.py` & `odin-2.8/tests/test_traversal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pytest
 
 import odin
 from odin import traversal
-from odin.exceptions import NoMatchError, InvalidPathError, MultipleMatchesError
+from odin.exceptions import InvalidPathError, MultipleMatchesError, NoMatchError
 
 
 class Level3(odin.Resource):
     class Meta:
         key_field_name = "name"
         namespace = "odin.traversal"
 
@@ -30,41 +30,41 @@
     level2 = odin.DictAs(Level2)
     level2s = odin.DictOf(Level2)
 
 
 TEST_STRUCTURE = Level1(
     name="a",
     level2=Level2(name="b", level3s=[]),
-    level2s=dict(
-        a=Level2(name="c", level3s=[]),
-        b=Level2(
+    level2s={
+        "a": Level2(name="c", level3s=[]),
+        "b": Level2(
             name="d", label="not_empty", level3s=[Level3(name="e"), Level3(name="f")]
         ),
-        c=Level2(name="g", label="not_empty", level3s=[Level3(name="h")]),
-    ),
+        "c": Level2(name="g", label="not_empty", level3s=[Level3(name="h")]),
+    },
 )
 
 TEST_LIST_STRUCTURE = [
     Level1(
         name="a",
         level2=Level2(name="b", level3s=[]),
-        level2s=dict(
-            a=Level2(name="c", level3s=[]),
-            b=Level2(name="d", level3s=[Level3(name="e"), Level3(name="f")]),
-            c=Level2(name="g", level3s=[Level3(name="h")]),
-        ),
+        level2s={
+            "a": Level2(name="c", level3s=[]),
+            "b": Level2(name="d", level3s=[Level3(name="e"), Level3(name="f")]),
+            "c": Level2(name="g", level3s=[Level3(name="h")]),
+        },
     ),
     Level1(
         name="i",
         level2=Level2(name="j", level3s=[]),
-        level2s=dict(
-            a=Level2(name="k", level3s=[]),
-            b=Level2(name="l", level3s=[Level3(name="m"), Level3(name="n")]),
-            c=Level2(name="o", level3s=[Level3(name="p")]),
-        ),
+        level2s={
+            "a": Level2(name="k", level3s=[]),
+            "b": Level2(name="l", level3s=[Level3(name="m"), Level3(name="n")]),
+            "c": Level2(name="o", level3s=[Level3(name="p")]),
+        },
     ),
 ]
 
 
 class ResourceTraversalIteratorTest(traversal.ResourceTraversalIterator):
     def __init__(self, resource):
         super().__init__(resource)
```

### Comparing `odin-2.6/tests/test_utils.py` & `odin-2.8/tests/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pytest
 
-from odin.utils import getmeta
 from odin import utils
+from odin.utils import getmeta
+
 from .resources import Book
 
 
 class TestCamelAndDashFormats:
     def test_camel_to_lower_separated(self):
         assert "this_is_an_example" == utils.camel_to_lower_underscore(
             "thisIsAnExample"
```

### Comparing `odin-2.6/tests/test_validators.py` & `odin-2.8/tests/test_validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,48 +66,48 @@
 
     def test_max_value_validator(self):
         target = validators.MaxValueValidator(10)
 
         target(10)
         target(1)
         target(-10)
-        assert str(target) == 'Value is less than or equal to 10.'
+        assert str(target) == "Value is less than or equal to 10."
         pytest.raises(ValidationError, target, 11)
 
     def test_min_value_validator(self):
         target = validators.MinValueValidator(10)
 
         target(10)
         target(11)
-        assert str(target) == 'Value is greater than or equal to 10.'
+        assert str(target) == "Value is greater than or equal to 10."
         pytest.raises(ValidationError, target, 1)
         pytest.raises(ValidationError, target, -10)
 
     def test_length_validator(self):
         target = validators.LengthValidator(10)
 
         target("1234567890")
-        assert str(target) == 'Values length is 10.'
+        assert str(target) == "Values length is 10."
         pytest.raises(ValidationError, target, "123456789")
         pytest.raises(ValidationError, target, "12345678901")
 
     def test_max_length_validator(self):
         target = validators.MaxLengthValidator(10)
 
         target("123457890")
         target("12345")
         target("")
-        assert str(target) == 'Values length is at most 10.'
+        assert str(target) == "Values length is at most 10."
         pytest.raises(ValidationError, target, "12345678901")
 
     def test_min_length_validator(self):
         target = validators.MinLengthValidator(10)
 
         target("12345678901")
-        assert str(target) == 'Values length is at least 10.'
+        assert str(target) == "Values length is at least 10."
         pytest.raises(ValidationError, target, "123457890")
         pytest.raises(ValidationError, target, "12345")
         pytest.raises(ValidationError, target, "")
 
 
 class TestSimpleValidator:
     def test_method(self):
@@ -268,15 +268,15 @@
 @pytest.mark.parametrize(
     "value kwargs".split(),
     (
         ("foo", None),
         (".foo@bar.com", None),
         ("foo@corpau", None),
         ("foo@localhost", {"whitelist": ""}),
-        ("foo@{0}.com".format("a" * 64), None),
+        ("foo@{}.com".format("a" * 64), None),
         ("foo@[::ff::0]", None),
     ),
 )
 def test_validate_email_invalid(value, kwargs):
     kwargs = kwargs or {}
     with pytest.raises(ValidationError):
         validators.EmailValidator(**kwargs)(value)
```

### Comparing `odin-2.6/PKG-INFO` & `odin-2.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odin
-Version: 2.6
+Version: 2.8
 Summary: Data-structure definition/validation/traversal, mapping and serialisation toolkit for Python
 Home-page: https://github.com/python-odin/odin
 License: BSD-3-Clause
 Keywords: data-structure,validation,data-mapping
 Author: Tim Savage
 Author-email: tim@savage.company
 Requires-Python: >=3.8,<4.0
@@ -14,18 +14,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: arrow
 Provides-Extra: msgpack
 Provides-Extra: pint
```

