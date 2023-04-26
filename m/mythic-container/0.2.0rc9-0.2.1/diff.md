# Comparing `tmp/mythic_container-0.2.0rc9.tar.gz` & `tmp/mythic_container-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mythic_container-0.2.0rc9.tar", last modified: Sat Mar 25 00:42:19 2023, max compression
+gzip compressed data, was "mythic_container-0.2.1.tar", last modified: Tue Apr 25 19:38:55 2023, max compression
```

## Comparing `mythic_container-0.2.0rc9.tar` & `mythic_container-0.2.1.tar`

### file list

```diff
@@ -1,86 +1,87 @@
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-03-25 00:42:19.749052 mythic_container-0.2.0rc9/
--rw-r--r--   0 itsafeature   (501) staff       (20)     1481 2023-03-07 22:54:23.000000 mythic_container-0.2.0rc9/LICENSE.md
--rw-r--r--   0 itsafeature   (501) staff       (20)     1517 2023-03-25 00:42:19.748774 mythic_container-0.2.0rc9/PKG-INFO
--rwxr-xr-x   0 itsafeature   (501) staff       (20)     1069 2023-02-27 20:26:00.000000 mythic_container-0.2.0rc9/README.md
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-03-25 00:42:19.702612 mythic_container-0.2.0rc9/mythic_container/
--rw-r--r--   0 itsafeature   (501) staff       (20)    16293 2023-02-21 17:50:11.000000 mythic_container-0.2.0rc9/mythic_container/C2ProfileBase.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3070 2023-02-23 00:16:47.000000 mythic_container-0.2.0rc9/mythic_container/LoggingBase.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    49127 2023-03-21 20:11:05.000000 mythic_container-0.2.0rc9/mythic_container/MythicCommandBase.py
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-03-25 00:42:19.746133 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/
--rw-r--r--   0 itsafeature   (501) staff       (20)     2481 2023-02-17 22:40:44.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/__init__.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1368 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1214 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_remove.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1721 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1562 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2181 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1316 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_add_command.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3360 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1770 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_decrypt_bytes.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1710 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_display_to_real_id_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1770 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_encrypt_bytes.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1343 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_remove_command.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7424 2023-03-23 13:36:37.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2272 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search_command.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3182 2023-03-13 17:15:03.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_update.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     4295 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1474 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_remove.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3478 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_command_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2267 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_credential_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2495 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_credential_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2767 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_file_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1330 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_file_get_content.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1785 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_file_register.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     4442 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_file_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2216 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_file_update.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3713 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1771 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_remove.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1852 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2621 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1898 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_operationeventlog_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2572 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_other_service_rpc.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1332 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_add_command.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     4632 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_scratch.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1833 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_uuid.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1359 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_get_content.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1359 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_remove_command.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     5343 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1748 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_update_build_step.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2017 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_payloadonhost_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3097 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_process_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     4779 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_process_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1327 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_start.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1318 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_stop.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1403 2023-03-25 00:41:22.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_response_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2072 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_response_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1940 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2659 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask_group.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1642 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_task_display_to_real_id_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7752 2023-02-22 19:46:40.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_task_search.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1833 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_task_update.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1372 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_token_create.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1375 2023-02-21 14:37:49.000000 mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_token_remove.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    28320 2023-02-21 14:36:00.000000 mythic_container-0.2.0rc9/mythic_container/MythicRPC.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    13243 2023-03-06 23:50:17.000000 mythic_container-0.2.0rc9/mythic_container/PayloadBuilder.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     6104 2023-02-28 00:19:56.000000 mythic_container-0.2.0rc9/mythic_container/TranslationBase.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7240 2023-02-22 22:10:41.000000 mythic_container-0.2.0rc9/mythic_container/WebhookBase.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     2507 2023-03-25 00:42:02.000000 mythic_container-0.2.0rc9/mythic_container/__init__.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    35588 2023-03-21 20:03:40.000000 mythic_container-0.2.0rc9/mythic_container/agent_utils.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    27628 2023-02-28 22:44:25.000000 mythic_container-0.2.0rc9/mythic_container/c2_utils.py
--rwxr-xr-x   0 itsafeature   (501) staff       (20)      262 2023-02-28 20:49:28.000000 mythic_container-0.2.0rc9/mythic_container/config.py
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-03-25 00:42:19.748018 mythic_container-0.2.0rc9/mythic_container/grpc/
--rw-r--r--   0 itsafeature   (501) staff       (20)        0 2023-02-20 17:25:18.000000 mythic_container-0.2.0rc9/mythic_container/grpc/__init__.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     4479 2023-02-21 13:59:33.000000 mythic_container-0.2.0rc9/mythic_container/grpc/translationContainerGRPC_pb2.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7092 2023-02-21 17:37:56.000000 mythic_container-0.2.0rc9/mythic_container/grpc/translationContainerGRPC_pb2_grpc.py
--rw-r--r--   0 itsafeature   (501) staff       (20)      937 2023-02-28 20:15:31.000000 mythic_container-0.2.0rc9/mythic_container/logging.py
--rwxr-xr-x   0 itsafeature   (501) staff       (20)    24443 2023-03-13 14:01:12.000000 mythic_container-0.2.0rc9/mythic_container/mythic_service.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    14031 2023-03-03 14:56:12.000000 mythic_container-0.2.0rc9/mythic_container/rabbitmq.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1670 2023-02-21 14:36:00.000000 mythic_container-0.2.0rc9/mythic_container/utils_mythic_file_transfer.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     1732 2023-02-22 03:09:36.000000 mythic_container-0.2.0rc9/mythic_container/webhook_utils.py
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-03-25 00:42:19.705034 mythic_container-0.2.0rc9/mythic_container.egg-info/
--rw-r--r--   0 itsafeature   (501) staff       (20)     1517 2023-03-25 00:42:19.000000 mythic_container-0.2.0rc9/mythic_container.egg-info/PKG-INFO
--rw-r--r--   0 itsafeature   (501) staff       (20)     4340 2023-03-25 00:42:19.000000 mythic_container-0.2.0rc9/mythic_container.egg-info/SOURCES.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)        1 2023-03-25 00:42:19.000000 mythic_container-0.2.0rc9/mythic_container.egg-info/dependency_links.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)       95 2023-03-25 00:42:19.000000 mythic_container-0.2.0rc9/mythic_container.egg-info/requires.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)       17 2023-03-25 00:42:19.000000 mythic_container-0.2.0rc9/mythic_container.egg-info/top_level.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)       38 2023-03-25 00:42:19.749315 mythic_container-0.2.0rc9/setup.cfg
--rwxr-xr-x   0 itsafeature   (501) staff       (20)     1092 2023-03-25 00:41:58.000000 mythic_container-0.2.0rc9/setup.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-25 19:38:55.566430 mythic_container-0.2.1/
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1481 2023-03-07 22:54:23.000000 mythic_container-0.2.1/LICENSE.md
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1438 2023-04-25 19:38:55.566192 mythic_container-0.2.1/PKG-INFO
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)      993 2023-04-25 19:15:08.000000 mythic_container-0.2.1/README.md
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-25 19:38:55.538044 mythic_container-0.2.1/mythic_container/
+-rw-r--r--   0 itsafeature   (501) staff       (20)    29960 2023-04-19 16:52:07.000000 mythic_container-0.2.1/mythic_container/C2ProfileBase.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    26032 2023-04-20 01:54:22.000000 mythic_container-0.2.1/mythic_container/LoggingBase.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    77811 2023-04-20 00:07:13.000000 mythic_container-0.2.1/mythic_container/MythicCommandBase.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-25 19:38:55.564539 mythic_container-0.2.1/mythic_container/MythicGoRPC/
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2482 2023-04-01 06:52:48.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/__init__.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1368 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1214 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_remove.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1721 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1562 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2181 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1316 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_add_command.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3360 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1770 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_decrypt_bytes.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1710 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_display_to_real_id_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1770 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_encrypt_bytes.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1343 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_remove_command.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7424 2023-03-23 13:36:37.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2273 2023-04-04 02:07:20.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search_command.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3182 2023-03-13 17:15:03.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_update.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4295 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1474 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_remove.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3478 2023-04-01 06:52:13.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_command_search_.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2267 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_credential_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2495 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_credential_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2767 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_file_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1330 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_file_get_content.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1785 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_file_register.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4453 2023-04-13 18:13:16.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_file_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2216 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_file_update.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3713 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1771 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_remove.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1852 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2621 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1898 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_operationeventlog_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2572 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_other_service_rpc.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1332 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_add_command.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4632 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_scratch.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1833 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_uuid.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1359 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_get_content.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1359 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_remove_command.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     6013 2023-04-01 05:24:39.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1748 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_update_build_step.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2017 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_payloadonhost_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3097 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_process_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4779 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_process_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1327 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_start.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1318 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_stop.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1403 2023-03-25 00:41:22.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_response_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2072 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_response_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1940 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2659 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask_group.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1642 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_task_display_to_real_id_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7752 2023-02-22 19:46:40.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_task_search.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1833 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_task_update.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1372 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_token_create.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1375 2023-02-21 14:37:49.000000 mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_token_remove.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    28320 2023-02-21 14:36:00.000000 mythic_container-0.2.1/mythic_container/MythicRPC.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    22324 2023-04-21 19:16:23.000000 mythic_container-0.2.1/mythic_container/PayloadBuilder.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7251 2023-04-19 16:38:54.000000 mythic_container-0.2.1/mythic_container/TranslationBase.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    13910 2023-04-25 19:08:24.000000 mythic_container-0.2.1/mythic_container/WebhookBase.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2577 2023-04-25 19:38:46.000000 mythic_container-0.2.1/mythic_container/__init__.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    36785 2023-04-21 19:16:40.000000 mythic_container-0.2.1/mythic_container/agent_utils.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    27738 2023-04-24 22:49:45.000000 mythic_container-0.2.1/mythic_container/c2_utils.py
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)      262 2023-02-28 20:49:28.000000 mythic_container-0.2.1/mythic_container/config.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-25 19:38:55.565768 mythic_container-0.2.1/mythic_container/grpc/
+-rw-r--r--   0 itsafeature   (501) staff       (20)        0 2023-02-20 17:25:18.000000 mythic_container-0.2.1/mythic_container/grpc/__init__.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4479 2023-02-21 13:59:33.000000 mythic_container-0.2.1/mythic_container/grpc/translationContainerGRPC_pb2.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7092 2023-02-21 17:37:56.000000 mythic_container-0.2.1/mythic_container/grpc/translationContainerGRPC_pb2_grpc.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)      937 2023-02-28 20:15:31.000000 mythic_container-0.2.1/mythic_container/logging.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4025 2023-04-19 23:39:10.000000 mythic_container-0.2.1/mythic_container/logging_utils.py
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)    28650 2023-04-25 19:14:22.000000 mythic_container-0.2.1/mythic_container/mythic_service.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    14498 2023-04-10 15:53:13.000000 mythic_container-0.2.1/mythic_container/rabbitmq.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1670 2023-02-21 14:36:00.000000 mythic_container-0.2.1/mythic_container/utils_mythic_file_transfer.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2821 2023-04-20 15:20:17.000000 mythic_container-0.2.1/mythic_container/webhook_utils.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-25 19:38:55.540162 mythic_container-0.2.1/mythic_container.egg-info/
+-rw-r--r--   0 itsafeature   (501) staff       (20)     1438 2023-04-25 19:38:55.000000 mythic_container-0.2.1/mythic_container.egg-info/PKG-INFO
+-rw-r--r--   0 itsafeature   (501) staff       (20)     4375 2023-04-25 19:38:55.000000 mythic_container-0.2.1/mythic_container.egg-info/SOURCES.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)        1 2023-04-25 19:38:55.000000 mythic_container-0.2.1/mythic_container.egg-info/dependency_links.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)       95 2023-04-25 19:38:55.000000 mythic_container-0.2.1/mythic_container.egg-info/requires.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)       17 2023-04-25 19:38:55.000000 mythic_container-0.2.1/mythic_container.egg-info/top_level.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)       38 2023-04-25 19:38:55.566528 mythic_container-0.2.1/setup.cfg
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)     1088 2023-04-25 19:38:30.000000 mythic_container-0.2.1/setup.py
```

### Comparing `mythic_container-0.2.0rc9/LICENSE.md` & `mythic_container-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/PKG-INFO` & `mythic_container-0.2.1/mythic_container.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mythic_container
-Version: 0.2.0rc9
+Name: mythic-container
+Version: 0.2.1
 Summary: Functionality for Mythic Services
 Home-page: https://docs.mythic-c2.net/customizing/payload-type-development
 Author: @its_a_feature_
 Author-email: 
 License: BSD3
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -23,15 +23,15 @@
 
 ```
 pip install mythic-container
 ```
 
 ## How to use
 
