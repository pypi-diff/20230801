# Comparing `tmp/llmtuner-0.1.3.tar.gz` & `tmp/llmtuner-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmtuner-0.1.3.tar", last modified: Fri Jul 21 08:46:23 2023, max compression
+gzip compressed data, was "llmtuner-0.1.4.tar", last modified: Tue Aug  1 04:14:57 2023, max compression
```

## Comparing `llmtuner-0.1.3.tar` & `llmtuner-0.1.4.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-21 08:46:23.642495 llmtuner-0.1.3/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    11524 2023-07-21 08:45:52.000000 llmtuner-0.1.3/LICENSE
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    15186 2023-07-21 08:46:23.642495 llmtuner-0.1.3/PKG-INFO
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    14586 2023-07-21 08:45:58.000000 llmtuner-0.1.3/README.md
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       87 2023-07-21 08:45:58.000000 llmtuner-0.1.3/pyproject.toml
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       38 2023-07-21 08:46:23.642495 llmtuner-0.1.3/setup.cfg
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2033 2023-07-21 08:45:58.000000 llmtuner-0.1.3/setup.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-21 08:46:23.466489 llmtuner-0.1.3/src/
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-21 08:46:23.482490 llmtuner-0.1.3/src/llmtuner/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       64 2023-07-21 08:45:56.000000 llmtuner-0.1.3/src/llmtuner/__init__.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-21 08:46:23.490490 llmtuner-0.1.3/src/llmtuner/api/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-07-21 08:45:53.000000 llmtuner-0.1.3/src/llmtuner/api/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4620 2023-07-21 08:45:53.000000 llmtuner-0.1.3/src/llmtuner/api/app.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2146 2023-07-21 08:45:53.000000 llmtuner-0.1.3/src/llmtuner/api/protocol.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-21 08:46:23.494490 llmtuner-0.1.3/src/llmtuner/chat/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-07-21 08:45:53.000000 llmtuner-0.1.3/src/llmtuner/chat/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3670 2023-07-21 08:45:53.000000 llmtuner-0.1.3/src/llmtuner/chat/stream_chat.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-21 08:46:23.502490 llmtuner-0.1.3/src/llmtuner/dsets/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      153 2023-07-21 08:45:54.000000 llmtuner-0.1.3/src/llmtuner/dsets/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4294 2023-07-21 08:45:53.000000 llmtuner-0.1.3/src/llmtuner/dsets/loader.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     8250 2023-07-21 08:45:53.000000 llmtuner-0.1.3/src/llmtuner/dsets/preprocess.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      515 2023-07-21 08:45:53.000000 llmtuner-0.1.3/src/llmtuner/dsets/utils.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-21 08:46:23.514491 llmtuner-0.1.3/src/llmtuner/extras/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-07-21 08:45:54.000000 llmtuner-0.1.3/src/llmtuner/extras/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3138 2023-07-21 08:45:54.000000 llmtuner-0.1.3/src/llmtuner/extras/callbacks.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1735 2023-07-21 08:45:54.000000 llmtuner-0.1.3/src/llmtuner/extras/constants.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      751 2023-07-21 08:45:54.000000 llmtuner-0.1.3/src/llmtuner/extras/logging.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3884 2023-07-21 08:45:54.000000 llmtuner-0.1.3/src/llmtuner/extras/misc.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1788 2023-07-21 08:45:54.000000 llmtuner-0.1.3/src/llmtuner/extras/ploting.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2196 2023-07-21 08:45:54.000000 llmtuner-0.1.3/src/llmtuner/extras/save_and_load.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6500 2023-07-21 08:45:54.000000 llmtuner-0.1.3/src/llmtuner/extras/template.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-21 08:46:23.530491 llmtuner-0.1.3/src/llmtuner/hparams/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      222 2023-07-21 08:45:54.000000 llmtuner-0.1.3/src/llmtuner/hparams/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5013 2023-07-21 08:45:54.000000 llmtuner-0.1.3/src/llmtuner/hparams/data_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3831 2023-07-21 08:45:54.000000 llmtuner-0.1.3/src/llmtuner/hparams/finetuning_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      388 2023-07-21 08:45:54.000000 llmtuner-0.1.3/src/llmtuner/hparams/general_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1973 2023-07-21 08:45:54.000000 llmtuner-0.1.3/src/llmtuner/hparams/generating_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3053 2023-07-21 08:45:54.000000 llmtuner-0.1.3/src/llmtuner/hparams/model_args.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-21 08:46:23.534491 llmtuner-0.1.3/src/llmtuner/tuner/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      241 2023-07-21 08:45:56.000000 llmtuner-0.1.3/src/llmtuner/tuner/__init__.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-21 08:46:23.554492 llmtuner-0.1.3/src/llmtuner/tuner/core/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      136 2023-07-21 08:45:55.000000 llmtuner-0.1.3/src/llmtuner/tuner/core/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3839 2023-07-21 08:45:55.000000 llmtuner-0.1.3/src/llmtuner/tuner/core/adapter.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6881 2023-07-21 08:45:55.000000 llmtuner-0.1.3/src/llmtuner/tuner/core/loader.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6431 2023-07-21 08:45:55.000000 llmtuner-0.1.3/src/llmtuner/tuner/core/parser.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4315 2023-07-21 08:45:55.000000 llmtuner-0.1.3/src/llmtuner/tuner/core/trainer.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-21 08:46:23.574493 llmtuner-0.1.3/src/llmtuner/tuner/ppo/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-07-21 08:45:55.000000 llmtuner-0.1.3/src/llmtuner/tuner/ppo/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     8221 2023-07-21 08:45:55.000000 llmtuner-0.1.3/src/llmtuner/tuner/ppo/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1673 2023-07-21 08:45:55.000000 llmtuner-0.1.3/src/llmtuner/tuner/ppo/utils.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3083 2023-07-21 08:45:55.000000 llmtuner-0.1.3/src/llmtuner/tuner/ppo/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-21 08:46:23.578493 llmtuner-0.1.3/src/llmtuner/tuner/pt/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       47 2023-07-21 08:45:55.000000 llmtuner-0.1.3/src/llmtuner/tuner/pt/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2516 2023-07-21 08:45:55.000000 llmtuner-0.1.3/src/llmtuner/tuner/pt/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-21 08:46:23.590494 llmtuner-0.1.3/src/llmtuner/tuner/rm/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       47 2023-07-21 08:45:56.000000 llmtuner-0.1.3/src/llmtuner/tuner/rm/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      722 2023-07-21 08:45:56.000000 llmtuner-0.1.3/src/llmtuner/tuner/rm/collator.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      273 2023-07-21 08:45:56.000000 llmtuner-0.1.3/src/llmtuner/tuner/rm/metric.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2555 2023-07-21 08:45:56.000000 llmtuner-0.1.3/src/llmtuner/tuner/rm/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2800 2023-07-21 08:45:56.000000 llmtuner-0.1.3/src/llmtuner/tuner/rm/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-21 08:46:23.598494 llmtuner-0.1.3/src/llmtuner/tuner/sft/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-07-21 08:45:56.000000 llmtuner-0.1.3/src/llmtuner/tuner/sft/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2183 2023-07-21 08:45:56.000000 llmtuner-0.1.3/src/llmtuner/tuner/sft/metric.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4553 2023-07-21 08:45:56.000000 llmtuner-0.1.3/src/llmtuner/tuner/sft/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3896 2023-07-21 08:45:56.000000 llmtuner-0.1.3/src/llmtuner/tuner/sft/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-21 08:46:23.618494 llmtuner-0.1.3/src/llmtuner/webui/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-07-21 08:45:57.000000 llmtuner-0.1.3/src/llmtuner/webui/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2997 2023-07-21 08:45:56.000000 llmtuner-0.1.3/src/llmtuner/webui/chat.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2564 2023-07-21 08:45:56.000000 llmtuner-0.1.3/src/llmtuner/webui/common.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-21 08:46:23.638495 llmtuner-0.1.3/src/llmtuner/webui/components/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      298 2023-07-21 08:45:57.000000 llmtuner-0.1.3/src/llmtuner/webui/components/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1703 2023-07-21 08:45:57.000000 llmtuner-0.1.3/src/llmtuner/webui/components/chatbot.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      625 2023-07-21 08:45:57.000000 llmtuner-0.1.3/src/llmtuner/webui/components/data.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2567 2023-07-21 08:45:57.000000 llmtuner-0.1.3/src/llmtuner/webui/components/eval.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      895 2023-07-21 08:45:57.000000 llmtuner-0.1.3/src/llmtuner/webui/components/export.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1424 2023-07-21 08:45:57.000000 llmtuner-0.1.3/src/llmtuner/webui/components/infer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5116 2023-07-21 08:45:57.000000 llmtuner-0.1.3/src/llmtuner/webui/components/sft.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2081 2023-07-21 08:45:57.000000 llmtuner-0.1.3/src/llmtuner/webui/components/top.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      387 2023-07-21 08:45:57.000000 llmtuner-0.1.3/src/llmtuner/webui/css.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1585 2023-07-21 08:45:57.000000 llmtuner-0.1.3/src/llmtuner/webui/interface.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    13920 2023-07-21 08:45:57.000000 llmtuner-0.1.3/src/llmtuner/webui/locales.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1224 2023-07-21 08:45:57.000000 llmtuner-0.1.3/src/llmtuner/webui/manager.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     8176 2023-07-21 08:45:57.000000 llmtuner-0.1.3/src/llmtuner/webui/runner.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4279 2023-07-21 08:45:57.000000 llmtuner-0.1.3/src/llmtuner/webui/utils.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-21 08:46:23.486490 llmtuner-0.1.3/src/llmtuner.egg-info/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    15186 2023-07-21 08:46:22.000000 llmtuner-0.1.3/src/llmtuner.egg-info/PKG-INFO
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2274 2023-07-21 08:46:22.000000 llmtuner-0.1.3/src/llmtuner.egg-info/SOURCES.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        1 2023-07-21 08:46:22.000000 llmtuner-0.1.3/src/llmtuner.egg-info/dependency_links.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      215 2023-07-21 08:46:22.000000 llmtuner-0.1.3/src/llmtuner.egg-info/requires.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        9 2023-07-21 08:46:22.000000 llmtuner-0.1.3/src/llmtuner.egg-info/top_level.txt
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-01 04:14:57.470154 llmtuner-0.1.4/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    11524 2023-07-21 08:45:52.000000 llmtuner-0.1.4/LICENSE
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    15186 2023-08-01 04:14:57.470154 llmtuner-0.1.4/PKG-INFO
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    14586 2023-07-21 08:45:58.000000 llmtuner-0.1.4/README.md
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       87 2023-07-21 08:45:58.000000 llmtuner-0.1.4/pyproject.toml
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       38 2023-08-01 04:14:57.470154 llmtuner-0.1.4/setup.cfg
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2033 2023-07-21 08:45:58.000000 llmtuner-0.1.4/setup.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-01 04:14:56.326114 llmtuner-0.1.4/src/
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-01 04:14:56.346114 llmtuner-0.1.4/src/llmtuner/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       64 2023-08-01 04:05:57.000000 llmtuner-0.1.4/src/llmtuner/__init__.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-01 04:14:56.362115 llmtuner-0.1.4/src/llmtuner/api/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-08-01 04:05:52.000000 llmtuner-0.1.4/src/llmtuner/api/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4620 2023-08-01 04:05:52.000000 llmtuner-0.1.4/src/llmtuner/api/app.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2146 2023-08-01 04:05:52.000000 llmtuner-0.1.4/src/llmtuner/api/protocol.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-01 04:14:56.394116 llmtuner-0.1.4/src/llmtuner/chat/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-08-01 04:05:52.000000 llmtuner-0.1.4/src/llmtuner/chat/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4420 2023-08-01 04:05:52.000000 llmtuner-0.1.4/src/llmtuner/chat/stream_chat.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-01 04:14:56.510120 llmtuner-0.1.4/src/llmtuner/dsets/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      153 2023-08-01 04:05:53.000000 llmtuner-0.1.4/src/llmtuner/dsets/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4657 2023-08-01 04:05:53.000000 llmtuner-0.1.4/src/llmtuner/dsets/loader.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     9418 2023-08-01 04:05:53.000000 llmtuner-0.1.4/src/llmtuner/dsets/preprocess.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      547 2023-08-01 04:05:53.000000 llmtuner-0.1.4/src/llmtuner/dsets/utils.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-01 04:14:56.630125 llmtuner-0.1.4/src/llmtuner/extras/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-08-01 04:05:53.000000 llmtuner-0.1.4/src/llmtuner/extras/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3091 2023-08-01 04:05:53.000000 llmtuner-0.1.4/src/llmtuner/extras/callbacks.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1735 2023-08-01 04:05:53.000000 llmtuner-0.1.4/src/llmtuner/extras/constants.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      965 2023-08-01 04:05:53.000000 llmtuner-0.1.4/src/llmtuner/extras/logging.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4262 2023-08-01 04:05:53.000000 llmtuner-0.1.4/src/llmtuner/extras/misc.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1788 2023-08-01 04:05:53.000000 llmtuner-0.1.4/src/llmtuner/extras/ploting.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2148 2023-08-01 04:05:53.000000 llmtuner-0.1.4/src/llmtuner/extras/save_and_load.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     6468 2023-08-01 04:05:53.000000 llmtuner-0.1.4/src/llmtuner/extras/template.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-01 04:14:56.746129 llmtuner-0.1.4/src/llmtuner/hparams/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      222 2023-08-01 04:05:54.000000 llmtuner-0.1.4/src/llmtuner/hparams/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5414 2023-08-01 04:05:54.000000 llmtuner-0.1.4/src/llmtuner/hparams/data_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3831 2023-08-01 04:05:54.000000 llmtuner-0.1.4/src/llmtuner/hparams/finetuning_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      374 2023-08-01 04:05:54.000000 llmtuner-0.1.4/src/llmtuner/hparams/general_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1973 2023-08-01 04:05:54.000000 llmtuner-0.1.4/src/llmtuner/hparams/generating_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3053 2023-08-01 04:05:54.000000 llmtuner-0.1.4/src/llmtuner/hparams/model_args.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-01 04:14:56.770130 llmtuner-0.1.4/src/llmtuner/tuner/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      241 2023-08-01 04:05:55.000000 llmtuner-0.1.4/src/llmtuner/tuner/__init__.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-01 04:14:56.926135 llmtuner-0.1.4/src/llmtuner/tuner/core/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      136 2023-08-01 04:05:54.000000 llmtuner-0.1.4/src/llmtuner/tuner/core/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3910 2023-08-01 04:05:54.000000 llmtuner-0.1.4/src/llmtuner/tuner/core/adapter.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     7060 2023-08-01 04:05:54.000000 llmtuner-0.1.4/src/llmtuner/tuner/core/loader.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     6910 2023-08-01 04:05:54.000000 llmtuner-0.1.4/src/llmtuner/tuner/core/parser.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4228 2023-08-01 04:05:54.000000 llmtuner-0.1.4/src/llmtuner/tuner/core/trainer.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-01 04:14:56.986137 llmtuner-0.1.4/src/llmtuner/tuner/ppo/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-08-01 04:05:55.000000 llmtuner-0.1.4/src/llmtuner/tuner/ppo/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     8287 2023-08-01 04:05:54.000000 llmtuner-0.1.4/src/llmtuner/tuner/ppo/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1719 2023-08-01 04:05:54.000000 llmtuner-0.1.4/src/llmtuner/tuner/ppo/utils.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3181 2023-08-01 04:05:54.000000 llmtuner-0.1.4/src/llmtuner/tuner/ppo/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-01 04:14:57.010138 llmtuner-0.1.4/src/llmtuner/tuner/pt/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       47 2023-08-01 04:05:55.000000 llmtuner-0.1.4/src/llmtuner/tuner/pt/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2595 2023-08-01 04:05:55.000000 llmtuner-0.1.4/src/llmtuner/tuner/pt/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-01 04:14:57.094141 llmtuner-0.1.4/src/llmtuner/tuner/rm/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       47 2023-08-01 04:05:55.000000 llmtuner-0.1.4/src/llmtuner/tuner/rm/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      802 2023-08-01 04:05:55.000000 llmtuner-0.1.4/src/llmtuner/tuner/rm/collator.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      273 2023-08-01 04:05:55.000000 llmtuner-0.1.4/src/llmtuner/tuner/rm/metric.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2601 2023-08-01 04:05:55.000000 llmtuner-0.1.4/src/llmtuner/tuner/rm/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2854 2023-08-01 04:05:55.000000 llmtuner-0.1.4/src/llmtuner/tuner/rm/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-01 04:14:57.158143 llmtuner-0.1.4/src/llmtuner/tuner/sft/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-08-01 04:05:55.000000 llmtuner-0.1.4/src/llmtuner/tuner/sft/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2225 2023-08-01 04:05:55.000000 llmtuner-0.1.4/src/llmtuner/tuner/sft/metric.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4595 2023-08-01 04:05:55.000000 llmtuner-0.1.4/src/llmtuner/tuner/sft/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3975 2023-08-01 04:05:55.000000 llmtuner-0.1.4/src/llmtuner/tuner/sft/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-01 04:14:57.298148 llmtuner-0.1.4/src/llmtuner/webui/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-08-01 04:05:56.000000 llmtuner-0.1.4/src/llmtuner/webui/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3089 2023-08-01 04:05:55.000000 llmtuner-0.1.4/src/llmtuner/webui/chat.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2564 2023-08-01 04:05:55.000000 llmtuner-0.1.4/src/llmtuner/webui/common.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-01 04:14:57.454153 llmtuner-0.1.4/src/llmtuner/webui/components/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      298 2023-08-01 04:05:56.000000 llmtuner-0.1.4/src/llmtuner/webui/components/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1759 2023-08-01 04:05:56.000000 llmtuner-0.1.4/src/llmtuner/webui/components/chatbot.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      677 2023-08-01 04:05:56.000000 llmtuner-0.1.4/src/llmtuner/webui/components/data.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2617 2023-08-01 04:05:56.000000 llmtuner-0.1.4/src/llmtuner/webui/components/eval.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      939 2023-08-01 04:05:56.000000 llmtuner-0.1.4/src/llmtuner/webui/components/export.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1468 2023-08-01 04:05:56.000000 llmtuner-0.1.4/src/llmtuner/webui/components/infer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5166 2023-08-01 04:05:56.000000 llmtuner-0.1.4/src/llmtuner/webui/components/sft.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2123 2023-08-01 04:05:56.000000 llmtuner-0.1.4/src/llmtuner/webui/components/top.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      387 2023-08-01 04:05:56.000000 llmtuner-0.1.4/src/llmtuner/webui/css.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1603 2023-08-01 04:05:56.000000 llmtuner-0.1.4/src/llmtuner/webui/interface.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    13920 2023-08-01 04:05:56.000000 llmtuner-0.1.4/src/llmtuner/webui/locales.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1261 2023-08-01 04:05:56.000000 llmtuner-0.1.4/src/llmtuner/webui/manager.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     8162 2023-08-01 04:05:56.000000 llmtuner-0.1.4/src/llmtuner/webui/runner.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4279 2023-08-01 04:05:56.000000 llmtuner-0.1.4/src/llmtuner/webui/utils.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-01 04:14:56.350115 llmtuner-0.1.4/src/llmtuner.egg-info/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    15186 2023-08-01 04:14:55.000000 llmtuner-0.1.4/src/llmtuner.egg-info/PKG-INFO
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2274 2023-08-01 04:14:55.000000 llmtuner-0.1.4/src/llmtuner.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        1 2023-08-01 04:14:55.000000 llmtuner-0.1.4/src/llmtuner.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      215 2023-08-01 04:14:55.000000 llmtuner-0.1.4/src/llmtuner.egg-info/requires.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        9 2023-08-01 04:14:55.000000 llmtuner-0.1.4/src/llmtuner.egg-info/top_level.txt
```

### Comparing `llmtuner-0.1.3/LICENSE` & `llmtuner-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.3/PKG-INFO` & `llmtuner-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmtuner
-Version: 0.1.3
+Version: 0.1.4
 Summary: Easy-to-use fine-tuning framework using PEFT
 Home-page: https://github.com/hiyouga/LLaMA-Efficient-Tuning
 Author: hiyouga
 Author-email: hiyouga@buaa.edu.cn
 License: Apache 2.0 License
 Keywords: LLaMA,BLOOM,Falcon,LLM,ChatGPT,transformer,pytorch,deep learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `llmtuner-0.1.3/README.md` & `llmtuner-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.3/setup.py` & `llmtuner-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.3/src/llmtuner/api/app.py` & `llmtuner-0.1.4/src/llmtuner/api/app.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.3/src/llmtuner/api/protocol.py` & `llmtuner-0.1.4/src/llmtuner/api/protocol.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.3/src/llmtuner/dsets/loader.py` & `llmtuner-0.1.4/src/llmtuner/dsets/loader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,106 +1,112 @@
 import os
 import hashlib
-from typing import List
+from typing import TYPE_CHECKING, List, Optional
 
-from datasets import Dataset, concatenate_datasets, load_dataset
+from datasets import concatenate_datasets, interleave_datasets, load_dataset
 
 from llmtuner.extras.logging import get_logger
-from llmtuner.hparams import ModelArguments, DataArguments
+
+if TYPE_CHECKING:
+    from datasets import Dataset
+    from llmtuner.hparams import ModelArguments, DataArguments
 
 
 logger = get_logger(__name__)
 
 
-def get_dataset(
-    model_args: ModelArguments,
-    data_args: DataArguments
-) -> Dataset:
-
-    def checksum(file_path, hash):
-        with open(file_path, "rb") as datafile:
-            binary_data = datafile.read()
-        sha1 = hashlib.sha1(binary_data).hexdigest()
-        if sha1 != hash:
-            logger.warning("Checksum failed for {}. It may vary depending on the platform.".format(file_path))
-
-    ext2type = {
-        "csv": "csv",
-        "json": "json",
-        "jsonl": "json",
-        "txt": "text"
-    }
+EXT2TYPE = {
+    "csv": "csv",
+    "json": "json",
+    "jsonl": "json",
+    "txt": "text"
+}
+
+
+def checksum(data_files: List[str], file_sha1: Optional[str] = None) -> None:
+    if file_sha1 is None:
+        logger.warning("Checksum failed: missing SHA-1 hash value in dataset_info.json.")
+        return
+
+    if len(data_files) != 1:
+        logger.warning("Checksum failed: too many files.")
+        return
+
+    with open(data_files[0], "rb") as f:
+        sha1 = hashlib.sha1(f.read()).hexdigest()
+        if sha1 != file_sha1:
+            logger.warning("Checksum failed: mismatched SHA-1 hash value at {}.".format(data_files[0]))
+
 
+def get_dataset(
+    model_args: "ModelArguments",
+    data_args: "DataArguments"
+) -> "Dataset":
     max_samples = data_args.max_samples
-    all_datasets: List[Dataset] = [] # support multiple datasets
+    all_datasets: List["Dataset"] = [] # support multiple datasets
 
     for dataset_attr in data_args.dataset_list:
-
         logger.info("Loading dataset {}...".format(dataset_attr))
 
         if dataset_attr.load_from == "hf_hub":
             data_path = dataset_attr.dataset_name
             data_files = None
         elif dataset_attr.load_from == "script":
             data_path = os.path.join(data_args.dataset_dir, dataset_attr.dataset_name)
             data_files = None
         elif dataset_attr.load_from == "file":
             data_path = None
             data_files: List[str] = []
 
-            if os.path.isdir(os.path.join(data_args.dataset_dir, dataset_attr.dataset_name)):
+            if os.path.isdir(os.path.join(data_args.dataset_dir, dataset_attr.dataset_name)): # directory
                 for file_name in os.listdir(os.path.join(data_args.dataset_dir, dataset_attr.dataset_name)):
                     data_files.append(os.path.join(data_args.dataset_dir, dataset_attr.dataset_name, file_name))
-
                     if data_path is None:
-                        data_path = ext2type.get(data_files[0].split(".")[-1], None)
+                        data_path = EXT2TYPE.get(file_name.split(".")[-1], None)
                     else:
-                        assert data_path == ext2type.get(data_files[-1].split(".")[-1], None), "file type does not match."
-            elif os.path.isfile(os.path.join(data_args.dataset_dir, dataset_attr.dataset_name)):
+                        assert data_path == EXT2TYPE.get(file_name.split(".")[-1], None), "file type does not match."
+            elif os.path.isfile(os.path.join(data_args.dataset_dir, dataset_attr.dataset_name)): # single file
                 data_files.append(os.path.join(data_args.dataset_dir, dataset_attr.dataset_name))
-                data_path = ext2type.get(data_files[0].split(".")[-1], None)
+                data_path = EXT2TYPE.get(dataset_attr.dataset_name.split(".")[-1], None)
             else:
                 raise ValueError("File not found.")
 
             assert data_path, "File extension must be txt, csv, json or jsonl."
-
-            if len(data_files) == 1 and dataset_attr.dataset_sha1 is not None:
-                checksum(data_files[0], dataset_attr.dataset_sha1)
-            else:
-                logger.warning("Checksum failed: missing SHA-1 hash value in dataset_info.json or too many files.")
+            checksum(data_files, dataset_attr.dataset_sha1)
         else:
             raise NotImplementedError
 
-        raw_datasets = load_dataset(
+        dataset = load_dataset(
             data_path,
             data_files=data_files,
+            split=data_args.split,
             cache_dir=model_args.cache_dir,
+            streaming=data_args.streaming,
             use_auth_token=True if model_args.use_auth_token else None
         )
-        dataset = raw_datasets[data_args.split]
 
         if max_samples is not None:
             max_samples_temp = min(len(dataset), max_samples)
             dataset = dataset.select(range(max_samples_temp))
 
-        dummy_data = [None] * len(dataset)
-        prefix_data = [dataset_attr.source_prefix] * len(dataset)
-        for column_name, target_name in [
-            ("prompt_column", "prompt"),
-            ("query_column", "query"),
-            ("response_column", "response"),
-            ("history_column", "history")
-        ]: # every dataset will have 4 columns same as each other
-            if getattr(dataset_attr, column_name) != target_name:
-                if getattr(dataset_attr, column_name):
-                    dataset = dataset.rename_column(getattr(dataset_attr, column_name), target_name)
-                else: # None or empty string
-                    dataset = dataset.add_column(target_name, dummy_data)
-        dataset = dataset.add_column("prefix", prefix_data)
+        for column_name in ["prompt", "query", "response", "history"]: # align datasets
+            if getattr(dataset_attr, column_name) and getattr(dataset_attr, column_name) != column_name:
+                dataset = dataset.rename_column(getattr(dataset_attr, column_name), column_name)
+
+        if dataset_attr.source_prefix: # add prefix
+            dataset = dataset.map(lambda _: {"prefix": dataset_attr.source_prefix})
+
         all_datasets.append(dataset)
 
     if len(data_args.dataset_list) == 1:
-        all_datasets = all_datasets[0]
+        return all_datasets[0]
+    elif data_args.mix_strategy == "concat":
+        if data_args.streaming:
+            logger.warning("The samples between different datasets will not be mixed in streaming mode.")
+        return concatenate_datasets(all_datasets)
+    elif data_args.mix_strategy.startswith("interleave"):
+        if not data_args.streaming:
+            logger.warning("We recommend using `mix_strategy=concat` in non-streaming mode.")
+        stopping_strategy = "first_exhausted" if data_args.mix_strategy.endswith("under") else "all_exhausted"
+        return interleave_datasets(all_datasets, stopping_strategy=stopping_strategy)
     else:
-        all_datasets = concatenate_datasets(all_datasets)
-
-    return all_datasets
+        raise ValueError("Unknown mixing strategy.")
```

