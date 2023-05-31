# Comparing `tmp/pyndjs-0.0.5.tar.gz` & `tmp/pyndjs-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyndjs-0.0.5.tar", last modified: Wed May 31 07:10:09 2023, max compression
+gzip compressed data, was "pyndjs-0.0.6.tar", last modified: Wed May 31 10:09:26 2023, max compression
```

## Comparing `pyndjs-0.0.5.tar` & `pyndjs-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 07:10:09.752204 pyndjs-0.0.5/
--rw-rw-rw-   0        0        0      160 2023-05-31 07:10:09.751198 pyndjs-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-31 07:10:09.743882 pyndjs-0.0.5/pyndjs/
--rw-rw-rw-   0        0        0       52 2023-02-08 08:23:02.000000 pyndjs-0.0.5/pyndjs/__init__.py
--rw-rw-rw-   0        0        0     6103 2023-05-31 07:09:59.000000 pyndjs-0.0.5/pyndjs/pyndjs.py
-drwxrwxrwx   0        0        0        0 2023-05-31 07:10:09.750084 pyndjs-0.0.5/pyndjs.egg-info/
--rw-rw-rw-   0        0        0      160 2023-05-31 07:10:09.000000 pyndjs-0.0.5/pyndjs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      193 2023-05-31 07:10:09.000000 pyndjs-0.0.5/pyndjs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 07:10:09.000000 pyndjs-0.0.5/pyndjs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-05-31 07:10:09.000000 pyndjs-0.0.5/pyndjs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-31 07:10:09.000000 pyndjs-0.0.5/pyndjs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 07:10:09.752204 pyndjs-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      275 2023-05-31 07:09:59.000000 pyndjs-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 10:09:26.143917 pyndjs-0.0.6/
+-rw-rw-rw-   0        0        0      160 2023-05-31 10:09:26.142918 pyndjs-0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-31 10:09:26.135535 pyndjs-0.0.6/pyndjs/
+-rw-rw-rw-   0        0        0       52 2023-02-08 08:23:02.000000 pyndjs-0.0.6/pyndjs/__init__.py
+-rw-rw-rw-   0        0        0     6121 2023-05-31 10:08:45.000000 pyndjs-0.0.6/pyndjs/pyndjs.py
+drwxrwxrwx   0        0        0        0 2023-05-31 10:09:26.141912 pyndjs-0.0.6/pyndjs.egg-info/
+-rw-rw-rw-   0        0        0      160 2023-05-31 10:09:26.000000 pyndjs-0.0.6/pyndjs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      193 2023-05-31 10:09:26.000000 pyndjs-0.0.6/pyndjs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 10:09:26.000000 pyndjs-0.0.6/pyndjs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-05-31 10:09:26.000000 pyndjs-0.0.6/pyndjs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-31 10:09:26.000000 pyndjs-0.0.6/pyndjs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-31 10:09:26.143917 pyndjs-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      275 2023-05-31 10:09:20.000000 pyndjs-0.0.6/setup.py
```

### Comparing `pyndjs-0.0.5/pyndjs/pyndjs.py` & `pyndjs-0.0.6/pyndjs/pyndjs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 from subprocess import Popen
 import six, sys, json, re, os
 
