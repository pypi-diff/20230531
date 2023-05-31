# Comparing `tmp/jupyverse-0.1.6.tar.gz` & `tmp/jupyverse-0.1.8.tar.gz`

## Comparing `jupyverse-0.1.6.tar` & `jupyverse-0.1.8.tar`

### file list

```diff
@@ -1,207 +1,217 @@
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 jupyverse-0.1.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0    61901 2020-02-02 00:00:00.000000 jupyverse-0.1.6/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 jupyverse-0.1.6/CONTRIBUTING.md
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyverse-0.1.6/MANIFEST.in
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 jupyverse-0.1.6/config.yaml
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 jupyverse-0.1.6/mkdocs.yml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 jupyverse-0.1.6/pytest.ini
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 jupyverse-0.1.6/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyverse-0.1.6/.devcontainer/requirements.txt
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 jupyverse-0.1.6/.github/workflows/check-release.yml
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 jupyverse-0.1.6/.github/workflows/main.yml
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 jupyverse-0.1.6/binder/environment.yml
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 jupyverse-0.1.6/binder/jupyter_notebook_config.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 jupyverse-0.1.6/binder/postBuild
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 jupyverse-0.1.6/binder/start
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 jupyverse-0.1.6/docs/index.md
--rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 jupyverse-0.1.6/docs/install.md
--rw-r--r--   0        0        0    11002 2020-02-02 00:00:00.000000 jupyverse-0.1.6/docs/jupyter.svg
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 jupyverse-0.1.6/docs/plugins/auth.md
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 jupyverse-0.1.6/docs/plugins/contents.md
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 jupyverse-0.1.6/docs/plugins/frontend.md
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyverse-0.1.6/docs/plugins/jupyterlab.md
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyverse-0.1.6/docs/plugins/kernels.md
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 jupyverse-0.1.6/docs/plugins/lab.md
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyverse-0.1.6/docs/plugins/login.md
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyverse-0.1.6/docs/plugins/nbconvert.md
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 jupyverse-0.1.6/docs/plugins/resource_usage.md
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 jupyverse-0.1.6/docs/plugins/retrolab.md
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 jupyverse-0.1.6/docs/plugins/terminals.md
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupyverse-0.1.6/docs/plugins/yjs.md
--rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 jupyverse-0.1.6/docs/usage/microservices.md
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 jupyverse-0.1.6/docs/usage/multi_user.md
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 jupyverse-0.1.6/docs/usage/single_user.md
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse/py.typed
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/COPYING.md
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/README.md
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/pyproject.toml
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/__init__.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/cli.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/py.typed
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/app/__init__.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/auth/__init__.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/auth/models.py
--rw-r--r--   0        0        0     4918 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/contents/__init__.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/contents/models.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/frontend/__init__.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/jupyterlab/__init__.py
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/kernels/__init__.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/kernels/models.py
--rw-r--r--   0        0        0     5439 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/lab/__init__.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/login/__init__.py
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/main/__init__.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/nbconvert/__init__.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/resource_usage/__init__.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/retrolab/__init__.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/terminals/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/terminals/models.py
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/yjs/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 jupyverse-0.1.6/jupyverse_api/jupyverse_api/yjs/models.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth/MANIFEST.in
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth/README.md
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth/fps_auth/__init__.py
--rw-r--r--   0        0        0    11596 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth/fps_auth/backends.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth/fps_auth/config.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth/fps_auth/db.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth/fps_auth/main.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth/fps_auth/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth/fps_auth/py.typed
--rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth/fps_auth/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth_fief/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth_fief/MANIFEST.in
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth_fief/README.md
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth_fief/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth_fief/fps_auth_fief/__init__.py
--rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth_fief/fps_auth_fief/backend.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth_fief/fps_auth_fief/config.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth_fief/fps_auth_fief/main.py
--rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/auth_fief/fps_auth_fief/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/contents/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/contents/MANIFEST.in
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/contents/README.md
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/contents/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/contents/fps_contents/__init__.py
--rw-r--r--   0        0        0     8386 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/contents/fps_contents/fileid.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/contents/fps_contents/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/contents/fps_contents/py.typed
--rw-r--r--   0        0        0     9082 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/contents/fps_contents/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/frontend/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/frontend/MANIFEST.in
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/frontend/README.md
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/frontend/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/frontend/fps_frontend/__init__.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/frontend/fps_frontend/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/frontend/fps_frontend/py.typed
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/jupyterlab/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/jupyterlab/MANIFEST.in
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/jupyterlab/README.md
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/jupyterlab/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/jupyterlab/fps_jupyterlab/__init__.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/jupyterlab/fps_jupyterlab/index.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/jupyterlab/fps_jupyterlab/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/jupyterlab/fps_jupyterlab/py.typed
--rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/jupyterlab/fps_jupyterlab/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/kernels/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/kernels/MANIFEST.in
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/kernels/README.md
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/kernels/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/kernels/fps_kernels/__init__.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/kernels/fps_kernels/main.py
--rw-r--r--   0        0        0    13051 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/kernels/fps_kernels/routes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/kernels/fps_kernels/kernel_driver/__init__.py
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/kernels/fps_kernels/kernel_driver/connect.py
--rw-r--r--   0        0        0     8632 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/kernels/fps_kernels/kernel_driver/driver.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/kernels/fps_kernels/kernel_driver/kernelspec.py
--rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/kernels/fps_kernels/kernel_driver/message.py
--rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/kernels/fps_kernels/kernel_driver/paths.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/kernels/fps_kernels/kernel_server/__init__.py
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/kernels/fps_kernels/kernel_server/message.py
--rw-r--r--   0        0        0    11591 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/kernels/fps_kernels/kernel_server/server.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/lab/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/lab/MANIFEST.in
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/lab/README.md
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/lab/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/lab/fps_lab/__init__.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/lab/fps_lab/main.py
--rw-r--r--   0        0        0     6739 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/lab/fps_lab/routes.py
--rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/lab/fps_lab/static/favicon.ico
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/login/COPYING.md
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/login/MANIFEST.in
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/login/README.md
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/login/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/login/fps_login/__init__.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/login/fps_login/main.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/login/fps_login/routes.py
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/login/fps_login/static/index.html
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/login/fps_login/static/favicons/favicon-busy-1.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/login/fps_login/static/favicons/favicon-busy-2.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/login/fps_login/static/favicons/favicon-busy-3.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/login/fps_login/static/favicons/favicon-file.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/login/fps_login/static/favicons/favicon-notebook.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/login/fps_login/static/favicons/favicon-terminal.ico
--rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/login/fps_login/static/favicons/favicon.ico
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/login/fps_login/static/logo/github.svg
--rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/login/fps_login/static/logo/logo.png
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/login/fps_login/static/style/index.css
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/nbconvert/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/nbconvert/MANIFEST.in
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/nbconvert/README.md
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/nbconvert/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/nbconvert/fps_nbconvert/__init__.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/nbconvert/fps_nbconvert/main.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/nbconvert/fps_nbconvert/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/noauth/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/noauth/MANIFEST.in
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/noauth/README.md
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/noauth/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/noauth/fps_noauth/__init__.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/noauth/fps_noauth/backends.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/noauth/fps_noauth/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/noauth/fps_noauth/py.typed
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/resource_usage/COPYING.md
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/resource_usage/README.md
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/resource_usage/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/resource_usage/fps_resource_usage/__init__.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/resource_usage/fps_resource_usage/main.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/resource_usage/fps_resource_usage/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/retrolab/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/retrolab/MANIFEST.in
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/retrolab/README.md
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/retrolab/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/retrolab/fps_retrolab/__init__.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/retrolab/fps_retrolab/main.py
--rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/retrolab/fps_retrolab/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/terminals/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/terminals/MANIFEST.in
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/terminals/README.md
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/terminals/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/terminals/fps_terminals/__init__.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/terminals/fps_terminals/main.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/terminals/fps_terminals/routes.py
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/terminals/fps_terminals/server.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/terminals/fps_terminals/win_server.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/yjs/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/yjs/MANIFEST.in
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/yjs/README.md
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/yjs/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/yjs/fps_yjs/__init__.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/yjs/fps_yjs/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/yjs/fps_yjs/py.typed
--rw-r--r--   0        0        0    13858 2020-02-02 00:00:00.000000 jupyverse-0.1.6/plugins/yjs/fps_yjs/routes.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 jupyverse-0.1.6/tests/conftest.py
--rw-r--r--   0        0        0     4485 2020-02-02 00:00:00.000000 jupyverse-0.1.6/tests/test_auth.py
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupyverse-0.1.6/tests/test_contents.py
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 jupyverse-0.1.6/tests/test_kernels.py
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 jupyverse-0.1.6/tests/test_server.py
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 jupyverse-0.1.6/tests/test_settings.py
--rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 jupyverse-0.1.6/tests/utils.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 jupyverse-0.1.6/tests/data/notebook0.ipynb
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 jupyverse-0.1.6/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.6/COPYING.md
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 jupyverse-0.1.6/README.md
--rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 jupyverse-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 jupyverse-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 jupyverse-0.1.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    63500 2020-02-02 00:00:00.000000 jupyverse-0.1.8/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 jupyverse-0.1.8/CONTRIBUTING.md
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyverse-0.1.8/MANIFEST.in
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 jupyverse-0.1.8/config.yaml
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 jupyverse-0.1.8/mkdocs.yml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 jupyverse-0.1.8/pytest.ini
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 jupyverse-0.1.8/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyverse-0.1.8/.devcontainer/requirements.txt
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 jupyverse-0.1.8/.github/workflows/check-release.yml
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 jupyverse-0.1.8/.github/workflows/main.yml
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 jupyverse-0.1.8/binder/environment.yml
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 jupyverse-0.1.8/binder/jupyter_notebook_config.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 jupyverse-0.1.8/binder/postBuild
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 jupyverse-0.1.8/binder/start
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 jupyverse-0.1.8/docs/index.md
+-rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 jupyverse-0.1.8/docs/install.md
+-rw-r--r--   0        0        0    11002 2020-02-02 00:00:00.000000 jupyverse-0.1.8/docs/jupyter.svg
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 jupyverse-0.1.8/docs/plugins/auth.md
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 jupyverse-0.1.8/docs/plugins/contents.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 jupyverse-0.1.8/docs/plugins/frontend.md
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyverse-0.1.8/docs/plugins/jupyterlab.md
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyverse-0.1.8/docs/plugins/kernels.md
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 jupyverse-0.1.8/docs/plugins/lab.md
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyverse-0.1.8/docs/plugins/login.md
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyverse-0.1.8/docs/plugins/nbconvert.md
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 jupyverse-0.1.8/docs/plugins/resource_usage.md
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 jupyverse-0.1.8/docs/plugins/retrolab.md
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 jupyverse-0.1.8/docs/plugins/terminals.md
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupyverse-0.1.8/docs/plugins/yjs.md
+-rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 jupyverse-0.1.8/docs/usage/microservices.md
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 jupyverse-0.1.8/docs/usage/multi_user.md
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 jupyverse-0.1.8/docs/usage/single_user.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse/py.typed
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/COPYING.md
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/README.md
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/pyproject.toml
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/__init__.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/cli.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/py.typed
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/app/__init__.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/auth/__init__.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/auth/models.py
+-rw-r--r--   0        0        0     5019 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/contents/__init__.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/contents/models.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/frontend/__init__.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/jupyterlab/__init__.py
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/kernels/__init__.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/kernels/models.py
+-rw-r--r--   0        0        0     5556 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/lab/__init__.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/login/__init__.py
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/main/__init__.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/nbconvert/__init__.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/resource_usage/__init__.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/retrolab/__init__.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/terminals/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/terminals/models.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/yjs/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 jupyverse-0.1.8/jupyverse_api/jupyverse_api/yjs/models.py
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 jupyverse-0.1.8/notebooks/admin_users.ipynb
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 jupyverse-0.1.8/notebooks/admin_users.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth/MANIFEST.in
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth/README.md
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth/fps_auth/__init__.py
+-rw-r--r--   0        0        0    11596 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth/fps_auth/backends.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth/fps_auth/config.py
+-rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth/fps_auth/db.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth/fps_auth/main.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth/fps_auth/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth/fps_auth/py.typed
+-rw-r--r--   0        0        0     7820 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth/fps_auth/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth_fief/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth_fief/MANIFEST.in
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth_fief/README.md
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth_fief/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth_fief/fps_auth_fief/__init__.py
+-rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth_fief/fps_auth_fief/backend.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth_fief/fps_auth_fief/config.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth_fief/fps_auth_fief/main.py
+-rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/auth_fief/fps_auth_fief/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/contents/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/contents/MANIFEST.in
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/contents/README.md
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/contents/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/contents/fps_contents/__init__.py
+-rw-r--r--   0        0        0     8561 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/contents/fps_contents/fileid.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/contents/fps_contents/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/contents/fps_contents/py.typed
+-rw-r--r--   0        0        0     9082 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/contents/fps_contents/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/frontend/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/frontend/MANIFEST.in
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/frontend/README.md
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/frontend/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/frontend/fps_frontend/__init__.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/frontend/fps_frontend/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/frontend/fps_frontend/py.typed
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/jupyterlab/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/jupyterlab/MANIFEST.in
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/jupyterlab/README.md
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/jupyterlab/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/jupyterlab/fps_jupyterlab/__init__.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/jupyterlab/fps_jupyterlab/index.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/jupyterlab/fps_jupyterlab/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/jupyterlab/fps_jupyterlab/py.typed
+-rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/jupyterlab/fps_jupyterlab/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/kernels/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/kernels/MANIFEST.in
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/kernels/README.md
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/kernels/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/kernels/fps_kernels/__init__.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/kernels/fps_kernels/main.py
+-rw-r--r--   0        0        0    13257 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/kernels/fps_kernels/routes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/kernels/fps_kernels/kernel_driver/__init__.py
+-rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/kernels/fps_kernels/kernel_driver/connect.py
+-rw-r--r--   0        0        0     8632 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/kernels/fps_kernels/kernel_driver/driver.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/kernels/fps_kernels/kernel_driver/kernelspec.py
+-rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/kernels/fps_kernels/kernel_driver/message.py
+-rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/kernels/fps_kernels/kernel_driver/paths.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/kernels/fps_kernels/kernel_server/__init__.py
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/kernels/fps_kernels/kernel_server/message.py
+-rw-r--r--   0        0        0    11591 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/kernels/fps_kernels/kernel_server/server.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/lab/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/lab/MANIFEST.in
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/lab/README.md
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/lab/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/lab/fps_lab/__init__.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/lab/fps_lab/main.py
+-rw-r--r--   0        0        0     7307 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/lab/fps_lab/routes.py
+-rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/lab/fps_lab/static/favicon.ico
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/login/COPYING.md
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/login/MANIFEST.in
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/login/README.md
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/login/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/login/fps_login/__init__.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/login/fps_login/main.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/login/fps_login/routes.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/login/fps_login/static/index.html
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/login/fps_login/static/favicons/favicon-busy-1.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/login/fps_login/static/favicons/favicon-busy-2.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/login/fps_login/static/favicons/favicon-busy-3.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/login/fps_login/static/favicons/favicon-file.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/login/fps_login/static/favicons/favicon-notebook.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/login/fps_login/static/favicons/favicon-terminal.ico
+-rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/login/fps_login/static/favicons/favicon.ico
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/login/fps_login/static/logo/github.svg
+-rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/login/fps_login/static/logo/logo.png
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/login/fps_login/static/style/index.css
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/nbconvert/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/nbconvert/MANIFEST.in
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/nbconvert/README.md
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/nbconvert/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/nbconvert/fps_nbconvert/__init__.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/nbconvert/fps_nbconvert/main.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/nbconvert/fps_nbconvert/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/noauth/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/noauth/MANIFEST.in
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/noauth/README.md
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/noauth/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/noauth/fps_noauth/__init__.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/noauth/fps_noauth/backends.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/noauth/fps_noauth/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/noauth/fps_noauth/py.typed
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/resource_usage/COPYING.md
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/resource_usage/README.md
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/resource_usage/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/resource_usage/fps_resource_usage/__init__.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/resource_usage/fps_resource_usage/main.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/resource_usage/fps_resource_usage/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/retrolab/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/retrolab/MANIFEST.in
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/retrolab/README.md
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/retrolab/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/retrolab/fps_retrolab/__init__.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/retrolab/fps_retrolab/main.py
+-rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/retrolab/fps_retrolab/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/terminals/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/terminals/MANIFEST.in
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/terminals/README.md
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/terminals/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/terminals/fps_terminals/__init__.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/terminals/fps_terminals/main.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/terminals/fps_terminals/routes.py
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/terminals/fps_terminals/server.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/terminals/fps_terminals/win_server.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/webdav/COPYING.md
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/webdav/README.md
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/webdav/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/webdav/fps_webdav/__init__.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/webdav/fps_webdav/config.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/webdav/fps_webdav/main.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/webdav/fps_webdav/routes.py
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/webdav/tests/test_webdav.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/yjs/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/yjs/MANIFEST.in
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/yjs/README.md
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/yjs/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/yjs/fps_yjs/__init__.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/yjs/fps_yjs/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/yjs/fps_yjs/py.typed
+-rw-r--r--   0        0        0    14935 2020-02-02 00:00:00.000000 jupyverse-0.1.8/plugins/yjs/fps_yjs/routes.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 jupyverse-0.1.8/tests/conftest.py
+-rw-r--r--   0        0        0     4485 2020-02-02 00:00:00.000000 jupyverse-0.1.8/tests/test_auth.py
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupyverse-0.1.8/tests/test_contents.py
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 jupyverse-0.1.8/tests/test_kernels.py
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 jupyverse-0.1.8/tests/test_server.py
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 jupyverse-0.1.8/tests/test_settings.py
+-rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 jupyverse-0.1.8/tests/utils.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 jupyverse-0.1.8/tests/data/notebook0.ipynb
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 jupyverse-0.1.8/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.1.8/COPYING.md
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 jupyverse-0.1.8/README.md
+-rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 jupyverse-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 jupyverse-0.1.8/PKG-INFO
```

