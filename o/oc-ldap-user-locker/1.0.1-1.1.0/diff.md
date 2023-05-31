# Comparing `tmp/oc_ldap_user_locker-1.0.1-py3-none-any.whl.zip` & `tmp/oc_ldap_user_locker-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 8954 bytes, number of entries: 8
--rw-r--r--  2.0 unx        0 b- defN 23-May-22 12:14 oc_ldap_user_locker/__init__.py
--rw-r--r--  2.0 unx      528 b- defN 23-May-22 12:14 oc_ldap_user_locker/__main__.py
--rw-r--r--  2.0 unx    10454 b- defN 23-May-22 12:14 oc_ldap_user_locker/locker.py
--rw-r--r--  2.0 unx    11357 b- defN 23-May-22 12:14 oc_ldap_user_locker-1.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      249 b- defN 23-May-22 12:14 oc_ldap_user_locker-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-22 12:14 oc_ldap_user_locker-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 23-May-22 12:14 oc_ldap_user_locker-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      705 b- defN 23-May-22 12:14 oc_ldap_user_locker-1.0.1.dist-info/RECORD
-8 files, 23405 bytes uncompressed, 7704 bytes compressed:  67.1%
+Zip file size: 12049 bytes, number of entries: 9
+-rw-r--r--  2.0 unx        0 b- defN 23-May-31 06:55 oc_ldap_user_locker/__init__.py
+-rw-r--r--  2.0 unx      528 b- defN 23-May-31 06:55 oc_ldap_user_locker/__main__.py
+-rw-r--r--  2.0 unx    15442 b- defN 23-May-31 06:55 oc_ldap_user_locker/locker.py
+-rw-r--r--  2.0 unx     5441 b- defN 23-May-31 06:55 oc_ldap_user_locker/mailer.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-31 06:55 oc_ldap_user_locker-1.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      274 b- defN 23-May-31 06:55 oc_ldap_user_locker-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-31 06:55 oc_ldap_user_locker-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-May-31 06:55 oc_ldap_user_locker-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      791 b- defN 23-May-31 06:55 oc_ldap_user_locker-1.1.0.dist-info/RECORD
+9 files, 33945 bytes uncompressed, 10665 bytes compressed:  68.6%
```

## zipnote {}

```diff
@@ -3,23 +3,26 @@
 
 Filename: oc_ldap_user_locker/__main__.py
 Comment: 
 
 Filename: oc_ldap_user_locker/locker.py
 Comment: 
 
-Filename: oc_ldap_user_locker-1.0.1.dist-info/LICENSE
+Filename: oc_ldap_user_locker/mailer.py
 Comment: 
 
-Filename: oc_ldap_user_locker-1.0.1.dist-info/METADATA
+Filename: oc_ldap_user_locker-1.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: oc_ldap_user_locker-1.0.1.dist-info/WHEEL
+Filename: oc_ldap_user_locker-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: oc_ldap_user_locker-1.0.1.dist-info/top_level.txt
+Filename: oc_ldap_user_locker-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: oc_ldap_user_locker-1.0.1.dist-info/RECORD
+Filename: oc_ldap_user_locker-1.1.0.dist-info/top_level.txt
+Comment: 
+
+Filename: oc_ldap_user_locker-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## oc_ldap_user_locker/locker.py

