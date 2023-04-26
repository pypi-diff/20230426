# Comparing `tmp/in_toto-1.3.2.tar.gz` & `tmp/in_toto-1.4.0.tar.gz`

## Comparing `in_toto-1.3.2.tar` & `in_toto-1.4.0.tar`

### file list

```diff
@@ -1,92 +1,96 @@
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 in_toto-1.3.2/.coveragerc
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 in_toto-1.3.2/requirements-dev.txt
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 in_toto-1.3.2/requirements-docs.txt
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 in_toto-1.3.2/requirements-pinned.txt
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 in_toto-1.3.2/requirements-tox.txt
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 in_toto-1.3.2/requirements.txt
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 in_toto-1.3.2/tox.ini
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 in_toto-1.3.2/in_toto/__init__.py
--rw-r--r--   0        0        0     6230 2020-02-02 00:00:00.000000 in_toto-1.3.2/in_toto/common_args.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 in_toto-1.3.2/in_toto/exceptions.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 in_toto-1.3.2/in_toto/formats.py
--rw-r--r--   0        0        0     4893 2020-02-02 00:00:00.000000 in_toto-1.3.2/in_toto/in_toto_keygen.py
--rwxr-xr-x   0        0        0     3476 2020-02-02 00:00:00.000000 in_toto-1.3.2/in_toto/in_toto_mock.py
--rw-r--r--   0        0        0     8361 2020-02-02 00:00:00.000000 in_toto-1.3.2/in_toto/in_toto_record.py
--rwxr-xr-x   0        0        0     8564 2020-02-02 00:00:00.000000 in_toto-1.3.2/in_toto/in_toto_run.py
--rw-r--r--   0        0        0    12478 2020-02-02 00:00:00.000000 in_toto-1.3.2/in_toto/in_toto_sign.py
--rwxr-xr-x   0        0        0     7428 2020-02-02 00:00:00.000000 in_toto-1.3.2/in_toto/in_toto_verify.py
--rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 in_toto-1.3.2/in_toto/log.py
--rw-r--r--   0        0        0    10037 2020-02-02 00:00:00.000000 in_toto-1.3.2/in_toto/rulelib.py
--rw-r--r--   0        0        0    38491 2020-02-02 00:00:00.000000 in_toto-1.3.2/in_toto/runlib.py
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 in_toto-1.3.2/in_toto/settings.py
--rw-r--r--   0        0        0     5943 2020-02-02 00:00:00.000000 in_toto-1.3.2/in_toto/user_settings.py
--rw-r--r--   0        0        0    50821 2020-02-02 00:00:00.000000 in_toto-1.3.2/in_toto/verifylib.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 in_toto-1.3.2/in_toto/models/__init__.py
--rw-r--r--   0        0        0     7659 2020-02-02 00:00:00.000000 in_toto-1.3.2/in_toto/models/_signer.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 in_toto-1.3.2/in_toto/models/common.py
--rw-r--r--   0        0        0    22230 2020-02-02 00:00:00.000000 in_toto-1.3.2/in_toto/models/layout.py
--rw-r--r--   0        0        0     5682 2020-02-02 00:00:00.000000 in_toto-1.3.2/in_toto/models/link.py
--rw-r--r--   0        0        0     8765 2020-02-02 00:00:00.000000 in_toto-1.3.2/in_toto/models/metadata.py
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/__init__.py
--rw-r--r--   0        0        0     5395 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/common.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/runtests.py
--rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/test_common_args.py
--rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/test_in_toto_keygen.py
--rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/test_in_toto_mock.py
--rw-r--r--   0        0        0     9011 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/test_in_toto_record.py
--rwxr-xr-x   0        0        0     9516 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/test_in_toto_run.py
--rw-r--r--   0        0        0     9175 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/test_in_toto_sign.py
--rwxr-xr-x   0        0        0     8059 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/test_in_toto_verify.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/test_log.py
--rw-r--r--   0        0        0     5770 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/test_param_substitution.py
--rw-r--r--   0        0        0    10867 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/test_rulelib.py
--rwxr-xr-x   0        0        0    37617 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/test_runlib.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/test_settings.py
--rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/test_user_settings.py
--rw-r--r--   0        0        0    59940 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/test_verifylib.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/demo_files/alice
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/demo_files/alice.pub
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/demo_files/bob
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/demo_files/bob.pub
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/demo_files/carl
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/demo_files/carl.pub
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/demo_files/danny
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/demo_files/danny.pub
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/demo_files/demo.layout.template
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/demo_files/foo.tar.gz
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/demo_files/package.2f89b927.link
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/demo_files/write-code.776a00e2.link
--rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/demo_files_gpg/demo.layout.template
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/demo_files_gpg/foo.tar.gz
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/demo_files_gpg/package.7b3abb26.link
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/demo_files_gpg/write-code.8288ef56.link
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/gpg_keyrings/dsa/C242A830DAAF1C2BEF604A9EF033A3A3E267B3B1.ssh
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/gpg_keyrings/dsa/pubring.gpg
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/gpg_keyrings/dsa/random_seed
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/gpg_keyrings/dsa/secring.gpg
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/gpg_keyrings/dsa/trustdb.gpg
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/gpg_keyrings/rsa/7B3ABB26B97B655AB9296BD15B0BD02E1C768C43.ssh
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/gpg_keyrings/rsa/8288EF560ED3795F9DF2C0DB56193089B285DA58.ssh
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/gpg_keyrings/rsa/8465A1E2E0FB2B40ADB2478E18FB3F537E0C8A17.ssh
--rw-r--r--   0        0        0    17740 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/gpg_keyrings/rsa/pubring.gpg
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/gpg_keyrings/rsa/random_seed
--rw-r--r--   0        0        0    27893 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/gpg_keyrings/rsa/secring.gpg
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/gpg_keyrings/rsa/trustdb.gpg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/models/__init__.py
--rwxr-xr-x   0        0        0      701 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/models/test_common.py
--rwxr-xr-x   0        0        0     1820 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/models/test_inspection.py
--rwxr-xr-x   0        0        0    13227 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/models/test_layout.py
--rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/models/test_link.py
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/models/test_metadata.py
--rw-r--r--   0        0        0     5084 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/models/test_signer.py
--rwxr-xr-x   0        0        0     2943 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/models/test_step.py
--rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/models/test_supply_chain_item.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/rc_test/.in_totorc
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/scripts/expr
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/scripts/tar
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 in_toto-1.3.2/tests/scripts/touch
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 in_toto-1.3.2/.gitignore
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 in_toto-1.3.2/LICENSE
--rw-r--r--   0        0        0    11304 2020-02-02 00:00:00.000000 in_toto-1.3.2/README.md
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 in_toto-1.3.2/pyproject.toml
--rw-r--r--   0        0        0    12838 2020-02-02 00:00:00.000000 in_toto-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 in_toto-1.4.0/.coveragerc
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 in_toto-1.4.0/requirements-dev.txt
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 in_toto-1.4.0/requirements-docs.txt
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 in_toto-1.4.0/requirements-pinned.txt
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 in_toto-1.4.0/requirements-tox.txt
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 in_toto-1.4.0/requirements.txt
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 in_toto-1.4.0/tox.ini
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/__init__.py
+-rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/common_args.py
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/exceptions.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/formats.py
+-rw-r--r--   0        0        0     4893 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/in_toto_keygen.py
+-rwxr-xr-x   0        0        0     3571 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/in_toto_mock.py
+-rw-r--r--   0        0        0     8469 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/in_toto_record.py
+-rwxr-xr-x   0        0        0     8666 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/in_toto_run.py
+-rw-r--r--   0        0        0    12640 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/in_toto_sign.py
+-rwxr-xr-x   0        0        0     7426 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/in_toto_verify.py
+-rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/log.py
+-rw-r--r--   0        0        0    10037 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/rulelib.py
+-rw-r--r--   0        0        0    40820 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/runlib.py
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/settings.py
+-rw-r--r--   0        0        0     5943 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/user_settings.py
+-rw-r--r--   0        0        0    50740 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/verifylib.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/models/__init__.py
+-rw-r--r--   0        0        0     7659 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/models/_signer.py
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/models/common.py
+-rw-r--r--   0        0        0    22230 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/models/layout.py
+-rw-r--r--   0        0        0     5682 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/models/link.py
+-rw-r--r--   0        0        0    13268 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/models/metadata.py
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     5395 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/common.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/runtests.py
+-rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/test_common_args.py
+-rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/test_in_toto_keygen.py
+-rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/test_in_toto_mock.py
+-rw-r--r--   0        0        0    11441 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/test_in_toto_record.py
+-rwxr-xr-x   0        0        0    13626 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/test_in_toto_run.py
+-rw-r--r--   0        0        0    13346 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/test_in_toto_sign.py
+-rwxr-xr-x   0        0        0    13887 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/test_in_toto_verify.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/test_log.py
+-rw-r--r--   0        0        0     6422 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/test_param_substitution.py
+-rw-r--r--   0        0        0    10867 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/test_rulelib.py
+-rwxr-xr-x   0        0        0    39644 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/test_runlib.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/test_settings.py
+-rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/test_user_settings.py
+-rw-r--r--   0        0        0    59574 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/test_verifylib.py
+-rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/demo_dsse_files/demo.layout.template
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/demo_dsse_files/package.2f89b927.link
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/demo_dsse_files/write-code.776a00e2.link
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/demo_files/alice
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/demo_files/alice.pub
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/demo_files/bob
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/demo_files/bob.pub
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/demo_files/carl
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/demo_files/carl.pub
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/demo_files/danny
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/demo_files/danny.pub
+-rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/demo_files/demo.layout.template
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/demo_files/foo.tar.gz
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/demo_files/package.2f89b927.link
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/demo_files/write-code.776a00e2.link
+-rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/demo_files_gpg/demo.layout.template
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/demo_files_gpg/foo.tar.gz
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/demo_files_gpg/package.7b3abb26.link
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/demo_files_gpg/write-code.8288ef56.link
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/gpg_keyrings/dsa/C242A830DAAF1C2BEF604A9EF033A3A3E267B3B1.ssh
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/gpg_keyrings/dsa/pubring.gpg
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/gpg_keyrings/dsa/random_seed
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/gpg_keyrings/dsa/secring.gpg
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/gpg_keyrings/dsa/trustdb.gpg
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/gpg_keyrings/rsa/7B3ABB26B97B655AB9296BD15B0BD02E1C768C43.ssh
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/gpg_keyrings/rsa/8288EF560ED3795F9DF2C0DB56193089B285DA58.ssh
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/gpg_keyrings/rsa/8465A1E2E0FB2B40ADB2478E18FB3F537E0C8A17.ssh
+-rw-r--r--   0        0        0    17740 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/gpg_keyrings/rsa/pubring.gpg
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/gpg_keyrings/rsa/random_seed
+-rw-r--r--   0        0        0    27893 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/gpg_keyrings/rsa/secring.gpg
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/gpg_keyrings/rsa/trustdb.gpg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/models/__init__.py
+-rwxr-xr-x   0        0        0      701 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/models/test_common.py
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/models/test_envelope.py
+-rwxr-xr-x   0        0        0     1820 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/models/test_inspection.py
+-rwxr-xr-x   0        0        0    13227 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/models/test_layout.py
+-rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/models/test_link.py
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/models/test_metadata.py
+-rw-r--r--   0        0        0     5084 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/models/test_signer.py
+-rwxr-xr-x   0        0        0     2943 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/models/test_step.py
+-rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/models/test_supply_chain_item.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/rc_test/.in_totorc
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/scripts/expr
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/scripts/tar
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/scripts/touch
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 in_toto-1.4.0/.gitignore
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 in_toto-1.4.0/LICENSE
+-rw-r--r--   0        0        0    11304 2020-02-02 00:00:00.000000 in_toto-1.4.0/README.md
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 in_toto-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0    12838 2020-02-02 00:00:00.000000 in_toto-1.4.0/PKG-INFO
```

### Comparing `in_toto-1.3.2/requirements-pinned.txt` & `in_toto-1.4.0/requirements-pinned.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --output-file=requirements-pinned.txt requirements.txt
 #
-attrs==22.2.0
+attrs==23.1.0
     # via -r requirements.txt
 cffi==1.15.1
     # via
     #   cryptography
     #   pynacl
-cryptography==39.0.2
+cryptography==40.0.2
     # via securesystemslib
 iso8601==1.1.0
     # via -r requirements.txt
-pathspec==0.11.0
+pathspec==0.11.1
     # via -r requirements.txt
 pycparser==2.21
     # via cffi
 pynacl==1.5.0
     # via securesystemslib
 python-dateutil==2.8.2
     # via -r requirements.txt
-securesystemslib[crypto,pynacl]==0.27.0
+securesystemslib[crypto,pynacl]==0.28.0
     # via -r requirements.txt
 six==1.16.0
     # via python-dateutil
```

### Comparing `in_toto-1.3.2/tox.ini` & `in_toto-1.4.0/tox.ini`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/in_toto/common_args.py` & `in_toto-1.4.0/in_toto/common_args.py`

 * *Files 3% similar despite different names*

```diff
@@ -158,14 +158,22 @@
   "required": False,
   "type": str,
   "metavar": "<directory>",
   "help": ("path to a directory to dump metadata. If '--metadata-directory'"
            " is not passed, the current working direcotry is used.")
 }
 
+DSSE_ARGS = ["--use-dsse"]
+DSSE_KWARGS = {
+  "dest": "use_dsse",
+  "default": False,
+  "action": "store_true",
+  "help": ("generate metadata using dsse (experimental)."),
+}
+
 
 def title_case_action_groups(parser):
   """Capitalize the first character of all words in the title of each action
   group of the passed parser.
 
   This is useful for consistency when using the sphinx argparse extension,
   which title-cases default action groups only.
```

### Comparing `in_toto-1.3.2/in_toto/exceptions.py` & `in_toto-1.4.0/in_toto/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,7 +25,10 @@
   """Indicates that a link file was not found. """
 
 class UnsupportedKeyTypeError(Error):
   """Indicates that the specified key type is not yet supported. """
 
 class PrefixError(Error):
   """Indicates that there is an error because of the prefixes passed. """
