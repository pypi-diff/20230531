# Comparing `tmp/hoyo-daily-logins-helper-2.4.2.tar.gz` & `tmp/hoyo-daily-logins-helper-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoyo-daily-logins-helper-2.4.2.tar", last modified: Wed May 17 08:17:33 2023, max compression
+gzip compressed data, was "hoyo-daily-logins-helper-2.5.0.tar", last modified: Wed May 31 07:40:55 2023, max compression
```

## Comparing `hoyo-daily-logins-helper-2.4.2.tar` & `hoyo-daily-logins-helper-2.5.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:17:33.099995 hoyo-daily-logins-helper-2.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-17 08:17:10.000000 hoyo-daily-logins-helper-2.4.2/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:17:33.095995 hoyo-daily-logins-helper-2.4.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:17:33.099995 hoyo-daily-logins-helper-2.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-17 08:17:10.000000 hoyo-daily-logins-helper-2.4.2/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-17 08:17:10.000000 hoyo-daily-logins-helper-2.4.2/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-05-17 08:17:10.000000 hoyo-daily-logins-helper-2.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-17 08:17:10.000000 hoyo-daily-logins-helper-2.4.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    34227 2023-05-17 08:17:10.000000 hoyo-daily-logins-helper-2.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-17 08:17:10.000000 hoyo-daily-logins-helper-2.4.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-05-17 08:17:33.099995 hoyo-daily-logins-helper-2.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-05-17 08:17:10.000000 hoyo-daily-logins-helper-2.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-17 08:17:10.000000 hoyo-daily-logins-helper-2.4.2/hoyo-daily-logins-helper.toml.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:17:33.099995 hoyo-daily-logins-helper-2.4.2/hoyo_daily_logins_helper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 08:17:10.000000 hoyo-daily-logins-helper-2.4.2/hoyo_daily_logins_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-17 08:17:10.000000 hoyo-daily-logins-helper-2.4.2/hoyo_daily_logins_helper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-17 08:17:33.000000 hoyo-daily-logins-helper-2.4.2/hoyo_daily_logins_helper/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-17 08:17:10.000000 hoyo-daily-logins-helper-2.4.2/hoyo_daily_logins_helper/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-05-17 08:17:10.000000 hoyo-daily-logins-helper-2.4.2/hoyo_daily_logins_helper/games.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-17 08:17:10.000000 hoyo-daily-logins-helper-2.4.2/hoyo_daily_logins_helper/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-17 08:17:10.000000 hoyo-daily-logins-helper-2.4.2/hoyo_daily_logins_helper/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-05-17 08:17:10.000000 hoyo-daily-logins-helper-2.4.2/hoyo_daily_logins_helper/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-17 08:17:10.000000 hoyo-daily-logins-helper-2.4.2/hoyo_daily_logins_helper/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-17 08:17:10.000000 hoyo-daily-logins-helper-2.4.2/hoyo_daily_logins_helper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:17:33.099995 hoyo-daily-logins-helper-2.4.2/hoyo_daily_logins_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-05-17 08:17:33.000000 hoyo-daily-logins-helper-2.4.2/hoyo_daily_logins_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-17 08:17:33.000000 hoyo-daily-logins-helper-2.4.2/hoyo_daily_logins_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 08:17:33.000000 hoyo-daily-logins-helper-2.4.2/hoyo_daily_logins_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-17 08:17:33.000000 hoyo-daily-logins-helper-2.4.2/hoyo_daily_logins_helper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-17 08:17:33.000000 hoyo-daily-logins-helper-2.4.2/hoyo_daily_logins_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-17 08:17:33.000000 hoyo-daily-logins-helper-2.4.2/hoyo_daily_logins_helper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-17 08:17:10.000000 hoyo-daily-logins-helper-2.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-17 08:17:10.000000 hoyo-daily-logins-helper-2.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 08:17:33.099995 hoyo-daily-logins-helper-2.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 08:17:10.000000 hoyo-daily-logins-helper-2.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:40:55.087072 hoyo-daily-logins-helper-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-31 07:40:30.000000 hoyo-daily-logins-helper-2.5.0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:40:55.079073 hoyo-daily-logins-helper-2.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:40:55.083073 hoyo-daily-logins-helper-2.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-31 07:40:30.000000 hoyo-daily-logins-helper-2.5.0/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-31 07:40:30.000000 hoyo-daily-logins-helper-2.5.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-05-31 07:40:30.000000 hoyo-daily-logins-helper-2.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-31 07:40:30.000000 hoyo-daily-logins-helper-2.5.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    34227 2023-05-31 07:40:30.000000 hoyo-daily-logins-helper-2.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-31 07:40:30.000000 hoyo-daily-logins-helper-2.5.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-05-31 07:40:55.087072 hoyo-daily-logins-helper-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-05-31 07:40:30.000000 hoyo-daily-logins-helper-2.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-31 07:40:30.000000 hoyo-daily-logins-helper-2.5.0/hoyo-daily-logins-helper.toml.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:40:55.083073 hoyo-daily-logins-helper-2.5.0/hoyo_daily_logins_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 07:40:30.000000 hoyo-daily-logins-helper-2.5.0/hoyo_daily_logins_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-31 07:40:30.000000 hoyo-daily-logins-helper-2.5.0/hoyo_daily_logins_helper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-31 07:40:54.000000 hoyo-daily-logins-helper-2.5.0/hoyo_daily_logins_helper/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-31 07:40:30.000000 hoyo-daily-logins-helper-2.5.0/hoyo_daily_logins_helper/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-31 07:40:30.000000 hoyo-daily-logins-helper-2.5.0/hoyo_daily_logins_helper/games.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-31 07:40:30.000000 hoyo-daily-logins-helper-2.5.0/hoyo_daily_logins_helper/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-05-31 07:40:30.000000 hoyo-daily-logins-helper-2.5.0/hoyo_daily_logins_helper/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-05-31 07:40:30.000000 hoyo-daily-logins-helper-2.5.0/hoyo_daily_logins_helper/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-31 07:40:30.000000 hoyo-daily-logins-helper-2.5.0/hoyo_daily_logins_helper/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-31 07:40:30.000000 hoyo-daily-logins-helper-2.5.0/hoyo_daily_logins_helper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 07:40:55.087072 hoyo-daily-logins-helper-2.5.0/hoyo_daily_logins_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-05-31 07:40:55.000000 hoyo-daily-logins-helper-2.5.0/hoyo_daily_logins_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-31 07:40:55.000000 hoyo-daily-logins-helper-2.5.0/hoyo_daily_logins_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 07:40:55.000000 hoyo-daily-logins-helper-2.5.0/hoyo_daily_logins_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-31 07:40:55.000000 hoyo-daily-logins-helper-2.5.0/hoyo_daily_logins_helper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-31 07:40:55.000000 hoyo-daily-logins-helper-2.5.0/hoyo_daily_logins_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-31 07:40:55.000000 hoyo-daily-logins-helper-2.5.0/hoyo_daily_logins_helper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-31 07:40:30.000000 hoyo-daily-logins-helper-2.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-31 07:40:30.000000 hoyo-daily-logins-helper-2.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 07:40:55.087072 hoyo-daily-logins-helper-2.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 07:40:30.000000 hoyo-daily-logins-helper-2.5.0/setup.py
```

### Comparing `hoyo-daily-logins-helper-2.4.2/.github/workflows/deploy.yml` & `hoyo-daily-logins-helper-2.5.0/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.4.2/.github/workflows/tests.yml` & `hoyo-daily-logins-helper-2.5.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.4.2/.gitignore` & `hoyo-daily-logins-helper-2.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.4.2/LICENSE` & `hoyo-daily-logins-helper-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.4.2/PKG-INFO` & `hoyo-daily-logins-helper-2.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoyo-daily-logins-helper
-Version: 2.4.2
+Version: 2.5.0
 Summary: Get hoyo daily login rewards automatically!
 Author-email: Christopher Kaster <me@atomicptr.de>
 Keywords: genshin,genshin-impact,starrail,honkai-starrail,game
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `hoyo-daily-logins-helper-2.4.2/README.md` & `hoyo-daily-logins-helper-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.4.2/hoyo-daily-logins-helper.toml.template` & `hoyo-daily-logins-helper-2.5.0/hoyo-daily-logins-helper.toml.template`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.4.2/hoyo_daily_logins_helper/games.py` & `hoyo-daily-logins-helper-2.5.0/hoyo_daily_logins_helper/games.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,16 @@
 
 
 def game_perform_checkin(
         account_ident: str,
         game: str,
         cookie_str: str,
         language: str,
-        notification_manager: Optional[NotificationManager]
+        notification_manager: Optional[NotificationManager],
+        skip_checkin: bool = False,
 ):
     if game not in GAMES:
         raise Exception(f"unknown game identifier found: {game}")
 
     game_name = GAMES[game]["name"]
     event_base_url = GAMES[game]["event_base_url"]
     act_id = GAMES[game]["act_id"]
