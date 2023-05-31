# Comparing `tmp/django-admin-datta-1.0.7.tar.gz` & `tmp/django-admin-datta-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-admin-datta-1.0.7.tar", last modified: Tue Feb 28 05:17:40 2023, max compression
+gzip compressed data, was "django-admin-datta-1.0.8.tar", last modified: Wed May 31 07:35:09 2023, max compression
```

## Comparing `django-admin-datta-1.0.7.tar` & `django-admin-datta-1.0.8.tar`

### file list

```diff
@@ -1,235 +1,248 @@
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.965947 django-admin-datta-1.0.7/
--rw-rw-rw-   0        0        0     1113 2022-09-27 05:30:21.000000 django-admin-datta-1.0.7/LICENSE.md
--rw-rw-rw-   0        0        0      144 2023-02-09 15:44:00.000000 django-admin-datta-1.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     7309 2023-02-28 05:17:40.964949 django-admin-datta-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     6214 2023-02-27 09:21:52.000000 django-admin-datta-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.204891 django-admin-datta-1.0.7/admin_datta/
--rw-rw-rw-   0        0        0       78 2022-09-27 05:30:21.000000 django-admin-datta-1.0.7/admin_datta/__init__.py
--rw-rw-rw-   0        0        0       78 2022-09-27 05:30:21.000000 django-admin-datta-1.0.7/admin_datta/admin.py
--rw-rw-rw-   0        0        0      235 2023-02-09 15:45:05.000000 django-admin-datta-1.0.7/admin_datta/apps.py
--rw-rw-rw-   0        0        0     2601 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/forms.py
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.205911 django-admin-datta-1.0.7/admin_datta/static/
--rw-rw-rw-   0        0        0        0 2022-09-27 05:30:21.000000 django-admin-datta-1.0.7/admin_datta/static/.gitkeep
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.139132 django-admin-datta-1.0.7/admin_datta/static/assets/
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.223915 django-admin-datta-1.0.7/admin_datta/static/assets/css/
--rw-rw-rw-   0        0        0     3610 2023-02-28 04:48:58.000000 django-admin-datta-1.0.7/admin_datta/static/assets/css/dark.css
--rw-rw-rw-   0        0        0     9593 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/css/forms.css
--rw-rw-rw-   0        0        0   325947 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/css/style.css
--rw-rw-rw-   0        0        0    12553 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/css/widgets.css
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.111810 django-admin-datta-1.0.7/admin_datta/static/assets/fonts/
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.225914 django-admin-datta-1.0.7/admin_datta/static/assets/fonts/datta/
--rw-rw-rw-   0        0        0     1623 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/fonts/datta/datta-icon.css
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.240742 django-admin-datta-1.0.7/admin_datta/static/assets/fonts/datta/fonts/
--rw-rw-rw-   0        0        0     2548 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/fonts/datta/fonts/pct.eot
--rw-rw-rw-   0        0        0     2553 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/fonts/datta/fonts/pct.svg
--rw-rw-rw-   0        0        0     2400 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/fonts/datta/fonts/pct.ttf
--rw-rw-rw-   0        0        0     1544 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/fonts/datta/fonts/pct.woff
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.110812 django-admin-datta-1.0.7/admin_datta/static/assets/fonts/feather/
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.241724 django-admin-datta-1.0.7/admin_datta/static/assets/fonts/feather/css/
--rw-rw-rw-   0        0        0    12312 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/fonts/feather/css/feather.css
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.253440 django-admin-datta-1.0.7/admin_datta/static/assets/fonts/feather/fonts/
--rw-rw-rw-   0        0        0    55828 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/fonts/feather/fonts/feather.eot
--rw-rw-rw-   0        0        0   192354 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/fonts/feather/fonts/feather.svg
--rw-rw-rw-   0        0        0    55664 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/fonts/feather/fonts/feather.ttf
--rw-rw-rw-   0        0        0    26432 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/fonts/feather/fonts/feather.woff
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.112811 django-admin-datta-1.0.7/admin_datta/static/assets/fonts/fontawesome/
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.256418 django-admin-datta-1.0.7/admin_datta/static/assets/fonts/fontawesome/css/
--rw-rw-rw-   0        0        0    41069 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/fonts/fontawesome/css/fontawesome-all.min.css
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.322557 django-admin-datta-1.0.7/admin_datta/static/assets/fonts/fontawesome/webfonts/
--rw-rw-rw-   0        0        0   111620 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-brands-400.eot
--rw-rw-rw-   0        0        0   600938 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-brands-400.svg
--rw-rw-rw-   0        0        0   111384 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-brands-400.ttf
--rw-rw-rw-   0        0        0    71560 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-brands-400.woff
--rw-rw-rw-   0        0        0    61336 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-brands-400.woff2
--rw-rw-rw-   0        0        0    31272 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-regular-400.eot
--rw-rw-rw-   0        0        0   105078 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-regular-400.svg
--rw-rw-rw-   0        0        0    31044 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-regular-400.ttf
--rw-rw-rw-   0        0        0    14724 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-regular-400.woff
--rw-rw-rw-   0        0        0    12188 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-regular-400.woff2
--rw-rw-rw-   0        0        0   133140 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.eot
--rw-rw-rw-   0        0        0   490291 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.svg
--rw-rw-rw-   0        0        0   132920 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.ttf
--rw-rw-rw-   0        0        0    63836 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.woff
--rw-rw-rw-   0        0        0    50372 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.woff2
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.357762 django-admin-datta-1.0.7/admin_datta/static/assets/images/
--rw-rw-rw-   0        0        0    45568 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/images/Thumbs.db
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.374875 django-admin-datta-1.0.7/admin_datta/static/assets/images/browser/
--rw-rw-rw-   0        0        0    23040 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/images/browser/Thumbs.db
--rw-rw-rw-   0        0        0     3822 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/images/browser/chrome.png
--rw-rw-rw-   0        0        0     4809 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/images/browser/firefox.png
--rw-rw-rw-   0        0        0     4359 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/images/browser/ie.png
--rw-rw-rw-   0        0        0     3379 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/images/browser/opera.png
--rw-rw-rw-   0        0        0     4915 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/images/browser/safari.png
--rw-rw-rw-   0        0        0     1150 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/images/favicon.ico
--rw-rw-rw-   0        0        0     2091 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/images/logo-dark.png
--rw-rw-rw-   0        0        0     1529 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/images/logo-thumb.png
--rw-rw-rw-   0        0        0     2131 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/images/logo.png
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.394907 django-admin-datta-1.0.7/admin_datta/static/assets/images/slider/
--rw-rw-rw-   0        0        0    31417 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/images/slider/img-slide-1.jpg
--rw-rw-rw-   0        0        0    66369 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/images/slider/img-slide-2.jpg
--rw-rw-rw-   0        0        0    22071 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/images/slider/img-slide-3.jpg
--rw-rw-rw-   0        0        0    21820 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/images/slider/img-slide-4.jpg
--rw-rw-rw-   0        0        0    33652 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/images/slider/img-slide-5.jpg
--rw-rw-rw-   0        0        0   246009 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/images/slider/img1.jpg
--rw-rw-rw-   0        0        0   165567 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/images/slider/img2.jpg
--rw-rw-rw-   0        0        0   168914 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/images/slider/img3.jpg
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.416927 django-admin-datta-1.0.7/admin_datta/static/assets/images/user/
--rw-rw-rw-   0        0        0    24576 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/images/user/Thumbs.db
--rw-rw-rw-   0        0        0     9287 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/images/user/avatar-1.jpg
--rw-rw-rw-   0        0        0     9372 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/images/user/avatar-2.jpg
--rw-rw-rw-   0        0        0     9408 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/images/user/avatar-3.jpg
--rw-rw-rw-   0        0        0     8489 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/images/user/avatar-4.jpg
--rw-rw-rw-   0        0        0     9350 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/images/user/avatar-5.jpg
--rw-rw-rw-   0        0        0     1662 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/images/user/user-1.png
--rw-rw-rw-   0        0        0     1560 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/images/user/user-2.png
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.437963 django-admin-datta-1.0.7/admin_datta/static/assets/images/widget/
--rw-rw-rw-   0        0        0   120832 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/images/widget/Thumbs.db
--rw-rw-rw-   0        0        0   104704 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/images/widget/dashborad-1.png
--rw-rw-rw-   0        0        0   170223 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/images/widget/dashborad-2.png
--rw-rw-rw-   0        0        0   115557 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/images/widget/dashborad-3.png
--rw-rw-rw-   0        0        0    14068 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/images/widget/dashborad-4.png
--rw-rw-rw-   0        0        0     6239 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/images/widget/dashborad-5.png
--rw-rw-rw-   0        0        0     8193 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/images/widget/dashborad-6.png
--rw-rw-rw-   0        0        0   111459 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/images/widget/emoticon.png
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.447267 django-admin-datta-1.0.7/admin_datta/static/assets/js/
--rw-rw-rw-   0        0        0     2141 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/js/dark-mode.js
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.452267 django-admin-datta-1.0.7/admin_datta/static/assets/js/pages/
--rw-rw-rw-   0        0        0     8008 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/js/pages/chart-morris-custom.js
--rw-rw-rw-   0        0        0     4360 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/js/pages/google-maps.js
--rw-rw-rw-   0        0        0    15247 2023-02-28 04:46:45.000000 django-admin-datta-1.0.7/admin_datta/static/assets/js/pcoded.min.js
--rw-rw-rw-   0        0        0   117122 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/js/vendor-all.min.js
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.137133 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.120083 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/amchart/
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.554702 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/amchart/js/
--rw-rw-rw-   0        0        0   209489 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/amchart/js/amcharts.js
--rw-rw-rw-   0        0        0   168766 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/amchart/js/ammap.min.js
--rw-rw-rw-   0        0        0    12860 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/amchart/js/gauge.js
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.559752 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/amchart/js/images/
--rw-rw-rw-   0        0        0      679 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/amchart/js/images/dragIconRoundBig.svg
--rw-rw-rw-   0        0        0      539 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/amchart/js/images/lens.svg
--rw-rw-rw-   0        0        0     2916 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/amchart/js/light.js
--rw-rw-rw-   0        0        0    14700 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/amchart/js/pie.min.js
--rw-rw-rw-   0        0        0     6464 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/amchart/js/radar.js
--rw-rw-rw-   0        0        0    49491 2023-02-11 11:10:18.000000 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/amchart/js/serial.js
--rw-rw-rw-   0        0        0    30336 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/amchart/js/usaLow.js
--rw-rw-rw-   0        0        0   130785 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/amchart/js/worldLow.js
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.122665 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/animation/
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.561728 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/animation/css/
--rw-rw-rw-   0        0        0    57908 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/animation/css/animate.min.css
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.123595 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/bootstrap/
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.582784 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/bootstrap/css/
--rw-rw-rw-   0        0        0   182626 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/bootstrap/css/bootstrap.css
--rw-rw-rw-   0        0        0   140893 2023-02-28 04:49:50.000000 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/bootstrap/css/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.590800 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/bootstrap/js/
--rw-rw-rw-   0        0        0   127709 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/bootstrap/js/bootstrap.js
--rw-rw-rw-   0        0        0    50698 2023-02-28 04:49:34.000000 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/bootstrap/js/bootstrap.min.js
--rw-rw-rw-   0        0        0    19213 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/bootstrap/js/popover.js
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.125596 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/chart-morris/
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.592364 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/chart-morris/css/
--rw-rw-rw-   0        0        0      435 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/chart-morris/css/morris.css
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.597329 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/chart-morris/js/
--rw-rw-rw-   0        0        0    35658 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/chart-morris/js/morris.min.js
--rw-rw-rw-   0        0        0    92631 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/chart-morris/js/raphael.min.js
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.126598 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/google-maps/
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.621741 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/google-maps/js/
--rw-rw-rw-   0        0        0    46138 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/google-maps/js/gmaps.js
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.138136 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/jquery/
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.638475 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/jquery/js/
--rw-rw-rw-   0        0        0    86929 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/jquery/js/jquery.min.js
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.130600 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/jquery-scrollbar/
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.627909 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/jquery-scrollbar/css/
--rw-rw-rw-   0        0        0     2851 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/jquery-scrollbar/css/jquery.scrollbar.min.css
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.629913 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/jquery-scrollbar/js/
--rw-rw-rw-   0        0        0    11662 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/jquery-scrollbar/js/jquery.scrollbar.min.js
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.136134 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/jquery-ui/
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.632418 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/jquery-ui/js/
--rw-rw-rw-   0        0        0   477536 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/static/assets/plugins/jquery-ui/js/jquery-ui.js
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.640431 django-admin-datta-1.0.7/admin_datta/static/assets/scss/
--rw-rw-rw-   0        0        0     3741 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/static/assets/scss/dark.scss
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.673952 django-admin-datta-1.0.7/admin_datta/templates/
--rw-rw-rw-   0        0        0        0 2022-09-27 05:30:21.000000 django-admin-datta-1.0.7/admin_datta/templates/.gitkeep
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.693566 django-admin-datta-1.0.7/admin_datta/templates/accounts/
--rw-rw-rw-   0        0        0     1479 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/accounts/auth-change-password.html
--rw-rw-rw-   0        0        0      963 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/accounts/auth-password-change-done.html
--rw-rw-rw-   0        0        0      994 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/accounts/auth-password-reset-complete.html
--rw-rw-rw-   0        0        0     1494 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/accounts/auth-password-reset-confirm.html
--rw-rw-rw-   0        0        0     1028 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/accounts/auth-password-reset-done.html
--rw-rw-rw-   0        0        0     1494 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/accounts/auth-reset-password.html
--rw-rw-rw-   0        0        0     2184 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/accounts/auth-signin.html
--rw-rw-rw-   0        0        0     2288 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/accounts/auth-signup.html
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.759530 django-admin-datta-1.0.7/admin_datta/templates/admin/
--rw-rw-rw-   0        0        0        0 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/admin/.gitkeep
--rw-rw-rw-   0        0        0     1743 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/admin/actions.html
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.142646 django-admin-datta-1.0.7/admin_datta/templates/admin/auth/
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.763043 django-admin-datta-1.0.7/admin_datta/templates/admin/auth/user/
--rw-rw-rw-   0        0        0      471 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/admin/auth/user/add_form.html
--rw-rw-rw-   0        0        0     5360 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/admin/auth/user/change_password.html
--rw-rw-rw-   0        0        0     4438 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/admin/change_form.html
--rw-rw-rw-   0        0        0      691 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/admin/change_form_object_tools.html
--rw-rw-rw-   0        0        0     4508 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/admin/change_list.html
--rw-rw-rw-   0        0        0      605 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/admin/change_list_object_tools.html
--rw-rw-rw-   0        0        0     3232 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/admin/change_list_results.html
--rw-rw-rw-   0        0        0     5853 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/admin/delete_confirmation.html
--rw-rw-rw-   0        0        0     6198 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/admin/delete_selected_confirmation.html
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.770053 django-admin-datta-1.0.7/admin_datta/templates/admin/edit_inline/
--rw-rw-rw-   0        0        0     3893 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/admin/edit_inline/stacked.html
--rw-rw-rw-   0        0        0     7834 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/admin/edit_inline/tabular.html
--rw-rw-rw-   0        0        0      643 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/admin/filter.html
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.777532 django-admin-datta-1.0.7/admin_datta/templates/admin/includes/
--rw-rw-rw-   0        0        0     2572 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/admin/includes/fieldset.html
--rw-rw-rw-   0        0        0      339 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/admin/includes/object_delete_summary.html
--rw-rw-rw-   0        0        0    28386 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/admin/index.html
--rw-rw-rw-   0        0        0     2724 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/admin/invalid_setup.html
--rw-rw-rw-   0        0        0     3365 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/admin/login.html
--rw-rw-rw-   0        0        0     2818 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/admin/object_history.html
--rw-rw-rw-   0        0        0     2317 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/admin/pagination.html
--rw-rw-rw-   0        0        0     2155 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/admin/search_form.html
--rw-rw-rw-   0        0        0     1616 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/admin/submit_line.html
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.844366 django-admin-datta-1.0.7/admin_datta/templates/includes/
--rw-rw-rw-   0        0        0      735 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/includes/breadcrumb.html
--rw-rw-rw-   0        0        0     1758 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/includes/head.html
--rw-rw-rw-   0        0        0     6727 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/includes/navigation.html
--rw-rw-rw-   0        0        0      168 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/includes/pre-loader.html
--rw-rw-rw-   0        0        0      323 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/includes/scripts.html
--rw-rw-rw-   0        0        0     8551 2023-02-27 06:26:13.000000 django-admin-datta-1.0.7/admin_datta/templates/includes/sidebar.html
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.862356 django-admin-datta-1.0.7/admin_datta/templates/layouts/
--rw-rw-rw-   0        0        0      306 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/layouts/base-auth.html
--rw-rw-rw-   0        0        0     1172 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/layouts/base.html
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.908403 django-admin-datta-1.0.7/admin_datta/templates/pages/
--rw-rw-rw-   0        0        0     2857 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/pages/chart-morris.html
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.924762 django-admin-datta-1.0.7/admin_datta/templates/pages/components/
--rw-rw-rw-   0        0        0     1907 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/pages/components/bc_badges.html
--rw-rw-rw-   0        0        0     4650 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/pages/components/bc_breadcrumb-pagination.html
--rw-rw-rw-   0        0        0    12079 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/pages/components/bc_button.html
--rw-rw-rw-   0        0        0     6970 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/pages/components/bc_collapse.html
--rw-rw-rw-   0        0        0    10818 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/pages/components/bc_tabs.html
--rw-rw-rw-   0        0        0     9952 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/pages/components/bc_typography.html
--rw-rw-rw-   0        0        0     5996 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/pages/components/icon-feather.html
--rw-rw-rw-   0        0        0    15591 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/pages/form_elements.html
--rw-rw-rw-   0        0        0    28386 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/pages/index.html
--rw-rw-rw-   0        0        0     5101 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/pages/map-google.html
--rw-rw-rw-   0        0        0     3810 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/pages/profile.html
--rw-rw-rw-   0        0        0      945 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/pages/sample-page.html
--rw-rw-rw-   0        0        0     4635 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/pages/tbl_bootstrap.html
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.946875 django-admin-datta-1.0.7/admin_datta/templates/registration/
--rw-rw-rw-   0        0        0        0 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/registration/.gitkeep
--rw-rw-rw-   0        0        0     1458 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/registration/logged_out.html
--rw-rw-rw-   0        0        0     1971 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/registration/password_change_done.html
--rw-rw-rw-   0        0        0     3308 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templates/registration/password_change_form.html
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.953407 django-admin-datta-1.0.7/admin_datta/templatetags/
--rw-rw-rw-   0        0        0        0 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templatetags/__init__.py
--rw-rw-rw-   0        0        0     2550 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templatetags/admin_datta.py
--rw-rw-rw-   0        0        0      178 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/templatetags/replace_value.py
--rw-rw-rw-   0        0        0     2342 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/urls.py
--rw-rw-rw-   0        0        0    16593 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/utils.py
--rw-rw-rw-   0        0        0     4313 2023-02-11 11:10:19.000000 django-admin-datta-1.0.7/admin_datta/views.py
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.961468 django-admin-datta-1.0.7/django_admin_datta.egg-info/
--rw-rw-rw-   0        0        0     7309 2023-02-28 05:17:39.000000 django-admin-datta-1.0.7/django_admin_datta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8935 2023-02-28 05:17:40.000000 django-admin-datta-1.0.7/django_admin_datta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-28 05:17:39.000000 django-admin-datta-1.0.7/django_admin_datta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-27 05:41:21.000000 django-admin-datta-1.0.7/django_admin_datta.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2023-02-28 05:17:39.000000 django-admin-datta-1.0.7/django_admin_datta.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-28 05:17:40.962942 django-admin-datta-1.0.7/docs/
--rw-rw-rw-   0        0        0       13 2022-09-27 05:30:21.000000 django-admin-datta-1.0.7/docs/blank.txt
--rw-rw-rw-   0        0        0       42 2023-02-28 05:17:40.966950 django-admin-datta-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1343 2023-02-28 05:15:31.000000 django-admin-datta-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.452172 django-admin-datta-1.0.8/
+-rw-rw-rw-   0        0        0     1113 2022-09-27 05:30:21.000000 django-admin-datta-1.0.8/LICENSE.md
+-rw-rw-rw-   0        0        0      144 2023-02-09 15:44:00.000000 django-admin-datta-1.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     7277 2023-05-31 07:35:09.449159 django-admin-datta-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     6182 2023-05-31 07:29:40.000000 django-admin-datta-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.742652 django-admin-datta-1.0.8/admin_datta/
+-rw-rw-rw-   0        0        0       78 2022-09-27 05:30:21.000000 django-admin-datta-1.0.8/admin_datta/__init__.py
+-rw-rw-rw-   0        0        0       78 2022-09-27 05:30:21.000000 django-admin-datta-1.0.8/admin_datta/admin.py
+-rw-rw-rw-   0        0        0      235 2023-02-09 15:45:05.000000 django-admin-datta-1.0.8/admin_datta/apps.py
+-rw-rw-rw-   0        0        0     2601 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/forms.py
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.744622 django-admin-datta-1.0.8/admin_datta/static/
+-rw-rw-rw-   0        0        0        0 2022-09-27 05:30:21.000000 django-admin-datta-1.0.8/admin_datta/static/.gitkeep
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.679965 django-admin-datta-1.0.8/admin_datta/static/assets/
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.778479 django-admin-datta-1.0.8/admin_datta/static/assets/css/
+-rw-rw-rw-   0        0        0     3610 2023-02-28 04:48:58.000000 django-admin-datta-1.0.8/admin_datta/static/assets/css/dark.css
+-rw-rw-rw-   0        0        0     9732 2023-05-31 07:29:40.000000 django-admin-datta-1.0.8/admin_datta/static/assets/css/forms.css
+-rw-rw-rw-   0        0        0   325947 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/css/style.css
+-rw-rw-rw-   0        0        0    12595 2023-05-31 07:29:40.000000 django-admin-datta-1.0.8/admin_datta/static/assets/css/widgets.css
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.646331 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.781490 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/datta/
+-rw-rw-rw-   0        0        0     1623 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/datta/datta-icon.css
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.792042 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/datta/fonts/
+-rw-rw-rw-   0        0        0     2548 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/datta/fonts/pct.eot
+-rw-rw-rw-   0        0        0     2553 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/datta/fonts/pct.svg
+-rw-rw-rw-   0        0        0     2400 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/datta/fonts/pct.ttf
+-rw-rw-rw-   0        0        0     1544 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/datta/fonts/pct.woff
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.645334 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/feather/
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.794041 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/feather/css/
+-rw-rw-rw-   0        0        0    12312 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/feather/css/feather.css
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.845343 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/feather/fonts/
+-rw-rw-rw-   0        0        0    55828 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/feather/fonts/feather.eot
+-rw-rw-rw-   0        0        0   192354 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/feather/fonts/feather.svg
+-rw-rw-rw-   0        0        0    55664 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/feather/fonts/feather.ttf
+-rw-rw-rw-   0        0        0    26432 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/feather/fonts/feather.woff
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.647330 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.847344 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/css/
+-rw-rw-rw-   0        0        0    41069 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/css/fontawesome-all.min.css
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.911785 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/
+-rw-rw-rw-   0        0        0   111620 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-brands-400.eot
+-rw-rw-rw-   0        0        0   600938 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-brands-400.svg
+-rw-rw-rw-   0        0        0   111384 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-brands-400.ttf
+-rw-rw-rw-   0        0        0    71560 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-brands-400.woff
+-rw-rw-rw-   0        0        0    61336 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-brands-400.woff2
+-rw-rw-rw-   0        0        0    31272 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-regular-400.eot
+-rw-rw-rw-   0        0        0   105078 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-regular-400.svg
+-rw-rw-rw-   0        0        0    31044 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-regular-400.ttf
+-rw-rw-rw-   0        0        0    14724 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-regular-400.woff
+-rw-rw-rw-   0        0        0    12188 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-regular-400.woff2
+-rw-rw-rw-   0        0        0   133140 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.eot
+-rw-rw-rw-   0        0        0   490291 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.svg
+-rw-rw-rw-   0        0        0   132920 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.ttf
+-rw-rw-rw-   0        0        0    63836 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.woff
+-rw-rw-rw-   0        0        0    50372 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.woff2
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.994316 django-admin-datta-1.0.8/admin_datta/static/assets/images/
+-rw-rw-rw-   0        0        0    45568 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/Thumbs.db
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.021776 django-admin-datta-1.0.8/admin_datta/static/assets/images/browser/
+-rw-rw-rw-   0        0        0    23040 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/browser/Thumbs.db
+-rw-rw-rw-   0        0        0     3822 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/browser/chrome.png
+-rw-rw-rw-   0        0        0     4809 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/browser/firefox.png
+-rw-rw-rw-   0        0        0     4359 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/browser/ie.png
+-rw-rw-rw-   0        0        0     3379 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/browser/opera.png
+-rw-rw-rw-   0        0        0     4915 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/browser/safari.png
+-rw-rw-rw-   0        0        0     1150 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/favicon.ico
+-rw-rw-rw-   0        0        0      334 2023-05-31 07:29:40.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/icon-addlink.svg
+-rw-rw-rw-   0        0        0     1095 2023-05-31 07:29:40.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/icon-calendar.svg
+-rw-rw-rw-   0        0        0      383 2023-05-31 07:29:40.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/icon-changelink.svg
+-rw-rw-rw-   0        0        0      686 2023-05-31 07:29:40.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/icon-clock.svg
+-rw-rw-rw-   0        0        0      395 2023-05-31 07:29:40.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/icon-deletelink.svg
+-rw-rw-rw-   0        0        0      563 2023-05-31 07:29:40.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/icon-no.svg
+-rw-rw-rw-   0        0        0      658 2023-05-31 07:29:40.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/icon-unknown-alt.svg
+-rw-rw-rw-   0        0        0      658 2023-05-31 07:29:40.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/icon-unknown.svg
+-rw-rw-rw-   0        0        0      584 2023-05-31 07:29:40.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/icon-viewlink.svg
+-rw-rw-rw-   0        0        0      439 2023-05-31 07:29:40.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/icon-yes.svg
+-rw-rw-rw-   0        0        0      563 2023-05-31 07:29:40.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/inline-delete.svg
+-rw-rw-rw-   0        0        0     2091 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/logo-dark.png
+-rw-rw-rw-   0        0        0     1529 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/logo-thumb.png
+-rw-rw-rw-   0        0        0     2131 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/logo.png
+-rw-rw-rw-   0        0        0      461 2023-05-31 07:29:40.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/search.svg
+-rw-rw-rw-   0        0        0     3325 2023-05-31 07:29:40.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/selector-icons.svg
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.044887 django-admin-datta-1.0.8/admin_datta/static/assets/images/slider/
+-rw-rw-rw-   0        0        0    31417 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/slider/img-slide-1.jpg
+-rw-rw-rw-   0        0        0    66369 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/slider/img-slide-2.jpg
+-rw-rw-rw-   0        0        0    22071 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/slider/img-slide-3.jpg
+-rw-rw-rw-   0        0        0    21820 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/slider/img-slide-4.jpg
+-rw-rw-rw-   0        0        0    33652 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/slider/img-slide-5.jpg
+-rw-rw-rw-   0        0        0   246009 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/slider/img1.jpg
+-rw-rw-rw-   0        0        0   165567 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/slider/img2.jpg
+-rw-rw-rw-   0        0        0   168914 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/slider/img3.jpg
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.068790 django-admin-datta-1.0.8/admin_datta/static/assets/images/user/
+-rw-rw-rw-   0        0        0    24576 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/user/Thumbs.db
+-rw-rw-rw-   0        0        0     9287 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/user/avatar-1.jpg
+-rw-rw-rw-   0        0        0     9372 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/user/avatar-2.jpg
+-rw-rw-rw-   0        0        0     9408 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/user/avatar-3.jpg
+-rw-rw-rw-   0        0        0     8489 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/user/avatar-4.jpg
+-rw-rw-rw-   0        0        0     9350 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/user/avatar-5.jpg
+-rw-rw-rw-   0        0        0     1662 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/user/user-1.png
+-rw-rw-rw-   0        0        0     1560 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/user/user-2.png
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.102031 django-admin-datta-1.0.8/admin_datta/static/assets/images/widget/
+-rw-rw-rw-   0        0        0   120832 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/widget/Thumbs.db
+-rw-rw-rw-   0        0        0   104704 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/widget/dashborad-1.png
+-rw-rw-rw-   0        0        0   170223 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/widget/dashborad-2.png
+-rw-rw-rw-   0        0        0   115557 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/widget/dashborad-3.png
+-rw-rw-rw-   0        0        0    14068 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/widget/dashborad-4.png
+-rw-rw-rw-   0        0        0     6239 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/widget/dashborad-5.png
+-rw-rw-rw-   0        0        0     8193 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/widget/dashborad-6.png
+-rw-rw-rw-   0        0        0   111459 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/images/widget/emoticon.png
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.128429 django-admin-datta-1.0.8/admin_datta/static/assets/js/
+-rw-rw-rw-   0        0        0     2141 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/js/dark-mode.js
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.134329 django-admin-datta-1.0.8/admin_datta/static/assets/js/pages/
+-rw-rw-rw-   0        0        0     8008 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/js/pages/chart-morris-custom.js
+-rw-rw-rw-   0        0        0     4360 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/js/pages/google-maps.js
+-rw-rw-rw-   0        0        0    15247 2023-02-28 04:46:45.000000 django-admin-datta-1.0.8/admin_datta/static/assets/js/pcoded.min.js
+-rw-rw-rw-   0        0        0   117122 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/js/vendor-all.min.js
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.678967 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.667291 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.183090 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/
+-rw-rw-rw-   0        0        0   209489 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/amcharts.js
+-rw-rw-rw-   0        0        0   168766 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/ammap.min.js
+-rw-rw-rw-   0        0        0    12860 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/gauge.js
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.189173 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/images/
+-rw-rw-rw-   0        0        0      679 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/images/dragIconRoundBig.svg
+-rw-rw-rw-   0        0        0      539 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/images/lens.svg
+-rw-rw-rw-   0        0        0     2916 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/light.js
+-rw-rw-rw-   0        0        0    14700 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/pie.min.js
+-rw-rw-rw-   0        0        0     6464 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/radar.js
+-rw-rw-rw-   0        0        0    49491 2023-02-11 11:10:18.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/serial.js
+-rw-rw-rw-   0        0        0    30336 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/usaLow.js
+-rw-rw-rw-   0        0        0   130785 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/worldLow.js
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.669450 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/animation/
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.191213 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/animation/css/
+-rw-rw-rw-   0        0        0    57908 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/animation/css/animate.min.css
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.671454 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/bootstrap/
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.197213 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/bootstrap/css/
+-rw-rw-rw-   0        0        0   182626 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/bootstrap/css/bootstrap.css
+-rw-rw-rw-   0        0        0   140893 2023-02-28 04:49:50.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/bootstrap/css/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.209029 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/bootstrap/js/
+-rw-rw-rw-   0        0        0   127709 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/bootstrap/js/bootstrap.js
+-rw-rw-rw-   0        0        0    50698 2023-02-28 04:49:34.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/bootstrap/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0    19213 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/bootstrap/js/popover.js
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.673455 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/chart-morris/
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.213032 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/chart-morris/css/
+-rw-rw-rw-   0        0        0      435 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/chart-morris/css/morris.css
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.218554 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/chart-morris/js/
+-rw-rw-rw-   0        0        0    35658 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/chart-morris/js/morris.min.js
+-rw-rw-rw-   0        0        0    92631 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/chart-morris/js/raphael.min.js
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.674453 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/google-maps/
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.222563 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/google-maps/js/
+-rw-rw-rw-   0        0        0    46138 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/google-maps/js/gmaps.js
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.678967 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/jquery/
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.239612 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/jquery/js/
+-rw-rw-rw-   0        0        0    86929 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/jquery/js/jquery.min.js
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.676452 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/jquery-scrollbar/
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.226563 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/jquery-scrollbar/css/
+-rw-rw-rw-   0        0        0     2851 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/jquery-scrollbar/css/jquery.scrollbar.min.css
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.229084 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/jquery-scrollbar/js/
+-rw-rw-rw-   0        0        0    11662 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/jquery-scrollbar/js/jquery.scrollbar.min.js
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.677958 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/jquery-ui/
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.232086 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/jquery-ui/js/
+-rw-rw-rw-   0        0        0   477536 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/static/assets/plugins/jquery-ui/js/jquery-ui.js
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.243623 django-admin-datta-1.0.8/admin_datta/static/assets/scss/
+-rw-rw-rw-   0        0        0     3741 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/static/assets/scss/dark.scss
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.248134 django-admin-datta-1.0.8/admin_datta/templates/
+-rw-rw-rw-   0        0        0        0 2022-09-27 05:30:21.000000 django-admin-datta-1.0.8/admin_datta/templates/.gitkeep
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.280315 django-admin-datta-1.0.8/admin_datta/templates/accounts/
+-rw-rw-rw-   0        0        0     1479 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/accounts/auth-change-password.html
+-rw-rw-rw-   0        0        0      963 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/accounts/auth-password-change-done.html
+-rw-rw-rw-   0        0        0      994 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/accounts/auth-password-reset-complete.html
+-rw-rw-rw-   0        0        0     1494 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/accounts/auth-password-reset-confirm.html
+-rw-rw-rw-   0        0        0     1028 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/accounts/auth-password-reset-done.html
+-rw-rw-rw-   0        0        0     1494 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/accounts/auth-reset-password.html
+-rw-rw-rw-   0        0        0     2184 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/accounts/auth-signin.html
+-rw-rw-rw-   0        0        0     2288 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/accounts/auth-signup.html
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.322087 django-admin-datta-1.0.8/admin_datta/templates/admin/
+-rw-rw-rw-   0        0        0        0 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/.gitkeep
+-rw-rw-rw-   0        0        0     1743 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/actions.html
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:08.682974 django-admin-datta-1.0.8/admin_datta/templates/admin/auth/
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.326603 django-admin-datta-1.0.8/admin_datta/templates/admin/auth/user/
+-rw-rw-rw-   0        0        0      471 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/auth/user/add_form.html
+-rw-rw-rw-   0        0        0     5360 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/auth/user/change_password.html
+-rw-rw-rw-   0        0        0     4438 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/change_form.html
+-rw-rw-rw-   0        0        0      691 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/change_form_object_tools.html
+-rw-rw-rw-   0        0        0     4508 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/change_list.html
+-rw-rw-rw-   0        0        0      605 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/change_list_object_tools.html
+-rw-rw-rw-   0        0        0     3232 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/change_list_results.html
+-rw-rw-rw-   0        0        0     5853 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/delete_confirmation.html
+-rw-rw-rw-   0        0        0     6198 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/delete_selected_confirmation.html
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.332170 django-admin-datta-1.0.8/admin_datta/templates/admin/edit_inline/
+-rw-rw-rw-   0        0        0     3893 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/edit_inline/stacked.html
+-rw-rw-rw-   0        0        0     7788 2023-05-31 07:29:40.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/edit_inline/tabular.html
+-rw-rw-rw-   0        0        0      643 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/filter.html
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.337172 django-admin-datta-1.0.8/admin_datta/templates/admin/includes/
+-rw-rw-rw-   0        0        0     2572 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/includes/fieldset.html
+-rw-rw-rw-   0        0        0      339 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/includes/object_delete_summary.html
+-rw-rw-rw-   0        0        0    28386 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/index.html
+-rw-rw-rw-   0        0        0     2724 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/invalid_setup.html
+-rw-rw-rw-   0        0        0     3365 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/login.html
+-rw-rw-rw-   0        0        0     2818 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/object_history.html
+-rw-rw-rw-   0        0        0     2317 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/pagination.html
+-rw-rw-rw-   0        0        0     2155 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/search_form.html
+-rw-rw-rw-   0        0        0     1616 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/admin/submit_line.html
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.349212 django-admin-datta-1.0.8/admin_datta/templates/includes/
+-rw-rw-rw-   0        0        0      735 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/includes/breadcrumb.html
+-rw-rw-rw-   0        0        0     1758 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/includes/head.html
+-rw-rw-rw-   0        0        0     6727 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/includes/navigation.html
+-rw-rw-rw-   0        0        0      168 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/includes/pre-loader.html
+-rw-rw-rw-   0        0        0      323 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/includes/scripts.html
+-rw-rw-rw-   0        0        0     8551 2023-02-27 06:26:13.000000 django-admin-datta-1.0.8/admin_datta/templates/includes/sidebar.html
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.368246 django-admin-datta-1.0.8/admin_datta/templates/layouts/
+-rw-rw-rw-   0        0        0      306 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/layouts/base-auth.html
+-rw-rw-rw-   0        0        0     1428 2023-05-31 07:29:40.000000 django-admin-datta-1.0.8/admin_datta/templates/layouts/base.html
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.398208 django-admin-datta-1.0.8/admin_datta/templates/pages/
+-rw-rw-rw-   0        0        0     2857 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/pages/chart-morris.html
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.422661 django-admin-datta-1.0.8/admin_datta/templates/pages/components/
+-rw-rw-rw-   0        0        0     1907 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/pages/components/bc_badges.html
+-rw-rw-rw-   0        0        0     4650 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/pages/components/bc_breadcrumb-pagination.html
+-rw-rw-rw-   0        0        0    12079 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/pages/components/bc_button.html
+-rw-rw-rw-   0        0        0     6970 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/pages/components/bc_collapse.html
+-rw-rw-rw-   0        0        0    10818 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/pages/components/bc_tabs.html
+-rw-rw-rw-   0        0        0     9952 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/pages/components/bc_typography.html
+-rw-rw-rw-   0        0        0     5996 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/pages/components/icon-feather.html
+-rw-rw-rw-   0        0        0    15591 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/pages/form_elements.html
+-rw-rw-rw-   0        0        0    28386 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/pages/index.html
+-rw-rw-rw-   0        0        0     5101 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/pages/map-google.html
+-rw-rw-rw-   0        0        0     3810 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/pages/profile.html
+-rw-rw-rw-   0        0        0      945 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/pages/sample-page.html
+-rw-rw-rw-   0        0        0     4635 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/pages/tbl_bootstrap.html
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.430123 django-admin-datta-1.0.8/admin_datta/templates/registration/
+-rw-rw-rw-   0        0        0        0 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/registration/.gitkeep
+-rw-rw-rw-   0        0        0     1458 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/registration/logged_out.html
+-rw-rw-rw-   0        0        0     1971 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/registration/password_change_done.html
+-rw-rw-rw-   0        0        0     3308 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templates/registration/password_change_form.html
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.437086 django-admin-datta-1.0.8/admin_datta/templatetags/
+-rw-rw-rw-   0        0        0        0 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     2550 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templatetags/admin_datta.py
+-rw-rw-rw-   0        0        0      178 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/templatetags/replace_value.py
+-rw-rw-rw-   0        0        0     2342 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/urls.py
+-rw-rw-rw-   0        0        0    16593 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/utils.py
+-rw-rw-rw-   0        0        0     4313 2023-02-11 11:10:19.000000 django-admin-datta-1.0.8/admin_datta/views.py
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.445647 django-admin-datta-1.0.8/django_admin_datta.egg-info/
+-rw-rw-rw-   0        0        0     7277 2023-05-31 07:35:07.000000 django-admin-datta-1.0.8/django_admin_datta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     9583 2023-05-31 07:35:08.000000 django-admin-datta-1.0.8/django_admin_datta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 07:35:07.000000 django-admin-datta-1.0.8/django_admin_datta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-02-27 05:41:21.000000 django-admin-datta-1.0.8/django_admin_datta.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2023-05-31 07:35:07.000000 django-admin-datta-1.0.8/django_admin_datta.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 07:35:09.446644 django-admin-datta-1.0.8/docs/
+-rw-rw-rw-   0        0        0       13 2022-09-27 05:30:21.000000 django-admin-datta-1.0.8/docs/blank.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 07:35:09.452172 django-admin-datta-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1343 2023-05-31 07:34:09.000000 django-admin-datta-1.0.8/setup.py
```

### Comparing `django-admin-datta-1.0.7/LICENSE.md` & `django-admin-datta-1.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/PKG-INFO` & `django-admin-datta-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-datta
-Version: 1.0.7
+Version: 1.0.8
 Summary: Modern template for Django admin interface
 Home-page: https://appseed.us/product/datta-able/django/
 Author: AppSeed.us
 Author-email: support@appseed.us
 License: MIT License
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -85,30 +85,30 @@
 ```
 
 <br />
 
 > Add `LOGIN_REDIRECT_URL` and `EMAIL_BACKEND` of your Django project `settings.py` file:
 
 ```python
