# Comparing `tmp/PyroFork-dev-2.2.6.dev202307272537.tar.gz` & `tmp/PyroFork-dev-2.2.6.dev202308012705.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyroFork-dev-2.2.6.dev202307272537.tar", last modified: Thu Jul 27 08:14:36 2023, max compression
+gzip compressed data, was "PyroFork-dev-2.2.6.dev202308012705.tar", last modified: Tue Aug  1 12:00:37 2023, max compression
```

## Comparing `PyroFork-dev-2.2.6.dev202307272537.tar` & `PyroFork-dev-2.2.6.dev202308012705.tar`

### file list

```diff
@@ -1,532 +1,532 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.935493 PyroFork-dev-2.2.6.dev202307272537/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/COPYING.lesser
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-07-27 08:14:36.935493 PyroFork-dev-2.2.6.dev202307272537/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.879493 PyroFork-dev-2.2.6.dev202307272537/PyroFork_dev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-07-27 08:14:36.000000 PyroFork-dev-2.2.6.dev202307272537/PyroFork_dev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20482 2023-07-27 08:14:36.000000 PyroFork-dev-2.2.6.dev202307272537/PyroFork_dev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 08:14:36.000000 PyroFork-dev-2.2.6.dev202307272537/PyroFork_dev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 08:14:36.000000 PyroFork-dev-2.2.6.dev202307272537/PyroFork_dev.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-27 08:14:36.000000 PyroFork-dev-2.2.6.dev202307272537/PyroFork_dev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-27 08:14:36.000000 PyroFork-dev-2.2.6.dev202307272537/PyroFork_dev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.879493 PyroFork-dev-2.2.6.dev202307272537/compiler/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.879493 PyroFork-dev-2.2.6.dev202307272537/compiler/api/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/compiler/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22402 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/compiler/api/compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.879493 PyroFork-dev-2.2.6.dev202307272537/compiler/api/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/compiler/api/source/auth_key.tl
--rw-r--r--   0 runner    (1001) docker     (123)   175007 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/compiler/api/source/main_api.tl
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/compiler/api/source/sys_msgs.tl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.879493 PyroFork-dev-2.2.6.dev202307272537/compiler/api/template/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/compiler/api/template/combinator.txt
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/compiler/api/template/type.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.879493 PyroFork-dev-2.2.6.dev202307272537/compiler/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/compiler/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19579 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/compiler/docs/compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.879493 PyroFork-dev-2.2.6.dev202307272537/compiler/docs/template/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/compiler/docs/template/page.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/compiler/docs/template/toctree.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.883493 PyroFork-dev-2.2.6.dev202307272537/compiler/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/compiler/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/compiler/errors/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/compiler/errors/sort.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.883493 PyroFork-dev-2.2.6.dev202307272537/compiler/errors/source/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/compiler/errors/source/303_SEE_OTHER.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    22907 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/compiler/errors/source/400_BAD_REQUEST.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/compiler/errors/source/401_UNAUTHORIZED.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/compiler/errors/source/403_FORBIDDEN.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/compiler/errors/source/420_FLOOD.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.883493 PyroFork-dev-2.2.6.dev202307272537/compiler/errors/template/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/compiler/errors/template/class.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/compiler/errors/template/sub_class.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.883493 PyroFork-dev-2.2.6.dev202307272537/pyrogram/
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-27 08:14:29.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41006 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.883493 PyroFork-dev-2.2.6.dev202307272537/pyrogram/connection/
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/connection/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.883493 PyroFork-dev-2.2.6.dev202307272537/pyrogram/connection/transport/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/connection/transport/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.887493 PyroFork-dev-2.2.6.dev202307272537/pyrogram/connection/transport/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/connection/transport/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/connection/transport/tcp/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/connection/transport/tcp/tcp_abridged.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/connection/transport/tcp/tcp_abridged_o.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/connection/transport/tcp/tcp_full.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/connection/transport/tcp/tcp_intermediate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/connection/transport/tcp/tcp_intermediate_o.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.887493 PyroFork-dev-2.2.6.dev202307272537/pyrogram/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/crypto/aes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/crypto/mtproto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/crypto/prime.py
--rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/crypto/rsa.py
--rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)   208021 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/emoji.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.887493 PyroFork-dev-2.2.6.dev202307272537/pyrogram/enums/
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/enums/auto_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/enums/chat_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/enums/chat_event_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/enums/chat_member_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/enums/chat_members_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/enums/chat_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/enums/message_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/enums/message_media_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/enums/message_service_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/enums/messages_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/enums/next_code_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/enums/parse_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/enums/poll_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/enums/sent_code_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/enums/user_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.887493 PyroFork-dev-2.2.6.dev202307272537/pyrogram/errors/
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/errors/rpc_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/file_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    24836 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.891492 PyroFork-dev-2.2.6.dev202307272537/pyrogram/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/handlers/callback_query_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/handlers/chat_join_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/handlers/chat_member_updated_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/handlers/chosen_inline_result_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/handlers/deleted_messages_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/handlers/disconnect_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/handlers/edited_message_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/handlers/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/handlers/inline_query_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/handlers/message_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/handlers/poll_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/handlers/raw_update_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/handlers/user_status_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.891492 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.891492 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/advanced/
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/advanced/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/advanced/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/advanced/resolve_peer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/advanced/save_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.891492 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/auth/
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/auth/accept_terms_of_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/auth/check_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/auth/connect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/auth/disconnect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/auth/get_password_hint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/auth/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/auth/log_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/auth/recover_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/auth/resend_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/auth/send_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/auth/send_recovery_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/auth/sign_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/auth/sign_in_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/auth/sign_up.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/auth/terminate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.895493 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/bots/
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/bots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/bots/answer_callback_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/bots/answer_inline_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/bots/answer_web_app_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/bots/delete_bot_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/bots/get_bot_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/bots/get_bot_default_privileges.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/bots/get_bot_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/bots/get_chat_menu_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/bots/get_game_high_scores.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/bots/get_inline_bot_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/bots/request_callback_answer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/bots/send_game.py
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/bots/send_inline_bot_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/bots/set_bot_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/bots/set_bot_default_privileges.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/bots/set_bot_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/bots/set_chat_menu_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/bots/set_game_score.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.899493 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/add_chat_members.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/archive_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/ban_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/close_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/close_general_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/create_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/create_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/create_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/create_supergroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/delete_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/delete_chat_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/delete_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/delete_supergroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/delete_user_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/edit_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/edit_general_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/get_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/get_chat_event_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/get_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/get_chat_members.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/get_chat_members_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/get_chat_online_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/get_dialogs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/get_dialogs_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/get_forum_topics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/get_forum_topics_by_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/get_nearby_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/get_send_as_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/hide_general_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/join_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/leave_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/mark_chat_unread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/pin_chat_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/promote_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/reopen_forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/reopen_general_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/restrict_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/set_administrator_title.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/set_chat_description.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/set_chat_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/set_chat_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/set_chat_protected_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/set_chat_title.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/set_chat_username.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/set_send_as_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/set_slow_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/unarchive_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/unban_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/unhide_general_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/unpin_all_chat_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/unpin_chat_message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.899493 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/contacts/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/contacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/contacts/add_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/contacts/delete_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/contacts/get_contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/contacts/get_contacts_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/contacts/import_contacts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.903493 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/decorators/on_callback_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/decorators/on_chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/decorators/on_chat_member_updated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/decorators/on_chosen_inline_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/decorators/on_deleted_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/decorators/on_disconnect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/decorators/on_edited_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/decorators/on_inline_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/decorators/on_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/decorators/on_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/decorators/on_raw_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/decorators/on_user_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.903493 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/invite_links/
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/invite_links/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/invite_links/approve_all_chat_join_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/invite_links/approve_chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/invite_links/create_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/invite_links/decline_all_chat_join_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/invite_links/decline_chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/invite_links/delete_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/invite_links/edit_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/invite_links/export_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/invite_links/get_chat_admin_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/invite_links/get_chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/invite_links/get_chat_join_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/invite_links/revoke_chat_invite_link.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.911493 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/copy_media_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/copy_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/delete_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/download_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/edit_inline_caption.py
--rw-r--r--   0 runner    (1001) docker     (123)    10375 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/edit_inline_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/edit_inline_reply_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/edit_inline_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/edit_message_caption.py
--rw-r--r--   0 runner    (1001) docker     (123)    13022 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/edit_message_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/edit_message_reply_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/edit_message_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/forward_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/get_chat_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/get_chat_history_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/get_custom_emoji_stickers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/get_discussion_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/get_discussion_replies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/get_discussion_replies_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/get_media_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/get_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/inline_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/read_chat_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/retract_vote.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/search_global.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/search_global_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/search_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/search_messages_count.py
--rw-r--r--   0 runner    (1001) docker     (123)    13426 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/send_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11912 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/send_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/send_cached_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/send_chat_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/send_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/send_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)    11262 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/send_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/send_location.py
--rw-r--r--   0 runner    (1001) docker     (123)    21371 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/send_media_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     8059 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/send_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    10280 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/send_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8865 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/send_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/send_reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/send_sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/send_venue.py
--rw-r--r--   0 runner    (1001) docker     (123)    12796 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/send_video.py
--rw-r--r--   0 runner    (1001) docker     (123)    10106 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/send_video_note.py
--rw-r--r--   0 runner    (1001) docker     (123)    10222 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/send_voice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/stop_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/stream_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/vote_poll.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.911493 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/password/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/password/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/password/change_cloud_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/password/enable_cloud_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/password/remove_cloud_password.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.911493 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/stickers/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/stickers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/stickers/add_sticker_to_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/stickers/create_sticker_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/stickers/get_sticker_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.915493 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/users/
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/users/block_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/users/delete_profile_photos.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/users/get_chat_photos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/users/get_chat_photos_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/users/get_common_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/users/get_default_emoji_statuses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/users/get_me.py
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/users/get_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/users/set_emoji_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/users/set_profile_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/users/set_username.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/users/unblock_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/users/update_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.915493 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/utilities/add_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/utilities/compose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/utilities/export_session_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/utilities/idle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/utilities/remove_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/utilities/restart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/utilities/run.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1554 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/utilities/run_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/utilities/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/utilities/stop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/utilities/stop_transmission.py
--rw-r--r--   0 runner    (1001) docker     (123)    61915 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/mime_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.915493 PyroFork-dev-2.2.6.dev202307272537/pyrogram/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/parser/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/parser/markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/parser/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.915493 PyroFork-dev-2.2.6.dev202307272537/pyrogram/raw/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/raw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.915493 PyroFork-dev-2.2.6.dev202307272537/pyrogram/raw/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/raw/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/raw/core/future_salt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/raw/core/future_salts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/raw/core/gzip_packed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/raw/core/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/raw/core/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/raw/core/msg_container.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.915493 PyroFork-dev-2.2.6.dev202307272537/pyrogram/raw/core/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/raw/core/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/raw/core/primitives/bool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/raw/core/primitives/bytes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/raw/core/primitives/double.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/raw/core/primitives/int.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/raw/core/primitives/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/raw/core/primitives/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/raw/core/tl_object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.919493 PyroFork-dev-2.2.6.dev202307272537/pyrogram/session/
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10513 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/session/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.919493 PyroFork-dev-2.2.6.dev202307272537/pyrogram/session/internals/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/session/internals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/session/internals/data_center.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/session/internals/msg_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/session/internals/msg_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/session/internals/seq_no.py
--rw-r--r--   0 runner    (1001) docker     (123)    13018 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/session/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.919493 PyroFork-dev-2.2.6.dev202307272537/pyrogram/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/storage/dummy_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/storage/file_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/storage/memory_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     6845 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/storage/mongo_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.919493 PyroFork-dev-2.2.6.dev202307272537/pyrogram/storage/sqlite/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/storage/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/storage/sqlite/cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/storage/sqlite/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/storage/sqlite_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/storage/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.919493 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.919493 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/authorization/
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/authorization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/authorization/sent_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/authorization/terms_of_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.923493 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/bot_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/bot_command_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/bot_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/callback_game.py
--rw-r--r--   0 runner    (1001) docker     (123)    12797 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/callback_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/force_reply.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/game_high_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     8120 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/keyboard_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/login_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/menu_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/menu_button_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/menu_button_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/menu_button_web_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/sent_web_app_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/web_app_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.927493 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/chosen_inline_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/inline_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/inline_query_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/inline_query_result_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/inline_query_result_article.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/inline_query_result_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/inline_query_result_cached_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/inline_query_result_cached_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/inline_query_result_cached_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/inline_query_result_cached_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/inline_query_result_cached_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/inline_query_result_cached_voice.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/inline_query_result_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/inline_query_result_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/inline_query_result_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/inline_query_result_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/inline_query_result_venue.py
--rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/inline_query_result_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/inline_query_result_voice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.927493 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/input_media/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/input_media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/input_media/input_media.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/input_media/input_media_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/input_media/input_media_audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/input_media/input_media_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/input_media/input_media_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/input_media/input_media_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/input_media/input_phone_contact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.927493 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/input_message_content/
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/input_message_content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/input_message_content/input_message_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/input_message_content/input_text_message_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.931493 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/game.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/location.py
--rw-r--r--   0 runner    (1001) docker     (123)   153586 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/message_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/message_reactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/poll_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/sticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/stickerset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/stripped_thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/venue.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/video.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/video_note.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/voice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/web_app_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/web_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.935493 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33966 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    22023 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/chat_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/chat_event_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/chat_invite_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/chat_join_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/chat_joined_by_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/chat_joiner.py
--rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/chat_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/chat_member_updated.py
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/chat_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/chat_photo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/chat_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/chat_privileges.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/chat_reactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/emoji_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/forum_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/forum_topic_closed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/forum_topic_created.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/forum_topic_edited.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/forum_topic_reopened.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/general_forum_topic_hidden.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/invite_link_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/peer_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/peer_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/restriction.py
--rw-r--r--   0 runner    (1001) docker     (123)    13658 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/username.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/video_chat_ended.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/video_chat_members_invited.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/video_chat_scheduled.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/video_chat_started.py
--rw-r--r--   0 runner    (1001) docker     (123)    11166 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/pyrogram/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 08:14:36.935493 PyroFork-dev-2.2.6.dev202307272537/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-07-27 08:14:29.000000 PyroFork-dev-2.2.6.dev202307272537/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.935493 PyroFork-dev-2.2.6.dev202307272537/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.935493 PyroFork-dev-2.2.6.dev202307272537/tests/filters/
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/tests/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/tests/filters/test_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 08:14:36.935493 PyroFork-dev-2.2.6.dev202307272537/tests/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/tests/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/tests/parser/test_html.py
--rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-07-27 08:14:19.000000 PyroFork-dev-2.2.6.dev202307272537/tests/test_file_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.709834 PyroFork-dev-2.2.6.dev202308012705/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/COPYING.lesser
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-08-01 12:00:37.709834 PyroFork-dev-2.2.6.dev202308012705/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.609830 PyroFork-dev-2.2.6.dev202308012705/PyroFork_dev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-08-01 12:00:37.000000 PyroFork-dev-2.2.6.dev202308012705/PyroFork_dev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20482 2023-08-01 12:00:37.000000 PyroFork-dev-2.2.6.dev202308012705/PyroFork_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 12:00:37.000000 PyroFork-dev-2.2.6.dev202308012705/PyroFork_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 12:00:37.000000 PyroFork-dev-2.2.6.dev202308012705/PyroFork_dev.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-01 12:00:37.000000 PyroFork-dev-2.2.6.dev202308012705/PyroFork_dev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-01 12:00:37.000000 PyroFork-dev-2.2.6.dev202308012705/PyroFork_dev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.609830 PyroFork-dev-2.2.6.dev202308012705/compiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.609830 PyroFork-dev-2.2.6.dev202308012705/compiler/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/compiler/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22402 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/compiler/api/compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.609830 PyroFork-dev-2.2.6.dev202308012705/compiler/api/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/compiler/api/source/auth_key.tl
+-rw-r--r--   0 runner    (1001) docker     (123)   175007 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/compiler/api/source/main_api.tl
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/compiler/api/source/sys_msgs.tl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.609830 PyroFork-dev-2.2.6.dev202308012705/compiler/api/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/compiler/api/template/combinator.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/compiler/api/template/type.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.609830 PyroFork-dev-2.2.6.dev202308012705/compiler/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/compiler/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19579 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/compiler/docs/compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.609830 PyroFork-dev-2.2.6.dev202308012705/compiler/docs/template/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/compiler/docs/template/page.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/compiler/docs/template/toctree.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.609830 PyroFork-dev-2.2.6.dev202308012705/compiler/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/compiler/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/compiler/errors/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/compiler/errors/sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.613830 PyroFork-dev-2.2.6.dev202308012705/compiler/errors/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/compiler/errors/source/303_SEE_OTHER.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    22907 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/compiler/errors/source/400_BAD_REQUEST.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/compiler/errors/source/401_UNAUTHORIZED.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/compiler/errors/source/403_FORBIDDEN.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/compiler/errors/source/406_NOT_ACCEPTABLE.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/compiler/errors/source/420_FLOOD.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/compiler/errors/source/503_SERVICE_UNAVAILABLE.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.613830 PyroFork-dev-2.2.6.dev202308012705/compiler/errors/template/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/compiler/errors/template/class.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/compiler/errors/template/sub_class.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.613830 PyroFork-dev-2.2.6.dev202308012705/pyrogram/
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-08-01 12:00:28.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41006 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.613830 PyroFork-dev-2.2.6.dev202308012705/pyrogram/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/connection/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.613830 PyroFork-dev-2.2.6.dev202308012705/pyrogram/connection/transport/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/connection/transport/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.617830 PyroFork-dev-2.2.6.dev202308012705/pyrogram/connection/transport/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/connection/transport/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/connection/transport/tcp/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/connection/transport/tcp/tcp_abridged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/connection/transport/tcp/tcp_abridged_o.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/connection/transport/tcp/tcp_full.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/connection/transport/tcp/tcp_intermediate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/connection/transport/tcp/tcp_intermediate_o.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.617830 PyroFork-dev-2.2.6.dev202308012705/pyrogram/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/crypto/aes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4762 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/crypto/mtproto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/crypto/prime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/crypto/rsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)   208021 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/emoji.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.617830 PyroFork-dev-2.2.6.dev202308012705/pyrogram/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/enums/auto_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/enums/chat_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/enums/chat_event_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/enums/chat_member_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/enums/chat_members_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/enums/chat_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/enums/message_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/enums/message_media_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/enums/message_service_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/enums/messages_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/enums/next_code_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/enums/parse_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/enums/poll_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/enums/sent_code_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/enums/user_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.617830 PyroFork-dev-2.2.6.dev202308012705/pyrogram/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/errors/rpc_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/file_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24836 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.621830 PyroFork-dev-2.2.6.dev202308012705/pyrogram/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/handlers/callback_query_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/handlers/chat_join_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/handlers/chat_member_updated_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/handlers/chosen_inline_result_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/handlers/deleted_messages_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/handlers/disconnect_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/handlers/edited_message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/handlers/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/handlers/inline_query_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/handlers/message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/handlers/poll_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/handlers/raw_update_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/handlers/user_status_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.621830 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.621830 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/advanced/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/advanced/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/advanced/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/advanced/resolve_peer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/advanced/save_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.625830 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/auth/accept_terms_of_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/auth/check_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/auth/connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/auth/disconnect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/auth/get_password_hint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/auth/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/auth/log_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/auth/recover_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/auth/resend_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/auth/send_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/auth/send_recovery_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/auth/sign_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/auth/sign_in_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/auth/sign_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/auth/terminate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.629830 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/bots/
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/bots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/bots/answer_callback_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/bots/answer_inline_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/bots/answer_web_app_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/bots/delete_bot_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/bots/get_bot_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/bots/get_bot_default_privileges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/bots/get_bot_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/bots/get_chat_menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/bots/get_game_high_scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/bots/get_inline_bot_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/bots/request_callback_answer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/bots/send_game.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/bots/send_inline_bot_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/bots/set_bot_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/bots/set_bot_default_privileges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/bots/set_bot_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/bots/set_chat_menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/bots/set_game_score.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.637831 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/add_chat_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/archive_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/ban_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/close_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/close_general_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/create_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/create_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/create_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/create_supergroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/delete_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/delete_chat_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/delete_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/delete_supergroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/delete_user_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/edit_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/edit_general_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/get_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/get_chat_event_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/get_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/get_chat_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/get_chat_members_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/get_chat_online_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/get_dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/get_dialogs_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/get_forum_topics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/get_forum_topics_by_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/get_nearby_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/get_send_as_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/hide_general_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/join_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/leave_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/mark_chat_unread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/pin_chat_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/promote_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/reopen_forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/reopen_general_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/restrict_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/set_administrator_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/set_chat_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/set_chat_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/set_chat_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/set_chat_protected_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/set_chat_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/set_chat_username.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/set_send_as_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/set_slow_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/unarchive_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/unban_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/unhide_general_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/unpin_all_chat_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/unpin_chat_message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.637831 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/contacts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/contacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/contacts/add_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/contacts/delete_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/contacts/get_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/contacts/get_contacts_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/contacts/import_contacts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.637831 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/decorators/on_callback_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/decorators/on_chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/decorators/on_chat_member_updated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/decorators/on_chosen_inline_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/decorators/on_deleted_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/decorators/on_disconnect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/decorators/on_edited_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/decorators/on_inline_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/decorators/on_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/decorators/on_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/decorators/on_raw_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/decorators/on_user_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.641831 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/invite_links/
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/invite_links/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/invite_links/approve_all_chat_join_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/invite_links/approve_chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/invite_links/create_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/invite_links/decline_all_chat_join_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/invite_links/decline_chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/invite_links/delete_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/invite_links/edit_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/invite_links/export_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/invite_links/get_chat_admin_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/invite_links/get_chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/invite_links/get_chat_join_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/invite_links/revoke_chat_invite_link.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.653832 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/copy_media_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/copy_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/delete_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/download_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/edit_inline_caption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10375 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/edit_inline_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/edit_inline_reply_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/edit_inline_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/edit_message_caption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13022 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/edit_message_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/edit_message_reply_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/edit_message_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/forward_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/get_chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/get_chat_history_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/get_custom_emoji_stickers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/get_discussion_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/get_discussion_replies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/get_discussion_replies_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/get_media_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/get_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/inline_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/read_chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/retract_vote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/search_global.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/search_global_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/search_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/search_messages_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13426 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/send_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11912 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/send_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/send_cached_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/send_chat_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/send_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/send_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11262 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/send_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5371 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/send_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21371 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/send_media_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8059 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/send_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10280 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/send_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8865 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/send_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/send_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/send_sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/send_venue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12796 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/send_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10106 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/send_video_note.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10222 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/send_voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/stop_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/stream_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/vote_poll.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.653832 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/password/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/password/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/password/change_cloud_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/password/enable_cloud_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/password/remove_cloud_password.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.657832 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/stickers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/stickers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/stickers/add_sticker_to_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/stickers/create_sticker_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/stickers/get_sticker_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.657832 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/users/
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/users/block_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/users/delete_profile_photos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/users/get_chat_photos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/users/get_chat_photos_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/users/get_common_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/users/get_default_emoji_statuses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/users/get_me.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/users/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/users/set_emoji_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/users/set_profile_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/users/set_username.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/users/unblock_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/users/update_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.661832 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/utilities/add_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/utilities/compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/utilities/export_session_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/utilities/idle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/utilities/remove_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/utilities/restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/utilities/run.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1554 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/utilities/run_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/utilities/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/utilities/stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/utilities/stop_transmission.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61915 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/mime_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.661832 PyroFork-dev-2.2.6.dev202308012705/pyrogram/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/parser/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/parser/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/parser/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.661832 PyroFork-dev-2.2.6.dev202308012705/pyrogram/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/raw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.661832 PyroFork-dev-2.2.6.dev202308012705/pyrogram/raw/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/raw/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/raw/core/future_salt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/raw/core/future_salts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/raw/core/gzip_packed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/raw/core/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/raw/core/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/raw/core/msg_container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.661832 PyroFork-dev-2.2.6.dev202308012705/pyrogram/raw/core/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/raw/core/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/raw/core/primitives/bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/raw/core/primitives/bytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/raw/core/primitives/double.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/raw/core/primitives/int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/raw/core/primitives/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/raw/core/primitives/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/raw/core/tl_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.665832 PyroFork-dev-2.2.6.dev202308012705/pyrogram/session/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10513 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/session/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.665832 PyroFork-dev-2.2.6.dev202308012705/pyrogram/session/internals/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/session/internals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/session/internals/data_center.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/session/internals/msg_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/session/internals/msg_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/session/internals/seq_no.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13018 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/session/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.665832 PyroFork-dev-2.2.6.dev202308012705/pyrogram/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/storage/dummy_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/storage/file_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/storage/memory_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6845 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/storage/mongo_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.665832 PyroFork-dev-2.2.6.dev202308012705/pyrogram/storage/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/storage/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/storage/sqlite/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/storage/sqlite/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/storage/sqlite_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/storage/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.669832 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.669832 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/authorization/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/authorization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/authorization/sent_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/authorization/terms_of_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.673833 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/bot_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/bot_command_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/bot_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/callback_game.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12797 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/callback_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/force_reply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/game_high_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8120 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/keyboard_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/login_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/menu_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/menu_button_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/menu_button_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/menu_button_web_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/sent_web_app_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/web_app_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.685833 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/chosen_inline_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/inline_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/inline_query_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/inline_query_result_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/inline_query_result_article.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/inline_query_result_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/inline_query_result_cached_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/inline_query_result_cached_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/inline_query_result_cached_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/inline_query_result_cached_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/inline_query_result_cached_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/inline_query_result_cached_voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/inline_query_result_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/inline_query_result_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/inline_query_result_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/inline_query_result_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/inline_query_result_venue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/inline_query_result_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/inline_query_result_voice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.685833 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/input_media/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/input_media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/input_media/input_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/input_media/input_media_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/input_media/input_media_audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/input_media/input_media_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/input_media/input_media_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/input_media/input_media_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/input_media/input_phone_contact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.685833 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/input_message_content/
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/input_message_content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/input_message_content/input_message_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/input_message_content/input_text_message_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.693833 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/game.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)   153586 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/message_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/message_reactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/poll_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/sticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/stickerset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/stripped_thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/venue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/video_note.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/web_app_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/web_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.709834 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34261 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22023 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/chat_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/chat_event_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/chat_invite_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/chat_join_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/chat_joined_by_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/chat_joiner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/chat_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/chat_member_updated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/chat_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/chat_photo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/chat_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/chat_privileges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/chat_reactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/emoji_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/forum_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/forum_topic_closed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/forum_topic_created.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/forum_topic_edited.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/forum_topic_reopened.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/general_forum_topic_hidden.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/invite_link_importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/peer_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/peer_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/restriction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13658 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/username.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/video_chat_ended.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/video_chat_members_invited.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/video_chat_scheduled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/video_chat_started.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11166 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/pyrogram/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 12:00:37.709834 PyroFork-dev-2.2.6.dev202308012705/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-08-01 12:00:28.000000 PyroFork-dev-2.2.6.dev202308012705/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.709834 PyroFork-dev-2.2.6.dev202308012705/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.709834 PyroFork-dev-2.2.6.dev202308012705/tests/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/tests/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/tests/filters/test_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:00:37.709834 PyroFork-dev-2.2.6.dev202308012705/tests/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/tests/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/tests/parser/test_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-08-01 12:00:16.000000 PyroFork-dev-2.2.6.dev202308012705/tests/test_file_id.py
```

### Comparing `PyroFork-dev-2.2.6.dev202307272537/COPYING` & `PyroFork-dev-2.2.6.dev202308012705/COPYING`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/COPYING.lesser` & `PyroFork-dev-2.2.6.dev202308012705/COPYING.lesser`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/NOTICE` & `PyroFork-dev-2.2.6.dev202308012705/NOTICE`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/PKG-INFO` & `PyroFork-dev-2.2.6.dev202308012705/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyroFork-dev
-Version: 2.2.6.dev202307272537
+Version: 2.2.6.dev202308012705
 Summary: Elegant, modern and asynchronous Telegram MTProto API framework in Python for users and bots
 Home-page: https://github.com/Mayuri-Chan/pyrofork
 Download-URL: https://github.com/Mayuri-Chan/pyrofork/releases/latest
 Author: wulan17
 Author-email: mayuri@mayuri.my.id
 License: LGPLv3
 Project-URL: Tracker, https://github.com/Mayuri-Chan/pyrofork/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyroFork-dev Version: 2.2.6.dev202307272537
+Metadata-Version: 2.1 Name: PyroFork-dev Version: 2.2.6.dev202308012705
 Summary: Elegant, modern and asynchronous Telegram MTProto API framework in
 Python for users and bots Home-page: https://github.com/Mayuri-Chan/pyrofork
 Download-URL: https://github.com/Mayuri-Chan/pyrofork/releases/latest Author:
 wulan17 Author-email: mayuri@mayuri.my.id License: LGPLv3 Project-URL: Tracker,
 https://github.com/Mayuri-Chan/pyrofork/issues Project-URL: Source, https://
 github.com/Mayuri-Chan/pyrofork Project-URL: Documentation, https://
 pyrofork.mayuri.my.id Keywords: telegram chat messenger mtproto api client
```

