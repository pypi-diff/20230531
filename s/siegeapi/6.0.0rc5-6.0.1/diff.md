# Comparing `tmp/siegeapi-6.0.0rc5.tar.gz` & `tmp/siegeapi-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siegeapi-6.0.0rc5.tar", last modified: Wed Jan  4 23:07:55 2023, max compression
+gzip compressed data, was "siegeapi-6.0.1.tar", last modified: Wed May 31 16:43:12 2023, max compression
```

## Comparing `siegeapi-6.0.0rc5.tar` & `siegeapi-6.0.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-01-04 23:07:55.603810 siegeapi-6.0.0rc5/
--rw-rw-rw-   0        0        0     1088 2022-01-22 13:51:16.000000 siegeapi-6.0.0rc5/LICENSE
--rw-rw-rw-   0        0        0     4263 2023-01-04 23:07:55.603309 siegeapi-6.0.0rc5/PKG-INFO
--rw-rw-rw-   0        0        0     3324 2023-01-04 23:07:12.000000 siegeapi-6.0.0rc5/README.md
--rw-rw-rw-   0        0        0       97 2021-12-02 11:40:13.000000 siegeapi-6.0.0rc5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-04 23:07:55.603810 siegeapi-6.0.0rc5/setup.cfg
--rw-rw-rw-   0        0        0     1229 2023-01-04 23:06:07.000000 siegeapi-6.0.0rc5/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-04 23:07:55.494361 siegeapi-6.0.0rc5/siegeapi/
--rw-rw-rw-   0        0        0       24 2022-04-13 12:58:09.000000 siegeapi-6.0.0rc5/siegeapi/__init__.py
--rw-rw-rw-   0        0        0    12044 2023-01-04 01:18:48.000000 siegeapi-6.0.0rc5/siegeapi/auth.py
-drwxrwxrwx   0        0        0        0 2023-01-04 23:07:55.511885 siegeapi-6.0.0rc5/siegeapi/constants/
--rw-rw-rw-   0        0        0      103 2022-04-13 12:58:09.000000 siegeapi-6.0.0rc5/siegeapi/constants/__init__.py
--rw-rw-rw-   0        0        0    31981 2022-12-07 00:12:44.000000 siegeapi-6.0.0rc5/siegeapi/constants/operators.py
--rw-rw-rw-   0        0        0     9497 2023-01-01 15:53:16.000000 siegeapi-6.0.0rc5/siegeapi/constants/ranks.py
--rw-rw-rw-   0        0        0     4197 2023-01-01 18:57:44.000000 siegeapi-6.0.0rc5/siegeapi/constants/seasons.py
--rw-rw-rw-   0        0        0    23102 2022-08-01 16:12:06.000000 siegeapi-6.0.0rc5/siegeapi/constants/weapons.py
--rw-rw-rw-   0        0        0     2860 2022-06-25 18:50:10.000000 siegeapi-6.0.0rc5/siegeapi/default_stats.py
--rw-rw-rw-   0        0        0      265 2023-01-01 18:09:38.000000 siegeapi-6.0.0rc5/siegeapi/exceptions.py
--rw-rw-rw-   0        0        0     1527 2023-01-01 22:44:20.000000 siegeapi-6.0.0rc5/siegeapi/maps.py
--rw-rw-rw-   0        0        0     2747 2022-12-14 00:11:28.000000 siegeapi-6.0.0rc5/siegeapi/operators.py
--rw-rw-rw-   0        0        0     9893 2023-01-04 22:53:33.000000 siegeapi-6.0.0rc5/siegeapi/player.py
--rw-rw-rw-   0        0        0     1516 2023-01-04 20:19:56.000000 siegeapi-6.0.0rc5/siegeapi/rank_profile.py
--rw-rw-rw-   0        0        0     1880 2023-01-01 15:55:47.000000 siegeapi-6.0.0rc5/siegeapi/ranks.py
--rw-rw-rw-   0        0        0      210 2022-12-13 23:58:32.000000 siegeapi-6.0.0rc5/siegeapi/summaries.py
--rw-rw-rw-   0        0        0     3178 2022-08-31 20:22:36.000000 siegeapi-6.0.0rc5/siegeapi/trends.py
--rw-rw-rw-   0        0        0     4596 2023-01-04 22:23:16.000000 siegeapi-6.0.0rc5/siegeapi/url_builder.py
--rw-rw-rw-   0        0        0     2846 2023-01-04 20:16:36.000000 siegeapi-6.0.0rc5/siegeapi/utils.py
--rw-rw-rw-   0        0        0     3078 2022-08-31 20:18:00.000000 siegeapi-6.0.0rc5/siegeapi/weapons.py
-drwxrwxrwx   0        0        0        0 2023-01-04 23:07:55.508870 siegeapi-6.0.0rc5/siegeapi.egg-info/
--rw-rw-rw-   0        0        0     4263 2023-01-04 23:07:55.000000 siegeapi-6.0.0rc5/siegeapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      642 2023-01-04 23:07:55.000000 siegeapi-6.0.0rc5/siegeapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-04 23:07:55.000000 siegeapi-6.0.0rc5/siegeapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-01-04 23:07:55.000000 siegeapi-6.0.0rc5/siegeapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-01-04 23:07:55.000000 siegeapi-6.0.0rc5/siegeapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 16:43:12.081540 siegeapi-6.0.1/
+-rw-rw-rw-   0        0        0     1088 2022-01-22 13:51:16.000000 siegeapi-6.0.1/LICENSE
+-rw-rw-rw-   0        0        0     4215 2023-05-31 16:43:12.081037 siegeapi-6.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3331 2023-03-10 17:01:21.000000 siegeapi-6.0.1/README.md
+-rw-rw-rw-   0        0        0       97 2021-12-02 11:40:13.000000 siegeapi-6.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-31 16:43:12.081540 siegeapi-6.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1175 2023-05-31 16:42:54.000000 siegeapi-6.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 16:43:12.073536 siegeapi-6.0.1/siegeapi/
+-rw-rw-rw-   0        0        0       24 2022-04-13 12:58:09.000000 siegeapi-6.0.1/siegeapi/__init__.py
+-rw-rw-rw-   0        0        0    12171 2023-04-13 00:49:53.000000 siegeapi-6.0.1/siegeapi/auth.py
+drwxrwxrwx   0        0        0        0 2023-05-31 16:43:12.079537 siegeapi-6.0.1/siegeapi/constants/
+-rw-rw-rw-   0        0        0      103 2022-04-13 12:58:09.000000 siegeapi-6.0.1/siegeapi/constants/__init__.py
+-rw-rw-rw-   0        0        0    32901 2023-05-31 16:26:20.000000 siegeapi-6.0.1/siegeapi/constants/operators.py
+-rw-rw-rw-   0        0        0     9497 2023-01-01 15:53:16.000000 siegeapi-6.0.1/siegeapi/constants/ranks.py
+-rw-rw-rw-   0        0        0     4487 2023-05-31 16:28:59.000000 siegeapi-6.0.1/siegeapi/constants/seasons.py
+-rw-rw-rw-   0        0        0    23102 2022-08-01 16:12:06.000000 siegeapi-6.0.1/siegeapi/constants/weapons.py
+-rw-rw-rw-   0        0        0     2860 2022-06-25 18:50:10.000000 siegeapi-6.0.1/siegeapi/default_stats.py
+-rw-rw-rw-   0        0        0      265 2023-01-01 18:09:38.000000 siegeapi-6.0.1/siegeapi/exceptions.py
+-rw-rw-rw-   0        0        0     1527 2023-01-01 22:44:20.000000 siegeapi-6.0.1/siegeapi/maps.py
+-rw-rw-rw-   0        0        0     2747 2022-12-14 00:11:28.000000 siegeapi-6.0.1/siegeapi/operators.py
+-rw-rw-rw-   0        0        0     9782 2023-03-10 16:55:45.000000 siegeapi-6.0.1/siegeapi/player.py
+-rw-rw-rw-   0        0        0     1516 2023-01-04 20:19:56.000000 siegeapi-6.0.1/siegeapi/rank_profile.py
+-rw-rw-rw-   0        0        0     1880 2023-01-01 15:55:47.000000 siegeapi-6.0.1/siegeapi/ranks.py
+-rw-rw-rw-   0        0        0      210 2022-12-13 23:58:32.000000 siegeapi-6.0.1/siegeapi/summaries.py
+-rw-rw-rw-   0        0        0     3178 2022-08-31 20:22:36.000000 siegeapi-6.0.1/siegeapi/trends.py
+-rw-rw-rw-   0        0        0     4542 2023-03-10 16:55:19.000000 siegeapi-6.0.1/siegeapi/url_builder.py
+-rw-rw-rw-   0        0        0     2602 2023-05-31 16:05:18.000000 siegeapi-6.0.1/siegeapi/utils.py
+-rw-rw-rw-   0        0        0     3078 2022-08-31 20:18:00.000000 siegeapi-6.0.1/siegeapi/weapons.py
+drwxrwxrwx   0        0        0        0 2023-05-31 16:43:12.076537 siegeapi-6.0.1/siegeapi.egg-info/
+-rw-rw-rw-   0        0        0     4215 2023-05-31 16:43:11.000000 siegeapi-6.0.1/siegeapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      642 2023-05-31 16:43:11.000000 siegeapi-6.0.1/siegeapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 16:43:11.000000 siegeapi-6.0.1/siegeapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-05-31 16:43:11.000000 siegeapi-6.0.1/siegeapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-31 16:43:11.000000 siegeapi-6.0.1/siegeapi.egg-info/top_level.txt
```

### Comparing `siegeapi-6.0.0rc5/LICENSE` & `siegeapi-6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `siegeapi-6.0.0rc5/PKG-INFO` & `siegeapi-6.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: siegeapi
-Version: 6.0.0rc5
+Version: 6.0.1
 Summary: Rainbow Six Siege API interface
 Home-page: https://github.com/CNDRD/siege-api
 Author: CNDRD
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
@@ -65,36 +64,36 @@
     await player.load_ranked_v2()
     print(f"Ranked Points: {player.ranked_profile.rank_points}")
     print(f"Rank: {player.ranked_profile.rank}")
     print(f"Max Rank Points: {player.ranked_profile.max_rank_points}")
     print(f"Max Rank: {player.ranked_profile.max_rank}")
 
     await player.load_progress()
-    print(f"XP: {player.xp}")
-    print(f"Total XP: {player.total_xp}")
-    print(f"XP to level up: {player.xp_to_level_up}")
+    print(f"XP: {player.xp:,}")
+    print(f"Total XP: {player.total_xp:,}")
+    print(f"XP to level up: {player.xp_to_level_up:,}")
     
     await auth.close()
 
 asyncio.get_event_loop().run_until_complete(sample())
 # Or `asyncio.run(sample())`  
 ```
 ### Output  
 ```text
 Name: CNDRD
 Profile pic URL: https://ubisoft-avatars.akamaized.net/7e0f63df-a39b-44c5-8de0-d39a05926e77/default_256_256.png
-Total Time Played: 7,634,850 seconds
-Level: 280
-Ranked Points: 3528
-Rank: Emerald 5
-Max Rank Points: 3694
-Max Rank: Emerald 4
-XP: 14174
-Total XP: 17271674
-XP to level up: 116826
+Total Time Played: 7,910,265 seconds
+Level: 285
+Ranked Points: 1000
+Rank: Unranked
+Max Rank Points: 1000
+Max Rank: Unranked
+XP: 56,362
+Total XP: 17,973,862
+XP to level up: 77,138
 ```
 
 ---  
 
 ## Siege Inventory  
 If you want to see every skin, headgear, uniform and more, head over to **[skins.cndrd.xyz](https://skins.cndrd.xyz/)**
```

#### html2text {}

```diff
@@ -1,20 +1,19 @@
-Metadata-Version: 2.1 Name: siegeapi Version: 6.0.0rc5 Summary: Rainbow Six
-Siege API interface Home-page: https://github.com/CNDRD/siege-api Author: CNDRD
+Metadata-Version: 2.1 Name: siegeapi Version: 6.0.1 Summary: Rainbow Six Siege
+API interface Home-page: https://github.com/CNDRD/siege-api Author: CNDRD
 License: MIT Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License Classifier: Intended
 Audience :: Developers Classifier: Natural Language :: English Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
-:: 3.11 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Topic :: Internet Classifier: Topic :: Software
-Development :: Libraries Classifier: Topic :: Software Development :: Libraries
-:: Python Modules Classifier: Topic :: Utilities Classifier: Typing :: Typed
-Requires-Python: >=3.8.0 Description-Content-Type: text/markdown License-File:
-LICENSE
+:: 3.10 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Topic :: Internet Classifier:
+Topic :: Software Development :: Libraries Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Classifier: Topic :: Utilities
+Classifier: Typing :: Typed Requires-Python: >=3.8.0 Description-Content-Type:
+text/markdown License-File: LICENSE
    [https://raw.githubusercontent.com/CNDRD/siegeapi/master/assets/siegeapi-
                                   banner.png]
                             ****** siegeapi ******
                 [https://img.shields.io/github/v/release/CNDRD/
                 siegeapi?label=latest%20release&style=for-the-
       badge&logo=github&logoColor=white] [https://img.shields.io/pypi/v/
            siegeapi?style=for-the-badge&logo=pypi&logoColor=white]
@@ -28,22 +27,22 @@
 URL: {player.profile_pic_url}") await player.load_playtime() print(f"Total Time
 Played: {player.total_time_played:,} seconds") print(f"Level: {player.level}")
 await player.load_ranked_v2() print(f"Ranked Points:
 {player.ranked_profile.rank_points}") print(f"Rank:
 {player.ranked_profile.rank}") print(f"Max Rank Points:
 {player.ranked_profile.max_rank_points}") print(f"Max Rank:
 {player.ranked_profile.max_rank}") await player.load_progress() print(f"XP:
-{player.xp}") print(f"Total XP: {player.total_xp}") print(f"XP to level up:
-{player.xp_to_level_up}") await auth.close() asyncio.get_event_loop
+{player.xp:,}") print(f"Total XP: {player.total_xp:,}") print(f"XP to level up:
+{player.xp_to_level_up:,}") await auth.close() asyncio.get_event_loop
 ().run_until_complete(sample()) # Or `asyncio.run(sample())` ``` ### Output
 ```text Name: CNDRD Profile pic URL: https://ubisoft-avatars.akamaized.net/
 7e0f63df-a39b-44c5-8de0-d39a05926e77/default_256_256.png Total Time Played:
-7,634,850 seconds Level: 280 Ranked Points: 3528 Rank: Emerald 5 Max Rank
-Points: 3694 Max Rank: Emerald 4 XP: 14174 Total XP: 17271674 XP to level up:
-116826 ``` --- ## Siege Inventory If you want to see every skin, headgear,
+7,910,265 seconds Level: 285 Ranked Points: 1000 Rank: Unranked Max Rank
+Points: 1000 Max Rank: Unranked XP: 56,362 Total XP: 17,973,862 XP to level up:
+77,138 ``` --- ## Siege Inventory If you want to see every skin, headgear,
 uniform and more, head over to **[skins.cndrd.xyz](https://skins.cndrd.xyz/)**
 ## Docs For docs go to [cndrd.github.io/siegeapi](https://cndrd.github.io/
 siegeapi/) ## Credits Operator Icons from [r6operators][r6operators_] by
 [marcopixel][marcopixel_] Built (and re-built) on top of what [billy-yoyo]
 [r6s_python_api] started ## Problems If you experience any problems, reach out
 to me, or submit a PR You can reach out here on GitHub or on Discord
 (_CNDRD#2233_) ![forthebadge](https://forthebadge.com/images/badges/works-on-
```

### Comparing `siegeapi-6.0.0rc5/README.md` & `siegeapi-6.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -40,36 +40,36 @@
     await player.load_ranked_v2()
     print(f"Ranked Points: {player.ranked_profile.rank_points}")
     print(f"Rank: {player.ranked_profile.rank}")
     print(f"Max Rank Points: {player.ranked_profile.max_rank_points}")
     print(f"Max Rank: {player.ranked_profile.max_rank}")
 
     await player.load_progress()
-    print(f"XP: {player.xp}")
-    print(f"Total XP: {player.total_xp}")
-    print(f"XP to level up: {player.xp_to_level_up}")
+    print(f"XP: {player.xp:,}")
+    print(f"Total XP: {player.total_xp:,}")
+    print(f"XP to level up: {player.xp_to_level_up:,}")
     
     await auth.close()
 
 asyncio.get_event_loop().run_until_complete(sample())
 # Or `asyncio.run(sample())`  
 ```
 ### Output  
 ```text
 Name: CNDRD
 Profile pic URL: https://ubisoft-avatars.akamaized.net/7e0f63df-a39b-44c5-8de0-d39a05926e77/default_256_256.png
-Total Time Played: 7,634,850 seconds
-Level: 280
-Ranked Points: 3528
-Rank: Emerald 5
-Max Rank Points: 3694
-Max Rank: Emerald 4
-XP: 14174
-Total XP: 17271674
-XP to level up: 116826
+Total Time Played: 7,910,265 seconds
+Level: 285
+Ranked Points: 1000
+Rank: Unranked
+Max Rank Points: 1000
+Max Rank: Unranked
+XP: 56,362
+Total XP: 17,973,862
+XP to level up: 77,138
 ```
 
 ---  
 
 ## Siege Inventory  
 If you want to see every skin, headgear, uniform and more, head over to **[skins.cndrd.xyz](https://skins.cndrd.xyz/)**
```

#### html2text {}

```diff
@@ -15,22 +15,22 @@
 URL: {player.profile_pic_url}") await player.load_playtime() print(f"Total Time
 Played: {player.total_time_played:,} seconds") print(f"Level: {player.level}")
 await player.load_ranked_v2() print(f"Ranked Points:
 {player.ranked_profile.rank_points}") print(f"Rank:
 {player.ranked_profile.rank}") print(f"Max Rank Points:
 {player.ranked_profile.max_rank_points}") print(f"Max Rank:
 {player.ranked_profile.max_rank}") await player.load_progress() print(f"XP:
-{player.xp}") print(f"Total XP: {player.total_xp}") print(f"XP to level up:
-{player.xp_to_level_up}") await auth.close() asyncio.get_event_loop
+{player.xp:,}") print(f"Total XP: {player.total_xp:,}") print(f"XP to level up:
+{player.xp_to_level_up:,}") await auth.close() asyncio.get_event_loop
 ().run_until_complete(sample()) # Or `asyncio.run(sample())` ``` ### Output
 ```text Name: CNDRD Profile pic URL: https://ubisoft-avatars.akamaized.net/
 7e0f63df-a39b-44c5-8de0-d39a05926e77/default_256_256.png Total Time Played:
-7,634,850 seconds Level: 280 Ranked Points: 3528 Rank: Emerald 5 Max Rank
-Points: 3694 Max Rank: Emerald 4 XP: 14174 Total XP: 17271674 XP to level up:
-116826 ``` --- ## Siege Inventory If you want to see every skin, headgear,
+7,910,265 seconds Level: 285 Ranked Points: 1000 Rank: Unranked Max Rank
+Points: 1000 Max Rank: Unranked XP: 56,362 Total XP: 17,973,862 XP to level up:
+77,138 ``` --- ## Siege Inventory If you want to see every skin, headgear,
 uniform and more, head over to **[skins.cndrd.xyz](https://skins.cndrd.xyz/)**
 ## Docs For docs go to [cndrd.github.io/siegeapi](https://cndrd.github.io/
 siegeapi/) ## Credits Operator Icons from [r6operators][r6operators_] by
 [marcopixel][marcopixel_] Built (and re-built) on top of what [billy-yoyo]
 [r6s_python_api] started ## Problems If you experience any problems, reach out
 to me, or submit a PR You can reach out here on GitHub or on Discord
 (_CNDRD#2233_) ![forthebadge](https://forthebadge.com/images/badges/works-on-
```

### Comparing `siegeapi-6.0.0rc5/setup.py` & `siegeapi-6.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name="siegeapi",
-    version="6.0.0rc5",
+    version="6.0.1",
     url="https://github.com/CNDRD/siege-api",
     description="Rainbow Six Siege API interface",
     author="CNDRD",
     packages=find_packages(),
     license="MIT",
     include_package_data=True,
     install_requires=["aiohttp>=3.6.0,<3.8.0"],
@@ -18,15 +18,14 @@
     long_description_content_type='text/markdown',
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: MIT License",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.8",
         "Topic :: Internet",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Utilities",
```

### Comparing `siegeapi-6.0.0rc5/siegeapi/auth.py` & `siegeapi-6.0.1/siegeapi/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,14 +110,17 @@
         """ Retrieves the current session, ensuring it's valid first """
         await self._ensure_session_valid()
         return self.session
 
     def save_creds(self) -> None:
         """ Saves the credentials to a file """
 
+        if not os.path.exists(os.path.dirname(self.creds_path)):
+            os.makedirs(os.path.dirname(self.creds_path))
+
         if not os.path.exists(self.creds_path):
             with open(self.creds_path, 'w') as f:
                 json.dump({}, f)
 
         # write to file, overwriting the old one
         with open(self.creds_path, 'w') as f:
             json.dump({
```

### Comparing `siegeapi-6.0.0rc5/siegeapi/constants/operators.py` & `siegeapi-6.0.1/siegeapi/constants/operators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,40 @@
 operator_dict = {
+   "fenrir": {
+      "name": "Fenrir",
+      "safename": "fenrir",
+      "realname": "Emil Svensson",
+      "birthplace": "Uppsala, Sweden",
+      "age": 34,
+      "date_of_birth": "December 3rd",
+      "season_introduced": "Y8S2",
+      "health": 2,
+      "speed": 2,
+      "unit": "Redhammer",
+      "country_code": "SE",
+      "roles": ["Trapper"],
+      "side": "defender",
+      "icon_url": "https://i.imgur.com/6T16oPJ.png",
+   },
+   "brava": {
+      "name": "Brava",
+      "safename": "brava",
+      "realname": "Nayara Cardoso",
+      "birthplace": "Curitiba, Brazil",
+      "age": 40,
+      "date_of_birth": "January 10th",
+      "season_introduced": "Y8S1",
+      "health": 1,
+      "speed": 3,
+      "unit": "Viperstrike",
+      "country_code": "BR",
+      "roles": ["Intel", "Anti Gadget"],
+      "side": "attacker",
+      "icon_url": "https://i.imgur.com/1Se82ke.png",
+   },
    "solis": {
       "name": "Solis",
       "safename": "solis",
       "realname": "Ana Valentina Díaz",
       "birthplace": "Zipaquirá, Colombia",
       "age": 37,
       "date_of_birth": "September 18th",
@@ -35,16 +67,16 @@
       "name": "Sens",
       "safename": "sens",
       "realname": "Néon Ngoma Mutombo",
       "birthplace": "Brussels, Belgium",
       "age": 30,
       "date_of_birth": "March 3rd",
       "season_introduced": "Y7S2",
-      "health": 3,
-      "speed": 1,
+      "health": 1,
+      "speed": 3,
       "unit": "SFG",
       "country_code": "BE",
       "roles": ["Covering Fire", "Area Denial", "Crowd Control"],
       "side": "attacker",
       "icon_url": "https://i.imgur.com/kwfMIVz.png",
    },
    "azami": {
@@ -83,32 +115,32 @@
       "name": "Osa",
       "safename": "osa",
       "realname": "Anja Katarina Janković",
       "birthplace": "Split, Croatia",
       "age": 27,
       "date_of_birth": "April 29th",
       "season_introduced": "Y6S3",
-      "health": 2,
-      "speed": 2,
+      "health": 3,
+      "speed": 1,
       "unit": "NIGHTHAVEN",
       "country_code": "HR",
       "roles": ["Intel Gatherer", "Area Denial", "Anti Roam"],
       "side": "attacker",
       "icon_url": "https://i.imgur.com/odZHbem.png",
    },
    "thunderbird": {
       "name": "Thunderbird",
       "safename": "thunderbird",
       "realname": "Mina Sky",
       "birthplace": "Nakoda Territories",
       "age": 36,
       "date_of_birth": "April 1st",
       "season_introduced": "Y6S2",
-      "health": 1,
-      "speed": 3,
+      "health": 2,
+      "speed": 2,
       "unit": "UNAFFILIATED",
       "country_code": "",
       "roles": ["Secure", "Roam", "Buff"],
       "side": "defender",
       "icon_url": "https://i.imgur.com/21vn9y7.png",
    },
    "flores": {
@@ -131,32 +163,32 @@
       "name": "Aruni",
       "safename": "aruni",
       "realname": "Apha Tawanroong",
       "birthplace": "Ta Phraya District, Thailand",
       "age": 42,
       "date_of_birth": "August 9th",
       "season_introduced": "Y5S4",
-      "health": 2,
-      "speed": 2,
+      "health": 3,
+      "speed": 1,
       "unit": "NIGHTHAVEN",
       "country_code": "TH",
       "roles": ["Secure", "Intel Gatherer", "Anchor"],
       "side": "defender",
       "icon_url": "https://i.imgur.com/PhCM38D.png",
    },
    "zero": {
       "name": "Zero",
       "safename": "zero",
       "realname": "Samuel Leo Fisher",
       "birthplace": "Baltimore, Maryland",
       "age": 63,
       "date_of_birth": "August 8th",
       "season_introduced": "Y5S3",
-      "health": 2,
-      "speed": 2,
+      "health": 1,
+      "speed": 3,
       "unit": "ROS",
       "country_code": "US",
       "roles": ["Intel Denier", "Intel Gatherer"],
       "side": "attacker",
       "icon_url": "https://i.imgur.com/87LCqv1.png",
    },
    "ace": {
@@ -179,16 +211,16 @@
       "name": "Melusi",
       "safename": "melusi",
       "realname": "Thandiwe Ndlovu",
       "birthplace": "Louwsburg, South Africa",
       "age": 32,
       "date_of_birth": "June 16th",
       "season_introduced": "Y5S2",
-      "health": 1,
-      "speed": 3,
+      "health": 3,
+      "speed": 1,
       "unit": "ITF",
       "country_code": "SA",
       "roles": ["Crowd Control", "Intel Gatherer", "Secure"],
       "side": "defender",
       "icon_url": "https://i.imgur.com/7BNXQnr.png",
    },
    "oryx": {
@@ -499,48 +531,48 @@
       "name": "Dokkaebi",
       "safename": "dokkaebi",
       "realname": "Grace Nam",
       "birthplace": "Seoul, South Korea",
       "age": 29,
       "date_of_birth": "February 2nd",
       "season_introduced": "Y2S4",
-      "health": 2,
-      "speed": 2,
+      "health": 1,
+      "speed": 3,
       "unit": "707TH SMB",
       "country_code": "SK",
       "roles": ["Anti Roam", "Flank", "Intel Denier", "Intel Gatherer"],
       "side": "attacker",
       "icon_url": "https://i.imgur.com/iVLOHr2.png",
    },
    "zofia": {
       "name": "Zofia",
       "safename": "zofia",
       "realname": "Zofia Bosak",
       "birthplace": "Wrocław, Poland",
       "age": 36,
       "date_of_birth": "January 28th",
       "season_introduced": "Y2S4",
-      "health": 2,
-      "speed": 2,
+      "health": 3,
+      "speed": 1,
       "unit": "G.R.O.",
       "country_code": "PL",
       "roles": ["Anti Roam", "Crowd Control", "Disable", "Flank", "Soft Breach"],
       "side": "attacker",
       "icon_url": "https://i.imgur.com/AMOYwMJ.png",
    },
    "ela": {
       "name": "Ela",
       "safename": "ela",
       "realname": "Elżbieta Bosak",
       "birthplace": "Wrocław, Poland",
       "age": 31,
       "date_of_birth": "November 8th",
       "season_introduced": "Y2S4",
-      "health": 1,
-      "speed": 3,
+      "health": 2,
+      "speed": 2,
       "unit": "G.R.O.",
       "country_code": "PL",
       "roles": ["Crowd Control", "Roam", "Trap"],
       "side": "defender",
       "icon_url": "https://i.imgur.com/OwjSJNB.png",
    },
    "ying": {
@@ -627,16 +659,16 @@
       "name": "Echo",
       "safename": "echo",
       "realname": "Masaru Enatsu",
       "birthplace": "Tokyo, Japan (Suginami-ku)",
       "age": 36,
       "date_of_birth": "October 31st",
       "season_introduced": "Y1S4",
-      "health": 3,
-      "speed": 1,
+      "health": 2,
+      "speed": 2,
       "unit": "S.A.T.",
       "country_code": "JP",
       "roles": ["Anchor", "Crowd Control", "Intel Gatherer", "Secure"],
       "side": "defender",
       "icon_url": "https://i.imgur.com/OMNe9qB.png",
    },
    "caveira": {
@@ -739,32 +771,32 @@
       "name": "Mute",
       "safename": "mute",
       "realname": "Mark R. Chandar",
       "birthplace": "York, England",
       "age": 25,
       "date_of_birth": "October 11th",
       "season_introduced": "Y0S0",
-      "health": 2,
-      "speed": 2,
+      "health": 3,
+      "speed": 1,
       "unit": "SAS",
       "country_code": "GB",
       "roles": ["Anti Hard Breach", "Intel Denier", "Secure"],
       "side": "defender",
       "icon_url": "https://i.imgur.com/peaKoO1.png",
    },
    "sledge": {
       "name": "Sledge",
       "safename": "sledge",
       "realname": "Seamus Cowden",
       "birthplace": "John O’Groats, Scotland",
       "age": 35,
       "date_of_birth": "April 2nd",
       "season_introduced": "Y0S0",
-      "health": 2,
-      "speed": 2,
+      "health": 3,
+      "speed": 1,
       "unit": "SAS",
       "country_code": "GB",
       "roles": ["Flank", "Soft Breach"],
       "side": "attacker",
       "icon_url": "https://i.imgur.com/JXV80ZY.png",
    },
    "smoke": {
@@ -787,16 +819,16 @@
       "name": "Thatcher",
       "safename": "thatcher",
       "realname": "Mike Baker",
       "birthplace": "Bideford, England",
       "age": 56,
       "date_of_birth": "June 22nd",
       "season_introduced": "Y0S0",
-      "health": 2,
-      "speed": 2,
+      "health": 3,
+      "speed": 1,
       "unit": "SAS",
       "country_code": "GB",
       "roles": ["Back Line", "Disable"],
       "side": "attacker",
       "icon_url": "https://i.imgur.com/BuEp8mz.png",
    },
    "ash": {
```

### Comparing `siegeapi-6.0.0rc5/siegeapi/constants/ranks.py` & `siegeapi-6.0.1/siegeapi/constants/ranks.py`

 * *Files identical despite different names*

### Comparing `siegeapi-6.0.0rc5/siegeapi/constants/seasons.py` & `siegeapi-6.0.1/siegeapi/constants/seasons.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,9 +192,24 @@
         "start_date": "2022-09-14"
     },
     28: {
         "name": "Solar Raid",
         "hex": "#d03314",
         "code": "Y7S4",
         "start_date": "2022-12-07"
+    },
+
+
+
+    29: {
+        "name": "Commanding Force",
+        "hex": "#45abf3",
+        "code": "Y8S1",
+        "start_date": "2023-03-07"
+    },
+    30: {
+        "name": "Dread Factor",
+        "hex": "#6432ef",
+        "code": "Y8S2",
+        "start_date": "2023-30-05"
     }
 }
```

### Comparing `siegeapi-6.0.0rc5/siegeapi/constants/weapons.py` & `siegeapi-6.0.1/siegeapi/constants/weapons.py`

 * *Files identical despite different names*

### Comparing `siegeapi-6.0.0rc5/siegeapi/default_stats.py` & `siegeapi-6.0.1/siegeapi/default_stats.py`

 * *Files identical despite different names*

### Comparing `siegeapi-6.0.0rc5/siegeapi/maps.py` & `siegeapi-6.0.1/siegeapi/maps.py`

 * *Files identical despite different names*

### Comparing `siegeapi-6.0.0rc5/siegeapi/operators.py` & `siegeapi-6.0.1/siegeapi/operators.py`

 * *Files identical despite different names*

### Comparing `siegeapi-6.0.0rc5/siegeapi/player.py` & `siegeapi-6.0.1/siegeapi/player.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,19 +119,18 @@
                         self.rank_skill_records.setdefault(season_id, {})
                         self.rank_skill_records[season_id]["global"] = rank_obj if played else None
                         self.rank_skill_records[season_id][region_id] = rank_obj if played else None
                     elif board_id == "pvp_casual":
                         self.casual_skill_records.setdefault(season_id, {})
                         self.casual_skill_records[season_id][region_id] = rank_obj if played else None
 
-    async def load_summaries(self, gamemodes: list[str] = None, team_roles: list[str] = None, seasons: list[str] = None) -> None:
+    async def load_summaries(self, gamemodes: list[str] = None, team_roles: list[str] = None) -> None:
         gamemodes = ",".join(gamemodes) if gamemodes else "all,ranked,unranked,casual"
         team_roles = ",".join(team_roles) if team_roles else "all,Attacker,Defender"
-        seasons = ",".join(seasons) if seasons else season_id_to_code(-1)
-        data = await self._auth.get(self._url_builder.seasonal_summaries(gamemodes, team_roles, seasons))
+        data = await self._auth.get(self._url_builder.seasonal_summaries(gamemodes, team_roles))
 
         data_gamemodes = data.get('profileData').get(self.id).get("platforms").get(self._platform_group).get("gameModes")
 
         for gamemode in data_gamemodes:
             roles = data_gamemodes[gamemode]['teamRoles']
 
             for role in roles:
```

### Comparing `siegeapi-6.0.0rc5/siegeapi/rank_profile.py` & `siegeapi-6.0.1/siegeapi/rank_profile.py`

 * *Files identical despite different names*

### Comparing `siegeapi-6.0.0rc5/siegeapi/ranks.py` & `siegeapi-6.0.1/siegeapi/ranks.py`

 * *Files identical despite different names*

### Comparing `siegeapi-6.0.0rc5/siegeapi/trends.py` & `siegeapi-6.0.1/siegeapi/trends.py`

 * *Files identical despite different names*

### Comparing `siegeapi-6.0.0rc5/siegeapi/url_builder.py` & `siegeapi-6.0.1/siegeapi/url_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,21 +80,20 @@
                f"&aggregation=maps" \
                f"&gameMode=all,ranked,casual,unranked" \
                f"&platformGroup=PC" \
                f"&teamRole=all,Attacker,Defender" \
                f"{self.start_date}" \
                f"{self.end_date}"
 
-    def seasonal_summaries(self, gamemodes: str, team_roles: str, seasons: str) -> str:
+    def seasonal_summaries(self, gamemodes: str, team_roles: str) -> str:
         return f"https://prod.datadev.ubisoft.com/v1/users/{self.player_id}/playerstats?" \
                f"spaceId={self.spaceid}" \
                f"&view=seasonal" \
                f"&aggregation=summary" \
                f"&gameMode={gamemodes}" \
                f"&platformGroup={self.platform_group}" \
-               f"&teamRole={team_roles}" \
-               f"&seasons={seasons}"
+               f"&teamRole={team_roles}"
 
     def full_profiles(self) -> str:
         return f"https://public-ubiservices.ubi.com/v2/spaces/0d2ae42d-4c27-4cb7-af6c-2099062302bb/title/r6s/skill/full_profiles?" \
                f"profile_ids={self.player_id}" \
                f"&platform_families={self.platform_group.lower()}"
```

### Comparing `siegeapi-6.0.0rc5/siegeapi/utils.py` & `siegeapi-6.0.1/siegeapi/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,21 +44,17 @@
     total = 0
     for level in range(1, lvl):
         total += get_xp_to_next_lvl(level)
     return total + current_xp
 
 
 def season_id_to_code(season_id: int) -> str:
-    """Depends on 'seasons_const' always being up-to-date.."""
     seasons_count = len(seasons_const) - 3
     season_id = seasons_count - season_id if season_id < 0 else season_id
 
-    if 0 <= season_id < 6 or season_id > seasons_count+1:
-        raise InvalidAttributeCombination(f"Season ID must be between than 6 and {seasons_count+1}, got {season_id}")
-
     return seasons_const.get(season_id, {}).get("code")
 
 
 def season_code_to_id(season_code: str) -> int:
     """Depends on 'seasons_const' always being up-to-date.."""
     seasons_count = len(seasons_const) - 3
     season_id = next((k for k, v in seasons_const.items() if v["code"] == season_code), None)
```

### Comparing `siegeapi-6.0.0rc5/siegeapi/weapons.py` & `siegeapi-6.0.1/siegeapi/weapons.py`

 * *Files identical despite different names*

### Comparing `siegeapi-6.0.0rc5/siegeapi.egg-info/PKG-INFO` & `siegeapi-6.0.1/siegeapi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: siegeapi
-Version: 6.0.0rc5
+Version: 6.0.1
 Summary: Rainbow Six Siege API interface
 Home-page: https://github.com/CNDRD/siege-api
 Author: CNDRD
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
@@ -65,36 +64,36 @@
     await player.load_ranked_v2()
     print(f"Ranked Points: {player.ranked_profile.rank_points}")
     print(f"Rank: {player.ranked_profile.rank}")
     print(f"Max Rank Points: {player.ranked_profile.max_rank_points}")
     print(f"Max Rank: {player.ranked_profile.max_rank}")
 
     await player.load_progress()
-    print(f"XP: {player.xp}")
-    print(f"Total XP: {player.total_xp}")
-    print(f"XP to level up: {player.xp_to_level_up}")
+    print(f"XP: {player.xp:,}")
+    print(f"Total XP: {player.total_xp:,}")
+    print(f"XP to level up: {player.xp_to_level_up:,}")
     
     await auth.close()
 
 asyncio.get_event_loop().run_until_complete(sample())
 # Or `asyncio.run(sample())`  
 ```
 ### Output  
 ```text
 Name: CNDRD
 Profile pic URL: https://ubisoft-avatars.akamaized.net/7e0f63df-a39b-44c5-8de0-d39a05926e77/default_256_256.png
-Total Time Played: 7,634,850 seconds
-Level: 280
-Ranked Points: 3528
-Rank: Emerald 5
-Max Rank Points: 3694
-Max Rank: Emerald 4
-XP: 14174
-Total XP: 17271674
-XP to level up: 116826
+Total Time Played: 7,910,265 seconds
+Level: 285
+Ranked Points: 1000
+Rank: Unranked
+Max Rank Points: 1000
+Max Rank: Unranked
+XP: 56,362
+Total XP: 17,973,862
+XP to level up: 77,138
 ```
 
 ---  
 
 ## Siege Inventory  
 If you want to see every skin, headgear, uniform and more, head over to **[skins.cndrd.xyz](https://skins.cndrd.xyz/)**
```

#### html2text {}

```diff
@@ -1,20 +1,19 @@
-Metadata-Version: 2.1 Name: siegeapi Version: 6.0.0rc5 Summary: Rainbow Six
-Siege API interface Home-page: https://github.com/CNDRD/siege-api Author: CNDRD
+Metadata-Version: 2.1 Name: siegeapi Version: 6.0.1 Summary: Rainbow Six Siege
+API interface Home-page: https://github.com/CNDRD/siege-api Author: CNDRD
 License: MIT Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License Classifier: Intended
 Audience :: Developers Classifier: Natural Language :: English Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
-:: 3.11 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Topic :: Internet Classifier: Topic :: Software
-Development :: Libraries Classifier: Topic :: Software Development :: Libraries
-:: Python Modules Classifier: Topic :: Utilities Classifier: Typing :: Typed
-Requires-Python: >=3.8.0 Description-Content-Type: text/markdown License-File:
-LICENSE
+:: 3.10 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Topic :: Internet Classifier:
+Topic :: Software Development :: Libraries Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Classifier: Topic :: Utilities
+Classifier: Typing :: Typed Requires-Python: >=3.8.0 Description-Content-Type:
+text/markdown License-File: LICENSE
    [https://raw.githubusercontent.com/CNDRD/siegeapi/master/assets/siegeapi-
                                   banner.png]
                             ****** siegeapi ******
                 [https://img.shields.io/github/v/release/CNDRD/
                 siegeapi?label=latest%20release&style=for-the-
       badge&logo=github&logoColor=white] [https://img.shields.io/pypi/v/
            siegeapi?style=for-the-badge&logo=pypi&logoColor=white]
@@ -28,22 +27,22 @@
 URL: {player.profile_pic_url}") await player.load_playtime() print(f"Total Time
 Played: {player.total_time_played:,} seconds") print(f"Level: {player.level}")
 await player.load_ranked_v2() print(f"Ranked Points:
 {player.ranked_profile.rank_points}") print(f"Rank:
 {player.ranked_profile.rank}") print(f"Max Rank Points:
 {player.ranked_profile.max_rank_points}") print(f"Max Rank:
 {player.ranked_profile.max_rank}") await player.load_progress() print(f"XP:
-{player.xp}") print(f"Total XP: {player.total_xp}") print(f"XP to level up:
-{player.xp_to_level_up}") await auth.close() asyncio.get_event_loop
+{player.xp:,}") print(f"Total XP: {player.total_xp:,}") print(f"XP to level up:
+{player.xp_to_level_up:,}") await auth.close() asyncio.get_event_loop
 ().run_until_complete(sample()) # Or `asyncio.run(sample())` ``` ### Output
 ```text Name: CNDRD Profile pic URL: https://ubisoft-avatars.akamaized.net/
 7e0f63df-a39b-44c5-8de0-d39a05926e77/default_256_256.png Total Time Played:
-7,634,850 seconds Level: 280 Ranked Points: 3528 Rank: Emerald 5 Max Rank
-Points: 3694 Max Rank: Emerald 4 XP: 14174 Total XP: 17271674 XP to level up:
-116826 ``` --- ## Siege Inventory If you want to see every skin, headgear,
+7,910,265 seconds Level: 285 Ranked Points: 1000 Rank: Unranked Max Rank
+Points: 1000 Max Rank: Unranked XP: 56,362 Total XP: 17,973,862 XP to level up:
+77,138 ``` --- ## Siege Inventory If you want to see every skin, headgear,
 uniform and more, head over to **[skins.cndrd.xyz](https://skins.cndrd.xyz/)**
 ## Docs For docs go to [cndrd.github.io/siegeapi](https://cndrd.github.io/
 siegeapi/) ## Credits Operator Icons from [r6operators][r6operators_] by
 [marcopixel][marcopixel_] Built (and re-built) on top of what [billy-yoyo]
 [r6s_python_api] started ## Problems If you experience any problems, reach out
 to me, or submit a PR You can reach out here on GitHub or on Discord
 (_CNDRD#2233_) ![forthebadge](https://forthebadge.com/images/badges/works-on-
```

### Comparing `siegeapi-6.0.0rc5/siegeapi.egg-info/SOURCES.txt` & `siegeapi-6.0.1/siegeapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

