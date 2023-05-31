# Comparing `tmp/fcm-django-1.0.9.tar.gz` & `tmp/fcm-django-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fcm-django-1.0.9.tar", last modified: Mon Mar 28 19:58:00 2022, max compression
+gzip compressed data, was "fcm-django-2.0.0.tar", last modified: Wed May 31 09:14:13 2023, max compression
```

## Comparing `fcm-django-1.0.9.tar` & `fcm-django-2.0.0.tar`

### file list

```diff
@@ -1,34 +1,37 @@
-drwxrwxr-x   0 xtrinch   (1000) xtrinch   (1000)        0 2022-03-28 19:58:00.597139 fcm-django-1.0.9/
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)     1130 2021-04-11 10:41:31.000000 fcm-django-1.0.9/LICENSE.txt
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)       55 2021-04-11 10:41:31.000000 fcm-django-1.0.9/MANIFEST.in
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)     1016 2022-03-28 19:58:00.597139 fcm-django-1.0.9/PKG-INFO
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)    12673 2022-03-28 19:44:13.000000 fcm-django-1.0.9/README.rst
-drwxrwxr-x   0 xtrinch   (1000) xtrinch   (1000)        0 2022-03-28 19:58:00.593139 fcm-django-1.0.9/fcm_django/
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)      309 2022-03-28 19:52:13.000000 fcm-django-1.0.9/fcm_django/__init__.py
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)     8741 2022-03-28 19:45:14.000000 fcm-django-1.0.9/fcm_django/admin.py
-drwxrwxr-x   0 xtrinch   (1000) xtrinch   (1000)        0 2022-03-28 19:58:00.597139 fcm-django-1.0.9/fcm_django/api/
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)      341 2021-07-10 12:52:28.000000 fcm-django-1.0.9/fcm_django/api/__init__.py
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)     5909 2022-03-28 19:42:44.000000 fcm-django-1.0.9/fcm_django/api/rest_framework.py
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)      806 2021-07-10 12:52:28.000000 fcm-django-1.0.9/fcm_django/api/tastypie.py
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)      207 2022-01-07 16:08:01.000000 fcm-django-1.0.9/fcm_django/apps.py
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)     4147 2022-03-28 19:56:39.000000 fcm-django-1.0.9/fcm_django/fields.py
-drwxrwxr-x   0 xtrinch   (1000) xtrinch   (1000)        0 2022-03-28 19:58:00.597139 fcm-django-1.0.9/fcm_django/migrations/
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)     2555 2021-07-10 12:52:28.000000 fcm-django-1.0.9/fcm_django/migrations/0001_initial.py
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)      598 2021-07-10 12:52:28.000000 fcm-django-1.0.9/fcm_django/migrations/0002_auto_20160808_1645.py
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)      504 2021-07-10 12:52:28.000000 fcm-django-1.0.9/fcm_django/migrations/0003_auto_20170313_1314.py
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)      444 2021-07-10 12:52:28.000000 fcm-django-1.0.9/fcm_django/migrations/0004_auto_20181128_1642.py
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)      750 2021-07-10 12:52:28.000000 fcm-django-1.0.9/fcm_django/migrations/0005_auto_20170808_1145.py
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)      610 2021-08-17 14:10:04.000000 fcm-django-1.0.9/fcm_django/migrations/0006_auto_20210802_1140.py
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)      362 2021-12-16 09:07:29.000000 fcm-django-1.0.9/fcm_django/migrations/0007_auto_20211001_1440.py
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)      477 2021-12-24 13:42:53.000000 fcm-django-1.0.9/fcm_django/migrations/0008_auto_20211224_1205.py
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)        0 2021-04-11 10:41:31.000000 fcm-django-1.0.9/fcm_django/migrations/__init__.py
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)    13763 2022-03-28 19:42:44.000000 fcm-django-1.0.9/fcm_django/models.py
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)      779 2021-07-10 12:52:28.000000 fcm-django-1.0.9/fcm_django/settings.py
-drwxrwxr-x   0 xtrinch   (1000) xtrinch   (1000)        0 2022-03-28 19:58:00.593139 fcm-django-1.0.9/fcm_django.egg-info/
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)     1016 2022-03-28 19:58:00.000000 fcm-django-1.0.9/fcm_django.egg-info/PKG-INFO
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)      851 2022-03-28 19:58:00.000000 fcm-django-1.0.9/fcm_django.egg-info/SOURCES.txt
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)        1 2022-03-28 19:58:00.000000 fcm-django-1.0.9/fcm_django.egg-info/dependency_links.txt
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)       28 2022-03-28 19:58:00.000000 fcm-django-1.0.9/fcm_django.egg-info/requires.txt
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)       48 2022-03-28 19:58:00.000000 fcm-django-1.0.9/fcm_django.egg-info/top_level.txt
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)       67 2022-03-28 19:58:00.597139 fcm-django-1.0.9/setup.cfg
--rw-rw-r--   0 xtrinch   (1000) xtrinch   (1000)     1329 2022-03-28 19:00:13.000000 fcm-django-1.0.9/setup.py
+drwxr-xr-x   0 mojcarojko   (501) staff       (20)        0 2023-05-31 09:14:13.902922 fcm-django-2.0.0/
+-rw-r--r--   0 mojcarojko   (501) staff       (20)     1130 2023-04-05 08:36:57.000000 fcm-django-2.0.0/LICENSE.txt
+-rw-r--r--   0 mojcarojko   (501) staff       (20)       55 2023-04-05 08:36:57.000000 fcm-django-2.0.0/MANIFEST.in
+-rw-r--r--   0 mojcarojko   (501) staff       (20)     1090 2023-05-31 09:14:13.903075 fcm-django-2.0.0/PKG-INFO
+-rw-r--r--   0 mojcarojko   (501) staff       (20)    14558 2023-05-31 09:11:42.000000 fcm-django-2.0.0/README.rst
+drwxr-xr-x   0 mojcarojko   (501) staff       (20)        0 2023-05-31 09:14:13.885071 fcm-django-2.0.0/fcm_django/
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      309 2023-05-31 09:13:22.000000 fcm-django-2.0.0/fcm_django/__init__.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)     8787 2023-04-05 08:36:57.000000 fcm-django-2.0.0/fcm_django/admin.py
+drwxr-xr-x   0 mojcarojko   (501) staff       (20)        0 2023-05-31 09:14:13.890071 fcm-django-2.0.0/fcm_django/api/
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      341 2023-04-05 08:36:57.000000 fcm-django-2.0.0/fcm_django/api/__init__.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)     5909 2023-04-05 08:36:57.000000 fcm-django-2.0.0/fcm_django/api/rest_framework.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      806 2023-04-05 08:36:57.000000 fcm-django-2.0.0/fcm_django/api/tastypie.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      207 2023-04-05 08:36:57.000000 fcm-django-2.0.0/fcm_django/apps.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)     4147 2023-04-05 08:36:57.000000 fcm-django-2.0.0/fcm_django/fields.py
+drwxr-xr-x   0 mojcarojko   (501) staff       (20)        0 2023-05-31 09:14:13.902652 fcm-django-2.0.0/fcm_django/migrations/
+-rw-r--r--   0 mojcarojko   (501) staff       (20)     2555 2023-04-05 08:36:57.000000 fcm-django-2.0.0/fcm_django/migrations/0001_initial.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      598 2023-04-05 08:36:57.000000 fcm-django-2.0.0/fcm_django/migrations/0002_auto_20160808_1645.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      504 2023-04-05 08:36:57.000000 fcm-django-2.0.0/fcm_django/migrations/0003_auto_20170313_1314.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      444 2023-04-05 08:36:57.000000 fcm-django-2.0.0/fcm_django/migrations/0004_auto_20181128_1642.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      750 2023-04-05 08:36:57.000000 fcm-django-2.0.0/fcm_django/migrations/0005_auto_20170808_1145.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      610 2023-04-05 08:36:57.000000 fcm-django-2.0.0/fcm_django/migrations/0006_auto_20210802_1140.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      362 2023-04-05 08:36:57.000000 fcm-django-2.0.0/fcm_django/migrations/0007_auto_20211001_1440.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      477 2023-04-05 08:36:57.000000 fcm-django-2.0.0/fcm_django/migrations/0008_auto_20211224_1205.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      734 2023-04-05 08:36:57.000000 fcm-django-2.0.0/fcm_django/migrations/0009_alter_fcmdevice_user.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)     1232 2023-05-29 13:01:34.000000 fcm-django-2.0.0/fcm_django/migrations/0010_unique_registration_id.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)     1215 2023-05-29 13:01:34.000000 fcm-django-2.0.0/fcm_django/migrations/0011_fcmdevice_fcm_django_registration_id_user_id_idx.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)        0 2023-04-05 08:36:57.000000 fcm-django-2.0.0/fcm_django/migrations/__init__.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)    14305 2023-05-05 07:48:50.000000 fcm-django-2.0.0/fcm_django/models.py
+-rw-r--r--   0 mojcarojko   (501) staff       (20)      902 2023-05-05 08:22:10.000000 fcm-django-2.0.0/fcm_django/settings.py
+drwxr-xr-x   0 mojcarojko   (501) staff       (20)        0 2023-05-31 09:14:13.887799 fcm-django-2.0.0/fcm_django.egg-info/
+-rw-r--r--   0 mojcarojko   (501) staff       (20)     1090 2023-05-31 09:14:13.000000 fcm-django-2.0.0/fcm_django.egg-info/PKG-INFO
+-rw-r--r--   0 mojcarojko   (501) staff       (20)     1034 2023-05-31 09:14:13.000000 fcm-django-2.0.0/fcm_django.egg-info/SOURCES.txt
+-rw-r--r--   0 mojcarojko   (501) staff       (20)        1 2023-05-31 09:14:13.000000 fcm-django-2.0.0/fcm_django.egg-info/dependency_links.txt
+-rw-r--r--   0 mojcarojko   (501) staff       (20)       28 2023-05-31 09:14:13.000000 fcm-django-2.0.0/fcm_django.egg-info/requires.txt
+-rw-r--r--   0 mojcarojko   (501) staff       (20)       48 2023-05-31 09:14:13.000000 fcm-django-2.0.0/fcm_django.egg-info/top_level.txt
+-rw-r--r--   0 mojcarojko   (501) staff       (20)       67 2023-05-31 09:14:13.903622 fcm-django-2.0.0/setup.cfg
+-rw-r--r--   0 mojcarojko   (501) staff       (20)     1423 2023-05-31 09:12:43.000000 fcm-django-2.0.0/setup.py
```

### Comparing `fcm-django-1.0.9/LICENSE.txt` & `fcm-django-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fcm-django-1.0.9/README.rst` & `fcm-django-2.0.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -68,16 +68,15 @@
 of bulk messages.
 
 .. code-block:: python
 
     from firebase_admin.messaging import Message, Notification
     topic = "A topic"
     FCMDevice.objects.handle_subscription(True, topic)