### Comparing `PyroFork-dev-2.2.6.dev202307272537/PyroFork_dev.egg-info/PKG-INFO` & `PyroFork-dev-2.2.6.dev202308012705/PyroFork_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyroFork-dev
-Version: 2.2.6.dev202307272537
+Version: 2.2.6.dev202308012705
 Summary: Elegant, modern and asynchronous Telegram MTProto API framework in Python for users and bots
 Home-page: https://github.com/Mayuri-Chan/pyrofork
 Download-URL: https://github.com/Mayuri-Chan/pyrofork/releases/latest
 Author: wulan17
 Author-email: mayuri@mayuri.my.id
 License: LGPLv3
 Project-URL: Tracker, https://github.com/Mayuri-Chan/pyrofork/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyroFork-dev Version: 2.2.6.dev202307272537
+Metadata-Version: 2.1 Name: PyroFork-dev Version: 2.2.6.dev202308012705
 Summary: Elegant, modern and asynchronous Telegram MTProto API framework in
 Python for users and bots Home-page: https://github.com/Mayuri-Chan/pyrofork
 Download-URL: https://github.com/Mayuri-Chan/pyrofork/releases/latest Author:
 wulan17 Author-email: mayuri@mayuri.my.id License: LGPLv3 Project-URL: Tracker,
 https://github.com/Mayuri-Chan/pyrofork/issues Project-URL: Source, https://
 github.com/Mayuri-Chan/pyrofork Project-URL: Documentation, https://
 pyrofork.mayuri.my.id Keywords: telegram chat messenger mtproto api client
