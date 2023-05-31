# Comparing `tmp/defi-services-lib-1.0.4.tar.gz` & `tmp/defi-services-lib-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "defi-services-lib-1.0.4.tar", last modified: Tue May 30 10:53:18 2023, max compression
+gzip compressed data, was "defi-services-lib-1.0.5.tar", last modified: Wed May 31 01:56:20 2023, max compression
```

## Comparing `defi-services-lib-1.0.4.tar` & `defi-services-lib-1.0.5.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-30 10:53:18.378684 defi-services-lib-1.0.4/
--rw-r--r--   0 vietbangpham   (501) staff       (20)     1129 2023-05-29 07:02:16.000000 defi-services-lib-1.0.4/LICENSE
--rw-r--r--   0 vietbangpham   (501) staff       (20)      840 2023-05-30 10:53:18.378090 defi-services-lib-1.0.4/PKG-INFO
--rw-r--r--   0 vietbangpham   (501) staff       (20)      259 2023-05-29 08:02:45.000000 defi-services-lib-1.0.4/README.md
--rw-r--r--   0 vietbangpham   (501) staff       (20)      107 2023-05-29 04:51:50.000000 defi-services-lib-1.0.4/pyproject.toml
--rw-r--r--   0 vietbangpham   (501) staff       (20)       38 2023-05-30 10:53:18.378948 defi-services-lib-1.0.4/setup.cfg
--rw-r--r--   0 vietbangpham   (501) staff       (20)     1201 2023-05-29 07:52:03.000000 defi-services-lib-1.0.4/setup.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-30 10:53:18.261790 defi-services-lib-1.0.4/src/
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-30 10:53:18.271426 defi-services-lib-1.0.4/src/defi_services/
--rw-r--r--   0 vietbangpham   (501) staff       (20)       22 2023-05-30 10:53:07.000000 defi-services-lib-1.0.4/src/defi_services/__init__.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-30 10:53:18.273982 defi-services-lib-1.0.4/src/defi_services/abis/
--rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:43:51.000000 defi-services-lib-1.0.4/src/defi_services/abis/__init__.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-30 10:53:18.277706 defi-services-lib-1.0.4/src/defi_services/abis/dex/
--rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:44:57.000000 defi-services-lib-1.0.4/src/defi_services/abis/dex/__init__.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    15950 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/dex/biswap_masterchef_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    18798 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/dex/pancakeswap_masterchef_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     5636 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/erc20_abi.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-30 10:53:18.304134 defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/
--rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:45:05.000000 defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/__init__.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    16070 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/alpaca_fair_launch_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    23376 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/alpaca_vault_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    10050 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/alpaca_vault_config_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     1418 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/chain_link_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    12726 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/chef_incentives_controller.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    43379 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/cream_comptroller_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    20100 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/cream_lens_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    23605 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/ctoken_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    29034 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/lending_pool_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     4399 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/oracle_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    13482 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/staked_incentives_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    21266 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/trava_lending_pool_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     4507 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/trava_oracle_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     9576 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/valas_multi_fee_distribution.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    43234 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/venus_comptroller_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    18613 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/venus_lens_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    14433 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/venus_lens_abi_v1.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-30 10:53:18.309218 defi-services-lib-1.0.4/src/defi_services/abis/vault/
--rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:45:15.000000 defi-services-lib-1.0.4/src/defi_services/abis/vault/__init__.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    12332 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/vault/incentive_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    31318 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/vault/trava_vault_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)      598 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/vault/valuator_abi.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    38341 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/abis/vault/ve_abi.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-30 10:53:18.318266 defi-services-lib-1.0.4/src/defi_services/constants/
--rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:45:24.000000 defi-services-lib-1.0.4/src/defi_services/constants/__init__.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)      136 2023-05-29 15:14:03.000000 defi-services-lib-1.0.4/src/defi_services/constants/chain_constant.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     1931 2023-05-30 10:36:00.000000 defi-services-lib-1.0.4/src/defi_services/constants/contract_address.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     2492 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/constants/db_constant.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)      792 2023-05-30 10:51:26.000000 defi-services-lib-1.0.4/src/defi_services/constants/mapping_constant.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)      181 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/constants/time_constant.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     1105 2023-05-30 09:09:58.000000 defi-services-lib-1.0.4/src/defi_services/defi_service.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-30 10:53:18.332294 defi-services-lib-1.0.4/src/defi_services/lending_pools/
--rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/__init__.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     2418 2023-05-30 10:51:26.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/aave_v2_service.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     2175 2023-05-30 10:51:26.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/compound_service.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     2475 2023-05-30 10:51:26.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/cream_service.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     1953 2023-05-30 10:51:26.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/geist_service.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-30 10:53:18.334113 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/
--rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/__init__.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-30 10:53:18.336147 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/arbitrum/
--rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/arbitrum/__init__.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     2635 2023-05-30 09:15:50.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/arbitrum/radiant_arbitrum.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-30 10:53:18.345177 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/bsc/
--rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/bsc/__init__.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     8425 2023-05-30 09:48:52.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/bsc/cream_bsc.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     2325 2023-05-30 07:45:58.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/bsc/radiant_bsc.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     3757 2023-05-30 07:34:54.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/bsc/trava_bsc.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     4095 2023-05-30 06:42:21.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/bsc/valas_bsc.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     4743 2023-05-30 09:46:20.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/bsc/venus_bsc.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-30 10:53:18.350996 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/ethereum/
--rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/ethereum/__init__.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    11944 2023-05-30 08:21:17.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/ethereum/aave_v2_eth.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     3674 2023-05-30 09:56:27.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/ethereum/compound_eth.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     1565 2023-05-30 07:34:54.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/ethereum/trava_eth.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-30 10:53:18.354169 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/fantom/
--rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/fantom/__init__.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     3257 2023-05-30 07:24:06.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/fantom/geist_ftm.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     1808 2023-05-30 07:34:54.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/fantom/trava_ftm.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-30 10:53:18.355494 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/optimism/
--rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/optimism/__init__.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-30 10:53:18.356970 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/polygon/
--rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/polygon/__init__.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     4448 2023-05-30 08:21:17.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/polygon/aave_v2_polygon.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     2021 2023-05-30 10:51:26.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/radiant_service.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-30 10:53:18.368425 defi-services-lib-1.0.4/src/defi_services/lending_pools/services/
--rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 14:38:12.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/services/__init__.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    13008 2023-05-30 08:59:53.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/services/aave_v2_state_service.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     4418 2023-05-30 10:39:37.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/services/compound_state_service.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    20627 2023-05-30 10:36:00.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/services/cream_state_service.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)      689 2023-05-30 07:24:06.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/services/geist_state_service.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     1060 2023-05-30 09:13:38.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/services/radiant_state_service.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    17188 2023-05-30 08:51:45.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/services/trava_state_service.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    15441 2023-05-30 08:59:53.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/services/valas_state_service.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)    14936 2023-05-30 10:36:00.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/services/venus_state_service.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     2353 2023-05-30 10:51:26.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/trava_service.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     1947 2023-05-30 10:06:57.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/valas_service.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     2047 2023-05-30 10:51:26.000000 defi-services-lib-1.0.4/src/defi_services/lending_pools/venus_service.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     4360 2023-05-30 10:51:26.000000 defi-services-lib-1.0.4/src/defi_services/state_service.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-30 10:53:18.372959 defi-services-lib-1.0.4/src/defi_services/utils/
--rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:45:50.000000 defi-services-lib-1.0.4/src/defi_services/utils/__init__.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     1830 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/utils/batch_queries_service.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)     6271 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/utils/graph_operations.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)      723 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/utils/market_service.py
--rw-r--r--   0 vietbangpham   (501) staff       (20)      851 2023-05-29 03:52:33.000000 defi-services-lib-1.0.4/src/defi_services/utils/memory_storage.py
-drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-30 10:53:18.377122 defi-services-lib-1.0.4/src/defi_services_lib.egg-info/
--rw-r--r--   0 vietbangpham   (501) staff       (20)      840 2023-05-30 10:53:18.000000 defi-services-lib-1.0.4/src/defi_services_lib.egg-info/PKG-INFO
--rw-r--r--   0 vietbangpham   (501) staff       (20)     4692 2023-05-30 10:53:18.000000 defi-services-lib-1.0.4/src/defi_services_lib.egg-info/SOURCES.txt
--rw-r--r--   0 vietbangpham   (501) staff       (20)        1 2023-05-30 10:53:18.000000 defi-services-lib-1.0.4/src/defi_services_lib.egg-info/dependency_links.txt
--rw-r--r--   0 vietbangpham   (501) staff       (20)       34 2023-05-30 10:53:18.000000 defi-services-lib-1.0.4/src/defi_services_lib.egg-info/requires.txt
--rw-r--r--   0 vietbangpham   (501) staff       (20)       14 2023-05-30 10:53:18.000000 defi-services-lib-1.0.4/src/defi_services_lib.egg-info/top_level.txt
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 01:56:20.107939 defi-services-lib-1.0.5/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     1129 2023-05-29 07:02:16.000000 defi-services-lib-1.0.5/LICENSE
+-rw-r--r--   0 vietbangpham   (501) staff       (20)      840 2023-05-31 01:56:20.107331 defi-services-lib-1.0.5/PKG-INFO
+-rw-r--r--   0 vietbangpham   (501) staff       (20)      259 2023-05-29 08:02:45.000000 defi-services-lib-1.0.5/README.md
+-rw-r--r--   0 vietbangpham   (501) staff       (20)      107 2023-05-29 04:51:50.000000 defi-services-lib-1.0.5/pyproject.toml
+-rw-r--r--   0 vietbangpham   (501) staff       (20)       38 2023-05-31 01:56:20.108199 defi-services-lib-1.0.5/setup.cfg
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     1201 2023-05-29 07:52:03.000000 defi-services-lib-1.0.5/setup.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 01:56:20.033667 defi-services-lib-1.0.5/src/
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 01:56:20.039715 defi-services-lib-1.0.5/src/defi_services/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)       22 2023-05-31 01:56:09.000000 defi-services-lib-1.0.5/src/defi_services/__init__.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 01:56:20.041974 defi-services-lib-1.0.5/src/defi_services/abis/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:43:51.000000 defi-services-lib-1.0.5/src/defi_services/abis/__init__.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 01:56:20.044508 defi-services-lib-1.0.5/src/defi_services/abis/dex/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:44:57.000000 defi-services-lib-1.0.5/src/defi_services/abis/dex/__init__.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    15950 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/dex/biswap_masterchef_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    18798 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/dex/pancakeswap_masterchef_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     5636 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/erc20_abi.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 01:56:20.060995 defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:45:05.000000 defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/__init__.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    16070 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/alpaca_fair_launch_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    23376 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/alpaca_vault_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    10050 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/alpaca_vault_config_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     1418 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/chain_link_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    12726 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/chef_incentives_controller.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    43379 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/cream_comptroller_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    20100 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/cream_lens_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    23605 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/ctoken_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    29034 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/lending_pool_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     4399 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/oracle_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    13482 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/staked_incentives_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    21266 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/trava_lending_pool_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     4507 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/trava_oracle_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     9576 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/valas_multi_fee_distribution.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    43234 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/venus_comptroller_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    18613 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/venus_lens_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    14433 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/venus_lens_abi_v1.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 01:56:20.065693 defi-services-lib-1.0.5/src/defi_services/abis/vault/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:45:15.000000 defi-services-lib-1.0.5/src/defi_services/abis/vault/__init__.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    12332 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/vault/incentive_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    31318 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/vault/trava_vault_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)      598 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/vault/valuator_abi.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    38341 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/abis/vault/ve_abi.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 01:56:20.069377 defi-services-lib-1.0.5/src/defi_services/constants/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:45:24.000000 defi-services-lib-1.0.5/src/defi_services/constants/__init__.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)      136 2023-05-29 15:14:03.000000 defi-services-lib-1.0.5/src/defi_services/constants/chain_constant.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     1931 2023-05-30 10:36:00.000000 defi-services-lib-1.0.5/src/defi_services/constants/contract_address.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     2492 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/constants/db_constant.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)      792 2023-05-30 10:51:26.000000 defi-services-lib-1.0.5/src/defi_services/constants/mapping_constant.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)      181 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/constants/time_constant.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     1105 2023-05-30 09:09:58.000000 defi-services-lib-1.0.5/src/defi_services/defi_service.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 01:56:20.074462 defi-services-lib-1.0.5/src/defi_services/lending_pools/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/__init__.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     2475 2023-05-31 01:51:18.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/aave_v2_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     2243 2023-05-31 01:51:18.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/compound_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     2543 2023-05-31 01:51:17.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/cream_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     2010 2023-05-31 01:51:18.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/geist_service.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 01:56:20.074964 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/__init__.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 01:56:20.075676 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/arbitrum/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/arbitrum/__init__.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     2635 2023-05-30 09:15:50.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/arbitrum/radiant_arbitrum.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 01:56:20.080083 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/bsc/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/bsc/__init__.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     8306 2023-05-31 01:43:08.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/bsc/cream_bsc.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     2325 2023-05-31 01:44:35.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/bsc/radiant_bsc.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     3757 2023-05-31 01:44:35.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/bsc/trava_bsc.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     4095 2023-05-31 01:44:35.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/bsc/valas_bsc.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     4743 2023-05-31 01:44:35.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/bsc/venus_bsc.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 01:56:20.083384 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/ethereum/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/ethereum/__init__.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    11944 2023-05-31 01:51:17.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/ethereum/aave_v2_eth.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     3674 2023-05-31 01:51:17.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/ethereum/compound_eth.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     1565 2023-05-31 01:39:39.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/ethereum/trava_eth.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 01:56:20.086131 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/fantom/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/fantom/__init__.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     3257 2023-05-30 07:24:06.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/fantom/geist_ftm.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     1808 2023-05-30 07:34:54.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/fantom/trava_ftm.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 01:56:20.087314 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/optimism/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/optimism/__init__.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 01:56:20.088819 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/polygon/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:00:39.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/polygon/__init__.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     4448 2023-05-31 01:51:18.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/polygon/aave_v2_polygon.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     2078 2023-05-31 01:51:17.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/radiant_service.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 01:56:20.096660 defi-services-lib-1.0.5/src/defi_services/lending_pools/services/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 14:38:12.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/services/__init__.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    13008 2023-05-30 08:59:53.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/services/aave_v2_state_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     4418 2023-05-30 10:39:37.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/services/compound_state_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    20627 2023-05-30 10:36:00.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/services/cream_state_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)      689 2023-05-30 07:24:06.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/services/geist_state_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     1060 2023-05-30 09:13:38.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/services/radiant_state_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    17188 2023-05-30 08:51:45.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/services/trava_state_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    15441 2023-05-30 08:59:53.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/services/valas_state_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)    14936 2023-05-30 10:36:00.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/services/venus_state_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     2411 2023-05-31 01:51:17.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/trava_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     2004 2023-05-31 01:51:18.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/valas_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     2115 2023-05-31 01:51:17.000000 defi-services-lib-1.0.5/src/defi_services/lending_pools/venus_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     4360 2023-05-30 10:51:26.000000 defi-services-lib-1.0.5/src/defi_services/state_service.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 01:56:20.100935 defi-services-lib-1.0.5/src/defi_services/utils/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        0 2023-05-29 08:45:50.000000 defi-services-lib-1.0.5/src/defi_services/utils/__init__.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     1830 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/utils/batch_queries_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     6271 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/utils/graph_operations.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)      723 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/utils/market_service.py
+-rw-r--r--   0 vietbangpham   (501) staff       (20)      851 2023-05-29 03:52:33.000000 defi-services-lib-1.0.5/src/defi_services/utils/memory_storage.py
+drwxr-xr-x   0 vietbangpham   (501) staff       (20)        0 2023-05-31 01:56:20.106065 defi-services-lib-1.0.5/src/defi_services_lib.egg-info/
+-rw-r--r--   0 vietbangpham   (501) staff       (20)      840 2023-05-31 01:56:19.000000 defi-services-lib-1.0.5/src/defi_services_lib.egg-info/PKG-INFO
+-rw-r--r--   0 vietbangpham   (501) staff       (20)     4692 2023-05-31 01:56:20.000000 defi-services-lib-1.0.5/src/defi_services_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 vietbangpham   (501) staff       (20)        1 2023-05-31 01:56:20.000000 defi-services-lib-1.0.5/src/defi_services_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 vietbangpham   (501) staff       (20)       34 2023-05-31 01:56:20.000000 defi-services-lib-1.0.5/src/defi_services_lib.egg-info/requires.txt
+-rw-r--r--   0 vietbangpham   (501) staff       (20)       14 2023-05-31 01:56:20.000000 defi-services-lib-1.0.5/src/defi_services_lib.egg-info/top_level.txt
```

### Comparing `defi-services-lib-1.0.4/LICENSE` & `defi-services-lib-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/PKG-INFO` & `defi-services-lib-1.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: defi-services-lib
-Version: 1.0.4
+Version: 1.0.5
 Summary: Calculate apy, apr, and wallet information,... in decentralized applications.
 Home-page: https://github.com/phamvietbang/defi-services-lib
 Author: Viet-Bang Pham
 Author-email: phamvietbang2965@gmail.com
 Project-URL: Bug Tracker, https://github.com/phamvietbang/defi-services-lib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `defi-services-lib-1.0.4/setup.py` & `defi-services-lib-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/abis/dex/biswap_masterchef_abi.py` & `defi-services-lib-1.0.5/src/defi_services/abis/dex/biswap_masterchef_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/abis/dex/pancakeswap_masterchef_abi.py` & `defi-services-lib-1.0.5/src/defi_services/abis/dex/pancakeswap_masterchef_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/abis/erc20_abi.py` & `defi-services-lib-1.0.5/src/defi_services/abis/erc20_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/alpaca_fair_launch_abi.py` & `defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/alpaca_fair_launch_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/alpaca_vault_abi.py` & `defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/alpaca_vault_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/alpaca_vault_config_abi.py` & `defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/alpaca_vault_config_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/chain_link_abi.py` & `defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/chain_link_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/chef_incentives_controller.py` & `defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/chef_incentives_controller.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/cream_comptroller_abi.py` & `defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/cream_comptroller_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/cream_lens_abi.py` & `defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/cream_lens_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/ctoken_abi.py` & `defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/ctoken_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/lending_pool_abi.py` & `defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/lending_pool_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/oracle_abi.py` & `defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/oracle_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/staked_incentives_abi.py` & `defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/staked_incentives_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/trava_lending_pool_abi.py` & `defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/trava_lending_pool_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/trava_oracle_abi.py` & `defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/trava_oracle_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/valas_multi_fee_distribution.py` & `defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/valas_multi_fee_distribution.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/venus_comptroller_abi.py` & `defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/venus_comptroller_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/venus_lens_abi.py` & `defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/venus_lens_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/abis/lending_pool/venus_lens_abi_v1.py` & `defi-services-lib-1.0.5/src/defi_services/abis/lending_pool/venus_lens_abi_v1.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/abis/vault/incentive_abi.py` & `defi-services-lib-1.0.5/src/defi_services/abis/vault/incentive_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/abis/vault/trava_vault_abi.py` & `defi-services-lib-1.0.5/src/defi_services/abis/vault/trava_vault_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/abis/vault/valuator_abi.py` & `defi-services-lib-1.0.5/src/defi_services/abis/vault/valuator_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/abis/vault/ve_abi.py` & `defi-services-lib-1.0.5/src/defi_services/abis/vault/ve_abi.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/constants/contract_address.py` & `defi-services-lib-1.0.5/src/defi_services/constants/contract_address.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/constants/db_constant.py` & `defi-services-lib-1.0.5/src/defi_services/constants/db_constant.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/constants/mapping_constant.py` & `defi-services-lib-1.0.5/src/defi_services/constants/mapping_constant.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/defi_service.py` & `defi-services-lib-1.0.5/src/defi_services/defi_service.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/lending_pools/aave_v2_service.py` & `defi-services-lib-1.0.5/src/defi_services/lending_pools/aave_v2_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 class AaveV2Service(DefiService):
     name = "aave v2 lending pool"
 
     def __init__(self, chain_id: str, provider_uri: str):
         super().__init__(chain_id, provider_uri)
         self.state_service = AaveV2StateService(provider_uri)
         self.defi_constant = self._get_constant()
