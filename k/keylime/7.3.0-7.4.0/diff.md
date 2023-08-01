# Comparing `tmp/keylime-7.3.0.tar.gz` & `tmp/keylime-7.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keylime-7.3.0.tar", last modified: Fri Jun 30 17:17:29 2023, max compression
+gzip compressed data, was "keylime-7.4.0.tar", last modified: Tue Aug  1 19:25:39 2023, max compression
```

## Comparing `keylime-7.3.0.tar` & `keylime-7.4.0.tar`

### file list

```diff
@@ -1,187 +1,187 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:29.163187 keylime-7.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-30 17:17:19.000000 keylime-7.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-30 17:17:19.000000 keylime-7.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12722 2023-06-30 17:17:29.163187 keylime-7.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-06-30 17:17:19.000000 keylime-7.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-30 17:17:19.000000 keylime-7.3.0/_pypi-notice.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:29.135187 keylime-7.3.0/keylime/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/agentstates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/api_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    45700 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/backport_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/ca_impl_openssl.py
--rw-r--r--   0 runner    (1001) docker     (123)    15559 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/ca_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/cert_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:29.135187 keylime-7.3.0/keylime/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/cli/policies.py
--rw-r--r--   0 runner    (1001) docker     (123)    12888 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/cloud_verifier_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    65012 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/cloud_verifier_tornado.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:29.139186 keylime-7.3.0/keylime/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/cmd/attest.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/cmd/ca.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20465 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/cmd/convert_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8890 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/cmd/convert_runtime_policy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22220 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/cmd/create_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/cmd/registrar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/cmd/sign_runtime_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/cmd/tenant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/cmd/user_data_encrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/cmd/verifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/cmd_exec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:29.139186 keylime-7.3.0/keylime/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/common/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/common/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/common/migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/common/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/common/states.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/common/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/common/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16220 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:29.139186 keylime-7.3.0/keylime/da/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/da/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/da/attest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:29.143187 keylime-7.3.0/keylime/da/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/da/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/da/examples/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/da/examples/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/da/examples/rekor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/da/examples/sqldb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/da/examples/tsa_rfc3161.py
--rw-r--r--   0 runner    (1001) docker     (123)    16781 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/da/record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:29.143187 keylime-7.3.0/keylime/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/db/keylime_db.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/db/registrar_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/db/verifier_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:29.143187 keylime-7.3.0/keylime/dsse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/dsse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/dsse/dsse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/dsse/ecdsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/dsse/x509.py
--rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/failure.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/fs_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:29.147187 keylime-7.3.0/keylime/ima/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/ima/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/ima/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/ima/dm_grammar.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18388 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/ima/file_signatures.py
--rw-r--r--   0 runner    (1001) docker     (123)    21055 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/ima/ima.py
--rw-r--r--   0 runner    (1001) docker     (123)    32160 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/ima/ima_dm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/ima/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/ip_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/keylime_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:29.147187 keylime-7.3.0/keylime/mba/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/mba/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:29.147187 keylime-7.3.0/keylime/mba/elchecking/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/mba/elchecking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/mba/elchecking/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17614 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/mba/elchecking/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/mba/elchecking/mbpolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/mba/elchecking/policies.py
--rw-r--r--   0 runner    (1001) docker     (123)    24300 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/mba/elchecking/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:29.147187 keylime-7.3.0/keylime/mba/elparsing/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/mba/elparsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/mba/elparsing/tpm2_tools_elparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/mba/elparsing/tpm_bootlog_enrich.py
--rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/mba/mba.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:29.147187 keylime-7.3.0/keylime/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:29.155187 keylime-7.3.0/keylime/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/039322ea079b_add_generator_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/1ac1513ef2a1_fix_mb_and_ima_column_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/257fe0f0c039_add_fields_for_revocation_context_to_.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/2fbc0fb8fa4d_add_checksum_to_allowlist.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/4089e1c79be9_add_tpm_clockinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/4329e2d14944_associate_moved_allowlists_to_agents.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/63c30820fdc1_add_mtls_cert_and_ak_to_verifier_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/7d5db1a6ffb0_add_agentstates_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/8a44a4364f5a_initial_database_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/8c0f8ded1f90_convert_allowlists_to_ima_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/8da20383f6e1_extend_ip_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/9169f80345ed_add_supported_version_to_verifiermain_.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/a09cc94177f0_add_last_received_quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/a72aec03d720_migrate_allowlists_to_separate_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/a79c27ec1054_add_mtls_cert_field_to_registrar.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/a7a64155ab3a_add_ima_filesigning_keys_column.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/ae898986c6e9_add_mb_refstate_column.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/b4d024197413_add_verfier_id_to_verifiermain_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/bc3b6b551b0a_drop_vtpm_colums.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/bf48e0c4751d_add_attestation_count_column.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/c3842cc9ee69_store_keyrings_learned_from_ima_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/cc2630851a1f_receive_the_aik_tpm_from_the_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/eb869a77abd1_create_allowlist_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/eeb702f77d7d_allowlist_rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/f35cdd35eb83_move_v_tpm_policy_to_jsonpickletype.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/f82c4252bc4f_add_ip_and_port_to_registrar.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/migrations/versions/f838d3cdeead_add_last_successful_attestation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/registrar_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20949 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/registrar_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/requests_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/revocation_notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/signing.py
--rw-r--r--   0 runner    (1001) docker     (123)    77727 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/tenant.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/tornado_requests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:29.159187 keylime-7.3.0/keylime/tpm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/tpm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/tpm/ec_crypto_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    16134 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/tpm/tpm2_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    18898 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/tpm/tpm2_objects_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18838 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/tpm/tpm_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    16468 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/tpm/tpm_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/tpm/tpm_util_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/tpm/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/tpm_ek_ca.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    17024 2023-06-30 17:17:19.000000 keylime-7.3.0/keylime/web_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:29.135187 keylime-7.3.0/keylime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12722 2023-06-30 17:17:29.000000 keylime-7.3.0/keylime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-06-30 17:17:29.000000 keylime-7.3.0/keylime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 17:17:29.000000 keylime-7.3.0/keylime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-30 17:17:29.000000 keylime-7.3.0/keylime.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 17:17:28.000000 keylime-7.3.0/keylime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 17:17:29.000000 keylime-7.3.0/keylime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-30 17:17:19.000000 keylime-7.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-30 17:17:29.163187 keylime-7.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-30 17:17:19.000000 keylime-7.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:29.127186 keylime-7.3.0/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:29.159187 keylime-7.3.0/templates/2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-06-30 17:17:19.000000 keylime-7.3.0/templates/2.0/adjust.py
--rw-r--r--   0 runner    (1001) docker     (123)     8390 2023-06-30 17:17:19.000000 keylime-7.3.0/templates/2.0/agent.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-30 17:17:19.000000 keylime-7.3.0/templates/2.0/ca.j2
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-30 17:17:19.000000 keylime-7.3.0/templates/2.0/logging.j2
--rw-r--r--   0 runner    (1001) docker     (123)    26824 2023-06-30 17:17:19.000000 keylime-7.3.0/templates/2.0/mapping.json
--rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-06-30 17:17:19.000000 keylime-7.3.0/templates/2.0/registrar.j2
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-06-30 17:17:19.000000 keylime-7.3.0/templates/2.0/tenant.j2
--rw-r--r--   0 runner    (1001) docker     (123)    11233 2023-06-30 17:17:19.000000 keylime-7.3.0/templates/2.0/verifier.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:17:29.163187 keylime-7.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_api_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_ca_impl_openssl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_ca_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_cert_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18107 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_convert_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_fs_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_ima_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)    23987 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_ima_dm.py
--rw-r--r--   0 runner    (1001) docker     (123)    20078 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_ima_verification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_mba_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_policy_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     7349 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_registrar_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_retry_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_signing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)    11601 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_verifier_db.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-30 17:17:19.000000 keylime-7.3.0/test/test_web_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:39.967908 keylime-7.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-01 19:25:30.000000 keylime-7.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-08-01 19:25:30.000000 keylime-7.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12722 2023-08-01 19:25:39.967908 keylime-7.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-08-01 19:25:30.000000 keylime-7.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-01 19:25:30.000000 keylime-7.4.0/_pypi-notice.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:39.951908 keylime-7.4.0/keylime/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/agentstates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/api_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45700 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/backport_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/ca_impl_openssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15559 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/ca_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/cert_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:39.951908 keylime-7.4.0/keylime/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/cli/policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12868 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/cloud_verifier_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65012 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/cloud_verifier_tornado.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:39.951908 keylime-7.4.0/keylime/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/cmd/attest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/cmd/ca.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20465 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/cmd/convert_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8890 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/cmd/convert_runtime_policy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22220 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/cmd/create_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/cmd/registrar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/cmd/sign_runtime_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/cmd/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/cmd/user_data_encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/cmd/verifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/cmd_exec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:39.955908 keylime-7.4.0/keylime/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/common/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/common/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/common/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/common/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/common/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/common/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/common/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16220 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:39.955908 keylime-7.4.0/keylime/da/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/da/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/da/attest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:39.955908 keylime-7.4.0/keylime/da/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/da/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/da/examples/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/da/examples/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/da/examples/rekor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/da/examples/sqldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/da/examples/tsa_rfc3161.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16951 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/da/record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:39.955908 keylime-7.4.0/keylime/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/db/keylime_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/db/registrar_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/db/verifier_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:39.955908 keylime-7.4.0/keylime/dsse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/dsse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/dsse/dsse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/dsse/ecdsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/dsse/x509.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/failure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/fs_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:39.955908 keylime-7.4.0/keylime/ima/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/ima/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/ima/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/ima/dm_grammar.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18388 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/ima/file_signatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21055 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/ima/ima.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32160 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/ima/ima_dm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/ima/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/ip_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/keylime_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:39.955908 keylime-7.4.0/keylime/mba/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/mba/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:39.959908 keylime-7.4.0/keylime/mba/elchecking/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/mba/elchecking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/mba/elchecking/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/mba/elchecking/elchecker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17614 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/mba/elchecking/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/mba/elchecking/policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24300 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/mba/elchecking/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:39.959908 keylime-7.4.0/keylime/mba/elparsing/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/mba/elparsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/mba/elparsing/tpm2_tools_elparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/mba/elparsing/tpm_bootlog_enrich.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/mba/mba.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:39.959908 keylime-7.4.0/keylime/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/migrations/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/migrations/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:39.963908 keylime-7.4.0/keylime/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/migrations/versions/039322ea079b_add_generator_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/migrations/versions/1ac1513ef2a1_fix_mb_and_ima_column_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/migrations/versions/257fe0f0c039_add_fields_for_revocation_context_to_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/migrations/versions/2fbc0fb8fa4d_add_checksum_to_allowlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/migrations/versions/4089e1c79be9_add_tpm_clockinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/migrations/versions/4329e2d14944_associate_moved_allowlists_to_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/migrations/versions/63c30820fdc1_add_mtls_cert_and_ak_to_verifier_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/migrations/versions/7d5db1a6ffb0_add_agentstates_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/migrations/versions/8a44a4364f5a_initial_database_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/migrations/versions/8c0f8ded1f90_convert_allowlists_to_ima_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/migrations/versions/8da20383f6e1_extend_ip_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/migrations/versions/9169f80345ed_add_supported_version_to_verifiermain_.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/migrations/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/migrations/versions/a09cc94177f0_add_last_received_quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/migrations/versions/a72aec03d720_migrate_allowlists_to_separate_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/migrations/versions/a79c27ec1054_add_mtls_cert_field_to_registrar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/migrations/versions/a7a64155ab3a_add_ima_filesigning_keys_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/migrations/versions/ae898986c6e9_add_mb_refstate_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/migrations/versions/b4d024197413_add_verfier_id_to_verifiermain_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/migrations/versions/bc3b6b551b0a_drop_vtpm_colums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/migrations/versions/bf48e0c4751d_add_attestation_count_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/migrations/versions/c3842cc9ee69_store_keyrings_learned_from_ima_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/migrations/versions/cc2630851a1f_receive_the_aik_tpm_from_the_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/migrations/versions/eb869a77abd1_create_allowlist_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/migrations/versions/eeb702f77d7d_allowlist_rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/migrations/versions/f35cdd35eb83_move_v_tpm_policy_to_jsonpickletype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/migrations/versions/f82c4252bc4f_add_ip_and_port_to_registrar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/migrations/versions/f838d3cdeead_add_last_successful_attestation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/registrar_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21763 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/registrar_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/requests_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/revocation_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/signing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78461 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/tornado_requests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:39.963908 keylime-7.4.0/keylime/tpm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/tpm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/tpm/ec_crypto_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16134 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/tpm/tpm2_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18898 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/tpm/tpm2_objects_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18466 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/tpm/tpm_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17864 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/tpm/tpm_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7735 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/tpm/tpm_util_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/tpm/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/tpm_ek_ca.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17024 2023-08-01 19:25:30.000000 keylime-7.4.0/keylime/web_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:39.951908 keylime-7.4.0/keylime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12722 2023-08-01 19:25:39.000000 keylime-7.4.0/keylime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-08-01 19:25:39.000000 keylime-7.4.0/keylime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 19:25:39.000000 keylime-7.4.0/keylime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-08-01 19:25:39.000000 keylime-7.4.0/keylime.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 19:25:39.000000 keylime-7.4.0/keylime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-01 19:25:39.000000 keylime-7.4.0/keylime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-08-01 19:25:30.000000 keylime-7.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-08-01 19:25:39.967908 keylime-7.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-08-01 19:25:30.000000 keylime-7.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:39.943908 keylime-7.4.0/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:39.963908 keylime-7.4.0/templates/2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-08-01 19:25:30.000000 keylime-7.4.0/templates/2.0/adjust.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8390 2023-08-01 19:25:30.000000 keylime-7.4.0/templates/2.0/agent.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-08-01 19:25:30.000000 keylime-7.4.0/templates/2.0/ca.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-08-01 19:25:30.000000 keylime-7.4.0/templates/2.0/logging.j2
+-rw-r--r--   0 runner    (1001) docker     (123)    26824 2023-08-01 19:25:30.000000 keylime-7.4.0/templates/2.0/mapping.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-08-01 19:25:30.000000 keylime-7.4.0/templates/2.0/registrar.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-08-01 19:25:30.000000 keylime-7.4.0/templates/2.0/tenant.j2
+-rw-r--r--   0 runner    (1001) docker     (123)    11233 2023-08-01 19:25:30.000000 keylime-7.4.0/templates/2.0/verifier.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:39.967908 keylime-7.4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-08-01 19:25:30.000000 keylime-7.4.0/test/test_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-08-01 19:25:30.000000 keylime-7.4.0/test/test_api_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-08-01 19:25:30.000000 keylime-7.4.0/test/test_ca_impl_openssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-08-01 19:25:30.000000 keylime-7.4.0/test/test_ca_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-08-01 19:25:30.000000 keylime-7.4.0/test/test_cert_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-08-01 19:25:30.000000 keylime-7.4.0/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18107 2023-08-01 19:25:30.000000 keylime-7.4.0/test/test_convert_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-08-01 19:25:30.000000 keylime-7.4.0/test/test_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-08-01 19:25:30.000000 keylime-7.4.0/test/test_fs_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-08-01 19:25:30.000000 keylime-7.4.0/test/test_ima_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23987 2023-08-01 19:25:30.000000 keylime-7.4.0/test/test_ima_dm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20078 2023-08-01 19:25:30.000000 keylime-7.4.0/test/test_ima_verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-08-01 19:25:30.000000 keylime-7.4.0/test/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-08-01 19:25:30.000000 keylime-7.4.0/test/test_mba_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-08-01 19:25:30.000000 keylime-7.4.0/test/test_policy_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7349 2023-08-01 19:25:30.000000 keylime-7.4.0/test/test_registrar_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-08-01 19:25:30.000000 keylime-7.4.0/test/test_retry_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-08-01 19:25:30.000000 keylime-7.4.0/test/test_signing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-08-01 19:25:30.000000 keylime-7.4.0/test/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11601 2023-08-01 19:25:30.000000 keylime-7.4.0/test/test_verifier_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-08-01 19:25:30.000000 keylime-7.4.0/test/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-08-01 19:25:30.000000 keylime-7.4.0/test/test_web_util.py
```

### Comparing `keylime-7.3.0/LICENSE` & `keylime-7.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/PKG-INFO` & `keylime-7.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keylime
-Version: 7.3.0
+Version: 7.4.0
 Summary: TPM-based key bootstrapping and system integrity measurement system for cloud
 Home-page: https://keylime.dev
 Author: Keylime Community
 Author-email: keylime@groups.io
 License: Apache-2.0
 Project-URL: Source, https://github.com/keylime/keylime
 Project-URL: Documentation, https://keylime.readthedocs.io/en/latest/
