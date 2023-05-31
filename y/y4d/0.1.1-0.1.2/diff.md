# Comparing `tmp/y4d-0.1.1.tar.gz` & `tmp/y4d-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "y4d-0.1.1.tar", max compression
+gzip compressed data, was "y4d-0.1.2.tar", max compression
```

## Comparing `y4d-0.1.1.tar` & `y4d-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      580 2023-05-28 22:50:51.549371 y4d-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      106 2023-05-27 19:34:50.001818 y4d-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-05-27 19:23:01.005617 y4d-0.1.1/y4d/__init__.py
--rw-r--r--   0        0        0     1573 2023-05-28 22:40:01.005087 y4d-0.1.1/y4d/checkAPI.py
--rw-r--r--   0        0        0    15423 2023-05-28 22:39:33.928475 y4d-0.1.1/y4d/codeParser.py
--rw-r--r--   0        0        0     8205 2023-05-28 22:40:55.151188 y4d-0.1.1/y4d/commentController.py
--rw-r--r--   0        0        0     6413 2023-05-28 22:41:16.788704 y4d-0.1.1/y4d/isolator.py
--rw-r--r--   0        0        0    35699 2023-05-28 22:41:39.466605 y4d-0.1.1/y4d/restrictor.py
--rw-r--r--   0        0        0      763 1970-01-01 00:00:00.000000 y4d-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      580 2023-05-31 19:18:15.778486 y4d-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      217 2023-05-31 19:18:03.375800 y4d-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-27 19:23:01.005617 y4d-0.1.2/y4d/__init__.py
+-rw-r--r--   0        0        0     1573 2023-05-31 19:18:56.287396 y4d-0.1.2/y4d/checkAPI.py
+-rw-r--r--   0        0        0    14966 2023-05-31 19:21:03.766957 y4d-0.1.2/y4d/codeParser.py
+-rw-r--r--   0        0        0     7277 2023-05-31 19:20:33.375528 y4d-0.1.2/y4d/commentController.py
+-rw-r--r--   0        0        0     6446 2023-05-31 19:20:08.431889 y4d-0.1.2/y4d/isolator.py
+-rw-r--r--   0        0        0    34273 2023-05-31 19:19:31.594710 y4d-0.1.2/y4d/restrictor.py
+-rw-r--r--   0        0        0      872 1970-01-01 00:00:00.000000 y4d-0.1.2/PKG-INFO
```

### Comparing `y4d-0.1.1/pyproject.toml` & `y4d-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "y4d"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["BahouA <antonbahou@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 checkAPI = "y4d.checkAPI:app"
 restrict = "y4d.restrictor:app"
```

### Comparing `y4d-0.1.1/y4d/checkAPI.py` & `y4d-0.1.2/y4d/checkAPI.py`

 * *Files identical despite different names*

### Comparing `y4d-0.1.1/y4d/codeParser.py` & `y4d-0.1.2/y4d/codeParser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,49 @@
 import json
 import clang.cindex
-from y4d import commentController as commentController
+import re
 from pathlib import Path
 
 def findLocationFunction(data, prototype: str, source):
-    #check for static, virtual, pure virtual, and constru
+    #Check for static, virtual, pure virtual, and constructors
     is_static = False
     is_pure = False
     is_virtual = False
     has_initializer = "false"
     
-    #Check constructos with initializer lists
+    #Check constructors with initializer lists
     if len(prototype.split("(")) > 2:
         has_initializer = "true" 
+
     #Check static functions
     if len(prototype.split("static")) > 1:
         is_static= True
+
     #Check virtual and pure virtual functions
     if len(prototype.split("virtual")) > 1:
         is_virtual= True
         if len( prototype.split("=0")) > 1:
             prototype = prototype.split("=0")[0]
             is_pure= True
         elif len( prototype.split("= 0")) > 1:
             prototype = prototype.split("= 0")[0]
             is_pure= True
             
-    #label function by its type 
+    #Label function by its type 
     if len(prototype.split("template"))> 1 :
         if len(prototype.split("::")) > 1 :
             type = "template_member_function"
         else:
             type = "template_function"
     elif len(prototype.split("::")) > 1:
         type = "member_function"
     else:
         type="function"
     
-    #extract information from function prototype
+    #Extract information from function prototype
     if type == "member_function" or type == "template_member_function":
         parent_class = prototype.split("::")[0].strip().split(" ")[-1]
         returntype = prototype.split(parent_class)[0].strip().split(" ")[-1]
         prototype=prototype.replace(" ", "")
         name = prototype.split("::")[1].split("(")[0]
         if len(name.split("~")) > 1 and name.split("~")[1] == parent_class:
             type = "decstructor"
@@ -60,15 +62,15 @@
             params = params.split(":")[0]
     else:
         params = prototype.split(name)[1]
         
     qualtype = returntype + params
     qualtype = qualtype.replace(" ", "")
 
-    #retrieve position of function
+    #Retrieve position of function
     pos=[]
     if type == "function":
         for item in data['nodes']:
             if item['kind'] == "FUNCTION_DECL" and item['spelling'].replace(" ", "") == name and item['prototype'].replace(" ", "") == qualtype:
                 if is_static == item['is_static_method'] and is_virtual == item['is_virtual_method'] and is_pure == item['is_pure']:
                     end = item['end']
                     start = item['start']
@@ -83,23 +85,23 @@
     if type == "template_function" or type == "template_member_function":
         for item in data['nodes']:
             if (item['kind'] == "FUNCTION_TEMPLATE" and item['spelling'].replace(" ", "") == name and item['prototype'].replace(" ", "") == qualtype and is_static == item['is_static_method'] and ((type == "template_function" and item['access_type'] == "invalid") or ( type == "template_member_function" and item['parent_class'] != "" and parent_class == item['parent_class'].split(" ")[1])  )  ):
                     start = item['start']
                     end =-1
                     with open(source, "r") as source_file:
                         lines = source_file.readlines()    
-                    #check for forward declaration 
+                    #Check for forward declaration 
                     openb =0
                     for char in lines[start-1]:
                         if char == '{':
                             openb = openb+1
                     if openb == 0:
                         pos += [start, start, type, item['access_type']]
                         continue
-                    #find when the function ends 
+                    #Find where the function ends 
                     i = start 
                     while(True):
                         for char in lines[i]:
                             if char == '{':
                                 openb = openb+1
                             if char == '}':
                                 openb = openb -1
@@ -118,15 +120,15 @@
                 pos += [start, end, type, item['access_type']] 
     if type == "decstructor":
         for item in data['nodes']:
             if item['kind'] == "DESTRUCTOR" and item['spelling'].replace(" ", "") == name:
                 end = item['end']
                 start = item['start']
                 pos += [start, end, type, item['access_type']] 
-    
+        
     return pos
 
 def findLocationClass(data, prototype: str, source, type: str, iteration = 0):
     #classes list stores all classes that inherits from\friend with main class in order to parse their member functions and nested classes  
     classes =  [prototype]
     pos=[]
     for class_i in classes:
@@ -165,20 +167,14 @@
                 if item['mangled_name'].startswith('?'):
                     mangledName= item['mangled_name'].split("@")
                     if len(mangledName) > 1 and mangledName[1] == name:
                         if item['kind'] == "CXX_METHOD":
                             returnType = item['prototype'].split(" ")[0]
                             func_prototype = returnType +" " + name + "::" +item['displayname']
                             pos+= findLocationFunction(data, func_prototype, source)
-                    if (item['kind'] == "CONSTRUCTOR" or item['kind'] == "DESTRUCTOR" )and item['parent_class'] == "class "+ name:
-                        returnType = item['prototype'].split(" ")[0]
-                        func_prototype = name + "::" +item['displayname']
-                        if item["initializer_list"] == "true":
-                            func_prototype += "("
-                        pos+= findLocationFunction(data, func_prototype, source)
             #check template member functions  
             if item["kind"] == "FUNCTION_TEMPLATE":
                 start_line = item['start']
                 j = i+1
                 template_node = data['nodes'][j]
                 while  j < len(data['nodes']) and template_node['start'] == start_line:
                     if template_node['kind'] == "TEMPLATE_TYPE_PARAMETER":
@@ -203,37 +199,38 @@
                     classes +=  [type + " "+  item['spelling']]
             i = i+1
         if iteration == 1:
             return pos
 
     return pos
  
+
+
 #find if a constructor has expression initializer list
 def hasInitializerList(cursor):
     for child in cursor.get_children():
         if child.kind.is_expression():
             return True
     return False
-def prepareData (source: str, hide: bool):
-    
-    index = clang.cindex.Index.create()
-    tu = index.parse(source)
-    
-    #check if source code compiles
-    if hide:
-        if len(tu.diagnostics) > 0:
-            print("Error: " + source + " doesn't compile successfully")
-            return ["error"]
 
-    #comment out libraries and include in source file
-    commentController.includePreparer(source)
+
+
+#Compile code and return parse tree
+def prepareData (source: str):
     
-    #Call again with code without libraries and using namespace
+    #Get Code from source
+    with open(source, 'r') as file:
+        source = file.read()
+
+    #String manipulate source for parse to work (removing libraries and using namespace)
+    source = re.sub(r'^#include\s*[\s\S][<"]\S+[>"]$', r'// \g<0>', source, flags=re.MULTILINE)
+    source = re.sub(r'^\s*using\s+namespace\s+\S+;$', r'// \g<0>', source, flags=re.MULTILINE)
+
     index = clang.cindex.Index.create()
-    tu = index.parse(source)
+    tu = index.parse('dud.cpp', unsaved_files=[('dud.cpp', source)])
     
     output = {"nodes": []}
     friendFlag = False
     classPointer = -1
     for node in tu.cursor.walk_preorder():
         access_type =""
         parent_class = ""
@@ -241,46 +238,47 @@
         #Check if the constructor has an expression initializer list
         if node.kind == clang.cindex.CursorKind.CONSTRUCTOR:
             if hasInitializerList(node):
                 initializer_list = "true"
                 
         #Save access type of member functions, anything else will have value "invalid"              
         access_type = str(node.access_specifier).split(".")[1]
-        
         #Save name of parent class
         if access_type == "INVALID":
             parent_class = ""
         else:
             parent = node.semantic_parent
             if parent is None:
                 parent_class=""
             elif parent.kind == clang.cindex.CursorKind.CLASS_DECL:
                 parent_class = "class " + str(parent.spelling)
             elif parent.kind == clang.cindex.CursorKind.STRUCT_DECL:
                 parent_class = "struct " + str(parent.spelling)
             
-        if node.kind == clang.cindex.CursorKind.CLASS_DECL or node.kind == clang.cindex.CursorKind.STRUCT_DECL:
+        if node.kind == clang.cindex.CursorKind.CLASS_DECL:
             classPointer = 0
             friendFlag = False
             
         elif node.kind == clang.cindex.CursorKind.CXX_BASE_SPECIFIER:
             inh = node.spelling
             output["nodes"][classPointer]["inherits_from"].append(inh)
 
         elif node.kind == clang.cindex.CursorKind.FRIEND_DECL:
             friendFlag = True
 
         elif friendFlag:
             friend = node.spelling
-            if len(friend.split("class")) == 1 and len(friend.split("struct")) == 1:
+            if len(friend.split("class")) == 1: #check this: or len(friend.split("struct")):
                 friend = node.type.spelling.split('(')[0] + node.displayname
             output["nodes"][classPointer]["friend_with"].append(friend)
             friendFlag = False
 
         classPointer = classPointer - 1
+
+        #Backbone of the project, retuning parse tree information.
         node_dict = {
             "kind": str(node.kind.name),
             "spelling": node.spelling,
             "prototype": node.type.spelling,
             "displayname": node.displayname,
             "type": str(node.type),
             "start": int(node.location.line),
@@ -299,41 +297,42 @@
             "parent_class" : parent_class,
             "initializer_list" : initializer_list,
         }
         output["nodes"].append(node_dict)
     
     jsonFormat = json.dumps(output, indent=4)
     data = json.loads(jsonFormat)
-    
-    # Revert commenting changes done before
-    commentController.includeRevert(source)
+
     return data
 
+
+#Return postions of anything the user is searching for.
 def positions ( source: str, type: str, prototype: str, option = 0):
     source_path = Path(source)
     if source_path.exists() == False:
         print("Error: " + source + " doesn't exist")
         return ["error"]
     
-    #checking if its .h file and converting it to .cpp, due to libclang capabilities 
+    #Checking if it is a .h file and converting it to .cpp, due to libclang requirements
     file_extension = source_path.suffix
     if file_extension == ".h":
         file_name = source_path.stem
         with open(source, 'r') as source:
             content = source.read()
         destination_file = file_name + ".cpp"
         with open(destination_file, 'w') as destination:
             destination.write(content)
         source = destination_file
         
-    data = prepareData(source, True)
-    if data == ["error"]:
-        return data
+    #Compiling the code
+    data = prepareData(source)
+    
+    #Varibale for saving position of anything the user is searching for.
     pos =[]
     
     if type == "class" or type == "struct":
         pos = findLocationClass(data, prototype , source, type, option)  
         
     if type == "function":
         pos = findLocationFunction( data, prototype, source)  
         
-    return pos
+    return pos
```

### Comparing `y4d-0.1.1/y4d/commentController.py` & `y4d-0.1.2/y4d/commentController.py`

 * *Files 10% similar despite different names*

```diff
@@ -164,37 +164,9 @@
     """
     This tool will comment out a function implementation from a C++ file using a function prototype (equivalent to deleting the function).
     """
     commentMaker(source, "function" , prototype, isolate, 0, output)
 
 
 
-#This function comments out all includes and using namespaces, this is needed to make libclang work properly
-def includePreparer(input: str):
-
-    with open(input, 'r') as f:
-        source = f.read()
-
-    source = re.sub(r'^#include\s*[\s\S][<"]\S+[>"]$', r'// \g<0>', source, flags=re.MULTILINE)
-    source = re.sub(r'^\s*using\s+namespace\s+\S+;$', r'// \g<0>', source, flags=re.MULTILINE)
-
-    with open(input, 'w') as f:
-        f.write(source)
-
-
-
-#This function comments out all includes and using namespaces, this is needed to make libclang work properly
-def includeRevert(input: str):
-
-    with open(input, 'r') as f:
-        source = f.read()
-
-    source = re.sub(r'^//\s*#include\s*', r'#include ', source, flags=re.MULTILINE)
-    source = re.sub(r'^\s*//\s*using\s+namespace\s*', r'using namespace ', source, flags=re.MULTILINE)
-
-    with open(input, 'w') as f:
-        f.write(source)
-
-
-
 if __name__ == "__main__":
     app()
```

### Comparing `y4d-0.1.1/y4d/isolator.py` & `y4d-0.1.2/y4d/isolator.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,33 +10,33 @@
 def isolateFunction(source: str  = typer.Argument(..., help="The source code that the function will be isolated from (.cpp/.h)"),
                     destination: str  = typer.Argument(..., help="The destination code where the function will be embedded or replaced (.cpp/.h)"),
                     prototype: str  = typer.Argument(..., help="The function prototype: return-type function-name parameters-types. In the case of member functions return-type class-name::function-name parameters-types. Example: int test(int, string). Must put them in quotations when using CLI.")):
     """
     This tool will isolate out a function, the function will be taken from source and replace the one in destination or add one.
     """
     
-    findFunction = codeParser.positions(source,"function", prototype)
+    findFunction = codeParser.positions(source,"function", prototype, True)
     if findFunction == ["error"]:
         return
     if findFunction == []:
         print("Warning: Function doesn't exist in " + source +" file")
         return 
     
     # Open the source file and read its contents
     with open(source, "r") as source_file:
         lines = source_file.readlines() 
     
     #check if its a member function and parent class exists in destination file 
     if findFunction[2] != "function" and findFunction[2] != "template_function":
         parent_class = prototype.split("::")[0].strip().split(" ")[-1]
-        findClass = codeParser.positions(destination, "class", "class " + parent_class)
+        findClass = codeParser.positions(destination, "class", "class " + parent_class, False)
         if findClass == ["error"]:
             return
         if findClass == []:
-            findClass = codeParser.positions(destination, "struct", "struct " + parent_class)
+            findClass = codeParser.positions(destination, "struct", "struct " + parent_class, False)
             if findClass == ["error"]:
                 return
             if findClass == []:
                 print("Warning: Parent Class doesn't exist in " +destination +" file")
                 return 
         class_end = findClass[1]
         #fixing protoype
@@ -86,15 +86,15 @@
     """
     This tool will isolate out a class, the class will be taken from source and replace the one in destination or add one.
     """
     option =0
     if all.lower() == "false":
         option = 1
     type = prototype.split(" ")[0]
-    position = codeParser.positions(source, type, prototype, option)
+    position = codeParser.positions(source, type, prototype, True, option)
     
     if position == ["error"]:
         return
     
     #checking if class exists in source code
     if position == []:
         print("Class not found in " + source)
@@ -112,15 +112,15 @@
         start_line = position[i]
         end_line = position[i+1]
         #functions implemented outside a class
         if start_line <= class_start or end_line >= class_end:
             things += lines[start_line - 1:end_line]
     
     #checking if class already exists in destination code and commenting it out
-    class_position = codeParser.positions(destination, type, prototype, 1)
+    class_position = codeParser.positions(destination, type, prototype, False, 1)
     if class_position == ["error"]:
         return
     commentController.CommentOutClass(destination, prototype, all, 1, destination)
     
     with open(destination, "r") as destination_file:
         lines = destination_file.readlines()
```

### Comparing `y4d-0.1.1/y4d/restrictor.py` & `y4d-0.1.2/y4d/restrictor.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,48 +6,51 @@
 from y4d import commentController as commentController
 
 app = typer.Typer()
 
 #Returns everything in the scope the user defined
 def scopeGetter(source:str, scope:str ):
     #Checks if scope for function or class
-        type = scope.split(" ")[0]
-        if type != "class":
-            type = "function"
-        
-        #Find where function or class is
-        pos = codeParser.positions(source, type, scope)
-        if pos == ["error"]:
-            return
-        if pos == []:
-            print("Warning: " + type + "doesn't exist in " + source +" file")
-            return
-        searchPos = []
-        count = 0
-        for p in pos:
-            if count != 2:
-                searchPos.append(p)
-                count += 1
-            else:
-                count = 0
+    type = scope.split(" ")[0]
+    if type != "class":
+        type = "function"
+    
+    #Find where function or class is
+    pos = codeParser.positions(source, type, scope)
+    if pos == ["error"]:
+        return ["error"]
+    if pos == []:
+        print("Warning: " + type + " doesn't exist in " + source +" file")
+        return ["error"]
+    searchPos = []
+    count = 0
+
+    for p in pos:
+        if count != 2 and count != 3:
+            searchPos.append(p)
+            count += 1
+        elif count == 2:
+            count += 1
+        else:
+            count = 0
 
-        #Get back only the lines in the specified scope
-        with open(source, 'r') as f:
-            source = f.readlines()
-        scopeLines = []
-        i = 0
-        while i < len(searchPos):
-            j = searchPos[i] - 1
-            while j < searchPos[i+1]:
-                scopeLines.append(source[j])
-                j += 1
-            i += 2
+    #Get back only the lines in the specified scope
+    with open(source, 'r') as f:
+        source = f.readlines()
+    scopeLines = []
+    i = 0
+    while i < len(searchPos):
+        j = searchPos[i] - 1
+        while j < searchPos[i+1]:
+            scopeLines.append(source[j])
+            j += 1
+        i += 2
 
-        source = '\n'.join(scopeLines)
-        return source
+    source = '\n'.join(scopeLines)
+    return source
 
 
 
 #Function that uses all other restriction functions that are below it, it recieves a YAML file which lets it know which functions to run
 @app.command("r")
 def restrict(source: str  = typer.Argument(..., help="The path of the .cpp or .h file the user wants restrictor to work on."),
              rules: str  = typer.Argument(..., help="The path of the YAML file containing user requirements."),
@@ -84,16 +87,16 @@
     violationCount = 0
 
     for criteria, critData in jsonData.items():
         #The following code is to print the findings of the code for each criteria in the YAML file
         if critOld != "start":
             if exactCount != 0 and compareCount != exactCount:
                 critAns = critAns & False
-            if critData['restriction'].lower() == 'exactly' and not critAns and not outputBool and not hide:
-                print(critOld + " are not exactly the same.")
+            # if critData['restriction'].lower() == 'exactly' and not critAns and not outputBool and not hide:
+            #     print(critOld + " are not exactly the same.")
             critAns = True
             compareCount = 0
             exactCount = 0
 
         critOld = criteria
 
         #Handles libraries in YAML file
@@ -179,25 +182,21 @@
                             if not hide:
                                 print("Missing class: " + cls)
                             else:
                                 print("Extra class: " + cls)
                     exactCount += 1
                     if exactCount == 1:
                         if critData['scope'].lower() == "global" or critData['scope'] == "":
-                            data = codeParser.prepareData(newSource, True)
-                            if data == ["error"]:
-                                return False
+                            data = codeParser.prepareData(newSource)
                         else:
                             scopeG = scopeGetter(newSource, critData['scope'])
                             file = open("restrictorGen.cpp", "w")
                             file.write(scopeG)
                             file.close()
-                            data = codeParser.prepareData("restrictorGen.cpp", True)
-                            if data == ["error"]:
-                                return False
+                            data = codeParser.prepareData("restrictorGen.cpp")
                         for decl in data['nodes']:
                             if decl['kind'] == "CLASS_DECL" and decl['start'] != decl['end']:
                                 compareCount += 1
 
         #Handles functions in YAML file
         elif criteria == 'functions':
             for func in critData['names']:
@@ -220,25 +219,21 @@
                             if not hide:
                                 print("Missing function: " + func)
                             else:
                                 print("Extra function: " + func)
                     exactCount += 1
                     if exactCount == 1:
                         if critData['scope'].lower() == "global" or critData['scope'] == "":
-                             data = codeParser.prepareData(newSource, True)
-                             if data == ["error"]:
-                                return False
+                             data = codeParser.prepareData(newSource)
                         else:
                             scopeG = scopeGetter(newSource, critData['scope'])
                             file = open("restrictorGen.cpp", "w")
                             file.write(scopeG)
                             file.close()
-                            data = codeParser.prepareData("restrictorGen.cpp", True)
-                            if data == ["error"]:
-                                return False
+                            data = codeParser.prepareData("restrictorGen.cpp")
                         for decl in data['nodes']:
                             if decl['kind'] == "FUNCTION_DECL" and decl['start'] != decl['end']:
                                 compareCount += 1
 
         #Handles (private/public/protected) functions in YAML file
         elif criteria == 'private_functions' or criteria == 'public_functions' or criteria == 'protected_functions':
             access = criteria.split("_")[0].upper()
@@ -262,39 +257,35 @@
                             if not hide:
                                 print("Missing " + access + " function: " + func)
                             else:
                                 print("Extra " + access + " function: " + func)
                     exactCount += 1
                     if exactCount == 1:
                         if critData['scope'].lower() == "global" or critData['scope'] == "":
-                             data = codeParser.prepareData(newSource, True)
-                             if data == ["error"]:
-                                return False
+                             data = codeParser.prepareData(newSource)
                         else:
                             scopeG = scopeGetter(newSource, critData['scope'])
                             file = open("restrictorGen.cpp", "w")
                             file.write(scopeG)
                             file.close()
-                            data = codeParser.prepareData("restrictorGen.cpp", True)
-                            if data == ["error"]:
-                                return False
+                            data = codeParser.prepareData("restrictorGen.cpp")
                         for decl in data['nodes']:
                             if decl['kind'] == "CXX_METHOD" and decl['access_type'] == access and (decl['start'] != decl['end'] or decl['is_virtual_method'] == True):
                                 if decl['is_virtual_method'] == True:
                                     if decl['parent_class'] in parentCheck:
                                         compareCount -= 1
                                     parentCheck.append(decl['parent_class'])
                                 compareCount += 1
     
 
     #To print the last criteria in the loop
     if exactCount != 0 and compareCount != exactCount:
         critAns = critAns & False
-    if critData['restriction'].lower() == "exactly" and not critAns and not outputBool and not hide:
-        print(critOld + " are not exactly the same.")
+    # if critData['restriction'].lower() == "exactly" and not critAns and not outputBool and not hide:
+    #     print(critOld + " are not exactly the same.")
     if outputBool:
         print(violationCount)
     
 
 
 
 #Function to restrict a single library, no need for the YAML file, further explanation available exactly below function definition
@@ -329,18 +320,19 @@
                     print("False")
                 return False
 
     #Handles restriction types "at_least" and "forbidden"
     else:
         existFlag = False
         header = re.findall(r'^#include\s*[\s\S][<"]\S+[>"]$', source, flags=re.MULTILINE)
-        lib1 = "#include <" + lib + ">"
-        lib2 = "#include \""+ lib + "\""
+        lib1 = "#include<" + lib + ">"
+        lib2 = "#include\""+ lib + "\""
 
         for library in header:
+            library = library.replace(" ","")
             if library == lib1 or library == lib2:
                 existFlag = True
 
         if restriction.lower() == "forbidden":
             if existFlag == False:
                 if not hide:
                     print("True")
@@ -379,17 +371,19 @@
     
     #Check if global scope or not, if not then use scopeGetter to get everything in the scope defined by the user
     if scope.lower() == "global" or scope == "":
         with open(source, 'r') as f:
             source = f.read()
     else:
         source = scopeGetter(source, scope)
+        if source == ["error"]:
+            return False
     
     #Check if keyword exists and print true or false according to restriction
-    if re.search(fr"(?i).*{re.escape(keyword)}.*", source):
+    if re.search(fr"(?i).*return\s*[^\n;]+{re.escape(keyword)}.*", source):
         if restriction.lower() == "at_least" or restriction.lower() == "exactly":
             if not hide:
                 print("True")
             return True
         elif restriction.lower() == "forbidden":
             if not hide:
                 print("False")
@@ -420,29 +414,25 @@
     #Makes sure that restriction inputted is a viable restriction
     if restriction.lower() not in ["exactly", "forbidden", "at_least"]:
         print("Invalid Restriction Input")
         return False
     
     #Check if global scope or not, if not then use scopeGetter to get everything in the scope defined by the user
     if scope.lower() == "global" or scope == "":
-        data = codeParser.prepareData(source, True)
-        if data == ["error"]:
-            return False
+        data = codeParser.prepareData(source)
         with open(source, 'r') as f:
             scopeG = f.read()
     else:
         scopeG = scopeGetter(source, scope)
         if scopeG == ["error"]:
             return False
         file = open("restrictorGen.cpp", "w")
         file.write(scopeG)
         file.close()
-        data = codeParser.prepareData("restrictorGen.cpp", False)
-        if data == ["error"]:
-            return False
+        data = codeParser.prepareData("restrictorGen.cpp")
 
     prototype = prototype.strip()
     empty = []
     #Check if class exists and print true or false according to restriction
     if codeParser.findLocationClass(data, prototype, source, "class") != empty:
         if restriction.lower() == "exactly":
             if len(re.findall(r"(?:(?<=\s)|(?<=^))class.*?\{(?=\s|$)", scopeG, flags=re.MULTILINE)) > 1:
@@ -487,39 +477,25 @@
     #Makes sure that restriction inputted is a viable restriction
     if restriction.lower() not in ["exactly", "forbidden", "at_least"]:
         print("Invalid Restriction Input")
         return False
     
     #Check if global scope or not, if not then use scopeGetter to get everything in the scope defined by the user
     if scope.lower() == "global" or scope == "":
-        data = codeParser.prepareData(source, True)
-        if data == ["error"]:
-            return False
+        data = codeParser.prepareData(source)
         with open(source, 'r') as f:
             scopeG = f.read()
     else:
         scopeG = scopeGetter(source, scope)
         if scopeG == ["error"]:
             return False
         file = open("restrictorGen.cpp", "w")
         file.write(scopeG)
         file.close()
-        data = codeParser.prepareData("restrictorGen.cpp", False)
-        if data == ["error"]:
-            return False
-    
-    #Making the regex suitable to find function no matter the user input
-    prototype = prototype.strip()
-    prototypeName = prototype.split("(")[0] + "\s*"
-    prototypeName += '('
-    prototypeVars = prototype.split("(")[1].split(")")[0].split(",")
-    prototypeRegex = "(?:(?<=\s)|(?<=^))" + prototypeName
-    for p in prototypeVars:
-        prototypeRegex += ".*" + p.strip().split(' ')[0] + ".*,"
-    prototypeRegex = prototypeRegex[:-1] + ').*\n*.*{[\s\S]*}(?=\s|$)'
+        data = codeParser.prepareData("restrictorGen.cpp")
 
     empty = []
     #Check if function exists and print true or false according to restriction
     if codeParser.findLocationFunction(data, prototype, source) != empty:
         if restriction.lower() == "exactly":
             if len(re.findall(r"\b[a-zA-Z_][a-zA-Z0-9_]*\s+[a-zA-Z_][a-zA-Z0-9_]*\s*\([^)]*\)\s*\{[^{}]*\}", scopeG, flags=re.MULTILINE)) > 1:
                 if not hide:
@@ -563,37 +539,33 @@
     #Makes sure that restriction inputted is a viable restriction
     if restriction.lower() not in ["exactly", "forbidden", "at_least"]:
         print("Invalid Restriction Input")
         return False
     
     #Check if global scope or not, if not then use scopeGetter to get everything in the scope defined by the user as well as preparing data for access_type search
     if scope.lower() == "global" or scope == "":
-        data = codeParser.prepareData(source, True)
-        if data == ["error"]:
-            return False
+        data = codeParser.prepareData(source)
     else:
         scopeG = scopeGetter(source, scope)
         if scopeG == ["error"]:
             return False
         file = open("restrictorGen.cpp", "w")
         file.write(scopeG)
         file.close()
-        data = codeParser.prepareData("restrictorGen.cpp", False)
-        if data == ["error"]:
-            return False
+        data = codeParser.prepareData("restrictorGen.cpp")
 
     #Variables used in the following if statement to find if function is private
     if len(prototype.split("virtual")) == 1 and len(prototype.split("static")) == 1:
         proto = prototype.split(' ')[0] + ' (' + prototype.split('(')[1].strip()
     else:
         proto = prototype.split(' ')[1] + ' (' + prototype.split('(')[1].strip()
     spelling = prototype.split('(')[0].split(' ')[-1].split('::')[-1]
     
     for decl in data['nodes']:
-        if decl['kind'] == "CXX_METHOD" and decl['spelling'] == spelling and decl['prototype'] == proto and decl['access_type'] == type.upper():
+        if decl['kind'] == "CXX_METHOD" and decl['spelling'] == spelling and decl['prototype'].replace(" ","") == proto.replace(" ","") and decl['access_type'] == type.lower():
             return funcRestrict(source, restriction, prototype, scope, hide)
     if not hide:
         print("False")
     return False
 
 
 
@@ -607,17 +579,15 @@
     This tool will compare two files together, the source and compare file, it will check if the function prototypes and class names match then return true or false accordingly.
     """
     #Used to control the style of output
     if output not in ["n", "N", "V", "v"]:
         print("Invalid -o input")
         return False
 
-    data = codeParser.prepareData(compare, True)
-    if data == ["error"]:
-        return False
+    data = codeParser.prepareData(compare)
 
     #Makes sure that restriction inputted is a viable restriction
     if restriction.lower() not in ["exactly", "forbidden", "at_least"]:
         print("Invalid Restriction Input")
         return False
     
     #Varibales and loop used to create the YAML file needed to run restrictor, YAML file made from compare file.
@@ -641,19 +611,19 @@
                 virtual = ""
             if decl['is_const_method'] == True:
                 const = " const"
             else:
                 const = ""
             if decl['access_type'] == "":
                 allFunctions.append(decl['prototype'].split(' ')[0] + unsigned + " " + decl['displayname'] + const)
-            elif decl['access_type'] == 'PRIVATE':
+            elif decl['access_type'] == 'private':
                 allPrivFunctions.append(virtual + decl['prototype'].split(' ')[0] + unsigned + " " + decl['parent_class'].split(' ')[1] + "::" + decl['displayname'] + const)
-            elif decl['access_type'] == 'PUBLIC':
+            elif decl['access_type'] == 'public':
                 allPublicFunctions.append(virtual + decl['prototype'].split(' ')[0] + unsigned + " " + decl['parent_class'].split(' ')[1] + "::" + decl['displayname'] + const)
-            elif decl['access_type'] == 'PROTECTED':
+            elif decl['access_type'] == 'protected':
                 allProtectedFunctions.append(virtual + decl['prototype'].split(' ')[0] + unsigned + " " + decl['parent_class'].split(' ')[1] + "::" + decl['displayname'] + const )
         elif decl['kind'] == "FUNCTION_DECL":
             if len(decl['prototype'].split('(')[0].split('**')) == 1 and len(decl['prototype'].split('(')[0].split('*')) == 1:
                 allFunctions.append(decl['prototype'].split(' ')[0] + unsigned + " " + decl['displayname'] + const)
             elif len(decl['prototype'].split('**')) > 1:
                 allFunctions.append(decl['prototype'].split('**')[0] + unsigned + "** " + decl['displayname'] + const)
             else:
```