-    LOGIN_REDIRECT_URL = '/'
-    # EMAIL_BACKEND = 'django.core.mail.backends.smtp.EmailBackend'
-    EMAIL_BACKEND = 'django.core.mail.backends.console.EmailBackend'
+LOGIN_REDIRECT_URL = '/'
+# EMAIL_BACKEND = 'django.core.mail.backends.smtp.EmailBackend'
+EMAIL_BACKEND = 'django.core.mail.backends.console.EmailBackend'
 ```
 
 <br />
 
 > Add `admin_datta` urls in your Django Project `urls.py` file
 
 ```python
-    from django.urls import path, include
+from django.urls import path, include
 
-    urlpatterns = [
-        ...
-        path('', include('admin_datta.urls')),
-    ]
+urlpatterns = [
+    ...
+    path('', include('admin_datta.urls')),
+]
 ```
 
 <br />
 
 > **Collect static** if you are in `production environment`:
 
 ```bash
```

### Comparing `django-admin-datta-1.0.7/README.md` & `django-admin-datta-1.0.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -58,30 +58,30 @@
 ```
 
 <br />
 
 > Add `LOGIN_REDIRECT_URL` and `EMAIL_BACKEND` of your Django project `settings.py` file:
 
 ```python
-    LOGIN_REDIRECT_URL = '/'
-    # EMAIL_BACKEND = 'django.core.mail.backends.smtp.EmailBackend'
-    EMAIL_BACKEND = 'django.core.mail.backends.console.EmailBackend'
+LOGIN_REDIRECT_URL = '/'
+# EMAIL_BACKEND = 'django.core.mail.backends.smtp.EmailBackend'
+EMAIL_BACKEND = 'django.core.mail.backends.console.EmailBackend'
 ```
 
 <br />
 
 > Add `admin_datta` urls in your Django Project `urls.py` file
 
 ```python