+
+class InvalidMetadata(Error):
+  """Indicates that the metadata is not valid."""
```

### Comparing `in_toto-1.3.2/in_toto/formats.py` & `in_toto-1.4.0/in_toto/formats.py`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/in_toto/in_toto_keygen.py` & `in_toto-1.4.0/in_toto/in_toto_keygen.py`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/in_toto/in_toto_mock.py` & `in_toto-1.4.0/in_toto/in_toto_mock.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,16 @@
   0 if no exception occurred
 
 """
 import sys
 import argparse
 import logging
 import in_toto.runlib
-from in_toto.common_args import title_case_action_groups, sort_action_groups
+from in_toto.common_args import (title_case_action_groups, sort_action_groups,
+    DSSE_ARGS, DSSE_KWARGS)
 from in_toto import __version__
 
 # Command line interfaces should use in_toto base logger (c.f. in_toto.log)
 LOG = logging.getLogger("in_toto")
 
 
 def create_parser():
@@ -76,14 +77,16 @@
   # FIXME: Do we limit the allowed characters for the name?
   named_args.add_argument("-n", "--name", type=str, required=True,
       metavar="<name>", help=(
       "name for the resulting link metadata file, which is written to"
       " '<name>.link'. It is also used to associate the link with a step"
       " defined in an in-toto layout."))
 
+  parser.add_argument(*DSSE_ARGS, **DSSE_KWARGS)
+
   # FIXME: This is not yet ideal.
   # What should we do with tokens like > or ; ?
   parser.add_argument("link_cmd", nargs="+", metavar="<command>",
       help=(
       "command to be executed. It is separated from named and optional"
       " arguments by a double dash '--'."))
 
@@ -102,15 +105,15 @@
   args = parser.parse_args()
 
   # in-toto-mock should not be used to secure the supply chain but only to try
   # out in-toto-run with max. user feedback, hence we set a verbose log level
   LOG.setLevel(logging.INFO)
 
   try:
-    in_toto.runlib.in_toto_mock(args.name, args.link_cmd)
+    in_toto.runlib.in_toto_mock(args.name, args.link_cmd, args.use_dsse)
 
   except Exception as e:
     LOG.error("(in-toto-mock) {0}: {1}".format(type(e).__name__, e))
     sys.exit(1)
 
   sys.exit(0)
```

### Comparing `in_toto-1.3.2/in_toto/in_toto_record.py` & `in_toto-1.4.0/in_toto/in_toto_record.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,16 @@
 
 from in_toto.common_args import (EXCLUDE_ARGS, EXCLUDE_KWARGS, BASE_PATH_ARGS,
     BASE_PATH_KWARGS, LSTRIP_PATHS_ARGS, LSTRIP_PATHS_KWARGS, KEY_ARGS,
     KEY_KWARGS, KEY_TYPE_KWARGS, KEY_TYPE_ARGS, GPG_ARGS, GPG_KWARGS,
     GPG_HOME_ARGS, GPG_HOME_KWARGS, VERBOSE_ARGS, VERBOSE_KWARGS, QUIET_ARGS,
     QUIET_KWARGS, METADATA_DIRECTORY_ARGS, METADATA_DIRECTORY_KWARGS,
     KEY_PASSWORD_ARGS, KEY_PASSWORD_KWARGS, parse_password_and_prompt_args,
-    sort_action_groups, title_case_action_groups, OPTS_TITLE)
+    sort_action_groups, title_case_action_groups, OPTS_TITLE, DSSE_ARGS,
+    DSSE_KWARGS)
 
 from securesystemslib import interface
 
 
 # Command line interfaces should use in_toto base logger (c.f. in_toto.log)
 LOG = logging.getLogger("in_toto")
 
@@ -108,14 +109,15 @@
 
   parent_named_args.add_argument(*GPG_ARGS, **GPG_KWARGS)
   parent_parser.add_argument(*GPG_HOME_ARGS, **GPG_HOME_KWARGS)
 
   parent_parser.add_argument(*EXCLUDE_ARGS, **EXCLUDE_KWARGS)
   parent_parser.add_argument(*BASE_PATH_ARGS, **BASE_PATH_KWARGS)
   parent_parser.add_argument(*LSTRIP_PATHS_ARGS, **LSTRIP_PATHS_KWARGS)
+  parent_parser.add_argument(*DSSE_ARGS, **DSSE_KWARGS)
 
   verbosity_args = parent_parser.add_mutually_exclusive_group(required=False)
   verbosity_args.add_argument(*VERBOSE_ARGS, **VERBOSE_KWARGS)
   verbosity_args.add_argument(*QUIET_ARGS, **QUIET_KWARGS)
 
   subparser_start = subparsers.add_parser("start", parents=[parent_parser],
       help=(
@@ -197,15 +199,15 @@
           args.key, key_type=args.key_type, password=password, prompt=prompt)
 
     if args.command == "start":
       in_toto.runlib.in_toto_record_start(args.step_name, args.materials,
           signing_key=key, gpg_keyid=gpg_keyid,
           gpg_use_default=gpg_use_default, gpg_home=args.gpg_home,
           exclude_patterns=args.exclude_patterns, base_path=args.base_path,
-          lstrip_paths=args.lstrip_paths)
+          lstrip_paths=args.lstrip_paths, use_dsse=args.use_dsse)
 
     # Mutually exclusiveness is guaranteed by argparser
     else: # args.command == "stop":
       in_toto.runlib.in_toto_record_stop(args.step_name, args.products,
           signing_key=key, gpg_keyid=gpg_keyid,
           gpg_use_default=gpg_use_default, gpg_home=args.gpg_home,
           exclude_patterns=args.exclude_patterns, base_path=args.base_path,
```

### Comparing `in_toto-1.3.2/in_toto/in_toto_run.py` & `in_toto-1.4.0/in_toto/in_toto_run.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,16 @@
 
 from in_toto.common_args import (EXCLUDE_ARGS, EXCLUDE_KWARGS, BASE_PATH_ARGS,
     BASE_PATH_KWARGS, LSTRIP_PATHS_ARGS, LSTRIP_PATHS_KWARGS, KEY_ARGS,
     KEY_KWARGS, KEY_TYPE_KWARGS, KEY_TYPE_ARGS, GPG_ARGS, GPG_KWARGS,
     GPG_HOME_ARGS, GPG_HOME_KWARGS, VERBOSE_ARGS, VERBOSE_KWARGS, QUIET_ARGS,
     QUIET_KWARGS, METADATA_DIRECTORY_ARGS, METADATA_DIRECTORY_KWARGS,
     KEY_PASSWORD_ARGS, KEY_PASSWORD_KWARGS, parse_password_and_prompt_args,
-    sort_action_groups, title_case_action_groups, OPTS_TITLE)
+    sort_action_groups, title_case_action_groups, OPTS_TITLE, DSSE_ARGS,
+    DSSE_KWARGS,)
 
 from securesystemslib import interface
 
 # Command line interfaces should use in_toto base logger (c.f. in_toto.log)
 LOG = logging.getLogger("in_toto")
 
 
@@ -148,14 +149,15 @@
   named_args.add_argument(*GPG_ARGS, **GPG_KWARGS)
   parser.add_argument(*GPG_HOME_ARGS, **GPG_HOME_KWARGS)
 
   parser.add_argument(*EXCLUDE_ARGS, **EXCLUDE_KWARGS)
   parser.add_argument(*BASE_PATH_ARGS, **BASE_PATH_KWARGS)
   parser.add_argument(*LSTRIP_PATHS_ARGS, **LSTRIP_PATHS_KWARGS)
   parser.add_argument(*METADATA_DIRECTORY_ARGS, **METADATA_DIRECTORY_KWARGS)
+  parser.add_argument(*DSSE_ARGS, **DSSE_KWARGS)
 
   verbosity_args = parser.add_mutually_exclusive_group(required=False)
   verbosity_args.add_argument(*VERBOSE_ARGS, **VERBOSE_KWARGS)
   verbosity_args.add_argument(*QUIET_ARGS, **QUIET_KWARGS)
 
 
   # FIXME: This is not yet ideal.
@@ -220,15 +222,15 @@
 
     runlib.in_toto_run(
         args.step_name, args.materials, args.products, args.link_cmd,
         record_streams=args.record_streams, signing_key=key,
         gpg_keyid=gpg_keyid, gpg_use_default=gpg_use_default,
         gpg_home=args.gpg_home, exclude_patterns=args.exclude_patterns,
         base_path=args.base_path, lstrip_paths=args.lstrip_paths,
-        metadata_directory=args.metadata_directory)
+        metadata_directory=args.metadata_directory, use_dsse=args.use_dsse)
 
   except Exception as e:
     LOG.error("(in-toto-run) {0}: {1}".format(type(e).__name__, e))
     sys.exit(1)
 
   sys.exit(0)
```

### Comparing `in_toto-1.3.2/in_toto/in_toto_sign.py` & `in_toto-1.4.0/in_toto/in_toto_sign.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,39 +24,42 @@
 """
 import sys
 import argparse
 import logging
 
 from in_toto import exceptions
 from in_toto.models.link import FILENAME_FORMAT
-from in_toto.models.metadata import Metablock
+from in_toto.models.metadata import Metadata
+from in_toto.models._signer import GPGSigner
 from in_toto.common_args import (GPG_HOME_ARGS, GPG_HOME_KWARGS, VERBOSE_ARGS,
     VERBOSE_KWARGS, QUIET_ARGS, QUIET_KWARGS, title_case_action_groups,
     sort_action_groups)
 from in_toto import (
     __version__, SUPPORTED_KEY_TYPES, KEY_TYPE_RSA, KEY_TYPE_ED25519,
     KEY_TYPE_ECDSA)
 
 import securesystemslib.formats
+import securesystemslib.exceptions
 from securesystemslib import interface
 from securesystemslib.gpg import functions as gpg_interface
+from securesystemslib.signer import SSlibSigner
 
 
 # Command line interfaces should use in_toto base logger (c.f. in_toto.log)
 LOG = logging.getLogger("in_toto")
 
 
 def _sign_and_dump_metadata(metadata, args):
   """
   <Purpose>
     Internal method to sign link or layout metadata and dump it to disk.
 
   <Arguments>
     metadata:
-            Metablock object (contains Link or Layout object)
+            Metadata object (contains Link or Layout object)
     args:
             see argparser
 
   <Exceptions>
     SystemExit(0) if signing is successful
     SystemExit(2) if any exception occurs
 
@@ -71,20 +74,22 @@
     # a list (not None) and we will try to sign with gpg.
     # If `--gpg-home` was not set, args.gpg_home is None and the signer tries
     # to use the default gpg keyring.
     if args.gpg is not None:
       # If `--gpg` was passed without argument we sign with the default key
       # Excluded so that coverage does not vary in different test environments
       if len(args.gpg) == 0: # pragma: no cover
-        signature = metadata.sign_gpg(gpg_keyid=None, gpg_home=args.gpg_home)
+        signature = metadata.create_signature(
+          GPGSigner(None, homedir=args.gpg_home))
 
       # Otherwise we sign with each passed keyid
       for keyid in args.gpg:
         securesystemslib.formats.KEYID_SCHEMA.check_match(keyid)
-        signature = metadata.sign_gpg(gpg_keyid=keyid, gpg_home=args.gpg_home)
+        signature = metadata.create_signature(
+            GPGSigner(keyid, homedir=args.gpg_home))
 
     # Alternatively we iterate over passed private key paths `--key KEYPATH
     # ...` load the corresponding key from disk and sign with it
     elif args.key is not None: # pragma: no branch
 
       if args.key_type is None:
         args.key_type = [KEY_TYPE_RSA] * len(args.key)
@@ -93,34 +98,35 @@
         raise securesystemslib.exceptions.FormatError(
           "number of key_types should match with the number"
           " of keys specified")
 
       for idx, key_path in enumerate(args.key):
         key = interface.import_privatekey_from_file(
             key_path, key_type=args.key_type[idx], prompt=args.prompt)
-        signature = metadata.sign(key)
+        signature = metadata.create_signature(SSlibSigner(key))
+
+    payload = metadata.get_payload()
+    _type = payload.type_
 
     # If `--output` was specified we store the signed link or layout metadata
     # to that location no matter what
     if args.output:
       out_path = args.output
 
     # Otherwise, in case of links, we build the filename using the link/step
     # name and the keyid of the created signature (there is only one for links)
-    elif metadata.type_ == "link":
-      securesystemslib.formats.ANY_SIGNATURE_SCHEMA.check_match(signature)
-      keyid = signature["keyid"]
-      out_path = FILENAME_FORMAT.format(step_name=metadata.signed.name,
-          keyid=keyid)
+    elif _type == "link":
+      keyid = signature.keyid
+      out_path = FILENAME_FORMAT.format(step_name=payload.name, keyid=keyid)
 
     # In case of layouts we just override the input file.
-    elif metadata.type_ == "layout": # pragma: no branch
+    elif _type == "layout": # pragma: no branch
       out_path = args.file
 
-    LOG.info("Dumping {0} to '{1}'...".format(metadata.type_, out_path))
+    LOG.info("Dumping {0} to '{1}'...".format(_type, out_path))
 
     metadata.dump(out_path)
     sys.exit(0)
 
   except Exception as e:
     LOG.error("The following error occurred while signing: "
         "{}".format(e))
@@ -130,15 +136,15 @@
 def _verify_metadata(metadata, args):
   """
   <Purpose>
     Internal method to verify link or layout signatures.
 
   <Arguments>
     metadata:
-            Metablock object (contains Link or Layout object)
+            Metadata object (contains Link or Layout object)
     args:
             see argparser
 
   <Exceptions>
     SystemExit(0) if verification passes
     SystemExit(1) if verification fails
     SystemExit(2) if any exception occurs
@@ -172,29 +178,29 @@
         "{}".format(e))
     sys.exit(2)
 
 
 def _load_metadata(file_path):
   """
   <Purpose>
-    Loads Metablock (link or layout metadata) file from disk
+    Loads Metadata (link or layout metadata) file from disk
 
   <Arguments>
     file_path:
             path to link or layout metadata file
 
   <Exceptions>
     SystemExit(2) if any exception occurs
 
   <Returns>
-    in-toto Metablock object (contains Link or Layout object)
+    in-toto Metadata object (contains Link or Layout object)
 
   """
   try:
-    return Metablock.load(file_path)
+    return Metadata.load(file_path)
 
   except Exception as e:
     LOG.error("The following error occurred while loading the file '{}': "
         "{}".format(file_path, e))
     sys.exit(2)
 
 
@@ -344,15 +350,16 @@
     parser.print_help()
     parser.error("missing arguments: specify at least one keyid for GPG"
       " signature verification ('--gpg KEYID ...')")
 
   metadata = _load_metadata(args.file)
 
   # Specific command line argument restrictions if we deal with links
-  if metadata.type_ == "link":
+  payload = metadata.get_payload()
+  if payload.type_ == "link":
     # Above we check that it's either `--key ...` or `--gpg ...`
     # Here we check that it is not more than one in each case when dealing
     # with links
     link_error_message = ("link metadata is associated with a"
         " single functionary and is usually namespaced accordingly:"
         " '<name>.<keyid prefix>.link'.")
```

### Comparing `in_toto-1.3.2/in_toto/in_toto_verify.py` & `in_toto-1.4.0/in_toto/in_toto_verify.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 import argparse
 import logging
 
 from in_toto import verifylib
 from in_toto.common_args import (GPG_HOME_ARGS, GPG_HOME_KWARGS, VERBOSE_ARGS,
     VERBOSE_KWARGS, QUIET_ARGS, QUIET_KWARGS, title_case_action_groups,
     sort_action_groups, OPTS_TITLE)
-from in_toto.models.metadata import Metablock
+from in_toto.models.metadata import Metadata
 from in_toto import (
     __version__, SUPPORTED_KEY_TYPES, KEY_TYPE_RSA, KEY_TYPE_ED25519,
     KEY_TYPE_ECDSA)
 from securesystemslib import interface
 from securesystemslib.gpg import functions as gpg_interface
 
 # Command line interfaces should use in_toto base logger (c.f. in_toto.log)
@@ -172,15 +172,15 @@
   if (args.layout_keys is None) and (args.gpg is None):
     parser.print_help()
     parser.error("wrong arguments: specify at least one of"
         " '--layout-keys path [path ...]' or '--gpg id [id ...]'")
 
   try:
     LOG.info("Loading layout...")
