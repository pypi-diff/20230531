# Comparing `tmp/bubble-sdk-0.1.5.tar.gz` & `tmp/bubble-sdk-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bubble-sdk-0.1.5.tar", last modified: Wed May 31 10:56:53 2023, max compression
+gzip compressed data, was "bubble-sdk-0.1.6.tar", last modified: Wed May 31 10:59:11 2023, max compression
```

## Comparing `bubble-sdk-0.1.5.tar` & `bubble-sdk-0.1.6.tar`

### file list

```diff
@@ -1,249 +1,249 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 10:56:53.192068 bubble-sdk-0.1.5/
--rw-rw-rw-   0        0        0     1101 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     2240 2023-05-31 10:56:53.192068 bubble-sdk-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1325 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 10:56:53.082291 bubble-sdk-0.1.5/bubble/
--rw-rw-rw-   0        0        0      802 2023-05-29 02:03:27.000000 bubble-sdk-0.1.5/bubble/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:56:53.082291 bubble-sdk-0.1.5/bubble/_utils/
--rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/bubble/_utils/__init__.py
--rw-rw-rw-   0        0        0    29754 2023-05-23 08:08:21.000000 bubble-sdk-0.1.5/bubble/_utils/abi.py
--rw-rw-rw-   0        0        0      477 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/bubble/_utils/async_caching.py
--rw-rw-rw-   0        0        0     7956 2023-05-23 08:08:28.000000 bubble-sdk-0.1.5/bubble/_utils/async_transactions.py
--rw-rw-rw-   0        0        0     2136 2023-05-23 08:08:28.000000 bubble-sdk-0.1.5/bubble/_utils/blocks.py
--rw-rw-rw-   0        0        0     1028 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/bubble/_utils/caching.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:56:53.097916 bubble-sdk-0.1.5/bubble/_utils/compat/
--rw-rw-rw-   0        0        0      337 2023-05-23 08:08:28.000000 bubble-sdk-0.1.5/bubble/_utils/compat/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/bubble/_utils/compat/compat_py2.py
--rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/bubble/_utils/compat/compat_py3.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:56:53.097916 bubble-sdk-0.1.5/bubble/_utils/contract_sources/
--rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/bubble/_utils/contract_sources/__init__.py
--rw-rw-rw-   0        0        0     6598 2023-05-23 08:08:21.000000 bubble-sdk-0.1.5/bubble/_utils/contract_sources/compile_contracts.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:56:53.097916 bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/
--rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/__init__.py
--rw-rw-rw-   0        0        0      538 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/_custom_contract_data.py
--rw-rw-rw-   0        0        0     5375 2023-05-23 08:08:31.000000 bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/address_reflector.py
--rw-rw-rw-   0        0        0    18951 2023-05-23 08:08:31.000000 bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/arrays_contract.py
--rw-rw-rw-   0        0        0    14866 2023-05-23 08:08:30.000000 bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/bytes_contracts.py
--rw-rw-rw-   0        0        0     6169 2023-05-23 08:08:30.000000 bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/constructor_contracts.py
--rw-rw-rw-   0        0        0     6395 2023-05-23 08:08:27.000000 bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/contract_caller_tester.py
--rw-rw-rw-   0        0        0    38386 2023-05-23 08:08:30.000000 bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/emitter_contract.py
--rw-rw-rw-   0        0        0     5670 2023-05-23 08:08:20.000000 bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/event_contracts.py
--rw-rw-rw-   0        0        0    15916 2023-05-23 08:08:28.000000 bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/extended_resolver.py
--rw-rw-rw-   0        0        0     1677 2023-05-23 08:08:29.000000 bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/fallback_function_contract.py
--rw-rw-rw-   0        0        0     7712 2023-05-23 08:08:28.000000 bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/math_contract.py
--rw-rw-rw-   0        0        0    16770 2023-05-23 08:08:24.000000 bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/offchain_lookup.py
--rw-rw-rw-   0        0        0    32747 2023-05-23 08:08:24.000000 bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/offchain_resolver.py
--rw-rw-rw-   0        0        0     1856 2023-05-23 08:08:26.000000 bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/payable_tester.py
--rw-rw-rw-   0        0        0    17352 2023-05-23 08:08:21.000000 bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/receive_function_contracts.py
--rw-rw-rw-   0        0        0     5295 2023-05-23 08:08:24.000000 bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/reflector_contracts.py
--rw-rw-rw-   0        0        0     4324 2023-05-23 08:08:28.000000 bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/revert_contract.py
--rw-rw-rw-   0        0        0     3586 2023-05-23 08:08:20.000000 bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/simple_resolver.py
--rw-rw-rw-   0        0        0    11630 2023-05-23 08:08:31.000000 bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/string_contract.py
--rw-rw-rw-   0        0        0    23337 2023-05-23 08:08:26.000000 bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/tuple_contracts.py
--rw-rw-rw-   0        0        0    15485 2023-05-23 08:08:30.000000 bubble-sdk-0.1.5/bubble/_utils/contracts.py
--rw-rw-rw-   0        0        0     1701 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/bubble/_utils/datatypes.py
--rw-rw-rw-   0        0        0     1796 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/bubble/_utils/decorators.py
--rw-rw-rw-   0        0        0      157 2023-05-23 08:08:21.000000 bubble-sdk-0.1.5/bubble/_utils/empty.py
--rw-rw-rw-   0        0        0     9376 2023-05-23 08:08:21.000000 bubble-sdk-0.1.5/bubble/_utils/encoding.py
--rw-rw-rw-   0        0        0     2218 2023-05-23 08:08:27.000000 bubble-sdk-0.1.5/bubble/_utils/ens.py
--rw-rw-rw-   0        0        0    17730 2023-05-23 08:08:29.000000 bubble-sdk-0.1.5/bubble/_utils/events.py
--rw-rw-rw-   0        0        0     2176 2023-05-23 08:08:21.000000 bubble-sdk-0.1.5/bubble/_utils/fee_utils.py
--rw-rw-rw-   0        0        0    12297 2023-05-23 08:08:29.000000 bubble-sdk-0.1.5/bubble/_utils/filters.py
--rw-rw-rw-   0        0        0     3344 2023-05-23 08:51:59.000000 bubble-sdk-0.1.5/bubble/_utils/formatters.py
--rw-rw-rw-   0        0        0       61 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/bubble/_utils/function_identifiers.py
--rw-rw-rw-   0        0        0      204 2023-05-23 08:08:29.000000 bubble-sdk-0.1.5/bubble/_utils/http.py
--rw-rw-rw-   0        0        0      219 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/bubble/_utils/hypothesis.py
--rw-rw-rw-   0        0        0     1088 2023-05-23 08:08:21.000000 bubble-sdk-0.1.5/bubble/_utils/math.py
--rw-rw-rw-   0        0        0    33265 2023-05-25 08:40:49.000000 bubble-sdk-0.1.5/bubble/_utils/method_formatters.py
--rw-rw-rw-   0        0        0     3249 2023-05-23 08:08:27.000000 bubble-sdk-0.1.5/bubble/_utils/module.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:56:53.113542 bubble-sdk-0.1.5/bubble/_utils/module_testing/
--rw-rw-rw-   0        0        0      560 2023-05-22 07:05:55.000000 bubble-sdk-0.1.5/bubble/_utils/module_testing/__init__.py
--rw-rw-rw-   0        0        0   170862 2023-05-23 08:08:29.000000 bubble-sdk-0.1.5/bubble/_utils/module_testing/eth_module.py
--rw-rw-rw-   0        0        0     3519 2023-05-23 08:08:31.000000 bubble-sdk-0.1.5/bubble/_utils/module_testing/go_ethereum_admin_module.py
--rw-rw-rw-   0        0        0    10645 2023-05-23 08:08:25.000000 bubble-sdk-0.1.5/bubble/_utils/module_testing/go_ethereum_personal_module.py
--rw-rw-rw-   0        0        0     1209 2023-05-23 08:08:27.000000 bubble-sdk-0.1.5/bubble/_utils/module_testing/go_ethereum_txpool_module.py
--rw-rw-rw-   0        0        0     4995 2023-05-23 08:08:20.000000 bubble-sdk-0.1.5/bubble/_utils/module_testing/module_testing_utils.py
--rw-rw-rw-   0        0        0     1329 2023-05-23 08:08:27.000000 bubble-sdk-0.1.5/bubble/_utils/module_testing/net_module.py
--rw-rw-rw-   0        0        0     9640 2023-05-23 08:08:30.000000 bubble-sdk-0.1.5/bubble/_utils/module_testing/web3_module.py
--rw-rw-rw-   0        0        0     7132 2023-05-26 01:35:35.000000 bubble-sdk-0.1.5/bubble/_utils/normalizers.py
--rw-rw-rw-   0        0        0     9102 2023-05-23 08:08:25.000000 bubble-sdk-0.1.5/bubble/_utils/request.py
--rw-rw-rw-   0        0        0     8800 2023-05-25 08:41:34.000000 bubble-sdk-0.1.5/bubble/_utils/rpc_abi.py
--rw-rw-rw-   0        0        0     4374 2023-05-23 08:08:24.000000 bubble-sdk-0.1.5/bubble/_utils/threads.py
--rw-rw-rw-   0        0        0     9032 2023-05-26 02:16:43.000000 bubble-sdk-0.1.5/bubble/_utils/transactions.py
--rw-rw-rw-   0        0        0      846 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/bubble/_utils/type_conversion.py
--rw-rw-rw-   0        0        0     1727 2023-05-23 08:08:26.000000 bubble-sdk-0.1.5/bubble/_utils/utility_methods.py
--rw-rw-rw-   0        0        0     6509 2023-05-23 08:08:28.000000 bubble-sdk-0.1.5/bubble/_utils/validation.py
--rw-rw-rw-   0        0        0     1032 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/bubble/_utils/windows.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:56:53.113542 bubble-sdk-0.1.5/bubble/auto/
--rw-rw-rw-   0        0        0       51 2023-05-23 08:08:20.000000 bubble-sdk-0.1.5/bubble/auto/__init__.py
--rw-rw-rw-   0        0        0      282 2023-05-23 08:08:20.000000 bubble-sdk-0.1.5/bubble/auto/gethdev.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:56:53.113542 bubble-sdk-0.1.5/bubble/beacon/
--rw-rw-rw-   0        0        0       93 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/bubble/beacon/__init__.py
--rw-rw-rw-   0        0        0     1555 2023-05-22 02:41:30.000000 bubble-sdk-0.1.5/bubble/beacon/api_endpoints.py
--rw-rw-rw-   0        0        0     5586 2023-05-23 08:08:28.000000 bubble-sdk-0.1.5/bubble/beacon/async_beacon.py
--rw-rw-rw-   0        0        0     4927 2023-05-23 08:08:21.000000 bubble-sdk-0.1.5/bubble/beacon/main.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:56:53.113542 bubble-sdk-0.1.5/bubble/bub/
--rw-rw-rw-   0        0        0      176 2023-05-22 02:55:48.000000 bubble-sdk-0.1.5/bubble/bub/__init__.py
--rw-rw-rw-   0        0        0    19802 2023-05-25 08:16:36.000000 bubble-sdk-0.1.5/bubble/bub/async_bub.py
--rw-rw-rw-   0        0        0     6143 2023-05-23 08:08:31.000000 bubble-sdk-0.1.5/bubble/bub/base_bub.py
--rw-rw-rw-   0        0        0    17985 2023-05-25 08:17:34.000000 bubble-sdk-0.1.5/bubble/bub/bub.py
--rw-rw-rw-   0        0        0      406 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/bubble/constants.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:56:53.113542 bubble-sdk-0.1.5/bubble/contract/
--rw-rw-rw-   0        0        0      228 2023-05-23 08:08:26.000000 bubble-sdk-0.1.5/bubble/contract/__init__.py
--rw-rw-rw-   0        0        0    20413 2023-05-23 08:08:25.000000 bubble-sdk-0.1.5/bubble/contract/async_contract.py
--rw-rw-rw-   0        0        0    36847 2023-05-23 08:08:21.000000 bubble-sdk-0.1.5/bubble/contract/base_contract.py
--rw-rw-rw-   0        0        0    19453 2023-05-23 08:08:20.000000 bubble-sdk-0.1.5/bubble/contract/contract.py
--rw-rw-rw-   0        0        0    12794 2023-05-23 08:08:31.000000 bubble-sdk-0.1.5/bubble/contract/utils.py
--rw-rw-rw-   0        0        0     9390 2023-05-23 08:08:26.000000 bubble-sdk-0.1.5/bubble/datastructures.py
--rw-rw-rw-   0        0        0      827 2023-05-31 10:46:14.000000 bubble-sdk-0.1.5/bubble/debug.py
--rw-rw-rw-   0        0        0      257 2023-05-24 07:10:11.000000 bubble-sdk-0.1.5/bubble/dpos.py
--rw-rw-rw-   0        0        0     6563 2023-05-23 08:08:29.000000 bubble-sdk-0.1.5/bubble/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:56:53.113542 bubble-sdk-0.1.5/bubble/gas_strategies/
--rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/bubble/gas_strategies/__init__.py
--rw-rw-rw-   0        0        0      459 2023-05-25 08:17:34.000000 bubble-sdk-0.1.5/bubble/gas_strategies/rpc.py
--rw-rw-rw-   0        0        0     9277 2023-05-23 08:08:31.000000 bubble-sdk-0.1.5/bubble/gas_strategies/time_based.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:56:53.113542 bubble-sdk-0.1.5/bubble/inner_contract/
--rw-rw-rw-   0        0        0      503 2023-05-25 02:11:17.000000 bubble-sdk-0.1.5/bubble/inner_contract/__init__.py
--rw-rw-rw-   0        0        0     3597 2023-05-24 07:08:55.000000 bubble-sdk-0.1.5/bubble/inner_contract/delegate.py
--rw-rw-rw-   0        0        0     5983 2023-05-23 10:08:11.000000 bubble-sdk-0.1.5/bubble/inner_contract/error_code.py
--rw-rw-rw-   0        0        0     6694 2023-05-31 09:47:08.000000 bubble-sdk-0.1.5/bubble/inner_contract/formatters.py
--rw-rw-rw-   0        0        0    10622 2023-05-31 09:47:30.000000 bubble-sdk-0.1.5/bubble/inner_contract/inner_contract.py
--rw-rw-rw-   0        0        0     9264 2023-05-31 10:37:37.000000 bubble-sdk-0.1.5/bubble/inner_contract/proposal.py
--rw-rw-rw-   0        0        0     1486 2023-05-24 07:26:08.000000 bubble-sdk-0.1.5/bubble/inner_contract/restricting.py
--rw-rw-rw-   0        0        0     1076 2023-05-24 07:26:26.000000 bubble-sdk-0.1.5/bubble/inner_contract/reward.py
--rw-rw-rw-   0        0        0     1747 2023-05-24 07:08:55.000000 bubble-sdk-0.1.5/bubble/inner_contract/slashing.py
--rw-rw-rw-   0        0        0     7134 2023-05-24 07:27:18.000000 bubble-sdk-0.1.5/bubble/inner_contract/staking.py
--rw-rw-rw-   0        0        0      208 2023-05-23 08:08:28.000000 bubble-sdk-0.1.5/bubble/logs.py
--rw-rw-rw-   0        0        0    13900 2023-05-25 09:00:17.000000 bubble-sdk-0.1.5/bubble/main.py
--rw-rw-rw-   0        0        0     8140 2023-05-23 08:08:26.000000 bubble-sdk-0.1.5/bubble/manager.py
--rw-rw-rw-   0        0        0     8699 2023-05-23 08:08:20.000000 bubble-sdk-0.1.5/bubble/method.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:56:53.130672 bubble-sdk-0.1.5/bubble/middleware/
--rw-rw-rw-   0        0        0     3857 2023-05-23 08:08:29.000000 bubble-sdk-0.1.5/bubble/middleware/__init__.py
--rw-rw-rw-   0        0        0      252 2023-05-23 08:08:25.000000 bubble-sdk-0.1.5/bubble/middleware/abi.py
--rw-rw-rw-   0        0        0     2860 2023-05-23 08:08:21.000000 bubble-sdk-0.1.5/bubble/middleware/async_cache.py
--rw-rw-rw-   0        0        0     1858 2023-05-23 08:08:29.000000 bubble-sdk-0.1.5/bubble/middleware/attrdict.py
--rw-rw-rw-   0        0        0     1736 2023-05-23 08:08:26.000000 bubble-sdk-0.1.5/bubble/middleware/bub_poa.py
--rw-rw-rw-   0        0        0     1853 2023-05-23 08:08:24.000000 bubble-sdk-0.1.5/bubble/middleware/buffered_gas_estimate.py
--rw-rw-rw-   0        0        0    13010 2023-05-25 08:17:34.000000 bubble-sdk-0.1.5/bubble/middleware/cache.py
--rw-rw-rw-   0        0        0     1220 2023-05-23 08:08:21.000000 bubble-sdk-0.1.5/bubble/middleware/exception_handling.py
--rw-rw-rw-   0        0        0     3249 2023-05-23 08:08:29.000000 bubble-sdk-0.1.5/bubble/middleware/exception_retry_request.py
--rw-rw-rw-   0        0        0    21799 2023-05-23 08:08:21.000000 bubble-sdk-0.1.5/bubble/middleware/filter.py
--rw-rw-rw-   0        0        0     4742 2023-05-23 08:08:27.000000 bubble-sdk-0.1.5/bubble/middleware/fixture.py
--rw-rw-rw-   0        0        0     4929 2023-05-23 08:08:31.000000 bubble-sdk-0.1.5/bubble/middleware/formatting.py
--rw-rw-rw-   0        0        0     4345 2023-05-23 08:08:26.000000 bubble-sdk-0.1.5/bubble/middleware/gas_price_strategy.py
--rw-rw-rw-   0        0        0      628 2023-05-23 08:08:21.000000 bubble-sdk-0.1.5/bubble/middleware/names.py
--rw-rw-rw-   0        0        0      259 2023-05-23 08:08:31.000000 bubble-sdk-0.1.5/bubble/middleware/normalize_request_parameters.py
--rw-rw-rw-   0        0        0      367 2023-05-23 08:08:21.000000 bubble-sdk-0.1.5/bubble/middleware/pythonic.py
--rw-rw-rw-   0        0        0     4635 2023-05-23 08:08:27.000000 bubble-sdk-0.1.5/bubble/middleware/signing.py
--rw-rw-rw-   0        0        0     1061 2023-05-23 08:08:27.000000 bubble-sdk-0.1.5/bubble/middleware/simulate_unmined_transaction.py
--rw-rw-rw-   0        0        0     3865 2023-05-23 08:08:27.000000 bubble-sdk-0.1.5/bubble/middleware/stalecheck.py
--rw-rw-rw-   0        0        0     4757 2023-05-23 08:08:31.000000 bubble-sdk-0.1.5/bubble/middleware/validation.py
--rw-rw-rw-   0        0        0     3757 2023-05-23 08:08:25.000000 bubble-sdk-0.1.5/bubble/module.py
--rw-rw-rw-   0        0        0     1643 2023-05-23 08:08:24.000000 bubble-sdk-0.1.5/bubble/net.py
--rw-rw-rw-   0        0        0    11907 2023-05-25 08:37:41.000000 bubble-sdk-0.1.5/bubble/node.py
--rw-rw-rw-   0        0        0    22263 2023-05-23 08:08:30.000000 bubble-sdk-0.1.5/bubble/pm.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:56:53.130672 bubble-sdk-0.1.5/bubble/providers/
--rw-rw-rw-   0        0        0      387 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/bubble/providers/__init__.py
--rw-rw-rw-   0        0        0     4320 2023-05-23 08:08:29.000000 bubble-sdk-0.1.5/bubble/providers/async_base.py
--rw-rw-rw-   0        0        0     2567 2023-05-23 08:08:31.000000 bubble-sdk-0.1.5/bubble/providers/async_rpc.py
--rw-rw-rw-   0        0        0     3576 2023-05-23 08:08:25.000000 bubble-sdk-0.1.5/bubble/providers/auto.py
--rw-rw-rw-   0        0        0     4254 2023-05-23 08:08:28.000000 bubble-sdk-0.1.5/bubble/providers/base.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:56:53.145182 bubble-sdk-0.1.5/bubble/providers/bub_tester/
--rw-rw-rw-   0        0        0       99 2023-05-22 06:53:52.000000 bubble-sdk-0.1.5/bubble/providers/bub_tester/__init__.py
--rw-rw-rw-   0        0        0    14864 2023-05-23 08:08:28.000000 bubble-sdk-0.1.5/bubble/providers/bub_tester/defaults.py
--rw-rw-rw-   0        0        0     5690 2023-05-23 08:08:25.000000 bubble-sdk-0.1.5/bubble/providers/bub_tester/main.py
--rw-rw-rw-   0        0        0    13288 2023-05-26 02:23:29.000000 bubble-sdk-0.1.5/bubble/providers/bub_tester/middleware.py
--rw-rw-rw-   0        0        0     6758 2023-05-23 08:08:26.000000 bubble-sdk-0.1.5/bubble/providers/ipc.py
--rw-rw-rw-   0        0        0     2796 2023-05-23 08:08:30.000000 bubble-sdk-0.1.5/bubble/providers/rpc.py
--rw-rw-rw-   0        0        0     4062 2023-05-23 08:08:26.000000 bubble-sdk-0.1.5/bubble/providers/websocket.py
--rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/bubble/py.typed
-drwxrwxrwx   0        0        0        0 2023-05-31 10:56:53.145182 bubble-sdk-0.1.5/bubble/scripts/
--rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/bubble/scripts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:56:53.145182 bubble-sdk-0.1.5/bubble/scripts/release/
--rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/bubble/scripts/release/__init__.py
--rw-rw-rw-   0        0        0     1594 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/bubble/scripts/release/test_package.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:56:53.145182 bubble-sdk-0.1.5/bubble/tools/
--rw-rw-rw-   0        0        0       75 2023-05-22 03:56:23.000000 bubble-sdk-0.1.5/bubble/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:56:53.145182 bubble-sdk-0.1.5/bubble/tools/benchmark/
--rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/bubble/tools/benchmark/__init__.py
--rw-rw-rw-   0        0        0     6098 2023-05-25 08:17:34.000000 bubble-sdk-0.1.5/bubble/tools/benchmark/main.py
--rw-rw-rw-   0        0        0     3542 2023-05-23 08:08:26.000000 bubble-sdk-0.1.5/bubble/tools/benchmark/node.py
--rw-rw-rw-   0        0        0      951 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/bubble/tools/benchmark/reporting.py
--rw-rw-rw-   0        0        0     1791 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/bubble/tools/benchmark/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:56:53.145182 bubble-sdk-0.1.5/bubble/tools/pytest_bubble/
--rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/bubble/tools/pytest_bubble/__init__.py
--rw-rw-rw-   0        0        0     4307 2023-05-23 08:08:28.000000 bubble-sdk-0.1.5/bubble/tools/pytest_bubble/_utils.py
--rw-rw-rw-   0        0        0     1471 2023-05-23 08:08:26.000000 bubble-sdk-0.1.5/bubble/tools/pytest_bubble/deployer.py
--rw-rw-rw-   0        0        0      402 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/bubble/tools/pytest_bubble/exceptions.py
--rw-rw-rw-   0        0        0     4053 2023-05-23 08:08:31.000000 bubble-sdk-0.1.5/bubble/tools/pytest_bubble/linker.py
--rw-rw-rw-   0        0        0      680 2023-05-23 08:08:26.000000 bubble-sdk-0.1.5/bubble/tools/pytest_bubble/plugins.py
--rw-rw-rw-   0        0        0     3302 2023-05-25 08:43:00.000000 bubble-sdk-0.1.5/bubble/tracing.py
--rw-rw-rw-   0        0        0    13659 2023-05-24 07:08:55.000000 bubble-sdk-0.1.5/bubble/types.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:56:53.145182 bubble-sdk-0.1.5/bubble/utils/
--rw-rw-rw-   0        0        0      472 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/bubble/utils/__init__.py
--rw-rw-rw-   0        0        0      521 2023-05-23 08:08:21.000000 bubble-sdk-0.1.5/bubble/utils/abi.py
--rw-rw-rw-   0        0        0     1008 2023-05-23 08:08:21.000000 bubble-sdk-0.1.5/bubble/utils/address.py
--rw-rw-rw-   0        0        0     3199 2023-05-23 08:08:27.000000 bubble-sdk-0.1.5/bubble/utils/async_exception_handling.py
--rw-rw-rw-   0        0        0     1569 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/bubble/utils/caching.py
--rw-rw-rw-   0        0        0     3157 2023-05-23 08:08:25.000000 bubble-sdk-0.1.5/bubble/utils/exception_handling.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:56:53.160849 bubble-sdk-0.1.5/bubble_sdk.egg-info/
--rw-rw-rw-   0        0        0     2240 2023-05-31 10:56:52.000000 bubble-sdk-0.1.5/bubble_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6916 2023-05-31 10:56:53.000000 bubble-sdk-0.1.5/bubble_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 10:56:52.000000 bubble-sdk-0.1.5/bubble_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-05-31 10:56:52.000000 bubble-sdk-0.1.5/bubble_sdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-31 10:56:52.000000 bubble-sdk-0.1.5/bubble_sdk.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     1174 2023-05-31 10:56:52.000000 bubble-sdk-0.1.5/bubble_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-31 10:56:52.000000 bubble-sdk-0.1.5/bubble_sdk.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-31 10:56:53.176444 bubble-sdk-0.1.5/ens/
--rw-rw-rw-   0        0        0      305 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/ens/__init__.py
--rw-rw-rw-   0        0        0    24627 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/ens/abis.py
--rw-rw-rw-   0        0        0    21480 2023-05-23 08:08:30.000000 bubble-sdk-0.1.5/ens/async_ens.py
--rw-rw-rw-   0        0        0       46 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/ens/auto.py
--rw-rw-rw-   0        0        0     3412 2023-05-23 08:08:26.000000 bubble-sdk-0.1.5/ens/base_ens.py
--rw-rw-rw-   0        0        0      629 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/ens/constants.py
--rw-rw-rw-   0        0        0   199146 2023-05-23 08:08:30.000000 bubble-sdk-0.1.5/ens/contract_data.py
--rw-rw-rw-   0        0        0    20613 2023-05-23 08:08:28.000000 bubble-sdk-0.1.5/ens/ens.py
--rw-rw-rw-   0        0        0     2511 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/ens/exceptions.py
--rw-rw-rw-   0        0        0     9333 2023-05-23 08:08:27.000000 bubble-sdk-0.1.5/ens/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:56:53.176444 bubble-sdk-0.1.5/ethpm/
--rw-rw-rw-   0        0        0      775 2023-05-22 03:42:55.000000 bubble-sdk-0.1.5/ethpm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:56:53.176444 bubble-sdk-0.1.5/ethpm/_utils/
--rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/ethpm/_utils/__init__.py
--rw-rw-rw-   0        0        0     2604 2023-05-22 03:42:55.000000 bubble-sdk-0.1.5/ethpm/_utils/backend.py
--rw-rw-rw-   0        0        0     1521 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/ethpm/_utils/cache.py
--rw-rw-rw-   0        0        0     2969 2023-05-23 08:08:29.000000 bubble-sdk-0.1.5/ethpm/_utils/chains.py
--rw-rw-rw-   0        0        0     1065 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/ethpm/_utils/contract.py
--rw-rw-rw-   0        0        0     5410 2023-05-23 08:08:21.000000 bubble-sdk-0.1.5/ethpm/_utils/deployments.py
--rw-rw-rw-   0        0        0     2835 2023-05-23 08:08:28.000000 bubble-sdk-0.1.5/ethpm/_utils/ipfs.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:56:53.176444 bubble-sdk-0.1.5/ethpm/_utils/protobuf/
--rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/ethpm/_utils/protobuf/__init__.py
--rw-rw-rw-   0        0        0     1971 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/ethpm/_utils/protobuf/ipfs_file_pb2.py
--rw-rw-rw-   0        0        0     1517 2023-05-22 02:41:29.000000 bubble-sdk-0.1.5/ethpm/_utils/registry.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:56:53.176444 bubble-sdk-0.1.5/ethpm/assets/
--rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/ethpm/assets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:56:53.176444 bubble-sdk-0.1.5/ethpm/backends/
--rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/ethpm/backends/__init__.py
--rw-rw-rw-   0        0        0      999 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/ethpm/backends/base.py
--rw-rw-rw-   0        0        0     3114 2023-05-22 03:42:55.000000 bubble-sdk-0.1.5/ethpm/backends/http.py
--rw-rw-rw-   0        0        0     6772 2023-05-23 08:08:32.000000 bubble-sdk-0.1.5/ethpm/backends/ipfs.py
--rw-rw-rw-   0        0        0     4332 2023-05-23 08:08:25.000000 bubble-sdk-0.1.5/ethpm/backends/registry.py
--rw-rw-rw-   0        0        0      422 2023-05-22 03:42:55.000000 bubble-sdk-0.1.5/ethpm/constants.py
--rw-rw-rw-   0        0        0     6448 2023-05-23 08:08:21.000000 bubble-sdk-0.1.5/ethpm/contract.py
--rw-rw-rw-   0        0        0     1948 2023-05-22 03:42:55.000000 bubble-sdk-0.1.5/ethpm/dependencies.py
--rw-rw-rw-   0        0        0     2218 2023-05-23 08:08:29.000000 bubble-sdk-0.1.5/ethpm/deployments.py
--rw-rw-rw-   0        0        0     1262 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/ethpm/exceptions.py
--rw-rw-rw-   0        0        0    14939 2023-05-23 08:08:20.000000 bubble-sdk-0.1.5/ethpm/package.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:56:53.176444 bubble-sdk-0.1.5/ethpm/tools/
--rw-rw-rw-   0        0        0      107 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/ethpm/tools/__init__.py
--rw-rw-rw-   0        0        0    27981 2023-05-23 08:08:21.000000 bubble-sdk-0.1.5/ethpm/tools/builder.py
--rw-rw-rw-   0        0        0    10687 2023-05-23 08:08:28.000000 bubble-sdk-0.1.5/ethpm/tools/checker.py
--rw-rw-rw-   0        0        0      494 2023-05-22 03:42:55.000000 bubble-sdk-0.1.5/ethpm/tools/get_manifest.py
--rw-rw-rw-   0        0        0     4513 2023-05-23 08:08:26.000000 bubble-sdk-0.1.5/ethpm/uri.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:56:53.192068 bubble-sdk-0.1.5/ethpm/validation/
--rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.5/ethpm/validation/__init__.py
--rw-rw-rw-   0        0        0     4862 2023-05-22 03:42:55.000000 bubble-sdk-0.1.5/ethpm/validation/manifest.py
--rw-rw-rw-   0        0        0     1115 2023-05-23 08:08:31.000000 bubble-sdk-0.1.5/ethpm/validation/misc.py
--rw-rw-rw-   0        0        0     2397 2023-05-22 03:42:55.000000 bubble-sdk-0.1.5/ethpm/validation/package.py
--rw-rw-rw-   0        0        0     5038 2023-05-23 08:08:28.000000 bubble-sdk-0.1.5/ethpm/validation/uri.py
--rw-rw-rw-   0        0        0       42 2023-05-31 10:56:53.192068 bubble-sdk-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     3300 2023-05-31 10:52:08.000000 bubble-sdk-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.439926 bubble-sdk-0.1.6/
+-rw-rw-rw-   0        0        0     1101 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     2240 2023-05-31 10:59:11.439926 bubble-sdk-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1325 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.330139 bubble-sdk-0.1.6/bubble/
+-rw-rw-rw-   0        0        0      802 2023-05-29 02:03:27.000000 bubble-sdk-0.1.6/bubble/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.345772 bubble-sdk-0.1.6/bubble/_utils/
+-rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/_utils/__init__.py
+-rw-rw-rw-   0        0        0    29754 2023-05-23 08:08:21.000000 bubble-sdk-0.1.6/bubble/_utils/abi.py
+-rw-rw-rw-   0        0        0      477 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/_utils/async_caching.py
+-rw-rw-rw-   0        0        0     7956 2023-05-23 08:08:28.000000 bubble-sdk-0.1.6/bubble/_utils/async_transactions.py
+-rw-rw-rw-   0        0        0     2136 2023-05-23 08:08:28.000000 bubble-sdk-0.1.6/bubble/_utils/blocks.py
+-rw-rw-rw-   0        0        0     1028 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/_utils/caching.py
+drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.361400 bubble-sdk-0.1.6/bubble/_utils/compat/
+-rw-rw-rw-   0        0        0      337 2023-05-23 08:08:28.000000 bubble-sdk-0.1.6/bubble/_utils/compat/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/_utils/compat/compat_py2.py
+-rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/_utils/compat/compat_py3.py
+drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.361400 bubble-sdk-0.1.6/bubble/_utils/contract_sources/
+-rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/__init__.py
+-rw-rw-rw-   0        0        0     6598 2023-05-23 08:08:21.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/compile_contracts.py
+drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.361400 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/
+-rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/__init__.py
+-rw-rw-rw-   0        0        0      538 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/_custom_contract_data.py
+-rw-rw-rw-   0        0        0     5375 2023-05-23 08:08:31.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/address_reflector.py
+-rw-rw-rw-   0        0        0    18951 2023-05-23 08:08:31.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/arrays_contract.py
+-rw-rw-rw-   0        0        0    14866 2023-05-23 08:08:30.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/bytes_contracts.py
+-rw-rw-rw-   0        0        0     6169 2023-05-23 08:08:30.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/constructor_contracts.py
+-rw-rw-rw-   0        0        0     6395 2023-05-23 08:08:27.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/contract_caller_tester.py
+-rw-rw-rw-   0        0        0    38386 2023-05-23 08:08:30.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/emitter_contract.py
+-rw-rw-rw-   0        0        0     5670 2023-05-23 08:08:20.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/event_contracts.py
+-rw-rw-rw-   0        0        0    15916 2023-05-23 08:08:28.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/extended_resolver.py
+-rw-rw-rw-   0        0        0     1677 2023-05-23 08:08:29.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/fallback_function_contract.py
+-rw-rw-rw-   0        0        0     7712 2023-05-23 08:08:28.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/math_contract.py
+-rw-rw-rw-   0        0        0    16770 2023-05-23 08:08:24.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/offchain_lookup.py
+-rw-rw-rw-   0        0        0    32747 2023-05-23 08:08:24.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/offchain_resolver.py
+-rw-rw-rw-   0        0        0     1856 2023-05-23 08:08:26.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/payable_tester.py
+-rw-rw-rw-   0        0        0    17352 2023-05-23 08:08:21.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/receive_function_contracts.py
+-rw-rw-rw-   0        0        0     5295 2023-05-23 08:08:24.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/reflector_contracts.py
+-rw-rw-rw-   0        0        0     4324 2023-05-23 08:08:28.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/revert_contract.py
+-rw-rw-rw-   0        0        0     3586 2023-05-23 08:08:20.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/simple_resolver.py
+-rw-rw-rw-   0        0        0    11630 2023-05-23 08:08:31.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/string_contract.py
+-rw-rw-rw-   0        0        0    23337 2023-05-23 08:08:26.000000 bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/tuple_contracts.py
+-rw-rw-rw-   0        0        0    15485 2023-05-23 08:08:30.000000 bubble-sdk-0.1.6/bubble/_utils/contracts.py
+-rw-rw-rw-   0        0        0     1701 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/_utils/datatypes.py
+-rw-rw-rw-   0        0        0     1796 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/_utils/decorators.py
+-rw-rw-rw-   0        0        0      157 2023-05-23 08:08:21.000000 bubble-sdk-0.1.6/bubble/_utils/empty.py
+-rw-rw-rw-   0        0        0     9376 2023-05-23 08:08:21.000000 bubble-sdk-0.1.6/bubble/_utils/encoding.py
+-rw-rw-rw-   0        0        0     2218 2023-05-23 08:08:27.000000 bubble-sdk-0.1.6/bubble/_utils/ens.py
+-rw-rw-rw-   0        0        0    17730 2023-05-23 08:08:29.000000 bubble-sdk-0.1.6/bubble/_utils/events.py
+-rw-rw-rw-   0        0        0     2176 2023-05-23 08:08:21.000000 bubble-sdk-0.1.6/bubble/_utils/fee_utils.py
+-rw-rw-rw-   0        0        0    12297 2023-05-23 08:08:29.000000 bubble-sdk-0.1.6/bubble/_utils/filters.py
+-rw-rw-rw-   0        0        0     3344 2023-05-23 08:51:59.000000 bubble-sdk-0.1.6/bubble/_utils/formatters.py
+-rw-rw-rw-   0        0        0       61 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/_utils/function_identifiers.py
+-rw-rw-rw-   0        0        0      204 2023-05-23 08:08:29.000000 bubble-sdk-0.1.6/bubble/_utils/http.py
+-rw-rw-rw-   0        0        0      219 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/_utils/hypothesis.py
+-rw-rw-rw-   0        0        0     1088 2023-05-23 08:08:21.000000 bubble-sdk-0.1.6/bubble/_utils/math.py
+-rw-rw-rw-   0        0        0    33265 2023-05-25 08:40:49.000000 bubble-sdk-0.1.6/bubble/_utils/method_formatters.py
+-rw-rw-rw-   0        0        0     3249 2023-05-23 08:08:27.000000 bubble-sdk-0.1.6/bubble/_utils/module.py
+drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.361400 bubble-sdk-0.1.6/bubble/_utils/module_testing/
+-rw-rw-rw-   0        0        0      560 2023-05-22 07:05:55.000000 bubble-sdk-0.1.6/bubble/_utils/module_testing/__init__.py
+-rw-rw-rw-   0        0        0   170862 2023-05-23 08:08:29.000000 bubble-sdk-0.1.6/bubble/_utils/module_testing/eth_module.py
+-rw-rw-rw-   0        0        0     3519 2023-05-23 08:08:31.000000 bubble-sdk-0.1.6/bubble/_utils/module_testing/go_ethereum_admin_module.py
+-rw-rw-rw-   0        0        0    10645 2023-05-23 08:08:25.000000 bubble-sdk-0.1.6/bubble/_utils/module_testing/go_ethereum_personal_module.py
+-rw-rw-rw-   0        0        0     1209 2023-05-23 08:08:27.000000 bubble-sdk-0.1.6/bubble/_utils/module_testing/go_ethereum_txpool_module.py
+-rw-rw-rw-   0        0        0     4995 2023-05-23 08:08:20.000000 bubble-sdk-0.1.6/bubble/_utils/module_testing/module_testing_utils.py
+-rw-rw-rw-   0        0        0     1329 2023-05-23 08:08:27.000000 bubble-sdk-0.1.6/bubble/_utils/module_testing/net_module.py
+-rw-rw-rw-   0        0        0     9640 2023-05-23 08:08:30.000000 bubble-sdk-0.1.6/bubble/_utils/module_testing/web3_module.py
+-rw-rw-rw-   0        0        0     7132 2023-05-26 01:35:35.000000 bubble-sdk-0.1.6/bubble/_utils/normalizers.py
+-rw-rw-rw-   0        0        0     9102 2023-05-23 08:08:25.000000 bubble-sdk-0.1.6/bubble/_utils/request.py
+-rw-rw-rw-   0        0        0     8800 2023-05-25 08:41:34.000000 bubble-sdk-0.1.6/bubble/_utils/rpc_abi.py
+-rw-rw-rw-   0        0        0     4374 2023-05-23 08:08:24.000000 bubble-sdk-0.1.6/bubble/_utils/threads.py
+-rw-rw-rw-   0        0        0     9032 2023-05-26 02:16:43.000000 bubble-sdk-0.1.6/bubble/_utils/transactions.py
+-rw-rw-rw-   0        0        0      846 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/_utils/type_conversion.py
+-rw-rw-rw-   0        0        0     1727 2023-05-23 08:08:26.000000 bubble-sdk-0.1.6/bubble/_utils/utility_methods.py
+-rw-rw-rw-   0        0        0     6509 2023-05-23 08:08:28.000000 bubble-sdk-0.1.6/bubble/_utils/validation.py
+-rw-rw-rw-   0        0        0     1032 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/_utils/windows.py
+drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.377027 bubble-sdk-0.1.6/bubble/auto/
+-rw-rw-rw-   0        0        0       51 2023-05-23 08:08:20.000000 bubble-sdk-0.1.6/bubble/auto/__init__.py
+-rw-rw-rw-   0        0        0      282 2023-05-23 08:08:20.000000 bubble-sdk-0.1.6/bubble/auto/gethdev.py
+drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.377027 bubble-sdk-0.1.6/bubble/beacon/
+-rw-rw-rw-   0        0        0       93 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/beacon/__init__.py
+-rw-rw-rw-   0        0        0     1555 2023-05-22 02:41:30.000000 bubble-sdk-0.1.6/bubble/beacon/api_endpoints.py
+-rw-rw-rw-   0        0        0     5586 2023-05-23 08:08:28.000000 bubble-sdk-0.1.6/bubble/beacon/async_beacon.py
+-rw-rw-rw-   0        0        0     4927 2023-05-23 08:08:21.000000 bubble-sdk-0.1.6/bubble/beacon/main.py
+drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.377027 bubble-sdk-0.1.6/bubble/bub/
+-rw-rw-rw-   0        0        0      176 2023-05-22 02:55:48.000000 bubble-sdk-0.1.6/bubble/bub/__init__.py
+-rw-rw-rw-   0        0        0    19802 2023-05-25 08:16:36.000000 bubble-sdk-0.1.6/bubble/bub/async_bub.py
+-rw-rw-rw-   0        0        0     6143 2023-05-23 08:08:31.000000 bubble-sdk-0.1.6/bubble/bub/base_bub.py
+-rw-rw-rw-   0        0        0    17985 2023-05-25 08:17:34.000000 bubble-sdk-0.1.6/bubble/bub/bub.py
+-rw-rw-rw-   0        0        0      406 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/constants.py
+drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.377027 bubble-sdk-0.1.6/bubble/contract/
+-rw-rw-rw-   0        0        0      228 2023-05-23 08:08:26.000000 bubble-sdk-0.1.6/bubble/contract/__init__.py
+-rw-rw-rw-   0        0        0    20413 2023-05-23 08:08:25.000000 bubble-sdk-0.1.6/bubble/contract/async_contract.py
+-rw-rw-rw-   0        0        0    36847 2023-05-23 08:08:21.000000 bubble-sdk-0.1.6/bubble/contract/base_contract.py
+-rw-rw-rw-   0        0        0    19453 2023-05-23 08:08:20.000000 bubble-sdk-0.1.6/bubble/contract/contract.py
+-rw-rw-rw-   0        0        0    12794 2023-05-23 08:08:31.000000 bubble-sdk-0.1.6/bubble/contract/utils.py
+-rw-rw-rw-   0        0        0     9390 2023-05-23 08:08:26.000000 bubble-sdk-0.1.6/bubble/datastructures.py
+-rw-rw-rw-   0        0        0      827 2023-05-31 10:46:14.000000 bubble-sdk-0.1.6/bubble/debug.py
+-rw-rw-rw-   0        0        0      257 2023-05-24 07:10:11.000000 bubble-sdk-0.1.6/bubble/dpos.py
+-rw-rw-rw-   0        0        0     6563 2023-05-23 08:08:29.000000 bubble-sdk-0.1.6/bubble/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.377027 bubble-sdk-0.1.6/bubble/gas_strategies/
+-rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/gas_strategies/__init__.py
+-rw-rw-rw-   0        0        0      459 2023-05-25 08:17:34.000000 bubble-sdk-0.1.6/bubble/gas_strategies/rpc.py
+-rw-rw-rw-   0        0        0     9277 2023-05-23 08:08:31.000000 bubble-sdk-0.1.6/bubble/gas_strategies/time_based.py
+drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.377027 bubble-sdk-0.1.6/bubble/inner_contract/
+-rw-rw-rw-   0        0        0      503 2023-05-25 02:11:17.000000 bubble-sdk-0.1.6/bubble/inner_contract/__init__.py
+-rw-rw-rw-   0        0        0     3597 2023-05-24 07:08:55.000000 bubble-sdk-0.1.6/bubble/inner_contract/delegate.py
+-rw-rw-rw-   0        0        0     5983 2023-05-23 10:08:11.000000 bubble-sdk-0.1.6/bubble/inner_contract/error_code.py
+-rw-rw-rw-   0        0        0     6694 2023-05-31 09:47:08.000000 bubble-sdk-0.1.6/bubble/inner_contract/formatters.py
+-rw-rw-rw-   0        0        0    10622 2023-05-31 09:47:30.000000 bubble-sdk-0.1.6/bubble/inner_contract/inner_contract.py
+-rw-rw-rw-   0        0        0     9264 2023-05-31 10:37:37.000000 bubble-sdk-0.1.6/bubble/inner_contract/proposal.py
+-rw-rw-rw-   0        0        0     1486 2023-05-24 07:26:08.000000 bubble-sdk-0.1.6/bubble/inner_contract/restricting.py
+-rw-rw-rw-   0        0        0     1076 2023-05-24 07:26:26.000000 bubble-sdk-0.1.6/bubble/inner_contract/reward.py
+-rw-rw-rw-   0        0        0     1747 2023-05-24 07:08:55.000000 bubble-sdk-0.1.6/bubble/inner_contract/slashing.py
+-rw-rw-rw-   0        0        0     7134 2023-05-24 07:27:18.000000 bubble-sdk-0.1.6/bubble/inner_contract/staking.py
+-rw-rw-rw-   0        0        0      208 2023-05-23 08:08:28.000000 bubble-sdk-0.1.6/bubble/logs.py
+-rw-rw-rw-   0        0        0    13900 2023-05-25 09:00:17.000000 bubble-sdk-0.1.6/bubble/main.py
+-rw-rw-rw-   0        0        0     8140 2023-05-23 08:08:26.000000 bubble-sdk-0.1.6/bubble/manager.py
+-rw-rw-rw-   0        0        0     8699 2023-05-23 08:08:20.000000 bubble-sdk-0.1.6/bubble/method.py
+drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.392646 bubble-sdk-0.1.6/bubble/middleware/
+-rw-rw-rw-   0        0        0     3857 2023-05-23 08:08:29.000000 bubble-sdk-0.1.6/bubble/middleware/__init__.py
+-rw-rw-rw-   0        0        0      252 2023-05-23 08:08:25.000000 bubble-sdk-0.1.6/bubble/middleware/abi.py
+-rw-rw-rw-   0        0        0     2860 2023-05-23 08:08:21.000000 bubble-sdk-0.1.6/bubble/middleware/async_cache.py
+-rw-rw-rw-   0        0        0     1858 2023-05-23 08:08:29.000000 bubble-sdk-0.1.6/bubble/middleware/attrdict.py
+-rw-rw-rw-   0        0        0     1736 2023-05-23 08:08:26.000000 bubble-sdk-0.1.6/bubble/middleware/bub_poa.py
+-rw-rw-rw-   0        0        0     1853 2023-05-23 08:08:24.000000 bubble-sdk-0.1.6/bubble/middleware/buffered_gas_estimate.py
+-rw-rw-rw-   0        0        0    13010 2023-05-25 08:17:34.000000 bubble-sdk-0.1.6/bubble/middleware/cache.py
+-rw-rw-rw-   0        0        0     1220 2023-05-23 08:08:21.000000 bubble-sdk-0.1.6/bubble/middleware/exception_handling.py
+-rw-rw-rw-   0        0        0     3249 2023-05-23 08:08:29.000000 bubble-sdk-0.1.6/bubble/middleware/exception_retry_request.py
+-rw-rw-rw-   0        0        0    21799 2023-05-23 08:08:21.000000 bubble-sdk-0.1.6/bubble/middleware/filter.py
+-rw-rw-rw-   0        0        0     4742 2023-05-23 08:08:27.000000 bubble-sdk-0.1.6/bubble/middleware/fixture.py
+-rw-rw-rw-   0        0        0     4929 2023-05-23 08:08:31.000000 bubble-sdk-0.1.6/bubble/middleware/formatting.py
+-rw-rw-rw-   0        0        0     4345 2023-05-23 08:08:26.000000 bubble-sdk-0.1.6/bubble/middleware/gas_price_strategy.py
+-rw-rw-rw-   0        0        0      628 2023-05-23 08:08:21.000000 bubble-sdk-0.1.6/bubble/middleware/names.py
+-rw-rw-rw-   0        0        0      259 2023-05-23 08:08:31.000000 bubble-sdk-0.1.6/bubble/middleware/normalize_request_parameters.py
+-rw-rw-rw-   0        0        0      367 2023-05-23 08:08:21.000000 bubble-sdk-0.1.6/bubble/middleware/pythonic.py
+-rw-rw-rw-   0        0        0     4635 2023-05-23 08:08:27.000000 bubble-sdk-0.1.6/bubble/middleware/signing.py
+-rw-rw-rw-   0        0        0     1061 2023-05-23 08:08:27.000000 bubble-sdk-0.1.6/bubble/middleware/simulate_unmined_transaction.py
+-rw-rw-rw-   0        0        0     3865 2023-05-23 08:08:27.000000 bubble-sdk-0.1.6/bubble/middleware/stalecheck.py
+-rw-rw-rw-   0        0        0     4757 2023-05-23 08:08:31.000000 bubble-sdk-0.1.6/bubble/middleware/validation.py
+-rw-rw-rw-   0        0        0     3757 2023-05-23 08:08:25.000000 bubble-sdk-0.1.6/bubble/module.py
+-rw-rw-rw-   0        0        0     1643 2023-05-23 08:08:24.000000 bubble-sdk-0.1.6/bubble/net.py
+-rw-rw-rw-   0        0        0    11907 2023-05-25 08:37:41.000000 bubble-sdk-0.1.6/bubble/node.py
+-rw-rw-rw-   0        0        0    22263 2023-05-23 08:08:30.000000 bubble-sdk-0.1.6/bubble/pm.py
+drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.392646 bubble-sdk-0.1.6/bubble/providers/
+-rw-rw-rw-   0        0        0      387 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/providers/__init__.py
+-rw-rw-rw-   0        0        0     4320 2023-05-23 08:08:29.000000 bubble-sdk-0.1.6/bubble/providers/async_base.py
+-rw-rw-rw-   0        0        0     2567 2023-05-23 08:08:31.000000 bubble-sdk-0.1.6/bubble/providers/async_rpc.py
+-rw-rw-rw-   0        0        0     3576 2023-05-23 08:08:25.000000 bubble-sdk-0.1.6/bubble/providers/auto.py
+-rw-rw-rw-   0        0        0     4254 2023-05-23 08:08:28.000000 bubble-sdk-0.1.6/bubble/providers/base.py
+drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.392646 bubble-sdk-0.1.6/bubble/providers/bub_tester/
+-rw-rw-rw-   0        0        0       99 2023-05-22 06:53:52.000000 bubble-sdk-0.1.6/bubble/providers/bub_tester/__init__.py
+-rw-rw-rw-   0        0        0    14864 2023-05-23 08:08:28.000000 bubble-sdk-0.1.6/bubble/providers/bub_tester/defaults.py
+-rw-rw-rw-   0        0        0     5690 2023-05-23 08:08:25.000000 bubble-sdk-0.1.6/bubble/providers/bub_tester/main.py
+-rw-rw-rw-   0        0        0    13288 2023-05-26 02:23:29.000000 bubble-sdk-0.1.6/bubble/providers/bub_tester/middleware.py
+-rw-rw-rw-   0        0        0     6758 2023-05-23 08:08:26.000000 bubble-sdk-0.1.6/bubble/providers/ipc.py
+-rw-rw-rw-   0        0        0     2796 2023-05-23 08:08:30.000000 bubble-sdk-0.1.6/bubble/providers/rpc.py
+-rw-rw-rw-   0        0        0     4062 2023-05-23 08:08:26.000000 bubble-sdk-0.1.6/bubble/providers/websocket.py
+-rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/py.typed
+drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.392646 bubble-sdk-0.1.6/bubble/scripts/
+-rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/scripts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.392646 bubble-sdk-0.1.6/bubble/scripts/release/
+-rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/scripts/release/__init__.py
+-rw-rw-rw-   0        0        0     1594 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/scripts/release/test_package.py
+drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.392646 bubble-sdk-0.1.6/bubble/tools/
+-rw-rw-rw-   0        0        0       75 2023-05-22 03:56:23.000000 bubble-sdk-0.1.6/bubble/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.392646 bubble-sdk-0.1.6/bubble/tools/benchmark/
+-rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/tools/benchmark/__init__.py
+-rw-rw-rw-   0        0        0     6098 2023-05-25 08:17:34.000000 bubble-sdk-0.1.6/bubble/tools/benchmark/main.py
+-rw-rw-rw-   0        0        0     3542 2023-05-23 08:08:26.000000 bubble-sdk-0.1.6/bubble/tools/benchmark/node.py
+-rw-rw-rw-   0        0        0      951 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/tools/benchmark/reporting.py
+-rw-rw-rw-   0        0        0     1791 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/tools/benchmark/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.408275 bubble-sdk-0.1.6/bubble/tools/pytest_bubble/
+-rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/tools/pytest_bubble/__init__.py
+-rw-rw-rw-   0        0        0     4307 2023-05-23 08:08:28.000000 bubble-sdk-0.1.6/bubble/tools/pytest_bubble/_utils.py
+-rw-rw-rw-   0        0        0     1471 2023-05-23 08:08:26.000000 bubble-sdk-0.1.6/bubble/tools/pytest_bubble/deployer.py
+-rw-rw-rw-   0        0        0      402 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/tools/pytest_bubble/exceptions.py
+-rw-rw-rw-   0        0        0     4053 2023-05-23 08:08:31.000000 bubble-sdk-0.1.6/bubble/tools/pytest_bubble/linker.py
+-rw-rw-rw-   0        0        0      680 2023-05-23 08:08:26.000000 bubble-sdk-0.1.6/bubble/tools/pytest_bubble/plugins.py
+-rw-rw-rw-   0        0        0     3302 2023-05-25 08:43:00.000000 bubble-sdk-0.1.6/bubble/tracing.py
+-rw-rw-rw-   0        0        0    13659 2023-05-24 07:08:55.000000 bubble-sdk-0.1.6/bubble/types.py
+drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.408275 bubble-sdk-0.1.6/bubble/utils/
+-rw-rw-rw-   0        0        0      472 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/utils/__init__.py
+-rw-rw-rw-   0        0        0      521 2023-05-23 08:08:21.000000 bubble-sdk-0.1.6/bubble/utils/abi.py
+-rw-rw-rw-   0        0        0     1008 2023-05-23 08:08:21.000000 bubble-sdk-0.1.6/bubble/utils/address.py
+-rw-rw-rw-   0        0        0     3199 2023-05-23 08:08:27.000000 bubble-sdk-0.1.6/bubble/utils/async_exception_handling.py
+-rw-rw-rw-   0        0        0     1569 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/bubble/utils/caching.py
+-rw-rw-rw-   0        0        0     3157 2023-05-23 08:08:25.000000 bubble-sdk-0.1.6/bubble/utils/exception_handling.py
+drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.408275 bubble-sdk-0.1.6/bubble_sdk.egg-info/
+-rw-rw-rw-   0        0        0     2240 2023-05-31 10:59:11.000000 bubble-sdk-0.1.6/bubble_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6916 2023-05-31 10:59:11.000000 bubble-sdk-0.1.6/bubble_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-31 10:59:11.000000 bubble-sdk-0.1.6/bubble_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-05-31 10:59:11.000000 bubble-sdk-0.1.6/bubble_sdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-31 10:56:52.000000 bubble-sdk-0.1.6/bubble_sdk.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     1174 2023-05-31 10:59:11.000000 bubble-sdk-0.1.6/bubble_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-31 10:59:11.000000 bubble-sdk-0.1.6/bubble_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.424291 bubble-sdk-0.1.6/ens/
+-rw-rw-rw-   0        0        0      305 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/ens/__init__.py
+-rw-rw-rw-   0        0        0    24627 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/ens/abis.py
+-rw-rw-rw-   0        0        0    21480 2023-05-23 08:08:30.000000 bubble-sdk-0.1.6/ens/async_ens.py
+-rw-rw-rw-   0        0        0       46 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/ens/auto.py
+-rw-rw-rw-   0        0        0     3412 2023-05-23 08:08:26.000000 bubble-sdk-0.1.6/ens/base_ens.py
+-rw-rw-rw-   0        0        0      629 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/ens/constants.py
+-rw-rw-rw-   0        0        0   199146 2023-05-23 08:08:30.000000 bubble-sdk-0.1.6/ens/contract_data.py
+-rw-rw-rw-   0        0        0    20613 2023-05-23 08:08:28.000000 bubble-sdk-0.1.6/ens/ens.py
+-rw-rw-rw-   0        0        0     2511 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/ens/exceptions.py
+-rw-rw-rw-   0        0        0     9333 2023-05-23 08:08:27.000000 bubble-sdk-0.1.6/ens/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.424291 bubble-sdk-0.1.6/ethpm/
+-rw-rw-rw-   0        0        0      775 2023-05-22 03:42:55.000000 bubble-sdk-0.1.6/ethpm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.424291 bubble-sdk-0.1.6/ethpm/_utils/
+-rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/ethpm/_utils/__init__.py
+-rw-rw-rw-   0        0        0     2604 2023-05-22 03:42:55.000000 bubble-sdk-0.1.6/ethpm/_utils/backend.py
+-rw-rw-rw-   0        0        0     1521 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/ethpm/_utils/cache.py
+-rw-rw-rw-   0        0        0     2969 2023-05-23 08:08:29.000000 bubble-sdk-0.1.6/ethpm/_utils/chains.py
+-rw-rw-rw-   0        0        0     1065 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/ethpm/_utils/contract.py
+-rw-rw-rw-   0        0        0     5410 2023-05-23 08:08:21.000000 bubble-sdk-0.1.6/ethpm/_utils/deployments.py
+-rw-rw-rw-   0        0        0     2835 2023-05-23 08:08:28.000000 bubble-sdk-0.1.6/ethpm/_utils/ipfs.py
+drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.424291 bubble-sdk-0.1.6/ethpm/_utils/protobuf/
+-rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/ethpm/_utils/protobuf/__init__.py
+-rw-rw-rw-   0        0        0     1971 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/ethpm/_utils/protobuf/ipfs_file_pb2.py
+-rw-rw-rw-   0        0        0     1517 2023-05-22 02:41:29.000000 bubble-sdk-0.1.6/ethpm/_utils/registry.py
+drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.424291 bubble-sdk-0.1.6/ethpm/assets/
+-rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/ethpm/assets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.424291 bubble-sdk-0.1.6/ethpm/backends/
+-rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/ethpm/backends/__init__.py
+-rw-rw-rw-   0        0        0      999 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/ethpm/backends/base.py
+-rw-rw-rw-   0        0        0     3114 2023-05-22 03:42:55.000000 bubble-sdk-0.1.6/ethpm/backends/http.py
+-rw-rw-rw-   0        0        0     6772 2023-05-23 08:08:32.000000 bubble-sdk-0.1.6/ethpm/backends/ipfs.py
+-rw-rw-rw-   0        0        0     4332 2023-05-23 08:08:25.000000 bubble-sdk-0.1.6/ethpm/backends/registry.py
+-rw-rw-rw-   0        0        0      422 2023-05-22 03:42:55.000000 bubble-sdk-0.1.6/ethpm/constants.py
+-rw-rw-rw-   0        0        0     6448 2023-05-23 08:08:21.000000 bubble-sdk-0.1.6/ethpm/contract.py
+-rw-rw-rw-   0        0        0     1948 2023-05-22 03:42:55.000000 bubble-sdk-0.1.6/ethpm/dependencies.py
+-rw-rw-rw-   0        0        0     2218 2023-05-23 08:08:29.000000 bubble-sdk-0.1.6/ethpm/deployments.py
+-rw-rw-rw-   0        0        0     1262 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/ethpm/exceptions.py
+-rw-rw-rw-   0        0        0    14939 2023-05-23 08:08:20.000000 bubble-sdk-0.1.6/ethpm/package.py
+drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.439926 bubble-sdk-0.1.6/ethpm/tools/
+-rw-rw-rw-   0        0        0      107 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/ethpm/tools/__init__.py
+-rw-rw-rw-   0        0        0    27981 2023-05-23 08:08:21.000000 bubble-sdk-0.1.6/ethpm/tools/builder.py
+-rw-rw-rw-   0        0        0    10687 2023-05-23 08:08:28.000000 bubble-sdk-0.1.6/ethpm/tools/checker.py
+-rw-rw-rw-   0        0        0      494 2023-05-22 03:42:55.000000 bubble-sdk-0.1.6/ethpm/tools/get_manifest.py
+-rw-rw-rw-   0        0        0     4513 2023-05-23 08:08:26.000000 bubble-sdk-0.1.6/ethpm/uri.py
+drwxrwxrwx   0        0        0        0 2023-05-31 10:59:11.439926 bubble-sdk-0.1.6/ethpm/validation/
+-rw-rw-rw-   0        0        0        0 2023-05-22 01:54:51.000000 bubble-sdk-0.1.6/ethpm/validation/__init__.py
+-rw-rw-rw-   0        0        0     4862 2023-05-22 03:42:55.000000 bubble-sdk-0.1.6/ethpm/validation/manifest.py
+-rw-rw-rw-   0        0        0     1115 2023-05-23 08:08:31.000000 bubble-sdk-0.1.6/ethpm/validation/misc.py
+-rw-rw-rw-   0        0        0     2397 2023-05-22 03:42:55.000000 bubble-sdk-0.1.6/ethpm/validation/package.py
+-rw-rw-rw-   0        0        0     5038 2023-05-23 08:08:28.000000 bubble-sdk-0.1.6/ethpm/validation/uri.py
+-rw-rw-rw-   0        0        0       42 2023-05-31 10:59:11.439926 bubble-sdk-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     3300 2023-05-31 10:59:05.000000 bubble-sdk-0.1.6/setup.py
```

### Comparing `bubble-sdk-0.1.5/LICENSE` & `bubble-sdk-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/PKG-INFO` & `bubble-sdk-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bubble-sdk
-Version: 0.1.5
+Version: 0.1.6
 Summary: Bubble sdk
 Home-page: https://github.com/shinnng/bubble.py
 Author: Shing
 Author-email: Shinnng@outlook.com
 License: MIT
 Keywords: bubble
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `bubble-sdk-0.1.5/README.md` & `bubble-sdk-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/__init__.py` & `bubble-sdk-0.1.6/bubble/__init__.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/abi.py` & `bubble-sdk-0.1.6/bubble/_utils/abi.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/async_transactions.py` & `bubble-sdk-0.1.6/bubble/_utils/async_transactions.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/blocks.py` & `bubble-sdk-0.1.6/bubble/_utils/blocks.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/caching.py` & `bubble-sdk-0.1.6/bubble/_utils/caching.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/contract_sources/compile_contracts.py` & `bubble-sdk-0.1.6/bubble/_utils/contract_sources/compile_contracts.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/_custom_contract_data.py` & `bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/_custom_contract_data.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/address_reflector.py` & `bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/address_reflector.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/arrays_contract.py` & `bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/arrays_contract.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/bytes_contracts.py` & `bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/bytes_contracts.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/constructor_contracts.py` & `bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/constructor_contracts.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/contract_caller_tester.py` & `bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/contract_caller_tester.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/emitter_contract.py` & `bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/emitter_contract.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/event_contracts.py` & `bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/event_contracts.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/extended_resolver.py` & `bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/extended_resolver.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/fallback_function_contract.py` & `bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/fallback_function_contract.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/math_contract.py` & `bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/math_contract.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/offchain_lookup.py` & `bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/offchain_lookup.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/offchain_resolver.py` & `bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/offchain_resolver.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/payable_tester.py` & `bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/payable_tester.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/receive_function_contracts.py` & `bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/receive_function_contracts.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/reflector_contracts.py` & `bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/reflector_contracts.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/revert_contract.py` & `bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/revert_contract.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/simple_resolver.py` & `bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/simple_resolver.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/string_contract.py` & `bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/string_contract.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/contract_sources/contract_data/tuple_contracts.py` & `bubble-sdk-0.1.6/bubble/_utils/contract_sources/contract_data/tuple_contracts.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/contracts.py` & `bubble-sdk-0.1.6/bubble/_utils/contracts.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/datatypes.py` & `bubble-sdk-0.1.6/bubble/_utils/datatypes.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/decorators.py` & `bubble-sdk-0.1.6/bubble/_utils/decorators.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/encoding.py` & `bubble-sdk-0.1.6/bubble/_utils/encoding.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/ens.py` & `bubble-sdk-0.1.6/bubble/_utils/ens.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/events.py` & `bubble-sdk-0.1.6/bubble/_utils/events.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/fee_utils.py` & `bubble-sdk-0.1.6/bubble/_utils/fee_utils.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/filters.py` & `bubble-sdk-0.1.6/bubble/_utils/filters.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/formatters.py` & `bubble-sdk-0.1.6/bubble/_utils/formatters.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/math.py` & `bubble-sdk-0.1.6/bubble/_utils/math.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/method_formatters.py` & `bubble-sdk-0.1.6/bubble/_utils/method_formatters.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/module.py` & `bubble-sdk-0.1.6/bubble/_utils/module.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/module_testing/__init__.py` & `bubble-sdk-0.1.6/bubble/_utils/module_testing/__init__.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/module_testing/eth_module.py` & `bubble-sdk-0.1.6/bubble/_utils/module_testing/eth_module.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/module_testing/go_ethereum_admin_module.py` & `bubble-sdk-0.1.6/bubble/_utils/module_testing/go_ethereum_admin_module.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/module_testing/go_ethereum_personal_module.py` & `bubble-sdk-0.1.6/bubble/_utils/module_testing/go_ethereum_personal_module.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/module_testing/go_ethereum_txpool_module.py` & `bubble-sdk-0.1.6/bubble/_utils/module_testing/go_ethereum_txpool_module.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/module_testing/module_testing_utils.py` & `bubble-sdk-0.1.6/bubble/_utils/module_testing/module_testing_utils.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/module_testing/net_module.py` & `bubble-sdk-0.1.6/bubble/_utils/module_testing/net_module.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/module_testing/web3_module.py` & `bubble-sdk-0.1.6/bubble/_utils/module_testing/web3_module.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/normalizers.py` & `bubble-sdk-0.1.6/bubble/_utils/normalizers.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/request.py` & `bubble-sdk-0.1.6/bubble/_utils/request.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/rpc_abi.py` & `bubble-sdk-0.1.6/bubble/_utils/rpc_abi.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/threads.py` & `bubble-sdk-0.1.6/bubble/_utils/threads.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/transactions.py` & `bubble-sdk-0.1.6/bubble/_utils/transactions.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/type_conversion.py` & `bubble-sdk-0.1.6/bubble/_utils/type_conversion.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/utility_methods.py` & `bubble-sdk-0.1.6/bubble/_utils/utility_methods.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/validation.py` & `bubble-sdk-0.1.6/bubble/_utils/validation.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/_utils/windows.py` & `bubble-sdk-0.1.6/bubble/_utils/windows.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/beacon/api_endpoints.py` & `bubble-sdk-0.1.6/bubble/beacon/api_endpoints.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/beacon/async_beacon.py` & `bubble-sdk-0.1.6/bubble/beacon/async_beacon.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/beacon/main.py` & `bubble-sdk-0.1.6/bubble/beacon/main.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/bub/async_bub.py` & `bubble-sdk-0.1.6/bubble/bub/async_bub.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/bub/base_bub.py` & `bubble-sdk-0.1.6/bubble/bub/base_bub.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/bub/bub.py` & `bubble-sdk-0.1.6/bubble/bub/bub.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/contract/async_contract.py` & `bubble-sdk-0.1.6/bubble/contract/async_contract.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/contract/base_contract.py` & `bubble-sdk-0.1.6/bubble/contract/base_contract.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/contract/contract.py` & `bubble-sdk-0.1.6/bubble/contract/contract.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/contract/utils.py` & `bubble-sdk-0.1.6/bubble/contract/utils.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/datastructures.py` & `bubble-sdk-0.1.6/bubble/datastructures.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/debug.py` & `bubble-sdk-0.1.6/bubble/debug.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/exceptions.py` & `bubble-sdk-0.1.6/bubble/exceptions.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/gas_strategies/time_based.py` & `bubble-sdk-0.1.6/bubble/gas_strategies/time_based.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/inner_contract/delegate.py` & `bubble-sdk-0.1.6/bubble/inner_contract/delegate.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/inner_contract/error_code.py` & `bubble-sdk-0.1.6/bubble/inner_contract/error_code.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/inner_contract/formatters.py` & `bubble-sdk-0.1.6/bubble/inner_contract/formatters.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/inner_contract/inner_contract.py` & `bubble-sdk-0.1.6/bubble/inner_contract/inner_contract.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/inner_contract/proposal.py` & `bubble-sdk-0.1.6/bubble/inner_contract/proposal.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/inner_contract/restricting.py` & `bubble-sdk-0.1.6/bubble/inner_contract/restricting.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/inner_contract/reward.py` & `bubble-sdk-0.1.6/bubble/inner_contract/reward.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/inner_contract/slashing.py` & `bubble-sdk-0.1.6/bubble/inner_contract/slashing.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/inner_contract/staking.py` & `bubble-sdk-0.1.6/bubble/inner_contract/staking.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/main.py` & `bubble-sdk-0.1.6/bubble/main.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/manager.py` & `bubble-sdk-0.1.6/bubble/manager.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/method.py` & `bubble-sdk-0.1.6/bubble/method.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/middleware/__init__.py` & `bubble-sdk-0.1.6/bubble/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/middleware/async_cache.py` & `bubble-sdk-0.1.6/bubble/middleware/async_cache.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/middleware/attrdict.py` & `bubble-sdk-0.1.6/bubble/middleware/attrdict.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/middleware/bub_poa.py` & `bubble-sdk-0.1.6/bubble/middleware/bub_poa.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/middleware/buffered_gas_estimate.py` & `bubble-sdk-0.1.6/bubble/middleware/buffered_gas_estimate.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/middleware/cache.py` & `bubble-sdk-0.1.6/bubble/middleware/cache.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/middleware/exception_handling.py` & `bubble-sdk-0.1.6/bubble/middleware/exception_handling.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/middleware/exception_retry_request.py` & `bubble-sdk-0.1.6/bubble/middleware/exception_retry_request.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/middleware/filter.py` & `bubble-sdk-0.1.6/bubble/middleware/filter.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/middleware/fixture.py` & `bubble-sdk-0.1.6/bubble/middleware/fixture.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/middleware/formatting.py` & `bubble-sdk-0.1.6/bubble/middleware/formatting.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/middleware/gas_price_strategy.py` & `bubble-sdk-0.1.6/bubble/middleware/gas_price_strategy.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/middleware/names.py` & `bubble-sdk-0.1.6/bubble/middleware/names.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/middleware/signing.py` & `bubble-sdk-0.1.6/bubble/middleware/signing.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/middleware/simulate_unmined_transaction.py` & `bubble-sdk-0.1.6/bubble/middleware/simulate_unmined_transaction.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/middleware/stalecheck.py` & `bubble-sdk-0.1.6/bubble/middleware/stalecheck.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/middleware/validation.py` & `bubble-sdk-0.1.6/bubble/middleware/validation.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/module.py` & `bubble-sdk-0.1.6/bubble/module.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/net.py` & `bubble-sdk-0.1.6/bubble/net.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/node.py` & `bubble-sdk-0.1.6/bubble/node.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/pm.py` & `bubble-sdk-0.1.6/bubble/pm.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/providers/async_base.py` & `bubble-sdk-0.1.6/bubble/providers/async_base.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/providers/async_rpc.py` & `bubble-sdk-0.1.6/bubble/providers/async_rpc.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/providers/auto.py` & `bubble-sdk-0.1.6/bubble/providers/auto.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/providers/base.py` & `bubble-sdk-0.1.6/bubble/providers/base.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/providers/bub_tester/defaults.py` & `bubble-sdk-0.1.6/bubble/providers/bub_tester/defaults.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/providers/bub_tester/main.py` & `bubble-sdk-0.1.6/bubble/providers/bub_tester/main.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/providers/bub_tester/middleware.py` & `bubble-sdk-0.1.6/bubble/providers/bub_tester/middleware.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/providers/ipc.py` & `bubble-sdk-0.1.6/bubble/providers/ipc.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/providers/rpc.py` & `bubble-sdk-0.1.6/bubble/providers/rpc.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/providers/websocket.py` & `bubble-sdk-0.1.6/bubble/providers/websocket.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/scripts/release/test_package.py` & `bubble-sdk-0.1.6/bubble/scripts/release/test_package.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/tools/benchmark/main.py` & `bubble-sdk-0.1.6/bubble/tools/benchmark/main.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/tools/benchmark/node.py` & `bubble-sdk-0.1.6/bubble/tools/benchmark/node.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/tools/benchmark/reporting.py` & `bubble-sdk-0.1.6/bubble/tools/benchmark/reporting.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/tools/benchmark/utils.py` & `bubble-sdk-0.1.6/bubble/tools/benchmark/utils.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/tools/pytest_bubble/_utils.py` & `bubble-sdk-0.1.6/bubble/tools/pytest_bubble/_utils.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/tools/pytest_bubble/deployer.py` & `bubble-sdk-0.1.6/bubble/tools/pytest_bubble/deployer.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/tools/pytest_bubble/linker.py` & `bubble-sdk-0.1.6/bubble/tools/pytest_bubble/linker.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/tools/pytest_bubble/plugins.py` & `bubble-sdk-0.1.6/bubble/tools/pytest_bubble/plugins.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/tracing.py` & `bubble-sdk-0.1.6/bubble/tracing.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/types.py` & `bubble-sdk-0.1.6/bubble/types.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/utils/abi.py` & `bubble-sdk-0.1.6/bubble/utils/abi.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/utils/address.py` & `bubble-sdk-0.1.6/bubble/utils/address.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/utils/async_exception_handling.py` & `bubble-sdk-0.1.6/bubble/utils/async_exception_handling.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/utils/caching.py` & `bubble-sdk-0.1.6/bubble/utils/caching.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble/utils/exception_handling.py` & `bubble-sdk-0.1.6/bubble/utils/exception_handling.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble_sdk.egg-info/PKG-INFO` & `bubble-sdk-0.1.6/bubble_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bubble-sdk
-Version: 0.1.5
+Version: 0.1.6
 Summary: Bubble sdk
 Home-page: https://github.com/shinnng/bubble.py
 Author: Shing
 Author-email: Shinnng@outlook.com
 License: MIT
 Keywords: bubble
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `bubble-sdk-0.1.5/bubble_sdk.egg-info/SOURCES.txt` & `bubble-sdk-0.1.6/bubble_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/bubble_sdk.egg-info/requires.txt` & `bubble-sdk-0.1.6/bubble_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/ens/abis.py` & `bubble-sdk-0.1.6/ens/abis.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/ens/async_ens.py` & `bubble-sdk-0.1.6/ens/async_ens.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/ens/base_ens.py` & `bubble-sdk-0.1.6/ens/base_ens.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/ens/constants.py` & `bubble-sdk-0.1.6/ens/constants.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/ens/contract_data.py` & `bubble-sdk-0.1.6/ens/contract_data.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/ens/ens.py` & `bubble-sdk-0.1.6/ens/ens.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/ens/exceptions.py` & `bubble-sdk-0.1.6/ens/exceptions.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/ens/utils.py` & `bubble-sdk-0.1.6/ens/utils.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/ethpm/__init__.py` & `bubble-sdk-0.1.6/ethpm/__init__.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/ethpm/_utils/backend.py` & `bubble-sdk-0.1.6/ethpm/_utils/backend.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/ethpm/_utils/cache.py` & `bubble-sdk-0.1.6/ethpm/_utils/cache.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/ethpm/_utils/chains.py` & `bubble-sdk-0.1.6/ethpm/_utils/chains.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/ethpm/_utils/contract.py` & `bubble-sdk-0.1.6/ethpm/_utils/contract.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/ethpm/_utils/deployments.py` & `bubble-sdk-0.1.6/ethpm/_utils/deployments.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/ethpm/_utils/ipfs.py` & `bubble-sdk-0.1.6/ethpm/_utils/ipfs.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/ethpm/_utils/protobuf/ipfs_file_pb2.py` & `bubble-sdk-0.1.6/ethpm/_utils/protobuf/ipfs_file_pb2.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/ethpm/_utils/registry.py` & `bubble-sdk-0.1.6/ethpm/_utils/registry.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/ethpm/backends/base.py` & `bubble-sdk-0.1.6/ethpm/backends/base.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/ethpm/backends/http.py` & `bubble-sdk-0.1.6/ethpm/backends/http.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/ethpm/backends/ipfs.py` & `bubble-sdk-0.1.6/ethpm/backends/ipfs.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/ethpm/backends/registry.py` & `bubble-sdk-0.1.6/ethpm/backends/registry.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/ethpm/contract.py` & `bubble-sdk-0.1.6/ethpm/contract.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/ethpm/dependencies.py` & `bubble-sdk-0.1.6/ethpm/dependencies.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/ethpm/deployments.py` & `bubble-sdk-0.1.6/ethpm/deployments.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/ethpm/exceptions.py` & `bubble-sdk-0.1.6/ethpm/exceptions.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/ethpm/package.py` & `bubble-sdk-0.1.6/ethpm/package.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/ethpm/tools/builder.py` & `bubble-sdk-0.1.6/ethpm/tools/builder.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/ethpm/tools/checker.py` & `bubble-sdk-0.1.6/ethpm/tools/checker.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/ethpm/uri.py` & `bubble-sdk-0.1.6/ethpm/uri.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/ethpm/validation/manifest.py` & `bubble-sdk-0.1.6/ethpm/validation/manifest.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/ethpm/validation/misc.py` & `bubble-sdk-0.1.6/ethpm/validation/misc.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/ethpm/validation/package.py` & `bubble-sdk-0.1.6/ethpm/validation/package.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/ethpm/validation/uri.py` & `bubble-sdk-0.1.6/ethpm/validation/uri.py`

 * *Files identical despite different names*

### Comparing `bubble-sdk-0.1.5/setup.py` & `bubble-sdk-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 with open("./README.md") as readme:
     long_description = readme.read()
 
 setup(
     name="bubble-sdk",
     # *IMPORTANT*: Don't manually change the version here. Use the 'bumpversion' utility.
-    version="0.1.5",
+    version="0.1.6",
     description="""Bubble sdk""",
     long_description_content_type="text/markdown",
     long_description=long_description,
     author="Shing",
     author_email="Shinnng@outlook.com",
     url="https://github.com/shinnng/bubble.py",
     include_package_data=True,
```

