# Comparing `tmp/gbp-0.9.8.tar.gz` & `tmp/gbp-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gbp-0.9.8.tar", last modified: Tue Apr  3 11:25:26 2018, max compression
+gzip compressed data, was "dist/gbp-0.9.9.tar", last modified: Mon May 21 13:12:33 2018, max compression
```

## Comparing `gbp-0.9.8.tar` & `gbp-0.9.9.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 agx       (1000) agx       (1000)        0 2018-04-03 11:25:26.000000 gbp-0.9.8/
-drwxr-xr-x   0 agx       (1000) agx       (1000)        0 2018-04-03 11:25:26.000000 gbp-0.9.8/gbp/
-drwxr-xr-x   0 agx       (1000) agx       (1000)        0 2018-04-03 11:25:26.000000 gbp-0.9.8/gbp/scripts/
--rw-r--r--   0 agx       (1000) agx       (1000)    18005 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/scripts/rpm_ch.py
--rw-r--r--   0 agx       (1000) agx       (1000)      775 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/scripts/__init__.py
--rwxr-xr-x   0 agx       (1000) agx       (1000)    25842 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/scripts/buildpackage.py
--rw-r--r--   0 agx       (1000) agx       (1000)     4048 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/scripts/supercommand.py
--rwxr-xr-x   0 agx       (1000) agx       (1000)    15666 2018-04-03 11:06:01.000000 gbp-0.9.8/gbp/scripts/export_orig.py
--rwxr-xr-x   0 agx       (1000) agx       (1000)     4080 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/scripts/config.py
--rw-r--r--   0 agx       (1000) agx       (1000)    22386 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/scripts/import_orig.py
--rw-r--r--   0 agx       (1000) agx       (1000)     4487 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/scripts/pristine_tar.py
--rwxr-xr-x   0 agx       (1000) agx       (1000)     6553 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/scripts/push.py
--rwxr-xr-x   0 agx       (1000) agx       (1000)     6028 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/scripts/tag.py
--rwxr-xr-x   0 agx       (1000) agx       (1000)    17811 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/scripts/pq_rpm.py
--rwxr-xr-x   0 agx       (1000) agx       (1000)    18937 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/scripts/pq.py
--rw-r--r--   0 agx       (1000) agx       (1000)    20939 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/scripts/import_dsc.py
--rw-r--r--   0 agx       (1000) agx       (1000)    29833 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/scripts/buildpackage_rpm.py
--rwxr-xr-x   0 agx       (1000) agx       (1000)     7908 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/scripts/pull.py
--rwxr-xr-x   0 agx       (1000) agx       (1000)     8210 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/scripts/clone.py
--rw-r--r--   0 agx       (1000) agx       (1000)    13037 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/scripts/create_remote_repo.py
--rw-r--r--   0 agx       (1000) agx       (1000)    25387 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/scripts/dch.py
-drwxr-xr-x   0 agx       (1000) agx       (1000)        0 2018-04-03 11:25:26.000000 gbp-0.9.8/gbp/scripts/common/
--rw-r--r--   0 agx       (1000) agx       (1000)     2344 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/scripts/common/__init__.py
--rw-r--r--   0 agx       (1000) agx       (1000)     3819 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/scripts/common/buildpackage.py
--rw-r--r--   0 agx       (1000) agx       (1000)     6223 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/scripts/common/import_orig.py
--rw-r--r--   0 agx       (1000) agx       (1000)     1431 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/scripts/common/hook.py
--rw-r--r--   0 agx       (1000) agx       (1000)     1126 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/scripts/common/repo_setup.py
--rw-r--r--   0 agx       (1000) agx       (1000)    12635 2018-04-03 11:04:51.000000 gbp-0.9.8/gbp/scripts/common/pq.py
--rwxr-xr-x   0 agx       (1000) agx       (1000)    21584 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/scripts/import_srpm.py
--rw-r--r--   0 agx       (1000) agx       (1000)     6545 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/scripts/import_dscs.py
--rw-r--r--   0 agx       (1000) agx       (1000)     3175 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/tristate.py
--rwxr-xr-x   0 agx       (1000) agx       (1000)      898 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/__init__.py
-drwxr-xr-x   0 agx       (1000) agx       (1000)        0 2018-04-03 11:25:26.000000 gbp-0.9.8/gbp/rpm/
--rw-r--r--   0 agx       (1000) agx       (1000)    41312 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/rpm/__init__.py
--rw-r--r--   0 agx       (1000) agx       (1000)     8075 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/rpm/policy.py
--rw-r--r--   0 agx       (1000) agx       (1000)     5840 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/rpm/linkedlist.py
--rw-r--r--   0 agx       (1000) agx       (1000)     4042 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/rpm/git.py
--rw-r--r--   0 agx       (1000) agx       (1000)     9311 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/rpm/changelog.py
--rw-r--r--   0 agx       (1000) agx       (1000)     1624 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/rpm/lib_rpm.py
--rw-r--r--   0 agx       (1000) agx       (1000)     1042 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/paths.py
--rw-r--r--   0 agx       (1000) agx       (1000)    12387 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/patch_series.py
--rw-r--r--   0 agx       (1000) agx       (1000)    34522 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/config.py
--rw-r--r--   0 agx       (1000) agx       (1000)     1766 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/tmpfile.py
--rw-r--r--   0 agx       (1000) agx       (1000)     2018 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/notifications.py
--rw-r--r--   0 agx       (1000) agx       (1000)     5873 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/log.py
-drwxr-xr-x   0 agx       (1000) agx       (1000)        0 2018-04-03 11:25:26.000000 gbp-0.9.8/gbp/git/
--rw-r--r--   0 agx       (1000) agx       (1000)     2131 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/git/__init__.py
--rw-r--r--   0 agx       (1000) agx       (1000)    73595 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/git/repository.py
--rw-r--r--   0 agx       (1000) agx       (1000)     1528 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/git/commit.py
--rw-r--r--   0 agx       (1000) agx       (1000)     2414 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/git/vfs.py
--rw-r--r--   0 agx       (1000) agx       (1000)     4709 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/git/fastimport.py
--rw-r--r--   0 agx       (1000) agx       (1000)     3134 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/git/args.py
--rw-r--r--   0 agx       (1000) agx       (1000)      871 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/git/errors.py
--rw-r--r--   0 agx       (1000) agx       (1000)     5425 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/git/modifier.py
-drwxr-xr-x   0 agx       (1000) agx       (1000)        0 2018-04-03 11:25:26.000000 gbp-0.9.8/gbp/pkg/
--rw-r--r--   0 agx       (1000) agx       (1000)     1207 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/pkg/__init__.py
--rw-r--r--   0 agx       (1000) agx       (1000)     2348 2018-04-03 11:06:01.000000 gbp-0.9.8/gbp/pkg/compressor.py
--rw-r--r--   0 agx       (1000) agx       (1000)     4915 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/pkg/git.py
--rw-r--r--   0 agx       (1000) agx       (1000)     6251 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/pkg/pkgpolicy.py
--rw-r--r--   0 agx       (1000) agx       (1000)     4086 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/pkg/pristinetar.py
--rw-r--r--   0 agx       (1000) agx       (1000)     3158 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/pkg/archive.py
--rw-r--r--   0 agx       (1000) agx       (1000)     6424 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/pkg/upstreamsource.py
--rw-r--r--   0 agx       (1000) agx       (1000)    12677 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/command_wrappers.py
--rw-r--r--   0 agx       (1000) agx       (1000)      972 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/errors.py
--rw-r--r--   0 agx       (1000) agx       (1000)     2429 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/format.py
--rw-r--r--   0 agx       (1000) agx       (1000)     5131 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/dch.py
--rw-r--r--   0 agx       (1000) agx       (1000)       55 2018-04-03 11:25:26.000000 gbp-0.9.8/gbp/version.py
-drwxr-xr-x   0 agx       (1000) agx       (1000)        0 2018-04-03 11:25:26.000000 gbp-0.9.8/gbp/deb/
--rw-r--r--   0 agx       (1000) agx       (1000)     4110 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/deb/__init__.py
--rw-r--r--   0 agx       (1000) agx       (1000)     4132 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/deb/policy.py
--rw-r--r--   0 agx       (1000) agx       (1000)     6843 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/deb/uscan.py
--rw-r--r--   0 agx       (1000) agx       (1000)    14505 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/deb/git.py
--rw-r--r--   0 agx       (1000) agx       (1000)     2393 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/deb/control.py
--rw-r--r--   0 agx       (1000) agx       (1000)     5121 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/deb/source.py
--rw-r--r--   0 agx       (1000) agx       (1000)     2804 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/deb/pristinetar.py
--rw-r--r--   0 agx       (1000) agx       (1000)    11597 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/deb/changelog.py
--rw-r--r--   0 agx       (1000) agx       (1000)     5969 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/deb/dscfile.py
--rw-r--r--   0 agx       (1000) agx       (1000)     5051 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/deb/rollbackgit.py
--rw-r--r--   0 agx       (1000) agx       (1000)     2034 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/deb/upstreamsource.py
--rw-r--r--   0 agx       (1000) agx       (1000)     3492 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp/deb/format.py
--rw-r--r--   0 agx       (1000) agx       (1000)     1721 2018-04-03 11:25:26.000000 gbp-0.9.8/PKG-INFO
-drwxr-xr-x   0 agx       (1000) agx       (1000)        0 2018-04-03 11:25:26.000000 gbp-0.9.8/bin/
--rwxr-xr-x   0 agx       (1000) agx       (1000)     2424 2018-03-16 12:00:14.000000 gbp-0.9.8/bin/gbp-builder-mock
--rwxr-xr-x   0 agx       (1000) agx       (1000)    23144 2018-03-16 12:00:14.000000 gbp-0.9.8/bin/git-pbuilder
--rwxr-xr-x   0 agx       (1000) agx       (1000)     2821 2018-03-16 12:00:14.000000 gbp-0.9.8/setup.py
--rw-r--r--   0 agx       (1000) agx       (1000)      208 2018-04-03 11:25:26.000000 gbp-0.9.8/setup.cfg
--rw-r--r--   0 agx       (1000) agx       (1000)     4425 2018-03-16 12:00:14.000000 gbp-0.9.8/gbp.conf
--rw-r--r--   0 agx       (1000) agx       (1000)      984 2018-03-16 12:00:14.000000 gbp-0.9.8/README.md
-drwxr-xr-x   0 agx       (1000) agx       (1000)        0 2018-04-03 11:25:26.000000 gbp-0.9.8/gbp.egg-info/
--rw-r--r--   0 agx       (1000) agx       (1000)     1768 2018-04-03 11:25:26.000000 gbp-0.9.8/gbp.egg-info/SOURCES.txt
--rw-r--r--   0 agx       (1000) agx       (1000)     1721 2018-04-03 11:25:26.000000 gbp-0.9.8/gbp.egg-info/PKG-INFO
--rw-r--r--   0 agx       (1000) agx       (1000)        4 2018-04-03 11:25:26.000000 gbp-0.9.8/gbp.egg-info/top_level.txt
--rw-r--r--   0 agx       (1000) agx       (1000)       63 2018-04-03 11:25:26.000000 gbp-0.9.8/gbp.egg-info/entry_points.txt
--rw-r--r--   0 agx       (1000) agx       (1000)        1 2018-04-03 11:25:26.000000 gbp-0.9.8/gbp.egg-info/dependency_links.txt
--rw-r--r--   0 agx       (1000) agx       (1000)       16 2018-04-03 11:25:26.000000 gbp-0.9.8/gbp.egg-info/requires.txt
+drwxr-xr-x   0 agx       (1000) agx       (1000)        0 2018-05-21 13:12:33.000000 gbp-0.9.9/
+drwxr-xr-x   0 agx       (1000) agx       (1000)        0 2018-05-21 13:12:33.000000 gbp-0.9.9/gbp/
+drwxr-xr-x   0 agx       (1000) agx       (1000)        0 2018-05-21 13:12:33.000000 gbp-0.9.9/gbp/scripts/
+-rw-r--r--   0 agx       (1000) agx       (1000)    18005 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/scripts/rpm_ch.py
+-rw-r--r--   0 agx       (1000) agx       (1000)      775 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/scripts/__init__.py
+-rwxr-xr-x   0 agx       (1000) agx       (1000)    25842 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/scripts/buildpackage.py
+-rw-r--r--   0 agx       (1000) agx       (1000)     4048 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/scripts/supercommand.py
+-rwxr-xr-x   0 agx       (1000) agx       (1000)    15666 2018-04-03 11:06:01.000000 gbp-0.9.9/gbp/scripts/export_orig.py
+-rwxr-xr-x   0 agx       (1000) agx       (1000)     4048 2018-04-26 07:35:47.000000 gbp-0.9.9/gbp/scripts/config.py
+-rw-r--r--   0 agx       (1000) agx       (1000)    22386 2018-04-23 09:08:21.000000 gbp-0.9.9/gbp/scripts/import_orig.py
+-rw-r--r--   0 agx       (1000) agx       (1000)     4487 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/scripts/pristine_tar.py
+-rwxr-xr-x   0 agx       (1000) agx       (1000)     6553 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/scripts/push.py
+-rwxr-xr-x   0 agx       (1000) agx       (1000)     6028 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/scripts/tag.py
+-rwxr-xr-x   0 agx       (1000) agx       (1000)    17811 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/scripts/pq_rpm.py
+-rwxr-xr-x   0 agx       (1000) agx       (1000)    18937 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/scripts/pq.py
+-rw-r--r--   0 agx       (1000) agx       (1000)    20939 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/scripts/import_dsc.py
+-rw-r--r--   0 agx       (1000) agx       (1000)    29833 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/scripts/buildpackage_rpm.py
+-rwxr-xr-x   0 agx       (1000) agx       (1000)     7908 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/scripts/pull.py
+-rwxr-xr-x   0 agx       (1000) agx       (1000)     8210 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/scripts/clone.py
+-rw-r--r--   0 agx       (1000) agx       (1000)    13037 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/scripts/create_remote_repo.py
+-rw-r--r--   0 agx       (1000) agx       (1000)    25387 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/scripts/dch.py
+drwxr-xr-x   0 agx       (1000) agx       (1000)        0 2018-05-21 13:12:33.000000 gbp-0.9.9/gbp/scripts/common/
+-rw-r--r--   0 agx       (1000) agx       (1000)     2344 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/scripts/common/__init__.py
+-rw-r--r--   0 agx       (1000) agx       (1000)     3819 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/scripts/common/buildpackage.py
+-rw-r--r--   0 agx       (1000) agx       (1000)     6223 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/scripts/common/import_orig.py
+-rw-r--r--   0 agx       (1000) agx       (1000)     1431 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/scripts/common/hook.py
+-rw-r--r--   0 agx       (1000) agx       (1000)     1126 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/scripts/common/repo_setup.py
+-rw-r--r--   0 agx       (1000) agx       (1000)    12635 2018-04-03 11:04:51.000000 gbp-0.9.9/gbp/scripts/common/pq.py
+-rwxr-xr-x   0 agx       (1000) agx       (1000)    21584 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/scripts/import_srpm.py
+-rw-r--r--   0 agx       (1000) agx       (1000)     6545 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/scripts/import_dscs.py
+-rw-r--r--   0 agx       (1000) agx       (1000)     3175 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/tristate.py
+-rwxr-xr-x   0 agx       (1000) agx       (1000)      898 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/__init__.py
+drwxr-xr-x   0 agx       (1000) agx       (1000)        0 2018-05-21 13:12:33.000000 gbp-0.9.9/gbp/rpm/
+-rw-r--r--   0 agx       (1000) agx       (1000)    41312 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/rpm/__init__.py
+-rw-r--r--   0 agx       (1000) agx       (1000)     8075 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/rpm/policy.py
+-rw-r--r--   0 agx       (1000) agx       (1000)     5840 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/rpm/linkedlist.py
+-rw-r--r--   0 agx       (1000) agx       (1000)     4042 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/rpm/git.py
+-rw-r--r--   0 agx       (1000) agx       (1000)     9311 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/rpm/changelog.py
+-rw-r--r--   0 agx       (1000) agx       (1000)     1624 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/rpm/lib_rpm.py
+-rw-r--r--   0 agx       (1000) agx       (1000)     1042 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/paths.py
+-rw-r--r--   0 agx       (1000) agx       (1000)    12387 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/patch_series.py
+-rw-r--r--   0 agx       (1000) agx       (1000)    34522 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/config.py
+-rw-r--r--   0 agx       (1000) agx       (1000)     1766 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/tmpfile.py
+-rw-r--r--   0 agx       (1000) agx       (1000)     2018 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/notifications.py
+-rw-r--r--   0 agx       (1000) agx       (1000)     5873 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/log.py
+drwxr-xr-x   0 agx       (1000) agx       (1000)        0 2018-05-21 13:12:33.000000 gbp-0.9.9/gbp/git/
+-rw-r--r--   0 agx       (1000) agx       (1000)     2131 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/git/__init__.py
+-rw-r--r--   0 agx       (1000) agx       (1000)    73595 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/git/repository.py
+-rw-r--r--   0 agx       (1000) agx       (1000)     1528 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/git/commit.py
+-rw-r--r--   0 agx       (1000) agx       (1000)     2414 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/git/vfs.py
+-rw-r--r--   0 agx       (1000) agx       (1000)     4709 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/git/fastimport.py
+-rw-r--r--   0 agx       (1000) agx       (1000)     3134 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/git/args.py
+-rw-r--r--   0 agx       (1000) agx       (1000)      871 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/git/errors.py
+-rw-r--r--   0 agx       (1000) agx       (1000)     5425 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/git/modifier.py
+drwxr-xr-x   0 agx       (1000) agx       (1000)        0 2018-05-21 13:12:33.000000 gbp-0.9.9/gbp/pkg/
+-rw-r--r--   0 agx       (1000) agx       (1000)     1207 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/pkg/__init__.py
+-rw-r--r--   0 agx       (1000) agx       (1000)     2348 2018-04-03 11:06:01.000000 gbp-0.9.9/gbp/pkg/compressor.py
+-rw-r--r--   0 agx       (1000) agx       (1000)     4915 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/pkg/git.py
+-rw-r--r--   0 agx       (1000) agx       (1000)     6251 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/pkg/pkgpolicy.py
+-rw-r--r--   0 agx       (1000) agx       (1000)     4086 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/pkg/pristinetar.py
+-rw-r--r--   0 agx       (1000) agx       (1000)     3158 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/pkg/archive.py
+-rw-r--r--   0 agx       (1000) agx       (1000)     6424 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/pkg/upstreamsource.py
+-rw-r--r--   0 agx       (1000) agx       (1000)    12677 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/command_wrappers.py
+-rw-r--r--   0 agx       (1000) agx       (1000)      972 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/errors.py
+-rw-r--r--   0 agx       (1000) agx       (1000)     2429 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/format.py
+-rw-r--r--   0 agx       (1000) agx       (1000)     5131 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/dch.py
+-rw-r--r--   0 agx       (1000) agx       (1000)       55 2018-05-21 13:12:33.000000 gbp-0.9.9/gbp/version.py
+drwxr-xr-x   0 agx       (1000) agx       (1000)        0 2018-05-21 13:12:33.000000 gbp-0.9.9/gbp/deb/
+-rw-r--r--   0 agx       (1000) agx       (1000)     4110 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/deb/__init__.py
+-rw-r--r--   0 agx       (1000) agx       (1000)     4132 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/deb/policy.py
+-rw-r--r--   0 agx       (1000) agx       (1000)     6843 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/deb/uscan.py
+-rw-r--r--   0 agx       (1000) agx       (1000)    14676 2018-04-23 09:29:46.000000 gbp-0.9.9/gbp/deb/git.py
+-rw-r--r--   0 agx       (1000) agx       (1000)     2393 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/deb/control.py
+-rw-r--r--   0 agx       (1000) agx       (1000)     5121 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/deb/source.py
+-rw-r--r--   0 agx       (1000) agx       (1000)     2804 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/deb/pristinetar.py
+-rw-r--r--   0 agx       (1000) agx       (1000)    11597 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/deb/changelog.py
+-rw-r--r--   0 agx       (1000) agx       (1000)     5969 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/deb/dscfile.py
+-rw-r--r--   0 agx       (1000) agx       (1000)     5051 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/deb/rollbackgit.py
+-rw-r--r--   0 agx       (1000) agx       (1000)     2034 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/deb/upstreamsource.py
+-rw-r--r--   0 agx       (1000) agx       (1000)     3492 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp/deb/format.py
+-rw-r--r--   0 agx       (1000) agx       (1000)     1721 2018-05-21 13:12:33.000000 gbp-0.9.9/PKG-INFO
+drwxr-xr-x   0 agx       (1000) agx       (1000)        0 2018-05-21 13:12:33.000000 gbp-0.9.9/bin/
+-rwx------   0 agx       (1000) agx       (1000)     2423 2018-05-15 05:52:34.000000 gbp-0.9.9/bin/gbp-builder-mock
+-rwxr-xr-x   0 agx       (1000) agx       (1000)    23144 2018-03-16 12:00:14.000000 gbp-0.9.9/bin/git-pbuilder
+-rwxr-xr-x   0 agx       (1000) agx       (1000)     2821 2018-03-16 12:00:14.000000 gbp-0.9.9/setup.py
+-rw-r--r--   0 agx       (1000) agx       (1000)      208 2018-05-21 13:12:33.000000 gbp-0.9.9/setup.cfg
+-rw-r--r--   0 agx       (1000) agx       (1000)     4425 2018-03-16 12:00:14.000000 gbp-0.9.9/gbp.conf
+-rw-r--r--   0 agx       (1000) agx       (1000)      984 2018-03-16 12:00:14.000000 gbp-0.9.9/README.md
+drwxr-xr-x   0 agx       (1000) agx       (1000)        0 2018-05-21 13:12:33.000000 gbp-0.9.9/gbp.egg-info/
+-rw-r--r--   0 agx       (1000) agx       (1000)     1768 2018-05-21 13:12:33.000000 gbp-0.9.9/gbp.egg-info/SOURCES.txt
+-rw-r--r--   0 agx       (1000) agx       (1000)     1721 2018-05-21 13:12:33.000000 gbp-0.9.9/gbp.egg-info/PKG-INFO
+-rw-r--r--   0 agx       (1000) agx       (1000)        4 2018-05-21 13:12:33.000000 gbp-0.9.9/gbp.egg-info/top_level.txt
+-rw-r--r--   0 agx       (1000) agx       (1000)       63 2018-05-21 13:12:33.000000 gbp-0.9.9/gbp.egg-info/entry_points.txt
+-rw-r--r--   0 agx       (1000) agx       (1000)        1 2018-05-21 13:12:33.000000 gbp-0.9.9/gbp.egg-info/dependency_links.txt
+-rw-r--r--   0 agx       (1000) agx       (1000)       16 2018-05-21 13:12:33.000000 gbp-0.9.9/gbp.egg-info/requires.txt
```

### Comparing `gbp-0.9.8/gbp/scripts/rpm_ch.py` & `gbp-0.9.9/gbp/scripts/rpm_ch.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/scripts/__init__.py` & `gbp-0.9.9/gbp/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/scripts/buildpackage.py` & `gbp-0.9.9/gbp/scripts/buildpackage.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/scripts/supercommand.py` & `gbp-0.9.9/gbp/scripts/supercommand.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/scripts/export_orig.py` & `gbp-0.9.9/gbp/scripts/export_orig.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/scripts/config.py` & `gbp-0.9.9/gbp/scripts/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         parser.parse_config_files()
     return parser
 
 
 def print_single_option(parser, option, printer):
     value = parser.get_config_file_value(option)
     if value is not None:
-        printer("%s.%s=%s" % (parser.command, option, value))
+        printer("%s" % value)
     else:
         return 2
     return 0
 
 
 def print_all_options(parser, printer):
     if not parser.valid_options:
```

### Comparing `gbp-0.9.8/gbp/scripts/import_orig.py` & `gbp-0.9.9/gbp/scripts/import_orig.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/scripts/pristine_tar.py` & `gbp-0.9.9/gbp/scripts/pristine_tar.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/scripts/push.py` & `gbp-0.9.9/gbp/scripts/push.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/scripts/tag.py` & `gbp-0.9.9/gbp/scripts/tag.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/scripts/pq_rpm.py` & `gbp-0.9.9/gbp/scripts/pq_rpm.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/scripts/pq.py` & `gbp-0.9.9/gbp/scripts/pq.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/scripts/import_dsc.py` & `gbp-0.9.9/gbp/scripts/import_dsc.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/scripts/buildpackage_rpm.py` & `gbp-0.9.9/gbp/scripts/buildpackage_rpm.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/scripts/pull.py` & `gbp-0.9.9/gbp/scripts/pull.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/scripts/clone.py` & `gbp-0.9.9/gbp/scripts/clone.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/scripts/create_remote_repo.py` & `gbp-0.9.9/gbp/scripts/create_remote_repo.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/scripts/dch.py` & `gbp-0.9.9/gbp/scripts/dch.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/scripts/common/__init__.py` & `gbp-0.9.9/gbp/scripts/common/__init__.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/scripts/common/buildpackage.py` & `gbp-0.9.9/gbp/scripts/common/buildpackage.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/scripts/common/import_orig.py` & `gbp-0.9.9/gbp/scripts/common/import_orig.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/scripts/common/hook.py` & `gbp-0.9.9/gbp/scripts/common/hook.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/scripts/common/repo_setup.py` & `gbp-0.9.9/gbp/scripts/common/repo_setup.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/scripts/common/pq.py` & `gbp-0.9.9/gbp/scripts/common/pq.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/scripts/import_srpm.py` & `gbp-0.9.9/gbp/scripts/import_srpm.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/scripts/import_dscs.py` & `gbp-0.9.9/gbp/scripts/import_dscs.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/tristate.py` & `gbp-0.9.9/gbp/tristate.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/__init__.py` & `gbp-0.9.9/gbp/__init__.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/rpm/__init__.py` & `gbp-0.9.9/gbp/rpm/__init__.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/rpm/policy.py` & `gbp-0.9.9/gbp/rpm/policy.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/rpm/linkedlist.py` & `gbp-0.9.9/gbp/rpm/linkedlist.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/rpm/git.py` & `gbp-0.9.9/gbp/rpm/git.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/rpm/changelog.py` & `gbp-0.9.9/gbp/rpm/changelog.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/rpm/lib_rpm.py` & `gbp-0.9.9/gbp/rpm/lib_rpm.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/paths.py` & `gbp-0.9.9/gbp/paths.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/patch_series.py` & `gbp-0.9.9/gbp/patch_series.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/config.py` & `gbp-0.9.9/gbp/config.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/tmpfile.py` & `gbp-0.9.9/gbp/tmpfile.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/notifications.py` & `gbp-0.9.9/gbp/notifications.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/log.py` & `gbp-0.9.9/gbp/log.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/git/__init__.py` & `gbp-0.9.9/gbp/git/__init__.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/git/repository.py` & `gbp-0.9.9/gbp/git/repository.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/git/commit.py` & `gbp-0.9.9/gbp/git/commit.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/git/vfs.py` & `gbp-0.9.9/gbp/git/vfs.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/git/fastimport.py` & `gbp-0.9.9/gbp/git/fastimport.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/git/args.py` & `gbp-0.9.9/gbp/git/args.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/git/errors.py` & `gbp-0.9.9/gbp/git/errors.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/git/modifier.py` & `gbp-0.9.9/gbp/git/modifier.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/pkg/__init__.py` & `gbp-0.9.9/gbp/pkg/__init__.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/pkg/compressor.py` & `gbp-0.9.9/gbp/pkg/compressor.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/pkg/git.py` & `gbp-0.9.9/gbp/pkg/git.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/pkg/pkgpolicy.py` & `gbp-0.9.9/gbp/pkg/pkgpolicy.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/pkg/pristinetar.py` & `gbp-0.9.9/gbp/pkg/pristinetar.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/pkg/archive.py` & `gbp-0.9.9/gbp/pkg/archive.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/pkg/upstreamsource.py` & `gbp-0.9.9/gbp/pkg/upstreamsource.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/command_wrappers.py` & `gbp-0.9.9/gbp/command_wrappers.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/errors.py` & `gbp-0.9.9/gbp/errors.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/format.py` & `gbp-0.9.9/gbp/format.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/dch.py` & `gbp-0.9.9/gbp/dch.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/deb/__init__.py` & `gbp-0.9.9/gbp/deb/__init__.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/deb/policy.py` & `gbp-0.9.9/gbp/deb/policy.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/deb/uscan.py` & `gbp-0.9.9/gbp/deb/uscan.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/deb/git.py` & `gbp-0.9.9/gbp/deb/git.py`

 * *Files 2% similar despite different names*

```diff
@@ -363,13 +363,17 @@
         except Exception as e:
             raise GitRepositoryError("Error creating %s: %s" % (output, e))
         return True
 
     def vcs_tag_parent(self, vcs_tag_format, version):
         """If linking to the upstream VCS get the commit id"""
         if vcs_tag_format:
-            return [self.rev_parse("%s^{}" % self.version_to_tag(vcs_tag_format, version))],
+            try:
+                tag = "%s^{}" % self.version_to_tag(vcs_tag_format, version)
+                return [self.rev_parse(tag)]
+            except GitRepositoryError:
+                raise GitRepositoryError("Can't find upstream vcs tag at '%s'" % tag)
         else:
             return None
 
 
 # vim:et:ts=4:sw=4:et:sts=4:ai:set list listchars=tab\:»·,trail\:·:
```

### Comparing `gbp-0.9.8/gbp/deb/control.py` & `gbp-0.9.9/gbp/deb/control.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/deb/source.py` & `gbp-0.9.9/gbp/deb/source.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/deb/pristinetar.py` & `gbp-0.9.9/gbp/deb/pristinetar.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/deb/changelog.py` & `gbp-0.9.9/gbp/deb/changelog.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/deb/dscfile.py` & `gbp-0.9.9/gbp/deb/dscfile.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/deb/rollbackgit.py` & `gbp-0.9.9/gbp/deb/rollbackgit.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/deb/upstreamsource.py` & `gbp-0.9.9/gbp/deb/upstreamsource.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp/deb/format.py` & `gbp-0.9.9/gbp/deb/format.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/PKG-INFO` & `gbp-0.9.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: gbp
-Version: 0.9.8
+Version: 0.9.9
 Summary: Suite to help with Debian packages in Git repositories
 Home-page: https://honk.sigxcpu.org/piki/projects/git-buildpackage/
 Author: Guido Günther
 Author-email: agx@sigxcpu.org
 License: GPLv2+
 Description: Git-buildpackage
         ----------------
