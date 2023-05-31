# Comparing `tmp/assemblyai-0.4.0.tar.gz` & `tmp/assemblyai-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assemblyai-0.4.0.tar", last modified: Tue May 30 18:31:57 2023, max compression
+gzip compressed data, was "assemblyai-0.4.1.tar", last modified: Wed May 31 19:20:30 2023, max compression
```

## Comparing `assemblyai-0.4.0.tar` & `assemblyai-0.4.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:31:57.952522 assemblyai-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-30 18:31:46.000000 assemblyai-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-05-30 18:31:57.952522 assemblyai-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-05-30 18:31:46.000000 assemblyai-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:31:57.948522 assemblyai-0.4.0/assemblyai/
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-30 18:31:46.000000 assemblyai-0.4.0/assemblyai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-05-30 18:31:46.000000 assemblyai-0.4.0/assemblyai/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-30 18:31:46.000000 assemblyai-0.4.0/assemblyai/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-05-30 18:31:46.000000 assemblyai-0.4.0/assemblyai/lemur.py
--rw-r--r--   0 runner    (1001) docker     (123)    20931 2023-05-30 18:31:46.000000 assemblyai-0.4.0/assemblyai/transcriber.py
--rw-r--r--   0 runner    (1001) docker     (123)    44868 2023-05-30 18:31:46.000000 assemblyai-0.4.0/assemblyai/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:31:57.952522 assemblyai-0.4.0/assemblyai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-05-30 18:31:57.000000 assemblyai-0.4.0/assemblyai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-30 18:31:57.000000 assemblyai-0.4.0/assemblyai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 18:31:57.000000 assemblyai-0.4.0/assemblyai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-30 18:31:57.000000 assemblyai-0.4.0/assemblyai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-30 18:31:57.000000 assemblyai-0.4.0/assemblyai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 18:31:57.952522 assemblyai-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-30 18:31:46.000000 assemblyai-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:31:57.952522 assemblyai-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:31:46.000000 assemblyai-0.4.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:31:57.952522 assemblyai-0.4.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:31:46.000000 assemblyai-0.4.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-30 18:31:46.000000 assemblyai-0.4.0/tests/unit/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-05-30 18:31:46.000000 assemblyai-0.4.0/tests/unit/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-30 18:31:46.000000 assemblyai-0.4.0/tests/unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-30 18:31:46.000000 assemblyai-0.4.0/tests/unit/test_domains.py
--rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-05-30 18:31:46.000000 assemblyai-0.4.0/tests/unit/test_lemur.py
--rw-r--r--   0 runner    (1001) docker     (123)    13292 2023-05-30 18:31:46.000000 assemblyai-0.4.0/tests/unit/test_transcriber.py
--rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-05-30 18:31:46.000000 assemblyai-0.4.0/tests/unit/test_transcript.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:20:30.358389 assemblyai-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-31 19:20:18.000000 assemblyai-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-05-31 19:20:30.358389 assemblyai-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-05-31 19:20:18.000000 assemblyai-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:20:30.354390 assemblyai-0.4.1/assemblyai/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-31 19:20:18.000000 assemblyai-0.4.1/assemblyai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-05-31 19:20:18.000000 assemblyai-0.4.1/assemblyai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-31 19:20:18.000000 assemblyai-0.4.1/assemblyai/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-05-31 19:20:18.000000 assemblyai-0.4.1/assemblyai/lemur.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22107 2023-05-31 19:20:18.000000 assemblyai-0.4.1/assemblyai/transcriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44877 2023-05-31 19:20:18.000000 assemblyai-0.4.1/assemblyai/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:20:30.354390 assemblyai-0.4.1/assemblyai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-05-31 19:20:30.000000 assemblyai-0.4.1/assemblyai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-31 19:20:30.000000 assemblyai-0.4.1/assemblyai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 19:20:30.000000 assemblyai-0.4.1/assemblyai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-31 19:20:30.000000 assemblyai-0.4.1/assemblyai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-31 19:20:30.000000 assemblyai-0.4.1/assemblyai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 19:20:30.358389 assemblyai-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-31 19:20:18.000000 assemblyai-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:20:30.354390 assemblyai-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 19:20:18.000000 assemblyai-0.4.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:20:30.358389 assemblyai-0.4.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 19:20:18.000000 assemblyai-0.4.1/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-31 19:20:18.000000 assemblyai-0.4.1/tests/unit/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-05-31 19:20:18.000000 assemblyai-0.4.1/tests/unit/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-31 19:20:18.000000 assemblyai-0.4.1/tests/unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-31 19:20:18.000000 assemblyai-0.4.1/tests/unit/test_domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-05-31 19:20:18.000000 assemblyai-0.4.1/tests/unit/test_lemur.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13291 2023-05-31 19:20:18.000000 assemblyai-0.4.1/tests/unit/test_transcriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9415 2023-05-31 19:20:18.000000 assemblyai-0.4.1/tests/unit/test_transcript.py
```

### Comparing `assemblyai-0.4.0/LICENSE` & `assemblyai-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `assemblyai-0.4.0/PKG-INFO` & `assemblyai-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyai
-Version: 0.4.0
+Version: 0.4.1
 Summary: AssemblyAI Python SDK
 Home-page: https://github.com/AssemblyAI/assemblyai-python-sdk
 Author: AssemblyAI
 Author-email: engineering.sdk@assemblyai.com
 License: MIT License
 Project-URL: Code, https://github.com/AssemblyAI/assemblyai-python-sdk
 Project-URL: Issues, https://github.com/AssemblyAI/assemblyai-python-sdk/issues
```

