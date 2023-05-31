# Comparing `tmp/flux-local-1.2.0.tar.gz` & `tmp/flux-local-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flux-local-1.2.0.tar", last modified: Wed May 24 02:37:09 2023, max compression
+gzip compressed data, was "flux-local-1.3.0.tar", last modified: Wed May 31 01:52:17 2023, max compression
```

## Comparing `flux-local-1.2.0.tar` & `flux-local-1.3.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:37:09.747829 flux-local-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-24 02:36:58.000000 flux-local-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9853 2023-05-24 02:37:09.747829 flux-local-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-05-24 02:36:58.000000 flux-local-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:37:09.743829 flux-local-1.2.0/flux_local/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-24 02:36:58.000000 flux-local-1.2.0/flux_local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-24 02:36:58.000000 flux-local-1.2.0/flux_local/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-24 02:36:58.000000 flux-local-1.2.0/flux_local/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20614 2023-05-24 02:36:58.000000 flux-local-1.2.0/flux_local/git_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-05-24 02:36:58.000000 flux-local-1.2.0/flux_local/helm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-05-24 02:36:58.000000 flux-local-1.2.0/flux_local/kustomize.py
--rw-r--r--   0 runner    (1001) docker     (123)    15085 2023-05-24 02:36:58.000000 flux-local-1.2.0/flux_local/manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:37:09.743829 flux-local-1.2.0/flux_local/tool/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-24 02:36:58.000000 flux-local-1.2.0/flux_local/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-24 02:36:58.000000 flux-local-1.2.0/flux_local/tool/build.py
--rw-r--r--   0 runner    (1001) docker     (123)    14698 2023-05-24 02:36:58.000000 flux-local-1.2.0/flux_local/tool/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-24 02:36:58.000000 flux-local-1.2.0/flux_local/tool/flux_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-24 02:36:58.000000 flux-local-1.2.0/flux_local/tool/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-05-24 02:36:58.000000 flux-local-1.2.0/flux_local/tool/get.py
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-05-24 02:36:58.000000 flux-local-1.2.0/flux_local/tool/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    13798 2023-05-24 02:36:58.000000 flux-local-1.2.0/flux_local/tool/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10083 2023-05-24 02:36:58.000000 flux-local-1.2.0/flux_local/tool/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:37:09.743829 flux-local-1.2.0/flux_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9853 2023-05-24 02:37:09.000000 flux-local-1.2.0/flux_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-24 02:37:09.000000 flux-local-1.2.0/flux_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 02:37:09.000000 flux-local-1.2.0/flux_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-24 02:37:09.000000 flux-local-1.2.0/flux_local.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-24 02:37:09.000000 flux-local-1.2.0/flux_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-24 02:37:09.000000 flux-local-1.2.0/flux_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-24 02:37:09.747829 flux-local-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-24 02:36:58.000000 flux-local-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:37:09.743829 flux-local-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-24 02:36:58.000000 flux-local-1.2.0/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (123)    13334 2023-05-24 02:36:58.000000 flux-local-1.2.0/tests/test_git_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-24 02:36:58.000000 flux-local-1.2.0/tests/test_helm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-05-24 02:36:58.000000 flux-local-1.2.0/tests/test_kustomize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-24 02:36:58.000000 flux-local-1.2.0/tests/test_manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:52:17.241509 flux-local-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-31 01:52:06.000000 flux-local-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12298 2023-05-31 01:52:17.241509 flux-local-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-05-31 01:52:06.000000 flux-local-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:52:17.237509 flux-local-1.3.0/flux_local/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-31 01:52:06.000000 flux-local-1.3.0/flux_local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-05-31 01:52:06.000000 flux-local-1.3.0/flux_local/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-31 01:52:06.000000 flux-local-1.3.0/flux_local/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24461 2023-05-31 01:52:06.000000 flux-local-1.3.0/flux_local/git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-05-31 01:52:06.000000 flux-local-1.3.0/flux_local/helm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9572 2023-05-31 01:52:06.000000 flux-local-1.3.0/flux_local/kustomize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15565 2023-05-31 01:52:06.000000 flux-local-1.3.0/flux_local/manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:52:17.241509 flux-local-1.3.0/flux_local/tool/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-31 01:52:06.000000 flux-local-1.3.0/flux_local/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-31 01:52:06.000000 flux-local-1.3.0/flux_local/tool/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16262 2023-05-31 01:52:06.000000 flux-local-1.3.0/flux_local/tool/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-31 01:52:06.000000 flux-local-1.3.0/flux_local/tool/flux_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-31 01:52:06.000000 flux-local-1.3.0/flux_local/tool/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7317 2023-05-31 01:52:06.000000 flux-local-1.3.0/flux_local/tool/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-05-31 01:52:06.000000 flux-local-1.3.0/flux_local/tool/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14233 2023-05-31 01:52:06.000000 flux-local-1.3.0/flux_local/tool/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-05-31 01:52:06.000000 flux-local-1.3.0/flux_local/tool/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:52:17.241509 flux-local-1.3.0/flux_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12298 2023-05-31 01:52:17.000000 flux-local-1.3.0/flux_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-31 01:52:17.000000 flux-local-1.3.0/flux_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 01:52:17.000000 flux-local-1.3.0/flux_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-31 01:52:17.000000 flux-local-1.3.0/flux_local.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-31 01:52:17.000000 flux-local-1.3.0/flux_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-31 01:52:17.000000 flux-local-1.3.0/flux_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-31 01:52:17.241509 flux-local-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-31 01:52:06.000000 flux-local-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 01:52:17.241509 flux-local-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-31 01:52:06.000000 flux-local-1.3.0/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14237 2023-05-31 01:52:06.000000 flux-local-1.3.0/tests/test_git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-31 01:52:06.000000 flux-local-1.3.0/tests/test_helm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-05-31 01:52:06.000000 flux-local-1.3.0/tests/test_kustomize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-31 01:52:06.000000 flux-local-1.3.0/tests/test_manifest.py
```

### Comparing `flux-local-1.2.0/LICENSE` & `flux-local-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flux-local-1.2.0/PKG-INFO` & `flux-local-1.3.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: flux-local
-Version: 1.2.0
-Summary: flux-local is a python library and set of tools for managing a flux gitops repository, with validation steps to help improve quality of commits, PRs, and general local testing.
-Home-page: https://github.com/allenporter/flux-local
-Author: Allen Porter
-Author-email: allen.porter@gmail.com
-License: Apache-2.0
-Classifier: License :: OSI Approved :: Apache Software License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 flux-local is a set of tools and libraries for managing a local flux gitops repository focused on validation steps to help improve quality of commits, PRs, and general local testing.
 
 This library uses command line tools like kustomize and helm to replicate the behavior of
 flux to gather objects in the cluster. It only looks at the local git repo, and not a live
 cluster. However, this is fine since the local repository has enough information and the
 definition is simple. Secrets are ignored as the content is not needed to validate the
 cluster is creating valid objects.
@@ -242,11 +230,98 @@
 
 clusters/dev .....................................                                                      [ 45%]
 clusters/prod ............................................                                              [100%]
 
 ======================================== 81 passed in 75.40s (0:01:15) ========================================
 ```
 
+## GitHub Action
+
+You may use `flux-local` as a github action to verify the health of the cluster on changes
+or PRs.
+
+### test action
+
+The `test` action will validate the cluster will build, and can optionally
+validate flux `HelmRelease` builds and also verify that all objects pass
+kyverno policies (e.g. for determining there are no deprecated api resources
+or that ingress objects are valid).
+
+This example will run `flux-local test` against the cluster in `clusters/prod` with
+helm release expansion enabled.
+
+```yaml
+- uses: allenporter/flux-local/test@2.0.0
+  with:
+    path: clusters/prod
+    enable-helm: true
+    enable-kyverno: false
+```
+
+### diff action
+
+The `diff` action will show you the final diffs of `Kustomization` or `HelmRelease`
+objects that are fully built. While typically you can just read diffs to understand
+how kustomzations may be affected, this action also supports overlays and multiple
+clusters showing you the final output.
+
+This is an example that diffs a `HelmRelease`:
+
+```yaml
+- uses: allenporter/flux-local/action/diff@2.0.0
+  id: diff
+  with:
+    live-branch: main
+    path: clusters/prod
+    resource: helmrelease
+- name: PR Comments
+  uses: mshick/add-pr-comment@v2
+  if: ${{ steps.diff.outputs.diff != '' }}
+  with:
+    repo-token: ${{ secrets.GITHUB_TOKEN }}
+    message-failure: Unable to post diff
+    message: |
+      `````diff
+      ${{ steps.diff.outputs.diff }}
+      `````
+```
+
+This is an example of a workflow that will diff `Kustomization` and `HelmRelease` objects
+in a repo with multiple clusters (`dev` and `prod`):
+
+```yaml
+jobs:
+  diffs:
+    name: Compute diffs
+    runs-on: ubuntu-latest
+    strategy:
+      matrix:
+        cluster_path:
+          - clusters/dev
+          - clusters/prod
+        resource:
+          - helmrelease
+          - kustomization
+    steps:
+      - uses: allenporter/flux-local/action/diff@2.0.0
+        id: diff
+        with:
+          live-branch: main
+          path: ${{ matrix.cluster_path }}
+          resource: ${{ matrix.resource }}
+      - name: PR Comments
+        uses: mshick/add-pr-comment@v2
+        if: ${{ steps.diff.outputs.diff != '' }}
+        with:
+          repo-token: ${{ secrets.GITHUB_TOKEN }}
+          message-id: ${{ matrix.cluster_path }}/${{ matrix.resource }}
+          message-failure: Unable to post kustomization diff
+          message: |
+            `````diff
+            ${{ steps.diff.outputs.diff }}
+            `````
+```
+
 ## Library
 
 The `flux_local` [library documentation](https://allenporter.github.io/flux-local/) for details
 on the python APIs provided.
```

