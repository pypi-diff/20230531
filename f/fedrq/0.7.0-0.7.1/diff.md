# Comparing `tmp/fedrq-0.7.0.tar.gz` & `tmp/fedrq-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedrq-0.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fedrq-0.7.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fedrq-0.7.0.tar` & `fedrq-0.7.1.tar`

### file list

```diff
@@ -1,117 +1,117 @@
--rw-r--r--   0        0        0      688 2023-05-28 23:13:09.924385 fedrq-0.7.0/.builds/epel9.yml
--rw-r--r--   0        0        0     2406 2023-05-28 08:06:22.506837 fedrq-0.7.0/.builds/main.yml
--rw-r--r--   0        0        0     1170 2023-05-28 23:13:09.924385 fedrq-0.7.0/.builds/mockbuild-36.yml
--rw-r--r--   0        0        0      751 2023-03-18 19:37:34.175930 fedrq-0.7.0/.builds/mockbuild.yml
--rw-r--r--   0        0        0      227 2023-02-19 18:37:34.746046 fedrq-0.7.0/.copr/Makefile
--rwxr-xr-x   0        0        0      512 2023-02-19 18:37:34.746046 fedrq-0.7.0/.copr/mk.sh
-lrwxr-xr-x   0        0        0        0 2023-02-19 18:37:34.747046 fedrq-0.7.0/.data/share/licenses/fedrq/GPL-2.0-or-later.txt -> ../../../../LICENSES/GPL-2.0-or-later.txt
-lrwxr-xr-x   0        0        0        0 2023-02-25 00:53:10.256118 fedrq-0.7.0/.data/share/licenses/fedrq/MIT.txt -> ../../../../LICENSES/MIT.txt
-lrwxr-xr-x   0        0        0        0 2023-02-25 00:53:10.256118 fedrq-0.7.0/.data/share/licenses/fedrq/PSF-2.0.txt -> ../../../../LICENSES/PSF-2.0.txt
-lrwxr-xr-x   0        0        0        0 2023-02-19 18:37:34.747046 fedrq-0.7.0/.data/share/licenses/fedrq/Unlicense.txt -> ../../../../LICENSES/Unlicense.txt
--rw-r--r--   0        0        0      268 2023-05-30 00:24:53.974774 fedrq-0.7.0/.gitignore
--rw-r--r--   0        0        0     2482 2023-03-19 02:41:47.073223 fedrq-0.7.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    17337 2022-12-13 02:49:11.735043 fedrq-0.7.0/LICENSES/GPL-2.0-or-later.txt
--rw-r--r--   0        0        0     1078 2022-12-13 02:49:11.735043 fedrq-0.7.0/LICENSES/MIT.txt
--rw-r--r--   0        0        0     2427 2023-02-19 18:37:34.747046 fedrq-0.7.0/LICENSES/PSF-2.0.txt
--rw-r--r--   0        0        0     1211 2023-02-19 18:37:34.747046 fedrq-0.7.0/LICENSES/Unlicense.txt
--rw-r--r--   0        0        0    12187 2023-05-30 00:25:30.044656 fedrq-0.7.0/NEWS.md
--rw-r--r--   0        0        0       89 2023-03-18 21:16:55.983019 fedrq-0.7.0/NEWS.md.license
--rw-r--r--   0        0        0    12144 2023-03-27 04:19:29.833647 fedrq-0.7.0/README.md
--rwxr-xr-x   0        0        0      687 2023-04-09 15:43:04.496271 fedrq-0.7.0/contrib/add_frag.py
--rwxr-xr-x   0        0        0      906 2023-03-19 23:05:00.923501 fedrq-0.7.0/contrib/api_examples/a_noarch_bash.py
--rwxr-xr-x   0        0        0     2502 2023-03-19 23:05:00.924501 fedrq-0.7.0/contrib/api_examples/ftbfs_retirements.py
--rw-r--r--   0        0        0      630 2023-03-19 23:07:21.352951 fedrq-0.7.0/contrib/deploy-docsite/main.yaml
--rw-r--r--   0        0        0      183 2023-03-19 23:07:21.352951 fedrq-0.7.0/contrib/deploy-docsite/roles/configure/handlers/main.yaml
--rw-r--r--   0        0        0      885 2023-03-19 23:07:21.352951 fedrq-0.7.0/contrib/deploy-docsite/roles/configure/tasks/main.yml
--rw-r--r--   0        0        0      163 2023-03-19 23:07:21.352951 fedrq-0.7.0/contrib/deploy-docsite/roles/configure/templates/fedrq.caddyfile
--rw-r--r--   0        0        0      415 2023-03-19 23:07:21.352951 fedrq-0.7.0/contrib/deploy-docsite/roles/deploy/tasks/main.yaml
--rw-r--r--   0        0        0      156 2023-03-19 23:07:21.352951 fedrq-0.7.0/contrib/deploy-docsite/vars.yaml
--rwxr-xr-x   0        0        0      914 2023-04-14 16:37:52.615305 fedrq-0.7.0/contrib/fedoraify.py
--rw-r--r--   0        0        0     5728 2023-04-11 14:33:20.624926 fedrq-0.7.0/doc/API/Summary.md
--rw-r--r--   0        0        0      147 2023-03-19 23:07:21.353951 fedrq-0.7.0/doc/API/backends/base.md
--rw-r--r--   0        0        0      343 2023-04-11 19:16:07.821729 fedrq-0.7.0/doc/API/backends/dnf.md
--rw-r--r--   0        0        0      532 2023-04-20 18:33:19.648796 fedrq-0.7.0/doc/API/backends/libdnf5.md
--rw-r--r--   0        0        0      133 2023-03-19 23:07:21.353951 fedrq-0.7.0/doc/API/config.md
--rw-r--r--   0        0        0      145 2023-03-19 23:07:21.353951 fedrq-0.7.0/doc/API/release_repo.md
-lrwxr-xr-x   0        0        0        0 2023-03-19 23:07:21.353951 fedrq-0.7.0/doc/News.md -> ../NEWS.md
--rw-r--r--   0        0        0     3322 2023-05-29 06:28:47.729780 fedrq-0.7.0/doc/dnf-repoquery-diff.md
--rw-r--r--   0        0        0    16162 2023-05-29 23:47:52.009062 fedrq-0.7.0/doc/fedrq.1.scd
--rw-r--r--   0        0        0       98 2023-02-19 18:37:34.749046 fedrq-0.7.0/doc/fedrq.1.scd.license
--rw-r--r--   0        0        0     4958 2023-04-11 12:51:07.649356 fedrq-0.7.0/doc/fedrq.5.scd
--rw-r--r--   0        0        0       98 2023-02-19 18:37:34.749046 fedrq-0.7.0/doc/fedrq.5.scd.license
-lrwxr-xr-x   0        0        0        0 2023-03-19 23:07:21.353951 fedrq-0.7.0/doc/index.md -> ../README.md
--rw-r--r--   0        0        0      131 2023-03-19 23:07:21.353951 fedrq-0.7.0/fedrq.rpmlintrc
--rw-r--r--   0        0        0     3419 2023-05-30 00:25:29.984656 fedrq-0.7.0/fedrq.spec
--rw-r--r--   0        0        0     2169 2023-04-11 19:22:07.524752 fedrq-0.7.0/mkdocs.yml
--rw-r--r--   0        0        0    12445 2023-05-30 00:22:03.019335 fedrq-0.7.0/noxfile.py
--rw-r--r--   0        0        0     2713 2023-05-30 00:25:22.777680 fedrq-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      532 2023-03-18 19:37:34.178930 fedrq-0.7.0/ruff.toml
--rw-r--r--   0        0        0      281 2023-02-21 18:02:47.599086 fedrq-0.7.0/src/fedrq/__init__.py
--rw-r--r--   0        0        0      219 2023-02-19 18:37:34.750046 fedrq-0.7.0/src/fedrq/__main__.py
--rw-r--r--   0        0        0     1713 2023-02-21 18:02:47.600086 fedrq-0.7.0/src/fedrq/_compat.py
--rw-r--r--   0        0        0      173 2023-03-18 19:37:34.178930 fedrq-0.7.0/src/fedrq/_config.py
--rw-r--r--   0        0        0     1248 2023-03-18 19:37:34.179930 fedrq-0.7.0/src/fedrq/_utils.py
--rw-r--r--   0        0        0     2529 2023-02-21 18:02:47.601086 fedrq-0.7.0/src/fedrq/backends/__init__.py
--rw-r--r--   0        0        0    14439 2023-05-29 15:11:03.621468 fedrq-0.7.0/src/fedrq/backends/base.py
--rw-r--r--   0        0        0      630 2023-02-21 18:02:47.603086 fedrq-0.7.0/src/fedrq/backends/dnf/__init__.py
--rw-r--r--   0        0        0     6949 2023-05-29 06:34:45.893651 fedrq-0.7.0/src/fedrq/backends/dnf/backend.py
--rw-r--r--   0        0        0      741 2023-02-21 18:02:47.604086 fedrq-0.7.0/src/fedrq/backends/libdnf5/__init__.py
--rw-r--r--   0        0        0    28006 2023-05-29 23:47:52.135062 fedrq-0.7.0/src/fedrq/backends/libdnf5/backend.py
--rw-r--r--   0        0        0     1955 2023-05-29 23:47:51.875063 fedrq-0.7.0/src/fedrq/cli/__init__.py
--rw-r--r--   0        0        0    15680 2023-05-29 23:47:51.877063 fedrq-0.7.0/src/fedrq/cli/base.py
--rw-r--r--   0        0        0        0 2023-02-19 18:37:34.751046 fedrq-0.7.0/src/fedrq/cli/commands/__init__.py
--rw-r--r--   0        0        0     2854 2023-03-18 19:37:34.182930 fedrq-0.7.0/src/fedrq/cli/commands/pkgs.py
--rw-r--r--   0        0        0     1489 2023-05-29 23:47:51.877063 fedrq-0.7.0/src/fedrq/cli/commands/repolist.py
--rw-r--r--   0        0        0     2425 2023-03-17 02:28:51.186103 fedrq-0.7.0/src/fedrq/cli/commands/subpkgs.py
--rw-r--r--   0        0        0    10843 2023-03-18 19:37:34.182930 fedrq-0.7.0/src/fedrq/cli/commands/whatrequires.py
--rw-r--r--   0        0        0    13071 2023-04-06 12:36:51.698430 fedrq-0.7.0/src/fedrq/cli/formatters.py
--rw-r--r--   0        0        0    16722 2023-05-30 00:06:50.295329 fedrq-0.7.0/src/fedrq/config.py
--rw-r--r--   0        0        0        0 2023-02-19 18:37:34.751046 fedrq-0.7.0/src/fedrq/data/__init__.py
--rw-r--r--   0        0        0     7030 2023-05-29 23:47:52.009062 fedrq-0.7.0/src/fedrq/data/releases.toml
--rw-r--r--   0        0        0        0 2023-02-19 18:37:34.752046 fedrq-0.7.0/src/fedrq/data/repos/__init__.py
--rw-r--r--   0        0        0     2053 2023-05-29 03:25:46.306279 fedrq-0.7.0/src/fedrq/data/repos/almalinux.repo
--rw-r--r--   0        0        0      639 2023-03-27 04:19:29.835647 fedrq-0.7.0/src/fedrq/data/repos/amazonlinux.repo
--rw-r--r--   0        0        0     1386 2023-05-29 03:25:46.306279 fedrq-0.7.0/src/fedrq/data/repos/centos-stream-compose.repo
--rw-r--r--   0        0        0     1850 2023-02-19 18:37:34.752046 fedrq-0.7.0/src/fedrq/data/repos/centos-stream.repo
--rw-r--r--   0        0        0     1494 2023-05-29 03:25:46.306279 fedrq-0.7.0/src/fedrq/data/repos/centos-stream8-compose.repo
--rw-r--r--   0        0        0     1599 2023-03-18 19:37:34.184930 fedrq-0.7.0/src/fedrq/data/repos/centos-stream8.repo
--rw-r--r--   0        0        0     1809 2023-05-29 03:58:29.496700 fedrq-0.7.0/src/fedrq/data/repos/eln.repo
--rw-r--r--   0        0        0     2158 2023-05-29 03:25:46.306279 fedrq-0.7.0/src/fedrq/data/repos/epel.repo
--rw-r--r--   0        0        0    14146 2023-05-29 03:25:46.419279 fedrq-0.7.0/src/fedrq/data/repos/fedora-eln.repo
--rw-r--r--   0        0        0     2402 2023-02-19 18:37:34.752046 fedrq-0.7.0/src/fedrq/data/repos/fedora-rawhide.repo
--rw-r--r--   0        0        0     1480 2023-02-19 18:37:34.752046 fedrq-0.7.0/src/fedrq/data/repos/fedora-updates-testing.repo
--rw-r--r--   0        0        0     1422 2023-02-19 18:37:34.752046 fedrq-0.7.0/src/fedrq/data/repos/fedora-updates.repo
--rw-r--r--   0        0        0     1375 2023-02-19 18:37:34.752046 fedrq-0.7.0/src/fedrq/data/repos/fedora.repo
--rw-r--r--   0        0        0      425 2023-05-29 03:25:46.306279 fedrq-0.7.0/src/fedrq/data/repos/rawhide-buildroot.repo
--rw-r--r--   0        0        0        0 2023-02-19 18:37:34.752046 fedrq-0.7.0/src/fedrq/py.typed
--rw-r--r--   0        0        0     8912 2023-05-28 01:30:25.101262 fedrq-0.7.0/src/fedrq/release_repo.py
--rw-r--r--   0        0        0      984 2023-02-21 18:02:47.612086 fedrq-0.7.0/src/fedrq/repoquery.py
--rwxr-xr-x   0        0        0      488 2023-02-19 18:37:34.753046 fedrq-0.7.0/srpm.sh
--rw-r--r--   0        0        0      154 2023-02-19 18:37:34.753046 fedrq-0.7.0/tests/.gitignore
--rw-r--r--   0        0        0        0 2023-05-29 04:18:46.483879 fedrq-0.7.0/tests/__init__.py
--rw-r--r--   0        0        0     2912 2023-02-21 18:02:47.613086 fedrq-0.7.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-05-29 04:18:46.483879 fedrq-0.7.0/tests/integration/__init__.py
--rw-r--r--   0        0        0     1739 2023-02-21 18:02:47.614086 fedrq-0.7.0/tests/integration/test_backends.py
--rw-r--r--   0        0        0      735 2023-05-28 08:06:22.609836 fedrq-0.7.0/tests/integration/test_pkgs.py
--rw-r--r--   0        0        0     1219 2023-03-18 19:37:34.185930 fedrq-0.7.0/tests/integration/test_subpkgs.py
--rw-r--r--   0        0        0     1725 2023-02-19 18:37:34.753046 fedrq-0.7.0/tests/integration/test_whatrequires.py
--rw-r--r--   0        0        0     1334 2023-02-19 18:37:34.753046 fedrq-0.7.0/tests/integration/test_whatrequires_src.py
--rw-r--r--   0        0        0        0 2023-05-29 04:18:46.484879 fedrq-0.7.0/tests/test_data/__init__.py
--rw-r--r--   0        0        0      332 2023-02-19 18:37:34.753046 fedrq-0.7.0/tests/test_data/_template.spec
--rwxr-xr-x   0        0        0     1449 2023-02-19 18:37:34.754046 fedrq-0.7.0/tests/test_data/build.sh
--rw-r--r--   0        0        0     1130 2023-02-19 18:37:34.754046 fedrq-0.7.0/tests/test_data/repos/repo1/specs/e1/packageb.spec
--rw-r--r--   0        0        0     1060 2023-02-19 18:37:34.754046 fedrq-0.7.0/tests/test_data/repos/repo1/specs/packagea.spec
--rw-r--r--   0        0        0     1156 2023-02-19 18:37:34.754046 fedrq-0.7.0/tests/test_data/repos/repo1/specs/packageb.spec
--rw-r--r--   0        0        0        0 2023-05-29 04:18:46.484879 fedrq-0.7.0/tests/unit/__init__.py
--rw-r--r--   0        0        0     2092 2023-05-29 15:11:03.621468 fedrq-0.7.0/tests/unit/test_checkconfig.py
--rw-r--r--   0        0        0     7127 2023-05-28 01:58:42.063000 fedrq-0.7.0/tests/unit/test_command.py
--rw-r--r--   0        0        0     7075 2023-02-21 18:02:47.617086 fedrq-0.7.0/tests/unit/test_formatters.py
--rw-r--r--   0        0        0     2161 2023-05-29 23:47:52.009062 fedrq-0.7.0/tests/unit/test_pkgs.py
--rw-r--r--   0        0        0     1645 2023-03-18 19:37:34.185930 fedrq-0.7.0/tests/unit/test_release.py
--rw-r--r--   0        0        0      413 2023-02-21 18:02:47.618086 fedrq-0.7.0/tests/unit/test_repo.py
--rw-r--r--   0        0        0      604 2023-05-29 23:47:51.877063 fedrq-0.7.0/tests/unit/test_repolist.py
--rw-r--r--   0        0        0     1289 2023-03-20 17:10:06.077134 fedrq-0.7.0/tests/unit/test_repoquery.py
--rw-r--r--   0        0        0     2676 2023-02-19 18:37:34.755046 fedrq-0.7.0/tests/unit/test_subbpkgs.py
--rw-r--r--   0        0        0     4052 2023-03-17 01:22:48.917895 fedrq-0.7.0/tests/unit/test_whatrequires.py
--rw-r--r--   0        0        0      653 2023-02-19 18:37:34.755046 fedrq-0.7.0/tests/unit/test_whatrequires_src.py
--rw-r--r--   0        0        0    14085 1970-01-01 00:00:00.000000 fedrq-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      688 2023-05-28 23:13:09.924385 fedrq-0.7.1/.builds/epel9.yml
+-rw-r--r--   0        0        0     2406 2023-05-28 08:06:22.506837 fedrq-0.7.1/.builds/main.yml
+-rw-r--r--   0        0        0     1170 2023-05-28 23:13:09.924385 fedrq-0.7.1/.builds/mockbuild-36.yml
+-rw-r--r--   0        0        0      751 2023-03-18 19:37:34.175930 fedrq-0.7.1/.builds/mockbuild.yml
+-rw-r--r--   0        0        0      227 2023-02-19 18:37:34.746046 fedrq-0.7.1/.copr/Makefile
+-rwxr-xr-x   0        0        0      512 2023-02-19 18:37:34.746046 fedrq-0.7.1/.copr/mk.sh
+lrwxr-xr-x   0        0        0        0 2023-02-19 18:37:34.747046 fedrq-0.7.1/.data/share/licenses/fedrq/GPL-2.0-or-later.txt -> ../../../../LICENSES/GPL-2.0-or-later.txt
+lrwxr-xr-x   0        0        0        0 2023-02-25 00:53:10.256118 fedrq-0.7.1/.data/share/licenses/fedrq/MIT.txt -> ../../../../LICENSES/MIT.txt
+lrwxr-xr-x   0        0        0        0 2023-02-25 00:53:10.256118 fedrq-0.7.1/.data/share/licenses/fedrq/PSF-2.0.txt -> ../../../../LICENSES/PSF-2.0.txt
+lrwxr-xr-x   0        0        0        0 2023-02-19 18:37:34.747046 fedrq-0.7.1/.data/share/licenses/fedrq/Unlicense.txt -> ../../../../LICENSES/Unlicense.txt
+-rw-r--r--   0        0        0      268 2023-05-30 00:24:53.974774 fedrq-0.7.1/.gitignore
+-rw-r--r--   0        0        0     2482 2023-03-19 02:41:47.073223 fedrq-0.7.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0    17337 2022-12-13 02:49:11.735043 fedrq-0.7.1/LICENSES/GPL-2.0-or-later.txt
+-rw-r--r--   0        0        0     1078 2022-12-13 02:49:11.735043 fedrq-0.7.1/LICENSES/MIT.txt
+-rw-r--r--   0        0        0     2427 2023-02-19 18:37:34.747046 fedrq-0.7.1/LICENSES/PSF-2.0.txt
+-rw-r--r--   0        0        0     1211 2023-02-19 18:37:34.747046 fedrq-0.7.1/LICENSES/Unlicense.txt
+-rw-r--r--   0        0        0    12505 2023-05-31 19:47:52.649519 fedrq-0.7.1/NEWS.md
+-rw-r--r--   0        0        0       89 2023-03-18 21:16:55.983019 fedrq-0.7.1/NEWS.md.license
+-rw-r--r--   0        0        0    12144 2023-03-27 04:19:29.833647 fedrq-0.7.1/README.md
+-rwxr-xr-x   0        0        0      687 2023-04-09 15:43:04.496271 fedrq-0.7.1/contrib/add_frag.py
+-rwxr-xr-x   0        0        0      906 2023-03-19 23:05:00.923501 fedrq-0.7.1/contrib/api_examples/a_noarch_bash.py
+-rwxr-xr-x   0        0        0     2502 2023-03-19 23:05:00.924501 fedrq-0.7.1/contrib/api_examples/ftbfs_retirements.py
+-rw-r--r--   0        0        0      630 2023-03-19 23:07:21.352951 fedrq-0.7.1/contrib/deploy-docsite/main.yaml
+-rw-r--r--   0        0        0      183 2023-03-19 23:07:21.352951 fedrq-0.7.1/contrib/deploy-docsite/roles/configure/handlers/main.yaml
+-rw-r--r--   0        0        0      885 2023-03-19 23:07:21.352951 fedrq-0.7.1/contrib/deploy-docsite/roles/configure/tasks/main.yml
+-rw-r--r--   0        0        0      163 2023-03-19 23:07:21.352951 fedrq-0.7.1/contrib/deploy-docsite/roles/configure/templates/fedrq.caddyfile
+-rw-r--r--   0        0        0      415 2023-03-19 23:07:21.352951 fedrq-0.7.1/contrib/deploy-docsite/roles/deploy/tasks/main.yaml
+-rw-r--r--   0        0        0      156 2023-03-19 23:07:21.352951 fedrq-0.7.1/contrib/deploy-docsite/vars.yaml
+-rwxr-xr-x   0        0        0      914 2023-04-14 16:37:52.615305 fedrq-0.7.1/contrib/fedoraify.py
+-rw-r--r--   0        0        0     5728 2023-04-11 14:33:20.624926 fedrq-0.7.1/doc/API/Summary.md
+-rw-r--r--   0        0        0      147 2023-03-19 23:07:21.353951 fedrq-0.7.1/doc/API/backends/base.md
+-rw-r--r--   0        0        0      343 2023-04-11 19:16:07.821729 fedrq-0.7.1/doc/API/backends/dnf.md
+-rw-r--r--   0        0        0      532 2023-04-20 18:33:19.648796 fedrq-0.7.1/doc/API/backends/libdnf5.md
+-rw-r--r--   0        0        0      133 2023-03-19 23:07:21.353951 fedrq-0.7.1/doc/API/config.md
+-rw-r--r--   0        0        0      145 2023-03-19 23:07:21.353951 fedrq-0.7.1/doc/API/release_repo.md
+lrwxr-xr-x   0        0        0        0 2023-03-19 23:07:21.353951 fedrq-0.7.1/doc/News.md -> ../NEWS.md
+-rw-r--r--   0        0        0     3322 2023-05-29 06:28:47.729780 fedrq-0.7.1/doc/dnf-repoquery-diff.md
+-rw-r--r--   0        0        0    16162 2023-05-29 23:47:52.009062 fedrq-0.7.1/doc/fedrq.1.scd
+-rw-r--r--   0        0        0       98 2023-02-19 18:37:34.749046 fedrq-0.7.1/doc/fedrq.1.scd.license
+-rw-r--r--   0        0        0     4958 2023-04-11 12:51:07.649356 fedrq-0.7.1/doc/fedrq.5.scd
+-rw-r--r--   0        0        0       98 2023-02-19 18:37:34.749046 fedrq-0.7.1/doc/fedrq.5.scd.license
+lrwxr-xr-x   0        0        0        0 2023-03-19 23:07:21.353951 fedrq-0.7.1/doc/index.md -> ../README.md
+-rw-r--r--   0        0        0      131 2023-03-19 23:07:21.353951 fedrq-0.7.1/fedrq.rpmlintrc
+-rw-r--r--   0        0        0     3493 2023-05-31 19:47:52.604519 fedrq-0.7.1/fedrq.spec
+-rw-r--r--   0        0        0     2169 2023-04-11 19:22:07.524752 fedrq-0.7.1/mkdocs.yml
+-rw-r--r--   0        0        0    12535 2023-05-30 00:43:08.753184 fedrq-0.7.1/noxfile.py
+-rw-r--r--   0        0        0     2713 2023-05-31 19:47:49.568530 fedrq-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      532 2023-03-18 19:37:34.178930 fedrq-0.7.1/ruff.toml
+-rw-r--r--   0        0        0      281 2023-02-21 18:02:47.599086 fedrq-0.7.1/src/fedrq/__init__.py
+-rw-r--r--   0        0        0      219 2023-02-19 18:37:34.750046 fedrq-0.7.1/src/fedrq/__main__.py
+-rw-r--r--   0        0        0     1713 2023-02-21 18:02:47.600086 fedrq-0.7.1/src/fedrq/_compat.py
+-rw-r--r--   0        0        0      173 2023-03-18 19:37:34.178930 fedrq-0.7.1/src/fedrq/_config.py
+-rw-r--r--   0        0        0     1248 2023-03-18 19:37:34.179930 fedrq-0.7.1/src/fedrq/_utils.py
+-rw-r--r--   0        0        0     2529 2023-02-21 18:02:47.601086 fedrq-0.7.1/src/fedrq/backends/__init__.py
+-rw-r--r--   0        0        0    14439 2023-05-29 15:11:03.621468 fedrq-0.7.1/src/fedrq/backends/base.py
+-rw-r--r--   0        0        0      630 2023-02-21 18:02:47.603086 fedrq-0.7.1/src/fedrq/backends/dnf/__init__.py
+-rw-r--r--   0        0        0     6949 2023-05-29 06:34:45.893651 fedrq-0.7.1/src/fedrq/backends/dnf/backend.py
+-rw-r--r--   0        0        0      741 2023-02-21 18:02:47.604086 fedrq-0.7.1/src/fedrq/backends/libdnf5/__init__.py
+-rw-r--r--   0        0        0    28232 2023-05-31 17:51:01.797529 fedrq-0.7.1/src/fedrq/backends/libdnf5/backend.py
+-rw-r--r--   0        0        0     1955 2023-05-29 23:47:51.875063 fedrq-0.7.1/src/fedrq/cli/__init__.py
+-rw-r--r--   0        0        0    15680 2023-05-29 23:47:51.877063 fedrq-0.7.1/src/fedrq/cli/base.py
+-rw-r--r--   0        0        0        0 2023-02-19 18:37:34.751046 fedrq-0.7.1/src/fedrq/cli/commands/__init__.py
+-rw-r--r--   0        0        0     2854 2023-03-18 19:37:34.182930 fedrq-0.7.1/src/fedrq/cli/commands/pkgs.py
+-rw-r--r--   0        0        0     1489 2023-05-29 23:47:51.877063 fedrq-0.7.1/src/fedrq/cli/commands/repolist.py
+-rw-r--r--   0        0        0     2425 2023-03-17 02:28:51.186103 fedrq-0.7.1/src/fedrq/cli/commands/subpkgs.py
+-rw-r--r--   0        0        0    10843 2023-03-18 19:37:34.182930 fedrq-0.7.1/src/fedrq/cli/commands/whatrequires.py
+-rw-r--r--   0        0        0    13071 2023-04-06 12:36:51.698430 fedrq-0.7.1/src/fedrq/cli/formatters.py
+-rw-r--r--   0        0        0    16722 2023-05-30 00:06:50.295329 fedrq-0.7.1/src/fedrq/config.py
+-rw-r--r--   0        0        0        0 2023-02-19 18:37:34.751046 fedrq-0.7.1/src/fedrq/data/__init__.py
+-rw-r--r--   0        0        0     7030 2023-05-29 23:47:52.009062 fedrq-0.7.1/src/fedrq/data/releases.toml
+-rw-r--r--   0        0        0        0 2023-02-19 18:37:34.752046 fedrq-0.7.1/src/fedrq/data/repos/__init__.py
+-rw-r--r--   0        0        0     2053 2023-05-29 03:25:46.306279 fedrq-0.7.1/src/fedrq/data/repos/almalinux.repo
+-rw-r--r--   0        0        0      639 2023-03-27 04:19:29.835647 fedrq-0.7.1/src/fedrq/data/repos/amazonlinux.repo
+-rw-r--r--   0        0        0     1386 2023-05-29 03:25:46.306279 fedrq-0.7.1/src/fedrq/data/repos/centos-stream-compose.repo
+-rw-r--r--   0        0        0     1850 2023-02-19 18:37:34.752046 fedrq-0.7.1/src/fedrq/data/repos/centos-stream.repo
+-rw-r--r--   0        0        0     1494 2023-05-29 03:25:46.306279 fedrq-0.7.1/src/fedrq/data/repos/centos-stream8-compose.repo
+-rw-r--r--   0        0        0     1599 2023-03-18 19:37:34.184930 fedrq-0.7.1/src/fedrq/data/repos/centos-stream8.repo
+-rw-r--r--   0        0        0     1809 2023-05-29 03:58:29.496700 fedrq-0.7.1/src/fedrq/data/repos/eln.repo
+-rw-r--r--   0        0        0     2158 2023-05-29 03:25:46.306279 fedrq-0.7.1/src/fedrq/data/repos/epel.repo
+-rw-r--r--   0        0        0    14146 2023-05-29 03:25:46.419279 fedrq-0.7.1/src/fedrq/data/repos/fedora-eln.repo
+-rw-r--r--   0        0        0     2402 2023-02-19 18:37:34.752046 fedrq-0.7.1/src/fedrq/data/repos/fedora-rawhide.repo
+-rw-r--r--   0        0        0     1480 2023-02-19 18:37:34.752046 fedrq-0.7.1/src/fedrq/data/repos/fedora-updates-testing.repo
+-rw-r--r--   0        0        0     1422 2023-02-19 18:37:34.752046 fedrq-0.7.1/src/fedrq/data/repos/fedora-updates.repo
+-rw-r--r--   0        0        0     1375 2023-02-19 18:37:34.752046 fedrq-0.7.1/src/fedrq/data/repos/fedora.repo
+-rw-r--r--   0        0        0      425 2023-05-29 03:25:46.306279 fedrq-0.7.1/src/fedrq/data/repos/rawhide-buildroot.repo
+-rw-r--r--   0        0        0        0 2023-02-19 18:37:34.752046 fedrq-0.7.1/src/fedrq/py.typed
+-rw-r--r--   0        0        0     8912 2023-05-28 01:30:25.101262 fedrq-0.7.1/src/fedrq/release_repo.py
+-rw-r--r--   0        0        0      984 2023-02-21 18:02:47.612086 fedrq-0.7.1/src/fedrq/repoquery.py
+-rwxr-xr-x   0        0        0      488 2023-02-19 18:37:34.753046 fedrq-0.7.1/srpm.sh
+-rw-r--r--   0        0        0      154 2023-02-19 18:37:34.753046 fedrq-0.7.1/tests/.gitignore
+-rw-r--r--   0        0        0        0 2023-05-29 04:18:46.483879 fedrq-0.7.1/tests/__init__.py
+-rw-r--r--   0        0        0     2912 2023-02-21 18:02:47.613086 fedrq-0.7.1/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:18:46.483879 fedrq-0.7.1/tests/integration/__init__.py
+-rw-r--r--   0        0        0     1739 2023-02-21 18:02:47.614086 fedrq-0.7.1/tests/integration/test_backends.py
+-rw-r--r--   0        0        0      735 2023-05-28 08:06:22.609836 fedrq-0.7.1/tests/integration/test_pkgs.py
+-rw-r--r--   0        0        0     1219 2023-03-18 19:37:34.185930 fedrq-0.7.1/tests/integration/test_subpkgs.py
+-rw-r--r--   0        0        0     1725 2023-02-19 18:37:34.753046 fedrq-0.7.1/tests/integration/test_whatrequires.py
+-rw-r--r--   0        0        0     1334 2023-02-19 18:37:34.753046 fedrq-0.7.1/tests/integration/test_whatrequires_src.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:18:46.484879 fedrq-0.7.1/tests/test_data/__init__.py
+-rw-r--r--   0        0        0      332 2023-02-19 18:37:34.753046 fedrq-0.7.1/tests/test_data/_template.spec
+-rwxr-xr-x   0        0        0     1449 2023-02-19 18:37:34.754046 fedrq-0.7.1/tests/test_data/build.sh
+-rw-r--r--   0        0        0     1130 2023-02-19 18:37:34.754046 fedrq-0.7.1/tests/test_data/repos/repo1/specs/e1/packageb.spec
+-rw-r--r--   0        0        0     1060 2023-02-19 18:37:34.754046 fedrq-0.7.1/tests/test_data/repos/repo1/specs/packagea.spec
+-rw-r--r--   0        0        0     1156 2023-02-19 18:37:34.754046 fedrq-0.7.1/tests/test_data/repos/repo1/specs/packageb.spec
+-rw-r--r--   0        0        0        0 2023-05-29 04:18:46.484879 fedrq-0.7.1/tests/unit/__init__.py
+-rw-r--r--   0        0        0     2092 2023-05-29 15:11:03.621468 fedrq-0.7.1/tests/unit/test_checkconfig.py
+-rw-r--r--   0        0        0     7127 2023-05-28 01:58:42.063000 fedrq-0.7.1/tests/unit/test_command.py
+-rw-r--r--   0        0        0     7075 2023-02-21 18:02:47.617086 fedrq-0.7.1/tests/unit/test_formatters.py
+-rw-r--r--   0        0        0     2161 2023-05-29 23:47:52.009062 fedrq-0.7.1/tests/unit/test_pkgs.py
+-rw-r--r--   0        0        0     1645 2023-03-18 19:37:34.185930 fedrq-0.7.1/tests/unit/test_release.py
+-rw-r--r--   0        0        0      413 2023-02-21 18:02:47.618086 fedrq-0.7.1/tests/unit/test_repo.py
+-rw-r--r--   0        0        0      604 2023-05-29 23:47:51.877063 fedrq-0.7.1/tests/unit/test_repolist.py
+-rw-r--r--   0        0        0     1289 2023-03-20 17:10:06.077134 fedrq-0.7.1/tests/unit/test_repoquery.py
+-rw-r--r--   0        0        0     2676 2023-02-19 18:37:34.755046 fedrq-0.7.1/tests/unit/test_subbpkgs.py
+-rw-r--r--   0        0        0     4052 2023-03-17 01:22:48.917895 fedrq-0.7.1/tests/unit/test_whatrequires.py
+-rw-r--r--   0        0        0      653 2023-02-19 18:37:34.755046 fedrq-0.7.1/tests/unit/test_whatrequires_src.py
+-rw-r--r--   0        0        0    14085 1970-01-01 00:00:00.000000 fedrq-0.7.1/PKG-INFO
```

