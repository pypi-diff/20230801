# Comparing `tmp/ibm-generative-ai-0.2.3.tar.gz` & `tmp/ibm-generative-ai-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibm-generative-ai-0.2.3.tar", last modified: Mon Jul 24 16:54:37 2023, max compression
+gzip compressed data, was "ibm-generative-ai-0.2.4.tar", last modified: Tue Aug  1 14:18:43 2023, max compression
```

## Comparing `ibm-generative-ai-0.2.3.tar` & `ibm-generative-ai-0.2.4.tar`

### file list

```diff
@@ -1,270 +1,270 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.628311 ibm-generative-ai-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.584310 ibm-generative-ai-0.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.584310 ibm-generative-ai-0.2.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/.github/ISSUE_TEMPLATE/01_bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/.github/ISSUE_TEMPLATE/02_feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/.github/ISSUE_TEMPLATE/03_documentation_update.md
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/.github/ISSUE_TEMPLATE/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.584310 ibm-generative-ai-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/.github/workflows/documentation.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/.github/workflows/integration-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/EXTENSIONS.md
--rw-r--r--   0 runner    (1001) docker     (123)    10494 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/GETTING_STARTED.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-24 16:54:37.628311 ibm-generative-ai-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/STARTER_TEAM.md
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/SUPPORT.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.584310 ibm-generative-ai-0.2.3/documentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/.nojekyll
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.584310 ibm-generative-ai-0.2.3/documentation/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    39195 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/assets/pull_request_from_fork_to_base.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.588310 ibm-generative-ai-0.2.3/documentation/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.588310 ibm-generative-ai-0.2.3/documentation/docs/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.588310 ibm-generative-ai-0.2.3/documentation/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.588310 ibm-generative-ai-0.2.3/documentation/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.588310 ibm-generative-ai-0.2.3/documentation/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/_templates/custom_landing_page.html
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.592310 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.592310 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/examples/async.examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/examples/async.examples.user.rst
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/examples/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/examples/examples.user.rst
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/examples/extensions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/examples/extensions.user.rst
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/examples/prompts.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/examples/prompts.user.rst
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.credentials.rst
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.exceptions.genai_exception.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.metadata.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.model.rst
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.prompt.prompt_pattern.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.prompt.quickstart.annexe.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9306 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.prompt.quickstart.basics.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.prompt.quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.prompt.rst
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.rst
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.schemas.descriptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.schemas.files_params.rst
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.schemas.generate_params.rst
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.schemas.history_params.rst
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.schemas.responses.rst
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.schemas.rst
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.schemas.token_params.rst
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.schemas.tunes_params.rst
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.services.request_handler.rst
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.services.rst
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.services.service_interface.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/local_server.rst
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.576309 ibm-generative-ai-0.2.3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.596310 ibm-generative-ai-0.2.3/examples/dev/
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/dev/async-flaky-request-handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/dev/async-flaky-responses-ordered.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/dev/generate-all-models.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/dev/history-async.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/dev/load_token_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/dev/logging_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.600310 ibm-generative-ai-0.2.3/examples/user/
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/alice_bob_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/alice_bob_talk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.604310 ibm-generative-ai-0.2.3/examples/user/assets/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/assets/country-capital.csv
--rw-r--r--   0 runner    (1001) docker     (123)    19258 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/assets/penguins.csv
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/assets/penguins2.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/assets/seed_tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)   110931 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/assets/seed_tasks.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/async_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/async_greetings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/async_ordered.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/async_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/complete_my_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/country-capital-qa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/explain_my_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/generate_with_input_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/gpt_chat_bash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/grid_search_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/grid_search_params_greeating.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/jsonprompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/jsonprompt_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/langchain_qa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.604310 ibm-generative-ai-0.2.3/examples/user/localserver/
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/localserver/localserver.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/localserver/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/logprob_returns.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/many_greetings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/model_as_string.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/model_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/prompt-raw-string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/prompt_csv_random_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/prompt_from_all_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/prompt_from_all_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/prompt_from_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/prompt_reuse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.604310 ibm-generative-ai-0.2.3/examples/user/prompt_templating/
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/prompt_templating/watsonx-prompt-output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/prompt_templating/watsonx-prompt-pattern-ux-async.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/prompt_templating/watsonx-prompt-pattern-ux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/prompt_templating/watsonx-prompt-templating.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.604310 ibm-generative-ai-0.2.3/examples/user/prompt_tuning/
--rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/prompt_tuning/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/prompt_tuning/file_to_tune.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/prompt_tuning/files_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/prompt_tuning/summarization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.604310 ibm-generative-ai-0.2.3/examples/user/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/prompts/Country-Capital-Factual-QA
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.604310 ibm-generative-ai-0.2.3/examples/user/prompts_adult_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/prompts_adult_dataset/prompt_generation_with_column_idx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/prompts_adult_dataset/prompt_generation_with_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/saving_prompts_as_hf_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/self-reflection.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/self_instruct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/streaming.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.608311 ibm-generative-ai-0.2.3/examples/user/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/templates/capital-qa.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/templates/instruction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/templates/qa.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/templates/self-reflection.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/templates/synth-animal.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/tokenize-sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/examples/user/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 16:54:37.628311 ibm-generative-ai-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.580309 ibm-generative-ai-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.608311 ibm-generative-ai-0.2.3/src/genai/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-24 16:54:37.000000 ibm-generative-ai-0.2.3/src/genai/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.608311 ibm-generative-ai-0.2.3/src/genai/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/exceptions/genai_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.580309 ibm-generative-ai-0.2.3/src/genai/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.608311 ibm-generative-ai-0.2.3/src/genai/extensions/huggingface/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/extensions/huggingface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/extensions/huggingface/save_huggingface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.608311 ibm-generative-ai-0.2.3/src/genai/extensions/langchain/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/extensions/langchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/extensions/langchain/llm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/extensions/langchain/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.612311 ibm-generative-ai-0.2.3/src/genai/extensions/localserver/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/extensions/localserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/extensions/localserver/custom_model_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/extensions/localserver/local_api_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/extensions/localserver/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.612311 ibm-generative-ai-0.2.3/src/genai/extensions/pandas/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/extensions/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/extensions/pandas/prompt_sub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    16392 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    24219 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/prompt_pattern.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.612311 ibm-generative-ai-0.2.3/src/genai/routers/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/routers/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/routers/prompt_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/routers/tunes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.612311 ibm-generative-ai-0.2.3/src/genai/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7887 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/schemas/descriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/schemas/files_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/schemas/generate_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/schemas/history_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/schemas/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/schemas/token_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/schemas/tunes_params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.616311 ibm-generative-ai-0.2.3/src/genai/services/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/services/async_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/services/connection_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/services/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/services/prompt_template_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    12951 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/services/request_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/services/service_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/services/tune_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.616311 ibm-generative-ai-0.2.3/src/genai/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/utils/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/utils/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/utils/request_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/utils/search_space_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/utils/service_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/src/genai/utils/watsonx_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.616311 ibm-generative-ai-0.2.3/src/ibm_generative_ai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-24 16:54:37.000000 ibm-generative-ai-0.2.3/src/ibm_generative_ai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-07-24 16:54:37.000000 ibm-generative-ai-0.2.3/src/ibm_generative_ai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 16:54:37.000000 ibm-generative-ai-0.2.3/src/ibm_generative_ai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-24 16:54:37.000000 ibm-generative-ai-0.2.3/src/ibm_generative_ai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 16:54:37.000000 ibm-generative-ai-0.2.3/src/ibm_generative_ai.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.620311 ibm-generative-ai-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.624311 ibm-generative-ai-0.2.3/tests/assets/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/assets/age-gender.csv
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/assets/capital-qa-content.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/assets/capital-qa-multivar.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/assets/capital-qa-sub-noheader.csv
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/assets/capital-qa-sub.csv
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/assets/capital-qa-sub.json
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/assets/capital-qa-sub.txt
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/assets/capital-qa.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/assets/csv_file.csv
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/assets/csv_file.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/assets/file_to_tune.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/assets/file_to_tune.json
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/assets/file_to_tune.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/assets/invalid-content-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/assets/invalid-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/assets/penguins.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/assets/prompt_contents.csv
--rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/assets/response_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/assets/story.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/assets/story_sub.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.628311 ibm-generative-ai-0.2.3/tests/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/extensions/test_langchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/extensions/test_localserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/extensions/test_save_huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/extensions/test_sub_from_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:37.628311 ibm-generative-ai-0.2.3/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/integration/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/integration/test_terms_of_use.py
--rw-r--r--   0 runner    (1001) docker     (123)    19430 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_concurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     9487 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    10998 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_generate_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_generate_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_json_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_model_async.py
--rw-r--r--   0 runner    (1001) docker     (123)    14265 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_prompt_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_prompt_pattern_watsonx.py
--rw-r--r--   0 runner    (1001) docker     (123)    12442 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_prompt_template_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_schema_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_service_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_service_interface_async.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_service_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_tunes.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-24 16:53:58.000000 ibm-generative-ai-0.2.3/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:18:43.881956 ibm-generative-ai-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:18:43.841955 ibm-generative-ai-0.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:18:43.841955 ibm-generative-ai-0.2.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/.github/ISSUE_TEMPLATE/01_bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/.github/ISSUE_TEMPLATE/02_feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/.github/ISSUE_TEMPLATE/03_documentation_update.md
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/.github/ISSUE_TEMPLATE/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:18:43.841955 ibm-generative-ai-0.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/.github/workflows/documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/.github/workflows/integration-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/EXTENSIONS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10546 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/GETTING_STARTED.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-08-01 14:18:43.881956 ibm-generative-ai-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/STARTER_TEAM.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/SUPPORT.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:18:43.841955 ibm-generative-ai-0.2.4/documentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/.nojekyll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:18:43.841955 ibm-generative-ai-0.2.4/documentation/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    39195 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/assets/pull_request_from_fork_to_base.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:18:43.841955 ibm-generative-ai-0.2.4/documentation/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:18:43.841955 ibm-generative-ai-0.2.4/documentation/docs/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/docs/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:18:43.841955 ibm-generative-ai-0.2.4/documentation/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:18:43.841955 ibm-generative-ai-0.2.4/documentation/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/docs/source/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:18:43.841955 ibm-generative-ai-0.2.4/documentation/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/docs/source/_templates/custom_landing_page.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:18:43.849955 ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:18:43.849955 ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/examples/async.examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/examples/async.examples.user.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/examples/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/examples/examples.user.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/examples/extensions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/examples/extensions.user.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/examples/prompts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/examples/prompts.user.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/genai.credentials.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/genai.exceptions.genai_exception.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/genai.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/genai.metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/genai.model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/genai.prompt.prompt_pattern.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/genai.prompt.quickstart.annexe.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9306 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/genai.prompt.quickstart.basics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/genai.prompt.quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/genai.prompt.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/genai.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/genai.schemas.descriptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/genai.schemas.files_params.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/genai.schemas.generate_params.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/genai.schemas.history_params.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/genai.schemas.responses.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/genai.schemas.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/genai.schemas.token_params.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/genai.schemas.tunes_params.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/genai.services.request_handler.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/genai.services.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/genai.services.service_interface.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/local_server.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:18:43.833955 ibm-generative-ai-0.2.4/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:18:43.849955 ibm-generative-ai-0.2.4/examples/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/dev/async-flaky-request-handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/dev/async-flaky-responses-ordered.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/dev/generate-all-models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/dev/history-async.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/dev/load_token_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/dev/logging_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:18:43.857955 ibm-generative-ai-0.2.4/examples/user/
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/alice_bob_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/alice_bob_talk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:18:43.857955 ibm-generative-ai-0.2.4/examples/user/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/assets/country-capital.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    19258 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/assets/penguins.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/assets/penguins2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/assets/seed_tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)   110931 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/assets/seed_tasks.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/async_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/async_greetings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/async_ordered.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/async_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/complete_my_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/country-capital-qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/explain_my_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/generate_with_input_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/gpt_chat_bash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/grid_search_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/grid_search_params_greeating.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/jsonprompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/jsonprompt_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/langchain_qa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:18:43.857955 ibm-generative-ai-0.2.4/examples/user/localserver/
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/localserver/localserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/localserver/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/logprob_returns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/many_greetings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/model_as_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/prompt-raw-string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/prompt_csv_random_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/prompt_from_all_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/prompt_from_all_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/prompt_from_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/prompt_reuse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:18:43.861956 ibm-generative-ai-0.2.4/examples/user/prompt_templating/
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/prompt_templating/watsonx-prompt-output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/prompt_templating/watsonx-prompt-pattern-ux-async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/prompt_templating/watsonx-prompt-pattern-ux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/prompt_templating/watsonx-prompt-templating.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:18:43.861956 ibm-generative-ai-0.2.4/examples/user/prompt_tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/prompt_tuning/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/prompt_tuning/file_to_tune.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/prompt_tuning/files_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/prompt_tuning/summarization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:18:43.861956 ibm-generative-ai-0.2.4/examples/user/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/prompts/Country-Capital-Factual-QA
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:18:43.861956 ibm-generative-ai-0.2.4/examples/user/prompts_adult_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/prompts_adult_dataset/prompt_generation_with_column_idx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/prompts_adult_dataset/prompt_generation_with_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/saving_prompts_as_hf_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/self-reflection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/self_instruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/streaming.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:18:43.861956 ibm-generative-ai-0.2.4/examples/user/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/templates/capital-qa.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/templates/instruction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/templates/qa.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/templates/self-reflection.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/templates/synth-animal.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/tokenize-sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/examples/user/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 14:18:43.881956 ibm-generative-ai-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:18:43.837955 ibm-generative-ai-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:18:43.865956 ibm-generative-ai-0.2.4/src/genai/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-01 14:18:43.000000 ibm-generative-ai-0.2.4/src/genai/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:18:43.865956 ibm-generative-ai-0.2.4/src/genai/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/exceptions/genai_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:18:43.837955 ibm-generative-ai-0.2.4/src/genai/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:18:43.865956 ibm-generative-ai-0.2.4/src/genai/extensions/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/extensions/huggingface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/extensions/huggingface/save_huggingface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:18:43.865956 ibm-generative-ai-0.2.4/src/genai/extensions/langchain/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/extensions/langchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/extensions/langchain/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/extensions/langchain/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:18:43.865956 ibm-generative-ai-0.2.4/src/genai/extensions/localserver/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/extensions/localserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/extensions/localserver/custom_model_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/extensions/localserver/local_api_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/extensions/localserver/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:18:43.865956 ibm-generative-ai-0.2.4/src/genai/extensions/pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/extensions/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/extensions/pandas/prompt_sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16392 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24219 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/prompt_pattern.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:18:43.865956 ibm-generative-ai-0.2.4/src/genai/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/routers/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/routers/prompt_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/routers/tunes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:18:43.869956 ibm-generative-ai-0.2.4/src/genai/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/schemas/descriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/schemas/files_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/schemas/generate_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/schemas/history_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/schemas/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/schemas/token_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/schemas/tunes_params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:18:43.869956 ibm-generative-ai-0.2.4/src/genai/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/services/async_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/services/connection_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/services/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/services/prompt_template_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12951 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/services/request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/services/service_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/services/tune_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:18:43.869956 ibm-generative-ai-0.2.4/src/genai/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/utils/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/utils/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/utils/request_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/utils/search_space_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/utils/service_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/src/genai/utils/watsonx_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:18:43.873956 ibm-generative-ai-0.2.4/src/ibm_generative_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-08-01 14:18:43.000000 ibm-generative-ai-0.2.4/src/ibm_generative_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-08-01 14:18:43.000000 ibm-generative-ai-0.2.4/src/ibm_generative_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:18:43.000000 ibm-generative-ai-0.2.4/src/ibm_generative_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-08-01 14:18:43.000000 ibm-generative-ai-0.2.4/src/ibm_generative_ai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 14:18:43.000000 ibm-generative-ai-0.2.4/src/ibm_generative_ai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:18:43.877956 ibm-generative-ai-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:18:43.881956 ibm-generative-ai-0.2.4/tests/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/assets/age-gender.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/assets/capital-qa-content.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/assets/capital-qa-multivar.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/assets/capital-qa-sub-noheader.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/assets/capital-qa-sub.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/assets/capital-qa-sub.json
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/assets/capital-qa-sub.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/assets/capital-qa.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/assets/csv_file.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/assets/csv_file.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/assets/file_to_tune.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/assets/file_to_tune.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/assets/file_to_tune.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/assets/invalid-content-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/assets/invalid-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/assets/penguins.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/assets/prompt_contents.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/assets/response_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/assets/story.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/assets/story_sub.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:18:43.881956 ibm-generative-ai-0.2.4/tests/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/extensions/test_langchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/extensions/test_localserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/extensions/test_save_huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/extensions/test_sub_from_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:18:43.881956 ibm-generative-ai-0.2.4/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/integration/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/integration/test_terms_of_use.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19433 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/test_concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9487 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/test_generate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/test_generate_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/test_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/test_json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/test_model_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14265 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/test_prompt_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/test_prompt_pattern_watsonx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12442 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/test_prompt_template_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/test_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/test_schema_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/test_service_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/test_service_interface_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/test_service_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/test_tunes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-01 14:17:51.000000 ibm-generative-ai-0.2.4/tests/test_version.py
```

### Comparing `ibm-generative-ai-0.2.3/.github/ISSUE_TEMPLATE/01_bug_report.md` & `ibm-generative-ai-0.2.4/.github/ISSUE_TEMPLATE/01_bug_report.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/.github/ISSUE_TEMPLATE/02_feature_request.md` & `ibm-generative-ai-0.2.4/.github/ISSUE_TEMPLATE/02_feature_request.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/.github/ISSUE_TEMPLATE/03_documentation_update.md` & `ibm-generative-ai-0.2.4/.github/ISSUE_TEMPLATE/03_documentation_update.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/.github/PULL_REQUEST_TEMPLATE.md` & `ibm-generative-ai-0.2.4/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/.github/workflows/documentation.yml` & `ibm-generative-ai-0.2.4/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/.github/workflows/integration-test.yml` & `ibm-generative-ai-0.2.4/.github/workflows/integration-test.yml`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/.github/workflows/main.yml` & `ibm-generative-ai-0.2.4/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/.github/workflows/python-publish.yml` & `ibm-generative-ai-0.2.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/.gitignore` & `ibm-generative-ai-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/.pre-commit-config.yaml` & `ibm-generative-ai-0.2.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/CODE_OF_CONDUCT.md` & `ibm-generative-ai-0.2.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/CONTRIBUTING.md` & `ibm-generative-ai-0.2.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/EXTENSIONS.md` & `ibm-generative-ai-0.2.4/EXTENSIONS.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/GETTING_STARTED.md` & `ibm-generative-ai-0.2.4/GETTING_STARTED.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # Getting Started Guideline
 
 ## <a name='TableofContents'></a>Table of Contents
 
-* [Table of Contents](#table-of-contents)
-* [Installation](#installation)
-* [Gen AI Endpoint](#gen-ai-endpoint)
-    * [Example](#example)
-* [Examples](#examples)
-    * [Async Example](#async-example)
-    * [Synchronous Example](#synchronous-example)
-* [Tips and Troubleshooting](#tips-and-troubleshooting)
-    * [Model Availability](#model-availability)
-    * [Enabling Logs](#enabling-logs)
-    * [Experimenting with a Large Number of Prompts](#many-prompts)
-* [Extensions](#extensions)
-    * [LangChain Extension](#langchain-extension)
-* [Support](#support)
+- [Table of Contents](#table-of-contents)
+- [Installation](#installation)
+- [Gen AI Endpoint](#gen-ai-endpoint)
+  - [Example](#example)
+- [Examples](#examples)
+  - [Async Example](#async-example)
+  - [Synchronous Example](#synchronous-example)
+- [Tips and Troubleshooting](#tips-and-troubleshooting)
+  - [Model Availability](#model-availability)
+  - [Enabling Logs](#enabling-logs)
+  - [Experimenting with a Large Number of Prompts](#many-prompts)
+- [Extensions](#extensions)
+  - [LangChain Extension](#langchain-extension)
+- [Support](#support)
 
 ## <a name='Installation'></a>Installation
 
 ```bash
 pip install ibm-generative-ai
 ```
 
@@ -53,15 +53,15 @@
 ```
 
 ```python
 import os
 
 from dotenv import load_dotenv
 
-from genai.model import Credentials
+from genai.credentials import Credentials
 
 # make sure you have a .env file under genai root with
 # GENAI_KEY=<your-genai-key>
 # GENAI_API=<genai-api-endpoint>
 load_dotenv()
 my_api_key = os.getenv("GENAI_KEY", None)
 my_api_endpoint = os.getenv("GENAI_API", None)
@@ -86,15 +86,16 @@
 ### <a name='AsyncExample'></a>Async Example
 
 ```python
 import os
 
 from dotenv import load_dotenv
 