-    from django.urls import path, include
+from django.urls import path, include
 
-    urlpatterns = [
-        ...
-        path('', include('admin_datta.urls')),
-    ]
+urlpatterns = [
+    ...
+    path('', include('admin_datta.urls')),
+]
 ```
 
 <br />
 
 > **Collect static** if you are in `production environment`:
 
 ```bash
```

### Comparing `django-admin-datta-1.0.7/admin_datta/forms.py` & `django-admin-datta-1.0.8/admin_datta/forms.py`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/css/dark.css` & `django-admin-datta-1.0.8/admin_datta/static/assets/css/dark.css`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/css/forms.css` & `django-admin-datta-1.0.8/admin_datta/static/assets/css/forms.css`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,22 @@
 /* FORM ROWS */
 
 .form-row {
     overflow: hidden;
     padding: 10px;
     font-size: 13px;
     border-bottom: 1px solid #eee;
+    display: table-row !important;
 }
-
 .form-row img, .form-row input {
     vertical-align: middle;
 }
+.form-row .field-title {
+    padding-left: 0 !important;
+}
 
 .form-row label input[type="checkbox"] {
     margin-top: 0;
     vertical-align: 0;
 }
 
 form .form-row p {
@@ -462,21 +465,21 @@
 .inline-group .tabular tr td.original {
     padding: 2px 0 0 0;
     width: 0;
     _position: relative;
 }
 
 .inline-group .tabular th.original {
-    width: 0px;
-    padding: 0;
+    width: 0px !important;
+    padding: 0 !important;
 }
 
 .inline-group .tabular td.original p {
     position: absolute;
-    right: 0;
+    left: 5px;
     /*height: 1.1em;*/
     /*padding: 2px 9px;*/
     overflow: hidden;
     font-size: 12px;
     font-weight: bold;
     /*color: #666;*/
     _width: 700px;
@@ -505,21 +508,21 @@
     padding: 8px 10px;
     border-bottom: 1px solid #eee;
 }
 
 .inline-group ul.tools a.add,
 .inline-group div.add-row a,
 .inline-group .tabular tr.add-row td a {
-    background: url(../img/icon-addlink.svg) 0 1px no-repeat;
+    background: url(../images/icon-addlink.svg) 0 1px no-repeat;
     padding-left: 16px;
     font-size: 12px;
 }
 
 .empty-form {
-    display: none;
+    display: none !important;
 }
 
 /* RELATED FIELD ADD ONE / LOOKUP */
 
 .add-another, .related-lookup {
     margin-left: 5px;
     display: inline-block;
@@ -527,21 +530,21 @@
     background-repeat: no-repeat;
     background-size: 14px;
 }
 
 .add-another {
     width: 16px;
     height: 16px;
-    background-image: url(../img/icon-addlink.svg);
+    background-image: url(../images/icon-addlink.svg);
 }
 
 .related-lookup {
     width: 16px;
     height: 16px;
-    background-image: url(../img/search.svg);
+    background-image: url(../images/search.svg);
 }
 
 form .related-widget-wrapper ul {
     display: inline-block;
     margin-left: 0;
     padding-left: 0;
 }
```

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/css/style.css` & `django-admin-datta-1.0.8/admin_datta/static/assets/css/style.css`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/css/widgets.css` & `django-admin-datta-1.0.8/admin_datta/static/assets/css/widgets.css`

 * *Files 2% similar despite different names*

