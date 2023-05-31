# Comparing `tmp/doFolder-0.0.5.tar.gz` & `tmp/doFolder-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doFolder-0.0.5.tar", last modified: Tue May 30 18:05:58 2023, max compression
+gzip compressed data, was "doFolder-0.0.6.tar", last modified: Wed May 31 15:06:30 2023, max compression
```

## Comparing `doFolder-0.0.5.tar` & `doFolder-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 18:05:58.527872 doFolder-0.0.5/
--rw-rw-rw-   0        0        0     3349 2023-05-30 18:05:58.527872 doFolder-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2624 2023-05-30 18:05:13.000000 doFolder-0.0.5/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-30 18:05:58.516871 doFolder-0.0.5/doFolder/
--rw-rw-rw-   0        0        0      569 2023-05-26 13:44:53.000000 doFolder-0.0.5/doFolder/__init__.py
--rw-rw-rw-   0        0        0    10825 2023-05-28 09:01:39.000000 doFolder-0.0.5/doFolder/compare.py
--rw-rw-rw-   0        0        0    19828 2023-05-30 17:53:26.000000 doFolder-0.0.5/doFolder/main.py
--rw-rw-rw-   0        0        0    13825 2023-05-28 09:04:58.000000 doFolder-0.0.5/doFolder/terminal.py
-drwxrwxrwx   0        0        0        0 2023-05-30 18:05:58.525872 doFolder-0.0.5/doFolder.egg-info/
--rw-rw-rw-   0        0        0     3349 2023-05-30 18:05:58.000000 doFolder-0.0.5/doFolder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-05-30 18:05:58.000000 doFolder-0.0.5/doFolder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 18:05:58.000000 doFolder-0.0.5/doFolder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-30 18:05:58.000000 doFolder-0.0.5/doFolder.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-05-30 18:05:58.000000 doFolder-0.0.5/doFolder.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-30 18:05:58.000000 doFolder-0.0.5/doFolder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 18:05:58.528872 doFolder-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1196 2023-05-30 18:05:25.000000 doFolder-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 15:06:30.497152 doFolder-0.0.6/
+-rw-rw-rw-   0        0        0     3349 2023-05-31 15:06:30.497152 doFolder-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2624 2023-05-30 18:05:13.000000 doFolder-0.0.6/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-31 15:06:30.487153 doFolder-0.0.6/doFolder/
+-rw-rw-rw-   0        0        0      569 2023-05-31 14:24:09.000000 doFolder-0.0.6/doFolder/__init__.py
+-rw-rw-rw-   0        0        0    10823 2023-05-31 14:59:56.000000 doFolder-0.0.6/doFolder/compare.py
+-rw-rw-rw-   0        0        0    21399 2023-05-31 15:02:01.000000 doFolder-0.0.6/doFolder/main.py
+-rw-rw-rw-   0        0        0    13847 2023-05-31 14:13:25.000000 doFolder-0.0.6/doFolder/terminal.py
+drwxrwxrwx   0        0        0        0 2023-05-31 15:06:30.495152 doFolder-0.0.6/doFolder.egg-info/
+-rw-rw-rw-   0        0        0     3349 2023-05-31 15:06:30.000000 doFolder-0.0.6/doFolder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-05-31 15:06:30.000000 doFolder-0.0.6/doFolder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 15:06:30.000000 doFolder-0.0.6/doFolder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-31 15:06:30.000000 doFolder-0.0.6/doFolder.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-05-31 15:06:30.000000 doFolder-0.0.6/doFolder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-31 15:06:30.000000 doFolder-0.0.6/doFolder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 15:06:30.498154 doFolder-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1196 2023-05-31 14:57:13.000000 doFolder-0.0.6/setup.py
```

### Comparing `doFolder-0.0.5/PKG-INFO` & `doFolder-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doFolder
-Version: 0.0.5
+Version: 0.0.6
 Summary: download files quickly
 Home-page: https://kuankuan2007.gitee.io/docs/do-folder/
 Author: kuankuan
 Author-email: 2163826131@qq.com
 License: Mulan PSL v2
 Keywords: file,foler,path,filesystem
 Platform: windows
```

### Comparing `doFolder-0.0.5/README.rst` & `doFolder-0.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `doFolder-0.0.5/doFolder/__init__.py` & `doFolder-0.0.6/doFolder/__init__.py`

 * *Files identical despite different names*

### Comparing `doFolder-0.0.5/doFolder/compare.py` & `doFolder-0.0.6/doFolder/compare.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,15 +173,15 @@
             "size":lambda f1,f2:f1.size==f2.size,
             "content":lambda f1,f2:f1.content==f2.content,
         }
         if compareContent in ma:
             return ma[compareContent]
         raise ValueError(f"compareContent is not valid. If you want to customize the comparison method, please pass in a comparison function")
     raise ValueError(f"compareContent must be callable or str,but \"{compareContent}\" is given")
