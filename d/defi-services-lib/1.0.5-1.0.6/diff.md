# Comparing `tmp/defi-services-lib-1.0.5.tar.gz` & `tmp/defi-services-lib-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "defi-services-lib-1.0.5.tar", last modified: Wed May 31 01:56:20 2023, max compression
+gzip compressed data, was "defi-services-lib-1.0.6.tar", last modified: Wed May 31 09:34:15 2023, max compression
```

## Comparing `defi-services-lib-1.0.5.tar` & `defi-services-lib-1.0.6.tar`

### file list

```diff
@@ -1,109 +1,119 @@
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 01:56:20.107939 defi-services-lib-1.0.5/
--rw-r--r--   0 vietbangpham   (501) staff       (20)     1129 2023-05-29 07:02:16.000000 defi-services-lib-1.0.5/LICENSE
--rw-r--r--   0 vietbangpham   (501) staff       (20)      840 2023-05-31 01:56:20.107331 defi-services-lib-1.0.5/PKG-INFO
--rw-r--r--   0 vietbangpham   (501) staff       (20)      259 2023-05-29 08:02:45.000000 defi-services-lib-1.0.5/README.md
--rw-r--r--   0 vietbangpham   (501) staff       (20)      107 2023-05-29 04:51:50.000000 defi-services-lib-1.0.5/pyproject.toml
--rw-r--r--   0 vietbangpham   (501) staff       (20)       38 2023-05-31 01:56:20.108199 defi-services-lib-1.0.5/setup.cfg
--rw-r--r--   0 vietbangpham   (501) staff       (20)     1201 2023-05-29 07:52:03.000000 defi-services-lib-1.0.5/setup.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 01:56:20.033667 defi-services-lib-1.0.5/src/
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 01:56:20.039715 defi-services-lib-1.0.5/src/defi_services/
--rw-r--r--   0 vietbangpham   (501) staff       (20)       22 2023-05-31 01:56:09.000000 defi-services-lib-1.0.5/src/defi_services/__init__.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 01:56:20.041974 defi-services-lib-1.0.5/src/defi_services/abis/
--rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:43:51.000000 defi-services-lib-1.0.5/src/defi_services/abis/__init__.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 01:56:20.044508 defi-services-lib-1.0.5/src/defi_services/abis/dex/
--rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:44:57.000000 defi-services-lib-1.0.5/src/defi_services/abis/dex/__init__.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    15950 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/dex/biswap_masterchef_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    18798 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/dex/pancakeswap_masterchef_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     5636 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/erc20_abi.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 01:56:20.060995 defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/
--rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:45:05.000000 defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/__init__.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    16070 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/alpaca_fair_launch_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    23376 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/alpaca_vault_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    10050 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/alpaca_vault_config_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     1418 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/chain_link_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    12726 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/chef_incentives_controller.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    43379 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/cream_comptroller_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    20100 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/cream_lens_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    23605 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/ctoken_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    29034 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/lending_pool_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     4399 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/oracle_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    13482 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/staked_incentives_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    21266 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/trava_lending_pool_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     4507 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/trava_oracle_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     9576 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/valas_multi_fee_distribution.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    43234 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/venus_comptroller_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    18613 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/venus_lens_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    14433 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/venus_lens_abi_v1.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 01:56:20.065693 defi-services-lib-1.0.5/src/defi_services/abis/vault/
--rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:45:15.000000 defi-services-lib-1.0.5/src/defi_services/abis/vault/__init__.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    12332 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/vault/incentive_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    31318 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/vault/trava_vault_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)      598 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/vault/valuator_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    38341 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/vault/ve_abi.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 01:56:20.069377 defi-services-lib-1.0.5/src/defi_services/constants/
--rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:45:24.000000 defi-services-lib-1.0.5/src/defi_services/constants/__init__.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)      136 2023-05-29 15:14:03.000000 defi-services-lib-1.0.5/src/defi_services/constants/chain_constant.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     1931 2023-05-30 10:36:00.000000 defi-services-lib-1.0.5/src/defi_services/constants/contract_address.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     2492 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/constants/db_constant.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)      792 2023-05-30 10:51:26.000000 defi-services-lib-1.0.5/src/defi_services/constants/mapping_constant.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)      181 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/constants/time_constant.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     1105 2023-05-30 09:09:58.000000 defi-services-lib-1.0.5/src/defi_services/defi_service.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 01:56:20.074462 defi-services-lib-1.0.5/src/defi_services/lending_pools/
--rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/__init__.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     2475 2023-05-31 01:51:18.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/aave_v2_service.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     2243 2023-05-31 01:51:18.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/compound_service.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     2543 2023-05-31 01:51:17.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/cream_service.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     2010 2023-05-31 01:51:18.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/geist_service.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 01:56:20.074964 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/
--rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/__init__.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 01:56:20.075676 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/arbitrum/
--rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/arbitrum/__init__.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     2635 2023-05-30 09:15:50.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/arbitrum/radiant_arbitrum.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 01:56:20.080083 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/bsc/
--rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/bsc/__init__.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     8306 2023-05-31 01:43:08.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/bsc/cream_bsc.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     2325 2023-05-31 01:44:35.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/bsc/radiant_bsc.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     3757 2023-05-31 01:44:35.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/bsc/trava_bsc.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     4095 2023-05-31 01:44:35.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/bsc/valas_bsc.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     4743 2023-05-31 01:44:35.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/bsc/venus_bsc.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 01:56:20.083384 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/ethereum/
--rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/ethereum/__init__.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    11944 2023-05-31 01:51:17.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/ethereum/aave_v2_eth.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     3674 2023-05-31 01:51:17.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/ethereum/compound_eth.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     1565 2023-05-31 01:39:39.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/ethereum/trava_eth.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 01:56:20.086131 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/fantom/
--rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/fantom/__init__.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     3257 2023-05-30 07:24:06.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/fantom/geist_ftm.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     1808 2023-05-30 07:34:54.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/fantom/trava_ftm.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 01:56:20.087314 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/optimism/
--rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/optimism/__init__.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 01:56:20.088819 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/polygon/
--rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/polygon/__init__.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     4448 2023-05-31 01:51:18.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/polygon/aave_v2_polygon.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     2078 2023-05-31 01:51:17.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/radiant_service.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 01:56:20.096660 defi-services-lib-1.0.5/src/defi_services/lending_pools/services/
--rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 14:38:12.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/services/__init__.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    13008 2023-05-30 08:59:53.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/services/aave_v2_state_service.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     4418 2023-05-30 10:39:37.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/services/compound_state_service.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    20627 2023-05-30 10:36:00.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/services/cream_state_service.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)      689 2023-05-30 07:24:06.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/services/geist_state_service.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     1060 2023-05-30 09:13:38.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/services/radiant_state_service.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    17188 2023-05-30 08:51:45.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/services/trava_state_service.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    15441 2023-05-30 08:59:53.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/services/valas_state_service.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    14936 2023-05-30 10:36:00.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/services/venus_state_service.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     2411 2023-05-31 01:51:17.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/trava_service.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     2004 2023-05-31 01:51:18.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/valas_service.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     2115 2023-05-31 01:51:17.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/venus_service.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     4360 2023-05-30 10:51:26.000000 defi-services-lib-1.0.5/src/defi_services/state_service.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 01:56:20.100935 defi-services-lib-1.0.5/src/defi_services/utils/
--rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:45:50.000000 defi-services-lib-1.0.5/src/defi_services/utils/__init__.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     1830 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/utils/batch_queries_service.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     6271 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/utils/graph_operations.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)      723 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/utils/market_service.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)      851 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/utils/memory_storage.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 01:56:20.106065 defi-services-lib-1.0.5/src/defi_services_lib.egg-info/
--rw-r--r--   0 vietbangpham   (501) staff       (20)      840 2023-05-31 01:56:19.000000 defi-services-lib-1.0.5/src/defi_services_lib.egg-info/PKG-INFO
--rw-r--r--   0 vietbangpham   (501) staff       (20)     4692 2023-05-31 01:56:20.000000 defi-services-lib-1.0.5/src/defi_services_lib.egg-info/SOURCES.txt
--rw-r--r--   0 vietbangpham   (501) staff       (20)        1 2023-05-31 01:56:20.000000 defi-services-lib-1.0.5/src/defi_services_lib.egg-info/dependency_links.txt
--rw-r--r--   0 vietbangpham   (501) staff       (20)       34 2023-05-31 01:56:20.000000 defi-services-lib-1.0.5/src/defi_services_lib.egg-info/requires.txt
--rw-r--r--   0 vietbangpham   (501) staff       (20)       14 2023-05-31 01:56:20.000000 defi-services-lib-1.0.5/src/defi_services_lib.egg-info/top_level.txt
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 09:34:15.286671 defi-services-lib-1.0.6/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     1129 2023-05-29 07:02:16.000000 defi-services-lib-1.0.6/LICENSE
+-rw-r--r--   0 vietbangpham   (501) staff       (20)      840 2023-05-31 09:34:15.286054 defi-services-lib-1.0.6/PKG-INFO
+-rw-r--r--   0 vietbangpham   (501) staff       (20)      259 2023-05-29 08:02:45.000000 defi-services-lib-1.0.6/README.md
+-rw-r--r--   0 vietbangpham   (501) staff       (20)      107 2023-05-29 04:51:50.000000 defi-services-lib-1.0.6/pyproject.toml
+-rw-r--r--   0 vietbangpham   (501) staff       (20)       38 2023-05-31 09:34:15.286888 defi-services-lib-1.0.6/setup.cfg
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     1201 2023-05-29 07:52:03.000000 defi-services-lib-1.0.6/setup.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 09:34:15.163043 defi-services-lib-1.0.6/src/
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 09:34:15.170229 defi-services-lib-1.0.6/src/defi_services/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)       22 2023-05-31 09:34:03.000000 defi-services-lib-1.0.6/src/defi_services/__init__.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 09:34:15.171985 defi-services-lib-1.0.6/src/defi_services/abis/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:43:51.000000 defi-services-lib-1.0.6/src/defi_services/abis/__init__.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 09:34:15.174932 defi-services-lib-1.0.6/src/defi_services/abis/dex/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:44:57.000000 defi-services-lib-1.0.6/src/defi_services/abis/dex/__init__.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    15950 2023-05-29 03:52:33.000000 defi-services-lib-1.0.6/src/defi_services/abis/dex/biswap_masterchef_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    18798 2023-05-29 03:52:33.000000 defi-services-lib-1.0.6/src/defi_services/abis/dex/pancakeswap_masterchef_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     5636 2023-05-29 03:52:33.000000 defi-services-lib-1.0.6/src/defi_services/abis/erc20_abi.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 09:34:15.202969 defi-services-lib-1.0.6/src/defi_services/abis/lending_pool/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:45:05.000000 defi-services-lib-1.0.6/src/defi_services/abis/lending_pool/__init__.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    18201 2023-05-31 03:35:00.000000 defi-services-lib-1.0.6/src/defi_services/abis/lending_pool/aave_v3_incentives_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    38831 2023-05-31 03:39:59.000000 defi-services-lib-1.0.6/src/defi_services/abis/lending_pool/aave_v3_lending_pool_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     4432 2023-05-31 03:39:59.000000 defi-services-lib-1.0.6/src/defi_services/abis/lending_pool/aave_v3_oracle_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    16070 2023-05-29 03:52:33.000000 defi-services-lib-1.0.6/src/defi_services/abis/lending_pool/alpaca_fair_launch_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    23376 2023-05-29 03:52:33.000000 defi-services-lib-1.0.6/src/defi_services/abis/lending_pool/alpaca_vault_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    10050 2023-05-29 03:52:33.000000 defi-services-lib-1.0.6/src/defi_services/abis/lending_pool/alpaca_vault_config_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     1418 2023-05-29 03:52:33.000000 defi-services-lib-1.0.6/src/defi_services/abis/lending_pool/chain_link_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    12726 2023-05-29 03:52:33.000000 defi-services-lib-1.0.6/src/defi_services/abis/lending_pool/chef_incentives_controller.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    43379 2023-05-29 03:52:33.000000 defi-services-lib-1.0.6/src/defi_services/abis/lending_pool/cream_comptroller_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    20100 2023-05-29 03:52:33.000000 defi-services-lib-1.0.6/src/defi_services/abis/lending_pool/cream_lens_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    23605 2023-05-29 03:52:33.000000 defi-services-lib-1.0.6/src/defi_services/abis/lending_pool/ctoken_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    29034 2023-05-29 03:52:33.000000 defi-services-lib-1.0.6/src/defi_services/abis/lending_pool/lending_pool_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     4399 2023-05-29 03:52:33.000000 defi-services-lib-1.0.6/src/defi_services/abis/lending_pool/oracle_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    13482 2023-05-29 03:52:33.000000 defi-services-lib-1.0.6/src/defi_services/abis/lending_pool/staked_incentives_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    21266 2023-05-29 03:52:33.000000 defi-services-lib-1.0.6/src/defi_services/abis/lending_pool/trava_lending_pool_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     4507 2023-05-29 03:52:33.000000 defi-services-lib-1.0.6/src/defi_services/abis/lending_pool/trava_oracle_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     9576 2023-05-29 03:52:33.000000 defi-services-lib-1.0.6/src/defi_services/abis/lending_pool/valas_multi_fee_distribution.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    43234 2023-05-29 03:52:33.000000 defi-services-lib-1.0.6/src/defi_services/abis/lending_pool/venus_comptroller_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    18613 2023-05-29 03:52:33.000000 defi-services-lib-1.0.6/src/defi_services/abis/lending_pool/venus_lens_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    14433 2023-05-29 03:52:33.000000 defi-services-lib-1.0.6/src/defi_services/abis/lending_pool/venus_lens_abi_v1.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 09:34:15.207160 defi-services-lib-1.0.6/src/defi_services/abis/vault/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:45:15.000000 defi-services-lib-1.0.6/src/defi_services/abis/vault/__init__.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    12332 2023-05-29 03:52:33.000000 defi-services-lib-1.0.6/src/defi_services/abis/vault/incentive_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    31318 2023-05-29 03:52:33.000000 defi-services-lib-1.0.6/src/defi_services/abis/vault/trava_vault_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)      598 2023-05-29 03:52:33.000000 defi-services-lib-1.0.6/src/defi_services/abis/vault/valuator_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    38341 2023-05-29 03:52:33.000000 defi-services-lib-1.0.6/src/defi_services/abis/vault/ve_abi.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 09:34:15.213043 defi-services-lib-1.0.6/src/defi_services/constants/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:45:24.000000 defi-services-lib-1.0.6/src/defi_services/constants/__init__.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)      136 2023-05-29 15:14:03.000000 defi-services-lib-1.0.6/src/defi_services/constants/chain_constant.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     1931 2023-05-30 10:36:00.000000 defi-services-lib-1.0.6/src/defi_services/constants/contract_address.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     2534 2023-05-31 03:51:31.000000 defi-services-lib-1.0.6/src/defi_services/constants/db_constant.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)      792 2023-05-30 10:51:26.000000 defi-services-lib-1.0.6/src/defi_services/constants/mapping_constant.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)      181 2023-05-29 03:52:33.000000 defi-services-lib-1.0.6/src/defi_services/constants/time_constant.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     1105 2023-05-30 09:09:58.000000 defi-services-lib-1.0.6/src/defi_services/defi_service.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 09:34:15.223256 defi-services-lib-1.0.6/src/defi_services/lending_pools/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/__init__.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     2538 2023-05-31 09:23:25.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/aave_v2_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     2882 2023-05-31 08:50:53.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/aave_v3_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     2354 2023-05-31 04:07:46.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/compound_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     2630 2023-05-31 04:07:46.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/cream_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     2097 2023-05-31 04:07:46.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/geist_service.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 09:34:15.224300 defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/__init__.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 09:34:15.226398 defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/arbitrum/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/arbitrum/__init__.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     3462 2023-05-31 07:41:55.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/arbitrum/aave_v3_arbitrum.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     2635 2023-05-31 03:28:10.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/arbitrum/radiant_arbitrum.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 09:34:15.231868 defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/bsc/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/bsc/__init__.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     8306 2023-05-31 01:43:08.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/bsc/cream_bsc.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     2325 2023-05-31 01:44:35.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/bsc/radiant_bsc.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     3757 2023-05-31 01:44:35.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/bsc/trava_bsc.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     4095 2023-05-31 01:44:35.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/bsc/valas_bsc.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     4743 2023-05-31 01:44:35.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/bsc/venus_bsc.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 09:34:15.236513 defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/ethereum/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/ethereum/__init__.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    11944 2023-05-31 07:10:09.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/ethereum/aave_v2_eth.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     5654 2023-05-31 07:41:55.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/ethereum/aave_v3_eth.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     3674 2023-05-31 01:51:17.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/ethereum/compound_eth.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     1565 2023-05-31 01:39:39.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/ethereum/trava_eth.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 09:34:15.242466 defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/fantom/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/fantom/__init__.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     3462 2023-05-31 07:41:55.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/fantom/aave_v3_ftm.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     3257 2023-05-30 07:24:06.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/fantom/geist_ftm.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     1808 2023-05-30 07:34:54.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/fantom/trava_ftm.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 09:34:15.245100 defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/optimism/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/optimism/__init__.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     4151 2023-05-31 07:41:55.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/optimism/aave_v3_optimism.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 09:34:15.248507 defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/polygon/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/polygon/__init__.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     4448 2023-05-31 08:55:32.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/polygon/aave_v2_polygon.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     6813 2023-05-31 07:41:55.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/polygon/aave_v3_polygon.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     2165 2023-05-31 04:07:46.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/radiant_service.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 09:34:15.273378 defi-services-lib-1.0.6/src/defi_services/lending_pools/services/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 14:38:12.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/services/__init__.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    14321 2023-05-31 09:32:46.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/services/aave_v2_state_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    20698 2023-05-31 08:50:53.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/services/aave_v3_state_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     4418 2023-05-30 10:39:37.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/services/compound_state_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    20627 2023-05-30 10:36:00.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/services/cream_state_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)      689 2023-05-30 07:24:06.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/services/geist_state_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     1060 2023-05-30 09:13:38.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/services/radiant_state_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    17188 2023-05-30 08:51:45.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/services/trava_state_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    15504 2023-05-31 04:07:46.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/services/valas_state_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    14936 2023-05-30 10:36:00.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/services/venus_state_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     2498 2023-05-31 04:07:46.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/trava_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     2091 2023-05-31 04:07:46.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/valas_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     2202 2023-05-31 04:07:46.000000 defi-services-lib-1.0.6/src/defi_services/lending_pools/venus_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     4360 2023-05-30 10:51:26.000000 defi-services-lib-1.0.6/src/defi_services/state_service.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 09:34:15.281561 defi-services-lib-1.0.6/src/defi_services/utils/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:45:50.000000 defi-services-lib-1.0.6/src/defi_services/utils/__init__.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     1830 2023-05-29 03:52:33.000000 defi-services-lib-1.0.6/src/defi_services/utils/batch_queries_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     6271 2023-05-29 03:52:33.000000 defi-services-lib-1.0.6/src/defi_services/utils/graph_operations.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)      723 2023-05-29 03:52:33.000000 defi-services-lib-1.0.6/src/defi_services/utils/market_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)      851 2023-05-29 03:52:33.000000 defi-services-lib-1.0.6/src/defi_services/utils/memory_storage.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 09:34:15.285139 defi-services-lib-1.0.6/src/defi_services_lib.egg-info/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)      840 2023-05-31 09:34:15.000000 defi-services-lib-1.0.6/src/defi_services_lib.egg-info/PKG-INFO
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     5379 2023-05-31 09:34:15.000000 defi-services-lib-1.0.6/src/defi_services_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        1 2023-05-31 09:34:15.000000 defi-services-lib-1.0.6/src/defi_services_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 vietbangpham   (501) staff       (20)       34 2023-05-31 09:34:15.000000 defi-services-lib-1.0.6/src/defi_services_lib.egg-info/requires.txt
+-rw-r--r--   0 vietbangpham   (501) staff       (20)       14 2023-05-31 09:34:15.000000 defi-services-lib-1.0.6/src/defi_services_lib.egg-info/top_level.txt
```

### Comparing `defi-services-lib-1.0.5/LICENSE` & `defi-services-lib-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/PKG-INFO` & `defi-services-lib-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: defi-services-lib
-Version: 1.0.5
+Version: 1.0.6
 Summary: Calculate apy, apr, and wallet information,... in decentralized applications.
 Home-page: https://github.com/phamvietbang/defi-services-lib
 Author: Viet-Bang Pham
 Author-email: phamvietbang2965@gmail.com
 Project-URL: Bug Tracker, https://github.com/phamvietbang/defi-services-lib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `defi-services-lib-1.0.5/setup.py` & `defi-services-lib-1.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/abis/dex/biswap_masterchef_abi.py` & `defi-services-lib-1.0.6/src/defi_services/abis/dex/biswap_masterchef_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/abis/dex/pancakeswap_masterchef_abi.py` & `defi-services-lib-1.0.6/src/defi_services/abis/dex/pancakeswap_masterchef_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/abis/erc20_abi.py` & `defi-services-lib-1.0.6/src/defi_services/abis/erc20_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/alpaca_fair_launch_abi.py` & `defi-services-lib-1.0.6/src/defi_services/abis/lending_pool/alpaca_fair_launch_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/alpaca_vault_abi.py` & `defi-services-lib-1.0.6/src/defi_services/abis/lending_pool/alpaca_vault_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/alpaca_vault_config_abi.py` & `defi-services-lib-1.0.6/src/defi_services/abis/lending_pool/alpaca_vault_config_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/chain_link_abi.py` & `defi-services-lib-1.0.6/src/defi_services/abis/lending_pool/chain_link_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/chef_incentives_controller.py` & `defi-services-lib-1.0.6/src/defi_services/abis/lending_pool/chef_incentives_controller.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/cream_comptroller_abi.py` & `defi-services-lib-1.0.6/src/defi_services/abis/lending_pool/cream_comptroller_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/cream_lens_abi.py` & `defi-services-lib-1.0.6/src/defi_services/abis/lending_pool/cream_lens_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/ctoken_abi.py` & `defi-services-lib-1.0.6/src/defi_services/abis/lending_pool/ctoken_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/lending_pool_abi.py` & `defi-services-lib-1.0.6/src/defi_services/abis/lending_pool/lending_pool_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/oracle_abi.py` & `defi-services-lib-1.0.6/src/defi_services/abis/lending_pool/oracle_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/staked_incentives_abi.py` & `defi-services-lib-1.0.6/src/defi_services/abis/lending_pool/staked_incentives_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/trava_lending_pool_abi.py` & `defi-services-lib-1.0.6/src/defi_services/abis/lending_pool/trava_lending_pool_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/trava_oracle_abi.py` & `defi-services-lib-1.0.6/src/defi_services/abis/lending_pool/trava_oracle_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/valas_multi_fee_distribution.py` & `defi-services-lib-1.0.6/src/defi_services/abis/lending_pool/valas_multi_fee_distribution.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/venus_comptroller_abi.py` & `defi-services-lib-1.0.6/src/defi_services/abis/lending_pool/venus_comptroller_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/venus_lens_abi.py` & `defi-services-lib-1.0.6/src/defi_services/abis/lending_pool/venus_lens_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/venus_lens_abi_v1.py` & `defi-services-lib-1.0.6/src/defi_services/abis/lending_pool/venus_lens_abi_v1.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/abis/vault/incentive_abi.py` & `defi-services-lib-1.0.6/src/defi_services/abis/vault/incentive_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/abis/vault/trava_vault_abi.py` & `defi-services-lib-1.0.6/src/defi_services/abis/vault/trava_vault_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/abis/vault/valuator_abi.py` & `defi-services-lib-1.0.6/src/defi_services/abis/vault/valuator_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/abis/vault/ve_abi.py` & `defi-services-lib-1.0.6/src/defi_services/abis/vault/ve_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/constants/contract_address.py` & `defi-services-lib-1.0.6/src/defi_services/constants/contract_address.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/constants/db_constant.py` & `defi-services-lib-1.0.6/src/defi_services/constants/db_constant.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     reward_deposit_apy = "rewardDepositAPY"
     reward_borrow_apy = "rewardBorrowAPY"
     type = "type"
     vaultType = "vaultType"
     created_at = "createdAt"
     deposit_apy = "depositAPY"
     borrow_apy = "borrowAPY"