```

### Comparing `keylime-7.3.0/README.md` & `keylime-7.4.0/README.md`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/agentstates.py` & `keylime-7.4.0/keylime/agentstates.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/api_version.py` & `keylime-7.4.0/keylime/api_version.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/backport_dataclasses.py` & `keylime-7.4.0/keylime/backport_dataclasses.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/ca_impl_openssl.py` & `keylime-7.4.0/keylime/ca_impl_openssl.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/ca_util.py` & `keylime-7.4.0/keylime/ca_util.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/cert_utils.py` & `keylime-7.4.0/keylime/cert_utils.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/cli/options.py` & `keylime-7.4.0/keylime/cli/options.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/cli/policies.py` & `keylime-7.4.0/keylime/cli/policies.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
             tpm_policy["mask"] = hex(int(tpm_policy["mask"], 0) | (1 << _pcr))
 
         logger.info("TPM PCR Mask automatically modified is %s to include IMA/Event log PCRs", tpm_policy["mask"])
 
         if isinstance(args["mb_refstate"], str):
             if args["mb_refstate"] == "default":
                 args["mb_refstate"] = config.get("tenant", "mb_refstate")
-            mb_refstate_data = mba.load_policy_file(args["mb_refstate"])
+            mb_refstate_data = mba.policy_load(args["mb_refstate"])
         else:
             raise UserError("Invalid measured boot reference state (intended state) provided")
 
     # Set up measured boot (TPM event log) reference state
     if tpm_util.check_mask(tpm_policy["mask"], config.MEASUREDBOOT_PCRS[2]):
         # Process measured boot reference state
         mb_refstate = mb_refstate_data
```

### Comparing `keylime-7.3.0/keylime/cloud_verifier_common.py` & `keylime-7.4.0/keylime/cloud_verifier_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from keylime import config, crypto, json, keylime_logging
 from keylime.agentstates import AgentAttestState, AgentAttestStates, TPMClockInfo
 from keylime.common import algorithms
 from keylime.db.verifier_db import VerfierMain
 from keylime.failure import Component, Event, Failure
 from keylime.ima import file_signatures
 from keylime.ima.types import RuntimePolicyType
+from keylime.mba import mba
 from keylime.tpm import tpm_util
 from keylime.tpm.tpm_main import Tpm
 
 # setup logging
 logger = keylime_logging.init_logging("cloudverifier_common")
 
 GLOBAL_TPM_INSTANCE: Optional[Tpm] = None
@@ -255,16 +256,15 @@
     }
     return params
 
 
 def process_get_status(agent: VerfierMain) -> Dict[str, Any]:
     has_mb_refstate = 0
     try:
-        mb_refstate = json.loads(cast(str, agent.mb_refstate))
-        if mb_refstate and mb_refstate.keys():
+        if mba.policy_is_valid(cast(str, agent.mb_refstate)):
             has_mb_refstate = 1
     except Exception as e:
         logger.warning(
             'Non-fatal problem ocurred while attempting to evaluate agent %s attribute "mb_refstate" (%s). Will just consider the value of this attribute as empty',
             agent.agent_id,
             e.args,
         )
