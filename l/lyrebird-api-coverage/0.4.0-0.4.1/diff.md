# Comparing `tmp/lyrebird-api-coverage-0.4.0.tar.gz` & `tmp/lyrebird-api-coverage-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lyrebird-api-coverage-0.4.0.tar", last modified: Thu May 25 13:32:36 2023, max compression
+gzip compressed data, was "dist/lyrebird-api-coverage-0.4.1.tar", last modified: Wed May 31 12:21:34 2023, max compression
```

## Comparing `lyrebird-api-coverage-0.4.0.tar` & `lyrebird-api-coverage-0.4.1.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:32:36.000000 lyrebird-api-coverage-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-05-25 13:32:36.000000 lyrebird-api-coverage-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:32:36.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:32:36.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/client/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/client/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/client/event_subscibe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/client/filter_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/client/format_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/client/jsonscheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/client/load_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/client/merge_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/client/report.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/client/url_compare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:32:36.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/default_conf/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/default_conf/base.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/default_conf/conf.json
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/default_conf/filter_config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:32:36.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:32:36.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/css/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/css/app.964cc419.css
--rw-r--r--   0 runner    (1001) docker     (123)   377184 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/css/chunk-vendors.129fc3b2.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:32:36.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    56484 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/fonts/codicon.a609dc0f.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    82216 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/fonts/ionicons.143146fa.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   197740 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/fonts/ionicons.99ac3308.woff
--rw-r--r--   0 runner    (1001) docker     (123)   197664 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/fonts/ionicons.d535a25a.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:32:36.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/img/
--rw-r--r--   0 runner    (1001) docker     (123)   555353 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/img/ionicons.a2c4a261.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:32:36.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/
--rw-r--r--   0 runner    (1001) docker     (123)    24092 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/app.6994bbbd.js
--rw-r--r--   0 runner    (1001) docker     (123)   704862 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-0b65ffb6.4d11c55b.js
--rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0a3577.e9944055.js
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0a43df.673ca57f.js
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0aa90c.bb4da71a.js
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0aab07.b30b422d.js
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0abc00.ae916ae6.js
--rw-r--r--   0 runner    (1001) docker     (123)    18269 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0ae937.5dfe330b.js
--rw-r--r--   0 runner    (1001) docker     (123)    18627 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0aeb45.d6889297.js
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0af08c.d2b0fda9.js
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0afa49.75ef7177.js
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0b2762.04d401e4.js
--rw-r--r--   0 runner    (1001) docker     (123)    17660 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0b6187.044b0232.js
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0ba136.3f3f68c3.js
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0bb267.de956ef3.js
--rw-r--r--   0 runner    (1001) docker     (123)    11812 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0bcec1.bb1e0dcf.js
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0bdf38.4ed8de90.js
--rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0bff92.0d3c28c2.js
--rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0c0494.089a3f44.js
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0c0a09.c01173ca.js
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0c4313.2d2e16b9.js
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0c46d1.1547c887.js
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0c512b.227874be.js
--rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0cf16e.d7823e95.js
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0d056d.50e40d69.js
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0d0645.00f3a9b7.js
--rw-r--r--   0 runner    (1001) docker     (123)    16969 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0d2f22.deddf49a.js
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0d61fd.c87f9452.js
--rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0d7e63.4e91911e.js
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0e1b57.2f0a463f.js
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0e1fbe.0fae86fb.js
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0e22d6.9822404b.js
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0e542a.00ed19f2.js
--rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0e57ec.9fc2995d.js
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0e6553.d113a072.js
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0e6c86.af95b5ef.js
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0ea098.47e7590e.js
--rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0f0a11.2c633a92.js
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d208ac5.2d741554.js
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d209408.fbdaeb7f.js
--rw-r--r--   0 runner    (1001) docker     (123)    14526 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d20f745.9eec45ed.js
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d20ff23.99d59ed8.js
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d2138c7.b8ff4f70.js
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d216f3b.7cfad27f.js
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d217e5b.b2ad3334.js
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d21b84a.59c92178.js
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d21dcd2.11000279.js
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d21f327.bb87e8ce.js
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d2214b3.ed0b709c.js
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d221799.af1ee392.js
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d221814.725c56d8.js
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d221a34.c98683c5.js
--rw-r--r--   0 runner    (1001) docker     (123)    22952 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d22502a.40401bee.js
--rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d226775.1ecaef90.js
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d229411.f42e99d7.js
--rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d2295e9.cf55c1f6.js
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d22c171.b06a7e37.js
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d22c2b8.160bc0cf.js
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d22ca58.01faff7d.js
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d2311f7.12260884.js
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d237ee7.6655aefa.js
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d238465.270fbbc6.js
--rw-r--r--   0 runner    (1001) docker     (123)   414560 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-30597b4a.ab012e90.js
--rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-7532b3ea.a9fe4911.js
--rw-r--r--   0 runner    (1001) docker     (123)   109437 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-e13e4362.9cc9d271.js
--rw-r--r--   0 runner    (1001) docker     (123)  3117005 2023-05-25 13:32:21.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-vendors.324e53e6.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:32:36.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/handlers/base_source_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/handlers/filter_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/handlers/import_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/handlers/result_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:32:36.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-05-25 13:32:36.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-05-25 13:32:36.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 13:32:36.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-25 13:32:36.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 13:32:36.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-25 13:32:36.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 13:32:36.000000 lyrebird-api-coverage-0.4.0/lyrebird_api_coverage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 13:32:36.000000 lyrebird-api-coverage-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-25 13:31:23.000000 lyrebird-api-coverage-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:21:34.000000 lyrebird-api-coverage-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-31 12:20:20.000000 lyrebird-api-coverage-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-05-31 12:21:34.000000 lyrebird-api-coverage-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-31 12:20:20.000000 lyrebird-api-coverage-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:21:34.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 12:20:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-31 12:20:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:21:34.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 12:20:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-31 12:20:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/client/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-31 12:20:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/client/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-31 12:20:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/client/event_subscibe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-31 12:20:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/client/filter_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-31 12:20:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/client/format_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-05-31 12:20:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/client/jsonscheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-31 12:20:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/client/load_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-05-31 12:20:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/client/merge_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-31 12:20:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/client/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-31 12:20:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/client/url_compare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:21:34.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/default_conf/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-31 12:20:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/default_conf/base.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-31 12:20:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/default_conf/conf.json
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-31 12:20:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/default_conf/filter_config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:21:34.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:21:34.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/css/app.964cc419.css
+-rw-r--r--   0 runner    (1001) docker     (123)   377184 2023-05-31 12:21:21.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/css/chunk-vendors.129fc3b2.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:21:34.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    56484 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/fonts/codicon.a609dc0f.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    82216 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/fonts/ionicons.143146fa.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   197740 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/fonts/ionicons.99ac3308.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   197664 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/fonts/ionicons.d535a25a.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:21:34.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/img/
+-rw-r--r--   0 runner    (1001) docker     (123)   555353 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/img/ionicons.a2c4a261.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:21:34.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    24092 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/app.6994bbbd.js
+-rw-r--r--   0 runner    (1001) docker     (123)   704862 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-0b65ffb6.4d11c55b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0a3577.e9944055.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0a43df.673ca57f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0aa90c.bb4da71a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0aab07.b30b422d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0abc00.ae916ae6.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18269 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0ae937.5dfe330b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18627 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0aeb45.d6889297.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0af08c.d2b0fda9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0afa49.75ef7177.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0b2762.04d401e4.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17660 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0b6187.044b0232.js
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0ba136.3f3f68c3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0bb267.de956ef3.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11812 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0bcec1.bb1e0dcf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0bdf38.4ed8de90.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0bff92.0d3c28c2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0c0494.089a3f44.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0c0a09.c01173ca.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0c4313.2d2e16b9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0c46d1.1547c887.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0c512b.227874be.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0cf16e.d7823e95.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0d056d.50e40d69.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0d0645.00f3a9b7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16969 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0d2f22.deddf49a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0d61fd.c87f9452.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0d7e63.4e91911e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0e1b57.2f0a463f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0e1fbe.0fae86fb.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0e22d6.9822404b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0e542a.00ed19f2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0e57ec.9fc2995d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0e6553.d113a072.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0e6c86.af95b5ef.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0ea098.47e7590e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0f0a11.2c633a92.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d208ac5.2d741554.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d209408.fbdaeb7f.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14526 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d20f745.9eec45ed.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d20ff23.99d59ed8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d2138c7.b8ff4f70.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d216f3b.7cfad27f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d217e5b.b2ad3334.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d21b84a.59c92178.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d21dcd2.11000279.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d21f327.bb87e8ce.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d2214b3.ed0b709c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d221799.af1ee392.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d221814.725c56d8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d221a34.c98683c5.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22952 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d22502a.40401bee.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5333 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d226775.1ecaef90.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d229411.f42e99d7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d2295e9.cf55c1f6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d22c171.b06a7e37.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-05-31 12:21:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d22c2b8.160bc0cf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-05-31 12:21:21.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d22ca58.01faff7d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-31 12:21:21.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d2311f7.12260884.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-05-31 12:21:21.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d237ee7.6655aefa.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-31 12:21:21.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d238465.270fbbc6.js
+-rw-r--r--   0 runner    (1001) docker     (123)   414560 2023-05-31 12:21:21.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-30597b4a.ab012e90.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-05-31 12:21:21.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-7532b3ea.a9fe4911.js
+-rw-r--r--   0 runner    (1001) docker     (123)   109437 2023-05-31 12:21:21.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-e13e4362.9cc9d271.js
+-rw-r--r--   0 runner    (1001) docker     (123)  3117005 2023-05-31 12:21:21.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-vendors.324e53e6.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:21:34.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 12:20:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-31 12:20:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/handlers/base_source_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-31 12:20:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/handlers/filter_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-31 12:20:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/handlers/import_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-05-31 12:20:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/handlers/result_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-05-31 12:20:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-31 12:20:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-31 12:20:20.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 12:21:34.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-05-31 12:21:33.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-05-31 12:21:34.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 12:21:33.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-31 12:21:33.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 12:21:33.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-31 12:21:33.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 12:21:33.000000 lyrebird-api-coverage-0.4.1/lyrebird_api_coverage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 12:21:34.000000 lyrebird-api-coverage-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-31 12:20:20.000000 lyrebird-api-coverage-0.4.1/setup.py
```

### Comparing `lyrebird-api-coverage-0.4.0/PKG-INFO` & `lyrebird-api-coverage-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyrebird-api-coverage
-Version: 0.4.0
+Version: 0.4.1
 Summary: UNKNOWN
 Home-page: https://github.com/meituan/lyrebird-api-coverage
 Author: HBQA
 License: UNKNOWN
 Description: # Lyrebird Plugin API-Coverage
         
         [![Build Status](https://travis-ci.org/meituan/lyrebird-api-coverage.svg?branch=master)](https://travis-ci.org/meituan/lyrebird-api-coverage)
```

### Comparing `lyrebird-api-coverage-0.4.0/README.md` & `lyrebird-api-coverage-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/api.py` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/api.py`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/client/config.py` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/client/config.py`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/client/context.py` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/client/context.py`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/client/filter_url.py` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/client/filter_url.py`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/client/format_url.py` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/client/format_url.py`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/client/jsonscheme.py` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/client/jsonscheme.py`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/client/load_base.py` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/client/load_base.py`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/client/merge_algorithm.py` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/client/merge_algorithm.py`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/client/report.py` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/client/report.py`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/client/url_compare.py` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/client/url_compare.py`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/css/chunk-vendors.129fc3b2.css` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/css/chunk-vendors.129fc3b2.css`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/fonts/codicon.a609dc0f.ttf` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/fonts/codicon.a609dc0f.ttf`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/fonts/ionicons.143146fa.woff2` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/fonts/ionicons.143146fa.woff2`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/fonts/ionicons.99ac3308.woff` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/fonts/ionicons.99ac3308.woff`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/fonts/ionicons.d535a25a.ttf` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/fonts/ionicons.d535a25a.ttf`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/img/ionicons.a2c4a261.svg` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/img/ionicons.a2c4a261.svg`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/index.html` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/index.html`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/app.6994bbbd.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/app.6994bbbd.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-0b65ffb6.4d11c55b.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-0b65ffb6.4d11c55b.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0a3577.e9944055.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0a3577.e9944055.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0a43df.673ca57f.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0a43df.673ca57f.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0aa90c.bb4da71a.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0aa90c.bb4da71a.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0aab07.b30b422d.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0aab07.b30b422d.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0abc00.ae916ae6.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0abc00.ae916ae6.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0ae937.5dfe330b.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0ae937.5dfe330b.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0aeb45.d6889297.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0aeb45.d6889297.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0af08c.d2b0fda9.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0af08c.d2b0fda9.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0afa49.75ef7177.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0afa49.75ef7177.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0b2762.04d401e4.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0b2762.04d401e4.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0b6187.044b0232.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0b6187.044b0232.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0ba136.3f3f68c3.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0ba136.3f3f68c3.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0bb267.de956ef3.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0bb267.de956ef3.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0bcec1.bb1e0dcf.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0bcec1.bb1e0dcf.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0bdf38.4ed8de90.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0bdf38.4ed8de90.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0bff92.0d3c28c2.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0bff92.0d3c28c2.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0c0494.089a3f44.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0c0494.089a3f44.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0c0a09.c01173ca.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0c0a09.c01173ca.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0c4313.2d2e16b9.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0c4313.2d2e16b9.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0c46d1.1547c887.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0c46d1.1547c887.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0c512b.227874be.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0c512b.227874be.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0cf16e.d7823e95.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0cf16e.d7823e95.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0d056d.50e40d69.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0d056d.50e40d69.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0d0645.00f3a9b7.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0d0645.00f3a9b7.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0d2f22.deddf49a.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0d2f22.deddf49a.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0d61fd.c87f9452.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0d61fd.c87f9452.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0d7e63.4e91911e.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0d7e63.4e91911e.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0e1b57.2f0a463f.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0e1b57.2f0a463f.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0e1fbe.0fae86fb.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0e1fbe.0fae86fb.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0e22d6.9822404b.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0e22d6.9822404b.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0e542a.00ed19f2.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0e542a.00ed19f2.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0e57ec.9fc2995d.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0e57ec.9fc2995d.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0e6553.d113a072.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0e6553.d113a072.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0e6c86.af95b5ef.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0e6c86.af95b5ef.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0ea098.47e7590e.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0ea098.47e7590e.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d0f0a11.2c633a92.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d0f0a11.2c633a92.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d208ac5.2d741554.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d208ac5.2d741554.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d209408.fbdaeb7f.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d209408.fbdaeb7f.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d20f745.9eec45ed.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d20f745.9eec45ed.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d20ff23.99d59ed8.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d20ff23.99d59ed8.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d2138c7.b8ff4f70.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d2138c7.b8ff4f70.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d216f3b.7cfad27f.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d216f3b.7cfad27f.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d217e5b.b2ad3334.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d217e5b.b2ad3334.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d21b84a.59c92178.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d21b84a.59c92178.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d21dcd2.11000279.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d21dcd2.11000279.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d21f327.bb87e8ce.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d21f327.bb87e8ce.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d2214b3.ed0b709c.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d2214b3.ed0b709c.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d221799.af1ee392.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d221799.af1ee392.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d221814.725c56d8.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d221814.725c56d8.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d221a34.c98683c5.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d221a34.c98683c5.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d22502a.40401bee.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d22502a.40401bee.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d226775.1ecaef90.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d226775.1ecaef90.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d229411.f42e99d7.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d229411.f42e99d7.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d2295e9.cf55c1f6.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d2295e9.cf55c1f6.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d22c171.b06a7e37.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d22c171.b06a7e37.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d22c2b8.160bc0cf.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d22c2b8.160bc0cf.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d22ca58.01faff7d.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d22ca58.01faff7d.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d2311f7.12260884.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d2311f7.12260884.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d237ee7.6655aefa.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d237ee7.6655aefa.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-2d238465.270fbbc6.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-2d238465.270fbbc6.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-30597b4a.ab012e90.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-30597b4a.ab012e90.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-7532b3ea.a9fe4911.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-7532b3ea.a9fe4911.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-e13e4362.9cc9d271.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-e13e4362.9cc9d271.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/dist/js/chunk-vendors.324e53e6.js` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/dist/js/chunk-vendors.324e53e6.js`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/handlers/base_source_handler.py` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/handlers/base_source_handler.py`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/handlers/filter_handler.py` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/handlers/filter_handler.py`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/handlers/import_file_handler.py` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/handlers/import_file_handler.py`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/handlers/result_handler.py` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/handlers/result_handler.py`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/interceptor.py` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/interceptor.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,22 +4,26 @@
 from lyrebird_api_coverage.client.context import app_context
 from lyrebird_api_coverage.client.merge_algorithm import mergeAlgorithm
 from lyrebird_api_coverage.client.report import report_worker
 from lyrebird_api_coverage.client.url_compare import compare_query
 from urllib.parse import urlparse
 
 logger = log.get_logger()
+block_list = application.config.get("apicoverage.block_list", [])
 import time
 
 def on_request(msg):
     req_starttime = time.time()
     req_msg = msg['flow']
     logger.debug(req_msg)
     if not msg['flow']['request']['url']:
         return
+    
+    if msg['flow']['request']['host'] in block_list:
+        return
 
     # 获取handler_context.id，为前端展开看详情准备
     path_id = msg['flow']['id']
     device_ip = msg['flow']['client_address']
     # 获取产品信息
     app_context.category = get_current_category(req_msg)
     if app_context.is_api_base_data:
@@ -43,40 +47,40 @@
         emit(req_starttime, path)
     # 如果path配置了对应的参数
     elif path in app_context.path_param_dic:
         ulr_list = app_context.path_param_dic[path]
         flag = 0
         for item in ulr_list:
             if compare_query(item['url'], msg['flow']['request']['url']):
-                mergeAlgorithm.merge_handler_new(item['url_base'], path_id)
+                mergeAlgorithm.merge_handler_new(item['url_base'], path_id, category)
                 mergeAlgorithm.coverage_handler()
                 report_worker(item['url_base'], device_ip, category)
                 flag = 1
         # 如果参数组合不存在，提取关注的字段
         if flag == 0:
             url_pgroup = ''
             params_list = []
             for item in ulr_list:
                 params_list.extend(item['params'].keys())
             # 去重
             for p in list(set(params_list)):
                 # Todo 这里在初始化之后看一下
-                val = msg['flow']['request']['query'][p]
+                val = msg['flow']['request']['query'].get(p)
                 if url_pgroup:
                     url_pgroup = url_pgroup + '&' + str(p) + '=' + str(val)
                 else:
                     url_pgroup = path + '?' + str(p) + '=' + str(val)
             mergeAlgorithm.merge_handler_new(url_pgroup, path_id, category)
             mergeAlgorithm.coverage_handler()
             report_worker(url_pgroup, device_ip, category)
         # 计算差值，指定时间间隔内只发1次io msg，限制刷新频率
         emit(req_starttime, path)
     # 如果不在base里，不需要merge到数据中
     else:
-        # mergeAlgorithm.merge_handler_new(path, path_id)
+        # mergeAlgorithm.merge_handler_new(path, path_id, category)
         # 进行上报
         report_worker(path, device_ip, category)
 
 def emit(starttime, path):
         duration = starttime - app_context.endtime
         if duration > app_context.SOCKET_PUSH_INTERVAL:
             app_context.endtime = starttime
```

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage/manifest.py` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage/manifest.py`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage.egg-info/PKG-INFO` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyrebird-api-coverage
-Version: 0.4.0
+Version: 0.4.1
 Summary: UNKNOWN
 Home-page: https://github.com/meituan/lyrebird-api-coverage
 Author: HBQA
 License: UNKNOWN
 Description: # Lyrebird Plugin API-Coverage
         
         [![Build Status](https://travis-ci.org/meituan/lyrebird-api-coverage.svg?branch=master)](https://travis-ci.org/meituan/lyrebird-api-coverage)
```

### Comparing `lyrebird-api-coverage-0.4.0/lyrebird_api_coverage.egg-info/SOURCES.txt` & `lyrebird-api-coverage-0.4.1/lyrebird_api_coverage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lyrebird-api-coverage-0.4.0/setup.py` & `lyrebird-api-coverage-0.4.1/setup.py`

 * *Files identical despite different names*