-    message = Message(..., topic=topic)
-    FCMDevice.objects.filter(is_cool=True).send_message(message)
+    FCMDevice.send_topic_message(Message(data={...}), "TOPIC NAME")
 
 There are two additional parameters to both methods:
 ``skip_registration_id_lookup`` and ``additional_registration_ids``.
 Visit `Sending Messages <https://github.com/xtrinch/fcm-django#sending-messages>`_ to learn more.
 
 Note: ``registration_ids`` is actually incorrect terminology as it
 should actually be called ``registration tokens``. However, to be
@@ -85,15 +84,15 @@
 switching to stay backwards compatible in the docs and with the
 sister package.
 
 Setup
 -----
 You can install the library directly from pypi using pip:
 
-.. code-block::
+.. code-block:: console
 
     pip install fcm-django
 
 
 Edit your settings.py file:
 
 .. code-block:: python
@@ -113,27 +112,26 @@
     # which is a path that point to a json file with your credentials.
     # Additional arguments are available: credentials, options, name
     FIREBASE_APP = initialize_app()
     # To learn more, visit the docs here:
     # https://cloud.google.com/docs/authentication/getting-started>
 
     FCM_DJANGO_SETTINGS = {
+         # an instance of firebase_admin.App to be used as default for all fcm-django requests
+         # default: None (the default Firebase app)
+        "DEFAULT_FIREBASE_APP": None,
          # default: _('FCM Django')
         "APP_VERBOSE_NAME": "[string for AppConfig's verbose_name]",
          # true if you want to have only one active device per registered user at a time
          # default: False
         "ONE_DEVICE_PER_USER": True/False,
          # devices to which notifications cannot be sent,
          # are deleted upon receiving error response from FCM
          # default: False
         "DELETE_INACTIVE_DEVICES": True/False,
-        # Transform create of an existing Device (based on registration id) into
-		    # an update. See the section
-        # "Update of device with duplicate registration ID" for more details.
-        "UPDATE_ON_DUPLICATE_REG_ID": True/False,
     }
 
 Native Django migrations are in use. ``manage.py migrate`` will install and migrate all models.
 
 Messages
 --------
 
