# Comparing `tmp/django-stachoutils-3.3.2.tar.gz` & `tmp/django-stachoutils-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-stachoutils-3.3.2.tar", last modified: Mon Apr  4 12:39:29 2022, max compression
+gzip compressed data, was "django-stachoutils-4.0.0.tar", last modified: Wed May 31 08:28:11 2023, max compression
```

## Comparing `django-stachoutils-3.3.2.tar` & `django-stachoutils-4.0.0.tar`

### file list

```diff
@@ -1,196 +1,196 @@
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.298136 django-stachoutils-3.3.2/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1488 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/LICENSE
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      199 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/MANIFEST.in
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     2134 2022-04-04 12:39:29.297903 django-stachoutils-3.3.2/PKG-INFO
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1256 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/README.rst
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.237364 django-stachoutils-3.3.2/django_stachoutils/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     3903 2020-11-30 15:48:58.000000 django-stachoutils-3.3.2/django_stachoutils/__init__.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      277 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/csv_utf8.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1799 2020-11-30 15:48:58.000000 django-stachoutils-3.3.2/django_stachoutils/decorators.py
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.240048 django-stachoutils-3.3.2/django_stachoutils/forms/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      347 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/forms/__init__.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      666 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/forms/fields.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     6062 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/forms/models.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     4062 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/forms/nested.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     6204 2021-01-26 16:59:59.000000 django-stachoutils-3.3.2/django_stachoutils/forms/widgets.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     3674 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/log.py
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.240351 django-stachoutils-3.3.2/django_stachoutils/management/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)        0 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/management/__init__.py
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.241714 django-stachoutils-3.3.2/django_stachoutils/management/commands/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)        0 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/management/commands/__init__.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    10369 2020-06-10 12:58:56.000000 django-stachoutils-3.3.2/django_stachoutils/management/commands/dumpdata_related.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1132 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/management/commands/hotspot_report.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      747 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/management/commands/sync_permissions.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      585 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/middlewares.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      185 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/models.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     3437 2022-04-04 12:34:34.000000 django-stachoutils-3.3.2/django_stachoutils/options.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1452 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/profiler.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     2254 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/shortcuts.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1836 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/sql.py
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.227281 django-stachoutils-3.3.2/django_stachoutils/static/
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.227799 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.243704 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/css/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      191 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/css/admin_extras.css
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      331 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/css/commons.css
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1797 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/css/forms.css
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.247770 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/img/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      517 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/img/filters.png
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      206 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/img/icon-inactive-no.gif
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      197 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/img/icon-inactive-yes.gif
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      176 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/img/icon-no.gif
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      299 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/img/icon-yes.gif
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      710 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/img/processing.png
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     6826 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/img/sprites.png
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.253549 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/js/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1693 2022-02-25 16:39:28.000000 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/js/admin_extras.js
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     2193 2022-02-24 14:12:10.000000 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/js/change_list.js
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     2022 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/js/editeur.js
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1964 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/js/forms.js
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1589 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/js/jquery.AjaxCSRFprotection.js
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     2878 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/js/jquery.charcounter.js
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1793 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/js/jquery.fieldselection.js
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.254826 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    19113 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/jquery.poshytip.js
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    11435 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/jquery.poshytip.min.js
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.256497 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/tip-darkgray/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1599 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/tip-darkgray/tip-darkgray.css
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     5199 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/tip-darkgray/tip-darkgray.png
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1261 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/tip-darkgray/tip-darkgray_arrows.png
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.257669 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/tip-green/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1312 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/tip-green/tip-green.css
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      118 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/tip-green/tip-green_arrows.gif
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.259307 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/tip-skyblue/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1421 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/tip-skyblue/tip-skyblue.css
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     4729 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/tip-skyblue/tip-skyblue.png
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      896 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/tip-skyblue/tip-skyblue_arrows.png
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.260732 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/tip-twitter/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1539 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/tip-twitter/tip-twitter.css
--rw-r--r--   0 guerrastanislas   (501) staff       (20)       87 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/tip-twitter/tip-twitter_arrows.gif
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.263068 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/tip-violet/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1556 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/tip-violet/tip-violet.css
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     4916 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/tip-violet/tip-violet.png
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1409 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/tip-violet/tip-violet_arrows.png
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.264773 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/tip-yellow/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1557 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/tip-yellow/tip-yellow.css
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     5069 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/tip-yellow/tip-yellow.png
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1402 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/tip-yellow/tip-yellow_arrows.png
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.266070 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/tip-yellowsimple/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1617 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/tip-yellowsimple/tip-yellowsimple.css
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      107 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/tip-yellowsimple/tip-yellowsimple_arrows.gif
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      378 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/storage.py
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.228987 django-stachoutils-3.3.2/django_stachoutils/templates/
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.267036 django-stachoutils-3.3.2/django_stachoutils/templates/django_stachoutils/
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.229198 django-stachoutils-3.3.2/django_stachoutils/templates/django_stachoutils/forms/
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.267543 django-stachoutils-3.3.2/django_stachoutils/templates/django_stachoutils/forms/widgets/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      505 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/templates/django_stachoutils/forms/widgets/texte_editeur.html
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      456 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/templates/django_stachoutils/pagination.html
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      523 2022-02-28 14:16:20.000000 django-stachoutils-3.3.2/django_stachoutils/templates/django_stachoutils/pagination_bootstrap.html
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.268258 django-stachoutils-3.3.2/django_stachoutils/templatetags/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)        0 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/templatetags/__init__.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    12315 2022-02-28 14:16:20.000000 django-stachoutils-3.3.2/django_stachoutils/templatetags/stachoutils_extras.py
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.269415 django-stachoutils-3.3.2/django_stachoutils/views/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)        0 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/views/__init__.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      591 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/django_stachoutils/views/actions.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    15913 2021-12-20 11:31:36.000000 django-stachoutils-3.3.2/django_stachoutils/views/generic.py
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.238725 django-stachoutils-3.3.2/django_stachoutils.egg-info/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     2134 2022-04-04 12:39:29.000000 django-stachoutils-3.3.2/django_stachoutils.egg-info/PKG-INFO
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     6546 2022-04-04 12:39:29.000000 django-stachoutils-3.3.2/django_stachoutils.egg-info/SOURCES.txt
--rw-r--r--   0 guerrastanislas   (501) staff       (20)        1 2022-04-04 12:39:29.000000 django-stachoutils-3.3.2/django_stachoutils.egg-info/dependency_links.txt
--rw-r--r--   0 guerrastanislas   (501) staff       (20)        7 2022-04-04 12:39:29.000000 django-stachoutils-3.3.2/django_stachoutils.egg-info/requires.txt
--rw-r--r--   0 guerrastanislas   (501) staff       (20)       19 2022-04-04 12:39:29.000000 django-stachoutils-3.3.2/django_stachoutils.egg-info/top_level.txt
--rw-r--r--   0 guerrastanislas   (501) staff       (20)       38 2022-04-04 12:39:29.298218 django-stachoutils-3.3.2/setup.cfg
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     2162 2022-04-04 12:35:20.000000 django-stachoutils-3.3.2/setup.py
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.271803 django-stachoutils-3.3.2/tests/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    16384 2022-04-04 10:19:59.000000 django-stachoutils-3.3.2/tests/.runtests.py.swp
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      374 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/Makefile
--rw-r--r--   0 guerrastanislas   (501) staff       (20)       34 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/coveragerc
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.274149 django-stachoutils-3.3.2/tests/forms/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)        0 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/forms/__init__.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1060 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/forms/models.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     5125 2021-12-20 11:10:00.000000 django-stachoutils-3.3.2/tests/forms/test_fields.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     4219 2021-12-20 11:10:00.000000 django-stachoutils-3.3.2/tests/forms/test_fields_with_thumbor.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    19278 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/forms/test_models.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     5168 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/forms/test_nested.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     9695 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/forms/test_widgets.py
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.275201 django-stachoutils-3.3.2/tests/javascript/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1452 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/javascript/demo_texte_editeur.html
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      674 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/javascript/runtests.html
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.275988 django-stachoutils-3.3.2/tests/javascript/tests/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     7440 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/javascript/tests/test_widgets.js
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.276891 django-stachoutils-3.3.2/tests/log/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)        0 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/log/__init__.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1325 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/log/test_smtp_handler.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     2244 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/log/tests.py
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.281427 django-stachoutils-3.3.2/tests/media/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)   206420 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/media/1st_Saab_9-3_SE.jpg
--rw-r--r--   0 guerrastanislas   (501) staff       (20)   384780 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/media/Saab_9-3_Vector_sedan.jpg
--rw-r--r--   0 guerrastanislas   (501) staff       (20)   736699 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/media/home_1.jpg
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    65868 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/media/jardin.jpg
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    30317 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/media/terrasse.jpg
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.282168 django-stachoutils-3.3.2/tests/middlewares/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)        0 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/middlewares/__init__.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1807 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/middlewares/tests.py
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.283168 django-stachoutils-3.3.2/tests/models/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)        0 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/models/__init__.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      545 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/models/models.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      660 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/models/tests.py
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.284401 django-stachoutils-3.3.2/tests/options/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)        0 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/options/__init__.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      380 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/options/models.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     4578 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/options/test_logs.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     2262 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/options/tests.py
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.231202 django-stachoutils-3.3.2/tests/projects/
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.285485 django-stachoutils-3.3.2/tests/projects/django_project/
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.286921 django-stachoutils-3.3.2/tests/projects/django_project/django_project/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)        0 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/projects/django_project/django_project/__init__.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     5635 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/projects/django_project/django_project/settings.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      124 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/projects/django_project/django_project/urls.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1443 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/projects/django_project/django_project/wsgi.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     2683 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/projects/django_project/initial_data.json
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      257 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/projects/django_project/manage.py
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.288964 django-stachoutils-3.3.2/tests/projects/django_project/my_app/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)        0 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/projects/django_project/my_app/__init__.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      849 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/projects/django_project/my_app/admin.py
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.290053 django-stachoutils-3.3.2/tests/projects/django_project/my_app/migrations/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     2362 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/projects/django_project/my_app/migrations/0001_initial.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      450 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/projects/django_project/my_app/migrations/0002_musicgenre_history.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)        0 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/projects/django_project/my_app/migrations/__init__.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     2667 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/projects/django_project/my_app/models.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)        0 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/projects/django_project/my_app/tests.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)        0 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/projects/django_project/my_app/views.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     5225 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/runtests.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     2235 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/settings.py
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.291010 django-stachoutils-3.3.2/tests/shortcuts/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)        0 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/shortcuts/__init__.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      252 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/shortcuts/models.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     4004 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/shortcuts/tests.py
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.292000 django-stachoutils-3.3.2/tests/sql/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)        0 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/sql/__init__.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      384 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/sql/models.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     2527 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/sql/tests.py
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.292989 django-stachoutils-3.3.2/tests/storage/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)        0 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/storage/__init__.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      453 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/storage/models.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1222 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/storage/tests.py
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.293624 django-stachoutils-3.3.2/tests/templates/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      332 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/templates/generic_list_filters_test.html
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      815 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/templates/generic_list_test.html
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.295480 django-stachoutils-3.3.2/tests/templatetags/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)        0 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/templatetags/__init__.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      566 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/templatetags/models.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     5940 2020-06-15 16:55:20.000000 django-stachoutils-3.3.2/tests/templatetags/test_filters.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     6017 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/templatetags/test_pagination_tags.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     7707 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/templatetags/test_tags.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     4390 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/templatetags/tests.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      877 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/templatetags/utils.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)       17 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/urls.py
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.296012 django-stachoutils-3.3.2/tests/utils/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)        0 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/utils/__init__.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     3546 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/utils/tests.py
-drwxr-xr-x   0 guerrastanislas   (501) staff       (20)        0 2022-04-04 12:39:29.297479 django-stachoutils-3.3.2/tests/views/
--rw-r--r--   0 guerrastanislas   (501) staff       (20)        0 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/views/__init__.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      127 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/views/actions.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      136 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/views/admin.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)     1546 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/views/models.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)      947 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/views/test_actions.py
--rw-r--r--   0 guerrastanislas   (501) staff       (20)    24400 2020-06-10 10:53:26.000000 django-stachoutils-3.3.2/tests/views/test_generic_view.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:11.000000 django-stachoutils-4.0.0/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1488 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/LICENSE
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      199 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/MANIFEST.in
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2531 2023-05-31 08:28:11.000000 django-stachoutils-4.0.0/PKG-INFO
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1256 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/README.rst
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:10.000000 django-stachoutils-4.0.0/django_stachoutils/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     3892 2023-05-31 07:02:07.000000 django-stachoutils-4.0.0/django_stachoutils/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      277 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/csv_utf8.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1799 2020-11-30 15:48:58.000000 django-stachoutils-4.0.0/django_stachoutils/decorators.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:10.000000 django-stachoutils-4.0.0/django_stachoutils/forms/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      347 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/forms/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      666 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/forms/fields.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     6062 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/forms/models.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     4062 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/forms/nested.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     6199 2023-05-31 08:09:59.000000 django-stachoutils-4.0.0/django_stachoutils/forms/widgets.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     3674 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/log.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:10.000000 django-stachoutils-4.0.0/django_stachoutils/management/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/management/__init__.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:10.000000 django-stachoutils-4.0.0/django_stachoutils/management/commands/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/management/commands/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    10369 2020-06-10 12:58:56.000000 django-stachoutils-4.0.0/django_stachoutils/management/commands/dumpdata_related.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1132 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/management/commands/hotspot_report.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      747 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/management/commands/sync_permissions.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      585 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/middlewares.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      185 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/models.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     3437 2022-04-04 12:34:34.000000 django-stachoutils-4.0.0/django_stachoutils/options.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1452 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/profiler.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2254 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/shortcuts.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1836 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/sql.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:10.000000 django-stachoutils-4.0.0/django_stachoutils/static/
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:10.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:10.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/css/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      191 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/css/admin_extras.css
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      331 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/css/commons.css
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1797 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/css/forms.css
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:10.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/img/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      517 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/img/filters.png
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      206 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/img/icon-inactive-no.gif
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      197 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/img/icon-inactive-yes.gif
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      176 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/img/icon-no.gif
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      299 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/img/icon-yes.gif
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      710 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/img/processing.png
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     6826 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/img/sprites.png
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:10.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/js/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1693 2022-02-25 16:39:28.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/js/admin_extras.js
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2193 2022-02-24 14:12:10.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/js/change_list.js
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2022 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/js/editeur.js
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1964 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/js/forms.js
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1589 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/js/jquery.AjaxCSRFprotection.js
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2878 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/js/jquery.charcounter.js
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1793 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/js/jquery.fieldselection.js
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:10.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    19113 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/jquery.poshytip.js
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    11435 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/jquery.poshytip.min.js
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:10.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/tip-darkgray/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1599 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/tip-darkgray/tip-darkgray.css
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     5199 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/tip-darkgray/tip-darkgray.png
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1261 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/tip-darkgray/tip-darkgray_arrows.png
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:10.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/tip-green/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1312 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/tip-green/tip-green.css
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      118 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/tip-green/tip-green_arrows.gif
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:10.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/tip-skyblue/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1421 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/tip-skyblue/tip-skyblue.css
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     4729 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/tip-skyblue/tip-skyblue.png
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      896 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/tip-skyblue/tip-skyblue_arrows.png
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:10.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/tip-twitter/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1539 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/tip-twitter/tip-twitter.css
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       87 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/tip-twitter/tip-twitter_arrows.gif
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:10.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/tip-violet/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1556 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/tip-violet/tip-violet.css
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     4916 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/tip-violet/tip-violet.png
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1409 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/tip-violet/tip-violet_arrows.png
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:10.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/tip-yellow/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1557 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/tip-yellow/tip-yellow.css
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     5069 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/tip-yellow/tip-yellow.png
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1402 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/tip-yellow/tip-yellow_arrows.png
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:10.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/tip-yellowsimple/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1617 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/tip-yellowsimple/tip-yellowsimple.css
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      107 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/tip-yellowsimple/tip-yellowsimple_arrows.gif
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      378 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/storage.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:10.000000 django-stachoutils-4.0.0/django_stachoutils/templates/
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:10.000000 django-stachoutils-4.0.0/django_stachoutils/templates/django_stachoutils/
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:10.000000 django-stachoutils-4.0.0/django_stachoutils/templates/django_stachoutils/forms/
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:10.000000 django-stachoutils-4.0.0/django_stachoutils/templates/django_stachoutils/forms/widgets/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      505 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/templates/django_stachoutils/forms/widgets/texte_editeur.html
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      456 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/templates/django_stachoutils/pagination.html
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      523 2022-02-28 14:16:20.000000 django-stachoutils-4.0.0/django_stachoutils/templates/django_stachoutils/pagination_bootstrap.html
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:10.000000 django-stachoutils-4.0.0/django_stachoutils/templatetags/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/templatetags/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    12315 2022-02-28 14:16:20.000000 django-stachoutils-4.0.0/django_stachoutils/templatetags/stachoutils_extras.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:10.000000 django-stachoutils-4.0.0/django_stachoutils/views/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/views/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      591 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/django_stachoutils/views/actions.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    15931 2023-05-31 08:08:37.000000 django-stachoutils-4.0.0/django_stachoutils/views/generic.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:10.000000 django-stachoutils-4.0.0/django_stachoutils.egg-info/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2531 2023-05-31 08:28:10.000000 django-stachoutils-4.0.0/django_stachoutils.egg-info/PKG-INFO
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     6556 2023-05-31 08:28:10.000000 django-stachoutils-4.0.0/django_stachoutils.egg-info/SOURCES.txt
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        1 2023-05-31 08:28:10.000000 django-stachoutils-4.0.0/django_stachoutils.egg-info/dependency_links.txt
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        7 2023-05-31 08:28:10.000000 django-stachoutils-4.0.0/django_stachoutils.egg-info/requires.txt
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       19 2023-05-31 08:28:10.000000 django-stachoutils-4.0.0/django_stachoutils.egg-info/top_level.txt
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       38 2023-05-31 08:28:11.000000 django-stachoutils-4.0.0/setup.cfg
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2162 2023-05-31 08:27:00.000000 django-stachoutils-4.0.0/setup.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:10.000000 django-stachoutils-4.0.0/tests/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      374 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/Makefile
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       34 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/coveragerc
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:11.000000 django-stachoutils-4.0.0/tests/forms/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    28672 2023-05-31 08:21:32.000000 django-stachoutils-4.0.0/tests/forms/.test_widgets.py.swp
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/forms/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1060 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/forms/models.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     5125 2021-12-20 11:10:00.000000 django-stachoutils-4.0.0/tests/forms/test_fields.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     4219 2021-12-20 11:10:00.000000 django-stachoutils-4.0.0/tests/forms/test_fields_with_thumbor.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    19278 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/forms/test_models.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     5168 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/forms/test_nested.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     9488 2023-05-31 08:21:23.000000 django-stachoutils-4.0.0/tests/forms/test_widgets.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:11.000000 django-stachoutils-4.0.0/tests/javascript/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1452 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/javascript/demo_texte_editeur.html
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      674 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/javascript/runtests.html
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:11.000000 django-stachoutils-4.0.0/tests/javascript/tests/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     7440 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/javascript/tests/test_widgets.js
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:11.000000 django-stachoutils-4.0.0/tests/log/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/log/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1325 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/log/test_smtp_handler.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2244 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/log/tests.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:11.000000 django-stachoutils-4.0.0/tests/media/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   206420 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/media/1st_Saab_9-3_SE.jpg
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   384780 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/media/Saab_9-3_Vector_sedan.jpg
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)   736699 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/media/home_1.jpg
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    65868 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/media/jardin.jpg
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    30317 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/media/terrasse.jpg
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:11.000000 django-stachoutils-4.0.0/tests/middlewares/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/middlewares/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1807 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/middlewares/tests.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:11.000000 django-stachoutils-4.0.0/tests/models/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/models/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      545 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/models/models.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      660 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/models/tests.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:11.000000 django-stachoutils-4.0.0/tests/options/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/options/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      380 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/options/models.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     4578 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/options/test_logs.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2262 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/options/tests.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:10.000000 django-stachoutils-4.0.0/tests/projects/
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:11.000000 django-stachoutils-4.0.0/tests/projects/django_project/
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:11.000000 django-stachoutils-4.0.0/tests/projects/django_project/django_project/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/projects/django_project/django_project/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     5635 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/projects/django_project/django_project/settings.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      124 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/projects/django_project/django_project/urls.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1443 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/projects/django_project/django_project/wsgi.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2683 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/projects/django_project/initial_data.json
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      257 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/projects/django_project/manage.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:11.000000 django-stachoutils-4.0.0/tests/projects/django_project/my_app/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/projects/django_project/my_app/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      849 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/projects/django_project/my_app/admin.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:11.000000 django-stachoutils-4.0.0/tests/projects/django_project/my_app/migrations/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2362 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/projects/django_project/my_app/migrations/0001_initial.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      450 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/projects/django_project/my_app/migrations/0002_musicgenre_history.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/projects/django_project/my_app/migrations/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2667 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/projects/django_project/my_app/models.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/projects/django_project/my_app/tests.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/projects/django_project/my_app/views.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     5225 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/runtests.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2235 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/settings.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:11.000000 django-stachoutils-4.0.0/tests/shortcuts/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/shortcuts/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      252 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/shortcuts/models.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     4004 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/shortcuts/tests.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:11.000000 django-stachoutils-4.0.0/tests/sql/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/sql/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      384 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/sql/models.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2527 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/sql/tests.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:11.000000 django-stachoutils-4.0.0/tests/storage/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/storage/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      453 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/storage/models.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1222 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/storage/tests.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:11.000000 django-stachoutils-4.0.0/tests/templates/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      332 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/templates/generic_list_filters_test.html
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      815 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/templates/generic_list_test.html
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:11.000000 django-stachoutils-4.0.0/tests/templatetags/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/templatetags/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      566 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/templatetags/models.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     5940 2020-06-15 16:55:20.000000 django-stachoutils-4.0.0/tests/templatetags/test_filters.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     6017 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/templatetags/test_pagination_tags.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     7707 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/templatetags/test_tags.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     4390 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/templatetags/tests.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      877 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/templatetags/utils.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       17 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/urls.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:11.000000 django-stachoutils-4.0.0/tests/utils/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/utils/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     3546 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/utils/tests.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2023-05-31 08:28:11.000000 django-stachoutils-4.0.0/tests/views/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/views/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      127 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/views/actions.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      136 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/views/admin.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1546 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/views/models.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      947 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/views/test_actions.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    24400 2020-06-10 10:53:26.000000 django-stachoutils-4.0.0/tests/views/test_generic_view.py
```

### Comparing `django-stachoutils-3.3.2/LICENSE` & `django-stachoutils-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/PKG-INFO` & `django-stachoutils-4.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,76 +1,73 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: django-stachoutils
-Version: 3.3.2
+Version: 4.0.0
 Summary: Commons for Django
 Home-page: https://github.com/Starou/django-stachoutils
 Author: Stanislas Guerra
 Author-email: stan@slashdev.me
 License: BSD Licence
 Project-URL: Source Code, https://github.com/Starou/django-stachoutils
 Project-URL: Issue Tracker, https://github.com/Starou/django-stachoutils/issues
