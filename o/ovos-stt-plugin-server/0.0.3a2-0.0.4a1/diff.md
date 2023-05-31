# Comparing `tmp/ovos_stt_plugin_server-0.0.3a2-py3-none-any.whl.zip` & `tmp/ovos_stt_plugin_server-0.0.4a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 9336 bytes, number of entries: 9
--rw-r--r--  2.0 unx     7339 b- defN 23-May-04 14:45 ovos_stt_plugin_server/__init__.py
--rw-r--r--  2.0 unx      177 b- defN 23-May-04 14:45 ovos_stt_plugin_server/version.py
--rw-r--r--  2.0 unx    11343 b- defN 23-May-04 14:45 ovos_stt_plugin_server-0.0.3a2.dist-info/LICENSE
--rw-r--r--  2.0 unx     1654 b- defN 23-May-04 14:45 ovos_stt_plugin_server-0.0.3a2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-04 14:45 ovos_stt_plugin_server-0.0.3a2.dist-info/WHEEL
--rw-r--r--  2.0 unx      278 b- defN 23-May-04 14:45 ovos_stt_plugin_server-0.0.3a2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       23 b- defN 23-May-04 14:45 ovos_stt_plugin_server-0.0.3a2.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-May-04 14:45 ovos_stt_plugin_server-0.0.3a2.dist-info/zip-safe
--rw-rw-r--  2.0 unx      868 b- defN 23-May-04 14:45 ovos_stt_plugin_server-0.0.3a2.dist-info/RECORD
-9 files, 21775 bytes uncompressed, 7796 bytes compressed:  64.2%
+Zip file size: 9030 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     6096 b- defN 23-May-31 14:26 ovos_stt_plugin_server/__init__.py
+-rw-r--r--  2.0 unx      177 b- defN 23-May-31 14:26 ovos_stt_plugin_server/version.py
+-rw-r--r--  2.0 unx    11343 b- defN 23-May-31 14:26 ovos_stt_plugin_server-0.0.4a1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1654 b- defN 23-May-31 14:26 ovos_stt_plugin_server-0.0.4a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-31 14:26 ovos_stt_plugin_server-0.0.4a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx      278 b- defN 23-May-31 14:26 ovos_stt_plugin_server-0.0.4a1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       23 b- defN 23-May-31 14:26 ovos_stt_plugin_server-0.0.4a1.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-May-31 14:26 ovos_stt_plugin_server-0.0.4a1.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      868 b- defN 23-May-31 14:26 ovos_stt_plugin_server-0.0.4a1.dist-info/RECORD
+9 files, 20532 bytes uncompressed, 7490 bytes compressed:  63.5%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
 Filename: ovos_stt_plugin_server/__init__.py
 Comment: 
 
 Filename: ovos_stt_plugin_server/version.py
 Comment: 
 
-Filename: ovos_stt_plugin_server-0.0.3a2.dist-info/LICENSE
+Filename: ovos_stt_plugin_server-0.0.4a1.dist-info/LICENSE
 Comment: 
 
-Filename: ovos_stt_plugin_server-0.0.3a2.dist-info/METADATA
+Filename: ovos_stt_plugin_server-0.0.4a1.dist-info/METADATA
 Comment: 
 
-Filename: ovos_stt_plugin_server-0.0.3a2.dist-info/WHEEL
+Filename: ovos_stt_plugin_server-0.0.4a1.dist-info/WHEEL
 Comment: 
 
-Filename: ovos_stt_plugin_server-0.0.3a2.dist-info/entry_points.txt
+Filename: ovos_stt_plugin_server-0.0.4a1.dist-info/entry_points.txt
 Comment: 
 
-Filename: ovos_stt_plugin_server-0.0.3a2.dist-info/top_level.txt
+Filename: ovos_stt_plugin_server-0.0.4a1.dist-info/top_level.txt
 Comment: 
 
-Filename: ovos_stt_plugin_server-0.0.3a2.dist-info/zip-safe
+Filename: ovos_stt_plugin_server-0.0.4a1.dist-info/zip-safe
 Comment: 
 
-Filename: ovos_stt_plugin_server-0.0.3a2.dist-info/RECORD
+Filename: ovos_stt_plugin_server-0.0.4a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ovos_stt_plugin_server/__init__.py