+    stable_borrow_apy = "stableBorrowAPY"
     t_token = "tToken"
     d_token = "dToken"
     ltv = "ltv"
     reserves_list = "reservesList"
     is_new = "isNew"
     dapp_name = "dappName"
     project_name = "projectName"
```

### Comparing `defi-services-lib-1.0.5/src/defi_services/constants/mapping_constant.py` & `defi-services-lib-1.0.6/src/defi_services/constants/mapping_constant.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/defi_service.py` & `defi-services-lib-1.0.6/src/defi_services/defi_service.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/lending_pools/aave_v2_service.py` & `defi-services-lib-1.0.6/src/defi_services/lending_pools/geist_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,48 @@
 from defi_services.constants.chain_constant import Chain
 from defi_services.defi_service import DefiService
-from defi_services.lending_pools.lending_pools_info.ethereum.aave_v2_eth import AAVE_V2_ETH
-from defi_services.lending_pools.lending_pools_info.polygon.aave_v2_polygon import AAVE_V2_POLYGON
-from defi_services.lending_pools.services.aave_v2_state_service import AaveV2StateService
+from defi_services.lending_pools.lending_pools_info.fantom.geist_ftm import GEIST_ETH
+from defi_services.lending_pools.services.geist_state_service import GeistStateService
 
 
-class AaveV2Service(DefiService):
-    name = "aave v2 lending pool"
+class GeistService(DefiService):
+    name = "geist lending pool"
 
     def __init__(self, chain_id: str, provider_uri: str):
         super().__init__(chain_id, provider_uri)