+print('\033[0;32m有问题欢迎随时联系：qq：1341977093\033[m')
+print(f'\033[0;36mnode路径：{os.popen("where node").read().strip()}')
+print(f'node版本：{os.popen("node -v").read()}\033[m'.strip())
+
 def _json2_source():
     return 'var JSON;if(!JSON){JSON={}}(function(){function f(n){return n<10?"0"+n:n}if(typeof Date.prototype.toJSON!=="function"){Date.prototype.toJSON=function(key){return isFinite(this.valueOf())?this.getUTCFullYear()+"-"+f(this.getUTCMonth()+1)+"-"+f(this.getUTCDate())+"T"+f(this.getUTCHours())+":"+f(this.getUTCMinutes())+":"+f(this.getUTCSeconds())+"Z":null};String.prototype.toJSON=Number.prototype.toJSON=Boolean.prototype.toJSON=function(key){return this.valueOf()}}var cx=/[\\u0000\\u00ad\\u0600-\\u0604\\u070f\\u17b4\\u17b5\\u200c-\\u200f\\u2028-\\u202f\\u2060-\\u206f\\ufeff\\ufff0-\\uffff]/g,escapable=/[\\\\\\"\\x00-\\x1f\\x7f-\\x9f\\u00ad\\u0600-\\u0604\\u070f\\u17b4\\u17b5\\u200c-\\u200f\\u2028-\\u202f\\u2060-\\u206f\\ufeff\\ufff0-\\uffff]/g,gap,indent,meta={"\\b":"\\\\b","\\t":"\\\\t","\\n":"\\\\n","\\f":"\\\\f","\\r":"\\\\r",\'"\':\'\\\\"\',"\\\\":"\\\\\\\\"},rep;function quote(string){escapable.lastIndex=0;return escapable.test(string)?\'"\'+string.replace(escapable,function(a){var c=meta[a];return typeof c==="string"?c:"\\\\u"+("0000"+a.charCodeAt(0).toString(16)).slice(-4)})+\'"\':\'"\'+string+\'"\'}function str(key,holder){var i,k,v,length,mind=gap,partial,value=holder[key];if(value&&typeof value==="object"&&typeof value.toJSON==="function"){value=value.toJSON(key)}if(typeof rep==="function"){value=rep.call(holder,key,value)}switch(typeof value){case"string":return quote(value);case"number":return isFinite(value)?String(value):"null";case"boolean":case"null":return String(value);case"object":if(!value){return"null"}gap+=indent;partial=[];if(Object.prototype.toString.apply(value)==="[object Array]"){length=value.length;for(i=0;i<length;i+=1){partial[i]=str(i,value)||"null"}v=partial.length===0?"[]":gap?"[\\n"+gap+partial.join(",\\n"+gap)+"\\n"+mind+"]":"["+partial.join(",")+"]";gap=mind;return v}if(rep&&typeof rep==="object"){length=rep.length;for(i=0;i<length;i+=1){if(typeof rep[i]==="string"){k=rep[i];v=str(k,value);if(v){partial.push(quote(k)+(gap?": ":":")+v)}}}}else{for(k in value){if(Object.prototype.hasOwnProperty.call(value,k)){v=str(k,value);if(v){partial.push(quote(k)+(gap?": ":":")+v)}}}}v=partial.length===0?"{}":gap?"{\\n"+gap+partial.join(",\\n"+gap)+"\\n"+mind+"}":"{"+partial.join(",")+"}";gap=mind;return v}}if(typeof JSON.stringify!=="function"){JSON.stringify=function(value,replacer,space){var i;gap="";indent="";if(typeof space==="number"){for(i=0;i<space;i+=1){indent+=" "}}else{if(typeof space==="string"){indent=space}}rep=replacer;if(replacer&&typeof replacer!=="function"&&(typeof replacer!=="object"||typeof replacer.length!=="number")){throw new Error("JSON.stringify")}return str("",{"":value})}}if(typeof JSON.parse!=="function"){JSON.parse=function(text,reviver){var j;function walk(holder,key){var k,v,value=holder[key];if(value&&typeof value==="object"){for(k in value){if(Object.prototype.hasOwnProperty.call(value,k)){v=walk(value,k);if(v!==undefined){value[k]=v}else{delete value[k]}}}}return reviver.call(holder,key,value)}text=String(text);cx.lastIndex=0;if(cx.test(text)){text=text.replace(cx,function(a){return"\\\\u"+("0000"+a.charCodeAt(0).toString(16)).slice(-4)})}if(/^[\\],:{}\\s]*$/.test(text.replace(/\\\\(?:["\\\\\\/bfnrt]|u[0-9a-fA-F]{4})/g,"@").replace(/"[^"\\\\\\n\\r]*"|true|false|null|-?\\d+(?:\\.\\d*)?(?:[eE][+\\-]?\\d+)?/g,"]").replace(/(?:^|:|,)(?:\\s*\\[)+/g,""))){j=eval("("+text+")");return typeof reviver==="function"?walk({"":j},""):j}throw new SyntaxError("JSON.parse")}}}());'
 
 
 def encode_unicode_codepoints(str):
     codepoint_format = '\\u{0:04x}'.format
 
@@ -51,17 +55,14 @@
     runner_source = re.sub(pattern, lambda m: replacements[m.group(0)](), runner_source)
     return runner_source
 
 
 def execute(js_code, fun_name, args, node_path=os.popen("where node").read().strip(), encoding='utf-8'):
     js_code = js_code + "\n" + \
              r"""return eval('('+"{}.apply(this, {})"+')')""".format(fun_name, args)
-    print('\033[0;32m有问题欢迎随时联系：qq：1341977093\033[m')
-    print(f'\033[0;36mnode路径：{node_path}')
-    print(f'node版本：{os.popen("node -v").read()}\033[m'.strip())
     cmd = [node_path.replace('\\', '/')]
     try:
         p = Popen(cmd, stdin=-1, stdout=-1, stderr=-1, cwd=None, universal_newlines=True, encoding=encoding)
         input = _compile(js_code)
         if six.PY2:
             input = input.encode(sys.getfilesystemencoding())
         stdoutdata, stderrdata = p.communicate(input=input)
```

