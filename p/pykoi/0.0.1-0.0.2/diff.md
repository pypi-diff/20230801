# Comparing `tmp/pykoi-0.0.1.tar.gz` & `tmp/pykoi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykoi-0.0.1.tar", max compression
+gzip compressed data, was "pykoi-0.0.2.tar", max compression
```

## Comparing `pykoi-0.0.1.tar` & `pykoi-0.0.2.tar`

### file list

```diff
@@ -1,66 +1,92 @@
--rw-r--r--   0        0        0    11357 2023-07-24 05:48:22.776468 pykoi-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      442 2023-07-24 08:01:06.918220 pykoi-0.0.1/README.md
--rw-r--r--   0        0        0      344 2023-07-24 06:45:28.869332 pykoi-0.0.1/pykoi/__init__.py
--rw-r--r--   0        0        0     8814 2023-07-24 06:54:35.491952 pykoi-0.0.1/pykoi/application.py
--rw-r--r--   0        0        0        0 2023-07-24 05:48:22.778002 pykoi-0.0.1/pykoi/component/__init__.py
--rw-r--r--   0        0        0     3910 2023-07-24 05:48:22.778068 pykoi-0.0.1/pykoi/component/base.py
--rw-r--r--   0        0        0     1033 2023-07-24 05:48:22.778116 pykoi-0.0.1/pykoi/component/chatbot_database_factory.py
--rw-r--r--   0        0        0      139 2023-07-24 05:48:22.778157 pykoi-0.0.1/pykoi/component/constants.py
--rw-r--r--   0        0        0        0 2023-07-24 05:48:22.778499 pykoi-0.0.1/pykoi/db/__init__.py
--rw-r--r--   0        0        0     7345 2023-07-24 05:48:22.778595 pykoi-0.0.1/pykoi/db/qa_database.py
--rw-r--r--   0        0        0     5768 2023-07-24 05:48:22.778641 pykoi-0.0.1/pykoi/db/ranking_database.py
--rw-r--r--   0        0        0      248 2023-07-24 05:48:22.778722 pykoi-0.0.1/pykoi/frontend/.gitignore
--rw-r--r--   0        0        0     2956 2023-07-24 05:48:22.778789 pykoi-0.0.1/pykoi/frontend/README.md
--rw-r--r--   0        0        0    91356 2023-07-24 05:48:22.779327 pykoi-0.0.1/pykoi/frontend/dist/assets/index-918eba54.js
--rw-r--r--   0        0        0    22972 2023-07-24 05:48:22.779667 pykoi-0.0.1/pykoi/frontend/dist/assets/index-cf40d152.css
--rw-r--r--   0        0        0      452 2023-07-24 05:48:22.779737 pykoi-0.0.1/pykoi/frontend/dist/index.html
--rw-r--r--   0        0        0     1498 2023-07-24 05:48:22.779799 pykoi-0.0.1/pykoi/frontend/dist/vite.svg
--rw-r--r--   0        0        0      360 2023-07-24 05:48:22.779852 pykoi-0.0.1/pykoi/frontend/index.html
--rw-r--r--   0        0        0      938 2023-07-24 05:48:22.779903 pykoi-0.0.1/pykoi/frontend/jsconfig.json
--rw-r--r--   0        0        0      540 2023-07-24 05:48:22.779955 pykoi-0.0.1/pykoi/frontend/package.json
--rw-r--r--   0        0        0     1498 2023-07-24 05:48:22.780032 pykoi-0.0.1/pykoi/frontend/public/vite.svg
--rw-r--r--   0        0        0     1500 2023-07-24 05:48:22.780119 pykoi-0.0.1/pykoi/frontend/src/App.svelte
--rw-r--r--   0        0        0    10286 2023-07-24 05:48:22.780215 pykoi-0.0.1/pykoi/frontend/src/app.css
--rw-r--r--   0        0        0     1951 2023-07-24 05:48:22.780300 pykoi-0.0.1/pykoi/frontend/src/assets/svelte.svg
--rw-r--r--   0        0        0     4901 2023-07-24 05:48:22.780451 pykoi-0.0.1/pykoi/frontend/src/lib/Annotations/QuestionRating.svelte
--rw-r--r--   0        0        0      290 2023-07-24 05:48:22.780533 pykoi-0.0.1/pykoi/frontend/src/lib/Chatbots/Chat.svelte
--rw-r--r--   0        0        0     8876 2023-07-24 05:48:22.780624 pykoi-0.0.1/pykoi/frontend/src/lib/Chatbots/Chatbot.svelte
--rw-r--r--   0        0        0     8705 2023-07-24 05:48:22.780670 pykoi-0.0.1/pykoi/frontend/src/lib/Chatbots/RankedChatbot.svelte
--rw-r--r--   0        0        0     3905 2023-07-24 05:48:22.780801 pykoi-0.0.1/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/ColumnChart.svelte
--rw-r--r--   0        0        0     3905 2023-07-24 05:48:22.780875 pykoi-0.0.1/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/HistogramAnswer.svelte
--rw-r--r--   0        0        0     3890 2023-07-24 05:48:22.780930 pykoi-0.0.1/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/HistogramQuestion.svelte
--rw-r--r--   0        0        0     4421 2023-07-24 05:48:22.780990 pykoi-0.0.1/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/HorizontalStackedBar.svelte
--rw-r--r--   0        0        0     2701 2023-07-24 05:48:22.781055 pykoi-0.0.1/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/MetricCardAbsolute.svelte
--rw-r--r--   0        0        0     2638 2023-07-24 05:48:22.781111 pykoi-0.0.1/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/MetricCardPercentage.svelte
--rw-r--r--   0        0        0     1384 2023-07-24 05:48:22.781164 pykoi-0.0.1/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/QACard.svelte
--rw-r--r--   0        0        0     1055 2023-07-24 05:48:22.781214 pykoi-0.0.1/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/QATable.svelte
--rw-r--r--   0        0        0     3326 2023-07-24 05:48:22.781273 pykoi-0.0.1/pykoi/frontend/src/lib/Dashboards/Feedback.svelte
--rw-r--r--   0        0        0     4317 2023-07-24 05:48:22.781387 pykoi-0.0.1/pykoi/frontend/src/lib/Evaluation/Bar.svelte
--rw-r--r--   0        0        0      507 2023-07-24 05:48:22.781437 pykoi-0.0.1/pykoi/frontend/src/lib/Evaluation/Cell.svelte
--rw-r--r--   0        0        0     3898 2023-07-24 05:48:22.781481 pykoi-0.0.1/pykoi/frontend/src/lib/Evaluation/EvalLineChart.svelte
--rw-r--r--   0        0        0     3910 2023-07-24 05:48:22.781525 pykoi-0.0.1/pykoi/frontend/src/lib/Evaluation/LineChart.svelte
--rw-r--r--   0        0        0     3611 2023-07-24 05:48:22.781587 pykoi-0.0.1/pykoi/frontend/src/lib/Evaluation/RLHFEvaluation.svelte
--rw-r--r--   0        0        0     5069 2023-07-24 05:48:22.781652 pykoi-0.0.1/pykoi/frontend/src/lib/Evaluation/Table.svelte
--rw-r--r--   0        0        0     1804 2023-07-24 05:48:22.781705 pykoi-0.0.1/pykoi/frontend/src/lib/Evaluation/data.js
--rw-r--r--   0        0        0      584 2023-07-24 05:48:22.781759 pykoi-0.0.1/pykoi/frontend/src/lib/Evaluation/store.js
--rw-r--r--   0        0        0      380 2023-07-24 05:48:22.781878 pykoi-0.0.1/pykoi/frontend/src/lib/UIComponents/Dropdown.svelte
--rw-r--r--   0        0        0      191 2023-07-24 05:48:22.781939 pykoi-0.0.1/pykoi/frontend/src/main.js
--rw-r--r--   0        0        0     6818 2023-07-24 05:48:22.782013 pykoi-0.0.1/pykoi/frontend/src/normalize.css
--rw-r--r--   0        0        0      542 2023-07-24 05:48:22.782090 pykoi-0.0.1/pykoi/frontend/src/store.js
--rw-r--r--   0        0        0     9194 2023-07-24 05:48:22.782137 pykoi-0.0.1/pykoi/frontend/src/styles.css
--rw-r--r--   0        0        0     1743 2023-07-24 05:48:22.782192 pykoi-0.0.1/pykoi/frontend/src/utils.js
--rw-r--r--   0        0        0       71 2023-07-24 05:48:22.782236 pykoi-0.0.1/pykoi/frontend/src/vite-env.d.ts
--rw-r--r--   0        0        0      228 2023-07-24 05:48:22.782288 pykoi-0.0.1/pykoi/frontend/svelte.config.js
--rw-r--r--   0        0        0      177 2023-07-24 05:48:22.782338 pykoi-0.0.1/pykoi/frontend/vite.config.js
--rw-r--r--   0        0        0        0 2023-07-24 05:48:22.782390 pykoi-0.0.1/pykoi/llm/__init__.py
--rw-r--r--   0        0        0      864 2023-07-24 05:48:22.782469 pykoi-0.0.1/pykoi/llm/abs_llm.py
--rw-r--r--   0        0        0      455 2023-07-24 07:45:46.634814 pykoi-0.0.1/pykoi/llm/constants.py
--rw-r--r--   0        0        0     2818 2023-07-24 05:48:22.782596 pykoi-0.0.1/pykoi/llm/huggingface.py
--rw-r--r--   0        0        0     2077 2023-07-24 07:46:28.170787 pykoi-0.0.1/pykoi/llm/model_factory.py
--rw-r--r--   0        0        0     2205 2023-07-24 05:48:22.782707 pykoi-0.0.1/pykoi/llm/openai.py
--rw-r--r--   0        0        0     3465 2023-07-24 08:51:40.226463 pykoi-0.0.1/pykoi/llm/peft_huggingface.py
--rw-r--r--   0        0        0        0 2023-07-24 05:48:22.782816 pykoi-0.0.1/pykoi/rlhf/__init__.py
--rw-r--r--   0        0        0    32326 2023-07-24 06:50:21.614734 pykoi-0.0.1/pykoi/rlhf/rlhf.py
--rw-r--r--   0        0        0     1014 2023-07-24 05:48:22.783034 pykoi-0.0.1/pykoi/state.py
--rw-r--r--   0        0        0      612 2023-07-24 09:27:54.670355 pykoi-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1363 1970-01-01 00:00:00.000000 pykoi-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-29 23:35:02.238057 pykoi-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     1753 2023-08-01 05:21:35.549386 pykoi-0.0.2/README.md
+-rw-r--r--   0        0        0      462 2023-07-31 07:48:56.593127 pykoi-0.0.2/pykoi/__init__.py
+-rw-r--r--   0        0        0    17630 2023-07-30 23:19:20.518401 pykoi-0.0.2/pykoi/application.py
+-rw-r--r--   0        0        0        0 2023-07-29 23:35:02.243138 pykoi-0.0.2/pykoi/component/__init__.py
+-rw-r--r--   0        0        0     3910 2023-07-29 23:35:02.243218 pykoi-0.0.2/pykoi/component/base.py
+-rw-r--r--   0        0        0     3291 2023-08-01 05:26:24.768975 pykoi-0.0.2/pykoi/component/chatbot_comparator.py
+-rw-r--r--   0        0        0     1033 2023-07-29 23:35:02.243328 pykoi-0.0.2/pykoi/component/chatbot_database_factory.py
+-rw-r--r--   0        0        0      139 2023-07-29 23:35:02.243375 pykoi-0.0.2/pykoi/component/constants.py
+-rw-r--r--   0        0        0        0 2023-07-29 23:35:02.243424 pykoi-0.0.2/pykoi/db/__init__.py
+-rw-r--r--   0        0        0     3175 2023-07-29 23:35:02.243507 pykoi-0.0.2/pykoi/db/abs_database.py
+-rw-r--r--   0        0        0     6521 2023-07-29 23:35:02.243569 pykoi-0.0.2/pykoi/db/comparator_database.py
+-rw-r--r--   0        0        0      756 2023-07-31 07:48:56.593275 pykoi-0.0.2/pykoi/db/constants.py
+-rw-r--r--   0        0        0     6985 2023-07-29 23:35:02.243702 pykoi-0.0.2/pykoi/db/qa_database.py
+-rw-r--r--   0        0        0     5883 2023-07-31 07:48:56.593422 pykoi-0.0.2/pykoi/db/ranking_database.py
+-rw-r--r--   0        0        0      248 2023-07-29 23:35:02.243850 pykoi-0.0.2/pykoi/frontend/.gitignore
+-rw-r--r--   0        0        0     2956 2023-07-29 23:35:02.243912 pykoi-0.0.2/pykoi/frontend/README.md
+-rw-r--r--   0        0        0    31654 2023-07-31 07:48:56.593639 pykoi-0.0.2/pykoi/frontend/dist/assets/index-f75c1c12.css
+-rw-r--r--   0        0        0   134563 2023-07-31 07:48:56.594277 pykoi-0.0.2/pykoi/frontend/dist/assets/index-fc1a91e8.js
+-rw-r--r--   0        0        0      452 2023-07-31 07:48:56.594441 pykoi-0.0.2/pykoi/frontend/dist/index.html
+-rw-r--r--   0        0        0     1498 2023-07-29 23:35:02.244816 pykoi-0.0.2/pykoi/frontend/dist/vite.svg
+-rw-r--r--   0        0        0      360 2023-07-29 23:35:02.244869 pykoi-0.0.2/pykoi/frontend/index.html
+-rw-r--r--   0        0        0      938 2023-07-29 23:35:02.244937 pykoi-0.0.2/pykoi/frontend/jsconfig.json
+-rw-r--r--   0        0        0      581 2023-07-29 23:35:02.244992 pykoi-0.0.2/pykoi/frontend/package.json
+-rw-r--r--   0        0        0     1498 2023-07-29 23:35:02.245082 pykoi-0.0.2/pykoi/frontend/public/vite.svg
+-rw-r--r--   0        0        0     1711 2023-07-30 23:19:20.519624 pykoi-0.0.2/pykoi/frontend/src/App.svelte
+-rw-r--r--   0        0        0    10286 2023-07-29 23:35:02.245272 pykoi-0.0.2/pykoi/frontend/src/app.css
+-rw-r--r--   0        0        0     1951 2023-07-29 23:35:02.245362 pykoi-0.0.2/pykoi/frontend/src/assets/svelte.svg
+-rw-r--r--   0        0        0     4901 2023-07-29 23:35:02.245523 pykoi-0.0.2/pykoi/frontend/src/lib/Annotations/QuestionRating.svelte
+-rw-r--r--   0        0        0      290 2023-07-29 23:35:02.245604 pykoi-0.0.2/pykoi/frontend/src/lib/Chatbots/Chat.svelte
+-rw-r--r--   0        0        0     8876 2023-07-29 23:35:02.245708 pykoi-0.0.2/pykoi/frontend/src/lib/Chatbots/Chatbot.svelte
+-rw-r--r--   0        0        0    10723 2023-07-31 07:48:56.594707 pykoi-0.0.2/pykoi/frontend/src/lib/Chatbots/ComparisonChat.svelte
+-rw-r--r--   0        0        0    10985 2023-07-30 23:19:20.520058 pykoi-0.0.2/pykoi/frontend/src/lib/Chatbots/RankChatComparison.svelte
+-rw-r--r--   0        0        0     8748 2023-07-30 23:19:20.520243 pykoi-0.0.2/pykoi/frontend/src/lib/Chatbots/RankChatbotOld.svelte
+-rw-r--r--   0        0        0     8748 2023-07-30 23:19:20.520475 pykoi-0.0.2/pykoi/frontend/src/lib/Chatbots/RankedChatbot.svelte
+-rw-r--r--   0        0        0     6295 2023-07-30 23:19:20.520621 pykoi-0.0.2/pykoi/frontend/src/lib/Comparison/BumpChart.svelte
+-rw-r--r--   0        0        0      507 2023-07-29 23:35:02.246162 pykoi-0.0.2/pykoi/frontend/src/lib/Comparison/Cell.svelte
+-rw-r--r--   0        0        0     5351 2023-07-30 23:19:20.520740 pykoi-0.0.2/pykoi/frontend/src/lib/Comparison/ComparisonChart.svelte
+-rw-r--r--   0        0        0     4924 2023-07-30 23:19:20.520861 pykoi-0.0.2/pykoi/frontend/src/lib/Comparison/CumulativeScore.svelte
+-rw-r--r--   0        0        0     5027 2023-07-30 23:19:20.520979 pykoi-0.0.2/pykoi/frontend/src/lib/Comparison/CumulativeStack.svelte
+-rw-r--r--   0        0        0     4952 2023-07-30 23:19:20.521096 pykoi-0.0.2/pykoi/frontend/src/lib/Comparison/Heatmap.svelte
+-rw-r--r--   0        0        0     3269 2023-07-30 23:19:20.521232 pykoi-0.0.2/pykoi/frontend/src/lib/Comparison/HorizontalBar.svelte
+-rw-r--r--   0        0        0     5916 2023-07-30 23:19:20.521356 pykoi-0.0.2/pykoi/frontend/src/lib/Comparison/Table.svelte
+-rw-r--r--   0        0        0     9692 2023-07-29 23:35:02.246653 pykoi-0.0.2/pykoi/frontend/src/lib/Comparison/data.js
+-rw-r--r--   0        0        0     2018 2023-07-30 23:19:20.521484 pykoi-0.0.2/pykoi/frontend/src/lib/Comparison/store.js
+-rw-r--r--   0        0        0     3644 2023-07-31 07:48:56.594904 pykoi-0.0.2/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/ColumnChart.svelte
+-rw-r--r--   0        0        0     3905 2023-07-29 23:35:02.246928 pykoi-0.0.2/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/HistogramAnswer.svelte
+-rw-r--r--   0        0        0     3890 2023-07-29 23:35:02.246987 pykoi-0.0.2/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/HistogramQuestion.svelte
+-rw-r--r--   0        0        0     4421 2023-07-29 23:35:02.247047 pykoi-0.0.2/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/HorizontalStackedBar.svelte
+-rw-r--r--   0        0        0     2701 2023-07-29 23:35:02.247105 pykoi-0.0.2/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/MetricCardAbsolute.svelte
+-rw-r--r--   0        0        0     2638 2023-07-29 23:35:02.247166 pykoi-0.0.2/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/MetricCardPercentage.svelte
+-rw-r--r--   0        0        0     1384 2023-07-29 23:35:02.247225 pykoi-0.0.2/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/QACard.svelte
+-rw-r--r--   0        0        0      998 2023-07-31 07:48:56.595032 pykoi-0.0.2/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/QATable.svelte
+-rw-r--r--   0        0        0     3326 2023-07-29 23:35:02.247365 pykoi-0.0.2/pykoi/frontend/src/lib/Dashboards/Feedback.svelte
+-rw-r--r--   0        0        0     4317 2023-07-29 23:35:02.247488 pykoi-0.0.2/pykoi/frontend/src/lib/Evaluation/Bar.svelte
+-rw-r--r--   0        0        0     4311 2023-07-29 23:35:02.247543 pykoi-0.0.2/pykoi/frontend/src/lib/Evaluation/BumpChart.svelte
+-rw-r--r--   0        0        0      507 2023-07-29 23:35:02.247600 pykoi-0.0.2/pykoi/frontend/src/lib/Evaluation/Cell.svelte
+-rw-r--r--   0        0        0     3651 2023-07-29 23:35:02.247649 pykoi-0.0.2/pykoi/frontend/src/lib/Evaluation/ComparisonChart.svelte
+-rw-r--r--   0        0        0     5362 2023-07-29 23:35:02.247712 pykoi-0.0.2/pykoi/frontend/src/lib/Evaluation/EvalLineChart.svelte
+-rw-r--r--   0        0        0     3910 2023-07-29 23:35:02.247757 pykoi-0.0.2/pykoi/frontend/src/lib/Evaluation/LineChart.svelte
+-rw-r--r--   0        0        0     3611 2023-07-29 23:35:02.247816 pykoi-0.0.2/pykoi/frontend/src/lib/Evaluation/RLHFEvaluation.svelte
+-rw-r--r--   0        0        0     5069 2023-07-29 23:35:02.247882 pykoi-0.0.2/pykoi/frontend/src/lib/Evaluation/Table.svelte
+-rw-r--r--   0        0        0     4655 2023-07-29 23:35:02.247934 pykoi-0.0.2/pykoi/frontend/src/lib/Evaluation/data.js
+-rw-r--r--   0        0        0      584 2023-07-29 23:35:02.247984 pykoi-0.0.2/pykoi/frontend/src/lib/Evaluation/store.js
+-rw-r--r--   0        0        0      380 2023-07-29 23:35:02.248077 pykoi-0.0.2/pykoi/frontend/src/lib/UIComponents/Dropdown.svelte
+-rw-r--r--   0        0        0      191 2023-07-29 23:35:02.248132 pykoi-0.0.2/pykoi/frontend/src/main.js
+-rw-r--r--   0        0        0     6818 2023-07-29 23:35:02.248201 pykoi-0.0.2/pykoi/frontend/src/normalize.css
+-rw-r--r--   0        0        0      586 2023-07-31 07:48:56.595166 pykoi-0.0.2/pykoi/frontend/src/store.js
+-rw-r--r--   0        0        0     9194 2023-07-29 23:35:02.248302 pykoi-0.0.2/pykoi/frontend/src/styles.css
+-rw-r--r--   0        0        0     1725 2023-07-31 07:48:56.595300 pykoi-0.0.2/pykoi/frontend/src/utils.js
+-rw-r--r--   0        0        0       71 2023-07-29 23:35:02.248401 pykoi-0.0.2/pykoi/frontend/src/vite-env.d.ts
+-rw-r--r--   0        0        0      228 2023-07-29 23:35:02.248463 pykoi-0.0.2/pykoi/frontend/svelte.config.js
+-rw-r--r--   0        0        0      177 2023-07-29 23:35:02.248512 pykoi-0.0.2/pykoi/frontend/vite.config.js
+-rw-r--r--   0        0        0        0 2023-08-01 05:26:24.769038 pykoi-0.0.2/pykoi/interactives/__init__.py
+-rw-r--r--   0        0        0    30580 2023-08-01 05:26:24.769471 pykoi-0.0.2/pykoi/interactives/barchart.py
+-rw-r--r--   0        0        0        0 2023-07-29 23:35:02.248566 pykoi-0.0.2/pykoi/llm/__init__.py
+-rw-r--r--   0        0        0     1203 2023-07-29 23:35:02.248632 pykoi-0.0.2/pykoi/llm/abs_llm.py
+-rw-r--r--   0        0        0      455 2023-07-29 23:35:02.248682 pykoi-0.0.2/pykoi/llm/constants.py
+-rw-r--r--   0        0        0     3751 2023-08-01 05:21:35.587141 pykoi-0.0.2/pykoi/llm/huggingface.py
+-rw-r--r--   0        0        0     9257 2023-08-01 05:21:35.587256 pykoi-0.0.2/pykoi/llm/instruct_pipeline.py
+-rw-r--r--   0        0        0     2077 2023-07-29 23:35:02.248800 pykoi-0.0.2/pykoi/llm/model_factory.py
+-rw-r--r--   0        0        0     2440 2023-07-29 23:35:02.248858 pykoi-0.0.2/pykoi/llm/openai.py
+-rw-r--r--   0        0        0     3797 2023-07-29 23:35:02.248920 pykoi-0.0.2/pykoi/llm/peft_huggingface.py
+-rw-r--r--   0        0        0        0 2023-07-29 23:35:02.248971 pykoi-0.0.2/pykoi/rlhf/__init__.py
+-rw-r--r--   0        0        0    12377 2023-07-31 07:48:56.595643 pykoi-0.0.2/pykoi/rlhf/config.py
+-rw-r--r--   0        0        0       21 2023-07-29 23:35:02.249106 pykoi-0.0.2/pykoi/rlhf/rl_finetuning.py
+-rw-r--r--   0        0        0    27621 2023-07-31 07:48:56.595876 pykoi-0.0.2/pykoi/rlhf/rlhf.py
+-rw-r--r--   0        0        0       31 2023-07-29 23:35:02.249377 pykoi-0.0.2/pykoi/rlhf/rw_finetuning.py
+-rw-r--r--   0        0        0     8145 2023-07-31 07:48:56.596054 pykoi-0.0.2/pykoi/rlhf/supervised_finetuning.py
+-rw-r--r--   0        0        0     1014 2023-07-29 23:35:02.249509 pykoi-0.0.2/pykoi/state.py
+-rw-r--r--   0        0        0      689 2023-08-01 05:57:59.479559 pykoi-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2811 1970-01-01 00:00:00.000000 pykoi-0.0.2/PKG-INFO
```

### Comparing `pykoi-0.0.1/LICENSE.txt` & `pykoi-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.1/pykoi/component/base.py` & `pykoi-0.0.2/pykoi/component/base.py`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.1/pykoi/component/chatbot_database_factory.py` & `pykoi-0.0.2/pykoi/component/chatbot_database_factory.py`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.1/pykoi/db/qa_database.py` & `pykoi-0.0.2/pykoi/db/comparator_database.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,212 +1,214 @@
-"""Question answer database module"""
-import csv
+"""Comparator Database"""
 import datetime
 import os
