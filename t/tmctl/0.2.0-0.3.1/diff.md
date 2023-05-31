# Comparing `tmp/tmctl-0.2.0.tar.gz` & `tmp/tmctl-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmctl-0.2.0.tar", last modified: Thu Apr 20 09:44:12 2023, max compression
+gzip compressed data, was "tmctl-0.3.1.tar", last modified: Wed May 31 10:09:57 2023, max compression
```

## Comparing `tmctl-0.2.0.tar` & `tmctl-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:44:12.042519 tmctl-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-20 09:44:12.042519 tmctl-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 09:44:12.042519 tmctl-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-20 09:43:51.000000 tmctl-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:44:12.042519 tmctl-0.2.0/tmctl/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-20 09:43:51.000000 tmctl-0.2.0/tmctl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32680 2023-04-20 09:43:51.000000 tmctl-0.2.0/tmctl/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-04-20 09:43:51.000000 tmctl-0.2.0/tmctl/tmctl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 09:44:12.042519 tmctl-0.2.0/tmctl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-20 09:44:12.000000 tmctl-0.2.0/tmctl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-20 09:44:12.000000 tmctl-0.2.0/tmctl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 09:44:12.000000 tmctl-0.2.0/tmctl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-20 09:44:12.000000 tmctl-0.2.0/tmctl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-20 09:44:12.000000 tmctl-0.2.0/tmctl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-20 09:44:12.000000 tmctl-0.2.0/tmctl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:09:57.658715 tmctl-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-31 10:09:57.658715 tmctl-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 10:09:57.658715 tmctl-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-31 10:09:41.000000 tmctl-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:09:57.654715 tmctl-0.3.1/tmctl/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-31 10:09:41.000000 tmctl-0.3.1/tmctl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34940 2023-05-31 10:09:41.000000 tmctl-0.3.1/tmctl/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-05-31 10:09:41.000000 tmctl-0.3.1/tmctl/tmctl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:09:57.658715 tmctl-0.3.1/tmctl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-31 10:09:57.000000 tmctl-0.3.1/tmctl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-31 10:09:57.000000 tmctl-0.3.1/tmctl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 10:09:57.000000 tmctl-0.3.1/tmctl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-31 10:09:57.000000 tmctl-0.3.1/tmctl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-31 10:09:57.000000 tmctl-0.3.1/tmctl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-31 10:09:57.000000 tmctl-0.3.1/tmctl.egg-info/top_level.txt
```

### Comparing `tmctl-0.2.0/tmctl/controller.py` & `tmctl-0.3.1/tmctl/controller.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,31 +15,31 @@
     output: str = "json"
     indent: int = 4
 
 
 @dataclass
 class CommonResponse:
     status: bool
-    error: dict = None
+    message: str = None
     data: dict = None
 
 
 class AdminClient(object):
     def __init__(self, common_option: CommonOption, base_url: str = None):
         self._common_option = common_option
         self._admin_url = self._common_option.admin_url
         self._output = self._common_option.output
         self._indent = self._common_option.indent
 
         self._base_url = base_url
 
     def _response_to_object(self, response: dict) -> CommonResponse:
         return CommonResponse(
-            status=response.get("status", False),
-            error=response.get("error", None) or {},
+            status=response.get("status", None) or None,
+            message=response.get("message", None) or {},
             data=response.get("data", None) or {},
         )
 
     def _extract_namespace(self, cluster) -> str:
         settings = cluster.get("settings", None) or {}
         namespace = settings.get("namespace", None) or None
 
@@ -70,194 +70,244 @@
 
         return proxy_name
 
     def _send_delete(self, url) -> bool:
         response = requests.delete(self._admin_url + url)
 
         if response.ok:
-            logging.debug(
-                f"url: {self._admin_url + url}, response ok, {response.status_code}, {response.text}"
-            )
-            return self._response_to_object(response.json()).status
+            return self._response_to_object(response.json())
         else:
-            logging.debug(
-                f"url: {self._admin_url + url}, response not ok, {response.status_code}, {response.text}"
-            )
-            return False
+            message = response.json()["message"]
+            print(f"[ERROR] reason : {message}")
+            exit(1)
 
     def _send_get(self, url, params=None) -> CommonResponse:
         params = params or {}
         response = requests.get(self._admin_url + url, params=params)
 
         if response.ok:
             return self._response_to_object(response.json())
         else:
+            message = response.json()["message"]
+            print(f"[ERROR] reason : {message}")
+            exit(1)
+
+    def _send_health_check_status_get(self, url, params=None) -> CommonResponse:
+        params = params or {}
+        response = requests.get(self._admin_url + url, params=params)
+
+        if response.ok:
+            return self._response_to_object(response.json())
+        else:
             return CommonResponse(
-                status=False,
-                error={"status_code": response.status_code, "text": response.text},
+                status=None,
+                message={"text": "cluster off"},
                 data=None,
             )
 
     def _send_binary_post(self, url, file_path, form_data):
         files = {"file": open(file_path, "rb")}
         # data = { "name": "test_name-changed", "target_path": "/etc/trino/test/222" }
 
         response = requests.post(self._admin_url + url, data=form_data, files=files)
         if response.ok:
             return self._response_to_object(response.json())
         else:
-            raise requests.exceptions.HTTPError(response.status_code)
+            message = response.json()["message"]
+            print(f"[ERROR] reason : {message}")
+            exit(1)
 
     def _send_download(self, url, params=None):
         # res = requests.get(url + f"/v1/files/1/download")
         # return res.content ? or write to file?
         response = requests.get(self._admin_url + url, params=params)
         if response.ok:
             return response.content
         else:
-            raise requests.exceptions.HTTPError(response.status_code)
+            message = response.json()["message"]
+            print(f"[ERROR] reason : {message}")
+            exit(1)
 
     def _send_post(self, url, json_data: dict = None, form_data: dict = None):
         json_data = json_data or {}
         response = requests.post(self._admin_url + url, data=form_data, json=json_data)
 
         if response.ok:
             return self._response_to_object(response.json())
         else:
-            logging.debug(response.text)
-            raise requests.exceptions.HTTPError(response.status_code)
+            message = response.json()["message"]
+            print(f"[ERROR] reason : {message}")
+            exit(1)
 
     def _yaml_load_all(self, filepath):
         yamls = []
 
-        for each in yaml.load_all(open(filepath, "r"), Loader=yaml.Loader):
-            yamls.append(each)
+        try:
+            for each in yaml.load_all(open(filepath, "r"), Loader=yaml.Loader):
+                yamls.append(each)
+        except Exception:
+            print(f"[ERROR] No such file or yaml : {filepath}")
+            exit(1)
 
         return yamls
 
     def delete(self, name: str, model_id: int = None):
+        """
+        delete command to name or model_id
+        """
         delete_response = None
         identifier = model_id or name
         return_value = None
 
         if model_id:
             delete_response = self._send_delete(f"{self._base_url}/{model_id}")
         elif name:
             response = self._send_get(f"{self._base_url}", params={"name": name})
 
-            if response.status:
-                models = response.data
-                if models:
-                    model = models[0]
+            models = response.data
+            if models:
+                model = models[0]
 
-                    model_id = model["id"]
+                model_id = model["id"]
 
-                    delete_response = self._send_delete(f"{self._base_url}/{model_id}")
+                delete_response = self._send_delete(f"{self._base_url}/{model_id}")
 
         if delete_response:
             return_value = f"identifier: {identifier} is successfully deleted!"
         else:
             return_value = f"identifier: {identifier} does not be successfully deleted!"
 
         return return_value
 
     def get(self, name):
+        """
+        get command to model name's info
+        """
         response = self._send_get(f"{self._base_url}", {"name": name})
-
-        if response.status:
-            for each in response.data:
-                self.print(each)
+        for each in response.data:
+            self._print(each)
 
     def list(self):
+        """
+        view command to group's list
+        """
         response = self._send_get(self._base_url)
-        if response.status:
-            self.print(response.data)
+        self._print(response.data)
 
     def ls(self):
+        """
+        view command to group's list
+        """
         return self.list()
 
-    def print(self, dictionary):
+    def _print(self, dictionary):
         dictionary = dictionary or {}
         if self._output == "json":
             print(json.dumps(dictionary, indent=self._indent))
         elif self._output == "yaml":
             print(yaml.dump(dictionary, indent=self._indent))
 
     def rm(self, name: str, model_id: int = None):
+        """
+        rm(delete) command to name or model_id
+        """
         return self.delete(name, model_id)
 
 
 class File(AdminClient):
+    """
+    File setting\n
+    preparation file
+        setting file yaml file
+    usage:
+        ex) tmctl <group> <command> <yaml file>
+        ex) tmctl file <ls(list), rm(delete), submit get> <manual.yaml>
+        ex) tmctl file ls
+        ex) tmctl file submit test.yaml
+    """
+
     def __init__(self, common_option: CommonOption):
         super(File, self).__init__(common_option, "/v1/files")
 
     def download(self, name, path=None):
