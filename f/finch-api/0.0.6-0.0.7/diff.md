# Comparing `tmp/finch_api-0.0.6.tar.gz` & `tmp/finch_api-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finch_api-0.0.6.tar", max compression
+gzip compressed data, was "finch_api-0.0.7.tar", max compression
```

## Comparing `finch_api-0.0.6.tar` & `finch_api-0.0.7.tar`

### file list

```diff
@@ -1,94 +1,94 @@
--rw-r--r--   0        0        0    11335 2023-07-22 01:36:26.371955 finch_api-0.0.6/LICENSE
--rw-r--r--   0        0        0     7481 2023-07-22 01:36:26.371955 finch_api-0.0.6/README.md
--rw-r--r--   0        0        0     1891 2023-07-22 01:36:26.371955 finch_api-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1834 2023-07-22 01:36:26.371955 finch_api-0.0.6/src/finch/__init__.py
--rw-r--r--   0        0        0    46805 2023-07-22 01:36:26.371955 finch_api-0.0.6/src/finch/_base_client.py
--rw-r--r--   0        0        0     3889 2023-07-22 01:36:26.371955 finch_api-0.0.6/src/finch/_base_exceptions.py
--rw-r--r--   0        0        0    17881 2023-07-22 01:36:26.371955 finch_api-0.0.6/src/finch/_client.py
--rw-r--r--   0        0        0     1285 2023-07-22 01:36:26.371955 finch_api-0.0.6/src/finch/_exceptions.py
--rw-r--r--   0        0        0     7343 2023-07-22 01:36:26.371955 finch_api-0.0.6/src/finch/_models.py
--rw-r--r--   0        0        0     4846 2023-07-22 01:36:26.371955 finch_api-0.0.6/src/finch/_qs.py
--rw-r--r--   0        0        0      872 2023-07-22 01:36:26.371955 finch_api-0.0.6/src/finch/_resource.py
--rw-r--r--   0        0        0     5884 2023-07-22 01:36:26.371955 finch_api-0.0.6/src/finch/_streaming.py
--rw-r--r--   0        0        0     4226 2023-07-22 01:36:26.371955 finch_api-0.0.6/src/finch/_types.py
--rw-r--r--   0        0        0     1277 2023-07-22 01:36:26.371955 finch_api-0.0.6/src/finch/_utils/__init__.py
--rw-r--r--   0        0        0     6710 2023-07-22 01:36:26.371955 finch_api-0.0.6/src/finch/_utils/_transform.py
--rw-r--r--   0        0        0     9411 2023-07-22 01:36:26.371955 finch_api-0.0.6/src/finch/_utils/_utils.py
--rw-r--r--   0        0        0      124 2023-07-22 01:36:26.371955 finch_api-0.0.6/src/finch/_version.py
--rw-r--r--   0        0        0    10630 2023-07-22 01:36:26.371955 finch_api-0.0.6/src/finch/pagination.py
--rw-r--r--   0        0        0        0 2023-07-22 01:36:26.371955 finch_api-0.0.6/src/finch/py.typed
--rw-r--r--   0        0        0      321 2023-07-22 01:36:26.371955 finch_api-0.0.6/src/finch/resources/__init__.py
--rw-r--r--   0        0        0     4144 2023-07-22 01:36:26.371955 finch_api-0.0.6/src/finch/resources/account.py
--rw-r--r--   0        0        0      532 2023-07-22 01:36:26.371955 finch_api-0.0.6/src/finch/resources/ats/__init__.py
--rw-r--r--   0        0        0     6374 2023-07-22 01:36:26.371955 finch_api-0.0.6/src/finch/resources/ats/applications.py
--rw-r--r--   0        0        0     1409 2023-07-22 01:36:26.371955 finch_api-0.0.6/src/finch/resources/ats/ats.py
--rw-r--r--   0        0        0     6638 2023-07-22 01:36:26.371955 finch_api-0.0.6/src/finch/resources/ats/candidates.py
--rw-r--r--   0        0        0     6044 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/resources/ats/jobs.py
--rw-r--r--   0        0        0     6148 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/resources/ats/offers.py
--rw-r--r--   0        0        0     2703 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/resources/ats/stages.py
--rw-r--r--   0        0        0      703 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/resources/hris/__init__.py
--rw-r--r--   0        0        0      231 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/resources/hris/benefits/__init__.py
--rw-r--r--   0        0        0    14280 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/resources/hris/benefits/benefits.py
--rw-r--r--   0        0        0    14347 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/resources/hris/benefits/individuals.py
--rw-r--r--   0        0        0     2021 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/resources/hris/company.py
--rw-r--r--   0        0        0     4175 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/resources/hris/directory.py
--rw-r--r--   0        0        0     1760 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/resources/hris/hris.py
--rw-r--r--   0        0        0      262 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/resources/hris/individuals/__init__.py
--rw-r--r--   0        0        0     4278 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/resources/hris/individuals/employment_data.py
--rw-r--r--   0        0        0     4552 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/resources/hris/individuals/individuals.py
--rw-r--r--   0        0        0     3963 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/resources/hris/pay_statements.py
--rw-r--r--   0        0        0     4247 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/resources/hris/payments.py
--rw-r--r--   0        0        0     2256 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/resources/providers.py
--rw-r--r--   0        0        0      416 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/__init__.py
--rw-r--r--   0        0        0      572 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/ats/__init__.py
--rw-r--r--   0        0        0      512 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/ats/application.py
--rw-r--r--   0        0        0      361 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/ats/application_list_params.py
--rw-r--r--   0        0        0      726 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/ats/candidate.py
--rw-r--r--   0        0        0      355 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/ats/candidate_list_params.py
--rw-r--r--   0        0        0      889 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/ats/job.py
--rw-r--r--   0        0        0      337 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/ats/job_list_params.py
--rw-r--r--   0        0        0      474 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/ats/offer.py
--rw-r--r--   0        0        0      343 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/ats/offer_list_params.py
--rw-r--r--   0        0        0      362 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/ats/stage.py
--rw-r--r--   0        0        0      266 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/disconnect_response.py
--rw-r--r--   0        0        0     1761 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/hris/__init__.py
--rw-r--r--   0        0        0      902 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/hris/benefit_create_params.py
--rw-r--r--   0        0        0      220 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/hris/benefit_frequency.py
--rw-r--r--   0        0        0      598 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/hris/benefit_type.py
--rw-r--r--   0        0        0      278 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/hris/benefit_update_params.py
--rw-r--r--   0        0        0      784 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/hris/benefits/__init__.py
--rw-r--r--   0        0        0      723 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/hris/benefits/enrolled_individual.py
--rw-r--r--   0        0        0      969 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/hris/benefits/individual_benefit.py
--rw-r--r--   0        0        0      550 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/hris/benefits/individual_enroll_many_params.py
--rw-r--r--   0        0        0      259 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/hris/benefits/individual_enrolled_ids_response.py
--rw-r--r--   0        0        0      398 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/hris/benefits/individual_retrieve_many_benefits_params.py
--rw-r--r--   0        0        0      329 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/hris/benefits/individual_unenroll_params.py
--rw-r--r--   0        0        0      647 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/hris/benefits/unenrolled_individual.py
--rw-r--r--   0        0        0      415 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/hris/benfit_contribution.py
--rw-r--r--   0        0        0     2209 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/hris/company.py
--rw-r--r--   0        0        0      596 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/hris/company_benefit.py
--rw-r--r--   0        0        0      202 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/hris/create_company_benefits_response.py
--rw-r--r--   0        0        0      376 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/hris/directory_list_individuals_params.py
--rw-r--r--   0        0        0     1361 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/hris/individual.py
--rw-r--r--   0        0        0     1025 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/hris/individual_in_directory.py
--rw-r--r--   0        0        0      327 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/hris/individual_response.py
--rw-r--r--   0        0        0      480 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/hris/individual_retrieve_many_params.py
--rw-r--r--   0        0        0      367 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/hris/individuals/__init__.py
--rw-r--r--   0        0        0     2985 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/hris/individuals/employment_data.py
--rw-r--r--   0        0        0      363 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/hris/individuals/employment_data_response.py
--rw-r--r--   0        0        0      703 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/hris/individuals/employment_data_retrieve_many_params.py
--rw-r--r--   0        0        0     3320 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/hris/pay_statement.py
--rw-r--r--   0        0        0      376 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/hris/pay_statement_response.py
--rw-r--r--   0        0        0      438 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/hris/pay_statement_response_body.py
--rw-r--r--   0        0        0      616 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/hris/pay_statement_retrieve_many_params.py
--rw-r--r--   0        0        0      791 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/hris/payment.py
--rw-r--r--   0        0        0      709 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/hris/payment_list_params.py
--rw-r--r--   0        0        0     1411 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/hris/supported_benefit.py
--rw-r--r--   0        0        0      200 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/hris/update_company_benefit_response.py
--rw-r--r--   0        0        0      724 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/income.py
--rw-r--r--   0        0        0      881 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/introspection.py
--rw-r--r--   0        0        0      631 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/location.py
--rw-r--r--   0        0        0      262 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/money.py
--rw-r--r--   0        0        0      369 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/paging.py
--rw-r--r--   0        0        0      959 2023-07-22 01:36:26.375955 finch_api-0.0.6/src/finch/types/provider.py
--rw-r--r--   0        0        0     8398 1970-01-01 00:00:00.000000 finch_api-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    11335 2023-08-01 11:57:21.627799 finch_api-0.0.7/LICENSE
+-rw-r--r--   0        0        0     7851 2023-08-01 11:57:21.627799 finch_api-0.0.7/README.md
+-rw-r--r--   0        0        0     1891 2023-08-01 11:57:21.627799 finch_api-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1834 2023-08-01 11:57:21.627799 finch_api-0.0.7/src/finch/__init__.py
+-rw-r--r--   0        0        0    47774 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/_base_client.py
+-rw-r--r--   0        0        0     3889 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/_base_exceptions.py
+-rw-r--r--   0        0        0    18102 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/_client.py
+-rw-r--r--   0        0        0     1285 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/_exceptions.py
+-rw-r--r--   0        0        0     7343 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/_models.py
+-rw-r--r--   0        0        0     4846 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/_qs.py
+-rw-r--r--   0        0        0      872 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/_resource.py
+-rw-r--r--   0        0        0     5884 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/_streaming.py
+-rw-r--r--   0        0        0     4226 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/_types.py
+-rw-r--r--   0        0        0     1277 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/_utils/__init__.py
+-rw-r--r--   0        0        0     6710 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/_utils/_transform.py
+-rw-r--r--   0        0        0     9411 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/_utils/_utils.py
+-rw-r--r--   0        0        0      124 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/_version.py
+-rw-r--r--   0        0        0    10704 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/pagination.py
+-rw-r--r--   0        0        0        0 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/py.typed
+-rw-r--r--   0        0        0      321 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/resources/__init__.py
+-rw-r--r--   0        0        0     4144 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/resources/account.py
+-rw-r--r--   0        0        0      532 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/resources/ats/__init__.py
+-rw-r--r--   0        0        0     6374 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/resources/ats/applications.py
+-rw-r--r--   0        0        0     1409 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/resources/ats/ats.py
+-rw-r--r--   0        0        0     6638 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/resources/ats/candidates.py
+-rw-r--r--   0        0        0     6044 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/resources/ats/jobs.py
+-rw-r--r--   0        0        0     6148 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/resources/ats/offers.py
+-rw-r--r--   0        0        0     2703 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/resources/ats/stages.py
+-rw-r--r--   0        0        0      703 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/resources/hris/__init__.py
+-rw-r--r--   0        0        0      231 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/resources/hris/benefits/__init__.py
+-rw-r--r--   0        0        0    14280 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/resources/hris/benefits/benefits.py
+-rw-r--r--   0        0        0    14347 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/resources/hris/benefits/individuals.py
+-rw-r--r--   0        0        0     2021 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/resources/hris/company.py
+-rw-r--r--   0        0        0     4175 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/resources/hris/directory.py
+-rw-r--r--   0        0        0     1760 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/resources/hris/hris.py
+-rw-r--r--   0        0        0      262 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/resources/hris/individuals/__init__.py
+-rw-r--r--   0        0        0     4278 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/resources/hris/individuals/employment_data.py
+-rw-r--r--   0        0        0     4552 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/resources/hris/individuals/individuals.py
+-rw-r--r--   0        0        0     3963 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/resources/hris/pay_statements.py
+-rw-r--r--   0        0        0     4247 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/resources/hris/payments.py
+-rw-r--r--   0        0        0     2256 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/resources/providers.py
+-rw-r--r--   0        0        0      416 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/__init__.py
+-rw-r--r--   0        0        0      572 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/ats/__init__.py
+-rw-r--r--   0        0        0      512 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/ats/application.py
+-rw-r--r--   0        0        0      361 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/ats/application_list_params.py
+-rw-r--r--   0        0        0      726 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/ats/candidate.py
+-rw-r--r--   0        0        0      355 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/ats/candidate_list_params.py
+-rw-r--r--   0        0        0      889 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/ats/job.py
+-rw-r--r--   0        0        0      337 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/ats/job_list_params.py
+-rw-r--r--   0        0        0      474 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/ats/offer.py
+-rw-r--r--   0        0        0      343 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/ats/offer_list_params.py
+-rw-r--r--   0        0        0      362 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/ats/stage.py
+-rw-r--r--   0        0        0      266 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/disconnect_response.py
+-rw-r--r--   0        0        0     1761 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/hris/__init__.py
+-rw-r--r--   0        0        0      902 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/hris/benefit_create_params.py
+-rw-r--r--   0        0        0      220 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/hris/benefit_frequency.py
+-rw-r--r--   0        0        0      598 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/hris/benefit_type.py
+-rw-r--r--   0        0        0      278 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/hris/benefit_update_params.py
+-rw-r--r--   0        0        0      784 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/hris/benefits/__init__.py
+-rw-r--r--   0        0        0      723 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/hris/benefits/enrolled_individual.py
+-rw-r--r--   0        0        0      969 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/hris/benefits/individual_benefit.py
+-rw-r--r--   0        0        0      550 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/hris/benefits/individual_enroll_many_params.py
+-rw-r--r--   0        0        0      259 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/hris/benefits/individual_enrolled_ids_response.py
+-rw-r--r--   0        0        0      398 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/hris/benefits/individual_retrieve_many_benefits_params.py
+-rw-r--r--   0        0        0      329 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/hris/benefits/individual_unenroll_params.py
+-rw-r--r--   0        0        0      647 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/hris/benefits/unenrolled_individual.py
+-rw-r--r--   0        0        0      415 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/hris/benfit_contribution.py
+-rw-r--r--   0        0        0     2209 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/hris/company.py
+-rw-r--r--   0        0        0      596 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/hris/company_benefit.py
+-rw-r--r--   0        0        0      202 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/hris/create_company_benefits_response.py
+-rw-r--r--   0        0        0      376 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/hris/directory_list_individuals_params.py
+-rw-r--r--   0        0        0     1361 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/hris/individual.py
+-rw-r--r--   0        0        0     1025 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/hris/individual_in_directory.py
+-rw-r--r--   0        0        0      327 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/hris/individual_response.py
+-rw-r--r--   0        0        0      480 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/hris/individual_retrieve_many_params.py
+-rw-r--r--   0        0        0      367 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/hris/individuals/__init__.py
+-rw-r--r--   0        0        0     2985 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/hris/individuals/employment_data.py
+-rw-r--r--   0        0        0      363 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/hris/individuals/employment_data_response.py
+-rw-r--r--   0        0        0      703 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/hris/individuals/employment_data_retrieve_many_params.py
+-rw-r--r--   0        0        0     3320 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/hris/pay_statement.py
+-rw-r--r--   0        0        0      376 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/hris/pay_statement_response.py
+-rw-r--r--   0        0        0      438 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/hris/pay_statement_response_body.py
+-rw-r--r--   0        0        0      616 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/hris/pay_statement_retrieve_many_params.py
+-rw-r--r--   0        0        0      791 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/hris/payment.py
+-rw-r--r--   0        0        0      709 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/hris/payment_list_params.py
+-rw-r--r--   0        0        0     1411 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/hris/supported_benefit.py
+-rw-r--r--   0        0        0      200 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/hris/update_company_benefit_response.py
+-rw-r--r--   0        0        0      724 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/income.py
+-rw-r--r--   0        0        0      881 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/introspection.py
+-rw-r--r--   0        0        0      631 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/location.py
+-rw-r--r--   0        0        0      262 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/money.py
+-rw-r--r--   0        0        0      369 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/paging.py
+-rw-r--r--   0        0        0      959 2023-08-01 11:57:21.631799 finch_api-0.0.7/src/finch/types/provider.py
+-rw-r--r--   0        0        0     8768 1970-01-01 00:00:00.000000 finch_api-0.0.7/PKG-INFO
```

### Comparing `finch_api-0.0.6/LICENSE` & `finch_api-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/README.md` & `finch_api-0.0.7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -17,38 +17,38 @@
 ```
 
 ## Usage
 
 ```python
 from finch import Finch
 
