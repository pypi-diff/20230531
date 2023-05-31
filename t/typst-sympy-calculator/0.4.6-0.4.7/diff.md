# Comparing `tmp/typst_sympy_calculator-0.4.6-py3-none-any.whl.zip` & `tmp/typst_sympy_calculator-0.4.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 33115 bytes, number of entries: 14
--rw-rw-rw-  2.0 fat     7111 b- defN 23-May-30 15:03 DefaultTypstCalculator.py
+Zip file size: 33138 bytes, number of entries: 14
+-rw-rw-rw-  2.0 fat     7111 b- defN 23-May-31 13:00 DefaultTypstCalculator.py
 -rw-rw-rw-  2.0 fat     4242 b- defN 23-May-30 08:32 TypstCalculator.py
 -rw-rw-rw-  2.0 fat     9984 b- defN 23-May-30 15:34 TypstCalculatorServer.py
--rw-rw-rw-  2.0 fat    21073 b- defN 23-May-30 11:08 TypstConverter.py
+-rw-rw-rw-  2.0 fat    21135 b- defN 23-May-31 13:01 TypstConverter.py
 -rw-rw-rw-  2.0 fat     5488 b- defN 23-May-30 08:34 TypstParser.py
 -rw-rw-rw-  2.0 fat    17356 b- defN 23-May-30 08:52 gen/TypstGrammarLexer.py
 -rw-rw-rw-  2.0 fat    10476 b- defN 23-May-30 08:50 gen/TypstGrammarListener.py
 -rw-rw-rw-  2.0 fat    94820 b- defN 23-May-30 08:52 gen/TypstGrammarParser.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-28 11:15 gen/__init__.py
--rw-rw-rw-  2.0 fat     1080 b- defN 23-May-30 16:52 typst_sympy_calculator-0.4.6.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat    12770 b- defN 23-May-30 16:52 typst_sympy_calculator-0.4.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 16:52 typst_sympy_calculator-0.4.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 16:52 typst_sympy_calculator-0.4.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1169 b- defN 23-May-30 16:52 typst_sympy_calculator-0.4.6.dist-info/RECORD
-14 files, 185753 bytes uncompressed, 31175 bytes compressed:  83.2%
+-rw-rw-rw-  2.0 fat     1080 b- defN 23-May-31 13:03 typst_sympy_calculator-0.4.7.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat    12770 b- defN 23-May-31 13:03 typst_sympy_calculator-0.4.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-31 13:03 typst_sympy_calculator-0.4.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-31 13:03 typst_sympy_calculator-0.4.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1169 b- defN 23-May-31 13:03 typst_sympy_calculator-0.4.7.dist-info/RECORD
+14 files, 185815 bytes uncompressed, 31198 bytes compressed:  83.2%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: gen/TypstGrammarParser.py
 Comment: 
 
 Filename: gen/__init__.py
 Comment: 
 
-Filename: typst_sympy_calculator-0.4.6.dist-info/LICENSE.txt
+Filename: typst_sympy_calculator-0.4.7.dist-info/LICENSE.txt
 Comment: 
 
-Filename: typst_sympy_calculator-0.4.6.dist-info/METADATA
+Filename: typst_sympy_calculator-0.4.7.dist-info/METADATA
 Comment: 
 
-Filename: typst_sympy_calculator-0.4.6.dist-info/WHEEL
+Filename: typst_sympy_calculator-0.4.7.dist-info/WHEEL
 Comment: 
 
-Filename: typst_sympy_calculator-0.4.6.dist-info/top_level.txt
+Filename: typst_sympy_calculator-0.4.7.dist-info/top_level.txt
 Comment: 
 
-Filename: typst_sympy_calculator-0.4.6.dist-info/RECORD
+Filename: typst_sympy_calculator-0.4.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## TypstConverter.py