```diff
@@ -119,23 +119,23 @@
 }
 
 .active.selector-add:hover, .active.selector-remove:hover {
     cursor: pointer;
 }
 
 .selector-add {
-    background: url(../img/selector-icons.svg) 0 -96px no-repeat;
+    background: url(../images/selector-icons.svg) 0 -96px no-repeat;
 }
 
 .active.selector-add:focus, .active.selector-add:hover {
     background-position: 0 -112px;
 }
 
 .selector-remove {
-    background: url(../img/selector-icons.svg) 0 -64px no-repeat;
+    background: url(../images/selector-icons.svg) 0 -64px no-repeat;
 }
 
 .active.selector-remove:focus, .active.selector-remove:hover {
     background-position: 0 -80px;
 }
 
 a.selector-chooseall, a.selector-clearall {
@@ -162,25 +162,25 @@
 
 a.active.selector-chooseall:hover, a.active.selector-clearall:hover {
     cursor: pointer;
 }
 
 a.selector-chooseall {
     padding: 0 18px 0 0;
-    background: url(../img/selector-icons.svg) right -160px no-repeat;
+    background: url(../images/selector-icons.svg) right -160px no-repeat;
     cursor: default;
 }
 
 a.active.selector-chooseall:focus, a.active.selector-chooseall:hover {
     background-position: 100% -176px;
 }
 
 a.selector-clearall {
     padding: 0 0 0 18px;
-    background: url(../img/selector-icons.svg) 0 -128px no-repeat;
+    background: url(../images/selector-icons.svg) 0 -128px no-repeat;
     cursor: default;
 }
 
 a.active.selector-clearall:focus, a.active.selector-clearall:hover {
     background-position: 0 -144px;
 }
 
@@ -222,48 +222,48 @@
 }
 
 .stacked .selector-chooseall, .stacked .selector-clearall {
     display: none;
 }
 
 .stacked .selector-add {
-    background: url(../img/selector-icons.svg) 0 -32px no-repeat;
+    background: url(../images/selector-icons.svg) 0 -32px no-repeat;
     cursor: default;
 }
 
 .stacked .active.selector-add {
     background-position: 0 -48px;
     cursor: pointer;
 }
 
 .stacked .selector-remove {
-    background: url(../img/selector-icons.svg) 0 0 no-repeat;
+    background: url(../images/selector-icons.svg) 0 0 no-repeat;
     cursor: default;
 }
 
 .stacked .active.selector-remove {
     background-position: 0 -16px;
     cursor: pointer;
 }
 
 .selector .help-icon {
-    background: url(../img/icon-unknown.svg) 0 0 no-repeat;
+    background: url(../images/icon-unknown.svg) 0 0 no-repeat;
     display: inline-block;
     vertical-align: middle;
     margin: -2px 0 0 2px;
     width: 13px;
     height: 13px;
 }
 
 .selector .selector-chosen .help-icon {
-    background: url(../img/icon-unknown-alt.svg) 0 0 no-repeat;
+    background: url(../images/icon-unknown-alt.svg) 0 0 no-repeat;
 }
 
 .selector .search-label-icon {
-    background: url(../img/search.svg) 0 0 no-repeat;
+    background: url(../images/search.svg) 0 0 no-repeat;
     display: inline-block;
     height: 25px;
     width: 25px;
 }
 
 /* DATE AND TIME */
 
@@ -301,24 +301,24 @@
     vertical-align: middle;
     height: 16px;
     width: 16px;
     overflow: hidden;
 }
 
 .datetimeshortcuts .clock-icon {
-    background: url(../img/icon-clock.svg) 0 0 no-repeat;
+    background: url(../images/icon-clock.svg) 0 0 no-repeat;
 }
 
 .datetimeshortcuts a:focus .clock-icon,
 .datetimeshortcuts a:hover .clock-icon {
     background-position: 0 -16px;
 }
 
 .datetimeshortcuts .date-icon {
-    background: url(../img/icon-calendar.svg) 0 0 no-repeat;
+    background: url(../images/icon-calendar.svg) 0 0 no-repeat;
     top: -1px;
 }
 
 .datetimeshortcuts a:focus .date-icon,
 .datetimeshortcuts a:hover .date-icon {
     background-position: 0 -16px;
 }
@@ -498,25 +498,25 @@
     height: 15px;
     text-indent: -9999px;
     padding: 0;
 }
 
 .calendarnav-previous {
     left: 10px;
-    background: url(../img/calendar-icons.svg) 0 0 no-repeat;
+    background: url(../images/calendar-icons.svg) 0 0 no-repeat;
 }
 
 .calendarbox .calendarnav-previous:focus,
 .calendarbox .calendarnav-previous:hover {
     background-position: 0 -15px;
 }
 
 .calendarnav-next {
     right: 10px;
-    background: url(../img/calendar-icons.svg) 0 -30px no-repeat;
+    background: url(../images/calendar-icons.svg) 0 -30px no-repeat;
 }
 
 .calendarbox .calendarnav-next:focus,
 .calendarbox .calendarnav-next:hover {
     background-position: 0 -45px;
 }
 
@@ -549,15 +549,15 @@
 }
 
 /* EDIT INLINE */
 
 .inline-deletelink {
     float: right;
     text-indent: -9999px;
-    background: url(../img/inline-delete.svg) 0 0 no-repeat;
+    background: url(../images/inline-delete.svg) 0 0 no-repeat;
     width: 16px;
     height: 16px;
     border: 0px none;
 }
 
 .inline-deletelink:focus, .inline-deletelink:hover {
     cursor: pointer;
```

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/fonts/datta/datta-icon.css` & `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/datta/datta-icon.css`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/fonts/datta/fonts/pct.eot` & `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/datta/fonts/pct.eot`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/fonts/datta/fonts/pct.svg` & `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/datta/fonts/pct.svg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/fonts/datta/fonts/pct.ttf` & `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/datta/fonts/pct.ttf`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/fonts/datta/fonts/pct.woff` & `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/datta/fonts/pct.woff`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/fonts/feather/css/feather.css` & `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/feather/css/feather.css`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/fonts/feather/fonts/feather.eot` & `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/feather/fonts/feather.eot`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/fonts/feather/fonts/feather.svg` & `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/feather/fonts/feather.svg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/fonts/feather/fonts/feather.ttf` & `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/feather/fonts/feather.ttf`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/fonts/feather/fonts/feather.woff` & `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/feather/fonts/feather.woff`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/fonts/fontawesome/css/fontawesome-all.min.css` & `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/css/fontawesome-all.min.css`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-brands-400.eot` & `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-brands-400.svg` & `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-brands-400.ttf` & `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-brands-400.woff` & `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-brands-400.woff2` & `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-regular-400.eot` & `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-regular-400.svg` & `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-regular-400.ttf` & `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-regular-400.woff` & `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-regular-400.woff2` & `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.eot` & `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.svg` & `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.ttf` & `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.woff` & `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.woff2` & `django-admin-datta-1.0.8/admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/images/Thumbs.db` & `django-admin-datta-1.0.8/admin_datta/static/assets/images/Thumbs.db`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/images/browser/Thumbs.db` & `django-admin-datta-1.0.8/admin_datta/static/assets/images/browser/Thumbs.db`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/images/browser/chrome.png` & `django-admin-datta-1.0.8/admin_datta/static/assets/images/browser/chrome.png`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/images/browser/firefox.png` & `django-admin-datta-1.0.8/admin_datta/static/assets/images/browser/firefox.png`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/images/browser/ie.png` & `django-admin-datta-1.0.8/admin_datta/static/assets/images/browser/ie.png`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/images/browser/opera.png` & `django-admin-datta-1.0.8/admin_datta/static/assets/images/browser/opera.png`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/images/browser/safari.png` & `django-admin-datta-1.0.8/admin_datta/static/assets/images/browser/safari.png`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/images/favicon.ico` & `django-admin-datta-1.0.8/admin_datta/static/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/images/logo-dark.png` & `django-admin-datta-1.0.8/admin_datta/static/assets/images/logo-dark.png`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/images/logo-thumb.png` & `django-admin-datta-1.0.8/admin_datta/static/assets/images/logo-thumb.png`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/images/logo.png` & `django-admin-datta-1.0.8/admin_datta/static/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/images/slider/img-slide-1.jpg` & `django-admin-datta-1.0.8/admin_datta/static/assets/images/slider/img-slide-1.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/images/slider/img-slide-2.jpg` & `django-admin-datta-1.0.8/admin_datta/static/assets/images/slider/img-slide-2.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/images/slider/img-slide-3.jpg` & `django-admin-datta-1.0.8/admin_datta/static/assets/images/slider/img-slide-3.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/images/slider/img-slide-4.jpg` & `django-admin-datta-1.0.8/admin_datta/static/assets/images/slider/img-slide-4.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/images/slider/img-slide-5.jpg` & `django-admin-datta-1.0.8/admin_datta/static/assets/images/slider/img-slide-5.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/images/slider/img1.jpg` & `django-admin-datta-1.0.8/admin_datta/static/assets/images/slider/img1.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/images/slider/img2.jpg` & `django-admin-datta-1.0.8/admin_datta/static/assets/images/slider/img2.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/images/slider/img3.jpg` & `django-admin-datta-1.0.8/admin_datta/static/assets/images/slider/img3.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/images/user/Thumbs.db` & `django-admin-datta-1.0.8/admin_datta/static/assets/images/user/Thumbs.db`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/images/user/avatar-1.jpg` & `django-admin-datta-1.0.8/admin_datta/static/assets/images/user/avatar-1.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/images/user/avatar-2.jpg` & `django-admin-datta-1.0.8/admin_datta/static/assets/images/user/avatar-2.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/images/user/avatar-3.jpg` & `django-admin-datta-1.0.8/admin_datta/static/assets/images/user/avatar-3.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/images/user/avatar-4.jpg` & `django-admin-datta-1.0.8/admin_datta/static/assets/images/user/avatar-4.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/images/user/avatar-5.jpg` & `django-admin-datta-1.0.8/admin_datta/static/assets/images/user/avatar-5.jpg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/images/user/user-1.png` & `django-admin-datta-1.0.8/admin_datta/static/assets/images/user/user-1.png`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/images/user/user-2.png` & `django-admin-datta-1.0.8/admin_datta/static/assets/images/user/user-2.png`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/images/widget/Thumbs.db` & `django-admin-datta-1.0.8/admin_datta/static/assets/images/widget/Thumbs.db`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/images/widget/dashborad-1.png` & `django-admin-datta-1.0.8/admin_datta/static/assets/images/widget/dashborad-1.png`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/images/widget/dashborad-2.png` & `django-admin-datta-1.0.8/admin_datta/static/assets/images/widget/dashborad-2.png`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/images/widget/dashborad-3.png` & `django-admin-datta-1.0.8/admin_datta/static/assets/images/widget/dashborad-3.png`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/images/widget/dashborad-4.png` & `django-admin-datta-1.0.8/admin_datta/static/assets/images/widget/dashborad-4.png`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/images/widget/dashborad-5.png` & `django-admin-datta-1.0.8/admin_datta/static/assets/images/widget/dashborad-5.png`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/images/widget/dashborad-6.png` & `django-admin-datta-1.0.8/admin_datta/static/assets/images/widget/dashborad-6.png`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/images/widget/emoticon.png` & `django-admin-datta-1.0.8/admin_datta/static/assets/images/widget/emoticon.png`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/js/dark-mode.js` & `django-admin-datta-1.0.8/admin_datta/static/assets/js/dark-mode.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/js/pages/chart-morris-custom.js` & `django-admin-datta-1.0.8/admin_datta/static/assets/js/pages/chart-morris-custom.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/js/pages/google-maps.js` & `django-admin-datta-1.0.8/admin_datta/static/assets/js/pages/google-maps.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/js/pcoded.min.js` & `django-admin-datta-1.0.8/admin_datta/static/assets/js/pcoded.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/js/vendor-all.min.js` & `django-admin-datta-1.0.8/admin_datta/static/assets/js/vendor-all.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/plugins/amchart/js/amcharts.js` & `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/amcharts.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/plugins/amchart/js/ammap.min.js` & `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/ammap.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/plugins/amchart/js/gauge.js` & `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/gauge.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/plugins/amchart/js/images/dragIconRoundBig.svg` & `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/images/dragIconRoundBig.svg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/plugins/amchart/js/images/lens.svg` & `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/images/lens.svg`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/plugins/amchart/js/light.js` & `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/light.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/plugins/amchart/js/pie.min.js` & `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/pie.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/plugins/amchart/js/radar.js` & `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/radar.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/plugins/amchart/js/serial.js` & `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/serial.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/plugins/amchart/js/usaLow.js` & `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/usaLow.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/plugins/amchart/js/worldLow.js` & `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/amchart/js/worldLow.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/plugins/animation/css/animate.min.css` & `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/animation/css/animate.min.css`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/plugins/bootstrap/css/bootstrap.css` & `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/plugins/bootstrap/css/bootstrap.min.css` & `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/plugins/bootstrap/js/bootstrap.js` & `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/plugins/bootstrap/js/bootstrap.min.js` & `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/plugins/bootstrap/js/popover.js` & `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/bootstrap/js/popover.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/plugins/chart-morris/js/morris.min.js` & `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/chart-morris/js/morris.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/plugins/chart-morris/js/raphael.min.js` & `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/chart-morris/js/raphael.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/plugins/google-maps/js/gmaps.js` & `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/google-maps/js/gmaps.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/plugins/jquery/js/jquery.min.js` & `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/jquery/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/plugins/jquery-scrollbar/css/jquery.scrollbar.min.css` & `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/jquery-scrollbar/css/jquery.scrollbar.min.css`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/plugins/jquery-scrollbar/js/jquery.scrollbar.min.js` & `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/jquery-scrollbar/js/jquery.scrollbar.min.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/plugins/jquery-ui/js/jquery-ui.js` & `django-admin-datta-1.0.8/admin_datta/static/assets/plugins/jquery-ui/js/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/static/assets/scss/dark.scss` & `django-admin-datta-1.0.8/admin_datta/static/assets/scss/dark.scss`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/accounts/auth-change-password.html` & `django-admin-datta-1.0.8/admin_datta/templates/accounts/auth-change-password.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/accounts/auth-password-change-done.html` & `django-admin-datta-1.0.8/admin_datta/templates/accounts/auth-password-change-done.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/accounts/auth-password-reset-complete.html` & `django-admin-datta-1.0.8/admin_datta/templates/accounts/auth-password-reset-complete.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/accounts/auth-password-reset-confirm.html` & `django-admin-datta-1.0.8/admin_datta/templates/accounts/auth-password-reset-confirm.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/accounts/auth-password-reset-done.html` & `django-admin-datta-1.0.8/admin_datta/templates/accounts/auth-password-reset-done.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/accounts/auth-reset-password.html` & `django-admin-datta-1.0.8/admin_datta/templates/accounts/auth-reset-password.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/accounts/auth-signin.html` & `django-admin-datta-1.0.8/admin_datta/templates/accounts/auth-signin.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/accounts/auth-signup.html` & `django-admin-datta-1.0.8/admin_datta/templates/accounts/auth-signup.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/admin/actions.html` & `django-admin-datta-1.0.8/admin_datta/templates/admin/actions.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/admin/auth/user/change_password.html` & `django-admin-datta-1.0.8/admin_datta/templates/admin/auth/user/change_password.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/admin/change_form.html` & `django-admin-datta-1.0.8/admin_datta/templates/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/admin/change_form_object_tools.html` & `django-admin-datta-1.0.8/admin_datta/templates/admin/change_form_object_tools.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/admin/change_list.html` & `django-admin-datta-1.0.8/admin_datta/templates/admin/change_list.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/admin/change_list_object_tools.html` & `django-admin-datta-1.0.8/admin_datta/templates/admin/change_list_object_tools.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/admin/change_list_results.html` & `django-admin-datta-1.0.8/admin_datta/templates/admin/change_list_results.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/admin/delete_confirmation.html` & `django-admin-datta-1.0.8/admin_datta/templates/admin/delete_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/admin/delete_selected_confirmation.html` & `django-admin-datta-1.0.8/admin_datta/templates/admin/delete_selected_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/admin/edit_inline/stacked.html` & `django-admin-datta-1.0.8/admin_datta/templates/admin/edit_inline/stacked.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/admin/edit_inline/tabular.html` & `django-admin-datta-1.0.8/admin_datta/templates/admin/edit_inline/tabular.html`

 * *Files 0% similar despite different names*

