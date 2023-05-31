# Comparing `tmp/Flask-Identity-1.0.3.dev7.tar.gz` & `tmp/flask_identity-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-Identity-1.0.3.dev7.tar", last modified: Thu Mar 11 08:17:21 2021, max compression
+gzip compressed data, was "flask_identity-1.0.4.tar", max compression
```

## Comparing `Flask-Identity-1.0.3.dev7.tar` & `flask_identity-1.0.4.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0     1119 2019-11-23 14:58:58.000000 Flask-Identity-1.0.3.dev7/LICENSE.rst
--rw-r--r--   0        0        0     2726 2021-02-20 10:02:41.787082 Flask-Identity-1.0.3.dev7/README.rst
--rw-r--r--   0        0        0      909 2021-02-18 03:53:54.605803 Flask-Identity-1.0.3.dev7/flask_identity/__init__.py
--rw-r--r--   0        0        0     2248 2021-02-07 13:35:31.274109 Flask-Identity-1.0.3.dev7/flask_identity/_hash_context.py
--rw-r--r--   0        0        0     3350 2021-02-10 03:41:26.536293 Flask-Identity-1.0.3.dev7/flask_identity/_token_context.py
--rw-r--r--   0        0        0     1247 2021-03-08 08:09:33.712571 Flask-Identity-1.0.3.dev7/flask_identity/babels.py
--rw-r--r--   0        0        0      844 2021-02-07 13:26:03.413234 Flask-Identity-1.0.3.dev7/flask_identity/compats.py
--rw-r--r--   0        0        0     8135 2021-03-08 06:19:53.532849 Flask-Identity-1.0.3.dev7/flask_identity/config.py
--rw-r--r--   0        0        0    18518 2021-03-08 06:25:49.577892 Flask-Identity-1.0.3.dev7/flask_identity/core.py
--rw-r--r--   0        0        0    14016 2021-02-24 05:52:01.765121 Flask-Identity-1.0.3.dev7/flask_identity/datastore.py
--rw-r--r--   0        0        0     7834 2021-02-24 07:52:30.800230 Flask-Identity-1.0.3.dev7/flask_identity/decorators.py
--rw-r--r--   0        0        0     3879 2021-03-11 07:42:14.653918 Flask-Identity-1.0.3.dev7/flask_identity/forms.py
--rw-r--r--   0        0        0     5243 2021-03-08 05:52:09.768255 Flask-Identity-1.0.3.dev7/flask_identity/mixins.py
--rw-r--r--   0        0        0      823 2021-03-08 07:06:51.986700 Flask-Identity-1.0.3.dev7/flask_identity/translations/en_US/LC_MESSAGES/flask_identity.mo
--rw-r--r--   0        0        0     1269 2021-03-08 07:06:29.668851 Flask-Identity-1.0.3.dev7/flask_identity/translations/en_US/LC_MESSAGES/flask_identity.po
--rw-r--r--   0        0        0     1076 2021-03-08 06:35:07.753539 Flask-Identity-1.0.3.dev7/flask_identity/translations/flask_identity.pot
--rw-r--r--   0        0        0      814 2021-03-08 07:06:51.995584 Flask-Identity-1.0.3.dev7/flask_identity/translations/zh_Hans_CN/LC_MESSAGES/flask_identity.mo
--rw-r--r--   0        0        0     1264 2021-03-08 07:04:04.314977 Flask-Identity-1.0.3.dev7/flask_identity/translations/zh_Hans_CN/LC_MESSAGES/flask_identity.po
--rw-r--r--   0        0        0    10114 2021-03-08 06:10:29.288586 Flask-Identity-1.0.3.dev7/flask_identity/utils.py
--rw-r--r--   0        0        0     6207 2021-02-24 08:01:10.218490 Flask-Identity-1.0.3.dev7/flask_identity/views.py
--rw-r--r--   0        0        0     1677 2021-03-11 08:17:17.889541 Flask-Identity-1.0.3.dev7/pyproject.toml
--rw-r--r--   0        0        0     3849 2021-03-11 08:17:21.552276 Flask-Identity-1.0.3.dev7/setup.py
--rw-r--r--   0        0        0     4394 2021-03-11 08:17:21.552621 Flask-Identity-1.0.3.dev7/PKG-INFO
+-rw-r--r--   0        0        0     1119 2023-05-29 12:41:30.306646 flask_identity-1.0.4/LICENSE.rst
+-rw-r--r--   0        0        0     2604 2023-05-29 12:45:53.285419 flask_identity-1.0.4/README.rst
+-rw-r--r--   0        0        0      905 2023-05-31 01:12:45.393303 flask_identity-1.0.4/flask_identity/__init__.py
+-rw-r--r--   0        0        0     2244 2023-05-31 01:12:45.386633 flask_identity-1.0.4/flask_identity/_hash_context.py
+-rw-r--r--   0        0        0     3346 2023-05-31 01:12:45.405665 flask_identity-1.0.4/flask_identity/_token_context.py
+-rw-r--r--   0        0        0     1243 2023-05-31 01:12:45.379734 flask_identity-1.0.4/flask_identity/babels.py
+-rw-r--r--   0        0        0      840 2023-05-31 01:12:45.404196 flask_identity-1.0.4/flask_identity/compats.py
+-rw-r--r--   0        0        0     9850 2023-05-31 02:44:57.794012 flask_identity-1.0.4/flask_identity/config.py
+-rw-r--r--   0        0        0    18080 2023-05-31 01:45:50.580150 flask_identity-1.0.4/flask_identity/core.py
+-rw-r--r--   0        0        0    14012 2023-05-31 01:12:45.398245 flask_identity-1.0.4/flask_identity/datastore.py
+-rw-r--r--   0        0        0     7829 2023-05-31 03:09:52.352538 flask_identity-1.0.4/flask_identity/decorators.py
+-rw-r--r--   0        0        0     3898 2023-05-31 01:48:31.110407 flask_identity-1.0.4/flask_identity/forms.py
+-rw-r--r--   0        0        0     5239 2023-05-31 01:12:45.344624 flask_identity-1.0.4/flask_identity/mixins.py
+-rw-r--r--   0        0        0      823 2023-05-29 12:41:30.313443 flask_identity-1.0.4/flask_identity/translations/en_US/LC_MESSAGES/flask_identity.mo
+-rw-r--r--   0        0        0     1269 2023-05-29 12:41:30.313585 flask_identity-1.0.4/flask_identity/translations/en_US/LC_MESSAGES/flask_identity.po
+-rw-r--r--   0        0        0     1076 2023-05-29 12:41:30.313677 flask_identity-1.0.4/flask_identity/translations/flask_identity.pot
+-rw-r--r--   0        0        0      814 2023-05-29 12:41:30.313893 flask_identity-1.0.4/flask_identity/translations/zh_hans_CN/LC_MESSAGES/flask_identity.mo
+-rw-r--r--   0        0        0     1264 2023-05-29 12:41:30.314002 flask_identity-1.0.4/flask_identity/translations/zh_hans_CN/LC_MESSAGES/flask_identity.po
+-rw-r--r--   0        0        0    10110 2023-05-31 01:12:45.347764 flask_identity-1.0.4/flask_identity/utils.py
+-rw-r--r--   0        0        0     6203 2023-05-31 01:12:45.382128 flask_identity-1.0.4/flask_identity/views.py
+-rw-r--r--   0        0        0     1743 2023-05-31 03:41:29.586482 flask_identity-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4219 1970-01-01 00:00:00.000000 flask_identity-1.0.4/PKG-INFO
```

### Comparing `Flask-Identity-1.0.3.dev7/LICENSE.rst` & `flask_identity-1.0.4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `Flask-Identity-1.0.3.dev7/README.rst` & `flask_identity-1.0.4/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -48,16 +48,15 @@
 some codes are direct merged from other successful open-source libraries:
 
 * `Flask-Login <https://flask-login.readthedocs.org/en/latest/>`_
 * `Flask-Security <https://flask-security.readthedocs.org/en/latest/>`_
 
 Contributing
 ++++++++++++
