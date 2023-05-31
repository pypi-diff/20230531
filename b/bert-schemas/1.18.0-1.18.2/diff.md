# Comparing `tmp/bert_schemas-1.18.0.tar.gz` & `tmp/bert_schemas-1.18.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bert_schemas-1.18.0.tar", max compression
+gzip compressed data, was "bert_schemas-1.18.2.tar", max compression
```

## Comparing `bert_schemas-1.18.0.tar` & `bert_schemas-1.18.2.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0      481 2023-05-15 14:27:01.954881 bert_schemas-1.18.0/README.md
--rw-r--r--   0        0        0       80 2023-05-15 14:27:01.954881 bert_schemas-1.18.0/bert_schemas/__init__.py
--rw-r--r--   0        0        0      870 2023-05-15 14:27:01.954881 bert_schemas-1.18.0/bert_schemas/access.py
--rw-r--r--   0        0        0      357 2023-05-15 14:27:01.954881 bert_schemas-1.18.0/bert_schemas/group.py
--rw-r--r--   0        0        0    45200 2023-05-18 17:04:20.796105 bert_schemas-1.18.0/bert_schemas/job.py
--rw-r--r--   0        0        0      770 2023-04-14 20:15:22.201190 bert_schemas-1.18.0/bert_schemas/message.py
--rw-r--r--   0        0        0     1967 2023-04-14 20:15:22.201190 bert_schemas-1.18.0/bert_schemas/questionnaire.py
--rw-r--r--   0        0        0      175 2023-04-14 20:15:22.201190 bert_schemas-1.18.0/bert_schemas/report.py
--rw-r--r--   0        0        0       51 2023-04-14 20:15:22.201190 bert_schemas-1.18.0/bert_schemas/testing/__init__.py
--rw-r--r--   0        0        0        0 2023-04-14 20:15:22.201190 bert_schemas-1.18.0/bert_schemas/testing/factories/__init__.py
--rw-r--r--   0        0        0      492 2023-04-14 20:15:22.201190 bert_schemas-1.18.0/bert_schemas/testing/factories/helpers.py
--rw-r--r--   0        0        0        0 2023-04-14 20:15:22.201190 bert_schemas-1.18.0/bert_schemas/testing/factories/job/__init__.py
--rw-r--r--   0        0        0     2713 2023-04-28 17:21:29.074962 bert_schemas-1.18.0/bert_schemas/testing/factories/job/barrier.py
--rw-r--r--   0        0        0     2509 2023-04-28 17:21:29.074962 bert_schemas-1.18.0/bert_schemas/testing/factories/job/bec.py
--rw-r--r--   0        0        0     2611 2023-04-28 17:21:29.074962 bert_schemas-1.18.0/bert_schemas/testing/factories/job/bragg.py
--rw-r--r--   0        0        0     2715 2023-04-28 17:21:29.074962 bert_schemas-1.18.0/bert_schemas/testing/factories/job/paint_1d.py
--rw-r--r--   0        0        0     2866 2023-04-28 17:21:29.074962 bert_schemas-1.18.0/bert_schemas/testing/factories/job/transistor.py
--rw-r--r--   0        0        0        0 2023-04-14 20:15:22.201190 bert_schemas-1.18.0/bert_schemas/testing/fixtures/__init__.py
--rw-r--r--   0        0        0     9136 2023-04-26 21:05:16.851464 bert_schemas-1.18.0/bert_schemas/testing/fixtures/job/__init__.py
--rw-r--r--   0        0        0     6071 2023-05-18 17:04:20.796105 bert_schemas-1.18.0/bert_schemas/testing/fixtures/job/barrier.py
--rw-r--r--   0        0        0     5811 2023-05-18 17:04:20.796105 bert_schemas-1.18.0/bert_schemas/testing/fixtures/job/bec.py
--rw-r--r--   0        0        0     5945 2023-05-18 17:04:20.796105 bert_schemas-1.18.0/bert_schemas/testing/fixtures/job/bragg.py
--rw-r--r--   0        0        0     6113 2023-05-18 17:04:20.796105 bert_schemas-1.18.0/bert_schemas/testing/fixtures/job/paint_1d.py
--rw-r--r--   0        0        0     6248 2023-05-18 17:04:20.796105 bert_schemas-1.18.0/bert_schemas/testing/fixtures/job/transistor.py
--rw-r--r--   0        0        0        0 2023-04-14 20:15:22.201190 bert_schemas-1.18.0/bert_schemas/testing/schemas/__init__.py
--rw-r--r--   0        0        0     1568 2023-04-14 20:15:22.201190 bert_schemas-1.18.0/bert_schemas/testing/schemas/job/__init__.py
--rw-r--r--   0        0        0     2275 2023-04-28 21:15:25.564351 bert_schemas-1.18.0/bert_schemas/testing/schemas/job/barrier.py
--rw-r--r--   0        0        0     2180 2023-04-28 21:15:25.564351 bert_schemas-1.18.0/bert_schemas/testing/schemas/job/bec.py
--rw-r--r--   0        0        0     2197 2023-04-28 21:15:25.564351 bert_schemas-1.18.0/bert_schemas/testing/schemas/job/bragg.py
--rw-r--r--   0        0        0     2368 2023-04-28 21:15:25.564351 bert_schemas-1.18.0/bert_schemas/testing/schemas/job/paint_1d.py
--rw-r--r--   0        0        0     2340 2023-04-28 21:15:25.564351 bert_schemas-1.18.0/bert_schemas/testing/schemas/job/shared.py
--rw-r--r--   0        0        0     2465 2023-04-28 21:15:25.564351 bert_schemas-1.18.0/bert_schemas/testing/schemas/job/transistor.py
--rw-r--r--   0        0        0     1950 2023-05-18 13:19:14.771500 bert_schemas-1.18.0/bert_schemas/user.py
--rw-r--r--   0        0        0     1329 2023-05-18 17:48:19.987547 bert_schemas-1.18.0/pyproject.toml
--rw-r--r--   0        0        0     1549 1970-01-01 00:00:00.000000 bert_schemas-1.18.0/setup.py
--rw-r--r--   0        0        0     1390 1970-01-01 00:00:00.000000 bert_schemas-1.18.0/PKG-INFO
+-rw-r--r--   0        0        0      481 2023-05-15 14:27:01.954881 bert_schemas-1.18.2/README.md
+-rw-r--r--   0        0        0       80 2023-05-31 16:47:44.137191 bert_schemas-1.18.2/bert_schemas/__init__.py
+-rw-r--r--   0        0        0      870 2023-05-31 16:47:44.137191 bert_schemas-1.18.2/bert_schemas/access.py
+-rw-r--r--   0        0        0      357 2023-05-31 16:47:44.137191 bert_schemas-1.18.2/bert_schemas/group.py
+-rw-r--r--   0        0        0    44878 2023-05-31 15:48:17.261694 bert_schemas-1.18.2/bert_schemas/job.py
+-rw-r--r--   0        0        0      770 2023-04-14 20:15:22.201190 bert_schemas-1.18.2/bert_schemas/message.py
+-rw-r--r--   0        0        0     1388 2023-05-31 16:47:44.137191 bert_schemas-1.18.2/bert_schemas/qpu.py
+-rw-r--r--   0        0        0     1967 2023-04-14 20:15:22.201190 bert_schemas-1.18.2/bert_schemas/questionnaire.py
+-rw-r--r--   0        0        0      175 2023-04-14 20:15:22.201190 bert_schemas-1.18.2/bert_schemas/report.py
+-rw-r--r--   0        0        0       51 2023-04-14 20:15:22.201190 bert_schemas-1.18.2/bert_schemas/testing/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-14 20:15:22.201190 bert_schemas-1.18.2/bert_schemas/testing/factories/__init__.py
+-rw-r--r--   0        0        0      492 2023-04-14 20:15:22.201190 bert_schemas-1.18.2/bert_schemas/testing/factories/helpers.py
+-rw-r--r--   0        0        0        0 2023-04-14 20:15:22.201190 bert_schemas-1.18.2/bert_schemas/testing/factories/job/__init__.py
+-rw-r--r--   0        0        0     2713 2023-04-28 17:21:29.074962 bert_schemas-1.18.2/bert_schemas/testing/factories/job/barrier.py
+-rw-r--r--   0        0        0     2509 2023-04-28 17:21:29.074962 bert_schemas-1.18.2/bert_schemas/testing/factories/job/bec.py
+-rw-r--r--   0        0        0     2611 2023-04-28 17:21:29.074962 bert_schemas-1.18.2/bert_schemas/testing/factories/job/bragg.py
+-rw-r--r--   0        0        0     2715 2023-04-28 17:21:29.074962 bert_schemas-1.18.2/bert_schemas/testing/factories/job/paint_1d.py
+-rw-r--r--   0        0        0     2866 2023-04-28 17:21:29.074962 bert_schemas-1.18.2/bert_schemas/testing/factories/job/transistor.py
+-rw-r--r--   0        0        0        0 2023-04-14 20:15:22.201190 bert_schemas-1.18.2/bert_schemas/testing/fixtures/__init__.py
+-rw-r--r--   0        0        0     9136 2023-04-26 21:05:16.851464 bert_schemas-1.18.2/bert_schemas/testing/fixtures/job/__init__.py
+-rw-r--r--   0        0        0     6106 2023-05-19 14:05:39.418474 bert_schemas-1.18.2/bert_schemas/testing/fixtures/job/barrier.py
+-rw-r--r--   0        0        0     5846 2023-05-19 14:05:39.418474 bert_schemas-1.18.2/bert_schemas/testing/fixtures/job/bec.py
+-rw-r--r--   0        0        0     5980 2023-05-19 14:05:39.418474 bert_schemas-1.18.2/bert_schemas/testing/fixtures/job/bragg.py
+-rw-r--r--   0        0        0     6148 2023-05-19 14:05:39.418474 bert_schemas-1.18.2/bert_schemas/testing/fixtures/job/paint_1d.py
+-rw-r--r--   0        0        0     6283 2023-05-19 14:05:39.418474 bert_schemas-1.18.2/bert_schemas/testing/fixtures/job/transistor.py
+-rw-r--r--   0        0        0        0 2023-04-14 20:15:22.201190 bert_schemas-1.18.2/bert_schemas/testing/schemas/__init__.py
+-rw-r--r--   0        0        0     1568 2023-04-14 20:15:22.201190 bert_schemas-1.18.2/bert_schemas/testing/schemas/job/__init__.py
+-rw-r--r--   0        0        0     2275 2023-04-28 21:15:25.564351 bert_schemas-1.18.2/bert_schemas/testing/schemas/job/barrier.py
+-rw-r--r--   0        0        0     2180 2023-04-28 21:15:25.564351 bert_schemas-1.18.2/bert_schemas/testing/schemas/job/bec.py
+-rw-r--r--   0        0        0     2197 2023-04-28 21:15:25.564351 bert_schemas-1.18.2/bert_schemas/testing/schemas/job/bragg.py
+-rw-r--r--   0        0        0     2368 2023-04-28 21:15:25.564351 bert_schemas-1.18.2/bert_schemas/testing/schemas/job/paint_1d.py
+-rw-r--r--   0        0        0     2340 2023-04-28 21:15:25.564351 bert_schemas-1.18.2/bert_schemas/testing/schemas/job/shared.py
+-rw-r--r--   0        0        0     2465 2023-04-28 21:15:25.564351 bert_schemas-1.18.2/bert_schemas/testing/schemas/job/transistor.py
+-rw-r--r--   0        0        0     1960 2023-05-31 16:47:44.137191 bert_schemas-1.18.2/bert_schemas/user.py
+-rw-r--r--   0        0        0     1329 2023-05-31 15:48:27.073624 bert_schemas-1.18.2/pyproject.toml
+-rw-r--r--   0        0        0     1549 1970-01-01 00:00:00.000000 bert_schemas-1.18.2/setup.py
+-rw-r--r--   0        0        0     1390 1970-01-01 00:00:00.000000 bert_schemas-1.18.2/PKG-INFO
```

### Comparing `bert_schemas-1.18.0/bert_schemas/access.py` & `bert_schemas-1.18.2/bert_schemas/access.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.18.0/bert_schemas/job.py` & `bert_schemas-1.18.2/bert_schemas/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,31 +15,15 @@
     conint,
     conlist,
     root_validator,
     validator,
 )
 from scipy.interpolate import interp1d
 from typing_extensions import TypedDict
