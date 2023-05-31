# Comparing `tmp/wikimedia-spicerack-7.1.0.tar.gz` & `tmp/wikimedia-spicerack-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikimedia-spicerack-7.1.0.tar", last modified: Mon May 15 08:08:23 2023, max compression
+gzip compressed data, was "wikimedia-spicerack-7.2.0.tar", last modified: Wed May 31 13:16:31 2023, max compression
```

## Comparing `wikimedia-spicerack-7.1.0.tar` & `wikimedia-spicerack-7.2.0.tar`

### file list

```diff
@@ -1,275 +1,279 @@
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.860638 wikimedia-spicerack-7.1.0/
--rw-r--r--   0 riccardo   (501) staff       (20)       45 2018-08-06 08:05:22.000000 wikimedia-spicerack-7.1.0/.coveragerc
--rw-r--r--   0 riccardo   (501) staff       (20)       84 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.1.0/.git-blame-ignore-revs
--rw-r--r--   0 riccardo   (501) staff       (20)      292 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.1.0/.gitignore
--rw-r--r--   0 riccardo   (501) staff       (20)       96 2018-08-06 08:05:22.000000 wikimedia-spicerack-7.1.0/.gitreview
--rw-r--r--   0 riccardo   (501) staff       (20)      668 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/.mailmap
--rw-r--r--   0 riccardo   (501) staff       (20)      207 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/.wmfconfig
--rw-r--r--   0 riccardo   (501) staff       (20)   105768 2023-05-15 07:49:19.000000 wikimedia-spicerack-7.1.0/CHANGELOG.rst
--rw-r--r--   0 riccardo   (501) staff       (20)      271 2018-08-06 08:05:22.000000 wikimedia-spicerack-7.1.0/COPYRIGHT
--rw-r--r--   0 riccardo   (501) staff       (20)    34686 2018-08-06 08:05:22.000000 wikimedia-spicerack-7.1.0/LICENSE
--rw-r--r--   0 riccardo   (501) staff       (20)     1691 2023-05-15 08:08:23.860933 wikimedia-spicerack-7.1.0/PKG-INFO
--rw-r--r--   0 riccardo   (501) staff       (20)      443 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.1.0/README.rst
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.239626 wikimedia-spicerack-7.1.0/doc/
--rw-r--r--   0 riccardo   (501) staff       (20)      611 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/doc/Makefile
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.242171 wikimedia-spicerack-7.1.0/doc/examples/
--rw-r--r--   0 riccardo   (501) staff       (20)     1801 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/doc/examples/config.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.270993 wikimedia-spicerack-7.1.0/doc/source/
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.272147 wikimedia-spicerack-7.1.0/doc/source/_static/
--rw-r--r--   0 riccardo   (501) staff       (20)      369 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/doc/source/_static/theme_overrides.css
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.373407 wikimedia-spicerack-7.1.0/doc/source/api/
--rw-r--r--   0 riccardo   (501) staff       (20)     1051 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/doc/source/api/index.rst
--rw-r--r--   0 riccardo   (501) staff       (20)      101 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.administrative.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       54 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.alerting.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       66 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.alertmanager.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       39 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.apt.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       51 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.confctl.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       57 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.constants.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       54 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.cookbook.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       60 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.debmonitor.rst
--rw-r--r--   0 riccardo   (501) staff       (20)      112 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.decorators.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       42 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.dhcp.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       51 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.dnsdisc.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       93 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.elasticsearch_cluster.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       60 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.exceptions.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.ganeti.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.icinga.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       63 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.interactive.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       42 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.ipmi.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       43 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.k8s.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       46 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.kafka.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       57 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.mediawiki.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       45 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.mysql.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       66 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.mysql_legacy.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.netbox.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       57 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.peeringdb.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.puppet.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       51 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.redfish.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       69 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.redis_cluster.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.remote.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       54 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.reposync.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       51 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.service.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       81 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.toolforge.etcdctl.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       57 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.toolforge.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.1.0/doc/source/api/spicerack.typing.rst
--rw-r--r--   0 riccardo   (501) staff       (20)     6769 2023-05-11 12:43:16.000000 wikimedia-spicerack-7.1.0/doc/source/conf.py
--rw-r--r--   0 riccardo   (501) staff       (20)      831 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/doc/source/configuration.rst
--rw-r--r--   0 riccardo   (501) staff       (20)      133 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.1.0/doc/source/cookbook.rst
--rw-r--r--   0 riccardo   (501) staff       (20)     2722 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/doc/source/development.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       44 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/doc/source/docutils.conf
--rw-r--r--   0 riccardo   (501) staff       (20)      384 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.1.0/doc/source/index.rst
--rw-r--r--   0 riccardo   (501) staff       (20)     1227 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/doc/source/installation.rst
--rw-r--r--   0 riccardo   (501) staff       (20)     9572 2023-05-11 12:43:16.000000 wikimedia-spicerack-7.1.0/doc/source/introduction.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       62 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/doc/source/release.rst
--rw-r--r--   0 riccardo   (501) staff       (20)     2078 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/prospector.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)      258 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/pyproject.toml
--rw-r--r--   0 riccardo   (501) staff       (20)      565 2023-05-15 08:08:23.861830 wikimedia-spicerack-7.1.0/setup.cfg
--rwxr-xr-x   0 riccardo   (501) staff       (20)     3281 2023-03-28 16:38:15.000000 wikimedia-spicerack-7.1.0/setup.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.516429 wikimedia-spicerack-7.1.0/spicerack/
--rw-r--r--   0 riccardo   (501) staff       (20)    27623 2023-05-11 12:43:16.000000 wikimedia-spicerack-7.1.0/spicerack/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)    17795 2023-05-11 12:43:06.000000 wikimedia-spicerack-7.1.0/spicerack/_cookbook.py
--rw-r--r--   0 riccardo   (501) staff       (20)     4077 2023-05-11 12:43:16.000000 wikimedia-spicerack-7.1.0/spicerack/_log.py
--rw-r--r--   0 riccardo   (501) staff       (20)    18780 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/_menu.py
--rw-r--r--   0 riccardo   (501) staff       (20)     1442 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/_module_api.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3478 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/administrative.py
--rw-r--r--   0 riccardo   (501) staff       (20)     2769 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/alerting.py
--rw-r--r--   0 riccardo   (501) staff       (20)    12766 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/alertmanager.py
--rw-r--r--   0 riccardo   (501) staff       (20)     5853 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/apt.py
--rw-r--r--   0 riccardo   (501) staff       (20)     8072 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/confctl.py
--rw-r--r--   0 riccardo   (501) staff       (20)      262 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/constants.py
--rw-r--r--   0 riccardo   (501) staff       (20)     5988 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/cookbook.py
--rw-r--r--   0 riccardo   (501) staff       (20)     2141 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/debmonitor.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3949 2023-05-11 12:43:16.000000 wikimedia-spicerack-7.1.0/spicerack/decorators.py
--rw-r--r--   0 riccardo   (501) staff       (20)    10644 2023-05-15 07:49:19.000000 wikimedia-spicerack-7.1.0/spicerack/dhcp.py
--rw-r--r--   0 riccardo   (501) staff       (20)    12124 2023-03-28 16:38:15.000000 wikimedia-spicerack-7.1.0/spicerack/dnsdisc.py
--rw-r--r--   0 riccardo   (501) staff       (20)    30520 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/elasticsearch_cluster.py
--rw-r--r--   0 riccardo   (501) staff       (20)      550 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/exceptions.py
--rw-r--r--   0 riccardo   (501) staff       (20)    13883 2023-05-08 07:16:17.000000 wikimedia-spicerack-7.1.0/spicerack/ganeti.py
--rw-r--r--   0 riccardo   (501) staff       (20)    27163 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/icinga.py
--rw-r--r--   0 riccardo   (501) staff       (20)      848 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/interactive.py
--rw-r--r--   0 riccardo   (501) staff       (20)    10263 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/ipmi.py
--rw-r--r--   0 riccardo   (501) staff       (20)    18466 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/k8s.py
--rw-r--r--   0 riccardo   (501) staff       (20)    14951 2023-04-17 16:31:29.000000 wikimedia-spicerack-7.1.0/spicerack/kafka.py
--rw-r--r--   0 riccardo   (501) staff       (20)    14797 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/mediawiki.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3329 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/mysql.py
--rw-r--r--   0 riccardo   (501) staff       (20)    14945 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/mysql_legacy.py
--rw-r--r--   0 riccardo   (501) staff       (20)    13278 2023-05-15 07:26:54.000000 wikimedia-spicerack-7.1.0/spicerack/netbox.py
--rw-r--r--   0 riccardo   (501) staff       (20)     5157 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/peeringdb.py
--rw-r--r--   0 riccardo   (501) staff       (20)    20891 2023-03-28 16:38:15.000000 wikimedia-spicerack-7.1.0/spicerack/puppet.py
--rw-r--r--   0 riccardo   (501) staff       (20)        0 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/py.typed
--rw-r--r--   0 riccardo   (501) staff       (20)    36793 2023-03-30 15:21:09.000000 wikimedia-spicerack-7.1.0/spicerack/redfish.py
--rw-r--r--   0 riccardo   (501) staff       (20)     6421 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/redis_cluster.py
--rw-r--r--   0 riccardo   (501) staff       (20)    28496 2023-05-15 07:49:19.000000 wikimedia-spicerack-7.1.0/spicerack/remote.py
--rw-r--r--   0 riccardo   (501) staff       (20)     7111 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/reposync.py
--rw-r--r--   0 riccardo   (501) staff       (20)    23081 2023-04-17 16:31:29.000000 wikimedia-spicerack-7.1.0/spicerack/service.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.520395 wikimedia-spicerack-7.1.0/spicerack/tests/
--rw-r--r--   0 riccardo   (501) staff       (20)      871 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/__init__.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.548266 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.551058 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/confctl/
--rw-r--r--   0 riccardo   (501) staff       (20)       33 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/confctl/config.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)      698 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/confctl/schema.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.552149 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/config/
--rw-r--r--   0 riccardo   (501) staff       (20)       59 2020-10-23 11:19:20.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/config/valid.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)       79 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/config.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)      219 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/config_bad_external_modules.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)       44 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/config_empty_base_dirs.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)      216 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/config_external_modules.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)      126 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/config_multiple_base_dirs.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)      113 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/config_wrong_overrides.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.182740 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.576471 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/
--rw-r--r--   0 riccardo   (501) staff       (20)      263 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/__do_not_add_init_py_file_here__
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.615072 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/
--rw-r--r--   0 riccardo   (501) staff       (20)       52 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      953 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/call_another_cookbook.py
--rw-r--r--   0 riccardo   (501) staff       (20)      648 2023-01-11 10:33:35.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/example.py
--rw-r--r--   0 riccardo   (501) staff       (20)      299 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/get_runner_raise.py
--rw-r--r--   0 riccardo   (501) staff       (20)      615 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/multiple.py
--rw-r--r--   0 riccardo   (501) staff       (20)      787 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/rollback.py
--rw-r--r--   0 riccardo   (501) staff       (20)      743 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/rollback_raise.py
--rw-r--r--   0 riccardo   (501) staff       (20)      632 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/runtime_description.py
--rw-r--r--   0 riccardo   (501) staff       (20)      638 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/runtime_description_raise.py
--rw-r--r--   0 riccardo   (501) staff       (20)      697 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/use_external_modules.py
--rw-r--r--   0 riccardo   (501) staff       (20)      438 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/cookbook.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.617489 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group1/
--rw-r--r--   0 riccardo   (501) staff       (20)       49 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group1/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      133 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group1/cookbook1.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.620562 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/
--rw-r--r--   0 riccardo   (501) staff       (20)       29 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      523 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/cookbook2.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.628337 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/subgroup1/
--rw-r--r--   0 riccardo   (501) staff       (20)       39 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/subgroup1/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      143 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/subgroup1/cookbook3.py
--rw-r--r--   0 riccardo   (501) staff       (20)      114 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/zcookbook4.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.665094 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/
--rw-r--r--   0 riccardo   (501) staff       (20)       29 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      267 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/argparse_ok.py
--rw-r--r--   0 riccardo   (501) staff       (20)      368 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/argument_parser_raise_system_exit.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.667574 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/empty_subgroup/
--rw-r--r--   0 riccardo   (501) staff       (20)       46 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/empty_subgroup/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      259 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/get_argument_parser_raise.py
--rw-r--r--   0 riccardo   (501) staff       (20)      274 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/get_argument_parser_raise_system_exit_str.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.669919 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/invalid_subgroup/
--rw-r--r--   0 riccardo   (501) staff       (20)       70 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/invalid_subgroup/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      148 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/invalid_subgroup/skipped.py
--rw-r--r--   0 riccardo   (501) staff       (20)      186 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/invalid_syntax.py
--rw-r--r--   0 riccardo   (501) staff       (20)      162 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/keyboard_interrupt.py
--rw-r--r--   0 riccardo   (501) staff       (20)       44 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/missing_run_function.py
--rw-r--r--   0 riccardo   (501) staff       (20)      144 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/non_zero_exit.py
--rw-r--r--   0 riccardo   (501) staff       (20)      173 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/raise_exception.py
--rw-r--r--   0 riccardo   (501) staff       (20)      154 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/raise_system_exit_0.py
--rw-r--r--   0 riccardo   (501) staff       (20)      164 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/raise_system_exit_9.py
--rw-r--r--   0 riccardo   (501) staff       (20)      170 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/raise_system_exit_str.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.672013 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/subgroup3/
--rw-r--r--   0 riccardo   (501) staff       (20)       39 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/subgroup3/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      143 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/subgroup3/cookbook4.py
--rw-r--r--   0 riccardo   (501) staff       (20)      615 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/multiple.py
--rw-r--r--   0 riccardo   (501) staff       (20)      276 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/root.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.673184 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/debmonitor/
--rw-r--r--   0 riccardo   (501) staff       (20)      109 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/debmonitor/config.ini
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.674479 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/discovery/
--rw-r--r--   0 riccardo   (501) staff       (20)       80 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/discovery/authdns.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.678339 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/elasticsearch/
--rw-r--r--   0 riccardo   (501) staff       (20)       84 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/elasticsearch/config.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.190389 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/external_cookbook/
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.689467 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/external_cookbook/cookbooks/
--rw-r--r--   0 riccardo   (501) staff       (20)      263 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/external_cookbook/cookbooks/__do_not_add_init_py_file_here__
--rw-r--r--   0 riccardo   (501) staff       (20)      456 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/external_cookbook/cookbooks/external_cookbook.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.695569 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/external_cookbook/cookbooks/external_group/
--rw-r--r--   0 riccardo   (501) staff       (20)       57 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/external_cookbook/cookbooks/external_group/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      141 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/external_cookbook/cookbooks/external_group/cookbook1.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.699332 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/external_modules/
--rw-r--r--   0 riccardo   (501) staff       (20)       32 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/external_modules/__init__.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.701750 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/external_modules/spicerack_ext/
--rw-r--r--   0 riccardo   (501) staff       (20)       42 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/external_modules/spicerack_ext/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      396 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/external_modules/spicerack_ext/cool_feature.py
--rw-r--r--   0 riccardo   (501) staff       (20)      695 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/external_modules/spicerack_extender.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.707693 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/ganeti/
--rw-r--r--   0 riccardo   (501) staff       (20)       96 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/ganeti/404.json
--rw-r--r--   0 riccardo   (501) staff       (20)       26 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/ganeti/bogus.json
--rw-r--r--   0 riccardo   (501) staff       (20)       53 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/ganeti/config.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)     8697 2020-11-03 18:42:40.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/ganeti/info.json
--rw-r--r--   0 riccardo   (501) staff       (20)     3398 2020-11-03 18:42:40.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/ganeti/instance.json
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.738736 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/icinga/
--rw-r--r--   0 riccardo   (501) staff       (20)      194 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/icinga/status_downtimed.json
--rw-r--r--   0 riccardo   (501) staff       (20)        4 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/icinga/status_invalid.json
--rw-r--r--   0 riccardo   (501) staff       (20)      214 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/icinga/status_missing.json
--rw-r--r--   0 riccardo   (501) staff       (20)      195 2022-06-06 10:26:19.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/icinga/status_valid.json
--rw-r--r--   0 riccardo   (501) staff       (20)      884 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/icinga/status_with_acknowledged_failures.json
--rw-r--r--   0 riccardo   (501) staff       (20)      884 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/icinga/status_with_acknowledged_warnings.json
--rw-r--r--   0 riccardo   (501) staff       (20)      884 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/icinga/status_with_all_acknowledged_failures.json
--rw-r--r--   0 riccardo   (501) staff       (20)      196 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/icinga/status_with_empty_failed_services.json
--rw-r--r--   0 riccardo   (501) staff       (20)      768 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/icinga/status_with_failed_services.json
--rw-r--r--   0 riccardo   (501) staff       (20)      188 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/icinga/status_with_no_matching_services.json
--rw-r--r--   0 riccardo   (501) staff       (20)      684 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/icinga/status_with_services.json
--rw-r--r--   0 riccardo   (501) staff       (20)      684 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/icinga/status_with_services_downtimed.json
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.740094 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/kafka/
--rw-r--r--   0 riccardo   (501) staff       (20)      347 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/kafka/config.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.741229 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/netbox/
--rw-r--r--   0 riccardo   (501) staff       (20)       82 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/netbox/config.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.749287 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/peeringdb/
--rw-r--r--   0 riccardo   (501) staff       (20)    11449 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/peeringdb/asn.json
--rw-r--r--   0 riccardo   (501) staff       (20)      797 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/peeringdb/ixlan.json
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.754520 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/phabricator/
--rw-r--r--   0 riccardo   (501) staff       (20)      100 2020-10-23 11:21:26.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/phabricator/valid.conf
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.759949 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/redis_cluster/
--rw-r--r--   0 riccardo   (501) staff       (20)      229 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/redis_cluster/cluster.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.767741 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/remote/
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/remote/config.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/remote/config_installer.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.768781 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/reposync/
--rw-r--r--   0 riccardo   (501) staff       (20)       66 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/reposync/config.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.772713 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/service/
--rw-r--r--   0 riccardo   (501) staff       (20)     3273 2023-04-17 16:31:29.000000 wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/service/service.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)     2580 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/sphinx_checker.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.844514 wikimedia-spicerack-7.1.0/spicerack/tests/unit/
--rw-r--r--   0 riccardo   (501) staff       (20)       40 2018-08-25 07:06:49.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)    28172 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test__cookbook.py
--rw-r--r--   0 riccardo   (501) staff       (20)     4775 2023-05-11 12:43:16.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test__log.py
--rw-r--r--   0 riccardo   (501) staff       (20)     2553 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_administrative.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3508 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_alerting.py
--rw-r--r--   0 riccardo   (501) staff       (20)    13229 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_alertmanager.py
--rw-r--r--   0 riccardo   (501) staff       (20)     1957 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_apt.py
--rw-r--r--   0 riccardo   (501) staff       (20)     8651 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_confctl.py
--rw-r--r--   0 riccardo   (501) staff       (20)     2078 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_debmonitor.py
--rw-r--r--   0 riccardo   (501) staff       (20)     5648 2023-05-11 12:43:16.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_decorators.py
--rw-r--r--   0 riccardo   (501) staff       (20)    19551 2023-05-15 07:49:19.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_dhcp.py
--rw-r--r--   0 riccardo   (501) staff       (20)    12139 2023-03-28 16:38:15.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_dnsdisc.py
--rw-r--r--   0 riccardo   (501) staff       (20)    42981 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_elasticsearch_cluster.py
--rw-r--r--   0 riccardo   (501) staff       (20)    15575 2023-05-11 12:43:16.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_ganeti.py
--rw-r--r--   0 riccardo   (501) staff       (20)    39132 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_icinga.py
--rw-r--r--   0 riccardo   (501) staff       (20)    14445 2023-05-11 12:43:16.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_init.py
--rw-r--r--   0 riccardo   (501) staff       (20)     1186 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_interactive.py
--rw-r--r--   0 riccardo   (501) staff       (20)    20462 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_ipmi.py
--rw-r--r--   0 riccardo   (501) staff       (20)    24006 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_k8s.py
--rw-r--r--   0 riccardo   (501) staff       (20)     9470 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_kafka.py
--rw-r--r--   0 riccardo   (501) staff       (20)    11536 2023-03-28 16:38:15.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_mediawiki.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3323 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_mysql.py
--rw-r--r--   0 riccardo   (501) staff       (20)    10535 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_mysql_legacy.py
--rw-r--r--   0 riccardo   (501) staff       (20)    14999 2023-05-12 17:35:57.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_netbox.py
--rw-r--r--   0 riccardo   (501) staff       (20)     4588 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_peeringdb.py
--rw-r--r--   0 riccardo   (501) staff       (20)    34515 2023-03-28 16:38:15.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_puppet.py
--rw-r--r--   0 riccardo   (501) staff       (20)    44515 2023-03-30 15:21:09.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_redfish.py
--rw-r--r--   0 riccardo   (501) staff       (20)     4275 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_redis_cluster.py
--rw-r--r--   0 riccardo   (501) staff       (20)    23896 2023-05-15 07:49:19.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_remote.py
--rw-r--r--   0 riccardo   (501) staff       (20)     5618 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_reposync.py
--rw-r--r--   0 riccardo   (501) staff       (20)    16842 2023-03-28 16:38:16.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_service.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.845851 wikimedia-spicerack-7.1.0/spicerack/tests/unit/toolforge/
--rw-r--r--   0 riccardo   (501) staff       (20)    28976 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/tests/unit/toolforge/test_etcdctl.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3676 2023-04-17 16:31:29.000000 wikimedia-spicerack-7.1.0/spicerack/tests/vulture_whitelist.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.849739 wikimedia-spicerack-7.1.0/spicerack/toolforge/
--rw-r--r--   0 riccardo   (501) staff       (20)       52 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.1.0/spicerack/toolforge/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)     9529 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/toolforge/etcdctl.py
--rw-r--r--   0 riccardo   (501) staff       (20)      299 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.1.0/spicerack/typing.py
--rw-r--r--   0 riccardo   (501) staff       (20)     2374 2023-03-28 16:38:16.000000 wikimedia-spicerack-7.1.0/tox.ini
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.852698 wikimedia-spicerack-7.1.0/utils/
--rwxr-xr-x   0 riccardo   (501) staff       (20)     1174 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/utils/check-style.sh
--rwxr-xr-x   0 riccardo   (501) staff       (20)      452 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.1.0/utils/format-code.sh
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-15 08:08:23.859628 wikimedia-spicerack-7.1.0/wikimedia_spicerack.egg-info/
--rw-r--r--   0 riccardo   (501) staff       (20)     1691 2023-05-15 08:08:22.000000 wikimedia-spicerack-7.1.0/wikimedia_spicerack.egg-info/PKG-INFO
--rw-r--r--   0 riccardo   (501) staff       (20)     9703 2023-05-15 08:08:23.000000 wikimedia-spicerack-7.1.0/wikimedia_spicerack.egg-info/SOURCES.txt
--rw-r--r--   0 riccardo   (501) staff       (20)        1 2023-05-15 08:08:22.000000 wikimedia-spicerack-7.1.0/wikimedia_spicerack.egg-info/dependency_links.txt
--rw-r--r--   0 riccardo   (501) staff       (20)       54 2023-05-15 08:08:22.000000 wikimedia-spicerack-7.1.0/wikimedia_spicerack.egg-info/entry_points.txt
--rw-r--r--   0 riccardo   (501) staff       (20)        1 2023-05-15 08:08:22.000000 wikimedia-spicerack-7.1.0/wikimedia_spicerack.egg-info/not-zip-safe
--rw-r--r--   0 riccardo   (501) staff       (20)      647 2023-05-15 08:08:22.000000 wikimedia-spicerack-7.1.0/wikimedia_spicerack.egg-info/requires.txt
--rw-r--r--   0 riccardo   (501) staff       (20)       10 2023-05-15 08:08:22.000000 wikimedia-spicerack-7.1.0/wikimedia_spicerack.egg-info/top_level.txt
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:31.067338 wikimedia-spicerack-7.2.0/
+-rw-r--r--   0 riccardo   (501) staff       (20)       45 2018-08-06 08:05:22.000000 wikimedia-spicerack-7.2.0/.coveragerc
+-rw-r--r--   0 riccardo   (501) staff       (20)       84 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.2.0/.git-blame-ignore-revs
+-rw-r--r--   0 riccardo   (501) staff       (20)      337 2023-05-31 12:56:46.000000 wikimedia-spicerack-7.2.0/.gitignore
+-rw-r--r--   0 riccardo   (501) staff       (20)       96 2018-08-06 08:05:22.000000 wikimedia-spicerack-7.2.0/.gitreview
+-rw-r--r--   0 riccardo   (501) staff       (20)      668 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/.mailmap
+-rw-r--r--   0 riccardo   (501) staff       (20)      207 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/.wmfconfig
+-rw-r--r--   0 riccardo   (501) staff       (20)   106481 2023-05-31 12:56:46.000000 wikimedia-spicerack-7.2.0/CHANGELOG.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)      271 2018-08-06 08:05:22.000000 wikimedia-spicerack-7.2.0/COPYRIGHT
+-rw-r--r--   0 riccardo   (501) staff       (20)    34686 2018-08-06 08:05:22.000000 wikimedia-spicerack-7.2.0/LICENSE
+-rw-r--r--   0 riccardo   (501) staff       (20)     1691 2023-05-31 13:16:31.067886 wikimedia-spicerack-7.2.0/PKG-INFO
+-rw-r--r--   0 riccardo   (501) staff       (20)      443 2023-05-21 08:23:21.000000 wikimedia-spicerack-7.2.0/README.rst
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:27.994041 wikimedia-spicerack-7.2.0/doc/
+-rw-r--r--   0 riccardo   (501) staff       (20)      611 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.2.0/doc/Makefile
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:27.995874 wikimedia-spicerack-7.2.0/doc/examples/
+-rw-r--r--   0 riccardo   (501) staff       (20)     1801 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/doc/examples/config.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:28.231004 wikimedia-spicerack-7.2.0/doc/source/
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:28.233238 wikimedia-spicerack-7.2.0/doc/source/_static/
+-rw-r--r--   0 riccardo   (501) staff       (20)      369 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.2.0/doc/source/_static/theme_overrides.css
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:28.687563 wikimedia-spicerack-7.2.0/doc/source/api/
+-rw-r--r--   0 riccardo   (501) staff       (20)     1051 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.2.0/doc/source/api/index.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)      101 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/doc/source/api/spicerack.administrative.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       54 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/doc/source/api/spicerack.alerting.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       66 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/doc/source/api/spicerack.alertmanager.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       39 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.2.0/doc/source/api/spicerack.apt.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       51 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.2.0/doc/source/api/spicerack.confctl.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       57 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.2.0/doc/source/api/spicerack.constants.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       54 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.2.0/doc/source/api/spicerack.cookbook.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       60 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.2.0/doc/source/api/spicerack.debmonitor.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)      112 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.2.0/doc/source/api/spicerack.decorators.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       42 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.2.0/doc/source/api/spicerack.dhcp.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       51 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.2.0/doc/source/api/spicerack.dnsdisc.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       93 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.2.0/doc/source/api/spicerack.elasticsearch_cluster.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       60 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.2.0/doc/source/api/spicerack.exceptions.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.2.0/doc/source/api/spicerack.ganeti.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.2.0/doc/source/api/spicerack.icinga.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       63 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.2.0/doc/source/api/spicerack.interactive.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       42 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.2.0/doc/source/api/spicerack.ipmi.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       43 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/doc/source/api/spicerack.k8s.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       46 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/doc/source/api/spicerack.kafka.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       57 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.2.0/doc/source/api/spicerack.mediawiki.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       45 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.2.0/doc/source/api/spicerack.mysql.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       66 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.2.0/doc/source/api/spicerack.mysql_legacy.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.2.0/doc/source/api/spicerack.netbox.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       57 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/doc/source/api/spicerack.peeringdb.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.2.0/doc/source/api/spicerack.puppet.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       51 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/doc/source/api/spicerack.redfish.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       69 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.2.0/doc/source/api/spicerack.redis_cluster.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2021-03-24 13:43:41.000000 wikimedia-spicerack-7.2.0/doc/source/api/spicerack.remote.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       54 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/doc/source/api/spicerack.reposync.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       51 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/doc/source/api/spicerack.service.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       81 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.2.0/doc/source/api/spicerack.toolforge.etcdctl.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       57 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.2.0/doc/source/api/spicerack.toolforge.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.2.0/doc/source/api/spicerack.typing.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)     6769 2023-05-11 12:43:16.000000 wikimedia-spicerack-7.2.0/doc/source/conf.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      831 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.2.0/doc/source/configuration.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)      133 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.2.0/doc/source/cookbook.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)     2722 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/doc/source/development.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       44 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.2.0/doc/source/docutils.conf
+-rw-r--r--   0 riccardo   (501) staff       (20)      384 2022-02-08 17:32:11.000000 wikimedia-spicerack-7.2.0/doc/source/index.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)     1227 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.2.0/doc/source/installation.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)     9572 2023-05-11 12:43:16.000000 wikimedia-spicerack-7.2.0/doc/source/introduction.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       62 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.2.0/doc/source/release.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)     2078 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/prospector.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)      258 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.2.0/pyproject.toml
+-rw-r--r--   0 riccardo   (501) staff       (20)      565 2023-05-31 13:16:31.072483 wikimedia-spicerack-7.2.0/setup.cfg
+-rwxr-xr-x   0 riccardo   (501) staff       (20)     3281 2023-05-30 10:31:39.000000 wikimedia-spicerack-7.2.0/setup.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:29.194397 wikimedia-spicerack-7.2.0/spicerack/
+-rw-r--r--   0 riccardo   (501) staff       (20)    27623 2023-05-11 12:43:16.000000 wikimedia-spicerack-7.2.0/spicerack/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    17795 2023-05-11 12:43:06.000000 wikimedia-spicerack-7.2.0/spicerack/_cookbook.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     4077 2023-05-11 12:43:16.000000 wikimedia-spicerack-7.2.0/spicerack/_log.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    18780 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.2.0/spicerack/_menu.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     1442 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.2.0/spicerack/_module_api.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3478 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.2.0/spicerack/administrative.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     2769 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.2.0/spicerack/alerting.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    12766 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.2.0/spicerack/alertmanager.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     5853 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.2.0/spicerack/apt.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     8072 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.2.0/spicerack/confctl.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      262 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.2.0/spicerack/constants.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     5988 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.2.0/spicerack/cookbook.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     2141 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.2.0/spicerack/debmonitor.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3949 2023-05-11 12:43:16.000000 wikimedia-spicerack-7.2.0/spicerack/decorators.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    11016 2023-05-31 12:56:46.000000 wikimedia-spicerack-7.2.0/spicerack/dhcp.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    12124 2023-03-28 16:38:15.000000 wikimedia-spicerack-7.2.0/spicerack/dnsdisc.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    30520 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.2.0/spicerack/elasticsearch_cluster.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      550 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/exceptions.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    14690 2023-05-31 12:56:46.000000 wikimedia-spicerack-7.2.0/spicerack/ganeti.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    27163 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.2.0/spicerack/icinga.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      848 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.2.0/spicerack/interactive.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    10263 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.2.0/spicerack/ipmi.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    18466 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.2.0/spicerack/k8s.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    14951 2023-04-17 16:31:29.000000 wikimedia-spicerack-7.2.0/spicerack/kafka.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    14797 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.2.0/spicerack/mediawiki.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3329 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.2.0/spicerack/mysql.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    14945 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.2.0/spicerack/mysql_legacy.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    13278 2023-05-15 07:26:54.000000 wikimedia-spicerack-7.2.0/spicerack/netbox.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     5157 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.2.0/spicerack/peeringdb.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    20891 2023-03-28 16:38:15.000000 wikimedia-spicerack-7.2.0/spicerack/puppet.py
+-rw-r--r--   0 riccardo   (501) staff       (20)        0 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/py.typed
+-rw-r--r--   0 riccardo   (501) staff       (20)    36793 2023-03-30 15:21:09.000000 wikimedia-spicerack-7.2.0/spicerack/redfish.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     6421 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.2.0/spicerack/redis_cluster.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    28496 2023-05-15 07:49:19.000000 wikimedia-spicerack-7.2.0/spicerack/remote.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     7111 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.2.0/spicerack/reposync.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    23081 2023-04-17 16:31:29.000000 wikimedia-spicerack-7.2.0/spicerack/service.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:29.200066 wikimedia-spicerack-7.2.0/spicerack/tests/
+-rw-r--r--   0 riccardo   (501) staff       (20)      871 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/__init__.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:29.305449 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:29.319687 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/confctl/
+-rw-r--r--   0 riccardo   (501) staff       (20)       33 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/confctl/config.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)      698 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/confctl/schema.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:29.322322 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/config/
+-rw-r--r--   0 riccardo   (501) staff       (20)       59 2020-10-23 11:19:20.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/config/valid.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)       79 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/config.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)      219 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/config_bad_external_modules.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)       44 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/config_empty_base_dirs.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)      216 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/config_external_modules.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)      126 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/config_multiple_base_dirs.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)      113 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/config_wrong_overrides.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:27.599263 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:29.338056 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/
+-rw-r--r--   0 riccardo   (501) staff       (20)      263 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/__do_not_add_init_py_file_here__
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:29.401242 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/
+-rw-r--r--   0 riccardo   (501) staff       (20)       52 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      953 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/call_another_cookbook.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      648 2023-01-11 10:33:35.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/example.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      299 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/get_runner_raise.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      615 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/multiple.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      787 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/rollback.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      743 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/rollback_raise.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      632 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/runtime_description.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      638 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/runtime_description_raise.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      697 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/use_external_modules.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      438 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/cookbook.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:29.535704 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/group1/
+-rw-r--r--   0 riccardo   (501) staff       (20)       49 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/group1/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      133 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/group1/cookbook1.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:29.605850 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/
+-rw-r--r--   0 riccardo   (501) staff       (20)       29 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      523 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/cookbook2.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:29.626410 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/subgroup1/
+-rw-r--r--   0 riccardo   (501) staff       (20)       39 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/subgroup1/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      143 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/subgroup1/cookbook3.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      114 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/zcookbook4.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:29.825719 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/
+-rw-r--r--   0 riccardo   (501) staff       (20)       29 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      267 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/argparse_ok.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      368 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/argument_parser_raise_system_exit.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:29.831120 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/empty_subgroup/
+-rw-r--r--   0 riccardo   (501) staff       (20)       46 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/empty_subgroup/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      259 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/get_argument_parser_raise.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      274 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/get_argument_parser_raise_system_exit_str.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:29.840879 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/invalid_subgroup/
+-rw-r--r--   0 riccardo   (501) staff       (20)       70 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/invalid_subgroup/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      148 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/invalid_subgroup/skipped.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      186 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/invalid_syntax.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      162 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/keyboard_interrupt.py
+-rw-r--r--   0 riccardo   (501) staff       (20)       44 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/missing_run_function.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      144 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/non_zero_exit.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      173 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/raise_exception.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      154 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/raise_system_exit_0.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      164 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/raise_system_exit_9.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      170 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/raise_system_exit_str.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:29.867462 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/subgroup3/
+-rw-r--r--   0 riccardo   (501) staff       (20)       39 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/subgroup3/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      143 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/group3/subgroup3/cookbook4.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      615 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/multiple.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      276 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/root.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:29.869415 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/debmonitor/
+-rw-r--r--   0 riccardo   (501) staff       (20)      109 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/debmonitor/config.ini
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:29.900843 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/discovery/
+-rw-r--r--   0 riccardo   (501) staff       (20)       80 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/discovery/authdns.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:29.902922 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/elasticsearch/
+-rw-r--r--   0 riccardo   (501) staff       (20)       84 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/elasticsearch/config.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:27.682319 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/external_cookbook/
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:29.925758 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/external_cookbook/cookbooks/
+-rw-r--r--   0 riccardo   (501) staff       (20)      263 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/external_cookbook/cookbooks/__do_not_add_init_py_file_here__
+-rw-r--r--   0 riccardo   (501) staff       (20)      456 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/external_cookbook/cookbooks/external_cookbook.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:29.932007 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/external_cookbook/cookbooks/external_group/
+-rw-r--r--   0 riccardo   (501) staff       (20)       57 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/external_cookbook/cookbooks/external_group/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      141 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/external_cookbook/cookbooks/external_group/cookbook1.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:29.934470 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/external_modules/
+-rw-r--r--   0 riccardo   (501) staff       (20)       32 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/external_modules/__init__.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:30.073402 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/external_modules/spicerack_ext/
+-rw-r--r--   0 riccardo   (501) staff       (20)       42 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/external_modules/spicerack_ext/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      396 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/external_modules/spicerack_ext/cool_feature.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      695 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/external_modules/spicerack_extender.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:30.181062 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/ganeti/
+-rw-r--r--   0 riccardo   (501) staff       (20)       96 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/ganeti/404.json
+-rw-r--r--   0 riccardo   (501) staff       (20)       26 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/ganeti/bogus.json
+-rw-r--r--   0 riccardo   (501) staff       (20)       53 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/ganeti/config.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)       76 2023-05-31 12:56:46.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/ganeti/groups.json
+-rw-r--r--   0 riccardo   (501) staff       (20)     3059 2023-05-31 12:56:46.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/ganeti/groups_bulk.json
+-rw-r--r--   0 riccardo   (501) staff       (20)     8697 2020-11-03 18:42:40.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/ganeti/info.json
+-rw-r--r--   0 riccardo   (501) staff       (20)     3398 2020-11-03 18:42:40.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/ganeti/instance.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      339 2023-05-31 12:56:46.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/ganeti/nodes.json
+-rw-r--r--   0 riccardo   (501) staff       (20)     3817 2023-05-31 12:56:46.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/ganeti/nodes_bulk.json
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:30.382481 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/icinga/
+-rw-r--r--   0 riccardo   (501) staff       (20)      194 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/icinga/status_downtimed.json
+-rw-r--r--   0 riccardo   (501) staff       (20)        4 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/icinga/status_invalid.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      214 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/icinga/status_missing.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      195 2022-06-06 10:26:19.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/icinga/status_valid.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      884 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/icinga/status_with_acknowledged_failures.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      884 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/icinga/status_with_acknowledged_warnings.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      884 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/icinga/status_with_all_acknowledged_failures.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      196 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/icinga/status_with_empty_failed_services.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      768 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/icinga/status_with_failed_services.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      188 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/icinga/status_with_no_matching_services.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      684 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/icinga/status_with_services.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      684 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/icinga/status_with_services_downtimed.json
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:30.398890 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/kafka/
+-rw-r--r--   0 riccardo   (501) staff       (20)      347 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/kafka/config.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:30.465685 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/netbox/
+-rw-r--r--   0 riccardo   (501) staff       (20)       82 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/netbox/config.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:30.482465 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/peeringdb/
+-rw-r--r--   0 riccardo   (501) staff       (20)    11449 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/peeringdb/asn.json
+-rw-r--r--   0 riccardo   (501) staff       (20)      797 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/peeringdb/ixlan.json
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:30.485038 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/phabricator/
+-rw-r--r--   0 riccardo   (501) staff       (20)      100 2020-10-23 11:21:26.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/phabricator/valid.conf
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:30.507763 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/redis_cluster/
+-rw-r--r--   0 riccardo   (501) staff       (20)      229 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/redis_cluster/cluster.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:30.515388 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/remote/
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/remote/config.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2020-08-18 11:01:17.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/remote/config_installer.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:30.531642 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/reposync/
+-rw-r--r--   0 riccardo   (501) staff       (20)       66 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/reposync/config.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:30.532861 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/service/
+-rw-r--r--   0 riccardo   (501) staff       (20)     3273 2023-04-17 16:31:29.000000 wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/service/service.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)     2580 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/sphinx_checker.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:30.898920 wikimedia-spicerack-7.2.0/spicerack/tests/unit/
+-rw-r--r--   0 riccardo   (501) staff       (20)       40 2018-08-25 07:06:49.000000 wikimedia-spicerack-7.2.0/spicerack/tests/unit/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    28172 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.2.0/spicerack/tests/unit/test__cookbook.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     4775 2023-05-11 12:43:16.000000 wikimedia-spicerack-7.2.0/spicerack/tests/unit/test__log.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     2553 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_administrative.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3508 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_alerting.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    13229 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_alertmanager.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     1957 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_apt.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     8651 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_confctl.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     2078 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_debmonitor.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     5648 2023-05-11 12:43:16.000000 wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_decorators.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    20137 2023-05-31 12:56:46.000000 wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_dhcp.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    12139 2023-03-28 16:38:15.000000 wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_dnsdisc.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    42981 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_elasticsearch_cluster.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    17348 2023-05-31 12:56:46.000000 wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_ganeti.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    39132 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_icinga.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    14445 2023-05-11 12:43:16.000000 wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_init.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     1186 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_interactive.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    20462 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_ipmi.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    24006 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_k8s.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     9470 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_kafka.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    11536 2023-03-28 16:38:15.000000 wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_mediawiki.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3323 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_mysql.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    10535 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_mysql_legacy.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    14999 2023-05-12 17:35:57.000000 wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_netbox.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     4588 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_peeringdb.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    34515 2023-03-28 16:38:15.000000 wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_puppet.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    44515 2023-03-30 15:21:09.000000 wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_redfish.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     4275 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_redis_cluster.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    23896 2023-05-15 07:49:19.000000 wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_remote.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     5618 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_reposync.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    16842 2023-03-28 16:38:16.000000 wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_service.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:30.902629 wikimedia-spicerack-7.2.0/spicerack/tests/unit/toolforge/
+-rw-r--r--   0 riccardo   (501) staff       (20)    28976 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.2.0/spicerack/tests/unit/toolforge/test_etcdctl.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3676 2023-04-17 16:31:29.000000 wikimedia-spicerack-7.2.0/spicerack/tests/vulture_whitelist.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:30.969541 wikimedia-spicerack-7.2.0/spicerack/toolforge/
+-rw-r--r--   0 riccardo   (501) staff       (20)       52 2022-02-08 17:32:12.000000 wikimedia-spicerack-7.2.0/spicerack/toolforge/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     9529 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.2.0/spicerack/toolforge/etcdctl.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      299 2023-03-15 15:44:38.000000 wikimedia-spicerack-7.2.0/spicerack/typing.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     2462 2023-05-31 12:56:46.000000 wikimedia-spicerack-7.2.0/tox.ini
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:31.050740 wikimedia-spicerack-7.2.0/utils/
+-rwxr-xr-x   0 riccardo   (501) staff       (20)     1174 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/utils/check-style.sh
+-rwxr-xr-x   0 riccardo   (501) staff       (20)      452 2023-03-14 11:49:21.000000 wikimedia-spicerack-7.2.0/utils/format-code.sh
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-05-31 13:16:31.066536 wikimedia-spicerack-7.2.0/wikimedia_spicerack.egg-info/
+-rw-r--r--   0 riccardo   (501) staff       (20)     1691 2023-05-31 13:16:25.000000 wikimedia-spicerack-7.2.0/wikimedia_spicerack.egg-info/PKG-INFO
+-rw-r--r--   0 riccardo   (501) staff       (20)     9887 2023-05-31 13:16:26.000000 wikimedia-spicerack-7.2.0/wikimedia_spicerack.egg-info/SOURCES.txt
+-rw-r--r--   0 riccardo   (501) staff       (20)        1 2023-05-31 13:16:25.000000 wikimedia-spicerack-7.2.0/wikimedia_spicerack.egg-info/dependency_links.txt
+-rw-r--r--   0 riccardo   (501) staff       (20)       54 2023-05-31 13:16:25.000000 wikimedia-spicerack-7.2.0/wikimedia_spicerack.egg-info/entry_points.txt
+-rw-r--r--   0 riccardo   (501) staff       (20)        1 2023-05-31 13:16:25.000000 wikimedia-spicerack-7.2.0/wikimedia_spicerack.egg-info/not-zip-safe
+-rw-r--r--   0 riccardo   (501) staff       (20)      647 2023-05-31 13:16:25.000000 wikimedia-spicerack-7.2.0/wikimedia_spicerack.egg-info/requires.txt
+-rw-r--r--   0 riccardo   (501) staff       (20)       10 2023-05-31 13:16:25.000000 wikimedia-spicerack-7.2.0/wikimedia_spicerack.egg-info/top_level.txt
```

### Comparing `wikimedia-spicerack-7.1.0/.mailmap` & `wikimedia-spicerack-7.2.0/.mailmap`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/CHANGELOG.rst` & `wikimedia-spicerack-7.2.0/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,28 @@
 Spicerack Changelog
 -------------------
 
+`v7.2.0`_ (2023-05-31)
+^^^^^^^^^^^^^^^^^^^^^^
+
+Minor improvements
+""""""""""""""""""
+
+* ganeti: add new ``GanetiRAPI`` methods ``nodes()`` and ``groups()`` to get the related info from the cluster.
+* ganeti: specify VM memory size in MB to allow for more fine-tune than GB.
+* dhcp: when re-generating the DHCP includes and then restarting the DHCP server, in case of a failure make sure to
+  delete the newly created snippet and refresh again to ensure the DHCP is in a good shape.
+* dhcp: reword some exception messages.
+
+Miscellanea
+"""""""""""
+
+* .gitignore: add local config files to it.
+* Add Python 3.11 support.
+
 `v7.1.0`_ (2023-05-15)
 ^^^^^^^^^^^^^^^^^^^^^^
 
 Minor improvements
 """"""""""""""""""
 
 * dhcp: expand support for hostname based match using the manufacturer to adapt to different settings.
@@ -2597,7 +2615,8 @@
 .. _`v6.3.0`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v6.3.0
 .. _`v6.4.0`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v6.4.0
 .. _`v6.4.1`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v6.4.1
 .. _`v6.4.2`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v6.4.2
 .. _`v6.4.3`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v6.4.3
 .. _`v7.0.0`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v7.0.0
 .. _`v7.1.0`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v7.1.0
+.. _`v7.2.0`: https://github.com/wikimedia/operations-software-spicerack/releases/tag/v7.2.0
```