-from genai.model import Credentials, Model
+from genai.credentials import Credentials
+from genai.model import Model
 from genai.schemas import GenerateParams
 
 # make sure you have a .env file under genai root with
 # GENAI_KEY=<your-genai-key>
 # GENAI_API=<genai-api-endpoint>
 load_dotenv()
 api_key = os.getenv("GENAI_KEY", None)
@@ -140,15 +141,16 @@
 ### <a name='SynchronousExample'></a>Synchronous Example
 
 ```python
 import os
 
 from dotenv import load_dotenv
 
-from genai.model import Credentials, Model
+from genai.credentials import Credentials
+from genai.model import Model
 from genai.schemas import GenerateParams
 
 # make sure you have a .env file under genai root with
 # GENAI_KEY=<your-genai-key>
 # GENAI_API=<genai-api-endpoint>
 load_dotenv()
 api_key = os.getenv("GENAI_KEY", None)
@@ -182,15 +184,17 @@
     print(f"Generated text: {response.generated_text}")
 
 ```
 
 ## <a name='TipsAndTroubleshooting'></a>Tips and Troubleshooting
 
 ### <a name='Model Availability'></a>Model Availability
+
 To test the reachability of your endpoint and availability of desired model, use the following utility script with your model details:
+
 ```python
 import os
 
 from dotenv import load_dotenv
 
 from genai.credentials import Credentials
 from genai.model import Model
```

