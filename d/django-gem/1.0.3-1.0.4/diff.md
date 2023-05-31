# Comparing `tmp/django_gem-1.0.3.tar.gz` & `tmp/django_gem-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_gem-1.0.3.tar", max compression
+gzip compressed data, was "django_gem-1.0.4.tar", max compression
```

## Comparing `django_gem-1.0.3.tar` & `django_gem-1.0.4.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     1067 2023-05-26 12:13:27.046599 django_gem-1.0.3/LICENSE
--rw-r--r--   0        0        0     2786 2023-05-26 12:13:27.046599 django_gem-1.0.3/README.md
--rw-r--r--   0        0        0        0 2023-05-26 12:13:27.046599 django_gem-1.0.3/django_gem/__init__.py
--rw-r--r--   0        0        0      257 2023-05-26 12:13:27.046599 django_gem-1.0.3/django_gem/apps.py
--rw-r--r--   0        0        0      457 2023-05-26 12:13:27.046599 django_gem-1.0.3/django_gem/constants.py
--rw-r--r--   0        0        0       71 2023-05-26 12:13:27.046599 django_gem-1.0.3/django_gem/context/__init__.py
--rw-r--r--   0        0        0      283 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/context/cutting_always_eager.py
--rw-r--r--   0        0        0      298 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/context/override_gem_setting.py
--rw-r--r--   0        0        0        0 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/cutters/__init__.py
--rw-r--r--   0        0        0     1026 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/cutters/base.py
--rw-r--r--   0        0        0       54 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/decorators/__init__.py
--rw-r--r--   0        0        0      220 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/decorators/context.py
--rw-r--r--   0        0        0     1104 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/decorators/cutters.py
--rw-r--r--   0        0        0     1536 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/decorators/models.py
--rw-r--r--   0        0        0        0 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/entities/__init__.py
--rw-r--r--   0        0        0      106 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/entities/context.py
--rw-r--r--   0        0        0      737 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/entities/models.py
--rw-r--r--   0        0        0     1544 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/entities/registry.py
--rw-r--r--   0        0        0     1108 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/exceptions.py
--rw-r--r--   0        0        0       58 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/logger.py
--rw-r--r--   0        0        0        0 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/management/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/management/commands/__init__.py
--rw-r--r--   0        0        0     1042 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/management/commands/cutmodel.py
--rw-r--r--   0        0        0     1090 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/management/commands/cutqueryset.py
--rw-r--r--   0        0        0     2622 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/migrations/__init__.py
--rw-r--r--   0        0        0       56 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/models/__init__.py
--rw-r--r--   0        0        0     1969 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/models/base.py
--rw-r--r--   0        0        0     1432 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/models/gem_log_entry.py
--rw-r--r--   0        0        0        0 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/models/managers/__init__.py
--rw-r--r--   0        0        0     1297 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/models/managers/gem_log_entry_manager.py
--rw-r--r--   0        0        0     2850 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/models/mixins.py
--rw-r--r--   0        0        0      178 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/overrides/__init__.py
--rw-r--r--   0        0        0     1150 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/overrides/delete.py
--rw-r--r--   0        0        0     1061 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/overrides/m2m_changed.py
--rw-r--r--   0        0        0     1522 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/overrides/save.py
--rw-r--r--   0        0        0      966 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/overrides/utils.py
--rw-r--r--   0        0        0      184 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/tasks/__init__.py
--rw-r--r--   0        0        0      243 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/tasks/cut_content_type.py
--rw-r--r--   0        0        0      187 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/tasks/cut_models.py
--rw-r--r--   0        0        0      229 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/tasks/cut_queryset.py
--rw-r--r--   0        0        0      251 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/toolkit/__init__.py
--rw-r--r--   0        0        0       57 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/toolkit/anvils/__init__.py
--rw-r--r--   0        0        0      100 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/toolkit/anvils/base.py
--rw-r--r--   0        0        0      272 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/toolkit/anvils/celery.py
--rw-r--r--   0        0        0      256 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/toolkit/anvils/eager.py
--rw-r--r--   0        0        0     2690 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/toolkit/chest.py
--rw-r--r--   0        0        0     5072 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/toolkit/forge.py
--rw-r--r--   0        0        0     7337 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/toolkit/registry.py
--rw-r--r--   0        0        0     4600 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/toolkit/saw.py
--rw-r--r--   0        0        0     1328 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/toolkit/settings.py
--rw-r--r--   0        0        0     1615 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/toolkit/smith.py
--rw-r--r--   0        0        0     4198 2023-05-26 12:13:27.050599 django_gem-1.0.3/django_gem/validators.py
--rw-r--r--   0        0        0      811 2023-05-26 12:13:27.054599 django_gem-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     3504 1970-01-01 00:00:00.000000 django_gem-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-31 18:40:19.660819 django_gem-1.0.4/LICENSE
+-rw-r--r--   0        0        0     2786 2023-05-31 18:40:19.660819 django_gem-1.0.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/__init__.py
+-rw-r--r--   0        0        0      257 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/apps.py
+-rw-r--r--   0        0        0      457 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/constants.py
+-rw-r--r--   0        0        0       71 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/context/__init__.py
+-rw-r--r--   0        0        0      283 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/context/cutting_always_eager.py
+-rw-r--r--   0        0        0      298 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/context/override_gem_setting.py
+-rw-r--r--   0        0        0        0 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/cutters/__init__.py
+-rw-r--r--   0        0        0     1026 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/cutters/base.py
+-rw-r--r--   0        0        0       54 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/decorators/__init__.py
+-rw-r--r--   0        0        0      220 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/decorators/context.py
+-rw-r--r--   0        0        0     1104 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/decorators/cutters.py
+-rw-r--r--   0        0        0     1536 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/decorators/models.py
+-rw-r--r--   0        0        0        0 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/entities/__init__.py
+-rw-r--r--   0        0        0      106 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/entities/context.py
+-rw-r--r--   0        0        0      737 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/entities/models.py
+-rw-r--r--   0        0        0     1544 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/entities/registry.py
+-rw-r--r--   0        0        0     1108 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/exceptions.py
+-rw-r--r--   0        0        0       58 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/logger.py
+-rw-r--r--   0        0        0        0 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/management/commands/__init__.py
+-rw-r--r--   0        0        0     1042 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/management/commands/cutmodel.py
+-rw-r--r--   0        0        0     1090 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/management/commands/cutqueryset.py
+-rw-r--r--   0        0        0     2622 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/migrations/__init__.py
+-rw-r--r--   0        0        0       56 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/models/__init__.py
+-rw-r--r--   0        0        0     1969 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/models/base.py
+-rw-r--r--   0        0        0     1432 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/models/gem_log_entry.py
+-rw-r--r--   0        0        0        0 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/models/managers/__init__.py
+-rw-r--r--   0        0        0     1297 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/models/managers/gem_log_entry_manager.py
+-rw-r--r--   0        0        0     2850 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/models/mixins.py
+-rw-r--r--   0        0        0      178 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/overrides/__init__.py
+-rw-r--r--   0        0        0     1150 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/overrides/delete.py
+-rw-r--r--   0        0        0     1061 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/overrides/m2m_changed.py
+-rw-r--r--   0        0        0     1522 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/overrides/save.py
+-rw-r--r--   0        0        0      966 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/overrides/utils.py
+-rw-r--r--   0        0        0      184 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/tasks/__init__.py
+-rw-r--r--   0        0        0      243 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/tasks/cut_content_type.py
+-rw-r--r--   0        0        0      187 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/tasks/cut_models.py
+-rw-r--r--   0        0        0      229 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/tasks/cut_queryset.py
+-rw-r--r--   0        0        0      251 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/toolkit/__init__.py
+-rw-r--r--   0        0        0       57 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/toolkit/anvils/__init__.py
+-rw-r--r--   0        0        0      100 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/toolkit/anvils/base.py
+-rw-r--r--   0        0        0      272 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/toolkit/anvils/celery.py
+-rw-r--r--   0        0        0      256 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/toolkit/anvils/eager.py
+-rw-r--r--   0        0        0     2690 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/toolkit/chest.py
+-rw-r--r--   0        0        0     5072 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/toolkit/forge.py
+-rw-r--r--   0        0        0     7337 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/toolkit/registry.py
+-rw-r--r--   0        0        0     4640 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/toolkit/saw.py
+-rw-r--r--   0        0        0     1328 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/toolkit/settings.py
+-rw-r--r--   0        0        0     1615 2023-05-31 18:40:19.660819 django_gem-1.0.4/django_gem/toolkit/smith.py
+-rw-r--r--   0        0        0     4198 2023-05-31 18:40:19.664818 django_gem-1.0.4/django_gem/validators.py
+-rw-r--r--   0        0        0      811 2023-05-31 18:40:19.664818 django_gem-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3504 1970-01-01 00:00:00.000000 django_gem-1.0.4/PKG-INFO
```

### Comparing `django_gem-1.0.3/LICENSE` & `django_gem-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.3/README.md` & `django_gem-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.3/django_gem/cutters/base.py` & `django_gem-1.0.4/django_gem/cutters/base.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.3/django_gem/decorators/cutters.py` & `django_gem-1.0.4/django_gem/decorators/cutters.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.3/django_gem/decorators/models.py` & `django_gem-1.0.4/django_gem/decorators/models.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.3/django_gem/entities/models.py` & `django_gem-1.0.4/django_gem/entities/models.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.3/django_gem/entities/registry.py` & `django_gem-1.0.4/django_gem/entities/registry.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.3/django_gem/exceptions.py` & `django_gem-1.0.4/django_gem/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.3/django_gem/management/commands/cutmodel.py` & `django_gem-1.0.4/django_gem/management/commands/cutmodel.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.3/django_gem/management/commands/cutqueryset.py` & `django_gem-1.0.4/django_gem/management/commands/cutqueryset.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.3/django_gem/migrations/0001_initial.py` & `django_gem-1.0.4/django_gem/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.3/django_gem/models/base.py` & `django_gem-1.0.4/django_gem/models/base.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.3/django_gem/models/gem_log_entry.py` & `django_gem-1.0.4/django_gem/models/gem_log_entry.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.3/django_gem/models/managers/gem_log_entry_manager.py` & `django_gem-1.0.4/django_gem/models/managers/gem_log_entry_manager.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.3/django_gem/models/mixins.py` & `django_gem-1.0.4/django_gem/models/mixins.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.3/django_gem/overrides/delete.py` & `django_gem-1.0.4/django_gem/overrides/delete.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.3/django_gem/overrides/m2m_changed.py` & `django_gem-1.0.4/django_gem/overrides/m2m_changed.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.3/django_gem/overrides/save.py` & `django_gem-1.0.4/django_gem/overrides/save.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.3/django_gem/overrides/utils.py` & `django_gem-1.0.4/django_gem/overrides/utils.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.3/django_gem/toolkit/chest.py` & `django_gem-1.0.4/django_gem/toolkit/chest.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.3/django_gem/toolkit/forge.py` & `django_gem-1.0.4/django_gem/toolkit/forge.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.3/django_gem/toolkit/registry.py` & `django_gem-1.0.4/django_gem/toolkit/registry.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.3/django_gem/toolkit/saw.py` & `django_gem-1.0.4/django_gem/toolkit/saw.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,36 +8,35 @@
 from django_gem.models.mixins import GemModelMixin
 from django_gem.toolkit import forge, gem_settings
 from django_gem.toolkit.chest import SealedChestItem
 
 
 class Saw:
     @classmethod
