# Comparing `tmp/doppler-sdk-1.0.1.tar.gz` & `tmp/doppler-sdk-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doppler-sdk-1.0.1.tar", last modified: Mon Jul 31 23:07:55 2023, max compression
+gzip compressed data, was "doppler-sdk-1.0.2.tar", last modified: Tue Aug  1 15:56:34 2023, max compression
```

## Comparing `doppler-sdk-1.0.1.tar` & `doppler-sdk-1.0.2.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:07:55.651224 doppler-sdk-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-31 23:07:55.651224 doppler-sdk-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 23:07:55.651224 doppler-sdk-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:07:55.635223 doppler-sdk-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:07:55.635223 doppler-sdk-1.0.1/src/doppler_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-31 23:07:55.000000 doppler-sdk-1.0.1/src/doppler_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-07-31 23:07:55.000000 doppler-sdk-1.0.1/src/doppler_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 23:07:55.000000 doppler-sdk-1.0.1/src/doppler_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-31 23:07:55.000000 doppler-sdk-1.0.1/src/doppler_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-31 23:07:55.000000 doppler-sdk-1.0.1/src/doppler_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:07:55.639223 doppler-sdk-1.0.1/src/dopplersdk/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:07:55.639223 doppler-sdk-1.0.1/src/dopplersdk/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/hooks/hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:07:55.647224 doppler-sdk-1.0.1/src/dopplersdk/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/ActivityLogsList200Response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/ActivityLogsRetrieve200Response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/ConfigLogsGet200Response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/ConfigLogsList200Response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/ConfigLogsRollback200Response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/ConfigsClone200Response.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/ConfigsCloneRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/ConfigsCreate200Response.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/ConfigsCreateRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/ConfigsDelete200Response.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/ConfigsDeleteRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/ConfigsGet200Response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/ConfigsList200Response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/ConfigsLock200Response.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/ConfigsLockRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/ConfigsUnlock200Response.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/ConfigsUnlockRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/ConfigsUpdate200Response.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/ConfigsUpdateRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/DynamicSecretsIssueLeaseRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/DynamicSecretsRevokeLease200Response.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/DynamicSecretsRevokeLeaseRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/EnvironmentsCreate200Response.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/EnvironmentsCreateRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/EnvironmentsGet200Response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/EnvironmentsList200Response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/EnvironmentsRename200Response.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/EnvironmentsRenameRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/IntegrationsCreate200Response.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/IntegrationsCreateRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/IntegrationsDelete200Response.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/IntegrationsGet200Response.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/IntegrationsUpdate200Response.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/IntegrationsUpdateRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/ProjectsCreate200Response.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/ProjectsCreateRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/ProjectsDeleteRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/ProjectsGet200Response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/ProjectsList200Response.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/ProjectsUpdate200Response.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/ProjectsUpdateRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/SecretsDownload200Response.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/SecretsGet200Response.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/SecretsListNames200Response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/SecretsUpdate200Response.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/SecretsUpdateNote200Response.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/SecretsUpdateNoteRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/SecretsUpdateRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/ServiceTokensCreateRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/ServiceTokensDelete200Response.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/ServiceTokensDeleteRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/SyncsCreate200Response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/SyncsCreateRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/SyncsDelete200Response.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/SyncsGet200Response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/V3Me200Response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:07:55.647224 doppler-sdk-1.0.1/src/dopplersdk/net/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/net/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/net/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/net/http_content_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/net/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:07:55.651224 doppler-sdk-1.0.1/src/dopplersdk/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/services/activity_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/services/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/services/config_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/services/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/services/dynamic_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/services/environments.py
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/services/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/services/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/services/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/services/service_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/services/syncs.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/services/v_3.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-31 23:07:42.000000 doppler-sdk-1.0.1/src/dopplersdk/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:56:33.994659 doppler-sdk-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-01 15:56:33.994659 doppler-sdk-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 15:56:33.994659 doppler-sdk-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:56:33.982659 doppler-sdk-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:56:33.982659 doppler-sdk-1.0.2/src/doppler_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-01 15:56:33.000000 doppler-sdk-1.0.2/src/doppler_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-08-01 15:56:33.000000 doppler-sdk-1.0.2/src/doppler_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 15:56:33.000000 doppler-sdk-1.0.2/src/doppler_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-01 15:56:33.000000 doppler-sdk-1.0.2/src/doppler_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-01 15:56:33.000000 doppler-sdk-1.0.2/src/doppler_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:56:33.986659 doppler-sdk-1.0.2/src/dopplersdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:56:33.986659 doppler-sdk-1.0.2/src/dopplersdk/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/hooks/hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:56:33.990659 doppler-sdk-1.0.2/src/dopplersdk/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/ActivityLogsList200Response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/ActivityLogsRetrieve200Response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/ConfigLogsGet200Response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/ConfigLogsList200Response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/ConfigLogsRollback200Response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/ConfigsClone200Response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/ConfigsCloneRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/ConfigsCreate200Response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/ConfigsCreateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/ConfigsDelete200Response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/ConfigsDeleteRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/ConfigsGet200Response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/ConfigsList200Response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/ConfigsLock200Response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/ConfigsLockRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/ConfigsUnlock200Response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/ConfigsUnlockRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/ConfigsUpdate200Response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/ConfigsUpdateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/DynamicSecretsIssueLeaseRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/DynamicSecretsRevokeLease200Response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/DynamicSecretsRevokeLeaseRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/EnvironmentsCreate200Response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/EnvironmentsCreateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/EnvironmentsGet200Response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/EnvironmentsList200Response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/EnvironmentsRename200Response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/EnvironmentsRenameRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/IntegrationsCreate200Response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/IntegrationsCreateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/IntegrationsDelete200Response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/IntegrationsGet200Response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/IntegrationsUpdate200Response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/IntegrationsUpdateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/ProjectsCreate200Response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/ProjectsCreateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/ProjectsDeleteRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/ProjectsGet200Response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/ProjectsList200Response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/ProjectsUpdate200Response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/ProjectsUpdateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/SecretsDownload200Response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/SecretsGet200Response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/SecretsListNames200Response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/SecretsUpdate200Response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/SecretsUpdateNote200Response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/SecretsUpdateNoteRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/SecretsUpdateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/ServiceTokensCreateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/ServiceTokensDelete200Response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/ServiceTokensDeleteRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/SyncsCreate200Response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/SyncsCreateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/SyncsDelete200Response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/SyncsGet200Response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/V3Me200Response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:56:33.990659 doppler-sdk-1.0.2/src/dopplersdk/net/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/net/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/net/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/net/http_content_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/net/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:56:33.994659 doppler-sdk-1.0.2/src/dopplersdk/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/services/activity_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/services/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/services/config_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/services/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/services/dynamic_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/services/environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/services/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/services/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/services/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/services/service_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/services/syncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/services/v_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-08-01 15:56:24.000000 doppler-sdk-1.0.2/src/dopplersdk/setup.py
```

### Comparing `doppler-sdk-1.0.1/PKG-INFO` & `doppler-sdk-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doppler-sdk
-Version: 1.0.1
+Version: 1.0.2
 Author-email: Example Author <author@example.com>
 License: SEE LICENSE IN LICENSE
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `doppler-sdk-1.0.1/README.md` & `doppler-sdk-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/doppler_sdk.egg-info/PKG-INFO` & `doppler-sdk-1.0.2/src/doppler_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doppler-sdk
-Version: 1.0.1
+Version: 1.0.2
 Author-email: Example Author <author@example.com>
 License: SEE LICENSE IN LICENSE
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `doppler-sdk-1.0.1/src/doppler_sdk.egg-info/SOURCES.txt` & `doppler-sdk-1.0.2/src/doppler_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/models/ActivityLogsList200Response.py` & `doppler-sdk-1.0.2/src/dopplersdk/models/ActivityLogsList200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/models/ActivityLogsRetrieve200Response.py` & `doppler-sdk-1.0.2/src/dopplersdk/models/ActivityLogsRetrieve200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/models/ConfigLogsGet200Response.py` & `doppler-sdk-1.0.2/src/dopplersdk/models/ConfigLogsGet200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/models/ConfigLogsList200Response.py` & `doppler-sdk-1.0.2/src/dopplersdk/models/ConfigLogsList200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/models/ConfigLogsRollback200Response.py` & `doppler-sdk-1.0.2/src/dopplersdk/models/ConfigLogsRollback200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/models/ConfigsClone200Response.py` & `doppler-sdk-1.0.2/src/dopplersdk/models/ConfigsClone200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/models/ConfigsCloneRequest.py` & `doppler-sdk-1.0.2/src/dopplersdk/models/ConfigsCloneRequest.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/models/ConfigsCreate200Response.py` & `doppler-sdk-1.0.2/src/dopplersdk/models/ConfigsCreate200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/models/ConfigsCreateRequest.py` & `doppler-sdk-1.0.2/src/dopplersdk/models/ConfigsCreateRequest.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/models/ConfigsGet200Response.py` & `doppler-sdk-1.0.2/src/dopplersdk/models/ConfigsGet200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/models/ConfigsList200Response.py` & `doppler-sdk-1.0.2/src/dopplersdk/models/ConfigsList200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/models/ConfigsLock200Response.py` & `doppler-sdk-1.0.2/src/dopplersdk/models/ConfigsLock200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/models/ConfigsUnlock200Response.py` & `doppler-sdk-1.0.2/src/dopplersdk/models/ConfigsUnlock200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/models/ConfigsUpdate200Response.py` & `doppler-sdk-1.0.2/src/dopplersdk/models/ConfigsUpdate200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/models/ConfigsUpdateRequest.py` & `doppler-sdk-1.0.2/src/dopplersdk/models/ConfigsUpdateRequest.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/models/DynamicSecretsIssueLeaseRequest.py` & `doppler-sdk-1.0.2/src/dopplersdk/models/DynamicSecretsIssueLeaseRequest.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/models/DynamicSecretsRevokeLeaseRequest.py` & `doppler-sdk-1.0.2/src/dopplersdk/models/DynamicSecretsRevokeLeaseRequest.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/models/EnvironmentsCreate200Response.py` & `doppler-sdk-1.0.2/src/dopplersdk/models/EnvironmentsCreate200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/models/EnvironmentsGet200Response.py` & `doppler-sdk-1.0.2/src/dopplersdk/models/EnvironmentsGet200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/models/EnvironmentsList200Response.py` & `doppler-sdk-1.0.2/src/dopplersdk/models/EnvironmentsList200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/models/EnvironmentsRename200Response.py` & `doppler-sdk-1.0.2/src/dopplersdk/models/EnvironmentsRename200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/models/IntegrationsCreateRequest.py` & `doppler-sdk-1.0.2/src/dopplersdk/models/IntegrationsCreateRequest.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/models/IntegrationsUpdateRequest.py` & `doppler-sdk-1.0.2/src/dopplersdk/models/IntegrationsUpdateRequest.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/models/ProjectsCreate200Response.py` & `doppler-sdk-1.0.2/src/dopplersdk/models/ProjectsCreate200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/models/ProjectsGet200Response.py` & `doppler-sdk-1.0.2/src/dopplersdk/models/ProjectsGet200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/models/ProjectsList200Response.py` & `doppler-sdk-1.0.2/src/dopplersdk/models/ProjectsList200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/models/ProjectsUpdate200Response.py` & `doppler-sdk-1.0.2/src/dopplersdk/models/ProjectsUpdate200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/models/ProjectsUpdateRequest.py` & `doppler-sdk-1.0.2/src/dopplersdk/models/ProjectsUpdateRequest.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/models/SecretsDownload200Response.py` & `doppler-sdk-1.0.2/src/dopplersdk/models/SecretsDownload200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/models/SecretsGet200Response.py` & `doppler-sdk-1.0.2/src/dopplersdk/models/SecretsGet200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/models/SecretsUpdate200Response.py` & `doppler-sdk-1.0.2/src/dopplersdk/models/SecretsUpdate200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/models/SecretsUpdateNoteRequest.py` & `doppler-sdk-1.0.2/src/dopplersdk/models/SecretsUpdateNoteRequest.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/models/SecretsUpdateRequest.py` & `doppler-sdk-1.0.2/src/dopplersdk/models/SecretsUpdateRequest.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/models/ServiceTokensCreateRequest.py` & `doppler-sdk-1.0.2/src/dopplersdk/models/ServiceTokensCreateRequest.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/models/ServiceTokensDeleteRequest.py` & `doppler-sdk-1.0.2/src/dopplersdk/models/ServiceTokensDeleteRequest.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/models/SyncsCreateRequest.py` & `doppler-sdk-1.0.2/src/dopplersdk/models/SyncsCreateRequest.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/models/V3Me200Response.py` & `doppler-sdk-1.0.2/src/dopplersdk/models/V3Me200Response.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/models/__init__.py` & `doppler-sdk-1.0.2/src/dopplersdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/models/base.py` & `doppler-sdk-1.0.2/src/dopplersdk/models/base.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/net/http_client.py` & `doppler-sdk-1.0.2/src/dopplersdk/net/http_client.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/net/http_content_types.py` & `doppler-sdk-1.0.2/src/dopplersdk/net/http_content_types.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/net/utils.py` & `doppler-sdk-1.0.2/src/dopplersdk/net/utils.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/sdk.py` & `doppler-sdk-1.0.2/src/dopplersdk/sdk.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/services/activity_logs.py` & `doppler-sdk-1.0.2/src/dopplersdk/services/activity_logs.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/services/base.py` & `doppler-sdk-1.0.2/src/dopplersdk/services/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,10 +89,10 @@
         Request authorization headers
 
         Parameters
         ----------
         headers: dict
             Headers dict to add auth headers to
         """
-        headers["User-Agent"] = "liblab/0.1.11 DopplerSDK/1.0.1 python/2.7"
+        headers["User-Agent"] = "liblab/0.1.11 DopplerSDK/1.0.2 python/2.7"
         headers["Authorization"] = f"Bearer {self._bearer_token}"
         return headers
```

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/services/config_logs.py` & `doppler-sdk-1.0.2/src/dopplersdk/services/config_logs.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/services/configs.py` & `doppler-sdk-1.0.2/src/dopplersdk/services/configs.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/services/dynamic_secrets.py` & `doppler-sdk-1.0.2/src/dopplersdk/services/dynamic_secrets.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/services/environments.py` & `doppler-sdk-1.0.2/src/dopplersdk/services/environments.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/services/integrations.py` & `doppler-sdk-1.0.2/src/dopplersdk/services/integrations.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/services/projects.py` & `doppler-sdk-1.0.2/src/dopplersdk/services/projects.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/services/secrets.py` & `doppler-sdk-1.0.2/src/dopplersdk/services/secrets.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/services/service_tokens.py` & `doppler-sdk-1.0.2/src/dopplersdk/services/service_tokens.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/services/syncs.py` & `doppler-sdk-1.0.2/src/dopplersdk/services/syncs.py`

 * *Files identical despite different names*

### Comparing `doppler-sdk-1.0.1/src/dopplersdk/services/v_3.py` & `doppler-sdk-1.0.2/src/dopplersdk/services/v_3.py`

 * *Files identical despite different names*