### Comparing `ibm-generative-ai-0.2.3/LICENSE` & `ibm-generative-ai-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/PKG-INFO` & `ibm-generative-ai-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibm-generative-ai
-Version: 0.2.3
+Version: 0.2.4
 Summary: IBM Generative AI is a Python library built on IBM's large language model REST interface.
 Author-email: Lee Martie <lee.martie@ibm.com>, Ana Fucs <ana.fucs@ibm.com>, Veronique Demers <vdemers@ibm.com>, Mairead O'Neill <moneill@ibm.com>, Mirian Silva <mirianfrsilva@ibm.com>, Onkar Bhardwaj <onkarbhardwaj@ibm.com>, James Sutton <james.sutton@uk.ibm.com>, Ja Young Lee <younglee@ibm.com>, Adriana Meza Soria <adriana.meza.soria@ibm.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: langchain
 Provides-Extra: huggingface
```

### Comparing `ibm-generative-ai-0.2.3/README.md` & `ibm-generative-ai-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/STARTER_TEAM.md` & `ibm-generative-ai-0.2.4/STARTER_TEAM.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/SUPPORT.md` & `ibm-generative-ai-0.2.4/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/documentation/assets/pull_request_from_fork_to_base.png` & `ibm-generative-ai-0.2.4/documentation/assets/pull_request_from_fork_to_base.png`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/documentation/docs/Makefile` & `ibm-generative-ai-0.2.4/documentation/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/documentation/docs/make.bat` & `ibm-generative-ai-0.2.4/documentation/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/documentation/docs/source/_templates/custom_landing_page.html` & `ibm-generative-ai-0.2.4/documentation/docs/source/_templates/custom_landing_page.html`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/documentation/docs/source/conf.py` & `ibm-generative-ai-0.2.4/documentation/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/documentation/docs/source/index.rst` & `ibm-generative-ai-0.2.4/documentation/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/examples/async.examples.user.rst` & `ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/examples/async.examples.user.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/examples/examples.user.rst` & `ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/examples/examples.user.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/examples/extensions.user.rst` & `ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/examples/extensions.user.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/examples/prompts.user.rst` & `ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/examples/prompts.user.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.prompt.quickstart.annexe.rst` & `ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/genai.prompt.quickstart.annexe.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.prompt.quickstart.basics.rst` & `ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/genai.prompt.quickstart.basics.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/genai.prompt.quickstart.rst` & `ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/genai.prompt.quickstart.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/documentation/docs/source/rst_source/local_server.rst` & `ibm-generative-ai-0.2.4/documentation/docs/source/rst_source/local_server.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/dev/async-flaky-request-handler.py` & `ibm-generative-ai-0.2.4/examples/dev/async-flaky-request-handler.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/dev/async-flaky-responses-ordered.py` & `ibm-generative-ai-0.2.4/examples/dev/async-flaky-responses-ordered.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/dev/generate-all-models.py` & `ibm-generative-ai-0.2.4/examples/dev/generate-all-models.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/dev/history-async.py` & `ibm-generative-ai-0.2.4/examples/dev/history-async.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/dev/logging_example.py` & `ibm-generative-ai-0.2.4/examples/dev/logging_example.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/alice_bob_qa.py` & `ibm-generative-ai-0.2.4/examples/user/alice_bob_qa.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/alice_bob_talk.py` & `ibm-generative-ai-0.2.4/examples/user/alice_bob_talk.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/assets/penguins.csv` & `ibm-generative-ai-0.2.4/examples/user/assets/penguins.csv`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/assets/penguins2.csv` & `ibm-generative-ai-0.2.4/examples/user/assets/penguins2.csv`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/assets/seed_tasks.json` & `ibm-generative-ai-0.2.4/examples/user/assets/seed_tasks.json`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/assets/seed_tasks.jsonl` & `ibm-generative-ai-0.2.4/examples/user/assets/seed_tasks.jsonl`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/async_callback.py` & `ibm-generative-ai-0.2.4/examples/user/async_callback.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/async_greetings.py` & `ibm-generative-ai-0.2.4/examples/user/async_greetings.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/async_ordered.py` & `ibm-generative-ai-0.2.4/examples/user/async_ordered.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/async_tokenize.py` & `ibm-generative-ai-0.2.4/examples/user/async_tokenize.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/complete_my_code.py` & `ibm-generative-ai-0.2.4/examples/user/complete_my_code.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/country-capital-qa.py` & `ibm-generative-ai-0.2.4/examples/user/country-capital-qa.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/explain_my_code.py` & `ibm-generative-ai-0.2.4/examples/user/explain_my_code.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/generate_with_input_text.py` & `ibm-generative-ai-0.2.4/examples/user/generate_with_input_text.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/gpt_chat_bash.py` & `ibm-generative-ai-0.2.4/examples/user/gpt_chat_bash.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/grid_search_params.py` & `ibm-generative-ai-0.2.4/examples/user/grid_search_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     "decoding_method": ["sample"],
     "max_new_tokens": [10, 20],
     "min_new_tokens": [1, 2],
     "temperature": [0.7, 0.8, 0.9, 1.5],
 }
 
 creds = Credentials(api_key=API_KEY, api_endpoint=API_ENDPOINT)