-    @transaction.atomic
     def cut_content_type(cls, content_type_id: int, field_names: list):
         gem_cutting_enabled = gem_settings.GEM_CUTTING_ENABLED
 
         if not gem_cutting_enabled:
             return
         try:
             content_type: ContentType = ContentType.objects.get(id=content_type_id)
         except ContentType.DoesNotExist:
             return
 
         model_class = content_type.model_class()
         for model_instance in model_class.objects.all():
             if isinstance(model_class, GemModelMixin):
                 model_class.update_cutting_started_at([model_instance.id])
-            for field_name in field_names:
-                forge.cut_model_field(model_instance, field_name)
+            with transaction.atomic():
+                for field_name in field_names:
+                    forge.cut_model_field(model_instance, field_name)
             if isinstance(model_class, GemModelMixin):
                 model_class.update_cutting_completed_at([model_instance.id])
 
     @classmethod
-    @transaction.atomic
     def cut_models(cls, sealed_chest: str):
         gem_cutting_enabled = gem_settings.GEM_CUTTING_ENABLED
 
         if not gem_cutting_enabled:
             return
         try:
             unsealed_chest: typing.Dict[int, typing.List[typing.Dict]] = json.loads(sealed_chest)
@@ -59,28 +58,27 @@
             if isinstance(model_class, GemModelMixin):
                 model_class.update_cutting_started_at(chest_item_object_ids)
 
             for model_instance in model_class.objects.filter(id__in=chest_item_object_ids):
                 model_instance_id = str(model_instance.id)
                 if (sealed_chest_item := sealed_chest_mapping.get(str(model_instance_id))) is None:
                     continue
