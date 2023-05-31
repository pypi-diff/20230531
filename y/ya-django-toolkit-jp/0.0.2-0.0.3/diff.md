# Comparing `tmp/ya_django_toolkit_jp-0.0.2.tar.gz` & `tmp/ya_django_toolkit_jp-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ya_django_toolkit_jp-0.0.2.tar", max compression
+gzip compressed data, was "ya_django_toolkit_jp-0.0.3.tar", max compression
```

## Comparing `ya_django_toolkit_jp-0.0.2.tar` & `ya_django_toolkit_jp-0.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1173 2023-05-26 18:38:18.080408 ya_django_toolkit_jp-0.0.2/CHANGELOG.md
--rw-r--r--   0        0        0      292 2023-05-26 18:38:18.080408 ya_django_toolkit_jp-0.0.2/README.md
--rw-r--r--   0        0        0     1335 2023-05-26 18:38:18.080408 ya_django_toolkit_jp-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-26 18:38:18.080408 ya_django_toolkit_jp-0.0.2/ya_django_toolkit_jp/__init__.py
--rw-r--r--   0        0        0      169 2023-05-26 18:38:18.080408 ya_django_toolkit_jp-0.0.2/ya_django_toolkit_jp/apps.py
--rw-r--r--   0        0        0        0 2023-05-26 18:38:18.080408 ya_django_toolkit_jp-0.0.2/ya_django_toolkit_jp/base/__init__.py
--rw-r--r--   0        0        0      186 2023-05-26 18:38:18.080408 ya_django_toolkit_jp-0.0.2/ya_django_toolkit_jp/base/models/__init__.py
--rw-r--r--   0        0        0      139 2023-05-26 18:38:18.080408 ya_django_toolkit_jp-0.0.2/ya_django_toolkit_jp/base/models/base.py
--rw-r--r--   0        0        0      183 2023-05-26 18:38:18.080408 ya_django_toolkit_jp-0.0.2/ya_django_toolkit_jp/base/models/base_ulid.py
--rw-r--r--   0        0        0      175 2023-05-26 18:38:18.080408 ya_django_toolkit_jp-0.0.2/ya_django_toolkit_jp/base/models/base_uuid.py
--rw-r--r--   0        0        0      212 2023-05-26 18:38:18.080408 ya_django_toolkit_jp-0.0.2/ya_django_toolkit_jp/base/models/ulid.py
--rw-r--r--   0        0        0     1292 2023-05-26 18:38:18.084408 ya_django_toolkit_jp-0.0.2/ya_django_toolkit_jp/base_app_settings.py
--rw-r--r--   0        0        0      109 2023-05-26 18:38:18.084408 ya_django_toolkit_jp-0.0.2/ya_django_toolkit_jp/fields/__init__.py
--rw-r--r--   0        0        0      366 2023-05-26 18:38:18.084408 ya_django_toolkit_jp-0.0.2/ya_django_toolkit_jp/fields/normalize_char_field.py
--rw-r--r--   0        0        0      743 2023-05-26 18:38:18.084408 ya_django_toolkit_jp-0.0.2/ya_django_toolkit_jp/fields/ulid.py
--rw-r--r--   0        0        0        0 2023-05-26 18:38:18.084408 ya_django_toolkit_jp-0.0.2/ya_django_toolkit_jp/ja/__init__.py
--rw-r--r--   0        0        0      118 2023-05-26 18:38:18.084408 ya_django_toolkit_jp-0.0.2/ya_django_toolkit_jp/ja/fields/__init__.py
--rw-r--r--   0        0        0      399 2023-05-26 18:38:18.084408 ya_django_toolkit_jp-0.0.2/ya_django_toolkit_jp/ja/fields/hiragana_char.py
--rw-r--r--   0        0        0      399 2023-05-26 18:38:18.084408 ya_django_toolkit_jp-0.0.2/ya_django_toolkit_jp/ja/fields/katakana_char.py
--rw-r--r--   0        0        0     1955 2023-05-26 18:38:18.084408 ya_django_toolkit_jp-0.0.2/ya_django_toolkit_jp/ja/utils.py
--rw-r--r--   0        0        0      130 2023-05-26 18:38:18.084408 ya_django_toolkit_jp-0.0.2/ya_django_toolkit_jp/ja/validators/__init__.py
--rw-r--r--   0        0        0      200 2023-05-26 18:38:18.084408 ya_django_toolkit_jp-0.0.2/ya_django_toolkit_jp/ja/validators/hiragana_only.py
--rw-r--r--   0        0        0      200 2023-05-26 18:38:18.084408 ya_django_toolkit_jp-0.0.2/ya_django_toolkit_jp/ja/validators/katakana_only.py
--rw-r--r--   0        0        0        0 2023-05-26 18:38:18.084408 ya_django_toolkit_jp-0.0.2/ya_django_toolkit_jp/templatetags/__init__.py
--rw-r--r--   0        0        0      832 2023-05-26 18:38:18.084408 ya_django_toolkit_jp-0.0.2/ya_django_toolkit_jp/templatetags/ya_django_toolkit_jp.py
--rw-r--r--   0        0        0        0 2023-05-26 18:38:18.084408 ya_django_toolkit_jp-0.0.2/ya_django_toolkit_jp/utils/__init__.py
--rw-r--r--   0        0        0      624 2023-05-26 18:38:18.084408 ya_django_toolkit_jp-0.0.2/ya_django_toolkit_jp/utils/file.py
--rw-r--r--   0        0        0     2031 2023-05-26 18:38:18.084408 ya_django_toolkit_jp-0.0.2/ya_django_toolkit_jp/utils/ip.py
--rw-r--r--   0        0        0      711 2023-05-26 18:38:18.084408 ya_django_toolkit_jp-0.0.2/ya_django_toolkit_jp/utils/ipv6.py
--rw-r--r--   0        0        0      206 2023-05-26 18:38:18.084408 ya_django_toolkit_jp-0.0.2/ya_django_toolkit_jp/utils/mimetypes.py
--rw-r--r--   0        0        0      508 2023-05-26 18:38:18.084408 ya_django_toolkit_jp-0.0.2/ya_django_toolkit_jp/utils/view.py
--rw-r--r--   0        0        0     1028 1970-01-01 00:00:00.000000 ya_django_toolkit_jp-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1471 2023-05-31 02:03:13.614296 ya_django_toolkit_jp-0.0.3/CHANGELOG.md
+-rw-r--r--   0        0        0      292 2023-05-31 02:03:13.614296 ya_django_toolkit_jp-0.0.3/README.md
+-rw-r--r--   0        0        0     1335 2023-05-31 02:03:13.614296 ya_django_toolkit_jp-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-31 02:03:13.618296 ya_django_toolkit_jp-0.0.3/ya_django_toolkit_jp/__init__.py
+-rw-r--r--   0        0        0      169 2023-05-31 02:03:13.618296 ya_django_toolkit_jp-0.0.3/ya_django_toolkit_jp/apps.py
+-rw-r--r--   0        0        0        0 2023-05-31 02:03:13.618296 ya_django_toolkit_jp-0.0.3/ya_django_toolkit_jp/base/__init__.py
+-rw-r--r--   0        0        0      186 2023-05-31 02:03:13.618296 ya_django_toolkit_jp-0.0.3/ya_django_toolkit_jp/base/models/__init__.py
+-rw-r--r--   0        0        0      139 2023-05-31 02:03:13.618296 ya_django_toolkit_jp-0.0.3/ya_django_toolkit_jp/base/models/base.py
+-rw-r--r--   0        0        0      183 2023-05-31 02:03:13.618296 ya_django_toolkit_jp-0.0.3/ya_django_toolkit_jp/base/models/base_ulid.py
+-rw-r--r--   0        0        0      175 2023-05-31 02:03:13.618296 ya_django_toolkit_jp-0.0.3/ya_django_toolkit_jp/base/models/base_uuid.py
+-rw-r--r--   0        0        0      212 2023-05-31 02:03:13.618296 ya_django_toolkit_jp-0.0.3/ya_django_toolkit_jp/base/models/ulid.py
+-rw-r--r--   0        0        0     1292 2023-05-31 02:03:13.618296 ya_django_toolkit_jp-0.0.3/ya_django_toolkit_jp/base_app_settings.py
+-rw-r--r--   0        0        0      109 2023-05-31 02:03:13.618296 ya_django_toolkit_jp-0.0.3/ya_django_toolkit_jp/fields/__init__.py
+-rw-r--r--   0        0        0      366 2023-05-31 02:03:13.618296 ya_django_toolkit_jp-0.0.3/ya_django_toolkit_jp/fields/normalize_char_field.py
+-rw-r--r--   0        0        0      743 2023-05-31 02:03:13.618296 ya_django_toolkit_jp-0.0.3/ya_django_toolkit_jp/fields/ulid.py
+-rw-r--r--   0        0        0        0 2023-05-31 02:03:13.618296 ya_django_toolkit_jp-0.0.3/ya_django_toolkit_jp/ja/__init__.py
+-rw-r--r--   0        0        0      118 2023-05-31 02:03:13.618296 ya_django_toolkit_jp-0.0.3/ya_django_toolkit_jp/ja/fields/__init__.py
+-rw-r--r--   0        0        0      399 2023-05-31 02:03:13.618296 ya_django_toolkit_jp-0.0.3/ya_django_toolkit_jp/ja/fields/hiragana_char.py
+-rw-r--r--   0        0        0      399 2023-05-31 02:03:13.618296 ya_django_toolkit_jp-0.0.3/ya_django_toolkit_jp/ja/fields/katakana_char.py
+-rw-r--r--   0        0        0     1955 2023-05-31 02:03:13.618296 ya_django_toolkit_jp-0.0.3/ya_django_toolkit_jp/ja/utils.py
+-rw-r--r--   0        0        0      130 2023-05-31 02:03:13.618296 ya_django_toolkit_jp-0.0.3/ya_django_toolkit_jp/ja/validators/__init__.py
+-rw-r--r--   0        0        0      200 2023-05-31 02:03:13.618296 ya_django_toolkit_jp-0.0.3/ya_django_toolkit_jp/ja/validators/hiragana_only.py
+-rw-r--r--   0        0        0      200 2023-05-31 02:03:13.618296 ya_django_toolkit_jp-0.0.3/ya_django_toolkit_jp/ja/validators/katakana_only.py
+-rw-r--r--   0        0        0        0 2023-05-31 02:03:13.618296 ya_django_toolkit_jp-0.0.3/ya_django_toolkit_jp/templatetags/__init__.py
+-rw-r--r--   0        0        0     1088 2023-05-31 02:03:13.618296 ya_django_toolkit_jp-0.0.3/ya_django_toolkit_jp/templatetags/ya_django_toolkit_jp.py
+-rw-r--r--   0        0        0        0 2023-05-31 02:03:13.618296 ya_django_toolkit_jp-0.0.3/ya_django_toolkit_jp/utils/__init__.py
+-rw-r--r--   0        0        0      624 2023-05-31 02:03:13.618296 ya_django_toolkit_jp-0.0.3/ya_django_toolkit_jp/utils/file.py
+-rw-r--r--   0        0        0     2031 2023-05-31 02:03:13.618296 ya_django_toolkit_jp-0.0.3/ya_django_toolkit_jp/utils/ip.py
+-rw-r--r--   0        0        0      711 2023-05-31 02:03:13.618296 ya_django_toolkit_jp-0.0.3/ya_django_toolkit_jp/utils/ipv6.py
+-rw-r--r--   0        0        0      206 2023-05-31 02:03:13.618296 ya_django_toolkit_jp-0.0.3/ya_django_toolkit_jp/utils/mimetypes.py
+-rw-r--r--   0        0        0      508 2023-05-31 02:03:13.618296 ya_django_toolkit_jp-0.0.3/ya_django_toolkit_jp/utils/view.py
+-rw-r--r--   0        0        0     1028 1970-01-01 00:00:00.000000 ya_django_toolkit_jp-0.0.3/PKG-INFO
```

### Comparing `ya_django_toolkit_jp-0.0.2/CHANGELOG.md` & `ya_django_toolkit_jp-0.0.3/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## [v0.0.3](https://github.com/yk-lab/ya-django-toolkit-jp/compare/v0.0.2...v0.0.3) - 2023-05-31
+
+- feat: is_active_view テンプレートタグ テンプレート中で list で view 名を渡しやすくするように変更 by @yk-lab in https://github.com/yk-lab/ya-django-toolkit-jp/pull/11
+
 ## [v0.0.2](https://github.com/yk-lab/ya-django-toolkit-jp/compare/v0.0.1...v0.0.2) - 2023-05-26
 
 - chore: テストコードの追加 by @yk-lab in https://github.com/yk-lab/ya-django-toolkit-jp/pull/7
 - chore: タグなしリリース時のバージョン名を PEP-440 準拠に変更 by @yk-lab in https://github.com/yk-lab/ya-django-toolkit-jp/pull/8
 - feat: 現在表示中の view や url であるかを判定するテンプレートタグを追加 by @yk-lab in https://github.com/yk-lab/ya-django-toolkit-jp/pull/9
 
 ## [v0.0.1](https://github.com/yk-lab/ya-django-toolkit-jp/commits/v0.0.1) - 2023-05-23
