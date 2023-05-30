# Comparing `tmp/django-cookie-consent-0.3.1.tar.gz` & `tmp/django-cookie-consent-0.4.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-cookie-consent-0.3.1.tar", last modified: Thu Feb 17 16:48:25 2022, max compression
+gzip compressed data, was "django-cookie-consent-0.4.0.dev0.tar", last modified: Tue May 30 22:09:47 2023, max compression
```

## Comparing `django-cookie-consent-0.3.1.tar` & `django-cookie-consent-0.4.0.dev0.tar`

### file list

```diff
@@ -1,55 +1,51 @@
-drwxr-xr-x   0 bmihelac  (1000) bmihelac  (1000)        0 2022-02-17 16:48:25.762322 django-cookie-consent-0.3.1/
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)      264 2022-02-17 16:48:25.000000 django-cookie-consent-0.3.1/AUTHORS
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)     1349 2022-02-17 16:48:25.000000 django-cookie-consent-0.3.1/LICENSE
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)      181 2022-02-17 16:48:25.000000 django-cookie-consent-0.3.1/MANIFEST.in
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)     2801 2022-02-17 16:48:25.762322 django-cookie-consent-0.3.1/PKG-INFO
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)     1694 2022-02-17 16:48:25.000000 django-cookie-consent-0.3.1/README.md
-drwxr-xr-x   0 bmihelac  (1000) bmihelac  (1000)        0 2022-02-17 16:48:25.762322 django-cookie-consent-0.3.1/cookie_consent/
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)        0 2022-02-17 16:48:25.000000 django-cookie-consent-0.3.1/cookie_consent/__init__.py
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)     1145 2022-02-17 16:48:25.000000 django-cookie-consent-0.3.1/cookie_consent/admin.py
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)      100 2022-02-17 16:48:25.000000 django-cookie-consent-0.3.1/cookie_consent/apps.py
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)      905 2022-02-17 16:48:25.000000 django-cookie-consent-0.3.1/cookie_consent/cache.py
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)      188 2022-02-17 16:48:25.000000 django-cookie-consent-0.3.1/cookie_consent/compat.py
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)      321 2022-02-17 16:48:25.000000 django-cookie-consent-0.3.1/cookie_consent/conf.py
-drwxr-xr-x   0 bmihelac  (1000) bmihelac  (1000)        0 2022-02-17 16:48:25.762322 django-cookie-consent-0.3.1/cookie_consent/fixtures/
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)     2449 2022-02-17 16:48:25.000000 django-cookie-consent-0.3.1/cookie_consent/fixtures/common_cookies.json
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)     1511 2022-02-17 16:48:25.000000 django-cookie-consent-0.3.1/cookie_consent/middleware.py
-drwxr-xr-x   0 bmihelac  (1000) bmihelac  (1000)        0 2022-02-17 16:48:25.762322 django-cookie-consent-0.3.1/cookie_consent/migrations/
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)     2710 2022-02-17 16:48:25.000000 django-cookie-consent-0.3.1/cookie_consent/migrations/0001_initial.py
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)     1113 2022-02-17 16:48:25.000000 django-cookie-consent-0.3.1/cookie_consent/migrations/0002_auto__add_logitem.py
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)        0 2022-02-17 16:48:25.000000 django-cookie-consent-0.3.1/cookie_consent/migrations/__init__.py
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)     3630 2022-02-17 16:48:25.000000 django-cookie-consent-0.3.1/cookie_consent/models.py
-drwxr-xr-x   0 bmihelac  (1000) bmihelac  (1000)        0 2022-02-17 16:48:25.762322 django-cookie-consent-0.3.1/cookie_consent/static/
-drwxr-xr-x   0 bmihelac  (1000) bmihelac  (1000)        0 2022-02-17 16:48:25.762322 django-cookie-consent-0.3.1/cookie_consent/static/cookie_consent/
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)     1828 2022-02-17 16:48:25.000000 django-cookie-consent-0.3.1/cookie_consent/static/cookie_consent/cookiebar.js
-drwxr-xr-x   0 bmihelac  (1000) bmihelac  (1000)        0 2022-02-17 16:48:25.762322 django-cookie-consent-0.3.1/cookie_consent/templates/
-drwxr-xr-x   0 bmihelac  (1000) bmihelac  (1000)        0 2022-02-17 16:48:25.762322 django-cookie-consent-0.3.1/cookie_consent/templates/cookie_consent/
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)     1496 2022-02-17 16:48:25.000000 django-cookie-consent-0.3.1/cookie_consent/templates/cookie_consent/_cookie_group.html
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)       85 2022-02-17 16:48:25.000000 django-cookie-consent-0.3.1/cookie_consent/templates/cookie_consent/base.html
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)      308 2022-02-17 16:48:25.000000 django-cookie-consent-0.3.1/cookie_consent/templates/cookie_consent/cookiegroup_list.html
-drwxr-xr-x   0 bmihelac  (1000) bmihelac  (1000)        0 2022-02-17 16:48:25.762322 django-cookie-consent-0.3.1/cookie_consent/templatetags/
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)       46 2022-02-17 16:48:25.000000 django-cookie-consent-0.3.1/cookie_consent/templatetags/__init__.py
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)     4004 2022-02-17 16:48:25.000000 django-cookie-consent-0.3.1/cookie_consent/templatetags/cookie_consent_tags.py
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)      862 2022-02-17 16:48:25.000000 django-cookie-consent-0.3.1/cookie_consent/urls.py
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)     5382 2022-02-17 16:48:25.000000 django-cookie-consent-0.3.1/cookie_consent/util.py
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)     2269 2022-02-17 16:48:25.000000 django-cookie-consent-0.3.1/cookie_consent/views.py
-drwxr-xr-x   0 bmihelac  (1000) bmihelac  (1000)        0 2022-02-17 16:48:25.762322 django-cookie-consent-0.3.1/django_cookie_consent.egg-info/
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)     2801 2022-02-17 16:48:25.000000 django-cookie-consent-0.3.1/django_cookie_consent.egg-info/PKG-INFO
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)     1264 2022-02-17 16:48:25.000000 django-cookie-consent-0.3.1/django_cookie_consent.egg-info/SOURCES.txt
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)        1 2022-02-17 16:48:25.000000 django-cookie-consent-0.3.1/django_cookie_consent.egg-info/dependency_links.txt
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)       27 2022-02-17 16:48:25.000000 django-cookie-consent-0.3.1/django_cookie_consent.egg-info/requires.txt
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)       21 2022-02-17 16:48:25.000000 django-cookie-consent-0.3.1/django_cookie_consent.egg-info/top_level.txt
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)       38 2022-02-17 16:48:25.762322 django-cookie-consent-0.3.1/setup.cfg
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)     1395 2022-02-17 16:48:25.000000 django-cookie-consent-0.3.1/setup.py
-drwxr-xr-x   0 bmihelac  (1000) bmihelac  (1000)        0 2022-02-17 16:48:25.762322 django-cookie-consent-0.3.1/tests/
-drwxr-xr-x   0 bmihelac  (1000) bmihelac  (1000)        0 2022-02-17 16:48:25.762322 django-cookie-consent-0.3.1/tests/core/
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)        0 2022-02-17 16:48:25.000000 django-cookie-consent-0.3.1/tests/core/__init__.py
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)        0 2022-02-17 16:48:25.000000 django-cookie-consent-0.3.1/tests/core/models.py
-drwxr-xr-x   0 bmihelac  (1000) bmihelac  (1000)        0 2022-02-17 16:48:25.762322 django-cookie-consent-0.3.1/tests/core/tests/
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)        0 2022-02-17 16:48:25.000000 django-cookie-consent-0.3.1/tests/core/tests/__init__.py
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)     1436 2022-02-17 16:48:25.000000 django-cookie-consent-0.3.1/tests/core/tests/test_cache.py
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)     1492 2022-02-17 16:48:25.000000 django-cookie-consent-0.3.1/tests/core/tests/test_models.py
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)     4890 2022-02-17 16:48:25.000000 django-cookie-consent-0.3.1/tests/core/tests/test_util.py
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)     6093 2022-02-17 16:48:25.000000 django-cookie-consent-0.3.1/tests/core/tests/test_views.py
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)      170 2022-02-17 16:48:25.000000 django-cookie-consent-0.3.1/tests/core/urls.py
--rw-r--r--   0 bmihelac  (1000) bmihelac  (1000)      534 2022-02-17 16:48:25.000000 django-cookie-consent-0.3.1/tests/core/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:09:47.072837 django-cookie-consent-0.4.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-05-30 22:09:47.072837 django-cookie-consent-0.4.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:09:47.072837 django-cookie-consent-0.4.0.dev0/cookie_consent/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:09:47.072837 django-cookie-consent-0.4.0.dev0/cookie_consent/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/fixtures/common_cookies.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:09:47.072837 django-cookie-consent-0.4.0.dev0/cookie_consent/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/migrations/0002_auto__add_logitem.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:09:47.068837 django-cookie-consent-0.4.0.dev0/cookie_consent/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:09:47.072837 django-cookie-consent-0.4.0.dev0/cookie_consent/static/cookie_consent/
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/static/cookie_consent/cookiebar.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:09:47.068837 django-cookie-consent-0.4.0.dev0/cookie_consent/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:09:47.072837 django-cookie-consent-0.4.0.dev0/cookie_consent/templates/cookie_consent/
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/templates/cookie_consent/_cookie_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/templates/cookie_consent/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/templates/cookie_consent/cookiegroup_list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:09:47.072837 django-cookie-consent-0.4.0.dev0/cookie_consent/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/templatetags/cookie_consent_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/cookie_consent/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:09:47.072837 django-cookie-consent-0.4.0.dev0/django_cookie_consent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-05-30 22:09:47.000000 django-cookie-consent-0.4.0.dev0/django_cookie_consent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-30 22:09:47.000000 django-cookie-consent-0.4.0.dev0/django_cookie_consent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 22:09:47.000000 django-cookie-consent-0.4.0.dev0/django_cookie_consent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 22:09:47.000000 django-cookie-consent-0.4.0.dev0/django_cookie_consent.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-30 22:09:47.000000 django-cookie-consent-0.4.0.dev0/django_cookie_consent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-30 22:09:47.000000 django-cookie-consent-0.4.0.dev0/django_cookie_consent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-30 22:09:47.076837 django-cookie-consent-0.4.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 22:09:47.072837 django-cookie-consent-0.4.0.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-05-30 22:09:36.000000 django-cookie-consent-0.4.0.dev0/tests/test_views.py
```

### Comparing `django-cookie-consent-0.3.1/LICENSE` & `django-cookie-consent-0.4.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.3.1/cookie_consent/fixtures/common_cookies.json` & `django-cookie-consent-0.4.0.dev0/cookie_consent/fixtures/common_cookies.json`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.3.1/cookie_consent/models.py` & `django-cookie-consent-0.4.0.dev0/cookie_consent/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,47 +1,50 @@
 # -*- coding: utf-8 -*-
 import re
 
+from django.core.validators import RegexValidator
 from django.db import models
 from django.utils.translation import gettext_lazy as _
-from django.core.validators import RegexValidator
 
 from cookie_consent.cache import delete_cache
 
-
-COOKIE_NAME_RE = re.compile(r'^[-_a-zA-Z0-9]+$')
+COOKIE_NAME_RE = re.compile(r"^[-_a-zA-Z0-9]+$")
 validate_cookie_name = RegexValidator(
     COOKIE_NAME_RE,
-    _(u"Enter a valid 'varname' consisting of letters, numbers"
-      ", underscores or hyphens."),
-    'invalid')
+    _(
+        "Enter a valid 'varname' consisting of letters, numbers"
+        ", underscores or hyphens."
+    ),
+    "invalid",
+)
 
 
 class CookieGroup(models.Model):
     varname = models.CharField(
-        _('Variable name'),
-        max_length=32,
-        validators=[validate_cookie_name])
-    name = models.CharField(_('Name'), max_length=100, blank=True)
-    description = models.TextField(_('Description'), blank=True)
+        _("Variable name"), max_length=32, validators=[validate_cookie_name]
+    )
+    name = models.CharField(_("Name"), max_length=100, blank=True)
+    description = models.TextField(_("Description"), blank=True)
     is_required = models.BooleanField(
-        _('Is required'),
-        help_text=_('Are cookies in this group required.'),
-        default=False)
+        _("Is required"),
+        help_text=_("Are cookies in this group required."),
+        default=False,
+    )
     is_deletable = models.BooleanField(
-        _('Is deletable?'),
-        help_text=_('Can cookies in this group be deleted.'),
-        default=True)
-    ordering = models.IntegerField(_('Ordering'), default=0)
-    created = models.DateTimeField(_('Created'), auto_now_add=True, blank=True)
+        _("Is deletable?"),
+        help_text=_("Can cookies in this group be deleted."),
+        default=True,
+    )
+    ordering = models.IntegerField(_("Ordering"), default=0)
+    created = models.DateTimeField(_("Created"), auto_now_add=True, blank=True)
 
     class Meta:
-        verbose_name = _('Cookie Group')
-        verbose_name_plural = _('Cookie Groups')
-        ordering = ['ordering']
+        verbose_name = _("Cookie Group")
+        verbose_name_plural = _("Cookie Groups")
+        ordering = ["ordering"]
 
     def __str__(self):
         return self.name
 
     def get_version(self):
         try:
             return str(self.cookie_set.all()[0].get_version())
@@ -57,25 +60,26 @@
         delete_cache()
 
 
 class Cookie(models.Model):
     cookiegroup = models.ForeignKey(
         CookieGroup,
         verbose_name=CookieGroup._meta.verbose_name,
-        on_delete=models.CASCADE)
-    name = models.CharField(_('Name'), max_length=250)
-    description = models.TextField(_('Description'), blank=True)
-    path = models.TextField(_('Path'), blank=True, default="/")
-    domain = models.CharField(_('Domain'), max_length=250, blank=True)
-    created = models.DateTimeField(_('Created'), auto_now_add=True, blank=True)
+        on_delete=models.CASCADE,
+    )
+    name = models.CharField(_("Name"), max_length=250)
+    description = models.TextField(_("Description"), blank=True)
+    path = models.TextField(_("Path"), blank=True, default="/")
+    domain = models.CharField(_("Domain"), max_length=250, blank=True)
+    created = models.DateTimeField(_("Created"), auto_now_add=True, blank=True)
 
     class Meta:
-        verbose_name = _('Cookie')
-        verbose_name_plural = _('Cookies')
-        ordering = ['-created']
+        verbose_name = _("Cookie")
+        verbose_name_plural = _("Cookies")
+        ordering = ["-created"]
 
     def __str__(self):
         return "%s %s%s" % (self.name, self.domain, self.path)
 
     @property
     def varname(self):
         return "%s=%s:%s" % (self.cookiegroup.varname, self.name, self.domain)
@@ -91,27 +95,29 @@
         super(Cookie, self).save(*args, **kwargs)
         delete_cache()
 
 
 ACTION_ACCEPTED = 1
 ACTION_DECLINED = -1
 ACTION_CHOICES = (
-    (ACTION_DECLINED, _('Declined')),
-    (ACTION_ACCEPTED, _('Accepted')),
+    (ACTION_DECLINED, _("Declined")),
+    (ACTION_ACCEPTED, _("Accepted")),
 )
 
 
 class LogItem(models.Model):
-    action = models.IntegerField(_('Action'), choices=ACTION_CHOICES)
+    action = models.IntegerField(_("Action"), choices=ACTION_CHOICES)
     cookiegroup = models.ForeignKey(
         CookieGroup,
         verbose_name=CookieGroup._meta.verbose_name,
-        on_delete=models.CASCADE)
-    version = models.CharField(_('Version'), max_length=32)
-    created = models.DateTimeField(_('Created'), auto_now_add=True, blank=True)
+        on_delete=models.CASCADE,
+    )
+    version = models.CharField(_("Version"), max_length=32)
+    created = models.DateTimeField(_("Created"), auto_now_add=True, blank=True)
+
     def __str__(self):
         return "%s %s" % (self.cookiegroup.name, self.version)
 
     class Meta:
-        verbose_name = _('Log item')
-        verbose_name_plural = _('Log items')
-        ordering = ['-created']
+        verbose_name = _("Log item")
+        verbose_name_plural = _("Log items")
+        ordering = ["-created"]
```

