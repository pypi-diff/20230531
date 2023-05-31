# Comparing `tmp/balaboba-3.0.0.tar.gz` & `tmp/balaboba-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balaboba-3.0.0.tar", max compression
+gzip compressed data, was "balaboba-3.0.1.tar", max compression
```

## Comparing `balaboba-3.0.0.tar` & `balaboba-3.0.1.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1065 2022-11-21 19:37:14.850082 balaboba-3.0.0/LICENSE
--rw-r--r--   0        0        0     1257 2022-11-26 16:29:16.261975 balaboba-3.0.0/README.md
--rw-r--r--   0        0        0      128 2022-11-26 15:27:32.779621 balaboba-3.0.0/balaboba/__init__.py
--rw-r--r--   0        0        0     1533 2022-11-26 15:11:23.132621 balaboba-3.0.0/balaboba/_balaboba.py
--rw-r--r--   0        0        0     1151 2022-11-26 11:36:05.288031 balaboba-3.0.0/balaboba/_http.py
--rw-r--r--   0        0        0      147 2022-11-26 11:32:07.174252 balaboba-3.0.0/balaboba/_text_type.py
--rw-r--r--   0        0        0        0 2022-11-26 15:22:47.213304 balaboba-3.0.0/balaboba/py.typed
--rw-r--r--   0        0        0     1488 2022-11-26 17:43:31.680494 balaboba-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     2059 1970-01-01 00:00:00.000000 balaboba-3.0.0/setup.py
--rw-r--r--   0        0        0     2302 1970-01-01 00:00:00.000000 balaboba-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-31 10:59:20.692139 balaboba-3.0.1/LICENSE
+-rw-r--r--   0        0        0     1041 2023-05-31 10:59:20.692139 balaboba-3.0.1/README.md
+-rw-r--r--   0        0        0      128 2023-05-31 10:59:20.692139 balaboba-3.0.1/balaboba/__init__.py
+-rw-r--r--   0        0        0     2935 2023-05-31 10:59:20.692139 balaboba-3.0.1/balaboba/_balaboba.py
+-rw-r--r--   0        0        0     1442 2023-05-31 10:59:20.692139 balaboba-3.0.1/balaboba/_http.py
+-rw-r--r--   0        0        0      147 2023-05-31 10:59:20.692139 balaboba-3.0.1/balaboba/_text_type.py
+-rw-r--r--   0        0        0        0 2023-05-31 10:59:20.692139 balaboba-3.0.1/balaboba/py.typed
+-rw-r--r--   0        0        0     2818 2023-05-31 10:59:20.696138 balaboba-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2494 1970-01-01 00:00:00.000000 balaboba-3.0.1/PKG-INFO
```

### Comparing `balaboba-3.0.0/LICENSE` & `balaboba-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `balaboba-3.0.0/README.md` & `balaboba-3.0.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # balaboba
 
-[![CI](https://github.com/monosans/balaboba/actions/workflows/ci.yml/badge.svg?branch=main&event=push)](https://github.com/monosans/balaboba/actions/workflows/ci.yml)
-[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/monosans/balaboba/main.svg)](https://results.pre-commit.ci/latest/github/monosans/balaboba/main)
-[![codecov](https://codecov.io/gh/monosans/balaboba/branch/main/graph/badge.svg)](https://codecov.io/gh/monosans/balaboba)
+[![CI](https://github.com/monosans/balaboba/actions/workflows/ci.yml/badge.svg)](https://github.com/monosans/balaboba/actions/workflows/ci.yml)
+[![Downloads](https://static.pepy.tech/badge/balaboba)](https://pepy.tech/project/balaboba)
 
 Wrapper for [Yandex Balaboba](https://yandex.com/lab/yalm-en) ([Яндекс Балабоба](https://yandex.ru/lab/yalm)).
 
 Asynchronous version [here](https://github.com/monosans/aiobalaboba).
 
 ## Disclaimer
 
 The neural network doesn’t really know what it’s saying, so it can say absolutely anything. Don’t get offended if it says something that hurts your feelings. When sharing the texts, make sure they’re not offensive or violate the law.
 
 ## Installation
 
 ```bash
