# Comparing `tmp/ochat-3.1.0.tar.gz` & `tmp/ochat-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ochat-3.1.0.tar", last modified: Mon Jul 31 06:51:19 2023, max compression
+gzip compressed data, was "ochat-3.1.1.tar", last modified: Tue Aug  1 17:53:29 2023, max compression
```

## Comparing `ochat-3.1.0.tar` & `ochat-3.1.1.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:51:19.702022 ochat-3.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:51:19.638022 ochat-3.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:51:19.642022 ochat-3.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-31 06:51:08.000000 ochat-3.1.0/.github/workflows/pypi_publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-07-31 06:51:08.000000 ochat-3.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-31 06:51:08.000000 ochat-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19091 2023-07-31 06:51:19.702022 ochat-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18617 2023-07-31 06:51:08.000000 ochat-3.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-31 06:51:08.000000 ochat-3.1.0/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:51:19.642022 ochat-3.1.0/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   568121 2023-07-31 06:51:08.000000 ochat-3.1.0/assets/embeddings.svg
--rw-r--r--   0 runner    (1001) docker     (123)    68349 2023-07-31 06:51:08.000000 ochat-3.1.0/assets/logo_new.png
--rw-r--r--   0 runner    (1001) docker     (123)    10181 2023-07-31 06:51:08.000000 ochat-3.1.0/assets/vicuna_gpt35.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-07-31 06:51:08.000000 ochat-3.1.0/assets/vicuna_gpt4.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:51:19.642022 ochat-3.1.0/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-31 06:51:08.000000 ochat-3.1.0/docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-31 06:51:08.000000 ochat-3.1.0/docker/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-31 06:51:08.000000 ochat-3.1.0/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:51:19.642022 ochat-3.1.0/ochat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:51:19.642022 ochat-3.1.0/ochat/config/
--rw-r--r--   0 runner    (1001) docker     (123)     8635 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/config/model_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:51:19.642022 ochat-3.1.0/ochat/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/data/clean_sharegpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/data/filter_language.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/data/filter_sharegpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/data/generate_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/data/generate_dataset_orca.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/data/merge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      882 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/data/run_data_pipeline.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:51:19.646022 ochat-3.1.0/ochat/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/conversation_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:51:19.638022 ochat-3.1.0/ochat/evaluation/eval_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:51:19.638022 ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:51:19.670022 ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/
--rw-r--r--   0 runner    (1001) docker     (123)   491290 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/boolean_expressions.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   902939 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/causal_judgement.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   384612 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/date_understanding.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)  1013894 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/disambiguation_qa.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   687182 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/dyck_languages.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)  1293180 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/formal_fallacies.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)  1341960 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/geometric_shapes.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   855574 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/hyperbaton.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   816845 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/logical_deduction_five_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   863272 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/logical_deduction_seven_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   770081 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/logical_deduction_three_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   618185 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/movie_recommendation.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   638443 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/multistep_arithmetic_two.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   616281 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/navigate.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   413258 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/object_counting.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   441275 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/penguins_in_a_table.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   725193 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/reasoning_about_colored_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   984109 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/ruin_names.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)  1870311 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/salient_translation_error_detection.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   614065 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/snarks.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   251485 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/sports_understanding.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   942794 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/temporal_sequences.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   852090 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/tracking_shuffled_objects_five_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   900774 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/tracking_shuffled_objects_seven_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   807604 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/tracking_shuffled_objects_three_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   809832 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/web_of_lies.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   669168 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/word_sorting.jsonl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:51:19.674022 ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/gsm8k/
--rw-r--r--   0 runner    (1001) docker     (123) 11708109 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/gsm8k/gsm8k.jsonl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:51:19.638022 ochat-3.1.0/ochat/evaluation/eval_data/zs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:51:19.690022 ochat-3.1.0/ochat/evaluation/eval_data/zs/agieval/
--rw-r--r--   0 runner    (1001) docker     (123)    92097 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/zs/agieval/aqua-rat.zero-shot.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   638524 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/zs/agieval/logiqa-en.zero-shot.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   235210 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/zs/agieval/lsat-ar.zero-shot.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   626756 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/zs/agieval/lsat-lr.zero-shot.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)  1003390 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/zs/agieval/lsat-rc.zero-shot.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   103531 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/zs/agieval/sat-en-without-passage.zero-shot.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   970033 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/zs/agieval/sat-en.zero-shot.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   102321 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/zs/agieval/sat-math.zero-shot.jsonl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:51:19.698022 ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/
--rw-r--r--   0 runner    (1001) docker     (123)    54425 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/boolean_expressions.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   227316 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/causal_judgment.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)    89913 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/date_understanding.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   115064 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/disambiguation_qa.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   182364 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/formal_fallacies_syllogisms_negation.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   113342 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/geometric_shapes.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)    73824 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/hyperbaton.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   201521 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/logical_deduction_five_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   247838 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/logical_deduction_seven_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   155266 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/logical_deduction_three_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)    84517 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/movie_recommendation.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)    99515 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/navigate.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)    98794 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/penguins_in_a_table.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   161261 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/reasoning_about_colored_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)    91553 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/ruin_names.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   326806 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/salient_translation_error_detection.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)    62891 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/snarks.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)    92422 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/sports_understanding.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   184818 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/temporal_sequences.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   227141 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/tracking_shuffled_objects_five_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   276090 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/tracking_shuffled_objects_seven_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)   184755 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/tracking_shuffled_objects_three_objects.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)    92710 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/web_of_lies.jsonl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:51:19.698022 ochat-3.1.0/ochat/evaluation/eval_data/zs/truthfulqa_orca/
--rw-r--r--   0 runner    (1001) docker     (123)   265442 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/eval_data/zs/truthfulqa_orca/truthfulqa_mc.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/match_answer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7711 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/run_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/evaluation/view_results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:51:19.702022 ochat-3.1.0/ochat/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/experimental/generate_dataset_old.py
--rw-r--r--   0 runner    (1001) docker     (123)    62488 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/experimental/sharegpt.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/experimental/test_multipack_dataloader.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    15217 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/experimental/text_length.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/experimental/train_alpaca.py
--rw-r--r--   0 runner    (1001) docker     (123)    19694 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/experimental/verify_dataset.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    21113 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/experimental/verify_dataset_orca.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:51:19.702022 ochat-3.1.0/ochat/models/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16732 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/models/unpadded_llama.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:51:19.702022 ochat-3.1.0/ochat/serving/
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/serving/async_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/serving/openai_api_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/serving/openai_api_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:51:19.702022 ochat-3.1.0/ochat/training_deepspeed/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/training_deepspeed/deepspeed_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/training_deepspeed/multipack_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/training_deepspeed/parquet_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    13155 2023-07-31 06:51:08.000000 ochat-3.1.0/ochat/training_deepspeed/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:51:19.642022 ochat-3.1.0/ochat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19091 2023-07-31 06:51:19.000000 ochat-3.1.0/ochat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-07-31 06:51:19.000000 ochat-3.1.0/ochat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 06:51:19.000000 ochat-3.1.0/ochat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-31 06:51:19.000000 ochat-3.1.0/ochat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-31 06:51:19.000000 ochat-3.1.0/ochat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-31 06:51:08.000000 ochat-3.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 06:51:19.702022 ochat-3.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.585908 ochat-3.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.525907 ochat-3.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.525907 ochat-3.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-01 17:53:19.000000 ochat-3.1.1/.github/workflows/pypi_publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-08-01 17:53:19.000000 ochat-3.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-08-01 17:53:19.000000 ochat-3.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19057 2023-08-01 17:53:29.585908 ochat-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18583 2023-08-01 17:53:19.000000 ochat-3.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-08-01 17:53:19.000000 ochat-3.1.1/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.529907 ochat-3.1.1/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   568121 2023-08-01 17:53:19.000000 ochat-3.1.1/assets/embeddings.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    68349 2023-08-01 17:53:19.000000 ochat-3.1.1/assets/logo_new.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10181 2023-08-01 17:53:19.000000 ochat-3.1.1/assets/vicuna_gpt35.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-08-01 17:53:19.000000 ochat-3.1.1/assets/vicuna_gpt4.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.529907 ochat-3.1.1/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-01 17:53:19.000000 ochat-3.1.1/docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-01 17:53:19.000000 ochat-3.1.1/docker/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-08-01 17:53:19.000000 ochat-3.1.1/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.529907 ochat-3.1.1/ochat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.529907 ochat-3.1.1/ochat/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     8635 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/config/model_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.529907 ochat-3.1.1/ochat/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/data/clean_sharegpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/data/filter_language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/data/filter_sharegpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/data/generate_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/data/generate_dataset_orca.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/data/merge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      882 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/data/run_data_pipeline.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.533907 ochat-3.1.1/ochat/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/conversation_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.525907 ochat-3.1.1/ochat/evaluation/eval_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.525907 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.557907 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/
+-rw-r--r--   0 runner    (1001) docker     (123)   491290 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/boolean_expressions.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   902939 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/causal_judgement.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   384612 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/date_understanding.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)  1013894 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/disambiguation_qa.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   687182 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/dyck_languages.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)  1293180 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/formal_fallacies.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)  1341960 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/geometric_shapes.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   855574 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/hyperbaton.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   816845 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/logical_deduction_five_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   863272 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/logical_deduction_seven_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   770081 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/logical_deduction_three_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   618185 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/movie_recommendation.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   638443 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/multistep_arithmetic_two.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   616281 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/navigate.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   413258 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/object_counting.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   441275 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/penguins_in_a_table.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   725193 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/reasoning_about_colored_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   984109 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/ruin_names.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)  1870311 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/salient_translation_error_detection.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   614065 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/snarks.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   251485 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/sports_understanding.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   942794 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/temporal_sequences.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   852090 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/tracking_shuffled_objects_five_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   900774 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/tracking_shuffled_objects_seven_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   807604 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/tracking_shuffled_objects_three_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   809832 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/web_of_lies.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   669168 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/word_sorting.jsonl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.557907 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/gsm8k/
+-rw-r--r--   0 runner    (1001) docker     (123) 11708109 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/gsm8k/gsm8k.jsonl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.525907 ochat-3.1.1/ochat/evaluation/eval_data/zs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.577908 ochat-3.1.1/ochat/evaluation/eval_data/zs/agieval/
+-rw-r--r--   0 runner    (1001) docker     (123)    92097 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/agieval/aqua-rat.zero-shot.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   638524 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/agieval/logiqa-en.zero-shot.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   235210 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/agieval/lsat-ar.zero-shot.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   626756 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/agieval/lsat-lr.zero-shot.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)  1003390 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/agieval/lsat-rc.zero-shot.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   103531 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/agieval/sat-en-without-passage.zero-shot.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   970033 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/agieval/sat-en.zero-shot.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   102321 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/agieval/sat-math.zero-shot.jsonl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.581908 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/
+-rw-r--r--   0 runner    (1001) docker     (123)    54425 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/boolean_expressions.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   227316 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/causal_judgment.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)    89913 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/date_understanding.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   115064 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/disambiguation_qa.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   182364 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/formal_fallacies_syllogisms_negation.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   113342 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/geometric_shapes.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)    73824 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/hyperbaton.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   201521 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/logical_deduction_five_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   247838 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/logical_deduction_seven_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   155266 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/logical_deduction_three_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)    84517 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/movie_recommendation.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)    99515 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/navigate.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)    98794 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/penguins_in_a_table.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   161261 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/reasoning_about_colored_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)    91553 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/ruin_names.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   326806 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/salient_translation_error_detection.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)    62891 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/snarks.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)    92422 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/sports_understanding.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   184818 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/temporal_sequences.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   227141 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/tracking_shuffled_objects_five_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   276090 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/tracking_shuffled_objects_seven_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)   184755 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/tracking_shuffled_objects_three_objects.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)    92710 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/web_of_lies.jsonl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.581908 ochat-3.1.1/ochat/evaluation/eval_data/zs/truthfulqa_orca/
+-rw-r--r--   0 runner    (1001) docker     (123)   265442 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/eval_data/zs/truthfulqa_orca/truthfulqa_mc.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/match_answer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7711 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/run_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/evaluation/view_results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.585908 ochat-3.1.1/ochat/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/experimental/generate_dataset_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62488 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/experimental/sharegpt.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/experimental/test_multipack_dataloader.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    15217 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/experimental/text_length.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/experimental/train_alpaca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19694 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/experimental/verify_dataset.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    21113 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/experimental/verify_dataset_orca.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.585908 ochat-3.1.1/ochat/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16845 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/models/unpadded_llama.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.585908 ochat-3.1.1/ochat/serving/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/serving/async_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/serving/openai_api_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/serving/openai_api_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.585908 ochat-3.1.1/ochat/training_deepspeed/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/training_deepspeed/deepspeed_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/training_deepspeed/multipack_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/training_deepspeed/parquet_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13155 2023-08-01 17:53:19.000000 ochat-3.1.1/ochat/training_deepspeed/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 17:53:29.529907 ochat-3.1.1/ochat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19057 2023-08-01 17:53:29.000000 ochat-3.1.1/ochat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-08-01 17:53:29.000000 ochat-3.1.1/ochat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 17:53:29.000000 ochat-3.1.1/ochat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-08-01 17:53:29.000000 ochat-3.1.1/ochat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 17:53:29.000000 ochat-3.1.1/ochat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-08-01 17:53:19.000000 ochat-3.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 17:53:29.585908 ochat-3.1.1/setup.cfg
```

### Comparing `ochat-3.1.0/.gitignore` & `ochat-3.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/LICENSE` & `ochat-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/PKG-INFO` & `ochat-3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ochat
-Version: 3.1.0
+Version: 3.1.1
 Summary: An efficient framework for training and serving top-tier, open-source conversational LLMs.
 Project-URL: Homepage, https://github.com/imoneoi/openchat
 Project-URL: Bug Tracker, https://github.com/imoneoi/openchat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -50,15 +50,15 @@
 <details>
   <summary>Example request (click to expand)</summary>
 
 ```bash
 curl http://localhost:18888/v1/chat/completions \
   -H "Content-Type: application/json" \
   -d '{
-    "model": "openchat_v3.1_llama2",
+    "model": "openchat_v3.2",
     "messages": [{"role": "user", "content": "You are a large language model named OpenChat. Write a poem to describe yourself"}]
   }'
 ```
 
 </details>
 
 | Model        | Size | Context | Weights                                                      | Serving                                                                                                                                                                      |
