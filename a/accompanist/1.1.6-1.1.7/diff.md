# Comparing `tmp/accompanist-1.1.6-py3-none-any.whl.zip` & `tmp/accompanist-1.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 45294 bytes, number of entries: 22
+Zip file size: 45293 bytes, number of entries: 22
 -rw-r--r--  2.0 unx        0 b- defN 23-May-18 15:07 accompanist/__init__.py
 -rw-r--r--  2.0 unx     1511 b- defN 23-May-20 14:35 accompanist/cmd_init.py
 -rw-r--r--  2.0 unx     6498 b- defN 23-May-24 14:49 accompanist/cmd_listen.py
 -rw-r--r--  2.0 unx     3338 b- defN 23-May-22 09:12 accompanist/cmd_play.py
 -rw-r--r--  2.0 unx      741 b- defN 23-May-18 15:08 accompanist/main.py
 -rw-r--r--  2.0 unx      310 b- defN 23-May-18 14:54 accompanist/utility.py
--rw-r--r--  2.0 unx       18 b- defN 23-May-31 03:59 accompanist/version.py
+-rw-r--r--  2.0 unx       18 b- defN 23-May-31 04:13 accompanist/version.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-18 15:10 accompanist/report/__init__.py
 -rw-r--r--  2.0 unx     4302 b- defN 23-May-20 15:45 accompanist/report/draw_histgram.py
--rw-r--r--  2.0 unx     4529 b- defN 23-May-31 03:57 accompanist/report/draw_pie_chart.py
+-rw-r--r--  2.0 unx     4578 b- defN 23-May-31 04:17 accompanist/report/draw_pie_chart.py
 -rw-r--r--  2.0 unx     3562 b- defN 23-May-20 14:16 accompanist/report/draw_table.py
 -rw-r--r--  2.0 unx     1602 b- defN 23-May-18 16:04 accompanist/report/write_comment.py
 -rw-r--r--  2.0 unx     1503 b- defN 23-May-21 16:45 accompanist/report/write_front_cover.py
 -rw-r--r--  2.0 unx     3645 b- defN 23-May-22 09:43 accompanist/report/write_header_footer.py
 -rw-r--r--  2.0 unx    19193 b- defN 23-Mar-26 08:39 accompanist/resource/logo_trans.png
 -rw-r--r--  2.0 unx     6761 b- defN 23-Mar-26 08:25 accompanist/resource/logo_trans_small.png
--rw-r--r--  2.0 unx     1063 b- defN 23-May-31 04:04 accompanist-1.1.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     6245 b- defN 23-May-31 04:04 accompanist-1.1.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-31 04:04 accompanist-1.1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 23-May-31 04:04 accompanist-1.1.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       31 b- defN 23-May-31 04:04 accompanist-1.1.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1889 b- defN 23-May-31 04:04 accompanist-1.1.6.dist-info/RECORD
-22 files, 66886 bytes uncompressed, 42192 bytes compressed:  36.9%
+-rw-r--r--  2.0 unx     1063 b- defN 23-May-31 04:20 accompanist-1.1.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6225 b- defN 23-May-31 04:20 accompanist-1.1.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-31 04:20 accompanist-1.1.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 23-May-31 04:20 accompanist-1.1.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       31 b- defN 23-May-31 04:20 accompanist-1.1.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1889 b- defN 23-May-31 04:20 accompanist-1.1.7.dist-info/RECORD
+22 files, 66915 bytes uncompressed, 42191 bytes compressed:  36.9%
```

## zipnote {}

```diff
@@ -42,26 +42,26 @@
 
 Filename: accompanist/resource/logo_trans.png
 Comment: 
 
 Filename: accompanist/resource/logo_trans_small.png
 Comment: 
 
-Filename: accompanist-1.1.6.dist-info/LICENSE
+Filename: accompanist-1.1.7.dist-info/LICENSE
 Comment: 
 
-Filename: accompanist-1.1.6.dist-info/METADATA
+Filename: accompanist-1.1.7.dist-info/METADATA
 Comment: 
 
-Filename: accompanist-1.1.6.dist-info/WHEEL
+Filename: accompanist-1.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: accompanist-1.1.6.dist-info/entry_points.txt
+Filename: accompanist-1.1.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: accompanist-1.1.6.dist-info/top_level.txt
+Filename: accompanist-1.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: accompanist-1.1.6.dist-info/RECORD
+Filename: accompanist-1.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## accompanist/version.py

```diff
@@ -1 +1 @@
-VERSION = "1.1.6"
+VERSION = "1.1.7"
```

## accompanist/report/draw_pie_chart.py

```diff
@@ -96,14 +96,17 @@
         masked_ip: str = '.'.join(ip_segments)
         masked_ips.append(masked_ip)
     ip_dataframe.index = [masked_ips[0], masked_ips[1], masked_ips[2],
                           masked_ips[3], masked_ips[4], masked_ips[5]]
     return ip_dataframe
 
 def add_cc_notation(fig_b: Figure) -> None:
+    """
+    Add country code next to IPs
+    """
     fig_b.add_artist(lines.Line2D([0.66, 0.93], [0.16, 0.16], color="#eeeeee", linewidth=60, zorder=0))
     CC_NOTE: str = "Please refer to the following for the country code."
     CC_LINK: str = "https://en.wikipedia.org/wiki/ISO_3166-2"
     fig_b.text(0.64, 0.17, CC_NOTE, fontsize=12, ha="left")
     fig_b.text(0.64, 0.13, CC_LINK, fontsize=12, ha="left", color="blue",
                url="https://en.wikipedia.org/wiki/ISO_3166-2")
```