+Description: ======================
+        Stachou's Django Utils
+        ======================
+        
+        .. image:: https://coveralls.io/repos/github/Starou/django-stachoutils/badge.svg?branch=master
+          :target: https://coveralls.io/github/Starou/django-stachoutils?branch=master
+        
+        .. image:: https://img.shields.io/pypi/v/django_stachoutils.svg
+            :target: https://pypi.python.org/pypi/django-stachoutils/
+            :alt: Current version
+        
+        .. image:: https://img.shields.io/pypi/pyversions/django_stachoutils.svg
+            :target: https://pypi.python.org/pypi/django-stachoutils/
+            :alt: Supported Python versions
+        
+        .. image:: https://img.shields.io/pypi/l/django_stachoutils.svg
+            :target: https://pypi.python.org/pypi/django-stachoutils/
+            :alt: License
+        
+        .. image:: https://travis-ci.org/Starou/django-stachoutils.svg
+            :target: https://travis-ci.org/Starou/django-stachoutils
+            :alt: Travis C.I.
+        
+        
+        This is mostly some common libs shared between several Django project I am working on.
+        
+        
+        Install
+        =======
+        
+        ::
+        
+            pip install django-stachoutils
+        
+        Tests
+        =====
+        
+        ::
+        
+            vagrant up
+            vagrant ssh
+            cd tests
+            make tests
+        
+        There is a demo project you can run (login: ``super:user``):
+        
+        ::
+        
+            cd tests/django_project
+            export PYTHONPATH=../../..:${PYTHONPATH}
+            python manage.py runserver
+        
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-License-File: LICENSE
-
-======================
-Stachou's Django Utils
-======================
-
-.. image:: https://coveralls.io/repos/github/Starou/django-stachoutils/badge.svg?branch=master
-  :target: https://coveralls.io/github/Starou/django-stachoutils?branch=master
-
-.. image:: https://img.shields.io/pypi/v/django_stachoutils.svg
-    :target: https://pypi.python.org/pypi/django-stachoutils/
-    :alt: Current version
-
-.. image:: https://img.shields.io/pypi/pyversions/django_stachoutils.svg
-    :target: https://pypi.python.org/pypi/django-stachoutils/
-    :alt: Supported Python versions
-
-.. image:: https://img.shields.io/pypi/l/django_stachoutils.svg
-    :target: https://pypi.python.org/pypi/django-stachoutils/
-    :alt: License
-
-.. image:: https://travis-ci.org/Starou/django-stachoutils.svg
-    :target: https://travis-ci.org/Starou/django-stachoutils
-    :alt: Travis C.I.
-
-
-This is mostly some common libs shared between several Django project I am working on.
-
-
-Install
-=======
-
-::
-
-    pip install django-stachoutils
-
-Tests
-=====
-
-::
-
-    vagrant up
-    vagrant ssh
-    cd tests
-    make tests
-
-There is a demo project you can run (login: ``super:user``):
-
-::
-
-    cd tests/django_project
-    export PYTHONPATH=../../..:${PYTHONPATH}
-    python manage.py runserver
-
-
```

### Comparing `django-stachoutils-3.3.2/README.rst` & `django-stachoutils-4.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/__init__.py` & `django-stachoutils-4.0.0/django_stachoutils/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
 from __future__ import unicode_literals
 
 from builtins import chr, map, range, str