-python -m pip install balaboba
+python -m pip install -U balaboba
 ```
 
 ## Usage example
 
 ```python
 from balaboba import Balaboba
```

### Comparing `balaboba-3.0.0/balaboba/_balaboba.py` & `balaboba-3.0.1/balaboba/_balaboba.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from __future__ import annotations
 
 import sys
-from typing import List, Optional, Union
+import urllib.parse
+from typing import Dict, List, Optional, Union
 
 from requests import Session
 
 from ._http import HTTPSession
 from ._text_type import TextType
 
-if sys.version_info < (3, 8):  # pragma: no cover
+if sys.version_info < (3, 8):  # pragma: <3.8 cover
     from typing_extensions import Literal
-else:  # pragma: no cover
+else:  # pragma: >=3.8 cover
     from typing import Literal
 
 
 class Balaboba:
     """Wrapper for Yandex Balaboba."""
 
     __slots__ = ("_session",)
@@ -27,24 +28,56 @@
     def session(self) -> Optional[Session]:
         return self._session.session
 
     @session.setter
     def session(self, session: Optional[Session]) -> None:
         self._session.session = session
 
-    def get_text_types(
-        self, language: Literal["en", "ru"] = "ru"
-    ) -> List[TextType]:
+    def get_text_types(self, language: Literal["en", "ru"] = "ru") -> List[TextType]:
         endpoint = "intros" if language == "ru" else "intros_eng"
-        response = self._session.get_response(method="GET", endpoint=endpoint)
+        response = self._session.get_response(
+            method="GET", endpoint=endpoint, headers=self._get_text_types_headers()
+        )
         return [TextType(*intro) for intro in response["intros"]]
 
     def balaboba(self, query: str, text_type: Union[TextType, int]) -> str:
-        intro = (
-            text_type.number if isinstance(text_type, TextType) else text_type
-        )
+        intro = text_type.number if isinstance(text_type, TextType) else text_type
         response = self._session.get_response(
             method="POST",
             endpoint="text3",
             json={"query": query, "intro": intro, "filter": 1},
+            headers=self._get_balaboba_headers(query, intro),
         )
         return "{}{}".format(response["query"], response["text"])
+
+    def _get_text_types_headers(self) -> Dict[str, str]:
+        return {
+            "User-Agent": (
+                "Mozilla/5.0 (Windows NT 10.0; rv:113.0) Gecko/20100101 Firefox/113.0"
+            ),
+            "Accept-Language": "en-US,en;q=0.5",
+            "Referer": "https://yandex.ru/lab/yalm",
+            "Sec-Fetch-Dest": "empty",
+            "Sec-Fetch-Mode": "cors",
+            "Sec-Fetch-Site": "same-origin",
+            "TE": "trailers",
+        }
+
+    def _get_balaboba_headers(self, query: str, text_type: int) -> Dict[str, str]:
+        return {
+            "User-Agent": (
+                "Mozilla/5.0 (Windows NT 10.0; rv:113.0) Gecko/20100101 Firefox/113.0"
+            ),
+            "Accept-Language": "en-US,en;q=0.5",
+            "Referer": f"https://yandex.ru/lab/yalm?style={text_type}",
+            "X-Requested-With": "XMLHttpRequest",
+            "X-Retpath-Y": (
+                "https://yandex.ru/lab/yalm?style={}&input={}&skipCurtain=1".format(
+                    text_type, urllib.parse.quote_plus(query)
+                )
+            ),
+            "Origin": "https://yandex.ru",
+            "Sec-Fetch-Dest": "empty",
+            "Sec-Fetch-Mode": "cors",
+            "Sec-Fetch-Site": "same-origin",
+            "TE": "trailers",
+        }
```

### Comparing `balaboba-3.0.0/balaboba/_http.py` & `balaboba-3.0.1/balaboba/_http.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,57 @@
 from __future__ import annotations
 
