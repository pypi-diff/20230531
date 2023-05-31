# Comparing `tmp/paper-qa-2.0.1.tar.gz` & `tmp/paper-qa-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper-qa-2.0.1.tar", last modified: Tue May 30 16:09:14 2023, max compression
+gzip compressed data, was "paper-qa-2.0.2.tar", last modified: Wed May 31 21:22:30 2023, max compression
```

## Comparing `paper-qa-2.0.1.tar` & `paper-qa-2.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:09:14.917566 paper-qa-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-30 16:08:31.000000 paper-qa-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13282 2023-05-30 16:09:14.917566 paper-qa-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12847 2023-05-30 16:08:31.000000 paper-qa-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:09:14.917566 paper-qa-2.0.1/paper_qa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13282 2023-05-30 16:09:14.000000 paper-qa-2.0.1/paper_qa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-30 16:09:14.000000 paper-qa-2.0.1/paper_qa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 16:09:14.000000 paper-qa-2.0.1/paper_qa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-30 16:09:14.000000 paper-qa-2.0.1/paper_qa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-30 16:09:14.000000 paper-qa-2.0.1/paper_qa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:09:14.917566 paper-qa-2.0.1/paperqa/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-30 16:08:31.000000 paper-qa-2.0.1/paperqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-05-30 16:08:31.000000 paper-qa-2.0.1/paperqa/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:09:14.917566 paper-qa-2.0.1/paperqa/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-30 16:08:31.000000 paper-qa-2.0.1/paperqa/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-05-30 16:08:31.000000 paper-qa-2.0.1/paperqa/contrib/zotero.py
--rw-r--r--   0 runner    (1001) docker     (123)    22396 2023-05-30 16:08:31.000000 paper-qa-2.0.1/paperqa/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-30 16:08:31.000000 paper-qa-2.0.1/paperqa/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-05-30 16:08:31.000000 paper-qa-2.0.1/paperqa/qaprompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-05-30 16:08:31.000000 paper-qa-2.0.1/paperqa/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-30 16:08:31.000000 paper-qa-2.0.1/paperqa/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-30 16:08:31.000000 paper-qa-2.0.1/paperqa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 16:08:31.000000 paper-qa-2.0.1/paperqa/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 16:09:14.917566 paper-qa-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-30 16:08:31.000000 paper-qa-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:09:14.917566 paper-qa-2.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    15562 2023-05-30 16:08:31.000000 paper-qa-2.0.1/tests/test_paperqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:22:30.689701 paper-qa-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-31 21:21:47.000000 paper-qa-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13282 2023-05-31 21:22:30.689701 paper-qa-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12847 2023-05-31 21:21:47.000000 paper-qa-2.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:22:30.689701 paper-qa-2.0.2/paper_qa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13282 2023-05-31 21:22:30.000000 paper-qa-2.0.2/paper_qa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-31 21:22:30.000000 paper-qa-2.0.2/paper_qa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 21:22:30.000000 paper-qa-2.0.2/paper_qa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-31 21:22:30.000000 paper-qa-2.0.2/paper_qa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 21:22:30.000000 paper-qa-2.0.2/paper_qa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:22:30.689701 paper-qa-2.0.2/paperqa/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-31 21:21:47.000000 paper-qa-2.0.2/paperqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-05-31 21:21:47.000000 paper-qa-2.0.2/paperqa/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:22:30.689701 paper-qa-2.0.2/paperqa/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-31 21:21:47.000000 paper-qa-2.0.2/paperqa/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-05-31 21:21:47.000000 paper-qa-2.0.2/paperqa/contrib/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22301 2023-05-31 21:21:47.000000 paper-qa-2.0.2/paperqa/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-31 21:21:47.000000 paper-qa-2.0.2/paperqa/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-05-31 21:21:47.000000 paper-qa-2.0.2/paperqa/qaprompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-05-31 21:21:47.000000 paper-qa-2.0.2/paperqa/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-31 21:21:47.000000 paper-qa-2.0.2/paperqa/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-31 21:21:47.000000 paper-qa-2.0.2/paperqa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 21:21:47.000000 paper-qa-2.0.2/paperqa/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 21:22:30.689701 paper-qa-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-31 21:21:47.000000 paper-qa-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:22:30.689701 paper-qa-2.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    15587 2023-05-31 21:21:47.000000 paper-qa-2.0.2/tests/test_paperqa.py
```

### Comparing `paper-qa-2.0.1/LICENSE` & `paper-qa-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `paper-qa-2.0.1/PKG-INFO` & `paper-qa-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 2.0.1
+Version: 2.0.2
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-2.0.1/README.md` & `paper-qa-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `paper-qa-2.0.1/paper_qa.egg-info/PKG-INFO` & `paper-qa-2.0.2/paper_qa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 2.0.1
+Version: 2.0.2
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-2.0.1/paperqa/agent.py` & `paper-qa-2.0.2/paperqa/agent.py`

 * *Files identical despite different names*

### Comparing `paper-qa-2.0.1/paperqa/contrib/zotero.py` & `paper-qa-2.0.2/paperqa/contrib/zotero.py`

 * *Files identical despite different names*

### Comparing `paper-qa-2.0.1/paperqa/docs.py` & `paper-qa-2.0.2/paperqa/docs.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,21 +119,22 @@
         # first check to see if we already have this document
         # this way we don't make api call to create citation on file we already have
         hash = md5sum(path)
         if hash in [d["hash"] for d in self.docs]:
             raise ValueError(f"Document {path} already in collection.")
 
         if citation is None:
