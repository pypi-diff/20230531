# Comparing `tmp/neuralpit-1.0.7.tar.gz` & `tmp/neuralpit-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralpit-1.0.7.tar", last modified: Wed May 31 14:10:03 2023, max compression
+gzip compressed data, was "neuralpit-1.0.8.tar", last modified: Wed May 31 15:08:25 2023, max compression
```

## Comparing `neuralpit-1.0.7.tar` & `neuralpit-1.0.8.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:10:03.672956 neuralpit-1.0.7/
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 14:09:22.000000 neuralpit-1.0.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      574 2023-05-31 14:10:03.672956 neuralpit-1.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      184 2023-05-31 14:09:22.000000 neuralpit-1.0.7/README.md
--rw-r--r--   0 root         (0) root         (0)     1029 2023-05-31 14:09:22.000000 neuralpit-1.0.7/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 14:10:03.672956 neuralpit-1.0.7/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:10:03.672956 neuralpit-1.0.7/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:10:03.672956 neuralpit-1.0.7/src/neuralpit/
--rw-r--r--   0 root         (0) root         (0)      211 2023-05-31 14:09:22.000000 neuralpit-1.0.7/src/neuralpit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1175 2023-05-31 14:09:22.000000 neuralpit-1.0.7/src/neuralpit/context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:10:03.672956 neuralpit-1.0.7/src/neuralpit/services/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 14:09:22.000000 neuralpit-1.0.7/src/neuralpit/services/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1196 2023-05-31 14:09:22.000000 neuralpit-1.0.7/src/neuralpit/services/api.py
--rw-r--r--   0 root         (0) root         (0)     1135 2023-05-31 14:09:22.000000 neuralpit-1.0.7/src/neuralpit/services/converter.py
--rw-r--r--   0 root         (0) root         (0)      368 2023-05-31 14:09:22.000000 neuralpit-1.0.7/src/neuralpit/services/converterFactory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:10:03.672956 neuralpit-1.0.7/src/neuralpit/tools/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 14:09:22.000000 neuralpit-1.0.7/src/neuralpit/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2474 2023-05-31 14:09:22.000000 neuralpit-1.0.7/src/neuralpit/tools/chat.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:10:03.672956 neuralpit-1.0.7/src/neuralpit/utils/
--rw-r--r--   0 root         (0) root         (0)      631 2023-05-31 14:09:22.000000 neuralpit-1.0.7/src/neuralpit/utils/indexer.py
--rw-r--r--   0 root         (0) root         (0)     2003 2023-05-31 14:09:22.000000 neuralpit-1.0.7/src/neuralpit/utils/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:10:03.672956 neuralpit-1.0.7/src/neuralpit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      574 2023-05-31 14:10:03.000000 neuralpit-1.0.7/src/neuralpit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      613 2023-05-31 14:10:03.000000 neuralpit-1.0.7/src/neuralpit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 14:10:03.000000 neuralpit-1.0.7/src/neuralpit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       84 2023-05-31 14:10:03.000000 neuralpit-1.0.7/src/neuralpit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-31 14:10:03.000000 neuralpit-1.0.7/src/neuralpit.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 14:10:03.672956 neuralpit-1.0.7/test/
--rw-r--r--   0 root         (0) root         (0)      546 2023-05-31 14:09:22.000000 neuralpit-1.0.7/test/testDocChat.py
--rw-r--r--   0 root         (0) root         (0)      594 2023-05-31 14:09:22.000000 neuralpit-1.0.7/test/testGetServiceProfile.py
--rw-r--r--   0 root         (0) root         (0)      264 2023-05-31 14:09:22.000000 neuralpit-1.0.7/test/testGetUserProfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:08:25.458119 neuralpit-1.0.8/
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 15:07:42.000000 neuralpit-1.0.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      574 2023-05-31 15:08:25.458119 neuralpit-1.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      184 2023-05-31 15:07:42.000000 neuralpit-1.0.8/README.md
+-rw-r--r--   0 root         (0) root         (0)     1029 2023-05-31 15:07:42.000000 neuralpit-1.0.8/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 15:08:25.458119 neuralpit-1.0.8/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:08:25.454119 neuralpit-1.0.8/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:08:25.454119 neuralpit-1.0.8/src/neuralpit/
+-rw-r--r--   0 root         (0) root         (0)      211 2023-05-31 15:07:42.000000 neuralpit-1.0.8/src/neuralpit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1175 2023-05-31 15:07:42.000000 neuralpit-1.0.8/src/neuralpit/context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:08:25.458119 neuralpit-1.0.8/src/neuralpit/services/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 15:07:42.000000 neuralpit-1.0.8/src/neuralpit/services/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1196 2023-05-31 15:07:42.000000 neuralpit-1.0.8/src/neuralpit/services/api.py
+-rw-r--r--   0 root         (0) root         (0)      986 2023-05-31 15:07:42.000000 neuralpit-1.0.8/src/neuralpit/services/converter.py
+-rw-r--r--   0 root         (0) root         (0)      368 2023-05-31 15:07:42.000000 neuralpit-1.0.8/src/neuralpit/services/converterFactory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:08:25.458119 neuralpit-1.0.8/src/neuralpit/tools/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 15:07:42.000000 neuralpit-1.0.8/src/neuralpit/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2477 2023-05-31 15:07:42.000000 neuralpit-1.0.8/src/neuralpit/tools/chat.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:08:25.458119 neuralpit-1.0.8/src/neuralpit/utils/
+-rw-r--r--   0 root         (0) root         (0)     1849 2023-05-31 15:07:42.000000 neuralpit-1.0.8/src/neuralpit/utils/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:08:25.454119 neuralpit-1.0.8/src/neuralpit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      574 2023-05-31 15:08:25.000000 neuralpit-1.0.8/src/neuralpit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      582 2023-05-31 15:08:25.000000 neuralpit-1.0.8/src/neuralpit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 15:08:25.000000 neuralpit-1.0.8/src/neuralpit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2023-05-31 15:08:25.000000 neuralpit-1.0.8/src/neuralpit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-31 15:08:25.000000 neuralpit-1.0.8/src/neuralpit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 15:08:25.458119 neuralpit-1.0.8/test/
+-rw-r--r--   0 root         (0) root         (0)      489 2023-05-31 15:07:42.000000 neuralpit-1.0.8/test/testDocChat.py
+-rw-r--r--   0 root         (0) root         (0)      594 2023-05-31 15:07:42.000000 neuralpit-1.0.8/test/testGetServiceProfile.py
+-rw-r--r--   0 root         (0) root         (0)      264 2023-05-31 15:07:42.000000 neuralpit-1.0.8/test/testGetUserProfile.py
```

### Comparing `neuralpit-1.0.7/PKG-INFO` & `neuralpit-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralpit
-Version: 1.0.7
+Version: 1.0.8
 Summary: NeuralPit SDK
 Author-email: Quang Nguyen <quang.nguyen@neuralpit.com>
 Keywords: api,neural,neuralpit
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `neuralpit-1.0.7/pyproject.toml` & `neuralpit-1.0.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "neuralpit"
-version = "1.0.7"
+version = "1.0.8"
 description = "NeuralPit SDK"
 readme = "README.md"
 authors = [{ name = "Quang Nguyen", email = "quang.nguyen@neuralpit.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `neuralpit-1.0.7/src/neuralpit/context.py` & `neuralpit-1.0.8/src/neuralpit/context.py`

 * *Files identical despite different names*

### Comparing `neuralpit-1.0.7/src/neuralpit/services/api.py` & `neuralpit-1.0.8/src/neuralpit/services/api.py`

 * *Files identical despite different names*

### Comparing `neuralpit-1.0.7/src/neuralpit/services/converter.py` & `neuralpit-1.0.8/src/neuralpit/services/converter.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,29 +8,26 @@
 class TikaConverterService():
 
     def __init__(self, tika_server_url) -> None:
         super().__init__()
         self.api_key = Enviroment.getApiKey()
         self.tika_server_url = tika_server_url
 