```diff
@@ -371,15 +371,16 @@
         elif supexpr.expr():
             return self.convert_expr(supexpr.expr())
         else:
             raise Exception(f'unknown supexpr {supexpr.getText()}')
 
     def convert_atom(self, atom):
         if atom.NUMBER():
-            return sympy.Number(atom.NUMBER().getText())
+            # convert to a rational number but not a float
+            return sympy.Rational(atom.NUMBER().getText())
         elif atom.symbol():
             return self.convert_symbol(atom.symbol())
         else:
             raise Exception(f'unknown atom {atom.getText()}')
 
     def convert_symbol(self, symbol):
         symbol_name = symbol.getText()
```

## Comparing `typst_sympy_calculator-0.4.6.dist-info/LICENSE.txt` & `typst_sympy_calculator-0.4.7.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `typst_sympy_calculator-0.4.6.dist-info/METADATA` & `typst_sympy_calculator-0.4.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typst-sympy-calculator
-Version: 0.4.6
+Version: 0.4.7
 Summary: Convert typst math expressions to sympy form with ANTLR and support matrix, calculous and custom functions.
 Home-page: https://github.com/OrangeX4/typst-sympy-calculator
 Author: OrangeX4
 Author-email: orangex4@qq.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

## Comparing `typst_sympy_calculator-0.4.6.dist-info/RECORD` & `typst_sympy_calculator-0.4.7.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 DefaultTypstCalculator.py,sha256=SpwQmZJ3SCXlFTFbXdD1e3nPywwzVztrlYCFEhzxd34,7111
 TypstCalculator.py,sha256=bfCf1g_vPkTDBp3gi8uVwmuybG3HJEspF226CcqVhiI,4242
 TypstCalculatorServer.py,sha256=NvFNnZeP2MbP-ICsIHX1dPOOVYlSn40q2FfulWWrAJg,9984
-TypstConverter.py,sha256=TjOPE9hIi2WEymjwol2yQ1yCqwTs7Ku4qSDoYRy0VRg,21073
+TypstConverter.py,sha256=fPh9d66rUDSspOKVvvdi5ZO0GYr74T2v2gLIKXfqMcI,21135
 TypstParser.py,sha256=DITF_chsZwsHWesL80r56GffmrracxN-3VN-Oi3wfOE,5488
 gen/TypstGrammarLexer.py,sha256=Aikej0mIRul_3e7C1_-2s2F7uwvjUonnl2KF00ta57g,17356
 gen/TypstGrammarListener.py,sha256=xGPQlgbFCe87-de8BySwJkI-WihW4zrhuOYiyxtxKTc,10476
 gen/TypstGrammarParser.py,sha256=aHsN1SilWTuNnwetpk-5LBSB2XUxFC36PtV7YJLYx58,94820
 gen/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-typst_sympy_calculator-0.4.6.dist-info/LICENSE.txt,sha256=1YAQAAy3zt2uDBzPtc72nALzM7sLCQNZFSCANVQ0KR8,1080
-typst_sympy_calculator-0.4.6.dist-info/METADATA,sha256=y0uigTP8-6F7mNpTy1Q0HxCZ7nvG2ovfTqhbEtY8HXE,12770
-typst_sympy_calculator-0.4.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-typst_sympy_calculator-0.4.6.dist-info/top_level.txt,sha256=F4cgxsFQa7AScDESLuHudytwtNvtoTm0J3ioLVCHK_o,92
-typst_sympy_calculator-0.4.6.dist-info/RECORD,,
+typst_sympy_calculator-0.4.7.dist-info/LICENSE.txt,sha256=1YAQAAy3zt2uDBzPtc72nALzM7sLCQNZFSCANVQ0KR8,1080
+typst_sympy_calculator-0.4.7.dist-info/METADATA,sha256=220qBFsx_Pu1-I8kV0H9u4YiTeTcjfdnjWOtTx77eyM,12770
+typst_sympy_calculator-0.4.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+typst_sympy_calculator-0.4.7.dist-info/top_level.txt,sha256=F4cgxsFQa7AScDESLuHudytwtNvtoTm0J3ioLVCHK_o,92
+typst_sympy_calculator-0.4.7.dist-info/RECORD,,
```

