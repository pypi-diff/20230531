# Comparing `tmp/pySMART-1.2.5.dev23.tar.gz` & `tmp/pySMART-1.2.5.dev24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pySMART-1.2.5.dev23.tar", last modified: Fri May 26 10:16:11 2023, max compression
+gzip compressed data, was "pySMART-1.2.5.dev24.tar", last modified: Wed May 31 10:00:31 2023, max compression
```

## Comparing `pySMART-1.2.5.dev23.tar` & `pySMART-1.2.5.dev24.tar`

### file list

```diff
@@ -1,163 +1,163 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.439471 pySMART-1.2.5.dev23/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.419471 pySMART-1.2.5.dev23/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.423471 pySMART-1.2.5.dev23/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/.github/ISSUE_TEMPLATE/bug_report.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.423471 pySMART-1.2.5.dev23/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    26462 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-05-26 10:16:11.439471 pySMART-1.2.5.dev23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.423471 pySMART-1.2.5.dev23/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-26 10:16:04.000000 pySMART-1.2.5.dev23/docs/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.423471 pySMART-1.2.5.dev23/docs/pySMART/
--rw-r--r--   0 runner    (1001) docker     (123)   109043 2023-05-26 10:16:04.000000 pySMART-1.2.5.dev23/docs/pySMART/utils.html
--rw-r--r--   0 runner    (1001) docker     (123)   864790 2023-05-26 10:16:04.000000 pySMART-1.2.5.dev23/docs/pySMART.html
--rw-r--r--   0 runner    (1001) docker     (123)   309690 2023-05-26 10:16:04.000000 pySMART-1.2.5.dev23/docs/search.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.427471 pySMART-1.2.5.dev23/pySMART/
--rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/pySMART/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/pySMART/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)    62538 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/pySMART/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/pySMART/device_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     7904 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/pySMART/diagnostics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.427471 pySMART-1.2.5.dev23/pySMART/interface/
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/pySMART/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42649 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/pySMART/interface/nvme.py
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/pySMART/smartctl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/pySMART/testentry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/pySMART/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-26 10:16:11.000000 pySMART-1.2.5.dev23/pySMART/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.427471 pySMART-1.2.5.dev23/pySMART.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-05-26 10:16:11.000000 pySMART-1.2.5.dev23/pySMART.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-05-26 10:16:11.000000 pySMART-1.2.5.dev23/pySMART.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 10:16:11.000000 pySMART-1.2.5.dev23/pySMART.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-26 10:16:11.000000 pySMART-1.2.5.dev23/pySMART.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-26 10:16:11.000000 pySMART-1.2.5.dev23/pySMART.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 10:16:11.439471 pySMART-1.2.5.dev23/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.427471 pySMART-1.2.5.dev23/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.419471 pySMART-1.2.5.dev23/tests/dataset/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.419471 pySMART-1.2.5.dev23/tests/dataset/listingtests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.427471 pySMART-1.2.5.dev23/tests/dataset/listingtests/linux_01/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/listingtests/linux_01/_--scan-open
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/listingtests/linux_01/_-d_nvme_--all__dev_nvme0
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/listingtests/linux_01/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.427471 pySMART-1.2.5.dev23/tests/dataset/listingtests/linux_multiple_devices/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/listingtests/linux_multiple_devices/_--scan-open
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/listingtests/linux_multiple_devices/_-d_nvme_--all__dev_nvme0
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/listingtests/linux_multiple_devices/_-d_nvme_--all__dev_nvme1
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/listingtests/linux_multiple_devices/_-d_sat+megaraid,60_--all__dev_bus_0
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/listingtests/linux_multiple_devices/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.427471 pySMART-1.2.5.dev23/tests/dataset/listingtests/mac_01/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/listingtests/mac_01/_--scan-open
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/listingtests/mac_01/_-d_ata_--all_IOService__AppleACPIPlatformExpert_PCI0@0_AppleACPIPCI_RP06@1C,5_IOPP_SSD0@0_AppleAHCI_PRT0@0_IOAHCIDevice@0_AppleAHCIDiskDriver_IOAHCIBlockStorageDevice
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/listingtests/mac_01/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.431471 pySMART-1.2.5.dev23/tests/dataset/listingtests/win10_01/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/listingtests/win10_01/_--scan-open
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/listingtests/win10_01/_-d_nvme_--all__dev_sda
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/listingtests/win10_01/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.423471 pySMART-1.2.5.dev23/tests/dataset/singletests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.431471 pySMART-1.2.5.dev23/tests/dataset/singletests/megaraid_ph_sas_hdd_0/
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/megaraid_ph_sas_hdd_0/_-d_megaraid,44_--all__dev_bus_7
--rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/megaraid_ph_sas_hdd_0/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.431471 pySMART-1.2.5.dev23/tests/dataset/singletests/megaraid_ph_sata_hdd_0/
--rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/megaraid_ph_sata_hdd_0/_-d_megaraid,16_--all__dev_bus_0
--rw-r--r--   0 runner    (1001) docker     (123)    17615 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/megaraid_ph_sata_hdd_0/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.431471 pySMART-1.2.5.dev23/tests/dataset/singletests/megaraid_ph_sata_hdd_1_issue_56/
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/megaraid_ph_sata_hdd_1_issue_56/_-d_sat+megaraid,60_--all__dev_bus_0
--rw-r--r--   0 runner    (1001) docker     (123)    22633 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/megaraid_ph_sata_hdd_1_issue_56/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.431471 pySMART-1.2.5.dev23/tests/dataset/singletests/megaraid_ph_sata_ssd_0/
--rw-r--r--   0 runner    (1001) docker     (123)     7706 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/megaraid_ph_sata_ssd_0/_-d_megaraid,28_--all__dev_bus_0
--rw-r--r--   0 runner    (1001) docker     (123)    22012 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/megaraid_ph_sata_ssd_0/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.431471 pySMART-1.2.5.dev23/tests/dataset/singletests/megaraid_vd_0/
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/megaraid_vd_0/_-d_scsi_--all__dev_sda
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/megaraid_vd_0/_-d_scsi_-l_background__dev_sda
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/megaraid_vd_0/_-d_test__dev_sda
--rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/megaraid_vd_0/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.431471 pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_0/
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_0/_-d_nvme_--all__dev_nvme0
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_0/_-d_test__dev_nvme0
--rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_0/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.431471 pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_1_issue_37/
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_1_issue_37/_-d_nvme_--all__dev_nvme0
--rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_1_issue_37/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.431471 pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_2_issue_46/
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_2_issue_46/_-d_nvme_--all__dev_nvme0
--rw-r--r--   0 runner    (1001) docker     (123)     8643 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_2_issue_46/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.431471 pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_3_issue_52/
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_3_issue_52/_-d_nvme_--all__dev_nvme0n1
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_3_issue_52/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.431471 pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_4_issue_53/
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_4_issue_53/_-d_nvme_--all__dev_nvme0
--rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_4_issue_53/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.431471 pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_5_issue_46/
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_5_issue_46/_-d_nvme_--all__dev_nvme0
--rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_5_issue_46/device.json
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_5_issue_46/nvmessd.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.431471 pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_6/
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_6/_-d_nvme_--all__dev_nvme0
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_6/_-d_test__dev_nvme0
--rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_6/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.431471 pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_7_issue_63/
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_7_issue_63/_-d_nvme_--all__dev_nvme0n1
--rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_7_issue_63/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.435471 pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_8/
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_8/_-d_nvme_--all__dev_nvme0n1
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_8/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.435471 pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_win10_0_issue_64/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_win10_0_issue_64/_--scan-open
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_win10_0_issue_64/_-d_nvme_--all__dev_sda
--rw-r--r--   0 runner    (1001) docker     (123)    14724 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_win10_0_issue_64/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.435471 pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_win10_mingw32_0_issue_48/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_win10_mingw32_0_issue_48/_--scan-open
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_win10_mingw32_0_issue_48/_-d_nvme_--all__dev_sda
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_win10_mingw32_0_issue_48/_-d_nvme_--all_sda
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_win10_mingw32_0_issue_48/_-d_test__dev_sda
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_win10_mingw32_0_issue_48/_-d_test_sda
--rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_win10_mingw32_0_issue_48/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.435471 pySMART-1.2.5.dev23/tests/dataset/singletests/sas_hdd_0_issue_51/
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/sas_hdd_0_issue_51/_-d_scsi_--all__dev_sdc
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/sas_hdd_0_issue_51/_-d_scsi_-l_background__dev_sdc
--rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/sas_hdd_0_issue_51/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.435471 pySMART-1.2.5.dev23/tests/dataset/singletests/sas_ssd_0_issue_57/
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/sas_ssd_0_issue_57/_-d_scsi_--all__dev_sdb
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/sas_ssd_0_issue_57/_-x__dev_sdb
--rw-r--r--   0 runner    (1001) docker     (123)    10217 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/sas_ssd_0_issue_57/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.435471 pySMART-1.2.5.dev23/tests/dataset/singletests/sat_hdd_0_issue70/
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/sat_hdd_0_issue70/_-d_sat_--all__dev_sg2
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/sat_hdd_0_issue70/_-d_test__dev_sg2
--rw-r--r--   0 runner    (1001) docker     (123)    20777 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/sat_hdd_0_issue70/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.435471 pySMART-1.2.5.dev23/tests/dataset/singletests/sat_ssd_0_issue_65/
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/sat_ssd_0_issue_65/_-d_sat_--all__dev_sda
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/sat_ssd_0_issue_65/_-d_test__dev_sda
--rw-r--r--   0 runner    (1001) docker     (123)    22000 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/sat_ssd_0_issue_65/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.435471 pySMART-1.2.5.dev23/tests/dataset/singletests/sata_hdd_0_issue42/
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/sata_hdd_0_issue42/_-d_ata_--all__dev_sdau
--rw-r--r--   0 runner    (1001) docker     (123)    23712 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/sata_hdd_0_issue42/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.435471 pySMART-1.2.5.dev23/tests/dataset/singletests/sata_hdd_1_issue46/
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/sata_hdd_1_issue46/_-d_ata_--all__dev_sdau
--rw-r--r--   0 runner    (1001) docker     (123)    17621 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/sata_hdd_1_issue46/device.json
--rw-r--r--   0 runner    (1001) docker     (123)    17855 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/sata_hdd_1_issue46/heliumhdd.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.435471 pySMART-1.2.5.dev23/tests/dataset/singletests/sata_ssd_0_issue_49/
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/sata_ssd_0_issue_49/_-d_ata_--all__dev_sda
--rw-r--r--   0 runner    (1001) docker     (123)    20400 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/sata_ssd_0_issue_49/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.435471 pySMART-1.2.5.dev23/tests/dataset/singletests/sata_ssd_1_issue_72/
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/sata_ssd_1_issue_72/_-d_ata_--all__dev_sda
--rw-r--r--   0 runner    (1001) docker     (123)    23567 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/sata_ssd_1_issue_72/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.439471 pySMART-1.2.5.dev23/tests/dataset/singletests/sata_ssd_macos_0/
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/sata_ssd_macos_0/_-d_ata_--all_IOService__AppleACPIPlatformExpert_PCI0@0_AppleACPIPCI_RP06@1C,5_IOPP_SSD0@0_AppleAHCI_PRT0@0_IOAHCIDevice@0_AppleAHCIDiskDriver_IOAHCIBlockStorageDevice
--rw-r--r--   0 runner    (1001) docker     (123)    15407 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/sata_ssd_macos_0/device.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:16:11.439471 pySMART-1.2.5.dev23/tests/dataset/singletests/usb_ssd_0_issue_50/
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/usb_ssd_0_issue_50/_-d_ata_--all__dev_sda
--rw-r--r--   0 runner    (1001) docker     (123)    25889 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/usb_ssd_0_issue_50/device.json
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/dataset/singletests/usb_ssd_0_issue_50/notes.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/gen_devicejson.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/smartctlfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-26 10:15:47.000000 pySMART-1.2.5.dev23/tests/test_device_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.890847 pySMART-1.2.5.dev24/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.870847 pySMART-1.2.5.dev24/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.874847 pySMART-1.2.5.dev24/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/.github/ISSUE_TEMPLATE/bug_report.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.874847 pySMART-1.2.5.dev24/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    26462 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-05-31 10:00:31.890847 pySMART-1.2.5.dev24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.874847 pySMART-1.2.5.dev24/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-31 10:00:24.000000 pySMART-1.2.5.dev24/docs/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.874847 pySMART-1.2.5.dev24/docs/pySMART/
+-rw-r--r--   0 runner    (1001) docker     (123)   109043 2023-05-31 10:00:24.000000 pySMART-1.2.5.dev24/docs/pySMART/utils.html
+-rw-r--r--   0 runner    (1001) docker     (123)   864790 2023-05-31 10:00:24.000000 pySMART-1.2.5.dev24/docs/pySMART.html
+-rw-r--r--   0 runner    (1001) docker     (123)   309690 2023-05-31 10:00:24.000000 pySMART-1.2.5.dev24/docs/search.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.874847 pySMART-1.2.5.dev24/pySMART/
+-rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/pySMART/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/pySMART/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62538 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/pySMART/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/pySMART/device_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7904 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/pySMART/diagnostics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.878847 pySMART-1.2.5.dev24/pySMART/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/pySMART/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42649 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/pySMART/interface/nvme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9087 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/pySMART/smartctl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/pySMART/testentry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/pySMART/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-31 10:00:31.000000 pySMART-1.2.5.dev24/pySMART/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.878847 pySMART-1.2.5.dev24/pySMART.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-05-31 10:00:31.000000 pySMART-1.2.5.dev24/pySMART.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-05-31 10:00:31.000000 pySMART-1.2.5.dev24/pySMART.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 10:00:31.000000 pySMART-1.2.5.dev24/pySMART.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-31 10:00:31.000000 pySMART-1.2.5.dev24/pySMART.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 10:00:31.000000 pySMART-1.2.5.dev24/pySMART.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 10:00:31.890847 pySMART-1.2.5.dev24/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.878847 pySMART-1.2.5.dev24/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.870847 pySMART-1.2.5.dev24/tests/dataset/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.870847 pySMART-1.2.5.dev24/tests/dataset/listingtests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.878847 pySMART-1.2.5.dev24/tests/dataset/listingtests/linux_01/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/listingtests/linux_01/_--scan-open
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/listingtests/linux_01/_-d_nvme_--all__dev_nvme0
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/listingtests/linux_01/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.878847 pySMART-1.2.5.dev24/tests/dataset/listingtests/linux_multiple_devices/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/listingtests/linux_multiple_devices/_--scan-open
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/listingtests/linux_multiple_devices/_-d_nvme_--all__dev_nvme0
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/listingtests/linux_multiple_devices/_-d_nvme_--all__dev_nvme1
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/listingtests/linux_multiple_devices/_-d_sat+megaraid,60_--all__dev_bus_0
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/listingtests/linux_multiple_devices/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.878847 pySMART-1.2.5.dev24/tests/dataset/listingtests/mac_01/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/listingtests/mac_01/_--scan-open
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/listingtests/mac_01/_-d_ata_--all_IOService__AppleACPIPlatformExpert_PCI0@0_AppleACPIPCI_RP06@1C,5_IOPP_SSD0@0_AppleAHCI_PRT0@0_IOAHCIDevice@0_AppleAHCIDiskDriver_IOAHCIBlockStorageDevice
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/listingtests/mac_01/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.878847 pySMART-1.2.5.dev24/tests/dataset/listingtests/win10_01/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/listingtests/win10_01/_--scan-open
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/listingtests/win10_01/_-d_nvme_--all__dev_sda
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/listingtests/win10_01/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.870847 pySMART-1.2.5.dev24/tests/dataset/singletests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.878847 pySMART-1.2.5.dev24/tests/dataset/singletests/megaraid_ph_sas_hdd_0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/megaraid_ph_sas_hdd_0/_-d_megaraid,44_--all__dev_bus_7
+-rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/megaraid_ph_sas_hdd_0/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.878847 pySMART-1.2.5.dev24/tests/dataset/singletests/megaraid_ph_sata_hdd_0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/megaraid_ph_sata_hdd_0/_-d_megaraid,16_--all__dev_bus_0
+-rw-r--r--   0 runner    (1001) docker     (123)    17615 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/megaraid_ph_sata_hdd_0/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.878847 pySMART-1.2.5.dev24/tests/dataset/singletests/megaraid_ph_sata_hdd_1_issue_56/
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/megaraid_ph_sata_hdd_1_issue_56/_-d_sat+megaraid,60_--all__dev_bus_0
+-rw-r--r--   0 runner    (1001) docker     (123)    22633 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/megaraid_ph_sata_hdd_1_issue_56/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.882847 pySMART-1.2.5.dev24/tests/dataset/singletests/megaraid_ph_sata_ssd_0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7706 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/megaraid_ph_sata_ssd_0/_-d_megaraid,28_--all__dev_bus_0
+-rw-r--r--   0 runner    (1001) docker     (123)    22012 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/megaraid_ph_sata_ssd_0/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.882847 pySMART-1.2.5.dev24/tests/dataset/singletests/megaraid_vd_0/
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/megaraid_vd_0/_-d_scsi_--all__dev_sda
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/megaraid_vd_0/_-d_scsi_-l_background__dev_sda
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/megaraid_vd_0/_-d_test__dev_sda
+-rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/megaraid_vd_0/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.882847 pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_0/_-d_nvme_--all__dev_nvme0
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_0/_-d_test__dev_nvme0
+-rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_0/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.882847 pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_1_issue_37/
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_1_issue_37/_-d_nvme_--all__dev_nvme0
+-rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_1_issue_37/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.882847 pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_2_issue_46/
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_2_issue_46/_-d_nvme_--all__dev_nvme0
+-rw-r--r--   0 runner    (1001) docker     (123)     8643 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_2_issue_46/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.882847 pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_3_issue_52/
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_3_issue_52/_-d_nvme_--all__dev_nvme0n1
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_3_issue_52/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.882847 pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_4_issue_53/
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_4_issue_53/_-d_nvme_--all__dev_nvme0
+-rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_4_issue_53/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.882847 pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_5_issue_46/
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_5_issue_46/_-d_nvme_--all__dev_nvme0
+-rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_5_issue_46/device.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_5_issue_46/nvmessd.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.882847 pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_6/
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_6/_-d_nvme_--all__dev_nvme0
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_6/_-d_test__dev_nvme0
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_6/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.882847 pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_7_issue_63/
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_7_issue_63/_-d_nvme_--all__dev_nvme0n1
+-rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_7_issue_63/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.882847 pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_8/
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_8/_-d_nvme_--all__dev_nvme0n1
+-rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_8/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.882847 pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_win10_0_issue_64/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_win10_0_issue_64/_--scan-open
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_win10_0_issue_64/_-d_nvme_--all__dev_sda
+-rw-r--r--   0 runner    (1001) docker     (123)    14724 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_win10_0_issue_64/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.886847 pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_win10_mingw32_0_issue_48/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_win10_mingw32_0_issue_48/_--scan-open
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_win10_mingw32_0_issue_48/_-d_nvme_--all__dev_sda
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_win10_mingw32_0_issue_48/_-d_nvme_--all_sda
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_win10_mingw32_0_issue_48/_-d_test__dev_sda
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_win10_mingw32_0_issue_48/_-d_test_sda
+-rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_win10_mingw32_0_issue_48/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.886847 pySMART-1.2.5.dev24/tests/dataset/singletests/sas_hdd_0_issue_51/
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/sas_hdd_0_issue_51/_-d_scsi_--all__dev_sdc
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/sas_hdd_0_issue_51/_-d_scsi_-l_background__dev_sdc
+-rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/sas_hdd_0_issue_51/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.886847 pySMART-1.2.5.dev24/tests/dataset/singletests/sas_ssd_0_issue_57/
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/sas_ssd_0_issue_57/_-d_scsi_--all__dev_sdb
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/sas_ssd_0_issue_57/_-x__dev_sdb
+-rw-r--r--   0 runner    (1001) docker     (123)    10217 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/sas_ssd_0_issue_57/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.886847 pySMART-1.2.5.dev24/tests/dataset/singletests/sat_hdd_0_issue70/
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/sat_hdd_0_issue70/_-d_sat_--all__dev_sg2
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/sat_hdd_0_issue70/_-d_test__dev_sg2
+-rw-r--r--   0 runner    (1001) docker     (123)    20777 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/sat_hdd_0_issue70/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.886847 pySMART-1.2.5.dev24/tests/dataset/singletests/sat_ssd_0_issue_65/
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/sat_ssd_0_issue_65/_-d_sat_--all__dev_sda
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/sat_ssd_0_issue_65/_-d_test__dev_sda
+-rw-r--r--   0 runner    (1001) docker     (123)    22000 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/sat_ssd_0_issue_65/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.886847 pySMART-1.2.5.dev24/tests/dataset/singletests/sata_hdd_0_issue42/
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/sata_hdd_0_issue42/_-d_ata_--all__dev_sdau
+-rw-r--r--   0 runner    (1001) docker     (123)    23712 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/sata_hdd_0_issue42/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.886847 pySMART-1.2.5.dev24/tests/dataset/singletests/sata_hdd_1_issue46/
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/sata_hdd_1_issue46/_-d_ata_--all__dev_sdau
+-rw-r--r--   0 runner    (1001) docker     (123)    17621 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/sata_hdd_1_issue46/device.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17855 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/sata_hdd_1_issue46/heliumhdd.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.886847 pySMART-1.2.5.dev24/tests/dataset/singletests/sata_ssd_0_issue_49/
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/sata_ssd_0_issue_49/_-d_ata_--all__dev_sda
+-rw-r--r--   0 runner    (1001) docker     (123)    20400 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/sata_ssd_0_issue_49/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.886847 pySMART-1.2.5.dev24/tests/dataset/singletests/sata_ssd_1_issue_72/
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/sata_ssd_1_issue_72/_-d_ata_--all__dev_sda
+-rw-r--r--   0 runner    (1001) docker     (123)    23567 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/sata_ssd_1_issue_72/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.886847 pySMART-1.2.5.dev24/tests/dataset/singletests/sata_ssd_macos_0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/sata_ssd_macos_0/_-d_ata_--all_IOService__AppleACPIPlatformExpert_PCI0@0_AppleACPIPCI_RP06@1C,5_IOPP_SSD0@0_AppleAHCI_PRT0@0_IOAHCIDevice@0_AppleAHCIDiskDriver_IOAHCIBlockStorageDevice
+-rw-r--r--   0 runner    (1001) docker     (123)    15407 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/sata_ssd_macos_0/device.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 10:00:31.886847 pySMART-1.2.5.dev24/tests/dataset/singletests/usb_ssd_0_issue_50/
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/usb_ssd_0_issue_50/_-d_ata_--all__dev_sda
+-rw-r--r--   0 runner    (1001) docker     (123)    25889 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/usb_ssd_0_issue_50/device.json
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/dataset/singletests/usb_ssd_0_issue_50/notes.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/gen_devicejson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/smartctlfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-31 10:00:08.000000 pySMART-1.2.5.dev24/tests/test_device_list.py
```

### Comparing `pySMART-1.2.5.dev23/.github/ISSUE_TEMPLATE/bug_report.md` & `pySMART-1.2.5.dev24/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/.github/workflows/check.yml` & `pySMART-1.2.5.dev24/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/.github/workflows/publish-to-test-pypi.yml` & `pySMART-1.2.5.dev24/.github/workflows/publish-to-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/CHANGELOG.md` & `pySMART-1.2.5.dev24/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Version 1.2.5
 =============
 - Minnor fix on serial NVME readings (MR [#69](https://github.com/truenas/py-SMART/pull/69)). Thanks @Heidistein
 - Minnor fix on reads/writes NVME readings (MR [#71](https://github.com/truenas/py-SMART/pull/71). Thanks @Heidistein
 - Fixed capacity detection in some devices & envirorments (issue [#72](https://github.com/truenas/py-SMART/issues/72)). Thanks @Shablykinm
-
+- Now file/process encodings are automatically detected. This whould fix issue [#72](https://github.com/truenas/py-SMART/issues/72)).
 
 Version 1.2.4
 =============
 - [dev tools] Test reorganization
 - [dev tools] Added new tests (issues [#46](https://github.com/truenas/py-SMART/issues/46))
 - Fixed parsing of NVMe devices on some systems / languages (issue [#63](https://github.com/truenas/py-SMART/issues/63))
 - Fixed parsing of NVMe tests on smartmontools >=7.4 (issue [#64](https://github.com/truenas/py-SMART/issues/64))
```

### Comparing `pySMART-1.2.5.dev23/LICENSE` & `pySMART-1.2.5.dev24/LICENSE`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/PKG-INFO` & `pySMART-1.2.5.dev24/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pySMART
-Version: 1.2.5.dev23
+Version: 1.2.5.dev24
 Summary: Wrapper for smartctl (smartmontools)
 Author-email: Rafael Leira <rafael.leira@naudit.es>, Marc Herndon <Herndon.MarcT@gmail.com>
 License: GNU LGPLv2.1
 Project-URL: Homepage, https://github.com/truenas/py-SMART
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
```

### Comparing `pySMART-1.2.5.dev23/README.md` & `pySMART-1.2.5.dev24/README.md`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/docs/pySMART/utils.html` & `pySMART-1.2.5.dev24/docs/pySMART/utils.html`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/docs/pySMART.html` & `pySMART-1.2.5.dev24/docs/pySMART.html`

 * *Files 0% similar despite different names*

```diff
@@ -4378,15 +4378,15 @@
 00011190: 7220 7661 7269 6162 6c65 223e 0a20 2020  r variable">.   
 000111a0: 2020 2020 2020 2020 203c 7370 616e 2063           <span c
 000111b0: 6c61 7373 3d22 6e61 6d65 223e 5f5f 7665  lass="name">__ve
 000111c0: 7273 696f 6e5f 5f3c 2f73 7061 6e3e 2020  rsion__</span>  
 000111d0: 2020 2020 2020 3d0a 3c73 7061 6e20 636c        =.<span cl
 000111e0: 6173 733d 2264 6566 6175 6c74 5f76 616c  ass="default_val
 000111f0: 7565 223e 2623 3339 3b31 2e32 2e35 2e64  ue">&#39;1.2.5.d
-00011200: 6576 3233 2623 3339 3b3c 2f73 7061 6e3e  ev23&#39;</span>
+00011200: 6576 3234 2623 3339 3b3c 2f73 7061 6e3e  ev24&#39;</span>
 00011210: 0a0a 2020 2020 2020 2020 0a20 2020 203c  ..        .    <
 00011220: 2f64 6976 3e0a 2020 2020 3c61 2063 6c61  /div>.    <a cla
 00011230: 7373 3d22 6865 6164 6572 6c69 6e6b 2220  ss="headerlink" 
 00011240: 6872 6566 3d22 235f 5f76 6572 7369 6f6e  href="#__version
 00011250: 5f5f 223e 3c2f 613e 0a20 2020 200a 2020  __"></a>.    .  
 00011260: 2020 0a0a 2020 2020 2020 2020 2020 2020    ..            
 00011270: 2020 2020 3c2f 7365 6374 696f 6e3e 0a20      </section>. 
@@ -4399,15 +4399,15 @@
 000112e0: 2020 2020 2020 2020 2020 2020 3c73 7061              <spa
 000112f0: 6e20 636c 6173 733d 226e 616d 6522 3e5f  n class="name">_
 00011300: 5f76 6572 7369 6f6e 5f74 7570 6c65 5f5f  _version_tuple__
 00011310: 3c2f 7370 616e 3e20 2020 2020 2020 203d  </span>        =
 00011320: 0a3c 7370 616e 2063 6c61 7373 3d22 6465  .<span class="de
 00011330: 6661 756c 745f 7661 6c75 6522 3e28 312c  fault_value">(1,
 00011340: 2032 2c20 352c 2026 2333 393b 6465 7632   2, 5, &#39;dev2
-00011350: 3326 2333 393b 293c 2f73 7061 6e3e 0a0a  3&#39;)</span>..
+00011350: 3426 2333 393b 293c 2f73 7061 6e3e 0a0a  4&#39;)</span>..
 00011360: 2020 2020 2020 2020 0a20 2020 203c 2f64          .    </d
 00011370: 6976 3e0a 2020 2020 3c61 2063 6c61 7373  iv>.    <a class
 00011380: 3d22 6865 6164 6572 6c69 6e6b 2220 6872  ="headerlink" hr
 00011390: 6566 3d22 235f 5f76 6572 7369 6f6e 5f74  ef="#__version_t
 000113a0: 7570 6c65 5f5f 223e 3c2f 613e 0a20 2020  uple__"></a>.   
 000113b0: 200a 2020 2020 0a0a 2020 2020 2020 2020   .    ..        
 000113c0: 2020 2020 2020 2020 3c2f 7365 6374 696f          </sectio
```

#### html2text {}

```diff
@@ -374,17 +374,17 @@
 155
 156__all__ = [
 157    '__version__', '__version_tuple__',
 158    'TestEntry', 'Attribute', 'utils', 'SMARTCTL', 'DeviceList', 'Device',
 159    'smart_health_assement'
 160]
 
-__version__ = '1.2.5.dev23'
+__version__ = '1.2.5.dev24'
 
-__version_tuple__ = (1, 2, 5, 'dev23')
+__version_tuple__ = (1, 2, 5, 'dev24')
    ⁰
 class TestEntry: View Source
 _27class TestEntry(object):
 _28    """
 _29    Contains all of the information associated with a single SMART Self-test
 _30    log entry. This data is intended to exactly mirror that obtained through
 _31    smartctl.
```

### Comparing `pySMART-1.2.5.dev23/docs/search.js` & `pySMART-1.2.5.dev24/docs/search.js`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/pySMART/__init__.py` & `pySMART-1.2.5.dev24/pySMART/__init__.py`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/pySMART/attribute.py` & `pySMART-1.2.5.dev24/pySMART/attribute.py`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/pySMART/device.py` & `pySMART-1.2.5.dev24/pySMART/device.py`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/pySMART/device_list.py` & `pySMART-1.2.5.dev24/pySMART/device_list.py`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/pySMART/diagnostics.py` & `pySMART-1.2.5.dev24/pySMART/diagnostics.py`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/pySMART/interface/__init__.py` & `pySMART-1.2.5.dev24/pySMART/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/pySMART/interface/nvme.py` & `pySMART-1.2.5.dev24/pySMART/interface/nvme.py`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/pySMART/smartctl.py` & `pySMART-1.2.5.dev24/pySMART/smartctl.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # MA  02110-1301, USA.
 #
 ################################################################
 from subprocess import Popen, PIPE
 from .utils import SMARTCTL_PATH
 from typing import List, Tuple, Union, Optional
 
+import chardet
 import logging
 import os
 
 logger = logging.getLogger('pySMART')
 
 os.environ["LANG"] = "C"
 
@@ -141,17 +142,45 @@
             cmd (List[str]): The command to be executed
 
         Returns:
             Tuple[List[str], int]: A raw line-by-line output from smartctl and the process return code
         """
         proc = Popen(cmd, stdout=PIPE, stderr=PIPE)
 
-        _stdout, _stderr = [i.decode('utf8') for i in proc.communicate()]
+        _stdout, _stderr = [i for i in proc.communicate()]
 
-        return _stdout.split('\n'), proc.returncode
+        return self._decode_output(_stdout), proc.returncode
+
+    def _decode_output(self, raw_output: bytes) -> List[str]:
+        """ Decodes the raw output from smartctl
+            This, should detect the encoding and decode the output
+
+        Args:
+            raw_output (bytes): The raw output from smartctl
+
+        Returns:
+            List[str]: A raw line-by-line output from smartctl
+        """
+        # Detect the encoding
+        encoding: Optional[str] = None
+        try:
+            encoding = chardet.detect(raw_output)['encoding']
+        except:
+            pass
+
+        if not encoding:
+            encoding = 'utf-8'
+
+        if encoding not in ['utf-8', 'ascii']:
+            logger.warning(f"Detected encoding: {encoding}")
+
+        # Decode the output
+        decoded_output = raw_output.decode(encoding).splitlines()
+
+        return decoded_output
 
     def scan(self) -> List[str]:
         """Queries smartctl with option --scan-open
 
         Returns:
             List[str]: A raw line-by-line output from smartctl
         """
```

### Comparing `pySMART-1.2.5.dev23/pySMART/testentry.py` & `pySMART-1.2.5.dev24/pySMART/testentry.py`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/pySMART/utils.py` & `pySMART-1.2.5.dev24/pySMART/utils.py`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/pySMART.egg-info/PKG-INFO` & `pySMART-1.2.5.dev24/pySMART.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pySMART
-Version: 1.2.5.dev23
+Version: 1.2.5.dev24
 Summary: Wrapper for smartctl (smartmontools)
 Author-email: Rafael Leira <rafael.leira@naudit.es>, Marc Herndon <Herndon.MarcT@gmail.com>
 License: GNU LGPLv2.1
 Project-URL: Homepage, https://github.com/truenas/py-SMART
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
```

### Comparing `pySMART-1.2.5.dev23/pySMART.egg-info/SOURCES.txt` & `pySMART-1.2.5.dev24/pySMART.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/pyproject.toml` & `pySMART-1.2.5.dev24/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Topic :: Software Development',
     'Topic :: Software Development :: Libraries',
     'Topic :: Software Development :: Libraries :: Python Modules',
 ]
-dependencies = ['humanfriendly']
+dependencies = ["chardet", 'humanfriendly']
 dynamic = ["version"]
 
 
 [project.urls]
 "Homepage" = "https://github.com/truenas/py-SMART"
 
 [project.optional-dependencies]
```

### Comparing `pySMART-1.2.5.dev23/tests/README.md` & `pySMART-1.2.5.dev24/tests/README.md`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/__init__.py` & `pySMART-1.2.5.dev24/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/listingtests/linux_01/_-d_nvme_--all__dev_nvme0` & `pySMART-1.2.5.dev24/tests/dataset/listingtests/linux_01/_-d_nvme_--all__dev_nvme0`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/listingtests/linux_multiple_devices/_-d_nvme_--all__dev_nvme0` & `pySMART-1.2.5.dev24/tests/dataset/listingtests/linux_multiple_devices/_-d_nvme_--all__dev_nvme0`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/listingtests/linux_multiple_devices/_-d_nvme_--all__dev_nvme1` & `pySMART-1.2.5.dev24/tests/dataset/listingtests/linux_multiple_devices/_-d_nvme_--all__dev_nvme1`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/listingtests/linux_multiple_devices/_-d_sat+megaraid,60_--all__dev_bus_0` & `pySMART-1.2.5.dev24/tests/dataset/listingtests/linux_multiple_devices/_-d_sat+megaraid,60_--all__dev_bus_0`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/listingtests/mac_01/_-d_ata_--all_IOService__AppleACPIPlatformExpert_PCI0@0_AppleACPIPCI_RP06@1C,5_IOPP_SSD0@0_AppleAHCI_PRT0@0_IOAHCIDevice@0_AppleAHCIDiskDriver_IOAHCIBlockStorageDevice` & `pySMART-1.2.5.dev24/tests/dataset/listingtests/mac_01/_-d_ata_--all_IOService__AppleACPIPlatformExpert_PCI0@0_AppleACPIPCI_RP06@1C,5_IOPP_SSD0@0_AppleAHCI_PRT0@0_IOAHCIDevice@0_AppleAHCIDiskDriver_IOAHCIBlockStorageDevice`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/listingtests/win10_01/_-d_nvme_--all__dev_sda` & `pySMART-1.2.5.dev24/tests/dataset/listingtests/win10_01/_-d_nvme_--all__dev_sda`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/megaraid_ph_sas_hdd_0/_-d_megaraid,44_--all__dev_bus_7` & `pySMART-1.2.5.dev24/tests/dataset/singletests/megaraid_ph_sas_hdd_0/_-d_megaraid,44_--all__dev_bus_7`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/megaraid_ph_sas_hdd_0/device.json` & `pySMART-1.2.5.dev24/tests/dataset/singletests/megaraid_ph_sas_hdd_0/device.json`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/megaraid_ph_sata_hdd_0/_-d_megaraid,16_--all__dev_bus_0` & `pySMART-1.2.5.dev24/tests/dataset/singletests/megaraid_ph_sata_hdd_0/_-d_megaraid,16_--all__dev_bus_0`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/megaraid_ph_sata_hdd_0/device.json` & `pySMART-1.2.5.dev24/tests/dataset/singletests/megaraid_ph_sata_hdd_0/device.json`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/megaraid_ph_sata_hdd_1_issue_56/_-d_sat+megaraid,60_--all__dev_bus_0` & `pySMART-1.2.5.dev24/tests/dataset/singletests/megaraid_ph_sata_hdd_1_issue_56/_-d_sat+megaraid,60_--all__dev_bus_0`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/megaraid_ph_sata_hdd_1_issue_56/device.json` & `pySMART-1.2.5.dev24/tests/dataset/singletests/megaraid_ph_sata_hdd_1_issue_56/device.json`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/megaraid_ph_sata_ssd_0/_-d_megaraid,28_--all__dev_bus_0` & `pySMART-1.2.5.dev24/tests/dataset/singletests/megaraid_ph_sata_ssd_0/_-d_megaraid,28_--all__dev_bus_0`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/megaraid_ph_sata_ssd_0/device.json` & `pySMART-1.2.5.dev24/tests/dataset/singletests/megaraid_ph_sata_ssd_0/device.json`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/megaraid_vd_0/_-d_scsi_--all__dev_sda` & `pySMART-1.2.5.dev24/tests/dataset/singletests/megaraid_vd_0/_-d_scsi_--all__dev_sda`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/megaraid_vd_0/device.json` & `pySMART-1.2.5.dev24/tests/dataset/singletests/megaraid_vd_0/device.json`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_0/_-d_nvme_--all__dev_nvme0` & `pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_0/_-d_nvme_--all__dev_nvme0`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_0/device.json` & `pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_0/device.json`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_1_issue_37/_-d_nvme_--all__dev_nvme0` & `pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_1_issue_37/_-d_nvme_--all__dev_nvme0`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_1_issue_37/device.json` & `pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_1_issue_37/device.json`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_2_issue_46/_-d_nvme_--all__dev_nvme0` & `pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_2_issue_46/_-d_nvme_--all__dev_nvme0`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_2_issue_46/device.json` & `pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_2_issue_46/device.json`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_3_issue_52/_-d_nvme_--all__dev_nvme0n1` & `pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_3_issue_52/_-d_nvme_--all__dev_nvme0n1`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_3_issue_52/device.json` & `pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_3_issue_52/device.json`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_4_issue_53/_-d_nvme_--all__dev_nvme0` & `pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_4_issue_53/_-d_nvme_--all__dev_nvme0`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_4_issue_53/device.json` & `pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_4_issue_53/device.json`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_5_issue_46/_-d_nvme_--all__dev_nvme0` & `pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_5_issue_46/_-d_nvme_--all__dev_nvme0`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_5_issue_46/device.json` & `pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_5_issue_46/device.json`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_5_issue_46/nvmessd.json` & `pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_5_issue_46/nvmessd.json`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_6/_-d_nvme_--all__dev_nvme0` & `pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_6/_-d_nvme_--all__dev_nvme0`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_6/device.json` & `pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_6/device.json`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_7_issue_63/_-d_nvme_--all__dev_nvme0n1` & `pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_7_issue_63/_-d_nvme_--all__dev_nvme0n1`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_7_issue_63/device.json` & `pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_7_issue_63/device.json`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_8/_-d_nvme_--all__dev_nvme0n1` & `pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_8/_-d_nvme_--all__dev_nvme0n1`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_8/device.json` & `pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_8/device.json`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_win10_0_issue_64/_-d_nvme_--all__dev_sda` & `pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_win10_0_issue_64/_-d_nvme_--all__dev_sda`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_win10_0_issue_64/device.json` & `pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_win10_0_issue_64/device.json`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_win10_mingw32_0_issue_48/_-d_nvme_--all__dev_sda` & `pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_win10_mingw32_0_issue_48/_-d_nvme_--all__dev_sda`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_win10_mingw32_0_issue_48/_-d_nvme_--all_sda` & `pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_win10_mingw32_0_issue_48/_-d_nvme_--all_sda`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/nvme_win10_mingw32_0_issue_48/device.json` & `pySMART-1.2.5.dev24/tests/dataset/singletests/nvme_win10_mingw32_0_issue_48/device.json`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/sas_hdd_0_issue_51/_-d_scsi_--all__dev_sdc` & `pySMART-1.2.5.dev24/tests/dataset/singletests/sas_hdd_0_issue_51/_-d_scsi_--all__dev_sdc`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/sas_hdd_0_issue_51/device.json` & `pySMART-1.2.5.dev24/tests/dataset/singletests/sas_hdd_0_issue_51/device.json`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/sas_ssd_0_issue_57/_-d_scsi_--all__dev_sdb` & `pySMART-1.2.5.dev24/tests/dataset/singletests/sas_ssd_0_issue_57/_-d_scsi_--all__dev_sdb`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/sas_ssd_0_issue_57/_-x__dev_sdb` & `pySMART-1.2.5.dev24/tests/dataset/singletests/sas_ssd_0_issue_57/_-x__dev_sdb`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/sas_ssd_0_issue_57/device.json` & `pySMART-1.2.5.dev24/tests/dataset/singletests/sas_ssd_0_issue_57/device.json`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/sat_hdd_0_issue70/_-d_sat_--all__dev_sg2` & `pySMART-1.2.5.dev24/tests/dataset/singletests/sat_hdd_0_issue70/_-d_sat_--all__dev_sg2`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/sat_hdd_0_issue70/device.json` & `pySMART-1.2.5.dev24/tests/dataset/singletests/sat_hdd_0_issue70/device.json`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/sat_ssd_0_issue_65/_-d_sat_--all__dev_sda` & `pySMART-1.2.5.dev24/tests/dataset/singletests/sat_ssd_0_issue_65/_-d_sat_--all__dev_sda`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/sat_ssd_0_issue_65/device.json` & `pySMART-1.2.5.dev24/tests/dataset/singletests/sat_ssd_0_issue_65/device.json`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/sata_hdd_0_issue42/_-d_ata_--all__dev_sdau` & `pySMART-1.2.5.dev24/tests/dataset/singletests/sata_hdd_0_issue42/_-d_ata_--all__dev_sdau`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/sata_hdd_0_issue42/device.json` & `pySMART-1.2.5.dev24/tests/dataset/singletests/sata_hdd_0_issue42/device.json`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/sata_hdd_1_issue46/_-d_ata_--all__dev_sdau` & `pySMART-1.2.5.dev24/tests/dataset/singletests/sata_hdd_1_issue46/_-d_ata_--all__dev_sdau`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/sata_hdd_1_issue46/device.json` & `pySMART-1.2.5.dev24/tests/dataset/singletests/sata_hdd_1_issue46/device.json`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/sata_hdd_1_issue46/heliumhdd.json` & `pySMART-1.2.5.dev24/tests/dataset/singletests/sata_hdd_1_issue46/heliumhdd.json`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/sata_ssd_0_issue_49/_-d_ata_--all__dev_sda` & `pySMART-1.2.5.dev24/tests/dataset/singletests/sata_ssd_0_issue_49/_-d_ata_--all__dev_sda`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/sata_ssd_0_issue_49/device.json` & `pySMART-1.2.5.dev24/tests/dataset/singletests/sata_ssd_0_issue_49/device.json`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/sata_ssd_1_issue_72/_-d_ata_--all__dev_sda` & `pySMART-1.2.5.dev24/tests/dataset/singletests/sata_ssd_1_issue_72/_-d_ata_--all__dev_sda`

 * *Files 10% similar despite different names*

```diff
@@ -1,102 +1,103 @@
-smartctl 7.3 2022-02-28 r5338 [x86_64-w64-mingw32-w10-b19045] (sf-7.3-1)
-Copyright (C) 2002-22, Bruce Allen, Christian Franke, www.smartmontools.org
-
-=== START OF INFORMATION SECTION ===
-Model Family:     Apacer AS340 SSDs
-Device Model:     Apacer AS340 240GB
-Serial Number:    LKC125R001176
-LU WWN Device Id: 5 02b2a2 01d1c1b1a
-Add. Product Id:  mavlsata
-Firmware Version: V4.25.0
-User Capacity:    240 057 409 536 bytes [240 GB]
-Sector Size:      512 bytes logical/physical
-Rotation Rate:    Solid State Device
-TRIM Command:     Available
-Device is:        In smartctl database 7.3/5319
-ATA Version is:   ACS-3 T13/2161-D revision 4
-SATA Version is:  SATA 3.2, 6.0 Gb/s (current: 6.0 Gb/s)
-Local Time is:    Fri May 26 11:16:44 2023 RTZ
-SMART support is: Available - device has SMART capability.
-SMART support is: Enabled
-
-=== START OF READ SMART DATA SECTION ===
-SMART overall-health self-assessment test result: PASSED
-
-General SMART Values:
-Offline data collection status:  (0x02) Offline data collection activity
-                                        was completed without error.
-                                        Auto Offline Data Collection: Disabled.
-Self-test execution status:      (   0) The previous self-test routine completed
-                                        without error or no self-test has ever
-                                        been run.
-Total time to complete Offline
-data collection:                (    0) seconds.
-Offline data collection
-capabilities:                    (0x75) SMART execute Offline immediate.
-                                        No Auto Offline data collection support.
-                                        Abort Offline collection upon new
-                                        command.
-                                        No Offline surface scan supported.
-                                        Self-test supported.
-                                        Conveyance Self-test supported.
-                                        Selective Self-test supported.
-SMART capabilities:            (0x0002) Does not save SMART data before
-                                        entering power-saving mode.
-                                        Supports SMART auto save timer.
-Error logging capability:        (0x00) Error logging NOT supported.
-                                        General Purpose Logging supported.
-Short self-test routine
-recommended polling time:        (   2) minutes.
-Extended self-test routine
-recommended polling time:        (  90) minutes.
-Conveyance self-test routine
-recommended polling time:        (   2) minutes.
-
-SMART Attributes Data Structure revision number: 5
-Vendor Specific SMART Attributes with Thresholds:
-ID# ATTRIBUTE_NAME          FLAG     VALUE WORST THRESH TYPE      UPDATED  WHEN_FAILED RAW_VALUE
-  5 Reallocated_Sector_Ct   0x0033   100   100   010    Pre-fail  Always       -       0
-  9 Power_On_Hours          0x0033   100   100   010    Pre-fail  Always       -       3517
- 12 Power_Cycle_Count       0x0033   100   100   010    Pre-fail  Always       -       7
-161 Unknown_Attribute       0x0033   100   100   010    Pre-fail  Always       -       0
-164 Average_Erase_Count     0x0033   100   100   010    Pre-fail  Always       -       66135
-165 Unknown_Attribute       0x0033   100   100   010    Pre-fail  Always       -       87
-166 Later_Bad_Block_Count   0x0033   100   100   010    Pre-fail  Always       -       3
-167 SSD_Protect_Mode        0x0033   100   100   010    Pre-fail  Always       -       64
-169 Unknown_Attribute       0x0033   100   100   010    Pre-fail  Always       -       0
-176 Erase_Fail_Count_Chip   0x0033   100   100   010    Pre-fail  Always       -       0
-177 Wear_Leveling_Count     0x0033   100   100   010    Pre-fail  Always       -       0
-178 Used_Rsvd_Blk_Cnt_Chip  0x0033   100   100   010    Pre-fail  Always       -       0
-192 Unexpect_Power_Loss_Ct  0x0033   100   100   010    Pre-fail  Always       -       0
-194 Temperature_Celsius     0x0033   100   100   010    Pre-fail  Always       -       47
-195 Hardware_ECC_Recovered  0x0033   100   100   010    Pre-fail  Always       -       0
-199 UDMA_CRC_Error_Count    0x0033   100   100   010    Pre-fail  Always       -       0
-241 Total_LBAs_Written      0x0033   100   100   010    Pre-fail  Always       -       3848
-242 Total_LBAs_Read         0x0033   100   100   010    Pre-fail  Always       -       1268
-243 Unknown_Attribute       0x0033   100   100   010    Pre-fail  Always       -       0
-244 Unknown_Attribute       0x0033   100   100   010    Pre-fail  Always       -       0
-245 Unknown_Attribute       0x0033   100   100   010    Pre-fail  Always       -       0
-246 Unknown_Attribute       0x0033   100   100   010    Pre-fail  Always       -       0
-248 Unknown_Attribute       0x0033   100   100   010    Pre-fail  Always       -       0
-249 Unknown_Attribute       0x0033   100   100   010    Pre-fail  Always       -       0
-250 Read_Error_Retry_Rate   0x0033   100   100   010    Pre-fail  Always       -       0
-251 Unknown_Attribute       0x0033   100   100   010    Pre-fail  Always       -       0
-252 Unknown_Attribute       0x0033   100   100   010    Pre-fail  Always       -       0
-253 Unknown_Attribute       0x0033   100   100   010    Pre-fail  Always       -       0
-254 Unknown_SSD_Attribute   0x0033   100   100   010    Pre-fail  Always       -       0
-
-SMART Error Log not supported
-
-SMART Self-test log structure revision number 1
-No self-tests have been logged.  [To run self-tests, use: smartctl -t]
-
-SMART Selective self-test log data structure revision number 1
- SPAN  MIN_LBA  MAX_LBA  CURRENT_TEST_STATUS
-    1        0        0  Not_testing
-    2        0        0  Not_testing
-    3        0        0  Not_testing
-    4        0        0  Not_testing
-    5        0        0  Not_testing
-Selective self-test flags (0x0):
-  After scanning selected spans, do NOT read-scan remainder of disk.
-If Selective self-test is pending on power-up, resume after 0 minute delay.
+smartctl 7.3 2022-02-28 r5338 [x86_64-w64-mingw32-w10-b19045] (sf-7.3-1)
+Copyright (C) 2002-22, Bruce Allen, Christian Franke, www.smartmontools.org
+
+=== START OF INFORMATION SECTION ===
+Model Family:     Apacer AS340 SSDs
+Device Model:     Apacer AS340 240GB
+Serial Number:    LKC125R001176
+LU WWN Device Id: 5 02b2a2 01d1c1b1a
+Add. Product Id:  mavlsata
+Firmware Version: V4.25.0
+User Capacity:    240 057 409 536 bytes [240 GB]
+Sector Size:      512 bytes logical/physical
+Rotation Rate:    Solid State Device
+TRIM Command:     Available
+Device is:        In smartctl database 7.3/5319
+ATA Version is:   ACS-3 T13/2161-D revision 4
+SATA Version is:  SATA 3.2, 6.0 Gb/s (current: 6.0 Gb/s)
+Local Time is:    Fri May 26 13:33:02 2023 RTZ
+SMART support is: Available - device has SMART capability.
+SMART support is: Enabled
+
+=== START OF READ SMART DATA SECTION ===
+SMART overall-health self-assessment test result: PASSED
+
+General SMART Values:
+Offline data collection status:  (0x02)	Offline data collection activity
+					was completed without error.
+					Auto Offline Data Collection: Disabled.
+Self-test execution status:      (   0)	The previous self-test routine completed
+					without error or no self-test has ever 
+					been run.
+Total time to complete Offline 
+data collection: 		(    0) seconds.
+Offline data collection
+capabilities: 			 (0x75) SMART execute Offline immediate.
+					No Auto Offline data collection support.
+					Abort Offline collection upon new
+					command.
+					No Offline surface scan supported.
+					Self-test supported.
+					Conveyance Self-test supported.
+					Selective Self-test supported.
+SMART capabilities:            (0x0002)	Does not save SMART data before
+					entering power-saving mode.
+					Supports SMART auto save timer.
+Error logging capability:        (0x00)	Error logging NOT supported.
+					General Purpose Logging supported.
+Short self-test routine 
+recommended polling time: 	 (   2) minutes.
+Extended self-test routine
+recommended polling time: 	 (  90) minutes.
+Conveyance self-test routine
+recommended polling time: 	 (   2) minutes.
+
+SMART Attributes Data Structure revision number: 5
+Vendor Specific SMART Attributes with Thresholds:
+ID# ATTRIBUTE_NAME          FLAG     VALUE WORST THRESH TYPE      UPDATED  WHEN_FAILED RAW_VALUE
+  5 Reallocated_Sector_Ct   0x0033   100   100   010    Pre-fail  Always       -       0
+  9 Power_On_Hours          0x0033   100   100   010    Pre-fail  Always       -       3519
+ 12 Power_Cycle_Count       0x0033   100   100   010    Pre-fail  Always       -       7
+161 Unknown_Attribute       0x0033   100   100   010    Pre-fail  Always       -       0
+164 Average_Erase_Count     0x0033   100   100   010    Pre-fail  Always       -       66179
+165 Unknown_Attribute       0x0033   100   100   010    Pre-fail  Always       -       87
+166 Later_Bad_Block_Count   0x0033   100   100   010    Pre-fail  Always       -       3
+167 SSD_Protect_Mode        0x0033   100   100   010    Pre-fail  Always       -       64
+169 Unknown_Attribute       0x0033   100   100   010    Pre-fail  Always       -       0
+176 Erase_Fail_Count_Chip   0x0033   100   100   010    Pre-fail  Always       -       0
+177 Wear_Leveling_Count     0x0033   100   100   010    Pre-fail  Always       -       0
+178 Used_Rsvd_Blk_Cnt_Chip  0x0033   100   100   010    Pre-fail  Always       -       0
+192 Unexpect_Power_Loss_Ct  0x0033   100   100   010    Pre-fail  Always       -       0
+194 Temperature_Celsius     0x0033   100   100   010    Pre-fail  Always       -       47
+195 Hardware_ECC_Recovered  0x0033   100   100   010    Pre-fail  Always       -       0
+199 UDMA_CRC_Error_Count    0x0033   100   100   010    Pre-fail  Always       -       0
+241 Total_LBAs_Written      0x0033   100   100   010    Pre-fail  Always       -       3851
+242 Total_LBAs_Read         0x0033   100   100   010    Pre-fail  Always       -       1268
+243 Unknown_Attribute       0x0033   100   100   010    Pre-fail  Always       -       0
+244 Unknown_Attribute       0x0033   100   100   010    Pre-fail  Always       -       0
+245 Unknown_Attribute       0x0033   100   100   010    Pre-fail  Always       -       0
+246 Unknown_Attribute       0x0033   100   100   010    Pre-fail  Always       -       0
+248 Unknown_Attribute       0x0033   100   100   010    Pre-fail  Always       -       0
+249 Unknown_Attribute       0x0033   100   100   010    Pre-fail  Always       -       0
+250 Read_Error_Retry_Rate   0x0033   100   100   010    Pre-fail  Always       -       0
+251 Unknown_Attribute       0x0033   100   100   010    Pre-fail  Always       -       0
+252 Unknown_Attribute       0x0033   100   100   010    Pre-fail  Always       -       0
+253 Unknown_Attribute       0x0033   100   100   010    Pre-fail  Always       -       0
+254 Unknown_SSD_Attribute   0x0033   100   100   010    Pre-fail  Always       -       0
+
+SMART Error Log not supported
+
+SMART Self-test log structure revision number 1
+No self-tests have been logged.  [To run self-tests, use: smartctl -t]
+
+SMART Selective self-test log data structure revision number 1
+ SPAN  MIN_LBA  MAX_LBA  CURRENT_TEST_STATUS
+    1        0        0  Not_testing
+    2        0        0  Not_testing
+    3        0        0  Not_testing
+    4        0        0  Not_testing
+    5        0        0  Not_testing
+Selective self-test flags (0x0):
+  After scanning selected spans, do NOT read-scan remainder of disk.
+If Selective self-test is pending on power-up, resume after 0 minute delay.
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+iso-8859-1
```

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/sata_ssd_1_issue_72/device.json` & `pySMART-1.2.5.dev24/tests/dataset/singletests/sata_ssd_1_issue_72/device.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999998031123992%*

 * *Differences: {"'values'": "{'attributes': {9: {'raw': '3519', 'raw_int': 3519}, 164: {'raw': '66179', "*

 * *             "'raw_int': 66179}, 241: {'raw': '3851', 'raw_int': 3851}}}"}*

```diff
@@ -34,16 +34,16 @@
             {
                 "_thresh": "010",
                 "_value": "100",
                 "_worst": "100",
                 "flags": 51,
                 "name": "Power_On_Hours",
                 "num": 9,
-                "raw": "3517",
-                "raw_int": 3517,
+                "raw": "3519",
+                "raw_int": 3519,
                 "thresh": 10,
                 "type": "Pre-fail",
                 "updated": "Always",
                 "value": "100",
                 "value_int": 100,
                 "value_str": "100",
                 "when_failed": "-",
@@ -240,16 +240,16 @@
             {
                 "_thresh": "010",
                 "_value": "100",
                 "_worst": "100",
                 "flags": 51,
                 "name": "Average_Erase_Count",
                 "num": 164,
-                "raw": "66135",
-                "raw_int": 66135,
+                "raw": "66179",
+                "raw_int": 66179,
                 "thresh": 10,
                 "type": "Pre-fail",
                 "updated": "Always",
                 "value": "100",
                 "value_int": 100,
                 "value_str": "100",
                 "when_failed": "-",
@@ -521,16 +521,16 @@
             {
                 "_thresh": "010",
                 "_value": "100",
                 "_worst": "100",
                 "flags": 51,
                 "name": "Total_LBAs_Written",
                 "num": 241,
-                "raw": "3848",
-                "raw_int": 3848,
+                "raw": "3851",
+                "raw_int": 3851,
                 "thresh": 10,
                 "type": "Pre-fail",
                 "updated": "Always",
                 "value": "100",
                 "value_int": 100,
                 "value_str": "100",
                 "when_failed": "-",
```

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/sata_ssd_macos_0/_-d_ata_--all_IOService__AppleACPIPlatformExpert_PCI0@0_AppleACPIPCI_RP06@1C,5_IOPP_SSD0@0_AppleAHCI_PRT0@0_IOAHCIDevice@0_AppleAHCIDiskDriver_IOAHCIBlockStorageDevice` & `pySMART-1.2.5.dev24/tests/dataset/singletests/sata_ssd_macos_0/_-d_ata_--all_IOService__AppleACPIPlatformExpert_PCI0@0_AppleACPIPCI_RP06@1C,5_IOPP_SSD0@0_AppleAHCI_PRT0@0_IOAHCIDevice@0_AppleAHCIDiskDriver_IOAHCIBlockStorageDevice`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/sata_ssd_macos_0/device.json` & `pySMART-1.2.5.dev24/tests/dataset/singletests/sata_ssd_macos_0/device.json`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/usb_ssd_0_issue_50/_-d_ata_--all__dev_sda` & `pySMART-1.2.5.dev24/tests/dataset/singletests/usb_ssd_0_issue_50/_-d_ata_--all__dev_sda`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/dataset/singletests/usb_ssd_0_issue_50/device.json` & `pySMART-1.2.5.dev24/tests/dataset/singletests/usb_ssd_0_issue_50/device.json`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/exceptions.py` & `pySMART-1.2.5.dev24/tests/exceptions.py`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/gen_devicejson.py` & `pySMART-1.2.5.dev24/tests/gen_devicejson.py`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/smartctlfile.py` & `pySMART-1.2.5.dev24/tests/smartctlfile.py`

 * *Files 16% similar despite different names*

```diff
@@ -55,15 +55,13 @@
 
         filename = os.path.join(
             self.smartctl_path, re.sub('[/\\\\:]', '_', filename))
 
         logger.trace("Opening file: {0}".format(filename))
 
         try:
-            with open(filename, encoding='utf-8') as f:
-                raw_data = f.readlines()
+            with open(filename, mode='rb') as f:
+                raw_data = f.read()
         except:
             raise SmartctlfileSampleNotFound(filename, final_params)
 
-        _stdout = [i.split('\n')[0] for i in raw_data]
-
-        return _stdout, 0
+        return self._decode_output(raw_data), 0
```

### Comparing `pySMART-1.2.5.dev23/tests/test_device.py` & `pySMART-1.2.5.dev24/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `pySMART-1.2.5.dev23/tests/test_device_list.py` & `pySMART-1.2.5.dev24/tests/test_device_list.py`

 * *Files identical despite different names*