### Comparing `llmtuner-0.1.3/src/llmtuner/dsets/utils.py` & `llmtuner-0.1.4/src/llmtuner/dsets/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from typing import Dict
-from datasets import Dataset
+from typing import TYPE_CHECKING, Dict
 
+if TYPE_CHECKING:
+    from datasets import Dataset
 
-def split_dataset(
-    dataset: Dataset, dev_ratio: float, do_train: bool
-) -> Dict[str, Dataset]:
-    # Split the dataset
+
+def split_dataset(dataset: "Dataset", dev_ratio: float, do_train: bool) -> Dict[str, "Dataset"]:
     if do_train:
-        if dev_ratio > 1e-6:
+        if dev_ratio > 1e-6: # Split the dataset
             dataset = dataset.train_test_split(test_size=dev_ratio)
             return {"train_dataset": dataset["train"], "eval_dataset": dataset["test"]}
         else:
             return {"train_dataset": dataset}
     else: # do_eval or do_predict
         return {"eval_dataset": dataset}
```

### Comparing `llmtuner-0.1.3/src/llmtuner/extras/callbacks.py` & `llmtuner-0.1.4/src/llmtuner/extras/callbacks.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,53 +1,50 @@
 import os
 import json
 import time
+from typing import TYPE_CHECKING
 from datetime import timedelta
 