-pt = PromptPattern.from_str("The capital of {{country}} is {{capital}}. The capital of Taiwan is")
+pt = PromptPattern.from_str("The capital of {{country}} is {{capital}}. The capital of Canada is")
 pt.sub("capital", "Madrid").sub("country", "Spain")
 
 # generate all combinations of parameters, returns a list of GenerateParams
 generate_params_list = grid_search_generate_params(my_space_params)
 
 for params in generate_params_list:
     model = Model("google/flan-t5-xxl", params=params, credentials=creds)
```

### Comparing `ibm-generative-ai-0.2.3/examples/user/grid_search_params_greeating.py` & `ibm-generative-ai-0.2.4/examples/user/grid_search_params_greeating.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/history.py` & `ibm-generative-ai-0.2.4/examples/user/history.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/jsonprompt.py` & `ibm-generative-ai-0.2.4/examples/user/jsonprompt.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/jsonprompt_multi.py` & `ibm-generative-ai-0.2.4/examples/user/jsonprompt_multi.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/langchain_qa.py` & `ibm-generative-ai-0.2.4/examples/user/langchain_qa.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/localserver/localserver.py` & `ibm-generative-ai-0.2.4/examples/user/localserver/localserver.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/logprob_returns.py` & `ibm-generative-ai-0.2.4/examples/user/logprob_returns.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/many_greetings.py` & `ibm-generative-ai-0.2.4/examples/user/many_greetings.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/model_as_string.py` & `ibm-generative-ai-0.2.4/examples/user/model_as_string.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/model_utils.py` & `ibm-generative-ai-0.2.4/examples/user/model_utils.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/prompt-raw-string.py` & `ibm-generative-ai-0.2.4/examples/user/prompt-raw-string.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/prompt_csv_random_rows.py` & `ibm-generative-ai-0.2.4/examples/user/prompt_csv_random_rows.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/prompt_from_all_csv.py` & `ibm-generative-ai-0.2.4/examples/user/prompt_from_all_csv.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/prompt_from_all_dataframe.py` & `ibm-generative-ai-0.2.4/examples/user/prompt_from_all_dataframe.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/prompt_from_dataframe.py` & `ibm-generative-ai-0.2.4/examples/user/prompt_from_dataframe.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/prompt_reuse.py` & `ibm-generative-ai-0.2.4/examples/user/prompt_reuse.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/prompt_templating/watsonx-prompt-output.py` & `ibm-generative-ai-0.2.4/examples/user/prompt_templating/watsonx-prompt-output.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/prompt_templating/watsonx-prompt-pattern-ux-async.py` & `ibm-generative-ai-0.2.4/examples/user/prompt_templating/watsonx-prompt-pattern-ux-async.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/prompt_templating/watsonx-prompt-pattern-ux.py` & `ibm-generative-ai-0.2.4/examples/user/prompt_templating/watsonx-prompt-pattern-ux.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/prompt_templating/watsonx-prompt-templating.py` & `ibm-generative-ai-0.2.4/examples/user/prompt_templating/watsonx-prompt-templating.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 from dotenv import load_dotenv
 