### Comparing `flux-local-1.2.0/README.md` & `flux-local-1.3.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: flux-local
+Version: 1.3.0
+Summary: flux-local is a python library and set of tools for managing a flux gitops repository, with validation steps to help improve quality of commits, PRs, and general local testing.
+Home-page: https://github.com/allenporter/flux-local
+Author: Allen Porter
+Author-email: allen.porter@gmail.com
+License: Apache-2.0
+Classifier: License :: OSI Approved :: Apache Software License
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 flux-local is a set of tools and libraries for managing a local flux gitops repository focused on validation steps to help improve quality of commits, PRs, and general local testing.
 
 This library uses command line tools like kustomize and helm to replicate the behavior of
 flux to gather objects in the cluster. It only looks at the local git repo, and not a live
 cluster. However, this is fine since the local repository has enough information and the
 definition is simple. Secrets are ignored as the content is not needed to validate the
 cluster is creating valid objects.
@@ -230,11 +242,98 @@
 
 clusters/dev .....................................                                                      [ 45%]
 clusters/prod ............................................                                              [100%]
 
 ======================================== 81 passed in 75.40s (0:01:15) ========================================
 ```
 
+## GitHub Action
+
+You may use `flux-local` as a github action to verify the health of the cluster on changes
+or PRs.
+
+### test action
+
+The `test` action will validate the cluster will build, and can optionally
+validate flux `HelmRelease` builds and also verify that all objects pass
+kyverno policies (e.g. for determining there are no deprecated api resources
+or that ingress objects are valid).
+
+This example will run `flux-local test` against the cluster in `clusters/prod` with
+helm release expansion enabled.
+
+```yaml
+- uses: allenporter/flux-local/test@2.0.0
+  with:
+    path: clusters/prod
+    enable-helm: true
+    enable-kyverno: false
+```
+
+### diff action
+
+The `diff` action will show you the final diffs of `Kustomization` or `HelmRelease`
+objects that are fully built. While typically you can just read diffs to understand
+how kustomzations may be affected, this action also supports overlays and multiple
+clusters showing you the final output.
+
+This is an example that diffs a `HelmRelease`:
+
+```yaml
+- uses: allenporter/flux-local/action/diff@2.0.0
+  id: diff
+  with:
+    live-branch: main
+    path: clusters/prod
+    resource: helmrelease
+- name: PR Comments
+  uses: mshick/add-pr-comment@v2
+  if: ${{ steps.diff.outputs.diff != '' }}
+  with:
+    repo-token: ${{ secrets.GITHUB_TOKEN }}
+    message-failure: Unable to post diff
+    message: |
+      `````diff
+      ${{ steps.diff.outputs.diff }}
+      `````
+```
+
+This is an example of a workflow that will diff `Kustomization` and `HelmRelease` objects
+in a repo with multiple clusters (`dev` and `prod`):
+
+```yaml
+jobs:
+  diffs:
+    name: Compute diffs
+    runs-on: ubuntu-latest
+    strategy:
+      matrix:
+        cluster_path:
+          - clusters/dev
+          - clusters/prod
+        resource:
+          - helmrelease
+          - kustomization
+    steps:
+      - uses: allenporter/flux-local/action/diff@2.0.0
+        id: diff
+        with:
+          live-branch: main
+          path: ${{ matrix.cluster_path }}
+          resource: ${{ matrix.resource }}
+      - name: PR Comments
+        uses: mshick/add-pr-comment@v2
+        if: ${{ steps.diff.outputs.diff != '' }}
+        with:
+          repo-token: ${{ secrets.GITHUB_TOKEN }}
+          message-id: ${{ matrix.cluster_path }}/${{ matrix.resource }}
+          message-failure: Unable to post kustomization diff
+          message: |
+            `````diff
+            ${{ steps.diff.outputs.diff }}
+            `````
+```
+
 ## Library
 
 The `flux_local` [library documentation](https://allenporter.github.io/flux-local/) for details
 on the python APIs provided.
```

### Comparing `flux-local-1.2.0/flux_local/command.py` & `flux-local-1.3.0/flux_local/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 from .exceptions import CommandException
 
 _LOGGER = logging.getLogger(__name__)
 
 _CONCURRENCY = 20
 _SEM = asyncio.Semaphore(_CONCURRENCY)
+_TIMEOUT = 20.0
 
 
 # No public API
 __all__: list[str] = []
 
 
 class Task(ABC):
@@ -88,15 +89,15 @@
 
 
 async def _run_piped_with_sem(cmds: Sequence[Task]) -> str:
     """Run a set of commands, piped together, returning stdout of last."""
     stdin = None
     out = None
     for cmd in cmds:
-        out = await cmd.run(stdin)
+        out = await asyncio.wait_for(cmd.run(stdin), _TIMEOUT)
         stdin = out
     return out.decode("utf-8") if out else ""
 
 
 async def run_piped(cmds: Sequence[Task]) -> str:
     """Run a set of commands, piped together, returning stdout of last."""
     async with _SEM:
```

### Comparing `flux-local-1.2.0/flux_local/exceptions.py` & `flux-local-1.3.0/flux_local/exceptions.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.2.0/flux_local/git_repo.py` & `flux-local-1.3.0/flux_local/git_repo.py`

 * *Files 10% similar despite different names*

```diff
@@ -70,17 +70,69 @@
 
 CLUSTER_KUSTOMIZE_KIND = "Kustomization"
 KUSTOMIZE_KIND = "Kustomization"
 HELM_REPO_KIND = "HelmRepository"
 HELM_RELEASE_KIND = "HelmRelease"
 CLUSTER_POLICY_KIND = "ClusterPolicy"
 GIT_REPO_KIND = "GitRepository"
+OCI_REPO_KIND = "OCIRepository"
 DEFAULT_NAMESPACE = "flux-system"
 
 
+@dataclass
+class Source:
+    """A source is a named mapping from a k8s object name to a path in the git repo.
+
+    This is needed to map the location within a reop if it's not the root. For example,
+    you may have a `GitRepository` that is relative to `/` and all if of the
+    `Kustomization`s inside may reference paths within it e.g. `/k8s/namespaces/`. But
+    you may also have an `OCIRepository` that was built relative to `/k8s/` where the
+    `Kustomization`s inside may reference the path relative to that like `/namespaces/`.
+    """
+
+    name: str
+    """The name of the repository source."""
+
+    root: Path
+    """The path name within the repo root."""
+
+    namespace: str
+    """The namespace of the repository source."""
+
+    @property
+    def source_name(self) -> str:
+        """Return the full name of the source."""
+        return f"{self.namespace}/{self.name}"
+
+    @classmethod
+    def from_str(self, value: str) -> "Source":
+        """Parse a Source from key=value string."""
+        if "=" not in value:
+            raise ValueError("Expected source name=root")
+        namespace = "flux-system"
+        name, root = value.split("=")
+        if "/" in name:
+            namespace, name = name.split("/")
+        return Source(name=name, root=Path(root), namespace=namespace)
+
+
+def has_source_name(name: str) -> Callable[[Source], bool]:
+    """Return a source root if the source exists."""
+
+    def predicate(source: Source) -> bool:
+        return source.name == name
+
+    return predicate
+
+
+def source_root(source: Source) -> Path:
+    """Return the sources root path."""
+    return source.root
+
+
 @cache
 def git_repo(path: Path | None = None) -> git.repo.Repo:
     """Return the local git repo path."""
     try:
         if path is None:
             return git.repo.Repo(os.getcwd(), search_parent_directories=True)
         return git.repo.Repo(str(path), search_parent_directories=True)
@@ -115,14 +167,17 @@
 @dataclass
 class PathSelector:
     """A pathlib.Path inside of a git repo."""
 
     path: Path | None = None
     """The path within a repo."""
 