-    layout = Metablock.load(args.layout)
+    layout = Metadata.load(args.layout)
 
     layout_key_dict = {}
     if args.layout_keys is not None:
       LOG.info("Loading layout key(s)...")
       layout_key_dict.update(
           interface.import_publickeys_from_file(
               args.layout_keys, args.key_types))
```

### Comparing `in_toto-1.3.2/in_toto/log.py` & `in_toto-1.4.0/in_toto/log.py`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/in_toto/rulelib.py` & `in_toto-1.4.0/in_toto/rulelib.py`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/in_toto/runlib.py` & `in_toto-1.4.0/in_toto/runlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
   The wrapper performs the following tasks which are implemented in this
   library.
 
     - Record state of material (files the command is executed on)
     - Execute command
       - Capture stdout/stderr/return value of the executed command
     - Record state of product (files after the command was executed)
-    - Return Metablock containing a Link object which can be can be signed
+    - Return Metadata containing a Link object which can be can be signed
       and stored to disk
 """
 import glob
 import logging
 import os
 import itertools
 import io
@@ -38,23 +38,25 @@
 import time
 
 from pathspec import PathSpec
 
 import in_toto.settings
 import in_toto.exceptions
 
+from in_toto.models._signer import GPGSigner
 from in_toto.models.link import (UNFINISHED_FILENAME_FORMAT, FILENAME_FORMAT,
     FILENAME_FORMAT_SHORT, UNFINISHED_FILENAME_FORMAT_GLOB)
+from in_toto.models.metadata import (Metadata, Envelope, Metablock)
 
 import securesystemslib.formats
 import securesystemslib.hash
 import securesystemslib.exceptions
 import securesystemslib.gpg
+from securesystemslib.signer import SSlibSigner, Signature
 
-from in_toto.models.metadata import Metablock
 
 
 # Inherits from in_toto base logger (c.f. in_toto.log)
 LOG = logging.getLogger(__name__)
 
 
 
@@ -458,43 +460,45 @@
   return {
       "stdout": stdout_str,
       "stderr": stderr_str,
       "return-value": return_code
     }
 
 
-def in_toto_mock(name, link_cmd_args):
+def in_toto_mock(name, link_cmd_args, use_dsse=False):
   """
   <Purpose>
     in_toto_run with defaults
      - Records materials and products in current directory
      - Does not sign resulting link file
      - Stores resulting link file under "<name>.link"
 
   <Arguments>
     name:
             A unique name to relate mock link metadata with a step or
             inspection defined in the layout.
     link_cmd_args:
             A list where the first element is a command and the remaining
             elements are arguments passed to that command.
+    use_dsse (optional):
+            A boolean indicating if DSSE should be used to generate metadata.
 
   <Exceptions>
     None.
 
   <Side Effects>
     Writes newly created link metadata file to disk using the filename scheme
     from link.FILENAME_FORMAT_SHORT
 
   <Returns>
-    Newly created Metablock object containing a Link object
+    Newly created Metadata object containing a Link object
 
   """
   link_metadata = in_toto_run(name, ["."], ["."], link_cmd_args,
-      record_streams=True)
+      record_streams=True, use_dsse=use_dsse)
 
   filename = FILENAME_FORMAT_SHORT.format(step_name=name)
   LOG.info("Storing unsigned link metadata to '{}'...".format(filename))
   link_metadata.dump(filename)
   return link_metadata
 
 
@@ -509,15 +513,16 @@
         "Signing key needs to be a private key.")
 
 
 def in_toto_run(name, material_list, product_list, link_cmd_args,
     record_streams=False, signing_key=None, gpg_keyid=None,
     gpg_use_default=False, gpg_home=None, exclude_patterns=None,
     base_path=None, compact_json=False, record_environment=False,
-    normalize_line_endings=False, lstrip_paths=None, metadata_directory=None):
+    normalize_line_endings=False, lstrip_paths=None, metadata_directory=None,
+    use_dsse=False):
   """Performs a supply chain step or inspection generating link metadata.
 
   Executes link_cmd_args, recording paths and hashes of files before and after
   command execution (aka. artifacts) in a link metadata file. The metadata is
   signed with the passed signing_key, a gpg key identified by its ID, or the
   default gpg key. If multiple key arguments are passed, only one key is used
   in above order of precedence. The resulting link file is written to
@@ -570,14 +575,17 @@
 
     lstrip_paths (optional): A list of path prefixes used to left-strip
         artifact paths before storing them in the resulting link metadata.
 
     metadata_directory (optional): A directory path to write the resulting link
         metadata file to. Default destination is the current working directory.
 
+    use_dsse (optional): A boolean indicating if DSSE should be used to
+        generate metadata.
+
   Raises:
     securesystemslib.exceptions.FormatError: Passed arguments are malformed.
 
     ValueError: Cannot change to base path directory.
 
     securesystemslib.exceptions.StorageError: Cannot hash artifacts.
 
@@ -599,15 +607,15 @@
   Side Effects:
     Reads artifact files from disk.
     Runs link command in subprocess.
     Calls system gpg in a subprocess, if a gpg key argument is passed.
     Writes link metadata file to disk, if any key argument is passed.
 
   Returns:
-    A Metablock object that contains the resulting link object.
+    A Metadata object that contains the resulting link object.
 
   """
   LOG.info("Running '{}'...".format(name))
 
   # Check key formats to fail early
   if signing_key:
     _check_match_signing_key(signing_key)
@@ -653,47 +661,54 @@
   if record_environment:
     environment['workdir'] = os.getcwd().replace('\\', '/')
 
   link = in_toto.models.link.Link(name=name,
       materials=materials_dict, products=products_dict, command=link_cmd_args,
       byproducts=byproducts, environment=environment)
 
-  link_metadata = Metablock(signed=link, compact_json=compact_json)
+  if use_dsse:
+    LOG.info("Generating link metadata using DSSE...")
+    link_metadata = Envelope.from_signable(link)
+  else:
+    LOG.info("Generating link metadata using Metablock...")
+    link_metadata = Metablock(signed=link, compact_json=compact_json)
 
-  signature = None
+  signer = None
   if signing_key:
     LOG.info("Signing link metadata using passed key...")
-    signature = link_metadata.sign(signing_key)
+    signer = SSlibSigner(signing_key)
 
   elif gpg_keyid:
     LOG.info("Signing link metadata using passed GPG keyid...")
-    signature = link_metadata.sign_gpg(gpg_keyid, gpg_home=gpg_home)
+    signer = GPGSigner(keyid=gpg_keyid, homedir=gpg_home)
 
   elif gpg_use_default:
     LOG.info("Signing link metadata using default GPG key ...")
-    signature = link_metadata.sign_gpg(gpg_keyid=None, gpg_home=gpg_home)
+    signer = GPGSigner(keyid=None, homedir=gpg_home)
 
   # We need the signature's keyid to write the link to keyid infix'ed filename
-  if signature:
-    signing_keyid = signature["keyid"]
+  if signer:
+    signature = link_metadata.create_signature(signer)
+    signing_keyid = signature.keyid
+
     filename = FILENAME_FORMAT.format(step_name=name, keyid=signing_keyid)
 
     if metadata_directory is not None:
       filename = os.path.join(metadata_directory, filename)
 
     LOG.info("Storing link metadata to '{}'...".format(filename))
     link_metadata.dump(filename)
 
   return link_metadata
 
 
 def in_toto_record_start(step_name, material_list, signing_key=None,
     gpg_keyid=None, gpg_use_default=False, gpg_home=None,
     exclude_patterns=None, base_path=None, record_environment=False,
-    normalize_line_endings=False, lstrip_paths=None):
+    normalize_line_endings=False, lstrip_paths=None, use_dsse=False):
   """Generates preliminary link metadata.
 
   Records paths and hashes of materials in a preliminary link metadata file.
   The metadata is signed with the passed signing_key, a gpg key identified by
   its ID, or the default gpg key. If multiple key arguments are passed, only
   one key is used in above order of precedence. At least one key argument must
   be passed. The resulting link file is written to
@@ -733,14 +748,17 @@
     normalize_line_endings (optional): A boolean indicating if line endings of
         artifacts should be normalized before hashing for cross-platform
         support.
 
     lstrip_paths (optional): A list of path prefixes used to left-strip
         artifact paths before storing them in the resulting link metadata.
 
+    use_dsse (optional): A boolean indicating if DSSE should be used to
+        generate metadata.
+
   Raises:
     securesystemslib.exceptions.FormatError: Passed arguments are malformed.
 
     ValueError: None of signing_key, gpg_keyid or gpg_use_default=True is
         passed.
 
     securesystemslib.exceptions.StorageError: Cannot hash artifacts.
@@ -798,44 +816,51 @@
   if record_environment:
     environment['workdir'] = os.getcwd().replace('\\', '/')
 
   link = in_toto.models.link.Link(name=step_name,
           materials=materials_dict, products={}, command=[], byproducts={},
           environment=environment)
 
-  link_metadata = Metablock(signed=link)
+  if use_dsse:
+    LOG.info("Generating link metadata using DSSE...")
+    link_metadata = Envelope.from_signable(link)
+  else:
+    LOG.info("Generating link metadata using Metablock...")
+    link_metadata = Metablock(signed=link)
 
   if signing_key:
     LOG.info("Signing link metadata using passed key...")
-    signature = link_metadata.sign(signing_key)
+    signer = SSlibSigner(signing_key)
 
   elif gpg_keyid:
     LOG.info("Signing link metadata using passed GPG keyid...")
-    signature = link_metadata.sign_gpg(gpg_keyid, gpg_home=gpg_home)
+    signer = GPGSigner(keyid=gpg_keyid, homedir=gpg_home)
 
   else:  # (gpg_use_default)
     LOG.info("Signing link metadata using default GPG key ...")
-    signature = link_metadata.sign_gpg(gpg_keyid=None, gpg_home=gpg_home)
+    signer = GPGSigner(keyid=None, homedir=gpg_home)
 
+  signature = link_metadata.create_signature(signer)
   # We need the signature's keyid to write the link to keyid infix'ed filename
-  signing_keyid = signature["keyid"]
+  signing_keyid = signature.keyid
 
   unfinished_fn = UNFINISHED_FILENAME_FORMAT.format(step_name=step_name,
     keyid=signing_keyid)
 
   LOG.info(
       "Storing preliminary link metadata to '{}'...".format(unfinished_fn))
   link_metadata.dump(unfinished_fn)
 
 
 
 def in_toto_record_stop(step_name, product_list, signing_key=None,
     gpg_keyid=None, gpg_use_default=False, gpg_home=None,
     exclude_patterns=None, base_path=None, normalize_line_endings=False,
-    lstrip_paths=None, metadata_directory=None):
+    lstrip_paths=None, metadata_directory=None, command=None, byproducts=None,
+    environment=None):
   """Finalizes preliminary link metadata generated with in_toto_record_start.
 
   Loads preliminary link metadata file, verifies its signature, and records
   paths and hashes as products, thus finalizing the link metadata. The metadata
   is signed with the passed signing_key, a gpg key identified by its ID, or the
   default gpg key. If multiple key arguments are passed, only one key is used
   in above order of precedence. At least one key argument must be passed and it
@@ -876,14 +901,30 @@
 
     lstrip_paths (optional): A list of path prefixes used to left-strip
         artifact paths before storing them in the resulting link metadata.
 
     metadata_directory (optional): A directory path to write the resulting link
         metadata file to. Default destination is the current working directory.
 
+    command (optional): A list consisting of a command and arguments executed
+        between in_toto_record_start() and in_toto_record_stop() to capture
+        the command ran in the resulting link metadata.
+
+    byproducts (optional): A dictionary that lists byproducts of the link
+        command execution. It should have at least the following entries
+        "stdout" (str), "stderr" (str) and "return-value" (int).
+
+    environment (optional): A dictionary to capture information about
+        the environment to be added in the resulting link metadata eg.::
+            {
+              "variables": "<list of env var KEY=value pairs>",
+              "filesystem": "<filesystem info>",
+              "workdir": "<CWD when executing link command>"
+            }
+
   Raises:
     securesystemslib.exceptions.FormatError: Passed arguments are malformed.
 
     ValueError: None of signing_key, gpg_keyid or gpg_use_default=True is
         passed.
 
     LinkNotFoundError: No preliminary link metadata file found.
@@ -957,15 +998,15 @@
           " preliminary links for step '{}' in the current working directory:"
           " {}. We need exactly one to stop recording.".format(
           step_name, ", ".join(unfinished_fn_list)))
 
     unfinished_fn = unfinished_fn_list[0]
 
   LOG.info("Loading preliminary link metadata '{}'...".format(unfinished_fn))
-  link_metadata = Metablock.load(unfinished_fn)
+  link_metadata = Metadata.load(unfinished_fn)
 
   # The file must have been signed by the same key
   # If we have a signing_key we use it for verification as well
   if signing_key:
     LOG.info(
         "Verifying preliminary link signature using passed signing key...")
     keyid = signing_key["keyid"]
@@ -982,41 +1023,65 @@
     # FIXME: Currently there is no way to know the default GPG key's keyid
     # before signing. As a workaround we extract the keyid of the preliminary
     # Link file's signature and try to export a pubkey from the gpg
     # home directory. We do this even if a gpg_keyid was specified, because gpg
     # accepts many different ids (mail, name, parts of an id, ...) but we
     # need a specific format.
     LOG.info("Verifying preliminary link signature using default gpg key...")
-    keyid = link_metadata.signatures[0]["keyid"]
+    # signatures are objects in DSSE.
+    sig = link_metadata.signatures[0]
+    if isinstance(sig, Signature):
+      keyid = sig.keyid
+    else:
+      keyid = sig["keyid"]
     gpg_pubkey = securesystemslib.gpg.functions.export_pubkey(
         keyid, gpg_home)
     verification_key = gpg_pubkey
 
   link_metadata.verify_signature(verification_key)
 
+  LOG.info("Extracting Link from metadata...")
+  link = link_metadata.get_payload()
+
   # Record products if a product path list was passed
   if product_list:
     LOG.info("Recording products '{}'...".format(", ".join(product_list)))
 
-  link_metadata.signed.products = record_artifacts_as_dict(
+  link.products = record_artifacts_as_dict(
       product_list, exclude_patterns=exclude_patterns, base_path=base_path,
       follow_symlink_dirs=True, normalize_line_endings=normalize_line_endings,
       lstrip_paths=lstrip_paths)
 
-  link_metadata.signatures = []
+  if command:
+    link.command = command
+
+  if byproducts:
+    link.byproducts = byproducts
+
+  if environment:
+    link.environment = environment
+
+  if isinstance(link_metadata, Metablock):
+    LOG.info("Generating link metadata using Metablock...")
+    link_metadata = Metablock(signed=link)
+  else:
+    LOG.info("Generating link metadata using DSSE...")
+    link_metadata = Envelope.from_signable(link)
+
   if signing_key:
     LOG.info("Updating signature with key '{:.8}...'...".format(keyid))
-    link_metadata.sign(signing_key)
+    signer = SSlibSigner(signing_key)
 
   else: # gpg_keyid or gpg_use_default
     # In both cases we use the keyid we got from verifying the preliminary
     # link signature above.
     LOG.info("Updating signature with gpg key '{:.8}...'...".format(keyid))
-    link_metadata.sign_gpg(keyid, gpg_home)
+    signer = GPGSigner(keyid=keyid, homedir=gpg_home)
 
+  link_metadata.create_signature(signer)
   fn = FILENAME_FORMAT.format(step_name=step_name, keyid=keyid)
 
   if metadata_directory is not None:
     fn = os.path.join(metadata_directory, fn)
 
   LOG.info("Storing link metadata to '{}'...".format(fn))
   link_metadata.dump(fn)
```

### Comparing `in_toto-1.3.2/in_toto/settings.py` & `in_toto-1.4.0/in_toto/settings.py`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/in_toto/user_settings.py` & `in_toto-1.4.0/in_toto/user_settings.py`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/in_toto/verifylib.py` & `in_toto-1.4.0/in_toto/verifylib.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,21 +35,23 @@
 import securesystemslib.exceptions
 
 import in_toto.settings
 import in_toto.runlib
 import in_toto.models.layout
 import in_toto.models.link
 import in_toto.formats
-from in_toto.models.metadata import Metablock
+from in_toto.models.metadata import Metadata
 from in_toto.exceptions import (RuleVerificationError, LayoutExpiredError,
     ThresholdVerificationError, BadReturnValueError,
     SignatureVerificationError)
-from securesystemslib.gpg.exceptions import KeyExpirationError
 import in_toto.rulelib
 
+import securesystemslib.formats
+from securesystemslib.gpg.exceptions import KeyExpirationError
+
 # Inherits from in_toto base logger (c.f. in_toto.log)
 LOG = logging.getLogger(__name__)
 
 RULE_TRACE = {}
 
 
 def _raise_on_bad_retval(return_value, command=None):
@@ -118,15 +120,15 @@
 
   <Returns>
     A dictionary carrying all the found metadata corresponding to the
     passed layout, e.g.:
 
     {
       <step name> : {
-        <functionary key id> : <Metablock containing a Link or Layout object>,
+        <functionary key id> : <Metadata containing a Link or Layout object>,
         ...
       }, ...
     }
 
 
   """
   steps_metadata = {}
