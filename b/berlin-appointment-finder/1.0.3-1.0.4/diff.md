# Comparing `tmp/berlin-appointment-finder-1.0.3.tar.gz` & `tmp/berlin-appointment-finder-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "berlin-appointment-finder-1.0.3.tar", last modified: Mon Apr 24 09:24:04 2023, max compression
+gzip compressed data, was "berlin-appointment-finder-1.0.4.tar", last modified: Wed May 31 14:09:32 2023, max compression
```

## Comparing `berlin-appointment-finder-1.0.3.tar` & `berlin-appointment-finder-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-04-24 09:24:04.357942 berlin-appointment-finder-1.0.3/
--rw-------   0 nicolas    (501) staff       (20)     1073 2022-01-25 21:16:12.000000 berlin-appointment-finder-1.0.3/LICENSE
--rw-r--r--   0 nicolas    (501) staff       (20)     2996 2023-04-24 09:24:04.357245 berlin-appointment-finder-1.0.3/PKG-INFO
--rw-r--r--   0 nicolas    (501) staff       (20)     2603 2023-04-16 12:00:04.000000 berlin-appointment-finder-1.0.3/README.md
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-04-24 09:24:04.349013 berlin-appointment-finder-1.0.3/appointments/
--rw-r--r--   0 nicolas    (501) staff       (20)        0 2023-04-11 08:41:36.000000 berlin-appointment-finder-1.0.3/appointments/__init__.py
--rw-r--r--   0 nicolas    (501) staff       (20)     7145 2023-04-24 09:20:58.000000 berlin-appointment-finder-1.0.3/appointments/appointments.py
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-04-24 09:24:04.354962 berlin-appointment-finder-1.0.3/berlin_appointment_finder.egg-info/
--rw-r--r--   0 nicolas    (501) staff       (20)     2996 2023-04-24 09:24:04.000000 berlin-appointment-finder-1.0.3/berlin_appointment_finder.egg-info/PKG-INFO
--rw-r--r--   0 nicolas    (501) staff       (20)      389 2023-04-24 09:24:04.000000 berlin-appointment-finder-1.0.3/berlin_appointment_finder.egg-info/SOURCES.txt
--rw-r--r--   0 nicolas    (501) staff       (20)        1 2023-04-24 09:24:04.000000 berlin-appointment-finder-1.0.3/berlin_appointment_finder.egg-info/dependency_links.txt
--rw-r--r--   0 nicolas    (501) staff       (20)        1 2023-04-05 11:21:55.000000 berlin-appointment-finder-1.0.3/berlin_appointment_finder.egg-info/not-zip-safe
--rw-r--r--   0 nicolas    (501) staff       (20)       85 2023-04-24 09:24:04.000000 berlin-appointment-finder-1.0.3/berlin_appointment_finder.egg-info/requires.txt
--rw-r--r--   0 nicolas    (501) staff       (20)       13 2023-04-24 09:24:04.000000 berlin-appointment-finder-1.0.3/berlin_appointment_finder.egg-info/top_level.txt
-drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-04-24 09:24:04.355827 berlin-appointment-finder-1.0.3/bin/
--rwxr-xr-x   0 nicolas    (501) staff       (20)     2259 2023-04-05 12:26:04.000000 berlin-appointment-finder-1.0.3/bin/appointments
--rw-r--r--   0 nicolas    (501) staff       (20)       38 2023-04-24 09:24:04.358156 berlin-appointment-finder-1.0.3/setup.cfg
--rw-r--r--   0 nicolas    (501) staff       (20)      857 2023-04-24 09:21:23.000000 berlin-appointment-finder-1.0.3/setup.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-05-31 14:09:32.854866 berlin-appointment-finder-1.0.4/
+-rw-------   0 nicolas    (501) staff       (20)     1073 2022-01-25 21:16:12.000000 berlin-appointment-finder-1.0.4/LICENSE
+-rw-r--r--   0 nicolas    (501) staff       (20)     3235 2023-05-31 14:09:32.854119 berlin-appointment-finder-1.0.4/PKG-INFO
+-rw-r--r--   0 nicolas    (501) staff       (20)     2842 2023-04-28 12:11:17.000000 berlin-appointment-finder-1.0.4/README.md
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-05-31 14:09:32.845719 berlin-appointment-finder-1.0.4/appointments/
+-rw-r--r--   0 nicolas    (501) staff       (20)        0 2023-04-11 08:41:36.000000 berlin-appointment-finder-1.0.4/appointments/__init__.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     6324 2023-05-31 14:06:19.000000 berlin-appointment-finder-1.0.4/appointments/appointments.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-05-31 14:09:32.851256 berlin-appointment-finder-1.0.4/berlin_appointment_finder.egg-info/
+-rw-r--r--   0 nicolas    (501) staff       (20)     3235 2023-05-31 14:09:32.000000 berlin-appointment-finder-1.0.4/berlin_appointment_finder.egg-info/PKG-INFO
+-rw-r--r--   0 nicolas    (501) staff       (20)      389 2023-05-31 14:09:32.000000 berlin-appointment-finder-1.0.4/berlin_appointment_finder.egg-info/SOURCES.txt
+-rw-r--r--   0 nicolas    (501) staff       (20)        1 2023-05-31 14:09:32.000000 berlin-appointment-finder-1.0.4/berlin_appointment_finder.egg-info/dependency_links.txt
+-rw-r--r--   0 nicolas    (501) staff       (20)        1 2023-04-05 11:21:55.000000 berlin-appointment-finder-1.0.4/berlin_appointment_finder.egg-info/not-zip-safe
+-rw-r--r--   0 nicolas    (501) staff       (20)       85 2023-05-31 14:09:32.000000 berlin-appointment-finder-1.0.4/berlin_appointment_finder.egg-info/requires.txt
+-rw-r--r--   0 nicolas    (501) staff       (20)       13 2023-05-31 14:09:32.000000 berlin-appointment-finder-1.0.4/berlin_appointment_finder.egg-info/top_level.txt
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-05-31 14:09:32.852111 berlin-appointment-finder-1.0.4/bin/
+-rwxr-xr-x   0 nicolas    (501) staff       (20)     2259 2023-04-05 12:26:04.000000 berlin-appointment-finder-1.0.4/bin/appointments
+-rw-r--r--   0 nicolas    (501) staff       (20)       38 2023-05-31 14:09:32.855049 berlin-appointment-finder-1.0.4/setup.cfg
+-rw-r--r--   0 nicolas    (501) staff       (20)      857 2023-05-31 14:08:20.000000 berlin-appointment-finder-1.0.4/setup.py
```

### Comparing `berlin-appointment-finder-1.0.3/LICENSE` & `berlin-appointment-finder-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `berlin-appointment-finder-1.0.3/PKG-INFO` & `berlin-appointment-finder-1.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: berlin-appointment-finder
-Version: 1.0.3
+Version: 1.0.4
 Summary: Finds appointments at the Berlin Bürgeramt, broadcasts them via websockets
 Home-page: https://github.com/nicbou/burgeramt-appointments-websockets
 Author: Nicolas Bouliane
 Author-email: contact@nicolasbouliane.com
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -68,7 +68,11 @@
 ```
 
 The script broadcasts broadcasts the appointments it finds with websockets. By default, it broadcasts them on port 80.
 
 A Dockerfile is supplied in this repo. It's the same one I use on All About Berlin.
 
 The polling rate is limited to 180 seconds (3 minutes), as required by the Berlin.de IKT-ZMS team (ikt-zms@seninnds.berlin.de).