+from urllib.parse import unquote
 import hashlib
 import re
 import unicodedata
 
 from datetime import datetime
 from django.utils import formats, dateformat
 from django.utils.encoding import force_str
 from django.utils.functional import keep_lazy_text
-from django.utils.http import urlunquote
 
 from .decorators import simple_decorator  # NOQA
 
 
 def format_datetime(value=None, date=True, time=True):
     if not date:
         format_type = 'TIME_FORMAT'
@@ -126,9 +126,9 @@
 
 def urldecode(url):
     out = {}
     get_params = (url.split('?')[1:] or [None])
     if get_params[0]:
         for param in get_params[0].split('&'):
             k, v = param.split('=')
-            out[k] = urlunquote(v)
+            out[k] = unquote(v)
     return out
```

### Comparing `django-stachoutils-3.3.2/django_stachoutils/decorators.py` & `django-stachoutils-4.0.0/django_stachoutils/decorators.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/forms/fields.py` & `django-stachoutils-4.0.0/django_stachoutils/forms/fields.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/forms/models.py` & `django-stachoutils-4.0.0/django_stachoutils/forms/models.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/forms/nested.py` & `django-stachoutils-4.0.0/django_stachoutils/forms/nested.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/forms/widgets.py` & `django-stachoutils-4.0.0/django_stachoutils/forms/widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 from builtins import object
+from urllib.parse import quote
 from django import forms
 from django.conf import settings
 from django.contrib.admin import widgets as admin_widgets