```

### Comparing `PyroFork-dev-2.2.6.dev202307272537/PyroFork_dev.egg-info/SOURCES.txt` & `PyroFork-dev-2.2.6.dev202308012705/PyroFork_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/README.md` & `PyroFork-dev-2.2.6.dev202308012705/README.md`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/compiler/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/compiler/api/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/compiler/api/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/compiler/api/compiler.py` & `PyroFork-dev-2.2.6.dev202308012705/compiler/api/compiler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/compiler/api/source/auth_key.tl` & `PyroFork-dev-2.2.6.dev202308012705/compiler/api/source/auth_key.tl`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/compiler/api/source/main_api.tl` & `PyroFork-dev-2.2.6.dev202308012705/compiler/api/source/main_api.tl`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/compiler/api/source/sys_msgs.tl` & `PyroFork-dev-2.2.6.dev202308012705/compiler/api/source/sys_msgs.tl`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/compiler/api/template/combinator.txt` & `PyroFork-dev-2.2.6.dev202308012705/compiler/api/template/combinator.txt`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/compiler/api/template/type.txt` & `PyroFork-dev-2.2.6.dev202308012705/compiler/api/template/type.txt`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/compiler/docs/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/compiler/docs/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/compiler/docs/compiler.py` & `PyroFork-dev-2.2.6.dev202308012705/compiler/docs/compiler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/compiler/errors/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/compiler/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/compiler/errors/compiler.py` & `PyroFork-dev-2.2.6.dev202308012705/compiler/errors/compiler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/compiler/errors/sort.py` & `PyroFork-dev-2.2.6.dev202308012705/compiler/errors/sort.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/compiler/errors/source/400_BAD_REQUEST.tsv` & `PyroFork-dev-2.2.6.dev202308012705/compiler/errors/source/400_BAD_REQUEST.tsv`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/compiler/errors/source/401_UNAUTHORIZED.tsv` & `PyroFork-dev-2.2.6.dev202308012705/compiler/errors/source/401_UNAUTHORIZED.tsv`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/compiler/errors/source/403_FORBIDDEN.tsv` & `PyroFork-dev-2.2.6.dev202308012705/compiler/errors/source/403_FORBIDDEN.tsv`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/compiler/errors/source/406_NOT_ACCEPTABLE.tsv` & `PyroFork-dev-2.2.6.dev202308012705/compiler/errors/source/406_NOT_ACCEPTABLE.tsv`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv` & `PyroFork-dev-2.2.6.dev202308012705/compiler/errors/source/500_INTERNAL_SERVER_ERROR.tsv`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU Lesser General Public License for more details.
 #
 #  You should have received a copy of the GNU Lesser General Public License
 #  along with Pyrogram.  If not, see <http://www.gnu.org/licenses/>.
 
 __fork_name__ = "PyroFork-dev"
-__version__ = "2.2.6.dev202307272537"
+__version__ = "2.2.6.dev202308012705"
 __license__ = "GNU Lesser General Public License v3.0 (LGPL-3.0)"
 __copyright__ = "Copyright (C) 2022-present Mayuri-Chan <https://github.com/Mayuri-Chan>"
 
 from concurrent.futures.thread import ThreadPoolExecutor
 
 
 class StopTransmission(Exception):
```

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/client.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/client.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/connection/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/connection/connection.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/connection/connection.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/connection/transport/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/connection/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/connection/transport/tcp/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/connection/transport/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/connection/transport/tcp/tcp.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/connection/transport/tcp/tcp.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/connection/transport/tcp/tcp_abridged.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/connection/transport/tcp/tcp_abridged.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/connection/transport/tcp/tcp_abridged_o.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/connection/transport/tcp/tcp_abridged_o.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/connection/transport/tcp/tcp_full.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/connection/transport/tcp/tcp_full.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/connection/transport/tcp/tcp_intermediate.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/connection/transport/tcp/tcp_intermediate.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/connection/transport/tcp/tcp_intermediate_o.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/connection/transport/tcp/tcp_intermediate_o.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/crypto/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/crypto/aes.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/crypto/mtproto.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/crypto/mtproto.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/crypto/prime.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/crypto/prime.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/crypto/rsa.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/crypto/rsa.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/dispatcher.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/dispatcher.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/emoji.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/emoji.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/enums/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/enums/auto_name.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/enums/auto_name.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/enums/chat_action.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/enums/chat_action.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/enums/chat_event_action.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/enums/chat_event_action.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/enums/chat_member_status.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/enums/chat_member_status.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/enums/chat_members_filter.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/enums/chat_members_filter.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/enums/chat_type.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/enums/chat_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/enums/message_entity_type.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/enums/message_entity_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/enums/message_media_type.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/enums/message_media_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/enums/message_service_type.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/enums/message_service_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/enums/messages_filter.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/enums/messages_filter.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/enums/next_code_type.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/enums/next_code_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/enums/parse_mode.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/enums/parse_mode.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/enums/poll_type.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/enums/poll_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/enums/sent_code_type.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/enums/sent_code_type.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/enums/user_status.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/enums/user_status.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/errors/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/errors/rpc_error.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/errors/rpc_error.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/file_id.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/file_id.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/filters.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/filters.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/handlers/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/handlers/callback_query_handler.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/handlers/callback_query_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/handlers/chat_join_request_handler.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/handlers/chat_join_request_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/handlers/chat_member_updated_handler.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/handlers/chat_member_updated_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/handlers/chosen_inline_result_handler.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/handlers/chosen_inline_result_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/handlers/deleted_messages_handler.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/handlers/deleted_messages_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/handlers/disconnect_handler.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/handlers/disconnect_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/handlers/edited_message_handler.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/handlers/edited_message_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/handlers/handler.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/handlers/inline_query_handler.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/handlers/inline_query_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/handlers/message_handler.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/handlers/message_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/handlers/poll_handler.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/handlers/poll_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/handlers/raw_update_handler.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/handlers/raw_update_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/handlers/user_status_handler.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/handlers/user_status_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/advanced/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/advanced/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/advanced/invoke.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/advanced/invoke.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/advanced/resolve_peer.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/advanced/resolve_peer.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/advanced/save_file.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/advanced/save_file.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/auth/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/auth/accept_terms_of_service.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/auth/accept_terms_of_service.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/auth/check_password.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/auth/check_password.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/auth/connect.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/auth/connect.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/auth/disconnect.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/auth/disconnect.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/auth/get_password_hint.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/auth/get_password_hint.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/auth/initialize.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/auth/initialize.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/auth/log_out.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/auth/log_out.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/auth/recover_password.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/auth/recover_password.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/auth/resend_code.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/auth/resend_code.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/auth/send_code.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/auth/send_code.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/auth/send_recovery_code.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/auth/send_recovery_code.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/auth/sign_in.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/auth/sign_in.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/auth/sign_in_bot.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/auth/sign_in_bot.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/auth/sign_up.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/auth/sign_up.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/auth/terminate.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/auth/terminate.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/bots/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/bots/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/bots/answer_callback_query.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/bots/answer_callback_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/bots/answer_inline_query.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/bots/answer_inline_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/bots/answer_web_app_query.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/bots/answer_web_app_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/bots/delete_bot_commands.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/bots/delete_bot_commands.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/bots/get_bot_commands.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/bots/get_bot_commands.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/bots/get_bot_default_privileges.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/bots/get_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/bots/get_bot_info.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/bots/get_bot_info.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/bots/get_chat_menu_button.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/bots/get_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/bots/get_game_high_scores.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/bots/get_game_high_scores.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/bots/get_inline_bot_results.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/bots/get_inline_bot_results.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/bots/request_callback_answer.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/bots/request_callback_answer.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/bots/send_game.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/bots/send_game.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/bots/send_inline_bot_result.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/bots/send_inline_bot_result.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/bots/set_bot_commands.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/bots/set_bot_commands.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/bots/set_bot_default_privileges.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/bots/set_bot_default_privileges.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/bots/set_bot_info.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/bots/set_bot_info.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/bots/set_chat_menu_button.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/bots/set_chat_menu_button.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/bots/set_game_score.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/bots/set_game_score.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/add_chat_members.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/add_chat_members.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/archive_chats.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/archive_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/ban_chat_member.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/ban_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/close_forum_topic.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/close_forum_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/close_general_topic.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/close_general_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/create_channel.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/create_channel.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/create_forum_topic.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/create_forum_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/create_group.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/create_group.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/create_supergroup.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/create_supergroup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/delete_channel.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/delete_channel.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/delete_chat_photo.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/delete_chat_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/delete_forum_topic.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/delete_forum_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/delete_supergroup.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/delete_supergroup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/delete_user_history.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/delete_user_history.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/edit_forum_topic.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/edit_forum_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/edit_general_topic.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/edit_general_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/get_chat.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/get_chat.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/get_chat_event_log.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/get_chat_event_log.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/get_chat_member.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/get_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/get_chat_members.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/get_chat_members.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/get_chat_members_count.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/get_chat_members_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/get_chat_online_count.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/get_chat_online_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/get_dialogs.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/get_dialogs.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/get_dialogs_count.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/get_dialogs_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/get_forum_topics.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/get_forum_topics.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/get_forum_topics_by_id.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/get_forum_topics_by_id.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/get_nearby_chats.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/get_nearby_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/get_send_as_chats.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/get_send_as_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/hide_general_topic.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/hide_general_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/join_chat.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/join_chat.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/leave_chat.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/leave_chat.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/mark_chat_unread.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/mark_chat_unread.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/pin_chat_message.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/pin_chat_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/promote_chat_member.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/promote_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/reopen_forum_topic.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/reopen_forum_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/reopen_general_topic.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/reopen_general_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/restrict_chat_member.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/restrict_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/set_administrator_title.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/set_administrator_title.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/set_chat_description.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/set_chat_description.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/set_chat_permissions.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/set_chat_permissions.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/set_chat_photo.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/set_chat_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/set_chat_protected_content.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/set_chat_protected_content.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/set_chat_title.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/set_chat_title.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/set_chat_username.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/set_chat_username.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/set_send_as_chat.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/set_send_as_chat.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/set_slow_mode.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/set_slow_mode.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/unarchive_chats.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/unarchive_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/unban_chat_member.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/unban_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/unhide_general_topic.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/unhide_general_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/unpin_all_chat_messages.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/unpin_all_chat_messages.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/chats/unpin_chat_message.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/chats/unpin_chat_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/contacts/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/contacts/add_contact.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/contacts/add_contact.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/contacts/delete_contacts.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/contacts/delete_contacts.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/contacts/get_contacts.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/contacts/get_contacts.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/contacts/get_contacts_count.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/contacts/get_contacts_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/contacts/import_contacts.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/contacts/import_contacts.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/decorators/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/decorators/on_callback_query.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/decorators/on_callback_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/decorators/on_chat_join_request.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/decorators/on_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/decorators/on_chat_member_updated.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/decorators/on_chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/decorators/on_chosen_inline_result.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/decorators/on_chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/decorators/on_deleted_messages.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/decorators/on_deleted_messages.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/decorators/on_disconnect.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/decorators/on_disconnect.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/decorators/on_edited_message.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/decorators/on_edited_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/decorators/on_inline_query.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/decorators/on_inline_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/decorators/on_message.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/decorators/on_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/decorators/on_poll.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/decorators/on_poll.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/decorators/on_raw_update.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/decorators/on_raw_update.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/decorators/on_user_status.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/decorators/on_user_status.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/invite_links/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/invite_links/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/invite_links/approve_all_chat_join_requests.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/invite_links/approve_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/invite_links/approve_chat_join_request.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/invite_links/approve_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/invite_links/create_chat_invite_link.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/invite_links/create_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/invite_links/decline_all_chat_join_requests.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/invite_links/decline_all_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/invite_links/decline_chat_join_request.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/invite_links/decline_chat_join_request.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/invite_links/delete_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/invite_links/delete_chat_invite_link.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/invite_links/delete_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/invite_links/edit_chat_invite_link.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/invite_links/edit_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/invite_links/export_chat_invite_link.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/invite_links/export_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/invite_links/get_chat_admin_invite_links.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/invite_links/get_chat_admin_invite_links.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/invite_links/get_chat_admin_invite_links_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/invite_links/get_chat_admins_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/invite_links/get_chat_invite_link.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/invite_links/get_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/invite_links/get_chat_invite_link_joiners.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/invite_links/get_chat_invite_link_joiners_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/invite_links/get_chat_join_requests.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/invite_links/get_chat_join_requests.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/invite_links/revoke_chat_invite_link.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/invite_links/revoke_chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/copy_media_group.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/copy_media_group.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/copy_message.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/copy_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/delete_messages.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/delete_messages.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/download_media.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/download_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/edit_inline_caption.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/edit_inline_caption.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/edit_inline_media.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/edit_inline_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/edit_inline_reply_markup.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/edit_inline_reply_markup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/edit_inline_text.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/edit_inline_text.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/edit_message_caption.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/edit_message_caption.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/edit_message_media.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/edit_message_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/edit_message_reply_markup.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/edit_message_reply_markup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/edit_message_text.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/edit_message_text.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/forward_messages.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/forward_messages.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/get_chat_history.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/get_chat_history.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/get_chat_history_count.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/get_chat_history_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/get_custom_emoji_stickers.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/get_custom_emoji_stickers.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/get_discussion_message.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/get_discussion_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/get_discussion_replies.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/get_discussion_replies.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/get_discussion_replies_count.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/get_discussion_replies_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/get_media_group.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/get_media_group.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/get_messages.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/get_messages.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/inline_session.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/inline_session.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/read_chat_history.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/read_chat_history.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/retract_vote.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/retract_vote.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/search_global.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/search_global.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/search_global_count.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/search_global_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/search_messages.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/search_messages.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/search_messages_count.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/search_messages_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/send_animation.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/send_animation.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/send_audio.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/send_audio.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/send_cached_media.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/send_cached_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/send_chat_action.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/send_chat_action.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/send_contact.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/send_contact.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/send_dice.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/send_dice.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/send_document.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/send_document.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/send_location.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/send_location.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/send_media_group.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/send_media_group.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/send_message.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/send_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/send_photo.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/send_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/send_poll.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/send_poll.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/send_reaction.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/send_reaction.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/send_sticker.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/send_sticker.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/send_venue.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/send_venue.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/send_video.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/send_video.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/send_video_note.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/send_video_note.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/send_voice.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/send_voice.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/stop_poll.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/stop_poll.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/stream_media.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/stream_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/messages/vote_poll.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/messages/vote_poll.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/password/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/password/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/password/change_cloud_password.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/password/change_cloud_password.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/password/enable_cloud_password.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/password/enable_cloud_password.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/password/remove_cloud_password.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/password/remove_cloud_password.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/stickers/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/stickers/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/stickers/add_sticker_to_set.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/stickers/add_sticker_to_set.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/stickers/create_sticker_set.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/stickers/create_sticker_set.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/stickers/get_sticker_set.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/stickers/get_sticker_set.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/users/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/users/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/users/block_user.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/users/block_user.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/users/delete_profile_photos.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/users/delete_profile_photos.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/users/get_chat_photos.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/users/get_chat_photos.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/users/get_chat_photos_count.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/users/get_chat_photos_count.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/users/get_common_chats.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/users/get_common_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/users/get_default_emoji_statuses.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/users/get_default_emoji_statuses.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/users/get_me.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/users/get_me.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/users/get_users.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/users/get_users.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/users/set_emoji_status.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/users/set_emoji_status.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/users/set_profile_photo.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/users/set_profile_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/users/set_username.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/users/set_username.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/users/unblock_user.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/users/unblock_user.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/users/update_profile.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/users/update_profile.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/utilities/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/utilities/add_handler.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/utilities/add_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/utilities/compose.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/utilities/compose.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/utilities/export_session_string.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/utilities/export_session_string.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/utilities/idle.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/utilities/idle.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/utilities/remove_handler.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/utilities/remove_handler.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/utilities/restart.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/utilities/restart.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/utilities/run.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/utilities/run.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/utilities/run_sync.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/utilities/run_sync.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/utilities/start.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/utilities/start.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/utilities/stop.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/utilities/stop.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/methods/utilities/stop_transmission.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/methods/utilities/stop_transmission.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/mime_types.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/mime_types.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/parser/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/parser/html.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/parser/html.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/parser/markdown.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/parser/markdown.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/parser/parser.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/parser/parser.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/parser/utils.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/parser/utils.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/raw/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/raw/core/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/raw/core/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/raw/core/future_salt.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/raw/core/future_salt.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/raw/core/future_salts.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/raw/core/future_salts.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/raw/core/gzip_packed.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/raw/core/gzip_packed.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/raw/core/list.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/raw/core/list.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/raw/core/message.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/raw/core/message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/raw/core/msg_container.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/raw/core/msg_container.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/raw/core/primitives/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/raw/core/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/raw/core/primitives/bool.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/raw/core/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/raw/core/primitives/bytes.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/raw/core/primitives/bytes.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/raw/core/primitives/double.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/raw/core/primitives/double.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/raw/core/primitives/int.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/raw/core/primitives/int.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/raw/core/primitives/string.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/raw/core/primitives/string.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/raw/core/primitives/vector.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/raw/core/primitives/vector.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/raw/core/tl_object.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/raw/core/tl_object.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/session/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/session/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/session/auth.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/session/auth.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/session/internals/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/session/internals/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/session/internals/data_center.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/session/internals/data_center.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/session/internals/msg_factory.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/session/internals/msg_factory.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/session/internals/msg_id.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/session/internals/msg_id.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/session/internals/seq_no.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/session/internals/seq_no.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/session/session.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/session/session.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/storage/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/storage/dummy_client.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/storage/dummy_client.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/storage/file_storage.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/storage/memory_storage.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/storage/memory_storage.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/storage/mongo_storage.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/storage/mongo_storage.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/storage/sqlite/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/storage/sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/storage/sqlite/cursor.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/storage/sqlite/cursor.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/storage/sqlite/sqlite.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/storage/sqlite/sqlite.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/storage/sqlite_storage.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/storage/storage.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/storage/storage.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/sync.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/sync.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/authorization/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/authorization/sent_code.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/authorization/sent_code.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/authorization/terms_of_service.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/authorization/terms_of_service.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/bot_command.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/bot_command.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/bot_command_scope.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/bot_command_scope.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/bot_command_scope_all_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/bot_command_scope_all_group_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/bot_command_scope_all_private_chats.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/bot_command_scope_chat.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_administrators.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/bot_command_scope_chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/bot_command_scope_default.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/bot_info.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/bot_info.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/callback_game.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/callback_game.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/callback_query.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/callback_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/force_reply.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/force_reply.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/game_high_score.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/game_high_score.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/inline_keyboard_button.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/inline_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/keyboard_button.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/keyboard_button.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/login_url.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/login_url.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/menu_button.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/menu_button.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/menu_button_commands.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/menu_button_commands.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/menu_button_default.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/menu_button_default.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/menu_button_web_app.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/menu_button_web_app.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/reply_keyboard_markup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/reply_keyboard_remove.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/sent_web_app_message.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/sent_web_app_message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/bots_and_keyboards/web_app_info.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/bots_and_keyboards/web_app_info.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/chosen_inline_result.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/chosen_inline_result.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/inline_query.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/inline_query.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/inline_query_result.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/inline_query_result.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/inline_query_result_animation.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/inline_query_result_animation.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/inline_query_result_article.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/inline_query_result_article.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/inline_query_result_audio.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/inline_query_result_audio.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/inline_query_result_cached_animation.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/inline_query_result_cached_animation.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/inline_query_result_cached_audio.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/inline_query_result_cached_audio.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/inline_query_result_cached_document.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/inline_query_result_cached_document.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/inline_query_result_cached_photo.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/inline_query_result_cached_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/inline_query_result_cached_sticker.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/inline_query_result_cached_video.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/inline_query_result_cached_video.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/inline_query_result_cached_voice.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/inline_query_result_cached_voice.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/inline_query_result_contact.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/inline_query_result_contact.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/inline_query_result_document.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/inline_query_result_document.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/inline_query_result_location.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/inline_query_result_location.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/inline_query_result_photo.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/inline_query_result_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/inline_query_result_venue.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/inline_query_result_venue.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/inline_query_result_video.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/inline_query_result_video.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/inline_mode/inline_query_result_voice.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/inline_mode/inline_query_result_voice.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/input_media/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/input_media/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/input_media/input_media.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/input_media/input_media.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/input_media/input_media_animation.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/input_media/input_media_animation.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/input_media/input_media_audio.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/input_media/input_media_audio.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/input_media/input_media_document.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/input_media/input_media_document.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/input_media/input_media_photo.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/input_media/input_media_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/input_media/input_media_video.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/input_media/input_media_video.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/input_media/input_phone_contact.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/input_media/input_phone_contact.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/input_message_content/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/input_message_content/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/input_message_content/input_message_content.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/input_message_content/input_message_content.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/input_message_content/input_text_message_content.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/input_message_content/input_text_message_content.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/list.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/list.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/animation.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/animation.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/audio.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/audio.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/contact.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/contact.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/dice.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/dice.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/document.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/document.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/game.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/game.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/location.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/location.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/message.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/message.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/message_entity.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/message_entity.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/message_reactions.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/message_reactions.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/photo.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/poll.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/poll.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/poll_option.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/poll_option.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/reaction.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/reaction.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/sticker.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/sticker.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/stickerset.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/stickerset.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/stripped_thumbnail.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/stripped_thumbnail.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/thumbnail.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/thumbnail.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/venue.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/venue.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/video.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/video.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/video_note.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/video_note.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/voice.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/voice.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/web_app_data.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/web_app_data.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/messages_and_media/web_page.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/messages_and_media/web_page.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/object.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/object.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/update.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/update.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/chat.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,17 @@
 
         is_support (``bool``):
             True, if this chat is part of the Telegram support team. Users and bots only.
 
         is_forum (``bool``, *optional*):
             True, if the supergroup chat is a forum
 