+    sources: list[Source] | None = None
+    """A list of repository sources for building relative paths."""
+
     @property
     def repo(self) -> git.repo.Repo:
         """Return the local git repo."""
         return git_repo(self.path)
 
     @property
     def root(self) -> Path:
@@ -220,14 +275,21 @@
 
 def ks_metadata_selector() -> MetadataSelector:
     """Create a new MetadataSelector for Kustomizations."""
     return MetadataSelector(namespace=DEFAULT_NAMESPACE)
 
 
 @dataclass
+class Options:
+    """Options for the resource selector for building manifets."""
+
+    kustomize_flags: list[str] = field(default_factory=list)
+
+
+@dataclass
 class ResourceSelector:
     """A filter for objects to select from the cluster.
 
     This is invoked when iterating over objects in the cluster to decide which
     resources should be inflated and returned, to avoid iterating over
     unnecessary resources.
     """
@@ -257,15 +319,15 @@
     """Find all flux Kustomizations in the specified path.
 
     This may be called repeatedly with different paths to repeatedly collect
     Kustomizations from the repo. Assumes that any flux Kustomization
     for a GitRepository is pointed at this cluster, following normal conventions.
     """
     cmd = kustomize.grep(f"kind={CLUSTER_KUSTOMIZE_KIND}", root / relative_path).grep(
-        f"spec.sourceRef.kind={GIT_REPO_KIND}"
+        f"spec.sourceRef.kind={GIT_REPO_KIND}|{OCI_REPO_KIND}"
     )
     docs = await cmd.objects()
     return [
         Kustomization.parse_doc(doc)
         for doc in filter(CLUSTER_KUSTOMIZE_DOMAIN_FILTER, docs)
     ]
 
@@ -318,46 +380,89 @@
                 ((root / path) / kustomization.source_path).relative_to(root)
             )
 
         visited |= set({path})
 
         _LOGGER.debug("Found %s Kustomizations", len(docs))
         for doc in docs:
-            found_path = Path(doc.path)
+            found_path: Path | None = None
+            _LOGGER.debug(
+                "Kustomization '%s' has sourceRef.kind '%s' of '%s'",
+                doc.name,
+                doc.source_kind,
+                doc.source_name,
+            )
+            if not doc.source_kind or doc.source_kind == GIT_REPO_KIND:
+                found_path = Path(doc.path)
+            elif doc.source_kind == OCI_REPO_KIND:
+                for source in path_selector.sources or ():
+                    if source.name == doc.source_name:
+                        found_path = source.root / doc.path
+                        break
+            elif not doc.source_kind or doc.source_kind == GIT_REPO_KIND:
+                found_path = Path(doc.path)
+
+            if not found_path:
+                _LOGGER.debug("Skipping kustomization %s; not known source", doc.name)
+                continue
+
             if not find_path_parent(found_path, visited) and found_path not in visited:
                 path_queue.put(found_path)
             else:
                 _LOGGER.debug("Already visited %s", found_path)
         kustomizations.extend(docs)
     return kustomizations
 
 
-def make_clusters(kustomizations: list[Kustomization]) -> list[Cluster]:
+def make_clusters(
+    kustomizations: list[Kustomization], sources: list[Source] | None = None
+) -> list[Cluster]:
     """Convert the flat list of Kustomizations into a Cluster.
 
     This will reverse engineer which Kustomizations are root nodes for the cluster
     based on the parent paths. Root Kustomizations are made the cluster and everything
     else is made a child.
     """
+    if not sources:
+        sources = []
 
     # Build a directed graph from a kustomization path to the path
     # of the kustomization that created it.
     graph = networkx.DiGraph()
     parent_paths = set([Path(ks.path) for ks in kustomizations])
     for ks in kustomizations:
         if not ks.source_path:
             raise InputException(
                 "Kustomization did not have source path; Old kustomize?"
             )
+
+        # OCIRepositories may be build pointed at a subset of the cluster which can
+        # only be determined based on input command line flags
+        if ks.source_kind == OCI_REPO_KIND:
+            if root := next(
+                map(
+                    source_root, filter(has_source_name(ks.source_name or ""), sources)
+                ),
+                None,
+            ):
+                ks.path = str(root / ks.path)
+                _LOGGER.debug(
+                    "Updated Source for OCIRepository %s: %s", ks.name, ks.path
+                )
+            else:
+                _LOGGER.debug("Excluding OCIRepository without source %s", ks.name)
+                continue
+
         path = Path(ks.path)
-        source = Path(ks.source_path)
         graph.add_node(path, ks=ks)
+
         # Find the parent Kustomization that produced this based on the
         # matching the kustomize source parent paths with a Kustomization
         # target path.
+        source = Path(ks.source_path)
         if (
             parent_path := find_path_parent(source, parent_paths)
         ) and parent_path != path:
             _LOGGER.debug("Found parent %s => %s", path, parent_path)
             graph.add_edge(parent_path, path)
         else:
             _LOGGER.debug("No parent for %s (%s)", path, source)
@@ -393,15 +498,20 @@
     path_selector: PathSelector,
     cluster_selector: MetadataSelector,
     kustomization_selector: MetadataSelector,
 ) -> list[Cluster]:
     """Load Cluster objects from the specified path."""
 
     kustomizations = await kustomization_traversal(path_selector)
-    clusters = list(filter(cluster_selector.predicate, make_clusters(kustomizations)))
+    clusters = list(
+        filter(
+            cluster_selector.predicate,
+            make_clusters(kustomizations, path_selector.sources or []),
+        )
+    )
     for cluster in clusters:
         cluster.kustomizations = list(
             filter(kustomization_selector.predicate, cluster.kustomizations)
         )
     return clusters
 
 
@@ -416,25 +526,25 @@
     kustomization: Kustomization,
     cluster_path: Path,
     root: Path,
     kustomization_selector: MetadataSelector,
     helm_release_selector: MetadataSelector,
     helm_repo_selector: MetadataSelector,
     cluster_policy_selector: MetadataSelector,
+    kustomize_flags: list[str],
 ) -> tuple[Iterable[HelmRepository], Iterable[HelmRelease], Iterable[ClusterPolicy]]:
     """Build helm objects for the Kustomization."""
     if (
         not kustomization_selector.enabled
         and not helm_release_selector.enabled
         and not helm_repo_selector.enabled
         and not cluster_policy_selector.enabled
     ):
         return ([], [], [])
-
-    cmd = kustomize.build(root / kustomization.path)
+    cmd = kustomize.build(root / kustomization.path, kustomize_flags)
     skips = []
     if kustomization_selector.skip_crds:
         skips.append(CRD_KIND)
     if kustomization_selector.skip_secrets:
         skips.append(SECRET_KIND)
     cmd = cmd.skip_resources(skips)
     try:
@@ -492,14 +602,15 @@
         ),
     )
 
 
 async def build_manifest(
     path: Path | None = None,
     selector: ResourceSelector = ResourceSelector(),
+    options: Options = Options(),
 ) -> Manifest:
     """Build a Manifest object from the local cluster.
 
     This will locate all Kustomizations that represent clusters, then find all
     the Kustomizations within that cluster, as well as all relevant Helm
     resources.
 
@@ -526,24 +637,29 @@
                 Kustomization(name="kustomization", path=str(selector.path.path))
             ]
             clusters.append(cluster)
 
     async def update_kustomization(cluster: Cluster) -> None:
         build_tasks = []
         for kustomization in cluster.kustomizations:
-            _LOGGER.debug("Processing kustomization: %s", kustomization.path)
+            _LOGGER.debug(
+                "Processing kustomization '%s': %s",
+                kustomization.name,
+                kustomization.path,
+            )
             build_tasks.append(
                 build_kustomization(
                     kustomization,
                     Path(cluster.path),
                     selector.path.root,
                     selector.kustomization,
                     selector.helm_release,
                     selector.helm_repo,
                     selector.cluster_policy,
+                    options.kustomize_flags,
                 )
             )
         results = list(await asyncio.gather(*build_tasks))
         for kustomization, (helm_repos, helm_releases, cluster_policies) in zip(
             cluster.kustomizations,
             results,
         ):
```

### Comparing `flux-local-1.2.0/flux_local/helm.py` & `flux-local-1.3.0/flux_local/helm.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.2.0/flux_local/kustomize.py` & `flux-local-1.3.0/flux_local/kustomize.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     print(f"Found ConfigMap: {object['metadata']['name']}")
 ```
 
 You can apply kyverno policies to the objects with the `validate` method.
 """
 
 import aiofiles
-from aiofiles.os import listdir  # type: ignore[attr-defined]
+from aiofiles.os import listdir
 from aiofiles.ospath import isdir, exists
 import asyncio
 import logging
 from pathlib import Path
 import tempfile
 from typing import Any, AsyncGenerator
 