@@ -94,15 +95,21 @@
     logging.debug(f"Sleep for {sleep_time}")
     time.sleep(sleep_time)
 
     request_data = json.dumps({
         "act_id": act_id,
     }, ensure_ascii=False)
 
-    response = http_post_json(sign_url, headers=headers, data=request_data)
+    if not skip_checkin:
+        response = http_post_json(sign_url, headers=headers, data=request_data)
+    else:
+        response = {
+            "retcode": 0,
+            "message": "Test Run, skipped actual checkin request"
+        }
 
     code = response.get("retcode", 99999)
 
     logging.debug(f"return code {code}")
 
     if code == RET_CODE_ALREADY_SIGNED_IN:
         logging.info("Already signed in for today...")
@@ -117,28 +124,28 @@
                 message=response["message"],
             ))
         return
 
     reward = awards[total_sign_in_day - 1]
 
     logging.info("Check-in complete!")
-    logging.info(f"\tTotal Sign-in Days: {total_sign_in_day + 1}")
+    logging.info(f"\tTotal Sign-in Days: {total_sign_in_day}")
     logging.info(f"\tReward: {reward['cnt']}x {reward['name']}")
     logging.info(f"\tMessage: {response['message']}")
 
     if notification_manager:
         notification_manager.send(Notification(
             success=True,
             account_identifier=account_ident,
             game_name=game_name,
             message=response["message"],
             custom_fields=[
                 {
                     "key": "Total Sign-in days",
-                    "value": total_sign_in_day + 1
+                    "value": total_sign_in_day
                 },
                 {
                     "key": "Rewards",
                     "value": f"{reward['cnt']}x {reward['name']}",
                 },
             ],
         ))