@@ -250,25 +248,71 @@
     from firebase_admin.messaging import Message
     from fcm_django.models import FCMDevice
     FCMDevice.objects.send_message(Message(...), False, ["registration_ids"])
 
 Using multiple FCM apps
 -----------------------
 
-By default the message will be sent using the default FCM ``firebase_admin.App`` (we initialized this in our settings). This default can be overridden by specifying an app when calling send_message. This can be used to send messages using different firebase projects.
+By default the message will be sent using the default FCM ``firebase_admin.App`` (we initialized this in our settings),
+or the one specified with the ``DEFAULT_FIREBASE_APP`` setting.
+
+This default can be overridden by specifying an app when calling send_message. This can be used to send messages using different firebase projects.
 
 .. code-block:: python
 
     from firebase_app import App
     from firebase_app.messaging import Notification
     from fcm_django.models import FCMDevice
 
     device = FCMDevice.objects.all().first()
     device.send_message(notification=Notification(...), app=App(...))
 
+Setting a default Firebase app for FCM
+--------------------------------------
+
+If you want to use a specific Firebase app for all fcm-django requests, you can create an instance of
+``firebase_admin.App`` and pass it to fcm-django with the ``DEFAULT_FIREBASE_APP`` setting.
+
+The ``DEFAULT_FIREBASE_APP`` will be used for all send / subscribe / unsubscribe requests, include ``FCMDevice``'s
+admin actions.
+
+In your ``settings.py``:
+
+.. code-block:: python
+
+    from firebase_admin import initialize_app, credentials
+    from google.auth import load_credentials_from_file
+    from google.oauth2.service_account import Credentials
+
+    # create a custom Credentials class to load a non-default google service account JSON
+    class CustomFirebaseCredentials(credentials.ApplicationDefault):
+        def __init__(self, account_file_path: str):
+            super().__init__()
+            self._account_file_path = account_file_path
+
+        def _load_credential(self):
+            if not self._g_credential:
+                self._g_credential, self._project_id = load_credentials_from_file(self._account_file_path,
+                                                                                  scopes=credentials._scopes)
+
+    # init default firebase app
+    # this loads the default google service account with GOOGLE_APPLICATION_CREDENTIALS env variable
+    FIREBASE_APP = initialize_app()
+
+    # init second firebase app for fcm-django
+    # the environment variable contains a path to the custom google service account JSON
+    custom_credentials = CustomFirebaseCredentials(os.getenv('CUSTOM_GOOGLE_APPLICATION_CREDENTIALS'))
+    FIREBASE_MESSAGING_APP = initialize_app(custom_credentials, name='messaging')
+
+    FCM_DJANGO_SETTINGS = {
+        "DEFAULT_FIREBASE_APP": FIREBASE_MESSAGING_APP,
+        # [...] your other settings
+    }
+
+
 Django REST Framework (DRF) support
 -----------------------------------
 
 Viewsets come in two different varieties:
 
 - ``FCMDeviceViewSet``
 
