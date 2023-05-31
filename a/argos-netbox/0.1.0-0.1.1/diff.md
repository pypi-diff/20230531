# Comparing `tmp/argos_netbox-0.1.0.tar.gz` & `tmp/argos_netbox-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argos_netbox-0.1.0.tar", last modified: Tue May 30 15:30:18 2023, max compression
+gzip compressed data, was "argos_netbox-0.1.1.tar", last modified: Wed May 31 14:03:56 2023, max compression
```

## Comparing `argos_netbox-0.1.0.tar` & `argos_netbox-0.1.1.tar`

### file list

```diff
@@ -1,140 +1,140 @@
--rw-r--r--   0        0        0      364 2023-05-30 15:25:26.391006 argos_netbox-0.1.0/README.md
--rw-r--r--   0        0        0        7 2023-03-06 08:38:06.442789 argos_netbox-0.1.0/argos/README.md
--rw-r--r--   0        0        0      325 2023-04-17 14:45:17.442482 argos_netbox-0.1.0/argos/__init__.py
--rw-r--r--   0        0        0        0 2023-03-10 10:20:09.691802 argos_netbox-0.1.0/argos/api/__init__.py
--rw-r--r--   0        0        0     6272 2023-05-26 06:59:58.819656 argos_netbox-0.1.0/argos/api/serializers.py
--rw-r--r--   0        0        0      545 2023-05-26 06:59:58.820538 argos_netbox-0.1.0/argos/api/urls.py
--rw-r--r--   0        0        0      976 2023-05-26 06:59:58.824307 argos_netbox-0.1.0/argos/api/views.py
--rw-r--r--   0        0        0      382 2023-03-15 22:15:20.607472 argos_netbox-0.1.0/argos/filtersets.py
--rw-r--r--   0        0        0     4601 2023-05-26 06:59:58.824827 argos_netbox-0.1.0/argos/forms.py
--rw-r--r--   0        0        0     1772 2023-05-26 06:59:58.825345 argos_netbox-0.1.0/argos/graphql.py
--rw-r--r--   0        0        0       36 2023-05-14 13:01:57.587396 argos_netbox-0.1.0/argos/migrations/.mypy_cache/.gitignore
--rw-r--r--   0        0        0        2 2023-05-14 13:01:57.582314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/@plugins_snapshot.json
--rw-r--r--   0        0        0   190035 2023-05-14 13:01:57.524313 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/_ast.data.json
--rw-r--r--   0        0        0     1775 2023-05-14 13:01:57.525315 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/_ast.meta.json
--rw-r--r--   0        0        0    61715 2023-05-14 13:01:57.516313 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/_codecs.data.json
--rw-r--r--   0        0        0     1821 2023-05-14 13:01:57.518314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/_codecs.meta.json
--rw-r--r--   0        0        0    19501 2023-05-14 13:01:57.513313 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/_collections_abc.data.json
--rw-r--r--   0        0        0     1729 2023-05-14 13:01:57.514313 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/_collections_abc.meta.json
--rw-r--r--   0        0        0     7729 2023-05-14 13:01:57.510313 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/_ctypes.data.json
--rw-r--r--   0        0        0     1731 2023-05-14 13:01:57.512313 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/_ctypes.meta.json
--rw-r--r--   0        0        0    92896 2023-05-14 13:01:57.508314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1832 2023-05-14 13:01:57.509315 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0    67142 2023-05-14 13:01:57.504314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/_winapi.data.json
--rw-r--r--   0        0        0     1804 2023-05-14 13:01:57.505313 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/_winapi.meta.json
--rw-r--r--   0        0        0    21692 2023-05-14 13:01:57.500312 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/abc.data.json
--rw-r--r--   0        0        0     1717 2023-05-14 13:01:57.501313 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/abc.meta.json
--rw-r--r--   0        0        0    62974 2023-05-14 13:01:57.497384 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/array.data.json
--rw-r--r--   0        0        0     1784 2023-05-14 13:01:57.498312 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/array.meta.json
--rw-r--r--   0        0        0  1147461 2023-05-14 13:01:57.558313 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/builtins.data.json
--rw-r--r--   0        0        0     1881 2023-05-14 13:01:57.559313 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/builtins.meta.json
--rw-r--r--   0        0        0   127544 2023-05-14 13:01:57.493313 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/codecs.data.json
--rw-r--r--   0        0        0     1821 2023-05-14 13:01:57.493313 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/codecs.meta.json
--rw-r--r--   0        0        0   390750 2023-05-14 13:01:57.487312 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/collections/__init__.data.json
--rw-r--r--   0        0        0     1800 2023-05-14 13:01:57.488313 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/collections/__init__.meta.json
--rw-r--r--   0        0        0     4044 2023-05-14 13:01:57.474316 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/collections/abc.data.json
--rw-r--r--   0        0        0     1696 2023-05-14 13:01:57.475314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/collections/abc.meta.json
--rw-r--r--   0        0        0   115814 2023-05-14 13:01:57.472313 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/contextlib.data.json
--rw-r--r--   0        0        0     1772 2023-05-14 13:01:57.472313 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/contextlib.meta.json
--rw-r--r--   0        0        0   144027 2023-05-14 13:01:57.467383 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1828 2023-05-14 13:01:57.468313 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     8126 2023-05-14 13:01:57.461314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/email/__init__.data.json
--rw-r--r--   0        0        0     1757 2023-05-14 13:01:57.462314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/email/__init__.meta.json
--rw-r--r--   0        0        0    12853 2023-05-14 13:01:57.458313 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/email/charset.data.json
--rw-r--r--   0        0        0     1693 2023-05-14 13:01:57.459314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/email/charset.meta.json
--rw-r--r--   0        0        0     7713 2023-05-14 13:01:57.456315 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/email/contentmanager.data.json
--rw-r--r--   0        0        0     1728 2023-05-14 13:01:57.457369 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25497 2023-05-14 13:01:57.454314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/email/errors.data.json
--rw-r--r--   0        0        0     1700 2023-05-14 13:01:57.455314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/email/errors.meta.json
--rw-r--r--   0        0        0     9703 2023-05-14 13:01:57.451313 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/email/header.data.json
--rw-r--r--   0        0        0     1713 2023-05-14 13:01:57.452313 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/email/header.meta.json
--rw-r--r--   0        0        0    62361 2023-05-14 13:01:57.449314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/email/message.data.json
--rw-r--r--   0        0        0     1850 2023-05-14 13:01:57.450313 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/email/message.meta.json
--rw-r--r--   0        0        0    32702 2023-05-14 13:01:57.445312 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/email/policy.data.json
--rw-r--r--   0        0        0     1786 2023-05-14 13:01:57.446313 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/email/policy.meta.json
--rw-r--r--   0        0        0    95101 2023-05-14 13:01:57.441314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/enum.data.json
--rw-r--r--   0        0        0     1749 2023-05-14 13:01:57.443313 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/enum.meta.json
--rw-r--r--   0        0        0    23882 2023-05-14 13:01:57.436314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/genericpath.data.json
--rw-r--r--   0        0        0     1746 2023-05-14 13:01:57.437378 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/genericpath.meta.json
--rw-r--r--   0        0        0     6520 2023-05-14 13:01:57.433314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/importlib/__init__.data.json
--rw-r--r--   0        0        0     1731 2023-05-14 13:01:57.434314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/importlib/__init__.meta.json
--rw-r--r--   0        0        0    73613 2023-05-14 13:01:57.430314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/importlib/abc.data.json
--rw-r--r--   0        0        0     1879 2023-05-14 13:01:57.431313 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/importlib/abc.meta.json
--rw-r--r--   0        0        0    68149 2023-05-14 13:01:57.425315 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/importlib/machinery.data.json
--rw-r--r--   0        0        0     1890 2023-05-14 13:01:57.426313 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/importlib/machinery.meta.json
--rw-r--r--   0        0        0    95589 2023-05-14 13:01:57.421314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1869 2023-05-14 13:01:57.422315 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    12491 2023-05-14 13:01:57.417314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1714 2023-05-14 13:01:57.418313 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0    88673 2023-05-14 13:01:57.414314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/io.data.json
--rw-r--r--   0        0        0     1840 2023-05-14 13:01:57.415313 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/io.meta.json
--rw-r--r--   0        0        0    24368 2023-05-14 13:01:57.409313 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/mmap.data.json
--rw-r--r--   0        0        0     1756 2023-05-14 13:01:57.410312 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/mmap.meta.json
--rw-r--r--   0        0        0    15200 2023-05-14 13:01:57.406313 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/ntpath.data.json
--rw-r--r--   0        0        0     1768 2023-05-14 13:01:57.407373 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/ntpath.meta.json
--rw-r--r--   0        0        0   248783 2023-05-14 13:01:57.403312 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/os/__init__.data.json
--rw-r--r--   0        0        0     1899 2023-05-14 13:01:57.405314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/os/__init__.meta.json
--rw-r--r--   0        0        0     5311 2023-05-14 13:01:57.394317 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/os/path.data.json
--rw-r--r--   0        0        0     1685 2023-05-14 13:01:57.395314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/os/path.meta.json
--rw-r--r--   0        0        0    90374 2023-05-14 13:01:57.390314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/pathlib.data.json
--rw-r--r--   0        0        0     1849 2023-05-14 13:01:57.392313 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/pathlib.meta.json
--rw-r--r--   0        0        0    47610 2023-05-14 13:01:57.384314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/pickle.data.json
--rw-r--r--   0        0        0     1785 2023-05-14 13:01:57.386314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/pickle.meta.json
--rw-r--r--   0        0        0    80910 2023-05-14 13:01:57.380314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/posixpath.data.json
--rw-r--r--   0        0        0     1779 2023-05-14 13:01:57.381316 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/posixpath.meta.json
--rw-r--r--   0        0        0   151627 2023-05-14 13:01:57.375314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/re.data.json
--rw-r--r--   0        0        0     1871 2023-05-14 13:01:57.377373 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/re.meta.json
--rw-r--r--   0        0        0    15014 2023-05-14 13:01:57.369314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/sre_compile.data.json
--rw-r--r--   0        0        0     1715 2023-05-14 13:01:57.370314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/sre_compile.meta.json
--rw-r--r--   0        0        0    29571 2023-05-14 13:01:57.366314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/sre_constants.data.json
--rw-r--r--   0        0        0     1699 2023-05-14 13:01:57.368315 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/sre_constants.meta.json
--rw-r--r--   0        0        0    52535 2023-05-14 13:01:57.363314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/sre_parse.data.json
--rw-r--r--   0        0        0     1779 2023-05-14 13:01:57.365313 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/sre_parse.meta.json
--rw-r--r--   0        0        0   181048 2023-05-14 13:01:57.359313 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/subprocess.data.json
--rw-r--r--   0        0        0     1859 2023-05-14 13:01:57.360314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/subprocess.meta.json
--rw-r--r--   0        0        0   168592 2023-05-14 13:01:57.351314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/sys.data.json
--rw-r--r--   0        0        0     1818 2023-05-14 13:01:57.353315 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/sys.meta.json
--rw-r--r--   0        0        0   254573 2023-05-14 13:01:57.345313 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/types.data.json
--rw-r--r--   0        0        0     1790 2023-05-14 13:01:57.346312 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/types.meta.json
--rw-r--r--   0        0        0   446716 2023-05-14 13:01:57.336313 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/typing.data.json
--rw-r--r--   0        0        0     1857 2023-05-14 13:01:57.337460 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/typing.meta.json
--rw-r--r--   0        0        0    54822 2023-05-14 13:01:57.320394 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/typing_extensions.data.json
--rw-r--r--   0        0        0     1780 2023-05-14 13:01:57.321394 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/typing_extensions.meta.json
--rw-r--r--   0        0        0     1528 2023-05-14 13:01:57.564314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/work/__init__.data.json
--rw-r--r--   0        0        0     1564 2023-05-14 13:01:57.565313 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/work/__init__.meta.json
--rw-r--r--   0        0        0     1381 2023-05-14 13:01:57.566969 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/work/school_projects.data.json
--rw-r--r--   0        0        0     1521 2023-05-14 13:01:57.567314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/work/school_projects.meta.json
--rw-r--r--   0        0        0     1424 2023-05-14 13:01:57.569314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/work/school_projects/argos.data.json
--rw-r--r--   0        0        0     1534 2023-05-14 13:01:57.570315 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/work/school_projects/argos.meta.json
--rw-r--r--   0        0        0     1523 2023-05-14 13:01:57.571314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin.data.json
--rw-r--r--   0        0        0     1563 2023-05-14 13:01:57.572316 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin.meta.json
--rw-r--r--   0        0        0     5506 2023-05-14 13:01:57.580315 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/__init__.data.json
--rw-r--r--   0        0        0     1738 2023-05-14 13:01:57.581314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/__init__.meta.json
--rw-r--r--   0        0        0     4680 2023-05-14 13:01:57.576315 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/migrations/0002_alter_bgp_mesh_options.data.json
--rw-r--r--   0        0        0     1740 2023-05-14 13:01:57.577314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/migrations/0002_alter_bgp_mesh_options.meta.json
--rw-r--r--   0        0        0     1955 2023-05-14 13:01:57.573314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/migrations/__init__.data.json
--rw-r--r--   0        0        0     1673 2023-05-14 13:01:57.574314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/migrations/__init__.meta.json
--rw-r--r--   0        0        0     1904 2023-05-14 13:01:57.562314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/version.data.json
--rw-r--r--   0        0        0     1658 2023-05-14 13:01:57.563314 argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/version.meta.json
--rw-r--r--   0        0        0      193 2023-05-14 13:01:57.591313 argos_netbox-0.1.0/argos/migrations/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     8947 2023-05-26 06:59:58.826346 argos_netbox-0.1.0/argos/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-04-16 19:09:07.716532 argos_netbox-0.1.0/argos/migrations/__init__.py
--rw-r--r--   0        0        0     6889 2023-05-30 08:20:54.913874 argos_netbox-0.1.0/argos/models.py
--rw-r--r--   0        0        0     2412 2023-05-26 06:59:58.827113 argos_netbox-0.1.0/argos/navigation.py
--rw-r--r--   0        0        0        0 2023-05-03 18:43:56.972393 argos_netbox-0.1.0/argos/requirements.txt
--rw-r--r--   0        0        0     3334 2023-05-30 08:20:54.913874 argos_netbox-0.1.0/argos/tables.py
--rw-r--r--   0        0        0     1810 2023-05-10 23:28:50.063751 argos_netbox-0.1.0/argos/templates/argos/address_family.html
--rw-r--r--   0        0        0     1067 2023-05-10 23:28:50.064752 argos_netbox-0.1.0/argos/templates/argos/address_family_edit.html
--rw-r--r--   0        0        0     1249 2023-05-26 06:59:58.829034 argos_netbox-0.1.0/argos/templates/argos/bgp_ce.html
--rw-r--r--   0        0        0     2510 2023-05-10 23:28:50.065752 argos_netbox-0.1.0/argos/templates/argos/bgp_mesh.html
--rw-r--r--   0        0        0     1852 2023-05-26 06:59:58.829985 argos_netbox-0.1.0/argos/templates/argos/bgp_pe.html
--rw-r--r--   0        0        0     1421 2023-05-30 08:20:54.914876 argos_netbox-0.1.0/argos/templates/argos/ldp.html
--rw-r--r--   0        0        0     1148 2023-05-05 12:10:51.465373 argos_netbox-0.1.0/argos/templates/argos/ldp_edit.html
--rw-r--r--   0        0        0     1328 2023-05-26 06:59:58.829985 argos_netbox-0.1.0/argos/templates/argos/mpls_instance.html
--rw-r--r--   0        0        0      680 2023-05-10 23:28:50.066751 argos_netbox-0.1.0/argos/templates/argos/util/hide_if_checked.html
--rw-r--r--   0        0        0      319 2023-05-10 23:28:50.067752 argos_netbox-0.1.0/argos/templatetags/argos_macros.py
--rw-r--r--   0        0        0     3925 2023-05-26 06:59:58.830994 argos_netbox-0.1.0/argos/urls.py
--rw-r--r--   0        0        0       20 2023-03-06 13:14:01.081952 argos_netbox-0.1.0/argos/version.py
--rw-r--r--   0        0        0     2967 2023-05-26 06:59:58.831506 argos_netbox-0.1.0/argos/views.py
--rw-r--r--   0        0        0     2385 2023-05-30 15:30:18.582755 argos_netbox-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      859 1970-01-01 00:00:00.000000 argos_netbox-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      364 2023-05-31 13:41:33.817429 argos_netbox-0.1.1/README.md
+-rw-r--r--   0        0        0        7 2023-05-31 13:41:34.021950 argos_netbox-0.1.1/argos_netbox/README.md
+-rw-r--r--   0        0        0      332 2023-05-31 13:41:34.026949 argos_netbox-0.1.1/argos_netbox/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 13:41:34.030951 argos_netbox-0.1.1/argos_netbox/api/__init__.py
+-rw-r--r--   0        0        0     6272 2023-05-31 13:41:34.030951 argos_netbox-0.1.1/argos_netbox/api/serializers.py
+-rw-r--r--   0        0        0      545 2023-05-31 13:41:34.031949 argos_netbox-0.1.1/argos_netbox/api/urls.py
+-rw-r--r--   0        0        0      976 2023-05-31 13:41:34.035949 argos_netbox-0.1.1/argos_netbox/api/views.py
+-rw-r--r--   0        0        0      382 2023-05-31 13:41:34.036950 argos_netbox-0.1.1/argos_netbox/filtersets.py
+-rw-r--r--   0        0        0     4601 2023-05-31 13:41:34.039948 argos_netbox-0.1.1/argos_netbox/forms.py
+-rw-r--r--   0        0        0     1772 2023-05-31 13:41:34.040948 argos_netbox-0.1.1/argos_netbox/graphql.py
+-rw-r--r--   0        0        0       36 2023-05-14 13:01:57.587396 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0        2 2023-05-14 13:01:57.582314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/@plugins_snapshot.json
+-rw-r--r--   0        0        0   190035 2023-05-14 13:01:57.524313 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/_ast.data.json
+-rw-r--r--   0        0        0     1775 2023-05-14 13:01:57.525315 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/_ast.meta.json
+-rw-r--r--   0        0        0    61715 2023-05-14 13:01:57.516313 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/_codecs.data.json
+-rw-r--r--   0        0        0     1821 2023-05-14 13:01:57.518314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/_codecs.meta.json
+-rw-r--r--   0        0        0    19501 2023-05-14 13:01:57.513313 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/_collections_abc.data.json
+-rw-r--r--   0        0        0     1729 2023-05-14 13:01:57.514313 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/_collections_abc.meta.json
+-rw-r--r--   0        0        0     7729 2023-05-14 13:01:57.510313 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/_ctypes.data.json
+-rw-r--r--   0        0        0     1731 2023-05-14 13:01:57.512313 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/_ctypes.meta.json
+-rw-r--r--   0        0        0    92896 2023-05-14 13:01:57.508314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1832 2023-05-14 13:01:57.509315 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0    67142 2023-05-14 13:01:57.504314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/_winapi.data.json
+-rw-r--r--   0        0        0     1804 2023-05-14 13:01:57.505313 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/_winapi.meta.json
+-rw-r--r--   0        0        0    21692 2023-05-14 13:01:57.500312 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/abc.data.json
+-rw-r--r--   0        0        0     1717 2023-05-14 13:01:57.501313 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/abc.meta.json
+-rw-r--r--   0        0        0    62974 2023-05-14 13:01:57.497384 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/array.data.json
+-rw-r--r--   0        0        0     1784 2023-05-14 13:01:57.498312 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/array.meta.json
+-rw-r--r--   0        0        0  1147461 2023-05-14 13:01:57.558313 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/builtins.data.json
+-rw-r--r--   0        0        0     1881 2023-05-14 13:01:57.559313 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/builtins.meta.json
+-rw-r--r--   0        0        0   127544 2023-05-14 13:01:57.493313 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/codecs.data.json
+-rw-r--r--   0        0        0     1821 2023-05-14 13:01:57.493313 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/codecs.meta.json
+-rw-r--r--   0        0        0   390750 2023-05-14 13:01:57.487312 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/collections/__init__.data.json
+-rw-r--r--   0        0        0     1800 2023-05-14 13:01:57.488313 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/collections/__init__.meta.json
+-rw-r--r--   0        0        0     4044 2023-05-14 13:01:57.474316 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/collections/abc.data.json
+-rw-r--r--   0        0        0     1696 2023-05-14 13:01:57.475314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/collections/abc.meta.json
+-rw-r--r--   0        0        0   115814 2023-05-14 13:01:57.472313 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/contextlib.data.json
+-rw-r--r--   0        0        0     1772 2023-05-14 13:01:57.472313 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/contextlib.meta.json
+-rw-r--r--   0        0        0   144027 2023-05-14 13:01:57.467383 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1828 2023-05-14 13:01:57.468313 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     8126 2023-05-14 13:01:57.461314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/email/__init__.data.json
+-rw-r--r--   0        0        0     1757 2023-05-14 13:01:57.462314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/email/__init__.meta.json
+-rw-r--r--   0        0        0    12853 2023-05-14 13:01:57.458313 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/email/charset.data.json
+-rw-r--r--   0        0        0     1693 2023-05-14 13:01:57.459314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/email/charset.meta.json
+-rw-r--r--   0        0        0     7713 2023-05-14 13:01:57.456315 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1728 2023-05-14 13:01:57.457369 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25497 2023-05-14 13:01:57.454314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/email/errors.data.json
+-rw-r--r--   0        0        0     1700 2023-05-14 13:01:57.455314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/email/errors.meta.json
+-rw-r--r--   0        0        0     9703 2023-05-14 13:01:57.451313 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/email/header.data.json
+-rw-r--r--   0        0        0     1713 2023-05-14 13:01:57.452313 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/email/header.meta.json
+-rw-r--r--   0        0        0    62361 2023-05-14 13:01:57.449314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/email/message.data.json
+-rw-r--r--   0        0        0     1850 2023-05-14 13:01:57.450313 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/email/message.meta.json
+-rw-r--r--   0        0        0    32702 2023-05-14 13:01:57.445312 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/email/policy.data.json
+-rw-r--r--   0        0        0     1786 2023-05-14 13:01:57.446313 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/email/policy.meta.json
+-rw-r--r--   0        0        0    95101 2023-05-14 13:01:57.441314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/enum.data.json
+-rw-r--r--   0        0        0     1749 2023-05-14 13:01:57.443313 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/enum.meta.json
+-rw-r--r--   0        0        0    23882 2023-05-14 13:01:57.436314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/genericpath.data.json
+-rw-r--r--   0        0        0     1746 2023-05-14 13:01:57.437378 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/genericpath.meta.json
+-rw-r--r--   0        0        0     6520 2023-05-14 13:01:57.433314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1731 2023-05-14 13:01:57.434314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    73613 2023-05-14 13:01:57.430314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/importlib/abc.data.json
+-rw-r--r--   0        0        0     1879 2023-05-14 13:01:57.431313 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/importlib/abc.meta.json
+-rw-r--r--   0        0        0    68149 2023-05-14 13:01:57.425315 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1890 2023-05-14 13:01:57.426313 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    95589 2023-05-14 13:01:57.421314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1869 2023-05-14 13:01:57.422315 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    12491 2023-05-14 13:01:57.417314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1714 2023-05-14 13:01:57.418313 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0    88673 2023-05-14 13:01:57.414314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/io.data.json
+-rw-r--r--   0        0        0     1840 2023-05-14 13:01:57.415313 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/io.meta.json
+-rw-r--r--   0        0        0    24368 2023-05-14 13:01:57.409313 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/mmap.data.json
+-rw-r--r--   0        0        0     1756 2023-05-14 13:01:57.410312 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/mmap.meta.json
+-rw-r--r--   0        0        0    15200 2023-05-14 13:01:57.406313 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/ntpath.data.json
+-rw-r--r--   0        0        0     1768 2023-05-14 13:01:57.407373 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/ntpath.meta.json
+-rw-r--r--   0        0        0   248783 2023-05-14 13:01:57.403312 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/os/__init__.data.json
+-rw-r--r--   0        0        0     1899 2023-05-14 13:01:57.405314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/os/__init__.meta.json
+-rw-r--r--   0        0        0     5311 2023-05-14 13:01:57.394317 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/os/path.data.json
+-rw-r--r--   0        0        0     1685 2023-05-14 13:01:57.395314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/os/path.meta.json
+-rw-r--r--   0        0        0    90374 2023-05-14 13:01:57.390314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/pathlib.data.json
+-rw-r--r--   0        0        0     1849 2023-05-14 13:01:57.392313 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/pathlib.meta.json
+-rw-r--r--   0        0        0    47610 2023-05-14 13:01:57.384314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/pickle.data.json
+-rw-r--r--   0        0        0     1785 2023-05-14 13:01:57.386314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/pickle.meta.json
+-rw-r--r--   0        0        0    80910 2023-05-14 13:01:57.380314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/posixpath.data.json
+-rw-r--r--   0        0        0     1779 2023-05-14 13:01:57.381316 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/posixpath.meta.json
+-rw-r--r--   0        0        0   151627 2023-05-14 13:01:57.375314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/re.data.json
+-rw-r--r--   0        0        0     1871 2023-05-14 13:01:57.377373 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/re.meta.json
+-rw-r--r--   0        0        0    15014 2023-05-14 13:01:57.369314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/sre_compile.data.json
+-rw-r--r--   0        0        0     1715 2023-05-14 13:01:57.370314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/sre_compile.meta.json
+-rw-r--r--   0        0        0    29571 2023-05-14 13:01:57.366314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/sre_constants.data.json
+-rw-r--r--   0        0        0     1699 2023-05-14 13:01:57.368315 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/sre_constants.meta.json
+-rw-r--r--   0        0        0    52535 2023-05-14 13:01:57.363314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/sre_parse.data.json
+-rw-r--r--   0        0        0     1779 2023-05-14 13:01:57.365313 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/sre_parse.meta.json
+-rw-r--r--   0        0        0   181048 2023-05-14 13:01:57.359313 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/subprocess.data.json
+-rw-r--r--   0        0        0     1859 2023-05-14 13:01:57.360314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/subprocess.meta.json
+-rw-r--r--   0        0        0   168592 2023-05-14 13:01:57.351314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/sys.data.json
+-rw-r--r--   0        0        0     1818 2023-05-14 13:01:57.353315 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/sys.meta.json
+-rw-r--r--   0        0        0   254573 2023-05-14 13:01:57.345313 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/types.data.json
+-rw-r--r--   0        0        0     1790 2023-05-14 13:01:57.346312 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/types.meta.json
+-rw-r--r--   0        0        0   446716 2023-05-14 13:01:57.336313 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/typing.data.json
+-rw-r--r--   0        0        0     1857 2023-05-14 13:01:57.337460 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/typing.meta.json
+-rw-r--r--   0        0        0    54822 2023-05-14 13:01:57.320394 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/typing_extensions.data.json
+-rw-r--r--   0        0        0     1780 2023-05-14 13:01:57.321394 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/typing_extensions.meta.json
+-rw-r--r--   0        0        0     1528 2023-05-14 13:01:57.564314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/work/__init__.data.json
+-rw-r--r--   0        0        0     1564 2023-05-14 13:01:57.565313 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/work/__init__.meta.json
+-rw-r--r--   0        0        0     1381 2023-05-14 13:01:57.566969 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects.data.json
+-rw-r--r--   0        0        0     1521 2023-05-14 13:01:57.567314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects.meta.json
+-rw-r--r--   0        0        0     1424 2023-05-14 13:01:57.569314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos.data.json
+-rw-r--r--   0        0        0     1534 2023-05-14 13:01:57.570315 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos.meta.json
+-rw-r--r--   0        0        0     1523 2023-05-14 13:01:57.571314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin.data.json
+-rw-r--r--   0        0        0     1563 2023-05-14 13:01:57.572316 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin.meta.json
+-rw-r--r--   0        0        0     5506 2023-05-14 13:01:57.580315 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/__init__.data.json
+-rw-r--r--   0        0        0     1738 2023-05-14 13:01:57.581314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/__init__.meta.json
+-rw-r--r--   0        0        0     4680 2023-05-14 13:01:57.576315 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/migrations/0002_alter_bgp_mesh_options.data.json
+-rw-r--r--   0        0        0     1740 2023-05-14 13:01:57.577314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/migrations/0002_alter_bgp_mesh_options.meta.json
+-rw-r--r--   0        0        0     1955 2023-05-14 13:01:57.573314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/migrations/__init__.data.json
+-rw-r--r--   0        0        0     1673 2023-05-14 13:01:57.574314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/migrations/__init__.meta.json
+-rw-r--r--   0        0        0     1904 2023-05-14 13:01:57.562314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/version.data.json
+-rw-r--r--   0        0        0     1658 2023-05-14 13:01:57.563314 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/version.meta.json
+-rw-r--r--   0        0        0      193 2023-05-14 13:01:57.591313 argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     8975 2023-05-31 13:41:34.041949 argos_netbox-0.1.1/argos_netbox/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-05-31 13:41:34.042950 argos_netbox-0.1.1/argos_netbox/migrations/__init__.py
+-rw-r--r--   0        0        0     6889 2023-05-31 13:41:34.042950 argos_netbox-0.1.1/argos_netbox/models.py
+-rw-r--r--   0        0        0     2412 2023-05-31 13:41:34.043949 argos_netbox-0.1.1/argos_netbox/navigation.py
+-rw-r--r--   0        0        0        0 2023-05-31 13:41:34.043949 argos_netbox-0.1.1/argos_netbox/requirements.txt
+-rw-r--r--   0        0        0     3334 2023-05-31 13:41:34.043949 argos_netbox-0.1.1/argos_netbox/tables.py
+-rw-r--r--   0        0        0     1810 2023-05-31 13:41:34.044948 argos_netbox-0.1.1/argos_netbox/templates/argos_netbox/address_family.html
+-rw-r--r--   0        0        0     1067 2023-05-31 13:41:34.045948 argos_netbox-0.1.1/argos_netbox/templates/argos_netbox/address_family_edit.html
+-rw-r--r--   0        0        0     1249 2023-05-31 13:41:34.046948 argos_netbox-0.1.1/argos_netbox/templates/argos_netbox/bgp_ce.html
+-rw-r--r--   0        0        0     2510 2023-05-31 13:41:34.046948 argos_netbox-0.1.1/argos_netbox/templates/argos_netbox/bgp_mesh.html
+-rw-r--r--   0        0        0     1852 2023-05-31 13:41:34.047949 argos_netbox-0.1.1/argos_netbox/templates/argos_netbox/bgp_pe.html
+-rw-r--r--   0        0        0     1421 2023-05-31 13:41:34.047949 argos_netbox-0.1.1/argos_netbox/templates/argos_netbox/ldp.html
+-rw-r--r--   0        0        0     1106 2023-05-31 13:41:34.048952 argos_netbox-0.1.1/argos_netbox/templates/argos_netbox/ldp_edit.html
+-rw-r--r--   0        0        0     1328 2023-05-31 13:41:34.049949 argos_netbox-0.1.1/argos_netbox/templates/argos_netbox/mpls_instance.html
+-rw-r--r--   0        0        0      680 2023-05-31 13:41:34.049949 argos_netbox-0.1.1/argos_netbox/templates/argos_netbox/util/hide_if_checked.html
+-rw-r--r--   0        0        0      326 2023-05-31 13:41:34.050950 argos_netbox-0.1.1/argos_netbox/templatetags/argos_macros.py
+-rw-r--r--   0        0        0     3925 2023-05-31 13:41:34.054948 argos_netbox-0.1.1/argos_netbox/urls.py
+-rw-r--r--   0        0        0       20 2023-05-31 14:00:25.251083 argos_netbox-0.1.1/argos_netbox/version.py
+-rw-r--r--   0        0        0     2981 2023-05-31 13:41:34.059947 argos_netbox-0.1.1/argos_netbox/views.py
+-rw-r--r--   0        0        0     1400 2023-05-31 14:03:56.296029 argos_netbox-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      859 1970-01-01 00:00:00.000000 argos_netbox-0.1.1/PKG-INFO
```

### Comparing `argos_netbox-0.1.0/argos/api/serializers.py` & `argos_netbox-0.1.1/argos_netbox/api/serializers.py`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/api/urls.py` & `argos_netbox-0.1.1/argos_netbox/api/urls.py`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/api/views.py` & `argos_netbox-0.1.1/argos_netbox/api/views.py`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/forms.py` & `argos_netbox-0.1.1/argos_netbox/forms.py`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/graphql.py` & `argos_netbox-0.1.1/argos_netbox/graphql.py`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/_ast.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/_ast.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/_ast.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/_codecs.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/_codecs.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/_collections_abc.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/_collections_abc.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/_ctypes.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/_ctypes.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/_typeshed/__init__.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/_typeshed/__init__.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/_winapi.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/_winapi.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/_winapi.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/_winapi.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/abc.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/abc.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/abc.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/abc.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/array.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/array.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/array.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/array.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/builtins.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/builtins.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/builtins.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/codecs.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/codecs.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/codecs.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/collections/__init__.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/collections/__init__.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/collections/abc.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/collections/abc.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/contextlib.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/contextlib.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/ctypes/__init__.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/ctypes/__init__.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/email/__init__.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/email/__init__.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/email/charset.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/email/charset.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/email/contentmanager.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/email/contentmanager.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/email/errors.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/email/errors.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/email/header.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/email/header.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/email/header.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/email/message.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/email/message.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/email/message.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/email/policy.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/email/policy.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/enum.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/enum.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/enum.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/enum.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/genericpath.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/genericpath.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/importlib/__init__.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/importlib/__init__.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/importlib/abc.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/importlib/abc.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/importlib/machinery.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/importlib/machinery.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/importlib/metadata/__init__.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/importlib/metadata/__init__.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/importlib/metadata/_meta.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/importlib/metadata/_meta.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/importlib/metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/io.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/io.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/io.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/io.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/mmap.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/mmap.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/mmap.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/ntpath.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/ntpath.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/ntpath.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/ntpath.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/os/__init__.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/os/__init__.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/os/path.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/os/path.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/os/path.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/pathlib.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/pathlib.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/pickle.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/pickle.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/pickle.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/posixpath.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/posixpath.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/re.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/re.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/re.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/re.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/sre_compile.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/sre_compile.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/sre_constants.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/sre_constants.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/sre_parse.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/sre_parse.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/subprocess.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/subprocess.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/sys.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/sys.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/sys.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/sys.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/types.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/types.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/types.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/types.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/typing.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/typing.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/typing.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/typing.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/typing_extensions.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/typing_extensions.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/work/__init__.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/work/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/work/__init__.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/work/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/work/school_projects.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/work/school_projects.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/work/school_projects/argos.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/work/school_projects/argos.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/__init__.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/__init__.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/migrations/0002_alter_bgp_mesh_options.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/migrations/0002_alter_bgp_mesh_options.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/migrations/0002_alter_bgp_mesh_options.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/migrations/0002_alter_bgp_mesh_options.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/migrations/__init__.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/migrations/__init__.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/migrations/__init__.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/migrations/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/version.data.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/version.data.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/version.meta.json` & `argos_netbox-0.1.1/argos_netbox/migrations/.mypy_cache/3.11/work/school_projects/argos/netbox_plugin/argos/version.meta.json`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/migrations/0001_initial.py` & `argos_netbox-0.1.1/argos_netbox/migrations/0001_initial.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
                 ('created', models.DateTimeField(auto_now_add=True, null=True)),
                 ('last_updated', models.DateTimeField(auto_now=True, null=True)),
                 (
                     'custom_field_data',
                     models.JSONField(blank=True, default=dict, encoder=utilities.json.CustomFieldJSONEncoder),
                 ),
                 ('comments', models.TextField()),