@@ -183,31 +183,33 @@
         """Run the task."""
         return self._out
 
 
 class Build(Task):
     """A task that issues a build command, handling implicit Kustomizations."""
 
-    def __init__(self, path: Path) -> None:
+    def __init__(self, path: Path, kustomize_flags: list[str] | None = None) -> None:
         """Initialize Build."""
         self._path = path
+        self._kustomize_flags = kustomize_flags or []
 
     async def run(self, stdin: bytes | None = None) -> bytes:
         """Run the task."""
         if stdin is not None:
             raise InputException("Invalid stdin cannot be passed to build command")
 
         if not await isdir(self._path):
             raise InputException(f"Specified path is not a directory: {self._path}")
         if not await can_kustomize_dir(self._path):
             # Attempt to effectively generate a kustomization.yaml on the fly
             # mirroring the behavior of flux
             return await fluxtomize(self._path)
 
         args = [KUSTOMIZE_BIN, "build"]
+        args.extend(self._kustomize_flags)
         cwd: Path | None = None
         if self._path.is_absolute():
             cwd = self._path
         else:
             args.append(str(self._path))
         task = Command(args, cwd=cwd, exc=KustomizeException)
         return await task.run()
@@ -253,17 +255,17 @@
     docs = []
     for result in results:
         docs.extend(result)
     out = yaml.dump_all(docs, sort_keys=False, explicit_start=True)
     return str(out).encode("utf-8")
 
 
-def build(path: Path) -> Kustomize:
+def build(path: Path, kustomize_flags: list[str] | None = None) -> Kustomize:
     """Build cluster artifacts from the specified path."""
-    return Kustomize(cmds=[Build(path)])
+    return Kustomize(cmds=[Build(path, kustomize_flags)])
 
 
 def grep(expr: str, path: Path, invert: bool = False) -> Kustomize:
     """Filter resources in the specified path based on an expression."""
     args = [KUSTOMIZE_BIN, "cfg", "grep", expr]
     if invert:
         args.append("--invert-match")
```

### Comparing `flux-local-1.2.0/flux_local/manifest.py` & `flux-local-1.3.0/flux_local/manifest.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         """Parse a serialized manifest."""
         doc = next(yaml.load_all(content, Loader=yaml.Loader), None)
         return cls.parse_obj(doc)
 
     def yaml(self, exclude: dict[str, Any] | None = None) -> str:
         """Return a YAML string representation of compact_dict."""
         data = self.compact_dict(exclude)
-        return cast(str, yaml.dump(data, sort_keys=False, explicit_start=True))
+        return yaml.dump(data, sort_keys=False, explicit_start=True)
 
 
 class HelmChart(BaseManifest):
     """A representation of an instantiation of a chart for a HelmRelease."""
 
     name: str
     """The name of the chart within the HelmRepository."""
@@ -87,15 +87,15 @@
     repo_name: str
     """The name of the HelmRepository."""
 
     repo_namespace: str
     """The namespace of the HelmRepository."""
 
     @classmethod
-    def parse_doc(cls, doc: dict[str, Any]) -> "HelmChart":
+    def parse_doc(cls, doc: dict[str, Any], default_namespace: str) -> "HelmChart":
         """Parse a HelmChart from a HelmRelease resource object."""
         _check_version(doc, HELM_RELEASE_DOMAIN)
         if not (spec := doc.get("spec")):
             raise InputException(f"Invalid {cls} missing spec: {doc}")
         if not (chart := spec.get("chart")):
             raise InputException(f"Invalid {cls} missing spec.chart: {doc}")
         if not (chart_spec := chart.get("spec")):
@@ -103,21 +103,21 @@
         if not (chart := chart_spec.get("chart")):
             raise InputException(f"Invalid {cls} missing spec.chart.spec.chart: {doc}")
         version = chart_spec.get("version")
         if not (source_ref := chart_spec.get("sourceRef")):
             raise InputException(
                 f"Invalid {cls} missing spec.chart.spec.sourceRef: {doc}"
             )
-        if "namespace" not in source_ref or "name" not in source_ref:
+        if "name" not in source_ref:
             raise InputException(f"Invalid {cls} missing sourceRef fields: {doc}")
         return cls(
             name=chart,
             version=version,
             repo_name=source_ref["name"],
-            repo_namespace=source_ref["namespace"],
+            repo_namespace=source_ref.get("namespace", default_namespace),
         )
 
     @property
     def chart_name(self) -> str:
         """Identifier for the HelmChart."""
         return f"{self.repo_namespace}-{self.repo_name}/{self.name}"
 
@@ -145,15 +145,15 @@
         _check_version(doc, HELM_RELEASE_DOMAIN)
         if not (metadata := doc.get("metadata")):
             raise InputException(f"Invalid {cls} missing metadata: {doc}")
         if not (name := metadata.get("name")):
             raise InputException(f"Invalid {cls} missing metadata.name: {doc}")
         if not (namespace := metadata.get("namespace")):
             raise InputException(f"Invalid {cls} missing metadata.namespace: {doc}")
-        chart = HelmChart.parse_doc(doc)
+        chart = HelmChart.parse_doc(doc, namespace)
         return cls(
             name=name,
             namespace=namespace,
             chart=chart,
             values=doc["spec"].get("values"),
         )
 
@@ -270,14 +270,20 @@
 
     cluster_policies: list[ClusterPolicy] = Field(default_factory=list)
     """The set of ClusterPolicies represented in this kustomization."""
 
     source_path: str | None = None
     """Optional source path for this Kustomization, relative to the build path."""
 
+    source_kind: str | None = None
+    """The sourceRef kind that provides this Kustomization e.g. GitRepository etc."""
+
+    source_name: str | None = None
+    """The name of the sourceRef that provides this Kustomization."""
+
     @classmethod
     def parse_doc(cls, doc: dict[str, Any]) -> "Kustomization":
         """Parse a partial Kustomization from a kubernetes resource."""
         _check_version(doc, CLUSTER_KUSTOMIZE_DOMAIN)
         if not (metadata := doc.get("metadata")):
             raise InputException(f"Invalid {cls} missing metadata: {doc}")
         if not (name := metadata.get("name")):
@@ -285,16 +291,22 @@
         if not (namespace := metadata.get("namespace")):
             raise InputException(f"Invalid {cls} missing metadata.namespace: {doc}")
         if not (spec := doc.get("spec")):
             raise InputException(f"Invalid {cls} missing spec: {doc}")
         if not (path := spec.get("path")):
             raise InputException(f"Invalid {cls} missing spec.path: {doc}")
         source_path = metadata.get("annotations", {}).get("config.kubernetes.io/path")
+        source_ref = spec.get("sourceRef", {})
         return Kustomization(
-            name=name, namespace=namespace, path=path, source_path=source_path
+            name=name,
+            namespace=namespace,
+            path=path,
+            source_path=source_path,
+            source_kind=source_ref.get("kind"),
+            source_name=source_ref.get("name"),
         )
 
     @property
     def id_name(self) -> str:
         """Identifier for the Kustomization in tests"""
         return f"{self.path}"
 
@@ -302,14 +314,16 @@
         "helm_releases": {
             "__all__": HelmRelease._COMPACT_EXCLUDE_FIELDS,
         },
         "cluster_policies": {
             "__all__": ClusterPolicy._COMPACT_EXCLUDE_FIELDS,
         },
         "source_path": True,
+        "source_name": True,
+        "source_kind": True,
     }
 
 
 class Cluster(BaseManifest):
     """A set of nodes that run containerized applications.
 
     Many flux git repos will only have a single flux cluster, though
```

### Comparing `flux-local-1.2.0/flux_local/tool/build.py` & `flux-local-1.3.0/flux_local/tool/build.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import logging
 import pathlib
 import tempfile
 
 
 from flux_local import git_repo
 
+from . import selector
 from .visitor import ContentOutput, HelmVisitor
 
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class BuildAction:
@@ -34,15 +35,17 @@
         query.helm_release.namespace = None
 
         content = ContentOutput()
         query.kustomization.visitor = content.visitor()
         helm_visitor = HelmVisitor()
         query.helm_repo.visitor = helm_visitor.repo_visitor()
         query.helm_release.visitor = helm_visitor.release_visitor()
-        await git_repo.build_manifest(selector=query)
+        await git_repo.build_manifest(
+            selector=query, options=selector.options(**kwargs)
+        )
 
         # We use a separate output object so that the contents of the HelmRelease
         # always come after the HelmRelease itself. This means all the helm releases
         # are built at the end. It might be more natural to sort by Kustomization
         # or have the contents of the release immediately following it if we could
         # make the ResourceKeys sort that way, but the helm visitor loses the
         # Kustomziation information at the moment.
```

### Comparing `flux-local-1.2.0/flux_local/tool/diff.py` & `flux-local-1.3.0/flux_local/tool/diff.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Flux-local diff action."""
 
 import asyncio