-
-
-class QPUName(StrEnum):
-    SMALLBERT = "SMALLBERT"
-    BIGBERT = "BIGBERT"
-    UNDEFINED = "UNDEFINED"
-
-    def __str__(self):
-        return str(self.value)
-
-
-class QPUStatus(StrEnum):
-    ONLINE = "ONLINE"
-    OFFLINE = "OFFLINE"
-
-    def __str__(self):
-        return str(self.value)
+from .qpu import QPU, QPUName
 
 
 class JobOrigin(StrEnum):
     WEB = auto()
     OQTANT = auto()
 
 
@@ -124,31 +108,14 @@
     LORENTZIAN = "LORENTZIAN"
     SQUARE = "SQUARE"
 
     def __str__(self):
         return str(self.value)
 
 
-class QPU(BaseModel):
-    name: QPUName
-    status: QPUStatus
-
-    class Config:
-        orm_mode = True
-
-
-class QPUState(QPU):
-    pending_internal_jobs: int
-    pending_external_jobs: int
-
-
-class QPUUpdate(BaseModel):
-    status: QPUStatus
-
-
 class JobName(ConstrainedStr):
     min_length = 1
     max_length = 50
 
 
 class JobNote(ConstrainedStr):
     max_length = 500
@@ -467,15 +434,15 @@
             x_limits (list, optional): Plot position range (in microns) as a list of [min, max]. Default is [-101, 101].
             y_limits (list, optional): Plot energy range (in kHz) as a list of [min, max]. Default is [0, 101].
         """
         if x_limits is None:
             x_limits = [-101, 101]
         if y_limits is None:
             y_limits = [0, 101]
-        positions = np.linspace(-100, 100, 201)
+        positions = np.linspace(-50, 50, 101)
         Plotter.plot_points_and_line(
             x_data_points=[],
             y_data_points=[],
             x_data_line=positions,
             y_data_line=self.get_potentials(time, positions),
             x_limits=x_limits,
             y_limits=y_limits,
@@ -1190,20 +1157,31 @@
             JobType.BEC: BecInput,
         }
         for job_input in v:
             schema_validation_map.get(values["job_type"], Input)(**job_input.dict())
         return v
 
 
+class ResponseInput(BaseModel):
+    job_id: Optional[int]
+    run: Optional[int]
+    values: object
+    output: Optional[object]
+    notes: Optional[JobNote]
+
+    class Config:
+        orm_mode = True
+
+
 class JobResponse(JobBase):
     external_id: UUID
     status: JobStatus
     qpu: Optional[QPU]
     time_submit: datetime
-    inputs: List[Input] | List[InputWithoutOutput]
+    inputs: List[ResponseInput]
     failed_inputs: List[int] = []
 
 
 class JobInputsResponse(JobBase):
     external_id: UUID
     status: JobStatus
     qpu_name: QPUName = QPUName.UNDEFINED
```

### Comparing `bert_schemas-1.18.0/bert_schemas/message.py` & `bert_schemas-1.18.2/bert_schemas/message.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.18.0/bert_schemas/questionnaire.py` & `bert_schemas-1.18.2/bert_schemas/questionnaire.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.18.0/bert_schemas/testing/factories/job/barrier.py` & `bert_schemas-1.18.2/bert_schemas/testing/factories/job/barrier.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.18.0/bert_schemas/testing/factories/job/bec.py` & `bert_schemas-1.18.2/bert_schemas/testing/factories/job/bec.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.18.0/bert_schemas/testing/factories/job/bragg.py` & `bert_schemas-1.18.2/bert_schemas/testing/factories/job/bragg.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.18.0/bert_schemas/testing/factories/job/paint_1d.py` & `bert_schemas-1.18.2/bert_schemas/testing/factories/job/paint_1d.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.18.0/bert_schemas/testing/factories/job/transistor.py` & `bert_schemas-1.18.2/bert_schemas/testing/factories/job/transistor.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.18.0/bert_schemas/testing/fixtures/job/__init__.py` & `bert_schemas-1.18.2/bert_schemas/testing/fixtures/job/__init__.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.18.0/bert_schemas/testing/fixtures/job/barrier.py` & `bert_schemas-1.18.2/bert_schemas/testing/fixtures/job/barrier.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,199 +1,200 @@
 """Pytest fixtures for BARRIER jobs"""
 
 import pytest
 
 from .... import job as job_schema
+from .... import qpu as qpu_schema
 from ...factories.helpers import add_notes, set_run
 from ...factories.job import barrier as BarrierFactories
 
 
 @pytest.fixture
 def pending_barrier_job():
     job = BarrierFactories.BarrierJobPendingFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test barrier job - pending")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.PENDING
     job.display = True
     yield job
 
 
 @pytest.fixture
 def running_barrier_job():
     job = BarrierFactories.BarrierJobRunningFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test barrier job - running")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.RUNNING
     job.display = True
     yield job
 
 
 @pytest.fixture
 def complete_barrier_job():
     job = BarrierFactories.BarrierJobCompleteFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test barrier job - complete")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.COMPLETE
     job.display = True
     yield job
 
 
 @pytest.fixture
 def failed_barrier_job():
     job = BarrierFactories.BarrierJobFailedFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test barrier job - failed")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.FAILED
     job.display = True
     yield job
 
 
 @pytest.fixture
 def pending_barrier_batch_job():
     job = BarrierFactories.BarrierBatchJobPendingFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test barrier batch job - pending")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.PENDING
     job.display = True
     yield job
 
 
 @pytest.fixture
 def running_barrier_batch_job():
     job = BarrierFactories.BarrierBatchJobRunningFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test barrier batch job - running")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.RUNNING
     job.display = True
     yield job
 
 
 @pytest.fixture
 def complete_barrier_batch_job():
     job = BarrierFactories.BarrierBatchJobCompleteFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test barrier batch job - complete")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.COMPLETE
     job.display = True
     yield job
 
 
 @pytest.fixture
 def failed_barrier_batch_job():
     job = BarrierFactories.BarrierBatchJobFailedFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test barrier batch job - failed")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.FAILED
     job.display = True
     yield job
 
 
 @pytest.fixture
 def pending_barrier_job_response():
     job = BarrierFactories.BarrierJobResponsePendingFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test barrier job response - pending")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.PENDING
     job.display = True
     yield job
 
 
 @pytest.fixture
 def running_barrier_job_response():
     job = BarrierFactories.BarrierJobResponseRunningFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test barrier job response - running")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.RUNNING
     job.display = True
     yield job
 
 
 @pytest.fixture
 def complete_barrier_job_response():
     job = BarrierFactories.BarrierJobResponseCompleteFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test barrier job response - complete")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.COMPLETE
     job.display = True
     yield job
 
 
 @pytest.fixture
 def failed_barrier_job_response():
     job = BarrierFactories.BarrierJobResponseFailedFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test barrier job response - failed")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.FAILED
     job.display = True
     yield job
 
 
 @pytest.fixture
 def pending_barrier_batch_job_response():
     job = BarrierFactories.BarrierBatchJobResponsePendingFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test barrier batch job response - pending")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.PENDING
     job.display = True
     yield job
 
 
 @pytest.fixture
 def running_barrier_batch_job_response():
     job = BarrierFactories.BarrierBatchJobResponseRunningFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test barrier batch job response - running")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.RUNNING
     job.display = True
     yield job
 
 
 @pytest.fixture
 def complete_barrier_batch_job_response():
     job = BarrierFactories.BarrierBatchJobResponseCompleteFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test barrier batch job response - complete")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.COMPLETE
     job.display = True
     yield job
 
 
 @pytest.fixture
 def failed_barrier_batch_job_response():
     job = BarrierFactories.BarrierBatchJobFailedFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test barrier batch job response - failed")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.FAILED
     job.display = True
     yield job
```

### Comparing `bert_schemas-1.18.0/bert_schemas/testing/fixtures/job/bec.py` & `bert_schemas-1.18.2/bert_schemas/testing/fixtures/job/bec.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,199 +1,200 @@
 """Pytest fixtures for BEC jobs"""
 
 import pytest
 
 from .... import job as job_schema
+from .... import qpu as qpu_schema
 from ...factories.helpers import add_notes, set_run
 from ...factories.job import bec as BecFactories
 
 
 @pytest.fixture
 def pending_bec_job():
     job = BecFactories.BecJobPendingFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test bec job - pending")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.PENDING
     job.display = True
     yield job
 
 
 @pytest.fixture
 def running_bec_job():
     job = BecFactories.BecJobRunningFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test bec job - running")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.RUNNING
     job.display = True
     yield job
 
 
 @pytest.fixture
 def complete_bec_job():
     job = BecFactories.BecJobCompleteFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test bec job - complete")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.COMPLETE
     job.display = True
     yield job
 
 
 @pytest.fixture
 def failed_bec_job():
     job = BecFactories.BecJobFailedFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test bec job - failed")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.FAILED
     job.display = True
     yield job
 
 
 @pytest.fixture
 def pending_bec_batch_job():
     job = BecFactories.BecBatchJobPendingFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test bec batch job - pending")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.PENDING
     job.display = True
     yield job
 
 
 @pytest.fixture
 def running_bec_batch_job():
     job = BecFactories.BecBatchJobRunningFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test bec batch job - running")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.RUNNING
     job.display = True
     yield job
 
 
 @pytest.fixture
 def complete_bec_batch_job():
     job = BecFactories.BecBatchJobCompleteFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test bec batch job - complete")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.COMPLETE
     job.display = True
     yield job
 
 
 @pytest.fixture
 def failed_bec_batch_job():
     job = BecFactories.BecBatchJobFailedFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test bec batch job - failed")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.FAILED
     job.display = True
     yield job
 
 
 @pytest.fixture
 def pending_bec_job_response():
     job = BecFactories.BecJobResponsePendingFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test bec job response - pending")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.PENDING
     job.display = True
     yield job
 
 
 @pytest.fixture
 def running_bec_job_response():
     job = BecFactories.BecJobResponseRunningFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test bec job response - running")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.RUNNING
     job.display = True
     yield job
 
 
 @pytest.fixture
 def complete_bec_job_response():
     job = BecFactories.BecJobResponseCompleteFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test bec job response - complete")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.COMPLETE
     job.display = True
     yield job
 
 
 @pytest.fixture
 def failed_bec_job_response():
     job = BecFactories.BecJobResponseFailedFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test bec job response - failed")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.FAILED
     job.display = True
     yield job
 
 
 @pytest.fixture
 def pending_bec_batch_job_response():
     job = BecFactories.BecBatchJobResponsePendingFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test bec batch job response - pending")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.PENDING
     job.display = True
     yield job
 
 
 @pytest.fixture
 def running_bec_batch_job_response():
     job = BecFactories.BecBatchJobResponseRunningFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test bec batch job response - running")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.RUNNING
     job.display = True
     yield job
 
 
 @pytest.fixture
 def complete_bec_batch_job_response():
     job = BecFactories.BecBatchJobResponseCompleteFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test bec batch job response - complete")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.COMPLETE
     job.display = True
     yield job
 
 
 @pytest.fixture
 def failed_bec_batch_job_response():
     job = BecFactories.BecBatchJobResponseFailedFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test bec batch job response - failed")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.FAILED
     job.display = True
     yield job
```

### Comparing `bert_schemas-1.18.0/bert_schemas/testing/fixtures/job/bragg.py` & `bert_schemas-1.18.2/bert_schemas/testing/fixtures/job/bragg.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,199 +1,200 @@
 """Pytest fixtures for BRAGG jobs"""
 
 import pytest
 
 from .... import job as job_schema
+from .... import qpu as qpu_schema
 from ...factories.helpers import add_notes, set_run
 from ...factories.job import bragg as BraggFactories
 
 
 @pytest.fixture
 def pending_bragg_job():
     job = BraggFactories.BraggJobPendingFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test bragg job - pending")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.PENDING
     job.display = True
     yield job
 
 
 @pytest.fixture
 def running_bragg_job():
     job = BraggFactories.BraggJobRunningFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test bragg job - running")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.RUNNING
     job.display = True
     yield job
 
 
 @pytest.fixture
 def complete_bragg_job():
     job = BraggFactories.BraggJobCompleteFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test bragg job - complete")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.COMPLETE
     job.display = True
     yield job
 
 
 @pytest.fixture
 def failed_bragg_job():
     job = BraggFactories.BraggJobFailedFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test bragg job - failed")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.FAILED
     job.display = True
     yield job
 
 
 @pytest.fixture
 def pending_bragg_batch_job():
     job = BraggFactories.BraggBatchJobPendingFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test bragg batch job - pending")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.PENDING
     job.display = True
     yield job
 
 
 @pytest.fixture
 def running_bragg_batch_job():
     job = BraggFactories.BraggBatchJobRunningFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test bragg batch job - running")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.RUNNING
     job.display = True
     yield job
 
 
 @pytest.fixture
 def complete_bragg_batch_job():
     job = BraggFactories.BraggBatchJobCompleteFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test bragg batch job - complete")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.COMPLETE
     job.display = True
     yield job
 
 
 @pytest.fixture
 def failed_bragg_batch_job():
     job = BraggFactories.BraggBatchJobFailedFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test bragg batch job - failed")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.FAILED
     job.display = True
     yield job
 
 
 @pytest.fixture
 def pending_bragg_job_response():
     job = BraggFactories.BraggJobResponsePendingFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test bragg job response - pending")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.PENDING
     job.display = True
     yield job
 
 
 @pytest.fixture
 def running_bragg_job_response():
     job = BraggFactories.BraggJobResponseRunningFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test bragg job response - running")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.RUNNING
     job.display = True
     yield job
 
 
 @pytest.fixture
 def complete_bragg_job_response():
     job = BraggFactories.BraggJobResponseCompleteFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test bragg job response - complete")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.COMPLETE
     job.display = True
     yield job
 
 
 @pytest.fixture
 def failed_bragg_job_response():
     job = BraggFactories.BraggJobResponseFailedFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test bragg job response - failed")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.FAILED
     job.display = True
     yield job
 
 
 @pytest.fixture
 def pending_bragg_batch_job_response():
     job = BraggFactories.BraggBatchJobResponsePendingFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test bragg batch job response - pending")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.PENDING
     job.display = True
     yield job
 
 
 @pytest.fixture
 def running_bragg_batch_job_response():
     job = BraggFactories.BraggBatchJobResponseRunningFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test bragg batch job response - running")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.RUNNING
     job.display = True
     yield job
 
 
 @pytest.fixture
 def complete_bragg_batch_job_response():
     job = BraggFactories.BraggBatchJobResponseCompleteFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test bragg batch job response - complete")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.COMPLETE
     job.display = True
     yield job
 
 
 @pytest.fixture
 def failed_bragg_batch_job_response():
     job = BraggFactories.BraggBatchJobResponseFailedFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test bragg batch job response - failed")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.FAILED
     job.display = True
     yield job
```

### Comparing `bert_schemas-1.18.0/bert_schemas/testing/fixtures/job/paint_1d.py` & `bert_schemas-1.18.2/bert_schemas/testing/fixtures/job/paint_1d.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,199 +1,200 @@
 """Pytest fixtures for PAINT_1D jobs"""
 
 import pytest
 
 from .... import job as job_schema
+from .... import qpu as qpu_schema
 from ...factories.helpers import add_notes, set_run
 from ...factories.job import paint_1d as Paint1DFactories
 
 
 @pytest.fixture
 def pending_paint_1d_job():
     job = Paint1DFactories.Paint1DJobPendingFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test paint_1d job - pending")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.PENDING
     job.display = True
     yield job
 
 
 @pytest.fixture
 def running_paint_1d_job():
     job = Paint1DFactories.Paint1DJobRunningFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test paint_1d job - running")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.RUNNING
     job.display = True
     yield job
 
 
 @pytest.fixture
 def complete_paint_1d_job():
     job = Paint1DFactories.Paint1DJobCompleteFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test paint_1d job - complete")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.COMPLETE
     job.display = True
     yield job
 
 
 @pytest.fixture
 def failed_paint_1d_job():
     job = Paint1DFactories.Paint1DJobFailedFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test paint_1d job - failed")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.FAILED
     job.display = True
     yield job
 
 
 @pytest.fixture
 def pending_paint_1d_batch_job():
     job = Paint1DFactories.Paint1DBatchJobPendingFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test paint_1d batch job - pending")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.PENDING
     job.display = True
     yield job
 
 
 @pytest.fixture
 def running_paint_1d_batch_job():
     job = Paint1DFactories.Paint1DBatchJobRunningFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test paint_1d batch job - running")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.RUNNING
     job.display = True
     yield job
 
 
 @pytest.fixture
 def complete_paint_1d_batch_job():
     job = Paint1DFactories.Paint1DBatchJobCompleteFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test paint_1d batch job - complete")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.COMPLETE
     job.display = True
     yield job
 
 
 @pytest.fixture
 def failed_paint_1d_batch_job():
     job = Paint1DFactories.Paint1DBatchJobFailedFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test paint_1d batch job - failed")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.FAILED
     job.display = True
     yield job
 
 
 @pytest.fixture
 def pending_paint_1d_job_response():
     job = Paint1DFactories.Paint1DJobResponsePendingFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test paint_1d job response - pending")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.PENDING
     job.display = True
     yield job
 
 
 @pytest.fixture
 def running_paint_1d_job_response():
     job = Paint1DFactories.Paint1DJobResponseRunningFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test paint_1d job response - running")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.RUNNING
     job.display = True
     yield job
 
 
 @pytest.fixture
 def complete_paint_1d_job_response():
     job = Paint1DFactories.Paint1DJobResponseCompleteFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test paint_1d job response - complete")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.COMPLETE
     job.display = True
     yield job
 
 
 @pytest.fixture
 def failed_paint_1d_job_response():
     job = Paint1DFactories.Paint1DJobResponseFailedFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test paint_1d job response - failed")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.FAILED
     job.display = True
     yield job
 
 
 @pytest.fixture
 def pending_paint_1d_batch_job_response():
     job = Paint1DFactories.Paint1DBatchJobResponsePendingFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test paint_1d batch job response - pending")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.PENDING
     job.display = True
     yield job
 
 
 @pytest.fixture
 def running_paint_1d_batch_job_response():
     job = Paint1DFactories.Paint1DBatchJobResponseRunningFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test paint_1d batch job response - running")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.RUNNING
     job.display = True
     yield job
 
 
 @pytest.fixture
 def complete_paint_1d_batch_job_response():
     job = Paint1DFactories.Paint1DBatchJobResponseCompleteFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test paint_1d batch job response - complete")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.COMPLETE
     job.display = True
     yield job
 
 
 @pytest.fixture
 def failed_paint_1d_batch_job_response():
     job = Paint1DFactories.Paint1DBatchJobResponseFailedFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test paint_1d batch job response - failed")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.FAILED
     job.display = True
     yield job
```

### Comparing `bert_schemas-1.18.0/bert_schemas/testing/fixtures/job/transistor.py` & `bert_schemas-1.18.2/bert_schemas/testing/fixtures/job/transistor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,199 +1,200 @@
 """Pytest fixtures for TRANSISTOR jobs"""
 
 import pytest
 
 from .... import job as job_schema
+from .... import qpu as qpu_schema
 from ...factories.helpers import add_notes, set_run
 from ...factories.job import transistor as TransistorFactories
 
 
 @pytest.fixture
 def pending_transistor_job():
     job = TransistorFactories.TransistorJobPendingFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test transistor job - pending")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.PENDING
     job.display = True
     yield job
 
 
 @pytest.fixture
 def running_transistor_job():
     job = TransistorFactories.TransistorJobRunningFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test transistor job - running")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.RUNNING
     job.display = True
     yield job
 
 
 @pytest.fixture
 def complete_transistor_job():
     job = TransistorFactories.TransistorJobCompleteFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test transistor job - complete")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.COMPLETE
     job.display = True
     yield job
 
 
 @pytest.fixture
 def failed_transistor_job():
     job = TransistorFactories.TransistorJobFailedFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test transistor job - failed")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.FAILED
     job.display = True
     yield job
 
 
 @pytest.fixture
 def pending_transistor_batch_job():
     job = TransistorFactories.TransistorBatchJobPendingFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test transistor batch job - pending")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.PENDING
     job.display = True
     yield job
 
 
 @pytest.fixture
 def running_transistor_batch_job():
     job = TransistorFactories.TransistorBatchJobRunningFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test transistor batch job - running")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.RUNNING
     job.display = True
     yield job
 
 
 @pytest.fixture
 def complete_transistor_batch_job():
     job = TransistorFactories.TransistorBatchJobCompleteFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test transistor batch job - complete")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.COMPLETE
     job.display = True
     yield job
 
 
 @pytest.fixture
 def failed_transistor_batch_job():
     job = TransistorFactories.TransistorBatchJobFailedFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test transistor batch job - failed")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.FAILED
     job.display = True
     yield job
 
 
 @pytest.fixture
 def pending_transistor_job_response():
     job = TransistorFactories.TransistorJobResponsePendingFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test transistor job response - pending")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.PENDING
     job.display = True
     yield job
 
 
 @pytest.fixture
 def running_transistor_job_response():
     job = TransistorFactories.TransistorJobResponseRunningFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test transistor job response - running")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.RUNNING
     job.display = True
     yield job
 
 
 @pytest.fixture
 def complete_transistor_job_response():
     job = TransistorFactories.TransistorJobResponseCompleteFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test transistor job response - complete")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.COMPLETE
     job.display = True
     yield job
 
 
 @pytest.fixture
 def failed_transistor_job_response():
     job = TransistorFactories.TransistorJobResponseFailedFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test transistor job response - failed")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.FAILED
     job.display = True
     yield job
 
 
 @pytest.fixture
 def pending_transistor_batch_job_response():
     job = TransistorFactories.TransistorBatchJobPendingFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test transistor batch job response - pending")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.PENDING
     job.display = True
     yield job
 
 
 @pytest.fixture
 def running_transistor_batch_job_response():
     job = TransistorFactories.TransistorBatchJobRunningFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test transistor batch job response - running")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.RUNNING
     job.display = True
     yield job
 
 
 @pytest.fixture
 def complete_transistor_batch_job_response():
     job = TransistorFactories.TransistorBatchJobCompleteFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test transistor batch job response - complete")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.COMPLETE
     job.display = True
     yield job
 
 
 @pytest.fixture
 def failed_transistor_batch_job_response():
     job = TransistorFactories.TransistorBatchJobFailedFactory.build()
     job = add_notes(job)
     job = set_run(job)
     job.name = job_schema.JobName("test transistor batch job response - failed")
-    job.qpu_name = job_schema.QPUName.BIGBERT
+    job.qpu_name = qpu_schema.QPUName.BIGBERT
     job.status = job_schema.JobStatus.FAILED
     job.display = True
     yield job
```

### Comparing `bert_schemas-1.18.0/bert_schemas/testing/schemas/job/__init__.py` & `bert_schemas-1.18.2/bert_schemas/testing/schemas/job/__init__.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.18.0/bert_schemas/testing/schemas/job/barrier.py` & `bert_schemas-1.18.2/bert_schemas/testing/schemas/job/barrier.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.18.0/bert_schemas/testing/schemas/job/bec.py` & `bert_schemas-1.18.2/bert_schemas/testing/schemas/job/bec.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.18.0/bert_schemas/testing/schemas/job/bragg.py` & `bert_schemas-1.18.2/bert_schemas/testing/schemas/job/bragg.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.18.0/bert_schemas/testing/schemas/job/paint_1d.py` & `bert_schemas-1.18.2/bert_schemas/testing/schemas/job/paint_1d.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.18.0/bert_schemas/testing/schemas/job/shared.py` & `bert_schemas-1.18.2/bert_schemas/testing/schemas/job/shared.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.18.0/bert_schemas/testing/schemas/job/transistor.py` & `bert_schemas-1.18.2/bert_schemas/testing/schemas/job/transistor.py`

 * *Files identical despite different names*

### Comparing `bert_schemas-1.18.0/bert_schemas/user.py` & `bert_schemas-1.18.2/bert_schemas/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
 class UserCreate(UserBase):
     external_user_id: external_user_id
 
 
 class UserSignUp(UserBase):
     questionnaire: RegistrationQandA
-    response: str
+    response: Optional[str]
 
     class Config:
         use_enum_values = True
 
 
 class Quota(BaseModel):
     quota_period: str
```

### Comparing `bert_schemas-1.18.0/pyproject.toml` & `bert_schemas-1.18.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bert-schemas"
-version = "1.18.0"
+version = "1.18.2"
 description = "Bert service schemas"
 authors = [
   "Larry Buza <lawrence.buza@coldquanta.com>",
   "Mike McGrath <michael.mcgrath@coldquanta.com>",
 ]
 license = "Apache-2.0"
 exclude = ["**/.pytest_cache/**/*", "**/__pycache__", ".gitignore"]
```

### Comparing `bert_schemas-1.18.0/setup.py` & `bert_schemas-1.18.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'matplotlib>=3.6.2,<3.7.0',
  'pydantic-factories>=1.17.0,<2.0.0',
  'pytest>=7.2.0,<8.0.0',
  'scipy>=1.10.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'bert-schemas',
-    'version': '1.18.0',
+    'version': '1.18.2',
     'description': 'Bert service schemas',
     'long_description': '# Bert Schemas\n\n[![License: Apache](https://img.shields.io/badge/License-Apache-yellow.svg)](https://opensource.org/licenses/Apache-2.0) [![Twitter](https://img.shields.io/twitter/url/https/twitter.com/Infleqtion.svg?style=social&label=Follow%20%40Infleqtion)](https://twitter.com/Infleqtion)\n\n## 🚀 Quick Install\n\n```python\npip install bert-schemas\n```\n\n## 🧭 Introduction\n\nThese Pydantic schemas are used by projects such as Oqtant for defining and validating REST payloads.\n',
     'author': 'Larry Buza',
     'author_email': 'lawrence.buza@coldquanta.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `bert_schemas-1.18.0/PKG-INFO` & `bert_schemas-1.18.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bert-schemas
-Version: 1.18.0
+Version: 1.18.2
 Summary: Bert service schemas
 License: Apache-2.0
 Author: Larry Buza
 Author-email: lawrence.buza@coldquanta.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

