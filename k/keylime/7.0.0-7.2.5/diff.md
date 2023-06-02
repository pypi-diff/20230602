# Comparing `tmp/keylime-7.0.0.tar.gz` & `tmp/keylime-7.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keylime-7.0.0.tar", last modified: Tue Apr 25 19:22:05 2023, max compression
+gzip compressed data, was "keylime-7.2.5.tar", last modified: Fri Jun  2 17:22:59 2023, max compression
```

## Comparing `keylime-7.0.0.tar` & `keylime-7.2.5.tar`

### file list

```diff
@@ -1,179 +1,186 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:22:05.163835 keylime-7.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-25 19:21:53.000000 keylime-7.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-25 19:21:53.000000 keylime-7.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-04-25 19:22:05.163835 keylime-7.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11220 2023-04-25 19:21:53.000000 keylime-7.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-25 19:21:53.000000 keylime-7.0.0/_pypi-notice.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:22:05.119835 keylime-7.0.0/keylime/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8609 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/agentstates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/api_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    45700 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/backport_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/ca_impl_openssl.py
--rw-r--r--   0 runner    (1001) docker     (123)    15541 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/ca_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/cert_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:22:05.119835 keylime-7.0.0/keylime/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/cli/policies.py
--rw-r--r--   0 runner    (1001) docker     (123)    12967 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/cloud_verifier_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    68876 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/cloud_verifier_tornado.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:22:05.123835 keylime-7.0.0/keylime/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/cmd/attest.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/cmd/ca.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20465 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/cmd/convert_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8890 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/cmd/convert_runtime_policy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22220 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/cmd/create_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/cmd/registrar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/cmd/sign_runtime_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/cmd/tenant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/cmd/user_data_encrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/cmd/verifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/cmd_exec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:22:05.127836 keylime-7.0.0/keylime/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/common/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/common/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/common/migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/common/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/common/states.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/common/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/common/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16220 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:22:05.127836 keylime-7.0.0/keylime/da/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/da/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/da/attest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:22:05.131836 keylime-7.0.0/keylime/da/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/da/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/da/examples/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/da/examples/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/da/examples/rekor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/da/examples/sqldb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/da/examples/tsa_rfc3161.py
--rw-r--r--   0 runner    (1001) docker     (123)    16781 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/da/record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:22:05.131836 keylime-7.0.0/keylime/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/db/keylime_db.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/db/registrar_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/db/verifier_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:22:05.131836 keylime-7.0.0/keylime/dsse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/dsse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/dsse/dsse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/dsse/ecdsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/dsse/x509.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:22:05.131836 keylime-7.0.0/keylime/elchecking/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/elchecking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/elchecking/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17614 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/elchecking/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/elchecking/policies.py
--rw-r--r--   0 runner    (1001) docker     (123)    24307 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/elchecking/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/failure.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/fs_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:22:05.135836 keylime-7.0.0/keylime/ima/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/ima/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14117 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/ima/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/ima/dm_grammar.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18471 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/ima/file_signatures.py
--rw-r--r--   0 runner    (1001) docker     (123)    24445 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/ima/ima.py
--rw-r--r--   0 runner    (1001) docker     (123)    32160 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/ima/ima_dm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/ima/ima_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/ima/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/ip_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/keylime_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/measured_boot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:22:05.135836 keylime-7.0.0/keylime/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:22:05.147836 keylime-7.0.0/keylime/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/039322ea079b_add_generator_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/1ac1513ef2a1_fix_mb_and_ima_column_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/257fe0f0c039_add_fields_for_revocation_context_to_.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/2fbc0fb8fa4d_add_checksum_to_allowlist.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/4089e1c79be9_add_tpm_clockinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/4329e2d14944_associate_moved_allowlists_to_agents.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/63c30820fdc1_add_mtls_cert_and_ak_to_verifier_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/7d5db1a6ffb0_add_agentstates_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/8a44a4364f5a_initial_database_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/8c0f8ded1f90_convert_allowlists_to_ima_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/8da20383f6e1_extend_ip_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/9169f80345ed_add_supported_version_to_verifiermain_.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/a09cc94177f0_add_last_received_quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/a72aec03d720_migrate_allowlists_to_separate_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/a79c27ec1054_add_mtls_cert_field_to_registrar.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/a7a64155ab3a_add_ima_filesigning_keys_column.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/ae898986c6e9_add_mb_refstate_column.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/b4d024197413_add_verfier_id_to_verifiermain_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/bc3b6b551b0a_drop_vtpm_colums.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/bf48e0c4751d_add_attestation_count_column.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/c3842cc9ee69_store_keyrings_learned_from_ima_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/cc2630851a1f_receive_the_aik_tpm_from_the_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/eb869a77abd1_create_allowlist_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/eeb702f77d7d_allowlist_rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/f35cdd35eb83_move_v_tpm_policy_to_jsonpickletype.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/f82c4252bc4f_add_ip_and_port_to_registrar.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/migrations/versions/f838d3cdeead_add_last_successful_attestation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/registrar_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23297 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/registrar_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/requests_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/revocation_notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/signing.py
--rw-r--r--   0 runner    (1001) docker     (123)    74195 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/tenant.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/tornado_requests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:22:05.151836 keylime-7.0.0/keylime/tpm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/tpm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12250 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/tpm/tpm2_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    17761 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/tpm/tpm2_objects_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/tpm/tpm_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    29642 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/tpm/tpm_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/tpm_bootlog_enrich.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/tpm_ek_ca.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    17135 2023-04-25 19:21:53.000000 keylime-7.0.0/keylime/web_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:22:05.119835 keylime-7.0.0/keylime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12665 2023-04-25 19:22:05.000000 keylime-7.0.0/keylime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-04-25 19:22:05.000000 keylime-7.0.0/keylime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 19:22:05.000000 keylime-7.0.0/keylime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-25 19:22:05.000000 keylime-7.0.0/keylime.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 19:22:04.000000 keylime-7.0.0/keylime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-25 19:22:05.000000 keylime-7.0.0/keylime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-25 19:21:53.000000 keylime-7.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-25 19:22:05.163835 keylime-7.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-25 19:21:53.000000 keylime-7.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:22:05.111836 keylime-7.0.0/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:22:05.155835 keylime-7.0.0/templates/2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-04-25 19:21:53.000000 keylime-7.0.0/templates/2.0/adjust.py
--rw-r--r--   0 runner    (1001) docker     (123)     8390 2023-04-25 19:21:53.000000 keylime-7.0.0/templates/2.0/agent.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-25 19:21:53.000000 keylime-7.0.0/templates/2.0/ca.j2
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-25 19:21:53.000000 keylime-7.0.0/templates/2.0/logging.j2
--rw-r--r--   0 runner    (1001) docker     (123)    26831 2023-04-25 19:21:53.000000 keylime-7.0.0/templates/2.0/mapping.json
--rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-04-25 19:21:53.000000 keylime-7.0.0/templates/2.0/registrar.j2
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-04-25 19:21:53.000000 keylime-7.0.0/templates/2.0/tenant.j2
--rw-r--r--   0 runner    (1001) docker     (123)    11233 2023-04-25 19:21:53.000000 keylime-7.0.0/templates/2.0/verifier.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:22:05.163835 keylime-7.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_api_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_ca_impl_openssl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_ca_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_cert_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18107 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_convert_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_fs_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_ima_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)    23474 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_ima_dm.py
--rw-r--r--   0 runner    (1001) docker     (123)    20101 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_ima_verification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_policy_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     7349 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_registrar_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_retry_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_signing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_tpm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)    11601 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_verifier_db.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-25 19:21:53.000000 keylime-7.0.0/test/test_web_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:59.465957 keylime-7.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-02 17:22:46.000000 keylime-7.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-02 17:22:46.000000 keylime-7.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12722 2023-06-02 17:22:59.465957 keylime-7.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-06-02 17:22:46.000000 keylime-7.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-02 17:22:46.000000 keylime-7.2.5/_pypi-notice.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:59.445955 keylime-7.2.5/keylime/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/agentstates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/api_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45700 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/backport_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/ca_impl_openssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15559 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/ca_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/cert_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:59.449956 keylime-7.2.5/keylime/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/cli/policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12911 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/cloud_verifier_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65426 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/cloud_verifier_tornado.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:59.449956 keylime-7.2.5/keylime/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/cmd/attest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/cmd/ca.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20465 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/cmd/convert_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8890 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/cmd/convert_runtime_policy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22220 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/cmd/create_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/cmd/registrar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/cmd/sign_runtime_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/cmd/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/cmd/user_data_encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/cmd/verifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/cmd_exec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:59.449956 keylime-7.2.5/keylime/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/common/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/common/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/common/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/common/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/common/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/common/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/common/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16220 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6834 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:59.453956 keylime-7.2.5/keylime/da/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/da/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/da/attest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:59.453956 keylime-7.2.5/keylime/da/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/da/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/da/examples/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/da/examples/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/da/examples/rekor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/da/examples/sqldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/da/examples/tsa_rfc3161.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16781 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/da/record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:59.453956 keylime-7.2.5/keylime/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/db/keylime_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/db/registrar_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/db/verifier_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:59.453956 keylime-7.2.5/keylime/dsse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/dsse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/dsse/dsse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/dsse/ecdsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/dsse/x509.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/failure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/fs_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:59.453956 keylime-7.2.5/keylime/ima/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/ima/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/ima/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/ima/dm_grammar.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18388 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/ima/file_signatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24265 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/ima/ima.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32160 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/ima/ima_dm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/ima/ima_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/ima/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/ip_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/keylime_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:59.453956 keylime-7.2.5/keylime/mba/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/mba/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:59.457956 keylime-7.2.5/keylime/mba/elchecking/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/mba/elchecking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/mba/elchecking/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17614 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/mba/elchecking/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/mba/elchecking/mbpolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/mba/elchecking/policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24213 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/mba/elchecking/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/mba/mba.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:59.457956 keylime-7.2.5/keylime/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:59.461957 keylime-7.2.5/keylime/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/039322ea079b_add_generator_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/1ac1513ef2a1_fix_mb_and_ima_column_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/257fe0f0c039_add_fields_for_revocation_context_to_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/2fbc0fb8fa4d_add_checksum_to_allowlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/4089e1c79be9_add_tpm_clockinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/4329e2d14944_associate_moved_allowlists_to_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/63c30820fdc1_add_mtls_cert_and_ak_to_verifier_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/7d5db1a6ffb0_add_agentstates_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/8a44a4364f5a_initial_database_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/8c0f8ded1f90_convert_allowlists_to_ima_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/8da20383f6e1_extend_ip_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/9169f80345ed_add_supported_version_to_verifiermain_.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/a09cc94177f0_add_last_received_quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/a72aec03d720_migrate_allowlists_to_separate_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/a79c27ec1054_add_mtls_cert_field_to_registrar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/a7a64155ab3a_add_ima_filesigning_keys_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/ae898986c6e9_add_mb_refstate_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/b4d024197413_add_verfier_id_to_verifiermain_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/bc3b6b551b0a_drop_vtpm_colums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/bf48e0c4751d_add_attestation_count_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/c3842cc9ee69_store_keyrings_learned_from_ima_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/cc2630851a1f_receive_the_aik_tpm_from_the_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/eb869a77abd1_create_allowlist_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/eeb702f77d7d_allowlist_rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/f35cdd35eb83_move_v_tpm_policy_to_jsonpickletype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/f82c4252bc4f_add_ip_and_port_to_registrar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/migrations/versions/f838d3cdeead_add_last_successful_attestation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/registrar_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20949 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/registrar_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/requests_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/revocation_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/signing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74523 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/tornado_requests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:59.461957 keylime-7.2.5/keylime/tpm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/tpm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/tpm/ec_crypto_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16134 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/tpm/tpm2_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18898 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/tpm/tpm2_objects_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/tpm/tpm_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31669 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/tpm/tpm_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15091 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/tpm/tpm_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/tpm/tpm_util_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/tpm/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/tpm_bootlog_enrich.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/tpm_ek_ca.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-06-02 17:22:46.000000 keylime-7.2.5/keylime/web_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:59.449956 keylime-7.2.5/keylime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12722 2023-06-02 17:22:59.000000 keylime-7.2.5/keylime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-06-02 17:22:59.000000 keylime-7.2.5/keylime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 17:22:59.000000 keylime-7.2.5/keylime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-02 17:22:59.000000 keylime-7.2.5/keylime.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 17:22:59.000000 keylime-7.2.5/keylime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 17:22:59.000000 keylime-7.2.5/keylime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-02 17:22:46.000000 keylime-7.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-02 17:22:59.469957 keylime-7.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-02 17:22:46.000000 keylime-7.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:59.441955 keylime-7.2.5/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:59.461957 keylime-7.2.5/templates/2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-06-02 17:22:46.000000 keylime-7.2.5/templates/2.0/adjust.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8390 2023-06-02 17:22:46.000000 keylime-7.2.5/templates/2.0/agent.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-02 17:22:46.000000 keylime-7.2.5/templates/2.0/ca.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-02 17:22:46.000000 keylime-7.2.5/templates/2.0/logging.j2
+-rw-r--r--   0 runner    (1001) docker     (123)    26831 2023-06-02 17:22:46.000000 keylime-7.2.5/templates/2.0/mapping.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-06-02 17:22:46.000000 keylime-7.2.5/templates/2.0/registrar.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-06-02 17:22:46.000000 keylime-7.2.5/templates/2.0/tenant.j2
+-rw-r--r--   0 runner    (1001) docker     (123)    11233 2023-06-02 17:22:46.000000 keylime-7.2.5/templates/2.0/verifier.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:22:59.465957 keylime-7.2.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_api_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_ca_impl_openssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_ca_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8792 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_cert_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18107 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_convert_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_fs_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_ima_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23987 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_ima_dm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20078 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_ima_verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_policy_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7349 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_registrar_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_retry_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_signing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_tpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11601 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_verifier_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-02 17:22:46.000000 keylime-7.2.5/test/test_web_util.py
```

### Comparing `keylime-7.0.0/LICENSE` & `keylime-7.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/PKG-INFO` & `keylime-7.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keylime
-Version: 7.0.0
+Version: 7.2.5
 Summary: TPM-based key bootstrapping and system integrity measurement system for cloud
 Home-page: https://keylime.dev
 Author: Keylime Community
 Author-email: keylime@groups.io
 License: Apache-2.0
 Project-URL: Source, https://github.com/keylime/keylime
 Project-URL: Documentation, https://keylime.readthedocs.io/en/latest/
@@ -178,15 +178,15 @@
 ## Systemd service support
 
 The directory `services/` includes `systemd` service files for the verifier,
 agent and registrar.
 
 You can install the services with the following command:
 
-`sudo ./services/install.sh`
+`sudo ./services/installer.sh`
 
 Once installed, you can run and inspect the services `keylime_verifier` and `keylime_registrar` via `systemctl`.
 The Rust agent repository also contains a systemd service file for the agent.
 
 ## Request a feature
 
 Keylime feature requests are tracked as enhancements in the [enhancements repository](https://github.com/keylime/enhancements)
@@ -233,15 +233,15 @@
 * Executive summary Keylime slides: [docs/old/keylime-elevator-slides.pptx](https://github.com/keylime/keylime/raw/master/docs/old/keylime-elevator-slides.pptx)
 * Detailed Keylime Architecture slides: [docs/old/keylime-detailed-architecture-v7.pptx](https://github.com/keylime/keylime/raw/master/docs/old/keylime-detailed-architecture-v7.pptx)
 * See ACSAC 2016 paper in doc directory: [docs/old/tci-acm.pdf](https://github.com/keylime/keylime/blob/master/docs/old/tci-acm.pdf)
   * and the ACSAC presentation on Keylime: [docs/old/llsrc-keylime-acsac-v6.pptx](https://github.com/keylime/keylime/raw/master/docs/old/llsrc-keylime-acsac-v6.pptx)
 * See the HotCloud 2018 paper: [docs/old/hotcloud18.pdf](https://github.com/keylime/keylime/blob/master/docs/old/hotcloud18.pdf)
 * Details about Keylime REST API: [docs/old/keylime RESTful API.docx](https://github.com/keylime/keylime/raw/master/docs/old/keylime%20RESTful%20API.docx)
 * [Demo files](demo/) - Some pre-packaged demos to show off what Keylime can do.
-* [IMA stub service](ima_stub_service/) - Allows you to test IMA and Keylime on a machine without a TPM.  Service keeps emulated TPM synchronized with IMA.
+* [IMA stub service](https://github.com/keylime/rust-keylime/tree/master/keylime-ima-emulator) - Allows you to test IMA and Keylime on a machine without a TPM.  Service keeps emulated TPM synchronized with IMA.
 
 #### Errata from the ACSAC Paper
 
 We discovered a typo in Figure 5 of the published ACSAC paper. The final interaction
 between the Tenant and Cloud Verifier showed an HMAC of the node's ID using the key
 K_e.  This should be using K_b. The paper in this repository and the ACSAC presentation
 have been updated to correct this typo.
```

### Comparing `keylime-7.0.0/README.md` & `keylime-7.2.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -145,15 +145,15 @@
 ## Systemd service support
 
 The directory `services/` includes `systemd` service files for the verifier,
 agent and registrar.
 
 You can install the services with the following command:
 
-`sudo ./services/install.sh`
+`sudo ./services/installer.sh`
 
 Once installed, you can run and inspect the services `keylime_verifier` and `keylime_registrar` via `systemctl`.
 The Rust agent repository also contains a systemd service file for the agent.
 
 ## Request a feature
 
 Keylime feature requests are tracked as enhancements in the [enhancements repository](https://github.com/keylime/enhancements)
@@ -200,15 +200,15 @@
 * Executive summary Keylime slides: [docs/old/keylime-elevator-slides.pptx](https://github.com/keylime/keylime/raw/master/docs/old/keylime-elevator-slides.pptx)
 * Detailed Keylime Architecture slides: [docs/old/keylime-detailed-architecture-v7.pptx](https://github.com/keylime/keylime/raw/master/docs/old/keylime-detailed-architecture-v7.pptx)
 * See ACSAC 2016 paper in doc directory: [docs/old/tci-acm.pdf](https://github.com/keylime/keylime/blob/master/docs/old/tci-acm.pdf)
   * and the ACSAC presentation on Keylime: [docs/old/llsrc-keylime-acsac-v6.pptx](https://github.com/keylime/keylime/raw/master/docs/old/llsrc-keylime-acsac-v6.pptx)
 * See the HotCloud 2018 paper: [docs/old/hotcloud18.pdf](https://github.com/keylime/keylime/blob/master/docs/old/hotcloud18.pdf)
 * Details about Keylime REST API: [docs/old/keylime RESTful API.docx](https://github.com/keylime/keylime/raw/master/docs/old/keylime%20RESTful%20API.docx)
 * [Demo files](demo/) - Some pre-packaged demos to show off what Keylime can do.
-* [IMA stub service](ima_stub_service/) - Allows you to test IMA and Keylime on a machine without a TPM.  Service keeps emulated TPM synchronized with IMA.
+* [IMA stub service](https://github.com/keylime/rust-keylime/tree/master/keylime-ima-emulator) - Allows you to test IMA and Keylime on a machine without a TPM.  Service keeps emulated TPM synchronized with IMA.
 
 #### Errata from the ACSAC Paper
 
 We discovered a typo in Figure 5 of the published ACSAC paper. The final interaction
 between the Tenant and Cloud Verifier showed an HMAC of the node's ID using the key
 K_e.  This should be using K_b. The paper in this repository and the ACSAC presentation
 have been updated to correct this typo.
```

### Comparing `keylime-7.0.0/keylime/agentstates.py` & `keylime-7.2.5/keylime/agentstates.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import sys
 import threading
-from typing import Any, Dict, Optional, Set
+from typing import Dict, Optional, Set
 
 from keylime.common.algorithms import Hash
-from keylime.ima.ast import get_FF_HASH, get_START_HASH
 from keylime.ima.file_signatures import ImaKeyrings
 
 if sys.version_info >= (3, 7):
     from dataclasses import dataclass
 else:
     from keylime.backport_dataclasses import dataclass
 
@@ -16,36 +15,29 @@
 class TPMClockInfo:
     clock: int
     resetcount: int
     restartcount: int
     safe: int
 
     @classmethod
-    def from_dict(cls, data: Dict[str, Any]) -> "TPMClockInfo":
-        dclki: Dict[str, int] = {}
-        if "clockInfo" in data:
-            dclki = data["clockInfo"]
-
-        if "clock" in data:
-            dclki = data
-
+    def from_dict(cls, dclki: Dict[str, int]) -> "TPMClockInfo":
         return cls(
             clock=dclki.get("clock", 0),
             resetcount=dclki.get("resetCount", 0),
             restartcount=dclki.get("restartCount", 0),
             safe=dclki.get("safe", 1),
         )
 
     def to_dict(self) -> Dict[str, int]:
-        data = {}
-        data["clock"] = self.clock
-        data["resetCount"] = self.resetcount
-        data["restartCount"] = self.restartcount
-        data["safe"] = self.safe
-        return data
+        return {
+            "clock": self.clock,
+            "resetCount": self.resetcount,
+            "restartCount": self.restartcount,
+            "safe": self.safe,
+        }
 
 
 class TPMState:
     """TPMState models the state of the TPM's PCRs"""
 
     pcrs: Dict[int, Optional[bytes]]
     hash_alg: Dict[int, Hash]
@@ -60,17 +52,17 @@
     def init_pcr(self, pcr_num: int, hash_alg: Hash) -> None:
         """Initializes a PCR"""
         if pcr_num not in self.hash_alg:
             self.hash_alg[pcr_num] = hash_alg
 
         if self.pcrs[pcr_num] is None:
             if 17 <= pcr_num <= 23:
-                self.pcrs[pcr_num] = get_FF_HASH(self.hash_alg[pcr_num])
+                self.pcrs[pcr_num] = self.hash_alg[pcr_num].get_ff_hash()
             else:
-                self.pcrs[pcr_num] = get_START_HASH(self.hash_alg[pcr_num])
+                self.pcrs[pcr_num] = self.hash_alg[pcr_num].get_start_hash()
 
     def reset_pcr(self, pcr_num: int) -> None:
         """Reset a specific PCR"""
         self.pcrs[pcr_num] = None
 
     def get_pcr(self, pcr_num: int) -> Optional[bytes]:
         """
```

### Comparing `keylime-7.0.0/keylime/api_version.py` & `keylime-7.2.5/keylime/api_version.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/backport_dataclasses.py` & `keylime-7.2.5/keylime/backport_dataclasses.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/ca_impl_openssl.py` & `keylime-7.2.5/keylime/ca_impl_openssl.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/ca_util.py` & `keylime-7.2.5/keylime/ca_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -360,15 +360,15 @@
     if os.path.exists("private.yml"):
         with open("private.yml", encoding="utf-8") as f:
             toread = yaml.load(f, Loader=SafeLoader)
         assert isinstance(global_password, str)
         key = crypto.kdf(global_password, toread["salt"])
         try:
             plain = crypto.decrypt(toread["priv"], key)
-        except ValueError as e:
+        except crypto_exceptions.InvalidTag as e:
             raise Exception("Invalid password for keystore") from e
 
         return yaml.load(plain, Loader=SafeLoader), toread["salt"]
 
     if warn:
         # file doesn't exist, just invent a salt
         logger.warning("Private certificate data %s does not exist yet.", os.path.abspath("private.yml"))
```

### Comparing `keylime-7.0.0/keylime/cert_utils.py` & `keylime-7.2.5/keylime/cert_utils.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/cli/options.py` & `keylime-7.2.5/keylime/cli/options.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/cli/policies.py` & `keylime-7.2.5/keylime/cli/policies.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import base64
 import json
 import sys
 from typing import Any, Dict, List, Optional, Tuple
 
-from keylime import config, keylime_logging, measured_boot
+from keylime import config, keylime_logging
 from keylime.cmd import convert_runtime_policy
 from keylime.ima import file_signatures, ima
+from keylime.mba import mba
 from keylime.tpm.tpm_abstract import TPM_Utilities
 
 if sys.version_info >= (3, 8):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
@@ -159,15 +160,15 @@
             tpm_policy["mask"] = hex(int(tpm_policy["mask"], 0) | (1 << _pcr))
 
         logger.info("TPM PCR Mask automatically modified is %s to include IMA/Event log PCRs", tpm_policy["mask"])
 
         if isinstance(args["mb_refstate"], str):
             if args["mb_refstate"] == "default":
                 args["mb_refstate"] = config.get("tenant", "mb_refstate")
-            mb_refstate_data = measured_boot.read_mb_refstate(args["mb_refstate"])
+            mb_refstate_data = mba.load_policy_file(args["mb_refstate"])
         else:
             raise UserError("Invalid measured boot reference state (intended state) provided")
 
     # Set up measured boot (TPM event log) reference state
     if TPM_Utilities.check_mask(tpm_policy["mask"], config.MEASUREDBOOT_PCRS[2]):
         # Process measured boot reference state
         mb_refstate = mb_refstate_data
```

### Comparing `keylime-7.0.0/keylime/cloud_verifier_common.py` & `keylime-7.2.5/keylime/cloud_verifier_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 from keylime.agentstates import AgentAttestState, AgentAttestStates, TPMClockInfo
 from keylime.common import algorithms
 from keylime.db.verifier_db import VerfierMain
 from keylime.failure import Component, Event, Failure
 from keylime.ima import file_signatures
 from keylime.ima.types import RuntimePolicyType
 from keylime.tpm.tpm_abstract import TPM_Utilities
-from keylime.tpm.tpm_main import tpm
+from keylime.tpm.tpm_main import Tpm
 
 # setup logging
 logger = keylime_logging.init_logging("cloudverifier_common")
 
-GLOBAL_TPM_INSTANCE: Optional[tpm] = None
+GLOBAL_TPM_INSTANCE: Optional[Tpm] = None
 DEFAULT_VERIFIER_ID: str = "default"
 
 
-def get_tpm_instance() -> tpm:
+def get_tpm_instance() -> Tpm:
     global GLOBAL_TPM_INSTANCE
     if GLOBAL_TPM_INSTANCE is None:
-        GLOBAL_TPM_INSTANCE = tpm()
+        GLOBAL_TPM_INSTANCE = Tpm()
     return GLOBAL_TPM_INSTANCE
 
 
 def get_AgentAttestStates() -> AgentAttestStates:
     return AgentAttestStates.get_instance()
 
 
@@ -95,53 +95,54 @@
         agent["provide_V"] = False
         received_public_key = agent["public_key"]
 
     hash_alg = json_response.get("hash_alg")
     enc_alg = json_response.get("enc_alg")
     sign_alg = json_response.get("sign_alg")
 
-    # Update chosen tpm and algorithms
-    agent["hash_alg"] = hash_alg
-    agent["enc_alg"] = enc_alg
-    agent["sign_alg"] = sign_alg
-
     # Ensure hash_alg is in accept_tpm_hash_alg list
     if (
         not hash_alg
         or not algorithms.is_accepted(hash_alg, agent["accept_tpm_hash_algs"])
         or not algorithms.Hash.is_recognized(hash_alg)
     ):
         logger.error("TPM Quote for agent %s is using an unaccepted hash algorithm: %s", agent_id, hash_alg)
         failure.add_event(
             "invalid_hash_alg",
             {"message": f"TPM Quote is using an unaccepted hash algorithm: {hash_alg}", "data": hash_alg},
             False,
         )
         return failure
 
+    agent["hash_alg"] = hash_alg
+
     # Ensure enc_alg is in accept_tpm_encryption_algs list
     if not enc_alg or not algorithms.is_accepted(enc_alg, agent["accept_tpm_encryption_algs"]):
         logger.error("TPM Quote for agent %s is using an unaccepted encryption algorithm: %s", agent_id, enc_alg)
         failure.add_event(
             "invalid_enc_alg",
             {"message": f"TPM Quote is using an unaccepted encryption algorithm: {enc_alg}", "data": enc_alg},
             False,
         )
         return failure
 
+    agent["enc_alg"] = enc_alg
+
     # Ensure sign_alg is in accept_tpm_encryption_algs list
     if not sign_alg or not algorithms.is_accepted(sign_alg, agent["accept_tpm_signing_algs"]):
         logger.error("TPM Quote for agent %s is using an unaccepted signing algorithm: %s", agent_id, sign_alg)
         failure.add_event(
             "invalid_sign_alg",
             {"message": f"TPM Quote is using an unaccepted signing algorithm: {sign_alg}", "data": sign_alg},
             False,
         )
         return failure
 
+    agent["sign_alg"] = sign_alg
+
     if ima_measurement_list_entry == 0:
         agentAttestState.reset_ima_attestation()
     elif ima_measurement_list_entry != agentAttestState.get_next_ima_ml_entry():
         # If we requested a particular entry number then the agent must return either
         # starting at 0 (handled above) or with the requested number.
         logger.error(
             "Agent %s did not respond with requested next IMA measurement list entry %s but started at %s",
@@ -252,28 +253,26 @@
         "mask": tpm_policy["mask"],
         "ima_ml_entry": agentAttestState.get_next_ima_ml_entry(),
     }
     return params
 
 
 def process_get_status(agent: VerfierMain) -> Dict[str, Any]:
-    agent_id = agent.agent_id
-
     has_mb_refstate = 0
     try:
         mb_refstate = json.loads(cast(str, agent.mb_refstate))
         if mb_refstate and mb_refstate.keys():
             has_mb_refstate = 1
     except Exception as e:
         logger.warning(
             'Non-fatal problem ocurred while attempting to evaluate agent %s attribute "mb_refstate" (%s). Will just consider the value of this attribute as empty',
-            agent_id,
+            agent.agent_id,
             e.args,
         )
-        logger.debug('The contents of the agent %s attribute "mb_refstate" are %s', agent_id, agent.mb_refstate)
+        logger.debug('The contents of the agent %s attribute "mb_refstate" are %s', agent.agent_id, agent.mb_refstate)
 
     has_runtime_policy = 0
     if agent.ima_policy.generator and agent.ima_policy.generator > 1:
         has_runtime_policy = 1
 
     response = {
         "operational_state": agent.operational_state,
```

### Comparing `keylime-7.0.0/keylime/cloud_verifier_tornado.py` & `keylime-7.2.5/keylime/cloud_verifier_tornado.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 import functools
 import os
 import signal
 import sys
 import traceback
 from concurrent.futures import ThreadPoolExecutor
 from multiprocessing import Process
-from typing import Any, Dict, List, Optional, cast
+from typing import Any, Dict, List, Optional, Tuple, Union, cast
 
 import tornado.httpserver
 import tornado.ioloop
 import tornado.netutil
 import tornado.process
 import tornado.web
 from sqlalchemy.engine import Engine
 from sqlalchemy.exc import SQLAlchemyError
 from sqlalchemy.orm import Session, joinedload
-from sqlalchemy.orm.exc import NoResultFound
+from sqlalchemy.orm.exc import NoResultFound  # pyright: ignore
 
 from keylime import api_version as keylime_api_version
 from keylime import (
     cloud_verifier_common,
     config,
     json,
     keylime_logging,
@@ -31,15 +31,14 @@
     web_util,
 )
 from keylime.agentstates import AgentAttestState, AgentAttestStates
 from keylime.common import retry, states, validators
 from keylime.da import record
 from keylime.db.keylime_db import DBEngineManager, SessionManager
 from keylime.db.verifier_db import VerfierMain, VerifierAllowlist
-from keylime.elchecking import policies
 from keylime.failure import MAX_SEVERITY_LABEL, Component, Event, Failure, set_severity_config
 from keylime.ima import ima
 
 logger = keylime_logging.init_logging("verifier")
 
 GLOBAL_POLICY_CACHE: Dict[str, Dict[str, str]] = {}
 
@@ -293,14 +292,57 @@
         web_util.echo_json_response(self, 405, "Not Implemented: Use GET interface instead")
 
     def data_received(self, chunk: Any) -> None:
         raise NotImplementedError()
 
 
 class AgentsHandler(BaseHandler):
+    def __validate_input(self, method: str) -> Tuple[Optional[Dict[str, Union[str, None]]], Optional[str]]:
+        if self.request.uri is None:
+            web_util.echo_json_response(self, 400, "URI not specified")
+            return None, None
+
+        rest_params = web_util.get_restful_params(self.request.uri)
+        if rest_params is None:
+            web_util.echo_json_response(self, 405, "Not Implemented: Use /agents/ interface")
+            return None, None
+
+        if not web_util.validate_api_version(self, cast(str, rest_params["api_version"]), logger):
+            return None, None
+
+        if "agents" not in rest_params:
+            web_util.echo_json_response(self, 400, "uri not supported")
+            if method != "DELETE":
+                logger.warning("%s returning 400 response. uri not supported: %s", method, self.request.path)
+            return None, None
+
+        agent_id = rest_params["agents"]
+
+        validate_agent_id = False
+        if method == "GET":
+            validate_agent_id = (agent_id is not None) and (agent_id != "")
+        elif method in ["PUT", "DELETE"]:
+            if agent_id is None:
+                web_util.echo_json_response(self, 400, "uri not supported")
+                logger.warning("%s returning 400 response. uri not supported", method)
+                if method == "DELETE":
+                    return None, None
+
+            validate_agent_id = True
+        else:
+            validate_agent_id = agent_id is not None
+
+        # If the agent ID is not valid (wrong set of characters), just do nothing.
+        if validate_agent_id and not validators.valid_agent_id(agent_id):
+            web_util.echo_json_response(self, 400, "agent_id not not valid")
+            logger.error("%s received an invalid agent ID: %s", method, agent_id)
+            return None, None
+
+        return rest_params, agent_id
+
     def head(self) -> None:
         """HEAD not supported"""
         web_util.echo_json_response(self, 405, "HEAD not supported")
 
     def get(self) -> None:
         """This method handles the GET requests to retrieve status on agents from the Cloud Verifier.
 
@@ -308,41 +350,21 @@
         will return errors. Agents requests require a single agent_id parameter which identifies the
         agent to be returned. If the agent_id is not found, a 404 response is returned.  If the agent_id
         was not found, it either completed successfully, or failed.  If found, the agent_id is still polling
         to contact the Cloud Agent.
         """
         session = get_session()
 
-        if self.request.uri is None:
-            web_util.echo_json_response(self, 400, "URI not specified")
-            return
-
-        rest_params = web_util.get_restful_params(self.request.uri)
-        if rest_params is None:
-            web_util.echo_json_response(self, 405, "Not Implemented: Use /agents/ interface")
+        rest_params, agent_id = self.__validate_input("GET")
+        if not rest_params:
             return
 
-        if not web_util.validate_api_version(self, cast(str, rest_params["api_version"]), logger):
-            return
-
-        if "agents" not in rest_params:
-            web_util.echo_json_response(self, 400, "uri not supported")
-            logger.warning("GET returning 400 response. uri not supported: %s", self.request.path)
-            return
-
-        agent_id = rest_params["agents"]
-
         if (agent_id is not None) and (agent_id != ""):
             # If the agent ID is not valid (wrong set of characters),
             # just do nothing.
-            if not validators.valid_agent_id(agent_id):
-                web_util.echo_json_response(self, 400, "agent_id not not valid")
-                logger.error("GET received an invalid agent ID: %s", agent_id)
-                return
-
             agent = None
             try:
                 agent = (
                     session.query(VerfierMain)
                     .options(  # type: ignore
                         joinedload(VerfierMain.ima_policy).load_only(
                             VerifierAllowlist.checksum, VerifierAllowlist.generator  # pyright: ignore
@@ -409,42 +431,16 @@
         """This method handles the DELETE requests to remove agents from the Cloud Verifier.
 
         Currently, only agents resources are available for DELETEing, i.e. /agents. All other DELETE uri's will return errors.
         agents requests require a single agent_id parameter which identifies the agent to be deleted.
         """
         session = get_session()
 
-        if self.request.uri is None:
-            web_util.echo_json_response(self, 400, "URI not specified")
-            return
-
-        rest_params = web_util.get_restful_params(self.request.uri)
-        if rest_params is None:
-            web_util.echo_json_response(self, 405, "Not Implemented: Use /agents/ interface")
-            return
-
-        if not web_util.validate_api_version(self, cast(str, rest_params["api_version"]), logger):
-            return
-
-        if "agents" not in rest_params:
-            web_util.echo_json_response(self, 400, "uri not supported")
-            return
-
-        agent_id = rest_params["agents"]
-
-        if agent_id is None:
-            web_util.echo_json_response(self, 400, "uri not supported")
-            logger.warning("DELETE returning 400 response. uri not supported: %s", self.request.path)
-            return
-
-        # If the agent ID is not valid (wrong set of characters), just
-        # do nothing.
-        if not validators.valid_agent_id(agent_id):
-            web_util.echo_json_response(self, 400, "agent_id not not valid")
-            logger.error("DELETE received an invalid agent ID: %s", agent_id)
+        rest_params, agent_id = self.__validate_input("DELETE")
+        if not rest_params or not agent_id:
             return
 
         agent = None
         try:
             agent = session.query(VerfierMain).filter_by(agent_id=agent_id).first()
         except SQLAlchemyError as e:
             logger.error("SQLAlchemy Error for agent ID %s: %s", agent_id, e)
@@ -497,79 +493,58 @@
         Currently, only agents resources are available for POSTing, i.e. /agents. All other POST uri's will return errors.
         agents requests require a json block sent in the body
         """
         session = get_session()
         # TODO: exception handling needs fixing
         # Maybe handle exceptions with if/else if/else blocks ... simple and avoids nesting
         try:  # pylint: disable=too-many-nested-blocks
-            if self.request.uri is None:
-                web_util.echo_json_response(self, 400, "URI not specified")
-                return
-
-            rest_params = web_util.get_restful_params(self.request.uri)
-            if rest_params is None:
-                web_util.echo_json_response(self, 405, "Not Implemented: Use /agents/ interface")
+            rest_params, agent_id = self.__validate_input("POST")
+            if not rest_params:
                 return
 
-            if not web_util.validate_api_version(self, cast(str, rest_params["api_version"]), logger):
-                return
-
-            if "agents" not in rest_params:
-                web_util.echo_json_response(self, 400, "uri not supported")
-                logger.warning("POST returning 400 response. uri not supported: %s", self.request.path)
-                return
-
-            agent_id = rest_params["agents"]
-
             if agent_id is not None:
-                # If the agent ID is not valid (wrong set of
-                # characters), just do nothing.
-                if not validators.valid_agent_id(agent_id):
-                    web_util.echo_json_response(self, 400, "agent_id not not valid")
-                    logger.error("POST received an invalid agent ID: %s", agent_id)
-                    return
-
                 content_length = len(self.request.body)
                 if content_length == 0:
                     web_util.echo_json_response(self, 400, "Expected non zero content length")
                     logger.warning("POST returning 400 response. Expected non zero content length.")
                 else:
                     json_body = json.loads(self.request.body)
-                    agent_data = {}
-                    agent_data["v"] = json_body["v"]
-                    agent_data["ip"] = json_body["cloudagent_ip"]
-                    agent_data["port"] = int(json_body["cloudagent_port"])
-                    agent_data["operational_state"] = states.START
-                    agent_data["public_key"] = ""
-                    agent_data["tpm_policy"] = json_body["tpm_policy"]
-                    agent_data["meta_data"] = json_body["metadata"]
-                    agent_data["mb_refstate"] = json_body["mb_refstate"]
-                    agent_data["ima_sign_verification_keys"] = json_body["ima_sign_verification_keys"]
-                    agent_data["revocation_key"] = json_body["revocation_key"]
-                    agent_data["accept_tpm_hash_algs"] = json_body["accept_tpm_hash_algs"]
-                    agent_data["accept_tpm_encryption_algs"] = json_body["accept_tpm_encryption_algs"]
-                    agent_data["accept_tpm_signing_algs"] = json_body["accept_tpm_signing_algs"]
-                    agent_data["supported_version"] = json_body["supported_version"]
-                    agent_data["ak_tpm"] = json_body["ak_tpm"]
-                    agent_data["mtls_cert"] = json_body.get("mtls_cert", None)
-                    agent_data["hash_alg"] = ""
-                    agent_data["enc_alg"] = ""
-                    agent_data["sign_alg"] = ""
-                    agent_data["agent_id"] = agent_id
-                    agent_data["boottime"] = 0
-                    agent_data["ima_pcrs"] = []
-                    agent_data["pcr10"] = None
-                    agent_data["next_ima_ml_entry"] = 0
-                    agent_data["learned_ima_keyrings"] = {}
-                    agent_data["verifier_id"] = config.get(
-                        "verifier", "uuid", fallback=cloud_verifier_common.DEFAULT_VERIFIER_ID
-                    )
-                    agent_data["attestation_count"] = 0
-                    agent_data["last_received_quote"] = 0
-                    agent_data["last_successful_attestation"] = 0
+                    agent_data = {
+                        "v": json_body["v"],
+                        "ip": json_body["cloudagent_ip"],
+                        "port": int(json_body["cloudagent_port"]),
+                        "operational_state": states.START,
+                        "public_key": "",
+                        "tpm_policy": json_body["tpm_policy"],
+                        "meta_data": json_body["metadata"],
+                        "mb_refstate": json_body["mb_refstate"],
+                        "ima_sign_verification_keys": json_body["ima_sign_verification_keys"],
+                        "revocation_key": json_body["revocation_key"],
+                        "accept_tpm_hash_algs": json_body["accept_tpm_hash_algs"],
+                        "accept_tpm_encryption_algs": json_body["accept_tpm_encryption_algs"],
+                        "accept_tpm_signing_algs": json_body["accept_tpm_signing_algs"],
+                        "supported_version": json_body["supported_version"],
+                        "ak_tpm": json_body["ak_tpm"],
+                        "mtls_cert": json_body.get("mtls_cert", None),
+                        "hash_alg": "",
+                        "enc_alg": "",
+                        "sign_alg": "",
+                        "agent_id": agent_id,
+                        "boottime": 0,
+                        "ima_pcrs": [],
+                        "pcr10": None,
+                        "next_ima_ml_entry": 0,
+                        "learned_ima_keyrings": {},
+                        "verifier_id": config.get(
+                            "verifier", "uuid", fallback=cloud_verifier_common.DEFAULT_VERIFIER_ID
+                        ),
+                        "attestation_count": 0,
+                        "last_received_quote": 0,
+                        "last_successful_attestation": 0,
+                    }
 
                     if "verifier_ip" in json_body:
                         agent_data["verifier_ip"] = json_body["verifier_ip"]
                     else:
                         agent_data["verifier_ip"] = config.get("verifier", "ip")
 
                     if "verifier_port" in json_body:
@@ -738,42 +713,16 @@
         """This method handles the PUT requests to add agents to the Cloud Verifier.
 
         Currently, only agents resources are available for PUTing, i.e. /agents. All other PUT uri's will return errors.
         agents requests require a json block sent in the body
         """
         session = get_session()
         try:
-            if self.request.uri is None:
-                web_util.echo_json_response(self, 400, "URI not specified")
-                return
-
-            rest_params = web_util.get_restful_params(self.request.uri)
-            if rest_params is None:
-                web_util.echo_json_response(self, 405, "Not Implemented: Use /agents/ interface")
-                return
-
-            if not web_util.validate_api_version(self, cast(str, rest_params["api_version"]), logger):
-                return
-
-            if "agents" not in rest_params:
-                web_util.echo_json_response(self, 400, "uri not supported")
-                logger.warning("PUT returning 400 response. uri not supported: %s", self.request.path)
-                return
-
-            agent_id = rest_params["agents"]
-
-            if agent_id is None:
-                web_util.echo_json_response(self, 400, "uri not supported")
-                logger.warning("PUT returning 400 response. uri not supported")
-
-            # If the agent ID is not valid (wrong set of characters),
-            # just do nothing.
-            if not validators.valid_agent_id(agent_id):
-                web_util.echo_json_response(self, 400, "agent_id not not valid")
-                logger.error("PUT received an invalid agent ID: %s", agent_id)
+            rest_params, agent_id = self.__validate_input("PUT")
+            if not rest_params:
                 return
 
             try:
                 verifier_id = config.get("verifier", "uuid", fallback=cloud_verifier_common.DEFAULT_VERIFIER_ID)
                 db_agent = session.query(VerfierMain).filter_by(agent_id=agent_id, verifier_id=verifier_id).one()
             except SQLAlchemyError as e:
                 logger.error("SQLAlchemy Error for agent ID %s: %s", agent_id, e)
@@ -922,23 +871,21 @@
         # NOTE(kaifeng) 204 Can not have response body, but current helper
         # doesn't support this case.
         self.set_status(204)
         self.set_header("Content-Type", "application/json")
         self.finish()
         logger.info("DELETE returning 204 response for allowlist: %s", allowlist_name)
 
-    def __get_runtime_policy_db_format(self, runtime_policy_name: str) -> Optional[Dict[str, Any]]:
+    def __get_runtime_policy_db_format(self, runtime_policy_name: str) -> Dict[str, Any]:
         """Get the IMA policy from the request and return it in Db format"""
         content_length = len(self.request.body)
         if content_length == 0:
             web_util.echo_json_response(self, 400, "Expected non zero content length")
             logger.warning("POST returning 400 response. Expected non zero content length.")
-            return None
-
-        runtime_policy = "{}"
+            return {}
 
         json_body = json.loads(self.request.body)
 
         runtime_policy = base64.b64decode(json_body.get("runtime_policy")).decode()
         runtime_policy_key_bytes = signing.get_runtime_policy_keys(
             runtime_policy.encode(),
             json_body.get("runtime_policy_key"),
@@ -949,25 +896,25 @@
                 runtime_policy.encode(),
                 runtime_policy_key_bytes,
                 verify_sig=config.getboolean("verifier", "require_allow_list_signatures", fallback=False),
             )
         except ima.ImaValidationError as e:
             web_util.echo_json_response(self, e.code, e.message)
             logger.warning(e.message)
-            return None
+            return {}
 
         tpm_policy = json_body.get("tpm_policy")
 
         try:
             runtime_policy_db_format = ima.runtime_policy_db_contents(runtime_policy_name, runtime_policy, tpm_policy)
         except ima.ImaValidationError as e:
             message = f"Runtime policy is malformatted: {e.message}"
             web_util.echo_json_response(self, e.code, message)
             logger.warning(message)
-            return None
+            return {}
 
         return runtime_policy_db_format
 
     def post(self) -> None:
         """Create an allowlist
 
         POST /allowlists/{name}
@@ -1060,31 +1007,26 @@
     params = cloud_verifier_common.prepare_get_quote(agent)
 
     partial_req = "1"
     if need_pubkey:
         partial_req = "0"
 
     # TODO: remove special handling after initial upgrade
+    kwargs = {}
     if agent["ssl_context"]:
-        res = tornado_requests.request(
-            "GET",
-            f"https://{agent['ip']}:{agent['port']}/v{agent['supported_version']}/quotes/integrity"
-            f"?nonce={params['nonce']}&mask={params['mask']}"
-            f"&partial={partial_req}&ima_ml_entry={params['ima_ml_entry']}",
-            context=agent["ssl_context"],
-            timeout=timeout,
-        )
-    else:
-        res = tornado_requests.request(
-            "GET",
-            f"http://{agent['ip']}:{agent['port']}/v{agent['supported_version']}/quotes/integrity"
-            f"?nonce={params['nonce']}&mask={params['mask']}"
-            f"&partial={partial_req}&ima_ml_entry={params['ima_ml_entry']}",
-            timeout=timeout,
-        )
+        kwargs["context"] = agent["ssl_context"]
+
+    res = tornado_requests.request(
+        "GET",
+        f"http://{agent['ip']}:{agent['port']}/v{agent['supported_version']}/quotes/integrity"
+        f"?nonce={params['nonce']}&mask={params['mask']}"
+        f"&partial={partial_req}&ima_ml_entry={params['ima_ml_entry']}",
+        **kwargs,
+        timeout=timeout,
+    )
     response = await res
 
     if response.status_code != 200:
         # this is a connection error, retry get quote
         if response.status_code in [408, 500, 599]:
             asyncio.ensure_future(process_agent(agent, states.GET_QUOTE_RETRY))
         else:
@@ -1133,37 +1075,31 @@
             asyncio.ensure_future(process_agent(agent, states.FAILED, failure))
 
 
 async def invoke_provide_v(agent: Optional[Dict[str, Any]], timeout: float = 60.0) -> None:
     failure = Failure(Component.INTERNAL, ["verifier"])
     if agent is None:
         raise Exception("Agent deleted while being processed")
-    try:
-        if agent["pending_event"] is not None:
-            agent["pending_event"] = None
-    except KeyError:
-        pass
+    if agent.get("pending_event") is not None:
+        agent["pending_event"] = None
+
     v_json_message = cloud_verifier_common.prepare_v(agent)
 
     # TODO: remove special handling after initial upgrade
+    kwargs = {}
     if agent["ssl_context"]:
-        res = tornado_requests.request(
-            "POST",
-            f"https://{agent['ip']}:{agent['port']}/v{agent['supported_version']}/keys/vkey",
-            data=v_json_message,
-            context=agent["ssl_context"],
-            timeout=timeout,
-        )
-    else:
-        res = tornado_requests.request(
-            "POST",
-            f"http://{agent['ip']}:{agent['port']}/v{agent['supported_version']}/keys/vkey",
-            data=v_json_message,
-            timeout=timeout,
-        )
+        kwargs["context"] = agent["ssl_context"]
+
+    res = tornado_requests.request(
+        "POST",
+        f"http://{agent['ip']}:{agent['port']}/v{agent['supported_version']}/keys/vkey",
+        data=v_json_message,
+        **kwargs,
+        timeout=timeout,
+    )
 
     response = await res
 
     if response.status_code != 200:
         if response.status_code in [408, 500, 599]:
             asyncio.ensure_future(process_agent(agent, states.PROVIDE_V_RETRY))
         else:
@@ -1274,23 +1210,23 @@
         if not stored_agent:
             logger.warning("Unable to retrieve agent %s from database. Stopping polling", agent["agent_id"])
             if agent["pending_event"] is not None:
                 tornado.ioloop.IOLoop.current().remove_timeout(agent["pending_event"])
             return
 
         # if the user did terminated this agent
-        if stored_agent.operational_state == states.TERMINATED:
+        if stored_agent.operational_state == states.TERMINATED:  # pyright: ignore
             logger.warning("Agent %s terminated by user.", agent["agent_id"])
             if agent["pending_event"] is not None:
                 tornado.ioloop.IOLoop.current().remove_timeout(agent["pending_event"])
             verifier_db_delete_agent(session, agent["agent_id"])
             return
 
         # if the user tells us to stop polling because the tenant quote check failed
-        if stored_agent.operational_state == states.TENANT_FAILED:
+        if stored_agent.operational_state == states.TENANT_FAILED:  # pyright: ignore
             logger.warning("Agent %s has failed tenant quote. Stopping polling", agent["agent_id"])
             if agent["pending_event"] is not None:
                 tornado.ioloop.IOLoop.current().remove_timeout(agent["pending_event"])
             return
 
         # Get request timeout from configuration file
         timeout = config.getfloat("verifier", "request_timeout", fallback=60.0)
@@ -1457,17 +1393,17 @@
         agent.verifier_port = verifier_port  # pyright: ignore
         agent_run = _from_db_obj(agent)
         if agent_run["mtls_cert"] and agent_run["mtls_cert"] != "disabled":
             agent_run["ssl_context"] = web_util.generate_agent_tls_context(
                 "verifier", agent_run["mtls_cert"], logger=logger
             )
 
-        if agent.operational_state == states.START:
+        if agent.operational_state == states.START:  # pyright: ignore
             asyncio.ensure_future(process_agent(agent_run, states.GET_QUOTE))
-        if agent.boottime:
+        if agent.boottime:  # pyright: ignore
             ima_pcrs_dict = {}
             assert isinstance(agent.ima_pcrs, list)
             for pcr_num in agent.ima_pcrs:
                 ima_pcrs_dict[pcr_num] = getattr(agent, f"pcr{pcr_num}")
             aas.add(
                 str(agent.agent_id),
                 int(agent.boottime),  # pyright: ignore
@@ -1492,20 +1428,14 @@
 
     config.check_version("verifier", logger=logger)
 
     verifier_port = config.get("verifier", "port")
     verifier_host = config.get("verifier", "ip")
     verifier_id = config.get("verifier", "uuid", fallback=cloud_verifier_common.DEFAULT_VERIFIER_ID)
 
-    # Check if measured boot was configured correctly
-    mb_policy_name = config.get("verifier", "measured_boot_policy_name", fallback="accept-all")
-    if mb_policy_name and policies.get_policy(mb_policy_name) is None:
-        logger.error('Measured boot policy "%s" could not be found!', mb_policy_name)
-        raise Exception(f'Measued boot policy "{mb_policy_name}" could not be found!')
-
     # allow tornado's max upload size to be configurable
     max_upload_size = None
     if config.has_option("verifier", "max_upload_size"):
         max_upload_size = int(config.get("verifier", "max_upload_size"))
 
     # set a conservative general umask
     os.umask(0o077)
```

### Comparing `keylime-7.0.0/keylime/cmd/convert_config.py` & `keylime-7.2.5/keylime/cmd/convert_config.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/cmd/convert_runtime_policy.py` & `keylime-7.2.5/keylime/cmd/convert_runtime_policy.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/cmd/create_policy.py` & `keylime-7.2.5/keylime/cmd/create_policy.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/cmd/registrar.py` & `keylime-7.2.5/keylime/cmd/registrar.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/cmd/sign_runtime_policy.py` & `keylime-7.2.5/keylime/cmd/sign_runtime_policy.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/cmd/user_data_encrypt.py` & `keylime-7.2.5/keylime/cmd/user_data_encrypt.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/cmd_exec.py` & `keylime-7.2.5/keylime/cmd_exec.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/common/algorithms.py` & `keylime-7.2.5/keylime/common/algorithms.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,20 @@
 
     def hash(self, data: bytes) -> bytes:
         return cast(bytes, self.__hashfn(data).digest())
 
     def get_size(self) -> int:
         return cast(int, self.__hashfn(b"").digest_size * 8)
 
+    def get_start_hash(self) -> bytes:
+        return b"\x00" * (self.get_size() // 8)
+
+    def get_ff_hash(self) -> bytes:
+        return b"\xff" * (self.get_size() // 8)
+
     def __str__(self) -> str:
         return self.value
 
 
 class Encrypt:
     RSA = "rsa"
     ECC = "ecc"
```

### Comparing `keylime-7.0.0/keylime/common/migrations.py` & `keylime-7.2.5/keylime/common/migrations.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/common/states.py` & `keylime-7.2.5/keylime/common/states.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/common/validators.py` & `keylime-7.2.5/keylime/common/validators.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/common/version.py` & `keylime-7.2.5/keylime/common/version.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/config.py` & `keylime-7.2.5/keylime/config.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/crypto.py` & `keylime-7.2.5/keylime/crypto.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/da/attest.py` & `keylime-7.2.5/keylime/da/attest.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import argparse
 import json
 import sys
 from datetime import datetime
 
 from keylime import cloud_verifier_common, config, keylime_logging
 from keylime.da import record
-from keylime.elchecking.policies import load_policies
+from keylime.mba import mba
 
 logger = keylime_logging.init_logging("durable_attestation_fetch_and_replay")
 
 
 def main() -> None:
     parser = argparse.ArgumentParser()
     parser.add_argument(
@@ -36,15 +36,15 @@
         dest="end_date",
         default="last",
         help='end date for attestation window in IS0 8601 format (e.g., "2008-09-03T21:56:35"), or keyworkd "last"',
     )
 
     args = parser.parse_args()
 
-    load_policies()
+    mba.load_policy_engine()
 
     rmcb = config.get("registrar", "durable_attestation_import", fallback="")
     rmc = record.get_record_mgt_class(rmcb)
     if not rmc:
         return
 
     rmc = rmc("registrar")
```

### Comparing `keylime-7.0.0/keylime/da/examples/file.py` & `keylime-7.2.5/keylime/da/examples/file.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/da/examples/redis.py` & `keylime-7.2.5/keylime/da/examples/redis.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/da/examples/rekor.py` & `keylime-7.2.5/keylime/da/examples/rekor.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/da/examples/sqldb.py` & `keylime-7.2.5/keylime/da/examples/sqldb.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/da/examples/tsa_rfc3161.py` & `keylime-7.2.5/keylime/da/examples/tsa_rfc3161.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/da/record.py` & `keylime-7.2.5/keylime/da/record.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/db/keylime_db.py` & `keylime-7.2.5/keylime/db/keylime_db.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/db/registrar_db.py` & `keylime-7.2.5/keylime/db/registrar_db.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/db/verifier_db.py` & `keylime-7.2.5/keylime/db/verifier_db.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/dsse/dsse.py` & `keylime-7.2.5/keylime/dsse/dsse.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/dsse/ecdsa.py` & `keylime-7.2.5/keylime/dsse/ecdsa.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/dsse/x509.py` & `keylime-7.2.5/keylime/dsse/x509.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/elchecking/__main__.py` & `keylime-7.2.5/keylime/mba/elchecking/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import argparse
 import json
 import sys
 
-from ..tpm import tpm_main
+from keylime.tpm import tpm_main
+
 from . import policies
 
 policies.load_policies()
 # This main module is just for command-line based testing.
 # It implements a command to do one test.
 # Invoke it with `python3 -m $packagename`, for some value of
 # `$packagename` that works with your `$PYTHONPATH`.
@@ -23,16 +24,16 @@
         f"Specified policy '{args.policy_name}' does not exist. Options are: {policies.get_policy_names()}.",
         file=sys.stderr,
     )
     sys.exit(1)
 refstate_str = args.refstate_file.read()
 refstate = json.loads(refstate_str)
 log_bin = args.eventlog_file.read()
-tpm = tpm_main.tpm()
-_, log_data = tpm.parse_binary_bootlog(log_bin)
+Tpm = tpm_main.Tpm()
+_, log_data = Tpm.parse_binary_bootlog(log_bin)
 with open("/tmp/parsed.json", "wt", encoding="utf-8") as log_data_file:
     log_data_file.write(json.dumps(log_data, indent=True))
 why_not = policy.evaluate(refstate, log_data)
 if why_not:
     print(why_not, file=sys.stderr)
     sys.exit(1)
 print("AOK")
```

### Comparing `keylime-7.0.0/keylime/elchecking/example.py` & `keylime-7.2.5/keylime/mba/elchecking/example.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/elchecking/policies.py` & `keylime-7.2.5/keylime/mba/elchecking/policies.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/elchecking/tests.py` & `keylime-7.2.5/keylime/mba/elchecking/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import abc
-import codecs
 import re
 import typing
 
 from keylime.common.algorithms import Hash
 
 # This module defines the abstraction of a Test (of JSON data)
 # and several specific test classes.
@@ -638,19 +637,19 @@
     """Test for valid EV_SEPARATOR entry values"""
 
     def __init__(self) -> None:
         # See TCG PC Client Platform Firmware Profile (Table 9 Events)
         valid_hex_values = ["00000000", "FFFFFFFF"]
         tests = []
         for value in valid_hex_values:
-            val_bytes = codecs.decode(value.encode(), "hex")
+            val_bytes = bytes.fromhex(value)
             event_test = FieldTest("Event", StringEqual(value))
             digests = {}
             for hash_alg in Hash:
-                digests[str(hash_alg)] = codecs.encode(hash_alg.hash(val_bytes), "hex").decode("utf-8")
+                digests[str(hash_alg)] = hash_alg.hash(val_bytes).hex()
             tests.append(And(event_test, DigestTest(digests)))
         super().__init__(*tests)
 
 
 class EvEfiActionTest(Test):
     """Test for valid EV_EFI_ACTION entry values"""
 
@@ -671,15 +670,15 @@
             return
 
         tests = []
         for value in self._expected_strings[pcr]:
             event_test = FieldTest("Event", StringEqual(value))
             digests = {}
             for hash_alg in Hash:
-                digests[str(hash_alg)] = codecs.encode(hash_alg.hash(value.encode()), "hex").decode("utf-8")
+                digests[str(hash_alg)] = hash_alg.hash(value.encode()).hex()
             tests.append(And(event_test, DigestTest(digests)))
         self.test = Or(*tests)
 
     def why_not(self, globs: Globals, subject: Data) -> str:
         if self.test is None:
             return f"No EV_EFI_ACTION event for {self.pcr} is expected in the spec"
```

### Comparing `keylime-7.0.0/keylime/failure.py` & `keylime-7.2.5/keylime/failure.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/ima/ast.py` & `keylime-7.2.5/keylime/ima/ast.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,872 +12,850 @@
 000000b0: 696e 7465 6772 6974 792f 696d 612f 696d  integrity/ima/im
 000000c0: 615f 7465 6d70 6c61 7465 2e63 0a20 202d  a_template.c.  -
 000000d0: 2068 7474 7073 3a2f 2f77 7777 2e6b 6572   https://www.ker
 000000e0: 6e65 6c2e 6f72 672f 646f 632f 6874 6d6c  nel.org/doc/html
 000000f0: 2f76 352e 3132 2f73 6563 7572 6974 792f  /v5.12/security/
 00000100: 494d 412d 7465 6d70 6c61 7465 732e 6874  IMA-templates.ht
 00000110: 6d6c 0a0a 2222 220a 0a69 6d70 6f72 7420  ml.."""..import 
-00000120: 6162 630a 696d 706f 7274 2062 696e 6173  abc.import binas
-00000130: 6369 690a 696d 706f 7274 2063 6f64 6563  cii.import codec
-00000140: 730a 696d 706f 7274 2073 7472 7563 740a  s.import struct.
-00000150: 696d 706f 7274 2074 7970 696e 670a 6672  import typing.fr
-00000160: 6f6d 2074 7970 696e 6720 696d 706f 7274  om typing import
-00000170: 2041 6e79 2c20 4361 6c6c 6162 6c65 2c20   Any, Callable, 
-00000180: 4469 6374 2c20 4f70 7469 6f6e 616c 2c20  Dict, Optional, 
-00000190: 556e 696f 6e0a 0a66 726f 6d20 6b65 796c  Union..from keyl
-000001a0: 696d 6520 696d 706f 7274 2063 6f6e 6669  ime import confi
-000001b0: 672c 206b 6579 6c69 6d65 5f6c 6f67 6769  g, keylime_loggi
-000001c0: 6e67 0a66 726f 6d20 6b65 796c 696d 652e  ng.from keylime.
-000001d0: 636f 6d6d 6f6e 2e61 6c67 6f72 6974 686d  common.algorithm
-000001e0: 7320 696d 706f 7274 2048 6173 680a 6672  s import Hash.fr
-000001f0: 6f6d 206b 6579 6c69 6d65 2e66 6169 6c75  om keylime.failu
-00000200: 7265 2069 6d70 6f72 7420 436f 6d70 6f6e  re import Compon
-00000210: 656e 742c 2046 6169 6c75 7265 0a0a 6c6f  ent, Failure..lo
-00000220: 6767 6572 203d 206b 6579 6c69 6d65 5f6c  gger = keylime_l
-00000230: 6f67 6769 6e67 2e69 6e69 745f 6c6f 6767  ogging.init_logg
-00000240: 696e 6728 2269 6d61 2229 0a0a 5443 475f  ing("ima")..TCG_
-00000250: 4556 454e 545f 4e41 4d45 5f4c 454e 5f4d  EVENT_NAME_LEN_M
-00000260: 4158 203d 2032 3535 0a53 4841 5f44 4947  AX = 255.SHA_DIG
-00000270: 4553 545f 4c45 4e20 3d20 3230 0a4d 4435  EST_LEN = 20.MD5
-00000280: 5f44 4947 4553 545f 4c45 4e20 3d20 3136  _DIGEST_LEN = 16
-00000290: 0a0a 4e55 4c4c 5f42 5954 4520 3d20 6f72  ..NULL_BYTE = or
-000002a0: 6428 225c 3022 290a 434f 4c4f 4e5f 4259  d("\0").COLON_BY
-000002b0: 5445 203d 206f 7264 2822 3a22 290a 0a0a  TE = ord(":")...
-000002c0: 6465 6620 6765 745f 5354 4152 545f 4841  def get_START_HA
-000002d0: 5348 2868 6173 685f 616c 673a 2048 6173  SH(hash_alg: Has
-000002e0: 6829 202d 3e20 6279 7465 733a 0a20 2020  h) -> bytes:.   
-000002f0: 2072 6574 7572 6e20 636f 6465 6373 2e64   return codecs.d
-00000300: 6563 6f64 6528 6222 3022 202a 2028 6861  ecode(b"0" * (ha
-00000310: 7368 5f61 6c67 2e67 6574 5f73 697a 6528  sh_alg.get_size(
-00000320: 2920 2f2f 2034 292c 2022 6865 7822 290a  ) // 4), "hex").
-00000330: 0a0a 6465 6620 6765 745f 4646 5f48 4153  ..def get_FF_HAS
-00000340: 4828 6861 7368 5f61 6c67 3a20 4861 7368  H(hash_alg: Hash
-00000350: 2920 2d3e 2062 7974 6573 3a0a 2020 2020  ) -> bytes:.    
-00000360: 7265 7475 726e 2063 6f64 6563 732e 6465  return codecs.de
-00000370: 636f 6465 2862 2266 2220 2a20 2868 6173  code(b"f" * (has
-00000380: 685f 616c 672e 6765 745f 7369 7a65 2829  h_alg.get_size()
-00000390: 202f 2f20 3429 2c20 2268 6578 2229 0a0a   // 4), "hex")..
-000003a0: 0a63 6c61 7373 2056 616c 6964 6174 6f72  .class Validator
-000003b0: 3a0a 2020 2020 6675 6e63 7469 6f6e 733a  :.    functions:
-000003c0: 2044 6963 745b 7479 7069 6e67 2e54 7970   Dict[typing.Typ
-000003d0: 655b 224d 6f64 6522 5d2c 2043 616c 6c61  e["Mode"], Calla
-000003e0: 626c 655b 2e2e 2e2c 2046 6169 6c75 7265  ble[..., Failure
-000003f0: 5d5d 0a0a 2020 2020 6465 6620 5f5f 696e  ]]..    def __in
-00000400: 6974 5f5f 2873 656c 662c 2066 756e 6374  it__(self, funct
-00000410: 696f 6e73 3a20 4469 6374 5b74 7970 696e  ions: Dict[typin
-00000420: 672e 5479 7065 5b22 4d6f 6465 225d 2c20  g.Type["Mode"], 
-00000430: 4361 6c6c 6162 6c65 5b2e 2e2e 2c20 4661  Callable[..., Fa
-00000440: 696c 7572 655d 5d29 3a0a 2020 2020 2020  ilure]]):.      
-00000450: 2020 7365 6c66 2e66 756e 6374 696f 6e73    self.functions
-00000460: 203d 2066 756e 6374 696f 6e73 0a0a 2020   = functions..  
-00000470: 2020 6465 6620 6765 745f 7661 6c69 6461    def get_valida
-00000480: 746f 7228 7365 6c66 2c20 636c 6173 735f  tor(self, class_
-00000490: 7479 7065 3a20 7479 7069 6e67 2e54 7970  type: typing.Typ
-000004a0: 655b 224d 6f64 6522 5d29 202d 3e20 4361  e["Mode"]) -> Ca
-000004b0: 6c6c 6162 6c65 5b2e 2e2e 2c20 4661 696c  llable[..., Fail
-000004c0: 7572 655d 3a0a 2020 2020 2020 2020 7661  ure]:.        va
-000004d0: 6c69 6461 746f 7220 3d20 7365 6c66 2e66  lidator = self.f
-000004e0: 756e 6374 696f 6e73 2e67 6574 2863 6c61  unctions.get(cla
-000004f0: 7373 5f74 7970 652c 204e 6f6e 6529 0a20  ss_type, None). 
-00000500: 2020 2020 2020 2069 6620 7661 6c69 6461         if valida
-00000510: 746f 7220 6973 204e 6f6e 653a 0a20 2020  tor is None:.   
-00000520: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-00000530: 7761 726e 696e 6728 224e 6f20 7661 6c69  warning("No vali
-00000540: 6461 746f 7220 7761 7320 696d 706c 656d  dator was implem
-00000550: 656e 7465 6420 666f 723a 2025 732e 2055  ented for: %s. U
-00000560: 7369 6e67 2061 6c77 6179 7320 6661 6c73  sing always fals
-00000570: 6520 7661 6c69 6461 746f 7221 222c 2063  e validator!", c
-00000580: 6c61 7373 5f74 7970 6529 0a20 2020 2020  lass_type).     
-00000590: 2020 2020 2020 2066 6169 6c75 7265 203d         failure =
-000005a0: 2046 6169 6c75 7265 2843 6f6d 706f 6e65   Failure(Compone
-000005b0: 6e74 2e49 4d41 2c20 5b22 7661 6c69 6461  nt.IMA, ["valida
-000005c0: 7469 6f6e 225d 290a 2020 2020 2020 2020  tion"]).        
-000005d0: 2020 2020 6661 696c 7572 652e 6164 645f      failure.add_
-000005e0: 6576 656e 7428 0a20 2020 2020 2020 2020  event(.         
-000005f0: 2020 2020 2020 2022 6e6f 5f76 616c 6964         "no_valid
-00000600: 6174 6f72 222c 2066 224e 6f20 7661 6c69  ator", f"No vali
-00000610: 6461 746f 7220 7761 7320 696d 706c 656d  dator was implem
-00000620: 656e 7465 6420 666f 723a 207b 636c 6173  ented for: {clas
-00000630: 735f 7479 7065 7d20 2e20 5573 696e 6720  s_type} . Using 
-00000640: 616c 7761 7973 2066 616c 7365 2076 616c  always false val
-00000650: 6964 6174 6f72 2122 2c20 5472 7565 0a20  idator!", True. 
-00000660: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00000670: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00000680: 6c61 6d62 6461 202a 5f3a 2066 6169 6c75  lambda *_: failu
-00000690: 7265 0a20 2020 2020 2020 2072 6574 7572  re.        retur
-000006a0: 6e20 7661 6c69 6461 746f 720a 0a0a 636c  n validator...cl
-000006b0: 6173 7320 5061 7273 6572 4572 726f 7228  ass ParserError(
-000006c0: 5479 7065 4572 726f 7229 3a0a 2020 2020  TypeError):.    
-000006d0: 2222 2249 7320 7468 726f 776e 2077 6865  """Is thrown whe
-000006e0: 6e20 6120 7479 7065 2063 6f75 6c64 206e  n a type could n
-000006f0: 6f74 2062 6520 636f 6e73 7472 7563 7465  ot be constructe
-00000700: 6420 7375 6363 6573 7366 756c 6c79 2e22  d successfully."
-00000710: 2222 0a0a 0a63 6c61 7373 204d 6f64 6528  ""...class Mode(
-00000720: 6162 632e 4142 4329 3a0a 2020 2020 4061  abc.ABC):.    @a
-00000730: 6263 2e61 6273 7472 6163 746d 6574 686f  bc.abstractmetho
-00000740: 640a 2020 2020 6465 6620 6973 5f64 6174  d.    def is_dat
-00000750: 615f 7661 6c69 6428 7365 6c66 2c20 7661  a_valid(self, va
-00000760: 6c69 6461 746f 723a 2056 616c 6964 6174  lidator: Validat
-00000770: 6f72 2920 2d3e 2046 6169 6c75 7265 3a0a  or) -> Failure:.
-00000780: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-00000790: 2020 4061 6263 2e61 6273 7472 6163 746d    @abc.abstractm
-000007a0: 6574 686f 640a 2020 2020 6465 6620 6279  ethod.    def by
-000007b0: 7465 7328 7365 6c66 2920 2d3e 2062 7974  tes(self) -> byt
-000007c0: 6573 3a0a 2020 2020 2020 2020 7061 7373  es:.        pass
-000007d0: 0a0a 0a63 6c61 7373 2054 7970 6528 6162  ...class Type(ab
-000007e0: 632e 4142 4329 3a0a 2020 2020 4061 6263  c.ABC):.    @abc
-000007f0: 2e61 6273 7472 6163 746d 6574 686f 640a  .abstractmethod.
-00000800: 2020 2020 6465 6620 7374 7275 6374 2873      def struct(s
-00000810: 656c 6629 202d 3e20 6279 7465 733a 0a20  elf) -> bytes:. 
-00000820: 2020 2020 2020 2070 6173 730a 0a0a 636c         pass...cl
-00000830: 6173 7320 4865 7844 6174 6128 5479 7065  ass HexData(Type
-00000840: 293a 0a20 2020 2064 6174 613a 2062 7974  ):.    data: byt
-00000850: 6573 0a0a 2020 2020 6465 6620 5f5f 696e  es..    def __in
-00000860: 6974 5f5f 2873 656c 662c 2064 6174 613a  it__(self, data:
-00000870: 2073 7472 293a 0a20 2020 2020 2020 2074   str):.        t
-00000880: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-00000890: 7365 6c66 2e64 6174 6120 3d20 636f 6465  self.data = code
-000008a0: 6373 2e64 6563 6f64 6528 6461 7461 2e65  cs.decode(data.e
-000008b0: 6e63 6f64 6528 2275 7466 2d38 2229 2c20  ncode("utf-8"), 
-000008c0: 2268 6578 2229 0a20 2020 2020 2020 2065  "hex").        e
-000008d0: 7863 6570 7420 6269 6e61 7363 6969 2e45  xcept binascii.E
-000008e0: 7272 6f72 2061 7320 653a 0a20 2020 2020  rror as e:.     
-000008f0: 2020 2020 2020 2072 6169 7365 2050 6172         raise Par
-00000900: 7365 7245 7272 6f72 2866 2250 726f 7669  serError(f"Provi
-00000910: 6465 6420 6461 7461 2077 6173 206e 6f74  ded data was not
-00000920: 2076 616c 6964 2068 6578 3a20 7b64 6174   valid hex: {dat
-00000930: 617d 2229 2066 726f 6d20 650a 0a20 2020  a}") from e..   
-00000940: 2064 6566 205f 5f73 7472 5f5f 2873 656c   def __str__(sel
-00000950: 6629 202d 3e20 7374 723a 0a20 2020 2020  f) -> str:.     
-00000960: 2020 2072 6574 7572 6e20 7365 6c66 2e64     return self.d
-00000970: 6174 612e 6465 636f 6465 2822 7574 662d  ata.decode("utf-
-00000980: 3822 290a 0a20 2020 2064 6566 2073 7472  8")..    def str
-00000990: 7563 7428 7365 6c66 2920 2d3e 2062 7974  uct(self) -> byt
-000009a0: 6573 3a0a 2020 2020 2020 2020 7265 7475  es:.        retu
-000009b0: 726e 2073 7472 7563 742e 7061 636b 2866  rn struct.pack(f
-000009c0: 223c 497b 6c65 6e28 7365 6c66 2e64 6174  "<I{len(self.dat
-000009d0: 6129 7d73 222c 206c 656e 2873 656c 662e  a)}s", len(self.
-000009e0: 6461 7461 292c 2073 656c 662e 6461 7461  data), self.data
-000009f0: 290a 0a0a 636c 6173 7320 5369 676e 6174  )...class Signat
-00000a00: 7572 6528 4865 7844 6174 6129 3a0a 2020  ure(HexData):.  
-00000a10: 2020 2222 220a 2020 2020 436c 6173 7320    """.    Class 
-00000a20: 666f 7220 7479 7065 2022 7369 6722 2e0a  for type "sig"..
-00000a30: 2020 2020 2222 220a 0a20 2020 2064 6566      """..    def
-00000a40: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-00000a50: 6461 7461 3a20 7374 7229 3a0a 2020 2020  data: str):.    
-00000a60: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
-00000a70: 6974 5f5f 2864 6174 6129 0a20 2020 2020  it__(data).     
-00000a80: 2020 2023 2062 6173 6963 2063 6865 636b     # basic check
-00000a90: 7320 6f6e 2073 6967 6e61 7475 7265 0a20  s on signature. 
-00000aa0: 2020 2020 2020 2066 6d74 203d 2022 3e42         fmt = ">B
-00000ab0: 4242 4948 220a 2020 2020 2020 2020 6864  BBIH".        hd
-00000ac0: 726c 656e 203d 2073 7472 7563 742e 6361  rlen = struct.ca
-00000ad0: 6c63 7369 7a65 2866 6d74 290a 2020 2020  lcsize(fmt).    
-00000ae0: 2020 2020 6966 206c 656e 2873 656c 662e      if len(self.
-00000af0: 6461 7461 2920 3c20 6864 726c 656e 3a0a  data) < hdrlen:.
-00000b00: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00000b10: 6520 5061 7273 6572 4572 726f 7228 2249  e ParserError("I
-00000b20: 6e76 616c 6964 2073 6967 6e61 7475 7265  nvalid signature
-00000b30: 3a20 6865 6164 6572 2074 6f6f 2073 686f  : header too sho
-00000b40: 7274 2229 0a20 2020 2020 2020 205f 2c20  rt").        _, 
-00000b50: 5f2c 205f 2c20 5f2c 2073 6967 5f73 697a  _, _, _, sig_siz
-00000b60: 6520 3d20 7374 7275 6374 2e75 6e70 6163  e = struct.unpac
-00000b70: 6b28 666d 742c 2073 656c 662e 6461 7461  k(fmt, self.data
-00000b80: 5b3a 6864 726c 656e 5d29 0a0a 2020 2020  [:hdrlen])..    
-00000b90: 2020 2020 6966 2068 6472 6c65 6e20 2b20      if hdrlen + 
-00000ba0: 7369 675f 7369 7a65 2021 3d20 6c65 6e28  sig_size != len(
-00000bb0: 7365 6c66 2e64 6174 6129 3a0a 2020 2020  self.data):.    
-00000bc0: 2020 2020 2020 2020 7261 6973 6520 5061          raise Pa
-00000bd0: 7273 6572 4572 726f 7228 2249 6e76 616c  rserError("Inval
-00000be0: 6964 2073 6967 6e61 7475 7265 3a20 6d61  id signature: ma
-00000bf0: 6c66 6f72 6d65 6420 6865 6164 6572 2229  lformed header")
-00000c00: 0a0a 0a63 6c61 7373 2042 7566 6665 7228  ...class Buffer(
-00000c10: 4865 7844 6174 6129 3a0a 2020 2020 2222  HexData):.    ""
-00000c20: 220a 2020 2020 436c 6173 7320 666f 7220  ".    Class for 
-00000c30: 7479 7065 2022 6275 6622 2e0a 2020 2020  type "buf"..    
-00000c40: 2222 220a 0a0a 636c 6173 7320 4e61 6d65  """...class Name
-00000c50: 2854 7970 6529 3a0a 2020 2020 2222 220a  (Type):.    """.
-00000c60: 2020 2020 436c 6173 7320 666f 7220 7479      Class for ty
-00000c70: 7065 2022 6e22 2061 6e64 2022 6e2d 6e67  pe "n" and "n-ng
-00000c80: 222e 0a20 2020 2022 2222 0a0a 2020 2020  "..    """..    
-00000c90: 6e61 6d65 3a20 7374 720a 2020 2020 6c65  name: str.    le
-00000ca0: 6761 6379 3a20 626f 6f6c 203d 2046 616c  gacy: bool = Fal
-00000cb0: 7365 0a0a 2020 2020 6465 6620 5f5f 696e  se..    def __in
-00000cc0: 6974 5f5f 2873 656c 662c 206e 616d 653a  it__(self, name:
-00000cd0: 2073 7472 2c20 6c65 6761 6379 3a20 626f   str, legacy: bo
-00000ce0: 6f6c 203d 2046 616c 7365 293a 0a20 2020  ol = False):.   
-00000cf0: 2020 2020 2073 656c 662e 6e61 6d65 203d       self.name =
-00000d00: 206e 616d 650a 2020 2020 2020 2020 7365   name.        se
-00000d10: 6c66 2e6c 6567 6163 7920 3d20 6c65 6761  lf.legacy = lega
-00000d20: 6379 0a0a 2020 2020 6465 6620 5f5f 7374  cy..    def __st
-00000d30: 725f 5f28 7365 6c66 2920 2d3e 2073 7472  r__(self) -> str
-00000d40: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00000d50: 2073 656c 662e 6e61 6d65 0a0a 2020 2020   self.name..    
-00000d60: 6465 6620 7374 7275 6374 2873 656c 6629  def struct(self)
-00000d70: 202d 3e20 6279 7465 733a 0a20 2020 2020   -> bytes:.     
-00000d80: 2020 206e 616d 655f 6279 7465 7320 3d20     name_bytes = 
-00000d90: 7365 6c66 2e6e 616d 652e 656e 636f 6465  self.name.encode
-00000da0: 2822 7574 662d 3822 290a 0a20 2020 2020  ("utf-8")..     
-00000db0: 2020 2023 2054 6865 206f 6c64 2022 6e22     # The old "n"
-00000dc0: 206f 7074 696f 6e20 6973 2066 6978 6564   option is fixed
-00000dd0: 206c 656e 6774 682e 0a20 2020 2020 2020   length..       
-00000de0: 2069 6620 7365 6c66 2e6c 6567 6163 793a   if self.legacy:
-00000df0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00000e00: 7572 6e20 7374 7275 6374 2e70 6163 6b28  urn struct.pack(
-00000e10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000e20: 2066 227b 6c65 6e28 6e61 6d65 5f62 7974   f"{len(name_byt
-00000e30: 6573 297d 7342 7b54 4347 5f45 5645 4e54  es)}sB{TCG_EVENT
-00000e40: 5f4e 414d 455f 4c45 4e5f 4d41 5820 2d20  _NAME_LEN_MAX - 
-00000e50: 6c65 6e28 6e61 6d65 5f62 7974 6573 297d  len(name_bytes)}
-00000e60: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
-00000e70: 2020 2020 6e61 6d65 5f62 7974 6573 2c0a      name_bytes,.
-00000e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e90: 4e55 4c4c 5f42 5954 452c 0a20 2020 2020  NULL_BYTE,.     
-00000ea0: 2020 2020 2020 2020 2020 2062 7974 6561             bytea
-00000eb0: 7272 6179 2854 4347 5f45 5645 4e54 5f4e  rray(TCG_EVENT_N
-00000ec0: 414d 455f 4c45 4e5f 4d41 5820 2d20 6c65  AME_LEN_MAX - le
-00000ed0: 6e28 6e61 6d65 5f62 7974 6573 2929 2c0a  n(name_bytes)),.
-00000ee0: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-00000ef0: 2020 2020 2020 2072 6574 7572 6e20 7374         return st
-00000f00: 7275 6374 2e70 6163 6b28 6622 3c49 7b6c  ruct.pack(f"<I{l
-00000f10: 656e 286e 616d 655f 6279 7465 7329 7d73  en(name_bytes)}s
-00000f20: 4222 2c20 6c65 6e28 6e61 6d65 5f62 7974  B", len(name_byt
-00000f30: 6573 2920 2b20 312c 206e 616d 655f 6279  es) + 1, name_by
-00000f40: 7465 732c 204e 554c 4c5f 4259 5445 290a  tes, NULL_BYTE).
-00000f50: 0a0a 636c 6173 7320 4469 6765 7374 3a0a  ..class Digest:.
-00000f60: 2020 2020 2222 220a 2020 2020 436c 6173      """.    Clas
-00000f70: 7320 666f 7220 7479 7065 7320 2264 2220  s for types "d" 
-00000f80: 616e 6420 2264 2d6e 6722 2077 6974 6820  and "d-ng" with 
-00000f90: 616e 6420 7769 7468 6f75 7420 616c 676f  and without algo
-00000fa0: 7269 7468 6d0a 2020 2020 2222 220a 0a20  rithm.    """.. 
-00000fb0: 2020 2068 6173 683a 2062 7974 6573 0a20     hash: bytes. 
-00000fc0: 2020 2061 6c67 6f72 6974 686d 3a20 7374     algorithm: st
-00000fd0: 720a 2020 2020 6c65 6761 6379 3a20 626f  r.    legacy: bo
-00000fe0: 6f6c 203d 2046 616c 7365 0a0a 2020 2020  ol = False..    
-00000ff0: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-00001000: 662c 2064 6967 6573 743a 2073 7472 2c20  f, digest: str, 
-00001010: 6c65 6761 6379 3a20 626f 6f6c 203d 2046  legacy: bool = F
-00001020: 616c 7365 293a 0a20 2020 2020 2020 2073  alse):.        s
-00001030: 656c 662e 6c65 6761 6379 203d 206c 6567  elf.legacy = leg
-00001040: 6163 790a 2020 2020 2020 2020 746f 6b65  acy.        toke
-00001050: 6e73 203d 2064 6967 6573 742e 7370 6c69  ns = digest.spli
-00001060: 7428 223a 2229 0a20 2020 2020 2020 2069  t(":").        i
-00001070: 6620 6c65 6e28 746f 6b65 6e73 2920 3d3d  f len(tokens) ==
-00001080: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
-00001090: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-000010a0: 2020 2020 2073 656c 662e 6861 7368 203d       self.hash =
-000010b0: 2063 6f64 6563 732e 6465 636f 6465 2874   codecs.decode(t
-000010c0: 6f6b 656e 735b 305d 2e65 6e63 6f64 6528  okens[0].encode(
-000010d0: 2275 7466 2d38 2229 2c20 2268 6578 2229  "utf-8"), "hex")
-000010e0: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
-000010f0: 6570 7420 6269 6e61 7363 6969 2e45 7272  ept binascii.Err
-00001100: 6f72 2061 7320 653a 0a20 2020 2020 2020  or as e:.       
-00001110: 2020 2020 2020 2020 2072 6169 7365 2050           raise P
-00001120: 6172 7365 7245 7272 6f72 2866 2244 6967  arserError(f"Dig
-00001130: 6573 7420 6861 7368 2069 7320 6e6f 7420  est hash is not 
-00001140: 7661 6c69 6420 6865 782e 2047 6f74 3a20  valid hex. Got: 
-00001150: 7b74 6f6b 656e 735b 305d 7d22 2920 6672  {tokens[0]}") fr
-00001160: 6f6d 2065 0a20 2020 2020 2020 2020 2020  om e.           
-00001170: 2069 6620 6c65 6e28 7365 6c66 2e68 6173   if len(self.has
-00001180: 6829 203d 3d20 5348 415f 4449 4745 5354  h) == SHA_DIGEST
-00001190: 5f4c 454e 3a0a 2020 2020 2020 2020 2020  _LEN:.          
-000011a0: 2020 2020 2020 7365 6c66 2e61 6c67 6f72        self.algor
-000011b0: 6974 686d 203d 2022 7368 6131 220a 2020  ithm = "sha1".  
-000011c0: 2020 2020 2020 2020 2020 656c 6966 206c            elif l
-000011d0: 656e 2873 656c 662e 6861 7368 2920 3d3d  en(self.hash) ==
-000011e0: 204d 4435 5f44 4947 4553 545f 4c45 4e3a   MD5_DIGEST_LEN:
-000011f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001200: 2073 656c 662e 616c 676f 7269 7468 6d20   self.algorithm 
-00001210: 3d20 226d 6435 220a 2020 2020 2020 2020  = "md5".        
-00001220: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00001230: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00001240: 5061 7273 6572 4572 726f 7228 0a20 2020  ParserError(.   
-00001250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001260: 2022 4361 6e6e 6f74 2063 7265 6174 6520   "Cannot create 
-00001270: 4469 6765 7374 2e20 4e6f 2068 6173 6820  Digest. No hash 
-00001280: 616c 676f 7269 7468 6d20 6973 2070 726f  algorithm is pro
-00001290: 7669 6465 6420 616e 6420 6861 7368 2064  vided and hash d
-000012a0: 6f65 7320 6e6f 7420 6265 6c6f 6e67 2074  oes not belong t
-000012b0: 6f20 6120 6d64 3520 6f72 2073 6861 3120  o a md5 or sha1 
-000012c0: 6861 7368 2e22 0a20 2020 2020 2020 2020  hash.".         
-000012d0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-000012e0: 2065 6c69 6620 6c65 6e28 746f 6b65 6e73   elif len(tokens
-000012f0: 2920 3d3d 2032 3a0a 2020 2020 2020 2020  ) == 2:.        
-00001300: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00001310: 2020 2020 2020 2020 2073 656c 662e 6861           self.ha
-00001320: 7368 203d 2063 6f64 6563 732e 6465 636f  sh = codecs.deco
-00001330: 6465 2874 6f6b 656e 735b 315d 2e65 6e63  de(tokens[1].enc
-00001340: 6f64 6528 2275 7466 2d38 2229 2c20 2268  ode("utf-8"), "h
-00001350: 6578 2229 0a20 2020 2020 2020 2020 2020  ex").           
-00001360: 2065 7863 6570 7420 6269 6e61 7363 6969   except binascii
-00001370: 2e45 7272 6f72 2061 7320 653a 0a20 2020  .Error as e:.   
-00001380: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-00001390: 7365 2050 6172 7365 7245 7272 6f72 2866  se ParserError(f
-000013a0: 2244 6967 6573 7420 6861 7368 2069 7320  "Digest hash is 
-000013b0: 6e6f 7420 7661 6c69 6420 6865 782e 2047  not valid hex. G
-000013c0: 6f74 3a20 7b74 6f6b 656e 735b 315d 7d22  ot: {tokens[1]}"
-000013d0: 2920 6672 6f6d 2065 0a20 2020 2020 2020  ) from e.       
-000013e0: 2020 2020 2073 656c 662e 616c 676f 7269       self.algori
-000013f0: 7468 6d20 3d20 746f 6b65 6e73 5b30 5d0a  thm = tokens[0].
-00001400: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00001410: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00001420: 5061 7273 6572 4572 726f 7228 6622 4361  ParserError(f"Ca
-00001430: 6e6e 6f74 2063 7265 6174 6520 4469 6765  nnot create Dige
-00001440: 7374 2065 7870 6563 7465 6420 3120 6f72  st expected 1 or
-00001450: 2032 2074 6f6b 656e 7320 676f 743a 207b   2 tokens got: {
-00001460: 6c65 6e28 746f 6b65 6e73 297d 2066 6f72  len(tokens)} for
-00001470: 207b 6469 6765 7374 7d22 290a 0a20 2020   {digest}")..   
-00001480: 2064 6566 2073 7472 7563 7428 7365 6c66   def struct(self
-00001490: 2920 2d3e 2062 7974 6573 3a0a 2020 2020  ) -> bytes:.    
-000014a0: 2020 2020 2320 5468 6520 6c65 6761 6379      # The legacy
-000014b0: 2066 6f72 6d61 7420 2264 2220 6861 7320   format "d" has 
-000014c0: 6669 7865 6420 6c65 6e67 7468 2c20 736f  fixed length, so
-000014d0: 2069 7420 646f 6573 206e 6f74 2063 6f6e   it does not con
-000014e0: 7461 696e 2061 206c 656e 6774 6820 6174  tain a length at
-000014f0: 7472 6962 7574 650a 2020 2020 2020 2020  tribute.        
-00001500: 6966 2073 656c 662e 6c65 6761 6379 3a0a  if self.legacy:.
-00001510: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00001520: 726e 2073 7472 7563 742e 7061 636b 2866  rn struct.pack(f
-00001530: 223c 7b6c 656e 2873 656c 662e 6861 7368  "<{len(self.hash
-00001540: 297d 7322 2c20 7365 6c66 2e68 6173 6829  )}s", self.hash)
-00001550: 0a0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
-00001560: 662e 616c 676f 7269 7468 6d20 6973 204e  f.algorithm is N
-00001570: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00001580: 2072 6574 7572 6e20 7374 7275 6374 2e70   return struct.p
-00001590: 6163 6b28 6622 3c49 7b6c 656e 2873 656c  ack(f"<I{len(sel
-000015a0: 662e 6861 7368 297d 7322 2c20 6c65 6e28  f.hash)}s", len(
-000015b0: 7365 6c66 2e68 6173 6829 2c20 7365 6c66  self.hash), self
-000015c0: 2e68 6173 6829 0a20 2020 2020 2020 2023  .hash).        #
-000015d0: 2041 6674 6572 2074 6865 2027 3a27 206d   After the ':' m
-000015e0: 7573 7420 6265 2061 2027 5c4f 273a 0a20  ust be a '\O':. 
-000015f0: 2020 2020 2020 2023 2068 7474 7073 3a2f         # https:/
-00001600: 2f65 6c69 7869 722e 626f 6f74 6c69 6e2e  /elixir.bootlin.
-00001610: 636f 6d2f 6c69 6e75 782f 7635 2e31 322e  com/linux/v5.12.
-00001620: 3130 2f73 6f75 7263 652f 7365 6375 7269  10/source/securi
-00001630: 7479 2f69 6e74 6567 7269 7479 2f69 6d61  ty/integrity/ima
-00001640: 2f69 6d61 5f74 656d 706c 6174 655f 6c69  /ima_template_li
-00001650: 622e 6323 4c32 3330 0a20 2020 2020 2020  b.c#L230.       
-00001660: 2072 6574 7572 6e20 7374 7275 6374 2e70   return struct.p
-00001670: 6163 6b28 0a20 2020 2020 2020 2020 2020  ack(.           
-00001680: 2066 223c 497b 6c65 6e28 7365 6c66 2e61   f"<I{len(self.a
-00001690: 6c67 6f72 6974 686d 297d 7342 427b 6c65  lgorithm)}sBB{le
-000016a0: 6e28 7365 6c66 2e68 6173 6829 7d73 222c  n(self.hash)}s",
-000016b0: 0a20 2020 2020 2020 2020 2020 206c 656e  .            len
-000016c0: 2873 656c 662e 616c 676f 7269 7468 6d29  (self.algorithm)
-000016d0: 202b 2032 202b 206c 656e 2873 656c 662e   + 2 + len(self.
-000016e0: 6861 7368 292c 0a20 2020 2020 2020 2020  hash),.         
-000016f0: 2020 2073 656c 662e 616c 676f 7269 7468     self.algorith
-00001700: 6d2e 656e 636f 6465 2822 7574 662d 3822  m.encode("utf-8"
-00001710: 292c 0a20 2020 2020 2020 2020 2020 2043  ),.            C
-00001720: 4f4c 4f4e 5f42 5954 452c 0a20 2020 2020  OLON_BYTE,.     
-00001730: 2020 2020 2020 204e 554c 4c5f 4259 5445         NULL_BYTE
-00001740: 2c0a 2020 2020 2020 2020 2020 2020 7365  ,.            se
-00001750: 6c66 2e68 6173 682c 0a20 2020 2020 2020  lf.hash,.       
-00001760: 2029 0a0a 2020 2020 6465 6620 5f5f 6571   )..    def __eq
-00001770: 5f5f 2873 656c 662c 206f 7468 6572 3a20  __(self, other: 
-00001780: 416e 7929 202d 3e20 626f 6f6c 3a0a 2020  Any) -> bool:.  
-00001790: 2020 2020 2020 7265 7475 726e 2028 0a20        return (. 
-000017a0: 2020 2020 2020 2020 2020 2069 7369 6e73             isins
-000017b0: 7461 6e63 6528 6f74 6865 722c 2044 6967  tance(other, Dig
-000017c0: 6573 7429 0a20 2020 2020 2020 2020 2020  est).           
-000017d0: 2061 6e64 2073 656c 662e 6c65 6761 6379   and self.legacy
-000017e0: 203d 3d20 6f74 6865 722e 6c65 6761 6379   == other.legacy
-000017f0: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
-00001800: 2073 656c 662e 6861 7368 203d 3d20 6f74   self.hash == ot
-00001810: 6865 722e 6861 7368 0a20 2020 2020 2020  her.hash.       
-00001820: 2020 2020 2061 6e64 2073 656c 662e 616c       and self.al
-00001830: 676f 7269 7468 6d20 3d3d 206f 7468 6572  gorithm == other
-00001840: 2e61 6c67 6f72 6974 686d 0a20 2020 2020  .algorithm.     
-00001850: 2020 2029 0a0a 0a63 6c61 7373 2049 6d61     )...class Ima
-00001860: 284d 6f64 6529 3a0a 2020 2020 2222 220a  (Mode):.    """.
-00001870: 2020 2020 436c 6173 7320 666f 7220 2269      Class for "i
-00001880: 6d61 222e 2043 6f6e 7461 696e 7320 7468  ma". Contains th
-00001890: 6520 6469 6765 7374 2061 6e64 2061 2070  e digest and a p
-000018a0: 6174 682e 0a20 2020 2022 2222 0a0a 2020  ath..    """..  
-000018b0: 2020 6469 6765 7374 3a20 4469 6765 7374    digest: Digest
-000018c0: 0a20 2020 2070 6174 683a 204e 616d 650a  .    path: Name.
-000018d0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-000018e0: 5f28 7365 6c66 2c20 6461 7461 3a20 7374  _(self, data: st
-000018f0: 7229 3a0a 2020 2020 2020 2020 746f 6b65  r):.        toke
-00001900: 6e73 203d 2064 6174 612e 7370 6c69 7428  ns = data.split(
-00001910: 2220 222c 206d 6178 7370 6c69 743d 3129  " ", maxsplit=1)
-00001920: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-00001930: 746f 6b65 6e73 2920 213d 2032 3a0a 2020  tokens) != 2:.  
-00001940: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00001950: 5061 7273 6572 4572 726f 7228 290a 2020  ParserError().  
-00001960: 2020 2020 2020 7365 6c66 2e64 6967 6573        self.diges
-00001970: 7420 3d20 4469 6765 7374 2874 6f6b 656e  t = Digest(token
-00001980: 735b 305d 2c20 6c65 6761 6379 3d54 7275  s[0], legacy=Tru
-00001990: 6529 0a20 2020 2020 2020 2073 656c 662e  e).        self.
-000019a0: 7061 7468 203d 204e 616d 6528 746f 6b65  path = Name(toke
-000019b0: 6e73 5b31 5d2c 206c 6567 6163 793d 5472  ns[1], legacy=Tr
-000019c0: 7565 290a 0a20 2020 2064 6566 2062 7974  ue)..    def byt
-000019d0: 6573 2873 656c 6629 202d 3e20 6279 7465  es(self) -> byte
-000019e0: 733a 0a20 2020 2020 2020 2072 6574 7572  s:.        retur
-000019f0: 6e20 7365 6c66 2e64 6967 6573 742e 7374  n self.digest.st
-00001a00: 7275 6374 2829 202b 2073 656c 662e 7061  ruct() + self.pa
-00001a10: 7468 2e73 7472 7563 7428 290a 0a20 2020  th.struct()..   
-00001a20: 2064 6566 2069 735f 6461 7461 5f76 616c   def is_data_val
-00001a30: 6964 2873 656c 662c 2076 616c 6964 6174  id(self, validat
-00001a40: 6f72 3a20 5661 6c69 6461 746f 7229 202d  or: Validator) -
-00001a50: 3e20 4661 696c 7572 653a 0a20 2020 2020  > Failure:.     
-00001a60: 2020 2072 6574 7572 6e20 7661 6c69 6461     return valida
-00001a70: 746f 722e 6765 745f 7661 6c69 6461 746f  tor.get_validato
-00001a80: 7228 7479 7065 2873 656c 6629 2928 7365  r(type(self))(se
-00001a90: 6c66 2e64 6967 6573 742c 2073 656c 662e  lf.digest, self.
-00001aa0: 7061 7468 290a 0a0a 636c 6173 7320 496d  path)...class Im
-00001ab0: 614e 6728 4d6f 6465 293a 0a20 2020 2022  aNg(Mode):.    "
-00001ac0: 2222 0a20 2020 2043 6c61 7373 2066 6f72  "".    Class for
-00001ad0: 2022 696d 612d 6e67 222e 2043 6f6e 7461   "ima-ng". Conta
-00001ae0: 696e 7320 7468 6520 6469 6765 7374 2061  ins the digest a
-00001af0: 6e64 2061 2070 6174 682e 0a20 2020 2022  nd a path..    "
-00001b00: 2222 0a0a 2020 2020 6469 6765 7374 3a20  ""..    digest: 
-00001b10: 4469 6765 7374 0a20 2020 2070 6174 683a  Digest.    path:
-00001b20: 204e 616d 650a 0a20 2020 2064 6566 205f   Name..    def _
-00001b30: 5f69 6e69 745f 5f28 7365 6c66 2c20 6461  _init__(self, da
-00001b40: 7461 3a20 7374 7229 3a0a 2020 2020 2020  ta: str):.      
-00001b50: 2020 746f 6b65 6e73 203d 2064 6174 612e    tokens = data.
-00001b60: 7370 6c69 7428 2220 222c 206d 6178 7370  split(" ", maxsp
-00001b70: 6c69 743d 3129 0a20 2020 2020 2020 2069  lit=1).        i
-00001b80: 6620 6c65 6e28 746f 6b65 6e73 2920 213d  f len(tokens) !=
-00001b90: 2032 3a0a 2020 2020 2020 2020 2020 2020   2:.            
-00001ba0: 7261 6973 6520 5061 7273 6572 4572 726f  raise ParserErro
-00001bb0: 7228 6622 4361 6e6e 6f74 2063 7265 6174  r(f"Cannot creat
-00001bc0: 6520 496d 614e 6720 6578 7065 6374 6564  e ImaNg expected
-00001bd0: 2032 2074 6f6b 656e 7320 676f 743a 207b   2 tokens got: {
-00001be0: 6c65 6e28 746f 6b65 6e73 297d 2e22 290a  len(tokens)}.").
-00001bf0: 2020 2020 2020 2020 7365 6c66 2e64 6967          self.dig
-00001c00: 6573 7420 3d20 4469 6765 7374 2874 6f6b  est = Digest(tok
-00001c10: 656e 735b 305d 290a 2020 2020 2020 2020  ens[0]).        
-00001c20: 7365 6c66 2e70 6174 6820 3d20 4e61 6d65  self.path = Name
-00001c30: 2874 6f6b 656e 735b 315d 290a 0a20 2020  (tokens[1])..   
-00001c40: 2064 6566 2062 7974 6573 2873 656c 6629   def bytes(self)
-00001c50: 202d 3e20 6279 7465 733a 0a20 2020 2020   -> bytes:.     
-00001c60: 2020 2072 6574 7572 6e20 7365 6c66 2e64     return self.d
-00001c70: 6967 6573 742e 7374 7275 6374 2829 202b  igest.struct() +
-00001c80: 2073 656c 662e 7061 7468 2e73 7472 7563   self.path.struc
-00001c90: 7428 290a 0a20 2020 2064 6566 2069 735f  t()..    def is_
-00001ca0: 6461 7461 5f76 616c 6964 2873 656c 662c  data_valid(self,
-00001cb0: 2076 616c 6964 6174 6f72 3a20 5661 6c69   validator: Vali
-00001cc0: 6461 746f 7229 202d 3e20 4661 696c 7572  dator) -> Failur
-00001cd0: 653a 0a20 2020 2020 2020 2072 6574 7572  e:.        retur
-00001ce0: 6e20 7661 6c69 6461 746f 722e 6765 745f  n validator.get_
-00001cf0: 7661 6c69 6461 746f 7228 7479 7065 2873  validator(type(s
-00001d00: 656c 6629 2928 7365 6c66 2e64 6967 6573  elf))(self.diges
-00001d10: 742c 2073 656c 662e 7061 7468 290a 0a0a  t, self.path)...
-00001d20: 636c 6173 7320 496d 6153 6967 284d 6f64  class ImaSig(Mod
-00001d30: 6529 3a0a 2020 2020 2222 220a 2020 2020  e):.    """.    
-00001d40: 436c 6173 7320 666f 7220 2269 6d61 2d73  Class for "ima-s
-00001d50: 6967 2220 7465 6d70 6c61 7465 2e20 4e65  ig" template. Ne
-00001d60: 6172 6c79 2074 6865 2073 616d 6520 6173  arly the same as
-00001d70: 2049 6d61 4e67 2062 7574 2063 616e 2063   ImaNg but can c
-00001d80: 6f6e 7461 696e 2061 206f 7074 696f 6e61  ontain a optiona
-00001d90: 6c20 7369 676e 6174 7572 652e 0a20 2020  l signature..   
-00001da0: 2022 2222 0a0a 2020 2020 6469 6765 7374   """..    digest
-00001db0: 3a20 4469 6765 7374 0a20 2020 2070 6174  : Digest.    pat
-00001dc0: 683a 204e 616d 650a 2020 2020 7369 676e  h: Name.    sign
-00001dd0: 6174 7572 653a 204f 7074 696f 6e61 6c5b  ature: Optional[
-00001de0: 5369 676e 6174 7572 655d 203d 204e 6f6e  Signature] = Non
-00001df0: 650a 0a20 2020 2064 6566 205f 5f69 6e69  e..    def __ini
-00001e00: 745f 5f28 7365 6c66 2c20 6461 7461 3a20  t__(self, data: 
-00001e10: 7374 7229 3a0a 2020 2020 2020 2020 2320  str):.        # 
-00001e20: 5468 6572 6520 6172 6520 616c 7761 7973  There are always
-00001e30: 2033 2066 6965 6c64 7320 696e 2061 2076   3 fields in a v
-00001e40: 616c 6964 2065 6e74 7279 2c20 6265 6361  alid entry, beca
-00001e50: 7573 653a 0a20 2020 2020 2020 2023 0a20  use:.        #. 
-00001e60: 2020 2020 2020 2023 202d 206e 2d6e 6720         # - n-ng 
-00001e70: 646f 6573 206e 6f74 2063 6f6e 7461 696e  does not contain
-00001e80: 2061 2073 7061 6365 2063 6861 7261 6374   a space charact
-00001e90: 6572 2c20 6173 2069 7420 6973 2065 7363  er, as it is esc
-00001ea0: 6170 6564 2074 6f20 616e 0a20 2020 2020  aped to an.     
-00001eb0: 2020 2023 2020 2075 6e64 6572 7363 6f72     #   underscor
-00001ec0: 6520 2822 5f22 293a 0a20 2020 2020 2020  e ("_"):.       
-00001ed0: 2023 2020 2068 7474 7073 3a2f 2f65 6c69   #   https://eli
-00001ee0: 7869 722e 626f 6f74 6c69 6e2e 636f 6d2f  xir.bootlin.com/
-00001ef0: 6c69 6e75 782f 7635 2e31 382f 736f 7572  linux/v5.18/sour
-00001f00: 6365 2f73 6563 7572 6974 792f 696e 7465  ce/security/inte
-00001f10: 6772 6974 792f 696d 612f 696d 615f 7465  grity/ima/ima_te
-00001f20: 6d70 6c61 7465 5f6c 6962 2e63 234c 3535  mplate_lib.c#L55
-00001f30: 0a20 2020 2020 2020 2023 202d 2074 6865  .        # - the
-00001f40: 206c 6173 7420 6669 656c 6420 636f 756c   last field coul
-00001f50: 6420 6265 2061 6e20 656d 7074 7920 7374  d be an empty st
-00001f60: 7269 6e67 2062 7574 2061 2064 656c 696d  ring but a delim
-00001f70: 6974 6572 2028 2220 2229 2073 686f 756c  iter (" ") shoul
-00001f80: 640a 2020 2020 2020 2020 2320 2020 7374  d.        #   st
-00001f90: 696c 6c20 7072 6573 656e 743a 0a20 2020  ill present:.   
-00001fa0: 2020 2020 2023 2020 2068 7474 7073 3a2f       #   https:/
-00001fb0: 2f65 6c69 7869 722e 626f 6f74 6c69 6e2e  /elixir.bootlin.
-00001fc0: 636f 6d2f 6c69 6e75 782f 7635 2e31 382f  com/linux/v5.18/
-00001fd0: 736f 7572 6365 2f73 6563 7572 6974 792f  source/security/
-00001fe0: 696e 7465 6772 6974 792f 696d 612f 696d  integrity/ima/im
-00001ff0: 615f 6673 2e63 234c 3234 340a 2020 2020  a_fs.c#L244.    
-00002000: 2020 2020 746f 6b65 6e73 203d 2064 6174      tokens = dat
-00002010: 612e 7370 6c69 7428 2220 222c 206d 6178  a.split(" ", max
-00002020: 7370 6c69 743d 3229 0a20 2020 2020 2020  split=2).       
-00002030: 2069 6620 6c65 6e28 746f 6b65 6e73 2920   if len(tokens) 
-00002040: 213d 2033 3a0a 2020 2020 2020 2020 2020  != 3:.          
-00002050: 2020 7261 6973 6520 5061 7273 6572 4572    raise ParserEr
-00002060: 726f 7228 6622 4361 6e6e 6f74 2063 7265  ror(f"Cannot cre
-00002070: 6174 6520 496d 6153 6967 2065 7870 6563  ate ImaSig expec
-00002080: 7465 6420 3320 746f 6b65 6e73 2067 6f74  ted 3 tokens got
-00002090: 3a20 7b6c 656e 2874 6f6b 656e 7329 7d2e  : {len(tokens)}.
-000020a0: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
-000020b0: 6469 6765 7374 203d 2044 6967 6573 7428  digest = Digest(
-000020c0: 746f 6b65 6e73 5b30 5d29 0a20 2020 2020  tokens[0]).     
-000020d0: 2020 2073 656c 662e 7061 7468 203d 204e     self.path = N
-000020e0: 616d 6528 746f 6b65 6e73 5b31 5d29 0a20  ame(tokens[1]). 
-000020f0: 2020 2020 2020 2073 656c 662e 7369 676e         self.sign
-00002100: 6174 7572 6520 3d20 7365 6c66 2e63 7265  ature = self.cre
-00002110: 6174 655f 7369 676e 6174 7572 6528 746f  ate_signature(to
-00002120: 6b65 6e73 5b32 5d29 0a0a 2020 2020 4073  kens[2])..    @s
-00002130: 7461 7469 636d 6574 686f 640a 2020 2020  taticmethod.    
-00002140: 6465 6620 6372 6561 7465 5f73 6967 6e61  def create_signa
-00002150: 7475 7265 2868 6578 7374 7269 6e67 3a20  ture(hexstring: 
-00002160: 7374 7229 202d 3e20 4f70 7469 6f6e 616c  str) -> Optional
-00002170: 5b53 6967 6e61 7475 7265 5d3a 0a20 2020  [Signature]:.   
-00002180: 2020 2020 2022 2222 4372 6561 7465 2074       """Create t
-00002190: 6865 2053 6967 6e61 7475 7265 206f 626a  he Signature obj
-000021a0: 6563 7420 6966 2074 6865 2068 6578 7374  ect if the hexst
-000021b0: 7269 6e67 2069 7320 6120 7661 6c69 6420  ring is a valid 
-000021c0: 7369 676e 6174 7572 6522 2222 0a20 2020  signature""".   
-000021d0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-000021e0: 2020 2020 2020 7265 7475 726e 2053 6967        return Sig
-000021f0: 6e61 7475 7265 2868 6578 7374 7269 6e67  nature(hexstring
-00002200: 290a 2020 2020 2020 2020 6578 6365 7074  ).        except
-00002210: 2050 6172 7365 7245 7272 6f72 3a0a 2020   ParserError:.  
-00002220: 2020 2020 2020 2020 2020 7061 7373 0a20            pass. 
-00002230: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
-00002240: 6e65 0a0a 2020 2020 6465 6620 6279 7465  ne..    def byte
-00002250: 7328 7365 6c66 2920 2d3e 2062 7974 6573  s(self) -> bytes
-00002260: 3a0a 2020 2020 2020 2020 6f75 7470 7574  :.        output
-00002270: 203d 2073 656c 662e 6469 6765 7374 2e73   = self.digest.s
-00002280: 7472 7563 7428 2920 2b20 7365 6c66 2e70  truct() + self.p
-00002290: 6174 682e 7374 7275 6374 2829 0a20 2020  ath.struct().   
-000022a0: 2020 2020 2023 2049 6620 6e6f 2073 6967       # If no sig
-000022b0: 6e61 7475 7265 2069 7320 7468 6572 6520  nature is there 
-000022c0: 7765 2073 696c 6c20 6861 7665 2074 6f20  we sill have to 
-000022d0: 6164 6420 7468 6520 656e 7472 7920 666f  add the entry fo
-000022e0: 7220 6974 0a20 2020 2020 2020 2069 6620  r it.        if 
-000022f0: 7365 6c66 2e73 6967 6e61 7475 7265 2069  self.signature i
-00002300: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00002310: 2020 2020 6f75 7470 7574 202b 3d20 7374      output += st
-00002320: 7275 6374 2e70 6163 6b28 223c 4930 7322  ruct.pack("<I0s"
-00002330: 2c20 302c 2062 2222 290a 2020 2020 2020  , 0, b"").      
-00002340: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00002350: 2020 2020 6f75 7470 7574 202b 3d20 7365      output += se
-00002360: 6c66 2e73 6967 6e61 7475 7265 2e73 7472  lf.signature.str
-00002370: 7563 7428 290a 2020 2020 2020 2020 7265  uct().        re
-00002380: 7475 726e 206f 7574 7075 740a 0a20 2020  turn output..   
-00002390: 2064 6566 2069 735f 6461 7461 5f76 616c   def is_data_val
-000023a0: 6964 2873 656c 662c 2076 616c 6964 6174  id(self, validat
-000023b0: 6f72 3a20 5661 6c69 6461 746f 7229 202d  or: Validator) -
-000023c0: 3e20 4661 696c 7572 653a 0a20 2020 2020  > Failure:.     
-000023d0: 2020 2072 6574 7572 6e20 7661 6c69 6461     return valida
-000023e0: 746f 722e 6765 745f 7661 6c69 6461 746f  tor.get_validato
-000023f0: 7228 7479 7065 2873 656c 6629 2928 7365  r(type(self))(se
-00002400: 6c66 2e64 6967 6573 742c 2073 656c 662e  lf.digest, self.
-00002410: 7061 7468 2c20 7365 6c66 2e73 6967 6e61  path, self.signa
-00002420: 7475 7265 290a 0a0a 636c 6173 7320 496d  ture)...class Im
-00002430: 6142 7566 284d 6f64 6529 3a0a 2020 2020  aBuf(Mode):.    
-00002440: 2222 220a 2020 2020 436c 6173 7320 666f  """.    Class fo
-00002450: 7220 2269 6d61 2d62 7566 222e 2043 6f6e  r "ima-buf". Con
-00002460: 7461 696e 7320 6120 6469 6765 7374 2c20  tains a digest, 
-00002470: 6275 6666 6572 206e 616d 6520 616e 6420  buffer name and 
-00002480: 7468 6520 6275 6666 6572 2069 7473 656c  the buffer itsel
-00002490: 662e 0a20 2020 2046 6f72 2076 616c 6964  f..    For valid
-000024a0: 6174 696f 6e20 7468 6520 6275 6666 6572  ation the buffer
-000024b0: 206d 7573 7420 6265 2064 6f6e 6520 6261   must be done ba
-000024c0: 7365 6420 6f6e 2074 6865 206e 616d 6520  sed on the name 
-000024d0: 6265 6361 7573 6520 494d 4120 6f6e 6c79  because IMA only
-000024e0: 2070 726f 7669 6465 7320 6974 2061 7320   provides it as 
-000024f0: 616e 2062 7974 6520 6172 7261 792e 0a20  an byte array.. 
-00002500: 2020 2022 2222 0a0a 2020 2020 6469 6765     """..    dige
-00002510: 7374 3a20 4469 6765 7374 0a20 2020 206e  st: Digest.    n
-00002520: 616d 653a 204e 616d 650a 2020 2020 6461  ame: Name.    da
-00002530: 7461 3a20 4275 6666 6572 0a0a 2020 2020  ta: Buffer..    
-00002540: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-00002550: 662c 2064 6174 613a 2073 7472 293a 0a20  f, data: str):. 
-00002560: 2020 2020 2020 2023 2054 6865 7265 2061         # There a
-00002570: 7265 2061 6c77 6179 7320 3320 6669 656c  re always 3 fiel
-00002580: 6473 2069 6e20 6120 7661 6c69 6420 656e  ds in a valid en
-00002590: 7472 792c 2062 6563 6175 7365 3a0a 2020  try, because:.  
-000025a0: 2020 2020 2020 230a 2020 2020 2020 2020        #.        
-000025b0: 2320 2d20 6e2d 6e67 2064 6f65 7320 6e6f  # - n-ng does no
-000025c0: 7420 636f 6e74 6169 6e20 6120 7370 6163  t contain a spac
-000025d0: 6520 6368 6172 6163 7465 722c 2061 7320  e character, as 
-000025e0: 6974 2069 7320 6573 6361 7065 6420 746f  it is escaped to
-000025f0: 2061 6e0a 2020 2020 2020 2020 2320 2020   an.        #   
-00002600: 756e 6465 7273 636f 7265 2028 225f 2229  underscore ("_")
-00002610: 3a0a 2020 2020 2020 2020 2320 2020 6874  :.        #   ht
-00002620: 7470 733a 2f2f 656c 6978 6972 2e62 6f6f  tps://elixir.boo
-00002630: 746c 696e 2e63 6f6d 2f6c 696e 7578 2f76  tlin.com/linux/v
-00002640: 352e 3138 2f73 6f75 7263 652f 7365 6375  5.18/source/secu
-00002650: 7269 7479 2f69 6e74 6567 7269 7479 2f69  rity/integrity/i
-00002660: 6d61 2f69 6d61 5f74 656d 706c 6174 655f  ma/ima_template_
-00002670: 6c69 622e 6323 4c35 350a 2020 2020 2020  lib.c#L55.      
-00002680: 2020 2320 2d20 7468 6520 6c61 7374 2066    # - the last f
-00002690: 6965 6c64 2063 6f75 6c64 2062 6520 616e  ield could be an
-000026a0: 2065 6d70 7479 2073 7472 696e 6720 6275   empty string bu
-000026b0: 7420 6120 6465 6c69 6d69 7465 7220 2822  t a delimiter ("
-000026c0: 2022 2920 7368 6f75 6c64 0a20 2020 2020   ") should.     
-000026d0: 2020 2023 2020 2073 7469 6c6c 2070 7265     #   still pre
-000026e0: 7365 6e74 3a0a 2020 2020 2020 2020 2320  sent:.        # 
-000026f0: 2020 6874 7470 733a 2f2f 656c 6978 6972    https://elixir
-00002700: 2e62 6f6f 746c 696e 2e63 6f6d 2f6c 696e  .bootlin.com/lin
-00002710: 7578 2f76 352e 3138 2f73 6f75 7263 652f  ux/v5.18/source/
-00002720: 7365 6375 7269 7479 2f69 6e74 6567 7269  security/integri
-00002730: 7479 2f69 6d61 2f69 6d61 5f66 732e 6323  ty/ima/ima_fs.c#
-00002740: 4c32 3434 0a20 2020 2020 2020 2074 6f6b  L244.        tok
-00002750: 656e 7320 3d20 6461 7461 2e73 706c 6974  ens = data.split
-00002760: 2822 2022 2c20 6d61 7873 706c 6974 3d32  (" ", maxsplit=2
-00002770: 290a 2020 2020 2020 2020 6966 206c 656e  ).        if len
-00002780: 2874 6f6b 656e 7329 2021 3d20 333a 0a20  (tokens) != 3:. 
-00002790: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-000027a0: 2050 6172 7365 7245 7272 6f72 2866 2243   ParserError(f"C
-000027b0: 616e 6e6f 7420 6372 6561 7465 2049 6d61  annot create Ima
-000027c0: 4275 6620 6578 7065 6374 6564 2033 2074  Buf expected 3 t
-000027d0: 6f6b 656e 7320 676f 743a 207b 6c65 6e28  okens got: {len(
-000027e0: 746f 6b65 6e73 297d 2e22 290a 2020 2020  tokens)}.").    
-000027f0: 2020 2020 7365 6c66 2e64 6967 6573 7420      self.digest 
-00002800: 3d20 4469 6765 7374 2874 6f6b 656e 735b  = Digest(tokens[
-00002810: 305d 290a 2020 2020 2020 2020 7365 6c66  0]).        self
-00002820: 2e6e 616d 6520 3d20 4e61 6d65 2874 6f6b  .name = Name(tok
-00002830: 656e 735b 315d 290a 2020 2020 2020 2020  ens[1]).        
-00002840: 7365 6c66 2e64 6174 6120 3d20 4275 6666  self.data = Buff
-00002850: 6572 2874 6f6b 656e 735b 325d 290a 0a20  er(tokens[2]).. 
-00002860: 2020 2064 6566 2062 7974 6573 2873 656c     def bytes(sel
-00002870: 6629 202d 3e20 6279 7465 733a 0a20 2020  f) -> bytes:.   
-00002880: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00002890: 2e64 6967 6573 742e 7374 7275 6374 2829  .digest.struct()
-000028a0: 202b 2073 656c 662e 6e61 6d65 2e73 7472   + self.name.str
-000028b0: 7563 7428 2920 2b20 7365 6c66 2e64 6174  uct() + self.dat
-000028c0: 612e 7374 7275 6374 2829 0a0a 2020 2020  a.struct()..    
-000028d0: 6465 6620 6973 5f64 6174 615f 7661 6c69  def is_data_vali
-000028e0: 6428 7365 6c66 2c20 7661 6c69 6461 746f  d(self, validato
-000028f0: 723a 2056 616c 6964 6174 6f72 2920 2d3e  r: Validator) ->
-00002900: 2046 6169 6c75 7265 3a0a 2020 2020 2020   Failure:.      
-00002910: 2020 7265 7475 726e 2076 616c 6964 6174    return validat
-00002920: 6f72 2e67 6574 5f76 616c 6964 6174 6f72  or.get_validator
-00002930: 2874 7970 6528 7365 6c66 2929 2873 656c  (type(self))(sel
-00002940: 662e 6469 6765 7374 2c20 7365 6c66 2e6e  f.digest, self.n
-00002950: 616d 652c 2073 656c 662e 6461 7461 290a  ame, self.data).
-00002960: 0a0a 636c 6173 7320 456e 7472 793a 0a20  ..class Entry:. 
-00002970: 2020 2022 2222 0a20 2020 2049 4d41 2045     """.    IMA E
-00002980: 6e74 7279 2e20 436f 6e74 6169 6e73 2074  ntry. Contains t
-00002990: 6865 2050 4352 2c20 7465 6d70 6c61 7465  he PCR, template
-000029a0: 2068 6173 6820 616e 6420 6d6f 6465 2e0a   hash and mode..
-000029b0: 2020 2020 2222 220a 0a20 2020 2070 6372      """..    pcr
-000029c0: 3a20 7374 720a 2020 2020 696d 615f 7465  : str.    ima_te
-000029d0: 6d70 6c61 7465 5f68 6173 683a 2062 7974  mplate_hash: byt
-000029e0: 6573 0a20 2020 2070 6372 5f74 656d 706c  es.    pcr_templ
-000029f0: 6174 655f 6861 7368 3a20 6279 7465 730a  ate_hash: bytes.
-00002a00: 2020 2020 6d6f 6465 3a20 4d6f 6465 0a20      mode: Mode. 
-00002a10: 2020 205f 6279 7465 733a 2062 7974 6573     _bytes: bytes
-00002a20: 0a20 2020 205f 7661 6c69 6461 746f 723a  .    _validator:
-00002a30: 204f 7074 696f 6e61 6c5b 5661 6c69 6461   Optional[Valida
-00002a40: 746f 725d 0a20 2020 205f 696d 615f 6861  tor].    _ima_ha
-00002a50: 7368 5f61 6c67 3a20 4861 7368 0a20 2020  sh_alg: Hash.   
-00002a60: 205f 7063 725f 6861 7368 5f61 6c67 3a20   _pcr_hash_alg: 
-00002a70: 4861 7368 0a0a 2020 2020 5f6d 6f64 655f  Hash..    _mode_
-00002a80: 6c6f 6f6b 7570 3a20 4469 6374 5b73 7472  lookup: Dict[str
-00002a90: 2c20 556e 696f 6e5b 7479 7069 6e67 2e54  , Union[typing.T
-00002aa0: 7970 655b 496d 615d 2c20 7479 7069 6e67  ype[Ima], typing
-00002ab0: 2e54 7970 655b 496d 614e 675d 2c20 7479  .Type[ImaNg], ty
-00002ac0: 7069 6e67 2e54 7970 655b 496d 6153 6967  ping.Type[ImaSig
-00002ad0: 5d2c 2074 7970 696e 672e 5479 7065 5b49  ], typing.Type[I
-00002ae0: 6d61 4275 665d 5d5d 203d 207b 0a20 2020  maBuf]]] = {.   
-00002af0: 2020 2020 2022 696d 6122 3a20 496d 612c       "ima": Ima,
-00002b00: 0a20 2020 2020 2020 2022 696d 612d 6e67  .        "ima-ng
-00002b10: 223a 2049 6d61 4e67 2c0a 2020 2020 2020  ": ImaNg,.      
-00002b20: 2020 2269 6d61 2d73 6967 223a 2049 6d61    "ima-sig": Ima
-00002b30: 5369 672c 0a20 2020 2020 2020 2022 696d  Sig,.        "im
-00002b40: 612d 6275 6622 3a20 496d 6142 7566 2c0a  a-buf": ImaBuf,.
-00002b50: 2020 2020 7d0a 0a20 2020 2064 6566 205f      }..    def _
-00002b60: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-00002b70: 2073 656c 662c 0a20 2020 2020 2020 2064   self,.        d
-00002b80: 6174 613a 2073 7472 2c0a 2020 2020 2020  ata: str,.      
-00002b90: 2020 7661 6c69 6461 746f 723a 204f 7074    validator: Opt
-00002ba0: 696f 6e61 6c5b 5661 6c69 6461 746f 725d  ional[Validator]
-00002bb0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00002bc0: 2069 6d61 5f68 6173 685f 616c 673a 2048   ima_hash_alg: H
-00002bd0: 6173 6820 3d20 4861 7368 2e53 4841 312c  ash = Hash.SHA1,
-00002be0: 0a20 2020 2020 2020 2070 6372 5f68 6173  .        pcr_has
-00002bf0: 685f 616c 673a 2048 6173 6820 3d20 4861  h_alg: Hash = Ha
-00002c00: 7368 2e53 4841 312c 0a20 2020 2029 3a0a  sh.SHA1,.    ):.
-00002c10: 2020 2020 2020 2020 7365 6c66 2e5f 7661          self._va
-00002c20: 6c69 6461 746f 7220 3d20 7661 6c69 6461  lidator = valida
-00002c30: 746f 720a 2020 2020 2020 2020 7365 6c66  tor.        self
-00002c40: 2e5f 696d 615f 6861 7368 5f61 6c67 203d  ._ima_hash_alg =
-00002c50: 2069 6d61 5f68 6173 685f 616c 670a 2020   ima_hash_alg.  
-00002c60: 2020 2020 2020 7365 6c66 2e5f 7063 725f        self._pcr_
-00002c70: 6861 7368 5f61 6c67 203d 2070 6372 5f68  hash_alg = pcr_h
-00002c80: 6173 685f 616c 670a 2020 2020 2020 2020  ash_alg.        
-00002c90: 746f 6b65 6e73 203d 2064 6174 612e 7370  tokens = data.sp
-00002ca0: 6c69 7428 2220 222c 206d 6178 7370 6c69  lit(" ", maxspli
-00002cb0: 743d 3329 0a20 2020 2020 2020 2069 6620  t=3).        if 
-00002cc0: 6c65 6e28 746f 6b65 6e73 2920 213d 2034  len(tokens) != 4
-00002cd0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-00002ce0: 6973 6520 5061 7273 6572 4572 726f 7228  ise ParserError(
-00002cf0: 6622 4361 6e6e 6f74 2063 7265 6174 6520  f"Cannot create 
-00002d00: 456e 7472 7920 6578 7065 6374 6564 2034  Entry expected 4
-00002d10: 2074 6f6b 656e 7320 676f 743a 207b 6c65   tokens got: {le
-00002d20: 6e28 746f 6b65 6e73 297d 2e22 290a 2020  n(tokens)}.").  
-00002d30: 2020 2020 2020 7365 6c66 2e70 6372 203d        self.pcr =
-00002d40: 2074 6f6b 656e 735b 305d 0a20 2020 2020   tokens[0].     
-00002d50: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00002d60: 2020 2020 7365 6c66 2e69 6d61 5f74 656d      self.ima_tem
-00002d70: 706c 6174 655f 6861 7368 203d 2063 6f64  plate_hash = cod
-00002d80: 6563 732e 6465 636f 6465 2874 6f6b 656e  ecs.decode(token
-00002d90: 735b 315d 2e65 6e63 6f64 6528 292c 2022  s[1].encode(), "
-00002da0: 6865 7822 290a 2020 2020 2020 2020 6578  hex").        ex
-00002db0: 6365 7074 2062 696e 6173 6369 692e 4572  cept binascii.Er
-00002dc0: 726f 7220 6173 2065 3a0a 2020 2020 2020  ror as e:.      
-00002dd0: 2020 2020 2020 7261 6973 6520 5061 7273        raise Pars
-00002de0: 6572 4572 726f 7228 6622 4361 6e6e 6f74  erError(f"Cannot
-00002df0: 2063 7265 6174 6520 456e 7472 7920 6578   create Entry ex
-00002e00: 7065 6374 6564 2034 2074 6f6b 656e 7320  pected 4 tokens 
-00002e10: 676f 743a 207b 6c65 6e28 746f 6b65 6e73  got: {len(tokens
-00002e20: 297d 2e22 2920 6672 6f6d 2065 0a0a 2020  )}.") from e..  
-00002e30: 2020 2020 2020 6d6f 6465 203d 2073 656c        mode = sel
-00002e40: 662e 5f6d 6f64 655f 6c6f 6f6b 7570 2e67  f._mode_lookup.g
-00002e50: 6574 2874 6f6b 656e 735b 325d 2c20 4e6f  et(tokens[2], No
-00002e60: 6e65 290a 2020 2020 2020 2020 6966 206d  ne).        if m
-00002e70: 6f64 6520 6973 204e 6f6e 653a 0a20 2020  ode is None:.   
-00002e80: 2020 2020 2020 2020 2072 6169 7365 2050           raise P
-00002e90: 6172 7365 7245 7272 6f72 2866 224e 6f20  arserError(f"No 
-00002ea0: 7061 7273 6572 2066 6f72 206d 6f64 6520  parser for mode 
-00002eb0: 7b74 6f6b 656e 735b 325d 7d20 696d 706c  {tokens[2]} impl
-00002ec0: 656d 656e 7465 642e 2229 0a20 2020 2020  emented.").     
-00002ed0: 2020 2073 656c 662e 6d6f 6465 203d 206d     self.mode = m
-00002ee0: 6f64 6528 746f 6b65 6e73 5b33 5d29 0a20  ode(tokens[3]). 
-00002ef0: 2020 2020 2020 2073 656c 662e 5f62 7974         self._byt
-00002f00: 6573 203d 2073 656c 662e 6d6f 6465 2e62  es = self.mode.b
-00002f10: 7974 6573 2829 0a20 2020 2020 2020 2073  ytes().        s
-00002f20: 656c 662e 7063 725f 7465 6d70 6c61 7465  elf.pcr_template
-00002f30: 5f68 6173 6820 3d20 7365 6c66 2e5f 7063  _hash = self._pc
-00002f40: 725f 6861 7368 5f61 6c67 2e68 6173 6828  r_hash_alg.hash(
-00002f50: 7365 6c66 2e5f 6279 7465 7329 0a20 2020  self._bytes).   
-00002f60: 2020 2020 2023 2053 6574 2063 6f72 7265       # Set corre
-00002f70: 6374 2068 6173 6820 666f 7220 7469 6d65  ct hash for time
-00002f80: 206f 6620 6d65 6173 7572 652c 2074 696d   of measure, tim
-00002f90: 6520 6f66 2075 7365 2028 546f 4d54 6f55  e of use (ToMToU
-00002fa0: 2920 6572 726f 7273 0a20 2020 2020 2020  ) errors.       
-00002fb0: 2023 2061 6e64 2069 6620 6120 6669 6c65   # and if a file
-00002fc0: 2069 7320 616c 7265 6164 7920 6f70 656e   is already open
-00002fd0: 6564 2066 6f72 2077 7269 7465 2e0a 2020  ed for write..  
-00002fe0: 2020 2020 2020 2320 6874 7470 733a 2f2f        # https://
-00002ff0: 656c 6978 6972 2e62 6f6f 746c 696e 2e63  elixir.bootlin.c
-00003000: 6f6d 2f6c 696e 7578 2f76 352e 3132 2e31  om/linux/v5.12.1
-00003010: 322f 736f 7572 6365 2f73 6563 7572 6974  2/source/securit
-00003020: 792f 696e 7465 6772 6974 792f 696d 612f  y/integrity/ima/
-00003030: 696d 615f 6d61 696e 2e63 234c 3130 310a  ima_main.c#L101.
-00003040: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00003050: 696d 615f 7465 6d70 6c61 7465 5f68 6173  ima_template_has
-00003060: 6820 3d3d 2067 6574 5f53 5441 5254 5f48  h == get_START_H
-00003070: 4153 4828 696d 615f 6861 7368 5f61 6c67  ASH(ima_hash_alg
-00003080: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-00003090: 656c 662e 696d 615f 7465 6d70 6c61 7465  elf.ima_template
-000030a0: 5f68 6173 6820 3d20 6765 745f 4646 5f48  _hash = get_FF_H
-000030b0: 4153 4828 696d 615f 6861 7368 5f61 6c67  ASH(ima_hash_alg
-000030c0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-000030d0: 6c66 2e70 6372 5f74 656d 706c 6174 655f  lf.pcr_template_
-000030e0: 6861 7368 203d 2067 6574 5f46 465f 4841  hash = get_FF_HA
-000030f0: 5348 2870 6372 5f68 6173 685f 616c 6729  SH(pcr_hash_alg)
-00003100: 0a0a 2020 2020 6465 6620 696e 7661 6c69  ..    def invali
-00003110: 6428 7365 6c66 2920 2d3e 2046 6169 6c75  d(self) -> Failu
-00003120: 7265 3a0a 2020 2020 2020 2020 6661 696c  re:.        fail
-00003130: 7572 6520 3d20 4661 696c 7572 6528 436f  ure = Failure(Co
-00003140: 6d70 6f6e 656e 742e 494d 412c 205b 2276  mponent.IMA, ["v
-00003150: 616c 6964 6174 696f 6e22 5d29 0a20 2020  alidation"]).   
-00003160: 2020 2020 2069 6620 7365 6c66 2e70 6372       if self.pcr
-00003170: 2021 3d20 7374 7228 636f 6e66 6967 2e49   != str(config.I
-00003180: 4d41 5f50 4352 293a 0a20 2020 2020 2020  MA_PCR):.       
-00003190: 2020 2020 206c 6f67 6765 722e 7761 726e       logger.warn
-000031a0: 696e 6728 2249 4d41 2065 6e74 7279 2050  ing("IMA entry P
-000031b0: 4352 2064 6f65 7320 6e6f 7420 6d61 7463  CR does not matc
-000031c0: 6820 2573 2e20 4974 2077 6173 3a20 2573  h %s. It was: %s
-000031d0: 222c 2063 6f6e 6669 672e 494d 415f 5043  ", config.IMA_PC
-000031e0: 522c 2073 656c 662e 7063 7229 0a20 2020  R, self.pcr).   
-000031f0: 2020 2020 2020 2020 2066 6169 6c75 7265           failure
-00003200: 2e61 6464 5f65 7665 6e74 280a 2020 2020  .add_event(.    
-00003210: 2020 2020 2020 2020 2020 2020 2269 6d61              "ima
-00003220: 5f70 6372 222c 0a20 2020 2020 2020 2020  _pcr",.         
-00003230: 2020 2020 2020 207b 226d 6573 7361 6765         {"message
-00003240: 223a 2022 494d 4120 5043 5220 6973 206e  ": "IMA PCR is n
-00003250: 6f74 2074 6865 2063 6f6e 6669 6775 7265  ot the configure
-00003260: 6420 6f6e 6522 2c20 2265 7870 6563 7465  d one", "expecte
-00003270: 6422 3a20 7374 7228 636f 6e66 6967 2e49  d": str(config.I
-00003280: 4d41 5f50 4352 292c 2022 676f 7422 3a20  MA_PCR), "got": 
-00003290: 7365 6c66 2e70 6372 7d2c 0a20 2020 2020  self.pcr},.     
-000032a0: 2020 2020 2020 2020 2020 2054 7275 652c             True,
-000032b0: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-000032c0: 2020 2020 2020 2020 2320 4967 6e6f 7265          # Ignore
-000032d0: 2074 656d 706c 6174 6520 6861 7368 2066   template hash f
-000032e0: 6f72 2054 6f4d 546f 5520 6572 726f 7273  or ToMToU errors
-000032f0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00003300: 2e69 6d61 5f74 656d 706c 6174 655f 6861  .ima_template_ha
-00003310: 7368 203d 3d20 6765 745f 4646 5f48 4153  sh == get_FF_HAS
-00003320: 4828 7365 6c66 2e5f 696d 615f 6861 7368  H(self._ima_hash
-00003330: 5f61 6c67 293a 0a20 2020 2020 2020 2020  _alg):.         
-00003340: 2020 206c 6f67 6765 722e 7761 726e 696e     logger.warnin
-00003350: 6728 2253 6b69 7070 6564 2074 656d 706c  g("Skipped templ
-00003360: 6174 655f 6861 7368 2076 616c 6964 6174  ate_hash validat
-00003370: 696f 6e20 656e 7472 7920 7769 7468 2046  ion entry with F
-00003380: 465f 4841 5348 2229 0a20 2020 2020 2020  F_HASH").       
-00003390: 2020 2020 2023 2042 7920 6465 6661 756c       # By defaul
-000033a0: 7420 546f 4d54 6f55 2065 7272 6f72 7320  t ToMToU errors 
-000033b0: 6172 6520 6e6f 7420 7472 6561 7465 6420  are not treated 
-000033c0: 6173 2061 2066 6169 6c75 7265 0a20 2020  as a failure.   
-000033d0: 2020 2020 2020 2020 2069 6620 636f 6e66           if conf
-000033e0: 6967 2e67 6574 626f 6f6c 6561 6e28 2276  ig.getboolean("v
-000033f0: 6572 6966 6965 7222 2c20 2269 676e 6f72  erifier", "ignor
-00003400: 655f 746f 6d74 6f75 5f65 7272 6f72 7322  e_tomtou_errors"
-00003410: 2c20 6661 6c6c 6261 636b 3d54 7275 6529  , fallback=True)
-00003420: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00003430: 2020 6661 696c 7572 652e 6164 645f 6576    failure.add_ev
-00003440: 656e 7428 2274 6f6d 746f 7522 2c20 2268  ent("tomtou", "h
-00003450: 6173 6820 7661 6c69 6461 7469 6f6e 2077  ash validation w
-00003460: 6173 2073 6b69 7070 6564 222c 2054 7275  as skipped", Tru
-00003470: 6529 0a20 2020 2020 2020 2020 2020 2072  e).            r
-00003480: 6574 7572 6e20 6661 696c 7572 650a 2020  eturn failure.  
-00003490: 2020 2020 2020 6966 2073 656c 662e 696d        if self.im
-000034a0: 615f 7465 6d70 6c61 7465 5f68 6173 6820  a_template_hash 
-000034b0: 213d 2073 656c 662e 5f69 6d61 5f68 6173  != self._ima_has
-000034c0: 685f 616c 672e 6861 7368 2873 656c 662e  h_alg.hash(self.
-000034d0: 5f62 7974 6573 293a 0a20 2020 2020 2020  _bytes):.       
-000034e0: 2020 2020 2066 6169 6c75 7265 2e61 6464       failure.add
-000034f0: 5f65 7665 6e74 280a 2020 2020 2020 2020  _event(.        
-00003500: 2020 2020 2020 2020 2269 6d61 5f68 6173          "ima_has
-00003510: 6822 2c0a 2020 2020 2020 2020 2020 2020  h",.            
-00003520: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-00003530: 2020 2020 2020 2020 2020 226d 6573 7361            "messa
-00003540: 6765 223a 2022 494d 4120 7465 6d70 6c61  ge": "IMA templa
-00003550: 7465 2068 6173 6820 646f 6573 206e 6f74  te hash does not
-00003560: 206d 6174 6368 2074 6865 2063 616c 6375   match the calcu
-00003570: 6c61 7465 6420 6861 7368 2e22 2c0a 2020  lated hash.",.  
-00003580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003590: 2020 2265 7870 6563 7465 6422 3a20 7374    "expected": st
-000035a0: 7228 7365 6c66 2e69 6d61 5f74 656d 706c  r(self.ima_templ
-000035b0: 6174 655f 6861 7368 292c 0a20 2020 2020  ate_hash),.     
-000035c0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000035d0: 676f 7422 3a20 7374 7228 7365 6c66 2e6d  got": str(self.m
-000035e0: 6f64 652e 6279 7465 7328 2929 2c0a 2020  ode.bytes()),.  
-000035f0: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
-00003600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003610: 2054 7275 652c 0a20 2020 2020 2020 2020   True,.         
-00003620: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00003630: 2072 6574 7572 6e20 6661 696c 7572 650a   return failure.
-00003640: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00003650: 5f76 616c 6964 6174 6f72 2069 7320 4e6f  _validator is No
-00003660: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00003670: 6661 696c 7572 652e 6164 645f 6576 656e  failure.add_even
-00003680: 7428 226e 6f5f 7661 6c69 6461 746f 7222  t("no_validator"
-00003690: 2c20 224e 6f20 7661 6c69 6461 746f 7220  , "No validator 
-000036a0: 7370 6563 6966 6965 6422 2c20 5472 7565  specified", True
-000036b0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-000036c0: 7475 726e 2066 6169 6c75 7265 0a0a 2020  turn failure..  
-000036d0: 2020 2020 2020 6661 696c 7572 652e 6d65        failure.me
-000036e0: 7267 6528 7365 6c66 2e6d 6f64 652e 6973  rge(self.mode.is
-000036f0: 5f64 6174 615f 7661 6c69 6428 7365 6c66  _data_valid(self
-00003700: 2e5f 7661 6c69 6461 746f 7229 290a 2020  ._validator)).  
-00003710: 2020 2020 2020 7265 7475 726e 2066 6169        return fai
-00003720: 6c75 7265 0a                             lure.
+00000120: 6162 630a 696d 706f 7274 2073 7472 7563  abc.import struc
+00000130: 740a 696d 706f 7274 2074 7970 696e 670a  t.import typing.
+00000140: 6672 6f6d 2074 7970 696e 6720 696d 706f  from typing impo
+00000150: 7274 2041 6e79 2c20 4361 6c6c 6162 6c65  rt Any, Callable
+00000160: 2c20 4469 6374 2c20 4f70 7469 6f6e 616c  , Dict, Optional
+00000170: 2c20 556e 696f 6e0a 0a66 726f 6d20 6b65  , Union..from ke
+00000180: 796c 696d 6520 696d 706f 7274 2063 6f6e  ylime import con
+00000190: 6669 672c 206b 6579 6c69 6d65 5f6c 6f67  fig, keylime_log
+000001a0: 6769 6e67 0a66 726f 6d20 6b65 796c 696d  ging.from keylim
+000001b0: 652e 636f 6d6d 6f6e 2e61 6c67 6f72 6974  e.common.algorit
+000001c0: 686d 7320 696d 706f 7274 2048 6173 680a  hms import Hash.
+000001d0: 6672 6f6d 206b 6579 6c69 6d65 2e66 6169  from keylime.fai
+000001e0: 6c75 7265 2069 6d70 6f72 7420 436f 6d70  lure import Comp
+000001f0: 6f6e 656e 742c 2046 6169 6c75 7265 0a0a  onent, Failure..
+00000200: 6c6f 6767 6572 203d 206b 6579 6c69 6d65  logger = keylime
+00000210: 5f6c 6f67 6769 6e67 2e69 6e69 745f 6c6f  _logging.init_lo
+00000220: 6767 696e 6728 2269 6d61 2229 0a0a 5443  gging("ima")..TC
+00000230: 475f 4556 454e 545f 4e41 4d45 5f4c 454e  G_EVENT_NAME_LEN
+00000240: 5f4d 4158 203d 2032 3535 0a53 4841 5f44  _MAX = 255.SHA_D
+00000250: 4947 4553 545f 4c45 4e20 3d20 3230 0a4d  IGEST_LEN = 20.M
+00000260: 4435 5f44 4947 4553 545f 4c45 4e20 3d20  D5_DIGEST_LEN = 
+00000270: 3136 0a0a 4e55 4c4c 5f42 5954 4520 3d20  16..NULL_BYTE = 
+00000280: 6f72 6428 225c 3022 290a 434f 4c4f 4e5f  ord("\0").COLON_
+00000290: 4259 5445 203d 206f 7264 2822 3a22 290a  BYTE = ord(":").
+000002a0: 0a0a 636c 6173 7320 5661 6c69 6461 746f  ..class Validato
+000002b0: 723a 0a20 2020 2066 756e 6374 696f 6e73  r:.    functions
+000002c0: 3a20 4469 6374 5b74 7970 696e 672e 5479  : Dict[typing.Ty
+000002d0: 7065 5b22 4d6f 6465 225d 2c20 4361 6c6c  pe["Mode"], Call
+000002e0: 6162 6c65 5b2e 2e2e 2c20 4661 696c 7572  able[..., Failur
+000002f0: 655d 5d0a 0a20 2020 2064 6566 205f 5f69  e]]..    def __i
+00000300: 6e69 745f 5f28 7365 6c66 2c20 6675 6e63  nit__(self, func
+00000310: 7469 6f6e 733a 2044 6963 745b 7479 7069  tions: Dict[typi
+00000320: 6e67 2e54 7970 655b 224d 6f64 6522 5d2c  ng.Type["Mode"],
+00000330: 2043 616c 6c61 626c 655b 2e2e 2e2c 2046   Callable[..., F
+00000340: 6169 6c75 7265 5d5d 293a 0a20 2020 2020  ailure]]):.     
+00000350: 2020 2073 656c 662e 6675 6e63 7469 6f6e     self.function
+00000360: 7320 3d20 6675 6e63 7469 6f6e 730a 0a20  s = functions.. 
+00000370: 2020 2064 6566 2067 6574 5f76 616c 6964     def get_valid
+00000380: 6174 6f72 2873 656c 662c 2063 6c61 7373  ator(self, class
+00000390: 5f74 7970 653a 2074 7970 696e 672e 5479  _type: typing.Ty
+000003a0: 7065 5b22 4d6f 6465 225d 2920 2d3e 2043  pe["Mode"]) -> C
+000003b0: 616c 6c61 626c 655b 2e2e 2e2c 2046 6169  allable[..., Fai
+000003c0: 6c75 7265 5d3a 0a20 2020 2020 2020 2076  lure]:.        v
+000003d0: 616c 6964 6174 6f72 203d 2073 656c 662e  alidator = self.
+000003e0: 6675 6e63 7469 6f6e 732e 6765 7428 636c  functions.get(cl
+000003f0: 6173 735f 7479 7065 2c20 4e6f 6e65 290a  ass_type, None).
+00000400: 2020 2020 2020 2020 6966 2076 616c 6964          if valid
+00000410: 6174 6f72 2069 7320 4e6f 6e65 3a0a 2020  ator is None:.  
+00000420: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+00000430: 2e77 6172 6e69 6e67 2822 4e6f 2076 616c  .warning("No val
+00000440: 6964 6174 6f72 2077 6173 2069 6d70 6c65  idator was imple
+00000450: 6d65 6e74 6564 2066 6f72 3a20 2573 2e20  mented for: %s. 
+00000460: 5573 696e 6720 616c 7761 7973 2066 616c  Using always fal
+00000470: 7365 2076 616c 6964 6174 6f72 2122 2c20  se validator!", 
+00000480: 636c 6173 735f 7479 7065 290a 2020 2020  class_type).    
+00000490: 2020 2020 2020 2020 6661 696c 7572 6520          failure 
+000004a0: 3d20 4661 696c 7572 6528 436f 6d70 6f6e  = Failure(Compon
+000004b0: 656e 742e 494d 412c 205b 2276 616c 6964  ent.IMA, ["valid
+000004c0: 6174 696f 6e22 5d29 0a20 2020 2020 2020  ation"]).       
+000004d0: 2020 2020 2066 6169 6c75 7265 2e61 6464       failure.add
+000004e0: 5f65 7665 6e74 280a 2020 2020 2020 2020  _event(.        
+000004f0: 2020 2020 2020 2020 226e 6f5f 7661 6c69          "no_vali
+00000500: 6461 746f 7222 2c20 6622 4e6f 2076 616c  dator", f"No val
+00000510: 6964 6174 6f72 2077 6173 2069 6d70 6c65  idator was imple
+00000520: 6d65 6e74 6564 2066 6f72 3a20 7b63 6c61  mented for: {cla
+00000530: 7373 5f74 7970 657d 202e 2055 7369 6e67  ss_type} . Using
+00000540: 2061 6c77 6179 7320 6661 6c73 6520 7661   always false va
+00000550: 6c69 6461 746f 7221 222c 2054 7275 650a  lidator!", True.
+00000560: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00000570: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00000580: 206c 616d 6264 6120 2a5f 3a20 6661 696c   lambda *_: fail
+00000590: 7572 650a 2020 2020 2020 2020 7265 7475  ure.        retu
+000005a0: 726e 2076 616c 6964 6174 6f72 0a0a 0a63  rn validator...c
+000005b0: 6c61 7373 2050 6172 7365 7245 7272 6f72  lass ParserError
+000005c0: 2854 7970 6545 7272 6f72 293a 0a20 2020  (TypeError):.   
+000005d0: 2022 2222 4973 2074 6872 6f77 6e20 7768   """Is thrown wh
+000005e0: 656e 2061 2074 7970 6520 636f 756c 6420  en a type could 
+000005f0: 6e6f 7420 6265 2063 6f6e 7374 7275 6374  not be construct
+00000600: 6564 2073 7563 6365 7373 6675 6c6c 792e  ed successfully.
+00000610: 2222 220a 0a0a 636c 6173 7320 4d6f 6465  """...class Mode
+00000620: 2861 6263 2e41 4243 293a 0a20 2020 2040  (abc.ABC):.    @
+00000630: 6162 632e 6162 7374 7261 6374 6d65 7468  abc.abstractmeth
+00000640: 6f64 0a20 2020 2064 6566 2069 735f 6461  od.    def is_da
+00000650: 7461 5f76 616c 6964 2873 656c 662c 2076  ta_valid(self, v
+00000660: 616c 6964 6174 6f72 3a20 5661 6c69 6461  alidator: Valida
+00000670: 746f 7229 202d 3e20 4661 696c 7572 653a  tor) -> Failure:
+00000680: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+00000690: 2020 2040 6162 632e 6162 7374 7261 6374     @abc.abstract
+000006a0: 6d65 7468 6f64 0a20 2020 2064 6566 2062  method.    def b
+000006b0: 7974 6573 2873 656c 6629 202d 3e20 6279  ytes(self) -> by
+000006c0: 7465 733a 0a20 2020 2020 2020 2070 6173  tes:.        pas
+000006d0: 730a 0a0a 636c 6173 7320 5479 7065 2861  s...class Type(a
+000006e0: 6263 2e41 4243 293a 0a20 2020 2040 6162  bc.ABC):.    @ab
+000006f0: 632e 6162 7374 7261 6374 6d65 7468 6f64  c.abstractmethod
+00000700: 0a20 2020 2064 6566 2073 7472 7563 7428  .    def struct(
+00000710: 7365 6c66 2920 2d3e 2062 7974 6573 3a0a  self) -> bytes:.
+00000720: 2020 2020 2020 2020 7061 7373 0a0a 0a63          pass...c
+00000730: 6c61 7373 2048 6578 4461 7461 2854 7970  lass HexData(Typ
+00000740: 6529 3a0a 2020 2020 6461 7461 3a20 6279  e):.    data: by
+00000750: 7465 730a 0a20 2020 2064 6566 205f 5f69  tes..    def __i
+00000760: 6e69 745f 5f28 7365 6c66 2c20 6461 7461  nit__(self, data
+00000770: 3a20 7374 7229 3a0a 2020 2020 2020 2020  : str):.        
+00000780: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+00000790: 2073 656c 662e 6461 7461 203d 2062 7974   self.data = byt
+000007a0: 6573 2e66 726f 6d68 6578 2864 6174 6129  es.fromhex(data)
+000007b0: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+000007c0: 5661 6c75 6545 7272 6f72 2061 7320 653a  ValueError as e:
+000007d0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+000007e0: 7365 2050 6172 7365 7245 7272 6f72 2866  se ParserError(f
+000007f0: 2250 726f 7669 6465 6420 6461 7461 2077  "Provided data w
+00000800: 6173 206e 6f74 2076 616c 6964 2068 6578  as not valid hex
+00000810: 3a20 7b64 6174 617d 2229 2066 726f 6d20  : {data}") from 
+00000820: 650a 0a20 2020 2064 6566 205f 5f73 7472  e..    def __str
+00000830: 5f5f 2873 656c 6629 202d 3e20 7374 723a  __(self) -> str:
+00000840: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00000850: 7365 6c66 2e64 6174 612e 6465 636f 6465  self.data.decode
+00000860: 2822 7574 662d 3822 290a 0a20 2020 2064  ("utf-8")..    d
+00000870: 6566 2073 7472 7563 7428 7365 6c66 2920  ef struct(self) 
+00000880: 2d3e 2062 7974 6573 3a0a 2020 2020 2020  -> bytes:.      
+00000890: 2020 7265 7475 726e 2073 7472 7563 742e    return struct.
+000008a0: 7061 636b 2866 223c 497b 6c65 6e28 7365  pack(f"<I{len(se
+000008b0: 6c66 2e64 6174 6129 7d73 222c 206c 656e  lf.data)}s", len
+000008c0: 2873 656c 662e 6461 7461 292c 2073 656c  (self.data), sel
+000008d0: 662e 6461 7461 290a 0a0a 636c 6173 7320  f.data)...class 
+000008e0: 5369 676e 6174 7572 6528 4865 7844 6174  Signature(HexDat
+000008f0: 6129 3a0a 2020 2020 2222 220a 2020 2020  a):.    """.    
+00000900: 436c 6173 7320 666f 7220 7479 7065 2022  Class for type "
+00000910: 7369 6722 2e0a 2020 2020 2222 220a 0a20  sig"..    """.. 
+00000920: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00000930: 7365 6c66 2c20 6461 7461 3a20 7374 7229  self, data: str)
+00000940: 3a0a 2020 2020 2020 2020 7375 7065 7228  :.        super(
+00000950: 292e 5f5f 696e 6974 5f5f 2864 6174 6129  ).__init__(data)
+00000960: 0a20 2020 2020 2020 2023 2062 6173 6963  .        # basic
+00000970: 2063 6865 636b 7320 6f6e 2073 6967 6e61   checks on signa
+00000980: 7475 7265 0a20 2020 2020 2020 2066 6d74  ture.        fmt
+00000990: 203d 2022 3e42 4242 4948 220a 2020 2020   = ">BBBIH".    
+000009a0: 2020 2020 6864 726c 656e 203d 2073 7472      hdrlen = str
+000009b0: 7563 742e 6361 6c63 7369 7a65 2866 6d74  uct.calcsize(fmt
+000009c0: 290a 2020 2020 2020 2020 6966 206c 656e  ).        if len
+000009d0: 2873 656c 662e 6461 7461 2920 3c20 6864  (self.data) < hd
+000009e0: 726c 656e 3a0a 2020 2020 2020 2020 2020  rlen:.          
+000009f0: 2020 7261 6973 6520 5061 7273 6572 4572    raise ParserEr
+00000a00: 726f 7228 2249 6e76 616c 6964 2073 6967  ror("Invalid sig
+00000a10: 6e61 7475 7265 3a20 6865 6164 6572 2074  nature: header t
+00000a20: 6f6f 2073 686f 7274 2229 0a20 2020 2020  oo short").     
+00000a30: 2020 205f 2c20 5f2c 205f 2c20 5f2c 2073     _, _, _, _, s
+00000a40: 6967 5f73 697a 6520 3d20 7374 7275 6374  ig_size = struct
+00000a50: 2e75 6e70 6163 6b28 666d 742c 2073 656c  .unpack(fmt, sel
+00000a60: 662e 6461 7461 5b3a 6864 726c 656e 5d29  f.data[:hdrlen])
+00000a70: 0a0a 2020 2020 2020 2020 6966 2068 6472  ..        if hdr
+00000a80: 6c65 6e20 2b20 7369 675f 7369 7a65 2021  len + sig_size !
+00000a90: 3d20 6c65 6e28 7365 6c66 2e64 6174 6129  = len(self.data)
+00000aa0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00000ab0: 6973 6520 5061 7273 6572 4572 726f 7228  ise ParserError(
+00000ac0: 2249 6e76 616c 6964 2073 6967 6e61 7475  "Invalid signatu
+00000ad0: 7265 3a20 6d61 6c66 6f72 6d65 6420 6865  re: malformed he
+00000ae0: 6164 6572 2229 0a0a 0a63 6c61 7373 2042  ader")...class B
+00000af0: 7566 6665 7228 4865 7844 6174 6129 3a0a  uffer(HexData):.
+00000b00: 2020 2020 2222 220a 2020 2020 436c 6173      """.    Clas
+00000b10: 7320 666f 7220 7479 7065 2022 6275 6622  s for type "buf"
+00000b20: 2e0a 2020 2020 2222 220a 0a0a 636c 6173  ..    """...clas
+00000b30: 7320 4e61 6d65 2854 7970 6529 3a0a 2020  s Name(Type):.  
+00000b40: 2020 2222 220a 2020 2020 436c 6173 7320    """.    Class 
+00000b50: 666f 7220 7479 7065 2022 6e22 2061 6e64  for type "n" and
+00000b60: 2022 6e2d 6e67 222e 0a20 2020 2022 2222   "n-ng"..    """
+00000b70: 0a0a 2020 2020 6e61 6d65 3a20 7374 720a  ..    name: str.
+00000b80: 2020 2020 6c65 6761 6379 3a20 626f 6f6c      legacy: bool
+00000b90: 203d 2046 616c 7365 0a0a 2020 2020 6465   = False..    de
+00000ba0: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
+00000bb0: 206e 616d 653a 2073 7472 2c20 6c65 6761   name: str, lega
+00000bc0: 6379 3a20 626f 6f6c 203d 2046 616c 7365  cy: bool = False
+00000bd0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+00000be0: 6e61 6d65 203d 206e 616d 650a 2020 2020  name = name.    
+00000bf0: 2020 2020 7365 6c66 2e6c 6567 6163 7920      self.legacy 
+00000c00: 3d20 6c65 6761 6379 0a0a 2020 2020 6465  = legacy..    de
+00000c10: 6620 5f5f 7374 725f 5f28 7365 6c66 2920  f __str__(self) 
+00000c20: 2d3e 2073 7472 3a0a 2020 2020 2020 2020  -> str:.        
+00000c30: 7265 7475 726e 2073 656c 662e 6e61 6d65  return self.name
+00000c40: 0a0a 2020 2020 6465 6620 7374 7275 6374  ..    def struct
+00000c50: 2873 656c 6629 202d 3e20 6279 7465 733a  (self) -> bytes:
+00000c60: 0a20 2020 2020 2020 206e 616d 655f 6279  .        name_by
+00000c70: 7465 7320 3d20 7365 6c66 2e6e 616d 652e  tes = self.name.
+00000c80: 656e 636f 6465 2822 7574 662d 3822 290a  encode("utf-8").
+00000c90: 0a20 2020 2020 2020 2023 2054 6865 206f  .        # The o
+00000ca0: 6c64 2022 6e22 206f 7074 696f 6e20 6973  ld "n" option is
+00000cb0: 2066 6978 6564 206c 656e 6774 682e 0a20   fixed length.. 
+00000cc0: 2020 2020 2020 2069 6620 7365 6c66 2e6c         if self.l
+00000cd0: 6567 6163 793a 0a20 2020 2020 2020 2020  egacy:.         
+00000ce0: 2020 2072 6574 7572 6e20 7374 7275 6374     return struct
+00000cf0: 2e70 6163 6b28 0a20 2020 2020 2020 2020  .pack(.         
+00000d00: 2020 2020 2020 2066 227b 6c65 6e28 6e61         f"{len(na
+00000d10: 6d65 5f62 7974 6573 297d 7342 7b54 4347  me_bytes)}sB{TCG
+00000d20: 5f45 5645 4e54 5f4e 414d 455f 4c45 4e5f  _EVENT_NAME_LEN_
+00000d30: 4d41 5820 2d20 6c65 6e28 6e61 6d65 5f62  MAX - len(name_b
+00000d40: 7974 6573 297d 7322 2c0a 2020 2020 2020  ytes)}s",.      
+00000d50: 2020 2020 2020 2020 2020 6e61 6d65 5f62            name_b
+00000d60: 7974 6573 2c0a 2020 2020 2020 2020 2020  ytes,.          
+00000d70: 2020 2020 2020 4e55 4c4c 5f42 5954 452c        NULL_BYTE,
+00000d80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000d90: 2062 7974 6561 7272 6179 2854 4347 5f45   bytearray(TCG_E
+00000da0: 5645 4e54 5f4e 414d 455f 4c45 4e5f 4d41  VENT_NAME_LEN_MA
+00000db0: 5820 2d20 6c65 6e28 6e61 6d65 5f62 7974  X - len(name_byt
+00000dc0: 6573 2929 2c0a 2020 2020 2020 2020 2020  es)),.          
+00000dd0: 2020 290a 0a20 2020 2020 2020 2072 6574    )..        ret
+00000de0: 7572 6e20 7374 7275 6374 2e70 6163 6b28  urn struct.pack(
+00000df0: 6622 3c49 7b6c 656e 286e 616d 655f 6279  f"<I{len(name_by
+00000e00: 7465 7329 7d73 4222 2c20 6c65 6e28 6e61  tes)}sB", len(na
+00000e10: 6d65 5f62 7974 6573 2920 2b20 312c 206e  me_bytes) + 1, n
+00000e20: 616d 655f 6279 7465 732c 204e 554c 4c5f  ame_bytes, NULL_
+00000e30: 4259 5445 290a 0a0a 636c 6173 7320 4469  BYTE)...class Di
+00000e40: 6765 7374 3a0a 2020 2020 2222 220a 2020  gest:.    """.  
+00000e50: 2020 436c 6173 7320 666f 7220 7479 7065    Class for type
+00000e60: 7320 2264 2220 616e 6420 2264 2d6e 6722  s "d" and "d-ng"
+00000e70: 2077 6974 6820 616e 6420 7769 7468 6f75   with and withou
+00000e80: 7420 616c 676f 7269 7468 6d0a 2020 2020  t algorithm.    
+00000e90: 2222 220a 0a20 2020 2068 6173 683a 2062  """..    hash: b
+00000ea0: 7974 6573 0a20 2020 2061 6c67 6f72 6974  ytes.    algorit
+00000eb0: 686d 3a20 7374 720a 2020 2020 6c65 6761  hm: str.    lega
+00000ec0: 6379 3a20 626f 6f6c 203d 2046 616c 7365  cy: bool = False
+00000ed0: 0a0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
+00000ee0: 5f5f 2873 656c 662c 2064 6967 6573 743a  __(self, digest:
+00000ef0: 2073 7472 2c20 6c65 6761 6379 3a20 626f   str, legacy: bo
+00000f00: 6f6c 203d 2046 616c 7365 293a 0a20 2020  ol = False):.   
+00000f10: 2020 2020 2073 656c 662e 6c65 6761 6379       self.legacy
+00000f20: 203d 206c 6567 6163 790a 2020 2020 2020   = legacy.      
+00000f30: 2020 746f 6b65 6e73 203d 2064 6967 6573    tokens = diges
+00000f40: 742e 7370 6c69 7428 223a 2229 0a20 2020  t.split(":").   
+00000f50: 2020 2020 2069 6620 6c65 6e28 746f 6b65       if len(toke
+00000f60: 6e73 2920 3d3d 2031 3a0a 2020 2020 2020  ns) == 1:.      
+00000f70: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+00000f80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00000f90: 6861 7368 203d 2062 7974 6573 2e66 726f  hash = bytes.fro
+00000fa0: 6d68 6578 2874 6f6b 656e 735b 305d 290a  mhex(tokens[0]).
+00000fb0: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+00000fc0: 7074 2056 616c 7565 4572 726f 7220 6173  pt ValueError as
+00000fd0: 2065 3a0a 2020 2020 2020 2020 2020 2020   e:.            
+00000fe0: 2020 2020 7261 6973 6520 5061 7273 6572      raise Parser
+00000ff0: 4572 726f 7228 6622 4469 6765 7374 2068  Error(f"Digest h
+00001000: 6173 6820 6973 206e 6f74 2076 616c 6964  ash is not valid
+00001010: 2068 6578 2e20 476f 743a 207b 746f 6b65   hex. Got: {toke
+00001020: 6e73 5b30 5d7d 2229 2066 726f 6d20 650a  ns[0]}") from e.
+00001030: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+00001040: 656e 2873 656c 662e 6861 7368 2920 3d3d  en(self.hash) ==
+00001050: 2053 4841 5f44 4947 4553 545f 4c45 4e3a   SHA_DIGEST_LEN:
+00001060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001070: 2073 656c 662e 616c 676f 7269 7468 6d20   self.algorithm 
+00001080: 3d20 2273 6861 3122 0a20 2020 2020 2020  = "sha1".       
+00001090: 2020 2020 2065 6c69 6620 6c65 6e28 7365       elif len(se
+000010a0: 6c66 2e68 6173 6829 203d 3d20 4d44 355f  lf.hash) == MD5_
+000010b0: 4449 4745 5354 5f4c 454e 3a0a 2020 2020  DIGEST_LEN:.    
+000010c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000010d0: 2e61 6c67 6f72 6974 686d 203d 2022 6d64  .algorithm = "md
+000010e0: 3522 0a20 2020 2020 2020 2020 2020 2065  5".            e
+000010f0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00001100: 2020 2020 2072 6169 7365 2050 6172 7365       raise Parse
+00001110: 7245 7272 6f72 280a 2020 2020 2020 2020  rError(.        
+00001120: 2020 2020 2020 2020 2020 2020 2243 616e              "Can
+00001130: 6e6f 7420 6372 6561 7465 2044 6967 6573  not create Diges
+00001140: 742e 204e 6f20 6861 7368 2061 6c67 6f72  t. No hash algor
+00001150: 6974 686d 2069 7320 7072 6f76 6964 6564  ithm is provided
+00001160: 2061 6e64 2068 6173 6820 646f 6573 206e   and hash does n
+00001170: 6f74 2062 656c 6f6e 6720 746f 2061 206d  ot belong to a m
+00001180: 6435 206f 7220 7368 6131 2068 6173 682e  d5 or sha1 hash.
+00001190: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+000011a0: 2020 290a 2020 2020 2020 2020 656c 6966    ).        elif
+000011b0: 206c 656e 2874 6f6b 656e 7329 203d 3d20   len(tokens) == 
+000011c0: 323a 0a20 2020 2020 2020 2020 2020 2074  2:.            t
+000011d0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+000011e0: 2020 2020 7365 6c66 2e68 6173 6820 3d20      self.hash = 
+000011f0: 6279 7465 732e 6672 6f6d 6865 7828 746f  bytes.fromhex(to
+00001200: 6b65 6e73 5b31 5d29 0a20 2020 2020 2020  kens[1]).       
+00001210: 2020 2020 2065 7863 6570 7420 5661 6c75       except Valu
+00001220: 6545 7272 6f72 2061 7320 653a 0a20 2020  eError as e:.   
+00001230: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+00001240: 7365 2050 6172 7365 7245 7272 6f72 2866  se ParserError(f
+00001250: 2244 6967 6573 7420 6861 7368 2069 7320  "Digest hash is 
+00001260: 6e6f 7420 7661 6c69 6420 6865 782e 2047  not valid hex. G
+00001270: 6f74 3a20 7b74 6f6b 656e 735b 315d 7d22  ot: {tokens[1]}"
+00001280: 2920 6672 6f6d 2065 0a20 2020 2020 2020  ) from e.       
+00001290: 2020 2020 2073 656c 662e 616c 676f 7269       self.algori
+000012a0: 7468 6d20 3d20 746f 6b65 6e73 5b30 5d0a  thm = tokens[0].
+000012b0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+000012c0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+000012d0: 5061 7273 6572 4572 726f 7228 6622 4361  ParserError(f"Ca
+000012e0: 6e6e 6f74 2063 7265 6174 6520 4469 6765  nnot create Dige
+000012f0: 7374 2065 7870 6563 7465 6420 3120 6f72  st expected 1 or
+00001300: 2032 2074 6f6b 656e 7320 676f 743a 207b   2 tokens got: {
+00001310: 6c65 6e28 746f 6b65 6e73 297d 2066 6f72  len(tokens)} for
+00001320: 207b 6469 6765 7374 7d22 290a 0a20 2020   {digest}")..   
+00001330: 2064 6566 2073 7472 7563 7428 7365 6c66   def struct(self
+00001340: 2920 2d3e 2062 7974 6573 3a0a 2020 2020  ) -> bytes:.    
+00001350: 2020 2020 2320 5468 6520 6c65 6761 6379      # The legacy
+00001360: 2066 6f72 6d61 7420 2264 2220 6861 7320   format "d" has 
+00001370: 6669 7865 6420 6c65 6e67 7468 2c20 736f  fixed length, so
+00001380: 2069 7420 646f 6573 206e 6f74 2063 6f6e   it does not con
+00001390: 7461 696e 2061 206c 656e 6774 6820 6174  tain a length at
+000013a0: 7472 6962 7574 650a 2020 2020 2020 2020  tribute.        
+000013b0: 6966 2073 656c 662e 6c65 6761 6379 3a0a  if self.legacy:.
+000013c0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000013d0: 726e 2073 7472 7563 742e 7061 636b 2866  rn struct.pack(f
+000013e0: 223c 7b6c 656e 2873 656c 662e 6861 7368  "<{len(self.hash
+000013f0: 297d 7322 2c20 7365 6c66 2e68 6173 6829  )}s", self.hash)
+00001400: 0a0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
+00001410: 662e 616c 676f 7269 7468 6d20 6973 204e  f.algorithm is N
+00001420: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00001430: 2072 6574 7572 6e20 7374 7275 6374 2e70   return struct.p
+00001440: 6163 6b28 6622 3c49 7b6c 656e 2873 656c  ack(f"<I{len(sel
+00001450: 662e 6861 7368 297d 7322 2c20 6c65 6e28  f.hash)}s", len(
+00001460: 7365 6c66 2e68 6173 6829 2c20 7365 6c66  self.hash), self
+00001470: 2e68 6173 6829 0a20 2020 2020 2020 2023  .hash).        #
+00001480: 2041 6674 6572 2074 6865 2027 3a27 206d   After the ':' m
+00001490: 7573 7420 6265 2061 2027 5c4f 273a 0a20  ust be a '\O':. 
+000014a0: 2020 2020 2020 2023 2068 7474 7073 3a2f         # https:/
+000014b0: 2f65 6c69 7869 722e 626f 6f74 6c69 6e2e  /elixir.bootlin.
+000014c0: 636f 6d2f 6c69 6e75 782f 7635 2e31 322e  com/linux/v5.12.
+000014d0: 3130 2f73 6f75 7263 652f 7365 6375 7269  10/source/securi
+000014e0: 7479 2f69 6e74 6567 7269 7479 2f69 6d61  ty/integrity/ima
+000014f0: 2f69 6d61 5f74 656d 706c 6174 655f 6c69  /ima_template_li
+00001500: 622e 6323 4c32 3330 0a20 2020 2020 2020  b.c#L230.       
+00001510: 2072 6574 7572 6e20 7374 7275 6374 2e70   return struct.p
+00001520: 6163 6b28 0a20 2020 2020 2020 2020 2020  ack(.           
+00001530: 2066 223c 497b 6c65 6e28 7365 6c66 2e61   f"<I{len(self.a
+00001540: 6c67 6f72 6974 686d 297d 7342 427b 6c65  lgorithm)}sBB{le
+00001550: 6e28 7365 6c66 2e68 6173 6829 7d73 222c  n(self.hash)}s",
+00001560: 0a20 2020 2020 2020 2020 2020 206c 656e  .            len
+00001570: 2873 656c 662e 616c 676f 7269 7468 6d29  (self.algorithm)
+00001580: 202b 2032 202b 206c 656e 2873 656c 662e   + 2 + len(self.
+00001590: 6861 7368 292c 0a20 2020 2020 2020 2020  hash),.         
+000015a0: 2020 2073 656c 662e 616c 676f 7269 7468     self.algorith
+000015b0: 6d2e 656e 636f 6465 2822 7574 662d 3822  m.encode("utf-8"
+000015c0: 292c 0a20 2020 2020 2020 2020 2020 2043  ),.            C
+000015d0: 4f4c 4f4e 5f42 5954 452c 0a20 2020 2020  OLON_BYTE,.     
+000015e0: 2020 2020 2020 204e 554c 4c5f 4259 5445         NULL_BYTE
+000015f0: 2c0a 2020 2020 2020 2020 2020 2020 7365  ,.            se
+00001600: 6c66 2e68 6173 682c 0a20 2020 2020 2020  lf.hash,.       
+00001610: 2029 0a0a 2020 2020 6465 6620 5f5f 6571   )..    def __eq
+00001620: 5f5f 2873 656c 662c 206f 7468 6572 3a20  __(self, other: 
+00001630: 416e 7929 202d 3e20 626f 6f6c 3a0a 2020  Any) -> bool:.  
+00001640: 2020 2020 2020 7265 7475 726e 2028 0a20        return (. 
+00001650: 2020 2020 2020 2020 2020 2069 7369 6e73             isins
+00001660: 7461 6e63 6528 6f74 6865 722c 2044 6967  tance(other, Dig
+00001670: 6573 7429 0a20 2020 2020 2020 2020 2020  est).           
+00001680: 2061 6e64 2073 656c 662e 6c65 6761 6379   and self.legacy
+00001690: 203d 3d20 6f74 6865 722e 6c65 6761 6379   == other.legacy
+000016a0: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
+000016b0: 2073 656c 662e 6861 7368 203d 3d20 6f74   self.hash == ot
+000016c0: 6865 722e 6861 7368 0a20 2020 2020 2020  her.hash.       
+000016d0: 2020 2020 2061 6e64 2073 656c 662e 616c       and self.al
+000016e0: 676f 7269 7468 6d20 3d3d 206f 7468 6572  gorithm == other
+000016f0: 2e61 6c67 6f72 6974 686d 0a20 2020 2020  .algorithm.     
+00001700: 2020 2029 0a0a 0a63 6c61 7373 2049 6d61     )...class Ima
+00001710: 284d 6f64 6529 3a0a 2020 2020 2222 220a  (Mode):.    """.
+00001720: 2020 2020 436c 6173 7320 666f 7220 2269      Class for "i
+00001730: 6d61 222e 2043 6f6e 7461 696e 7320 7468  ma". Contains th
+00001740: 6520 6469 6765 7374 2061 6e64 2061 2070  e digest and a p
+00001750: 6174 682e 0a20 2020 2022 2222 0a0a 2020  ath..    """..  
+00001760: 2020 6469 6765 7374 3a20 4469 6765 7374    digest: Digest
+00001770: 0a20 2020 2070 6174 683a 204e 616d 650a  .    path: Name.
+00001780: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00001790: 5f28 7365 6c66 2c20 6461 7461 3a20 7374  _(self, data: st
+000017a0: 7229 3a0a 2020 2020 2020 2020 746f 6b65  r):.        toke
+000017b0: 6e73 203d 2064 6174 612e 7370 6c69 7428  ns = data.split(
+000017c0: 2220 222c 206d 6178 7370 6c69 743d 3129  " ", maxsplit=1)
+000017d0: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
+000017e0: 746f 6b65 6e73 2920 213d 2032 3a0a 2020  tokens) != 2:.  
+000017f0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00001800: 5061 7273 6572 4572 726f 7228 290a 2020  ParserError().  
+00001810: 2020 2020 2020 7365 6c66 2e64 6967 6573        self.diges
+00001820: 7420 3d20 4469 6765 7374 2874 6f6b 656e  t = Digest(token
+00001830: 735b 305d 2c20 6c65 6761 6379 3d54 7275  s[0], legacy=Tru
+00001840: 6529 0a20 2020 2020 2020 2073 656c 662e  e).        self.
+00001850: 7061 7468 203d 204e 616d 6528 746f 6b65  path = Name(toke
+00001860: 6e73 5b31 5d2c 206c 6567 6163 793d 5472  ns[1], legacy=Tr
+00001870: 7565 290a 0a20 2020 2064 6566 2062 7974  ue)..    def byt
+00001880: 6573 2873 656c 6629 202d 3e20 6279 7465  es(self) -> byte
+00001890: 733a 0a20 2020 2020 2020 2072 6574 7572  s:.        retur
+000018a0: 6e20 7365 6c66 2e64 6967 6573 742e 7374  n self.digest.st
+000018b0: 7275 6374 2829 202b 2073 656c 662e 7061  ruct() + self.pa
+000018c0: 7468 2e73 7472 7563 7428 290a 0a20 2020  th.struct()..   
+000018d0: 2064 6566 2069 735f 6461 7461 5f76 616c   def is_data_val
+000018e0: 6964 2873 656c 662c 2076 616c 6964 6174  id(self, validat
+000018f0: 6f72 3a20 5661 6c69 6461 746f 7229 202d  or: Validator) -
+00001900: 3e20 4661 696c 7572 653a 0a20 2020 2020  > Failure:.     
+00001910: 2020 2072 6574 7572 6e20 7661 6c69 6461     return valida
+00001920: 746f 722e 6765 745f 7661 6c69 6461 746f  tor.get_validato
+00001930: 7228 7479 7065 2873 656c 6629 2928 7365  r(type(self))(se
+00001940: 6c66 2e64 6967 6573 742c 2073 656c 662e  lf.digest, self.
+00001950: 7061 7468 290a 0a0a 636c 6173 7320 496d  path)...class Im
+00001960: 614e 6728 4d6f 6465 293a 0a20 2020 2022  aNg(Mode):.    "
+00001970: 2222 0a20 2020 2043 6c61 7373 2066 6f72  "".    Class for
+00001980: 2022 696d 612d 6e67 222e 2043 6f6e 7461   "ima-ng". Conta
+00001990: 696e 7320 7468 6520 6469 6765 7374 2061  ins the digest a
+000019a0: 6e64 2061 2070 6174 682e 0a20 2020 2022  nd a path..    "
+000019b0: 2222 0a0a 2020 2020 6469 6765 7374 3a20  ""..    digest: 
+000019c0: 4469 6765 7374 0a20 2020 2070 6174 683a  Digest.    path:
+000019d0: 204e 616d 650a 0a20 2020 2064 6566 205f   Name..    def _
+000019e0: 5f69 6e69 745f 5f28 7365 6c66 2c20 6461  _init__(self, da
+000019f0: 7461 3a20 7374 7229 3a0a 2020 2020 2020  ta: str):.      
+00001a00: 2020 746f 6b65 6e73 203d 2064 6174 612e    tokens = data.
+00001a10: 7370 6c69 7428 2220 222c 206d 6178 7370  split(" ", maxsp
+00001a20: 6c69 743d 3129 0a20 2020 2020 2020 2069  lit=1).        i
+00001a30: 6620 6c65 6e28 746f 6b65 6e73 2920 213d  f len(tokens) !=
+00001a40: 2032 3a0a 2020 2020 2020 2020 2020 2020   2:.            
+00001a50: 7261 6973 6520 5061 7273 6572 4572 726f  raise ParserErro
+00001a60: 7228 6622 4361 6e6e 6f74 2063 7265 6174  r(f"Cannot creat
+00001a70: 6520 496d 614e 6720 6578 7065 6374 6564  e ImaNg expected
+00001a80: 2032 2074 6f6b 656e 7320 676f 743a 207b   2 tokens got: {
+00001a90: 6c65 6e28 746f 6b65 6e73 297d 2e22 290a  len(tokens)}.").
+00001aa0: 2020 2020 2020 2020 7365 6c66 2e64 6967          self.dig
+00001ab0: 6573 7420 3d20 4469 6765 7374 2874 6f6b  est = Digest(tok
+00001ac0: 656e 735b 305d 290a 2020 2020 2020 2020  ens[0]).        
+00001ad0: 7365 6c66 2e70 6174 6820 3d20 4e61 6d65  self.path = Name
+00001ae0: 2874 6f6b 656e 735b 315d 290a 0a20 2020  (tokens[1])..   
+00001af0: 2064 6566 2062 7974 6573 2873 656c 6629   def bytes(self)
+00001b00: 202d 3e20 6279 7465 733a 0a20 2020 2020   -> bytes:.     
+00001b10: 2020 2072 6574 7572 6e20 7365 6c66 2e64     return self.d
+00001b20: 6967 6573 742e 7374 7275 6374 2829 202b  igest.struct() +
+00001b30: 2073 656c 662e 7061 7468 2e73 7472 7563   self.path.struc
+00001b40: 7428 290a 0a20 2020 2064 6566 2069 735f  t()..    def is_
+00001b50: 6461 7461 5f76 616c 6964 2873 656c 662c  data_valid(self,
+00001b60: 2076 616c 6964 6174 6f72 3a20 5661 6c69   validator: Vali
+00001b70: 6461 746f 7229 202d 3e20 4661 696c 7572  dator) -> Failur
+00001b80: 653a 0a20 2020 2020 2020 2072 6574 7572  e:.        retur
+00001b90: 6e20 7661 6c69 6461 746f 722e 6765 745f  n validator.get_
+00001ba0: 7661 6c69 6461 746f 7228 7479 7065 2873  validator(type(s
+00001bb0: 656c 6629 2928 7365 6c66 2e64 6967 6573  elf))(self.diges
+00001bc0: 742c 2073 656c 662e 7061 7468 290a 0a0a  t, self.path)...
+00001bd0: 636c 6173 7320 496d 6153 6967 284d 6f64  class ImaSig(Mod
+00001be0: 6529 3a0a 2020 2020 2222 220a 2020 2020  e):.    """.    
+00001bf0: 436c 6173 7320 666f 7220 2269 6d61 2d73  Class for "ima-s
+00001c00: 6967 2220 7465 6d70 6c61 7465 2e20 4e65  ig" template. Ne
+00001c10: 6172 6c79 2074 6865 2073 616d 6520 6173  arly the same as
+00001c20: 2049 6d61 4e67 2062 7574 2063 616e 2063   ImaNg but can c
+00001c30: 6f6e 7461 696e 2061 206f 7074 696f 6e61  ontain a optiona
+00001c40: 6c20 7369 676e 6174 7572 652e 0a20 2020  l signature..   
+00001c50: 2022 2222 0a0a 2020 2020 6469 6765 7374   """..    digest
+00001c60: 3a20 4469 6765 7374 0a20 2020 2070 6174  : Digest.    pat
+00001c70: 683a 204e 616d 650a 2020 2020 7369 676e  h: Name.    sign
+00001c80: 6174 7572 653a 204f 7074 696f 6e61 6c5b  ature: Optional[
+00001c90: 5369 676e 6174 7572 655d 203d 204e 6f6e  Signature] = Non
+00001ca0: 650a 0a20 2020 2064 6566 205f 5f69 6e69  e..    def __ini
+00001cb0: 745f 5f28 7365 6c66 2c20 6461 7461 3a20  t__(self, data: 
+00001cc0: 7374 7229 3a0a 2020 2020 2020 2020 2320  str):.        # 
+00001cd0: 5468 6572 6520 6172 6520 616c 7761 7973  There are always
+00001ce0: 2033 2066 6965 6c64 7320 696e 2061 2076   3 fields in a v
+00001cf0: 616c 6964 2065 6e74 7279 2c20 6265 6361  alid entry, beca
+00001d00: 7573 653a 0a20 2020 2020 2020 2023 0a20  use:.        #. 
+00001d10: 2020 2020 2020 2023 202d 206e 2d6e 6720         # - n-ng 
+00001d20: 646f 6573 206e 6f74 2063 6f6e 7461 696e  does not contain
+00001d30: 2061 2073 7061 6365 2063 6861 7261 6374   a space charact
+00001d40: 6572 2c20 6173 2069 7420 6973 2065 7363  er, as it is esc
+00001d50: 6170 6564 2074 6f20 616e 0a20 2020 2020  aped to an.     
+00001d60: 2020 2023 2020 2075 6e64 6572 7363 6f72     #   underscor
+00001d70: 6520 2822 5f22 293a 0a20 2020 2020 2020  e ("_"):.       
+00001d80: 2023 2020 2068 7474 7073 3a2f 2f65 6c69   #   https://eli
+00001d90: 7869 722e 626f 6f74 6c69 6e2e 636f 6d2f  xir.bootlin.com/
+00001da0: 6c69 6e75 782f 7635 2e31 382f 736f 7572  linux/v5.18/sour
+00001db0: 6365 2f73 6563 7572 6974 792f 696e 7465  ce/security/inte
+00001dc0: 6772 6974 792f 696d 612f 696d 615f 7465  grity/ima/ima_te
+00001dd0: 6d70 6c61 7465 5f6c 6962 2e63 234c 3535  mplate_lib.c#L55
+00001de0: 0a20 2020 2020 2020 2023 202d 2074 6865  .        # - the
+00001df0: 206c 6173 7420 6669 656c 6420 636f 756c   last field coul
+00001e00: 6420 6265 2061 6e20 656d 7074 7920 7374  d be an empty st
+00001e10: 7269 6e67 2062 7574 2061 2064 656c 696d  ring but a delim
+00001e20: 6974 6572 2028 2220 2229 2073 686f 756c  iter (" ") shoul
+00001e30: 640a 2020 2020 2020 2020 2320 2020 7374  d.        #   st
+00001e40: 696c 6c20 7072 6573 656e 743a 0a20 2020  ill present:.   
+00001e50: 2020 2020 2023 2020 2068 7474 7073 3a2f       #   https:/
+00001e60: 2f65 6c69 7869 722e 626f 6f74 6c69 6e2e  /elixir.bootlin.
+00001e70: 636f 6d2f 6c69 6e75 782f 7635 2e31 382f  com/linux/v5.18/
+00001e80: 736f 7572 6365 2f73 6563 7572 6974 792f  source/security/
+00001e90: 696e 7465 6772 6974 792f 696d 612f 696d  integrity/ima/im
+00001ea0: 615f 6673 2e63 234c 3234 340a 2020 2020  a_fs.c#L244.    
+00001eb0: 2020 2020 746f 6b65 6e73 203d 2064 6174      tokens = dat
+00001ec0: 612e 7370 6c69 7428 2220 222c 206d 6178  a.split(" ", max
+00001ed0: 7370 6c69 743d 3229 0a20 2020 2020 2020  split=2).       
+00001ee0: 2069 6620 6c65 6e28 746f 6b65 6e73 2920   if len(tokens) 
+00001ef0: 213d 2033 3a0a 2020 2020 2020 2020 2020  != 3:.          
+00001f00: 2020 7261 6973 6520 5061 7273 6572 4572    raise ParserEr
+00001f10: 726f 7228 6622 4361 6e6e 6f74 2063 7265  ror(f"Cannot cre
+00001f20: 6174 6520 496d 6153 6967 2065 7870 6563  ate ImaSig expec
+00001f30: 7465 6420 3320 746f 6b65 6e73 2067 6f74  ted 3 tokens got
+00001f40: 3a20 7b6c 656e 2874 6f6b 656e 7329 7d2e  : {len(tokens)}.
+00001f50: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+00001f60: 6469 6765 7374 203d 2044 6967 6573 7428  digest = Digest(
+00001f70: 746f 6b65 6e73 5b30 5d29 0a20 2020 2020  tokens[0]).     
+00001f80: 2020 2073 656c 662e 7061 7468 203d 204e     self.path = N
+00001f90: 616d 6528 746f 6b65 6e73 5b31 5d29 0a20  ame(tokens[1]). 
+00001fa0: 2020 2020 2020 2073 656c 662e 7369 676e         self.sign
+00001fb0: 6174 7572 6520 3d20 7365 6c66 2e63 7265  ature = self.cre
+00001fc0: 6174 655f 7369 676e 6174 7572 6528 746f  ate_signature(to
+00001fd0: 6b65 6e73 5b32 5d29 0a0a 2020 2020 4073  kens[2])..    @s
+00001fe0: 7461 7469 636d 6574 686f 640a 2020 2020  taticmethod.    
+00001ff0: 6465 6620 6372 6561 7465 5f73 6967 6e61  def create_signa
+00002000: 7475 7265 2868 6578 7374 7269 6e67 3a20  ture(hexstring: 
+00002010: 7374 7229 202d 3e20 4f70 7469 6f6e 616c  str) -> Optional
+00002020: 5b53 6967 6e61 7475 7265 5d3a 0a20 2020  [Signature]:.   
+00002030: 2020 2020 2022 2222 4372 6561 7465 2074       """Create t
+00002040: 6865 2053 6967 6e61 7475 7265 206f 626a  he Signature obj
+00002050: 6563 7420 6966 2074 6865 2068 6578 7374  ect if the hexst
+00002060: 7269 6e67 2069 7320 6120 7661 6c69 6420  ring is a valid 
+00002070: 7369 676e 6174 7572 6522 2222 0a20 2020  signature""".   
+00002080: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+00002090: 2020 2020 2020 7265 7475 726e 2053 6967        return Sig
+000020a0: 6e61 7475 7265 2868 6578 7374 7269 6e67  nature(hexstring
+000020b0: 290a 2020 2020 2020 2020 6578 6365 7074  ).        except
+000020c0: 2050 6172 7365 7245 7272 6f72 3a0a 2020   ParserError:.  
+000020d0: 2020 2020 2020 2020 2020 7061 7373 0a20            pass. 
+000020e0: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+000020f0: 6e65 0a0a 2020 2020 6465 6620 6279 7465  ne..    def byte
+00002100: 7328 7365 6c66 2920 2d3e 2062 7974 6573  s(self) -> bytes
+00002110: 3a0a 2020 2020 2020 2020 6f75 7470 7574  :.        output
+00002120: 203d 2073 656c 662e 6469 6765 7374 2e73   = self.digest.s
+00002130: 7472 7563 7428 2920 2b20 7365 6c66 2e70  truct() + self.p
+00002140: 6174 682e 7374 7275 6374 2829 0a20 2020  ath.struct().   
+00002150: 2020 2020 2023 2049 6620 6e6f 2073 6967       # If no sig
+00002160: 6e61 7475 7265 2069 7320 7468 6572 6520  nature is there 
+00002170: 7765 2073 696c 6c20 6861 7665 2074 6f20  we sill have to 
+00002180: 6164 6420 7468 6520 656e 7472 7920 666f  add the entry fo
+00002190: 7220 6974 0a20 2020 2020 2020 2069 6620  r it.        if 
+000021a0: 7365 6c66 2e73 6967 6e61 7475 7265 2069  self.signature i
+000021b0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+000021c0: 2020 2020 6f75 7470 7574 202b 3d20 7374      output += st
+000021d0: 7275 6374 2e70 6163 6b28 223c 4930 7322  ruct.pack("<I0s"
+000021e0: 2c20 302c 2062 2222 290a 2020 2020 2020  , 0, b"").      
+000021f0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00002200: 2020 2020 6f75 7470 7574 202b 3d20 7365      output += se
+00002210: 6c66 2e73 6967 6e61 7475 7265 2e73 7472  lf.signature.str
+00002220: 7563 7428 290a 2020 2020 2020 2020 7265  uct().        re
+00002230: 7475 726e 206f 7574 7075 740a 0a20 2020  turn output..   
+00002240: 2064 6566 2069 735f 6461 7461 5f76 616c   def is_data_val
+00002250: 6964 2873 656c 662c 2076 616c 6964 6174  id(self, validat
+00002260: 6f72 3a20 5661 6c69 6461 746f 7229 202d  or: Validator) -
+00002270: 3e20 4661 696c 7572 653a 0a20 2020 2020  > Failure:.     
+00002280: 2020 2072 6574 7572 6e20 7661 6c69 6461     return valida
+00002290: 746f 722e 6765 745f 7661 6c69 6461 746f  tor.get_validato
+000022a0: 7228 7479 7065 2873 656c 6629 2928 7365  r(type(self))(se
+000022b0: 6c66 2e64 6967 6573 742c 2073 656c 662e  lf.digest, self.
+000022c0: 7061 7468 2c20 7365 6c66 2e73 6967 6e61  path, self.signa
+000022d0: 7475 7265 290a 0a0a 636c 6173 7320 496d  ture)...class Im
+000022e0: 6142 7566 284d 6f64 6529 3a0a 2020 2020  aBuf(Mode):.    
+000022f0: 2222 220a 2020 2020 436c 6173 7320 666f  """.    Class fo
+00002300: 7220 2269 6d61 2d62 7566 222e 2043 6f6e  r "ima-buf". Con
+00002310: 7461 696e 7320 6120 6469 6765 7374 2c20  tains a digest, 
+00002320: 6275 6666 6572 206e 616d 6520 616e 6420  buffer name and 
+00002330: 7468 6520 6275 6666 6572 2069 7473 656c  the buffer itsel
+00002340: 662e 0a20 2020 2046 6f72 2076 616c 6964  f..    For valid
+00002350: 6174 696f 6e20 7468 6520 6275 6666 6572  ation the buffer
+00002360: 206d 7573 7420 6265 2064 6f6e 6520 6261   must be done ba
+00002370: 7365 6420 6f6e 2074 6865 206e 616d 6520  sed on the name 
+00002380: 6265 6361 7573 6520 494d 4120 6f6e 6c79  because IMA only
+00002390: 2070 726f 7669 6465 7320 6974 2061 7320   provides it as 
+000023a0: 616e 2062 7974 6520 6172 7261 792e 0a20  an byte array.. 
+000023b0: 2020 2022 2222 0a0a 2020 2020 6469 6765     """..    dige
+000023c0: 7374 3a20 4469 6765 7374 0a20 2020 206e  st: Digest.    n
+000023d0: 616d 653a 204e 616d 650a 2020 2020 6461  ame: Name.    da
+000023e0: 7461 3a20 4275 6666 6572 0a0a 2020 2020  ta: Buffer..    
+000023f0: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+00002400: 662c 2064 6174 613a 2073 7472 293a 0a20  f, data: str):. 
+00002410: 2020 2020 2020 2023 2054 6865 7265 2061         # There a
+00002420: 7265 2061 6c77 6179 7320 3320 6669 656c  re always 3 fiel
+00002430: 6473 2069 6e20 6120 7661 6c69 6420 656e  ds in a valid en
+00002440: 7472 792c 2062 6563 6175 7365 3a0a 2020  try, because:.  
+00002450: 2020 2020 2020 230a 2020 2020 2020 2020        #.        
+00002460: 2320 2d20 6e2d 6e67 2064 6f65 7320 6e6f  # - n-ng does no
+00002470: 7420 636f 6e74 6169 6e20 6120 7370 6163  t contain a spac
+00002480: 6520 6368 6172 6163 7465 722c 2061 7320  e character, as 
+00002490: 6974 2069 7320 6573 6361 7065 6420 746f  it is escaped to
+000024a0: 2061 6e0a 2020 2020 2020 2020 2320 2020   an.        #   
+000024b0: 756e 6465 7273 636f 7265 2028 225f 2229  underscore ("_")
+000024c0: 3a0a 2020 2020 2020 2020 2320 2020 6874  :.        #   ht
+000024d0: 7470 733a 2f2f 656c 6978 6972 2e62 6f6f  tps://elixir.boo
+000024e0: 746c 696e 2e63 6f6d 2f6c 696e 7578 2f76  tlin.com/linux/v
+000024f0: 352e 3138 2f73 6f75 7263 652f 7365 6375  5.18/source/secu
+00002500: 7269 7479 2f69 6e74 6567 7269 7479 2f69  rity/integrity/i
+00002510: 6d61 2f69 6d61 5f74 656d 706c 6174 655f  ma/ima_template_
+00002520: 6c69 622e 6323 4c35 350a 2020 2020 2020  lib.c#L55.      
+00002530: 2020 2320 2d20 7468 6520 6c61 7374 2066    # - the last f
+00002540: 6965 6c64 2063 6f75 6c64 2062 6520 616e  ield could be an
+00002550: 2065 6d70 7479 2073 7472 696e 6720 6275   empty string bu
+00002560: 7420 6120 6465 6c69 6d69 7465 7220 2822  t a delimiter ("
+00002570: 2022 2920 7368 6f75 6c64 0a20 2020 2020   ") should.     
+00002580: 2020 2023 2020 2073 7469 6c6c 2070 7265     #   still pre
+00002590: 7365 6e74 3a0a 2020 2020 2020 2020 2320  sent:.        # 
+000025a0: 2020 6874 7470 733a 2f2f 656c 6978 6972    https://elixir
+000025b0: 2e62 6f6f 746c 696e 2e63 6f6d 2f6c 696e  .bootlin.com/lin
+000025c0: 7578 2f76 352e 3138 2f73 6f75 7263 652f  ux/v5.18/source/
+000025d0: 7365 6375 7269 7479 2f69 6e74 6567 7269  security/integri
+000025e0: 7479 2f69 6d61 2f69 6d61 5f66 732e 6323  ty/ima/ima_fs.c#
+000025f0: 4c32 3434 0a20 2020 2020 2020 2074 6f6b  L244.        tok
+00002600: 656e 7320 3d20 6461 7461 2e73 706c 6974  ens = data.split
+00002610: 2822 2022 2c20 6d61 7873 706c 6974 3d32  (" ", maxsplit=2
+00002620: 290a 2020 2020 2020 2020 6966 206c 656e  ).        if len
+00002630: 2874 6f6b 656e 7329 2021 3d20 333a 0a20  (tokens) != 3:. 
+00002640: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00002650: 2050 6172 7365 7245 7272 6f72 2866 2243   ParserError(f"C
+00002660: 616e 6e6f 7420 6372 6561 7465 2049 6d61  annot create Ima
+00002670: 4275 6620 6578 7065 6374 6564 2033 2074  Buf expected 3 t
+00002680: 6f6b 656e 7320 676f 743a 207b 6c65 6e28  okens got: {len(
+00002690: 746f 6b65 6e73 297d 2e22 290a 2020 2020  tokens)}.").    
+000026a0: 2020 2020 7365 6c66 2e64 6967 6573 7420      self.digest 
+000026b0: 3d20 4469 6765 7374 2874 6f6b 656e 735b  = Digest(tokens[
+000026c0: 305d 290a 2020 2020 2020 2020 7365 6c66  0]).        self
+000026d0: 2e6e 616d 6520 3d20 4e61 6d65 2874 6f6b  .name = Name(tok
+000026e0: 656e 735b 315d 290a 2020 2020 2020 2020  ens[1]).        
+000026f0: 7365 6c66 2e64 6174 6120 3d20 4275 6666  self.data = Buff
+00002700: 6572 2874 6f6b 656e 735b 325d 290a 0a20  er(tokens[2]).. 
+00002710: 2020 2064 6566 2062 7974 6573 2873 656c     def bytes(sel
+00002720: 6629 202d 3e20 6279 7465 733a 0a20 2020  f) -> bytes:.   
+00002730: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00002740: 2e64 6967 6573 742e 7374 7275 6374 2829  .digest.struct()
+00002750: 202b 2073 656c 662e 6e61 6d65 2e73 7472   + self.name.str
+00002760: 7563 7428 2920 2b20 7365 6c66 2e64 6174  uct() + self.dat
+00002770: 612e 7374 7275 6374 2829 0a0a 2020 2020  a.struct()..    
+00002780: 6465 6620 6973 5f64 6174 615f 7661 6c69  def is_data_vali
+00002790: 6428 7365 6c66 2c20 7661 6c69 6461 746f  d(self, validato
+000027a0: 723a 2056 616c 6964 6174 6f72 2920 2d3e  r: Validator) ->
+000027b0: 2046 6169 6c75 7265 3a0a 2020 2020 2020   Failure:.      
+000027c0: 2020 7265 7475 726e 2076 616c 6964 6174    return validat
+000027d0: 6f72 2e67 6574 5f76 616c 6964 6174 6f72  or.get_validator
+000027e0: 2874 7970 6528 7365 6c66 2929 2873 656c  (type(self))(sel
+000027f0: 662e 6469 6765 7374 2c20 7365 6c66 2e6e  f.digest, self.n
+00002800: 616d 652c 2073 656c 662e 6461 7461 290a  ame, self.data).
+00002810: 0a0a 636c 6173 7320 456e 7472 793a 0a20  ..class Entry:. 
+00002820: 2020 2022 2222 0a20 2020 2049 4d41 2045     """.    IMA E
+00002830: 6e74 7279 2e20 436f 6e74 6169 6e73 2074  ntry. Contains t
+00002840: 6865 2050 4352 2c20 7465 6d70 6c61 7465  he PCR, template
+00002850: 2068 6173 6820 616e 6420 6d6f 6465 2e0a   hash and mode..
+00002860: 2020 2020 2222 220a 0a20 2020 2070 6372      """..    pcr
+00002870: 3a20 7374 720a 2020 2020 696d 615f 7465  : str.    ima_te
+00002880: 6d70 6c61 7465 5f68 6173 683a 2062 7974  mplate_hash: byt
+00002890: 6573 0a20 2020 2070 6372 5f74 656d 706c  es.    pcr_templ
+000028a0: 6174 655f 6861 7368 3a20 6279 7465 730a  ate_hash: bytes.
+000028b0: 2020 2020 6d6f 6465 3a20 4d6f 6465 0a20      mode: Mode. 
+000028c0: 2020 205f 6279 7465 733a 2062 7974 6573     _bytes: bytes
+000028d0: 0a20 2020 205f 7661 6c69 6461 746f 723a  .    _validator:
+000028e0: 204f 7074 696f 6e61 6c5b 5661 6c69 6461   Optional[Valida
+000028f0: 746f 725d 0a20 2020 205f 696d 615f 6861  tor].    _ima_ha
+00002900: 7368 5f61 6c67 3a20 4861 7368 0a20 2020  sh_alg: Hash.   
+00002910: 205f 7063 725f 6861 7368 5f61 6c67 3a20   _pcr_hash_alg: 
+00002920: 4861 7368 0a0a 2020 2020 5f6d 6f64 655f  Hash..    _mode_
+00002930: 6c6f 6f6b 7570 3a20 4469 6374 5b73 7472  lookup: Dict[str
+00002940: 2c20 556e 696f 6e5b 7479 7069 6e67 2e54  , Union[typing.T
+00002950: 7970 655b 496d 615d 2c20 7479 7069 6e67  ype[Ima], typing
+00002960: 2e54 7970 655b 496d 614e 675d 2c20 7479  .Type[ImaNg], ty
+00002970: 7069 6e67 2e54 7970 655b 496d 6153 6967  ping.Type[ImaSig
+00002980: 5d2c 2074 7970 696e 672e 5479 7065 5b49  ], typing.Type[I
+00002990: 6d61 4275 665d 5d5d 203d 207b 0a20 2020  maBuf]]] = {.   
+000029a0: 2020 2020 2022 696d 6122 3a20 496d 612c       "ima": Ima,
+000029b0: 0a20 2020 2020 2020 2022 696d 612d 6e67  .        "ima-ng
+000029c0: 223a 2049 6d61 4e67 2c0a 2020 2020 2020  ": ImaNg,.      
+000029d0: 2020 2269 6d61 2d73 6967 223a 2049 6d61    "ima-sig": Ima
+000029e0: 5369 672c 0a20 2020 2020 2020 2022 696d  Sig,.        "im
+000029f0: 612d 6275 6622 3a20 496d 6142 7566 2c0a  a-buf": ImaBuf,.
+00002a00: 2020 2020 7d0a 0a20 2020 2064 6566 205f      }..    def _
+00002a10: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+00002a20: 2073 656c 662c 0a20 2020 2020 2020 2064   self,.        d
+00002a30: 6174 613a 2073 7472 2c0a 2020 2020 2020  ata: str,.      
+00002a40: 2020 7661 6c69 6461 746f 723a 204f 7074    validator: Opt
+00002a50: 696f 6e61 6c5b 5661 6c69 6461 746f 725d  ional[Validator]
+00002a60: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00002a70: 2069 6d61 5f68 6173 685f 616c 673a 2048   ima_hash_alg: H
+00002a80: 6173 6820 3d20 4861 7368 2e53 4841 312c  ash = Hash.SHA1,
+00002a90: 0a20 2020 2020 2020 2070 6372 5f68 6173  .        pcr_has
+00002aa0: 685f 616c 673a 2048 6173 6820 3d20 4861  h_alg: Hash = Ha
+00002ab0: 7368 2e53 4841 312c 0a20 2020 2029 3a0a  sh.SHA1,.    ):.
+00002ac0: 2020 2020 2020 2020 7365 6c66 2e5f 7661          self._va
+00002ad0: 6c69 6461 746f 7220 3d20 7661 6c69 6461  lidator = valida
+00002ae0: 746f 720a 2020 2020 2020 2020 7365 6c66  tor.        self
+00002af0: 2e5f 696d 615f 6861 7368 5f61 6c67 203d  ._ima_hash_alg =
+00002b00: 2069 6d61 5f68 6173 685f 616c 670a 2020   ima_hash_alg.  
+00002b10: 2020 2020 2020 7365 6c66 2e5f 7063 725f        self._pcr_
+00002b20: 6861 7368 5f61 6c67 203d 2070 6372 5f68  hash_alg = pcr_h
+00002b30: 6173 685f 616c 670a 2020 2020 2020 2020  ash_alg.        
+00002b40: 746f 6b65 6e73 203d 2064 6174 612e 7370  tokens = data.sp
+00002b50: 6c69 7428 2220 222c 206d 6178 7370 6c69  lit(" ", maxspli
+00002b60: 743d 3329 0a20 2020 2020 2020 2069 6620  t=3).        if 
+00002b70: 6c65 6e28 746f 6b65 6e73 2920 213d 2034  len(tokens) != 4
+00002b80: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00002b90: 6973 6520 5061 7273 6572 4572 726f 7228  ise ParserError(
+00002ba0: 6622 4361 6e6e 6f74 2063 7265 6174 6520  f"Cannot create 
+00002bb0: 456e 7472 7920 6578 7065 6374 6564 2034  Entry expected 4
+00002bc0: 2074 6f6b 656e 7320 676f 743a 207b 6c65   tokens got: {le
+00002bd0: 6e28 746f 6b65 6e73 297d 2e22 290a 2020  n(tokens)}.").  
+00002be0: 2020 2020 2020 7365 6c66 2e70 6372 203d        self.pcr =
+00002bf0: 2074 6f6b 656e 735b 305d 0a20 2020 2020   tokens[0].     
+00002c00: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+00002c10: 2020 2020 7365 6c66 2e69 6d61 5f74 656d      self.ima_tem
+00002c20: 706c 6174 655f 6861 7368 203d 2062 7974  plate_hash = byt
+00002c30: 6573 2e66 726f 6d68 6578 2874 6f6b 656e  es.fromhex(token
+00002c40: 735b 315d 290a 2020 2020 2020 2020 6578  s[1]).        ex
+00002c50: 6365 7074 2056 616c 7565 4572 726f 7220  cept ValueError 
+00002c60: 6173 2065 3a0a 2020 2020 2020 2020 2020  as e:.          
+00002c70: 2020 7261 6973 6520 5061 7273 6572 4572    raise ParserEr
+00002c80: 726f 7228 6622 4361 6e6e 6f74 2063 7265  ror(f"Cannot cre
+00002c90: 6174 6520 456e 7472 7920 6578 7065 6374  ate Entry expect
+00002ca0: 6564 2034 2074 6f6b 656e 7320 676f 743a  ed 4 tokens got:
+00002cb0: 207b 6c65 6e28 746f 6b65 6e73 297d 2e22   {len(tokens)}."
+00002cc0: 2920 6672 6f6d 2065 0a0a 2020 2020 2020  ) from e..      
+00002cd0: 2020 6d6f 6465 203d 2073 656c 662e 5f6d    mode = self._m
+00002ce0: 6f64 655f 6c6f 6f6b 7570 2e67 6574 2874  ode_lookup.get(t
+00002cf0: 6f6b 656e 735b 325d 2c20 4e6f 6e65 290a  okens[2], None).
+00002d00: 2020 2020 2020 2020 6966 206d 6f64 6520          if mode 
+00002d10: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00002d20: 2020 2020 2072 6169 7365 2050 6172 7365       raise Parse
+00002d30: 7245 7272 6f72 2866 224e 6f20 7061 7273  rError(f"No pars
+00002d40: 6572 2066 6f72 206d 6f64 6520 7b74 6f6b  er for mode {tok
+00002d50: 656e 735b 325d 7d20 696d 706c 656d 656e  ens[2]} implemen
+00002d60: 7465 642e 2229 0a20 2020 2020 2020 2073  ted.").        s
+00002d70: 656c 662e 6d6f 6465 203d 206d 6f64 6528  elf.mode = mode(
+00002d80: 746f 6b65 6e73 5b33 5d29 0a20 2020 2020  tokens[3]).     
+00002d90: 2020 2073 656c 662e 5f62 7974 6573 203d     self._bytes =
+00002da0: 2073 656c 662e 6d6f 6465 2e62 7974 6573   self.mode.bytes
+00002db0: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+00002dc0: 7063 725f 7465 6d70 6c61 7465 5f68 6173  pcr_template_has
+00002dd0: 6820 3d20 7365 6c66 2e5f 7063 725f 6861  h = self._pcr_ha
+00002de0: 7368 5f61 6c67 2e68 6173 6828 7365 6c66  sh_alg.hash(self
+00002df0: 2e5f 6279 7465 7329 0a20 2020 2020 2020  ._bytes).       
+00002e00: 2023 2053 6574 2063 6f72 7265 6374 2068   # Set correct h
+00002e10: 6173 6820 666f 7220 7469 6d65 206f 6620  ash for time of 
+00002e20: 6d65 6173 7572 652c 2074 696d 6520 6f66  measure, time of
+00002e30: 2075 7365 2028 546f 4d54 6f55 2920 6572   use (ToMToU) er
+00002e40: 726f 7273 0a20 2020 2020 2020 2023 2061  rors.        # a
+00002e50: 6e64 2069 6620 6120 6669 6c65 2069 7320  nd if a file is 
+00002e60: 616c 7265 6164 7920 6f70 656e 6564 2066  already opened f
+00002e70: 6f72 2077 7269 7465 2e0a 2020 2020 2020  or write..      
+00002e80: 2020 2320 6874 7470 733a 2f2f 656c 6978    # https://elix
+00002e90: 6972 2e62 6f6f 746c 696e 2e63 6f6d 2f6c  ir.bootlin.com/l
+00002ea0: 696e 7578 2f76 352e 3132 2e31 322f 736f  inux/v5.12.12/so
+00002eb0: 7572 6365 2f73 6563 7572 6974 792f 696e  urce/security/in
+00002ec0: 7465 6772 6974 792f 696d 612f 696d 615f  tegrity/ima/ima_
+00002ed0: 6d61 696e 2e63 234c 3130 310a 2020 2020  main.c#L101.    
+00002ee0: 2020 2020 6966 2073 656c 662e 696d 615f      if self.ima_
+00002ef0: 7465 6d70 6c61 7465 5f68 6173 6820 3d3d  template_hash ==
+00002f00: 2069 6d61 5f68 6173 685f 616c 672e 6765   ima_hash_alg.ge
+00002f10: 745f 7374 6172 745f 6861 7368 2829 3a0a  t_start_hash():.
+00002f20: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00002f30: 2e69 6d61 5f74 656d 706c 6174 655f 6861  .ima_template_ha
+00002f40: 7368 203d 2069 6d61 5f68 6173 685f 616c  sh = ima_hash_al
+00002f50: 672e 6765 745f 6666 5f68 6173 6828 290a  g.get_ff_hash().
+00002f60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00002f70: 2e70 6372 5f74 656d 706c 6174 655f 6861  .pcr_template_ha
+00002f80: 7368 203d 2070 6372 5f68 6173 685f 616c  sh = pcr_hash_al
+00002f90: 672e 6765 745f 6666 5f68 6173 6828 290a  g.get_ff_hash().
+00002fa0: 0a20 2020 2064 6566 2069 6e76 616c 6964  .    def invalid
+00002fb0: 2873 656c 6629 202d 3e20 4661 696c 7572  (self) -> Failur
+00002fc0: 653a 0a20 2020 2020 2020 2066 6169 6c75  e:.        failu
+00002fd0: 7265 203d 2046 6169 6c75 7265 2843 6f6d  re = Failure(Com
+00002fe0: 706f 6e65 6e74 2e49 4d41 2c20 5b22 7661  ponent.IMA, ["va
+00002ff0: 6c69 6461 7469 6f6e 225d 290a 2020 2020  lidation"]).    
+00003000: 2020 2020 6966 2073 656c 662e 7063 7220      if self.pcr 
+00003010: 213d 2073 7472 2863 6f6e 6669 672e 494d  != str(config.IM
+00003020: 415f 5043 5229 3a0a 2020 2020 2020 2020  A_PCR):.        
+00003030: 2020 2020 6c6f 6767 6572 2e77 6172 6e69      logger.warni
+00003040: 6e67 2822 494d 4120 656e 7472 7920 5043  ng("IMA entry PC
+00003050: 5220 646f 6573 206e 6f74 206d 6174 6368  R does not match
+00003060: 2025 732e 2049 7420 7761 733a 2025 7322   %s. It was: %s"
+00003070: 2c20 636f 6e66 6967 2e49 4d41 5f50 4352  , config.IMA_PCR
+00003080: 2c20 7365 6c66 2e70 6372 290a 2020 2020  , self.pcr).    
+00003090: 2020 2020 2020 2020 6661 696c 7572 652e          failure.
+000030a0: 6164 645f 6576 656e 7428 0a20 2020 2020  add_event(.     
+000030b0: 2020 2020 2020 2020 2020 2022 696d 615f             "ima_
+000030c0: 7063 7222 2c0a 2020 2020 2020 2020 2020  pcr",.          
+000030d0: 2020 2020 2020 7b22 6d65 7373 6167 6522        {"message"
+000030e0: 3a20 2249 4d41 2050 4352 2069 7320 6e6f  : "IMA PCR is no
+000030f0: 7420 7468 6520 636f 6e66 6967 7572 6564  t the configured
+00003100: 206f 6e65 222c 2022 6578 7065 6374 6564   one", "expected
+00003110: 223a 2073 7472 2863 6f6e 6669 672e 494d  ": str(config.IM
+00003120: 415f 5043 5229 2c20 2267 6f74 223a 2073  A_PCR), "got": s
+00003130: 656c 662e 7063 727d 2c0a 2020 2020 2020  elf.pcr},.      
+00003140: 2020 2020 2020 2020 2020 5472 7565 2c0a            True,.
+00003150: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+00003160: 2020 2020 2020 2023 2049 676e 6f72 6520         # Ignore 
+00003170: 7465 6d70 6c61 7465 2068 6173 6820 666f  template hash fo
+00003180: 7220 546f 4d54 6f55 2065 7272 6f72 730a  r ToMToU errors.
+00003190: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000031a0: 696d 615f 7465 6d70 6c61 7465 5f68 6173  ima_template_has
+000031b0: 6820 3d3d 2073 656c 662e 5f69 6d61 5f68  h == self._ima_h
+000031c0: 6173 685f 616c 672e 6765 745f 6666 5f68  ash_alg.get_ff_h
+000031d0: 6173 6828 293a 0a20 2020 2020 2020 2020  ash():.         
+000031e0: 2020 206c 6f67 6765 722e 7761 726e 696e     logger.warnin
+000031f0: 6728 2253 6b69 7070 6564 2074 656d 706c  g("Skipped templ
+00003200: 6174 655f 6861 7368 2076 616c 6964 6174  ate_hash validat
+00003210: 696f 6e20 656e 7472 7920 7769 7468 2046  ion entry with F
+00003220: 465f 4841 5348 2229 0a20 2020 2020 2020  F_HASH").       
+00003230: 2020 2020 2023 2042 7920 6465 6661 756c       # By defaul
+00003240: 7420 546f 4d54 6f55 2065 7272 6f72 7320  t ToMToU errors 
+00003250: 6172 6520 6e6f 7420 7472 6561 7465 6420  are not treated 
+00003260: 6173 2061 2066 6169 6c75 7265 0a20 2020  as a failure.   
+00003270: 2020 2020 2020 2020 2069 6620 636f 6e66           if conf
+00003280: 6967 2e67 6574 626f 6f6c 6561 6e28 2276  ig.getboolean("v
+00003290: 6572 6966 6965 7222 2c20 2269 676e 6f72  erifier", "ignor
+000032a0: 655f 746f 6d74 6f75 5f65 7272 6f72 7322  e_tomtou_errors"
+000032b0: 2c20 6661 6c6c 6261 636b 3d54 7275 6529  , fallback=True)
+000032c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000032d0: 2020 6661 696c 7572 652e 6164 645f 6576    failure.add_ev
+000032e0: 656e 7428 2274 6f6d 746f 7522 2c20 2268  ent("tomtou", "h
+000032f0: 6173 6820 7661 6c69 6461 7469 6f6e 2077  ash validation w
+00003300: 6173 2073 6b69 7070 6564 222c 2054 7275  as skipped", Tru
+00003310: 6529 0a20 2020 2020 2020 2020 2020 2072  e).            r
+00003320: 6574 7572 6e20 6661 696c 7572 650a 2020  eturn failure.  
+00003330: 2020 2020 2020 6966 2073 656c 662e 696d        if self.im
+00003340: 615f 7465 6d70 6c61 7465 5f68 6173 6820  a_template_hash 
+00003350: 213d 2073 656c 662e 5f69 6d61 5f68 6173  != self._ima_has
+00003360: 685f 616c 672e 6861 7368 2873 656c 662e  h_alg.hash(self.
+00003370: 5f62 7974 6573 293a 0a20 2020 2020 2020  _bytes):.       
+00003380: 2020 2020 2066 6169 6c75 7265 2e61 6464       failure.add
+00003390: 5f65 7665 6e74 280a 2020 2020 2020 2020  _event(.        
+000033a0: 2020 2020 2020 2020 2269 6d61 5f68 6173          "ima_has
+000033b0: 6822 2c0a 2020 2020 2020 2020 2020 2020  h",.            
+000033c0: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+000033d0: 2020 2020 2020 2020 2020 226d 6573 7361            "messa
+000033e0: 6765 223a 2022 494d 4120 7465 6d70 6c61  ge": "IMA templa
+000033f0: 7465 2068 6173 6820 646f 6573 206e 6f74  te hash does not
+00003400: 206d 6174 6368 2074 6865 2063 616c 6375   match the calcu
+00003410: 6c61 7465 6420 6861 7368 2e22 2c0a 2020  lated hash.",.  
+00003420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003430: 2020 2265 7870 6563 7465 6422 3a20 7374    "expected": st
+00003440: 7228 7365 6c66 2e69 6d61 5f74 656d 706c  r(self.ima_templ
+00003450: 6174 655f 6861 7368 292c 0a20 2020 2020  ate_hash),.     
+00003460: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00003470: 676f 7422 3a20 7374 7228 7365 6c66 2e6d  got": str(self.m
+00003480: 6f64 652e 6279 7465 7328 2929 2c0a 2020  ode.bytes()),.  
+00003490: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
+000034a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000034b0: 2054 7275 652c 0a20 2020 2020 2020 2020   True,.         
+000034c0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+000034d0: 2072 6574 7572 6e20 6661 696c 7572 650a   return failure.
+000034e0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000034f0: 5f76 616c 6964 6174 6f72 2069 7320 4e6f  _validator is No
+00003500: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00003510: 6661 696c 7572 652e 6164 645f 6576 656e  failure.add_even
+00003520: 7428 226e 6f5f 7661 6c69 6461 746f 7222  t("no_validator"
+00003530: 2c20 224e 6f20 7661 6c69 6461 746f 7220  , "No validator 
+00003540: 7370 6563 6966 6965 6422 2c20 5472 7565  specified", True
+00003550: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+00003560: 7475 726e 2066 6169 6c75 7265 0a0a 2020  turn failure..  
+00003570: 2020 2020 2020 6661 696c 7572 652e 6d65        failure.me
+00003580: 7267 6528 7365 6c66 2e6d 6f64 652e 6973  rge(self.mode.is
+00003590: 5f64 6174 615f 7661 6c69 6428 7365 6c66  _data_valid(self
+000035a0: 2e5f 7661 6c69 6461 746f 7229 290a 2020  ._validator)).  
+000035b0: 2020 2020 2020 7265 7475 726e 2066 6169        return fai
+000035c0: 6c75 7265 0a                             lure.
```

### Comparing `keylime-7.0.0/keylime/ima/dm_grammar.py` & `keylime-7.2.5/keylime/ima/dm_grammar.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/ima/file_signatures.py` & `keylime-7.2.5/keylime/ima/file_signatures.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,24 +67,24 @@
     """Basic class for Streebog512"""
 
     name = "streebog512"  # type: ignore
     digest_size = 64  # type: ignore
     block_size = 64  # type: ignore
 
 
-HASH_FUNCS = {
+HASH_FUNCS: Dict[int, hashes.HashAlgorithm] = {
     # The list of hash functions we need for signature verification.
-    HashAlgo.HASH_ALGO_MD5: hashes.__dict__.get("MD5"),
-    HashAlgo.HASH_ALGO_SHA1: hashes.__dict__.get("SHA1"),
-    HashAlgo.HASH_ALGO_SHA256: hashes.__dict__.get("SHA256"),
-    HashAlgo.HASH_ALGO_SHA384: hashes.__dict__.get("SHA384"),
-    HashAlgo.HASH_ALGO_SHA512: hashes.__dict__.get("SHA512"),
-    HashAlgo.HASH_ALGO_SHA224: hashes.__dict__.get("SHA224"),
-    HashAlgo.HASH_ALGO_STREEBOG_256: MyStreebog256,
-    HashAlgo.HASH_ALGO_STREEBOG_512: MyStreebog512,
+    HashAlgo.HASH_ALGO_MD5: hashes.MD5(),
+    HashAlgo.HASH_ALGO_SHA1: hashes.SHA1(),
+    HashAlgo.HASH_ALGO_SHA256: hashes.SHA256(),
+    HashAlgo.HASH_ALGO_SHA384: hashes.SHA384(),
+    HashAlgo.HASH_ALGO_SHA512: hashes.SHA512(),
+    HashAlgo.HASH_ALGO_SHA224: hashes.SHA224(),
+    HashAlgo.HASH_ALGO_STREEBOG_256: MyStreebog256(),
+    HashAlgo.HASH_ALGO_STREEBOG_512: MyStreebog512(),
 }
 
 
 class EvmImaXattrType(enum.IntEnum):
     """https://elixir.bootlin.com/linux/v5.9.8/source/security/integrity/integrity.h#L74"""
 
     IMA_XATTR_DIGEST = 1
@@ -324,33 +324,31 @@
             return False
 
         hashfunc = HASH_FUNCS.get(hash_algo)
         if not hashfunc:
             logger.warning("Unsupported hash algo with id '%d'", hash_algo)
             return False
 
-        if filehash_type != hashfunc().name:
-            logger.warning(
-                "Mismatching filehash type %s and ima signature hash used %s", filehash_type, hashfunc().name
-            )
+        if filehash_type != hashfunc.name:
+            logger.warning("Mismatching filehash type %s and ima signature hash used %s", filehash_type, hashfunc.name)
             return False
 
         # Try all the keyrings until we find one with a key with the given keyidv2
         pubkey = None
         for keyring in self.get_all_keyrings():
             pubkey = keyring.get_pubkey_by_keyidv2(keyidv2)
             if pubkey:
                 break
 
         if not pubkey:
             logger.warning("No key with id 0x%08x available", keyidv2)
             return False
 
         try:
-            ImaKeyrings._verify(pubkey, signature[hdrlen:], filehash, hashfunc())
+            ImaKeyrings._verify(pubkey, signature[hdrlen:], filehash, hashfunc)
         except InvalidSignature:
             return False
         return True
 
     def integrity_digsig_verify(self, signature: bytes, filehash: bytes, filehash_type: str) -> bool:
         """Validate the signature against the given hash trying all keyrings.
         This function resembles the kernel code at:
```

### Comparing `keylime-7.0.0/keylime/ima/ima.py` & `keylime-7.2.5/keylime/ima/ima.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import codecs
 import copy
 import enum
 import functools
 import hashlib
 import json
 from typing import Any, Dict, List, Optional, Pattern, Set, TextIO, Tuple, Type
 
@@ -208,26 +207,27 @@
 
         accept_list = runtime_policy[hash_types].get(path.name, None)  # type: ignore
         if accept_list is None:
             logger.warning("File not found in allowlist: %s", path.name)
             failure.add_event("not_in_allowlist", f"File not found in allowlist: {path.name}", True)
             return failure
 
-        if codecs.encode(digest.hash, "hex").decode("utf-8") not in accept_list:
+        hex_hash = digest.hash.hex()
+        if hex_hash not in accept_list:
             logger.warning(
                 "Hashes for file %s don't match %s not in %s",
                 path.name,
-                codecs.encode(digest.hash, "hex").decode("utf-8"),
+                hex_hash,
                 runtime_policy,
             )
             failure.add_event(
                 "runtime_policy_hash",
                 {
                     "message": "Hash not found in runtime policy",
-                    "got": codecs.encode(digest.hash, "hex").decode("utf-8"),
+                    "got": hex_hash,
                     "expected": accept_list,
                 },
                 True,
             )
             return failure
 
     return failure
@@ -317,15 +317,15 @@
     running_hash = agentAttestState.get_pcr_state(config.IMA_PCR, hash_alg)
     assert running_hash
 
     found_pcr = pcrval is None
     errors: Dict[Type[ast.Mode], int] = {}
     pcrval_bytes = b""
     if pcrval is not None:
-        pcrval_bytes = codecs.decode(pcrval.encode("utf-8"), "hex")
+        pcrval_bytes = bytes.fromhex(pcrval)
 
     if runtime_policy is not None:
         exclude_list = runtime_policy.get("excludes")
     else:
         exclude_list = None
 
     ima_log_hash_alg = algorithms.Hash.SHA1
@@ -427,15 +427,15 @@
 
     # Check if any validators failed
     if sum(errors.values()) > 0:
         error_msg = "IMA ERRORS: Some entries couldn't be validated. Number of failures in modes: "
         error_msg += ", ".join([f"{k.__name__ } {v}" for k, v in errors.items()])
         logger.error("%s.", error_msg)
 
-    return codecs.encode(running_hash, "hex").decode("utf-8"), failure
+    return running_hash.hex(), failure
 
 
 def process_measurement_list(
     agentAttestState: AgentAttestState,
     lines: List[str],
     runtime_policy: Optional[RuntimePolicyType] = None,
     pcrval: Optional[str] = None,
@@ -569,32 +569,31 @@
 
     if runtime_policy is None:
         raise ImaValidationError(
             message="No IMA policy provided!",
             code=400,
         )
 
+    # validate that the runtime_policy is proper JSON
+    try:
+        runtime_policy_json = json.loads(runtime_policy)
+    except Exception as error:
+        raise ImaValidationError(message="Runtime policy is not valid JSON!", code=400) from error
+
     # detect if runtime policy is DSSE
-    runtime_policy_json = json.loads(runtime_policy)
     if runtime_policy_json.get("payload"):
         if verify_sig:
             if not signing.verify_dsse_envelope(runtime_policy, runtime_policy_key):
                 raise ImaValidationError(message="Runtime policy failed DSSE signature verification!", code=401)
             logger.info("Runtime policy passed DSSE signature verification")
         else:
             runtime_policy = dsse.b64dec(runtime_policy_json["payload"])
 
-    # validate that the runtime_policy is proper JSON
-    try:
-        lists = json.loads(runtime_policy)
-    except Exception as error:
-        raise ImaValidationError(message="Runtime policy is not valid JSON!", code=400) from error
-
     # Validate exclude list contains valid regular expressions
-    _, excl_err_msg = validators.valid_exclude_list(lists.get("exclude"))
+    _, excl_err_msg = validators.valid_exclude_list(runtime_policy_json.get("exclude"))
     if excl_err_msg:
         raise ImaValidationError(
             message=f"{excl_err_msg} Exclude list regex is misformatted. Please correct the issue and try again.",
             code=400,
         )
```

### Comparing `keylime-7.0.0/keylime/ima/ima_dm.py` & `keylime-7.2.5/keylime/ima/ima_dm.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/ima/ima_test.py` & `keylime-7.2.5/keylime/ima/ima_test.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/ima/types.py` & `keylime-7.2.5/keylime/ima/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     device_rename: DeviceRenameRule
     device_remove: DeviceRemoveRule
     allow_clear: bool
     table_load: TableLoadRule
 
 
 class Policies(TypedDict):
+    version: Required[int]
     match_on: MatchKeyType
     rules: Dict[str, Rule]
 
 
 ### Runtime policy data types
```

### Comparing `keylime-7.0.0/keylime/json.py` & `keylime-7.2.5/keylime/json.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/keylime_logging.py` & `keylime-7.2.5/keylime/keylime_logging.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/migrations/alembic.ini` & `keylime-7.2.5/keylime/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/migrations/env.py` & `keylime-7.2.5/keylime/migrations/env.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/migrations/versions/039322ea079b_add_generator_column.py` & `keylime-7.2.5/keylime/migrations/versions/039322ea079b_add_generator_column.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/migrations/versions/1ac1513ef2a1_fix_mb_and_ima_column_types.py` & `keylime-7.2.5/keylime/migrations/versions/1ac1513ef2a1_fix_mb_and_ima_column_types.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/migrations/versions/257fe0f0c039_add_fields_for_revocation_context_to_.py` & `keylime-7.2.5/keylime/migrations/versions/257fe0f0c039_add_fields_for_revocation_context_to_.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/migrations/versions/2fbc0fb8fa4d_add_checksum_to_allowlist.py` & `keylime-7.2.5/keylime/migrations/versions/2fbc0fb8fa4d_add_checksum_to_allowlist.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/migrations/versions/4089e1c79be9_add_tpm_clockinfo.py` & `keylime-7.2.5/keylime/migrations/versions/4089e1c79be9_add_tpm_clockinfo.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/migrations/versions/4329e2d14944_associate_moved_allowlists_to_agents.py` & `keylime-7.2.5/keylime/migrations/versions/4329e2d14944_associate_moved_allowlists_to_agents.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/migrations/versions/63c30820fdc1_add_mtls_cert_and_ak_to_verifier_db.py` & `keylime-7.2.5/keylime/migrations/versions/63c30820fdc1_add_mtls_cert_and_ak_to_verifier_db.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/migrations/versions/7d5db1a6ffb0_add_agentstates_columns.py` & `keylime-7.2.5/keylime/migrations/versions/7d5db1a6ffb0_add_agentstates_columns.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/migrations/versions/8a44a4364f5a_initial_database_migration.py` & `keylime-7.2.5/keylime/migrations/versions/8a44a4364f5a_initial_database_migration.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/migrations/versions/8c0f8ded1f90_convert_allowlists_to_ima_policies.py` & `keylime-7.2.5/keylime/migrations/versions/8c0f8ded1f90_convert_allowlists_to_ima_policies.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/migrations/versions/8da20383f6e1_extend_ip_field.py` & `keylime-7.2.5/keylime/migrations/versions/8da20383f6e1_extend_ip_field.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/migrations/versions/9169f80345ed_add_supported_version_to_verifiermain_.py` & `keylime-7.2.5/keylime/migrations/versions/9169f80345ed_add_supported_version_to_verifiermain_.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/migrations/versions/a09cc94177f0_add_last_received_quote.py` & `keylime-7.2.5/keylime/migrations/versions/a09cc94177f0_add_last_received_quote.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/migrations/versions/a72aec03d720_migrate_allowlists_to_separate_table.py` & `keylime-7.2.5/keylime/migrations/versions/a72aec03d720_migrate_allowlists_to_separate_table.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/migrations/versions/a79c27ec1054_add_mtls_cert_field_to_registrar.py` & `keylime-7.2.5/keylime/migrations/versions/a79c27ec1054_add_mtls_cert_field_to_registrar.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/migrations/versions/a7a64155ab3a_add_ima_filesigning_keys_column.py` & `keylime-7.2.5/keylime/migrations/versions/a7a64155ab3a_add_ima_filesigning_keys_column.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/migrations/versions/ae898986c6e9_add_mb_refstate_column.py` & `keylime-7.2.5/keylime/migrations/versions/ae898986c6e9_add_mb_refstate_column.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/migrations/versions/b4d024197413_add_verfier_id_to_verifiermain_table.py` & `keylime-7.2.5/keylime/migrations/versions/b4d024197413_add_verfier_id_to_verifiermain_table.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/migrations/versions/bc3b6b551b0a_drop_vtpm_colums.py` & `keylime-7.2.5/keylime/migrations/versions/bc3b6b551b0a_drop_vtpm_colums.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/migrations/versions/bf48e0c4751d_add_attestation_count_column.py` & `keylime-7.2.5/keylime/migrations/versions/bf48e0c4751d_add_attestation_count_column.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/migrations/versions/c3842cc9ee69_store_keyrings_learned_from_ima_log.py` & `keylime-7.2.5/keylime/migrations/versions/c3842cc9ee69_store_keyrings_learned_from_ima_log.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/migrations/versions/cc2630851a1f_receive_the_aik_tpm_from_the_agent.py` & `keylime-7.2.5/keylime/migrations/versions/cc2630851a1f_receive_the_aik_tpm_from_the_agent.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/migrations/versions/eb869a77abd1_create_allowlist_table.py` & `keylime-7.2.5/keylime/migrations/versions/eb869a77abd1_create_allowlist_table.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/migrations/versions/eeb702f77d7d_allowlist_rename.py` & `keylime-7.2.5/keylime/migrations/versions/eeb702f77d7d_allowlist_rename.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/migrations/versions/f35cdd35eb83_move_v_tpm_policy_to_jsonpickletype.py` & `keylime-7.2.5/keylime/migrations/versions/f35cdd35eb83_move_v_tpm_policy_to_jsonpickletype.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/migrations/versions/f82c4252bc4f_add_ip_and_port_to_registrar.py` & `keylime-7.2.5/keylime/migrations/versions/f82c4252bc4f_add_ip_and_port_to_registrar.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/migrations/versions/f838d3cdeead_add_last_successful_attestation.py` & `keylime-7.2.5/keylime/migrations/versions/f838d3cdeead_add_last_successful_attestation.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/registrar_client.py` & `keylime-7.2.5/keylime/registrar_client.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/registrar_common.py` & `keylime-7.2.5/keylime/registrar_common.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 import signal
 import socket
 import sys
 import threading
 from http.server import BaseHTTPRequestHandler, HTTPServer
 from ipaddress import IPv6Address, ip_address
 from socketserver import ThreadingMixIn
-from typing import Any, Dict, Tuple, cast
+from typing import Any, Dict, Optional, Tuple, Union, cast
 
 from cryptography.hazmat.primitives.asymmetric import ec, rsa
 from sqlalchemy.exc import SQLAlchemyError
-from sqlalchemy.orm.exc import NoResultFound
+from sqlalchemy.orm.exc import NoResultFound  # pyright: ignore
 
 from keylime import api_version as keylime_api_version
 from keylime import cert_utils, config, crypto, json, keylime_logging, web_util
 from keylime.common import validators
 from keylime.da import record
 from keylime.db.keylime_db import DBEngineManager, SessionManager
 from keylime.db.registrar_db import RegistrarMain
 from keylime.tpm import tpm2_objects
-from keylime.tpm.tpm_main import tpm
+from keylime.tpm.tpm_main import Tpm
 
 logger = keylime_logging.init_logging("registrar")
 
 
 try:
     engine = DBEngineManager().make_engine("registrar")
 except SQLAlchemyError as err:
@@ -38,15 +38,49 @@
     if rmc:
         rmc = rmc("registrar")
 except record.RecordManagementException as rme:
     logger.error("Error initializing Durable Attestation: %s", rme)
     sys.exit(1)
 
 
-class ProtectedHandler(BaseHTTPRequestHandler, SessionManager):
+class BaseHandler(BaseHTTPRequestHandler, SessionManager):
+    def _validate_input(
+        self, method: str, respond_on_agent_id_none: bool
+    ) -> Tuple[Optional[Dict[str, Union[str, None]]], Optional[str]]:
+        rest_params = web_util.get_restful_params(self.path)
+        if rest_params is None:
+            web_util.echo_json_response(self, 405, "Not Implemented: Use /agents/ interface")
+            return None, None
+
+        if not web_util.validate_api_version(self, cast(str, rest_params["api_version"]), logger):
+            return None, None
+
+        if "agents" not in rest_params:
+            web_util.echo_json_response(self, 400, "URI not supported")
+            logger.warning("%s agent returning 400 response. uri not supported: %s", method, self.path)
+            return None, None
+
+        agent_id = rest_params["agents"]
+
+        if agent_id is None:
+            if respond_on_agent_id_none:
+                web_util.echo_json_response(self, 400, "agent id not found in uri")
+                logger.warning("%s agent returning 400 response. agent id not found in uri %s", method, self.path)
+            return rest_params, None
+
+        # If the agent ID is not valid (wrong set of characters), just do nothing.
+        if not validators.valid_agent_id(agent_id):
+            web_util.echo_json_response(self, 400, "agent_id is not valid")
+            logger.error("%s received an invalid agent ID: %s", method, agent_id)
+            return None, None
+
+        return rest_params, agent_id
+
+
+class ProtectedHandler(BaseHandler):
     def do_HEAD(self) -> None:
         """HEAD not supported"""
         web_util.echo_json_response(self, 405, "HEAD not supported")
 
     def do_PATCH(self) -> None:
         """PATCH not supported"""
         web_util.echo_json_response(self, 405, "PATCH not supported")
@@ -55,38 +89,20 @@
         """This method handles the GET requests to retrieve status on agents from the Registrar Server.
 
         Currently, only agents resources are available for GETing, i.e. /agents. All other GET uri's
         will return errors. agents requests require a single agent_id parameter which identifies the
         agent to be returned. If the agent_id is not found, a 404 response is returned.
         """
         session = SessionManager().make_session(engine)
-        rest_params = web_util.get_restful_params(self.path)
-        if rest_params is None:
-            web_util.echo_json_response(self, 405, "Not Implemented: Use /agents/ interface")
-            return
 
-        if not web_util.validate_api_version(self, cast(str, rest_params["api_version"]), logger):
+        rest_params, agent_id = self._validate_input("GET", False)
+        if not rest_params:
             return
 
-        if "agents" not in rest_params:
-            web_util.echo_json_response(self, 400, "uri not supported")
-            logger.warning("GET returning 400 response. uri not supported: %s", self.path)
-            return
-
-        agent_id = rest_params["agents"]
-
         if agent_id is not None:
-            # If the agent ID is not valid (wrong set of characters),
-            # just do nothing.
-            if not validators.valid_agent_id(agent_id):
-                web_util.echo_json_response(self, 400, "agent_id not not valid")
-                logger.error("GET received an invalid agent ID: %s", agent_id)
-                return
-
-            agent = None
             try:
                 agent = session.query(RegistrarMain).filter_by(agent_id=agent_id).first()
             except SQLAlchemyError as e:
                 logger.error("SQLAlchemy Error for agent ID %s: %s", agent_id, e)
                 return
 
             if agent is None:
@@ -105,15 +121,15 @@
                 "ekcert": agent.ekcert,
                 "mtls_cert": agent.mtls_cert,
                 "ip": agent.ip,
                 "port": agent.port,
                 "regcount": agent.regcount,
             }
 
-            if agent.virtual:
+            if agent.virtual:  # pyright: ignore
                 response["provider_keys"] = agent.provider_keys
 
             web_util.echo_json_response(self, 200, "Success", response)
             logger.info("GET returning 200 response for agent_id: %s", agent_id)
         else:
             # return the available registered uuids from the DB
             json_response = session.query(RegistrarMain.agent_id).all()
@@ -134,37 +150,20 @@
     def do_DELETE(self) -> None:
         """This method handles the DELETE requests to remove agents from the Registrar Server.
 
         Currently, only agents resources are available for DELETEing, i.e. /agents. All other DELETE uri's will return errors.
         agents requests require a single agent_id parameter which identifies the agent to be deleted.
         """
         session = SessionManager().make_session(engine)
-        rest_params = web_util.get_restful_params(self.path)
-        if rest_params is None:
-            web_util.echo_json_response(self, 405, "Not Implemented: Use /agents/ interface")
-            return
 
-        if not web_util.validate_api_version(self, cast(str, rest_params["api_version"]), logger):
-            return
-
-        if "agents" not in rest_params:
-            web_util.echo_json_response(self, 400, "URI not supported")
-            logger.warning("DELETE agent returning 400 response. uri not supported: %s", self.path)
+        rest_params, agent_id = self._validate_input("DELETE", False)
+        if not rest_params:
             return
 
-        agent_id = rest_params["agents"]
-
         if agent_id is not None:
-            # If the agent ID is not valid (wrong set of characters),
-            # just do nothing.
-            if not validators.valid_agent_id(agent_id):
-                web_util.echo_json_response(self, 400, "agent_id not not valid")
-                logger.error("DELETE received an invalid agent ID: %s", agent_id)
-                return
-
             if session.query(RegistrarMain).filter_by(agent_id=agent_id).delete():
                 # send response
                 try:
                     session.commit()
                 except SQLAlchemyError as e:
                     logger.error("SQLAlchemy Error: %s", e)
                 web_util.echo_json_response(self, 200, "Success")
@@ -177,15 +176,15 @@
         web_util.echo_json_response(self, 404)
 
     # pylint: disable=W0622
     def log_message(self, format: str, *args: Any) -> None:
         return
 
 
-class UnprotectedHandler(BaseHTTPRequestHandler, SessionManager):
+class UnprotectedHandler(BaseHandler):
     def do_HEAD(self) -> None:
         """HEAD not supported"""
         web_util.echo_json_response(self, 405, "HEAD not supported")
 
     def do_PATCH(self) -> None:
         """PATCH not supported"""
         web_util.echo_json_response(self, 405, "PATCH not supported")
@@ -208,47 +207,55 @@
         version_info = {
             "current_version": keylime_api_version.current_version(),
             "supported_versions": keylime_api_version.all_versions(),
         }
 
         web_util.echo_json_response(self, 200, "Success", version_info)
 
+    @staticmethod
+    def get_network_params(
+        json_body: Dict[str, Any], agent_id: str
+    ) -> Tuple[Optional[str], Optional[int], Optional[str]]:
+        # Validate ip and port
+        ip = json_body.get("ip")
+        if ip is not None:
+            try:
+                ipaddress.ip_address(ip)
+            except ValueError:
+                logger.warning("Contact ip for agent %s is not a valid ip got: %s.", agent_id, ip)
+                ip = None
+
+        port = json_body.get("port")
+        if port is not None:
+            try:
+                port = int(port)
+                if port < 1 or port > 65535:
+                    logger.warning("Contact port for agent %s is not a number between 1 and got: %s.", agent_id, port)
+                    port = None
+            except ValueError:
+                logger.warning("Contact port for agent %s is not a valid number got: %s.", agent_id, port)
+                port = None
+
+        mtls_cert = json_body.get("mtls_cert")
+        if mtls_cert is None or mtls_cert == "disabled":
+            logger.warning("Agent %s did not send a mTLS certificate. Most operations will not work!", agent_id)
+
+        return ip, port, mtls_cert
+
     def do_POST(self) -> None:
         """This method handles the POST requests to add agents to the Registrar Server.
 
         Currently, only agents resources are available for POSTing, i.e. /agents. All other POST uri's
         will return errors. POST requests require an an agent_id identifying the agent to add, and json
         block sent in the body with 2 entries: ek and aik.
         """
         session = SessionManager().make_session(engine)
-        rest_params = web_util.get_restful_params(self.path)
-        if rest_params is None:
-            web_util.echo_json_response(self, 405, "Not Implemented: Use /agents/ interface")
-            return
 
-        if not web_util.validate_api_version(self, cast(str, rest_params["api_version"]), logger):
-            return
-
-        if "agents" not in rest_params:
-            web_util.echo_json_response(self, 400, "uri not supported")
-            logger.warning("POST agent returning 400 response. uri not supported: %s", self.path)
-            return
-
-        agent_id = rest_params["agents"]
-
-        if agent_id is None:
-            web_util.echo_json_response(self, 400, "agent id not found in uri")
-            logger.warning("POST agent returning 400 response. agent id not found in uri %s", self.path)
-            return
-
-        # If the agent ID is not valid (wrong set of characters), just
-        # do nothing.
-        if not validators.valid_agent_id(agent_id):
-            web_util.echo_json_response(self, 400, "agent id not valid")
-            logger.error("POST received an invalid agent ID: %s", agent_id)
+        _, agent_id = self._validate_input("POST", True)
+        if not agent_id:
             return
 
         try:
             content_length = int(self.headers.get("Content-Length", 0))
             if content_length == 0:
                 web_util.echo_json_response(self, 400, "Expected non zero content length")
                 logger.warning("POST for %s returning 400 response. Expected non zero content length.", agent_id)
@@ -256,16 +263,14 @@
 
             post_body = self.rfile.read(content_length)
             json_body = json.loads(post_body)
 
             ekcert = json_body["ekcert"]
             aik_tpm = json_body["aik_tpm"]
 
-            initialize_tpm = tpm()
-
             if ekcert is None or ekcert == "emulator":
                 logger.warning("Agent %s did not submit an ekcert", agent_id)
                 ek_tpm = json_body["ek_tpm"]
             else:
                 if "ek_tpm" in json_body:
                     # This would mean the agent submitted both a non-None ekcert, *and*
                     #  an ek_tpm... We can deal with it by just ignoring the ek_tpm they sent
@@ -289,95 +294,71 @@
                     agent_id,
                     tpm2_objects.object_attributes_description(aik_attrs),
                     tpm2_objects.object_attributes_description(tpm2_objects.AK_EXPECTED_ATTRS),
                 )
                 return
 
             # try to encrypt the AIK
-            aik_enc = initialize_tpm.encryptAIK(
+            aik_enc = Tpm.encryptAIK(
                 agent_id,
                 base64.b64decode(ek_tpm),
                 base64.b64decode(aik_tpm),
             )
-            if aik_enc is not None:
-                (blob, key) = aik_enc
-            else:
+            if aik_enc is None:
                 logger.warning("Agent %s failed encrypting AIK", agent_id)
                 web_util.echo_json_response(self, 400, "Error: failed encrypting AK")
                 return
 
+            blob, key = aik_enc
+
             # special behavior if we've registered this uuid before
             regcount = 1
             try:
                 agent = session.query(RegistrarMain).filter_by(agent_id=agent_id).first()
             except NoResultFound:
                 agent = None
             except SQLAlchemyError as e:
                 logger.error("SQLAlchemy Error: %s", e)
                 raise
 
             if agent is not None:
                 # keep track of how many ek-ekcerts have registered on this uuid
                 assert isinstance(agent.regcount, int)
                 regcount = agent.regcount
-                if agent.ek_tpm != ek_tpm or agent.ekcert != ekcert:
+                if agent.ek_tpm != ek_tpm or agent.ekcert != ekcert:  # pyright: ignore
                     logger.warning("WARNING: Overwriting previous registration for this UUID with new ek-ekcert pair!")
                     regcount += 1
 
                 # force overwrite
                 logger.info("Overwriting previous registration for this UUID.")
                 try:
                     session.query(RegistrarMain).filter_by(agent_id=agent_id).delete()
                     session.commit()
                 except SQLAlchemyError as e:
                     logger.error("SQLAlchemy Error: %s", e)
                     raise
-            # Check for ip and port
-            contact_ip = json_body.get("ip", None)
-            contact_port = json_body.get("port", None)
 
-            # Validate ip and port
-            if contact_ip is not None:
-                try:
-                    # Use parser from the standard library instead of implementing our own
-                    ipaddress.ip_address(contact_ip)
-                except ValueError:
-                    logger.warning("Contact ip for agent %s is not a valid ip got: %s.", agent_id, contact_ip)
-                    contact_ip = None
-            if contact_port is not None:
-                try:
-                    contact_port = int(contact_port)
-                    if contact_port < 1 or contact_port > 65535:
-                        logger.warning(
-                            "Contact port for agent %s is not a number between 1 and got: %s.", agent_id, contact_port
-                        )
-                        contact_port = None
-                except ValueError:
-                    logger.warning("Contact port for agent %s is not a valid number got: %s.", agent_id, contact_port)
-                    contact_port = None
-
-            # Check for mTLS cert
-            mtls_cert = json_body.get("mtls_cert", None)
-            if mtls_cert is None or mtls_cert == "disabled":
-                logger.warning("Agent %s did not send a mTLS certificate. Most operations will not work!", agent_id)
+            # Check for ip and port and mTLS cert
+            contact_ip, contact_port, mtls_cert = UnprotectedHandler.get_network_params(json_body, agent_id)
 
             # Add values to database
-            d: Dict[str, Any] = {}
-            d["agent_id"] = agent_id
-            d["ek_tpm"] = ek_tpm
-            d["aik_tpm"] = aik_tpm
-            d["ekcert"] = ekcert
-            d["ip"] = contact_ip
-            d["mtls_cert"] = mtls_cert
-            d["port"] = contact_port
-            d["virtual"] = int(ekcert == "virtual")
-            d["active"] = int(False)
-            d["key"] = key
-            d["provider_keys"] = {}
-            d["regcount"] = regcount
+            d: Dict[str, Any] = {
+                "agent_id": agent_id,
+                "ek_tpm": ek_tpm,
+                "aik_tpm": aik_tpm,
+                "ekcert": ekcert,
+                "ip": contact_ip,
+                "mtls_cert": mtls_cert,
+                "port": contact_port,
+                "virtual": int(ekcert == "virtual"),
+                "active": int(False),
+                "key": key,
+                "provider_keys": {},
+                "regcount": regcount,
+            }
 
             try:
                 session.add(RegistrarMain(**d))
                 session.commit()
             except SQLAlchemyError as e:
                 logger.error("SQLAlchemy Error: %s", e)
                 raise
@@ -404,39 +385,17 @@
     def do_PUT(self) -> None:
         """This method handles the PUT requests to add agents to the Registrar Server.
 
         Currently, only agents resources are available for PUTing, i.e. /agents. All other PUT uri's
         will return errors.
         """
         session = SessionManager().make_session(engine)
-        rest_params = web_util.get_restful_params(self.path)
-        if rest_params is None:
-            web_util.echo_json_response(self, 405, "Not Implemented: Use /agents/ interface")
-            return
 
-        if not web_util.validate_api_version(self, cast(str, rest_params["api_version"]), logger):
-            return
-
-        if "agents" not in rest_params:
-            web_util.echo_json_response(self, 400, "uri not supported")
-            logger.warning("PUT agent returning 400 response. uri not supported: %s", self.path)
-            return
-
-        agent_id = rest_params["agents"]
-
-        if agent_id is None:
-            web_util.echo_json_response(self, 400, "agent id not found in uri")
-            logger.warning("PUT agent returning 400 response. agent id not found in uri %s", self.path)
-            return
-
-        # If the agent ID is not valid (wrong set of characters), just
-        # do nothing.
-        if not validators.valid_agent_id(agent_id):
-            web_util.echo_json_response(self, 400, "agent_id not not valid")
-            logger.error("PUT received an invalid agent ID: %s", agent_id)
+        _, agent_id = self._validate_input("PUT", True)
+        if not agent_id:
             return
 
         try:
             content_length = int(self.headers.get("Content-Length", 0))
             if content_length == 0:
                 web_util.echo_json_response(self, 400, "Expected non zero content length")
                 logger.warning("PUT for %s returning 400 response. Expected non zero content length.", agent_id)
```

### Comparing `keylime-7.0.0/keylime/requests_client.py` & `keylime-7.2.5/keylime/requests_client.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/revocation_notifier.py` & `keylime-7.2.5/keylime/revocation_notifier.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/signing.py` & `keylime-7.2.5/keylime/signing.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/tenant.py` & `keylime-7.2.5/keylime/tenant.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from keylime.cli import options, policies
 from keylime.cmd import user_data_encrypt
 from keylime.common import algorithms, retry, states, validators
 from keylime.ip_util import bracketize_ipv6
 from keylime.requests_client import RequestsClient
 from keylime.tpm import tpm2_objects
 from keylime.tpm.tpm_abstract import TPM_Utilities
-from keylime.tpm.tpm_main import tpm
+from keylime.tpm.tpm_main import Tpm
 
 # setup logging
 logger = keylime_logging.init_logging("tenant")
 
 
 # special exception that suppresses stack traces when it happens
 class UserError(Exception):
@@ -91,15 +91,15 @@
     tls_context: Optional[ssl.SSLContext] = None
 
     # Context with the agent's mTLS certificate
     agent_tls_context: Optional[ssl.SSLContext] = None
 
     payload: Optional[bytes] = None
 
-    tpm_instance: tpm = tpm()
+    tpm_instance: Tpm = Tpm()
 
     def __init__(self) -> None:
         """Set up required values and TLS"""
         self.nonce = None
         self.agent_ip = None
         self.agent_port = None
         self.verifier_id = None
@@ -359,15 +359,18 @@
 
             if not os.path.exists(args["ca_dir"]) or not os.path.exists(os.path.join(args["ca_dir"], "cacert.crt")):
                 logger.warning("CA directory does not exist. Creating...")
                 ca_util.cmd_init(args["ca_dir"])
             if not os.path.exists(os.path.join(args["ca_dir"], f"{self.agent_uuid}-private.pem")):
                 ca_util.cmd_mkcert(args["ca_dir"], self.agent_uuid)
 
-            cert_pkg, serial, subject = ca_util.cmd_certpkg(args["ca_dir"], self.agent_uuid)
+            try:
+                cert_pkg, serial, subject = ca_util.cmd_certpkg(args["ca_dir"], self.agent_uuid)
+            except Exception as e:
+                raise UserError(f"Error reading the keystore from {args['ca_dir']}: {e}") from e
 
             # support revocation
             if not os.path.exists(os.path.join(args["ca_dir"], "RevocationNotifier-private.pem")):
                 ca_util.cmd_mkcert(args["ca_dir"], "RevocationNotifier")
             rev_package, _, _ = ca_util.cmd_certpkg(args["ca_dir"], "RevocationNotifier")
 
             # extract public and private keys from package
@@ -554,15 +557,15 @@
             "cloudagent_port": self.agent_port,
             "verifier_ip": self.verifier_ip,
             "verifier_port": self.verifier_port,
             "tpm_policy": json.dumps(self.tpm_policy),
             "runtime_policy": self.runtime_policy,
             "runtime_policy_name": self.runtime_policy_name,
             "runtime_policy_key": self.runtime_policy_key,
-            "mb_refstate": json.dumps(self.mb_refstate),
+            "mb_refstate": self.mb_refstate,
             "ima_sign_verification_keys": self.ima_sign_verification_keys,
             "metadata": json.dumps(self.metadata),
             "revocation_key": self.revocation_key,
             "accept_tpm_hash_algs": self.accept_tpm_hash_algs,
             "accept_tpm_encryption_algs": self.accept_tpm_encryption_algs,
             "accept_tpm_signing_algs": self.accept_tpm_signing_algs,
             "ak_tpm": self.registrar_data["aik_tpm"],
@@ -1164,30 +1167,36 @@
                         self.maxr,
                         next_retry,
                     )
                     time.sleep(next_retry)
                     continue
                 self.do_cvstop()
                 raise e
+
+            mac = ""
+            ex_mac = crypto.do_hmac(self.K, challenge)
+
             if response.status_code == 200:
                 if "results" not in response_json or "hmac" not in response_json["results"]:
-                    logger.critical("Error: unexpected http response body from Cloud Agent: %s", response.status_code)
+                    logger.critical(
+                        "Error: unexpected http response body from on agent %s with port %s : %s",
+                        self.agent_ip,
+                        self.agent_port,
+                        response.status_code,
+                    )
                     self.do_cvstop()
                     break
                 mac = response_json["results"]["hmac"]
 
-                ex_mac = crypto.do_hmac(self.K, challenge)
-
                 if mac == ex_mac:
-                    logger.info("Key derivation successful")
-                else:
-                    logger.error("Key derivation failed")
-                    self.do_cvstop()
-            else:
-                keylime_logging.log_http_response(logger, logging.ERROR, response_json)
+                    logger.info("Agent on %s with port %s successfully derived key", self.agent_ip, self.agent_port)
+
+            if mac != ex_mac:
+                if response.status_code != 200:
+                    keylime_logging.log_http_response(logger, logging.ERROR, response_json)
                 numtries += 1
                 if numtries >= self.maxr:
                     logger.error("Agent on %s with port %s failed key derivation", self.agent_ip, self.agent_port)
                     self.do_cvstop()
                     sys.exit()
                 next_retry = retry.retry_time(self.exponential_backoff, self.retry_interval, numtries, logger)
                 logger.info(
```

### Comparing `keylime-7.0.0/keylime/tornado_requests.py` & `keylime-7.2.5/keylime/tornado_requests.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/tpm/tpm2_objects.py` & `keylime-7.2.5/keylime/tpm/tpm2_objects.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 import hashlib
 import struct
-from typing import Any, Tuple, Union, cast
+from typing import Any, Dict, Tuple, Union, cast
 
 import cryptography.hazmat.primitives.asymmetric.ec as crypto_ec
 from cryptography.hazmat.backends import default_backend
+from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.asymmetric.ec import (
     EllipticCurve,
     EllipticCurvePublicKey,
     EllipticCurvePublicNumbers,
 )
 from cryptography.hazmat.primitives.asymmetric.rsa import RSAPublicKey, RSAPublicNumbers
+from cryptography.hazmat.primitives.ciphers import algorithms
+
+from keylime.tpm.types import TpmsAttestType
 
 pubkey_type = Union[RSAPublicKey, EllipticCurvePublicKey]
 
 
 def _pack_in_tpm2b(val: bytes) -> bytes:
     return struct.pack(">H", len(val)) + val
 
@@ -34,14 +38,21 @@
 TPM_ALG_SHA256 = 0x000B
 TPM_ALG_SHA384 = 0x000C
 TPM_ALG_SHA512 = 0x000D
 
 TPM_ALG_AES = 0x0006
 TPM_ALG_CFB = 0x0043
 
+TPM_ALG_RSASSA = 0x0014
+
+TPM_ALG_ECDSA = 0x0018
+
+TPM_GENERATED_VALUE = 0xFF544347
+
+TPM_ST_ATTEST_QUOTE = 0x8018
 
 # These are the object attribute values important for EK certs
 OA_FIXEDTPM = 0x00000002
 OA_STCLEAR = 0x00000004
 OA_FIXEDPARENT = 0x00000010
 OA_SENSITIVEDATAORIGIN = 0x00000020
 OA_USERWITHAUTH = 0x00000040
@@ -56,14 +67,27 @@
 # These are some common object attribute values
 # Source for AK_EXPECTED_ATTRS: tpm2-tools, tpm2_createak.c, set_key_algorithm
 AK_EXPECTED_ATTRS = (
     OA_RESTRICTED | OA_USERWITHAUTH | OA_SIGN_ENCRYPT | OA_FIXEDTPM | OA_FIXEDPARENT | OA_SENSITIVEDATAORIGIN
 )
 
 
+# The hash functions used by TPM
+HASH_FUNCS: Dict[int, hashes.HashAlgorithm] = {
+    TPM_ALG_SHA1: hashes.SHA1(),
+    TPM_ALG_SHA256: hashes.SHA256(),
+    TPM_ALG_SHA384: hashes.SHA384(),
+    TPM_ALG_SHA512: hashes.SHA512(),
+}
+
+SYMCIPHER_FUNCS = {
+    TPM_ALG_AES: algorithms.AES,
+}
+
+
 class NonAsymAlgSpecificParameters:
     sym_algorithm: int
     sym_keybits: int
     sym_mode: int
     sym_details: int
     scheme_scheme: int
     scheme_details: int
@@ -243,44 +267,46 @@
     (length,) = struct.unpack(">H", vals[0:2])
     # Ignore the length itself when returning
     vals = vals[2:]
     # Return first the currect buffer, and then the rest
     return (vals[:length], vals[length:])
 
 
-def pubkey_from_tpm2b_public(public: bytes) -> pubkey_type:
+def pubkey_parms_from_tpm2b_public(
+    public: bytes,
+) -> Tuple[pubkey_type, int]:
     (public, rest) = _extract_tpm2b(public)
     if len(rest) != 0:
         raise ValueError("More in tpm2b_public than tpmt_public")
-    # Extract type, [nameAlg], and [objectAttributes] (we don't care about the
-    #  latter two)
-    (alg_type, _, _) = struct.unpack(">HHI", public[0:8])
+    # Extract type, nameAlg, and [objectAttributes] (we don't care about the
+    #  latter)
+    (alg_type, name_alg, _) = struct.unpack(">HHI", public[0:8])
     # Ignore the authPolicy
     (_, sym_parms) = _extract_tpm2b(public[8:])
     # Ignore the non-asym-alg parameters
-    (sym_mode,) = struct.unpack(">H", sym_parms[0:2])
+    (sym_alg,) = struct.unpack(">H", sym_parms[0:2])
     # Ignore the sym_mode and keybits (4 bytes), possibly symmetric (2) and sign
     #  scheme (2)
     to_skip = 4 + 2  # sym_mode, keybits and sign scheme
-    if sym_mode != TPM2_ALG_NULL:
+    if sym_alg != TPM2_ALG_NULL:
         to_skip = to_skip + 2
     asym_parms = sym_parms[to_skip:]
 
     # Handle fields
     if alg_type == TPM_ALG_RSA:
         (keybits, exponent) = struct.unpack(">HI", asym_parms[0:6])
         if exponent == 0:
             exponent = 65537
         (modulus, _) = _extract_tpm2b(asym_parms[6:])
         if (len(modulus) * 8) != keybits:
             raise ValueError(f"Misparsed either modulus or keybits: {len(modulus)}*8 != {keybits}")
         bmodulus = int.from_bytes(modulus, byteorder="big")
 
         rsa_numbers = RSAPublicNumbers(exponent, bmodulus)
-        return rsa_numbers.public_key(backend=default_backend())
+        return rsa_numbers.public_key(backend=default_backend()), name_alg
 
     if alg_type == TPM_ALG_ECC:
         (curve_id, _) = struct.unpack(">HH", asym_parms[0:4])
         asym_x = asym_parms[4:]
         curve = _curve_from_curve_id(curve_id)
 
         (x, asym_y) = _extract_tpm2b(asym_x)
@@ -293,19 +319,24 @@
         if (len(y) * 8) != curve.key_size:
             raise ValueError(f"Misparsed either Y or curve curve: {len(y)}*8 != {curve.key_size}")
 
         bx = int.from_bytes(x, byteorder="big")
         by = int.from_bytes(y, byteorder="big")
 
         ecc_numbers = EllipticCurvePublicNumbers(bx, by, curve)
-        return ecc_numbers.public_key(backend=default_backend())
+        return ecc_numbers.public_key(backend=default_backend()), name_alg
 
     raise ValueError(f"Invalid tpm2b_public type: {alg_type}")
 
 
+def pubkey_from_tpm2b_public(public: bytes) -> pubkey_type:
+    pubkey, _ = pubkey_parms_from_tpm2b_public(public)
+    return pubkey
+
+
 def tpm2b_public_from_pubkey(
     pubkey: pubkey_type, name_alg: int, attributes: int, auth_policy: bytes, parms: NonAsymAlgSpecificParameters
 ) -> bytes:
     """
     Returns a reconstructed TPM2B_PUBLIC from a public key.
     """
     if isinstance(pubkey, RSAPublicKey):
@@ -373,14 +404,28 @@
         _,
         _,
         attrs,
     ) = struct.unpack(">HHHI", public[0:10])
     return cast(int, attrs)
 
 
+def get_tpm2b_public_symkey_params(
+    public: bytes,
+) -> Tuple[int, int]:
+    # Ignore length, type, namealg and attributes
+    (public, rest) = _extract_tpm2b(public)
+    if len(rest) != 0:
+        raise ValueError("More in tpm2b_public than tpmt_public")
+    # Ignore the authPolicy
+    (_, sym_parms) = _extract_tpm2b(public[8:])
+
+    sym_alg, symkey_bits = struct.unpack(">HH", sym_parms[0:4])
+    return sym_alg, symkey_bits
+
+
 def get_tpm2b_public_name(public: bytes) -> str:
     """
     Return the TPM name of an object provided as TPM2B_PUBLIC.
 
     The name is equal to: nameAlg || H(T_Public)
     where
         H is the hash function identified by nameAlg
@@ -436,7 +481,87 @@
     return tpm2b_public_from_pubkey(
         pubkey,
         EK_LOW_NAMEALG,
         EK_LOW_ATTRIBUTES,
         EK_LOW_AUTH_POLICY,
         EK_LOW_NON_ASYM_ALG_PARMS,
     )
+
+
+def unmarshal_tpms_clock_info(clock_info: bytes) -> Dict[str, int]:
+    clock, resetCount, restartCount, safe = struct.unpack(">QIIB", clock_info)
+    return {"clock": clock, "resetCount": resetCount, "restartCount": restartCount, "safe": safe}
+
+
+def unmarshal_tpms_quote_info(tpms_quote_info: bytes) -> bytes:
+    # TPMS_QUOTE_INFO: TPML_PCR_SELECTION
+    _, sz = unmarshal_tpml_pcr_selection(tpms_quote_info)
+    o = sz
+    # TPMS_QUOTE_INFO: TPM2B_DIGEST
+    (sz,) = struct.unpack_from(">H", tpms_quote_info, o)
+    o = o + 2
+    (pcrDigest,) = struct.unpack_from(f"{sz}s", tpms_quote_info, o)
+
+    return bytes(pcrDigest)
+
+
+def unmarshal_tpms_attest(tpms_attest: bytes) -> TpmsAttestType:
+    magic, typ = struct.unpack_from(">IH", tpms_attest, 0)
+    if magic != TPM_GENERATED_VALUE:
+        raise Exception("Bad magic in tpms_attest")
+    if typ != TPM_ST_ATTEST_QUOTE:
+        raise Exception(f"Unsupported type in tpms_attest: {typ:#x}")
+    o = 6
+    # TPM2B_NAME
+    (sz,) = struct.unpack_from(">H", tpms_attest, o)
+    o = o + 2 + sz
+    # TPM2B_NAME
+    (sz,) = struct.unpack_from(">H", tpms_attest, o)
+    o = o + 2
+    (extradata,) = struct.unpack_from(f"{sz}s", tpms_attest, o)
+    o = o + sz
+    # TPMS_CLOCK_INFO
+    clock_info = unmarshal_tpms_clock_info(tpms_attest[o : o + 17])
+    o = o + 17
+    # UINT64
+    o = o + 8
+    pcrDigest = unmarshal_tpms_quote_info(tpms_attest[o:])
+
+    return {
+        "clockInfo": clock_info,
+        "extraData": bytes(extradata),
+        "attested.quote.pcrDigest": pcrDigest,
+    }
+
+
+def get_tpms_attest_clock_info(tpms_attest: bytes) -> Dict[str, int]:
+    retDict = unmarshal_tpms_attest(tpms_attest)
+    return retDict["clockInfo"]
+
+
+def unmarshal_tpms_pcr_selection(tpms_pcr_selection: bytes) -> Tuple[int, int, int]:
+    hash_alg, size_of_select = struct.unpack_from(">HB", tpms_pcr_selection, 0)
+    (select,) = struct.unpack_from(f"{size_of_select}s", tpms_pcr_selection, 3)
+    return hash_alg, select, 3 + size_of_select
+
+
+def unmarshal_tpml_pcr_selection(tpml_pcr_selection: bytes) -> Tuple[Dict[int, int], int]:
+    (count,) = struct.unpack_from(">I", tpml_pcr_selection, 0)
+    o = 4
+
+    selections: Dict[int, int] = {}
+    for _ in range(0, count):
+        hash_alg, select, sz = unmarshal_tpms_pcr_selection(tpml_pcr_selection[o:])
+        selections[hash_alg] = select
+        o = o + sz
+
+    return selections, o
+
+
+def tpms_ecc_point_marshal(public_key: EllipticCurvePublicKey) -> bytes:
+    pn = public_key.public_numbers()
+
+    sz = (pn.x.bit_length() + 7) // 8
+    secret = struct.pack(">H", sz) + pn.x.to_bytes(sz, "big")
+
+    sz = (pn.y.bit_length() + 7) // 8
+    return secret + struct.pack(">H", sz) + pn.y.to_bytes(sz, "big")
```

### Comparing `keylime-7.0.0/keylime/tpm/tpm2_objects_test.py` & `keylime-7.2.5/keylime/tpm/tpm2_objects_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,19 +13,24 @@
     OA_FIXEDTPM,
     OA_NODA,
     OA_RESTRICTED,
     OA_SENSITIVEDATAORIGIN,
     OA_SIGN_ENCRYPT,
     OA_STCLEAR,
     OA_USERWITHAUTH,
+    TPM_ALG_AES,
+    TPM_ALG_SHA256,
     ek_low_tpm2b_public_from_pubkey,
     get_tpm2b_public_name,
     get_tpm2b_public_object_attributes,
+    get_tpm2b_public_symkey_params,
     object_attributes_description,
     pubkey_from_tpm2b_public,
+    pubkey_parms_from_tpm2b_public,
+    unmarshal_tpms_attest,
 )
 
 
 class TestTpm2Objects(unittest.TestCase):
     def test_get_tpm2b_public_name(self) -> None:
         test_pub = base64.b64decode(
             "ARgAAQALAAUAcgAAABAAFAALCAAAAAAAAQDJBIF+SxeEt8TAwcnMZIvJWs3luBARcI"
@@ -178,14 +183,18 @@
         assert isinstance(correct_rsa_pubkey, rsa.RSAPublicKey)
         new_rsa_pubkey_n = new_rsa_pubkey.public_numbers()
         correct_rsa_pubkey_n = correct_rsa_pubkey.public_numbers()
         self.assertEqual(new_rsa_pubkey.key_size, correct_rsa_pubkey.key_size)
         self.assertEqual(new_rsa_pubkey_n.e, correct_rsa_pubkey_n.e)  # pylint: disable=no-member
         self.assertEqual(new_rsa_pubkey_n.n, correct_rsa_pubkey_n.n)  # pylint: disable=no-member
 
+        sym_alg, symkey_bits = get_tpm2b_public_symkey_params(correct_rsa_obj)
+        self.assertEqual(sym_alg, TPM_ALG_AES)
+        self.assertEqual(symkey_bits, 128)
+
     def test_pubkey_from_tpm2b_public_rsa_without_encryption(self) -> None:
         new_rsa_pubkey = pubkey_from_tpm2b_public(
             bytes.fromhex(
                 "01180001000b00050072000000100014000b0800000000000100cac43903c6"
                 "16bba049ce413c961c901b56181392c7999e672e6e5ecdd7a625d4702c3d78"
                 "deac81e1372b0ca1894ac0f16add636bb53d3d5b112d8f3b169ccadef6bac0"
                 "d909067d1ff81dae34b26cd538a52fa20ee7bbf3b16214417d35bde80cbb0f"
@@ -237,16 +246,17 @@
         )
         correct_ec_obj = base64.b64decode(
             "AHoAIwALAAMAsgAgg3GXZ0SEs/gakMyNRqXXJP1S124GUgtk8qHaGzMUaaoABgCAAE"
             "MAEAADABAAINK9AtBnW5bwNG2ZIWDrM8w/h03Ht2lp3MUosV05DeBHACBZkRl+Yqwc"
             "wGqmoOwgqQSByVBrADgEVHlhS9J2tJQNMQ=="
         )
         test_ec_cert = load_der_x509_certificate(test_ec_cert_bytes, backend=default_backend())
-        new_ec_pubkey = pubkey_from_tpm2b_public(correct_ec_obj)
+        new_ec_pubkey, name_alg = pubkey_parms_from_tpm2b_public(correct_ec_obj)
         assert isinstance(new_ec_pubkey, ec.EllipticCurvePublicKey)
+        self.assertEqual(name_alg, TPM_ALG_SHA256)
 
         correct_ec_pubkey = test_ec_cert.public_key()
         assert isinstance(correct_ec_pubkey, ec.EllipticCurvePublicKey)
         new_ec_pubkey_n = new_ec_pubkey.public_numbers()
         correct_ec_pubkey_n = correct_ec_pubkey.public_numbers()
         self.assertEqual(new_ec_pubkey_n.curve.name, correct_ec_pubkey_n.curve.name)
         self.assertEqual(new_ec_pubkey_n.x, correct_ec_pubkey_n.x)
@@ -301,10 +311,24 @@
             self.assertEqual(
                 val,
                 "fixed-tpm | st-clear | fixed-parent | sensitive-data-origin | "
                 "user-with-auth | admin-with-policy | no-da | "
                 "encrypted-duplication | restricted | decrypt | sign-encrypt",
             )
 
+    def test_unmarshal_tpms_attest(self) -> None:
+        tpms_attest = base64.b64decode(
+            "/1RDR4AYACIACzi1x2WoenP+buZXpt2LdpW0GTj5lBE6PXQmPZ0upQM0ABRBaTVNNVNqWWpua3l2"
+            "NFA3aXRIMQAAAABMlE7mAAAAAwAAAAABIBkQIwAWNjYAAAABAAsDAAABACBtTTdJEy9iVxchZM1f"
+            "8xNfRHlz1KXITgGJAfZ1NwW3AQ=="
+        )
+        retDict = unmarshal_tpms_attest(tpms_attest)
+        self.assertEqual(retDict["clockInfo"], {"clock": 1284787942, "resetCount": 3, "restartCount": 0, "safe": 1})
+        self.assertEqual(retDict["extraData"].hex(), "4169354d35536a596a6e6b797634503769744831")
+        self.assertEqual(
+            retDict["attested.quote.pcrDigest"].hex(),
+            "6d4d3749132f6257172164cd5ff3135f447973d4a5c84e018901f6753705b701",
+        )
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `keylime-7.0.0/keylime/tpm/tpm_main.py` & `keylime-7.2.5/keylime/tpm/tpm_main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 import base64
 import binascii
-import codecs
 import hashlib
-import os
 import re
 import sys
 import tempfile
 import threading
-import time
 import typing
 import zlib
-from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
+from typing import Any, Dict, List, Optional, Sequence, Set, Tuple, Union
 
 from cryptography.hazmat.primitives import serialization as crypto_serialization
 from packaging.version import Version
 
-from keylime import cert_utils, cmd_exec, config, keylime_logging
+from keylime import cert_utils, cmd_exec, config, json, keylime_logging
 from keylime.agentstates import AgentAttestState, TPMClockInfo
-from keylime.common import algorithms, retry
+from keylime.common import algorithms
 from keylime.common.algorithms import Hash
-from keylime.elchecking.policies import RefState
 from keylime.failure import Component, Failure
 from keylime.ima import ima
 from keylime.ima.file_signatures import ImaKeyrings
 from keylime.ima.types import RuntimePolicyType
-from keylime.tpm import tpm2_objects, tpm_abstract
+from keylime.mba import mba
+from keylime.tpm import tpm2_objects, tpm_abstract, tpm_util
 
 logger = keylime_logging.init_logging("tpm")
 
+EXIT_SUCCESS: int = 0
 
-class tpm(tpm_abstract.AbstractTPM):
+
+class Tpm:
     tools_version: str = ""
 
     tpmutilLock: threading.Lock
 
     def __init__(self) -> None:
         super().__init__()
         # Shared lock to serialize access to tools
@@ -43,15 +42,15 @@
 
     def __get_tpm2_tools(self) -> None:
         retDict = self.__run(["tpm2_startup", "--version"])
 
         code = retDict["code"]
         output = "".join(config.convert(retDict["retout"]))
         errout = "".join(config.convert(retDict["reterr"]))
-        if code != tpm_abstract.AbstractTPM.EXIT_SUCESS:
+        if code != EXIT_SUCCESS:
             raise Exception(
                 "Error establishing tpm2-tools version using TPM2_Startup: %s" + str(code) + ": " + str(errout)
             )
 
         # Extract the `version="x.x.x"` from tools
         version_str_ = re.search(r'version="([^"]+)"', output)
         if version_str_ is None:
@@ -80,197 +79,78 @@
         elif Version(tools_version[0]) >= Version("3.2.0"):
             logger.info("TPM2-TOOLS Version: %s", tools_version[0])
             self.tools_version = "3.2"
         else:
             logger.error("TPM2-TOOLS Version %s is not supported.", tools_version[0])
             sys.exit()
 
-    def run(self, cmd: Sequence[str]) -> cmd_exec.RetDictType:
-        return self.__run(cmd, lock=False)
-
     def __run(
         self,
         cmd: Sequence[str],
-        expectedcode: int = tpm_abstract.AbstractTPM.EXIT_SUCESS,
-        raiseOnError: bool = True,
         lock: bool = True,
-        outputpaths: Optional[Union[List[str], str]] = None,
     ) -> cmd_exec.RetDictType:
-        # Convert single outputpath to list
-        if isinstance(outputpaths, str):
-            outputpaths = [outputpaths]
-
-        numtries = 0
-        while True:
-            if lock:
-                with self.tpmutilLock:
-                    retDict = cmd_exec.run(
-                        cmd=cmd, expectedcode=expectedcode, raiseOnError=False, outputpaths=outputpaths
-                    )
-            else:
-                retDict = cmd_exec.run(cmd=cmd, expectedcode=expectedcode, raiseOnError=False, outputpaths=outputpaths)
-            code = retDict["code"]
-            retout = retDict["retout"]
-            reterr = retDict["reterr"]
-
-            # keep trying to get quote if a PCR race condition occurred in quote
-            if cmd[0] == "tpm2_quote" and cmd_exec.list_contains_substring(
-                reterr, "Error validating calculated PCR composite with quote"
-            ):
-                numtries += 1
-                maxr = config.getint("agent", "max_retries")
-                if numtries >= maxr:
-                    logger.error("Agent did not return proper quote due to PCR race condition.")
-                    break
-                interval = config.getfloat("agent", "retry_interval")
-                exponential_backoff = config.getboolean("agent", "exponential_backoff")
-                next_retry = retry.retry_time(exponential_backoff, interval, numtries, logger)
-                logger.info(
-                    "Failed to get quote %d/%d times, trying again in %f seconds...", numtries, maxr, next_retry
-                )
-                time.sleep(next_retry)
-                continue
-
-            break
+        if lock:
+            with self.tpmutilLock:
+                retDict = cmd_exec.run(cmd=cmd, expectedcode=EXIT_SUCCESS, raiseOnError=False)
+        else:
+            retDict = cmd_exec.run(cmd=cmd, expectedcode=EXIT_SUCCESS, raiseOnError=False)
+        code = retDict["code"]
+        retout = retDict["retout"]
+        reterr = retDict["reterr"]
 
         # Don't bother continuing if TPM call failed and we're raising on error
-        if code != expectedcode and raiseOnError:
+        if code != EXIT_SUCCESS:
             raise Exception(
-                f"Command: {cmd} returned {code}, expected {expectedcode}, output {retout}, stderr {reterr}"
+                f"Command: {cmd} returned {code}, expected {EXIT_SUCCESS}, output {retout}, stderr {reterr}"
             )
 
         return retDict
 
-    def encryptAIK(self, uuid: str, ek_tpm: bytes, aik_tpm: bytes) -> Optional[Tuple[bytes, str]]:
+    @staticmethod
+    def encryptAIK(uuid: str, ek_tpm: bytes, aik_tpm: bytes) -> Optional[Tuple[bytes, str]]:
         if ek_tpm is None or aik_tpm is None:
             logger.error("Missing parameters for encryptAIK")
             return None
 
         aik_name = tpm2_objects.get_tpm2b_public_name(aik_tpm)
 
-        efd = keyfd = blobfd = -1
-        ekFile = None
-        challengeFile = None
-        keyblob = None
-        blobpath = None
-
         try:
-            # write out the public EK
-            efd, etemp = tempfile.mkstemp()
-            with open(etemp, "wb") as ekFile:
-                ekFile.write(ek_tpm)
-
             # write out the challenge
             challenge_str = tpm_abstract.TPM_Utilities.random_password(32)
             challenge = challenge_str.encode()
-            keyfd, keypath = tempfile.mkstemp()
-            with open(keypath, "wb") as challengeFile:
-                challengeFile.write(challenge)
-
-            # create temp file for the blob
-            blobfd, blobpath = tempfile.mkstemp()
-            command = [
-                "tpm2_makecredential",
-                "-T",
-                "none",
-                "-e",
-                ekFile.name,
-                "-s",
-                challengeFile.name,
-                "-n",
-                aik_name,
-                "-o",
-                blobpath,
-            ]
-            self.__run(command, lock=False)
 
             logger.info("Encrypting AIK for UUID %s", uuid)
 
-            # read in the blob
-            with open(blobpath, "rb") as f:
-                keyblob = base64.b64encode(f.read())
-
             # read in the aes key
             key = base64.b64encode(challenge).decode("utf-8")
 
+            credentialblob = tpm_util.makecredential(ek_tpm, challenge, bytes.fromhex(aik_name))
+            keyblob = base64.b64encode(credentialblob)
+
         except Exception as e:
             logger.error("Error encrypting AIK: %s", str(e))
             logger.exception(e)
             raise
-        finally:
-            for fd in [efd, keyfd, blobfd]:
-                if fd >= 0:
-                    os.close(fd)
-            for fi in [ekFile, challengeFile]:
-                if fi is not None:
-                    os.remove(fi.name)
-            if blobpath is not None:
-                os.remove(blobpath)
 
         return (keyblob, key)
 
-    def verify_ek(self, ekcert: bytes, tpm_cert_store: str) -> bool:
+    @staticmethod
+    def verify_ek(ekcert: bytes, tpm_cert_store: str) -> bool:
         """Verify that the provided EK certificate is signed by a trusted root
         :param ekcert: The Endorsement Key certificate in DER format
         :returns: True if the certificate can be verified, false otherwise
         """
         return cert_utils.verify_ek(ekcert, tpm_cert_store)
 
-    # tpm_quote
-    def __tpm2_checkquote(
-        self, pubaik: str, nonce: str, quoteFile: str, sigFile: str, pcrFile: str, hash_alg: Union[Hash, str]
-    ) -> cmd_exec.RetDictType:
-        nonce = bytes(nonce, encoding="utf8").hex()
-        if self.tools_version == "3.2":
-            command = [
-                "tpm2_checkquote",
-                "-c",
-                pubaik,
-                "-m",
-                quoteFile,
-                "-s",
-                sigFile,
-                "-p",
-                pcrFile,
-                "-G",
-                hash_alg,
-                "-q",
-                nonce,
-            ]
-        else:
-            # versions >= 4.0
-            command = [
-                "tpm2_checkquote",
-                "-u",
-                pubaik,
-                "-m",
-                quoteFile,
-                "-s",
-                sigFile,
-                "-f",
-                pcrFile,
-                "-g",
-                hash_alg,
-                "-q",
-                nonce,
-            ]
-
-        retDict = self.__run(command, lock=False)
-        return retDict
-
-    def __tpm2_printquote(self, quoteFile: str) -> cmd_exec.RetDictType:
-        command = ["tpm2_print", "-t", "TPMS_ATTEST", quoteFile]
-        retDict = self.__run(command, lock=False)
-        return retDict
-
-    def _tpm2_printquote(self, quote: str, compressed: bool) -> Tuple[Optional[List[bytes]], bool]:
+    @staticmethod
+    def _tpm2_clock_info_from_quote(quote: str, compressed: bool) -> Dict[str, Any]:
         """Get TPM timestamp info from quote
         :param quote: quote data in the format 'r<b64-compressed-quoteblob>:<b64-compressed-sigblob>:<b64-compressed-pcrblob>
         :param compressed: if the quote data is compressed with zlib or not
-        :returns: Returns the 'retout' from running tpm2_print and True in case of success, None and False in case of error.
+        :returns: Returns a dict holding the TPMS_CLOCK_INFO fields
         This function throws an Exception on bad input.
         """
 
         if quote[0] != "r":
             raise Exception(f"Invalid quote type {quote[0]}")
         quote = quote[1:]
 
@@ -280,48 +160,25 @@
 
         quoteblob = base64.b64decode(quote_tokens[0])
 
         if compressed:
             logger.warning("Decompressing quote data which is unsafe!")
             quoteblob = zlib.decompress(quoteblob)
 
-        qfd = -1
-        quoteFile = None
-
         try:
-            # write out quote
-            qfd, qtemp = tempfile.mkstemp()
-            with open(qtemp, "wb") as quoteFile:
-                quoteFile.write(quoteblob)
-
-            retDict = self.__tpm2_printquote(quoteFile.name)
-            retout = retDict["retout"]
-            reterr = retDict["reterr"]
-            code = retDict["code"]
+            return tpm2_objects.get_tpms_attest_clock_info(quoteblob)
         except Exception as e:
-            logger.error("Error printing quote: %s", str(e))
+            logger.error("Error extracting clock info from quote: %s", str(e))
             logger.exception(e)
-            return None, False
-        finally:
-            for fd in [qfd]:
-                if fd >= 0:
-                    os.close(fd)
-            for fi in [quoteFile]:
-                if fi is not None:
-                    os.remove(fi.name)
-
-        if len(retout) < 1 or code != tpm_abstract.AbstractTPM.EXIT_SUCESS:
-            logger.error("Failed to print quote info, output: %s", reterr)
-            return None, False
-
-        return retout, True
+            return {}
 
+    @staticmethod
     def _tpm2_checkquote(
-        self, aikTpmFromRegistrar: str, quote: str, nonce: str, hash_alg: Union[Hash, str], compressed: bool
-    ) -> Tuple[Optional[List[bytes]], bool]:
+        aikTpmFromRegistrar: str, quote: str, nonce: str, hash_alg: str, compressed: bool
+    ) -> Tuple[Dict[int, str], str]:
         """Write the files from data returned from tpm2_quote for running tpm2_checkquote
         :param aikTpmFromRegistrar: AIK used to generate the quote and is needed for verifying it now.
         :param quote: quote data in the format 'r<b64-compressed-quoteblob>:<b64-compressed-sigblob>:<b64-compressed-pcrblob>
         :param nonce: nonce that was used to create the quote
         :param hash_alg: the hash algorithm that was used
         :param compressed: if the quote data is compressed with zlib or not
         :returns: Returns the 'retout' from running tpm2_checkquote and True in case of success, None and False in case of error.
@@ -348,61 +205,251 @@
 
         if compressed:
             logger.warning("Decompressing quote data which is unsafe!")
             quoteblob = zlib.decompress(quoteblob)
             sigblob = zlib.decompress(sigblob)
             pcrblob = zlib.decompress(pcrblob)
 
-        qfd = sfd = pfd = afd = -1
-        quoteFile = None
-        aikFile = None
-        sigFile = None
-        pcrFile = None
-
         try:
-            # write out quote
-            qfd, qtemp = tempfile.mkstemp()
-            with open(qtemp, "wb") as quoteFile:
-                quoteFile.write(quoteblob)
-
-            # write out sig
-            sfd, stemp = tempfile.mkstemp()
-            with open(stemp, "wb") as sigFile:
-                sigFile.write(sigblob)
-
-            # write out pcr
-            pfd, ptemp = tempfile.mkstemp()
-            with open(ptemp, "wb") as pcrFile:
-                pcrFile.write(pcrblob)
-
-            afd, atemp = tempfile.mkstemp()
-            with open(atemp, "wb") as aikFile:
-                aikFile.write(aikFromRegistrar)
-
-            retDict = self.__tpm2_checkquote(aikFile.name, nonce, quoteFile.name, sigFile.name, pcrFile.name, hash_alg)
-            retout = retDict["retout"]
-            reterr = retDict["reterr"]
-            code = retDict["code"]
+            pcrs_dict = tpm_util.checkquote(aikFromRegistrar, nonce, sigblob, quoteblob, pcrblob, hash_alg)
         except Exception as e:
             logger.error("Error verifying quote: %s", str(e))
             logger.exception(e)
-            return None, False
-        finally:
-            for fd in [qfd, sfd, pfd, afd]:
-                if fd >= 0:
-                    os.close(fd)
-            for fi in [aikFile, quoteFile, sigFile, pcrFile]:
-                if fi is not None:
-                    os.remove(fi.name)
-
-        if len(retout) < 1 or code != tpm_abstract.AbstractTPM.EXIT_SUCESS:
-            logger.error("Failed to validate signature, output: %s", reterr)
-            return None, False
+            return {}, str(e)
+
+        return pcrs_dict, ""
 
-        return retout, True
+    @staticmethod
+    def __check_ima(
+        agentAttestState: AgentAttestState,
+        pcrval: str,
+        ima_measurement_list: str,
+        runtime_policy: Optional[RuntimePolicyType],
+        ima_keyrings: Optional[ImaKeyrings],
+        boot_aggregates: Optional[Dict[str, List[str]]],
+        hash_alg: Hash,
+    ) -> Failure:
+        failure = Failure(Component.IMA)
+        logger.info("Checking IMA measurement list on agent: %s", agentAttestState.get_agent_id())
+        _, ima_failure = ima.process_measurement_list(
+            agentAttestState,
+            ima_measurement_list.split("\n"),
+            runtime_policy,
+            pcrval=pcrval,
+            ima_keyrings=ima_keyrings,
+            boot_aggregates=boot_aggregates,
+            hash_alg=hash_alg,
+        )
+        failure.merge(ima_failure)
+        if not failure:
+            logger.debug("IMA measurement list of agent %s validated", agentAttestState.get_agent_id())
+        return failure
+
+    def check_pcrs(
+        self,
+        agentAttestState: AgentAttestState,
+        tpm_policy: Union[str, Dict[str, Any]],
+        pcrs_dict: Dict[int, str],
+        data: str,
+        ima_measurement_list: Optional[str],
+        runtime_policy: Optional[RuntimePolicyType],
+        ima_keyrings: Optional[ImaKeyrings],
+        mb_measurement_list: Optional[str],
+        mb_refstate: Optional[str],
+        hash_alg: Hash,
+    ) -> Failure:
+        failure = Failure(Component.PCR_VALIDATION)
+
+        agent_id = agentAttestState.get_agent_id()
+
+        if isinstance(tpm_policy, str):
+            tpm_policy_dict = json.loads(tpm_policy)
+        else:
+            tpm_policy_dict = tpm_policy
+
+        pcr_allowlist = tpm_policy_dict.copy()
+
+        if "mask" in pcr_allowlist:
+            del pcr_allowlist["mask"]
+        # convert all pcr num keys to integers
+        pcr_allowlist = {int(k): v for k, v in list(pcr_allowlist.items())}
+
+        # temporary: to avoid a CI failure, we don't attempt to evaluate
+        # boot logs when the policy is empty. This is because the CI
+        # system currently cannot simulate MBA correctly.
+        # we parse mb_refstate here to figure out whether it's empty.
+        if not mb_refstate:
+            mb_refstate_data = None
+        else:
+            mb_refstate_data = json.loads(mb_refstate)
+
+        mb_pcrs_hashes, boot_aggregates, mb_measurement_data, mb_failure = self.parse_mb_bootlog(
+            mb_measurement_list, hash_alg
+        )
+        failure.merge(mb_failure)
+
+        pcrs_in_quote: Set[int] = set()  # PCRs in quote that were already used for some kind of validation
+
+        pcr_nums = set(pcrs_dict.keys())
+
+        # Validate data PCR
+        if config.TPM_DATA_PCR in pcr_nums and data is not None:
+            expectedval = self.sim_extend(data, hash_alg)
+            if expectedval != pcrs_dict[config.TPM_DATA_PCR]:
+                logger.error(
+                    "PCR #%s: invalid bind data %s from quote (from agent %s) does not match expected value %s",
+                    config.TPM_DATA_PCR,
+                    pcrs_dict[config.TPM_DATA_PCR],
+                    agent_id,
+                    expectedval,
+                )
+                failure.add_event(
+                    f"invalid_pcr_{config.TPM_DATA_PCR}",
+                    {"got": pcrs_dict[config.TPM_DATA_PCR], "expected": expectedval},
+                    True,
+                )
+            pcrs_in_quote.add(config.TPM_DATA_PCR)
+        else:
+            logger.error(
+                "Binding PCR #%s was not included in the quote (from agent %s), but is required",
+                config.TPM_DATA_PCR,
+                agent_id,
+            )
+            failure.add_event(
+                f"missing_pcr_{config.TPM_DATA_PCR}",
+                f"Data PCR {config.TPM_DATA_PCR} is missing in quote, but is required",
+                True,
+            )
+        # Check for ima PCR
+        if config.IMA_PCR in pcr_nums:
+            if ima_measurement_list is None:
+                logger.error("IMA PCR in policy, but no measurement list provided by agent %s", agent_id)
+                failure.add_event(
+                    f"unused_pcr_{config.IMA_PCR}", "IMA PCR in policy, but no measurement list provided", True
+                )
+            else:
+                ima_failure = Tpm.__check_ima(
+                    agentAttestState,
+                    pcrs_dict[config.IMA_PCR],
+                    ima_measurement_list,
+                    runtime_policy,
+                    ima_keyrings,
+                    boot_aggregates,
+                    hash_alg,
+                )
+                failure.merge(ima_failure)
+
+            pcrs_in_quote.add(config.IMA_PCR)
+
+        # Collect mismatched measured boot PCRs as measured_boot failures
+        mb_pcr_failure = Failure(Component.MEASURED_BOOT)
+        # Handle measured boot PCRs only if the parsing worked
+        if not mb_failure:
+            for pcr_num in set(config.MEASUREDBOOT_PCRS) & pcr_nums:
+                if mb_refstate_data:
+                    if not mb_measurement_list:
+                        logger.error(
+                            "Measured Boot PCR %d in policy, but no measurement list provided by agent %s",
+                            pcr_num,
+                            agent_id,
+                        )
+                        failure.add_event(
+                            f"unused_pcr_{pcr_num}",
+                            f"Measured Boot PCR {pcr_num} in policy, but no measurement list provided",
+                            True,
+                        )
+                        continue
+
+                    val_from_log_int = mb_pcrs_hashes.get(str(pcr_num), 0)
+                    val_from_log_hex = hex(val_from_log_int)[2:]
+                    val_from_log_hex_stripped = val_from_log_hex.lstrip("0")
+                    pcrval_stripped = pcrs_dict[pcr_num].lstrip("0")
+                    if val_from_log_hex_stripped != pcrval_stripped:
+                        logger.error(
+                            "For PCR %d and hash %s the boot event log has value %r but the agent %s returned %r",
+                            pcr_num,
+                            str(hash_alg),
+                            val_from_log_hex,
+                            agent_id,
+                            pcrs_dict[pcr_num],
+                        )
+                        mb_pcr_failure.add_event(
+                            f"invalid_pcr_{pcr_num}",
+                            {
+                                "context": "SHA256 boot event log PCR value does not match",
+                                "got": pcrs_dict[pcr_num],
+                                "expected": val_from_log_hex,
+                            },
+                            True,
+                        )
+
+                    if pcr_num in pcr_allowlist and pcrs_dict[pcr_num] not in pcr_allowlist[pcr_num]:
+                        logger.error(
+                            "PCR #%s: %s from quote (from agent %s) does not match expected value %s",
+                            pcr_num,
+                            pcrs_dict[pcr_num],
+                            agent_id,
+                            pcr_allowlist[pcr_num],
+                        )
+                        failure.add_event(
+                            f"invalid_pcr_{pcr_num}",
+                            {
+                                "context": "PCR value is not in allowlist",
+                                "got": pcrs_dict[pcr_num],
+                                "expected": pcr_allowlist[pcr_num],
+                            },
+                            True,
+                        )
+                    pcrs_in_quote.add(pcr_num)
+        failure.merge(mb_pcr_failure)
+
+        # Check the remaining non validated PCRs
+        for pcr_num in pcr_nums - pcrs_in_quote:
+            if pcr_num not in list(pcr_allowlist.keys()):
+                logger.warning(
+                    "PCR #%s in quote (from agent %s) not found in tpm_policy, skipping.",
+                    pcr_num,
+                    agent_id,
+                )
+                continue
+            if pcrs_dict[pcr_num] not in pcr_allowlist[pcr_num]:
+                logger.error(
+                    "PCR #%s: %s from quote (from agent %s) does not match expected value %s",
+                    pcr_num,
+                    pcrs_dict[pcr_num],
+                    agent_id,
+                    pcr_allowlist[pcr_num],
+                )
+                failure.add_event(
+                    f"invalid_pcr_{pcr_num}",
+                    {
+                        "context": "PCR value is not in allowlist",
+                        "got": pcrs_dict[pcr_num],
+                        "expected": pcr_allowlist[pcr_num],
+                    },
+                    True,
+                )
+
+            pcrs_in_quote.add(pcr_num)
+
+        missing = set(pcr_allowlist.keys()) - pcrs_in_quote
+        if len(missing) > 0:
+            logger.error("PCRs specified in policy not in quote (from agent %s): %s", agent_id, missing)
+            failure.add_event("missing_pcrs", {"context": "PCRs are missing in quote", "data": list(missing)}, True)
+
+        if not mb_failure and mb_refstate_data:
+            mb_policy_failure = mba.evaluate_bootlog(
+                mb_refstate,
+                mb_measurement_data,
+                pcrs_in_quote,
+                agentAttestState.get_agent_id(),
+            )
+            failure.merge(mb_policy_failure)
+
+        return failure
 
     def check_quote(
         self,
         agentAttestState: AgentAttestState,
         nonce: str,
         data: str,
         quote: str,
@@ -418,96 +465,73 @@
     ) -> Failure:
         if tpm_policy is None:
             tpm_policy = {}
 
         if runtime_policy is None:
             runtime_policy = ima.EMPTY_RUNTIME_POLICY
 
-        agent_id = agentAttestState.agent_id
-
         failure = Failure(Component.QUOTE_VALIDATION)
         if hash_alg is None:
             failure.add_event("hash_alg_missing", "Hash algorithm cannot be empty", False)
             return failure
 
         # First and foremost, the quote needs to be validated
-        retout, success = self._tpm2_checkquote(aikTpmFromRegistrar, quote, nonce, hash_alg, compressed)
-        if not success:
+        pcrs_dict, err = Tpm._tpm2_checkquote(aikTpmFromRegistrar, quote, nonce, str(hash_alg), compressed)
+        if err:
             # If the quote validation fails we will skip all other steps therefore this failure is irrecoverable.
-            failure.add_event(
-                "quote_validation", {"message": "Quote data validation using tpm2-tools", "data": retout}, False
-            )
+            failure.add_event("quote_validation", {"message": "Quote data validation", "error": err}, False)
             return failure
 
         # Only after validating the quote, the TPM clock information can be extracted from it.
-        clock_failure, current_clock_info = self.check_quote_timing(
+        clock_failure, current_clock_info = Tpm.check_quote_timing(
             agentAttestState.get_tpm_clockinfo(), quote, compressed
         )
         if clock_failure:
             failure.add_event(
                 "quote_validation",
                 {"message": "Validation of clockinfo from quote using tpm2-tools", "data": clock_failure},
                 False,
             )
             return failure
         if current_clock_info:
             agentAttestState.set_tpm_clockinfo(current_clock_info)
 
-        pcrs = []
-        jsonout = config.yaml_to_dict(retout, logger=logger)
-        if jsonout is None:
-            failure.add_event(
-                "quote_validation",
-                {"message": "YAML parsing failed for quote validation using tpm2-tools.", "data": retout},
-                False,
-            )
-            return failure
-        if "pcrs" in jsonout:
-            # The hash algorithm might be in the YAML output but does not contain any data, so we also check that.
-            if hash_alg in jsonout["pcrs"] and jsonout["pcrs"][hash_alg] is not None:
-                alg_size = hash_alg.get_size() // 4
-                for pcrval, hashval in jsonout["pcrs"][hash_alg].items():
-                    pcrs.append(f"PCR {pcrval} {hashval:0{alg_size}x}")
-
-        if len(pcrs) == 0:
+        if len(pcrs_dict) == 0:
             logger.warning(
                 "Quote for agent %s does not contain any PCRs. Make sure that the TPM supports %s PCR banks",
-                agent_id,
+                agentAttestState.agent_id,
                 str(hash_alg),
             )
 
         return self.check_pcrs(
             agentAttestState,
             tpm_policy,
-            pcrs,
+            pcrs_dict,
             data,
             ima_measurement_list,
             runtime_policy,
             ima_keyrings,
             mb_measurement_list,
             mb_refstate,
             hash_alg,
         )
 
+    @staticmethod
     def check_quote_timing(
-        self, previous_clockinfo: TPMClockInfo, quote: str, compressed: bool
+        previous_clockinfo: TPMClockInfo, quote: str, compressed: bool
     ) -> Tuple[Optional[str], Optional[TPMClockInfo]]:
         # Sanity check quote clock information
 
         current_clockinfo = None
 
-        retout, success = self._tpm2_printquote(quote, compressed)
-        if not success:
-            return "tpm2_print failed with " + str(retout), current_clockinfo
-
-        tpm_data_str_dict = config.yaml_to_dict(retout, add_newlines=False, logger=logger)
-        if tpm_data_str_dict is None:
-            return "yaml output of tpm2_print could not be parsed!", current_clockinfo
+        clock_info_dict = Tpm._tpm2_clock_info_from_quote(quote, compressed)
+        if not clock_info_dict:
+            return "_tpm2_clock_info_from_quote failed ", current_clockinfo
 
-        tentative_current_clockinfo = TPMClockInfo.from_dict(tpm_data_str_dict)
+        tentative_current_clockinfo = TPMClockInfo.from_dict(clock_info_dict)
 
         resetdiff = tentative_current_clockinfo.resetcount - previous_clockinfo.resetcount
         restartdiff = tentative_current_clockinfo.restartcount - previous_clockinfo.restartcount
 
         if resetdiff < 0:
             return "resetCount value decreased on TPM between two consecutive quotes", current_clockinfo
 
@@ -524,26 +548,20 @@
                     current_clockinfo,
                 )
 
             current_clockinfo = tentative_current_clockinfo
 
         return None, current_clockinfo
 
-    def sim_extend(self, hashval_1: str, hash_alg: Hash) -> str:
-        hashval_0 = self.START_HASH(hash_alg)
-
-        # compute expected value  H(0|H(data))
-        hdata = self.hashdigest(hashval_1.encode("utf-8"), hash_alg)
-        assert hdata is not None
-        hext = self.hashdigest(
-            codecs.decode(hashval_0, "hex_codec") + codecs.decode(hdata, "hex_codec"),
-            hash_alg,
-        )
-        assert hext is not None
-        return hext.lower()
+    @staticmethod
+    def sim_extend(hashval_1: str, hash_alg: Hash) -> str:
+        """Compute expected value  H(0|H(data))"""
+        hdata = hash_alg.hash(hashval_1.encode("utf-8"))
+        hext = hash_alg.hash(hash_alg.get_start_hash() + hdata)
+        return hext.hex()
 
     @staticmethod
     def __stringify_pcr_keys(log: Dict[str, Dict[str, Dict[str, str]]]) -> None:
         """Ensure that the PCR indices are strings
 
         The YAML produced by `tpm2_eventlog`, when loaded by the yaml module,
         uses integer keys in the dicts holding PCR contents.  That does not
@@ -600,15 +618,15 @@
         """
         Newer versions of tpm2-tools escapes the YAML output and including the trailing null byte.
         See: https://github.com/tpm2-software/tpm2-tools/commit/c78d258b2588aee535fd17594ad2f5e808056373
         This converts it back to an unescaped string.
         Example:
             '"MokList\\0"' -> 'MokList'
         """
-        if tpm.tools_version in ["3.2", "4.0", "4.2"]:
+        if Tpm.tools_version in ["3.2", "4.0", "4.2"]:
             return
 
         escaped_chars = [
             ("\0", "\\0"),
             ("\a", "\\a"),
             ("\b", "\\b"),
             ("\t", "\\t"),
@@ -673,17 +691,17 @@
                 "bootlog_enrich",
                 f"Could not load tpm_bootlog_enrich (which depends on {config.LIBEFIVAR}): {str(e)}",
                 True,
             )
             return failure, None
         # pylint: enable=import-outside-toplevel
         tpm_bootlog_enrich.enrich(log_parsed_data)
-        tpm.__stringify_pcr_keys(log_parsed_data)
-        tpm.__add_boot_aggregate(log_parsed_data)
-        tpm.__unescape_eventlog(log_parsed_data)
+        Tpm.__stringify_pcr_keys(log_parsed_data)
+        Tpm.__add_boot_aggregate(log_parsed_data)
+        Tpm.__unescape_eventlog(log_parsed_data)
         return failure, log_parsed_data
 
     def _parse_mb_bootlog(self, log_b64: str) -> typing.Tuple[Failure, typing.Optional[Dict[str, Any]]]:
         """Parse and enrich a BIOS boot log
 
         The input is the base64 encoding of a binary log.
         The output is the result of parsing and applying other conveniences."""
@@ -697,15 +715,15 @@
         except binascii.Error:
             failure.add_event("log.base64decode", "Measured boot log could not be decoded", True)
             result = None
         return failure, result
 
     def parse_mb_bootlog(
         self, mb_measurement_list: Optional[str], hash_alg: algorithms.Hash
-    ) -> typing.Tuple[Dict[str, int], typing.Optional[Dict[str, List[str]]], RefState, Failure]:
+    ) -> typing.Tuple[Dict[str, int], typing.Optional[Dict[str, List[str]]], Dict[str, Any], Failure]:
         """Parse the measured boot log and return its object and the state of the PCRs
         :param mb_measurement_list: The measured boot measurement list
         :param hash_alg: the hash algorithm that should be used for the PCRs
         :returns: Returns a map of the state of the PCRs, measured boot data object and True for success
                   and False in case an error occurred
         """
         failure = Failure(Component.MEASURED_BOOT, ["parser"])
```

### Comparing `keylime-7.0.0/keylime/tpm_bootlog_enrich.py` & `keylime-7.2.5/keylime/tpm_bootlog_enrich.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/keylime/web_util.py` & `keylime-7.2.5/keylime/web_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,18 +121,16 @@
                 if client_key_pw:
                     client_key_pw = str(client_key_pw)
                 ca_util.cmd_mkcert(tls_dir, "client", password=client_key_pw)
 
     elif tls_dir == "default":
         # Use the keys/certificates generated for the verifier
         tls_dir = os.path.abspath(os.path.join(config.WORK_DIR, "cv_ca"))
-        if not os.path.exists(os.path.join(tls_dir, "cacert.crt")):
-            raise Exception(
-                "It appears that the verifier has not yet created a CA and certificates, please run the verifier first"
-            )
+        if not os.path.exists(tls_dir):
+            raise Exception(f"It appears that the specified tls_dir does not exist: {tls_dir}")
     else:
         # if it is relative path, convert to absolute in WORK_DIR
         tls_dir = os.path.abspath(os.path.join(config.WORK_DIR, tls_dir))
 
     return tls_dir
```

### Comparing `keylime-7.0.0/keylime.egg-info/PKG-INFO` & `keylime-7.2.5/keylime.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keylime
-Version: 7.0.0
+Version: 7.2.5
 Summary: TPM-based key bootstrapping and system integrity measurement system for cloud
 Home-page: https://keylime.dev
 Author: Keylime Community
 Author-email: keylime@groups.io
 License: Apache-2.0
 Project-URL: Source, https://github.com/keylime/keylime
 Project-URL: Documentation, https://keylime.readthedocs.io/en/latest/
@@ -178,15 +178,15 @@
 ## Systemd service support
 
 The directory `services/` includes `systemd` service files for the verifier,
 agent and registrar.
 
 You can install the services with the following command:
 
-`sudo ./services/install.sh`
+`sudo ./services/installer.sh`
 
 Once installed, you can run and inspect the services `keylime_verifier` and `keylime_registrar` via `systemctl`.
 The Rust agent repository also contains a systemd service file for the agent.
 
 ## Request a feature
 
 Keylime feature requests are tracked as enhancements in the [enhancements repository](https://github.com/keylime/enhancements)
@@ -233,15 +233,15 @@
 * Executive summary Keylime slides: [docs/old/keylime-elevator-slides.pptx](https://github.com/keylime/keylime/raw/master/docs/old/keylime-elevator-slides.pptx)
 * Detailed Keylime Architecture slides: [docs/old/keylime-detailed-architecture-v7.pptx](https://github.com/keylime/keylime/raw/master/docs/old/keylime-detailed-architecture-v7.pptx)
 * See ACSAC 2016 paper in doc directory: [docs/old/tci-acm.pdf](https://github.com/keylime/keylime/blob/master/docs/old/tci-acm.pdf)
   * and the ACSAC presentation on Keylime: [docs/old/llsrc-keylime-acsac-v6.pptx](https://github.com/keylime/keylime/raw/master/docs/old/llsrc-keylime-acsac-v6.pptx)
 * See the HotCloud 2018 paper: [docs/old/hotcloud18.pdf](https://github.com/keylime/keylime/blob/master/docs/old/hotcloud18.pdf)
 * Details about Keylime REST API: [docs/old/keylime RESTful API.docx](https://github.com/keylime/keylime/raw/master/docs/old/keylime%20RESTful%20API.docx)
 * [Demo files](demo/) - Some pre-packaged demos to show off what Keylime can do.
-* [IMA stub service](ima_stub_service/) - Allows you to test IMA and Keylime on a machine without a TPM.  Service keeps emulated TPM synchronized with IMA.
+* [IMA stub service](https://github.com/keylime/rust-keylime/tree/master/keylime-ima-emulator) - Allows you to test IMA and Keylime on a machine without a TPM.  Service keeps emulated TPM synchronized with IMA.
 
 #### Errata from the ACSAC Paper
 
 We discovered a typo in Figure 5 of the published ACSAC paper. The final interaction
 between the Tenant and Cloud Verifier showed an HMAC of the node's ID using the key
 K_e.  This should be using K_b. The paper in this repository and the ACSAC presentation
 have been updated to correct this typo.
```

### Comparing `keylime-7.0.0/keylime.egg-info/SOURCES.txt` & `keylime-7.2.5/keylime.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 keylime/config.py
 keylime/crypto.py
 keylime/failure.py
 keylime/fs_util.py
 keylime/ip_util.py
 keylime/json.py
 keylime/keylime_logging.py
-keylime/measured_boot.py
 keylime/registrar_client.py
 keylime/registrar_common.py
 keylime/requests_client.py
 keylime/revocation_notifier.py
 keylime/signing.py
 keylime/tenant.py
 keylime/tornado_requests.py
@@ -75,27 +74,30 @@
 keylime/db/keylime_db.py
 keylime/db/registrar_db.py
 keylime/db/verifier_db.py
 keylime/dsse/__init__.py
 keylime/dsse/dsse.py
 keylime/dsse/ecdsa.py
 keylime/dsse/x509.py
-keylime/elchecking/__init__.py
-keylime/elchecking/__main__.py
-keylime/elchecking/example.py
-keylime/elchecking/policies.py
-keylime/elchecking/tests.py
 keylime/ima/__init__.py
 keylime/ima/ast.py
 keylime/ima/dm_grammar.py
 keylime/ima/file_signatures.py
 keylime/ima/ima.py
 keylime/ima/ima_dm.py
 keylime/ima/ima_test.py
 keylime/ima/types.py
+keylime/mba/__init__.py
+keylime/mba/mba.py
+keylime/mba/elchecking/__init__.py
+keylime/mba/elchecking/__main__.py
+keylime/mba/elchecking/example.py
+keylime/mba/elchecking/mbpolicy.py
+keylime/mba/elchecking/policies.py
+keylime/mba/elchecking/tests.py
 keylime/migrations/__init__.py
 keylime/migrations/alembic.ini
 keylime/migrations/env.py
 keylime/migrations/versions/039322ea079b_add_generator_column.py
 keylime/migrations/versions/1ac1513ef2a1_fix_mb_and_ima_column_types.py
 keylime/migrations/versions/257fe0f0c039_add_fields_for_revocation_context_to_.py
 keylime/migrations/versions/2fbc0fb8fa4d_add_checksum_to_allowlist.py
@@ -120,18 +122,22 @@
 keylime/migrations/versions/cc2630851a1f_receive_the_aik_tpm_from_the_agent.py
 keylime/migrations/versions/eb869a77abd1_create_allowlist_table.py
 keylime/migrations/versions/eeb702f77d7d_allowlist_rename.py
 keylime/migrations/versions/f35cdd35eb83_move_v_tpm_policy_to_jsonpickletype.py
 keylime/migrations/versions/f82c4252bc4f_add_ip_and_port_to_registrar.py
 keylime/migrations/versions/f838d3cdeead_add_last_successful_attestation.py
 keylime/tpm/__init__.py
+keylime/tpm/ec_crypto_helper.py
 keylime/tpm/tpm2_objects.py
 keylime/tpm/tpm2_objects_test.py
 keylime/tpm/tpm_abstract.py
 keylime/tpm/tpm_main.py
+keylime/tpm/tpm_util.py
+keylime/tpm/tpm_util_test.py
+keylime/tpm/types.py
 templates/2.0/adjust.py
 templates/2.0/agent.j2
 templates/2.0/ca.j2
 templates/2.0/logging.j2
 templates/2.0/mapping.json
 templates/2.0/registrar.j2
 templates/2.0/tenant.j2
```

### Comparing `keylime-7.0.0/keylime.egg-info/entry_points.txt` & `keylime-7.2.5/keylime.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/pyproject.toml` & `keylime-7.2.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -16,20 +16,17 @@
 profile = "black"
 line_length = 120
 
 [tool.pyright]
 include = ["keylime", "test"]
 ignore = [
     "keylime/backport_dataclasses.py",
-    "keylime/elchecking/",
+    "keylime/mba/elchecking/",
     "keylime/migrations/versions/",
     "keylime/da/examples/tsa_rfc3161.py",
     "keylime/da/examples/sqldb.py",
     "keylime/da/examples/redis.py",
     "keylime/da/examples/file.py",
     "keylime/da/record.py",
-    "test/oldtest.py",
-    "test/test_ima_dm.py",
-    "test/test_restful.py",
     "test/data/template-invalid-adjust/2.0/adjust.py",
 ]
 reportMissingImports = false
```

### Comparing `keylime-7.0.0/setup.cfg` & `keylime-7.2.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = keylime
-version = 7.0.0
+version = 7.2.5
 description = TPM-based key bootstrapping and system integrity measurement system for cloud
 long_description = file: _pypi-notice.md, README.md
 long_description_content_type = text/markdown; charset=UTF-8
 url = https://keylime.dev
 author = Keylime Community
 author_email = keylime@groups.io
 license = Apache-2.0
```

### Comparing `keylime-7.0.0/setup.py` & `keylime-7.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/templates/2.0/adjust.py` & `keylime-7.2.5/templates/2.0/adjust.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/templates/2.0/agent.j2` & `keylime-7.2.5/templates/2.0/agent.j2`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/templates/2.0/ca.j2` & `keylime-7.2.5/templates/2.0/ca.j2`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/templates/2.0/logging.j2` & `keylime-7.2.5/templates/2.0/logging.j2`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/templates/2.0/mapping.json` & `keylime-7.2.5/templates/2.0/mapping.json`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/templates/2.0/registrar.j2` & `keylime-7.2.5/templates/2.0/registrar.j2`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/templates/2.0/tenant.j2` & `keylime-7.2.5/templates/2.0/tenant.j2`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/templates/2.0/verifier.j2` & `keylime-7.2.5/templates/2.0/verifier.j2`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/test/test_algorithms.py` & `keylime-7.2.5/test/test_algorithms.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/test/test_api_version.py` & `keylime-7.2.5/test/test_api_version.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/test/test_ca_impl_openssl.py` & `keylime-7.2.5/test/test_ca_impl_openssl.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/test/test_ca_util.py` & `keylime-7.2.5/test/test_ca_util.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/test/test_cert_utils.py` & `keylime-7.2.5/test/test_cert_utils.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/test/test_config.py` & `keylime-7.2.5/test/test_config.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/test/test_convert_config.py` & `keylime-7.2.5/test/test_convert_config.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/test/test_crypto.py` & `keylime-7.2.5/test/test_crypto.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/test/test_fs_util.py` & `keylime-7.2.5/test/test_fs_util.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/test/test_ima_ast.py` & `keylime-7.2.5/test/test_ima_ast.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/test/test_ima_dm.py` & `keylime-7.2.5/test/test_ima_dm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # pylint: disable=protected-access
 import unittest
+from typing import cast
 
-from keylime.ima import ast, ima_dm
+from keylime.ima import ast, ima_dm, types
 
 # Note that the tests depend also on ast parsing the raw data correctly.
 
 # Test dm_table_load events for all supported targets
 table_load_verity = ast.Entry(
     "10 fdcd389a7d084c7e1af8ed6917d080b1f0ee0625 ima-buf sha256:09e8a13203b10ce8d352aaafcdaf74986a6e2940e42c44c1a6603624135e1117 dm_table_load 646d5f76657273696f6e3d342e34352e303b6e616d653d746573742c757569643d43525950542d5645524954592d63373664303733343364336134396235616230313032356433623335346466352d746573742c6d616a6f723d3235332c6d696e6f723d302c6d696e6f725f636f756e743d312c6e756d5f746172676574733d313b7461726765745f696e6465783d302c7461726765745f626567696e3d302c7461726765745f6c656e3d3230343830382c7461726765745f6e616d653d7665726974792c7461726765745f76657273696f6e3d312e382e302c686173685f6661696c65643d562c7665726974795f76657273696f6e3d312c646174615f6465766963655f6e616d653d373a312c686173685f6465766963655f6e616d653d373a302c7665726974795f616c676f726974686d3d7368613235362c726f6f745f6469676573743d366561666665366238623031393930613165333937313236353734363865396237323263623634626139393432633664353836393438646131626434303936372c73616c743d643733386664396634323033663339376635613135353632633330323131393537303430636436373165666334363937313562663236383935363232656162632c69676e6f72655f7a65726f5f626c6f636b733d6e2c636865636b5f61745f6d6f73745f6f6e63653d6e3b"
 )
@@ -38,15 +39,15 @@
 target_update_verity = ast.Entry(
     "10 cf05b61f406363ba08d642a6b4e2c8760d68e12b ima-buf sha256:e480e9677c5865d72bbde6e84d8ea5d75ee3c87a682dd127b8bb439c643823ee dm_target_update 646d5f76657273696f6e3d342e34352e303b6e616d653d746573742c757569643d43525950542d5645524954592d63373664303733343364336134396235616230313032356433623335346466352d746573742c6d616a6f723d3235332c6d696e6f723d302c6d696e6f725f636f756e743d312c6e756d5f746172676574733d313b7461726765745f696e6465783d302c7461726765745f626567696e3d302c7461726765745f6c656e3d3230343830382c7461726765745f6e616d653d7665726974792c7461726765745f76657273696f6e3d312e382e302c686173685f6661696c65643d432c7665726974795f76657273696f6e3d312c646174615f6465766963655f6e616d653d373a312c686173685f6465766963655f6e616d653d373a302c7665726974795f616c676f726974686d3d7368613235362c726f6f745f6469676573743d366561666665366238623031393930613165333937313236353734363865396237323263623634626139393432633664353836393438646131626434303936372c73616c743d643733386664396634323033663339376635613135353632633330323131393537303430636436373165666334363937313562663236383935363232656162632c69676e6f72655f7a65726f5f626c6f636b733d6e2c636865636b5f61745f6d6f73745f6f6e63653d6e3b"
 )
 table_clear = ast.Entry(
     "10 6149775a61f3e878a806554865798b62295b90d0 ima-buf sha256:da71026bb20de95fd3f9d18b2b278980dcbe227a54fa8f94c8a4c26b2b2e5e55 dm_table_clear 646d5f76657273696f6e3d342e34352e303b6e616d653d746573742c757569643d43525950542d5645524954592d63373664303733343364336134396235616230313032356433623335346466352d746573743b7461626c655f636c6561723d6e6f5f646174613b00000000000000000000000000000000000063757272656e745f6465766963655f63617061636974793d3230343830383b"
 )
 
-example_policy_verity = {
+example_policy_verity: types.Policies = {
     "version": 1,
     "match_on": "uuid",
     "rules": {
         "example": {
             "required": True,
             "device_resume_required": True,
             "device_rename": {"valid_name": False, "valid_uuid": False},
@@ -93,15 +94,15 @@
 linear_rename_name = ast.Entry(
     "10 cf9f33a163183ebd4d92a42cd38305dfbc814748 ima-buf sha256:4088aee6143157dff39df843ff20467a500234f07d2c38b9312108455ea99968 dm_device_rename 646d5f76657273696f6e3d342e34352e303b6e616d653d746573742c757569643d2c6d616a6f723d3235332c6d696e6f723d302c6d696e6f725f636f756e743d312c6e756d5f746172676574733d313b6e65775f6e616d653d74657374322c6e65775f757569643d3b63757272656e745f6465766963655f63617061636974793d343236383033323b"
 )
 linear_rename_uuid = ast.Entry(
     "10 9f9f094b0aab1f07f967c61d0c4a18b26fad73ce ima-buf sha256:9144918395fbd350087fae06d02950c968342463734bb127533ae232bbbf1a42 dm_device_rename 646d5f76657273696f6e3d342e34352e303b6e616d653d74657374322c757569643d2c6d616a6f723d3235332c6d696e6f723d302c6d696e6f725f636f756e743d312c6e756d5f746172676574733d313b6e65775f6e616d653d74657374322c6e65775f757569643d746573745f757569643b63757272656e745f6465766963655f63617061636974793d343236383033323b"
 )
 
-example_policy_linear = {
+example_policy_linear: types.Policies = {
     "version": 1,
     "match_on": "name",
     "rules": {
         "example": {
             "required": True,
             "device_resume_required": True,
             "device_rename": {"valid_name": "test|test2", "valid_uuid": "invalid"},
@@ -131,183 +132,183 @@
     },
 }
 
 
 class TestImaDM(unittest.TestCase):
     def test_parser_table_load_verity(self):
         try:
-            ima_buf: ast.ImaBuf = table_load_verity.mode
+            ima_buf: ast.ImaBuf = cast(ast.ImaBuf, table_load_verity.mode)
             ima_dm.parse(ima_buf.data.data.decode(), ima_buf.name.name)
         except Exception as e:
             self.fail(f"Parsing failed with {str(e)}")
 
     def test_parser_table_load_linear(self):
         try:
-            ima_buf: ast.ImaBuf = table_load_linear.mode
+            ima_buf: ast.ImaBuf = cast(ast.ImaBuf, table_load_linear.mode)
             ima_dm.parse(ima_buf.data.data.decode(), ima_buf.name.name)
         except Exception as e:
             self.fail(f"Parsing failed with {str(e)}")
 
     def test_parser_table_load_snapshot(self):
         try:
-            ima_buf: ast.ImaBuf = table_load_snapshot.mode
+            ima_buf: ast.ImaBuf = cast(ast.ImaBuf, table_load_snapshot.mode)
             ima_dm.parse(ima_buf.data.data.decode(), ima_buf.name.name)
         except Exception as e:
             self.fail(f"Parsing failed with {str(e)}")
 
     def test_parser_table_load_integrity(self):
         try:
-            ima_buf: ast.ImaBuf = table_load_integrity.mode
+            ima_buf: ast.ImaBuf = cast(ast.ImaBuf, table_load_integrity.mode)
             ima_dm.parse(ima_buf.data.data.decode(), ima_buf.name.name)
         except Exception as e:
             self.fail(f"Parsing failed with {str(e)}")
 
     def test_parser_table_load_crypt(self):
         try:
-            ima_buf: ast.ImaBuf = table_load_crypt.mode
+            ima_buf: ast.ImaBuf = cast(ast.ImaBuf, table_load_crypt.mode)
             ima_dm.parse(ima_buf.data.data.decode(), ima_buf.name.name)
         except Exception as e:
             self.fail(f"Parsing failed with {str(e)}")
 
     def test_parser_table_load_cache(self):
         try:
-            ima_buf: ast.ImaBuf = table_load_cache.mode
+            ima_buf: ast.ImaBuf = cast(ast.ImaBuf, table_load_cache.mode)
             ima_dm.parse(ima_buf.data.data.decode(), ima_buf.name.name)
         except Exception as e:
             self.fail(f"Parsing failed with {str(e)}")
 
     def test_parser_table_load_mirror(self):
         try:
-            ima_buf: ast.ImaBuf = table_load_mirror.mode
+            ima_buf: ast.ImaBuf = cast(ast.ImaBuf, table_load_mirror.mode)
             ima_dm.parse(ima_buf.data.data.decode(), ima_buf.name.name)
         except Exception as e:
             self.fail(f"Parsing failed with {str(e)}")
 
     def test_parser_device_resume(self):
         try:
-            ima_buf: ast.ImaBuf = device_resume.mode
+            ima_buf: ast.ImaBuf = cast(ast.ImaBuf, device_resume.mode)
             ima_dm.parse(ima_buf.data.data.decode(), ima_buf.name.name)
         except Exception as e:
             self.fail(f"Parsing failed with {str(e)}")
 
     def test_parser_device_remove(self):
         try:
-            ima_buf: ast.ImaBuf = device_remove.mode
+            ima_buf: ast.ImaBuf = cast(ast.ImaBuf, device_remove.mode)
             ima_dm.parse(ima_buf.data.data.decode(), ima_buf.name.name)
         except Exception as e:
             self.fail(f"Parsing failed with {str(e)}")
 
     def test_parser_device_rename(self):
         try:
-            ima_buf: ast.ImaBuf = linear_rename_name.mode
+            ima_buf: ast.ImaBuf = cast(ast.ImaBuf, linear_rename_name.mode)
             ima_dm.parse(ima_buf.data.data.decode(), ima_buf.name.name)
         except Exception as e:
             self.fail(f"Parsing failed with {str(e)}")
 
     def test_parser_table_clear(self):
         try:
-            ima_buf: ast.ImaBuf = table_clear.mode
+            ima_buf: ast.ImaBuf = cast(ast.ImaBuf, table_clear.mode)
             ima_dm.parse(ima_buf.data.data.decode(), ima_buf.name.name)
         except Exception as e:
             self.fail(f"Parsing failed with {str(e)}")
 
     def test_basic_validation_verity(self):
         validator = ima_dm.DmIMAValidator(example_policy_verity)
 
         # Testing table load
-        ima_buf: ast.ImaBuf = table_load_verity.mode
+        ima_buf: ast.ImaBuf = cast(ast.ImaBuf, table_load_verity.mode)
         failure = validator.validate(ima_buf.digest, ima_buf.name, ima_buf.data)
         # the table load entry itself should be valid
         self.assertFalse(
             failure, f"Validation of table load failed with: {list(map(lambda x: x.context, failure.events))}"
         )
         # The policy also requires a table resume, so the overall state is invalid
         self.assertTrue(validator.invalid())
 
         # Testing device resume
-        ima_buf: ast.ImaBuf = device_resume.mode
+        ima_buf: ast.ImaBuf = cast(ast.ImaBuf, device_resume.mode)
         failure = validator.validate(ima_buf.digest, ima_buf.name, ima_buf.data)
         # the device resume entry itself should be valid
         self.assertFalse(
             failure, f"Validation of device resume failed with: {list(map(lambda x: x.context, failure.events))}"
         )
         # Now the all the policy should be valid
         self.assertFalse(validator.invalid())
 
         # Store valid state for restoring it between the next tests
         valid_state = validator.state_dump()
 
         # Test remove
         validator.state_load(valid_state)
-        ima_buf: ast.ImaBuf = device_remove.mode
+        ima_buf: ast.ImaBuf = cast(ast.ImaBuf, device_remove.mode)
         failure = validator.validate(ima_buf.digest, ima_buf.name, ima_buf.data)
         self.assertIn("ima.validation.dm.dm_device_remove.device_removed", failure.get_event_ids())
 
         # Test double load
         validator.state_load(valid_state)
-        ima_buf: ast.ImaBuf = table_load_verity.mode
+        ima_buf: ast.ImaBuf = cast(ast.ImaBuf, table_load_verity.mode)
         failure = validator.validate(ima_buf.digest, ima_buf.name, ima_buf.data)
         self.assertIn("ima.validation.dm.dm_table_load.multiple_table_loads", failure.get_event_ids())
 
         # Test target update
         validator.state_load(valid_state)
-        ima_buf: ast.ImaBuf = target_update_verity.mode
+        ima_buf: ast.ImaBuf = cast(ast.ImaBuf, target_update_verity.mode)
         failure = validator.validate(ima_buf.digest, ima_buf.name, ima_buf.data)
         self.assertIn("ima.validation.dm.dm_target_update.target_data_invalid", failure.get_event_ids())
 
         # Test clear
         validator.state_load(valid_state)
-        ima_buf: ast.ImaBuf = table_clear.mode
+        ima_buf: ast.ImaBuf = cast(ast.ImaBuf, table_clear.mode)
         failure = validator.validate(ima_buf.digest, ima_buf.name, ima_buf.data)
         self.assertIn("ima.validation.dm.dm_table_clear.table_cleared", failure.get_event_ids())
 
     def test_events_before_table_load(self):
         validator = ima_dm.DmIMAValidator(example_policy_verity)
 
         # Resume
-        ima_buf: ast.ImaBuf = device_resume.mode
+        ima_buf: ast.ImaBuf = cast(ast.ImaBuf, device_resume.mode)
         failure = validator.validate(ima_buf.digest, ima_buf.name, ima_buf.data)
         self.assertIn("ima.validation.dm.dm_device_resume.resume_before_table_load", failure.get_event_ids())
 
         # Remove
-        ima_buf: ast.ImaBuf = device_remove.mode
+        ima_buf: ast.ImaBuf = cast(ast.ImaBuf, device_remove.mode)
         failure = validator.validate(ima_buf.digest, ima_buf.name, ima_buf.data)
         self.assertIn("ima.validation.dm.dm_device_remove.remove_before_table_load", failure.get_event_ids())
 
         # Clear
-        ima_buf: ast.ImaBuf = table_clear.mode
+        ima_buf: ast.ImaBuf = cast(ast.ImaBuf, table_clear.mode)
         failure = validator.validate(ima_buf.digest, ima_buf.name, ima_buf.data)
         self.assertIn("ima.validation.dm.dm_table_clear.clear_before_table_load", failure.get_event_ids())
 
         # Update
-        ima_buf: ast.ImaBuf = target_update_verity.mode
+        ima_buf: ast.ImaBuf = cast(ast.ImaBuf, target_update_verity.mode)
         failure = validator.validate(ima_buf.digest, ima_buf.name, ima_buf.data)
         self.assertIn("ima.validation.dm.dm_target_update.update_before_table_load", failure.get_event_ids())
 
     def test_device_rename(self):
         validator = ima_dm.DmIMAValidator(example_policy_linear)
-        ima_buf: ast.ImaBuf = linear_table_load.mode
+        ima_buf: ast.ImaBuf = cast(ast.ImaBuf, linear_table_load.mode)
         failure = validator.validate(ima_buf.digest, ima_buf.name, ima_buf.data)
         self.assertFalse(failure)
 
-        ima_buf: ast.ImaBuf = linear_device_resume.mode
+        ima_buf: ast.ImaBuf = cast(ast.ImaBuf, linear_device_resume.mode)
         failure = validator.validate(ima_buf.digest, ima_buf.name, ima_buf.data)
         self.assertFalse(failure)
 
         # Rename the device
         self.assertIn("test", validator.devices)
-        ima_buf: ast.ImaBuf = linear_rename_name.mode
+        ima_buf: ast.ImaBuf = cast(ast.ImaBuf, linear_rename_name.mode)
         failure = validator.validate(ima_buf.digest, ima_buf.name, ima_buf.data)
         self.assertFalse(failure)
         # Check if the device was also moved in the validator
         self.assertNotIn("test", validator.devices)
         self.assertIn("test2", validator.devices)
 
         # New uuid should be invalid
-        ima_buf: ast.ImaBuf = linear_rename_uuid.mode
+        ima_buf: ast.ImaBuf = cast(ast.ImaBuf, linear_rename_uuid.mode)
         failure = validator.validate(ima_buf.digest, ima_buf.name, ima_buf.data)
         self.assertIn("ima.validation.dm.dm_device_rename.new_uuid_invalid", failure.get_event_ids())
 
     def test_matching_func(self):
         for entry in [None, False, True, "test", 123]:
             self.assertTrue(ima_dm._check_attr(entry, None))
```

### Comparing `keylime-7.0.0/test/test_ima_verification.py` & `keylime-7.2.5/test/test_ima_verification.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
         pcrval = None
         lines = MEASUREMENTS.splitlines()
         agentAttestState = AgentAttestState("1")
         running_hash = agentAttestState.get_pcr_state(10)
         assert running_hash is not None
         for line in lines:
             parts = line.split(" ")
-            template_hash = codecs.decode(parts[1].encode("utf-8"), "hex")
+            template_hash = bytes.fromhex(parts[1])
             running_hash = hashlib.sha1(running_hash + template_hash).digest()
             pcrval = codecs.encode(running_hash, "hex").decode("utf-8")
             ima_hash, _ = ima.process_measurement_list(agentAttestState, [line], pcrval=pcrval)
             self.assertTrue(ima_hash == pcrval)
 
         # Feed empty iterative measurement list simulating 'no new measurement list entries' on attested system
         ima_hash, _ = ima.process_measurement_list(agentAttestState, [], pcrval=pcrval)
```

### Comparing `keylime-7.0.0/test/test_json.py` & `keylime-7.2.5/test/test_json.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/test/test_policy_conversion.py` & `keylime-7.2.5/test/test_policy_conversion.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/test/test_registrar_db.py` & `keylime-7.2.5/test/test_registrar_db.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/test/test_retry_algo.py` & `keylime-7.2.5/test/test_retry_algo.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/test/test_signing.py` & `keylime-7.2.5/test/test_signing.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/test/test_tpm.py` & `keylime-7.2.5/test/test_tpm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import unittest
 
 from packaging.version import Version
 
 from keylime.common.algorithms import Hash
-from keylime.tpm.tpm_main import tpm
+from keylime.tpm.tpm_main import Tpm
 
-TPM2TOOLS_VERSION = Version(tpm().tools_version)
+TPM2TOOLS_VERSION = Version(Tpm().tools_version)
 
 # ############################################################
 # list of input challenges for get_tpm_manufacturer function
 # ############################################################
 tpm_manufacturer_tests = [
     # Infineon Optiga SLB9665'
     {
@@ -78,25 +78,25 @@
         "response": "SW",
     },
 ]
 
 
 class TestTPM(unittest.TestCase):
     def setUp(self):
-        self.tpm = tpm()
+        self.Tpm = Tpm()
 
     @unittest.skipIf(TPM2TOOLS_VERSION < Version("4.2"), "tpm_eventlog is not available")
     def test_parse_mb_bootlog(self):
         """Test parsing binary measured boot event log"""
         # Use the file that triggered https://github.com/keylime/keylime/issues/1153
         mb_log_path = os.path.abspath(os.path.join(os.path.dirname(__file__), "data/mb_log.b64"))
         with open(mb_log_path, encoding="utf-8") as f:
             # Read the base64 input and remove the newlines
             b64 = "".join(f.read().splitlines())
-            pcr_hashes, boot_aggregates, measurement_data, failure = self.tpm.parse_mb_bootlog(b64, Hash.SHA256)
+            pcr_hashes, boot_aggregates, measurement_data, failure = self.Tpm.parse_mb_bootlog(b64, Hash.SHA256)
 
             self.assertFalse(
                 failure, f"Parsing of measured boot log failed with: {list(map(lambda x: x.context, failure.events))}"
             )
             self.assertTrue(isinstance(pcr_hashes, dict))
             self.assertTrue(isinstance(boot_aggregates, dict))
             self.assertTrue(isinstance(measurement_data, dict))
```

### Comparing `keylime-7.0.0/test/test_validators.py` & `keylime-7.2.5/test/test_validators.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/test/test_verifier_db.py` & `keylime-7.2.5/test/test_verifier_db.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/test/test_version.py` & `keylime-7.2.5/test/test_version.py`

 * *Files identical despite different names*

### Comparing `keylime-7.0.0/test/test_web_util.py` & `keylime-7.2.5/test/test_web_util.py`

 * *Files identical despite different names*