### Comparing `wikimedia-spicerack-7.1.0/LICENSE` & `wikimedia-spicerack-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/PKG-INFO` & `wikimedia-spicerack-7.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikimedia-spicerack
-Version: 7.1.0
+Version: 7.2.0
 Summary: Automation framework for the WMF production infrastructure
 Home-page: https://github.com/wikimedia/operations-software-spicerack
 Author: Riccardo Coccioli
 Author-email: rcoccioli@wikimedia.org
 License: GPLv3+
 Keywords: wmf,automation,orchestration
 Platform: GNU/Linux
```

### Comparing `wikimedia-spicerack-7.1.0/doc/Makefile` & `wikimedia-spicerack-7.2.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/doc/examples/config.yaml` & `wikimedia-spicerack-7.2.0/doc/examples/config.yaml`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/doc/source/api/index.rst` & `wikimedia-spicerack-7.2.0/doc/source/api/index.rst`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/doc/source/conf.py` & `wikimedia-spicerack-7.2.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/doc/source/configuration.rst` & `wikimedia-spicerack-7.2.0/doc/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/doc/source/development.rst` & `wikimedia-spicerack-7.2.0/doc/source/development.rst`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/doc/source/installation.rst` & `wikimedia-spicerack-7.2.0/doc/source/installation.rst`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/doc/source/introduction.rst` & `wikimedia-spicerack-7.2.0/doc/source/introduction.rst`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/prospector.yaml` & `wikimedia-spicerack-7.2.0/prospector.yaml`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/setup.cfg` & `wikimedia-spicerack-7.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/setup.py` & `wikimedia-spicerack-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/__init__.py` & `wikimedia-spicerack-7.2.0/spicerack/__init__.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/_cookbook.py` & `wikimedia-spicerack-7.2.0/spicerack/_cookbook.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/_log.py` & `wikimedia-spicerack-7.2.0/spicerack/_log.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/_menu.py` & `wikimedia-spicerack-7.2.0/spicerack/_menu.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/_module_api.py` & `wikimedia-spicerack-7.2.0/spicerack/_module_api.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/administrative.py` & `wikimedia-spicerack-7.2.0/spicerack/administrative.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/alerting.py` & `wikimedia-spicerack-7.2.0/spicerack/alerting.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/alertmanager.py` & `wikimedia-spicerack-7.2.0/spicerack/alertmanager.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/apt.py` & `wikimedia-spicerack-7.2.0/spicerack/apt.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/confctl.py` & `wikimedia-spicerack-7.2.0/spicerack/confctl.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/cookbook.py` & `wikimedia-spicerack-7.2.0/spicerack/cookbook.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/debmonitor.py` & `wikimedia-spicerack-7.2.0/spicerack/debmonitor.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/decorators.py` & `wikimedia-spicerack-7.2.0/spicerack/decorators.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/dhcp.py` & `wikimedia-spicerack-7.2.0/spicerack/dhcp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """Provide an interface for manipulating DHCP configuration snippets for our dynamic/temporary DHCP system."""
 
 import base64