@@ -276,15 +320,15 @@
     - A device may be registered without associating it with a user
     - Will not allow duplicate registration_id's
 
 - ``FCMDeviceAuthorizedViewSet``
 
     - Permissions are ``IsAuthenticated`` and custom permission ``IsOwner``, which will only allow the ``request.user`` to get and update devices that belong to that user
     - Requires a user to be authenticated, so all devices will be associated with a user
-    - Will allow duplicate registration_id's for different users, so you are responsible for cleanup (if you do not want duplicate registration id's, use the ``UPDATE_ON_DUPLICATE_REG_ID`` flag)
+    - Will update the device on duplicate registration id
 
 Routes can be added one of two ways:
 
 - `Routers`_ (include all views)
 
 .. _Routers: http://www.django-rest-framework.org/tutorial/6-viewsets-and-routers#using-routers
 
@@ -318,30 +362,30 @@
         path('devices', FCMDeviceAuthorizedViewSet.as_view({'post': 'create'}), name='create_fcm_device'),
         # ...
     ]
 
 Update of device with duplicate registration ID
 -----------------------------------------------
 
-The DRF viewset enforce the uniqueness of the registration ID. In same use case it
-may cause an issue: If an already registered mobile device changes its user, then
-it will fail to register because the registration ID already exist.
-
-When option ``UPDATE_ON_DUPLICATE_REG_ID`` is set to True, then any creation of
-device with an already existing registration ID will be transformed into an update.
+Tokens are device specific, so if the user e.g. logs out of their account on your device, and another user
+logins on the same device, you do not wish the old user to receive messages while logged out.
 