-        self.state_service = AaveV2StateService(provider_uri)
+        self.state_service = GeistStateService(provider_uri)
         self.defi_constant = self._get_constant()
         self.address = self.defi_constant.get("address")
 
     def _get_constant(self):
-        if self.chain_id == Chain.polygon:
-            return AAVE_V2_POLYGON
-        elif self.chain_id == Chain.ethereum:
-            return AAVE_V2_ETH
-
+        if self.chain_id == Chain.fantom:
+            return GEIST_ETH
         return None
 
-    def get_apy_defi_app(self, block_number: int = "latest", **kwargs):
+    def get_apy_defi_app(self, block_number: int = "latest"):
         return self.state_service.get_apy_lending_pool(
             pool_address=self.defi_constant.get("address"),
-            staked_incentive_address=self.defi_constant.get("stakedIncentiveAddress"),
+            chef_incentive_address=self.defi_constant.get("chefIncentiveAddress"),
             oracle_address=self.defi_constant.get("oracleAddress"),
-            block_number=block_number,
-            reserves_info=self.defi_constant.get("reservesList"),
-            wrapped_native_token_price=kwargs.get("wrapped_native_token_price"),
+            block_number=block_number
         )
 
     def get_rewards_balance(self, wallet_address: str, block_number: int = "latest"):