@@ -144,15 +146,15 @@
           {}).get("subkeys", {}).keys()):
 
         filename = in_toto.models.link.FILENAME_FORMAT.format(
             step_name=step.name, keyid=keyid)
         filepath = os.path.join(link_dir_path, filename)
 
         try:
-          metadata = Metablock.load(filepath)
+          metadata = Metadata.load(filepath)
           links_per_step[keyid] = metadata
 
         except IOError:
           pass
 
     # This is only a preliminary threshold check, based on (authorized)
     # filenames, to fail early. A more thorough signature-based threshold
@@ -168,16 +170,15 @@
 
 
 def run_all_inspections(layout, persist_inspection_links):
   """
   <Purpose>
     Extracts all inspections from a passed Layout's inspect field and
     iteratively runs each command defined in the Inspection's `run` field using
-    `runlib.in_toto_run`, which returns a Metablock object containing a Link
-    object.
+    `runlib.in_toto_run`, which returns a Link object.
 
     If a link command returns non-zero the verification is aborted.
 
   <Arguments>
     layout:
             A Layout object which is used to extract the Inspections.
 
@@ -190,15 +191,15 @@
     non-int or non-zero.
 
   <Returns>
     A dictionary of metadata about the executed inspections, e.g.:
 
     {
       <inspection name> : {
-        <Metablock containing a Link object>,
+        <Link object>,
         ...
       }, ...
     }
 
   """
   inspection_links_dict = {}
   for inspection in layout.inspect:
@@ -218,15 +219,15 @@
     link = in_toto.runlib.in_toto_run(inspection.name, material_list,
         product_list, inspection.run)
 
     _raise_on_bad_retval(
         link.signed.byproducts.get("return-value"),
         inspection.run)
 
-    inspection_links_dict[inspection.name] = link
+    inspection_links_dict[inspection.name] = link.signed
 
     # If client requests persistent inspection links,
     # Dump the inspection link file for auditing
     # Keep in mind that this pollutes the verifier's (client's) filesystem.
     if persist_inspection_links:
       filename = in_toto.models.link.FILENAME_FORMAT_SHORT.format(
           step_name=inspection.name)
@@ -334,26 +335,26 @@
 
     inspection.run = new_run
     inspection.expected_materials = new_material_rules
     inspection.expected_products = new_product_rules
 
 
 
-def verify_layout_signatures(layout_metablock, keys_dict):
+def verify_metadata_signatures(metadata, keys_dict):
   """
   <Purpose>
-    Iteratively verifies the signatures of a Metablock object containing
+    Iteratively verifies the signatures of a Metadata object containing
     a Layout object for every verification key in the passed keys dictionary.
 
     Requires at least one key to be passed and requires every passed key to
     find a valid signature.
 
   <Arguments>
-    layout_metablock:
-            A Metablock object containing a Layout whose signatures are
+    metadata:
+            A Metadata object containing a Layout whose signatures are
             verified.
 
     keys_dict:
             A dictionary of keys to verify the signatures conformant with
             securesystemslib.formats.VERIFICATION_KEY_DICT_SCHEMA.
 
   <Exceptions>
@@ -373,68 +374,68 @@
   # Fail if an empty verification key dictionary was passed
   if len(keys_dict) < 1:
     raise SignatureVerificationError("Layout signature verification"
         " requires at least one key.")
 
   # Fail if any of the passed keys can't verify a signature on the Layout
   for junk, verify_key in keys_dict.items():
-    layout_metablock.verify_signature(verify_key)
+    metadata.verify_signature(verify_key)
 
 
-def verify_link_signature_thresholds(layout, chain_link_dict):
+def verify_link_signature_thresholds(layout, steps_metadata):
   """
   <Purpose>
     Verify that for each step of the layout there are at least `threshold`
-    links, signed by different authorized functionaries and return the chain
-    link dictionary containing only authorized links whose signatures
-    were successfully verified.
+    links metadata, signed by different authorized functionaries and return the
+    verified link metadata dictionary containing only authorized links metadata
+    whose signatures were successfully verified.
 
     NOTE: If the layout's key store (`layout.keys`) lists a (master) key `K`,
     with a subkey `K'`, then `K'` is authorized implicitly, to sign any link
     that `K` is authorized to sign. In other words, the trust in a master key
     extends to the trust in a subkey. The inverse is not true.
 
   <Arguments>
     layout:
             A Layout object whose Steps are extracted and verified.
 
-    chain_link_dict:
+    steps_metadata:
             A dictionary containing link metadata per functionary per step,
             e.g.:
             {
               <link name> : {
-                <functionary key id> : <Metablock containing a Link or Layout
+                <functionary key id> : <Metadata containing a Link or Layout
                                         object>,
                 ...
               }, ...
             }
 
   <Exceptions>
     ThresholdVerificationError
             If any of the steps of the passed layout does not have enough
             (`step.threshold`) links signed by different authorized
             functionaries.
 
   <Returns>
-    A chain_link_dict containing only links with valid signatures created by
+    A steps_metadata containing only links with valid signatures created by
     authorized functionaries.
 
   """
   # Create an inverse keys-subkeys dictionary, with subkey keyids as
   # dictionary keys and main keys as dictionary values. This will be
   # required below to assess main-subkey trust delegations.
   # We assume that a given subkey can only belong to one master key
   # TODO: Is this a safe assumption? Should we assert for it?
   main_keys_for_subkeys = {}
   for main_key in list(layout.keys.values()):
     for sub_keyid in main_key.get("subkeys", []):
       main_keys_for_subkeys[sub_keyid] = main_key
 
   # Dict for valid and authorized links of all steps of the layout
-  verfied_chain_link_dict = {}
+  verified_steps_metadata = {}
 
   # For each step of the layout check the signatures of corresponding links.
   # Consider only links where the signature is valid and keys are authorized,
   # and discard others.
   # Only count one of multiple links signed with different subkeys of a main
   # key towards link threshold.
   # Only proceed with final product verification if threshold requirements are
@@ -442,15 +443,15 @@
   for step in layout.steps:
     # Dict for valid and authorized links of a given step
     verified_key_link_dict = {}
     # List of used keyids
     used_main_keyids = []
 
     # Do per step link threshold verification
-    for link_keyid, link in chain_link_dict.get(step.name, {}).items():
+    for link_keyid, link in steps_metadata.get(step.name, {}).items():
       # Iterate over authorized keyids to find a key or subkey corresponding
       # to the given link and check if the link's keyid is authorized.
       # Subkeys of authorized main keys are authorized implicitly.
       for authorized_keyid in step.pubkeys:
 
         authorized_key = layout.keys.get(authorized_keyid)
         main_key_for_subkey = main_keys_for_subkeys.get(authorized_keyid)
@@ -499,32 +500,31 @@
 
       # Keep only links with valid and authorized signature
       verified_key_link_dict[link_keyid] = link
 
     # For each step, verify that we have enough validly signed links from
     # distinct authorized functionaries. Links signed by different subkeys of
     # the same main key are counted only once towards the threshold.
-    valid_authorized_links_cnt = (len(verified_key_link_dict) -
-        (len(used_main_keyids) - len(set(used_main_keyids))))
+    valid_authorized_links_cnt = len(set(used_main_keyids))
     # TODO: To guarantee that links are signed by different functionaries
     # we rely on the layout to not carry duplicate verification keys under
     # different dictionary keys, e.g. {keyid1: KEY1, keyid2: KEY1}
     # Maybe we should add such a check to the layout validation? Or here?
     if valid_authorized_links_cnt < step.threshold:
       raise ThresholdVerificationError("Step '{}' requires at least '{}' links"
           " validly signed by different authorized functionaries. Only"
           " found '{}'".format(step.name, step.threshold,
           valid_authorized_links_cnt))
 
     # Add all good links of this step to the dictionary of links of all steps
-    verfied_chain_link_dict[step.name] = verified_key_link_dict
+    verified_steps_metadata[step.name] = verified_key_link_dict
 
   # Threshold verification succeeded, return valid and authorized links for
   # further verification
-  return verfied_chain_link_dict
+  return verified_steps_metadata
 
 def verify_command_alignment(command, expected_command):
   """
   <Purpose>
     Checks if a run command aligns with an expected command. The commands align
     if all of their elements are equal. If alignment fails, a warning is
     printed.
@@ -568,15 +568,15 @@
             A Layout object to extract the expected commands from.
 
     chain_link_dict:
             A dictionary containing link metadata per functionary per step,
             e.g.:
             {
               <link name> : {
-                <functionary key id> : <Metablock containing a Link object>,
+                <functionary key id> : <Link object>,
                 ...
               }, ...
             }
 
   <Exceptions>
     None.
 
@@ -592,15 +592,15 @@
     # FIXME: I think we could do this for one link per step only
     # providing that we verify command alignment AFTER threshold equality
     for keyid, link in key_link_dict.items():
       LOG.info("Verifying command alignment for '{0}'...".format(
           in_toto.models.link.FILENAME_FORMAT.format(step_name=step.name,
               keyid=keyid)))
 
-      command = link.signed.command
+      command = link.command
       verify_command_alignment(command, expected_command)
 
 
 def verify_match_rule(rule_data, artifacts_queue, source_artifacts, links):
   """
   <Purpose>
     Filters artifacts from artifact queue using rule pattern and optional rule
@@ -627,15 +627,15 @@
 
     source_artifacts:
             All artifacts of the source item (including hashes).
 
     links:
             A dictionary containing link metadata per step or inspection, e.g.:
             {
-              <link name> : <Metablock containing a link object>,
+              <link name> : <Link object>,
               ...
             }
 
   <Exceptions>
     None.
 
   <Side Effects>
@@ -649,15 +649,15 @@
 
   # The rule can only consume artifacts if the destination link exists
   dest_link = links.get(rule_data["dest_name"])
   if not dest_link:
     return consumed
 
   # Extract destination artifacts from destination link
-  dest_artifacts = getattr(dest_link.signed, rule_data["dest_type"])
+  dest_artifacts = getattr(dest_link, rule_data["dest_type"])
 
   # Filter part 1 - Filter artifacts using optional source prefix, and subtract
   # prefix before filtering with rule pattern (see filter part 2) to prevent
   # globbing in the prefix.
   if rule_data["source_prefix"]:
     filtered_source_paths = []
     # Add trailing slash to source prefix if it does not exist
@@ -998,15 +998,15 @@
     rules:
             The list of rules (material or product rules) for the item being
             verified.
 
     links:
             A dictionary containing link metadata per step or inspection, e.g.:
             {
-              <link name> : <Metablock containing a link>,
+              <link name> : <Link object>,
               ...
             }
 
   <Exceptions>
     FormatError
         if source_type is not "materials" or "products", or
         if a rule in the passed list of rules does not conform with any rule
@@ -1023,25 +1023,25 @@
   if source_type not in ["materials", "products"]:
     raise securesystemslib.exceptions.FormatError(
         "Argument 'source_type' of function 'verify_item_rules' has to be "
         "one of 'materials' or 'products'. Got: '{}'".format(source_type))
 
   # Create shortcuts to item's materials and products (including hashes),
   # required to verify "modify" and "match" rules.
-  materials_dict = links[source_name].signed.materials
-  products_dict = links[source_name].signed.products
+  materials_dict = links[source_name].materials
+  products_dict = links[source_name].products
 
   # All other rules only require materials or products paths (without hashes)
   materials_paths = set(materials_dict.keys())
   products_paths = set(products_dict.keys())
 
   # Depending on the source type we create the artifact queue from the item's
   # materials or products and use it to keep track of (not) consumed artifacts.
   # The queue also only contains aritfact keys (without hashes)
-  artifacts = getattr(links[source_name].signed, source_type)
+  artifacts = getattr(links[source_name], source_type)
   artifacts_queue = set(artifacts.keys())
 
   # Reset and re-populate rule traceback info dict for a rich error message
   RULE_TRACE.clear()
   RULE_TRACE["source_name"] = source_name
   RULE_TRACE["source_type"] = source_type
   RULE_TRACE["materials"] = list(materials_dict)
@@ -1111,15 +1111,15 @@
     items:
             A list containing Step or Inspection objects whose material
             and product rules will be verified.
 
     links:
             A dictionary containing link metadata per step or inspection, e.g.:
             {
-              <link name> : <Metablock containing a Link object>,
+              <link name> : <Link object>,
               ...
             }
 
   <Exceptions>
     None.
 
   <Side Effects>
@@ -1150,15 +1150,15 @@
             The layout whose step thresholds are being verified
 
     chain_link_dict:
             A dictionary containing link metadata per functionary per step,
             e.g.:
             {
               <link name> : {
-                <functionary key id> : <Metablock containing a Link object>,
+                <functionary key id> : <Link object>,
                 ...
               }, ...
             }
 
   <Exceptions>
     ThresholdVerificationError
         If there are not enough (threshold) links for a steps
@@ -1196,16 +1196,16 @@
     reference_keyid = list(key_link_dict.keys())[0]
     reference_link = key_link_dict[reference_keyid]
 
     # Iterate over all links to compare their properties with a reference_link
     for keyid, link in key_link_dict.items():
       # TODO: Do we only care for artifacts, or do we want to
       # assert equality of other properties as well?
-      if (reference_link.signed.materials != link.signed.materials or
-          reference_link.signed.products != link.signed.products):
+      if (reference_link.materials != link.materials or
+          reference_link.products != link.products):
         raise ThresholdVerificationError("Links '{0}' and '{1}' have different"
             " artifacts!".format(
                 in_toto.models.link.FILENAME_FORMAT.format(
                     step_name=step.name, keyid=reference_keyid),
                 in_toto.models.link.FILENAME_FORMAT.format(
                     step_name=step.name, keyid=keyid)))
 
@@ -1224,15 +1224,15 @@
             threshold will be verified.
 
     chain_link_dict:
             A dictionary containing link metadata per functionary per step,
             e.g.:
             {
               <link name> : {
-                <functionary key id> : <Metablock containing a Link object>,
+                <functionary key id> : <Link object>,
                 ...
               }, ...
             }
 
   <Exceptions>
     None.
 
@@ -1252,31 +1252,32 @@
     # take one exemplary link (e.g. the first in the step_link_dict)
     # form the reduced_chain_link_dict to return
     reduced_chain_link_dict[step_name] = list(key_link_dict.values())[0]
 
   return reduced_chain_link_dict
 
 
-def verify_sublayouts(layout, chain_link_dict, superlayout_link_dir_path):
+def verify_sublayouts(layout, steps_metadata, superlayout_link_dir_path):
   """
   <Purpose>
