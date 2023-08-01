# Comparing `tmp/naruno-0.60.1.tar.gz` & `tmp/naruno-0.60.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naruno-0.60.1.tar", last modified: Sat Jul 29 00:28:26 2023, max compression
+gzip compressed data, was "naruno-0.60.2.tar", last modified: Tue Aug  1 14:28:23 2023, max compression
```

## Comparing `naruno-0.60.1.tar` & `naruno-0.60.2.tar`

### file list

```diff
@@ -1,304 +1,304 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.595879 naruno-0.60.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-29 00:28:12.000000 naruno-0.60.1/LICENCE-naruno-gui_lib__.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-29 00:28:12.000000 naruno-0.60.1/LICENCE-naruno-lib-kot__.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-29 00:28:12.000000 naruno-0.60.1/LICENCE-naruno-lib-mix__.md
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-29 00:28:12.000000 naruno-0.60.1/LICENCE-naruno-wallet-elipticcurve__.md
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-29 00:28:12.000000 naruno-0.60.1/LICENSE-others__.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-29 00:28:12.000000 naruno-0.60.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-07-29 00:28:26.595879 naruno-0.60.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-07-29 00:28:12.000000 naruno-0.60.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.567879 naruno-0.60.1/naruno/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.567879 naruno-0.60.1/naruno/accounts/
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/accounts/account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.567879 naruno-0.60.1/naruno/accounts/commanders/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/accounts/commanders/delete_commander.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/accounts/commanders/get_comnder.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/accounts/commanders/save_commander.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/accounts/get_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/accounts/get_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/accounts/get_sequence_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/accounts/save_accounts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.567879 naruno-0.60.1/naruno/api/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.567879 naruno-0.60.1/naruno/api/buildozer/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/api/buildozer/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    25532 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/api/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.567879 naruno-0.60.1/naruno/apps/
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/apps/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)    29604 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/apps/remote_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.559879 naruno-0.60.1/naruno/blockchain/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.571879 naruno-0.60.1/naruno/blockchain/block/
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/blockchain/block/block_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/blockchain/block/blocks_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/blockchain/block/change_transaction_fee.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/blockchain/block/create_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/blockchain/block/get_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/blockchain/block/get_block_from_blockchain_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/blockchain/block/get_minumum_transfer_amount.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.571879 naruno-0.60.1/naruno/blockchain/block/hash/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/blockchain/block/hash/accounts_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/blockchain/block/hash/blocks_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/blockchain/block/hash/calculate_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/blockchain/block/hash/tx_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/blockchain/block/just_one_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/blockchain/block/max_data_size.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/blockchain/block/max_tx_number.py
--rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/blockchain/block/save_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/blockchain/block/save_block_to_blockchain_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/blockchain/block/shares.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.571879 naruno-0.60.1/naruno/blockchain/candidate_block/
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/blockchain/candidate_block/candidate_block_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.571879 naruno-0.60.1/naruno/cli/
--rw-r--r--   0 runner    (1001) docker     (123)    18299 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.571879 naruno-0.60.1/naruno/consensus/
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/consensus/consensus_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.571879 naruno-0.60.1/naruno/consensus/finished/
--rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/consensus/finished/finished_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.571879 naruno-0.60.1/naruno/consensus/finished/transactions/
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/consensus/finished/transactions/transactions_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.571879 naruno-0.60.1/naruno/consensus/finished/true_time/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/consensus/finished/true_time/true_time_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.571879 naruno-0.60.1/naruno/consensus/ongoing/
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/consensus/ongoing/ongoing_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.559879 naruno-0.60.1/naruno/consensus/rounds/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.571879 naruno-0.60.1/naruno/consensus/rounds/round_1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.571879 naruno-0.60.1/naruno/consensus/rounds/round_1/checks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.571879 naruno-0.60.1/naruno/consensus/rounds/round_1/checks/candidate_blocks/
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/consensus/rounds/round_1/checks/candidate_blocks/candidate_blocks_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/consensus/rounds/round_1/checks/checks_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.559879 naruno-0.60.1/naruno/consensus/rounds/round_1/checks/time/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.571879 naruno-0.60.1/naruno/consensus/rounds/round_1/checks/time/time_difference/
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/consensus/rounds/round_1/checks/time/time_difference/time_difference_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.571879 naruno-0.60.1/naruno/consensus/rounds/round_1/process/
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/consensus/rounds/round_1/process/process_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.571879 naruno-0.60.1/naruno/consensus/rounds/round_1/process/transactions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.571879 naruno-0.60.1/naruno/consensus/rounds/round_1/process/transactions/checks/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/consensus/rounds/round_1/process/transactions/checks/duplicated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.571879 naruno-0.60.1/naruno/consensus/rounds/round_1/process/transactions/find_newly/
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/consensus/rounds/round_1/process/transactions/find_newly/find_newly_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.571879 naruno-0.60.1/naruno/consensus/rounds/round_1/process/transactions/find_validated/
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/consensus/rounds/round_1/process/transactions/find_validated/find_validated_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/consensus/rounds/round_1/process/transactions/transactions_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/consensus/rounds/round_1/round_1_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.571879 naruno-0.60.1/naruno/consensus/rounds/round_2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.571879 naruno-0.60.1/naruno/consensus/rounds/round_2/checks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.571879 naruno-0.60.1/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/candidate_blocks_hashes_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/consensus/rounds/round_2/checks/checks_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.563879 naruno-0.60.1/naruno/consensus/rounds/round_2/checks/time/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.571879 naruno-0.60.1/naruno/consensus/rounds/round_2/checks/time/time_difference/
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/consensus/rounds/round_2/checks/time/time_difference/time_difference_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.571879 naruno-0.60.1/naruno/consensus/rounds/round_2/process/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.571879 naruno-0.60.1/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/candidate_blocks_hashes_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/consensus/rounds/round_2/process/process_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.571879 naruno-0.60.1/naruno/consensus/rounds/round_2/process/rescue/
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/consensus/rounds/round_2/process/rescue/rescue_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.571879 naruno-0.60.1/naruno/consensus/rounds/round_2/process/validate/
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/consensus/rounds/round_2/process/validate/validate_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/consensus/rounds/round_2/round_2_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.575879 naruno-0.60.1/naruno/consensus/sync/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/consensus/sync/send_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/consensus/sync/send_block_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/consensus/sync/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.575879 naruno-0.60.1/naruno/db/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/db/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.575879 naruno-0.60.1/naruno/db/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/db/blocks/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.575879 naruno-0.60.1/naruno/db/commanders/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/db/commanders/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.575879 naruno-0.60.1/naruno/db/connected_nodes/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/db/connected_nodes/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.575879 naruno-0.60.1/naruno/db/connected_nodes_test_0/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/db/connected_nodes_test_0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.575879 naruno-0.60.1/naruno/db/connected_nodes_test_1/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/db/connected_nodes_test_1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.575879 naruno-0.60.1/naruno/db/connected_nodes_test_2/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/db/connected_nodes_test_2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.575879 naruno-0.60.1/naruno/db/extracted_proofs/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/db/extracted_proofs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.575879 naruno-0.60.1/naruno/db/my_transactions/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/db/my_transactions/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.575879 naruno-0.60.1/naruno/db/pending_transactions/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/db/pending_transactions/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.575879 naruno-0.60.1/naruno/db/pending_transactions_test_0/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/db/pending_transactions_test_0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.575879 naruno-0.60.1/naruno/db/pending_transactions_test_1/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/db/pending_transactions_test_1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.575879 naruno-0.60.1/naruno/db/pending_transactions_test_2/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/db/pending_transactions_test_2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.575879 naruno-0.60.1/naruno/db/proof/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/db/proof/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.575879 naruno-0.60.1/naruno/db/qrs/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/db/qrs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.575879 naruno-0.60.1/naruno/db/remote_app_cache/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/db/remote_app_cache/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.575879 naruno-0.60.1/naruno/db/signs/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/db/signs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.575879 naruno-0.60.1/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.575879 naruno-0.60.1/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB_not_our_transaction/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB_not_our_transaction/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.575879 naruno-0.60.1/naruno/db/test_consensus_trigger_finished/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/db/test_consensus_trigger_finished/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.575879 naruno-0.60.1/naruno/db/test_finished_main/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/db/test_finished_main/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.575879 naruno-0.60.1/naruno/db/test_finished_main_2/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/db/test_finished_main_2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.575879 naruno-0.60.1/naruno/db/test_finished_main_3/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/db/test_finished_main_3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.575879 naruno-0.60.1/naruno/db/test_finished_main_false_time/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/db/test_finished_main_false_time/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.575879 naruno-0.60.1/naruno/db/test_finished_main_no_reset/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/db/test_finished_main_no_reset/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.575879 naruno-0.60.1/naruno/db/test_proof_extracted/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/db/test_proof_extracted/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.575879 naruno-0.60.1/naruno/gui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.563879 naruno-0.60.1/naruno/gui/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.583879 naruno-0.60.1/naruno/gui/lib/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/gui/lib/fonts/POPPINS_LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)   151396 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/gui/lib/fonts/Poppins-Black.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   171604 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/gui/lib/fonts/Poppins-BlackItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   153944 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/gui/lib/fonts/Poppins-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   176588 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/gui/lib/fonts/Poppins-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   152764 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/gui/lib/fonts/Poppins-ExtraBold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   173916 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/gui/lib/fonts/Poppins-ExtraBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   161456 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/gui/lib/fonts/Poppins-ExtraLight.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   186168 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/gui/lib/fonts/Poppins-ExtraLightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   182012 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/gui/lib/fonts/Poppins-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   159892 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/gui/lib/fonts/Poppins-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   184460 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/gui/lib/fonts/Poppins-LightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   156520 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/gui/lib/fonts/Poppins-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   180444 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/gui/lib/fonts/Poppins-MediumItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   158240 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/gui/lib/fonts/Poppins-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   155232 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/gui/lib/fonts/Poppins-SemiBold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   178584 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/gui/lib/fonts/Poppins-SemiBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   161652 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/gui/lib/fonts/Poppins-Thin.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   187044 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/gui/lib/fonts/Poppins-ThinItalic.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.583879 naruno-0.60.1/naruno/gui/lib/images/
--rw-r--r--   0 runner    (1001) docker     (123)   254014 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/gui/lib/images/logo.ico
--rw-r--r--   0 runner    (1001) docker     (123)    19780 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/gui/lib/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    16238 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/gui/lib/images/logo_sm_orb_fw.png
--rw-r--r--   0 runner    (1001) docker     (123)    21468 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/gui/lib/images/logo_w_bc.png
--rw-r--r--   0 runner    (1001) docker     (123)   254014 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/gui/lib/images/logo_win.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.563879 naruno-0.60.1/naruno/gui/lib/libs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.583879 naruno-0.60.1/naruno/gui/lib/libs/baseclass/
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/gui/lib/libs/baseclass/node_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/gui/lib/libs/baseclass/operations_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/gui/lib/libs/baseclass/root_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/gui/lib/libs/baseclass/settings_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/gui/lib/libs/baseclass/tabnavigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/gui/lib/libs/baseclass/wallet_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/gui/lib/libs/baseclass/welcome_screen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.583879 naruno-0.60.1/naruno/gui/lib/libs/kv/
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/gui/lib/libs/kv/node_screen.kv
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/gui/lib/libs/kv/operations_screen.kv
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/gui/lib/libs/kv/root_screen.kv
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/gui/lib/libs/kv/settings_screen.kv
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/gui/lib/libs/kv/tabnavigation.kv
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/gui/lib/libs/kv/wallet_screen.kv
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/gui/lib/libs/kv/welcome_screen.kv
--rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/gui/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/gui/popup.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/gui/the_naruno_gui_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.587879 naruno-0.60.1/naruno/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.587879 naruno-0.60.1/naruno/lib/backup/
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/lib/backup/naruno_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/lib/backup/naruno_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/lib/clean_up.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/lib/config_system.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/lib/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/lib/export.py
--rw-r--r--   0 runner    (1001) docker     (123)    25920 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/lib/kot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/lib/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.587879 naruno-0.60.1/naruno/lib/mix/
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/lib/mix/merkle_root.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/lib/mix/mixlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/lib/notification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.587879 naruno-0.60.1/naruno/lib/performance_analyzers/
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/lib/performance_analyzers/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/lib/performance_analyzers/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/lib/performance_analyzers/blockshash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/lib/performance_analyzers/blockshash_part.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/lib/performance_analyzers/heartbeat_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/lib/performance_analyzers/transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/lib/perpetualtimer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/lib/qr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/lib/safety.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/lib/settings_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/lib/sign.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/lib/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/lib/verify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.587879 naruno-0.60.1/naruno/logs/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/logs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.587879 naruno-0.60.1/naruno/node/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.587879 naruno-0.60.1/naruno/node/client/
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/node/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6206 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/node/get_candidate_blocks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.587879 naruno-0.60.1/naruno/node/server/
--rw-r--r--   0 runner    (1001) docker     (123)    33899 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/node/server/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/node/unl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.591879 naruno-0.60.1/naruno/transactions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.591879 naruno-0.60.1/naruno/transactions/check/
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/transactions/check/check_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.591879 naruno-0.60.1/naruno/transactions/check/datas/
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/transactions/check/datas/check_datas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.591879 naruno-0.60.1/naruno/transactions/check/len/
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/transactions/check/len/check_len.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.591879 naruno-0.60.1/naruno/transactions/check/sign/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/transactions/check/sign/check_sign.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.591879 naruno-0.60.1/naruno/transactions/check/type/
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/transactions/check/type/check_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/transactions/cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/transactions/get_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.591879 naruno-0.60.1/naruno/transactions/my_transactions/
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/transactions/my_transactions/check_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/transactions/my_transactions/get_my_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/transactions/my_transactions/get_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/transactions/my_transactions/save_my_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/transactions/my_transactions/save_to_my_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/transactions/my_transactions/sended_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/transactions/my_transactions/validate_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.591879 naruno-0.60.1/naruno/transactions/pending/
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/transactions/pending/delete_pending.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/transactions/pending/get_pending.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/transactions/pending/save_pending.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/transactions/pending_to_validating.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/transactions/print_transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/transactions/process_the_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/transactions/send.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/transactions/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.591879 naruno-0.60.1/naruno/wallet/
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/wallet/delete_current_wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.591879 naruno-0.60.1/naruno/wallet/ellipticcurve/
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/wallet/ellipticcurve/curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/wallet/ellipticcurve/ecdsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/wallet/ellipticcurve/math.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/wallet/ellipticcurve/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/wallet/ellipticcurve/privateKey.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/wallet/ellipticcurve/publicKey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/wallet/ellipticcurve/signature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.595879 naruno-0.60.1/naruno/wallet/ellipticcurve/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/wallet/ellipticcurve/utils/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/wallet/ellipticcurve/utils/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/wallet/ellipticcurve/utils/der.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/wallet/ellipticcurve/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/wallet/ellipticcurve/utils/integer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/wallet/ellipticcurve/utils/oid.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/wallet/ellipticcurve/utils/pem.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/wallet/get_saved_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/wallet/print_wallets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/wallet/save_wallet_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/wallet/wallet_create.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/wallet/wallet_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/wallet/wallet_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-29 00:28:12.000000 naruno-0.60.1/naruno/wallet/wallet_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 00:28:26.567879 naruno-0.60.1/naruno.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-07-29 00:28:26.000000 naruno-0.60.1/naruno.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-07-29 00:28:26.000000 naruno-0.60.1/naruno.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 00:28:26.000000 naruno-0.60.1/naruno.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-29 00:28:26.000000 naruno-0.60.1/naruno.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-29 00:28:26.000000 naruno-0.60.1/naruno.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 00:28:26.595879 naruno-0.60.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-29 00:28:12.000000 naruno-0.60.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.588044 naruno-0.60.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-08-01 14:28:12.000000 naruno-0.60.2/LICENCE-naruno-gui_lib__.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-01 14:28:12.000000 naruno-0.60.2/LICENCE-naruno-lib-kot__.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-01 14:28:12.000000 naruno-0.60.2/LICENCE-naruno-lib-mix__.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-01 14:28:12.000000 naruno-0.60.2/LICENCE-naruno-wallet-elipticcurve__.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-08-01 14:28:12.000000 naruno-0.60.2/LICENSE-others__.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 14:28:12.000000 naruno-0.60.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-08-01 14:28:23.588044 naruno-0.60.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-08-01 14:28:12.000000 naruno-0.60.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.564043 naruno-0.60.2/naruno/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.568043 naruno-0.60.2/naruno/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/accounts/account.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.568043 naruno-0.60.2/naruno/accounts/commanders/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/accounts/commanders/delete_commander.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/accounts/commanders/get_comnder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/accounts/commanders/save_commander.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/accounts/get_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/accounts/get_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/accounts/get_sequence_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/accounts/save_accounts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.568043 naruno-0.60.2/naruno/api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.568043 naruno-0.60.2/naruno/api/buildozer/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/api/buildozer/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25816 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/api/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.568043 naruno-0.60.2/naruno/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/apps/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29947 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/apps/remote_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.560043 naruno-0.60.2/naruno/blockchain/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.568043 naruno-0.60.2/naruno/blockchain/block/
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/blockchain/block/block_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/blockchain/block/blocks_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/blockchain/block/change_transaction_fee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/blockchain/block/create_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/blockchain/block/get_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/blockchain/block/get_block_from_blockchain_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/blockchain/block/get_minumum_transfer_amount.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.568043 naruno-0.60.2/naruno/blockchain/block/hash/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/blockchain/block/hash/accounts_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/blockchain/block/hash/blocks_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/blockchain/block/hash/calculate_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/blockchain/block/hash/tx_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/blockchain/block/just_one_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/blockchain/block/max_data_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/blockchain/block/max_tx_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/blockchain/block/save_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/blockchain/block/save_block_to_blockchain_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/blockchain/block/shares.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.568043 naruno-0.60.2/naruno/blockchain/candidate_block/
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/blockchain/candidate_block/candidate_block_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.568043 naruno-0.60.2/naruno/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)    18299 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.568043 naruno-0.60.2/naruno/consensus/
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/consensus_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.568043 naruno-0.60.2/naruno/consensus/finished/
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/finished/finished_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.568043 naruno-0.60.2/naruno/consensus/finished/transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/finished/transactions/transactions_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.568043 naruno-0.60.2/naruno/consensus/finished/true_time/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/finished/true_time/true_time_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.568043 naruno-0.60.2/naruno/consensus/ongoing/
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/ongoing/ongoing_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.560043 naruno-0.60.2/naruno/consensus/rounds/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.568043 naruno-0.60.2/naruno/consensus/rounds/round_1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.568043 naruno-0.60.2/naruno/consensus/rounds/round_1/checks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/consensus/rounds/round_1/checks/candidate_blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/rounds/round_1/checks/candidate_blocks/candidate_blocks_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/rounds/round_1/checks/checks_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.560043 naruno-0.60.2/naruno/consensus/rounds/round_1/checks/time/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/consensus/rounds/round_1/checks/time/time_difference/
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/rounds/round_1/checks/time/time_difference/time_difference_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/consensus/rounds/round_1/process/
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/rounds/round_1/process/process_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/consensus/rounds/round_1/process/transactions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/consensus/rounds/round_1/process/transactions/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/rounds/round_1/process/transactions/checks/duplicated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/consensus/rounds/round_1/process/transactions/find_newly/
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/rounds/round_1/process/transactions/find_newly/find_newly_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/consensus/rounds/round_1/process/transactions/find_validated/
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/rounds/round_1/process/transactions/find_validated/find_validated_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/rounds/round_1/process/transactions/transactions_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/rounds/round_1/round_1_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/consensus/rounds/round_2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/consensus/rounds/round_2/checks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/candidate_blocks_hashes_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/rounds/round_2/checks/checks_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.560043 naruno-0.60.2/naruno/consensus/rounds/round_2/checks/time/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/consensus/rounds/round_2/checks/time/time_difference/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/rounds/round_2/checks/time/time_difference/time_difference_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/consensus/rounds/round_2/process/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/candidate_blocks_hashes_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/rounds/round_2/process/process_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/consensus/rounds/round_2/process/rescue/
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/rounds/round_2/process/rescue/rescue_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/consensus/rounds/round_2/process/validate/
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/rounds/round_2/process/validate/validate_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/rounds/round_2/round_2_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/consensus/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/sync/send_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/sync/send_block_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/consensus/sync/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/blocks/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/commanders/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/commanders/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/connected_nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/connected_nodes/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/connected_nodes_test_0/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/connected_nodes_test_0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/connected_nodes_test_1/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/connected_nodes_test_1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/connected_nodes_test_2/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/connected_nodes_test_2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/extracted_proofs/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/extracted_proofs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/my_transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/my_transactions/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/pending_transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/pending_transactions/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/pending_transactions_test_0/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/pending_transactions_test_0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/pending_transactions_test_1/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/pending_transactions_test_1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/pending_transactions_test_2/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/pending_transactions_test_2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/proof/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/proof/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/qrs/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/qrs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/remote_app_cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/remote_app_cache/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/signs/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/signs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB_not_our_transaction/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB_not_our_transaction/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/test_consensus_trigger_finished/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/test_consensus_trigger_finished/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/test_finished_main/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/test_finished_main/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/test_finished_main_2/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/test_finished_main_2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.572043 naruno-0.60.2/naruno/db/test_finished_main_3/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/test_finished_main_3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.576043 naruno-0.60.2/naruno/db/test_finished_main_false_time/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/test_finished_main_false_time/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.576043 naruno-0.60.2/naruno/db/test_finished_main_no_reset/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/test_finished_main_no_reset/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.576043 naruno-0.60.2/naruno/db/test_proof_extracted/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/db/test_proof_extracted/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.576043 naruno-0.60.2/naruno/gui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.564043 naruno-0.60.2/naruno/gui/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.580044 naruno-0.60.2/naruno/gui/lib/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/fonts/POPPINS_LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)   151396 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/fonts/Poppins-Black.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   171604 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/fonts/Poppins-BlackItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   153944 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/fonts/Poppins-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   176588 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/fonts/Poppins-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   152764 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/fonts/Poppins-ExtraBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   173916 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/fonts/Poppins-ExtraBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   161456 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/fonts/Poppins-ExtraLight.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   186168 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/fonts/Poppins-ExtraLightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   182012 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/fonts/Poppins-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   159892 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/fonts/Poppins-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   184460 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/fonts/Poppins-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   156520 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/fonts/Poppins-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   180444 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/fonts/Poppins-MediumItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   158240 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/fonts/Poppins-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   155232 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/fonts/Poppins-SemiBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   178584 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/fonts/Poppins-SemiBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   161652 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/fonts/Poppins-Thin.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   187044 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/fonts/Poppins-ThinItalic.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.580044 naruno-0.60.2/naruno/gui/lib/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   254014 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/images/logo.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    19780 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16238 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/images/logo_sm_orb_fw.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21468 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/images/logo_w_bc.png
+-rw-r--r--   0 runner    (1001) docker     (123)   254014 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/images/logo_win.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.564043 naruno-0.60.2/naruno/gui/lib/libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.580044 naruno-0.60.2/naruno/gui/lib/libs/baseclass/
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/libs/baseclass/node_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/libs/baseclass/operations_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/libs/baseclass/root_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/libs/baseclass/settings_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/libs/baseclass/tabnavigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/libs/baseclass/wallet_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/libs/baseclass/welcome_screen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.584044 naruno-0.60.2/naruno/gui/lib/libs/kv/
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/libs/kv/node_screen.kv
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/libs/kv/operations_screen.kv
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/libs/kv/root_screen.kv
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/libs/kv/settings_screen.kv
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/libs/kv/tabnavigation.kv
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/libs/kv/wallet_screen.kv
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/lib/libs/kv/welcome_screen.kv
+-rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/popup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/gui/the_naruno_gui_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.584044 naruno-0.60.2/naruno/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.584044 naruno-0.60.2/naruno/lib/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/backup/naruno_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/backup/naruno_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/clean_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/config_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26004 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/kot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.584044 naruno-0.60.2/naruno/lib/mix/
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/mix/merkle_root.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/mix/mixlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/notification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.584044 naruno-0.60.2/naruno/lib/performance_analyzers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/performance_analyzers/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/performance_analyzers/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/performance_analyzers/blockshash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/performance_analyzers/blockshash_part.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/performance_analyzers/heartbeat_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/performance_analyzers/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/perpetualtimer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/qr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/safety.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/settings_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/lib/verify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.584044 naruno-0.60.2/naruno/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/logs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.584044 naruno-0.60.2/naruno/node/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.584044 naruno-0.60.2/naruno/node/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/node/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/node/get_candidate_blocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.584044 naruno-0.60.2/naruno/node/server/
+-rw-r--r--   0 runner    (1001) docker     (123)    33899 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/node/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/node/unl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.584044 naruno-0.60.2/naruno/transactions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.584044 naruno-0.60.2/naruno/transactions/check/
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/check/check_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.584044 naruno-0.60.2/naruno/transactions/check/datas/
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/check/datas/check_datas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.584044 naruno-0.60.2/naruno/transactions/check/len/
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/check/len/check_len.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.584044 naruno-0.60.2/naruno/transactions/check/sign/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/check/sign/check_sign.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.588044 naruno-0.60.2/naruno/transactions/check/type/
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/check/type/check_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/get_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.588044 naruno-0.60.2/naruno/transactions/my_transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/my_transactions/check_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/my_transactions/get_my_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/my_transactions/get_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/my_transactions/save_my_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/my_transactions/save_to_my_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/my_transactions/sended_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/my_transactions/validate_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.588044 naruno-0.60.2/naruno/transactions/pending/
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/pending/delete_pending.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/pending/get_pending.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/pending/save_pending.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/pending_to_validating.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/print_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/process_the_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/send.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/transactions/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.588044 naruno-0.60.2/naruno/wallet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/delete_current_wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.588044 naruno-0.60.2/naruno/wallet/ellipticcurve/
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/ellipticcurve/curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/ellipticcurve/ecdsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/ellipticcurve/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/ellipticcurve/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/ellipticcurve/privateKey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/ellipticcurve/publicKey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/ellipticcurve/signature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.588044 naruno-0.60.2/naruno/wallet/ellipticcurve/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/ellipticcurve/utils/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/ellipticcurve/utils/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/ellipticcurve/utils/der.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/ellipticcurve/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/ellipticcurve/utils/integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/ellipticcurve/utils/oid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/ellipticcurve/utils/pem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/get_saved_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/print_wallets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/save_wallet_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/wallet_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/wallet_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/wallet_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-08-01 14:28:12.000000 naruno-0.60.2/naruno/wallet/wallet_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:23.568043 naruno-0.60.2/naruno.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-08-01 14:28:23.000000 naruno-0.60.2/naruno.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-08-01 14:28:23.000000 naruno-0.60.2/naruno.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:28:23.000000 naruno-0.60.2/naruno.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-01 14:28:23.000000 naruno-0.60.2/naruno.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-01 14:28:23.000000 naruno-0.60.2/naruno.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 14:28:23.588044 naruno-0.60.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-08-01 14:28:12.000000 naruno-0.60.2/setup.py
```

### Comparing `naruno-0.60.1/LICENCE-naruno-gui_lib__.md` & `naruno-0.60.2/LICENCE-naruno-gui_lib__.md`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/LICENCE-naruno-lib-kot__.md` & `naruno-0.60.2/LICENCE-naruno-lib-kot__.md`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/LICENCE-naruno-lib-mix__.md` & `naruno-0.60.2/LICENCE-naruno-lib-mix__.md`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/LICENCE-naruno-wallet-elipticcurve__.md` & `naruno-0.60.2/LICENCE-naruno-wallet-elipticcurve__.md`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/LICENSE-others__.md` & `naruno-0.60.2/LICENSE-others__.md`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/PKG-INFO` & `naruno-0.60.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naruno
-Version: 0.60.1
+Version: 0.60.2
 Summary: Naruno is a lightning-fast, secure, and scalable blockchain that is able to create transaction proofs and verification via raw data and timestamp. We remove the archive nodes and lazy web3 integrations. With Naruno everyone can get the proof (5-10MB) of their transactions via their nodes and after everyone can use in another node for verification the raw data and timestamp. Also you can integrate your web3 applications with 4 code lines (just python for now) via our remote app system.
 Home-page: https://github.com/Naruno/Naruno
 Author: Naruno Developers
 Author-email: onur.atakan.ulusoy@naruno.org
 License: MPL-2.0
 Description: <p align="center">
           <a href="https://github.com/Naruno/Naruno">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: naruno Version: 0.60.1 Summary: Naruno is a
+Metadata-Version: 2.1 Name: naruno Version: 0.60.2 Summary: Naruno is a
 lightning-fast, secure, and scalable blockchain that is able to create
 transaction proofs and verification via raw data and timestamp. We remove the
 archive nodes and lazy web3 integrations. With Naruno everyone can get the
 proof (5-10MB) of their transactions via their nodes and after everyone can use
 in another node for verification the raw data and timestamp. Also you can
 integrate your web3 applications with 4 code lines (just python for now) via
 our remote app system. Home-page: https://github.com/Naruno/Naruno Author:
```

