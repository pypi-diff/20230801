# Comparing `tmp/fern_cohere-0.0.5.tar.gz` & `tmp/fern_cohere-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fern_cohere-0.0.5.tar", max compression
+gzip compressed data, was "fern_cohere-0.0.6.tar", max compression
```

## Comparing `fern_cohere-0.0.5.tar` & `fern_cohere-0.0.6.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0        0 2023-07-28 17:02:33.000847 fern_cohere-0.0.5/README.md
--rw-r--r--   0        0        0      390 2023-07-28 17:02:33.000847 fern_cohere-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3582 2023-07-28 17:02:33.004847 fern_cohere-0.0.5/src/cohere/__init__.py
--rw-r--r--   0        0        0    57471 2023-07-28 17:02:33.004847 fern_cohere-0.0.5/src/cohere/client.py
--rw-r--r--   0        0        0      519 2023-07-28 17:02:33.004847 fern_cohere-0.0.5/src/cohere/core/__init__.py
--rw-r--r--   0        0        0      426 2023-07-28 17:02:33.004847 fern_cohere-0.0.5/src/cohere/core/api_error.py
--rw-r--r--   0        0        0     1202 2023-07-28 17:02:33.004847 fern_cohere-0.0.5/src/cohere/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2023-07-28 17:02:33.004847 fern_cohere-0.0.5/src/cohere/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-07-28 17:02:33.004847 fern_cohere-0.0.5/src/cohere/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2023-07-28 17:02:33.004847 fern_cohere-0.0.5/src/cohere/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      156 2023-07-28 17:02:33.004847 fern_cohere-0.0.5/src/cohere/environment.py
--rw-r--r--   0        0        0      221 2023-07-28 17:02:33.004847 fern_cohere-0.0.5/src/cohere/errors/__init__.py
--rw-r--r--   0        0        0      248 2023-07-28 17:02:33.004847 fern_cohere-0.0.5/src/cohere/errors/bad_request_error.py
--rw-r--r--   0        0        0      252 2023-07-28 17:02:33.004847 fern_cohere-0.0.5/src/cohere/errors/internal_server_error.py
--rw-r--r--   0        0        0        0 2023-07-28 17:02:33.004847 fern_cohere-0.0.5/src/cohere/py.typed
--rw-r--r--   0        0        0     5292 2023-07-28 17:02:33.004847 fern_cohere-0.0.5/src/cohere/types/__init__.py
--rw-r--r--   0        0        0      810 2023-07-28 17:02:33.004847 fern_cohere-0.0.5/src/cohere/types/classify_request_examples_item.py
--rw-r--r--   0        0        0     1092 2023-07-28 17:02:33.004847 fern_cohere-0.0.5/src/cohere/types/classify_request_truncate.py
--rw-r--r--   0        0        0     1037 2023-07-28 17:02:33.004847 fern_cohere-0.0.5/src/cohere/types/classify_response.py
--rw-r--r--   0        0        0     1628 2023-07-28 17:02:33.004847 fern_cohere-0.0.5/src/cohere/types/classify_response_classifications_item.py
--rw-r--r--   0        0        0      805 2023-07-28 17:02:33.004847 fern_cohere-0.0.5/src/cohere/types/classify_response_classifications_item_labels_value.py
--rw-r--r--   0        0        0      975 2023-07-28 17:02:33.004847 fern_cohere-0.0.5/src/cohere/types/classify_response_meta_item.py
--rw-r--r--   0        0        0      859 2023-07-28 17:02:33.004847 fern_cohere-0.0.5/src/cohere/types/classify_response_meta_item_api_version_item.py
--rw-r--r--   0        0        0     1138 2023-07-28 17:02:33.004847 fern_cohere-0.0.5/src/cohere/types/detect_language_response.py
--rw-r--r--   0        0        0     1000 2023-07-28 17:02:33.004847 fern_cohere-0.0.5/src/cohere/types/detect_language_response_meta_item.py
--rw-r--r--   0        0        0      865 2023-07-28 17:02:33.004847 fern_cohere-0.0.5/src/cohere/types/detect_language_response_meta_item_api_version_item.py
--rw-r--r--   0        0        0      833 2023-07-28 17:02:33.004847 fern_cohere-0.0.5/src/cohere/types/detect_language_response_results_item.py
--rw-r--r--   0        0        0      963 2023-07-28 17:02:33.004847 fern_cohere-0.0.5/src/cohere/types/detokenize_response.py
--rw-r--r--   0        0        0      983 2023-07-28 17:02:33.004847 fern_cohere-0.0.5/src/cohere/types/detokenize_response_meta_item.py
--rw-r--r--   0        0        0      861 2023-07-28 17:02:33.004847 fern_cohere-0.0.5/src/cohere/types/detokenize_response_meta_item_api_version_item.py
--rw-r--r--   0        0        0     1080 2023-07-28 17:02:33.004847 fern_cohere-0.0.5/src/cohere/types/embed_request_truncate.py
--rw-r--r--   0        0        0     1328 2023-07-28 17:02:33.004847 fern_cohere-0.0.5/src/cohere/types/embed_response.py
--rw-r--r--   0        0        0      963 2023-07-28 17:02:33.004847 fern_cohere-0.0.5/src/cohere/types/embed_response_meta_item.py
--rw-r--r--   0        0        0      856 2023-07-28 17:02:33.004847 fern_cohere-0.0.5/src/cohere/types/embed_response_meta_item_api_version_item.py
--rw-r--r--   0        0        0     1139 2023-07-28 17:02:33.004847 fern_cohere-0.0.5/src/cohere/types/finish_reason.py
--rw-r--r--   0        0        0     1057 2023-07-28 17:02:33.004847 fern_cohere-0.0.5/src/cohere/types/generate_request_return_likelihoods.py
--rw-r--r--   0        0        0     1092 2023-07-28 17:02:33.004847 fern_cohere-0.0.5/src/cohere/types/generate_request_truncate.py
--rw-r--r--   0        0        0     1101 2023-07-28 17:02:33.004847 fern_cohere-0.0.5/src/cohere/types/generation.py
--rw-r--r--   0        0        0      980 2023-07-28 17:02:33.008847 fern_cohere-0.0.5/src/cohere/types/generation_final_response.py
--rw-r--r--   0        0        0      888 2023-07-28 17:02:33.008847 fern_cohere-0.0.5/src/cohere/types/generation_final_response_response.py
--rw-r--r--   0        0        0      950 2023-07-28 17:02:33.008847 fern_cohere-0.0.5/src/cohere/types/generation_meta_item.py
--rw-r--r--   0        0        0      853 2023-07-28 17:02:33.008847 fern_cohere-0.0.5/src/cohere/types/generation_meta_item_api_version_item.py
--rw-r--r--   0        0        0     1007 2023-07-28 17:02:33.008847 fern_cohere-0.0.5/src/cohere/types/generation_stream.py
--rw-r--r--   0        0        0      317 2023-07-28 17:02:33.008847 fern_cohere-0.0.5/src/cohere/types/rerank_request_documents_item.py
--rw-r--r--   0        0        0      854 2023-07-28 17:02:33.008847 fern_cohere-0.0.5/src/cohere/types/rerank_request_documents_item_rerank_request_documents_item.py
--rw-r--r--   0        0        0     1050 2023-07-28 17:02:33.008847 fern_cohere-0.0.5/src/cohere/types/rerank_response.py
--rw-r--r--   0        0        0      876 2023-07-28 17:02:33.008847 fern_cohere-0.0.5/src/cohere/types/rerank_response_meta.py
--rw-r--r--   0        0        0      782 2023-07-28 17:02:33.008847 fern_cohere-0.0.5/src/cohere/types/rerank_response_meta_api_version.py
--rw-r--r--   0        0        0     1153 2023-07-28 17:02:33.008847 fern_cohere-0.0.5/src/cohere/types/rerank_response_results_item.py
--rw-r--r--   0        0        0      887 2023-07-28 17:02:33.008847 fern_cohere-0.0.5/src/cohere/types/rerank_response_results_item_document.py
--rw-r--r--   0        0        0     1622 2023-07-28 17:02:33.008847 fern_cohere-0.0.5/src/cohere/types/single_generation.py
--rw-r--r--   0        0        0     1069 2023-07-28 17:02:33.008847 fern_cohere-0.0.5/src/cohere/types/single_generation_in_stream.py
--rw-r--r--   0        0        0      793 2023-07-28 17:02:33.008847 fern_cohere-0.0.5/src/cohere/types/single_generation_token_likelihoods_item.py
--rw-r--r--   0        0        0      199 2023-07-28 17:02:33.008847 fern_cohere-0.0.5/src/cohere/types/streamed_generation.py
--rw-r--r--   0        0        0      273 2023-07-28 17:02:33.008847 fern_cohere-0.0.5/src/cohere/types/streamed_generation_item.py
--rw-r--r--   0        0        0     1039 2023-07-28 17:02:33.008847 fern_cohere-0.0.5/src/cohere/types/summarize_request_extractiveness.py
--rw-r--r--   0        0        0      779 2023-07-28 17:02:33.008847 fern_cohere-0.0.5/src/cohere/types/summarize_request_format.py
--rw-r--r--   0        0        0      866 2023-07-28 17:02:33.008847 fern_cohere-0.0.5/src/cohere/types/summarize_request_length.py
--rw-r--r--   0        0        0      823 2023-07-28 17:02:33.008847 fern_cohere-0.0.5/src/cohere/types/summarize_request_model.py
--rw-r--r--   0        0        0     1101 2023-07-28 17:02:33.008847 fern_cohere-0.0.5/src/cohere/types/summarize_response.py
--rw-r--r--   0        0        0      979 2023-07-28 17:02:33.008847 fern_cohere-0.0.5/src/cohere/types/summarize_response_meta_item.py
--rw-r--r--   0        0        0      860 2023-07-28 17:02:33.008847 fern_cohere-0.0.5/src/cohere/types/summarize_response_meta_item_api_version_item.py
--rw-r--r--   0        0        0      935 2023-07-28 17:02:33.008847 fern_cohere-0.0.5/src/cohere/types/summarize_response_results_item.py
--rw-r--r--   0        0        0     1016 2023-07-28 17:02:33.008847 fern_cohere-0.0.5/src/cohere/types/tokenize_response.py
--rw-r--r--   0        0        0      975 2023-07-28 17:02:33.008847 fern_cohere-0.0.5/src/cohere/types/tokenize_response_meta_item.py
--rw-r--r--   0        0        0      859 2023-07-28 17:02:33.008847 fern_cohere-0.0.5/src/cohere/types/tokenize_response_meta_item_api_version_item.py
--rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 fern_cohere-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     3313 2023-08-01 13:31:43.306331 fern_cohere-0.0.6/README.md
+-rw-r--r--   0        0        0      390 2023-08-01 13:31:43.306331 fern_cohere-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3582 2023-08-01 13:31:43.306331 fern_cohere-0.0.6/src/cohere/__init__.py
+-rw-r--r--   0        0        0    57471 2023-08-01 13:31:43.306331 fern_cohere-0.0.6/src/cohere/client.py
+-rw-r--r--   0        0        0      519 2023-08-01 13:31:43.306331 fern_cohere-0.0.6/src/cohere/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-08-01 13:31:43.306331 fern_cohere-0.0.6/src/cohere/core/api_error.py
+-rw-r--r--   0        0        0     1202 2023-08-01 13:31:43.306331 fern_cohere-0.0.6/src/cohere/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2023-08-01 13:31:43.306331 fern_cohere-0.0.6/src/cohere/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-08-01 13:31:43.306331 fern_cohere-0.0.6/src/cohere/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2023-08-01 13:31:43.306331 fern_cohere-0.0.6/src/cohere/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      156 2023-08-01 13:31:43.306331 fern_cohere-0.0.6/src/cohere/environment.py
+-rw-r--r--   0        0        0      221 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/errors/__init__.py
+-rw-r--r--   0        0        0      248 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/errors/bad_request_error.py
+-rw-r--r--   0        0        0      252 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/errors/internal_server_error.py
+-rw-r--r--   0        0        0        0 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/py.typed
+-rw-r--r--   0        0        0     5292 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/__init__.py
+-rw-r--r--   0        0        0      810 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/classify_request_examples_item.py
+-rw-r--r--   0        0        0     1092 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/classify_request_truncate.py
+-rw-r--r--   0        0        0     1037 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/classify_response.py
+-rw-r--r--   0        0        0     1628 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/classify_response_classifications_item.py
+-rw-r--r--   0        0        0      805 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/classify_response_classifications_item_labels_value.py
+-rw-r--r--   0        0        0      975 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/classify_response_meta_item.py
+-rw-r--r--   0        0        0      859 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/classify_response_meta_item_api_version_item.py
+-rw-r--r--   0        0        0     1138 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/detect_language_response.py
+-rw-r--r--   0        0        0     1000 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/detect_language_response_meta_item.py
+-rw-r--r--   0        0        0      865 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/detect_language_response_meta_item_api_version_item.py
+-rw-r--r--   0        0        0      833 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/detect_language_response_results_item.py
+-rw-r--r--   0        0        0      963 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/detokenize_response.py
+-rw-r--r--   0        0        0      983 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/detokenize_response_meta_item.py
+-rw-r--r--   0        0        0      861 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/detokenize_response_meta_item_api_version_item.py
+-rw-r--r--   0        0        0     1080 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/embed_request_truncate.py
+-rw-r--r--   0        0        0     1328 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/embed_response.py
+-rw-r--r--   0        0        0      963 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/embed_response_meta_item.py
+-rw-r--r--   0        0        0      856 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/embed_response_meta_item_api_version_item.py
+-rw-r--r--   0        0        0     1139 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/finish_reason.py
+-rw-r--r--   0        0        0     1057 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/generate_request_return_likelihoods.py
+-rw-r--r--   0        0        0     1092 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/generate_request_truncate.py
+-rw-r--r--   0        0        0     1101 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/generation.py
+-rw-r--r--   0        0        0      980 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/generation_final_response.py
+-rw-r--r--   0        0        0      888 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/generation_final_response_response.py
+-rw-r--r--   0        0        0      950 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/generation_meta_item.py
+-rw-r--r--   0        0        0      853 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/generation_meta_item_api_version_item.py
+-rw-r--r--   0        0        0     1007 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/generation_stream.py
+-rw-r--r--   0        0        0      317 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/rerank_request_documents_item.py
+-rw-r--r--   0        0        0      854 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/rerank_request_documents_item_rerank_request_documents_item.py
+-rw-r--r--   0        0        0     1050 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/rerank_response.py
+-rw-r--r--   0        0        0      876 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/rerank_response_meta.py
+-rw-r--r--   0        0        0      782 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/rerank_response_meta_api_version.py
+-rw-r--r--   0        0        0     1153 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/rerank_response_results_item.py
+-rw-r--r--   0        0        0      887 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/rerank_response_results_item_document.py
+-rw-r--r--   0        0        0     1622 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/single_generation.py
+-rw-r--r--   0        0        0     1069 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/single_generation_in_stream.py
+-rw-r--r--   0        0        0      793 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/single_generation_token_likelihoods_item.py
+-rw-r--r--   0        0        0      199 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/streamed_generation.py
+-rw-r--r--   0        0        0      273 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/streamed_generation_item.py
+-rw-r--r--   0        0        0     1039 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/summarize_request_extractiveness.py
+-rw-r--r--   0        0        0      779 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/summarize_request_format.py
+-rw-r--r--   0        0        0      866 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/summarize_request_length.py
+-rw-r--r--   0        0        0      823 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/summarize_request_model.py
+-rw-r--r--   0        0        0     1101 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/summarize_response.py
+-rw-r--r--   0        0        0      979 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/summarize_response_meta_item.py
+-rw-r--r--   0        0        0      860 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/summarize_response_meta_item_api_version_item.py
+-rw-r--r--   0        0        0      935 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/summarize_response_results_item.py
+-rw-r--r--   0        0        0     1016 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/tokenize_response.py
+-rw-r--r--   0        0        0      975 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/tokenize_response_meta_item.py
+-rw-r--r--   0        0        0      859 2023-08-01 13:31:43.310332 fern_cohere-0.0.6/src/cohere/types/tokenize_response_meta_item_api_version_item.py
+-rw-r--r--   0        0        0     3713 1970-01-01 00:00:00.000000 fern_cohere-0.0.6/PKG-INFO
```

### Comparing `fern_cohere-0.0.5/src/cohere/__init__.py` & `fern_cohere-0.0.6/src/cohere/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/client.py` & `fern_cohere-0.0.6/src/cohere/client.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/core/__init__.py` & `fern_cohere-0.0.6/src/cohere/core/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/core/client_wrapper.py` & `fern_cohere-0.0.6/src/cohere/core/client_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     def __init__(self, *, api_key: typing.Union[str, typing.Callable[[], str]]):
         self._api_key = api_key
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "fern-cohere",
-            "X-Fern-SDK-Version": "0.0.5",
+            "X-Fern-SDK-Version": "0.0.6",
         }
         headers["Authorization"] = f"Bearer {self._get_api_key()}"
         return headers
 
     def _get_api_key(self) -> str:
         if isinstance(self._api_key, str):
             return self._api_key