```

### Comparing `gbp-0.9.8/bin/gbp-builder-mock` & `gbp-0.9.9/bin/gbp-builder-mock`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program; if not, please see
 #  <http://www.gnu.org/licenses/>
 #
 #  Copyright (C) 2015 Tzafrir Cohen
-#            (C) 2015 Guido Günther
+#            (C) 2015 Guido Gunther
 
 set -e
 
 # There must be a saner way to do that or a reason why this is not required
 fix_arch() {
 	GBP_BUILDER_MOCK_ARCH=${GBP_BUILDER_MOCK_ARCH:-`uname -m`}
 	case "$ARCH" in
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `gbp-0.9.8/bin/git-pbuilder` & `gbp-0.9.9/bin/git-pbuilder`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/setup.py` & `gbp-0.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp.conf` & `gbp-0.9.9/gbp.conf`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/README.md` & `gbp-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp.egg-info/SOURCES.txt` & `gbp-0.9.9/gbp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gbp-0.9.8/gbp.egg-info/PKG-INFO` & `gbp-0.9.9/gbp.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: gbp
-Version: 0.9.8
+Version: 0.9.9
 Summary: Suite to help with Debian packages in Git repositories
 Home-page: https://honk.sigxcpu.org/piki/projects/git-buildpackage/
 Author: Guido Günther
 Author-email: agx@sigxcpu.org
 License: GPLv2+
 Description: Git-buildpackage
         ----------------
```

