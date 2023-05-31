# Comparing `tmp/arkindex_export-0.1.3-py3-none-any.whl.zip` & `tmp/arkindex_export-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4019 bytes, number of entries: 7
--rw-r--r--  2.0 unx     1671 b- defN 23-May-26 09:28 arkindex_export/__init__.py
--rw-r--r--  2.0 unx     6105 b- defN 23-May-26 09:28 arkindex_export/models.py
--rw-r--r--  2.0 unx     1800 b- defN 23-May-26 09:28 arkindex_export/queries.py
--rw-r--r--  2.0 unx      199 b- defN 23-May-26 09:30 arkindex_export-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-26 09:30 arkindex_export-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-May-26 09:30 arkindex_export-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      578 b- defN 23-May-26 09:30 arkindex_export-0.1.3.dist-info/RECORD
-7 files, 10461 bytes uncompressed, 2989 bytes compressed:  71.4%
+Zip file size: 4107 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     1671 b- defN 23-May-31 08:12 arkindex_export/__init__.py
+-rw-r--r--  2.0 unx     7313 b- defN 23-May-31 08:12 arkindex_export/models.py
+-rw-r--r--  2.0 unx     1800 b- defN 23-May-31 08:12 arkindex_export/queries.py
+-rw-r--r--  2.0 unx      199 b- defN 23-May-31 08:13 arkindex_export-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-31 08:13 arkindex_export-0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-May-31 08:13 arkindex_export-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      578 b- defN 23-May-31 08:13 arkindex_export-0.1.4.dist-info/RECORD
+7 files, 11669 bytes uncompressed, 3077 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: arkindex_export/models.py
 Comment: 
 
 Filename: arkindex_export/queries.py
 Comment: 
 
-Filename: arkindex_export-0.1.3.dist-info/METADATA
+Filename: arkindex_export-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: arkindex_export-0.1.3.dist-info/WHEEL
+Filename: arkindex_export-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: arkindex_export-0.1.3.dist-info/top_level.txt
+Filename: arkindex_export-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: arkindex_export-0.1.3.dist-info/RECORD
+Filename: arkindex_export-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## arkindex_export/models.py

```diff
@@ -35,14 +35,29 @@
     revision = CharField()
     type = CharField()
 
     class Meta:
         table_name = "worker_version"
 
 
+class WorkerRun(BaseModel):
+    id = CharField(primary_key=True)
+    worker_version = ForeignKeyField(
+        column_name="worker_version_id", field="id", model=WorkerVersion
+    )
+    model_version_id = CharField(null=True)
+    model_id = CharField(null=True)
+    model_name = CharField(null=True)
+    configuration_id = CharField(null=True)
+    configuration = TextField(null=True)
+
+    class Meta:
+        table_name = "worker_run"
+
+
 class ImageServer(BaseModel):
     id = CharField(primary_key=True)
     url = TextField(unique=True)
     display_name = CharField()
     max_width = IntegerField(null=True)
     max_height = IntegerField(null=True)
 
@@ -69,14 +84,17 @@
     polygon = TextField(null=True)
     confidence = FloatField(null=True)
     rotation_angle = IntegerField(constraints=[SQL("DEFAULT 0")])
     mirrored = IntegerField(constraints=[SQL("DEFAULT 0")])
     worker_version = ForeignKeyField(
         column_name="worker_version_id", field="id", model=WorkerVersion, null=True
     )
+    worker_run = ForeignKeyField(
+        column_name="worker_run_id", field="id", model=WorkerRun, null=True
+    )
 
     created = FloatField()
     updated = FloatField()
 
     class Meta:
         table_name = "element"
 
@@ -88,14 +106,17 @@
     state = CharField(constraints=[SQL("DEFAULT 'pending'")])
     element = ForeignKeyField(column_name="element_id", field="id", model=Element)
     high_confidence = IntegerField(constraints=[SQL("DEFAULT 0")])
     moderator = CharField(null=True)
     worker_version = ForeignKeyField(
         column_name="worker_version_id", field="id", model=WorkerVersion, null=True
     )
+    worker_run = ForeignKeyField(
+        column_name="worker_run_id", field="id", model=WorkerRun, null=True
+    )
 
     class Meta:
         table_name = "classification"
 
 
 class ElementPath(BaseModel):
     id = CharField(primary_key=True)
@@ -125,14 +146,17 @@
     type = ForeignKeyField(column_name="type_id", field="id", model=EntityType)
     metas = TextField(null=True)
     moderator = CharField(null=True)
     validated = IntegerField(constraints=[SQL("DEFAULT 0")])
     worker_version = ForeignKeyField(
         column_name="worker_version_id", field="id", model=WorkerVersion, null=True
     )
+    worker_run = ForeignKeyField(
+        column_name="worker_run_id", field="id", model=WorkerRun, null=True
+    )
 
     class Meta:
         table_name = "entity"
 
 
 class EntityRole(BaseModel):
     id = CharField(primary_key=True)
@@ -173,27 +197,34 @@
     element = ForeignKeyField(column_name="element_id", field="id", model=Element)
     entity = ForeignKeyField(
         column_name="entity_id", field="id", model=Entity, null=True
     )
     worker_version = ForeignKeyField(
         column_name="worker_version_id", field="id", model=WorkerVersion, null=True
     )
+    worker_run = ForeignKeyField(
+        column_name="worker_run_id", field="id", model=WorkerRun, null=True
+    )
 
     class Meta:
         table_name = "metadata"
 
 
 class Transcription(BaseModel):
     id = CharField(primary_key=True)
+    orientation = TextField(constraints=[SQL("DEFAULT 'horizontal-lr'")])
     text = TextField()
     confidence = FloatField(null=True)
     element = ForeignKeyField(column_name="element_id", field="id", model=Element)
     worker_version = ForeignKeyField(
         column_name="worker_version_id", field="id", model=WorkerVersion, null=True
     )
+    worker_run = ForeignKeyField(
+        column_name="worker_run_id", field="id", model=WorkerRun, null=True
+    )
 
     class Meta:
         table_name = "transcription"
 
 
 class TranscriptionEntity(BaseModel):
     id = CharField(primary_key=True)
@@ -203,13 +234,16 @@
     confidence = FloatField(null=True)
     transcription = ForeignKeyField(
         column_name="transcription_id", field="id", model=Transcription
     )
     worker_version = ForeignKeyField(
         column_name="worker_version_id", field="id", model=WorkerVersion, null=True
     )
+    worker_run = ForeignKeyField(
+        column_name="worker_run_id", field="id", model=WorkerRun, null=True
+    )
 
     class Meta:
         table_name = "transcription_entity"
         indexes = (
             (("transcription", "entity", "offset", "length", "worker_version"), True),
         )
```