-The ``UPDATE_ON_DUPLICATE_REG_ID`` only works with DRF.
+Via DRF, any creation of device with an already existing registration ID will be transformed into an update.
+If done manually, you are responsible for deleting the old device entry.
 
 Python 3 support
 ----------------
-``fcm-django`` is fully compatible with Python 3.6+
+- ``fcm-django`` is fully compatible with Python 3.7+
+- for Python 3.6, use ``fcm-django < 2.0.0`` , because `firebase-admin with version 6 drop support of Python 3.6 <https://firebase.google.com/support/release-notes/admin/python#version_600_-_06_october_2022>`_
 
 Django version compatibility
 ----------------------------
-Compatible with Django versions 2.2+. For lower django versions, use version ``fcm-django < 1``.
+Compatible with Django versions 3.0+.
+For Django version 2.2, use version ``fcm-django < 1.0.13``.
+For lower django versions, use version ``fcm-django < 1.0.0``.
 
 Acknowledgements
 ----------------
 Library relies on firebase-admin-sdk for sending notifications, for more info about all the possible fields, see:
 https://github.com/firebase/firebase-admin-python
 
 Migration from v0 to v1 was done by `Andrew-Chen-Wang <https://github.com/Andrew-Chen-Wang>`_
```

### Comparing `fcm-django-1.0.9/fcm_django/admin.py` & `fcm-django-2.0.0/fcm_django/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,19 @@
         "device_id",
         "name",
         "type",
         "user",
         "active",
         "date_created",
     )
-    list_filter = ("active",)
+    list_filter = (
+        "active",
+        "user",
+        "type",
+    )
     actions = (
         "send_message",
         "send_bulk_message",
         "subscribe_to_topic",
         "bulk_subscribe_to_topic",
         "unsubscribe_to_topic",
         "bulk_unsubscribe_to_topic",
```

### Comparing `fcm-django-1.0.9/fcm_django/api/rest_framework.py` & `fcm-django-2.0.0/fcm_django/api/rest_framework.py`

 * *Files identical despite different names*

### Comparing `fcm-django-1.0.9/fcm_django/api/tastypie.py` & `fcm-django-2.0.0/fcm_django/api/tastypie.py`

 * *Files identical despite different names*

### Comparing `fcm-django-1.0.9/fcm_django/fields.py` & `fcm-django-2.0.0/fcm_django/fields.py`

 * *Files identical despite different names*

### Comparing `fcm-django-1.0.9/fcm_django/migrations/0001_initial.py` & `fcm-django-2.0.0/fcm_django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `fcm-django-1.0.9/fcm_django/migrations/0002_auto_20160808_1645.py` & `fcm-django-2.0.0/fcm_django/migrations/0002_auto_20160808_1645.py`

 * *Files identical despite different names*

### Comparing `fcm-django-1.0.9/fcm_django/migrations/0005_auto_20170808_1145.py` & `fcm-django-2.0.0/fcm_django/migrations/0005_auto_20170808_1145.py`

 * *Files identical despite different names*

### Comparing `fcm-django-1.0.9/fcm_django/migrations/0006_auto_20210802_1140.py` & `fcm-django-2.0.0/fcm_django/migrations/0006_auto_20210802_1140.py`

 * *Files identical despite different names*

### Comparing `fcm-django-1.0.9/fcm_django/models.py` & `fcm-django-2.0.0/fcm_django/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from copy import copy
-from itertools import repeat
 from typing import List, NamedTuple, Optional, Sequence, Union
 
 from django.db import models
 from django.utils.translation import gettext_lazy as _
 from firebase_admin import messaging
 from firebase_admin.exceptions import FirebaseError, InvalidArgumentError
 
@@ -29,15 +28,15 @@
         help_text=_("Inactive devices will not be sent notifications"),
     )
     user = models.ForeignKey(
         SETTINGS["USER_MODEL"],
         blank=True,
         null=True,
         on_delete=models.CASCADE,
-        related_query_name=_("device"),
+        related_query_name=_("fcmdevice"),
     )
     date_created = models.DateTimeField(
         verbose_name=_("Creation date"), auto_now_add=True, null=True
     )
 
     class Meta:
         abstract = True