### Comparing `assemblyai-0.4.0/README.md` & `assemblyai-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `assemblyai-0.4.0/assemblyai/__init__.py` & `assemblyai-0.4.1/assemblyai/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,36 @@
-from .transcriber import Transcriber, Transcript, TranscriptGroup
 from .client import Client
 from .lemur import Lemur
-
+from .transcriber import Transcriber, Transcript, TranscriptGroup
 from .types import (
     AssemblyAIError,
-    Settings,
-    TranscriptError,
-    TranscriptStatus,
-    TranscriptionConfig,
-    Utterance,
-    UtteranceWord,
     LanguageCode,
-    Paragraph,
-    Sentence,
-    LemurModel,
     LemurError,
+    LemurModel,
     LemurQuestion,
     LemurQuestionResult,
-    SummarizationModel,
+    Paragraph,
+    PIIRedactionPolicy,
     PIISubstitutionPolicy,
     RawTranscriptionConfig,
+    Sentence,
+    Settings,
+    SummarizationModel,
     SummarizationType,
+    Timestamp,
+    TranscriptError,
+    TranscriptionConfig,
+    TranscriptStatus,
+    Utterance,
+    UtteranceWord,
+    Word,
     WordBoost,
     WordSearchMatch,
-    Word,
-    Timestamp,
-    PIIRedactionPolicy,
 )
 