-from genai.model import Credentials
+from genai.credentials import Credentials
 from genai.prompt_pattern import PromptPattern
 from genai.schemas import TokenParams
 from genai.services.prompt_template_manager import PromptTemplateManager
 
 # make sure you have a .env file under genai root with
 # GENAI_KEY=<your-genai-key>
 load_dotenv()
```

### Comparing `ibm-generative-ai-0.2.3/examples/user/prompt_tuning/classification.py` & `ibm-generative-ai-0.2.4/examples/user/prompt_tuning/classification.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/prompt_tuning/file_to_tune.jsonl` & `ibm-generative-ai-0.2.4/examples/user/prompt_tuning/file_to_tune.jsonl`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/prompt_tuning/files_manager.py` & `ibm-generative-ai-0.2.4/examples/user/prompt_tuning/files_manager.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/prompt_tuning/summarization.py` & `ibm-generative-ai-0.2.4/examples/user/prompt_tuning/summarization.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/prompts_adult_dataset/prompt_generation_with_column_idx.py` & `ibm-generative-ai-0.2.4/examples/user/prompts_adult_dataset/prompt_generation_with_column_idx.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/prompts_adult_dataset/prompt_generation_with_headers.py` & `ibm-generative-ai-0.2.4/examples/user/prompts_adult_dataset/prompt_generation_with_headers.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/saving_prompts_as_hf_dataset.py` & `ibm-generative-ai-0.2.4/examples/user/saving_prompts_as_hf_dataset.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/self-reflection.py` & `ibm-generative-ai-0.2.4/examples/user/self-reflection.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/self_instruct.py` & `ibm-generative-ai-0.2.4/examples/user/self_instruct.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/streaming.py` & `ibm-generative-ai-0.2.4/examples/user/streaming.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/tokenize-sync.py` & `ibm-generative-ai-0.2.4/examples/user/tokenize-sync.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/examples/user/tokens.py` & `ibm-generative-ai-0.2.4/examples/user/tokens.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/pyproject.toml` & `ibm-generative-ai-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/src/genai/credentials.py` & `ibm-generative-ai-0.2.4/src/genai/credentials.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/src/genai/exceptions/genai_exception.py` & `ibm-generative-ai-0.2.4/src/genai/exceptions/genai_exception.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/src/genai/extensions/huggingface/save_huggingface.py` & `ibm-generative-ai-0.2.4/src/genai/extensions/huggingface/save_huggingface.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/src/genai/extensions/langchain/llm.py` & `ibm-generative-ai-0.2.4/src/genai/extensions/langchain/llm.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/src/genai/extensions/langchain/prompt.py` & `ibm-generative-ai-0.2.4/src/genai/extensions/langchain/prompt.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/src/genai/extensions/localserver/custom_model_interface.py` & `ibm-generative-ai-0.2.4/src/genai/extensions/localserver/custom_model_interface.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/src/genai/extensions/localserver/local_api_server.py` & `ibm-generative-ai-0.2.4/src/genai/extensions/localserver/local_api_server.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/src/genai/extensions/pandas/prompt_sub.py` & `ibm-generative-ai-0.2.4/src/genai/extensions/pandas/prompt_sub.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/src/genai/metadata.py` & `ibm-generative-ai-0.2.4/src/genai/metadata.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/src/genai/model.py` & `ibm-generative-ai-0.2.4/src/genai/model.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/src/genai/prompt_pattern.py` & `ibm-generative-ai-0.2.4/src/genai/prompt_pattern.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/src/genai/routers/files.py` & `ibm-generative-ai-0.2.4/src/genai/routers/files.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/src/genai/routers/prompt_template.py` & `ibm-generative-ai-0.2.4/src/genai/routers/prompt_template.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/src/genai/routers/tunes.py` & `ibm-generative-ai-0.2.4/src/genai/routers/tunes.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/src/genai/schemas/__init__.py` & `ibm-generative-ai-0.2.4/src/genai/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/src/genai/schemas/descriptions.py` & `ibm-generative-ai-0.2.4/src/genai/schemas/descriptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     STREAM = "Enables to stream partial progress as server-sent events. Defaults to false."
     TEMPERATURE = "The value used to module the next token probabilities. The range is 0.05 to 2.00, a value set to 0.05 would make it deterministic. Valid only with decoding_method=sample."
     TIME_LIMIT = "Time limit in milliseconds - if not completed within this time, generation will stop. The text generated so far will be returned along with the TIME_LIMIT stop reason."
     TOP_K = "The number of highest probability vocabulary tokens to keep for top-k-filtering. The range is any value >= 1. Valid only with decoding_method=sample."
     TOP_P = "If set to value < 1, only the most probable tokens with probabilities that add up to top_p or higher are kept for generation. The range is 0.00 to 1.00. Valid only with decoding_method=sample."
     REPETITION_PENALTY = "The parameter for repetition penalty. 1.0 means no penalty."
     TRUNCATE_INPUT_TOKENS = "Truncate to this many input tokens. Can be used to avoid requests failing due to input being longer than configured limits. Zero means don't truncate."
+    BEAM_WIDTH = "Multiple output sequences of tokens are generated, using your decoding selection, and then the output sequence with the highest overall probability is returned. When beam search is enabled, there will be a performance penalty, and Stop sequences will not be available."  # noqa
 
     # Params.Token
     RETURN_TOKEN = "Return tokens with the response. Defaults to false."
 
     # Params.History
     LIMIT = "Specifies the maximum number of items in the collection that should be returned. Defaults to 100. Maximum is 100."
     OFFSET = "Specifies the starting position in the collection. Defaults to 0."
```