@@ -112,65 +111,63 @@
         QuerySet lookup
         :returns a list of registration IDs
         """
         registration_ids = (
             list(additional_registration_ids) if additional_registration_ids else []
         )
         if not skip_registration_id_lookup:
-            if not self.exists() and not additional_registration_ids:
-                return []
             registration_ids.extend(
                 self.filter(active=True).values_list("registration_id", flat=True)
             )
         return registration_ids
 
     def send_message(
         self,
         message: messaging.Message,
         skip_registration_id_lookup: bool = False,
         additional_registration_ids: Sequence[str] = None,
+        app: "firebase_admin.App" = SETTINGS["DEFAULT_FIREBASE_APP"],
         **more_send_message_kwargs,
     ) -> FirebaseResponseDict:
         """
         Send notification of single message for all active devices in
         queryset and deactivate if DELETE_INACTIVE_DEVICES setting is set to True.
         Bulk sends using firebase.messaging.send_all. For every 500 messages, we send a
         single HTTP request to Firebase (the 500 is set by the firebase-sdk).
 
         :param message: firebase.messaging.Message. If `message` includes a token/id, it
         will be overridden.
         :param skip_registration_id_lookup: skips the QuerySet lookup and solely uses
         the list of IDs from additional_registration_ids
         :param additional_registration_ids: specific registration_ids to add to the
+        :param app: firebase_admin.App. Specify a specific app to use
         QuerySet lookup
         :param more_send_message_kwargs: Parameters for firebase.messaging.send_all()
         - dry_run: bool. Whether to actually send the notification to the device
-        - app: firebase_admin.App. Specify a specific app to use
         If there are any new parameters, you can still specify them here.
 
         :raises FirebaseError
         :returns FirebaseResponseDict
         """
         registration_ids = self.get_registration_ids(
             skip_registration_id_lookup,
             additional_registration_ids,
         )
         if not registration_ids:
             return self.get_default_send_message_response()
         responses: List[messaging.SendResponse] = []
         for i in range(0, len(registration_ids), MAX_MESSAGES_PER_BATCH):
             messages = [
-                self._prepare_message(m, t)
-                for m, t in zip(
-                    repeat(message, MAX_MESSAGES_PER_BATCH),
-                    registration_ids[i : i + MAX_MESSAGES_PER_BATCH],
-                )
+                self._prepare_message(message, token)
+                for token in registration_ids[i : i + MAX_MESSAGES_PER_BATCH]
             ]
             responses.extend(
-                messaging.send_all(messages, **more_send_message_kwargs).responses
+                messaging.send_all(
+                    messages, app=app, **more_send_message_kwargs
+                ).responses
             )
         return FirebaseResponseDict(
             response=messaging.BatchResponse(responses),
             registration_ids_sent=registration_ids,
             deactivated_registration_ids=self.deactivate_devices_with_error_results(
                 registration_ids, responses
             ),
@@ -213,31 +210,32 @@
 
     def handle_topic_subscription(
         self,
         should_subscribe: bool,
         topic: str,
         skip_registration_id_lookup: bool = False,
         additional_registration_ids: Sequence[str] = None,
+        app: "firebase_admin.App" = SETTINGS["DEFAULT_FIREBASE_APP"],
         **more_subscribe_kwargs,
     ) -> FirebaseResponseDict:
         """
         Subscribes or Unsubscribes filtered and/or given tokens/registration_ids
         to given topic.
 
         :param should_subscribe: whether to have these users subscribe (True) or
         unsubscribe to a topic (False).
         :param topic: Name of the topic to subscribe to. May contain the ``/topics/``
         prefix.
         :param skip_registration_id_lookup: skips the QuerySet lookup and solely uses
         the list of IDs from additional_registration_ids
         :param additional_registration_ids: specific registration_ids to add to the
+        :param app: firebase_admin.App. Specify a specific app to use
         QuerySet lookup
         :param more_subscribe_kwargs: Parameters for
         ``firebase.messaging.subscribe_to_topic()``