### Comparing `naruno-0.60.1/README.md` & `naruno-0.60.2/README.md`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/accounts/account.py` & `naruno-0.60.2/naruno/accounts/account.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/accounts/commanders/delete_commander.py` & `naruno-0.60.2/naruno/accounts/commanders/delete_commander.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/accounts/commanders/get_comnder.py` & `naruno-0.60.2/naruno/accounts/commanders/get_comnder.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/accounts/commanders/save_commander.py` & `naruno-0.60.2/naruno/accounts/commanders/save_commander.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/accounts/get_accounts.py` & `naruno-0.60.2/naruno/accounts/get_accounts.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/accounts/get_balance.py` & `naruno-0.60.2/naruno/accounts/get_balance.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/accounts/get_sequence_number.py` & `naruno-0.60.2/naruno/accounts/get_sequence_number.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/accounts/save_accounts.py` & `naruno-0.60.2/naruno/accounts/save_accounts.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/api/buildozer/main.py` & `naruno-0.60.2/naruno/api/buildozer/main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/api/main.py` & `naruno-0.60.2/naruno/api/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,17 +16,18 @@
 from flask import request
 from waitress import serve
 from waitress.server import create_server
 
 sys.path.append(os.path.join(os.path.dirname(__file__), "..", ".."))
 
 from flask_cors import CORS