-from django.utils.http import quote
 from django.utils.safestring import mark_safe
 
 if "django_thumbor" in settings.INSTALLED_APPS:
     from django_thumbor import generate_url
 else:
     from django.template import Context, Template
```

### Comparing `django-stachoutils-3.3.2/django_stachoutils/log.py` & `django-stachoutils-4.0.0/django_stachoutils/log.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/management/commands/dumpdata_related.py` & `django-stachoutils-4.0.0/django_stachoutils/management/commands/dumpdata_related.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/management/commands/hotspot_report.py` & `django-stachoutils-4.0.0/django_stachoutils/management/commands/hotspot_report.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/management/commands/sync_permissions.py` & `django-stachoutils-4.0.0/django_stachoutils/management/commands/sync_permissions.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/middlewares.py` & `django-stachoutils-4.0.0/django_stachoutils/middlewares.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/options.py` & `django-stachoutils-4.0.0/django_stachoutils/options.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/profiler.py` & `django-stachoutils-4.0.0/django_stachoutils/profiler.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/shortcuts.py` & `django-stachoutils-4.0.0/django_stachoutils/shortcuts.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/sql.py` & `django-stachoutils-4.0.0/django_stachoutils/sql.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/css/forms.css` & `django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/css/forms.css`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/img/filters.png` & `django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/img/filters.png`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/img/processing.png` & `django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/img/processing.png`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/img/sprites.png` & `django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/img/sprites.png`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/js/admin_extras.js` & `django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/js/admin_extras.js`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/js/change_list.js` & `django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/js/change_list.js`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/js/editeur.js` & `django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/js/editeur.js`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/js/forms.js` & `django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/js/forms.js`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/js/jquery.AjaxCSRFprotection.js` & `django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/js/jquery.AjaxCSRFprotection.js`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/js/jquery.charcounter.js` & `django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/js/jquery.charcounter.js`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/js/jquery.fieldselection.js` & `django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/js/jquery.fieldselection.js`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/jquery.poshytip.js` & `django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/jquery.poshytip.js`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/jquery.poshytip.min.js` & `django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/jquery.poshytip.min.js`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/tip-darkgray/tip-darkgray.css` & `django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/tip-darkgray/tip-darkgray.css`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/tip-darkgray/tip-darkgray.png` & `django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/tip-darkgray/tip-darkgray.png`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/tip-darkgray/tip-darkgray_arrows.png` & `django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/tip-darkgray/tip-darkgray_arrows.png`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/tip-green/tip-green.css` & `django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/tip-green/tip-green.css`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/tip-skyblue/tip-skyblue.css` & `django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/tip-skyblue/tip-skyblue.css`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/tip-skyblue/tip-skyblue.png` & `django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/tip-skyblue/tip-skyblue.png`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/tip-skyblue/tip-skyblue_arrows.png` & `django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/tip-skyblue/tip-skyblue_arrows.png`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/tip-twitter/tip-twitter.css` & `django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/tip-twitter/tip-twitter.css`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/tip-violet/tip-violet.css` & `django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/tip-violet/tip-violet.css`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/tip-violet/tip-violet.png` & `django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/tip-violet/tip-violet.png`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/tip-violet/tip-violet_arrows.png` & `django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/tip-violet/tip-violet_arrows.png`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/tip-yellow/tip-yellow.css` & `django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/tip-yellow/tip-yellow.css`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/tip-yellow/tip-yellow.png` & `django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/tip-yellow/tip-yellow.png`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/tip-yellow/tip-yellow_arrows.png` & `django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/tip-yellow/tip-yellow_arrows.png`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/static/django_stachoutils/poshytip/tip-yellowsimple/tip-yellowsimple.css` & `django-stachoutils-4.0.0/django_stachoutils/static/django_stachoutils/poshytip/tip-yellowsimple/tip-yellowsimple.css`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/templates/django_stachoutils/pagination_bootstrap.html` & `django-stachoutils-4.0.0/django_stachoutils/templates/django_stachoutils/pagination_bootstrap.html`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/templatetags/stachoutils_extras.py` & `django-stachoutils-4.0.0/django_stachoutils/templatetags/stachoutils_extras.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/views/actions.py` & `django-stachoutils-4.0.0/django_stachoutils/views/actions.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/django_stachoutils/views/generic.py` & `django-stachoutils-4.0.0/django_stachoutils/views/generic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # -*- coding: utf-8 -*-
 
 from builtins import object
 from builtins import str as text
+from urllib.parse import unquote
 from django.contrib import admin, messages
 from django.contrib.admin.helpers import ACTION_CHECKBOX_NAME
 from django.contrib.admin.utils import label_for_field
 from django.db.models import Q
 from django.db.models.query import QuerySet
 from django.db.models.fields import BooleanField
 from django.http import HttpResponseRedirect
 from django.shortcuts import render
-from django.utils.http import urlencode, urlunquote
+from django.utils.http import urlencode
 from django.utils.translation import gettext as _
 from django_stachoutils.options import paginate
 from django_stachoutils.views.actions import regroup_actions
 
 ORDER_BY_ATTR = 'o'
 ORDER_TYPE_ATTR = 'ot'
 
@@ -323,15 +324,15 @@
     """ Return {'key': 'value', ...} """
 
     filters_keys = [f[0] for f in filters]
 
     current_filters = {}
     for k, v in request.GET.items():
         if k.replace('__exact', '') in filters_keys or is_a_filter(model, k):
-            current_filters[str(k)] = str(urlunquote(v))
+            current_filters[str(k)] = str(unquote(v))
     return current_filters
 
 
 ##
 
 LOOKUPS = [
     'exact',
```