-from transformers import (
-    TrainerCallback,
-    TrainerControl,
-    TrainerState,
-    TrainingArguments
-)
-from transformers.trainer_callback import TrainerControl, TrainerState
-from transformers.training_args import TrainingArguments
+from transformers import TrainerCallback
+
+if TYPE_CHECKING:
+    from transformers import TrainingArguments, TrainerState, TrainerControl
 
 
 class LogCallback(TrainerCallback):
 
     def __init__(self, runner=None):
         self.runner = runner
         self.start_time = time.time()
         self.tracker = {}
 
-    def on_train_begin(self, args: TrainingArguments, state: TrainerState, control: TrainerControl, **kwargs):
+    def on_train_begin(self, args: "TrainingArguments", state: "TrainerState", control: "TrainerControl", **kwargs):
         r"""
         Event called at the beginning of training.
         """
         self.start_time = time.time()
 
-    def on_step_begin(self, args: TrainingArguments, state: TrainerState, control: TrainerControl, **kwargs):
+    def on_step_begin(self, args: "TrainingArguments", state: "TrainerState", control: "TrainerControl", **kwargs):
         r"""
         Event called at the beginning of a training step. If using gradient accumulation, one training step
         might take several inputs.
         """
         if self.runner is not None and self.runner.aborted:
             control.should_epoch_stop = True
             control.should_training_stop = True
 
-    def on_substep_end(self, args: TrainingArguments, state: TrainerState, control: TrainerControl, **kwargs):
+    def on_substep_end(self, args: "TrainingArguments", state: "TrainerState", control: "TrainerControl", **kwargs):
         r"""
         Event called at the end of an substep during gradient accumulation.
         """
         if self.runner is not None and self.runner.aborted:
             control.should_epoch_stop = True
             control.should_training_stop = True
 
-    def on_log(self, args: TrainingArguments, state: TrainerState, control: TrainerControl, **kwargs) -> None:
+    def on_log(self, args: "TrainingArguments", state: "TrainerState", control: "TrainerControl", **kwargs) -> None:
         r"""
         Event called after logging the last logs.
         """
         if not state.is_world_process_zero:
             return
 
         cur_time = time.time()
```

### Comparing `llmtuner-0.1.3/src/llmtuner/extras/constants.py` & `llmtuner-0.1.4/src/llmtuner/extras/constants.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.3/src/llmtuner/extras/logging.py` & `llmtuner-0.1.4/src/llmtuner/extras/logging.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,16 +12,24 @@
         if record.name == "httpx":
             return
         log_entry = self.format(record)
         self.log += log_entry
         self.log += "\n\n"
 
 
-def get_logger(name: str) -> logging.Logger:
+def reset_logging():
+    r"""
+    Removes basic config of root logger
+    """
+    root = logging.getLogger()
+    list(map(root.removeHandler, root.handlers))
+    list(map(root.removeFilter, root.filters))
+
 
+def get_logger(name: str) -> logging.Logger:
     formatter = logging.Formatter(
         fmt="%(asctime)s - %(levelname)s - %(name)s - %(message)s",
         datefmt="%m/%d/%Y %H:%M:%S"
     )
     handler = logging.StreamHandler(sys.stdout)
     handler.setFormatter(formatter)
```

### Comparing `llmtuner-0.1.3/src/llmtuner/extras/misc.py` & `llmtuner-0.1.4/src/llmtuner/extras/misc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import torch
-from typing import List, Optional
+from typing import TYPE_CHECKING, List, Optional, Tuple
 
-from transformers.modeling_utils import PreTrainedModel
 from transformers.generation.utils import LogitsProcessorList
 from transformers.generation.logits_process import LogitsProcessor
 
 from llmtuner.extras.constants import LAYERNORM_NAMES
 
+if TYPE_CHECKING:
+    from transformers.modeling_utils import PreTrainedModel
+
 
 class AverageMeter:
     r"""
     Computes and stores the average and current value.
     """
     def __init__(self):
         self.reset()
@@ -24,15 +26,15 @@
     def update(self, val, n=1):
         self.val = val
         self.sum += val * n
         self.count += n
         self.avg = self.sum / self.count
 
 
-# Avoid runtime error in model.generate(do_sample=True).
+# Avoids runtime error in model.generate(do_sample=True).
 class InvalidScoreLogitsProcessor(LogitsProcessor):
 
     def __call__(self, input_ids: torch.LongTensor, scores: torch.FloatTensor) -> torch.FloatTensor:
         if torch.isnan(scores).any() or torch.isinf(scores).any():
             scores.zero_()
             scores[..., 0] = 1.0
         return scores
@@ -40,37 +42,45 @@
 
 def get_logits_processor() -> LogitsProcessorList:
     logits_processor = LogitsProcessorList()
     logits_processor.append(InvalidScoreLogitsProcessor())
     return logits_processor
 
 
-def print_trainable_params(model: torch.nn.Module) -> None:
+def count_parameters(model: torch.nn.Module) -> Tuple[int, int]:
+    r"""
+    Returns the number of trainable parameters and number of all parameters in the model.
+    """
     trainable_params, all_param = 0, 0
     for param in model.parameters():
         num_params = param.numel()
         # if using DS Zero 3 and the weights are initialized empty
         if num_params == 0 and hasattr(param, "ds_numel"):
             num_params = param.ds_numel
+
+        # Due to the design of 4bit linear layers from bitsandbytes, multiply the number of parameters by 2
+        if param.__class__.__name__ == "Params4bit":
+            num_params = num_params * 2
+
         all_param += num_params
         if param.requires_grad:
             trainable_params += num_params
-    print("trainable params: {:d} || all params: {:d} || trainable%: {:.4f}".format(
-                trainable_params, all_param, 100 * trainable_params / all_param))
+
+    return trainable_params, all_param
 
 
 # Includes: (1) cast the layernorm in fp32 (2) make output embedding layer require grads (3) upcast the lm_head to fp32
 # Inspired by: https://github.com/huggingface/peft/blob/c0209c35abbf88c63aa267800d98a8e212ed0a42/src/peft/utils/other.py#L35
 def prepare_model_for_training(
-    model: PreTrainedModel,
+    model: "PreTrainedModel",
     finetuning_type: str,
-    output_embedding_layer_name: Optional[str] = "lm_head",
+    output_layer_name: Optional[str] = "lm_head",
     use_gradient_checkpointing: Optional[bool] = True,
     layer_norm_names: Optional[List[str]] = LAYERNORM_NAMES
-) -> PreTrainedModel:
+) -> "PreTrainedModel":
 
     for name, param in model.named_parameters():
         if param.ndim == 1 and any(layer_norm_name in name for layer_norm_name in layer_norm_names):
             param.data = param.data.to(torch.float32)
 
     if use_gradient_checkpointing:
         if hasattr(model, "enable_input_require_grads"):
@@ -79,27 +89,31 @@
             def make_inputs_require_grad(module, input, output):
                 output.requires_grad_(True)
             model.get_input_embeddings().register_forward_hook(make_inputs_require_grad)
 
         model.gradient_checkpointing_enable()
         model.config.use_cache = False # turn off when gradient checkpointing is enabled
 
-    if finetuning_type != "full" and hasattr(model, output_embedding_layer_name):
-        output_embedding_layer: torch.nn.Linear = getattr(model, output_embedding_layer_name)
-        input_dtype = output_embedding_layer.weight.dtype
+    if finetuning_type != "full" and hasattr(model, output_layer_name):
+        if hasattr(model, "config") and hasattr(model.config, "pretraining_tp"):
+            model.config.pretraining_tp = 1 # disable TP for LoRA (https://github.com/huggingface/peft/pull/728)
+
+        output_layer: torch.nn.Linear = getattr(model, output_layer_name)
+        input_dtype = output_layer.weight.dtype
 
         class CastOutputToFloat(torch.nn.Sequential):
 
             def forward(self, x: torch.Tensor) -> torch.Tensor:
                 return super().forward(x.to(input_dtype)).to(torch.float32)
 
-        setattr(model, output_embedding_layer_name, CastOutputToFloat(output_embedding_layer))
+        setattr(model, output_layer_name, CastOutputToFloat(output_layer))
 
     return model
 
+
 def torch_gc() -> None:
     r"""
     Collects GPU memory.
     """
     if torch.cuda.is_available():
         torch.cuda.empty_cache()
         torch.cuda.ipc_collect()
```

### Comparing `llmtuner-0.1.3/src/llmtuner/extras/ploting.py` & `llmtuner-0.1.4/src/llmtuner/extras/ploting.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.3/src/llmtuner/extras/save_and_load.py` & `llmtuner-0.1.4/src/llmtuner/extras/save_and_load.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import os
 import torch
-from typing import Dict, Optional
+from typing import Dict
 
 from transformers.trainer import WEIGHTS_NAME, WEIGHTS_INDEX_NAME
 from transformers.modeling_utils import load_sharded_checkpoint
 
 from llmtuner.extras.constants import VALUE_HEAD_FILE_NAME
 from llmtuner.extras.logging import get_logger
 
 
 logger = get_logger(__name__)
 
 
-def get_state_dict(model: torch.nn.Module, trainable_only: Optional[bool] = True) -> Dict[str, torch.Tensor]:
-    state_dict = model.state_dict()
+def get_state_dict(model: torch.nn.Module) -> Dict[str, torch.Tensor]:
+    state_dict: Dict[str, torch.Tensor] = model.state_dict()
     filtered_state_dict = {}
 
     for k, v in model.named_parameters():
-        if (not trainable_only) or v.requires_grad:
+        if v.requires_grad:
             filtered_state_dict[k] = state_dict[k].cpu().clone().detach()
 
     return filtered_state_dict
 
 
 def load_trainable_params(model: torch.nn.Module, checkpoint_dir: os.PathLike) -> bool:
     weights_file = os.path.join(checkpoint_dir, WEIGHTS_NAME)
```

### Comparing `llmtuner-0.1.3/src/llmtuner/extras/template.py` & `llmtuner-0.1.4/src/llmtuner/extras/template.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,45 +7,54 @@
 
     prefix: str
     prompt: str
     sep: str
     use_history: bool
 
     def get_prompt(
-        self, query: str, history: Optional[List[Tuple[str, str]]] = None, prefix: Optional[str] = ""
+        self,
+        query: str,
+        history: Optional[List[Tuple[str, str]]] = None,
+        prefix: Optional[str] = "",
+        eos_token: Optional[str] = "</s>"
     ) -> str:
         r"""
         Returns a string containing prompt without response.
         """
-        return "".join(self._format_example(query, history, prefix))
+        return eos_token.join(map(lambda x: x[0] + x[1], self._format_example(query, history, prefix)))
 
     def get_dialog(
-        self, query: str, resp: str, history: Optional[List[Tuple[str, str]]] = None, prefix: Optional[str] = ""
-    ) -> List[str]:
+        self,
+        query: str,
+        resp: str,
+        history: Optional[List[Tuple[str, str]]] = None,
+        prefix: Optional[str] = ""
+    ) -> List[Tuple[str, str]]:
         r"""
-        Returns a list containing 2 * n elements where the 2k-th is a query and the (2k+1)-th is a response.
+        Returns a list containing prompt-response pairs.
         """
-        return self._format_example(query, history, prefix) + [resp]
+        result = self._format_example(query, history, prefix)
+        result[-1][-1] = resp
+        return result
 
     def _format_example(
-        self, query: str, history: Optional[List[Tuple[str, str]]] = None, prefix: Optional[str] = ""
-    ) -> List[str]:
+        self,
+        query: str,
+        history: Optional[List[Tuple[str, str]]] = None,
+        prefix: Optional[str] = ""
+    ) -> List[Tuple[str, str]]:
         prefix = prefix or self.prefix # use prefix if provided
         prefix = prefix + self.sep if prefix else "" # add separator for non-empty prefix
         history = history if (history and self.use_history) else []
