# Comparing `tmp/stellar-sdk-mini-8.2.0.post1.tar.gz` & `tmp/stellar-sdk-mini-8.2.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stellar-sdk-mini-8.2.0.post1.tar", last modified: Tue May 30 16:41:04 2023, max compression
+gzip compressed data, was "stellar-sdk-mini-8.2.0.post2.tar", last modified: Wed May 31 00:34:31 2023, max compression
```

## Comparing `stellar-sdk-mini-8.2.0.post1.tar` & `stellar-sdk-mini-8.2.0.post2.tar`

### file list

```diff
@@ -1,365 +1,365 @@
-drwxr-xr-x   0 overcat    (501) staff       (20)        0 2023-05-30 16:41:04.939311 stellar-sdk-mini-8.2.0.post1/
--rw-r--r--   0 overcat    (501) staff       (20)    11357 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/LICENSE
--rw-r--r--   0 overcat    (501) staff       (20)     7390 2023-05-30 16:41:04.939389 stellar-sdk-mini-8.2.0.post1/PKG-INFO
--rw-r--r--   0 overcat    (501) staff       (20)     6068 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/README.rst
--rw-r--r--   0 overcat    (501) staff       (20)      110 2023-05-30 16:41:04.939654 stellar-sdk-mini-8.2.0.post1/setup.cfg
--rw-r--r--   0 overcat    (501) staff       (20)     2013 2023-05-30 16:40:39.000000 stellar-sdk-mini-8.2.0.post1/setup.py
-drwxr-xr-x   0 overcat    (501) staff       (20)        0 2023-05-30 16:41:04.860343 stellar-sdk-mini-8.2.0.post1/stellar_sdk/
--rw-r--r--   0 overcat    (501) staff       (20)      812 2023-05-30 16:13:27.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/__init__.py
--rw-r--r--   0 overcat    (501) staff       (20)      864 2023-05-30 16:41:02.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/__version__.py
--rw-r--r--   0 overcat    (501) staff       (20)     3871 2023-05-30 16:22:04.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/account.py
--rw-r--r--   0 overcat    (501) staff       (20)     9194 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/asset.py
--rw-r--r--   0 overcat    (501) staff       (20)    13621 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/base_server.py
--rw-r--r--   0 overcat    (501) staff       (20)     5492 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/base_transaction_envelope.py
--rw-r--r--   0 overcat    (501) staff       (20)     1836 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/decorated_signature.py
--rw-r--r--   0 overcat    (501) staff       (20)     1722 2023-05-30 16:19:18.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/exceptions.py
--rw-r--r--   0 overcat    (501) staff       (20)     5226 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/fee_bump_transaction.py
--rw-r--r--   0 overcat    (501) staff       (20)     5562 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/fee_bump_transaction_envelope.py
--rw-r--r--   0 overcat    (501) staff       (20)     1998 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/helpers.py
--rw-r--r--   0 overcat    (501) staff       (20)    12080 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/keypair.py
--rw-r--r--   0 overcat    (501) staff       (20)     2298 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/ledger_bounds.py
--rw-r--r--   0 overcat    (501) staff       (20)     5997 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/liquidity_pool_asset.py
--rw-r--r--   0 overcat    (501) staff       (20)     2195 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/liquidity_pool_id.py
--rw-r--r--   0 overcat    (501) staff       (20)     8941 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/memo.py
--rw-r--r--   0 overcat    (501) staff       (20)     6110 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/muxed_account.py
--rw-r--r--   0 overcat    (501) staff       (20)     1742 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/network.py
-drwxr-xr-x   0 overcat    (501) staff       (20)        0 2023-05-30 16:41:04.865339 stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/
--rw-r--r--   0 overcat    (501) staff       (20)      845 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/__init__.py
--rw-r--r--   0 overcat    (501) staff       (20)     2087 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/account_merge.py
--rw-r--r--   0 overcat    (501) staff       (20)     6259 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/allow_trust.py
--rw-r--r--   0 overcat    (501) staff       (20)     2890 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/begin_sponsoring_future_reserves.py
--rw-r--r--   0 overcat    (501) staff       (20)     2163 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/bump_sequence.py
--rw-r--r--   0 overcat    (501) staff       (20)     3157 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/change_trust.py
--rw-r--r--   0 overcat    (501) staff       (20)     2529 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/claim_claimable_balance.py
--rw-r--r--   0 overcat    (501) staff       (20)     2679 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/clawback.py
--rw-r--r--   0 overcat    (501) staff       (20)     2510 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/clawback_claimable_balance.py
--rw-r--r--   0 overcat    (501) staff       (20)     3271 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/create_account.py
--rw-r--r--   0 overcat    (501) staff       (20)    16694 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/create_claimable_balance.py
--rw-r--r--   0 overcat    (501) staff       (20)     4357 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/create_passive_sell_offer.py
--rw-r--r--   0 overcat    (501) staff       (20)     1737 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/end_sponsoring_future_reserves.py
--rw-r--r--   0 overcat    (501) staff       (20)     1212 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/inflation.py
--rw-r--r--   0 overcat    (501) staff       (20)     4741 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/liquidity_pool_deposit.py
--rw-r--r--   0 overcat    (501) staff       (20)     4147 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/liquidity_pool_withdraw.py
--rw-r--r--   0 overcat    (501) staff       (20)     3881 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/manage_buy_offer.py
--rw-r--r--   0 overcat    (501) staff       (20)     3391 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/manage_data.py
--rw-r--r--   0 overcat    (501) staff       (20)     3892 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/manage_sell_offer.py
--rw-r--r--   0 overcat    (501) staff       (20)     4909 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/operation.py
--rw-r--r--   0 overcat    (501) staff       (20)     5001 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/path_payment_strict_receive.py
--rw-r--r--   0 overcat    (501) staff       (20)     4935 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/path_payment_strict_send.py
--rw-r--r--   0 overcat    (501) staff       (20)     2783 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/payment.py
--rw-r--r--   0 overcat    (501) staff       (20)    23692 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/revoke_sponsorship.py
--rw-r--r--   0 overcat    (501) staff       (20)    10477 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/set_options.py
--rw-r--r--   0 overcat    (501) staff       (20)     4633 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/set_trust_line_flags.py
--rw-r--r--   0 overcat    (501) staff       (20)     8384 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/preconditions.py
--rw-r--r--   0 overcat    (501) staff       (20)     2039 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/price.py
-drwxr-xr-x   0 overcat    (501) staff       (20)        0 2023-05-30 16:41:04.865587 stellar-sdk-mini-8.2.0.post1/stellar_sdk/sep/
--rw-r--r--   0 overcat    (501) staff       (20)        0 2023-05-30 16:21:00.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/sep/__init__.py
--rw-r--r--   0 overcat    (501) staff       (20)     3117 2023-05-30 16:21:45.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/sep/mnemonic.py
--rw-r--r--   0 overcat    (501) staff       (20)     4072 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/signer.py
--rw-r--r--   0 overcat    (501) staff       (20)    11183 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/signer_key.py
--rw-r--r--   0 overcat    (501) staff       (20)    12157 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/strkey.py
--rw-r--r--   0 overcat    (501) staff       (20)     2516 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/time_bounds.py
--rw-r--r--   0 overcat    (501) staff       (20)    10470 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/transaction.py
--rw-r--r--   0 overcat    (501) staff       (20)    55381 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/transaction_builder.py
--rw-r--r--   0 overcat    (501) staff       (20)     7136 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/transaction_envelope.py
--rw-r--r--   0 overcat    (501) staff       (20)     5850 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/utils.py
-drwxr-xr-x   0 overcat    (501) staff       (20)        0 2023-05-30 16:41:04.938596 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/
--rw-r--r--   0 overcat    (501) staff       (20)    15456 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/__init__.py
--rw-r--r--   0 overcat    (501) staff       (20)     5998 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/account_entry.py
--rw-r--r--   0 overcat    (501) staff       (20)     2173 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/account_entry_ext.py
--rw-r--r--   0 overcat    (501) staff       (20)     2199 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/account_entry_extension_v1.py
--rw-r--r--   0 overcat    (501) staff       (20)     2239 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/account_entry_extension_v1_ext.py
--rw-r--r--   0 overcat    (501) staff       (20)     3775 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/account_entry_extension_v2.py
--rw-r--r--   0 overcat    (501) staff       (20)     2239 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/account_entry_extension_v2_ext.py
--rw-r--r--   0 overcat    (501) staff       (20)     2600 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/account_entry_extension_v3.py
--rw-r--r--   0 overcat    (501) staff       (20)     1975 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/account_flags.py
--rw-r--r--   0 overcat    (501) staff       (20)     1435 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/account_id.py
--rw-r--r--   0 overcat    (501) staff       (20)     2643 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/account_merge_result.py
--rw-r--r--   0 overcat    (501) staff       (20)     2246 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/account_merge_result_code.py
--rw-r--r--   0 overcat    (501) staff       (20)     2307 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/allow_trust_op.py
--rw-r--r--   0 overcat    (501) staff       (20)     1865 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/allow_trust_result.py
--rw-r--r--   0 overcat    (501) staff       (20)     2154 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/allow_trust_result_code.py
--rw-r--r--   0 overcat    (501) staff       (20)     1903 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/alpha_num12.py
--rw-r--r--   0 overcat    (501) staff       (20)     1891 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/alpha_num4.py
--rw-r--r--   0 overcat    (501) staff       (20)     3284 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/asset.py
--rw-r--r--   0 overcat    (501) staff       (20)     3133 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/asset_code.py
--rw-r--r--   0 overcat    (501) staff       (20)     1482 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/asset_code12.py
--rw-r--r--   0 overcat    (501) staff       (20)     1462 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/asset_code4.py
--rw-r--r--   0 overcat    (501) staff       (20)     1368 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/asset_type.py
--rw-r--r--   0 overcat    (501) staff       (20)     1586 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/auth.py
--rw-r--r--   0 overcat    (501) staff       (20)     2203 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/auth_cert.py
--rw-r--r--   0 overcat    (501) staff       (20)     2188 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/authenticated_message.py
--rw-r--r--   0 overcat    (501) staff       (20)     2297 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/authenticated_message_v0.py
--rw-r--r--   0 overcat    (501) staff       (20)     6074 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/base.py
--rw-r--r--   0 overcat    (501) staff       (20)     1771 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/begin_sponsoring_future_reserves_op.py
--rw-r--r--   0 overcat    (501) staff       (20)     2290 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/begin_sponsoring_future_reserves_result.py
--rw-r--r--   0 overcat    (501) staff       (20)     1843 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/begin_sponsoring_future_reserves_result_code.py
--rw-r--r--   0 overcat    (501) staff       (20)     4114 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/bucket_entry.py
--rw-r--r--   0 overcat    (501) staff       (20)     1529 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/bucket_entry_type.py
--rw-r--r--   0 overcat    (501) staff       (20)     2165 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/bucket_metadata.py
--rw-r--r--   0 overcat    (501) staff       (20)     1620 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/bucket_metadata_ext.py
--rw-r--r--   0 overcat    (501) staff       (20)     1617 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/bump_sequence_op.py
--rw-r--r--   0 overcat    (501) staff       (20)     1899 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/bump_sequence_result.py
--rw-r--r--   0 overcat    (501) staff       (20)     1451 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/bump_sequence_result_code.py
--rw-r--r--   0 overcat    (501) staff       (20)     4223 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/change_trust_asset.py
--rw-r--r--   0 overcat    (501) staff       (20)     1907 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/change_trust_op.py
--rw-r--r--   0 overcat    (501) staff       (20)     1882 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/change_trust_result.py
--rw-r--r--   0 overcat    (501) staff       (20)     2395 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/change_trust_result_code.py
--rw-r--r--   0 overcat    (501) staff       (20)     3812 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/claim_atom.py
--rw-r--r--   0 overcat    (501) staff       (20)     1327 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/claim_atom_type.py
--rw-r--r--   0 overcat    (501) staff       (20)     1737 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/claim_claimable_balance_op.py
--rw-r--r--   0 overcat    (501) staff       (20)     2056 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/claim_claimable_balance_result.py
--rw-r--r--   0 overcat    (501) staff       (20)     1795 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/claim_claimable_balance_result_code.py
--rw-r--r--   0 overcat    (501) staff       (20)     3197 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/claim_liquidity_atom.py
--rw-r--r--   0 overcat    (501) staff       (20)     3449 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/claim_offer_atom.py
--rw-r--r--   0 overcat    (501) staff       (20)     3512 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/claim_offer_atom_v0.py
--rw-r--r--   0 overcat    (501) staff       (20)     7156 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/claim_predicate.py
--rw-r--r--   0 overcat    (501) staff       (20)     1604 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/claim_predicate_type.py
--rw-r--r--   0 overcat    (501) staff       (20)     3858 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/claimable_balance_entry.py
--rw-r--r--   0 overcat    (501) staff       (20)     2273 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/claimable_balance_entry_ext.py
--rw-r--r--   0 overcat    (501) staff       (20)     2176 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/claimable_balance_entry_extension_v1.py
--rw-r--r--   0 overcat    (501) staff       (20)     1728 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/claimable_balance_entry_extension_v1_ext.py
--rw-r--r--   0 overcat    (501) staff       (20)     1388 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/claimable_balance_flags.py
--rw-r--r--   0 overcat    (501) staff       (20)     2220 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/claimable_balance_id.py
--rw-r--r--   0 overcat    (501) staff       (20)     1235 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/claimable_balance_id_type.py
--rw-r--r--   0 overcat    (501) staff       (20)     2258 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/claimant.py
--rw-r--r--   0 overcat    (501) staff       (20)     1151 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/claimant_type.py
--rw-r--r--   0 overcat    (501) staff       (20)     2075 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/claimant_v0.py
--rw-r--r--   0 overcat    (501) staff       (20)     1758 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/clawback_claimable_balance_op.py
--rw-r--r--   0 overcat    (501) staff       (20)     2192 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/clawback_claimable_balance_result.py
--rw-r--r--   0 overcat    (501) staff       (20)     1783 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/clawback_claimable_balance_result_code.py
--rw-r--r--   0 overcat    (501) staff       (20)     2136 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/clawback_op.py
--rw-r--r--   0 overcat    (501) staff       (20)     1827 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/clawback_result.py
--rw-r--r--   0 overcat    (501) staff       (20)     1598 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/clawback_result_code.py
--rw-r--r--   0 overcat    (501) staff       (20)      847 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/constants.py
--rw-r--r--   0 overcat    (501) staff       (20)     2123 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/create_account_op.py
--rw-r--r--   0 overcat    (501) staff       (20)     1916 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/create_account_result.py
--rw-r--r--   0 overcat    (501) staff       (20)     1857 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/create_account_result_code.py
--rw-r--r--   0 overcat    (501) staff       (20)     2745 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/create_claimable_balance_op.py
--rw-r--r--   0 overcat    (501) staff       (20)     2670 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/create_claimable_balance_result.py
--rw-r--r--   0 overcat    (501) staff       (20)     1804 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/create_claimable_balance_result_code.py
--rw-r--r--   0 overcat    (501) staff       (20)     2543 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/create_passive_sell_offer_op.py
--rw-r--r--   0 overcat    (501) staff       (20)     1578 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/crypto_key_type.py
--rw-r--r--   0 overcat    (501) staff       (20)     1572 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/curve25519_public.py
--rw-r--r--   0 overcat    (501) staff       (20)     1572 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/curve25519_secret.py
--rw-r--r--   0 overcat    (501) staff       (20)     2750 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/data_entry.py
--rw-r--r--   0 overcat    (501) staff       (20)     1590 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/data_entry_ext.py
--rw-r--r--   0 overcat    (501) staff       (20)     1450 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/data_value.py
--rw-r--r--   0 overcat    (501) staff       (20)     2004 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/decorated_signature.py
--rw-r--r--   0 overcat    (501) staff       (20)     1830 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/dont_have.py
--rw-r--r--   0 overcat    (501) staff       (20)     1392 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/duration.py
--rw-r--r--   0 overcat    (501) staff       (20)     1527 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/encrypted_body.py
--rw-r--r--   0 overcat    (501) staff       (20)     2256 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/end_sponsoring_future_reserves_result.py
--rw-r--r--   0 overcat    (501) staff       (20)     1589 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/end_sponsoring_future_reserves_result_code.py
--rw-r--r--   0 overcat    (501) staff       (20)     1642 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/envelope_type.py
--rw-r--r--   0 overcat    (501) staff       (20)     1750 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/error.py
--rw-r--r--   0 overcat    (501) staff       (20)     1401 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/error_code.py
--rw-r--r--   0 overcat    (501) staff       (20)     1595 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/extension_point.py
--rw-r--r--   0 overcat    (501) staff       (20)     2890 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/fee_bump_transaction.py
--rw-r--r--   0 overcat    (501) staff       (20)     2668 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/fee_bump_transaction_envelope.py
--rw-r--r--   0 overcat    (501) staff       (20)     1644 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/fee_bump_transaction_ext.py
--rw-r--r--   0 overcat    (501) staff       (20)     2237 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/fee_bump_transaction_inner_tx.py
--rw-r--r--   0 overcat    (501) staff       (20)     1353 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/hash.py
--rw-r--r--   0 overcat    (501) staff       (20)     3538 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/hash_id_preimage.py
--rw-r--r--   0 overcat    (501) staff       (20)     2399 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/hash_id_preimage_operation_id.py
--rw-r--r--   0 overcat    (501) staff       (20)     3081 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/hash_id_preimage_revoke_id.py
--rw-r--r--   0 overcat    (501) staff       (20)     4324 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/hello.py
--rw-r--r--   0 overcat    (501) staff       (20)     1551 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/hmac_sha256_key.py
--rw-r--r--   0 overcat    (501) staff       (20)     1551 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/hmac_sha256_mac.py
--rw-r--r--   0 overcat    (501) staff       (20)     1964 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/inflation_payout.py
--rw-r--r--   0 overcat    (501) staff       (20)     2804 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/inflation_result.py
--rw-r--r--   0 overcat    (501) staff       (20)     1386 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/inflation_result_code.py
--rw-r--r--   0 overcat    (501) staff       (20)     3356 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/inner_transaction_result.py
--rw-r--r--   0 overcat    (501) staff       (20)     1668 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/inner_transaction_result_ext.py
--rw-r--r--   0 overcat    (501) staff       (20)     2231 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/inner_transaction_result_pair.py
--rw-r--r--   0 overcat    (501) staff       (20)     6296 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/inner_transaction_result_result.py
--rw-r--r--   0 overcat    (501) staff       (20)     1344 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/int32.py
--rw-r--r--   0 overcat    (501) staff       (20)     1340 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/int64.py
--rw-r--r--   0 overcat    (501) staff       (20)     1150 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ip_addr_type.py
--rw-r--r--   0 overcat    (501) staff       (20)     1948 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_bounds.py
--rw-r--r--   0 overcat    (501) staff       (20)     2012 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_close_meta.py
--rw-r--r--   0 overcat    (501) staff       (20)     5280 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_close_meta_v0.py
--rw-r--r--   0 overcat    (501) staff       (20)     2045 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_close_value_signature.py
--rw-r--r--   0 overcat    (501) staff       (20)     3105 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_entry.py
--rw-r--r--   0 overcat    (501) staff       (20)     4292 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_entry_change.py
--rw-r--r--   0 overcat    (501) staff       (20)     1541 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_entry_change_type.py
--rw-r--r--   0 overcat    (501) staff       (20)     2241 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_entry_changes.py
--rw-r--r--   0 overcat    (501) staff       (20)     5915 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_entry_data.py
--rw-r--r--   0 overcat    (501) staff       (20)     2162 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_entry_ext.py
--rw-r--r--   0 overcat    (501) staff       (20)     2198 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_entry_extension_v1.py
--rw-r--r--   0 overcat    (501) staff       (20)     1668 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_entry_extension_v1_ext.py
--rw-r--r--   0 overcat    (501) staff       (20)     1384 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_entry_type.py
--rw-r--r--   0 overcat    (501) staff       (20)     7964 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_header.py
--rw-r--r--   0 overcat    (501) staff       (20)     2173 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_header_ext.py
--rw-r--r--   0 overcat    (501) staff       (20)     2059 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_header_extension_v1.py
--rw-r--r--   0 overcat    (501) staff       (20)     1674 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_header_extension_v1_ext.py
--rw-r--r--   0 overcat    (501) staff       (20)     1425 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_header_flags.py
--rw-r--r--   0 overcat    (501) staff       (20)     2422 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_header_history_entry.py
--rw-r--r--   0 overcat    (501) staff       (20)     1680 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_header_history_entry_ext.py
--rw-r--r--   0 overcat    (501) staff       (20)     6398 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_key.py
--rw-r--r--   0 overcat    (501) staff       (20)     1636 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_key_account.py
--rw-r--r--   0 overcat    (501) staff       (20)     1736 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_key_claimable_balance.py
--rw-r--r--   0 overcat    (501) staff       (20)     1944 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_key_data.py
--rw-r--r--   0 overcat    (501) staff       (20)     1740 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_key_liquidity_pool.py
--rw-r--r--   0 overcat    (501) staff       (20)     1911 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_key_offer.py
--rw-r--r--   0 overcat    (501) staff       (20)     1959 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_key_trust_line.py
--rw-r--r--   0 overcat    (501) staff       (20)     2442 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_scp_messages.py
--rw-r--r--   0 overcat    (501) staff       (20)     5635 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_upgrade.py
--rw-r--r--   0 overcat    (501) staff       (20)     1501 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_upgrade_type.py
--rw-r--r--   0 overcat    (501) staff       (20)     1798 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/liabilities.py
--rw-r--r--   0 overcat    (501) staff       (20)     2363 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/liquidity_pool_constant_product_parameters.py
--rw-r--r--   0 overcat    (501) staff       (20)     3239 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/liquidity_pool_deposit_op.py
--rw-r--r--   0 overcat    (501) staff       (20)     2052 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/liquidity_pool_deposit_result.py
--rw-r--r--   0 overcat    (501) staff       (20)     2592 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/liquidity_pool_deposit_result_code.py
--rw-r--r--   0 overcat    (501) staff       (20)     2675 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/liquidity_pool_entry.py
--rw-r--r--   0 overcat    (501) staff       (20)     3023 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/liquidity_pool_entry_body.py
--rw-r--r--   0 overcat    (501) staff       (20)     3600 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/liquidity_pool_entry_constant_product.py
--rw-r--r--   0 overcat    (501) staff       (20)     2666 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/liquidity_pool_parameters.py
--rw-r--r--   0 overcat    (501) staff       (20)     1211 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/liquidity_pool_type.py
--rw-r--r--   0 overcat    (501) staff       (20)     2869 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/liquidity_pool_withdraw_op.py
--rw-r--r--   0 overcat    (501) staff       (20)     2069 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/liquidity_pool_withdraw_result.py
--rw-r--r--   0 overcat    (501) staff       (20)     2272 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/liquidity_pool_withdraw_result_code.py
--rw-r--r--   0 overcat    (501) staff       (20)     2979 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/manage_buy_offer_op.py
--rw-r--r--   0 overcat    (501) staff       (20)     2450 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/manage_buy_offer_result.py
--rw-r--r--   0 overcat    (501) staff       (20)     2928 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/manage_buy_offer_result_code.py
--rw-r--r--   0 overcat    (501) staff       (20)     2153 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/manage_data_op.py
--rw-r--r--   0 overcat    (501) staff       (20)     1865 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/manage_data_result.py
--rw-r--r--   0 overcat    (501) staff       (20)     1863 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/manage_data_result_code.py
--rw-r--r--   0 overcat    (501) staff       (20)     1323 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/manage_offer_effect.py
--rw-r--r--   0 overcat    (501) staff       (20)     2931 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/manage_offer_success_result.py
--rw-r--r--   0 overcat    (501) staff       (20)     2790 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/manage_offer_success_result_offer.py
--rw-r--r--   0 overcat    (501) staff       (20)     2899 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/manage_sell_offer_op.py
--rw-r--r--   0 overcat    (501) staff       (20)     2467 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/manage_sell_offer_result.py
--rw-r--r--   0 overcat    (501) staff       (20)     3030 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/manage_sell_offer_result_code.py
--rw-r--r--   0 overcat    (501) staff       (20)     4005 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/memo.py
--rw-r--r--   0 overcat    (501) staff       (20)     1293 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/memo_type.py
--rw-r--r--   0 overcat    (501) staff       (20)     2023 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/message_type.py
--rw-r--r--   0 overcat    (501) staff       (20)     3024 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/muxed_account.py
--rw-r--r--   0 overcat    (501) staff       (20)     1847 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/muxed_account_med25519.py
--rw-r--r--   0 overcat    (501) staff       (20)     1384 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/node_id.py
--rw-r--r--   0 overcat    (501) staff       (20)     3951 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/offer_entry.py
--rw-r--r--   0 overcat    (501) staff       (20)     1596 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/offer_entry_ext.py
--rw-r--r--   0 overcat    (501) staff       (20)     1256 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/offer_entry_flags.py
--rw-r--r--   0 overcat    (501) staff       (20)     4571 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/operation.py
--rw-r--r--   0 overcat    (501) staff       (20)    23123 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/operation_body.py
--rw-r--r--   0 overcat    (501) staff       (20)     1632 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/operation_meta.py
--rw-r--r--   0 overcat    (501) staff       (20)     4688 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/operation_result.py
--rw-r--r--   0 overcat    (501) staff       (20)     1842 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/operation_result_code.py
--rw-r--r--   0 overcat    (501) staff       (20)    27203 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/operation_result_tr.py
--rw-r--r--   0 overcat    (501) staff       (20)     2646 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/operation_type.py
--rw-r--r--   0 overcat    (501) staff       (20)     4041 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/path_payment_strict_receive_op.py
--rw-r--r--   0 overcat    (501) staff       (20)     3795 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/path_payment_strict_receive_result.py
--rw-r--r--   0 overcat    (501) staff       (20)     3327 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/path_payment_strict_receive_result_code.py
--rw-r--r--   0 overcat    (501) staff       (20)     2505 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/path_payment_strict_receive_result_success.py
--rw-r--r--   0 overcat    (501) staff       (20)     4054 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/path_payment_strict_send_op.py
--rw-r--r--   0 overcat    (501) staff       (20)     3623 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/path_payment_strict_send_result.py
--rw-r--r--   0 overcat    (501) staff       (20)     3217 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/path_payment_strict_send_result_code.py
--rw-r--r--   0 overcat    (501) staff       (20)     2487 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/path_payment_strict_send_result_success.py
--rw-r--r--   0 overcat    (501) staff       (20)     2306 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/payment_op.py
--rw-r--r--   0 overcat    (501) staff       (20)     1810 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/payment_result.py
--rw-r--r--   0 overcat    (501) staff       (20)     2316 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/payment_result_code.py
--rw-r--r--   0 overcat    (501) staff       (20)     2323 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/peer_address.py
--rw-r--r--   0 overcat    (501) staff       (20)     2697 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/peer_address_ip.py
--rw-r--r--   0 overcat    (501) staff       (20)     2020 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/peer_stat_list.py
--rw-r--r--   0 overcat    (501) staff       (20)     7616 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/peer_stats.py
--rw-r--r--   0 overcat    (501) staff       (20)     1358 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/pool_id.py
--rw-r--r--   0 overcat    (501) staff       (20)     1257 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/precondition_type.py
--rw-r--r--   0 overcat    (501) staff       (20)     3135 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/preconditions.py
--rw-r--r--   0 overcat    (501) staff       (20)     5895 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/preconditions_v2.py
--rw-r--r--   0 overcat    (501) staff       (20)     1652 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/price.py
--rw-r--r--   0 overcat    (501) staff       (20)     2168 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/public_key.py
--rw-r--r--   0 overcat    (501) staff       (20)     1186 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/public_key_type.py
--rw-r--r--   0 overcat    (501) staff       (20)     3281 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/revoke_sponsorship_op.py
--rw-r--r--   0 overcat    (501) staff       (20)     2058 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/revoke_sponsorship_op_signer.py
--rw-r--r--   0 overcat    (501) staff       (20)     1984 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/revoke_sponsorship_result.py
--rw-r--r--   0 overcat    (501) staff       (20)     1847 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/revoke_sponsorship_result_code.py
--rw-r--r--   0 overcat    (501) staff       (20)     1312 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/revoke_sponsorship_type.py
--rw-r--r--   0 overcat    (501) staff       (20)     1815 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/scp_ballot.py
--rw-r--r--   0 overcat    (501) staff       (20)     1939 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/scp_envelope.py
--rw-r--r--   0 overcat    (501) staff       (20)     2012 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/scp_history_entry.py
--rw-r--r--   0 overcat    (501) staff       (20)     2709 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/scp_history_entry_v0.py
--rw-r--r--   0 overcat    (501) staff       (20)     3171 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/scp_nomination.py
--rw-r--r--   0 overcat    (501) staff       (20)     3250 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/scp_quorum_set.py
--rw-r--r--   0 overcat    (501) staff       (20)     3468 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/scp_statement.py
--rw-r--r--   0 overcat    (501) staff       (20)     2954 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/scp_statement_confirm.py
--rw-r--r--   0 overcat    (501) staff       (20)     2467 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/scp_statement_externalize.py
--rw-r--r--   0 overcat    (501) staff       (20)     5360 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/scp_statement_pledges.py
--rw-r--r--   0 overcat    (501) staff       (20)     3650 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/scp_statement_prepare.py
--rw-r--r--   0 overcat    (501) staff       (20)     1346 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/scp_statement_type.py
--rw-r--r--   0 overcat    (501) staff       (20)     1594 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/send_more.py
--rw-r--r--   0 overcat    (501) staff       (20)     1499 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/sequence_number.py
--rw-r--r--   0 overcat    (501) staff       (20)     6199 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/set_options_op.py
--rw-r--r--   0 overcat    (501) staff       (20)     1865 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/set_options_result.py
--rw-r--r--   0 overcat    (501) staff       (20)     2584 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/set_options_result_code.py
--rw-r--r--   0 overcat    (501) staff       (20)     2618 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/set_trust_line_flags_op.py
--rw-r--r--   0 overcat    (501) staff       (20)     1992 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/set_trust_line_flags_result.py
--rw-r--r--   0 overcat    (501) staff       (20)     1983 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/set_trust_line_flags_result_code.py
--rw-r--r--   0 overcat    (501) staff       (20)     1440 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/signature.py
--rw-r--r--   0 overcat    (501) staff       (20)     1513 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/signature_hint.py
--rw-r--r--   0 overcat    (501) staff       (20)     2192 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/signed_survey_request_message.py
--rw-r--r--   0 overcat    (501) staff       (20)     2228 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/signed_survey_response_message.py
--rw-r--r--   0 overcat    (501) staff       (20)     1793 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/signer.py
--rw-r--r--   0 overcat    (501) staff       (20)     4930 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/signer_key.py
--rw-r--r--   0 overcat    (501) staff       (20)     2100 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/signer_key_ed25519_signed_payload.py
--rw-r--r--   0 overcat    (501) staff       (20)     1504 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/signer_key_type.py
--rw-r--r--   0 overcat    (501) staff       (20)     2256 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/simple_payment_result.py
--rw-r--r--   0 overcat    (501) staff       (20)     1868 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/sponsorship_descriptor.py
--rw-r--r--   0 overcat    (501) staff       (20)    13256 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/stellar_message.py
--rw-r--r--   0 overcat    (501) staff       (20)     3780 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/stellar_value.py
--rw-r--r--   0 overcat    (501) staff       (20)     2671 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/stellar_value_ext.py
--rw-r--r--   0 overcat    (501) staff       (20)     1248 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/stellar_value_type.py
--rw-r--r--   0 overcat    (501) staff       (20)     1405 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/string32.py
--rw-r--r--   0 overcat    (501) staff       (20)     1405 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/string64.py
--rw-r--r--   0 overcat    (501) staff       (20)     1221 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/survey_message_command_type.py
--rw-r--r--   0 overcat    (501) staff       (20)     3354 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/survey_request_message.py
--rw-r--r--   0 overcat    (501) staff       (20)     2633 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/survey_response_body.py
--rw-r--r--   0 overcat    (501) staff       (20)     3346 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/survey_response_message.py
--rw-r--r--   0 overcat    (501) staff       (20)     1350 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/threshold_indexes.py
--rw-r--r--   0 overcat    (501) staff       (20)     1452 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/thresholds.py
--rw-r--r--   0 overcat    (501) staff       (20)     1885 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/time_bounds.py
--rw-r--r--   0 overcat    (501) staff       (20)     1419 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/time_point.py
--rw-r--r--   0 overcat    (501) staff       (20)     3111 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/topology_response_body.py
--rw-r--r--   0 overcat    (501) staff       (20)     4356 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction.py
--rw-r--r--   0 overcat    (501) staff       (20)     3675 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_envelope.py
--rw-r--r--   0 overcat    (501) staff       (20)     1602 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_ext.py
--rw-r--r--   0 overcat    (501) staff       (20)     2500 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_history_entry.py
--rw-r--r--   0 overcat    (501) staff       (20)     1674 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_history_entry_ext.py
--rw-r--r--   0 overcat    (501) staff       (20)     2681 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_history_result_entry.py
--rw-r--r--   0 overcat    (501) staff       (20)     1710 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_history_result_entry_ext.py
--rw-r--r--   0 overcat    (501) staff       (20)     3762 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_meta.py
--rw-r--r--   0 overcat    (501) staff       (20)     2634 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_meta_v1.py
--rw-r--r--   0 overcat    (501) staff       (20)     3340 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_meta_v2.py
--rw-r--r--   0 overcat    (501) staff       (20)     2874 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_result.py
--rw-r--r--   0 overcat    (501) staff       (20)     2894 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_result_code.py
--rw-r--r--   0 overcat    (501) staff       (20)     1638 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_result_ext.py
--rw-r--r--   0 overcat    (501) staff       (20)     2650 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_result_meta.py
--rw-r--r--   0 overcat    (501) staff       (20)     2122 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_result_pair.py
--rw-r--r--   0 overcat    (501) staff       (20)     4972 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_result_result.py
--rw-r--r--   0 overcat    (501) staff       (20)     2170 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_result_set.py
--rw-r--r--   0 overcat    (501) staff       (20)     2506 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_set.py
--rw-r--r--   0 overcat    (501) staff       (20)     2646 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_signature_payload.py
--rw-r--r--   0 overcat    (501) staff       (20)     3202 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_signature_payload_tagged_transaction.py
--rw-r--r--   0 overcat    (501) staff       (20)     4455 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_v0.py
--rw-r--r--   0 overcat    (501) staff       (20)     2607 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_v0_envelope.py
--rw-r--r--   0 overcat    (501) staff       (20)     1614 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_v0_ext.py
--rw-r--r--   0 overcat    (501) staff       (20)     2596 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_v1_envelope.py
--rw-r--r--   0 overcat    (501) staff       (20)     4167 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/trust_line_asset.py
--rw-r--r--   0 overcat    (501) staff       (20)     3848 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/trust_line_entry.py
--rw-r--r--   0 overcat    (501) staff       (20)     2472 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/trust_line_entry_ext.py
--rw-r--r--   0 overcat    (501) staff       (20)     2317 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/trust_line_entry_extension_v2.py
--rw-r--r--   0 overcat    (501) staff       (20)     1686 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/trust_line_entry_extension_v2_ext.py
--rw-r--r--   0 overcat    (501) staff       (20)     2194 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/trust_line_entry_v1.py
--rw-r--r--   0 overcat    (501) staff       (20)     2256 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/trust_line_entry_v1_ext.py
--rw-r--r--   0 overcat    (501) staff       (20)     1710 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/trust_line_flags.py
--rw-r--r--   0 overcat    (501) staff       (20)     1404 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/uint256.py
--rw-r--r--   0 overcat    (501) staff       (20)     1394 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/uint32.py
--rw-r--r--   0 overcat    (501) staff       (20)     1390 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/uint64.py
--rw-r--r--   0 overcat    (501) staff       (20)     1978 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/upgrade_entry_meta.py
--rw-r--r--   0 overcat    (501) staff       (20)     1487 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/upgrade_type.py
--rw-r--r--   0 overcat    (501) staff       (20)     1386 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/value.py
-drwxr-xr-x   0 overcat    (501) staff       (20)        0 2023-05-30 16:41:04.939194 stellar-sdk-mini-8.2.0.post1/stellar_sdk_mini.egg-info/
--rw-r--r--   0 overcat    (501) staff       (20)     7390 2023-05-30 16:41:04.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk_mini.egg-info/PKG-INFO
--rw-r--r--   0 overcat    (501) staff       (20)    13853 2023-05-30 16:41:04.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk_mini.egg-info/SOURCES.txt
--rw-r--r--   0 overcat    (501) staff       (20)        1 2023-05-30 16:41:04.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk_mini.egg-info/dependency_links.txt
--rw-r--r--   0 overcat    (501) staff       (20)       71 2023-05-30 16:41:04.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk_mini.egg-info/requires.txt
--rw-r--r--   0 overcat    (501) staff       (20)       12 2023-05-30 16:41:04.000000 stellar-sdk-mini-8.2.0.post1/stellar_sdk_mini.egg-info/top_level.txt
+drwxr-xr-x   0 overcat    (501) staff       (20)        0 2023-05-31 00:34:31.433508 stellar-sdk-mini-8.2.0.post2/
+-rw-r--r--   0 overcat    (501) staff       (20)    11357 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/LICENSE
+-rw-r--r--   0 overcat    (501) staff       (20)     7390 2023-05-31 00:34:31.433595 stellar-sdk-mini-8.2.0.post2/PKG-INFO
+-rw-r--r--   0 overcat    (501) staff       (20)     6068 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/README.rst
+-rw-r--r--   0 overcat    (501) staff       (20)      110 2023-05-31 00:34:31.433859 stellar-sdk-mini-8.2.0.post2/setup.cfg
+-rw-r--r--   0 overcat    (501) staff       (20)     1993 2023-05-31 00:30:09.000000 stellar-sdk-mini-8.2.0.post2/setup.py
+drwxr-xr-x   0 overcat    (501) staff       (20)        0 2023-05-31 00:34:31.379362 stellar-sdk-mini-8.2.0.post2/stellar_sdk/
+-rw-r--r--   0 overcat    (501) staff       (20)      812 2023-05-30 16:13:27.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/__init__.py
+-rw-r--r--   0 overcat    (501) staff       (20)      864 2023-05-31 00:31:02.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/__version__.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3871 2023-05-30 16:22:04.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/account.py
+-rw-r--r--   0 overcat    (501) staff       (20)     9194 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/asset.py
+-rw-r--r--   0 overcat    (501) staff       (20)    13621 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/base_server.py
+-rw-r--r--   0 overcat    (501) staff       (20)     5492 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/base_transaction_envelope.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1836 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/decorated_signature.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1722 2023-05-30 16:19:18.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/exceptions.py
+-rw-r--r--   0 overcat    (501) staff       (20)     5226 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/fee_bump_transaction.py
+-rw-r--r--   0 overcat    (501) staff       (20)     5562 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/fee_bump_transaction_envelope.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1998 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/helpers.py
+-rw-r--r--   0 overcat    (501) staff       (20)    12080 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/keypair.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2298 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/ledger_bounds.py
+-rw-r--r--   0 overcat    (501) staff       (20)     5997 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/liquidity_pool_asset.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2195 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/liquidity_pool_id.py
+-rw-r--r--   0 overcat    (501) staff       (20)     8941 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/memo.py
+-rw-r--r--   0 overcat    (501) staff       (20)     6110 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/muxed_account.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1742 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/network.py
+drwxr-xr-x   0 overcat    (501) staff       (20)        0 2023-05-31 00:34:31.382137 stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/
+-rw-r--r--   0 overcat    (501) staff       (20)      845 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/__init__.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2087 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/account_merge.py
+-rw-r--r--   0 overcat    (501) staff       (20)     6259 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/allow_trust.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2890 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/begin_sponsoring_future_reserves.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2163 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/bump_sequence.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3157 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/change_trust.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2529 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/claim_claimable_balance.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2679 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/clawback.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2510 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/clawback_claimable_balance.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3271 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/create_account.py
+-rw-r--r--   0 overcat    (501) staff       (20)    16694 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/create_claimable_balance.py
+-rw-r--r--   0 overcat    (501) staff       (20)     4357 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/create_passive_sell_offer.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1737 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/end_sponsoring_future_reserves.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1212 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/inflation.py
+-rw-r--r--   0 overcat    (501) staff       (20)     4741 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/liquidity_pool_deposit.py
+-rw-r--r--   0 overcat    (501) staff       (20)     4147 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/liquidity_pool_withdraw.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3881 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/manage_buy_offer.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3391 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/manage_data.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3892 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/manage_sell_offer.py
+-rw-r--r--   0 overcat    (501) staff       (20)     4909 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/operation.py
+-rw-r--r--   0 overcat    (501) staff       (20)     5001 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/path_payment_strict_receive.py
+-rw-r--r--   0 overcat    (501) staff       (20)     4935 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/path_payment_strict_send.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2783 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/payment.py
+-rw-r--r--   0 overcat    (501) staff       (20)    23692 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/revoke_sponsorship.py
+-rw-r--r--   0 overcat    (501) staff       (20)    10477 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/set_options.py
+-rw-r--r--   0 overcat    (501) staff       (20)     4633 2023-05-30 16:19:41.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/set_trust_line_flags.py
+-rw-r--r--   0 overcat    (501) staff       (20)     8384 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/preconditions.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2039 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/price.py
+drwxr-xr-x   0 overcat    (501) staff       (20)        0 2023-05-31 00:34:31.382320 stellar-sdk-mini-8.2.0.post2/stellar_sdk/sep/
+-rw-r--r--   0 overcat    (501) staff       (20)        0 2023-05-30 16:21:00.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/sep/__init__.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3117 2023-05-30 16:21:45.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/sep/mnemonic.py
+-rw-r--r--   0 overcat    (501) staff       (20)     4072 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/signer.py
+-rw-r--r--   0 overcat    (501) staff       (20)    11183 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/signer_key.py
+-rw-r--r--   0 overcat    (501) staff       (20)    12157 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/strkey.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2516 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/time_bounds.py
+-rw-r--r--   0 overcat    (501) staff       (20)    10470 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/transaction.py
+-rw-r--r--   0 overcat    (501) staff       (20)    55381 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/transaction_builder.py
+-rw-r--r--   0 overcat    (501) staff       (20)     7136 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/transaction_envelope.py
+-rw-r--r--   0 overcat    (501) staff       (20)     5850 2023-05-30 16:19:25.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/utils.py
+drwxr-xr-x   0 overcat    (501) staff       (20)        0 2023-05-31 00:34:31.432855 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/
+-rw-r--r--   0 overcat    (501) staff       (20)    15456 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/__init__.py
+-rw-r--r--   0 overcat    (501) staff       (20)     5998 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/account_entry.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2173 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/account_entry_ext.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2199 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/account_entry_extension_v1.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2239 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/account_entry_extension_v1_ext.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3775 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/account_entry_extension_v2.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2239 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/account_entry_extension_v2_ext.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2600 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/account_entry_extension_v3.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1975 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/account_flags.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1435 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/account_id.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2643 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/account_merge_result.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2246 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/account_merge_result_code.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2307 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/allow_trust_op.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1865 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/allow_trust_result.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2154 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/allow_trust_result_code.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1903 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/alpha_num12.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1891 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/alpha_num4.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3284 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/asset.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3133 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/asset_code.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1482 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/asset_code12.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1462 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/asset_code4.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1368 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/asset_type.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1586 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/auth.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2203 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/auth_cert.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2188 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/authenticated_message.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2297 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/authenticated_message_v0.py
+-rw-r--r--   0 overcat    (501) staff       (20)     6074 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/base.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1771 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/begin_sponsoring_future_reserves_op.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2290 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/begin_sponsoring_future_reserves_result.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1843 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/begin_sponsoring_future_reserves_result_code.py
+-rw-r--r--   0 overcat    (501) staff       (20)     4114 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/bucket_entry.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1529 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/bucket_entry_type.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2165 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/bucket_metadata.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1620 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/bucket_metadata_ext.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1617 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/bump_sequence_op.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1899 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/bump_sequence_result.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1451 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/bump_sequence_result_code.py
+-rw-r--r--   0 overcat    (501) staff       (20)     4223 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/change_trust_asset.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1907 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/change_trust_op.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1882 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/change_trust_result.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2395 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/change_trust_result_code.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3812 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/claim_atom.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1327 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/claim_atom_type.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1737 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/claim_claimable_balance_op.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2056 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/claim_claimable_balance_result.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1795 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/claim_claimable_balance_result_code.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3197 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/claim_liquidity_atom.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3449 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/claim_offer_atom.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3512 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/claim_offer_atom_v0.py
+-rw-r--r--   0 overcat    (501) staff       (20)     7156 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/claim_predicate.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1604 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/claim_predicate_type.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3858 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/claimable_balance_entry.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2273 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/claimable_balance_entry_ext.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2176 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/claimable_balance_entry_extension_v1.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1728 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/claimable_balance_entry_extension_v1_ext.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1388 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/claimable_balance_flags.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2220 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/claimable_balance_id.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1235 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/claimable_balance_id_type.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2258 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/claimant.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1151 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/claimant_type.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2075 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/claimant_v0.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1758 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/clawback_claimable_balance_op.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2192 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/clawback_claimable_balance_result.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1783 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/clawback_claimable_balance_result_code.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2136 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/clawback_op.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1827 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/clawback_result.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1598 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/clawback_result_code.py
+-rw-r--r--   0 overcat    (501) staff       (20)      847 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/constants.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2123 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/create_account_op.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1916 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/create_account_result.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1857 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/create_account_result_code.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2745 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/create_claimable_balance_op.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2670 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/create_claimable_balance_result.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1804 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/create_claimable_balance_result_code.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2543 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/create_passive_sell_offer_op.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1578 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/crypto_key_type.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1572 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/curve25519_public.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1572 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/curve25519_secret.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2750 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/data_entry.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1590 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/data_entry_ext.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1450 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/data_value.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2004 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/decorated_signature.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1830 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/dont_have.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1392 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/duration.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1527 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/encrypted_body.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2256 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/end_sponsoring_future_reserves_result.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1589 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/end_sponsoring_future_reserves_result_code.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1642 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/envelope_type.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1750 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/error.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1401 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/error_code.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1595 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/extension_point.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2890 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/fee_bump_transaction.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2668 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/fee_bump_transaction_envelope.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1644 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/fee_bump_transaction_ext.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2237 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/fee_bump_transaction_inner_tx.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1353 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/hash.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3538 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/hash_id_preimage.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2399 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/hash_id_preimage_operation_id.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3081 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/hash_id_preimage_revoke_id.py
+-rw-r--r--   0 overcat    (501) staff       (20)     4324 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/hello.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1551 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/hmac_sha256_key.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1551 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/hmac_sha256_mac.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1964 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/inflation_payout.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2804 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/inflation_result.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1386 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/inflation_result_code.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3356 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/inner_transaction_result.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1668 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/inner_transaction_result_ext.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2231 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/inner_transaction_result_pair.py
+-rw-r--r--   0 overcat    (501) staff       (20)     6296 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/inner_transaction_result_result.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1344 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/int32.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1340 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/int64.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1150 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ip_addr_type.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1948 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_bounds.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2012 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_close_meta.py
+-rw-r--r--   0 overcat    (501) staff       (20)     5280 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_close_meta_v0.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2045 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_close_value_signature.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3105 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_entry.py
+-rw-r--r--   0 overcat    (501) staff       (20)     4292 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_entry_change.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1541 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_entry_change_type.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2241 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_entry_changes.py
+-rw-r--r--   0 overcat    (501) staff       (20)     5915 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_entry_data.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2162 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_entry_ext.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2198 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_entry_extension_v1.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1668 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_entry_extension_v1_ext.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1384 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_entry_type.py
+-rw-r--r--   0 overcat    (501) staff       (20)     7964 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_header.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2173 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_header_ext.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2059 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_header_extension_v1.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1674 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_header_extension_v1_ext.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1425 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_header_flags.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2422 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_header_history_entry.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1680 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_header_history_entry_ext.py
+-rw-r--r--   0 overcat    (501) staff       (20)     6398 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_key.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1636 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_key_account.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1736 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_key_claimable_balance.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1944 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_key_data.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1740 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_key_liquidity_pool.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1911 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_key_offer.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1959 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_key_trust_line.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2442 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_scp_messages.py
+-rw-r--r--   0 overcat    (501) staff       (20)     5635 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_upgrade.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1501 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_upgrade_type.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1798 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/liabilities.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2363 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/liquidity_pool_constant_product_parameters.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3239 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/liquidity_pool_deposit_op.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2052 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/liquidity_pool_deposit_result.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2592 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/liquidity_pool_deposit_result_code.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2675 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/liquidity_pool_entry.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3023 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/liquidity_pool_entry_body.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3600 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/liquidity_pool_entry_constant_product.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2666 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/liquidity_pool_parameters.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1211 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/liquidity_pool_type.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2869 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/liquidity_pool_withdraw_op.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2069 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/liquidity_pool_withdraw_result.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2272 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/liquidity_pool_withdraw_result_code.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2979 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/manage_buy_offer_op.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2450 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/manage_buy_offer_result.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2928 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/manage_buy_offer_result_code.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2153 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/manage_data_op.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1865 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/manage_data_result.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1863 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/manage_data_result_code.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1323 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/manage_offer_effect.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2931 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/manage_offer_success_result.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2790 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/manage_offer_success_result_offer.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2899 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/manage_sell_offer_op.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2467 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/manage_sell_offer_result.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3030 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/manage_sell_offer_result_code.py
+-rw-r--r--   0 overcat    (501) staff       (20)     4005 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/memo.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1293 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/memo_type.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2023 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/message_type.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3024 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/muxed_account.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1847 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/muxed_account_med25519.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1384 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/node_id.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3951 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/offer_entry.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1596 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/offer_entry_ext.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1256 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/offer_entry_flags.py
+-rw-r--r--   0 overcat    (501) staff       (20)     4571 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/operation.py
+-rw-r--r--   0 overcat    (501) staff       (20)    23123 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/operation_body.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1632 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/operation_meta.py
+-rw-r--r--   0 overcat    (501) staff       (20)     4688 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/operation_result.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1842 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/operation_result_code.py
+-rw-r--r--   0 overcat    (501) staff       (20)    27203 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/operation_result_tr.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2646 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/operation_type.py
+-rw-r--r--   0 overcat    (501) staff       (20)     4041 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/path_payment_strict_receive_op.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3795 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/path_payment_strict_receive_result.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3327 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/path_payment_strict_receive_result_code.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2505 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/path_payment_strict_receive_result_success.py
+-rw-r--r--   0 overcat    (501) staff       (20)     4054 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/path_payment_strict_send_op.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3623 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/path_payment_strict_send_result.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3217 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/path_payment_strict_send_result_code.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2487 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/path_payment_strict_send_result_success.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2306 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/payment_op.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1810 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/payment_result.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2316 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/payment_result_code.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2323 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/peer_address.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2697 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/peer_address_ip.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2020 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/peer_stat_list.py
+-rw-r--r--   0 overcat    (501) staff       (20)     7616 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/peer_stats.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1358 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/pool_id.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1257 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/precondition_type.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3135 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/preconditions.py
+-rw-r--r--   0 overcat    (501) staff       (20)     5895 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/preconditions_v2.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1652 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/price.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2168 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/public_key.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1186 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/public_key_type.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3281 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/revoke_sponsorship_op.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2058 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/revoke_sponsorship_op_signer.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1984 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/revoke_sponsorship_result.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1847 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/revoke_sponsorship_result_code.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1312 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/revoke_sponsorship_type.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1815 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/scp_ballot.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1939 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/scp_envelope.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2012 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/scp_history_entry.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2709 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/scp_history_entry_v0.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3171 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/scp_nomination.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3250 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/scp_quorum_set.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3468 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/scp_statement.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2954 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/scp_statement_confirm.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2467 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/scp_statement_externalize.py
+-rw-r--r--   0 overcat    (501) staff       (20)     5360 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/scp_statement_pledges.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3650 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/scp_statement_prepare.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1346 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/scp_statement_type.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1594 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/send_more.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1499 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/sequence_number.py
+-rw-r--r--   0 overcat    (501) staff       (20)     6199 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/set_options_op.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1865 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/set_options_result.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2584 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/set_options_result_code.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2618 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/set_trust_line_flags_op.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1992 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/set_trust_line_flags_result.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1983 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/set_trust_line_flags_result_code.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1440 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/signature.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1513 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/signature_hint.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2192 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/signed_survey_request_message.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2228 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/signed_survey_response_message.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1793 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/signer.py
+-rw-r--r--   0 overcat    (501) staff       (20)     4930 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/signer_key.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2100 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/signer_key_ed25519_signed_payload.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1504 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/signer_key_type.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2256 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/simple_payment_result.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1868 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/sponsorship_descriptor.py
+-rw-r--r--   0 overcat    (501) staff       (20)    13256 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/stellar_message.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3780 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/stellar_value.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2671 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/stellar_value_ext.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1248 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/stellar_value_type.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1405 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/string32.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1405 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/string64.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1221 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/survey_message_command_type.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3354 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/survey_request_message.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2633 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/survey_response_body.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3346 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/survey_response_message.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1350 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/threshold_indexes.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1452 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/thresholds.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1885 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/time_bounds.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1419 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/time_point.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3111 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/topology_response_body.py
+-rw-r--r--   0 overcat    (501) staff       (20)     4356 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3675 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_envelope.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1602 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_ext.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2500 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_history_entry.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1674 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_history_entry_ext.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2681 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_history_result_entry.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1710 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_history_result_entry_ext.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3762 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_meta.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2634 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_meta_v1.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3340 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_meta_v2.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2874 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_result.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2894 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_result_code.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1638 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_result_ext.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2650 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_result_meta.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2122 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_result_pair.py
+-rw-r--r--   0 overcat    (501) staff       (20)     4972 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_result_result.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2170 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_result_set.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2506 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_set.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2646 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_signature_payload.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3202 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_signature_payload_tagged_transaction.py
+-rw-r--r--   0 overcat    (501) staff       (20)     4455 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_v0.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2607 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_v0_envelope.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1614 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_v0_ext.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2596 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_v1_envelope.py
+-rw-r--r--   0 overcat    (501) staff       (20)     4167 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/trust_line_asset.py
+-rw-r--r--   0 overcat    (501) staff       (20)     3848 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/trust_line_entry.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2472 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/trust_line_entry_ext.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2317 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/trust_line_entry_extension_v2.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1686 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/trust_line_entry_extension_v2_ext.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2194 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/trust_line_entry_v1.py
+-rw-r--r--   0 overcat    (501) staff       (20)     2256 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/trust_line_entry_v1_ext.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1710 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/trust_line_flags.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1404 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/uint256.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1394 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/uint32.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1390 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/uint64.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1978 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/upgrade_entry_meta.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1487 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/upgrade_type.py
+-rw-r--r--   0 overcat    (501) staff       (20)     1386 2023-05-30 15:50:33.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/value.py
+drwxr-xr-x   0 overcat    (501) staff       (20)        0 2023-05-31 00:34:31.433407 stellar-sdk-mini-8.2.0.post2/stellar_sdk_mini.egg-info/
+-rw-r--r--   0 overcat    (501) staff       (20)     7390 2023-05-31 00:34:31.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk_mini.egg-info/PKG-INFO
+-rw-r--r--   0 overcat    (501) staff       (20)    13853 2023-05-31 00:34:31.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk_mini.egg-info/SOURCES.txt
+-rw-r--r--   0 overcat    (501) staff       (20)        1 2023-05-31 00:34:31.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk_mini.egg-info/dependency_links.txt
+-rw-r--r--   0 overcat    (501) staff       (20)       58 2023-05-31 00:34:31.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk_mini.egg-info/requires.txt
+-rw-r--r--   0 overcat    (501) staff       (20)       12 2023-05-31 00:34:31.000000 stellar-sdk-mini-8.2.0.post2/stellar_sdk_mini.egg-info/top_level.txt
```

### Comparing `stellar-sdk-mini-8.2.0.post1/LICENSE` & `stellar-sdk-mini-8.2.0.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/PKG-INFO` & `stellar-sdk-mini-8.2.0.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stellar-sdk-mini
-Version: 8.2.0.post1
+Version: 8.2.0.post2
 Summary: The Python Stellar SDK library provides APIs to build transactions and connect to Horizon.
 Home-page: https://github.com/StellarCN/py-stellar-base
 Author: Eno, overcat
 Author-email: appweb.cn@gmail.com, 4catcode@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://stellar-sdk.readthedocs.org
 Project-URL: Code, https://github.com/StellarCN/py-stellar-base