+            # skip system because it's too hesitant to answer
             cite_chain = make_chain(
-                prompt=citation_prompt, llm=self.summary_llm)
+                prompt=citation_prompt, llm=self.summary_llm, skip_system=True
+            )
             # peak first chunk
             texts, _ = read_doc(path, "", "", chunk_chars=chunk_chars)
             if len(texts) == 0:
-                raise ValueError(
-                    f"Could not read document {path}. Is it empty?")
+                raise ValueError(f"Could not read document {path}. Is it empty?")
             citation = cite_chain.run(texts[0])
             if len(citation) < 3 or "Unknown" in citation or "insufficient" in citation:
                 citation = f"Unknown, {os.path.basename(path)}, {datetime.now().year}"
 
         if key is None:
             # get first name and year from citation
             try:
@@ -145,16 +146,15 @@
                 )
             try:
                 year = re.search(r"(\d{4})", citation).group(1)
             except AttributeError:
                 year = ""
             key = f"{author}{year}"
         key = self.get_unique_key(key)
-        texts, metadata = read_doc(
-            path, citation, key, chunk_chars=chunk_chars)
+        texts, metadata = read_doc(path, citation, key, chunk_chars=chunk_chars)
         # loose check to see if document was loaded
         #
         if len("".join(texts)) < 10 or (
             not disable_check and not maybe_is_text("".join(texts))
         ):
             raise ValueError(
                 f"This does not look like a text document: {path}. Path disable_check to ignore this error."
@@ -228,36 +228,35 @@
     def doc_previews(self) -> List[Tuple[int, str, str]]:
         """Return a list of tuples of (key, citation) for each document."""
         return [
             (
                 len(doc["texts"]),
                 doc["metadata"][0]["dockey"],
                 doc["metadata"][0]["citation"],
+                doc["hash"],
             )
             for doc in self.docs
         ]
 
     async def adoc_match(
         self, query: str, k: int = 25, callbacks: List[AsyncCallbackHandler] = []
     ) -> List[str]:
         """Return a list of documents that match the query."""
         if len(self.docs) == 0:
             return ""
         if self._doc_index is None:
             texts = [doc["metadata"][0]["citation"] for doc in self.docs]
-            metadatas = [{"key": doc["metadata"][0]["dockey"]}
-                         for doc in self.docs]
+            metadatas = [{"key": doc["metadata"][0]["dockey"]} for doc in self.docs]
             self._doc_index = FAISS.from_texts(
                 texts, metadatas=metadatas, embedding=self.embeddings
             )
         docs = self._doc_index.max_marginal_relevance_search(
             query, k=k + len(self._deleted_keys)
         )
-        docs = [doc for doc in docs if doc.metadata["key"]
-                not in self._deleted_keys]
+        docs = [doc for doc in docs if doc.metadata["key"] not in self._deleted_keys]
         chain = make_chain(select_paper_prompt, self.summary_llm)
         papers = [f"{d.metadata['key']}: {d.page_content}" for d in docs]
         result = await chain.arun(
             question=query, papers="\n".join(papers), callbacks=callbacks
         )
         return result
 
@@ -265,24 +264,22 @@
         self, query: str, k: int = 25, callbacks: List[AsyncCallbackHandler] = []
     ) -> List[str]:
         """Return a list of documents that match the query."""
         if len(self.docs) == 0:
             return ""
         if self._doc_index is None:
             texts = [doc["metadata"][0]["citation"] for doc in self.docs]