## Comparing `accompanist-1.1.6.dist-info/LICENSE` & `accompanist-1.1.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `accompanist-1.1.6.dist-info/METADATA` & `accompanist-1.1.7.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: accompanist
-Version: 1.1.6
+Version: 1.1.7
 Summary: Analysis AWS WAF logs and generate a report
 Author: itsuki
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click (>=8.1.3)
 Requires-Dist: boto3 (>=1.26.126)
 Requires-Dist: datetime (>=5.1)
 Requires-Dist: pandas (>=2.0.1)
 Requires-Dist: matplotlib (>=3.7.1)
 Requires-Dist: PdfPages (>=0.1.0)
 
-![logo](./logo.jpg)
 
 [![Python](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-green?style=for-the-badge&logo=appveyor)  ](https://pypi.org/project/accompanist/)  
 
 # Introduction
 ---
 
 ## What is Accomapnist?
```

## Comparing `accompanist-1.1.6.dist-info/RECORD` & `accompanist-1.1.7.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 accompanist/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 accompanist/cmd_init.py,sha256=zil_aW0B6trmh_TYZ777_7hc_3LpIHujqC3c1cfNACU,1511
 accompanist/cmd_listen.py,sha256=LEenowGLgxJpwMkUa95xacCKO5BAylDQkerumTEw5aA,6498
 accompanist/cmd_play.py,sha256=fX_fJZY0wPvpKNL1RXOOW3JIMR37Awjy66d1NhxIFlc,3338
 accompanist/main.py,sha256=g3QBePVSozsf-dpiyjXkUui9gUQHXd0g0znMZQL9TQ4,741
 accompanist/utility.py,sha256=FRzk5G0akYlODVy6RJtbLt6xJRZtdonH2UTh5JLY33I,310
-accompanist/version.py,sha256=GPX0GA6w6CgE_Nlr1lTr6e2UERw45gCZMMp81Vy8dJA,18
+accompanist/version.py,sha256=swSC7Ji8JQdPbrE-3ZFHR4ljb0HO2UsntsDKA7a1Ruc,18
 accompanist/report/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 accompanist/report/draw_histgram.py,sha256=cYxzjROtITo98QL6M8O98EXKlvM78E-WfE9thsPbzEE,4302
-accompanist/report/draw_pie_chart.py,sha256=G7B3mhAMpa1xhrFhanU2_QdXWKKYFPS18fIf6erdAXg,4529
+accompanist/report/draw_pie_chart.py,sha256=74Tml51TqX6A1OMTiUDV5vB0p0gD3ML3ZWTY68GISeU,4578
 accompanist/report/draw_table.py,sha256=YZ9PpGS6sLaEgYsqL2Jj5yR7_ng1ywrLEozSlyfnNGQ,3562
 accompanist/report/write_comment.py,sha256=FqGVuAGRlOQry4ThvoB_I_1NtL1A5MFZMRWTI48nq98,1602
 accompanist/report/write_front_cover.py,sha256=lwRs7u17v7NbuoDVS-9TsH0PX0a1WQk-NEzbK3-ez10,1503
 accompanist/report/write_header_footer.py,sha256=siFZ3JRFwJj3oW7TZEOQJfHI6uSuwLPJfqX5kqjPKGA,3645
 accompanist/resource/logo_trans.png,sha256=IbkfTLMa9qzSifN32YocbOdpDRecelHA7k8cLrBVK_4,19193
 accompanist/resource/logo_trans_small.png,sha256=SS9AlZGL3Ce-6BbD4EW5rbn7zuDcje7HkEXW_lHE2zs,6761
-accompanist-1.1.6.dist-info/LICENSE,sha256=EHImwl3uAjnXzz33MkVgnfcyDByFp0t6O-H4QaGLs4M,1063
-accompanist-1.1.6.dist-info/METADATA,sha256=p1uKGr9wvaexbULnKXdleibPVrPCfKyhqNItBU9tbb0,6245
-accompanist-1.1.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-accompanist-1.1.6.dist-info/entry_points.txt,sha256=gLZwXDl7kf85kYQ1HNQZSxCe81vLub8Eb8wWqrThDeM,53
-accompanist-1.1.6.dist-info/top_level.txt,sha256=vUeFtOUVsBOaqJK8b1z7iVPvaRhz3jGN4Uw79o1o9Ck,31
-accompanist-1.1.6.dist-info/RECORD,,
+accompanist-1.1.7.dist-info/LICENSE,sha256=EHImwl3uAjnXzz33MkVgnfcyDByFp0t6O-H4QaGLs4M,1063
+accompanist-1.1.7.dist-info/METADATA,sha256=4IZLPUWUmvzdLCqHL8bjnwWZx-h7dxvncCG1nR0ehlw,6225
+accompanist-1.1.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+accompanist-1.1.7.dist-info/entry_points.txt,sha256=gLZwXDl7kf85kYQ1HNQZSxCe81vLub8Eb8wWqrThDeM,53
+accompanist-1.1.7.dist-info/top_level.txt,sha256=vUeFtOUVsBOaqJK8b1z7iVPvaRhz3jGN4Uw79o1o9Ck,31
+accompanist-1.1.7.dist-info/RECORD,,
```

