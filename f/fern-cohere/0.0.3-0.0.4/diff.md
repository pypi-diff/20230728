# Comparing `tmp/fern_cohere-0.0.3.tar.gz` & `tmp/fern_cohere-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fern_cohere-0.0.3.tar", max compression
+gzip compressed data, was "fern_cohere-0.0.4.tar", max compression
```

## Comparing `fern_cohere-0.0.3.tar` & `fern_cohere-0.0.4.tar`

### file list

```diff
@@ -1,66 +1,67 @@
--rw-r--r--   0        0        0        0 2023-07-28 16:47:14.631223 fern_cohere-0.0.3/README.md
--rw-r--r--   0        0        0      372 2023-07-28 16:47:14.631223 fern_cohere-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3582 2023-07-28 16:47:14.631223 fern_cohere-0.0.3/src/cohere/__init__.py
--rw-r--r--   0        0        0    28778 2023-07-28 16:47:14.631223 fern_cohere-0.0.3/src/cohere/client.py
--rw-r--r--   0        0        0      348 2023-07-28 16:47:14.631223 fern_cohere-0.0.3/src/cohere/core/__init__.py
--rw-r--r--   0        0        0      426 2023-07-28 16:47:14.631223 fern_cohere-0.0.3/src/cohere/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-07-28 16:47:14.631223 fern_cohere-0.0.3/src/cohere/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-07-28 16:47:14.631223 fern_cohere-0.0.3/src/cohere/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-07-28 16:47:14.631223 fern_cohere-0.0.3/src/cohere/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      156 2023-07-28 16:47:14.631223 fern_cohere-0.0.3/src/cohere/environment.py
--rw-r--r--   0        0        0      221 2023-07-28 16:47:14.631223 fern_cohere-0.0.3/src/cohere/errors/__init__.py
--rw-r--r--   0        0        0      248 2023-07-28 16:47:14.631223 fern_cohere-0.0.3/src/cohere/errors/bad_request_error.py
--rw-r--r--   0        0        0      252 2023-07-28 16:47:14.631223 fern_cohere-0.0.3/src/cohere/errors/internal_server_error.py
--rw-r--r--   0        0        0        0 2023-07-28 16:47:14.631223 fern_cohere-0.0.3/src/cohere/py.typed
--rw-r--r--   0        0        0     5292 2023-07-28 16:47:14.631223 fern_cohere-0.0.3/src/cohere/types/__init__.py
--rw-r--r--   0        0        0      810 2023-07-28 16:47:14.631223 fern_cohere-0.0.3/src/cohere/types/classify_request_examples_item.py
--rw-r--r--   0        0        0     1092 2023-07-28 16:47:14.631223 fern_cohere-0.0.3/src/cohere/types/classify_request_truncate.py
--rw-r--r--   0        0        0     1037 2023-07-28 16:47:14.631223 fern_cohere-0.0.3/src/cohere/types/classify_response.py
--rw-r--r--   0        0        0     1670 2023-07-28 16:47:14.631223 fern_cohere-0.0.3/src/cohere/types/classify_response_classifications_item.py
--rw-r--r--   0        0        0      805 2023-07-28 16:47:14.631223 fern_cohere-0.0.3/src/cohere/types/classify_response_classifications_item_labels_value.py
--rw-r--r--   0        0        0      975 2023-07-28 16:47:14.631223 fern_cohere-0.0.3/src/cohere/types/classify_response_meta_item.py
--rw-r--r--   0        0        0      859 2023-07-28 16:47:14.631223 fern_cohere-0.0.3/src/cohere/types/classify_response_meta_item_api_version_item.py
--rw-r--r--   0        0        0     1142 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/detect_language_response.py
--rw-r--r--   0        0        0     1000 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/detect_language_response_meta_item.py
--rw-r--r--   0        0        0      865 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/detect_language_response_meta_item_api_version_item.py
--rw-r--r--   0        0        0      833 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/detect_language_response_results_item.py
--rw-r--r--   0        0        0      967 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/detokenize_response.py
--rw-r--r--   0        0        0      983 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/detokenize_response_meta_item.py
--rw-r--r--   0        0        0      861 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/detokenize_response_meta_item_api_version_item.py
--rw-r--r--   0        0        0     1080 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/embed_request_truncate.py
--rw-r--r--   0        0        0     1358 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/embed_response.py
--rw-r--r--   0        0        0      963 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/embed_response_meta_item.py
--rw-r--r--   0        0        0      856 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/embed_response_meta_item_api_version_item.py
--rw-r--r--   0        0        0     1139 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/finish_reason.py
--rw-r--r--   0        0        0     1057 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/generate_request_return_likelihoods.py
--rw-r--r--   0        0        0     1092 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/generate_request_truncate.py
--rw-r--r--   0        0        0     1109 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/generation.py
--rw-r--r--   0        0        0      980 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/generation_final_response.py
--rw-r--r--   0        0        0      888 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/generation_final_response_response.py
--rw-r--r--   0        0        0      950 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/generation_meta_item.py
--rw-r--r--   0        0        0      853 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/generation_meta_item_api_version_item.py
--rw-r--r--   0        0        0     1015 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/generation_stream.py
--rw-r--r--   0        0        0      317 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/rerank_request_documents_item.py
--rw-r--r--   0        0        0      858 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/rerank_request_documents_item_rerank_request_documents_item.py
--rw-r--r--   0        0        0     1068 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/rerank_response.py
--rw-r--r--   0        0        0      876 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/rerank_response_meta.py
--rw-r--r--   0        0        0      782 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/rerank_response_meta_api_version.py
--rw-r--r--   0        0        0     1165 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/rerank_response_results_item.py
--rw-r--r--   0        0        0      891 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/rerank_response_results_item_document.py
--rw-r--r--   0        0        0     1652 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/single_generation.py
--rw-r--r--   0        0        0     1077 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/single_generation_in_stream.py
--rw-r--r--   0        0        0      793 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/single_generation_token_likelihoods_item.py
--rw-r--r--   0        0        0      199 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/streamed_generation.py
--rw-r--r--   0        0        0      273 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/streamed_generation_item.py
--rw-r--r--   0        0        0     1039 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/summarize_request_extractiveness.py
--rw-r--r--   0        0        0      779 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/summarize_request_format.py
--rw-r--r--   0        0        0      866 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/summarize_request_length.py
--rw-r--r--   0        0        0      823 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/summarize_request_model.py
--rw-r--r--   0        0        0     1105 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/summarize_response.py
--rw-r--r--   0        0        0      979 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/summarize_response_meta_item.py
--rw-r--r--   0        0        0      860 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/summarize_response_meta_item_api_version_item.py
--rw-r--r--   0        0        0      943 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/summarize_response_results_item.py
--rw-r--r--   0        0        0     1020 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/tokenize_response.py
--rw-r--r--   0        0        0      975 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/tokenize_response_meta_item.py
--rw-r--r--   0        0        0      859 2023-07-28 16:47:14.635223 fern_cohere-0.0.3/src/cohere/types/tokenize_response_meta_item_api_version_item.py
--rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 fern_cohere-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-28 16:56:27.489351 fern_cohere-0.0.4/README.md
+-rw-r--r--   0        0        0      390 2023-07-28 16:56:27.489351 fern_cohere-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3582 2023-07-28 16:56:27.489351 fern_cohere-0.0.4/src/cohere/__init__.py
+-rw-r--r--   0        0        0    57405 2023-07-28 16:56:27.489351 fern_cohere-0.0.4/src/cohere/client.py
+-rw-r--r--   0        0        0      519 2023-07-28 16:56:27.489351 fern_cohere-0.0.4/src/cohere/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-28 16:56:27.489351 fern_cohere-0.0.4/src/cohere/core/api_error.py
+-rw-r--r--   0        0        0     1174 2023-07-28 16:56:27.489351 fern_cohere-0.0.4/src/cohere/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2023-07-28 16:56:27.489351 fern_cohere-0.0.4/src/cohere/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-07-28 16:56:27.489351 fern_cohere-0.0.4/src/cohere/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2023-07-28 16:56:27.489351 fern_cohere-0.0.4/src/cohere/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      156 2023-07-28 16:56:27.489351 fern_cohere-0.0.4/src/cohere/environment.py
+-rw-r--r--   0        0        0      221 2023-07-28 16:56:27.489351 fern_cohere-0.0.4/src/cohere/errors/__init__.py
+-rw-r--r--   0        0        0      248 2023-07-28 16:56:27.489351 fern_cohere-0.0.4/src/cohere/errors/bad_request_error.py
+-rw-r--r--   0        0        0      252 2023-07-28 16:56:27.489351 fern_cohere-0.0.4/src/cohere/errors/internal_server_error.py
+-rw-r--r--   0        0        0        0 2023-07-28 16:56:27.489351 fern_cohere-0.0.4/src/cohere/py.typed
+-rw-r--r--   0        0        0     5292 2023-07-28 16:56:27.489351 fern_cohere-0.0.4/src/cohere/types/__init__.py
+-rw-r--r--   0        0        0      810 2023-07-28 16:56:27.489351 fern_cohere-0.0.4/src/cohere/types/classify_request_examples_item.py
+-rw-r--r--   0        0        0     1092 2023-07-28 16:56:27.489351 fern_cohere-0.0.4/src/cohere/types/classify_request_truncate.py
+-rw-r--r--   0        0        0     1037 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/classify_response.py
+-rw-r--r--   0        0        0     1628 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/classify_response_classifications_item.py
+-rw-r--r--   0        0        0      805 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/classify_response_classifications_item_labels_value.py
+-rw-r--r--   0        0        0      975 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/classify_response_meta_item.py
+-rw-r--r--   0        0        0      859 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/classify_response_meta_item_api_version_item.py
+-rw-r--r--   0        0        0     1138 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/detect_language_response.py
+-rw-r--r--   0        0        0     1000 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/detect_language_response_meta_item.py
+-rw-r--r--   0        0        0      865 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/detect_language_response_meta_item_api_version_item.py
+-rw-r--r--   0        0        0      833 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/detect_language_response_results_item.py
+-rw-r--r--   0        0        0      963 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/detokenize_response.py
+-rw-r--r--   0        0        0      983 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/detokenize_response_meta_item.py
+-rw-r--r--   0        0        0      861 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/detokenize_response_meta_item_api_version_item.py
+-rw-r--r--   0        0        0     1080 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/embed_request_truncate.py
+-rw-r--r--   0        0        0     1328 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/embed_response.py
+-rw-r--r--   0        0        0      963 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/embed_response_meta_item.py
+-rw-r--r--   0        0        0      856 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/embed_response_meta_item_api_version_item.py
+-rw-r--r--   0        0        0     1139 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/finish_reason.py
+-rw-r--r--   0        0        0     1057 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/generate_request_return_likelihoods.py
+-rw-r--r--   0        0        0     1092 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/generate_request_truncate.py
+-rw-r--r--   0        0        0     1101 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/generation.py
+-rw-r--r--   0        0        0      980 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/generation_final_response.py
+-rw-r--r--   0        0        0      888 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/generation_final_response_response.py
+-rw-r--r--   0        0        0      950 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/generation_meta_item.py
+-rw-r--r--   0        0        0      853 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/generation_meta_item_api_version_item.py
+-rw-r--r--   0        0        0     1007 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/generation_stream.py
+-rw-r--r--   0        0        0      317 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/rerank_request_documents_item.py
+-rw-r--r--   0        0        0      854 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/rerank_request_documents_item_rerank_request_documents_item.py
+-rw-r--r--   0        0        0     1050 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/rerank_response.py
+-rw-r--r--   0        0        0      876 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/rerank_response_meta.py
+-rw-r--r--   0        0        0      782 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/rerank_response_meta_api_version.py
+-rw-r--r--   0        0        0     1153 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/rerank_response_results_item.py
+-rw-r--r--   0        0        0      887 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/rerank_response_results_item_document.py
+-rw-r--r--   0        0        0     1622 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/single_generation.py
+-rw-r--r--   0        0        0     1069 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/single_generation_in_stream.py
+-rw-r--r--   0        0        0      793 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/single_generation_token_likelihoods_item.py
+-rw-r--r--   0        0        0      199 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/streamed_generation.py
+-rw-r--r--   0        0        0      273 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/streamed_generation_item.py
+-rw-r--r--   0        0        0     1039 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/summarize_request_extractiveness.py
+-rw-r--r--   0        0        0      779 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/summarize_request_format.py
+-rw-r--r--   0        0        0      866 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/summarize_request_length.py
+-rw-r--r--   0        0        0      823 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/summarize_request_model.py
+-rw-r--r--   0        0        0     1101 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/summarize_response.py
+-rw-r--r--   0        0        0      979 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/summarize_response_meta_item.py
+-rw-r--r--   0        0        0      860 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/summarize_response_meta_item_api_version_item.py
+-rw-r--r--   0        0        0      935 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/summarize_response_results_item.py
+-rw-r--r--   0        0        0     1016 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/tokenize_response.py
+-rw-r--r--   0        0        0      975 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/tokenize_response_meta_item.py
+-rw-r--r--   0        0        0      859 2023-07-28 16:56:27.493351 fern_cohere-0.0.4/src/cohere/types/tokenize_response_meta_item_api_version_item.py
+-rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 fern_cohere-0.0.4/PKG-INFO
```

### Comparing `fern_cohere-0.0.3/src/cohere/__init__.py` & `fern_cohere-0.0.4/src/cohere/__init__.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # This file was auto-generated by Fern from our API Definition.
 