+import logging
 import re
 import textwrap
 from abc import ABC, abstractmethod
 from collections.abc import Iterator
 from contextlib import contextmanager
 from dataclasses import dataclass
 from hashlib import sha256
 from ipaddress import IPv4Address
 
 from wmflib.constants import ALL_DATACENTERS
 
 from spicerack.exceptions import SpicerackError
 from spicerack.remote import RemoteExecutionError, RemoteHosts
 
+logger = logging.getLogger(__name__)
 DHCP_TARGET_PATH: str = "/etc/dhcp/automation"
 """The path to the top of the DHCPd automation directory."""
-
 MGMT_HOSTNAME_RE: str = r"\.mgmt\.{dc}\.wmnet"
 """A regular expression when formatted with a `dc` parameter will match a management hostname."""
 
 
 class DHCPError(SpicerackError):
     """Base class for DHCP object errors."""
 
@@ -127,15 +128,15 @@
 
         See Also:
             https://docs.python.org/3/library/dataclasses.html#post-init-processing
 
         """
         mac_pattern = r"[0-9A-Fa-f]{2}(:[0-9A-Fa-f]{2}){5}"
         if re.fullmatch(mac_pattern, self.mac) is None:
-            raise DHCPError(f"Got invalid MAC address {self.mac}, not matching pattern {mac_pattern}")
+            raise DHCPError(f"Invalid MAC address {self.mac}, must match pattern {mac_pattern}.")
 
     @property
     def filename(self) -> str:
         """Return the proposed filename based on this configuration."""
         return f"ttyS{self.ttys}-115200/{self.hostname}.conf"
 
 
@@ -167,17 +168,18 @@
         range {s.ipv4} {s.ipv4};
     }}
     """
 
     def __post_init__(self) -> None:
         """Validate parameters."""
         if self.datacenter not in ALL_DATACENTERS:
-            raise DHCPError(f"invalid datacenter {self.datacenter}")
-        if not re.search(MGMT_HOSTNAME_RE.format(dc=self.datacenter), self.fqdn):
-            raise DHCPError(f"hostname does not look like a valid management hostname: {self.fqdn}")
+            raise DHCPError(f"Invalid datacenter {self.datacenter}, must be one of {ALL_DATACENTERS}.")
+        pattern = MGMT_HOSTNAME_RE.format(dc=self.datacenter)
+        if not re.search(pattern, self.fqdn):
+            raise DHCPError(f"Invalid management FQDN {self.fqdn}, must match {pattern}.")
 
     @property
     def filename(self) -> str:
         """Return the filename that corresponds to this configuration."""
         return f"""mgmt-{self.datacenter}/{self.fqdn}.conf"""
 
     @property
@@ -207,86 +209,90 @@
         self._hosts = hosts
 
     def refresh_dhcp(self) -> None:
         """Regenerate includes on target data center and restart DHCP, or raise if failure at any stage."""
         try:
             self._hosts.run_sync("/usr/local/sbin/dhcpincludes -r commit", print_progress_bars=False)
         except RemoteExecutionError as exc:
-            raise DHCPRestartError("restarting generating dhcp config or restarting dhcpd failed") from exc
+            raise DHCPRestartError("Failed to refresh the DHCP server when running dhcpincludes.") from exc
 
     def push_configuration(self, configuration: DHCPConfiguration) -> None:
         """Push a specified file with specified content to DHCP server and call refresh_dhcp.
 
         Arguments:
             configuration: An instance which provides content and filename for a configuration.
 
         """
