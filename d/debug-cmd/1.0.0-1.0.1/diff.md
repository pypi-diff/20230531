# Comparing `tmp/debug_cmd-1.0.0-py3-none-any.whl.zip` & `tmp/debug_cmd-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4744 bytes, number of entries: 8
+Zip file size: 5801 bytes, number of entries: 8
 -rw-r--r--  2.0 unx        0 b- defN 23-May-31 11:25 debug_cmd/__init__.py
--rw-r--r--  2.0 unx     5030 b- defN 23-May-31 12:06 debug_cmd/debug_cmd.py
--rw-r--r--  2.0 unx     1071 b- defN 23-May-31 12:17 debug_cmd-1.0.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      762 b- defN 23-May-31 12:17 debug_cmd-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-31 12:17 debug_cmd-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       55 b- defN 23-May-31 12:17 debug_cmd-1.0.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 23-May-31 12:17 debug_cmd-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      646 b- defN 23-May-31 12:17 debug_cmd-1.0.0.dist-info/RECORD
-8 files, 7666 bytes uncompressed, 3606 bytes compressed:  53.0%
+-rw-r--r--  2.0 unx     8346 b- defN 23-May-31 14:37 debug_cmd/debug_cmd.py
+-rw-r--r--  2.0 unx     1071 b- defN 23-May-31 14:43 debug_cmd-1.0.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      762 b- defN 23-May-31 14:43 debug_cmd-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-31 14:43 debug_cmd-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       55 b- defN 23-May-31 14:43 debug_cmd-1.0.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-May-31 14:43 debug_cmd-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      646 b- defN 23-May-31 14:43 debug_cmd-1.0.1.dist-info/RECORD
+8 files, 10982 bytes uncompressed, 4663 bytes compressed:  57.5%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: debug_cmd/__init__.py
 Comment: 
 
 Filename: debug_cmd/debug_cmd.py
 Comment: 
 
-Filename: debug_cmd-1.0.0.dist-info/LICENSE
+Filename: debug_cmd-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: debug_cmd-1.0.0.dist-info/METADATA
+Filename: debug_cmd-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: debug_cmd-1.0.0.dist-info/WHEEL
+Filename: debug_cmd-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: debug_cmd-1.0.0.dist-info/entry_points.txt
+Filename: debug_cmd-1.0.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: debug_cmd-1.0.0.dist-info/top_level.txt
+Filename: debug_cmd-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: debug_cmd-1.0.0.dist-info/RECORD
+Filename: debug_cmd-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## debug_cmd/debug_cmd.py