+        """
+        file download command\n
+        """
         path = path or "./"
         response = self._send_get(f"{self._base_url}", {"name": name})
 
-        if response.status:
-            file = response.data[0]
+        file = response.data[0]
 
-            binary = self._send_download(f"{self._base_url}/{file['id']}/download")
+        binary = self._send_download(f"{self._base_url}/{file['id']}/download")
 
-            if binary:
-                file_path = os.path.join(path, file["file_name"])
-                with open(file_path, "wb") as _f:
-                    _f.write(binary)
+        if binary:
+            file_path = os.path.join(path, file["file_name"])
+            with open(file_path, "wb") as _f:
+                _f.write(binary)
 
-                self.print("download success.")
-            else:
-                self.print("empty binary")
+            self._print("download success.")
         else:
-            self.print("cannot download file")
+            self._print("empty binary")
+
+    def ls(self):
+        """
+        file list(ls) check\n
+        """
+        self.list()
+
+    def rm(self, name: str, model_id: int = None):
+        """
+        file delete(rm) command\n
+        """
+        return self.delete(name, model_id)
 
     def submit(self, path):
+        """
+        file submit(add) command\n
+        """
         yamls = self._yaml_load_all(path)
 
         for each in yamls:
             version = each.get("version", None)
             action_type = each.get("type", None)
 
             if version in ["v1/file"]:
                 file_config = each.get("file", None) or {}
                 name = file_config.get("name", None)
                 file_path = file_config.get("file_path", None)
                 target_path = file_config.get("target_path", None)
 
                 if not name:
                     print("invalid name", name)
-                    break
+                    exit(1)
 
                 if action_type == "create":
                     file_exists = os.path.exists(file_path)
 
                     if (not file_path) or (not file_exists):
                         print("invalid file_path", file_path)
-                        break
+                        exit(1)
 
                     response = self._send_binary_post(
                         "/v1/files",
                         file_path,
                         form_data={"name": name, "target_path": target_path},
                     )
+                    self._print(response.data)
 
-                    if response.status:
-                        self.print(response.data)
-                    else:
-                        logging.warning("file failed")
                 elif action_type == "update":
                     file_id = file_config.get("id", None)
 
                     if file_id:
                         if file_path:
                             file_exists = os.path.exists(file_path)
 
                             if (not file_path) or (not file_exists):
                                 print("invalid file_path", file_path)