-Issues and pull requests are welcome. Other maintainers are also welcome. Unlike
-the original Flask-Security - issue pull requests against the *master* branch.
+Issues and pull requests are welcome.
 Please consult these `contributing`_ guidelines.
 
 .. _contributing: https://github.com/solardiax/flask-identity/blob/master/CONTRIBUTING.rst
 
 Installing
 ----------
 Install and update using `pip <https://pip.pypa.io/en/stable/quickstart/>`_:
```

### Comparing `Flask-Identity-1.0.3.dev7/flask_identity/__init__.py` & `flask_identity-1.0.4/flask_identity/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
     Flask-Identity
     ~~~~~~~~~~~~~~~~~~~
     A lightweight Identity Manager for Flask
 
     :author: solardiax <solardiax@hotmail.com>
     :copyright: (c) 2020 by DreamEx Works.
-    :license: GPL-3.0, see LICENSE for more details.
+    :license: MIT, see LICENSE for more details.
 """
 
 from .core import IdentityManager
 from .decorators import auth_required, login_required, roles_accepted, roles_required
 from .mixins import UserMixin, AnonymousUserMixin, RoleMixin
 from .utils import hash_password, verify_password, login_user, logout_user, current_user, current_identity
 from .views import url_for_identity
```

### Comparing `Flask-Identity-1.0.3.dev7/flask_identity/_hash_context.py` & `flask_identity-1.0.4/flask_identity/_hash_context.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
     identity._hash_context
     ~~~~~~~~~~~~~~~~~~~
     Hash Context of Flask-Identity
 
     :author: solardiax <solardiax@hotmail.com>
     :copyright: (c) 2020 by DreamEx Works.
-    :license: GPL-3.0, see LICENSE for more details.
+    :license: MIT, see LICENSE for more details.
 """
 
 
 from passlib.context import CryptContext
 
 
 class HashContext(object):