+
+### Local development
+
+To work on this script, install it with `pip install -e /path/to/this/repo`. When you run `appointments`, it will run your local version with any changes you have made to it. You only need to run this command once.
```

### Comparing `berlin-appointment-finder-1.0.3/README.md` & `berlin-appointment-finder-1.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -55,8 +55,12 @@
 BOOKING_TOOL_URL=https://service.berlin.de/dienstleistung/120686/
 ```
 
 The script broadcasts broadcasts the appointments it finds with websockets. By default, it broadcasts them on port 80.
 
 A Dockerfile is supplied in this repo. It's the same one I use on All About Berlin.
 
-The polling rate is limited to 180 seconds (3 minutes), as required by the Berlin.de IKT-ZMS team (ikt-zms@seninnds.berlin.de).
+The polling rate is limited to 180 seconds (3 minutes), as required by the Berlin.de IKT-ZMS team (ikt-zms@seninnds.berlin.de).
+
+### Local development
+
+To work on this script, install it with `pip install -e /path/to/this/repo`. When you run `appointments`, it will run your local version with any changes you have made to it. You only need to run this command once.
```

### Comparing `berlin-appointment-finder-1.0.3/appointments/appointments.py` & `berlin-appointment-finder-1.0.4/appointments/appointments.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,69 +30,48 @@
     'appointmentDates': [],
 }
 
 
 timezone = pytz.timezone('Europe/Berlin')
 
 