### Comparing `ibm-generative-ai-0.2.3/src/genai/schemas/files_params.py` & `ibm-generative-ai-0.2.4/src/genai/schemas/files_params.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 from genai.schemas.descriptions import FilesAPIDescriptions as tx
 
 
 class FileListParams(BaseModel):
     """Class to hold the parameters for file listing."""
 
     class Config:
-        anystr_strip_whitespace: True
-        extra: Extra.forbid
+        anystr_strip_whitespace = True
+        extra = Extra.forbid
 
     limit: Optional[int] = Field(None, description=tx.LIMIT, le=100)
     offset: Optional[int] = Field(None, description=tx.OFFSET)
     search: Optional[str] = Field(None, description=tx.SEARCH)
 
 
 class MultipartFormData(BaseModel):
     class Config:
-        anystr_strip_whitespace: True
-        extra: Extra.forbid
+        anystr_strip_whitespace = True
+        extra = Extra.forbid
 
     purpose: str = Field(..., description=tx.PURPOSE)
     file: str = Field(..., description=tx.FILE)
```

### Comparing `ibm-generative-ai-0.2.3/src/genai/schemas/generate_params.py` & `ibm-generative-ai-0.2.4/src/genai/schemas/generate_params.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 from genai.schemas import Descriptions as tx
 
 # API Reference : https://workbench.res.ibm.com/docs
 
 
 class LengthPenalty(BaseModel):
     class Config:
-        anystr_strip_whitespace: True
-        extra: Extra.forbid
+        anystr_strip_whitespace = True
+        extra = Extra.forbid
 
     decay_factor: Optional[float] = Field(None, description=tx.DECAY_FACTOR, gt=1.00)
     start_index: Optional[int] = Field(None, description=tx.START_INDEX)
 
 
 class ReturnOptions(BaseModel):
     class Config:
-        anystr_strip_whitespace: True
-        extra: Extra.forbid
+        anystr_strip_whitespace = True
+        extra = Extra.forbid
 
     input_text: Optional[bool] = Field(None, description=tx.INPUT_TEXT)
     generated_tokens: Optional[bool] = Field(None, description=tx.GENERATED_TOKEN)
     input_tokens: Optional[bool] = Field(None, description=tx.INPUT_TOKEN)
     token_logprobs: Optional[bool] = Field(None, description=tx.TOKEN_LOGPROBS)
     token_ranks: Optional[bool] = Field(None, description=tx.TOKEN_RANKS)
     top_n_tokens: Optional[int] = Field(None, description=tx.TOP_N_TOKENS)
@@ -49,20 +49,23 @@
     class Config:
         anystr_strip_whitespace = True
         extra = Extra.allow
         allow_population_by_field_name = True
 
     decoding_method: Optional[Literal["greedy", "sample"]] = Field(None, description=tx.DECODING_METHOD)
     length_penalty: Optional[LengthPenalty] = Field(None, description=tx.LENGTH_PENALTY)
-    max_new_tokens: Optional[int] = Field(None, description=tx.MAX_NEW_TOKEN)
-    min_new_tokens: Optional[int] = Field(None, description=tx.MIN_NEW_TOKEN)
-    random_seed: Optional[int] = Field(None, description=tx.RANDOM_SEED, ge=1, le=9999)
-    stop_sequences: Optional[list[str]] = Field(None, description=tx.STOP_SQUENCES)
+    max_new_tokens: Optional[int] = Field(None, description=tx.MAX_NEW_TOKEN, ge=1)
+    min_new_tokens: Optional[int] = Field(None, description=tx.MIN_NEW_TOKEN, ge=0)
+    random_seed: Optional[int] = Field(None, description=tx.RANDOM_SEED, ge=1)
+    stop_sequences: Optional[list[str]] = Field(None, description=tx.STOP_SQUENCES, min_length=1)
     stream: Optional[bool] = Field(None, description=tx.STREAM)
-    temperature: Optional[float] = Field(None, description=tx.TEMPERATURE, ge=0.00, le=2.00)
+    temperature: Optional[float] = Field(None, description=tx.TEMPERATURE, ge=0.05, le=2.00)
     time_limit: Optional[int] = Field(None, description=tx.TIME_LIMIT)
     top_k: Optional[int] = Field(None, description=tx.TOP_K, ge=1)
     top_p: Optional[float] = Field(None, description=tx.TOP_P, ge=0.00, le=1.00)
-    repetition_penalty: Optional[float] = Field(None, description=tx.REPETITION_PENALTY)
-    truncate_input_tokens: Optional[int] = Field(None, description=tx.TRUNCATE_INPUT_TOKENS)
+    repetition_penalty: Optional[float] = Field(
+        None, description=tx.REPETITION_PENALTY, multiple_of=0.01, ge=1.00, le=2.00
+    )
+    truncate_input_tokens: Optional[int] = Field(None, description=tx.TRUNCATE_INPUT_TOKENS, ge=0)
+    beam_width: Optional[int] = Field(None, description=tx.BEAM_WIDTH, ge=0)
     return_options: Optional[ReturnOptions] = Field(None, description=tx.RETURN)
     returns: Optional[Return] = Field(None, description=tx.RETURN, alias="return", deprecated=True)