-This container reports to mythic as version "v1.0.0" (PyPi version 0.1.18). Use it with Mythic version 3.0.0.
+Use it with Mythic version 3.0.0.
 
 For the main execution of the heartbeat and service functionality, simply import and start the service:
 ```
 import mythic_container
 import [my agent | my c2 profile | my translation container | my webhooks | my loggers]
 mythic_container.mythic_service.start_and_run_forever()
 ```
```

### Comparing `mythic_container-0.2.0rc9/README.md` & `mythic_container-0.2.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 ```
 pip install mythic-container
 ```
 
 ## How to use
 
-This container reports to mythic as version "v1.0.0" (PyPi version 0.1.18). Use it with Mythic version 3.0.0.
+Use it with Mythic version 3.0.0.
 
 For the main execution of the heartbeat and service functionality, simply import and start the service:
 ```
 import mythic_container
 import [my agent | my c2 profile | my translation container | my webhooks | my loggers]
 mythic_container.mythic_service.start_and_run_forever()
 ```
```

### Comparing `mythic_container-0.2.0rc9/mythic_container/LoggingBase.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_process_create.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,93 +1,88 @@
-from collections.abc import Callable, Awaitable
-from typing import Union
-
 import mythic_container
-from .logging import logger
-import aiohttp
-from .config import settings
-import json
+from mythic_container.logging import logger
+
+MYTHIC_RPC_PROCESS_CREATE = "mythic_rpc_process_create"
 
-class NewCallbackLoggingData:
+class MythicRPCProcessCreateData:
     def __init__(self,
-                 user: str = None,
-                 host: str = None,
-                 ips: str = None,
-                 domain: str = None,
-                 external_ip: str = None,
-                 process_name: str = None,
-                 pid: int = 0,
-                 os: str = None,
-                 architecture: str = None,
-                 agent_type: str = None,
-                 description: str = None,
-                 extra_info: str = None,
-                 sleep_info: str = None,
-                 display_id: int = 0,
-                 id: int = 0,
-                 integrity_level: int = 2):
-        self.User = user
-        self.Host = host
-        self.IPs = json.loads(ips) if ips is not None else None
-        self.Domain = domain
-        self.ExternalIP = external_ip
-        self.ProcessName = process_name
-        self.PID = pid
-        self.Os = os
-        self.Architecture = architecture
-        self.AgentType = agent_type
-        self.Description = description
-        self.ExtraInfo = extra_info
-        self.SleepInfo = sleep_info
-        self.DisplayID = display_id
-        self.ID = id
-        self.IntegrityLevel = integrity_level
+                 Host: str = None,
+                 ProcessID: int = None,
+                 ParentProcessID: int = None,
+                 Architecture: str = None,
+                 BinPath: str = None,
+                 Name: str = None,
+                 User: str = None,
+                 CommandLine: str = None,
+                 IntegrityLevel: int = None,
+                 StartTime: int = None,
+                 Description: str = None,
+                 Signer: str = None,
+                 ProtectionProcessLevel: int = None,
+                 **kwargs):
+        self.Host = Host
+        self.ProcessID = ProcessID
+        self.ParentProcessID = ParentProcessID
+        self.Architecture = Architecture
+        self.BinPath = BinPath
+        self.Name = Name
+        self.User = User
+        self.CommandLine = CommandLine
+        self.IntegrityLevel = IntegrityLevel
+        self.StartTime = StartTime
+        self.Description = Description
+        self.Signer = Signer
+        self.ProtectionProcessLevel = ProtectionProcessLevel
+        self.other = kwargs
+
     def to_json(self):
         return {
-            "user": self.User,
             "host": self.Host,
-            "ips": self.IPs,
-            "domain": self.Domain,
-            "external_ip": self.ExternalIP,
-            "process_name": self.ProcessName,
-            "pid": self.PID,
-            "os": self.Os,
+            "process_id": self.ProcessID,
+            "parent_process_id": self.ParentProcessID,
             "architecture": self.Architecture,
+            "bin_path": self.BinPath,
+            "name": self.Name,
+            "user": self.User,
+            "command_line": self.CommandLine,
+            "integrity_level": self.IntegrityLevel,
+            "start_time": self.StartTime,
             "description": self.Description,
-            "extra_info": self.ExtraInfo,
-            "sleep_info": self.SleepInfo,
-            "display_id": self.DisplayID,
-            "id": self.ID,
-            "integrity_level": self.IntegrityLevel
+            "signer": self.Signer,
+            "protected_process_level": self.ProtectionProcessLevel,
+            **self.other
         }
 