```

### Comparing `stellar-sdk-mini-8.2.0.post1/README.rst` & `stellar-sdk-mini-8.2.0.post2/README.rst`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/setup.py` & `stellar-sdk-mini-8.2.0.post2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 install_requires = [
     "cffi==1.15.1",
     "mnemonic==0.20",
     "pycparser==2.21",
     "PyNaCl==1.5.0",
-    "toml==0.10.2",
 ]
 
 about = {}
 with open(
         os.path.join(here, "stellar_sdk", "__version__.py"), mode="r", encoding="utf-8"
 ) as f:
     exec(f.read(), about)
```

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/__init__.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/__version__.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/__version__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,11 +7,11 @@
  |_____/   |_|  |______|______|______/_/    \_\_|  \_\    |_____/|_____/|_|\_\
 """
 
 __title__ = "stellar-sdk-mini"
 __description__ = "The Python Stellar SDK library provides APIs to build transactions and connect to Horizon."
 __url__ = "https://github.com/StellarCN/py-stellar-base"
 __issues__ = f"{__url__}/issues"
-__version__ = "8.2.0.post1"
+__version__ = "8.2.0.post2"
 __author__ = "Eno, overcat"
 __author_email__ = "appweb.cn@gmail.com, 4catcode@gmail.com"
 __license__ = "Apache License 2.0"
```

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/account.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/account.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/asset.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/asset.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/base_server.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/base_server.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/base_transaction_envelope.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/base_transaction_envelope.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/decorated_signature.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/decorated_signature.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/exceptions.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/fee_bump_transaction.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/fee_bump_transaction.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/fee_bump_transaction_envelope.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/fee_bump_transaction_envelope.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/helpers.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/helpers.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/keypair.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/keypair.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/ledger_bounds.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/ledger_bounds.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/liquidity_pool_asset.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/liquidity_pool_asset.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/liquidity_pool_id.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/liquidity_pool_id.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/memo.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/memo.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/muxed_account.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/muxed_account.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/network.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/network.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/__init__.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/__init__.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/account_merge.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/account_merge.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/allow_trust.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/allow_trust.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/begin_sponsoring_future_reserves.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/begin_sponsoring_future_reserves.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/bump_sequence.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/bump_sequence.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/change_trust.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/change_trust.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/claim_claimable_balance.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/claim_claimable_balance.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/clawback.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/clawback.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/clawback_claimable_balance.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/clawback_claimable_balance.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/create_account.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/create_account.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/create_claimable_balance.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/create_claimable_balance.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/create_passive_sell_offer.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/create_passive_sell_offer.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/end_sponsoring_future_reserves.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/end_sponsoring_future_reserves.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/inflation.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/inflation.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/liquidity_pool_deposit.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/liquidity_pool_deposit.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/liquidity_pool_withdraw.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/liquidity_pool_withdraw.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/manage_buy_offer.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/manage_buy_offer.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/manage_data.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/manage_data.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/manage_sell_offer.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/manage_sell_offer.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/operation.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/operation.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/path_payment_strict_receive.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/path_payment_strict_receive.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/path_payment_strict_send.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/path_payment_strict_send.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/payment.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/payment.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/revoke_sponsorship.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/revoke_sponsorship.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/set_options.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/set_options.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/operation/set_trust_line_flags.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/operation/set_trust_line_flags.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/preconditions.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/preconditions.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/price.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/price.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/sep/mnemonic.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/sep/mnemonic.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/signer.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/signer.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/signer_key.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/signer_key.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/strkey.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/strkey.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/time_bounds.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/time_bounds.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/transaction.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/transaction.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/transaction_builder.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/transaction_builder.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/transaction_envelope.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/transaction_envelope.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/utils.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/__init__.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/__init__.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/account_entry.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/account_entry.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/account_entry_ext.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/account_entry_ext.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/account_entry_extension_v1.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/account_entry_extension_v1.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/account_entry_extension_v1_ext.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/account_entry_extension_v1_ext.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/account_entry_extension_v2.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/account_entry_extension_v2.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/account_entry_extension_v2_ext.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/account_entry_extension_v2_ext.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/account_entry_extension_v3.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/account_entry_extension_v3.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/account_flags.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/account_flags.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/account_id.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/account_id.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/account_merge_result.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/account_merge_result.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/account_merge_result_code.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/account_merge_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/allow_trust_op.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/allow_trust_op.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/allow_trust_result.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/allow_trust_result.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/allow_trust_result_code.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/allow_trust_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/alpha_num12.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/alpha_num12.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/alpha_num4.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/alpha_num4.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/asset.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/asset.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/asset_code.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/asset_code.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/asset_code12.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/asset_code12.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/asset_code4.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/asset_code4.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/asset_type.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/asset_type.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/auth.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/auth.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/auth_cert.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/auth_cert.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/authenticated_message.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/authenticated_message.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/authenticated_message_v0.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/authenticated_message_v0.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/base.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/base.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/begin_sponsoring_future_reserves_op.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/begin_sponsoring_future_reserves_op.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/begin_sponsoring_future_reserves_result.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/begin_sponsoring_future_reserves_result.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/begin_sponsoring_future_reserves_result_code.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/begin_sponsoring_future_reserves_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/bucket_entry.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/bucket_entry.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/bucket_entry_type.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/bucket_entry_type.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/bucket_metadata.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/bucket_metadata.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/bucket_metadata_ext.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/bucket_metadata_ext.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/bump_sequence_op.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/bump_sequence_op.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/bump_sequence_result.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/bump_sequence_result.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/bump_sequence_result_code.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/bump_sequence_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/change_trust_asset.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/change_trust_asset.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/change_trust_op.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/change_trust_op.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/change_trust_result.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/change_trust_result.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/change_trust_result_code.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/change_trust_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/claim_atom.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/claim_atom.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/claim_atom_type.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/claim_atom_type.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/claim_claimable_balance_op.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/claim_claimable_balance_op.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/claim_claimable_balance_result.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/claim_claimable_balance_result.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/claim_claimable_balance_result_code.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/claim_claimable_balance_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/claim_liquidity_atom.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/claim_liquidity_atom.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/claim_offer_atom.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/claim_offer_atom.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/claim_offer_atom_v0.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/claim_offer_atom_v0.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/claim_predicate.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/claim_predicate.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/claim_predicate_type.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/claim_predicate_type.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/claimable_balance_entry.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/claimable_balance_entry.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/claimable_balance_entry_ext.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/claimable_balance_entry_ext.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/claimable_balance_entry_extension_v1.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/claimable_balance_entry_extension_v1.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/claimable_balance_entry_extension_v1_ext.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/claimable_balance_entry_extension_v1_ext.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/claimable_balance_flags.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/claimable_balance_flags.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/claimable_balance_id.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/claimable_balance_id.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/claimable_balance_id_type.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/claimable_balance_id_type.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/claimant.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/claimant.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/claimant_type.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/claimant_type.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/claimant_v0.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/claimant_v0.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/clawback_claimable_balance_op.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/clawback_claimable_balance_op.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/clawback_claimable_balance_result.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/clawback_claimable_balance_result.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/clawback_claimable_balance_result_code.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/clawback_claimable_balance_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/clawback_op.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/clawback_op.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/clawback_result.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/clawback_result.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/clawback_result_code.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/clawback_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/constants.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/constants.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/create_account_op.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/create_account_op.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/create_account_result.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/create_account_result.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/create_account_result_code.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/create_account_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/create_claimable_balance_op.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/create_claimable_balance_op.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/create_claimable_balance_result.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/create_claimable_balance_result.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/create_claimable_balance_result_code.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/create_claimable_balance_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/create_passive_sell_offer_op.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/create_passive_sell_offer_op.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/crypto_key_type.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/crypto_key_type.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/curve25519_public.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/curve25519_public.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/curve25519_secret.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/curve25519_secret.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/data_entry.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/data_entry.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/data_entry_ext.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/data_entry_ext.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/data_value.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/data_value.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/decorated_signature.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/decorated_signature.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/dont_have.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/dont_have.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/duration.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/duration.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/encrypted_body.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/encrypted_body.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/end_sponsoring_future_reserves_result.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/end_sponsoring_future_reserves_result.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/end_sponsoring_future_reserves_result_code.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/end_sponsoring_future_reserves_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/envelope_type.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/envelope_type.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/error.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/error.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/error_code.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/error_code.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/extension_point.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/extension_point.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/fee_bump_transaction.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/fee_bump_transaction.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/fee_bump_transaction_envelope.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/fee_bump_transaction_envelope.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/fee_bump_transaction_ext.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/fee_bump_transaction_ext.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/fee_bump_transaction_inner_tx.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/fee_bump_transaction_inner_tx.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/hash.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/hash.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/hash_id_preimage.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/hash_id_preimage.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/hash_id_preimage_operation_id.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/hash_id_preimage_operation_id.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/hash_id_preimage_revoke_id.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/hash_id_preimage_revoke_id.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/hello.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/hello.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/hmac_sha256_key.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/hmac_sha256_key.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/hmac_sha256_mac.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/hmac_sha256_mac.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/inflation_payout.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/inflation_payout.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/inflation_result.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/inflation_result.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/inflation_result_code.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/inflation_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/inner_transaction_result.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/inner_transaction_result.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/inner_transaction_result_ext.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/inner_transaction_result_ext.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/inner_transaction_result_pair.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/inner_transaction_result_pair.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/inner_transaction_result_result.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/inner_transaction_result_result.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/int32.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/int32.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/int64.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/int64.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ip_addr_type.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ip_addr_type.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_bounds.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_bounds.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_close_meta.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_close_meta.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_close_meta_v0.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_close_meta_v0.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_close_value_signature.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_close_value_signature.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_entry.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_entry.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_entry_change.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_entry_change.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_entry_change_type.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_entry_change_type.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_entry_changes.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_entry_changes.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_entry_data.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_entry_data.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_entry_ext.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_entry_ext.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_entry_extension_v1.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_entry_extension_v1.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_entry_extension_v1_ext.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_entry_extension_v1_ext.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_entry_type.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_entry_type.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_header.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_header.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_header_ext.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_header_ext.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_header_extension_v1.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_header_extension_v1.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_header_extension_v1_ext.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_header_extension_v1_ext.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_header_flags.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_header_flags.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_header_history_entry.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_header_history_entry.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_header_history_entry_ext.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_header_history_entry_ext.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_key.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_key.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_key_account.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_key_account.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_key_claimable_balance.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_key_claimable_balance.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_key_data.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_key_data.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_key_liquidity_pool.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_key_liquidity_pool.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_key_offer.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_key_offer.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_key_trust_line.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_key_trust_line.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_scp_messages.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_scp_messages.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_upgrade.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_upgrade.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/ledger_upgrade_type.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/ledger_upgrade_type.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/liabilities.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/liabilities.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/liquidity_pool_constant_product_parameters.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/liquidity_pool_constant_product_parameters.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/liquidity_pool_deposit_op.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/liquidity_pool_deposit_op.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/liquidity_pool_deposit_result.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/liquidity_pool_deposit_result.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/liquidity_pool_deposit_result_code.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/liquidity_pool_deposit_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/liquidity_pool_entry.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/liquidity_pool_entry.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/liquidity_pool_entry_body.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/liquidity_pool_entry_body.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/liquidity_pool_entry_constant_product.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/liquidity_pool_entry_constant_product.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/liquidity_pool_parameters.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/liquidity_pool_parameters.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/liquidity_pool_type.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/liquidity_pool_type.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/liquidity_pool_withdraw_op.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/liquidity_pool_withdraw_op.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/liquidity_pool_withdraw_result.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/liquidity_pool_withdraw_result.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/liquidity_pool_withdraw_result_code.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/liquidity_pool_withdraw_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/manage_buy_offer_op.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/manage_buy_offer_op.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/manage_buy_offer_result.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/manage_buy_offer_result.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/manage_buy_offer_result_code.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/manage_buy_offer_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/manage_data_op.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/manage_data_op.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/manage_data_result.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/manage_data_result.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/manage_data_result_code.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/manage_data_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/manage_offer_effect.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/manage_offer_effect.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/manage_offer_success_result.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/manage_offer_success_result.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/manage_offer_success_result_offer.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/manage_offer_success_result_offer.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/manage_sell_offer_op.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/manage_sell_offer_op.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/manage_sell_offer_result.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/manage_sell_offer_result.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/manage_sell_offer_result_code.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/manage_sell_offer_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/memo.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/memo.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/memo_type.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/memo_type.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/message_type.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/message_type.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/muxed_account.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/muxed_account.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/muxed_account_med25519.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/muxed_account_med25519.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/node_id.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/node_id.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/offer_entry.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/offer_entry.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/offer_entry_ext.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/offer_entry_ext.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/offer_entry_flags.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/offer_entry_flags.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/operation.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/operation.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/operation_body.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/operation_body.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/operation_meta.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/operation_meta.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/operation_result.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/operation_result.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/operation_result_code.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/operation_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/operation_result_tr.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/operation_result_tr.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/operation_type.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/operation_type.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/path_payment_strict_receive_op.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/path_payment_strict_receive_op.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/path_payment_strict_receive_result.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/path_payment_strict_receive_result.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/path_payment_strict_receive_result_code.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/path_payment_strict_receive_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/path_payment_strict_receive_result_success.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/path_payment_strict_receive_result_success.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/path_payment_strict_send_op.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/path_payment_strict_send_op.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/path_payment_strict_send_result.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/path_payment_strict_send_result.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/path_payment_strict_send_result_code.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/path_payment_strict_send_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/path_payment_strict_send_result_success.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/path_payment_strict_send_result_success.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/payment_op.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/payment_op.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/payment_result.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/payment_result.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/payment_result_code.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/payment_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/peer_address.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/peer_address.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/peer_address_ip.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/peer_address_ip.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/peer_stat_list.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/peer_stat_list.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/peer_stats.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/peer_stats.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/pool_id.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/pool_id.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/precondition_type.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/precondition_type.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/preconditions.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/preconditions.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/preconditions_v2.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/preconditions_v2.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/price.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/price.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/public_key.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/public_key.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/public_key_type.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/public_key_type.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/revoke_sponsorship_op.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/revoke_sponsorship_op.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/revoke_sponsorship_op_signer.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/revoke_sponsorship_op_signer.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/revoke_sponsorship_result.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/revoke_sponsorship_result.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/revoke_sponsorship_result_code.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/revoke_sponsorship_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/revoke_sponsorship_type.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/revoke_sponsorship_type.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/scp_ballot.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/scp_ballot.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/scp_envelope.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/scp_envelope.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/scp_history_entry.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/scp_history_entry.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/scp_history_entry_v0.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/scp_history_entry_v0.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/scp_nomination.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/scp_nomination.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/scp_quorum_set.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/scp_quorum_set.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/scp_statement.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/scp_statement.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/scp_statement_confirm.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/scp_statement_confirm.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/scp_statement_externalize.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/scp_statement_externalize.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/scp_statement_pledges.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/scp_statement_pledges.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/scp_statement_prepare.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/scp_statement_prepare.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/scp_statement_type.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/scp_statement_type.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/send_more.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/send_more.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/sequence_number.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/sequence_number.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/set_options_op.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/set_options_op.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/set_options_result.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/set_options_result.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/set_options_result_code.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/set_options_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/set_trust_line_flags_op.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/set_trust_line_flags_op.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/set_trust_line_flags_result.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/set_trust_line_flags_result.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/set_trust_line_flags_result_code.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/set_trust_line_flags_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/signature.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/signature.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/signature_hint.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/signature_hint.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/signed_survey_request_message.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/signed_survey_request_message.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/signed_survey_response_message.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/signed_survey_response_message.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/signer.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/signer.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/signer_key.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/signer_key.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/signer_key_ed25519_signed_payload.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/signer_key_ed25519_signed_payload.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/signer_key_type.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/signer_key_type.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/simple_payment_result.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/simple_payment_result.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/sponsorship_descriptor.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/sponsorship_descriptor.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/stellar_message.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/stellar_message.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/stellar_value.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/stellar_value.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/stellar_value_ext.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/stellar_value_ext.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/stellar_value_type.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/stellar_value_type.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/string32.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/string32.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/string64.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/string64.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/survey_message_command_type.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/survey_message_command_type.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/survey_request_message.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/survey_request_message.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/survey_response_body.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/survey_response_body.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/survey_response_message.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/survey_response_message.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/threshold_indexes.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/threshold_indexes.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/thresholds.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/thresholds.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/time_bounds.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/time_bounds.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/time_point.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/time_point.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/topology_response_body.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/topology_response_body.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_envelope.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_envelope.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_ext.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_ext.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_history_entry.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_history_entry.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_history_entry_ext.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_history_entry_ext.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_history_result_entry.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_history_result_entry.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_history_result_entry_ext.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_history_result_entry_ext.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_meta.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_meta.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_meta_v1.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_meta_v1.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_meta_v2.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_meta_v2.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_result.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_result.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_result_code.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_result_ext.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_result_ext.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_result_meta.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_result_meta.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_result_pair.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_result_pair.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_result_result.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_result_result.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_result_set.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_result_set.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_set.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_set.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_signature_payload.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_signature_payload.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_signature_payload_tagged_transaction.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_signature_payload_tagged_transaction.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_v0.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_v0.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_v0_envelope.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_v0_envelope.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_v0_ext.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_v0_ext.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/transaction_v1_envelope.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/transaction_v1_envelope.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/trust_line_asset.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/trust_line_asset.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/trust_line_entry.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/trust_line_entry.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/trust_line_entry_ext.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/trust_line_entry_ext.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/trust_line_entry_extension_v2.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/trust_line_entry_extension_v2.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/trust_line_entry_extension_v2_ext.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/trust_line_entry_extension_v2_ext.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/trust_line_entry_v1.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/trust_line_entry_v1.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/trust_line_entry_v1_ext.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/trust_line_entry_v1_ext.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/trust_line_flags.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/trust_line_flags.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/uint256.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/uint256.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/uint32.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/uint32.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/uint64.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/uint64.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/upgrade_entry_meta.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/upgrade_entry_meta.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/upgrade_type.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/upgrade_type.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk/xdr/value.py` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk/xdr/value.py`

 * *Files identical despite different names*

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk_mini.egg-info/PKG-INFO` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk_mini.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stellar-sdk-mini
-Version: 8.2.0.post1
+Version: 8.2.0.post2
 Summary: The Python Stellar SDK library provides APIs to build transactions and connect to Horizon.
 Home-page: https://github.com/StellarCN/py-stellar-base
 Author: Eno, overcat
 Author-email: appweb.cn@gmail.com, 4catcode@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://stellar-sdk.readthedocs.org
 Project-URL: Code, https://github.com/StellarCN/py-stellar-base
```

### Comparing `stellar-sdk-mini-8.2.0.post1/stellar_sdk_mini.egg-info/SOURCES.txt` & `stellar-sdk-mini-8.2.0.post2/stellar_sdk_mini.egg-info/SOURCES.txt`

 * *Files identical despite different names*

