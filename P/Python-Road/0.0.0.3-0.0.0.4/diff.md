# Comparing `tmp/Python_Road-0.0.0.3.tar.gz` & `tmp/Python_Road-0.0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Python_Road-0.0.0.3.tar", last modified: Tue May 30 13:41:03 2023, max compression
+gzip compressed data, was "Python_Road-0.0.0.4.tar", last modified: Wed May 31 10:55:33 2023, max compression
```

## Comparing `Python_Road-0.0.0.3.tar` & `Python_Road-0.0.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 13:41:03.094923 Python_Road-0.0.0.3/
--rw-rw-rw-   0        0        0      134 2023-05-30 13:41:03.094923 Python_Road-0.0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-30 13:41:03.094923 Python_Road-0.0.0.3/Python_Road.egg-info/
--rw-rw-rw-   0        0        0      134 2023-05-30 13:41:02.000000 Python_Road-0.0.0.3/Python_Road.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      163 2023-05-30 13:41:03.000000 Python_Road-0.0.0.3/Python_Road.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 13:41:02.000000 Python_Road-0.0.0.3/Python_Road.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 13:41:02.000000 Python_Road-0.0.0.3/Python_Road.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4412 2023-05-30 13:26:29.000000 Python_Road-0.0.0.3/Python_Road.py
--rw-rw-rw-   0        0        0       42 2023-05-30 13:41:03.094923 Python_Road-0.0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      213 2023-05-30 13:40:13.000000 Python_Road-0.0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 10:55:33.510226 Python_Road-0.0.0.4/
+-rw-rw-rw-   0        0        0      134 2023-05-31 10:55:33.510226 Python_Road-0.0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-31 10:55:33.510226 Python_Road-0.0.0.4/Python_Road.egg-info/
+-rw-rw-rw-   0        0        0      134 2023-05-31 10:55:33.000000 Python_Road-0.0.0.4/Python_Road.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      163 2023-05-31 10:55:33.000000 Python_Road-0.0.0.4/Python_Road.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 10:55:33.000000 Python_Road-0.0.0.4/Python_Road.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 10:55:33.000000 Python_Road-0.0.0.4/Python_Road.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5119 2023-05-31 10:51:36.000000 Python_Road-0.0.0.4/Python_Road.py
+-rw-rw-rw-   0        0        0       42 2023-05-31 10:55:33.510226 Python_Road-0.0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      213 2023-05-31 10:07:18.000000 Python_Road-0.0.0.4/setup.py
```

### Comparing `Python_Road-0.0.0.3/Python_Road.py` & `Python_Road-0.0.0.4/Python_Road.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 import os
-import pygame
-import turtle
+import tqdm
+import requests
 import traceback
 import random
+import sys
 
 
+all_var = {"Size":[],"Math":["pi_string","pi","tau"],"Random":[]}
 all_func = [{"Size":["find_all_size","all_file_size","__get_all_size","__size_small"]},{"Math":["evolution","power","cipher"]},{"Random":["random_number","random_choice","random_number_with_step"]},"printer","eval_inputer","Download_with_progress_bar","if_not_error"]
-class Size:
-	def find_file_size(self, path="C:\\", max_or_min="max"):
-		size_path, size_list = self.__get_all_size(path)
-		if max_or_min == "max":
-			fsize = size_path[size_list.index(max(size_list))][0]
-		elif max_or_min == "min":
-			fsize = size_path[size_list.index(min(size_list))][0]
-		else:
-			raise ValueError("max_or_min参数只能填max或min")
-		return self.__size_small(fsize, size_path, size_list)
 
-	def __get_all_size(self, path):
+
+class Size:
+	def __get_all_size(path):
 		size_path = []
 		for path, file_dir, files in os.walk(path):
 			for file_name in files:
 				size_path.append([os.path.getsize(os.path.join(path, file_name)), os.path.join(path, file_name)])
 			for dir in file_dir:
 				size_path.append([os.path.getsize(os.path.join(path, dir)), os.path.join(path, dir)])
 		size_list = []
 		for i in range(len(size_path)):
 			size_list.append(size_path[i][0])
 		return size_path, size_list
 
+	def find_file_size(self, path="C:\\", max_or_min="max"):
+		size_path, size_list = self.__get_all_size(path)
+		if max_or_min == "max":
+			fsize = size_path[size_list.index(max(size_list))][0]
+		elif max_or_min == "min":
+			fsize = size_path[size_list.index(min(size_list))][0]
+		else:
+			raise ValueError("max_or_min参数只能填max或min")
+		return self.__size_small(fsize, size_path, size_list)
+
 	def __size_small(self, fsize, size_path, size_list):
 		if fsize < 1024:
 			return str(round(fsize, 2)) + 'B', size_path[size_list.index(max(size_list))][1]
 		else:
 			KBX = fsize / 1024
 			if KBX < 1024:
 				return str(round(KBX / 1024, 2)) + 'K', size_path[size_list.index(max(size_list))][1]
@@ -119,14 +123,15 @@
 	inputer = input(string)
 	try:
 		return eval(inputer)
 	except:
 		return inputer
 
 
+# noinspection PyCallingNonCallable
 def Download_with_progress_bar(url, fname):
 	resp = requests.get(url, stream=True)
 	total = int(resp.headers.get('content-length', 0))
 	with open(fname, 'wb') as file, tqdm(
 			desc=fname,
 			total=total,
 			unit='iB',
@@ -134,26 +139,44 @@
 			unit_divisor=1024,
 	) as bar:
 		for data in resp.iter_content(chunk_size=1024):
 			size = file.write(data)
 			bar.update(size)
 
 
-def if_not_error(*args,func):
+def if_not_error(*args,func,if_p=True,if_w=False,path="",txt_name="Error",f_or_e=True):
 	try:
-		print("------------------------------")
-		print("运行成功")
-		print(f"运行结果：{func(*args)}")
-		print("------------------------------")
+		print_str = func(*args)
+		if if_p:
+			print("------------------------------")
+			print("运行成功")
+			print(f"运行结果：{print_str}")
+			print("------------------------------")
+		if if_w and path != "":
+			try:
+				loader = open(path+f"\\{txt_name}.log", "a+")
+				if f_or_e:
+					loader.write("\n"+print_str)
+				else:
+					loader.write(print_str+"\n")
+			except:
+				print("文件地址错误或者加载错误")
 	except:
-		print("------------------------------")
-		print("运行失败")
-		print("错误提示：")
-		print(traceback.format_exc())
-		print("------------------------------")
-
-
+		if if_p:
+			print("------------------------------")
+			print("运行失败")
+			print("错误提示：")
+			print(traceback.format_exc())
+			print("------------------------------")
+		try:
+			loader = open(path + f"\\{txt_name}.log", "a+")
+			if f_or_e:
+				loader.write("\n" + traceback.format_exc())
+			else:
+				loader.write(traceback.format_exc() + "\n")
+		except:
+			print("文件地址错误或者加载错误")
 
 
 math = Math()
 size = Size()
-
+ran = Random()
```