-        filename = configuration.filename
+        filename = f"{DHCP_TARGET_PATH}/{configuration.filename}"
         try:
             self._hosts.run_sync(
-                f"/usr/bin/test '!' '-e'  {DHCP_TARGET_PATH}/{filename}",
-                is_safe=True,
-                print_output=False,
-                print_progress_bars=False,
+                f"/usr/bin/test '!' '-e' {filename}", is_safe=True, print_output=False, print_progress_bars=False
             )
         except RemoteExecutionError as exc:
-            raise DHCPError(f"target file {filename} exists") from exc
+            raise DHCPError(
+                f"Snippet {filename} already exists, is there another operation in progress for the same device? "
+                "If not you delete it and retry."
+            ) from exc
 
         b64encoded = base64.b64encode(str(configuration).encode()).decode()
         try:
             self._hosts.run_sync(
-                f"/bin/echo '{b64encoded}' | /usr/bin/base64 -d > {DHCP_TARGET_PATH}/{filename}",
-                print_progress_bars=False,
+                f"/bin/echo '{b64encoded}' | /usr/bin/base64 -d > {filename}", print_progress_bars=False
             )
         except RemoteExecutionError as exc:
-            raise DHCPError(f"target file {filename} failed to be created.") from exc
+            raise DHCPError(f"Failed to create snippet {filename}.") from exc
 