-        history = history + [(query, "<dummy>")]
-        convs = []
-        for turn_idx, (user_query, bot_resp) in enumerate(history):
-            if turn_idx == 0:
-                convs.append(prefix + self.prompt.format(query=user_query))
-                convs.append(bot_resp)
-            else:
-                convs.append(self.sep + self.prompt.format(query=user_query))
-                convs.append(bot_resp)
-        return convs[:-1] # drop last
+        history = history + [(query, "")]
+        convs = [
+            [(self.sep if turn_idx else prefix) + self.prompt.format(query=query_i), resp_i]
+            for turn_idx, (query_i, resp_i) in enumerate(history)
+        ]
+        return convs
 
 
 templates: Dict[str, Template] = {}
 
 
 def register_template(name: str, prefix: str, prompt: str, sep: str, use_history: bool) -> None:
     templates[name] = Template(
@@ -99,15 +108,15 @@
            "Your answers should not include any harmful, unethical, "
            "racist, sexist, toxic, dangerous, or illegal content. "
            "Please ensure that your responses are socially unbiased and positive in nature.\n"
            "If a question does not make any sense, or is not factually coherent, "
            "explain why instead of answering something not correct. "
            "If you don't know the answer to a question, please don't share false information.\n<</SYS>>\n\n",
     prompt=" [INST] {query} [/INST] ",
-    sep="</s>",
+    sep="",
     use_history=True
 )
 
 
 r"""
 Supports: https://huggingface.co/tatsu-lab/alpaca-7b-wdiff
           https://github.com/ymcui/Chinese-LLaMA-Alpaca
@@ -127,15 +136,15 @@
           https://huggingface.co/lmsys/vicuna-13b-delta-v1.1
 """
 register_template(
     name="vicuna",
     prefix="A chat between a curious user and an artificial intelligence assistant. "
            "The assistant gives helpful, detailed, and polite answers to the user's questions.",
     prompt="USER: {query} ASSISTANT: ",
-    sep="</s>",
+    sep="",
     use_history=True
 )
 
 
 r"""
 Supports: https://huggingface.co/BelleGroup/BELLE-LLaMA-EXT-13B
 """