-            metadatas = [{"key": doc["metadata"][0]["dockey"]}
-                         for doc in self.docs]
+            metadatas = [{"key": doc["metadata"][0]["dockey"]} for doc in self.docs]
             self._doc_index = FAISS.from_texts(
                 texts, metadatas=metadatas, embedding=self.embeddings
             )
         docs = self._doc_index.max_marginal_relevance_search(
             query, k=k + len(self._deleted_keys)
         )
-        docs = [doc for doc in docs if doc.metadata["key"]
-                not in self._deleted_keys]
+        docs = [doc for doc in docs if doc.metadata["key"] not in self._deleted_keys]
         chain = make_chain(select_paper_prompt, self.summary_llm)
         papers = [f"{d.metadata['key']}: {d.page_content}" for d in docs]
         result = chain.run(
             question=query, papers="\n".join(papers), callbacks=callbacks
         )
         return result
 
@@ -293,35 +290,32 @@
         del state["_faiss_index"]
         del state["_doc_index"]
         return state
 
     def __setstate__(self, state):
         self.__dict__.update(state)
         try:
-            self._faiss_index = FAISS.load_local(
-                self.index_path, self.embeddings)
+            self._faiss_index = FAISS.load_local(self.index_path, self.embeddings)
         except:
             # they use some special exception type, but I don't want to import it
             self._faiss_index = None
         if not hasattr(self, "_doc_index"):
             self._doc_index = None
         # must be a better way to have backwards compatibility
         if not hasattr(self, "_deleted_keys"):
             self._deleted_keys = set()
         if not hasattr(self, "max_concurrent"):
             self.max_concurrent = 5
         self.update_llm(None, None)
 
     def _build_faiss_index(self):
         if self._faiss_index is None:
-            texts = reduce(lambda x, y: x + y,
-                           [doc["texts"] for doc in self.docs], [])
+            texts = reduce(lambda x, y: x + y, [doc["texts"] for doc in self.docs], [])
             text_embeddings = reduce(
-                lambda x, y: x + y, [doc["text_embeddings"]
-                                     for doc in self.docs], []
+                lambda x, y: x + y, [doc["text_embeddings"] for doc in self.docs], []
             )
             metadatas = reduce(
                 lambda x, y: x + y, [doc["metadata"] for doc in self.docs], []
             )
             self._faiss_index = FAISS.from_embeddings(
                 # wow adding list to the zip was tricky
                 text_embeddings=list(zip(texts, text_embeddings)),
@@ -382,16 +376,15 @@
             )
         else:
             docs = self._faiss_index.similarity_search(
                 answer.question, k=_k, fetch_k=5 * _k
             )
         # ok now filter
         if key_filter is not None:
-            docs = [doc for doc in docs if doc.metadata["dockey"]
-                    in key_filter][:k]
+            docs = [doc for doc in docs if doc.metadata["dockey"] in key_filter][:k]
 
         async def process(doc):
             if doc.metadata["dockey"] in self._deleted_keys:
                 return None, None
             # check if it is already in answer (possible in agent setting)
             if doc.metadata["key"] in [c.key for c in answer.contexts]:
                 return None, None
```

### Comparing `paper-qa-2.0.1/paperqa/qaprompts.py` & `paper-qa-2.0.2/paperqa/qaprompts.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 def _get_datetime():
     now = datetime.now()
     return now.strftime("%m/%d/%Y")
 
 
 citation_prompt = prompts.PromptTemplate(
     input_variables=["text"],
-    template="Provide a citation for the following text in MLA Format. You must answer. Today's date is {date}\n"
+    template="Provide the citation for the following text in MLA Format. Today's date is {date}\n"
     "{text}\n\n"
     "Citation:",
     partial_variables={"date": _get_datetime},
 )
 
 
 class FallbackLLMChain(LLMChain):
@@ -91,25 +91,28 @@
         """Generate LLM result from inputs."""
         try:
             return await super().agenerate(input_list, run_manager=run_manager)
         except NotImplementedError as e:
             return self.generate(input_list, run_manager=run_manager)
 
 
