# Comparing `tmp/django-bom-1.98.tar.gz` & `tmp/django-bom-1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-bom-1.98.tar", last modified: Sun Oct 20 00:07:55 2019, max compression
+gzip compressed data, was "dist/django-bom-1.99.tar", last modified: Sun Oct 20 19:33:43 2019, max compression
```

## Comparing `django-bom-1.98.tar` & `django-bom-1.99.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2019-10-20 00:07:55.000000 django-bom-1.98/
--rw-r--r--   0 mike       (501) staff       (20)     1070 2019-10-16 22:03:06.000000 django-bom-1.98/LICENSE
--rw-r--r--   0 mike       (501) staff       (20)      156 2019-10-16 22:03:06.000000 django-bom-1.98/MANIFEST.in
--rw-r--r--   0 mike       (501) staff       (20)     6845 2019-10-20 00:07:55.000000 django-bom-1.98/PKG-INFO
--rw-r--r--   0 mike       (501) staff       (20)     4889 2019-10-16 22:03:06.000000 django-bom-1.98/README.md
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2019-10-20 00:07:55.000000 django-bom-1.98/bom/
--rw-r--r--   0 mike       (501) staff       (20)       41 2019-10-16 22:03:06.000000 django-bom-1.98/bom/__init__.py
--rw-r--r--   0 mike       (501) staff       (20)     3754 2019-10-16 22:03:06.000000 django-bom-1.98/bom/admin.py
--rw-r--r--   0 mike       (501) staff       (20)      147 2019-10-16 22:03:06.000000 django-bom-1.98/bom/apps.py
--rw-r--r--   0 mike       (501) staff       (20)      309 2019-10-16 22:03:06.000000 django-bom-1.98/bom/context_processors.py
--rw-r--r--   0 mike       (501) staff       (20)      346 2019-10-16 22:03:06.000000 django-bom-1.98/bom/convert.py
--rw-r--r--   0 mike       (501) staff       (20)      645 2019-10-16 22:03:06.000000 django-bom-1.98/bom/decorators.py
--rw-r--r--   0 mike       (501) staff       (20)    11675 2019-10-16 22:03:06.000000 django-bom-1.98/bom/forms.py
--rw-r--r--   0 mike       (501) staff       (20)    12608 2019-10-19 23:14:11.000000 django-bom-1.98/bom/helpers.py
--rw-r--r--   0 mike       (501) staff       (20)      883 2019-10-16 22:03:06.000000 django-bom-1.98/bom/local_settings.py
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2019-10-20 00:07:55.000000 django-bom-1.98/bom/migrations/
--rw-r--r--   0 mike       (501) staff       (20)     7005 2019-10-16 22:03:06.000000 django-bom-1.98/bom/migrations/0001_initial.py
--rw-r--r--   0 mike       (501) staff       (20)      753 2019-10-16 22:03:06.000000 django-bom-1.98/bom/migrations/0002_auto_20180908_2151.py
--rw-r--r--   0 mike       (501) staff       (20)      414 2019-10-16 22:03:06.000000 django-bom-1.98/bom/migrations/0003_sellerpart_data_source.py
--rw-r--r--   0 mike       (501) staff       (20)      432 2019-10-16 22:03:06.000000 django-bom-1.98/bom/migrations/0004_auto_20180911_0011.py
--rw-r--r--   0 mike       (501) staff       (20)     2402 2019-10-16 22:03:06.000000 django-bom-1.98/bom/migrations/0005_auto_20181007_1934.py
--rw-r--r--   0 mike       (501) staff       (20)     1249 2019-10-16 22:03:06.000000 django-bom-1.98/bom/migrations/0006_auto_20181007_1949.py
--rw-r--r--   0 mike       (501) staff       (20)      569 2019-10-16 22:03:06.000000 django-bom-1.98/bom/migrations/0007_auto_20181009_0256.py
--rw-r--r--   0 mike       (501) staff       (20)      570 2019-10-16 22:03:06.000000 django-bom-1.98/bom/migrations/0008_auto_20181030_0427.py
--rw-r--r--   0 mike       (501) staff       (20)      404 2019-10-16 22:03:06.000000 django-bom-1.98/bom/migrations/0009_subpart_reference.py
--rw-r--r--   0 mike       (501) staff       (20)      632 2019-10-16 22:03:06.000000 django-bom-1.98/bom/migrations/0010_auto_20181202_0733.py
--rw-r--r--   0 mike       (501) staff       (20)      555 2019-10-16 22:03:06.000000 django-bom-1.98/bom/migrations/0011_auto_20181202_2113.py
--rw-r--r--   0 mike       (501) staff       (20)     1511 2019-10-16 22:03:06.000000 django-bom-1.98/bom/migrations/0012_partchangehistory.py
--rw-r--r--   0 mike       (501) staff       (20)      472 2019-10-16 22:03:06.000000 django-bom-1.98/bom/migrations/0013_auto_20190222_1631.py
--rw-r--r--   0 mike       (501) staff       (20)      369 2019-10-16 22:03:06.000000 django-bom-1.98/bom/migrations/0014_auto_20190223_2353.py
--rw-r--r--   0 mike       (501) staff       (20)     4673 2019-10-16 22:03:06.000000 django-bom-1.98/bom/migrations/0015_auto_20190303_1915.py
--rw-r--r--   0 mike       (501) staff       (20)     1800 2019-10-16 22:03:06.000000 django-bom-1.98/bom/migrations/0016_auto_20190405_2308.py
--rw-r--r--   0 mike       (501) staff       (20)      382 2019-10-16 22:03:06.000000 django-bom-1.98/bom/migrations/0017_auto_20190616_1912.py
--rw-r--r--   0 mike       (501) staff       (20)      688 2019-10-16 22:03:06.000000 django-bom-1.98/bom/migrations/0018_auto_20190616_2143.py
--rw-r--r--   0 mike       (501) staff       (20)     1590 2019-10-16 22:03:06.000000 django-bom-1.98/bom/migrations/0019_auto_20190624_1246.py
--rw-r--r--   0 mike       (501) staff       (20)     1147 2019-10-16 22:03:06.000000 django-bom-1.98/bom/migrations/0020_auto_20190627_0207.py
--rw-r--r--   0 mike       (501) staff       (20)      625 2019-10-16 22:03:06.000000 django-bom-1.98/bom/migrations/0021_auto_20190627_0428.py
--rw-r--r--   0 mike       (501) staff       (20)     1025 2019-10-16 22:03:06.000000 django-bom-1.98/bom/migrations/0022_auto_20190811_2140.py
--rw-r--r--   0 mike       (501) staff       (20)        0 2019-10-16 22:03:06.000000 django-bom-1.98/bom/migrations/__init__.py
--rw-r--r--   0 mike       (501) staff       (20)    16340 2019-10-16 22:03:06.000000 django-bom-1.98/bom/models.py
--rw-r--r--   0 mike       (501) staff       (20)     6440 2019-10-19 22:02:03.000000 django-bom-1.98/bom/settings.py
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2019-10-20 00:07:55.000000 django-bom-1.98/bom/static/
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2019-10-20 00:07:55.000000 django-bom-1.98/bom/static/bom/
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2019-10-20 00:07:55.000000 django-bom-1.98/bom/static/bom/css/
--rwxr-xr-x   0 mike       (501) staff       (20)      652 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/css/jquery.treetable.css
--rw-r--r--   0 mike       (501) staff       (20)   141841 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/css/materialize.min.css
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2019-10-20 00:07:55.000000 django-bom-1.98/bom/static/bom/img/
--rw-r--r--   0 mike       (501) staff       (20)      127 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/img/_ionicons_svg_md-arrow-dropdown.svg
--rw-r--r--   0 mike       (501) staff       (20)      127 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/img/_ionicons_svg_md-arrow-dropright.svg
--rw-r--r--   0 mike       (501) staff       (20)     1150 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/img/favicon.ico
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2019-10-20 00:07:55.000000 django-bom-1.98/bom/static/bom/img/google/
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2019-10-20 00:07:55.000000 django-bom-1.98/bom/static/bom/img/google/web/
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2019-10-20 00:07:55.000000 django-bom-1.98/bom/static/bom/img/google/web/1x/
--rw-r--r--   0 mike       (501) staff       (20)     2308 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/img/google/web/1x/btn_google_signin_dark_disabled_web.png
--rw-r--r--   0 mike       (501) staff       (20)     4185 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/img/google/web/1x/btn_google_signin_dark_focus_web.png
--rw-r--r--   0 mike       (501) staff       (20)     3983 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/img/google/web/1x/btn_google_signin_dark_normal_web.png
--rw-r--r--   0 mike       (501) staff       (20)     4236 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/img/google/web/1x/btn_google_signin_dark_pressed_web.png
--rw-r--r--   0 mike       (501) staff       (20)     2308 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/img/google/web/1x/btn_google_signin_light_disabled_web.png
--rw-r--r--   0 mike       (501) staff       (20)     4328 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/img/google/web/1x/btn_google_signin_light_focus_web.png
--rw-r--r--   0 mike       (501) staff       (20)     4099 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/img/google/web/1x/btn_google_signin_light_normal_web.png
--rw-r--r--   0 mike       (501) staff       (20)     4135 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/img/google/web/1x/btn_google_signin_light_pressed_web.png
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2019-10-20 00:07:55.000000 django-bom-1.98/bom/static/bom/img/google/web/2x/
--rw-r--r--   0 mike       (501) staff       (20)     4897 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/img/google/web/2x/btn_google_signin_dark_disabled_web@2x.png
--rw-r--r--   0 mike       (501) staff       (20)     8513 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/img/google/web/2x/btn_google_signin_dark_focus_web@2x.png
--rw-r--r--   0 mike       (501) staff       (20)     8001 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/img/google/web/2x/btn_google_signin_dark_normal_web@2x.png
--rw-r--r--   0 mike       (501) staff       (20)     8483 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/img/google/web/2x/btn_google_signin_dark_pressed_web@2x.png
--rw-r--r--   0 mike       (501) staff       (20)     4897 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/img/google/web/2x/btn_google_signin_light_disabled_web@2x.png
--rw-r--r--   0 mike       (501) staff       (20)     8664 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/img/google/web/2x/btn_google_signin_light_focus_web@2x.png
--rw-r--r--   0 mike       (501) staff       (20)     8055 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/img/google/web/2x/btn_google_signin_light_normal_web@2x.png
--rw-r--r--   0 mike       (501) staff       (20)     8265 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/img/google/web/2x/btn_google_signin_light_pressed_web@2x.png
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2019-10-20 00:07:55.000000 django-bom-1.98/bom/static/bom/img/google/web/vector/
--rw-r--r--   0 mike       (501) staff       (20)    20286 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/img/google/web/vector/btn_google_dark_disabled_ios.eps
--rw-r--r--   0 mike       (501) staff       (20)     1996 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/img/google/web/vector/btn_google_dark_disabled_ios.svg
--rw-r--r--   0 mike       (501) staff       (20)    94048 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/img/google/web/vector/btn_google_dark_focus_ios.eps
--rw-r--r--   0 mike       (501) staff       (20)     4917 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/img/google/web/vector/btn_google_dark_focus_ios.svg
--rw-r--r--   0 mike       (501) staff       (20)    26465 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/img/google/web/vector/btn_google_dark_normal_ios.eps
--rw-r--r--   0 mike       (501) staff       (20)     4779 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/img/google/web/vector/btn_google_dark_normal_ios.svg
--rw-r--r--   0 mike       (501) staff       (20)    26484 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/img/google/web/vector/btn_google_dark_pressed_ios.eps
--rw-r--r--   0 mike       (501) staff       (20)     4781 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/img/google/web/vector/btn_google_dark_pressed_ios.svg
--rw-r--r--   0 mike       (501) staff       (20)    20286 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/img/google/web/vector/btn_google_light_disabled_ios.eps
--rw-r--r--   0 mike       (501) staff       (20)     1998 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/img/google/web/vector/btn_google_light_disabled_ios.svg
--rw-r--r--   0 mike       (501) staff       (20)    93663 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/img/google/web/vector/btn_google_light_focus_ios.eps
--rw-r--r--   0 mike       (501) staff       (20)     4496 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/img/google/web/vector/btn_google_light_focus_ios.svg
--rw-r--r--   0 mike       (501) staff       (20)    26080 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/img/google/web/vector/btn_google_light_normal_ios.eps
--rw-r--r--   0 mike       (501) staff       (20)     4358 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/img/google/web/vector/btn_google_light_normal_ios.svg
--rw-r--r--   0 mike       (501) staff       (20)    26107 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/img/google/web/vector/btn_google_light_pressed_ios.eps
--rw-r--r--   0 mike       (501) staff       (20)     4360 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/img/google/web/vector/btn_google_light_pressed_ios.svg
--rw-r--r--   0 mike       (501) staff       (20)     1102 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/img/google_drive_logo.svg
--rw-r--r--   0 mike       (501) staff       (20)    42071 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/img/indabom.png
--rw-r--r--   0 mike       (501) staff       (20)     1351 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/img/octopart_blue.svg
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2019-10-20 00:07:55.000000 django-bom-1.98/bom/static/bom/js/
--rw-r--r--   0 mike       (501) staff       (20)     1271 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/js/jquery.ba-floatingscrollbar.min.js
--rwxr-xr-x   0 mike       (501) staff       (20)    16611 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/js/jquery.treetable.js
--rw-r--r--   0 mike       (501) staff       (20)   181114 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/js/materialize.min.js
--rw-r--r--   0 mike       (501) staff       (20)     2765 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/style.css
--rw-r--r--   0 mike       (501) staff       (20)    24032 2019-10-16 22:03:06.000000 django-bom-1.98/bom/static/bom/treetable-theme.css
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2019-10-20 00:07:55.000000 django-bom-1.98/bom/templates/
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2019-10-20 00:07:55.000000 django-bom-1.98/bom/templates/bom/
--rw-r--r--   0 mike       (501) staff       (20)     2344 2019-10-16 22:03:06.000000 django-bom-1.98/bom/templates/bom/add-manufacturer-part.html
--rw-r--r--   0 mike       (501) staff       (20)     3271 2019-10-16 22:03:06.000000 django-bom-1.98/bom/templates/bom/add-sellerpart.html
--rw-r--r--   0 mike       (501) staff       (20)     5947 2019-10-16 22:03:06.000000 django-bom-1.98/bom/templates/bom/base.html
--rw-r--r--   0 mike       (501) staff       (20)     1004 2019-10-16 22:03:06.000000 django-bom-1.98/bom/templates/bom/bom-action-btn.html
--rw-r--r--   0 mike       (501) staff       (20)     1030 2019-10-16 22:03:06.000000 django-bom-1.98/bom/templates/bom/bom-form.html
--rw-r--r--   0 mike       (501) staff       (20)      296 2019-10-16 22:03:06.000000 django-bom-1.98/bom/templates/bom/bom-signup.html
--rw-r--r--   0 mike       (501) staff       (20)     2813 2019-10-20 00:07:18.000000 django-bom-1.98/bom/templates/bom/create-part.html
--rw-r--r--   0 mike       (501) staff       (20)     4586 2019-10-16 22:03:06.000000 django-bom-1.98/bom/templates/bom/dashboard.html
--rw-r--r--   0 mike       (501) staff       (20)     2299 2019-10-16 22:03:06.000000 django-bom-1.98/bom/templates/bom/edit-manufacturer-part.html
--rw-r--r--   0 mike       (501) staff       (20)     2190 2019-10-16 22:03:06.000000 django-bom-1.98/bom/templates/bom/edit-part.html
--rw-r--r--   0 mike       (501) staff       (20)      700 2019-10-16 22:03:06.000000 django-bom-1.98/bom/templates/bom/error.html
--rw-r--r--   0 mike       (501) staff       (20)    32522 2019-10-16 22:03:06.000000 django-bom-1.98/bom/templates/bom/part-info.html
--rw-r--r--   0 mike       (501) staff       (20)    10404 2019-10-16 22:03:06.000000 django-bom-1.98/bom/templates/bom/part-rev-manage-bom.html
--rw-r--r--   0 mike       (501) staff       (20)     1323 2019-10-16 22:03:06.000000 django-bom-1.98/bom/templates/bom/part-revision-edit.html
--rw-r--r--   0 mike       (501) staff       (20)     1960 2019-10-16 22:03:06.000000 django-bom-1.98/bom/templates/bom/part-revision-new.html
--rw-r--r--   0 mike       (501) staff       (20)     1826 2019-10-16 22:03:06.000000 django-bom-1.98/bom/templates/bom/part-revision-release.html
--rw-r--r--   0 mike       (501) staff       (20)     4444 2019-10-16 22:03:06.000000 django-bom-1.98/bom/templates/bom/settings.html
--rw-r--r--   0 mike       (501) staff       (20)     1945 2019-10-16 22:03:06.000000 django-bom-1.98/bom/templates/bom/upload-parts.html
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2019-10-20 00:07:55.000000 django-bom-1.98/bom/templates/registration/
--rw-r--r--   0 mike       (501) staff       (20)     1100 2019-10-16 22:03:06.000000 django-bom-1.98/bom/templates/registration/login.html
--rw-r--r--   0 mike       (501) staff       (20)    25968 2019-10-19 23:24:02.000000 django-bom-1.98/bom/tests.py
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2019-10-20 00:07:55.000000 django-bom-1.98/bom/third_party_apis/
--rw-r--r--   0 mike       (501) staff       (20)        0 2019-10-16 22:03:06.000000 django-bom-1.98/bom/third_party_apis/__init__.py
--rw-r--r--   0 mike       (501) staff       (20)     1741 2019-10-16 22:03:06.000000 django-bom-1.98/bom/third_party_apis/base_api.py
--rw-r--r--   0 mike       (501) staff       (20)     6112 2019-10-16 22:03:06.000000 django-bom-1.98/bom/third_party_apis/google_drive.py
--rw-r--r--   0 mike       (501) staff       (20)     3836 2019-10-16 22:03:06.000000 django-bom-1.98/bom/third_party_apis/mouser.py
--rw-r--r--   0 mike       (501) staff       (20)      679 2019-10-19 22:45:00.000000 django-bom-1.98/bom/third_party_apis/test_apis.py
--rw-r--r--   0 mike       (501) staff       (20)     4270 2019-10-16 22:03:06.000000 django-bom-1.98/bom/urls.py
--rw-r--r--   0 mike       (501) staff       (20)      419 2019-10-16 22:03:06.000000 django-bom-1.98/bom/utils.py
--rw-r--r--   0 mike       (501) staff       (20)      336 2019-10-16 22:03:06.000000 django-bom-1.98/bom/validators.py
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2019-10-20 00:07:55.000000 django-bom-1.98/bom/views/
--rw-r--r--   0 mike       (501) staff       (20)        0 2019-10-16 22:03:06.000000 django-bom-1.98/bom/views/__init__.py
--rw-r--r--   0 mike       (501) staff       (20)     2332 2019-10-16 22:03:06.000000 django-bom-1.98/bom/views/json_views.py
--rw-r--r--   0 mike       (501) staff       (20)    58417 2019-10-19 23:23:09.000000 django-bom-1.98/bom/views/views.py
--rw-r--r--   0 mike       (501) staff       (20)      380 2019-10-16 22:03:06.000000 django-bom-1.98/bom/wsgi.py
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2019-10-20 00:07:55.000000 django-bom-1.98/django_bom.egg-info/
--rw-r--r--   0 mike       (501) staff       (20)     6845 2019-10-20 00:07:55.000000 django-bom-1.98/django_bom.egg-info/PKG-INFO
--rw-r--r--   0 mike       (501) staff       (20)     5129 2019-10-20 00:07:55.000000 django-bom-1.98/django_bom.egg-info/SOURCES.txt
--rw-r--r--   0 mike       (501) staff       (20)        1 2019-10-20 00:07:55.000000 django-bom-1.98/django_bom.egg-info/dependency_links.txt
--rw-r--r--   0 mike       (501) staff       (20)       94 2019-10-20 00:07:55.000000 django-bom-1.98/django_bom.egg-info/requires.txt
--rw-r--r--   0 mike       (501) staff       (20)        4 2019-10-20 00:07:55.000000 django-bom-1.98/django_bom.egg-info/top_level.txt
--rw-r--r--   0 mike       (501) staff       (20)       38 2019-10-20 00:07:55.000000 django-bom-1.98/setup.cfg
--rw-r--r--   0 mike       (501) staff       (20)     1306 2019-10-20 00:07:54.000000 django-bom-1.98/setup.py
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2019-10-20 19:33:43.000000 django-bom-1.99/
+-rw-r--r--   0 mike       (501) staff       (20)     1070 2019-10-16 22:03:06.000000 django-bom-1.99/LICENSE
+-rw-r--r--   0 mike       (501) staff       (20)      156 2019-10-16 22:03:06.000000 django-bom-1.99/MANIFEST.in
+-rw-r--r--   0 mike       (501) staff       (20)     6845 2019-10-20 19:33:43.000000 django-bom-1.99/PKG-INFO
+-rw-r--r--   0 mike       (501) staff       (20)     4889 2019-10-16 22:03:06.000000 django-bom-1.99/README.md
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2019-10-20 19:33:43.000000 django-bom-1.99/bom/
+-rw-r--r--   0 mike       (501) staff       (20)       41 2019-10-16 22:03:06.000000 django-bom-1.99/bom/__init__.py
+-rw-r--r--   0 mike       (501) staff       (20)     3754 2019-10-16 22:03:06.000000 django-bom-1.99/bom/admin.py
+-rw-r--r--   0 mike       (501) staff       (20)      147 2019-10-16 22:03:06.000000 django-bom-1.99/bom/apps.py
+-rw-r--r--   0 mike       (501) staff       (20)      309 2019-10-16 22:03:06.000000 django-bom-1.99/bom/context_processors.py
+-rw-r--r--   0 mike       (501) staff       (20)      346 2019-10-16 22:03:06.000000 django-bom-1.99/bom/convert.py
+-rw-r--r--   0 mike       (501) staff       (20)      645 2019-10-16 22:03:06.000000 django-bom-1.99/bom/decorators.py
+-rw-r--r--   0 mike       (501) staff       (20)    11675 2019-10-16 22:03:06.000000 django-bom-1.99/bom/forms.py
+-rw-r--r--   0 mike       (501) staff       (20)    12608 2019-10-19 23:14:11.000000 django-bom-1.99/bom/helpers.py
+-rw-r--r--   0 mike       (501) staff       (20)      883 2019-10-16 22:03:06.000000 django-bom-1.99/bom/local_settings.py
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2019-10-20 19:33:43.000000 django-bom-1.99/bom/migrations/
+-rw-r--r--   0 mike       (501) staff       (20)     7005 2019-10-16 22:03:06.000000 django-bom-1.99/bom/migrations/0001_initial.py
+-rw-r--r--   0 mike       (501) staff       (20)      753 2019-10-16 22:03:06.000000 django-bom-1.99/bom/migrations/0002_auto_20180908_2151.py
+-rw-r--r--   0 mike       (501) staff       (20)      414 2019-10-16 22:03:06.000000 django-bom-1.99/bom/migrations/0003_sellerpart_data_source.py
+-rw-r--r--   0 mike       (501) staff       (20)      432 2019-10-16 22:03:06.000000 django-bom-1.99/bom/migrations/0004_auto_20180911_0011.py
+-rw-r--r--   0 mike       (501) staff       (20)     2402 2019-10-16 22:03:06.000000 django-bom-1.99/bom/migrations/0005_auto_20181007_1934.py
+-rw-r--r--   0 mike       (501) staff       (20)     1249 2019-10-16 22:03:06.000000 django-bom-1.99/bom/migrations/0006_auto_20181007_1949.py
+-rw-r--r--   0 mike       (501) staff       (20)      569 2019-10-16 22:03:06.000000 django-bom-1.99/bom/migrations/0007_auto_20181009_0256.py
+-rw-r--r--   0 mike       (501) staff       (20)      570 2019-10-16 22:03:06.000000 django-bom-1.99/bom/migrations/0008_auto_20181030_0427.py
+-rw-r--r--   0 mike       (501) staff       (20)      404 2019-10-16 22:03:06.000000 django-bom-1.99/bom/migrations/0009_subpart_reference.py
+-rw-r--r--   0 mike       (501) staff       (20)      632 2019-10-16 22:03:06.000000 django-bom-1.99/bom/migrations/0010_auto_20181202_0733.py
+-rw-r--r--   0 mike       (501) staff       (20)      555 2019-10-16 22:03:06.000000 django-bom-1.99/bom/migrations/0011_auto_20181202_2113.py
+-rw-r--r--   0 mike       (501) staff       (20)     1511 2019-10-16 22:03:06.000000 django-bom-1.99/bom/migrations/0012_partchangehistory.py
+-rw-r--r--   0 mike       (501) staff       (20)      472 2019-10-16 22:03:06.000000 django-bom-1.99/bom/migrations/0013_auto_20190222_1631.py
+-rw-r--r--   0 mike       (501) staff       (20)      369 2019-10-16 22:03:06.000000 django-bom-1.99/bom/migrations/0014_auto_20190223_2353.py
+-rw-r--r--   0 mike       (501) staff       (20)     4673 2019-10-16 22:03:06.000000 django-bom-1.99/bom/migrations/0015_auto_20190303_1915.py
+-rw-r--r--   0 mike       (501) staff       (20)     1800 2019-10-16 22:03:06.000000 django-bom-1.99/bom/migrations/0016_auto_20190405_2308.py
+-rw-r--r--   0 mike       (501) staff       (20)      382 2019-10-16 22:03:06.000000 django-bom-1.99/bom/migrations/0017_auto_20190616_1912.py
+-rw-r--r--   0 mike       (501) staff       (20)      688 2019-10-16 22:03:06.000000 django-bom-1.99/bom/migrations/0018_auto_20190616_2143.py
+-rw-r--r--   0 mike       (501) staff       (20)     1590 2019-10-16 22:03:06.000000 django-bom-1.99/bom/migrations/0019_auto_20190624_1246.py
+-rw-r--r--   0 mike       (501) staff       (20)     1147 2019-10-16 22:03:06.000000 django-bom-1.99/bom/migrations/0020_auto_20190627_0207.py
+-rw-r--r--   0 mike       (501) staff       (20)      625 2019-10-16 22:03:06.000000 django-bom-1.99/bom/migrations/0021_auto_20190627_0428.py
+-rw-r--r--   0 mike       (501) staff       (20)     1025 2019-10-16 22:03:06.000000 django-bom-1.99/bom/migrations/0022_auto_20190811_2140.py
+-rw-r--r--   0 mike       (501) staff       (20)        0 2019-10-16 22:03:06.000000 django-bom-1.99/bom/migrations/__init__.py
+-rw-r--r--   0 mike       (501) staff       (20)    16340 2019-10-16 22:03:06.000000 django-bom-1.99/bom/models.py
+-rw-r--r--   0 mike       (501) staff       (20)     6440 2019-10-19 22:02:03.000000 django-bom-1.99/bom/settings.py
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2019-10-20 19:33:43.000000 django-bom-1.99/bom/static/
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2019-10-20 19:33:43.000000 django-bom-1.99/bom/static/bom/
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2019-10-20 19:33:43.000000 django-bom-1.99/bom/static/bom/css/
+-rwxr-xr-x   0 mike       (501) staff       (20)      652 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/css/jquery.treetable.css
+-rw-r--r--   0 mike       (501) staff       (20)   141841 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/css/materialize.min.css
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2019-10-20 19:33:43.000000 django-bom-1.99/bom/static/bom/img/
+-rw-r--r--   0 mike       (501) staff       (20)      127 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/img/_ionicons_svg_md-arrow-dropdown.svg
+-rw-r--r--   0 mike       (501) staff       (20)      127 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/img/_ionicons_svg_md-arrow-dropright.svg
+-rw-r--r--   0 mike       (501) staff       (20)     1150 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/img/favicon.ico
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2019-10-20 19:33:43.000000 django-bom-1.99/bom/static/bom/img/google/
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2019-10-20 19:33:43.000000 django-bom-1.99/bom/static/bom/img/google/web/
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2019-10-20 19:33:43.000000 django-bom-1.99/bom/static/bom/img/google/web/1x/
+-rw-r--r--   0 mike       (501) staff       (20)     2308 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/img/google/web/1x/btn_google_signin_dark_disabled_web.png
+-rw-r--r--   0 mike       (501) staff       (20)     4185 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/img/google/web/1x/btn_google_signin_dark_focus_web.png
+-rw-r--r--   0 mike       (501) staff       (20)     3983 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/img/google/web/1x/btn_google_signin_dark_normal_web.png
+-rw-r--r--   0 mike       (501) staff       (20)     4236 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/img/google/web/1x/btn_google_signin_dark_pressed_web.png
+-rw-r--r--   0 mike       (501) staff       (20)     2308 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/img/google/web/1x/btn_google_signin_light_disabled_web.png
+-rw-r--r--   0 mike       (501) staff       (20)     4328 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/img/google/web/1x/btn_google_signin_light_focus_web.png
+-rw-r--r--   0 mike       (501) staff       (20)     4099 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/img/google/web/1x/btn_google_signin_light_normal_web.png
+-rw-r--r--   0 mike       (501) staff       (20)     4135 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/img/google/web/1x/btn_google_signin_light_pressed_web.png
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2019-10-20 19:33:43.000000 django-bom-1.99/bom/static/bom/img/google/web/2x/
+-rw-r--r--   0 mike       (501) staff       (20)     4897 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/img/google/web/2x/btn_google_signin_dark_disabled_web@2x.png
+-rw-r--r--   0 mike       (501) staff       (20)     8513 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/img/google/web/2x/btn_google_signin_dark_focus_web@2x.png
+-rw-r--r--   0 mike       (501) staff       (20)     8001 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/img/google/web/2x/btn_google_signin_dark_normal_web@2x.png
+-rw-r--r--   0 mike       (501) staff       (20)     8483 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/img/google/web/2x/btn_google_signin_dark_pressed_web@2x.png
+-rw-r--r--   0 mike       (501) staff       (20)     4897 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/img/google/web/2x/btn_google_signin_light_disabled_web@2x.png
+-rw-r--r--   0 mike       (501) staff       (20)     8664 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/img/google/web/2x/btn_google_signin_light_focus_web@2x.png
+-rw-r--r--   0 mike       (501) staff       (20)     8055 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/img/google/web/2x/btn_google_signin_light_normal_web@2x.png
+-rw-r--r--   0 mike       (501) staff       (20)     8265 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/img/google/web/2x/btn_google_signin_light_pressed_web@2x.png
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2019-10-20 19:33:43.000000 django-bom-1.99/bom/static/bom/img/google/web/vector/
+-rw-r--r--   0 mike       (501) staff       (20)    20286 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/img/google/web/vector/btn_google_dark_disabled_ios.eps
+-rw-r--r--   0 mike       (501) staff       (20)     1996 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/img/google/web/vector/btn_google_dark_disabled_ios.svg
+-rw-r--r--   0 mike       (501) staff       (20)    94048 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/img/google/web/vector/btn_google_dark_focus_ios.eps
+-rw-r--r--   0 mike       (501) staff       (20)     4917 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/img/google/web/vector/btn_google_dark_focus_ios.svg
+-rw-r--r--   0 mike       (501) staff       (20)    26465 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/img/google/web/vector/btn_google_dark_normal_ios.eps
+-rw-r--r--   0 mike       (501) staff       (20)     4779 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/img/google/web/vector/btn_google_dark_normal_ios.svg
+-rw-r--r--   0 mike       (501) staff       (20)    26484 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/img/google/web/vector/btn_google_dark_pressed_ios.eps
+-rw-r--r--   0 mike       (501) staff       (20)     4781 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/img/google/web/vector/btn_google_dark_pressed_ios.svg
+-rw-r--r--   0 mike       (501) staff       (20)    20286 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/img/google/web/vector/btn_google_light_disabled_ios.eps
+-rw-r--r--   0 mike       (501) staff       (20)     1998 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/img/google/web/vector/btn_google_light_disabled_ios.svg
+-rw-r--r--   0 mike       (501) staff       (20)    93663 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/img/google/web/vector/btn_google_light_focus_ios.eps
+-rw-r--r--   0 mike       (501) staff       (20)     4496 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/img/google/web/vector/btn_google_light_focus_ios.svg
+-rw-r--r--   0 mike       (501) staff       (20)    26080 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/img/google/web/vector/btn_google_light_normal_ios.eps
+-rw-r--r--   0 mike       (501) staff       (20)     4358 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/img/google/web/vector/btn_google_light_normal_ios.svg
+-rw-r--r--   0 mike       (501) staff       (20)    26107 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/img/google/web/vector/btn_google_light_pressed_ios.eps
+-rw-r--r--   0 mike       (501) staff       (20)     4360 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/img/google/web/vector/btn_google_light_pressed_ios.svg
+-rw-r--r--   0 mike       (501) staff       (20)     1102 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/img/google_drive_logo.svg
+-rw-r--r--   0 mike       (501) staff       (20)    42071 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/img/indabom.png
+-rw-r--r--   0 mike       (501) staff       (20)     1351 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/img/octopart_blue.svg
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2019-10-20 19:33:43.000000 django-bom-1.99/bom/static/bom/js/
+-rw-r--r--   0 mike       (501) staff       (20)     1271 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/js/jquery.ba-floatingscrollbar.min.js
+-rwxr-xr-x   0 mike       (501) staff       (20)    16611 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/js/jquery.treetable.js
+-rw-r--r--   0 mike       (501) staff       (20)   181114 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/js/materialize.min.js
+-rw-r--r--   0 mike       (501) staff       (20)     2765 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/style.css
+-rw-r--r--   0 mike       (501) staff       (20)    24032 2019-10-16 22:03:06.000000 django-bom-1.99/bom/static/bom/treetable-theme.css
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2019-10-20 19:33:43.000000 django-bom-1.99/bom/templates/
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2019-10-20 19:33:43.000000 django-bom-1.99/bom/templates/bom/
+-rw-r--r--   0 mike       (501) staff       (20)     2344 2019-10-16 22:03:06.000000 django-bom-1.99/bom/templates/bom/add-manufacturer-part.html
+-rw-r--r--   0 mike       (501) staff       (20)     3271 2019-10-16 22:03:06.000000 django-bom-1.99/bom/templates/bom/add-sellerpart.html
+-rw-r--r--   0 mike       (501) staff       (20)     5947 2019-10-16 22:03:06.000000 django-bom-1.99/bom/templates/bom/base.html
+-rw-r--r--   0 mike       (501) staff       (20)     1004 2019-10-16 22:03:06.000000 django-bom-1.99/bom/templates/bom/bom-action-btn.html
+-rw-r--r--   0 mike       (501) staff       (20)     1030 2019-10-16 22:03:06.000000 django-bom-1.99/bom/templates/bom/bom-form.html
+-rw-r--r--   0 mike       (501) staff       (20)      296 2019-10-16 22:03:06.000000 django-bom-1.99/bom/templates/bom/bom-signup.html
+-rw-r--r--   0 mike       (501) staff       (20)     2813 2019-10-20 00:07:18.000000 django-bom-1.99/bom/templates/bom/create-part.html
+-rw-r--r--   0 mike       (501) staff       (20)     4586 2019-10-16 22:03:06.000000 django-bom-1.99/bom/templates/bom/dashboard.html
+-rw-r--r--   0 mike       (501) staff       (20)     2299 2019-10-16 22:03:06.000000 django-bom-1.99/bom/templates/bom/edit-manufacturer-part.html
+-rw-r--r--   0 mike       (501) staff       (20)     2190 2019-10-16 22:03:06.000000 django-bom-1.99/bom/templates/bom/edit-part.html
+-rw-r--r--   0 mike       (501) staff       (20)      700 2019-10-16 22:03:06.000000 django-bom-1.99/bom/templates/bom/error.html
+-rw-r--r--   0 mike       (501) staff       (20)    32522 2019-10-16 22:03:06.000000 django-bom-1.99/bom/templates/bom/part-info.html
+-rw-r--r--   0 mike       (501) staff       (20)    10404 2019-10-16 22:03:06.000000 django-bom-1.99/bom/templates/bom/part-rev-manage-bom.html
+-rw-r--r--   0 mike       (501) staff       (20)     1323 2019-10-16 22:03:06.000000 django-bom-1.99/bom/templates/bom/part-revision-edit.html
+-rw-r--r--   0 mike       (501) staff       (20)     1960 2019-10-16 22:03:06.000000 django-bom-1.99/bom/templates/bom/part-revision-new.html
+-rw-r--r--   0 mike       (501) staff       (20)     1826 2019-10-16 22:03:06.000000 django-bom-1.99/bom/templates/bom/part-revision-release.html
+-rw-r--r--   0 mike       (501) staff       (20)     4444 2019-10-16 22:03:06.000000 django-bom-1.99/bom/templates/bom/settings.html
+-rw-r--r--   0 mike       (501) staff       (20)     1945 2019-10-16 22:03:06.000000 django-bom-1.99/bom/templates/bom/upload-parts.html
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2019-10-20 19:33:43.000000 django-bom-1.99/bom/templates/registration/
+-rw-r--r--   0 mike       (501) staff       (20)     1100 2019-10-16 22:03:06.000000 django-bom-1.99/bom/templates/registration/login.html
+-rw-r--r--   0 mike       (501) staff       (20)    25968 2019-10-19 23:24:02.000000 django-bom-1.99/bom/tests.py
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2019-10-20 19:33:43.000000 django-bom-1.99/bom/third_party_apis/
+-rw-r--r--   0 mike       (501) staff       (20)        0 2019-10-16 22:03:06.000000 django-bom-1.99/bom/third_party_apis/__init__.py
+-rw-r--r--   0 mike       (501) staff       (20)     1741 2019-10-16 22:03:06.000000 django-bom-1.99/bom/third_party_apis/base_api.py
+-rw-r--r--   0 mike       (501) staff       (20)     6112 2019-10-16 22:03:06.000000 django-bom-1.99/bom/third_party_apis/google_drive.py
+-rw-r--r--   0 mike       (501) staff       (20)     3836 2019-10-16 22:03:06.000000 django-bom-1.99/bom/third_party_apis/mouser.py
+-rw-r--r--   0 mike       (501) staff       (20)      679 2019-10-19 22:45:00.000000 django-bom-1.99/bom/third_party_apis/test_apis.py
+-rw-r--r--   0 mike       (501) staff       (20)     4270 2019-10-16 22:03:06.000000 django-bom-1.99/bom/urls.py
+-rw-r--r--   0 mike       (501) staff       (20)      419 2019-10-16 22:03:06.000000 django-bom-1.99/bom/utils.py
+-rw-r--r--   0 mike       (501) staff       (20)      336 2019-10-16 22:03:06.000000 django-bom-1.99/bom/validators.py
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2019-10-20 19:33:43.000000 django-bom-1.99/bom/views/
+-rw-r--r--   0 mike       (501) staff       (20)        0 2019-10-16 22:03:06.000000 django-bom-1.99/bom/views/__init__.py
+-rw-r--r--   0 mike       (501) staff       (20)     2332 2019-10-16 22:03:06.000000 django-bom-1.99/bom/views/json_views.py
+-rw-r--r--   0 mike       (501) staff       (20)    58677 2019-10-20 19:30:59.000000 django-bom-1.99/bom/views/views.py
+-rw-r--r--   0 mike       (501) staff       (20)      380 2019-10-16 22:03:06.000000 django-bom-1.99/bom/wsgi.py
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2019-10-20 19:33:43.000000 django-bom-1.99/django_bom.egg-info/
+-rw-r--r--   0 mike       (501) staff       (20)     6845 2019-10-20 19:33:42.000000 django-bom-1.99/django_bom.egg-info/PKG-INFO
+-rw-r--r--   0 mike       (501) staff       (20)     5129 2019-10-20 19:33:42.000000 django-bom-1.99/django_bom.egg-info/SOURCES.txt
+-rw-r--r--   0 mike       (501) staff       (20)        1 2019-10-20 19:33:42.000000 django-bom-1.99/django_bom.egg-info/dependency_links.txt
+-rw-r--r--   0 mike       (501) staff       (20)       94 2019-10-20 19:33:42.000000 django-bom-1.99/django_bom.egg-info/requires.txt
+-rw-r--r--   0 mike       (501) staff       (20)        4 2019-10-20 19:33:42.000000 django-bom-1.99/django_bom.egg-info/top_level.txt
+-rw-r--r--   0 mike       (501) staff       (20)       38 2019-10-20 19:33:43.000000 django-bom-1.99/setup.cfg
+-rw-r--r--   0 mike       (501) staff       (20)     1306 2019-10-20 19:33:42.000000 django-bom-1.99/setup.py
```

### Comparing `django-bom-1.98/LICENSE` & `django-bom-1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/PKG-INFO` & `django-bom-1.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-bom
-Version: 1.98
+Version: 1.99
 Summary: A simple Django app to manage a bill of materials.
 Home-page: https://www.indabom.com/
 Author: Mike Kasparian
 Author-email: mpkasp@gmail.com
 License: MIT License
 Description: # BOM