```diff
@@ -19,16 +19,15 @@
                     <table class="table table-centered table-nowrap mb-0 rounded">
                         <thead class="thead-light">
                         <tr>
                             <th class="original"></th>
 
                             {% for field in inline_admin_formset.fields %}
                                 {% if not field.widget.is_hidden %}
-                                    <th class="column-
-                                            {{ field.name }}{% if field.required %} required{% endif %}">{{ field.label|capfirst }}
+                                    <th class="column-{{ field.name }}{% if field.required %} required{% endif %}">{{ field.label|capfirst }}
                                         {% if field.help_text %}
                                             <img src="{% static "admin/img/icon-unknown.svg" %}" class="help help-tooltip"
                                                  width="10" height="10" alt="({{ field.help_text|striptags }})"
                                                  title="{{ field.help_text|striptags }}">{% endif %}
                                     </th>
                                 {% endif %}
                             {% endfor %}
```

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/admin/filter.html` & `django-admin-datta-1.0.8/admin_datta/templates/admin/filter.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/admin/includes/fieldset.html` & `django-admin-datta-1.0.8/admin_datta/templates/admin/includes/fieldset.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/admin/index.html` & `django-admin-datta-1.0.8/admin_datta/templates/admin/index.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/admin/invalid_setup.html` & `django-admin-datta-1.0.8/admin_datta/templates/admin/invalid_setup.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/admin/login.html` & `django-admin-datta-1.0.8/admin_datta/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/admin/object_history.html` & `django-admin-datta-1.0.8/admin_datta/templates/admin/object_history.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/admin/pagination.html` & `django-admin-datta-1.0.8/admin_datta/templates/admin/pagination.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/admin/search_form.html` & `django-admin-datta-1.0.8/admin_datta/templates/admin/search_form.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/admin/submit_line.html` & `django-admin-datta-1.0.8/admin_datta/templates/admin/submit_line.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/includes/breadcrumb.html` & `django-admin-datta-1.0.8/admin_datta/templates/includes/breadcrumb.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/includes/head.html` & `django-admin-datta-1.0.8/admin_datta/templates/includes/head.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/includes/navigation.html` & `django-admin-datta-1.0.8/admin_datta/templates/includes/navigation.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/includes/sidebar.html` & `django-admin-datta-1.0.8/admin_datta/templates/includes/sidebar.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/layouts/base.html` & `django-admin-datta-1.0.8/admin_datta/templates/layouts/base.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 <!DOCTYPE html>
+{% load i18n static admin_datta %}
+{% get_current_language as LANGUAGE_CODE %}
+{% get_current_language_bidi as LANGUAGE_BIDI %}
+{% get_direction as direction %}
+{% get_admin_setting as admin_setting %}
 <html lang="en">
 
 <head>
   {% include 'includes/head.html' %}
   {% block extrastyle %}{% endblock extrastyle %}