```

### Comparing `ibm-generative-ai-0.2.3/src/genai/schemas/history_params.py` & `ibm-generative-ai-0.2.4/src/genai/schemas/history_params.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,14 @@
 from genai.schemas import Descriptions as tx
 
 # API Reference : https://workbench.res.ibm.com/docs
 
 
 class HistoryParams(BaseModel):
     class Config:
-        anystr_strip_whitespace: True
-        extra: Extra.forbid
+        anystr_strip_whitespace = True
+        extra = Extra.forbid
 
     limit: Optional[int] = Field(None, description=tx.LIMIT, le=100)
     offset: Optional[int] = Field(None, description=tx.OFFSET)
     status: Optional[Literal["SUCCESS", "ERROR"]] = Field(None, description=tx.STATUS)
     origin: Optional[Literal["API", "UI"]] = Field(None, description=tx.ORIGIN)
```

### Comparing `ibm-generative-ai-0.2.3/src/genai/schemas/responses.py` & `ibm-generative-ai-0.2.4/src/genai/schemas/responses.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/src/genai/schemas/tunes_params.py` & `ibm-generative-ai-0.2.4/src/genai/schemas/tunes_params.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 from genai.schemas.descriptions import TunesAPIDescriptions as tx
 
 
 class TunesListParams(BaseModel):
     """Class to hold the parameters for listing tunes."""
 
     class Config:
-        anystr_strip_whitespace: True
-        extra: Extra.forbid
+        anystr_strip_whitespace = True
+        extra = Extra.forbid
 
     limit: Optional[int] = Field(None, description=tx.LIMIT, le=100)
     offset: Optional[int] = Field(None, description=tx.OFFSET)
     status: Optional[str] = Field(None, description=tx.STATUS)
     search: Optional[str] = Field(None, description=tx.SEARCH)
 
 
 class CreateTuneHyperParams(BaseModel):
     """Class to hold the hyperparameters for creating tunes."""
 
     class Config:
-        anystr_strip_whitespace: True
-        # extra: Extra.forbid
+        anystr_strip_whitespace = True
+        extra = Extra.allow
 
     accumulate_steps: Optional[int] = Field(16, description=tx.ACCUMULATE_STEPS)
     batch_size: Optional[int] = Field(16, description=tx.BATCH_SIZE)
     learning_rate: Optional[float] = Field(0.3, description=tx.LEARNING_RATE)
     max_input_tokens: Optional[int] = Field(256, description=tx.MAX_INPUT_TOKENS)
     max_output_tokens: Optional[int] = Field(128, description=tx.MAX_OUTPUT_TOKENS)
     num_epochs: Optional[int] = Field(20, description=tx.NUM_EPOCHS)
@@ -38,16 +38,16 @@
     init_text: Optional[str] = Field(None, description=tx.INIT_TEXT)
 
 
 class CreateTuneParams(BaseModel):
     """Class to hold the parameters for creating tunes."""
 
     class Config:
-        anystr_strip_whitespace: True
-        # extra: Extra.forbid
+        anystr_strip_whitespace = True
+        extra = Extra.allow
 
     name: str = Field(None, description=tx.NAME)
     model_id: str = Field(None, description=tx.MODEL_ID)
     method_id: str = Field(None, description=tx.METHOD_ID)
     task_id: str = Field(None, description=tx.TASK_ID)
     training_file_ids: list[str] = Field(None, description=tx.TRAINING_FILE_IDS)
     validation_file_ids: Optional[list[str]] = Field(None, description=tx.VALIDATION_FILE_IDS)
```

### Comparing `ibm-generative-ai-0.2.3/src/genai/services/__init__.py` & `ibm-generative-ai-0.2.4/src/genai/services/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/src/genai/services/async_generator.py` & `ibm-generative-ai-0.2.4/src/genai/services/async_generator.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/src/genai/services/connection_manager.py` & `ibm-generative-ai-0.2.4/src/genai/services/connection_manager.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/src/genai/services/file_manager.py` & `ibm-generative-ai-0.2.4/src/genai/services/file_manager.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/src/genai/services/prompt_template_manager.py` & `ibm-generative-ai-0.2.4/src/genai/services/prompt_template_manager.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/src/genai/services/request_handler.py` & `ibm-generative-ai-0.2.4/src/genai/services/request_handler.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/src/genai/services/service_interface.py` & `ibm-generative-ai-0.2.4/src/genai/services/service_interface.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/src/genai/services/tune_manager.py` & `ibm-generative-ai-0.2.4/src/genai/services/tune_manager.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/src/genai/utils/extensions.py` & `ibm-generative-ai-0.2.4/src/genai/utils/extensions.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/src/genai/utils/json_utils.py` & `ibm-generative-ai-0.2.4/src/genai/utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/src/genai/utils/search_space_params.py` & `ibm-generative-ai-0.2.4/src/genai/utils/search_space_params.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/src/genai/utils/service_utils.py` & `ibm-generative-ai-0.2.4/src/genai/utils/service_utils.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/src/ibm_generative_ai.egg-info/PKG-INFO` & `ibm-generative-ai-0.2.4/src/ibm_generative_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibm-generative-ai
-Version: 0.2.3
+Version: 0.2.4
 Summary: IBM Generative AI is a Python library built on IBM's large language model REST interface.
 Author-email: Lee Martie <lee.martie@ibm.com>, Ana Fucs <ana.fucs@ibm.com>, Veronique Demers <vdemers@ibm.com>, Mairead O'Neill <moneill@ibm.com>, Mirian Silva <mirianfrsilva@ibm.com>, Onkar Bhardwaj <onkarbhardwaj@ibm.com>, James Sutton <james.sutton@uk.ibm.com>, Ja Young Lee <younglee@ibm.com>, Adriana Meza Soria <adriana.meza.soria@ibm.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: langchain
 Provides-Extra: huggingface
```

### Comparing `ibm-generative-ai-0.2.3/src/ibm_generative_ai.egg-info/SOURCES.txt` & `ibm-generative-ai-0.2.4/src/ibm_generative_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/src/ibm_generative_ai.egg-info/requires.txt` & `ibm-generative-ai-0.2.4/src/ibm_generative_ai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/tests/assets/file_to_tune.json` & `ibm-generative-ai-0.2.4/tests/assets/file_to_tune.json`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/tests/assets/file_to_tune.jsonl` & `ibm-generative-ai-0.2.4/tests/assets/file_to_tune.jsonl`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/tests/assets/response_helper.py` & `ibm-generative-ai-0.2.4/tests/assets/response_helper.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/tests/extensions/test_langchain.py` & `ibm-generative-ai-0.2.4/tests/extensions/test_langchain.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/tests/extensions/test_localserver.py` & `ibm-generative-ai-0.2.4/tests/extensions/test_localserver.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/tests/extensions/test_save_huggingface.py` & `ibm-generative-ai-0.2.4/tests/extensions/test_save_huggingface.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/tests/extensions/test_sub_from_pandas.py` & `ibm-generative-ai-0.2.4/tests/extensions/test_sub_from_pandas.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/tests/integration/conftest.py` & `ibm-generative-ai-0.2.4/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/tests/integration/test_examples.py` & `ibm-generative-ai-0.2.4/tests/integration/test_examples.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/tests/test_concurrent.py` & `ibm-generative-ai-0.2.4/tests/test_concurrent.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     def mock_generate_json(self, mocker):
         async_mock = AsyncMock()
         mocker.patch("genai.services.AsyncResponseGenerator._get_response_json", side_effect=async_mock)
         return async_mock
 
     @pytest.fixture
     def generate_params(self):