### Comparing `django-stachoutils-3.3.2/django_stachoutils.egg-info/PKG-INFO` & `django-stachoutils-4.0.0/django_stachoutils.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,76 +1,73 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: django-stachoutils
-Version: 3.3.2
+Version: 4.0.0
 Summary: Commons for Django
 Home-page: https://github.com/Starou/django-stachoutils
 Author: Stanislas Guerra
 Author-email: stan@slashdev.me
 License: BSD Licence
 Project-URL: Source Code, https://github.com/Starou/django-stachoutils
 Project-URL: Issue Tracker, https://github.com/Starou/django-stachoutils/issues
+Description: ======================
+        Stachou's Django Utils
+        ======================
+        
+        .. image:: https://coveralls.io/repos/github/Starou/django-stachoutils/badge.svg?branch=master
+          :target: https://coveralls.io/github/Starou/django-stachoutils?branch=master
+        
+        .. image:: https://img.shields.io/pypi/v/django_stachoutils.svg
+            :target: https://pypi.python.org/pypi/django-stachoutils/
+            :alt: Current version
+        
+        .. image:: https://img.shields.io/pypi/pyversions/django_stachoutils.svg
+            :target: https://pypi.python.org/pypi/django-stachoutils/
+            :alt: Supported Python versions
+        
+        .. image:: https://img.shields.io/pypi/l/django_stachoutils.svg
+            :target: https://pypi.python.org/pypi/django-stachoutils/
+            :alt: License
+        
+        .. image:: https://travis-ci.org/Starou/django-stachoutils.svg
+            :target: https://travis-ci.org/Starou/django-stachoutils
+            :alt: Travis C.I.
+        
+        
+        This is mostly some common libs shared between several Django project I am working on.
+        
+        
+        Install
+        =======
+        
+        ::
+        
+            pip install django-stachoutils
+        
+        Tests
+        =====
+        
+        ::
+        
+            vagrant up
+            vagrant ssh
+            cd tests
+            make tests
+        
+        There is a demo project you can run (login: ``super:user``):
+        
+        ::
+        
+            cd tests/django_project
+            export PYTHONPATH=../../..:${PYTHONPATH}
+            python manage.py runserver
+        
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-License-File: LICENSE
-
-======================
-Stachou's Django Utils
-======================
-
-.. image:: https://coveralls.io/repos/github/Starou/django-stachoutils/badge.svg?branch=master
-  :target: https://coveralls.io/github/Starou/django-stachoutils?branch=master
-
-.. image:: https://img.shields.io/pypi/v/django_stachoutils.svg
-    :target: https://pypi.python.org/pypi/django-stachoutils/
-    :alt: Current version
-
-.. image:: https://img.shields.io/pypi/pyversions/django_stachoutils.svg
-    :target: https://pypi.python.org/pypi/django-stachoutils/
-    :alt: Supported Python versions
-
-.. image:: https://img.shields.io/pypi/l/django_stachoutils.svg
-    :target: https://pypi.python.org/pypi/django-stachoutils/
-    :alt: License
-
-.. image:: https://travis-ci.org/Starou/django-stachoutils.svg
-    :target: https://travis-ci.org/Starou/django-stachoutils
-    :alt: Travis C.I.
-
-
-This is mostly some common libs shared between several Django project I am working on.
-
-
-Install
-=======
-
-::
-
-    pip install django-stachoutils
-
-Tests
-=====
-
-::
-
-    vagrant up
-    vagrant ssh
-    cd tests
-    make tests
-
-There is a demo project you can run (login: ``super:user``):
-
-::
-
-    cd tests/django_project
-    export PYTHONPATH=../../..:${PYTHONPATH}
-    python manage.py runserver
-
-
```

### Comparing `django-stachoutils-3.3.2/django_stachoutils.egg-info/SOURCES.txt` & `django-stachoutils-4.0.0/django_stachoutils.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -69,20 +69,20 @@
 django_stachoutils/templates/django_stachoutils/pagination_bootstrap.html
 django_stachoutils/templates/django_stachoutils/forms/widgets/texte_editeur.html
 django_stachoutils/templatetags/__init__.py
 django_stachoutils/templatetags/stachoutils_extras.py
 django_stachoutils/views/__init__.py
 django_stachoutils/views/actions.py
 django_stachoutils/views/generic.py