+  {% block extrahead %}{% endblock extrahead %}
 </head>
 <body>
 
   {% block pre_loader %}
     {% include 'includes/pre-loader.html' %}
   {% endblock pre_loader %}
```

#### html2text {}

```diff
@@ -1,9 +1,12 @@
+ {% load i18n static admin_datta %} {% get_current_language as LANGUAGE_CODE %}
+{% get_current_language_bidi as LANGUAGE_BIDI %} {% get_direction as direction
+%} {% get_admin_setting as admin_setting %}
 {% include 'includes/head.html' %} {% block extrastyle %}{% endblock extrastyle
-%}
+%} {% block extrahead %}{% endblock extrahead %}
 {% block pre_loader %} {% include 'includes/pre-loader.html' %} {% endblock
 pre_loader %} {% block sidebar %} {% include 'includes/sidebar.html' %} {%
 endblock sidebar %} {% block header %} {% include 'includes/navigation.html' %}
 {% endblock header %}
  {% block breadcrumbs %} {% include 'includes/breadcrumb.html' %} {% endblock
 breadcrumbs %}
 {% block content %}{% endblock content %}
```

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/pages/chart-morris.html` & `django-admin-datta-1.0.8/admin_datta/templates/pages/chart-morris.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/pages/components/bc_badges.html` & `django-admin-datta-1.0.8/admin_datta/templates/pages/components/bc_badges.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/pages/components/bc_breadcrumb-pagination.html` & `django-admin-datta-1.0.8/admin_datta/templates/pages/components/bc_breadcrumb-pagination.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/pages/components/bc_button.html` & `django-admin-datta-1.0.8/admin_datta/templates/pages/components/bc_button.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/pages/components/bc_collapse.html` & `django-admin-datta-1.0.8/admin_datta/templates/pages/components/bc_collapse.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/pages/components/bc_tabs.html` & `django-admin-datta-1.0.8/admin_datta/templates/pages/components/bc_tabs.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/pages/components/bc_typography.html` & `django-admin-datta-1.0.8/admin_datta/templates/pages/components/bc_typography.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/pages/components/icon-feather.html` & `django-admin-datta-1.0.8/admin_datta/templates/pages/components/icon-feather.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/pages/form_elements.html` & `django-admin-datta-1.0.8/admin_datta/templates/pages/form_elements.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/pages/index.html` & `django-admin-datta-1.0.8/admin_datta/templates/pages/index.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/pages/map-google.html` & `django-admin-datta-1.0.8/admin_datta/templates/pages/map-google.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/pages/profile.html` & `django-admin-datta-1.0.8/admin_datta/templates/pages/profile.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/pages/sample-page.html` & `django-admin-datta-1.0.8/admin_datta/templates/pages/sample-page.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/pages/tbl_bootstrap.html` & `django-admin-datta-1.0.8/admin_datta/templates/pages/tbl_bootstrap.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/registration/logged_out.html` & `django-admin-datta-1.0.8/admin_datta/templates/registration/logged_out.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/registration/password_change_done.html` & `django-admin-datta-1.0.8/admin_datta/templates/registration/password_change_done.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templates/registration/password_change_form.html` & `django-admin-datta-1.0.8/admin_datta/templates/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/templatetags/admin_datta.py` & `django-admin-datta-1.0.8/admin_datta/templatetags/admin_datta.py`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/urls.py` & `django-admin-datta-1.0.8/admin_datta/urls.py`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/utils.py` & `django-admin-datta-1.0.8/admin_datta/utils.py`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/admin_datta/views.py` & `django-admin-datta-1.0.8/admin_datta/views.py`

 * *Files identical despite different names*

### Comparing `django-admin-datta-1.0.7/django_admin_datta.egg-info/PKG-INFO` & `django-admin-datta-1.0.8/django_admin_datta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-admin-datta
-Version: 1.0.7
+Version: 1.0.8
 Summary: Modern template for Django admin interface
 Home-page: https://appseed.us/product/datta-able/django/
 Author: AppSeed.us
 Author-email: support@appseed.us
 License: MIT License
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -85,30 +85,30 @@
 ```
 
 <br />
 
 > Add `LOGIN_REDIRECT_URL` and `EMAIL_BACKEND` of your Django project `settings.py` file:
 
 ```python