```

### Comparing `Flask-Identity-1.0.3.dev7/flask_identity/_token_context.py` & `flask_identity-1.0.4/flask_identity/_token_context.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
     identity._token_context
     ~~~~~~~~~~~~~~~~~~~
     Token Context of Flask-Identity
 
     :author: solardiax <solardiax@hotmail.com>
     :copyright: (c) 2020 by DreamEx Works.
-    :license: GPL-3.0, see LICENSE for more details.
+    :license: MIT, see LICENSE for more details.
 """
 
 import base64
 import json
 from datetime import timedelta
 from cryptography.fernet import Fernet
```

### Comparing `Flask-Identity-1.0.3.dev7/flask_identity/babels.py` & `flask_identity-1.0.4/flask_identity/babels.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
     identity.babel
     ~~~~~~~~~~~~~~~~~~~
     I18N support modules of Flask-Identity
 
     :author: solardiax <solardiax@hotmail.com>
     :copyright: (c) 2020 by DreamEx Works.
-    :license: GPL-3.0, see LICENSE for more details.
+    :license: MIT, see LICENSE for more details.
 """
 
 from flask_babel import Domain
 from babel.support import LazyProxy
 from wtforms.i18n import messages_path
 
 from .utils import config_value
```

### Comparing `Flask-Identity-1.0.3.dev7/flask_identity/compats.py` & `flask_identity-1.0.4/flask_identity/compats.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
     identity.compats
     ~~~~~~~~~~~~~~~~~~~
     Compatibility modules of Flask-Identity
 
     :author: solardiax <solardiax@hotmail.com>
     :copyright: (c) 2020 by DreamEx Works.