### Comparing `django-cookie-consent-0.3.1/cookie_consent/static/cookie_consent/cookiebar.js` & `django-cookie-consent-0.4.0.dev0/cookie_consent/static/cookie_consent/cookiebar.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -48,16 +48,16 @@
                 })
         });
 
     document
         .querySelector(".cc-cookie-decline", content)
         .addEventListener('click', (e) => {
             e.preventDefault();
-            if (typeof opts.declined === "function") {
-                opts.declined();
+            if (typeof opts.beforeDeclined === "function") {
+                opts.beforeDeclined();
             }
             fetch(e.target.getAttribute("href"), {
                     method: "POST"
                 })
                 .then(() => {
                     content.style.display = "none";
                     body.classList.remove('with-cookie-bar');
```

### Comparing `django-cookie-consent-0.3.1/cookie_consent/templates/cookie_consent/_cookie_group.html` & `django-cookie-consent-0.4.0.dev0/cookie_consent/templates/cookie_consent/_cookie_group.html`

 * *Files identical despite different names*

### Comparing `django-cookie-consent-0.3.1/cookie_consent/templatetags/cookie_consent_tags.py` & `django-cookie-consent-0.4.0.dev0/cookie_consent/templatetags/cookie_consent_tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 from django import template
+
 try:
     from django.urls import reverse
 except ImportError:
     from django.core.urlresolvers import reverse
 
+from cookie_consent.conf import settings
 from cookie_consent.util import (
+    are_all_cookies_accepted,
     get_accepted_cookies,
+    get_cookie_dict_from_request,
     get_cookie_string,
     get_cookie_value_from_request,
-    get_cookie_dict_from_request,
-    are_all_cookies_accepted,
     get_not_accepted_or_declined_cookie_groups,
     is_cookie_consent_enabled,
 )
-from cookie_consent.conf import settings
-
 
 register = template.Library()
 
 
 @register.filter
 def cookie_group_accepted(request, arg):
     """
@@ -137,11 +137,13 @@
 
 
 @register.filter
 def accepted_cookies(request):
     """
     Filter returns accepted cookies varnames.
 
-    ::
+    .. code-block:: django
+
         {{ request|accepted_cookies }}
+
     """
     return [c.varname for c in get_accepted_cookies(request)]
```

### Comparing `django-cookie-consent-0.3.1/cookie_consent/urls.py` & `django-cookie-consent-0.4.0.dev0/cookie_consent/urls.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 # -*- coding: utf-8 -*-
 from django.urls import re_path
 from django.views.decorators.csrf import csrf_exempt
 
-from .views import (
-    CookieGroupListView,
-    CookieGroupAcceptView,
-    CookieGroupDeclineView,
-)
+from .views import CookieGroupAcceptView, CookieGroupDeclineView, CookieGroupListView
 
 urlpatterns = [
-    re_path(r'^accept/$',
+    re_path(
+        r"^accept/$",
         csrf_exempt(CookieGroupAcceptView.as_view()),
-        name='cookie_consent_accept_all'),
-    re_path(r'^accept/(?P<varname>.*)/$',
+        name="cookie_consent_accept_all",
+    ),
+    re_path(
+        r"^accept/(?P<varname>.*)/$",
         csrf_exempt(CookieGroupAcceptView.as_view()),
-        name='cookie_consent_accept'),
-    re_path(r'^decline/(?P<varname>.*)/$',
+        name="cookie_consent_accept",
+    ),
+    re_path(
+        r"^decline/(?P<varname>.*)/$",
         csrf_exempt(CookieGroupDeclineView.as_view()),
-        name='cookie_consent_decline'),
-    re_path(r'^decline/$',
+        name="cookie_consent_decline",
+    ),
+    re_path(
+        r"^decline/$",
         csrf_exempt(CookieGroupDeclineView.as_view()),
-        name='cookie_consent_decline_all'),
-    re_path(r'^$',
-        CookieGroupListView.as_view(),
-        name='cookie_consent_cookie_group_list'),
+        name="cookie_consent_decline_all",
+    ),
+    re_path(
+        r"^$", CookieGroupListView.as_view(), name="cookie_consent_cookie_group_list"
+    ),
 ]
```

### Comparing `django-cookie-consent-0.3.1/cookie_consent/util.py` & `django-cookie-consent-0.4.0.dev0/cookie_consent/util.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,15 @@
 # -*- coding: utf-8 -*-
 import datetime
 
 from django.utils.encoding import smart_str
 
-from cookie_consent.cache import (
-    get_cookie_group,
-    all_cookie_groups,
-    get_cookie,
-)
-from cookie_consent.models import (
-    ACTION_ACCEPTED,
-    ACTION_DECLINED,
-    LogItem,
-)
+from cookie_consent.cache import all_cookie_groups, get_cookie, get_cookie_group
 from cookie_consent.conf import settings
+from cookie_consent.models import ACTION_ACCEPTED, ACTION_DECLINED, LogItem
 
 
 def parse_cookie_str(cookie):
     dic = {}
     if not cookie:
         return dic
     for c in cookie.split("|"):
@@ -32,17 +24,23 @@
 
 def get_cookie_dict_from_request(request):
     cookie_str = request.COOKIES.get(settings.COOKIE_CONSENT_NAME)
     return parse_cookie_str(cookie_str)
 
 
 def set_cookie_dict_to_response(response, dic):
-    response.set_cookie(settings.COOKIE_CONSENT_NAME,
-                        dict_to_cookie_str(dic),
-                        settings.COOKIE_CONSENT_MAX_AGE)
+    response.set_cookie(
+        settings.COOKIE_CONSENT_NAME,
+        dict_to_cookie_str(dic),
+        max_age=settings.COOKIE_CONSENT_MAX_AGE,
+        domain=settings.COOKIE_CONSENT_DOMAIN,
+        secure=settings.COOKIE_CONSENT_SECURE or None,
+        httponly=settings.COOKIE_CONSENT_HTTPONLY or None,
+        samesite=settings.COOKIE_CONSENT_SAMESITE,
+    )
 
 
 def get_cookie_value_from_request(request, varname, cookie=None):
     """
     Returns if cookie group or its specific cookie has been accepted.
 
     Returns True or False when cookie is accepted or declined or None
@@ -87,57 +85,66 @@
     """
     Accept cookies in Cookie Group specified by ``varname``.
     """
     cookie_dic = get_cookie_dict_from_request(request)
     for cookie_group in get_cookie_groups(varname):
         cookie_dic[cookie_group.varname] = cookie_group.get_version()
         if settings.COOKIE_CONSENT_LOG_ENABLED:
-            LogItem.objects.create(action=ACTION_ACCEPTED,
-                                cookiegroup=cookie_group,
-                                version=cookie_group.get_version())
+            LogItem.objects.create(
+                action=ACTION_ACCEPTED,
+                cookiegroup=cookie_group,
+                version=cookie_group.get_version(),
+            )
     set_cookie_dict_to_response(response, cookie_dic)
 
 
 def delete_cookies(response, cookie_group):
     if cookie_group.is_deletable:
         for cookie in cookie_group.cookie_set.all():
-            response.delete_cookie(smart_str(cookie.name),
-                                   cookie.path, cookie.domain)
+            response.delete_cookie(smart_str(cookie.name), cookie.path, cookie.domain)
 
 
 def decline_cookies(request, response, varname=None):
     """
     Decline and delete cookies in CookieGroup specified by ``varname``.
     """
     cookie_dic = get_cookie_dict_from_request(request)
     for cookie_group in get_cookie_groups(varname):
         cookie_dic[cookie_group.varname] = settings.COOKIE_CONSENT_DECLINE
         delete_cookies(response, cookie_group)
         if settings.COOKIE_CONSENT_LOG_ENABLED:
-            LogItem.objects.create(action=ACTION_DECLINED,
-                                cookiegroup=cookie_group,
-                                version=cookie_group.get_version())
+            LogItem.objects.create(
+                action=ACTION_DECLINED,
+                cookiegroup=cookie_group,
+                version=cookie_group.get_version(),
+            )
     set_cookie_dict_to_response(response, cookie_dic)
 
 
 def are_all_cookies_accepted(request):
     """
     Returns if all cookies are accepted.
     """
-    return all([get_cookie_value_from_request(request, cookie_group.varname)
-                for cookie_group in get_cookie_groups()])
+    return all(
+        [
+            get_cookie_value_from_request(request, cookie_group.varname)
+            for cookie_group in get_cookie_groups()
+        ]
+    )
 
 
 def get_not_accepted_or_declined_cookie_groups(request):
     """
     Returns all cookie groups that are neither accepted or declined.
     """
-    return [cookie_group for cookie_group in get_cookie_groups()
-            if get_cookie_value_from_request(
-                request, cookie_group.varname) is None]
+    return [
+        cookie_group
+        for cookie_group in get_cookie_groups()
+        if get_cookie_value_from_request(request, cookie_group.varname) is None
+    ]
 
 
 def is_cookie_consent_enabled(request):
     """
     Returns if django-cookie-consent is enabled for given request.
     """
     enabled = settings.COOKIE_CONSENT_ENABLED
@@ -148,19 +155,20 @@
 
 
 def get_cookie_string(cookie_dic):
     """
     Returns cookie in format suitable for use in javascript.
     """
     expires = datetime.datetime.now() + datetime.timedelta(
-        seconds=settings.COOKIE_CONSENT_MAX_AGE)
+        seconds=settings.COOKIE_CONSENT_MAX_AGE
+    )
     cookie_str = "%s=%s; expires=%s; path=/" % (
         settings.COOKIE_CONSENT_NAME,
         dict_to_cookie_str(cookie_dic),
-        expires.strftime("%a, %d %b %Y %H:%M:%S GMT")
+        expires.strftime("%a, %d %b %Y %H:%M:%S GMT"),
     )
     return cookie_str
 
 
 def get_accepted_cookies(request):
     """
     Returns all accepted cookies.
```

### Comparing `django-cookie-consent-0.3.1/cookie_consent/views.py` & `django-cookie-consent-0.4.0.dev0/cookie_consent/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,57 +1,48 @@
 # -*- coding: utf-8 -*-
 from django.core.exceptions import SuspiciousOperation
-from django.contrib.auth.views import SuccessURLAllowedHostsMixin
-from django.http import HttpResponseRedirect, HttpResponse
+from django.http import HttpResponse, HttpResponseRedirect
 from django.urls import reverse
-from django.views.generic import (
-    ListView,
-    View,
-)
-
-from .compat import url_has_allowed_host_and_scheme
-from .models import (
-    CookieGroup,
-)
-from .util import (
-    accept_cookies,
-    decline_cookies,
-)
+from django.views.generic import ListView, View
+
+from .compat import RedirectURLMixin, url_has_allowed_host_and_scheme
+from .models import CookieGroup
+from .util import accept_cookies, decline_cookies
 
 
 class CookieGroupListView(ListView):
     """
     Display all cookies.
     """
-    model = CookieGroup
 
+    model = CookieGroup
 
-class CookieGroupBaseProcessView(SuccessURLAllowedHostsMixin, View):
 
+class CookieGroupBaseProcessView(RedirectURLMixin, View):
     def get_success_url(self):
         """
-        If user adds a 'next' as URL parameter or hidden input, 
-        redirect to the value of 'next'. Otherwise, redirect to 
+        If user adds a 'next' as URL parameter or hidden input,
+        redirect to the value of 'next'. Otherwise, redirect to
         cookie consent group list
         """
-        redirect_to = self.request.POST.get('next', self.request.GET.get('next'))
+        redirect_to = self.request.POST.get("next", self.request.GET.get("next"))
         if redirect_to and not url_has_allowed_host_and_scheme(
             url=redirect_to,
             allowed_hosts=self.get_success_url_allowed_hosts(),
             require_https=self.request.is_secure(),
         ):
-            raise SuspiciousOperation('Unsafe open redirect suspected.')
-        return redirect_to or reverse('cookie_consent_cookie_group_list')
+            raise SuspiciousOperation("Unsafe open redirect suspected.")
+        return redirect_to or reverse("cookie_consent_cookie_group_list")
 
     def process(self, request, response, varname):
         raise NotImplementedError()
 
     def post(self, request, *args, **kwargs):
-        varname = kwargs.get('varname', None)
-        if request.META.get('HTTP_X_REQUESTED_WITH') == 'XMLHttpRequest':
+        varname = kwargs.get("varname", None)
+        if request.META.get("HTTP_X_REQUESTED_WITH") == "XMLHttpRequest":
             response = HttpResponse()
         else:
             response = HttpResponseRedirect(self.get_success_url())
         self.process(request, response, varname)
         return response
```

### Comparing `django-cookie-consent-0.3.1/django_cookie_consent.egg-info/SOURCES.txt` & `django-cookie-consent-0.4.0.dev0/django_cookie_consent.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 AUTHORS
 LICENSE
 MANIFEST.in
 README.md
+setup.cfg
 setup.py
 cookie_consent/__init__.py
 cookie_consent/admin.py
 cookie_consent/apps.py
 cookie_consent/cache.py
 cookie_consent/compat.py
 cookie_consent/conf.py
@@ -23,18 +24,16 @@
 cookie_consent/templates/cookie_consent/base.html
 cookie_consent/templates/cookie_consent/cookiegroup_list.html
 cookie_consent/templatetags/__init__.py
 cookie_consent/templatetags/cookie_consent_tags.py
 django_cookie_consent.egg-info/PKG-INFO
 django_cookie_consent.egg-info/SOURCES.txt
 django_cookie_consent.egg-info/dependency_links.txt
+django_cookie_consent.egg-info/not-zip-safe
 django_cookie_consent.egg-info/requires.txt
 django_cookie_consent.egg-info/top_level.txt
-tests/core/__init__.py
-tests/core/models.py
-tests/core/urls.py
-tests/core/views.py
-tests/core/tests/__init__.py
-tests/core/tests/test_cache.py
-tests/core/tests/test_models.py
-tests/core/tests/test_util.py
-tests/core/tests/test_views.py
+tests/test_cache.py
+tests/test_middleware.py
+tests/test_models.py
+tests/test_settings.py
+tests/test_util.py
+tests/test_views.py
```

### Comparing `django-cookie-consent-0.3.1/tests/core/tests/test_models.py` & `django-cookie-consent-0.4.0.dev0/tests/test_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,32 @@
 # -*- coding: utf-8 -*-
 from django.core.exceptions import ValidationError
-from django.test import (
-    TestCase,
-)
-
-from cookie_consent.models import (
-    Cookie,
-    CookieGroup,
-    validate_cookie_name,
-)
+from django.test import TestCase
 
+from cookie_consent.models import Cookie, CookieGroup, validate_cookie_name
 
-class CookieGroupTest(TestCase):
 
+class CookieGroupTest(TestCase):
     def setUp(self):
         self.cookie_group = CookieGroup.objects.create(
             varname="optional",
             name="Optional",
         )
         self.cookie = Cookie.objects.create(
             cookiegroup=self.cookie_group,
             name="foo",
         )
 
     def test_get_version(self):
         self.assertEqual(
-            self.cookie_group.get_version(),
-            self.cookie.created.isoformat()
+            self.cookie_group.get_version(), self.cookie.created.isoformat()
         )
 
 
 class CookieTest(TestCase):
-
     def setUp(self):
         self.cookie_group = CookieGroup.objects.create(
             varname="optional",
             name="Optional",
         )
         self.cookie = Cookie.objects.create(
             cookiegroup=self.cookie_group,
@@ -44,15 +35,14 @@
         )
 
     def test_varname(self):
         self.assertEqual(self.cookie.varname, "optional=foo:.example.com")
 
 
 class ValidateCookieNameTest(TestCase):
-
     def test_valid(self):
         validate_cookie_name("_foo-bar")
 
     def test_invalid(self):
         invalid_names = (
             "space inside",
             "a!b",
```

### Comparing `django-cookie-consent-0.3.1/tests/core/tests/test_util.py` & `django-cookie-consent-0.4.0.dev0/tests/test_util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,122 +1,112 @@
 # -*- coding: utf-8 -*-
 from datetime import datetime
 
-from django.test import (
-    TestCase,
-)
+from django.test import TestCase
 from django.test.client import RequestFactory
 from django.test.utils import override_settings
 
-from cookie_consent.models import (
-    Cookie,
-    CookieGroup,
-)
+from cookie_consent.conf import settings
+from cookie_consent.models import Cookie, CookieGroup
 from cookie_consent.util import (
+    dict_to_cookie_str,
     get_accepted_cookies,
-    get_cookie_value_from_request,
     get_cookie_groups,
-    parse_cookie_str,
-    dict_to_cookie_str,
+    get_cookie_value_from_request,
     is_cookie_consent_enabled,
+    parse_cookie_str,
 )
-from cookie_consent.conf import settings
 
 
 class UtilTest(TestCase):
-
     def setUp(self):
         self.cookie_group = CookieGroup.objects.create(
             varname="optional",
             name="Optional",
         )
         self.cookie = Cookie.objects.create(
             cookiegroup=self.cookie_group,
             name="foo",
         )
         self.factory = RequestFactory()
-        self.request = self.factory.get('')
+        self.request = self.factory.get("")
 
     def test_parse_cookie_str(self):
         cookie_str = "foo=2013-06-04T01:08:58.262162|bar=2013-06-04T01:08:58"
         res = parse_cookie_str(cookie_str)
         dic = {
-            'foo': "2013-06-04T01:08:58.262162",
-            'bar': "2013-06-04T01:08:58",
+            "foo": "2013-06-04T01:08:58.262162",
+            "bar": "2013-06-04T01:08:58",
         }
         self.assertEqual(res, dic)
 
     def test_dict_to_cookie_str(self):
         cookie_str = "|"
         dic = {
-            'foo': "2013-06-04T01:08:58.262162",
-            'bar': "2013-06-04T01:08:58",
+            "foo": "2013-06-04T01:08:58.262162",
+            "bar": "2013-06-04T01:08:58",
         }
         cookie_str = dict_to_cookie_str(dic)
         self.assertEqual(parse_cookie_str(cookie_str), dic)
 
     def test_get_cookie_value_from_request(self):
-        cookie_str = dict_to_cookie_str({
-            "optional": self.cookie_group.get_version()
-        })
+        cookie_str = dict_to_cookie_str({"optional": self.cookie_group.get_version()})
         self.request.COOKIES[settings.COOKIE_CONSENT_NAME] = cookie_str
-        res = get_cookie_value_from_request(self.request, 'optional')
+        res = get_cookie_value_from_request(self.request, "optional")
         self.assertTrue(res)
 
     def test_get_cookie_value_from_request_declined(self):
-        cookie_str = dict_to_cookie_str({
-            "optional": datetime(1999, 1, 1).isoformat()
-        })
+        cookie_str = dict_to_cookie_str({"optional": datetime(1999, 1, 1).isoformat()})
         self.request.COOKIES[settings.COOKIE_CONSENT_NAME] = cookie_str
-        res = get_cookie_value_from_request(self.request, 'optional')
+        res = get_cookie_value_from_request(self.request, "optional")
         self.assertFalse(res)
 
     def test_get_cookie_value_from_request_empty(self):
-        res = get_cookie_value_from_request(self.request, 'optional')
+        res = get_cookie_value_from_request(self.request, "optional")
         self.assertIsNone(res)
 
     def test_get_cookie_value_from_request_added_cookies(self):
-        cookie_str = dict_to_cookie_str({
-            "optional": self.cookie_group.get_version(),
-        })
+        cookie_str = dict_to_cookie_str(
+            {
+                "optional": self.cookie_group.get_version(),
+            }
+        )
         Cookie.objects.create(
             cookiegroup=self.cookie_group,
             name="bar",
             domain=".example.com",
         )
         self.request.COOKIES[settings.COOKIE_CONSENT_NAME] = cookie_str
-        res = get_cookie_value_from_request(self.request, 'optional')
+        res = get_cookie_value_from_request(self.request, "optional")
         self.assertIsNone(res)
 
     def test_get_cookie_value_from_request_specific_cookie(self):
-        cookie_str = dict_to_cookie_str({
-            "optional": self.cookie_group.get_version()
-        })
+        cookie_str = dict_to_cookie_str({"optional": self.cookie_group.get_version()})
         self.request.COOKIES[settings.COOKIE_CONSENT_NAME] = cookie_str
-        res = get_cookie_value_from_request(self.request, 'optional', "foo:")
+        res = get_cookie_value_from_request(self.request, "optional", "foo:")
         self.assertTrue(res)
 
         Cookie.objects.create(
             cookiegroup=self.cookie_group,
             name="bar",
             domain=".example.com",
         )
-        res = get_cookie_value_from_request(self.request, 'optional',
-                                            "bar:.example.com")
+        res = get_cookie_value_from_request(
+            self.request, "optional", "bar:.example.com"
+        )
         self.assertFalse(res)
 
-        res = get_cookie_value_from_request(self.request, 'optional', "foo:")
+        res = get_cookie_value_from_request(self.request, "optional", "foo:")
         self.assertTrue(res)
 
-        cookie_str = dict_to_cookie_str({
-            "optional": self.cookie_group.get_version()
-        })
+        cookie_str = dict_to_cookie_str({"optional": self.cookie_group.get_version()})
         self.request.COOKIES[settings.COOKIE_CONSENT_NAME] = cookie_str
-        res = get_cookie_value_from_request(self.request, 'optional',
-                                            "bar:.example.com")
+        res = get_cookie_value_from_request(
+            self.request, "optional", "bar:.example.com"
+        )
         self.assertTrue(res)
 
     def test_is_cookie_consent_enabled(self):
         self.assertTrue(is_cookie_consent_enabled(None))
 
     @override_settings(COOKIE_CONSENT_ENABLED=lambda r: False)
     def test_is_cookie_consent_enabled_callable(self):
@@ -129,13 +119,11 @@
             varname="foo",
             name="foo",
         )
         self.assertIn(self.cookie_group, get_cookie_groups("foo,optional"))
         self.assertIn(cookie_group2, get_cookie_groups("foo,optional"))
 
     def test_get_accepted_cookies(self):
-        cookie_str = dict_to_cookie_str({
-            "optional": self.cookie_group.get_version()
-        })
+        cookie_str = dict_to_cookie_str({"optional": self.cookie_group.get_version()})
         self.request.COOKIES[settings.COOKIE_CONSENT_NAME] = cookie_str
         cookies = get_accepted_cookies(self.request)
         self.assertIn(self.cookie, cookies)
```

### Comparing `django-cookie-consent-0.3.1/tests/core/tests/test_views.py` & `django-cookie-consent-0.4.0.dev0/tests/test_views.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,158 +1,161 @@
 # -*- coding: utf-8 -*-
-from django.test import (
-    TestCase,
-)
+from django.test import TestCase
 from django.test.utils import override_settings
 from django.urls import reverse
 
 from cookie_consent.models import (
+    ACTION_ACCEPTED,
+    ACTION_DECLINED,
     Cookie,
     CookieGroup,
     LogItem,
-    ACTION_ACCEPTED,
-    ACTION_DECLINED,
 )
 
 
 class CookieGroupBaseProcessViewTests(TestCase):
-
     def test_get_success_url(self):
         """
         If user adds a 'next' as URL parameter it should,
         redirect to the value of 'next'
         """
-        expected_url = reverse('test_page')
-        url = "{}?next={}".format(
-            reverse('cookie_consent_accept_all'), expected_url
-        )
+        expected_url = reverse("test_page")
+        url = "{}?next={}".format(reverse("cookie_consent_accept_all"), expected_url)
         response = self.client.post(url, follow=True)
         self.assertRedirects(response, expected_url)
 
     def test_no_open_redirects(self):
-        url = "{}?next=https://evil.com".format(
-            reverse('cookie_consent_accept_all')
-        )
+        url = "{}?next=https://evil.com".format(reverse("cookie_consent_accept_all"))
         response = self.client.post(url, follow=True)
         self.assertEqual(response.status_code, 400)  # result of SupiciousOperation
 
 
 class IntegrationTest(TestCase):
-
     def setUp(self):
         self.cookie_group = CookieGroup.objects.create(
             varname="optional",
             name="Optional",
         )
         self.cookie = Cookie.objects.create(
             cookiegroup=self.cookie_group,
             name="foo",
         )
 
     def test_cookies_view(self):
-        response = self.client.get(reverse('cookie_consent_cookie_group_list'))
+        response = self.client.get(reverse("cookie_consent_cookie_group_list"))
         self.assertEqual(response.status_code, 200)
-        self.assertContains(
-            response,
-            '<input type="submit" value="Accept">')
-        self.assertContains(
-            response,
-            '<input type="submit" value="Decline">')
+        self.assertContains(response, '<input type="submit" value="Accept">')
+        self.assertContains(response, '<input type="submit" value="Decline">')
 
     def test_accept_cookie(self):
-        response = self.client.post(reverse('cookie_consent_accept',
-                                            kwargs={"varname": "optional"}),
-                                    follow=True)
+        response = self.client.post(
+            reverse("cookie_consent_accept", kwargs={"varname": "optional"}),
+            follow=True,
+        )
         self.assertEqual(response.status_code, 200)
         self.assertContains(
-            response,
-            '<span class="cookie-consent-accepted">Accepted</span>')
+            response, '<span class="cookie-consent-accepted">Accepted</span>'
+        )
 
     def test_accept_cookie_ajax(self):
-        response = self.client.post(reverse('cookie_consent_accept',
-                                            kwargs={"varname": "optional"}),
-                                    HTTP_X_REQUESTED_WITH='XMLHttpRequest')
+        response = self.client.post(
+            reverse("cookie_consent_accept", kwargs={"varname": "optional"}),
+            HTTP_X_REQUESTED_WITH="XMLHttpRequest",
+        )
         self.assertEqual(response.status_code, 200)
 
     def test_decline_cookie(self):
-        response = self.client.post(reverse('cookie_consent_decline',
-                                            kwargs={"varname": "optional"}),
-                                    follow=True)
+        response = self.client.post(
+            reverse("cookie_consent_decline", kwargs={"varname": "optional"}),
+            follow=True,
+        )
         self.assertEqual(response.status_code, 200)
         self.assertContains(
-            response,
-            '<span class="cookie-consent-declined">Declined</span>')
+            response, '<span class="cookie-consent-declined">Declined</span>'
+        )
 
     def test_decline_cookie_ajax(self):
-        response = self.client.delete(reverse('cookie_consent_decline',
-                                              kwargs={"varname": "optional"}),
-                                      HTTP_X_REQUESTED_WITH='XMLHttpRequest')
+        response = self.client.delete(
+            reverse("cookie_consent_decline", kwargs={"varname": "optional"}),
+            HTTP_X_REQUESTED_WITH="XMLHttpRequest",
+        )
         self.assertEqual(response.status_code, 200)
 
     def test_cookies(self):
         CookieGroup.objects.create(
             varname="social",
             name="Social",
         )
         Cookie.objects.create(
             cookiegroup=self.cookie_group,
             name="optional_test_cookie",
         )
 
-        url = reverse('test_page')
+        url = reverse("test_page")
         response = self.client.get(url)
-        self.assertContains(response,
-                            '"optional" cookies not accepted or declined')
+        self.assertContains(response, '"optional" cookies not accepted or declined')
 
-        response = self.client.post(reverse('cookie_consent_accept',
-                                            kwargs={"varname": "optional"}))
+        response = self.client.post(
+            reverse("cookie_consent_accept", kwargs={"varname": "optional"})
+        )
         response = self.client.get(url)
         self.assertContains(response, '"optional" cookies accepted')
-        self.assertEqual(self.client.cookies.get('optional_test_cookie').value,
-                         "optional cookie set from django")
+        self.assertEqual(
+            self.client.cookies.get("optional_test_cookie").value,
+            "optional cookie set from django",
+        )
 
-        response = self.client.post(reverse('cookie_consent_decline',
-                                            kwargs={"varname": "optional"}))
+        response = self.client.post(
+            reverse("cookie_consent_decline", kwargs={"varname": "optional"})
+        )
         response = self.client.get(url)
         self.assertContains(response, '"optional" cookies declined')
-        #test client returns cookie with value of ''
-        #self.assertIsNone(self.client.cookies.get('optional_test_cookie'))
-        self.assertFalse(self.client.cookies.get('optional_test_cookie').value)
+        # test client returns cookie with value of ''
+        # self.assertIsNone(self.client.cookies.get('optional_test_cookie'))
+        self.assertFalse(self.client.cookies.get("optional_test_cookie").value)
 
     def test_logging(self):
-        self.client.post(reverse('cookie_consent_accept',
-                                 kwargs={"varname": "optional"}))
+        self.client.post(
+            reverse("cookie_consent_accept", kwargs={"varname": "optional"})
+        )
         log_items = LogItem.objects.filter(
             cookiegroup=self.cookie_group,
             version=self.cookie_group.get_version(),
-            action=ACTION_ACCEPTED)
+            action=ACTION_ACCEPTED,
+        )
         self.assertEqual(log_items.count(), 1)
 
-        self.client.delete(reverse('cookie_consent_decline',
-                                   kwargs={"varname": "optional"}))
+        self.client.delete(
+            reverse("cookie_consent_decline", kwargs={"varname": "optional"})
+        )
         log_items = LogItem.objects.filter(
             cookiegroup=self.cookie_group,
             version=self.cookie_group.get_version(),
-            action=ACTION_DECLINED)
+            action=ACTION_DECLINED,
+        )
         self.assertEqual(log_items.count(), 1)
 
     @override_settings(COOKIE_CONSENT_LOG_ENABLED=False)
     def test_logging_disabled(self):
         """
-        When the COOKIE_CONSENT_LOG_ENABLED is False, no log item should be 
+        When the COOKIE_CONSENT_LOG_ENABLED is False, no log item should be
         created
         """
-        self.client.post(reverse('cookie_consent_accept',
-                                 kwargs={"varname": "optional"}))
+        self.client.post(
+            reverse("cookie_consent_accept", kwargs={"varname": "optional"})
+        )
         log_items = LogItem.objects.filter(
             cookiegroup=self.cookie_group,
             version=self.cookie_group.get_version(),
-            action=ACTION_ACCEPTED)
+            action=ACTION_ACCEPTED,
+        )
         self.assertEqual(log_items.count(), 0)
 
-        self.client.delete(reverse('cookie_consent_decline',
-                                   kwargs={"varname": "optional"}))
+        self.client.delete(
+            reverse("cookie_consent_decline", kwargs={"varname": "optional"})
+        )
         log_items = LogItem.objects.filter(
             cookiegroup=self.cookie_group,
             version=self.cookie_group.get_version(),
-            action=ACTION_DECLINED)
+            action=ACTION_DECLINED,
+        )
         self.assertEqual(log_items.count(), 0)
```