-from naruno.blockchain.block.block_main import Block
+
 from naruno.accounts.get_balance import GetBalance
 from naruno.accounts.get_sequence_number import GetSequanceNumber
+from naruno.blockchain.block.block_main import Block
 from naruno.blockchain.block.create_block import CreateBlock
 from naruno.blockchain.block.get_block import GetBlock
 from naruno.blockchain.block.just_one_tx import GetJustOneTX
 from naruno.blockchain.block.max_data_size import GetMaxDataSize
 from naruno.blockchain.block.max_tx_number import GetMaxTXNumber
 from naruno.blockchain.block.save_block import SaveBlock
 from naruno.consensus.consensus_main import consensus_trigger
@@ -192,19 +193,18 @@
                     custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH,
                     custom_TEMP_ACCOUNTS_PATH=custom_TEMP_ACCOUNTS_PATH,
                     custom_TEMP_BLOCKSHASH_PATH=custom_TEMP_BLOCKSHASH_PATH,
                     custom_TEMP_BLOCKSHASH_PART_PATH=
                     custom_TEMP_BLOCKSHASH_PART_PATH,
                 )
             result = send_tx.dump_json()
-  
+
     except:
         traceback.print_exc()
 
-
     return jsonify(result)
 
 
 @app.route("/wallet/balance", methods=["GET"])
 def balance_wallets_page():
     logger.debug(
         f"{request.remote_addr} {request.method} {request.url} {request.data}")
