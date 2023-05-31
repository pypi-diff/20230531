# Comparing `tmp/HawaData-0.5.6.tar.gz` & `tmp/HawaData-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HawaData-0.5.6.tar", last modified: Wed May 24 13:26:41 2023, max compression
+gzip compressed data, was "HawaData-0.5.8.tar", last modified: Wed May 31 13:02:28 2023, max compression
```

## Comparing `HawaData-0.5.6.tar` & `HawaData-0.5.8.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 13:26:41.887565 HawaData-0.5.6/
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 13:26:41.877208 HawaData-0.5.6/HawaData.egg-info/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2544 2023-05-24 13:26:41.000000 HawaData-0.5.6/HawaData.egg-info/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      541 2023-05-24 13:26:41.000000 HawaData-0.5.6/HawaData.egg-info/SOURCES.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-05-24 13:26:41.000000 HawaData-0.5.6/HawaData.egg-info/dependency_links.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-05-24 13:26:41.000000 HawaData-0.5.6/HawaData.egg-info/top_level.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)     2544 2023-05-24 13:26:41.887285 HawaData-0.5.6/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.5.6/README.md
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 13:26:41.877805 HawaData-0.5.6/hawa/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.5.6/hawa/__init__.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 13:26:41.880754 HawaData-0.5.6/hawa/base/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.5.6/hawa/base/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     3014 2023-05-05 08:28:22.000000 HawaData-0.5.6/hawa/base/db.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.5.6/hawa/base/decos.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.5.6/hawa/base/errors.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.5.6/hawa/base/init.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 13:26:41.882420 HawaData-0.5.6/hawa/common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.5.6/hawa/common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     9327 2023-05-24 07:17:27.000000 HawaData-0.5.6/hawa/common/data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5323 2023-05-23 06:47:14.000000 HawaData-0.5.6/hawa/common/query.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2784 2023-05-05 08:28:22.000000 HawaData-0.5.6/hawa/common/utils.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.5.6/hawa/config.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 13:26:41.885020 HawaData-0.5.6/hawa/data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.5.6/hawa/data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.5.6/hawa/data/city.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.5.6/hawa/data/district.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.5.6/hawa/data/klass.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      564 2023-05-22 09:15:45.000000 HawaData-0.5.6/hawa/data/school.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 13:26:41.886128 HawaData-0.5.6/hawa/paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.5.6/hawa/paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    26310 2023-05-24 13:25:10.000000 HawaData-0.5.6/hawa/paper/health.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-05-05 07:06:02.000000 HawaData-0.5.6/hawa/paper/mht.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-05-24 13:26:41.887639 HawaData-0.5.6/setup.cfg
--rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.5.6/setup.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-24 13:26:41.886681 HawaData-0.5.6/test/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.5.6/test/test_query.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-31 13:02:28.339717 HawaData-0.5.8/
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-31 13:02:28.328223 HawaData-0.5.8/HawaData.egg-info/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2612 2023-05-31 13:02:28.000000 HawaData-0.5.8/HawaData.egg-info/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      541 2023-05-31 13:02:28.000000 HawaData-0.5.8/HawaData.egg-info/SOURCES.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-05-31 13:02:28.000000 HawaData-0.5.8/HawaData.egg-info/dependency_links.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-05-31 13:02:28.000000 HawaData-0.5.8/HawaData.egg-info/top_level.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2612 2023-05-31 13:02:28.339445 HawaData-0.5.8/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.5.8/README.md
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-31 13:02:28.329028 HawaData-0.5.8/hawa/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.5.8/hawa/__init__.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-31 13:02:28.331800 HawaData-0.5.8/hawa/base/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.5.8/hawa/base/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3014 2023-05-05 08:28:22.000000 HawaData-0.5.8/hawa/base/db.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.5.8/hawa/base/decos.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.5.8/hawa/base/errors.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.5.8/hawa/base/init.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-31 13:02:28.333933 HawaData-0.5.8/hawa/common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.5.8/hawa/common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     9327 2023-05-24 07:17:27.000000 HawaData-0.5.8/hawa/common/data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5323 2023-05-23 06:47:14.000000 HawaData-0.5.8/hawa/common/query.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2784 2023-05-05 08:28:22.000000 HawaData-0.5.8/hawa/common/utils.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.5.8/hawa/config.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-31 13:02:28.336569 HawaData-0.5.8/hawa/data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.5.8/hawa/data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.5.8/hawa/data/city.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.5.8/hawa/data/district.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.5.8/hawa/data/klass.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      564 2023-05-22 09:15:45.000000 HawaData-0.5.8/hawa/data/school.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-31 13:02:28.338083 HawaData-0.5.8/hawa/paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.5.8/hawa/paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    26659 2023-05-31 12:59:00.000000 HawaData-0.5.8/hawa/paper/health.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-05-05 07:06:02.000000 HawaData-0.5.8/hawa/paper/mht.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-05-31 13:02:28.339793 HawaData-0.5.8/setup.cfg
+-rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.5.8/setup.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-31 13:02:28.338788 HawaData-0.5.8/test/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.5.8/test/test_query.py
```

### Comparing `HawaData-0.5.6/HawaData.egg-info/PKG-INFO` & `HawaData-0.5.8/HawaData.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.5.6
+Version: 0.5.8
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -88,7 +88,9 @@
 - 0.5.0 add health api data
 - 0.5.1 add grade param
 - 0.5.2 fix score rank percent
 - 0.5.3 add NoCasesError
 - 0.5.4 add NoCasesError
 - 0.5.5 add gender compare data to health api
 - 0.5.6 add dim or field gender compare data to health api