```

### Comparing `fern_cohere-0.0.5/src/cohere/core/datetime_utils.py` & `fern_cohere-0.0.6/src/cohere/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/core/jsonable_encoder.py` & `fern_cohere-0.0.6/src/cohere/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/__init__.py` & `fern_cohere-0.0.6/src/cohere/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/classify_request_examples_item.py` & `fern_cohere-0.0.6/src/cohere/types/classify_request_examples_item.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/classify_request_truncate.py` & `fern_cohere-0.0.6/src/cohere/types/classify_request_truncate.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/classify_response.py` & `fern_cohere-0.0.6/src/cohere/types/classify_response.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/classify_response_classifications_item.py` & `fern_cohere-0.0.6/src/cohere/types/classify_response_classifications_item.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/classify_response_classifications_item_labels_value.py` & `fern_cohere-0.0.6/src/cohere/types/classify_response_classifications_item_labels_value.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/classify_response_meta_item.py` & `fern_cohere-0.0.6/src/cohere/types/classify_response_meta_item.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/classify_response_meta_item_api_version_item.py` & `fern_cohere-0.0.6/src/cohere/types/classify_response_meta_item_api_version_item.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/detect_language_response.py` & `fern_cohere-0.0.6/src/cohere/types/detect_language_response.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/detect_language_response_meta_item.py` & `fern_cohere-0.0.6/src/cohere/types/detect_language_response_meta_item.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/detect_language_response_meta_item_api_version_item.py` & `fern_cohere-0.0.6/src/cohere/types/detect_language_response_meta_item_api_version_item.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/detect_language_response_results_item.py` & `fern_cohere-0.0.6/src/cohere/types/detect_language_response_results_item.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/detokenize_response.py` & `fern_cohere-0.0.6/src/cohere/types/detokenize_response.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/detokenize_response_meta_item.py` & `fern_cohere-0.0.6/src/cohere/types/detokenize_response_meta_item.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/detokenize_response_meta_item_api_version_item.py` & `fern_cohere-0.0.6/src/cohere/types/detokenize_response_meta_item_api_version_item.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/embed_request_truncate.py` & `fern_cohere-0.0.6/src/cohere/types/embed_request_truncate.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/embed_response.py` & `fern_cohere-0.0.6/src/cohere/types/embed_response.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/embed_response_meta_item.py` & `fern_cohere-0.0.6/src/cohere/types/embed_response_meta_item.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/embed_response_meta_item_api_version_item.py` & `fern_cohere-0.0.6/src/cohere/types/embed_response_meta_item_api_version_item.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/finish_reason.py` & `fern_cohere-0.0.6/src/cohere/types/finish_reason.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/generate_request_return_likelihoods.py` & `fern_cohere-0.0.6/src/cohere/types/generate_request_return_likelihoods.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/generate_request_truncate.py` & `fern_cohere-0.0.6/src/cohere/types/generate_request_truncate.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/generation.py` & `fern_cohere-0.0.6/src/cohere/types/generation.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/generation_final_response.py` & `fern_cohere-0.0.6/src/cohere/types/generation_final_response.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/generation_final_response_response.py` & `fern_cohere-0.0.6/src/cohere/types/generation_final_response_response.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/generation_meta_item.py` & `fern_cohere-0.0.6/src/cohere/types/generation_meta_item.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/generation_meta_item_api_version_item.py` & `fern_cohere-0.0.6/src/cohere/types/generation_meta_item_api_version_item.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/generation_stream.py` & `fern_cohere-0.0.6/src/cohere/types/generation_stream.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/rerank_request_documents_item_rerank_request_documents_item.py` & `fern_cohere-0.0.6/src/cohere/types/rerank_request_documents_item_rerank_request_documents_item.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/rerank_response.py` & `fern_cohere-0.0.6/src/cohere/types/rerank_response.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/rerank_response_meta.py` & `fern_cohere-0.0.6/src/cohere/types/rerank_response_meta.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/rerank_response_meta_api_version.py` & `fern_cohere-0.0.6/src/cohere/types/rerank_response_meta_api_version.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/rerank_response_results_item.py` & `fern_cohere-0.0.6/src/cohere/types/rerank_response_results_item.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/rerank_response_results_item_document.py` & `fern_cohere-0.0.6/src/cohere/types/rerank_response_results_item_document.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/single_generation.py` & `fern_cohere-0.0.6/src/cohere/types/single_generation.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/single_generation_in_stream.py` & `fern_cohere-0.0.6/src/cohere/types/single_generation_in_stream.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/single_generation_token_likelihoods_item.py` & `fern_cohere-0.0.6/src/cohere/types/single_generation_token_likelihoods_item.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/summarize_request_extractiveness.py` & `fern_cohere-0.0.6/src/cohere/types/summarize_request_extractiveness.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/summarize_request_format.py` & `fern_cohere-0.0.6/src/cohere/types/summarize_request_format.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/summarize_request_length.py` & `fern_cohere-0.0.6/src/cohere/types/summarize_request_length.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/summarize_request_model.py` & `fern_cohere-0.0.6/src/cohere/types/summarize_request_model.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/summarize_response.py` & `fern_cohere-0.0.6/src/cohere/types/summarize_response.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/summarize_response_meta_item.py` & `fern_cohere-0.0.6/src/cohere/types/summarize_response_meta_item.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/summarize_response_meta_item_api_version_item.py` & `fern_cohere-0.0.6/src/cohere/types/summarize_response_meta_item_api_version_item.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/summarize_response_results_item.py` & `fern_cohere-0.0.6/src/cohere/types/summarize_response_results_item.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/tokenize_response.py` & `fern_cohere-0.0.6/src/cohere/types/tokenize_response.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/tokenize_response_meta_item.py` & `fern_cohere-0.0.6/src/cohere/types/tokenize_response_meta_item.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.5/src/cohere/types/tokenize_response_meta_item_api_version_item.py` & `fern_cohere-0.0.6/src/cohere/types/tokenize_response_meta_item_api_version_item.py`

 * *Files identical despite different names*