-class LoggingMessage:
-    Data: Union[dict | NewCallbackLoggingData | None]
+
+class MythicRPCProcessesCreateMessage:
     def __init__(self,
-                 operation_id: int = None,
-                 operation_name: str = None,
-                 operator_username: str = None,
-                 timestamp: str = None,
-                 action: str = None,
-                 data: dict = None,
+                 TaskID: int,
+                 Processes: list[MythicRPCProcessCreateData] = None,
                  **kwargs):
-        self.OperationID = operation_id
-        self.OperationName = operation_name
-        self.OperatorUsername = operator_username
-        self.Timestamp = timestamp
-        self.Action = action
-        if self.Action == mythic_container.LOG_TYPE_CALLBACK:
-            self.Data = NewCallbackLoggingData(**data)
-        else:
-            self.Data = data
-        for k,v in kwargs.items():
-            logger.info(f"unknown kwarg {k} {v}")
-
-
-class Log:
-
-    new_callback: Callable[ [LoggingMessage], Awaitable[None] ] = None
-    new_feedback: Callable[ [LoggingMessage], Awaitable[None] ] = None
-    new_startup:  Callable[ [LoggingMessage], Awaitable[None] ] = None
+        self.TaskID = TaskID
+        self.Processes = Processes
+        for k, v in kwargs.items():
+            logger.info(f"Unknown kwarg {k} - {v}")
 
+    def to_json(self):
+        return {
+            "task_id": self.TaskID,
+            "processes": [x.to_json() for x in self.Processes]
+        }
+
+
+class MythicRPCProcessesCreateMessageResponse:
+    def __init__(self,
+                 success: bool = False,
+                 error: str = "",
+                 **kwargs):
+        self.Success = success
+        self.Error = error
+        for k, v in kwargs.items():
+            logger.info(f"Unknown kwarg {k} - {v}")
 
 
+async def SendMythicRPCProcessCreate(
+        msg: MythicRPCProcessesCreateMessage) -> MythicRPCProcessesCreateMessageResponse:
+    response = await mythic_container.RabbitmqConnection.SendRPCDictMessage(queue=MYTHIC_RPC_PROCESS_CREATE,
+                                                                            body=msg.to_json())
+    return MythicRPCProcessesCreateMessageResponse(**response)
```

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/__init__.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from .send_mythic_rpc_callback_remove_command import *
 from .send_mythic_rpc_callback_search import *
 from .send_mythic_rpc_callback_display_to_real_id_search import *
 from .send_mythic_rpc_callback_search_command import *
 from .send_mythic_rpc_callback_update import *
 from .send_mythic_rpc_callbacktoken_create import *
 from .send_mythic_rpc_callbacktoken_remove import *
-from .send_mythic_rpc_command_search import *
+from .send_mythic_rpc_command_search_ import *
 from .send_mythic_rpc_credential_create import *
 from .send_mythic_rpc_credential_search import *
 from .send_mythic_rpc_file_create import *
 from .send_mythic_rpc_file_get_content import *
 from .send_mythic_rpc_file_register import *
 from .send_mythic_rpc_file_search import *
 from .send_mythic_rpc_file_update import *
```

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_create.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_remove.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_remove.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_search.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_agentstorage_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_create.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_search.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_artifact_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_add_command.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_add_command.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_create.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_decrypt_bytes.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_decrypt_bytes.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_display_to_real_id_search.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_display_to_real_id_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_encrypt_bytes.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_encrypt_bytes.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_remove_command.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_remove_command.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search_command.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_search_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import mythic_container
 from mythic_container.logging import logger
-from .send_mythic_rpc_command_search import MythicRPCCommandSearchData
+from .send_mythic_rpc_command_search_ import MythicRPCCommandSearchData
 
 MYTHIC_RPC_CALLBACK_SEARCH_COMMAND = "mythic_rpc_callback_search_command"
 
 
 class MythicRPCCallbackSearchCommandMessage:
     def __init__(self,
                  CallbackID: int = None,
```

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callback_update.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callback_update.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_create.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_remove.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_remove.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_command_search.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_command_search_.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_credential_create.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_credential_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_credential_search.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_credential_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_file_create.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_file_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_file_get_content.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_file_get_content.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_file_register.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_file_register.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_file_search.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_file_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         return {
             "task_id": self.TaskID,
             "callback_id": self.CallbackID,
             "limit_by_callback": self.LimitByCallback,
             "max_results": self.MaxResults,
             "filename": self.Filename,
             "is_screenshot": self.IsScreenshot,
-            "is_download": self.IsDownloadFromAgent,
+            "is_download_from_agent": self.IsDownloadFromAgent,
             "is_payload": self.IsPayload,
             "file_id": self.AgentFileID,
             "comment": self.Comment
         }
 
 
 class FileData:
```

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_file_update.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_file_update.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_create.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_remove.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_filebrowser_remove.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_create.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_search.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_keylog_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_operationeventlog_create.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_operationeventlog_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_other_service_rpc.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_other_service_rpc.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_add_command.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_add_command.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_scratch.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_scratch.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_uuid.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_create_from_uuid.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_get_content.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_get_content.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_remove_command.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_remove_command.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_search.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_search.py`

 * *Files 8% similar despite different names*

```diff
@@ -86,40 +86,55 @@
                  build_parameters: list[MythicRPCPayloadConfigurationBuildParameter] = None,
                  commands: list[str] = None,
                  selected_os: str = None,
                  filename: str = None,
                  wrapped_payload: str = None,
                  uuid: str = None,
                  agent_file_id: str = None,
+                 build_phase: str = None,
                  **kwargs):
         self.Description = description
         self.PayloadType = payload_type
-        self.C2Profiles = c2_profiles
-        self.BuildParameters = build_parameters
+        if c2_profiles is not None:
+            if isinstance(c2_profiles, list):
+                self.C2Profiles = [MythicRPCPayloadConfigurationC2Profile(**x) for x in c2_profiles]
+            else:
+                self.C2Profiles = c2_profiles
+        else:
+            self.C2Profiles = None
+        if build_parameters is not None:
+            if isinstance(build_parameters, list):
+                self.BuildParameters = [MythicRPCPayloadConfigurationBuildParameter(**x) for x in build_parameters]
+            else:
+                self.BuildParameters = build_parameters
+        else:
+            self.BuildParameters = None
         self.Commands = commands
         self.SelectedOS = selected_os
         self.Filename = filename
         self.WrappedPayloadUUID = wrapped_payload
         self.UUID = uuid
         self.AgentFileId = agent_file_id