```

### Comparing `django-bom-1.98/README.md` & `django-bom-1.99/README.md`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/admin.py` & `django-bom-1.99/bom/admin.py`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/decorators.py` & `django-bom-1.99/bom/decorators.py`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/forms.py` & `django-bom-1.99/bom/forms.py`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/helpers.py` & `django-bom-1.99/bom/helpers.py`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/local_settings.py` & `django-bom-1.99/bom/local_settings.py`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/migrations/0001_initial.py` & `django-bom-1.99/bom/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/migrations/0002_auto_20180908_2151.py` & `django-bom-1.99/bom/migrations/0002_auto_20180908_2151.py`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/migrations/0005_auto_20181007_1934.py` & `django-bom-1.99/bom/migrations/0005_auto_20181007_1934.py`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/migrations/0006_auto_20181007_1949.py` & `django-bom-1.99/bom/migrations/0006_auto_20181007_1949.py`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/migrations/0007_auto_20181009_0256.py` & `django-bom-1.99/bom/migrations/0007_auto_20181009_0256.py`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/migrations/0008_auto_20181030_0427.py` & `django-bom-1.99/bom/migrations/0008_auto_20181030_0427.py`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/migrations/0010_auto_20181202_0733.py` & `django-bom-1.99/bom/migrations/0010_auto_20181202_0733.py`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/migrations/0011_auto_20181202_2113.py` & `django-bom-1.99/bom/migrations/0011_auto_20181202_2113.py`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/migrations/0012_partchangehistory.py` & `django-bom-1.99/bom/migrations/0012_partchangehistory.py`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/migrations/0015_auto_20190303_1915.py` & `django-bom-1.99/bom/migrations/0015_auto_20190303_1915.py`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/migrations/0016_auto_20190405_2308.py` & `django-bom-1.99/bom/migrations/0016_auto_20190405_2308.py`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/migrations/0018_auto_20190616_2143.py` & `django-bom-1.99/bom/migrations/0018_auto_20190616_2143.py`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/migrations/0019_auto_20190624_1246.py` & `django-bom-1.99/bom/migrations/0019_auto_20190624_1246.py`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/migrations/0020_auto_20190627_0207.py` & `django-bom-1.99/bom/migrations/0020_auto_20190627_0207.py`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/migrations/0021_auto_20190627_0428.py` & `django-bom-1.99/bom/migrations/0021_auto_20190627_0428.py`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/migrations/0022_auto_20190811_2140.py` & `django-bom-1.99/bom/migrations/0022_auto_20190811_2140.py`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/models.py` & `django-bom-1.99/bom/models.py`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/settings.py` & `django-bom-1.99/bom/settings.py`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/css/jquery.treetable.css` & `django-bom-1.99/bom/static/bom/css/jquery.treetable.css`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/css/materialize.min.css` & `django-bom-1.99/bom/static/bom/css/materialize.min.css`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/img/favicon.ico` & `django-bom-1.99/bom/static/bom/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/img/google/web/1x/btn_google_signin_dark_disabled_web.png` & `django-bom-1.99/bom/static/bom/img/google/web/1x/btn_google_signin_dark_disabled_web.png`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/img/google/web/1x/btn_google_signin_dark_focus_web.png` & `django-bom-1.99/bom/static/bom/img/google/web/1x/btn_google_signin_dark_focus_web.png`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/img/google/web/1x/btn_google_signin_dark_normal_web.png` & `django-bom-1.99/bom/static/bom/img/google/web/1x/btn_google_signin_dark_normal_web.png`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/img/google/web/1x/btn_google_signin_dark_pressed_web.png` & `django-bom-1.99/bom/static/bom/img/google/web/1x/btn_google_signin_dark_pressed_web.png`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/img/google/web/1x/btn_google_signin_light_disabled_web.png` & `django-bom-1.99/bom/static/bom/img/google/web/1x/btn_google_signin_light_disabled_web.png`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/img/google/web/1x/btn_google_signin_light_focus_web.png` & `django-bom-1.99/bom/static/bom/img/google/web/1x/btn_google_signin_light_focus_web.png`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/img/google/web/1x/btn_google_signin_light_normal_web.png` & `django-bom-1.99/bom/static/bom/img/google/web/1x/btn_google_signin_light_normal_web.png`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/img/google/web/1x/btn_google_signin_light_pressed_web.png` & `django-bom-1.99/bom/static/bom/img/google/web/1x/btn_google_signin_light_pressed_web.png`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/img/google/web/2x/btn_google_signin_dark_disabled_web@2x.png` & `django-bom-1.99/bom/static/bom/img/google/web/2x/btn_google_signin_dark_disabled_web@2x.png`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/img/google/web/2x/btn_google_signin_dark_focus_web@2x.png` & `django-bom-1.99/bom/static/bom/img/google/web/2x/btn_google_signin_dark_focus_web@2x.png`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/img/google/web/2x/btn_google_signin_dark_normal_web@2x.png` & `django-bom-1.99/bom/static/bom/img/google/web/2x/btn_google_signin_dark_normal_web@2x.png`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/img/google/web/2x/btn_google_signin_dark_pressed_web@2x.png` & `django-bom-1.99/bom/static/bom/img/google/web/2x/btn_google_signin_dark_pressed_web@2x.png`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/img/google/web/2x/btn_google_signin_light_disabled_web@2x.png` & `django-bom-1.99/bom/static/bom/img/google/web/2x/btn_google_signin_light_disabled_web@2x.png`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/img/google/web/2x/btn_google_signin_light_focus_web@2x.png` & `django-bom-1.99/bom/static/bom/img/google/web/2x/btn_google_signin_light_focus_web@2x.png`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/img/google/web/2x/btn_google_signin_light_normal_web@2x.png` & `django-bom-1.99/bom/static/bom/img/google/web/2x/btn_google_signin_light_normal_web@2x.png`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/img/google/web/2x/btn_google_signin_light_pressed_web@2x.png` & `django-bom-1.99/bom/static/bom/img/google/web/2x/btn_google_signin_light_pressed_web@2x.png`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/img/google/web/vector/btn_google_dark_disabled_ios.eps` & `django-bom-1.99/bom/static/bom/img/google/web/vector/btn_google_dark_disabled_ios.eps`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/img/google/web/vector/btn_google_dark_disabled_ios.svg` & `django-bom-1.99/bom/static/bom/img/google/web/vector/btn_google_dark_disabled_ios.svg`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/img/google/web/vector/btn_google_dark_focus_ios.eps` & `django-bom-1.99/bom/static/bom/img/google/web/vector/btn_google_dark_focus_ios.eps`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/img/google/web/vector/btn_google_dark_focus_ios.svg` & `django-bom-1.99/bom/static/bom/img/google/web/vector/btn_google_dark_focus_ios.svg`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/img/google/web/vector/btn_google_dark_normal_ios.eps` & `django-bom-1.99/bom/static/bom/img/google/web/vector/btn_google_dark_normal_ios.eps`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/img/google/web/vector/btn_google_dark_normal_ios.svg` & `django-bom-1.99/bom/static/bom/img/google/web/vector/btn_google_dark_normal_ios.svg`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/img/google/web/vector/btn_google_dark_pressed_ios.eps` & `django-bom-1.99/bom/static/bom/img/google/web/vector/btn_google_dark_pressed_ios.eps`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/img/google/web/vector/btn_google_dark_pressed_ios.svg` & `django-bom-1.99/bom/static/bom/img/google/web/vector/btn_google_dark_pressed_ios.svg`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/img/google/web/vector/btn_google_light_disabled_ios.eps` & `django-bom-1.99/bom/static/bom/img/google/web/vector/btn_google_light_disabled_ios.eps`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/img/google/web/vector/btn_google_light_disabled_ios.svg` & `django-bom-1.99/bom/static/bom/img/google/web/vector/btn_google_light_disabled_ios.svg`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/img/google/web/vector/btn_google_light_focus_ios.eps` & `django-bom-1.99/bom/static/bom/img/google/web/vector/btn_google_light_focus_ios.eps`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/img/google/web/vector/btn_google_light_focus_ios.svg` & `django-bom-1.99/bom/static/bom/img/google/web/vector/btn_google_light_focus_ios.svg`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/img/google/web/vector/btn_google_light_normal_ios.eps` & `django-bom-1.99/bom/static/bom/img/google/web/vector/btn_google_light_normal_ios.eps`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/img/google/web/vector/btn_google_light_normal_ios.svg` & `django-bom-1.99/bom/static/bom/img/google/web/vector/btn_google_light_normal_ios.svg`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/img/google/web/vector/btn_google_light_pressed_ios.eps` & `django-bom-1.99/bom/static/bom/img/google/web/vector/btn_google_light_pressed_ios.eps`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/img/google/web/vector/btn_google_light_pressed_ios.svg` & `django-bom-1.99/bom/static/bom/img/google/web/vector/btn_google_light_pressed_ios.svg`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/img/google_drive_logo.svg` & `django-bom-1.99/bom/static/bom/img/google_drive_logo.svg`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/img/indabom.png` & `django-bom-1.99/bom/static/bom/img/indabom.png`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/img/octopart_blue.svg` & `django-bom-1.99/bom/static/bom/img/octopart_blue.svg`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/js/jquery.ba-floatingscrollbar.min.js` & `django-bom-1.99/bom/static/bom/js/jquery.ba-floatingscrollbar.min.js`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/js/jquery.treetable.js` & `django-bom-1.99/bom/static/bom/js/jquery.treetable.js`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/js/materialize.min.js` & `django-bom-1.99/bom/static/bom/js/materialize.min.js`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/style.css` & `django-bom-1.99/bom/static/bom/style.css`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/static/bom/treetable-theme.css` & `django-bom-1.99/bom/static/bom/treetable-theme.css`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/templates/bom/add-manufacturer-part.html` & `django-bom-1.99/bom/templates/bom/add-manufacturer-part.html`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/templates/bom/add-sellerpart.html` & `django-bom-1.99/bom/templates/bom/add-sellerpart.html`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/templates/bom/base.html` & `django-bom-1.99/bom/templates/bom/base.html`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/templates/bom/bom-action-btn.html` & `django-bom-1.99/bom/templates/bom/bom-action-btn.html`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/templates/bom/bom-form.html` & `django-bom-1.99/bom/templates/bom/bom-form.html`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/templates/bom/create-part.html` & `django-bom-1.99/bom/templates/bom/create-part.html`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/templates/bom/dashboard.html` & `django-bom-1.99/bom/templates/bom/dashboard.html`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/templates/bom/edit-manufacturer-part.html` & `django-bom-1.99/bom/templates/bom/edit-manufacturer-part.html`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/templates/bom/edit-part.html` & `django-bom-1.99/bom/templates/bom/edit-part.html`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/templates/bom/error.html` & `django-bom-1.99/bom/templates/bom/error.html`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/templates/bom/part-info.html` & `django-bom-1.99/bom/templates/bom/part-info.html`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/templates/bom/part-rev-manage-bom.html` & `django-bom-1.99/bom/templates/bom/part-rev-manage-bom.html`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/templates/bom/part-revision-edit.html` & `django-bom-1.99/bom/templates/bom/part-revision-edit.html`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/templates/bom/part-revision-new.html` & `django-bom-1.99/bom/templates/bom/part-revision-new.html`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/templates/bom/part-revision-release.html` & `django-bom-1.99/bom/templates/bom/part-revision-release.html`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/templates/bom/settings.html` & `django-bom-1.99/bom/templates/bom/settings.html`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/templates/bom/upload-parts.html` & `django-bom-1.99/bom/templates/bom/upload-parts.html`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/templates/registration/login.html` & `django-bom-1.99/bom/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/tests.py` & `django-bom-1.99/bom/tests.py`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/third_party_apis/base_api.py` & `django-bom-1.99/bom/third_party_apis/base_api.py`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/third_party_apis/google_drive.py` & `django-bom-1.99/bom/third_party_apis/google_drive.py`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/third_party_apis/mouser.py` & `django-bom-1.99/bom/third_party_apis/mouser.py`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/third_party_apis/test_apis.py` & `django-bom-1.99/bom/third_party_apis/test_apis.py`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/urls.py` & `django-bom-1.99/bom/urls.py`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/views/json_views.py` & `django-bom-1.99/bom/views/json_views.py`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/bom/views/views.py` & `django-bom-1.99/bom/views/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import logging
 
 from django.contrib import messages
 from django.contrib.auth.decorators import login_required
 from django.core.exceptions import ObjectDoesNotExist
 from django.core.cache import cache
 from django.core.paginator import Paginator, EmptyPage, PageNotAnInteger
+from django.db import IntegrityError
 from django.db.models import Q
 from django.http import HttpResponse, HttpResponseRedirect
 from django.shortcuts import get_object_or_404
 from django.template.response import TemplateResponse
 from django.urls import reverse
 from django.utils.encoding import smart_str
 
@@ -763,37 +764,41 @@
     organization = profile.organization
     title = 'Create New Part'
 
     if request.method == 'POST':
         part_form = PartForm(request.POST)
         manufacturer_form = ManufacturerForm(request.POST)
         manufacturer_part_form = ManufacturerPartForm(request.POST, organization=organization)
+        part_revision_form = PartRevisionForm(request.POST)
         if part_form.is_valid() and manufacturer_form.is_valid() and manufacturer_part_form.is_valid():
             mpn = manufacturer_part_form.cleaned_data['manufacturer_part_number']
             old_manufacturer = manufacturer_part_form.cleaned_data['manufacturer']
             new_manufacturer_name = manufacturer_form.cleaned_data['name']
 
             manufacturer = None
             if mpn:
                 if old_manufacturer and new_manufacturer_name == '':
                     manufacturer = old_manufacturer
                 elif new_manufacturer_name != '' and not old_manufacturer:
                     manufacturer, created = Manufacturer.objects.get_or_create(name=new_manufacturer_name,
                                                                                organization=organization)
                 else:
-                    part_revision_form = PartRevisionForm(request.POST)
                     messages.error(request, "Either create a new manufacturer, or select an existing manufacturer.")
                     return TemplateResponse(request, 'bom/create-part.html', locals())
             elif old_manufacturer or new_manufacturer_name != '':
                 messages.warning(request,
                                  "No manufacturer was selected or created, no manufacturer part number was assigned.")
 
             new_part = part_form.save(commit=False)
             new_part.organization = organization
-            new_part.save(no_part_revision=True)
+            try:
+                new_part.save(no_part_revision=True)
+            except IntegrityError:
+                messages.error(request, "Error! Already created a part with that part number.")
+                return TemplateResponse(request, 'bom/create-part.html', locals())
 
             updated_data = request.POST.copy()
             updated_data.update({'part': new_part.id})
             part_revision_form = PartRevisionForm(updated_data)
             if part_revision_form.is_valid():
                 pr = part_revision_form.save(commit=False)
                 pr.part = new_part
```

### Comparing `django-bom-1.98/django_bom.egg-info/PKG-INFO` & `django-bom-1.99/django_bom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-bom
-Version: 1.98
+Version: 1.99
 Summary: A simple Django app to manage a bill of materials.
 Home-page: https://www.indabom.com/
 Author: Mike Kasparian
 Author-email: mpkasp@gmail.com
 License: MIT License
 Description: # BOM
```

### Comparing `django-bom-1.98/django_bom.egg-info/SOURCES.txt` & `django-bom-1.99/django_bom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-bom-1.98/setup.py` & `django-bom-1.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-bom',
-    version='1.98',
+    version='1.99',
     packages=find_packages(),
     include_package_data=True,
     license='MIT License',
     description='A simple Django app to manage a bill of materials.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://www.indabom.com/',
```