-    :license: GPL-3.0, see LICENSE for more details.
+    :license: MIT, see LICENSE for more details.
 """
 
 import flask
 
 if "quart." in flask.__name__ or hasattr(flask, "_quart_patched"):  # pragma: no cover
     is_quart = True
 else:
```

### Comparing `Flask-Identity-1.0.3.dev7/flask_identity/config.py` & `flask_identity-1.0.4/flask_identity/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
     identity.config
     ~~~~~~~~~~~~~~~~~~~
     Default configuration of Flask-Identity
 
     :author: solardiax <solardiax@hotmail.com>
     :copyright: (c) 2020 by DreamEx Works.
-    :license: GPL-3.0, see LICENSE for more details.
+    :license: MIT, see LICENSE for more details.
 """
 
 import pkg_resources
 from datetime import timedelta
 
 default_config = {
     #: Specifies the view to redirect to if a user attempts to access a URL/endpoint that they do
@@ -216,8 +216,51 @@
     #: Specifies the name for domain used for translations.
     #: Default: ``'flask_identity'``.
     'I18N_DOMAIN': 'flask_identity',
 
     #: Specifies the directory containing the MO files used for translations.
     #: Default: ``[PATH_LIB]/flask_identity/translations``.
     'I18N_DIRNAME': pkg_resources.resource_filename('flask_identity', 'translations'),
+
+    #: Flask-WTF: Set to False to disable all CSRF protection.
+    #: Default is ``True``
+    'WTF_CSRF_ENABLED': True,
+
+    #: Flask-WTF: When using the CSRF protection extension, this controls whether every view is protected by default.
+    #: Default: ``True``
+    'WTF_CSRF_CHECK_DEFAULT': True,
+
+    #: Flask-WTF: Random data for generating secure tokens. If this is not set then SECRET_KEY is used.
+    #: Default: ``None``
+    'WTF_CSRF_SECRET_KEY': None,
+
+    #: Flask-WTF: HTTP methods to protect from CSRF.
+    #: Default is ``{'POST', 'PUT', 'PATCH', 'DELETE'}``
+    'WTF_CSRF_METHODS': {'POST', 'PUT', 'PATCH', 'DELETE'},
+
+    #: Flask-WTF: Name of the form field and session key that holds the CSRF token.
+    #: Default: ``'csrf_token'``
+    'WTF_CSRF_FIELD_NAME': 'csrf_token',
+
+    #: Flask-WTF: HTTP headers to search for CSRF token when it is not provided in the form.
+    #: Default: ``['X-CSRFToken', 'X-CSRF-Token']``
+    'WTF_CSRF_HEADERS': ['X-CSRFToken', 'X-CSRF-Token'],
+
+    #: Flask-WTF: Max age in seconds for CSRF tokens.
+    #: If set to None, the CSRF token is valid for the life of the session.
+    #: Default: ``3600``
+    'WTF_CSRF_TIME_LIMIT': 3600,
+
+    #: Flask-WTF: Whether to enforce the same origin policy by checking that the referrer matches the host.
+    #: Only applies to HTTPS requests.
+    #: Default: ``True``
+    'WTF_CSRF_SSL_STRICT': True,
+
+    #: Flask-WTF: Set to False to disable Flask-Babel I18N support.
+    #: Also set to False if you want to use WTForms’s built-in messages directly.
+    #: Default: ``True``
+    'WTF_I18N_ENABLED': True,
+
+    #: Specifies the endpoint to ignore CSRF check.
+    #: Default: ``[]``
+    'WTF_CSRF_IGNORE_UNAUTH_ENDPOINTS': []
 }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Flask-Identity-1.0.3.dev7/flask_identity/core.py` & `flask_identity-1.0.4/flask_identity/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
     identity.core
     ~~~~~~~~~~~~~~~~~~~
     The core methods of Flask-Identity
 
     :author: solardiax <solardiax@hotmail.com>
     :copyright: (c) 2020 by DreamEx Works.
-    :license: GPL-3.0, see LICENSE for more details.
+    :license: MIT, see LICENSE for more details.
 """
 
 import logging
 
 from datetime import datetime, timedelta
 from hashlib import sha512
 from inspect import isclass
@@ -171,33 +171,25 @@
         self.app = app
 
         if register_blueprint is None:
             register_blueprint = self._config.get('BLUEPRINT_ENABLED', True)
             self._register_blueprint = register_blueprint
 
         if register_blueprint:
-            create_blueprint(self, __name__, app.json_encoder)
+            create_blueprint(self, __name__, app.json)
 
         self._i18n_domain = get_i18n_domain(app)
 
-        @app.before_first_request
-        def _register_i18n():
-            # This is only not registered if Flask-Babel isn't installed...
-            if "_" not in app.jinja_env.globals:
-                current_app.jinja_env.globals["_"] = self._i18n_domain.gettext
-            # Register so other packages can reference our translations.
-            current_app.jinja_env.globals["_fsdomain"] = self._i18n_domain.gettext
-
-        @app.before_first_request
-        def check_babel():
-            # Verify that if Flask-Babel is installed
-            if have_babel() and "babel" not in app.extensions:
-                raise ValueError(
-                    "Flask-Babel is installed but not initialized"
-                )
+        current_app.jinja_env.globals["_fsdomain"] = self._i18n_domain.gettext
+
+        # Verify that if Flask-Babel is installed
+        if have_babel() and "babel" not in app.extensions:
+            raise ValueError(
+                "Flask-Babel is installed but not initialized"
+            )
 
     def _add_ctx_processor(self, endpoint, fn):
         group = self._context_processors.setdefault(endpoint, [])
         fn not in group and group.append(fn)
 
     def _run_ctx_processor(self, endpoint):
         rv = {}
```

### Comparing `Flask-Identity-1.0.3.dev7/flask_identity/datastore.py` & `flask_identity-1.0.4/flask_identity/datastore.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
     identity.datastore
     ~~~~~~~~~~~~~~~~~~~
     The Predefined Datastore of Flask-Identity
 
     :author: solardiax <solardiax@hotmail.com>
     :copyright: (c) 2020 by DreamEx Works.
-    :license: GPL-3.0, see LICENSE for more details.
+    :license: MIT, see LICENSE for more details.
 """
 
 import uuid
 
 from .utils import config_value
