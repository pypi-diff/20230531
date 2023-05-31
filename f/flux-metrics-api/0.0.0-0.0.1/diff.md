# Comparing `tmp/flux-metrics-api-0.0.0.tar.gz` & `tmp/flux-metrics-api-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flux-metrics-api-0.0.0.tar", last modified: Tue May 30 03:45:12 2023, max compression
+gzip compressed data, was "flux-metrics-api-0.0.1.tar", last modified: Wed May 31 04:49:57 2023, max compression
```

## Comparing `flux-metrics-api-0.0.0.tar` & `flux-metrics-api-0.0.1.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-30 03:45:12.205657 flux-metrics-api-0.0.0/
--rw-r--r--   0 vanessa   (1000) vanessa   (1000)      498 2023-05-30 01:03:44.000000 flux-metrics-api-0.0.0/COPYRIGHT
--rw-r--r--   0 vanessa   (1000) vanessa   (1000)     1108 2023-05-30 01:03:44.000000 flux-metrics-api-0.0.0/LICENSE
--rw-r--r--   0 vanessa   (1000) vanessa   (1000)      341 2023-05-30 01:23:07.000000 flux-metrics-api-0.0.0/MANIFEST.in
--rw-r--r--   0 vanessa   (1000) vanessa   (1000)     1167 2023-05-30 01:03:44.000000 flux-metrics-api-0.0.0/NOTICE
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5185 2023-05-30 03:45:12.205657 flux-metrics-api-0.0.0/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4358 2023-05-30 03:32:07.000000 flux-metrics-api-0.0.0/README.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-30 03:45:12.201657 flux-metrics-api-0.0.0/flux_metrics_api/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       69 2023-05-30 01:23:07.000000 flux-metrics-api-0.0.0/flux_metrics_api/__init__.py
--rw-r--r--   0 vanessa   (1000) vanessa   (1000)      293 2023-05-30 03:36:04.000000 flux-metrics-api-0.0.0/flux_metrics_api/defaults.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6127 2023-05-30 01:03:44.000000 flux-metrics-api-0.0.0/flux_metrics_api/logger.py
--rw-r--r--   0 vanessa   (1000) vanessa   (1000)     2151 2023-05-30 03:37:33.000000 flux-metrics-api-0.0.0/flux_metrics_api/metrics.py
--rw-r--r--   0 vanessa   (1000) vanessa   (1000)     2958 2023-05-30 03:36:46.000000 flux-metrics-api-0.0.0/flux_metrics_api/routes.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3832 2023-05-30 03:36:05.000000 flux-metrics-api-0.0.0/flux_metrics_api/server.py
--rw-r--r--   0 vanessa   (1000) vanessa   (1000)     1306 2023-05-30 03:36:04.000000 flux-metrics-api-0.0.0/flux_metrics_api/types.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      952 2023-05-30 01:23:59.000000 flux-metrics-api-0.0.0/flux_metrics_api/version.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-30 03:45:12.205657 flux-metrics-api-0.0.0/flux_metrics_api.egg-info/
--rw-r--r--   0 vanessa   (1000) vanessa   (1000)     5185 2023-05-30 03:45:12.000000 flux-metrics-api-0.0.0/flux_metrics_api.egg-info/PKG-INFO
--rw-r--r--   0 vanessa   (1000) vanessa   (1000)      582 2023-05-30 03:45:12.000000 flux-metrics-api-0.0.0/flux_metrics_api.egg-info/SOURCES.txt
--rw-r--r--   0 vanessa   (1000) vanessa   (1000)        1 2023-05-30 03:45:12.000000 flux-metrics-api-0.0.0/flux_metrics_api.egg-info/dependency_links.txt
--rw-r--r--   0 vanessa   (1000) vanessa   (1000)       67 2023-05-30 03:45:12.000000 flux-metrics-api-0.0.0/flux_metrics_api.egg-info/entry_points.txt
--rw-r--r--   0 vanessa   (1000) vanessa   (1000)        1 2023-05-30 02:17:12.000000 flux-metrics-api-0.0.0/flux_metrics_api.egg-info/not-zip-safe
--rw-r--r--   0 vanessa   (1000) vanessa   (1000)       43 2023-05-30 03:45:12.000000 flux-metrics-api-0.0.0/flux_metrics_api.egg-info/requires.txt
--rw-r--r--   0 vanessa   (1000) vanessa   (1000)       17 2023-05-30 03:45:12.000000 flux-metrics-api-0.0.0/flux_metrics_api.egg-info/top_level.txt
--rw-r--r--   0 vanessa   (1000) vanessa   (1000)      132 2023-05-30 01:03:44.000000 flux-metrics-api-0.0.0/pyproject.toml
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      413 2023-05-30 03:45:12.205657 flux-metrics-api-0.0.0/setup.cfg
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3483 2023-05-30 03:36:05.000000 flux-metrics-api-0.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:49:57.987536 flux-metrics-api-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-31 04:49:27.000000 flux-metrics-api-0.0.1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-31 04:49:27.000000 flux-metrics-api-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-31 04:49:27.000000 flux-metrics-api-0.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-31 04:49:27.000000 flux-metrics-api-0.0.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-05-31 04:49:57.987536 flux-metrics-api-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-05-31 04:49:27.000000 flux-metrics-api-0.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:49:57.983536 flux-metrics-api-0.0.1/flux_metrics_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-31 04:49:27.000000 flux-metrics-api-0.0.1/flux_metrics_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-31 04:49:27.000000 flux-metrics-api-0.0.1/flux_metrics_api/apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-31 04:49:27.000000 flux-metrics-api-0.0.1/flux_metrics_api/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-05-31 04:49:27.000000 flux-metrics-api-0.0.1/flux_metrics_api/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-31 04:49:27.000000 flux-metrics-api-0.0.1/flux_metrics_api/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-05-31 04:49:27.000000 flux-metrics-api-0.0.1/flux_metrics_api/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-05-31 04:49:27.000000 flux-metrics-api-0.0.1/flux_metrics_api/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-31 04:49:27.000000 flux-metrics-api-0.0.1/flux_metrics_api/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-31 04:49:27.000000 flux-metrics-api-0.0.1/flux_metrics_api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-31 04:49:27.000000 flux-metrics-api-0.0.1/flux_metrics_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:49:57.987536 flux-metrics-api-0.0.1/flux_metrics_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-05-31 04:49:57.000000 flux-metrics-api-0.0.1/flux_metrics_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-31 04:49:57.000000 flux-metrics-api-0.0.1/flux_metrics_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 04:49:57.000000 flux-metrics-api-0.0.1/flux_metrics_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-31 04:49:57.000000 flux-metrics-api-0.0.1/flux_metrics_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 04:49:57.000000 flux-metrics-api-0.0.1/flux_metrics_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-31 04:49:57.000000 flux-metrics-api-0.0.1/flux_metrics_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-31 04:49:57.000000 flux-metrics-api-0.0.1/flux_metrics_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-31 04:49:27.000000 flux-metrics-api-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-31 04:49:57.987536 flux-metrics-api-0.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-05-31 04:49:27.000000 flux-metrics-api-0.0.1/setup.py
```

### Comparing `flux-metrics-api-0.0.0/LICENSE` & `flux-metrics-api-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flux-metrics-api-0.0.0/NOTICE` & `flux-metrics-api-0.0.1/NOTICE`

 * *Files identical despite different names*

### Comparing `flux-metrics-api-0.0.0/PKG-INFO` & `flux-metrics-api-0.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: flux-metrics-api
-Version: 0.0.0
-Summary: Custom metrics exporter for Flux in Kubernetes
-Home-page: https://github.com/converged-computing/flux-metrics-api
-Author: Vanessa Sochat
-Author-email: vsoch@users.noreply.github.com
-Maintainer: Vanessa Sochat
-License: LICENSE
-Keywords: cloud,flux,flux-framework,monitoring
-Platform: UNKNOWN
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development
-Classifier: Topic :: Scientific/Engineering
-Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
-Provides-Extra: all
-License-File: LICENSE
-License-File: NOTICE
-
 # Flux Metrics API
 
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
 [![All Contributors](https://img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 [![PyPI](https://img.shields.io/pypi/v/flux-metrics-api)](https://pypi.org/project/flux-metrics-api/)
 
@@ -66,52 +42,72 @@
 
 You'll want to be running in a Flux instance, as we need to connect to the broker handle.
 
 ```bash
 $ flux start --test-size=4
 ```
 
-And then start the server. This will use a default port and host (0.0.0.0:8080) that you can customize
+And then start the server. This will use a default port and host (0.0.0.0:8443) that you can customize
 if desired.
 
 ```bash
 $ flux-metrics-api start
 
 # customize the port or host
 $ flux-metrics-api start --port 9000 --host 127.0.0.1
 ```
 
+If you want ssl (port 443) you can provide the path to a certificate and keyfile:
+
+```bash
+$ flux-metrics-api start --ssl-certfile /etc/certs/tls.crt --ssl-keyfile /etc/certs/tls.key
+```
+
+An example of a full command we might run from within a pod:
+
+```bash
+$ flux-metrics-api start --port 8443 --ssl-certfile /etc/certs/tls.crt --ssl-keyfile /etc/certs/tls.key --namespace flux-operator --service-name custom-metrics-apiserver
+```
+
 See `--help` to see other options available.
 
 ### Endpoints
 
 #### Metric
 
 **GET /apis/custom.metrics.k8s.io/v1beta2/namespaces/<namespace>/metrics/<metric_name>**
 
 Here is an example to get the "node_up_count" metric:
 
 ```bash
- curl -s http://localhost:8080/apis/custom.metrics.k8s.io/v1beta2/namespaces/flux-operator/metrics/node_up_count | jq
+ curl -s http://localhost:8443/apis/custom.metrics.k8s.io/v1beta2/namespaces/flux-operator/metrics/node_up_count | jq
 ```
 ```console
 {
   "items": [
     {
       "metric": {
         "name": "node_up_count"
       },
-      "value": 4,
-      "time": "",
+      "value": 2,
+      "timestamp": "2023-05-31T04:44:57+00:00",
       "windowSeconds": 0,
-      "describedObject": null
+      "describedObject": {
+        "kind": "Service",
+        "namespace": "flux-operator",
+        "name": "custom-metrics-apiserver",
+        "apiVersion": "v1beta2"
+      }
     }
   ],
   "apiVersion": "custom.metrics.k8s.io/v1beta2",
-  "kind": "MetricValueList"
+  "kind": "MetricValueList",
+  "metadata": {
+    "selfLink": "/apis/custom.metrics.k8s.io/v1beta2"
+  }
 }
 ```
 
 The following metrics are supported:
 
  - **node_up_count**: number of nodes up in the MiniCluster
  - **node_free_count**: number of nodes free in the MiniCluster
@@ -121,23 +117,28 @@
 ### Docker
 
 We have a docker container, which you can customize for your use case, but it's more intended to
 be a demo. You can either build it yourself, or use our build.
 
 ```bash
 $ docker build -t flux_metrics_api .
-$ docker run -it -p 8080:8080 flux_metrics_api
+$ docker run -it -p 8443:8443 flux_metrics_api
 ```
 or
 
 ```bash
-$ docker run -it -p 8080:8080 ghcr.io/converged-computing/flux-metrics-api
+$ docker run -it -p 8443:8443 ghcr.io/converged-computing/flux-metrics-api
 ```
 
-You can then open up the browser at [http://localhost:8080/metrics/](http://localhost:8080/metrics) to see
+### Development
+
+Note that this is implemented in Python, but (I found this after) we could [also use Go](https://github.com/kubernetes-sigs/custom-metrics-apiserver).
+Specifically, I found this repository useful to see the [spec format](https://github.com/kubernetes-sigs/custom-metrics-apiserver/blob/master/pkg/generated/openapi/custommetrics/zz_generated.openapi.go).
+
+You can then open up the browser at [http://localhost:8443/metrics/](http://localhost:8443/metrics) to see
 the metrics!
 
 ## 😁️ Contributors 😁️
 
 We use the [all-contributors](https://github.com/all-contributors/all-contributors)
 tool to generate a contributors graphic below.
 
@@ -165,9 +166,7 @@
 See [LICENSE](https://github.com/converged-computing/flux-metrics-api/blob/main/LICENSE),
 [COPYRIGHT](https://github.com/converged-computing/flux-metrics-api/blob/main/COPYRIGHT), and
 [NOTICE](https://github.com/converged-computing/flux-metrics-api/blob/main/NOTICE) for details.
 
 SPDX-License-Identifier: (MIT)
 
 LLNL-CODE- 842614
-
-
```

### Comparing `flux-metrics-api-0.0.0/README.md` & `flux-metrics-api-0.0.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,273 +1,389 @@
-00000000: 2320 466c 7578 204d 6574 7269 6373 2041  # Flux Metrics A
-00000010: 5049 0a0a 3c21 2d2d 2041 4c4c 2d43 4f4e  PI..<!-- ALL-CON
-00000020: 5452 4942 5554 4f52 532d 4241 4447 453a  TRIBUTORS-BADGE:
-00000030: 5354 4152 5420 2d20 446f 206e 6f74 2072  START - Do not r
-00000040: 656d 6f76 6520 6f72 206d 6f64 6966 7920  emove or modify 
-00000050: 7468 6973 2073 6563 7469 6f6e 202d 2d3e  this section -->
-00000060: 0a5b 215b 416c 6c20 436f 6e74 7269 6275  .[![All Contribu
-00000070: 746f 7273 5d28 6874 7470 733a 2f2f 696d  tors](https://im
-00000080: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-00000090: 6765 2f61 6c6c 5f63 6f6e 7472 6962 7574  ge/all_contribut
-000000a0: 6f72 732d 312d 6f72 616e 6765 2e73 7667  ors-1-orange.svg
-000000b0: 3f73 7479 6c65 3d66 6c61 742d 7371 7561  ?style=flat-squa
-000000c0: 7265 295d 2823 636f 6e74 7269 6275 746f  re)](#contributo
-000000d0: 7273 2d29 0a3c 212d 2d20 414c 4c2d 434f  rs-).<!-- ALL-CO
-000000e0: 4e54 5249 4255 544f 5253 2d42 4144 4745  NTRIBUTORS-BADGE
-000000f0: 3a45 4e44 202d 2d3e 0a5b 215b 5079 5049  :END -->.[![PyPI
-00000100: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-00000110: 6965 6c64 732e 696f 2f70 7970 692f 762f  ields.io/pypi/v/
-00000120: 666c 7578 2d6d 6574 7269 6373 2d61 7069  flux-metrics-api
-00000130: 295d 2868 7474 7073 3a2f 2f70 7970 692e  )](https://pypi.
-00000140: 6f72 672f 7072 6f6a 6563 742f 666c 7578  org/project/flux
-00000150: 2d6d 6574 7269 6373 2d61 7069 2f29 0a0a  -metrics-api/)..
-00000160: 5468 6973 2069 7320 616e 2065 7870 6572  This is an exper
-00000170: 696d 656e 7420 746f 2063 7265 6174 6520  iment to create 
-00000180: 6120 6d65 7472 6963 7320 4150 4920 666f  a metrics API fo
-00000190: 7220 4b75 6265 726e 6574 6573 2074 6861  r Kubernetes tha
-000001a0: 7420 6361 6e20 6265 2072 756e 2064 6972  t can be run dir
-000001b0: 6563 746c 7920 6672 6f6d 2074 6865 2046  ectly from the F
-000001c0: 6c75 780a 6c65 6164 6572 2062 726f 6b65  lux.leader broke
-000001d0: 7220 706f 642e 2057 6520 6d61 6465 2074  r pod. We made t
-000001e0: 6869 7320 6166 7465 7220 6372 6561 7469  his after creati
-000001f0: 6e67 205b 7072 6f6d 6574 6865 7573 2d66  ng [prometheus-f
-00000200: 6c75 785d 2868 7474 7073 3a2f 2f67 6974  lux](https://git
-00000210: 6875 622e 636f 6d2f 636f 6e76 6572 6765  hub.com/converge
-00000220: 642d 636f 6d70 7574 696e 672f 7072 6f6d  d-computing/prom
-00000230: 6574 6865 7573 2d66 6c75 7829 0a61 6e64  etheus-flux).and
-00000240: 2077 616e 7469 6e67 2061 206d 6f72 6520   wanting a more 
-00000250: 6d69 6e69 6d61 6c69 7374 2064 6573 6967  minimalist desig
-00000260: 6e2e 2049 276d 206e 6f74 2065 7665 6e20  n. I'm not even 
-00000270: 7375 7265 2069 7420 7769 6c6c 2077 6f72  sure it will wor
-00000280: 6b2c 2062 7574 2069 7427 7320 776f 7274  k, but it's wort
-00000290: 6820 6120 7472 7921 0a0a 2323 2055 7361  h a try!..## Usa
-000002a0: 6765 0a0a 2323 2320 496e 7374 616c 6c0a  ge..### Install.
-000002b0: 0a59 6f75 2063 616e 2069 6e73 7461 6c6c  .You can install
-000002c0: 2066 726f 6d20 7079 7069 206f 7220 6672   from pypi or fr
-000002d0: 6f6d 2073 6f75 7263 653a 0a0a 6060 6062  om source:..```b
-000002e0: 6173 680a 2420 7079 7468 6f6e 202d 6d20  ash.$ python -m 
-000002f0: 7665 6e76 2065 6e76 0a24 2073 6f75 7263  venv env.$ sourc
-00000300: 6520 656e 762f 6269 6e2f 6163 7469 7661  e env/bin/activa
-00000310: 7465 0a24 2070 6970 2069 6e73 7461 6c6c  te.$ pip install
-00000320: 2066 6c75 782d 6d65 7472 6963 732d 6170   flux-metrics-ap
-00000330: 690a 0a23 206f 720a 0a24 2067 6974 2063  i..# or..$ git c
-00000340: 6c6f 6e65 2068 7474 7073 3a2f 2f67 6974  lone https://git
-00000350: 6875 622e 636f 6d2f 636f 6e76 6572 6765  hub.com/converge
-00000360: 642d 636f 6d70 7574 696e 672f 666c 7578  d-computing/flux
-00000370: 2d6d 6574 7269 6373 2d61 7069 0a24 2063  -metrics-api.$ c
-00000380: 6420 666c 7578 2d6d 6574 7269 6373 2d61  d flux-metrics-a
-00000390: 7069 0a24 2070 6970 2069 6e73 7461 6c6c  pi.$ pip install
-000003a0: 202e 0a23 2079 6f75 2063 616e 2061 6c73   ..# you can als
-000003b0: 6f20 646f 2022 7069 7020 696e 7374 616c  o do "pip instal
-000003c0: 6c20 2d65 202e 220a 6060 600a 0a54 6869  l -e .".```..Thi
-000003d0: 7320 7769 6c6c 2069 6e73 7461 6c6c 2074  s will install t
-000003e0: 6865 2065 7865 6375 7461 626c 6520 746f  he executable to
-000003f0: 2079 6f75 7220 7061 7468 2c20 7768 6963   your path, whic
-00000400: 6820 6d69 6768 7420 6265 2079 6f75 7220  h might be your 
-00000410: 6c6f 6361 6c20 7573 6572 2062 696e 3a0a  local user bin:.
-00000420: 0a60 6060 6261 7368 0a24 2077 6869 6368  .```bash.$ which
-00000430: 2066 6c75 782d 6d65 7472 6963 2d61 7069   flux-metric-api
-00000440: 0a2f 686f 6d65 2f76 7363 6f64 652f 2e6c  ./home/vscode/.l
-00000450: 6f63 616c 2f62 696e 2f66 6c75 782d 6d65  ocal/bin/flux-me
-00000460: 7472 6963 732d 6170 690a 6060 600a 0a4e  trics-api.```..N
-00000470: 6f74 6520 7468 6174 2074 6865 2070 726f  ote that the pro
-00000480: 7669 6465 6420 5b2e 6465 7663 6f6e 7461  vided [.devconta
-00000490: 696e 6572 5d28 2e64 6576 636f 6e74 6169  iner](.devcontai
-000004a0: 6e65 7229 2069 6e63 6c75 6465 7320 616e  ner) includes an
-000004b0: 2065 6e76 6972 6f6e 6d65 6e74 2066 6f72   environment for
-000004c0: 2056 5343 6f64 6520 7768 6572 6520 796f   VSCode where yo
-000004d0: 7520 6861 7665 2046 6c75 780a 616e 6420  u have Flux.and 
-000004e0: 6361 6e20 696e 7374 616c 6c20 7468 6973  can install this
-000004f0: 2061 6e64 2075 7365 2072 6561 6479 2074   and use ready t
-00000500: 6f20 676f 210a 0a23 2323 2053 7461 7274  o go!..### Start
-00000510: 0a0a 596f 7527 6c6c 2077 616e 7420 746f  ..You'll want to
-00000520: 2062 6520 7275 6e6e 696e 6720 696e 2061   be running in a
-00000530: 2046 6c75 7820 696e 7374 616e 6365 2c20   Flux instance, 
-00000540: 6173 2077 6520 6e65 6564 2074 6f20 636f  as we need to co
-00000550: 6e6e 6563 7420 746f 2074 6865 2062 726f  nnect to the bro
-00000560: 6b65 7220 6861 6e64 6c65 2e0a 0a60 6060  ker handle...```
-00000570: 6261 7368 0a24 2066 6c75 7820 7374 6172  bash.$ flux star
-00000580: 7420 2d2d 7465 7374 2d73 697a 653d 340a  t --test-size=4.
-00000590: 6060 600a 0a41 6e64 2074 6865 6e20 7374  ```..And then st
-000005a0: 6172 7420 7468 6520 7365 7276 6572 2e20  art the server. 
-000005b0: 5468 6973 2077 696c 6c20 7573 6520 6120  This will use a 
-000005c0: 6465 6661 756c 7420 706f 7274 2061 6e64  default port and
-000005d0: 2068 6f73 7420 2830 2e30 2e30 2e30 3a38   host (0.0.0.0:8
-000005e0: 3038 3029 2074 6861 7420 796f 7520 6361  080) that you ca
-000005f0: 6e20 6375 7374 6f6d 697a 650a 6966 2064  n customize.if d
-00000600: 6573 6972 6564 2e0a 0a60 6060 6261 7368  esired...```bash
-00000610: 0a24 2066 6c75 782d 6d65 7472 6963 732d  .$ flux-metrics-
-00000620: 6170 6920 7374 6172 740a 0a23 2063 7573  api start..# cus
-00000630: 746f 6d69 7a65 2074 6865 2070 6f72 7420  tomize the port 
-00000640: 6f72 2068 6f73 740a 2420 666c 7578 2d6d  or host.$ flux-m
-00000650: 6574 7269 6373 2d61 7069 2073 7461 7274  etrics-api start
-00000660: 202d 2d70 6f72 7420 3930 3030 202d 2d68   --port 9000 --h
-00000670: 6f73 7420 3132 372e 302e 302e 310a 6060  ost 127.0.0.1.``
-00000680: 600a 0a53 6565 2060 2d2d 6865 6c70 6020  `..See `--help` 
-00000690: 746f 2073 6565 206f 7468 6572 206f 7074  to see other opt
-000006a0: 696f 6e73 2061 7661 696c 6162 6c65 2e0a  ions available..
-000006b0: 0a23 2323 2045 6e64 706f 696e 7473 0a0a  .### Endpoints..
-000006c0: 2323 2323 204d 6574 7269 630a 0a2a 2a47  #### Metric..**G
-000006d0: 4554 202f 6170 6973 2f63 7573 746f 6d2e  ET /apis/custom.
-000006e0: 6d65 7472 6963 732e 6b38 732e 696f 2f76  metrics.k8s.io/v
-000006f0: 3162 6574 6132 2f6e 616d 6573 7061 6365  1beta2/namespace
-00000700: 732f 3c6e 616d 6573 7061 6365 3e2f 6d65  s/<namespace>/me
-00000710: 7472 6963 732f 3c6d 6574 7269 635f 6e61  trics/<metric_na
-00000720: 6d65 3e2a 2a0a 0a48 6572 6520 6973 2061  me>**..Here is a
-00000730: 6e20 6578 616d 706c 6520 746f 2067 6574  n example to get
-00000740: 2074 6865 2022 6e6f 6465 5f75 705f 636f   the "node_up_co
-00000750: 756e 7422 206d 6574 7269 633a 0a0a 6060  unt" metric:..``
-00000760: 6062 6173 680a 2063 7572 6c20 2d73 2068  `bash. curl -s h
-00000770: 7474 703a 2f2f 6c6f 6361 6c68 6f73 743a  ttp://localhost:
-00000780: 3830 3830 2f61 7069 732f 6375 7374 6f6d  8080/apis/custom
-00000790: 2e6d 6574 7269 6373 2e6b 3873 2e69 6f2f  .metrics.k8s.io/
-000007a0: 7631 6265 7461 322f 6e61 6d65 7370 6163  v1beta2/namespac
-000007b0: 6573 2f66 6c75 782d 6f70 6572 6174 6f72  es/flux-operator
-000007c0: 2f6d 6574 7269 6373 2f6e 6f64 655f 7570  /metrics/node_up
-000007d0: 5f63 6f75 6e74 207c 206a 710a 6060 600a  _count | jq.```.
-000007e0: 6060 6063 6f6e 736f 6c65 0a7b 0a20 2022  ```console.{.  "
-000007f0: 6974 656d 7322 3a20 5b0a 2020 2020 7b0a  items": [.    {.
-00000800: 2020 2020 2020 226d 6574 7269 6322 3a20        "metric": 
-00000810: 7b0a 2020 2020 2020 2020 226e 616d 6522  {.        "name"
-00000820: 3a20 226e 6f64 655f 7570 5f63 6f75 6e74  : "node_up_count
-00000830: 220a 2020 2020 2020 7d2c 0a20 2020 2020  ".      },.     
-00000840: 2022 7661 6c75 6522 3a20 342c 0a20 2020   "value": 4,.   
-00000850: 2020 2022 7469 6d65 223a 2022 222c 0a20     "time": "",. 
-00000860: 2020 2020 2022 7769 6e64 6f77 5365 636f       "windowSeco
-00000870: 6e64 7322 3a20 302c 0a20 2020 2020 2022  nds": 0,.      "
-00000880: 6465 7363 7269 6265 644f 626a 6563 7422  describedObject"
-00000890: 3a20 6e75 6c6c 0a20 2020 207d 0a20 205d  : null.    }.  ]
-000008a0: 2c0a 2020 2261 7069 5665 7273 696f 6e22  ,.  "apiVersion"
-000008b0: 3a20 2263 7573 746f 6d2e 6d65 7472 6963  : "custom.metric
-000008c0: 732e 6b38 732e 696f 2f76 3162 6574 6132  s.k8s.io/v1beta2
-000008d0: 222c 0a20 2022 6b69 6e64 223a 2022 4d65  ",.  "kind": "Me
-000008e0: 7472 6963 5661 6c75 654c 6973 7422 0a7d  tricValueList".}
-000008f0: 0a60 6060 0a0a 5468 6520 666f 6c6c 6f77  .```..The follow
-00000900: 696e 6720 6d65 7472 6963 7320 6172 6520  ing metrics are 
-00000910: 7375 7070 6f72 7465 643a 0a0a 202d 202a  supported:.. - *
-00000920: 2a6e 6f64 655f 7570 5f63 6f75 6e74 2a2a  *node_up_count**
-00000930: 3a20 6e75 6d62 6572 206f 6620 6e6f 6465  : number of node
-00000940: 7320 7570 2069 6e20 7468 6520 4d69 6e69  s up in the Mini
-00000950: 436c 7573 7465 720a 202d 202a 2a6e 6f64  Cluster. - **nod
-00000960: 655f 6672 6565 5f63 6f75 6e74 2a2a 3a20  e_free_count**: 
-00000970: 6e75 6d62 6572 206f 6620 6e6f 6465 7320  number of nodes 
-00000980: 6672 6565 2069 6e20 7468 6520 4d69 6e69  free in the Mini
-00000990: 436c 7573 7465 720a 202d 202a 2a6e 6f64  Cluster. - **nod
-000009a0: 655f 636f 7265 735f 6672 6565 5f63 6f75  e_cores_free_cou
-000009b0: 6e74 2a2a 3a20 6e75 6d62 6572 206f 6620  nt**: number of 
-000009c0: 6e6f 6465 2063 6f72 6573 2066 7265 6520  node cores free 
-000009d0: 696e 2074 6865 204d 696e 6943 6c75 7374  in the MiniClust
-000009e0: 6572 0a20 2d20 2a2a 6e6f 6465 5f63 6f72  er. - **node_cor
-000009f0: 6573 5f75 705f 636f 756e 742a 2a3a 206e  es_up_count**: n
-00000a00: 756d 6265 7220 6f66 206e 6f64 6520 636f  umber of node co
-00000a10: 7265 7320 7570 2069 6e20 7468 6520 4d69  res up in the Mi
-00000a20: 6e69 436c 7573 7465 720a 0a23 2323 2044  niCluster..### D
-00000a30: 6f63 6b65 720a 0a57 6520 6861 7665 2061  ocker..We have a
-00000a40: 2064 6f63 6b65 7220 636f 6e74 6169 6e65   docker containe
-00000a50: 722c 2077 6869 6368 2079 6f75 2063 616e  r, which you can
-00000a60: 2063 7573 746f 6d69 7a65 2066 6f72 2079   customize for y
-00000a70: 6f75 7220 7573 6520 6361 7365 2c20 6275  our use case, bu
-00000a80: 7420 6974 2773 206d 6f72 6520 696e 7465  t it's more inte
-00000a90: 6e64 6564 2074 6f0a 6265 2061 2064 656d  nded to.be a dem
-00000aa0: 6f2e 2059 6f75 2063 616e 2065 6974 6865  o. You can eithe
-00000ab0: 7220 6275 696c 6420 6974 2079 6f75 7273  r build it yours
-00000ac0: 656c 662c 206f 7220 7573 6520 6f75 7220  elf, or use our 
-00000ad0: 6275 696c 642e 0a0a 6060 6062 6173 680a  build...```bash.
-00000ae0: 2420 646f 636b 6572 2062 7569 6c64 202d  $ docker build -
-00000af0: 7420 666c 7578 5f6d 6574 7269 6373 5f61  t flux_metrics_a
-00000b00: 7069 202e 0a24 2064 6f63 6b65 7220 7275  pi ..$ docker ru
-00000b10: 6e20 2d69 7420 2d70 2038 3038 303a 3830  n -it -p 8080:80
-00000b20: 3830 2066 6c75 785f 6d65 7472 6963 735f  80 flux_metrics_
-00000b30: 6170 690a 6060 600a 6f72 0a0a 6060 6062  api.```.or..```b
-00000b40: 6173 680a 2420 646f 636b 6572 2072 756e  ash.$ docker run
-00000b50: 202d 6974 202d 7020 3830 3830 3a38 3038   -it -p 8080:808
-00000b60: 3020 6768 6372 2e69 6f2f 636f 6e76 6572  0 ghcr.io/conver
-00000b70: 6765 642d 636f 6d70 7574 696e 672f 666c  ged-computing/fl
-00000b80: 7578 2d6d 6574 7269 6373 2d61 7069 0a60  ux-metrics-api.`
-00000b90: 6060 0a0a 596f 7520 6361 6e20 7468 656e  ``..You can then
-00000ba0: 206f 7065 6e20 7570 2074 6865 2062 726f   open up the bro
-00000bb0: 7773 6572 2061 7420 5b68 7474 703a 2f2f  wser at [http://
-00000bc0: 6c6f 6361 6c68 6f73 743a 3830 3830 2f6d  localhost:8080/m
-00000bd0: 6574 7269 6373 2f5d 2868 7474 703a 2f2f  etrics/](http://
-00000be0: 6c6f 6361 6c68 6f73 743a 3830 3830 2f6d  localhost:8080/m
-00000bf0: 6574 7269 6373 2920 746f 2073 6565 0a74  etrics) to see.t
-00000c00: 6865 206d 6574 7269 6373 210a 0a23 2320  he metrics!..## 
-00000c10: f09f 9881 efb8 8f20 436f 6e74 7269 6275  ....... Contribu
-00000c20: 746f 7273 20f0 9f98 81ef b88f 0a0a 5765  tors .........We
-00000c30: 2075 7365 2074 6865 205b 616c 6c2d 636f   use the [all-co
-00000c40: 6e74 7269 6275 746f 7273 5d28 6874 7470  ntributors](http
-00000c50: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f61  s://github.com/a
-00000c60: 6c6c 2d63 6f6e 7472 6962 7574 6f72 732f  ll-contributors/
-00000c70: 616c 6c2d 636f 6e74 7269 6275 746f 7273  all-contributors
-00000c80: 290a 746f 6f6c 2074 6f20 6765 6e65 7261  ).tool to genera
-00000c90: 7465 2061 2063 6f6e 7472 6962 7574 6f72  te a contributor
-00000ca0: 7320 6772 6170 6869 6320 6265 6c6f 772e  s graphic below.
-00000cb0: 0a0a 3c21 2d2d 2041 4c4c 2d43 4f4e 5452  ..<!-- ALL-CONTR
-00000cc0: 4942 5554 4f52 532d 4c49 5354 3a53 5441  IBUTORS-LIST:STA
-00000cd0: 5254 202d 2044 6f20 6e6f 7420 7265 6d6f  RT - Do not remo
-00000ce0: 7665 206f 7220 6d6f 6469 6679 2074 6869  ve or modify thi
-00000cf0: 7320 7365 6374 696f 6e20 2d2d 3e0a 3c21  s section -->.<!
-00000d00: 2d2d 2070 7265 7474 6965 722d 6967 6e6f  -- prettier-igno
-00000d10: 7265 2d73 7461 7274 202d 2d3e 0a3c 212d  re-start -->.<!-
-00000d20: 2d20 6d61 726b 646f 776e 6c69 6e74 2d64  - markdownlint-d
-00000d30: 6973 6162 6c65 202d 2d3e 0a3c 7461 626c  isable -->.<tabl
-00000d40: 653e 0a20 203c 7462 6f64 793e 0a20 2020  e>.  <tbody>.   
-00000d50: 203c 7472 3e0a 2020 2020 2020 3c74 6420   <tr>.      <td 
-00000d60: 616c 6967 6e3d 2263 656e 7465 7222 2076  align="center" v
-00000d70: 616c 6967 6e3d 2274 6f70 2220 7769 6474  align="top" widt
-00000d80: 683d 2231 342e 3238 2522 3e3c 6120 6872  h="14.28%"><a hr
-00000d90: 6566 3d22 6874 7470 733a 2f2f 7673 6f63  ef="https://vsoc
-00000da0: 682e 6769 7468 7562 2e69 6f22 3e3c 696d  h.github.io"><im
-00000db0: 6720 7372 633d 2268 7474 7073 3a2f 2f61  g src="https://a
-00000dc0: 7661 7461 7273 2e67 6974 6875 6275 7365  vatars.githubuse
-00000dd0: 7263 6f6e 7465 6e74 2e63 6f6d 2f75 2f38  rcontent.com/u/8
-00000de0: 3134 3332 323f 763d 343f 733d 3130 3022  14322?v=4?s=100"
-00000df0: 2077 6964 7468 3d22 3130 3070 783b 2220   width="100px;" 
-00000e00: 616c 743d 2256 616e 6573 7361 7361 7572  alt="Vanessasaur
-00000e10: 7573 222f 3e3c 6272 202f 3e3c 7375 623e  us"/><br /><sub>
-00000e20: 3c62 3e56 616e 6573 7361 7361 7572 7573  <b>Vanessasaurus
-00000e30: 3c2f 623e 3c2f 7375 623e 3c2f 613e 3c62  </b></sub></a><b
-00000e40: 7220 2f3e 3c61 2068 7265 663d 2268 7474  r /><a href="htt
-00000e50: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000e60: 636f 6e76 6572 6765 642d 636f 6d70 7574  converged-comput
-00000e70: 696e 672f 666c 7578 2d6d 6574 7269 6373  ing/flux-metrics
-00000e80: 2d61 7069 2f63 6f6d 6d69 7473 3f61 7574  -api/commits?aut
-00000e90: 686f 723d 7673 6f63 6822 2074 6974 6c65  hor=vsoch" title
-00000ea0: 3d22 436f 6465 223e f09f 92bb 3c2f 613e  ="Code">....</a>
-00000eb0: 3c2f 7464 3e0a 2020 2020 3c2f 7472 3e0a  </td>.    </tr>.
-00000ec0: 2020 3c2f 7462 6f64 793e 0a3c 2f74 6162    </tbody>.</tab
-00000ed0: 6c65 3e0a 0a3c 212d 2d20 6d61 726b 646f  le>..<!-- markdo
-00000ee0: 776e 6c69 6e74 2d72 6573 746f 7265 202d  wnlint-restore -
-00000ef0: 2d3e 0a3c 212d 2d20 7072 6574 7469 6572  ->.<!-- prettier
-00000f00: 2d69 676e 6f72 652d 656e 6420 2d2d 3e0a  -ignore-end -->.
-00000f10: 0a3c 212d 2d20 414c 4c2d 434f 4e54 5249  .<!-- ALL-CONTRI
-00000f20: 4255 544f 5253 2d4c 4953 543a 454e 4420  BUTORS-LIST:END 
-00000f30: 2d2d 3e0a 0a23 2320 4c69 6365 6e73 650a  -->..## License.
-00000f40: 0a48 5043 4943 2044 6576 546f 6f6c 7320  .HPCIC DevTools 
-00000f50: 6973 2064 6973 7472 6962 7574 6564 2075  is distributed u
-00000f60: 6e64 6572 2074 6865 2074 6572 6d73 206f  nder the terms o
-00000f70: 6620 7468 6520 4d49 5420 6c69 6365 6e73  f the MIT licens
-00000f80: 652e 0a41 6c6c 206e 6577 2063 6f6e 7472  e..All new contr
-00000f90: 6962 7574 696f 6e73 206d 7573 7420 6265  ibutions must be
-00000fa0: 206d 6164 6520 756e 6465 7220 7468 6973   made under this
-00000fb0: 206c 6963 656e 7365 2e0a 0a53 6565 205b   license...See [
-00000fc0: 4c49 4345 4e53 455d 2868 7474 7073 3a2f  LICENSE](https:/
-00000fd0: 2f67 6974 6875 622e 636f 6d2f 636f 6e76  /github.com/conv
-00000fe0: 6572 6765 642d 636f 6d70 7574 696e 672f  erged-computing/
-00000ff0: 666c 7578 2d6d 6574 7269 6373 2d61 7069  flux-metrics-api
-00001000: 2f62 6c6f 622f 6d61 696e 2f4c 4943 454e  /blob/main/LICEN
-00001010: 5345 292c 0a5b 434f 5059 5249 4748 545d  SE),.[COPYRIGHT]
-00001020: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00001030: 636f 6d2f 636f 6e76 6572 6765 642d 636f  com/converged-co
-00001040: 6d70 7574 696e 672f 666c 7578 2d6d 6574  mputing/flux-met
-00001050: 7269 6373 2d61 7069 2f62 6c6f 622f 6d61  rics-api/blob/ma
-00001060: 696e 2f43 4f50 5952 4947 4854 292c 2061  in/COPYRIGHT), a
-00001070: 6e64 0a5b 4e4f 5449 4345 5d28 6874 7470  nd.[NOTICE](http
-00001080: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f63  s://github.com/c
-00001090: 6f6e 7665 7267 6564 2d63 6f6d 7075 7469  onverged-computi
-000010a0: 6e67 2f66 6c75 782d 6d65 7472 6963 732d  ng/flux-metrics-
-000010b0: 6170 692f 626c 6f62 2f6d 6169 6e2f 4e4f  api/blob/main/NO
-000010c0: 5449 4345 2920 666f 7220 6465 7461 696c  TICE) for detail
-000010d0: 732e 0a0a 5350 4458 2d4c 6963 656e 7365  s...SPDX-License
-000010e0: 2d49 6465 6e74 6966 6965 723a 2028 4d49  -Identifier: (MI
-000010f0: 5429 0a0a 4c4c 4e4c 2d43 4f44 452d 2038  T)..LLNL-CODE- 8
-00001100: 3432 3631 340a                           42614.
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 666c 7578  : 2.1.Name: flux
+00000020: 2d6d 6574 7269 6373 2d61 7069 0a56 6572  -metrics-api.Ver
+00000030: 7369 6f6e 3a20 302e 302e 310a 5375 6d6d  sion: 0.0.1.Summ
+00000040: 6172 793a 2043 7573 746f 6d20 6d65 7472  ary: Custom metr
+00000050: 6963 7320 6578 706f 7274 6572 2066 6f72  ics exporter for
+00000060: 2046 6c75 7820 696e 204b 7562 6572 6e65   Flux in Kuberne
+00000070: 7465 730a 486f 6d65 2d70 6167 653a 2068  tes.Home-page: h
+00000080: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000090: 6d2f 636f 6e76 6572 6765 642d 636f 6d70  m/converged-comp
+000000a0: 7574 696e 672f 666c 7578 2d6d 6574 7269  uting/flux-metri
+000000b0: 6373 2d61 7069 0a41 7574 686f 723a 2056  cs-api.Author: V
+000000c0: 616e 6573 7361 2053 6f63 6861 740a 4175  anessa Sochat.Au
+000000d0: 7468 6f72 2d65 6d61 696c 3a20 7673 6f63  thor-email: vsoc
+000000e0: 6840 7573 6572 732e 6e6f 7265 706c 792e  h@users.noreply.
+000000f0: 6769 7468 7562 2e63 6f6d 0a4d 6169 6e74  github.com.Maint
+00000100: 6169 6e65 723a 2056 616e 6573 7361 2053  ainer: Vanessa S
+00000110: 6f63 6861 740a 4c69 6365 6e73 653a 204c  ochat.License: L
+00000120: 4943 454e 5345 0a4b 6579 776f 7264 733a  ICENSE.Keywords:
+00000130: 2063 6c6f 7564 2c66 6c75 782c 666c 7578   cloud,flux,flux
+00000140: 2d66 7261 6d65 776f 726b 2c6d 6f6e 6974  -framework,monit
+00000150: 6f72 696e 670a 436c 6173 7369 6669 6572  oring.Classifier
+00000160: 3a20 496e 7465 6e64 6564 2041 7564 6965  : Intended Audie
+00000170: 6e63 6520 3a3a 2053 6369 656e 6365 2f52  nce :: Science/R
+00000180: 6573 6561 7263 680a 436c 6173 7369 6669  esearch.Classifi
+00000190: 6572 3a20 496e 7465 6e64 6564 2041 7564  er: Intended Aud
+000001a0: 6965 6e63 6520 3a3a 2044 6576 656c 6f70  ience :: Develop
+000001b0: 6572 730a 436c 6173 7369 6669 6572 3a20  ers.Classifier: 
+000001c0: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
+000001d0: 7070 726f 7665 6420 3a3a 204d 4954 204c  pproved :: MIT L
+000001e0: 6963 656e 7365 0a43 6c61 7373 6966 6965  icense.Classifie
+000001f0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+00000200: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000210: 6e0a 436c 6173 7369 6669 6572 3a20 546f  n.Classifier: To
+00000220: 7069 6320 3a3a 2053 6f66 7477 6172 6520  pic :: Software 
+00000230: 4465 7665 6c6f 706d 656e 740a 436c 6173  Development.Clas
+00000240: 7369 6669 6572 3a20 546f 7069 6320 3a3a  sifier: Topic ::
+00000250: 2053 6369 656e 7469 6669 632f 456e 6769   Scientific/Engi
+00000260: 6e65 6572 696e 670a 436c 6173 7369 6669  neering.Classifi
+00000270: 6572 3a20 4f70 6572 6174 696e 6720 5379  er: Operating Sy
+00000280: 7374 656d 203a 3a20 556e 6978 0a43 6c61  stem :: Unix.Cla
+00000290: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+000002a0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000002b0: 2050 7974 686f 6e20 3a3a 2033 2e38 0a44   Python :: 3.8.D
+000002c0: 6573 6372 6970 7469 6f6e 2d43 6f6e 7465  escription-Conte
+000002d0: 6e74 2d54 7970 653a 2074 6578 742f 6d61  nt-Type: text/ma
+000002e0: 726b 646f 776e 0a50 726f 7669 6465 732d  rkdown.Provides-
+000002f0: 4578 7472 613a 2061 6c6c 0a4c 6963 656e  Extra: all.Licen
+00000300: 7365 2d46 696c 653a 204c 4943 454e 5345  se-File: LICENSE
+00000310: 0a4c 6963 656e 7365 2d46 696c 653a 204e  .License-File: N
+00000320: 4f54 4943 450a 0a23 2046 6c75 7820 4d65  OTICE..# Flux Me
+00000330: 7472 6963 7320 4150 490a 0a3c 212d 2d20  trics API..<!-- 
+00000340: 414c 4c2d 434f 4e54 5249 4255 544f 5253  ALL-CONTRIBUTORS
+00000350: 2d42 4144 4745 3a53 5441 5254 202d 2044  -BADGE:START - D
+00000360: 6f20 6e6f 7420 7265 6d6f 7665 206f 7220  o not remove or 
+00000370: 6d6f 6469 6679 2074 6869 7320 7365 6374  modify this sect
+00000380: 696f 6e20 2d2d 3e0a 5b21 5b41 6c6c 2043  ion -->.[![All C
+00000390: 6f6e 7472 6962 7574 6f72 735d 2868 7474  ontributors](htt
+000003a0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+000003b0: 2e69 6f2f 6261 6467 652f 616c 6c5f 636f  .io/badge/all_co
+000003c0: 6e74 7269 6275 746f 7273 2d31 2d6f 7261  ntributors-1-ora
+000003d0: 6e67 652e 7376 673f 7374 796c 653d 666c  nge.svg?style=fl
+000003e0: 6174 2d73 7175 6172 6529 5d28 2363 6f6e  at-square)](#con
+000003f0: 7472 6962 7574 6f72 732d 290a 3c21 2d2d  tributors-).<!--
+00000400: 2041 4c4c 2d43 4f4e 5452 4942 5554 4f52   ALL-CONTRIBUTOR
+00000410: 532d 4241 4447 453a 454e 4420 2d2d 3e0a  S-BADGE:END -->.
+00000420: 5b21 5b50 7950 495d 2868 7474 7073 3a2f  [![PyPI](https:/
+00000430: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000440: 7079 7069 2f76 2f66 6c75 782d 6d65 7472  pypi/v/flux-metr
+00000450: 6963 732d 6170 6929 5d28 6874 7470 733a  ics-api)](https:
+00000460: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
+00000470: 6374 2f66 6c75 782d 6d65 7472 6963 732d  ct/flux-metrics-
+00000480: 6170 692f 290a 0a54 6869 7320 6973 2061  api/)..This is a
+00000490: 6e20 6578 7065 7269 6d65 6e74 2074 6f20  n experiment to 
+000004a0: 6372 6561 7465 2061 206d 6574 7269 6373  create a metrics
+000004b0: 2041 5049 2066 6f72 204b 7562 6572 6e65   API for Kuberne
+000004c0: 7465 7320 7468 6174 2063 616e 2062 6520  tes that can be 
+000004d0: 7275 6e20 6469 7265 6374 6c79 2066 726f  run directly fro
+000004e0: 6d20 7468 6520 466c 7578 0a6c 6561 6465  m the Flux.leade
+000004f0: 7220 6272 6f6b 6572 2070 6f64 2e20 5765  r broker pod. We
+00000500: 206d 6164 6520 7468 6973 2061 6674 6572   made this after
+00000510: 2063 7265 6174 696e 6720 5b70 726f 6d65   creating [prome
+00000520: 7468 6575 732d 666c 7578 5d28 6874 7470  theus-flux](http
+00000530: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f63  s://github.com/c
+00000540: 6f6e 7665 7267 6564 2d63 6f6d 7075 7469  onverged-computi
+00000550: 6e67 2f70 726f 6d65 7468 6575 732d 666c  ng/prometheus-fl
+00000560: 7578 290a 616e 6420 7761 6e74 696e 6720  ux).and wanting 
+00000570: 6120 6d6f 7265 206d 696e 696d 616c 6973  a more minimalis
+00000580: 7420 6465 7369 676e 2e20 4927 6d20 6e6f  t design. I'm no
+00000590: 7420 6576 656e 2073 7572 6520 6974 2077  t even sure it w
+000005a0: 696c 6c20 776f 726b 2c20 6275 7420 6974  ill work, but it
+000005b0: 2773 2077 6f72 7468 2061 2074 7279 210a  's worth a try!.
+000005c0: 0a23 2320 5573 6167 650a 0a23 2323 2049  .## Usage..### I
+000005d0: 6e73 7461 6c6c 0a0a 596f 7520 6361 6e20  nstall..You can 
+000005e0: 696e 7374 616c 6c20 6672 6f6d 2070 7970  install from pyp
+000005f0: 6920 6f72 2066 726f 6d20 736f 7572 6365  i or from source
+00000600: 3a0a 0a60 6060 6261 7368 0a24 2070 7974  :..```bash.$ pyt
+00000610: 686f 6e20 2d6d 2076 656e 7620 656e 760a  hon -m venv env.
+00000620: 2420 736f 7572 6365 2065 6e76 2f62 696e  $ source env/bin
+00000630: 2f61 6374 6976 6174 650a 2420 7069 7020  /activate.$ pip 
+00000640: 696e 7374 616c 6c20 666c 7578 2d6d 6574  install flux-met
+00000650: 7269 6373 2d61 7069 0a0a 2320 6f72 0a0a  rics-api..# or..
+00000660: 2420 6769 7420 636c 6f6e 6520 6874 7470  $ git clone http
+00000670: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f63  s://github.com/c
+00000680: 6f6e 7665 7267 6564 2d63 6f6d 7075 7469  onverged-computi
+00000690: 6e67 2f66 6c75 782d 6d65 7472 6963 732d  ng/flux-metrics-
+000006a0: 6170 690a 2420 6364 2066 6c75 782d 6d65  api.$ cd flux-me
+000006b0: 7472 6963 732d 6170 690a 2420 7069 7020  trics-api.$ pip 
+000006c0: 696e 7374 616c 6c20 2e0a 2320 796f 7520  install ..# you 
+000006d0: 6361 6e20 616c 736f 2064 6f20 2270 6970  can also do "pip
+000006e0: 2069 6e73 7461 6c6c 202d 6520 2e22 0a60   install -e .".`
+000006f0: 6060 0a0a 5468 6973 2077 696c 6c20 696e  ``..This will in
+00000700: 7374 616c 6c20 7468 6520 6578 6563 7574  stall the execut
+00000710: 6162 6c65 2074 6f20 796f 7572 2070 6174  able to your pat
+00000720: 682c 2077 6869 6368 206d 6967 6874 2062  h, which might b
+00000730: 6520 796f 7572 206c 6f63 616c 2075 7365  e your local use
+00000740: 7220 6269 6e3a 0a0a 6060 6062 6173 680a  r bin:..```bash.
+00000750: 2420 7768 6963 6820 666c 7578 2d6d 6574  $ which flux-met
+00000760: 7269 632d 6170 690a 2f68 6f6d 652f 7673  ric-api./home/vs
+00000770: 636f 6465 2f2e 6c6f 6361 6c2f 6269 6e2f  code/.local/bin/
+00000780: 666c 7578 2d6d 6574 7269 6373 2d61 7069  flux-metrics-api
+00000790: 0a60 6060 0a0a 4e6f 7465 2074 6861 7420  .```..Note that 
+000007a0: 7468 6520 7072 6f76 6964 6564 205b 2e64  the provided [.d
+000007b0: 6576 636f 6e74 6169 6e65 725d 282e 6465  evcontainer](.de
+000007c0: 7663 6f6e 7461 696e 6572 2920 696e 636c  vcontainer) incl
+000007d0: 7564 6573 2061 6e20 656e 7669 726f 6e6d  udes an environm
+000007e0: 656e 7420 666f 7220 5653 436f 6465 2077  ent for VSCode w
+000007f0: 6865 7265 2079 6f75 2068 6176 6520 466c  here you have Fl
+00000800: 7578 0a61 6e64 2063 616e 2069 6e73 7461  ux.and can insta
+00000810: 6c6c 2074 6869 7320 616e 6420 7573 6520  ll this and use 
+00000820: 7265 6164 7920 746f 2067 6f21 0a0a 2323  ready to go!..##
+00000830: 2320 5374 6172 740a 0a59 6f75 276c 6c20  # Start..You'll 
+00000840: 7761 6e74 2074 6f20 6265 2072 756e 6e69  want to be runni
+00000850: 6e67 2069 6e20 6120 466c 7578 2069 6e73  ng in a Flux ins
+00000860: 7461 6e63 652c 2061 7320 7765 206e 6565  tance, as we nee
+00000870: 6420 746f 2063 6f6e 6e65 6374 2074 6f20  d to connect to 
+00000880: 7468 6520 6272 6f6b 6572 2068 616e 646c  the broker handl
+00000890: 652e 0a0a 6060 6062 6173 680a 2420 666c  e...```bash.$ fl
+000008a0: 7578 2073 7461 7274 202d 2d74 6573 742d  ux start --test-
+000008b0: 7369 7a65 3d34 0a60 6060 0a0a 416e 6420  size=4.```..And 
+000008c0: 7468 656e 2073 7461 7274 2074 6865 2073  then start the s
+000008d0: 6572 7665 722e 2054 6869 7320 7769 6c6c  erver. This will
+000008e0: 2075 7365 2061 2064 6566 6175 6c74 2070   use a default p
+000008f0: 6f72 7420 616e 6420 686f 7374 2028 302e  ort and host (0.
+00000900: 302e 302e 303a 3834 3433 2920 7468 6174  0.0.0:8443) that
+00000910: 2079 6f75 2063 616e 2063 7573 746f 6d69   you can customi
+00000920: 7a65 0a69 6620 6465 7369 7265 642e 0a0a  ze.if desired...
+00000930: 6060 6062 6173 680a 2420 666c 7578 2d6d  ```bash.$ flux-m
+00000940: 6574 7269 6373 2d61 7069 2073 7461 7274  etrics-api start
+00000950: 0a0a 2320 6375 7374 6f6d 697a 6520 7468  ..# customize th
+00000960: 6520 706f 7274 206f 7220 686f 7374 0a24  e port or host.$
+00000970: 2066 6c75 782d 6d65 7472 6963 732d 6170   flux-metrics-ap
+00000980: 6920 7374 6172 7420 2d2d 706f 7274 2039  i start --port 9
+00000990: 3030 3020 2d2d 686f 7374 2031 3237 2e30  000 --host 127.0
+000009a0: 2e30 2e31 0a60 6060 0a0a 4966 2079 6f75  .0.1.```..If you
+000009b0: 2077 616e 7420 7373 6c20 2870 6f72 7420   want ssl (port 
+000009c0: 3434 3329 2079 6f75 2063 616e 2070 726f  443) you can pro
+000009d0: 7669 6465 2074 6865 2070 6174 6820 746f  vide the path to
+000009e0: 2061 2063 6572 7469 6669 6361 7465 2061   a certificate a
+000009f0: 6e64 206b 6579 6669 6c65 3a0a 0a60 6060  nd keyfile:..```
+00000a00: 6261 7368 0a24 2066 6c75 782d 6d65 7472  bash.$ flux-metr
+00000a10: 6963 732d 6170 6920 7374 6172 7420 2d2d  ics-api start --
+00000a20: 7373 6c2d 6365 7274 6669 6c65 202f 6574  ssl-certfile /et
+00000a30: 632f 6365 7274 732f 746c 732e 6372 7420  c/certs/tls.crt 
+00000a40: 2d2d 7373 6c2d 6b65 7966 696c 6520 2f65  --ssl-keyfile /e
+00000a50: 7463 2f63 6572 7473 2f74 6c73 2e6b 6579  tc/certs/tls.key
+00000a60: 0a60 6060 0a0a 416e 2065 7861 6d70 6c65  .```..An example
+00000a70: 206f 6620 6120 6675 6c6c 2063 6f6d 6d61   of a full comma
+00000a80: 6e64 2077 6520 6d69 6768 7420 7275 6e20  nd we might run 
+00000a90: 6672 6f6d 2077 6974 6869 6e20 6120 706f  from within a po
+00000aa0: 643a 0a0a 6060 6062 6173 680a 2420 666c  d:..```bash.$ fl
+00000ab0: 7578 2d6d 6574 7269 6373 2d61 7069 2073  ux-metrics-api s
+00000ac0: 7461 7274 202d 2d70 6f72 7420 3834 3433  tart --port 8443
+00000ad0: 202d 2d73 736c 2d63 6572 7466 696c 6520   --ssl-certfile 
+00000ae0: 2f65 7463 2f63 6572 7473 2f74 6c73 2e63  /etc/certs/tls.c
+00000af0: 7274 202d 2d73 736c 2d6b 6579 6669 6c65  rt --ssl-keyfile
+00000b00: 202f 6574 632f 6365 7274 732f 746c 732e   /etc/certs/tls.
+00000b10: 6b65 7920 2d2d 6e61 6d65 7370 6163 6520  key --namespace 
+00000b20: 666c 7578 2d6f 7065 7261 746f 7220 2d2d  flux-operator --
+00000b30: 7365 7276 6963 652d 6e61 6d65 2063 7573  service-name cus
+00000b40: 746f 6d2d 6d65 7472 6963 732d 6170 6973  tom-metrics-apis
+00000b50: 6572 7665 720a 6060 600a 0a53 6565 2060  erver.```..See `
+00000b60: 2d2d 6865 6c70 6020 746f 2073 6565 206f  --help` to see o
+00000b70: 7468 6572 206f 7074 696f 6e73 2061 7661  ther options ava
+00000b80: 696c 6162 6c65 2e0a 0a23 2323 2045 6e64  ilable...### End
+00000b90: 706f 696e 7473 0a0a 2323 2323 204d 6574  points..#### Met
+00000ba0: 7269 630a 0a2a 2a47 4554 202f 6170 6973  ric..**GET /apis
+00000bb0: 2f63 7573 746f 6d2e 6d65 7472 6963 732e  /custom.metrics.
+00000bc0: 6b38 732e 696f 2f76 3162 6574 6132 2f6e  k8s.io/v1beta2/n
+00000bd0: 616d 6573 7061 6365 732f 3c6e 616d 6573  amespaces/<names
+00000be0: 7061 6365 3e2f 6d65 7472 6963 732f 3c6d  pace>/metrics/<m
+00000bf0: 6574 7269 635f 6e61 6d65 3e2a 2a0a 0a48  etric_name>**..H
+00000c00: 6572 6520 6973 2061 6e20 6578 616d 706c  ere is an exampl
+00000c10: 6520 746f 2067 6574 2074 6865 2022 6e6f  e to get the "no
+00000c20: 6465 5f75 705f 636f 756e 7422 206d 6574  de_up_count" met
+00000c30: 7269 633a 0a0a 6060 6062 6173 680a 2063  ric:..```bash. c
+00000c40: 7572 6c20 2d73 2068 7474 703a 2f2f 6c6f  url -s http://lo
+00000c50: 6361 6c68 6f73 743a 3834 3433 2f61 7069  calhost:8443/api
+00000c60: 732f 6375 7374 6f6d 2e6d 6574 7269 6373  s/custom.metrics
+00000c70: 2e6b 3873 2e69 6f2f 7631 6265 7461 322f  .k8s.io/v1beta2/
+00000c80: 6e61 6d65 7370 6163 6573 2f66 6c75 782d  namespaces/flux-
+00000c90: 6f70 6572 6174 6f72 2f6d 6574 7269 6373  operator/metrics
+00000ca0: 2f6e 6f64 655f 7570 5f63 6f75 6e74 207c  /node_up_count |
+00000cb0: 206a 710a 6060 600a 6060 6063 6f6e 736f   jq.```.```conso
+00000cc0: 6c65 0a7b 0a20 2022 6974 656d 7322 3a20  le.{.  "items": 
+00000cd0: 5b0a 2020 2020 7b0a 2020 2020 2020 226d  [.    {.      "m
+00000ce0: 6574 7269 6322 3a20 7b0a 2020 2020 2020  etric": {.      
+00000cf0: 2020 226e 616d 6522 3a20 226e 6f64 655f    "name": "node_
+00000d00: 7570 5f63 6f75 6e74 220a 2020 2020 2020  up_count".      
+00000d10: 7d2c 0a20 2020 2020 2022 7661 6c75 6522  },.      "value"
+00000d20: 3a20 322c 0a20 2020 2020 2022 7469 6d65  : 2,.      "time
+00000d30: 7374 616d 7022 3a20 2232 3032 332d 3035  stamp": "2023-05
+00000d40: 2d33 3154 3034 3a34 343a 3537 2b30 303a  -31T04:44:57+00:
+00000d50: 3030 222c 0a20 2020 2020 2022 7769 6e64  00",.      "wind
+00000d60: 6f77 5365 636f 6e64 7322 3a20 302c 0a20  owSeconds": 0,. 
+00000d70: 2020 2020 2022 6465 7363 7269 6265 644f       "describedO
+00000d80: 626a 6563 7422 3a20 7b0a 2020 2020 2020  bject": {.      
+00000d90: 2020 226b 696e 6422 3a20 2253 6572 7669    "kind": "Servi
+00000da0: 6365 222c 0a20 2020 2020 2020 2022 6e61  ce",.        "na
+00000db0: 6d65 7370 6163 6522 3a20 2266 6c75 782d  mespace": "flux-
+00000dc0: 6f70 6572 6174 6f72 222c 0a20 2020 2020  operator",.     
+00000dd0: 2020 2022 6e61 6d65 223a 2022 6375 7374     "name": "cust
+00000de0: 6f6d 2d6d 6574 7269 6373 2d61 7069 7365  om-metrics-apise
+00000df0: 7276 6572 222c 0a20 2020 2020 2020 2022  rver",.        "
+00000e00: 6170 6956 6572 7369 6f6e 223a 2022 7631  apiVersion": "v1
+00000e10: 6265 7461 3222 0a20 2020 2020 207d 0a20  beta2".      }. 
+00000e20: 2020 207d 0a20 205d 2c0a 2020 2261 7069     }.  ],.  "api
+00000e30: 5665 7273 696f 6e22 3a20 2263 7573 746f  Version": "custo
+00000e40: 6d2e 6d65 7472 6963 732e 6b38 732e 696f  m.metrics.k8s.io
+00000e50: 2f76 3162 6574 6132 222c 0a20 2022 6b69  /v1beta2",.  "ki
+00000e60: 6e64 223a 2022 4d65 7472 6963 5661 6c75  nd": "MetricValu
+00000e70: 654c 6973 7422 2c0a 2020 226d 6574 6164  eList",.  "metad
+00000e80: 6174 6122 3a20 7b0a 2020 2020 2273 656c  ata": {.    "sel
+00000e90: 664c 696e 6b22 3a20 222f 6170 6973 2f63  fLink": "/apis/c
+00000ea0: 7573 746f 6d2e 6d65 7472 6963 732e 6b38  ustom.metrics.k8
+00000eb0: 732e 696f 2f76 3162 6574 6132 220a 2020  s.io/v1beta2".  
+00000ec0: 7d0a 7d0a 6060 600a 0a54 6865 2066 6f6c  }.}.```..The fol
+00000ed0: 6c6f 7769 6e67 206d 6574 7269 6373 2061  lowing metrics a
+00000ee0: 7265 2073 7570 706f 7274 6564 3a0a 0a20  re supported:.. 
+00000ef0: 2d20 2a2a 6e6f 6465 5f75 705f 636f 756e  - **node_up_coun
+00000f00: 742a 2a3a 206e 756d 6265 7220 6f66 206e  t**: number of n
+00000f10: 6f64 6573 2075 7020 696e 2074 6865 204d  odes up in the M
+00000f20: 696e 6943 6c75 7374 6572 0a20 2d20 2a2a  iniCluster. - **
+00000f30: 6e6f 6465 5f66 7265 655f 636f 756e 742a  node_free_count*
+00000f40: 2a3a 206e 756d 6265 7220 6f66 206e 6f64  *: number of nod
+00000f50: 6573 2066 7265 6520 696e 2074 6865 204d  es free in the M
+00000f60: 696e 6943 6c75 7374 6572 0a20 2d20 2a2a  iniCluster. - **
+00000f70: 6e6f 6465 5f63 6f72 6573 5f66 7265 655f  node_cores_free_
+00000f80: 636f 756e 742a 2a3a 206e 756d 6265 7220  count**: number 
+00000f90: 6f66 206e 6f64 6520 636f 7265 7320 6672  of node cores fr
+00000fa0: 6565 2069 6e20 7468 6520 4d69 6e69 436c  ee in the MiniCl
+00000fb0: 7573 7465 720a 202d 202a 2a6e 6f64 655f  uster. - **node_
+00000fc0: 636f 7265 735f 7570 5f63 6f75 6e74 2a2a  cores_up_count**
+00000fd0: 3a20 6e75 6d62 6572 206f 6620 6e6f 6465  : number of node
+00000fe0: 2063 6f72 6573 2075 7020 696e 2074 6865   cores up in the
+00000ff0: 204d 696e 6943 6c75 7374 6572 0a0a 2323   MiniCluster..##
+00001000: 2320 446f 636b 6572 0a0a 5765 2068 6176  # Docker..We hav
+00001010: 6520 6120 646f 636b 6572 2063 6f6e 7461  e a docker conta
+00001020: 696e 6572 2c20 7768 6963 6820 796f 7520  iner, which you 
+00001030: 6361 6e20 6375 7374 6f6d 697a 6520 666f  can customize fo
+00001040: 7220 796f 7572 2075 7365 2063 6173 652c  r your use case,
+00001050: 2062 7574 2069 7427 7320 6d6f 7265 2069   but it's more i
+00001060: 6e74 656e 6465 6420 746f 0a62 6520 6120  ntended to.be a 
+00001070: 6465 6d6f 2e20 596f 7520 6361 6e20 6569  demo. You can ei
+00001080: 7468 6572 2062 7569 6c64 2069 7420 796f  ther build it yo
+00001090: 7572 7365 6c66 2c20 6f72 2075 7365 206f  urself, or use o
+000010a0: 7572 2062 7569 6c64 2e0a 0a60 6060 6261  ur build...```ba
+000010b0: 7368 0a24 2064 6f63 6b65 7220 6275 696c  sh.$ docker buil
+000010c0: 6420 2d74 2066 6c75 785f 6d65 7472 6963  d -t flux_metric
+000010d0: 735f 6170 6920 2e0a 2420 646f 636b 6572  s_api ..$ docker
+000010e0: 2072 756e 202d 6974 202d 7020 3834 3433   run -it -p 8443
+000010f0: 3a38 3434 3320 666c 7578 5f6d 6574 7269  :8443 flux_metri
+00001100: 6373 5f61 7069 0a60 6060 0a6f 720a 0a60  cs_api.```.or..`
+00001110: 6060 6261 7368 0a24 2064 6f63 6b65 7220  ``bash.$ docker 
+00001120: 7275 6e20 2d69 7420 2d70 2038 3434 333a  run -it -p 8443:
+00001130: 3834 3433 2067 6863 722e 696f 2f63 6f6e  8443 ghcr.io/con
+00001140: 7665 7267 6564 2d63 6f6d 7075 7469 6e67  verged-computing
+00001150: 2f66 6c75 782d 6d65 7472 6963 732d 6170  /flux-metrics-ap
+00001160: 690a 6060 600a 0a23 2323 2044 6576 656c  i.```..### Devel
+00001170: 6f70 6d65 6e74 0a0a 4e6f 7465 2074 6861  opment..Note tha
+00001180: 7420 7468 6973 2069 7320 696d 706c 656d  t this is implem
+00001190: 656e 7465 6420 696e 2050 7974 686f 6e2c  ented in Python,
+000011a0: 2062 7574 2028 4920 666f 756e 6420 7468   but (I found th
+000011b0: 6973 2061 6674 6572 2920 7765 2063 6f75  is after) we cou
+000011c0: 6c64 205b 616c 736f 2075 7365 2047 6f5d  ld [also use Go]
+000011d0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+000011e0: 636f 6d2f 6b75 6265 726e 6574 6573 2d73  com/kubernetes-s
+000011f0: 6967 732f 6375 7374 6f6d 2d6d 6574 7269  igs/custom-metri
+00001200: 6373 2d61 7069 7365 7276 6572 292e 0a53  cs-apiserver)..S
+00001210: 7065 6369 6669 6361 6c6c 792c 2049 2066  pecifically, I f
+00001220: 6f75 6e64 2074 6869 7320 7265 706f 7369  ound this reposi
+00001230: 746f 7279 2075 7365 6675 6c20 746f 2073  tory useful to s
+00001240: 6565 2074 6865 205b 7370 6563 2066 6f72  ee the [spec for
+00001250: 6d61 745d 2868 7474 7073 3a2f 2f67 6974  mat](https://git
+00001260: 6875 622e 636f 6d2f 6b75 6265 726e 6574  hub.com/kubernet
+00001270: 6573 2d73 6967 732f 6375 7374 6f6d 2d6d  es-sigs/custom-m
+00001280: 6574 7269 6373 2d61 7069 7365 7276 6572  etrics-apiserver
+00001290: 2f62 6c6f 622f 6d61 7374 6572 2f70 6b67  /blob/master/pkg
+000012a0: 2f67 656e 6572 6174 6564 2f6f 7065 6e61  /generated/opena
+000012b0: 7069 2f63 7573 746f 6d6d 6574 7269 6373  pi/custommetrics
+000012c0: 2f7a 7a5f 6765 6e65 7261 7465 642e 6f70  /zz_generated.op
+000012d0: 656e 6170 692e 676f 292e 0a0a 596f 7520  enapi.go)...You 
+000012e0: 6361 6e20 7468 656e 206f 7065 6e20 7570  can then open up
+000012f0: 2074 6865 2062 726f 7773 6572 2061 7420   the browser at 
+00001300: 5b68 7474 703a 2f2f 6c6f 6361 6c68 6f73  [http://localhos
+00001310: 743a 3834 3433 2f6d 6574 7269 6373 2f5d  t:8443/metrics/]
+00001320: 2868 7474 703a 2f2f 6c6f 6361 6c68 6f73  (http://localhos
+00001330: 743a 3834 3433 2f6d 6574 7269 6373 2920  t:8443/metrics) 
+00001340: 746f 2073 6565 0a74 6865 206d 6574 7269  to see.the metri
+00001350: 6373 210a 0a23 2320 f09f 9881 efb8 8f20  cs!..## ....... 
+00001360: 436f 6e74 7269 6275 746f 7273 20f0 9f98  Contributors ...
+00001370: 81ef b88f 0a0a 5765 2075 7365 2074 6865  ......We use the
+00001380: 205b 616c 6c2d 636f 6e74 7269 6275 746f   [all-contributo
+00001390: 7273 5d28 6874 7470 733a 2f2f 6769 7468  rs](https://gith
+000013a0: 7562 2e63 6f6d 2f61 6c6c 2d63 6f6e 7472  ub.com/all-contr
+000013b0: 6962 7574 6f72 732f 616c 6c2d 636f 6e74  ibutors/all-cont
+000013c0: 7269 6275 746f 7273 290a 746f 6f6c 2074  ributors).tool t
+000013d0: 6f20 6765 6e65 7261 7465 2061 2063 6f6e  o generate a con
+000013e0: 7472 6962 7574 6f72 7320 6772 6170 6869  tributors graphi
+000013f0: 6320 6265 6c6f 772e 0a0a 3c21 2d2d 2041  c below...<!-- A
+00001400: 4c4c 2d43 4f4e 5452 4942 5554 4f52 532d  LL-CONTRIBUTORS-
+00001410: 4c49 5354 3a53 5441 5254 202d 2044 6f20  LIST:START - Do 
+00001420: 6e6f 7420 7265 6d6f 7665 206f 7220 6d6f  not remove or mo
+00001430: 6469 6679 2074 6869 7320 7365 6374 696f  dify this sectio
+00001440: 6e20 2d2d 3e0a 3c21 2d2d 2070 7265 7474  n -->.<!-- prett
+00001450: 6965 722d 6967 6e6f 7265 2d73 7461 7274  ier-ignore-start
+00001460: 202d 2d3e 0a3c 212d 2d20 6d61 726b 646f   -->.<!-- markdo
+00001470: 776e 6c69 6e74 2d64 6973 6162 6c65 202d  wnlint-disable -
+00001480: 2d3e 0a3c 7461 626c 653e 0a20 203c 7462  ->.<table>.  <tb
+00001490: 6f64 793e 0a20 2020 203c 7472 3e0a 2020  ody>.    <tr>.  
+000014a0: 2020 2020 3c74 6420 616c 6967 6e3d 2263      <td align="c
+000014b0: 656e 7465 7222 2076 616c 6967 6e3d 2274  enter" valign="t
+000014c0: 6f70 2220 7769 6474 683d 2231 342e 3238  op" width="14.28
+000014d0: 2522 3e3c 6120 6872 6566 3d22 6874 7470  %"><a href="http
+000014e0: 733a 2f2f 7673 6f63 682e 6769 7468 7562  s://vsoch.github
+000014f0: 2e69 6f22 3e3c 696d 6720 7372 633d 2268  .io"><img src="h
+00001500: 7474 7073 3a2f 2f61 7661 7461 7273 2e67  ttps://avatars.g
+00001510: 6974 6875 6275 7365 7263 6f6e 7465 6e74  ithubusercontent
+00001520: 2e63 6f6d 2f75 2f38 3134 3332 323f 763d  .com/u/814322?v=
+00001530: 343f 733d 3130 3022 2077 6964 7468 3d22  4?s=100" width="
+00001540: 3130 3070 783b 2220 616c 743d 2256 616e  100px;" alt="Van
+00001550: 6573 7361 7361 7572 7573 222f 3e3c 6272  essasaurus"/><br
+00001560: 202f 3e3c 7375 623e 3c62 3e56 616e 6573   /><sub><b>Vanes
+00001570: 7361 7361 7572 7573 3c2f 623e 3c2f 7375  sasaurus</b></su
+00001580: 623e 3c2f 613e 3c62 7220 2f3e 3c61 2068  b></a><br /><a h
+00001590: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+000015a0: 6875 622e 636f 6d2f 636f 6e76 6572 6765  hub.com/converge
+000015b0: 642d 636f 6d70 7574 696e 672f 666c 7578  d-computing/flux
+000015c0: 2d6d 6574 7269 6373 2d61 7069 2f63 6f6d  -metrics-api/com
+000015d0: 6d69 7473 3f61 7574 686f 723d 7673 6f63  mits?author=vsoc
+000015e0: 6822 2074 6974 6c65 3d22 436f 6465 223e  h" title="Code">
+000015f0: f09f 92bb 3c2f 613e 3c2f 7464 3e0a 2020  ....</a></td>.  
+00001600: 2020 3c2f 7472 3e0a 2020 3c2f 7462 6f64    </tr>.  </tbod
+00001610: 793e 0a3c 2f74 6162 6c65 3e0a 0a3c 212d  y>.</table>..<!-
+00001620: 2d20 6d61 726b 646f 776e 6c69 6e74 2d72  - markdownlint-r
+00001630: 6573 746f 7265 202d 2d3e 0a3c 212d 2d20  estore -->.<!-- 
+00001640: 7072 6574 7469 6572 2d69 676e 6f72 652d  prettier-ignore-
+00001650: 656e 6420 2d2d 3e0a 0a3c 212d 2d20 414c  end -->..<!-- AL
+00001660: 4c2d 434f 4e54 5249 4255 544f 5253 2d4c  L-CONTRIBUTORS-L
+00001670: 4953 543a 454e 4420 2d2d 3e0a 0a23 2320  IST:END -->..## 
+00001680: 4c69 6365 6e73 650a 0a48 5043 4943 2044  License..HPCIC D
+00001690: 6576 546f 6f6c 7320 6973 2064 6973 7472  evTools is distr
+000016a0: 6962 7574 6564 2075 6e64 6572 2074 6865  ibuted under the
+000016b0: 2074 6572 6d73 206f 6620 7468 6520 4d49   terms of the MI
+000016c0: 5420 6c69 6365 6e73 652e 0a41 6c6c 206e  T license..All n
+000016d0: 6577 2063 6f6e 7472 6962 7574 696f 6e73  ew contributions
+000016e0: 206d 7573 7420 6265 206d 6164 6520 756e   must be made un
+000016f0: 6465 7220 7468 6973 206c 6963 656e 7365  der this license
+00001700: 2e0a 0a53 6565 205b 4c49 4345 4e53 455d  ...See [LICENSE]
+00001710: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00001720: 636f 6d2f 636f 6e76 6572 6765 642d 636f  com/converged-co
+00001730: 6d70 7574 696e 672f 666c 7578 2d6d 6574  mputing/flux-met
+00001740: 7269 6373 2d61 7069 2f62 6c6f 622f 6d61  rics-api/blob/ma
+00001750: 696e 2f4c 4943 454e 5345 292c 0a5b 434f  in/LICENSE),.[CO
+00001760: 5059 5249 4748 545d 2868 7474 7073 3a2f  PYRIGHT](https:/
+00001770: 2f67 6974 6875 622e 636f 6d2f 636f 6e76  /github.com/conv
+00001780: 6572 6765 642d 636f 6d70 7574 696e 672f  erged-computing/
+00001790: 666c 7578 2d6d 6574 7269 6373 2d61 7069  flux-metrics-api
+000017a0: 2f62 6c6f 622f 6d61 696e 2f43 4f50 5952  /blob/main/COPYR
+000017b0: 4947 4854 292c 2061 6e64 0a5b 4e4f 5449  IGHT), and.[NOTI
+000017c0: 4345 5d28 6874 7470 733a 2f2f 6769 7468  CE](https://gith
+000017d0: 7562 2e63 6f6d 2f63 6f6e 7665 7267 6564  ub.com/converged
+000017e0: 2d63 6f6d 7075 7469 6e67 2f66 6c75 782d  -computing/flux-
+000017f0: 6d65 7472 6963 732d 6170 692f 626c 6f62  metrics-api/blob
+00001800: 2f6d 6169 6e2f 4e4f 5449 4345 2920 666f  /main/NOTICE) fo
+00001810: 7220 6465 7461 696c 732e 0a0a 5350 4458  r details...SPDX
+00001820: 2d4c 6963 656e 7365 2d49 6465 6e74 6966  -License-Identif
+00001830: 6965 723a 2028 4d49 5429 0a0a 4c4c 4e4c  ier: (MIT)..LLNL
+00001840: 2d43 4f44 452d 2038 3432 3631 340a       -CODE- 842614.
```

### Comparing `flux-metrics-api-0.0.0/flux_metrics_api/logger.py` & `flux-metrics-api-0.0.1/flux_metrics_api/logger.py`

 * *Files identical despite different names*

### Comparing `flux-metrics-api-0.0.0/flux_metrics_api/metrics.py` & `flux-metrics-api-0.0.1/flux_metrics_api/metrics.py`

 * *Files identical despite different names*

### Comparing `flux-metrics-api-0.0.0/flux_metrics_api/routes.py` & `flux-metrics-api-0.0.1/flux_metrics_api/routes.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,73 +1,80 @@
 # Copyright 2023 Lawrence Livermore National Security, LLC and other
 # HPCIC DevTools Developers. See the top-level COPYRIGHT file for details.
 #
 # SPDX-License-Identifier: (MIT)
 
+from apispec import APISpec
 from starlette.endpoints import HTTPEndpoint
 from starlette.responses import JSONResponse
 from starlette.routing import Route
-from starlette.schemas import SchemaGenerator
+from starlette_apispec import APISpecSchemaGenerator
 
 import flux_metrics_api.defaults as defaults
 import flux_metrics_api.types as types
 import flux_metrics_api.version as version
 from flux_metrics_api.metrics import metrics
 
-schemas = SchemaGenerator(
-    {
-        "openapi": "3.0.0",
-        "info": {"title": "Flux Metrics API", "version": version.__version__},
-    }
+schemas = APISpecSchemaGenerator(
+    APISpec(
+        title="Flux Metrics API",
+        version=version.__version__,
+        openapi_version="3.0.0",
+        info={"description": "Export Flux custom metrics."},
+    )
+)
+
+not_found_response = JSONResponse(
+    {"detail": "The metric server is not running in a Kubernetes pod."},
+    status_code=404,
 )
 
 
 class Root(HTTPEndpoint):
     """
     Root of the API
 
-    This needs to return 200 for a health check
+    This needs to return 200 for a health check. I later discovered it also needs
+    to return the listing of available metrics!
     """
 
     async def get(self, request):
-        return JSONResponse({})
+        return JSONResponse(types.new_resource_list())
 
 
 def get_metric(request):
     """
     Shared function to get and return a metric response
 
     We could do some checks / validation of namespace here, but since
     we are just running inside a single namespace we don't care.
     """
     metric_name = request.path_params["metric_name"]
     namespace = request.path_params.get("namespace")
+    print(f"Requested metric {metric_name} in  namespace {namespace}")
 
-    if (
-        namespace is not None
-        and defaults.NAMESPACES is not None
-        and namespace not in defaults.NAMESPACES
-    ):
-        return JSONResponse(
-            {"detail": "This namespace is not known to the server."}, status_code=404
-        )
-
+    # TODO we don't do anything with namespace currently, we assume we won't
+    # be able to hit this if running in the wrong one
     # Unknown metric
     if metric_name not in metrics:
+        print(f"Unknown metric requested {metric_name}")
         return JSONResponse(
             {"detail": "This metric is not known to the server."}, status_code=404
         )
 
     # Prepare the metric
     metric = types.new_identifier(metric_name)
 
     # Get the value from Flux, assemble into listing
     value = metrics[metric_name]()
     metric_value = types.new_metric(metric, value=value)
-    listing = types.new_metric_list([metric_value])
+
+    # Give the endpoint for the service as metadata
+    metadata = {"selfLink": defaults.API_ROOT}
+    listing = types.new_metric_list([metric_value], metadata=metadata)
     return JSONResponse(listing)
 
 
 class Metric(HTTPEndpoint):
     """
     Get a metric for a namespace.
 
@@ -75,28 +82,54 @@
     we are getting the metric for where it is running (and don't care)
     """
 
     async def get(self, request):
         return get_metric(request)
 
 
+class APIGroupList(HTTPEndpoint):
+    """
+    Service a faux resource list just for our custom metrics endpoint.
+    """
+
+    async def get(self, request):
+        listing = types.new_group_list()
+        if not listing:
+            return not_found_response
+        return JSONResponse(listing)
+
+
+class OpenAPI(HTTPEndpoint):
+    """
+    Forward the cluster openapi endpoint
+    """
+
+    async def get(self, request):
+        version = request.path_params["version"]
+        openapi = types.get_cluster_schema(version)
+        if not openapi:
+            return not_found_response
+        return JSONResponse(openapi)
+
+
 def openapi_schema(request):
     """
     Get the openapi spec from the endpoints
-
-    TODO: debug why paths empty
     """
     return JSONResponse(schemas.get_schema(routes=routes))
 
 
-# STOPPED HERE - make open api spec s we can see endpoints and query
 routes = [
     Route(defaults.API_ROOT, Root),
-    # Optional for openapi, we could add if needed
+    # This is a faux route so we can get the preferred resource version
+    Route("/apis", APIGroupList),
+    Route("/openapi/{version}", OpenAPI),
     Route(defaults.API_ROOT + "/namespaces/{namespace}/metrics/{metric_name}", Metric),
     Route(defaults.API_ROOT + "/{resource}/{name}/{metric_name}", Metric),
     Route(
         defaults.API_ROOT + "/namespaces/{namespace}/{resource}/{name}/{metric_name}",
         Metric,
     ),
+    # These are for our endpoints
+    Route("/schema", openapi_schema, include_in_schema=False),
     Route(f"{defaults.API_ROOT}/openapi/v2", openapi_schema, include_in_schema=False),
 ]
```

### Comparing `flux-metrics-api-0.0.0/flux_metrics_api/server.py` & `flux-metrics-api-0.0.1/flux_metrics_api/server.py`

 * *Files 24% similar despite different names*

```diff
@@ -61,48 +61,68 @@
     start = subparsers.add_parser(
         "start",
         description="Start the running server.",
         formatter_class=argparse.RawTextHelpFormatter,
     )
     start.add_argument(
         "--port",
-        help="Port to run application",
-        default=8080,
+        help="Port to run application (defaults to 8443)",
+        default=8443,
         type=int,
     )
+    start.add_argument("--namespace", help="Namespace the API is running in")
     start.add_argument(
-        "--namespace", help="Scope to running in these namespace(s)", action="append"
+        "--service-name", help="Service name the metrics service is running from"
     )
     start.add_argument(
         "--api-path",
         dest="api_path",
         help="Custom API path (defaults to /apis/custom.metrics.k8s.io/v1beta2)",
         default=None,
     )
-
     start.add_argument(
         "--host",
         help="Host address to run application",
         default="0.0.0.0",
     )
     start.add_argument(
         "--verbose",
         help="add verbose metrics about server usage and garbage collection (not related to Flux).",
         default=False,
         action="store_true",
     )
+    start.add_argument(
+        "--no-cache",
+        help="Do not cache Kubernetes API responses.",
+        default=False,
+        action="store_true",
+    )
+    start.add_argument("--ssl-keyfile", help="full path to ssl keyfile")
+    start.add_argument("--ssl-certfile", help="full path to ssl certfile")
     return parser
 
 
 def start(args):
     """
     Start the server with uvicorn
     """
+    # Validate certificates if provided
+    if args.ssl_keyfile and not args.ssl_certfile:
+        sys.exit("A --ssl-keyfile was provided without a --ssl-certfile.")
+    if args.ssl_certfile and not args.ssl_keyfile:
+        sys.exit("A --ssl-certfile was provided without a --ssl-keyfile.")
+
     app = Starlette(debug=args.debug, routes=routes)
-    uvicorn.run(app, host=args.host, port=args.port)
+    uvicorn.run(
+        app,
+        host=args.host,
+        port=args.port,
+        ssl_keyfile=args.ssl_keyfile,
+        ssl_certfile=args.ssl_certfile,
+    )
 
 
 def main():
     parser = get_parser()
 
     def help(return_code=0):
         version = flux_metrics_api.__version__
@@ -127,22 +147,30 @@
 
     setup_logger(
         quiet=args.quiet,
         debug=args.debug,
     )
 
     # Setup the registry - non verbose is default
-    print(f"API endpoint is at {defaults.API_ROOT}")
     if args.api_path is not None:
-        print(f"Setting API endpoint to {args.api_path}")
         defaults.API_ROOT = args.api_path
+    print(f"API endpoint is at {defaults.API_ROOT}")
 
-    # Limit to specific namespaces?
+    # Do not cache responses
+    if args.no_cache is True:
+        defaults.USE_CACHE = False
+
+    # Set namespace or service name to be different than defaults
     if args.namespace:
-        defaults.NAMESPACES = args.namespace
+        defaults.NAMESPACE = args.namespace
+    print(f"Running from namespace {defaults.NAMESPACE}")
+
+    if args.service_name:
+        defaults.SERVICE_NAME = args.service_name
+    print(f"Service name {defaults.SERVICE_NAME}")
 
     # Does the user want a shell?
     if args.command == "start":
         return start(args)
 
     sys.exit(f"{args.command} is not a known command.")
```

### Comparing `flux-metrics-api-0.0.0/flux_metrics_api/version.py` & `flux-metrics-api-0.0.1/flux_metrics_api/version.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # Copyright 2023 Lawrence Livermore National Security, LLC and other
 # HPCIC DevTools Developers. See the top-level COPYRIGHT file for details.
 #
 # SPDX-License-Identifier: (MIT)
 
-__version__ = "0.0.0"
+__version__ = "0.0.1"
 AUTHOR = "Vanessa Sochat"
 EMAIL = "vsoch@users.noreply.github.com"
 NAME = "flux-metrics-api"
 PACKAGE_URL = "https://github.com/converged-computing/flux-metrics-api"
 KEYWORDS = "cloud, flux, flux-framework, monitoring"
 DESCRIPTION = "Custom metrics exporter for Flux in Kubernetes"
 LICENSE = "LICENSE"
 
 ################################################################################
 # Global requirements
 
 INSTALL_REQUIRES = (
     ("uvicorn", {"min_version": None}),
     ("starlette", {"min_version": None}),
+    ("starlette-apispec", {"min_version": None}),
 )
 
 TESTS_REQUIRES = (("pytest", {"min_version": "4.6.2"}),)
 
 ################################################################################
 # Submodule Requirements (versions that include database)
```

### Comparing `flux-metrics-api-0.0.0/flux_metrics_api.egg-info/PKG-INFO` & `flux-metrics-api-0.0.1/flux_metrics_api.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: flux-metrics-api
-Version: 0.0.0
+Version: 0.0.1
 Summary: Custom metrics exporter for Flux in Kubernetes
 Home-page: https://github.com/converged-computing/flux-metrics-api
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: cloud,flux,flux-framework,monitoring
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Unix
@@ -66,52 +65,72 @@
 
 You'll want to be running in a Flux instance, as we need to connect to the broker handle.
 
 ```bash
 $ flux start --test-size=4
 ```
 
-And then start the server. This will use a default port and host (0.0.0.0:8080) that you can customize
+And then start the server. This will use a default port and host (0.0.0.0:8443) that you can customize
 if desired.
 
 ```bash
 $ flux-metrics-api start
 
 # customize the port or host
 $ flux-metrics-api start --port 9000 --host 127.0.0.1
 ```
 
+If you want ssl (port 443) you can provide the path to a certificate and keyfile:
+
+```bash
+$ flux-metrics-api start --ssl-certfile /etc/certs/tls.crt --ssl-keyfile /etc/certs/tls.key
+```
+
+An example of a full command we might run from within a pod:
+
+```bash
+$ flux-metrics-api start --port 8443 --ssl-certfile /etc/certs/tls.crt --ssl-keyfile /etc/certs/tls.key --namespace flux-operator --service-name custom-metrics-apiserver
+```
+
 See `--help` to see other options available.
 
 ### Endpoints
 
 #### Metric
 
 **GET /apis/custom.metrics.k8s.io/v1beta2/namespaces/<namespace>/metrics/<metric_name>**
 
 Here is an example to get the "node_up_count" metric:
 
 ```bash
- curl -s http://localhost:8080/apis/custom.metrics.k8s.io/v1beta2/namespaces/flux-operator/metrics/node_up_count | jq
+ curl -s http://localhost:8443/apis/custom.metrics.k8s.io/v1beta2/namespaces/flux-operator/metrics/node_up_count | jq
 ```
 ```console
 {
   "items": [
     {
       "metric": {
         "name": "node_up_count"
       },
-      "value": 4,
-      "time": "",
+      "value": 2,
+      "timestamp": "2023-05-31T04:44:57+00:00",
       "windowSeconds": 0,
-      "describedObject": null
+      "describedObject": {
+        "kind": "Service",
+        "namespace": "flux-operator",
+        "name": "custom-metrics-apiserver",
+        "apiVersion": "v1beta2"
+      }
     }
   ],
   "apiVersion": "custom.metrics.k8s.io/v1beta2",
-  "kind": "MetricValueList"
+  "kind": "MetricValueList",
+  "metadata": {
+    "selfLink": "/apis/custom.metrics.k8s.io/v1beta2"
+  }
 }
 ```
 
 The following metrics are supported:
 
  - **node_up_count**: number of nodes up in the MiniCluster
  - **node_free_count**: number of nodes free in the MiniCluster
@@ -121,23 +140,28 @@
 ### Docker
 
 We have a docker container, which you can customize for your use case, but it's more intended to
 be a demo. You can either build it yourself, or use our build.
 
 ```bash
 $ docker build -t flux_metrics_api .
-$ docker run -it -p 8080:8080 flux_metrics_api
+$ docker run -it -p 8443:8443 flux_metrics_api
 ```
 or
 
 ```bash
-$ docker run -it -p 8080:8080 ghcr.io/converged-computing/flux-metrics-api
+$ docker run -it -p 8443:8443 ghcr.io/converged-computing/flux-metrics-api
 ```
 
-You can then open up the browser at [http://localhost:8080/metrics/](http://localhost:8080/metrics) to see
+### Development
+
+Note that this is implemented in Python, but (I found this after) we could [also use Go](https://github.com/kubernetes-sigs/custom-metrics-apiserver).
+Specifically, I found this repository useful to see the [spec format](https://github.com/kubernetes-sigs/custom-metrics-apiserver/blob/master/pkg/generated/openapi/custommetrics/zz_generated.openapi.go).
+
+You can then open up the browser at [http://localhost:8443/metrics/](http://localhost:8443/metrics) to see
 the metrics!
 
 ## 😁️ Contributors 😁️
 
 We use the [all-contributors](https://github.com/all-contributors/all-contributors)
 tool to generate a contributors graphic below.
 
@@ -165,9 +189,7 @@
 See [LICENSE](https://github.com/converged-computing/flux-metrics-api/blob/main/LICENSE),
 [COPYRIGHT](https://github.com/converged-computing/flux-metrics-api/blob/main/COPYRIGHT), and
 [NOTICE](https://github.com/converged-computing/flux-metrics-api/blob/main/NOTICE) for details.
 
 SPDX-License-Identifier: (MIT)
 
 LLNL-CODE- 842614
-
-
```

### Comparing `flux-metrics-api-0.0.0/flux_metrics_api.egg-info/SOURCES.txt` & `flux-metrics-api-0.0.1/flux_metrics_api.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -3,20 +3,22 @@
 MANIFEST.in
 NOTICE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 flux_metrics_api/__init__.py
+flux_metrics_api/apis.py
 flux_metrics_api/defaults.py
 flux_metrics_api/logger.py
 flux_metrics_api/metrics.py
 flux_metrics_api/routes.py
 flux_metrics_api/server.py
 flux_metrics_api/types.py
+flux_metrics_api/utils.py
 flux_metrics_api/version.py
 flux_metrics_api.egg-info/PKG-INFO
 flux_metrics_api.egg-info/SOURCES.txt
 flux_metrics_api.egg-info/dependency_links.txt
 flux_metrics_api.egg-info/entry_points.txt
 flux_metrics_api.egg-info/not-zip-safe
 flux_metrics_api.egg-info/requires.txt
```

### Comparing `flux-metrics-api-0.0.0/setup.py` & `flux-metrics-api-0.0.1/setup.py`

 * *Files identical despite different names*