-async def get_appointments_url(service_page_url: str, email: str, script_id: str):
-    headers = {
+def get_headers(email: str, script_id: str) -> dict:
+    return {
         'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8',
         'Upgrade-Insecure-Requests': '1',
         'User-Agent': f"Mozilla/5.0 AppointmentBookingTool/1.1 (https://github.com/nicbou/burgeramt-appointments-websockets; {email}; {script_id})",
         'Accept-Language': 'en-gb',
         'Accept-Encoding': 'gzip, deflate',
         'Connection': 'keep-alive',
     }
-    async with aiohttp.ClientSession() as session:
-        async with session.get(service_page_url, headers=headers) as response:
-            service_page_content = await response.text()
-            termin_suchen_button = SoupStrainer('div', class_='zmstermin-multi inner')
-            termin_suchen_link = BeautifulSoup(service_page_content, 'lxml', parse_only=termin_suchen_button).find('a')
-            return termin_suchen_link['href']
+
+
+def get_appointments_url(service_page_url: str):
+    service_id = service_page_url.rstrip('/').split('/')[-1]
+    return f"https://service.berlin.de/terminvereinbarung/termin/all/{service_id}/"
 
 
 async def get_appointments(appointments_url: str, email: str, script_id: str) -> list:
     """
     Fetches the appointments calendar on Berlin.de, parses it, and returns available appointment dates.
     """
     today = timezone.localize(datetime.now())
     next_month = timezone.localize(datetime(today.year, today.month % 12 + 1, 1))
     next_month_timestamp = int(next_month.timestamp())
 
     async with aiohttp.ClientSession(raise_for_status=True) as session:
-        headers = {
-            'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8',
-            'Upgrade-Insecure-Requests': '1',
-            'User-Agent': f"Mozilla/5.0 AppointmentBookingTool/1.1 (https://github.com/nicbou/burgeramt-appointments-websockets; {email}; {script_id})",
-            'Accept-Language': 'en-gb',
-            'Accept-Encoding': 'gzip, deflate',
-            'Connection': 'keep-alive',
-        }
-
         # Load the first two months
-        response_p1 = await session.get(appointments_url, headers=headers, timeout=20)
-        response_p1.raise_for_status()
-        await asyncio.sleep(1)
-
-        # Load the next two months
-        response_p2 = await session.get(
-            f'https://service.berlin.de/terminvereinbarung/termin/day/{next_month_timestamp}/',
-            headers=headers, timeout=20
-        )
-        response_p2.raise_for_status()
-
-    return sorted(
-        list(
-            set(
-                parse_appointment_dates(await response_p1.text())
-                + parse_appointment_dates(await response_p2.text())
-            )
-        )
-    )
+        async with session.get(appointments_url, headers=get_headers(email, script_id), timeout=20) as response_page1:
+            page1_dates = parse_appointment_dates(await response_page1.text())
+
+        page2_url = f'https://service.berlin.de/terminvereinbarung/termin/day/{next_month_timestamp}/'
+        async with session.get(page2_url, headers=get_headers(email, script_id), timeout=20) as response_page2:
+            page2_dates = parse_appointment_dates(await response_page2.text())
+
+    return sorted(list(set(page1_dates + page2_dates)))
 
 
 def parse_appointment_dates(page_content: str) -> list:
     """
     Parse the content of the calendar page on Berlin.de, and returns available appointment dates.
     """
     appointment_strainer = SoupStrainer('td', class_='buchbar')
@@ -134,21 +113,21 @@
         return {
             'time': datetime_to_json(datetime.now()),
             'status': 502,
             'message': 'Could not fetch results from Berlin.de - Got connection error.',
             'appointmentDates': [],
         }
     except asyncio.exceptions.TimeoutError:
-        logger.warning(f"Got Timeout on response from Berlin.de. Checking in {refresh_delay} seconds")
+        logger.exception(f"Got Timeout on response from Berlin.de. Checking in {refresh_delay} seconds")
         if not quiet:
             chime.error()
         return {
             'time': datetime_to_json(datetime.now()),
             'status': 504,
-            'message': f'Could not fetch results from Berlin.de. - Timeout',
+            'message': 'Could not fetch results from Berlin.de. - Request timed out',
             'appointmentDates': [],
         }
     except Exception as err:
         logger.exception("Could not fetch results due to an unexpected error.")
         if not quiet:
             chime.error()
         return {
@@ -174,15 +153,15 @@
 
 async def watch_for_appointments(service_page_url: str, email: str, script_id: str, server_port: int, quiet: bool):
     """
     Constantly look for new appointments on Berlin.de until stopped.
     """
     global last_message
     logger.info(f"Getting appointment URL for {service_page_url}")
-    appointments_url = await get_appointments_url(service_page_url, email, script_id)
+    appointments_url = get_appointments_url(service_page_url)
     logger.info(f"URL found: {appointments_url}")
     async with websockets.serve(on_connect, port=server_port):
         logger.info(f"Server is running on port {server_port}. Looking for appointments every {refresh_delay} seconds.")
         while True:
             last_message = await look_for_appointments(appointments_url, email, script_id, quiet)
             websockets.broadcast(connected_clients, json.dumps(last_message))
             await asyncio.sleep(refresh_delay)
```

### Comparing `berlin-appointment-finder-1.0.3/berlin_appointment_finder.egg-info/PKG-INFO` & `berlin-appointment-finder-1.0.4/berlin_appointment_finder.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: berlin-appointment-finder
-Version: 1.0.3
+Version: 1.0.4
 Summary: Finds appointments at the Berlin Bürgeramt, broadcasts them via websockets
 Home-page: https://github.com/nicbou/burgeramt-appointments-websockets
 Author: Nicolas Bouliane
 Author-email: contact@nicolasbouliane.com
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -68,7 +68,11 @@
 ```
 
 The script broadcasts broadcasts the appointments it finds with websockets. By default, it broadcasts them on port 80.
 
 A Dockerfile is supplied in this repo. It's the same one I use on All About Berlin.
 
 The polling rate is limited to 180 seconds (3 minutes), as required by the Berlin.de IKT-ZMS team (ikt-zms@seninnds.berlin.de).
+
+### Local development
+
+To work on this script, install it with `pip install -e /path/to/this/repo`. When you run `appointments`, it will run your local version with any changes you have made to it. You only need to run this command once.
```

### Comparing `berlin-appointment-finder-1.0.3/bin/appointments` & `berlin-appointment-finder-1.0.4/bin/appointments`

 * *Files identical despite different names*

### Comparing `berlin-appointment-finder-1.0.3/setup.py` & `berlin-appointment-finder-1.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name='berlin-appointment-finder',
-    version='1.0.3',
+    version='1.0.4',
     description='Finds appointments at the Berlin Bürgeramt, broadcasts them via websockets',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/nicbou/burgeramt-appointments-websockets',
     author='Nicolas Bouliane',
     author_email='contact@nicolasbouliane.com',
     license='MIT',
```