+        self.address = self.defi_constant.get("address")
 
     def _get_constant(self):
         if self.chain_id == Chain.polygon:
             return AAVE_V2_POLYGON
         elif self.chain_id == Chain.ethereum:
             return AAVE_V2_ETH
```

### Comparing `defi-services-lib-1.0.4/src/defi_services/lending_pools/compound_service.py` & `defi-services-lib-1.0.5/src/defi_services/lending_pools/compound_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 class CompoundService(DefiService):
     name = "compound lending pool"
 
     def __init__(self, chain_id: str, provider_uri: str):
         super().__init__(chain_id, provider_uri)
         self.state_service = CompoundStateService(provider_uri)
         self.defi_constant = self._get_constant()
+        self.address = self.defi_constant.get("comptrollerAddress")
 
     def _get_constant(self):
         if self.chain_id == Chain.ethereum:
             return COMPOUND_ETH
         return None
 
     def get_pool_token(self):
```

### Comparing `defi-services-lib-1.0.4/src/defi_services/lending_pools/cream_service.py` & `defi-services-lib-1.0.5/src/defi_services/lending_pools/cream_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 class CreamService(DefiService):
     name = "cream lending pool"
 
     def __init__(self, chain_id: str, provider_uri: str):
         super().__init__(chain_id, provider_uri)
         self.state_service = CreamStateService(provider_uri)
         self.defi_constant = self._get_constant()
