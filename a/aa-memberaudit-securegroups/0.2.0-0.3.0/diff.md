# Comparing `tmp/aa_memberaudit_securegroups-0.2.0.tar.gz` & `tmp/aa_memberaudit_securegroups-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_memberaudit_securegroups-0.2.0.tar", last modified: Mon Feb 27 13:47:04 2023, max compression
+gzip compressed data, was "aa_memberaudit_securegroups-0.3.0.tar", last modified: Wed May 31 21:01:09 2023, max compression
```

## Comparing `aa_memberaudit_securegroups-0.2.0.tar` & `aa_memberaudit_securegroups-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,55 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 13:47:04.226696 aa_memberaudit_securegroups-0.2.0/
--rw-rw-rw-   0 root         (0) root         (0)      972 2023-02-27 13:46:44.000000 aa_memberaudit_securegroups-0.2.0/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)    35149 2023-02-27 13:46:44.000000 aa_memberaudit_securegroups-0.2.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-02-27 13:46:44.000000 aa_memberaudit_securegroups-0.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3788 2023-02-27 13:47:04.226696 aa_memberaudit_securegroups-0.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2422 2023-02-27 13:46:44.000000 aa_memberaudit_securegroups-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 13:47:04.224862 aa_memberaudit_securegroups-0.2.0/aa_memberaudit_securegroups.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3788 2023-02-27 13:47:04.000000 aa_memberaudit_securegroups-0.2.0/aa_memberaudit_securegroups.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      649 2023-02-27 13:47:04.000000 aa_memberaudit_securegroups-0.2.0/aa_memberaudit_securegroups.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-27 13:47:04.000000 aa_memberaudit_securegroups-0.2.0/aa_memberaudit_securegroups.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-27 13:47:04.000000 aa_memberaudit_securegroups-0.2.0/aa_memberaudit_securegroups.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       77 2023-02-27 13:47:04.000000 aa_memberaudit_securegroups-0.2.0/aa_memberaudit_securegroups.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-02-27 13:47:04.000000 aa_memberaudit_securegroups-0.2.0/aa_memberaudit_securegroups.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 13:47:04.225779 aa_memberaudit_securegroups-0.2.0/memberaudit_securegroups/
--rw-rw-rw-   0 root         (0) root         (0)       43 2023-02-27 13:46:44.000000 aa_memberaudit_securegroups-0.2.0/memberaudit_securegroups/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2025 2023-02-27 13:46:44.000000 aa_memberaudit_securegroups-0.2.0/memberaudit_securegroups/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      313 2023-02-27 13:46:44.000000 aa_memberaudit_securegroups-0.2.0/memberaudit_securegroups/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      488 2023-02-27 13:46:44.000000 aa_memberaudit_securegroups-0.2.0/memberaudit_securegroups/auth_hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-27 13:47:04.226696 aa_memberaudit_securegroups-0.2.0/memberaudit_securegroups/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     6062 2023-02-27 13:46:44.000000 aa_memberaudit_securegroups-0.2.0/memberaudit_securegroups/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-27 13:46:44.000000 aa_memberaudit_securegroups-0.2.0/memberaudit_securegroups/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12844 2023-02-27 13:46:44.000000 aa_memberaudit_securegroups-0.2.0/memberaudit_securegroups/models.py
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-02-27 13:46:44.000000 aa_memberaudit_securegroups-0.2.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1631 2023-02-27 13:47:04.227613 aa_memberaudit_securegroups-0.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 21:01:09.971734 aa_memberaudit_securegroups-0.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1182 2023-05-31 21:00:53.000000 aa_memberaudit_securegroups-0.3.0/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2023-05-31 21:00:53.000000 aa_memberaudit_securegroups-0.3.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-05-31 21:00:53.000000 aa_memberaudit_securegroups-0.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3788 2023-05-31 21:01:09.971734 aa_memberaudit_securegroups-0.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2422 2023-05-31 21:00:53.000000 aa_memberaudit_securegroups-0.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 21:01:09.967734 aa_memberaudit_securegroups-0.3.0/aa_memberaudit_securegroups.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3788 2023-05-31 21:01:09.000000 aa_memberaudit_securegroups-0.3.0/aa_memberaudit_securegroups.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1333 2023-05-31 21:01:09.000000 aa_memberaudit_securegroups-0.3.0/aa_memberaudit_securegroups.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 21:01:09.000000 aa_memberaudit_securegroups-0.3.0/aa_memberaudit_securegroups.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 21:01:09.000000 aa_memberaudit_securegroups-0.3.0/aa_memberaudit_securegroups.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       75 2023-05-31 21:01:09.000000 aa_memberaudit_securegroups-0.3.0/aa_memberaudit_securegroups.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-05-31 21:01:09.000000 aa_memberaudit_securegroups-0.3.0/aa_memberaudit_securegroups.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 21:01:09.968734 aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/
+-rw-rw-rw-   0 root         (0) root         (0)       43 2023-05-31 21:00:53.000000 aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2308 2023-05-31 21:00:53.000000 aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      464 2023-05-31 21:00:53.000000 aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      488 2023-05-31 21:00:53.000000 aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/auth_hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 21:01:09.968734 aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 21:01:09.961734 aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 21:01:09.969734 aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     2937 2023-05-31 21:00:53.000000 aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/locale/de/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     3902 2023-05-31 21:00:53.000000 aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/locale/de/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)     2705 2023-05-31 21:00:53.000000 aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/locale/django.pot
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 21:01:09.962734 aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/locale/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 21:01:09.969734 aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     2697 2023-05-31 21:00:53.000000 aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 21:01:09.962734 aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/locale/fr_FR/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 21:01:09.969734 aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/locale/fr_FR/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     2650 2023-05-31 21:00:53.000000 aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/locale/fr_FR/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 21:01:09.962734 aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/locale/it_IT/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 21:01:09.969734 aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/locale/it_IT/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     2650 2023-05-31 21:00:53.000000 aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/locale/it_IT/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 21:01:09.963734 aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/locale/ja/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 21:01:09.969734 aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/locale/ja/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     2638 2023-05-31 21:00:53.000000 aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 21:01:09.963734 aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/locale/ko_KR/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 21:01:09.970734 aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/locale/ko_KR/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     2650 2023-05-31 21:00:53.000000 aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/locale/ko_KR/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 21:01:09.963734 aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/locale/ru/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 21:01:09.970734 aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/locale/ru/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     3791 2023-05-31 21:00:53.000000 aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)     4846 2023-05-31 21:00:53.000000 aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 21:01:09.964734 aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/locale/uk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 21:01:09.970734 aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/locale/uk/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     2890 2023-05-31 21:00:53.000000 aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/locale/uk/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 21:01:09.964734 aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/locale/zh_Hans/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 21:01:09.970734 aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/locale/zh_Hans/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     2638 2023-05-31 21:00:53.000000 aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 21:01:09.971734 aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     6044 2023-05-31 21:00:53.000000 aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-31 21:00:53.000000 aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13491 2023-05-31 21:00:53.000000 aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-05-31 21:00:53.000000 aa_memberaudit_securegroups-0.3.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1629 2023-05-31 21:01:09.971734 aa_memberaudit_securegroups-0.3.0/setup.cfg
```

### Comparing `aa_memberaudit_securegroups-0.2.0/CHANGELOG.md` & `aa_memberaudit_securegroups-0.3.0/CHANGELOG.md`

 * *Files 21% similar despite different names*

```diff
@@ -4,14 +4,28 @@
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/)
 and this project adheres to [Semantic Versioning](http://semver.org/).
 
 ## [In Development]
 
 
+## [0.3.0] - 2023-05-31
+
+### Fixed
+
+- Migration dependency for Member Audit >= 2.0.0
+
+### Changed
+
+- Dependencies:
+    - aa-memberaudit>=2.0.0
+    - allianceauth>=3.0.0
+    - allianceauth-securegroups>=0.5.1
+
+
 ## [0.2.0] - 2023-02-27
 
 ### Added
 
 - Secure Group's audit filter to the filters for better visual feedback
```

### Comparing `aa_memberaudit_securegroups-0.2.0/LICENSE` & `aa_memberaudit_securegroups-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_memberaudit_securegroups-0.2.0/PKG-INFO` & `aa_memberaudit_securegroups-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa_memberaudit_securegroups
-Version: 0.2.0
+Version: 0.3.0
 Summary: Member Audit Secure Groups integration for Alliance Auth
 Home-page: https://gitlab.com/eclipse-expeditions/aa-memberaudit-securegroups
 Author: Rebecca Murphy
 Author-email: rebecca@rcmurphy.me
 Maintainer: Peter Pfeufer
 Maintainer-email: develop@ppfeufer.de
 License: GPL-3.0
```

### Comparing `aa_memberaudit_securegroups-0.2.0/README.md` & `aa_memberaudit_securegroups-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `aa_memberaudit_securegroups-0.2.0/aa_memberaudit_securegroups.egg-info/PKG-INFO` & `aa_memberaudit_securegroups-0.3.0/aa_memberaudit_securegroups.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-memberaudit-securegroups
-Version: 0.2.0
+Version: 0.3.0
 Summary: Member Audit Secure Groups integration for Alliance Auth
 Home-page: https://gitlab.com/eclipse-expeditions/aa-memberaudit-securegroups
 Author: Rebecca Murphy
 Author-email: rebecca@rcmurphy.me
 Maintainer: Peter Pfeufer
 Maintainer-email: develop@ppfeufer.de
 License: GPL-3.0
```

### Comparing `aa_memberaudit_securegroups-0.2.0/memberaudit_securegroups/admin.py` & `aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/admin.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 
 # Third Party
 import humanize
 
 # Django
 from django.contrib import admin
+from django.utils.translation import ngettext
 
 # Memberaudit Securegroups
 from memberaudit_securegroups.models import (
     ActivityFilter,
     AgeFilter,
     AssetFilter,
     ComplianceFilter,
@@ -38,15 +39,23 @@
     """
     ActivityFilterAdmin
     """
 
     list_display = ("description", "_inactivity_threshold")
 
     def _inactivity_threshold(self, obj):
-        return f"{obj.inactivity_threshold:d} days"
+        inactivity_threshold = obj.inactivity_threshold
+
+        return_value = ngettext(
+            f"{inactivity_threshold:d} day",
+            f"{inactivity_threshold:d} days",
+            inactivity_threshold,
+        )
+
+        return return_value
 
 
 @admin.register(AgeFilter)
 class AgeFilterAdmin(admin.ModelAdmin):
     """
     AgeFilterAdmin
     """
@@ -81,15 +90,17 @@
     """
     SkillPointFilterAdmin
     """
 
     list_display = ("description", "_skill_point_threshold")
 
     def _skill_point_threshold(self, obj):
-        return f"{humanize.intword(obj.skill_point_threshold)} skill points"
+        skillpoints = humanize.intword(obj.skill_point_threshold)
+
+        return f"{skillpoints} skill points"
 
 
 @admin.register(SkillSetFilter)
 class SkillSetFilterAdmin(admin.ModelAdmin):
     """
     SkillSetFilterAdmin
     """
```

### Comparing `aa_memberaudit_securegroups-0.2.0/memberaudit_securegroups/migrations/0001_initial.py` & `aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/migrations/0001_initial.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 class Migration(migrations.Migration):
     initial = True
 
     dependencies = [
         ("eveuniverse", "0004_effect_longer_name"),
-        ("memberaudit", "0003_stats_n_skillset_autocomplete"),
+        ("memberaudit", "0001_initial_new"),
     ]
 
     operations = [
         migrations.CreateModel(
             name="ActivityFilter",
             fields=[
                 (
```

### Comparing `aa_memberaudit_securegroups-0.2.0/memberaudit_securegroups/models.py` & `aa_memberaudit_securegroups-0.3.0/memberaudit_securegroups/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 # Django
 from django.contrib.auth.models import User
 from django.core.cache import cache
 from django.db import models
 from django.db.models import Q
 from django.utils.translation import gettext_lazy as _
+from django.utils.translation import ngettext
 
 # Alliance Auth
 from allianceauth.authentication.models import CharacterOwnership
 
 # Member Audit
 from memberaudit.app_settings import MEMBERAUDIT_APP_NAME
 from memberaudit.models import Character, CharacterAsset, General, SkillSet
@@ -120,26 +121,26 @@
     def process_filter(self, user: User):
         """
         This is the check run against a users characters
         :param user:
         :return:
         """
 
-        raise NotImplementedError("Please Create a filter!")
+        raise NotImplementedError(_("Please Create a filter!"))
 
     def audit_filter(self, users):
         """
         Bulk check system that also advises the user with simple messages
         :param users:
         :type users:
         :return:
         :rtype:
         """
 
-        raise NotImplementedError("Please Create an audit function!")
+        raise NotImplementedError(_("Please Create an audit function!"))
 
 
 class ActivityFilter(BaseFilter):
     """
     ActivityFilter
     """
 
@@ -150,15 +151,21 @@
     @property
     def name(self):
         """
         Filter name
         :return:
         """
 
-        return f"Activity [days={self.inactivity_threshold}]"
+        inactivity_threshold = ngettext(
+            f"{self.inactivity_threshold:d} day",
+            f"{self.inactivity_threshold:d} days",
+            self.inactivity_threshold,
+        )
+
+        return _(f"Activity [Last {inactivity_threshold}]")
 
     def process_filter(self, user: User):
         """
         Processing filter
         :param user:
         :return:
         """
@@ -203,15 +210,15 @@
 
                 for char in characters:
                     chars[char.user.pk].append(char.eve_character.character_name)
 
                 for char_user, char_list in chars.items():
                     active_characters = ", ".join(char_list)
                     output[char_user] = {
-                        "message": f"Active Characters: {active_characters}",
+                        "message": _(f"Active Characters: {active_characters}"),
                         "check": True,
                     }
 
         return output
 
 
 class AgeFilter(BaseFilter):
@@ -226,15 +233,21 @@
     @property
     def name(self):
         """
         Filter name
         :return:
         """
 
-        return f"Character Age [days={self.age_threshold}]"
+        age_threshold = ngettext(
+            f"{self.age_threshold:d} day",
+            f"{self.age_threshold:d} days",
+            self.age_threshold,
+        )
+
+        return _(f"Character Age [{age_threshold}]")
 
     def process_filter(self, user: User):
         """
         Processing filter
         :param user:
         :return:
         """
@@ -291,15 +304,15 @@
     @property
     def name(self):
         """
         Filter name
         :return:
         """
 
-        return "Member Audit Asset"
+        return _("Member Audit Asset")
 
     def process_filter(self, user: User):
         """
         Processing filter
         :param user:
         :return:
         """
@@ -360,15 +373,15 @@
     @property
     def name(self):
         """
         Filter name
         :return:
         """
 
-        return "Compliance"
+        return _("Compliance")
 
     def process_filter(self, user: User):
         """
         Processing filter
         :param user:
         :return:
         """
@@ -387,15 +400,17 @@
         """
 
         output = defaultdict(lambda: {"message": "", "check": False})
 
         for user in users:
             if General.compliant_users().filter(pk=user.pk).exists():
                 output[user.pk] = {
-                    "message": f"All characters have been added to {MEMBERAUDIT_APP_NAME}",
+                    "message": _(
+                        f"All characters have been added to {MEMBERAUDIT_APP_NAME}"
+                    ),
                     "check": True,
                 }
 
         return output
 
 
 class SkillPointFilter(BaseFilter):
@@ -410,19 +425,24 @@
     @property
     def name(self):
         """
         Filter name
         :return:
         """
 
-        return (
-            "Member Audit Skill Points "
-            f"[sp={humanize.intword(self.skill_point_threshold)}]"
+        sp_threshold = humanize.intword(self.skill_point_threshold)
+
+        skill_point_threshold = ngettext(
+            f"{sp_threshold} skill point",
+            f"{sp_threshold} skill points",
+            self.skill_point_threshold,
         )
 
+        return _(f"Member Audit Skill Points [{skill_point_threshold}]")
+
     def process_filter(self, user: User):
         """
         Processing filter
         :param user:
         :return:
         """
 
@@ -477,15 +497,15 @@
     @property
     def name(self):
         """
         Filter name
         :return:
         """
 
-        return "Member Audit Skill Set"
+        return _("Member Audit Skill Set")
 
     def process_filter(self, user: User):
         """
         Processing filter
         :param user:
         :return:
         """
```

### Comparing `aa_memberaudit_securegroups-0.2.0/setup.cfg` & `aa_memberaudit_securegroups-0.3.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 project_urls = 
 	Issue / Bug Reports = https://gitlab.com/eclipse-expeditions/aa-memberaudit-securegroups/-/issues
 	Changelog = https://gitlab.com/eclipse-expeditions/aa-memberaudit-securegroups/-/blob/master/CHANGELOG.md
 
 [options]
 packages = find_namespace:
 install_requires = 
-	aa-memberaudit>=1.15.1
-	allianceauth>=2.15.1
-	allianceauth-securegroups>=0.2.1
+	aa-memberaudit>=2.0.0
+	allianceauth>=3.0.0
+	allianceauth-securegroups>=0.5.1
 python_requires = ~=3.8
 include_package_data = True
 zip_safe = False
 
 [options.packages.find]
 include = memberaudit_securegroups*
```