-        self.refresh_dhcp()
+        try:
+            self.refresh_dhcp()
+        except DHCPRestartError:
+            logger.error("Failed to refresh DHCPd, removing snippet {filename} and refreshing again.")
+            self._hosts.run_sync(f"/bin/rm -v {filename}", print_output=False, print_progress_bars=False)
+            self.refresh_dhcp()
+            raise
 
     def remove_configuration(self, configuration: DHCPConfiguration, force: bool = False) -> None:
         """Remove configuration from target DHCP server then call refresh_dhcp.
 
         This will fail if contents do not match unless force is True.
 
         Arguments:
             configuration: An instance which provides content and filename for a configuration.
             force: If set to True, will remove filename regardless.
 
         """
+        filename = f"{DHCP_TARGET_PATH}/{configuration.filename}"
         if not force:
             confsha256 = sha256(str(configuration).encode()).hexdigest()
             try:
                 results = self._hosts.run_sync(
-                    f"sha256sum {DHCP_TARGET_PATH}/{configuration.filename}",
-                    is_safe=True,
-                    print_output=False,
-                    print_progress_bars=False,
+                    f"sha256sum {filename}", is_safe=True, print_output=False, print_progress_bars=False
                 )
             except RemoteExecutionError as exc:
-                raise DHCPError(f"Can't test {configuration.filename} for removal.") from exc
+                raise DHCPError(f"Failed to checksum {filename} for safe removal.") from exc
+
             seen_match = False
             for _, result in RemoteHosts.results_to_list(results):
                 remotesha256 = result.strip().split()[0]
                 if remotesha256 != confsha256 and not self._dry_run:
-                    raise DHCPError(f"Remote {configuration.filename} has a mismatched SHA256, refusing to remove.")
+                    raise DHCPError(f"Remote snippet {filename} has a mismatched SHA256, refusing to remove it.")
                 seen_match = True
+
             if not seen_match:
-                raise DHCPError("Did not get any result trying to get SHA256, refusing to attempt to remove.")
+                raise DHCPError(f"No output when trying to checksum snippet {filename}, refusing to remove it.")
+
         try:
-            self._hosts.run_sync(
-                f"/bin/rm -v {DHCP_TARGET_PATH}/{configuration.filename}", print_output=False, print_progress_bars=False
-            )
+            self._hosts.run_sync(f"/bin/rm -v {filename}", print_output=False, print_progress_bars=False)
         except RemoteExecutionError as exc:
-            raise DHCPError(f"Can't remove {configuration.filename}.") from exc
+            raise DHCPError(f"Failed to remove snippet {filename}.") from exc
 
         self.refresh_dhcp()
 
     @contextmanager
     def config(self, dhcp_config: DHCPConfiguration) -> Iterator[None]:
-        """A context manager to perform actions while the given DHCP config is valid.
+        """A context manager to perform actions while the given DHCP config is active.
 
         Arguments:
              dhcp_config: The DHCP configuration to use.
 
         """
         self.push_configuration(dhcp_config)
         try:
```

### Comparing `wikimedia-spicerack-7.1.0/spicerack/dnsdisc.py` & `wikimedia-spicerack-7.2.0/spicerack/dnsdisc.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/elasticsearch_cluster.py` & `wikimedia-spicerack-7.2.0/spicerack/elasticsearch_cluster.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/exceptions.py` & `wikimedia-spicerack-7.2.0/spicerack/exceptions.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/ganeti.py` & `wikimedia-spicerack-7.2.0/spicerack/ganeti.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Ganeti module."""
 
 import logging
 from dataclasses import dataclass
-from typing import Optional
+from typing import Optional, Union
 
 from requests.auth import HTTPBasicAuth
 from requests.exceptions import RequestException
 from wmflib.requests import http_session
 
 from spicerack.constants import PUPPET_CA_PATH
 from spicerack.exceptions import SpicerackError
@@ -143,14 +143,36 @@
         """
         instance_info = self.fetch_instance(fqdn)
         if "nic.macs" not in instance_info or not instance_info["nic.macs"]:
             raise GanetiError("Can't find any MACs for instance")
 
         return instance_info["nic.macs"][0]
 
+    def groups(self, bulk: bool = False) -> dict:
+        """Get a list of Cluster groups.
+
+        Arguments:
+            bulk: if true set bulk=1 to return detailed information.
+                see https://docs.ganeti.org/docs/ganeti/2.9/html/rapi.html#bulk
+
+        """
+        target = "groups?bulk=1" if bulk else "groups"
+        return self._api_get_request(target)
+
+    def nodes(self, bulk: bool = False) -> dict:
+        """Get a list of Cluster nodes.
+
+        Arguments:
+            bulk: if true set bulk=1 to return detailed information.
+                see https://docs.ganeti.org/docs/ganeti/2.9/html/rapi.html#bulk
+
+        """
+        target = "nodes?bulk=1" if bulk else "nodes"
+        return self._api_get_request(target)
+
 
 class GntInstance:
     """Class that wraps gnt-instance command execution on a Ganeti cluster master host."""
 
     def __init__(self, master: RemoteHosts, cluster: str, instance: str):
         """Initialize the instance.
 
@@ -207,15 +229,15 @@
         logger.info(
             "Removing VM %s in cluster %s. This may take a few minutes.",
             self._instance,
             self._cluster,
         )
         self._master.run_sync(f"gnt-instance remove --shutdown-timeout={shutdown_timeout} --force {self._instance}")
 