@@ -67,38 +67,38 @@
 | OpenChat 3.1 | 13B  | 4096    | [Huggingface](https://huggingface.co/openchat/openchat_v3.1) | `python -m ochat.serving.openai_api_server --model-type openchat_v3.1_llama2 --model openchat/openchat_v3.1 --engine-use-ray --worker-use-ray --max-num-batched-tokens 5120` |
 
 For inference with Huggingface Transformers (slow and not recommended), follow the conversation template provided below:
 
 <details>
   <summary>Conversation templates (click to expand)</summary>
 
-V3.1
-
-```python
-# Single-turn V3.1
-tokenize("Assistant is GPT4<|end_of_turn|>User: Hello<|end_of_turn|>Assistant:")
-# Result: [1, 4007, 22137, 338, 402, 7982, 29946, 32000, 4911, 29901, 15043, 32000, 4007, 22137, 29901]
-
-# Multi-turn V3.1
-tokenize("Assistant is GPT4<|end_of_turn|>User: Hello<|end_of_turn|>Assistant: Hi<|end_of_turn|>User: How are you today?<|end_of_turn|>Assistant:")
-# Result: [1, 4007, 22137, 338, 402, 7982, 29946, 32000, 4911, 29901, 15043, 32000, 4007, 22137, 29901, 6324, 32000, 4911, 29901, 1128, 526, 366, 9826, 29973, 32000, 4007, 22137, 29901]
-```
-
 V3.2
 
 ```python
 # Single-turn V3.2
 tokenize("GPT4 User: Hello<|end_of_turn|>GPT4 Assistant:")
 # Result: [1, 402, 7982, 29946, 4911, 29901, 15043, 32000, 402, 7982, 29946, 4007, 22137, 29901]
 
 # Multi-turn V3.2
 tokenize("GPT4 User: Hello<|end_of_turn|>GPT4 Assistant: Hi<|end_of_turn|>GPT4 User: How are you today?<|end_of_turn|>GPT4 Assistant:")
 # Result: [1, 402, 7982, 29946, 4911, 29901, 15043, 32000, 402, 7982, 29946, 4007, 22137, 29901, 6324, 32000, 402, 7982, 29946, 4911, 29901, 1128, 526, 366, 9826, 29973, 32000, 402, 7982, 29946, 4007, 22137, 29901]
 ```
 
+V3.1
+
+```python
+# Single-turn V3.1
+tokenize("Assistant is GPT4<|end_of_turn|>User: Hello<|end_of_turn|>Assistant:")
+# Result: [1, 4007, 22137, 338, 402, 7982, 29946, 32000, 4911, 29901, 15043, 32000, 4007, 22137, 29901]
+
+# Multi-turn V3.1
+tokenize("Assistant is GPT4<|end_of_turn|>User: Hello<|end_of_turn|>Assistant: Hi<|end_of_turn|>User: How are you today?<|end_of_turn|>Assistant:")
+# Result: [1, 4007, 22137, 338, 402, 7982, 29946, 32000, 4911, 29901, 15043, 32000, 4007, 22137, 29901, 6324, 32000, 4911, 29901, 1128, 526, 366, 9826, 29973, 32000, 4007, 22137, 29901]
+```
+
 </details>
 
 ## <a id="benchmarks"></a> Benchmarks
 
 We have evaluated our models using the two most popular evaluation benchmarks **, including AlpacaEval and MT-bench. Here we list the top models with our released versions, sorted by model size in descending order. The full version can be found on the [MT-bench](https://chat.lmsys.org/?leaderboard) and [AlpacaEval](https://tatsu-lab.github.io/alpaca_eval/) leaderboards.
 
 To ensure consistency, we used the same routine as ChatGPT / GPT-4 to run these benchmarks. We started the OpenAI API-compatible server and set the `openai.api_base` to `http://localhost:18888/v1` in the benchmark program.
@@ -122,24 +122,28 @@
 
 🚀 To ensure comprehensive evaluation of large language models (LLMs), we are working on developing a suite of accelerated standard benchmarks, including AGIEval, BBH, and Chain-of-Thought Hub, named vLLM Eval. This suite leverages the speedup provided by [vLLM](https://github.com/vllm-project/vllm) and allows us to finish the entire benchmark in just 5 minutes.
 
 We will release the evaluation results as soon as they become available, so stay tuned!
 
 ## <a id="installation"></a> Installation
 
-To use OpenChat, you need to install CUDA and PyTorch, then install FlashAttention 1. After that you can install OpenChat via pip:
+To use OpenChat, you need to install CUDA and PyTorch, then you can install OpenChat via pip:
+
+```bash
+pip3 install ochat
+```
+
+If you want to train models, please also install FlashAttention 1.
 
 ```bash
 pip3 install packaging ninja
 pip3 install --no-build-isolation "flash-attn<2"
-
-pip3 install ochat
 ```
 
-FlashAttention may have compatibility issues. If you encounter these problems, you can try to create a new `conda` environment following the instructions below.
+FlashAttention and vLLM may have compatibility issues. If you encounter these problems, you can try to create a new `conda` environment following the instructions below.
 
 ```bash
 conda create -y --name openchat
 conda activate openchat
 
 conda install -y python
 conda install -y cudatoolkit-dev -c conda-forge
@@ -154,17 +158,14 @@
 <details>
   <summary>In addition to pypi, you can also install from source (click to expand)</summary>
 
 ```bash
 git clone https://github.com/imoneoi/openchat
 cd openchat
 
-pip3 install packaging ninja
-pip3 install --no-build-isolation "flash-attn<2"
-
 pip3 install --upgrade pip  # enable PEP 660 support
 pip3 install -e .
 ```
 </details>
 
 
 ## <a id="web-ui"></a> Web UI
```

### Comparing `ochat-3.1.0/README.md` & `ochat-3.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 <details>
   <summary>Example request (click to expand)</summary>
 
 ```bash
 curl http://localhost:18888/v1/chat/completions \
   -H "Content-Type: application/json" \
   -d '{
-    "model": "openchat_v3.1_llama2",
+    "model": "openchat_v3.2",
     "messages": [{"role": "user", "content": "You are a large language model named OpenChat. Write a poem to describe yourself"}]
   }'
 ```
 
 </details>
 
 | Model        | Size | Context | Weights                                                      | Serving                                                                                                                                                                      |
@@ -55,38 +55,38 @@
 | OpenChat 3.1 | 13B  | 4096    | [Huggingface](https://huggingface.co/openchat/openchat_v3.1) | `python -m ochat.serving.openai_api_server --model-type openchat_v3.1_llama2 --model openchat/openchat_v3.1 --engine-use-ray --worker-use-ray --max-num-batched-tokens 5120` |
 
 For inference with Huggingface Transformers (slow and not recommended), follow the conversation template provided below:
 
 <details>
   <summary>Conversation templates (click to expand)</summary>
 
-V3.1
-
-```python
-# Single-turn V3.1
-tokenize("Assistant is GPT4<|end_of_turn|>User: Hello<|end_of_turn|>Assistant:")
-# Result: [1, 4007, 22137, 338, 402, 7982, 29946, 32000, 4911, 29901, 15043, 32000, 4007, 22137, 29901]
-
-# Multi-turn V3.1
-tokenize("Assistant is GPT4<|end_of_turn|>User: Hello<|end_of_turn|>Assistant: Hi<|end_of_turn|>User: How are you today?<|end_of_turn|>Assistant:")
-# Result: [1, 4007, 22137, 338, 402, 7982, 29946, 32000, 4911, 29901, 15043, 32000, 4007, 22137, 29901, 6324, 32000, 4911, 29901, 1128, 526, 366, 9826, 29973, 32000, 4007, 22137, 29901]
-```
-
 V3.2
 
 ```python
 # Single-turn V3.2
 tokenize("GPT4 User: Hello<|end_of_turn|>GPT4 Assistant:")
 # Result: [1, 402, 7982, 29946, 4911, 29901, 15043, 32000, 402, 7982, 29946, 4007, 22137, 29901]
 
 # Multi-turn V3.2
 tokenize("GPT4 User: Hello<|end_of_turn|>GPT4 Assistant: Hi<|end_of_turn|>GPT4 User: How are you today?<|end_of_turn|>GPT4 Assistant:")
 # Result: [1, 402, 7982, 29946, 4911, 29901, 15043, 32000, 402, 7982, 29946, 4007, 22137, 29901, 6324, 32000, 402, 7982, 29946, 4911, 29901, 1128, 526, 366, 9826, 29973, 32000, 402, 7982, 29946, 4007, 22137, 29901]
 ```
 
+V3.1
+
+```python
+# Single-turn V3.1
+tokenize("Assistant is GPT4<|end_of_turn|>User: Hello<|end_of_turn|>Assistant:")
+# Result: [1, 4007, 22137, 338, 402, 7982, 29946, 32000, 4911, 29901, 15043, 32000, 4007, 22137, 29901]
+
+# Multi-turn V3.1
+tokenize("Assistant is GPT4<|end_of_turn|>User: Hello<|end_of_turn|>Assistant: Hi<|end_of_turn|>User: How are you today?<|end_of_turn|>Assistant:")
+# Result: [1, 4007, 22137, 338, 402, 7982, 29946, 32000, 4911, 29901, 15043, 32000, 4007, 22137, 29901, 6324, 32000, 4911, 29901, 1128, 526, 366, 9826, 29973, 32000, 4007, 22137, 29901]
+```
+
 </details>
 
 ## <a id="benchmarks"></a> Benchmarks
 
 We have evaluated our models using the two most popular evaluation benchmarks **, including AlpacaEval and MT-bench. Here we list the top models with our released versions, sorted by model size in descending order. The full version can be found on the [MT-bench](https://chat.lmsys.org/?leaderboard) and [AlpacaEval](https://tatsu-lab.github.io/alpaca_eval/) leaderboards.
 
 To ensure consistency, we used the same routine as ChatGPT / GPT-4 to run these benchmarks. We started the OpenAI API-compatible server and set the `openai.api_base` to `http://localhost:18888/v1` in the benchmark program.
@@ -110,24 +110,28 @@
 
 🚀 To ensure comprehensive evaluation of large language models (LLMs), we are working on developing a suite of accelerated standard benchmarks, including AGIEval, BBH, and Chain-of-Thought Hub, named vLLM Eval. This suite leverages the speedup provided by [vLLM](https://github.com/vllm-project/vllm) and allows us to finish the entire benchmark in just 5 minutes.
 
 We will release the evaluation results as soon as they become available, so stay tuned!
 
 ## <a id="installation"></a> Installation
 
-To use OpenChat, you need to install CUDA and PyTorch, then install FlashAttention 1. After that you can install OpenChat via pip:
+To use OpenChat, you need to install CUDA and PyTorch, then you can install OpenChat via pip:
+
+```bash
+pip3 install ochat
+```
+
+If you want to train models, please also install FlashAttention 1.
 
 ```bash
 pip3 install packaging ninja
 pip3 install --no-build-isolation "flash-attn<2"
-
-pip3 install ochat
 ```
 
-FlashAttention may have compatibility issues. If you encounter these problems, you can try to create a new `conda` environment following the instructions below.
+FlashAttention and vLLM may have compatibility issues. If you encounter these problems, you can try to create a new `conda` environment following the instructions below.
 
 ```bash
 conda create -y --name openchat
 conda activate openchat
 
 conda install -y python
 conda install -y cudatoolkit-dev -c conda-forge
@@ -142,17 +146,14 @@
 <details>
   <summary>In addition to pypi, you can also install from source (click to expand)</summary>
 
 ```bash
 git clone https://github.com/imoneoi/openchat
 cd openchat
 
-pip3 install packaging ninja
-pip3 install --no-build-isolation "flash-attn<2"
-
 pip3 install --upgrade pip  # enable PEP 660 support
 pip3 install -e .
 ```
 </details>
 
 
 ## <a id="web-ui"></a> Web UI
```

### Comparing `ochat-3.1.0/SECURITY.md` & `ochat-3.1.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/assets/embeddings.svg` & `ochat-3.1.1/assets/embeddings.svg`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/assets/logo_new.png` & `ochat-3.1.1/assets/logo_new.png`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/assets/vicuna_gpt35.svg` & `ochat-3.1.1/assets/vicuna_gpt35.svg`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/assets/vicuna_gpt4.svg` & `ochat-3.1.1/assets/vicuna_gpt4.svg`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/docker-compose.yml` & `ochat-3.1.1/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/config/model_config.py` & `ochat-3.1.1/ochat/config/model_config.py`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/data/clean_sharegpt.py` & `ochat-3.1.1/ochat/data/clean_sharegpt.py`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/data/filter_language.py` & `ochat-3.1.1/ochat/data/filter_language.py`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/data/filter_sharegpt.py` & `ochat-3.1.1/ochat/data/filter_sharegpt.py`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/data/generate_dataset.py` & `ochat-3.1.1/ochat/data/generate_dataset.py`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/data/generate_dataset_orca.py` & `ochat-3.1.1/ochat/data/generate_dataset_orca.py`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/data/merge.py` & `ochat-3.1.1/ochat/data/merge.py`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/data/run_data_pipeline.sh` & `ochat-3.1.1/ochat/data/run_data_pipeline.sh`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/conversation_templates.py` & `ochat-3.1.1/ochat/evaluation/conversation_templates.py`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/boolean_expressions.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/boolean_expressions.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/causal_judgement.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/causal_judgement.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/date_understanding.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/date_understanding.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/disambiguation_qa.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/disambiguation_qa.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/dyck_languages.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/dyck_languages.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/formal_fallacies.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/formal_fallacies.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/geometric_shapes.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/geometric_shapes.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/hyperbaton.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/hyperbaton.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/logical_deduction_five_objects.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/logical_deduction_five_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/logical_deduction_seven_objects.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/logical_deduction_seven_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/logical_deduction_three_objects.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/logical_deduction_three_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/movie_recommendation.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/movie_recommendation.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/multistep_arithmetic_two.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/multistep_arithmetic_two.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/navigate.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/navigate.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/object_counting.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/object_counting.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/penguins_in_a_table.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/penguins_in_a_table.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/reasoning_about_colored_objects.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/reasoning_about_colored_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/ruin_names.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/ruin_names.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/salient_translation_error_detection.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/salient_translation_error_detection.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/snarks.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/snarks.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/sports_understanding.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/sports_understanding.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/temporal_sequences.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/temporal_sequences.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/tracking_shuffled_objects_five_objects.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/tracking_shuffled_objects_five_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/tracking_shuffled_objects_seven_objects.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/tracking_shuffled_objects_seven_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/tracking_shuffled_objects_three_objects.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/tracking_shuffled_objects_three_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/web_of_lies.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/web_of_lies.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/bbh/word_sorting.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/bbh/word_sorting.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/fs_cothub/gsm8k/gsm8k.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/fs_cothub/gsm8k/gsm8k.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/zs/agieval/aqua-rat.zero-shot.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/zs/agieval/aqua-rat.zero-shot.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/zs/agieval/logiqa-en.zero-shot.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/zs/agieval/logiqa-en.zero-shot.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/zs/agieval/lsat-ar.zero-shot.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/zs/agieval/lsat-ar.zero-shot.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/zs/agieval/lsat-lr.zero-shot.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/zs/agieval/lsat-lr.zero-shot.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/zs/agieval/lsat-rc.zero-shot.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/zs/agieval/lsat-rc.zero-shot.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/zs/agieval/sat-en-without-passage.zero-shot.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/zs/agieval/sat-en-without-passage.zero-shot.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/zs/agieval/sat-en.zero-shot.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/zs/agieval/sat-en.zero-shot.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/zs/agieval/sat-math.zero-shot.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/zs/agieval/sat-math.zero-shot.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/boolean_expressions.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/boolean_expressions.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/causal_judgment.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/causal_judgment.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/date_understanding.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/date_understanding.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/disambiguation_qa.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/disambiguation_qa.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/formal_fallacies_syllogisms_negation.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/formal_fallacies_syllogisms_negation.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/geometric_shapes.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/geometric_shapes.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/hyperbaton.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/hyperbaton.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/logical_deduction_five_objects.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/logical_deduction_five_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/logical_deduction_seven_objects.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/logical_deduction_seven_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/logical_deduction_three_objects.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/logical_deduction_three_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/movie_recommendation.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/movie_recommendation.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/navigate.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/navigate.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/penguins_in_a_table.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/penguins_in_a_table.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/reasoning_about_colored_objects.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/reasoning_about_colored_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/ruin_names.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/ruin_names.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/salient_translation_error_detection.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/salient_translation_error_detection.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/snarks.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/snarks.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/sports_understanding.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/sports_understanding.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/temporal_sequences.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/temporal_sequences.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/tracking_shuffled_objects_five_objects.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/tracking_shuffled_objects_five_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/tracking_shuffled_objects_seven_objects.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/tracking_shuffled_objects_seven_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/tracking_shuffled_objects_three_objects.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/tracking_shuffled_objects_three_objects.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/zs/bbh_mc_orca/web_of_lies.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/zs/bbh_mc_orca/web_of_lies.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/eval_data/zs/truthfulqa_orca/truthfulqa_mc.jsonl` & `ochat-3.1.1/ochat/evaluation/eval_data/zs/truthfulqa_orca/truthfulqa_mc.jsonl`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/match_answer.py` & `ochat-3.1.1/ochat/evaluation/match_answer.py`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/run_eval.py` & `ochat-3.1.1/ochat/evaluation/run_eval.py`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/evaluation/view_results.py` & `ochat-3.1.1/ochat/evaluation/view_results.py`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/experimental/generate_dataset_old.py` & `ochat-3.1.1/ochat/experimental/generate_dataset_old.py`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/experimental/sharegpt.ipynb` & `ochat-3.1.1/ochat/experimental/sharegpt.ipynb`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/experimental/test_multipack_dataloader.ipynb` & `ochat-3.1.1/ochat/experimental/test_multipack_dataloader.ipynb`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/experimental/text_length.ipynb` & `ochat-3.1.1/ochat/experimental/text_length.ipynb`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/experimental/train_alpaca.py` & `ochat-3.1.1/ochat/experimental/train_alpaca.py`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/experimental/verify_dataset.ipynb` & `ochat-3.1.1/ochat/experimental/verify_dataset.ipynb`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/experimental/verify_dataset_orca.ipynb` & `ochat-3.1.1/ochat/experimental/verify_dataset_orca.ipynb`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/models/unpadded_llama.py` & `ochat-3.1.1/ochat/models/unpadded_llama.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,16 +28,19 @@
 
 from transformers.activations import ACT2FN
 from transformers.modeling_outputs import CausalLMOutputWithPast
 from transformers.modeling_utils import PreTrainedModel
 from transformers.utils import logging
 from transformers.models.llama.configuration_llama import LlamaConfig
 
-from flash_attn.flash_attn_interface import flash_attn_unpadded_func
-from flash_attn.bert_padding import pad_input
+try:
+    from flash_attn.flash_attn_interface import flash_attn_unpadded_func
+    from flash_attn.bert_padding import pad_input
+except ImportError:
+    print ("FlashAttention not found. Install it if you need to train models.")
 
 
 logger = logging.get_logger(__name__)
 
 
 @torch.jit.script
 def weighted_cross_entropy(logits: torch.Tensor, labels: torch.Tensor, weights: torch.Tensor):
```

### Comparing `ochat-3.1.0/ochat/serving/async_tokenizer.py` & `ochat-3.1.1/ochat/serving/async_tokenizer.py`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/serving/openai_api_protocol.py` & `ochat-3.1.1/ochat/serving/openai_api_protocol.py`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/serving/openai_api_server.py` & `ochat-3.1.1/ochat/serving/openai_api_server.py`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/training_deepspeed/multipack_dataloader.py` & `ochat-3.1.1/ochat/training_deepspeed/multipack_dataloader.py`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/training_deepspeed/parquet_dataset.py` & `ochat-3.1.1/ochat/training_deepspeed/parquet_dataset.py`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat/training_deepspeed/train.py` & `ochat-3.1.1/ochat/training_deepspeed/train.py`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/ochat.egg-info/PKG-INFO` & `ochat-3.1.1/ochat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ochat
-Version: 3.1.0
+Version: 3.1.1
 Summary: An efficient framework for training and serving top-tier, open-source conversational LLMs.
 Project-URL: Homepage, https://github.com/imoneoi/openchat
 Project-URL: Bug Tracker, https://github.com/imoneoi/openchat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -50,15 +50,15 @@
 <details>
   <summary>Example request (click to expand)</summary>
 
 ```bash
 curl http://localhost:18888/v1/chat/completions \
   -H "Content-Type: application/json" \
   -d '{
-    "model": "openchat_v3.1_llama2",
+    "model": "openchat_v3.2",
     "messages": [{"role": "user", "content": "You are a large language model named OpenChat. Write a poem to describe yourself"}]
   }'
 ```
 
 </details>
 
 | Model        | Size | Context | Weights                                                      | Serving                                                                                                                                                                      |
@@ -67,38 +67,38 @@
 | OpenChat 3.1 | 13B  | 4096    | [Huggingface](https://huggingface.co/openchat/openchat_v3.1) | `python -m ochat.serving.openai_api_server --model-type openchat_v3.1_llama2 --model openchat/openchat_v3.1 --engine-use-ray --worker-use-ray --max-num-batched-tokens 5120` |
 
 For inference with Huggingface Transformers (slow and not recommended), follow the conversation template provided below:
 
 <details>
   <summary>Conversation templates (click to expand)</summary>
 
-V3.1
-
-```python
-# Single-turn V3.1
-tokenize("Assistant is GPT4<|end_of_turn|>User: Hello<|end_of_turn|>Assistant:")
-# Result: [1, 4007, 22137, 338, 402, 7982, 29946, 32000, 4911, 29901, 15043, 32000, 4007, 22137, 29901]
-
-# Multi-turn V3.1
-tokenize("Assistant is GPT4<|end_of_turn|>User: Hello<|end_of_turn|>Assistant: Hi<|end_of_turn|>User: How are you today?<|end_of_turn|>Assistant:")
-# Result: [1, 4007, 22137, 338, 402, 7982, 29946, 32000, 4911, 29901, 15043, 32000, 4007, 22137, 29901, 6324, 32000, 4911, 29901, 1128, 526, 366, 9826, 29973, 32000, 4007, 22137, 29901]
-```
-
 V3.2
 
 ```python
 # Single-turn V3.2
 tokenize("GPT4 User: Hello<|end_of_turn|>GPT4 Assistant:")
 # Result: [1, 402, 7982, 29946, 4911, 29901, 15043, 32000, 402, 7982, 29946, 4007, 22137, 29901]
 
 # Multi-turn V3.2
 tokenize("GPT4 User: Hello<|end_of_turn|>GPT4 Assistant: Hi<|end_of_turn|>GPT4 User: How are you today?<|end_of_turn|>GPT4 Assistant:")
 # Result: [1, 402, 7982, 29946, 4911, 29901, 15043, 32000, 402, 7982, 29946, 4007, 22137, 29901, 6324, 32000, 402, 7982, 29946, 4911, 29901, 1128, 526, 366, 9826, 29973, 32000, 402, 7982, 29946, 4007, 22137, 29901]
 ```
 
+V3.1
+
+```python
+# Single-turn V3.1
+tokenize("Assistant is GPT4<|end_of_turn|>User: Hello<|end_of_turn|>Assistant:")
+# Result: [1, 4007, 22137, 338, 402, 7982, 29946, 32000, 4911, 29901, 15043, 32000, 4007, 22137, 29901]
+
+# Multi-turn V3.1
+tokenize("Assistant is GPT4<|end_of_turn|>User: Hello<|end_of_turn|>Assistant: Hi<|end_of_turn|>User: How are you today?<|end_of_turn|>Assistant:")
+# Result: [1, 4007, 22137, 338, 402, 7982, 29946, 32000, 4911, 29901, 15043, 32000, 4007, 22137, 29901, 6324, 32000, 4911, 29901, 1128, 526, 366, 9826, 29973, 32000, 4007, 22137, 29901]
+```
+
 </details>
 
 ## <a id="benchmarks"></a> Benchmarks
 
 We have evaluated our models using the two most popular evaluation benchmarks **, including AlpacaEval and MT-bench. Here we list the top models with our released versions, sorted by model size in descending order. The full version can be found on the [MT-bench](https://chat.lmsys.org/?leaderboard) and [AlpacaEval](https://tatsu-lab.github.io/alpaca_eval/) leaderboards.
 
 To ensure consistency, we used the same routine as ChatGPT / GPT-4 to run these benchmarks. We started the OpenAI API-compatible server and set the `openai.api_base` to `http://localhost:18888/v1` in the benchmark program.
@@ -122,24 +122,28 @@
 
 🚀 To ensure comprehensive evaluation of large language models (LLMs), we are working on developing a suite of accelerated standard benchmarks, including AGIEval, BBH, and Chain-of-Thought Hub, named vLLM Eval. This suite leverages the speedup provided by [vLLM](https://github.com/vllm-project/vllm) and allows us to finish the entire benchmark in just 5 minutes.
 
 We will release the evaluation results as soon as they become available, so stay tuned!
 
 ## <a id="installation"></a> Installation
 
-To use OpenChat, you need to install CUDA and PyTorch, then install FlashAttention 1. After that you can install OpenChat via pip:
+To use OpenChat, you need to install CUDA and PyTorch, then you can install OpenChat via pip:
+
+```bash
+pip3 install ochat
+```
+
+If you want to train models, please also install FlashAttention 1.
 
 ```bash
 pip3 install packaging ninja
 pip3 install --no-build-isolation "flash-attn<2"
-
-pip3 install ochat
 ```
 
-FlashAttention may have compatibility issues. If you encounter these problems, you can try to create a new `conda` environment following the instructions below.
+FlashAttention and vLLM may have compatibility issues. If you encounter these problems, you can try to create a new `conda` environment following the instructions below.
 
 ```bash
 conda create -y --name openchat
 conda activate openchat
 
 conda install -y python
 conda install -y cudatoolkit-dev -c conda-forge
@@ -154,17 +158,14 @@
 <details>
   <summary>In addition to pypi, you can also install from source (click to expand)</summary>
 
 ```bash
 git clone https://github.com/imoneoi/openchat
 cd openchat
 
-pip3 install packaging ninja
-pip3 install --no-build-isolation "flash-attn<2"
-
 pip3 install --upgrade pip  # enable PEP 660 support
 pip3 install -e .
 ```
 </details>
 
 
 ## <a id="web-ui"></a> Web UI
```

### Comparing `ochat-3.1.0/ochat.egg-info/SOURCES.txt` & `ochat-3.1.1/ochat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ochat-3.1.0/pyproject.toml` & `ochat-3.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     "datasets", 
     "orjson", 
     "torch", 
     "ray", 
     "sentencepiece", 
     "transformers", 
     "accelerate", 
-    "flash-attn<2", 
     "protobuf<3.21", 
     "fastapi", 
     "pydantic", 
     "shortuuid", 
     "uvicorn", 
     "vllm"
 ]
```