-    Checks if any step has been delegated by the functionary, recurses into
-    the delegation and replaces the layout object in the chain_link_dict
-    by an equivalent link object.
+    Extracts link or layout object for each step in steps_metadata. Checks if
+    any step has been delegated by the functionary, recurses into the
+    delegation, and replaces the layout object with an equivalent link object.
+    Returns the extracted link objects in a dict called chain_link_dict.
 
   <Arguments>
     layout:
             The layout specified by the project owner.
 
-    chain_link_dict:
+    steps_metadata:
             A dictionary containing link metadata per functionary per step,
             e.g.:
             {
               <link name> : {
-                <functionary key id> : <Metablock containing a Link or Layout
+                <functionary key id> : <Metadata containing a Link or Layout
                                           object>,
                 ...
               }, ...
             }
 
     superlayout_link_dir_path:
             A path to a directory, where links of the superlayout are loaded
@@ -1287,30 +1288,36 @@
   <Exceptions>
     raises an Exception if verification of the delegated step fails.
 
   <Side Effects>
     None.
 
   <Returns>
-    The passed dictionary containing link metadata per functionary per step,
-    with layouts replaced with summary links.
+    The passed dictionary containing Link objects instead of metadata per
+    functionary per step, with layouts replaced with summary links.
     e.g.:
     {
       <link name> : {
-        <functionary key id> : <Metablock containing a Link object>,
+        <functionary key id> : <Link object>,
         ...
       }, ...
     }
 
   """
-  for step_name, key_link_dict in chain_link_dict.items():
+  chain_link_dict = {}
 
-    for keyid, link in key_link_dict.items():
+  for step_name, metadata_dict in steps_metadata.items():
+
+    key_link_dict = {}
+    for keyid, metadata in metadata_dict.items():
+
+      payload = metadata.get_payload()
+
+      if payload.type_ == "layout":
 
-      if link.type_ == "layout":
         LOG.info("Verifying sublayout {}...".format(step_name))
         layout_key_dict = {}
 
         # Retrieve the entire key object for the keyid
         # corresponding to the link
         layout_key_dict = {keyid: layout.keys.get(keyid)}
 
@@ -1322,20 +1329,23 @@
             name=step_name, keyid=keyid)
 
         sublayout_link_dir_path = os.path.join(
             superlayout_link_dir_path, sub_link_dir)
 
         # Make a recursive call to in_toto_verify with the
         # layout and the extracted key object
-        summary_link = in_toto_verify(link, layout_key_dict,
+        summary_link = in_toto_verify(metadata, layout_key_dict,
             link_dir_path=sublayout_link_dir_path, step_name=step_name)
 
-        # Replace the layout object in the passed chain_link_dict
-        # with the link file returned by in-toto-verify
-        key_link_dict[keyid] = summary_link
+        # Replace the layout object with the link object returned
+        # by in-toto-verify
+        payload = summary_link
+
+      key_link_dict[keyid] = payload
+    chain_link_dict[step_name] = key_link_dict
 
   return chain_link_dict
 
 
 def get_summary_link(layout, reduced_chain_link_dict, name):
   """
   <Purpose>
@@ -1352,51 +1362,51 @@
     layout:
             The layout specified by the project owner.
 
     reduced_chain_link_dict:
             A dictionary containing link metadata per step,
             e.g.:
             {
-              <link name> : <Metablock containing a Link object>,
+              <link name> : <Link object>,
               ...
             }
     name:
             The name that the summary link will be associated with.
 
   <Exceptions>
     None.
 
   <Side Effects>
     None.
 
   <Returns>
-    A Metablock object containing a Link which summarizes the materials and
-    products of the overall software supply chain.
+    A Link object which summarizes the materials and products of the overall
+    software supply chain.
 
   """
   # Create empty link object
   summary_link = in_toto.models.link.Link()
 
   # Take first and last link in the order the corresponding
   # steps appear in the layout, if there are any.
   if len(layout.steps) > 0:
     first_step_link = reduced_chain_link_dict[layout.steps[0].name]
     last_step_link = reduced_chain_link_dict[layout.steps[-1].name]
 
-    summary_link.materials = first_step_link.signed.materials
+    summary_link.materials = first_step_link.materials
     summary_link.name = name
 
-    summary_link.products = last_step_link.signed.products
-    summary_link.byproducts = last_step_link.signed.byproducts
-    summary_link.command = last_step_link.signed.command
+    summary_link.products = last_step_link.products
+    summary_link.byproducts = last_step_link.byproducts
+    summary_link.command = last_step_link.command
 
-  return Metablock(signed=summary_link)
+  return summary_link
 
 
-def in_toto_verify(layout, layout_key_dict, link_dir_path=".",
+def in_toto_verify(metadata, layout_key_dict, link_dir_path=".",
     substitution_parameters=None, step_name="",
     persist_inspection_links=True):
   """Performs complete in-toto supply chain verification for a final product.
 
   The verification procedure consists of the following activities, performed in
   the given order:
 
@@ -1412,15 +1422,15 @@
       https://github.com/in-toto/docs/blob/master/in-toto-spec.md#431-steps
   8.  Verify threshold artifact constraints
   9.  Process step product and material rules
   10. Execute inspection commands and generate inspection links
   11. Process inspection product and material rules
 
   Arguments:
-    layout: A Metablock object that contains a Layout object to be verified.
+    metadata: A Metadata object that contains a Layout object to be verified.
 
     layout_key_dict: A public key dictionary. The verification routine requires
         at least one key, and a valid signature on the layout for each key.
 
     link_dir_path (optional): A directory path to link metadata files. The
         expected filename format for link metadata files is
         ``STEP-NAME.KEYID-PREFIX.link``. Link metadata files for a sublayout
@@ -1461,43 +1471,45 @@
     BadReturnValueError: An inspection command returns a non-zero value.
 
   Side Effects:
     Reads link metadata files from disk.
     Runs inspection commands in subprocess.
 
   Returns:
-    A Metablock object that contains a Link object, which summarizes the
-    materials and products of the overall software supply chain. This is mostly
-    useful during recursive sublayout verification.
+    A Link object, which summarizes the materials and products of the overall
+    software supply chain. This is mostly useful during recursive sublayout
+    verification.
 
   """
-  LOG.info("Verifying layout signatures...")
-  verify_layout_signatures(layout, layout_key_dict)
+
+  LOG.info("Verifying layout metadata signatures...")
+  verify_metadata_signatures(metadata, layout_key_dict)
 
   # For the rest of the verification we only care about the layout payload
   # (Layout) that carries all the information and not about the layout
   # container (Metablock) that also carries the signatures
-  layout = layout.signed
+  LOG.info("Extracting layout from metadata...")
+  layout = metadata.get_payload()
 
   LOG.info("Verifying layout expiration...")
   verify_layout_expiration(layout)
 
   # If there are parameters sent to the translation layer, substitute them
   if substitution_parameters is not None:
     LOG.info('Performing parameter substitution...')
     substitute_parameters(layout, substitution_parameters)
 
   LOG.info("Reading link metadata files...")
-  chain_link_dict = load_links_for_layout(layout, link_dir_path)
+  steps_metadata = load_links_for_layout(layout, link_dir_path)
 
   LOG.info("Verifying link metadata signatures...")
-  chain_link_dict = verify_link_signature_thresholds(layout, chain_link_dict)
+  steps_metadata = verify_link_signature_thresholds(layout, steps_metadata)
 
   LOG.info("Verifying sublayouts...")
-  chain_link_dict = verify_sublayouts(layout, chain_link_dict, link_dir_path)
+  chain_link_dict = verify_sublayouts(layout, steps_metadata, link_dir_path)
 
   LOG.info("Verifying alignment of reported commands...")
   verify_all_steps_command_alignment(layout, chain_link_dict)
 
   LOG.info("Verifying threshold constraints...")
   verify_threshold_constraints(layout, chain_link_dict)
   reduced_chain_link_dict = reduce_chain_links(chain_link_dict)
```

### Comparing `in_toto-1.3.2/in_toto/models/_signer.py` & `in_toto-1.4.0/in_toto/models/_signer.py`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/in_toto/models/common.py` & `in_toto-1.4.0/in_toto/models/common.py`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/in_toto/models/layout.py` & `in_toto-1.4.0/in_toto/models/layout.py`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/in_toto/models/link.py` & `in_toto-1.4.0/in_toto/models/link.py`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/__init__.py` & `in_toto-1.4.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/common.py` & `in_toto-1.4.0/tests/common.py`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/runtests.py` & `in_toto-1.4.0/tests/runtests.py`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/test_common_args.py` & `in_toto-1.4.0/tests/test_common_args.py`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/test_in_toto_keygen.py` & `in_toto-1.4.0/tests/test_in_toto_keygen.py`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/test_in_toto_mock.py` & `in_toto-1.4.0/tests/test_in_toto_mock.py`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/test_in_toto_record.py` & `in_toto-1.4.0/tests/test_in_toto_record.py`

 * *Files 17% similar despite different names*

```diff
@@ -223,9 +223,69 @@
     args = ["--step-name", "no-link", "--key", self.rsa_key_path]
     self.assert_cli_sys_exit(["stop"] + args, 1)
 
     args = ["--step-name", "no-link", "--key", self.ed25519_key_path, "--key-type", "ed25519"]
     self.assert_cli_sys_exit(["stop"] + args, 1)
 
 
+class TestInTotoRecordToolWithDSSE(CliTestCase, TmpDirMixin, GPGKeysMixin, GenKeysMixin):
+  """Test in_toto_record's main() with --use-dsse argument - requires sys.argv
+  patching; and in_toto_record_start/in_toto_record_stop - calls runlib and
+  error logs/exits on Exception. """
+  cli_main_func = staticmethod(in_toto_record_main)
+
+  @classmethod
+  def setUpClass(self):
+    """Create and change into temporary directory,
+    generate key pair, dummy artifact and base arguments. """
+    self.set_up_test_dir()
+    self.set_up_keys()
+
+    self.test_artifact1 = "test_artifact1"
+    self.test_artifact2 = "test_artifact2"
+    Path(self.test_artifact1).touch()
+    Path(self.test_artifact2).touch()
+
+
+  @classmethod
+  def tearDownClass(self):
+    self.tear_down_test_dir()
+
+
+  def test_start_stop(self):
+    """Test CLI command record start/stop with various arguments. """
+
+    # Start/stop recording using rsa key
+    args = ["--step-name", "test1", "--key", self.rsa_key_path, "--use-dsse"]
+    self.assert_cli_sys_exit(["start"] + args, 0)
+    self.assert_cli_sys_exit(["stop"] + args, 0)
+
+    # Start/stop with recording one artifact using rsa key
+    args = ["--step-name", "test2", "--key", self.rsa_key_path, "--use-dsse"]
+    self.assert_cli_sys_exit(["start"] + args + ["--materials",
+      self.test_artifact1], 0)
+    self.assert_cli_sys_exit(["stop"] + args + ["--products",
+      self.test_artifact1], 0)
+
+    # Start/stop with excluding one artifact using rsa key
+    args = ["--step-name", "test2.5", "--key", self.rsa_key_path, "--use-dsse"]
+    self.assert_cli_sys_exit(["start"] + args + ["--materials",
+      self.test_artifact1, "--exclude", "test*"], 0)
+    self.assert_cli_sys_exit(["stop"] + args + ["--products",
+      self.test_artifact1, "--exclude", "test*"], 0)
+
+    # Start/stop with base-path using rsa key
+    args = ["--step-name", "test2.6", "--key", self.rsa_key_path, "--base-path",
+      self.test_dir, "--use-dsse"]
+    self.assert_cli_sys_exit(["start"] + args, 0)
+    self.assert_cli_sys_exit(["stop"] + args, 0)
+
+    # Start/stop with recording multiple artifacts using rsa key
+    args = ["--step-name", "test3", "--key", self.rsa_key_path, "--use-dsse"]
+    self.assert_cli_sys_exit(["start"] + args + ["--materials",
+      self.test_artifact1, self.test_artifact2], 0)
+    self.assert_cli_sys_exit(["stop"] + args + ["--products",
+      self.test_artifact2, self.test_artifact2], 0)
+
+
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `in_toto-1.3.2/tests/test_in_toto_run.py` & `in_toto-1.4.0/tests/test_in_toto_run.py`

 * *Files 21% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import unittest
 import glob
 import tempfile
 
 from pathlib import Path
 from unittest import mock
 
-from in_toto.models.metadata import Metablock
+from in_toto.models.metadata import Metadata, Metablock
 from in_toto.in_toto_run import main as in_toto_run_main
 from in_toto.models.link import FILENAME_FORMAT
 
 from tests.common import CliTestCase, TmpDirMixin, GPGKeysMixin, GenKeysMixin
 
 import securesystemslib.interface # pylint: disable=unused-import
 
@@ -271,9 +271,123 @@
     self.assert_cli_sys_exit(args, 1)
     self.assertFalse(os.path.exists(self.test_link_rsa_enc))
 
     args = ["-n", self.test_step, "--key", self.ed25519_key_enc_path, "-x"]
     self.assert_cli_sys_exit(args, 1)
     self.assertFalse(os.path.exists(self.test_link_ed25519_enc))
 
+
+class TestInTotoRunToolWithDSSE(CliTestCase, TmpDirMixin, GPGKeysMixin, GenKeysMixin):
+  """Test in_toto_run's main() with --use-dsse argument - requires sys.argv
+  patching; and in_toto_run- calls runlib and error logs/exits on Exception."""
+  cli_main_func = staticmethod(in_toto_run_main)
+
+  @classmethod
+  def setUpClass(self):
+    """Create and change into temporary directory,
+    generate key pair, dummy artifact and base arguments. """
+    self.set_up_test_dir()
+    self.set_up_gpg_keys()
+    self.set_up_keys()
+
+    self.test_step = "test_step"
+    self.test_link_rsa = FILENAME_FORMAT.format(
+        step_name=self.test_step, keyid=self.rsa_key_id)
+    self.test_link_ed25519 = FILENAME_FORMAT.format(
+        step_name=self.test_step, keyid=self.ed25519_key_id)
+    self.test_link_rsa_enc = FILENAME_FORMAT.format(
+        step_name=self.test_step, keyid=self.rsa_key_enc_id)
+    self.test_link_ed25519_enc = FILENAME_FORMAT.format(
+        step_name=self.test_step, keyid=self.ed25519_key_enc_id)
+
+    self.test_artifact = "test_artifact"
+    Path(self.test_artifact).touch()
+
+  @classmethod
+  def tearDownClass(self):
+    self.tear_down_test_dir()
+
+  def tearDown(self):
+    for link in glob.glob("*.link"):
+      os.remove(link)
+
+  def test_main_required_args(self):
+    """Test CLI command with required arguments. """
+
+    args = ["--step-name", self.test_step, "--key", self.rsa_key_path,
+        "--use-dsse", "--", "python", "--version"]
+
+    self.assert_cli_sys_exit(args, 0)
+    self.assertTrue(os.path.exists(self.test_link_rsa))
+
+
+  def test_main_optional_args(self):
+    """Test CLI command with optional arguments. """
+
+    named_args = ["--step-name", self.test_step, "--key",
+        self.rsa_key_path, "--materials", self.test_artifact, "--products",
+        self.test_artifact, "--record-streams", "--use-dsse"]
+    positional_args = ["--", "python", "--version"]
+
+    # Test and assert recorded artifacts
+    args1 = named_args + positional_args
+    self.assert_cli_sys_exit(args1, 0)
+    metadata = Metadata.load(self.test_link_rsa)
+    link = metadata.get_payload()
+    self.assertTrue(self.test_artifact in
+        list(link.materials.keys()))
+    self.assertTrue(self.test_artifact in
+        list(link.products.keys()))
+
+    # Test and assert exlcuded artifacts
+    args2 = named_args + ["--exclude", "*test*"] + positional_args
+    self.assert_cli_sys_exit(args2, 0)
+    link = Metadata.load(self.test_link_rsa).get_payload()
+    self.assertFalse(link.materials)
+    self.assertFalse(link.products)
+
+    # Test with base path
+    args3 = named_args + ["--base-path", self.test_dir] + positional_args
+    self.assert_cli_sys_exit(args3, 0)
+    link = Metadata.load(self.test_link_rsa).get_payload()
+    self.assertListEqual(list(link.materials.keys()),
+        [self.test_artifact])
+    self.assertListEqual(list(link.products.keys()),
+        [self.test_artifact])
+
+    # Test with bogus base path
+    args4 = named_args + ["--base-path", "bogus/path"] + positional_args
+    self.assert_cli_sys_exit(args4, 1)
+
+    # Test with lstrip path
+    strip_prefix = self.test_artifact[:-1]
+    args5 = named_args + ["--lstrip-paths", strip_prefix] + positional_args
+    self.assert_cli_sys_exit(args5, 0)
+    link = Metadata.load(self.test_link_rsa).get_payload()
+    self.assertListEqual(list(link.materials.keys()),
+        [self.test_artifact[len(strip_prefix):]])
+    self.assertListEqual(list(link.products.keys()),
+        [self.test_artifact[len(strip_prefix):]])
+
+
+  def test_main_with_default_gpg_key(self):
+    """Test CLI command with default gpg key."""
+    args = ["-n", self.test_step,
+            "--gpg", "--gpg-home", self.gnupg_home, "--use-dsse",
+            "--", "python", "--version"]
+
+    self.assert_cli_sys_exit(args, 1)
+
+
+  def test_main_no_command_arg(self):
+    """Test CLI command with --no-command argument. """
+
+    args = ["in_toto_run.py", "--step-name", self.test_step, "--key",
+        self.rsa_key_path, "--no-command", "--use-dsse"]
+
+    self.assert_cli_sys_exit(args, 0)
+
+    self.assertTrue(os.path.exists(self.test_link_rsa))
+
+
 if __name__ == "__main__":
   unittest.main()
```

### Comparing `in_toto-1.3.2/tests/test_in_toto_sign.py` & `in_toto-1.4.0/tests/test_in_toto_sign.py`

 * *Files 25% similar despite different names*

```diff
@@ -326,9 +326,150 @@
       f.write(json.dumps({}).encode("utf-8"))
 
     self.assert_cli_sys_exit([
         "-f", "tmp.json",
         "-k", "key-not-used",
         ], 2)
 
+class TestInTotoSignToolWithDSSE(CliTestCase, TmpDirMixin, GPGKeysMixin, GenKeysMixin):
+  """Test in_toto_sign's main() for dsse metadata files - requires sys.argv
+  patching; error logs/exits on Exception. """
+  cli_main_func = staticmethod(in_toto_sign_main)
+
+  @classmethod
+  def setUpClass(self):
+    # Find demo files
+    demo_files = os.path.join(
+        os.path.dirname(os.path.realpath(__file__)), "demo_files")
+
+    # Demo DSSE Metadata Files
+    demo_dsse_files = os.path.join(
+        os.path.dirname(os.path.realpath(__file__)), "demo_dsse_files")
+
+    # Create and change into temporary directory
+    self.set_up_test_dir()
+    self.set_up_gpg_keys()
+    self.set_up_keys()
+
+    # Copy demo files to temp dir
+    for file_path in os.listdir(demo_files):
+      shutil.copy(os.path.join(demo_files, file_path), self.test_dir)
+
+    # Copy demo DSSE files to temp dir
+    for file_path in os.listdir(demo_dsse_files):
+      shutil.copy(os.path.join(demo_dsse_files, file_path), self.test_dir)
+
+    self.layout_path = "demo.layout.template"
+    self.link_path = "package.2f89b927.link"
+    self.alice_path = "alice"
+    self.alice_pub_path = "alice.pub"
+    self.bob_path = "bob"
+    self.bob_pub_path = "bob.pub"
+    self.carl_path = "carl"
+    self.carl_pub_path = "carl.pub"
+    self.danny_path = "danny"
+    self.danny_pub_path = "danny.pub"
+
+  @classmethod
+  def tearDownClass(self):
+    self.tear_down_test_dir()
+
+
+  def test_sign_and_verify(self):
+    """Test signing and verifying Layout and Link metadata with
+    different combinations of arguments. """
+
+    # Sign Layout with multiple keys and write to "tmp.layout"
+    self.assert_cli_sys_exit([
+        "-f", self.layout_path,
+        "-k", self.alice_path, self.bob_path,
+        "-o", "tmp.layout",
+        ], 0)
+
+    # Verify "tmp.layout" (requires all keys)
+    self.assert_cli_sys_exit([
+        "-f", "tmp.layout",
+        "-k", self.alice_pub_path, self.bob_pub_path,
+        "--verify",
+        ], 0)
+
+    # Sign Layout "tmp.layout", appending new signature, write to "tmp.layout"
+    self.assert_cli_sys_exit([
+        "-f", "tmp.layout",
+        "-k", self.carl_path,
+        "-a"
+        ], 0)
+
+    # Verify "tmp.layout" (has three signatures now)
+    self.assert_cli_sys_exit([
+        "-f", "tmp.layout",
+        "-k", self.alice_pub_path, self.bob_pub_path, self.carl_pub_path,
+        "--verify"
+        ], 0)
+
+    # Sign Layout "tmp.layout" with ed25519 key, appending new signature,
+    # write to "tmp.layout"
+    self.assert_cli_sys_exit([
+        "-f", "tmp.layout",
+        "-k", self.danny_path,
+        "-t", "ed25519",
+        "-a"
+        ], 0)
+
+    # Verify "tmp.layout" (has four signatures now)
+    self.assert_cli_sys_exit([
+        "-f", "tmp.layout",
+        "-k", self.alice_pub_path, self.bob_pub_path, self.carl_pub_path,
+        self.danny_pub_path,
+        "-t", "rsa", "rsa", "rsa", "ed25519",
+        "--verify"
+        ], 0)
+
+    # Sign Link, replacing old signature
+    # and write to same file as input
+    self.assert_cli_sys_exit([
+        "-f", self.link_path,
+        "-k", self.bob_path,
+        "-o", self.link_path,
+        ], 0)
+
+    # Verify Link
+    self.assert_cli_sys_exit([
+        "-f", self.link_path,
+        "-k", self.bob_pub_path,
+        "--verify"
+        ], 0)
+
+    # Replace signature to Link and store to new file using passed
+    # key's (alice) id as infix
+    self.assert_cli_sys_exit([
+        "-f", self.link_path,
+        "-k", self.alice_path
+        ], 0)
+    # Verify Link with alice's keyid as infix
+    self.assert_cli_sys_exit([
+        "-f", "package.556caebd.link",
+        "-k", self.alice_pub_path,
+        "--verify"
+        ], 0)
+
+
+  def test_fail_verification(self):
+    """Fail signature verification. """
+    # Fail with wrong key (not used for signing)
+    self.assert_cli_sys_exit([
+        "-f", self.layout_path,
+        "-k", self.carl_pub_path,
+        "--verify"
+        ], 1)
+
+    # Fail with wrong gpg keyid (not used for signing)
+    self.assert_cli_sys_exit([
+        "-f", self.layout_path,
+        "-g", self.gpg_key_0C8A17,
+        "--gpg-home", self.gnupg_home,
+        "--verify"
+        ], 2)
+
+
 if __name__ == "__main__":
   unittest.main()
```

### Comparing `in_toto-1.3.2/tests/test_in_toto_verify.py` & `in_toto-1.4.0/tests/test_in_toto_verify.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,19 +21,20 @@
 
 """
 
 import os
 import unittest
 import shutil
 
-from in_toto.models.metadata import Metablock
+from in_toto.models.metadata import Metadata
 from in_toto.in_toto_verify import main as in_toto_verify_main
 from securesystemslib.interface import (import_rsa_privatekey_from_file,
     import_ed25519_privatekey_from_file)
 from securesystemslib.gpg.constants import have_gpg
+from securesystemslib.signer import SSlibSigner
 
 from tests.common import CliTestCase, TmpDirMixin, GPGKeysMixin
 
 
 
 class TestInTotoVerifyTool(CliTestCase, TmpDirMixin):
   """
@@ -76,15 +77,15 @@
     # Copy demo files to temp dir
     for fn in os.listdir(demo_files):
       shutil.copy(os.path.join(demo_files, fn), self.test_dir)
 
     shutil.copytree(scripts_directory, 'scripts')
 
     # Load layout template
-    layout_template = Metablock.load("demo.layout.template")
+    layout_template = Metadata.load("demo.layout.template")
 
     # Store layout paths to be used in tests
     self.layout_single_signed_path = "single-signed.layout"
     self.layout_double_signed_path = "double-signed.layout"
 
     # Import layout signing keys
     alice = import_rsa_privatekey_from_file("alice")
@@ -147,14 +148,121 @@
 
     # Fail with an explicit link directory, where no links are found
     args = ["--layout", self.layout_single_signed_path,
         "--layout-keys", self.alice_path, "--link-dir", "bad-link-dir"]
     self.assert_cli_sys_exit(args, 1)
 
 
+class TestInTotoVerifyToolWithDSSE(CliTestCase, TmpDirMixin):
+  """
+  Tests
+    - in_toto_verify's main() - requires sys.argv patching;
+    - in_toto_verify - calls verifylib.in_toto_verify and error logs/exits
+      in case of a raised Exception.
+
+  Uses in-toto demo supply chain link metadata files and basic layout for
+  verification:
+
+  Copies the basic layout for different test scenarios:
+    - signed layout
+    - multiple signed layout (using two project owner keys)
+  """
+  cli_main_func = staticmethod(in_toto_verify_main)
+
+
+  @classmethod
+  def setUpClass(self):
+    """Creates and changes into temporary directory.
+    Copies demo files to temp dir...
+      - owner/functionary key pairs
+      - *.link metadata files
+      - layout template (not signed, no expiration date)
+      - final product
+
+    ...and dumps various layouts for different test scenarios
+    """
+
+    # Find demo files
+    demo_files = os.path.join(
+        os.path.dirname(os.path.realpath(__file__)), "demo_files")
+
+    # Demo DSSE Metadata Files
+    demo_dsse_files = os.path.join(
+        os.path.dirname(os.path.realpath(__file__)), "demo_dsse_files")
+
+    # find where the scripts directory is located.
+    scripts_directory = os.path.join(
+        os.path.dirname(os.path.realpath(__file__)), "scripts")
+
+    self.set_up_test_dir()
+
+    # Copy demo files to temp dir
+    for fn in os.listdir(demo_files):
+      shutil.copy(os.path.join(demo_files, fn), self.test_dir)
+
+    for fn in os.listdir(demo_dsse_files):
+      shutil.copy(os.path.join(demo_dsse_files, fn), self.test_dir)
+
+    shutil.copytree(scripts_directory, 'scripts')
+
+    # Load layout template
+    layout_template = Metadata.load("demo.layout.template")
+
+    # Store layout paths to be used in tests
+    self.layout_single_signed_path = "single-signed.layout"
+    self.layout_double_signed_path = "double-signed.layout"
+
+    # Import layout signing keys
+    alice = import_rsa_privatekey_from_file("alice")
+    bob = import_rsa_privatekey_from_file("bob")
+    self.alice_path = "alice.pub"
+    self.bob_path = "bob.pub"
+
+    # dump a single signed layout
+    layout_template.create_signature(SSlibSigner(alice))
+    layout_template.dump(self.layout_single_signed_path)
+    # dump a double signed layout
+    layout_template.create_signature(SSlibSigner(bob))
+    layout_template.dump(self.layout_double_signed_path)
+
+
+  @classmethod
+  def tearDownClass(self):
+    self.tear_down_test_dir()
+
+
+  def test_main_required_args(self):
+    """Test in-toto-verify CLI tool with required arguments. """
+    args = ["--layout", self.layout_single_signed_path,
+        "--layout-keys", self.alice_path]
+
+    self.assert_cli_sys_exit(args, 0)
+
+
+  def test_main_multiple_keys(self):
+    """Test in-toto-verify CLI tool with multiple keys. """
+    args = ["--layout", self.layout_double_signed_path,
+        "--layout-keys", self.alice_path, self.bob_path]
+    self.assert_cli_sys_exit(args, 0)
+
+
+  def test_main_link_dir(self):
+    """Test in-toto-verify CLI tool with explicit link dir. """
+
+    # Use current working directory explicitly to load links
+    args = ["--layout", self.layout_single_signed_path,
+        "--layout-keys", self.alice_path, "--link-dir", "."]
+    self.assert_cli_sys_exit(args, 0)
+
+    # Fail with an explicit link directory, where no links are found
+    args = ["--layout", self.layout_single_signed_path,
+        "--layout-keys", self.alice_path, "--link-dir", "bad-link-dir"]
+    self.assert_cli_sys_exit(args, 1)
+
+
 
 class TestInTotoVerifyToolMixedKeys(CliTestCase, TmpDirMixin):
   """ Tests in-toto-verify like TestInTotoVerifyTool but with
   both rsa and ed25519 project owner and functionary keys. """
   cli_main_func = staticmethod(in_toto_verify_main)
 
 
@@ -181,15 +289,15 @@
     # Copy demo files to temp dir
     for fn in os.listdir(demo_files):
       shutil.copy(os.path.join(demo_files, fn), self.test_dir)
 
     shutil.copytree(scripts_directory, 'scripts')
 
     # Load layout template
-    layout_template = Metablock.load("demo.layout.template")
+    layout_template = Metadata.load("demo.layout.template")
 
     # Store layout paths to be used in tests
     self.layout_double_signed_path = "double-signed.layout"
 
     # Import layout signing keys
     alice = import_rsa_privatekey_from_file("alice")
     danny = import_ed25519_privatekey_from_file("danny")
@@ -210,14 +318,84 @@
     """Test in-toto-verify CLI tool with multiple keys. """
     args = ["--layout", self.layout_double_signed_path,
        "--layout-keys", self.alice_path, self.danny_path,
        "--key-types", "rsa", "ed25519"]
     self.assert_cli_sys_exit(args, 0)
 
 
+class TestInTotoVerifyToolMixedKeysWithDSSE(CliTestCase, TmpDirMixin):
+  """ Tests in-toto-verify like TestInTotoVerifyTool but with
+  both rsa and ed25519 project owner and functionary keys. """
+  cli_main_func = staticmethod(in_toto_verify_main)
+
+
+  @classmethod
+  def setUpClass(self):
+    """Creates and changes into temporary directory.
+    Copies demo files to temp dir...
+      - owner/functionary key pairs
+      - *.link metadata files
+      - layout template (not signed, no expiration date)
+      - final product
+
+    ...and dumps layout for test scenario
+    """
+    # Find demo files
+    demo_files = os.path.join(
+        os.path.dirname(os.path.realpath(__file__)), "demo_files")
+
+    # Demo DSSE Metadata Files
+    demo_dsse_files = os.path.join(
+        os.path.dirname(os.path.realpath(__file__)), "demo_dsse_files")
+
+    # find where the scripts directory is located.
+    scripts_directory = os.path.join(
+        os.path.dirname(os.path.realpath(__file__)), "scripts")
+
+    self.set_up_test_dir()
+
+    # Copy demo files to temp dir
+    for fn in os.listdir(demo_files):
+      shutil.copy(os.path.join(demo_files, fn), self.test_dir)
+
+    for fn in os.listdir(demo_dsse_files):
+      shutil.copy(os.path.join(demo_dsse_files, fn), self.test_dir)
+
+    shutil.copytree(scripts_directory, 'scripts')
+
+    # Load layout template
+    layout_template = Metadata.load("demo.layout.template")
+
+    # Store layout paths to be used in tests
+    self.layout_double_signed_path = "double-signed.layout"
+
+    # Import layout signing keys
+    alice = import_rsa_privatekey_from_file("alice")
+    danny = import_ed25519_privatekey_from_file("danny")
+    self.alice_path = "alice.pub"
+    self.danny_path = "danny.pub"
+
+    # dump a double signed layout
+    layout_template.create_signature(SSlibSigner(alice))
+    layout_template.create_signature(SSlibSigner(danny))
+    layout_template.dump(self.layout_double_signed_path)
+
+
+  @classmethod
+  def tearDownClass(self):
+    self.tear_down_test_dir()
+
+  def test_main_multiple_keys(self):
+    """Test in-toto-verify CLI tool with multiple keys. """
+    args = ["--layout", self.layout_double_signed_path,
+       "--layout-keys", self.alice_path, self.danny_path,
+       "--key-types", "rsa", "ed25519"]
+    self.assert_cli_sys_exit(args, 0)
+
+
 @unittest.skipIf(not have_gpg(), "gpg not found")
 class TestInTotoVerifyToolGPG(CliTestCase, TmpDirMixin, GPGKeysMixin):
   """ Tests in-toto-verify like TestInTotoVerifyTool but with
   gpg project owner and functionary keys. """
   cli_main_func = staticmethod(in_toto_verify_main)
 
 
@@ -239,15 +417,15 @@
     for fn in os.listdir(demo_files):
       shutil.copy(os.path.join(demo_files, fn), self.test_dir)
 
     # Change into test dir
     shutil.copytree(scripts_directory, 'scripts')
 
     # Sign layout template with gpg key
-    layout_template = Metablock.load("demo.layout.template")
+    layout_template = Metadata.load("demo.layout.template")
 
     self.layout_path = "gpg_signed.layout"
     layout_template.sign_gpg(self.gpg_key_0C8A17, self.gnupg_home)
     layout_template.dump(self.layout_path)
 
 
   @classmethod
```

### Comparing `in_toto-1.3.2/tests/test_log.py` & `in_toto-1.4.0/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/test_param_substitution.py` & `in_toto-1.4.0/tests/test_param_substitution.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,20 +24,21 @@
 """
 
 import os
 import shutil
 import unittest
 
 import in_toto.settings