```diff
@@ -11,37 +11,47 @@
 
 import os
 import sys
 import locale
 import argparse
 import platform
 import subprocess
-from typing import Union
-from typing import Generator
+from typing import Generator, Union
 
-import openai
+from langchain import PromptTemplate
+from langchain.chat_models import ChatOpenAI
+from langchain.chains.summarize import load_summarize_chain
+from langchain.docstore.document import Document
+from langchain.text_splitter import CharacterTextSplitter
 
 
 # CLI encoding.
 _CLI_ENCODING = locale.getpreferredencoding()
 
+# llm.
+# :see: https://platform.openai.com/docs/models/model-endpoint-compatibility
+_LLM: ChatOpenAI = ChatOpenAI(temperature=1, model_name="gpt-4", max_tokens=4096)
+# _LLM = ChatOpenAI(temperature=1, model_name="gpt-3.5-turbo", max_tokens=2048)
+
 
 def main() -> None:
     """
     Entry point.
     """
     _assert_environment_variables()
-    commands = _load_cli_args()
+    commands, force = _load_cli_args()
 
     return_code, cmd_out = _exec_command(commands)
 
-    if return_code == 0:
+    # successfully ends.
+    if return_code == 0 and not force:
         print('\n-------- コマンドは成功しました --------')
-        sys.exit(0)
+        return
 
+    # ask llm about error.
     print('\n-------- エラー原因を解析中 --------')
     cmd_str = ' '.join(commands) if type(commands) is list else commands
     answer = _ask_llm_about_error(cmd=cmd_str, error_message=cmd_out)
     print(answer)
 
 
 def _assert_environment_variables() -> None:
@@ -52,34 +62,38 @@
 
     for e in environments:
         if e not in os.environ:
             sys.stderr.write(f'Please set environment variable "{e}".')
             sys.exit(1)
 
 
-def _load_cli_args() -> Union[str, list[str]]:
+def _load_cli_args() -> tuple[Union[str, list[str]], bool]:
     """
     Parse CLI arguments.
 
-    :return: command line arguments.
+    :return: (<command line arguments>, <-f option>).
     """
     parser = argparse.ArgumentParser(
         prog='debug_cmd',
         description='Debug linux command error by using GPT/LLM.',
     )
 
     parser.add_argument('command', nargs='*', type=str, help='command and arguments separated by spaces. cannot use pipe(|), redirect(>), etc.')  # nopep8
     parser.add_argument('-c', type=str, help='shell string like "sh -c ..."')
+    parser.add_argument('-f', action=argparse.BooleanOptionalAction, help='even if the return code is successful(0), the process is executed forcefully.')  # nopep8
     args = parser.parse_args()
 
     if not args.command and not args.c:
         parser.print_help()
         sys.exit(1)
 
-    return args.c if args.c else [arg for arg in args.command if arg]
+    cmd = args.c if args.c else [arg for arg in args.command if arg]
+    force = args.f
+
+    return cmd, force
 
 
 def _exec_command(cmd: Union[str, list[str]]) -> (int, str):
     """
     :param cmd: command line arguments.
     :return: (return code, stdout+stderr)
     """
@@ -113,37 +127,126 @@
             break
 
         yield line.decode(_CLI_ENCODING)
 
 
 def _ask_llm_about_error(cmd: str, error_message: str) -> str:
     """
-    Entry point.
+    :param str cmd: command line arguments.
+    :param str error_message: error message.
+    :return: an answer.
+    """
+    # split error message.
+    docs = _split_error_message(error_message)
+
+    # create a prompt.
+    query_text = _get_question(cmd)
+
+    # using refine.
+    question_prompt = _get_prompt_template(query_text)
+    refine_prompt = _get_refine_template(query_text)
+    chain = load_summarize_chain(_LLM, chain_type="refine", question_prompt=question_prompt, refine_prompt=refine_prompt)  # nopep8
+
+    return chain.run(docs)
+
 
+def _split_error_message(error_message: str) -> list[Document]:
+    """
+    Split error message for LangChain Refine.
+
+    :param str error_message: error message.
+    :return: a list of LangChain documents.
+    """
+    text_splitter = CharacterTextSplitter(
+        separator='\n',
+        chunk_size=_LLM.max_tokens / 1,
+        chunk_overlap=_LLM.max_tokens / 10,
+        length_function=len,
+    )
+    texts = text_splitter.split_text(error_message)
+    documents = [Document(page_content=t) for t in texts]
+
+    return documents
+
+
+def _get_question(cmd: str) -> str:
+    """
     :param cmd: command line arguments.
-    :param error_message: command error message.
-    :return: answer.
+    :return: llm prompt.
     """
-    # create a chat completion
-    chat_completion = openai.ChatCompletion.create(
-        model='gpt-4',
-        messages=[
-            {'role': 'system', 'content': 'あなたは Mac, Unix, Linux のターミナル上で発生したコマンドのエラーの解消を手助けする AI アシスタントです'},
-            {'role': 'assistant', 'content': 'あなたの使っているパソコンの OS名, OSバージョン を教えて下さい'},
-            {'role': 'user', 'content': f'私のパソコンは {_get_os()} です'},
-            {'role': 'assistant', 'content': 'エラーが発生したコマンドを教えて下さい'},
-            {'role': 'user', 'content': cmd},
-            {'role': 'assistant', 'content': 'エラーが発生したコマンドのエラーメッセージを教えて下さい'},
-            {'role': 'user', 'content': error_message},
-            {'role': 'assistant', 'content': 'コマンドのエラーの原因が分かりました。以下にエラーの原因とその解決策を示します。追加の質問は受付しません'},
-        ]
+    return (
+        'あなたは Mac, Unix, Linux のターミナル上で発生したコマンドのエラーの解消を手助けする AI アシスタントです\n'
+        f'質問者が使っているパソコンの OS名, OSバージョン: {_get_os()}\n'
+        f'質問者のパソコンでエラーが発生したコマンド: {cmd}\n'
+        'これらの情報と与えられたエラーメッセージを元に、エラーの原因とその解決策を示して下さい: '
     )
 
-    # print the chat completion
-    return chat_completion.choices[0].message.content
+
+def _get_prompt_template(query_str: str) -> PromptTemplate:
+    """
+    Create new prompt template in japanese.
+
+    :param str query_str: query string.
+    :return: A prompt template.
+    :see: https://python.langchain.com/en/latest/modules/chains/index_examples/summarize.html#the-refine-chain
+    """
+    prompt_template = (
+        "We have provided context information (error message) below.\n"
+        "------------\n"
+        "{text}\n"
+        "------------\n"
+        "Given this information, please answer the following question in Japanese.\n"
+        "------------\n"
+        f"{_escape_for_prompt_template(query_str)}\n"
+        "------------\n"
+    )
+
+    return PromptTemplate(template=prompt_template, input_variables=["text"])
+
+
+def _get_refine_template(query_str: str) -> PromptTemplate:
+    """
+    Create new refine template in japanese.
+
+    :param str query_str: query string.
+    :return: A refine template.
+    :see: https://python.langchain.com/en/latest/modules/chains/index_examples/summarize.html#the-refine-chain
+    """
+    refine_template = (
+        "Your job is to produce a final answer.\n"
+        "We have provided an existing answer below up to a certain point.\n"
+        "------------\n"
+        "{existing_answer}\n"
+        "------------\n"
+        "We have also provided original question for existing answer below.\n"
+        "------------\n"
+        f"{_escape_for_prompt_template(query_str)}\n"
+        "------------\n"
+        "We have the opportunity to refine the existing answer"
+        "(only if needed) with some more context (error message) below.\n"
+        "------------\n"
+        "{text}\n"
+        "------------\n"
+        "Given the new context, refine the original answer in Japanese.\n"
+        "If the context isn't useful, return the original answer."
+    )
+
+    return PromptTemplate(
+        input_variables=["existing_answer", "text"],
+        template=refine_template,
+    )
+
+
+def _escape_for_prompt_template(text: str) -> str:
+    """
+    :param text:
+    :return:
+    :see: https://github.com/hwchase17/langchain/issues/1660#issuecomment-1469320129
+    """
+    return text.replace('{', '{{').replace('}', '}}')
 
 
 def _get_os() -> str:
     """
     :return: '{OS name} {OS version}'.
     """
     os_name = platform.system()
```