### Comparing `fedrq-0.7.0/.builds/epel9.yml` & `fedrq-0.7.1/.builds/epel9.yml`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/.builds/main.yml` & `fedrq-0.7.1/.builds/main.yml`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/.builds/mockbuild-36.yml` & `fedrq-0.7.1/.builds/mockbuild-36.yml`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/.builds/mockbuild.yml` & `fedrq-0.7.1/.builds/mockbuild.yml`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/.copr/mk.sh` & `fedrq-0.7.1/.copr/mk.sh`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/CONTRIBUTING.md` & `fedrq-0.7.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/LICENSES/GPL-2.0-or-later.txt` & `fedrq-0.7.1/LICENSES/GPL-2.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/LICENSES/MIT.txt` & `fedrq-0.7.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/LICENSES/PSF-2.0.txt` & `fedrq-0.7.1/LICENSES/PSF-2.0.txt`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/LICENSES/Unlicense.txt` & `fedrq-0.7.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/NEWS.md` & `fedrq-0.7.1/NEWS.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 NEWS
 =====
 
+## 0.7.1 - 2023-05-31 <a id='0.7.1'></a>
+
+### Fixed
+
+- libdnf5: fix downloadsize and size formatters compat.
+  This change is needed to maintain compat after
+  [rpm-software-management/dnf5#766fb3a][766fb3a].
+
+[766fb3a]: https://github.com/rpm-software-management/dnf5/commit/766fb3ad8745e42e4d5b73417aa54898e2d0f89f
+
 ## 0.7.0 - 2023-05-30 <a id='0.7.0'></a>
 
 ### Highlighted examples
 
 fedrq now has a Fedora ELN release configuration builtin!
 
 You can preform simple queries
```

### Comparing `fedrq-0.7.0/README.md` & `fedrq-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/contrib/add_frag.py` & `fedrq-0.7.1/contrib/add_frag.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/contrib/api_examples/a_noarch_bash.py` & `fedrq-0.7.1/contrib/api_examples/a_noarch_bash.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/contrib/api_examples/ftbfs_retirements.py` & `fedrq-0.7.1/contrib/api_examples/ftbfs_retirements.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/contrib/deploy-docsite/main.yaml` & `fedrq-0.7.1/contrib/deploy-docsite/main.yaml`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/contrib/deploy-docsite/roles/configure/tasks/main.yml` & `fedrq-0.7.1/contrib/deploy-docsite/roles/configure/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/contrib/fedoraify.py` & `fedrq-0.7.1/contrib/fedoraify.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/doc/API/Summary.md` & `fedrq-0.7.1/doc/API/Summary.md`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/doc/API/backends/libdnf5.md` & `fedrq-0.7.1/doc/API/backends/libdnf5.md`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/doc/dnf-repoquery-diff.md` & `fedrq-0.7.1/doc/dnf-repoquery-diff.md`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/doc/fedrq.1.scd` & `fedrq-0.7.1/doc/fedrq.1.scd`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/doc/fedrq.5.scd` & `fedrq-0.7.1/doc/fedrq.5.scd`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/fedrq.spec` & `fedrq-0.7.1/fedrq.spec`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright (C) 2022 Maxwell G <gotmax@e.email>
 # SPDX-License-Identifier: MIT
 # License text: https://spdx.org/licenses/MIT.html
 
 %bcond libdnf5 %[0%{?fedora} >= 38]
 
 Name:           fedrq
-Version:        0.7.0
+Version:        0.7.1
 Release:        1%{?dist}
 Summary:        A tool to query the Fedora and EPEL repositories
 
 # - code is GPL-2.0-or-later
 # - the data and config files in fedrq/data are UNLICENSEed
 # - Embeded repo defs are MIT.
 # - PSF-2.0 code copied from Cpython 3.11 for older Python versions
@@ -95,14 +95,17 @@
 %{bash_completions_dir}/fedrq
 %{fish_completions_dir}/fedrq.fish
 %{_mandir}/man1/fedrq.1*
 %{_mandir}/man5/fedrq.5*
 
 
 %changelog
+* Wed May 31 2023 Maxwell G <maxwell@gtmx.me> - 0.7.1-1
+- Release 0.7.1.
+
 * Tue May 30 2023 Maxwell G <maxwell@gtmx.me> - 0.7.0-1
 - Release 0.7.0.
 
 * Sat Apr 08 2023 Maxwell G <maxwell@gtmx.me> - 0.6.0-1
 - Release 0.6.0
 
 * Sat Mar 18 2023 Maxwell G <maxwell@gtmx.me> - 0.5.0-1
```

### Comparing `fedrq-0.7.0/mkdocs.yml` & `fedrq-0.7.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/noxfile.py` & `fedrq-0.7.1/noxfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -344,30 +344,32 @@
 
 
 @nox.session
 def publish(session: nox.Session):
     # Setup
     ensure_clean(session)
     install(session, "twine", "tomcli[tomlkit]")
+
+    # Upload to PyPI
     session.run(
         "twine",
         "upload",
         "--non-interactive",
         "--username",
         "__token__",
-        *_get_artifacts(("*.whl", "*.tar.gz"), extra_allowed=False, expected_count=2),
+        *_get_artifacts(("*.whl", "*.tar.gz"), expected_count=2),
     )
 
-    # Copr build
-    copr_release(session)
-
-    # Push to git
-    if session.interactive and input("Push to Sourcehut (Y/n)").lower() != "n":
+    # Push to git, publish artifacts to sourcehut, and release to copr
+    if not session.interactive or input(
+        "Push to Sourcehut and copr build (Y/n)"
+    ).lower() in ("", "y"):
         git(session, "push", "--follow-tags")
         srht_artifacts(session)
+        copr_release(session)
 
     # Post-release bump
     version = session.run(  # type: ignore[union-attr]
         "tomcli-get", "pyproject.toml", "project.version", silent=True
     ).strip()
     session.run(
         "tomcli-set", "pyproject.toml", "str", "project.version", f"{version}.post0"
@@ -403,18 +405,18 @@
         # fmt: on
 
 
 @nox.session
 def copr_release(session: nox.Session):
     install(session, "copr-cli", "requests-gssapi", "specfile")
     tmp = Path(session.create_tmp())
-    dest = tmp / "tomcli.spec"
-    copy2("tomcli.spec", dest)
+    dest = tmp / f"{PROJECT}.spec"
+    copy2(f"{PROJECT}.spec", dest)
     session.run("python", "contrib/fedoraify.py", str(dest))
-    session.run("copr-cli", "build", "--nowait", "gotmax23/tomcli", str(dest))
+    session.run("copr-cli", "build", "--nowait", f"gotmax23/{PROJECT}", str(dest))
 
 
 @nox.session(python="none")
 def srht_artifacts(session: nox.Session):
     artifacts = map(str, Path("dist").glob("*"))
     session.run("hut", "git", "artifact", "upload", *artifacts, external=True)
```

### Comparing `fedrq-0.7.0/pyproject.toml` & `fedrq-0.7.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 requires = ["flit_core >=3.7,<4"]
 build-backend = "flit_core.buildapi"
 
 
 [project]
 name = "fedrq"
 description = "fedrq is a tool to query the Fedora and EPEL repositories"
-version = "0.7.0"
+version = "0.7.1"
 authors = [{ name = "Maxwell G", email = "gotmax@e.email" }]
 readme = "README.md"
 license = { text = "GPL-2.0-or-later AND Unlicense AND MIT" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
```

### Comparing `fedrq-0.7.0/ruff.toml` & `fedrq-0.7.1/ruff.toml`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/src/fedrq/_compat.py` & `fedrq-0.7.1/src/fedrq/_compat.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/src/fedrq/_utils.py` & `fedrq-0.7.1/src/fedrq/_utils.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/src/fedrq/backends/__init__.py` & `fedrq-0.7.1/src/fedrq/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/src/fedrq/backends/base.py` & `fedrq-0.7.1/src/fedrq/backends/base.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/src/fedrq/backends/dnf/__init__.py` & `fedrq-0.7.1/src/fedrq/backends/dnf/__init__.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/src/fedrq/backends/dnf/backend.py` & `fedrq-0.7.1/src/fedrq/backends/dnf/backend.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/src/fedrq/backends/libdnf5/__init__.py` & `fedrq-0.7.1/src/fedrq/backends/libdnf5/__init__.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/src/fedrq/backends/libdnf5/backend.py` & `fedrq-0.7.1/src/fedrq/backends/libdnf5/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -357,14 +357,15 @@
         repoq.filter_id([name])
         return next(iter(repoq), None)
 
     def load_filelists(self) -> None:
         LOG.debug("Loading filelists")
         option = self._get_option(self.config, "optional_metadata_types")
         func = option.add_item
+        # https://github.com/rpm-software-management/dnf5/commit/ba011ff
         if "priority" in inspect.signature(func).parameters:
             func(Priority_RUNTIME, libdnf5.conf.METADATA_TYPE_FILELISTS)
         else:
             func(libdnf5.conf.METADATA_TYPE_FILELISTS)
 
     def create_repo(self, repoid: str, **kwargs) -> None:
         """
@@ -510,19 +511,23 @@
 
     @property
     def buildtime(self) -> int:
         return self.get_build_time()
 
     @property
     def size(self) -> int:
-        return self.get_package_size()
+        return self.downloadsize
 
     @property
     def downloadsize(self) -> int:
-        return self.get_package_size()
+        # https://github.com/rpm-software-management/dnf5/pull/558
+        try:
+            return self.get_download_size()
+        except AttributeError:
+            return self.get_package_size()
 
     @property
     def installsize(self) -> int:
         return self.get_install_size()
 
     @property
     def provides(self) -> Iterable[Reldep5]:
```

### Comparing `fedrq-0.7.0/src/fedrq/cli/__init__.py` & `fedrq-0.7.1/src/fedrq/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/src/fedrq/cli/base.py` & `fedrq-0.7.1/src/fedrq/cli/base.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/src/fedrq/cli/commands/pkgs.py` & `fedrq-0.7.1/src/fedrq/cli/commands/pkgs.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/src/fedrq/cli/commands/repolist.py` & `fedrq-0.7.1/src/fedrq/cli/commands/repolist.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/src/fedrq/cli/commands/subpkgs.py` & `fedrq-0.7.1/src/fedrq/cli/commands/subpkgs.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/src/fedrq/cli/commands/whatrequires.py` & `fedrq-0.7.1/src/fedrq/cli/commands/whatrequires.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/src/fedrq/cli/formatters.py` & `fedrq-0.7.1/src/fedrq/cli/formatters.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/src/fedrq/config.py` & `fedrq-0.7.1/src/fedrq/config.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/src/fedrq/data/releases.toml` & `fedrq-0.7.1/src/fedrq/data/releases.toml`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/src/fedrq/data/repos/almalinux.repo` & `fedrq-0.7.1/src/fedrq/data/repos/almalinux.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/src/fedrq/data/repos/amazonlinux.repo` & `fedrq-0.7.1/src/fedrq/data/repos/amazonlinux.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/src/fedrq/data/repos/centos-stream-compose.repo` & `fedrq-0.7.1/src/fedrq/data/repos/centos-stream-compose.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/src/fedrq/data/repos/centos-stream.repo` & `fedrq-0.7.1/src/fedrq/data/repos/centos-stream.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/src/fedrq/data/repos/centos-stream8-compose.repo` & `fedrq-0.7.1/src/fedrq/data/repos/centos-stream8-compose.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/src/fedrq/data/repos/centos-stream8.repo` & `fedrq-0.7.1/src/fedrq/data/repos/centos-stream8.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/src/fedrq/data/repos/eln.repo` & `fedrq-0.7.1/src/fedrq/data/repos/eln.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/src/fedrq/data/repos/epel.repo` & `fedrq-0.7.1/src/fedrq/data/repos/epel.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/src/fedrq/data/repos/fedora-eln.repo` & `fedrq-0.7.1/src/fedrq/data/repos/fedora-eln.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/src/fedrq/data/repos/fedora-rawhide.repo` & `fedrq-0.7.1/src/fedrq/data/repos/fedora-rawhide.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/src/fedrq/data/repos/fedora-updates-testing.repo` & `fedrq-0.7.1/src/fedrq/data/repos/fedora-updates-testing.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/src/fedrq/data/repos/fedora-updates.repo` & `fedrq-0.7.1/src/fedrq/data/repos/fedora-updates.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/src/fedrq/data/repos/fedora.repo` & `fedrq-0.7.1/src/fedrq/data/repos/fedora.repo`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/src/fedrq/release_repo.py` & `fedrq-0.7.1/src/fedrq/release_repo.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/src/fedrq/repoquery.py` & `fedrq-0.7.1/src/fedrq/repoquery.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/tests/conftest.py` & `fedrq-0.7.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/tests/integration/test_backends.py` & `fedrq-0.7.1/tests/integration/test_backends.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/tests/integration/test_pkgs.py` & `fedrq-0.7.1/tests/integration/test_pkgs.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/tests/integration/test_subpkgs.py` & `fedrq-0.7.1/tests/integration/test_subpkgs.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/tests/integration/test_whatrequires.py` & `fedrq-0.7.1/tests/integration/test_whatrequires.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/tests/integration/test_whatrequires_src.py` & `fedrq-0.7.1/tests/integration/test_whatrequires_src.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/tests/test_data/build.sh` & `fedrq-0.7.1/tests/test_data/build.sh`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/tests/test_data/repos/repo1/specs/e1/packageb.spec` & `fedrq-0.7.1/tests/test_data/repos/repo1/specs/e1/packageb.spec`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/tests/test_data/repos/repo1/specs/packagea.spec` & `fedrq-0.7.1/tests/test_data/repos/repo1/specs/packagea.spec`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/tests/test_data/repos/repo1/specs/packageb.spec` & `fedrq-0.7.1/tests/test_data/repos/repo1/specs/packageb.spec`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/tests/unit/test_checkconfig.py` & `fedrq-0.7.1/tests/unit/test_checkconfig.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/tests/unit/test_command.py` & `fedrq-0.7.1/tests/unit/test_command.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/tests/unit/test_formatters.py` & `fedrq-0.7.1/tests/unit/test_formatters.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/tests/unit/test_pkgs.py` & `fedrq-0.7.1/tests/unit/test_pkgs.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/tests/unit/test_release.py` & `fedrq-0.7.1/tests/unit/test_release.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/tests/unit/test_repolist.py` & `fedrq-0.7.1/tests/unit/test_repolist.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/tests/unit/test_repoquery.py` & `fedrq-0.7.1/tests/unit/test_repoquery.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/tests/unit/test_subbpkgs.py` & `fedrq-0.7.1/tests/unit/test_subbpkgs.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/tests/unit/test_whatrequires.py` & `fedrq-0.7.1/tests/unit/test_whatrequires.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/tests/unit/test_whatrequires_src.py` & `fedrq-0.7.1/tests/unit/test_whatrequires_src.py`

 * *Files identical despite different names*

### Comparing `fedrq-0.7.0/PKG-INFO` & `fedrq-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedrq
-Version: 0.7.0
+Version: 0.7.1
 Summary: fedrq is a tool to query the Fedora and EPEL repositories
 Author-email: Maxwell G <gotmax@e.email>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