@@ -212,15 +221,15 @@
 r"""
 Supports: https://huggingface.co/baichuan-inc/Baichuan-13B-Chat
 """
 register_template(
     name="baichuan",
     prefix="",
     prompt="<reserved_102>{query}<reserved_103>",
-    sep="</s>",
+    sep="",
     use_history=True
 )
 
 
 r"""
 Supports: https://huggingface.co/HuggingFaceH4/starchat-alpha
           https://huggingface.co/HuggingFaceH4/starchat-beta
```

### Comparing `llmtuner-0.1.3/src/llmtuner/hparams/data_args.py` & `llmtuner-0.1.4/src/llmtuner/hparams/data_args.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import json
-from typing import List, Optional
+from typing import List, Literal, Optional
 from dataclasses import dataclass, field
 
 
 @dataclass
 class DatasetAttr:
 
     load_from: str
@@ -12,37 +12,52 @@
     dataset_sha1: Optional[str] = None
     source_prefix: Optional[str] = None
 
     def __repr__(self) -> str:
         return self.dataset_name
 
     def __post_init__(self):
-        self.prompt_column = "instruction"
-        self.query_column = "input"
-        self.response_column = "output"
-        self.history_column = None
+        self.prompt = "instruction"
+        self.query = "input"
+        self.response = "output"
+        self.history = None
 
 
 @dataclass
 class DataArguments:
     """
     Arguments pertaining to what data we are going to input our model for training and evaluation.
     """
+    template: str = field(
+        metadata={"help": "Which template to use for constructing prompts in training and inference."}
+    )
     dataset: Optional[str] = field(
-        default="alpaca_zh",
+        default="alpaca_en",
         metadata={"help": "The name of provided dataset(s) to use. Use commas to separate multiple datasets."}
     )
     dataset_dir: Optional[str] = field(
         default="data",
         metadata={"help": "The name of the folder containing datasets."}
     )
     split: Optional[str] = field(
         default="train",
         metadata={"help": "Which dataset split to use for training and evaluation."}
     )
+    streaming: Optional[bool] = field(
+        default=False,
+        metadata={"help": "Enable streaming mode."}
+    )
+    buffer_size: Optional[int] = field(
+        default=16384,
+        metadata={"help": "Size of the buffer to randomly sample examples from in streaming mode."}
+    )
+    mix_strategy: Optional[Literal["concat", "interleave_under", "interleave_over"]] = field(
+        default="concat",
+        metadata={"help": "Strategy to use in dataset mixing."}
+    )
     overwrite_cache: Optional[bool] = field(
         default=False,
         metadata={"help": "Overwrite the cached training and evaluation sets."}
     )
     preprocessing_num_workers: Optional[int] = field(
         default=None,
         metadata={"help": "The number of processes to use for the preprocessing."}
@@ -71,18 +86,14 @@
         default=None,
         metadata={"help": "A prefix to add before every source text. Use `|` to separate multiple prefixes in training."}
     )
     dev_ratio: Optional[float] = field(
         default=0,
         metadata={"help": "Proportion of the dataset to include in the development set, should be between 0.0 and 1.0."}
     )
-    prompt_template: Optional[str] = field(
-        default="default",
-        metadata={"help": "Which template to use for constructing prompts in training and inference."}
-    )
 
     def init_for_training(self): # support mixing multiple datasets
         dataset_names = [ds.strip() for ds in self.dataset.split(",")]
         with open(os.path.join(self.dataset_dir, "dataset_info.json"), "r") as f:
             dataset_info = json.load(f)
 
         if self.source_prefix is not None:
@@ -107,13 +118,13 @@
                     dataset_name=dataset_info[name]["file_name"],
                     dataset_sha1=dataset_info[name].get("file_sha1", None)
                 )
 
             dataset_attr.source_prefix = prefix_list[i]
 
             if "columns" in dataset_info[name]:
-                dataset_attr.prompt_column = dataset_info[name]["columns"].get("prompt", None)
-                dataset_attr.query_column = dataset_info[name]["columns"].get("query", None)
-                dataset_attr.response_column = dataset_info[name]["columns"].get("response", None)
-                dataset_attr.history_column = dataset_info[name]["columns"].get("history", None)
+                dataset_attr.prompt = dataset_info[name]["columns"].get("prompt", None)
+                dataset_attr.query = dataset_info[name]["columns"].get("query", None)
+                dataset_attr.response = dataset_info[name]["columns"].get("response", None)
+                dataset_attr.history = dataset_info[name]["columns"].get("history", None)
 
-            self.dataset_list.append(dataset_attr)
+            self.dataset_list.append(dataset_attr)
```

### Comparing `llmtuner-0.1.3/src/llmtuner/hparams/finetuning_args.py` & `llmtuner-0.1.4/src/llmtuner/hparams/finetuning_args.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.3/src/llmtuner/hparams/generating_args.py` & `llmtuner-0.1.4/src/llmtuner/hparams/generating_args.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.3/src/llmtuner/hparams/model_args.py` & `llmtuner-0.1.4/src/llmtuner/hparams/model_args.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.3/src/llmtuner/tuner/core/adapter.py` & `llmtuner-0.1.4/src/llmtuner/tuner/core/adapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 import os
 import torch
+from typing import TYPE_CHECKING
 
-from transformers.modeling_utils import PreTrainedModel
 from peft import (
     PeftModel,
     TaskType,
     LoraConfig,
     get_peft_model
 )
 from peft.utils import CONFIG_NAME, WEIGHTS_NAME
 
 from llmtuner.extras.logging import get_logger
 from llmtuner.extras.save_and_load import load_trainable_params
-from llmtuner.hparams import ModelArguments, FinetuningArguments
+
+if TYPE_CHECKING:
+    from transformers.modeling_utils import PreTrainedModel
+    from llmtuner.hparams import ModelArguments, FinetuningArguments
 
 
 logger = get_logger(__name__)
 
 
 def init_adapter(
-    model: PreTrainedModel,
-    model_args: ModelArguments,
-    finetuning_args: FinetuningArguments,
+    model: "PreTrainedModel",
+    model_args: "ModelArguments",
+    finetuning_args: "FinetuningArguments",
     is_trainable: bool,
     is_mergeable: bool
-) -> PreTrainedModel:
+) -> "PreTrainedModel":
     r"""
     Initializes the adapters.
 
     Support full-parameter, freeze and LoRA training.
 
     Note that the trainable parameters must be cast to float32.
     """
```

### Comparing `llmtuner-0.1.3/src/llmtuner/tuner/core/loader.py` & `llmtuner-0.1.4/src/llmtuner/tuner/core/loader.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,149 +1,158 @@
-import os
-import torch
-from typing import Literal, Optional, Tuple
-
-from transformers import (
-    AutoConfig,
-    AutoModelForCausalLM,
-    AutoTokenizer,
-    BitsAndBytesConfig
-)
-from transformers.utils import check_min_version
-from transformers.utils.versions import require_version
-from transformers.deepspeed import is_deepspeed_zero3_enabled
-from transformers.modeling_utils import PretrainedConfig, PreTrainedModel
-from transformers.tokenization_utils import PreTrainedTokenizerBase
-from trl import AutoModelForCausalLMWithValueHead
-
-from llmtuner.extras.logging import get_logger
-from llmtuner.extras.misc import prepare_model_for_training, print_trainable_params
-from llmtuner.extras.save_and_load import load_valuehead_params
-from llmtuner.hparams import ModelArguments, FinetuningArguments
-from llmtuner.tuner.core.adapter import init_adapter
-
-
-logger = get_logger(__name__)
-
-
-check_min_version("4.29.1")
-require_version("datasets>=2.12.0", "To fix: pip install datasets>=2.12.0")
-require_version("accelerate>=0.21.0", "To fix: pip install accelerate>=0.21.0")
-require_version("peft>=0.4.0", "To fix: pip install peft>=0.4.0")
-require_version("trl>=0.4.7", "To fix: pip install trl>=0.4.7")
-
-
-def load_model_and_tokenizer(
-    model_args: ModelArguments,
-    finetuning_args: FinetuningArguments,
-    is_trainable: Optional[bool] = False,
-    stage: Optional[Literal["pt", "sft", "rm", "ppo"]] = "sft"
-) -> Tuple[PreTrainedModel, PreTrainedTokenizerBase]:
-    r"""
-    Loads pretrained model and tokenizer.
-
-    Support both training and inference.
-    """
-    if (not is_trainable) and model_args.checkpoint_dir is None:
-        logger.warning("Checkpoint is not found at evaluation, load the original model.")
-        finetuning_args = FinetuningArguments(finetuning_type="none")
-
-    assert stage in ["pt", "sft"] or finetuning_args.finetuning_type == "lora", \
-        "RM and PPO training can only be performed with the LoRA method."
-
-    config_kwargs = {
-        "trust_remote_code": True,
-        "cache_dir": model_args.cache_dir,
-        "revision": model_args.model_revision,
-        "use_auth_token": True if model_args.use_auth_token else None,
-    }
-
-    tokenizer = AutoTokenizer.from_pretrained(
-        model_args.model_name_or_path,
-        use_fast=model_args.use_fast_tokenizer,
-        padding_side=model_args.padding_side,
-        **config_kwargs
-    )
-    if tokenizer.pad_token_id is None or tokenizer.pad_token_id == 64000: # 64000 for baichuan model (older version)
-        tokenizer.pad_token_id = 0 # set as the <unk> token
-
-    config = AutoConfig.from_pretrained(model_args.model_name_or_path, **config_kwargs)
-    is_mergeable = True
-
-    # Quantization configurations (using bitsandbytes library).
-    if model_args.quantization_bit is not None:
-        if model_args.quantization_bit == 8:
-            require_version("bitsandbytes>=0.37.0", "To fix: pip install bitsandbytes>=0.37.0")
-            config_kwargs["load_in_8bit"] = True
-            config_kwargs["quantization_config"] = BitsAndBytesConfig(
-                load_in_8bit=True,
-                llm_int8_threshold=6.0
-            )
-
-        elif model_args.quantization_bit == 4:
-            require_version("bitsandbytes>=0.39.0", "To fix: pip install bitsandbytes>=0.39.0")
-            config_kwargs["load_in_4bit"] = True
-            config_kwargs["quantization_config"] = BitsAndBytesConfig(
-                load_in_4bit=True,
-                bnb_4bit_compute_dtype=model_args.compute_dtype,
-                bnb_4bit_use_double_quant=model_args.double_quantization,
-                bnb_4bit_quant_type=model_args.quantization_type
-            )
-
-        is_mergeable = False
-        config_kwargs["device_map"] = {"": int(os.environ.get("LOCAL_RANK", "0"))}
-        logger.info("Quantizing model to {} bit.".format(model_args.quantization_bit))
-
-    if not is_trainable: # `device_map=auto` should be used for inference only
-        config_kwargs["device_map"] = "auto"
-
-    if model_args.checkpoint_dir is not None and finetuning_args.finetuning_type == "full":
-        model_to_load = model_args.checkpoint_dir[0]
-    else:
-        model_to_load = model_args.model_name_or_path
-
-    # Load and prepare pretrained models (without valuehead).
-    model = AutoModelForCausalLM.from_pretrained(
-        model_to_load,
-        config=config,
-        torch_dtype=torch.bfloat16 if model_args.compute_dtype == torch.bfloat16 else torch.float16,
-        low_cpu_mem_usage=(not is_deepspeed_zero3_enabled()),
-        **config_kwargs
-    )
-
-    # Register auto class to save the custom code files.
-    if isinstance(config, PretrainedConfig) and "AutoConfig" in getattr(config, "auto_map", {}):
-        config.__class__.register_for_auto_class()
-    if isinstance(model, PreTrainedModel) and "AutoModelForCausalLM" in getattr(config, "auto_map", {}):
-        model.__class__.register_for_auto_class()
-    if isinstance(tokenizer, PreTrainedTokenizerBase) and "AutoTokenizer" in tokenizer.init_kwargs.get("auto_map", {}):
-        tokenizer.__class__.register_for_auto_class()
-
-    # Initialize adapters
-    model = prepare_model_for_training(model, finetuning_args.finetuning_type) if is_trainable else model
-    model = init_adapter(model, model_args, finetuning_args, is_trainable, is_mergeable)
-
-    if stage == "rm" or stage == "ppo": # add value head
-        model = AutoModelForCausalLMWithValueHead.from_pretrained(model)
-
-        if stage == "rm" and model_args.checkpoint_dir is not None: # load valuehead weights to evaluate reward model
-            logger.warning("Only the last checkpoint containing valuehead will be loaded as the valuehead.")
-            if load_valuehead_params(model, model_args.checkpoint_dir[-1]):
-                model.v_head.load_state_dict({
-                    "summary.weight": getattr(model, "reward_head_weight"),
-                    "summary.bias": getattr(model, "reward_head_bias")
-                })
-
-        if stage == "ppo": # load reward model
-            assert is_trainable, "PPO stage cannot be performed at evaluation."
-            assert model_args.reward_model is not None, "Reward model is necessary for PPO training."
-            logger.info("Load reward model from {}".format(model_args.reward_model))
-            model.pretrained_model.load_adapter(model_args.reward_model, "reward", is_trainable=False)
-            assert load_valuehead_params(model, model_args.reward_model), "Reward model is not correctly loaded."
-
-    if not is_trainable:
-        model.requires_grad_(False) # fix all model params
-        model = model.half() if model_args.quantization_bit is None else model # cast from fp32 to fp16
-
-    print_trainable_params(model)
-
-    return model, tokenizer
+import os
+import torch
+from typing import TYPE_CHECKING, Literal, Optional, Tuple
+
+from transformers import (
+    AutoConfig,
+    AutoModelForCausalLM,
+    AutoTokenizer,
+    BitsAndBytesConfig
+)
+from transformers.utils import check_min_version
+from transformers.utils.versions import require_version
+from transformers.deepspeed import is_deepspeed_zero3_enabled
+from transformers.modeling_utils import PretrainedConfig, PreTrainedModel
+from transformers.tokenization_utils import PreTrainedTokenizerBase
+from trl import AutoModelForCausalLMWithValueHead
+
+from llmtuner.extras.logging import reset_logging, get_logger
+from llmtuner.extras.misc import count_parameters, prepare_model_for_training
+from llmtuner.extras.save_and_load import load_valuehead_params
+from llmtuner.hparams import FinetuningArguments
+from llmtuner.tuner.core.adapter import init_adapter
+
+if TYPE_CHECKING:
+    from llmtuner.hparams import ModelArguments
+
+
+logger = get_logger(__name__)
+
+
+check_min_version("4.29.1")
+require_version("datasets>=2.12.0", "To fix: pip install datasets>=2.12.0")
+require_version("accelerate>=0.21.0", "To fix: pip install accelerate>=0.21.0")
+require_version("peft>=0.4.0", "To fix: pip install peft>=0.4.0")
+require_version("trl>=0.4.7", "To fix: pip install trl>=0.4.7")
+
+
+def load_model_and_tokenizer(
+    model_args: "ModelArguments",
+    finetuning_args: "FinetuningArguments",
+    is_trainable: Optional[bool] = False,
+    stage: Optional[Literal["pt", "sft", "rm", "ppo"]] = "sft"
+) -> Tuple[PreTrainedModel, PreTrainedTokenizerBase]:
+    r"""
+    Loads pretrained model and tokenizer.
+
+    Support both training and inference.
+    """
+    if (not is_trainable) and model_args.checkpoint_dir is None:
+        logger.warning("Checkpoint is not found at evaluation, load the original model.")
+        finetuning_args = FinetuningArguments(finetuning_type="none")
+
+    assert stage in ["pt", "sft"] or finetuning_args.finetuning_type == "lora", \
+        "RM and PPO training can only be performed with the LoRA method."
+
+    config_kwargs = {
+        "trust_remote_code": True,
+        "cache_dir": model_args.cache_dir,
+        "revision": model_args.model_revision,
+        "use_auth_token": True if model_args.use_auth_token else None,
+    }
+
+    tokenizer = AutoTokenizer.from_pretrained(
+        model_args.model_name_or_path,
+        use_fast=model_args.use_fast_tokenizer,
+        padding_side=model_args.padding_side,
+        **config_kwargs
+    )
+    if tokenizer.pad_token_id is None or tokenizer.pad_token_id == 64000: # 64000 for baichuan model (older version)
+        tokenizer.pad_token_id = 0 # set as the <unk> token
+
+    config = AutoConfig.from_pretrained(model_args.model_name_or_path, **config_kwargs)
+    is_mergeable = True
+
+    # Quantization configurations (using bitsandbytes library).
+    if model_args.quantization_bit is not None:
+        if model_args.quantization_bit == 8:
+            require_version("bitsandbytes>=0.37.0", "To fix: pip install bitsandbytes>=0.37.0")
+            config_kwargs["load_in_8bit"] = True
+            config_kwargs["quantization_config"] = BitsAndBytesConfig(
+                load_in_8bit=True,
+                llm_int8_threshold=6.0
+            )
+
+        elif model_args.quantization_bit == 4:
+            require_version("bitsandbytes>=0.39.0", "To fix: pip install bitsandbytes>=0.39.0")
+            config_kwargs["load_in_4bit"] = True
+            config_kwargs["quantization_config"] = BitsAndBytesConfig(
+                load_in_4bit=True,
+                bnb_4bit_compute_dtype=model_args.compute_dtype,
+                bnb_4bit_use_double_quant=model_args.double_quantization,
+                bnb_4bit_quant_type=model_args.quantization_type
+            )
+
+        is_mergeable = False
+        logger.info("Quantizing model to {} bit.".format(model_args.quantization_bit))
+
+    if (
+        model_args.quantization_bit is not None
+        or (os.environ.get('LOCAL_RANK') is not None and not is_deepspeed_zero3_enabled())
+    ):
+        config_kwargs["device_map"] = {"": int(os.environ.get("LOCAL_RANK", "0"))}
+
+    if model_args.checkpoint_dir is not None and finetuning_args.finetuning_type == "full":
+        model_to_load = model_args.checkpoint_dir[0]
+    else:
+        model_to_load = model_args.model_name_or_path
+
+    # Load and prepare pretrained models (without valuehead).
+    model = AutoModelForCausalLM.from_pretrained(
+        model_to_load,
+        config=config,
+        torch_dtype=torch.bfloat16 if model_args.compute_dtype == torch.bfloat16 else torch.float16,
+        low_cpu_mem_usage=(not is_deepspeed_zero3_enabled()),
+        **config_kwargs
+    )
+
+    # Register auto class to save the custom code files.
+    if isinstance(config, PretrainedConfig) and "AutoConfig" in getattr(config, "auto_map", {}):
+        config.__class__.register_for_auto_class()
+    if isinstance(model, PreTrainedModel) and "AutoModelForCausalLM" in getattr(config, "auto_map", {}):
+        model.__class__.register_for_auto_class()
+    if isinstance(tokenizer, PreTrainedTokenizerBase) and "AutoTokenizer" in tokenizer.init_kwargs.get("auto_map", {}):
+        tokenizer.__class__.register_for_auto_class()
+
+    # Initialize adapters
+    model = prepare_model_for_training(model, finetuning_args.finetuning_type) if is_trainable else model
+    model = init_adapter(model, model_args, finetuning_args, is_trainable, is_mergeable)
+
+    if stage == "rm" or stage == "ppo": # add value head
+        model = AutoModelForCausalLMWithValueHead.from_pretrained(model)
+        reset_logging()
+
+        if stage == "rm" and model_args.checkpoint_dir is not None: # load valuehead weights to evaluate reward model
+            logger.warning("Only the last checkpoint containing valuehead will be loaded as the valuehead.")
+            if load_valuehead_params(model, model_args.checkpoint_dir[-1]):
+                model.v_head.load_state_dict({
+                    "summary.weight": getattr(model, "reward_head_weight"),
+                    "summary.bias": getattr(model, "reward_head_bias")
+                })
+
+        if stage == "ppo": # load reward model
+            assert is_trainable, "PPO stage cannot be performed at evaluation."
+            assert model_args.reward_model is not None, "Reward model is necessary for PPO training."
+            logger.info("Load reward model from {}".format(model_args.reward_model))
+            model.pretrained_model.load_adapter(model_args.reward_model, "reward", is_trainable=False)
+            assert load_valuehead_params(model, model_args.reward_model), "Reward model is not correctly loaded."
+
+    if not is_trainable:
+        model.requires_grad_(False) # fix all model params
+        model = model.half() if model_args.quantization_bit is None else model # cast from fp32 to fp16
+
+    trainable_params, all_param = count_parameters(model)
+    logger.info("trainable params: {:d} || all params: {:d} || trainable%: {:.4f}".format(
+        trainable_params, all_param, 100 * trainable_params / all_param
+    ))
+
+    return model, tokenizer
```

### Comparing `llmtuner-0.1.3/src/llmtuner/tuner/core/parser.py` & `llmtuner-0.1.4/src/llmtuner/tuner/core/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,28 +15,47 @@
     GeneralArguments
 )
 
 
 logger = get_logger(__name__)
 
 
-def get_train_args(
-    args: Optional[Dict[str, Any]] = None
-) -> Tuple[ModelArguments, DataArguments, Seq2SeqTrainingArguments, FinetuningArguments, GeneralArguments]:
-
-    parser = HfArgumentParser((ModelArguments, DataArguments, Seq2SeqTrainingArguments, FinetuningArguments, GeneralArguments))
-
+def _parse_args(parser: HfArgumentParser, args: Optional[Dict[str, Any]] = None):
     if args is not None:
-        model_args, data_args, training_args, finetuning_args, general_args = parser.parse_dict(args)
+        return parser.parse_dict(args)
     elif len(sys.argv) == 2 and sys.argv[1].endswith(".yaml"):
-        model_args, data_args, training_args, finetuning_args, general_args = parser.parse_yaml_file(os.path.abspath(sys.argv[1]))
+        return parser.parse_yaml_file(os.path.abspath(sys.argv[1]))
     elif len(sys.argv) == 2 and sys.argv[1].endswith(".json"):
-        model_args, data_args, training_args, finetuning_args, general_args = parser.parse_json_file(os.path.abspath(sys.argv[1]))
+        return parser.parse_json_file(os.path.abspath(sys.argv[1]))
     else:
-        model_args, data_args, training_args, finetuning_args, general_args = parser.parse_args_into_dataclasses()
+        return parser.parse_args_into_dataclasses()
+
+
+def parse_train_args(
+    args: Optional[Dict[str, Any]] = None
+) -> Tuple[ModelArguments, DataArguments, Seq2SeqTrainingArguments, FinetuningArguments, GeneralArguments]:
+    parser = HfArgumentParser((
+        ModelArguments, DataArguments, Seq2SeqTrainingArguments, FinetuningArguments, GeneralArguments
+    ))
+    return _parse_args(parser, args)
+
+
+def parse_infer_args(
+    args: Optional[Dict[str, Any]] = None
+) -> Tuple[ModelArguments, DataArguments, FinetuningArguments, GeneratingArguments]:
+    parser = HfArgumentParser((
+        ModelArguments, DataArguments, FinetuningArguments, GeneratingArguments
+    ))
+    return _parse_args(parser, args)
+
+
+def get_train_args(
+    args: Optional[Dict[str, Any]] = None
+) -> Tuple[ModelArguments, DataArguments, Seq2SeqTrainingArguments, FinetuningArguments, GeneralArguments]:
+    model_args, data_args, training_args, finetuning_args, general_args = parse_train_args(args)
 
     # Setup logging
     if training_args.should_log:
         # The default of training_args.log_level is passive, so we set log level at info here to have that default.
         transformers.utils.logging.set_verbosity_info()
 
     log_level = training_args.get_process_log_level()
@@ -56,79 +75,84 @@
 
     assert general_args.stage != "sft" or (not training_args.do_predict) or training_args.predict_with_generate, \
         "Please enable `predict_with_generate` to save model predictions."
 
     assert model_args.quantization_bit is None or finetuning_args.finetuning_type == "lora", \
         "Quantization is only compatible with the LoRA method."
 
+    assert not (training_args.max_steps == -1 and data_args.streaming), \
+        "Please specify `max_steps` in streaming mode."
+
+    assert training_args.evaluation_strategy == "no" or (not data_args.streaming), \
+        "Streaming mode does not support evaluation currently."
+
+    assert not (general_args.stage == "ppo" and data_args.streaming), \
+        "Streaming mode does not suppport PPO training currently."
+
     if model_args.checkpoint_dir is not None:
         if finetuning_args.finetuning_type != "lora":
             assert len(model_args.checkpoint_dir) == 1, "Only LoRA tuning accepts multiple checkpoints."
         else:
             assert model_args.quantization_bit is None or len(model_args.checkpoint_dir) == 1, \
                 "Quantized model only accepts a single checkpoint."
 
     if model_args.quantization_bit is not None and (not training_args.do_train):
         logger.warning("Evaluating model in 4/8-bit mode may cause lower scores.")
 
     if training_args.do_train and (not training_args.fp16):
         logger.warning("We recommend enable fp16 mixed precision training.")
 
-    if data_args.prompt_template == "default":
-        logger.warning("Please specify `prompt_template` if you are using other pre-trained models.")
-
-    if training_args.local_rank != -1 and training_args.ddp_find_unused_parameters is None:
-        logger.warning("`ddp_find_unused_parameters` needs to be set as False in DDP training.")
+    if (
+        training_args.local_rank != -1
+        and training_args.ddp_find_unused_parameters is None
+        and finetuning_args.finetuning_type == "lora"
+    ):
+        logger.warning("`ddp_find_unused_parameters` needs to be set as False for LoRA in DDP training.")
         training_args.ddp_find_unused_parameters = False
 
+    if data_args.max_samples is not None and data_args.streaming:
+        logger.warning("`max_samples` is incompatible with `streaming`. Disabling max_samples.")
+        data_args.max_samples = None
+
+    if data_args.dev_ratio > 1e-6 and data_args.streaming:
+        logger.warning("`dev_ratio` is incompatible with `streaming`. Disabling development set.")
+        data_args.dev_ratio = 0
+
     training_args.optim = "adamw_torch" if training_args.optim == "adamw_hf" else training_args.optim # suppress warning
 
     if model_args.quantization_bit is not None:
         if training_args.fp16:
             model_args.compute_dtype = torch.float16
         elif training_args.bf16:
             model_args.compute_dtype = torch.bfloat16
         else:
             model_args.compute_dtype = torch.float32
 
     # Log on each process the small summary:
-    logger.info(
-        f"Process rank: {training_args.local_rank}, device: {training_args.device}, n_gpu: {training_args.n_gpu}\n"
-        + f"  distributed training: {bool(training_args.local_rank != -1)}, 16-bits training: {training_args.fp16}"
-    )
+    logger.info("Process rank: {}, device: {}, n_gpu: {}\n  distributed training: {}, 16-bits training: {}".format(
+        training_args.local_rank, training_args.device, training_args.n_gpu,
+        bool(training_args.local_rank != -1), training_args.fp16
+    ))
     logger.info(f"Training/evaluation parameters {training_args}")
 
     # Set seed before initializing model.
     transformers.set_seed(training_args.seed)
 
     return model_args, data_args, training_args, finetuning_args, general_args
 
 
 def get_infer_args(
     args: Optional[Dict[str, Any]] = None
 ) -> Tuple[ModelArguments, DataArguments, FinetuningArguments, GeneratingArguments]:
-
-    parser = HfArgumentParser((ModelArguments, DataArguments, FinetuningArguments, GeneratingArguments))
-
-    if args is not None:
-        model_args, data_args, finetuning_args, generating_args = parser.parse_dict(args)
-    elif len(sys.argv) == 2 and sys.argv[1].endswith(".yaml"):
-        model_args, data_args, finetuning_args, generating_args = parser.parse_yaml_file(os.path.abspath(sys.argv[1]))
-    elif len(sys.argv) == 2 and sys.argv[1].endswith(".json"):
-        model_args, data_args, finetuning_args, generating_args = parser.parse_json_file(os.path.abspath(sys.argv[1]))
-    else:
-        model_args, data_args, finetuning_args, generating_args = parser.parse_args_into_dataclasses()
+    model_args, data_args, finetuning_args, generating_args = parse_infer_args(args)
 
     assert model_args.quantization_bit is None or finetuning_args.finetuning_type == "lora", \
         "Quantization is only compatible with the LoRA method."
 
     if model_args.checkpoint_dir is not None:
         if finetuning_args.finetuning_type != "lora":
             assert len(model_args.checkpoint_dir) == 1, "Only LoRA tuning accepts multiple checkpoints."
         else:
             assert model_args.quantization_bit is None or len(model_args.checkpoint_dir) == 1, \
                 "Quantized model only accepts a single checkpoint."
 
-    if data_args.prompt_template == "default":
-        logger.warning("Please specify `prompt_template` if you are using other pre-trained models.")
-
     return model_args, data_args, finetuning_args, generating_args
```

### Comparing `llmtuner-0.1.3/src/llmtuner/tuner/core/trainer.py` & `llmtuner-0.1.4/src/llmtuner/tuner/core/trainer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 import os
 import torch
-from typing import Dict, Optional
+from typing import TYPE_CHECKING, Dict, Optional
 
 from transformers import Seq2SeqTrainer
-from transformers.trainer import TRAINING_ARGS_NAME
+from transformers.trainer import TRAINING_ARGS_NAME, WEIGHTS_NAME
 from transformers.modeling_utils import PreTrainedModel, unwrap_model
 from peft import PeftModel
+from trl import PreTrainedModelWrapper
 
 from llmtuner.extras.constants import FINETUNING_ARGS_NAME, VALUE_HEAD_FILE_NAME
 from llmtuner.extras.logging import get_logger
-from llmtuner.extras.save_and_load import get_state_dict, load_trainable_params, load_valuehead_params
-from llmtuner.hparams import FinetuningArguments
+from llmtuner.extras.save_and_load import get_state_dict, load_trainable_params
+
+if TYPE_CHECKING:
+    from llmtuner.hparams import FinetuningArguments
 
 
 logger = get_logger(__name__)
 
 
 class PeftTrainer(Seq2SeqTrainer):
     r"""
     Inherits Seq2SeqTrainer to support parameter-efficient checkpoints.
     """
 
-    def __init__(self, finetuning_args: FinetuningArguments, **kwargs):
+    def __init__(self, finetuning_args: "FinetuningArguments", **kwargs):
         super().__init__(**kwargs)
         self.finetuning_args = finetuning_args
         self._remove_log()
 
     def _remove_log(self):
         if self.is_world_process_zero() and os.path.exists(os.path.join(self.args.output_dir, "trainer_log.jsonl")):
             logger.warning("Previous log file in this folder will be deleted.")
@@ -38,54 +41,56 @@
         This function will only be executed at the process zero.
 
         Subclass and override to inject custom behavior. It should not be directly used by external scripts.
         """
         output_dir = output_dir if output_dir is not None else self.args.output_dir
         os.makedirs(output_dir, exist_ok=True)
         logger.info(f"Saving model checkpoint to {output_dir}")