-def compare(folder1:doFolder.Folder,folder2:doFolder.Folder,compareContent:unformatedCompareContent="ignore",threaded:bool=False,threads:Union[None,int]=None)->CompareResult:
+def compare(folder1:doFolder.Folder,folder2:doFolder.Folder,compareContent:unformatedCompareContent="ignore",threaded:bool=False,threads:Union[None,int]=10)->CompareResult:
     threadPool=ThreadPoolExecutor(max_workers=threads) if threaded else None
     result=_compare(folder1,folder2,folder1,folder2,_normalizedCompareContent(compareContent),threadPool)
     assert result
     if threadPool:threadPool.shutdown(wait=True)
     return result
 def _compareFile(result:CompareResult,file1:doFolder.File,file2:doFolder.File,compareContent:formatedCompareContent,root1:doFolder.Folder
             ,root2:doFolder.Folder)->None:
```

### Comparing `doFolder-0.0.5/doFolder/main.py` & `doFolder-0.0.6/doFolder/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 THIS SOFTWARE IS PROVIDED ON AN "AS IS" BASIS, WITHOUT WARRANTIES OF ANY KIND,
 EITHER EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO NON-INFRINGEMENT,
 MERCHANTABILITY OR FIT FOR A PARTICULAR PURPOSE.
 See the Mulan PSL v2 for more details.
 """
 import os
 import re
-from typing import Any,Union,Callable,Literal,List,Tuple,Iterable,TypeVar,Generic,Protocol
+from typing import Any,Union,Callable,Literal,List,Tuple,Iterable,TypeVar,Generic,IO
 import shutil
 import copy
 from watchdog.observers import Observer
 from watchdog.events import FileSystemEventHandler,FileSystemEvent,FileSystemMovedEvent,EVENT_TYPE_CREATED,EVENT_TYPE_DELETED,EVENT_TYPE_MOVED,EVENT_TYPE_MODIFIED
 import hashlib
 import logging
 from concurrent.futures import ThreadPoolExecutor
@@ -52,14 +52,22 @@
     def __init__(self,reason):
         self.reason=reason
     def __str__(self) -> str:
         return str(self.reason)
     def __repr__(self) -> str:
         return str(self.reason)
 
+class FileOrFolderAlreadyExists(Exception):
+    def __init__(self,reason):
+        self.reason=reason
+    def __str__(self) -> str:
+        return str(self.reason)
+    def __repr__(self) -> str:
+        return str(self.reason)
+
 def _formatMatching(condition:UnformattedMatching)->FormatedMatching:
     limit=(1,1)
     if type(condition)==tuple and not callable(condition):
         limit=(condition[1],condition[2])
         condition= condition[0]
     if type(condition)==str and not callable(condition):
         match:Callable[[Union["File","Folder"]],bool]=lambda item:item.name==condition
@@ -155,15 +163,15 @@
         li=self.path.split("/")
         while "" in li:
             li.remove("")
         return li
     @property
     def name(self)->str:
         """The name of the path points to"""
-        return self.partition[-1]
+        return self.partition[-1] if len(self.partition) else self.driver+"/"
     def add(self, value:str):
         """add another dir name after the path"""
         if self[-1]!="/":
             return Path(self+"/"+value)
         return Path(self+value)
     def adds(self, value:List[str])->"Path":
         new=copy.deepcopy(self)
@@ -208,25 +216,29 @@
         self._md5:Union[None,str]=None
         self._sha1:Union[None,str]=None
         self._sha256:Union[None,str]=None
         self._sha512:Union[None,str]=None
     @property
     def name(self)->str:
         return self.path.name
-    def open(self,*args,**kw):
+    def open(self,*args,**kw)->IO:
         """open the file by function open"""
         return open(self.path,*args,**kw)
     def __str__(self)->str:
         return f"<File \"{self.name}\">"
     def __repr__(self) -> str:
         return f"<File \"{self.name}\">"
     @property
     def content(self)->bytes:
         with self.open("rb") as f:
             return f.read()
+    @content.setter
+    def _setContent(self,content:bytes):
+        with self.open("wb") as f:
+            f.write(content)
     @property
     def md5(self)->str:
         if self._md5:
             return self._md5
         self._md5=hashlib.md5(self.content).hexdigest()
         return self._md5
     @property
@@ -385,31 +397,39 @@
         shutil.rmtree(self.path)
     def move(self,path:str)->None:
         self.logger.info(f"Moving folder to {path}")
         shutil.move(self.path,path)
     def copy(self,path:str)->None:
         self.logger.info(f"Copying folder to {path}")
         shutil.copytree(self.path, path)
-    def hasSubfolder(self,name:str)->bool:
+    def hasSubfolder(self,name:str,recursive:bool=False)->bool:
         """
         Whether to include a subfolder
         :param name:folder name
         """
         for i in self.subfolder:
             if i.name==name:
                 return True
+        if recursive:
+            for i  in self.subfolder:
+                if i.hasSubfolder(name,recursive=recursive):
+                    return True
         return False
-    def hasFile(self,name:str)->bool:
+    def hasFile(self,name:str,recursive:bool=False)->bool:
         """
         Whether to include a file
         :param name:file name
         """
         for i in self.files:
             if i.name==name:
                 return True
+        if recursive:
+            for i  in self.subfolder:
+                if i.hasFile(name,recursive=recursive):
+                    return True
         return False
     def search(self,condition:List[UnformattedMatching],aim:Literal["file","folder","both"]="both",threaded:bool=False,threads:Union[None,int]=None)->SearchResult:
         """
         Search item in the Folder
         :param condition: search conditions which is unformatted
         str: match the files whose name == condition\n
         re.Pattern[str]: match the files whose name matches the regular expression\n