+- 0.5.7 update describe_grade_text
+- 0.5.8 update other report text
```

### Comparing `HawaData-0.5.6/HawaData.egg-info/SOURCES.txt` & `HawaData-0.5.8/HawaData.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.6/PKG-INFO` & `HawaData-0.5.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.5.6
+Version: 0.5.8
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -88,7 +88,9 @@
 - 0.5.0 add health api data
 - 0.5.1 add grade param
 - 0.5.2 fix score rank percent
 - 0.5.3 add NoCasesError
 - 0.5.4 add NoCasesError
 - 0.5.5 add gender compare data to health api
 - 0.5.6 add dim or field gender compare data to health api
+- 0.5.7 update describe_grade_text
+- 0.5.8 update other report text
```

### Comparing `HawaData-0.5.6/README.md` & `HawaData-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.6/hawa/base/db.py` & `HawaData-0.5.8/hawa/base/db.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.6/hawa/base/init.py` & `HawaData-0.5.8/hawa/base/init.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.6/hawa/common/data.py` & `HawaData-0.5.8/hawa/common/data.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.6/hawa/common/query.py` & `HawaData-0.5.8/hawa/common/query.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.6/hawa/common/utils.py` & `HawaData-0.5.8/hawa/common/utils.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.6/hawa/config.py` & `HawaData-0.5.8/hawa/config.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.6/hawa/data/klass.py` & `HawaData-0.5.8/hawa/data/klass.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.6/hawa/data/school.py` & `HawaData-0.5.8/hawa/data/school.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.6/hawa/paper/health.py` & `HawaData-0.5.8/hawa/paper/health.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """健康测评数据"""
 import itertools
 import json
-import random
 from collections import defaultdict, Counter
 from dataclasses import dataclass, field
 from typing import Union, Set, Optional
 
 import pandas as pd
 from munch import Munch
 from pingouin import cronbach_alpha
@@ -291,15 +290,15 @@
 
             dimensions = self._count_df_reverse(first_col='code', second_col='total', data=base_dimensions)
             fields = self._count_df_reverse(first_col='code', second_col='total', data=base_fields)
             a = base.loc[base.category == 'field', ['F']].mean().mean()
             b = base.loc[base.category == 'field', ['M']].mean().mean()
             records[grade] = {
                 'dimension': dimensions, 'field': fields,
-                'cond': self.count_cond(a, b)
+                'cond': self.count_cond(a, b, target='男生')
             }
         self.grade_code_score = records
 
     def _to_count_n_compare_grade_year_school(self):
         if not self.is_load_last:
             return
         res = defaultdict(dict)
@@ -419,26 +418,26 @@
     def _count_df_reverse(self, first_col: str, second_col: str, data: pd.DataFrame):
         base = data.to_dict(orient='records')
         middle = {d[first_col]: d[second_col] / 100 for d in base}
         reverse_middle = {v: k for k, v in middle.items()}
         res = [(self._retain_prec(k), reverse_middle[k]) for k in sorted(reverse_middle.keys(), reverse=True)]
         return res
 
-    def count_cond(self, a: float, b: float):
+    def count_cond(self, a: float, b: float, target: str = ''):
         if a == b:
-            conditions = '等于'.split()
+            condition = f'等于{target}' if target else '等于'
         elif a - b >= 5:
-            conditions = '明显高于'.split()
+            condition = f'明显高于{target}' if target else '明显高于'
         elif abs(a - b) < 5:
-            conditions = '差异不明显于'.split()
+            condition = f'与{target}的差异不明显' if target else '差异不明显于'
         elif a - b <= -5:
-            conditions = '明显低于'.split()
+            condition = f'明显低于{target}' if target else '明显低于'
         else:
             raise
-        return random.choice(conditions)
+        return condition
 
     def _count_dim_field_diff(self, grade: int, key: str):
         """计算学校与全国对比的维度、领域高低
         :param key: 比较的项：total/M/F
         """
         data = self._build_one_data(grade=grade)
         key_col = f'{key}_y_s'
@@ -477,17 +476,17 @@
 
     def compare_gender_text(self, grade: int):
         grade_rank_dis_m = self.grade_rank_dis[grade].M
         grade_rank_dis_f = self.grade_rank_dis[grade].F
         level_m = round(sum([grade_rank_dis_m['优秀'], grade_rank_dis_m['良好']]), 1)
         level_f = round(sum([grade_rank_dis_f['优秀'], grade_rank_dis_f['良好']]), 1)
         if level_m - level_f >= 5:
-            return '男生明显大于女生'
+            return '男生明显高于女生'
         elif level_m - level_f <= -5:
-            return '男生明显小于女生'
+            return '男生明显低于女生'
         else:
             return '男生与女生不存在明显差异'
 
     def low_high_code_text(self, grade: int, gender: str):
         """相对最高、相对最低文本
         :param grade: total/M/F
         :param gender: total/M/F
@@ -513,15 +512,16 @@
             res += '其余维度和领域没有明显差异。'
         return res
 
     def _build_codes(self, codes: list[str]):
         if len(codes) == 1:
             return f'“{codes[0]}”'
         elif len(codes) > 1:
-            return '、'.join([f'“{i}”' for i in codes[:-1]]) + f'和“{codes[-1]}”'
+            code_text = '、'.join([f'“{i}”' for i in codes[:-1]]) + f'和“{codes[-1]}”'
+            return f"在{code_text}等维度和领域，"
         else:
             return ''
 
     def compare_grade_gen_text(self):
         """生成整体分析标题及一句分析文本。"""
         data = {}
         for grade in self.grade.grades:
@@ -550,27 +550,29 @@
         describe_text = f"{grade_text}{self.meta_unit.short_name}各年级的健康素养水平{cond}{self.last_year_num}年的全国平均水平"
         return title_text, describe_text
 
     def describe_grade_text(self, category: str):
         """描述全年级对比情况
         :param category: total/gender  total：总体比全国 / gender：男生比女生。
         """
-        bigger, smaller = [], []
+        bigger, smaller, others = [], [], []
         for grade in self.grade.grades:
             if category == 'total':
                 first = self.grade_score[grade].avg
                 last_year_grade_data = self.get_last_year_miss(grade=grade)
                 second = last_year_grade_data['score']['total']
             else:
                 first = self.summary_scores[grade]['M']
                 second = self.summary_scores[grade]['F']
             if first - second >= 5:
                 bigger.append(f"{project.grade_simple[grade]}年级")
             elif first - second <= -5:
                 smaller.append(f"{project.grade_simple[grade]}年级")
+            else:
+                others.append(f"{project.grade_simple[grade]}年级")
         res = ''
         if bigger:
             local_codes = self._build_codes(bigger)
             res += f"{self.meta_unit.short_name}{local_codes}分数"
             match category:
                 case 'total':
                     res += '明显高于全国平均分数，'
@@ -581,12 +583,13 @@
             local_codes = self._build_codes(smaller)
             res += f"{self.meta_unit.short_name}{local_codes}分数"
             match category:
                 case 'total':
                     res += "明显低于全国平均分数，"
                 case 'gender':
                     res += "男生明显低于女生，"
-        if (bigger or smaller) and len(bigger) + len(smaller) < len(self.grade.grades):
-            res += '其他年级没有明显差异。'
+        if (bigger or smaller) and ((len(bigger) + len(smaller)) < len(self.grade.grades)):
+            local_codes = self._build_codes(others)
+            res += f'{local_codes}没有明显差异。'
         if not bigger and not smaller:
             res = f'{self.meta_unit.short_name}分数对比无明显差异。'
         return res
```

### Comparing `HawaData-0.5.6/hawa/paper/mht.py` & `HawaData-0.5.8/hawa/paper/mht.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.6/setup.py` & `HawaData-0.5.8/setup.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.6/test/test_query.py` & `HawaData-0.5.8/test/test_query.py`

 * *Files identical despite different names*

