# Comparing `tmp/langchain_utils-0.4.2.tar.gz` & `tmp/langchain_utils-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_utils-0.4.2.tar", max compression
+gzip compressed data, was "langchain_utils-0.4.3.tar", max compression
```

## Comparing `langchain_utils-0.4.2.tar` & `langchain_utils-0.4.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    13101 2023-05-29 13:16:54.761092 langchain_utils-0.4.2/README.md
--rw-r--r--   0        0        0       22 2023-05-29 13:20:37.127656 langchain_utils-0.4.2/langchain_utils/__init__.py
--rw-r--r--   0        0        0     2163 2023-05-29 09:12:58.926326 langchain_utils-0.4.2/langchain_utils/config.py
--rw-r--r--   0        0        0     4476 2023-05-29 09:15:45.189121 langchain_utils-0.4.2/langchain_utils/document_loaders.py
--rwxr-xr-x   0        0        0     3130 2023-04-17 03:23:31.837819 langchain_utils-0.4.2/langchain_utils/get_html_prompt.py
--rwxr-xr-x   0        0        0     4938 2023-05-29 13:20:07.175620 langchain_utils-0.4.2/langchain_utils/get_pdf_prompt.py
--rwxr-xr-x   0        0        0     3721 2023-04-17 03:23:31.791685 langchain_utils-0.4.2/langchain_utils/get_text_prompt.py
--rwxr-xr-x   0        0        0     4101 2023-05-03 03:00:37.545180 langchain_utils-0.4.2/langchain_utils/get_url_prompt.py
--rwxr-xr-x   0        0        0     3476 2023-04-17 03:23:31.837872 langchain_utils-0.4.2/langchain_utils/get_word_prompt.py
--rwxr-xr-x   0        0        0     2874 2023-05-23 10:30:00.649134 langchain_utils-0.4.2/langchain_utils/get_youtube_transcript_prompt.py
--rw-r--r--   0        0        0     3505 2023-05-29 09:16:10.506138 langchain_utils-0.4.2/langchain_utils/loaders.py
--rw-r--r--   0        0        0      509 2023-04-16 15:20:17.709721 langchain_utils-0.4.2/langchain_utils/prompts.py
--rw-r--r--   0        0        0    10484 2023-05-03 02:59:26.472452 langchain_utils-0.4.2/langchain_utils/utils.py
--rw-r--r--   0        0        0     2154 2023-04-16 15:19:45.633897 langchain_utils-0.4.2/langchain_utils/utils_argparse.py
--rw-r--r--   0        0        0     3314 2023-05-29 08:59:46.652209 langchain_utils-0.4.2/langchain_utils/utils_doc_loaders.py
--rw-r--r--   0        0        0     1933 2023-05-29 13:20:37.126888 langchain_utils-0.4.2/pyproject.toml
--rw-r--r--   0        0        0    14219 1970-01-01 00:00:00.000000 langchain_utils-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0    13101 2023-05-29 13:16:54.761092 langchain_utils-0.4.3/README.md
+-rw-r--r--   0        0        0       22 2023-05-31 04:20:17.538384 langchain_utils-0.4.3/langchain_utils/__init__.py
+-rw-r--r--   0        0        0     2163 2023-05-29 09:12:58.926326 langchain_utils-0.4.3/langchain_utils/config.py
+-rw-r--r--   0        0        0     4523 2023-05-31 04:07:36.378255 langchain_utils-0.4.3/langchain_utils/document_loaders.py
+-rwxr-xr-x   0        0        0     2959 2023-05-31 04:06:21.103056 langchain_utils-0.4.3/langchain_utils/get_html_prompt.py
+-rwxr-xr-x   0        0        0     4928 2023-05-31 04:18:55.050216 langchain_utils-0.4.3/langchain_utils/get_pdf_prompt.py
+-rwxr-xr-x   0        0        0     3550 2023-05-31 04:11:22.760517 langchain_utils-0.4.3/langchain_utils/get_text_prompt.py
+-rwxr-xr-x   0        0        0     3971 2023-05-31 04:11:27.982204 langchain_utils-0.4.3/langchain_utils/get_url_prompt.py
+-rwxr-xr-x   0        0        0     3476 2023-04-17 03:23:31.837872 langchain_utils-0.4.3/langchain_utils/get_word_prompt.py
+-rwxr-xr-x   0        0        0     2874 2023-05-23 10:30:00.649134 langchain_utils-0.4.3/langchain_utils/get_youtube_transcript_prompt.py
+-rw-r--r--   0        0        0     3505 2023-05-29 09:16:10.506138 langchain_utils-0.4.3/langchain_utils/loaders.py
+-rw-r--r--   0        0        0      509 2023-04-16 15:20:17.709721 langchain_utils-0.4.3/langchain_utils/prompts.py
+-rw-r--r--   0        0        0    10699 2023-05-31 04:09:39.160287 langchain_utils-0.4.3/langchain_utils/utils.py
+-rw-r--r--   0        0        0     2154 2023-04-16 15:19:45.633897 langchain_utils-0.4.3/langchain_utils/utils_argparse.py
+-rw-r--r--   0        0        0     3310 2023-05-31 04:08:37.439910 langchain_utils-0.4.3/langchain_utils/utils_doc_loaders.py
+-rw-r--r--   0        0        0     1933 2023-05-31 04:20:17.535688 langchain_utils-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0    14219 1970-01-01 00:00:00.000000 langchain_utils-0.4.3/PKG-INFO
```

### Comparing `langchain_utils-0.4.2/README.md` & `langchain_utils-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.4.2/langchain_utils/config.py` & `langchain_utils-0.4.3/langchain_utils/config.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.4.2/langchain_utils/document_loaders.py` & `langchain_utils-0.4.3/langchain_utils/document_loaders.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,16 @@
                         flags=0, dpi=300, full=True, language=ocr_language
                     )
                 ).encode("utf-8"),
                 metadata=dict(
                     {
                         "source": file_path,
                         "file_path": file_path,
-                        "page_number": page.number + 1,
+                        # "page_number": page.number + 1,
+                        "page": page.number,
                         "total_pages": len(doc),
                     },
                     **{
                         k: doc.metadata[k]
                         for k in doc.metadata
                         if type(doc.metadata[k]) in [str, int]
                     }
```

### Comparing `langchain_utils-0.4.2/langchain_utils/get_html_prompt.py` & `langchain_utils-0.4.3/langchain_utils/get_html_prompt.py`

 * *Files 7% similar despite different names*

```diff
@@ -77,18 +77,14 @@
         file=sys.stderr,
     )
     if args.merge:
         from langchain.docstore.document import Document
 
         merged = Document(
             page_content=all_text,
-            # metadata=docs[0].metadata,
-            # metadata={
-            #     k: v for k, v in docs[0].metadata.items() if k not in {'page_number'}
-            # },
         )
     documents = [merged] if args.merge else docs  # type: ignore
     num_docs = len(documents)
     if args.no_split:
         needs_splitting = False
     elif word_count > args.chunk_size * 0.75:
         needs_splitting = True
