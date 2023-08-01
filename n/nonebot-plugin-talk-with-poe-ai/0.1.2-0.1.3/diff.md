# Comparing `tmp/nonebot_plugin_talk_with_poe_ai-0.1.2.tar.gz` & `tmp/nonebot_plugin_talk_with_poe_ai-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_talk_with_poe_ai-0.1.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_talk_with_poe_ai-0.1.3.tar", max compression
```

## Comparing `nonebot_plugin_talk_with_poe_ai-0.1.2.tar` & `nonebot_plugin_talk_with_poe_ai-0.1.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0    12104 2023-08-01 13:22:09.154390 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/__init__.py
--rw-r--r--   0        0        0       32 2023-08-01 03:19:51.510068 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/__init__.py
--rw-r--r--   0        0        0    49262 2023-08-01 13:29:33.340733 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/client.py
--rw-r--r--   0        0        0     1145 2023-08-01 03:19:51.511055 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/AddHumanMessageMutation.graphql
--rw-r--r--   0        0        0      536 2023-08-01 03:19:51.512054 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/AddMessageBreakMutation.graphql
--rw-r--r--   0        0        0      187 2023-08-01 03:19:51.512054 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/AutoSubscriptionMutation.graphql
--rw-r--r--   0        0        0      701 2023-08-01 03:19:51.513055 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/availableBotsListModalPaginationQuery.graphql
--rw-r--r--   0        0        0      105 2023-08-01 03:19:51.513055 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/BioFragment.graphql
--rw-r--r--   0        0        0      169 2023-08-01 03:19:51.514055 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/BotDeletionButton_poeBotDelete_Mutation.graphql
--rw-r--r--   0        0        0       78 2023-08-01 03:19:51.514055 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatAddedSubscription.graphql
--rw-r--r--   0        0        0      106 2023-08-01 03:19:51.515056 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatFragment.graphql
--rw-r--r--   0        0        0    12084 2023-08-01 03:19:51.515056 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatListPaginationQuery.graphql
--rw-r--r--   0        0        0      712 2023-08-01 03:19:51.516054 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatPaginationQuery.graphql
--rw-r--r--   0        0        0      162 2023-08-01 03:19:51.516054 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatViewQuery.graphql
--rw-r--r--   0        0        0      167 2023-08-01 03:19:51.517055 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/DeleteHumanMessagesMutation.graphql
--rw-r--r--   0        0        0      129 2023-08-01 03:19:51.517055 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/DeleteMessageMutation.graphql
--rw-r--r--   0        0        0      154 2023-08-01 03:19:51.517993 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/DeleteUserMessagesMutation.graphql
--rw-r--r--   0        0        0     1148 2023-08-01 03:19:51.517993 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ExploreBotsListPaginationQuery.graphql
--rw-r--r--   0        0        0      111 2023-08-01 03:19:51.518986 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/HandleFragment.graphql
--rw-r--r--   0        0        0      319 2023-08-01 03:19:51.518986 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/LoginWithVerificationCodeMutation.graphql
--rw-r--r--   0        0        0     1985 2023-08-01 03:19:51.519987 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageAddedSubscription.graphql
--rw-r--r--   0        0        0      141 2023-08-01 03:19:51.520991 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageDeletedSubscription.graphql
--rw-r--r--   0        0        0      207 2023-08-01 03:19:51.520991 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageFragment.graphql
--rw-r--r--   0        0        0      152 2023-08-01 03:19:51.521987 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageRemoveVoteMutation.graphql
--rw-r--r--   0        0        0      223 2023-08-01 03:19:51.522987 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageSetVoteMutation.graphql
--rw-r--r--   0        0        0     1832 2023-08-01 03:19:51.522987 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/PoeBotCreateMutation.graphql
--rw-r--r--   0        0        0      968 2023-08-01 03:19:51.523987 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/PoeBotEditMutation.graphql
--rw-r--r--   0        0        0      963 2023-08-01 03:19:51.524986 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SendMessageMutation.graphql
--rw-r--r--   0        0        0      275 2023-08-01 03:19:51.524986 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SendVerificationCodeForLoginMutation.graphql
--rw-r--r--   0        0        0      222 2023-08-01 03:19:51.525986 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ShareMessagesMutation.graphql
--rw-r--r--   0        0        0      321 2023-08-01 03:19:51.525986 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SignupWithVerificationCodeMutation.graphql
--rw-r--r--   0        0        0      166 2023-08-01 03:19:51.526987 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/StaleChatUpdateMutation.graphql
--rw-r--r--   0        0        0      170 2023-08-01 03:19:51.526987 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SubscriptionsMutation.graphql
--rw-r--r--   0        0        0       98 2023-08-01 03:19:51.527990 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SummarizePlainPostQuery.graphql
--rw-r--r--   0        0        0      150 2023-08-01 03:19:51.528991 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SummarizeQuotePostQuery.graphql
--rw-r--r--   0        0        0      183 2023-08-01 03:19:51.528991 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SummarizeSharePostQuery.graphql
--rw-r--r--   0        0        0      382 2023-08-01 03:19:51.529994 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/UserSnippetFragment.graphql
--rw-r--r--   0        0        0      421 2023-08-01 03:19:51.529994 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ViewerInfoQuery.graphql
--rw-r--r--   0        0        0     1068 2023-08-01 03:19:51.530986 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ViewerStateFragment.graphql
--rw-r--r--   0        0        0      700 2023-08-01 03:19:51.530986 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ViewerStateUpdatedSubscription.graphql
--rw-r--r--   0        0        0       53 2023-08-01 03:19:51.531986 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/requirements.txt
--rw-r--r--   0        0        0     1648 2023-08-01 13:29:20.242168 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/util.py
--rw-r--r--   0        0        0    10484 2023-08-01 13:11:08.666579 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/config.py
--rw-r--r--   0        0        0     4826 2023-08-01 08:04:47.152640 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/data_handle.py
--rw-r--r--   0        0        0  7232220 2023-01-06 09:31:31.000000 nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/HYWenHei-85W.ttf
--rw-r--r--   0        0        0     1009 2023-08-01 13:29:46.574351 nonebot_plugin_talk_with_poe_ai-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5466 2023-08-01 13:29:49.857577 nonebot_plugin_talk_with_poe_ai-0.1.2/README.md
--rw-r--r--   0        0        0     6451 1970-01-01 00:00:00.000000 nonebot_plugin_talk_with_poe_ai-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    12104 2023-08-01 13:22:09.154390 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/__init__.py
+-rw-r--r--   0        0        0       32 2023-08-01 03:19:51.510068 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/__init__.py
+-rw-r--r--   0        0        0    49240 2023-08-01 13:31:07.632194 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/client.py
+-rw-r--r--   0        0        0     1145 2023-08-01 03:19:51.511055 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/AddHumanMessageMutation.graphql
+-rw-r--r--   0        0        0      536 2023-08-01 03:19:51.512054 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/AddMessageBreakMutation.graphql
+-rw-r--r--   0        0        0      187 2023-08-01 03:19:51.512054 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/AutoSubscriptionMutation.graphql
+-rw-r--r--   0        0        0      701 2023-08-01 03:19:51.513055 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/availableBotsListModalPaginationQuery.graphql
+-rw-r--r--   0        0        0      105 2023-08-01 03:19:51.513055 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/BioFragment.graphql
+-rw-r--r--   0        0        0      169 2023-08-01 03:19:51.514055 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/BotDeletionButton_poeBotDelete_Mutation.graphql
+-rw-r--r--   0        0        0       78 2023-08-01 03:19:51.514055 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatAddedSubscription.graphql
+-rw-r--r--   0        0        0      106 2023-08-01 03:19:51.515056 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatFragment.graphql
+-rw-r--r--   0        0        0    12084 2023-08-01 03:19:51.515056 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatListPaginationQuery.graphql
+-rw-r--r--   0        0        0      712 2023-08-01 03:19:51.516054 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatPaginationQuery.graphql
+-rw-r--r--   0        0        0      162 2023-08-01 03:19:51.516054 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatViewQuery.graphql
+-rw-r--r--   0        0        0      167 2023-08-01 03:19:51.517055 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/DeleteHumanMessagesMutation.graphql
+-rw-r--r--   0        0        0      129 2023-08-01 03:19:51.517055 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/DeleteMessageMutation.graphql
+-rw-r--r--   0        0        0      154 2023-08-01 03:19:51.517993 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/DeleteUserMessagesMutation.graphql
+-rw-r--r--   0        0        0     1148 2023-08-01 03:19:51.517993 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ExploreBotsListPaginationQuery.graphql
+-rw-r--r--   0        0        0      111 2023-08-01 03:19:51.518986 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/HandleFragment.graphql
+-rw-r--r--   0        0        0      319 2023-08-01 03:19:51.518986 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/LoginWithVerificationCodeMutation.graphql
+-rw-r--r--   0        0        0     1985 2023-08-01 03:19:51.519987 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageAddedSubscription.graphql
+-rw-r--r--   0        0        0      141 2023-08-01 03:19:51.520991 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageDeletedSubscription.graphql
+-rw-r--r--   0        0        0      207 2023-08-01 03:19:51.520991 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageFragment.graphql
+-rw-r--r--   0        0        0      152 2023-08-01 03:19:51.521987 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageRemoveVoteMutation.graphql
+-rw-r--r--   0        0        0      223 2023-08-01 03:19:51.522987 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageSetVoteMutation.graphql
+-rw-r--r--   0        0        0     1832 2023-08-01 03:19:51.522987 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/PoeBotCreateMutation.graphql
+-rw-r--r--   0        0        0      968 2023-08-01 03:19:51.523987 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/PoeBotEditMutation.graphql
+-rw-r--r--   0        0        0      963 2023-08-01 03:19:51.524986 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SendMessageMutation.graphql
+-rw-r--r--   0        0        0      275 2023-08-01 03:19:51.524986 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SendVerificationCodeForLoginMutation.graphql
+-rw-r--r--   0        0        0      222 2023-08-01 03:19:51.525986 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ShareMessagesMutation.graphql
+-rw-r--r--   0        0        0      321 2023-08-01 03:19:51.525986 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SignupWithVerificationCodeMutation.graphql
+-rw-r--r--   0        0        0      166 2023-08-01 03:19:51.526987 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/StaleChatUpdateMutation.graphql
+-rw-r--r--   0        0        0      170 2023-08-01 03:19:51.526987 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SubscriptionsMutation.graphql
+-rw-r--r--   0        0        0       98 2023-08-01 03:19:51.527990 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SummarizePlainPostQuery.graphql
+-rw-r--r--   0        0        0      150 2023-08-01 03:19:51.528991 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SummarizeQuotePostQuery.graphql
+-rw-r--r--   0        0        0      183 2023-08-01 03:19:51.528991 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SummarizeSharePostQuery.graphql
+-rw-r--r--   0        0        0      382 2023-08-01 03:19:51.529994 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/UserSnippetFragment.graphql
+-rw-r--r--   0        0        0      421 2023-08-01 03:19:51.529994 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ViewerInfoQuery.graphql
+-rw-r--r--   0        0        0     1068 2023-08-01 03:19:51.530986 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ViewerStateFragment.graphql
+-rw-r--r--   0        0        0      700 2023-08-01 03:19:51.530986 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ViewerStateUpdatedSubscription.graphql
+-rw-r--r--   0        0        0       53 2023-08-01 03:19:51.531986 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/requirements.txt
+-rw-r--r--   0        0        0     1648 2023-08-01 13:29:20.242168 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/util.py
+-rw-r--r--   0        0        0    10484 2023-08-01 13:11:08.666579 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/config.py
+-rw-r--r--   0        0        0     4826 2023-08-01 08:04:47.152640 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/data_handle.py
+-rw-r--r--   0        0        0  7232220 2023-01-06 09:31:31.000000 nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/HYWenHei-85W.ttf
+-rw-r--r--   0        0        0     1009 2023-08-01 13:31:16.850270 nonebot_plugin_talk_with_poe_ai-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5466 2023-08-01 13:31:11.755619 nonebot_plugin_talk_with_poe_ai-0.1.3/README.md
+-rw-r--r--   0        0        0     6451 1970-01-01 00:00:00.000000 nonebot_plugin_talk_with_poe_ai-0.1.3/PKG-INFO
```

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/__init__.py` & `nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/client.py` & `nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     GQL_URL,
     GQL_RECV_URL,
     SETTING_URL,
     CONST_NAMESPACE,
     generate_data,
     QUERIES,
     generate_nonce,
-    extract_formkey,
 )
 
 
 class Poe_Client:
     def __init__(
         self, p_b: str, formkey: Optional[str] = "", proxy: Optional[str] = ""
     ):
```

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/AddHumanMessageMutation.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/AddHumanMessageMutation.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/AddMessageBreakMutation.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/AddMessageBreakMutation.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/availableBotsListModalPaginationQuery.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/availableBotsListModalPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatListPaginationQuery.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatListPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatPaginationQuery.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ChatPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ExploreBotsListPaginationQuery.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ExploreBotsListPaginationQuery.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageAddedSubscription.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/MessageAddedSubscription.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/PoeBotCreateMutation.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/PoeBotCreateMutation.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/PoeBotEditMutation.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/PoeBotEditMutation.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SendMessageMutation.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/SendMessageMutation.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ViewerStateFragment.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ViewerStateFragment.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ViewerStateUpdatedSubscription.graphql` & `nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/poe_graphql/ViewerStateUpdatedSubscription.graphql`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/async_poe_client/util.py` & `nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/async_poe_client/util.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/config.py` & `nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/data_handle.py` & `nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/data_handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.2/nonebot_plugin_talk_with_poe_ai/HYWenHei-85W.ttf` & `nonebot_plugin_talk_with_poe_ai-0.1.3/nonebot_plugin_talk_with_poe_ai/HYWenHei-85W.ttf`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.2/pyproject.toml` & `nonebot_plugin_talk_with_poe_ai-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_talk_with_poe_ai"
-version = "0.1.2"
+version = "0.1.3"
 description = "Nonebot2 基于poe cookie登录AI聊天插件"
 authors = ["nikissXI <1299577815@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_talk_with_poe_ai"}]
 homepage = "https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_poe_ai"
 repository = "https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_poe_ai"