-        - app: firebase_admin.App. Specify a specific app to use
         If there are any new parameters, you can still specify them here.
 
         :raises FirebaseError
         :returns FirebaseResponseDict
         """
         registration_ids = self.get_registration_ids(
             skip_registration_id_lookup,
@@ -245,102 +243,115 @@
         )
         if not registration_ids:
             return self.get_default_topic_response()
         response = (
             messaging.subscribe_to_topic
             if should_subscribe
             else messaging.unsubscribe_from_topic
-        )(registration_ids, topic, **more_subscribe_kwargs)
+        )(registration_ids, topic, app=app, **more_subscribe_kwargs)
         return FirebaseResponseDict(
             response=response,
             registration_ids_sent=registration_ids,
             deactivated_registration_ids=self.deactivate_devices_with_error_results(
                 registration_ids, response.errors
             ),
         )
 
 
 FCMDeviceManager = _FCMDeviceManager.from_queryset(FCMDeviceQuerySet)
 
 
-class AbstractFCMDevice(Device):
-    DEVICE_TYPES = (("ios", "ios"), ("android", "android"), ("web", "web"))
+class DeviceType(models.TextChoices):
+    IOS = "ios", "ios"
+    ANDROID = "android", "android"
+    WEB = "web", "web"
+
 
+class AbstractFCMDevice(Device):
     device_id = models.CharField(
         verbose_name=_("Device ID"),
         blank=True,
         null=True,
         db_index=True,
         help_text=_("Unique device identifier"),
         max_length=255,
     )
-    registration_id = models.TextField(verbose_name=_("Registration token"))
-    type = models.CharField(choices=DEVICE_TYPES, max_length=10)
+    registration_id = models.TextField(
+        verbose_name=_("Registration token"),
+        unique=True,
+    )
+    type = models.CharField(choices=DeviceType.choices, max_length=10)
     objects: "FCMDeviceQuerySet" = FCMDeviceManager()
 
     class Meta:
         abstract = True
         verbose_name = _("FCM device")
+        indexes = [
+            models.Index(fields=["registration_id", "user"]),
+        ]
 
     def send_message(
         self,
         message: messaging.Message,
+        app: "firebase_admin.App" = SETTINGS["DEFAULT_FIREBASE_APP"],
         **more_send_message_kwargs,
     ) -> Union[Optional[messaging.SendResponse], FirebaseError]:
         """
         Send single message. The message's token should be blank (and will be
         overridden if not). Responds with message ID string.
 
         :param message: firebase.messaging.Message. If `message` includes a token/id, it
         will be overridden.
+        :param app: firebase_admin.App. Specify a specific app to use
         :param more_send_message_kwargs: Parameters for firebase.messaging.send_all()
         - dry_run: bool. Whether to actually send the notification to the device
-        - app: firebase_admin.App. Specify a specific app to use
         If there are any new parameters, you can still specify them here.
 
         :raises FirebaseError
         :returns messaging.SendResponse or FirebaseError if the device was
         deactivated due to an error.
         """
         message.token = self.registration_id
         try:
             return messaging.SendResponse(
-                {"name": messaging.send(message, **more_send_message_kwargs)}, None
+                {"name": messaging.send(message, app=app, **more_send_message_kwargs)},
+                None,
             )
         except FirebaseError as e:
             self.deactivate_devices_with_error_result(self.registration_id, e)
             return e
 
     def handle_topic_subscription(
         self,
         should_subscribe: bool,
         topic: str,
+        app: "firebase_admin.App" = SETTINGS["DEFAULT_FIREBASE_APP"],
         **more_subscribe_kwargs,
     ) -> FirebaseResponseDict:
         """
         Subscribes or Unsubscribes based on instance's registration_id
 
         :param should_subscribe: whether to have these users subscribe (True) or
         unsubscribe to a topic (False).
         :param topic: Name of the topic to subscribe to. May contain the ``/topics/``
         prefix.
+        :param app: firebase_admin.App. Specify a specific app to use
         :param more_subscribe_kwargs: Parameters for
         ``firebase.messaging.subscribe_to_topic()``