```

### Comparing `Flask-Identity-1.0.3.dev7/flask_identity/decorators.py` & `flask_identity-1.0.4/flask_identity/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
     identity.decorators
     ~~~~~~~~~~~~~~~~~~~
     Decorators definition of Flask-Identity
 
     :author: solardiax <solardiax@hotmail.com>
     :copyright: (c) 2020 by DreamEx Works.
-    :license: GPL-3.0, see LICENSE for more details.
+    :license: MIT, see LICENSE for more details.
 """
 
 from collections import namedtuple
 from functools import wraps
 
 # noinspection PyProtectedMember
 from flask import request, _request_ctx_stack
@@ -204,15 +204,15 @@
     This decorator does nothing unless Flask-WTF::CSRFProtect has been initialized.
 
     This decorator does nothing if *WTF_CSRF_ENABLED* == **False**.
 
     This decorator will always require CSRF if the caller is authenticated.
 
     This decorator will suppress CSRF if caller isn't authenticated and has set the
-    *SECURITY_CSRF_IGNORE_UNAUTH_ENDPOINTS* config variable.
+    *WTF_CSRF_IGNORE_UNAUTH_ENDPOINTS* config variable.
 
     :param fall_through: if set to True, then if CSRF fails here - simply keep going.
         This is appropriate if underlying view is form based and once the form is
         instantiated, the csrf_token will be available.
         Note that this can mask some errors such as 'The CSRF session token is missing.'
         meaning that the caller didn't send a session cookie and instead the caller
         might get a 'The CSRF token is missing.' error.
@@ -220,15 +220,15 @@
 
     def wrapper(fn):
         @wraps(fn)
         def decorated(*args, **kwargs):
             if not current_app.config.get("WTF_CSRF_ENABLED", False) or not current_app.extensions.get("csrf", None):
                 return fn(*args, **kwargs)
 
-            if config_value("CSRF_IGNORE_UNAUTH_ENDPOINTS") and not current_user.is_authenticated:
+            if config_value("WTF_CSRF_IGNORE_UNAUTH_ENDPOINTS") and not current_user.is_authenticated:
                 _request_ctx_stack.top.fs_ignore_csrf = True
             else:
                 try:
                     _csrf.protect()
                 except:
                     if not fall_through:
                         raise
```

### Comparing `Flask-Identity-1.0.3.dev7/flask_identity/forms.py` & `flask_identity-1.0.4/flask_identity/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
     identity.forms
     ~~~~~~~~~~~~~~~~~~~
     Default forms of Flask-Identity
     
     :author: solardiax <solardiax@hotmail.com>
     :copyright: (c) 2020 by DreamEx Works.
-    :license: GPL-3.0, see LICENSE for more details.
+    :license: MIT, see LICENSE for more details.
 """
 
 from flask import flash, request, session
 from flask_wtf import FlaskForm
 from wtforms import HiddenField, PasswordField, StringField, BooleanField, ValidationError
 from wtforms.validators import DataRequired
 from .utils import validate_redirect_url, config_value, current_identity, get_message
@@ -84,15 +84,15 @@
             if config_value('NEXT_STORE') == 'request':
                 getattr(self, self._NEXT_FIELD).data = request.args.get(next_key, "")
             else:
                 getattr(self, self._NEXT_FIELD).data = session.get(next_key, "")
 
         getattr(self, self._REMEBER_FIELD).default = config_value("DEFAULT_REMEMBER_ME")
 