```diff
@@ -1,30 +1,68 @@
 import json
 import os
 import logging
 from oc_ldap_client.oc_ldap_objects import OcLdapUserCat, OcLdapUserRecord
 import re
 import datetime
 from copy import copy
+from .mailer import LockMailer
 
 class OcLdapUserLocker:
     def __init__(self, config_path):
         """
         Initialization
         :param str config_path: path to JSON locker configuration
         """
         if not config_path:
             raise ValueError("No configuration path provided")
 
         config_path = os.path.abspath(config_path)
         logging.info("Configuration path: '%s'" % config_path)
+        self._config_path = config_path
 
         with open(config_path, mode='rt') as _fl_in:
             self.config = json.load(_fl_in)
 
+        self._check_ldap_params()
+        self._mailer = None
+
+    def _check_ldap_params(self):
+        """
+        Check LDAP parameters are set
+        update them from environment if not
+        """
+        _ldap_params = self.config.get("LDAP")
+
+        if not _ldap_params:
+            logging.debug("LDAP configuration missing, trying to create it from environment")
+            self.config["LDAP"] = dict()
+            _ldap_params = self.config.get("LDAP")
+
+        _ldap_env = {
+                "url": "LDAP_URL",
+                "user_cert": "LDAP_TLS_CERT",
+                "user_key": "LDAP_TLS_KEY",
+                "ca_chain": "LDAP_TLS_CACERT",
+                "baseDn": "LDAP_BASE_DN"}
+
+        for _key in _ldap_env.keys():
+            _value = _ldap_params.get(_key) or os.getenv(_ldap_env.get(_key))
+
+            if not _value:
+                raise ValueError("%s not set", _ldap_env.get(_key))
+
+            if _key in ["user_cert", "ca_chain", "user_key"]:
+                # this is a path to file, make sure it is absolute
+                if not os.path.isabs(_value):
+                    _value = os.path.join(os.path.dirname(self._config_path), _value)
+
+            logging.debug("%s: '%s'" % (_ldap_env.get(_key), _value))
+            self.config["LDAP"][_key] = _value
+
     def _compare_attribute(self, values, match_conf):
         """
         Compare a values to match configuration
         :param list values: values to compare
         :param dict match_conf: configuration dictionary
         """
         if not values:
@@ -192,54 +230,137 @@
         # this will raise an exception if any of mandatory parameter is missing or has wrong type
         logging.info("User '%s' is valid for '%d' days, time attributes: '%s'" % (
             _user_rec.get_attribute('cn'), _conf['days_valid'], ':'.join(_conf['time_attributes'])))
 
         # now check the time attributes specified in the conf and find out the nearest one
         # note that 'tzinfo' is to be discarged because of possible datetime exception while
         #   subtracting them
-        _lock = self._check_lock_conf(_user_rec, _conf['days_valid'], _conf['time_attributes'])
+        _lock_date = self._get_account_lock_date(_user_rec, _conf['days_valid'], _conf['time_attributes'])
 
-        if not _lock:
+        if not _lock_date:
+            # should never happen
+            logging.debug("Account '%s' is not to be locked ever", _user_rec.get_attribute('cn'))
             return
 
+        logging.debug("Account lock date for '%s': '%s'" % (
+            _user_rec.get_attribute('cn'), _lock_date.isoformat(sep=" ")))
+
+        _days_before_lock = self._get_days_before_lock(_lock_date)
+        logging.debug("Days before lock account '%s': %d" % (
+            _user_rec.get_attribute('cn'), _days_before_lock))
+
+        # check lock e-mail notifications
+        self._check_lock_notifications(
+                _user_rec, _conf, lock_date=_lock_date, days_before_lock=_days_before_lock)
+
+        if _days_before_lock > 0:
+            logging.debug("Is not the time to lock '%s', returning" % _user_rec.get_attribute('cn'))
+            return
+
+        logging.info("Locking '%s', days: '%d'" % (
+            _user_rec.get_attribute('cn'), _days_before_lock))
+
         _user_rec.lock()
         ldap_c.put_record(_user_rec)
+       
+    def _check_lock_notifications(self, user_rec, conf, lock_date, days_before_lock):
+        """
+        Check if user is to be notified about account locking
+        Send mail notifications is so
+        :param OcLdapRecord user_rec: user record from LDAP catalogue
+        :param dict conf: configuration to check agianst
+        :param datetime.datetime lock_date: date when account will be locked
+        :param int days_before_lock: days left for the date when account will be locked
+        """
+        # if any of argumets absent then we should have an exception.
+        # so do not check
+
+        if not conf.get("lock_notifications"):
+            logging.debug("Notifications are not configured for '%s'" % user_rec.get_attribute('cn'))
+            return
+
+        if not user_rec.get_attribute("mail"):
+            logging.debug("User '%s' nas no mail, nothing to do" % user_rec.get_attribute('cn')) 
+            return
+
+        # if 'days_before_lock' is negative - use zero-value notification since account is to be locked now
+        if days_before_lock < 0:
+            days_before_lock = 0
+
+        # if no suitable configuration for 'days_before_lock' - skip
+        _conf = list(filter(lambda x: x.get("days_before") == days_before_lock, conf.get("lock_notifications")))
+
+        if not _conf:
+            #empty list?
+            logging.debug("No notification for '%s' in %d days before lock" %
+                    (user_rec.get_attribute('cn'), days_before_lock))
+            return
+        
+        _conf = _conf.pop()
+
+        if not self._mailer:
+            self._mailer = LockMailer(self.config.get("SMTP") or dict(), os.path.dirname(self._config_path))
+
+        # filter substitutes for mail template
+        _substitutes = dict((_k, user_rec.get_attribute(_k)) for _k in [
+            'cn', 'givenName', 'sn', 'displayName'])
 
-    def _check_lock_conf(self, user_rec, days_valid, time_attributes):
+        _substitutes.update({
+                "lockDate": lock_date.strftime("%Y-%d-%m"),
+                "lockDays": str(days_before_lock)})
+
+        self._mailer.send_notification(user_rec.get_attribute('mail'), _conf.get("template"), _substitutes)
+
+
+    def _get_days_before_lock(self, lock_date):
         """
         Check if user is to be locked or not
+        :param datetime.datetime lock_date: the date account should be locked at, without timezone, not None
+        :reurn int: days before lock, negative if 'after' lock
+        """
+        _today = datetime.datetime.now()
+        _today = _today.replace(tzinfo=None)
+        _diff = lock_date - _today
+
+        return _diff.days
+
+    def _get_account_lock_date(self, user_rec, days_valid, time_attributes):
+        """
+        Calculate account lock date basing on current 'time_attribute' values
         :param OcLdapRecord user_rec: record from LDAP
         :param int days_valid: how many days record is valid
         :param list time_attributes: list of time attributes to check (strings)
-        :return bool: True if user is to be locked
+        :return datetime.datetime: the date and time account should be locked; 'None' means 'never'
         """
-        _today = datetime.datetime.now()
-        _today = _today.replace(tzinfo=None)
+
+        _result = None
+        _append = datetime.timedelta(days=days_valid)
 
         for _time_attrib in time_attributes:
             # note that list of time attributes is not supported, so assuming it is a datetime.datetime value
             # note that we are doing 'copy' - to get rid of record attribute get changed and then raise LDAP error
             #   on saving it
             _time_value = copy(user_rec.get_attribute(_time_attrib))
 
             # time value may be "None" - assuming attribute is not set and skipping comparison
             if not _time_value:
                 continue
 
-            # if any of attribute is 'less' than 'days' - do not lock an account
+            # appending 'days'
             _time_value = _time_value.replace(tzinfo=None)
-            _diff = _today - _time_value
+            _time_value = _time_value + _append
 
-            if _diff.days < days_valid:
-                logging.info("Not locking: '%s'" % user_rec.get_attribute('cn'))
-                return False
+            # we have to choose the value in the farest future of possibles
+            if not _result or _result < _time_value:
+                _result = _time_value
 
-        logging.info("Locking '%s'" % user_rec.get_attribute('cn'))
+        logging.debug("Locking date for '%s': '%s'" % (user_rec.get_attribute('cn'),
+            'None' if not _result else _result.isoformat(sep=' ')))
 
-        return True
+        return _result
 
     def run(self):
         """
         Run the process
         """
         logging.debug("Started")
```