@@ -353,40 +353,41 @@
             {"error": "You can't turn off the debug mode in publisher mode."})
     app.config["DEBUG"] = False
     ft_mode_settings(False)
     return jsonify("OK")
 
 
 def block_get_page_proccess(the_server):
-        the_block = CreateBlock(custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH)
-        SaveBlock(
-            the_block,
-            custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH,
-            custom_TEMP_ACCOUNTS_PATH=custom_TEMP_ACCOUNTS_PATH,
-            custom_TEMP_BLOCKSHASH_PATH=custom_TEMP_BLOCKSHASH_PATH,
-            custom_TEMP_BLOCKSHASH_PART_PATH=custom_TEMP_BLOCKSHASH_PART_PATH,
-        )
-        the_server.send_block_to_other_nodes()
-        the_consensus_trigger = (consensus_trigger if custom_consensus_trigger
-                                 is None else custom_consensus_trigger)
-        trigger = perpetualTimer(the_block.consensus_timer,
-                                 the_consensus_trigger, the_consensus=True)
-        global custom_consensus_trigger_result
-        custom_consensus_trigger_result = trigger
+    the_block = CreateBlock(custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH)
+    SaveBlock(
+        the_block,
+        custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH,
+        custom_TEMP_ACCOUNTS_PATH=custom_TEMP_ACCOUNTS_PATH,
+        custom_TEMP_BLOCKSHASH_PATH=custom_TEMP_BLOCKSHASH_PATH,
+        custom_TEMP_BLOCKSHASH_PART_PATH=custom_TEMP_BLOCKSHASH_PART_PATH,
+    )
+    the_server.send_block_to_other_nodes()
+    the_consensus_trigger = (consensus_trigger if custom_consensus_trigger
+                             is None else custom_consensus_trigger)
+    trigger = perpetualTimer(the_block.consensus_timer,
+                             the_consensus_trigger,
+                             the_consensus=True)
+    global custom_consensus_trigger_result
+    custom_consensus_trigger_result = trigger
 
 
 @app.route("/block/get", methods=["GET"])
 def block_get_page():
     logger.debug(
         f"{request.remote_addr} {request.method} {request.url} {request.data}")
     if the_settings()["publisher_mode"]:
         return jsonify({"error": "You can't get the block in publisher mode."})
     the_server = server.Server if custom_server is None else custom_server
     if the_settings()["test_mode"]:
-        block_get_page_proccess(the_server,)
+        block_get_page_proccess(the_server, )
     else:
         the_server.send_me_full_block()
     return jsonify("OK")
 
 
 @app.route("/export/transactions/csv", methods=["GET"])
 def export_transaction_csv_page():
@@ -537,42 +538,48 @@
 def balance_get_page():
     logger.debug(
         f"{request.remote_addr} {request.method} {request.url} {request.data}")
     # Check publisher mode
     if not the_settings()["publisher_mode"]:
         return jsonify("403"), 403
     address = str(request.args.get("address"))
-    the_block = Block("API")
+    block = None
+    with contextlib.suppress(Exception):
+        block = (GetBlock(custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH)
+                 if custom_block is None else custom_block)
 
     return jsonify(
         GetBalance(
             address,
-            block=the_block,
+            block=block,
             account_list=custom_account_list,
             dont_convert=True,
         ))
 
 
 @app.route("/sequence/get/", methods=["GET"])
 def sequence_get_page():
     logger.debug(
         f"{request.remote_addr} {request.method} {request.url} {request.data}")
     # Check publisher mode
     if not the_settings()["publisher_mode"]:
         return jsonify("403"), 403
     address = str(request.args.get("address"))
 
