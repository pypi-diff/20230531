# Comparing `tmp/increase-0.5.0.tar.gz` & `tmp/increase-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "increase-0.5.0.tar", max compression
+gzip compressed data, was "increase-0.6.0.tar", max compression
```

## Comparing `increase-0.5.0.tar` & `increase-0.6.0.tar`

### file list

```diff
@@ -1,177 +1,205 @@
--rw-r--r--   0        0        0    11338 2023-01-25 16:53:45.697921 increase-0.5.0/LICENSE
--rw-r--r--   0        0        0     8436 2023-03-15 18:51:50.414999 increase-0.5.0/README.md
--rw-r--r--   0        0        0     1856 2023-03-18 01:26:15.043025 increase-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2587 2023-03-18 01:26:08.353678 increase-0.5.0/src/increase/__init__.py
--rw-r--r--   0        0        0    45366 2023-03-18 01:26:08.353944 increase-0.5.0/src/increase/_base_client.py
--rw-r--r--   0        0        0     3889 2023-03-15 18:51:50.417952 increase-0.5.0/src/increase/_base_exceptions.py
--rw-r--r--   0        0        0    25024 2023-03-18 01:26:08.354159 increase-0.5.0/src/increase/_client.py
--rw-r--r--   0        0        0    10885 2023-03-15 18:51:50.418426 increase-0.5.0/src/increase/_exceptions.py
--rw-r--r--   0        0        0     7343 2023-03-15 18:51:50.418574 increase-0.5.0/src/increase/_models.py
--rw-r--r--   0        0        0     4781 2023-01-25 16:53:45.700289 increase-0.5.0/src/increase/_qs.py
--rw-r--r--   0        0        0      890 2023-01-25 16:53:45.700394 increase-0.5.0/src/increase/_resource.py
--rw-r--r--   0        0        0     3979 2023-03-15 18:51:50.418683 increase-0.5.0/src/increase/_types.py
--rw-r--r--   0        0        0     1277 2023-03-18 01:26:08.354316 increase-0.5.0/src/increase/_utils/__init__.py
--rw-r--r--   0        0        0     6701 2023-03-15 18:51:50.418919 increase-0.5.0/src/increase/_utils/_transform.py
--rw-r--r--   0        0        0     9411 2023-03-18 01:26:08.354474 increase-0.5.0/src/increase/_utils/_utils.py
--rw-r--r--   0        0        0       99 2023-03-18 01:26:15.062748 increase-0.5.0/src/increase/_version.py
--rw-r--r--   0        0        0     1109 2023-01-25 16:53:45.701431 increase-0.5.0/src/increase/pagination.py
--rw-r--r--   0        0        0        0 2023-01-25 16:53:45.701483 increase-0.5.0/src/increase/py.typed
--rw-r--r--   0        0        0     3601 2023-03-15 18:51:50.419165 increase-0.5.0/src/increase/resources/__init__.py
--rw-r--r--   0        0        0    12621 2023-03-18 01:26:08.354632 increase-0.5.0/src/increase/resources/account_numbers.py
--rw-r--r--   0        0        0     6054 2023-03-15 18:51:50.419444 increase-0.5.0/src/increase/resources/account_statements.py
--rw-r--r--   0        0        0    14190 2023-03-18 01:26:08.354803 increase-0.5.0/src/increase/resources/account_transfers.py
--rw-r--r--   0        0        0    14028 2023-03-18 01:26:08.354940 increase-0.5.0/src/increase/resources/accounts.py
--rw-r--r--   0        0        0    13890 2023-03-18 01:26:08.355106 increase-0.5.0/src/increase/resources/ach_prenotifications.py
--rw-r--r--   0        0        0    22211 2023-03-18 01:26:08.355263 increase-0.5.0/src/increase/resources/ach_transfers.py
--rw-r--r--   0        0        0     9049 2023-03-18 01:26:08.355407 increase-0.5.0/src/increase/resources/card_disputes.py
--rw-r--r--   0        0        0     8939 2023-03-18 01:26:08.355539 increase-0.5.0/src/increase/resources/card_profiles.py
--rw-r--r--   0        0        0    15682 2023-03-18 01:26:08.355669 increase-0.5.0/src/increase/resources/cards.py
--rw-r--r--   0        0        0    10071 2023-03-18 01:26:08.355788 increase-0.5.0/src/increase/resources/check_deposits.py
--rw-r--r--   0        0        0    18218 2023-03-18 01:26:08.355926 increase-0.5.0/src/increase/resources/check_transfers.py
--rw-r--r--   0        0        0     6437 2023-03-15 18:51:50.420676 increase-0.5.0/src/increase/resources/declined_transactions.py
--rw-r--r--   0        0        0     6019 2023-03-15 18:51:50.420785 increase-0.5.0/src/increase/resources/digital_wallet_tokens.py
--rw-r--r--   0        0        0     5867 2023-03-15 18:51:50.420887 increase-0.5.0/src/increase/resources/documents.py
--rw-r--r--   0        0        0      282 2023-01-25 16:53:45.708475 increase-0.5.0/src/increase/resources/entities/__init__.py
--rw-r--r--   0        0        0    12106 2023-03-18 01:26:08.356099 increase-0.5.0/src/increase/resources/entities/entities.py
--rw-r--r--   0        0        0     3462 2023-03-18 01:26:08.356240 increase-0.5.0/src/increase/resources/entities/supplemental_documents.py
--rw-r--r--   0        0        0    16465 2023-03-18 01:26:08.356392 increase-0.5.0/src/increase/resources/event_subscriptions.py
--rw-r--r--   0        0        0     5880 2023-03-15 18:51:50.421369 increase-0.5.0/src/increase/resources/events.py
--rw-r--r--   0        0        0    13155 2023-03-18 01:26:08.356536 increase-0.5.0/src/increase/resources/external_accounts.py
--rw-r--r--   0        0        0    11091 2023-03-18 01:26:08.356676 increase-0.5.0/src/increase/resources/files.py
--rw-r--r--   0        0        0     1817 2023-01-25 16:53:45.709112 increase-0.5.0/src/increase/resources/groups.py
--rw-r--r--   0        0        0    10293 2023-03-18 01:26:08.356811 increase-0.5.0/src/increase/resources/inbound_ach_transfer_returns.py
--rw-r--r--   0        0        0     5681 2023-03-15 18:51:50.421721 increase-0.5.0/src/increase/resources/inbound_wire_drawdown_requests.py
--rw-r--r--   0        0        0    12137 2023-03-18 01:26:08.356940 increase-0.5.0/src/increase/resources/limits.py
--rw-r--r--   0        0        0     5275 2023-03-15 18:51:50.421951 increase-0.5.0/src/increase/resources/oauth_connections.py
--rw-r--r--   0        0        0     6742 2023-03-15 18:51:50.422075 increase-0.5.0/src/increase/resources/pending_transactions.py
--rw-r--r--   0        0        0     7058 2023-03-18 01:26:08.357096 increase-0.5.0/src/increase/resources/real_time_decisions.py
--rw-r--r--   0        0        0     4595 2023-03-15 18:51:50.422283 increase-0.5.0/src/increase/resources/routing_numbers.py
--rw-r--r--   0        0        0     1782 2023-03-15 18:51:50.422399 increase-0.5.0/src/increase/resources/simulations/__init__.py
--rw-r--r--   0        0        0     3649 2023-03-18 01:26:08.357257 increase-0.5.0/src/increase/resources/simulations/account_statements.py
--rw-r--r--   0        0        0     2907 2023-03-18 01:26:08.357992 increase-0.5.0/src/increase/resources/simulations/account_transfers.py
--rw-r--r--   0        0        0    15569 2023-03-18 01:26:08.358174 increase-0.5.0/src/increase/resources/simulations/ach_transfers.py
--rw-r--r--   0        0        0     4563 2023-03-18 01:26:08.358323 increase-0.5.0/src/increase/resources/simulations/card_disputes.py
--rw-r--r--   0        0        0     3590 2023-03-18 01:26:08.358467 increase-0.5.0/src/increase/resources/simulations/card_refunds.py
--rw-r--r--   0        0        0     9773 2023-03-18 01:26:08.358613 increase-0.5.0/src/increase/resources/simulations/cards.py
--rw-r--r--   0        0        0     6864 2023-03-18 01:26:08.358751 increase-0.5.0/src/increase/resources/simulations/check_deposits.py
--rw-r--r--   0        0        0     4857 2023-03-18 01:26:08.358900 increase-0.5.0/src/increase/resources/simulations/check_transfers.py
--rw-r--r--   0        0        0     3708 2023-03-18 01:26:08.359032 increase-0.5.0/src/increase/resources/simulations/digital_wallet_token_requests.py
--rw-r--r--   0        0        0     3262 2023-03-18 01:26:08.359215 increase-0.5.0/src/increase/resources/simulations/documents.py
--rw-r--r--   0        0        0    13110 2023-03-18 01:26:08.359370 increase-0.5.0/src/increase/resources/simulations/inbound_wire_drawdown_requests.py
--rw-r--r--   0        0        0     6562 2023-03-18 01:26:08.359515 increase-0.5.0/src/increase/resources/simulations/real_time_payments_transfers.py
--rw-r--r--   0        0        0     4127 2023-03-15 18:51:50.423588 increase-0.5.0/src/increase/resources/simulations/simulations.py
--rw-r--r--   0        0        0    11995 2023-03-18 01:26:08.359669 increase-0.5.0/src/increase/resources/simulations/wire_transfers.py
--rw-r--r--   0        0        0     6352 2023-03-15 18:51:50.423822 increase-0.5.0/src/increase/resources/transactions.py
--rw-r--r--   0        0        0    11620 2023-03-18 01:26:08.359820 increase-0.5.0/src/increase/resources/wire_drawdown_requests.py
--rw-r--r--   0        0        0    21545 2023-03-18 01:26:08.360004 increase-0.5.0/src/increase/resources/wire_transfers.py
--rw-r--r--   0        0        0     7159 2023-03-15 18:51:50.424237 increase-0.5.0/src/increase/types/__init__.py
--rw-r--r--   0        0        0     1969 2023-03-15 18:51:50.424331 increase-0.5.0/src/increase/types/account.py
--rw-r--r--   0        0        0      597 2023-01-25 16:53:45.712239 increase-0.5.0/src/increase/types/account_create_params.py
--rw-r--r--   0        0        0      608 2023-01-25 16:53:45.712331 increase-0.5.0/src/increase/types/account_list_params.py
--rw-r--r--   0        0        0     1026 2023-03-15 18:51:50.424425 increase-0.5.0/src/increase/types/account_number.py
--rw-r--r--   0        0        0      408 2023-01-25 16:53:45.712514 increase-0.5.0/src/increase/types/account_number_create_params.py
--rw-r--r--   0        0        0      635 2023-01-25 16:53:45.712611 increase-0.5.0/src/increase/types/account_number_list_params.py
--rw-r--r--   0        0        0      435 2023-01-25 16:53:45.712717 increase-0.5.0/src/increase/types/account_number_update_params.py
--rw-r--r--   0        0        0     1347 2023-03-15 18:51:50.424524 increase-0.5.0/src/increase/types/account_statement.py
--rw-r--r--   0        0        0     1534 2023-03-15 18:51:50.424629 increase-0.5.0/src/increase/types/account_statement_list_params.py
--rw-r--r--   0        0        0     2558 2023-03-15 18:51:50.424734 increase-0.5.0/src/increase/types/account_transfer.py
--rw-r--r--   0        0        0      814 2023-01-25 16:53:45.713107 increase-0.5.0/src/increase/types/account_transfer_create_params.py
--rw-r--r--   0        0        0     1494 2023-03-15 18:51:50.424832 increase-0.5.0/src/increase/types/account_transfer_list_params.py
--rw-r--r--   0        0        0      271 2023-01-25 16:53:45.713286 increase-0.5.0/src/increase/types/account_update_params.py
--rw-r--r--   0        0        0     2152 2023-03-15 18:51:50.425066 increase-0.5.0/src/increase/types/ach_prenotification.py
--rw-r--r--   0        0        0     1847 2023-03-15 18:51:50.425196 increase-0.5.0/src/increase/types/ach_prenotification_create_params.py
--rw-r--r--   0        0        0     1391 2023-03-15 18:51:50.425294 increase-0.5.0/src/increase/types/ach_prenotification_list_params.py
--rw-r--r--   0        0        0     6363 2023-03-15 18:51:50.425379 increase-0.5.0/src/increase/types/ach_transfer.py
--rw-r--r--   0        0        0     3390 2023-03-15 18:51:50.425466 increase-0.5.0/src/increase/types/ach_transfer_create_params.py
--rw-r--r--   0        0        0     1592 2023-03-15 18:51:50.425558 increase-0.5.0/src/increase/types/ach_transfer_list_params.py
--rw-r--r--   0        0        0     2342 2023-03-15 18:51:50.425655 increase-0.5.0/src/increase/types/card.py
--rw-r--r--   0        0        0     1581 2023-03-15 18:51:50.425751 increase-0.5.0/src/increase/types/card_create_params.py
--rw-r--r--   0        0        0      907 2023-01-25 16:53:45.714157 increase-0.5.0/src/increase/types/card_details.py
--rw-r--r--   0        0        0     2021 2023-03-15 18:51:50.425874 increase-0.5.0/src/increase/types/card_dispute.py
--rw-r--r--   0        0        0      483 2023-01-25 16:53:45.714386 increase-0.5.0/src/increase/types/card_dispute_create_params.py
--rw-r--r--   0        0        0     1661 2023-03-15 18:51:50.425974 increase-0.5.0/src/increase/types/card_dispute_list_params.py
--rw-r--r--   0        0        0     1451 2023-03-15 18:51:50.426077 increase-0.5.0/src/increase/types/card_list_params.py
--rw-r--r--   0        0        0     2186 2023-03-15 18:51:50.426193 increase-0.5.0/src/increase/types/card_profile.py
--rw-r--r--   0        0        0     1820 2023-03-15 18:51:50.426279 increase-0.5.0/src/increase/types/card_profile_create_params.py
--rw-r--r--   0        0        0      715 2023-03-15 18:51:50.426391 increase-0.5.0/src/increase/types/card_profile_list_params.py
--rw-r--r--   0        0        0     1619 2023-03-15 18:51:50.426470 increase-0.5.0/src/increase/types/card_update_params.py
--rw-r--r--   0        0        0     4819 2023-03-15 18:51:50.426581 increase-0.5.0/src/increase/types/check_deposit.py
--rw-r--r--   0        0        0      748 2023-01-25 16:53:45.715374 increase-0.5.0/src/increase/types/check_deposit_create_params.py
--rw-r--r--   0        0        0     1477 2023-03-15 18:51:50.426670 increase-0.5.0/src/increase/types/check_deposit_list_params.py
--rw-r--r--   0        0        0     4533 2023-03-15 18:51:50.426770 increase-0.5.0/src/increase/types/check_transfer.py
--rw-r--r--   0        0        0     1939 2023-03-15 18:51:50.426872 increase-0.5.0/src/increase/types/check_transfer_create_params.py
--rw-r--r--   0        0        0     1488 2023-03-15 18:51:50.426961 increase-0.5.0/src/increase/types/check_transfer_list_params.py
--rw-r--r--   0        0        0    12204 2023-03-15 18:51:50.427085 increase-0.5.0/src/increase/types/declined_transaction.py
--rw-r--r--   0        0        0     1598 2023-03-15 18:51:50.427185 increase-0.5.0/src/increase/types/declined_transaction_list_params.py
--rw-r--r--   0        0        0      950 2023-03-15 18:51:50.427287 increase-0.5.0/src/increase/types/digital_wallet_token.py
--rw-r--r--   0        0        0     1489 2023-03-15 18:51:50.427386 increase-0.5.0/src/increase/types/digital_wallet_token_list_params.py
--rw-r--r--   0        0        0      834 2023-03-15 18:51:50.427486 increase-0.5.0/src/increase/types/document.py
--rw-r--r--   0        0        0     1730 2023-03-15 18:51:50.427584 increase-0.5.0/src/increase/types/document_list_params.py
--rw-r--r--   0        0        0      217 2023-01-25 16:53:45.717030 increase-0.5.0/src/increase/types/entities/__init__.py
--rw-r--r--   0        0        0      343 2023-01-25 16:53:45.717085 increase-0.5.0/src/increase/types/entities/supplemental_document_create_params.py
--rw-r--r--   0        0        0    11352 2023-03-15 18:51:50.427708 increase-0.5.0/src/increase/types/entity.py
--rw-r--r--   0        0        0    25685 2023-03-15 18:51:50.427853 increase-0.5.0/src/increase/types/entity_create_params.py
--rw-r--r--   0        0        0      404 2023-01-25 16:53:45.717436 increase-0.5.0/src/increase/types/entity_list_params.py
--rw-r--r--   0        0        0     2660 2023-03-15 18:51:50.427956 increase-0.5.0/src/increase/types/event.py
--rw-r--r--   0        0        0     3964 2023-03-15 18:51:50.428034 increase-0.5.0/src/increase/types/event_list_params.py
--rw-r--r--   0        0        0     3052 2023-03-15 18:51:50.428121 increase-0.5.0/src/increase/types/event_subscription.py
--rw-r--r--   0        0        0     2462 2023-03-15 18:51:50.428224 increase-0.5.0/src/increase/types/event_subscription_create_params.py
--rw-r--r--   0        0        0      426 2023-01-25 16:53:45.717897 increase-0.5.0/src/increase/types/event_subscription_list_params.py
--rw-r--r--   0        0        0      360 2023-01-25 16:53:45.717992 increase-0.5.0/src/increase/types/event_subscription_update_params.py
--rw-r--r--   0        0        0     1205 2023-03-15 18:51:50.428325 increase-0.5.0/src/increase/types/external_account.py
--rw-r--r--   0        0        0      706 2023-01-25 16:53:45.718164 increase-0.5.0/src/increase/types/external_account_create_params.py
--rw-r--r--   0        0        0      700 2023-03-15 18:51:50.428440 increase-0.5.0/src/increase/types/external_account_list_params.py
--rw-r--r--   0        0        0      420 2023-03-15 18:51:50.428551 increase-0.5.0/src/increase/types/external_account_update_params.py
--rw-r--r--   0        0        0     1500 2023-03-15 18:51:50.428657 increase-0.5.0/src/increase/types/file.py
--rw-r--r--   0        0        0     1009 2023-01-25 16:53:45.718498 increase-0.5.0/src/increase/types/file_create_params.py
--rw-r--r--   0        0        0     2058 2023-03-15 18:51:50.428762 increase-0.5.0/src/increase/types/file_list_params.py
--rw-r--r--   0        0        0      738 2023-03-15 18:51:50.428864 increase-0.5.0/src/increase/types/group.py
--rw-r--r--   0        0        0     1693 2023-03-15 18:51:50.428939 increase-0.5.0/src/increase/types/inbound_ach_transfer_return.py
--rw-r--r--   0        0        0     1109 2023-03-15 18:51:50.429004 increase-0.5.0/src/increase/types/inbound_ach_transfer_return_create_params.py
--rw-r--r--   0        0        0      440 2023-03-15 18:51:50.429062 increase-0.5.0/src/increase/types/inbound_ach_transfer_return_list_params.py
--rw-r--r--   0        0        0     2916 2023-03-15 18:51:50.429124 increase-0.5.0/src/increase/types/inbound_wire_drawdown_request.py
--rw-r--r--   0        0        0      444 2023-03-15 18:51:50.429189 increase-0.5.0/src/increase/types/inbound_wire_drawdown_request_list_params.py
--rw-r--r--   0        0        0     1041 2023-01-25 16:53:45.718754 increase-0.5.0/src/increase/types/limit.py
--rw-r--r--   0        0        0      696 2023-01-25 16:53:45.718845 increase-0.5.0/src/increase/types/limit_create_params.py
--rw-r--r--   0        0        0      527 2023-01-25 16:53:45.718920 increase-0.5.0/src/increase/types/limit_list_params.py
--rw-r--r--   0        0        0      332 2023-01-25 16:53:45.718997 increase-0.5.0/src/increase/types/limit_update_params.py
--rw-r--r--   0        0        0      779 2023-03-15 18:51:50.429277 increase-0.5.0/src/increase/types/oauth_connection.py
--rw-r--r--   0        0        0      422 2023-01-25 16:53:45.719145 increase-0.5.0/src/increase/types/oauth_connection_list_params.py
--rw-r--r--   0        0        0    11929 2023-03-15 18:51:50.429408 increase-0.5.0/src/increase/types/pending_transaction.py
--rw-r--r--   0        0        0     1010 2023-03-15 18:51:50.429504 increase-0.5.0/src/increase/types/pending_transaction_list_params.py
--rw-r--r--   0        0        0     6113 2023-03-15 18:51:50.429630 increase-0.5.0/src/increase/types/real_time_decision.py
--rw-r--r--   0        0        0     2451 2023-03-15 18:51:50.429740 increase-0.5.0/src/increase/types/real_time_decision_action_params.py
--rw-r--r--   0        0        0      895 2023-01-25 16:53:45.719648 increase-0.5.0/src/increase/types/routing_number.py
--rw-r--r--   0        0        0      522 2023-01-25 16:53:45.719742 increase-0.5.0/src/increase/types/routing_number_list_params.py
--rw-r--r--   0        0        0      155 2023-03-15 18:51:50.429835 increase-0.5.0/src/increase/types/shared/__init__.py
--rw-r--r--   0        0        0      525 2023-03-15 18:51:50.429902 increase-0.5.0/src/increase/types/shared/point_of_service_entry_mode.py
--rw-r--r--   0        0        0      155 2023-03-15 18:51:50.429999 increase-0.5.0/src/increase/types/shared_params/__init__.py
--rw-r--r--   0        0        0      525 2023-03-15 18:51:50.430063 increase-0.5.0/src/increase/types/shared_params/point_of_service_entry_mode.py
--rw-r--r--   0        0        0     2041 2023-03-15 18:51:50.430236 increase-0.5.0/src/increase/types/simulations/__init__.py
--rw-r--r--   0        0        0      338 2023-01-25 16:53:45.719932 increase-0.5.0/src/increase/types/simulations/account_statement_create_params.py
--rw-r--r--   0        0        0     1027 2023-01-25 16:53:45.720024 increase-0.5.0/src/increase/types/simulations/ach_transfer_create_inbound_params.py
--rw-r--r--   0        0        0     1317 2023-01-25 16:53:45.720077 increase-0.5.0/src/increase/types/simulations/ach_transfer_return_params.py
--rw-r--r--   0        0        0    48383 2023-03-15 18:51:50.430584 increase-0.5.0/src/increase/types/simulations/ach_transfer_simulation.py
--rw-r--r--   0        0        0    25926 2023-03-15 18:51:50.430698 increase-0.5.0/src/increase/types/simulations/card_authorization_simulation.py
--rw-r--r--   0        0        0      477 2023-01-25 16:53:45.720909 increase-0.5.0/src/increase/types/simulations/card_authorize_params.py
--rw-r--r--   0        0        0      443 2023-01-25 16:53:45.720968 increase-0.5.0/src/increase/types/simulations/card_dispute_action_params.py
--rw-r--r--   0        0        0      400 2023-01-25 16:53:45.721022 increase-0.5.0/src/increase/types/simulations/card_refund_create_params.py
--rw-r--r--   0        0        0      610 2023-01-25 16:53:45.721121 increase-0.5.0/src/increase/types/simulations/card_settlement_params.py
--rw-r--r--   0        0        0      346 2023-01-25 16:53:45.721224 increase-0.5.0/src/increase/types/simulations/digital_wallet_token_request_create_params.py
--rw-r--r--   0        0        0      953 2023-01-25 16:53:45.721286 increase-0.5.0/src/increase/types/simulations/digital_wallet_token_request_create_response.py
--rw-r--r--   0        0        0      325 2023-01-25 16:53:45.721340 increase-0.5.0/src/increase/types/simulations/document_create_params.py
--rw-r--r--   0        0        0    48554 2023-03-15 18:51:50.430910 increase-0.5.0/src/increase/types/simulations/inbound_real_time_payments_transfer_simulation_result.py
--rw-r--r--   0        0        0     2648 2023-03-15 18:51:50.430998 increase-0.5.0/src/increase/types/simulations/inbound_wire_drawdown_request_create_params.py
--rw-r--r--   0        0        0     1020 2023-01-25 16:53:45.721579 increase-0.5.0/src/increase/types/simulations/real_time_payments_transfer_create_inbound_params.py
--rw-r--r--   0        0        0     2591 2023-01-25 16:53:45.721689 increase-0.5.0/src/increase/types/simulations/wire_transfer_create_inbound_params.py
--rw-r--r--   0        0        0    35557 2023-03-15 18:51:50.431137 increase-0.5.0/src/increase/types/simulations/wire_transfer_simulation.py
--rw-r--r--   0        0        0    33872 2023-03-15 18:51:50.431336 increase-0.5.0/src/increase/types/transaction.py
--rw-r--r--   0        0        0     3522 2023-03-15 18:51:50.431475 increase-0.5.0/src/increase/types/transaction_list_params.py
--rw-r--r--   0        0        0     2239 2023-03-15 18:51:50.431583 increase-0.5.0/src/increase/types/wire_drawdown_request.py
--rw-r--r--   0        0        0     1148 2023-01-25 16:53:45.722263 increase-0.5.0/src/increase/types/wire_drawdown_request_create_params.py
--rw-r--r--   0        0        0      430 2023-01-25 16:53:45.722365 increase-0.5.0/src/increase/types/wire_drawdown_request_list_params.py
--rw-r--r--   0        0        0     4817 2023-03-15 18:51:50.431699 increase-0.5.0/src/increase/types/wire_transfer.py
--rw-r--r--   0        0        0     1367 2023-01-25 16:53:45.722596 increase-0.5.0/src/increase/types/wire_transfer_create_params.py
--rw-r--r--   0        0        0     1588 2023-03-15 18:51:50.431795 increase-0.5.0/src/increase/types/wire_transfer_list_params.py
--rw-r--r--   0        0        0     9793 1970-01-01 00:00:00.000000 increase-0.5.0/setup.py
--rw-r--r--   0        0        0     9339 1970-01-01 00:00:00.000000 increase-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11338 2023-05-31 10:09:43.188289 increase-0.6.0/LICENSE
+-rw-r--r--   0        0        0     8443 2023-05-31 10:09:43.188289 increase-0.6.0/README.md
+-rw-r--r--   0        0        0     1883 2023-05-31 10:09:43.188289 increase-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2587 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/__init__.py
+-rw-r--r--   0        0        0    46447 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/_base_client.py
+-rw-r--r--   0        0        0     3889 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/_base_exceptions.py
+-rw-r--r--   0        0        0    26766 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/_client.py
+-rw-r--r--   0        0        0    10875 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/_exceptions.py
+-rw-r--r--   0        0        0     7343 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/_models.py
+-rw-r--r--   0        0        0     4781 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/_qs.py
+-rw-r--r--   0        0        0      890 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/_resource.py
+-rw-r--r--   0        0        0     3979 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/_types.py
+-rw-r--r--   0        0        0     1277 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/_utils/__init__.py
+-rw-r--r--   0        0        0     6710 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/_utils/_transform.py
+-rw-r--r--   0        0        0     9411 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/_utils/_utils.py
+-rw-r--r--   0        0        0      127 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/_version.py
+-rw-r--r--   0        0        0     1109 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/pagination.py
+-rw-r--r--   0        0        0        0 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/py.typed
+-rw-r--r--   0        0        0     4478 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/resources/__init__.py
+-rw-r--r--   0        0        0    14153 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/resources/account_numbers.py
+-rw-r--r--   0        0        0     6612 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/resources/account_statements.py
+-rw-r--r--   0        0        0    15452 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/resources/account_transfers.py
+-rw-r--r--   0        0        0    16078 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/resources/accounts.py
+-rw-r--r--   0        0        0    14804 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/resources/ach_prenotifications.py
+-rw-r--r--   0        0        0    23469 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/resources/ach_transfers.py
+-rw-r--r--   0        0        0     4285 2023-05-31 10:09:43.188289 increase-0.6.0/src/increase/resources/balance_lookups.py
+-rw-r--r--   0        0        0     8651 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/bookkeeping_accounts.py
+-rw-r--r--   0        0        0     4122 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/bookkeeping_entries.py
+-rw-r--r--   0        0        0     4842 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/bookkeeping_entry_sets.py
+-rw-r--r--   0        0        0     9963 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/card_disputes.py
+-rw-r--r--   0        0        0     9853 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/card_profiles.py
+-rw-r--r--   0        0        0    17566 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/cards.py
+-rw-r--r--   0        0        0    10985 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/check_deposits.py
+-rw-r--r--   0        0        0    19654 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/check_transfers.py
+-rw-r--r--   0        0        0     6995 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/declined_transactions.py
+-rw-r--r--   0        0        0     6577 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/digital_wallet_tokens.py
+-rw-r--r--   0        0        0     6425 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/documents.py
+-rw-r--r--   0        0        0      282 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/entities/__init__.py
+-rw-r--r--   0        0        0    13266 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/entities/entities.py
+-rw-r--r--   0        0        0     3839 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/entities/supplemental_documents.py
+-rw-r--r--   0        0        0    17879 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/event_subscriptions.py
+-rw-r--r--   0        0        0     6438 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/events.py
+-rw-r--r--   0        0        0     9804 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/exports.py
+-rw-r--r--   0        0        0    14425 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/external_accounts.py
+-rw-r--r--   0        0        0    12069 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/files.py
+-rw-r--r--   0        0        0     2040 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/groups.py
+-rw-r--r--   0        0        0    11207 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/inbound_ach_transfer_returns.py
+-rw-r--r--   0        0        0     6239 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/inbound_wire_drawdown_requests.py
+-rw-r--r--   0        0        0    13407 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/limits.py
+-rw-r--r--   0        0        0     5833 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/oauth_connections.py
+-rw-r--r--   0        0        0     7572 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/pending_transactions.py
+-rw-r--r--   0        0        0     5552 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/programs.py
+-rw-r--r--   0        0        0     7616 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/real_time_decisions.py
+-rw-r--r--   0        0        0    14164 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/real_time_payments_transfers.py
+-rw-r--r--   0        0        0     4951 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/routing_numbers.py
+-rw-r--r--   0        0        0     1906 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/simulations/__init__.py
+-rw-r--r--   0        0        0     4026 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/simulations/account_statements.py
+-rw-r--r--   0        0        0     3102 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/simulations/account_transfers.py
+-rw-r--r--   0        0        0    16455 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/simulations/ach_transfers.py
+-rw-r--r--   0        0        0     4919 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/simulations/card_disputes.py
+-rw-r--r--   0        0        0     3967 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/simulations/card_refunds.py
+-rw-r--r--   0        0        0    11463 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/simulations/cards.py
+-rw-r--r--   0        0        0     7407 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/simulations/check_deposits.py
+-rw-r--r--   0        0        0     8993 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/simulations/check_transfers.py
+-rw-r--r--   0        0        0     4085 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/simulations/digital_wallet_token_requests.py
+-rw-r--r--   0        0        0     3639 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/simulations/documents.py
+-rw-r--r--   0        0        0    13466 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/simulations/inbound_wire_drawdown_requests.py
+-rw-r--r--   0        0        0     4411 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/simulations/interest_payments.py
+-rw-r--r--   0        0        0    11027 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/simulations/real_time_payments_transfers.py
+-rw-r--r--   0        0        0     4404 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/simulations/simulations.py
+-rw-r--r--   0        0        0    12351 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/simulations/wire_transfers.py
+-rw-r--r--   0        0        0     7036 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/transactions.py
+-rw-r--r--   0        0        0    12534 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/wire_drawdown_requests.py
+-rw-r--r--   0        0        0    23155 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/resources/wire_transfers.py
+-rw-r--r--   0        0        0     8739 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/types/__init__.py
+-rw-r--r--   0        0        0     1452 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/types/account.py
+-rw-r--r--   0        0        0      690 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/types/account_create_params.py
+-rw-r--r--   0        0        0     1571 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/types/account_list_params.py
+-rw-r--r--   0        0        0     1026 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/types/account_number.py
+-rw-r--r--   0        0        0      408 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/types/account_number_create_params.py
+-rw-r--r--   0        0        0     1598 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/types/account_number_list_params.py
+-rw-r--r--   0        0        0      435 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/types/account_number_update_params.py
+-rw-r--r--   0        0        0     1347 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/types/account_statement.py
+-rw-r--r--   0        0        0     1534 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/types/account_statement_list_params.py
+-rw-r--r--   0        0        0     2648 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/types/account_transfer.py
+-rw-r--r--   0        0        0      814 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/types/account_transfer_create_params.py
+-rw-r--r--   0        0        0     1494 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/types/account_transfer_list_params.py
+-rw-r--r--   0        0        0      271 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/types/account_update_params.py
+-rw-r--r--   0        0        0     2152 2023-05-31 10:09:43.192289 increase-0.6.0/src/increase/types/ach_prenotification.py
+-rw-r--r--   0        0        0     1847 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/ach_prenotification_create_params.py
+-rw-r--r--   0        0        0     1391 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/ach_prenotification_list_params.py
+-rw-r--r--   0        0        0     6791 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/ach_transfer.py
+-rw-r--r--   0        0        0     3388 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/ach_transfer_create_params.py
+-rw-r--r--   0        0        0     1592 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/ach_transfer_list_params.py
+-rw-r--r--   0        0        0      585 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/balance_lookup_lookup_params.py
+-rw-r--r--   0        0        0      780 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/balance_lookup_lookup_response.py
+-rw-r--r--   0        0        0      823 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/bookkeeping_account.py
+-rw-r--r--   0        0        0      626 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/bookkeeping_account_create_params.py
+-rw-r--r--   0        0        0      428 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/bookkeeping_account_list_params.py
+-rw-r--r--   0        0        0      698 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/bookkeeping_entry.py
+-rw-r--r--   0        0        0      424 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/bookkeeping_entry_list_params.py
+-rw-r--r--   0        0        0      895 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/bookkeeping_entry_set.py
+-rw-r--r--   0        0        0     1133 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/bookkeeping_entry_set_create_params.py
+-rw-r--r--   0        0        0     2342 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/card.py
+-rw-r--r--   0        0        0     1767 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/card_create_params.py
+-rw-r--r--   0        0        0      907 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/card_details.py
+-rw-r--r--   0        0        0     2011 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/card_dispute.py
+-rw-r--r--   0        0        0      483 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/card_dispute_create_params.py
+-rw-r--r--   0        0        0     1661 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/card_dispute_list_params.py
+-rw-r--r--   0        0        0     1451 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/card_list_params.py
+-rw-r--r--   0        0        0     2186 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/card_profile.py
+-rw-r--r--   0        0        0     1820 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/card_profile_create_params.py
+-rw-r--r--   0        0        0      715 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/card_profile_list_params.py
+-rw-r--r--   0        0        0     1619 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/card_update_params.py
+-rw-r--r--   0        0        0     4861 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/check_deposit.py
+-rw-r--r--   0        0        0      748 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/check_deposit_create_params.py
+-rw-r--r--   0        0        0     1477 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/check_deposit_list_params.py
+-rw-r--r--   0        0        0     6608 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/check_transfer.py
+-rw-r--r--   0        0        0     1939 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/check_transfer_create_params.py
+-rw-r--r--   0        0        0     1488 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/check_transfer_list_params.py
+-rw-r--r--   0        0        0    13910 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/declined_transaction.py
+-rw-r--r--   0        0        0     1598 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/declined_transaction_list_params.py
+-rw-r--r--   0        0        0      950 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/digital_wallet_token.py
+-rw-r--r--   0        0        0     1489 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/digital_wallet_token_list_params.py
+-rw-r--r--   0        0        0     2581 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/document.py
+-rw-r--r--   0        0        0     3899 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/document_list_params.py
+-rw-r--r--   0        0        0      217 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/entities/__init__.py
+-rw-r--r--   0        0        0      343 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/entities/supplemental_document_create_params.py
+-rw-r--r--   0        0        0    11352 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/entity.py
+-rw-r--r--   0        0        0    25685 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/entity_create_params.py
+-rw-r--r--   0        0        0     1367 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/entity_list_params.py
+-rw-r--r--   0        0        0     2724 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/event.py
+-rw-r--r--   0        0        0     4044 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/event_list_params.py
+-rw-r--r--   0        0        0     3124 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/event_subscription.py
+-rw-r--r--   0        0        0     2526 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/event_subscription_create_params.py
+-rw-r--r--   0        0        0      426 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/event_subscription_list_params.py
+-rw-r--r--   0        0        0      360 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/event_subscription_update_params.py
+-rw-r--r--   0        0        0     1147 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/export.py
+-rw-r--r--   0        0        0     2946 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/export_create_params.py
+-rw-r--r--   0        0        0      404 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/export_list_params.py
+-rw-r--r--   0        0        0     1205 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/external_account.py
+-rw-r--r--   0        0        0      706 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/external_account_create_params.py
+-rw-r--r--   0        0        0      700 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/external_account_list_params.py
+-rw-r--r--   0        0        0      420 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/external_account_update_params.py
+-rw-r--r--   0        0        0     1546 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/file.py
+-rw-r--r--   0        0        0     1041 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/file_create_params.py
+-rw-r--r--   0        0        0     2120 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/file_list_params.py
+-rw-r--r--   0        0        0      738 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/group.py
+-rw-r--r--   0        0        0     1693 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/inbound_ach_transfer_return.py
+-rw-r--r--   0        0        0     1109 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/inbound_ach_transfer_return_create_params.py
+-rw-r--r--   0        0        0      440 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/inbound_ach_transfer_return_list_params.py
+-rw-r--r--   0        0        0     2916 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/inbound_wire_drawdown_request.py
+-rw-r--r--   0        0        0      444 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/inbound_wire_drawdown_request_list_params.py
+-rw-r--r--   0        0        0     1041 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/limit.py
+-rw-r--r--   0        0        0      696 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/limit_create_params.py
+-rw-r--r--   0        0        0      527 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/limit_list_params.py
+-rw-r--r--   0        0        0      332 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/limit_update_params.py
+-rw-r--r--   0        0        0      779 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/oauth_connection.py
+-rw-r--r--   0        0        0      422 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/oauth_connection_list_params.py
+-rw-r--r--   0        0        0    13613 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/pending_transaction.py
+-rw-r--r--   0        0        0     1955 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/pending_transaction_list_params.py
+-rw-r--r--   0        0        0      735 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/program.py
+-rw-r--r--   0        0        0      406 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/program_list_params.py
+-rw-r--r--   0        0        0     6113 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/real_time_decision.py
+-rw-r--r--   0        0        0     2451 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/real_time_decision_action_params.py
+-rw-r--r--   0        0        0     5096 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/real_time_payments_transfer.py
+-rw-r--r--   0        0        0     1283 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/real_time_payments_transfer_create_params.py
+-rw-r--r--   0        0        0     1664 2023-05-31 10:09:43.196289 increase-0.6.0/src/increase/types/real_time_payments_transfer_list_params.py
+-rw-r--r--   0        0        0      895 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/routing_number.py
+-rw-r--r--   0        0        0      522 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/routing_number_list_params.py
+-rw-r--r--   0        0        0      155 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/shared/__init__.py
+-rw-r--r--   0        0        0      489 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/shared/point_of_service_entry_mode.py
+-rw-r--r--   0        0        0      155 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/shared_params/__init__.py
+-rw-r--r--   0        0        0      525 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/shared_params/point_of_service_entry_mode.py
+-rw-r--r--   0        0        0     2530 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/__init__.py
+-rw-r--r--   0        0        0      338 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/account_statement_create_params.py
+-rw-r--r--   0        0        0     1027 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/ach_transfer_create_inbound_params.py
+-rw-r--r--   0        0        0     1317 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/ach_transfer_return_params.py
+-rw-r--r--   0        0        0    54696 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/ach_transfer_simulation.py
+-rw-r--r--   0        0        0    29427 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/card_authorization_simulation.py
+-rw-r--r--   0        0        0      823 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/card_authorize_params.py
+-rw-r--r--   0        0        0      443 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/card_dispute_action_params.py
+-rw-r--r--   0        0        0      400 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/card_refund_create_params.py
+-rw-r--r--   0        0        0      610 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/card_settlement_params.py
+-rw-r--r--   0        0        0      425 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/check_transfer_return_params.py
+-rw-r--r--   0        0        0      346 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/digital_wallet_token_request_create_params.py
+-rw-r--r--   0        0        0      953 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/digital_wallet_token_request_create_response.py
+-rw-r--r--   0        0        0      325 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/document_create_params.py
+-rw-r--r--   0        0        0    54867 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/inbound_real_time_payments_transfer_simulation_result.py
+-rw-r--r--   0        0        0     2648 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/inbound_wire_drawdown_request_create_params.py
+-rw-r--r--   0        0        0      435 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/interest_payment_create_params.py
+-rw-r--r--   0        0        0    40063 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/interest_payment_simulation_result.py
+-rw-r--r--   0        0        0     1362 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/real_time_payments_transfer_complete_params.py
+-rw-r--r--   0        0        0     1020 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/real_time_payments_transfer_create_inbound_params.py
+-rw-r--r--   0        0        0     2591 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/wire_transfer_create_inbound_params.py
+-rw-r--r--   0        0        0    40107 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/simulations/wire_transfer_simulation.py
+-rw-r--r--   0        0        0    38323 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/transaction.py
+-rw-r--r--   0        0        0     3652 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/transaction_list_params.py
+-rw-r--r--   0        0        0     2239 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/wire_drawdown_request.py
+-rw-r--r--   0        0        0     1148 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/wire_drawdown_request_create_params.py
+-rw-r--r--   0        0        0      430 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/wire_drawdown_request_list_params.py
+-rw-r--r--   0        0        0     5343 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/wire_transfer.py
+-rw-r--r--   0        0        0     1367 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/wire_transfer_create_params.py
+-rw-r--r--   0        0        0     1588 2023-05-31 10:09:43.200289 increase-0.6.0/src/increase/types/wire_transfer_list_params.py
+-rw-r--r--   0        0        0     9346 1970-01-01 00:00:00.000000 increase-0.6.0/PKG-INFO
```

### Comparing `increase-0.5.0/LICENSE` & `increase-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/README.md` & `increase-0.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -124,31 +124,31 @@
 Or just work directly with the returned data:
 
 ```python
 first_page = await increase.accounts.list()
 
 print(f"next page cursor: {first_page.next_cursor}")  # => "next page cursor: ..."
 for account in first_page.data:
-    print(account.balances)
+    print(account.created_at)
 
 # Remove `await` for non-async usage.
 ```
 
 ## Nested params
 
 Nested parameters are dictionaries, typed using `TypedDict`, for example:
 
-```py
+```python
 from increase import Increase
 
 increase = Increase()
 
 increase.accounts.create(
     foo={
-        "bar": True
+        "bar": True,
     },
 )
 ```
 
 ## File Uploads
 
 Request parameters that correspond to file uploads can be passed as `bytes` or a tuple of `(filename, contents, media type)`.
```

### Comparing `increase-0.5.0/pyproject.toml` & `increase-0.6.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "increase"
-version = "0.5.0"
+version = "0.6.0"
 description = "Client library for the increase API"
 readme = "README.md"
 authors = ["Increase <dev-feedback@increase.com>"]
 license = "Apache-2.0"
 repository = "https://github.com/increase/increase-python"
 packages = [
   { include = "increase", from = "src" }
@@ -14,25 +14,27 @@
 python = "^3.7"
 httpx = ">= 0.23.0"
 pydantic = ">= 1.9.0"
 typing-extensions = ">= 4.1.1"
 anyio = ">= 3.5.0"
 distro = ">= 1.7.0"
 
+
 [tool.poetry.group.dev.dependencies]
-pyright = "^1.1.297"
-mypy = "^1.1.1"
-black = "^22.1.0"
-respx = "^0.19.2"
-pytest = "^7.1.1"
-pytest-asyncio = "^0.18.3"
-ruff = "^0.0.239"
+pyright = "1.1.297"
+mypy = "1.1.1"
+black = "22.10.0"
+respx = "0.19.2"
+pytest = "7.1.1"
+pytest-asyncio = "0.18.3"
+ruff = "0.0.239"
 isort = "5.10.1"
 time-machine = "^2.9.0"
 
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
 target-version = ["py37"]
@@ -40,14 +42,17 @@
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 addopts = "--tb=short"
 xfail_strict = true
 log_cli = true
 log_level = "INFO"
 asyncio_mode = "auto"
+filterwarnings = [
+  "error"
+]
 
 [tool.pyright]
 # this enables practically every flag given by pyright.
 # there are a couple of flags that are still disabled by
 # default in strict mode as they are experimental and niche.
 typeCheckingMode = "strict"
 pythonVersion = "3.7"
```

### Comparing `increase-0.5.0/src/increase/__init__.py` & `increase-0.6.0/src/increase/__init__.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/_base_client.py` & `increase-0.6.0/src/increase/_base_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,18 +123,26 @@
 
     def __iter(self) -> Iterator[ResponseT]:
         cast_to = self._cast_to
         response = self.response
         process_line = self._client._process_stream_line
         process_data = self._client._process_response_data
 
+        awaiting_ping_data = False
         for raw_line in response.iter_lines():
             if not raw_line or raw_line == "\n":
                 continue
 
+            if raw_line.startswith("event: ping"):
+                awaiting_ping_data = True
+                continue
+            if awaiting_ping_data:
+                awaiting_ping_data = False
+                continue
+
             try:
                 line = process_line(raw_line)
             except StopStreaming:
                 # we are done!
                 break
 
             yield process_data(data=json.loads(line), cast_to=cast_to, response=response)
@@ -164,18 +172,26 @@
 
     async def __iter(self) -> AsyncIterator[ResponseT]:
         cast_to = self._cast_to
         response = self.response
         process_line = self._client._process_stream_line
         process_data = self._client._process_response_data
 
+        awaiting_ping_data = False
         async for raw_line in response.aiter_lines():
             if not raw_line or raw_line == "\n":
                 continue
 
+            if raw_line.startswith("event: ping"):
+                awaiting_ping_data = True
+                continue
+            if awaiting_ping_data:
+                awaiting_ping_data = False
+                continue
+
             try:
                 line = process_line(raw_line)
             except StopStreaming:
                 # we are done!
                 break
 
             yield process_data(data=json.loads(line), cast_to=cast_to, response=response)
@@ -462,14 +478,23 @@
             if not options.idempotency_key:
                 options.idempotency_key = self._idempotency_key()
 
             headers[idempotency_header] = options.idempotency_key
 
         return headers
 
+    def _prepare_request(self, request: httpx.Request) -> None:
+        """This method is used as a callback for mutating the `Request` object
+        after it has been constructed.
+
+        This is useful for cases where you want to add certain headers based off of
+        the request properties, e.g. `url`, `method` etc.
+        """
+        return None
+
     def _build_request(
         self,
         options: FinalRequestOptions,
     ) -> httpx.Request:
         headers = self._build_headers(options)
 
         kwargs: dict[str, Any] = {}
@@ -499,28 +524,30 @@
                 if not is_dict(json_data):
                     raise TypeError(
                         f"Expected query input to be a dictionary for multipart requests but got {type(json_data)} instead."
                     )
                 kwargs["data"] = self._serialize_multipartform(json_data)
 
         # TODO: report this error to httpx
-        return self._client.build_request(  # pyright: ignore[reportUnknownMemberType]
+        request = self._client.build_request(  # pyright: ignore[reportUnknownMemberType]
             headers=headers,
             timeout=self.timeout if isinstance(options.timeout, NotGiven) else options.timeout,
             method=options.method,
             url=options.url,
             # the `Query` type that we use is incompatible with qs'
             # `Params` type as it needs to be typed as `Mapping[str, object]`
             # so that passing a `TypedDict` doesn't cause an error.
             # https://github.com/microsoft/pyright/issues/3526#event-6715453066
             params=self.qs.stringify(cast(Mapping[str, Any], params)) if params else None,
             json=json_data,
             files=options.files,
             **kwargs,
         )
+        self._prepare_request(request)
+        return request
 
     def _serialize_multipartform(self, data: Mapping[object, object]) -> dict[str, object]:
         items = self.qs.stringify_items(
             # TODO: type ignore is required as stringify_items is well typed but we can't be
             # well typed without heavy validation.
             data,  # type: ignore
             array_format="brackets",
@@ -606,15 +633,15 @@
         if self._strict_response_validation:
             return cast(ResponseT, validate_type(type_=cast_to, value=data))
 
         return cast(ResponseT, construct_type(type_=cast_to, value=data))
 
     def _process_stream_line(self, contents: str) -> str:
         """Pre-process an indiviudal line from a streaming response"""
-        if contents == "data: [DONE]\n":
+        if contents.startswith("data: [DONE]"):
             raise StopStreaming()
 
         if contents.startswith("data: "):
             return contents[6:]
 
         return contents
 
@@ -623,19 +650,19 @@
         return Querystring()
 
     @property
     def custom_auth(self) -> httpx.Auth | None:
         return None
 
     @property
-    def auth_headers(self) -> Dict[str, str]:
+    def auth_headers(self) -> dict[str, str]:
         return {}
 
     @property
-    def default_headers(self) -> Dict[str, str]:
+    def default_headers(self) -> dict[str, str | Omit]:
         return {
             "Content-Type": "application/json",
             "User-Agent": self.user_agent,
             **self.platform_headers(),
             **self.auth_headers,
             **self._custom_headers,
         }
@@ -1279,14 +1306,15 @@
 def make_request_options(
     *,
     query: Query | None = None,
     extra_headers: Headers | None = None,
     extra_query: Query | None = None,
     extra_body: Body | None = None,
     idempotency_key: str | None = None,
+    timeout: float | None | NotGiven = NOT_GIVEN,
 ) -> RequestOptions:
     """Create a dict of type RequestOptions without keys of NotGiven values."""
     options: RequestOptions = {}
     if extra_headers is not None:
         options["headers"] = extra_headers
 
     if extra_body is not None:
@@ -1294,14 +1322,17 @@
 
     if query is not None:
         options["params"] = query
 
     if extra_query is not None:
         options["params"] = {**options.get("params", {}), **extra_query}
 
+    if not isinstance(timeout, NotGiven):
+        options["timeout"] = timeout
+
     if idempotency_key is not None:
         options["idempotency_key"] = idempotency_key
 
     return options
 
 
 class OtherPlatform:
```

### Comparing `increase-0.5.0/src/increase/_base_exceptions.py` & `increase-0.6.0/src/increase/_base_exceptions.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/_client.py` & `increase-0.6.0/src/increase/_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,22 +44,29 @@
     "sandbox": "https://sandbox.increase.com",
 }
 
 
 class Increase(SyncAPIClient):
     accounts: resources.Accounts
     account_numbers: resources.AccountNumbers
+    bookkeeping_accounts: resources.BookkeepingAccounts
+    bookkeeping_entry_sets: resources.BookkeepingEntrySets
+    bookkeeping_entries: resources.BookkeepingEntries
     real_time_decisions: resources.RealTimeDecisions
+    real_time_payments_transfers: resources.RealTimePaymentsTransfers
+    balance_lookups: resources.BalanceLookups
     cards: resources.Cards
     card_disputes: resources.CardDisputes
     card_profiles: resources.CardProfiles
     external_accounts: resources.ExternalAccounts
+    exports: resources.Exports
     digital_wallet_tokens: resources.DigitalWalletTokens
     transactions: resources.Transactions
     pending_transactions: resources.PendingTransactions
+    programs: resources.Programs
     declined_transactions: resources.DeclinedTransactions
     limits: resources.Limits
     account_transfers: resources.AccountTransfers
     ach_transfers: resources.ACHTransfers
     inbound_ach_transfer_returns: resources.InboundACHTransferReturns
     ach_prenotifications: resources.ACHPrenotifications
     documents: resources.Documents
@@ -142,22 +149,29 @@
 
         self.api_key = api_key
 
         self._idempotency_header = "Idempotency-Key"
 
         self.accounts = resources.Accounts(self)
         self.account_numbers = resources.AccountNumbers(self)
+        self.bookkeeping_accounts = resources.BookkeepingAccounts(self)
+        self.bookkeeping_entry_sets = resources.BookkeepingEntrySets(self)
+        self.bookkeeping_entries = resources.BookkeepingEntries(self)
         self.real_time_decisions = resources.RealTimeDecisions(self)
+        self.real_time_payments_transfers = resources.RealTimePaymentsTransfers(self)
+        self.balance_lookups = resources.BalanceLookups(self)
         self.cards = resources.Cards(self)
         self.card_disputes = resources.CardDisputes(self)
         self.card_profiles = resources.CardProfiles(self)
         self.external_accounts = resources.ExternalAccounts(self)
+        self.exports = resources.Exports(self)
         self.digital_wallet_tokens = resources.DigitalWalletTokens(self)
         self.transactions = resources.Transactions(self)
         self.pending_transactions = resources.PendingTransactions(self)
+        self.programs = resources.Programs(self)
         self.declined_transactions = resources.DeclinedTransactions(self)
         self.limits = resources.Limits(self)
         self.account_transfers = resources.AccountTransfers(self)
         self.ach_transfers = resources.ACHTransfers(self)
         self.inbound_ach_transfer_returns = resources.InboundACHTransferReturns(self)
         self.ach_prenotifications = resources.ACHPrenotifications(self)
         self.documents = resources.Documents(self)
@@ -177,16 +191,17 @@
         self.simulations = resources.Simulations(self)
 
     @property
     def qs(self) -> Querystring:
         return Querystring(nested_format="dots", array_format="comma")
 
     @property
-    def auth_headers(self) -> Dict[str, str]:
-        return {"Authorization": f"Bearer {self.api_key}"}
+    def auth_headers(self) -> dict[str, str]:
+        api_key = self.api_key
+        return {"Authorization": f"Bearer {api_key}"}
 
     def copy(
         self,
         *,
         api_key: str | None = None,
         environment: Literal["production", "sandbox"] | None = None,
         base_url: str | None = None,
@@ -304,22 +319,29 @@
             )
         return super()._make_status_error(err_msg, request=request, response=response, body=body)
 
 
 class AsyncIncrease(AsyncAPIClient):
     accounts: resources.AsyncAccounts
     account_numbers: resources.AsyncAccountNumbers
+    bookkeeping_accounts: resources.AsyncBookkeepingAccounts
+    bookkeeping_entry_sets: resources.AsyncBookkeepingEntrySets
+    bookkeeping_entries: resources.AsyncBookkeepingEntries
     real_time_decisions: resources.AsyncRealTimeDecisions
+    real_time_payments_transfers: resources.AsyncRealTimePaymentsTransfers
+    balance_lookups: resources.AsyncBalanceLookups
     cards: resources.AsyncCards
     card_disputes: resources.AsyncCardDisputes
     card_profiles: resources.AsyncCardProfiles
     external_accounts: resources.AsyncExternalAccounts
+    exports: resources.AsyncExports
     digital_wallet_tokens: resources.AsyncDigitalWalletTokens
     transactions: resources.AsyncTransactions
     pending_transactions: resources.AsyncPendingTransactions
+    programs: resources.AsyncPrograms
     declined_transactions: resources.AsyncDeclinedTransactions
     limits: resources.AsyncLimits
     account_transfers: resources.AsyncAccountTransfers
     ach_transfers: resources.AsyncACHTransfers
     inbound_ach_transfer_returns: resources.AsyncInboundACHTransferReturns
     ach_prenotifications: resources.AsyncACHPrenotifications
     documents: resources.AsyncDocuments
@@ -402,22 +424,29 @@
 
         self.api_key = api_key
 
         self._idempotency_header = "Idempotency-Key"
 
         self.accounts = resources.AsyncAccounts(self)
         self.account_numbers = resources.AsyncAccountNumbers(self)
+        self.bookkeeping_accounts = resources.AsyncBookkeepingAccounts(self)
+        self.bookkeeping_entry_sets = resources.AsyncBookkeepingEntrySets(self)
+        self.bookkeeping_entries = resources.AsyncBookkeepingEntries(self)
         self.real_time_decisions = resources.AsyncRealTimeDecisions(self)
+        self.real_time_payments_transfers = resources.AsyncRealTimePaymentsTransfers(self)
+        self.balance_lookups = resources.AsyncBalanceLookups(self)
         self.cards = resources.AsyncCards(self)
         self.card_disputes = resources.AsyncCardDisputes(self)
         self.card_profiles = resources.AsyncCardProfiles(self)
         self.external_accounts = resources.AsyncExternalAccounts(self)
+        self.exports = resources.AsyncExports(self)
         self.digital_wallet_tokens = resources.AsyncDigitalWalletTokens(self)
         self.transactions = resources.AsyncTransactions(self)
         self.pending_transactions = resources.AsyncPendingTransactions(self)
+        self.programs = resources.AsyncPrograms(self)
         self.declined_transactions = resources.AsyncDeclinedTransactions(self)
         self.limits = resources.AsyncLimits(self)
         self.account_transfers = resources.AsyncAccountTransfers(self)
         self.ach_transfers = resources.AsyncACHTransfers(self)
         self.inbound_ach_transfer_returns = resources.AsyncInboundACHTransferReturns(self)
         self.ach_prenotifications = resources.AsyncACHPrenotifications(self)
         self.documents = resources.AsyncDocuments(self)
@@ -437,16 +466,17 @@
         self.simulations = resources.AsyncSimulations(self)
 
     @property
     def qs(self) -> Querystring:
         return Querystring(nested_format="dots", array_format="comma")
 
     @property
-    def auth_headers(self) -> Dict[str, str]:
-        return {"Authorization": f"Bearer {self.api_key}"}
+    def auth_headers(self) -> dict[str, str]:
+        api_key = self.api_key
+        return {"Authorization": f"Bearer {api_key}"}
 
     def copy(
         self,
         *,
         api_key: str | None = None,
         environment: Literal["production", "sandbox"] | None = None,
         base_url: str | None = None,
```

### Comparing `increase-0.5.0/src/increase/_exceptions.py` & `increase-0.6.0/src/increase/_exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,23 +48,23 @@
     "RateLimitedError",
 ]
 
 
 class InvalidParametersError(exceptions.BadRequestError):
     detail: Optional[str]
 
+    errors: List[object]
+    """All errors related to parsing the request parameters."""
+
     status: Literal[400]
 
     title: str
 
     type: Literal["invalid_parameters_error"]
 
-    errors: Optional[List[object]]
-    """All errors related to parsing the request parameters."""
-
     def __init__(self, message: str, *, body: object, request: httpx.Request, response: httpx.Response) -> None:
         data = cast(Mapping[str, object], body if is_mapping(body) else {})
         title = cast(Any, data.get("title"))
         super().__init__(title or message, request=request, response=response, body=body)
 
         self.type = cast(Any, data.get("type"))
         self.title = cast(Any, data.get("title"))
```

### Comparing `increase-0.5.0/src/increase/_models.py` & `increase-0.6.0/src/increase/_models.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/_qs.py` & `increase-0.6.0/src/increase/_qs.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/_resource.py` & `increase-0.6.0/src/increase/_resource.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/_types.py` & `increase-0.6.0/src/increase/_types.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/_utils/__init__.py` & `increase-0.6.0/src/increase/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/_utils/_transform.py` & `increase-0.6.0/src/increase/_utils/_transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 def _maybe_transform_key(key: str, type_: type) -> str:
     annotated_type = _get_annoted_type(type_)
     if annotated_type is None:
         # no `Annotated` definition for this type, no transformation needed
         return key
 
     # ignore the first argument as it is the actual type
-    annotations = get_args(type_)[1:]
+    annotations = get_args(annotated_type)[1:]
     for annotation in annotations:
         if isinstance(annotation, PropertyInfo) and annotation.alias is not None:
             return annotation.alias
 
     return key
```

### Comparing `increase-0.5.0/src/increase/_utils/_utils.py` & `increase-0.6.0/src/increase/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/pagination.py` & `increase-0.6.0/src/increase/pagination.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/resources/account_numbers.py` & `increase-0.6.0/src/increase/resources/account_numbers.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         account_id: str,
         name: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> AccountNumber:
         """
         Create an Account Number
 
         Args:
           account_id: The Account the Account Number should belong to.
@@ -42,14 +43,16 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             "/account_numbers",
             body=maybe_transform(
                 {
                     "account_id": account_id,
@@ -57,47 +60,52 @@
                 },
                 account_number_create_params.AccountNumberCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=AccountNumber,
         )
 
     def retrieve(
         self,
         account_number_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> AccountNumber:
         """Retrieve an Account Number"""
         return self._get(
             f"/account_numbers/{account_number_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=AccountNumber,
         )
 
     def update(
         self,
         account_number_id: str,
         *,
         name: str | NotGiven = NOT_GIVEN,
         status: Literal["active", "disabled", "canceled"] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> AccountNumber:
         """
         Update an Account Number
 
         Args:
           name: The name you choose for the Account Number.
@@ -106,14 +114,16 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._patch(
             f"/account_numbers/{account_number_id}",
             body=maybe_transform(
                 {
                     "name": name,
@@ -121,31 +131,34 @@
                 },
                 account_number_update_params.AccountNumberUpdateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=AccountNumber,
         )
 
     def list(
         self,
         *,
         account_id: str | NotGiven = NOT_GIVEN,
+        created_at: account_number_list_params.CreatedAt | NotGiven = NOT_GIVEN,
         cursor: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         status: Literal["active", "disabled", "canceled"] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> SyncPage[AccountNumber]:
         """
         List Account Numbers
 
         Args:
           account_id: Filter Account Numbers to those belonging to the specified Account.
 
@@ -157,28 +170,32 @@
           status: The status to retrieve Account Numbers for.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/account_numbers",
             page=SyncPage[AccountNumber],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                         "status": status,
                         "account_id": account_id,
+                        "created_at": created_at,
                     },
                     account_number_list_params.AccountNumberListParams,
                 ),
             ),
             model=AccountNumber,
         )
 
@@ -190,14 +207,15 @@
         account_id: str,
         name: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> AccountNumber:
         """
         Create an Account Number
 
         Args:
           account_id: The Account the Account Number should belong to.
@@ -206,14 +224,16 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             "/account_numbers",
             body=maybe_transform(
                 {
                     "account_id": account_id,
@@ -221,47 +241,52 @@
                 },
                 account_number_create_params.AccountNumberCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=AccountNumber,
         )
 
     async def retrieve(
         self,
         account_number_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> AccountNumber:
         """Retrieve an Account Number"""
         return await self._get(
             f"/account_numbers/{account_number_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=AccountNumber,
         )
 
     async def update(
         self,
         account_number_id: str,
         *,
         name: str | NotGiven = NOT_GIVEN,
         status: Literal["active", "disabled", "canceled"] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> AccountNumber:
         """
         Update an Account Number
 
         Args:
           name: The name you choose for the Account Number.
@@ -270,14 +295,16 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._patch(
             f"/account_numbers/{account_number_id}",
             body=maybe_transform(
                 {
                     "name": name,
@@ -285,31 +312,34 @@
                 },
                 account_number_update_params.AccountNumberUpdateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=AccountNumber,
         )
 
     def list(
         self,
         *,
         account_id: str | NotGiven = NOT_GIVEN,
+        created_at: account_number_list_params.CreatedAt | NotGiven = NOT_GIVEN,
         cursor: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         status: Literal["active", "disabled", "canceled"] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> AsyncPaginator[AccountNumber, AsyncPage[AccountNumber]]:
         """
         List Account Numbers
 
         Args:
           account_id: Filter Account Numbers to those belonging to the specified Account.
 
@@ -321,27 +351,31 @@
           status: The status to retrieve Account Numbers for.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/account_numbers",
             page=AsyncPage[AccountNumber],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                         "status": status,
                         "account_id": account_id,
+                        "created_at": created_at,
                     },
                     account_number_list_params.AccountNumberListParams,
                 ),
             ),
             model=AccountNumber,
         )
```

### Comparing `increase-0.5.0/src/increase/resources/account_statements.py` & `increase-0.6.0/src/increase/resources/account_statements.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,19 +18,22 @@
         account_statement_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> AccountStatement:
         """Retrieve an Account Statement"""
         return self._get(
             f"/account_statements/{account_statement_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=AccountStatement,
         )
 
     def list(
         self,
         *,
         account_id: str | NotGiven = NOT_GIVEN,
@@ -38,14 +41,15 @@
         limit: int | NotGiven = NOT_GIVEN,
         statement_period_start: account_statement_list_params.StatementPeriodStart | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> SyncPage[AccountStatement]:
         """
         List Account Statements
 
         Args:
           account_id: Filter Account Statements to those belonging to the specified Account.
 
@@ -55,22 +59,25 @@
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/account_statements",
             page=SyncPage[AccountStatement],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                         "account_id": account_id,
                         "statement_period_start": statement_period_start,
                     },
@@ -87,19 +94,22 @@
         account_statement_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> AccountStatement:
         """Retrieve an Account Statement"""
         return await self._get(
             f"/account_statements/{account_statement_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=AccountStatement,
         )
 
     def list(
         self,
         *,
         account_id: str | NotGiven = NOT_GIVEN,
@@ -107,14 +117,15 @@
         limit: int | NotGiven = NOT_GIVEN,
         statement_period_start: account_statement_list_params.StatementPeriodStart | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> AsyncPaginator[AccountStatement, AsyncPage[AccountStatement]]:
         """
         List Account Statements
 
         Args:
           account_id: Filter Account Statements to those belonging to the specified Account.
 
@@ -124,22 +135,25 @@
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/account_statements",
             page=AsyncPage[AccountStatement],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                         "account_id": account_id,
                         "statement_period_start": statement_period_start,
                     },
```

### Comparing `increase-0.5.0/src/increase/resources/account_transfers.py` & `increase-0.6.0/src/increase/resources/external_accounts.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,364 +1,383 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
+from typing_extensions import Literal
+
 from ..types import (
-    AccountTransfer,
-    account_transfer_list_params,
-    account_transfer_create_params,
+    ExternalAccount,
+    external_account_list_params,
+    external_account_create_params,
+    external_account_update_params,
 )
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from .._utils import maybe_transform
 from .._resource import SyncAPIResource, AsyncAPIResource
 from ..pagination import SyncPage, AsyncPage
 from .._base_client import AsyncPaginator, make_request_options
 
-__all__ = ["AccountTransfers", "AsyncAccountTransfers"]
+__all__ = ["ExternalAccounts", "AsyncExternalAccounts"]
 
 
-class AccountTransfers(SyncAPIResource):
+class ExternalAccounts(SyncAPIResource):
     def create(
         self,
         *,
-        account_id: str,
-        amount: int,
+        account_number: str,
         description: str,
-        destination_account_id: str,
-        require_approval: bool | NotGiven = NOT_GIVEN,
+        routing_number: str,
+        funding: Literal["checking", "savings", "other"] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
-    ) -> AccountTransfer:
+    ) -> ExternalAccount:
         """
-        Create an Account Transfer
+        Create an External Account
 
         Args:
-          account_id: The identifier for the account that will send the transfer.
-
-          amount: The transfer amount in the minor unit of the account currency. For dollars, for
-              example, this is cents.
+          account_number: The account number for the destination account.
 
-          description: The description you choose to give the transfer.
+          description: The name you choose for the Account.
 
-          destination_account_id: The identifier for the account that will receive the transfer.
+          routing_number: The American Bankers' Association (ABA) Routing Transit Number (RTN) for the
+              destination account.
 
-          require_approval: Whether the transfer requires explicit approval via the dashboard or API.
+          funding: The type of the destination account. Defaults to `checking`.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
-            "/account_transfers",
+            "/external_accounts",
             body=maybe_transform(
                 {
-                    "account_id": account_id,
-                    "amount": amount,
+                    "routing_number": routing_number,
+                    "account_number": account_number,
+                    "funding": funding,
                     "description": description,
-                    "destination_account_id": destination_account_id,
-                    "require_approval": require_approval,
                 },
-                account_transfer_create_params.AccountTransferCreateParams,
+                external_account_create_params.ExternalAccountCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
-            cast_to=AccountTransfer,
+            cast_to=ExternalAccount,
         )
 
     def retrieve(
         self,
-        account_transfer_id: str,
+        external_account_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
-    ) -> AccountTransfer:
-        """Retrieve an Account Transfer"""
+        timeout: float | None | NotGiven = NOT_GIVEN,
+    ) -> ExternalAccount:
+        """Retrieve an External Account"""
         return self._get(
-            f"/account_transfers/{account_transfer_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
-            cast_to=AccountTransfer,
+            f"/external_accounts/{external_account_id}",
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
+            cast_to=ExternalAccount,
+        )
+
+    def update(
+        self,
+        external_account_id: str,
+        *,
+        description: str | NotGiven = NOT_GIVEN,
+        status: Literal["active", "archived"] | NotGiven = NOT_GIVEN,
+        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
+        # The extra values given here take precedence over values defined on the client or passed to this method.
+        extra_headers: Headers | None = None,
+        extra_query: Query | None = None,
+        extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
+        idempotency_key: str | None = None,
+    ) -> ExternalAccount:
+        """
+        Update an External Account
+
+        Args:
+          description: The description you choose to give the external account.
+
+          status: The status of the External Account.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
+        """
+        return self._patch(
+            f"/external_accounts/{external_account_id}",
+            body=maybe_transform(
+                {
+                    "description": description,
+                    "status": status,
+                },
+                external_account_update_params.ExternalAccountUpdateParams,
+            ),
+            options=make_request_options(
+                extra_headers=extra_headers,
+                extra_query=extra_query,
+                extra_body=extra_body,
+                timeout=timeout,
+                idempotency_key=idempotency_key,
+            ),
+            cast_to=ExternalAccount,
         )
 
     def list(
         self,
         *,
-        account_id: str | NotGiven = NOT_GIVEN,
-        created_at: account_transfer_list_params.CreatedAt | NotGiven = NOT_GIVEN,
         cursor: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
+        status: external_account_list_params.Status | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
-    ) -> SyncPage[AccountTransfer]:
+        timeout: float | None | NotGiven = NOT_GIVEN,
+    ) -> SyncPage[ExternalAccount]:
         """
-        List Account Transfers
+        List External Accounts
 
         Args:
-          account_id: Filter Account Transfers to those that originated from the specified Account.
-
           cursor: Return the page of entries after this one.
 
           limit: Limit the size of the list that is returned. The default (and maximum) is 100
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
-            "/account_transfers",
-            page=SyncPage[AccountTransfer],
+            "/external_accounts",
+            page=SyncPage[ExternalAccount],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
-                        "account_id": account_id,
-                        "created_at": created_at,
+                        "status": status,
                     },
-                    account_transfer_list_params.AccountTransferListParams,
+                    external_account_list_params.ExternalAccountListParams,
                 ),
             ),
-            model=AccountTransfer,
+            model=ExternalAccount,
         )
 
-    def approve(
+
+class AsyncExternalAccounts(AsyncAPIResource):
+    async def create(
         self,
-        account_transfer_id: str,
         *,
+        account_number: str,
+        description: str,
+        routing_number: str,
+        funding: Literal["checking", "savings", "other"] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
-    ) -> AccountTransfer:
-        """Approve an Account Transfer"""
-        return self._post(
-            f"/account_transfers/{account_transfer_id}/approve",
+    ) -> ExternalAccount:
+        """
+        Create an External Account
+
+        Args:
+          account_number: The account number for the destination account.
+
+          description: The name you choose for the Account.
+
+          routing_number: The American Bankers' Association (ABA) Routing Transit Number (RTN) for the
+              destination account.
+
+          funding: The type of the destination account. Defaults to `checking`.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
+        """
+        return await self._post(
+            "/external_accounts",
+            body=maybe_transform(
+                {
+                    "routing_number": routing_number,
+                    "account_number": account_number,
+                    "funding": funding,
+                    "description": description,
+                },
+                external_account_create_params.ExternalAccountCreateParams,
+            ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
-            cast_to=AccountTransfer,
+            cast_to=ExternalAccount,
         )
 
-    def cancel(
+    async def retrieve(
         self,
-        account_transfer_id: str,
+        external_account_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
-        idempotency_key: str | None = None,
-    ) -> AccountTransfer:
-        """Cancel an Account Transfer"""
-        return self._post(
-            f"/account_transfers/{account_transfer_id}/cancel",
+        timeout: float | None | NotGiven = NOT_GIVEN,
+    ) -> ExternalAccount:
+        """Retrieve an External Account"""
+        return await self._get(
+            f"/external_accounts/{external_account_id}",
             options=make_request_options(
-                extra_headers=extra_headers,
-                extra_query=extra_query,
-                extra_body=extra_body,
-                idempotency_key=idempotency_key,
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=AccountTransfer,
+            cast_to=ExternalAccount,
         )
 
-
-class AsyncAccountTransfers(AsyncAPIResource):
-    async def create(
+    async def update(
         self,
+        external_account_id: str,
         *,
-        account_id: str,
-        amount: int,
-        description: str,
-        destination_account_id: str,
-        require_approval: bool | NotGiven = NOT_GIVEN,
+        description: str | NotGiven = NOT_GIVEN,
+        status: Literal["active", "archived"] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
-    ) -> AccountTransfer:
+    ) -> ExternalAccount:
         """
-        Create an Account Transfer
+        Update an External Account
 
         Args:
-          account_id: The identifier for the account that will send the transfer.
+          description: The description you choose to give the external account.
 
-          amount: The transfer amount in the minor unit of the account currency. For dollars, for
-              example, this is cents.
-
-          description: The description you choose to give the transfer.
-
-          destination_account_id: The identifier for the account that will receive the transfer.
-
-          require_approval: Whether the transfer requires explicit approval via the dashboard or API.
+          status: The status of the External Account.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
-        return await self._post(
-            "/account_transfers",
+        return await self._patch(
+            f"/external_accounts/{external_account_id}",
             body=maybe_transform(
                 {
-                    "account_id": account_id,
-                    "amount": amount,
                     "description": description,
-                    "destination_account_id": destination_account_id,
-                    "require_approval": require_approval,
+                    "status": status,
                 },
-                account_transfer_create_params.AccountTransferCreateParams,
+                external_account_update_params.ExternalAccountUpdateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
-            cast_to=AccountTransfer,
-        )
-
-    async def retrieve(
-        self,
-        account_transfer_id: str,
-        *,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-    ) -> AccountTransfer:
-        """Retrieve an Account Transfer"""
-        return await self._get(
-            f"/account_transfers/{account_transfer_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
-            cast_to=AccountTransfer,
+            cast_to=ExternalAccount,
         )
 
     def list(
         self,
         *,
-        account_id: str | NotGiven = NOT_GIVEN,
-        created_at: account_transfer_list_params.CreatedAt | NotGiven = NOT_GIVEN,
         cursor: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
+        status: external_account_list_params.Status | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
-    ) -> AsyncPaginator[AccountTransfer, AsyncPage[AccountTransfer]]:
+        timeout: float | None | NotGiven = NOT_GIVEN,
+    ) -> AsyncPaginator[ExternalAccount, AsyncPage[ExternalAccount]]:
         """
-        List Account Transfers
+        List External Accounts
 
         Args:
-          account_id: Filter Account Transfers to those that originated from the specified Account.
-
           cursor: Return the page of entries after this one.
 
           limit: Limit the size of the list that is returned. The default (and maximum) is 100
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
-            "/account_transfers",
-            page=AsyncPage[AccountTransfer],
+            "/external_accounts",
+            page=AsyncPage[ExternalAccount],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
-                        "account_id": account_id,
-                        "created_at": created_at,
+                        "status": status,
                     },
-                    account_transfer_list_params.AccountTransferListParams,
+                    external_account_list_params.ExternalAccountListParams,
                 ),
             ),
-            model=AccountTransfer,
-        )
-
-    async def approve(
-        self,
-        account_transfer_id: str,
-        *,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        idempotency_key: str | None = None,
-    ) -> AccountTransfer:
-        """Approve an Account Transfer"""
-        return await self._post(
-            f"/account_transfers/{account_transfer_id}/approve",
-            options=make_request_options(
-                extra_headers=extra_headers,
-                extra_query=extra_query,
-                extra_body=extra_body,
-                idempotency_key=idempotency_key,
-            ),
-            cast_to=AccountTransfer,
-        )
-
-    async def cancel(
-        self,
-        account_transfer_id: str,
-        *,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        idempotency_key: str | None = None,
-    ) -> AccountTransfer:
-        """Cancel an Account Transfer"""
-        return await self._post(
-            f"/account_transfers/{account_transfer_id}/cancel",
-            options=make_request_options(
-                extra_headers=extra_headers,
-                extra_query=extra_query,
-                extra_body=extra_body,
-                idempotency_key=idempotency_key,
-            ),
-            cast_to=AccountTransfer,
+            model=ExternalAccount,
         )
```

### Comparing `increase-0.5.0/src/increase/resources/accounts.py` & `increase-0.6.0/src/increase/resources/accounts.py`

 * *Files 21% similar despite different names*

```diff
@@ -22,126 +22,143 @@
 class Accounts(SyncAPIResource):
     def create(
         self,
         *,
         name: str,
         entity_id: str | NotGiven = NOT_GIVEN,
         informational_entity_id: str | NotGiven = NOT_GIVEN,
+        program_id: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> Account:
         """
         Create an Account
 
         Args:
           name: The name you choose for the Account.
 
           entity_id: The identifier for the Entity that will own the Account.
 
           informational_entity_id: The identifier of an Entity that, while not owning the Account, is associated
               with its activity. Its relationship to your group must be `informational`.
 
+          program_id: The identifier for the Program that this Account falls under.
+
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             "/accounts",
             body=maybe_transform(
                 {
                     "entity_id": entity_id,
+                    "program_id": program_id,
                     "informational_entity_id": informational_entity_id,
                     "name": name,
                 },
                 account_create_params.AccountCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=Account,
         )
 
     def retrieve(
         self,
         account_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> Account:
         """Retrieve an Account"""
         return self._get(
             f"/accounts/{account_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=Account,
         )
 
     def update(
         self,
         account_id: str,
         *,
         name: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> Account:
         """
         Update an Account
 
         Args:
           name: The new name of the Account.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._patch(
             f"/accounts/{account_id}",
             body=maybe_transform({"name": name}, account_update_params.AccountUpdateParams),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=Account,
         )
 
     def list(
         self,
         *,
+        created_at: account_list_params.CreatedAt | NotGiven = NOT_GIVEN,
         cursor: str | NotGiven = NOT_GIVEN,
         entity_id: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         status: Literal["open", "closed"] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> SyncPage[Account]:
         """
         List Accounts
 
         Args:
           cursor: Return the page of entries after this one.
 
@@ -153,28 +170,32 @@
           status: Filter Accounts for those with the specified status.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/accounts",
             page=SyncPage[Account],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                         "entity_id": entity_id,
                         "status": status,
+                        "created_at": created_at,
                     },
                     account_list_params.AccountListParams,
                 ),
             ),
             model=Account,
         )
 
@@ -183,148 +204,167 @@
         account_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> Account:
         """Close an Account"""
         return self._post(
             f"/accounts/{account_id}/close",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=Account,
         )
 
 
 class AsyncAccounts(AsyncAPIResource):
     async def create(
         self,
         *,
         name: str,
         entity_id: str | NotGiven = NOT_GIVEN,
         informational_entity_id: str | NotGiven = NOT_GIVEN,
+        program_id: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> Account:
         """
         Create an Account
 
         Args:
           name: The name you choose for the Account.
 
           entity_id: The identifier for the Entity that will own the Account.
 
           informational_entity_id: The identifier of an Entity that, while not owning the Account, is associated
               with its activity. Its relationship to your group must be `informational`.
 
+          program_id: The identifier for the Program that this Account falls under.
+
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             "/accounts",
             body=maybe_transform(
                 {
                     "entity_id": entity_id,
+                    "program_id": program_id,
                     "informational_entity_id": informational_entity_id,
                     "name": name,
                 },
                 account_create_params.AccountCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=Account,
         )
 
     async def retrieve(
         self,
         account_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> Account:
         """Retrieve an Account"""
         return await self._get(
             f"/accounts/{account_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=Account,
         )
 
     async def update(
         self,
         account_id: str,
         *,
         name: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> Account:
         """
         Update an Account
 
         Args:
           name: The new name of the Account.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._patch(
             f"/accounts/{account_id}",
             body=maybe_transform({"name": name}, account_update_params.AccountUpdateParams),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=Account,
         )
 
     def list(
         self,
         *,
+        created_at: account_list_params.CreatedAt | NotGiven = NOT_GIVEN,
         cursor: str | NotGiven = NOT_GIVEN,
         entity_id: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         status: Literal["open", "closed"] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> AsyncPaginator[Account, AsyncPage[Account]]:
         """
         List Accounts
 
         Args:
           cursor: Return the page of entries after this one.
 
@@ -336,28 +376,32 @@
           status: Filter Accounts for those with the specified status.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/accounts",
             page=AsyncPage[Account],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                         "entity_id": entity_id,
                         "status": status,
+                        "created_at": created_at,
                     },
                     account_list_params.AccountListParams,
                 ),
             ),
             model=Account,
         )
 
@@ -366,20 +410,22 @@
         account_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> Account:
         """Close an Account"""
         return await self._post(
             f"/accounts/{account_id}/close",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=Account,
         )
```

### Comparing `increase-0.5.0/src/increase/resources/ach_prenotifications.py` & `increase-0.6.0/src/increase/resources/ach_prenotifications.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         ]
         | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> ACHPrenotification:
         """
         Create an ACH Prenotification
 
         Args:
           account_number: The account number for the destination account.
@@ -79,14 +80,16 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             "/ach_prenotifications",
             body=maybe_transform(
                 {
                     "account_number": account_number,
@@ -104,47 +107,52 @@
                 },
                 ach_prenotification_create_params.ACHPrenotificationCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=ACHPrenotification,
         )
 
     def retrieve(
         self,
         ach_prenotification_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> ACHPrenotification:
         """Retrieve an ACH Prenotification"""
         return self._get(
             f"/ach_prenotifications/{ach_prenotification_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=ACHPrenotification,
         )
 
     def list(
         self,
         *,
         created_at: ach_prenotification_list_params.CreatedAt | NotGiven = NOT_GIVEN,
         cursor: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> SyncPage[ACHPrenotification]:
         """
         List ACH Prenotifications
 
         Args:
           cursor: Return the page of entries after this one.
 
@@ -152,22 +160,25 @@
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/ach_prenotifications",
             page=SyncPage[ACHPrenotification],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                         "created_at": created_at,
                     },
                     ach_prenotification_list_params.ACHPrenotificationListParams,
@@ -197,14 +208,15 @@
         ]
         | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> ACHPrenotification:
         """
         Create an ACH Prenotification
 
         Args:
           account_number: The account number for the destination account.
@@ -236,14 +248,16 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             "/ach_prenotifications",
             body=maybe_transform(
                 {
                     "account_number": account_number,
@@ -261,47 +275,52 @@
                 },
                 ach_prenotification_create_params.ACHPrenotificationCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=ACHPrenotification,
         )
 
     async def retrieve(
         self,
         ach_prenotification_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> ACHPrenotification:
         """Retrieve an ACH Prenotification"""
         return await self._get(
             f"/ach_prenotifications/{ach_prenotification_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=ACHPrenotification,
         )
 
     def list(
         self,
         *,
         created_at: ach_prenotification_list_params.CreatedAt | NotGiven = NOT_GIVEN,
         cursor: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> AsyncPaginator[ACHPrenotification, AsyncPage[ACHPrenotification]]:
         """
         List ACH Prenotifications
 
         Args:
           cursor: Return the page of entries after this one.
 
@@ -309,22 +328,25 @@
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/ach_prenotifications",
             page=AsyncPage[ACHPrenotification],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                         "created_at": created_at,
                     },
                     ach_prenotification_list_params.ACHPrenotificationListParams,
```

### Comparing `increase-0.5.0/src/increase/resources/ach_transfers.py` & `increase-0.6.0/src/increase/resources/ach_transfers.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         ]
         | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> ACHTransfer:
         """
         Create an ACH Transfer
 
         Args:
           account_id: The Increase identifier for the account that will send the transfer.
@@ -65,15 +66,15 @@
               `individual_name` and `company_name` instead of relying on this fallback.
 
           account_number: The account number for the destination account.
 
           addendum: Additional information that will be sent to the recipient. This is included in
               the transfer data sent to the receiving bank.
 
-          company_descriptive_date: The description of the date of the transfer, usually in the format `YYYYMMDD`.
+          company_descriptive_date: The description of the date of the transfer, usually in the format `YYMMDD`.
               This is included in the transfer data sent to the receiving bank.
 
           company_discretionary_data: The data you choose to associate with the transfer. This is included in the
               transfer data sent to the receiving bank.
 
           company_entry_description: A description of the transfer. This is included in the transfer data sent to the
               receiving bank.
@@ -103,14 +104,16 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             "/ach_transfers",
             body=maybe_transform(
                 {
                     "account_id": account_id,
@@ -133,33 +136,37 @@
                 },
                 ach_transfer_create_params.ACHTransferCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=ACHTransfer,
         )
 
     def retrieve(
         self,
         ach_transfer_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> ACHTransfer:
         """Retrieve an ACH Transfer"""
         return self._get(
             f"/ach_transfers/{ach_transfer_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=ACHTransfer,
         )
 
     def list(
         self,
         *,
         account_id: str | NotGiven = NOT_GIVEN,
@@ -168,14 +175,15 @@
         external_account_id: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> SyncPage[ACHTransfer]:
         """
         List ACH Transfers
 
         Args:
           account_id: Filter ACH Transfers to those that originated from the specified Account.
 
@@ -187,22 +195,25 @@
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/ach_transfers",
             page=SyncPage[ACHTransfer],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                         "account_id": account_id,
                         "external_account_id": external_account_id,
                         "created_at": created_at,
@@ -218,46 +229,50 @@
         ach_transfer_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> ACHTransfer:
         """Approves an ACH Transfer in a pending_approval state."""
         return self._post(
             f"/ach_transfers/{ach_transfer_id}/approve",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=ACHTransfer,
         )
 
     def cancel(
         self,
         ach_transfer_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> ACHTransfer:
         """Cancels an ACH Transfer in a pending_approval state."""
         return self._post(
             f"/ach_transfers/{ach_transfer_id}/cancel",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=ACHTransfer,
         )
 
 
 class AsyncACHTransfers(AsyncAPIResource):
@@ -285,14 +300,15 @@
         ]
         | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> ACHTransfer:
         """
         Create an ACH Transfer
 
         Args:
           account_id: The Increase identifier for the account that will send the transfer.
@@ -309,15 +325,15 @@
               `individual_name` and `company_name` instead of relying on this fallback.
 
           account_number: The account number for the destination account.
 
           addendum: Additional information that will be sent to the recipient. This is included in
               the transfer data sent to the receiving bank.
 
-          company_descriptive_date: The description of the date of the transfer, usually in the format `YYYYMMDD`.
+          company_descriptive_date: The description of the date of the transfer, usually in the format `YYMMDD`.
               This is included in the transfer data sent to the receiving bank.
 
           company_discretionary_data: The data you choose to associate with the transfer. This is included in the
               transfer data sent to the receiving bank.
 
           company_entry_description: A description of the transfer. This is included in the transfer data sent to the
               receiving bank.
@@ -347,14 +363,16 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             "/ach_transfers",
             body=maybe_transform(
                 {
                     "account_id": account_id,
@@ -377,33 +395,37 @@
                 },
                 ach_transfer_create_params.ACHTransferCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=ACHTransfer,
         )
 
     async def retrieve(
         self,
         ach_transfer_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> ACHTransfer:
         """Retrieve an ACH Transfer"""
         return await self._get(
             f"/ach_transfers/{ach_transfer_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=ACHTransfer,
         )
 
     def list(
         self,
         *,
         account_id: str | NotGiven = NOT_GIVEN,
@@ -412,14 +434,15 @@
         external_account_id: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> AsyncPaginator[ACHTransfer, AsyncPage[ACHTransfer]]:
         """
         List ACH Transfers
 
         Args:
           account_id: Filter ACH Transfers to those that originated from the specified Account.
 
@@ -431,22 +454,25 @@
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/ach_transfers",
             page=AsyncPage[ACHTransfer],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                         "account_id": account_id,
                         "external_account_id": external_account_id,
                         "created_at": created_at,
@@ -462,43 +488,47 @@
         ach_transfer_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> ACHTransfer:
         """Approves an ACH Transfer in a pending_approval state."""
         return await self._post(
             f"/ach_transfers/{ach_transfer_id}/approve",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=ACHTransfer,
         )
 
     async def cancel(
         self,
         ach_transfer_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> ACHTransfer:
         """Cancels an ACH Transfer in a pending_approval state."""
         return await self._post(
             f"/ach_transfers/{ach_transfer_id}/cancel",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=ACHTransfer,
         )
```

### Comparing `increase-0.5.0/src/increase/resources/card_disputes.py` & `increase-0.6.0/src/increase/resources/card_disputes.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
         disputed_transaction_id: str,
         explanation: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> CardDispute:
         """
         Create a Card Dispute
 
         Args:
           disputed_transaction_id: The Transaction you wish to dispute. This Transaction must have a `source_type`
@@ -36,14 +37,16 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             "/card_disputes",
             body=maybe_transform(
                 {
                     "disputed_transaction_id": disputed_transaction_id,
@@ -51,33 +54,37 @@
                 },
                 card_dispute_create_params.CardDisputeCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=CardDispute,
         )
 
     def retrieve(
         self,
         card_dispute_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> CardDispute:
         """Retrieve a Card Dispute"""
         return self._get(
             f"/card_disputes/{card_dispute_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=CardDispute,
         )
 
     def list(
         self,
         *,
         created_at: card_dispute_list_params.CreatedAt | NotGiven = NOT_GIVEN,
@@ -85,14 +92,15 @@
         limit: int | NotGiven = NOT_GIVEN,
         status: card_dispute_list_params.Status | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> SyncPage[CardDispute]:
         """
         List Card Disputes
 
         Args:
           cursor: Return the page of entries after this one.
 
@@ -100,22 +108,25 @@
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/card_disputes",
             page=SyncPage[CardDispute],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                         "created_at": created_at,
                         "status": status,
                     },
@@ -133,14 +144,15 @@
         disputed_transaction_id: str,
         explanation: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> CardDispute:
         """
         Create a Card Dispute
 
         Args:
           disputed_transaction_id: The Transaction you wish to dispute. This Transaction must have a `source_type`
@@ -150,14 +162,16 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             "/card_disputes",
             body=maybe_transform(
                 {
                     "disputed_transaction_id": disputed_transaction_id,
@@ -165,33 +179,37 @@
                 },
                 card_dispute_create_params.CardDisputeCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=CardDispute,
         )
 
     async def retrieve(
         self,
         card_dispute_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> CardDispute:
         """Retrieve a Card Dispute"""
         return await self._get(
             f"/card_disputes/{card_dispute_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=CardDispute,
         )
 
     def list(
         self,
         *,
         created_at: card_dispute_list_params.CreatedAt | NotGiven = NOT_GIVEN,
@@ -199,14 +217,15 @@
         limit: int | NotGiven = NOT_GIVEN,
         status: card_dispute_list_params.Status | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> AsyncPaginator[CardDispute, AsyncPage[CardDispute]]:
         """
         List Card Disputes
 
         Args:
           cursor: Return the page of entries after this one.
 
@@ -214,22 +233,25 @@
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/card_disputes",
             page=AsyncPage[CardDispute],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                         "created_at": created_at,
                         "status": status,
                     },
```

### Comparing `increase-0.5.0/src/increase/resources/card_profiles.py` & `increase-0.6.0/src/increase/resources/card_profiles.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,14 +19,15 @@
         description: str,
         digital_wallets: card_profile_create_params.DigitalWallets,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> CardProfile:
         """
         Create a Card Profile
 
         Args:
           description: A description you can use to identify the Card Profile.
@@ -36,14 +37,16 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             "/card_profiles",
             body=maybe_transform(
                 {
                     "description": description,
@@ -51,47 +54,52 @@
                 },
                 card_profile_create_params.CardProfileCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=CardProfile,
         )
 
     def retrieve(
         self,
         card_profile_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> CardProfile:
         """Retrieve a Card Profile"""
         return self._get(
             f"/card_profiles/{card_profile_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=CardProfile,
         )
 
     def list(
         self,
         *,
         cursor: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         status: card_profile_list_params.Status | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> SyncPage[CardProfile]:
         """
         List Card Profiles
 
         Args:
           cursor: Return the page of entries after this one.
 
@@ -99,22 +107,25 @@
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/card_profiles",
             page=SyncPage[CardProfile],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                         "status": status,
                     },
                     card_profile_list_params.CardProfileListParams,
@@ -131,14 +142,15 @@
         description: str,
         digital_wallets: card_profile_create_params.DigitalWallets,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> CardProfile:
         """
         Create a Card Profile
 
         Args:
           description: A description you can use to identify the Card Profile.
@@ -148,14 +160,16 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             "/card_profiles",
             body=maybe_transform(
                 {
                     "description": description,
@@ -163,47 +177,52 @@
                 },
                 card_profile_create_params.CardProfileCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=CardProfile,
         )
 
     async def retrieve(
         self,
         card_profile_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> CardProfile:
         """Retrieve a Card Profile"""
         return await self._get(
             f"/card_profiles/{card_profile_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=CardProfile,
         )
 
     def list(
         self,
         *,
         cursor: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         status: card_profile_list_params.Status | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> AsyncPaginator[CardProfile, AsyncPage[CardProfile]]:
         """
         List Card Profiles
 
         Args:
           cursor: Return the page of entries after this one.
 
@@ -211,22 +230,25 @@
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/card_profiles",
             page=AsyncPage[CardProfile],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                         "status": status,
                     },
                     card_profile_list_params.CardProfileListParams,
```

### Comparing `increase-0.5.0/src/increase/resources/cards.py` & `increase-0.6.0/src/increase/resources/cards.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,36 +29,41 @@
         description: str | NotGiven = NOT_GIVEN,
         digital_wallet: card_create_params.DigitalWallet | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> Card:
         """
         Create a Card
 
         Args:
           account_id: The Account the card should belong to.
 
           billing_address: The card's billing address.
 
           description: The description you choose to give the card.
 
           digital_wallet: The contact information used in the two-factor steps for digital wallet card
-              creation. At least one field must be present to complete the digital wallet
-              steps.
+              creation. To add the card to a digital wallet, you may supply an email or phone
+              number with this request. Otherwise, subscribe and then action a Real Time
+              Decision with the category `digital_wallet_token_requested` or
+              `digital_wallet_authentication_requested`.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             "/cards",
             body=maybe_transform(
                 {
                     "account_id": account_id,
@@ -68,33 +73,37 @@
                 },
                 card_create_params.CardCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=Card,
         )
 
     def retrieve(
         self,
         card_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> Card:
         """Retrieve a Card"""
         return self._get(
             f"/cards/{card_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=Card,
         )
 
     def update(
         self,
         card_id: str,
         *,
@@ -103,14 +112,15 @@
         digital_wallet: card_update_params.DigitalWallet | NotGiven = NOT_GIVEN,
         status: Literal["active", "disabled", "canceled"] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> Card:
         """
         Update a Card
 
         Args:
           billing_address: The card's updated billing address.
@@ -125,14 +135,16 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._patch(
             f"/cards/{card_id}",
             body=maybe_transform(
                 {
                     "description": description,
@@ -142,14 +154,15 @@
                 },
                 card_update_params.CardUpdateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=Card,
         )
 
     def list(
         self,
@@ -159,14 +172,15 @@
         cursor: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> SyncPage[Card]:
         """
         List Cards
 
         Args:
           account_id: Filter Cards to ones belonging to the specified Account.
 
@@ -176,22 +190,25 @@
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/cards",
             page=SyncPage[Card],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                         "account_id": account_id,
                         "created_at": created_at,
                     },
@@ -206,19 +223,22 @@
         card_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> CardDetails:
         """Retrieve sensitive details for a Card"""
         return self._get(
             f"/cards/{card_id}/details",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=CardDetails,
         )
 
 
 class AsyncCards(AsyncAPIResource):
     async def create(
         self,
@@ -228,36 +248,41 @@
         description: str | NotGiven = NOT_GIVEN,
         digital_wallet: card_create_params.DigitalWallet | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> Card:
         """
         Create a Card
 
         Args:
           account_id: The Account the card should belong to.
 
           billing_address: The card's billing address.
 
           description: The description you choose to give the card.
 
           digital_wallet: The contact information used in the two-factor steps for digital wallet card
-              creation. At least one field must be present to complete the digital wallet
-              steps.
+              creation. To add the card to a digital wallet, you may supply an email or phone
+              number with this request. Otherwise, subscribe and then action a Real Time
+              Decision with the category `digital_wallet_token_requested` or
+              `digital_wallet_authentication_requested`.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             "/cards",
             body=maybe_transform(
                 {
                     "account_id": account_id,
@@ -267,33 +292,37 @@
                 },
                 card_create_params.CardCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=Card,
         )
 
     async def retrieve(
         self,
         card_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> Card:
         """Retrieve a Card"""
         return await self._get(
             f"/cards/{card_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=Card,
         )
 
     async def update(
         self,
         card_id: str,
         *,
@@ -302,14 +331,15 @@
         digital_wallet: card_update_params.DigitalWallet | NotGiven = NOT_GIVEN,
         status: Literal["active", "disabled", "canceled"] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> Card:
         """
         Update a Card
 
         Args:
           billing_address: The card's updated billing address.
@@ -324,14 +354,16 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._patch(
             f"/cards/{card_id}",
             body=maybe_transform(
                 {
                     "description": description,
@@ -341,14 +373,15 @@
                 },
                 card_update_params.CardUpdateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=Card,
         )
 
     def list(
         self,
@@ -358,14 +391,15 @@
         cursor: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> AsyncPaginator[Card, AsyncPage[Card]]:
         """
         List Cards
 
         Args:
           account_id: Filter Cards to ones belonging to the specified Account.
 
@@ -375,22 +409,25 @@
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/cards",
             page=AsyncPage[Card],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                         "account_id": account_id,
                         "created_at": created_at,
                     },
@@ -405,14 +442,17 @@
         card_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> CardDetails:
         """Retrieve sensitive details for a Card"""
         return await self._get(
             f"/cards/{card_id}/details",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=CardDetails,
         )
```

### Comparing `increase-0.5.0/src/increase/resources/check_deposits.py` & `increase-0.6.0/src/increase/resources/check_deposits.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         currency: str,
         front_image_file_id: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> CheckDeposit:
         """
         Create a Check Deposit
 
         Args:
           account_id: The identifier for the Account to deposit the check in.
@@ -45,14 +46,16 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             "/check_deposits",
             body=maybe_transform(
                 {
                     "account_id": account_id,
@@ -63,33 +66,37 @@
                 },
                 check_deposit_create_params.CheckDepositCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=CheckDeposit,
         )
 
     def retrieve(
         self,
         check_deposit_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> CheckDeposit:
         """Retrieve a Check Deposit"""
         return self._get(
             f"/check_deposits/{check_deposit_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=CheckDeposit,
         )
 
     def list(
         self,
         *,
         account_id: str | NotGiven = NOT_GIVEN,
@@ -97,14 +104,15 @@
         cursor: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> SyncPage[CheckDeposit]:
         """
         List Check Deposits
 
         Args:
           account_id: Filter Check Deposits to those belonging to the specified Account.
 
@@ -114,22 +122,25 @@
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/check_deposits",
             page=SyncPage[CheckDeposit],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                         "account_id": account_id,
                         "created_at": created_at,
                     },
@@ -150,14 +161,15 @@
         currency: str,
         front_image_file_id: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> CheckDeposit:
         """
         Create a Check Deposit
 
         Args:
           account_id: The identifier for the Account to deposit the check in.
@@ -173,14 +185,16 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             "/check_deposits",
             body=maybe_transform(
                 {
                     "account_id": account_id,
@@ -191,33 +205,37 @@
                 },
                 check_deposit_create_params.CheckDepositCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=CheckDeposit,
         )
 
     async def retrieve(
         self,
         check_deposit_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> CheckDeposit:
         """Retrieve a Check Deposit"""
         return await self._get(
             f"/check_deposits/{check_deposit_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=CheckDeposit,
         )
 
     def list(
         self,
         *,
         account_id: str | NotGiven = NOT_GIVEN,
@@ -225,14 +243,15 @@
         cursor: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> AsyncPaginator[CheckDeposit, AsyncPage[CheckDeposit]]:
         """
         List Check Deposits
 
         Args:
           account_id: Filter Check Deposits to those belonging to the specified Account.
 
@@ -242,22 +261,25 @@
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/check_deposits",
             page=AsyncPage[CheckDeposit],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                         "account_id": account_id,
                         "created_at": created_at,
                     },
```

### Comparing `increase-0.5.0/src/increase/resources/check_transfers.py` & `increase-0.6.0/src/increase/resources/check_transfers.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         require_approval: bool | NotGiven = NOT_GIVEN,
         return_address: check_transfer_create_params.ReturnAddress | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> CheckTransfer:
         """
         Create a Check Transfer
 
         Args:
           account_id: The identifier for the account that will send the transfer.
@@ -70,14 +71,16 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             "/check_transfers",
             body=maybe_transform(
                 {
                     "account_id": account_id,
@@ -95,33 +98,37 @@
                 },
                 check_transfer_create_params.CheckTransferCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=CheckTransfer,
         )
 
     def retrieve(
         self,
         check_transfer_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> CheckTransfer:
         """Retrieve a Check Transfer"""
         return self._get(
             f"/check_transfers/{check_transfer_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=CheckTransfer,
         )
 
     def list(
         self,
         *,
         account_id: str | NotGiven = NOT_GIVEN,
@@ -129,14 +136,15 @@
         cursor: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> SyncPage[CheckTransfer]:
         """
         List Check Transfers
 
         Args:
           account_id: Filter Check Transfers to those that originated from the specified Account.
 
@@ -146,22 +154,25 @@
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/check_transfers",
             page=SyncPage[CheckTransfer],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                         "account_id": account_id,
                         "created_at": created_at,
                     },
@@ -176,69 +187,75 @@
         check_transfer_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> CheckTransfer:
         """Approve a Check Transfer"""
         return self._post(
             f"/check_transfers/{check_transfer_id}/approve",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=CheckTransfer,
         )
 
     def cancel(
         self,
         check_transfer_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> CheckTransfer:
         """Cancel a pending Check Transfer"""
         return self._post(
             f"/check_transfers/{check_transfer_id}/cancel",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=CheckTransfer,
         )
 
     def stop_payment(
         self,
         check_transfer_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> CheckTransfer:
         """Request a stop payment on a Check Transfer"""
         return self._post(
             f"/check_transfers/{check_transfer_id}/stop_payment",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=CheckTransfer,
         )
 
 
 class AsyncCheckTransfers(AsyncAPIResource):
@@ -258,14 +275,15 @@
         require_approval: bool | NotGiven = NOT_GIVEN,
         return_address: check_transfer_create_params.ReturnAddress | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> CheckTransfer:
         """
         Create a Check Transfer
 
         Args:
           account_id: The identifier for the account that will send the transfer.
@@ -295,14 +313,16 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             "/check_transfers",
             body=maybe_transform(
                 {
                     "account_id": account_id,
@@ -320,33 +340,37 @@
                 },
                 check_transfer_create_params.CheckTransferCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=CheckTransfer,
         )
 
     async def retrieve(
         self,
         check_transfer_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> CheckTransfer:
         """Retrieve a Check Transfer"""
         return await self._get(
             f"/check_transfers/{check_transfer_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=CheckTransfer,
         )
 
     def list(
         self,
         *,
         account_id: str | NotGiven = NOT_GIVEN,
@@ -354,14 +378,15 @@
         cursor: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> AsyncPaginator[CheckTransfer, AsyncPage[CheckTransfer]]:
         """
         List Check Transfers
 
         Args:
           account_id: Filter Check Transfers to those that originated from the specified Account.
 
@@ -371,22 +396,25 @@
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/check_transfers",
             page=AsyncPage[CheckTransfer],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                         "account_id": account_id,
                         "created_at": created_at,
                     },
@@ -401,66 +429,72 @@
         check_transfer_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> CheckTransfer:
         """Approve a Check Transfer"""
         return await self._post(
             f"/check_transfers/{check_transfer_id}/approve",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=CheckTransfer,
         )
 
     async def cancel(
         self,
         check_transfer_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> CheckTransfer:
         """Cancel a pending Check Transfer"""
         return await self._post(
             f"/check_transfers/{check_transfer_id}/cancel",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=CheckTransfer,
         )
 
     async def stop_payment(
         self,
         check_transfer_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> CheckTransfer:
         """Request a stop payment on a Check Transfer"""
         return await self._post(
             f"/check_transfers/{check_transfer_id}/stop_payment",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=CheckTransfer,
         )
```

### Comparing `increase-0.5.0/src/increase/resources/declined_transactions.py` & `increase-0.6.0/src/increase/resources/declined_transactions.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,19 +18,22 @@
         declined_transaction_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> DeclinedTransaction:
         """Retrieve a Declined Transaction"""
         return self._get(
             f"/declined_transactions/{declined_transaction_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=DeclinedTransaction,
         )
 
     def list(
         self,
         *,
         account_id: str | NotGiven = NOT_GIVEN,
@@ -39,14 +42,15 @@
         limit: int | NotGiven = NOT_GIVEN,
         route_id: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> SyncPage[DeclinedTransaction]:
         """
         List Declined Transactions
 
         Args:
           account_id: Filter Declined Transactions to ones belonging to the specified Account.
 
@@ -58,22 +62,25 @@
           route_id: Filter Declined Transactions to those belonging to the specified route.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/declined_transactions",
             page=SyncPage[DeclinedTransaction],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                         "account_id": account_id,
                         "route_id": route_id,
                         "created_at": created_at,
@@ -91,19 +98,22 @@
         declined_transaction_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> DeclinedTransaction:
         """Retrieve a Declined Transaction"""
         return await self._get(
             f"/declined_transactions/{declined_transaction_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=DeclinedTransaction,
         )
 
     def list(
         self,
         *,
         account_id: str | NotGiven = NOT_GIVEN,
@@ -112,14 +122,15 @@
         limit: int | NotGiven = NOT_GIVEN,
         route_id: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> AsyncPaginator[DeclinedTransaction, AsyncPage[DeclinedTransaction]]:
         """
         List Declined Transactions
 
         Args:
           account_id: Filter Declined Transactions to ones belonging to the specified Account.
 
@@ -131,22 +142,25 @@
           route_id: Filter Declined Transactions to those belonging to the specified route.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/declined_transactions",
             page=AsyncPage[DeclinedTransaction],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                         "account_id": account_id,
                         "route_id": route_id,
                         "created_at": created_at,
```

### Comparing `increase-0.5.0/src/increase/resources/digital_wallet_tokens.py` & `increase-0.6.0/src/increase/resources/digital_wallet_tokens.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,19 +18,22 @@
         digital_wallet_token_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> DigitalWalletToken:
         """Retrieve a Digital Wallet Token"""
         return self._get(
             f"/digital_wallet_tokens/{digital_wallet_token_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=DigitalWalletToken,
         )
 
     def list(
         self,
         *,
         card_id: str | NotGiven = NOT_GIVEN,
@@ -38,14 +41,15 @@
         cursor: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> SyncPage[DigitalWalletToken]:
         """
         List Digital Wallet Tokens
 
         Args:
           card_id: Filter Digital Wallet Tokens to ones belonging to the specified Card.
 
@@ -55,22 +59,25 @@
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/digital_wallet_tokens",
             page=SyncPage[DigitalWalletToken],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                         "card_id": card_id,
                         "created_at": created_at,
                     },
@@ -87,19 +94,22 @@
         digital_wallet_token_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> DigitalWalletToken:
         """Retrieve a Digital Wallet Token"""
         return await self._get(
             f"/digital_wallet_tokens/{digital_wallet_token_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=DigitalWalletToken,
         )
 
     def list(
         self,
         *,
         card_id: str | NotGiven = NOT_GIVEN,
@@ -107,14 +117,15 @@
         cursor: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> AsyncPaginator[DigitalWalletToken, AsyncPage[DigitalWalletToken]]:
         """
         List Digital Wallet Tokens
 
         Args:
           card_id: Filter Digital Wallet Tokens to ones belonging to the specified Card.
 
@@ -124,22 +135,25 @@
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/digital_wallet_tokens",
             page=AsyncPage[DigitalWalletToken],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                         "card_id": card_id,
                         "created_at": created_at,
                     },
```

### Comparing `increase-0.5.0/src/increase/resources/documents.py` & `increase-0.6.0/src/increase/resources/documents.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,19 +18,22 @@
         document_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> Document:
         """Retrieve a Document"""
         return self._get(
             f"/documents/{document_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=Document,
         )
 
     def list(
         self,
         *,
         category: document_list_params.Category | NotGiven = NOT_GIVEN,
@@ -39,14 +42,15 @@
         entity_id: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> SyncPage[Document]:
         """
         List Documents
 
         Args:
           cursor: Return the page of entries after this one.
 
@@ -56,22 +60,25 @@
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/documents",
             page=SyncPage[Document],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                         "entity_id": entity_id,
                         "category": category,
                         "created_at": created_at,
@@ -89,19 +96,22 @@
         document_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> Document:
         """Retrieve a Document"""
         return await self._get(
             f"/documents/{document_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=Document,
         )
 
     def list(
         self,
         *,
         category: document_list_params.Category | NotGiven = NOT_GIVEN,
@@ -110,14 +120,15 @@
         entity_id: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> AsyncPaginator[Document, AsyncPage[Document]]:
         """
         List Documents
 
         Args:
           cursor: Return the page of entries after this one.
 
@@ -127,22 +138,25 @@
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/documents",
             page=AsyncPage[Document],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                         "entity_id": entity_id,
                         "category": category,
                         "created_at": created_at,
```

### Comparing `increase-0.5.0/src/increase/resources/entities/entities.py` & `increase-0.6.0/src/increase/resources/entities/entities.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         supplemental_documents: List[entity_create_params.SupplementalDocument] | NotGiven = NOT_GIVEN,
         trust: entity_create_params.Trust | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> Entity:
         """
         Create an Entity
 
         Args:
           relationship: The relationship between your group and the entity.
@@ -72,14 +73,16 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             "/entities",
             body=maybe_transform(
                 {
                     "structure": structure,
@@ -93,46 +96,52 @@
                 },
                 entity_create_params.EntityCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=Entity,
         )
 
     def retrieve(
         self,
         entity_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> Entity:
         """Retrieve an Entity"""
         return self._get(
             f"/entities/{entity_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=Entity,
         )
 
     def list(
         self,
         *,
+        created_at: entity_list_params.CreatedAt | NotGiven = NOT_GIVEN,
         cursor: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> SyncPage[Entity]:
         """
         List Entities
 
         Args:
           cursor: Return the page of entries after this one.
 
@@ -140,26 +149,30 @@
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/entities",
             page=SyncPage[Entity],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
+                        "created_at": created_at,
                     },
                     entity_list_params.EntityListParams,
                 ),
             ),
             model=Entity,
         )
 
@@ -183,14 +196,15 @@
         supplemental_documents: List[entity_create_params.SupplementalDocument] | NotGiven = NOT_GIVEN,
         trust: entity_create_params.Trust | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> Entity:
         """
         Create an Entity
 
         Args:
           relationship: The relationship between your group and the entity.
@@ -217,14 +231,16 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             "/entities",
             body=maybe_transform(
                 {
                     "structure": structure,
@@ -238,46 +254,52 @@
                 },
                 entity_create_params.EntityCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=Entity,
         )
 
     async def retrieve(
         self,
         entity_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> Entity:
         """Retrieve an Entity"""
         return await self._get(
             f"/entities/{entity_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=Entity,
         )
 
     def list(
         self,
         *,
+        created_at: entity_list_params.CreatedAt | NotGiven = NOT_GIVEN,
         cursor: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> AsyncPaginator[Entity, AsyncPage[Entity]]:
         """
         List Entities
 
         Args:
           cursor: Return the page of entries after this one.
 
@@ -285,25 +307,29 @@
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/entities",
             page=AsyncPage[Entity],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
+                        "created_at": created_at,
                     },
                     entity_list_params.EntityListParams,
                 ),
             ),
             model=Entity,
         )
```

### Comparing `increase-0.5.0/src/increase/resources/entities/supplemental_documents.py` & `increase-0.6.0/src/increase/resources/entities/supplemental_documents.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
 from ...types import Entity
-from ..._types import Body, Query, Headers
+from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from ..._utils import maybe_transform
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ..._base_client import make_request_options
 from ...types.entities import supplemental_document_create_params
 
 __all__ = ["SupplementalDocuments", "AsyncSupplementalDocuments"]
 
@@ -19,39 +19,43 @@
         *,
         file_id: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> Entity:
         """
         Create a supplemental document for an Entity
 
         Args:
           file_id: The identifier of the File containing the document.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             f"/entities/{entity_id}/supplemental_documents",
             body=maybe_transform(
                 {"file_id": file_id}, supplemental_document_create_params.SupplementalDocumentCreateParams
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=Entity,
         )
 
 
 class AsyncSupplementalDocuments(AsyncAPIResource):
@@ -61,36 +65,40 @@
         *,
         file_id: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> Entity:
         """
         Create a supplemental document for an Entity
 
         Args:
           file_id: The identifier of the File containing the document.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             f"/entities/{entity_id}/supplemental_documents",
             body=maybe_transform(
                 {"file_id": file_id}, supplemental_document_create_params.SupplementalDocumentCreateParams
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=Entity,
         )
```

### Comparing `increase-0.5.0/src/increase/resources/event_subscriptions.py` & `increase-0.6.0/src/increase/resources/event_subscriptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,14 +34,16 @@
             "account_transfer.updated",
             "ach_prenotification.created",
             "ach_prenotification.updated",
             "ach_transfer.created",
             "ach_transfer.updated",
             "card.created",
             "card.updated",
+            "card_payment.created",
+            "card_payment.updated",
             "card_dispute.created",
             "card_dispute.updated",
             "check_deposit.created",
             "check_deposit.updated",
             "check_transfer.created",
             "check_transfer.updated",
             "declined_transaction.created",
@@ -77,14 +79,15 @@
         | NotGiven = NOT_GIVEN,
         shared_secret: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> EventSubscription:
         """
         Create an Event Subscription
 
         Args:
           url: The URL you'd like us to send webhooks to.
@@ -97,14 +100,16 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             "/event_subscriptions",
             body=maybe_transform(
                 {
                     "url": url,
@@ -113,69 +118,77 @@
                 },
                 event_subscription_create_params.EventSubscriptionCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=EventSubscription,
         )
 
     def retrieve(
         self,
         event_subscription_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> EventSubscription:
         """Retrieve an Event Subscription"""
         return self._get(
             f"/event_subscriptions/{event_subscription_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=EventSubscription,
         )
 
     def update(
         self,
         event_subscription_id: str,
         *,
         status: Literal["active", "disabled", "deleted"] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> EventSubscription:
         """
         Update an Event Subscription
 
         Args:
           status: The status to update the Event Subscription with.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._patch(
             f"/event_subscriptions/{event_subscription_id}",
             body=maybe_transform({"status": status}, event_subscription_update_params.EventSubscriptionUpdateParams),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=EventSubscription,
         )
 
     def list(
         self,
@@ -183,14 +196,15 @@
         cursor: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> SyncPage[EventSubscription]:
         """
         List Event Subscriptions
 
         Args:
           cursor: Return the page of entries after this one.
 
@@ -198,22 +212,25 @@
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/event_subscriptions",
             page=SyncPage[EventSubscription],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                     },
                     event_subscription_list_params.EventSubscriptionListParams,
                 ),
@@ -237,14 +254,16 @@
             "account_transfer.updated",
             "ach_prenotification.created",
             "ach_prenotification.updated",
             "ach_transfer.created",
             "ach_transfer.updated",
             "card.created",
             "card.updated",
+            "card_payment.created",
+            "card_payment.updated",
             "card_dispute.created",
             "card_dispute.updated",
             "check_deposit.created",
             "check_deposit.updated",
             "check_transfer.created",
             "check_transfer.updated",
             "declined_transaction.created",
@@ -280,14 +299,15 @@
         | NotGiven = NOT_GIVEN,
         shared_secret: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> EventSubscription:
         """
         Create an Event Subscription
 
         Args:
           url: The URL you'd like us to send webhooks to.
@@ -300,14 +320,16 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             "/event_subscriptions",
             body=maybe_transform(
                 {
                     "url": url,
@@ -316,69 +338,77 @@
                 },
                 event_subscription_create_params.EventSubscriptionCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=EventSubscription,
         )
 
     async def retrieve(
         self,
         event_subscription_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> EventSubscription:
         """Retrieve an Event Subscription"""
         return await self._get(
             f"/event_subscriptions/{event_subscription_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=EventSubscription,
         )
 
     async def update(
         self,
         event_subscription_id: str,
         *,
         status: Literal["active", "disabled", "deleted"] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> EventSubscription:
         """
         Update an Event Subscription
 
         Args:
           status: The status to update the Event Subscription with.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._patch(
             f"/event_subscriptions/{event_subscription_id}",
             body=maybe_transform({"status": status}, event_subscription_update_params.EventSubscriptionUpdateParams),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=EventSubscription,
         )
 
     def list(
         self,
@@ -386,14 +416,15 @@
         cursor: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> AsyncPaginator[EventSubscription, AsyncPage[EventSubscription]]:
         """
         List Event Subscriptions
 
         Args:
           cursor: Return the page of entries after this one.
 
@@ -401,22 +432,25 @@
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/event_subscriptions",
             page=AsyncPage[EventSubscription],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                     },
                     event_subscription_list_params.EventSubscriptionListParams,
                 ),
```

### Comparing `increase-0.5.0/src/increase/resources/events.py` & `increase-0.6.0/src/increase/resources/events.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,19 +18,22 @@
         event_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> Event:
         """Retrieve an Event"""
         return self._get(
             f"/events/{event_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=Event,
         )
 
     def list(
         self,
         *,
         associated_object_id: str | NotGiven = NOT_GIVEN,
@@ -39,14 +42,15 @@
         cursor: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> SyncPage[Event]:
         """
         List Events
 
         Args:
           associated_object_id: Filter Events to those belonging to the object with the provided identifier.
 
@@ -56,22 +60,25 @@
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/events",
             page=SyncPage[Event],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                         "associated_object_id": associated_object_id,
                         "created_at": created_at,
                         "category": category,
@@ -89,19 +96,22 @@
         event_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> Event:
         """Retrieve an Event"""
         return await self._get(
             f"/events/{event_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=Event,
         )
 
     def list(
         self,
         *,
         associated_object_id: str | NotGiven = NOT_GIVEN,
@@ -110,14 +120,15 @@
         cursor: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> AsyncPaginator[Event, AsyncPage[Event]]:
         """
         List Events
 
         Args:
           associated_object_id: Filter Events to those belonging to the object with the provided identifier.
 
@@ -127,22 +138,25 @@
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/events",
             page=AsyncPage[Event],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                         "associated_object_id": associated_object_id,
                         "created_at": created_at,
                         "category": category,
```

### Comparing `increase-0.5.0/src/increase/resources/external_accounts.py` & `increase-0.6.0/src/increase/resources/limits.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,353 +1,372 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
 from typing_extensions import Literal
 
-from ..types import (
-    ExternalAccount,
-    external_account_list_params,
-    external_account_create_params,
-    external_account_update_params,
-)
+from ..types import Limit, limit_list_params, limit_create_params, limit_update_params
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from .._utils import maybe_transform
 from .._resource import SyncAPIResource, AsyncAPIResource
 from ..pagination import SyncPage, AsyncPage
 from .._base_client import AsyncPaginator, make_request_options
 
-__all__ = ["ExternalAccounts", "AsyncExternalAccounts"]
+__all__ = ["Limits", "AsyncLimits"]
 
 
-class ExternalAccounts(SyncAPIResource):
+class Limits(SyncAPIResource):
     def create(
         self,
         *,
-        account_number: str,
-        description: str,
-        routing_number: str,
-        funding: Literal["checking", "savings", "other"] | NotGiven = NOT_GIVEN,
+        metric: Literal["count", "volume"],
+        model_id: str,
+        value: int,
+        interval: Literal["transaction", "day", "week", "month", "year", "all_time"] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
-    ) -> ExternalAccount:
+    ) -> Limit:
         """
-        Create an External Account
+        Create a Limit
 
         Args:
-          account_number: The account number for the destination account.
+          metric: The metric for the limit.
 
-          description: The name you choose for the Account.
+          model_id: The identifier of the Account or Account Number you wish to associate the limit
+              with.
 
-          routing_number: The American Bankers' Association (ABA) Routing Transit Number (RTN) for the
-              destination account.
+          value: The value to test the limit against.
 
-          funding: The type of the destination account. Defaults to `checking`.
+          interval: The interval for the metric. Required if `metric` is `count` or `volume`.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
-            "/external_accounts",
+            "/limits",
             body=maybe_transform(
                 {
-                    "routing_number": routing_number,
-                    "account_number": account_number,
-                    "funding": funding,
-                    "description": description,
+                    "metric": metric,
+                    "interval": interval,
+                    "model_id": model_id,
+                    "value": value,
                 },
-                external_account_create_params.ExternalAccountCreateParams,
+                limit_create_params.LimitCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
-            cast_to=ExternalAccount,
+            cast_to=Limit,
         )
 
     def retrieve(
         self,
-        external_account_id: str,
+        limit_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
-    ) -> ExternalAccount:
-        """Retrieve an External Account"""
+        timeout: float | None | NotGiven = NOT_GIVEN,
+    ) -> Limit:
+        """Retrieve a Limit"""
         return self._get(
-            f"/external_accounts/{external_account_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
-            cast_to=ExternalAccount,
+            f"/limits/{limit_id}",
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
+            cast_to=Limit,
         )
 
     def update(
         self,
-        external_account_id: str,
+        limit_id: str,
         *,
-        description: str | NotGiven = NOT_GIVEN,
-        status: Literal["active", "archived"] | NotGiven = NOT_GIVEN,
+        status: Literal["inactive", "active"],
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
-    ) -> ExternalAccount:
+    ) -> Limit:
         """
-        Update an External Account
+        Update a Limit
 
         Args:
-          description: The description you choose to give the external account.
-
-          status: The status of the External Account.
+          status: The status to update the limit with.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._patch(
-            f"/external_accounts/{external_account_id}",
-            body=maybe_transform(
-                {
-                    "description": description,
-                    "status": status,
-                },
-                external_account_update_params.ExternalAccountUpdateParams,
-            ),
+            f"/limits/{limit_id}",
+            body=maybe_transform({"status": status}, limit_update_params.LimitUpdateParams),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
-            cast_to=ExternalAccount,
+            cast_to=Limit,
         )
 
     def list(
         self,
         *,
         cursor: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
-        status: external_account_list_params.Status | NotGiven = NOT_GIVEN,
+        model_id: str | NotGiven = NOT_GIVEN,
+        status: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
-    ) -> SyncPage[ExternalAccount]:
+        timeout: float | None | NotGiven = NOT_GIVEN,
+    ) -> SyncPage[Limit]:
         """
-        List External Accounts
+        List Limits
 
         Args:
           cursor: Return the page of entries after this one.
 
           limit: Limit the size of the list that is returned. The default (and maximum) is 100
               objects.
 
+          model_id: The model to retrieve limits for.
+
+          status: The status to retrieve limits for.
+
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
-            "/external_accounts",
-            page=SyncPage[ExternalAccount],
+            "/limits",
+            page=SyncPage[Limit],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
+                        "model_id": model_id,
                         "status": status,
                     },
-                    external_account_list_params.ExternalAccountListParams,
+                    limit_list_params.LimitListParams,
                 ),
             ),
-            model=ExternalAccount,
+            model=Limit,
         )
 
 
-class AsyncExternalAccounts(AsyncAPIResource):
+class AsyncLimits(AsyncAPIResource):
     async def create(
         self,
         *,
-        account_number: str,
-        description: str,
-        routing_number: str,
-        funding: Literal["checking", "savings", "other"] | NotGiven = NOT_GIVEN,
+        metric: Literal["count", "volume"],
+        model_id: str,
+        value: int,
+        interval: Literal["transaction", "day", "week", "month", "year", "all_time"] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
-    ) -> ExternalAccount:
+    ) -> Limit:
         """
-        Create an External Account
+        Create a Limit
 
         Args:
-          account_number: The account number for the destination account.
+          metric: The metric for the limit.
 
-          description: The name you choose for the Account.
+          model_id: The identifier of the Account or Account Number you wish to associate the limit
+              with.
 
-          routing_number: The American Bankers' Association (ABA) Routing Transit Number (RTN) for the
-              destination account.
+          value: The value to test the limit against.
 
-          funding: The type of the destination account. Defaults to `checking`.
+          interval: The interval for the metric. Required if `metric` is `count` or `volume`.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
-            "/external_accounts",
+            "/limits",
             body=maybe_transform(
                 {
-                    "routing_number": routing_number,
-                    "account_number": account_number,
-                    "funding": funding,
-                    "description": description,
+                    "metric": metric,
+                    "interval": interval,
+                    "model_id": model_id,
+                    "value": value,
                 },
-                external_account_create_params.ExternalAccountCreateParams,
+                limit_create_params.LimitCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
-            cast_to=ExternalAccount,
+            cast_to=Limit,
         )
 
     async def retrieve(
         self,
-        external_account_id: str,
+        limit_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
-    ) -> ExternalAccount:
-        """Retrieve an External Account"""
+        timeout: float | None | NotGiven = NOT_GIVEN,
+    ) -> Limit:
+        """Retrieve a Limit"""
         return await self._get(
-            f"/external_accounts/{external_account_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
-            cast_to=ExternalAccount,
+            f"/limits/{limit_id}",
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
+            cast_to=Limit,
         )
 
     async def update(
         self,
-        external_account_id: str,
+        limit_id: str,
         *,
-        description: str | NotGiven = NOT_GIVEN,
-        status: Literal["active", "archived"] | NotGiven = NOT_GIVEN,
+        status: Literal["inactive", "active"],
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
-    ) -> ExternalAccount:
+    ) -> Limit:
         """
-        Update an External Account
+        Update a Limit
 
         Args:
-          description: The description you choose to give the external account.
-
-          status: The status of the External Account.
+          status: The status to update the limit with.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._patch(
-            f"/external_accounts/{external_account_id}",
-            body=maybe_transform(
-                {
-                    "description": description,
-                    "status": status,
-                },
-                external_account_update_params.ExternalAccountUpdateParams,
-            ),
+            f"/limits/{limit_id}",
+            body=maybe_transform({"status": status}, limit_update_params.LimitUpdateParams),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
-            cast_to=ExternalAccount,
+            cast_to=Limit,
         )
 
     def list(
         self,
         *,
         cursor: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
-        status: external_account_list_params.Status | NotGiven = NOT_GIVEN,
+        model_id: str | NotGiven = NOT_GIVEN,
+        status: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
-    ) -> AsyncPaginator[ExternalAccount, AsyncPage[ExternalAccount]]:
+        timeout: float | None | NotGiven = NOT_GIVEN,
+    ) -> AsyncPaginator[Limit, AsyncPage[Limit]]:
         """
-        List External Accounts
+        List Limits
 
         Args:
           cursor: Return the page of entries after this one.
 
           limit: Limit the size of the list that is returned. The default (and maximum) is 100
               objects.
 
+          model_id: The model to retrieve limits for.
+
+          status: The status to retrieve limits for.
+
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
-            "/external_accounts",
-            page=AsyncPage[ExternalAccount],
+            "/limits",
+            page=AsyncPage[Limit],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
+                        "model_id": model_id,
                         "status": status,
                     },
-                    external_account_list_params.ExternalAccountListParams,
+                    limit_list_params.LimitListParams,
                 ),
             ),
-            model=ExternalAccount,
+            model=Limit,
         )
```

### Comparing `increase-0.5.0/src/increase/resources/files.py` & `increase-0.6.0/src/increase/resources/files.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,22 +25,24 @@
             "check_image_back",
             "form_ss_4",
             "identity_document",
             "other",
             "trust_formation_document",
             "digital_wallet_artwork",
             "digital_wallet_app_icon",
+            "document_request",
             "entity_supplemental_document",
         ],
         description: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> File:
         """
         To upload a file to Increase, you'll need to send a request of Content-Type
         `multipart/form-data`. The request should contain the file you would like to
         upload, as well as the parameters for creating a file.
 
@@ -55,14 +57,16 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         body = deepcopy_minimal(
             {
                 "file": file,
                 "description": description,
                 "purpose": purpose,
@@ -79,33 +83,37 @@
             "/files",
             body=maybe_transform(body, file_create_params.FileCreateParams),
             files=files,
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=File,
         )
 
     def retrieve(
         self,
         file_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> File:
         """Retrieve a File"""
         return self._get(
             f"/files/{file_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=File,
         )
 
     def list(
         self,
         *,
         created_at: file_list_params.CreatedAt | NotGiven = NOT_GIVEN,
@@ -113,14 +121,15 @@
         limit: int | NotGiven = NOT_GIVEN,
         purpose: file_list_params.Purpose | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> SyncPage[File]:
         """
         List Files
 
         Args:
           cursor: Return the page of entries after this one.
 
@@ -128,22 +137,25 @@
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/files",
             page=SyncPage[File],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                         "created_at": created_at,
                         "purpose": purpose,
                     },
@@ -164,22 +176,24 @@
             "check_image_back",
             "form_ss_4",
             "identity_document",
             "other",
             "trust_formation_document",
             "digital_wallet_artwork",
             "digital_wallet_app_icon",
+            "document_request",
             "entity_supplemental_document",
         ],
         description: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> File:
         """
         To upload a file to Increase, you'll need to send a request of Content-Type
         `multipart/form-data`. The request should contain the file you would like to
         upload, as well as the parameters for creating a file.
 
@@ -194,14 +208,16 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         body = deepcopy_minimal(
             {
                 "file": file,
                 "description": description,
                 "purpose": purpose,
@@ -218,33 +234,37 @@
             "/files",
             body=maybe_transform(body, file_create_params.FileCreateParams),
             files=files,
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=File,
         )
 
     async def retrieve(
         self,
         file_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> File:
         """Retrieve a File"""
         return await self._get(
             f"/files/{file_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=File,
         )
 
     def list(
         self,
         *,
         created_at: file_list_params.CreatedAt | NotGiven = NOT_GIVEN,
@@ -252,14 +272,15 @@
         limit: int | NotGiven = NOT_GIVEN,
         purpose: file_list_params.Purpose | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> AsyncPaginator[File, AsyncPage[File]]:
         """
         List Files
 
         Args:
           cursor: Return the page of entries after this one.
 
@@ -267,22 +288,25 @@
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/files",
             page=AsyncPage[File],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                         "created_at": created_at,
                         "purpose": purpose,
                     },
```

### Comparing `increase-0.5.0/src/increase/resources/groups.py` & `increase-0.6.0/src/increase/resources/groups.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
 from ..types import Group
-from .._types import Body, Query, Headers
+from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from .._resource import SyncAPIResource, AsyncAPIResource
 from .._base_client import make_request_options
 
 __all__ = ["Groups", "AsyncGroups"]
 
 
 class Groups(SyncAPIResource):
@@ -15,32 +15,38 @@
         self,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> Group:
         """Returns details for the currently authenticated Group."""
         return self._get(
             "/groups/current",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=Group,
         )
 
 
 class AsyncGroups(AsyncAPIResource):
     async def retrieve_details(
         self,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> Group:
         """Returns details for the currently authenticated Group."""
         return await self._get(
             "/groups/current",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=Group,
         )
```

### Comparing `increase-0.5.0/src/increase/resources/inbound_ach_transfer_returns.py` & `increase-0.6.0/src/increase/resources/inbound_ach_transfer_returns.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,14 +34,15 @@
         ],
         transaction_id: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> InboundACHTransferReturn:
         """
         Create an ACH Return
 
         Args:
           reason: The reason why this transfer will be returned. The most usual return codes are
@@ -52,14 +53,16 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             "/inbound_ach_transfer_returns",
             body=maybe_transform(
                 {
                     "transaction_id": transaction_id,
@@ -67,46 +70,51 @@
                 },
                 inbound_ach_transfer_return_create_params.InboundACHTransferReturnCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=InboundACHTransferReturn,
         )
 
     def retrieve(
         self,
         inbound_ach_transfer_return_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> InboundACHTransferReturn:
         """Retrieve an Inbound ACH Transfer Return"""
         return self._get(
             f"/inbound_ach_transfer_returns/{inbound_ach_transfer_return_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=InboundACHTransferReturn,
         )
 
     def list(
         self,
         *,
         cursor: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> SyncPage[InboundACHTransferReturn]:
         """
         List Inbound ACH Transfer Returns
 
         Args:
           cursor: Return the page of entries after this one.
 
@@ -114,22 +122,25 @@
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/inbound_ach_transfer_returns",
             page=SyncPage[InboundACHTransferReturn],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                     },
                     inbound_ach_transfer_return_list_params.InboundACHTransferReturnListParams,
                 ),
@@ -154,14 +165,15 @@
         ],
         transaction_id: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> InboundACHTransferReturn:
         """
         Create an ACH Return
 
         Args:
           reason: The reason why this transfer will be returned. The most usual return codes are
@@ -172,14 +184,16 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             "/inbound_ach_transfer_returns",
             body=maybe_transform(
                 {
                     "transaction_id": transaction_id,
@@ -187,46 +201,51 @@
                 },
                 inbound_ach_transfer_return_create_params.InboundACHTransferReturnCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=InboundACHTransferReturn,
         )
 
     async def retrieve(
         self,
         inbound_ach_transfer_return_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> InboundACHTransferReturn:
         """Retrieve an Inbound ACH Transfer Return"""
         return await self._get(
             f"/inbound_ach_transfer_returns/{inbound_ach_transfer_return_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=InboundACHTransferReturn,
         )
 
     def list(
         self,
         *,
         cursor: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> AsyncPaginator[InboundACHTransferReturn, AsyncPage[InboundACHTransferReturn]]:
         """
         List Inbound ACH Transfer Returns
 
         Args:
           cursor: Return the page of entries after this one.
 
@@ -234,22 +253,25 @@
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/inbound_ach_transfer_returns",
             page=AsyncPage[InboundACHTransferReturn],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                     },
                     inbound_ach_transfer_return_list_params.InboundACHTransferReturnListParams,
                 ),
```

### Comparing `increase-0.5.0/src/increase/resources/inbound_wire_drawdown_requests.py` & `increase-0.6.0/src/increase/resources/inbound_wire_drawdown_requests.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,32 +21,36 @@
         inbound_wire_drawdown_request_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> InboundWireDrawdownRequest:
         """Retrieve an Inbound Wire Drawdown Request"""
         return self._get(
             f"/inbound_wire_drawdown_requests/{inbound_wire_drawdown_request_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=InboundWireDrawdownRequest,
         )
 
     def list(
         self,
         *,
         cursor: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> SyncPage[InboundWireDrawdownRequest]:
         """
         List Inbound Wire Drawdown Requests
 
         Args:
           cursor: Return the page of entries after this one.
 
@@ -54,22 +58,25 @@
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/inbound_wire_drawdown_requests",
             page=SyncPage[InboundWireDrawdownRequest],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                     },
                     inbound_wire_drawdown_request_list_params.InboundWireDrawdownRequestListParams,
                 ),
@@ -84,32 +91,36 @@
         inbound_wire_drawdown_request_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> InboundWireDrawdownRequest:
         """Retrieve an Inbound Wire Drawdown Request"""
         return await self._get(
             f"/inbound_wire_drawdown_requests/{inbound_wire_drawdown_request_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=InboundWireDrawdownRequest,
         )
 
     def list(
         self,
         *,
         cursor: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> AsyncPaginator[InboundWireDrawdownRequest, AsyncPage[InboundWireDrawdownRequest]]:
         """
         List Inbound Wire Drawdown Requests
 
         Args:
           cursor: Return the page of entries after this one.
 
@@ -117,22 +128,25 @@
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/inbound_wire_drawdown_requests",
             page=AsyncPage[InboundWireDrawdownRequest],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                     },
                     inbound_wire_drawdown_request_list_params.InboundWireDrawdownRequestListParams,
                 ),
```

### Comparing `increase-0.5.0/src/increase/resources/limits.py` & `increase-0.6.0/src/increase/resources/simulations/cards.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,342 +1,278 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing_extensions import Literal
+from ...types import Transaction
+from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
+from ..._utils import maybe_transform
+from ..._resource import SyncAPIResource, AsyncAPIResource
+from ..._base_client import make_request_options
+from ...types.simulations import (
+    CardAuthorizationSimulation,
+    card_authorize_params,
+    card_settlement_params,
+)
 
-from ..types import Limit, limit_list_params, limit_create_params, limit_update_params
-from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
-from .._utils import maybe_transform
-from .._resource import SyncAPIResource, AsyncAPIResource
-from ..pagination import SyncPage, AsyncPage
-from .._base_client import AsyncPaginator, make_request_options
+__all__ = ["Cards", "AsyncCards"]
 
-__all__ = ["Limits", "AsyncLimits"]
 
-
-class Limits(SyncAPIResource):
-    def create(
+class Cards(SyncAPIResource):
+    def authorize(
         self,
         *,
-        metric: Literal["count", "volume"],
-        model_id: str,
-        value: int,
-        interval: Literal["transaction", "day", "week", "month", "year", "all_time"] | NotGiven = NOT_GIVEN,
+        amount: int,
+        card_id: str | NotGiven = NOT_GIVEN,
+        digital_wallet_token_id: str | NotGiven = NOT_GIVEN,
+        event_subscription_id: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
-    ) -> Limit:
-        """
-        Create a Limit
+    ) -> CardAuthorizationSimulation:
+        """Simulates a purchase authorization on a [Card](#cards).
+
+        Depending on the balance
+        available to the card and the `amount` submitted, the authorization activity
+        will result in a [Pending Transaction](#pending-transactions) of type
+        `card_authorization` or a [Declined Transaction](#declined-transactions) of type
+        `card_decline`. You can pass either a Card id or a
+        [Digital Wallet Token](#digital-wallet-tokens) id to simulate the two different
+        ways purchases can be made.
 
         Args:
-          metric: The metric for the limit.
+          amount: The authorization amount in cents.
 
-          model_id: The identifier of the Account or Account Number you wish to associate the limit
-              with.
+          card_id: The identifier of the Card to be authorized.
 
-          value: The value to test the limit against.
+          digital_wallet_token_id: The identifier of the Digital Wallet Token to be authorized.
 
-          interval: The interval for the metric. Required if `metric` is `count` or `volume`.
+          event_subscription_id: The identifier of the Event Subscription to use. If provided, will override the
+              default real time event subscription. Because you can only create one real time
+              decision event subscription, you can use this field to route events to any
+              specified event subscription for testing purposes.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
-            "/limits",
+            "/simulations/card_authorizations",
             body=maybe_transform(
                 {
-                    "metric": metric,
-                    "interval": interval,
-                    "model_id": model_id,
-                    "value": value,
+                    "amount": amount,
+                    "card_id": card_id,
+                    "digital_wallet_token_id": digital_wallet_token_id,
+                    "event_subscription_id": event_subscription_id,
                 },
-                limit_create_params.LimitCreateParams,
+                card_authorize_params.CardAuthorizeParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
-            cast_to=Limit,
-        )
-
-    def retrieve(
-        self,
-        limit_id: str,
-        *,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-    ) -> Limit:
-        """Retrieve a Limit"""
-        return self._get(
-            f"/limits/{limit_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
-            cast_to=Limit,
+            cast_to=CardAuthorizationSimulation,
         )
 
-    def update(
+    def settlement(
         self,
-        limit_id: str,
         *,
-        status: Literal["inactive", "active"],
+        card_id: str,
+        pending_transaction_id: str,
+        amount: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
-    ) -> Limit:
-        """
-        Update a Limit
-
-        Args:
-          status: The status to update the limit with.
-
-          extra_headers: Send extra headers
-
-          extra_query: Add additional query parameters to the request
-
-          extra_body: Add additional JSON properties to the request
-
-          idempotency_key: Specify a custom idempotency key for this request
-        """
-        return self._patch(
-            f"/limits/{limit_id}",
-            body=maybe_transform({"status": status}, limit_update_params.LimitUpdateParams),
-            options=make_request_options(
-                extra_headers=extra_headers,
-                extra_query=extra_query,
-                extra_body=extra_body,
-                idempotency_key=idempotency_key,
-            ),
-            cast_to=Limit,
-        )
+    ) -> Transaction:
+        """Simulates the settlement of an authorization by a card acquirer.
 
-    def list(
-        self,
-        *,
-        cursor: str | NotGiven = NOT_GIVEN,
-        limit: int | NotGiven = NOT_GIVEN,
-        model_id: str | NotGiven = NOT_GIVEN,
-        status: str | NotGiven = NOT_GIVEN,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-    ) -> SyncPage[Limit]:
-        """
-        List Limits
+        After a card
+        authorization is created, the merchant will eventually send a settlement. This
+        simulates that event, which may occur many days after the purchase in
+        production. The amount settled can be different from the amount originally
+        authorized, for example, when adding a tip to a restaurant bill.
 
         Args:
-          cursor: Return the page of entries after this one.
-
-          limit: Limit the size of the list that is returned. The default (and maximum) is 100
-              objects.
+          card_id: The identifier of the Card to create a settlement on.
 
-          model_id: The model to retrieve limits for.
+          pending_transaction_id: The identifier of the Pending Transaction for the Card Authorization you wish to
+              settle.
 
-          status: The status to retrieve limits for.
+          amount: The amount to be settled. This defaults to the amount of the Pending Transaction
+              being settled.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
         """
-        return self._get_api_list(
-            "/limits",
-            page=SyncPage[Limit],
+        return self._post(
+            "/simulations/card_settlements",
+            body=maybe_transform(
+                {
+                    "card_id": card_id,
+                    "pending_transaction_id": pending_transaction_id,
+                    "amount": amount,
+                },
+                card_settlement_params.CardSettlementParams,
+            ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query=maybe_transform(
-                    {
-                        "cursor": cursor,
-                        "limit": limit,
-                        "model_id": model_id,
-                        "status": status,
-                    },
-                    limit_list_params.LimitListParams,
-                ),
+                timeout=timeout,
+                idempotency_key=idempotency_key,
             ),
-            model=Limit,
+            cast_to=Transaction,
         )
 
 
-class AsyncLimits(AsyncAPIResource):
-    async def create(
+class AsyncCards(AsyncAPIResource):
+    async def authorize(
         self,
         *,
-        metric: Literal["count", "volume"],
-        model_id: str,
-        value: int,
-        interval: Literal["transaction", "day", "week", "month", "year", "all_time"] | NotGiven = NOT_GIVEN,
+        amount: int,
+        card_id: str | NotGiven = NOT_GIVEN,
+        digital_wallet_token_id: str | NotGiven = NOT_GIVEN,
+        event_subscription_id: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
-    ) -> Limit:
-        """
-        Create a Limit
+    ) -> CardAuthorizationSimulation:
+        """Simulates a purchase authorization on a [Card](#cards).
+
+        Depending on the balance
+        available to the card and the `amount` submitted, the authorization activity
+        will result in a [Pending Transaction](#pending-transactions) of type
+        `card_authorization` or a [Declined Transaction](#declined-transactions) of type
+        `card_decline`. You can pass either a Card id or a
+        [Digital Wallet Token](#digital-wallet-tokens) id to simulate the two different
+        ways purchases can be made.
 
         Args:
-          metric: The metric for the limit.
+          amount: The authorization amount in cents.
 
-          model_id: The identifier of the Account or Account Number you wish to associate the limit
-              with.
+          card_id: The identifier of the Card to be authorized.
 
-          value: The value to test the limit against.
+          digital_wallet_token_id: The identifier of the Digital Wallet Token to be authorized.
 
-          interval: The interval for the metric. Required if `metric` is `count` or `volume`.
+          event_subscription_id: The identifier of the Event Subscription to use. If provided, will override the
+              default real time event subscription. Because you can only create one real time
+              decision event subscription, you can use this field to route events to any
+              specified event subscription for testing purposes.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
-            "/limits",
+            "/simulations/card_authorizations",
             body=maybe_transform(
                 {
-                    "metric": metric,
-                    "interval": interval,
-                    "model_id": model_id,
-                    "value": value,
+                    "amount": amount,
+                    "card_id": card_id,
+                    "digital_wallet_token_id": digital_wallet_token_id,
+                    "event_subscription_id": event_subscription_id,
                 },
-                limit_create_params.LimitCreateParams,
+                card_authorize_params.CardAuthorizeParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
-            cast_to=Limit,
+            cast_to=CardAuthorizationSimulation,
         )
 
-    async def retrieve(
+    async def settlement(
         self,
-        limit_id: str,
         *,
+        card_id: str,
+        pending_transaction_id: str,
+        amount: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
-    ) -> Limit:
-        """Retrieve a Limit"""
-        return await self._get(
-            f"/limits/{limit_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
-            cast_to=Limit,
-        )
-
-    async def update(
-        self,
-        limit_id: str,
-        *,
-        status: Literal["inactive", "active"],
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
-    ) -> Limit:
-        """
-        Update a Limit
+    ) -> Transaction:
+        """Simulates the settlement of an authorization by a card acquirer.
 
-        Args:
-          status: The status to update the limit with.
-
-          extra_headers: Send extra headers
-
-          extra_query: Add additional query parameters to the request
-
-          extra_body: Add additional JSON properties to the request
-
-          idempotency_key: Specify a custom idempotency key for this request
-        """
-        return await self._patch(
-            f"/limits/{limit_id}",
-            body=maybe_transform({"status": status}, limit_update_params.LimitUpdateParams),
-            options=make_request_options(
-                extra_headers=extra_headers,
-                extra_query=extra_query,
-                extra_body=extra_body,
-                idempotency_key=idempotency_key,
-            ),
-            cast_to=Limit,
-        )
-
-    def list(
-        self,
-        *,
-        cursor: str | NotGiven = NOT_GIVEN,
-        limit: int | NotGiven = NOT_GIVEN,
-        model_id: str | NotGiven = NOT_GIVEN,
-        status: str | NotGiven = NOT_GIVEN,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-    ) -> AsyncPaginator[Limit, AsyncPage[Limit]]:
-        """
-        List Limits
+        After a card
+        authorization is created, the merchant will eventually send a settlement. This
+        simulates that event, which may occur many days after the purchase in
+        production. The amount settled can be different from the amount originally
+        authorized, for example, when adding a tip to a restaurant bill.
 
         Args:
-          cursor: Return the page of entries after this one.
-
-          limit: Limit the size of the list that is returned. The default (and maximum) is 100
-              objects.
+          card_id: The identifier of the Card to create a settlement on.
 
-          model_id: The model to retrieve limits for.
+          pending_transaction_id: The identifier of the Pending Transaction for the Card Authorization you wish to
+              settle.
 
-          status: The status to retrieve limits for.
+          amount: The amount to be settled. This defaults to the amount of the Pending Transaction
+              being settled.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
         """
-        return self._get_api_list(
-            "/limits",
-            page=AsyncPage[Limit],
+        return await self._post(
+            "/simulations/card_settlements",
+            body=maybe_transform(
+                {
+                    "card_id": card_id,
+                    "pending_transaction_id": pending_transaction_id,
+                    "amount": amount,
+                },
+                card_settlement_params.CardSettlementParams,
+            ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query=maybe_transform(
-                    {
-                        "cursor": cursor,
-                        "limit": limit,
-                        "model_id": model_id,
-                        "status": status,
-                    },
-                    limit_list_params.LimitListParams,
-                ),
+                timeout=timeout,
+                idempotency_key=idempotency_key,
             ),
-            model=Limit,
+            cast_to=Transaction,
         )
```

### Comparing `increase-0.5.0/src/increase/resources/oauth_connections.py` & `increase-0.6.0/src/increase/resources/oauth_connections.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,32 +18,36 @@
         oauth_connection_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> OauthConnection:
         """Retrieve an OAuth Connection"""
         return self._get(
             f"/oauth_connections/{oauth_connection_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=OauthConnection,
         )
 
     def list(
         self,
         *,
         cursor: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> SyncPage[OauthConnection]:
         """
         List OAuth Connections
 
         Args:
           cursor: Return the page of entries after this one.
 
@@ -51,22 +55,25 @@
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/oauth_connections",
             page=SyncPage[OauthConnection],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                     },
                     oauth_connection_list_params.OauthConnectionListParams,
                 ),
@@ -81,32 +88,36 @@
         oauth_connection_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> OauthConnection:
         """Retrieve an OAuth Connection"""
         return await self._get(
             f"/oauth_connections/{oauth_connection_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=OauthConnection,
         )
 
     def list(
         self,
         *,
         cursor: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> AsyncPaginator[OauthConnection, AsyncPage[OauthConnection]]:
         """
         List OAuth Connections
 
         Args:
           cursor: Return the page of entries after this one.
 
@@ -114,22 +125,25 @@
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/oauth_connections",
             page=AsyncPage[OauthConnection],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                     },
                     oauth_connection_list_params.OauthConnectionListParams,
                 ),
```

### Comparing `increase-0.5.0/src/increase/resources/pending_transactions.py` & `increase-0.6.0/src/increase/resources/transactions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,166 +1,178 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from ..types import PendingTransaction, pending_transaction_list_params
+from ..types import Transaction, transaction_list_params
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from .._utils import maybe_transform
 from .._resource import SyncAPIResource, AsyncAPIResource
 from ..pagination import SyncPage, AsyncPage
 from .._base_client import AsyncPaginator, make_request_options
 
-__all__ = ["PendingTransactions", "AsyncPendingTransactions"]
+__all__ = ["Transactions", "AsyncTransactions"]
 
 
-class PendingTransactions(SyncAPIResource):
+class Transactions(SyncAPIResource):
     def retrieve(
         self,
-        pending_transaction_id: str,
+        transaction_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
-    ) -> PendingTransaction:
-        """Retrieve a Pending Transaction"""
+        timeout: float | None | NotGiven = NOT_GIVEN,
+    ) -> Transaction:
+        """Retrieve a Transaction"""
         return self._get(
-            f"/pending_transactions/{pending_transaction_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
-            cast_to=PendingTransaction,
+            f"/transactions/{transaction_id}",
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
+            cast_to=Transaction,
         )
 
     def list(
         self,
         *,
         account_id: str | NotGiven = NOT_GIVEN,
+        category: transaction_list_params.Category | NotGiven = NOT_GIVEN,
+        created_at: transaction_list_params.CreatedAt | NotGiven = NOT_GIVEN,
         cursor: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         route_id: str | NotGiven = NOT_GIVEN,
-        source_id: str | NotGiven = NOT_GIVEN,
-        status: pending_transaction_list_params.Status | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
-    ) -> SyncPage[PendingTransaction]:
+        timeout: float | None | NotGiven = NOT_GIVEN,
+    ) -> SyncPage[Transaction]:
         """
-        List Pending Transactions
+        List Transactions
 
         Args:
-          account_id: Filter pending transactions to those belonging to the specified Account.
+          account_id: Filter Transactions for those belonging to the specified Account.
 
           cursor: Return the page of entries after this one.
 
           limit: Limit the size of the list that is returned. The default (and maximum) is 100
               objects.
 
-          route_id: Filter pending transactions to those belonging to the specified Route.
-
-          source_id: Filter pending transactions to those caused by the specified source.
+          route_id: Filter Transactions for those belonging to the specified route. This could be a
+              Card ID or an Account Number ID.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
-            "/pending_transactions",
-            page=SyncPage[PendingTransaction],
+            "/transactions",
+            page=SyncPage[Transaction],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                         "account_id": account_id,
                         "route_id": route_id,
-                        "source_id": source_id,
-                        "status": status,
+                        "created_at": created_at,
+                        "category": category,
                     },
-                    pending_transaction_list_params.PendingTransactionListParams,
+                    transaction_list_params.TransactionListParams,
                 ),
             ),
-            model=PendingTransaction,
+            model=Transaction,
         )
 
 
-class AsyncPendingTransactions(AsyncAPIResource):
+class AsyncTransactions(AsyncAPIResource):
     async def retrieve(
         self,
-        pending_transaction_id: str,
+        transaction_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
-    ) -> PendingTransaction:
-        """Retrieve a Pending Transaction"""
+        timeout: float | None | NotGiven = NOT_GIVEN,
+    ) -> Transaction:
+        """Retrieve a Transaction"""
         return await self._get(
-            f"/pending_transactions/{pending_transaction_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
-            cast_to=PendingTransaction,
+            f"/transactions/{transaction_id}",
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
+            cast_to=Transaction,
         )
 
     def list(
         self,
         *,
         account_id: str | NotGiven = NOT_GIVEN,
+        category: transaction_list_params.Category | NotGiven = NOT_GIVEN,
+        created_at: transaction_list_params.CreatedAt | NotGiven = NOT_GIVEN,
         cursor: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         route_id: str | NotGiven = NOT_GIVEN,
-        source_id: str | NotGiven = NOT_GIVEN,
-        status: pending_transaction_list_params.Status | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
-    ) -> AsyncPaginator[PendingTransaction, AsyncPage[PendingTransaction]]:
+        timeout: float | None | NotGiven = NOT_GIVEN,
+    ) -> AsyncPaginator[Transaction, AsyncPage[Transaction]]:
         """
-        List Pending Transactions
+        List Transactions
 
         Args:
-          account_id: Filter pending transactions to those belonging to the specified Account.
+          account_id: Filter Transactions for those belonging to the specified Account.
 
           cursor: Return the page of entries after this one.
 
           limit: Limit the size of the list that is returned. The default (and maximum) is 100
               objects.
 
-          route_id: Filter pending transactions to those belonging to the specified Route.
-
-          source_id: Filter pending transactions to those caused by the specified source.
+          route_id: Filter Transactions for those belonging to the specified route. This could be a
+              Card ID or an Account Number ID.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
-            "/pending_transactions",
-            page=AsyncPage[PendingTransaction],
+            "/transactions",
+            page=AsyncPage[Transaction],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                         "account_id": account_id,
                         "route_id": route_id,
-                        "source_id": source_id,
-                        "status": status,
+                        "created_at": created_at,
+                        "category": category,
                     },
-                    pending_transaction_list_params.PendingTransactionListParams,
+                    transaction_list_params.TransactionListParams,
                 ),
             ),
-            model=PendingTransaction,
+            model=Transaction,
         )
```

### Comparing `increase-0.5.0/src/increase/resources/real_time_decisions.py` & `increase-0.6.0/src/increase/resources/real_time_decisions.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,19 +17,22 @@
         real_time_decision_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> RealTimeDecision:
         """Retrieve a Real-Time Decision"""
         return self._get(
             f"/real_time_decisions/{real_time_decision_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=RealTimeDecision,
         )
 
     def action(
         self,
         real_time_decision_id: str,
         *,
@@ -38,14 +41,15 @@
         | NotGiven = NOT_GIVEN,
         digital_wallet_token: real_time_decision_action_params.DigitalWalletToken | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> RealTimeDecision:
         """
         Action a Real-Time Decision
 
         Args:
           card_authorization: If the Real-Time Decision relates to a card authorization attempt, this object
@@ -59,14 +63,16 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             f"/real_time_decisions/{real_time_decision_id}/action",
             body=maybe_transform(
                 {
                     "card_authorization": card_authorization,
@@ -75,14 +81,15 @@
                 },
                 real_time_decision_action_params.RealTimeDecisionActionParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=RealTimeDecision,
         )
 
 
 class AsyncRealTimeDecisions(AsyncAPIResource):
@@ -91,19 +98,22 @@
         real_time_decision_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> RealTimeDecision:
         """Retrieve a Real-Time Decision"""
         return await self._get(
             f"/real_time_decisions/{real_time_decision_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=RealTimeDecision,
         )
 
     async def action(
         self,
         real_time_decision_id: str,
         *,
@@ -112,14 +122,15 @@
         | NotGiven = NOT_GIVEN,
         digital_wallet_token: real_time_decision_action_params.DigitalWalletToken | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> RealTimeDecision:
         """
         Action a Real-Time Decision
 
         Args:
           card_authorization: If the Real-Time Decision relates to a card authorization attempt, this object
@@ -133,14 +144,16 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             f"/real_time_decisions/{real_time_decision_id}/action",
             body=maybe_transform(
                 {
                     "card_authorization": card_authorization,
@@ -149,11 +162,12 @@
                 },
                 real_time_decision_action_params.RealTimeDecisionActionParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=RealTimeDecision,
         )
```

### Comparing `increase-0.5.0/src/increase/resources/routing_numbers.py` & `increase-0.6.0/src/increase/resources/routing_numbers.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         cursor: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> SyncPage[RoutingNumber]:
         """
         You can use this API to confirm if a routing number is valid, such as when a
         user is providing you with bank account details. Since routing numbers uniquely
         identify a bank, this will always return 0 or 1 entry. In Sandbox, the only
         valid routing number for this method is 110000000.
 
@@ -40,22 +41,25 @@
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/routing_numbers",
             page=SyncPage[RoutingNumber],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                         "routing_number": routing_number,
                     },
                     routing_number_list_params.RoutingNumberListParams,
@@ -73,14 +77,15 @@
         cursor: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> AsyncPaginator[RoutingNumber, AsyncPage[RoutingNumber]]:
         """
         You can use this API to confirm if a routing number is valid, such as when a
         user is providing you with bank account details. Since routing numbers uniquely
         identify a bank, this will always return 0 or 1 entry. In Sandbox, the only
         valid routing number for this method is 110000000.
 
@@ -93,22 +98,25 @@
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/routing_numbers",
             page=AsyncPage[RoutingNumber],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                         "routing_number": routing_number,
                     },
                     routing_number_list_params.RoutingNumberListParams,
```

### Comparing `increase-0.5.0/src/increase/resources/simulations/__init__.py` & `increase-0.6.0/src/increase/resources/simulations/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from .card_refunds import CardRefunds, AsyncCardRefunds
 from .ach_transfers import ACHTransfers, AsyncACHTransfers
 from .card_disputes import CardDisputes, AsyncCardDisputes
 from .check_deposits import CheckDeposits, AsyncCheckDeposits
 from .wire_transfers import WireTransfers, AsyncWireTransfers
 from .check_transfers import CheckTransfers, AsyncCheckTransfers
 from .account_transfers import AccountTransfers, AsyncAccountTransfers
+from .interest_payments import InterestPayments, AsyncInterestPayments
 from .account_statements import AccountStatements, AsyncAccountStatements
 from .real_time_payments_transfers import (
     RealTimePaymentsTransfers,
     AsyncRealTimePaymentsTransfers,
 )
 from .digital_wallet_token_requests import (
     DigitalWalletTokenRequests,
@@ -41,14 +42,16 @@
     "AsyncDocuments",
     "DigitalWalletTokenRequests",
     "AsyncDigitalWalletTokenRequests",
     "CheckDeposits",
     "AsyncCheckDeposits",
     "InboundWireDrawdownRequests",
     "AsyncInboundWireDrawdownRequests",
+    "InterestPayments",
+    "AsyncInterestPayments",
     "WireTransfers",
     "AsyncWireTransfers",
     "Cards",
     "AsyncCards",
     "RealTimePaymentsTransfers",
     "AsyncRealTimePaymentsTransfers",
     "Simulations",
```

### Comparing `increase-0.5.0/src/increase/resources/simulations/account_statements.py` & `increase-0.6.0/src/increase/resources/simulations/account_statements.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
 from ...types import AccountStatement
-from ..._types import Body, Query, Headers
+from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from ..._utils import maybe_transform
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ..._base_client import make_request_options
 from ...types.simulations import account_statement_create_params
 
 __all__ = ["AccountStatements", "AsyncAccountStatements"]
 
@@ -18,14 +18,15 @@
         *,
         account_id: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> AccountStatement:
         """
         Simulates an [Account Statement](#account-statements) being created for an
         account. In production, Account Statements are generated once per month.
 
         Args:
@@ -33,25 +34,28 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             "/simulations/account_statements",
             body=maybe_transform(
                 {"account_id": account_id}, account_statement_create_params.AccountStatementCreateParams
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=AccountStatement,
         )
 
 
 class AsyncAccountStatements(AsyncAPIResource):
@@ -60,14 +64,15 @@
         *,
         account_id: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> AccountStatement:
         """
         Simulates an [Account Statement](#account-statements) being created for an
         account. In production, Account Statements are generated once per month.
 
         Args:
@@ -75,22 +80,25 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             "/simulations/account_statements",
             body=maybe_transform(
                 {"account_id": account_id}, account_statement_create_params.AccountStatementCreateParams
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=AccountStatement,
         )
```

### Comparing `increase-0.5.0/src/increase/resources/simulations/account_transfers.py` & `increase-0.6.0/src/increase/resources/simulations/account_transfers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
 from ...types import AccountTransfer
-from ..._types import Body, Query, Headers
+from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ..._base_client import make_request_options
 
 __all__ = ["AccountTransfers", "AsyncAccountTransfers"]
 
 
 class AccountTransfers(SyncAPIResource):
@@ -16,28 +16,30 @@
         account_transfer_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> AccountTransfer:
         """
         If your account is configured to require approval for each transfer, this
         endpoint simulates the approval of an [Account Transfer](#account-transfers).
         You can also approve sandbox Account Transfers in the dashboard. This transfer
         must first have a `status` of `pending_approval`.
         """
         return self._post(
             f"/simulations/account_transfers/{account_transfer_id}/complete",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=AccountTransfer,
         )
 
 
 class AsyncAccountTransfers(AsyncAPIResource):
@@ -46,25 +48,27 @@
         account_transfer_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> AccountTransfer:
         """
         If your account is configured to require approval for each transfer, this
         endpoint simulates the approval of an [Account Transfer](#account-transfers).
         You can also approve sandbox Account Transfers in the dashboard. This transfer
         must first have a `status` of `pending_approval`.
         """
         return await self._post(
             f"/simulations/account_transfers/{account_transfer_id}/complete",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=AccountTransfer,
         )
```

### Comparing `increase-0.5.0/src/increase/resources/simulations/ach_transfers.py` & `increase-0.6.0/src/increase/resources/simulations/ach_transfers.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         company_id: str | NotGiven = NOT_GIVEN,
         company_name: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> ACHTransferSimulation:
         """Simulates an inbound ACH transfer to your account.
 
         This imitates initiating a
         transaction to an Increase account from a different financial institution. The
         transfer may be either a credit or a debit depending on if the `amount` is
@@ -64,14 +65,16 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             "/simulations/inbound_ach_transfers",
             body=maybe_transform(
                 {
                     "account_number_id": account_number_id,
@@ -84,14 +87,15 @@
                 },
                 ach_transfer_create_inbound_params.ACHTransferCreateInboundParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=ACHTransferSimulation,
         )
 
     def return_(
         self,
@@ -124,14 +128,15 @@
         ]
         | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> ACHTransfer:
         """
         Simulates the return of an [ACH Transfer](#ach-transfers) by the Federal Reserve
         due to an error condition. This will also create a Transaction to account for
         the returned funds. This transfer must first have a `status` of `submitted`.
 
@@ -141,37 +146,41 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             f"/simulations/ach_transfers/{ach_transfer_id}/return",
             body=maybe_transform({"reason": reason}, ach_transfer_return_params.ACHTransferReturnParams),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=ACHTransfer,
         )
 
     def submit(
         self,
         ach_transfer_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> ACHTransfer:
         """
         Simulates the submission of an [ACH Transfer](#ach-transfers) to the Federal
         Reserve. This transfer must first have a `status` of `pending_approval` or
         `pending_submission`. In production, Increase submits ACH Transfers to the
         Federal Reserve three times per day on weekdays. Since sandbox ACH Transfers are
@@ -180,14 +189,15 @@
         """
         return self._post(
             f"/simulations/ach_transfers/{ach_transfer_id}/submit",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=ACHTransfer,
         )
 
 
 class AsyncACHTransfers(AsyncAPIResource):
@@ -202,14 +212,15 @@
         company_id: str | NotGiven = NOT_GIVEN,
         company_name: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> ACHTransferSimulation:
         """Simulates an inbound ACH transfer to your account.
 
         This imitates initiating a
         transaction to an Increase account from a different financial institution. The
         transfer may be either a credit or a debit depending on if the `amount` is
@@ -236,14 +247,16 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             "/simulations/inbound_ach_transfers",
             body=maybe_transform(
                 {
                     "account_number_id": account_number_id,
@@ -256,14 +269,15 @@
                 },
                 ach_transfer_create_inbound_params.ACHTransferCreateInboundParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=ACHTransferSimulation,
         )
 
     async def return_(
         self,
@@ -296,14 +310,15 @@
         ]
         | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> ACHTransfer:
         """
         Simulates the return of an [ACH Transfer](#ach-transfers) by the Federal Reserve
         due to an error condition. This will also create a Transaction to account for
         the returned funds. This transfer must first have a `status` of `submitted`.
 
@@ -313,37 +328,41 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             f"/simulations/ach_transfers/{ach_transfer_id}/return",
             body=maybe_transform({"reason": reason}, ach_transfer_return_params.ACHTransferReturnParams),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=ACHTransfer,
         )
 
     async def submit(
         self,
         ach_transfer_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> ACHTransfer:
         """
         Simulates the submission of an [ACH Transfer](#ach-transfers) to the Federal
         Reserve. This transfer must first have a `status` of `pending_approval` or
         `pending_submission`. In production, Increase submits ACH Transfers to the
         Federal Reserve three times per day on weekdays. Since sandbox ACH Transfers are
@@ -352,11 +371,12 @@
         """
         return await self._post(
             f"/simulations/ach_transfers/{ach_transfer_id}/submit",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=ACHTransfer,
         )
```

### Comparing `increase-0.5.0/src/increase/resources/simulations/card_disputes.py` & `increase-0.6.0/src/increase/resources/simulations/card_disputes.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         status: Literal["accepted", "rejected"],
         explanation: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> CardDispute:
         """
         After a [Card Dispute](#card-disputes) is created in production, the dispute
         will be reviewed. Since no review happens in sandbox, this endpoint simulates
         moving a Card Dispute into a rejected or accepted state. A Card Dispute can only
         be actioned one time and must have a status of `pending_reviewing`.
@@ -41,14 +42,16 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             f"/simulations/card_disputes/{card_dispute_id}/action",
             body=maybe_transform(
                 {
                     "status": status,
@@ -56,14 +59,15 @@
                 },
                 card_dispute_action_params.CardDisputeActionParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=CardDispute,
         )
 
 
 class AsyncCardDisputes(AsyncAPIResource):
@@ -74,14 +78,15 @@
         status: Literal["accepted", "rejected"],
         explanation: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> CardDispute:
         """
         After a [Card Dispute](#card-disputes) is created in production, the dispute
         will be reviewed. Since no review happens in sandbox, this endpoint simulates
         moving a Card Dispute into a rejected or accepted state. A Card Dispute can only
         be actioned one time and must have a status of `pending_reviewing`.
@@ -93,14 +98,16 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             f"/simulations/card_disputes/{card_dispute_id}/action",
             body=maybe_transform(
                 {
                     "status": status,
@@ -108,11 +115,12 @@
                 },
                 card_dispute_action_params.CardDisputeActionParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=CardDispute,
         )
```

### Comparing `increase-0.5.0/src/increase/resources/simulations/card_refunds.py` & `increase-0.6.0/src/increase/resources/simulations/card_refunds.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
 from ...types import Transaction
-from ..._types import Body, Query, Headers
+from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from ..._utils import maybe_transform
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ..._base_client import make_request_options
 from ...types.simulations import card_refund_create_params
 
 __all__ = ["CardRefunds", "AsyncCardRefunds"]
 
@@ -18,14 +18,15 @@
         *,
         transaction_id: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> Transaction:
         """Simulates refunding a card transaction.
 
         The full value of the original sandbox
         transaction is refunded.
 
@@ -35,23 +36,26 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             "/simulations/card_refunds",
             body=maybe_transform({"transaction_id": transaction_id}, card_refund_create_params.CardRefundCreateParams),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=Transaction,
         )
 
 
 class AsyncCardRefunds(AsyncAPIResource):
@@ -60,14 +64,15 @@
         *,
         transaction_id: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> Transaction:
         """Simulates refunding a card transaction.
 
         The full value of the original sandbox
         transaction is refunded.
 
@@ -77,20 +82,23 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             "/simulations/card_refunds",
             body=maybe_transform({"transaction_id": transaction_id}, card_refund_create_params.CardRefundCreateParams),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=Transaction,
         )
```

### Comparing `increase-0.5.0/src/increase/resources/simulations/cards.py` & `increase-0.6.0/src/increase/resources/bookkeeping_accounts.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,248 +1,234 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from ...types import Transaction
-from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
-from ..._utils import maybe_transform
-from ..._resource import SyncAPIResource, AsyncAPIResource
-from ..._base_client import make_request_options
-from ...types.simulations import (
-    CardAuthorizationSimulation,
-    card_authorize_params,
-    card_settlement_params,
+from typing_extensions import Literal
+
+from ..types import (
+    BookkeepingAccount,
+    bookkeeping_account_list_params,
+    bookkeeping_account_create_params,
 )
+from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
+from .._utils import maybe_transform
+from .._resource import SyncAPIResource, AsyncAPIResource
+from ..pagination import SyncPage, AsyncPage
+from .._base_client import AsyncPaginator, make_request_options
 
-__all__ = ["Cards", "AsyncCards"]
+__all__ = ["BookkeepingAccounts", "AsyncBookkeepingAccounts"]
 
 
-class Cards(SyncAPIResource):
-    def authorize(
+class BookkeepingAccounts(SyncAPIResource):
+    def create(
         self,
         *,
-        amount: int,
-        card_id: str | NotGiven = NOT_GIVEN,
-        digital_wallet_token_id: str | NotGiven = NOT_GIVEN,
+        name: str,
+        account_id: str | NotGiven = NOT_GIVEN,
+        compliance_category: Literal["commingled_cash", "customer_balance"] | NotGiven = NOT_GIVEN,
+        entity_id: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
-    ) -> CardAuthorizationSimulation:
-        """Simulates a purchase authorization on a [Card](#cards).
-
-        Depending on the balance
-        available to the card and the `amount` submitted, the authorization activity
-        will result in a [Pending Transaction](#pending-transactions) of type
-        `card_authorization` or a [Declined Transaction](#declined-transactions) of type
-        `card_decline`. You can pass either a Card id or a
-        [Digital Wallet Token](#digital-wallet-tokens) id to simulate the two different
-        ways purchases can be made.
+    ) -> BookkeepingAccount:
+        """
+        Create a Bookkeeping Account
 
         Args:
-          amount: The authorization amount in cents.
+          name: The name you choose for the account.
+
+          account_id: The entity, if `compliance_category` is `commingled_cash`.
 
-          card_id: The identifier of the Card to be authorized.
+          compliance_category: The account compliance category.
 
-          digital_wallet_token_id: The identifier of the Digital Wallet Token to be authorized.
+          entity_id: The entity, if `compliance_category` is `customer_balance`.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
-            "/simulations/card_authorizations",
+            "/bookkeeping_accounts",
             body=maybe_transform(
                 {
-                    "amount": amount,
-                    "card_id": card_id,
-                    "digital_wallet_token_id": digital_wallet_token_id,
+                    "compliance_category": compliance_category,
+                    "entity_id": entity_id,
+                    "account_id": account_id,
+                    "name": name,
                 },
-                card_authorize_params.CardAuthorizeParams,
+                bookkeeping_account_create_params.BookkeepingAccountCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
-            cast_to=CardAuthorizationSimulation,
+            cast_to=BookkeepingAccount,
         )
 
-    def settlement(
+    def list(
         self,
         *,
-        card_id: str,
-        pending_transaction_id: str,
-        amount: int | NotGiven = NOT_GIVEN,
+        cursor: str | NotGiven = NOT_GIVEN,
+        limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
-        idempotency_key: str | None = None,
-    ) -> Transaction:
-        """Simulates the settlement of an authorization by a card acquirer.
-
-        After a card
-        authorization is created, the merchant will eventually send a settlement. This
-        simulates that event, which may occur many days after the purchase in
-        production. The amount settled can be different from the amount originally
-        authorized, for example, when adding a tip to a restaurant bill.
+        timeout: float | None | NotGiven = NOT_GIVEN,
+    ) -> SyncPage[BookkeepingAccount]:
+        """
+        List Bookkeeping Accounts
 
         Args:
-          card_id: The identifier of the Card to create a settlement on.
+          cursor: Return the page of entries after this one.
 
-          pending_transaction_id: The identifier of the Pending Transaction for the Card Authorization you wish to
-              settle.
-
-          amount: The amount to be settled. This defaults to the amount of the Pending Transaction
-              being settled.
+          limit: Limit the size of the list that is returned. The default (and maximum) is 100
+              objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
-          idempotency_key: Specify a custom idempotency key for this request
+          timeout: Override the client-level default timeout for this request, in seconds
         """
-        return self._post(
-            "/simulations/card_settlements",
-            body=maybe_transform(
-                {
-                    "card_id": card_id,
-                    "pending_transaction_id": pending_transaction_id,
-                    "amount": amount,
-                },
-                card_settlement_params.CardSettlementParams,
-            ),
+        return self._get_api_list(
+            "/bookkeeping_accounts",
+            page=SyncPage[BookkeepingAccount],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                idempotency_key=idempotency_key,
+                timeout=timeout,
+                query=maybe_transform(
+                    {
+                        "cursor": cursor,
+                        "limit": limit,
+                    },
+                    bookkeeping_account_list_params.BookkeepingAccountListParams,
+                ),
             ),
-            cast_to=Transaction,
+            model=BookkeepingAccount,
         )
 
 
-class AsyncCards(AsyncAPIResource):
-    async def authorize(
+class AsyncBookkeepingAccounts(AsyncAPIResource):
+    async def create(
         self,
         *,
-        amount: int,
-        card_id: str | NotGiven = NOT_GIVEN,
-        digital_wallet_token_id: str | NotGiven = NOT_GIVEN,
+        name: str,
+        account_id: str | NotGiven = NOT_GIVEN,
+        compliance_category: Literal["commingled_cash", "customer_balance"] | NotGiven = NOT_GIVEN,
+        entity_id: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
-    ) -> CardAuthorizationSimulation:
-        """Simulates a purchase authorization on a [Card](#cards).
-
-        Depending on the balance
-        available to the card and the `amount` submitted, the authorization activity
-        will result in a [Pending Transaction](#pending-transactions) of type
-        `card_authorization` or a [Declined Transaction](#declined-transactions) of type
-        `card_decline`. You can pass either a Card id or a
-        [Digital Wallet Token](#digital-wallet-tokens) id to simulate the two different
-        ways purchases can be made.
+    ) -> BookkeepingAccount:
+        """
+        Create a Bookkeeping Account
 
         Args:
-          amount: The authorization amount in cents.
+          name: The name you choose for the account.
 
-          card_id: The identifier of the Card to be authorized.
+          account_id: The entity, if `compliance_category` is `commingled_cash`.
 
-          digital_wallet_token_id: The identifier of the Digital Wallet Token to be authorized.
+          compliance_category: The account compliance category.
+
+          entity_id: The entity, if `compliance_category` is `customer_balance`.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
-            "/simulations/card_authorizations",
+            "/bookkeeping_accounts",
             body=maybe_transform(
                 {
-                    "amount": amount,
-                    "card_id": card_id,
-                    "digital_wallet_token_id": digital_wallet_token_id,
+                    "compliance_category": compliance_category,
+                    "entity_id": entity_id,
+                    "account_id": account_id,
+                    "name": name,
                 },
-                card_authorize_params.CardAuthorizeParams,
+                bookkeeping_account_create_params.BookkeepingAccountCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
-            cast_to=CardAuthorizationSimulation,
+            cast_to=BookkeepingAccount,
         )
 
-    async def settlement(
+    def list(
         self,
         *,
-        card_id: str,
-        pending_transaction_id: str,
-        amount: int | NotGiven = NOT_GIVEN,
+        cursor: str | NotGiven = NOT_GIVEN,
+        limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
-        idempotency_key: str | None = None,
-    ) -> Transaction:
-        """Simulates the settlement of an authorization by a card acquirer.
-
-        After a card
-        authorization is created, the merchant will eventually send a settlement. This
-        simulates that event, which may occur many days after the purchase in
-        production. The amount settled can be different from the amount originally
-        authorized, for example, when adding a tip to a restaurant bill.
+        timeout: float | None | NotGiven = NOT_GIVEN,
+    ) -> AsyncPaginator[BookkeepingAccount, AsyncPage[BookkeepingAccount]]:
+        """
+        List Bookkeeping Accounts
 
         Args:
-          card_id: The identifier of the Card to create a settlement on.
-
-          pending_transaction_id: The identifier of the Pending Transaction for the Card Authorization you wish to
-              settle.
+          cursor: Return the page of entries after this one.
 
-          amount: The amount to be settled. This defaults to the amount of the Pending Transaction
-              being settled.
+          limit: Limit the size of the list that is returned. The default (and maximum) is 100
+              objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
-          idempotency_key: Specify a custom idempotency key for this request
+          timeout: Override the client-level default timeout for this request, in seconds
         """
-        return await self._post(
-            "/simulations/card_settlements",
-            body=maybe_transform(
-                {
-                    "card_id": card_id,
-                    "pending_transaction_id": pending_transaction_id,
-                    "amount": amount,
-                },
-                card_settlement_params.CardSettlementParams,
-            ),
+        return self._get_api_list(
+            "/bookkeeping_accounts",
+            page=AsyncPage[BookkeepingAccount],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                idempotency_key=idempotency_key,
+                timeout=timeout,
+                query=maybe_transform(
+                    {
+                        "cursor": cursor,
+                        "limit": limit,
+                    },
+                    bookkeeping_account_list_params.BookkeepingAccountListParams,
+                ),
             ),
-            cast_to=Transaction,
+            model=BookkeepingAccount,
         )
```

### Comparing `increase-0.5.0/src/increase/resources/simulations/check_deposits.py` & `increase-0.6.0/src/increase/resources/simulations/check_deposits.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
 from ...types import CheckDeposit
-from ..._types import Body, Query, Headers
+from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ..._base_client import make_request_options
 
 __all__ = ["CheckDeposits", "AsyncCheckDeposits"]
 
 
 class CheckDeposits(SyncAPIResource):
@@ -16,80 +16,86 @@
         check_deposit_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> CheckDeposit:
         """
         Simulates the rejection of a [Check Deposit](#check-deposits) by Increase due to
         factors like poor image quality. This Check Deposit must first have a `status`
         of `pending`.
         """
         return self._post(
             f"/simulations/check_deposits/{check_deposit_id}/reject",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=CheckDeposit,
         )
 
     def return_(
         self,
         check_deposit_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> CheckDeposit:
         """Simulates the return of a [Check Deposit](#check-deposits).
 
         This Check Deposit
         must first have a `status` of `submitted`.
         """
         return self._post(
             f"/simulations/check_deposits/{check_deposit_id}/return",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=CheckDeposit,
         )
 
     def submit(
         self,
         check_deposit_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> CheckDeposit:
         """
         Simulates the submission of a [Check Deposit](#check-deposits) to the Federal
         Reserve. This Check Deposit must first have a `status` of `pending`.
         """
         return self._post(
             f"/simulations/check_deposits/{check_deposit_id}/submit",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=CheckDeposit,
         )
 
 
 class AsyncCheckDeposits(AsyncAPIResource):
@@ -98,77 +104,83 @@
         check_deposit_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> CheckDeposit:
         """
         Simulates the rejection of a [Check Deposit](#check-deposits) by Increase due to
         factors like poor image quality. This Check Deposit must first have a `status`
         of `pending`.
         """
         return await self._post(
             f"/simulations/check_deposits/{check_deposit_id}/reject",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=CheckDeposit,
         )
 
     async def return_(
         self,
         check_deposit_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> CheckDeposit:
         """Simulates the return of a [Check Deposit](#check-deposits).
 
         This Check Deposit
         must first have a `status` of `submitted`.
         """
         return await self._post(
             f"/simulations/check_deposits/{check_deposit_id}/return",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=CheckDeposit,
         )
 
     async def submit(
         self,
         check_deposit_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> CheckDeposit:
         """
         Simulates the submission of a [Check Deposit](#check-deposits) to the Federal
         Reserve. This Check Deposit must first have a `status` of `pending`.
         """
         return await self._post(
             f"/simulations/check_deposits/{check_deposit_id}/submit",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=CheckDeposit,
         )
```

### Comparing `increase-0.5.0/src/increase/resources/simulations/check_transfers.py` & `increase-0.6.0/src/increase/resources/simulations/interest_payments.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,122 +1,122 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from ...types import CheckTransfer
-from ..._types import Body, Query, Headers
+from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
+from ..._utils import maybe_transform
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ..._base_client import make_request_options
+from ...types.simulations import (
+    InterestPaymentSimulationResult,
+    interest_payment_create_params,
+)
 
-__all__ = ["CheckTransfers", "AsyncCheckTransfers"]
+__all__ = ["InterestPayments", "AsyncInterestPayments"]
 
 
-class CheckTransfers(SyncAPIResource):
-    def deposit(
+class InterestPayments(SyncAPIResource):
+    def create(
         self,
-        check_transfer_id: str,
         *,
+        account_id: str,
+        amount: int,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
-    ) -> CheckTransfer:
-        """Simulates a [Check Transfer](#check-transfers) being deposited at a bank.
+    ) -> InterestPaymentSimulationResult:
+        """Simulates an interest payment to your account.
 
-        This
-        transfer must first have a `status` of `mailed`.
-        """
-        return self._post(
-            f"/simulations/check_transfers/{check_transfer_id}/deposit",
-            options=make_request_options(
-                extra_headers=extra_headers,
-                extra_query=extra_query,
-                extra_body=extra_body,
-                idempotency_key=idempotency_key,
-            ),
-            cast_to=CheckTransfer,
-        )
+        In production, this happens
+        automatically on the first of each month.
 
-    def mail(
-        self,
-        check_transfer_id: str,
-        *,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        idempotency_key: str | None = None,
-    ) -> CheckTransfer:
-        """
-        Simulates the mailing of a [Check Transfer](#check-transfers), which happens
-        once per weekday in production but can be sped up in sandbox. This transfer must
-        first have a `status` of `pending_approval` or `pending_submission`.
+        Args:
+          account_id: The identifier of the Account Number the Interest Payment is for.
+
+          amount: The interest amount in cents. Must be positive.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
-            f"/simulations/check_transfers/{check_transfer_id}/mail",
+            "/simulations/interest_payment",
+            body=maybe_transform(
+                {
+                    "account_id": account_id,
+                    "amount": amount,
+                },
+                interest_payment_create_params.InterestPaymentCreateParams,
+            ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
-            cast_to=CheckTransfer,
+            cast_to=InterestPaymentSimulationResult,
         )
 
 
-class AsyncCheckTransfers(AsyncAPIResource):
-    async def deposit(
+class AsyncInterestPayments(AsyncAPIResource):
+    async def create(
         self,
-        check_transfer_id: str,
         *,
+        account_id: str,
+        amount: int,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
-    ) -> CheckTransfer:
-        """Simulates a [Check Transfer](#check-transfers) being deposited at a bank.
+    ) -> InterestPaymentSimulationResult:
+        """Simulates an interest payment to your account.
 
-        This
-        transfer must first have a `status` of `mailed`.
-        """
-        return await self._post(
-            f"/simulations/check_transfers/{check_transfer_id}/deposit",
-            options=make_request_options(
-                extra_headers=extra_headers,
-                extra_query=extra_query,
-                extra_body=extra_body,
-                idempotency_key=idempotency_key,
-            ),
-            cast_to=CheckTransfer,
-        )
+        In production, this happens
+        automatically on the first of each month.
 
-    async def mail(
-        self,
-        check_transfer_id: str,
-        *,
-        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
-        # The extra values given here take precedence over values defined on the client or passed to this method.
-        extra_headers: Headers | None = None,
-        extra_query: Query | None = None,
-        extra_body: Body | None = None,
-        idempotency_key: str | None = None,
-    ) -> CheckTransfer:
-        """
-        Simulates the mailing of a [Check Transfer](#check-transfers), which happens
-        once per weekday in production but can be sped up in sandbox. This transfer must
-        first have a `status` of `pending_approval` or `pending_submission`.
+        Args:
+          account_id: The identifier of the Account Number the Interest Payment is for.
+
+          amount: The interest amount in cents. Must be positive.
+
+          extra_headers: Send extra headers
+
+          extra_query: Add additional query parameters to the request
+
+          extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
+
+          idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
-            f"/simulations/check_transfers/{check_transfer_id}/mail",
+            "/simulations/interest_payment",
+            body=maybe_transform(
+                {
+                    "account_id": account_id,
+                    "amount": amount,
+                },
+                interest_payment_create_params.InterestPaymentCreateParams,
+            ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
-            cast_to=CheckTransfer,
+            cast_to=InterestPaymentSimulationResult,
         )
```

### Comparing `increase-0.5.0/src/increase/resources/simulations/digital_wallet_token_requests.py` & `increase-0.6.0/src/increase/resources/simulations/digital_wallet_token_requests.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from ..._types import Body, Query, Headers
+from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from ..._utils import maybe_transform
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ..._base_client import make_request_options
 from ...types.simulations import (
     DigitalWalletTokenRequestCreateResponse,
     digital_wallet_token_request_create_params,
 )
@@ -20,14 +20,15 @@
         *,
         card_id: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> DigitalWalletTokenRequestCreateResponse:
         """
         Simulates a user attempting add a [Card](#cards) to a digital wallet such as
         Apple Pay.
 
         Args:
@@ -35,25 +36,28 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             "/simulations/digital_wallet_token_requests",
             body=maybe_transform(
                 {"card_id": card_id}, digital_wallet_token_request_create_params.DigitalWalletTokenRequestCreateParams
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=DigitalWalletTokenRequestCreateResponse,
         )
 
 
 class AsyncDigitalWalletTokenRequests(AsyncAPIResource):
@@ -62,14 +66,15 @@
         *,
         card_id: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> DigitalWalletTokenRequestCreateResponse:
         """
         Simulates a user attempting add a [Card](#cards) to a digital wallet such as
         Apple Pay.
 
         Args:
@@ -77,22 +82,25 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             "/simulations/digital_wallet_token_requests",
             body=maybe_transform(
                 {"card_id": card_id}, digital_wallet_token_request_create_params.DigitalWalletTokenRequestCreateParams
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=DigitalWalletTokenRequestCreateResponse,
         )
```

### Comparing `increase-0.5.0/src/increase/resources/simulations/documents.py` & `increase-0.6.0/src/increase/resources/simulations/documents.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
 from ...types import Document
-from ..._types import Body, Query, Headers
+from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from ..._utils import maybe_transform
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ..._base_client import make_request_options
 from ...types.simulations import document_create_params
 
 __all__ = ["Documents", "AsyncDocuments"]
 
@@ -18,37 +18,41 @@
         *,
         account_id: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> Document:
         """
         Simulates an tax document being created for an account.
 
         Args:
           account_id: The identifier of the Account the tax document is for.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             "/simulations/documents",
             body=maybe_transform({"account_id": account_id}, document_create_params.DocumentCreateParams),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=Document,
         )
 
 
 class AsyncDocuments(AsyncAPIResource):
@@ -57,34 +61,38 @@
         *,
         account_id: str,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> Document:
         """
         Simulates an tax document being created for an account.
 
         Args:
           account_id: The identifier of the Account the tax document is for.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             "/simulations/documents",
             body=maybe_transform({"account_id": account_id}, document_create_params.DocumentCreateParams),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=Document,
         )
```

### Comparing `increase-0.5.0/src/increase/resources/simulations/inbound_wire_drawdown_requests.py` & `increase-0.6.0/src/increase/resources/simulations/inbound_wire_drawdown_requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         originator_to_beneficiary_information_line3: str | NotGiven = NOT_GIVEN,
         originator_to_beneficiary_information_line4: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> InboundWireDrawdownRequest:
         """
         Simulates the receival of an
         [Inbound Wire Drawdown Request](#inbound-wire-drawdown-requests).
 
         Args:
@@ -96,14 +97,16 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             "/simulations/inbound_wire_drawdown_requests",
             body=maybe_transform(
                 {
                     "recipient_account_number_id": recipient_account_number_id,
@@ -129,14 +132,15 @@
                 },
                 inbound_wire_drawdown_request_create_params.InboundWireDrawdownRequestCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=InboundWireDrawdownRequest,
         )
 
 
 class AsyncInboundWireDrawdownRequests(AsyncAPIResource):
@@ -164,14 +168,15 @@
         originator_to_beneficiary_information_line3: str | NotGiven = NOT_GIVEN,
         originator_to_beneficiary_information_line4: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> InboundWireDrawdownRequest:
         """
         Simulates the receival of an
         [Inbound Wire Drawdown Request](#inbound-wire-drawdown-requests).
 
         Args:
@@ -223,14 +228,16 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             "/simulations/inbound_wire_drawdown_requests",
             body=maybe_transform(
                 {
                     "recipient_account_number_id": recipient_account_number_id,
@@ -256,11 +263,12 @@
                 },
                 inbound_wire_drawdown_request_create_params.InboundWireDrawdownRequestCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=InboundWireDrawdownRequest,
         )
```

### Comparing `increase-0.5.0/src/increase/resources/simulations/real_time_payments_transfers.py` & `increase-0.6.0/src/increase/resources/simulations/check_transfers.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,156 +1,220 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
+from typing_extensions import Literal
+
+from ...types import CheckTransfer
 from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from ..._utils import maybe_transform
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ..._base_client import make_request_options
-from ...types.simulations import (
-    InboundRealTimePaymentsTransferSimulationResult,
-    real_time_payments_transfer_create_inbound_params,
-)
+from ...types.simulations import check_transfer_return_params
 
-__all__ = ["RealTimePaymentsTransfers", "AsyncRealTimePaymentsTransfers"]
+__all__ = ["CheckTransfers", "AsyncCheckTransfers"]
 
 
-class RealTimePaymentsTransfers(SyncAPIResource):
-    def create_inbound(
+class CheckTransfers(SyncAPIResource):
+    def deposit(
         self,
+        check_transfer_id: str,
         *,
-        account_number_id: str,
-        amount: int,
-        debtor_account_number: str | NotGiven = NOT_GIVEN,
-        debtor_name: str | NotGiven = NOT_GIVEN,
-        debtor_routing_number: str | NotGiven = NOT_GIVEN,
-        remittance_information: str | NotGiven = NOT_GIVEN,
-        request_for_payment_id: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
-    ) -> InboundRealTimePaymentsTransferSimulationResult:
-        """Simulates an inbound Real Time Payments transfer to your account.
-
-        Real Time
-        Payments are a beta feature.
-
-        Args:
-          account_number_id: The identifier of the Account Number the inbound Real Time Payments Transfer is
-              for.
-
-          amount: The transfer amount in USD cents. Must be positive.
-
-          debtor_account_number: The account number of the account that sent the transfer.
+    ) -> CheckTransfer:
+        """Simulates a [Check Transfer](#check-transfers) being deposited at a bank.
 
-          debtor_name: The name provided by the sender of the transfer.
+        This
+        transfer must first have a `status` of `mailed`.
+        """
+        return self._post(
+            f"/simulations/check_transfers/{check_transfer_id}/deposit",
+            options=make_request_options(
+                extra_headers=extra_headers,
+                extra_query=extra_query,
+                extra_body=extra_body,
+                timeout=timeout,
+                idempotency_key=idempotency_key,
+            ),
+            cast_to=CheckTransfer,
+        )
 
-          debtor_routing_number: The routing number of the account that sent the transfer.
+    def mail(
+        self,
+        check_transfer_id: str,
+        *,
+        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
+        # The extra values given here take precedence over values defined on the client or passed to this method.
+        extra_headers: Headers | None = None,
+        extra_query: Query | None = None,
+        extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
+        idempotency_key: str | None = None,
+    ) -> CheckTransfer:
+        """
+        Simulates the mailing of a [Check Transfer](#check-transfers), which happens
+        once per weekday in production but can be sped up in sandbox. This transfer must
+        first have a `status` of `pending_approval` or `pending_submission`.
+        """
+        return self._post(
+            f"/simulations/check_transfers/{check_transfer_id}/mail",
+            options=make_request_options(
+                extra_headers=extra_headers,
+                extra_query=extra_query,
+                extra_body=extra_body,
+                timeout=timeout,
+                idempotency_key=idempotency_key,
+            ),
+            cast_to=CheckTransfer,
+        )
 
-          remittance_information: Additional information included with the transfer.
+    def return_(
+        self,
+        check_transfer_id: str,
+        *,
+        reason: Literal["mail_delivery_failure", "refused_by_recipient", "returned_not_authorized"],
+        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
+        # The extra values given here take precedence over values defined on the client or passed to this method.
+        extra_headers: Headers | None = None,
+        extra_query: Query | None = None,
+        extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
+        idempotency_key: str | None = None,
+    ) -> CheckTransfer:
+        """
+        Simulates a [Check Transfer](#check-transfers) being returned via USPS to
+        Increase. This transfer must first have a `status` of `mailed`.
 
-          request_for_payment_id: The identifier of a pending Request for Payment that this transfer will fulfill.
+        Args:
+          reason: The reason why the Check Transfer was returned to Increase.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
-            "/simulations/inbound_real_time_payments_transfers",
-            body=maybe_transform(
-                {
-                    "account_number_id": account_number_id,
-                    "amount": amount,
-                    "request_for_payment_id": request_for_payment_id,
-                    "debtor_name": debtor_name,
-                    "debtor_account_number": debtor_account_number,
-                    "debtor_routing_number": debtor_routing_number,
-                    "remittance_information": remittance_information,
-                },
-                real_time_payments_transfer_create_inbound_params.RealTimePaymentsTransferCreateInboundParams,
-            ),
+            f"/simulations/check_transfers/{check_transfer_id}/return",
+            body=maybe_transform({"reason": reason}, check_transfer_return_params.CheckTransferReturnParams),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
-            cast_to=InboundRealTimePaymentsTransferSimulationResult,
+            cast_to=CheckTransfer,
         )
 
 
-class AsyncRealTimePaymentsTransfers(AsyncAPIResource):
-    async def create_inbound(
+class AsyncCheckTransfers(AsyncAPIResource):
+    async def deposit(
         self,
+        check_transfer_id: str,
         *,
-        account_number_id: str,
-        amount: int,
-        debtor_account_number: str | NotGiven = NOT_GIVEN,
-        debtor_name: str | NotGiven = NOT_GIVEN,
-        debtor_routing_number: str | NotGiven = NOT_GIVEN,
-        remittance_information: str | NotGiven = NOT_GIVEN,
-        request_for_payment_id: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
-    ) -> InboundRealTimePaymentsTransferSimulationResult:
-        """Simulates an inbound Real Time Payments transfer to your account.
+    ) -> CheckTransfer:
+        """Simulates a [Check Transfer](#check-transfers) being deposited at a bank.
 
-        Real Time
-        Payments are a beta feature.
-
-        Args:
-          account_number_id: The identifier of the Account Number the inbound Real Time Payments Transfer is
-              for.
-
-          amount: The transfer amount in USD cents. Must be positive.
-
-          debtor_account_number: The account number of the account that sent the transfer.
-
-          debtor_name: The name provided by the sender of the transfer.
+        This
+        transfer must first have a `status` of `mailed`.
+        """
+        return await self._post(
+            f"/simulations/check_transfers/{check_transfer_id}/deposit",
+            options=make_request_options(
+                extra_headers=extra_headers,
+                extra_query=extra_query,
+                extra_body=extra_body,
+                timeout=timeout,
+                idempotency_key=idempotency_key,
+            ),
+            cast_to=CheckTransfer,
+        )
 
-          debtor_routing_number: The routing number of the account that sent the transfer.
+    async def mail(
+        self,
+        check_transfer_id: str,
+        *,
+        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
+        # The extra values given here take precedence over values defined on the client or passed to this method.
+        extra_headers: Headers | None = None,
+        extra_query: Query | None = None,
+        extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
+        idempotency_key: str | None = None,
+    ) -> CheckTransfer:
+        """
+        Simulates the mailing of a [Check Transfer](#check-transfers), which happens
+        once per weekday in production but can be sped up in sandbox. This transfer must
+        first have a `status` of `pending_approval` or `pending_submission`.
+        """
+        return await self._post(
+            f"/simulations/check_transfers/{check_transfer_id}/mail",
+            options=make_request_options(
+                extra_headers=extra_headers,
+                extra_query=extra_query,
+                extra_body=extra_body,
+                timeout=timeout,
+                idempotency_key=idempotency_key,
+            ),
+            cast_to=CheckTransfer,
+        )
 
-          remittance_information: Additional information included with the transfer.
+    async def return_(
+        self,
+        check_transfer_id: str,
+        *,
+        reason: Literal["mail_delivery_failure", "refused_by_recipient", "returned_not_authorized"],
+        # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
+        # The extra values given here take precedence over values defined on the client or passed to this method.
+        extra_headers: Headers | None = None,
+        extra_query: Query | None = None,
+        extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
+        idempotency_key: str | None = None,
+    ) -> CheckTransfer:
+        """
+        Simulates a [Check Transfer](#check-transfers) being returned via USPS to
+        Increase. This transfer must first have a `status` of `mailed`.
 
-          request_for_payment_id: The identifier of a pending Request for Payment that this transfer will fulfill.
+        Args:
+          reason: The reason why the Check Transfer was returned to Increase.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
-            "/simulations/inbound_real_time_payments_transfers",
-            body=maybe_transform(
-                {
-                    "account_number_id": account_number_id,
-                    "amount": amount,
-                    "request_for_payment_id": request_for_payment_id,
-                    "debtor_name": debtor_name,
-                    "debtor_account_number": debtor_account_number,
-                    "debtor_routing_number": debtor_routing_number,
-                    "remittance_information": remittance_information,
-                },
-                real_time_payments_transfer_create_inbound_params.RealTimePaymentsTransferCreateInboundParams,
-            ),
+            f"/simulations/check_transfers/{check_transfer_id}/return",
+            body=maybe_transform({"reason": reason}, check_transfer_return_params.CheckTransferReturnParams),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
-            cast_to=InboundRealTimePaymentsTransferSimulationResult,
+            cast_to=CheckTransfer,
         )
```

### Comparing `increase-0.5.0/src/increase/resources/simulations/simulations.py` & `increase-0.6.0/src/increase/resources/simulations/simulations.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from .card_refunds import CardRefunds, AsyncCardRefunds
 from .ach_transfers import ACHTransfers, AsyncACHTransfers
 from .card_disputes import CardDisputes, AsyncCardDisputes
 from .check_deposits import CheckDeposits, AsyncCheckDeposits
 from .wire_transfers import WireTransfers, AsyncWireTransfers
 from .check_transfers import CheckTransfers, AsyncCheckTransfers
 from .account_transfers import AccountTransfers, AsyncAccountTransfers
+from .interest_payments import InterestPayments, AsyncInterestPayments
 from .account_statements import AccountStatements, AsyncAccountStatements
 from .real_time_payments_transfers import (
     RealTimePaymentsTransfers,
     AsyncRealTimePaymentsTransfers,
 )
 from .digital_wallet_token_requests import (
     DigitalWalletTokenRequests,
@@ -41,14 +42,15 @@
     card_disputes: CardDisputes
     card_refunds: CardRefunds
     check_transfers: CheckTransfers
     documents: Documents
     digital_wallet_token_requests: DigitalWalletTokenRequests
     check_deposits: CheckDeposits
     inbound_wire_drawdown_requests: InboundWireDrawdownRequests
+    interest_payments: InterestPayments
     wire_transfers: WireTransfers
     cards: Cards
     real_time_payments_transfers: RealTimePaymentsTransfers
 
     def __init__(self, client: Increase) -> None:
         super().__init__(client)
         self.account_transfers = AccountTransfers(client)
@@ -57,14 +59,15 @@
         self.card_disputes = CardDisputes(client)
         self.card_refunds = CardRefunds(client)
         self.check_transfers = CheckTransfers(client)
         self.documents = Documents(client)
         self.digital_wallet_token_requests = DigitalWalletTokenRequests(client)
         self.check_deposits = CheckDeposits(client)
         self.inbound_wire_drawdown_requests = InboundWireDrawdownRequests(client)
+        self.interest_payments = InterestPayments(client)
         self.wire_transfers = WireTransfers(client)
         self.cards = Cards(client)
         self.real_time_payments_transfers = RealTimePaymentsTransfers(client)
 
 
 class AsyncSimulations(AsyncAPIResource):
     account_transfers: AsyncAccountTransfers
@@ -73,14 +76,15 @@
     card_disputes: AsyncCardDisputes
     card_refunds: AsyncCardRefunds
     check_transfers: AsyncCheckTransfers
     documents: AsyncDocuments
     digital_wallet_token_requests: AsyncDigitalWalletTokenRequests
     check_deposits: AsyncCheckDeposits
     inbound_wire_drawdown_requests: AsyncInboundWireDrawdownRequests
+    interest_payments: AsyncInterestPayments
     wire_transfers: AsyncWireTransfers
     cards: AsyncCards
     real_time_payments_transfers: AsyncRealTimePaymentsTransfers
 
     def __init__(self, client: AsyncIncrease) -> None:
         super().__init__(client)
         self.account_transfers = AsyncAccountTransfers(client)
@@ -89,10 +93,11 @@
         self.card_disputes = AsyncCardDisputes(client)
         self.card_refunds = AsyncCardRefunds(client)
         self.check_transfers = AsyncCheckTransfers(client)
         self.documents = AsyncDocuments(client)
         self.digital_wallet_token_requests = AsyncDigitalWalletTokenRequests(client)
         self.check_deposits = AsyncCheckDeposits(client)
         self.inbound_wire_drawdown_requests = AsyncInboundWireDrawdownRequests(client)
+        self.interest_payments = AsyncInterestPayments(client)
         self.wire_transfers = AsyncWireTransfers(client)
         self.cards = AsyncCards(client)
         self.real_time_payments_transfers = AsyncRealTimePaymentsTransfers(client)
```

### Comparing `increase-0.5.0/src/increase/resources/simulations/wire_transfers.py` & `increase-0.6.0/src/increase/resources/simulations/wire_transfers.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,15 @@
         originator_to_beneficiary_information_line3: str | NotGiven = NOT_GIVEN,
         originator_to_beneficiary_information_line4: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> WireTransferSimulation:
         """
         Simulates an inbound Wire Transfer to your account.
 
         Args:
           account_number_id: The identifier of the Account Number the inbound Wire Transfer is for.
@@ -89,14 +90,16 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             "/simulations/inbound_wire_transfers",
             body=maybe_transform(
                 {
                     "account_number_id": account_number_id,
@@ -117,14 +120,15 @@
                 },
                 wire_transfer_create_inbound_params.WireTransferCreateInboundParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=WireTransferSimulation,
         )
 
 
 class AsyncWireTransfers(AsyncAPIResource):
@@ -147,14 +151,15 @@
         originator_to_beneficiary_information_line3: str | NotGiven = NOT_GIVEN,
         originator_to_beneficiary_information_line4: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> WireTransferSimulation:
         """
         Simulates an inbound Wire Transfer to your account.
 
         Args:
           account_number_id: The identifier of the Account Number the inbound Wire Transfer is for.
@@ -202,14 +207,16 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             "/simulations/inbound_wire_transfers",
             body=maybe_transform(
                 {
                     "account_number_id": account_number_id,
@@ -230,11 +237,12 @@
                 },
                 wire_transfer_create_inbound_params.WireTransferCreateInboundParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=WireTransferSimulation,
         )
```

### Comparing `increase-0.5.0/src/increase/resources/transactions.py` & `increase-0.6.0/src/increase/resources/pending_transactions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,162 +1,184 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from ..types import Transaction, transaction_list_params
+from ..types import PendingTransaction, pending_transaction_list_params
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from .._utils import maybe_transform
 from .._resource import SyncAPIResource, AsyncAPIResource
 from ..pagination import SyncPage, AsyncPage
 from .._base_client import AsyncPaginator, make_request_options
 
-__all__ = ["Transactions", "AsyncTransactions"]
+__all__ = ["PendingTransactions", "AsyncPendingTransactions"]
 
 
-class Transactions(SyncAPIResource):
+class PendingTransactions(SyncAPIResource):
     def retrieve(
         self,
-        transaction_id: str,
+        pending_transaction_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
-    ) -> Transaction:
-        """Retrieve a Transaction"""
+        timeout: float | None | NotGiven = NOT_GIVEN,
+    ) -> PendingTransaction:
+        """Retrieve a Pending Transaction"""
         return self._get(
-            f"/transactions/{transaction_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
-            cast_to=Transaction,
+            f"/pending_transactions/{pending_transaction_id}",
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
+            cast_to=PendingTransaction,
         )
 
     def list(
         self,
         *,
         account_id: str | NotGiven = NOT_GIVEN,
-        category: transaction_list_params.Category | NotGiven = NOT_GIVEN,
-        created_at: transaction_list_params.CreatedAt | NotGiven = NOT_GIVEN,
+        created_at: pending_transaction_list_params.CreatedAt | NotGiven = NOT_GIVEN,
         cursor: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         route_id: str | NotGiven = NOT_GIVEN,
+        source_id: str | NotGiven = NOT_GIVEN,
+        status: pending_transaction_list_params.Status | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
-    ) -> SyncPage[Transaction]:
+        timeout: float | None | NotGiven = NOT_GIVEN,
+    ) -> SyncPage[PendingTransaction]:
         """
-        List Transactions
+        List Pending Transactions
 
         Args:
-          account_id: Filter Transactions for those belonging to the specified Account.
+          account_id: Filter pending transactions to those belonging to the specified Account.
 
           cursor: Return the page of entries after this one.
 
           limit: Limit the size of the list that is returned. The default (and maximum) is 100
               objects.
 
-          route_id: Filter Transactions for those belonging to the specified route.
+          route_id: Filter pending transactions to those belonging to the specified Route.
+
+          source_id: Filter pending transactions to those caused by the specified source.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
-            "/transactions",
-            page=SyncPage[Transaction],
+            "/pending_transactions",
+            page=SyncPage[PendingTransaction],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                         "account_id": account_id,
                         "route_id": route_id,
+                        "source_id": source_id,
+                        "status": status,
                         "created_at": created_at,
-                        "category": category,
                     },
-                    transaction_list_params.TransactionListParams,
+                    pending_transaction_list_params.PendingTransactionListParams,
                 ),
             ),
-            model=Transaction,
+            model=PendingTransaction,
         )
 
 
-class AsyncTransactions(AsyncAPIResource):
+class AsyncPendingTransactions(AsyncAPIResource):
     async def retrieve(
         self,
-        transaction_id: str,
+        pending_transaction_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
-    ) -> Transaction:
-        """Retrieve a Transaction"""
+        timeout: float | None | NotGiven = NOT_GIVEN,
+    ) -> PendingTransaction:
+        """Retrieve a Pending Transaction"""
         return await self._get(
-            f"/transactions/{transaction_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
-            cast_to=Transaction,
+            f"/pending_transactions/{pending_transaction_id}",
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
+            cast_to=PendingTransaction,
         )
 
     def list(
         self,
         *,
         account_id: str | NotGiven = NOT_GIVEN,
-        category: transaction_list_params.Category | NotGiven = NOT_GIVEN,
-        created_at: transaction_list_params.CreatedAt | NotGiven = NOT_GIVEN,
+        created_at: pending_transaction_list_params.CreatedAt | NotGiven = NOT_GIVEN,
         cursor: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         route_id: str | NotGiven = NOT_GIVEN,
+        source_id: str | NotGiven = NOT_GIVEN,
+        status: pending_transaction_list_params.Status | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
-    ) -> AsyncPaginator[Transaction, AsyncPage[Transaction]]:
+        timeout: float | None | NotGiven = NOT_GIVEN,
+    ) -> AsyncPaginator[PendingTransaction, AsyncPage[PendingTransaction]]:
         """
-        List Transactions
+        List Pending Transactions
 
         Args:
-          account_id: Filter Transactions for those belonging to the specified Account.
+          account_id: Filter pending transactions to those belonging to the specified Account.
 
           cursor: Return the page of entries after this one.
 
           limit: Limit the size of the list that is returned. The default (and maximum) is 100
               objects.
 
-          route_id: Filter Transactions for those belonging to the specified route.
+          route_id: Filter pending transactions to those belonging to the specified Route.
+
+          source_id: Filter pending transactions to those caused by the specified source.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
-            "/transactions",
-            page=AsyncPage[Transaction],
+            "/pending_transactions",
+            page=AsyncPage[PendingTransaction],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                         "account_id": account_id,
                         "route_id": route_id,
+                        "source_id": source_id,
+                        "status": status,
                         "created_at": created_at,
-                        "category": category,
                     },
-                    transaction_list_params.TransactionListParams,
+                    pending_transaction_list_params.PendingTransactionListParams,
                 ),
             ),
-            model=Transaction,
+            model=PendingTransaction,
         )
```

### Comparing `increase-0.5.0/src/increase/resources/wire_drawdown_requests.py` & `increase-0.6.0/src/increase/resources/wire_drawdown_requests.py`

 * *Files 18% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         recipient_address_line2: str | NotGiven = NOT_GIVEN,
         recipient_address_line3: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> WireDrawdownRequest:
         """
         Create a Wire Drawdown Request
 
         Args:
           account_number_id: The Account Number to which the recipient should send funds.
@@ -60,14 +61,16 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             "/wire_drawdown_requests",
             body=maybe_transform(
                 {
                     "account_number_id": account_number_id,
@@ -82,46 +85,51 @@
                 },
                 wire_drawdown_request_create_params.WireDrawdownRequestCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=WireDrawdownRequest,
         )
 
     def retrieve(
         self,
         wire_drawdown_request_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> WireDrawdownRequest:
         """Retrieve a Wire Drawdown Request"""
         return self._get(
             f"/wire_drawdown_requests/{wire_drawdown_request_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=WireDrawdownRequest,
         )
 
     def list(
         self,
         *,
         cursor: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> SyncPage[WireDrawdownRequest]:
         """
         List Wire Drawdown Requests
 
         Args:
           cursor: Return the page of entries after this one.
 
@@ -129,22 +137,25 @@
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/wire_drawdown_requests",
             page=SyncPage[WireDrawdownRequest],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                     },
                     wire_drawdown_request_list_params.WireDrawdownRequestListParams,
                 ),
@@ -167,14 +178,15 @@
         recipient_address_line2: str | NotGiven = NOT_GIVEN,
         recipient_address_line3: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> WireDrawdownRequest:
         """
         Create a Wire Drawdown Request
 
         Args:
           account_number_id: The Account Number to which the recipient should send funds.
@@ -197,14 +209,16 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             "/wire_drawdown_requests",
             body=maybe_transform(
                 {
                     "account_number_id": account_number_id,
@@ -219,46 +233,51 @@
                 },
                 wire_drawdown_request_create_params.WireDrawdownRequestCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=WireDrawdownRequest,
         )
 
     async def retrieve(
         self,
         wire_drawdown_request_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> WireDrawdownRequest:
         """Retrieve a Wire Drawdown Request"""
         return await self._get(
             f"/wire_drawdown_requests/{wire_drawdown_request_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=WireDrawdownRequest,
         )
 
     def list(
         self,
         *,
         cursor: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> AsyncPaginator[WireDrawdownRequest, AsyncPage[WireDrawdownRequest]]:
         """
         List Wire Drawdown Requests
 
         Args:
           cursor: Return the page of entries after this one.
 
@@ -266,22 +285,25 @@
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/wire_drawdown_requests",
             page=AsyncPage[WireDrawdownRequest],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                     },
                     wire_drawdown_request_list_params.WireDrawdownRequestListParams,
                 ),
```

### Comparing `increase-0.5.0/src/increase/resources/wire_transfers.py` & `increase-0.6.0/src/increase/resources/wire_transfers.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         require_approval: bool | NotGiven = NOT_GIVEN,
         routing_number: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> WireTransfer:
         """
         Create a Wire Transfer
 
         Args:
           account_id: The identifier for the account that will send the transfer.
@@ -64,14 +65,16 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return self._post(
             "/wire_transfers",
             body=maybe_transform(
                 {
                     "account_id": account_id,
@@ -88,33 +91,37 @@
                 },
                 wire_transfer_create_params.WireTransferCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=WireTransfer,
         )
 
     def retrieve(
         self,
         wire_transfer_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> WireTransfer:
         """Retrieve a Wire Transfer"""
         return self._get(
             f"/wire_transfers/{wire_transfer_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=WireTransfer,
         )
 
     def list(
         self,
         *,
         account_id: str | NotGiven = NOT_GIVEN,
@@ -123,14 +130,15 @@
         external_account_id: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> SyncPage[WireTransfer]:
         """
         List Wire Transfers
 
         Args:
           account_id: Filter Wire Transfers to those belonging to the specified Account.
 
@@ -142,22 +150,25 @@
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/wire_transfers",
             page=SyncPage[WireTransfer],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                         "account_id": account_id,
                         "external_account_id": external_account_id,
                         "created_at": created_at,
@@ -173,101 +184,109 @@
         wire_transfer_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> WireTransfer:
         """Approve a Wire Transfer"""
         return self._post(
             f"/wire_transfers/{wire_transfer_id}/approve",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=WireTransfer,
         )
 
     def cancel(
         self,
         wire_transfer_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> WireTransfer:
         """Cancel a pending Wire Transfer"""
         return self._post(
             f"/wire_transfers/{wire_transfer_id}/cancel",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=WireTransfer,
         )
 
     def reverse(
         self,
         wire_transfer_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> WireTransfer:
         """
         Simulates the reversal of a [Wire Transfer](#wire-transfers) by the Federal
         Reserve due to error conditions. This will also create a
         [Transaction](#transaction) to account for the returned funds. This Wire
         Transfer must first have a `status` of `complete`.'
         """
         return self._post(
             f"/simulations/wire_transfers/{wire_transfer_id}/reverse",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=WireTransfer,
         )
 
     def submit(
         self,
         wire_transfer_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> WireTransfer:
         """
         Simulates the submission of a [Wire Transfer](#wire-transfers) to the Federal
         Reserve. This transfer must first have a `status` of `pending_approval` or
         `pending_creating`.
         """
         return self._post(
             f"/simulations/wire_transfers/{wire_transfer_id}/submit",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=WireTransfer,
         )
 
 
 class AsyncWireTransfers(AsyncAPIResource):
@@ -286,14 +305,15 @@
         require_approval: bool | NotGiven = NOT_GIVEN,
         routing_number: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> WireTransfer:
         """
         Create a Wire Transfer
 
         Args:
           account_id: The identifier for the account that will send the transfer.
@@ -322,14 +342,16 @@
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
 
+          timeout: Override the client-level default timeout for this request, in seconds
+
           idempotency_key: Specify a custom idempotency key for this request
         """
         return await self._post(
             "/wire_transfers",
             body=maybe_transform(
                 {
                     "account_id": account_id,
@@ -346,33 +368,37 @@
                 },
                 wire_transfer_create_params.WireTransferCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=WireTransfer,
         )
 
     async def retrieve(
         self,
         wire_transfer_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> WireTransfer:
         """Retrieve a Wire Transfer"""
         return await self._get(
             f"/wire_transfers/{wire_transfer_id}",
-            options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
+            options=make_request_options(
+                extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
+            ),
             cast_to=WireTransfer,
         )
 
     def list(
         self,
         *,
         account_id: str | NotGiven = NOT_GIVEN,
@@ -381,14 +407,15 @@
         external_account_id: str | NotGiven = NOT_GIVEN,
         limit: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
     ) -> AsyncPaginator[WireTransfer, AsyncPage[WireTransfer]]:
         """
         List Wire Transfers
 
         Args:
           account_id: Filter Wire Transfers to those belonging to the specified Account.
 
@@ -400,22 +427,25 @@
               objects.
 
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
+
+          timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._get_api_list(
             "/wire_transfers",
             page=AsyncPage[WireTransfer],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 query=maybe_transform(
                     {
                         "cursor": cursor,
                         "limit": limit,
                         "account_id": account_id,
                         "external_account_id": external_account_id,
                         "created_at": created_at,
@@ -431,98 +461,106 @@
         wire_transfer_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> WireTransfer:
         """Approve a Wire Transfer"""
         return await self._post(
             f"/wire_transfers/{wire_transfer_id}/approve",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=WireTransfer,
         )
 
     async def cancel(
         self,
         wire_transfer_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> WireTransfer:
         """Cancel a pending Wire Transfer"""
         return await self._post(
             f"/wire_transfers/{wire_transfer_id}/cancel",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=WireTransfer,
         )
 
     async def reverse(
         self,
         wire_transfer_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> WireTransfer:
         """
         Simulates the reversal of a [Wire Transfer](#wire-transfers) by the Federal
         Reserve due to error conditions. This will also create a
         [Transaction](#transaction) to account for the returned funds. This Wire
         Transfer must first have a `status` of `complete`.'
         """
         return await self._post(
             f"/simulations/wire_transfers/{wire_transfer_id}/reverse",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=WireTransfer,
         )
 
     async def submit(
         self,
         wire_transfer_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
+        timeout: float | None | NotGiven = NOT_GIVEN,
         idempotency_key: str | None = None,
     ) -> WireTransfer:
         """
         Simulates the submission of a [Wire Transfer](#wire-transfers) to the Federal
         Reserve. This transfer must first have a `status` of `pending_approval` or
         `pending_creating`.
         """
         return await self._post(
             f"/simulations/wire_transfers/{wire_transfer_id}/submit",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
+                timeout=timeout,
                 idempotency_key=idempotency_key,
             ),
             cast_to=WireTransfer,
         )
```

### Comparing `increase-0.5.0/src/increase/types/__init__.py` & `increase-0.6.0/src/increase/types/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 
 from .card import Card as Card
 from .file import File as File
 from .event import Event as Event
 from .group import Group as Group
 from .limit import Limit as Limit
 from .entity import Entity as Entity
+from .export import Export as Export
 from .shared import PointOfServiceEntryMode as PointOfServiceEntryMode
 from .account import Account as Account
+from .program import Program as Program
 from .document import Document as Document
 from .transaction import Transaction as Transaction
 from .ach_transfer import ACHTransfer as ACHTransfer
 from .card_details import CardDetails as CardDetails
 from .card_dispute import CardDispute as CardDispute
 from .card_profile import CardProfile as CardProfile
 from .check_deposit import CheckDeposit as CheckDeposit
@@ -23,33 +25,39 @@
 from .routing_number import RoutingNumber as RoutingNumber
 from .account_transfer import AccountTransfer as AccountTransfer
 from .card_list_params import CardListParams as CardListParams
 from .external_account import ExternalAccount as ExternalAccount
 from .file_list_params import FileListParams as FileListParams
 from .oauth_connection import OauthConnection as OauthConnection
 from .account_statement import AccountStatement as AccountStatement
+from .bookkeeping_entry import BookkeepingEntry as BookkeepingEntry
 from .event_list_params import EventListParams as EventListParams
 from .limit_list_params import LimitListParams as LimitListParams
 from .card_create_params import CardCreateParams as CardCreateParams
 from .card_update_params import CardUpdateParams as CardUpdateParams
 from .entity_list_params import EntityListParams as EntityListParams
 from .event_subscription import EventSubscription as EventSubscription
+from .export_list_params import ExportListParams as ExportListParams
 from .file_create_params import FileCreateParams as FileCreateParams
 from .real_time_decision import RealTimeDecision as RealTimeDecision
 from .account_list_params import AccountListParams as AccountListParams
 from .ach_prenotification import ACHPrenotification as ACHPrenotification
+from .bookkeeping_account import BookkeepingAccount as BookkeepingAccount
 from .limit_create_params import LimitCreateParams as LimitCreateParams
 from .limit_update_params import LimitUpdateParams as LimitUpdateParams
 from .pending_transaction import PendingTransaction as PendingTransaction
+from .program_list_params import ProgramListParams as ProgramListParams
 from .declined_transaction import DeclinedTransaction as DeclinedTransaction
 from .digital_wallet_token import DigitalWalletToken as DigitalWalletToken
 from .document_list_params import DocumentListParams as DocumentListParams
 from .entity_create_params import EntityCreateParams as EntityCreateParams
+from .export_create_params import ExportCreateParams as ExportCreateParams
 from .account_create_params import AccountCreateParams as AccountCreateParams
 from .account_update_params import AccountUpdateParams as AccountUpdateParams
+from .bookkeeping_entry_set import BookkeepingEntrySet as BookkeepingEntrySet
 from .wire_drawdown_request import WireDrawdownRequest as WireDrawdownRequest
 from .transaction_list_params import TransactionListParams as TransactionListParams
 from .ach_transfer_list_params import ACHTransferListParams as ACHTransferListParams
 from .card_dispute_list_params import CardDisputeListParams as CardDisputeListParams
 from .card_profile_list_params import CardProfileListParams as CardProfileListParams
 from .check_deposit_list_params import CheckDepositListParams as CheckDepositListParams
 from .wire_transfer_list_params import WireTransferListParams as WireTransferListParams
@@ -73,56 +81,71 @@
 )
 from .check_deposit_create_params import (
     CheckDepositCreateParams as CheckDepositCreateParams,
 )
 from .inbound_ach_transfer_return import (
     InboundACHTransferReturn as InboundACHTransferReturn,
 )
+from .real_time_payments_transfer import (
+    RealTimePaymentsTransfer as RealTimePaymentsTransfer,
+)
 from .wire_transfer_create_params import (
     WireTransferCreateParams as WireTransferCreateParams,
 )
 from .account_number_create_params import (
     AccountNumberCreateParams as AccountNumberCreateParams,
 )
 from .account_number_update_params import (
     AccountNumberUpdateParams as AccountNumberUpdateParams,
 )
 from .account_transfer_list_params import (
     AccountTransferListParams as AccountTransferListParams,
 )
+from .balance_lookup_lookup_params import (
+    BalanceLookupLookupParams as BalanceLookupLookupParams,
+)
 from .check_transfer_create_params import (
     CheckTransferCreateParams as CheckTransferCreateParams,
 )
 from .external_account_list_params import (
     ExternalAccountListParams as ExternalAccountListParams,
 )
 from .oauth_connection_list_params import (
     OauthConnectionListParams as OauthConnectionListParams,
 )
 from .account_statement_list_params import (
     AccountStatementListParams as AccountStatementListParams,
 )
+from .bookkeeping_entry_list_params import (
+    BookkeepingEntryListParams as BookkeepingEntryListParams,
+)
 from .inbound_wire_drawdown_request import (
     InboundWireDrawdownRequest as InboundWireDrawdownRequest,
 )
 from .account_transfer_create_params import (
     AccountTransferCreateParams as AccountTransferCreateParams,
 )
+from .balance_lookup_lookup_response import (
+    BalanceLookupLookupResponse as BalanceLookupLookupResponse,
+)
 from .event_subscription_list_params import (
     EventSubscriptionListParams as EventSubscriptionListParams,
 )
 from .external_account_create_params import (
     ExternalAccountCreateParams as ExternalAccountCreateParams,
 )
 from .external_account_update_params import (
     ExternalAccountUpdateParams as ExternalAccountUpdateParams,
 )
 from .ach_prenotification_list_params import (
     ACHPrenotificationListParams as ACHPrenotificationListParams,
 )
+from .bookkeeping_account_list_params import (
+    BookkeepingAccountListParams as BookkeepingAccountListParams,
+)
 from .pending_transaction_list_params import (
     PendingTransactionListParams as PendingTransactionListParams,
 )
 from .declined_transaction_list_params import (
     DeclinedTransactionListParams as DeclinedTransactionListParams,
 )
 from .digital_wallet_token_list_params import (
@@ -136,22 +159,34 @@
 )
 from .real_time_decision_action_params import (
     RealTimeDecisionActionParams as RealTimeDecisionActionParams,
 )
 from .ach_prenotification_create_params import (
     ACHPrenotificationCreateParams as ACHPrenotificationCreateParams,
 )
+from .bookkeeping_account_create_params import (
+    BookkeepingAccountCreateParams as BookkeepingAccountCreateParams,
+)
 from .wire_drawdown_request_list_params import (
     WireDrawdownRequestListParams as WireDrawdownRequestListParams,
 )
+from .bookkeeping_entry_set_create_params import (
+    BookkeepingEntrySetCreateParams as BookkeepingEntrySetCreateParams,
+)
 from .wire_drawdown_request_create_params import (
     WireDrawdownRequestCreateParams as WireDrawdownRequestCreateParams,
 )
 from .inbound_ach_transfer_return_list_params import (
     InboundACHTransferReturnListParams as InboundACHTransferReturnListParams,
 )
+from .real_time_payments_transfer_list_params import (
+    RealTimePaymentsTransferListParams as RealTimePaymentsTransferListParams,
+)
 from .inbound_ach_transfer_return_create_params import (
     InboundACHTransferReturnCreateParams as InboundACHTransferReturnCreateParams,
 )
 from .inbound_wire_drawdown_request_list_params import (
     InboundWireDrawdownRequestListParams as InboundWireDrawdownRequestListParams,
 )
+from .real_time_payments_transfer_create_params import (
+    RealTimePaymentsTransferCreateParams as RealTimePaymentsTransferCreateParams,
+)
```

### Comparing `increase-0.5.0/src/increase/types/account.py` & `increase-0.6.0/src/increase/types/account.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,38 +2,18 @@
 
 from typing import Optional
 from datetime import date, datetime
 from typing_extensions import Literal
 
 from .._models import BaseModel
 
-__all__ = ["Account", "Balances"]
-
-
-class Balances(BaseModel):
-    available_balance: int
-    """
-    The Account's available balance, representing the current balance less any open
-    Pending Transactions on the Account.
-    """
-
-    current_balance: int
-    """
-    The Account's current balance, representing the sum of all posted Transactions
-    on the Account.
-    """
+__all__ = ["Account"]
 
 
 class Account(BaseModel):
-    balances: Balances
-    """The Account's balances in the minor unit of its currency.
-
-    For dollars, for example, these values will represent cents.
-    """
-
     created_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) time at which the Account
     was created.
     """
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
```

### Comparing `increase-0.5.0/src/increase/types/account_create_params.py` & `increase-0.6.0/src/increase/types/account_create_params.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,7 +15,10 @@
     """The identifier for the Entity that will own the Account."""
 
     informational_entity_id: str
     """
     The identifier of an Entity that, while not owning the Account, is associated
     with its activity. Its relationship to your group must be `informational`.
     """
+
+    program_id: str
+    """The identifier for the Program that this Account falls under."""
```

### Comparing `increase-0.5.0/src/increase/types/account_number.py` & `increase-0.6.0/src/increase/types/account_number.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/account_number_list_params.py` & `increase-0.6.0/src/increase/types/group.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 # File generated from our OpenAPI spec by Stainless.
 
-from __future__ import annotations
+from datetime import datetime
+from typing_extensions import Literal
 
-from typing_extensions import Literal, TypedDict
+from .._models import BaseModel
 
-__all__ = ["AccountNumberListParams"]
+__all__ = ["Group"]
 
 
-class AccountNumberListParams(TypedDict, total=False):
-    account_id: str
-    """Filter Account Numbers to those belonging to the specified Account."""
+class Group(BaseModel):
+    ach_debit_status: Literal["disabled", "enabled"]
+    """If the Group is allowed to create ACH debits."""
 
-    cursor: str
-    """Return the page of entries after this one."""
+    activation_status: Literal["unactivated", "activated"]
+    """If the Group is activated or not."""
 
-    limit: int
-    """Limit the size of the list that is returned.
-
-    The default (and maximum) is 100 objects.
+    created_at: datetime
+    """
+    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) time at which the Group
+    was created.
     """
 
-    status: Literal["active", "disabled", "canceled"]
-    """The status to retrieve Account Numbers for."""
+    id: str
+    """The Group identifier."""
+
+    type: Literal["group"]
+    """A constant representing the object's type.
+
+    For this resource it will always be `group`.
+    """
```

### Comparing `increase-0.5.0/src/increase/types/account_statement.py` & `increase-0.6.0/src/increase/types/account_statement.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/account_statement_list_params.py` & `increase-0.6.0/src/increase/types/account_statement_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/account_transfer.py` & `increase-0.6.0/src/increase/types/account_transfer.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,22 +12,34 @@
 class Approval(BaseModel):
     approved_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
     the transfer was approved.
     """
 
+    approved_by: Optional[str]
+    """
+    If the Transfer was approved by a user in the dashboard, the email address of
+    that user.
+    """
+
 
 class Cancellation(BaseModel):
     canceled_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
     the Transfer was canceled.
     """
 
+    canceled_by: Optional[str]
+    """
+    If the Transfer was canceled by a user in the dashboard, the email address of
+    that user.
+    """
+
 
 class AccountTransfer(BaseModel):
     account_id: str
     """The Account to which the transfer belongs."""
 
     amount: int
     """The transfer amount in the minor unit of the destination account currency.
@@ -70,22 +82,17 @@
 
     id: str
     """The account transfer's identifier."""
 
     network: Literal["account"]
     """The transfer's network."""
 
-    status: Literal[
-        "pending_submission", "pending_approval", "canceled", "requires_attention", "flagged_by_operator", "complete"
-    ]
+    status: Literal["pending_approval", "canceled", "complete"]
     """The lifecycle status of the transfer."""
 
-    template_id: Optional[str]
-    """If the transfer was created from a template, this will be the template's ID."""
-
     transaction_id: Optional[str]
     """The ID for the transaction funding the transfer."""
 
     type: Literal["account_transfer"]
     """A constant representing the object's type.
 
     For this resource it will always be `account_transfer`.
```

### Comparing `increase-0.5.0/src/increase/types/account_transfer_create_params.py` & `increase-0.6.0/src/increase/types/account_transfer_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/account_transfer_list_params.py` & `increase-0.6.0/src/increase/types/account_transfer_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/ach_prenotification.py` & `increase-0.6.0/src/increase/types/ach_prenotification.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/ach_prenotification_create_params.py` & `increase-0.6.0/src/increase/types/ach_prenotification_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/ach_prenotification_list_params.py` & `increase-0.6.0/src/increase/types/ach_prenotification_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/ach_transfer.py` & `increase-0.6.0/src/increase/types/ach_transfer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,49 @@
 # File generated from our OpenAPI spec by Stainless.
 
-from typing import Optional
-from datetime import datetime
+from typing import List, Optional
+from datetime import date, datetime
 from typing_extensions import Literal
 
-from pydantic import Field
+from pydantic import Field as FieldInfo
 
 from .._models import BaseModel
 
-__all__ = ["ACHTransfer", "Approval", "Cancellation", "NotificationOfChange", "Return", "Submission"]
+__all__ = ["ACHTransfer", "Approval", "Cancellation", "NotificationsOfChange", "Return", "Submission"]
 
 
 class Approval(BaseModel):
     approved_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
     the transfer was approved.
     """
 
+    approved_by: Optional[str]
+    """
+    If the Transfer was approved by a user in the dashboard, the email address of
+    that user.
+    """
+
 
 class Cancellation(BaseModel):
     canceled_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
     the Transfer was canceled.
     """
 
+    canceled_by: Optional[str]
+    """
+    If the Transfer was canceled by a user in the dashboard, the email address of
+    that user.
+    """
+
 
-class NotificationOfChange(BaseModel):
+class NotificationsOfChange(BaseModel):
     change_code: str
     """The type of change that occurred."""
 
     corrected_data: str
     """The corrected data."""
 
     created_at: datetime
@@ -140,14 +152,20 @@
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transfer's
     currency. For ACH transfers this is always equal to `usd`.
     """
 
+    effective_date: Optional[date]
+    """
+    The transfer effective date in
+    [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) format.
+    """
+
     external_account_id: Optional[str]
     """The identifier of the External Account the transfer was made to, if any."""
 
     funding: Literal["checking", "savings"]
     """The type of the account to which the transfer will be sent."""
 
     id: str
@@ -161,48 +179,52 @@
 
     This value is information and not verified by the recipient's bank.
     """
 
     network: Literal["ach"]
     """The transfer's network."""
 
-    notification_of_change: Optional[NotificationOfChange]
+    notifications_of_change: List[NotificationsOfChange]
     """
     If the receiving bank accepts the transfer but notifies that future transfers
     should use different details, this will contain those details.
     """
 
-    return_: Optional[Return] = Field(alias="return")
+    return_: Optional[Return] = FieldInfo(alias="return")
     """If your transfer is returned, this will contain details of the return."""
 
     routing_number: str
     """The American Bankers' Association (ABA) Routing Transit Number (RTN)."""
 
     standard_entry_class_code: Literal[
         "corporate_credit_or_debit", "prearranged_payments_and_deposit", "internet_initiated"
     ]
     """The Standard Entry Class (SEC) code to use for the transfer."""
 
     statement_descriptor: str
     """The descriptor that will show on the recipient's bank statement."""
 
     status: Literal[
-        "pending_approval", "canceled", "pending_submission", "submitted", "returned", "requires_attention", "rejected"
+        "pending_approval",
+        "canceled",
+        "pending_reviewing",
+        "pending_submission",
+        "submitted",
+        "returned",
+        "requires_attention",
+        "rejected",
     ]
     """The lifecycle status of the transfer."""
 
     submission: Optional[Submission]
     """
     After the transfer is submitted to FedACH, this will contain supplemental
     details.
     """
 
-    template_id: Optional[str]
-    """If the transfer was created from a template, this will be the template's ID."""
-
     transaction_id: Optional[str]
     """The ID for the transaction funding the transfer."""
 
     type: Literal["ach_transfer"]
     """A constant representing the object's type.
 
     For this resource it will always be `ach_transfer`.
```

### Comparing `increase-0.5.0/src/increase/types/ach_transfer_create_params.py` & `increase-0.6.0/src/increase/types/ach_transfer_create_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     addendum: str
     """Additional information that will be sent to the recipient.
 
     This is included in the transfer data sent to the receiving bank.
     """
 
     company_descriptive_date: str
-    """The description of the date of the transfer, usually in the format `YYYYMMDD`.
+    """The description of the date of the transfer, usually in the format `YYMMDD`.
 
     This is included in the transfer data sent to the receiving bank.
     """
 
     company_discretionary_data: str
     """The data you choose to associate with the transfer.
```

### Comparing `increase-0.5.0/src/increase/types/ach_transfer_list_params.py` & `increase-0.6.0/src/increase/types/ach_transfer_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/card.py` & `increase-0.6.0/src/increase/types/card.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/card_create_params.py` & `increase-0.6.0/src/increase/types/card_update_params.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing_extensions import Required, TypedDict
+from typing_extensions import Literal, Required, TypedDict
 
-__all__ = ["CardCreateParams", "BillingAddress", "DigitalWallet"]
+__all__ = ["CardUpdateParams", "BillingAddress", "DigitalWallet"]
 
 
 class BillingAddress(TypedDict, total=False):
     city: Required[str]
     """The city of the billing address."""
 
     line1: Required[str]
@@ -40,23 +40,23 @@
     phone: str
     """
     A phone number that can be used to verify the cardholder via one-time passcode
     over SMS.
     """
 
 
-class CardCreateParams(TypedDict, total=False):
-    account_id: Required[str]
-    """The Account the card should belong to."""
-
+class CardUpdateParams(TypedDict, total=False):
     billing_address: BillingAddress
-    """The card's billing address."""
+    """The card's updated billing address."""
 
     description: str
     """The description you choose to give the card."""
 
     digital_wallet: DigitalWallet
     """
     The contact information used in the two-factor steps for digital wallet card
     creation. At least one field must be present to complete the digital wallet
     steps.
     """
+
+    status: Literal["active", "disabled", "canceled"]
+    """The status to update the Card with."""
```

### Comparing `increase-0.5.0/src/increase/types/card_details.py` & `increase-0.6.0/src/increase/types/card_details.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/card_dispute.py` & `increase-0.6.0/src/increase/types/card_dispute.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
     the Card Dispute was accepted.
     """
 
     card_dispute_id: str
     """The identifier of the Card Dispute that was accepted."""
 
-    transaction_id: Optional[str]
+    transaction_id: str
     """
     The identifier of the Transaction that was created to return the disputed funds
     to your account.
     """
 
 
 class Rejection(BaseModel):
```

### Comparing `increase-0.5.0/src/increase/types/card_dispute_list_params.py` & `increase-0.6.0/src/increase/types/card_dispute_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/card_list_params.py` & `increase-0.6.0/src/increase/types/card_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/card_profile.py` & `increase-0.6.0/src/increase/types/card_profile.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/card_profile_create_params.py` & `increase-0.6.0/src/increase/types/card_profile_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/card_profile_list_params.py` & `increase-0.6.0/src/increase/types/card_profile_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/check_deposit.py` & `increase-0.6.0/src/increase/types/check_deposit.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
     reason: Literal[
         "incomplete_image",
         "duplicate",
         "poor_image_quality",
         "incorrect_amount",
         "incorrect_recipient",
         "not_eligible_for_mobile_deposit",
+        "missing_required_data_elements",
         "unknown",
     ]
     """Why the check deposit was rejected."""
 
     rejected_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
```

### Comparing `increase-0.5.0/src/increase/types/check_deposit_create_params.py` & `increase-0.6.0/src/increase/types/check_deposit_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/check_deposit_list_params.py` & `increase-0.6.0/src/increase/types/check_deposit_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/check_transfer_create_params.py` & `increase-0.6.0/src/increase/types/check_transfer_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/check_transfer_list_params.py` & `increase-0.6.0/src/increase/types/check_transfer_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/declined_transaction.py` & `increase-0.6.0/src/increase/types/declined_transaction.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     "SourceCardDecline",
     "SourceCardDeclineNetworkDetails",
     "SourceCardDeclineNetworkDetailsVisa",
     "SourceCheckDecline",
     "SourceInboundRealTimePaymentsTransferDecline",
     "SourceInternationalACHDecline",
     "SourceCardRouteDecline",
+    "SourceWireDecline",
 ]
 
 
 class SourceACHDecline(BaseModel):
     amount: int
     """The declined amount in the minor unit of the destination account currency.
 
@@ -39,19 +40,20 @@
     reason: Literal[
         "ach_route_canceled",
         "ach_route_disabled",
         "breaches_limit",
         "credit_entry_refused_by_receiver",
         "duplicate_return",
         "entity_not_active",
-        "transaction_not_allowed",
         "group_locked",
         "insufficient_funds",
+        "misrouted_return",
         "no_ach_route",
         "originator_request",
+        "transaction_not_allowed",
     ]
     """Why the ACH transfer was declined."""
 
     receiver_id_number: Optional[str]
 
     receiver_name: Optional[str]
 
@@ -147,18 +149,21 @@
     reason: Literal[
         "card_not_active",
         "entity_not_active",
         "group_locked",
         "insufficient_funds",
         "cvv2_mismatch",
         "transaction_not_allowed",
+        "breaches_internal_limit",
         "breaches_limit",
         "webhook_declined",
         "webhook_timed_out",
         "declined_by_stand_in_processing",
+        "invalid_physical_card",
+        "missing_original_authorization",
     ]
     """Why the transaction was declined."""
 
 
 class SourceCheckDecline(BaseModel):
     amount: int
     """The declined amount in the minor unit of the destination account currency.
@@ -176,14 +181,17 @@
         "group_locked",
         "insufficient_funds",
         "unable_to_locate_account",
         "unable_to_process",
         "refer_to_image",
         "stop_payment_requested",
         "returned",
+        "duplicate_presentment",
+        "not_authorized",
+        "altered_or_fictitious",
     ]
     """Why the check was declined."""
 
 
 class SourceInboundRealTimePaymentsTransferDecline(BaseModel):
     amount: int
     """The declined amount in the minor unit of the destination account currency.
@@ -209,14 +217,15 @@
 
     debtor_routing_number: str
     """The routing number of the account that sent the transfer."""
 
     reason: Literal[
         "account_number_canceled",
         "account_number_disabled",
+        "account_restricted",
         "group_locked",
         "entity_not_active",
         "real_time_payments_not_enabled",
     ]
     """Why the transfer was declined."""
 
     remittance_information: Optional[str]
@@ -326,14 +335,62 @@
     merchant_country: str
 
     merchant_descriptor: str
 
     merchant_state: Optional[str]
 
 
+class SourceWireDecline(BaseModel):
+    amount: int
+    """The declined amount in the minor unit of the destination account currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    beneficiary_address_line1: Optional[str]
+
+    beneficiary_address_line2: Optional[str]
+
+    beneficiary_address_line3: Optional[str]
+
+    beneficiary_name: Optional[str]
+
+    beneficiary_reference: Optional[str]
+
+    description: str
+
+    input_message_accountability_data: Optional[str]
+
+    originator_address_line1: Optional[str]
+
+    originator_address_line2: Optional[str]
+
+    originator_address_line3: Optional[str]
+
+    originator_name: Optional[str]
+
+    originator_to_beneficiary_information_line1: Optional[str]
+
+    originator_to_beneficiary_information_line2: Optional[str]
+
+    originator_to_beneficiary_information_line3: Optional[str]
+
+    originator_to_beneficiary_information_line4: Optional[str]
+
+    reason: Literal[
+        "account_number_canceled",
+        "account_number_disabled",
+        "entity_not_active",
+        "group_locked",
+        "no_account_number",
+        "transaction_not_allowed",
+    ]
+    """Why the wire transfer was declined."""
+
+
 class Source(BaseModel):
     ach_decline: Optional[SourceACHDecline]
     """A ACH Decline object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `ach_decline`.
     """
@@ -355,14 +412,15 @@
     category: Literal[
         "ach_decline",
         "card_decline",
         "check_decline",
         "inbound_real_time_payments_transfer_decline",
         "international_ach_decline",
         "card_route_decline",
+        "wire_decline",
         "other",
     ]
     """The type of decline that took place.
 
     We may add additional possible values for this enum over time; your application
     should be able to handle such additions gracefully.
     """
@@ -384,14 +442,21 @@
     international_ach_decline: Optional[SourceInternationalACHDecline]
     """A International ACH Decline object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `international_ach_decline`.
     """
 
+    wire_decline: Optional[SourceWireDecline]
+    """A Wire Decline object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `wire_decline`.
+    """
+
 
 class DeclinedTransaction(BaseModel):
     account_id: str
     """The identifier for the Account the Declined Transaction belongs to."""
 
     amount: int
     """The Declined Transaction amount in the minor unit of its currency.
@@ -420,15 +485,15 @@
 
     route_id: Optional[str]
     """The identifier for the route this Declined Transaction came through.
 
     Routes are things like cards and ACH details.
     """
 
-    route_type: Optional[str]
+    route_type: Optional[Literal["account_number", "card"]]
     """The type of the route this Declined Transaction came through."""
 
     source: Source
     """
     This is an object giving more details on the network-level event that caused the
     Declined Transaction. For example, for a card transaction this lists the
     merchant's industry and location. Note that for backwards compatibility reasons,
```

### Comparing `increase-0.5.0/src/increase/types/declined_transaction_list_params.py` & `increase-0.6.0/src/increase/types/declined_transaction_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/digital_wallet_token.py` & `increase-0.6.0/src/increase/types/digital_wallet_token.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/digital_wallet_token_list_params.py` & `increase-0.6.0/src/increase/types/digital_wallet_token_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/document.py` & `increase-0.6.0/src/increase/types/program.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 # File generated from our OpenAPI spec by Stainless.
 
-from typing import Optional
 from datetime import datetime
 from typing_extensions import Literal
 
 from .._models import BaseModel
 
-__all__ = ["Document"]
+__all__ = ["Program"]
 
 
-class Document(BaseModel):
-    category: Literal["form_1099_int"]
-    """The type of document."""
-
+class Program(BaseModel):
     created_at: datetime
     """
-    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) time at which the
-    Document was created.
+    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) time at which the Program
+    was created.
     """
 
-    entity_id: Optional[str]
-    """The identifier of the Entity the document was generated for."""
-
-    file_id: str
-    """The identifier of the File containing the Document's contents."""
-
     id: str
-    """The Document identifier."""
+    """The Program identifier."""
+
+    name: str
+    """The name of the Program."""
 
-    type: Literal["document"]
+    type: Literal["program"]
     """A constant representing the object's type.
 
-    For this resource it will always be `document`.
+    For this resource it will always be `program`.
+    """
+
+    updated_at: datetime
+    """
+    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) time at which the Program
+    was last updated.
     """
```

### Comparing `increase-0.5.0/src/increase/types/document_list_params.py` & `increase-0.6.0/src/increase/types/account_list_params.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,18 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing import List, Union
+from typing import Union
 from datetime import datetime
 from typing_extensions import Literal, Annotated, TypedDict
 
 from .._utils import PropertyInfo
 
-__all__ = ["DocumentListParams", "Category", "CreatedAt"]
-
-_CategoryReservedKeywords = TypedDict(
-    "_CategoryReservedKeywords",
-    {
-        "in": List[Literal["form_1099_int"]],
-    },
-    total=False,
-)
-
-
-class Category(_CategoryReservedKeywords, total=False):
-    pass
+__all__ = ["AccountListParams", "CreatedAt"]
 
 
 class CreatedAt(TypedDict, total=False):
     after: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results after this [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601)
     timestamp.
@@ -45,23 +33,24 @@
     on_or_before: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """
     Return results on or before this
     [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) timestamp.
     """
 
 
-class DocumentListParams(TypedDict, total=False):
-    category: Category
-
+class AccountListParams(TypedDict, total=False):
     created_at: CreatedAt
 
     cursor: str
     """Return the page of entries after this one."""
 
     entity_id: str
-    """Filter Documents to ones belonging to the specified Entity."""
+    """Filter Accounts for those belonging to the specified Entity."""
 
     limit: int
     """Limit the size of the list that is returned.
 
     The default (and maximum) is 100 objects.
     """
+
+    status: Literal["open", "closed"]
+    """Filter Accounts for those with the specified status."""
```

### Comparing `increase-0.5.0/src/increase/types/entity.py` & `increase-0.6.0/src/increase/types/entity.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/entity_create_params.py` & `increase-0.6.0/src/increase/types/entity_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/event.py` & `increase-0.6.0/src/increase/types/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,16 @@
         "account_transfer.updated",
         "ach_prenotification.created",
         "ach_prenotification.updated",
         "ach_transfer.created",
         "ach_transfer.updated",
         "card.created",
         "card.updated",
+        "card_payment.created",
+        "card_payment.updated",
         "card_dispute.created",
         "card_dispute.updated",
         "check_deposit.created",
         "check_deposit.updated",
         "check_transfer.created",
         "check_transfer.updated",
         "declined_transaction.created",
```

### Comparing `increase-0.5.0/src/increase/types/event_list_params.py` & `increase-0.6.0/src/increase/types/event_list_params.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,14 +51,16 @@
                 "account_transfer.updated",
                 "ach_prenotification.created",
                 "ach_prenotification.updated",
                 "ach_transfer.created",
                 "ach_transfer.updated",
                 "card.created",
                 "card.updated",
+                "card_payment.created",
+                "card_payment.updated",
                 "card_dispute.created",
                 "card_dispute.updated",
                 "check_deposit.created",
                 "check_deposit.updated",
                 "check_transfer.created",
                 "check_transfer.updated",
                 "declined_transaction.created",
```

### Comparing `increase-0.5.0/src/increase/types/event_subscription.py` & `increase-0.6.0/src/increase/types/event_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,16 @@
             "account_transfer.updated",
             "ach_prenotification.created",
             "ach_prenotification.updated",
             "ach_transfer.created",
             "ach_transfer.updated",
             "card.created",
             "card.updated",
+            "card_payment.created",
+            "card_payment.updated",
             "card_dispute.created",
             "card_dispute.updated",
             "check_deposit.created",
             "check_deposit.updated",
             "check_transfer.created",
             "check_transfer.updated",
             "declined_transaction.created",
```

### Comparing `increase-0.5.0/src/increase/types/event_subscription_create_params.py` & `increase-0.6.0/src/increase/types/event_subscription_create_params.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,16 @@
         "account_transfer.updated",
         "ach_prenotification.created",
         "ach_prenotification.updated",
         "ach_transfer.created",
         "ach_transfer.updated",
         "card.created",
         "card.updated",
+        "card_payment.created",
+        "card_payment.updated",
         "card_dispute.created",
         "card_dispute.updated",
         "check_deposit.created",
         "check_deposit.updated",
         "check_transfer.created",
         "check_transfer.updated",
         "declined_transaction.created",
```

### Comparing `increase-0.5.0/src/increase/types/external_account.py` & `increase-0.6.0/src/increase/types/external_account.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/external_account_create_params.py` & `increase-0.6.0/src/increase/types/external_account_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/external_account_list_params.py` & `increase-0.6.0/src/increase/types/external_account_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/file.py` & `increase-0.6.0/src/increase/types/file.py`

 * *Files 18% similar despite different names*

```diff
@@ -38,15 +38,17 @@
         "form_ss_4",
         "identity_document",
         "increase_statement",
         "other",
         "trust_formation_document",
         "digital_wallet_artwork",
         "digital_wallet_app_icon",
+        "document_request",
         "entity_supplemental_document",
+        "export",
     ]
     """What the File will be used for.
 
     We may add additional possible values for this enum over time; your application
     should be able to handle such additions gracefully.
     """
```

### Comparing `increase-0.5.0/src/increase/types/file_create_params.py` & `increase-0.6.0/src/increase/types/file_create_params.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,14 +24,15 @@
             "check_image_back",
             "form_ss_4",
             "identity_document",
             "other",
             "trust_formation_document",
             "digital_wallet_artwork",
             "digital_wallet_app_icon",
+            "document_request",
             "entity_supplemental_document",
         ]
     ]
     """What the File will be used for in Increase's systems."""
 
     description: str
     """The description you choose to give the File."""
```

### Comparing `increase-0.5.0/src/increase/types/file_list_params.py` & `increase-0.6.0/src/increase/types/file_list_params.py`

 * *Files 9% similar despite different names*

```diff
@@ -48,15 +48,17 @@
                 "form_ss_4",
                 "identity_document",
                 "increase_statement",
                 "other",
                 "trust_formation_document",
                 "digital_wallet_artwork",
                 "digital_wallet_app_icon",
+                "document_request",
                 "entity_supplemental_document",
+                "export",
             ]
         ],
     },
     total=False,
 )
```

### Comparing `increase-0.5.0/src/increase/types/inbound_ach_transfer_return.py` & `increase-0.6.0/src/increase/types/inbound_ach_transfer_return.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/inbound_ach_transfer_return_create_params.py` & `increase-0.6.0/src/increase/types/inbound_ach_transfer_return_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/inbound_wire_drawdown_request.py` & `increase-0.6.0/src/increase/types/inbound_wire_drawdown_request.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/limit.py` & `increase-0.6.0/src/increase/types/limit.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/limit_create_params.py` & `increase-0.6.0/src/increase/types/limit_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/limit_list_params.py` & `increase-0.6.0/src/increase/types/limit_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/oauth_connection.py` & `increase-0.6.0/src/increase/types/oauth_connection.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/pending_transaction.py` & `increase-0.6.0/src/increase/types/pending_transaction.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     "SourceCardAuthorization",
     "SourceCardAuthorizationNetworkDetails",
     "SourceCardAuthorizationNetworkDetailsVisa",
     "SourceCheckDepositInstruction",
     "SourceCheckTransferInstruction",
     "SourceInboundFundsHold",
     "SourceCardRouteAuthorization",
+    "SourceRealTimePaymentsTransferInstruction",
     "SourceWireDrawdownPaymentInstruction",
     "SourceWireTransferInstruction",
 ]
 
 
 class SourceAccountTransferInstruction(BaseModel):
     amount: int
@@ -98,14 +99,23 @@
 
     digital_wallet_token_id: Optional[str]
     """
     If the authorization was made via a Digital Wallet Token (such as an Apple Pay
     purchase), the identifier of the token that was used.
     """
 
+    expires_at: datetime
+    """
+    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) when this authorization
+    will expire and the pending transaction will be released.
+    """
+
+    id: str
+    """The Card Authorization identifier."""
+
     merchant_acceptor_id: str
     """
     The merchant identifier (commonly abbreviated as MID) of the merchant the card
     is transacting with.
     """
 
     merchant_category_code: Optional[str]
@@ -125,20 +135,29 @@
 
     network: Literal["visa"]
     """The payment network used to process this card authorization"""
 
     network_details: SourceCardAuthorizationNetworkDetails
     """Fields specific to the `network`"""
 
+    pending_transaction_id: Optional[str]
+    """The identifier of the Pending Transaction associated with this Transaction."""
+
     real_time_decision_id: Optional[str]
     """
     The identifier of the Real-Time Decision sent to approve or decline this
     transaction.
     """
 
+    type: Literal["card_authorization"]
+    """A constant representing the object's type.
+
+    For this resource it will always be `card_authorization`.
+    """
+
 
 class SourceCheckDepositInstruction(BaseModel):
     amount: int
     """The pending amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
     """
@@ -191,23 +210,32 @@
 
     automatically_releases_at: datetime
     """When the hold will be released automatically.
 
     Certain conditions may cause it to be released before this time.
     """
 
+    created_at: datetime
+    """
+    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) time at which the hold
+    was created.
+    """
+
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the hold's
     currency.
     """
 
     held_transaction_id: Optional[str]
     """The ID of the Transaction for which funds were held."""
 
+    pending_transaction_id: Optional[str]
+    """The ID of the Pending Transaction representing the held funds."""
+
     released_at: Optional[datetime]
     """When the hold was released (if it has been released)."""
 
     status: Literal["held", "complete"]
     """The status of the hold."""
 
 
@@ -233,14 +261,28 @@
     merchant_country: str
 
     merchant_descriptor: str
 
     merchant_state: Optional[str]
 
 
+class SourceRealTimePaymentsTransferInstruction(BaseModel):
+    amount: int
+    """The pending amount in the minor unit of the transaction's currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    transfer_id: str
+    """
+    The identifier of the Real Time Payments Transfer that led to this Pending
+    Transaction.
+    """
+
+
 class SourceWireDrawdownPaymentInstruction(BaseModel):
     account_number: str
 
     amount: int
     """The pending amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
@@ -332,14 +374,21 @@
     inbound_funds_hold: Optional[SourceInboundFundsHold]
     """A Inbound Funds Hold object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `inbound_funds_hold`.
     """
 
+    real_time_payments_transfer_instruction: Optional[SourceRealTimePaymentsTransferInstruction]
+    """A Real Time Payments Transfer Instruction object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `real_time_payments_transfer_instruction`.
+    """
+
     wire_drawdown_payment_instruction: Optional[SourceWireDrawdownPaymentInstruction]
     """A Wire Drawdown Payment Instruction object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `wire_drawdown_payment_instruction`.
     """
 
@@ -357,14 +406,20 @@
 
     amount: int
     """The Pending Transaction amount in the minor unit of its currency.
 
     For dollars, for example, this is cents.
     """
 
+    completed_at: Optional[datetime]
+    """
+    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date on which the Pending
+    Transaction was completed.
+    """
+
     created_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date on which the Pending
     Transaction occured.
     """
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
@@ -386,15 +441,15 @@
 
     route_id: Optional[str]
     """The identifier for the route this Pending Transaction came through.
 
     Routes are things like cards and ACH details.
     """
 
-    route_type: Optional[str]
+    route_type: Optional[Literal["account_number", "card"]]
     """The type of the route this Pending Transaction came through."""
 
     source: Source
     """
     This is an object giving more details on the network-level event that caused the
     Pending Transaction. For example, for a card transaction this lists the
     merchant's industry and location.
```

### Comparing `increase-0.5.0/src/increase/types/real_time_decision.py` & `increase-0.6.0/src/increase/types/real_time_decision.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/real_time_decision_action_params.py` & `increase-0.6.0/src/increase/types/real_time_decision_action_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/routing_number.py` & `increase-0.6.0/src/increase/types/routing_number.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/routing_number_list_params.py` & `increase-0.6.0/src/increase/types/routing_number_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/shared/point_of_service_entry_mode.py` & `increase-0.6.0/src/increase/types/shared_params/point_of_service_entry_mode.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/simulations/__init__.py` & `increase-0.6.0/src/increase/types/simulations/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,32 +10,44 @@
 from .card_refund_create_params import CardRefundCreateParams as CardRefundCreateParams
 from .ach_transfer_return_params import (
     ACHTransferReturnParams as ACHTransferReturnParams,
 )
 from .card_dispute_action_params import (
     CardDisputeActionParams as CardDisputeActionParams,
 )
+from .check_transfer_return_params import (
+    CheckTransferReturnParams as CheckTransferReturnParams,
+)
 from .card_authorization_simulation import (
     CardAuthorizationSimulation as CardAuthorizationSimulation,
 )
+from .interest_payment_create_params import (
+    InterestPaymentCreateParams as InterestPaymentCreateParams,
+)
 from .account_statement_create_params import (
     AccountStatementCreateParams as AccountStatementCreateParams,
 )
 from .ach_transfer_create_inbound_params import (
     ACHTransferCreateInboundParams as ACHTransferCreateInboundParams,
 )
+from .interest_payment_simulation_result import (
+    InterestPaymentSimulationResult as InterestPaymentSimulationResult,
+)
 from .wire_transfer_create_inbound_params import (
     WireTransferCreateInboundParams as WireTransferCreateInboundParams,
 )
 from .digital_wallet_token_request_create_params import (
     DigitalWalletTokenRequestCreateParams as DigitalWalletTokenRequestCreateParams,
 )
 from .inbound_wire_drawdown_request_create_params import (
     InboundWireDrawdownRequestCreateParams as InboundWireDrawdownRequestCreateParams,
 )
+from .real_time_payments_transfer_complete_params import (
+    RealTimePaymentsTransferCompleteParams as RealTimePaymentsTransferCompleteParams,
+)
 from .digital_wallet_token_request_create_response import (
     DigitalWalletTokenRequestCreateResponse as DigitalWalletTokenRequestCreateResponse,
 )
 from .real_time_payments_transfer_create_inbound_params import (
     RealTimePaymentsTransferCreateInboundParams as RealTimePaymentsTransferCreateInboundParams,
 )
 from .inbound_real_time_payments_transfer_simulation_result import (
```

### Comparing `increase-0.5.0/src/increase/types/simulations/ach_transfer_create_inbound_params.py` & `increase-0.6.0/src/increase/types/simulations/ach_transfer_create_inbound_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/simulations/ach_transfer_return_params.py` & `increase-0.6.0/src/increase/types/simulations/ach_transfer_return_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/simulations/ach_transfer_simulation.py` & `increase-0.6.0/src/increase/types/simulations/ach_transfer_simulation.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,34 +16,37 @@
     "TransactionSourceACHCheckConversion",
     "TransactionSourceACHTransferIntention",
     "TransactionSourceACHTransferRejection",
     "TransactionSourceACHTransferReturn",
     "TransactionSourceCardDisputeAcceptance",
     "TransactionSourceCardRefund",
     "TransactionSourceCardSettlement",
+    "TransactionSourceCardRevenuePayment",
     "TransactionSourceCheckDepositAcceptance",
     "TransactionSourceCheckDepositReturn",
     "TransactionSourceCheckTransferIntention",
     "TransactionSourceCheckTransferReturn",
     "TransactionSourceCheckTransferRejection",
     "TransactionSourceCheckTransferStopPaymentRequest",
     "TransactionSourceDisputeResolution",
     "TransactionSourceEmpyrealCashDeposit",
+    "TransactionSourceFeePayment",
     "TransactionSourceInboundACHTransfer",
     "TransactionSourceInboundCheck",
     "TransactionSourceInboundInternationalACHTransfer",
     "TransactionSourceInboundRealTimePaymentsTransferConfirmation",
     "TransactionSourceInboundWireDrawdownPaymentReversal",
     "TransactionSourceInboundWireDrawdownPayment",
     "TransactionSourceInboundWireReversal",
     "TransactionSourceInboundWireTransfer",
     "TransactionSourceInterestPayment",
     "TransactionSourceInternalSource",
     "TransactionSourceCardRouteRefund",
     "TransactionSourceCardRouteSettlement",
+    "TransactionSourceRealTimePaymentsTransferAcknowledgement",
     "TransactionSourceSampleFunds",
     "TransactionSourceWireDrawdownPaymentIntention",
     "TransactionSourceWireDrawdownPaymentRejection",
     "TransactionSourceWireTransferIntention",
     "TransactionSourceWireTransferRejection",
     "DeclinedTransaction",
     "DeclinedTransactionSource",
@@ -51,14 +54,15 @@
     "DeclinedTransactionSourceCardDecline",
     "DeclinedTransactionSourceCardDeclineNetworkDetails",
     "DeclinedTransactionSourceCardDeclineNetworkDetailsVisa",
     "DeclinedTransactionSourceCheckDecline",
     "DeclinedTransactionSourceInboundRealTimePaymentsTransferDecline",
     "DeclinedTransactionSourceInternationalACHDecline",
     "DeclinedTransactionSourceCardRouteDecline",
+    "DeclinedTransactionSourceWireDecline",
 ]
 
 
 class TransactionSourceAccountTransferIntention(BaseModel):
     amount: int
     """The pending amount in the minor unit of the transaction's currency.
 
@@ -175,66 +179,107 @@
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
     the Card Dispute was accepted.
     """
 
     card_dispute_id: str
     """The identifier of the Card Dispute that was accepted."""
 
-    transaction_id: Optional[str]
+    transaction_id: str
     """
     The identifier of the Transaction that was created to return the disputed funds
     to your account.
     """
 
 
 class TransactionSourceCardRefund(BaseModel):
     amount: int
     """The pending amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
     """
 
-    card_settlement_transaction_id: Optional[str]
-    """The identifier for the Transaction this refunds, if any."""
-
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
     transaction's currency.
     """
 
+    id: str
+    """The Card Refund identifier."""
+
+    merchant_acceptor_id: Optional[str]
+    """
+    The merchant identifier (commonly abbreviated as MID) of the merchant the card
+    is transacting with.
+    """
+
+    merchant_category_code: str
+    """The 4-digit MCC describing the merchant's business."""
+
+    merchant_city: Optional[str]
+    """The city the merchant resides in."""
+
+    merchant_country: str
+    """The country the merchant resides in."""
+
+    merchant_name: Optional[str]
+    """The name of the merchant."""
+
+    merchant_state: Optional[str]
+    """The state the merchant resides in."""
+
     type: Literal["card_refund"]
     """A constant representing the object's type.
 
     For this resource it will always be `card_refund`.
     """
 
 
 class TransactionSourceCardSettlement(BaseModel):
     amount: int
     """The amount in the minor unit of the transaction's settlement currency.
 
     For dollars, for example, this is cents.
     """
 
+    card_authorization: Optional[str]
+    """
+    The Card Authorization that was created prior to this Card Settlement, if on
+    exists.
+    """
+
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
     transaction's settlement currency.
     """
 
+    id: str
+    """The Card Settlement identifier."""
+
+    merchant_acceptor_id: Optional[str]
+    """
+    The merchant identifier (commonly abbreviated as MID) of the merchant the card
+    is transacting with.
+    """
+
     merchant_category_code: str
+    """The 4-digit MCC describing the merchant's business."""
 
     merchant_city: Optional[str]
+    """The city the merchant resides in."""
 
     merchant_country: str
+    """The country the merchant resides in."""
 
     merchant_name: Optional[str]
+    """The name of the merchant."""
 
     merchant_state: Optional[str]
+    """The state the merchant resides in."""
 
     pending_transaction_id: Optional[str]
     """The identifier of the Pending Transaction associated with this Transaction."""
 
     presentment_amount: int
     """The amount in the minor unit of the transaction's presentment currency."""
 
@@ -247,14 +292,37 @@
     type: Literal["card_settlement"]
     """A constant representing the object's type.
 
     For this resource it will always be `card_settlement`.
     """
 
 
+class TransactionSourceCardRevenuePayment(BaseModel):
+    amount: int
+    """The amount in the minor unit of the transaction's currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
+    """
+    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transaction
+    currency.
+    """
+
+    period_end: datetime
+    """The end of the period for which this transaction paid interest."""
+
+    period_start: datetime
+    """The start of the period for which this transaction paid interest."""
+
+    transacted_on_account_id: Optional[str]
+    """The account the card belonged to."""
+
+
 class TransactionSourceCheckDepositAcceptance(BaseModel):
     account_number: str
     """The account number printed on the check."""
 
     amount: int
     """The amount to be deposited in the minor unit of the transaction's currency.
 
@@ -362,14 +430,29 @@
     """The identifier of the Check Transfer with which this is associated."""
 
 
 class TransactionSourceCheckTransferReturn(BaseModel):
     file_id: Optional[str]
     """If available, a document with additional information about the return."""
 
+    reason: Literal["mail_delivery_failure", "refused_by_recipient", "returned_not_authorized"]
+    """The reason why the check was returned."""
+
+    returned_at: datetime
+    """
+    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
+    the check was returned.
+    """
+
+    transaction_id: Optional[str]
+    """
+    The identifier of the Transaction that was created to credit you for the
+    returned check.
+    """
+
     transfer_id: str
     """The identifier of the returned Check Transfer."""
 
 
 class TransactionSourceCheckTransferRejection(BaseModel):
     transfer_id: str
     """The identifier of the Check Transfer that led to this Transaction."""
@@ -417,14 +500,28 @@
     """
 
     bag_id: str
 
     deposit_date: datetime
 
 
+class TransactionSourceFeePayment(BaseModel):
+    amount: int
+    """The amount in the minor unit of the transaction's currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
+    """
+    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transaction
+    currency.
+    """
+
+
 class TransactionSourceInboundACHTransfer(BaseModel):
     amount: int
     """The amount in the minor unit of the destination account currency.
 
     For dollars, for example, this is cents.
     """
 
@@ -639,14 +736,20 @@
     originator_to_beneficiary_information: Optional[str]
 
 
 class TransactionSourceInboundWireReversal(BaseModel):
     amount: int
     """The amount that was reversed."""
 
+    created_at: datetime
+    """
+    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
+    the reversal was created.
+    """
+
     description: str
     """The description on the reversal message from Fedwire."""
 
     financial_institution_to_financial_institution_information: Optional[str]
     """Additional financial institution information included in the wire reversal."""
 
     input_cycle_date: date
@@ -675,14 +778,20 @@
 
     receiver_financial_institution_information: Optional[str]
     """
     Information included in the wire reversal for the receiving financial
     institution.
     """
 
+    transaction_id: Optional[str]
+    """The ID for the Transaction associated with the transfer reversal."""
+
+    wire_transfer_id: str
+    """The ID for the Wire Transfer that is being reversed."""
+
 
 class TransactionSourceInboundWireTransfer(BaseModel):
     amount: int
     """The amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
     """
@@ -755,19 +864,21 @@
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transaction
     currency.
     """
 
     reason: Literal[
         "bank_migration",
         "cashback",
+        "collection_receivable",
         "empyreal_adjustment",
         "error",
         "error_correction",
         "fees",
         "interest",
+        "negative_balance_forgiveness",
         "sample_funds",
         "sample_funds_return",
     ]
 
 
 class TransactionSourceCardRouteRefund(BaseModel):
     amount: int
@@ -817,14 +928,31 @@
     merchant_country: Optional[str]
 
     merchant_descriptor: str
 
     merchant_state: Optional[str]
 
 
+class TransactionSourceRealTimePaymentsTransferAcknowledgement(BaseModel):
+    amount: int
+    """The transfer amount in USD cents."""
+
+    destination_account_number: str
+    """The destination account number."""
+
+    destination_routing_number: str
+    """The American Bankers' Association (ABA) Routing Transit Number (RTN)."""
+
+    remittance_information: str
+    """Unstructured information that will show on the recipient's bank statement."""
+
+    transfer_id: str
+    """The identifier of the Real Time Payments Transfer that led to this Transaction."""
+
+
 class TransactionSourceSampleFunds(BaseModel):
     originator: str
     """Where the sample funds came from."""
 
 
 class TransactionSourceWireDrawdownPaymentIntention(BaseModel):
     account_number: str
@@ -916,14 +1044,21 @@
     card_refund: Optional[TransactionSourceCardRefund]
     """A Card Refund object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `card_refund`.
     """
 
+    card_revenue_payment: Optional[TransactionSourceCardRevenuePayment]
+    """A Card Revenue Payment object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `card_revenue_payment`.
+    """
+
     card_route_refund: Optional[TransactionSourceCardRouteRefund]
     """A Deprecated Card Refund object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `card_route_refund`.
     """
 
@@ -947,22 +1082,24 @@
         "ach_check_conversion",
         "ach_transfer_intention",
         "ach_transfer_rejection",
         "ach_transfer_return",
         "card_dispute_acceptance",
         "card_refund",
         "card_settlement",
+        "card_revenue_payment",
         "check_deposit_acceptance",
         "check_deposit_return",
         "check_transfer_intention",
         "check_transfer_return",
         "check_transfer_rejection",
         "check_transfer_stop_payment_request",
         "dispute_resolution",
         "empyreal_cash_deposit",
+        "fee_payment",
         "inbound_ach_transfer",
         "inbound_ach_transfer_return_intention",
         "inbound_check",
         "inbound_international_ach_transfer",
         "inbound_real_time_payments_transfer_confirmation",
         "inbound_wire_drawdown_payment_reversal",
         "inbound_wire_drawdown_payment",
@@ -1039,14 +1176,21 @@
     empyreal_cash_deposit: Optional[TransactionSourceEmpyrealCashDeposit]
     """A Empyreal Cash Deposit object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `empyreal_cash_deposit`.
     """
 
+    fee_payment: Optional[TransactionSourceFeePayment]
+    """A Fee Payment object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `fee_payment`.
+    """
+
     inbound_ach_transfer: Optional[TransactionSourceInboundACHTransfer]
     """A Inbound ACH Transfer object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `inbound_ach_transfer`.
     """
 
@@ -1111,14 +1255,21 @@
     internal_source: Optional[TransactionSourceInternalSource]
     """A Internal Source object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `internal_source`.
     """
 
+    real_time_payments_transfer_acknowledgement: Optional[TransactionSourceRealTimePaymentsTransferAcknowledgement]
+    """A Real Time Payments Transfer Acknowledgement object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `real_time_payments_transfer_acknowledgement`.
+    """
+
     sample_funds: Optional[TransactionSourceSampleFunds]
     """A Sample Funds object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `sample_funds`.
     """
 
@@ -1186,15 +1337,15 @@
 
     route_id: Optional[str]
     """The identifier for the route this Transaction came through.
 
     Routes are things like cards and ACH details.
     """
 
-    route_type: Optional[str]
+    route_type: Optional[Literal["account_number", "card"]]
     """The type of the route this Transaction came through."""
 
     source: TransactionSource
     """
     This is an object giving more details on the network-level event that caused the
     Transaction. Note that for backwards compatibility reasons, additional
     undocumented keys may appear in this object. These should be treated as
@@ -1226,19 +1377,20 @@
     reason: Literal[
         "ach_route_canceled",
         "ach_route_disabled",
         "breaches_limit",
         "credit_entry_refused_by_receiver",
         "duplicate_return",
         "entity_not_active",
-        "transaction_not_allowed",
         "group_locked",
         "insufficient_funds",
+        "misrouted_return",
         "no_ach_route",
         "originator_request",
+        "transaction_not_allowed",
     ]
     """Why the ACH transfer was declined."""
 
     receiver_id_number: Optional[str]
 
     receiver_name: Optional[str]
 
@@ -1334,18 +1486,21 @@
     reason: Literal[
         "card_not_active",
         "entity_not_active",
         "group_locked",
         "insufficient_funds",
         "cvv2_mismatch",
         "transaction_not_allowed",
+        "breaches_internal_limit",
         "breaches_limit",
         "webhook_declined",
         "webhook_timed_out",
         "declined_by_stand_in_processing",
+        "invalid_physical_card",
+        "missing_original_authorization",
     ]
     """Why the transaction was declined."""
 
 
 class DeclinedTransactionSourceCheckDecline(BaseModel):
     amount: int
     """The declined amount in the minor unit of the destination account currency.
@@ -1363,14 +1518,17 @@
         "group_locked",
         "insufficient_funds",
         "unable_to_locate_account",
         "unable_to_process",
         "refer_to_image",
         "stop_payment_requested",
         "returned",
+        "duplicate_presentment",
+        "not_authorized",
+        "altered_or_fictitious",
     ]
     """Why the check was declined."""
 
 
 class DeclinedTransactionSourceInboundRealTimePaymentsTransferDecline(BaseModel):
     amount: int
     """The declined amount in the minor unit of the destination account currency.
@@ -1396,14 +1554,15 @@
 
     debtor_routing_number: str
     """The routing number of the account that sent the transfer."""
 
     reason: Literal[
         "account_number_canceled",
         "account_number_disabled",
+        "account_restricted",
         "group_locked",
         "entity_not_active",
         "real_time_payments_not_enabled",
     ]
     """Why the transfer was declined."""
 
     remittance_information: Optional[str]
@@ -1513,14 +1672,62 @@
     merchant_country: str
 
     merchant_descriptor: str
 
     merchant_state: Optional[str]
 
 
+class DeclinedTransactionSourceWireDecline(BaseModel):
+    amount: int
+    """The declined amount in the minor unit of the destination account currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    beneficiary_address_line1: Optional[str]
+
+    beneficiary_address_line2: Optional[str]
+
+    beneficiary_address_line3: Optional[str]
+
+    beneficiary_name: Optional[str]
+
+    beneficiary_reference: Optional[str]
+
+    description: str
+
+    input_message_accountability_data: Optional[str]
+
+    originator_address_line1: Optional[str]
+
+    originator_address_line2: Optional[str]
+
+    originator_address_line3: Optional[str]
+
+    originator_name: Optional[str]
+
+    originator_to_beneficiary_information_line1: Optional[str]
+
+    originator_to_beneficiary_information_line2: Optional[str]
+
+    originator_to_beneficiary_information_line3: Optional[str]
+
+    originator_to_beneficiary_information_line4: Optional[str]
+
+    reason: Literal[
+        "account_number_canceled",
+        "account_number_disabled",
+        "entity_not_active",
+        "group_locked",
+        "no_account_number",
+        "transaction_not_allowed",
+    ]
+    """Why the wire transfer was declined."""
+
+
 class DeclinedTransactionSource(BaseModel):
     ach_decline: Optional[DeclinedTransactionSourceACHDecline]
     """A ACH Decline object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `ach_decline`.
     """
@@ -1542,14 +1749,15 @@
     category: Literal[
         "ach_decline",
         "card_decline",
         "check_decline",
         "inbound_real_time_payments_transfer_decline",
         "international_ach_decline",
         "card_route_decline",
+        "wire_decline",
         "other",
     ]
     """The type of decline that took place.
 
     We may add additional possible values for this enum over time; your application
     should be able to handle such additions gracefully.
     """
@@ -1573,14 +1781,21 @@
     international_ach_decline: Optional[DeclinedTransactionSourceInternationalACHDecline]
     """A International ACH Decline object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `international_ach_decline`.
     """
 
+    wire_decline: Optional[DeclinedTransactionSourceWireDecline]
+    """A Wire Decline object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `wire_decline`.
+    """
+
 
 class DeclinedTransaction(BaseModel):
     account_id: str
     """The identifier for the Account the Declined Transaction belongs to."""
 
     amount: int
     """The Declined Transaction amount in the minor unit of its currency.
@@ -1609,15 +1824,15 @@
 
     route_id: Optional[str]
     """The identifier for the route this Declined Transaction came through.
 
     Routes are things like cards and ACH details.
     """
 
-    route_type: Optional[str]
+    route_type: Optional[Literal["account_number", "card"]]
     """The type of the route this Declined Transaction came through."""
 
     source: DeclinedTransactionSource
     """
     This is an object giving more details on the network-level event that caused the
     Declined Transaction. For example, for a card transaction this lists the
     merchant's industry and location. Note that for backwards compatibility reasons,
```

### Comparing `increase-0.5.0/src/increase/types/simulations/card_authorization_simulation.py` & `increase-0.6.0/src/increase/types/simulations/card_authorization_simulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,26 +16,28 @@
     "PendingTransactionSourceCardAuthorization",
     "PendingTransactionSourceCardAuthorizationNetworkDetails",
     "PendingTransactionSourceCardAuthorizationNetworkDetailsVisa",
     "PendingTransactionSourceCheckDepositInstruction",
     "PendingTransactionSourceCheckTransferInstruction",
     "PendingTransactionSourceInboundFundsHold",
     "PendingTransactionSourceCardRouteAuthorization",
+    "PendingTransactionSourceRealTimePaymentsTransferInstruction",
     "PendingTransactionSourceWireDrawdownPaymentInstruction",
     "PendingTransactionSourceWireTransferInstruction",
     "DeclinedTransaction",
     "DeclinedTransactionSource",
     "DeclinedTransactionSourceACHDecline",
     "DeclinedTransactionSourceCardDecline",
     "DeclinedTransactionSourceCardDeclineNetworkDetails",
     "DeclinedTransactionSourceCardDeclineNetworkDetailsVisa",
     "DeclinedTransactionSourceCheckDecline",
     "DeclinedTransactionSourceInboundRealTimePaymentsTransferDecline",
     "DeclinedTransactionSourceInternationalACHDecline",
     "DeclinedTransactionSourceCardRouteDecline",
+    "DeclinedTransactionSourceWireDecline",
 ]
 
 
 class PendingTransactionSourceAccountTransferInstruction(BaseModel):
     amount: int
     """The pending amount in the minor unit of the transaction's currency.
 
@@ -109,14 +111,23 @@
 
     digital_wallet_token_id: Optional[str]
     """
     If the authorization was made via a Digital Wallet Token (such as an Apple Pay
     purchase), the identifier of the token that was used.
     """
 
+    expires_at: datetime
+    """
+    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) when this authorization
+    will expire and the pending transaction will be released.
+    """
+
+    id: str
+    """The Card Authorization identifier."""
+
     merchant_acceptor_id: str
     """
     The merchant identifier (commonly abbreviated as MID) of the merchant the card
     is transacting with.
     """
 
     merchant_category_code: Optional[str]
@@ -136,20 +147,29 @@
 
     network: Literal["visa"]
     """The payment network used to process this card authorization"""
 
     network_details: PendingTransactionSourceCardAuthorizationNetworkDetails
     """Fields specific to the `network`"""
 
+    pending_transaction_id: Optional[str]
+    """The identifier of the Pending Transaction associated with this Transaction."""
+
     real_time_decision_id: Optional[str]
     """
     The identifier of the Real-Time Decision sent to approve or decline this
     transaction.
     """
 
+    type: Literal["card_authorization"]
+    """A constant representing the object's type.
+
+    For this resource it will always be `card_authorization`.
+    """
+
 
 class PendingTransactionSourceCheckDepositInstruction(BaseModel):
     amount: int
     """The pending amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
     """
@@ -202,23 +222,32 @@
 
     automatically_releases_at: datetime
     """When the hold will be released automatically.
 
     Certain conditions may cause it to be released before this time.
     """
 
+    created_at: datetime
+    """
+    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) time at which the hold
+    was created.
+    """
+
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the hold's
     currency.
     """
 
     held_transaction_id: Optional[str]
     """The ID of the Transaction for which funds were held."""
 
+    pending_transaction_id: Optional[str]
+    """The ID of the Pending Transaction representing the held funds."""
+
     released_at: Optional[datetime]
     """When the hold was released (if it has been released)."""
 
     status: Literal["held", "complete"]
     """The status of the hold."""
 
 
@@ -244,14 +273,28 @@
     merchant_country: str
 
     merchant_descriptor: str
 
     merchant_state: Optional[str]
 
 
+class PendingTransactionSourceRealTimePaymentsTransferInstruction(BaseModel):
+    amount: int
+    """The pending amount in the minor unit of the transaction's currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    transfer_id: str
+    """
+    The identifier of the Real Time Payments Transfer that led to this Pending
+    Transaction.
+    """
+
+
 class PendingTransactionSourceWireDrawdownPaymentInstruction(BaseModel):
     account_number: str
 
     amount: int
     """The pending amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
@@ -343,14 +386,21 @@
     inbound_funds_hold: Optional[PendingTransactionSourceInboundFundsHold]
     """A Inbound Funds Hold object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `inbound_funds_hold`.
     """
 
+    real_time_payments_transfer_instruction: Optional[PendingTransactionSourceRealTimePaymentsTransferInstruction]
+    """A Real Time Payments Transfer Instruction object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `real_time_payments_transfer_instruction`.
+    """
+
     wire_drawdown_payment_instruction: Optional[PendingTransactionSourceWireDrawdownPaymentInstruction]
     """A Wire Drawdown Payment Instruction object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `wire_drawdown_payment_instruction`.
     """
 
@@ -368,14 +418,20 @@
 
     amount: int
     """The Pending Transaction amount in the minor unit of its currency.
 
     For dollars, for example, this is cents.
     """
 
+    completed_at: Optional[datetime]
+    """
+    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date on which the Pending
+    Transaction was completed.
+    """
+
     created_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date on which the Pending
     Transaction occured.
     """
 
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
@@ -397,15 +453,15 @@
 
     route_id: Optional[str]
     """The identifier for the route this Pending Transaction came through.
 
     Routes are things like cards and ACH details.
     """
 
-    route_type: Optional[str]
+    route_type: Optional[Literal["account_number", "card"]]
     """The type of the route this Pending Transaction came through."""
 
     source: PendingTransactionSource
     """
     This is an object giving more details on the network-level event that caused the
     Pending Transaction. For example, for a card transaction this lists the
     merchant's industry and location.
@@ -442,19 +498,20 @@
     reason: Literal[
         "ach_route_canceled",
         "ach_route_disabled",
         "breaches_limit",
         "credit_entry_refused_by_receiver",
         "duplicate_return",
         "entity_not_active",
-        "transaction_not_allowed",
         "group_locked",
         "insufficient_funds",
+        "misrouted_return",
         "no_ach_route",
         "originator_request",
+        "transaction_not_allowed",
     ]
     """Why the ACH transfer was declined."""
 
     receiver_id_number: Optional[str]
 
     receiver_name: Optional[str]
 
@@ -550,18 +607,21 @@
     reason: Literal[
         "card_not_active",
         "entity_not_active",
         "group_locked",
         "insufficient_funds",
         "cvv2_mismatch",
         "transaction_not_allowed",
+        "breaches_internal_limit",
         "breaches_limit",
         "webhook_declined",
         "webhook_timed_out",
         "declined_by_stand_in_processing",
+        "invalid_physical_card",
+        "missing_original_authorization",
     ]
     """Why the transaction was declined."""
 
 
 class DeclinedTransactionSourceCheckDecline(BaseModel):
     amount: int
     """The declined amount in the minor unit of the destination account currency.
@@ -579,14 +639,17 @@
         "group_locked",
         "insufficient_funds",
         "unable_to_locate_account",
         "unable_to_process",
         "refer_to_image",
         "stop_payment_requested",
         "returned",
+        "duplicate_presentment",
+        "not_authorized",
+        "altered_or_fictitious",
     ]
     """Why the check was declined."""
 
 
 class DeclinedTransactionSourceInboundRealTimePaymentsTransferDecline(BaseModel):
     amount: int
     """The declined amount in the minor unit of the destination account currency.
@@ -612,14 +675,15 @@
 
     debtor_routing_number: str
     """The routing number of the account that sent the transfer."""
 
     reason: Literal[
         "account_number_canceled",
         "account_number_disabled",
+        "account_restricted",
         "group_locked",
         "entity_not_active",
         "real_time_payments_not_enabled",
     ]
     """Why the transfer was declined."""
 
     remittance_information: Optional[str]
@@ -729,14 +793,62 @@
     merchant_country: str
 
     merchant_descriptor: str
 
     merchant_state: Optional[str]
 
 
+class DeclinedTransactionSourceWireDecline(BaseModel):
+    amount: int
+    """The declined amount in the minor unit of the destination account currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    beneficiary_address_line1: Optional[str]
+
+    beneficiary_address_line2: Optional[str]
+
+    beneficiary_address_line3: Optional[str]
+
+    beneficiary_name: Optional[str]
+
+    beneficiary_reference: Optional[str]
+
+    description: str
+
+    input_message_accountability_data: Optional[str]
+
+    originator_address_line1: Optional[str]
+
+    originator_address_line2: Optional[str]
+
+    originator_address_line3: Optional[str]
+
+    originator_name: Optional[str]
+
+    originator_to_beneficiary_information_line1: Optional[str]
+
+    originator_to_beneficiary_information_line2: Optional[str]
+
+    originator_to_beneficiary_information_line3: Optional[str]
+
+    originator_to_beneficiary_information_line4: Optional[str]
+
+    reason: Literal[
+        "account_number_canceled",
+        "account_number_disabled",
+        "entity_not_active",
+        "group_locked",
+        "no_account_number",
+        "transaction_not_allowed",
+    ]
+    """Why the wire transfer was declined."""
+
+
 class DeclinedTransactionSource(BaseModel):
     ach_decline: Optional[DeclinedTransactionSourceACHDecline]
     """A ACH Decline object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `ach_decline`.
     """
@@ -758,14 +870,15 @@
     category: Literal[
         "ach_decline",
         "card_decline",
         "check_decline",
         "inbound_real_time_payments_transfer_decline",
         "international_ach_decline",
         "card_route_decline",
+        "wire_decline",
         "other",
     ]
     """The type of decline that took place.
 
     We may add additional possible values for this enum over time; your application
     should be able to handle such additions gracefully.
     """
@@ -789,14 +902,21 @@
     international_ach_decline: Optional[DeclinedTransactionSourceInternationalACHDecline]
     """A International ACH Decline object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `international_ach_decline`.
     """
 
+    wire_decline: Optional[DeclinedTransactionSourceWireDecline]
+    """A Wire Decline object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `wire_decline`.
+    """
+
 
 class DeclinedTransaction(BaseModel):
     account_id: str
     """The identifier for the Account the Declined Transaction belongs to."""
 
     amount: int
     """The Declined Transaction amount in the minor unit of its currency.
@@ -825,15 +945,15 @@
 
     route_id: Optional[str]
     """The identifier for the route this Declined Transaction came through.
 
     Routes are things like cards and ACH details.
     """
 
-    route_type: Optional[str]
+    route_type: Optional[Literal["account_number", "card"]]
     """The type of the route this Declined Transaction came through."""
 
     source: DeclinedTransactionSource
     """
     This is an object giving more details on the network-level event that caused the
     Declined Transaction. For example, for a card transaction this lists the
     merchant's industry and location. Note that for backwards compatibility reasons,
```

### Comparing `increase-0.5.0/src/increase/types/simulations/card_settlement_params.py` & `increase-0.6.0/src/increase/types/simulations/card_settlement_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/simulations/digital_wallet_token_request_create_response.py` & `increase-0.6.0/src/increase/types/simulations/digital_wallet_token_request_create_response.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/simulations/inbound_real_time_payments_transfer_simulation_result.py` & `increase-0.6.0/src/increase/types/simulations/inbound_real_time_payments_transfer_simulation_result.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,34 +16,37 @@
     "TransactionSourceACHCheckConversion",
     "TransactionSourceACHTransferIntention",
     "TransactionSourceACHTransferRejection",
     "TransactionSourceACHTransferReturn",
     "TransactionSourceCardDisputeAcceptance",
     "TransactionSourceCardRefund",
     "TransactionSourceCardSettlement",
+    "TransactionSourceCardRevenuePayment",
     "TransactionSourceCheckDepositAcceptance",
     "TransactionSourceCheckDepositReturn",
     "TransactionSourceCheckTransferIntention",
     "TransactionSourceCheckTransferReturn",
     "TransactionSourceCheckTransferRejection",
     "TransactionSourceCheckTransferStopPaymentRequest",
     "TransactionSourceDisputeResolution",
     "TransactionSourceEmpyrealCashDeposit",
+    "TransactionSourceFeePayment",
     "TransactionSourceInboundACHTransfer",
     "TransactionSourceInboundCheck",
     "TransactionSourceInboundInternationalACHTransfer",
     "TransactionSourceInboundRealTimePaymentsTransferConfirmation",
     "TransactionSourceInboundWireDrawdownPaymentReversal",
     "TransactionSourceInboundWireDrawdownPayment",
     "TransactionSourceInboundWireReversal",
     "TransactionSourceInboundWireTransfer",
     "TransactionSourceInterestPayment",
     "TransactionSourceInternalSource",
     "TransactionSourceCardRouteRefund",
     "TransactionSourceCardRouteSettlement",
+    "TransactionSourceRealTimePaymentsTransferAcknowledgement",
     "TransactionSourceSampleFunds",
     "TransactionSourceWireDrawdownPaymentIntention",
     "TransactionSourceWireDrawdownPaymentRejection",
     "TransactionSourceWireTransferIntention",
     "TransactionSourceWireTransferRejection",
     "DeclinedTransaction",
     "DeclinedTransactionSource",
@@ -51,14 +54,15 @@
     "DeclinedTransactionSourceCardDecline",
     "DeclinedTransactionSourceCardDeclineNetworkDetails",
     "DeclinedTransactionSourceCardDeclineNetworkDetailsVisa",
     "DeclinedTransactionSourceCheckDecline",
     "DeclinedTransactionSourceInboundRealTimePaymentsTransferDecline",
     "DeclinedTransactionSourceInternationalACHDecline",
     "DeclinedTransactionSourceCardRouteDecline",
+    "DeclinedTransactionSourceWireDecline",
 ]
 
 
 class TransactionSourceAccountTransferIntention(BaseModel):
     amount: int
     """The pending amount in the minor unit of the transaction's currency.
 
@@ -175,66 +179,107 @@
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
     the Card Dispute was accepted.
     """
 
     card_dispute_id: str
     """The identifier of the Card Dispute that was accepted."""
 
-    transaction_id: Optional[str]
+    transaction_id: str
     """
     The identifier of the Transaction that was created to return the disputed funds
     to your account.
     """
 
 
 class TransactionSourceCardRefund(BaseModel):
     amount: int
     """The pending amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
     """
 
-    card_settlement_transaction_id: Optional[str]
-    """The identifier for the Transaction this refunds, if any."""
-
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
     transaction's currency.
     """
 
+    id: str
+    """The Card Refund identifier."""
+
+    merchant_acceptor_id: Optional[str]
+    """
+    The merchant identifier (commonly abbreviated as MID) of the merchant the card
+    is transacting with.
+    """
+
+    merchant_category_code: str
+    """The 4-digit MCC describing the merchant's business."""
+
+    merchant_city: Optional[str]
+    """The city the merchant resides in."""
+
+    merchant_country: str
+    """The country the merchant resides in."""
+
+    merchant_name: Optional[str]
+    """The name of the merchant."""
+
+    merchant_state: Optional[str]
+    """The state the merchant resides in."""
+
     type: Literal["card_refund"]
     """A constant representing the object's type.
 
     For this resource it will always be `card_refund`.
     """
 
 
 class TransactionSourceCardSettlement(BaseModel):
     amount: int
     """The amount in the minor unit of the transaction's settlement currency.
 
     For dollars, for example, this is cents.
     """
 
+    card_authorization: Optional[str]
+    """
+    The Card Authorization that was created prior to this Card Settlement, if on
+    exists.
+    """
+
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
     transaction's settlement currency.
     """
 
+    id: str
+    """The Card Settlement identifier."""
+
+    merchant_acceptor_id: Optional[str]
+    """
+    The merchant identifier (commonly abbreviated as MID) of the merchant the card
+    is transacting with.
+    """
+
     merchant_category_code: str
+    """The 4-digit MCC describing the merchant's business."""
 
     merchant_city: Optional[str]
+    """The city the merchant resides in."""
 
     merchant_country: str
+    """The country the merchant resides in."""
 
     merchant_name: Optional[str]
+    """The name of the merchant."""
 
     merchant_state: Optional[str]
+    """The state the merchant resides in."""
 
     pending_transaction_id: Optional[str]
     """The identifier of the Pending Transaction associated with this Transaction."""
 
     presentment_amount: int
     """The amount in the minor unit of the transaction's presentment currency."""
 
@@ -247,14 +292,37 @@
     type: Literal["card_settlement"]
     """A constant representing the object's type.
 
     For this resource it will always be `card_settlement`.
     """
 
 
+class TransactionSourceCardRevenuePayment(BaseModel):
+    amount: int
+    """The amount in the minor unit of the transaction's currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
+    """
+    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transaction
+    currency.
+    """
+
+    period_end: datetime
+    """The end of the period for which this transaction paid interest."""
+
+    period_start: datetime
+    """The start of the period for which this transaction paid interest."""
+
+    transacted_on_account_id: Optional[str]
+    """The account the card belonged to."""
+
+
 class TransactionSourceCheckDepositAcceptance(BaseModel):
     account_number: str
     """The account number printed on the check."""
 
     amount: int
     """The amount to be deposited in the minor unit of the transaction's currency.
 
@@ -362,14 +430,29 @@
     """The identifier of the Check Transfer with which this is associated."""
 
 
 class TransactionSourceCheckTransferReturn(BaseModel):
     file_id: Optional[str]
     """If available, a document with additional information about the return."""
 
+    reason: Literal["mail_delivery_failure", "refused_by_recipient", "returned_not_authorized"]
+    """The reason why the check was returned."""
+
+    returned_at: datetime
+    """
+    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
+    the check was returned.
+    """
+
+    transaction_id: Optional[str]
+    """
+    The identifier of the Transaction that was created to credit you for the
+    returned check.
+    """
+
     transfer_id: str
     """The identifier of the returned Check Transfer."""
 
 
 class TransactionSourceCheckTransferRejection(BaseModel):
     transfer_id: str
     """The identifier of the Check Transfer that led to this Transaction."""
@@ -417,14 +500,28 @@
     """
 
     bag_id: str
 
     deposit_date: datetime
 
 
+class TransactionSourceFeePayment(BaseModel):
+    amount: int
+    """The amount in the minor unit of the transaction's currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
+    """
+    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transaction
+    currency.
+    """
+
+
 class TransactionSourceInboundACHTransfer(BaseModel):
     amount: int
     """The amount in the minor unit of the destination account currency.
 
     For dollars, for example, this is cents.
     """
 
@@ -639,14 +736,20 @@
     originator_to_beneficiary_information: Optional[str]
 
 
 class TransactionSourceInboundWireReversal(BaseModel):
     amount: int
     """The amount that was reversed."""
 
+    created_at: datetime
+    """
+    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
+    the reversal was created.
+    """
+
     description: str
     """The description on the reversal message from Fedwire."""
 
     financial_institution_to_financial_institution_information: Optional[str]
     """Additional financial institution information included in the wire reversal."""
 
     input_cycle_date: date
@@ -675,14 +778,20 @@
 
     receiver_financial_institution_information: Optional[str]
     """
     Information included in the wire reversal for the receiving financial
     institution.
     """
 
+    transaction_id: Optional[str]
+    """The ID for the Transaction associated with the transfer reversal."""
+
+    wire_transfer_id: str
+    """The ID for the Wire Transfer that is being reversed."""
+
 
 class TransactionSourceInboundWireTransfer(BaseModel):
     amount: int
     """The amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
     """
@@ -755,19 +864,21 @@
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transaction
     currency.
     """
 
     reason: Literal[
         "bank_migration",
         "cashback",
+        "collection_receivable",
         "empyreal_adjustment",
         "error",
         "error_correction",
         "fees",
         "interest",
+        "negative_balance_forgiveness",
         "sample_funds",
         "sample_funds_return",
     ]
 
 
 class TransactionSourceCardRouteRefund(BaseModel):
     amount: int
@@ -817,14 +928,31 @@
     merchant_country: Optional[str]
 
     merchant_descriptor: str
 
     merchant_state: Optional[str]
 
 
+class TransactionSourceRealTimePaymentsTransferAcknowledgement(BaseModel):
+    amount: int
+    """The transfer amount in USD cents."""
+
+    destination_account_number: str
+    """The destination account number."""
+
+    destination_routing_number: str
+    """The American Bankers' Association (ABA) Routing Transit Number (RTN)."""
+
+    remittance_information: str
+    """Unstructured information that will show on the recipient's bank statement."""
+
+    transfer_id: str
+    """The identifier of the Real Time Payments Transfer that led to this Transaction."""
+
+
 class TransactionSourceSampleFunds(BaseModel):
     originator: str
     """Where the sample funds came from."""
 
 
 class TransactionSourceWireDrawdownPaymentIntention(BaseModel):
     account_number: str
@@ -916,14 +1044,21 @@
     card_refund: Optional[TransactionSourceCardRefund]
     """A Card Refund object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `card_refund`.
     """
 
+    card_revenue_payment: Optional[TransactionSourceCardRevenuePayment]
+    """A Card Revenue Payment object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `card_revenue_payment`.
+    """
+
     card_route_refund: Optional[TransactionSourceCardRouteRefund]
     """A Deprecated Card Refund object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `card_route_refund`.
     """
 
@@ -947,22 +1082,24 @@
         "ach_check_conversion",
         "ach_transfer_intention",
         "ach_transfer_rejection",
         "ach_transfer_return",
         "card_dispute_acceptance",
         "card_refund",
         "card_settlement",
+        "card_revenue_payment",
         "check_deposit_acceptance",
         "check_deposit_return",
         "check_transfer_intention",
         "check_transfer_return",
         "check_transfer_rejection",
         "check_transfer_stop_payment_request",
         "dispute_resolution",
         "empyreal_cash_deposit",
+        "fee_payment",
         "inbound_ach_transfer",
         "inbound_ach_transfer_return_intention",
         "inbound_check",
         "inbound_international_ach_transfer",
         "inbound_real_time_payments_transfer_confirmation",
         "inbound_wire_drawdown_payment_reversal",
         "inbound_wire_drawdown_payment",
@@ -1039,14 +1176,21 @@
     empyreal_cash_deposit: Optional[TransactionSourceEmpyrealCashDeposit]
     """A Empyreal Cash Deposit object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `empyreal_cash_deposit`.
     """
 
+    fee_payment: Optional[TransactionSourceFeePayment]
+    """A Fee Payment object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `fee_payment`.
+    """
+
     inbound_ach_transfer: Optional[TransactionSourceInboundACHTransfer]
     """A Inbound ACH Transfer object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `inbound_ach_transfer`.
     """
 
@@ -1111,14 +1255,21 @@
     internal_source: Optional[TransactionSourceInternalSource]
     """A Internal Source object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `internal_source`.
     """
 
+    real_time_payments_transfer_acknowledgement: Optional[TransactionSourceRealTimePaymentsTransferAcknowledgement]
+    """A Real Time Payments Transfer Acknowledgement object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `real_time_payments_transfer_acknowledgement`.
+    """
+
     sample_funds: Optional[TransactionSourceSampleFunds]
     """A Sample Funds object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `sample_funds`.
     """
 
@@ -1186,15 +1337,15 @@
 
     route_id: Optional[str]
     """The identifier for the route this Transaction came through.
 
     Routes are things like cards and ACH details.
     """
 
-    route_type: Optional[str]
+    route_type: Optional[Literal["account_number", "card"]]
     """The type of the route this Transaction came through."""
 
     source: TransactionSource
     """
     This is an object giving more details on the network-level event that caused the
     Transaction. Note that for backwards compatibility reasons, additional
     undocumented keys may appear in this object. These should be treated as
@@ -1226,19 +1377,20 @@
     reason: Literal[
         "ach_route_canceled",
         "ach_route_disabled",
         "breaches_limit",
         "credit_entry_refused_by_receiver",
         "duplicate_return",
         "entity_not_active",
-        "transaction_not_allowed",
         "group_locked",
         "insufficient_funds",
+        "misrouted_return",
         "no_ach_route",
         "originator_request",
+        "transaction_not_allowed",
     ]
     """Why the ACH transfer was declined."""
 
     receiver_id_number: Optional[str]
 
     receiver_name: Optional[str]
 
@@ -1334,18 +1486,21 @@
     reason: Literal[
         "card_not_active",
         "entity_not_active",
         "group_locked",
         "insufficient_funds",
         "cvv2_mismatch",
         "transaction_not_allowed",
+        "breaches_internal_limit",
         "breaches_limit",
         "webhook_declined",
         "webhook_timed_out",
         "declined_by_stand_in_processing",
+        "invalid_physical_card",
+        "missing_original_authorization",
     ]
     """Why the transaction was declined."""
 
 
 class DeclinedTransactionSourceCheckDecline(BaseModel):
     amount: int
     """The declined amount in the minor unit of the destination account currency.
@@ -1363,14 +1518,17 @@
         "group_locked",
         "insufficient_funds",
         "unable_to_locate_account",
         "unable_to_process",
         "refer_to_image",
         "stop_payment_requested",
         "returned",
+        "duplicate_presentment",
+        "not_authorized",
+        "altered_or_fictitious",
     ]
     """Why the check was declined."""
 
 
 class DeclinedTransactionSourceInboundRealTimePaymentsTransferDecline(BaseModel):
     amount: int
     """The declined amount in the minor unit of the destination account currency.
@@ -1396,14 +1554,15 @@
 
     debtor_routing_number: str
     """The routing number of the account that sent the transfer."""
 
     reason: Literal[
         "account_number_canceled",
         "account_number_disabled",
+        "account_restricted",
         "group_locked",
         "entity_not_active",
         "real_time_payments_not_enabled",
     ]
     """Why the transfer was declined."""
 
     remittance_information: Optional[str]
@@ -1513,14 +1672,62 @@
     merchant_country: str
 
     merchant_descriptor: str
 
     merchant_state: Optional[str]
 
 
+class DeclinedTransactionSourceWireDecline(BaseModel):
+    amount: int
+    """The declined amount in the minor unit of the destination account currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    beneficiary_address_line1: Optional[str]
+
+    beneficiary_address_line2: Optional[str]
+
+    beneficiary_address_line3: Optional[str]
+
+    beneficiary_name: Optional[str]
+
+    beneficiary_reference: Optional[str]
+
+    description: str
+
+    input_message_accountability_data: Optional[str]
+
+    originator_address_line1: Optional[str]
+
+    originator_address_line2: Optional[str]
+
+    originator_address_line3: Optional[str]
+
+    originator_name: Optional[str]
+
+    originator_to_beneficiary_information_line1: Optional[str]
+
+    originator_to_beneficiary_information_line2: Optional[str]
+
+    originator_to_beneficiary_information_line3: Optional[str]
+
+    originator_to_beneficiary_information_line4: Optional[str]
+
+    reason: Literal[
+        "account_number_canceled",
+        "account_number_disabled",
+        "entity_not_active",
+        "group_locked",
+        "no_account_number",
+        "transaction_not_allowed",
+    ]
+    """Why the wire transfer was declined."""
+
+
 class DeclinedTransactionSource(BaseModel):
     ach_decline: Optional[DeclinedTransactionSourceACHDecline]
     """A ACH Decline object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `ach_decline`.
     """
@@ -1542,14 +1749,15 @@
     category: Literal[
         "ach_decline",
         "card_decline",
         "check_decline",
         "inbound_real_time_payments_transfer_decline",
         "international_ach_decline",
         "card_route_decline",
+        "wire_decline",
         "other",
     ]
     """The type of decline that took place.
 
     We may add additional possible values for this enum over time; your application
     should be able to handle such additions gracefully.
     """
@@ -1573,14 +1781,21 @@
     international_ach_decline: Optional[DeclinedTransactionSourceInternationalACHDecline]
     """A International ACH Decline object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `international_ach_decline`.
     """
 
+    wire_decline: Optional[DeclinedTransactionSourceWireDecline]
+    """A Wire Decline object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `wire_decline`.
+    """
+
 
 class DeclinedTransaction(BaseModel):
     account_id: str
     """The identifier for the Account the Declined Transaction belongs to."""
 
     amount: int
     """The Declined Transaction amount in the minor unit of its currency.
@@ -1609,15 +1824,15 @@
 
     route_id: Optional[str]
     """The identifier for the route this Declined Transaction came through.
 
     Routes are things like cards and ACH details.
     """
 
-    route_type: Optional[str]
+    route_type: Optional[Literal["account_number", "card"]]
     """The type of the route this Declined Transaction came through."""
 
     source: DeclinedTransactionSource
     """
     This is an object giving more details on the network-level event that caused the
     Declined Transaction. For example, for a card transaction this lists the
     merchant's industry and location. Note that for backwards compatibility reasons,
```

### Comparing `increase-0.5.0/src/increase/types/simulations/inbound_wire_drawdown_request_create_params.py` & `increase-0.6.0/src/increase/types/simulations/inbound_wire_drawdown_request_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/simulations/real_time_payments_transfer_create_inbound_params.py` & `increase-0.6.0/src/increase/types/simulations/real_time_payments_transfer_create_inbound_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/simulations/wire_transfer_create_inbound_params.py` & `increase-0.6.0/src/increase/types/simulations/wire_transfer_create_inbound_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/simulations/wire_transfer_simulation.py` & `increase-0.6.0/src/increase/types/simulations/interest_payment_simulation_result.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,46 +3,49 @@
 from typing import Optional
 from datetime import date, datetime
 from typing_extensions import Literal
 
 from ..._models import BaseModel
 
 __all__ = [
-    "WireTransferSimulation",
+    "InterestPaymentSimulationResult",
     "Transaction",
     "TransactionSource",
     "TransactionSourceAccountTransferIntention",
     "TransactionSourceACHCheckConversionReturn",
     "TransactionSourceACHCheckConversion",
     "TransactionSourceACHTransferIntention",
     "TransactionSourceACHTransferRejection",
     "TransactionSourceACHTransferReturn",
     "TransactionSourceCardDisputeAcceptance",
     "TransactionSourceCardRefund",
     "TransactionSourceCardSettlement",
+    "TransactionSourceCardRevenuePayment",
     "TransactionSourceCheckDepositAcceptance",
     "TransactionSourceCheckDepositReturn",
     "TransactionSourceCheckTransferIntention",
     "TransactionSourceCheckTransferReturn",
     "TransactionSourceCheckTransferRejection",
     "TransactionSourceCheckTransferStopPaymentRequest",
     "TransactionSourceDisputeResolution",
     "TransactionSourceEmpyrealCashDeposit",
+    "TransactionSourceFeePayment",
     "TransactionSourceInboundACHTransfer",
     "TransactionSourceInboundCheck",
     "TransactionSourceInboundInternationalACHTransfer",
     "TransactionSourceInboundRealTimePaymentsTransferConfirmation",
     "TransactionSourceInboundWireDrawdownPaymentReversal",
     "TransactionSourceInboundWireDrawdownPayment",
     "TransactionSourceInboundWireReversal",
     "TransactionSourceInboundWireTransfer",
     "TransactionSourceInterestPayment",
     "TransactionSourceInternalSource",
     "TransactionSourceCardRouteRefund",
     "TransactionSourceCardRouteSettlement",
+    "TransactionSourceRealTimePaymentsTransferAcknowledgement",
     "TransactionSourceSampleFunds",
     "TransactionSourceWireDrawdownPaymentIntention",
     "TransactionSourceWireDrawdownPaymentRejection",
     "TransactionSourceWireTransferIntention",
     "TransactionSourceWireTransferRejection",
 ]
 
@@ -164,66 +167,107 @@
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
     the Card Dispute was accepted.
     """
 
     card_dispute_id: str
     """The identifier of the Card Dispute that was accepted."""
 
-    transaction_id: Optional[str]
+    transaction_id: str
     """
     The identifier of the Transaction that was created to return the disputed funds
     to your account.
     """
 
 
 class TransactionSourceCardRefund(BaseModel):
     amount: int
     """The pending amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
     """
 
-    card_settlement_transaction_id: Optional[str]
-    """The identifier for the Transaction this refunds, if any."""
-
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
     transaction's currency.
     """
 
+    id: str
+    """The Card Refund identifier."""
+
+    merchant_acceptor_id: Optional[str]
+    """
+    The merchant identifier (commonly abbreviated as MID) of the merchant the card
+    is transacting with.
+    """
+
+    merchant_category_code: str
+    """The 4-digit MCC describing the merchant's business."""
+
+    merchant_city: Optional[str]
+    """The city the merchant resides in."""
+
+    merchant_country: str
+    """The country the merchant resides in."""
+
+    merchant_name: Optional[str]
+    """The name of the merchant."""
+
+    merchant_state: Optional[str]
+    """The state the merchant resides in."""
+
     type: Literal["card_refund"]
     """A constant representing the object's type.
 
     For this resource it will always be `card_refund`.
     """
 
 
 class TransactionSourceCardSettlement(BaseModel):
     amount: int
     """The amount in the minor unit of the transaction's settlement currency.
 
     For dollars, for example, this is cents.
     """
 
+    card_authorization: Optional[str]
+    """
+    The Card Authorization that was created prior to this Card Settlement, if on
+    exists.
+    """
+
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
     transaction's settlement currency.
     """
 
+    id: str
+    """The Card Settlement identifier."""
+
+    merchant_acceptor_id: Optional[str]
+    """
+    The merchant identifier (commonly abbreviated as MID) of the merchant the card
+    is transacting with.
+    """
+
     merchant_category_code: str
+    """The 4-digit MCC describing the merchant's business."""
 
     merchant_city: Optional[str]
+    """The city the merchant resides in."""
 
     merchant_country: str
+    """The country the merchant resides in."""
 
     merchant_name: Optional[str]
+    """The name of the merchant."""
 
     merchant_state: Optional[str]
+    """The state the merchant resides in."""
 
     pending_transaction_id: Optional[str]
     """The identifier of the Pending Transaction associated with this Transaction."""
 
     presentment_amount: int
     """The amount in the minor unit of the transaction's presentment currency."""
 
@@ -236,14 +280,37 @@
     type: Literal["card_settlement"]
     """A constant representing the object's type.
 
     For this resource it will always be `card_settlement`.
     """
 
 
+class TransactionSourceCardRevenuePayment(BaseModel):
+    amount: int
+    """The amount in the minor unit of the transaction's currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
+    """
+    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transaction
+    currency.
+    """
+
+    period_end: datetime
+    """The end of the period for which this transaction paid interest."""
+
+    period_start: datetime
+    """The start of the period for which this transaction paid interest."""
+
+    transacted_on_account_id: Optional[str]
+    """The account the card belonged to."""
+
+
 class TransactionSourceCheckDepositAcceptance(BaseModel):
     account_number: str
     """The account number printed on the check."""
 
     amount: int
     """The amount to be deposited in the minor unit of the transaction's currency.
 
@@ -351,14 +418,29 @@
     """The identifier of the Check Transfer with which this is associated."""
 
 
 class TransactionSourceCheckTransferReturn(BaseModel):
     file_id: Optional[str]
     """If available, a document with additional information about the return."""
 
+    reason: Literal["mail_delivery_failure", "refused_by_recipient", "returned_not_authorized"]
+    """The reason why the check was returned."""
+
+    returned_at: datetime
+    """
+    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
+    the check was returned.
+    """
+
+    transaction_id: Optional[str]
+    """
+    The identifier of the Transaction that was created to credit you for the
+    returned check.
+    """
+
     transfer_id: str
     """The identifier of the returned Check Transfer."""
 
 
 class TransactionSourceCheckTransferRejection(BaseModel):
     transfer_id: str
     """The identifier of the Check Transfer that led to this Transaction."""
@@ -406,14 +488,28 @@
     """
 
     bag_id: str
 
     deposit_date: datetime
 
 
+class TransactionSourceFeePayment(BaseModel):
+    amount: int
+    """The amount in the minor unit of the transaction's currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
+    """
+    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transaction
+    currency.
+    """
+
+
 class TransactionSourceInboundACHTransfer(BaseModel):
     amount: int
     """The amount in the minor unit of the destination account currency.
 
     For dollars, for example, this is cents.
     """
 
@@ -628,14 +724,20 @@
     originator_to_beneficiary_information: Optional[str]
 
 
 class TransactionSourceInboundWireReversal(BaseModel):
     amount: int
     """The amount that was reversed."""
 
+    created_at: datetime
+    """
+    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
+    the reversal was created.
+    """
+
     description: str
     """The description on the reversal message from Fedwire."""
 
     financial_institution_to_financial_institution_information: Optional[str]
     """Additional financial institution information included in the wire reversal."""
 
     input_cycle_date: date
@@ -664,14 +766,20 @@
 
     receiver_financial_institution_information: Optional[str]
     """
     Information included in the wire reversal for the receiving financial
     institution.
     """
 
+    transaction_id: Optional[str]
+    """The ID for the Transaction associated with the transfer reversal."""
+
+    wire_transfer_id: str
+    """The ID for the Wire Transfer that is being reversed."""
+
 
 class TransactionSourceInboundWireTransfer(BaseModel):
     amount: int
     """The amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
     """
@@ -744,19 +852,21 @@
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transaction
     currency.
     """
 
     reason: Literal[
         "bank_migration",
         "cashback",
+        "collection_receivable",
         "empyreal_adjustment",
         "error",
         "error_correction",
         "fees",
         "interest",
+        "negative_balance_forgiveness",
         "sample_funds",
         "sample_funds_return",
     ]
 
 
 class TransactionSourceCardRouteRefund(BaseModel):
     amount: int
@@ -806,14 +916,31 @@
     merchant_country: Optional[str]
 
     merchant_descriptor: str
 
     merchant_state: Optional[str]
 
 
+class TransactionSourceRealTimePaymentsTransferAcknowledgement(BaseModel):
+    amount: int
+    """The transfer amount in USD cents."""
+
+    destination_account_number: str
+    """The destination account number."""
+
+    destination_routing_number: str
+    """The American Bankers' Association (ABA) Routing Transit Number (RTN)."""
+
+    remittance_information: str
+    """Unstructured information that will show on the recipient's bank statement."""
+
+    transfer_id: str
+    """The identifier of the Real Time Payments Transfer that led to this Transaction."""
+
+
 class TransactionSourceSampleFunds(BaseModel):
     originator: str
     """Where the sample funds came from."""
 
 
 class TransactionSourceWireDrawdownPaymentIntention(BaseModel):
     account_number: str
@@ -905,14 +1032,21 @@
     card_refund: Optional[TransactionSourceCardRefund]
     """A Card Refund object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `card_refund`.
     """
 
+    card_revenue_payment: Optional[TransactionSourceCardRevenuePayment]
+    """A Card Revenue Payment object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `card_revenue_payment`.
+    """
+
     card_route_refund: Optional[TransactionSourceCardRouteRefund]
     """A Deprecated Card Refund object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `card_route_refund`.
     """
 
@@ -936,22 +1070,24 @@
         "ach_check_conversion",
         "ach_transfer_intention",
         "ach_transfer_rejection",
         "ach_transfer_return",
         "card_dispute_acceptance",
         "card_refund",
         "card_settlement",
+        "card_revenue_payment",
         "check_deposit_acceptance",
         "check_deposit_return",
         "check_transfer_intention",
         "check_transfer_return",
         "check_transfer_rejection",
         "check_transfer_stop_payment_request",
         "dispute_resolution",
         "empyreal_cash_deposit",
+        "fee_payment",
         "inbound_ach_transfer",
         "inbound_ach_transfer_return_intention",
         "inbound_check",
         "inbound_international_ach_transfer",
         "inbound_real_time_payments_transfer_confirmation",
         "inbound_wire_drawdown_payment_reversal",
         "inbound_wire_drawdown_payment",
@@ -1028,14 +1164,21 @@
     empyreal_cash_deposit: Optional[TransactionSourceEmpyrealCashDeposit]
     """A Empyreal Cash Deposit object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `empyreal_cash_deposit`.
     """
 
+    fee_payment: Optional[TransactionSourceFeePayment]
+    """A Fee Payment object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `fee_payment`.
+    """
+
     inbound_ach_transfer: Optional[TransactionSourceInboundACHTransfer]
     """A Inbound ACH Transfer object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `inbound_ach_transfer`.
     """
 
@@ -1100,14 +1243,21 @@
     internal_source: Optional[TransactionSourceInternalSource]
     """A Internal Source object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `internal_source`.
     """
 
+    real_time_payments_transfer_acknowledgement: Optional[TransactionSourceRealTimePaymentsTransferAcknowledgement]
+    """A Real Time Payments Transfer Acknowledgement object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `real_time_payments_transfer_acknowledgement`.
+    """
+
     sample_funds: Optional[TransactionSourceSampleFunds]
     """A Sample Funds object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `sample_funds`.
     """
 
@@ -1175,15 +1325,15 @@
 
     route_id: Optional[str]
     """The identifier for the route this Transaction came through.
 
     Routes are things like cards and ACH details.
     """
 
-    route_type: Optional[str]
+    route_type: Optional[Literal["account_number", "card"]]
     """The type of the route this Transaction came through."""
 
     source: TransactionSource
     """
     This is an object giving more details on the network-level event that caused the
     Transaction. Note that for backwards compatibility reasons, additional
     undocumented keys may appear in this object. These should be treated as
@@ -1193,20 +1343,19 @@
     type: Literal["transaction"]
     """A constant representing the object's type.
 
     For this resource it will always be `transaction`.
     """
 
 
-class WireTransferSimulation(BaseModel):
+class InterestPaymentSimulationResult(BaseModel):
     transaction: Transaction
-    """
-    If the Wire Transfer attempt succeeds, this will contain the resulting
-    [Transaction](#transactions) object. The Transaction's `source` will be of
-    `category: inbound_wire_transfer`.
+    """This will contain the resulting [Transaction](#transactions) object.
+
+    The Transaction's `source` will be of `category: interest_payment`.
     """
 
-    type: Literal["inbound_wire_transfer_simulation_result"]
+    type: Literal["interest_payment_simulation_result"]
     """A constant representing the object's type.
 
-    For this resource it will always be `inbound_wire_transfer_simulation_result`.
+    For this resource it will always be `interest_payment_simulation_result`.
     """
```

### Comparing `increase-0.5.0/src/increase/types/transaction.py` & `increase-0.6.0/src/increase/types/transaction.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,34 +14,37 @@
     "SourceACHCheckConversion",
     "SourceACHTransferIntention",
     "SourceACHTransferRejection",
     "SourceACHTransferReturn",
     "SourceCardDisputeAcceptance",
     "SourceCardRefund",
     "SourceCardSettlement",
+    "SourceCardRevenuePayment",
     "SourceCheckDepositAcceptance",
     "SourceCheckDepositReturn",
     "SourceCheckTransferIntention",
     "SourceCheckTransferReturn",
     "SourceCheckTransferRejection",
     "SourceCheckTransferStopPaymentRequest",
     "SourceDisputeResolution",
     "SourceEmpyrealCashDeposit",
+    "SourceFeePayment",
     "SourceInboundACHTransfer",
     "SourceInboundCheck",
     "SourceInboundInternationalACHTransfer",
     "SourceInboundRealTimePaymentsTransferConfirmation",
     "SourceInboundWireDrawdownPaymentReversal",
     "SourceInboundWireDrawdownPayment",
     "SourceInboundWireReversal",
     "SourceInboundWireTransfer",
     "SourceInterestPayment",
     "SourceInternalSource",
     "SourceCardRouteRefund",
     "SourceCardRouteSettlement",
+    "SourceRealTimePaymentsTransferAcknowledgement",
     "SourceSampleFunds",
     "SourceWireDrawdownPaymentIntention",
     "SourceWireDrawdownPaymentRejection",
     "SourceWireTransferIntention",
     "SourceWireTransferRejection",
 ]
 
@@ -163,66 +166,107 @@
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
     the Card Dispute was accepted.
     """
 
     card_dispute_id: str
     """The identifier of the Card Dispute that was accepted."""
 
-    transaction_id: Optional[str]
+    transaction_id: str
     """
     The identifier of the Transaction that was created to return the disputed funds
     to your account.
     """
 
 
 class SourceCardRefund(BaseModel):
     amount: int
     """The pending amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
     """
 
-    card_settlement_transaction_id: Optional[str]
-    """The identifier for the Transaction this refunds, if any."""
-
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
     transaction's currency.
     """
 
+    id: str
+    """The Card Refund identifier."""
+
+    merchant_acceptor_id: Optional[str]
+    """
+    The merchant identifier (commonly abbreviated as MID) of the merchant the card
+    is transacting with.
+    """
+
+    merchant_category_code: str
+    """The 4-digit MCC describing the merchant's business."""
+
+    merchant_city: Optional[str]
+    """The city the merchant resides in."""
+
+    merchant_country: str
+    """The country the merchant resides in."""
+
+    merchant_name: Optional[str]
+    """The name of the merchant."""
+
+    merchant_state: Optional[str]
+    """The state the merchant resides in."""
+
     type: Literal["card_refund"]
     """A constant representing the object's type.
 
     For this resource it will always be `card_refund`.
     """
 
 
 class SourceCardSettlement(BaseModel):
     amount: int
     """The amount in the minor unit of the transaction's settlement currency.
 
     For dollars, for example, this is cents.
     """
 
+    card_authorization: Optional[str]
+    """
+    The Card Authorization that was created prior to this Card Settlement, if on
+    exists.
+    """
+
     currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
     """
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
     transaction's settlement currency.
     """
 
+    id: str
+    """The Card Settlement identifier."""
+
+    merchant_acceptor_id: Optional[str]
+    """
+    The merchant identifier (commonly abbreviated as MID) of the merchant the card
+    is transacting with.
+    """
+
     merchant_category_code: str
+    """The 4-digit MCC describing the merchant's business."""
 
     merchant_city: Optional[str]
+    """The city the merchant resides in."""
 
     merchant_country: str
+    """The country the merchant resides in."""
 
     merchant_name: Optional[str]
+    """The name of the merchant."""
 
     merchant_state: Optional[str]
+    """The state the merchant resides in."""
 
     pending_transaction_id: Optional[str]
     """The identifier of the Pending Transaction associated with this Transaction."""
 
     presentment_amount: int
     """The amount in the minor unit of the transaction's presentment currency."""
 
@@ -235,14 +279,37 @@
     type: Literal["card_settlement"]
     """A constant representing the object's type.
 
     For this resource it will always be `card_settlement`.
     """
 
 
+class SourceCardRevenuePayment(BaseModel):
+    amount: int
+    """The amount in the minor unit of the transaction's currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
+    """
+    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transaction
+    currency.
+    """
+
+    period_end: datetime
+    """The end of the period for which this transaction paid interest."""
+
+    period_start: datetime
+    """The start of the period for which this transaction paid interest."""
+
+    transacted_on_account_id: Optional[str]
+    """The account the card belonged to."""
+
+
 class SourceCheckDepositAcceptance(BaseModel):
     account_number: str
     """The account number printed on the check."""
 
     amount: int
     """The amount to be deposited in the minor unit of the transaction's currency.
 
@@ -350,14 +417,29 @@
     """The identifier of the Check Transfer with which this is associated."""
 
 
 class SourceCheckTransferReturn(BaseModel):
     file_id: Optional[str]
     """If available, a document with additional information about the return."""
 
+    reason: Literal["mail_delivery_failure", "refused_by_recipient", "returned_not_authorized"]
+    """The reason why the check was returned."""
+
+    returned_at: datetime
+    """
+    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
+    the check was returned.
+    """
+
+    transaction_id: Optional[str]
+    """
+    The identifier of the Transaction that was created to credit you for the
+    returned check.
+    """
+
     transfer_id: str
     """The identifier of the returned Check Transfer."""
 
 
 class SourceCheckTransferRejection(BaseModel):
     transfer_id: str
     """The identifier of the Check Transfer that led to this Transaction."""
@@ -405,14 +487,28 @@
     """
 
     bag_id: str
 
     deposit_date: datetime
 
 
+class SourceFeePayment(BaseModel):
+    amount: int
+    """The amount in the minor unit of the transaction's currency.
+
+    For dollars, for example, this is cents.
+    """
+
+    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
+    """
+    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transaction
+    currency.
+    """
+
+
 class SourceInboundACHTransfer(BaseModel):
     amount: int
     """The amount in the minor unit of the destination account currency.
 
     For dollars, for example, this is cents.
     """
 
@@ -627,14 +723,20 @@
     originator_to_beneficiary_information: Optional[str]
 
 
 class SourceInboundWireReversal(BaseModel):
     amount: int
     """The amount that was reversed."""
 
+    created_at: datetime
+    """
+    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
+    the reversal was created.
+    """
+
     description: str
     """The description on the reversal message from Fedwire."""
 
     financial_institution_to_financial_institution_information: Optional[str]
     """Additional financial institution information included in the wire reversal."""
 
     input_cycle_date: date
@@ -663,14 +765,20 @@
 
     receiver_financial_institution_information: Optional[str]
     """
     Information included in the wire reversal for the receiving financial
     institution.
     """
 
+    transaction_id: Optional[str]
+    """The ID for the Transaction associated with the transfer reversal."""
+
+    wire_transfer_id: str
+    """The ID for the Wire Transfer that is being reversed."""
+
 
 class SourceInboundWireTransfer(BaseModel):
     amount: int
     """The amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
     """
@@ -743,19 +851,21 @@
     The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the transaction
     currency.
     """
 
     reason: Literal[
         "bank_migration",
         "cashback",
+        "collection_receivable",
         "empyreal_adjustment",
         "error",
         "error_correction",
         "fees",
         "interest",
+        "negative_balance_forgiveness",
         "sample_funds",
         "sample_funds_return",
     ]
 
 
 class SourceCardRouteRefund(BaseModel):
     amount: int
@@ -805,14 +915,31 @@
     merchant_country: Optional[str]
 
     merchant_descriptor: str
 
     merchant_state: Optional[str]
 
 
+class SourceRealTimePaymentsTransferAcknowledgement(BaseModel):
+    amount: int
+    """The transfer amount in USD cents."""
+
+    destination_account_number: str
+    """The destination account number."""
+
+    destination_routing_number: str
+    """The American Bankers' Association (ABA) Routing Transit Number (RTN)."""
+
+    remittance_information: str
+    """Unstructured information that will show on the recipient's bank statement."""
+
+    transfer_id: str
+    """The identifier of the Real Time Payments Transfer that led to this Transaction."""
+
+
 class SourceSampleFunds(BaseModel):
     originator: str
     """Where the sample funds came from."""
 
 
 class SourceWireDrawdownPaymentIntention(BaseModel):
     account_number: str
@@ -904,14 +1031,21 @@
     card_refund: Optional[SourceCardRefund]
     """A Card Refund object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `card_refund`.
     """
 
+    card_revenue_payment: Optional[SourceCardRevenuePayment]
+    """A Card Revenue Payment object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `card_revenue_payment`.
+    """
+
     card_route_refund: Optional[SourceCardRouteRefund]
     """A Deprecated Card Refund object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `card_route_refund`.
     """
 
@@ -935,22 +1069,24 @@
         "ach_check_conversion",
         "ach_transfer_intention",
         "ach_transfer_rejection",
         "ach_transfer_return",
         "card_dispute_acceptance",
         "card_refund",
         "card_settlement",
+        "card_revenue_payment",
         "check_deposit_acceptance",
         "check_deposit_return",
         "check_transfer_intention",
         "check_transfer_return",
         "check_transfer_rejection",
         "check_transfer_stop_payment_request",
         "dispute_resolution",
         "empyreal_cash_deposit",
+        "fee_payment",
         "inbound_ach_transfer",
         "inbound_ach_transfer_return_intention",
         "inbound_check",
         "inbound_international_ach_transfer",
         "inbound_real_time_payments_transfer_confirmation",
         "inbound_wire_drawdown_payment_reversal",
         "inbound_wire_drawdown_payment",
@@ -1027,14 +1163,21 @@
     empyreal_cash_deposit: Optional[SourceEmpyrealCashDeposit]
     """A Empyreal Cash Deposit object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `empyreal_cash_deposit`.
     """
 
+    fee_payment: Optional[SourceFeePayment]
+    """A Fee Payment object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `fee_payment`.
+    """
+
     inbound_ach_transfer: Optional[SourceInboundACHTransfer]
     """A Inbound ACH Transfer object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `inbound_ach_transfer`.
     """
 
@@ -1097,14 +1240,21 @@
     internal_source: Optional[SourceInternalSource]
     """A Internal Source object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `internal_source`.
     """
 
+    real_time_payments_transfer_acknowledgement: Optional[SourceRealTimePaymentsTransferAcknowledgement]
+    """A Real Time Payments Transfer Acknowledgement object.
+
+    This field will be present in the JSON response if and only if `category` is
+    equal to `real_time_payments_transfer_acknowledgement`.
+    """
+
     sample_funds: Optional[SourceSampleFunds]
     """A Sample Funds object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `sample_funds`.
     """
 
@@ -1172,15 +1322,15 @@
 
     route_id: Optional[str]
     """The identifier for the route this Transaction came through.
 
     Routes are things like cards and ACH details.
     """
 
-    route_type: Optional[str]
+    route_type: Optional[Literal["account_number", "card"]]
     """The type of the route this Transaction came through."""
 
     source: Source
     """
     This is an object giving more details on the network-level event that caused the
     Transaction. Note that for backwards compatibility reasons, additional
     undocumented keys may appear in this object. These should be treated as
```

### Comparing `increase-0.5.0/src/increase/types/transaction_list_params.py` & `increase-0.6.0/src/increase/types/transaction_list_params.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,22 +47,24 @@
                 "ach_check_conversion",
                 "ach_transfer_intention",
                 "ach_transfer_rejection",
                 "ach_transfer_return",
                 "card_dispute_acceptance",
                 "card_refund",
                 "card_settlement",
+                "card_revenue_payment",
                 "check_deposit_acceptance",
                 "check_deposit_return",
                 "check_transfer_intention",
                 "check_transfer_return",
                 "check_transfer_rejection",
                 "check_transfer_stop_payment_request",
                 "dispute_resolution",
                 "empyreal_cash_deposit",
+                "fee_payment",
                 "inbound_ach_transfer",
                 "inbound_ach_transfer_return_intention",
                 "inbound_check",
                 "inbound_international_ach_transfer",
                 "inbound_real_time_payments_transfer_confirmation",
                 "inbound_wire_drawdown_payment_reversal",
                 "inbound_wire_drawdown_payment",
@@ -105,8 +107,11 @@
     limit: int
     """Limit the size of the list that is returned.
 
     The default (and maximum) is 100 objects.
     """
 
     route_id: str
-    """Filter Transactions for those belonging to the specified route."""
+    """Filter Transactions for those belonging to the specified route.
+
+    This could be a Card ID or an Account Number ID.
+    """
```

### Comparing `increase-0.5.0/src/increase/types/wire_drawdown_request.py` & `increase-0.6.0/src/increase/types/wire_drawdown_request.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/wire_drawdown_request_create_params.py` & `increase-0.6.0/src/increase/types/wire_drawdown_request_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/wire_transfer.py` & `increase-0.6.0/src/increase/types/wire_transfer.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,27 +12,45 @@
 class Approval(BaseModel):
     approved_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
     the transfer was approved.
     """
 
+    approved_by: Optional[str]
+    """
+    If the Transfer was approved by a user in the dashboard, the email address of
+    that user.
+    """
+
 
 class Cancellation(BaseModel):
     canceled_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
     the Transfer was canceled.
     """
 
+    canceled_by: Optional[str]
+    """
+    If the Transfer was canceled by a user in the dashboard, the email address of
+    that user.
+    """
+
 
 class Reversal(BaseModel):
     amount: int
     """The amount that was reversed."""
 
+    created_at: datetime
+    """
+    The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
+    the reversal was created.
+    """
+
     description: str
     """The description on the reversal message from Fedwire."""
 
     financial_institution_to_financial_institution_information: Optional[str]
     """Additional financial institution information included in the wire reversal."""
 
     input_cycle_date: date
@@ -61,14 +79,20 @@
 
     receiver_financial_institution_information: Optional[str]
     """
     Information included in the wire reversal for the receiving financial
     institution.
     """
 
+    transaction_id: Optional[str]
+    """The ID for the Transaction associated with the transfer reversal."""
+
+    wire_transfer_id: str
+    """The ID for the Wire Transfer that is being reversed."""
+
 
 class Submission(BaseModel):
     input_message_accountability_data: str
     """The accountability data for the submission."""
 
     submitted_at: datetime
     """When this wire transfer was submitted to Fedwire."""
@@ -145,17 +169,14 @@
 
     submission: Optional[Submission]
     """
     After the transfer is submitted to Fedwire, this will contain supplemental
     details.
     """
 
-    template_id: Optional[str]
-    """If the transfer was created from a template, this will be the template's ID."""
-
     transaction_id: Optional[str]
     """The ID for the transaction funding the transfer."""
 
     type: Literal["wire_transfer"]
     """A constant representing the object's type.
 
     For this resource it will always be `wire_transfer`.
```

### Comparing `increase-0.5.0/src/increase/types/wire_transfer_create_params.py` & `increase-0.6.0/src/increase/types/wire_transfer_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/src/increase/types/wire_transfer_list_params.py` & `increase-0.6.0/src/increase/types/wire_transfer_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.5.0/setup.py` & `increase-0.6.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,47 +1,332 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: increase
+Version: 0.6.0
+Summary: Client library for the increase API
+Home-page: https://github.com/increase/increase-python
+License: Apache-2.0
+Author: Increase
+Author-email: dev-feedback@increase.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: anyio (>=3.5.0)
+Requires-Dist: distro (>=1.7.0)
+Requires-Dist: httpx (>=0.23.0)
+Requires-Dist: pydantic (>=1.9.0)
+Requires-Dist: typing-extensions (>=4.1.1)
+Project-URL: Repository, https://github.com/increase/increase-python
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# Increase Python API Library
 
-packages = \
-['increase',
- 'increase._utils',
- 'increase.resources',
- 'increase.resources.entities',
- 'increase.resources.simulations',
- 'increase.types',
- 'increase.types.entities',
- 'increase.types.shared',
- 'increase.types.shared_params',
- 'increase.types.simulations']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['anyio>=3.5.0',
- 'distro>=1.7.0',
- 'httpx>=0.23.0',
- 'pydantic>=1.9.0',
- 'typing-extensions>=4.1.1']
-
-setup_kwargs = {
-    'name': 'increase',
-    'version': '0.5.0',
-    'description': 'Client library for the increase API',
-    'long_description': '# Increase Python API Library\n\n[![PyPI version](https://img.shields.io/pypi/v/increase.svg)](https://pypi.org/project/increase/)\n\nThe Increase Python library provides convenient access to the Increase REST API from any Python 3.7+\napplication. It includes type definitions for all request params and response fields,\nand offers both synchronous and asynchronous clients powered by [httpx](https://github.com/encode/httpx).\n\n## Documentation\n\nThe API documentation can be found [here](https://increase.com/documentation).\n\n## Installation\n\n```sh\npip install increase\n```\n\n## Usage\n\n```python\nfrom increase import Increase\n\nincrease = Increase(\n    # defaults to os.environ.get("INCREASE_API_KEY")\n    api_key="my api key",\n    # defaults to "production".\n    environment="sandbox",\n)\n\naccount = increase.accounts.create(\n    name="My First Increase Account",\n)\nprint(account.id)\n```\n\nWhile you can provide an `api_key` keyword argument, we recommend using [python-dotenv](https://pypi.org/project/python-dotenv/)\nand adding `INCREASE_API_KEY="my api key"` to your `.env` file so that your API Key is not stored in source control.\n\n## Async Usage\n\nSimply import `AsyncIncrease` instead of `Increase` and use `await` with each API call:\n\n```python\nfrom increase import AsyncIncrease\n\nincrease = AsyncIncrease(\n    # defaults to os.environ.get("INCREASE_API_KEY")\n    api_key="my api key",\n    # defaults to "production".\n    environment="sandbox",\n)\n\n\nasync def main():\n    account = await increase.accounts.create(\n        name="My First Increase Account",\n    )\n    print(account.id)\n\n\nasyncio.run(main())\n```\n\nFunctionality between the synchronous and asynchronous clients is otherwise identical.\n\n## Using Types\n\nNested request parameters are [TypedDicts](https://docs.python.org/3/library/typing.html#typing.TypedDict), while responses are [Pydantic](https://pydantic-docs.helpmanual.io/) models. This helps provide autocomplete and documentation within your editor.\n\nIf you would like to see type errors in VS Code to help catch bugs earlier, set `python.analysis.typeCheckingMode` to `"basic"`.\n\n## Pagination\n\nList methods in the Increase API are paginated.\n\nThis library provides auto-paginating iterators with each list response, so you do not have to request successive pages manually:\n\n```python\nimport increase\n\nincrease = Increase()\n\nall_accounts = []\n# Automatically fetches more pages as needed.\nfor account in increase.accounts.list():\n    # Do something with account here\n    all_accounts.append(account)\nprint(all_accounts)\n```\n\nOr, asynchronously:\n\n```python\nimport asyncio\nimport increase\n\nincrease = AsyncIncrease()\n\n\nasync def main() -> None:\n    all_accounts = []\n    # Iterate through items across all pages, issuing requests as needed.\n    async for account in increase.accounts.list():\n        all_accounts.append(account)\n    print(all_accounts)\n\n\nasyncio.run(main())\n```\n\nAlternatively, you can use the `.has_next_page()`, `.next_page_info()`, or `.get_next_page()` methods for more granular control working with pages:\n\n```python\nfirst_page = await increase.accounts.list()\nif first_page.has_next_page():\n    print(f"will fetch next page using these details: {first_page.next_page_info()}")\n    next_page = await first_page.get_next_page()\n    print(f"number of items we just fetched: {len(next_page.data)}")\n\n# Remove `await` for non-async usage.\n```\n\nOr just work directly with the returned data:\n\n```python\nfirst_page = await increase.accounts.list()\n\nprint(f"next page cursor: {first_page.next_cursor}")  # => "next page cursor: ..."\nfor account in first_page.data:\n    print(account.balances)\n\n# Remove `await` for non-async usage.\n```\n\n## Nested params\n\nNested parameters are dictionaries, typed using `TypedDict`, for example:\n\n```py\nfrom increase import Increase\n\nincrease = Increase()\n\nincrease.accounts.create(\n    foo={\n        "bar": True\n    },\n)\n```\n\n## File Uploads\n\nRequest parameters that correspond to file uploads can be passed as `bytes` or a tuple of `(filename, contents, media type)`.\n\n```python\nfrom pathlib import Path\nfrom increase import Increase\n\nincrease = Increase()\n\ncontents = Path("my/file.txt").read_bytes()\nincrease.files.create(\n    file=contents,\n    purpose="other",\n)\n```\n\nThe async client uses the exact same interface. This example uses `aiofiles` to asynchronously read the file contents but you can use whatever method you would like.\n\n```python\nimport aiofiles\nfrom increase import Increase\n\nincrease = Increase()\n\nasync with aiofiles.open("pytest.ini", mode="rb") as f:\n    contents = await f.read()\n\nawait increase.files.create(\n    file=contents,\n    purpose="other",\n)\n```\n\n## Handling errors\n\nWhen the library is unable to connect to the API (e.g., due to network connection problems or a timeout), a subclass of `increase.APIConnectionError` is raised.\n\nWhen the API returns a non-success status code (i.e., 4xx or 5xx\nresponse), a subclass of `increase.APIStatusError` will be raised, containing `status_code` and `response` properties.\n\nAll errors inherit from `increase.APIError`.\n\n```python\nfrom increase import Increase\n\nincrease = Increase()\n\ntry:\n    increase.accounts.create(\n        naem="Oops",\n    )\nexcept increase.APIConnectionError as e:\n    print("The server could not be reached")\n    print(e.__cause__)  # an underlying Exception, likely raised within httpx.\nexcept increase.RateLimitError as e:\n    print("A 429 status code was received; we should back off a bit.")\nexcept increase.APIStatusError as e:\n    print("Another non-200-range status code was received")\n    print(e.status_code)\n    print(e.response)\n```\n\nError codes are as followed:\n\n| Status Code | Error Type                 |\n| ----------- | -------------------------- |\n| 400         | `BadRequestError`          |\n| 401         | `AuthenticationError`      |\n| 403         | `PermissionDeniedError`    |\n| 404         | `NotFoundError`            |\n| 422         | `UnprocessableEntityError` |\n| 429         | `RateLimitError`           |\n| >=500       | `InternalServerError`      |\n| N/A         | `APIConnectionError`       |\n\n### Retries\n\nCertain errors will be automatically retried 2 times by default, with a short exponential backoff.\nConnection errors (for example, due to a network connectivity problem), 409 Conflict, 429 Rate Limit,\nand >=500 Internal errors will all be retried by default.\n\nYou can use the `max_retries` option to configure or disable this:\n\n```python\nfrom increase import Increase\n\n# Configure the default for all requests:\nincrease = Increase(\n    # default is 2\n    max_retries=0,\n)\n\n# Or, configure per-request:\nincrease.with_options(max_retries=5).accounts.create(\n    name="Jack",\n)\n```\n\n### Timeouts\n\nRequests time out after 60 seconds by default. You can configure this with a `timeout` option,\nwhich accepts a float or an [`httpx.Timeout`](https://www.python-httpx.org/advanced/#fine-tuning-the-configuration):\n\n```python\nfrom increase import Increase\n\n# Configure the default for all requests:\nincrease = Increase(\n    # default is 60s\n    timeout=20.0,\n)\n\n# More granular control:\nincrease = Increase(\n    timeout=httpx.Timeout(60.0, read=5.0, write=10.0, connect=2.0),\n)\n\n# Override per-request:\nincrease.with_options(timeout=5 * 1000).accounts.list(\n    status="open",\n)\n```\n\nOn timeout, an `APITimeoutError` is thrown.\n\nNote that requests which time out will be [retried twice by default](#retries).\n\n## Advanced: Configuring custom URLs, proxies, and transports\n\nYou can configure the following keyword arguments when instantiating the client:\n\n```python\nimport httpx\nfrom increase import Increase\n\nincrease = Increase(\n    # Use a custom base URL\n    base_url="http://my.test.server.example.com:8083",\n    proxies="http://my.test.proxy.example.com",\n    transport=httpx.HTTPTransport(local_address="0.0.0.0"),\n)\n```\n\nSee the httpx documentation for information about the [`proxies`](https://www.python-httpx.org/advanced/#http-proxying) and [`transport`](https://www.python-httpx.org/advanced/#custom-transports) keyword arguments.\n\n## Status\n\nThis package is in beta. Its internals and interfaces are not stable and subject to change without a major semver bump;\nplease reach out if you rely on any undocumented behavior.\n\nWe are keen for your feedback; please email us at [dev-feedback@increase.com](mailto:dev-feedback@increase.com) or open an issue with questions,\nbugs, or suggestions.\n\n## Requirements\n\nPython 3.7 or higher.',
-    'author': 'Increase',
-    'author_email': 'dev-feedback@increase.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/increase/increase-python',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
+[![PyPI version](https://img.shields.io/pypi/v/increase.svg)](https://pypi.org/project/increase/)
 
+The Increase Python library provides convenient access to the Increase REST API from any Python 3.7+
+application. It includes type definitions for all request params and response fields,
+and offers both synchronous and asynchronous clients powered by [httpx](https://github.com/encode/httpx).
 
-setup(**setup_kwargs)
+## Documentation
+
+The API documentation can be found [here](https://increase.com/documentation).
+
+## Installation
+
+```sh
+pip install increase
+```
+
+## Usage
+
+```python
+from increase import Increase
+
+increase = Increase(
+    # defaults to os.environ.get("INCREASE_API_KEY")
+    api_key="my api key",
+    # defaults to "production".
+    environment="sandbox",
+)
+
+account = increase.accounts.create(
+    name="My First Increase Account",
+)
+print(account.id)
+```
+
+While you can provide an `api_key` keyword argument, we recommend using [python-dotenv](https://pypi.org/project/python-dotenv/)
+and adding `INCREASE_API_KEY="my api key"` to your `.env` file so that your API Key is not stored in source control.
+
+## Async Usage
+
+Simply import `AsyncIncrease` instead of `Increase` and use `await` with each API call:
+
+```python
+from increase import AsyncIncrease
+
+increase = AsyncIncrease(
+    # defaults to os.environ.get("INCREASE_API_KEY")
+    api_key="my api key",
+    # defaults to "production".
+    environment="sandbox",
+)
+
+
+async def main():
+    account = await increase.accounts.create(
+        name="My First Increase Account",
+    )
+    print(account.id)
+
+
+asyncio.run(main())
+```
+
+Functionality between the synchronous and asynchronous clients is otherwise identical.
+
+## Using Types
+
+Nested request parameters are [TypedDicts](https://docs.python.org/3/library/typing.html#typing.TypedDict), while responses are [Pydantic](https://pydantic-docs.helpmanual.io/) models. This helps provide autocomplete and documentation within your editor.
+
+If you would like to see type errors in VS Code to help catch bugs earlier, set `python.analysis.typeCheckingMode` to `"basic"`.
+
+## Pagination
+
+List methods in the Increase API are paginated.
+
+This library provides auto-paginating iterators with each list response, so you do not have to request successive pages manually:
+
+```python
+import increase
+
+increase = Increase()
+
+all_accounts = []
+# Automatically fetches more pages as needed.
+for account in increase.accounts.list():
+    # Do something with account here
+    all_accounts.append(account)
+print(all_accounts)
+```
+
+Or, asynchronously:
+
+```python
+import asyncio
+import increase
+
+increase = AsyncIncrease()
+
+
+async def main() -> None:
+    all_accounts = []
+    # Iterate through items across all pages, issuing requests as needed.
+    async for account in increase.accounts.list():
+        all_accounts.append(account)
+    print(all_accounts)
+
+
+asyncio.run(main())
+```
+
+Alternatively, you can use the `.has_next_page()`, `.next_page_info()`, or `.get_next_page()` methods for more granular control working with pages:
+
+```python
+first_page = await increase.accounts.list()
+if first_page.has_next_page():
+    print(f"will fetch next page using these details: {first_page.next_page_info()}")
+    next_page = await first_page.get_next_page()
+    print(f"number of items we just fetched: {len(next_page.data)}")
+
+# Remove `await` for non-async usage.
+```
+
+Or just work directly with the returned data:
+
+```python
+first_page = await increase.accounts.list()
+
+print(f"next page cursor: {first_page.next_cursor}")  # => "next page cursor: ..."
+for account in first_page.data:
+    print(account.created_at)
+
+# Remove `await` for non-async usage.
+```
+
+## Nested params
+
+Nested parameters are dictionaries, typed using `TypedDict`, for example:
+
+```python
+from increase import Increase
+
+increase = Increase()
+
+increase.accounts.create(
+    foo={
+        "bar": True,
+    },
+)
+```
+
+## File Uploads
+
+Request parameters that correspond to file uploads can be passed as `bytes` or a tuple of `(filename, contents, media type)`.
+
+```python
+from pathlib import Path
+from increase import Increase
+
+increase = Increase()
+
+contents = Path("my/file.txt").read_bytes()
+increase.files.create(
+    file=contents,
+    purpose="other",
+)
+```
+
+The async client uses the exact same interface. This example uses `aiofiles` to asynchronously read the file contents but you can use whatever method you would like.
+
+```python
+import aiofiles
+from increase import Increase
+
+increase = Increase()
+
+async with aiofiles.open("pytest.ini", mode="rb") as f:
+    contents = await f.read()
+
+await increase.files.create(
+    file=contents,
+    purpose="other",
+)
+```
+
+## Handling errors
+
+When the library is unable to connect to the API (e.g., due to network connection problems or a timeout), a subclass of `increase.APIConnectionError` is raised.
+
+When the API returns a non-success status code (i.e., 4xx or 5xx
+response), a subclass of `increase.APIStatusError` will be raised, containing `status_code` and `response` properties.
+
+All errors inherit from `increase.APIError`.
+
+```python
+from increase import Increase
+
+increase = Increase()
+
+try:
+    increase.accounts.create(
+        naem="Oops",
+    )
+except increase.APIConnectionError as e:
+    print("The server could not be reached")
+    print(e.__cause__)  # an underlying Exception, likely raised within httpx.
+except increase.RateLimitError as e:
+    print("A 429 status code was received; we should back off a bit.")
+except increase.APIStatusError as e:
+    print("Another non-200-range status code was received")
+    print(e.status_code)
+    print(e.response)
+```
+
+Error codes are as followed:
+
+| Status Code | Error Type                 |
+| ----------- | -------------------------- |
+| 400         | `BadRequestError`          |
+| 401         | `AuthenticationError`      |
+| 403         | `PermissionDeniedError`    |
+| 404         | `NotFoundError`            |
+| 422         | `UnprocessableEntityError` |
+| 429         | `RateLimitError`           |
+| >=500       | `InternalServerError`      |
+| N/A         | `APIConnectionError`       |
+
+### Retries
+
+Certain errors will be automatically retried 2 times by default, with a short exponential backoff.
+Connection errors (for example, due to a network connectivity problem), 409 Conflict, 429 Rate Limit,
+and >=500 Internal errors will all be retried by default.
+
+You can use the `max_retries` option to configure or disable this:
+
+```python
+from increase import Increase
+
+# Configure the default for all requests:
+increase = Increase(
+    # default is 2
+    max_retries=0,
+)
+
+# Or, configure per-request:
+increase.with_options(max_retries=5).accounts.create(
+    name="Jack",
+)
+```
+
+### Timeouts
+
+Requests time out after 60 seconds by default. You can configure this with a `timeout` option,
+which accepts a float or an [`httpx.Timeout`](https://www.python-httpx.org/advanced/#fine-tuning-the-configuration):
+
+```python
+from increase import Increase
+
+# Configure the default for all requests:
+increase = Increase(
+    # default is 60s
+    timeout=20.0,
+)
+
+# More granular control:
+increase = Increase(
+    timeout=httpx.Timeout(60.0, read=5.0, write=10.0, connect=2.0),
+)
+
+# Override per-request:
+increase.with_options(timeout=5 * 1000).accounts.list(
+    status="open",
+)
+```
+
+On timeout, an `APITimeoutError` is thrown.
+
+Note that requests which time out will be [retried twice by default](#retries).
+
+## Advanced: Configuring custom URLs, proxies, and transports
+
+You can configure the following keyword arguments when instantiating the client:
+
+```python
+import httpx
+from increase import Increase
+
+increase = Increase(
+    # Use a custom base URL
+    base_url="http://my.test.server.example.com:8083",
+    proxies="http://my.test.proxy.example.com",
+    transport=httpx.HTTPTransport(local_address="0.0.0.0"),
+)
+```
+
+See the httpx documentation for information about the [`proxies`](https://www.python-httpx.org/advanced/#http-proxying) and [`transport`](https://www.python-httpx.org/advanced/#custom-transports) keyword arguments.
+
+## Status
+
+This package is in beta. Its internals and interfaces are not stable and subject to change without a major semver bump;
+please reach out if you rely on any undocumented behavior.
+
+We are keen for your feedback; please email us at [dev-feedback@increase.com](mailto:dev-feedback@increase.com) or open an issue with questions,
+bugs, or suggestions.
+
+## Requirements
+
+Python 3.7 or higher.
```