-tests/.runtests.py.swp
 tests/Makefile
 tests/coveragerc
 tests/runtests.py
 tests/settings.py
 tests/urls.py
+tests/forms/.test_widgets.py.swp
 tests/forms/__init__.py
 tests/forms/models.py
 tests/forms/test_fields.py
 tests/forms/test_fields_with_thumbor.py
 tests/forms/test_models.py
 tests/forms/test_nested.py
 tests/forms/test_widgets.py
```

### Comparing `django-stachoutils-3.3.2/setup.py` & `django-stachoutils-4.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 
 setup(
     name="django-stachoutils",
-    version="3.3.2",
+    version="4.0.0",
     license='BSD Licence',
     author='Stanislas Guerra',
     author_email='stan@slashdev.me',
     description='Commons for Django',
     url='https://github.com/Starou/django-stachoutils',
     project_urls={
         'Source Code': 'https://github.com/Starou/django-stachoutils',
@@ -49,12 +49,12 @@
         'Environment :: Web Environment',
         'Framework :: Django',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.9',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
     ]
 )
```

### Comparing `django-stachoutils-3.3.2/tests/forms/models.py` & `django-stachoutils-4.0.0/tests/forms/models.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/tests/forms/test_fields.py` & `django-stachoutils-4.0.0/tests/forms/test_fields.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/tests/forms/test_fields_with_thumbor.py` & `django-stachoutils-4.0.0/tests/forms/test_fields_with_thumbor.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/tests/forms/test_models.py` & `django-stachoutils-4.0.0/tests/forms/test_models.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/tests/forms/test_nested.py` & `django-stachoutils-4.0.0/tests/forms/test_nested.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/tests/forms/test_widgets.py` & `django-stachoutils-4.0.0/tests/forms/test_widgets.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,17 +47,17 @@
               </td>
             </tr>
             """
         )
         self.assertHTMLEqual(
             str(form.media),
             """