-from typing import Any, Dict, Optional
+from typing import Any, Mapping, Optional
 
-from requests import Session
+from requests import Response, Session
 
 
 class HTTPSession:
     __slots__ = ("session",)
 
     def __init__(self, session: Optional[Session]) -> None:
         self.session = session
 
     def get_response(
         self,
         *,
         method: str,
         endpoint: str,
-        json: Optional[Dict[str, Any]] = None,
+        json: Any = None,
+        headers: Mapping[str, str],
     ) -> Any:
         if isinstance(self.session, Session):
-            return self._fetch(
+            response = self._fetch(
                 method=method,
                 endpoint=endpoint,
                 json=json,
+                headers=headers,
                 session=self.session,
             )
-        with Session() as session:
-            return self._fetch(
-                method=method, endpoint=endpoint, json=json, session=session
-            )
+        else:
+            with Session() as session:
+                response = self._fetch(
+                    method=method,
+                    endpoint=endpoint,
+                    json=json,
+                    headers=headers,
+                    session=session,
+                )
+        response.raise_for_status()
+        return response.json()
 
     def _fetch(
         self,
         *,
         method: str,
         endpoint: str,
-        json: Optional[Dict[str, Any]],
+        json: Any,
+        headers: Mapping[str, str],
         session: Session,
-    ) -> Any:
+    ) -> Response:
         with session.request(
-            method, f"https://yandex.ru/lab/api/yalm/{endpoint}", json=json
+            method,
+            f"https://yandex.ru/lab/api/yalm/{endpoint}",
+            json=json,
+            headers=headers,
         ) as response:
-            response.raise_for_status()
-            return response.json()
+            return response
```

### Comparing `balaboba-3.0.0/PKG-INFO` & `balaboba-3.0.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,52 +1,60 @@
 Metadata-Version: 2.1
 Name: balaboba
-Version: 3.0.0
+Version: 3.0.1
 Summary: Wrapper for Yandex Balaboba
 Home-page: https://github.com/monosans/balaboba
 License: MIT
 Keywords: yalm
 Author: monosans
 Author-email: hsyqixco@protonmail.com
 Requires-Python: >=3.7,<4.0
+Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
 Classifier: Natural Language :: Russian
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Internet
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: requests (>=2.28,<3.0)
-Requires-Dist: typing-extensions (>=3.7.4.3,<5); python_version < "3.8"
+Requires-Dist: typing-extensions (>=3.7.4.3,<5) ; python_version < "3.8"
 Project-URL: Repository, https://github.com/monosans/balaboba
 Description-Content-Type: text/markdown
 
 # balaboba
 
-[![CI](https://github.com/monosans/balaboba/actions/workflows/ci.yml/badge.svg?branch=main&event=push)](https://github.com/monosans/balaboba/actions/workflows/ci.yml)
-[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/monosans/balaboba/main.svg)](https://results.pre-commit.ci/latest/github/monosans/balaboba/main)
-[![codecov](https://codecov.io/gh/monosans/balaboba/branch/main/graph/badge.svg)](https://codecov.io/gh/monosans/balaboba)
+[![CI](https://github.com/monosans/balaboba/actions/workflows/ci.yml/badge.svg)](https://github.com/monosans/balaboba/actions/workflows/ci.yml)
+[![Downloads](https://static.pepy.tech/badge/balaboba)](https://pepy.tech/project/balaboba)
 
 Wrapper for [Yandex Balaboba](https://yandex.com/lab/yalm-en) ([Яндекс Балабоба](https://yandex.ru/lab/yalm)).
 
 Asynchronous version [here](https://github.com/monosans/aiobalaboba).
 
 ## Disclaimer
 
 The neural network doesn’t really know what it’s saying, so it can say absolutely anything. Don’t get offended if it says something that hurts your feelings. When sharing the texts, make sure they’re not offensive or violate the law.
 
 ## Installation
 
 ```bash
-python -m pip install balaboba
+python -m pip install -U balaboba
 ```
 
 ## Usage example
 
 ```python
 from balaboba import Balaboba
```