+        self.address = self.defi_constant.get("comptrollerAddress")
 
     def _get_constant(self):
         if self.chain_id == Chain.bsc:
             return CREAM_BSC
         return None
 
     def get_pool_token(self):
```

### Comparing `defi-services-lib-1.0.4/src/defi_services/lending_pools/geist_service.py` & `defi-services-lib-1.0.5/src/defi_services/lending_pools/geist_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 class GeistService(DefiService):
     name = "geist lending pool"
 
     def __init__(self, chain_id: str, provider_uri: str):
         super().__init__(chain_id, provider_uri)
         self.state_service = GeistStateService(provider_uri)
         self.defi_constant = self._get_constant()
+        self.address = self.defi_constant.get("address")
 
     def _get_constant(self):
         if self.chain_id == Chain.fantom:
             return GEIST_ETH
         return None
 
     def get_apy_defi_app(self, block_number: int = "latest"):
```

### Comparing `defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/arbitrum/radiant_arbitrum.py` & `defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/arbitrum/radiant_arbitrum.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/bsc/cream_bsc.py` & `defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/bsc/cream_bsc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 CREAM_BSC = {
-    "_id": "0x38_0x589de0f0ccf905477646599bb3e5c622c84cc0ba",
     "chainId": "0x38",
-    "createdAt": 1577836800,
     "comptrollerAddress": "0x589de0f0ccf905477646599bb3e5c622c84cc0ba",
     "comptrollerImplementationAddress": "0x49a08f9f445af5734cf15a1deab3b1c6a7988fb4",
-    "projectName": "Cream",
     "name": "Cream Lending Pool",
     "rewardToken": "0xd4cb328a82bdf5f03eb737f37fa6b370aef3e888",
     "lensAddress": "0x1a014ffe0cd187a298a7e79ba5ab05538686ea4a",
     "type": "LENDING_POOL",
     "reservesList": {
         "0x0000000000000000000000000000000000000000": {
             "cToken": "0x1ffe17b99b439be0afc831239ddecda2a790ff3a",
```

### Comparing `defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/bsc/radiant_bsc.py` & `defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/bsc/radiant_bsc.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 RADIANT_BSC = {
-    "address": "0xd50Cf00b6e600Dd036Ba8eF475677d816d6c4281",
+    "address": "0xd50cf00b6e600dd036ba8ef475677d816d6c4281",
     "name": "Radiant Lending Pool",
-    "rewardToken": "0xf7DE7E8A6bd59ED41a4b5fe50278b3B7f31384dF",
-    "multiFeeAddress": "0x4FD9F7C5ca0829A656561486baDA018505dfcB5E",
-    "chefIncentiveAddress": '0x7C16aBb090d3FB266E9d17F60174B632f4229933',
-    "oracleAddress": "0x0BB5c1Bc173b207cBf47CDf013617087776F3782",
+    "rewardToken": "0xf7de7e8a6bd59ed41a4b5fe50278b3b7f31384df",
+    "multiFeeAddress": "0x4fd9f7c5ca0829a656561486bada018505dfcb5e",
+    "chefIncentiveAddress": '0x7c16abb090d3fb266e9d17f60174b632f4229933',
+    "oracleAddress": "0x0bb5c1bc173b207cbf47cdf013617087776f3782",
     "type": "LENDING_POOL",
     "reservesList": {
         "0x7130d2a12b9bcbfae4f2634d864a1ee1ce3ead9c": {
             "tToken": "0x34d4f4459c1b529bebe1c426f1e584151be2c1e5",
             "dToken": "0x3c84437794a5515150982a6f69de5b3e017004a1",
             "sdToken": "0x10db119731a6af08c3bb4207f2ee04e256ab9085",
             "liquidationThreshold": 0.75
```

### Comparing `defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/bsc/trava_bsc.py` & `defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/bsc/trava_bsc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 TRAVA_BSC = {
     "address": "0x75de5f7c91a89c16714017c7443eca20c7a8c295",
-    "stakedIncentiveAddress": "0x4c481E66798c6C82aF77d1e14d3233fE5D592A0b",
+    "stakedIncentiveAddress": "0x4c481e66798c6c82af77d1e14d3233fe5d592a0b",
     "oracleAddress": "0x7cd53b71bf56cc6c9c9b43719fe98e7c360c35df",
     "name": "Trava Lending Pool",
     "rewardToken": "0x170772a06affc0d375ce90ef59c8ec04c7ebf5d2",
     "reservesList": {
         "0x1af3f329e8be154074d8769d1ffa4ee058b1dbc3": {
             "tToken": "0x17335ff98beba2e36d11421d4bd613c24b61acbe",
             "dToken": "0xfa0be8c6dd8bc5d44c54ba538d360380f949d0df",
```

### Comparing `defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/bsc/valas_bsc.py` & `defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/bsc/valas_bsc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 VALAS_BSC = {
     "address": "0xe29a55a6aeff5c8b1beede5bcf2f0cb3af8f91f5",
     "name": "Valas Lending Pool",
     "rewardToken": "0xb1ebdd56729940089ecc3ad0bbeeb12b6842ea6f",
-    "multiFeeAddress": "0x685D3b02b9b0F044A3C01Dbb95408FC2eB15a3b3",
+    "multiFeeAddress": "0x685d3b02b9b0f044a3c01dbb95408fc2eb15a3b3",
     "chefIncentiveAddress": '0xb7c1d99069a4eb582fc04e7e1124794000e7ecbf',
-    "oracleAddress": "0x3436c4B4A27B793539844090e271591cbCb0303c",
+    "oracleAddress": "0x3436c4b4a27b793539844090e271591cbcb0303c",
     "type": "LENDING_POOL",
     "reservesList": {
         "0xbb4cdb9cbd36b01bd1cbaebf2de08d9173bc095c": {
             "createdAt": 1648498798,
             "tToken": "0xb11a912cd93dcffa8b609b4c021e89723ceb7fe8",
             "dToken": "0xe7cdc4e53915d50b74496847eeba7233cae85ce5",
             "id": "binancecoin",
```

### Comparing `defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/bsc/venus_bsc.py` & `defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/bsc/venus_bsc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 VENUS_BSC = {
     "chainId": "0x38",
     "projectName": "Venus",
     "name": "Venus Lending Pool",
     "rewardToken": "0xcf6bb5389c92bdda8a3747ddb454cb7a64626c63",
     "comptrollerAddress": "0xfd36e2c2a6789db23113685031d7f16329158384",
-    "lensAddress": "0xCDa4a4Ab96DfC1728EE265B9392373DB40e769F2",
+    "lensAddress": "0xcda4a4ab96dfc1728ee265b9392373db40e769f2",
     "type": "LENDING_POOL",
     "reservesList": {
         "0x8ac76a51cc950d9822d68b83fe1ad97b32cd580d": {
             "cToken": "0xeca88125a5adbe82614ffc12d0db554e2e2867c8",
             "liquidationThreshold": 0.825
         },
         "0x55d398326f99059ff775485246999027b3197955": {
```

### Comparing `defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/ethereum/aave_v2_eth.py` & `defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/ethereum/aave_v2_eth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 AAVE_V2_ETH = {
-    "address": "0x7d2768dE32b0b80b7a3454c06BdAc94A69DDc7A9",
+    "address": "0x7d2768de32b0b80b7a3454c06bdac94a69ddc7a9",
     "name": "Aave V2 Lending Pool",
-    "rewardToken": "0x7Fc66500c84A76Ad7e9c93437bFc5Ac33E2DDaE9",
-    "stakedIncentiveAddress": '0x83D055D382f25e6793099713505c68a5C7535a35',
-    "oracleAddress": "0xA50ba011c48153De246E5192C8f9258A2ba79Ca9",
+    "rewardToken": "0x7fc66500c84a76ad7e9c93437bfc5ac33e2ddae9",
+    "stakedIncentiveAddress": '0x83d055d382f25e6793099713505c68a5c7535a35',
+    "oracleAddress": "0xa50ba011c48153de246e5192c8f9258a2ba79ca9",
     "type": "LENDING_POOL",
     "reservesList": {
         "0xdac17f958d2ee523a2206206994597c13d831ec7": {
             "tToken": "0x3ed3b47dd13ec9a98b44e6204a523e766b225811",
             "dToken": "0x531842cebbdd378f8ee36d171d6cc9c4fcf475ec",
             "sdToken": "0xe91d55ab2240594855abd11b3faae801fd4c4687",
             "liquidationThreshold": 0.0
```

### Comparing `defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/ethereum/compound_eth.py` & `defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/ethereum/compound_eth.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 COMPOUND_ETH = {
     "chainId": "0x38",
     "name": "Compound Lending Pool",
     "rewardToken": "0xc00e94cb662c3520282e6f5717214004a7f26888",
     "comptrollerAddress": "0x3d9819210a31b4961b30ef54be2aed79b9c9cd3b",
-    "lensAddress": "0xA6c8D1c55951e8AC44a0EaA959Be5Fd21cc07531",
+    "lensAddress": "0xa6c8d1c55951e8ac44a0eaa959be5fd21cc07531",
     "type": "LENDING_POOL",
     "reservesList": {
         "0x0d8775f648430679a709e98d2b0cb6250d2887ef": {
             "cToken": "0x6c8c6b02e7b2be14d4fa6022dfd6d75921d90e4e",
             "liquidationThreshold": 0.6
         },
         "0x6b175474e89094c44da98b954eedeac495271d0f": {
```

### Comparing `defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/ethereum/trava_eth.py` & `defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/ethereum/trava_eth.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 TRAVA_ETH = {
     "address": "0xd61afaaa8a69ba541bc4db9c9b40d4142b43b9a4",
-    "stakedIncentiveAddress": "0x4c481E66798c6C82aF77d1e14d3233fE5D592A0b",
+    "stakedIncentiveAddress": "0x43cf9fb8cf26e46890d6e3a4e6494a843bbb6615",
     "oracleAddress": "0x2bd81260fe864173b6ec1ec9ee41a76366922565",
     "name": "Trava Lending Pool",
     "rewardToken": "0x044ede67afdb0f56d7451bb3aaccaeab3f772fad",
     "reservesList": {
         "0x6b175474e89094c44da98b954eedeac495271d0f": {
             "tToken": "0x9ba5f8d3343cb2555a81b1d6caee25be10526540",
             "dToken": "0xf960570f53d98ac285c4ce81467cbf903c50fa35",
```

### Comparing `defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/fantom/geist_ftm.py` & `defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/fantom/geist_ftm.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/fantom/trava_ftm.py` & `defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/fantom/trava_ftm.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/lending_pools/lending_pools_info/polygon/aave_v2_polygon.py` & `defi-services-lib-1.0.5/src/defi_services/lending_pools/lending_pools_info/polygon/aave_v2_polygon.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 AAVE_V2_POLYGON = {
-    "address": "0x8dFf5E27EA6b7AC08EbFdf9eB090F32ee9a30fcf",
+    "address": "0x8dff5e27ea6b7ac08ebfdf9eb090f32ee9a30fcf",
     "name": "Aave V2 Lending Pool",
-    "rewardToken": "0xD6DF932A45C0f255f85145f286eA0b292B21C90B",
-    "stakedIncentiveAddress": '0x2C901a65071c077C78209b06AB2b5D8eC285aB84',
-    "oracleAddress": "0x0229F777B0fAb107F9591a41d5F02E4e98dB6f2d",
+    "rewardToken": "0xd6df932a45c0f255f85145f286ea0b292b21c90b",
+    "stakedIncentiveAddress": '0x2c901a65071c077c78209b06ab2b5d8ec285ab84',
+    "oracleAddress": "0x0229f777b0fab107f9591a41d5f02e4e98db6f2d",
     "type": "LENDING_POOL",
     "reservesList": {
         "0x8f3cf7ad23cd3cadbd9735aff958023239c6a063": {
             "tToken": "0x27f8d03b3a2196956ed754badc28d73be8830a6e",
             "dToken": "0x75c4d1fb84429023170086f06e682dcbbf537b7d",
             "sdToken": "0x2238101b7014c279aaf6b408a284e49cdbd5db55",
             "liquidationThreshold": 0.8
```

### Comparing `defi-services-lib-1.0.4/src/defi_services/lending_pools/radiant_service.py` & `defi-services-lib-1.0.5/src/defi_services/lending_pools/radiant_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 class RadiantService(DefiService):
     name = "radiant lending pool"
 
     def __init__(self, chain_id: str, provider_uri: str):
         super().__init__(chain_id, provider_uri)
         self.state_service = RadiantStateService(provider_uri)
         self.defi_constant = self._get_constant()
+        self.address = self.defi_constant.get("address")
 
     def _get_constant(self):
         if self.chain_id == Chain.bsc:
             return RADIANT_BSC
         return None
 
     def get_apy_defi_app(self, block_number: int = "latest"):
```

### Comparing `defi-services-lib-1.0.4/src/defi_services/lending_pools/services/aave_v2_state_service.py` & `defi-services-lib-1.0.5/src/defi_services/lending_pools/services/aave_v2_state_service.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/lending_pools/services/compound_state_service.py` & `defi-services-lib-1.0.5/src/defi_services/lending_pools/services/compound_state_service.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/lending_pools/services/cream_state_service.py` & `defi-services-lib-1.0.5/src/defi_services/lending_pools/services/cream_state_service.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/lending_pools/services/geist_state_service.py` & `defi-services-lib-1.0.5/src/defi_services/lending_pools/services/geist_state_service.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/lending_pools/services/radiant_state_service.py` & `defi-services-lib-1.0.5/src/defi_services/lending_pools/services/radiant_state_service.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/lending_pools/services/trava_state_service.py` & `defi-services-lib-1.0.5/src/defi_services/lending_pools/services/trava_state_service.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/lending_pools/services/valas_state_service.py` & `defi-services-lib-1.0.5/src/defi_services/lending_pools/services/valas_state_service.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/lending_pools/services/venus_state_service.py` & `defi-services-lib-1.0.5/src/defi_services/lending_pools/services/venus_state_service.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/lending_pools/trava_service.py` & `defi-services-lib-1.0.5/src/defi_services/lending_pools/trava_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 from defi_services.lending_pools.lending_pools_info.ethereum.trava_eth import TRAVA_ETH
 from defi_services.lending_pools.lending_pools_info.fantom.trava_ftm import TRAVA_FTM
 from defi_services.lending_pools.services.trava_state_service import TravaStateService
 
 
 class TravaService(DefiService):
     name = "trava lending pool"
+
     def __init__(self, chain_id: str, provider_uri: str):
         super().__init__(chain_id, provider_uri)
         self.state_service = TravaStateService(provider_uri)
         self.defi_constant = self._get_constant()
+        self.address = self.defi_constant.get("address")
 
     def _get_constant(self):
         if self.chain_id == Chain.bsc:
             return TRAVA_BSC
         elif self.chain_id == Chain.fantom:
             return TRAVA_FTM
         elif self.chain_id == Chain.ethereum:
```

### Comparing `defi-services-lib-1.0.4/src/defi_services/lending_pools/valas_service.py` & `defi-services-lib-1.0.5/src/defi_services/lending_pools/valas_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 class ValasService(DefiService):
     name = "valas lending pool"
 
     def __init__(self, chain_id: str, provider_uri: str):
         super().__init__(chain_id, provider_uri)
         self.state_service = ValasStateService(provider_uri)
         self.defi_constant = self._get_constant()
+        self.address = self.defi_constant.get("address")
 
     def _get_constant(self):
         if self.chain_id == Chain.bsc:
             return VALAS_BSC
         return None
 
     def get_apy_defi_app(self, block_number: int = "latest"):
```

### Comparing `defi-services-lib-1.0.4/src/defi_services/lending_pools/venus_service.py` & `defi-services-lib-1.0.5/src/defi_services/lending_pools/venus_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 class VenusService(DefiService):
     name = "venus lending pool"
 
     def __init__(self, chain_id: str, provider_uri: str):
         super().__init__(chain_id, provider_uri)
         self.state_service = VenusStateService(provider_uri)
         self.defi_constant = self._get_constant()
+        self.address = self.defi_constant.get("comptrollerAddress")
 
     def _get_constant(self):
         if self.chain_id == Chain.bsc:
             return VENUS_BSC
         return None
 
     def get_pool_token(self):
```

### Comparing `defi-services-lib-1.0.4/src/defi_services/state_service.py` & `defi-services-lib-1.0.5/src/defi_services/state_service.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/utils/batch_queries_service.py` & `defi-services-lib-1.0.5/src/defi_services/utils/batch_queries_service.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/utils/graph_operations.py` & `defi-services-lib-1.0.5/src/defi_services/utils/graph_operations.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/utils/market_service.py` & `defi-services-lib-1.0.5/src/defi_services/utils/market_service.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services/utils/memory_storage.py` & `defi-services-lib-1.0.5/src/defi_services/utils/memory_storage.py`

 * *Files identical despite different names*

### Comparing `defi-services-lib-1.0.4/src/defi_services_lib.egg-info/PKG-INFO` & `defi-services-lib-1.0.5/src/defi_services_lib.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: defi-services-lib
-Version: 1.0.4
+Version: 1.0.5
 Summary: Calculate apy, apr, and wallet information,... in decentralized applications.
 Home-page: https://github.com/phamvietbang/defi-services-lib
 Author: Viet-Bang Pham
 Author-email: phamvietbang2965@gmail.com
 Project-URL: Bug Tracker, https://github.com/phamvietbang/defi-services-lib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `defi-services-lib-1.0.4/src/defi_services_lib.egg-info/SOURCES.txt` & `defi-services-lib-1.0.5/src/defi_services_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