-    LOGIN_REDIRECT_URL = '/'
-    # EMAIL_BACKEND = 'django.core.mail.backends.smtp.EmailBackend'
-    EMAIL_BACKEND = 'django.core.mail.backends.console.EmailBackend'
+LOGIN_REDIRECT_URL = '/'
+# EMAIL_BACKEND = 'django.core.mail.backends.smtp.EmailBackend'
+EMAIL_BACKEND = 'django.core.mail.backends.console.EmailBackend'
 ```
 
 <br />
 
 > Add `admin_datta` urls in your Django Project `urls.py` file
 
 ```python
-    from django.urls import path, include
+from django.urls import path, include
 
-    urlpatterns = [
-        ...
-        path('', include('admin_datta.urls')),
-    ]
+urlpatterns = [
+    ...
+    path('', include('admin_datta.urls')),
+]
 ```
 
 <br />
 
 > **Collect static** if you are in `production environment`:
 
 ```bash
```

### Comparing `django-admin-datta-1.0.7/django_admin_datta.egg-info/SOURCES.txt` & `django-admin-datta-1.0.8/django_admin_datta.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -38,17 +38,30 @@
 admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.eot
 admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.svg
 admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.ttf
 admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.woff
 admin_datta/static/assets/fonts/fontawesome/webfonts/fa-solid-900.woff2
 admin_datta/static/assets/images/Thumbs.db
 admin_datta/static/assets/images/favicon.ico