```

### Comparing `keylime-7.3.0/keylime/cloud_verifier_tornado.py` & `keylime-7.4.0/keylime/cloud_verifier_tornado.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/cmd/convert_config.py` & `keylime-7.4.0/keylime/cmd/convert_config.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/cmd/convert_runtime_policy.py` & `keylime-7.4.0/keylime/cmd/convert_runtime_policy.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/cmd/create_policy.py` & `keylime-7.4.0/keylime/cmd/create_policy.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/cmd/registrar.py` & `keylime-7.4.0/keylime/cmd/registrar.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/cmd/sign_runtime_policy.py` & `keylime-7.4.0/keylime/cmd/sign_runtime_policy.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/cmd/user_data_encrypt.py` & `keylime-7.4.0/keylime/cmd/user_data_encrypt.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/cmd/verifier.py` & `keylime-7.4.0/keylime/cmd/verifier.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,18 +6,16 @@
 
 
 def main() -> None:
     # if we are configured to auto-migrate the DB, check if there are any migrations to perform
     if config.has_option("verifier", "auto_migrate_db") and config.getboolean("verifier", "auto_migrate_db"):
         apply("cloud_verifier")
 
-    # Load explicitly the policy modules into Keylime for the verifier,
-    # so that they are not loaded accidentally from other components
-    mba.load_policy_engine()
-    mba.load_parser_engine()
+    # Explicitly load and initialize measured boot components
+    mba.load_imports()
     cloud_verifier_tornado.main()
 
 
 if __name__ == "__main__":
     try:
         main()
     except Exception as e:
```

### Comparing `keylime-7.3.0/keylime/cmd_exec.py` & `keylime-7.4.0/keylime/cmd_exec.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/common/algorithms.py` & `keylime-7.4.0/keylime/common/algorithms.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/common/migrations.py` & `keylime-7.4.0/keylime/common/migrations.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/common/states.py` & `keylime-7.4.0/keylime/common/states.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/common/validators.py` & `keylime-7.4.0/keylime/common/validators.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/common/version.py` & `keylime-7.4.0/keylime/common/version.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/config.py` & `keylime-7.4.0/keylime/config.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/crypto.py` & `keylime-7.4.0/keylime/crypto.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/da/attest.py` & `keylime-7.4.0/keylime/da/attest.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,15 @@
         dest="end_date",
         default="last",
         help='end date for attestation window in IS0 8601 format (e.g., "2008-09-03T21:56:35"), or keyworkd "last"',
     )
 
     args = parser.parse_args()
 
-    mba.load_policy_engine()
-    mba.load_parser_engine()
+    mba.load_imports()
 
     rmcb = config.get("registrar", "durable_attestation_import", fallback="")
     rmc = record.get_record_mgt_class(rmcb)
     if not rmc:
         return
 
     rmc = rmc("registrar")
```

### Comparing `keylime-7.3.0/keylime/da/examples/file.py` & `keylime-7.4.0/keylime/da/examples/file.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/da/examples/redis.py` & `keylime-7.4.0/keylime/da/examples/redis.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/da/examples/rekor.py` & `keylime-7.4.0/keylime/da/examples/rekor.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/da/examples/sqldb.py` & `keylime-7.4.0/keylime/da/examples/sqldb.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/da/examples/tsa_rfc3161.py` & `keylime-7.4.0/keylime/da/examples/tsa_rfc3161.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,28 +6,30 @@
 from keylime.da.record import RecordManagementException
 
 logger = keylime_logging.init_logging("durable_attestation_time_stamp_authority")
 
 
 def record_timestamp_create(record_object, agent_id, contents, tsa_url, tsa_cert):
     if tsa_url:
+        _certificate = None
         if tsa_cert:
             with open(tsa_cert, "rb") as fp:
                 _certificate = fp.read()
 
         _rt = rfc3161ng.RemoteTimestamper(tsa_url._replace(fragment="").geturl(), certificate=_certificate)
         _tst = _rt.timestamp(data=contents)
         if _rt.check(_tst, data=contents):
             record_object["signature_timestamp_response"] = base64.b64encode(_tst)
         else:
             raise RecordManagementException(f"Failure while timestamping data for agent {agent_id}")
 
 
 def record_timestamp_check(record_object, agent_id, contents, tsa_url, tsa_cert):
     if tsa_url:
+        _certificate = None
         if tsa_cert:
             with open(tsa_cert, "rb") as fp:
                 _certificate = fp.read()
 
         _rt = rfc3161ng.RemoteTimestamper(tsa_url, certificate=_certificate)
         _tst = base64.b64decode(record_object["signature_timestamp_response"])
         if not _rt.check(_tst, data=contents):
```

### Comparing `keylime-7.3.0/keylime/da/record.py` & `keylime-7.4.0/keylime/da/record.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,17 +82,20 @@
         """Serialize, and optionally encodes, record"""
 
         manipulated_record_object = copy.deepcopy(record_object)
 
         if self.rcd_fmt == "pickle":
             serialized_record_object = pickle.dumps(manipulated_record_object)
 
-        if self.rcd_fmt == "json":
+        elif self.rcd_fmt == "json":
             serialized_record_object = json.dumps(manipulated_record_object, indent=4).encode("utf-8")
 
+        else:
+            raise Exception("Unknown or unsupported record format")
+
         if self.rcd_enc == "base64":
             serialized_record_object = base64.b64encode(serialized_record_object)
 
         return serialized_record_object
 
     def record_deserialize(self, record_object: Union[Any, bytes]) -> Union[Any, Dict[Any, Any]]:
         """Deserialize, and optionally decodes, record"""
@@ -101,18 +104,21 @@
 
         if self.rcd_enc == "base64":
             manipulated_record_object = base64.b64decode(manipulated_record_object)
 
         if self.rcd_fmt == "pickle":
             deserialized_record_object = pickle.loads(manipulated_record_object)
 
-        if self.rcd_fmt == "json":
+        elif self.rcd_fmt == "json":
             deserialized_record_object = manipulated_record_object.decode("utf-8")
             deserialized_record_object = json.loads(deserialized_record_object)
 
+        else:
+            raise Exception("Unknown or unsupported record format")
+
         return deserialized_record_object
 
     def record_sanitize(self, record_object: Dict[Any, Any]) -> Dict[Any, Any]:
         """Removes a set of pre-defined key,pairs from record"""
 
         # copy.deepcopy fails at "ssl_context"
```

### Comparing `keylime-7.3.0/keylime/db/keylime_db.py` & `keylime-7.4.0/keylime/db/keylime_db.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/db/registrar_db.py` & `keylime-7.4.0/keylime/db/registrar_db.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/db/verifier_db.py` & `keylime-7.4.0/keylime/db/verifier_db.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/dsse/dsse.py` & `keylime-7.4.0/keylime/dsse/dsse.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/dsse/ecdsa.py` & `keylime-7.4.0/keylime/dsse/ecdsa.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/dsse/x509.py` & `keylime-7.4.0/keylime/dsse/x509.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/failure.py` & `keylime-7.4.0/keylime/failure.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/ima/ast.py` & `keylime-7.4.0/keylime/ima/ast.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/ima/dm_grammar.py` & `keylime-7.4.0/keylime/ima/dm_grammar.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/ima/file_signatures.py` & `keylime-7.4.0/keylime/ima/file_signatures.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/ima/ima.py` & `keylime-7.4.0/keylime/ima/ima.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/ima/ima_dm.py` & `keylime-7.4.0/keylime/ima/ima_dm.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/ima/types.py` & `keylime-7.4.0/keylime/ima/types.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/json.py` & `keylime-7.4.0/keylime/json.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/keylime_logging.py` & `keylime-7.4.0/keylime/keylime_logging.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/mba/elchecking/__main__.py` & `keylime-7.4.0/keylime/mba/elchecking/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import argparse
 import json
 import sys
 
+from keylime.mba import mba
 from keylime.mba.elparsing import tpm2_tools_elparser
 
 from . import policies
 
-policies.load_policies()
 # This main module is just for command-line based testing.
 # It implements a command to do one test.
 # Invoke it with `python3 -m $packagename`, for some value of
 # `$packagename` that works with your `$PYTHONPATH`.
 
 
 parser = argparse.ArgumentParser()
 parser.add_argument("policy_name", choices=policies.get_policy_names())
 parser.add_argument("refstate_file", type=argparse.FileType("rt"))
 parser.add_argument("eventlog_file", type=argparse.FileType("rb"), default=sys.stdin)
 args = parser.parse_args()
+mba.load_imports()
 policy = policies.get_policy(args.policy_name)
 if policy is None:
     print(
         f"Specified policy '{args.policy_name}' does not exist. Options are: {policies.get_policy_names()}.",
         file=sys.stderr,
     )
     sys.exit(1)
```

### Comparing `keylime-7.3.0/keylime/mba/elchecking/example.py` & `keylime-7.4.0/keylime/mba/elchecking/example.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/mba/elchecking/policies.py` & `keylime-7.4.0/keylime/mba/elchecking/policies.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 import abc
-import importlib
 import typing
 
-from keylime import config
-
 from . import tests
 
 # This module defines Policy for testing measured boot logs.
 # This module also implements a registry of policies and a few trivial
 # policies.
 
 # RefState is a succinct description of what is expected to be found
@@ -97,16 +94,7 @@
 
     Returns either:
     (a) an empty string to signal a good result or
     (b) a non-empty string identifying something wrong.
     """
     tester = refstate_to_test(policy_name, refstate)
     return tester.why_not({}, eventlog)
-
-
-def load_policies() -> None:
-    imports = config.getlist("verifier", "measured_boot_imports")
-    imports.append(".example")
-    if imports:
-        for imp in imports:
-            if imp:
-                importlib.import_module(imp, __package__)
```

### Comparing `keylime-7.3.0/keylime/mba/elchecking/tests.py` & `keylime-7.4.0/keylime/mba/elchecking/tests.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/mba/elparsing/tpm2_tools_elparser.py` & `keylime-7.4.0/keylime/mba/elparsing/tpm2_tools_elparser.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 import tempfile
 import typing
 from typing import Any, Dict, Optional
 
 from packaging.version import Version
 
 from keylime import cmd_exec, config, keylime_logging
-from keylime.common import algorithms
 from keylime.failure import Component, Failure
 
 if typing.TYPE_CHECKING:
     from keylime.mba.mba import MBAgg, MBLog, MBPCRDict
 
 logger = keylime_logging.init_logging("elparsing")
 
 
-def parse_bootlog(
-    mb_measurement_list: Optional[str], hash_alg: algorithms.Hash
+def bootlog_parse(
+    mb_measurement_list: Optional[str], hash_alg: str
 ) -> typing.Tuple["MBPCRDict", "MBAgg", "MBLog", Failure]:
-    """Parse the measured boot log and return its object and the state of the PCRs
+    """
+    Parse the measured boot log and return its object and the state of the PCRs
     :param mb_measurement_list: The measured boot measurement list
     :param hash_alg: the hash algorithm that should be used for the PCRs
     :returns: Returns a map of the state of the PCRs, measured boot data object and True for success
     and False in case an error occurred
     """
     failure = Failure(Component.MEASURED_BOOT, ["parser"])
     if mb_measurement_list:
@@ -35,19 +35,17 @@
             logger.error("Unable to parse measured boot event log. Check previous messages for a reason for error.")
             return {}, None, {}, failure
         log_pcrs = mb_measurement_data.get("pcrs")
         if not isinstance(log_pcrs, dict):
             logger.error("Parse of measured boot event log has unexpected value for .pcrs: %r", log_pcrs)
             failure.add_event("invalid_pcrs", {"got": log_pcrs}, True)
             return {}, None, {}, failure
-        pcr_hashes = log_pcrs.get(str(hash_alg))
+        pcr_hashes = log_pcrs.get(hash_alg)
         if (not isinstance(pcr_hashes, dict)) or not pcr_hashes:
-            logger.error(
-                "Parse of measured boot event log has unexpected value for .pcrs.%s: %r", str(hash_alg), pcr_hashes
-            )
+            logger.error("Parse of measured boot event log has unexpected value for .pcrs.%s: %r", hash_alg, pcr_hashes)
             failure.add_event("invalid_pcrs_hashes", {"got": pcr_hashes}, True)
             return {}, None, {}, failure
         boot_aggregates = mb_measurement_data.get("boot_aggregates")
         if (not isinstance(boot_aggregates, dict)) or not boot_aggregates:
             logger.error(
                 "Parse of measured boot event log has unexpected value for .boot_aggragtes: %r", boot_aggregates
             )
@@ -241,32 +239,33 @@
     if Version(tools_version[0]) >= Version("5.4") or (
         # Also mark first git version that introduces the change to the tpm2_eventlog format as 5.4
         # See: https://github.com/tpm2-software/tpm2-tools/commit/c78d258b2588aee535fd17594ad2f5e808056373
         Version(tools_version[0]) == Version("5.3")
         and len(tools_version) > 1
         and int(tools_version[1]) >= 24
     ):
-        logger.info("TPM2-TOOLS Version: %s", tools_version[0])
         _tpm2_tools_version = "5.4"
         return _tpm2_tools_version
     if Version(tools_version[0]) == Version("5.2"):
         # GA, MaS: experimentally found that version 5.2 of the tpm2_eventlog package produces output with
         # zero-terminated strings on both centos 9 and Ubuntu 22.04.
         # Adding a separate category for tpm2_tools_version so we can control whether strings are unescaped properly.
-        logger.info("TPM2-TOOLS Version: %s", tools_version[0])
         _tpm2_tools_version = "5.2"
         return _tpm2_tools_version
     if Version(tools_version[0]) >= Version("4.2"):
-        logger.info("TPM2-TOOLS Version: %s", tools_version[0])
         _tpm2_tools_version = "4.2"
         return _tpm2_tools_version
     if Version(tools_version[0]) >= Version("4.0.0"):
-        logger.info("TPM2-TOOLS Version: %s", tools_version[0])
         _tpm2_tools_version = "4.0"
         return _tpm2_tools_version
     if Version(tools_version[0]) >= Version("3.2.0"):
-        logger.info("TPM2-TOOLS Version: %s", tools_version[0])
         _tpm2_tools_version = "3.2"
         return _tpm2_tools_version
     logger.error("TPM2-TOOLS Version %s is not supported.", tools_version[0])
     _tpm2_tools_version = "unknown"
     return _tpm2_tools_version
+
+
+toolversion = tpm2_tools_getversion()
+if toolversion == "unknown":
+    raise ValueError("TPM2-TOOLS: version cannot be determined or unsupported")
+logger.debug("mba.elparser.tpm2_tools_elparser: TPM2-TOOLS %s detected.", toolversion)
```

### Comparing `keylime-7.3.0/keylime/mba/elparsing/tpm_bootlog_enrich.py` & `keylime-7.4.0/keylime/mba/elparsing/tpm_bootlog_enrich.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/migrations/alembic.ini` & `keylime-7.4.0/keylime/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/migrations/env.py` & `keylime-7.4.0/keylime/migrations/env.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/migrations/versions/039322ea079b_add_generator_column.py` & `keylime-7.4.0/keylime/migrations/versions/039322ea079b_add_generator_column.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/migrations/versions/1ac1513ef2a1_fix_mb_and_ima_column_types.py` & `keylime-7.4.0/keylime/migrations/versions/1ac1513ef2a1_fix_mb_and_ima_column_types.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/migrations/versions/257fe0f0c039_add_fields_for_revocation_context_to_.py` & `keylime-7.4.0/keylime/migrations/versions/257fe0f0c039_add_fields_for_revocation_context_to_.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/migrations/versions/2fbc0fb8fa4d_add_checksum_to_allowlist.py` & `keylime-7.4.0/keylime/migrations/versions/2fbc0fb8fa4d_add_checksum_to_allowlist.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/migrations/versions/4089e1c79be9_add_tpm_clockinfo.py` & `keylime-7.4.0/keylime/migrations/versions/4089e1c79be9_add_tpm_clockinfo.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/migrations/versions/4329e2d14944_associate_moved_allowlists_to_agents.py` & `keylime-7.4.0/keylime/migrations/versions/4329e2d14944_associate_moved_allowlists_to_agents.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/migrations/versions/63c30820fdc1_add_mtls_cert_and_ak_to_verifier_db.py` & `keylime-7.4.0/keylime/migrations/versions/63c30820fdc1_add_mtls_cert_and_ak_to_verifier_db.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/migrations/versions/7d5db1a6ffb0_add_agentstates_columns.py` & `keylime-7.4.0/keylime/migrations/versions/7d5db1a6ffb0_add_agentstates_columns.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/migrations/versions/8a44a4364f5a_initial_database_migration.py` & `keylime-7.4.0/keylime/migrations/versions/8a44a4364f5a_initial_database_migration.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/migrations/versions/8c0f8ded1f90_convert_allowlists_to_ima_policies.py` & `keylime-7.4.0/keylime/migrations/versions/8c0f8ded1f90_convert_allowlists_to_ima_policies.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/migrations/versions/8da20383f6e1_extend_ip_field.py` & `keylime-7.4.0/keylime/migrations/versions/8da20383f6e1_extend_ip_field.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/migrations/versions/9169f80345ed_add_supported_version_to_verifiermain_.py` & `keylime-7.4.0/keylime/migrations/versions/9169f80345ed_add_supported_version_to_verifiermain_.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/migrations/versions/a09cc94177f0_add_last_received_quote.py` & `keylime-7.4.0/keylime/migrations/versions/a09cc94177f0_add_last_received_quote.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/migrations/versions/a72aec03d720_migrate_allowlists_to_separate_table.py` & `keylime-7.4.0/keylime/migrations/versions/a72aec03d720_migrate_allowlists_to_separate_table.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/migrations/versions/a79c27ec1054_add_mtls_cert_field_to_registrar.py` & `keylime-7.4.0/keylime/migrations/versions/a79c27ec1054_add_mtls_cert_field_to_registrar.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/migrations/versions/a7a64155ab3a_add_ima_filesigning_keys_column.py` & `keylime-7.4.0/keylime/migrations/versions/a7a64155ab3a_add_ima_filesigning_keys_column.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/migrations/versions/ae898986c6e9_add_mb_refstate_column.py` & `keylime-7.4.0/keylime/migrations/versions/ae898986c6e9_add_mb_refstate_column.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/migrations/versions/b4d024197413_add_verfier_id_to_verifiermain_table.py` & `keylime-7.4.0/keylime/migrations/versions/b4d024197413_add_verfier_id_to_verifiermain_table.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/migrations/versions/bc3b6b551b0a_drop_vtpm_colums.py` & `keylime-7.4.0/keylime/migrations/versions/bc3b6b551b0a_drop_vtpm_colums.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/migrations/versions/bf48e0c4751d_add_attestation_count_column.py` & `keylime-7.4.0/keylime/migrations/versions/bf48e0c4751d_add_attestation_count_column.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/migrations/versions/c3842cc9ee69_store_keyrings_learned_from_ima_log.py` & `keylime-7.4.0/keylime/migrations/versions/c3842cc9ee69_store_keyrings_learned_from_ima_log.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/migrations/versions/cc2630851a1f_receive_the_aik_tpm_from_the_agent.py` & `keylime-7.4.0/keylime/migrations/versions/cc2630851a1f_receive_the_aik_tpm_from_the_agent.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/migrations/versions/eb869a77abd1_create_allowlist_table.py` & `keylime-7.4.0/keylime/migrations/versions/eb869a77abd1_create_allowlist_table.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/migrations/versions/eeb702f77d7d_allowlist_rename.py` & `keylime-7.4.0/keylime/migrations/versions/eeb702f77d7d_allowlist_rename.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/migrations/versions/f35cdd35eb83_move_v_tpm_policy_to_jsonpickletype.py` & `keylime-7.4.0/keylime/migrations/versions/f35cdd35eb83_move_v_tpm_policy_to_jsonpickletype.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/migrations/versions/f82c4252bc4f_add_ip_and_port_to_registrar.py` & `keylime-7.4.0/keylime/migrations/versions/f82c4252bc4f_add_ip_and_port_to_registrar.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/migrations/versions/f838d3cdeead_add_last_successful_attestation.py` & `keylime-7.4.0/keylime/migrations/versions/f838d3cdeead_add_last_successful_attestation.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/registrar_client.py` & `keylime-7.4.0/keylime/registrar_client.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/registrar_common.py` & `keylime-7.4.0/keylime/registrar_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import base64
 import http.server
 import ipaddress
 import os