-from in_toto.models.metadata import Metablock
+from in_toto.models.metadata import Envelope, Metablock
 from in_toto.models.layout import  Layout
 from in_toto.verifylib import in_toto_verify, substitute_parameters
 from securesystemslib.interface import (
     import_rsa_privatekey_from_file,
     import_publickeys_from_file)
+from securesystemslib.signer import SSlibSigner
 
 import in_toto.exceptions
 
 from tests.common import TmpDirMixin
 
 class Test_SubstituteArtifacts(unittest.TestCase):
   """Test parameter substitution on artifact rules. """
@@ -185,12 +186,26 @@
 
     # we will catch a LinkNotFound error because we don't have (and don't need)
     # the metadata.
     with self.assertRaises(in_toto.exceptions.LinkNotFoundError):
       in_toto_verify(signed_layout, self.alice_pub_dict,
           substitution_parameters={"EDITOR":"vim"})
 
+    self.assertEqual(self.layout.steps[0].expected_command[0], "vim")
+
+  def test_substitute_for_envelope(self):
+    """Do a simple substitution on the expected_command field for DSSE
+    envelope."""
+    signed_layout = Envelope.from_signable(self.layout)
+    signed_layout.create_signature(SSlibSigner(self.alice))
+
+    # we will catch a LinkNotFound error because we don't have (and don't need)
+    # the metadata.
+    with self.assertRaises(in_toto.exceptions.LinkNotFoundError):
+      in_toto_verify(signed_layout, self.alice_pub_dict,
+          substitution_parameters={"EDITOR":"vim"})
+
     self.assertEqual(self.layout.steps[0].expected_command[0], "vim")
 
 
 if __name__ == "__main__":
   unittest.main()
```

### Comparing `in_toto-1.3.2/tests/test_rulelib.py` & `in_toto-1.4.0/tests/test_rulelib.py`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/test_runlib.py` & `in_toto-1.4.0/tests/test_runlib.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 import tempfile
 import sys
 import stat
 import subprocess
 
 import in_toto.settings
 import in_toto.exceptions
-from in_toto.models.metadata import Metablock
+from in_toto.models.metadata import Envelope, Metablock
 from in_toto.exceptions import SignatureVerificationError
 from in_toto.runlib import (in_toto_run, in_toto_record_start,
     in_toto_record_stop, record_artifacts_as_dict, _apply_exclude_patterns,
     _hash_artifact, _subprocess_run_duplicate_streams)
 from securesystemslib.interface import (
     generate_and_write_unencrypted_rsa_keypair,
     import_rsa_privatekey_from_file,
@@ -768,14 +768,22 @@
     # make the directory read only
     os.chmod(tmp_dir, stat.S_IREAD)
     with self.assertRaises(PermissionError):
       in_toto_run(self.step_name, None, None, ["python", "--version"],
           True, self.key, metadata_directory=tmp_dir)
     os.rmdir(tmp_dir)
 
+  def test_in_toto_for_dsse(self):
+    """Test metadata generation using dsse."""
+
+    link_metadata = in_toto_run(self.step_name, None, None,
+        ["python", "--version"], True, self.key, use_dsse=True)
+    self.assertIsInstance(link_metadata, Envelope)
+    link_metadata.verify_signature(self.key)
+
 
 class TestInTotoRecordStart(unittest.TestCase, TmpDirMixin):
   """"Test in_toto_record_start(step_name, key, material_list). """
 
   @classmethod
   def setUpClass(self):
     """Create and change into temporary directory, generate key pair and dummy
@@ -805,29 +813,37 @@
     """Test record start creates metadata with expected material. """
     in_toto_record_start(
         self.step_name, [self.test_material], self.key)
     link = Metablock.load(self.link_name_unfinished)
     self.assertEqual(list(link.signed.materials.keys()), [self.test_material])
     os.remove(self.link_name_unfinished)
 
-  def test_create_unfininished_metadata_verify_signature(self):
+  def test_create_unfinished_metadata_verify_signature(self):
     """Test record start creates metadata with expected signature. """
     in_toto_record_start(
         self.step_name, [self.test_material], self.key)
     link = Metablock.load(self.link_name_unfinished)
     link.verify_signature(self.key)
     os.remove(self.link_name_unfinished)
 
   def test_no_key_arguments(self):
     """Test record start without passing one required key argument. """
     with self.assertRaises(ValueError):
       in_toto_record_start(
           self.step_name, [], signing_key=None, gpg_keyid=None,
           gpg_use_default=False)
 
+  def test_create_unfinished_metadata_using_dsse(self):
+    """Test record start creates metadata using dsse."""
+    in_toto_record_start(
+        self.step_name, [self.test_material], self.key, use_dsse=True)
+    link_metadata = Envelope.load(self.link_name_unfinished)
+    link_metadata.verify_signature(self.key)
+    os.remove(self.link_name_unfinished)
+
 class TestInTotoRecordStop(unittest.TestCase, TmpDirMixin):
   """"Test in_toto_record_stop(step_name, key, product_list). """
 
   @classmethod
   def setUpClass(self):
     """Create and change into temporary directory, generate two key pairs
     and dummy product. """
@@ -991,10 +1007,40 @@
     os.chmod(tmp_dir, stat.S_IREAD)
     with self.assertRaises(PermissionError):
       in_toto_record_start(self.step_name, [], self.key)
       in_toto_record_stop(self.step_name, [], self.key,
           metadata_directory=tmp_dir)
     os.rmdir(tmp_dir)
 
+  def test_created_metadata_using_dsse(self):
+    """Test record stop records created metadata with dsse."""
+    in_toto_record_start(self.step_name, [], self.key, use_dsse=True)
+    in_toto_record_stop(self.step_name, [self.test_product], self.key)
+
+    link_metadata = Envelope.load(self.link_name)
+    link_metadata.verify_signature(self.key)
+
+    link = link_metadata.get_payload()
+    self.assertEqual(list(link.products.keys()), [self.test_product])
+    os.remove(self.link_name)
+
+  def test_create_metadata_with_command_byproducts_environment(self):
+    """Test record stop records expected product. """
+    command = ["cp", "src", "dest"]
+    byproducts = {"stdout": "success", "stderr": "errors", "return-value": 0}
+    environment = {
+              "variables": "ENV_NAME=ENV_VALUE",
+              "filesystem": "<filesystem info>",
+              "workdir": "./"
+            }
+
+    in_toto_record_start(self.step_name, [], self.key, record_environment=True)
+    in_toto_record_stop(self.step_name, [self.test_product], self.key, command=command,
+      byproducts=byproducts, environment=environment)
+    link = Metablock.load(self.link_name)
+    self.assertEqual(link.signed.command, command)
+    self.assertDictEqual(link.signed.byproducts, byproducts)
+    self.assertDictEqual(link.signed.environment, environment)
+    os.remove(self.link_name)
 
 if __name__ == "__main__":
   unittest.main()
```