+admin_datta/static/assets/images/icon-addlink.svg
+admin_datta/static/assets/images/icon-calendar.svg
+admin_datta/static/assets/images/icon-changelink.svg
+admin_datta/static/assets/images/icon-clock.svg
+admin_datta/static/assets/images/icon-deletelink.svg
+admin_datta/static/assets/images/icon-no.svg
+admin_datta/static/assets/images/icon-unknown-alt.svg
+admin_datta/static/assets/images/icon-unknown.svg
+admin_datta/static/assets/images/icon-viewlink.svg
+admin_datta/static/assets/images/icon-yes.svg
+admin_datta/static/assets/images/inline-delete.svg
 admin_datta/static/assets/images/logo-dark.png
 admin_datta/static/assets/images/logo-thumb.png
 admin_datta/static/assets/images/logo.png
+admin_datta/static/assets/images/search.svg
+admin_datta/static/assets/images/selector-icons.svg
 admin_datta/static/assets/images/browser/Thumbs.db
 admin_datta/static/assets/images/browser/chrome.png
 admin_datta/static/assets/images/browser/firefox.png
 admin_datta/static/assets/images/browser/ie.png
 admin_datta/static/assets/images/browser/opera.png
 admin_datta/static/assets/images/browser/safari.png
 admin_datta/static/assets/images/slider/img-slide-1.jpg
```

### Comparing `django-admin-datta-1.0.7/setup.py` & `django-admin-datta-1.0.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
     README = readme.read()
 
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
 name='django-admin-datta',
-version='1.0.7',
+version='1.0.8',
 zip_safe=False,
 packages=find_packages(),
 include_package_data=True,
 description='Modern template for Django admin interface',
 long_description=README,
 long_description_content_type="text/markdown",
 url='https://appseed.us/product/datta-able/django/',
```