-from .environment import CohereEnvironment
-from .errors import BadRequestError, InternalServerError
 from .types import (
     ClassifyRequestExamplesItem,
     ClassifyRequestTruncate,
     ClassifyResponse,
     ClassifyResponseClassificationsItem,
     ClassifyResponseClassificationsItemLabelsValue,
     ClassifyResponseMetaItem,
@@ -50,14 +48,16 @@
     SummarizeResponseMetaItem,
     SummarizeResponseMetaItemApiVersionItem,
     SummarizeResponseResultsItem,
     TokenizeResponse,
     TokenizeResponseMetaItem,
     TokenizeResponseMetaItemApiVersionItem,
 )
+from .errors import BadRequestError, InternalServerError
+from .environment import CohereEnvironment
 
 __all__ = [
     "BadRequestError",
     "ClassifyRequestExamplesItem",
     "ClassifyRequestTruncate",
     "ClassifyResponse",
     "ClassifyResponseClassificationsItem",
```

### Comparing `fern_cohere-0.0.3/src/cohere/core/datetime_utils.py` & `fern_cohere-0.0.4/src/cohere/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.3/src/cohere/core/jsonable_encoder.py` & `fern_cohere-0.0.4/src/cohere/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.3/src/cohere/types/__init__.py` & `fern_cohere-0.0.4/src/cohere/types/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.3/src/cohere/types/classify_request_examples_item.py` & `fern_cohere-0.0.4/src/cohere/types/classify_request_examples_item.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.3/src/cohere/types/classify_request_truncate.py` & `fern_cohere-0.0.4/src/cohere/types/classify_request_truncate.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.3/src/cohere/types/classify_response.py` & `fern_cohere-0.0.4/src/cohere/types/classify_response.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.3/src/cohere/types/classify_response_classifications_item.py` & `fern_cohere-0.0.4/src/cohere/types/classify_response_classifications_item.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,24 +7,22 @@
 
 from ..core.datetime_utils import serialize_datetime
 from .classify_response_classifications_item_labels_value import ClassifyResponseClassificationsItemLabelsValue
 
 
 class ClassifyResponseClassificationsItem(pydantic.BaseModel):
     id: str
-    input: typing.Optional[str] = pydantic.Field(description=("The input text that was classified\n"))
-    prediction: str = pydantic.Field(description=("The predicted label for the associated query\n"))
-    confidence: float = pydantic.Field(description=("The confidence score for the top predicted class\n"))
+    input: typing.Optional[str] = pydantic.Field(description="The input text that was classified")
+    prediction: str = pydantic.Field(description="The predicted label for the associated query")
+    confidence: float = pydantic.Field(description="The confidence score for the top predicted class")
     labels: typing.Dict[str, ClassifyResponseClassificationsItemLabelsValue] = pydantic.Field(
-        description=(
-            "A map containing each label and its confidence score according to the classifier. All the confidence scores add up to 1.\n"
-        )
+        description="A map containing each label and its confidence score according to the classifier. All the confidence scores add up to 1."
     )
     confidences: typing.Optional[typing.List[typing.Dict[str, typing.Any]]] = pydantic.Field(
-        description=("An array containing each label and its confidence score according to the classifier\n")
+        description="An array containing each label and its confidence score according to the classifier"
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `fern_cohere-0.0.3/src/cohere/types/classify_response_classifications_item_labels_value.py` & `fern_cohere-0.0.4/src/cohere/types/classify_response_classifications_item_labels_value.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.3/src/cohere/types/classify_response_meta_item.py` & `fern_cohere-0.0.4/src/cohere/types/classify_response_meta_item.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.3/src/cohere/types/classify_response_meta_item_api_version_item.py` & `fern_cohere-0.0.4/src/cohere/types/classify_response_meta_item_api_version_item.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.3/src/cohere/types/detect_language_response.py` & `fern_cohere-0.0.4/src/cohere/types/summarize_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .detect_language_response_meta_item import DetectLanguageResponseMetaItem
-from .detect_language_response_results_item import DetectLanguageResponseResultsItem
+from .summarize_response_meta_item import SummarizeResponseMetaItem
+from .summarize_response_results_item import SummarizeResponseResultsItem
 
 
-class DetectLanguageResponse(pydantic.BaseModel):
-    results: typing.Optional[typing.List[DetectLanguageResponseResultsItem]] = pydantic.Field(
-        description=("List of languages, one per input text\n")
+class SummarizeResponse(pydantic.BaseModel):
+    results: typing.Optional[typing.List[SummarizeResponseResultsItem]] = pydantic.Field(
+        description="List of languages, one per input text"
     )
-    meta: typing.Optional[typing.List[DetectLanguageResponseMetaItem]]
+    meta: typing.Optional[typing.List[SummarizeResponseMetaItem]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_cohere-0.0.3/src/cohere/types/detect_language_response_meta_item.py` & `fern_cohere-0.0.4/src/cohere/types/detect_language_response_meta_item.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.3/src/cohere/types/detect_language_response_meta_item_api_version_item.py` & `fern_cohere-0.0.4/src/cohere/types/detect_language_response_meta_item_api_version_item.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.3/src/cohere/types/detect_language_response_results_item.py` & `fern_cohere-0.0.4/src/cohere/types/detect_language_response_results_item.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.3/src/cohere/types/detokenize_response.py` & `fern_cohere-0.0.4/src/cohere/types/detokenize_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 from .detokenize_response_meta_item import DetokenizeResponseMetaItem
 
 
 class DetokenizeResponse(pydantic.BaseModel):
-    text: str = pydantic.Field(description=("A string representing the list of tokens.\n"))
+    text: str = pydantic.Field(description="A string representing the list of tokens.")
     meta: typing.Optional[typing.List[DetokenizeResponseMetaItem]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `fern_cohere-0.0.3/src/cohere/types/detokenize_response_meta_item.py` & `fern_cohere-0.0.4/src/cohere/types/detokenize_response_meta_item.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.3/src/cohere/types/detokenize_response_meta_item_api_version_item.py` & `fern_cohere-0.0.4/src/cohere/types/detokenize_response_meta_item_api_version_item.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.3/src/cohere/types/embed_request_truncate.py` & `fern_cohere-0.0.4/src/cohere/types/embed_request_truncate.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.3/src/cohere/types/embed_response.py` & `fern_cohere-0.0.4/src/cohere/types/embed_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,19 +8,17 @@
 from ..core.datetime_utils import serialize_datetime
 from .embed_response_meta_item import EmbedResponseMetaItem
 
 
 class EmbedResponse(pydantic.BaseModel):
     id: str
     embeddings: typing.List[typing.List[float]] = pydantic.Field(
-        description=(
-            "An array of embeddings, where each embedding is an array of floats. The length of the `embeddings` array will be the same as the length of the original `texts` array. The `small` embeddings have length `1024` and the large embeddings have length `4096`.\n"
-        )
+        description="An array of embeddings, where each embedding is an array of floats. The length of the `embeddings` array will be the same as the length of the original `texts` array. The `small` embeddings have length `1024` and the large embeddings have length `4096`."
     )
-    texts: typing.List[str] = pydantic.Field(description=("The text entries for which embeddings were returned.\n"))
+    texts: typing.List[str] = pydantic.Field(description="The text entries for which embeddings were returned.")
     meta: typing.Optional[typing.List[EmbedResponseMetaItem]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `fern_cohere-0.0.3/src/cohere/types/embed_response_meta_item.py` & `fern_cohere-0.0.4/src/cohere/types/embed_response_meta_item.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.3/src/cohere/types/embed_response_meta_item_api_version_item.py` & `fern_cohere-0.0.4/src/cohere/types/embed_response_meta_item_api_version_item.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.3/src/cohere/types/finish_reason.py` & `fern_cohere-0.0.4/src/cohere/types/finish_reason.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.3/src/cohere/types/generate_request_return_likelihoods.py` & `fern_cohere-0.0.4/src/cohere/types/generate_request_return_likelihoods.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.3/src/cohere/types/generate_request_truncate.py` & `fern_cohere-0.0.4/src/cohere/types/generate_request_truncate.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.3/src/cohere/types/generation.py` & `fern_cohere-0.0.4/src/cohere/types/generation.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from ..core.datetime_utils import serialize_datetime
 from .generation_meta_item import GenerationMetaItem
 from .single_generation import SingleGeneration
 
 
 class Generation(pydantic.BaseModel):
     id: str
-    prompt: typing.Optional[str] = pydantic.Field(description=("Prompt used for generations.\n"))
-    generations: typing.List[SingleGeneration] = pydantic.Field(description=("List of generated results\n"))
+    prompt: typing.Optional[str] = pydantic.Field(description="Prompt used for generations.")
+    generations: typing.List[SingleGeneration] = pydantic.Field(description="List of generated results")
     meta: typing.Optional[typing.List[GenerationMetaItem]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `fern_cohere-0.0.3/src/cohere/types/generation_final_response.py` & `fern_cohere-0.0.4/src/cohere/types/generation_final_response.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.3/src/cohere/types/generation_final_response_response.py` & `fern_cohere-0.0.4/src/cohere/types/generation_final_response_response.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.3/src/cohere/types/generation_meta_item.py` & `fern_cohere-0.0.4/src/cohere/types/generation_meta_item.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.3/src/cohere/types/generation_meta_item_api_version_item.py` & `fern_cohere-0.0.4/src/cohere/types/generation_meta_item_api_version_item.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.3/src/cohere/types/generation_stream.py` & `fern_cohere-0.0.4/src/cohere/types/tokenize_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
+from .tokenize_response_meta_item import TokenizeResponseMetaItem
 
 
-class GenerationStream(pydantic.BaseModel):
-    text: str = pydantic.Field(description=("A segment of text of the generation.\n"))
-    index: typing.Optional[int] = pydantic.Field(
-        description=("Refers to the nth generation. Only present when `num_generations` is greater than zero.\n")
-    )
-    is_finished: bool
+class TokenizeResponse(pydantic.BaseModel):
+    tokens: typing.List[int] = pydantic.Field(description="An array of tokens, where each token is an integer.")
+    token_strings: typing.List[str]
+    meta: typing.Optional[typing.List[TokenizeResponseMetaItem]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_cohere-0.0.3/src/cohere/types/rerank_request_documents_item_rerank_request_documents_item.py` & `fern_cohere-0.0.4/src/cohere/types/rerank_request_documents_item_rerank_request_documents_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
 class RerankRequestDocumentsItemRerankRequestDocumentsItem(pydantic.BaseModel):
-    text: str = pydantic.Field(description=("The text of the document to rerank.\n"))
+    text: str = pydantic.Field(description="The text of the document to rerank.")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_cohere-0.0.3/src/cohere/types/rerank_response.py` & `fern_cohere-0.0.4/src/cohere/types/rerank_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,17 +8,15 @@
 from ..core.datetime_utils import serialize_datetime
 from .rerank_response_meta import RerankResponseMeta
 from .rerank_response_results_item import RerankResponseResultsItem
 
 
 class RerankResponse(pydantic.BaseModel):
     id: typing.Optional[str]
-    results: typing.List[RerankResponseResultsItem] = pydantic.Field(
-        description=("An ordered list of ranked documents\n")
-    )
+    results: typing.List[RerankResponseResultsItem] = pydantic.Field(description="An ordered list of ranked documents")
     meta: typing.Optional[RerankResponseMeta]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `fern_cohere-0.0.3/src/cohere/types/rerank_response_meta.py` & `fern_cohere-0.0.4/src/cohere/types/rerank_response_meta.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.3/src/cohere/types/rerank_response_meta_api_version.py` & `fern_cohere-0.0.4/src/cohere/types/rerank_response_meta_api_version.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.3/src/cohere/types/rerank_response_results_item.py` & `fern_cohere-0.0.4/src/cohere/types/summarize_response_results_item.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,23 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .rerank_response_results_item_document import RerankResponseResultsItemDocument
 
 
-class RerankResponseResultsItem(pydantic.BaseModel):
-    document: typing.Optional[RerankResponseResultsItemDocument] = pydantic.Field(
-        description=("The doc object which was ranked\n")
-    )
-    index: int = pydantic.Field(description=("The index of the input document\n"))
-    relevance_score: float = pydantic.Field(description=("A relevance score assigned to the ranking\n"))
+class SummarizeResponseResultsItem(pydantic.BaseModel):
+    id: typing.Optional[str] = pydantic.Field(description="Generated ID for the summary")
+    summary: typing.Optional[str] = pydantic.Field(description="Generated summary for the text")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_cohere-0.0.3/src/cohere/types/rerank_response_results_item_document.py` & `fern_cohere-0.0.4/src/cohere/types/tokenize_response_meta_item_api_version_item.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,20 +4,18 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class RerankResponseResultsItemDocument(pydantic.BaseModel):
-    """
-    The doc object which was ranked
-    """
-
-    text: str = pydantic.Field(description=("The text of the document to rerank\n"))
+class TokenizeResponseMetaItemApiVersionItem(pydantic.BaseModel):
+    version: str
+    is_deprecated: typing.Optional[bool]
+    is_experimental: typing.Optional[bool]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_cohere-0.0.3/src/cohere/types/single_generation.py` & `fern_cohere-0.0.4/src/cohere/types/single_generation.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,21 +9,19 @@
 from .single_generation_token_likelihoods_item import SingleGenerationTokenLikelihoodsItem
 
 
 class SingleGeneration(pydantic.BaseModel):
     id: str
     text: str
     index: typing.Optional[int] = pydantic.Field(
-        description=("Refers to the nth generation. Only present when `num_generations` is greater than zero.\n")
+        description="Refers to the nth generation. Only present when `num_generations` is greater than zero."
     )
     likelihood: typing.Optional[float]
     token_likelihoods: typing.Optional[typing.List[SingleGenerationTokenLikelihoodsItem]] = pydantic.Field(
-        description=(
-            "Only returned if `return_likelihoods` is set to `GENERATION` or `ALL`. The likelihood refers to the average log-likelihood of the entire specified string, which is useful for [evaluating the performance of your model](likelihood-eval), especially if you've created a [custom model](/docs/training-custom-models). Individual token likelihoods provide the log-likelihood of each token. The first token will not have a likelihood.\n"
-        )
+        description="Only returned if `return_likelihoods` is set to `GENERATION` or `ALL`. The likelihood refers to the average log-likelihood of the entire specified string, which is useful for [evaluating the performance of your model](likelihood-eval), especially if you've created a [custom model](/docs/training-custom-models). Individual token likelihoods provide the log-likelihood of each token. The first token will not have a likelihood."
     )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `fern_cohere-0.0.3/src/cohere/types/single_generation_in_stream.py` & `fern_cohere-0.0.4/src/cohere/types/single_generation_in_stream.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 from ..core.datetime_utils import serialize_datetime
 from .finish_reason import FinishReason
 
 
 class SingleGenerationInStream(pydantic.BaseModel):
     id: str
-    text: str = pydantic.Field(description=("Full text of the generation.\n"))
+    text: str = pydantic.Field(description="Full text of the generation.")
     index: typing.Optional[int] = pydantic.Field(
-        description=("Refers to the nth generation. Only present when `num_generations` is greater than zero.\n")
+        description="Refers to the nth generation. Only present when `num_generations` is greater than zero."
     )
     finish_reason: FinishReason
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `fern_cohere-0.0.3/src/cohere/types/single_generation_token_likelihoods_item.py` & `fern_cohere-0.0.4/src/cohere/types/single_generation_token_likelihoods_item.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.3/src/cohere/types/summarize_request_extractiveness.py` & `fern_cohere-0.0.4/src/cohere/types/summarize_request_extractiveness.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.3/src/cohere/types/summarize_request_format.py` & `fern_cohere-0.0.4/src/cohere/types/summarize_request_format.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.3/src/cohere/types/summarize_request_length.py` & `fern_cohere-0.0.4/src/cohere/types/summarize_request_length.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.3/src/cohere/types/summarize_request_model.py` & `fern_cohere-0.0.4/src/cohere/types/summarize_request_model.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.3/src/cohere/types/summarize_response.py` & `fern_cohere-0.0.4/src/cohere/types/summarize_response_meta_item.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,23 +2,20 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .summarize_response_meta_item import SummarizeResponseMetaItem
-from .summarize_response_results_item import SummarizeResponseResultsItem
+from .summarize_response_meta_item_api_version_item import SummarizeResponseMetaItemApiVersionItem
 
 
-class SummarizeResponse(pydantic.BaseModel):
-    results: typing.Optional[typing.List[SummarizeResponseResultsItem]] = pydantic.Field(
-        description=("List of languages, one per input text\n")
-    )
-    meta: typing.Optional[typing.List[SummarizeResponseMetaItem]]
+class SummarizeResponseMetaItem(pydantic.BaseModel):
+    api_version: typing.Optional[typing.List[SummarizeResponseMetaItemApiVersionItem]]
+    warnings: typing.Optional[typing.List[str]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_cohere-0.0.3/src/cohere/types/summarize_response_meta_item.py` & `fern_cohere-0.0.4/src/cohere/types/tokenize_response_meta_item.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .summarize_response_meta_item_api_version_item import SummarizeResponseMetaItemApiVersionItem
+from .tokenize_response_meta_item_api_version_item import TokenizeResponseMetaItemApiVersionItem
 
 
-class SummarizeResponseMetaItem(pydantic.BaseModel):
-    api_version: typing.Optional[typing.List[SummarizeResponseMetaItemApiVersionItem]]
+class TokenizeResponseMetaItem(pydantic.BaseModel):
+    api_version: typing.Optional[typing.List[TokenizeResponseMetaItemApiVersionItem]]
     warnings: typing.Optional[typing.List[str]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `fern_cohere-0.0.3/src/cohere/types/summarize_response_meta_item_api_version_item.py` & `fern_cohere-0.0.4/src/cohere/types/summarize_response_meta_item_api_version_item.py`

 * *Files identical despite different names*

### Comparing `fern_cohere-0.0.3/src/cohere/types/summarize_response_results_item.py` & `fern_cohere-0.0.4/src/cohere/types/generation_stream.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,17 +4,20 @@
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
 
 
-class SummarizeResponseResultsItem(pydantic.BaseModel):
-    id: typing.Optional[str] = pydantic.Field(description=("Generated ID for the summary\n"))
-    summary: typing.Optional[str] = pydantic.Field(description=("Generated summary for the text\n"))
+class GenerationStream(pydantic.BaseModel):
+    text: str = pydantic.Field(description="A segment of text of the generation.")
+    index: typing.Optional[int] = pydantic.Field(
+        description="Refers to the nth generation. Only present when `num_generations` is greater than zero."
+    )
+    is_finished: bool
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_cohere-0.0.3/src/cohere/types/tokenize_response.py` & `fern_cohere-0.0.4/src/cohere/types/rerank_response_results_item.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,21 +2,23 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .tokenize_response_meta_item import TokenizeResponseMetaItem
+from .rerank_response_results_item_document import RerankResponseResultsItemDocument
 
 
-class TokenizeResponse(pydantic.BaseModel):
-    tokens: typing.List[int] = pydantic.Field(description=("An array of tokens, where each token is an integer.\n"))
-    token_strings: typing.List[str]
-    meta: typing.Optional[typing.List[TokenizeResponseMetaItem]]
+class RerankResponseResultsItem(pydantic.BaseModel):
+    document: typing.Optional[RerankResponseResultsItemDocument] = pydantic.Field(
+        description="The doc object which was ranked"
+    )
+    index: int = pydantic.Field(description="The index of the input document")
+    relevance_score: float = pydantic.Field(description="A relevance score assigned to the ranking")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `fern_cohere-0.0.3/src/cohere/types/tokenize_response_meta_item.py` & `fern_cohere-0.0.4/src/cohere/types/detect_language_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,20 +2,23 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ..core.datetime_utils import serialize_datetime
-from .tokenize_response_meta_item_api_version_item import TokenizeResponseMetaItemApiVersionItem
+from .detect_language_response_meta_item import DetectLanguageResponseMetaItem
+from .detect_language_response_results_item import DetectLanguageResponseResultsItem
 
 
-class TokenizeResponseMetaItem(pydantic.BaseModel):
-    api_version: typing.Optional[typing.List[TokenizeResponseMetaItemApiVersionItem]]
-    warnings: typing.Optional[typing.List[str]]
+class DetectLanguageResponse(pydantic.BaseModel):
+    results: typing.Optional[typing.List[DetectLanguageResponseResultsItem]] = pydantic.Field(
+        description="List of languages, one per input text"
+    )
+    meta: typing.Optional[typing.List[DetectLanguageResponseMetaItem]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