### Comparing `in_toto-1.3.2/tests/test_settings.py` & `in_toto-1.4.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/test_user_settings.py` & `in_toto-1.4.0/tests/test_user_settings.py`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/test_verifylib.py` & `in_toto-1.4.0/tests/test_verifylib.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,54 +17,50 @@
   See LICENSE for licensing information.
 
 <Purpose>
   Test verifylib functions.
 
 """
 
+import copy
+import glob
 import os
+import shlex
 import shutil
-import copy
 import tempfile
 import unittest
-import glob
-import shlex
-
+from datetime import datetime
 from unittest.mock import patch
 
-from datetime import datetime
+import securesystemslib.exceptions
+import securesystemslib.gpg.functions
 from dateutil.relativedelta import relativedelta
+from securesystemslib.interface import (import_publickeys_from_file,
+    import_rsa_privatekey_from_file, import_rsa_publickey_from_file)
 
+import in_toto.exceptions
 import in_toto.settings
+from in_toto.exceptions import (BadReturnValueError, LayoutExpiredError,
+    RuleVerificationError, ThresholdVerificationError,
+    SignatureVerificationError)
+from in_toto.models.layout import (SUBLAYOUT_LINK_DIR_FORMAT, Inspection,
+    Layout, Step)
+from in_toto.models.link import FILENAME_FORMAT, Link
 from in_toto.models.metadata import Metablock
-from in_toto.models.link import Link, FILENAME_FORMAT
-from in_toto.models.layout import (Step, Inspection, Layout,
-    SUBLAYOUT_LINK_DIR_FORMAT)
-from in_toto.verifylib import (verify_delete_rule, verify_create_rule,
-    verify_modify_rule, verify_allow_rule, verify_disallow_rule,
-    verify_require_rule, verify_match_rule, verify_item_rules,
-    verify_all_item_rules, verify_command_alignment, run_all_inspections,
-    in_toto_verify, verify_sublayouts, get_summary_link, _raise_on_bad_retval,
-    load_links_for_layout, verify_link_signature_thresholds,
-    verify_threshold_constraints)
-from in_toto.exceptions import (RuleVerificationError,
-    SignatureVerificationError, LayoutExpiredError, BadReturnValueError,
-    ThresholdVerificationError)
-from securesystemslib.interface import (
-    import_rsa_privatekey_from_file,
-    import_rsa_publickey_from_file,
-    import_publickeys_from_file)
 from in_toto.rulelib import unpack_rule
-import securesystemslib.gpg.functions
 from securesystemslib.gpg.constants import have_gpg
 
-import securesystemslib.exceptions
-import in_toto.exceptions
-
-from tests.common import TmpDirMixin, GPGKeysMixin
+from in_toto.verifylib import (_raise_on_bad_retval, get_summary_link,
+    in_toto_verify, load_links_for_layout, run_all_inspections,
+    verify_all_item_rules, verify_allow_rule, verify_command_alignment,
+    verify_create_rule, verify_delete_rule, verify_disallow_rule,
+    verify_item_rules, verify_link_signature_thresholds, verify_match_rule,
+    verify_modify_rule, verify_require_rule, verify_sublayouts,
+    verify_threshold_constraints)
+from tests.common import GPGKeysMixin, TmpDirMixin
 
 
 class Test_RaiseOnBadRetval(unittest.TestCase):
   """Tests internal function that raises an exception if the passed
   "return_value" is not and integer and not zero. """
 
   def test_zero_return_value(self):
@@ -410,18 +406,19 @@
       "sub/lib/bar": {"sha256": self.sha256_bar},
       "sub/lib/barfoo": {"sha256": self.sha256_barfoo},
       "build/bar": {"sha256": self.sha256_bar},
       "build/barfoo": {"sha256": self.sha256_barfoo},
     }
 
     self.links = {
-        "dest-item": Metablock(signed=Link(
+        "dest-item": Link(
             name="dest-item",
             materials=self.materials,
-            products=self.products)),
+            products=self.products
+          ),
     }
 
 
   def test_verify_match_rule(self):
     test_data_keys = [
         "rule string", "artifacts queue", "source artifacts", "expected"]
     test_cases = [
@@ -600,29 +597,28 @@
     self.item_name = "item"
     self.sha256_1 = \
         "d65165279105ca6773180500688df4bdc69a2c7b771752f0a46ef120b7fd8ec3"
     self.sha256_2 = \
         "cfdaaf1ab2e4661952a9dec5e8fa3c360c1b06b1a073e8493a7c46d2af8c504b"
 
     self.links = {
-      "item": Metablock(signed=Link(name="item",
-          materials={
-              "foo": {"sha256": self.sha256_1},
-              "foobar": {"sha256": self.sha256_1},
-              "bar": {"sha256": self.sha256_1},
-              "foobarbaz": {"sha256": self.sha256_1}
-          },
-          products={
-              "baz" : {"sha256": self.sha256_1},
-              "foo": {"sha256": self.sha256_1},
-              "bar": {"sha256": self.sha256_2},
-              "foobarbaz": {"sha256": self.sha256_1}
-
-          }
-      ))
+      "item": Link(name="item",
+        materials={
+            "foo": {"sha256": self.sha256_1},
+            "foobar": {"sha256": self.sha256_1},
+            "bar": {"sha256": self.sha256_1},
+            "foobarbaz": {"sha256": self.sha256_1}
+        },
+        products={
+            "baz" : {"sha256": self.sha256_1},
+            "foo": {"sha256": self.sha256_1},
+            "bar": {"sha256": self.sha256_2},
+            "foobarbaz": {"sha256": self.sha256_1}
+        }
+      )
     }
 
   def test_pass_rules_with_each_rule_type(self):
     """Pass with list of rules of each rule type. """
     rules = [
       ["DELETE", "foobar"],
       ["REQUIRE", "foobarbaz"],
@@ -700,45 +696,45 @@
                 ["MATCH", "foo", "IN", "dir", "WITH", "PRODUCTS",
                     "FROM", "write-code"]
             ]
         )
     ]
 
     self.links = {
-      "write-code" : Metablock(signed=Link(name="write-code",
-          products={
-              "foo": {
-                  "sha256": self.sha256_foo
-              }
-          }
-      )),
-      "package" : Metablock(signed=Link(name="package",
+      "write-code" : Link(name="write-code",
+        products={
+            "foo": {
+                "sha256": self.sha256_foo
+            }
+        }
+      ),
+      "package" : Link(name="package",
+        materials={
+            "foo": {
+                "sha256": self.sha256_foo
+            }
+        },
+        products={
+            "foo.tar.gz": {
+                "sha256": self.sha256_foo_tar
+            }
+        }
+      ),
+        "untar" : Link(name="untar",
           materials={
-              "foo": {
-                  "sha256": self.sha256_foo
-              }
-          },
-          products={
               "foo.tar.gz": {
                   "sha256": self.sha256_foo_tar
               }
+          },
+          products={
+              "dir/foo": {
+                  "sha256": self.sha256_foo
+              },
           }
-      )),
-        "untar" : Metablock(signed=Link(name="untar",
-            materials={
-                "foo.tar.gz": {
-                    "sha256": self.sha256_foo_tar
-                }
-            },
-            products={
-                "dir/foo": {
-                    "sha256": self.sha256_foo
-                },
-            }
-        ))
+        )
     }
 
   def test_pass_verify_all_step_rules(self):
     """Pass rule verification for dummy supply chain Steps. """
     verify_all_item_rules(self.steps, self.links)
 
   def test_pass_verify_all_inspection_rules(self):
@@ -945,26 +941,25 @@
     with self.assertRaises(SignatureVerificationError):
       in_toto_verify(layout_metablock, {})
 
   def test_verify_layout_signatures_fail_with_malformed_signature(self):
     """Layout signature verification fails with malformed signatures. """
     layout_metablock = Metablock(signed=Layout())
     signature = layout_metablock.sign(self.alice)
-    pubkey = self.alice
+    pubkey = copy.deepcopy(self.alice)
     pubkey["keyval"]["private"] = ""
 
     del signature["sig"]
     layout_metablock.signed.signatures = [signature]
     with self.assertRaises(SignatureVerificationError):
       in_toto_verify(layout_metablock, {self.alice["keyid"]: pubkey})
 
 
 
 
-
 class TestInTotoVerifyThresholds(unittest.TestCase):
   """Test verifylib functions related to signature thresholds.
 
     - verifylib.verify_link_signature_thresholds
     - verifylib.verify_threshold_constraints """
 
 
@@ -1131,24 +1126,22 @@
       verify_threshold_constraints(layout, chain_link_dict)
 
 
   def test_threshold_constraints_fail_with_unequal_links(self):
     """ Test that the links for a step recorded the same artifacts. """
     # Layout with one step and threshold 2
     layout = Layout(steps=[Step(name=self.name, threshold=2)])
-    link_bob = Metablock(
-        signed=Link(
-          name=self.name,
-          materials={
-            "foo": {"sha256": self.foo_hash}
-          }
-        )
-      )
+    link_bob = Link(
+      name=self.name,
+      materials={
+        "foo": {"sha256": self.foo_hash}
+      }
+    )
     # Cf. signing comment in test_thresholds_constraints_with_not_enough_links
-    link_alice = Metablock(signed=Link(name=self.name))
+    link_alice = Link(name=self.name)
 
     chain_link_dict = {
       self.name: {
         self.bob_keyid: link_bob,
         self.alice_keyid: link_alice,
       }
     }
@@ -1160,30 +1153,26 @@
 
   def test_threshold_constraints_pas_with_equal_links(self):
     """ Pass threshold constraint verification with equal links. """
     # Layout with one step and threshold 2
     layout = Layout(steps=[Step(name=self.name, threshold=2)])
     # Two authorized links with equal artifact recordings (materials)
     # Cf. signing comment in test_thresholds_constraints_with_not_enough_links
-    link_bob = Metablock(
-        signed=Link(
-          name=self.name,
-          materials={
-            "foo": {"sha256": self.foo_hash}
-          }
-        )
-      )
-    link_alice = Metablock(
-        signed=Link(
-          name=self.name,
-          materials={
-            "foo": {"sha256": self.foo_hash}
-          }
-        )
-      )
+    link_bob = Link(
+      name=self.name,
+      materials={
+        "foo": {"sha256": self.foo_hash}
+      }
+    )
+    link_alice = Link(
+      name=self.name,
+      materials={
+        "foo": {"sha256": self.foo_hash}
+      }
+    )
 
     chain_link_dict = {
       self.name: {
         self.bob_keyid: link_bob,
         self.alice_keyid: link_alice,
       }
     }
@@ -1681,33 +1670,33 @@
     for fn in os.listdir(demo_files):
       shutil.copy(os.path.join(demo_files, fn), self.test_dir)
 
     self.demo_layout = Metablock.load("demo.layout.template")
     self.code_link = Metablock.load("package.2f89b927.link")
     self.package_link = Metablock.load("write-code.776a00e2.link")
     self.demo_links = {
-        "write-code": self.code_link,
-        "package": self.package_link
+        "write-code": self.code_link.signed,
+        "package": self.package_link.signed
       }
 
   @classmethod
   def tearDownClass(self):
     self.tear_down_test_dir()
 
   def test_get_summary_link_from_demo_layout(self):
     """Create summary link from demo link files and compare properties. """
     sum_link = get_summary_link(self.demo_layout.signed, self.demo_links, "")
 
-    self.assertEqual(sum_link.signed._type, self.code_link.signed._type)
-    self.assertEqual(sum_link.signed.name, "")
-    self.assertEqual(sum_link.signed.materials, self.code_link.signed.materials)
-
-    self.assertEqual(sum_link.signed.products, self.package_link.signed.products)
-    self.assertEqual(sum_link.signed.command, self.package_link.signed.command)
-    self.assertEqual(sum_link.signed.byproducts, self.package_link.signed.byproducts)
-    self.assertEqual(sum_link.signed.byproducts.get("return-value"),
+    self.assertEqual(sum_link._type, self.code_link.signed._type)
+    self.assertEqual(sum_link.name, "")
+    self.assertEqual(sum_link.materials, self.code_link.signed.materials)
+
+    self.assertEqual(sum_link.products, self.package_link.signed.products)
+    self.assertEqual(sum_link.command, self.package_link.signed.command)
+    self.assertEqual(sum_link.byproducts, self.package_link.signed.byproducts)
+    self.assertEqual(sum_link.byproducts.get("return-value"),
         self.package_link.signed.byproducts.get("return-value"))
 
 
 
 if __name__ == "__main__":
   unittest.main()
```

### Comparing `in_toto-1.3.2/tests/demo_files/alice` & `in_toto-1.4.0/tests/demo_files/alice`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/demo_files/alice.pub` & `in_toto-1.4.0/tests/demo_files/alice.pub`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/demo_files/bob` & `in_toto-1.4.0/tests/demo_files/bob`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/demo_files/bob.pub` & `in_toto-1.4.0/tests/demo_files/bob.pub`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/demo_files/carl` & `in_toto-1.4.0/tests/demo_files/carl`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/demo_files/carl.pub` & `in_toto-1.4.0/tests/demo_files/carl.pub`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/demo_files/demo.layout.template` & `in_toto-1.4.0/tests/demo_files/demo.layout.template`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/demo_files/package.2f89b927.link` & `in_toto-1.4.0/tests/demo_files/package.2f89b927.link`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/demo_files/write-code.776a00e2.link` & `in_toto-1.4.0/tests/demo_files/write-code.776a00e2.link`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/demo_files_gpg/demo.layout.template` & `in_toto-1.4.0/tests/demo_files_gpg/demo.layout.template`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/demo_files_gpg/package.7b3abb26.link` & `in_toto-1.4.0/tests/demo_files_gpg/package.7b3abb26.link`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/demo_files_gpg/write-code.8288ef56.link` & `in_toto-1.4.0/tests/demo_files_gpg/write-code.8288ef56.link`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/gpg_keyrings/dsa/C242A830DAAF1C2BEF604A9EF033A3A3E267B3B1.ssh` & `in_toto-1.4.0/tests/gpg_keyrings/dsa/C242A830DAAF1C2BEF604A9EF033A3A3E267B3B1.ssh`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/gpg_keyrings/dsa/pubring.gpg` & `in_toto-1.4.0/tests/gpg_keyrings/dsa/pubring.gpg`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/gpg_keyrings/dsa/random_seed` & `in_toto-1.4.0/tests/gpg_keyrings/dsa/random_seed`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/gpg_keyrings/dsa/secring.gpg` & `in_toto-1.4.0/tests/gpg_keyrings/dsa/secring.gpg`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/gpg_keyrings/dsa/trustdb.gpg` & `in_toto-1.4.0/tests/gpg_keyrings/dsa/trustdb.gpg`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/gpg_keyrings/rsa/pubring.gpg` & `in_toto-1.4.0/tests/gpg_keyrings/rsa/pubring.gpg`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/gpg_keyrings/rsa/random_seed` & `in_toto-1.4.0/tests/gpg_keyrings/rsa/random_seed`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/gpg_keyrings/rsa/secring.gpg` & `in_toto-1.4.0/tests/gpg_keyrings/rsa/secring.gpg`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/gpg_keyrings/rsa/trustdb.gpg` & `in_toto-1.4.0/tests/gpg_keyrings/rsa/trustdb.gpg`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/models/test_common.py` & `in_toto-1.4.0/tests/models/test_common.py`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/models/test_inspection.py` & `in_toto-1.4.0/tests/models/test_inspection.py`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/models/test_layout.py` & `in_toto-1.4.0/tests/models/test_layout.py`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/models/test_link.py` & `in_toto-1.4.0/tests/models/test_link.py`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/models/test_metadata.py` & `in_toto-1.4.0/tests/models/test_metadata.py`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/models/test_signer.py` & `in_toto-1.4.0/tests/models/test_signer.py`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/models/test_step.py` & `in_toto-1.4.0/tests/models/test_step.py`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/models/test_supply_chain_item.py` & `in_toto-1.4.0/tests/models/test_supply_chain_item.py`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/scripts/expr` & `in_toto-1.4.0/tests/scripts/expr`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/scripts/tar` & `in_toto-1.4.0/tests/scripts/tar`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/tests/scripts/touch` & `in_toto-1.4.0/tests/scripts/touch`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/.gitignore` & `in_toto-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/LICENSE` & `in_toto-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/README.md` & `in_toto-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `in_toto-1.3.2/pyproject.toml` & `in_toto-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     "Topic :: Software Development",
 ]
 dependencies = [
     "attrs",
     "iso8601",
     "pathspec",
     "python-dateutil",
-    "securesystemslib[crypto]>=0.27.0",
+    "securesystemslib[crypto]>=0.28.0",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 # Install pynacl as optional dependency to use with securesystemslib, as a
 # workaround for `"ssl-pynacl": ["securesystemslib[pynacl]>=0.11.3"]`,
 # which currently is not supported in "extra_require" (see pypa/pip#4957).
```

### Comparing `in_toto-1.3.2/PKG-INFO` & `in_toto-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: in-toto
-Version: 1.3.2
+Version: 1.4.0
 Summary: A framework to define and secure the integrity of software supply chains
 Project-URL: Bug Reports, https://github.com/in-toto/in-toto/issues
 Project-URL: Homepage, https://in-toto.io
 Project-URL: Source, https://github.com/in-toto/in-toto
 Author-email: "New York University: Secure Systems Lab" <in-toto-dev@googlegroups.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -26,15 +26,15 @@
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development
 Requires-Python: ~=3.7
 Requires-Dist: attrs
 Requires-Dist: iso8601
 Requires-Dist: pathspec
 Requires-Dist: python-dateutil
-Requires-Dist: securesystemslib[crypto]>=0.27.0
+Requires-Dist: securesystemslib[crypto]>=0.28.0
 Provides-Extra: pynacl
 Requires-Dist: pynacl>1.2.0; extra == 'pynacl'
 Description-Content-Type: text/markdown
 
 # in-toto ![Build](https://github.com/in-toto/in-toto/workflows/Run%20in-toto%20tests%20and%20linter/badge.svg) [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/1523/badge)](https://bestpractices.coreinfrastructure.org/projects/1523) [![Build status](https://ci.appveyor.com/api/projects/status/taxlhrrlf3co07e1/branch/develop?svg=true)](https://ci.appveyor.com/project/in-toto/in-toto/branch/develop) [![Documentation Status](https://readthedocs.org/projects/in-toto/badge/?version=latest)](https://in-toto.readthedocs.io/en/latest/?badge=latest)
 
 in-toto provides a framework to protect the integrity of the software supply chain. It does so by verifying that each task in the chain is carried out as planned, by authorized personnel only, and that the product is not tampered with in transit.
```