-    the_block = Block("API")
+    block = None
+    with contextlib.suppress(Exception):
+        block = (GetBlock(custom_TEMP_BLOCK_PATH=custom_TEMP_BLOCK_PATH)
+                 if custom_block is None else custom_block)
 
     return jsonify(
         GetSequanceNumber(
             address,
             account_list=custom_account_list,
             dont_convert=True,
-            block=the_block,
+            block=block,
         ))
 
 
 # Write a api for directing a transaction with GetTransaction
 @app.route("/transaction/send/", methods=["POST"])
 def transaction_send_page():
     logger.debug(
```

### Comparing `naruno-0.60.1/naruno/apps/checker.py` & `naruno-0.60.2/naruno/apps/checker.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/apps/remote_app.py` & `naruno-0.60.2/naruno/apps/remote_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 import math
 import os
 import random
 import string
 import sys
 import threading
 import time
-from hashlib import sha256
 import traceback
+from hashlib import sha256
 
 import requests
 
 from naruno.accounts.commanders.delete_commander import DeleteCommander
 from naruno.accounts.commanders.get_comnder import GetCommander
 from naruno.accounts.commanders.save_commander import SaveCommander
 from naruno.api.main import start
@@ -65,14 +65,15 @@
         sended=False,
         sended_not_validated=False,
         cache_true=True,
         wait_amount=None,
         checking=True,
         commander=None,
         total_check=None,
+        wait_amount_between_multiple_sendings=10,
     ):
         """
         :param host: The host of the node
         :param port: The port of the node
         :param password: The password of the wallet
         """
         self.app_name = app_name
@@ -104,18 +105,20 @@
         self.last_sended = 0
 
         self.sending_wait_time = 10
 
         a_block = Block("Onur")
 
         if wait_amount is None:
-            self.wait_amount = a_block.block_time * 2
+            self.wait_amount = a_block.block_time * 4
         else:
             self.wait_amount = wait_amount
 
+        self.wait_amount_between_multiple_sendings = wait_amount_between_multiple_sendings
+
         self.get_cache()
 
         self.sended_txs = []
 
         self.checking = checking
 
         self.commander = commander
@@ -150,15 +153,15 @@
                 self.total_check = False if "true" in self.total_check else True
 
             self.original_wait_amoount = copy.copy(self.wait_amount)
 
             self.check_thread = (perpetualTimer(
                 self.original_wait_amoount, checker,
                 (self, )) if self.total_check else self.check_thread)
-            self.wait_amount = 0 if self.total_check else self.wait_amount
+            self.wait_amount = (self.wait_amount_between_multiple_sendings if self.total_check else self.wait_amount)
             success = True
         except:
             traceback.print_exc()
 
         logger.error("Network is not active") if not success else None
         self.close() if not success else None
         sys.exit() if not success else None
@@ -228,20 +231,18 @@
                 self.cache.remove(each_cache)
 
     def save_cache(self):
         if self.cache_true == False:
             self.get_cache()
             return
 
-
         self.backward_support_cache()
 
         self.integrationcache_db.set("cache", self.cache)
 