## Comparing `debug_cmd-1.0.0.dist-info/LICENSE` & `debug_cmd-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `debug_cmd-1.0.0.dist-info/METADATA` & `debug_cmd-1.0.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debug-cmd
-Version: 1.0.0
+Version: 1.0.1
 Summary: Debug linux command error by using GPT/LLM.
 Home-page: https://github.com/megmogmog1965/debug_cmd
 Author: Yusuke Kawatsu
 Author-email: mail@sample.com
 License: MIT
 Keywords: gpt debug
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `debug_cmd-1.0.0.dist-info/RECORD` & `debug_cmd-1.0.1.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 debug_cmd/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-debug_cmd/debug_cmd.py,sha256=GeBpQPAoqO5UqwEFf5wwSEHZHHZaqPtQUlmSiYzdCUw,5030
-debug_cmd-1.0.0.dist-info/LICENSE,sha256=u8EpYn6Vw79WHlICc-rMtlgUrA-0AcSlcF94AJD0FB0,1071
-debug_cmd-1.0.0.dist-info/METADATA,sha256=3x7HdVSryJDI6GH6Y8ssaDn5GRzEyW2HSq7_QvrGK78,762
-debug_cmd-1.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-debug_cmd-1.0.0.dist-info/entry_points.txt,sha256=OpigP5xJALw-yWnPmoncGyEYycqqPHPbTynH5GEWcvs,55
-debug_cmd-1.0.0.dist-info/top_level.txt,sha256=8XGxPpLiDBklKXrkfYGxBz7GGXCtB7NT_VfjI2SJBoI,10
-debug_cmd-1.0.0.dist-info/RECORD,,
+debug_cmd/debug_cmd.py,sha256=GnL9lCrZqX7zn980CNqF6o4YEYGhy-8-11nJ5Fzr9XA,8346
+debug_cmd-1.0.1.dist-info/LICENSE,sha256=u8EpYn6Vw79WHlICc-rMtlgUrA-0AcSlcF94AJD0FB0,1071
+debug_cmd-1.0.1.dist-info/METADATA,sha256=3UuAh65m7IRUpPCeWW6kPBJG3ZbYf8-jCz-8ZRGHCh4,762
+debug_cmd-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+debug_cmd-1.0.1.dist-info/entry_points.txt,sha256=OpigP5xJALw-yWnPmoncGyEYycqqPHPbTynH5GEWcvs,55
+debug_cmd-1.0.1.dist-info/top_level.txt,sha256=8XGxPpLiDBklKXrkfYGxBz7GGXCtB7NT_VfjI2SJBoI,10
+debug_cmd-1.0.1.dist-info/RECORD,,
```