-                with contextlib.suppress(IntegrityError):
+                with contextlib.suppress(IntegrityError), transaction.atomic():
                     # Because of the distributed nature of cutting, the update to gem can happen
                     # after the referencing model was deleted. This will ensure we don't stop
                     # all the cuttings if something goes wrong.
                     forge.cut_model_fields(
                         model_instance,
                         sealed_chest_item.gem_fields,
                     )
 
             if isinstance(model_class, GemModelMixin):
                 model_class.update_cutting_completed_at(chest_item_object_ids)
 
     @classmethod
-    @transaction.atomic
     def cut_queryset(cls, content_type_id: int, object_ids: list):
         gem_cutting_enabled = gem_settings.GEM_CUTTING_ENABLED
 
         if not gem_cutting_enabled:
             return
         from django_gem.toolkit import forge, smith
 
@@ -106,8 +104,9 @@
                     reverse_cutter_trigger.model
                 )
                 smith.add_item(
                     content_type_id=reversed_cutter_model_content_type.id,
                     object_ids=object_ids,
                     gem_fields=reverse_cutter_trigger.gem_fields,
                 )
-            smith.initiate_cutting()
+            with transaction.atomic():
+                smith.initiate_cutting()
```

### Comparing `django_gem-1.0.3/django_gem/toolkit/settings.py` & `django_gem-1.0.4/django_gem/toolkit/settings.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.3/django_gem/toolkit/smith.py` & `django_gem-1.0.4/django_gem/toolkit/smith.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.3/django_gem/validators.py` & `django_gem-1.0.4/django_gem/validators.py`

 * *Files identical despite different names*

### Comparing `django_gem-1.0.3/pyproject.toml` & `django_gem-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 profile = "black"
 
 [tool.black]
 line-length = 100
 
 [tool.poetry]
 name = "django-gem"
-version = "1.0.3"
+version = "1.0.4"
 description = "Distrubited calculations for Django models"
 authors = ["Artur Veres <artur8118@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "django_gem"}]
 
 [tool.poetry.dependencies]
```

### Comparing `django_gem-1.0.3/PKG-INFO` & `django_gem-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-gem
-Version: 1.0.3
+Version: 1.0.4
 Summary: Distrubited calculations for Django models
 License: MIT
 Author: Artur Veres
 Author-email: artur8118@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