-def make_chain(prompt, llm):
+def make_chain(prompt, llm, skip_system=False):
     if type(llm) == ChatOpenAI:
         system_message_prompt = SystemMessage(
             content="Answer in an unbiased, concise, scholarly tone. "
             "You may refuse to answer if there is insufficient information. "
             "If there are ambiguous terms or acronyms, first define them. ",
         )
         human_message_prompt = HumanMessagePromptTemplate(prompt=prompt)
-        prompt = ChatPromptTemplate.from_messages(
-            [system_message_prompt, human_message_prompt]
-        )
+        if skip_system:
+            prompt = ChatPromptTemplate.from_messages([human_message_prompt])
+        else:
+            prompt = ChatPromptTemplate.from_messages(
+                [system_message_prompt, human_message_prompt]
+            )
     return FallbackLLMChain(prompt=prompt, llm=llm)
 
 
 def get_score(text):
     score = re.search(r"[sS]core[:is\s]+([0-9]+)", text)
     if score:
         return int(score.group(1))
```

### Comparing `paper-qa-2.0.1/paperqa/readers.py` & `paper-qa-2.0.2/paperqa/readers.py`

 * *Files identical despite different names*

### Comparing `paper-qa-2.0.1/paperqa/types.py` & `paper-qa-2.0.2/paperqa/types.py`

 * *Files identical despite different names*

### Comparing `paper-qa-2.0.1/paperqa/utils.py` & `paper-qa-2.0.2/paperqa/utils.py`

 * *Files identical despite different names*

### Comparing `paper-qa-2.0.1/setup.py` & `paper-qa-2.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `paper-qa-2.0.1/tests/test_paperqa.py` & `paper-qa-2.0.2/tests/test_paperqa.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,46 +137,44 @@
 
 def test_docs_pickle():
     doc_path = "example.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get front page of wikipedia
         r = requests.get("https://en.wikipedia.org/wiki/National_Flag_of_Canada_Day")
         f.write(r.text)
-    llm = OpenAI(temperature=0.0, model_name="text-babbage-001")
+    llm = OpenAI(temperature=0.0, model_name="text-curie-001")
     docs = paperqa.Docs(llm=llm)
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now", chunk_chars=1000)
     docs_pickle = pickle.dumps(docs)
     docs2 = pickle.loads(docs_pickle)
     docs2.update_llm(llm)
     assert len(docs.docs) == len(docs2.docs)
-    assert (
-        strings_similarity(
-            docs.get_evidence(
-                paperqa.Answer("What date is flag day in Canada?"),
-                k=3,
-                max_sources=1,
-            ).context,
-            docs2.get_evidence(
-                paperqa.Answer("What date is flag day in Canada?"),
-                k=3,
-                max_sources=1,
-            ).context,
-        )
-        > 0.75
+    context1, context2 = (
+        docs.get_evidence(
+            paperqa.Answer("What date is flag day in Canada?"),
+            k=3,
+            max_sources=1,
+        ).context,
+        docs2.get_evidence(
+            paperqa.Answer("What date is flag day in Canada?"),
+            k=3,
+            max_sources=1,
+        ).context,
     )
+    assert strings_similarity(context1, context2) > 0.75
     os.remove(doc_path)
 
 
 def test_docs_pickle_no_faiss():
     doc_path = "example.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get front page of wikipedia
         r = requests.get("https://en.wikipedia.org/wiki/National_Flag_of_Canada_Day")
         f.write(r.text)
-    llm = OpenAI(temperature=0.0, model_name="text-babbage-001")
+    llm = OpenAI(temperature=0.0, model_name="text-curie-001")
     docs = paperqa.Docs(llm=llm)
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now", chunk_chars=1000)
     docs._faiss_index = None
     docs_pickle = pickle.dumps(docs)
     docs2 = pickle.loads(docs_pickle)
     docs2.update_llm(llm)
     assert len(docs.docs) == len(docs2.docs)
@@ -302,14 +300,15 @@
     doc_path = "example.txt"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get wiki page about politician
         r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
         f.write(r.text)
     docs = paperqa.Docs()
     docs.add(doc_path)
+    print(docs.docs[0]["metadata"][0]["citation"])
     assert (
         list(docs.docs)[0]["metadata"][0]["key"] == "Wikipedia2023"
         or list(docs.docs)[0]["metadata"][0]["key"] == "Frederick2023"
     )
 
 
 def test_dockey_filter():
```