-            <script type="text/javascript" src="/static/django_stachoutils/js/jquery.charcounter.js"></script>
-            <script type="text/javascript" src="/static/django_stachoutils/js/jquery.fieldselection.js"></script>
-            <script type="text/javascript" src="/static/django_stachoutils/js/editeur.js"></script>
+            <script src="/static/django_stachoutils/js/jquery.charcounter.js"></script>
+            <script src="/static/django_stachoutils/js/jquery.fieldselection.js"></script>
+            <script src="/static/django_stachoutils/js/editeur.js"></script>
             """
         )
 
     def test_render_textarea_counter_widget(self):
         from django_stachoutils.forms.widgets import TextareaCounter
 
         class CarForm(forms.ModelForm):
@@ -98,17 +98,17 @@
               </td>
             </tr>
             """
         )
         self.assertHTMLEqual(
             str(form.media),
             """
-            <script type="text/javascript" src="/static/django_stachoutils/js/jquery.charcounter.js"></script>
-            <script type="text/javascript" src="/static/django_stachoutils/js/jquery.fieldselection.js"></script>
-            <script type="text/javascript" src="/static/django_stachoutils/js/editeur.js"></script>
+            <script src="/static/django_stachoutils/js/jquery.charcounter.js"></script>
+            <script src="/static/django_stachoutils/js/jquery.fieldselection.js"></script>
+            <script src="/static/django_stachoutils/js/editeur.js"></script>
             """
         )
 
     def test_render_textarea_counter_widget_reversed_counter(self):
         from django_stachoutils.forms.widgets import TextareaCounter
 
         class CarForm(forms.ModelForm):