```diff
@@ -1,27 +1,38 @@
 from queue import Queue
 from uuid import uuid4
 
 import requests
-from ovos_plugin_manager.stt import STT
-from ovos_plugin_manager.stt import StreamingSTT, StreamThread
+from ovos_utils.log import LOG
+from ovos_plugin_manager.stt import STT, StreamingSTT, StreamThread
 
 
 class OVOSHTTPServerSTT(STT):
     """STT interface for the OVOS-HTTP-STT-Server"""
+    public_servers = [
+        "https://stt.openvoiceos.org/stt"
+    ]
 
     def __init__(self, config=None):
         super().__init__(config)
-        self.url = self.config.get("url") or "https://stt.strongthany.cc/stt"
+        self.urls = self.config.get("url") or self.config.get("urls") or self.public_servers
+        if not isinstance(self.urls, list):
+            self.urls = [self.urls]
 
     def execute(self, audio, language=None):
-        self.response = requests.post(self.url, data=audio.get_wav_data(),
-                                      headers={"Content-Type": "audio/wav"},
-                                      params={"lang": language or self.lang})
-        return self.response.text if self.response else None
+        for url in self.urls:
+            try:
+                self.response = requests.post(url, data=audio.get_wav_data(),
+                                              headers={"Content-Type": "audio/wav"},
+                                              params={"lang": language or self.lang})
+                if self.response:
+                    return self.response.text
+            except:
+                pass
+            LOG.error(f"STT request to {url} failed")
 
 
 class OVOSHTTPStreamServerStreamThread(StreamThread):
     def __init__(self, queue, language, url="https://stt.strongthany.cc/stream"):
         super().__init__(queue, language)
         self.url = url
         self.session = requests.Session()
@@ -62,212 +73,136 @@
         self.queue = Queue()
 
         stream = OVOSHTTPStreamServerStreamThread(self.queue, self.lang, url)
         stream.reset_model()
         return stream
 
 
-# will list the public instances of google STT proxies as valid configs
-# but thats not the main intended usage of this plugin
 
+# public instances
+OVOSHTTPServerSTTConfig = {}
 
-# taken from https://stackoverflow.com/questions/14257598/what-are-language-codes-in-chromes-implementation-of-the-html5-speech-recogniti/14302134#14302134
-_lang = {
-    "Afrikaans": [
-        ["South Africa", "af-ZA"]
-    ],
-    "Arabic": [
-        ["Algeria", "ar-DZ"],
-        ["Bahrain", "ar-BH"],
-        ["Egypt", "ar-EG"],
-        ["Israel", "ar-IL"],
-        ["Iraq", "ar-IQ"],
-        ["Jordan", "ar-JO"],
-        ["Kuwait", "ar-KW"],
-        ["Lebanon", "ar-LB"],
-        ["Morocco", "ar-MA"],
-        ["Oman", "ar-OM"],
-        ["Palestinian Territory", "ar-PS"],
-        ["Qatar", "ar-QA"],
-        ["Saudi Arabia", "ar-SA"],
-        ["Tunisia", "ar-TN"],
-        ["UAE", "ar-AE"]
-    ],
-    "Basque": [
-        ["Spain", "eu-ES"]
-    ],
-    "Bulgarian": [
-        ["Bulgaria", "bg-BG"]
-    ],
-    "Catalan": [
-        ["Spain", "ca-ES"]
-    ],
-    "Chinese Mandarin": [
-        ["China (Simp.)", "cmn-Hans-CN"],
-        ["Hong Kong SAR (Trad.)", "cmn-Hans-HK"],
-        ["Taiwan (Trad.)", "cmn-Hant-TW"]
-    ],
-    "Chinese Cantonese": [
-        ["Hong Kong", "yue-Hant-HK"]
-    ],
-    "Croatian": [
-        ["Croatia", "hr_HR"]
-    ],
-    "Czech": [
-        ["Czech Republic", "cs-CZ"]
-    ],
-    "Danish": [
-        ["Denmark", "da-DK"]
-    ],
-    "English": [
-        ["Australia", "en-AU"],
-        ["Canada", "en-CA"],
-        ["India", "en-IN"],
-        ["Ireland", "en-IE"],
-        ["New Zealand", "en-NZ"],
-        ["Philippines", "en-PH"],
-        ["South Africa", "en-ZA"],
-        ["United Kingdom", "en-GB"],
-        ["United States", "en-US"]
-    ],
-    "Farsi": [
-        ["Iran", "fa-IR"]
-    ],
-    "French": [
-        ["France", "fr-FR"]
-    ],
-    "Filipino": [
-        ["Philippines", "fil-PH"]
-    ],
-    "Galician": [
-        ["Spain", "gl-ES"]
-    ],
-    "German": [
-        ["Germany", "de-DE"]
-    ],
-    "Greek": [
-        ["Greece", "el-GR"]
-    ],
-    "Finnish": [
-        ["Finland", "fi-FI"]
-    ],
-    "Hebrew": [
-        ["Israel", "he-IL"]
-    ],
-    "Hindi": [
-        ["India", "hi-IN"]
-    ],
-    "Hungarian": [
-        ["Hungary", "hu-HU"]
-    ],
-    "Indonesian": [
-        ["Indonesia", "id-ID"]
-    ],
-    "Icelandic": [
-        ["Iceland", "is-IS"]
-    ],
-    "Italian": [
-        ["Italy", "it-IT"],
-        ["Switzerland", "it-CH"]
-    ],
-    "Japanese": [
-        ["Japan", "ja-JP"]
-    ],
-    "Korean": [
-        ["Korea", "ko-KR"]
-    ],
-    "Lithuanian": [
-        ["Lithuania", "lt-LT"]
-    ],
-    "Malaysian": [
-        ["Malaysia", "ms-MY"]
-    ],
-    "Dutch": [
-        ["Netherlands", "nl-NL"]
-    ],
-    "Norwegian": [
-        ["Norway", "nb-NO"]
-    ],
-    "Polish": [
-        ["Poland", "pl-PL"]
-    ],
-    "Portuguese": [
-        ["Brazil", "pt-BR"],
-        ["Portugal", "pt-PT"]
-    ],
-    "Romanian": [
-        ["Romania", "ro-RO"]
-    ],
-    "Russian": [
-        ["Russia", "ru-RU"]
-    ],
-    "Serbian": [
-        ["Serbia", "sr-RS"]
-    ],
-    "Slovak": [
-        ["Slovakia", "sk-SK"]
-    ],
-    "Slovenian": [
-        ["Slovenia", "sl-SI"]
-    ],
-    "Spanish": [
-        ["Argentina", "es-AR"],
-        ["Bolivia", "es-BO"],
-        ["Chile", "es-CL"],
-        ["Colombia", "es-CO"],
-        ["Costa Rica", "es-CR"],
-        ["Dominican Republic", "es-DO"],
-        ["Ecuador", "es-EC"],
-        ["El Salvador", "es-SV"],
-        ["Guatemala", "es-GT"],
-        ["Honduras", "es-HN"],
-        ["México", "es-MX"],
-        ["Nicaragua", "es-NI"],
-        ["Panamá", "es-PA"],
-        ["Paraguay", "es-PY"],
-        ["Perú", "es-PE"],
-        ["Puerto Rico", "es-PR"],
-        ["Spain", "es-ES"],
-        ["Uruguay", "es-UY"],
-        ["United States", "es-US"],
-        ["Venezuela", "es-VE"]
-    ],
-    "Swedish": [
-        ["Sweden", "sv-SE"]
-    ],
-    "Thai": [
-        ["Thailand", "th-TH"]
-    ],
-    "Turkish": [
-        ["Turkey", "tr-TR"]
-    ],
-    "Ukrainian": [
-        ["Ukraine", "uk-UA"]
-    ],
-    "Vietnamese": [
-        ["Viet Nam", "vi-VN"]
-    ],
-    "Zulu": [
-        ["South Africa", "zu-ZA"]
+_whisper_lang = {
+        "en": "english",
+        "zh": "chinese",
+        "de": "german",
+        "es": "spanish",
+        "ru": "russian",
+        "ko": "korean",
+        "fr": "french",
+        "ja": "japanese",
+        "pt": "portuguese",
+        "tr": "turkish",
+        "pl": "polish",
+        "ca": "catalan",
+        "nl": "dutch",
+        "ar": "arabic",
+        "sv": "swedish",
+        "it": "italian",
+        "id": "indonesian",
+        "hi": "hindi",
+        "fi": "finnish",
+        "vi": "vietnamese",
+        "iw": "hebrew",
+        "uk": "ukrainian",
+        "el": "greek",
+        "ms": "malay",
+        "cs": "czech",
+        "ro": "romanian",
+        "da": "danish",
+        "hu": "hungarian",
+        "ta": "tamil",
+        "no": "norwegian",
+        "th": "thai",
+        "ur": "urdu",
+        "hr": "croatian",
+        "bg": "bulgarian",
+        "lt": "lithuanian",
+        "la": "latin",
+        "mi": "maori",
+        "ml": "malayalam",
+        "cy": "welsh",
+        "sk": "slovak",
+        "te": "telugu",
+        "fa": "persian",
+        "lv": "latvian",
+        "bn": "bengali",
+        "sr": "serbian",
+        "az": "azerbaijani",
+        "sl": "slovenian",
+        "kn": "kannada",
+        "et": "estonian",
+        "mk": "macedonian",
+        "br": "breton",
+        "eu": "basque",
+        "is": "icelandic",
+        "hy": "armenian",
+        "ne": "nepali",
+        "mn": "mongolian",
+        "bs": "bosnian",
+        "kk": "kazakh",
+        "sq": "albanian",
+        "sw": "swahili",
+        "gl": "galician",
+        "mr": "marathi",
+        "pa": "punjabi",
+        "si": "sinhala",
+        "km": "khmer",
+        "sn": "shona",
+        "yo": "yoruba",
+        "so": "somali",
+        "af": "afrikaans",
+        "oc": "occitan",
+        "ka": "georgian",
+        "be": "belarusian",
+        "tg": "tajik",
+        "sd": "sindhi",
+        "gu": "gujarati",
+        "am": "amharic",
+        "yi": "yiddish",
+        "lo": "lao",
+        "uz": "uzbek",
+        "fo": "faroese",
+        "ht": "haitian creole",
+        "ps": "pashto",
+        "tk": "turkmen",
+        "nn": "nynorsk",
+        "mt": "maltese",
+        "sa": "sanskrit",
+        "lb": "luxembourgish",
+        "my": "myanmar",
+        "bo": "tibetan",
+        "tl": "tagalog",
+        "mg": "malagasy",
+        "as": "assamese",
+        "tt": "tatar",
+        "haw": "hawaiian",
+        "ln": "lingala",
+        "ha": "hausa",
+        "ba": "bashkir",
+        "jw": "javanese",
+        "su": "sundanese",
+    }
+
+for code, lang in _whisper_lang.items():
+    OVOSHTTPServerSTTConfig[code] = [
+        {"lang": code,
+         "url": "https://stt.openvoiceos.org/stt",
+         "meta": {
+             "priority": 30,
+             "display_name": f"OVOS FasterWhisper (small)",
+             "offline": False}
+         }
     ]
-}
 
-OVOSHTTPServerSTTConfig = {}
+if __name__ == "__main__":
+    from speech_recognition import Recognizer, AudioFile
+
+    engine = OVOSHTTPServerSTT()
+
+    # inference
+    jfk = "/home/miro/PycharmProjects/ovos-stt-plugin-fasterwhisper/jfk.wav"
+    with AudioFile(jfk) as source:
+        audio = Recognizer().record(source)
 
-for lang, data in _lang.items():
-    for region, code in data:
-        OVOSHTTPServerSTTConfig[code] = [
-            {"lang": code,
-             "url": "https://stt.openvoiceos.com",
-             "meta": {
-                 "priority": 30,
-                 "display_name": f"OVOS Google Proxy {lang} ({region})",
-                 "offline": False}
-             },
-            {"lang": code,
-             "url": "https://stt.strongthany.cc",
-             "meta": {
-                 "priority": 80,
-                 "display_name": f"Strongthany Google Proxy {lang} ({region})",
-                 "offline": False}
-             }
-        ]
+    pred = engine.execute(audio)
+    print(pred)
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## ovos_stt_plugin_server/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 0
-VERSION_BUILD = 3
-VERSION_ALPHA = 2
+VERSION_BUILD = 4
+VERSION_ALPHA = 1
 # END_VERSION_BLOCK
```

## Comparing `ovos_stt_plugin_server-0.0.3a2.dist-info/LICENSE` & `ovos_stt_plugin_server-0.0.4a1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ovos_stt_plugin_server-0.0.3a2.dist-info/METADATA` & `ovos_stt_plugin_server-0.0.4a1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-stt-plugin-server
-Version: 0.0.3a2
+Version: 0.0.4a1
 Summary: ovos stt server plugin for mycroft
 Home-page: https://github.com/OpenVoiceOS/ovos-stt-server-plugin
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Keywords: mycroft OpenVoiceOS OVOS plugin stt
 Platform: UNKNOWN
```