+        self.BuildPhase = build_phase
         for k, v in kwargs.items():
             logger.info(f"Unknown kwarg {k} - {v}")
 
     def to_json(self):
         return {
             "description": self.Description,
             "payload_type": self.PayloadType,
             "c2_profiles": [x.to_json() for x in self.C2Profiles],
             "build_parameters": [x.to_json() for x in self.BuildParameters],
             "commands": self.Commands,
             "selected_os": self.SelectedOS,
             "filename": self.Filename,
             "wrapped_payload": self.WrappedPayloadUUID,
             "uuid": self.UUID,
-            "agent_file_id": self.AgentFileId
+            "agent_file_id": self.AgentFileId,
+            "build_phase": self.BuildPhase
         }
 class MythicRPCPayloadSearchMessageResponse:
     Payloads: list[MythicRPCPayloadConfiguration]
 
     def __init__(self,
                  success: bool = False,
                  error: str = "",
```

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_payload_update_build_step.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_payload_update_build_step.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_payloadonhost_create.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_payloadonhost_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_process_search.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_process_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_start.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_start.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_stop.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_proxy_stop.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_response_create.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_response_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_response_search.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_response_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask_group.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_task_create_subtask_group.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_task_display_to_real_id_search.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_task_display_to_real_id_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_task_search.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_task_search.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_task_update.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_task_update.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_token_create.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_token_create.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicGoRPC/send_mythic_rpc_token_remove.py` & `mythic_container-0.2.1/mythic_container/MythicGoRPC/send_mythic_rpc_token_remove.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/MythicRPC.py` & `mythic_container-0.2.1/mythic_container/MythicRPC.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/TranslationBase.py` & `mythic_container-0.2.1/mythic_container/TranslationBase.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,58 @@
 import asyncio
 from abc import abstractmethod
 from .grpc.translationContainerGRPC_pb2_grpc import TranslationContainerStub
 from .grpc.translationContainerGRPC_pb2 import TrGenerateEncryptionKeysMessage, TrGenerateEncryptionKeysMessageResponse
-from .grpc.translationContainerGRPC_pb2 import TrCustomMessageToMythicC2FormatMessage, TrCustomMessageToMythicC2FormatMessageResponse
-from .grpc.translationContainerGRPC_pb2 import TrMythicC2ToCustomMessageFormatMessage, TrMythicC2ToCustomMessageFormatMessageResponse
+from .grpc.translationContainerGRPC_pb2 import TrCustomMessageToMythicC2FormatMessage, \
+    TrCustomMessageToMythicC2FormatMessageResponse
+from .grpc.translationContainerGRPC_pb2 import TrMythicC2ToCustomMessageFormatMessage, \
+    TrMythicC2ToCustomMessageFormatMessageResponse
 import grpc.aio
 from mythic_container.logging import logger
 from .config import settings
+import json
+
 
 class TranslationContainer:
+    """The base definition for a Translation Container Service.
+
+    To have this hooked up to a Payload Type, you need to specify this service's name as the translation_container attribute in your Payload Type.
+
+    This uses gRPC to connect to port 17444 on the Mythic Server.
 
+    Attributes:
+        name (str): The name of the translation container
+        description (str): Description of the translation container to appear in Mythic's UI
+        author (str): The author of the container
+
+    Functions:
+        to_json:
+            return dictionary form of class
+        generate_keys:
+            A function for generating encryption/decryption keys based on provided C2 info
+        translate_to_c2_format:
+            A function for translating from Mythic's JSON format to a custom C2 format
+        translate_from_c2_format:
+            A function for translating from a custom C2 format to Mythic's JSON format
+
+    """
     async def generate_keys(self, inputMsg: TrGenerateEncryptionKeysMessage) -> TrGenerateEncryptionKeysMessageResponse:
         response = TrGenerateEncryptionKeysMessageResponse(Success=False)
         response.Error = f"Not Implemented:\n{inputMsg}"
 
         return response
 
-    async def translate_to_c2_format(self, inputMsg: TrMythicC2ToCustomMessageFormatMessage) -> TrMythicC2ToCustomMessageFormatMessageResponse:
+    async def translate_to_c2_format(self,
+                                     inputMsg: TrMythicC2ToCustomMessageFormatMessage) -> TrMythicC2ToCustomMessageFormatMessageResponse:
         response = TrMythicC2ToCustomMessageFormatMessageResponse(Success=False)
         response.Error = f"Not Implemented:\n{inputMsg}"
         return response
 
-    async def translate_from_c2_format(self, inputMsg: TrCustomMessageToMythicC2FormatMessage) -> TrCustomMessageToMythicC2FormatMessageResponse:
+    async def translate_from_c2_format(self,
+                                       inputMsg: TrCustomMessageToMythicC2FormatMessage) -> TrCustomMessageToMythicC2FormatMessageResponse:
         response = TrCustomMessageToMythicC2FormatMessageResponse(Success=False)
         response.Error = f"Not Implemented:\n{inputMsg}"
         return response
 
     @property
     @abstractmethod
     def name(self):
@@ -44,23 +71,27 @@
     def to_json(self):
         return {
             "name": self.name,
             "description": self.description,
             "author": self.author,
         }
 
+    def __str__(self):
+        return json.dumps(self.to_json(), sort_keys=True, indent=2)
+
 
 translationServices: dict[str, TranslationContainer] = {}
 
 
 async def handleTranslationServices(tr_name: str):
     while True:
         try:
             logger.info(f"Attempting connection to gRPC for {tr_name}...")
-            channel = grpc.aio.insecure_channel(f'{settings.get("mythic_server_host", "127.0.0.1")}:{settings.get("mythic_server_grpc_port", 17444)}')
+            channel = grpc.aio.insecure_channel(
+                f'{settings.get("mythic_server_host", "127.0.0.1")}:{settings.get("mythic_server_grpc_port", 17444)}')
             await channel.channel_ready()
             client = TranslationContainerStub(channel=channel)
             genKeys = handleGenerateKeys(tr_name, client)
             customToMythic = handleCustomToMythic(tr_name, client)
             mythicToCustom = handleMythicToCustom(tr_name, client)
             logger.info(f"[+] Successfully connected to gRPC for {tr_name}")
             await asyncio.gather(genKeys, customToMythic, mythicToCustom)
@@ -133,8 +164,8 @@
                 logger.exception(f"Failed to process message:\n{d}")
                 await stream.write(TrMythicC2ToCustomMessageFormatMessageResponse(
                     Success=False,
                     TranslationContainerName=tr_name,
                     Error=f"Failed to process message:\n{d}"
                 ))
     except Exception as e:
-        logger.exception(f"[-] exception in handleMythicToCustom for {tr_name}")
+        logger.exception(f"[-] exception in handleMythicToCustom for {tr_name}")
```

### Comparing `mythic_container-0.2.0rc9/mythic_container/__init__.py` & `mythic_container-0.2.1/mythic_container/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .rabbitmq import rabbitmqConnectionClass
 from .mythic_service import start_and_run_forever, test_command
 
-containerVersion = "v1.0.0-0.0.7"
+containerVersion = "v1.0.0-rc9"
 
-PyPi_version = "0.2.0-rc9"
+PyPi_version = "0.2.1"
 
 RabbitmqConnection = rabbitmqConnectionClass()
 
 MYTHIC_RPC_OTHER_SERVICES_RPC = "mythic_rpc_other_service_rpc"
 PAYLOAD_BUILD_C2_ROUTING_KEY = "payload_c2_build"
 # payload routes
 PT_SYNC_ROUTING_KEY = "pt_sync"
@@ -44,14 +44,16 @@
 TR_SYNC_ROUTING_KEY = "tr_sync"
 TR_RPC_RESYNC_ROUTING_KEY = "tr_rpc_resync"
 # webhook routes
 EMIT_WEBHOOK_ROUTING_KEY_PREFIX = "emit_webhook"
 WEBHOOK_TYPE_NEW_CALLBACK = "new_callback"
 WEBHOOK_TYPE_NEW_FEEDBACK = "new_feedback"
 WEBHOOK_TYPE_NEW_STARTUP = "new_startup"
+WEBHOOK_TYPE_NEW_ALERT = "new_alert"
+WEBHOOK_TYPE_NEW_CUSTOM = "new_custom"
 # log routes
 EMIT_LOG_ROUTING_KEY_PREFIX = "emit_log"
 LOG_TYPE_CALLBACK = "new_callback"
 LOG_TYPE_CREDENTIAL = "new_credential"
 LOG_TYPE_FILE = "new_file"
 LOG_TYPE_ARTIFACT = "new_artifact"
 LOG_TYPE_TASK = "new_task"
```

### Comparing `mythic_container-0.2.0rc9/mythic_container/agent_utils.py` & `mythic_container-0.2.1/mythic_container/agent_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import ujson
 from . import PayloadBuilder
 from . import MythicCommandBase
 import traceback
 import mythic_container
 from .utils_mythic_file_transfer import sendFileToMythic
 import asyncio
+from mythic_container.MythicRPC import *
 
 OPSEC_ROLE_LEAD = "lead"
 OPSEC_ROLE_OPERATOR = "operator"
 OPSEC_ROLE_OTHER_OPERATOR = "other_operator"
 
 
 async def makePayloadBuildResponse(buildMessage: dict, buildResponse: PayloadBuilder.BuildResponse) -> dict:
@@ -17,15 +18,16 @@
         response = {
             "uuid": buildMessage["uuid"],
             "agent_file_id": buildMessage["payload_file_uuid"],
             "success": True if str(buildResponse.get_status()) == "success" else False,
             "build_stderr": buildResponse.get_build_stderr(),
             "build_stdout": buildResponse.get_build_stdout(),
             "build_message": buildResponse.get_build_message(),
-            "updated_command_list": buildResponse.get_updated_command_list()
+            "updated_command_list": buildResponse.get_updated_command_list(),
+            "updated_filename": buildResponse.get_updated_filename()
         }
         if not response["success"]:
             if response["build_stderr"] == "":
                 response["build_stderr"] = response["build_message"]
         await uploadPayloadBuildResponse(buildMessage, buildResponse)
         return response
     except Exception as e:
@@ -39,26 +41,29 @@
 
 async def buildWrapper(msg: bytes) -> None:
     try:
         msgDict = ujson.loads(msg)
         for name, pt in PayloadBuilder.payloadTypes.items():
             if pt.name == msgDict["payload_type"]:
                 # go through all the data from rabbitmq to make the proper classes
+                commands = PayloadBuilder.CommandList(msgDict["commands"])
+                # go through all the data from rabbitmq to make the proper classes
                 c2info_list = []
-                for c2 in msgDict["c2profiles"]:
-                    params = c2.pop("parameters", None)
-                    c2info_list.append(
-                        PayloadBuilder.C2ProfileParameters(
-                            parameters=params, c2profile=c2
+                if msgDict["c2profiles"] is not None:
+                    for c2 in msgDict["c2profiles"]:
+                        params = c2.pop("parameters", None)
+                        c2info_list.append(
+                            PayloadBuilder.C2ProfileParameters(
+                                parameters=params, c2profile=c2
+                            )
                         )
-                    )
-                commands = PayloadBuilder.CommandList(msgDict["commands"])
                 agent_builder = pt.__class__(
                     uuid=msgDict["uuid"],
                     c2info=c2info_list,
+                    filename=msgDict["filename"],
                     selected_os=msgDict["selected_os"],
                     commands=commands,
                     wrapped_payload=msgDict["wrapped_payload"] if "wrapped_payload" in msgDict else None,
                 )
                 try:
                     await agent_builder.set_and_validate_build_parameters(msgDict["build_parameters"])
                     build_resp = await agent_builder.build()
@@ -316,15 +321,15 @@
                                 try:
                                     if hasattr(cmd, "create_go_tasking"):
                                         taskData = mythic_container.MythicCommandBase.PTTaskMessageAllData(**msgDict,
                                                                                                            args=cmd.argument_class)
                                         if not await verifyTaskArgs(taskData,
                                                                     mythic_container.PT_TASK_CREATE_TASKING_RESPONSE):
                                             return
-                                        createTaskingResponse = await cmd.create_go_tasking(taskData=taskData)
+                                        createTaskingResponse = await cmd.create_go_tasking(taskData)
                                         createTaskingResponse.Params = str(taskData.args)
                                         await mythic_container.RabbitmqConnection.SendDictDirectMessage(
                                             queue=mythic_container.PT_TASK_CREATE_TASKING_RESPONSE,
                                             body=createTaskingResponse.to_json()
                                         )
                                         return
                                     else:
@@ -389,14 +394,23 @@
             if pt.name == msgDict["task"]["payload_type"]:
                 if pt.name not in MythicCommandBase.commands:
                     logger.error(f"[-] no commands for payload type, can't do completion function")
                 else:
                     for cmd in MythicCommandBase.commands[pt.name]:
                         if cmd.cmd == msgDict["task"]["task"]["command_name"]:
                             completionFunctionInput = MythicCommandBase.PTTaskCompletionFunctionMessage(args=cmd.argument_class, **msgDict)
+                            if not await verifyTaskArgs(completionFunctionInput.TaskData, mythic_container.PT_TASK_COMPLETION_FUNCTION_RESPONSE):
+                                return
+                            if completionFunctionInput.SubtaskData is not None:
+                                for subcmd in MythicCommandBase.commands[pt.name]:
+                                    if subcmd.cmd == completionFunctionInput.SubtaskData.Task.CommandName:
+                                        completionFunctionInput.SubtaskData = MythicCommandBase.PTTaskMessageAllData(**msgDict["subtask"], args=subcmd.argument_class)
+                                        if not await verifyTaskArgs(completionFunctionInput.SubtaskData, mythic_container.PT_TASK_COMPLETION_FUNCTION_RESPONSE):
+                                            return
+                                        break
                             try:
                                 if completionFunctionInput.CompletionFunctionName in cmd.completion_functions:
                                     response = await cmd.completion_functions[
                                         completionFunctionInput.CompletionFunctionName](completionFunctionInput)
                                 else:
                                     response = mythic_container.MythicCommandBase.PTTaskCompletionFunctionMessageResponse(
                                         Success=False,
```

### Comparing `mythic_container-0.2.0rc9/mythic_container/c2_utils.py` & `mythic_container-0.2.1/mythic_container/c2_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,24 +18,28 @@
         pass
     except Exception as e:
         logger.exception(f"[-] Failed to kill process: {e}")
 
 
 async def deal_with_stdout(c2_profile: str) -> str:
     output = ""
-    try:
-        line = await asyncio.wait_for(mythic_container.C2ProfileBase.runningServers[c2_profile]["process"].stdout.readline(), timeout=3.0)
-        #async for line in mythic_container.C2ProfileBase.runningServers[c2_profile]["process"].stdout:
-        #    output += line.decode()
-        output += line.decode()
-    except asyncio.TimeoutError:
-        pass
-    except Exception as e:
-        logger.exception(f"hit exception trying to get server output: {traceback.format_exc()}")
-
+    lines = 0
+    while True:
+        try:
+            line = await asyncio.wait_for(
+                mythic_container.C2ProfileBase.runningServers[c2_profile]["process"].stdout.readline(), timeout=3.0)
+            output += line.decode()
+            lines += 1
+            if lines > 100:
+                break
+        except asyncio.TimeoutError:
+            break
+        except Exception as e:
+            logger.exception(f"hit exception trying to get server output: {traceback.format_exc()}")
+            return output + traceback.format_exc()
     return output
 
 
 async def opsecChecks(msg: bytes) -> bytes:
     try:
         msgDict = ujson.loads(msg)
         for name, c2 in mythic_container.C2ProfileBase.c2Profiles.items():
@@ -315,15 +319,15 @@
             mythic_container.C2ProfileBase.runningServers[c2.name] = {
                 "process": None
             }
         path = c2.server_binary_path.resolve()
         cwd = c2.server_folder_path.resolve()
         os.chmod(path, mode=0o777)
         process = await asyncio.create_subprocess_shell(cmd=str(path), stdout=subprocess.PIPE, stderr=subprocess.STDOUT,
-                                                        shell=True, cwd=str(cwd))
+                                                        shell=True, cwd=str(cwd), env=os.environ.copy())
         mythic_container.C2ProfileBase.runningServers[c2.name]["process"] = process
         await asyncio.sleep(3)
         if process.returncode is not None:
             # this means something went wrong and the process is dead
             return mythic_container.C2ProfileBase.C2StartServerMessageResponse(
                 Success=False,
                 Error=f"Failed to start\nOutput:\n{await deal_with_stdout(c2.name)}",
@@ -413,15 +417,16 @@
                         try:
                             kill(mythic_container.C2ProfileBase.runningServers[c2.name]["process"].pid)
                         except Exception as e:
                             pass
                         # now try to start it again
                         await asyncio.sleep(3)
                         response = mythic_container.C2ProfileBase.C2StopServerMessageResponse(
-                            Success=True, Error="", Message=f"Stopped server:\nOutput:{await deal_with_stdout(c2.name)}",
+                            Success=True, Error="",
+                            Message=f"Stopped server:\nOutput:{await deal_with_stdout(c2.name)}",
                             InternalServerRunning=False
                         )
                         mythic_container.C2ProfileBase.runningServers[c2.name]["output"] = ""
                         return ujson.dumps(response.to_json()).encode()
                 else:
                     # just means we've never started it before, so start it now
                     response = mythic_container.C2ProfileBase.C2StopServerMessageResponse(
@@ -518,8 +523,8 @@
         for name, c2 in mythic_container.C2ProfileBase.c2Profiles.items():
             if c2.name == msgDict["c2_profile_name"]:
                 await mythic_container.mythic_service.syncC2ProfileData(c2)
                 return ujson.dumps({"success": True}).encode()
         return ujson.dumps({"success": False, "error": "Failed to find c2 profile"}).encode()
     except Exception as e:
         logger.exception(f"Failed to re-sync c2 profile: {e}")
-        return ujson.dumps({"success": False, "error": f"Failed to sync: {traceback.format_exc()}\n{e}"}).encode()
+        return ujson.dumps({"success": False, "error": f"Failed to sync: {traceback.format_exc()}\n{e}"}).encode()
```

### Comparing `mythic_container-0.2.0rc9/mythic_container/grpc/translationContainerGRPC_pb2.py` & `mythic_container-0.2.1/mythic_container/grpc/translationContainerGRPC_pb2.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/grpc/translationContainerGRPC_pb2_grpc.py` & `mythic_container-0.2.1/mythic_container/grpc/translationContainerGRPC_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/logging.py` & `mythic_container-0.2.1/mythic_container/logging.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/mythic_service.py` & `mythic_container-0.2.1/mythic_container/mythic_service.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 from .logging import logger, initialize
 from . import agent_utils
 from . import MythicGoRPC
 from . import C2ProfileBase
 from . import c2_utils
 from . import TranslationBase
 from . import WebhookBase
+from . import LoggingBase
 from . import webhook_utils
+from . import logging_utils
 from .rabbitmq import failedConnectRetryDelay
 
 
 # set the global hostname variable
 output = ""
 
 
@@ -35,14 +37,18 @@
     return f"{containerName}_{baseKey}"
 
 
 def getWebhookRoutingKey(webhookType: str) -> str:
     return f"{mythic_container.EMIT_WEBHOOK_ROUTING_KEY_PREFIX}.{webhookType}"
 
 
+def getLoggingRoutingKey(loggingType: str) -> str:
+    return f"{mythic_container.EMIT_LOG_ROUTING_KEY_PREFIX}.{loggingType}"
+
+
 payloadQueueTasks = []
 
 
 async def startPayloadRabbitMQ(pt: PayloadBuilder.PayloadType) -> None:
     payloadQueueTasks.append(asyncio.create_task(mythic_container.RabbitmqConnection.ReceiveFromMythicDirectExchange(
         queue=getRoutingKey(pt.name, mythic_container.PAYLOAD_BUILD_ROUTING_KEY),
         routing_key=getRoutingKey(pt.name, mythic_container.PAYLOAD_BUILD_ROUTING_KEY),
@@ -254,27 +260,92 @@
         )))
     if wb.new_feedback is not None and callable(wb.new_feedback):
         payloadQueueTasks.append(asyncio.create_task(mythic_container.RabbitmqConnection.ReceiveFromMythicDirectTopicExchange(
             queue=getWebhookRoutingKey(mythic_container.WEBHOOK_TYPE_NEW_FEEDBACK),
             routing_key=getWebhookRoutingKey(mythic_container.WEBHOOK_TYPE_NEW_FEEDBACK),
             handler=webhook_utils.new_feedback
         )))
+    if wb.new_alert is not None and callable(wb.new_alert):
+        payloadQueueTasks.append(asyncio.create_task(mythic_container.RabbitmqConnection.ReceiveFromMythicDirectTopicExchange(
+            queue=getWebhookRoutingKey(mythic_container.WEBHOOK_TYPE_NEW_ALERT),
+            routing_key=getWebhookRoutingKey(mythic_container.WEBHOOK_TYPE_NEW_ALERT),
+            handler=webhook_utils.new_alert
+        )))
+    if wb.new_custom is not None and callable(wb.new_custom):
+        payloadQueueTasks.append(asyncio.create_task(mythic_container.RabbitmqConnection.ReceiveFromMythicDirectTopicExchange(
+            queue=getWebhookRoutingKey(mythic_container.WEBHOOK_TYPE_NEW_CUSTOM),
+            routing_key=getWebhookRoutingKey(mythic_container.WEBHOOK_TYPE_NEW_CUSTOM),
+            handler=webhook_utils.new_custom
+        )))
     logger.info(f"Successfully started webhook service")
 
+
+async def syncLoggingData(wb: LoggingBase.Log) -> None:
+    if wb.new_callback is not None and callable(wb.new_callback):
+        payloadQueueTasks.append(asyncio.create_task(mythic_container.RabbitmqConnection.ReceiveFromMythicDirectTopicExchange(
+            queue=getLoggingRoutingKey(mythic_container.LOG_TYPE_CALLBACK),
+            routing_key=getLoggingRoutingKey(mythic_container.LOG_TYPE_CALLBACK),
+            handler=logging_utils.new_callback
+        )))
+    if wb.new_credential is not None and callable(wb.new_credential):
+        payloadQueueTasks.append(asyncio.create_task(mythic_container.RabbitmqConnection.ReceiveFromMythicDirectTopicExchange(
+            queue=getLoggingRoutingKey(mythic_container.LOG_TYPE_CREDENTIAL),
+            routing_key=getLoggingRoutingKey(mythic_container.LOG_TYPE_CREDENTIAL),
+            handler=logging_utils.new_credential
+        )))
+    if wb.new_keylog is not None and callable(wb.new_keylog):
+        payloadQueueTasks.append(asyncio.create_task(mythic_container.RabbitmqConnection.ReceiveFromMythicDirectTopicExchange(
+            queue=getLoggingRoutingKey(mythic_container.LOG_TYPE_KEYLOG),
+            routing_key=getLoggingRoutingKey(mythic_container.LOG_TYPE_KEYLOG),
+            handler=logging_utils.new_keylog
+        )))
+    if wb.new_file is not None and callable(wb.new_file):
+        payloadQueueTasks.append(asyncio.create_task(mythic_container.RabbitmqConnection.ReceiveFromMythicDirectTopicExchange(
+            queue=getLoggingRoutingKey(mythic_container.LOG_TYPE_FILE),
+            routing_key=getLoggingRoutingKey(mythic_container.LOG_TYPE_FILE),
+            handler=logging_utils.new_file
+        )))
+    if wb.new_payload is not None and callable(wb.new_payload):
+        payloadQueueTasks.append(asyncio.create_task(mythic_container.RabbitmqConnection.ReceiveFromMythicDirectTopicExchange(
+            queue=getLoggingRoutingKey(mythic_container.LOG_TYPE_PAYLOAD),
+            routing_key=getLoggingRoutingKey(mythic_container.LOG_TYPE_PAYLOAD),
+            handler=logging_utils.new_payload
+        )))
+    if wb.new_artifact is not None and callable(wb.new_artifact):
+        payloadQueueTasks.append(asyncio.create_task(mythic_container.RabbitmqConnection.ReceiveFromMythicDirectTopicExchange(
+            queue=getLoggingRoutingKey(mythic_container.LOG_TYPE_ARTIFACT),
+            routing_key=getLoggingRoutingKey(mythic_container.LOG_TYPE_ARTIFACT),
+            handler=logging_utils.new_artifact
+        )))
+    if wb.new_task is not None and callable(wb.new_task):
+        payloadQueueTasks.append(asyncio.create_task(mythic_container.RabbitmqConnection.ReceiveFromMythicDirectTopicExchange(
+            queue=getLoggingRoutingKey(mythic_container.LOG_TYPE_TASK),
+            routing_key=getLoggingRoutingKey(mythic_container.LOG_TYPE_TASK),
+            handler=logging_utils.new_task
+        )))
+
+    logger.info(f"Successfully started logging service")
+
 consumingServices = []
 async def start_services():
     initialize()
 
     logger.info(f"[+] Starting Services with version {mythic_container.containerVersion} and PyPi version {mythic_container.PyPi_version}\n")
     webhook_services = WebhookBase.Webhook.__subclasses__()
     for cls in webhook_services:
         logger.info(f"[*] Processing webhook service")
         webhook = cls()
         consumingServices.append(webhook)
         await syncWebhookData(webhook)
+    logging_services = LoggingBase.Log.__subclasses__()
+    for cls in logging_services:
+        logger.info(f"[*] Processing logging services")
+        definedLog = cls()
+        consumingServices.append(definedLog)
+        await syncLoggingData(definedLog)
     payloadTypes = PayloadBuilder.PayloadType.__subclasses__()
     for cls in payloadTypes:
         payload_type = cls()
         if payload_type.name in PayloadBuilder.payloadTypes:
             logger.error(f"[-] attempting to import {payload_type.name} multiple times - probably due to import issues")
             continue
         PayloadBuilder.payloadTypes[payload_type.name] = payload_type
@@ -300,16 +371,14 @@
             logger.error(f"[-] attempting to import {translator.name} multiple times - probably due to import issues")
             continue
         TranslationBase.translationServices[translator.name] = translator
         logger.info(f"[*] Processing translation service: {translator.name}")
         await syncTranslatorData(translator)
         await startTranslatorRabbitMQ(translator)
 
-
-
     logger.info("[+] All services initialized!")
 
 
 async def test_command(payload_type_name: str,
                        command_name: str,
                        operation_name: str = None,
                        task_id: int = None,
```

### Comparing `mythic_container-0.2.0rc9/mythic_container/rabbitmq.py` & `mythic_container-0.2.1/mythic_container/rabbitmq.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,28 +101,28 @@
                     logger.error(f"[-] Failed to connect to rabbitmq: {e}")
                     await asyncio.sleep(failedConnectRetryDelay)
 
     async def SendMessage(self, queue: str, body: bytes):
         while True:
             try:
                 connection = await self.GetConnection()
-                chan = await connection.channel(publisher_confirms=True,
-                                                on_return_raises=True)
-                exchange = await chan.declare_exchange("mythic_exchange",
-                                                       durable=True,
-                                                       auto_delete=True)
-                message = aio_pika.Message(body=body,
-                                           content_type="application/json")
-                await exchange.publish(
-                    message=message,
-                    routing_key=queue,
-                    timeout=failedConnectRetryDelay,
-                    mandatory=True,
-                    immediate=False)
-                return
+                async with connection.channel(publisher_confirms=True,
+                                              on_return_raises=True) as chan:
+                    exchange = await chan.declare_exchange("mythic_exchange",
+                                                           durable=True,
+                                                           auto_delete=True)
+                    message = aio_pika.Message(body=body,
+                                               content_type="application/json")
+                    await exchange.publish(
+                        message=message,
+                        routing_key=queue,
+                        timeout=failedConnectRetryDelay,
+                        mandatory=True,
+                        immediate=False)
+                    return
             except Exception as e:
                 logger.exception(f"[-] failed to send message: {e}")
                 return
 
     async def SendDictDirectMessage(self, queue: str, body: dict) -> None:
         #logger.debug(f"Sending Direct msg to {queue}: {body}")
         return await self.SendMessage(queue=queue, body=ujson.dumps(body).encode())
@@ -131,34 +131,34 @@
         future = asyncio.get_event_loop().create_future()
         logger.debug(f"Sending RPC message to {queue}")
         try:
             correlation_id = str(uuid.uuid4())
             self.futures[correlation_id] = future
             while True:
                 connection = await self.GetConnection()
-                chan = await connection.channel(on_return_raises=True)
-                exchange = await chan.declare_exchange("mythic_exchange",
-                                                       durable=True,
-                                                       auto_delete=True)
-                callback_queue = await chan.declare_queue(name="amq.rabbitmq.reply-to",)
-                await callback_queue.consume(self.on_response,
-                                             no_ack=True)
-                message = aio_pika.Message(body=body,
-                                           content_type="application/json",
-                                           reply_to=callback_queue.name,
-                                           correlation_id=correlation_id)
-                # make sure the queue exists first before we try to send to it
-                await exchange.publish(
-                    message=message,
-                    routing_key=queue,
-                    mandatory=True,
-                    immediate=False,
-                )
-                result = await future
-                return result
+                async with connection.channel(on_return_raises=True) as chan:
+                    exchange = await chan.declare_exchange("mythic_exchange",
+                                                           durable=True,
+                                                           auto_delete=True)
+                    callback_queue = await chan.declare_queue(name="amq.rabbitmq.reply-to",)
+                    await callback_queue.consume(self.on_response,
+                                                 no_ack=True)
+                    message = aio_pika.Message(body=body,
+                                               content_type="application/json",
+                                               reply_to=callback_queue.name,
+                                               correlation_id=correlation_id)
+                    # make sure the queue exists first before we try to send to it
+                    await exchange.publish(
+                        message=message,
+                        routing_key=queue,
+                        mandatory=True,
+                        immediate=False,
+                    )
+                    result = await future
+                    return result
         except Exception as e:
             logger.error(f"[-] failed to send rpc message to {queue}: {e}")
             future.set_result({})
             return {}
 
     def on_response(self, message: aio_pika.abc.AbstractIncomingMessage) -> None:
         try:
@@ -184,131 +184,130 @@
     async def SendRPCDictMessage(self, queue: str, body: dict) -> dict:
         #logger.debug(f"Sending RPC msg: {body}")
         return await self.SendRPCMessage(queue=queue, body=ujson.dumps(body).encode())
 
     async def ReplyMessage(self, response: bytes, message: aio_pika.abc.AbstractIncomingMessage):
         try:
             connection = await self.GetConnection()
-            chan = await connection.channel(
-                                            on_return_raises=True)
-            exchange = chan.default_exchange
-            newMessage = aio_pika.Message(
-                body=response,
-                content_type="application/json",
-                correlation_id=message.correlation_id)
-
-            await exchange.publish(
-                newMessage,
-                routing_key=message.reply_to,
-                mandatory=False
-            )
+            async with connection.channel(on_return_raises=True) as chan:
+                exchange = chan.default_exchange
+                newMessage = aio_pika.Message(
+                    body=response,
+                    content_type="application/json",
+                    correlation_id=message.correlation_id)
+
+                await exchange.publish(
+                    newMessage,
+                    routing_key=message.reply_to,
+                    mandatory=False
+                )
 
         except Exception as e:
             logger.exception(f"[-] failed to send reply message: {e}")
             pass
 
     async def ReceiveFromMythicDirectExchange(self, queue: str, routing_key: str,
                                               handler: Coroutine[any, any, None]):
         while True:
             try:
                 connection = await self.GetConnection()
-                chan = await connection.channel()
-                exchange = await chan.declare_exchange(
-                    name="mythic_exchange",
-                    type="direct",
-                    durable=True,
-                    auto_delete=True,
-                    internal=False,
-                )
-                q = await chan.declare_queue(
-                    name=queue,
-                    durable=False,
-                    auto_delete=True,
-                    exclusive=False,
-                )
-                await q.bind(
-                    exchange=exchange,
-                    routing_key=routing_key,
-                )
-                await q.consume(
-                    callback=partial(directExchangeCallback, trueFunction=handler)
-                )
-                logger.info(f"[*] started listening for messages on {queue}")
-                try:
-                    await asyncio.Future()
-                    logger.error(f"asyncio.Future() finished in ReceiveFromMythicDirectExchange for {queue}")
-                except Exception as directException:
-                    logger.exception(f"[-] exception trying to listen for direct messages on {queue}\n{directException}")
+                async with connection.channel() as chan:
+                    exchange = await chan.declare_exchange(
+                        name="mythic_exchange",
+                        type="direct",
+                        durable=True,
+                        auto_delete=True,
+                        internal=False,
+                    )
+                    q = await chan.declare_queue(
+                        name=queue,
+                        durable=False,
+                        auto_delete=True,
+                        exclusive=False,
+                    )
+                    await q.bind(
+                        exchange=exchange,
+                        routing_key=routing_key,
+                    )
+                    await q.consume(
+                        callback=partial(directExchangeCallback, trueFunction=handler)
+                    )
+                    logger.info(f"[*] started listening for messages on {queue}")
+                    try:
+                        await asyncio.Future()
+                        logger.error(f"asyncio.Future() finished in ReceiveFromMythicDirectExchange for {queue}")
+                    except Exception as directException:
+                        logger.exception(f"[-] exception trying to listen for direct messages on {queue}\n{directException}")
             except Exception as e:
                 logger.exception(f"[-] stopped listening for messages on {queue}, {e}")
                 await asyncio.sleep(failedConnectRetryDelay)
 
     async def ReceiveFromRPCQueue(self, queue: str, routing_key: str, handler: Coroutine[any, any, None]):
         while True:
             try:
                 connection = await self.GetConnection()
-                chan = await connection.channel()
-                exchange = await chan.declare_exchange(
-                    name="mythic_exchange",
-                    type="direct",
-                    durable=True,
-                    auto_delete=True,
-                    internal=False,
-
-                )
-                q = await chan.declare_queue(
-                    name=queue,
-                    durable=False,
-                    auto_delete=True,
-                    exclusive=True,
-                )
-                await q.bind(
-                    exchange=exchange,
-                    routing_key=routing_key,
-                )
-                await q.consume(
-                    callback=partial(rpcExchangeCallback, trueFunction=handler)
-                )
-                logger.info(f"[*] started listening for messages on {queue}")
-                try:
-                    await asyncio.Future()
-                finally:
-                    logger.error(f"asyncio.Future() finished in ReceiveFromRPCQueue for queue {queue}")
+                async with connection.channel() as chan:
+                    exchange = await chan.declare_exchange(
+                        name="mythic_exchange",
+                        type="direct",
+                        durable=True,
+                        auto_delete=True,
+                        internal=False,
+
+                    )
+                    q = await chan.declare_queue(
+                        name=queue,
+                        durable=False,
+                        auto_delete=True,
+                        exclusive=True,
+                    )
+                    await q.bind(
+                        exchange=exchange,
+                        routing_key=routing_key,
+                    )
+                    await q.consume(
+                        callback=partial(rpcExchangeCallback, trueFunction=handler)
+                    )
+                    logger.info(f"[*] started listening for messages on {queue}")
+                    try:
+                        await asyncio.Future()
+                    finally:
+                        logger.error(f"asyncio.Future() finished in ReceiveFromRPCQueue for queue {queue}")
             except Exception as e:
                 logger.exception(f"[-] stopped listening for messages on {queue}, {e}")
                 await asyncio.sleep(failedConnectRetryDelay)
 
     async def ReceiveFromMythicDirectTopicExchange(self, queue: str, routing_key: str,
                                                    handler: Coroutine[any, any, None]):
         while True:
             try:
                 connection = await self.GetConnection()
-                chan = await connection.channel()
-                exchange = await chan.declare_exchange(
-                    name="mythic_topic_exchange",
-                    type="topic",
-                    durable=True,
-                    auto_delete=True,
-                    internal=False,
-                )
-                q = await chan.declare_queue(
-                    name="",
-                    durable=False,
-                    auto_delete=True,
-                    exclusive=False,
-                )
-                await q.bind(
-                    exchange=exchange,
-                    routing_key=queue,
-                )
-                await q.consume(
-                    callback=partial(directExchangeCallback, trueFunction=handler)
-                )
-                logger.info(f"[*] started listening for messages on {queue}")
-                try:
-                    await asyncio.Future()
-                    logger.error(f"asyncio.Future() finished in ReceiveFromMythicDirectTopicExchange for {queue}")
-                except Exception as directException:
-                    logger.exception(f"[-] exception trying to listen for direct messages on {queue}\n{directException}")
+                async with connection.channel() as chan:
+                    exchange = await chan.declare_exchange(
+                        name="mythic_topic_exchange",
+                        type="topic",
+                        durable=True,
+                        auto_delete=True,
+                        internal=False,
+                    )
+                    q = await chan.declare_queue(
+                        name="",
+                        durable=False,
+                        auto_delete=True,
+                        exclusive=False,
+                    )
+                    await q.bind(
+                        exchange=exchange,
+                        routing_key=queue,
+                    )
+                    await q.consume(
+                        callback=partial(directExchangeCallback, trueFunction=handler)
+                    )
+                    logger.info(f"[*] started listening for messages on {queue}")
+                    try:
+                        await asyncio.Future()
+                        logger.error(f"asyncio.Future() finished in ReceiveFromMythicDirectTopicExchange for {queue}")
+                    except Exception as directException:
+                        logger.exception(f"[-] exception trying to listen for direct messages on {queue}\n{directException}")
             except Exception as e:
                 logger.exception(f"[-] stopped listening for messages on {queue}, {e}")
                 await asyncio.sleep(failedConnectRetryDelay)
```

### Comparing `mythic_container-0.2.0rc9/mythic_container/utils_mythic_file_transfer.py` & `mythic_container-0.2.1/mythic_container/utils_mythic_file_transfer.py`

 * *Files identical despite different names*

### Comparing `mythic_container-0.2.0rc9/mythic_container/webhook_utils.py` & `mythic_container-0.2.1/mythic_container/webhook_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,40 +6,68 @@
 async def new_startup(msg: bytes) -> None:
     try:
         msgDict = ujson.loads(msg)
         webhookServices = Webhook.__subclasses__()
         for cls in webhookServices:
             webhook = cls()
             if webhook.new_startup is not None and callable(webhook.new_startup):
-                await webhook.new_startup(WebookMessage(**msgDict))
+                await webhook.new_startup(WebhookMessage(**msgDict))
             else:
                 logger.error(f"No valid function for new_startup from webhook")
     except Exception as e:
         logger.exception(f"Failed to execute new_startup webhook: {e}")
 
 
 async def new_callback(msg: bytes) -> None:
     try:
         msgDict = ujson.loads(msg)
         webhookServices = Webhook.__subclasses__()
         for cls in webhookServices:
             webhook = cls()
             if webhook.new_callback is not None and callable(webhook.new_callback):
-                await webhook.new_callback(WebookMessage(**msgDict))
+                await webhook.new_callback(WebhookMessage(**msgDict))
             else:
                 logger.error(f"No valid function for new_callback from webhook")
     except Exception as e:
         logger.exception(f"Failed to execute new_callback webhook: {e}")
 
 
 async def new_feedback(msg: bytes) -> None:
     try:
         msgDict = ujson.loads(msg)
         webhookServices = Webhook.__subclasses__()
         for cls in webhookServices:
             webhook = cls()
             if webhook.new_feedback is not None and callable(webhook.new_feedback):
-                await webhook.new_feedback(WebookMessage(**msgDict))
+                await webhook.new_feedback(WebhookMessage(**msgDict))
             else:
                 logger.error(f"No valid function for new_feedback from webhook")
     except Exception as e:
-        logger.exception(f"Failed to execute new_feedback webhook: {e}")
+        logger.exception(f"Failed to execute new_feedback webhook: {e}")
+
+
+async def new_alert(msg: bytes) -> None:
+    try:
+        msgDict = ujson.loads(msg)
+        webhookServices = Webhook.__subclasses__()
+        for cls in webhookServices:
+            webhook = cls()
+            if webhook.new_alert is not None and callable(webhook.new_alert):
+                await webhook.new_alert(WebhookMessage(**msgDict))
+            else:
+                logger.error(f"No valid function for new_alert from webhook")
+    except Exception as e:
+        logger.exception(f"Failed to execute new_alert webhook: {e}")
+
+
+async def new_custom(msg: bytes) -> None:
+    try:
+        msgDict = ujson.loads(msg)
+        webhookServices = Webhook.__subclasses__()
+        for cls in webhookServices:
+            webhook = cls()
+            if webhook.new_custom is not None and callable(webhook.new_custom):
+                await webhook.new_custom(WebhookMessage(**msgDict))
+            else:
+                logger.error(f"No valid function for new_custom from webhook")
+    except Exception as e:
+        logger.exception(f"Failed to execute new_custom webhook: {e}")
```

### Comparing `mythic_container-0.2.0rc9/mythic_container.egg-info/PKG-INFO` & `mythic_container-0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mythic-container
-Version: 0.2.0rc9
+Name: mythic_container
+Version: 0.2.1
 Summary: Functionality for Mythic Services
 Home-page: https://docs.mythic-c2.net/customizing/payload-type-development
 Author: @its_a_feature_
 Author-email: 
 License: BSD3
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -23,15 +23,15 @@
 
 ```
 pip install mythic-container
 ```
 
 ## How to use
 
-This container reports to mythic as version "v1.0.0" (PyPi version 0.1.18). Use it with Mythic version 3.0.0.
+Use it with Mythic version 3.0.0.
 
 For the main execution of the heartbeat and service functionality, simply import and start the service:
 ```
 import mythic_container
 import [my agent | my c2 profile | my translation container | my webhooks | my loggers]
 mythic_container.mythic_service.start_and_run_forever()
 ```
```

### Comparing `mythic_container-0.2.0rc9/mythic_container.egg-info/SOURCES.txt` & `mythic_container-0.2.1/mythic_container.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 mythic_container/TranslationBase.py
 mythic_container/WebhookBase.py
 mythic_container/__init__.py
 mythic_container/agent_utils.py
 mythic_container/c2_utils.py
 mythic_container/config.py
 mythic_container/logging.py
+mythic_container/logging_utils.py
 mythic_container/mythic_service.py
 mythic_container/rabbitmq.py
 mythic_container/utils_mythic_file_transfer.py
 mythic_container/webhook_utils.py
 mythic_container.egg-info/PKG-INFO
 mythic_container.egg-info/SOURCES.txt
 mythic_container.egg-info/dependency_links.txt
@@ -35,15 +36,15 @@
 mythic_container/MythicGoRPC/send_mythic_rpc_callback_encrypt_bytes.py
 mythic_container/MythicGoRPC/send_mythic_rpc_callback_remove_command.py
 mythic_container/MythicGoRPC/send_mythic_rpc_callback_search.py
 mythic_container/MythicGoRPC/send_mythic_rpc_callback_search_command.py
 mythic_container/MythicGoRPC/send_mythic_rpc_callback_update.py
 mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_create.py
 mythic_container/MythicGoRPC/send_mythic_rpc_callbacktoken_remove.py
-mythic_container/MythicGoRPC/send_mythic_rpc_command_search.py
+mythic_container/MythicGoRPC/send_mythic_rpc_command_search_.py
 mythic_container/MythicGoRPC/send_mythic_rpc_credential_create.py
 mythic_container/MythicGoRPC/send_mythic_rpc_credential_search.py
 mythic_container/MythicGoRPC/send_mythic_rpc_file_create.py
 mythic_container/MythicGoRPC/send_mythic_rpc_file_get_content.py
 mythic_container/MythicGoRPC/send_mythic_rpc_file_register.py
 mythic_container/MythicGoRPC/send_mythic_rpc_file_search.py
 mythic_container/MythicGoRPC/send_mythic_rpc_file_update.py
```

### Comparing `mythic_container-0.2.0rc9/setup.py` & `mythic_container-0.2.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="mythic_container",
-    version="0.2.0-rc9",
+    version="0.2.1",
     description="Functionality for Mythic Services",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://docs.mythic-c2.net/customizing/payload-type-development",
     author="@its_a_feature_",
     author_email="",
     license="BSD3",
```