-        - app: firebase_admin.App. Specify a specific app to use
         If there are any new parameters, you can still specify them here.
 
         :raises FirebaseError
         :returns FirebaseResponseDict
         """
         _r_ids = [self.registration_id]
         response = (
             messaging.subscribe_to_topic
             if should_subscribe
             else messaging.unsubscribe_from_topic
-        )(_r_ids, topic, **more_subscribe_kwargs)
+        )(_r_ids, topic, app=app, **more_subscribe_kwargs)
         return FirebaseResponseDict(
             response=response,
             registration_ids_sent=_r_ids,
             deactivated_registration_ids=type(
                 self
             ).objects.deactivate_devices_with_error_results(_r_ids, response.errors),
         )
@@ -353,23 +364,29 @@
             [registration_id], [messaging.SendResponse({"name": name}, firebase_exc)]
         )
 
     @staticmethod
     def send_topic_message(
         message: messaging.Message,
         topic_name: str,
+        app: "firebase_admin.App" = SETTINGS["DEFAULT_FIREBASE_APP"],
         **more_send_message_kwargs,
     ) -> Union[Optional[messaging.SendResponse], FirebaseError]:
         message.topic = topic_name
 
         try:
             return messaging.SendResponse(
-                {"name": messaging.send(message, **more_send_message_kwargs)}, None
+                {"name": messaging.send(message, app=app, **more_send_message_kwargs)},
+                None,
             )
         except FirebaseError as e:
             return e
 
 
 class FCMDevice(AbstractFCMDevice):
     class Meta:
         verbose_name = _("FCM device")
         verbose_name_plural = _("FCM devices")
+
+        indexes = [
+            models.Index(fields=["registration_id", "user"]),
+        ]
```

### Comparing `fcm-django-1.0.9/fcm_django/settings.py` & `fcm-django-2.0.0/fcm_django/settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from django.conf import settings
 from django.utils.translation import gettext_lazy as _
 
 FCM_DJANGO_SETTINGS = getattr(settings, "FCM_DJANGO_SETTINGS", {})
 
 # FCM
+FCM_DJANGO_SETTINGS.setdefault("DEFAULT_FIREBASE_APP", None)
 FCM_DJANGO_SETTINGS.setdefault("APP_VERBOSE_NAME", _("FCM Django"))
 FCM_DJANGO_SETTINGS.setdefault("ONE_DEVICE_PER_USER", False)
 FCM_DJANGO_SETTINGS.setdefault("DELETE_INACTIVE_DEVICES", False)
-FCM_DJANGO_SETTINGS.setdefault("UPDATE_ON_DUPLICATE_REG_ID", False)
+FCM_DJANGO_SETTINGS.setdefault(
+    "UPDATE_ON_DUPLICATE_REG_ID", True
+)  # TODO: remove this setting as it should always be True
 
 # User model
 FCM_DJANGO_SETTINGS.setdefault("USER_MODEL", settings.AUTH_USER_MODEL)
 
 FCM_DJANGO_SETTINGS.setdefault(
     "ERRORS",
     {
```

### Comparing `fcm-django-1.0.9/fcm_django.egg-info/SOURCES.txt` & `fcm-django-2.0.0/fcm_django.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -21,8 +21,11 @@
 fcm_django/migrations/0002_auto_20160808_1645.py
 fcm_django/migrations/0003_auto_20170313_1314.py
 fcm_django/migrations/0004_auto_20181128_1642.py
 fcm_django/migrations/0005_auto_20170808_1145.py
 fcm_django/migrations/0006_auto_20210802_1140.py
 fcm_django/migrations/0007_auto_20211001_1440.py
 fcm_django/migrations/0008_auto_20211224_1205.py
+fcm_django/migrations/0009_alter_fcmdevice_user.py
+fcm_django/migrations/0010_unique_registration_id.py
+fcm_django/migrations/0011_fcmdevice_fcm_django_registration_id_user_id_idx.py
 fcm_django/migrations/__init__.py
```

### Comparing `fcm-django-1.0.9/setup.py` & `fcm-django-2.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,27 +14,29 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: System :: Networking",
 ]
 
 setup(
     name="fcm-django",
     packages=[
         "fcm_django",
         "fcm_django/api",
         "fcm_django/migrations",
     ],
-    python_requires=">=3",
-    install_requires=["firebase-admin>=5,<6", "Django"],
+    python_requires=">=3.7",
+    install_requires=["firebase-admin>=5,<7", "Django"],
     author=fcm_django.__author__,
     author_email=fcm_django.__email__,
     classifiers=CLASSIFIERS,
     description="Send push notifications to mobile devices & browsers through "
     "FCM in Django.",
     download_url="https://github.com/xtrinch/fcm-django/tarball/master",
     long_description="",
```