-
     def delete_cache(self):
         self.integrationcache_db.delete("cache")
 
     def prepare_request(self, end_point, type, data=None) -> requests.Response:
         """
         :param end_point: The end point of the request
         :param type: The type of the request (get, post)
@@ -372,68 +373,69 @@
 
         system_length = len(
             json.dumps({
                 "action": self.app_name + action,
                 "app_data": ""
             }))
 
-        true_length = (self.max_data_size / self.max_tx_number -
+        true_length = (self.max_data_size * 0.8 / self.max_tx_number -
                        system_length) - 10
 
         if len(app_data) > true_length:
             self.send_splitter(
                 action,
                 app_data,
                 to_user,
                 system_length,
                 true_length,
                 force=force,
                 retrysecond=retrysecond,
             )
+        else:
 
-        data = json.dumps(data)
+            data = json.dumps(data)
 
-        request_body = {
-            "password": self.password,
-            "to_user": to_user,
-            "data": data,
-        }
-
-        alread_in_sended = False
-        for tx in self.sended_txs:
-            if (tx[0] == action and tx[1] == app_data and tx[2] == to_user
-                    and tx[3] == amount and tx[4] == force
-                    and tx[5] == retrysecond and tx[6] == data):
-                alread_in_sended = True
-        if not alread_in_sended:
-            self.sended_txs.append(
-                [action, app_data, to_user, amount, force, retrysecond, data])
-
-        if amount is not None:
-            request_body["amount"] = amount
-
-        response = self.prepare_request("/send/",
-                                        type="post",
-                                        data=request_body)
-
-        if "false" in response.text:
-            logger.error("Error on sending message")
-            if force:
-                logger.info("Trying to send again")
-                return self.send_forcer(action, app_data, to_user, retrysecond)
-            return False
-        else:
-            logger.info(
-                f"Message sent: app_name:{self.app_name} action:{action} data: {data} to: {to_user}"
-            )
-            time.sleep(1)
-            self.last_sended = time.time()
-            if self.checking and self.check_thread is None:
-                checker(self)
-            return True
+            request_body = {
+                "password": self.password,
+                "to_user": to_user,
+                "data": data,
+            }
+
+            alread_in_sended = False
+            for tx in self.sended_txs:
+                if (tx[0] == action and tx[1] == app_data and tx[2] == to_user
+                        and tx[3] == amount and tx[4] == force
+                        and tx[5] == retrysecond and tx[6] == data):
+                    alread_in_sended = True
+            if not alread_in_sended:
+                self.sended_txs.append(
+                    [action, app_data, to_user, amount, force, retrysecond, data])
+
+            if amount is not None:
+                request_body["amount"] = amount
+
+            response = self.prepare_request("/send/",
+                                            type="post",
+                                            data=request_body)
+
+            if "false" in response.text:
+                logger.error("Error on sending message")
+                if force:
+                    logger.info("Trying to send again")
+                    return self.send_forcer(action, app_data, to_user, retrysecond)
+                return False
+            else:
+                logger.info(
+                    f"Message sent: app_name:{self.app_name} action:{action} data: {data} to: {to_user}"
+                )
+                time.sleep(1)
+                self.last_sended = time.time()
+                if self.checking and self.check_thread is None:
+                    checker(self)
+                return True
 
     def get_(
         self,
         get_all,
         disable_caches,
         disable_sended_not_validated,
         force_sended,
```

### Comparing `naruno-0.60.1/naruno/blockchain/block/block_main.py` & `naruno-0.60.2/naruno/blockchain/block/block_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/blockchain/block/blocks_hash.py` & `naruno-0.60.2/naruno/blockchain/block/blocks_hash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/blockchain/block/change_transaction_fee.py` & `naruno-0.60.2/naruno/blockchain/block/change_transaction_fee.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/blockchain/block/create_block.py` & `naruno-0.60.2/naruno/blockchain/block/create_block.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/blockchain/block/get_block.py` & `naruno-0.60.2/naruno/blockchain/block/get_block.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/blockchain/block/get_block_from_blockchain_db.py` & `naruno-0.60.2/naruno/blockchain/block/get_block_from_blockchain_db.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/blockchain/block/get_minumum_transfer_amount.py` & `naruno-0.60.2/naruno/blockchain/block/get_minumum_transfer_amount.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/blockchain/block/hash/accounts_hash.py` & `naruno-0.60.2/naruno/blockchain/block/hash/accounts_hash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/blockchain/block/hash/blocks_hash.py` & `naruno-0.60.2/naruno/blockchain/block/hash/blocks_hash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/blockchain/block/hash/calculate_hash.py` & `naruno-0.60.2/naruno/blockchain/block/hash/calculate_hash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/blockchain/block/hash/tx_hash.py` & `naruno-0.60.2/naruno/blockchain/block/hash/tx_hash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/blockchain/block/just_one_tx.py` & `naruno-0.60.2/naruno/blockchain/block/just_one_tx.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/blockchain/block/max_data_size.py` & `naruno-0.60.2/naruno/blockchain/block/max_data_size.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/blockchain/block/max_tx_number.py` & `naruno-0.60.2/naruno/blockchain/block/max_tx_number.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/blockchain/block/save_block.py` & `naruno-0.60.2/naruno/blockchain/block/save_block.py`

 * *Files 0% similar despite different names*

```diff
@@ -308,15 +308,16 @@
     "e7b72ca5af68bc5b8ddd98e4187c68efcfbec5cd",
 ]
 
 specials = ["e087a455c3b35d5022491b380e3e34d68df4ca6c"]
 
 special_testers = [
     "d78101e2cb261efab28ee54a0e6d716820a1bab1",
-    "40a175793d9b7082157fd3e1632fc25c9f3f5234"
+    "40a175793d9b7082157fd3e1632fc25c9f3f5234",
+    "9febe30ed21991fdca2e84d1a42d594c1a02ab36"
     ]
 
 
 def SaveBlock(
     block: Block,
     custom_TEMP_BLOCK_PATH=None,
     custom_TEMP_ACCOUNTS_PATH=None,
```

### Comparing `naruno-0.60.1/naruno/blockchain/block/save_block_to_blockchain_db.py` & `naruno-0.60.2/naruno/blockchain/block/save_block_to_blockchain_db.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/blockchain/block/shares.py` & `naruno-0.60.2/naruno/blockchain/block/shares.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/blockchain/candidate_block/candidate_block_main.py` & `naruno-0.60.2/naruno/blockchain/candidate_block/candidate_block_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/cli/main.py` & `naruno-0.60.2/naruno/cli/main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/config.py` & `naruno-0.60.2/naruno/config.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/consensus/consensus_main.py` & `naruno-0.60.2/naruno/consensus/consensus_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/consensus/finished/finished_main.py` & `naruno-0.60.2/naruno/consensus/finished/finished_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/consensus/finished/transactions/transactions_main.py` & `naruno-0.60.2/naruno/consensus/finished/transactions/transactions_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/consensus/finished/true_time/true_time_main.py` & `naruno-0.60.2/naruno/consensus/finished/true_time/true_time_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/consensus/ongoing/ongoing_main.py` & `naruno-0.60.2/naruno/consensus/ongoing/ongoing_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/consensus/rounds/round_1/checks/candidate_blocks/candidate_blocks_main.py` & `naruno-0.60.2/naruno/consensus/rounds/round_1/checks/candidate_blocks/candidate_blocks_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/consensus/rounds/round_1/checks/checks_main.py` & `naruno-0.60.2/naruno/consensus/rounds/round_1/checks/checks_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/consensus/rounds/round_1/checks/time/time_difference/time_difference_main.py` & `naruno-0.60.2/naruno/consensus/rounds/round_1/checks/time/time_difference/time_difference_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/consensus/rounds/round_1/process/process_main.py` & `naruno-0.60.2/naruno/consensus/rounds/round_1/process/process_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/consensus/rounds/round_1/process/transactions/checks/duplicated.py` & `naruno-0.60.2/naruno/consensus/rounds/round_1/process/transactions/checks/duplicated.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/consensus/rounds/round_1/process/transactions/find_newly/find_newly_main.py` & `naruno-0.60.2/naruno/consensus/rounds/round_1/process/transactions/find_newly/find_newly_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/consensus/rounds/round_1/process/transactions/find_validated/find_validated_main.py` & `naruno-0.60.2/naruno/consensus/rounds/round_1/process/transactions/find_validated/find_validated_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/consensus/rounds/round_1/process/transactions/transactions_main.py` & `naruno-0.60.2/naruno/consensus/rounds/round_1/process/transactions/transactions_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/consensus/rounds/round_1/round_1_main.py` & `naruno-0.60.2/naruno/consensus/rounds/round_1/round_1_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/candidate_blocks_hashes_main.py` & `naruno-0.60.2/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/candidate_blocks_hashes_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/consensus/rounds/round_2/checks/checks_main.py` & `naruno-0.60.2/naruno/consensus/rounds/round_2/checks/checks_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/consensus/rounds/round_2/checks/time/time_difference/time_difference_main.py` & `naruno-0.60.2/naruno/consensus/rounds/round_2/checks/time/time_difference/time_difference_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/candidate_blocks_hashes_main.py` & `naruno-0.60.2/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/candidate_blocks_hashes_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/consensus/rounds/round_2/process/process_main.py` & `naruno-0.60.2/naruno/consensus/rounds/round_2/process/process_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/consensus/rounds/round_2/process/rescue/rescue_main.py` & `naruno-0.60.2/naruno/consensus/rounds/round_2/process/rescue/rescue_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/consensus/rounds/round_2/process/validate/validate_main.py` & `naruno-0.60.2/naruno/consensus/rounds/round_2/process/validate/validate_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/consensus/rounds/round_2/round_2_main.py` & `naruno-0.60.2/naruno/consensus/rounds/round_2/round_2_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/consensus/sync/send_block.py` & `naruno-0.60.2/naruno/consensus/sync/send_block.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/consensus/sync/send_block_hash.py` & `naruno-0.60.2/naruno/consensus/sync/send_block_hash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/consensus/sync/sync.py` & `naruno-0.60.2/naruno/consensus/sync/sync.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/gui/lib/fonts/POPPINS_LICENCE` & `naruno-0.60.2/naruno/gui/lib/fonts/POPPINS_LICENCE`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/gui/lib/fonts/Poppins-Black.ttf` & `naruno-0.60.2/naruno/gui/lib/fonts/Poppins-Black.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/gui/lib/fonts/Poppins-BlackItalic.ttf` & `naruno-0.60.2/naruno/gui/lib/fonts/Poppins-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/gui/lib/fonts/Poppins-Bold.ttf` & `naruno-0.60.2/naruno/gui/lib/fonts/Poppins-Bold.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/gui/lib/fonts/Poppins-BoldItalic.ttf` & `naruno-0.60.2/naruno/gui/lib/fonts/Poppins-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/gui/lib/fonts/Poppins-ExtraBold.ttf` & `naruno-0.60.2/naruno/gui/lib/fonts/Poppins-ExtraBold.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/gui/lib/fonts/Poppins-ExtraBoldItalic.ttf` & `naruno-0.60.2/naruno/gui/lib/fonts/Poppins-ExtraBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/gui/lib/fonts/Poppins-ExtraLight.ttf` & `naruno-0.60.2/naruno/gui/lib/fonts/Poppins-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/gui/lib/fonts/Poppins-ExtraLightItalic.ttf` & `naruno-0.60.2/naruno/gui/lib/fonts/Poppins-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/gui/lib/fonts/Poppins-Italic.ttf` & `naruno-0.60.2/naruno/gui/lib/fonts/Poppins-Italic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/gui/lib/fonts/Poppins-Light.ttf` & `naruno-0.60.2/naruno/gui/lib/fonts/Poppins-Light.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/gui/lib/fonts/Poppins-LightItalic.ttf` & `naruno-0.60.2/naruno/gui/lib/fonts/Poppins-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/gui/lib/fonts/Poppins-Medium.ttf` & `naruno-0.60.2/naruno/gui/lib/fonts/Poppins-Medium.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/gui/lib/fonts/Poppins-MediumItalic.ttf` & `naruno-0.60.2/naruno/gui/lib/fonts/Poppins-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/gui/lib/fonts/Poppins-Regular.ttf` & `naruno-0.60.2/naruno/gui/lib/fonts/Poppins-Regular.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/gui/lib/fonts/Poppins-SemiBold.ttf` & `naruno-0.60.2/naruno/gui/lib/fonts/Poppins-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/gui/lib/fonts/Poppins-SemiBoldItalic.ttf` & `naruno-0.60.2/naruno/gui/lib/fonts/Poppins-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/gui/lib/fonts/Poppins-Thin.ttf` & `naruno-0.60.2/naruno/gui/lib/fonts/Poppins-Thin.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/gui/lib/fonts/Poppins-ThinItalic.ttf` & `naruno-0.60.2/naruno/gui/lib/fonts/Poppins-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/gui/lib/images/logo.ico` & `naruno-0.60.2/naruno/gui/lib/images/logo.ico`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/gui/lib/images/logo.png` & `naruno-0.60.2/naruno/gui/lib/images/logo.png`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/gui/lib/images/logo_sm_orb_fw.png` & `naruno-0.60.2/naruno/gui/lib/images/logo_sm_orb_fw.png`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/gui/lib/images/logo_w_bc.png` & `naruno-0.60.2/naruno/gui/lib/images/logo_w_bc.png`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/gui/lib/images/logo_win.ico` & `naruno-0.60.2/naruno/gui/lib/images/logo_win.ico`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/gui/lib/libs/baseclass/node_screen.py` & `naruno-0.60.2/naruno/gui/lib/libs/baseclass/node_screen.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/gui/lib/libs/baseclass/operations_screen.py` & `naruno-0.60.2/naruno/gui/lib/libs/baseclass/operations_screen.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/gui/lib/libs/baseclass/root_screen.py` & `naruno-0.60.2/naruno/gui/lib/libs/baseclass/root_screen.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/gui/lib/libs/baseclass/settings_screen.py` & `naruno-0.60.2/naruno/gui/lib/libs/baseclass/settings_screen.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/gui/lib/libs/baseclass/tabnavigation.py` & `naruno-0.60.2/naruno/gui/lib/libs/baseclass/tabnavigation.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/gui/lib/libs/baseclass/wallet_screen.py` & `naruno-0.60.2/naruno/gui/lib/libs/baseclass/wallet_screen.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/gui/lib/libs/baseclass/welcome_screen.py` & `naruno-0.60.2/naruno/gui/lib/libs/baseclass/welcome_screen.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/gui/lib/libs/kv/node_screen.kv` & `naruno-0.60.2/naruno/gui/lib/libs/kv/node_screen.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/gui/lib/libs/kv/operations_screen.kv` & `naruno-0.60.2/naruno/gui/lib/libs/kv/operations_screen.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/gui/lib/libs/kv/root_screen.kv` & `naruno-0.60.2/naruno/gui/lib/libs/kv/root_screen.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/gui/lib/libs/kv/settings_screen.kv` & `naruno-0.60.2/naruno/gui/lib/libs/kv/settings_screen.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/gui/lib/libs/kv/tabnavigation.kv` & `naruno-0.60.2/naruno/gui/lib/libs/kv/tabnavigation.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/gui/lib/libs/kv/wallet_screen.kv` & `naruno-0.60.2/naruno/gui/lib/libs/kv/wallet_screen.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/gui/lib/libs/kv/welcome_screen.kv` & `naruno-0.60.2/naruno/gui/lib/libs/kv/welcome_screen.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/gui/main.py` & `naruno-0.60.2/naruno/gui/main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/gui/popup.py` & `naruno-0.60.2/naruno/gui/popup.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/lib/backup/naruno_export.py` & `naruno-0.60.2/naruno/lib/backup/naruno_export.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/lib/backup/naruno_import.py` & `naruno-0.60.2/naruno/lib/backup/naruno_import.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/lib/clean_up.py` & `naruno-0.60.2/naruno/lib/clean_up.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/lib/config_system.py` & `naruno-0.60.2/naruno/lib/config_system.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/lib/encryption.py` & `naruno-0.60.2/naruno/lib/encryption.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/lib/export.py` & `naruno-0.60.2/naruno/lib/export.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/lib/kot.py` & `naruno-0.60.2/naruno/lib/kot.py`

 * *Files 1% similar despite different names*

```diff
@@ -664,22 +664,23 @@
         return True
 
     def dict(self, encryption_key: str = "", no_data: bool = False):
         encryption_key = force_encrypt if force_encrypt != False else encryption_key
         result = {}
         for key in os.listdir(self.location):
             if not "." in key:
-                the_key = self.get_key(key)
-                if not the_key is None:
-                    if the_key != False:
-                        result_of_key = (self.get(
-                            the_key, encryption_key=encryption_key)
-                                         if not no_data else True)
-                        if not result_of_key is None:
-                            result[the_key] = result_of_key
+                with contextlib.suppress(Exception):
+                    the_key = self.get_key(key)
+                    if not the_key is None:
+                        if the_key != False:
+                            result_of_key = (self.get(
+                                the_key, encryption_key=encryption_key)
+                                            if not no_data else True)
+                            if not result_of_key is None:
+                                result[the_key] = result_of_key
         return result
 
     def size_all(self) -> int:
         # Calculate self.location size
         total_size = 0
 
         for dirpath, dirnames, filenames in os.walk(self.location):
```

### Comparing `naruno-0.60.1/naruno/lib/log.py` & `naruno-0.60.2/naruno/lib/log.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/lib/mix/merkle_root.py` & `naruno-0.60.2/naruno/lib/mix/merkle_root.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/lib/mix/mixlib.py` & `naruno-0.60.2/naruno/lib/mix/mixlib.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/lib/notification.py` & `naruno-0.60.2/naruno/lib/notification.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/lib/performance_analyzers/accounts.py` & `naruno-0.60.2/naruno/lib/performance_analyzers/accounts.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/lib/performance_analyzers/block.py` & `naruno-0.60.2/naruno/lib/performance_analyzers/block.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/lib/performance_analyzers/blockshash.py` & `naruno-0.60.2/naruno/lib/performance_analyzers/blockshash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/lib/performance_analyzers/blockshash_part.py` & `naruno-0.60.2/naruno/lib/performance_analyzers/blockshash_part.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/lib/performance_analyzers/heartbeat_db.py` & `naruno-0.60.2/naruno/lib/performance_analyzers/heartbeat_db.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/lib/performance_analyzers/transactions.py` & `naruno-0.60.2/naruno/lib/performance_analyzers/transactions.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/lib/perpetualtimer.py` & `naruno-0.60.2/naruno/lib/perpetualtimer.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/lib/qr.py` & `naruno-0.60.2/naruno/lib/qr.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/lib/safety.py` & `naruno-0.60.2/naruno/lib/safety.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/lib/settings_system.py` & `naruno-0.60.2/naruno/lib/settings_system.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/lib/sign.py` & `naruno-0.60.2/naruno/lib/sign.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/lib/status.py` & `naruno-0.60.2/naruno/lib/status.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/lib/verify.py` & `naruno-0.60.2/naruno/lib/verify.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/node/client/client.py` & `naruno-0.60.2/naruno/node/client/client.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/node/get_candidate_blocks.py` & `naruno-0.60.2/naruno/node/get_candidate_blocks.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,41 +33,51 @@
                 will_add_candidate_block = naruno.node.get_candidate_blocks.our_candidates[0]
                 will_add_candidate_block_hash = naruno.node.get_candidate_blocks.our_candidates[1]
             
             first_validating = [i.dump_json() for i in the_block.validating_list]
             second_validating = [i.dump_json() for i in block.validating_list]
             if not block.round_1 or will_add_candidate_block is None:
                 if block.sequence_number+block.empty_block_number > the_block.sequence_number+the_block.empty_block_number or block.sequence_number == 0 or reset or will_add_candidate_block is None:
+
+                    the_block = copy.copy(block)
                     will_add_candidate_block = {
                                 "action": "myblock",
                                 "transaction": new_list,
                                 "signature": a_time,
-                                "sequence_number": block.sequence_number+block.empty_block_number,
+                                "sequence_number": the_block.sequence_number+the_block.empty_block_number,
                                 "total_length": len(new_list)
                             }
-                    the_block = copy.copy(block)
+
             if (block.round_1 and not block.round_2)  or block.sequence_number == 0 or will_add_candidate_block_hash is None:
                 if block.sequence_number+block.empty_block_number > the_block_2.sequence_number+the_block_2.empty_block_number or block.sequence_number == 0 or reset or will_add_candidate_block_hash is None:
-                    will_add_candidate_block_hash = {
-                                "action":
-                                "myblockhash",
-                                "hash":
-                                block.hash,
-                                "previous_hash":
-                                block.previous_hash,
-                                "signature":
-                                a_time,
-                                "sequence_number":
-                                block.sequence_number+block.empty_block_number,
-                            }
-                    
-                    the_block_2 = copy.copy(block)
+                    last_control = True
+                    if block.sequence_number != 0:
+                        if block.hash == None:
+                            last_control = False
+            
+
+                    if last_control:
+
+                        the_block_2 = copy.copy(block)
                     
+                        will_add_candidate_block_hash = {
+                                    "action":
+                                    "myblockhash",
+                                    "hash":
+                                    the_block_2.hash,
+                                    "previous_hash":
+                                    the_block_2.previous_hash,
+                                    "signature":
+                                    a_time,
+                                    "sequence_number":
+                                    the_block_2.sequence_number+the_block_2.empty_block_number,
+                                }
                 
-                
+
+
             
             naruno.node.get_candidate_blocks.our_candidates = [will_add_candidate_block, will_add_candidate_block_hash, the_block, the_block_2]
             
 
             return [the_block, the_block_2]
```

### Comparing `naruno-0.60.1/naruno/node/server/server.py` & `naruno-0.60.2/naruno/node/server/server.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/node/unl.py` & `naruno-0.60.2/naruno/node/unl.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/transactions/check/check_transaction.py` & `naruno-0.60.2/naruno/transactions/check/check_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/transactions/check/datas/check_datas.py` & `naruno-0.60.2/naruno/transactions/check/datas/check_datas.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/transactions/check/len/check_len.py` & `naruno-0.60.2/naruno/transactions/check/len/check_len.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/transactions/check/sign/check_sign.py` & `naruno-0.60.2/naruno/transactions/check/sign/check_sign.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/transactions/check/type/check_type.py` & `naruno-0.60.2/naruno/transactions/check/type/check_type.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/transactions/cleaner.py` & `naruno-0.60.2/naruno/transactions/cleaner.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/transactions/get_transaction.py` & `naruno-0.60.2/naruno/transactions/get_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/transactions/my_transactions/check_proof.py` & `naruno-0.60.2/naruno/transactions/my_transactions/check_proof.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/transactions/my_transactions/get_my_transaction.py` & `naruno-0.60.2/naruno/transactions/my_transactions/get_my_transaction.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,76 +1,76 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 import contextlib
+import copy
 import json
 import os
 import traceback
 from urllib.request import urlopen
-import copy
 
 from naruno.lib.config_system import get_config
 from naruno.lib.kot import KOT
 from naruno.lib.settings_system import the_settings
-
 from naruno.transactions.transaction import Transaction
+import naruno
 
 mytransactions_db = KOT("mytransactions",
                         folder=get_config()["main_folder"] + "/db")
 
-
 mytransactions_db_ram = {}
 
 
 def check_from_network():
     """
     Checks if the transaction is in the network.
     """
     validated_transactions = []
     if the_settings()["baklava"]:
- 
-            # export validated transactions
-            response = (urlopen(
-                "http://test_net.1.naruno.org:8000/transactions/received").
-                        read().decode("utf-8"))
-            response = json.loads(response)
-            for transaction in response:
-                if response[transaction]["validated"]:
-                    validated_transactions.append(transaction)
-
+        # export validated transactions
+        response = (
+            urlopen("http://test_net.1.naruno.org:8000/transactions/received"
+                    ).read().decode("utf-8"))
+        response = json.loads(response)
+        for transaction in response:
+            if response[transaction]["validated"]:
+                validated_transactions.append(transaction)
 
     return validated_transactions
 
 
 def GetMyTransaction(sended=None, validated=None, turn_json=False) -> list:
     """
     Returns the transaction db.
     """
     network_validated_source = check_from_network()
 
-
     network_validated = []
 
     the_transactions = []
 
-    all_records = mytransactions_db.get_all() if mytransactions_db_ram == {} else mytransactions_db_ram
+    if len(naruno.transactions.my_transactions.get_my_transaction.mytransactions_db_ram) != mytransactions_db.get_count():
+        naruno.transactions.my_transactions.get_my_transaction.mytransactions_db_ram = {}
+
+    all_records = (mytransactions_db.get_all()
+                   if naruno.transactions.my_transactions.get_my_transaction.mytransactions_db_ram == {} else naruno.transactions.my_transactions.get_my_transaction.mytransactions_db_ram)
     for entry in copy.copy(all_records):
         if not entry.endswith("validated") and not entry.endswith("sended"):
             try:
                 the_transactions_json = all_records[entry]
                 the_tx = Transaction.load_json(the_transactions_json)
                 each_validated = (False if mytransactions_db.get(entry +
                                                                  "validated")
                                   == None else True)
 
-                if (the_transactions_json["signature"] in network_validated_source
-                        and not each_validated):
+                if (the_transactions_json["signature"]
+                        in network_validated_source and not each_validated):
                     each_validated = True
                     network_validated.append(the_tx)
 
                 each_sended = (False if mytransactions_db.get(entry + "sended")
                                == None else True)
                 the_transactions.append([
                     the_tx,
@@ -89,24 +89,26 @@
         the_transactions = [
             tx for tx in the_transactions if tx[1] == validated
         ]
 
     # sort
     the_transactions.sort(key=lambda x: x[0].signature)
 
-    from naruno.transactions.my_transactions.validate_transaction import ValidateTransaction
+    from naruno.transactions.my_transactions.validate_transaction import \
+        ValidateTransaction
+
     for i in network_validated:
-        ValidateTransaction(i, custom_currently_list=the_transactions, force_notify=True)
-  
+        ValidateTransaction(i,
+                            custom_currently_list=the_transactions,
+                            force_notify=True)
+
     if turn_json:
         the_transactions = {
             tx[0].signature: {
                 "transaction": tx[0].dump_json(),
                 "validated": tx[1],
                 "sended": tx[2],
             }
             for tx in the_transactions
         }
 
-
-
     return the_transactions
```

### Comparing `naruno-0.60.1/naruno/transactions/my_transactions/get_proof.py` & `naruno-0.60.2/naruno/transactions/my_transactions/get_proof.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/transactions/my_transactions/save_my_transaction.py` & `naruno-0.60.2/naruno/transactions/my_transactions/save_my_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/transactions/my_transactions/save_to_my_transaction.py` & `naruno-0.60.2/naruno/transactions/my_transactions/save_to_my_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/transactions/my_transactions/sended_transaction.py` & `naruno-0.60.2/naruno/transactions/my_transactions/sended_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/transactions/my_transactions/validate_transaction.py` & `naruno-0.60.2/naruno/transactions/my_transactions/validate_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/transactions/pending/delete_pending.py` & `naruno-0.60.2/naruno/transactions/pending/delete_pending.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/transactions/pending/get_pending.py` & `naruno-0.60.2/naruno/transactions/pending/get_pending.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/transactions/pending/save_pending.py` & `naruno-0.60.2/naruno/transactions/pending/save_pending.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/transactions/pending_to_validating.py` & `naruno-0.60.2/naruno/transactions/pending_to_validating.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/transactions/print_transactions.py` & `naruno-0.60.2/naruno/transactions/print_transactions.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/transactions/process_the_transaction.py` & `naruno-0.60.2/naruno/transactions/process_the_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/transactions/send.py` & `naruno-0.60.2/naruno/transactions/send.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/transactions/transaction.py` & `naruno-0.60.2/naruno/transactions/transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/wallet/delete_current_wallet.py` & `naruno-0.60.2/naruno/wallet/delete_current_wallet.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/wallet/ellipticcurve/curve.py` & `naruno-0.60.2/naruno/wallet/ellipticcurve/curve.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/wallet/ellipticcurve/ecdsa.py` & `naruno-0.60.2/naruno/wallet/ellipticcurve/ecdsa.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/wallet/ellipticcurve/math.py` & `naruno-0.60.2/naruno/wallet/ellipticcurve/math.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/wallet/ellipticcurve/privateKey.py` & `naruno-0.60.2/naruno/wallet/ellipticcurve/privateKey.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/wallet/ellipticcurve/publicKey.py` & `naruno-0.60.2/naruno/wallet/ellipticcurve/publicKey.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/wallet/ellipticcurve/signature.py` & `naruno-0.60.2/naruno/wallet/ellipticcurve/signature.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/wallet/ellipticcurve/utils/binary.py` & `naruno-0.60.2/naruno/wallet/ellipticcurve/utils/binary.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/wallet/ellipticcurve/utils/compatibility.py` & `naruno-0.60.2/naruno/wallet/ellipticcurve/utils/compatibility.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/wallet/ellipticcurve/utils/der.py` & `naruno-0.60.2/naruno/wallet/ellipticcurve/utils/der.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/wallet/ellipticcurve/utils/oid.py` & `naruno-0.60.2/naruno/wallet/ellipticcurve/utils/oid.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/wallet/get_saved_wallet.py` & `naruno-0.60.2/naruno/wallet/get_saved_wallet.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/wallet/print_wallets.py` & `naruno-0.60.2/naruno/wallet/print_wallets.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/wallet/save_wallet_list.py` & `naruno-0.60.2/naruno/wallet/save_wallet_list.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/wallet/wallet_create.py` & `naruno-0.60.2/naruno/wallet/wallet_create.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/wallet/wallet_delete.py` & `naruno-0.60.2/naruno/wallet/wallet_delete.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/wallet/wallet_import.py` & `naruno-0.60.2/naruno/wallet/wallet_import.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno/wallet/wallet_selector.py` & `naruno-0.60.2/naruno/wallet/wallet_selector.py`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/naruno.egg-info/PKG-INFO` & `naruno-0.60.2/naruno.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naruno
-Version: 0.60.1
+Version: 0.60.2
 Summary: Naruno is a lightning-fast, secure, and scalable blockchain that is able to create transaction proofs and verification via raw data and timestamp. We remove the archive nodes and lazy web3 integrations. With Naruno everyone can get the proof (5-10MB) of their transactions via their nodes and after everyone can use in another node for verification the raw data and timestamp. Also you can integrate your web3 applications with 4 code lines (just python for now) via our remote app system.
 Home-page: https://github.com/Naruno/Naruno
 Author: Naruno Developers
 Author-email: onur.atakan.ulusoy@naruno.org
 License: MPL-2.0
 Description: <p align="center">
           <a href="https://github.com/Naruno/Naruno">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: naruno Version: 0.60.1 Summary: Naruno is a
+Metadata-Version: 2.1 Name: naruno Version: 0.60.2 Summary: Naruno is a
 lightning-fast, secure, and scalable blockchain that is able to create
 transaction proofs and verification via raw data and timestamp. We remove the
 archive nodes and lazy web3 integrations. With Naruno everyone can get the
 proof (5-10MB) of their transactions via their nodes and after everyone can use
 in another node for verification the raw data and timestamp. Also you can
 integrate your web3 applications with 4 code lines (just python for now) via
 our remote app system. Home-page: https://github.com/Naruno/Naruno Author:
```

### Comparing `naruno-0.60.1/naruno.egg-info/SOURCES.txt` & `naruno-0.60.2/naruno.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `naruno-0.60.1/setup.py` & `naruno-0.60.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup
 
 setup(
     author="Naruno Developers",
     author_email="onur.atakan.ulusoy@naruno.org",
     packages=["naruno"],
     name="naruno",
-    version="0.60.1",
+    version="0.60.2",
     url="https://github.com/Naruno/Naruno",
     description=
     "Naruno is a lightning-fast, secure, and scalable blockchain that is able to create transaction proofs and verification via raw data and timestamp. We remove the archive nodes and lazy web3 integrations. With Naruno everyone can get the proof (5-10MB) of their transactions via their nodes and after everyone can use in another node for verification the raw data and timestamp. Also you can integrate your web3 applications with 4 code lines (just python for now) via our remote app system.",
     keywords=[
         "python",
         "cryptography",
         "blockchain",
```