-    def validate(self):
+    def validate(self, extra_validators=None):
         if not super().validate():
             return False
 
         self.user = current_identity.datastore.find_user(**{self._IDENTITY_FIELD: self.data[self._IDENTITY_FIELD]})
 
         if self.user is None:
             getattr(self, self._IDENTITY_FIELD).errors.append(get_message('USER_DOES_NOT_EXIST')[0])
```

### Comparing `Flask-Identity-1.0.3.dev7/flask_identity/mixins.py` & `flask_identity-1.0.4/flask_identity/mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
     identity.mixins
     ~~~~~~~~~~~~~~~~~~~
     Mixins of Flask-Identity
 
     :author: solardiax <solardiax@hotmail.com>
     :copyright: (c) 2020 by DreamEx Works.
-    :license: GPL-3.0, see LICENSE for more details.
+    :license: MIT, see LICENSE for more details.
 """
 
 
 # noinspection PyUnresolvedReferences
 class RoleMixin(object):
     """Mixin for `Role` model definitions"""
```

### Comparing `Flask-Identity-1.0.3.dev7/flask_identity/translations/en_US/LC_MESSAGES/flask_identity.mo` & `flask_identity-1.0.4/flask_identity/translations/en_US/LC_MESSAGES/flask_identity.mo`

 * *Files identical despite different names*

### Comparing `Flask-Identity-1.0.3.dev7/flask_identity/translations/en_US/LC_MESSAGES/flask_identity.po` & `flask_identity-1.0.4/flask_identity/translations/en_US/LC_MESSAGES/flask_identity.po`

 * *Files identical despite different names*

### Comparing `Flask-Identity-1.0.3.dev7/flask_identity/translations/flask_identity.pot` & `flask_identity-1.0.4/flask_identity/translations/flask_identity.pot`

 * *Files identical despite different names*

### Comparing `Flask-Identity-1.0.3.dev7/flask_identity/translations/zh_Hans_CN/LC_MESSAGES/flask_identity.mo` & `flask_identity-1.0.4/flask_identity/translations/zh_hans_CN/LC_MESSAGES/flask_identity.mo`

 * *Files identical despite different names*

### Comparing `Flask-Identity-1.0.3.dev7/flask_identity/translations/zh_Hans_CN/LC_MESSAGES/flask_identity.po` & `flask_identity-1.0.4/flask_identity/translations/zh_hans_CN/LC_MESSAGES/flask_identity.po`

 * *Files identical despite different names*

### Comparing `Flask-Identity-1.0.3.dev7/flask_identity/utils.py` & `flask_identity-1.0.4/flask_identity/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
     identity.utils
     ~~~~~~~~~~~~~~~~~~~
     Utils of Flask-Identity
 
     :author: solardiax <solardiax@hotmail.com>
     :copyright: (c) 2020 by DreamEx Works.
-    :license: GPL-3.0, see LICENSE for more details.
+    :license: MIT, see LICENSE for more details.
 """
 
 from datetime import datetime
 from urllib.parse import parse_qsl, urlsplit, urlunsplit, urlencode
 
 # noinspection PyProtectedMember
 from flask import current_app, has_request_context, request, session, url_for, _request_ctx_stack
```

### Comparing `Flask-Identity-1.0.3.dev7/flask_identity/views.py` & `flask_identity-1.0.4/flask_identity/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
     identity.views
     ~~~~~~~~~~~~~~~~~~~
     Default views of Flask-Identity
     
     :author: solardiax <solardiax@hotmail.com>
     :copyright: (c) 2020 by DreamEx Works.
