# Comparing `tmp/ghas_cli-1.5.0.tar.gz` & `tmp/ghas_cli-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghas_cli-1.5.0.tar", max compression
+gzip compressed data, was "ghas_cli-1.5.1.tar", max compression
```

## Comparing `ghas_cli-1.5.0.tar` & `ghas_cli-1.5.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rwxr-xr-x   0        0        0     1069 2023-02-08 18:00:34.563166 ghas_cli-1.5.0/LICENSE
--rwxr-xr-x   0        0        0     4878 2023-05-10 13:28:28.804158 ghas_cli-1.5.0/README.md
--rwxr-xr-x   0        0        0     1134 2023-05-10 17:42:46.091602 ghas_cli-1.5.0/pyproject.toml
--rwxr-xr-x   0        0        0    33392 2023-05-10 17:42:57.305520 ghas_cli-1.5.0/src/cli.py
--rwxr-xr-x   0        0        0        0 2023-02-08 18:00:34.643212 ghas_cli-1.5.0/src/ghas_cli/__init__.py
--rwxr-xr-x   0        0        0        0 2023-02-08 18:00:34.673123 ghas_cli-1.5.0/src/ghas_cli/utils/__init__.py
--rwxr-xr-x   0        0        0      666 2023-02-08 18:00:34.698192 ghas_cli-1.5.0/src/ghas_cli/utils/actions.py
--rwxr-xr-x   0        0        0      417 2023-05-10 17:42:10.795557 ghas_cli-1.5.0/src/ghas_cli/utils/export.py
--rwxr-xr-x   0        0        0     2810 2023-02-08 18:00:34.732994 ghas_cli-1.5.0/src/ghas_cli/utils/issues.py
--rwxr-xr-x   0        0        0     2120 2023-05-10 17:42:10.801997 ghas_cli-1.5.0/src/ghas_cli/utils/network.py
--rwxr-xr-x   0        0        0    21717 2023-05-10 17:42:10.811903 ghas_cli-1.5.0/src/ghas_cli/utils/repositories.py
--rwxr-xr-x   0        0        0     1285 2023-02-08 18:00:34.788075 ghas_cli-1.5.0/src/ghas_cli/utils/roles.py
--rwxr-xr-x   0        0        0     1350 2023-05-10 17:42:10.817870 ghas_cli-1.5.0/src/ghas_cli/utils/secrets.py
--rwxr-xr-x   0        0        0     2575 2023-05-10 17:42:10.825735 ghas_cli-1.5.0/src/ghas_cli/utils/teams.py
--rwxr-xr-x   0        0        0     1442 2023-05-10 13:28:28.864807 ghas_cli-1.5.0/src/ghas_cli/utils/vulns.py
--rw-r--r--   0        0        0     6208 1970-01-01 00:00:00.000000 ghas_cli-1.5.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2023-02-08 18:00:34.563166 ghas_cli-1.5.1/LICENSE
+-rwxr-xr-x   0        0        0     5338 2023-05-31 10:45:00.256447 ghas_cli-1.5.1/README.md
+-rwxr-xr-x   0        0        0     1142 2023-05-31 10:45:18.206032 ghas_cli-1.5.1/pyproject.toml
+-rwxr-xr-x   0        0        0    34814 2023-05-31 10:45:28.169160 ghas_cli-1.5.1/src/cli.py
+-rwxr-xr-x   0        0        0        0 2023-02-08 18:00:34.643212 ghas_cli-1.5.1/src/ghas_cli/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-02-08 18:00:34.673123 ghas_cli-1.5.1/src/ghas_cli/utils/__init__.py
+-rwxr-xr-x   0        0        0      666 2023-05-24 11:38:02.249582 ghas_cli-1.5.1/src/ghas_cli/utils/actions.py
+-rwxr-xr-x   0        0        0      417 2023-05-24 11:38:02.256021 ghas_cli-1.5.1/src/ghas_cli/utils/export.py
+-rwxr-xr-x   0        0        0     2810 2023-02-08 18:00:34.732994 ghas_cli-1.5.1/src/ghas_cli/utils/issues.py
+-rwxr-xr-x   0        0        0     2228 2023-05-24 11:38:02.262906 ghas_cli-1.5.1/src/ghas_cli/utils/network.py
+-rwxr-xr-x   0        0        0    21784 2023-05-31 10:45:00.279130 ghas_cli-1.5.1/src/ghas_cli/utils/repositories.py
+-rwxr-xr-x   0        0        0     1285 2023-05-24 11:38:02.277202 ghas_cli-1.5.1/src/ghas_cli/utils/roles.py
+-rwxr-xr-x   0        0        0     1350 2023-05-24 11:38:02.282627 ghas_cli-1.5.1/src/ghas_cli/utils/secrets.py
+-rwxr-xr-x   0        0        0     2575 2023-05-24 11:38:02.289058 ghas_cli-1.5.1/src/ghas_cli/utils/teams.py
+-rwxr-xr-x   0        0        0     1442 2023-05-24 11:38:02.295934 ghas_cli-1.5.1/src/ghas_cli/utils/vulns.py
+-rw-r--r--   0        0        0     6668 1970-01-01 00:00:00.000000 ghas_cli-1.5.1/PKG-INFO
```

### Comparing `ghas_cli-1.5.0/LICENSE` & `ghas_cli-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ghas_cli-1.5.0/README.md` & `ghas_cli-1.5.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # ghas-cli
 
 [![CodeQL](https://github.com/Malwarebytes/ghas-cli/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/Malwarebytes/ghas-cli/actions/workflows/codeql-analysis.yml)
+[![Downloads](https://static.pepy.tech/personalized-badge/ghas-cli?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads)](https://pepy.tech/project/ghas-cli)
+[![Supported Versions](https://img.shields.io/pypi/pyversions/ghas-cli.svg)](https://pypi.org/project/ghas-cli)
+[![Contributors](https://img.shields.io/github/contributors/malwarebytes/ghas-cli.svg)](https://github.com/malwarebytes/ghas-cli/graphs/contributors)
 
 CLI utility to interact with [GitHub Advanced Security](https://docs.github.com/en/enterprise-cloud@latest/get-started/learning-about-github/about-github-advanced-security) (_"GHAS"_).
 
 It allows to deploy GHAS features individually or at scale, while taking into account each repository configuration.
 
 More specifically, it automates the following:
```

### Comparing `ghas_cli-1.5.0/pyproject.toml` & `ghas_cli-1.5.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ghas-cli"
-version = "1.5.0"
+version = "1.5.1"
 description = "Command line interface to interact with GitHub Advanced Security."
 authors = ["jboursier <jboursier@malwarebytes.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Malwarebytes/ghas-cli"
 documentation = "https://github.com/Malwarebytes/ghas-cli/wiki"
 repository = "https://github.com/Malwarebytes/ghas-cli"
@@ -24,15 +24,15 @@
 [tool.poetry.dependencies]
 python = ">=3.7,<4"
 click = ">=8"
 requests = "*"
 colorama = "*"
 configparser = "*"
 python-magic = "*"
-urllib3 = "^1.26.12"
+urllib3 = ">=1.26.12,<3.0.0"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.scripts]
 ghas-cli = 'src.cli:main'
 
 [build-system]
```

### Comparing `ghas_cli-1.5.0/src/cli.py` & `ghas_cli-1.5.1/src/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 #!/usr/bin/env python3
 
 __author__ = "jboursier"
 __copyright__ = "Copyright 2023, Malwarebytes"
-__version__ = "1.5.0"
+__version__ = "1.5.1"
 __maintainer__ = "jboursier"
 __email__ = "jboursier@malwarebytes.com"
 __status__ = "Production"
 
 try:
     import click
     import json
@@ -475,15 +475,41 @@
 @click.option("-o", "--organization", prompt="Organization name", type=str)
 def repositories_archive(
     repository: str,
     organization: str,
     token: str,
 ) -> None:
     """Archive a repository"""
-    click.echo(repositories.archive(organization, token, repository))
+    click.echo(repositories.archive(organization, token, repository, archive=True))
+
+
+@repositories_cli.command("unarchive")
+@click.option(
+    "-r",
+    "--repository",
+    prompt="Repository name",
+)
+@click.option(
+    "-t",
+    "--token",
+    prompt=False,
+    type=str,
+    default=None,
+    hide_input=True,
+    confirmation_prompt=False,
+    show_envvar=True,
+)
+@click.option("-o", "--organization", prompt="Organization name", type=str)
+def repositories_unarchive(
+    repository: str,
+    organization: str,
+    token: str,
+) -> None:
+    """Unarchive a repository"""
+    click.echo(repositories.archive(organization, token, repository, archive=False))
 
 
 #########
 # Teams #
 #########
 
 
@@ -1201,21 +1227,55 @@
 
     for repo in repos_list:
         repo = repo.rstrip("\n")
 
         click.echo(f"{repo}...", nl=False)
 
         if repositories.archive(
-            organization=organization, token=token, repository=repo
+            organization=organization, token=token, repository=repo, archive=True
         ):
             click.echo(" Archived.")
         else:
             click.echo(" Not Archived.", err=True)
 
 
+@mass_cli.command("unarchive")
+@click.argument("input_repos_list", type=click.File("r"))
+@click.option(
+    "-t",
+    "--token",
+    prompt=False,
+    type=str,
+    default=None,
+    hide_input=True,
+    confirmation_prompt=False,
+    show_envvar=True,
+)
+@click.option("-o", "--organization", prompt="Organization name", type=str)
+def mass_unarchive(
+    input_repos_list: Any,
+    organization: str,
+    token: str,
+) -> None:
+    repos_list = input_repos_list.readlines()
+
+    for repo in repos_list:
+
+        repo = repo.rstrip("\n")
+
+        click.echo(f"{repo}...", nl=False)
+
+        if repositories.archive(
+            organization=organization, token=token, repository=repo, archive=False
+        ):
+            click.echo(" Unarchived.")
+        else:
+            click.echo(" Not Unarchived.", err=True)
+
+
 @mass_cli.command("issue_upcoming_archive")
 @click.argument("input_repos_list", type=click.File("r"))
 @click.option(
     "-u",
     "--archived_date",
     prompt="Target date when the repositories will be archived",
     type=str,
```

### Comparing `ghas_cli-1.5.0/src/ghas_cli/utils/actions.py` & `ghas_cli-1.5.1/src/ghas_cli/utils/actions.py`

 * *Files identical despite different names*

### Comparing `ghas_cli-1.5.0/src/ghas_cli/utils/issues.py` & `ghas_cli-1.5.1/src/ghas_cli/utils/issues.py`

 * *Files identical despite different names*

### Comparing `ghas_cli-1.5.0/src/ghas_cli/utils/network.py` & `ghas_cli-1.5.1/src/ghas_cli/utils/network.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,27 +17,31 @@
 RETRIES = 5
 
 
 def get_github_headers(token: str) -> Dict:
     return {
         "accept": "application/vnd.github+json",
         "authorization": f"Bearer {token}",
-        "User-Agent": "malwarebytes/bulk_enable_ghas",
+        "User-Agent": "malwarebytes/ghas-cli",
         "X-GitHub-Api-Version": "2022-11-28",  # https://docs.github.com/en/rest/overview/api-versions#supported-api-versions
     }
 
 
 def check_rate_limit(response: Any) -> bool:
     if "0" == response.headers["x-ratelimit-remaining"]:
         reset_time = datetime.fromtimestamp(int(response.headers["x-ratelimit-reset"]))
         logging.warn(
             f"Rate limit reached: {response.headers['x-ratelimit-remaining']}/{response.headers['x-ratelimit-limit']} - {reset_time}"
         )
 
-        time.sleep(int(response.headers["x-ratelimit-remaining"]))
+        time_to_wait = int(reset_time.timestamp()) - (time.time())
+        
+        logging.info(f"Waiting {time_to_wait} seconds before retrying.")
+        time.sleep(time_to_wait)
+
         return True
 
     if response.status_code == 403:
         # This can be secondary rate limit or SSO error
         logging.warn(response.json()["message"])
         return True
```

### Comparing `ghas_cli-1.5.0/src/ghas_cli/utils/repositories.py` & `ghas_cli-1.5.1/src/ghas_cli/utils/repositories.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,18 +233,20 @@
     branch_res = branch_res.json()
 
     return datetime.datetime.strptime(
         branch_res["commit"]["commit"]["author"]["date"].split("T")[0], "%Y-%m-%d"
     )
 
 
-def archive(organization: str, token: str, repository: str) -> bool:
+def archive(
+    organization: str, token: str, repository: str, archive: bool = True
+) -> bool:
     headers = network.get_github_headers(token)
 
-    payload = {"archived": True}
+    payload = {"archived": archive}
 
     status = network.patch(
         url=f"https://api.github.com/repos/{organization}/{repository}",
         headers=headers,
         json=payload,
     )
 
@@ -398,15 +400,15 @@
 
 
 def load_codeql_base64_template(
     languages: List, branches: List = ["main"]
 ) -> str:
     with open(f"./templates/codeql-analysis-default.yml", "r") as f:
         data = "".join(f.readlines())
-        data = data.replace("""branches: [ ]""", f"""branches: [{', '.join(f"'branch'" for branch in branches)   }]""")
+        data = data.replace("""branches: [ ]""", f"""branches: [{', '.join(f"'{branch}'" for branch in branches)   }]""")
         data = data.replace("""language: [ ]""", f"""language: {languages}""")
         return base64.b64encode(data.encode("utf-8")).decode("utf-8")
 
 
 def load_codeql_config_base64_template() -> str:
     with open(f"./templates/codeql-config-default.yml", "r") as f:
         template = f.read()
@@ -489,23 +491,23 @@
     # Workflow config
     template = load_codeql_base64_template(languages, [default_branch])
     workflow_commit_payload = {
         "message": f"Create CodeQL analysis workflow",
         "content": template,
         "branch": target_branch,
         "sha": get_file_sha(
-            organization, repository, headers, ".github/workflows/codeql.yml"
+            organization, repository, headers, ".github/workflows/codeql-analysis-default.yml"
         ),
     }
 
     if workflow_commit_payload["sha"]:
         workflow_commit_payload["message"] = "Update CodeQL analysis workflow"
 
     workflow_commit_resp = network.put(
-        url=f"https://api.github.com/repos/{organization}/{repository}/contents/.github/workflows/codeql.yml",
+        url=f"https://api.github.com/repos/{organization}/{repository}/contents/.github/workflows/codeql-analysis-default.yml",
         headers=headers,
         json=workflow_commit_payload,
     )
 
     if workflow_commit_resp.status_code not in [200, 201]:
         logging.error(
             f"Commit response for CodeQL workflow: {workflow_commit_resp.status_code}"
```

### Comparing `ghas_cli-1.5.0/src/ghas_cli/utils/roles.py` & `ghas_cli-1.5.1/src/ghas_cli/utils/roles.py`

 * *Files identical despite different names*

### Comparing `ghas_cli-1.5.0/src/ghas_cli/utils/secrets.py` & `ghas_cli-1.5.1/src/ghas_cli/utils/secrets.py`

 * *Files identical despite different names*

### Comparing `ghas_cli-1.5.0/src/ghas_cli/utils/teams.py` & `ghas_cli-1.5.1/src/ghas_cli/utils/teams.py`

 * *Files identical despite different names*

### Comparing `ghas_cli-1.5.0/src/ghas_cli/utils/vulns.py` & `ghas_cli-1.5.1/src/ghas_cli/utils/vulns.py`

 * *Files identical despite different names*

### Comparing `ghas_cli-1.5.0/PKG-INFO` & `ghas_cli-1.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghas-cli
-Version: 1.5.0
+Version: 1.5.1
 Summary: Command line interface to interact with GitHub Advanced Security.
 Home-page: https://github.com/Malwarebytes/ghas-cli
 License: MIT
 Keywords: security,cli,github,utility
 Author: jboursier
 Author-email: jboursier@malwarebytes.com
 Requires-Python: >=3.7,<4
@@ -23,22 +23,25 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Requires-Dist: click (>=8)
 Requires-Dist: colorama
 Requires-Dist: configparser
 Requires-Dist: python-magic
 Requires-Dist: requests
-Requires-Dist: urllib3 (>=1.26.12,<2.0.0)
+Requires-Dist: urllib3 (>=1.26.12,<3.0.0)
 Project-URL: Documentation, https://github.com/Malwarebytes/ghas-cli/wiki
 Project-URL: Repository, https://github.com/Malwarebytes/ghas-cli
 Description-Content-Type: text/markdown
 
 # ghas-cli
 
 [![CodeQL](https://github.com/Malwarebytes/ghas-cli/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/Malwarebytes/ghas-cli/actions/workflows/codeql-analysis.yml)
+[![Downloads](https://static.pepy.tech/personalized-badge/ghas-cli?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Downloads)](https://pepy.tech/project/ghas-cli)
+[![Supported Versions](https://img.shields.io/pypi/pyversions/ghas-cli.svg)](https://pypi.org/project/ghas-cli)
+[![Contributors](https://img.shields.io/github/contributors/malwarebytes/ghas-cli.svg)](https://github.com/malwarebytes/ghas-cli/graphs/contributors)
 
 CLI utility to interact with [GitHub Advanced Security](https://docs.github.com/en/enterprise-cloud@latest/get-started/learning-about-github/about-github-advanced-security) (_"GHAS"_).
 
 It allows to deploy GHAS features individually or at scale, while taking into account each repository configuration.
 
 More specifically, it automates the following:
```