+
         model = unwrap_model(self.model)
 
-        if hasattr(model, "pretrained_model"): # for models with valuehead (currently using LoRA only)
-            backbone_model = getattr(model, "pretrained_model")
-            torch.save(get_state_dict(getattr(model, "v_head")), os.path.join(output_dir, VALUE_HEAD_FILE_NAME))
+        if isinstance(model, PreTrainedModelWrapper):
+            # Custom state dict: https://github.com/lvwerra/trl/blob/v0.4.7/trl/models/modeling_value_head.py#L200
+            model_state_dict = state_dict or model.state_dict()
+            v_head_state_dict = {
+                name.replace("v_head.", ""): model_state_dict[name].cpu().clone().detach()
+                for name in model_state_dict.keys() if name.startswith("v_head.")
+            }
+
+            torch.save(v_head_state_dict, os.path.join(output_dir, VALUE_HEAD_FILE_NAME))
+            model = model.pretrained_model
+
+        state_dict = state_dict or get_state_dict(model)
+        if isinstance(model, (PeftModel, PreTrainedModel)):
+            model.config.use_cache = True
+            model.save_pretrained(output_dir, state_dict=state_dict, safe_serialization=self.args.save_safetensors)
+            model.config.use_cache = False
         else:
-            backbone_model = model
+            torch.save(state_dict, os.path.join(output_dir, WEIGHTS_NAME))
 
-        if isinstance(backbone_model, PeftModel): # LoRA tuning
-            backbone_model.save_pretrained(output_dir, state_dict=get_state_dict(backbone_model))
-        elif isinstance(backbone_model, PreTrainedModel): # freeze/full tuning
-            backbone_model.config.use_cache = True
-            backbone_model.save_pretrained(
-                output_dir,
-                state_dict=get_state_dict(backbone_model, trainable_only=(self.finetuning_args.finetuning_type != "full")),
-                safe_serialization=self.args.save_safetensors
-            )
-            backbone_model.config.use_cache = False
-            if self.tokenizer is not None:
-                self.tokenizer.save_pretrained(output_dir)
-        else:
-            logger.warning("No model to save.")
+        if self.finetuning_args.finetuning_type == "full" and self.tokenizer is not None:
+            self.tokenizer.save_pretrained(output_dir)
 
         with open(os.path.join(output_dir, TRAINING_ARGS_NAME), "w", encoding="utf-8") as f:
             f.write(self.args.to_json_string() + "\n")
+
         self.finetuning_args.save_to_json(os.path.join(output_dir, FINETUNING_ARGS_NAME))
 
     def _load_best_model(self):
         r"""
         Loads trainable parameters from model checkpoint.
 
         Subclass and override to inject custom behavior. It should not be directly used by external scripts.
         """
         logger.info(f"Loading best model from {self.state.best_model_checkpoint} (score: {self.state.best_metric}).")
-
         model = unwrap_model(self.model)
-        backbone_model = getattr(model, "pretrained_model") if hasattr(model, "pretrained_model") else model
 
-        if isinstance(backbone_model, PeftModel):
-            backbone_model.load_adapter(self.state.best_model_checkpoint, backbone_model.active_adapter)
-            if hasattr(model, "v_head") and load_valuehead_params(model, self.state.best_model_checkpoint):
-                model.v_head.load_state_dict({
-                    "summary.weight": getattr(model, "reward_head_weight"),
-                    "summary.bias": getattr(model, "reward_head_bias")
-                })
+        if isinstance(model, PreTrainedModelWrapper):
+            model.v_head.load_state_dict(torch.load(
+                os.path.join(self.state.best_model_checkpoint, VALUE_HEAD_FILE_NAME), map_location="cpu"
+            ))
+            model = model.pretrained_model
+
+        if isinstance(model, PeftModel):
+            model.load_adapter(self.state.best_model_checkpoint, model.active_adapter)
         else: # freeze/full-tuning
-            load_trainable_params(backbone_model, self.state.best_model_checkpoint)
+            load_trainable_params(model, self.state.best_model_checkpoint)
```

### Comparing `llmtuner-0.1.3/src/llmtuner/tuner/ppo/trainer.py` & `llmtuner-0.1.4/src/llmtuner/tuner/ppo/trainer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 import os
 import math
 import torch
 from tqdm import tqdm
-from typing import Callable, Dict, List, Optional
+from typing import TYPE_CHECKING, Callable, Dict, List, Optional
 
-from transformers import Seq2SeqTrainingArguments, TrainerState, TrainerControl
+from transformers import TrainerState, TrainerControl
 from transformers.modeling_utils import PreTrainedModel
 
 from trl import PPOTrainer
 from trl.core import LengthSampler
 
-from llmtuner.extras.callbacks import LogCallback
 from llmtuner.extras.logging import get_logger
-from llmtuner.extras.misc import AverageMeter, get_logits_processor
-from llmtuner.hparams import FinetuningArguments
+from llmtuner.extras.misc import AverageMeter, count_parameters, get_logits_processor
+
 from llmtuner.tuner.core.trainer import PeftTrainer
 from llmtuner.tuner.ppo.utils import cast_layernorm_dtype, replace_model
 
+if TYPE_CHECKING:
+    from transformers import Seq2SeqTrainingArguments
+    from llmtuner.extras.callbacks import LogCallback
+    from llmtuner.hparams import FinetuningArguments
+
 
 logger = get_logger(__name__)
 
 
 class PPOPeftTrainer(PPOTrainer, PeftTrainer):
     r"""
     Inherits PPOTrainer.
     """
+
     def __init__(
         self,
-        training_args: Seq2SeqTrainingArguments,
-        finetuning_args: FinetuningArguments,
-        callbacks: List[LogCallback],
+        training_args: "Seq2SeqTrainingArguments",
+        finetuning_args: "FinetuningArguments",
+        callbacks: List["LogCallback"],
         **kwargs
     ):
         PPOTrainer.__init__(self, **kwargs)
         self.args = training_args
         self.finetuning_args = finetuning_args
         self.log_callback = callbacks[0]
         self.state = TrainerState()
@@ -62,15 +67,15 @@
             logger.info("***** Running training *****")
             logger.info(f"  Num examples = {num_examples}")
             logger.info(f"  Num Epochs = {num_train_epochs}")
             logger.info(f"  Instantaneous batch size per device = {self.args.per_device_train_batch_size}")
             logger.info(f"  Total train batch size (w. parallel, distributed & accumulation) = {total_train_batch_size}")
             logger.info(f"  Gradient Accumulation steps = {self.args.gradient_accumulation_steps}")
             logger.info(f"  Total optimization steps = {max_steps}")
-            logger.info(f"  Number of trainable parameters = {sum(p.numel() for p in self.model.parameters() if p.requires_grad)}")
+            logger.info(f"  Number of trainable parameters = {count_parameters(self.model)[0]}")
 
         # Keyword arguments for `model.generate`
         gen_kwargs = {
             "top_k": 0.0,
             "top_p": 1.0,
             "do_sample": True,
             "pad_token_id": self.tokenizer.pad_token_id,
```

### Comparing `llmtuner-0.1.3/src/llmtuner/tuner/ppo/utils.py` & `llmtuner-0.1.4/src/llmtuner/tuner/ppo/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 import torch
-from typing import Dict, List, Literal, Optional, Tuple
-from trl import AutoModelForCausalLMWithValueHead
+from typing import TYPE_CHECKING, Dict, List, Literal, Optional, Tuple
 
 from llmtuner.extras.constants import LAYERNORM_NAMES
 
+if TYPE_CHECKING:
+    from trl import AutoModelForCausalLMWithValueHead
 
-def replace_model(model: AutoModelForCausalLMWithValueHead, target: Literal["default", "reward"]) -> None:
+
+def replace_model(model: "AutoModelForCausalLMWithValueHead", target: Literal["default", "reward"]) -> None:
     if target == "reward": # save default head temporarily
         valuehead_state_dict = model.v_head.state_dict()
         setattr(model, "default_head_weight", valuehead_state_dict["summary.weight"])
         setattr(model, "default_head_bias", valuehead_state_dict["summary.bias"])
 
     model.pretrained_model.set_adapter(target) # set the LoRA adapter to be active
     model.v_head.load_state_dict({
         "summary.weight": getattr(model, "{}_head_weight".format(target)),
         "summary.bias": getattr(model, "{}_head_bias".format(target))
     })
 
 
 def cast_layernorm_dtype(
-    model: AutoModelForCausalLMWithValueHead,
+    model: "AutoModelForCausalLMWithValueHead",
     layer_norm_names: List[str] = LAYERNORM_NAMES,
     layer_norm_params: Optional[Dict[str, torch.Tensor]] = None
-) -> Tuple[AutoModelForCausalLMWithValueHead, Dict[str, torch.Tensor]]:
+) -> Tuple["AutoModelForCausalLMWithValueHead", Dict[str, torch.Tensor]]:
 
     layer_norm_state_dict = {}
 
     for name, param in model.named_parameters():
         if param.ndim == 1 and any(layer_norm_name in name for layer_norm_name in layer_norm_names):
             if layer_norm_params is not None:
                 param.data = layer_norm_params[name] # restore float32 weights