+import functools
 import os
 from argparse import ArgumentParser
 from argparse import _SubParsersAction as SubParsersAction
 from contextlib import contextmanager
 from dataclasses import asdict
 import difflib
 import logging
@@ -18,19 +19,22 @@
 from flux_local import git_repo, command
 
 from . import selector
 from .visitor import HelmVisitor, ObjectOutput, ResourceKey
 
 _LOGGER = logging.getLogger(__name__)
 
+# Type for command line flags of comma separated list
+_CSV = functools.partial(str.split, sep=",")
+
+_TRUNCATE = "[Diff truncated by flux-local]"
+
 
 def perform_object_diff(
-    a: ObjectOutput,
-    b: ObjectOutput,
-    n: int,
+    a: ObjectOutput, b: ObjectOutput, n: int, limit_bytes: int
 ) -> Generator[str, None, None]:
     """Generate diffs between the two output objects."""
     for kustomization_key in set(a.content.keys()) | set(b.content.keys()):
         _LOGGER.debug(
             "Diffing results for Kustomization %s (n=%d)", kustomization_key, n
         )
         a_resources = a.content.get(kustomization_key, {})
@@ -39,22 +43,28 @@
             diff_text = difflib.unified_diff(
                 a=a_resources.get(resource_key, []),
                 b=b_resources.get(resource_key, []),
                 fromfile=f"{kustomization_key.label} {resource_key.compact_label}",
                 tofile=f"{kustomization_key.label} {resource_key.compact_label}",
                 n=n,
             )
+            size = 0
             for line in diff_text:
+                size += len(line)
+                if limit_bytes and size > limit_bytes:
+                    yield _TRUNCATE
+                    break
                 yield line
 
 
 async def perform_external_diff(
     cmd: list[str],
     a: ObjectOutput,
     b: ObjectOutput,
+    limit_bytes: int,
 ) -> AsyncGenerator[str, None]:
     """Generate diffs between the two output objects."""
     with tempfile.TemporaryDirectory() as tmpdir:
         for kustomization_key in set(a.content.keys()) | set(b.content.keys()):
             _LOGGER.debug(
                 "Diffing results for Kustomization %s",
                 kustomization_key,
@@ -82,26 +92,30 @@
                 )
             )
 
             out = await command.Command(
                 cmd + [str(a_file), str(b_file)], retcodes=[0, 1]
             ).run()
             if out:
-                yield out.decode("utf-8")
+                result = out.decode("utf-8")
+                if limit_bytes and len(result) > limit_bytes:
+                    result = result[:limit_bytes] + "\n" + _TRUNCATE
+                yield result
 
 
 def omit_none(obj: Any) -> dict[str, Any]:
     """Creates a dictionary with None values missing."""
     return {k: v for k, v in obj if v is not None}
 
 
 def perform_yaml_diff(
     a: ObjectOutput,
     b: ObjectOutput,
     n: int,
+    limit_bytes: int,
 ) -> Generator[str, None, None]:
     """Generate diffs between the two output objects."""
 
     diffs = []
     for kustomization_key in set(a.content.keys()) | set(b.content.keys()):
         _LOGGER.debug("Diffing results for %s (n=%d)", kustomization_key, n)
         a_resources = a.content.get(kustomization_key, {})
@@ -114,14 +128,16 @@
                 fromfile=f"{kustomization_key.label} {resource_key.compact_label}",
                 tofile=f"{kustomization_key.label} {resource_key.compact_label}",
                 n=n,
             )
             diff_content = "\n".join(diff_text)
             if not diff_content:
                 continue
+            if limit_bytes and len(diff_content) > limit_bytes:
+                diff_content = diff_content[:limit_bytes] + "\n" + _TRUNCATE
             obj = {
                 **asdict(resource_key, dict_factory=omit_none),
                 "diff": diff_content,
             }
             resource_diffs.append(obj)
         if resource_diffs:
             diffs.append(
@@ -171,14 +187,25 @@
     args.add_argument(
         "--path-orig",
         help="Path to compare against, or creates a work tree if not specified",
         type=pathlib.Path,
         default=None,
         nargs="?",
     )
+    args.add_argument(
+        "--strip-attrs",
+        help="Labels or annotations to strip from the diff",
+        type=_CSV,
+    )
+    args.add_argument(
+        "--limit-bytes",
+        help="Maximum bytes for each diff output (0=unlimited)",
+        type=int,
+        default=0,
+    )
 
 
 @contextmanager
 def create_diff_path(
     selector: git_repo.PathSelector,
     **kwargs: Any,
 ) -> Generator[git_repo.PathSelector, None, None]:
@@ -220,46 +247,52 @@
         args.set_defaults(cls=cls)
         return args
 
     async def run(  # type: ignore[no-untyped-def]
         self,
         output: str,
         unified: int,
+        strip_attrs: list[str] | None,
+        limit_bytes: int,
         **kwargs,  # pylint: disable=unused-argument
     ) -> None:
         """Async Action implementation."""
         query = selector.build_ks_selector(**kwargs)
         query.helm_release.enabled = False
 
-        content = ObjectOutput()
+        content = ObjectOutput(strip_attrs)
         query.kustomization.visitor = content.visitor()
-        await git_repo.build_manifest(selector=query)
+        await git_repo.build_manifest(
+            selector=query, options=selector.options(**kwargs)
+        )
 
-        orig_content = ObjectOutput()
+        orig_content = ObjectOutput(strip_attrs)
         with create_diff_path(query.path, **kwargs) as path_selector:
             query.path = path_selector
             query.kustomization.visitor = orig_content.visitor()
-            await git_repo.build_manifest(selector=query)
+            await git_repo.build_manifest(
+                selector=query, options=selector.options(**kwargs)
+            )
 
         if not orig_content.content and not content.content:
             print(selector.not_found("Kustomization", query.kustomization))
             return
 
         _LOGGER.debug("Diffing content")
         if output == "yaml":
-            result = perform_yaml_diff(orig_content, content, unified)
+            result = perform_yaml_diff(orig_content, content, unified, limit_bytes)
             for line in result:
                 print(line)
         elif external_diff := os.environ.get("DIFF"):
             async for line in perform_external_diff(
-                shlex.split(external_diff), orig_content, content
+                shlex.split(external_diff), orig_content, content, limit_bytes
             ):
                 print(line)
         else:
-            result = perform_object_diff(orig_content, content, unified)
+            result = perform_object_diff(orig_content, content, unified, limit_bytes)
             for line in result:
                 print(line)
 
 
 class DiffHelmReleaseAction:
     """Flux-local diff for HelmRelease."""
 
@@ -285,33 +318,39 @@
         args.set_defaults(cls=cls)
         return args
 
     async def run(  # type: ignore[no-untyped-def]
         self,
         output: str,
         unified: int,
+        strip_attrs: list[str] | None,
+        limit_bytes: int,
         **kwargs,  # pylint: disable=unused-argument
     ) -> None:
         """Async Action implementation."""
         query = selector.build_hr_selector(**kwargs)
-        content = ObjectOutput()
+        content = ObjectOutput(strip_attrs)
         helm_visitor = HelmVisitor()
         query.kustomization.visitor = content.visitor()
         query.helm_repo.visitor = helm_visitor.repo_visitor()
         query.helm_release.visitor = helm_visitor.release_visitor()
-        await git_repo.build_manifest(selector=query)
+        await git_repo.build_manifest(
+            selector=query, options=selector.options(**kwargs)
+        )
 
-        orig_content = ObjectOutput()
+        orig_content = ObjectOutput(strip_attrs)
         orig_helm_visitor = HelmVisitor()
         with create_diff_path(query.path, **kwargs) as path_selector:
             query.path = path_selector
             query.kustomization.visitor = orig_content.visitor()
             query.helm_repo.visitor = orig_helm_visitor.repo_visitor()
             query.helm_release.visitor = orig_helm_visitor.release_visitor()
-            await git_repo.build_manifest(selector=query)
+            await git_repo.build_manifest(
+                selector=query, options=selector.options(**kwargs)
+            )
 
         if not helm_visitor.releases and not orig_helm_visitor.releases:
             print(selector.not_found("HelmRelease", query.helm_release))
             return
 
         # Find HelmRelease objects with diffs and prune all other HelmReleases from
         # the helm visitors. We assume that the only way for a HelmRelease output
@@ -341,16 +380,16 @@
                 releases = [
                     release
                     for release in orig_helm_visitor.releases[cluster_path]
                     if f"{release.namespace}/{release.name}" in diff_names
                 ]
                 orig_helm_visitor.releases[cluster_path] = releases
 
-        helm_content = ObjectOutput()
-        orig_helm_content = ObjectOutput()
+        helm_content = ObjectOutput(strip_attrs)
+        orig_helm_content = ObjectOutput(strip_attrs)
         with tempfile.TemporaryDirectory() as helm_cache_dir:
             await asyncio.gather(
                 helm_visitor.inflate(
                     pathlib.Path(helm_cache_dir),
                     helm_content.visitor(),
                     query.helm_release.skip_crds,
                     skip_secrets=query.helm_release.skip_secrets,
@@ -360,23 +399,27 @@
                     orig_helm_content.visitor(),
                     query.helm_release.skip_crds,
                     skip_secrets=query.helm_release.skip_secrets,
                 ),
             )
 
         if output == "yaml":
-            for line in perform_yaml_diff(orig_helm_content, helm_content, unified):
+            for line in perform_yaml_diff(
+                orig_helm_content, helm_content, unified, limit_bytes
+            ):
                 print(line)
         elif external_diff := os.environ.get("DIFF"):
             async for line in perform_external_diff(
-                shlex.split(external_diff), orig_helm_content, helm_content
+                shlex.split(external_diff), orig_helm_content, helm_content, limit_bytes
             ):
                 print(line)
         else:
-            for line in perform_object_diff(orig_helm_content, helm_content, unified):
+            for line in perform_object_diff(
+                orig_helm_content, helm_content, unified, limit_bytes
+            ):
                 print(line)
 
 
 class DiffAction:
     """Flux-local diff action."""
 
     @classmethod
```

### Comparing `flux-local-1.2.0/flux_local/tool/flux_local.py` & `flux-local-1.3.0/flux_local/tool/flux_local.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,14 +66,20 @@
     build_args.add_argument(
         "--skip-secrets",
         type=bool,
         default=True,
         action=argparse.BooleanOptionalAction,
         help="Omit secrets from the output to reduce random output.",
     )
+    build_args.add_argument(
+        "--kustomize-build-flags",
+        type=str,
+        default="",
+        help="If present, additional flags to pass to `kustomize build`",
+    )
     build_args.set_defaults(cls=build.BuildAction)
 
     get.GetAction.register(subparsers)
     diff.DiffAction.register(subparsers)
     test.TestAction.register(subparsers)
 
     args = parser.parse_args()
```

### Comparing `flux-local-1.2.0/flux_local/tool/format.py` & `flux-local-1.3.0/flux_local/tool/format.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.2.0/flux_local/tool/get.py` & `flux-local-1.3.0/flux_local/tool/get.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,17 @@
         **kwargs,  # pylint: disable=unused-argument
     ) -> None:
         """Async Action implementation."""
         query = selector.build_ks_selector(**kwargs)
         if output != "wide":
             query.helm_release.enabled = False
             query.helm_repo.enabled = False