```

### Comparing `hoyo-daily-logins-helper-2.4.2/hoyo_daily_logins_helper/http.py` & `hoyo-daily-logins-helper-2.5.0/hoyo_daily_logins_helper/http.py`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.4.2/hoyo_daily_logins_helper/main.py` & `hoyo-daily-logins-helper-2.5.0/hoyo_daily_logins_helper/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,14 +101,20 @@
     parser.add_argument(
         "--debug",
         help="run with debug flags",
         action="store_true",
     )
 
     parser.add_argument(
+        "--skip-checkin",
+        help="skip check-in, used for testing",
+        action="store_true",
+    )
+
+    parser.add_argument(
         "-v", "--version",
         action="version",
         version=__version__,
     )
 
     args = parser.parse_args(cli_args)
 
@@ -210,15 +216,16 @@
             identifier = account_identifiers[index]
 
         game_perform_checkin(
             identifier,
             game,
             cookie,
             args.language,
-            notification_manager
+            notification_manager,
+            skip_checkin=args.skip_checkin
         )
 
 
 def has_legacy_environment_variable() -> bool:
     for env_var in ["LANGUAGE", "COOKIE", "GAME"]:
         if env_var in os.environ:
             return True
```

### Comparing `hoyo-daily-logins-helper-2.4.2/hoyo_daily_logins_helper/notifications.py` & `hoyo-daily-logins-helper-2.5.0/hoyo_daily_logins_helper/notifications.py`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.4.2/hoyo_daily_logins_helper/scheduler.py` & `hoyo-daily-logins-helper-2.5.0/hoyo_daily_logins_helper/scheduler.py`

 * *Files 5% similar despite different names*

```diff
@@ -94,14 +94,14 @@
     next_reset = next_reset.replace(
         hour=_RESET_TIME.hour,
         minute=_RESET_TIME.minute,
         second=0,
     )
 
     if next_reset < now:
-        next_reset = next_reset.replace(day=next_reset.day+1)
+        next_reset = next_reset + timedelta(days=1)
 
     diff = next_reset - now
 
     hours = round(diff.total_seconds() / 60 / 60, 1)
 
     logging.info(f"Next reset time is in {hours} hours.")
```

### Comparing `hoyo-daily-logins-helper-2.4.2/hoyo_daily_logins_helper.egg-info/PKG-INFO` & `hoyo-daily-logins-helper-2.5.0/hoyo_daily_logins_helper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoyo-daily-logins-helper
-Version: 2.4.2
+Version: 2.5.0
 Summary: Get hoyo daily login rewards automatically!
 Author-email: Christopher Kaster <me@atomicptr.de>
 Keywords: genshin,genshin-impact,starrail,honkai-starrail,game
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `hoyo-daily-logins-helper-2.4.2/hoyo_daily_logins_helper.egg-info/SOURCES.txt` & `hoyo-daily-logins-helper-2.5.0/hoyo_daily_logins_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.4.2/pyproject.toml` & `hoyo-daily-logins-helper-2.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-2.4.2/requirements.txt` & `hoyo-daily-logins-helper-2.5.0/requirements.txt`

 * *Files identical despite different names*