+        is_participants_hidden (``bool``, *optional*):
+            True, if the chat members are hidden.
+
         title (``str``, *optional*):
             Title, for supergroups, channels and basic group chats.
 
         username (``str``, *optional*):
             Username, for private chats, bots, supergroups and channels if available.
 
         first_name (``str``, *optional*):
@@ -150,14 +153,15 @@
         is_verified: bool = None,
         is_restricted: bool = None,
         is_creator: bool = None,
         is_scam: bool = None,
         is_fake: bool = None,
         is_support: bool = None,
         is_forum: bool = None,
+        is_participants_hidden: bool = None,
         title: str = None,
         username: str = None,
         first_name: str = None,
         last_name: str = None,
         photo: "types.ChatPhoto" = None,
         bio: str = None,
         description: str = None,
@@ -183,14 +187,15 @@
         self.is_verified = is_verified
         self.is_restricted = is_restricted
         self.is_creator = is_creator
         self.is_scam = is_scam
         self.is_fake = is_fake
         self.is_support = is_support
         self.is_forum = is_forum
+        self.is_participants_hidden = is_participants_hidden
         self.title = title
         self.username = username
         self.first_name = first_name
         self.last_name = last_name
         self.photo = photo
         self.bio = bio
         self.description = description
@@ -349,14 +354,15 @@
             else:
                 parsed_chat = Chat._parse_channel_chat(client, chat_raw)
                 parsed_chat.members_count = full_chat.participants_count
                 parsed_chat.description = full_chat.about or None
                 # TODO: Add StickerSet type
                 parsed_chat.can_set_sticker_set = full_chat.can_set_stickers
                 parsed_chat.sticker_set_name = getattr(full_chat.stickerset, "short_name", None)