```

### Comparing `ya_django_toolkit_jp-0.0.2/pyproject.toml` & `ya_django_toolkit_jp-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ya_django_toolkit_jp-0.0.2/ya_django_toolkit_jp/base_app_settings.py` & `ya_django_toolkit_jp-0.0.3/ya_django_toolkit_jp/base_app_settings.py`

 * *Files identical despite different names*

### Comparing `ya_django_toolkit_jp-0.0.2/ya_django_toolkit_jp/fields/ulid.py` & `ya_django_toolkit_jp-0.0.3/ya_django_toolkit_jp/fields/ulid.py`

 * *Files identical despite different names*

### Comparing `ya_django_toolkit_jp-0.0.2/ya_django_toolkit_jp/ja/utils.py` & `ya_django_toolkit_jp-0.0.3/ya_django_toolkit_jp/ja/utils.py`

 * *Files identical despite different names*

### Comparing `ya_django_toolkit_jp-0.0.2/ya_django_toolkit_jp/utils/file.py` & `ya_django_toolkit_jp-0.0.3/ya_django_toolkit_jp/utils/file.py`

 * *Files identical despite different names*

### Comparing `ya_django_toolkit_jp-0.0.2/ya_django_toolkit_jp/utils/ip.py` & `ya_django_toolkit_jp-0.0.3/ya_django_toolkit_jp/utils/ip.py`

 * *Files identical despite different names*

### Comparing `ya_django_toolkit_jp-0.0.2/ya_django_toolkit_jp/utils/ipv6.py` & `ya_django_toolkit_jp-0.0.3/ya_django_toolkit_jp/utils/ipv6.py`

 * *Files identical despite different names*

### Comparing `ya_django_toolkit_jp-0.0.2/PKG-INFO` & `ya_django_toolkit_jp-0.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ya-django-toolkit-jp
-Version: 0.0.2
+Version: 0.0.3
 Summary: 日本語（マルチバイト文字）の考慮も入れた Django プロジェクトのためのユーティリティです。
 Home-page: https://github.com/yk-lab
 License: MIT
 Author: yk-lab a.k.a YetAnother_yk
 Author-email: yk-lab@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

