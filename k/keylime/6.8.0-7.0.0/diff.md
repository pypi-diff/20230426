# Comparing `tmp/keylime-6.8.0.tar.gz` & `tmp/keylime-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keylime-6.8.0.tar", last modified: Tue Apr 25 18:28:28 2023, max compression
+gzip compressed data, was "keylime-7.0.0.tar", last modified: Tue Apr 25 19:22:05 2023, max compression
```

## Comparing `keylime-6.8.0.tar` & `keylime-7.0.0.tar`

### file list

```diff
@@ -1,179 +1,179 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:28:28.364539 keylime-6.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-25 18:28:19.000000 keylime-6.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-25 18:28:19.000000 keylime-6.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-04-25 18:28:28.364539 keylime-6.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11220 2023-04-25 18:28:19.000000 keylime-6.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-25 18:28:19.000000 keylime-6.8.0/_pypi-notice.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:28:28.344539 keylime-6.8.0/keylime/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/agentstates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/api_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    45700 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/backport_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/ca_impl_openssl.py
--rw-r--r--   0 runner    (1001) docker     (123)    15541 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/ca_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/cert_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:28:28.348539 keylime-6.8.0/keylime/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/cli/policies.py
--rw-r--r--   0 runner    (1001) docker     (123)    12967 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/cloud_verifier_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    68876 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/cloud_verifier_tornado.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:28:28.348539 keylime-6.8.0/keylime/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/cmd/attest.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/cmd/ca.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20465 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/cmd/convert_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8890 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/cmd/convert_runtime_policy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22220 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/cmd/create_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/cmd/registrar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/cmd/sign_runtime_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/cmd/tenant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/cmd/user_data_encrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/cmd/verifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/cmd_exec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:28:28.348539 keylime-6.8.0/keylime/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/common/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/common/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/common/migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/common/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/common/states.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/common/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/common/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16220 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:28:28.352539 keylime-6.8.0/keylime/da/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/da/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/da/attest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:28:28.352539 keylime-6.8.0/keylime/da/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/da/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/da/examples/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/da/examples/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/da/examples/rekor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/da/examples/sqldb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/da/examples/tsa_rfc3161.py
--rw-r--r--   0 runner    (1001) docker     (123)    16781 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/da/record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:28:28.352539 keylime-6.8.0/keylime/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/db/keylime_db.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/db/registrar_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/db/verifier_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:28:28.352539 keylime-6.8.0/keylime/dsse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/dsse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/dsse/dsse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/dsse/ecdsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/dsse/x509.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:28:28.352539 keylime-6.8.0/keylime/elchecking/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/elchecking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/elchecking/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17614 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/elchecking/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/elchecking/policies.py
--rw-r--r--   0 runner    (1001) docker     (123)    24307 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/elchecking/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/failure.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/fs_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:28:28.352539 keylime-6.8.0/keylime/ima/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/ima/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14117 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/ima/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/ima/dm_grammar.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18471 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/ima/file_signatures.py
--rw-r--r--   0 runner    (1001) docker     (123)    24445 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/ima/ima.py
--rw-r--r--   0 runner    (1001) docker     (123)    32160 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/ima/ima_dm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/ima/ima_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/ima/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/ip_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/keylime_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/measured_boot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:28:28.356539 keylime-6.8.0/keylime/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/migrations/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/migrations/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:28:28.356539 keylime-6.8.0/keylime/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/migrations/versions/039322ea079b_add_generator_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/migrations/versions/1ac1513ef2a1_fix_mb_and_ima_column_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/migrations/versions/257fe0f0c039_add_fields_for_revocation_context_to_.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/migrations/versions/2fbc0fb8fa4d_add_checksum_to_allowlist.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/migrations/versions/4089e1c79be9_add_tpm_clockinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/migrations/versions/4329e2d14944_associate_moved_allowlists_to_agents.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/migrations/versions/63c30820fdc1_add_mtls_cert_and_ak_to_verifier_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/migrations/versions/7d5db1a6ffb0_add_agentstates_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/migrations/versions/8a44a4364f5a_initial_database_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/migrations/versions/8c0f8ded1f90_convert_allowlists_to_ima_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/migrations/versions/8da20383f6e1_extend_ip_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/migrations/versions/9169f80345ed_add_supported_version_to_verifiermain_.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/migrations/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/migrations/versions/a09cc94177f0_add_last_received_quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/migrations/versions/a72aec03d720_migrate_allowlists_to_separate_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/migrations/versions/a79c27ec1054_add_mtls_cert_field_to_registrar.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/migrations/versions/a7a64155ab3a_add_ima_filesigning_keys_column.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/migrations/versions/ae898986c6e9_add_mb_refstate_column.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/migrations/versions/b4d024197413_add_verfier_id_to_verifiermain_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/migrations/versions/bc3b6b551b0a_drop_vtpm_colums.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/migrations/versions/bf48e0c4751d_add_attestation_count_column.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/migrations/versions/c3842cc9ee69_store_keyrings_learned_from_ima_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/migrations/versions/cc2630851a1f_receive_the_aik_tpm_from_the_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/migrations/versions/eb869a77abd1_create_allowlist_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/migrations/versions/eeb702f77d7d_allowlist_rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/migrations/versions/f35cdd35eb83_move_v_tpm_policy_to_jsonpickletype.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/migrations/versions/f82c4252bc4f_add_ip_and_port_to_registrar.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/migrations/versions/f838d3cdeead_add_last_successful_attestation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/registrar_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23297 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/registrar_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/requests_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/revocation_notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/signing.py
--rw-r--r--   0 runner    (1001) docker     (123)    74195 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/tenant.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/tornado_requests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:28:28.360539 keylime-6.8.0/keylime/tpm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/tpm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12250 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/tpm/tpm2_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    17761 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/tpm/tpm2_objects_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/tpm/tpm_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    29642 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/tpm/tpm_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/tpm_bootlog_enrich.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/tpm_ek_ca.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    17135 2023-04-25 18:28:19.000000 keylime-6.8.0/keylime/web_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:28:28.348539 keylime-6.8.0/keylime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-04-25 18:28:28.000000 keylime-6.8.0/keylime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-04-25 18:28:28.000000 keylime-6.8.0/keylime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 18:28:28.000000 keylime-6.8.0/keylime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-25 18:28:28.000000 keylime-6.8.0/keylime.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 18:28:28.000000 keylime-6.8.0/keylime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-25 18:28:28.000000 keylime-6.8.0/keylime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-25 18:28:19.000000 keylime-6.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-25 18:28:28.364539 keylime-6.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-25 18:28:19.000000 keylime-6.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:28:28.340539 keylime-6.8.0/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:28:28.360539 keylime-6.8.0/templates/2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-04-25 18:28:19.000000 keylime-6.8.0/templates/2.0/adjust.py
--rw-r--r--   0 runner    (1001) docker     (123)     8390 2023-04-25 18:28:19.000000 keylime-6.8.0/templates/2.0/agent.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-25 18:28:19.000000 keylime-6.8.0/templates/2.0/ca.j2
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-25 18:28:19.000000 keylime-6.8.0/templates/2.0/logging.j2
--rw-r--r--   0 runner    (1001) docker     (123)    26831 2023-04-25 18:28:19.000000 keylime-6.8.0/templates/2.0/mapping.json
--rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-04-25 18:28:19.000000 keylime-6.8.0/templates/2.0/registrar.j2
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-04-25 18:28:19.000000 keylime-6.8.0/templates/2.0/tenant.j2
--rw-r--r--   0 runner    (1001) docker     (123)    11233 2023-04-25 18:28:19.000000 keylime-6.8.0/templates/2.0/verifier.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:28:28.364539 keylime-6.8.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-25 18:28:19.000000 keylime-6.8.0/test/test_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-04-25 18:28:19.000000 keylime-6.8.0/test/test_api_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-25 18:28:19.000000 keylime-6.8.0/test/test_ca_impl_openssl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-25 18:28:19.000000 keylime-6.8.0/test/test_ca_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-04-25 18:28:19.000000 keylime-6.8.0/test/test_cert_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-04-25 18:28:19.000000 keylime-6.8.0/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18107 2023-04-25 18:28:19.000000 keylime-6.8.0/test/test_convert_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-25 18:28:19.000000 keylime-6.8.0/test/test_crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-25 18:28:19.000000 keylime-6.8.0/test/test_fs_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-04-25 18:28:19.000000 keylime-6.8.0/test/test_ima_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)    23474 2023-04-25 18:28:19.000000 keylime-6.8.0/test/test_ima_dm.py
--rw-r--r--   0 runner    (1001) docker     (123)    20101 2023-04-25 18:28:19.000000 keylime-6.8.0/test/test_ima_verification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-25 18:28:19.000000 keylime-6.8.0/test/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-25 18:28:19.000000 keylime-6.8.0/test/test_policy_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     7349 2023-04-25 18:28:19.000000 keylime-6.8.0/test/test_registrar_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-25 18:28:19.000000 keylime-6.8.0/test/test_retry_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-25 18:28:19.000000 keylime-6.8.0/test/test_signing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-04-25 18:28:19.000000 keylime-6.8.0/test/test_tpm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-04-25 18:28:19.000000 keylime-6.8.0/test/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)    11601 2023-04-25 18:28:19.000000 keylime-6.8.0/test/test_verifier_db.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-25 18:28:19.000000 keylime-6.8.0/test/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-25 18:28:19.000000 keylime-6.8.0/test/test_web_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:22:05.163835 keylime-7.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-25 19:21:53.000000 keylime-7.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-25 19:21:53.000000 keylime-7.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-04-25 19:22:05.163835 keylime-7.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11220 2023-04-25 19:21:53.000000 keylime-7.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-25 19:21:53.000000 keylime-7.0.0/_pypi-notice.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:22:05.119835 keylime-7.0.0/keylime/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/agentstates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/api_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45700 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/backport_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/ca_impl_openssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15541 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/ca_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/cert_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:22:05.119835 keylime-7.0.0/keylime/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/cli/policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12967 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/cloud_verifier_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68876 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/cloud_verifier_tornado.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:22:05.123835 keylime-7.0.0/keylime/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/cmd/attest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/cmd/ca.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20465 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/cmd/convert_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8890 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/cmd/convert_runtime_policy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22220 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/cmd/create_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/cmd/registrar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/cmd/sign_runtime_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/cmd/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/cmd/user_data_encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/cmd/verifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/cmd_exec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:22:05.127836 keylime-7.0.0/keylime/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/common/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/common/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/common/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/common/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/common/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/common/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/common/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16220 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:22:05.127836 keylime-7.0.0/keylime/da/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/da/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/da/attest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:22:05.131836 keylime-7.0.0/keylime/da/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/da/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/da/examples/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/da/examples/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/da/examples/rekor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/da/examples/sqldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/da/examples/tsa_rfc3161.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16781 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/da/record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:22:05.131836 keylime-7.0.0/keylime/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/db/keylime_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/db/registrar_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/db/verifier_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:22:05.131836 keylime-7.0.0/keylime/dsse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/dsse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/dsse/dsse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/dsse/ecdsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/dsse/x509.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:22:05.131836 keylime-7.0.0/keylime/elchecking/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/elchecking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/elchecking/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17614 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/elchecking/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/elchecking/policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24307 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/elchecking/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/failure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/fs_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:22:05.135836 keylime-7.0.0/keylime/ima/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/ima/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14117 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/ima/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/ima/dm_grammar.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18471 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/ima/file_signatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24445 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/ima/ima.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32160 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/ima/ima_dm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/ima/ima_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/ima/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/ip_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/keylime_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/measured_boot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:22:05.135836 keylime-7.0.0/keylime/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:22:05.147836 keylime-7.0.0/keylime/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/039322ea079b_add_generator_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/1ac1513ef2a1_fix_mb_and_ima_column_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/257fe0f0c039_add_fields_for_revocation_context_to_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/2fbc0fb8fa4d_add_checksum_to_allowlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/4089e1c79be9_add_tpm_clockinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/4329e2d14944_associate_moved_allowlists_to_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/63c30820fdc1_add_mtls_cert_and_ak_to_verifier_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/7d5db1a6ffb0_add_agentstates_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/8a44a4364f5a_initial_database_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/8c0f8ded1f90_convert_allowlists_to_ima_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/8da20383f6e1_extend_ip_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/9169f80345ed_add_supported_version_to_verifiermain_.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/a09cc94177f0_add_last_received_quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/a72aec03d720_migrate_allowlists_to_separate_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/a79c27ec1054_add_mtls_cert_field_to_registrar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/a7a64155ab3a_add_ima_filesigning_keys_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/ae898986c6e9_add_mb_refstate_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/b4d024197413_add_verfier_id_to_verifiermain_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/bc3b6b551b0a_drop_vtpm_colums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/bf48e0c4751d_add_attestation_count_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/c3842cc9ee69_store_keyrings_learned_from_ima_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/cc2630851a1f_receive_the_aik_tpm_from_the_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/eb869a77abd1_create_allowlist_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/eeb702f77d7d_allowlist_rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/f35cdd35eb83_move_v_tpm_policy_to_jsonpickletype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/f82c4252bc4f_add_ip_and_port_to_registrar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/f838d3cdeead_add_last_successful_attestation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/registrar_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23297 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/registrar_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/requests_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/revocation_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/signing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74195 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/tornado_requests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:22:05.151836 keylime-7.0.0/keylime/tpm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/tpm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12250 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/tpm/tpm2_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17761 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/tpm/tpm2_objects_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/tpm/tpm_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29642 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/tpm/tpm_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/tpm_bootlog_enrich.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/tpm_ek_ca.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17135 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/web_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:22:05.119835 keylime-7.0.0/keylime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-04-25 19:22:05.000000 keylime-7.0.0/keylime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-04-25 19:22:05.000000 keylime-7.0.0/keylime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 19:22:05.000000 keylime-7.0.0/keylime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-25 19:22:05.000000 keylime-7.0.0/keylime.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 19:22:04.000000 keylime-7.0.0/keylime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-25 19:22:05.000000 keylime-7.0.0/keylime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-25 19:21:53.000000 keylime-7.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-25 19:22:05.163835 keylime-7.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-25 19:21:53.000000 keylime-7.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:22:05.111836 keylime-7.0.0/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:22:05.155835 keylime-7.0.0/templates/2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-04-25 19:21:53.000000 keylime-7.0.0/templates/2.0/adjust.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8390 2023-04-25 19:21:53.000000 keylime-7.0.0/templates/2.0/agent.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-25 19:21:53.000000 keylime-7.0.0/templates/2.0/ca.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-25 19:21:53.000000 keylime-7.0.0/templates/2.0/logging.j2
+-rw-r--r--   0 runner    (1001) docker     (123)    26831 2023-04-25 19:21:53.000000 keylime-7.0.0/templates/2.0/mapping.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-04-25 19:21:53.000000 keylime-7.0.0/templates/2.0/registrar.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-04-25 19:21:53.000000 keylime-7.0.0/templates/2.0/tenant.j2
+-rw-r--r--   0 runner    (1001) docker     (123)    11233 2023-04-25 19:21:53.000000 keylime-7.0.0/templates/2.0/verifier.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:22:05.163835 keylime-7.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_api_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_ca_impl_openssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_ca_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_cert_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18107 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_convert_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_fs_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_ima_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23474 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_ima_dm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20101 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_ima_verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_policy_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7349 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_registrar_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_retry_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_signing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_tpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11601 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_verifier_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_web_util.py
```

### Comparing `keylime-6.8.0/LICENSE` & `keylime-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/PKG-INFO` & `keylime-7.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keylime
-Version: 6.8.0
+Version: 7.0.0
 Summary: TPM-based key bootstrapping and system integrity measurement system for cloud
 Home-page: https://keylime.dev
 Author: Keylime Community
 Author-email: keylime@groups.io
 License: Apache-2.0
 Project-URL: Source, https://github.com/keylime/keylime
 Project-URL: Documentation, https://keylime.readthedocs.io/en/latest/