-                                break
+                                exit(1)
 
                             response = self._send_binary_post(
                                 f"/v1/files/{file_id}",
                                 file_path,
                                 form_data={
                                     "name": name,
                                     "target_path": target_path,
@@ -268,182 +318,206 @@
                                 f"/v1/files/{file_id}",
                                 form_data={
                                     "name": name,
                                     "target_path": target_path,
                                 },
                             )
 
-                        if response.status:
-                            self.print(response.data)
-                        else:
-                            logging.warning("file submit failed")
+                        self._print(response.data)
 
 
 class Catalog(AdminClient):
+    """
+    catalog setting\n
+    preparation file
+        setting catalog yaml file
+    usage:
+        ex) tmctl <group> <command> <yaml file>
+        ex) tmctl catalog <ls(list), rm(delete), submit get> <manual.yaml>
+        ex) tmctl catalog ls
+        ex) tmctl catalog submit test.yaml
+    """
+
     def __init__(self, common_option: CommonOption):
         super(Catalog, self).__init__(common_option, "/v1/catalogs")
 
-    def list(self):
-        response = self._send_get("/v1/catalogs")
-        if response.status:
-            self.print(response.data)
-
     def ls(self):
+        """
+        catalog list(ls) check\n
+        """
         self.list()
 
     def rm(self, name: str = None, catalog_id: int = None):
+        """
+        catalog delete(rm) command\n
+        """
         return self.delete(name, catalog_id)
 
     def submit(self, path):
+        """
+        catalog submit(add)\n
+        """
         yamls = self._yaml_load_all(path)
 
         for each in yamls:
             version = each.get("version", None)
             action_type = each.get("type", None)
 
             if version in ["v1/catalog"]:
                 catalog_config = each.get("catalog", None) or {}
                 name = catalog_config.get("name", None)
                 catalog_type = catalog_config.get("catalog_type", None)
                 properties = catalog_config.get("properties", None)
 
                 if not name:
                     print("invalid name", name)
-                    break
+                    exit(1)
 
                 if not catalog_type:
                     print("invalid chart name", catalog_type)
-                    break
+                    exit(1)
 
                 if action_type == "create":
                     response = self._send_post(
                         "/v1/catalogs",
                         json_data={
                             "name": name,
                             "catalog_type": catalog_type,
                             "properties": properties,
                         },
                     )
 
-                    if response.status:
-                        self.print(response.data)
-                    else:
-                        logging.warning("chart submit failed")
+                    self._print(response.data)
                 elif action_type == "update":
                     catalog_id = catalog_config.get("id", None)
 
                     if catalog_id:
                         response = self._send_post(
                             f"/v1/catalogs/{catalog_id}",
                             json_data={
                                 "name": name,
                                 "catalog_type": catalog_type,
                                 "properties": properties,
                             },
                         )
-
-                        if response.status:
-                            self.print(response.data)
-                        else:
-                            logging.warning("catalog submit failed")
+                        self._print(response.data)
+                    else:
+                        message = "catalog_id is None"
+                        print(f"[ERROR] reason : {message}")
+                        exit(1)
+                else:
+                    message = "invalid action type"
+                    print(f"[ERROR] reason : {message}")
+                    exit(1)
 
 
 class Cluster(AdminClient):
+    """
+    cluster setting\n
+    preparation file
+        setting cluster yaml file
+    usage:
+        ex) tmctl <group> <command> <yaml file>
+        ex) tmctl cluster <ls(list), rm(delete), submit get> <manual.yaml>
+        ex) tmctl cluster ls
+        ex) tmctl cluster submit test.yaml
+    """
+
     def __init__(self, url):
         super(Cluster, self).__init__(url, "/v1/clusters")
 
     def delete(self, name, force=False, refresh=1, timeout=120):
+        """
+        cluster delete(rm) command\n
+        """
         response = self._send_get("/v1/clusters", {"name": name})
 
-        if response.status:
-            clusters = response.data
+        clusters = response.data
 
-            if clusters:
-                cluster = clusters[0]
-                health_check = self._health_check_status(cluster["id"])
-
-                if health_check:
-                    if force:
-                        self.off(name=name, refresh=refresh, timeout=timeout)
-                    else:
-                        print("Cluster is on. please off the cluster first.")
-                        logging.warning("Cluster is on. please off the cluster first.")
-                        return
+        if clusters:
+            cluster = clusters[0]
+            health_check = self._health_check_status(cluster["id"]).data
+
+            if health_check:
+                if force:
+                    self.off(name=name, refresh=refresh, timeout=timeout)
+
+                else:
+                    print("Cluster is on. please off the cluster first.")
+                    logging.warning("Cluster is on. please off the cluster first.")
+                    exit(1)
 
-            super().delete(name)
+        super().delete(name)
 
     def _health_check_status(self, cluster_id):
-        response = self._send_get(f"/v1/clusters/{cluster_id}/gateway/health")
-
-        if response.status:
-            logging.debug(f"{response.data}")
-            return True
-        else:
-            return False
+        response = self._send_health_check_status_get(
+            f"/v1/clusters/{cluster_id}/gateway/health"
+        )
+        return response
 
     def _waiting_release(self, release_id, refresh, timeout):
         start_time = datetime.datetime.now(datetime.timezone.utc)
 
         response = self._send_get(f"/v1/releases/{release_id}")
         finished = False
         timeout_flag = False
-        release = response.data[0] if response.status else None
+        release = response.data[0]
 
         while release.get("status", "QUEUED") not in ["FINISHED", "FAILED"]:
             time.sleep(refresh)
 
             current_time = datetime.datetime.now(datetime.timezone.utc)
 
             if (current_time - start_time).seconds > timeout:
                 timeout_flag = True
-                break
+                exit(1)
 
             response = self._send_get(f"/v1/releases/{release_id}")
-            release = response.data[0] if response.status else None
-            self.print(release)
+            release = response.data[0]
+            self._print(release)
 
         if timeout_flag:
             finished = False
         else:
             finished = True
 
         return finished
 
     def _waiting_and_get_release_log(self, release_id, refresh, timeout):
         start_time = datetime.datetime.now(datetime.timezone.utc)
 
         response = self._send_get(f"/v1/releases/{release_id}/log")
-        celery_response = response.data[0] if response.status else None
+        celery_response = response.data[0]
 
         timeout_flag = False
         while celery_response.get("state", "PENDING") not in ["SUCCESS", "FAILURE"]:
             time.sleep(refresh)
             current_time = datetime.datetime.now(datetime.timezone.utc)
 
             if (current_time - start_time).seconds > timeout:
                 timeout_flag = True
-                break
+                exit(1)
 
             response = self._send_get(f"/v1/releases/{release_id}/log")
-            celery_response = response.data[0] if response.status else None
+            celery_response = response.data[0]
 
-            self.print(celery_response)
+            self._print(celery_response)
 
         if timeout_flag:
             response = None
 
         return celery_response
 
     def _execute_and_get_helm_release_log(self, url, refresh, timeout):
         response = self._send_post(url)
-        release = response.data[0] if response.status else None
+        release = response.data[0]
 
         release_id = release["id"]
 
-        self.print(release)
+        self._print(release)
 
         if not self._waiting_release(release_id, refresh, timeout):
             return None
 
         log_response = self._waiting_and_get_release_log(release_id, refresh, timeout)
 
         return log_response
@@ -455,54 +529,63 @@
 
     def _do_upgrade(self, cluster_id, refresh, timeout):
         return self._execute_and_get_helm_release_log(
             f"/v1/clusters/{cluster_id}/upgrade", refresh, timeout
         )
 
     def list(self):
+        """
+        cluster list(ls) check\n
+        """
         response = self._send_get(self._base_url)
 
-        if response.status:
-            clusters = response.data
+        clusters = response.data
 
-            for cluster in clusters:
-                cluster["status"] = (
-                    "ON" if self._health_check_status(cluster["id"]) else "OFF"
-                )
+        for cluster in clusters:
+            cluster["status"] = (
+                "ON" if self._health_check_status(cluster["id"]).data else "OFF"
+            )
 
-            self.print(clusters)
+        self._print(clusters)
 
     def ls(self):
+        """
+        cluster list(ls) check\n
+        """
         self.list()
 
     def get(self, name):
+        """
+        cluster info(ON/OFF) get\n
+        """
         response = self._send_get("/v1/clusters", {"name": name})
 
-        if response.status:
-            clusters = response.data
+        clusters = response.data
 
-            if clusters:
-                cluster = clusters[0]
+        if clusters:
+            cluster = clusters[0]
 
-                cluster["status"] = (
-                    "ON" if self._health_check_status(cluster["id"]) else "OFF"
-                )
+            cluster["status"] = (
+                "ON" if self._health_check_status(cluster["id"]).data else "OFF"
+            )
 
-                self.print(cluster)
+            self._print(cluster)
 
     def status(self, name, refresh=1, timeout=120):
+        """
+        cluster status get\n
+        """
         cluster = None
 
         response = self._send_get("/v1/clusters", params={"name": name})
 
-        if response.status:
-            clusters = response.data
+        clusters = response.data
 
-            if clusters:
-                cluster = clusters[0]
+        if clusters:
+            cluster = clusters[0]
 
         if not cluster:
             return
 
         cluster_status_response = self._execute_and_get_helm_release_log(
             f"/v1/clusters/{cluster['id']}/status", refresh, timeout
         )
@@ -520,23 +603,31 @@
         return_value = response_log.get("return", {}) or {}
 
         is_proxy_installed = len(return_value.get("stdout", "")) > 0
 
         status = {
             "cluster installed:": is_cluster_installed,
             "proxy installed:": is_proxy_installed,
-            "cluster status (health check):": self._health_check_status(cluster["id"]),
+            "cluster status (health check):": "ON"
+            if self._health_check_status(cluster["id"]).data
+            else "OFF",
         }
 
-        self.print(status)
+        self._print(status)
 
     def rm(self, name, force=False, refresh=1, timeout=120):
+        """
+        cluster delete(rm) command\n
+        """
         return self.delete(name, force, refresh, timeout)
 
     def submit(self, path):
+        """
+        cluster submit(add)\n
+        """
         yamls = self._yaml_load_all(path)
 
         for each in yamls:
             version = each.get("version", None)
             action_type = each.get("type", None)
 
             if version in ["v1/cluster"]:
@@ -548,80 +639,75 @@
                 chart_name = cluster_config.get("chart", None)
 
                 params = {"name": chart_name}
 
                 response = self._send_get("/v1/charts", params=params)
 
                 chart_id = None
-                if response.status:
-                    charts = response.data
-                    if charts:
-                        chart_id = charts[0]["id"]
+                charts = response.data
+                if charts:
+                    chart_id = charts[0]["id"]
 
-                    if not chart_id:
-                        raise Exception("invalid chart options")
+                if not chart_id:
+                    raise Exception("invalid chart options")
 
                 catalog_config = cluster_config.get("catalogs", None) or []
 
                 catalog_list = []
 
                 for catalog_name in catalog_config:
                     response = self._send_get(f"/v1/catalogs?name={catalog_name}")
 
-                    if response.status:
-                        catalogs = response.data
+                    catalogs = response.data
 
-                        if catalogs:
-                            catalog_list.append(catalogs[0]["id"])
+                    if catalogs:
+                        catalog_list.append(catalogs[0]["id"])
 
                 file_config = cluster_config.get("files", None) or []
 
                 file_list = []
 
                 for file_name in file_config:
                     response = self._send_get(f"/v1/files?name={file_name}")
 
-                    if response.status:
-                        files = response.data
+                    files = response.data
 
-                        if files:
-                            file_list.append(files[0]["id"])
+                    if files:
+                        file_list.append(files[0]["id"])
 
                 settings = cluster_config.get("settings", None) or {}
 
                 if not name:
                     print("invalid name", name)
-                    break
+                    exit(1)
 
                 if not chart_id:
                     print("invalid chart id or chart_name", chart_id, chart_name)
-                    break
+                    exit(1)
 
                 if action_type == "create":
                     response = self._send_post(
                         "/v1/clusters",
                         json_data={
                             "name": name,
                             "chart_id": chart_id,
                             "catalog_list": catalog_list,
                             "file_list": file_list,
                             "settings": settings,
                         },
                     )
 
-                    if response.status:
-                        clusters = response.data
+                    clusters = response.data
+
+                    if clusters:
+                        cluster = clusters[0]
+                        self._print(cluster)
+                        if direct_on:
+                            self.on(cluster_id=cluster["id"], is_update=False)
 
-                        if clusters:
-                            cluster = clusters[0]
-                            self.print(cluster)
-                            if direct_on:
-                                self.on(cluster_id=cluster["id"], is_update=False)
-                    else:
-                        logging.warning("cluster submit failed")
                 elif action_type == "update":
                     cluster_id = cluster_config.get("id", None)
 
                     if cluster_id:
                         response = self._send_post(
                             f"/v1/clusters/{cluster_id}",
                             json_data={
@@ -629,47 +715,50 @@
                                 "chart_id": chart_id,
                                 "catalog_list": catalog_list,
                                 "file_list": file_list,
                                 "settings": settings,
                             },
                         )
 
-                        if response.status:
-                            clusters = response.data
+                        clusters = response.data
 
-                            if clusters:
-                                cluster = clusters[0]
-                                self.print(cluster)
-                                if direct_on:
-                                    self.on(cluster_id=cluster_id, is_update=True)
-                        else:
-                            logging.warning("cluster submit failed")
+                        if clusters:
+                            cluster = clusters[0]
+                            self._print(cluster)
+                            if direct_on:
+                                self.on(cluster_id=cluster_id, is_update=True)
                     else:
-                        logging.warning("cluster id is unknown.")
+                        message = "cluster_id is None"
+                        # logging.warning("cluster id is unknown.")
+                        print(f"[ERROR] reason : {message}")
+                        exit(1)
+                else:
+                    message = "invalid action type"
+                    print(f"[ERROR] reason : {message}")
+                    exit(1)
 
     def on(self, name=None, cluster_id=None, is_update=False, refresh=1, timeout=120):
+        """
+        cluster on command
+        """
         cluster = None
         cluster_identifer = name or cluster_id
 
         if cluster_id:
             response = self._send_get(f"/v1/clusters/{cluster_id}")
-
-            if response.status:
-                cluster = response.data[0]
+            cluster = response.data[0]
         elif name:
             response = self._send_get("/v1/clusters", params={"name": name})
-
-            if response.status:
-                clusters = response.data
-                if clusters:
-                    cluster = clusters[0]
+            clusters = response.data
+            if clusters:
+                cluster = clusters[0]
 
         if not cluster:
             logging.warning(f"cluster: {cluster_identifer} is invalid")
-            return
+            exit(1)
 
         cluster_id = cluster["id"]
         namespace_name = self._extract_namespace(cluster)
 
         response = {}
 
         if is_update:
@@ -683,90 +772,112 @@
         if response_log.get("success", False) or False:
             logging.info(return_value)
             logging.info("cluster install is succeeded!")
             logging.info("try to register proxy to api gateway...")
         else:
             logging.warning(response_log)
             logging.warning("cluster install failed")
-            return
+            exit(1)
 
         proxy_manifest = self._execute_and_get_helm_release_log(
             f"/v1/clusters/{cluster_id}/proxy/manifest", refresh, timeout
         )
 
         if not proxy_manifest:
             logging.warning("getting cluster proxy information is failed")
-            return None
+            exit(1)
 
         response_log = proxy_manifest.get("log", {}) or {}
         return_value = response_log.get("return", {}) or {}
 
         if response_log.get("success", False) or False:
             pass
         else:
             logging.warning("get proxy info failed")
-            return
+            exit(1)
 
         proxy_name = self._parse_proxy_service(return_value.get("stdout", ""))
 
         service_name = f"""{proxy_name}.{namespace_name}"""
 
         response = self._send_post(
             f"/v1/clusters/{cluster_id}/gateway/register",
             {"service_name": service_name},
         )
 
         logging.info(response)
 
     def off(self, name=None, cluster_id=None, refresh=1, timeout=120):
+        """
+        cluster off command(not delete)
+        """
         cluster = None
 
         if cluster_id:
             response = self._send_get(f"/v1/clusters/{cluster_id}")
 
-            if response.status:
-                cluster = response.data[0]
+            cluster = response.data[0]
         if name:
             response = self._send_get("/v1/clusters", params={"name": name})
 
-            if response.status:
-                clusters = response.data
-                if clusters:
-                    cluster = clusters[0]
+            clusters = response.data
+            if clusters:
+                cluster = clusters[0]
 
         if not cluster:
             logging.warning("cluster id or name is invalid")
-            return
+            exit(1)
 
         cluster_id = cluster["id"]
 
         response = self._send_delete(f"/v1/clusters/{cluster_id}/gateway/deregister")
         logging.info(response)
 
         uninstall_response = self._execute_and_get_helm_release_log(
             f"/v1/clusters/{cluster_id}/uninstall", refresh, timeout
         )
 
         if not uninstall_response:
-            self.print("cluster uninstall is failed")
+            self._print("cluster uninstall is failed")
+            exit(1)
         else:
-            self.print("cluster uninstall is succeeded!")
+            self._print("cluster uninstall is succeeded!")
 
 
 class HelmChart(AdminClient):
+    """
+    helm_chart setting\n
+    preparation file
+        setting helm_chart yaml file
+    usage:
+        ex) tmctl <group> <command> <yaml file>
+        ex) tmctl helm_chart <ls(list), rm(delete), submit get> <manual.yaml>
+        ex) tmctl helm_chart ls
+        ex) tmctl helm_chart submit test.yaml
+    """
+
     def __init__(self, url):
         super(HelmChart, self).__init__(url, "/v1/charts")
 
     def ls(self):
+        """
+        helm_chart list check\n
+        """
         self.list()
 
     def rm(self, name: str = None, chart_id: int = None):
+        """
+        helm_chart remove\n
+        """
         return self.delete(name, chart_id)
 
     def submit(self, path):
+        """
+        helm_chart submit(add)\n
+        """
         yamls = self._yaml_load_all(path)
 
         for each in yamls:
             version = each.get("version", None)
             action_type = each.get("type", None)
 
             if version in ["v1/chart"]:
@@ -776,120 +887,149 @@
                 chart_version = chart_config.get("version", None)
                 registry = chart_config.get("registry", None)
                 repository = chart_config.get("repository", None)
                 values = chart_config.get("values", None)
 
                 if not name:
                     print("invalid name", name)
-                    break
+                    exit(1)
 
                 if not chart_name:
                     print("invalid chart name", chart_name)
-                    break
+                    exit(1)
 
                 if action_type == "create":
                     response = self._send_post(
                         "/v1/charts",
                         json_data={
                             "name": name,
                             "chart_name": chart_name,
                             "version": chart_version,
                             "registry": registry,
                             "repository": repository,
                             "values": values,
                         },
                     )
 
-                    if response.status:
-                        self.print(response.data[0])
-                    else:
-                        logging.warning("chart submit failed")
+                    self._print(response.data[0])
                 elif action_type == "update":
                     chart_id = chart_config.get("id", None)
 
                     if chart_id:
                         response = self._send_post(
                             f"/v1/charts/{chart_id}",
                             json_data={
                                 "name": name,
                                 "chart_name": chart_name,
                                 "version": chart_version,
                                 "registry": registry,
                                 "repository": repository,
                             },
                         )
-
-                        if response.status:
-                            self.print(response.data[0])
-                        else:
-                            logging.warning("chart submit failed")
+                        self._print(response.data[0])
+                    else:
+                        message = "chart_id is None"
+                        print(f"[ERROR] reason : {message}")
+                        exit(1)
+                else:
+                    message = "invalid action type"
+                    print(f"[ERROR] reason : {message}")
+                    exit(1)
 
 
 class MountFile(AdminClient):
+    """
+    Mount File setting\n
+    preparation file
+        setting mount yaml file
+    usage:
+        ex) tmctl <group> <command> <yaml file>
+        ex) tmctl mount <ls(list), rm(delete), submit get> <manual.yaml>
+        ex) tmctl mount ls
+        ex) tmctl mount submit test.yaml
+    """
+
     def __init__(self, url):
         super(MountFile, self).__init__(url, "/v1/mounts")
 
     def get(self, mount_path):
+        """
+        mount file info get\n
+        """
         response = self._send_get(f"{self._base_url}", {"mount_path": mount_path})
-
-        if response.status:
-            for each in response.data:
-                self.print(each)
+        for each in response.data:
+            self._print(each)
 
     def delete(self, mount_path: str, model_id: int = None):
+        """
+        mount file delete(rm) command\n
+        """
         delete_response = None
         identifier = model_id or mount_path
         return_value = None
 
         if model_id:
             delete_response = self._send_delete(f"{self._base_url}/{model_id}")
         elif mount_path:
             response = self._send_get(
                 f"{self._base_url}", params={"mount_path": mount_path}
             )
 
-            if response.status:
-                models = response.data
-                if models:
-                    model = models[0]
+            models = response.data
+            if models:
+                model = models[0]
 
-                    model_id = model["id"]
+                model_id = model["id"]
 
-                    delete_response = self._send_delete(f"{self._base_url}/{model_id}")
+                delete_response = self._send_delete(f"{self._base_url}/{model_id}")
 
         if delete_response:
             return_value = f"identifier: {identifier} is successfully deleted!"
         else:
             return_value = f"identifier: {identifier} does not be successfully deleted!"
 
         return return_value
 
     def download(self, mount_path, path=None):
+        """
+        mount file download command\n
+        """
         path = path or "./"
         response = self._send_get(f"{self._base_url}", {"mount_path": mount_path})
 
-        if response.status:
-            mount_file = response.data[0]
+        mount_file = response.data[0]
 
-            binary = self._send_download(
-                f"{self._base_url}/{mount_file['id']}/download"
-            )
+        binary = self._send_download(f"{self._base_url}/{mount_file['id']}/download")
 
-            if binary:
-                file_path = os.path.join(path, mount_file["file_name"])
-                with open(file_path, "wb") as _f:
-                    _f.write(binary)
-
-                self.print("download success.")
-            else:
-                self.print("empty binary")
+        if binary:
+            file_path = os.path.join(path, mount_file["file_name"])
+            with open(file_path, "wb") as _f:
+                _f.write(binary)
+
+            self._print("download success.")
         else:
-            self.print("cannot download file")
+            self._print("empty binary")
+            exit(1)
+
+    def ls(self):
+        """
+        mount file list(ls) check\n
+        """
+        self.list()
+
+    def rm(self, mount_path: str, model_id: int = None):
+        """
+        mount file delete(rm) command\n
+        """
+        return self.delete(mount_path, model_id)
 
     def submit(self, path):
+        """
+        mount file submit(add) command\n
+        """
         yamls = self._yaml_load_all(path)
 
         for each in yamls:
             version = each.get("version", None)
             action_type = each.get("type", None)
 
             if version in ["v1/mount"]:
@@ -898,25 +1038,25 @@
                 mount_path = file_config.get("mount_path", None)
                 target_path = file_config.get("target_path", None)
                 refresh = file_config.get("refresh", None) or False
 
                 if not refresh:
                     if not source_path:
                         print("invalid path", source_path)
-                        break
+                        exit(1)
 
                     file_exists = os.path.exists(source_path)
 
                     if not file_exists:
                         print("invalid currnet source fil path", source_path)
-                        break
+                        exit(1)
 
                     if not mount_path:
                         print("invalid mount_path", mount_path)
-                        break
+                        exit(1)
 
                 if action_type == "create":
                     response = None
                     if refresh:
                         response = self._send_post(
                             "/v1/mounts",
                             form_data={
@@ -931,28 +1071,22 @@
                             source_path,
                             form_data={
                                 "mount_path": mount_path,
                                 "target_path": target_path,
                             },
                         )
 
-                    if response.status:
-                        self.print(response.data)
-                    else:
-                        logging.warning("mount file create failed")
+                    self._print(response.data)
                 elif action_type == "update":
                     mount_file_id = file_config.get("id", None)
 
                     if mount_file_id:
                         response = self._send_binary_post(
                             f"/v1/mounts/{mount_file_id}",
                             source_path,
                             form_data={
                                 "mount_path": mount_path,
                                 "target_path": target_path,
                             },
                         )
 
-                        if response.status:
-                            self.print(response.data)
-                        else:
-                            logging.warning("mount file update failed")
+                        self._print(response.data)
```