-                ('advertised_customers', models.ManyToManyField(blank=True, to='argos.bgp_ce')),
+                ('advertised_customers', models.ManyToManyField(blank=True, to='argos_netbox.bgp_ce')),
                 ('asn', models.ForeignKey(on_delete=django.db.models.deletion.PROTECT, to='ipam.asn')),
                 ('device', models.OneToOneField(on_delete=django.db.models.deletion.PROTECT, to='dcim.device')),
                 ('tags', taggit.managers.TaggableManager(through='extras.TaggedItem', to='extras.Tag')),
                 (
                     'update_source_interface',
                     models.OneToOneField(
                         limit_choices_to=models.Q(('device_id', models.F('device'))),
@@ -144,19 +144,19 @@
                 ('created', models.DateTimeField(auto_now_add=True, null=True)),
                 ('last_updated', models.DateTimeField(auto_now=True, null=True)),
                 (
                     'custom_field_data',
                     models.JSONField(blank=True, default=dict, encoder=utilities.json.CustomFieldJSONEncoder),
                 ),
                 ('comments', models.TextField()),
-                ('bgp_mesh', models.ManyToManyField(blank=False, related_name='bgp_mesh', to='argos.bgp_pe')),
+                ('bgp_mesh', models.ManyToManyField(blank=False, related_name='bgp_mesh', to='argos_netbox.bgp_pe')),
                 (
                     'address_family',
                     models.ForeignKey(
-                        blank=False, on_delete=django.db.models.deletion.PROTECT, to='argos.address_family'
+                        blank=False, on_delete=django.db.models.deletion.PROTECT, to='argos_netbox.address_family'
                     ),
                 ),
                 ('name', models.CharField(max_length=50)),
                 ('tags', taggit.managers.TaggableManager(through='extras.TaggedItem', to='extras.Tag')),
             ],
             options={
                 'verbose_name': 'BGP Mesh',
@@ -175,15 +175,15 @@
                 ('service', models.CharField(blank=False, max_length=50, null=False)),
                 ('name', models.CharField(max_length=50)),
                 ('last_updated', models.DateTimeField(auto_now=True, null=True)),
                 ('comments', models.TextField()),
                 (
                     'ibgp',
                     models.OneToOneField(
-                        on_delete=django.db.models.deletion.PROTECT, related_name='ibgp', to='argos.bgp_mesh'
+                        on_delete=django.db.models.deletion.PROTECT, related_name='ibgp', to='argos_netbox.bgp_mesh'
                     ),
                 ),
                 ('tags', taggit.managers.TaggableManager(through='extras.TaggedItem', to='extras.Tag')),
             ],
             options={
                 'verbose_name': 'MPLS Instance',
                 'verbose_name_plural': 'MPLS Instances',
```

### Comparing `argos_netbox-0.1.0/argos/models.py` & `argos_netbox-0.1.1/argos_netbox/models.py`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/navigation.py` & `argos_netbox-0.1.1/argos_netbox/navigation.py`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/tables.py` & `argos_netbox-0.1.1/argos_netbox/tables.py`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/templates/argos/address_family.html` & `argos_netbox-0.1.1/argos_netbox/templates/argos_netbox/address_family.html`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/templates/argos/address_family_edit.html` & `argos_netbox-0.1.1/argos_netbox/templates/argos_netbox/address_family_edit.html`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/templates/argos/bgp_ce.html` & `argos_netbox-0.1.1/argos_netbox/templates/argos_netbox/bgp_ce.html`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/templates/argos/bgp_mesh.html` & `argos_netbox-0.1.1/argos_netbox/templates/argos_netbox/bgp_mesh.html`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/templates/argos/bgp_pe.html` & `argos_netbox-0.1.1/argos_netbox/templates/argos_netbox/bgp_pe.html`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/templates/argos/ldp.html` & `argos_netbox-0.1.1/argos_netbox/templates/argos_netbox/ldp.html`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/templates/argos/mpls_instance.html` & `argos_netbox-0.1.1/argos_netbox/templates/argos_netbox/mpls_instance.html`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/templates/argos/util/hide_if_checked.html` & `argos_netbox-0.1.1/argos_netbox/templates/argos_netbox/util/hide_if_checked.html`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/urls.py` & `argos_netbox-0.1.1/argos_netbox/urls.py`

 * *Files identical despite different names*

### Comparing `argos_netbox-0.1.0/argos/views.py` & `argos_netbox-0.1.1/argos_netbox/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     queryset = models.LDP.objects.all()
     table = tables.LDP_Table
 
 
 class LDP_EditView(generic.ObjectEditView):
     queryset = models.LDP.objects.all()
     form = forms.LDP_Form
-    template_name = 'argos/ldp_edit.html'
+    template_name = 'argos_netbox/ldp_edit.html'
 
 
 class LDP_DeleteView(generic.ObjectDeleteView):
     queryset = models.LDP.objects.all()
 
 
 # BGP CE
@@ -93,15 +93,15 @@
     queryset = models.Address_Family.objects.all()
     table = tables.Address_Family_Table
 
 
 class Address_Family_EditView(generic.ObjectEditView):
     queryset = models.Address_Family.objects.all()
     form = forms.Address_Family_Form
-    template_name = 'argos/address_family_edit.html'
+    template_name = 'argos_netbox/address_family_edit.html'
 
 
 class Address_Family_DeleteView(generic.ObjectDeleteView):
     queryset = models.Address_Family.objects.all()
 
 
 # MPLS Instance
```

### Comparing `argos_netbox-0.1.0/PKG-INFO` & `argos_netbox-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argos-netbox
-Version: 0.1.0
+Version: 0.1.1
 Author-Email: Dominic Walther <dominic.walther@ost.ch>, Dejan Jovicic <dejan.jovicic@ost.ch>
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Project-URL: Repository, https://gitlab.ost.ch/pydantic-sa/netboxify
 Requires-Python: >=3.9
 Requires-Dist: django-taggit>=3.1.0
```