@@ -179,17 +179,17 @@
               <td><input type="text" name="brand" required id="id_brand" maxlength="100" /></td>
             </tr>
             """
         )
         self.assertHTMLEqual(
             str(form.media),
             """
-            <script type="text/javascript" src="/static/django_stachoutils/js/jquery.charcounter.js"></script>
-            <script type="text/javascript" src="/static/django_stachoutils/js/jquery.fieldselection.js"></script>
-            <script type="text/javascript" src="/static/django_stachoutils/js/editeur.js"></script>
+            <script src="/static/django_stachoutils/js/jquery.charcounter.js"></script>
+            <script src="/static/django_stachoutils/js/jquery.fieldselection.js"></script>
+            <script src="/static/django_stachoutils/js/editeur.js"></script>
             """
         )
 
     def test_render_textinput_counter_widget_reversed_counter(self):
         from django_stachoutils.forms.widgets import TextInputCounter
 
         class CarForm(forms.ModelForm):
```

### Comparing `django-stachoutils-3.3.2/tests/javascript/demo_texte_editeur.html` & `django-stachoutils-4.0.0/tests/javascript/demo_texte_editeur.html`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/tests/javascript/runtests.html` & `django-stachoutils-4.0.0/tests/javascript/runtests.html`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/tests/javascript/tests/test_widgets.js` & `django-stachoutils-4.0.0/tests/javascript/tests/test_widgets.js`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/tests/log/test_smtp_handler.py` & `django-stachoutils-4.0.0/tests/log/test_smtp_handler.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/tests/log/tests.py` & `django-stachoutils-4.0.0/tests/log/tests.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/tests/media/1st_Saab_9-3_SE.jpg` & `django-stachoutils-4.0.0/tests/media/1st_Saab_9-3_SE.jpg`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/tests/media/Saab_9-3_Vector_sedan.jpg` & `django-stachoutils-4.0.0/tests/media/Saab_9-3_Vector_sedan.jpg`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/tests/media/home_1.jpg` & `django-stachoutils-4.0.0/tests/media/home_1.jpg`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/tests/media/jardin.jpg` & `django-stachoutils-4.0.0/tests/media/jardin.jpg`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/tests/media/terrasse.jpg` & `django-stachoutils-4.0.0/tests/media/terrasse.jpg`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/tests/middlewares/tests.py` & `django-stachoutils-4.0.0/tests/middlewares/tests.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/tests/models/models.py` & `django-stachoutils-4.0.0/tests/models/models.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/tests/models/tests.py` & `django-stachoutils-4.0.0/tests/models/tests.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/tests/options/test_logs.py` & `django-stachoutils-4.0.0/tests/options/test_logs.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/tests/options/tests.py` & `django-stachoutils-4.0.0/tests/options/tests.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/tests/projects/django_project/django_project/settings.py` & `django-stachoutils-4.0.0/tests/projects/django_project/django_project/settings.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/tests/projects/django_project/django_project/wsgi.py` & `django-stachoutils-4.0.0/tests/projects/django_project/django_project/wsgi.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/tests/projects/django_project/initial_data.json` & `django-stachoutils-4.0.0/tests/projects/django_project/initial_data.json`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/tests/projects/django_project/my_app/admin.py` & `django-stachoutils-4.0.0/tests/projects/django_project/my_app/admin.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/tests/projects/django_project/my_app/migrations/0001_initial.py` & `django-stachoutils-4.0.0/tests/projects/django_project/my_app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/tests/projects/django_project/my_app/models.py` & `django-stachoutils-4.0.0/tests/projects/django_project/my_app/models.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/tests/runtests.py` & `django-stachoutils-4.0.0/tests/runtests.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/tests/settings.py` & `django-stachoutils-4.0.0/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/tests/shortcuts/tests.py` & `django-stachoutils-4.0.0/tests/shortcuts/tests.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/tests/sql/tests.py` & `django-stachoutils-4.0.0/tests/sql/tests.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/tests/storage/tests.py` & `django-stachoutils-4.0.0/tests/storage/tests.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/tests/templates/generic_list_test.html` & `django-stachoutils-4.0.0/tests/templates/generic_list_test.html`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/tests/templatetags/models.py` & `django-stachoutils-4.0.0/tests/templatetags/models.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/tests/templatetags/test_filters.py` & `django-stachoutils-4.0.0/tests/templatetags/test_filters.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/tests/templatetags/test_pagination_tags.py` & `django-stachoutils-4.0.0/tests/templatetags/test_pagination_tags.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/tests/templatetags/test_tags.py` & `django-stachoutils-4.0.0/tests/templatetags/test_tags.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/tests/templatetags/tests.py` & `django-stachoutils-4.0.0/tests/templatetags/tests.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/tests/templatetags/utils.py` & `django-stachoutils-4.0.0/tests/templatetags/utils.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/tests/utils/tests.py` & `django-stachoutils-4.0.0/tests/utils/tests.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/tests/views/models.py` & `django-stachoutils-4.0.0/tests/views/models.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/tests/views/test_actions.py` & `django-stachoutils-4.0.0/tests/views/test_actions.py`

 * *Files identical despite different names*

### Comparing `django-stachoutils-3.3.2/tests/views/test_generic_view.py` & `django-stachoutils-4.0.0/tests/views/test_generic_view.py`

 * *Files identical despite different names*