```

### Comparing `langchain_utils-0.4.2/langchain_utils/get_pdf_prompt.py` & `langchain_utils-0.4.3/langchain_utils/get_pdf_prompt.py`

 * *Files 5% similar despite different names*

```diff
@@ -97,24 +97,24 @@
     if args.pages and args.page_slice:
         print(
             'Please specify either --pages or --page-slice, not both',
             file=sys.stderr,
         )
         sys.exit(1)
     if args.pages:
-        args.pages = [p for p in args.pages if p <= num_whole_pdf_pages and p > 0]
-        docs = [doc for doc in docs if doc.metadata['page_number'] in args.pages]
+        args.pages = [p - 1 for p in args.pages if p <= num_whole_pdf_pages and p > 0]
+        docs = [doc for doc in docs if doc.metadata['page'] in args.pages]
     if args.page_slice:
         args.pages = list(
-            x + 1
+            x - 1
             for x in list(range(num_whole_pdf_pages))[
                 convert_str_slice_notation_to_slice(args.page_slice)
             ]
         )
-        docs = [doc for doc in docs if doc.metadata['page_number'] in args.pages]
+        docs = [doc for doc in docs if doc.metadata['page'] in args.pages]
     texts = [doc.page_content for doc in docs]
     all_text = '\n'.join(texts)
     word_count = get_word_count((all_text))
     char_count = len(all_text)
     print(
         f'Loaded {len(docs)} pages. Word count: {word_count} Char count: {len(all_text)}',
         file=sys.stderr,
```

### Comparing `langchain_utils-0.4.2/langchain_utils/get_text_prompt.py` & `langchain_utils-0.4.3/langchain_utils/get_text_prompt.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,18 +90,14 @@
         print(f'Token / Char: {token_count / char_count:.2f}', file=sys.stderr)
         return
     if args.merge:
         from langchain.docstore.document import Document
 
         merged = Document(
             page_content=all_text,
-            # metadata=docs[0].metadata,
-            # metadata={
-            #     k: v for k, v in docs[0].metadata.items() if k not in {'page_number'}
-            # },
         )
     documents = [merged] if args.merge else docs  # type: ignore
     num_docs = len(documents)
     if args.no_split:
         needs_splitting = False
     elif word_count > args.chunk_size * 0.75:
         needs_splitting = True
```

### Comparing `langchain_utils-0.4.2/langchain_utils/get_url_prompt.py` & `langchain_utils-0.4.3/langchain_utils/get_url_prompt.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,17 +103,14 @@
         print(f'Token / Char: {token_count / char_count:.2f}', file=sys.stderr)
         return
     if args.merge:
         from langchain.docstore.document import Document
 
         merged = Document(
             page_content=all_text,
-            # metadata={
-            #     k: v for k, v in docs[0].metadata.items() if k not in {'page_number'}
-            # },
         )
     if args.no_split:
         needs_splitting = False
     elif word_count > args.chunk_size * 0.75:
         needs_splitting = True
     else:
         needs_splitting = False
```

### Comparing `langchain_utils-0.4.2/langchain_utils/get_word_prompt.py` & `langchain_utils-0.4.3/langchain_utils/get_word_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.4.2/langchain_utils/get_youtube_transcript_prompt.py` & `langchain_utils-0.4.3/langchain_utils/get_youtube_transcript_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.4.2/langchain_utils/loaders.py` & `langchain_utils-0.4.3/langchain_utils/loaders.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.4.2/langchain_utils/utils.py` & `langchain_utils-0.4.3/langchain_utils/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,16 +66,19 @@
 
 def format_date(dt: 'datetime') -> str:
     return dt.strftime('%Y-%m-%d')
 
 
 def pymupdf_doc_page_info(document: 'Document') -> str:
     metadata = document.metadata
-    if 'page_number' in metadata:
+    total_pages_in_metadata = 'total_pages' in metadata
+    if 'page_number' in metadata and total_pages_in_metadata:
         return f', Page {metadata["page_number"]}/{metadata["total_pages"]}'
+    elif 'page' in metadata and total_pages_in_metadata:
+        return f', Page {metadata["page"] + 1}/{metadata["total_pages"]}'
     else:
         return ''
 
 
 def html_source_info(document: 'Document') -> str:
     metadata = document.metadata
     if 'source' in metadata:
```

### Comparing `langchain_utils-0.4.2/langchain_utils/utils_argparse.py` & `langchain_utils-0.4.3/langchain_utils/utils_argparse.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.4.2/langchain_utils/utils_doc_loaders.py` & `langchain_utils-0.4.3/langchain_utils/utils_doc_loaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
             data = f.read(65536)
             if not data:
                 break
             sha1.update(data)
     return sha1.hexdigest()
 
 
-
 def get_str_punc_and_whitespace_chars_pct(text):
     # write a python function to count the % of chars in a str that is 1) punctuation, or 2) \t, \n
     import string
 
     punc_and_whitespace_chars = string.punctuation + "\t\n"
     count = sum(1 for c in text if c in punc_and_whitespace_chars)
     return count / len(text)
@@ -60,12 +59,12 @@
     # source_id = item.get("source_id", None)
     # url = item.get("url", None)
     # created_at = item.get("created_at", None)
     # author = item.get("author", None)
     return {
         "text": doc.page_content,
         "source": doc.metadata['source']
-        + f'page {doc.metadata["page_number"]}/{doc.metadata["total_pages"]}',
+        + f'page {doc.metadata["page"] + 1}/{doc.metadata["total_pages"]}',
         "author": doc.metadata['author'],
         "created_at": doc.metadata['creationDate'],
         "url": f'file://{doc.metadata["file_path"]}',
     }
```

### Comparing `langchain_utils-0.4.2/pyproject.toml` & `langchain_utils-0.4.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-utils"
-version = "0.4.2"
+version = "0.4.3"
 description = "Utilities built upon the langchain library"
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "langchain_utils" }]
 license = "MIT"
 homepage = "https://github.com/tddschn/langchain-utils"
 repository = "https://github.com/tddschn/langchain-utils"
```

### Comparing `langchain_utils-0.4.2/PKG-INFO` & `langchain_utils-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-utils
-Version: 0.4.2
+Version: 0.4.3
 Summary: Utilities built upon the langchain library
 Home-page: https://github.com/tddschn/langchain-utils
 License: MIT
 Keywords: langchain,utils,LLM,prompts,CLI
 Author: Teddy Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
```