-    def convertFileToString(self, file_content) -> List[str]:
+    def getFilePages(self, file_content) -> List[str]:
         headers = {'x-api-key':self.api_key, 'Accept': 'application/json'}
         resp = requests.put(self.tika_server_url+"/tika", headers = headers, data = file_content)
         resp_json = json.loads(resp.content)
         file_content = resp_json['X-TIKA:content']
         soup = BeautifulSoup(file_content, features="lxml")
         pages = soup.find_all("div", {"class": "page"})
         return [page.get_text() for page in pages] 
 
-    def convertImageToString(self, file) -> List[str]:
-        pass
 
 class LocalConverterService():
 
     def __init__(self) -> None:
         super().__init__()
 
-    def convertFileToString(self, file) -> List[str]:
+    def getFilePages(self, file) -> List[str]:
         pass
 
-    def convertImageToString(self, file) -> List[str]:
-        pass
+
```

### Comparing `neuralpit-1.0.7/src/neuralpit/tools/chat.py` & `neuralpit-1.0.8/src/neuralpit/tools/chat.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import openai
-from langchain.chains import LLMChain, RetrievalQAWithSourcesChain
+from langchain.chains import RetrievalQAWithSourcesChain
 from langchain import OpenAI
 from neuralpit.context import Context
-from neuralpit.utils.loader import BinaryLoader
-from neuralpit.utils.indexer import DocumentIndexer
-from langchain.prompts import PromptTemplate
-from langchain.agents import AgentType, Tool, initialize_agent, AgentExecutor, BaseSingleActionAgent
-
+from langchain.agents import Tool, AgentExecutor, BaseSingleActionAgent
+from langchain.embeddings.openai import OpenAIEmbeddings
+from langchain.vectorstores.faiss import FAISS
 from typing import List, Tuple, Any, Union
 from langchain.schema import AgentAction, AgentFinish
 
 class ChatAgent(BaseSingleActionAgent):
     """Chat Custom Agent."""
     
     @property