```

### Comparing `llmtuner-0.1.3/src/llmtuner/tuner/ppo/workflow.py` & `llmtuner-0.1.4/src/llmtuner/tuner/ppo/workflow.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 # Inspired by:
 # https://github.com/lvwerra/trl/blob/main/examples/sentiment/scripts/gpt-neox-20b_peft/gpt-neo-20b_sentiment_peft.py
 
 import math
+from typing import TYPE_CHECKING
 from trl import PPOConfig
 from torch.optim import AdamW
 from typing import Optional, List
-from transformers import DataCollatorForSeq2Seq, Seq2SeqTrainingArguments, TrainerCallback
+from transformers import DataCollatorForSeq2Seq
 from transformers.optimization import get_scheduler
 
 from llmtuner.dsets import get_dataset, preprocess_dataset
 from llmtuner.extras.callbacks import LogCallback
 from llmtuner.extras.ploting import plot_loss
-from llmtuner.hparams import ModelArguments, DataArguments, FinetuningArguments
 from llmtuner.tuner.core import load_model_and_tokenizer
 from llmtuner.tuner.ppo.trainer import PPOPeftTrainer
 
+if TYPE_CHECKING:
+    from transformers import Seq2SeqTrainingArguments, TrainerCallback
+    from llmtuner.hparams import ModelArguments, DataArguments, FinetuningArguments
+
 
 def run_ppo(
-    model_args: ModelArguments,
-    data_args: DataArguments,
-    training_args: Seq2SeqTrainingArguments,
-    finetuning_args: FinetuningArguments,
-    callbacks: Optional[List[TrainerCallback]] = [LogCallback()]
+    model_args: "ModelArguments",
+    data_args: "DataArguments",
+    training_args: "Seq2SeqTrainingArguments",
+    finetuning_args: "FinetuningArguments",
+    callbacks: Optional[List["TrainerCallback"]] = [LogCallback()]
 ):
     dataset = get_dataset(model_args, data_args)
     model, tokenizer = load_model_and_tokenizer(model_args, finetuning_args, training_args.do_train, stage="ppo")
     dataset = preprocess_dataset(dataset, tokenizer, data_args, training_args, stage="ppo")
     data_collator = DataCollatorForSeq2Seq(tokenizer=tokenizer, label_pad_token_id=tokenizer.pad_token_id)
 
     ppo_config = PPOConfig(
```

### Comparing `llmtuner-0.1.3/src/llmtuner/tuner/pt/workflow.py` & `llmtuner-0.1.4/src/llmtuner/tuner/sft/workflow.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,87 @@
-# Inspired by: https://github.com/huggingface/transformers/blob/v4.29.2/examples/pytorch/language-modeling/run_clm.py
+# Inspired by: https://github.com/huggingface/transformers/blob/v4.29.2/examples/pytorch/summarization/run_summarization.py
 
-import math
-from typing import Optional, List
-from transformers import Seq2SeqTrainingArguments, DataCollatorForSeq2Seq, TrainerCallback
+from typing import TYPE_CHECKING, Optional, List
+from transformers import DataCollatorForSeq2Seq
 
 from llmtuner.dsets import get_dataset, preprocess_dataset, split_dataset
 from llmtuner.extras.callbacks import LogCallback
 from llmtuner.extras.constants import IGNORE_INDEX
+from llmtuner.extras.misc import get_logits_processor
 from llmtuner.extras.ploting import plot_loss
-from llmtuner.hparams import ModelArguments, DataArguments, FinetuningArguments
 from llmtuner.tuner.core import load_model_and_tokenizer
-from llmtuner.tuner.core.trainer import PeftTrainer
+from llmtuner.tuner.sft.metric import ComputeMetrics
+from llmtuner.tuner.sft.trainer import Seq2SeqPeftTrainer
 
+if TYPE_CHECKING:
+    from transformers import Seq2SeqTrainingArguments, TrainerCallback
+    from llmtuner.hparams import ModelArguments, DataArguments, FinetuningArguments
 
-def run_pt(
-    model_args: ModelArguments,
-    data_args: DataArguments,
-    training_args: Seq2SeqTrainingArguments,
-    finetuning_args: FinetuningArguments,
-    callbacks: Optional[List[TrainerCallback]] = [LogCallback()]
+
+def run_sft(
+    model_args: "ModelArguments",
+    data_args: "DataArguments",
+    training_args: "Seq2SeqTrainingArguments",
+    finetuning_args: "FinetuningArguments",
+    callbacks: Optional[List["TrainerCallback"]] = [LogCallback()]
 ):
     dataset = get_dataset(model_args, data_args)
-    model, tokenizer = load_model_and_tokenizer(model_args, finetuning_args, training_args.do_train, stage="pt")
-    dataset = preprocess_dataset(dataset, tokenizer, data_args, training_args, stage="pt")
+    model, tokenizer = load_model_and_tokenizer(model_args, finetuning_args, training_args.do_train, stage="sft")
+    dataset = preprocess_dataset(dataset, tokenizer, data_args, training_args, stage="sft")
     data_collator = DataCollatorForSeq2Seq(
         tokenizer=tokenizer,
         label_pad_token_id=IGNORE_INDEX if data_args.ignore_pad_token_for_loss else tokenizer.pad_token_id
     )
 
+    # Override the decoding parameters of Seq2SeqTrainer
+    training_args.generation_max_length = training_args.generation_max_length if \
+                training_args.generation_max_length is not None else data_args.max_target_length
+    training_args.generation_num_beams = data_args.eval_num_beams if \
+                data_args.eval_num_beams is not None else training_args.generation_num_beams
+
     # Initialize our Trainer
-    trainer = PeftTrainer(
+    trainer = Seq2SeqPeftTrainer(
         finetuning_args=finetuning_args,
         model=model,
         args=training_args,
         tokenizer=tokenizer,
         data_collator=data_collator,
         callbacks=callbacks,
+        compute_metrics=ComputeMetrics(tokenizer) if training_args.predict_with_generate else None,
         **split_dataset(dataset, data_args.dev_ratio, training_args.do_train)
     )
 
+    # Keyword arguments for `model.generate`
+    gen_kwargs = {
+        "do_sample": True,
+        "top_p": 0.7,
+        "max_new_tokens": data_args.max_target_length + 1,
+        "temperature": 0.95,
+        "logits_processor": get_logits_processor()
+    }
+
     # Training
     if training_args.do_train:
         train_result = trainer.train()
         trainer.log_metrics("train", train_result.metrics)
         trainer.save_metrics("train", train_result.metrics)
         trainer.save_state()
         trainer.save_model()
         if trainer.is_world_process_zero() and model_args.plot_loss:
             plot_loss(training_args.output_dir, keys=["loss", "eval_loss"])
 
     # Evaluation
     if training_args.do_eval:
-        metrics = trainer.evaluate(metric_key_prefix="eval")
-        try:
-            perplexity = math.exp(metrics["eval_loss"])
-        except OverflowError:
-            perplexity = float("inf")
-
-        metrics["perplexity"] = perplexity
-
+        metrics = trainer.evaluate(metric_key_prefix="eval", **gen_kwargs)
+        if training_args.predict_with_generate: # eval_loss will be wrong if predict_with_generate is enabled
+            metrics.pop("eval_loss", None)
         trainer.log_metrics("eval", metrics)
         trainer.save_metrics("eval", metrics)
+
+    # Predict
+    if training_args.do_predict:
+        predict_results = trainer.predict(dataset, metric_key_prefix="predict", **gen_kwargs)
+        if training_args.predict_with_generate: # predict_loss will be wrong if predict_with_generate is enabled
+            predict_results.metrics.pop("predict_loss", None)
+        trainer.log_metrics("predict", predict_results.metrics)
+        trainer.save_metrics("predict", predict_results.metrics)
+        trainer.save_predictions(predict_results)
```

### Comparing `llmtuner-0.1.3/src/llmtuner/tuner/rm/collator.py` & `llmtuner-0.1.4/src/llmtuner/tuner/rm/collator.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,9 +11,12 @@
     def __call__(self, features: Sequence[Dict[str, Any]]) -> Dict[str, torch.Tensor]:
         r"""
         Pads batched data to the longest sequence in the batch.
 
         We generate 2 * n examples where the first n examples represent chosen examples and
         the last n examples represent rejected examples.
         """
-        features = [{"input_ids": feature[key]} for key in ("accept_ids", "reject_ids") for feature in features]
+        features = [
+            {"input_ids": feature[key], "attention_mask": [1] * len(feature[key])}
+            for key in ("accept_ids", "reject_ids") for feature in features
+        ]
         return super().__call__(features)
```

### Comparing `llmtuner-0.1.3/src/llmtuner/tuner/rm/trainer.py` & `llmtuner-0.1.4/src/llmtuner/tuner/rm/trainer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import os
 import json
 import torch
-from typing import Dict, List, Optional, Tuple, Union
-from transformers.trainer import PredictionOutput
-from transformers.modeling_utils import PreTrainedModel
+from typing import TYPE_CHECKING, Dict, List, Optional, Tuple, Union
 
 from llmtuner.extras.logging import get_logger
 from llmtuner.tuner.core.trainer import PeftTrainer
 
+if TYPE_CHECKING:
+    from transformers.trainer import PredictionOutput
+    from transformers.modeling_utils import PreTrainedModel
+
 
 logger = get_logger(__name__)
 
 
 class PairwisePeftTrainer(PeftTrainer):
     r"""
     Inherits PeftTrainer to compute pairwise loss.
@@ -19,15 +21,15 @@
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.can_return_loss = True # override property to return eval_loss
 
     def compute_loss(
         self,
-        model: PreTrainedModel,
+        model: "PreTrainedModel",
         inputs: Dict[str, torch.Tensor],
         return_outputs: Optional[bool] = False
     ) -> Union[torch.Tensor, Tuple[torch.Tensor, List[torch.Tensor]]]:
         r"""
         Computes pairwise loss. The first n examples are chosen and the last n examples are rejected.
 
         We use score on the EOS token to represent reward of the whole sentence.
@@ -42,15 +44,15 @@
         _, _, values = model(**inputs, output_hidden_states=True, return_dict=True)
         r_accept, r_reject = values[:, -1].split(batch_size, dim=0)
         loss = -torch.log(torch.sigmoid(r_accept - r_reject)).mean()
         return (loss, [loss, r_accept, r_reject]) if return_outputs else loss
 
     def save_predictions(
         self,
-        predict_results: PredictionOutput
+        predict_results: "PredictionOutput"
     ) -> None:
         r"""
         Saves model predictions to `output_dir`.
 
         A custom behavior that not contained in Seq2SeqTrainer.
         """
         if not self.is_world_process_zero():
```

### Comparing `llmtuner-0.1.3/src/llmtuner/tuner/rm/workflow.py` & `llmtuner-0.1.4/src/llmtuner/tuner/rm/workflow.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # Inspired by:
 # https://github.com/lvwerra/trl/blob/main/examples/summarization/scripts/reward_summarization.py
 # https://github.com/CarperAI/trlx/blob/main/examples/summarize_rlhf/reward_model/train_reward_model_gptj.py
 
-from typing import Optional, List
-from transformers import Seq2SeqTrainingArguments, TrainerCallback
+from typing import TYPE_CHECKING, Optional, List
 
 from llmtuner.dsets import get_dataset, preprocess_dataset, split_dataset
 from llmtuner.extras.callbacks import LogCallback
 from llmtuner.extras.ploting import plot_loss
-from llmtuner.hparams import ModelArguments, DataArguments, FinetuningArguments
 from llmtuner.tuner.core import load_model_and_tokenizer
 from llmtuner.tuner.rm.metric import compute_accuracy
 from llmtuner.tuner.rm.collator import PairwiseDataCollatorWithPadding
 from llmtuner.tuner.rm.trainer import PairwisePeftTrainer
 
+if TYPE_CHECKING:
+    from transformers import Seq2SeqTrainingArguments, TrainerCallback
+    from llmtuner.hparams import ModelArguments, DataArguments, FinetuningArguments
+
 
 def run_rm(
-    model_args: ModelArguments,
-    data_args: DataArguments,
-    training_args: Seq2SeqTrainingArguments,
-    finetuning_args: FinetuningArguments,
-    callbacks: Optional[List[TrainerCallback]] = [LogCallback()]
+    model_args: "ModelArguments",
+    data_args: "DataArguments",
+    training_args: "Seq2SeqTrainingArguments",
+    finetuning_args: "FinetuningArguments",
+    callbacks: Optional[List["TrainerCallback"]] = [LogCallback()]
 ):
     dataset = get_dataset(model_args, data_args)
     model, tokenizer = load_model_and_tokenizer(model_args, finetuning_args, training_args.do_train, stage="rm")
     dataset = preprocess_dataset(dataset, tokenizer, data_args, training_args, stage="rm")
     data_collator = PairwiseDataCollatorWithPadding(tokenizer)
 
     training_args.remove_unused_columns = False # important for pairwise dataset
```

### Comparing `llmtuner-0.1.3/src/llmtuner/tuner/sft/metric.py` & `llmtuner-0.1.4/src/llmtuner/tuner/sft/metric.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import numpy as np
 from dataclasses import dataclass
-from typing import Dict, Sequence, Tuple, Union
-from transformers.tokenization_utils import PreTrainedTokenizer
+from typing import TYPE_CHECKING, Dict, Sequence, Tuple, Union
 
 import jieba
 from rouge_chinese import Rouge
 from nltk.translate.bleu_score import sentence_bleu, SmoothingFunction
 
 from llmtuner.extras.constants import IGNORE_INDEX
 
+if TYPE_CHECKING:
+    from transformers.tokenization_utils import PreTrainedTokenizer
+
 
 @dataclass
 class ComputeMetrics:
     r"""
     Wraps the tokenizer into metric functions, used in Seq2SeqPeftTrainer.
     """
 
-    tokenizer: PreTrainedTokenizer
+    tokenizer: "PreTrainedTokenizer"
 
     def __call__(self, eval_preds: Sequence[Union[np.ndarray, Tuple[np.ndarray]]]) -> Dict[str, float]:
         r"""
         Uses the model predictions to compute metrics.
         """
         preds, labels = eval_preds
         score_dict = {"accuracy": [], "rouge-1": [], "rouge-2": [], "rouge-l": [], "bleu-4": []}
```

### Comparing `llmtuner-0.1.3/src/llmtuner/tuner/sft/trainer.py` & `llmtuner-0.1.4/src/llmtuner/tuner/sft/trainer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import os
 import json
 import torch
 import numpy as np
 import torch.nn as nn
-from typing import Any, Dict, List, Optional, Tuple, Union
-from transformers.trainer import PredictionOutput
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
 from llmtuner.extras.constants import IGNORE_INDEX
 from llmtuner.extras.logging import get_logger
 from llmtuner.tuner.core.trainer import PeftTrainer
 
+if TYPE_CHECKING:
+    from transformers.trainer import PredictionOutput
+
 
 logger = get_logger(__name__)
 
 
 class Seq2SeqPeftTrainer(PeftTrainer):
     r"""
     Inherits PeftTrainer to compute generative metrics such as BLEU and ROUGE.
@@ -77,15 +79,15 @@
 
         padded_tensor = pad_token_id * torch.ones_like(tgt_tensor)
         padded_tensor[:, -src_tensor.shape[-1]:] = src_tensor # adopt left-padding
         return padded_tensor
 
     def save_predictions(
         self,
-        predict_results: PredictionOutput
+        predict_results: "PredictionOutput"
     ) -> None:
         r"""
         Saves model predictions to `output_dir`.
 
         A custom behavior that not contained in Seq2SeqTrainer.
         """
         if not self.is_world_process_zero():
```

### Comparing `llmtuner-0.1.3/src/llmtuner/webui/chat.py` & `llmtuner-0.1.4/src/llmtuner/webui/chat.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
         yield ALERTS["info_loading"][lang]
         args = dict(
             model_name_or_path=model_name_or_path,
             checkpoint_dir=checkpoint_dir,
             finetuning_type=finetuning_type,
             quantization_bit=int(quantization_bit) if quantization_bit else None,
-            prompt_template=template,
+            template=template,
             source_prefix=source_prefix
         )
         super().__init__(*get_infer_args(args))
 
         yield ALERTS["info_loaded"][lang]
 
     def unload_model(self, lang: str):
@@ -86,10 +86,12 @@
             response += new_text
             response = self.postprocess(response)
             new_history = history + [(query, response)]
             chatbot[-1] = [query, response]
             yield chatbot, new_history
 
     def postprocess(self, response: str) -> str:
-        response = response.replace("<", "&lt;")
-        response = response.replace(">", "&gt;")
-        return response
+        blocks = response.split("```")
+        for i, block in enumerate(blocks):
+            if i % 2 == 0:
+                blocks[i] = block.replace("<", "&lt;").replace(">", "&gt;")
+        return "```".join(blocks)
```

### Comparing `llmtuner-0.1.3/src/llmtuner/webui/common.py` & `llmtuner-0.1.4/src/llmtuner/webui/common.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.3/src/llmtuner/webui/components/chatbot.py` & `llmtuner-0.1.4/src/llmtuner/webui/components/chatbot.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-from typing import Dict, Optional, Tuple
+from typing import TYPE_CHECKING, Dict, Optional, Tuple
 
 import gradio as gr
-from gradio.blocks import Block
-from gradio.components import Component
 
-from llmtuner.webui.chat import WebChatModel
+if TYPE_CHECKING:
+    from gradio.blocks import Block
+    from gradio.components import Component
+    from llmtuner.webui.chat import WebChatModel
 
 
 def create_chat_box(
-    chat_model: WebChatModel,
+    chat_model: "WebChatModel",
     visible: Optional[bool] = False
-) -> Tuple[Block, Component, Component, Dict[str, Component]]:
+) -> Tuple["Block", "Component", "Component", Dict[str, "Component"]]:
     with gr.Box(visible=visible) as chat_box:
         chatbot = gr.Chatbot()
 
         with gr.Row():
             with gr.Column(scale=4):
                 prefix = gr.Textbox(show_label=False)
                 query = gr.Textbox(show_label=False, lines=8)
```

### Comparing `llmtuner-0.1.3/src/llmtuner/webui/components/eval.py` & `llmtuner-0.1.4/src/llmtuner/webui/components/eval.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-from typing import Dict
+from typing import TYPE_CHECKING, Dict
 import gradio as gr
-from gradio.components import Component
 
 from llmtuner.webui.common import list_dataset, DEFAULT_DATA_DIR
 from llmtuner.webui.components.data import create_preview_box
-from llmtuner.webui.runner import Runner
 from llmtuner.webui.utils import can_preview, get_preview
 
+if TYPE_CHECKING:
+    from gradio.components import Component
+    from llmtuner.webui.runner import Runner
 
-def create_eval_tab(top_elems: Dict[str, Component], runner: Runner) -> Dict[str, Component]:
+
+def create_eval_tab(top_elems: Dict[str, "Component"], runner: "Runner") -> Dict[str, "Component"]:
     with gr.Row():
         dataset_dir = gr.Textbox(value=DEFAULT_DATA_DIR, scale=2)
         dataset = gr.Dropdown(multiselect=True, scale=4)
         preview_btn = gr.Button(interactive=False, scale=1)
 
     preview_box, preview_count, preview_samples, close_btn = create_preview_box()
```

### Comparing `llmtuner-0.1.3/src/llmtuner/webui/components/export.py` & `llmtuner-0.1.4/src/llmtuner/webui/components/export.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-from typing import Dict
+from typing import TYPE_CHECKING, Dict
 import gradio as gr
-from gradio.components import Component
 
 from llmtuner.webui.utils import export_model
 
+if TYPE_CHECKING:
+    from gradio.components import Component
 
-def create_export_tab(top_elems: Dict[str, Component]) -> Dict[str, Component]:
+
+def create_export_tab(top_elems: Dict[str, "Component"]) -> Dict[str, "Component"]:
     with gr.Row():
         save_dir = gr.Textbox()
         max_shard_size = gr.Slider(value=10, minimum=1, maximum=100)
 
     export_btn = gr.Button()
     info_box = gr.Textbox(show_label=False, interactive=False)
```

### Comparing `llmtuner-0.1.3/src/llmtuner/webui/components/infer.py` & `llmtuner-0.1.4/src/llmtuner/webui/components/infer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-from typing import Dict
+from typing import TYPE_CHECKING, Dict
 
 import gradio as gr
-from gradio.components import Component
 
 from llmtuner.webui.chat import WebChatModel
 from llmtuner.webui.components.chatbot import create_chat_box
 
+if TYPE_CHECKING:
+    from gradio.components import Component
 
-def create_infer_tab(top_elems: Dict[str, Component]) -> Dict[str, Component]:
+
+def create_infer_tab(top_elems: Dict[str, "Component"]) -> Dict[str, "Component"]:
     with gr.Row():
         load_btn = gr.Button()
         unload_btn = gr.Button()
 
     info_box = gr.Textbox(show_label=False, interactive=False)
 
     chat_model = WebChatModel()
```

### Comparing `llmtuner-0.1.3/src/llmtuner/webui/components/sft.py` & `llmtuner-0.1.4/src/llmtuner/webui/components/sft.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-from typing import Dict
+from typing import TYPE_CHECKING, Dict
 from transformers.trainer_utils import SchedulerType
 
 import gradio as gr
-from gradio.components import Component
 
 from llmtuner.webui.common import list_dataset, DEFAULT_DATA_DIR
 from llmtuner.webui.components.data import create_preview_box
-from llmtuner.webui.runner import Runner
 from llmtuner.webui.utils import can_preview, get_preview, gen_plot
 
+if TYPE_CHECKING:
+    from gradio.components import Component
+    from llmtuner.webui.runner import Runner
 
-def create_sft_tab(top_elems: Dict[str, Component], runner: Runner) -> Dict[str, Component]:
+
+def create_sft_tab(top_elems: Dict[str, "Component"], runner: "Runner") -> Dict[str, "Component"]:
     with gr.Row():
         dataset_dir = gr.Textbox(value=DEFAULT_DATA_DIR, scale=2)
         dataset = gr.Dropdown(multiselect=True, scale=4)
         preview_btn = gr.Button(interactive=False, scale=1)
 
     preview_box, preview_count, preview_samples, close_btn = create_preview_box()
 
@@ -52,15 +54,15 @@
             lora_target = gr.Textbox(scale=2)
 
     with gr.Row():
         start_btn = gr.Button()
         stop_btn = gr.Button()
 
     with gr.Row():
-        with gr.Column(scale=4):
+        with gr.Column(scale=3):
             output_dir = gr.Textbox()
 
             with gr.Box():
                 output_box = gr.Markdown()
 
         with gr.Column(scale=1):
             loss_viewer = gr.Plot()
```

### Comparing `llmtuner-0.1.3/src/llmtuner/webui/components/top.py` & `llmtuner-0.1.4/src/llmtuner/webui/components/top.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-from typing import Dict
+from typing import TYPE_CHECKING, Dict
 
 import gradio as gr
-from gradio.components import Component
 
 from llmtuner.extras.constants import METHODS, SUPPORTED_MODELS
 from llmtuner.extras.template import templates
 from llmtuner.webui.common import list_checkpoint, get_model_path, save_config
 from llmtuner.webui.utils import can_quantize
 
+if TYPE_CHECKING:
+    from gradio.components import Component
 
-def create_top() -> Dict[str, Component]:
+
+def create_top() -> Dict[str, "Component"]:
     available_models = list(SUPPORTED_MODELS.keys()) + ["Custom"]
 
     with gr.Row():
         lang = gr.Dropdown(choices=["en", "zh"], value="en", scale=1)
         model_name = gr.Dropdown(choices=available_models, scale=3)
         model_path = gr.Textbox(scale=3)
```

### Comparing `llmtuner-0.1.3/src/llmtuner/webui/interface.py` & `llmtuner-0.1.4/src/llmtuner/webui/interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,8 +51,8 @@
 
     return demo
 
 
 if __name__ == "__main__":
     demo = create_ui()
     demo.queue()
-    demo.launch(server_name="0.0.0.0", share=False, inbrowser=True)
+    demo.launch(server_name="0.0.0.0", server_port=7860, share=False, inbrowser=True)
```

### Comparing `llmtuner-0.1.3/src/llmtuner/webui/locales.py` & `llmtuner-0.1.4/src/llmtuner/webui/locales.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.3/src/llmtuner/webui/manager.py` & `llmtuner-0.1.4/src/llmtuner/webui/manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import gradio as gr
-from typing import Any, Dict, List
 from gradio.components import Component
+from typing import Any, Dict, List
 
 from llmtuner.webui.common import get_model_path, list_dataset, load_config
 from llmtuner.webui.locales import LOCALES
 from llmtuner.webui.utils import get_time
 
 
 class Manager:
@@ -20,15 +20,15 @@
         user_config = load_config()
         if user_config["last_model"]:
             refresh_dict["model_name"] = {"value": user_config["last_model"]}
             refresh_dict["model_path"] = {"value": get_model_path(user_config["last_model"])}
 
         return refresh_dict
 
-    def gen_label(self, lang: str) -> Dict[Component, dict]:
+    def gen_label(self, lang: str) -> Dict[Component, Dict[str, Any]]: # cannot use TYPE_CHECKING
         update_dict = {}
         refresh_dict = self.gen_refresh()
 
         for elems in self.elem_list:
             for name, component in elems.items():
                 update_dict[component] = gr.update(**LOCALES[name][lang], **refresh_dict.get(name, {}))
```

### Comparing `llmtuner-0.1.3/src/llmtuner/webui/runner.py` & `llmtuner-0.1.4/src/llmtuner/webui/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         args = dict(
             model_name_or_path=model_name_or_path,
             do_train=True,
             overwrite_cache=True,
             checkpoint_dir=checkpoint_dir,
             finetuning_type=finetuning_type,
             quantization_bit=int(quantization_bit) if quantization_bit else None,
-            prompt_template=template,
+            template=template,
             source_prefix=source_prefix,
             dataset_dir=dataset_dir,
             dataset=",".join(dataset),
             max_source_length=max_source_length,
             max_target_length=max_target_length,
             learning_rate=float(learning_rate),
             num_train_epochs=float(num_train_epochs),
@@ -197,15 +197,15 @@
             model_name_or_path=model_name_or_path,
             do_eval=True,
             overwrite_cache=True,
             predict_with_generate=True,
             checkpoint_dir=checkpoint_dir,
             finetuning_type=finetuning_type,
             quantization_bit=int(quantization_bit) if quantization_bit else None,
-            prompt_template=template,
+            template=template,
             source_prefix=source_prefix,
             dataset_dir=dataset_dir,
             dataset=",".join(dataset),
             max_source_length=max_source_length,
             max_target_length=max_target_length,
             max_samples=int(max_samples),
             per_device_eval_batch_size=batch_size,
```

### Comparing `llmtuner-0.1.3/src/llmtuner/webui/utils.py` & `llmtuner-0.1.4/src/llmtuner/webui/utils.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.3/src/llmtuner.egg-info/PKG-INFO` & `llmtuner-0.1.4/src/llmtuner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmtuner
-Version: 0.1.3
+Version: 0.1.4
 Summary: Easy-to-use fine-tuning framework using PEFT
 Home-page: https://github.com/hiyouga/LLaMA-Efficient-Tuning
 Author: hiyouga
 Author-email: hiyouga@buaa.edu.cn
 License: Apache 2.0 License
 Keywords: LLaMA,BLOOM,Falcon,LLM,ChatGPT,transformer,pytorch,deep learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `llmtuner-0.1.3/src/llmtuner.egg-info/SOURCES.txt` & `llmtuner-0.1.4/src/llmtuner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