## Comparing `oc_ldap_user_locker-1.0.1.dist-info/LICENSE` & `oc_ldap_user_locker-1.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `oc_ldap_user_locker-1.0.1.dist-info/RECORD` & `oc_ldap_user_locker-1.1.0.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 oc_ldap_user_locker/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 oc_ldap_user_locker/__main__.py,sha256=rg29B6Ou1-_XqIdqt0AFuRSBYAt96KmoELjydZvmPQc,528
-oc_ldap_user_locker/locker.py,sha256=UVkNb77hglbdKjr9KkCYL2uDLIVkar29qxThxy8VFTQ,10454
-oc_ldap_user_locker-1.0.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-oc_ldap_user_locker-1.0.1.dist-info/METADATA,sha256=oRA2XuzMNWRl6eH1clIYqWMqeOrBMoJ7cqsa_Ypmbew,249
-oc_ldap_user_locker-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-oc_ldap_user_locker-1.0.1.dist-info/top_level.txt,sha256=VgvLdN22xrjMzdP18fGULsr4ergDZbPZBI4GHD62ep0,20
-oc_ldap_user_locker-1.0.1.dist-info/RECORD,,
+oc_ldap_user_locker/locker.py,sha256=ZaX00EpVnF_nM2co7SpNpgH0J1F3Cj3z5a6dx3GWCJ8,15442
+oc_ldap_user_locker/mailer.py,sha256=qDAdc4Eetxuj0g8xhzuc_Qk7KX_VhfPWJkEw7g5XsSc,5441
+oc_ldap_user_locker-1.1.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+oc_ldap_user_locker-1.1.0.dist-info/METADATA,sha256=Kcikg_1f86LE8-Z-j6eX9MNsGj_wAA0Ghu-6vM3wwPk,274
+oc_ldap_user_locker-1.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+oc_ldap_user_locker-1.1.0.dist-info/top_level.txt,sha256=VgvLdN22xrjMzdP18fGULsr4ergDZbPZBI4GHD62ep0,20
+oc_ldap_user_locker-1.1.0.dist-info/RECORD,,
```