```

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.2/README.md` & `nonebot_plugin_talk_with_poe_ai-0.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -117,10 +117,10 @@
 | /reset | 重置对话（不会重置预设） |
 | /prompt | 设置预设（人格），设置后会重置对话 |
 | /poeai | 如果talk_with_poe_ai_all_group_enable为false，则用该命令启用 |
 | /poeai re | poe ai 重连，有时候可能各种因素导致登陆失败 |
 | /poeai auth | 修改登录凭证并重新登录 |
 
 ## 更新日志
-### 2023/8/1 \[v0.1.2]
+### 2023/8/1 \[v0.1.3]
 
 * 发布插件
```

#### html2text {}

```diff
@@ -63,8 +63,8 @@
 | å¼å§å¯¹è¯ï¼é»è®¤ç¾¤é@æºå¨äººä¹å¯ä»¥ | | /hi |
 æ²æµ¸å¼å¯¹è¯ï¼ä»éç§èï¼ | | /reset |
 éç½®å¯¹è¯ï¼ä¸ä¼éç½®é¢è®¾ï¼ | | /prompt |
 è®¾ç½®é¢è®¾ï¼äººæ ¼ï¼ï¼è®¾ç½®åä¼éç½®å¯¹è¯ | | /poeai |
 å¦ætalk_with_poe_ai_all_group_enableä¸ºfalseï¼åç¨è¯¥å½ä»¤å¯ç¨ | | /
 poeai re | poe ai éè¿ï¼ææ¶åå¯è½åç§å ç´ å¯¼è´ç»éå¤±è´¥ | | /
 poeai auth | ä¿®æ¹ç»å½å­è¯å¹¶éæ°ç»å½ | ## æ´æ°æ¥å¿ ### 2023/8/1 \
-[v0.1.2] * åå¸æä»¶
+[v0.1.3] * åå¸æä»¶
```