@@ -454,8 +474,26 @@
                 while k<len(restCondition):
                     if restCondition[k][1]!=0:
                         break
                     k+=1
                 if (k==len(restCondition)):
                     retsult.append(j)
             if condition[i][1]>0:
-                break
+                break
+    def createFile(self,path:Union[str,Path],content:bytes=b"")->Path:
+        path=Path(os.path.join(self.path, path))
+        if os.path.exists(path):
+            raise FileOrFolderAlreadyExists(f"Can't create file {path} because it already exists")
+        with open(path,"wb") as f:
+            f.write(content)
+        return path
+    def createFolder(self,path:Union[str,Path],content:bytes=b"")->Path:
+        path=Path(os.path.join(self.path, path))
+        if os.path.exists(path):
+            raise FileOrFolderAlreadyExists(f"Can't create folder {path} because it already exists")
+        os.makedirs(path)
+        return path
+    def add(self,aim:Union["File","Folder"],move:bool=False):
+        if move:
+            aim.move(self.path)
+        else:
+            aim.copy(self.path)
```

### Comparing `doFolder-0.0.5/doFolder/terminal.py` & `doFolder-0.0.6/doFolder/terminal.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         'overwrited':"[cyan]overwrited[/cyan]",
     }
     argparser = argparse.ArgumentParser()
     argparser.add_argument('folder1',type = str, help = 'The first folder to compare')
     argparser.add_argument('folder2',type = str, help = 'The second folder to compare')
     argparser.add_argument('-c', '--content', type = str, choices=['ignore', 'md5', 'sha1', 'sha256', 'sha512', 'hash', 'content', 'size'] ,default="ignore", help = 'How to compare the content of the file')
     argparser.add_argument('-t', '--threaded', action="store_true", help = 'Use multithreaded scanning')
-    argparser.add_argument('-n', '--num', help = 'Maximum number of threads')
+    argparser.add_argument('-n', '--num',type = int,default=10, help = 'Maximum number of threads')
     args = argparser.parse_args()
     folder1 = doFolder.Folder(args.folder1)
     folder2 = doFolder.Folder(args.folder2)
     retsult=comp.compare(folder1, folder2,args.content,args.threaded,args.num)
     fileMissingList=retsult.fileMissingList
     folderMissingList=retsult.folderMissingList
     fileDifferentList=retsult.fileDifferentList
```

### Comparing `doFolder-0.0.5/doFolder.egg-info/PKG-INFO` & `doFolder-0.0.6/doFolder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doFolder
-Version: 0.0.5
+Version: 0.0.6
 Summary: download files quickly
 Home-page: https://kuankuan2007.gitee.io/docs/do-folder/
 Author: kuankuan
 Author-email: 2163826131@qq.com
 License: Mulan PSL v2
 Keywords: file,foler,path,filesystem
 Platform: windows
```

### Comparing `doFolder-0.0.5/setup.py` & `doFolder-0.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from distutils.core import setup
 setup(
     name = 'doFolder',
-    version = '0.0.5',
+    version = '0.0.6',
     keywords = ['file',"foler","path","filesystem"],
     description = 'download files quickly',
     long_description = open("README.rst","r",encoding="utf-8").read(),
     author = 'kuankuan',
     author_email = '2163826131@qq.com',
     url="https://kuankuan2007.gitee.io/docs/do-folder/",
     install_requires = [
```