```

### Comparing `keylime-6.8.0/README.md` & `keylime-7.0.0/README.md`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/agentstates.py` & `keylime-7.0.0/keylime/agentstates.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/api_version.py` & `keylime-7.0.0/keylime/api_version.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/backport_dataclasses.py` & `keylime-7.0.0/keylime/backport_dataclasses.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/ca_impl_openssl.py` & `keylime-7.0.0/keylime/ca_impl_openssl.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/ca_util.py` & `keylime-7.0.0/keylime/ca_util.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/cert_utils.py` & `keylime-7.0.0/keylime/cert_utils.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/cli/options.py` & `keylime-7.0.0/keylime/cli/options.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/cli/policies.py` & `keylime-7.0.0/keylime/cli/policies.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/cloud_verifier_common.py` & `keylime-7.0.0/keylime/cloud_verifier_common.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/cloud_verifier_tornado.py` & `keylime-7.0.0/keylime/cloud_verifier_tornado.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/cmd/convert_config.py` & `keylime-7.0.0/keylime/cmd/convert_config.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/cmd/convert_runtime_policy.py` & `keylime-7.0.0/keylime/cmd/convert_runtime_policy.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/cmd/create_policy.py` & `keylime-7.0.0/keylime/cmd/create_policy.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/cmd/registrar.py` & `keylime-7.0.0/keylime/cmd/registrar.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/cmd/sign_runtime_policy.py` & `keylime-7.0.0/keylime/cmd/sign_runtime_policy.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/cmd/user_data_encrypt.py` & `keylime-7.0.0/keylime/cmd/user_data_encrypt.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/cmd/verifier.py` & `keylime-7.0.0/keylime/cmd/verifier.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/cmd_exec.py` & `keylime-7.0.0/keylime/cmd_exec.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/common/algorithms.py` & `keylime-7.0.0/keylime/common/algorithms.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/common/migrations.py` & `keylime-7.0.0/keylime/common/migrations.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/common/states.py` & `keylime-7.0.0/keylime/common/states.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/common/validators.py` & `keylime-7.0.0/keylime/common/validators.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/common/version.py` & `keylime-7.0.0/keylime/common/version.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/config.py` & `keylime-7.0.0/keylime/config.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/crypto.py` & `keylime-7.0.0/keylime/crypto.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/da/attest.py` & `keylime-7.0.0/keylime/da/attest.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/da/examples/file.py` & `keylime-7.0.0/keylime/da/examples/file.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/da/examples/redis.py` & `keylime-7.0.0/keylime/da/examples/redis.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/da/examples/rekor.py` & `keylime-7.0.0/keylime/da/examples/rekor.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/da/examples/sqldb.py` & `keylime-7.0.0/keylime/da/examples/sqldb.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/da/examples/tsa_rfc3161.py` & `keylime-7.0.0/keylime/da/examples/tsa_rfc3161.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/da/record.py` & `keylime-7.0.0/keylime/da/record.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/db/keylime_db.py` & `keylime-7.0.0/keylime/db/keylime_db.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/db/registrar_db.py` & `keylime-7.0.0/keylime/db/registrar_db.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/db/verifier_db.py` & `keylime-7.0.0/keylime/db/verifier_db.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/dsse/dsse.py` & `keylime-7.0.0/keylime/dsse/dsse.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/dsse/ecdsa.py` & `keylime-7.0.0/keylime/dsse/ecdsa.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/dsse/x509.py` & `keylime-7.0.0/keylime/dsse/x509.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/elchecking/__main__.py` & `keylime-7.0.0/keylime/elchecking/__main__.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/elchecking/example.py` & `keylime-7.0.0/keylime/elchecking/example.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/elchecking/policies.py` & `keylime-7.0.0/keylime/elchecking/policies.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/elchecking/tests.py` & `keylime-7.0.0/keylime/elchecking/tests.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/failure.py` & `keylime-7.0.0/keylime/failure.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/ima/ast.py` & `keylime-7.0.0/keylime/ima/ast.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/ima/dm_grammar.py` & `keylime-7.0.0/keylime/ima/dm_grammar.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/ima/file_signatures.py` & `keylime-7.0.0/keylime/ima/file_signatures.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/ima/ima.py` & `keylime-7.0.0/keylime/ima/ima.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/ima/ima_dm.py` & `keylime-7.0.0/keylime/ima/ima_dm.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/ima/ima_test.py` & `keylime-7.0.0/keylime/ima/ima_test.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/ima/types.py` & `keylime-7.0.0/keylime/ima/types.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/json.py` & `keylime-7.0.0/keylime/json.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/keylime_logging.py` & `keylime-7.0.0/keylime/keylime_logging.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/measured_boot.py` & `keylime-7.0.0/keylime/measured_boot.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/migrations/alembic.ini` & `keylime-7.0.0/keylime/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/migrations/env.py` & `keylime-7.0.0/keylime/migrations/env.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/migrations/versions/039322ea079b_add_generator_column.py` & `keylime-7.0.0/keylime/migrations/versions/039322ea079b_add_generator_column.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/migrations/versions/1ac1513ef2a1_fix_mb_and_ima_column_types.py` & `keylime-7.0.0/keylime/migrations/versions/1ac1513ef2a1_fix_mb_and_ima_column_types.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/migrations/versions/257fe0f0c039_add_fields_for_revocation_context_to_.py` & `keylime-7.0.0/keylime/migrations/versions/257fe0f0c039_add_fields_for_revocation_context_to_.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/migrations/versions/2fbc0fb8fa4d_add_checksum_to_allowlist.py` & `keylime-7.0.0/keylime/migrations/versions/2fbc0fb8fa4d_add_checksum_to_allowlist.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/migrations/versions/4089e1c79be9_add_tpm_clockinfo.py` & `keylime-7.0.0/keylime/migrations/versions/4089e1c79be9_add_tpm_clockinfo.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/migrations/versions/4329e2d14944_associate_moved_allowlists_to_agents.py` & `keylime-7.0.0/keylime/migrations/versions/4329e2d14944_associate_moved_allowlists_to_agents.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/migrations/versions/63c30820fdc1_add_mtls_cert_and_ak_to_verifier_db.py` & `keylime-7.0.0/keylime/migrations/versions/63c30820fdc1_add_mtls_cert_and_ak_to_verifier_db.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/migrations/versions/7d5db1a6ffb0_add_agentstates_columns.py` & `keylime-7.0.0/keylime/migrations/versions/7d5db1a6ffb0_add_agentstates_columns.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/migrations/versions/8a44a4364f5a_initial_database_migration.py` & `keylime-7.0.0/keylime/migrations/versions/8a44a4364f5a_initial_database_migration.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/migrations/versions/8c0f8ded1f90_convert_allowlists_to_ima_policies.py` & `keylime-7.0.0/keylime/migrations/versions/8c0f8ded1f90_convert_allowlists_to_ima_policies.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/migrations/versions/8da20383f6e1_extend_ip_field.py` & `keylime-7.0.0/keylime/migrations/versions/8da20383f6e1_extend_ip_field.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/migrations/versions/9169f80345ed_add_supported_version_to_verifiermain_.py` & `keylime-7.0.0/keylime/migrations/versions/9169f80345ed_add_supported_version_to_verifiermain_.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/migrations/versions/a09cc94177f0_add_last_received_quote.py` & `keylime-7.0.0/keylime/migrations/versions/a09cc94177f0_add_last_received_quote.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/migrations/versions/a72aec03d720_migrate_allowlists_to_separate_table.py` & `keylime-7.0.0/keylime/migrations/versions/a72aec03d720_migrate_allowlists_to_separate_table.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/migrations/versions/a79c27ec1054_add_mtls_cert_field_to_registrar.py` & `keylime-7.0.0/keylime/migrations/versions/a79c27ec1054_add_mtls_cert_field_to_registrar.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/migrations/versions/a7a64155ab3a_add_ima_filesigning_keys_column.py` & `keylime-7.0.0/keylime/migrations/versions/a7a64155ab3a_add_ima_filesigning_keys_column.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/migrations/versions/ae898986c6e9_add_mb_refstate_column.py` & `keylime-7.0.0/keylime/migrations/versions/ae898986c6e9_add_mb_refstate_column.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/migrations/versions/b4d024197413_add_verfier_id_to_verifiermain_table.py` & `keylime-7.0.0/keylime/migrations/versions/b4d024197413_add_verfier_id_to_verifiermain_table.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/migrations/versions/bc3b6b551b0a_drop_vtpm_colums.py` & `keylime-7.0.0/keylime/migrations/versions/bc3b6b551b0a_drop_vtpm_colums.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/migrations/versions/bf48e0c4751d_add_attestation_count_column.py` & `keylime-7.0.0/keylime/migrations/versions/bf48e0c4751d_add_attestation_count_column.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/migrations/versions/c3842cc9ee69_store_keyrings_learned_from_ima_log.py` & `keylime-7.0.0/keylime/migrations/versions/c3842cc9ee69_store_keyrings_learned_from_ima_log.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/migrations/versions/cc2630851a1f_receive_the_aik_tpm_from_the_agent.py` & `keylime-7.0.0/keylime/migrations/versions/cc2630851a1f_receive_the_aik_tpm_from_the_agent.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/migrations/versions/eb869a77abd1_create_allowlist_table.py` & `keylime-7.0.0/keylime/migrations/versions/eb869a77abd1_create_allowlist_table.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/migrations/versions/eeb702f77d7d_allowlist_rename.py` & `keylime-7.0.0/keylime/migrations/versions/eeb702f77d7d_allowlist_rename.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/migrations/versions/f35cdd35eb83_move_v_tpm_policy_to_jsonpickletype.py` & `keylime-7.0.0/keylime/migrations/versions/f35cdd35eb83_move_v_tpm_policy_to_jsonpickletype.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/migrations/versions/f82c4252bc4f_add_ip_and_port_to_registrar.py` & `keylime-7.0.0/keylime/migrations/versions/f82c4252bc4f_add_ip_and_port_to_registrar.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/migrations/versions/f838d3cdeead_add_last_successful_attestation.py` & `keylime-7.0.0/keylime/migrations/versions/f838d3cdeead_add_last_successful_attestation.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/registrar_client.py` & `keylime-7.0.0/keylime/registrar_client.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/registrar_common.py` & `keylime-7.0.0/keylime/registrar_common.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/requests_client.py` & `keylime-7.0.0/keylime/requests_client.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/revocation_notifier.py` & `keylime-7.0.0/keylime/revocation_notifier.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/signing.py` & `keylime-7.0.0/keylime/signing.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/tenant.py` & `keylime-7.0.0/keylime/tenant.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/tornado_requests.py` & `keylime-7.0.0/keylime/tornado_requests.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/tpm/tpm2_objects.py` & `keylime-7.0.0/keylime/tpm/tpm2_objects.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/tpm/tpm2_objects_test.py` & `keylime-7.0.0/keylime/tpm/tpm2_objects_test.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/tpm/tpm_abstract.py` & `keylime-7.0.0/keylime/tpm/tpm_abstract.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/tpm/tpm_main.py` & `keylime-7.0.0/keylime/tpm/tpm_main.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/tpm_bootlog_enrich.py` & `keylime-7.0.0/keylime/tpm_bootlog_enrich.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime/web_util.py` & `keylime-7.0.0/keylime/web_util.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime.egg-info/PKG-INFO` & `keylime-7.0.0/keylime.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keylime
-Version: 6.8.0
+Version: 7.0.0
 Summary: TPM-based key bootstrapping and system integrity measurement system for cloud
 Home-page: https://keylime.dev
 Author: Keylime Community
 Author-email: keylime@groups.io
 License: Apache-2.0
 Project-URL: Source, https://github.com/keylime/keylime
 Project-URL: Documentation, https://keylime.readthedocs.io/en/latest/
```