### Comparing `nonebot_plugin_talk_with_poe_ai-0.1.2/PKG-INFO` & `nonebot_plugin_talk_with_poe_ai-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-talk-with-poe-ai
-Version: 0.1.2
+Version: 0.1.3
 Summary: Nonebot2 基于poe cookie登录AI聊天插件
 Home-page: https://github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_poe_ai
 License: MIT
 Author: nikissXI
 Author-email: 1299577815@qq.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -142,11 +142,11 @@
 | /reset | 重置对话（不会重置预设） |
 | /prompt | 设置预设（人格），设置后会重置对话 |
 | /poeai | 如果talk_with_poe_ai_all_group_enable为false，则用该命令启用 |
 | /poeai re | poe ai 重连，有时候可能各种因素导致登陆失败 |
 | /poeai auth | 修改登录凭证并重新登录 |
 
 ## 更新日志
-### 2023/8/1 \[v0.1.2]
+### 2023/8/1 \[v0.1.3]
 
 * 发布插件
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-talk-with-poe-ai Version: 0.1.2
+Metadata-Version: 2.1 Name: nonebot-plugin-talk-with-poe-ai Version: 0.1.3
 Summary: Nonebot2 åºäºpoe cookieç»å½AIèå¤©æä»¶ Home-page: https://
 github.com/nikissXI/nonebot_plugins/tree/main/nonebot_plugin_talk_with_poe_ai
 License: MIT Author: nikissXI Author-email: 1299577815@qq.com Requires-Python:
 >=3.8 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
@@ -78,8 +78,8 @@
 | å¼å§å¯¹è¯ï¼é»è®¤ç¾¤é@æºå¨äººä¹å¯ä»¥ | | /hi |
 æ²æµ¸å¼å¯¹è¯ï¼ä»éç§èï¼ | | /reset |
 éç½®å¯¹è¯ï¼ä¸ä¼éç½®é¢è®¾ï¼ | | /prompt |
 è®¾ç½®é¢è®¾ï¼äººæ ¼ï¼ï¼è®¾ç½®åä¼éç½®å¯¹è¯ | | /poeai |
 å¦ætalk_with_poe_ai_all_group_enableä¸ºfalseï¼åç¨è¯¥å½ä»¤å¯ç¨ | | /
 poeai re | poe ai éè¿ï¼ææ¶åå¯è½åç§å ç´ å¯¼è´ç»éå¤±è´¥ | | /
 poeai auth | ä¿®æ¹ç»å½å­è¯å¹¶éæ°ç»å½ | ## æ´æ°æ¥å¿ ### 2023/8/1 \
-[v0.1.2] * åå¸æä»¶
+[v0.1.3] * åå¸æä»¶
```