-        manifest = await git_repo.build_manifest(selector=query)
+        manifest = await git_repo.build_manifest(
+            selector=query, options=selector.options(**kwargs)
+        )
 
         results: list[dict[str, str]] = []
         cols = ["name", "path"]
         if output == "wide":
             cols.extend(["helmrepos", "releases"])
         if len(manifest.clusters) > 1:
             cols.insert(0, "cluster")
@@ -101,15 +103,17 @@
 
     async def run(  # type: ignore[no-untyped-def]
         self,
         **kwargs,  # pylint: disable=unused-argument
     ) -> None:
         """Async Action implementation."""
         query = selector.build_hr_selector(**kwargs)
-        manifest = await git_repo.build_manifest(selector=query)
+        manifest = await git_repo.build_manifest(
+            selector=query, options=selector.options(**kwargs)
+        )
 
         cols = ["name", "revision", "chart", "source"]
         if query.helm_release.namespace is None:
             cols.insert(0, "namespace")
         results: list[dict[str, Any]] = []
         for cluster in manifest.clusters:
             for helmrelease in cluster.helm_releases:
@@ -158,15 +162,17 @@
         self,
         output: str,
         **kwargs,  # pylint: disable=unused-argument
     ) -> None:
         """Async Action implementation."""
         query = selector.build_cluster_selector(**kwargs)
         query.helm_release.enabled = output == "yaml"
-        manifest = await git_repo.build_manifest(selector=query)
+        manifest = await git_repo.build_manifest(
+            selector=query, options=selector.options(**kwargs)
+        )
         if output == "yaml":
             YamlFormatter().print([manifest.compact_dict()])
             return
 
         cols = ["name", "path", "kustomizations"]
         if query.cluster.namespace is None:
             cols.insert(0, "namespace")
```

### Comparing `flux-local-1.2.0/flux_local/tool/test.py` & `flux-local-1.3.0/flux_local/tool/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 _LOGGER = logging.getLogger(__name__)
 
 
 @dataclass
 class TestConfig:
     """Test configuration, which are parameters to types of the tests."""
 
+    options: git_repo.Options
     kube_version: str | None = None
     api_versions: str | None = None
 
 
 class HelmReleaseTest(pytest.Item):
     """Test case for a Kustomization."""
 
@@ -133,15 +134,20 @@
     def runtest(self) -> None:
         """Dispatch the async work and run the test."""
         nest_asyncio.apply()
         asyncio.run(self.async_runtest())
 
     async def async_runtest(self) -> None:
         """Run the Kustomizations test."""
-        cmd = await kustomize.build(Path(self.kustomization.path)).stash()
+        kustomize_flags = []
+        if self.test_config.options:
+            kustomize_flags = self.test_config.options.kustomize_flags
+        cmd = await kustomize.build(
+            Path(self.kustomization.path), kustomize_flags
+        ).stash()
         await cmd.objects()
         await cmd.validate_policies(self.cluster.cluster_policies)
 
 
 class KustomizationCollector(pytest.Collector):
     """Test collector for a Kustomization."""
 
@@ -272,30 +278,33 @@
     def pytest_sessionstart(self, session: pytest.Session) -> None:
         nest_asyncio.apply()
         asyncio.run(self.async_pytest_sessionstart(session))
 
     async def async_pytest_sessionstart(self, session: pytest.Session) -> None:
         """Run the Kustomizations test."""
         _LOGGER.debug("async_pytest_sessionstart")
-        manifest = await git_repo.build_manifest(selector=self.selector)
+        manifest = await git_repo.build_manifest(
+            selector=self.selector,
+            options=self.test_config.options,
+        )
         self.manifest = manifest
         _LOGGER.debug("async_pytest_sessionstart ended")
 
     def pytest_collection(self, session: pytest.Session) -> None:
         _LOGGER.debug("pytest_collection:%s", session)
         if not self.manifest:
             raise ValueError("ManifestPlugin not initialized properly")
         manifest_collector = ManifestCollector.from_parent(
             parent=session,
             manifest=self.manifest,
             test_config=self.test_config,
         )
         # Ignore the default files found by pytest and instead create
         # tests based on the manifest contents.