-import sqlite3
-import threading
 
-import pandas as pd
-
-# QA_CSV_HEADER = ('ID', 'Question', 'Answer', 'Vote Status', 'Timestamp')
-QA_CSV_HEADER_ID = "ID"
-QA_CSV_HEADER_QUESTION = "Question"
-QA_CSV_HEADER_ANSWER = "Answer"
-QA_CSV_HEADER_VOTE_STATUS = "Vote Status"
-QA_CSV_HEADER_TIMESTAMPS = "Timestamp"
-QA_CSV_HEADER = (
-    QA_CSV_HEADER_ID,
-    QA_CSV_HEADER_QUESTION,
-    QA_CSV_HEADER_ANSWER,
-    QA_CSV_HEADER_VOTE_STATUS,
-    QA_CSV_HEADER_TIMESTAMPS,
+from typing import (
+    List,
+    Tuple
 )
 
+from pykoi.db.abs_database import AbsDatabase
+
 
-class QuestionAnswerDatabase:
-    """Question Answer Database class"""
+class ComparatorQuestionDatabase(AbsDatabase):
+    """Comparator Question Database class"""
 
-    def __init__(
-        self, db_file: str = os.path.join(os.getcwd(), "qd.db"), debug: bool = False
-    ):
+    def __init__(self,
+                 db_file: str = os.path.join(os.getcwd(), "comparator.db"),
+                 debug: bool = False) -> None:
         """
-        Initializes a new instance of the QuestionAnswerDatabase class.
+        Initializes a new instance of the ComparatorQuestionDatabase class.
 
         Args:
             db_file (str): The path to the SQLite database file.
             debug (bool, optional): Whether to print debug messages. Defaults to False.
         """
-        self._db_file = db_file
-        self._debug = debug
-        self._local = threading.local()  # Thread-local storage
-        self._lock = threading.Lock()  # Lock for concurrent write operations
-        self.create_table()
-
-    def get_connection(self):
-        """Returns the thread-local database connection"""
-        if not hasattr(self._local, "connection"):
-            self._local.connection = sqlite3.connect(self._db_file)
-        return self._local.connection
-
-    def get_cursor(self):
-        """Returns the thread-local database cursor"""
-        if not hasattr(self._local, "cursor"):
-            self._local.cursor = self.get_connection().cursor()
-        return self._local.cursor
-
-    def create_table(self):
-        """
-        Creates the question_answer table if it does not already exist in the database.
-        The table has four columns: id (primary key), question, answer, and vote_status.
-        vote_status is a text field that can only have the values 'up', 'down', or 'n/a'.
-        """
         query = """
-        CREATE TABLE IF NOT EXISTS question_answer (
+        CREATE TABLE IF NOT EXISTS comparator_question (
             id INTEGER PRIMARY KEY AUTOINCREMENT,
             question TEXT,
-            answer TEXT,
-            vote_status TEXT CHECK (vote_status IN ('up', 'down', 'n/a')),
             timestamp TIMESTAMP DEFAULT CURRENT_TIMESTAMP
         );
         """
-        with self._lock:
-            cursor = self.get_cursor()
-            cursor.execute(query)
-            self.get_connection().commit()
-
-        if self._debug:
-            rows = self.retrieve_all_question_answers()
-            print("Table contents after creating table:")
-            self.print_table(rows)
+        super().__init__(db_file, debug)
+        self.create_table(query)
 
-    def insert_question_answer(self, question: str, answer: str):
+    def insert(self, **kwargs) -> None:
         """
-        Inserts a new question-answer pair into the database with the given question and answer.
-        The vote_status field is set to 'n/a' by default.
-        Returns the ID of the newly inserted row.
+        Inserts question, timestamp into the database.
 
         Args:
-            question (str): The question to insert.
-            answer (str): The answer to insert.
+            kwargs (dict): The key-value pairs to insert into the database.
 
         Returns:
             int: The ID of the newly inserted row.
         """
+        question = kwargs["question"]
         timestamp = datetime.datetime.now()
         query = """
-        INSERT INTO question_answer (question, answer, vote_status, timestamp)
-        VALUES (?, ?, 'n/a', ?);
+        INSERT INTO comparator_question (question, timestamp)
+        VALUES (?, ?);
         """
         with self._lock:
             cursor = self.get_cursor()
-            cursor.execute(query, (question, answer, timestamp))
+            cursor.execute(query, (question, timestamp))
             self.get_connection().commit()
 
         if self._debug:
-            rows = self.retrieve_all_question_answers()
+            rows = self.retrieve_all()
             print("Table contents after inserting table:")
             self.print_table(rows)
 
         return cursor.lastrowid
 
-    def update_vote_status(self, id, vote_status):
+    def update(self, **kwargs) -> None:
+        """
+        Updates the database.
         """
-        Updates the vote status of a question-answer pair with the given ID.
+        raise NotImplementedError(
+            "ComparatorQuestionDatabase does not support update.")
 
-        Args:
-            id (int): The ID of the question-answer pair to update.
-            vote_status (str): The new vote status to set. Must be one of 'up', 'down', or 'n/a'.
+    def retrieve_all(self) -> List[Tuple]:
+        """
+        Retrieves all pairs from the database.
 
-        Raises:
-            ValueError: If the question with the given ID does not exist.
+        Returns:
+            list: A list of tuples.
         """
         query = """
-        UPDATE question_answer
-        SET vote_status = ?
-        WHERE id = ?;
+        SELECT * FROM comparator_question;
         """
         with self._lock:
             cursor = self.get_cursor()
-            cursor.execute(query, (vote_status, id))
-            self.get_connection().commit()
+            cursor.execute(query)
+            rows = cursor.fetchall()
+        return rows
+
+    def print_table(self, rows: List[Tuple]) -> None:
+        """
+        Prints the contents of the table in a formatted manner.
+
+        Args:
+            rows (list): A list of tuples where each tuple represents a row in the table.
+                        Each tuple contains five elements: ID, Question.
+        """
+        for row in rows:
+            print(
+                f"ID: {row[0]}, Question: {row[1]}, Timestamp: {row[2]}"
+            )
+
+
+class ComparatorDatabase(AbsDatabase):
+    """ComparatorDatabase class."""
+
+    def __init__(self,
+                 db_file: str = os.path.join(os.getcwd(), "comparator.db"),
+                 debug: bool = False) -> None:
+        query = """
+        CREATE TABLE IF NOT EXISTS comparator (
+            id INTEGER PRIMARY KEY AUTOINCREMENT,
+            model TEXT NOT NULL,
+            qid INTEGER NOT NULL,
+            rank INTEGER NOT NULL,
+            answer TEXT NOT NULL,
+            timestamp TIMESTAMP DEFAULT CURRENT_TIMESTAMP
+            );
+            """
+        super().__init__(db_file, debug)
+        self.create_table(query)
+
+    def insert(self, **kwargs) -> None:
+        """
+        Inserts a new row into the comparator table.
+
+        Args:
+            kwargs (dict): The key-value pairs to insert into the database.
+        """
+        timestamp = datetime.datetime.now()
+        check_query = """
+        SELECT * FROM comparator
+        WHERE model = ? AND qid = ?;
+        """
+        with self._lock:
+            cursor = self.get_cursor()
+            cursor.execute(check_query, (kwargs["model"], kwargs["qid"]))
+            existing_row = cursor.fetchone()
+
+            if existing_row is not None:
+                raise ValueError(f"Row with model={kwargs['model']} and qid={kwargs['qid']} already exists")
 
-        if cursor.rowcount == 0:
-            raise ValueError(f"Question with ID {id} does not exist.")
+            query = """
+            INSERT INTO comparator (model, qid, rank, answer, timestamp)
+            VALUES (?, ?, ?, ?, ?);
+            """
+            cursor.execute(query,
+                           (kwargs["model"],
+                            kwargs["qid"],
+                            kwargs["rank"],
+                            kwargs["answer"],
+                            timestamp))
+            self.get_connection().commit()
 
         if self._debug:
-            rows = self.retrieve_all_question_answers()
-            print("Table contents after updating table:")
+            rows = self.retrieve_all()
+            print("Table contents after inserting table")
             self.print_table(rows)
 
-    def retrieve_all_question_answers(self):
+    def update(self, **kwargs) -> None:
         """
-        Retrieves all question-answer pairs from the database.
+        Updates the rank of a row in the comparator table by its id.
 
-        Returns:
-            list: A list of tuples representing the question-answer pairs.
+        Args:
+            kwargs (dict): The key-value pairs to update in the database.
         """
         query = """
-        SELECT * FROM question_answer;
+        UPDATE comparator
+        SET rank = ?
+        WHERE qid = ? AND model = ?;
         """
         with self._lock:
             cursor = self.get_cursor()
-            cursor.execute(query)
-            rows = cursor.fetchall()
-        return rows
+            cursor.execute(
+                query,
+                (kwargs["rank"],
+                 kwargs["qid"],
+                 kwargs["model"]))
+            self.get_connection().commit()
+        if self._debug:
+            rows = self.retrieve_all()
+            print("Table contents after updating table")
+            self.print_table(rows)
 
-    def retrieve_all_question_answers_as_pandas(self):
+    def retrieve_all(self) -> List[Tuple]:
         """
-        Retrieves all question-answer pairs from the database as a pandas dataframe.
+        Retrieves all pairs from the database.
 
         Returns:
-            DataFrame: A pandas dataframe.
+            list: A list of tuples.
         """
-        rows = self.retrieve_all_question_answers()
-        rows_to_pd = pd.DataFrame(rows)
-        rows_to_pd.columns = QA_CSV_HEADER
-        return rows_to_pd
-
-    def close_connection(self):
-        """
-        Closes the connection to the database.
+        query = """
+        SELECT * FROM comparator;
         """
-        if hasattr(self._local, "cursor"):
-            self._local.cursor.close()
-            del self._local.cursor
-        if hasattr(self._local, "connection"):
-            self._local.connection.close()
-            del self._local.connection
+        with self._lock:
+            cursor = self.get_cursor()
+            cursor.execute(query)
+            rows = cursor.fetchall()
+        return rows
 
-    def print_table(self, rows):
+    def print_table(self, rows: List[Tuple]) -> None:
         """
-        Prints the contents of the table in a formatted manner.
+        Prints the comparator table.
 
         Args:
             rows (list): A list of tuples where each tuple represents a row in the table.
-                        Each tuple contains five elements: ID, Question, Answer, Timestamp, and Vote Status.
+                        Each tuple contains five elements: ID, Model, QID, Rank, Answer, Timestamp.
         """
         for row in rows:
             print(
-                f"ID: {row[0]}, Question: {row[1]}, "
-                f"Answer: {row[2]}, Vote Status: {row[3]}, Timestamp: {row[4]}"
+                f"ID: {row[0]}, "
+                f"Model: {row[1]}, "
+                f"QID: {row[2]}, "
+                f"Rank: {row[3]}, "
+                f"Answer: {row[4]}, "
+                f"Timestamp: {row[5]}"
             )
-
-    def save_to_csv(self, csv_file_name="question_answer_votes.csv"):
-        """
-        This method saves the contents of the question_answer table into a CSV file.
-
-        Args:
-            csv_file_name (str, optional): The name of the CSV file to which the data will be written.
-            Defaults to "question_answer_votes.csv".
-
-        The CSV file will have the following columns: ID, Question, Answer, Vote Status. Each row in the
-        CSV file corresponds to a row in the question_answer table.
-
-        This method first retrieves all question-answer pairs from the database by calling the
-        retrieve_all_question_answers method. It then writes this data to the CSV file.
-        """
-        my_sql_data = self.retrieve_all_question_answers()
-
-        with open(csv_file_name, "w", newline="") as file:
-            writer = csv.writer(file)
-            writer.writerow(QA_CSV_HEADER)
-            writer.writerows(my_sql_data)
```

### Comparing `pykoi-0.0.1/pykoi/db/ranking_database.py` & `pykoi-0.0.2/pykoi/db/ranking_database.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,16 @@
 """This file contains the RankingDatabase class which is used to store and retrieve"""
 import csv
 import os
 import sqlite3
 import threading
 
-CSV_HEADER_ID = "ID"
-CSV_HEADER_QUESTION = "Question"
-RANKING_CSV_HEADER_UP_RANKING_ANSWER = "Up Ranking Answer"
-RANKING_CSV_HEADER_LOW_RANKING_ANSWER = "Low Ranking Answer"
-RANKING_CSV_HEADER = (
-    CSV_HEADER_ID,
-    CSV_HEADER_QUESTION,
-    RANKING_CSV_HEADER_UP_RANKING_ANSWER,
-    RANKING_CSV_HEADER_LOW_RANKING_ANSWER,
-)
+import pandas as pd
+
+from pykoi.db.constants import RANKING_CSV_HEADER
 
 
 class RankingDatabase:
     """Ranking Database class"""
 
     def __init__(
         self,
@@ -160,7 +153,19 @@
         """
         ranking_data = self.retrieve_all_question_answers()
 
         with open(csv_file_name, "w", newline="") as file:
             writer = csv.writer(file)
             writer.writerow(RANKING_CSV_HEADER)
             writer.writerows(ranking_data)
+
+    def retrieve_all_question_answers_as_pandas(self):
+        """
+        Retrieves pairs from the database as a pandas dataframe.
+
+        Returns:
+            DataFrame: A pandas dataframe.
+        """
+        rows = self.retrieve_all_question_answers()
+        rows_to_pd = pd.DataFrame(rows)
+        rows_to_pd.columns = RANKING_CSV_HEADER
+        return rows_to_pd
```

### Comparing `pykoi-0.0.1/pykoi/frontend/README.md` & `pykoi-0.0.2/pykoi/frontend/README.md`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.1/pykoi/frontend/dist/assets/index-cf40d152.css` & `pykoi-0.0.2/pykoi/frontend/dist/assets/index-f75c1c12.css`

 * *Files 19% similar despite different names*

```diff
@@ -1 +1 @@
-@import"https://fonts.googleapis.com/css?family=Work+Sans:400|Lato:400|Inconsolata:400";:root{font-family:Inter,system-ui,Avenir,Helvetica,Arial,sans-serif;line-height:1.5;font-weight:400;color-scheme:light dark;color:#ffffffde;background-color:#242424;font-synthesis:none;text-rendering:optimizeLegibility;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;-webkit-text-size-adjust:100%}a{font-weight:500;color:#646cff;text-decoration:inherit}a:hover{color:#535bf2}body{margin:auto;width:100%}h1{font-size:3.2em;line-height:1.1}.card{padding:2em}#app{margin:0 auto;text-align:center}button{border-radius:8px;border:1px solid transparent;padding:.6em 1.2em;font-size:1em;font-weight:500;font-family:inherit;background-color:#1a1a1a;cursor:pointer;transition:border-color .25s}button:hover{border-color:#646cff}button:focus,button:focus-visible{outline:4px auto -webkit-focus-ring-color}@media (prefers-color-scheme: light){:root{color:#213547;background-color:#fff}a:hover{color:#747bff}button{background-color:#f9f9f9}}:root{--green: #00ebc7;--red: #FF5470;--yellow: #fde24f;--black: #1b2d45;--darkBlue: #00214d;--darkGrey: #222;--grey: #bfbfbf;--lightGrey: #f2f4f6;--white: white;--primary: var(--yellow);--danger: var(--red);--background: var(--lightGrey);--textColor: var(--black);--lineColor: var(--grey);--cardBg: var(--white);--headerBackground: var(--white);--footerBackground: var(--darkBlue);--footerTextColor: var(--lightGrey);--headerTextColor: var(--black);--buttonColor: var(--primary);--buttonTextColor: var(--textColor);--borderBottom: solid 2px var(--primary);--line: solid 1px var(--lineColor);--headingFont: "Lato", monospace;--bodyFont: "Inconsolata", sans-serif;--baseFontSize: 100%;--h1: 3.052em;--h2: 2.441em;--h3: 1.953em;--h4: 1.563em;--h5: 1.25em;--smallText: .8em;--shadow-s: 0 1px 3px 0 rgb(0 0 0 / .1), 0 1px 2px -1px rgb(0 0 0 / .1);--shadow-md: 0 4px 6px -1px rgb(0 0 0 / .1), 0 2px 4px -2px rgb(0 0 0 / .1);--shadow-lg: 0 10px 15px -3px rgb(0 0 0 / .1), 0 4px 6px -4px rgb(0 0 0 / .1);--shadow-xl: 0 20px 25px -5px rgb(0 0 0 / .1), 0 8px 10px -6px rgb(0 0 0 / .1);--containerPadding: 2.5%;--headerHeight: 3rem;--borderRadius: 0px}header{color:var(--headerTextColor);position:fixed;left:0;top:0;width:100%;height:var(--headerHeight);background:var(--headerBackground);border-bottom:var(--line);display:flex;justify-content:space-between;align-items:center;padding:0 var(--containerPadding)}footer{color:var(--footerTextColor);background-color:var(--footerBackground);padding:calc(var(--headerHeight) * .75) var(--containerPadding);text-align:center;position:absolute;bottom:0;width:100%}button{-webkit-appearance:none;-moz-appearance:none;appearance:none;color:var(--buttonTextColor);background-color:var(--white);border:var(--line);border-radius:var(--borderRadius);padding:5px 25px;box-shadow:var(--shadow-s);transition:.3s ease-in-out box-shadow}.dark{--background: var(--black);--textColor: var(--lightGrey);--headerBackground: var(--darkGrey);--footerBackground: var(--darkGrey);--cardBg: var(--darkGrey);--buttonTextColor: var(--black)}.theme{--green: #00ebc7;--red: #FF5470;--yellow: #fde24f;--black: #1b2d45;--darkBlue: #00214d;--darkGrey: #222;--grey: #bfbfbf;--lightGrey: #f2f4f6;--white: white;--primary: var(--green);--danger: var(--red);--background: var(--lightGrey);--textColor: var(--black);--lineColor: var(--grey);--cardBg: var(--white);--headerBackground: var(--darkBlue);--footerBackground: var(--darkBlue);--footerTextColor: var(--lightGrey);--buttonColor: var(--primary);--buttonTextColor: var(--textColor);--line: solid 1px var(--lineColor);--headingFont: "Lato", monospace;--bodyFont: "Work Sans", sans-serif;--baseFontSize: 100%;--h1: 3.052em;--h2: 2.441em;--h3: 1.953em;--h4: 1.563em;--h5: 1.25em;--smallText: .8em;--shadow-s: 0 1px 3px 0 rgb(0 0 0 / .1), 0 1px 2px -1px rgb(0 0 0 / .1);--shadow-md: 0 4px 6px -1px rgb(0 0 0 / .1), 0 2px 4px -2px rgb(0 0 0 / .1);--shadow-lg: 0 10px 15px -3px rgb(0 0 0 / .1), 0 4px 6px -4px rgb(0 0 0 / .1);--shadow-xl: 0 20px 25px -5px rgb(0 0 0 / .1), 0 8px 10px -6px rgb(0 0 0 / .1);--containerPadding: 2.5%;--headerHeight: 3rem;--borderRadius: 10px}:root{--left: 300px}/*! normalize.css v8.0.1 | MIT License | github.com/necolas/normalize.css */html{line-height:1.15;-webkit-text-size-adjust:100%}body{margin:0}main{display:block}h1{font-size:2em;margin:.67em 0}hr{box-sizing:content-box;height:0;overflow:visible}pre{font-family:monospace,monospace;font-size:1em}a{background-color:transparent}abbr[title]{border-bottom:none;text-decoration:underline;text-decoration:underline dotted}b,strong{font-weight:bolder}code,kbd,samp{font-family:monospace,monospace;font-size:1em}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}img{border-style:none}button,input,optgroup,select,textarea{font-family:inherit;font-size:100%;line-height:1.15;margin:0}button,input{overflow:visible}button,select{text-transform:none}button,[type=button],[type=reset],[type=submit]{-webkit-appearance:button}button::-moz-focus-inner,[type=button]::-moz-focus-inner,[type=reset]::-moz-focus-inner,[type=submit]::-moz-focus-inner{border-style:none;padding:0}button:-moz-focusring,[type=button]:-moz-focusring,[type=reset]:-moz-focusring,[type=submit]:-moz-focusring{outline:1px dotted ButtonText}fieldset{padding:.35em .75em .625em}legend{box-sizing:border-box;color:inherit;display:table;max-width:100%;padding:0;white-space:normal}progress{vertical-align:baseline}textarea{overflow:auto}[type=checkbox],[type=radio]{box-sizing:border-box;padding:0}[type=number]::-webkit-inner-spin-button,[type=number]::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}[type=search]::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}details{display:block}summary{display:list-item}template{display:none}[hidden]{display:none}:root{--green: #00ebc7;--red: #FF5470;--yellow: #fde24f;--black: #1b2d45;--darkBlue: #00214d;--darkGrey: #222;--grey: #bfbfbf;--lightGrey: #f2f4f6;--white: white;--primary: var(--yellow);--danger: var(--red);--background: var(--white);--textColor: var(--black);--lineColor: var(--grey);--cardBg: var(--white);--headerBackground: var(--white);--footerBackground: var(--green);--footerTextColor: var(--black);--headerTextColor: var(--black);--buttonColor: var(--primary);--buttonTextColor: var(--textColor);--borderBottom: solid 2px var(--primary);--line: solid 1px var(--lineColor);--headingFont: "Lato", monospace;--bodyFont: "Work Sans", sans-serif;--baseFontSize: 100%;--h1: 3.052em;--h2: 2.441em;--h3: 1.953em;--h4: 1.563em;--h5: 1.25em;--smallText: .8em;--shadow-s: 0 1px 3px 0 rgb(0 0 0 / .1), 0 1px 2px -1px rgb(0 0 0 / .1);--shadow-md: 0 4px 6px -1px rgb(0 0 0 / .1), 0 2px 4px -2px rgb(0 0 0 / .1);--shadow-lg: 0 10px 15px -3px rgb(0 0 0 / .1), 0 4px 6px -4px rgb(0 0 0 / .1);--shadow-xl: 0 20px 25px -5px rgb(0 0 0 / .1), 0 8px 10px -6px rgb(0 0 0 / .1);--containerPadding: 2.5%;--headerHeight: 3rem;--borderRadius: 0px;--height: height: calc(100vh - var(--headerHeight))}html{box-sizing:border-box;font-size:var(--baseFontSize)}*,*:before,*:after{box-sizing:inherit}body{font-family:var(--bodyFont);font-weight:400;line-height:1.75;background:var(--background);color:var(--textColor)}header{color:var(--headerTextColor);margin-top:1%;height:var(--headerHeight);background:var(--headerBackground);font-size:var(--h5);display:flex;justify-content:space-between;align-items:center;padding:0 var(--containerPadding)}header nav a{color:var(--white);text-decoration:none}header nav a+a{margin-left:10px}footer{color:var(--footerTextColor);background-color:var(--footerBackground);padding:calc(var(--headerHeight) * .75) var(--containerPadding);text-align:center;bottom:0;width:100%}footer a{color:var(--footerTextColor)}footer nav a+a{margin-left:10px}footer p{margin-bottom:0;max-width:none}p{margin-bottom:1rem}p a,blockquote a{color:var(--textColor);text-decoration:none;border-bottom:var(--borderBottom)}h1,h2,h3,h4,h5{margin:3rem 0 1.38rem;font-family:var(--headingFont);font-weight:400;line-height:1.15}h1{margin-top:0;font-size:var(--h1)}h2{font-size:var(--h2)}h3{font-size:var(--h3)}h4{font-size:var(--h4)}h5{font-size:var(--h5)}small,.text_small{font-size:var(--smallText)}blockquote{margin:10px;padding:2em;background:var(--cardBg);box-shadow:var(--shadow-lg)}label{display:block;font-size:var(--smallText)}input,textarea{padding:2px 5px;border:var(--line);border-radius:4px}textarea{width:100%;height:5rem}::placeholder{color:var(--grey)}::selection,.highlight{background:#ffb7b7;background:var(--red);color:var(--white)}select{border:var(--line)}hr{border-top:var(--line)}button{-webkit-appearance:none;-moz-appearance:none;appearance:none;color:var(--buttonTextColor);background-color:var(--white);border:var(--line);border-radius:var(--borderRadius);padding:10px 25px;box-shadow:var(--shadow-s);transition:.3s ease-in-out box-shadow}button:hover{cursor:pointer;box-shadow:var(--shadow-md)}button[disabled]{opacity:.4}button.cancel{--buttonColor: var(--danger);--buttonTextColor: var(--white)}button.small{font-size:var(--smallText)}.layout{padding-top:calc(0rem + var(--headerHeight))}.grid{--gridCols: 2;display:block;grid-template-columns:repeat(var(--gridCols),1fr)}.cols-3{--gridCols: 3}.cols-4{--gridCols: 4}.flex{--justifyContent: space-between;display:block;justify-content:var(--justifyContent)}.flex-around{--justifyContent: space-around}.card{padding:2em;background:var(--cardBg);box-shadow:var(--shadow-lg);border-radius:var(--borderRadius)}.grid-split{display:grid;grid-template-columns:33% 67%;gap:20px}@media only screen and (min-width: 600px){:root{--baseFontSize: 100%}.grid{display:grid}.flex{display:flex}}.logo{font-size:var(--baseFontSize);margin:0 0 0 8px}.dark{--background: var(--black);--textColor: var(--lightGrey);--headerBackground: var(--darkGrey);--footerBackground: var(--yellow);--cardBg: var(--darkGrey);--buttonTextColor: var(--black)}.oled{--black: #000;--cardBg: var(--darkGrey);--headerBackground: var(--darkGrey);--footerBackground: var(--darkGrey)}.theme{--green: #00ebc7;--red: #FF5470;--yellow: #fde24f;--black: #1b2d45;--darkBlue: #00214d;--darkGrey: #222;--grey: #bfbfbf;--lightGrey: #f2f4f6;--white: white;--primary: var(--green);--danger: var(--red);--background: var(--lightGrey);--textColor: var(--black);--lineColor: var(--grey);--cardBg: var(--white);--headerBackground: var(--darkBlue);--footerBackground: var(--darkBlue);--footerTextColor: var(--black);--buttonColor: var(--primary);--buttonTextColor: var(--textColor);--line: solid 1px var(--lineColor);--headingFont: "Lato", monospace;--bodyFont: "Work Sans", sans-serif;--baseFontSize: 100%;--h1: 3.052em;--h2: 2.441em;--h3: 1.953em;--h4: 1.563em;--h5: 1.25em;--smallText: .8em;--shadow-s: 0 1px 3px 0 rgb(0 0 0 / .1), 0 1px 2px -1px rgb(0 0 0 / .1);--shadow-md: 0 4px 6px -1px rgb(0 0 0 / .1), 0 2px 4px -2px rgb(0 0 0 / .1);--shadow-lg: 0 10px 15px -3px rgb(0 0 0 / .1), 0 4px 6px -4px rgb(0 0 0 / .1);--shadow-xl: 0 20px 25px -5px rgb(0 0 0 / .1), 0 8px 10px -6px rgb(0 0 0 / .1);--containerPadding: 2.5%;--headerHeight: 3rem;--borderRadius: 10px}:root{--left: 25px}.grid-sidemenu{--gridCols: 2;display:grid;grid-template-columns:var(--left) 1fr}header{padding:0 15px 0 0}header nav a+a{margin-left:15px}.corner{margin-left:var(--left)}header nav a{color:var(--black);text-decoration:none}.page{padding:3em}.page-title{text-decoration:none;border-bottom:var(--borderBottom)}.card{padding:2em;background:var(--cardBg);box-shadow:var(--shadow-lg);border-radius:var(--borderRadius);font-size:var(--smallText)}.card:hover{box-shadow:var(--shadow-xl)}.card>*:first-child{margin-top:0}.card>*:last-child{margin-bottom:0}table{margin:auto}button{margin:5px}.small-button.svelte-9ap43o.svelte-9ap43o{margin-left:10px;background:none;border:3px solid transparent;color:inherit;padding:6px 10px;cursor:pointer;box-shadow:none;font-size:var(--smallText)}.feedback-buttons.svelte-9ap43o.svelte-9ap43o{text-align:center;margin:auto;width:20%}.small-button.svelte-9ap43o.svelte-9ap43o:hover{box-shadow:var(--shadow-md)}.thumbs-up.svelte-9ap43o.svelte-9ap43o,.thumbs-up.svelte-9ap43o.svelte-9ap43o:hover,.thumbs-up.svelte-9ap43o.svelte-9ap43o::selection{background:var(--green)}.thumbs-down.svelte-9ap43o.svelte-9ap43o,.thumbs-down.svelte-9ap43o.svelte-9ap43o:hover,.thumbs-down.svelte-9ap43o.svelte-9ap43o::selection{background:var(--red)}.ranked-chat.svelte-9ap43o.svelte-9ap43o{height:100vh;display:grid;grid-template-columns:100%;grid-template-rows:80% 20%}.message.svelte-9ap43o.svelte-9ap43o{font-size:var(--smallText);padding-left:40px;padding-right:40px;margin:0 auto}.chat-input-holder.svelte-9ap43o.svelte-9ap43o{display:flex;flex-direction:column;align-items:center;padding:24px;width:100%;max-width:640px;margin:auto}.chat-input-textarea.svelte-9ap43o.svelte-9ap43o{background-color:var(--lightgrey);cursor:pointer;width:100%;border:var(--line);border-color:none;margin:12px;outline:none;padding:12px;color:var(--black);font-size:var(--baseFontSize);box-shadow:var(--shadow-md);flex:3;border-radius:0;border-right:0px}.chat-input-form.svelte-9ap43o.svelte-9ap43o{display:flex;width:100%}.btnyousend.svelte-9ap43o.svelte-9ap43o{border-radius:0;margin-top:12px;margin-bottom:12px;margin-left:-15px;background:var(--primary);color:var(--black);opacity:.5;transition:all .3s}.active.svelte-9ap43o.svelte-9ap43o{opacity:1}.green.svelte-9ap43o.svelte-9ap43o{border-bottom:2px solid var(--green)}.red.svelte-9ap43o.svelte-9ap43o{border-bottom:2px solid var(--red)}.instructions.svelte-9ap43o.svelte-9ap43o{text-align:center;padding:5%}.instructions.svelte-9ap43o h5.svelte-9ap43o{text-align:left}.instructions.svelte-9ap43o p.svelte-9ap43o{font-size:var(--smallText);text-align:left}.instructions.svelte-9ap43o button.svelte-9ap43o{font-size:var(--smallText)}.ranked-feedback-container.svelte-9ap43o.svelte-9ap43o{display:grid;grid-template-columns:20% 80%}.underline.svelte-9ap43o.svelte-9ap43o{border-bottom:var(--line)}.bold.svelte-9ap43o.svelte-9ap43o{font-weight:700;font-size:var(--smallText);margin:0;padding:0}.chatbox.svelte-9ap43o.svelte-9ap43o{display:flex;flex-direction:column;justify-content:space-between;height:calc(100vh - var(--headerHeight));background-color:var(--white);box-sizing:border-box;width:95%;margin:auto;height:100%}.chat-log.svelte-9ap43o.svelte-9ap43o{flex:1;overflow-y:auto;padding:0 10px;box-sizing:border-box}.chat-message.svelte-9ap43o.svelte-9ap43o{background-color:var(--white);border-bottom:var(--line);box-sizing:border-box}.chat-message-center.svelte-9ap43o.svelte-9ap43o{display:flex;flex-direction:column;margin-left:auto;margin-right:auto;padding:12px;box-sizing:border-box}.message-content.svelte-9ap43o.svelte-9ap43o{display:flex;flex-direction:column;box-sizing:border-box}.message-content.svelte-9ap43o .question.svelte-9ap43o{text-align:left;border:1px solid var(--grey);padding:5px;background-color:var(--lightGrey)}.message-content.svelte-9ap43o .answer.svelte-9ap43o{display:inline-block;text-align:left;padding:10px;border:1px solid var(--black)}.message-content.svelte-9ap43o .answers.svelte-9ap43o{display:grid;grid-template-columns:100%;gap:0%;width:100%;margin:auto}.ranked-chat.svelte-au920n.svelte-au920n{height:100vh;display:grid;grid-template-columns:100%;grid-template-rows:80% 20%}.message.svelte-au920n.svelte-au920n{font-size:var(--smallText);padding-left:40px;padding-right:40px;margin:0 auto}.chat-input-holder.svelte-au920n.svelte-au920n{display:flex;flex-direction:column;align-items:center;padding:24px;width:100%;max-width:640px;margin:auto}.chat-input-textarea.svelte-au920n.svelte-au920n{background-color:var(--lightgrey);cursor:pointer;width:100%;border:var(--line);border-color:none;margin:12px;outline:none;padding:12px;color:var(--black);font-size:var(--baseFontSize);box-shadow:var(--shadow-md);flex:3;border-radius:0;border-right:0px}.chat-input-form.svelte-au920n.svelte-au920n{display:flex;width:100%}.btnyousend.svelte-au920n.svelte-au920n{border-radius:0;margin-top:12px;margin-bottom:12px;margin-left:-15px;background:var(--primary);color:var(--black);opacity:.5;transition:all .3s}.active.svelte-au920n.svelte-au920n{opacity:1}.green.svelte-au920n.svelte-au920n{border-bottom:2px solid var(--green)}.red.svelte-au920n.svelte-au920n{border-bottom:2px solid var(--red)}.instructions.svelte-au920n.svelte-au920n{text-align:center;padding:5%}.instructions.svelte-au920n h5.svelte-au920n{text-align:left}.instructions.svelte-au920n p.svelte-au920n{font-size:var(--smallText);text-align:left}.instructions.svelte-au920n button.svelte-au920n{font-size:var(--smallText)}.ranked-feedback-container.svelte-au920n.svelte-au920n{display:grid;grid-template-columns:20% 80%}.underline.svelte-au920n.svelte-au920n{border-bottom:var(--line)}.bold.svelte-au920n.svelte-au920n{font-weight:700;font-size:var(--smallText);margin:0;padding:0}.chatbox.svelte-au920n.svelte-au920n{display:flex;flex-direction:column;justify-content:space-between;height:calc(100vh - var(--headerHeight));background-color:var(--white);box-sizing:border-box;width:95%;margin:auto;height:100%}.chat-log.svelte-au920n.svelte-au920n{flex:1;overflow-y:auto;padding:0 10px;box-sizing:border-box}.chat-message.svelte-au920n.svelte-au920n{background-color:var(--white);border-bottom:var(--line);box-sizing:border-box}.chat-message-center.svelte-au920n.svelte-au920n{display:flex;flex-direction:column;margin-left:auto;margin-right:auto;padding:12px;box-sizing:border-box}.message-content.svelte-au920n.svelte-au920n{display:flex;flex-direction:column;box-sizing:border-box}.message-content.svelte-au920n .question.svelte-au920n{text-align:left;border:1px solid var(--grey);padding:5px;margin-bottom:10px;background-color:var(--lightGrey)}.message-content.svelte-au920n .answer.svelte-au920n{display:inline-block;text-align:left;padding:10px;border:1px solid var(--black)}.message-content.svelte-au920n .answers.svelte-au920n{display:grid;grid-template-columns:49% 49%;gap:2%;width:100%;margin:auto}.series.svelte-tg5p7i:focus{outline:none}.horizontal-bar-rect.selected.svelte-tg5p7i{stroke:var(--black);stroke-width:3}#stackedrect-holder.svelte-tg5p7i{height:100%;width:100%}.line.svelte-tg5p7i{stroke-width:3;stroke:var(--black);fill:none}.horizontal-bar-rect.svelte-tg5p7i{transition:opacity .3s}.horizontal-bar-rect.svelte-tg5p7i:hover{stroke:var(--black);stroke-width:3}.horizontal-bar-text.svelte-tg5p7i{transition:opacity .3s;stroke:var(--white);stroke-width:4px;fill:var(--black);stroke-linejoin:round;paint-order:stroke fill;pointer-events:none;font-size:var(--smallText)}.qa-card.svelte-szi0e{border:2px solid var(--black);display:flex;flex-direction:column;font-size:var(--smallText);padding:4px;margin:6px}.qa-card.svelte-szi0e:hover{border:3px solid var(--black)}.question.svelte-szi0e{background-color:var(--white);margin:0;padding:8px;border-bottom:1px solid var(--black)}.answer.svelte-szi0e{background-color:var(--lightGrey);margin:0;padding:8px}.feedback.svelte-szi0e{margin:0;padding:8px}.up.svelte-szi0e{background-color:var(--green)}.down.svelte-szi0e{background-color:var(--red)}.na.svelte-szi0e{background-color:var(--yellow)}.qa-container.svelte-1xv9cfi{border:2px solid var(--background);max-height:100%;overflow-y:auto}.chart-title.svelte-1oikip4{font-size:var(--smallText)}rect.svelte-1oikip4:hover{stroke:var(--black)}#stackedrect-holder.svelte-1oikip4{height:100%;width:100%}.axis-line.svelte-1oikip4{stroke-width:3;stroke:var(--black);fill:none}.axis-tick.svelte-1oikip4{stroke-width:1;fill:none;opacity:0;font-size:9px}.axis-text.svelte-1oikip4{font-size:calc(var(--smallText) * .9)}.svelte-kz2qh6{transition:all .3s}.chart-title.svelte-kz2qh6{font-size:var(--smallText)}rect.svelte-kz2qh6:hover{stroke:var(--black)}.histogram-container.svelte-kz2qh6{height:100%;width:100%}.axis-line.svelte-kz2qh6{stroke-width:3;stroke:var(--black);fill:none}.axis-tick.svelte-kz2qh6{stroke-width:1;fill:none;opacity:0;font-size:9px}.axis-text.svelte-kz2qh6{font-size:calc(var(--smallText) * .9)}.svelte-1pknxov{font-family:Lato}.card-container.svelte-1pknxov{border:2px solid var(--black);width:100%;height:100%;display:grid;grid-template-columns:100%;grid-template-rows:35% 50% 10%;padding:5px;box-sizing:border-box}.card-text.svelte-1pknxov{text-align:left;margin:0;padding:0 0 0 2px;font-weight:700;font-size:.8em}#feedback-dropdown.svelte-1pknxov{width:98%;border:none;border-bottom:1px solid var(--black);border-top:1px solid var(--black);font-size:var(--smallText);margin-bottom:1px}svg.svelte-1pknxov{width:100%;height:100%;border-bottom:1px solid var(--black)}.small.svelte-1pknxov{font-size:.6em}text.svelte-1pknxov{font-size:3rem;transition:opacity .3s;stroke:#fff;stroke-width:6px;fill:var(--black);stroke-linejoin:round;paint-order:stroke fill;pointer-events:none}.card-container.svelte-mchgj2{border:2px solid var(--black);width:100%;height:100%;display:grid;grid-template-columns:100%;grid-template-rows:35% 50% 10%;padding:5px;box-sizing:border-box}.card-text.svelte-mchgj2{text-align:left;margin:0;padding:0 0 0 2px;font-weight:700;font-size:.8em}#feedback-dropdown.svelte-mchgj2{width:98%;border:none;border-bottom:1px solid var(--black);border-top:1px solid var(--black);font-size:var(--smallText);margin-bottom:1px}svg.svelte-mchgj2{width:100%;height:100%;border-bottom:1px solid var(--black)}.small.svelte-mchgj2{font-size:.6em}text.svelte-mchgj2{font-size:3rem;transition:opacity .3s;stroke:#fff;stroke-width:6px;fill:var(--black);stroke-linejoin:round;paint-order:stroke fill;pointer-events:none}.feedback-container.svelte-14znspc{border-bottom:var(--line);border-right:var(--line);display:grid;grid-template-columns:30% 70%;grid-template-rows:100%;width:90%;height:calc(100vh - var(--headerHeight))}.feedback-left.svelte-14znspc{border-bottom:var(--line);display:grid;grid-template-columns:100%;grid-template-rows:25% 25% 25% 12.5% 12.5%}.left-text.svelte-14znspc{text-align:center;border-bottom:var(--line);border-right:var(--line);display:grid;grid-template-rows:100%;grid-template-columns:50% 50%}.left-confidence.svelte-14znspc{text-align:center;border-bottom:var(--line);border-right:var(--line);display:grid;grid-template-rows:40% 55%}.left-question.svelte-14znspc,.left-filter.svelte-14znspc{border-bottom:var(--line);border-right:var(--line)}.feedback-right.svelte-14znspc{border-bottom:var(--line);border-right:var(--line);display:grid;grid-template-columns:100%;grid-template-rows:30% 70%;grid-template-rows:0% 100%}.right-chart.svelte-14znspc{border-bottom:var(--line);border-right:var(--line);display:grid;grid-template-columns:50% 50%;grid-template-rows:100%}.right-chart-1.svelte-14znspc,.right-chart-2.svelte-14znspc{border-right:var(--line)}.right-table.svelte-14znspc{border-bottom:var(--line);border-right:var(--line)}.card-1.svelte-14znspc{border-right:var(--line)}
+@import"https://fonts.googleapis.com/css?family=Work+Sans:400|Lato:400|Inconsolata:400";:root{font-family:Inter,system-ui,Avenir,Helvetica,Arial,sans-serif;line-height:1.5;font-weight:400;color-scheme:light dark;color:#ffffffde;background-color:#242424;font-synthesis:none;text-rendering:optimizeLegibility;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;-webkit-text-size-adjust:100%}a{font-weight:500;color:#646cff;text-decoration:inherit}a:hover{color:#535bf2}body{margin:auto;width:100%}h1{font-size:3.2em;line-height:1.1}.card{padding:2em}#app{margin:0 auto;text-align:center}button{border-radius:8px;border:1px solid transparent;padding:.6em 1.2em;font-size:1em;font-weight:500;font-family:inherit;background-color:#1a1a1a;cursor:pointer;transition:border-color .25s}button:hover{border-color:#646cff}button:focus,button:focus-visible{outline:4px auto -webkit-focus-ring-color}@media (prefers-color-scheme: light){:root{color:#213547;background-color:#fff}a:hover{color:#747bff}button{background-color:#f9f9f9}}:root{--green: #00ebc7;--red: #FF5470;--yellow: #fde24f;--black: #1b2d45;--darkBlue: #00214d;--darkGrey: #222;--grey: #bfbfbf;--lightGrey: #f2f4f6;--white: white;--primary: var(--yellow);--danger: var(--red);--background: var(--lightGrey);--textColor: var(--black);--lineColor: var(--grey);--cardBg: var(--white);--headerBackground: var(--white);--footerBackground: var(--darkBlue);--footerTextColor: var(--lightGrey);--headerTextColor: var(--black);--buttonColor: var(--primary);--buttonTextColor: var(--textColor);--borderBottom: solid 2px var(--primary);--line: solid 1px var(--lineColor);--headingFont: "Lato", monospace;--bodyFont: "Inconsolata", sans-serif;--baseFontSize: 100%;--h1: 3.052em;--h2: 2.441em;--h3: 1.953em;--h4: 1.563em;--h5: 1.25em;--smallText: .8em;--shadow-s: 0 1px 3px 0 rgb(0 0 0 / .1), 0 1px 2px -1px rgb(0 0 0 / .1);--shadow-md: 0 4px 6px -1px rgb(0 0 0 / .1), 0 2px 4px -2px rgb(0 0 0 / .1);--shadow-lg: 0 10px 15px -3px rgb(0 0 0 / .1), 0 4px 6px -4px rgb(0 0 0 / .1);--shadow-xl: 0 20px 25px -5px rgb(0 0 0 / .1), 0 8px 10px -6px rgb(0 0 0 / .1);--containerPadding: 2.5%;--headerHeight: 3rem;--borderRadius: 0px}header{color:var(--headerTextColor);position:fixed;left:0;top:0;width:100%;height:var(--headerHeight);background:var(--headerBackground);border-bottom:var(--line);display:flex;justify-content:space-between;align-items:center;padding:0 var(--containerPadding)}footer{color:var(--footerTextColor);background-color:var(--footerBackground);padding:calc(var(--headerHeight) * .75) var(--containerPadding);text-align:center;position:absolute;bottom:0;width:100%}button{-webkit-appearance:none;-moz-appearance:none;appearance:none;color:var(--buttonTextColor);background-color:var(--white);border:var(--line);border-radius:var(--borderRadius);padding:5px 25px;box-shadow:var(--shadow-s);transition:.3s ease-in-out box-shadow}.dark{--background: var(--black);--textColor: var(--lightGrey);--headerBackground: var(--darkGrey);--footerBackground: var(--darkGrey);--cardBg: var(--darkGrey);--buttonTextColor: var(--black)}.theme{--green: #00ebc7;--red: #FF5470;--yellow: #fde24f;--black: #1b2d45;--darkBlue: #00214d;--darkGrey: #222;--grey: #bfbfbf;--lightGrey: #f2f4f6;--white: white;--primary: var(--green);--danger: var(--red);--background: var(--lightGrey);--textColor: var(--black);--lineColor: var(--grey);--cardBg: var(--white);--headerBackground: var(--darkBlue);--footerBackground: var(--darkBlue);--footerTextColor: var(--lightGrey);--buttonColor: var(--primary);--buttonTextColor: var(--textColor);--line: solid 1px var(--lineColor);--headingFont: "Lato", monospace;--bodyFont: "Work Sans", sans-serif;--baseFontSize: 100%;--h1: 3.052em;--h2: 2.441em;--h3: 1.953em;--h4: 1.563em;--h5: 1.25em;--smallText: .8em;--shadow-s: 0 1px 3px 0 rgb(0 0 0 / .1), 0 1px 2px -1px rgb(0 0 0 / .1);--shadow-md: 0 4px 6px -1px rgb(0 0 0 / .1), 0 2px 4px -2px rgb(0 0 0 / .1);--shadow-lg: 0 10px 15px -3px rgb(0 0 0 / .1), 0 4px 6px -4px rgb(0 0 0 / .1);--shadow-xl: 0 20px 25px -5px rgb(0 0 0 / .1), 0 8px 10px -6px rgb(0 0 0 / .1);--containerPadding: 2.5%;--headerHeight: 3rem;--borderRadius: 10px}:root{--left: 300px}/*! normalize.css v8.0.1 | MIT License | github.com/necolas/normalize.css */html{line-height:1.15;-webkit-text-size-adjust:100%}body{margin:0}main{display:block}h1{font-size:2em;margin:.67em 0}hr{box-sizing:content-box;height:0;overflow:visible}pre{font-family:monospace,monospace;font-size:1em}a{background-color:transparent}abbr[title]{border-bottom:none;text-decoration:underline;text-decoration:underline dotted}b,strong{font-weight:bolder}code,kbd,samp{font-family:monospace,monospace;font-size:1em}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}img{border-style:none}button,input,optgroup,select,textarea{font-family:inherit;font-size:100%;line-height:1.15;margin:0}button,input{overflow:visible}button,select{text-transform:none}button,[type=button],[type=reset],[type=submit]{-webkit-appearance:button}button::-moz-focus-inner,[type=button]::-moz-focus-inner,[type=reset]::-moz-focus-inner,[type=submit]::-moz-focus-inner{border-style:none;padding:0}button:-moz-focusring,[type=button]:-moz-focusring,[type=reset]:-moz-focusring,[type=submit]:-moz-focusring{outline:1px dotted ButtonText}fieldset{padding:.35em .75em .625em}legend{box-sizing:border-box;color:inherit;display:table;max-width:100%;padding:0;white-space:normal}progress{vertical-align:baseline}textarea{overflow:auto}[type=checkbox],[type=radio]{box-sizing:border-box;padding:0}[type=number]::-webkit-inner-spin-button,[type=number]::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}[type=search]::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}details{display:block}summary{display:list-item}template{display:none}[hidden]{display:none}:root{--green: #00ebc7;--red: #FF5470;--yellow: #fde24f;--black: #1b2d45;--darkBlue: #00214d;--darkGrey: #222;--grey: #bfbfbf;--lightGrey: #f2f4f6;--white: white;--primary: var(--yellow);--danger: var(--red);--background: var(--white);--textColor: var(--black);--lineColor: var(--grey);--cardBg: var(--white);--headerBackground: var(--white);--footerBackground: var(--green);--footerTextColor: var(--black);--headerTextColor: var(--black);--buttonColor: var(--primary);--buttonTextColor: var(--textColor);--borderBottom: solid 2px var(--primary);--line: solid 1px var(--lineColor);--headingFont: "Lato", monospace;--bodyFont: "Work Sans", sans-serif;--baseFontSize: 100%;--h1: 3.052em;--h2: 2.441em;--h3: 1.953em;--h4: 1.563em;--h5: 1.25em;--smallText: .8em;--shadow-s: 0 1px 3px 0 rgb(0 0 0 / .1), 0 1px 2px -1px rgb(0 0 0 / .1);--shadow-md: 0 4px 6px -1px rgb(0 0 0 / .1), 0 2px 4px -2px rgb(0 0 0 / .1);--shadow-lg: 0 10px 15px -3px rgb(0 0 0 / .1), 0 4px 6px -4px rgb(0 0 0 / .1);--shadow-xl: 0 20px 25px -5px rgb(0 0 0 / .1), 0 8px 10px -6px rgb(0 0 0 / .1);--containerPadding: 2.5%;--headerHeight: 3rem;--borderRadius: 0px;--height: height: calc(100vh - var(--headerHeight))}html{box-sizing:border-box;font-size:var(--baseFontSize)}*,*:before,*:after{box-sizing:inherit}body{font-family:var(--bodyFont);font-weight:400;line-height:1.75;background:var(--background);color:var(--textColor)}header{color:var(--headerTextColor);margin-top:1%;height:var(--headerHeight);background:var(--headerBackground);font-size:var(--h5);display:flex;justify-content:space-between;align-items:center;padding:0 var(--containerPadding)}header nav a{color:var(--white);text-decoration:none}header nav a+a{margin-left:10px}footer{color:var(--footerTextColor);background-color:var(--footerBackground);padding:calc(var(--headerHeight) * .75) var(--containerPadding);text-align:center;bottom:0;width:100%}footer a{color:var(--footerTextColor)}footer nav a+a{margin-left:10px}footer p{margin-bottom:0;max-width:none}p{margin-bottom:1rem}p a,blockquote a{color:var(--textColor);text-decoration:none;border-bottom:var(--borderBottom)}h1,h2,h3,h4,h5{margin:3rem 0 1.38rem;font-family:var(--headingFont);font-weight:400;line-height:1.15}h1{margin-top:0;font-size:var(--h1)}h2{font-size:var(--h2)}h3{font-size:var(--h3)}h4{font-size:var(--h4)}h5{font-size:var(--h5)}small,.text_small{font-size:var(--smallText)}blockquote{margin:10px;padding:2em;background:var(--cardBg);box-shadow:var(--shadow-lg)}label{display:block;font-size:var(--smallText)}input,textarea{padding:2px 5px;border:var(--line);border-radius:4px}textarea{width:100%;height:5rem}::placeholder{color:var(--grey)}::selection,.highlight{background:#ffb7b7;background:var(--red);color:var(--white)}select{border:var(--line)}hr{border-top:var(--line)}button{-webkit-appearance:none;-moz-appearance:none;appearance:none;color:var(--buttonTextColor);background-color:var(--white);border:var(--line);border-radius:var(--borderRadius);padding:10px 25px;box-shadow:var(--shadow-s);transition:.3s ease-in-out box-shadow}button:hover{cursor:pointer;box-shadow:var(--shadow-md)}button[disabled]{opacity:.4}button.cancel{--buttonColor: var(--danger);--buttonTextColor: var(--white)}button.small{font-size:var(--smallText)}.layout{padding-top:calc(0rem + var(--headerHeight))}.grid{--gridCols: 2;display:block;grid-template-columns:repeat(var(--gridCols),1fr)}.cols-3{--gridCols: 3}.cols-4{--gridCols: 4}.flex{--justifyContent: space-between;display:block;justify-content:var(--justifyContent)}.flex-around{--justifyContent: space-around}.card{padding:2em;background:var(--cardBg);box-shadow:var(--shadow-lg);border-radius:var(--borderRadius)}.grid-split{display:grid;grid-template-columns:33% 67%;gap:20px}@media only screen and (min-width: 600px){:root{--baseFontSize: 100%}.grid{display:grid}.flex{display:flex}}.logo{font-size:var(--baseFontSize);margin:0 0 0 8px}.dark{--background: var(--black);--textColor: var(--lightGrey);--headerBackground: var(--darkGrey);--footerBackground: var(--yellow);--cardBg: var(--darkGrey);--buttonTextColor: var(--black)}.oled{--black: #000;--cardBg: var(--darkGrey);--headerBackground: var(--darkGrey);--footerBackground: var(--darkGrey)}.theme{--green: #00ebc7;--red: #FF5470;--yellow: #fde24f;--black: #1b2d45;--darkBlue: #00214d;--darkGrey: #222;--grey: #bfbfbf;--lightGrey: #f2f4f6;--white: white;--primary: var(--green);--danger: var(--red);--background: var(--lightGrey);--textColor: var(--black);--lineColor: var(--grey);--cardBg: var(--white);--headerBackground: var(--darkBlue);--footerBackground: var(--darkBlue);--footerTextColor: var(--black);--buttonColor: var(--primary);--buttonTextColor: var(--textColor);--line: solid 1px var(--lineColor);--headingFont: "Lato", monospace;--bodyFont: "Work Sans", sans-serif;--baseFontSize: 100%;--h1: 3.052em;--h2: 2.441em;--h3: 1.953em;--h4: 1.563em;--h5: 1.25em;--smallText: .8em;--shadow-s: 0 1px 3px 0 rgb(0 0 0 / .1), 0 1px 2px -1px rgb(0 0 0 / .1);--shadow-md: 0 4px 6px -1px rgb(0 0 0 / .1), 0 2px 4px -2px rgb(0 0 0 / .1);--shadow-lg: 0 10px 15px -3px rgb(0 0 0 / .1), 0 4px 6px -4px rgb(0 0 0 / .1);--shadow-xl: 0 20px 25px -5px rgb(0 0 0 / .1), 0 8px 10px -6px rgb(0 0 0 / .1);--containerPadding: 2.5%;--headerHeight: 3rem;--borderRadius: 10px}:root{--left: 25px}.grid-sidemenu{--gridCols: 2;display:grid;grid-template-columns:var(--left) 1fr}header{padding:0 15px 0 0}header nav a+a{margin-left:15px}.corner{margin-left:var(--left)}header nav a{color:var(--black);text-decoration:none}.page{padding:3em}.page-title{text-decoration:none;border-bottom:var(--borderBottom)}.card{padding:2em;background:var(--cardBg);box-shadow:var(--shadow-lg);border-radius:var(--borderRadius);font-size:var(--smallText)}.card:hover{box-shadow:var(--shadow-xl)}.card>*:first-child{margin-top:0}.card>*:last-child{margin-bottom:0}table{margin:auto}button{margin:5px}.small-button.svelte-9ap43o.svelte-9ap43o{margin-left:10px;background:none;border:3px solid transparent;color:inherit;padding:6px 10px;cursor:pointer;box-shadow:none;font-size:var(--smallText)}.feedback-buttons.svelte-9ap43o.svelte-9ap43o{text-align:center;margin:auto;width:20%}.small-button.svelte-9ap43o.svelte-9ap43o:hover{box-shadow:var(--shadow-md)}.thumbs-up.svelte-9ap43o.svelte-9ap43o,.thumbs-up.svelte-9ap43o.svelte-9ap43o:hover,.thumbs-up.svelte-9ap43o.svelte-9ap43o::selection{background:var(--green)}.thumbs-down.svelte-9ap43o.svelte-9ap43o,.thumbs-down.svelte-9ap43o.svelte-9ap43o:hover,.thumbs-down.svelte-9ap43o.svelte-9ap43o::selection{background:var(--red)}.ranked-chat.svelte-9ap43o.svelte-9ap43o{height:100vh;display:grid;grid-template-columns:100%;grid-template-rows:80% 20%}.message.svelte-9ap43o.svelte-9ap43o{font-size:var(--smallText);padding-left:40px;padding-right:40px;margin:0 auto}.chat-input-holder.svelte-9ap43o.svelte-9ap43o{display:flex;flex-direction:column;align-items:center;padding:24px;width:100%;max-width:640px;margin:auto}.chat-input-textarea.svelte-9ap43o.svelte-9ap43o{background-color:var(--lightgrey);cursor:pointer;width:100%;border:var(--line);border-color:none;margin:12px;outline:none;padding:12px;color:var(--black);font-size:var(--baseFontSize);box-shadow:var(--shadow-md);flex:3;border-radius:0;border-right:0px}.chat-input-form.svelte-9ap43o.svelte-9ap43o{display:flex;width:100%}.btnyousend.svelte-9ap43o.svelte-9ap43o{border-radius:0;margin-top:12px;margin-bottom:12px;margin-left:-15px;background:var(--primary);color:var(--black);opacity:.5;transition:all .3s}.active.svelte-9ap43o.svelte-9ap43o{opacity:1}.green.svelte-9ap43o.svelte-9ap43o{border-bottom:2px solid var(--green)}.red.svelte-9ap43o.svelte-9ap43o{border-bottom:2px solid var(--red)}.instructions.svelte-9ap43o.svelte-9ap43o{text-align:center;padding:5%}.instructions.svelte-9ap43o h5.svelte-9ap43o{text-align:left}.instructions.svelte-9ap43o p.svelte-9ap43o{font-size:var(--smallText);text-align:left}.instructions.svelte-9ap43o button.svelte-9ap43o{font-size:var(--smallText)}.ranked-feedback-container.svelte-9ap43o.svelte-9ap43o{display:grid;grid-template-columns:20% 80%}.underline.svelte-9ap43o.svelte-9ap43o{border-bottom:var(--line)}.bold.svelte-9ap43o.svelte-9ap43o{font-weight:700;font-size:var(--smallText);margin:0;padding:0}.chatbox.svelte-9ap43o.svelte-9ap43o{display:flex;flex-direction:column;justify-content:space-between;height:calc(100vh - var(--headerHeight));background-color:var(--white);box-sizing:border-box;width:95%;margin:auto;height:100%}.chat-log.svelte-9ap43o.svelte-9ap43o{flex:1;overflow-y:auto;padding:0 10px;box-sizing:border-box}.chat-message.svelte-9ap43o.svelte-9ap43o{background-color:var(--white);border-bottom:var(--line);box-sizing:border-box}.chat-message-center.svelte-9ap43o.svelte-9ap43o{display:flex;flex-direction:column;margin-left:auto;margin-right:auto;padding:12px;box-sizing:border-box}.message-content.svelte-9ap43o.svelte-9ap43o{display:flex;flex-direction:column;box-sizing:border-box}.message-content.svelte-9ap43o .question.svelte-9ap43o{text-align:left;border:1px solid var(--grey);padding:5px;background-color:var(--lightGrey)}.message-content.svelte-9ap43o .answer.svelte-9ap43o{display:inline-block;text-align:left;padding:10px;border:1px solid var(--black)}.message-content.svelte-9ap43o .answers.svelte-9ap43o{display:grid;grid-template-columns:100%;gap:0%;width:100%;margin:auto}.ranked-chat.svelte-au920n.svelte-au920n{height:100vh;display:grid;grid-template-columns:100%;grid-template-rows:80% 20%}.message.svelte-au920n.svelte-au920n{font-size:var(--smallText);padding-left:40px;padding-right:40px;margin:0 auto}.chat-input-holder.svelte-au920n.svelte-au920n{display:flex;flex-direction:column;align-items:center;padding:24px;width:100%;max-width:640px;margin:auto}.chat-input-textarea.svelte-au920n.svelte-au920n{background-color:var(--lightgrey);cursor:pointer;width:100%;border:var(--line);border-color:none;margin:12px;outline:none;padding:12px;color:var(--black);font-size:var(--baseFontSize);box-shadow:var(--shadow-md);flex:3;border-radius:0;border-right:0px}.chat-input-form.svelte-au920n.svelte-au920n{display:flex;width:100%}.btnyousend.svelte-au920n.svelte-au920n{border-radius:0;margin-top:12px;margin-bottom:12px;margin-left:-15px;background:var(--primary);color:var(--black);opacity:.5;transition:all .3s}.active.svelte-au920n.svelte-au920n{opacity:1}.green.svelte-au920n.svelte-au920n{border-bottom:2px solid var(--green)}.red.svelte-au920n.svelte-au920n{border-bottom:2px solid var(--red)}.instructions.svelte-au920n.svelte-au920n{text-align:center;padding:5%}.instructions.svelte-au920n h5.svelte-au920n{text-align:left}.instructions.svelte-au920n p.svelte-au920n{font-size:var(--smallText);text-align:left}.instructions.svelte-au920n button.svelte-au920n{font-size:var(--smallText)}.ranked-feedback-container.svelte-au920n.svelte-au920n{display:grid;grid-template-columns:20% 80%}.underline.svelte-au920n.svelte-au920n{border-bottom:var(--line)}.bold.svelte-au920n.svelte-au920n{font-weight:700;font-size:var(--smallText);margin:0;padding:0}.chatbox.svelte-au920n.svelte-au920n{display:flex;flex-direction:column;justify-content:space-between;height:calc(100vh - var(--headerHeight));background-color:var(--white);box-sizing:border-box;width:95%;margin:auto;height:100%}.chat-log.svelte-au920n.svelte-au920n{flex:1;overflow-y:auto;padding:0 10px;box-sizing:border-box}.chat-message.svelte-au920n.svelte-au920n{background-color:var(--white);border-bottom:var(--line);box-sizing:border-box}.chat-message-center.svelte-au920n.svelte-au920n{display:flex;flex-direction:column;margin-left:auto;margin-right:auto;padding:12px;box-sizing:border-box}.message-content.svelte-au920n.svelte-au920n{display:flex;flex-direction:column;box-sizing:border-box}.message-content.svelte-au920n .question.svelte-au920n{text-align:left;border:1px solid var(--grey);padding:5px;margin-bottom:10px;background-color:var(--lightGrey)}.message-content.svelte-au920n .answer.svelte-au920n{display:inline-block;text-align:left;padding:10px;border:1px solid var(--black)}.message-content.svelte-au920n .answers.svelte-au920n{display:grid;grid-template-columns:49% 49%;gap:2%;width:100%;margin:auto}.series.svelte-tg5p7i:focus{outline:none}.horizontal-bar-rect.selected.svelte-tg5p7i{stroke:var(--black);stroke-width:3}#stackedrect-holder.svelte-tg5p7i{height:100%;width:100%}.line.svelte-tg5p7i{stroke-width:3;stroke:var(--black);fill:none}.horizontal-bar-rect.svelte-tg5p7i{transition:opacity .3s}.horizontal-bar-rect.svelte-tg5p7i:hover{stroke:var(--black);stroke-width:3}.horizontal-bar-text.svelte-tg5p7i{transition:opacity .3s;stroke:var(--white);stroke-width:4px;fill:var(--black);stroke-linejoin:round;paint-order:stroke fill;pointer-events:none;font-size:var(--smallText)}.qa-card.svelte-szi0e{border:2px solid var(--black);display:flex;flex-direction:column;font-size:var(--smallText);padding:4px;margin:6px}.qa-card.svelte-szi0e:hover{border:3px solid var(--black)}.question.svelte-szi0e{background-color:var(--white);margin:0;padding:8px;border-bottom:1px solid var(--black)}.answer.svelte-szi0e{background-color:var(--lightGrey);margin:0;padding:8px}.feedback.svelte-szi0e{margin:0;padding:8px}.up.svelte-szi0e{background-color:var(--green)}.down.svelte-szi0e{background-color:var(--red)}.na.svelte-szi0e{background-color:var(--yellow)}.qa-container.svelte-1xv9cfi{border:2px solid var(--background);max-height:100%;overflow-y:auto}.chart-title.svelte-1oikip4{font-size:var(--smallText)}rect.svelte-1oikip4:hover{stroke:var(--black)}#stackedrect-holder.svelte-1oikip4{height:100%;width:100%}.axis-line.svelte-1oikip4{stroke-width:3;stroke:var(--black);fill:none}.axis-tick.svelte-1oikip4{stroke-width:1;fill:none;opacity:0;font-size:9px}.axis-text.svelte-1oikip4{font-size:calc(var(--smallText) * .9)}.svelte-kz2qh6{transition:all .3s}.chart-title.svelte-kz2qh6{font-size:var(--smallText)}rect.svelte-kz2qh6:hover{stroke:var(--black)}.histogram-container.svelte-kz2qh6{height:100%;width:100%}.axis-line.svelte-kz2qh6{stroke-width:3;stroke:var(--black);fill:none}.axis-tick.svelte-kz2qh6{stroke-width:1;fill:none;opacity:0;font-size:9px}.axis-text.svelte-kz2qh6{font-size:calc(var(--smallText) * .9)}.svelte-1pknxov{font-family:Lato}.card-container.svelte-1pknxov{border:2px solid var(--black);width:100%;height:100%;display:grid;grid-template-columns:100%;grid-template-rows:35% 50% 10%;padding:5px;box-sizing:border-box}.card-text.svelte-1pknxov{text-align:left;margin:0;padding:0 0 0 2px;font-weight:700;font-size:.8em}#feedback-dropdown.svelte-1pknxov{width:98%;border:none;border-bottom:1px solid var(--black);border-top:1px solid var(--black);font-size:var(--smallText);margin-bottom:1px}svg.svelte-1pknxov{width:100%;height:100%;border-bottom:1px solid var(--black)}.small.svelte-1pknxov{font-size:.6em}text.svelte-1pknxov{font-size:3rem;transition:opacity .3s;stroke:#fff;stroke-width:6px;fill:var(--black);stroke-linejoin:round;paint-order:stroke fill;pointer-events:none}.card-container.svelte-mchgj2{border:2px solid var(--black);width:100%;height:100%;display:grid;grid-template-columns:100%;grid-template-rows:35% 50% 10%;padding:5px;box-sizing:border-box}.card-text.svelte-mchgj2{text-align:left;margin:0;padding:0 0 0 2px;font-weight:700;font-size:.8em}#feedback-dropdown.svelte-mchgj2{width:98%;border:none;border-bottom:1px solid var(--black);border-top:1px solid var(--black);font-size:var(--smallText);margin-bottom:1px}svg.svelte-mchgj2{width:100%;height:100%;border-bottom:1px solid var(--black)}.small.svelte-mchgj2{font-size:.6em}text.svelte-mchgj2{font-size:3rem;transition:opacity .3s;stroke:#fff;stroke-width:6px;fill:var(--black);stroke-linejoin:round;paint-order:stroke fill;pointer-events:none}.feedback-container.svelte-14znspc{border-bottom:var(--line);border-right:var(--line);display:grid;grid-template-columns:30% 70%;grid-template-rows:100%;width:90%;height:calc(100vh - var(--headerHeight))}.feedback-left.svelte-14znspc{border-bottom:var(--line);display:grid;grid-template-columns:100%;grid-template-rows:25% 25% 25% 12.5% 12.5%}.left-text.svelte-14znspc{text-align:center;border-bottom:var(--line);border-right:var(--line);display:grid;grid-template-rows:100%;grid-template-columns:50% 50%}.left-confidence.svelte-14znspc{text-align:center;border-bottom:var(--line);border-right:var(--line);display:grid;grid-template-rows:40% 55%}.left-question.svelte-14znspc,.left-filter.svelte-14znspc{border-bottom:var(--line);border-right:var(--line)}.feedback-right.svelte-14znspc{border-bottom:var(--line);border-right:var(--line);display:grid;grid-template-columns:100%;grid-template-rows:30% 70%;grid-template-rows:0% 100%}.right-chart.svelte-14znspc{border-bottom:var(--line);border-right:var(--line);display:grid;grid-template-columns:50% 50%;grid-template-rows:100%}.right-chart-1.svelte-14znspc,.right-chart-2.svelte-14znspc{border-right:var(--line)}.right-table.svelte-14znspc{border-bottom:var(--line);border-right:var(--line)}.card-1.svelte-14znspc{border-right:var(--line)}.ranked-chat.svelte-1nj8mt0.svelte-1nj8mt0{height:100vh;display:grid;grid-template-columns:100%;grid-template-rows:80% 20%}.chat-input-holder.svelte-1nj8mt0.svelte-1nj8mt0{display:flex;flex-direction:column;align-items:center;padding:24px;width:100%;max-width:640px;margin:auto}.chat-input-textarea.svelte-1nj8mt0.svelte-1nj8mt0{background-color:var(--lightgrey);cursor:pointer;width:100%;border:var(--line);border-color:none;margin:12px;outline:none;padding:12px;color:var(--black);font-size:var(--baseFontSize);box-shadow:var(--shadow-md);flex:3;border-radius:0;border-right:0px}.chat-input-form.svelte-1nj8mt0.svelte-1nj8mt0{display:flex;width:100%}.btnyousend.svelte-1nj8mt0.svelte-1nj8mt0{border-radius:0;margin-top:12px;margin-bottom:12px;margin-left:-15px;background:var(--primary);color:var(--black);opacity:.5;transition:all .3s}.active.svelte-1nj8mt0.svelte-1nj8mt0{opacity:1}.instructions.svelte-1nj8mt0.svelte-1nj8mt0{text-align:center;padding:5%;border-right:var(--line)}.instructions.svelte-1nj8mt0 h5.svelte-1nj8mt0{text-align:left}.instructions.svelte-1nj8mt0 p.svelte-1nj8mt0{font-size:var(--smallText);text-align:left;margin:0}.instructions.svelte-1nj8mt0 button.svelte-1nj8mt0{font-size:var(--smallText)}.ranked-feedback-container.svelte-1nj8mt0.svelte-1nj8mt0{display:grid;grid-template-columns:20% 80%}.underline.svelte-1nj8mt0.svelte-1nj8mt0{border-bottom:var(--line)}.bold.svelte-1nj8mt0.svelte-1nj8mt0{font-weight:700;font-size:var(--smallText);margin:0;padding:0}.chatbox.svelte-1nj8mt0.svelte-1nj8mt0{display:flex;flex-direction:column;justify-content:space-between;height:calc(100vh - var(--headerHeight));background-color:var(--white);box-sizing:border-box;width:95%;margin:auto;height:100%}.chat-log.svelte-1nj8mt0.svelte-1nj8mt0{flex:1;overflow-y:auto;padding:0 10px;box-sizing:border-box}.chat-message.svelte-1nj8mt0.svelte-1nj8mt0{background-color:var(--white);border-bottom:var(--line);box-sizing:border-box}.chat-message-center.svelte-1nj8mt0.svelte-1nj8mt0{display:flex;flex-direction:column;margin-left:auto;margin-right:auto;padding:12px;box-sizing:border-box}.message-content.svelte-1nj8mt0.svelte-1nj8mt0{display:flex;flex-direction:column;box-sizing:border-box}.message-content.svelte-1nj8mt0 .question.svelte-1nj8mt0{text-align:left;border:1px solid var(--grey);padding:5px;margin-bottom:10px;background-color:var(--lightGrey)}.message-content.svelte-1nj8mt0 .answer.svelte-1nj8mt0{display:inline-block;text-align:left;padding:10px;border:1px solid var(--black)}option.svelte-1nj8mt0.svelte-1nj8mt0{font-weight:700;font-size:120%}p.svelte-1nj8mt0.svelte-1nj8mt0{margin:0}.svelte-1nna9rx{font-family:Lato}#chart-holder.svelte-1nna9rx{height:100%;width:100%}.axis-line.svelte-1nna9rx{stroke-width:3;stroke:#000;fill:none}.axis-tick.svelte-1nna9rx{stroke-width:2;stroke:#000;fill:none;opacity:.13}.axis-text.svelte-1nna9rx{font-family:Arial;font-size:12px}.bump-text.svelte-1nna9rx{font-size:12px;pointer-events:none}.model-path.svelte-1nna9rx{fill:none;stroke-width:5;stroke-linecap:round;stroke-linejoin:round}.model-path-outer.svelte-1nna9rx{fill:none;stroke-width:8;stroke-linecap:round;stroke-linejoin:round}.chart-subtitle.svelte-1nna9rx{font-size:12px}#bar-chart-holder.svelte-1y9gffu{height:100%;width:100%}.axis-text.svelte-1y9gffu{font-size:9px}.axis-line.svelte-1y9gffu{stroke-width:3;stroke:#000;fill:none}.label-text.svelte-1y9gffu{font-size:9px}.cell.svelte-hnulv9{max-height:40px;overflow:hidden;white-space:nowrap;text-overflow:ellipsis}.cell.active.svelte-hnulv9{max-height:100%;overflow:visible;white-space:normal}.svelte-owgjbp.svelte-owgjbp{font-family:Lato,monospace}.table.svelte-owgjbp.svelte-owgjbp{margin:auto;width:90%}.pretty-pager.svelte-owgjbp.svelte-owgjbp{padding-top:1rem}.pretty-table.normal.svelte-owgjbp.svelte-owgjbp{font-size:15px}.pretty-table.normal.svelte-owgjbp th.svelte-owgjbp,.pretty-table.normal.svelte-owgjbp td.svelte-owgjbp{padding:3px 2px}.pretty-table.svelte-owgjbp th.svelte-owgjbp,.pretty-table.svelte-owgjbp td.svelte-owgjbp{vertical-align:top}.pretty-table.svelte-owgjbp thead th.svelte-owgjbp{text-transform:uppercase;font-weight:700;font-family:Work Sans,sans-serif;border-bottom:2px solid black}.pretty-table.svelte-owgjbp th.svelte-owgjbp{cursor:pointer}.pretty-table.svelte-owgjbp tbody td.cell-type-number.svelte-owgjbp,.pretty-table.svelte-owgjbp tbody td.cell-rank.svelte-owgjbp{text-align:right}.pretty-table.svelte-owgjbp tbody td.cell-type-number.svelte-owgjbp,.pretty-table.svelte-owgjbp tbody td.cell-rank.svelte-owgjbp{font-family:menlo,consolas,monaco,monospace;font-size:90%}.pretty-table.svelte-owgjbp tbody td.cell-rank.svelte-owgjbp{padding-right:1em;color:#666}table.pretty-table.svelte-owgjbp.svelte-owgjbp{border-collapse:collapse}table.pretty-table.svelte-owgjbp.svelte-owgjbp{border-collapse:collapse;table-layout:fixed}.pretty-table.svelte-owgjbp tr.svelte-owgjbp{border-bottom:1px solid #eee}td.active.svelte-owgjbp.svelte-owgjbp{max-height:100%;overflow:auto;color:red}td.svelte-owgjbp.svelte-owgjbp:not(.active){overflow:hidden;white-space:normal}tr.svelte-owgjbp.svelte-owgjbp:hover{background:#eee}.pretty-table.svelte-owgjbp.svelte-owgjbp{width:100%}#heatmap-holder.svelte-t6wv8i{height:100%;width:100%}.axis-text.svelte-t6wv8i,.chart-subtitle.svelte-t6wv8i{font-size:12px}.holder.svelte-1gze3r0.svelte-1gze3r0{height:100vh;width:100%;display:flex;justify-content:center;align-items:center}button.svelte-1gze3r0.svelte-1gze3r0{margin:0}.chart-captions.svelte-1gze3r0.svelte-1gze3r0{margin:auto;width:100%;text-align:left;height:100%}.chart-captions.svelte-1gze3r0 h4.svelte-1gze3r0{padding:0;margin:0}.instructions.svelte-1gze3r0.svelte-1gze3r0{text-align:left;padding-left:0}.instructions.svelte-1gze3r0 p.svelte-1gze3r0{font-size:var(--smallText);text-align:left}.instructions.svelte-1gze3r0 button.svelte-1gze3r0{font-size:var(--smallText)}.underline.svelte-1gze3r0.svelte-1gze3r0{border-bottom:var(--line)}.bold.svelte-1gze3r0.svelte-1gze3r0{font-weight:700;font-size:var(--smallText);margin:0;padding:0}.instructions.svelte-1gze3r0.svelte-1gze3r0{border-right:1px solid #eee}.main-container.svelte-1gze3r0.svelte-1gze3r0{display:grid;grid-template-columns:20% 80%}.eval-container.svelte-1gze3r0.svelte-1gze3r0{display:grid;height:100vh;grid-template-rows:100%;grid-template-columns:65% 35%;padding:1rem}.left-charts.svelte-1gze3r0.svelte-1gze3r0{display:grid;grid-template-columns:100%;grid-template-rows:15% 60% 25%}.eval-table.svelte-1gze3r0.svelte-1gze3r0{margin:auto;width:100%}.right-charts.svelte-1gze3r0.svelte-1gze3r0{display:grid;grid-template-columns:100%;grid-template-rows:10% 33% 33%;gap:1%}.main-annotation-container.svelte-3wjb3y.svelte-3wjb3y{display:grid;grid-template-columns:100%;grid-template-rows:90% 10%;height:100vh;width:100%;margin:auto}.buttons.svelte-3wjb3y.svelte-3wjb3y{display:flex;background:var(--grey)}.rating-button.svelte-3wjb3y.svelte-3wjb3y{padding:10px;border:none}.rating-button.svelte-3wjb3y+.rating-button.svelte-3wjb3y{margin-left:-1px}.ranked-chat.svelte-3wjb3y.svelte-3wjb3y{display:grid;grid-template-columns:100%;grid-template-rows:100%;border:var(--line);margin:12px}.chat-input-holder.svelte-3wjb3y.svelte-3wjb3y{align-items:center;width:100%;margin:auto;border-top:var(--line)}.instructions.svelte-3wjb3y.svelte-3wjb3y{text-align:center;padding:5%}.instructions.svelte-3wjb3y h5.svelte-3wjb3y{text-align:left}.instructions.svelte-3wjb3y p.svelte-3wjb3y{font-size:var(--smallText);text-align:left}.instructions.svelte-3wjb3y button.svelte-3wjb3y{font-size:var(--smallText)}.annotation-container.svelte-3wjb3y.svelte-3wjb3y{display:grid;grid-template-columns:40% 60%}.underline.svelte-3wjb3y.svelte-3wjb3y{border-bottom:var(--line)}.bold.svelte-3wjb3y.svelte-3wjb3y{font-weight:700;font-size:var(--smallText);margin:0;padding:0}.chatbox.svelte-3wjb3y.svelte-3wjb3y{display:flex;flex-direction:column;justify-content:space-between;height:calc(100vh - var(--headerHeight));background-color:var(--white);box-sizing:border-box;width:95%;margin:auto;height:100%}.chat-message-center.svelte-3wjb3y.svelte-3wjb3y{display:flex;flex-direction:column;padding:12px;box-sizing:border-box}.message-content.svelte-3wjb3y.svelte-3wjb3y{display:flex;flex-direction:column;box-sizing:border-box;display:block}.message-content.svelte-3wjb3y .question.svelte-3wjb3y{text-align:left;border:1px solid var(--grey);padding:5px;margin-bottom:10px;background-color:var(--lightGrey)}.message-content.svelte-3wjb3y .answer.svelte-3wjb3y{display:block;text-align:left;padding:10px;border:1px solid var(--black)}.message-content.svelte-3wjb3y .answers.svelte-3wjb3y{display:grid;grid-template-columns:100%;gap:2%;width:100%;margin:auto}
```

### Comparing `pykoi-0.0.1/pykoi/frontend/dist/vite.svg` & `pykoi-0.0.2/pykoi/frontend/dist/vite.svg`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.1/pykoi/frontend/jsconfig.json` & `pykoi-0.0.2/pykoi/frontend/jsconfig.json`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.1/pykoi/frontend/public/vite.svg` & `pykoi-0.0.2/pykoi/frontend/public/vite.svg`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.1/pykoi/frontend/src/App.svelte` & `pykoi-0.0.2/pykoi/frontend/src/App.svelte`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 <script>
   import { writable } from "svelte/store";
   import Chat from "./lib/Chatbots/Chat.svelte";
   import Dropdown from "./lib/UIComponents/Dropdown.svelte";
   import Feedback from "./lib/Dashboards/Feedback.svelte";
-  import RlhfEvaluation from "./lib/Evaluation/RLHFEvaluation.svelte";
+  import ComparisonChat from "./lib/Chatbots/ComparisonChat.svelte";
+  import ComparisonChart from "./lib/Comparison/ComparisonChart.svelte";
+  import QuestionRating from "./lib/Annotations/QuestionRating.svelte";
+  import RankedChatbot from "./lib/Chatbots/RankedChatbot.svelte";
 
   const components = writable([]);
   const selectedPage = writable(null);
 
   const componentMap = {
     Chatbot: Chat,
     Dropdown: Dropdown,
     Feedback: Feedback,
+    Compare: ComparisonChat,
   };
 
   const setSelectedPage = (component) => {
     selectedPage.set(component);
   };
 
   // Attempt to fetch components to load from server
@@ -44,14 +48,13 @@
       on:click={() => setSelectedPage(component)}
       >{component.svelte_component}</button
     >
   {/each}
 {/if}
 
 <!-- Loaded selected component (tab) -->
-<!-- {#if $selectedPage}
+{#if $selectedPage}
   <svelte:component
     this={componentMap[$selectedPage.svelte_component]}
     {...$selectedPage.props}
   />
-{/if} -->
-<RlhfEvaluation />
+{/if}
```

#### html2text {}

```diff
@@ -1,3 +1,4 @@
    {#if $components.length > 1} {#each $components as component}
 {component.svelte_component} component`} on:click={() => setSelectedPage
-(component)} >{component.svelte_component} {/each} {/if}
+(component)} >{component.svelte_component} {/each} {/if}  {#if $selectedPage}
+...$selectedPage.props} /> {/if}
```

### Comparing `pykoi-0.0.1/pykoi/frontend/src/app.css` & `pykoi-0.0.2/pykoi/frontend/src/app.css`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.1/pykoi/frontend/src/assets/svelte.svg` & `pykoi-0.0.2/pykoi/frontend/src/assets/svelte.svg`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.1/pykoi/frontend/src/lib/Annotations/QuestionRating.svelte` & `pykoi-0.0.2/pykoi/frontend/src/lib/Annotations/QuestionRating.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.1/pykoi/frontend/src/lib/Chatbots/Chatbot.svelte` & `pykoi-0.0.2/pykoi/frontend/src/lib/Chatbots/Chatbot.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.1/pykoi/frontend/src/lib/Chatbots/RankedChatbot.svelte` & `pykoi-0.0.2/pykoi/frontend/src/lib/Chatbots/RankChatbotOld.svelte`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     let currentEntry = {
       question: mymessage,
       up_ranking_answer: "Loading...",
       low_ranking_answer: "Loading...",
     };
     $rankChatLog = [...$rankChatLog, currentEntry];
 
-    const response = await fetch(`/chat/ranking_table/${mymessage}`, {
+    const response = await fetch(`/chat/multi_responses/${mymessage}`, {
       method: "POST",
       headers: {
         "Content-Type": "application/json",
       },
       body: JSON.stringify({
         prompt: mymessage,
       }),
@@ -82,14 +82,15 @@
       headers: {
         "Content-Type": "application/json",
       },
       body: JSON.stringify(rankingUpdate),
     });
 
     if (response.ok) {
+      console.log("response", response);
     } else {
       const err = await response.text();
       alert(err);
     }
   }
 
   function handleClick(event, msg, questionIndex, answerIndex) {
```

### Comparing `pykoi-0.0.1/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/ColumnChart.svelte` & `pykoi-0.0.2/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/ColumnChart.svelte`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 <script>
-  import { max, min } from "d3-array";
+  import { max } from "d3-array";
   import { format } from "d3-format";
   import { scaleLinear, scaleBand } from "d3-scale";
   import { questionDistribution, feedbackSelection } from "../../../store.js";
-  import { interpolate } from "d3-interpolate";
 
   const emojiObj = {
     up: "Good 👍",
     down: "Bad 👎",
     "n/a": "No Rating",
     all: "All",
   };
@@ -30,30 +29,24 @@
   };
 
   const formatter = format(".1f");
 
   $: width = outerWidth - margin.left - margin.right;
   $: height = outerHeight - margin.top - margin.bottom;
 
-  // const color = scaleOrdinal().range(["#2074d5", "#fde24f"]);
-
   $: xScale = scaleBand()
     .rangeRound([margin.left, width - margin.right])
     .padding(0.05)
     .domain($questionDistribution.map((d) => d.question));
 
   $: yScale = scaleLinear()
     .rangeRound([height - margin.bottom, margin.top])
     .domain([0, max($questionDistribution, (d) => d.count)]);
 
-  $: maxValue = max($questionDistribution, (d) => d.count);
-  $: color = scaleLinear()
-    .domain([0, maxValue])
-    .range(["white", colorObj[$feedbackSelection]])
-    .interpolate(interpolate);
+  $: console.log($questionDistribution);
 </script>
 
 <div
   id="stackedrect-holder"
   bind:offsetWidth={outerWidth}
   bind:offsetHeight={outerHeight}
 >
@@ -94,15 +87,15 @@
     <!-- stacked rects -->
     {#each $questionDistribution as d}
       <g class="series">
         <rect
           x={xScale(d.question)}
           y={yScale(d.count)}
           height={height - yScale(d.count) - margin.bottom}
-          fill={color(d.count)}
+          fill={colorObj[$feedbackSelection]}
           fill-opacity="0.95"
           width={xScale.bandwidth()}
         />
         <text
           class="axis-text"
           x={xScale(d.question) + xScale.bandwidth() / 2}
           y={yScale(d.count) - 5}
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
   {#each $questionDistribution.map((d) => d.question) as tick}
  xScale.bandwidth() / 2} ${ height - margin.bottom })`} >
  margin.bottom + margin.top} stroke="var(--squidink)" stroke-dasharray="4" />
 {tick}  {/each}  {#each yScale.ticks() as tick}
 {yScale(tick) + 0})`}>
  margin.right - margin.left} y1="0" y2="0" stroke="black" />  {/each}  {#each
 $questionDistribution as d}
- yScale(d.count) - margin.bottom} fill={color(d.count)} fill-opacity="0.95"
-width={xScale.bandwidth()} />
+ yScale(d.count) - margin.bottom} fill={colorObj[$feedbackSelection]} fill-
+opacity="0.95" width={xScale.bandwidth()} />
  xScale.bandwidth() / 2} y={yScale(d.count) - 5} text-anchor="middle">
 {Math.round(formatter(d.count))}  {/each}
 2 + 1} x={(width + margin.left) / 2} text-anchor="middle">Question Type:
 {emojiObj[$feedbackSelection]}
  margin.right} y1={height - margin.bottom} y2={height - margin.bottom} />
  margin.bottom} opacity="0" />
```

### Comparing `pykoi-0.0.1/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/HistogramAnswer.svelte` & `pykoi-0.0.2/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/HistogramAnswer.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.1/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/HistogramQuestion.svelte` & `pykoi-0.0.2/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/HistogramQuestion.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.1/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/HorizontalStackedBar.svelte` & `pykoi-0.0.2/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/HorizontalStackedBar.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.1/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/MetricCardAbsolute.svelte` & `pykoi-0.0.2/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/MetricCardAbsolute.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.1/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/MetricCardPercentage.svelte` & `pykoi-0.0.2/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/MetricCardPercentage.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.1/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/QACard.svelte` & `pykoi-0.0.2/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/QACard.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.1/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/QATable.svelte` & `pykoi-0.0.2/pykoi/frontend/src/lib/Dashboards/DashboardFeedback/QATable.svelte`

 * *Files 10% similar despite different names*

```diff
@@ -3,23 +3,21 @@
   import { cubicOut } from "svelte/easing";
   import QACard from "./QACard.svelte";
   import {
     chatLog,
     feedbackSelection,
     questionDistribution,
   } from "../../../store";
-  import { tallyQuestions, getQAWordFrequency } from "../../../utils";
+  import { tallyQuestions } from "../../../utils";
 
   $: qadata =
     $feedbackSelection === "all"
       ? $chatLog
       : $chatLog.filter((d) => d.vote_status === $feedbackSelection);
 
-  $: console.log("qadata", qadata);
-
   const customSlide = (
     node,
     { delay = 0, duration = 1000, easing = cubicOut }
   ) => {
     return slide(node, { delay, duration, easing });
   };
```

### Comparing `pykoi-0.0.1/pykoi/frontend/src/lib/Dashboards/Feedback.svelte` & `pykoi-0.0.2/pykoi/frontend/src/lib/Dashboards/Feedback.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.1/pykoi/frontend/src/lib/Evaluation/Bar.svelte` & `pykoi-0.0.2/pykoi/frontend/src/lib/Evaluation/Bar.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.1/pykoi/frontend/src/lib/Evaluation/EvalLineChart.svelte` & `pykoi-0.0.2/pykoi/frontend/src/lib/Evaluation/LineChart.svelte`

 * *Files 3% similar despite different names*

```diff
@@ -42,21 +42,21 @@
 <div
   class="chart-holder"
   bind:offsetWidth={outerWidth}
   bind:offsetHeight={outerHeight}
 >
   <svg width={outerWidth} height={outerHeight}>
     <defs>
-      <linearGradient id="area-gradient" x1="0" y1="0" x2="0" y2="1">
-        <stop offset="0%" style="stop-color: #FF5470; stop-opacity: 1" />
+      <linearGradient id="area-gradien2t" x1="0" y1="0" x2="0" y2="1">
+        <stop offset="0%" style="stop-color: var(--green); stop-opacity: 1" />
         <stop offset="100%" style="stop-color: white; stop-opacity: .2" />
       </linearGradient>
     </defs>
 
-    <path class="area-path" d={pathArea(data)} fill="url(#area-gradient)" />
+    <path class="area-path" d={pathArea(data)} fill="url(#area-gradien2t)" />
     <path class="outer-path" d={pathLine(data)} />
     <path class="inner-path" d={pathLine(data)} />
 
     <line
       class="axis-line"
       x1={margin.left}
       x2={width - margin.right}
@@ -148,15 +148,15 @@
   }
   .axis-text {
     font-family: Arial;
     font-size: 12px;
   }
 
   .inner-path {
-    stroke: #ff5470;
+    stroke: var(--green);
     stroke-width: 4;
     fill: none;
     stroke-linecap: round;
   }
   .outer-path {
     stroke: white;
     stroke-width: 5;
```

### Comparing `pykoi-0.0.1/pykoi/frontend/src/lib/Evaluation/LineChart.svelte` & `pykoi-0.0.2/pykoi/frontend/src/lib/Evaluation/EvalLineChart.svelte`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,46 @@
 <script>
-  import { extent } from "d3-array";
+  import { bisect, extent } from "d3-array";
   import { scaleLinear } from "d3-scale";
   import { line, curveBasis, area } from "d3-shape";
   import { data } from "./data";
+  import { select } from "d3-selection";
 
   let outerHeight;
   let outerWidth;
 
+  let m = { x: 0, y: 0 };
+
+  function handleMousemove(event) {
+    select("#annotation-tooltip").style("opacity", 1);
+    m.x = event.clientX - event.currentTarget.getBoundingClientRect().left;
+    m.y = event.clientY - event.currentTarget.getBoundingClientRect().top;
+    if (m.x < margin.left) {
+      m.x = margin.left;
+      //   select("#annotation-tooltip").style("opacity", 0);
+    }
+    if (m.x > width - margin.right) {
+      m.x = width - margin.right;
+      //   select("#annotation-tooltip").style("opacity", 0);
+    }
+    // if (m.y > height - margin.right) {
+    //   m.y = width - margin.right;
+    //   select("#annotation-tooltip").style("opacity", 0);
+    // }
+    // if (m.y > height - margin.right) {
+    //   m.y = width - margin.right;
+    //   select("#annotation-tooltip").style("opacity", 0);
+    // }
+  }
+
+  function handleMouseout(event) {
+    console.log("out");
+    select("#annotation-tooltip").style("opacity", 0);
+  }
+
   let margin = {
     top: 10,
     bottom: 15,
     left: 35,
     right: 0,
   };
 
@@ -40,23 +70,30 @@
 </script>
 
 <div
   class="chart-holder"
   bind:offsetWidth={outerWidth}
   bind:offsetHeight={outerHeight}
 >
-  <svg width={outerWidth} height={outerHeight}>
+  <svg
+    width={outerWidth}
+    height={outerHeight}
+    on:touchmove={handleMousemove}
+    on:mousemove={handleMousemove}
+    on:mouseleave={handleMouseout}
+    on:touchend={handleMouseout}
+  >
     <defs>
-      <linearGradient id="area-gradien2t" x1="0" y1="0" x2="0" y2="1">
-        <stop offset="0%" style="stop-color: var(--green); stop-opacity: 1" />
+      <linearGradient id="area-gradient" x1="0" y1="0" x2="0" y2="1">
+        <stop offset="0%" style="stop-color: #FF5470; stop-opacity: 1" />
         <stop offset="100%" style="stop-color: white; stop-opacity: .2" />
       </linearGradient>
     </defs>
 
-    <path class="area-path" d={pathArea(data)} fill="url(#area-gradien2t)" />
+    <path class="area-path" d={pathArea(data)} fill="url(#area-gradient)" />
     <path class="outer-path" d={pathLine(data)} />
     <path class="inner-path" d={pathLine(data)} />
 
     <line
       class="axis-line"
       x1={margin.left}
       x2={width - margin.right}
@@ -123,14 +160,32 @@
     <text
       class="axis-label"
       y={margin.left / 2}
       x={-(height / 2)}
       text-anchor="middle"
       transform="rotate(-90)"
     />
+
+    <!-- tooltip -->
+    <line
+      id="annotation-tooltip"
+      x1={m.x}
+      y1={height - margin.bottom}
+      x2={m.x}
+      y2={margin.top}
+      stroke-width="4"
+      stroke="black"
+    />
+    <circle
+      id="annotation-tooltip-circle"
+      r="10"
+      cx={m.x}
+      cy={m.y}
+      fill="red"
+    />
   </svg>
 </div>
 
 <style>
   .chart-holder {
     height: 100%;
     width: 100%;
@@ -148,15 +203,15 @@
   }
   .axis-text {
     font-family: Arial;
     font-size: 12px;
   }
 
   .inner-path {
-    stroke: var(--green);
+    stroke: #ff5470;
     stroke-width: 4;
     fill: none;
     stroke-linecap: round;
   }
   .outer-path {
     stroke: white;
     stroke-width: 5;
```

#### html2text {}

```diff
@@ -6,8 +6,9 @@
 each}  {#each yScale.ticks() as tick}
 {yScale(tick) + 0})`}>
  margin.right - margin.left} y1="0" y2="0" stroke="black" stroke-dasharray="4"
 /> {tick}  {/each}
 2} x={(width + margin.left) / 2} text-anchor="middle" />
  margin.bottom + 2} x={(width + margin.left) / 2} text-anchor="middle" />
 2} x={-(height / 2)} text-anchor="middle" transform="rotate(-90)" />
+ margin.bottom} x2={m.x} y2={margin.top} stroke-width="4" stroke="black" />
```

### Comparing `pykoi-0.0.1/pykoi/frontend/src/lib/Evaluation/RLHFEvaluation.svelte` & `pykoi-0.0.2/pykoi/frontend/src/lib/Evaluation/RLHFEvaluation.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.1/pykoi/frontend/src/lib/Evaluation/Table.svelte` & `pykoi-0.0.2/pykoi/frontend/src/lib/Evaluation/Table.svelte`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.1/pykoi/frontend/src/lib/Evaluation/store.js` & `pykoi-0.0.2/pykoi/frontend/src/lib/Evaluation/store.js`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.1/pykoi/frontend/src/normalize.css` & `pykoi-0.0.2/pykoi/frontend/src/normalize.css`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.1/pykoi/frontend/src/store.js` & `pykoi-0.0.2/pykoi/frontend/src/store.js`

 * *Files 25% similar despite different names*

#### js-beautify {}

```diff
@@ -4,25 +4,26 @@
 import {
     tweened
 } from "svelte/motion";
 
 export const state = writable({});
 export const chatLog = writable([]);
 export const rankChatLog = writable([]);
+export const compareChatLog = writable([]);
 
 // feedback (rewrite)
 export const feedbackSelection = writable("all"); // up, down, or NA
 
 export const stackedData = writable({
     "n/a": 1,
     up: 1,
     down: 1
 });
 
-const questions = ["Who", "What", "How", "Why", "Where", "Does", "Can", "N/A"];
+const questions = ["who", "what", "how", "why", "where", "does", "can", "n/a"];
 
 export const questionDistribution = tweened(
     questions.map((question) => ({
         question,
         count: 0
     }))
 );
```

### Comparing `pykoi-0.0.1/pykoi/frontend/src/styles.css` & `pykoi-0.0.2/pykoi/frontend/src/styles.css`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.1/pykoi/frontend/src/utils.js` & `pykoi-0.0.2/pykoi/frontend/src/utils.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -13,50 +13,49 @@
 
     return parseFloat((bytes / Math.pow(k, i)).toFixed(dm)) + " " + sizes[i];
 }
 
 export function tallyQuestions(data) {
     // Create an empty object to store the count of each question category
     let questionCounts = {
-        Who: 0,
-        What: 0,
-        How: 0,
-        Why: 0,
-        Where: 0,
-        Does: 0,
-        Can: 0,
-        "N/A": 0,
+        who: 0,
+        what: 0,
+        how: 0,
+        why: 0,
+        where: 0,
+        does: 0,
+        can: 0,
+        "n/a": 0,
     };
 
     // Iterate through each item in the data
     for (let i = 0; i < data.length; i++) {
         // Get the first word of the question (i.e., the question category)
-        let questionCategory = data[i].question.split(" ")[0];
+        let questionCategory = data[i].question.split(" ")[0].toLowerCase();
 
         // If this question category exists in our counts object, increment its count
         if (questionCategory in questionCounts) {
             questionCounts[questionCategory]++;
         }
-        // Otherwise, count it as "N/A"
+        // Otherwise, count it as "n/a"
         else {
-            questionCounts["N/A"]++;
+            questionCounts["n/a"]++;
         }
     }
 
     // Transform the counts object into an array of objects
     let result = Object.keys(questionCounts).map((key) => ({
         question: key,
         count: questionCounts[key],
     }));
 
     return result;
 }
 
 export function getQAWordFrequency(arr) {
-    // console.log("input", arr);
     return arr.map((item) => {
         const questionTokens = item.question.split(" ").length;
         const answerTokens = item.answer.split(" ").length;
 
         return {
             index: item.index,
             question: +questionTokens,
```

### Comparing `pykoi-0.0.1/pykoi/llm/abs_llm.py` & `pykoi-0.0.2/pykoi/llm/abs_llm.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,7 +22,18 @@
             message (str): The input message used to predict the next word.
             num_of_response (int): How many completions to generate for each prompt.
 
         Raises:
             NotImplementedError: This method must be implemented by subclasses.
         """
         raise NotImplementedError("This method must be implemented by subclasses.")
+
+    @property
+    def name(self):
+        """Return the name of the model.
+
+        This method must be implemented by any subclass of `AbsLlm`.
+
+        Raises:
+            NotImplementedError: This method must be implemented by subclasses.
+        """
+        raise NotImplementedError("This method must be implemented by subclasses.")
```

### Comparing `pykoi-0.0.1/pykoi/llm/huggingface.py` & `pykoi-0.0.2/pykoi/llm/huggingface.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 
 class HuggingfaceModel(AbsLlm):
     """
     This class is a wrapper for the Huggingface model for Language Model (LLM) Chain.
     It inherits from the abstract base class AbsLlm.
     """
+    model_source = "huggingface"
 
     def __init__(
         self,
         pretrained_model_name_or_path: str,
         trust_remote_code: bool = True,
         load_in_8bit: bool = True,
         max_length: int = 100,
@@ -40,39 +41,57 @@
         self._tokenizer = AutoTokenizer.from_pretrained(
             pretrained_model_name_or_path,
             trust_remote_code=trust_remote_code,
             load_in_8bit=load_in_8bit,
             device_map=device_map,
         )
         self._max_length = max_length
+        self._pretrained_model_name_or_path = pretrained_model_name_or_path
         super().__init__()
 
+    @property
+    def name(self):
+        return "_".join([
+            str(HuggingfaceModel.model_source),
+            str(self._pretrained_model_name_or_path),
+            str(self._max_length)
+        ])
+
     def predict(self, message: str, num_of_response: int = 1):
         """
         Predict the next word based on the input message.
 
         Args:
             message (str): The input message for the model.
             num_of_response (int): The number of response to generate. Default is 1.
 
         Returns:
             List[str]: List of response.
         """
-        print("[HuggingfaceModel] encode...")
-        input_ids = self._tokenizer.encode(message, return_tensors="pt")
-        input_ids = input_ids.to("cuda")
-        print("[HuggingfaceModel] generate...")
-        output_ids = self._model.generate(
-            input_ids,
-            max_length=self._max_length,
-            num_return_sequences=num_of_response,
-            do_sample=True,
-            temperature=0.3,
-        )
-        print("[HuggingfaceModel] decode...")
-        response = [
-            self._tokenizer.decode(ids, skip_special_tokens=True) for ids in output_ids
-        ]
+        ## TODO: need to refractor and include all the derivatives of dolly family
+        if "dolly" in self._pretrained_model_name_or_path:
+            from pykoi.llm.instruct_pipeline import InstructionTextGenerationPipeline
+            generate_text = InstructionTextGenerationPipeline(model=self._model, 
+                                                              tokenizer=self._tokenizer)
+            res = generate_text(message)
+            response = [res[0]["generated_text"]]
+        ## all other models except dolly family
+        else:
+            print("[HuggingfaceModel] encode...")
+            input_ids = self._tokenizer.encode(message, return_tensors="pt")
+            input_ids = input_ids.to("cuda")
+            print("[HuggingfaceModel] generate...")
+            output_ids = self._model.generate(
+                input_ids,
+                max_length=self._max_length,
+                num_return_sequences=num_of_response,
+                do_sample=True,
+                temperature=0.3,
+            )
+            print("[HuggingfaceModel] decode...")
+            response = [
+                self._tokenizer.decode(ids, skip_special_tokens=True) for ids in output_ids
+            ]
 
-        response = [resp.split("\n")[1] for resp in response if "\n" in resp]
+            response = [resp.split("\n")[1] for resp in response if "\n" in resp]
 
         return response
```

### Comparing `pykoi-0.0.1/pykoi/llm/model_factory.py` & `pykoi-0.0.2/pykoi/llm/model_factory.py`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.1/pykoi/llm/openai.py` & `pykoi-0.0.2/pykoi/llm/openai.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,14 +13,15 @@
         _max_tokens (int): The maximum number of tokens to generate.
         _temperature (float): The temperature to use for the OpenAI model.
 
     Methods:
         __init__(self, api_key: str, engine: str, max_tokens: int, temperature: float): Initializes the OpenAI model.
         predict(self, message: str): Predicts the next word based on the given message.
     """
+    model_source = "openai"
 
     def __init__(
         self,
         api_key: str,
         engine: str = "davinci",
         max_tokens: int = 100,
         temperature: float = 0.5,
@@ -36,14 +37,22 @@
         """
         openai.api_key = api_key
         self._engine = engine
         self._max_tokens = max_tokens
         self._temperature = temperature
         super().__init__()
 
+    @property
+    def name(self):
+        return "_".join([
+            str(OpenAIModel.model_source),
+            str(self._engine),
+            str(self._max_tokens),
+            str(self._temperature)])
+
     def predict(self, message: str, num_of_response: int = 1):
         """
         Predicts the next word based on the given message.
 
         Args:
             message (str): The message to base the prediction on.
             num_of_response (int): How many completions to generate for each prompt. Defaults to 1.
```

### Comparing `pykoi-0.0.1/pykoi/llm/peft_huggingface.py` & `pykoi-0.0.2/pykoi/llm/peft_huggingface.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     This class is a wrapper for the Huggingface PEFT model for Language Model (LLM).
 
     Attributes:
         _model (PeftModel): The PEFT model.
         _tokenizer (AutoTokenizer): The tokenizer for the model.
         _max_length (int): The maximum length of the generated text.
     """
+    model_source = "peft_huggingface"
 
     def __init__(
         self,
         base_model_path: str,
         lora_model_path: str,
         trust_remote_code: bool = True,
         load_in_8bit: bool = True,
@@ -56,18 +57,29 @@
         self._tokenizer = AutoTokenizer.from_pretrained(
             pretrained_model_name_or_path=base_model_path,
             trust_remote_code=trust_remote_code,
             load_in_8bit=load_in_8bit,
             device_map=device_map,
         )
         self._max_length = max_length
+        self._base_model_path = base_model_path
+        self._lora_model_path = lora_model_path
         self._model.to("cuda")
         self._model.eval()
         super().__init__()
 
+    @property
+    def name(self):
+        return "_".join([
+            str(PeftHuggingfacemodel.model_source),
+            str(self._base_model_path),
+            str(self._lora_model_path),
+            str(self._max_length)
+        ])
+
     def predict(self, message: str, num_of_response: int = 1):
         """
         Predict the next word based on the input message.
 
         Args:
             message (str): The input message for the model.
             num_of_response (int, optional): The number of response to generate. Default is 1.
@@ -75,15 +87,14 @@
         Returns:
             List[str]: List of response.
         """
         print("[HuggingfaceModel] encode...")
         input_ids = self._tokenizer.encode(message, return_tensors="pt")
         input_ids = input_ids.to("cuda")
         print("[HuggingfaceModel] generate...")
-        print("input_ids: ", input_ids)
         output_ids = self._model.generate(
             input_ids=input_ids,
             max_length=self._max_length,
             num_return_sequences=num_of_response,
             do_sample=True,
             temperature=0.3,
         )
```

### Comparing `pykoi-0.0.1/pykoi/state.py` & `pykoi-0.0.2/pykoi/state.py`

 * *Files identical despite different names*

### Comparing `pykoi-0.0.1/pyproject.toml` & `pykoi-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 [tool.poetry]
 name = "pykoi"
-version = "0.0.01"
+version = "0.0.02"
 description = ""
 authors = ["CambioML <wanwanaiai45@gmail.com>"]
 license = "Apache"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
-flask = "2.3.2"
-flask-cors = "4.0.0"
+fastapi = "0.100.0"
+pydantic = "2.1.1"
+starlette = "0.27.0"
+uvicorn = "0.23.1"
 transformers = "4.31.0"
 einops = "0.6.1"
 accelerate = "0.21.0"
 bitsandbytes = "0.40.2"
 scipy = "1.11.1"
 pyngrok = "6.0.0"
 pandas = "2.0.3"
 datasets = "2.13.1"
 evaluate = "0.4.0"
 peft = "0.4.0"
 trl = "0.4.7"
 openai = "0.27.8"
+passlib = "1.7.4"
+bcrypt = "4.0.1"
 
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.3.3"
 
 [build-system]
 requires = ["poetry-core"]
```