### Comparing `keylime-6.8.0/keylime.egg-info/SOURCES.txt` & `keylime-7.0.0/keylime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/keylime.egg-info/entry_points.txt` & `keylime-7.0.0/keylime.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/pyproject.toml` & `keylime-7.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/setup.cfg` & `keylime-7.0.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = keylime
-version = 6.8.0
+version = 7.0.0
 description = TPM-based key bootstrapping and system integrity measurement system for cloud
 long_description = file: _pypi-notice.md, README.md
 long_description_content_type = text/markdown; charset=UTF-8
 url = https://keylime.dev
 author = Keylime Community
 author_email = keylime@groups.io
 license = Apache-2.0
```

### Comparing `keylime-6.8.0/setup.py` & `keylime-7.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/templates/2.0/adjust.py` & `keylime-7.0.0/templates/2.0/adjust.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/templates/2.0/agent.j2` & `keylime-7.0.0/templates/2.0/agent.j2`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/templates/2.0/ca.j2` & `keylime-7.0.0/templates/2.0/ca.j2`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/templates/2.0/logging.j2` & `keylime-7.0.0/templates/2.0/logging.j2`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/templates/2.0/mapping.json` & `keylime-7.0.0/templates/2.0/mapping.json`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/templates/2.0/registrar.j2` & `keylime-7.0.0/templates/2.0/registrar.j2`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/templates/2.0/tenant.j2` & `keylime-7.0.0/templates/2.0/tenant.j2`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/templates/2.0/verifier.j2` & `keylime-7.0.0/templates/2.0/verifier.j2`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/test/test_algorithms.py` & `keylime-7.0.0/test/test_algorithms.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/test/test_api_version.py` & `keylime-7.0.0/test/test_api_version.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/test/test_ca_impl_openssl.py` & `keylime-7.0.0/test/test_ca_impl_openssl.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/test/test_ca_util.py` & `keylime-7.0.0/test/test_ca_util.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/test/test_cert_utils.py` & `keylime-7.0.0/test/test_cert_utils.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/test/test_config.py` & `keylime-7.0.0/test/test_config.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/test/test_convert_config.py` & `keylime-7.0.0/test/test_convert_config.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/test/test_crypto.py` & `keylime-7.0.0/test/test_crypto.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/test/test_fs_util.py` & `keylime-7.0.0/test/test_fs_util.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/test/test_ima_ast.py` & `keylime-7.0.0/test/test_ima_ast.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/test/test_ima_dm.py` & `keylime-7.0.0/test/test_ima_dm.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/test/test_ima_verification.py` & `keylime-7.0.0/test/test_ima_verification.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/test/test_json.py` & `keylime-7.0.0/test/test_json.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/test/test_policy_conversion.py` & `keylime-7.0.0/test/test_policy_conversion.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/test/test_registrar_db.py` & `keylime-7.0.0/test/test_registrar_db.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/test/test_retry_algo.py` & `keylime-7.0.0/test/test_retry_algo.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/test/test_signing.py` & `keylime-7.0.0/test/test_signing.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/test/test_tpm.py` & `keylime-7.0.0/test/test_tpm.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/test/test_validators.py` & `keylime-7.0.0/test/test_validators.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/test/test_verifier_db.py` & `keylime-7.0.0/test/test_verifier_db.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/test/test_version.py` & `keylime-7.0.0/test/test_version.py`

 * *Files identical despite different names*

### Comparing `keylime-6.8.0/test/test_web_util.py` & `keylime-7.0.0/test/test_web_util.py`

 * *Files identical despite different names*

