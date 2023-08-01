# Comparing `tmp/fano-oss-py-sdk-7.1.16.tar.gz` & `tmp/fano-oss-py-sdk-7.1.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/patrickwu/Git/fano-oss-py-sdk/dist/.tmp-ok1p8von/fano-oss-py-sdk-7.1.16.tar", last modified: Thu Jul  6 08:16:53 2023, max compression
+gzip compressed data, was "/Users/patrickwu/Git/fano-oss-py-sdk/dist/.tmp-6a470jcl/fano-oss-py-sdk-7.1.17.tar", last modified: Tue Aug  1 10:34:45 2023, max compression
```

## Comparing `fano-oss-py-sdk-7.1.16.tar` & `fano-oss-py-sdk-7.1.17.tar`

### file list

```diff
@@ -1,155 +1,155 @@
-drwxr-xr-x   0 patrickwu   (501) staff       (20)        0 2023-07-06 08:16:53.000000 fano-oss-py-sdk-7.1.16/
--rw-r--r--   0 patrickwu   (501) staff       (20)    11358 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/LICENSE
--rw-r--r--   0 patrickwu   (501) staff       (20)      235 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/MANIFEST.in
--rw-r--r--   0 patrickwu   (501) staff       (20)     1475 2023-07-06 08:16:53.000000 fano-oss-py-sdk-7.1.16/PKG-INFO
--rw-r--r--   0 patrickwu   (501) staff       (20)      610 2023-07-06 08:04:09.000000 fano-oss-py-sdk-7.1.16/README.md
--rw-r--r--   0 patrickwu   (501) staff       (20)     3222 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/README.orig.md
--rw-r--r--   0 patrickwu   (501) staff       (20)     9087 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/README_zh_CN.md
-drwxr-xr-x   0 patrickwu   (501) staff       (20)        0 2023-07-06 08:16:53.000000 fano-oss-py-sdk-7.1.16/docs/
--rw-r--r--   0 patrickwu   (501) staff       (20)    63144 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/docs/API.md
-drwxr-xr-x   0 patrickwu   (501) staff       (20)        0 2023-07-06 08:16:53.000000 fano-oss-py-sdk-7.1.16/docs/zh_CN/
--rw-r--r--   0 patrickwu   (501) staff       (20)    33853 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/docs/zh_CN/API.md
--rw-r--r--   0 patrickwu   (501) staff       (20)      688 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/docs/zh_CN/CONTRIBUTING.md
-drwxr-xr-x   0 patrickwu   (501) staff       (20)        0 2023-07-06 08:16:53.000000 fano-oss-py-sdk-7.1.16/examples/
--rw-r--r--   0 patrickwu   (501) staff       (20)      930 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/bucket_exists.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     1744 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/compose_object.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     1733 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/copy_object.py
--rw-r--r--   0 patrickwu   (501) staff       (20)      873 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/delete_bucket_encryption.py
--rw-r--r--   0 patrickwu   (501) staff       (20)      872 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/delete_bucket_lifecycle.py
--rw-r--r--   0 patrickwu   (501) staff       (20)      875 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/delete_bucket_notification.py
--rw-r--r--   0 patrickwu   (501) staff       (20)      869 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/delete_bucket_policy.py
--rw-r--r--   0 patrickwu   (501) staff       (20)      874 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/delete_bucket_replication.py
--rw-r--r--   0 patrickwu   (501) staff       (20)      867 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/delete_bucket_tags.py
--rw-r--r--   0 patrickwu   (501) staff       (20)      874 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/delete_object_lock_config.py
--rw-r--r--   0 patrickwu   (501) staff       (20)      880 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/delete_object_tags.py
--rw-r--r--   0 patrickwu   (501) staff       (20)      887 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/disable_object_legal_hold.py
--rw-r--r--   0 patrickwu   (501) staff       (20)      886 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/enable_object_legal_hold.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     1288 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/fget_object.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     3561 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/fput_object.py
--rw-r--r--   0 patrickwu   (501) staff       (20)      879 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/get_bucket_encryption.py
--rw-r--r--   0 patrickwu   (501) staff       (20)      878 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/get_bucket_lifecycle.py
--rw-r--r--   0 patrickwu   (501) staff       (20)      881 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/get_bucket_notification.py
--rw-r--r--   0 patrickwu   (501) staff       (20)      875 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/get_bucket_policy.py
--rw-r--r--   0 patrickwu   (501) staff       (20)      880 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/get_bucket_replication.py
--rw-r--r--   0 patrickwu   (501) staff       (20)      871 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/get_bucket_tags.py
--rw-r--r--   0 patrickwu   (501) staff       (20)      900 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/get_bucket_versioning.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     1818 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/get_object.py
--rw-r--r--   0 patrickwu   (501) staff       (20)      880 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/get_object_lock_config.py
--rw-r--r--   0 patrickwu   (501) staff       (20)      891 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/get_object_retention.py
--rw-r--r--   0 patrickwu   (501) staff       (20)      884 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/get_object_tags.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     1600 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/get_presigned_url.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     1000 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/is_object_legal_hold_enabled.py
--rw-r--r--   0 patrickwu   (501) staff       (20)      918 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/list_buckets.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     1641 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/list_objects.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     1026 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/listen_bucket_notification.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     1074 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/make_bucket.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     1635 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/minio_with_assume_role_provider.py
--rw-r--r--   0 patrickwu   (501) staff       (20)      897 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/minio_with_aws_config_provider.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     1209 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/minio_with_certificate_identity_provider.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     1274 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/minio_with_chained_provider.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     1686 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/minio_with_client_grants_provider.py
--rw-r--r--   0 patrickwu   (501) staff       (20)      891 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/minio_with_env_aws_provider.py
--rw-r--r--   0 patrickwu   (501) staff       (20)      900 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/minio_with_env_minio_provider.py
--rw-r--r--   0 patrickwu   (501) staff       (20)      891 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/minio_with_iam_aws_provider.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     1161 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/minio_with_ldap_identity_provider.py
--rw-r--r--   0 patrickwu   (501) staff       (20)      925 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/minio_with_minio_client_config_provider.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     2009 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/minio_with_web_identity_provider.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     1222 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/presigned_get_object.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     1386 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/presigned_post_policy.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     1234 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/presigned_put_object.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     6203 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/progress.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     4036 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/put_object.py
--rw-r--r--   0 patrickwu   (501) staff       (20)      852 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/remove_bucket.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     1023 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/remove_object.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     1490 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/remove_objects.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     1297 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/select_object_content.py
--rw-r--r--   0 patrickwu   (501) staff       (20)      956 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/set_bucket_encryption.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     1410 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/set_bucket_lifecycle.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     1260 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/set_bucket_notification.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     2252 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/set_bucket_policy.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     1650 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/set_bucket_replication.py
--rw-r--r--   0 patrickwu   (501) staff       (20)      992 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/set_bucket_tags.py
--rw-r--r--   0 patrickwu   (501) staff       (20)      988 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/set_bucket_versioning.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     1027 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/set_object_lock_config.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     1083 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/set_object_retention.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     1005 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/set_object_tags.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     1567 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/stat_object.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     1266 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/examples/upload_snowball_objects.py
-drwxr-xr-x   0 patrickwu   (501) staff       (20)        0 2023-07-06 08:16:53.000000 fano-oss-py-sdk-7.1.16/fano_oss_py_sdk.egg-info/
--rw-r--r--   0 patrickwu   (501) staff       (20)     1475 2023-07-06 08:16:53.000000 fano-oss-py-sdk-7.1.16/fano_oss_py_sdk.egg-info/PKG-INFO
--rw-r--r--   0 patrickwu   (501) staff       (20)     4184 2023-07-06 08:16:53.000000 fano-oss-py-sdk-7.1.16/fano_oss_py_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 patrickwu   (501) staff       (20)        1 2023-07-06 08:16:53.000000 fano-oss-py-sdk-7.1.16/fano_oss_py_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 patrickwu   (501) staff       (20)       16 2023-07-06 08:16:53.000000 fano-oss-py-sdk-7.1.16/fano_oss_py_sdk.egg-info/requires.txt
--rw-r--r--   0 patrickwu   (501) staff       (20)        6 2023-07-06 08:16:53.000000 fano-oss-py-sdk-7.1.16/fano_oss_py_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 patrickwu   (501) staff       (20)        0 2023-07-06 08:16:53.000000 fano-oss-py-sdk-7.1.16/minio/
--rw-r--r--   0 patrickwu   (501) staff       (20)     1569 2023-07-06 08:16:30.000000 fano-oss-py-sdk-7.1.16/minio/__init__.py
--rw-r--r--   0 patrickwu   (501) staff       (20)   108025 2023-07-04 10:12:40.000000 fano-oss-py-sdk-7.1.16/minio/api.py
--rw-r--r--   0 patrickwu   (501) staff       (20)    16029 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/minio/commonconfig.py
-drwxr-xr-x   0 patrickwu   (501) staff       (20)        0 2023-07-06 08:16:53.000000 fano-oss-py-sdk-7.1.16/minio/credentials/
--rw-r--r--   0 patrickwu   (501) staff       (20)     1096 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/minio/credentials/__init__.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     2017 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/minio/credentials/credentials.py
--rw-r--r--   0 patrickwu   (501) staff       (20)    21375 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/minio/credentials/providers.py
--rw-r--r--   0 patrickwu   (501) staff       (20)    26494 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/minio/datatypes.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     4837 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/minio/deleteobjects.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     4394 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/minio/error.py
--rw-r--r--   0 patrickwu   (501) staff       (20)    22749 2023-07-04 09:47:59.000000 fano-oss-py-sdk-7.1.16/minio/helpers.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     1430 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/minio/legalhold.py
--rw-r--r--   0 patrickwu   (501) staff       (20)    12765 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/minio/lifecycleconfig.py
--rw-r--r--   0 patrickwu   (501) staff       (20)    10253 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/minio/minioadmin.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     9775 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/minio/notificationconfig.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     2987 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/minio/objectlockconfig.py
--rw-r--r--   0 patrickwu   (501) staff       (20)    15277 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/minio/replicationconfig.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     2243 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/minio/retention.py
--rw-r--r--   0 patrickwu   (501) staff       (20)    14413 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/minio/select.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     8448 2023-07-04 10:14:14.000000 fano-oss-py-sdk-7.1.16/minio/signer.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     3168 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/minio/sse.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     3039 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/minio/sseconfig.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     1508 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/minio/tagging.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     3522 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/minio/time.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     2141 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/minio/versioningconfig.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     2896 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/minio/xml.py
--rw-r--r--   0 patrickwu   (501) staff       (20)       38 2023-07-06 08:16:53.000000 fano-oss-py-sdk-7.1.16/setup.cfg
--rw-r--r--   0 patrickwu   (501) staff       (20)     2195 2023-07-06 08:05:24.000000 fano-oss-py-sdk-7.1.16/setup.py
-drwxr-xr-x   0 patrickwu   (501) staff       (20)        0 2023-07-06 08:16:53.000000 fano-oss-py-sdk-7.1.16/tests/
--rw-r--r--   0 patrickwu   (501) staff       (20)        0 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/tests/__init__.py
-drwxr-xr-x   0 patrickwu   (501) staff       (20)        0 2023-07-06 08:16:53.000000 fano-oss-py-sdk-7.1.16/tests/certs/
--rw-r--r--   0 patrickwu   (501) staff       (20)      241 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/tests/certs/private.key
--rw-r--r--   0 patrickwu   (501) staff       (20)      696 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/tests/certs/public.crt
-drwxr-xr-x   0 patrickwu   (501) staff       (20)        0 2023-07-06 08:16:53.000000 fano-oss-py-sdk-7.1.16/tests/functional/
--rw-r--r--   0 patrickwu   (501) staff       (20)      119 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/tests/functional/play.min.io.kes.root.key
--rw-r--r--   0 patrickwu   (501) staff       (20)    69407 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/tests/functional/tests.py
-drwxr-xr-x   0 patrickwu   (501) staff       (20)        0 2023-07-06 08:16:53.000000 fano-oss-py-sdk-7.1.16/tests/unit/
--rw-r--r--   0 patrickwu   (501) staff       (20)      656 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/tests/unit/__init__.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     2758 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/tests/unit/bucket_exist_test.py
--rw-r--r--   0 patrickwu   (501) staff       (20)      334 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/tests/unit/config.json.sample
--rw-r--r--   0 patrickwu   (501) staff       (20)     1662 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/tests/unit/copy_object_test.py
--rw-r--r--   0 patrickwu   (501) staff       (20)        0 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/tests/unit/credentials.empty
--rw-r--r--   0 patrickwu   (501) staff       (20)      242 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/tests/unit/credentials.sample
--rw-r--r--   0 patrickwu   (501) staff       (20)     9162 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/tests/unit/credentials_test.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     3612 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/tests/unit/get_bucket_policy_test.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     2101 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/tests/unit/get_object_test.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     1110 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/tests/unit/helpers.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     1118 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/tests/unit/legelhold_test.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     3045 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/tests/unit/lifecycleconfig_test.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     3436 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/tests/unit/list_buckets_test.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     3713 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/tests/unit/list_objects_test.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     7280 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/tests/unit/list_objects_v1_test.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     2521 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/tests/unit/make_bucket_test.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     2856 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/tests/unit/minio_mocks.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     5966 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/tests/unit/minio_test.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     2190 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/tests/unit/notificationconfig_test.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     1486 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/tests/unit/objectlockconfig_test.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     2014 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/tests/unit/presigned_get_object_test.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     1383 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/tests/unit/presigned_put_object_test.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     1595 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/tests/unit/put_object_test.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     1806 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/tests/unit/remove_bucket_test.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     1872 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/tests/unit/remove_object_test.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     3064 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/tests/unit/remove_objects_test.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     2548 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/tests/unit/replicationconfig_test.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     1477 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/tests/unit/retention_test.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     7856 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/tests/unit/sign_test.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     1572 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/tests/unit/sseconfig_test.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     2130 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/tests/unit/stat_object_test.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     1339 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/tests/unit/tagging_test.py
--rw-r--r--   0 patrickwu   (501) staff       (20)      886 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/tests/unit/trace_test.py
--rw-r--r--   0 patrickwu   (501) staff       (20)     1917 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.16/tests/unit/versioningconfig_test.py
+drwxr-xr-x   0 patrickwu   (501) staff       (20)        0 2023-08-01 10:34:45.000000 fano-oss-py-sdk-7.1.17/
+-rw-r--r--   0 patrickwu   (501) staff       (20)    11358 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/LICENSE
+-rw-r--r--   0 patrickwu   (501) staff       (20)      235 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/MANIFEST.in
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1475 2023-08-01 10:34:45.000000 fano-oss-py-sdk-7.1.17/PKG-INFO
+-rw-r--r--   0 patrickwu   (501) staff       (20)      610 2023-07-06 08:04:09.000000 fano-oss-py-sdk-7.1.17/README.md
+-rw-r--r--   0 patrickwu   (501) staff       (20)     3222 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/README.orig.md
+-rw-r--r--   0 patrickwu   (501) staff       (20)     9087 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/README_zh_CN.md
+drwxr-xr-x   0 patrickwu   (501) staff       (20)        0 2023-08-01 10:34:45.000000 fano-oss-py-sdk-7.1.17/docs/
+-rw-r--r--   0 patrickwu   (501) staff       (20)    63144 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/docs/API.md
+drwxr-xr-x   0 patrickwu   (501) staff       (20)        0 2023-08-01 10:34:45.000000 fano-oss-py-sdk-7.1.17/docs/zh_CN/
+-rw-r--r--   0 patrickwu   (501) staff       (20)    33853 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/docs/zh_CN/API.md
+-rw-r--r--   0 patrickwu   (501) staff       (20)      688 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/docs/zh_CN/CONTRIBUTING.md
+drwxr-xr-x   0 patrickwu   (501) staff       (20)        0 2023-08-01 10:34:45.000000 fano-oss-py-sdk-7.1.17/examples/
+-rw-r--r--   0 patrickwu   (501) staff       (20)      930 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/bucket_exists.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1744 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/compose_object.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1733 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/copy_object.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)      873 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/delete_bucket_encryption.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)      872 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/delete_bucket_lifecycle.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)      875 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/delete_bucket_notification.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)      869 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/delete_bucket_policy.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)      874 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/delete_bucket_replication.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)      867 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/delete_bucket_tags.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)      874 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/delete_object_lock_config.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)      880 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/delete_object_tags.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)      887 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/disable_object_legal_hold.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)      886 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/enable_object_legal_hold.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1288 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/fget_object.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     3561 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/fput_object.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)      879 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/get_bucket_encryption.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)      878 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/get_bucket_lifecycle.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)      881 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/get_bucket_notification.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)      875 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/get_bucket_policy.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)      880 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/get_bucket_replication.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)      871 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/get_bucket_tags.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)      900 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/get_bucket_versioning.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1818 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/get_object.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)      880 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/get_object_lock_config.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)      891 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/get_object_retention.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)      884 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/get_object_tags.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1600 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/get_presigned_url.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1000 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/is_object_legal_hold_enabled.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)      918 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/list_buckets.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1641 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/list_objects.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1026 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/listen_bucket_notification.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1074 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/make_bucket.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1635 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/minio_with_assume_role_provider.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)      897 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/minio_with_aws_config_provider.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1209 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/minio_with_certificate_identity_provider.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1274 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/minio_with_chained_provider.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1686 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/minio_with_client_grants_provider.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)      891 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/minio_with_env_aws_provider.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)      900 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/minio_with_env_minio_provider.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)      891 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/minio_with_iam_aws_provider.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1161 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/minio_with_ldap_identity_provider.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)      925 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/minio_with_minio_client_config_provider.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     2009 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/minio_with_web_identity_provider.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1222 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/presigned_get_object.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1386 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/presigned_post_policy.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1234 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/presigned_put_object.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     6203 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/progress.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     4036 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/put_object.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)      852 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/remove_bucket.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1023 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/remove_object.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1490 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/remove_objects.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1297 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/select_object_content.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)      956 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/set_bucket_encryption.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1410 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/set_bucket_lifecycle.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1260 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/set_bucket_notification.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     2252 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/set_bucket_policy.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1650 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/set_bucket_replication.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)      992 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/set_bucket_tags.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)      988 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/set_bucket_versioning.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1027 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/set_object_lock_config.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1083 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/set_object_retention.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1005 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/set_object_tags.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1567 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/stat_object.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1266 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/examples/upload_snowball_objects.py
+drwxr-xr-x   0 patrickwu   (501) staff       (20)        0 2023-08-01 10:34:45.000000 fano-oss-py-sdk-7.1.17/fano_oss_py_sdk.egg-info/
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1475 2023-08-01 10:34:45.000000 fano-oss-py-sdk-7.1.17/fano_oss_py_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 patrickwu   (501) staff       (20)     4184 2023-08-01 10:34:45.000000 fano-oss-py-sdk-7.1.17/fano_oss_py_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 patrickwu   (501) staff       (20)        1 2023-08-01 10:34:45.000000 fano-oss-py-sdk-7.1.17/fano_oss_py_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 patrickwu   (501) staff       (20)       16 2023-08-01 10:34:45.000000 fano-oss-py-sdk-7.1.17/fano_oss_py_sdk.egg-info/requires.txt
+-rw-r--r--   0 patrickwu   (501) staff       (20)        6 2023-08-01 10:34:45.000000 fano-oss-py-sdk-7.1.17/fano_oss_py_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 patrickwu   (501) staff       (20)        0 2023-08-01 10:34:45.000000 fano-oss-py-sdk-7.1.17/minio/
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1569 2023-08-01 10:31:31.000000 fano-oss-py-sdk-7.1.17/minio/__init__.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)   108271 2023-08-01 10:28:32.000000 fano-oss-py-sdk-7.1.17/minio/api.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)    16029 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/minio/commonconfig.py
+drwxr-xr-x   0 patrickwu   (501) staff       (20)        0 2023-08-01 10:34:45.000000 fano-oss-py-sdk-7.1.17/minio/credentials/
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1096 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/minio/credentials/__init__.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     2017 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/minio/credentials/credentials.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)    21375 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/minio/credentials/providers.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)    26494 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/minio/datatypes.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     4837 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/minio/deleteobjects.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     4394 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/minio/error.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)    22749 2023-08-01 10:28:23.000000 fano-oss-py-sdk-7.1.17/minio/helpers.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1430 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/minio/legalhold.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)    12765 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/minio/lifecycleconfig.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)    10253 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/minio/minioadmin.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     9775 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/minio/notificationconfig.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     2987 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/minio/objectlockconfig.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)    15277 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/minio/replicationconfig.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     2243 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/minio/retention.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)    14413 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/minio/select.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     8448 2023-07-04 10:14:14.000000 fano-oss-py-sdk-7.1.17/minio/signer.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     3168 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/minio/sse.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     3039 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/minio/sseconfig.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1508 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/minio/tagging.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     3522 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/minio/time.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     2141 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/minio/versioningconfig.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     2896 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/minio/xml.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)       38 2023-08-01 10:34:45.000000 fano-oss-py-sdk-7.1.17/setup.cfg
+-rw-r--r--   0 patrickwu   (501) staff       (20)     2195 2023-07-06 08:05:24.000000 fano-oss-py-sdk-7.1.17/setup.py
+drwxr-xr-x   0 patrickwu   (501) staff       (20)        0 2023-08-01 10:34:45.000000 fano-oss-py-sdk-7.1.17/tests/
+-rw-r--r--   0 patrickwu   (501) staff       (20)        0 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/tests/__init__.py
+drwxr-xr-x   0 patrickwu   (501) staff       (20)        0 2023-08-01 10:34:45.000000 fano-oss-py-sdk-7.1.17/tests/certs/
+-rw-r--r--   0 patrickwu   (501) staff       (20)      241 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/tests/certs/private.key
+-rw-r--r--   0 patrickwu   (501) staff       (20)      696 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/tests/certs/public.crt
+drwxr-xr-x   0 patrickwu   (501) staff       (20)        0 2023-08-01 10:34:45.000000 fano-oss-py-sdk-7.1.17/tests/functional/
+-rw-r--r--   0 patrickwu   (501) staff       (20)      119 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/tests/functional/play.min.io.kes.root.key
+-rw-r--r--   0 patrickwu   (501) staff       (20)    69407 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/tests/functional/tests.py
+drwxr-xr-x   0 patrickwu   (501) staff       (20)        0 2023-08-01 10:34:45.000000 fano-oss-py-sdk-7.1.17/tests/unit/
+-rw-r--r--   0 patrickwu   (501) staff       (20)      656 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/tests/unit/__init__.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     2758 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/tests/unit/bucket_exist_test.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)      334 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/tests/unit/config.json.sample
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1662 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/tests/unit/copy_object_test.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)        0 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/tests/unit/credentials.empty
+-rw-r--r--   0 patrickwu   (501) staff       (20)      242 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/tests/unit/credentials.sample
+-rw-r--r--   0 patrickwu   (501) staff       (20)     9162 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/tests/unit/credentials_test.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     3612 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/tests/unit/get_bucket_policy_test.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     2101 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/tests/unit/get_object_test.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1110 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/tests/unit/helpers.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1118 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/tests/unit/legelhold_test.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     3045 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/tests/unit/lifecycleconfig_test.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     3436 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/tests/unit/list_buckets_test.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     3713 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/tests/unit/list_objects_test.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     7280 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/tests/unit/list_objects_v1_test.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     2521 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/tests/unit/make_bucket_test.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     2856 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/tests/unit/minio_mocks.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     5966 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/tests/unit/minio_test.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     2190 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/tests/unit/notificationconfig_test.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1486 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/tests/unit/objectlockconfig_test.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     2014 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/tests/unit/presigned_get_object_test.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1383 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/tests/unit/presigned_put_object_test.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1595 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/tests/unit/put_object_test.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1806 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/tests/unit/remove_bucket_test.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1872 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/tests/unit/remove_object_test.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     3064 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/tests/unit/remove_objects_test.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     2548 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/tests/unit/replicationconfig_test.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1477 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/tests/unit/retention_test.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     7856 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/tests/unit/sign_test.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1572 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/tests/unit/sseconfig_test.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     2130 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/tests/unit/stat_object_test.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1339 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/tests/unit/tagging_test.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)      886 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/tests/unit/trace_test.py
+-rw-r--r--   0 patrickwu   (501) staff       (20)     1917 2023-07-04 07:51:58.000000 fano-oss-py-sdk-7.1.17/tests/unit/versioningconfig_test.py
```

### Comparing `fano-oss-py-sdk-7.1.16/LICENSE` & `fano-oss-py-sdk-7.1.17/LICENSE`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/PKG-INFO` & `fano-oss-py-sdk-7.1.17/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fano-oss-py-sdk
-Version: 7.1.16
+Version: 7.1.17
 Summary: A fork of minio-py with some modifications.
 Author: Fano Labs
 Author-email: patrick.wu@fano.ai
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `fano-oss-py-sdk-7.1.16/README.md` & `fano-oss-py-sdk-7.1.17/README.md`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/README.orig.md` & `fano-oss-py-sdk-7.1.17/README.orig.md`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/README_zh_CN.md` & `fano-oss-py-sdk-7.1.17/README_zh_CN.md`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/docs/API.md` & `fano-oss-py-sdk-7.1.17/docs/API.md`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/docs/zh_CN/API.md` & `fano-oss-py-sdk-7.1.17/docs/zh_CN/API.md`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/docs/zh_CN/CONTRIBUTING.md` & `fano-oss-py-sdk-7.1.17/docs/zh_CN/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/bucket_exists.py` & `fano-oss-py-sdk-7.1.17/examples/bucket_exists.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/compose_object.py` & `fano-oss-py-sdk-7.1.17/examples/compose_object.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/copy_object.py` & `fano-oss-py-sdk-7.1.17/examples/copy_object.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/delete_bucket_encryption.py` & `fano-oss-py-sdk-7.1.17/examples/delete_bucket_encryption.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/delete_bucket_lifecycle.py` & `fano-oss-py-sdk-7.1.17/examples/delete_bucket_lifecycle.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/delete_bucket_notification.py` & `fano-oss-py-sdk-7.1.17/examples/delete_bucket_notification.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/delete_bucket_policy.py` & `fano-oss-py-sdk-7.1.17/examples/delete_bucket_policy.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/delete_bucket_replication.py` & `fano-oss-py-sdk-7.1.17/examples/delete_bucket_replication.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/delete_bucket_tags.py` & `fano-oss-py-sdk-7.1.17/examples/delete_bucket_tags.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/delete_object_lock_config.py` & `fano-oss-py-sdk-7.1.17/examples/delete_object_lock_config.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/delete_object_tags.py` & `fano-oss-py-sdk-7.1.17/examples/delete_object_tags.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/disable_object_legal_hold.py` & `fano-oss-py-sdk-7.1.17/examples/disable_object_legal_hold.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/enable_object_legal_hold.py` & `fano-oss-py-sdk-7.1.17/examples/enable_object_legal_hold.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/fget_object.py` & `fano-oss-py-sdk-7.1.17/examples/fget_object.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/fput_object.py` & `fano-oss-py-sdk-7.1.17/examples/fput_object.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/get_bucket_encryption.py` & `fano-oss-py-sdk-7.1.17/examples/get_bucket_encryption.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/get_bucket_lifecycle.py` & `fano-oss-py-sdk-7.1.17/examples/get_bucket_lifecycle.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/get_bucket_notification.py` & `fano-oss-py-sdk-7.1.17/examples/get_bucket_notification.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/get_bucket_policy.py` & `fano-oss-py-sdk-7.1.17/examples/get_bucket_policy.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/get_bucket_replication.py` & `fano-oss-py-sdk-7.1.17/examples/get_bucket_replication.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/get_bucket_tags.py` & `fano-oss-py-sdk-7.1.17/examples/get_bucket_tags.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/get_bucket_versioning.py` & `fano-oss-py-sdk-7.1.17/examples/get_bucket_versioning.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/get_object.py` & `fano-oss-py-sdk-7.1.17/examples/get_object.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/get_object_lock_config.py` & `fano-oss-py-sdk-7.1.17/examples/get_object_lock_config.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/get_object_retention.py` & `fano-oss-py-sdk-7.1.17/examples/get_object_retention.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/get_object_tags.py` & `fano-oss-py-sdk-7.1.17/examples/get_object_tags.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/get_presigned_url.py` & `fano-oss-py-sdk-7.1.17/examples/get_presigned_url.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/is_object_legal_hold_enabled.py` & `fano-oss-py-sdk-7.1.17/examples/is_object_legal_hold_enabled.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/list_buckets.py` & `fano-oss-py-sdk-7.1.17/examples/list_buckets.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/list_objects.py` & `fano-oss-py-sdk-7.1.17/examples/list_objects.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/listen_bucket_notification.py` & `fano-oss-py-sdk-7.1.17/examples/listen_bucket_notification.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/make_bucket.py` & `fano-oss-py-sdk-7.1.17/examples/make_bucket.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/minio_with_assume_role_provider.py` & `fano-oss-py-sdk-7.1.17/examples/minio_with_assume_role_provider.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/minio_with_aws_config_provider.py` & `fano-oss-py-sdk-7.1.17/examples/minio_with_aws_config_provider.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/minio_with_certificate_identity_provider.py` & `fano-oss-py-sdk-7.1.17/examples/minio_with_certificate_identity_provider.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/minio_with_chained_provider.py` & `fano-oss-py-sdk-7.1.17/examples/minio_with_chained_provider.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/minio_with_client_grants_provider.py` & `fano-oss-py-sdk-7.1.17/examples/minio_with_client_grants_provider.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/minio_with_env_aws_provider.py` & `fano-oss-py-sdk-7.1.17/examples/minio_with_env_aws_provider.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/minio_with_env_minio_provider.py` & `fano-oss-py-sdk-7.1.17/examples/minio_with_env_minio_provider.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/minio_with_iam_aws_provider.py` & `fano-oss-py-sdk-7.1.17/examples/minio_with_iam_aws_provider.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/minio_with_ldap_identity_provider.py` & `fano-oss-py-sdk-7.1.17/examples/minio_with_ldap_identity_provider.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/minio_with_minio_client_config_provider.py` & `fano-oss-py-sdk-7.1.17/examples/minio_with_minio_client_config_provider.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/minio_with_web_identity_provider.py` & `fano-oss-py-sdk-7.1.17/examples/minio_with_web_identity_provider.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/presigned_get_object.py` & `fano-oss-py-sdk-7.1.17/examples/presigned_get_object.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/presigned_post_policy.py` & `fano-oss-py-sdk-7.1.17/examples/presigned_post_policy.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/presigned_put_object.py` & `fano-oss-py-sdk-7.1.17/examples/presigned_put_object.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/progress.py` & `fano-oss-py-sdk-7.1.17/examples/progress.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/put_object.py` & `fano-oss-py-sdk-7.1.17/examples/put_object.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/remove_bucket.py` & `fano-oss-py-sdk-7.1.17/examples/remove_bucket.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/remove_object.py` & `fano-oss-py-sdk-7.1.17/examples/remove_object.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/remove_objects.py` & `fano-oss-py-sdk-7.1.17/examples/remove_objects.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/select_object_content.py` & `fano-oss-py-sdk-7.1.17/examples/select_object_content.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/set_bucket_encryption.py` & `fano-oss-py-sdk-7.1.17/examples/set_bucket_encryption.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/set_bucket_lifecycle.py` & `fano-oss-py-sdk-7.1.17/examples/set_bucket_lifecycle.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/set_bucket_notification.py` & `fano-oss-py-sdk-7.1.17/examples/set_bucket_notification.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/set_bucket_policy.py` & `fano-oss-py-sdk-7.1.17/examples/set_bucket_policy.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/set_bucket_replication.py` & `fano-oss-py-sdk-7.1.17/examples/set_bucket_replication.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/set_bucket_tags.py` & `fano-oss-py-sdk-7.1.17/examples/set_bucket_tags.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/set_bucket_versioning.py` & `fano-oss-py-sdk-7.1.17/examples/set_bucket_versioning.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/set_object_lock_config.py` & `fano-oss-py-sdk-7.1.17/examples/set_object_lock_config.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/set_object_retention.py` & `fano-oss-py-sdk-7.1.17/examples/set_object_retention.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/set_object_tags.py` & `fano-oss-py-sdk-7.1.17/examples/set_object_tags.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/stat_object.py` & `fano-oss-py-sdk-7.1.17/examples/stat_object.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/examples/upload_snowball_objects.py` & `fano-oss-py-sdk-7.1.17/examples/upload_snowball_objects.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/fano_oss_py_sdk.egg-info/PKG-INFO` & `fano-oss-py-sdk-7.1.17/fano_oss_py_sdk.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fano-oss-py-sdk
-Version: 7.1.16
+Version: 7.1.17
 Summary: A fork of minio-py with some modifications.
 Author: Fano Labs
 Author-email: patrick.wu@fano.ai
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `fano-oss-py-sdk-7.1.16/fano_oss_py_sdk.egg-info/SOURCES.txt` & `fano-oss-py-sdk-7.1.17/fano_oss_py_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/minio/__init__.py` & `fano-oss-py-sdk-7.1.17/minio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 :copyright: (C) 2015-2020 MinIO, Inc., 2023 Fanolabs 
 :license: Apache 2.0, see LICENSE for more details.
 """
 
 __title__ = "fano-oss-py-sdk"
 __author__ = "Fano Labs"
-__version__ = "7.1.16"
+__version__ = "7.1.17"
 __license__ = "Apache 2.0"
 __copyright__ = "Copyright 2015, 2016, 2017, 2018, 2019, 2020 MinIO, Inc."
 
 # pylint: disable=unused-import
 from .api import Minio
 from .error import InvalidResponseError, S3Error, ServerError
 from .minioadmin import MinioAdmin
```

### Comparing `fano-oss-py-sdk-7.1.16/minio/api.py` & `fano-oss-py-sdk-7.1.17/minio/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,23 +119,27 @@
                  session_token=None,
                  secure=True,
                  region=None,
                  http_client=None,
                  credentials=None,
                  cert_check=True,
                  external_host=None,
-                 contextual_path=False):
+                 contextual_path=False,
+                 force_region=False):
         # Validate http client has correct base class.
         if http_client and not isinstance(
                 http_client,
                 urllib3.poolmanager.PoolManager):
             raise ValueError(
                 "HTTP client should be instance of "
                 "`urllib3.poolmanager.PoolManager`"
             )
+        force_region = force_region if os.getenv('FANO_OSS_FORCE_REGION') is None else os.getenv('FANO_OSS_FORCE_REGION') == 'true'
+        if region is None and force_region:
+            region = "us-east-1"
 
         self._region_map = {}
         self._base_url = BaseURL(
             ("https://" if secure else "http://") + endpoint,
             region,
         )
         if external_host is not None:
```

### Comparing `fano-oss-py-sdk-7.1.16/minio/commonconfig.py` & `fano-oss-py-sdk-7.1.17/minio/commonconfig.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/minio/credentials/__init__.py` & `fano-oss-py-sdk-7.1.17/minio/credentials/__init__.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/minio/credentials/credentials.py` & `fano-oss-py-sdk-7.1.17/minio/credentials/credentials.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/minio/credentials/providers.py` & `fano-oss-py-sdk-7.1.17/minio/credentials/providers.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/minio/datatypes.py` & `fano-oss-py-sdk-7.1.17/minio/datatypes.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/minio/deleteobjects.py` & `fano-oss-py-sdk-7.1.17/minio/deleteobjects.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/minio/error.py` & `fano-oss-py-sdk-7.1.17/minio/error.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/minio/helpers.py` & `fano-oss-py-sdk-7.1.17/minio/helpers.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/minio/legalhold.py` & `fano-oss-py-sdk-7.1.17/minio/legalhold.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/minio/lifecycleconfig.py` & `fano-oss-py-sdk-7.1.17/minio/lifecycleconfig.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/minio/minioadmin.py` & `fano-oss-py-sdk-7.1.17/minio/minioadmin.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/minio/notificationconfig.py` & `fano-oss-py-sdk-7.1.17/minio/notificationconfig.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/minio/objectlockconfig.py` & `fano-oss-py-sdk-7.1.17/minio/objectlockconfig.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/minio/replicationconfig.py` & `fano-oss-py-sdk-7.1.17/minio/replicationconfig.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/minio/retention.py` & `fano-oss-py-sdk-7.1.17/minio/retention.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/minio/select.py` & `fano-oss-py-sdk-7.1.17/minio/select.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/minio/signer.py` & `fano-oss-py-sdk-7.1.17/minio/signer.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/minio/sse.py` & `fano-oss-py-sdk-7.1.17/minio/sse.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/minio/sseconfig.py` & `fano-oss-py-sdk-7.1.17/minio/sseconfig.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/minio/tagging.py` & `fano-oss-py-sdk-7.1.17/minio/tagging.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/minio/time.py` & `fano-oss-py-sdk-7.1.17/minio/time.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/minio/versioningconfig.py` & `fano-oss-py-sdk-7.1.17/minio/versioningconfig.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/minio/xml.py` & `fano-oss-py-sdk-7.1.17/minio/xml.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/setup.py` & `fano-oss-py-sdk-7.1.17/setup.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/tests/certs/public.crt` & `fano-oss-py-sdk-7.1.17/tests/certs/public.crt`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/tests/functional/tests.py` & `fano-oss-py-sdk-7.1.17/tests/functional/tests.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/tests/unit/__init__.py` & `fano-oss-py-sdk-7.1.17/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/tests/unit/bucket_exist_test.py` & `fano-oss-py-sdk-7.1.17/tests/unit/bucket_exist_test.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/tests/unit/copy_object_test.py` & `fano-oss-py-sdk-7.1.17/tests/unit/copy_object_test.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/tests/unit/credentials_test.py` & `fano-oss-py-sdk-7.1.17/tests/unit/credentials_test.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/tests/unit/get_bucket_policy_test.py` & `fano-oss-py-sdk-7.1.17/tests/unit/get_bucket_policy_test.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/tests/unit/get_object_test.py` & `fano-oss-py-sdk-7.1.17/tests/unit/get_object_test.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/tests/unit/helpers.py` & `fano-oss-py-sdk-7.1.17/tests/unit/helpers.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/tests/unit/legelhold_test.py` & `fano-oss-py-sdk-7.1.17/tests/unit/legelhold_test.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/tests/unit/lifecycleconfig_test.py` & `fano-oss-py-sdk-7.1.17/tests/unit/lifecycleconfig_test.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/tests/unit/list_buckets_test.py` & `fano-oss-py-sdk-7.1.17/tests/unit/list_buckets_test.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/tests/unit/list_objects_test.py` & `fano-oss-py-sdk-7.1.17/tests/unit/list_objects_test.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/tests/unit/list_objects_v1_test.py` & `fano-oss-py-sdk-7.1.17/tests/unit/list_objects_v1_test.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/tests/unit/make_bucket_test.py` & `fano-oss-py-sdk-7.1.17/tests/unit/make_bucket_test.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/tests/unit/minio_mocks.py` & `fano-oss-py-sdk-7.1.17/tests/unit/minio_mocks.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/tests/unit/minio_test.py` & `fano-oss-py-sdk-7.1.17/tests/unit/minio_test.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/tests/unit/notificationconfig_test.py` & `fano-oss-py-sdk-7.1.17/tests/unit/notificationconfig_test.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/tests/unit/objectlockconfig_test.py` & `fano-oss-py-sdk-7.1.17/tests/unit/objectlockconfig_test.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/tests/unit/presigned_get_object_test.py` & `fano-oss-py-sdk-7.1.17/tests/unit/presigned_get_object_test.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/tests/unit/presigned_put_object_test.py` & `fano-oss-py-sdk-7.1.17/tests/unit/presigned_put_object_test.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/tests/unit/put_object_test.py` & `fano-oss-py-sdk-7.1.17/tests/unit/put_object_test.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/tests/unit/remove_bucket_test.py` & `fano-oss-py-sdk-7.1.17/tests/unit/remove_bucket_test.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/tests/unit/remove_object_test.py` & `fano-oss-py-sdk-7.1.17/tests/unit/remove_object_test.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/tests/unit/remove_objects_test.py` & `fano-oss-py-sdk-7.1.17/tests/unit/remove_objects_test.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/tests/unit/replicationconfig_test.py` & `fano-oss-py-sdk-7.1.17/tests/unit/replicationconfig_test.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/tests/unit/retention_test.py` & `fano-oss-py-sdk-7.1.17/tests/unit/retention_test.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/tests/unit/sign_test.py` & `fano-oss-py-sdk-7.1.17/tests/unit/sign_test.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/tests/unit/sseconfig_test.py` & `fano-oss-py-sdk-7.1.17/tests/unit/sseconfig_test.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/tests/unit/stat_object_test.py` & `fano-oss-py-sdk-7.1.17/tests/unit/stat_object_test.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/tests/unit/tagging_test.py` & `fano-oss-py-sdk-7.1.17/tests/unit/tagging_test.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/tests/unit/trace_test.py` & `fano-oss-py-sdk-7.1.17/tests/unit/trace_test.py`

 * *Files identical despite different names*

### Comparing `fano-oss-py-sdk-7.1.16/tests/unit/versioningconfig_test.py` & `fano-oss-py-sdk-7.1.17/tests/unit/versioningconfig_test.py`

 * *Files identical despite different names*