-finch = Finch(
+client = Finch(
     access_token="my access token",
 )
 
-candidate = finch.ats.candidates.retrieve(
+candidate = client.ats.candidates.retrieve(
     "<candidate id>",
 )
 print(candidate.first_name)
 ```
 
 ## Async Usage
 
 Simply import `AsyncFinch` instead of `Finch` and use `await` with each API call:
 
 ```python
 from finch import AsyncFinch
 
-finch = AsyncFinch(
+client = AsyncFinch(
     access_token="my access token",
 )
 
 
 async def main():
-    candidate = await finch.ats.candidates.retrieve(
+    candidate = await client.ats.candidates.retrieve(
         "<candidate id>",
     )
     print(candidate.first_name)
 
 
 asyncio.run(main())
 ```
@@ -66,60 +66,60 @@
 List methods in the Finch API are paginated.
 
 This library provides auto-paginating iterators with each list response, so you do not have to request successive pages manually:
 
 ```python
 import finch
 
-finch = Finch()
+client = Finch()
 
 all_jobs = []
 # Automatically fetches more pages as needed.
-for job in finch.ats.jobs.list():
+for job in client.ats.jobs.list():
     # Do something with job here
     all_jobs.append(job)
 print(all_jobs)
 ```
 
 Or, asynchronously:
 
 ```python
 import asyncio
 import finch
 
-finch = AsyncFinch()
+client = AsyncFinch()
 
 
 async def main() -> None:
     all_jobs = []
     # Iterate through items across all pages, issuing requests as needed.
-    async for job in finch.ats.jobs.list():
+    async for job in client.ats.jobs.list():
         all_jobs.append(job)
     print(all_jobs)
 
 
 asyncio.run(main())
 ```
 
 Alternatively, you can use the `.has_next_page()`, `.next_page_info()`, or `.get_next_page()` methods for more granular control working with pages:
 
 ```python
-first_page = await finch.ats.jobs.list()
+first_page = await client.ats.jobs.list()
 if first_page.has_next_page():
     print(f"will fetch next page using these details: {first_page.next_page_info()}")
     next_page = await first_page.get_next_page()
     print(f"number of items we just fetched: {len(next_page.jobs)}")
 
 # Remove `await` for non-async usage.
 ```
 
 Or just work directly with the returned data:
 
 ```python
-first_page = await finch.ats.jobs.list()
+first_page = await client.ats.jobs.list()
 
 print(
     f"the current start offset for this page: {first_page.paging.offset}"
 )  # => "the current start offset for this page: 1"
 for job in first_page.jobs:
     print(job.id)
 
@@ -129,17 +129,17 @@
 ## Nested params
 
 Nested parameters are dictionaries, typed using `TypedDict`, for example:
 
 ```python
 from finch import Finch
 
-finch = Finch()
+client = Finch()
 
-finch.hris.directory.list_individuals(
+client.hris.directory.list_individuals(
     path_params=[],
     params={},
 )
 ```
 
 ## Handling errors
 
@@ -190,44 +190,44 @@
 
 You can use the `max_retries` option to configure or disable this:
 
 ```python
 from finch import Finch
 
 # Configure the default for all requests:
-finch = Finch(
+client = Finch(
     # default is 2
     max_retries=0,
 )
 
 # Or, configure per-request:
-finch.with_options(max_retries=5).hris.directory.list_individuals()
+client.with_options(max_retries=5).hris.directory.list_individuals()
 ```
 
 ### Timeouts
 
 Requests time out after 60 seconds by default. You can configure this with a `timeout` option,
 which accepts a float or an [`httpx.Timeout`](https://www.python-httpx.org/advanced/#fine-tuning-the-configuration):
 
 ```python
 from finch import Finch
 
 # Configure the default for all requests:
-finch = Finch(
+client = Finch(
     # default is 60s
     timeout=20.0,
 )
 
 # More granular control:
-finch = Finch(
+client = Finch(
     timeout=httpx.Timeout(60.0, read=5.0, write=10.0, connect=2.0),
 )
 
 # Override per-request:
-finch.with_options(timeout=5 * 1000).hris.directory.list_individuals()
+client.with_options(timeout=5 * 1000).hris.directory.list_individuals()
 ```
 
 On timeout, an `APITimeoutError` is thrown.
 
 Note that requests which time out will be [retried twice by default](#retries).
 
 ## Default Headers
@@ -237,37 +237,41 @@
 If you need to, you can override it by setting default headers per-request or on the client object.
 
 Be aware that doing so may result in incorrect types and other unexpected or undefined behavior in the SDK.
 
 ```python
 from finch import Finch
 
-finch = Finch(
+client = Finch(
     default_headers={"Finch-API-Version": "My-Custom-Value"},
 )
 ```
 
 ## Advanced: Configuring custom URLs, proxies, and transports
 
 You can configure the following keyword arguments when instantiating the client:
 
 ```python
 import httpx
 from finch import Finch
 
-finch = Finch(
+client = Finch(
     # Use a custom base URL
     base_url="http://my.test.server.example.com:8083",
     proxies="http://my.test.proxy.example.com",
     transport=httpx.HTTPTransport(local_address="0.0.0.0"),
 )
 ```
 
 See the httpx documentation for information about the [`proxies`](https://www.python-httpx.org/advanced/#http-proxying) and [`transport`](https://www.python-httpx.org/advanced/#custom-transports) keyword arguments.
 
+## Advanced: Managing HTTP resources
+
+By default we will close the underlying HTTP connections whenever the client is [garbage collected](https://docs.python.org/3/reference/datamodel.html#object.__del__) is called but you can also manually close the client using the `.close()` method if desired, or with a context manager that closes when exiting.
+
 ## Status
 
 This package is in beta. Its internals and interfaces are not stable and subject to change without a major semver bump;
 please reach out if you rely on any undocumented behavior.
 
 We are keen for your feedback; please open an [issue](https://www.github.com/Finch-API/finch-api-python/issues) with questions, bugs, or suggestions.
```

### Comparing `finch_api-0.0.6/pyproject.toml` & `finch_api-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "finch-api"
-version = "0.0.6"
+version = "0.0.7"
 description = "Client library for the Finch API"
 readme = "README.md"
 authors = ["Finch <founders@tryfinch.com>"]
 license = "Apache-2.0"
 repository = "https://github.com/Finch-API/finch-api-python"
 packages = [
   { include = "finch", from = "src" }
@@ -16,15 +16,15 @@
 pydantic = "^1.9.0"
 typing-extensions = ">= 4.1.1, < 5"
 anyio = ">= 3.5.0, < 4"
 distro = ">= 1.7.0, < 2"
 
 
 [tool.poetry.group.dev.dependencies]
-pyright = "1.1.297"
+pyright = "1.1.318"
 mypy = "1.1.1"
 black = "22.10.0"
 respx = "0.19.2"
 pytest = "7.1.1"
 pytest-asyncio = "0.18.3"
 ruff = "0.0.239"
 isort = "5.10.1"
```

### Comparing `finch_api-0.0.6/src/finch/__init__.py` & `finch_api-0.0.7/src/finch/__init__.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/_base_client.py` & `finch_api-0.0.7/src/finch/_base_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import json
 import time
 import uuid
 import inspect
 import platform
+from types import TracebackType
 from random import random
 from typing import (
     Any,
     Dict,
     Type,
     Union,
     Generic,
@@ -673,14 +674,35 @@
             timeout=timeout,
             proxies=proxies,  # type: ignore
             transport=transport,  # type: ignore
             limits=limits,
             headers={"Accept": "application/json"},
         )
 
+    def is_closed(self) -> bool:
+        return self._client.is_closed
+
+    def close(self) -> None:
+        """Close the underlying HTTPX client.
+
+        The client will *not* be usable after this.
+        """
+        self._client.close()
+
+    def __enter__(self: _T) -> _T:
+        return self
+
+    def __exit__(
+        self,
+        exc_type: type[BaseException] | None,
+        exc: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> None:
+        self.close()
+
     @overload
     def request(
         self,
         cast_to: Type[ResponseT],
         options: FinalRequestOptions,
         remaining_retries: Optional[int] = None,
         *,
@@ -808,15 +830,15 @@
 
     def _request_api_list(
         self,
         model: Type[ModelT],
         page: Type[SyncPageT],
         options: FinalRequestOptions,
     ) -> SyncPageT:
-        resp = cast(SyncPageT, self.request(page, options, stream=False))
+        resp = self.request(page, options, stream=False)
         resp._set_private_attributes(  # pyright: ignore[reportPrivateUsage]
             client=self,
             model=model,
             options=options,
         )
         return resp
 
@@ -929,38 +951,38 @@
         path: str,
         *,
         cast_to: Type[ResponseT],
         body: Body | None = None,
         options: RequestOptions = {},
     ) -> ResponseT:
         opts = FinalRequestOptions.construct(method="patch", url=path, json_data=body, **options)
-        return cast(ResponseT, self.request(cast_to, opts))
+        return self.request(cast_to, opts)
 
     def put(
         self,
         path: str,
         *,
         cast_to: Type[ResponseT],
         body: Body | None = None,
         files: RequestFiles | None = None,
         options: RequestOptions = {},
     ) -> ResponseT:
         opts = FinalRequestOptions.construct(method="put", url=path, json_data=body, files=files, **options)
-        return cast(ResponseT, self.request(cast_to, opts))
+        return self.request(cast_to, opts)
 
     def delete(
         self,
         path: str,
         *,
         cast_to: Type[ResponseT],
         body: Body | None = None,
         options: RequestOptions = {},
     ) -> ResponseT:
         opts = FinalRequestOptions.construct(method="delete", url=path, json_data=body, **options)
-        return cast(ResponseT, self.request(cast_to, opts))
+        return self.request(cast_to, opts)
 
     def get_api_list(
         self,
         path: str,
         *,
         model: Type[ModelT],
         page: Type[SyncPageT],
@@ -1005,14 +1027,35 @@
             timeout=timeout,
             proxies=proxies,  # type: ignore
             transport=transport,  # type: ignore
             limits=limits,
             headers={"Accept": "application/json"},
         )
 
+    def is_closed(self) -> bool:
+        return self._client.is_closed
+
+    async def close(self) -> None:
+        """Close the underlying HTTPX client.
+
+        The client will *not* be usable after this.
+        """
+        await self._client.aclose()
+
+    async def __aenter__(self: _T) -> _T:
+        return self
+
+    async def __aexit__(
+        self,
+        exc_type: type[BaseException] | None,
+        exc: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> None:
+        await self.close()
+
     @overload
     async def request(
         self,
         cast_to: Type[ResponseT],
         options: FinalRequestOptions,
         *,
         stream: Literal[False] = False,
```

### Comparing `finch_api-0.0.6/src/finch/_base_exceptions.py` & `finch_api-0.0.7/src/finch/_base_exceptions.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/_client.py` & `finch_api-0.0.7/src/finch/_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
 import os
+import asyncio
 from typing import Union, Mapping, Optional
 
 import httpx
 
 from . import resources
 from ._qs import Querystring
 from ._types import (
@@ -83,39 +84,38 @@
     ) -> None:
         """Construct a new synchronous Finch client instance.
 
         This automatically infers the following arguments from their corresponding environment variables if they are not provided:
         - `client_id` from `FINCH_CLIENT_ID`
         - `client_secret` from `FINCH_CLIENT_SECRET`
         """
+        self.access_token = access_token
+
+        client_id_envvar = os.environ.get("FINCH_CLIENT_ID", None)
+        self.client_id = client_id or client_id_envvar or None
+
+        client_secret_envvar = os.environ.get("FINCH_CLIENT_SECRET", None)
+        self.client_secret = client_secret or client_secret_envvar or None
 
         if base_url is None:
-            base_url = "https://api.tryfinch.com"
+            base_url = f"https://api.tryfinch.com"
 
         super().__init__(
             version=__version__,
             base_url=base_url,
             max_retries=max_retries,
             timeout=timeout,
             transport=transport,
             proxies=proxies,
             limits=connection_pool_limits,
             custom_headers=default_headers,
             custom_query=default_query,
             _strict_response_validation=_strict_response_validation,
         )
 
-        self.access_token = access_token
-
-        client_id_envvar = os.environ.get("FINCH_CLIENT_ID", None)
-        self.client_id = client_id or client_id_envvar or None
-
-        client_secret_envvar = os.environ.get("FINCH_CLIENT_SECRET", None)
-        self.client_secret = client_secret or client_secret_envvar or None
-
         self.ats = resources.ATS(self)
         self.hris = resources.HRIS(self)
         self.providers = resources.Providers(self)
         self.account = resources.Account(self)
 
     @property
     def qs(self) -> Querystring:
@@ -200,14 +200,17 @@
             default_query=params,
         )
 
     # Alias for `copy` for nicer inline usage, e.g.
     # client.with_options(timeout=10).foo.create(...)
     with_options = copy
 
+    def __del__(self) -> None:
+        self.close()
+
     def get_access_token(
         self,
         code: str,
         *,
         redirect_uri: str,
     ) -> str:
         """Returns an access token for the Finch API given an authorization code.
@@ -304,39 +307,38 @@
     ) -> None:
         """Construct a new async Finch client instance.
 
         This automatically infers the following arguments from their corresponding environment variables if they are not provided:
         - `client_id` from `FINCH_CLIENT_ID`
         - `client_secret` from `FINCH_CLIENT_SECRET`
         """
+        self.access_token = access_token
+
+        client_id_envvar = os.environ.get("FINCH_CLIENT_ID", None)
+        self.client_id = client_id or client_id_envvar or None
+
+        client_secret_envvar = os.environ.get("FINCH_CLIENT_SECRET", None)
+        self.client_secret = client_secret or client_secret_envvar or None
 
         if base_url is None:
-            base_url = "https://api.tryfinch.com"
+            base_url = f"https://api.tryfinch.com"
 
         super().__init__(
             version=__version__,
             base_url=base_url,
             max_retries=max_retries,
             timeout=timeout,
             transport=transport,
             proxies=proxies,
             limits=connection_pool_limits,
             custom_headers=default_headers,
             custom_query=default_query,
             _strict_response_validation=_strict_response_validation,
         )
 
-        self.access_token = access_token
-
-        client_id_envvar = os.environ.get("FINCH_CLIENT_ID", None)
-        self.client_id = client_id or client_id_envvar or None
-
-        client_secret_envvar = os.environ.get("FINCH_CLIENT_SECRET", None)
-        self.client_secret = client_secret or client_secret_envvar or None
-
         self.ats = resources.AsyncATS(self)
         self.hris = resources.AsyncHRIS(self)
         self.providers = resources.AsyncProviders(self)
         self.account = resources.AsyncAccount(self)
 
     @property
     def qs(self) -> Querystring:
@@ -421,14 +423,20 @@
             default_query=params,
         )
 
     # Alias for `copy` for nicer inline usage, e.g.
     # client.with_options(timeout=10).foo.create(...)
     with_options = copy
 
+    def __del__(self) -> None:
+        try:
+            asyncio.get_running_loop().create_task(self.close())
+        except Exception:
+            pass
+
     async def get_access_token(
         self,
         code: str,
         *,
         redirect_uri: str,
     ) -> str:
         """Returns an access token for the Finch API given an authorization code.
```

### Comparing `finch_api-0.0.6/src/finch/_exceptions.py` & `finch_api-0.0.7/src/finch/_exceptions.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/_models.py` & `finch_api-0.0.7/src/finch/_models.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/_qs.py` & `finch_api-0.0.7/src/finch/_qs.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/_resource.py` & `finch_api-0.0.7/src/finch/_resource.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/_streaming.py` & `finch_api-0.0.7/src/finch/_streaming.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/_types.py` & `finch_api-0.0.7/src/finch/_types.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/_utils/__init__.py` & `finch_api-0.0.7/src/finch/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/_utils/_transform.py` & `finch_api-0.0.7/src/finch/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/_utils/_utils.py` & `finch_api-0.0.7/src/finch/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/pagination.py` & `finch_api-0.0.7/src/finch/pagination.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # File generated from our OpenAPI spec by Stainless.
 
-from typing import List, Type, Generic, Mapping, TypeVar, Optional
+from typing import Any, List, Type, Generic, Mapping, TypeVar, Optional, cast
 
 from httpx import Response
 
 from ._types import ModelT
+from ._utils import is_mapping
 from ._models import BaseModel
 from ._base_client import BasePage, PageInfo, BaseSyncPage, BaseAsyncPage
 
 __all__ = [
     "SyncSinglePage",
     "AsyncSinglePage",
     "SyncResponsesPage",
@@ -41,15 +42,15 @@
         """
         return None
 
     @classmethod
     def build(cls: Type[_BaseModelT], *, response: Response, data: object) -> _BaseModelT:
         return cls.construct(
             **{
-                **(data if isinstance(data, Mapping) else {"items": data}),
+                **(cast(Mapping[str, Any], data) if is_mapping(data) else {"items": data}),
             }
         )
 
 
 class AsyncSinglePage(BaseAsyncPage[ModelT], BasePage[ModelT], Generic[ModelT]):
     items: List[ModelT]
 
@@ -63,15 +64,15 @@
         """
         return None
 
     @classmethod
     def build(cls: Type[_BaseModelT], *, response: Response, data: object) -> _BaseModelT:
         return cls.construct(
             **{
-                **(data if isinstance(data, Mapping) else {"items": data}),
+                **(cast(Mapping[str, Any], data) if is_mapping(data) else {"items": data}),
             }
         )
 
 
 class SyncResponsesPage(BaseSyncPage[ModelT], BasePage[ModelT], Generic[ModelT]):
     responses: List[ModelT]
```

### Comparing `finch_api-0.0.6/src/finch/resources/account.py` & `finch_api-0.0.7/src/finch/resources/account.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/resources/ats/__init__.py` & `finch_api-0.0.7/src/finch/resources/ats/__init__.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/resources/ats/applications.py` & `finch_api-0.0.7/src/finch/resources/ats/applications.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/resources/ats/ats.py` & `finch_api-0.0.7/src/finch/resources/ats/ats.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/resources/ats/candidates.py` & `finch_api-0.0.7/src/finch/resources/ats/candidates.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/resources/ats/jobs.py` & `finch_api-0.0.7/src/finch/resources/ats/jobs.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/resources/ats/offers.py` & `finch_api-0.0.7/src/finch/resources/ats/offers.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/resources/ats/stages.py` & `finch_api-0.0.7/src/finch/resources/ats/stages.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/resources/hris/__init__.py` & `finch_api-0.0.7/src/finch/resources/hris/__init__.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/resources/hris/benefits/benefits.py` & `finch_api-0.0.7/src/finch/resources/hris/benefits/benefits.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/resources/hris/benefits/individuals.py` & `finch_api-0.0.7/src/finch/resources/hris/benefits/individuals.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/resources/hris/company.py` & `finch_api-0.0.7/src/finch/resources/hris/company.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/resources/hris/directory.py` & `finch_api-0.0.7/src/finch/resources/hris/directory.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/resources/hris/hris.py` & `finch_api-0.0.7/src/finch/resources/hris/hris.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/resources/hris/individuals/employment_data.py` & `finch_api-0.0.7/src/finch/resources/hris/individuals/employment_data.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/resources/hris/individuals/individuals.py` & `finch_api-0.0.7/src/finch/resources/hris/individuals/individuals.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/resources/hris/pay_statements.py` & `finch_api-0.0.7/src/finch/resources/hris/pay_statements.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/resources/hris/payments.py` & `finch_api-0.0.7/src/finch/resources/hris/payments.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/resources/providers.py` & `finch_api-0.0.7/src/finch/resources/providers.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/types/ats/__init__.py` & `finch_api-0.0.7/src/finch/types/ats/__init__.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/types/ats/application.py` & `finch_api-0.0.7/src/finch/types/ats/application.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/types/ats/candidate.py` & `finch_api-0.0.7/src/finch/types/ats/candidate.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/types/ats/job.py` & `finch_api-0.0.7/src/finch/types/ats/job.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/types/hris/__init__.py` & `finch_api-0.0.7/src/finch/types/hris/__init__.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/types/hris/benefit_create_params.py` & `finch_api-0.0.7/src/finch/types/hris/benefit_create_params.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/types/hris/benefit_type.py` & `finch_api-0.0.7/src/finch/types/hris/benefit_type.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/types/hris/benefits/__init__.py` & `finch_api-0.0.7/src/finch/types/hris/benefits/__init__.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/types/hris/benefits/enrolled_individual.py` & `finch_api-0.0.7/src/finch/types/hris/benefits/enrolled_individual.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/types/hris/benefits/individual_benefit.py` & `finch_api-0.0.7/src/finch/types/hris/benefits/individual_benefit.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/types/hris/benefits/individual_enroll_many_params.py` & `finch_api-0.0.7/src/finch/types/hris/benefits/individual_enroll_many_params.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/types/hris/benefits/unenrolled_individual.py` & `finch_api-0.0.7/src/finch/types/hris/benefits/unenrolled_individual.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/types/hris/company.py` & `finch_api-0.0.7/src/finch/types/hris/company.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/types/hris/company_benefit.py` & `finch_api-0.0.7/src/finch/types/hris/company_benefit.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/types/hris/individual.py` & `finch_api-0.0.7/src/finch/types/hris/individual.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/types/hris/individual_in_directory.py` & `finch_api-0.0.7/src/finch/types/hris/individual_in_directory.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/types/hris/individuals/employment_data.py` & `finch_api-0.0.7/src/finch/types/hris/individuals/employment_data.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/types/hris/individuals/employment_data_retrieve_many_params.py` & `finch_api-0.0.7/src/finch/types/hris/individuals/employment_data_retrieve_many_params.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/types/hris/pay_statement.py` & `finch_api-0.0.7/src/finch/types/hris/pay_statement.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/types/hris/pay_statement_retrieve_many_params.py` & `finch_api-0.0.7/src/finch/types/hris/pay_statement_retrieve_many_params.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/types/hris/payment.py` & `finch_api-0.0.7/src/finch/types/hris/payment.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/types/hris/payment_list_params.py` & `finch_api-0.0.7/src/finch/types/hris/payment_list_params.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/types/hris/supported_benefit.py` & `finch_api-0.0.7/src/finch/types/hris/supported_benefit.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/types/income.py` & `finch_api-0.0.7/src/finch/types/income.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/types/introspection.py` & `finch_api-0.0.7/src/finch/types/introspection.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/types/location.py` & `finch_api-0.0.7/src/finch/types/location.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/src/finch/types/provider.py` & `finch_api-0.0.7/src/finch/types/provider.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.0.6/PKG-INFO` & `finch_api-0.0.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finch-api
-Version: 0.0.6
+Version: 0.0.7
 Summary: Client library for the Finch API
 Home-page: https://github.com/Finch-API/finch-api-python
 License: Apache-2.0
 Author: Finch
 Author-email: founders@tryfinch.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -41,38 +41,38 @@
 ```
 
 ## Usage
 
 ```python
 from finch import Finch
 
-finch = Finch(
+client = Finch(
     access_token="my access token",
 )
 
-candidate = finch.ats.candidates.retrieve(
+candidate = client.ats.candidates.retrieve(
     "<candidate id>",
 )
 print(candidate.first_name)
 ```
 
 ## Async Usage
 
 Simply import `AsyncFinch` instead of `Finch` and use `await` with each API call:
 
 ```python
 from finch import AsyncFinch
 
-finch = AsyncFinch(
+client = AsyncFinch(
     access_token="my access token",
 )
 
 
 async def main():
-    candidate = await finch.ats.candidates.retrieve(
+    candidate = await client.ats.candidates.retrieve(
         "<candidate id>",
     )
     print(candidate.first_name)
 
 
 asyncio.run(main())
 ```
@@ -90,60 +90,60 @@
 List methods in the Finch API are paginated.
 
 This library provides auto-paginating iterators with each list response, so you do not have to request successive pages manually:
 
 ```python
 import finch
 
-finch = Finch()
+client = Finch()
 
 all_jobs = []
 # Automatically fetches more pages as needed.
-for job in finch.ats.jobs.list():
+for job in client.ats.jobs.list():
     # Do something with job here
     all_jobs.append(job)
 print(all_jobs)
 ```
 
 Or, asynchronously:
 
 ```python
 import asyncio
 import finch
 
-finch = AsyncFinch()
+client = AsyncFinch()
 
 
 async def main() -> None:
     all_jobs = []
     # Iterate through items across all pages, issuing requests as needed.
-    async for job in finch.ats.jobs.list():
+    async for job in client.ats.jobs.list():
         all_jobs.append(job)
     print(all_jobs)
 
 
 asyncio.run(main())
 ```
 
 Alternatively, you can use the `.has_next_page()`, `.next_page_info()`, or `.get_next_page()` methods for more granular control working with pages:
 
 ```python
-first_page = await finch.ats.jobs.list()
+first_page = await client.ats.jobs.list()
 if first_page.has_next_page():
     print(f"will fetch next page using these details: {first_page.next_page_info()}")
     next_page = await first_page.get_next_page()
     print(f"number of items we just fetched: {len(next_page.jobs)}")
 
 # Remove `await` for non-async usage.
 ```
 
 Or just work directly with the returned data:
 
 ```python
-first_page = await finch.ats.jobs.list()
+first_page = await client.ats.jobs.list()
 
 print(
     f"the current start offset for this page: {first_page.paging.offset}"
 )  # => "the current start offset for this page: 1"
 for job in first_page.jobs:
     print(job.id)
 
@@ -153,17 +153,17 @@
 ## Nested params
 
 Nested parameters are dictionaries, typed using `TypedDict`, for example:
 
 ```python
 from finch import Finch
 
-finch = Finch()
+client = Finch()
 
-finch.hris.directory.list_individuals(
+client.hris.directory.list_individuals(
     path_params=[],
     params={},
 )
 ```
 
 ## Handling errors
 
@@ -214,44 +214,44 @@
 
 You can use the `max_retries` option to configure or disable this:
 
 ```python
 from finch import Finch
 
 # Configure the default for all requests:
-finch = Finch(
+client = Finch(
     # default is 2
     max_retries=0,
 )
 
 # Or, configure per-request:
-finch.with_options(max_retries=5).hris.directory.list_individuals()
+client.with_options(max_retries=5).hris.directory.list_individuals()
 ```
 
 ### Timeouts
 
 Requests time out after 60 seconds by default. You can configure this with a `timeout` option,
 which accepts a float or an [`httpx.Timeout`](https://www.python-httpx.org/advanced/#fine-tuning-the-configuration):
 
 ```python
 from finch import Finch
 
 # Configure the default for all requests:
-finch = Finch(
+client = Finch(
     # default is 60s
     timeout=20.0,
 )
 
 # More granular control:
-finch = Finch(
+client = Finch(
     timeout=httpx.Timeout(60.0, read=5.0, write=10.0, connect=2.0),
 )
 
 # Override per-request:
-finch.with_options(timeout=5 * 1000).hris.directory.list_individuals()
+client.with_options(timeout=5 * 1000).hris.directory.list_individuals()
 ```
 
 On timeout, an `APITimeoutError` is thrown.
 
 Note that requests which time out will be [retried twice by default](#retries).
 
 ## Default Headers
@@ -261,37 +261,41 @@
 If you need to, you can override it by setting default headers per-request or on the client object.
 
 Be aware that doing so may result in incorrect types and other unexpected or undefined behavior in the SDK.
 
 ```python
 from finch import Finch
 
-finch = Finch(
+client = Finch(
     default_headers={"Finch-API-Version": "My-Custom-Value"},
 )
 ```
 
 ## Advanced: Configuring custom URLs, proxies, and transports
 
 You can configure the following keyword arguments when instantiating the client:
 
 ```python
 import httpx
 from finch import Finch
 
-finch = Finch(
+client = Finch(
     # Use a custom base URL
     base_url="http://my.test.server.example.com:8083",
     proxies="http://my.test.proxy.example.com",
     transport=httpx.HTTPTransport(local_address="0.0.0.0"),
 )
 ```
 
 See the httpx documentation for information about the [`proxies`](https://www.python-httpx.org/advanced/#http-proxying) and [`transport`](https://www.python-httpx.org/advanced/#custom-transports) keyword arguments.
 
+## Advanced: Managing HTTP resources
+
+By default we will close the underlying HTTP connections whenever the client is [garbage collected](https://docs.python.org/3/reference/datamodel.html#object.__del__) is called but you can also manually close the client using the `.close()` method if desired, or with a context manager that closes when exiting.
+
 ## Status
 
 This package is in beta. Its internals and interfaces are not stable and subject to change without a major semver bump;
 please reach out if you rely on any undocumented behavior.
 
 We are keen for your feedback; please open an [issue](https://www.github.com/Finch-API/finch-api-python/issues) with questions, bugs, or suggestions.
```