### Comparing `jupyverse-0.1.6/.pre-commit-config.yaml` & `jupyverse-0.1.8/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -17,11 +17,11 @@
 
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.263
+    rev: v0.0.270
     hooks:
       - id: ruff
         args: ["--fix"]
```

### Comparing `jupyverse-0.1.6/CHANGELOG.md` & `jupyverse-0.1.8/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,50 @@
 # Changes in Jupyverse {#changelog}
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 0.1.8
+
+No merged PRs
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
+## 0.1.7
+
+([Full Changelog](https://github.com/jupyter-server/jupyverse/compare/v0.1.6...d1d54a22429136b87fd45b7540d43937b2e6b695))
+
+### Merged PRs
+
+- Add WebDAV plugin [#312](https://github.com/jupyter-server/jupyverse/pull/312) ([@davidbrochart](https://github.com/davidbrochart))
+- Fix contents for empty directory [#311](https://github.com/jupyter-server/jupyverse/pull/311) ([@davidbrochart](https://github.com/davidbrochart))
+- Replace request with permissions query parameter in GET /api/me [#309](https://github.com/jupyter-server/jupyverse/pull/309) ([@davidbrochart](https://github.com/davidbrochart))
+- Add notebook for user administration [#308](https://github.com/jupyter-server/jupyverse/pull/308) ([@davidbrochart](https://github.com/davidbrochart))
+- Refactor fps_yjs [#307](https://github.com/jupyter-server/jupyverse/pull/307) ([@davidbrochart](https://github.com/davidbrochart))
+- Fix labextensions, move fileid.db to .fileid.db, update to jupyterlab v4 [#304](https://github.com/jupyter-server/jupyverse/pull/304) ([@davidbrochart](https://github.com/davidbrochart))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyter-server/jupyverse/graphs/contributors?from=2023-05-05&to=2023-05-31&type=c))
+
+[@davidbrochart](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyverse+involves%3Adavidbrochart+updated%3A2023-05-05..2023-05-31&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyverse+involves%3Apre-commit-ci+updated%3A2023-05-05..2023-05-31&type=Issues)
+
 ## 0.1.6
 
 ([Full Changelog](https://github.com/jupyter-server/jupyverse/compare/v0.1.5...442f12896cb390ef8346a2fc99e927fa3295421b))
 
 ### Merged PRs
 
 - Update dependencies [#298](https://github.com/jupyter-server/jupyverse/pull/298) ([@davidbrochart](https://github.com/davidbrochart))
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyter-server/jupyverse/graphs/contributors?from=2023-04-29&to=2023-05-05&type=c))
 
 [@davidbrochart](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyverse+involves%3Adavidbrochart+updated%3A2023-04-29..2023-05-05&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyverse+involves%3Apre-commit-ci+updated%3A2023-04-29..2023-05-05&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.1.5
 
 ([Full Changelog](https://github.com/jupyter-server/jupyverse/compare/v0.1.4...bea8fa74efe86fa59ea6054f6e332ffd3d58b23f))
 
 ### Merged PRs
 
 - Update with FastAPI-Users v11 [#296](https://github.com/jupyter-server/jupyverse/pull/296) ([@davidbrochart](https://github.com/davidbrochart))
```

### Comparing `jupyverse-0.1.6/CONTRIBUTING.md` & `jupyverse-0.1.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/config.yaml` & `jupyverse-0.1.8/config.yaml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/mkdocs.yml` & `jupyverse-0.1.8/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/.devcontainer/devcontainer.json` & `jupyverse-0.1.8/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/.github/workflows/check-release.yml` & `jupyverse-0.1.8/.github/workflows/check-release.yml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/.github/workflows/main.yml` & `jupyverse-0.1.8/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/binder/jupyter_notebook_config.py` & `jupyverse-0.1.8/binder/jupyter_notebook_config.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/docs/index.md` & `jupyverse-0.1.8/docs/index.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/docs/install.md` & `jupyverse-0.1.8/docs/install.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/docs/jupyter.svg` & `jupyverse-0.1.8/docs/jupyter.svg`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/docs/plugins/auth.md` & `jupyverse-0.1.8/docs/plugins/auth.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/docs/usage/microservices.md` & `jupyverse-0.1.8/docs/usage/microservices.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/docs/usage/multi_user.md` & `jupyverse-0.1.8/docs/usage/multi_user.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,16 @@
-Jupyverse supports multiple users working collaboratively. Depending on the chosen authentication method, access to the server can be finer-grained. For instance, it is possible to require users to create an account before they can log in, and to give them permissions restricting access to specific resources. It is also possible to let them log in as anonymous users. The authentication method largely depends on the level of security you want.
+Jupyverse supports multiple users working collaboratively. Depending on the chosen authentication method, access to the server can be finer-grained. For instance, it is possible to require users to create an account before they can log in, and to give them permissions restricting access to specific resources. It is also possible to let them log in as anonymous users. The authentication method largely depends on the desired level of security.
 
 ## Collaborative editing
 
-The first thing to do is to allow collaborative editing when launching Jupyverse:
+The first thing to do is to install the Jupyter collaboration package:
+```bash
+pip install jupyter-collaboration
+```
+Jupyverse must then be launched in collaborative mode:
 ```bash
 jupyverse --set frontend.collaborative=true
 ```
 The collaborative mode will handle users through the [auth plugin](../../plugins/auth) you have installed, which will provide user identity.
 
 ## Identity provider
```

### Comparing `jupyverse-0.1.6/docs/usage/single_user.md` & `jupyverse-0.1.8/docs/usage/single_user.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/jupyverse_api/COPYING.md` & `jupyverse-0.1.8/jupyverse_api/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/jupyverse_api/pyproject.toml` & `jupyverse-0.1.8/jupyverse_api/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/jupyverse_api/jupyverse_api/__init__.py` & `jupyverse-0.1.8/jupyverse_api/jupyverse_api/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Dict
 
 from pydantic import BaseModel, Extra
 
 from .app import App
 
 
-__version__ = "0.1.6"
+__version__ = "0.1.8"
 
 
 class Singleton(type):
     _instances: Dict = {}
 
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
@@ -36,7 +36,10 @@
         return self.__class__.__name__
 
     def include_router(self, router, **kwargs):
         self._app._include_router(router, self._type, **kwargs)
 
     def mount(self, path: str, *args, **kwargs) -> None:
         self._app._mount(path, self._type, *args, **kwargs)
+
+    def add_middleware(self, middleware, *args, **kwargs) -> None:
+        self._app.add_middleware(middleware, *args, **kwargs)
```

### Comparing `jupyverse-0.1.6/jupyverse_api/jupyverse_api/cli.py` & `jupyverse-0.1.8/jupyverse_api/jupyverse_api/cli.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/jupyverse_api/jupyverse_api/app/__init__.py` & `jupyverse-0.1.8/jupyverse_api/jupyverse_api/app/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,7 +45,10 @@
             if path in _paths:
                 raise RuntimeError(
                     f"{_type } mounts a path that is already defined in {_router}: {path}"
                 )
         self._router_paths[_type].append(path)
         logger.debug("%s mounted path: %s", _type, path)
         self._app.mount(path, *args, **kwargs)
+
+    def add_middleware(self, middleware, *args, **kwargs) -> None:
+        self._app.add_middleware(middleware, *args, **kwargs)
```

### Comparing `jupyverse-0.1.6/jupyverse_api/jupyverse_api/auth/__init__.py` & `jupyverse-0.1.8/jupyverse_api/jupyverse_api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/jupyverse_api/jupyverse_api/contents/__init__.py` & `jupyverse-0.1.8/jupyverse_api/jupyverse_api/contents/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,20 @@
     async def get_path(self, file_id: str) -> str:
         ...
 
     @abstractmethod
     async def get_id(self, file_path: str) -> str:
         ...
 
+    def watch(self, path: str):
+        ...
+
+    def unwatch(self, path: str, watcher):
+        ...
+
 
 class Contents(Router, ABC):
     def __init__(self, app: App, auth: Auth):
         super().__init__(app=app)
 
         router = APIRouter()
```

### Comparing `jupyverse-0.1.6/jupyverse_api/jupyverse_api/contents/models.py` & `jupyverse-0.1.8/jupyverse_api/jupyverse_api/contents/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 class Content(BaseModel):
     name: str
     path: str
     last_modified: Optional[str]
     created: Optional[str]
-    content: Optional[Union[str, Dict, List[Dict]]]
+    content: Optional[Union[List[Dict], str, Dict]]
     format: Optional[str]
     mimetype: Optional[str]
     size: Optional[int]
     writable: bool
     type: str
```

### Comparing `jupyverse-0.1.6/jupyverse_api/jupyverse_api/jupyterlab/__init__.py` & `jupyverse-0.1.8/jupyverse_api/jupyverse_api/jupyterlab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/jupyverse_api/jupyverse_api/kernels/__init__.py` & `jupyverse-0.1.8/jupyverse_api/jupyverse_api/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/jupyverse_api/jupyverse_api/kernels/models.py` & `jupyverse-0.1.8/jupyverse_api/jupyverse_api/kernels/models.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/jupyverse_api/jupyverse_api/lab/__init__.py` & `jupyverse-0.1.8/jupyverse_api/jupyverse_api/lab/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from ..auth import Auth, User
 from ..app import App
 
 
 class Lab(Router, ABC):
     prefix_dir: Path
     jlab_dir: Path
+    labextensions_dir: Path
     extensions_dir: Path
     redirect_after_root: str
 
     def __init__(self, app: App, auth: Auth, jupyterlab_config: Optional[JupyterLabConfig]):
         super().__init__(app)
 
         self.prefix_dir = Path(sys.prefix)
@@ -32,14 +33,15 @@
             jlab_dev_mode = jupyterlab_config.dev_mode
         else:
             jlab_dev_mode = False
         if jlab_dev_mode:
             self.jlab_dir = Path(jupyterlab_module.__file__).parents[1] / "dev_mode"
         else:
             self.jlab_dir = self.prefix_dir / "share" / "jupyter" / "lab"
+        self.labextensions_dir = self.prefix_dir / "share" / "jupyter" / "labextensions"
         for ext in self.federated_extensions:
             name = ext["name"]
             self.mount(
                 f"/lab/extensions/{name}/static",
                 StaticFiles(directory=self.extensions_dir / name / "static"),
                 name=name,
             )
```

### Comparing `jupyverse-0.1.6/jupyverse_api/jupyverse_api/main/__init__.py` & `jupyverse-0.1.8/jupyverse_api/jupyverse_api/main/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/jupyverse_api/jupyverse_api/nbconvert/__init__.py` & `jupyverse-0.1.8/jupyverse_api/jupyverse_api/nbconvert/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/jupyverse_api/jupyverse_api/resource_usage/__init__.py` & `jupyverse-0.1.8/jupyverse_api/jupyverse_api/resource_usage/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/jupyverse_api/jupyverse_api/retrolab/__init__.py` & `jupyverse-0.1.8/jupyverse_api/jupyverse_api/retrolab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/jupyverse_api/jupyverse_api/terminals/__init__.py` & `jupyverse-0.1.8/jupyverse_api/jupyverse_api/terminals/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/auth/COPYING.md` & `jupyverse-0.1.8/plugins/auth/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/auth/pyproject.toml` & `jupyverse-0.1.8/plugins/auth/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/auth/fps_auth/backends.py` & `jupyverse-0.1.8/plugins/auth/fps_auth/backends.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/auth/fps_auth/config.py` & `jupyverse-0.1.8/plugins/auth/fps_auth/config.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/auth/fps_auth/db.py` & `jupyverse-0.1.8/plugins/auth/fps_auth/db.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,14 +66,17 @@
     userdb_path = jupyter_dir / f"{name}_users.db"
 
     if auth_config.clear_users:
         if userdb_path.is_file():
             userdb_path.unlink()
         if secret_path.is_file():
             secret_path.unlink()
+    if auth_config.mode == "token":
+        if secret_path.is_file():
+            secret_path.unlink()
 
     if not secret_path.is_file():
         secret_path.write_text(secrets.token_hex(32))
 
     secret = secret_path.read_text()
 
     database_url = f"sqlite+aiosqlite:///{userdb_path}"
```

### Comparing `jupyverse-0.1.6/plugins/auth/fps_auth/main.py` & `jupyverse-0.1.8/plugins/auth/fps_auth/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/auth_fief/COPYING.md` & `jupyverse-0.1.8/plugins/auth_fief/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/auth_fief/pyproject.toml` & `jupyverse-0.1.8/plugins/auth_fief/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/auth_fief/fps_auth_fief/backend.py` & `jupyverse-0.1.8/plugins/auth_fief/fps_auth_fief/backend.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/auth_fief/fps_auth_fief/main.py` & `jupyverse-0.1.8/plugins/auth_fief/fps_auth_fief/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/auth_fief/fps_auth_fief/routes.py` & `jupyverse-0.1.8/plugins/auth_fief/fps_auth_fief/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/contents/COPYING.md` & `jupyverse-0.1.8/plugins/contents/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/contents/pyproject.toml` & `jupyverse-0.1.8/plugins/contents/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/contents/fps_contents/fileid.py` & `jupyverse-0.1.8/plugins/contents/fps_contents/fileid.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import asyncio
 import logging
-from typing import Dict, List, Optional
+from typing import Dict, List, Optional, Set
 from uuid import uuid4
 
 import aiosqlite
 from anyio import Path
 from jupyverse_api import Singleton
 from watchfiles import Change, awatch
 
@@ -31,15 +31,15 @@
 
 class FileIdManager(metaclass=Singleton):
     db_path: str
     initialized: asyncio.Event
     watchers: Dict[str, List[Watcher]]
     lock: asyncio.Lock
 
-    def __init__(self, db_path: str = "fileid.db"):
+    def __init__(self, db_path: str = ".fileid.db"):
         self.db_path = db_path
         self.initialized = asyncio.Event()
         self.watchers = {}
         self.watch_files_task = asyncio.create_task(self.watch_files())
         self.stop_watching_files = asyncio.Event()
         self.stopped_watching_files = asyncio.Event()
         self.lock = asyncio.Lock()
@@ -97,16 +97,16 @@
                     )
                 await db.commit()
                 self.initialized.set()
 
         async for changes in awatch(".", stop_event=self.stop_watching_files):
             async with self.lock:
                 async with aiosqlite.connect(self.db_path) as db:
-                    deleted_paths = []
-                    added_paths = []
+                    deleted_paths = set()
+                    added_paths = set()
                     for change, changed_path in changes:
                         # get relative path
                         changed_path = Path(changed_path).relative_to(await Path().absolute())
                         changed_path_str = str(changed_path)
 
                         if change == Change.deleted:
                             logger.debug("File %s was deleted", changed_path_str)
@@ -143,24 +143,26 @@
                                     continue
                             mtime = (await changed_path.stat()).st_mtime
                             await db.execute(
                                 "UPDATE fileids SET mtime = ? WHERE path = ?",
                                 (mtime, changed_path_str),
                             )
 
-                    for path in deleted_paths + added_paths:
+                    for path in deleted_paths - added_paths:
+                        logger.debug("Unindexing file %s ", path)
                         await db.execute("DELETE FROM fileids WHERE path = ?", (path,))
                     await db.commit()
 
             for change in changes:
                 changed_path = change[1]
                 # get relative path
-                changed_path = str(Path(changed_path).relative_to(await Path().absolute()))
-                for watcher in self.watchers.get(changed_path, []):
-                    watcher.notify(change)
+                relative_changed_path = str(Path(changed_path).relative_to(await Path().absolute()))
+                relative_change = (change[0], relative_changed_path)
+                for watcher in self.watchers.get(relative_changed_path, []):
+                    watcher.notify(relative_change)
 
         self.stopped_watching_files.set()
 
     def watch(self, path: str) -> Watcher:
         watcher = Watcher(path)
         self.watchers.setdefault(path, []).append(watcher)
         return watcher
@@ -180,15 +182,15 @@
         mtime = (await Path(path).stat()).st_mtime
     except FileNotFoundError:
         return None
     return mtime
 
 
 async def maybe_rename(
-    db, changed_path: str, changed_paths: List[str], other_paths: List[str], is_added_path
+    db, changed_path: str, changed_paths: Set[str], other_paths: Set[str], is_added_path: bool
 ) -> None:
     # check if the same file was added/deleted, this would be a rename
     db_or_fs1, db_or_fs2 = db, None
     if is_added_path:
         db_or_fs1, db_or_fs2 = db_or_fs2, db_or_fs1
     mtime1 = await get_mtime(changed_path, db_or_fs1)
     if mtime1 is None:
@@ -200,8 +202,8 @@
             path1, path2 = changed_path, other_path
             if is_added_path:
                 path1, path2 = path2, path1
             logger.debug("File %s was renamed to %s", path1, path2)
             await db.execute("UPDATE fileids SET path = ? WHERE path = ?", (path2, path1))
             other_paths.remove(other_path)
             return
-    changed_paths.append(changed_path)
+    changed_paths.add(changed_path)
```

### Comparing `jupyverse-0.1.6/plugins/contents/fps_contents/routes.py` & `jupyverse-0.1.8/plugins/contents/fps_contents/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/frontend/COPYING.md` & `jupyverse-0.1.8/plugins/frontend/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/frontend/pyproject.toml` & `jupyverse-0.1.8/plugins/frontend/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/jupyterlab/COPYING.md` & `jupyverse-0.1.8/plugins/jupyterlab/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/jupyterlab/pyproject.toml` & `jupyverse-0.1.8/plugins/jupyterlab/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "fps_jupyterlab"
 description = "An FPS plugin for the JupyterLab API"
 keywords = [ "jupyter", "server", "fastapi", "plugins" ]
 requires-python = ">=3.8"
 dependencies = [
-  "jupyterlab >=4.0.0rc0,<5",
+  "jupyterlab >=4.0.0,<5",
   "jupyverse-api >=0.1.2,<1",
 ]
 dynamic = [ "version",]
 [[project.authors]]
 name = "Jupyter Development Team"
 email = "jupyter@googlegroups.com"
```

### Comparing `jupyverse-0.1.6/plugins/jupyterlab/fps_jupyterlab/index.py` & `jupyverse-0.1.8/plugins/jupyterlab/fps_jupyterlab/index.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/jupyterlab/fps_jupyterlab/main.py` & `jupyverse-0.1.8/plugins/jupyterlab/fps_jupyterlab/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/jupyterlab/fps_jupyterlab/routes.py` & `jupyverse-0.1.8/plugins/jupyterlab/fps_jupyterlab/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/kernels/COPYING.md` & `jupyverse-0.1.8/plugins/kernels/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/kernels/pyproject.toml` & `jupyverse-0.1.8/plugins/kernels/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/kernels/fps_kernels/main.py` & `jupyverse-0.1.8/plugins/kernels/fps_kernels/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 import asyncio
-import logging
 from collections.abc import AsyncGenerator
 from pathlib import Path
 from typing import Optional
 
 from asphalt.core import Component, Context, context_teardown
 
 from jupyverse_api.auth import Auth
@@ -12,17 +11,14 @@
 from jupyverse_api.kernels import Kernels, KernelsConfig
 from jupyverse_api.yjs import Yjs
 from jupyverse_api.app import App
 
 from .routes import _Kernels
 
 
-logger = logging.getLogger("kernels")
-
-
 class KernelsComponent(Component):
     def __init__(self, **kwargs):
         self.kernels_config = KernelsConfig(**kwargs)
 
     @context_teardown
     async def start(
         self,
```

### Comparing `jupyverse-0.1.6/plugins/kernels/fps_kernels/routes.py` & `jupyverse-0.1.8/plugins/kernels/fps_kernels/routes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import logging
 import uuid
 from http import HTTPStatus
 from pathlib import Path
 from typing import Dict, List, Optional, Set, Tuple
 
 from fastapi import HTTPException, Response
 from fastapi.responses import FileResponse
@@ -20,14 +21,17 @@
 from .kernel_server.server import (
     AcceptedWebSocket,
     KernelServer,
     kernels,
 )
 
 
+logger = logging.getLogger("kernels")
+
+
 class _Kernels(Kernels):
     def __init__(
         self,
         app: App,
         kernels_config: KernelsConfig,
         auth: Auth,
         frontend_config: FrontendConfig,
@@ -142,17 +146,22 @@
         user: User,
     ):
         create_session = CreateSession(**(await request.json()))
         kernel_id = create_session.kernel.id
         kernel_name = create_session.kernel.name
         if kernel_name is not None:
             # launch a new ("internal") kernel
+            kernel_cwd = Path(create_session.path).parent
+            while True:
+                if kernel_cwd.is_dir():
+                    break
+                kernel_cwd = kernel_cwd.parent
             kernel_server = KernelServer(
                 kernelspec_path=Path(find_kernelspec(kernel_name)).as_posix(),
-                kernel_cwd=str(Path(create_session.path).parent),
+                kernel_cwd=str(kernel_cwd),
             )
             kernel_id = str(uuid.uuid4())
             kernels[kernel_id] = {"name": kernel_name, "server": kernel_server, "driver": None}
             await kernel_server.start()
         elif kernel_id is not None:
             # external kernel
             kernel_name = kernels[kernel_id]["name"]
@@ -227,15 +236,15 @@
     ):
         if self.yjs is None:
             raise RuntimeError("Cannot execute without a Yjs plugin.")
 
         r = await request.json()
         execution = Execution(**r)
         if kernel_id in kernels:
-            ynotebook = self.yjs.websocket_server.get_room(execution.document_id).document
+            ynotebook = self.yjs.get_document(execution.document_id)
             cell = ynotebook.get_cell(execution.cell_idx)
             cell["outputs"] = []
 
             kernel = kernels[kernel_id]
             if not kernel["driver"]:
                 kernel["driver"] = driver = KernelDriver(
                     kernelspec_path=Path(find_kernelspec(kernel["name"])).as_posix(),
```

### Comparing `jupyverse-0.1.6/plugins/kernels/fps_kernels/kernel_driver/connect.py` & `jupyverse-0.1.8/plugins/kernels/fps_kernels/kernel_driver/connect.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/kernels/fps_kernels/kernel_driver/driver.py` & `jupyverse-0.1.8/plugins/kernels/fps_kernels/kernel_driver/driver.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/kernels/fps_kernels/kernel_driver/kernelspec.py` & `jupyverse-0.1.8/plugins/kernels/fps_kernels/kernel_driver/kernelspec.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/kernels/fps_kernels/kernel_driver/message.py` & `jupyverse-0.1.8/plugins/kernels/fps_kernels/kernel_driver/message.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/kernels/fps_kernels/kernel_driver/paths.py` & `jupyverse-0.1.8/plugins/kernels/fps_kernels/kernel_driver/paths.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/kernels/fps_kernels/kernel_server/message.py` & `jupyverse-0.1.8/plugins/kernels/fps_kernels/kernel_server/message.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/kernels/fps_kernels/kernel_server/server.py` & `jupyverse-0.1.8/plugins/kernels/fps_kernels/kernel_server/server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/lab/COPYING.md` & `jupyverse-0.1.8/plugins/lab/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/lab/pyproject.toml` & `jupyverse-0.1.8/plugins/lab/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/lab/fps_lab/main.py` & `jupyverse-0.1.8/plugins/lab/fps_lab/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/lab/fps_lab/routes.py` & `jupyverse-0.1.8/plugins/lab/fps_lab/routes.py`

 * *Files 12% similar despite different names*

```diff
@@ -154,39 +154,47 @@
     ):
         settings = json.loads(user.settings)
         settings[f"{name0}:{name1}"] = await request.json()
         await user_update({"settings": json.dumps(settings)})
         return Response(status_code=HTTPStatus.NO_CONTENT.value)
 
     async def get_settings(self, user: User):
-        with open(self.jlab_dir / "static" / "package.json") as f:
-            package = json.load(f)
         if user:
             user_settings = json.loads(user.settings)
         else:
             user_settings = {}
         settings = []
-        for path in (self.jlab_dir / "schemas" / "@jupyterlab").glob("*/*.json"):
-            with open(path) as f:
-                schema = json.load(f)
-            key = f"{path.parent.name}:{path.stem}"
-            setting = {
-                "id": f"@jupyterlab/{key}",
-                "schema": schema,
-                "version": package["version"],
-                "raw": "{}",
-                "settings": {},
-                "warning": None,
-                "last_modified": None,
-                "created": None,
-            }
-            if key in user_settings:
-                setting.update(user_settings[key])
-                setting["settings"] = json5.loads(user_settings[key]["raw"])
-            settings.append(setting)
+        schemas = [self.jlab_dir / "schemas"]
+        for d1 in self.labextensions_dir.iterdir():
+            if (d1 / "schemas").exists():
+                schemas.append(d1 / "schemas")
+            for d2 in d1.iterdir():
+                if (d2 / "schemas").exists():
+                    schemas.append(d2 / "schemas")
+        for s in schemas:
+            for d1 in s.iterdir():
+                for d2 in d1.iterdir():
+                    package = json.loads((d2 / "package.json.orig").read_text())
+                    for path in [p for p in d2.iterdir() if p.suffix == ".json"]:
+                        schema = json.loads(path.read_text())
+                        key = f"{path.parent.name}:{path.stem}"
+                        setting = {
+                            "id": f"{d1.name}/{key}",
+                            "schema": schema,
+                            "version": package["version"],
+                            "raw": "{}",
+                            "settings": {},
+                            "warning": None,
+                            "last_modified": None,
+                            "created": None,
+                        }
+                        if key in user_settings:
+                            setting.update(user_settings[key])
+                            setting["settings"] = json5.loads(user_settings[key]["raw"])
+                        settings.append(setting)
         return {"settings": settings}
 
     def get_federated_extensions(self, extensions_dir: Path) -> Tuple[List, List]:
         federated_extensions = []
         disabled_extensions = []
 
         for path in glob(os.path.join(extensions_dir, "**", "package.json"), recursive=True):
```

### Comparing `jupyverse-0.1.6/plugins/lab/fps_lab/static/favicon.ico` & `jupyverse-0.1.8/plugins/lab/fps_lab/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/login/COPYING.md` & `jupyverse-0.1.8/plugins/login/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/login/pyproject.toml` & `jupyverse-0.1.8/plugins/login/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/login/fps_login/routes.py` & `jupyverse-0.1.8/plugins/login/fps_login/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/login/fps_login/static/index.html` & `jupyverse-0.1.8/plugins/login/fps_login/static/index.html`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/login/fps_login/static/favicons/favicon-busy-1.ico` & `jupyverse-0.1.8/plugins/login/fps_login/static/favicons/favicon-busy-1.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/login/fps_login/static/favicons/favicon-busy-2.ico` & `jupyverse-0.1.8/plugins/login/fps_login/static/favicons/favicon-busy-2.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/login/fps_login/static/favicons/favicon-busy-3.ico` & `jupyverse-0.1.8/plugins/login/fps_login/static/favicons/favicon-busy-3.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/login/fps_login/static/favicons/favicon-file.ico` & `jupyverse-0.1.8/plugins/login/fps_login/static/favicons/favicon-file.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/login/fps_login/static/favicons/favicon-notebook.ico` & `jupyverse-0.1.8/plugins/login/fps_login/static/favicons/favicon-notebook.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/login/fps_login/static/favicons/favicon-terminal.ico` & `jupyverse-0.1.8/plugins/login/fps_login/static/favicons/favicon-terminal.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/login/fps_login/static/favicons/favicon.ico` & `jupyverse-0.1.8/plugins/login/fps_login/static/favicons/favicon.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/login/fps_login/static/logo/github.svg` & `jupyverse-0.1.8/plugins/login/fps_login/static/logo/github.svg`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/login/fps_login/static/logo/logo.png` & `jupyverse-0.1.8/plugins/login/fps_login/static/logo/logo.png`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/login/fps_login/static/style/index.css` & `jupyverse-0.1.8/plugins/login/fps_login/static/style/index.css`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/nbconvert/COPYING.md` & `jupyverse-0.1.8/plugins/nbconvert/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/nbconvert/pyproject.toml` & `jupyverse-0.1.8/plugins/nbconvert/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/nbconvert/fps_nbconvert/routes.py` & `jupyverse-0.1.8/plugins/nbconvert/fps_nbconvert/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/noauth/COPYING.md` & `jupyverse-0.1.8/plugins/noauth/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/noauth/pyproject.toml` & `jupyverse-0.1.8/plugins/noauth/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/noauth/fps_noauth/backends.py` & `jupyverse-0.1.8/plugins/noauth/fps_noauth/backends.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/resource_usage/COPYING.md` & `jupyverse-0.1.8/plugins/resource_usage/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/resource_usage/pyproject.toml` & `jupyverse-0.1.8/plugins/resource_usage/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/resource_usage/fps_resource_usage/main.py` & `jupyverse-0.1.8/plugins/resource_usage/fps_resource_usage/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/resource_usage/fps_resource_usage/routes.py` & `jupyverse-0.1.8/plugins/resource_usage/fps_resource_usage/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/retrolab/COPYING.md` & `jupyverse-0.1.8/plugins/retrolab/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/retrolab/pyproject.toml` & `jupyverse-0.1.8/plugins/retrolab/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/retrolab/fps_retrolab/main.py` & `jupyverse-0.1.8/plugins/retrolab/fps_retrolab/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/retrolab/fps_retrolab/routes.py` & `jupyverse-0.1.8/plugins/retrolab/fps_retrolab/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/terminals/COPYING.md` & `jupyverse-0.1.8/plugins/terminals/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/terminals/pyproject.toml` & `jupyverse-0.1.8/plugins/terminals/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/terminals/fps_terminals/main.py` & `jupyverse-0.1.8/plugins/terminals/fps_terminals/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/terminals/fps_terminals/routes.py` & `jupyverse-0.1.8/plugins/terminals/fps_terminals/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/terminals/fps_terminals/server.py` & `jupyverse-0.1.8/plugins/terminals/fps_terminals/server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/terminals/fps_terminals/win_server.py` & `jupyverse-0.1.8/plugins/terminals/fps_terminals/win_server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/yjs/COPYING.md` & `jupyverse-0.1.8/plugins/webdav/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/yjs/pyproject.toml` & `jupyverse-0.1.8/plugins/yjs/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/plugins/yjs/fps_yjs/main.py` & `jupyverse-0.1.8/plugins/yjs/fps_yjs/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+
 from collections.abc import AsyncGenerator
 from typing import Optional
 
 from asphalt.core import Component, Context, context_teardown
 from jupyverse_api.app import App
 from jupyverse_api.auth import Auth
 from jupyverse_api.contents import Contents
@@ -25,9 +26,10 @@
         ctx.add_resource(yjs, types=Yjs)
 
         # start indexing in the background
         contents.file_id_manager
 
         yield
 
+        yjs.room_manager.stop()
         contents.file_id_manager.stop_watching_files.set()
         await contents.file_id_manager.stopped_watching_files.wait()
```

### Comparing `jupyverse-0.1.6/plugins/yjs/fps_yjs/routes.py` & `jupyverse-0.1.8/plugins/yjs/fps_yjs/routes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,113 +1,106 @@
+from __future__ import annotations
+
 import asyncio
+import logging
 from datetime import datetime
-from pathlib import Path
-from typing import Optional, Tuple, cast
+from functools import partial
+from typing import Dict
 from uuid import uuid4
 
 from fastapi import (
     HTTPException,
     Request,
     Response,
     WebSocketDisconnect,
     status,
 )
-from jupyter_ydoc import ydocs as YDOCS  # type: ignore
+from jupyter_ydoc import ydocs as YDOCS
+from jupyter_ydoc.ybasedoc import YBaseDoc
 from jupyverse_api.app import App
 from jupyverse_api.auth import Auth, User
 from jupyverse_api.contents import Contents
 from jupyverse_api.yjs import Yjs
 from jupyverse_api.yjs.models import CreateDocumentSession
+from websockets.exceptions import ConnectionClosedOK
 from ypy_websocket.websocket_server import WebsocketServer, YRoom
-from ypy_websocket.ystore import BaseYStore, SQLiteYStore, YDocNotFound
+from ypy_websocket.ystore import SQLiteYStore, YDocNotFound
 from ypy_websocket.yutils import YMessageType, YSyncMessageType
 
 YFILE = YDOCS["file"]
 AWARENESS = 1
-RENAME_SESSION = 127
 SERVER_SESSION = uuid4().hex
+logger = logging.getLogger("yjs")
 
 
 class JupyterSQLiteYStore(SQLiteYStore):
-    db_path = ".jupyter_ystore.db"
+    db_path = ".jupyter_ystore.db"  # FIXME: pass in config
 
 
 class _Yjs(Yjs):
     def __init__(
         self,
         app: App,
         auth: Auth,
         contents: Contents,
     ) -> None:
         super().__init__(app=app, auth=auth)
         self.contents = contents
-        self.websocket_server = YDocWebSocketHandler.websocket_server
-
-    async def serve_room(self, websocket_permissions, path):
-        if websocket_permissions is None:
-            return
-        websocket, permissions = websocket_permissions
-        await websocket.accept()
-        socket = YDocWebSocketHandler(
-            WebsocketAdapter(websocket, path), path, permissions, self.contents
-        )
-        await socket.serve()
-
-    async def yjs_websocket(
-        self,
-        path,
-        websocket_permissions,
-    ):
-        await self.serve_room(websocket_permissions, path)
+        self.room_manager = RoomManager(contents)
 
     async def collaboration_room_websocket(
         self,
         path,
         websocket_permissions,
     ):
-        await self.serve_room(websocket_permissions, path)
+        if websocket_permissions is None:
+            return
+        websocket, permissions = websocket_permissions
+        await websocket.accept()
+        ypy_websocket = YpyWebsocket(websocket, path)
+        await self.room_manager.serve(ypy_websocket, permissions)
 
     async def create_roomid(
         self,
         path,
         request: Request,
         response: Response,
         user: User,
     ):
         # we need to process the request manually
         # see https://github.com/tiangolo/fastapi/issues/3373#issuecomment-1306003451
         create_document_session = CreateDocumentSession(**(await request.json()))
         idx = await self.contents.file_id_manager.get_id(path)
+        res = {
+            "format": create_document_session.format,
+            "type": create_document_session.type,
+            "sessionId": SERVER_SESSION,
+        }
         if idx is not None:
-            return {
-                "format": create_document_session.format,
-                "type": create_document_session.type,
-                "fileId": idx,
-                "sessionId": SERVER_SESSION,
-            }
+            res["fileId"] = idx
+            return res
 
         idx = await self.contents.file_id_manager.index(path)
         if idx is None:
             raise HTTPException(status_code=404, detail=f"File {path} does not exist")
 
         response.status_code = status.HTTP_201_CREATED
-        return {
-            "format": create_document_session.format,
-            "type": create_document_session.type,
-            "fileId": idx,
-            "sessionId": SERVER_SESSION,
-        }
+        res["fileId"] = idx
+        return res
+
+    def get_document(self, document_id: str) -> YBaseDoc:
+        return self.room_manager.documents[document_id]
 
 
 def to_datetime(iso_date: str) -> datetime:
     return datetime.fromisoformat(iso_date.rstrip("Z"))
 
 
-class WebsocketAdapter:
-    """An adapter to make a Starlette's WebSocket look like a ypy-websocket's WebSocket"""
+class YpyWebsocket:
+    """An wrapper to make a Starlette's WebSocket look like a ypy-websocket's WebSocket"""
 
     def __init__(self, websocket, path: str):
         self._websocket = websocket
         self._path = path
 
     @property
     def path(self) -> str:
@@ -124,232 +117,250 @@
         try:
             message = await self._websocket.receive_bytes()
         except WebSocketDisconnect:
             raise StopAsyncIteration()
         return message
 
     async def send(self, message):
-        await self._websocket.send_bytes(message)
+        try:
+            await self._websocket.send_bytes(message)
+        except ConnectionClosedOK:
+            return
 
     async def recv(self):
         return await self._websocket.receive_bytes()
 
 
-class DocumentRoom(YRoom):
-    """A Y room for a possibly stored document (e.g. a notebook)."""
-
-    is_transient = False
-
-    def __init__(self, type: str, ystore: BaseYStore):
-        super().__init__(ready=False, ystore=ystore)
-        self.type = type
-        self.cleaner = None
-        self.watcher = None
-        self.document = YDOCS.get(type, YFILE)(self.ydoc)
-
-
-class TransientRoom(YRoom):
-    """A Y room for sharing state (e.g. awareness)."""
-
-    is_transient = True
-
+class RoomManager:
+    contents: Contents
+    documents: Dict[str, YBaseDoc]
+    watchers: Dict[str, asyncio.Task]
+    savers: Dict[str, asyncio.Task]
+    cleaners: Dict[YRoom, asyncio.Task]
+    last_modified: Dict[str, datetime]
+    websocket_server: JupyterWebsocketServer
+    lock: asyncio.Lock
 
-class JupyterWebsocketServer(WebsocketServer):
-    def get_room(self, path: str) -> YRoom:
-        if path not in self.rooms.keys():
-            if path.count(":") >= 2:
-                # it is a stored document (e.g. a notebook)
-                file_format, file_type, file_path = path.split(":", 2)
-                p = Path(file_path)
-                updates_file_path = (p.parent / f".{file_type}:{p.name}.y").as_posix()
-                ystore = JupyterSQLiteYStore(path=updates_file_path)  # FIXME: pass in config
-                self.rooms[path] = DocumentRoom(file_type, ystore)
-            else:
-                # it is a transient document (e.g. awareness)
-                self.rooms[path] = TransientRoom()
-        return self.rooms[path]
-
-
-class YDocWebSocketHandler:
-    saving_document: Optional[asyncio.Task]
-    websocket_server = JupyterWebsocketServer(rooms_ready=False, auto_clean_rooms=False)
-
-    def __init__(self, websocket, path, permissions, contents: Contents):
-        self.websocket = websocket
+    def __init__(self, contents: Contents):
         self.contents = contents
-        self.can_write = permissions is None or "write" in permissions.get("yjs", [])
+        self.documents = {}  # a dictionary of room_name:document
+        self.watchers = {}  # a dictionary of file_id:task
+        self.savers = {}  # a dictionary of file_id:task
+        self.cleaners = {}  # a dictionary of room:task
+        self.last_modified = {}  # a dictionary of file_id:last_modification_date
+        self.websocket_server = JupyterWebsocketServer(rooms_ready=False, auto_clean_rooms=False)
         self.lock = asyncio.Lock()
-        self.room = self.websocket_server.get_room(self.websocket.path)
-        self.set_file_info(path)
 
-    async def get_file_info(self) -> Tuple[str, str, str]:
-        room_name = self.websocket_server.get_room_name(self.room)
-        file_format, file_type, file_id = room_name.split(":", 2)
-        file_path = await self.contents.file_id_manager.get_path(file_id)
-        room = cast(DocumentRoom, self.room)
-        if file_path is None:
-            raise RuntimeError(f"File {room.document.path} cannot be found anymore")
-        if file_path != room.document.path:
-            room.document.path = file_path
-        return file_format, file_type, file_path
-
-    def set_file_info(self, value: str) -> None:
-        self.websocket_server.rename_room(value, from_room=self.room)
-        self.websocket.path = value
-
-    async def serve(self):
-        self.set_file_info(self.websocket.path)
-        self.saving_document = None
-        self.room.on_message = self.on_message
-
-        # cancel the deletion of the room if it was scheduled
-        if not self.room.is_transient and self.room.cleaner is not None:
-            self.room.cleaner.cancel()
-
-        if not self.room.is_transient and not self.room.ready:
-            file_format, file_type, file_path = await self.get_file_info()
-            is_notebook = file_type == "notebook"
-            model = await self.contents.read_content(file_path, True, as_json=is_notebook)
-            self.last_modified = to_datetime(model.last_modified)
-            # check again if ready, because loading the file is async
-            if not self.room.ready:
-                # try to apply Y updates from the YStore for this document
-                try:
-                    await self.room.ystore.apply_updates(self.room.ydoc)
-                    read_from_source = False
-                except YDocNotFound:
-                    # YDoc not found in the YStore, create the document from
-                    # the source file (no change history)
-                    read_from_source = True
-                if not read_from_source:
-                    # if YStore updates and source file are out-of-sync, resync updates
-                    # with source
-                    if self.room.document.source != model.content:
+    def stop(self):
+        for watcher in self.watchers.values():
+            watcher.cancel()
+        for saver in self.savers.values():
+            saver.cancel()
+        for cleaner in self.cleaners.values():
+            cleaner.cancel()
+
+    async def serve(self, websocket: YpyWebsocket, permissions) -> None:
+        room = self.websocket_server.get_room(websocket.path)
+        can_write = permissions is None or "write" in permissions.get("yjs", [])
+        room.on_message = partial(self.filter_message, can_write)
+        is_stored_document = websocket.path.count(":") >= 2
+        if is_stored_document:
+            assert room.ystore is not None
+            file_format, file_type, file_id = websocket.path.split(":", 2)
+            if room in self.cleaners:
+                # cleaning the room was scheduled because there was no client left
+                # cancel that since there is a new client
+                self.cleaners[room].cancel()
+            if not room.ready:
+                file_path = await self.contents.file_id_manager.get_path(file_id)
+                logger.info(f"Opening collaboration room: {websocket.path} ({file_path})")
+                document = YDOCS.get(file_type, YFILE)(room.ydoc)
+                self.documents[websocket.path] = document
+                is_notebook = file_type == "notebook"
+                async with self.lock:
+                    model = await self.contents.read_content(file_path, True, as_json=is_notebook)
+                assert model.last_modified is not None
+                self.last_modified[file_id] = to_datetime(model.last_modified)
+                if not room.ready:
+                    # try to apply Y updates from the YStore for this document
+                    try:
+                        await room.ystore.apply_updates(room.ydoc)
+                        read_from_source = False
+                    except YDocNotFound:
+                        # YDoc not found in the YStore, create the document from
+                        # the source file (no change history)
                         read_from_source = True
-                if read_from_source:
-                    self.room.document.source = model.content
-                    await self.room.ystore.encode_state_as_update(self.room.ydoc)
-
-                self.room.document.dirty = False
-                self.room.ready = True
-                self.room.watcher = asyncio.create_task(self.watch_file())
-                # save the document when changed
-                self.room.document.observe(self.on_document_change)
+                    if not read_from_source:
+                        # if YStore updates and source file are out-of-sync, resync updates
+                        # with source
+                        if document.source != model.content:
+                            read_from_source = True
+                    if read_from_source:
+                        document.source = model.content
+                        await room.ystore.encode_state_as_update(room.ydoc)
+
+                    document.dirty = False
+                    room.ready = True
+                    # save the document to file when changed
+                    document.observe(partial(self.on_document_change, file_id, file_type, document))
+                    # update the document when file changes
+                    if file_id not in self.watchers:
+                        self.watchers[file_id] = asyncio.create_task(
+                            self.watch_file(file_type, file_id, document)
+                        )
 
-        await self.websocket_server.serve(self.websocket)
-        if not self.room.is_transient and not self.room.clients:
+        await self.websocket_server.serve(websocket)
+
+        if is_stored_document and not room.clients:
             # no client in this room after we disconnect
-            # keep the document for a while in case someone reconnects
-            self.room.cleaner = asyncio.create_task(self.clean_room())
+            self.cleaners[room] = asyncio.create_task(self.maybe_clean_room(room, websocket.path))
 
-    async def on_message(self, message: bytes) -> bool:
+    async def filter_message(self, can_write: bool, message: bytes) -> bool:
         """
         Called whenever a message is received, before forwarding it to other clients.
 
-        :param message: received message
+        :param can_write: True if updating the document is permitted, False otherwise.
+        :param message: received message.
         :returns: True if the message must be discarded, False otherwise (default: False).
         """
         skip = False
         byte = message[0]
         msg = message[1:]
-        if byte == RENAME_SESSION:
-            # The client moved the document to a different location. After receiving this
-            # message, we make the current document available under a different url.
-            # The other clients are automatically notified of this change because
-            # the path is shared through the Yjs document as well.
-            new_room_name = msg.decode("utf-8")
-            self.set_file_info(new_room_name)
-            self.websocket_server.rename_room(new_room_name, from_room=self.room)
-            # send rename acknowledge
-            await self.websocket.send(bytes([RENAME_SESSION, 1]))
-        elif byte == AWARENESS:
+        if byte == AWARENESS:
             # changes = self.room.awareness.get_changes(msg)
             # # filter out message depending on changes
             # skip = True
             pass
         elif byte == YMessageType.SYNC:
-            if not self.can_write and msg[0] == YSyncMessageType.SYNC_UPDATE:
+            if not can_write and msg[0] == YSyncMessageType.SYNC_UPDATE:
                 skip = True
         else:
             skip = True
         return skip
 
-    async def watch_file(self):
-        file_format, file_type, file_path = await self.get_file_info()
+    async def get_file_path(self, file_id: str, document) -> str | None:
+        file_path = await self.contents.file_id_manager.get_path(file_id)
+        if file_path is None:
+            return
+        if file_path != document.path:
+            document.path = file_path
+        return file_path
+
+    async def watch_file(self, file_type: str, file_id: str, document: YBaseDoc) -> None:
+        file_path = await self.get_file_path(file_id, document)
+        assert file_path is not None
+        logger.debug(f"Watching file: {file_path}")
         while True:
             watcher = self.contents.file_id_manager.watch(file_path)
             async for changes in watcher:
-                file_format, file_type, new_file_path = await self.get_file_info()
+                new_file_path = await self.get_file_path(file_id, document)
+                if new_file_path is None:
+                    continue
                 if new_file_path != file_path:
                     # file was renamed
                     self.contents.file_id_manager.unwatch(file_path, watcher)
                     file_path = new_file_path
-                    break
-                await self.maybe_load_document()
+                    # break
+                await self.maybe_load_file(file_type, file_path, file_id)
 
-    async def maybe_load_document(self):
-        file_format, file_type, file_path = await self.get_file_info()
+    async def maybe_load_file(self, file_type: str, file_path: str, file_id: str) -> None:
         async with self.lock:
             model = await self.contents.read_content(file_path, False)
         # do nothing if the file was saved by us
-        if self.last_modified < to_datetime(model.last_modified):
+        assert model.last_modified is not None
+        if self.last_modified[file_id] < to_datetime(model.last_modified):
+            # the file was not saved by us, update the shared document(s)
             is_notebook = file_type == "notebook"
-            model = await self.contents.read_content(file_path, True, as_json=is_notebook)
-            self.room.document.source = model.content
-            self.last_modified = to_datetime(model.last_modified)
-
-    async def clean_room(self) -> None:
-        await asyncio.sleep(60)  # FIXME: pass in config
-        room = cast(DocumentRoom, self.room)
-        if room.watcher:
-            room.watcher.cancel()
-        room.document.unobserve()
-        self.websocket_server.delete_room(room=room)
+            async with self.lock:
+                model = await self.contents.read_content(file_path, True, as_json=is_notebook)
+            assert model.last_modified is not None
+            documents = [v for k, v in self.documents.items() if k.split(":", 2)[2] == file_id]
+            for document in documents:
+                document.source = model.content
+            self.last_modified[file_id] = to_datetime(model.last_modified)
 
-    def on_document_change(self, target, event):
+    def on_document_change(
+        self, file_id: str, file_type: str, document: YBaseDoc, target, event
+    ) -> None:
         if target == "state" and "dirty" in event.keys:
             dirty = event.keys["dirty"]["newValue"]
             if not dirty:
                 # we cleared the dirty flag, nothing to save
                 return
         # unobserve and observe again because the structure of the document may have changed
         # e.g. a new cell added to a notebook
-        self.room.document.unobserve()
-        self.room.document.observe(self.on_document_change)
-        if self.saving_document is not None and not self.saving_document.done():
-            # the document is being saved, cancel that
-            self.saving_document.cancel()
-            self.saving_document = None
-        self.saving_document = asyncio.create_task(self.maybe_save_document())
+        document.unobserve()
+        document.observe(partial(self.on_document_change, file_id, file_type, document))
+        if file_id in self.savers:
+            self.savers[file_id].cancel()
+        self.savers[file_id] = asyncio.create_task(
+            self.maybe_save_document(file_id, file_type, document)
+        )
 
-    async def maybe_save_document(self):
+    async def maybe_save_document(self, file_id: str, file_type: str, document: YBaseDoc) -> None:
         # save after 1 second of inactivity to prevent too frequent saving
-        await asyncio.sleep(1)
+        await asyncio.sleep(1)  # FIXME: pass in config
         # if the room cannot be found, don't save
         try:
-            file_format, file_type, file_path = await self.get_file_info()
-        except Exception:
+            file_path = await self.get_file_path(file_id, document)
+        except BaseException:
             return
+        assert file_path is not None
         is_notebook = file_type == "notebook"
         async with self.lock:
             model = await self.contents.read_content(file_path, True, as_json=is_notebook)
-        if self.last_modified < to_datetime(model.last_modified):
+        assert model.last_modified is not None
+        if self.last_modified[file_id] < to_datetime(model.last_modified):
             # file changed on disk, let's revert
-            self.room.document.source = model.content
-            self.last_modified = to_datetime(model.last_modified)
+            document.source = model.content
+            self.last_modified[file_id] = to_datetime(model.last_modified)
             return
-        if model.content != self.room.document.source:
+        if model.content != document.source:
             # don't save if not needed
             # this also prevents the dirty flag from bouncing between windows of
             # the same document opened as different types (e.g. notebook/text editor)
             format = "json" if file_type == "notebook" else "text"
             content = {
-                "content": self.room.document.source,
+                "content": document.source,
                 "format": format,
                 "path": file_path,
                 "type": file_type,
             }
             async with self.lock:
                 await self.contents.write_content(content)
                 model = await self.contents.read_content(file_path, False)
-                self.last_modified = to_datetime(model.last_modified)
-        self.room.document.dirty = False
+            assert model.last_modified is not None
+            self.last_modified[file_id] = to_datetime(model.last_modified)
+        document.dirty = False
+        # we're done saving, remove the saver
+        del self.savers[file_id]
+
+    async def maybe_clean_room(self, room, ws_path: str) -> None:
+        file_id = ws_path.split(":", 2)[2]
+        # keep the document for a while in case someone reconnects
+        await asyncio.sleep(60)  # FIXME: pass in config
+        document = self.documents[ws_path]
+        document.unobserve()
+        del self.documents[ws_path]
+        documents = [v for k, v in self.documents.items() if k.split(":", 2)[2] == file_id]
+        if not documents:
+            self.watchers[file_id].cancel()
+            del self.watchers[file_id]
+        room_name = self.websocket_server.get_room_name(room)
+        self.websocket_server.delete_room(room=room)
+        file_path = await self.get_file_path(file_id, document)
+        logger.info(f"Closing collaboration room: {room_name} ({file_path})")
+
+
+class JupyterWebsocketServer(WebsocketServer):
+    def get_room(self, ws_path: str) -> YRoom:
+        if ws_path not in self.rooms:
+            if ws_path.count(":") >= 2:
+                # it is a stored document (e.g. a notebook)
+                file_format, file_type, file_id = ws_path.split(":", 2)
+                updates_file_path = f".{file_type}:{file_id}.y"
+                ystore = JupyterSQLiteYStore(path=updates_file_path)  # FIXME: pass in config
+                self.rooms[ws_path] = YRoom(ready=False, ystore=ystore)
+            else:
+                # it is a transient document (e.g. awareness)
+                self.rooms[ws_path] = YRoom()
+        return self.rooms[ws_path]
```

### Comparing `jupyverse-0.1.6/tests/conftest.py` & `jupyverse-0.1.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/tests/test_auth.py` & `jupyverse-0.1.8/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/tests/test_contents.py` & `jupyverse-0.1.8/tests/test_contents.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/tests/test_kernels.py` & `jupyverse-0.1.8/tests/test_kernels.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/tests/test_server.py` & `jupyverse-0.1.8/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/tests/test_settings.py` & `jupyverse-0.1.8/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/tests/utils.py` & `jupyverse-0.1.8/tests/utils.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/tests/data/notebook0.ipynb` & `jupyverse-0.1.8/tests/data/notebook0.ipynb`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/.gitignore` & `jupyverse-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/COPYING.md` & `jupyverse-0.1.8/plugins/yjs/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/README.md` & `jupyverse-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.1.6/pyproject.toml` & `jupyverse-0.1.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -63,14 +63,15 @@
   "pip install -e ./plugins/frontend",
   "pip install -e ./plugins/kernels",
   "pip install -e ./plugins/lab",
   "pip install -e ./plugins/nbconvert",
   "pip install -e ./plugins/terminals",
   "pip install -e ./plugins/yjs",
   "pip install -e ./plugins/resource_usage",
+  "pip install -e ./plugins/webdav[test]",
 ]
 features = ["test"]
 
 [tool.hatch.envs.dev.overrides]
 matrix.frontend.post-install-commands = [
   { value = "pip install -e ./plugins/jupyterlab", if = ["jupyterlab"]},
   { value = "pip install -e ./plugins/retrolab", if = ["retrolab"]},
@@ -93,29 +94,30 @@
 ]
 
 [[tool.hatch.envs.dev.matrix]]
 frontend = ["jupyterlab", "retrolab"]
 auth = ["noauth", "auth", "auth_fief"]
 
 [tool.hatch.envs.dev.scripts]
-test = "pytest ./tests -v"
+test = "pytest ./tests plugins/webdav/tests -v"
 lint = [
   "black --line-length 100 jupyverse ./plugins",
   "isort --profile=black jupyverse ./plugins",
 ]
 typecheck0 = """mypy --no-incremental \
 ./jupyverse_api \
 ./plugins/contents \
 ./plugins/frontend \
 ./plugins/kernels \
 ./plugins/lab \
 ./plugins/nbconvert \
 ./plugins/terminals \
 ./plugins/yjs \
 ./plugins/resource_usage \
+./plugins/webdav \
 """
 
 [tool.hatch.envs.docs]
 features = ["docs"]
 
 [tool.hatch.envs.docs.scripts]
 build = "mkdocs build --clean --strict"
@@ -147,15 +149,16 @@
     "plugins/lab:fps-lab",
     "plugins/nbconvert:fps-nbconvert",
     "plugins/retrolab:fps-retrolab",
     "plugins/terminals:fps-terminals",
     "plugins/yjs:fps-yjs",
     "plugins/resource_usage:fps-resource-usage",
     "plugins/login:fps-login",
-    ".:jupyverse:jupyverse_api,fps-noauth,fps-auth,fps-auth-fief,fps-contents,fps-jupyterlab,fps-kernels,fps-lab,fps-frontend,fps-nbconvert,fps-retrolab,fps-terminals,fps-yjs,fps-resource-usage"
+    "plugins/webdav:fps-webdav",
+    ".:jupyverse:jupyverse_api,fps-noauth,fps-auth,fps-auth-fief,fps-contents,fps-jupyterlab,fps-kernels,fps-lab,fps-frontend,fps-nbconvert,fps-retrolab,fps-terminals,fps-yjs,fps-resource-usage,fps-webdav"
 ]
 
 [tool.hatch.version]
 path = "jupyverse/__init__.py"
 
 [tool.pytest.ini_options]
 asyncio_mode = "strict"
```

### Comparing `jupyverse-0.1.6/PKG-INFO` & `jupyverse-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyverse
-Version: 0.1.6
+Version: 0.1.8
 Summary: A set of FPS plugins implementing a Jupyter server
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: fastapi,jupyter,plugins,server
 Requires-Python: >=3.8
```