@@ -47,17 +45,18 @@
         """
         return AgentAction(tool="QA", tool_input=kwargs["input"], log="")
     
 class ChatAgentBuilder():
 
     @staticmethod
     def fromLoader(loader):
-        indexer = DocumentIndexer(loader)
-        index = indexer.getIndex()
         context = Context.instance()
+        embeddings = OpenAIEmbeddings(openai_api_key=context.getOpenAIKey())
+        docs = loader.list()
+        index = FAISS.from_documents(docs, embeddings)
         llm = OpenAI(openai_api_key=context.getOpenAIKey())
         qqa_chain = RetrievalQAWithSourcesChain.from_chain_type(
                 llm=llm,
                 chain_type = "map_reduce",
                 retriever=index.as_retriever(),
             )
         tools = [
```

### Comparing `neuralpit-1.0.7/src/neuralpit/utils/loader.py` & `neuralpit-1.0.8/src/neuralpit/utils/loader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List
 from langchain.docstore.document import Document
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 from neuralpit.services.converterFactory import ConverterFactory
 from neuralpit.context import Context
 
-def textToDocs(text: str) -> List[Document]:
+def textToDocs(text: str, file_index: int) -> List[Document]:
     """Converts a string or list of strings to a list of Documents with metadata."""
     if isinstance(text, str):
         # Take a single string as one page
         text = [text]
     page_docs = [Document(page_content=page) for page in text]
 
     # Add page numbers as metadata
@@ -23,35 +23,32 @@
             chunk_size=2000,
             separators=["\n\n", "\n", ".", "!", "?", ",", " ", ""],
             chunk_overlap=0,
         )
         chunks = text_splitter.split_text(doc.page_content)
         for i, chunk in enumerate(chunks):
             doc = Document(
-                page_content=chunk, metadata={"page": doc.metadata["page"], "chunk": i}
+                page_content=chunk, metadata={"fileIndex":file_index, "page": doc.metadata["page"], "chunk": i}
             )
             # Add sources a metadata
-            doc.metadata["source"] = f"{doc.metadata['page']}-{doc.metadata['chunk']}"
+            doc.metadata["source"] = f"{doc.metadata['fileIndex']}-{doc.metadata['page']}-{doc.metadata['chunk']}"
             doc_chunks.append(doc)
     return doc_chunks
 
 
-class BinaryLoader():
+class MemFileLoader():
 
     def __init__(self, binary):
-        self.binary = binary
-    
-    def loadSingleFileFromDisck(self, binary):
-        if not self._converter:
-            context = Context.instance()
-            self._converter = ConverterFactory.buildConverter(context.getConverterInfo())
-        pages = self._converter.convertFileToString(binary)
-        self._docs =  self.textToDocs(pages)
+        self._binary = binary
+
     
     def list(self)->List[Document]:
         context = Context.instance()
         converter = ConverterFactory.buildConverter(context.getConverterInfo())
-        pages = converter.convertFileToString(self.binary)
-        return textToDocs(pages)
+        files = [converter.getFilePages(self._binary)]
+        docs = []
+        for idx, pages in enumerate(files):
+            docs.extend(textToDocs(pages, idx ))
+        return docs
```

### Comparing `neuralpit-1.0.7/src/neuralpit.egg-info/PKG-INFO` & `neuralpit-1.0.8/src/neuralpit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralpit
-Version: 1.0.7
+Version: 1.0.8
 Summary: NeuralPit SDK
 Author-email: Quang Nguyen <quang.nguyen@neuralpit.com>
 Keywords: api,neural,neuralpit
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `neuralpit-1.0.7/src/neuralpit.egg-info/SOURCES.txt` & `neuralpit-1.0.8/src/neuralpit.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -10,12 +10,11 @@
 src/neuralpit.egg-info/top_level.txt
 src/neuralpit/services/__init__.py
 src/neuralpit/services/api.py
 src/neuralpit/services/converter.py
 src/neuralpit/services/converterFactory.py
 src/neuralpit/tools/__init__.py
 src/neuralpit/tools/chat.py
-src/neuralpit/utils/indexer.py
 src/neuralpit/utils/loader.py
 test/testDocChat.py
 test/testGetServiceProfile.py
 test/testGetUserProfile.py
```

### Comparing `neuralpit-1.0.7/test/testGetServiceProfile.py` & `neuralpit-1.0.8/test/testGetServiceProfile.py`

 * *Files identical despite different names*

