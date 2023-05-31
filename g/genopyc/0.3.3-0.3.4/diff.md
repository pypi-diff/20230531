# Comparing `tmp/genopyc-0.3.3-py3-none-any.whl.zip` & `tmp/genopyc-0.3.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 18358 bytes, number of entries: 7
+Zip file size: 18394 bytes, number of entries: 7
 -rwxrwxrwx  2.0 unx      958 b- defN 23-May-31 10:58 genopyc/__init__.py
--rwxrwxrwx  2.0 unx    23936 b- defN 23-May-31 10:49 genopyc/genopyc.py
--rwxrwxrwx  2.0 unx    34523 b- defN 23-May-31 10:59 genopyc-0.3.3.dist-info/LICENSE.txt
--rwxrwxrwx  2.0 unx      463 b- defN 23-May-31 10:59 genopyc-0.3.3.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 23-May-31 10:59 genopyc-0.3.3.dist-info/WHEEL
--rwxrwxrwx  2.0 unx        8 b- defN 23-May-31 10:59 genopyc-0.3.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      540 b- defN 23-May-31 10:59 genopyc-0.3.3.dist-info/RECORD
-7 files, 60520 bytes uncompressed, 17404 bytes compressed:  71.2%
+-rwxrwxrwx  2.0 unx    24064 b- defN 23-May-31 11:18 genopyc/genopyc.py
+-rwxrwxrwx  2.0 unx    34523 b- defN 23-May-31 11:19 genopyc-0.3.4.dist-info/LICENSE.txt
+-rwxrwxrwx  2.0 unx      463 b- defN 23-May-31 11:19 genopyc-0.3.4.dist-info/METADATA
+-rwxrwxrwx  2.0 unx       92 b- defN 23-May-31 11:19 genopyc-0.3.4.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx        8 b- defN 23-May-31 11:19 genopyc-0.3.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      540 b- defN 23-May-31 11:19 genopyc-0.3.4.dist-info/RECORD
+7 files, 60648 bytes uncompressed, 17440 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: genopyc/__init__.py
 Comment: 
 
 Filename: genopyc/genopyc.py
 Comment: 
 
-Filename: genopyc-0.3.3.dist-info/LICENSE.txt
+Filename: genopyc-0.3.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: genopyc-0.3.3.dist-info/METADATA
+Filename: genopyc-0.3.4.dist-info/METADATA
 Comment: 
 
-Filename: genopyc-0.3.3.dist-info/WHEEL
+Filename: genopyc-0.3.4.dist-info/WHEEL
 Comment: 
 
-Filename: genopyc-0.3.3.dist-info/top_level.txt
+Filename: genopyc-0.3.4.dist-info/top_level.txt
 Comment: 
 
-Filename: genopyc-0.3.3.dist-info/RECORD
+Filename: genopyc-0.3.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## genopyc/genopyc.py

```diff
@@ -593,17 +593,20 @@
                   variants{
                       id
                       }
                    }
               }
               """
         for variant in ListOfVariants:
-            r = requests.post(OT_url, json={'query': query % (variant)})
-            JsonResponse=r.json()
-            MappingDict[variant]=JsonResponse['data']['search']['variants'][0]['id']
+            try:
+                r = requests.post(OT_url, json={'query': query % (variant)})
+                JsonResponse=r.json()
+                MappingDict[variant]=JsonResponse['data']['search']['variants'][0]['id']
+            except Exception as e:
+                print(e, f"Couldn't Convert Variant {variant}")
         return list(map(MappingDict.get,ListOfVariants))
 
 
     
 def OTVariantsToGenes(ListofVariants,score=0.1,output='genes'):
     query="""{
               genesForVariant(variantId:"%s"){
```

## Comparing `genopyc-0.3.3.dist-info/LICENSE.txt` & `genopyc-0.3.4.dist-info/LICENSE.txt`

 * *Files identical despite different names*