-    def add(self, *, group: str, vcpus: int, memory: int, disk: int, link: str) -> None:
+    def add(self, *, group: str, vcpus: int, memory: Union[int, float], disk: int, link: str) -> None:
         """Create the VM for the instance in the Ganeti cluster with the specified characteristic.
 
         Arguments:
             group: the Ganeti group that matches the Datacenter physical row or rack where to allocate the instance.
             vcpus: the number of virtual CPUs to assign to the instance.
             memory: the amount of RAM to assign to the instance in gigabytes.
             disk: the amount of disk to assign to the instance in gigabytes.
@@ -234,25 +256,26 @@
         local_vars = locals()
         for var_label in ("vcpus", "memory", "disk"):
             if local_vars[var_label] <= 0:
                 raise GanetiError(
                     f"Invalid value '{local_vars[var_label]}' for {var_label}, expected positive integer."
                 )
 
+        memory_mb = int(memory * 1024)
         command = (
             "gnt-instance add"
             " -t drbd"
             " -I hail"
             f" --net 0:link={link}"
             " --hypervisor-parameters=kvm:boot_order=network"
             " -o debootstrap+default"
             " --no-install"
             " --no-wait-for-sync"
             f" -g {group}"
-            f" -B vcpus={vcpus},memory={memory}g"
+            f" -B vcpus={vcpus},memory={memory_mb}m"
             f" --disk 0:size={disk}g"
             f" {self._instance}"
         )
 
         logger.info(
             (
                 "Creating VM %s in cluster %s with group=%s vcpus=%d memory=%dGB disk=%dGB link=%s. "
```

### Comparing `wikimedia-spicerack-7.1.0/spicerack/icinga.py` & `wikimedia-spicerack-7.2.0/spicerack/icinga.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/interactive.py` & `wikimedia-spicerack-7.2.0/spicerack/interactive.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/ipmi.py` & `wikimedia-spicerack-7.2.0/spicerack/ipmi.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/k8s.py` & `wikimedia-spicerack-7.2.0/spicerack/k8s.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/kafka.py` & `wikimedia-spicerack-7.2.0/spicerack/kafka.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/mediawiki.py` & `wikimedia-spicerack-7.2.0/spicerack/mediawiki.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/mysql.py` & `wikimedia-spicerack-7.2.0/spicerack/mysql.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/mysql_legacy.py` & `wikimedia-spicerack-7.2.0/spicerack/mysql_legacy.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/netbox.py` & `wikimedia-spicerack-7.2.0/spicerack/netbox.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/peeringdb.py` & `wikimedia-spicerack-7.2.0/spicerack/peeringdb.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/puppet.py` & `wikimedia-spicerack-7.2.0/spicerack/puppet.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/redfish.py` & `wikimedia-spicerack-7.2.0/spicerack/redfish.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/redis_cluster.py` & `wikimedia-spicerack-7.2.0/spicerack/redis_cluster.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/remote.py` & `wikimedia-spicerack-7.2.0/spicerack/remote.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/reposync.py` & `wikimedia-spicerack-7.2.0/spicerack/reposync.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/service.py` & `wikimedia-spicerack-7.2.0/spicerack/service.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/__init__.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/confctl/schema.yaml` & `wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/confctl/schema.yaml`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/call_another_cookbook.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/call_another_cookbook.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/example.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/example.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/multiple.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/multiple.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/rollback.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/rollback.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/rollback_raise.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/rollback_raise.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/runtime_description.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/runtime_description.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/runtime_description_raise.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/runtime_description_raise.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/use_external_modules.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/class_api/use_external_modules.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/cookbook2.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/group2/cookbook2.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/cookbook/cookbooks/multiple.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/cookbook/cookbooks/multiple.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/external_modules/spicerack_extender.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/external_modules/spicerack_extender.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/ganeti/info.json` & `wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/ganeti/info.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/ganeti/instance.json` & `wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/ganeti/instance.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/icinga/status_with_acknowledged_failures.json` & `wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/icinga/status_with_acknowledged_failures.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/icinga/status_with_acknowledged_warnings.json` & `wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/icinga/status_with_acknowledged_warnings.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/icinga/status_with_all_acknowledged_failures.json` & `wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/icinga/status_with_all_acknowledged_failures.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/icinga/status_with_failed_services.json` & `wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/icinga/status_with_failed_services.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/icinga/status_with_services.json` & `wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/icinga/status_with_services.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/icinga/status_with_services_downtimed.json` & `wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/icinga/status_with_services_downtimed.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/peeringdb/asn.json` & `wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/peeringdb/asn.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/peeringdb/ixlan.json` & `wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/peeringdb/ixlan.json`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/fixtures/service/service.yaml` & `wikimedia-spicerack-7.2.0/spicerack/tests/fixtures/service/service.yaml`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/sphinx_checker.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/sphinx_checker.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test__cookbook.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/unit/test__cookbook.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test__log.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/unit/test__log.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_administrative.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_administrative.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_alerting.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_alerting.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_alertmanager.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_alertmanager.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_apt.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_apt.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_confctl.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_confctl.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_debmonitor.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_debmonitor.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_decorators.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_decorators.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_dhcp.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_dhcp.py`

 * *Files 2% similar despite different names*

```diff
@@ -252,15 +252,15 @@
         "01-23-45-67-89-AB",
         "0123.4567.89AB",
         "01-23-45-67-89-AB-CD-EF",
     ),
 )
 def test_dhcp_conf_mac_invalid_mac(mac):
     """It should raise DHCPError if an invalid MAC address is passed."""
-    with pytest.raises(dhcp.DHCPError, match="Got invalid MAC address"):
+    with pytest.raises(dhcp.DHCPError, match="Invalid MAC address"):
         dhcp.DHCPConfMac(hostname="testhost0", ipv4=IPv4Address("10.0.0.1"), mac=mac, ttys=1, distro="bullseye")
 
 
 def test_dhcp_mgmt_fail():
     """A DHCPConfMgmt object should fail to create if invalid parameters are passed to its init."""
     with pytest.raises(dhcp.DHCPError):
         # data center must be a value in ALL_DATACENTERS
@@ -319,15 +319,15 @@
         """Test push_configuration success."""
         config = get_mock_config()
         hosts = self._setup_dhcp_mocks()
 
         self.dhcp.push_configuration(config)
 
         call_test = mock.call(
-            f"/usr/bin/test '!' '-e'  {dhcp.DHCP_TARGET_PATH}/{config.filename}",
+            f"/usr/bin/test '!' '-e' {dhcp.DHCP_TARGET_PATH}/{config.filename}",
             is_safe=True,
             print_output=False,
             print_progress_bars=False,
         )
         call_write = mock.call(
             f"/bin/echo '{config.config_base64}' | /usr/bin/base64 -d > {dhcp.DHCP_TARGET_PATH}/{config.filename}",
             print_progress_bars=False,
@@ -338,25 +338,42 @@
     def test_push_configuration_test_fail(self):
         """Test push_configuration where the file apparently exists."""
         config = get_mock_config()
         self._setup_dhcp_mocks(hosts=get_mock_fail_hosts())
 
         with pytest.raises(dhcp.DHCPError) as exc:
             self.dhcp.push_configuration(config)
-        assert str(exc.value) == f"target file {config.filename} exists"
+        assert "already exists, is there another operation in progress" in str(exc.value)
 
     # - does it deal correctly with echo command failing
     def test_push_configuration_echo_fail(self):
         """Test push_configuration, where writing to the file fails."""
         config = get_mock_config()
         self._setup_dhcp_mocks(hosts=get_mock_suc_fail_hosts())
 
         with pytest.raises(dhcp.DHCPError) as exc:
             self.dhcp.push_configuration(config)
-        assert str(exc.value) == f"target file {config.filename} failed to be created."
+        assert "Failed to create snippet" in str(exc.value)
+
+    def test_push_configuration_refresh_fail(self):
+        """When the call to refresh_dhcp() fails, it should remove the snippet and refresh again."""
+        config = get_mock_config()
+        hosts = get_mock_suc_fail_hosts()
+        hosts.run_sync.side_effect = [
+            "some value",
+            "some value",
+            RemoteExecutionError("mock error", 1, iter(())),
+            "some value",
+            "some value",
+        ]
+        self._setup_dhcp_mocks(hosts=hosts)
+
+        with pytest.raises(dhcp.DHCPRestartError) as exc:
+            self.dhcp.push_configuration(config)
+        assert str(exc.value) == "Failed to refresh the DHCP server when running dhcpincludes."
 
     # test DHCP.remove_configuration
     # - does it deal correctly with succeeding commands
     def test_remove_config(self):
         """Test remove_configuration where everything succeeds."""
         config = get_mock_config()
         hosts = self._setup_dhcp_mocks()
@@ -384,39 +401,39 @@
         config = get_mock_config()
         self._setup_dhcp_mocks()
         with mock.patch("spicerack.dhcp.RemoteHosts") as mock_remotehosts:
             mock_remotehosts.results_to_list.return_value = []
 
             with pytest.raises(dhcp.DHCPError) as exc:
                 self.dhcp.remove_configuration(config)
-            assert str(exc.value) == "Did not get any result trying to get SHA256, refusing to attempt to remove."
+            assert "No output when trying to checksum snippet" in str(exc.value)
 
     # - does it deal with sha256sum failing
     def test_remove_config_sha256_fail(self):
         """Test remove_configuration where sha256sum fails to run."""
         config = get_mock_config()
         self._setup_dhcp_mocks(hosts=get_mock_fail_hosts())
 
         with pytest.raises(dhcp.DHCPError) as exc:
             self.dhcp.remove_configuration(config)
-        assert str(exc.value) == f"Can't test {config.filename} for removal."
+        assert "Failed to checksum" in str(exc.value)
 
     # - does it deal with sha256sum mismatch
     def test_remove_config_sha256_mismatch(self):
         """Test remove_configuration where sha256sum and the locally computed sum mismatch."""
         config = get_mock_config()
         self._setup_dhcp_mocks()
         configsha256 = sha256(str(config).encode()).hexdigest()
         config.__str__.return_value = "different test configuration"
 
         with mock.patch("spicerack.dhcp.RemoteHosts") as mock_remotehosts:
             mock_remotehosts.results_to_list.return_value = [[None, f"{configsha256} {config.filename}"]]
             with pytest.raises(dhcp.DHCPError) as exc:
                 self.dhcp.remove_configuration(config)
-            assert str(exc.value) == f"Remote {config.filename} has a mismatched SHA256, refusing to remove."
+            assert "has a mismatched SHA256, refusing to remove it" in str(exc.value)
 
     # - does it deal with sha256sum mismatch (but force)
     def test_remove_config_sha256_mismatch_force(self):
         """Test remove_configuration where there is a sha256 mismatch but we pass force=True."""
         config = get_mock_config()
         hosts = self._setup_dhcp_mocks()
         configsha256 = sha256(str(config).encode()).hexdigest()
@@ -441,15 +458,15 @@
 
         with mock.patch("spicerack.dhcp.RemoteHosts") as mock_remotehosts:
             configsha256 = sha256(str(config).encode()).hexdigest()
             mock_remotehosts.results_to_list.return_value = [[None, f"{configsha256} {config.filename}"]]
 
             with pytest.raises(dhcp.DHCPError) as exc:
                 self.dhcp.remove_configuration(config)
-            assert str(exc.value) == f"Can't remove {config.filename}."
+            assert "Failed to remove snippet" in str(exc.value)
 
     def test_push_context_manager(self):
         """Test push context manager success."""
         config = get_mock_config()
         hosts = self._setup_dhcp_mocks()
         call_sha256 = mock.call(
             f"sha256sum {dhcp.DHCP_TARGET_PATH}/{config.filename}",
@@ -474,15 +491,15 @@
     # - does it still teardown when an error occurs
     def test_push_context_manager_raise(self):
         """Test push context manager where internal code raises."""
         config = get_mock_config()
         hosts = self._setup_dhcp_mocks()
 
         call_test = mock.call(
-            f"/usr/bin/test '!' '-e'  {dhcp.DHCP_TARGET_PATH}/{config.filename}",
+            f"/usr/bin/test '!' '-e' {dhcp.DHCP_TARGET_PATH}/{config.filename}",
             is_safe=True,
             print_output=False,
             print_progress_bars=False,
         )
         call_write = mock.call(
             f"/bin/echo '{config.config_base64}' | /usr/bin/base64 -d > {dhcp.DHCP_TARGET_PATH}/{config.filename}",
             print_progress_bars=False,
```

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_dnsdisc.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_dnsdisc.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_elasticsearch_cluster.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_elasticsearch_cluster.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_ganeti.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_ganeti.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "sitea": "ganeti01.svc.sitea.example.com",
     "siteb01": "ganeti01.svc.siteb.example.com",
     "siteb02": "ganeti02.svc.siteb.example.com",
     "sitea_test": "ganeti-test01.svc.sitea.example.com",
 }
 
 
-class TestGaneti:
+class TestGaneti:  # pylint: disable=too-many-instance-attributes
     """Ganeti tests class."""
 
     def setup_method(self):
         """Setup test environment."""
         # pylint: disable=attribute-defined-outside-init
         self.remote = mock.MagicMock(spec_set=Remote)
         self.netbox = mock.MagicMock(spec_set=Netbox)
@@ -54,14 +54,22 @@
             self.info = info_json.read()
         with open(get_fixture_path("ganeti", "404.json"), encoding="utf-8") as fourohfour_json:
             self.fourohfour = fourohfour_json.read()
         with open(get_fixture_path("ganeti", "instance.json"), encoding="utf-8") as instance_json:
             self.instance_info = instance_json.read()
         with open(get_fixture_path("ganeti", "bogus.json"), encoding="utf-8") as bogus_json:
             self.bogus_data = bogus_json.read()
+        with open(get_fixture_path("ganeti", "groups.json"), encoding="utf-8") as groups_json:
+            self.groups_data = groups_json.read()
+        with open(get_fixture_path("ganeti", "groups_bulk.json"), encoding="utf-8") as groups_bulk_json:
+            self.groups_bulk_data = groups_bulk_json.read()
+        with open(get_fixture_path("ganeti", "nodes.json"), encoding="utf-8") as nodes_json:
+            self.nodes_data = nodes_json.read()
+        with open(get_fixture_path("ganeti", "nodes_bulk.json"), encoding="utf-8") as nodes_bulk_json:
+            self.nodes_bulk_data = nodes_bulk_json.read()
 
     def _set_requests_mock_for_instance(self, requests_mock, missing_active=False):
         """Set request mock to be 404 on all other clusters."""
         for cluster in TEST_CLUSTERS:
             if cluster == self.cluster and not missing_active:
                 requests_mock.get(self.instance_url, text=self.instance_info)
             else:
@@ -171,14 +179,44 @@
     def test_rapi_instance_valid(self, requests_mock):
         """The MAC returned by RAPI.fetch_instance_mac should match the data returned by the API."""
         rapi = self.ganeti.rapi(self.cluster)
         requests_mock.get(self.instance_url, text=self.instance_info)
         mac = json.loads(self.instance_info)["nic.macs"][0]
         assert mac == rapi.fetch_instance_mac(self.instance)
 
+    @pytest.mark.parametrize("bulk", (True, False))
+    def test_rapi_nodes(self, requests_mock, bulk):
+        """The master property of a RAPI should be the hostname for the master of this cluster."""
+        if bulk:
+            uri = "/nodes?bulk=1"
+            data = self.nodes_bulk_data
+        else:
+            uri = "/nodes"
+            data = self.nodes_data
+        rapi = self.ganeti.rapi(self.cluster)
+        requests_mock.get(self.base_url + uri, text=data)
+
+        nodes = json.loads(data)
+        assert rapi.nodes(bulk) == nodes
+
+    @pytest.mark.parametrize("bulk", (True, False))
+    def test_rapi_groups(self, requests_mock, bulk):
+        """The master property of a RAPI should be the hostname for the master of this cluster."""
+        if bulk:
+            uri = "/groups?bulk=1"
+            data = self.groups_bulk_data
+        else:
+            uri = "/groups"
+            data = self.groups_data
+        requests_mock.get(self.base_url + uri, text=data)
+
+        groups = json.loads(data)
+        rapi = self.ganeti.rapi(self.cluster)
+        assert rapi.groups(bulk) == groups
+
     @pytest.mark.parametrize("cluster", ("", "sitea"))
     def test_instance_ok(self, cluster, requests_mock):
         """It should return an instance of GntInstance for a properly configured cluster."""
         self._set_requests_mock_for_instance(requests_mock)
         requests_mock.get(self.base_url + "/info", text=self.info)
         instance = self.ganeti.instance(self.instance, cluster=cluster)
         assert isinstance(instance, ganeti.GntInstance)
@@ -253,19 +291,19 @@
             (
                 nodeset("ganeti-master.example.com"),
                 MsgTreeElem(b"creation logs", parent=MsgTreeElem()),
             )
         ]
         self.remote.query.return_value.run_sync.return_value = iter(results)
 
-        instance.add(group="row_A", vcpus=2, memory=3, disk=4, link="private")
+        instance.add(group="row_A", vcpus=2, memory=3.1, disk=4, link="private")
 
         self.remote.query.return_value.run_sync.assert_called_once_with(
             "gnt-instance add -t drbd -I hail --net 0:link=private --hypervisor-parameters=kvm:boot_order=network "
-            "-o debootstrap+default --no-install --no-wait-for-sync -g row_A -B vcpus=2,memory=3g --disk 0:size=4g "
+            "-o debootstrap+default --no-install --no-wait-for-sync -g row_A -B vcpus=2,memory=3174m --disk 0:size=4g "
             "test.example.com",
             print_output=True,
         )
 
     @pytest.mark.parametrize(
         "kwargs, exc_message",
         (
```

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_icinga.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_icinga.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_init.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_init.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_interactive.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_interactive.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_ipmi.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_ipmi.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_k8s.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_k8s.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_kafka.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_kafka.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_mediawiki.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_mediawiki.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_mysql.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_mysql.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_mysql_legacy.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_mysql_legacy.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_netbox.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_netbox.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_peeringdb.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_peeringdb.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_puppet.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_puppet.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_redfish.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_redfish.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_redis_cluster.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_redis_cluster.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_remote.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_remote.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_reposync.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_reposync.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/unit/test_service.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/unit/test_service.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/unit/toolforge/test_etcdctl.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/unit/toolforge/test_etcdctl.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/tests/vulture_whitelist.py` & `wikimedia-spicerack-7.2.0/spicerack/tests/vulture_whitelist.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/spicerack/toolforge/etcdctl.py` & `wikimedia-spicerack-7.2.0/spicerack/toolforge/etcdctl.py`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/tox.ini` & `wikimedia-spicerack-7.2.0/tox.ini`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tox]
 minversion = 3.10.0
-envlist = py{39,310}-{flake8,unit,bandit,mypy,prospector,sphinx},py{39,310}-style
+envlist = py{39,310,311}-{flake8,unit,bandit,mypy,prospector,sphinx},py{39,310,311}-style
 skip_missing_interpreters = True
 
 
 [testenv]
 usedevelop = True
 download = True
 allowlist_externals =
@@ -19,20 +19,22 @@
     bandit: Security-oriented static analyzer
     mypy: Static analyzer for type annotations
     prospector: Static analysis multi-tool
     sphinx: Build documentation and manpages
     py3: (Python 3)
     py39: (Python 3.9)
     py310: (Python 3.10)
+    py311: (Python 3.11)
 envdir =
     prospector: {toxworkdir}/{envname}
     !py3-style: {toxworkdir}/{envname}
     py3: {toxworkdir}/py3-tests
     py39-!prospector-!style: {toxworkdir}/py39-tests
     py310-!prospector-!style: {toxworkdir}/py310-tests
+    py311-!prospector-!style: {toxworkdir}/py311-tests
 commands =
     flake8: flake8 setup.py spicerack
     style: {toxinidir}/utils/check-style.sh
     format: {toxinidir}/utils/format-code.sh
     unit: py.test --strict-markers --cov-report=term-missing --cov=spicerack spicerack/tests/unit {posargs}
     # Skip some bandit issues:
     # - assert_used (B101) in tests
```

### Comparing `wikimedia-spicerack-7.1.0/utils/check-style.sh` & `wikimedia-spicerack-7.2.0/utils/check-style.sh`

 * *Files identical despite different names*

### Comparing `wikimedia-spicerack-7.1.0/wikimedia_spicerack.egg-info/PKG-INFO` & `wikimedia-spicerack-7.2.0/wikimedia_spicerack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikimedia-spicerack
-Version: 7.1.0
+Version: 7.2.0
 Summary: Automation framework for the WMF production infrastructure
 Home-page: https://github.com/wikimedia/operations-software-spicerack
 Author: Riccardo Coccioli
 Author-email: rcoccioli@wikimedia.org
 License: GPLv3+
 Keywords: wmf,automation,orchestration
 Platform: GNU/Linux
```

### Comparing `wikimedia-spicerack-7.1.0/wikimedia_spicerack.egg-info/SOURCES.txt` & `wikimedia-spicerack-7.2.0/wikimedia_spicerack.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -157,16 +157,20 @@
 spicerack/tests/fixtures/external_modules/__init__.py
 spicerack/tests/fixtures/external_modules/spicerack_extender.py
 spicerack/tests/fixtures/external_modules/spicerack_ext/__init__.py
 spicerack/tests/fixtures/external_modules/spicerack_ext/cool_feature.py
 spicerack/tests/fixtures/ganeti/404.json
 spicerack/tests/fixtures/ganeti/bogus.json
 spicerack/tests/fixtures/ganeti/config.yaml
+spicerack/tests/fixtures/ganeti/groups.json
+spicerack/tests/fixtures/ganeti/groups_bulk.json
 spicerack/tests/fixtures/ganeti/info.json
 spicerack/tests/fixtures/ganeti/instance.json
+spicerack/tests/fixtures/ganeti/nodes.json
+spicerack/tests/fixtures/ganeti/nodes_bulk.json
 spicerack/tests/fixtures/icinga/status_downtimed.json
 spicerack/tests/fixtures/icinga/status_invalid.json
 spicerack/tests/fixtures/icinga/status_missing.json
 spicerack/tests/fixtures/icinga/status_valid.json
 spicerack/tests/fixtures/icinga/status_with_acknowledged_failures.json
 spicerack/tests/fixtures/icinga/status_with_acknowledged_warnings.json
 spicerack/tests/fixtures/icinga/status_with_all_acknowledged_failures.json
```

### Comparing `wikimedia-spicerack-7.1.0/wikimedia_spicerack.egg-info/requires.txt` & `wikimedia-spicerack-7.2.0/wikimedia_spicerack.egg-info/requires.txt`

 * *Files identical despite different names*