-        return self.state_service.get_rewards_balance(
+        reward = self.state_service.get_rewards_balance(
             wallet_address=wallet_address,
             pool_address=self.defi_constant.get("address"),
-            staked_incentive_address=self.defi_constant.get("stakedIncentiveAddress"),
+            multi_fee_address=self.defi_constant.get("multiFeeAddress"),
             block_number=block_number,
             reserves_info=self.defi_constant.get("reservesList")
         )
+        return {
+            self.defi_constant.get("rewardToken"): reward
+        }
 
-    def get_wallet_deposit_borrow_balance(self, wallet_address: str, block_number: int = "latest", **kwargs):
+    def get_wallet_deposit_borrow_balance(self, wallet_address: str, block_number: int = "latest"):
         return self.state_service.get_wallet_deposit_borrow_balance(
             wallet_address=wallet_address,
             pool_address=self.defi_constant.get("address"),
             oracle_address=self.defi_constant.get("oracleAddress"),
             block_number=block_number,
-            reserves_info=self.defi_constant.get("reservesList"),
-            wrapped_native_token_price=kwargs.get("wrapped_native_token_price"),
+            reserves_info=self.defi_constant.get("reservesList")
         )
```

### Comparing `defi-services-lib-1.0.5/src/defi_services/lending_pools/compound_service.py` & `defi-services-lib-1.0.6/src/defi_services/lending_pools/cream_service.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,59 @@
 from defi_services.constants.chain_constant import Chain
+from defi_services.constants.contract_address import ContractAddresses
 from defi_services.defi_service import DefiService
-from defi_services.lending_pools.lending_pools_info.ethereum.compound_eth import COMPOUND_ETH
-from defi_services.lending_pools.services.compound_state_service import CompoundStateService
+from defi_services.lending_pools.lending_pools_info.bsc.cream_bsc import CREAM_BSC
+from defi_services.lending_pools.services.cream_state_service import CreamStateService
 
 
-class CompoundService(DefiService):
-    name = "compound lending pool"
+class CreamService(DefiService):
+    name = "cream lending pool"
 
     def __init__(self, chain_id: str, provider_uri: str):
         super().__init__(chain_id, provider_uri)
-        self.state_service = CompoundStateService(provider_uri)
+        self.state_service = CreamStateService(provider_uri)
         self.defi_constant = self._get_constant()
         self.address = self.defi_constant.get("comptrollerAddress")
 
     def _get_constant(self):
-        if self.chain_id == Chain.ethereum:
-            return COMPOUND_ETH
+        if self.chain_id == Chain.bsc:
+            return CREAM_BSC
         return None
 
     def get_pool_token(self):
         return self.defi_constant.get("rewardToken")
 
+    def get_wrapped_native_token(self):
+        if self.chain_id == Chain.bsc:
+            return ContractAddresses.WBNB
+        return None
+
     def get_apy_defi_app(self, block_number: int = "latest", **kwargs):
         return self.state_service.get_apy_lending_pool(
             comptroller_address=self.defi_constant.get("comptrollerAddress"),
             lens_address=self.defi_constant.get("lensAddress"),
             pool_token_price=float(kwargs.get("pool_token_price")),
-            wrapped_native_token_price=1,
+            wrapped_native_token_price=float(kwargs.get("wrapped_native_token_price")),
             block_number=block_number
         )
 
     def get_rewards_balance(self, wallet_address: str, block_number: int = "latest"):
-        return self.state_service.get_rewards_balance(
+        reward = self.state_service.get_rewards_balance(
             wallet_address=wallet_address,
-            comptroller_address=self.defi_constant.get("comptrollerAddress"),
+            comptroller_implementation_address=self.defi_constant.get("comptrollerImplementationAddress"),
             lens_address=self.defi_constant.get("lensAddress"),
             pool_token=self.defi_constant.get("rewardToken"),
             block_number=block_number
         )
+        return {
+            self.defi_constant.get("rewardToken"): reward
+        }
 
     def get_wallet_deposit_borrow_balance(self, wallet_address: str, block_number: int = "latest", **kwargs):
         return self.state_service.get_wallet_deposit_borrow_balance(
             wallet_address=wallet_address,
             lens_address=self.defi_constant.get("lensAddress"),
             reserves_info=self.defi_constant.get("reservesList"),
-            wrapped_native_token_price=1,
+            wrapped_native_token_price=float(kwargs.get("wrapped_native_token_price")),
             block_number=block_number,
             wrapped_native_token=self.get_wrapped_native_token()
         )
```

### Comparing `defi-services-lib-1.0.5/src/defi_services/lending_pools/cream_service.py` & `defi-services-lib-1.0.6/src/defi_services/lending_pools/venus_service.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,56 +1,51 @@
 from defi_services.constants.chain_constant import Chain
-from defi_services.constants.contract_address import ContractAddresses
 from defi_services.defi_service import DefiService
-from defi_services.lending_pools.lending_pools_info.bsc.cream_bsc import CREAM_BSC
-from defi_services.lending_pools.services.cream_state_service import CreamStateService
+from defi_services.lending_pools.lending_pools_info.bsc.venus_bsc import VENUS_BSC
+from defi_services.lending_pools.services.venus_state_service import VenusStateService
 
 
-class CreamService(DefiService):
-    name = "cream lending pool"
+class VenusService(DefiService):
+    name = "venus lending pool"
 
     def __init__(self, chain_id: str, provider_uri: str):
         super().__init__(chain_id, provider_uri)
-        self.state_service = CreamStateService(provider_uri)
+        self.state_service = VenusStateService(provider_uri)
         self.defi_constant = self._get_constant()
         self.address = self.defi_constant.get("comptrollerAddress")
 
     def _get_constant(self):
         if self.chain_id == Chain.bsc:
-            return CREAM_BSC
+            return VENUS_BSC
         return None
 
     def get_pool_token(self):
         return self.defi_constant.get("rewardToken")
 
-    def get_wrapped_native_token(self):
-        if self.chain_id == Chain.bsc:
-            return ContractAddresses.WBNB
-        return None
-
     def get_apy_defi_app(self, block_number: int = "latest", **kwargs):
         return self.state_service.get_apy_lending_pool(
             comptroller_address=self.defi_constant.get("comptrollerAddress"),
             lens_address=self.defi_constant.get("lensAddress"),
             pool_token_price=float(kwargs.get("pool_token_price")),
-            wrapped_native_token_price=float(kwargs.get("wrapped_native_token_price")),
             block_number=block_number
         )
 
     def get_rewards_balance(self, wallet_address: str, block_number: int = "latest"):
-        return self.state_service.get_rewards_balance(
+        reward = self.state_service.get_rewards_balance(
             wallet_address=wallet_address,
-            comptroller_implementation_address=self.defi_constant.get("comptrollerImplementationAddress"),
+            comptroller_address=self.defi_constant.get("comptrollerAddress"),
             lens_address=self.defi_constant.get("lensAddress"),
             pool_token=self.defi_constant.get("rewardToken"),
             block_number=block_number
         )
+        return {
+            self.defi_constant.get("rewardToken"): reward
+        }
 
-    def get_wallet_deposit_borrow_balance(self, wallet_address: str, block_number: int = "latest", **kwargs):
+    def get_wallet_deposit_borrow_balance(self, wallet_address: str, block_number: int = "latest"):
         return self.state_service.get_wallet_deposit_borrow_balance(
             wallet_address=wallet_address,
             lens_address=self.defi_constant.get("lensAddress"),
             reserves_info=self.defi_constant.get("reservesList"),
-            wrapped_native_token_price=float(kwargs.get("wrapped_native_token_price")),
             block_number=block_number,
             wrapped_native_token=self.get_wrapped_native_token()
         )
```

### Comparing `defi-services-lib-1.0.5/src/defi_services/lending_pools/geist_service.py` & `defi-services-lib-1.0.6/src/defi_services/lending_pools/valas_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 from defi_services.constants.chain_constant import Chain
 from defi_services.defi_service import DefiService
-from defi_services.lending_pools.lending_pools_info.fantom.geist_ftm import GEIST_ETH
-from defi_services.lending_pools.services.geist_state_service import GeistStateService
+from defi_services.lending_pools.lending_pools_info.bsc.valas_bsc import VALAS_BSC
+from defi_services.lending_pools.services.valas_state_service import ValasStateService
 
 
-class GeistService(DefiService):
-    name = "geist lending pool"
+class ValasService(DefiService):
+    name = "valas lending pool"
 
     def __init__(self, chain_id: str, provider_uri: str):
         super().__init__(chain_id, provider_uri)
-        self.state_service = GeistStateService(provider_uri)
+        self.state_service = ValasStateService(provider_uri)
         self.defi_constant = self._get_constant()
         self.address = self.defi_constant.get("address")
 
     def _get_constant(self):
-        if self.chain_id == Chain.fantom:
-            return GEIST_ETH
+        if self.chain_id == Chain.bsc:
+            return VALAS_BSC
         return None
 
     def get_apy_defi_app(self, block_number: int = "latest"):
         return self.state_service.get_apy_lending_pool(
             pool_address=self.defi_constant.get("address"),
             chef_incentive_address=self.defi_constant.get("chefIncentiveAddress"),
             oracle_address=self.defi_constant.get("oracleAddress"),
             block_number=block_number
         )
 
     def get_rewards_balance(self, wallet_address: str, block_number: int = "latest"):
-        return self.state_service.get_rewards_balance(
+        reward = self.state_service.get_rewards_balance(
             wallet_address=wallet_address,
             pool_address=self.defi_constant.get("address"),
             multi_fee_address=self.defi_constant.get("multiFeeAddress"),
             block_number=block_number,
             reserves_info=self.defi_constant.get("reservesList")
         )
+        return {
+            self.defi_constant.get("rewardToken"): reward
+        }
 
     def get_wallet_deposit_borrow_balance(self, wallet_address: str, block_number: int = "latest"):
         return self.state_service.get_wallet_deposit_borrow_balance(
             wallet_address=wallet_address,
             pool_address=self.defi_constant.get("address"),
             oracle_address=self.defi_constant.get("oracleAddress"),
             block_number=block_number,
```

### Comparing `defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/arbitrum/radiant_arbitrum.py` & `defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/arbitrum/radiant_arbitrum.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 RADIANT_ARB = {
-    "address": "0xF4B1486DD74D07706052A33d31d7c0AAFD0659E1",
+    "address": "0xf4b1486dd74d07706052a33d31d7c0aafd0659e1",
     "name": "Radiant Lending Pool",
-    "rewardToken": "0x3082CC23568eA640225c2467653dB90e9250AaA0",
-    "multiFeeAddress": "0x76ba3eC5f5adBf1C58c91e86502232317EeA72dE",
-    "chefIncentiveAddress": '0xebC85d44cefb1293707b11f707bd3CEc34B4D5fA',
-    "oracleAddress": "0xC0cE5De939aaD880b0bdDcf9aB5750a53EDa454b",
+    "rewardToken": "0x3082cc23568ea640225c2467653db90e9250aaa0",
+    "multiFeeAddress": "0x76ba3ec5f5adbf1c58c91e86502232317eea72de",
+    "chefIncentiveAddress": '0xebc85d44cefb1293707b11f707bd3cec34b4d5fa',
+    "oracleAddress": "0xc0ce5de939aad880b0bddcf9ab5750a53eda454b",
     "type": "LENDING_POOL",
     "reservesList": {
         "0x2f2a2543b76a4166549f7aab2e75bef0aefc5b0f": {
             "tToken": "0x727354712bdfcd8596a3852fd2065b3c34f4f770",
             "dToken": "0x3eeafa33625df20837ed0cb83ae4d1e34788b141",
             "sdToken": "0x9ee73b7dd519f89168592ef97b29c97d844befb0",
             "liquidationThreshold": 0.75
```

### Comparing `defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/bsc/cream_bsc.py` & `defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/bsc/cream_bsc.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/bsc/radiant_bsc.py` & `defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/bsc/radiant_bsc.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/bsc/trava_bsc.py` & `defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/bsc/trava_bsc.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/bsc/valas_bsc.py` & `defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/bsc/valas_bsc.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/bsc/venus_bsc.py` & `defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/bsc/venus_bsc.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/ethereum/aave_v2_eth.py` & `defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/ethereum/aave_v2_eth.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 AAVE_V2_ETH = {
     "address": "0x7d2768de32b0b80b7a3454c06bdac94a69ddc7a9",
     "name": "Aave V2 Lending Pool",
-    "rewardToken": "0x7fc66500c84a76ad7e9c93437bfc5ac33e2ddae9",
+    "rewardToken": "0x4da27a545c0c5b758a6ba100e3a049001de870f5",
     "stakedIncentiveAddress": '0x83d055d382f25e6793099713505c68a5c7535a35',
     "oracleAddress": "0xa50ba011c48153de246e5192c8f9258a2ba79ca9",
     "type": "LENDING_POOL",
     "reservesList": {
         "0xdac17f958d2ee523a2206206994597c13d831ec7": {
             "tToken": "0x3ed3b47dd13ec9a98b44e6204a523e766b225811",
             "dToken": "0x531842cebbdd378f8ee36d171d6cc9c4fcf475ec",
```

### Comparing `defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/ethereum/compound_eth.py` & `defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/ethereum/compound_eth.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/ethereum/trava_eth.py` & `defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/ethereum/trava_eth.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/fantom/geist_ftm.py` & `defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/fantom/geist_ftm.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/fantom/trava_ftm.py` & `defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/fantom/trava_ftm.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/polygon/aave_v2_polygon.py` & `defi-services-lib-1.0.6/src/defi_services/lending_pools/lending_pools_info/polygon/aave_v2_polygon.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 AAVE_V2_POLYGON = {
     "address": "0x8dff5e27ea6b7ac08ebfdf9eb090f32ee9a30fcf",
     "name": "Aave V2 Lending Pool",
-    "rewardToken": "0xd6df932a45c0f255f85145f286ea0b292b21c90b",
+    "rewardToken": "0x0d500b1d8e8ef31e21c99d1db9a6444d3adf1270",
     "stakedIncentiveAddress": '0x2c901a65071c077c78209b06ab2b5d8ec285ab84',
     "oracleAddress": "0x0229f777b0fab107f9591a41d5f02e4e98db6f2d",
     "type": "LENDING_POOL",
     "reservesList": {
         "0x8f3cf7ad23cd3cadbd9735aff958023239c6a063": {
             "tToken": "0x27f8d03b3a2196956ed754badc28d73be8830a6e",
             "dToken": "0x75c4d1fb84429023170086f06e682dcbbf537b7d",
```

### Comparing `defi-services-lib-1.0.5/src/defi_services/lending_pools/radiant_service.py` & `defi-services-lib-1.0.6/src/defi_services/lending_pools/radiant_service.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,21 +24,24 @@
             chef_incentive_address=self.defi_constant.get("chefIncentiveAddress"),
             oracle_address=self.defi_constant.get("oracleAddress"),
             block_number=block_number,
             pool_decimals=8
         )
 
     def get_rewards_balance(self, wallet_address: str, block_number: int = "latest"):
-        return self.state_service.get_rewards_balance(
+        reward = self.state_service.get_rewards_balance(
             wallet_address=wallet_address,
             pool_address=self.defi_constant.get("address"),
             multi_fee_address=self.defi_constant.get("multiFeeAddress"),
             block_number=block_number,
             reserves_info=self.defi_constant.get("reservesList")
         )
+        return {
+            self.defi_constant.get("rewardToken"): reward
+        }
 
     def get_wallet_deposit_borrow_balance(self, wallet_address: str, block_number: int = "latest"):
         return self.state_service.get_wallet_deposit_borrow_balance(
             wallet_address=wallet_address,
             pool_address=self.defi_constant.get("address"),
             oracle_address=self.defi_constant.get("oracleAddress"),
             block_number=block_number,
```

### Comparing `defi-services-lib-1.0.5/src/defi_services/lending_pools/services/aave_v2_state_service.py` & `defi-services-lib-1.0.6/src/defi_services/lending_pools/services/aave_v2_state_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,33 @@
 from defi_services.abis.lending_pool.lending_pool_abi import LENDING_POOL_ABI
 
 
 class AaveV2StateService(TravaStateService):
     def __init__(self, provider_uri: str):
         super().__init__(provider_uri)
 
+    def get_asset_data_of_token_list(self, stake_incentive_address: str, token_addresses: list,
+                                     stake_incentive_abi: list = STAKED_INCENTIVES_ABI, block_number: int = 'latest'):
+        list_rpc_call, list_call_id = [], []
+        for token_address in token_addresses:
+            add_rpc_call(
+                abi=stake_incentive_abi, fn_name='assets', contract_address=stake_incentive_address,
+                block_number=block_number, fn_paras=token_address, list_rpc_call=list_rpc_call,
+                list_call_id=list_call_id
+
+            )
+        data_response = self.client_querier.sent_batch_to_provider(list_rpc_call, batch_size=100)
+        decoded_data = decode_data_response(data_response, list_call_id)
+        result = {}
+        for token_address in token_addresses:
+            get_reserve_data_call_id = f'assets_{stake_incentive_address}_{token_address}_{block_number}'.lower()
+            result[token_address.lower()] = decoded_data.get(get_reserve_data_call_id)
+
+        return result
+
     def _decode_apy_lending_pool_function_call(
             self,
             list_rpc_call: list,
             list_call_id: list,
             pool_address: str,
             reserves_list: list,
             stake_incentive_address: str = None,
@@ -30,16 +49,18 @@
             reserves_data[token.lower()] = decoded_data.get(get_reserve_data_call_id)
 
         interest_rate, ttokens, debt_tokens, decimals = {}, {}, {}, {}
         sdebt_tokens, decimals = {}, {}
         for token_address in reserves_list:
             lower_address = token_address.lower()
             reserve_data = reserves_data[lower_address]
-            interest_rate[lower_address] = {DBConst.deposit_apy: float(reserve_data[3]) / 10 ** 27,
-                                            DBConst.borrow_apy: float(reserve_data[4]) / 10 ** 27}
+            interest_rate[lower_address] = {
+                DBConst.deposit_apy: float(reserve_data[3]) / 10 ** 27,
+                DBConst.borrow_apy: float(reserve_data[4]) / 10 ** 27,
+                DBConst.stable_borrow_apy: float(reserve_data[5]) / 10 ** 27}
             ttoken = reserve_data[7].lower()
             sdebt_token = reserve_data[8].lower()
             debt_token = reserve_data[9].lower()
             ttokens[lower_address] = ttoken
             debt_tokens[lower_address] = debt_token
             sdebt_tokens[lower_address] = sdebt_token
             decimals_call_id = f'decimals_{token_address}_{block_number}'.lower()
@@ -131,41 +152,45 @@
             debt_token = debt_tokens.get(token_address)
             decimal = decimals.get(token_address)
             total_supply_t = total_supply_tokens.get(ttoken)
             total_supply_d = total_supply_tokens.get(debt_token)
             asset_data_t = asset_data_tokens.get(ttoken)
             asset_data_d = asset_data_tokens.get(debt_token)
             # update deposit, borrow apy
-            total_supply_t = total_supply_t * wrapped_native_token_price / 10 ** decimal
-            total_supply_d = total_supply_d * wrapped_native_token_price / 10 ** decimal
-            eps_t = asset_data_t[1] / 10 ** 18
-            eps_d = asset_data_d[1] / 10 ** 18
+            total_supply_t = total_supply_t / 10 ** decimal
+            total_supply_d = total_supply_d / 10 ** decimal
+            eps_t = asset_data_t[0] / 10 ** 18
+            eps_d = asset_data_d[0] / 10 ** 18
             token_price = token_prices.get(token_address)
             if total_supply_t:
+                total_supply_t_in_usd = total_supply_t * token_price * wrapped_native_token_price
                 deposit_apr = eps_t * TimeConstants.A_YEAR * pool_token_price / (
-                    total_supply_t * token_price)
+                    total_supply_t_in_usd)
             else:
+                total_supply_t_in_usd = 0
                 deposit_apr = 0
             if total_supply_d:
+                total_supply_d_in_usd = total_supply_d * token_price * wrapped_native_token_price
                 borrow_apr = eps_d * TimeConstants.A_YEAR * pool_token_price / (
-                    total_supply_d * token_price)
+                        total_supply_d_in_usd)
             else:
+                total_supply_d_in_usd = 0
                 borrow_apr = 0
             interest_rate[token_address].update({
                 "utilization": total_supply_d / total_supply_t,
                 DBConst.reward_deposit_apy: deposit_apr,
                 DBConst.reward_borrow_apy: borrow_apr})
             # update liquidity
             liquidity_log = {
                 DBConst.total_borrow: {
                     DBConst.amount: total_supply_d,
-                    DBConst.value_in_usd: total_supply_d * token_price},
+                    DBConst.value_in_usd: total_supply_d_in_usd},
                 DBConst.total_deposit: {
                     DBConst.amount: total_supply_t,
-                    DBConst.value_in_usd: total_supply_t * token_price}
+                    DBConst.value_in_usd: total_supply_t_in_usd}
             }
             interest_rate[token_address].update({DBConst.liquidity_change_logs: liquidity_log})
 
         return interest_rate
 
     def get_wallet_deposit_borrow_balance(
             self,
```

### Comparing `defi-services-lib-1.0.5/src/defi_services/lending_pools/services/compound_state_service.py` & `defi-services-lib-1.0.6/src/defi_services/lending_pools/services/compound_state_service.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/lending_pools/services/cream_state_service.py` & `defi-services-lib-1.0.6/src/defi_services/lending_pools/services/cream_state_service.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/lending_pools/services/geist_state_service.py` & `defi-services-lib-1.0.6/src/defi_services/lending_pools/services/geist_state_service.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/lending_pools/services/radiant_state_service.py` & `defi-services-lib-1.0.6/src/defi_services/lending_pools/services/radiant_state_service.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/lending_pools/services/trava_state_service.py` & `defi-services-lib-1.0.6/src/defi_services/lending_pools/services/trava_state_service.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/lending_pools/services/valas_state_service.py` & `defi-services-lib-1.0.6/src/defi_services/lending_pools/services/valas_state_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,16 +108,18 @@
             get_reserve_data_call_id = f'getReserveData_{pool_address}_{token}_{block_number}'.lower()
             reserves_data[token.lower()] = decoded_data.get(get_reserve_data_call_id)
 
         interest_rate, ttokens, debt_tokens, decimals = {}, {}, {}, {}
         for token_address in reserves_list:
             lower_address = token_address.lower()
             reserve_data = reserves_data[lower_address]
-            interest_rate[lower_address] = {DBConst.deposit_apy: float(reserve_data[3]) / 10 ** 27,
-                                            DBConst.borrow_apy: float(reserve_data[4]) / 10 ** 27}
+            interest_rate[lower_address] = {
+                DBConst.deposit_apy: float(reserve_data[3]) / 10 ** 27,
+                DBConst.borrow_apy: float(reserve_data[4]) / 10 ** 27,
+                DBConst.stable_borrow_apy: float(reserve_data[5]) / 10 ** 27}
             ttoken = reserve_data[7].lower()
             debt_token = reserve_data[9].lower()
             ttokens[lower_address] = ttoken
             debt_tokens[lower_address] = debt_token
             decimals_call_id = f'decimals_{token_address}_{block_number}'.lower()
             decimals[lower_address] = decoded_data.get(decimals_call_id)
         rewards_per_second_id = f"rewardsPerSecond_{chef_incentive_address}_{block_number}".lower()
@@ -166,15 +168,15 @@
         debt_tokens = decoded_data["debt_tokens"]
         decimals = decoded_data["decimals"]
         rewards_per_second = decoded_data["rewards_per_second"]
         total_alloc_point = decoded_data["total_alloc_point"]
         debt_and_t_tokens = list(debt_tokens.values()) + list(ttokens.values())
         total_supply_tokens = self.total_supply_of_token_list(debt_and_t_tokens)
         asset_data_tokens = self.pool_info_of_token_list(
-                chef_incentive_address, debt_and_t_tokens, chef_incentive_abi, block_number)
+            chef_incentive_address, debt_and_t_tokens, chef_incentive_abi, block_number)
         # Decode data
         lower_addresses = [i.lower() for i in reserves_list]
         for token_address in lower_addresses:
             ttoken = ttokens.get(token_address)
             debt_token = debt_tokens.get(token_address)
             decimal = decimals.get(token_address)
             total_supply_t = total_supply_tokens.get(ttoken)
```

### Comparing `defi-services-lib-1.0.5/src/defi_services/lending_pools/services/venus_state_service.py` & `defi-services-lib-1.0.6/src/defi_services/lending_pools/services/venus_state_service.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/lending_pools/trava_service.py` & `defi-services-lib-1.0.6/src/defi_services/lending_pools/trava_service.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,21 +31,24 @@
             staked_incentive_address=self.defi_constant.get("stakedIncentiveAddress"),
             oracle_address=self.defi_constant.get("oracleAddress"),
             block_number=block_number,
             reserves_info=self.defi_constant.get("reservesList")
         )
 
     def get_rewards_balance(self, wallet_address: str, block_number: int = "latest"):
-        return self.state_service.get_rewards_balance(
+        reward = self.state_service.get_rewards_balance(
             wallet_address=wallet_address,
             pool_address=self.defi_constant.get("address"),
             staked_incentive_address=self.defi_constant.get("stakedIncentiveAddress"),
             block_number=block_number,
             reserves_info=self.defi_constant.get("reservesList")
         )
+        return {
+            self.defi_constant.get("rewardToken"): reward
+        }
 
     def get_wallet_deposit_borrow_balance(self, wallet_address: str, block_number: int = "latest"):
         return self.state_service.get_wallet_deposit_borrow_balance(
             wallet_address=wallet_address,
             pool_address=self.defi_constant.get("address"),
             oracle_address=self.defi_constant.get("oracleAddress"),
             block_number=block_number,
```

### Comparing `defi-services-lib-1.0.5/src/defi_services/lending_pools/valas_service.py` & `defi-services-lib-1.0.6/src/defi_services/lending_pools/aave_v2_service.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,55 @@
 from defi_services.constants.chain_constant import Chain
 from defi_services.defi_service import DefiService
-from defi_services.lending_pools.lending_pools_info.bsc.valas_bsc import VALAS_BSC
-from defi_services.lending_pools.services.valas_state_service import ValasStateService
+from defi_services.lending_pools.lending_pools_info.ethereum.aave_v2_eth import AAVE_V2_ETH
+from defi_services.lending_pools.lending_pools_info.polygon.aave_v2_polygon import AAVE_V2_POLYGON
+from defi_services.lending_pools.services.aave_v2_state_service import AaveV2StateService
 
 
-class ValasService(DefiService):
-    name = "valas lending pool"
+class AaveV2Service(DefiService):
+    name = "aave v2 lending pool"
 
     def __init__(self, chain_id: str, provider_uri: str):
         super().__init__(chain_id, provider_uri)
-        self.state_service = ValasStateService(provider_uri)
+        self.state_service = AaveV2StateService(provider_uri)
         self.defi_constant = self._get_constant()
         self.address = self.defi_constant.get("address")
 
     def _get_constant(self):
-        if self.chain_id == Chain.bsc:
-            return VALAS_BSC
+        if self.chain_id == Chain.polygon:
+            return AAVE_V2_POLYGON
+        elif self.chain_id == Chain.ethereum:
+            return AAVE_V2_ETH
+
         return None
 
-    def get_apy_defi_app(self, block_number: int = "latest"):
+    def get_apy_defi_app(self, block_number: int = "latest", **kwargs):
         return self.state_service.get_apy_lending_pool(
             pool_address=self.defi_constant.get("address"),
-            chef_incentive_address=self.defi_constant.get("chefIncentiveAddress"),
+            staked_incentive_address=self.defi_constant.get("stakedIncentiveAddress"),
             oracle_address=self.defi_constant.get("oracleAddress"),
-            block_number=block_number
+            block_number=block_number,
+            reserves_info=self.defi_constant.get("reservesList"),
+            wrapped_native_token_price=kwargs.get("ethereum_price"),
         )
 
     def get_rewards_balance(self, wallet_address: str, block_number: int = "latest"):
-        return self.state_service.get_rewards_balance(
+        reward = self.state_service.get_rewards_balance(
             wallet_address=wallet_address,
             pool_address=self.defi_constant.get("address"),
-            multi_fee_address=self.defi_constant.get("multiFeeAddress"),
+            staked_incentive_address=self.defi_constant.get("stakedIncentiveAddress"),
             block_number=block_number,
             reserves_info=self.defi_constant.get("reservesList")
         )
+        return {
+            self.defi_constant.get("rewardToken"): reward
+        }
 
-    def get_wallet_deposit_borrow_balance(self, wallet_address: str, block_number: int = "latest"):
+    def get_wallet_deposit_borrow_balance(self, wallet_address: str, block_number: int = "latest", **kwargs):
         return self.state_service.get_wallet_deposit_borrow_balance(
             wallet_address=wallet_address,
             pool_address=self.defi_constant.get("address"),
             oracle_address=self.defi_constant.get("oracleAddress"),
             block_number=block_number,
-            reserves_info=self.defi_constant.get("reservesList")
+            reserves_info=self.defi_constant.get("reservesList"),
+            wrapped_native_token_price=kwargs.get("ethereum_price"),
         )
```

### Comparing `defi-services-lib-1.0.5/src/defi_services/lending_pools/venus_service.py` & `defi-services-lib-1.0.6/src/defi_services/lending_pools/compound_service.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 from defi_services.constants.chain_constant import Chain
 from defi_services.defi_service import DefiService
-from defi_services.lending_pools.lending_pools_info.bsc.venus_bsc import VENUS_BSC
-from defi_services.lending_pools.services.venus_state_service import VenusStateService
+from defi_services.lending_pools.lending_pools_info.ethereum.compound_eth import COMPOUND_ETH
+from defi_services.lending_pools.services.compound_state_service import CompoundStateService
 
 
-class VenusService(DefiService):
-    name = "venus lending pool"
+class CompoundService(DefiService):
+    name = "compound lending pool"
 
     def __init__(self, chain_id: str, provider_uri: str):
         super().__init__(chain_id, provider_uri)
-        self.state_service = VenusStateService(provider_uri)
+        self.state_service = CompoundStateService(provider_uri)
         self.defi_constant = self._get_constant()
         self.address = self.defi_constant.get("comptrollerAddress")
 
     def _get_constant(self):
-        if self.chain_id == Chain.bsc:
-            return VENUS_BSC
+        if self.chain_id == Chain.ethereum:
+            return COMPOUND_ETH
         return None
 
     def get_pool_token(self):
         return self.defi_constant.get("rewardToken")
 
     def get_apy_defi_app(self, block_number: int = "latest", **kwargs):
         return self.state_service.get_apy_lending_pool(
             comptroller_address=self.defi_constant.get("comptrollerAddress"),
             lens_address=self.defi_constant.get("lensAddress"),
             pool_token_price=float(kwargs.get("pool_token_price")),
+            wrapped_native_token_price=1,
             block_number=block_number
         )
 
     def get_rewards_balance(self, wallet_address: str, block_number: int = "latest"):
-        return self.state_service.get_rewards_balance(
-            wallet_address=wallet_address,
-            comptroller_address=self.defi_constant.get("comptrollerAddress"),
-            lens_address=self.defi_constant.get("lensAddress"),
-            pool_token=self.defi_constant.get("rewardToken"),
-            block_number=block_number
-        )
+        reward = self.state_service.get_rewards_balance(
+                wallet_address=wallet_address,
+                comptroller_address=self.defi_constant.get("comptrollerAddress"),
+                lens_address=self.defi_constant.get("lensAddress"),
+                pool_token=self.defi_constant.get("rewardToken"),
+                block_number=block_number
+            )
+        return {
+            self.defi_constant.get("rewardToken"): reward
+        }
 
-    def get_wallet_deposit_borrow_balance(self, wallet_address: str, block_number: int = "latest"):
+    def get_wallet_deposit_borrow_balance(self, wallet_address: str, block_number: int = "latest", **kwargs):
         return self.state_service.get_wallet_deposit_borrow_balance(
             wallet_address=wallet_address,
             lens_address=self.defi_constant.get("lensAddress"),
             reserves_info=self.defi_constant.get("reservesList"),
+            wrapped_native_token_price=1,
             block_number=block_number,
             wrapped_native_token=self.get_wrapped_native_token()
         )
```

### Comparing `defi-services-lib-1.0.5/src/defi_services/state_service.py` & `defi-services-lib-1.0.6/src/defi_services/state_service.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/utils/batch_queries_service.py` & `defi-services-lib-1.0.6/src/defi_services/utils/batch_queries_service.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/utils/graph_operations.py` & `defi-services-lib-1.0.6/src/defi_services/utils/graph_operations.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/utils/market_service.py` & `defi-services-lib-1.0.6/src/defi_services/utils/market_service.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services/utils/memory_storage.py` & `defi-services-lib-1.0.6/src/defi_services/utils/memory_storage.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.5/src/defi_services_lib.egg-info/PKG-INFO` & `defi-services-lib-1.0.6/src/defi_services_lib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: defi-services-lib
-Version: 1.0.5
+Version: 1.0.6
 Summary: Calculate apy, apr, and wallet information,... in decentralized applications.
 Home-page: https://github.com/phamvietbang/defi-services-lib
 Author: Viet-Bang Pham
 Author-email: phamvietbang2965@gmail.com
 Project-URL: Bug Tracker, https://github.com/phamvietbang/defi-services-lib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `defi-services-lib-1.0.5/src/defi_services_lib.egg-info/SOURCES.txt` & `defi-services-lib-1.0.6/src/defi_services_lib.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 src/defi_services/state_service.py
 src/defi_services/abis/__init__.py
 src/defi_services/abis/erc20_abi.py
 src/defi_services/abis/dex/__init__.py
 src/defi_services/abis/dex/biswap_masterchef_abi.py
 src/defi_services/abis/dex/pancakeswap_masterchef_abi.py
 src/defi_services/abis/lending_pool/__init__.py
+src/defi_services/abis/lending_pool/aave_v3_incentives_abi.py
+src/defi_services/abis/lending_pool/aave_v3_lending_pool_abi.py
+src/defi_services/abis/lending_pool/aave_v3_oracle_abi.py
 src/defi_services/abis/lending_pool/alpaca_fair_launch_abi.py
 src/defi_services/abis/lending_pool/alpaca_vault_abi.py
 src/defi_services/abis/lending_pool/alpaca_vault_config_abi.py
 src/defi_services/abis/lending_pool/chain_link_abi.py
 src/defi_services/abis/lending_pool/chef_incentives_controller.py
 src/defi_services/abis/lending_pool/cream_comptroller_abi.py
 src/defi_services/abis/lending_pool/cream_lens_abi.py
@@ -37,42 +40,49 @@
 src/defi_services/constants/chain_constant.py
 src/defi_services/constants/contract_address.py
 src/defi_services/constants/db_constant.py
 src/defi_services/constants/mapping_constant.py
 src/defi_services/constants/time_constant.py
 src/defi_services/lending_pools/__init__.py
 src/defi_services/lending_pools/aave_v2_service.py
+src/defi_services/lending_pools/aave_v3_service.py
 src/defi_services/lending_pools/compound_service.py
 src/defi_services/lending_pools/cream_service.py
 src/defi_services/lending_pools/geist_service.py
 src/defi_services/lending_pools/radiant_service.py
 src/defi_services/lending_pools/trava_service.py
 src/defi_services/lending_pools/valas_service.py
 src/defi_services/lending_pools/venus_service.py
 src/defi_services/lending_pools/lending_pools_info/__init__.py
 src/defi_services/lending_pools/lending_pools_info/arbitrum/__init__.py
+src/defi_services/lending_pools/lending_pools_info/arbitrum/aave_v3_arbitrum.py
 src/defi_services/lending_pools/lending_pools_info/arbitrum/radiant_arbitrum.py
 src/defi_services/lending_pools/lending_pools_info/bsc/__init__.py
 src/defi_services/lending_pools/lending_pools_info/bsc/cream_bsc.py
 src/defi_services/lending_pools/lending_pools_info/bsc/radiant_bsc.py
 src/defi_services/lending_pools/lending_pools_info/bsc/trava_bsc.py
 src/defi_services/lending_pools/lending_pools_info/bsc/valas_bsc.py
 src/defi_services/lending_pools/lending_pools_info/bsc/venus_bsc.py
 src/defi_services/lending_pools/lending_pools_info/ethereum/__init__.py
 src/defi_services/lending_pools/lending_pools_info/ethereum/aave_v2_eth.py
+src/defi_services/lending_pools/lending_pools_info/ethereum/aave_v3_eth.py
 src/defi_services/lending_pools/lending_pools_info/ethereum/compound_eth.py
 src/defi_services/lending_pools/lending_pools_info/ethereum/trava_eth.py
 src/defi_services/lending_pools/lending_pools_info/fantom/__init__.py
+src/defi_services/lending_pools/lending_pools_info/fantom/aave_v3_ftm.py
 src/defi_services/lending_pools/lending_pools_info/fantom/geist_ftm.py
 src/defi_services/lending_pools/lending_pools_info/fantom/trava_ftm.py
 src/defi_services/lending_pools/lending_pools_info/optimism/__init__.py
+src/defi_services/lending_pools/lending_pools_info/optimism/aave_v3_optimism.py
 src/defi_services/lending_pools/lending_pools_info/polygon/__init__.py
 src/defi_services/lending_pools/lending_pools_info/polygon/aave_v2_polygon.py
+src/defi_services/lending_pools/lending_pools_info/polygon/aave_v3_polygon.py
 src/defi_services/lending_pools/services/__init__.py
 src/defi_services/lending_pools/services/aave_v2_state_service.py
+src/defi_services/lending_pools/services/aave_v3_state_service.py
 src/defi_services/lending_pools/services/compound_state_service.py
 src/defi_services/lending_pools/services/cream_state_service.py
 src/defi_services/lending_pools/services/geist_state_service.py
 src/defi_services/lending_pools/services/radiant_state_service.py
 src/defi_services/lending_pools/services/trava_state_service.py
 src/defi_services/lending_pools/services/valas_state_service.py
 src/defi_services/lending_pools/services/venus_state_service.py
```