-    :license: GPL-3.0, see LICENSE for more details.
+    :license: MIT, see LICENSE for more details.
 """
 
 from flask import request, after_this_request, jsonify, url_for, Blueprint
 from flask_wtf import csrf
 from werkzeug.datastructures import MultiDict
 
 from .decorators import unauth_csrf
```

### Comparing `Flask-Identity-1.0.3.dev7/pyproject.toml` & `flask_identity-1.0.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 [[tool.poetry.source]]
+name = "PyPI"
+priority = "primary"
+
+[[tool.poetry.source]]
 name = "aliyun"
 url = "https://mirrors.aliyun.com/pypi/simple/"
-default = true
+priority = "supplemental"
 
 [tool.poetry]
 name = "Flask-Identity"
-version = "1.0.3dev7"
+version = "1.0.4"
 description = "A lightweight extension & library to security Flask applications quickly and simply."
 authors = ["SolardiaX <solardiax@hotmail.com>"]
 maintainers = ["SolardiaX <solardiax@hotmail.com>"]
 license = "MIT"
 readme="README.rst"
 repository="https://github.com/SolardiaX/flask-identity"
 homepage="https://github.com/SolardiaX/flask-identity"
@@ -31,25 +35,25 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 include = [
     "LICENSE.rst"
 ]
 
 [tool.poetry.dependencies]
-bcrypt = "^3.2.0"
-cryptography = "^3.4.6"
-flask = "^1.1.2"
-flask-wtf = "^0.14.3"
-flask-babel = "^2.0.0"
+bcrypt = "^4.0.1"
+cryptography = "^41.0.0"
+flask = "^2.3.2"
+flask-wtf = "^1.1.1"
+flask-babel = "^3.1.0"
 passlib = "^1.7.4"
-python = "^3.6"
+python = "^3.9"
 
 [tool.poetry.dev-dependencies]
-flask-sqlalchemy = "^2.4.4"
-sphinx = "^3.5.1"
+flask-sqlalchemy = "^3.0.3"
+sphinx = "^7.0.1"
 flask-sphinx-themes = "^1.0.2"
-pallets-sphinx-themes = "^1.2.3"
-sphinx-issues = "^1.2.0"
+pallets-sphinx-themes = "^2.1.0"
+sphinx-issues = "^3.0.1"
 
 [build-system]
-requires = ["poetry-core>=1.0.0", "setuptools", "wheel"]
+requires = ["poetry-core>=1.5.1", "setuptools", "wheel"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `Flask-Identity-1.0.3.dev7/PKG-INFO` & `flask_identity-1.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 Metadata-Version: 2.1
 Name: flask-identity
-Version: 1.0.3.dev7
+Version: 1.0.4
 Summary: A lightweight extension & library to security Flask applications quickly and simply.
 Home-page: https://github.com/SolardiaX/flask-identity
 License: MIT
 Author: SolardiaX
 Author-email: solardiax@hotmail.com
 Maintainer: SolardiaX
 Maintainer-email: solardiax@hotmail.com
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
-Requires-Dist: bcrypt (>=3.2.0,<4.0.0)
-Requires-Dist: cryptography (>=3.4.6,<4.0.0)
-Requires-Dist: flask (>=1.1.2,<2.0.0)
-Requires-Dist: flask-babel (>=2.0.0,<3.0.0)
-Requires-Dist: flask-wtf (>=0.14.3,<0.15.0)
+Requires-Dist: bcrypt (>=4.0.1,<5.0.0)
+Requires-Dist: cryptography (>=41.0.0,<42.0.0)
+Requires-Dist: flask (>=2.3.2,<3.0.0)
+Requires-Dist: flask-babel (>=3.1.0,<4.0.0)
+Requires-Dist: flask-wtf (>=1.1.1,<2.0.0)
 Requires-Dist: passlib (>=1.7.4,<2.0.0)
 Project-URL: Repository, https://github.com/SolardiaX/flask-identity
 Description-Content-Type: text/x-rst
 
 Flask-Identity
 ===================
 
@@ -87,16 +86,15 @@
 some codes are direct merged from other successful open-source libraries:
 
 * `Flask-Login <https://flask-login.readthedocs.org/en/latest/>`_
 * `Flask-Security <https://flask-security.readthedocs.org/en/latest/>`_
 
 Contributing
 ++++++++++++
-Issues and pull requests are welcome. Other maintainers are also welcome. Unlike
-the original Flask-Security - issue pull requests against the *master* branch.
+Issues and pull requests are welcome.
 Please consult these `contributing`_ guidelines.
 
 .. _contributing: https://github.com/solardiax/flask-identity/blob/master/CONTRIBUTING.rst
 
 Installing
 ----------
 Install and update using `pip <https://pip.pypa.io/en/stable/quickstart/>`_:
```