+                parsed_chat.is_participants_hidden = full_chat.participants_hidden
 
                 linked_chat_raw = chats.get(full_chat.linked_chat_id, None)
 
                 if linked_chat_raw:
                     parsed_chat.linked_chat = Chat._parse_channel_chat(client, linked_chat_raw)
 
                 default_send_as = full_chat.default_send_as
```

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/chat_admin_with_invite_links.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/chat_event.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/chat_event.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/chat_event_filter.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/chat_event_filter.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/chat_invite_link.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/chat_invite_link.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/chat_join_request.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/chat_join_request.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/chat_joined_by_request.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/chat_joined_by_request.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/chat_joiner.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/chat_joiner.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/chat_member.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/chat_member.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/chat_member_updated.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/chat_member_updated.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/chat_permissions.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/chat_permissions.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/chat_photo.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/chat_photo.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/chat_preview.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/chat_preview.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/chat_privileges.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/chat_privileges.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/chat_reactions.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/chat_reactions.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/dialog.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/dialog.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/emoji_status.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/emoji_status.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/forum_topic.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/forum_topic.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/forum_topic_closed.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/forum_topic_closed.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/forum_topic_created.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/forum_topic_created.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/forum_topic_edited.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/forum_topic_edited.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/forum_topic_reopened.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/forum_topic_reopened.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/general_forum_topic_hidden.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/general_forum_topic_hidden.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/general_forum_topic_unhidden.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/invite_link_importer.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/invite_link_importer.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/peer_channel.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/peer_channel.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/peer_user.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/peer_user.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/restriction.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/restriction.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/user.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/user.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/username.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/username.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/video_chat_ended.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/video_chat_ended.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/video_chat_members_invited.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/video_chat_members_invited.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/video_chat_scheduled.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/video_chat_scheduled.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/types/user_and_chats/video_chat_started.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/types/user_and_chats/video_chat_started.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/pyrogram/utils.py` & `PyroFork-dev-2.2.6.dev202308012705/pyrogram/utils.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/setup.py` & `PyroFork-dev-2.2.6.dev202308012705/setup.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/tests/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/tests/filters/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/tests/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/tests/filters/test_command.py` & `PyroFork-dev-2.2.6.dev202308012705/tests/filters/test_command.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/tests/parser/__init__.py` & `PyroFork-dev-2.2.6.dev202308012705/tests/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/tests/parser/test_html.py` & `PyroFork-dev-2.2.6.dev202308012705/tests/parser/test_html.py`

 * *Files identical despite different names*

### Comparing `PyroFork-dev-2.2.6.dev202307272537/tests/test_file_id.py` & `PyroFork-dev-2.2.6.dev202308012705/tests/test_file_id.py`

 * *Files identical despite different names*