-        return GenerateParams(temperature=0, max_new_tokens=3, return_options=ReturnOptions(input_text=True))
+        return GenerateParams(temperature=0.05, max_new_tokens=3, return_options=ReturnOptions(input_text=True))
 
     @pytest.fixture
     def mock_tokenize_json(self, mocker):
         async_mock = AsyncMock()
         mocker.patch("genai.services.AsyncResponseGenerator._get_response_json", side_effect=async_mock)
         return async_mock
```

### Comparing `ibm-generative-ai-0.2.3/tests/test_files.py` & `ibm-generative-ai-0.2.4/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/tests/test_generate_schema.py` & `ibm-generative-ai-0.2.4/tests/test_generate_schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
             stream=False,
             temperature=0.5,
             time_limit=10.0,
             top_k=10,
             top_p=0.7,
             repetition_penalty=1.2,
             truncate_input_tokens=2,
+            beam_width=1,
             return_options=ReturnOptions(
                 input_text=True,
                 generated_tokens=True,
                 input_tokens=True,
                 token_logprobs=False,
             ),
         )
@@ -118,16 +119,14 @@
 
     def test_random_seed_invalid_type(self):
         # test that random_seed must be an integer between 1 and 9999
         with pytest.raises(ValidationError):
             GenerateParams(random_seed="dummy")
         with pytest.raises(ValidationError):
             GenerateParams(random_seed=0)
-        with pytest.raises(ValidationError):
-            GenerateParams(random_seed=10000)
 
     def test_random_seed_valid_type(self, request_body):
         # test that random_seed must be an integer between 1 and 9999
         params = request_body["params"]
         assert params.random_seed >= 1
         assert params.random_seed <= 9999
         assert isinstance(params.random_seed, int)
@@ -158,15 +157,15 @@
 
     def test_stream_valid_type(self, request_body):
         # test that stream must be a boolean
         params = request_body["params"]
         assert isinstance(params.stream, bool)
 
     def test_temperature_invalid_type(self):
-        # test that temperature must be a float between 0 and 1
+        # test that temperature must be a float between 0.05 and 1
         with pytest.raises(ValidationError):
             GenerateParams(temperature="")
         with pytest.raises(ValidationError):
             GenerateParams(temperature=[0, 1, 2])
         with pytest.raises(ValidationError):
             GenerateParams(temperature="dummy")
         with pytest.raises(ValidationError):
@@ -234,37 +233,48 @@
         params = request_body["params"]
         assert params.top_p >= 0
         assert params.top_p <= 1
         assert isinstance(params.top_p, float)
 
     def test_repetition_penalty_invalid_type(self):
         # test that repetition_penalty must be a float
-        # NOTE: repetition_penalty can be 0 or less then 0?
+        # NOTE: repetition_penalty can be 0 or less than 0?
         with pytest.raises(ValidationError):
             GenerateParams(repetition_penalty="")
         with pytest.raises(ValidationError):
             GenerateParams(repetition_penalty=[0, 1, 2])
         with pytest.raises(ValidationError):
             GenerateParams(repetition_penalty="dummy")
 
     def test_repetition_penalty_valid_type(self, request_body):
         # test that repetition_penalty must be a float
         params = request_body["params"]
         # assert params.repetition_penalty >= 0
         assert isinstance(params.repetition_penalty, float)
 
     def test_truncate_input_tokens_invalid_type(self):
-        # test that truncate_input_tokens must be a interger
+        # test that truncate_input_tokens must be an integer
         with pytest.raises(ValidationError):
             GenerateParams(truncate_input_tokens="")
         with pytest.raises(ValidationError):
             GenerateParams(truncate_input_tokens=[0, 1, 2])
         with pytest.raises(ValidationError):
             GenerateParams(truncate_input_tokens="dummy")
 
+    def test_beam_width_valid_type(self, request_body):
+        params = request_body["params"]
+        assert isinstance(params.beam_width, int)
+
+    def test_beam_width_invalid_type(self):
+        # test that beam_width must be an non-negative integer
+        with pytest.raises(ValidationError):
+            GenerateParams(beam_width="")
+        with pytest.raises(ValidationError):
+            GenerateParams(beam_width=-100)
+
     def test_truncate_input_tokens_valid_type(self, request_body):
         params = request_body["params"]
         assert isinstance(params.truncate_input_tokens, int)
 
     def test_returns_raises_warning(self):
         with pytest.deprecated_call():
             GenerateParams(returns=Return())
```

### Comparing `ibm-generative-ai-0.2.3/tests/test_generate_service.py` & `ibm-generative-ai-0.2.4/tests/test_generate_service.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/tests/test_history.py` & `ibm-generative-ai-0.2.4/tests/test_history.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/tests/test_json_utils.py` & `ibm-generative-ai-0.2.4/tests/test_json_utils.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/tests/test_logging.py` & `ibm-generative-ai-0.2.4/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/tests/test_metadata.py` & `ibm-generative-ai-0.2.4/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/tests/test_model.py` & `ibm-generative-ai-0.2.4/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/tests/test_model_async.py` & `ibm-generative-ai-0.2.4/tests/test_model_async.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/tests/test_prompt_pattern.py` & `ibm-generative-ai-0.2.4/tests/test_prompt_pattern.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/tests/test_prompt_pattern_watsonx.py` & `ibm-generative-ai-0.2.4/tests/test_prompt_pattern_watsonx.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/tests/test_prompt_template_manager.py` & `ibm-generative-ai-0.2.4/tests/test_prompt_template_manager.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/tests/test_request_handler.py` & `ibm-generative-ai-0.2.4/tests/test_request_handler.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/tests/test_schema_validation.py` & `ibm-generative-ai-0.2.4/tests/test_schema_validation.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/tests/test_service_interface.py` & `ibm-generative-ai-0.2.4/tests/test_service_interface.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/tests/test_service_interface_async.py` & `ibm-generative-ai-0.2.4/tests/test_service_interface_async.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/tests/test_service_utils.py` & `ibm-generative-ai-0.2.4/tests/test_service_utils.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/tests/test_token.py` & `ibm-generative-ai-0.2.4/tests/test_token.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.3/tests/test_tunes.py` & `ibm-generative-ai-0.2.4/tests/test_tunes.py`

 * *Files identical despite different names*