-        session.collect = manifest_collector.collect  # type: ignore[assignment]
+        session.collect = manifest_collector.collect  # type: ignore[method-assign]
         _LOGGER.debug("pytest_collection end:%s", session)
 
     def pytest_collection_modifyitems(
         self,
         session: pytest.Session,
         config: pytest.Config,
         items: list[pytest.Item],
@@ -397,14 +406,15 @@
             # If a real file path, then clear so it is not a test nodeid filter
             if test_path.startswith(".") or test_path.startswith("/"):
                 test_path = None
         query.kustomization.skip_crds = True
         query.helm_release.enabled = enable_helm
         query.helm_release.namespace = None
         query.cluster_policy.enabled = enable_kyverno
+        options = selector.options(**kwargs)
 
         nest_asyncio.apply()
         pytest_args = [
             "--verbosity",
             str(verbosity),
             "--no-header",
             "--disable-warnings",
@@ -414,14 +424,18 @@
         ]
         _LOGGER.debug("pytest.main: %s", pytest_args)
         retcode = pytest.main(
             pytest_args,
             plugins=[
                 ManifestPlugin(
                     query,
-                    TestConfig(kube_version=kube_version, api_versions=api_versions),
+                    TestConfig(
+                        options=options,
+                        kube_version=kube_version,
+                        api_versions=api_versions,
+                    ),
                     test_filter=[str(test_path)] if test_path else [],
                 )
             ],
         )
         if retcode:
             sys.exit(retcode)
```

### Comparing `flux-local-1.2.0/flux_local/tool/visitor.py` & `flux-local-1.3.0/flux_local/tool/visitor.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,32 +3,41 @@
 import asyncio
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 import logging
 import pathlib
 import tempfile
 import yaml
+from typing import Any
 
 from flux_local import git_repo
 from flux_local.kustomize import Kustomize
 from flux_local.helm import Helm
-from flux_local.manifest import HelmRelease, Kustomization, HelmRepository
+from flux_local.manifest import (
+    HelmRelease,
+    Kustomization,
+    HelmRepository,
+    ClusterPolicy,
+)
 
 
 _LOGGER = logging.getLogger(__name__)
 
 
 # Strip any annotations from kustomize that contribute to diff noise when
 # objects are re-ordered in the output
-STRIP_ANNOTATIONS = [
+STRIP_ATTRIBUTES = [
     "config.kubernetes.io/index",
     "internal.config.kubernetes.io/index",
 ]
 
 
+ResourceType = Kustomization | HelmRelease | HelmRepository | ClusterPolicy
+
+
 @dataclass(frozen=True, order=True)
 class ResourceKey:
     """Key for a Kustomization object output."""
 
     cluster_path: str
     kustomization_path: str
     kind: str
@@ -73,35 +82,29 @@
         return git_repo.ResourceVisitor(func=self.call_async)
 
     @abstractmethod
     async def call_async(
         self,
         cluster_path: pathlib.Path,
         kustomization_path: pathlib.Path,
-        doc: Kustomization | HelmRelease | HelmRepository,
+        doc: ResourceType,
         cmd: Kustomize | None,
     ) -> None:
         """Visitor function invoked to record build output."""
 
     def key_func(
         self,
         cluster_path: pathlib.Path,
         kustomization_path: pathlib.Path,
-        resource: Kustomization | HelmRelease | HelmRepository,
+        resource: ResourceType,
     ) -> ResourceKey:
-        if isinstance(resource, HelmRepository):
-            kind = "HelmRepostiory"
-        elif isinstance(resource, HelmRelease):
-            kind = "HelmRelease"
-        else:
-            kind = "Kustomization"
         return ResourceKey(
             cluster_path=str(cluster_path),
             kustomization_path=str(kustomization_path),
-            kind=kind,
+            kind=resource.__class__.__name__,
             namespace=resource.namespace or "",
             name=resource.name or "",
         )
 
 
 class ContentOutput(ResourceOutput):
     """Resource visitor that build string outputs."""
@@ -110,39 +113,56 @@
         """Initialize KustomizationContentOutput."""
         self.content: dict[ResourceKey, list[str]] = {}
 
     async def call_async(
         self,
         cluster_path: pathlib.Path,
         kustomization_path: pathlib.Path,
-        doc: Kustomization | HelmRelease | HelmRepository,
+        doc: ResourceType,
         cmd: Kustomize | None,
     ) -> None:
         """Visitor function invoked to record build output."""
         if cmd:
             content = await cmd.run()
             lines = content.split("\n")
             if lines[0] != "---":
                 lines.insert(0, "---")
             self.content[self.key_func(cluster_path, kustomization_path, doc)] = lines
 
 
+def strip_attrs(metadata: dict[str, Any], strip_attributes: list[str]) -> None:
+    """Update the resource object, stripping any requested labels to simplify diff."""
+
+    for attr_key in ("annotations", "labels"):
+        if not (val := metadata.get(attr_key)):
+            continue
+        for key in strip_attributes:
+            if key in val:
+                del val[key]
+            if not val:
+                del metadata[attr_key]
+                break
+
+
 class ObjectOutput(ResourceOutput):
     """Resource visitor that builds outputs for objects within the kustomization."""
 
-    def __init__(self) -> None:
+    def __init__(self, strip_attributes: list[str] | None) -> None:
         """Initialize ObjectOutput."""
         # Map of kustomizations to the map of built objects as lines of the yaml string
         self.content: dict[ResourceKey, dict[ResourceKey, list[str]]] = {}
+        self.strip_attributes = STRIP_ATTRIBUTES
+        if strip_attributes:
+            self.strip_attributes.extend(strip_attributes)
 
     async def call_async(
         self,
         cluster_path: pathlib.Path,
         kustomization_path: pathlib.Path,
-        doc: Kustomization | HelmRelease | HelmRepository,
+        doc: ResourceType,
         cmd: Kustomize | None,
     ) -> None:
         """Visitor function invoked to build and record resource objects."""
         if cmd:
             contents: dict[ResourceKey, list[str]] = {}
             objects = await cmd.objects()
             for resource in objects:
@@ -150,20 +170,23 @@
                     metadata := resource.get("metadata")
                 ):
                     _LOGGER.warning(
                         "Invalid document did not contain kind or metadata: %s",
                         resource,
                     )
                     continue
-                if annotations := metadata.get("annotations"):
-                    for key in STRIP_ANNOTATIONS:
-                        if key in annotations:
-                            del annotations[key]
-                    if not annotations:
-                        del metadata["annotations"]
+                # Remove common noisy labels
+                strip_attrs(metadata, self.strip_attributes)
+                # Remove common noisy labels in commonly used templates
+                if (
+                    (spec := resource.get("spec"))
+                    and (templ := spec.get("template"))
+                    and (meta := templ.get("metadata"))
+                ):
+                    strip_attrs(meta, self.strip_attributes)
                 resource_key = ResourceKey(
                     kind=kind,
                     cluster_path=str(cluster_path),
                     kustomization_path=str(kustomization_path),
                     namespace=metadata.get("namespace", doc.namespace),
                     name=metadata.get("name", ""),
                 )
@@ -211,15 +234,15 @@
 
     def repo_visitor(self) -> git_repo.ResourceVisitor:
         """Return a git_repo.ResourceVisitor that points to this object."""
 
         async def add_repo(
             cluster_path: pathlib.Path,
             kustomization_path: pathlib.Path,
-            doc: Kustomization | HelmRelease | HelmRepository,
+            doc: ResourceType,
             cmd: Kustomize | None,
         ) -> None:
             if not isinstance(doc, HelmRepository):
                 raise ValueError(f"Expected HelmRepository: {doc}")
             self.repos[str(cluster_path)] = self.repos.get(str(cluster_path), []) + [
                 doc
             ]
@@ -228,15 +251,15 @@
 
     def release_visitor(self) -> git_repo.ResourceVisitor:
         """Return a git_repo.ResourceVisitor that points to this object."""
 
         async def add_release(
             cluster_path: pathlib.Path,
             kustomization_path: pathlib.Path,
-            doc: Kustomization | HelmRelease | HelmRepository,
+            doc: ResourceType,
             cmd: Kustomize | None,
         ) -> None:
             if not isinstance(doc, HelmRelease):
                 raise ValueError(f"Expected HelmRelease: {doc}")
             self.releases[str(cluster_path)] = self.releases.get(
                 str(cluster_path), []
             ) + [doc]
```

### Comparing `flux-local-1.2.0/flux_local.egg-info/PKG-INFO` & `flux-local-1.3.0/flux_local.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-local
-Version: 1.2.0
+Version: 1.3.0
 Summary: flux-local is a python library and set of tools for managing a flux gitops repository, with validation steps to help improve quality of commits, PRs, and general local testing.
 Home-page: https://github.com/allenporter/flux-local
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
@@ -242,11 +242,98 @@
 
 clusters/dev .....................................                                                      [ 45%]
 clusters/prod ............................................                                              [100%]
 
 ======================================== 81 passed in 75.40s (0:01:15) ========================================
 ```
 
+## GitHub Action
+
+You may use `flux-local` as a github action to verify the health of the cluster on changes
+or PRs.
+
+### test action
+
+The `test` action will validate the cluster will build, and can optionally
+validate flux `HelmRelease` builds and also verify that all objects pass
+kyverno policies (e.g. for determining there are no deprecated api resources
+or that ingress objects are valid).
+
+This example will run `flux-local test` against the cluster in `clusters/prod` with
+helm release expansion enabled.
+
+```yaml
+- uses: allenporter/flux-local/test@2.0.0
+  with:
+    path: clusters/prod
+    enable-helm: true
+    enable-kyverno: false
+```
+
+### diff action
+
+The `diff` action will show you the final diffs of `Kustomization` or `HelmRelease`
+objects that are fully built. While typically you can just read diffs to understand
+how kustomzations may be affected, this action also supports overlays and multiple
+clusters showing you the final output.
+
+This is an example that diffs a `HelmRelease`:
+
+```yaml
+- uses: allenporter/flux-local/action/diff@2.0.0
+  id: diff
+  with:
+    live-branch: main
+    path: clusters/prod
+    resource: helmrelease
+- name: PR Comments
+  uses: mshick/add-pr-comment@v2
+  if: ${{ steps.diff.outputs.diff != '' }}
+  with:
+    repo-token: ${{ secrets.GITHUB_TOKEN }}
+    message-failure: Unable to post diff
+    message: |
+      `````diff
+      ${{ steps.diff.outputs.diff }}
+      `````
+```
+
+This is an example of a workflow that will diff `Kustomization` and `HelmRelease` objects
+in a repo with multiple clusters (`dev` and `prod`):
+
+```yaml
+jobs:
+  diffs:
+    name: Compute diffs
+    runs-on: ubuntu-latest
+    strategy:
+      matrix:
+        cluster_path:
+          - clusters/dev
+          - clusters/prod
+        resource:
+          - helmrelease
+          - kustomization
+    steps:
+      - uses: allenporter/flux-local/action/diff@2.0.0
+        id: diff
+        with:
+          live-branch: main
+          path: ${{ matrix.cluster_path }}
+          resource: ${{ matrix.resource }}
+      - name: PR Comments
+        uses: mshick/add-pr-comment@v2
+        if: ${{ steps.diff.outputs.diff != '' }}
+        with:
+          repo-token: ${{ secrets.GITHUB_TOKEN }}
+          message-id: ${{ matrix.cluster_path }}/${{ matrix.resource }}
+          message-failure: Unable to post kustomization diff
+          message: |
+            `````diff
+            ${{ steps.diff.outputs.diff }}
+            `````
+```
+
 ## Library
 
 The `flux_local` [library documentation](https://allenporter.github.io/flux-local/) for details
 on the python APIs provided.
```

### Comparing `flux-local-1.2.0/flux_local.egg-info/SOURCES.txt` & `flux-local-1.3.0/flux_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flux-local-1.2.0/setup.cfg` & `flux-local-1.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flux-local
-version = 1.2.0
+version = 1.3.0
 description = flux-local is a python library and set of tools for managing a flux gitops repository, with validation steps to help improve quality of commits, PRs, and general local testing.
 long_description = file: README.md
 long_description_content_type = text/markdown
 prodid = github.com/allenporter/flux-local
 url = https://github.com/allenporter/flux-local
 author = Allen Porter
 author_email = allen.porter@gmail.com
```

### Comparing `flux-local-1.2.0/tests/test_command.py` & `flux-local-1.3.0/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.2.0/tests/test_git_repo.py` & `flux-local-1.3.0/tests/test_git_repo.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from unittest.mock import patch
 
 from flux_local.git_repo import (
     build_manifest,
     ResourceSelector,
     ResourceVisitor,
     kustomization_traversal,
+    Source,
     PathSelector,
     make_clusters,
 )
 from flux_local.kustomize import Kustomize
 from flux_local.manifest import Kustomization
 
 TESTDATA = Path("tests/testdata/cluster")
@@ -26,16 +27,16 @@
     manifest = await build_manifest(TESTDATA)
     assert len(manifest.clusters) == 1
     cluster = manifest.clusters[0]
     assert cluster.name == "flux-system"
     assert cluster.namespace == "flux-system"
     assert cluster.path == "./tests/testdata/cluster/clusters/prod"
     assert len(cluster.kustomizations) == 4
-    assert len(cluster.helm_repos) == 2
-    assert len(cluster.helm_releases) == 2
+    assert len(cluster.helm_repos) == 3
+    assert len(cluster.helm_releases) == 3
 
 
 async def test_build_manifest_ks_path() -> None:
     """Tests for building a kustomization directly."""
 
     query = ResourceSelector()
     query.path.path = TESTDATA / "apps/prod"
@@ -89,15 +90,15 @@
     manifest = await build_manifest(selector=query)
     assert len(manifest.clusters) == 1
     cluster = manifest.clusters[0]
     assert cluster.name == "flux-system"
     assert cluster.namespace == "flux-system"
     assert cluster.path == "./tests/testdata/cluster/clusters/prod"
     assert len(cluster.kustomizations) == 4
-    assert len(cluster.helm_repos) == 2
+    assert len(cluster.helm_repos) == 3
     assert len(cluster.helm_releases) == 0
 
 
 async def test_helm_repo_selector_disabled() -> None:
     """Tests for building the manifest with helm repos disabled."""
 
     query = ResourceSelector()
@@ -108,15 +109,15 @@
     assert len(manifest.clusters) == 1
     cluster = manifest.clusters[0]
     assert cluster.name == "flux-system"
     assert cluster.namespace == "flux-system"
     assert cluster.path == "./tests/testdata/cluster/clusters/prod"
     assert len(cluster.kustomizations) == 4
     assert len(cluster.helm_repos) == 0
-    assert len(cluster.helm_releases) == 2
+    assert len(cluster.helm_releases) == 3
 
 
 async def test_kustomization_visitor() -> None:
     """Tests for visiting Kustomizations."""
 
     query = ResourceSelector()
     query.path.path = TESTDATA
@@ -195,16 +196,16 @@
     manifest = await build_manifest(selector=query)
     assert len(manifest.clusters) == 1
     cluster = manifest.clusters[0]
     assert cluster.name == "flux-system"
     assert cluster.namespace == "flux-system"
     assert cluster.path == "./tests/testdata/cluster/clusters/prod"
     assert len(cluster.kustomizations) == 4
-    assert len(cluster.helm_repos) == 2
-    assert len(cluster.helm_releases) == 2
+    assert len(cluster.helm_repos) == 3
+    assert len(cluster.helm_releases) == 3
 
     visits.sort()
     assert visits == [
         (
             "tests/testdata/cluster/clusters/prod",
             "tests/testdata/cluster/infrastructure/configs",
             "flux-system",
@@ -212,14 +213,20 @@
         ),
         (
             "tests/testdata/cluster/clusters/prod",
             "tests/testdata/cluster/infrastructure/configs",
             "flux-system",
             "podinfo",
         ),
+        (
+            "tests/testdata/cluster/clusters/prod",
+            "tests/testdata/cluster/infrastructure/configs",
+            "flux-system",
+            "weave-charts",
+        ),
     ]
 
 
 async def test_helm_release_visitor() -> None:
     """Tests for visiting a HelmRelease objects."""
 
     query = ResourceSelector()
@@ -237,28 +244,34 @@
     manifest = await build_manifest(selector=query)
     assert len(manifest.clusters) == 1
     cluster = manifest.clusters[0]
     assert cluster.name == "flux-system"
     assert cluster.namespace == "flux-system"
     assert cluster.path == "./tests/testdata/cluster/clusters/prod"
     assert len(cluster.kustomizations) == 4
-    assert len(cluster.helm_repos) == 2
-    assert len(cluster.helm_releases) == 2
+    assert len(cluster.helm_repos) == 3
+    assert len(cluster.helm_releases) == 3
 
     visits.sort()
     assert visits == [
         (
             "tests/testdata/cluster/clusters/prod",
             "tests/testdata/cluster/apps/prod",
             "podinfo",
             "podinfo",
         ),
         (
             "tests/testdata/cluster/clusters/prod",
             "tests/testdata/cluster/infrastructure/controllers",
+            "flux-system",
+            "weave-gitops",
+        ),
+        (
+            "tests/testdata/cluster/clusters/prod",
+            "tests/testdata/cluster/infrastructure/controllers",
             "metallb",
             "metallb",
         ),
     ]
 
 
 @pytest.mark.parametrize(
@@ -419,7 +432,23 @@
     assert cluster.namespace == "flux-system"
     assert cluster.path == "./clusters/prod"
     assert [ks.path for ks in cluster.kustomizations] == [
         "./certmanager/prod",
         "./clusters/prod",
         "./crds",
     ]
+
+
+def test_source() -> None:
+    """Test parsing a source from a string."""
+    source = Source.from_str("cluster=./k8s")
+    assert source.name == "cluster"
+    assert source.namespace == "flux-system"
+    assert str(source.root) == "k8s"
+
+
+def test_source_with_namespace() -> None:
+    """Test parsing a source from a string."""
+    source = Source.from_str("flux-system2/cluster=./k8s")
+    assert source.name == "cluster"
+    assert source.namespace == "flux-system2"
+    assert str(source.root) == "k8s"
```

### Comparing `flux-local-1.2.0/tests/test_helm.py` & `flux-local-1.3.0/tests/test_helm.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,13 +52,13 @@
     await helm.update()
 
 
 async def test_template(helm: Helm, helm_releases: list[dict[str, Any]]) -> None:
     """Test helm template command."""
     await helm.update()
 
-    assert len(helm_releases) == 1
+    assert len(helm_releases) == 2
     release = helm_releases[0]
     obj = await helm.template(HelmRelease.parse_doc(release))
     docs = await obj.grep("kind=ServiceAccount").objects()
     names = [doc.get("metadata", {}).get("name") for doc in docs]
     assert names == ["metallb-controller", "metallb-speaker"]
```

### Comparing `flux-local-1.2.0/tests/test_kustomize.py` & `flux-local-1.3.0/tests/test_kustomize.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.2.0/tests/test_manifest.py` & `flux-local-1.3.0/tests/test_manifest.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
     docs = list(
         yaml.load_all(
             (TESTDATA_DIR / "configs/helm-repositories.yaml").read_text(),
             Loader=yaml.CLoader,
         )
     )
-    assert len(docs) == 2
+    assert len(docs) == 3
     repo = HelmRepository.parse_doc(docs[0])
     assert repo.name == "bitnami"
     assert repo.namespace == "flux-system"
     assert repo.url == "https://charts.bitnami.com/bitnami"
     assert repo.repo_type == "default"
     repo = HelmRepository.parse_doc(docs[1])
     assert repo.name == "podinfo"
```