-
 settings = Settings()
 """Global settings object that applies to all classes that use the `Client` class."""
 
 
 __all__ = [
     # types
     "AssemblyAIError",
```

### Comparing `assemblyai-0.4.0/assemblyai/api.py` & `assemblyai-0.4.1/assemblyai/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from typing import Optional, List, BinaryIO
-
-from . import types
+from typing import BinaryIO, List, Optional
 
 import httpx
 
+from . import types
+
 
 def _get_error_message(response: httpx.Response) -> str:
     """
     Tries to retrieve the `error` field if the response is JSON, otherwise
     returns the response text.
 
     Args:
```

### Comparing `assemblyai-0.4.0/assemblyai/client.py` & `assemblyai-0.4.1/assemblyai/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import threading
-from typing import Optional, ClassVar
+from typing import ClassVar, Optional
+
+import httpx
 from typing_extensions import Self
 
 from . import types
 
-import httpx
-
 
 class Client:
     _default: ClassVar[Optional["Client"]] = None
     _lock: ClassVar[threading.Lock] = threading.Lock()
 
     def __init__(
         self,
```

### Comparing `assemblyai-0.4.0/assemblyai/lemur.py` & `assemblyai-0.4.1/assemblyai/lemur.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from typing import Optional, List, Union, Dict, Any
+from typing import Any, Dict, List, Optional, Union
 
-from . import api, types
+from . import api
 from . import client as _client
+from . import types
 
 
 class _LemurImpl:
     def __init__(
         self,
         *,
         client: _client.Client,
```

### Comparing `assemblyai-0.4.0/assemblyai/transcriber.py` & `assemblyai-0.4.1/assemblyai/transcriber.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from __future__ import annotations
+
+import concurrent.futures
 import os
 import time
+from typing import Dict, Iterator, List, Optional, Union
 from urllib.parse import urlparse
-import concurrent.futures
-from typing import Dict, Iterator, Optional, List, Union
+
 from typing_extensions import Self
 
-from . import lemur, types, api
+from . import api
 from . import client as _client
+from . import lemur, types
 
 
 class _TranscriptImpl:
     def __init__(
         self,
         *,
         client: _client.Client,
@@ -210,14 +213,53 @@
     @property
     def error(self) -> Optional[str]:
         "The error message in case the transcription fails"
 
         return self._impl.transcript.error
 
     @property
+    def words(self) -> Optional[List[types.Word]]:
+        "The list of words in the transcript"
+
+        return self._impl.transcript.words
+
+    @property
+    def utterances(self) -> Optional[List[types.Utterance]]:
+        """
+        When `dual_channel` or `speaker_labels` is enabled,
+        a list of utterances in the transcript.
+        """
+
+        return self._impl.transcript.utterances
+
+    @property
+    def confidence(self) -> Optional[float]:
+        "The confidence our model has in the transcribed text, between 0 and 1"
+
+        return self._impl.transcript.confidence
+
+    @property
+    def audio_duration(self) -> Optional[float]:
+        "The duration of the audio in seconds"
+
+        return self._impl.transcript.audio_duration
+
+    @property
+    def webhook_status_code(self) -> Optional[int]:
+        "The status code we received from your server when delivering your webhook"
+
+        return self._impl.transcript.webhook_status_code
+
+    @property
+    def webhook_auth(self) -> Optional[bool]:
+        "Whether the webhook was sent with an HTTP authentication header"
+
+        return self._impl.transcript.webhook_auth
+
+    @property
     def lemur(self) -> lemur.Lemur:
         """
         Access AssemblyAI's LeMUR features.
         """
 
         return lemur.Lemur(
             client=self._client,
```

### Comparing `assemblyai-0.4.0/assemblyai/types.py` & `assemblyai-0.4.1/assemblyai/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from enum import Enum
-
-from typing import Optional, Dict, Any, List, Tuple, Union, Sequence
-from typing_extensions import Self
+from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
 
 from pydantic import BaseModel, BaseSettings, Extra
+from typing_extensions import Self
 
 
 class AssemblyAIError(Exception):
     """
     Base exception for all AssemblyAI errors
     """
 
@@ -1267,15 +1266,15 @@
 
     # content_safety: bool = False
     # "Enable Content Safety Detection."
 
     # iab_categories: bool = False
     # "Enable Topic Detection."
 
-    custom_spelling: Optional[List[dict]]
+    custom_spelling: Optional[List[Dict[str, str]]]
     "Customize how words are spelled and formatted using to and from values"
 
     disfluencies: Optional[bool]
     "Transcribe Filler Words, like 'umm', in your media file."
 
     # sentiment_analysis: bool = False
     # "Enable Sentiment Analysis."
@@ -1343,15 +1342,15 @@
 
     confidence: Optional[float]
     "The confidence our model has in the transcribed text, between 0.0 and 1.0"
 
     audio_duration: Optional[float]
     "The duration of your media file, in seconds"
 
-    webhook_status_code: Optional[str]
+    webhook_status_code: Optional[int]
     "The status code we received from your server when delivering your webhook"
     webhook_auth: Optional[bool]
     "Whether the webhook was sent with an HTTP authentication header"
 
     # auto_highlights_result: Optional[AutohighlightResponse] = None
     # "The list of results when enabling Automatic Transcript Highlights"
```

### Comparing `assemblyai-0.4.0/assemblyai.egg-info/PKG-INFO` & `assemblyai-0.4.1/assemblyai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyai
-Version: 0.4.0
+Version: 0.4.1
 Summary: AssemblyAI Python SDK
 Home-page: https://github.com/AssemblyAI/assemblyai-python-sdk
 Author: AssemblyAI
 Author-email: engineering.sdk@assemblyai.com
 License: MIT License
 Project-URL: Code, https://github.com/AssemblyAI/assemblyai-python-sdk
 Project-URL: Issues, https://github.com/AssemblyAI/assemblyai-python-sdk/issues
```

### Comparing `assemblyai-0.4.0/assemblyai.egg-info/SOURCES.txt` & `assemblyai-0.4.1/assemblyai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `assemblyai-0.4.0/setup.py` & `assemblyai-0.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from pathlib import Path
 
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="assemblyai",
-    version="0.4.0",
+    version="0.4.1",
     description="AssemblyAI Python SDK",
     author="AssemblyAI",
     author_email="engineering.sdk@assemblyai.com",
     packages=find_packages(),
     install_requires=[
         "httpx>=0.19.0",
         "pydantic>=1.7.0",
```

### Comparing `assemblyai-0.4.0/tests/unit/factories.py` & `assemblyai-0.4.1/tests/unit/factories.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Contains factories that are used for mocking certain requests/responses
 from AssemblyAI's API.
 """
 
 from functools import partial
-from typing import Any, Dict, Callable
+from typing import Any, Callable, Dict
 
 import factory
 import factory.base
 
 import assemblyai as aai
 from assemblyai import types
```

### Comparing `assemblyai-0.4.0/tests/unit/test_domains.py` & `assemblyai-0.4.1/tests/unit/test_domains.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.4.0/tests/unit/test_lemur.py` & `assemblyai-0.4.1/tests/unit/test_lemur.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-import httpx
-from pytest_httpx import HTTPXMock
 import uuid
 
+import httpx
+import pytest
+from pytest_httpx import HTTPXMock
 
 import assemblyai as aai
 from tests.unit import factories
 
-import pytest
-
-
 aai.settings.api_key = "test"
 
 
 def test_lemur_single_question_succeeds(httpx_mock: HTTPXMock):
     """
     Tests whether asking a single question succeeds.
     """
```

### Comparing `assemblyai-0.4.0/tests/unit/test_transcriber.py` & `assemblyai-0.4.1/tests/unit/test_transcriber.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-import httpx
-from pytest_httpx import HTTPXMock
-from unittest.mock import patch, mock_open
-import os
 import copy
+import os
+from unittest.mock import mock_open, patch
 
+import httpx
 import pytest
-
+from pytest_httpx import HTTPXMock
 
 import assemblyai as aai
 from tests.unit import factories
 
 aai.settings.api_key = "test"
```

### Comparing `assemblyai-0.4.0/tests/unit/test_transcript.py` & `assemblyai-0.4.1/tests/unit/test_transcript.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from typing import Any, Dict, List
+
 import httpx
+import pytest
+from faker import Faker
 from pytest_httpx import HTTPXMock
 
-
 import assemblyai as aai
 from tests.unit import factories
 
-import pytest
-from faker import Faker
-
-
 aai.settings.api_key = "test"
 
 
 def test_export_subtitles_succeeds(httpx_mock: HTTPXMock, faker: Faker):
     """
     Tests whether exporting subtitles succeed.
     """
```