+import select
 import signal
 import socket
+import ssl
 import sys
 import threading
 from http.server import BaseHTTPRequestHandler, HTTPServer
 from ipaddress import IPv6Address, ip_address
 from socketserver import ThreadingMixIn
 from typing import Any, Dict, Optional, Tuple, Union, cast
 
@@ -73,14 +75,33 @@
             logger.error("%s received an invalid agent ID: %s", method, agent_id)
             return None, None
 
         return rest_params, agent_id
 
 
 class ProtectedHandler(BaseHandler):
+    def handle(self) -> None:
+        """Need to perform SSL handshake here, as
+        do_handshake_on_connect=False for non-blocking SSL socket"""
+        while True:
+            try:
+                self.request.do_handshake()
+                break
+            except ssl.SSLWantReadError:
+                select.select([self.request], [], [])
+            except ssl.SSLWantWriteError:
+                select.select([], [self.request], [])
+            except ssl.SSLError as e:
+                logger.error("SSL connection error: %s", e)
+                return
+            except Exception as e:
+                logger.error("General communication failure: %s", e)
+                return
+        BaseHTTPRequestHandler.handle(self)
+
     def do_HEAD(self) -> None:
         """HEAD not supported"""
         web_util.echo_json_response(self, 405, "HEAD not supported")
 
     def do_PATCH(self) -> None:
         """PATCH not supported"""
         web_util.echo_json_response(self, 405, "PATCH not supported")
@@ -479,15 +500,17 @@
     except SQLAlchemyError as e:
         logger.error("SQLAlchemy Error: %s", e)
 
     # Set up the protected registrar server
     protected_server = RegistrarServer((host, tlsport), ProtectedHandler)
     context = web_util.init_mtls("registrar", logger=logger)
     if context is not None:
-        protected_server.socket = context.wrap_socket(protected_server.socket, server_side=True)
+        protected_server.socket = context.wrap_socket(
+            protected_server.socket, server_side=True, do_handshake_on_connect=False
+        )
     thread_protected_server = threading.Thread(target=protected_server.serve_forever)
 
     # Set up the unprotected registrar server
     unprotected_server = RegistrarServer((host, port), UnprotectedHandler)
     thread_unprotected_server = threading.Thread(target=unprotected_server.serve_forever)
 
     logger.info("Starting Cloud Registrar Server on ports %s and %s (TLS) use <Ctrl-C> to stop", port, tlsport)
```

### Comparing `keylime-7.3.0/keylime/requests_client.py` & `keylime-7.4.0/keylime/requests_client.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/revocation_notifier.py` & `keylime-7.4.0/keylime/revocation_notifier.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/signing.py` & `keylime-7.4.0/keylime/signing.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/tenant.py` & `keylime-7.4.0/keylime/tenant.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from keylime import api_version as keylime_api_version
 from keylime import ca_util, cert_utils, config, crypto, keylime_logging, registrar_client, signing, web_util
 from keylime.agentstates import AgentAttestState
 from keylime.cli import options, policies
 from keylime.cmd import user_data_encrypt
 from keylime.common import algorithms, retry, states, validators
 from keylime.ip_util import bracketize_ipv6
+from keylime.mba import mba
 from keylime.requests_client import RequestsClient
 from keylime.tpm import tpm2_objects, tpm_util
 from keylime.tpm.tpm_main import Tpm
 
 # setup logging
 logger = keylime_logging.init_logging("tenant")
 
@@ -152,14 +153,16 @@
                 cert, key, trusted_ca, key_password, verify_server_cert, is_client=True, logger=logger
             )
 
             logger.info("TLS is enabled.")
         else:
             logger.warning("TLS is disabled.")
 
+        mba.load_imports()
+
     @property
     def verifier_base_url(self) -> str:
         return f"{bracketize_ipv6(self.verifier_ip)}:{self.verifier_port}"
 
     def set_full_id_str(self) -> None:
         self.agent_fid_str = f"Agent {self.agent_uuid}"
         if self.agent_ip:
@@ -594,129 +597,120 @@
         json_message = json.dumps(data)
         do_cv = RequestsClient(self.verifier_base_url, True, tls_context=self.tls_context)
         response = do_cv.post(
             (f"/v{self.api_version}/agents/{self.agent_uuid}"), data=json_message, timeout=self.request_timeout
         )
 
         if response.status_code == 503:
-            logger.error(
-                "Cannot connect to %s while adding %s. Connection refused.",
-                self.verifier_fid_str,
-                self.agent_fid_str,
+            raise UserError(
+                f"Cannot connect to {self.verifier_fid_str} while adding {self.agent_fid_str}. Connection refused."
             )
-            sys.exit()
-        elif response.status_code == 504:
+
+        if response.status_code == 504:
             logger.error("%s timed out while adding %s.", self.verifier_fid_str, self.agent_fid_str)
-            sys.exit()
+            raise UserError(f"{self.verifier_fid_str} timed out while adding {self.agent_fid_str}")
 
         response_json = Tenant._jsonify_response(response, print_response=False, raise_except=True)
 
         if response.status_code == 409:
-            # this is a conflict, need to update or delete it
-            print(response_json)
-            sys.exit()
-        elif response.status_code != 200:
+            raise UserError(
+                f'{self.verifier_fid_str} responded indicating a conflict for agent {self.agent_fid_str}. Run "delete" or "update" first.'
+            )
+
+        if response.status_code != 200:
             keylime_logging.log_http_response(logger, logging.ERROR, response_json)
-            logger.error(
-                "POST command response: %s Unexpected response from %s: %s",
-                response.status_code,
-                self.verifier_fid_str,
-                response.text,
+            raise UserError(
+                f"POST command response: {response.status_code} Unexpected response from {self.verifier_fid_str}: {response.text}",
             )
-            sys.exit()
-        else:
-            numtries = 0
-            added = False
 
-            while not added:
-                reponse_json = self.do_cvstatus()
-                if reponse_json["code"] != 200:
-                    numtries += 1
-                    if numtries >= self.maxr:
-                        logger.error(
-                            "%s still not added to %s after %d tries",
-                            self.agent_fid_str,
-                            self.verifier_fid_str,
-                            numtries,
-                        )
-                        sys.exit()
-                    next_retry = retry.retry_time(self.exponential_backoff, self.retry_interval, numtries, logger)
-                    logger.info(
-                        "%s still not added to %s at try %d/%d, trying again in %d seconds...",
-                        self.agent_fid_str,
-                        self.verifier_fid_str,
-                        numtries,
-                        self.maxr,
-                        next_retry,
+        numtries = 0
+        added = False
+
+        while not added:
+            reponse_json = self.do_cvstatus(not_found_fail=False)
+            if reponse_json["code"] != 200:
+                numtries += 1
+                if numtries >= self.maxr:
+                    raise UserError(
+                        f"{self.agent_fid_str} still not added to {self.verifier_fid_str} after ${numtries} tries"
                     )
-                    time.sleep(next_retry)
-                else:
-                    added = True
+
+                next_retry = retry.retry_time(self.exponential_backoff, self.retry_interval, numtries, logger)
+                logger.info(
+                    "%s still not added to %s at try %d/%d, trying again in %d seconds...",
+                    self.agent_fid_str,
+                    self.verifier_fid_str,
+                    numtries,
+                    self.maxr,
+                    next_retry,
+                )
+                time.sleep(next_retry)
+            else:
+                added = True
 
             if added:
                 logger.info(
                     "%s added to %s after %d tries",
                     self.agent_fid_str,
                     self.verifier_fid_str,
                     numtries,
                 )
 
-    def do_cvstatus(self) -> Dict[str, Any]:
+    def do_cvstatus(self, not_found_fail: bool = True) -> Dict[str, Any]:
         """Perform operational state look up for agent on the verifier"""
 
         self.set_full_id_str()
 
         do_cvstatus = RequestsClient(self.verifier_base_url, True, tls_context=self.tls_context)
 
         response = do_cvstatus.get((f"/v{self.api_version}/agents/{self.agent_uuid}"), timeout=self.request_timeout)
 
         response_json = Tenant._jsonify_response(response, print_response=False, raise_except=True)
 
         if response.status_code == 503:
-            logger.error(
-                "Cannot connect to %s. Connection refused.",
-                self.verifier_fid_str,
-            )
-            return response_json
+            raise UserError(f"Cannot connect to {self.verifier_fid_str}. Connection refused.")
+
         if response.status_code == 504:
             logger.error("%s timed out.", self.verifier_fid_str)
-            return response_json
+            raise UserError("{self.verifier_fid_str} timed out.")
+
         if response.status_code == 404:
             # Marked for deletion (need to modify the code on CI tests)
             logger.info(
                 "Verifier at %s with Port %s does not have agent %s.",
                 self.verifier_ip,
                 self.verifier_port,
                 self.agent_uuid,
             )
-            logger.info(
-                "%s does not exist on %s.",
-                self.agent_fid_str,
-                self.verifier_fid_str,
-            )
+            if not_found_fail:
+                raise UserError(f"{self.agent_fid_str} does not exist on {self.verifier_fid_str}.")
+
             return response_json
 
         if response.status_code == 200:
             res = response_json.pop("results")
             response_json["results"] = {self.agent_uuid: res}
 
             operational_state = states.state_to_str(response_json["results"][self.agent_uuid]["operational_state"])
             response_json["results"][self.agent_uuid]["operational_state"] = operational_state
 
             logger.info("Agent Info from %s:\n%s", self.verifier_fid_str, json.dumps(response_json["results"]))
 
             return response_json
 
-        logger.info(
-            "Status command response: %s. Unexpected response from %s. %s",
-            response.status_code,
-            self.verifier_fid_str,
-            str(response),
+        # EVALUATE DELETION
+        #        logger.info(
+        #            "Status command response: %s. Unexpected response from %s. %s",
+        #            response.status_code,
+        #            self.verifier_fid_str,
+        #            str(response),
+        #        )
+        raise UserError(
+            f"Status command response: {response.status_code}. Unexpected response from {self.verifier_fid_str} while checking status for {self.agent_fid_str} : {response}"
         )
-        return response_json
 
     def do_cvlist(self) -> Union[requests.Response, Dict[str, Any]]:
         """List all agent statuses in cloudverifier"""
 
         do_cvstatus = RequestsClient(self.verifier_base_url, True, tls_context=self.tls_context)
 
         verifier_id = ""
@@ -740,33 +734,30 @@
             return response_json
         if response.status_code == 404:
             logger.info(
                 "%s does not have any agents",
                 self.verifier_fid_str,
             )
             return response_json
+
         if response.status_code == 200:
             # Marked for deletion (need to modify the code on CI tests)
             logger.info(
                 'From verifier %s port %s retrieved: "%s"\n', self.verifier_ip, self.verifier_port, response_json
             )
 
             logger.info(
                 "Agent list from %s retrieved: \n%s", self.verifier_fid_str, json.dumps(response_json["results"])
             )
 
             return response
 
-        logger.info(
-            "Status command response: %s. Unexpected response from %s. %s",
-            response.status_code,
-            self.verifier_fid_str,
-            str(response),
+        raise UserError(
+            f"Status command response: {response.status_code}. Unexpected response from {self.verifier_fid_str} while providing agent list : {response}"
         )
-        return response
 
     def do_cvbulkinfo(self) -> Dict[str, Any]:
         """Perform operational state look up for all agents"""
 
         do_cvstatus = RequestsClient(self.verifier_base_url, True, tls_context=self.tls_context)
 
         verifier_id = ""
@@ -787,24 +778,24 @@
                     response_json["results"][agent]["operational_state"]
                 )
             logger.info("Bulk Agent Info:\n%s", json.dumps(response_json["results"]))
 
             return response_json
 
         raise UserError(
-            f"Bulk Status: Unexpected response from {self.verifier_fid_str}. Response status code is {response.status_code}"
+            f"Status command response: {response.status_code}. Unexpected response from {self.verifier_fid_str} while providing bulk status for all agents : {response}"
         )
 
     def do_cvdelete(self, verifier_check: bool = True) -> None:
         """Delete agent from Verifier."""
 
         self.set_full_id_str()
 
         if verifier_check:
-            cvresponse = self.do_cvstatus()
+            cvresponse = self.do_cvstatus(not_found_fail=False)
 
             if not isinstance(cvresponse, dict):
                 keylime_logging.log_http_response(logger, logging.ERROR, cvresponse)
                 sys.exit()
 
             if cvresponse["code"] == 404:
                 logger.info(
@@ -824,43 +815,51 @@
 
         do_cvdelete = RequestsClient(self.verifier_base_url, True, tls_context=self.tls_context)
         response = do_cvdelete.delete(f"/v{self.api_version}/agents/{self.agent_uuid}", timeout=self.request_timeout)
 
         response_json = Tenant._jsonify_response(response, print_response=False, raise_except=True)
 
         if response_json["code"] == 503:
-            logger.error(
-                "Cannot connect to %s to delete %s. Connection refused.",
-                self.verifier_fid_str,
-                self.agent_fid_str,
+            # EVALUATE DELETION
+            #            logger.error(
+            #                "Cannot connect to %s to delete %s. Connection refused.",
+            #                self.verifier_fid_str,
+            #                self.agent_fid_str,
+            #            )
+            #            keylime_logging.log_http_response(logger, logging.ERROR, response_json)
+            raise UserError(
+                f"Cannot connect to {self.verifier_fid_str} to delete {self.agent_fid_str}. Connection refused."
             )
-            keylime_logging.log_http_response(logger, logging.ERROR, response_json)
-            sys.exit()
 
         if response_json["code"] == 504:
-            logger.error("%s timed out while deleting %s.", self.verifier_fid_str, self.agent_fid_str)
-            keylime_logging.log_http_response(logger, logging.ERROR, response_json)
-            sys.exit()
+            # EVALUATE DELETION
+            #            logger.error("%s timed out while deleting %s.", self.verifier_fid_str, self.agent_fid_str)
+            #            keylime_logging.log_http_response(logger, logging.ERROR, response_json)
+            raise UserError(f"{self.verifier_fid_str} timed out while deleting {self.agent_fid_str}.")
 
         if response_json["code"] == 202:
             numtries = 0
             deleted = False
 
             while not deleted:
-                reponse_json = self.do_cvstatus()
+                reponse_json = self.do_cvstatus(not_found_fail=False)
                 if reponse_json["code"] != 404:
                     numtries += 1
                     if numtries >= self.maxr:
-                        logger.error(
-                            "%s was not deleted from %s after %d tries",
-                            self.agent_fid_str,
-                            self.verifier_fid_str,
-                            numtries,
+                        # EVALUATE DELETION
+                        #                        logger.error(
+                        #                            "%s was not deleted from %s after %d tries",
+                        #                            self.agent_fid_str,
+                        #                            self.verifier_fid_str,
+                        #                            numtries,
+                        #                        )
+                        raise UserError(
+                            f"{self.agent_fid_str,} was not deleted from {self.verifier_fid_str} after %d tries"
                         )
-                        sys.exit()
+
                     next_retry = retry.retry_time(self.exponential_backoff, self.retry_interval, numtries, logger)
                     logger.info(
                         "%s still not deleted from %s at try %d/%d, trying again in %s seconds...",
                         self.agent_fid_str,
                         self.verifier_fid_str,
                         numtries,
                         self.maxr,
@@ -900,30 +899,34 @@
             response = {
                 "code": 404,
                 # Marked for deletion. The "status" field should be replaced by "status": f"{self.agent_fid_str} does not exist on {self.registrar_fid_str}.",
                 "status": f"Agent {self.agent_uuid} does not exist on "
                 f"registrar {self.registrar_ip} port {self.registrar_port}.",
                 "results": {},
             }
+            # should be DEBUG # EVALUATE DELETION
             logger.info(json.dumps(response))
-            return response
+            raise UserError(
+                f"{self.agent_fid_str} does not exist on {self.registrar_fid_str}. Check the agent logs to for error messages while attempting to get registered."
+            )
 
         # Marked for deletion (the "status" line need to be changed to f"registrar {self.registrar_ip} port {self.registrar_port}.")
         response = {
             "code": 200,
             "status": f"Agent {self.agent_uuid} exists on "
             f"registrar {self.registrar_ip} port {self.registrar_port}.",
             "results": {},
         }
 
         assert isinstance(response["results"], dict)
         response["results"][self.agent_uuid] = agent_info
         response["results"][self.agent_uuid]["operational_state"] = states.state_to_str(states.REGISTERED)
 
         logger.info("Status from %s: %s", self.registrar_fid_str, response["status"])
+        # should be DEBUG
         logger.info(json.dumps(response))
         logger.info("Agent Info from %s:\n%s", self.registrar_fid_str, json.dumps(response["results"]))
 
         return response
 
     def do_reglist(self) -> Optional[Dict[str, Any]]:
         """List agents from Registrar"""
@@ -1006,61 +1009,51 @@
             data=b"",
             timeout=self.request_timeout,
         )
 
         response_json = Tenant._jsonify_response(response, print_response=False, raise_except=True)
 
         if response.status_code == 503:
-            logger.error(
-                "Cannot connect to %s. Connection refused.",
-                self.verifier_fid_str,
-            )
-            return response_json
+            raise UserError(f"Cannot connect to {self.verifier_fid_str}. Connection refused.")
+
         if response.status_code == 504:
-            logger.error("%s timed out.", self.verifier_fid_str)
-            return response_json
+            raise UserError(f"{self.verifier_fid_str} timed out.")
+
         if response.status_code == 200:
             # Marked for deletion (need to modify the code on CI tests)
             logger.info("Agent %s re-activated", self.agent_uuid)
             logger.info("%s re-activated", self.agent_fid_str)
             return response_json
 
-        keylime_logging.log_http_response(logger, logging.ERROR, response_json)
-        logger.error(
-            "Reactivate command response: %s Unexpected response from %s.", response.status_code, self.verifier_fid_str
+        raise UserError(
+            f"Reactivate command response: {response.status_code} Unexpected response from {self.verifier_fid_str}."
         )
-        return response_json
 
     def do_cvstop(self) -> None:
         """Stop declared active agent"""
         params = f"/v{self.api_version}/agents/{self.agent_uuid}/stop"
         do_cvstop = RequestsClient(self.verifier_base_url, True, tls_context=self.tls_context)
         response = do_cvstop.put(params, data=b"", timeout=self.request_timeout)
 
         self.set_full_id_str()
 
         if response.status_code == 503:
-            logger.error(
-                "Cannot connect to %s. Connection refused.",
-                self.verifier_fid_str,
-            )
-            sys.exit()
-        elif response.status_code == 504:
-            logger.error("%s timed out.", self.verifier_fid_str)
-            sys.exit()
+            raise UserError(f"Cannot connect to {self.verifier_fid_str}. Connection refused.")
 
-        response_json = Tenant._jsonify_response(response, print_response=False, raise_except=True)
+        if response.status_code == 504:
+            # EVALUATE DELETION
+            #            logger.error("%s timed out.", self.verifier_fid_str)
+            raise UserError(f"{self.verifier_fid_str} timed out.")
 
         if response.status_code != 200:
-            keylime_logging.log_http_response(logger, logging.ERROR, response_json)
-            logger.error(
-                "Stop command response: %s Unexpected response from %s.", response.status_code, self.verifier_fid_str
+            raise UserError(
+                f"Stop command response: {response.status_code} Unexpected response from {self.verifier_fid_str}."
             )
-        else:
-            logger.info("%s stopped", self.agent_fid_str)
+
+        logger.info("%s stopped", self.agent_fid_str)
 
     def do_quote(self) -> None:
         """Perform TPM quote by GET towards Agent
 
         Raises:
             UserError: Connection handler
         """
@@ -1088,19 +1081,16 @@
 
                 response_json = Tenant._jsonify_response(response, print_response=True, raise_except=True)
 
             except Exception as e:
                 if response is None or response.status_code in (503, 504):
                     numtries += 1
                     if numtries >= self.maxr:
-                        logger.error(
-                            "Tenant cannot establish connection to %s",
-                            self.agent_fid_str,
-                        )
-                        sys.exit()
+                        raise UserError(f"Tenant cannot establish connection to {self.agent_fid_str}") from e
+
                     next_retry = retry.retry_time(self.exponential_backoff, self.retry_interval, numtries, logger)
                     logger.info(
                         "Tenant connection to %s refused %s/%s times, trying again in %s seconds...",
                         self.agent_fid_str,
                         numtries,
                         self.maxr,
                         next_retry,
@@ -1109,15 +1099,15 @@
                     continue
 
                 raise e
             break
 
         if response is not None and response.status_code != 200:
             raise UserError(
-                f"Status command response: {response.status_code} Unexpected response from {self.agent_fid_str}."
+                f"TPM Quote command response: {response.status_code} Unexpected response from {self.agent_fid_str}."
             )
 
         if "results" not in response_json:
             raise UserError(
                 f"Error: unexpected http response body from {self.agent_fid_str}: {str(response.status_code)}"
             )
 
@@ -1177,22 +1167,18 @@
                 response = post_ukey.post(params, json=data, timeout=self.request_timeout)
         else:
             logger.warning("Connecting to %s without using mTLS!", self.agent_fid_str)
             post_ukey = RequestsClient(cloudagent_base_url, tls_enabled=False)
             response = post_ukey.post(params, json=data, timeout=self.request_timeout)
 
         if response.status_code == 503:
-            logger.error(
-                "Cannot connect to %s to post encrypted U. Connection refused.",
-                self.agent_fid_str,
-            )
-            sys.exit()
-        elif response.status_code == 504:
-            logger.error("%s timed out while posting encrypted U", self.agent_fid_str)
-            sys.exit()
+            raise UserError(f"Cannot connect to {self.agent_fid_str} to post encrypted U. Connection refused.")
+
+        if response.status_code == 504:
+            raise UserError(f"{self.agent_fid_str} timed out while posting encrypted U")
 
         if response.status_code != 200:
             keylime_logging.log_http_response(logger, logging.ERROR, response_json)
             raise UserError(
                 f"Posting of encrypted U to {self.agent_fid_str} failed with response code {response.status_code} ({response.text})"
             )
 
@@ -1225,17 +1211,17 @@
 
                 response_json = Tenant._jsonify_response(response, print_response=False, raise_except=True)
 
             except Exception as e:
                 if response is not None and response.status_code in (503, 504):
                     numtries += 1
                     if numtries >= self.maxr:
-                        logger.error("Cannot establish connection to %s", self.agent_fid_str)
                         self.do_cvstop()
-                        sys.exit()
+                        raise UserError(f"Cannot establish connection to {self.agent_fid_str}") from e
+
                     next_retry = retry.retry_time(self.exponential_backoff, self.retry_interval, numtries, logger)
                     logger.info(
                         "Connection to %s refused %s/%s times, trying again in %s seconds...",
                         self.agent_fid_str,
                         numtries,
                         self.maxr,
                         next_retry,
@@ -1246,39 +1232,41 @@
                 raise e
 
             mac = ""
             ex_mac = crypto.do_hmac(self.K, challenge)
 
             if response.status_code == 200:
                 if "results" not in response_json or "hmac" not in response_json["results"]:
-                    logger.critical(
-                        "Error: unexpected http response body from %s : %s",
-                        self.agent_fid_str,
-                        response.status_code,
-                    )
                     self.do_cvstop()
-                    break
+                    raise UserError(
+                        f"Error: unexpected http response body from {self.agent_fid_str} : {response.status_code}"
+                    )
+
                 mac = response_json["results"]["hmac"]
 
                 if mac == ex_mac:
                     logger.info("Successful key derivation for %s", self.agent_fid_str)
 
             if mac != ex_mac:
                 if response.status_code != 200:
                     keylime_logging.log_http_response(logger, logging.ERROR, response_json)
                 numtries += 1
                 if numtries >= self.maxr:
-                    logger.error(
-                        "Failed key derivation for %s (expected length %d, received %d",
-                        self.agent_fid_str,
-                        len(ex_mac),
-                        len(mac),
-                    )
+                    # EVALUATE DELETION
+                    #                    logger.error(
+                    #                        "Failed key derivation for %s (expected length %d, received %d",
+                    #                        self.agent_fid_str,
+                    #                        len(ex_mac),
+                    #                        len(mac),
+                    #                    )
                     self.do_cvstop()
-                    sys.exit()
+                    raise UserError(
+                        f"Failed key derivation for {self.agent_fid_str} (expected length {len(ex_mac)}, received {len(mac)})"
+                    )
+
                 next_retry = retry.retry_time(self.exponential_backoff, self.retry_interval, numtries, logger)
                 logger.info(
                     "Key derivation not yet complete for %s at try %d/%d (expected length %d, received length %d) trying again in %d seconds... (Ctrl-C to stop)",
                     self.agent_fid_str,
                     numtries,
                     self.maxr,
                     len(ex_mac),
```

### Comparing `keylime-7.3.0/keylime/tornado_requests.py` & `keylime-7.4.0/keylime/tornado_requests.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/tpm/ec_crypto_helper.py` & `keylime-7.4.0/keylime/tpm/ec_crypto_helper.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/tpm/tpm2_objects.py` & `keylime-7.4.0/keylime/tpm/tpm2_objects.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/tpm/tpm2_objects_test.py` & `keylime-7.4.0/keylime/tpm/tpm2_objects_test.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime/tpm/tpm_main.py` & `keylime-7.4.0/keylime/tpm/tpm_main.py`

 * *Files 3% similar despite different names*

```diff
@@ -176,24 +176,15 @@
         pcr_allowlist = tpm_policy_dict.copy()
 
         if "mask" in pcr_allowlist:
             del pcr_allowlist["mask"]
         # convert all pcr num keys to integers
         pcr_allowlist = {int(k): v for k, v in list(pcr_allowlist.items())}
 
-        # temporary: to avoid a CI failure, we don't attempt to evaluate
-        # boot logs when the policy is empty. This is because the CI
-        # system currently cannot simulate MBA correctly.
-        # we parse mb_refstate here to figure out whether it's empty.
-        if not mb_refstate:
-            mb_refstate_data = None
-        else:
-            mb_refstate_data = json.loads(mb_refstate)
-
-        mb_pcrs_hashes, boot_aggregates, mb_measurement_data, mb_failure = mba.parse_bootlog(
+        mb_pcrs_hashes, boot_aggregates, mb_measurement_data, mb_failure = mba.bootlog_parse(
             mb_measurement_list, hash_alg
         )
         failure.merge(mb_failure)
 
         pcrs_in_quote: Set[int] = set()  # PCRs in quote that were already used for some kind of validation
 
         pcr_nums = set(pcrs_dict.keys())
@@ -248,15 +239,15 @@
             pcrs_in_quote.add(config.IMA_PCR)
 
         # Collect mismatched measured boot PCRs as measured_boot failures
         mb_pcr_failure = Failure(Component.MEASURED_BOOT)
         # Handle measured boot PCRs only if the parsing worked
         if not mb_failure:
             for pcr_num in set(config.MEASUREDBOOT_PCRS) & pcr_nums:
-                if mb_refstate_data:
+                if mba.policy_is_valid(mb_refstate):
                     if not mb_measurement_list:
                         logger.error(
                             "Measured Boot PCR %d in policy, but no measurement list provided by agent %s",
                             pcr_num,
                             agent_id,
                         )
                         failure.add_event(
@@ -339,16 +330,16 @@
             pcrs_in_quote.add(pcr_num)
 
         missing = set(pcr_allowlist.keys()) - pcrs_in_quote
         if len(missing) > 0:
             logger.error("PCRs specified in policy not in quote (from agent %s): %s", agent_id, missing)
             failure.add_event("missing_pcrs", {"context": "PCRs are missing in quote", "data": list(missing)}, True)
 
-        if not mb_failure and mb_refstate_data:
-            mb_policy_failure = mba.evaluate_bootlog(
+        if not mb_failure and mba.policy_is_valid(mb_refstate):
+            mb_policy_failure = mba.bootlog_evaluate(
                 mb_refstate,
                 mb_measurement_data,
                 pcrs_in_quote,
                 agentAttestState.get_agent_id(),
             )
             failure.merge(mb_policy_failure)
```

### Comparing `keylime-7.3.0/keylime/tpm/tpm_util.py` & `keylime-7.4.0/keylime/tpm/tpm_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,50 @@
+# Some of the functions in this file were adapted from Microsoft's TPM 2
+# reference implementation that states the following:
+#
+# Microsoft Reference Implementation for TPM 2.0
+#
+#  The copyright in this software is being made available under the BSD License,
+#  included below. This software may be subject to other third party and
+#  contributor rights, including patent rights, and no such rights are granted
+#  under this license.
+#
+#  Copyright (c) Microsoft Corporation
+#
+#  All rights reserved.
+#
+#  BSD License
+#
+#  Redistribution and use in source and binary forms, with or without modification,
+#  are permitted provided that the following conditions are met:
+#
+#  Redistributions of source code must retain the above copyright notice, this list
+#  of conditions and the following disclaimer.
+#
+#  Redistributions in binary form must reproduce the above copyright notice, this
+#  list of conditions and the following disclaimer in the documentation and/or
+#  other materials provided with the distribution.
+#
+#  THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS ""AS IS""
+#  AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+#  IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+#  DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR
+#  ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
+#  (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
+#  LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
+#  ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+#  (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
+#  SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+#
+
 import os
 import string
 import struct
 from typing import Any, Dict, List, Optional, Tuple, Union
 
-from cryptography.exceptions import InvalidSignature
 from cryptography.hazmat import backends
 from cryptography.hazmat.primitives import hashes, hmac, serialization
 from cryptography.hazmat.primitives.asymmetric import ec, padding
 from cryptography.hazmat.primitives.asymmetric.ec import EllipticCurvePublicKey
 from cryptography.hazmat.primitives.asymmetric.rsa import RSAPublicKey
 from cryptography.hazmat.primitives.asymmetric.utils import Prehashed
 from cryptography.hazmat.primitives.ciphers import Cipher, modes
@@ -151,37 +188,27 @@
     if hashfunc.name != exp_hash_alg:
         raise ValueError(f"Quote was expected to use {exp_hash_alg} but used {hashfunc.name} instead")
 
     digest = hashes.Hash(hashfunc, backend=backends.default_backend())
     digest.update(quoteblob)
     quote_digest = digest.finalize()
 
-    try:
-        verify(pubkey, signature, quote_digest, hashfunc)
-    except InvalidSignature:
-        logger.error("Invalid quote signature!")
+    verify(pubkey, signature, quote_digest, hashfunc)
 
     # Check that reported nonce is expected one
     retDict = tpm2_objects.unmarshal_tpms_attest(quoteblob)
     extradata = retDict["extraData"]
     if extradata.decode("utf-8") != nonce:
         raise Exception("The nonce from the attestation differs from the expected nonce")
 
     # Check that correct quote_digest was used which is equivalent to hash(quoteblob)
     compare_digest, pcrs_dict = __get_and_hash_pcrs(pcrblob, hash_alg)
     if retDict["attested.quote.pcrDigest"] != compare_digest:
         raise Exception("The digest used for quoting is different than the one that was calculated")
 
-    digest = hashes.Hash(hashfunc, backend=backends.default_backend())
-    digest.update(quoteblob)
-    quoteblob_digest = digest.finalize()
-
-    if quoteblob_digest != quote_digest:
-        raise Exception("The digest of the quoteblob differs from the quote's digest")
-
     return pcrs_dict
 
 
 def label_to_bytes(label: str) -> bytes:
     return bytes(label, "UTF-8") + b"\x00"
```

### Comparing `keylime-7.3.0/keylime/tpm/tpm_util_test.py` & `keylime-7.4.0/keylime/tpm/tpm_util_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import base64
 import unittest
 from unittest import mock
 
+from cryptography.exceptions import InvalidSignature
 from cryptography.hazmat.primitives.asymmetric.ec import (
     SECP256R1,
     EllipticCurve,
     EllipticCurvePrivateKey,
     EllipticCurvePrivateNumbers,
     EllipticCurvePublicNumbers,
 )
@@ -56,14 +57,34 @@
         nonce = "Ai5M5SjYjnkyv4P7itH1"
 
         try:
             checkquote(aikblob, nonce, sigblob, quoteblob, pcrblob, "sha256")
         except Exception as e:
             self.fail(f"checkquote failed with {e}")
 
+        # test bad input
+        bad_quoteblob = bytearray(quoteblob)
+        bad_quoteblob[5] ^= 0x1
+        with self.assertRaises(InvalidSignature):
+            checkquote(aikblob, nonce, sigblob, bad_quoteblob, pcrblob, "sha256")
+
+        l = list(nonce)
+        l[0] = "a"
+        bad_nonce = "".join(l)
+        with self.assertRaises(Exception):
+            checkquote(aikblob, bad_nonce, sigblob, quoteblob, pcrblob, "sha256")
+
+        bad_pcrblob = bytearray(pcrblob)
+        bad_pcrblob[5] ^= 0x1
+        with self.assertRaises(Exception):
+            checkquote(aikblob, nonce, sigblob, quoteblob, bad_pcrblob, "sha256")
+
+        with self.assertRaises(ValueError):
+            checkquote(aikblob, nonce, sigblob, quoteblob, pcrblob, "sha1")
+
     @staticmethod
     def not_random(numbytes: int) -> bytes:
         return b"\x12" * numbytes
 
     def test_makecredential(self) -> None:
         with mock.patch("os.urandom", TestTpmUtil.not_random):
             ek_tpm = bytes.fromhex(
```

### Comparing `keylime-7.3.0/keylime/web_util.py` & `keylime-7.4.0/keylime/web_util.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/keylime.egg-info/PKG-INFO` & `keylime-7.4.0/keylime.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keylime
-Version: 7.3.0
+Version: 7.4.0
 Summary: TPM-based key bootstrapping and system integrity measurement system for cloud
 Home-page: https://keylime.dev
 Author: Keylime Community
 Author-email: keylime@groups.io
 License: Apache-2.0
 Project-URL: Source, https://github.com/keylime/keylime
 Project-URL: Documentation, https://keylime.readthedocs.io/en/latest/
```

### Comparing `keylime-7.3.0/keylime.egg-info/SOURCES.txt` & `keylime-7.4.0/keylime.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -84,16 +84,16 @@
 keylime/ima/ima.py
 keylime/ima/ima_dm.py
 keylime/ima/types.py
 keylime/mba/__init__.py
 keylime/mba/mba.py
 keylime/mba/elchecking/__init__.py
 keylime/mba/elchecking/__main__.py
+keylime/mba/elchecking/elchecker.py
 keylime/mba/elchecking/example.py
-keylime/mba/elchecking/mbpolicy.py
 keylime/mba/elchecking/policies.py
 keylime/mba/elchecking/tests.py
 keylime/mba/elparsing/__init__.py
 keylime/mba/elparsing/tpm2_tools_elparser.py
 keylime/mba/elparsing/tpm_bootlog_enrich.py
 keylime/migrations/__init__.py
 keylime/migrations/alembic.ini
```

### Comparing `keylime-7.3.0/keylime.egg-info/entry_points.txt` & `keylime-7.4.0/keylime.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/setup.cfg` & `keylime-7.4.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = keylime
-version = 7.3.0
+version = 7.4.0
 description = TPM-based key bootstrapping and system integrity measurement system for cloud
 long_description = file: _pypi-notice.md, README.md
 long_description_content_type = text/markdown; charset=UTF-8
 url = https://keylime.dev
 author = Keylime Community
 author_email = keylime@groups.io
 license = Apache-2.0
```

### Comparing `keylime-7.3.0/setup.py` & `keylime-7.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/templates/2.0/adjust.py` & `keylime-7.4.0/templates/2.0/adjust.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/templates/2.0/agent.j2` & `keylime-7.4.0/templates/2.0/agent.j2`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/templates/2.0/ca.j2` & `keylime-7.4.0/templates/2.0/ca.j2`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/templates/2.0/logging.j2` & `keylime-7.4.0/templates/2.0/logging.j2`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/templates/2.0/mapping.json` & `keylime-7.4.0/templates/2.0/mapping.json`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/templates/2.0/registrar.j2` & `keylime-7.4.0/templates/2.0/registrar.j2`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/templates/2.0/tenant.j2` & `keylime-7.4.0/templates/2.0/tenant.j2`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/templates/2.0/verifier.j2` & `keylime-7.4.0/templates/2.0/verifier.j2`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/test/test_algorithms.py` & `keylime-7.4.0/test/test_algorithms.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/test/test_api_version.py` & `keylime-7.4.0/test/test_api_version.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/test/test_ca_impl_openssl.py` & `keylime-7.4.0/test/test_ca_impl_openssl.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/test/test_ca_util.py` & `keylime-7.4.0/test/test_ca_util.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/test/test_cert_utils.py` & `keylime-7.4.0/test/test_cert_utils.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/test/test_config.py` & `keylime-7.4.0/test/test_config.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/test/test_convert_config.py` & `keylime-7.4.0/test/test_convert_config.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/test/test_crypto.py` & `keylime-7.4.0/test/test_crypto.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/test/test_fs_util.py` & `keylime-7.4.0/test/test_fs_util.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/test/test_ima_ast.py` & `keylime-7.4.0/test/test_ima_ast.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/test/test_ima_dm.py` & `keylime-7.4.0/test/test_ima_dm.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/test/test_ima_verification.py` & `keylime-7.4.0/test/test_ima_verification.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/test/test_json.py` & `keylime-7.4.0/test/test_json.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/test/test_mba_parsing.py` & `keylime-7.4.0/test/test_mba_parsing.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 from keylime.common.algorithms import Hash
 from keylime.mba import mba
 
 
 class TestMBAParsing(unittest.TestCase):
     def test_parse_bootlog(self):
         """Test parsing binary measured boot event log"""
+        mba.load_imports()
         # Use the file that triggered https://github.com/keylime/keylime/issues/1153
         mb_log_path = os.path.abspath(os.path.join(os.path.dirname(__file__), "data/mb_log.b64"))
         with open(mb_log_path, encoding="utf-8") as f:
             # Read the base64 input and remove the newlines
             b64 = "".join(f.read().splitlines())
-            pcr_hashes, boot_aggregates, measurement_data, failure = mba.parse_bootlog(b64, Hash.SHA256)
+            pcr_hashes, boot_aggregates, measurement_data, failure = mba.bootlog_parse(b64, Hash.SHA256)
 
             self.assertFalse(
                 failure, f"Parsing of measured boot log failed with: {list(map(lambda x: x.context, failure.events))}"
             )
             self.assertTrue(isinstance(pcr_hashes, dict))
             self.assertTrue(isinstance(boot_aggregates, dict))
             self.assertTrue(isinstance(measurement_data, dict))
```

### Comparing `keylime-7.3.0/test/test_policy_conversion.py` & `keylime-7.4.0/test/test_policy_conversion.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/test/test_registrar_db.py` & `keylime-7.4.0/test/test_registrar_db.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/test/test_retry_algo.py` & `keylime-7.4.0/test/test_retry_algo.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/test/test_signing.py` & `keylime-7.4.0/test/test_signing.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/test/test_validators.py` & `keylime-7.4.0/test/test_validators.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/test/test_verifier_db.py` & `keylime-7.4.0/test/test_verifier_db.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/test/test_version.py` & `keylime-7.4.0/test/test_version.py`

 * *Files identical despite different names*

### Comparing `keylime-7.3.0/test/test_web_util.py` & `keylime-7.4.0/test/test_web_util.py`

 * *Files identical despite different names*

