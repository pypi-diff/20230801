# Comparing `tmp/sparksampling-0.4.0.tar.gz` & `tmp/sparksampling-0.4.1.tar.gz`

## Comparing `sparksampling-0.4.0.tar` & `sparksampling-0.4.1.tar`

### file list

```diff
@@ -1,100 +1,100 @@
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 sparksampling-0.4.0/.editorconfig
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 sparksampling-0.4.0/.gitattributes
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 sparksampling-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 sparksampling-0.4.0/.travis.yml
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 sparksampling-0.4.0/MANIFEST.in
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 sparksampling-0.4.0/RELEASE.md
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 sparksampling-0.4.0/pip.conf
--rw-r--r--   0        0        0    11324 2020-02-02 00:00:00.000000 sparksampling-0.4.0/client/LICENSE
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 sparksampling-0.4.0/client/README.md
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 sparksampling-0.4.0/client/RELEASE.md
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 sparksampling-0.4.0/client/pyproject.toml
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 sparksampling-0.4.0/client/dockerbuild/config.json
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 sparksampling-0.4.0/client/dockerbuild/ssc.Dockerfile
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sparksampling-0.4.0/client/sparksampling_client/__init__.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 sparksampling-0.4.0/client/sparksampling_client/cli.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 sparksampling-0.4.0/client/sparksampling_client/config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparksampling-0.4.0/client/sparksampling_client/logging.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 sparksampling-0.4.0/client/sparksampling_client/session.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparksampling-0.4.0/client/sparksampling_client/proto/__init__.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 sparksampling-0.4.0/client/sparksampling_client/proto/sampling_service_pb2.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 sparksampling-0.4.0/client/sparksampling_client/proto/sampling_service_pb2_grpc.py
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 sparksampling-0.4.0/client/tests/test_apply.py
--rw-r--r--   0        0        0  2988942 2020-02-02 00:00:00.000000 sparksampling-0.4.0/data/10w_x_10.csv
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 sparksampling-0.4.0/data/empty.csv
--rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 sparksampling-0.4.0/data/iris.csv
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 sparksampling-0.4.0/data/relation-a.csv
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 sparksampling-0.4.0/data/relation-b.csv
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 sparksampling-0.4.0/data/relation-c.csv
--rw-r--r--   0        0        0   943860 2020-02-02 00:00:00.000000 sparksampling-0.4.0/data/ten_million_top1k.csv
--rw-r--r--   0        0        0    15359 2020-02-02 00:00:00.000000 sparksampling-0.4.0/data/unbalance_500v50_10.csv
--rw-r--r--   0        0        0  1518641 2020-02-02 00:00:00.000000 sparksampling-0.4.0/data/unbalance_5w1k_10.csv
--rw-r--r--   0        0        0  1634682 2020-02-02 00:00:00.000000 sparksampling-0.4.0/data/unbalance_5w5k_10.csv
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 sparksampling-0.4.0/dockerbuild/pysparksampling-dev.Dockerfile
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 sparksampling-0.4.0/dockerbuild/pysparksampling.Dockerfile
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 sparksampling-0.4.0/example/extension-example/DEVELOP.md
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 sparksampling-0.4.0/example/extension-example/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparksampling-0.4.0/example/extension-example/sparksampling/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparksampling-0.4.0/example/extension-example/sparksampling/evaluation_extension/__init__.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 sparksampling-0.4.0/example/extension-example/sparksampling/evaluation_extension/example_extension/__init__.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 sparksampling-0.4.0/example/extension-example/sparksampling/evaluation_extension/example_extension/example_extension.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 sparksampling-0.4.0/k8s/spark-sampling-deployment.yaml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 sparksampling-0.4.0/k8s/spark-sampling-headless-service.yaml
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 sparksampling-0.4.0/k8s/spark-sampling-service.yaml
--rwxr-xr-x   0        0        0      151 2020-02-02 00:00:00.000000 sparksampling-0.4.0/k8s/start.sh
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling/__init__.py
--rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling/app.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling/config.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling/default_app_config.py
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling/engine_factory.py
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling/error.py
--rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling/mixin.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling/sdk.py
--rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling/service.py
--rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling/utilities.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling/engine/__init__.py
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling/engine/base_engine.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling/engine/dummy_engine.py
--rw-r--r--   0        0        0    11737 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling/engine/rms_engine.py
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling/engine/sms_engine.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling/engine/stop_engine.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling/evaluation/__init__.py
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling/evaluation/base_hook.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling/evaluation/dummy_hook.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling/evaluation/hook_msg.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling/evaluation/warn_hook.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling/evaluation_extension/__init__.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling/evaluation_extension/dummy_extension/__init__.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling/evaluation_extension/dummy_extension/dummy_hook.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling/file_format/__init__.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling/file_format/base_file_format.py
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling/file_format/csv_file_imp.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling/file_format/file_factory.py
--rw-r--r--   0        0        0     5779 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling/file_format/output_adapter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling/proto/__init__.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling/proto/sampling_service_pb2.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling/proto/sampling_service_pb2_grpc.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling/sample/__init__.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling/sample/base_sampling.py
--rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling/sample/cluster_sampling_imp.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling/sample/random_sampling_imp.py
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling/sample/sampling_factory.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling/sample/simple_sampling_imp.py
--rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling/sample/stratified_sampling_imp.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling_proto/README.md
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling_proto/pyproject.toml
--rw-r--r--   0        0        0     7201 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling_proto/pb/sampling_service.proto
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling_proto/sparksampling_proto/__init__.py
--rw-r--r--   0        0        0     7621 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling_proto/sparksampling_proto/sampling_service_pb2.py
--rw-r--r--   0        0        0     5934 2020-02-02 00:00:00.000000 sparksampling-0.4.0/sparksampling_proto/sparksampling_proto/sampling_service_pb2_grpc.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 sparksampling-0.4.0/tests/conftest.py
--rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 sparksampling-0.4.0/tests/test_feature.py
--rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 sparksampling-0.4.0/tests/test_rms_engine.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 sparksampling-0.4.0/tests/test_s3.py
--rw-r--r--   0        0        0    13415 2020-02-02 00:00:00.000000 sparksampling-0.4.0/tests/test_sms_sampling.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 sparksampling-0.4.0/tests/utilities.py
--rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 sparksampling-0.4.0/.gitignore
--rw-r--r--   0        0        0    11324 2020-02-02 00:00:00.000000 sparksampling-0.4.0/LICENSE
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 sparksampling-0.4.0/README.md
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 sparksampling-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 sparksampling-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 sparksampling-0.4.1/.editorconfig
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 sparksampling-0.4.1/.gitattributes
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 sparksampling-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 sparksampling-0.4.1/.travis.yml
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 sparksampling-0.4.1/MANIFEST.in
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 sparksampling-0.4.1/RELEASE.md
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 sparksampling-0.4.1/pip.conf
+-rw-r--r--   0        0        0    11324 2020-02-02 00:00:00.000000 sparksampling-0.4.1/client/LICENSE
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 sparksampling-0.4.1/client/README.md
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 sparksampling-0.4.1/client/RELEASE.md
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 sparksampling-0.4.1/client/pyproject.toml
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 sparksampling-0.4.1/client/dockerbuild/config.json
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 sparksampling-0.4.1/client/dockerbuild/ssc.Dockerfile
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sparksampling-0.4.1/client/sparksampling_client/__init__.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 sparksampling-0.4.1/client/sparksampling_client/cli.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 sparksampling-0.4.1/client/sparksampling_client/config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparksampling-0.4.1/client/sparksampling_client/logging.py
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 sparksampling-0.4.1/client/sparksampling_client/session.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparksampling-0.4.1/client/sparksampling_client/proto/__init__.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 sparksampling-0.4.1/client/sparksampling_client/proto/sampling_service_pb2.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 sparksampling-0.4.1/client/sparksampling_client/proto/sampling_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 sparksampling-0.4.1/client/tests/test_apply.py
+-rw-r--r--   0        0        0  2988942 2020-02-02 00:00:00.000000 sparksampling-0.4.1/data/10w_x_10.csv
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 sparksampling-0.4.1/data/empty.csv
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 sparksampling-0.4.1/data/iris.csv
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 sparksampling-0.4.1/data/relation-a.csv
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 sparksampling-0.4.1/data/relation-b.csv
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 sparksampling-0.4.1/data/relation-c.csv
+-rw-r--r--   0        0        0   943860 2020-02-02 00:00:00.000000 sparksampling-0.4.1/data/ten_million_top1k.csv
+-rw-r--r--   0        0        0    15359 2020-02-02 00:00:00.000000 sparksampling-0.4.1/data/unbalance_500v50_10.csv
+-rw-r--r--   0        0        0  1518641 2020-02-02 00:00:00.000000 sparksampling-0.4.1/data/unbalance_5w1k_10.csv
+-rw-r--r--   0        0        0  1634682 2020-02-02 00:00:00.000000 sparksampling-0.4.1/data/unbalance_5w5k_10.csv
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 sparksampling-0.4.1/dockerbuild/pysparksampling-dev.Dockerfile
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 sparksampling-0.4.1/dockerbuild/pysparksampling.Dockerfile
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 sparksampling-0.4.1/example/extension-example/DEVELOP.md
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 sparksampling-0.4.1/example/extension-example/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparksampling-0.4.1/example/extension-example/sparksampling/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparksampling-0.4.1/example/extension-example/sparksampling/evaluation_extension/__init__.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 sparksampling-0.4.1/example/extension-example/sparksampling/evaluation_extension/example_extension/__init__.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 sparksampling-0.4.1/example/extension-example/sparksampling/evaluation_extension/example_extension/example_extension.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 sparksampling-0.4.1/k8s/spark-sampling-deployment.yaml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 sparksampling-0.4.1/k8s/spark-sampling-headless-service.yaml
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 sparksampling-0.4.1/k8s/spark-sampling-service.yaml
+-rwxr-xr-x   0        0        0      151 2020-02-02 00:00:00.000000 sparksampling-0.4.1/k8s/start.sh
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling/__init__.py
+-rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling/app.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling/config.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling/default_app_config.py
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling/engine_factory.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling/error.py
+-rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling/mixin.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling/sdk.py
+-rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling/service.py
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling/utilities.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling/engine/__init__.py
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling/engine/base_engine.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling/engine/dummy_engine.py
+-rw-r--r--   0        0        0    11737 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling/engine/rms_engine.py
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling/engine/sms_engine.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling/engine/stop_engine.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling/evaluation/__init__.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling/evaluation/base_hook.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling/evaluation/dummy_hook.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling/evaluation/hook_msg.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling/evaluation/warn_hook.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling/evaluation_extension/__init__.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling/evaluation_extension/dummy_extension/__init__.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling/evaluation_extension/dummy_extension/dummy_hook.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling/file_format/__init__.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling/file_format/base_file_format.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling/file_format/csv_file_imp.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling/file_format/file_factory.py
+-rw-r--r--   0        0        0     5779 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling/file_format/output_adapter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling/proto/__init__.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling/proto/sampling_service_pb2.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling/proto/sampling_service_pb2_grpc.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling/sample/__init__.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling/sample/base_sampling.py
+-rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling/sample/cluster_sampling_imp.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling/sample/random_sampling_imp.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling/sample/sampling_factory.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling/sample/simple_sampling_imp.py
+-rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling/sample/stratified_sampling_imp.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling_proto/README.md
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling_proto/pyproject.toml
+-rw-r--r--   0        0        0     7201 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling_proto/pb/sampling_service.proto
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling_proto/sparksampling_proto/__init__.py
+-rw-r--r--   0        0        0     7621 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling_proto/sparksampling_proto/sampling_service_pb2.py
+-rw-r--r--   0        0        0     5934 2020-02-02 00:00:00.000000 sparksampling-0.4.1/sparksampling_proto/sparksampling_proto/sampling_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 sparksampling-0.4.1/tests/conftest.py
+-rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 sparksampling-0.4.1/tests/test_feature.py
+-rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 sparksampling-0.4.1/tests/test_rms_engine.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 sparksampling-0.4.1/tests/test_s3.py
+-rw-r--r--   0        0        0    13415 2020-02-02 00:00:00.000000 sparksampling-0.4.1/tests/test_sms_sampling.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 sparksampling-0.4.1/tests/utilities.py
+-rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 sparksampling-0.4.1/.gitignore
+-rw-r--r--   0        0        0    11324 2020-02-02 00:00:00.000000 sparksampling-0.4.1/LICENSE
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 sparksampling-0.4.1/README.md
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 sparksampling-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 sparksampling-0.4.1/PKG-INFO
```

### Comparing `sparksampling-0.4.0/.pre-commit-config.yaml` & `sparksampling-0.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/RELEASE.md` & `sparksampling-0.4.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/client/LICENSE` & `sparksampling-0.4.1/client/LICENSE`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/client/README.md` & `sparksampling-0.4.1/client/README.md`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/client/RELEASE.md` & `sparksampling-0.4.1/client/RELEASE.md`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/client/pyproject.toml` & `sparksampling-0.4.1/client/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/client/sparksampling_client/cli.py` & `sparksampling-0.4.1/client/sparksampling_client/cli.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/client/sparksampling_client/config.py` & `sparksampling-0.4.1/client/sparksampling_client/config.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/client/sparksampling_client/session.py` & `sparksampling-0.4.1/client/sparksampling_client/session.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/client/tests/test_apply.py` & `sparksampling-0.4.1/client/tests/test_apply.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/data/10w_x_10.csv` & `sparksampling-0.4.1/data/10w_x_10.csv`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/data/iris.csv` & `sparksampling-0.4.1/data/iris.csv`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/data/ten_million_top1k.csv` & `sparksampling-0.4.1/data/ten_million_top1k.csv`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/data/unbalance_500v50_10.csv` & `sparksampling-0.4.1/data/unbalance_500v50_10.csv`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/data/unbalance_5w1k_10.csv` & `sparksampling-0.4.1/data/unbalance_5w1k_10.csv`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/data/unbalance_5w5k_10.csv` & `sparksampling-0.4.1/data/unbalance_5w5k_10.csv`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/example/extension-example/DEVELOP.md` & `sparksampling-0.4.1/example/extension-example/DEVELOP.md`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/example/extension-example/setup.py` & `sparksampling-0.4.1/example/extension-example/setup.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/k8s/spark-sampling-deployment.yaml` & `sparksampling-0.4.1/k8s/spark-sampling-deployment.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -19,17 +19,17 @@
       containers:
         - name: spark-sampling
           image: wh1isper/pysparksampling:latest
           ports:
             - containerPort: 8530
           imagePullPolicy: IfNotPresent
           env:
-            - name: SPARK_DRIVER_BINDADDRESS
+            - name: SPARGLIM_DRIVER_HOST
               valueFrom:
                 fieldRef:
                   fieldPath: status.podIP
-            - name: SPARK_DRIVER_POD_NAME
+            - name: SPARGLIM_DRIVER_POD_NAME
               valueFrom:
                 fieldRef:
                   fieldPath: metadata.name
             - name: DEPLOY_ON_K8S
               value: 'true'
```

### Comparing `sparksampling-0.4.0/sparksampling/app.py` & `sparksampling-0.4.1/sparksampling/app.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/sparksampling/config.py` & `sparksampling-0.4.1/sparksampling/config.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/sparksampling/engine_factory.py` & `sparksampling-0.4.1/sparksampling/engine_factory.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/sparksampling/error.py` & `sparksampling-0.4.1/sparksampling/error.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/sparksampling/mixin.py` & `sparksampling-0.4.1/sparksampling/mixin.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/sparksampling/service.py` & `sparksampling-0.4.1/sparksampling/service.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/sparksampling/utilities.py` & `sparksampling-0.4.1/sparksampling/utilities.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/sparksampling/engine/base_engine.py` & `sparksampling-0.4.1/sparksampling/engine/base_engine.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/sparksampling/engine/dummy_engine.py` & `sparksampling-0.4.1/sparksampling/engine/dummy_engine.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/sparksampling/engine/rms_engine.py` & `sparksampling-0.4.1/sparksampling/engine/rms_engine.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/sparksampling/engine/sms_engine.py` & `sparksampling-0.4.1/sparksampling/engine/sms_engine.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/sparksampling/evaluation/__init__.py` & `sparksampling-0.4.1/sparksampling/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/sparksampling/evaluation/base_hook.py` & `sparksampling-0.4.1/sparksampling/evaluation/base_hook.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/sparksampling/file_format/base_file_format.py` & `sparksampling-0.4.1/sparksampling/file_format/base_file_format.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/sparksampling/file_format/csv_file_imp.py` & `sparksampling-0.4.1/sparksampling/file_format/csv_file_imp.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,24 @@
     def write(self, df, output_path, output_col=None):
         if output_col:
             self.log.info(f"Write to the specified columns: {output_col}")
             df = df[output_col]
         # When repartition(1), spark will write to a single file
         # Usually this is better for other applications, but there is a performance penalty
         if os.getenv("NO_REPARTITION"):
-            df.write.csv(output_path, sep=self.sep, header=self.with_header, mode="overwrite")
+            df.write.csv(
+                output_path,
+                sep=self.sep,
+                header=self.with_header,
+                escapeQuotes=False,
+                mode="overwrite",
+            )
         else:
             df.repartition(1).write.csv(
-                output_path, sep=self.sep, header=self.with_header, mode="overwrite"
+                output_path,
+                sep=self.sep,
+                header=self.with_header,
+                escapeQuotes=False,
+                mode="overwrite",
             )
 
         return self._get_sampled_file(output_path, sep=self.sep, spark=self.spark)
```

### Comparing `sparksampling-0.4.0/sparksampling/file_format/file_factory.py` & `sparksampling-0.4.1/sparksampling/file_format/file_factory.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/sparksampling/file_format/output_adapter.py` & `sparksampling-0.4.1/sparksampling/file_format/output_adapter.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/sparksampling/sample/base_sampling.py` & `sparksampling-0.4.1/sparksampling/sample/base_sampling.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/sparksampling/sample/cluster_sampling_imp.py` & `sparksampling-0.4.1/sparksampling/sample/cluster_sampling_imp.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/sparksampling/sample/random_sampling_imp.py` & `sparksampling-0.4.1/sparksampling/sample/random_sampling_imp.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/sparksampling/sample/sampling_factory.py` & `sparksampling-0.4.1/sparksampling/sample/sampling_factory.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/sparksampling/sample/simple_sampling_imp.py` & `sparksampling-0.4.1/sparksampling/sample/simple_sampling_imp.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/sparksampling/sample/stratified_sampling_imp.py` & `sparksampling-0.4.1/sparksampling/sample/stratified_sampling_imp.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/sparksampling_proto/pyproject.toml` & `sparksampling-0.4.1/sparksampling_proto/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/sparksampling_proto/pb/sampling_service.proto` & `sparksampling-0.4.1/sparksampling_proto/pb/sampling_service.proto`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/sparksampling_proto/sparksampling_proto/sampling_service_pb2.py` & `sparksampling-0.4.1/sparksampling_proto/sparksampling_proto/sampling_service_pb2.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/sparksampling_proto/sparksampling_proto/sampling_service_pb2_grpc.py` & `sparksampling-0.4.1/sparksampling_proto/sparksampling_proto/sampling_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/tests/conftest.py` & `sparksampling-0.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/tests/test_feature.py` & `sparksampling-0.4.1/tests/test_feature.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/tests/test_rms_engine.py` & `sparksampling-0.4.1/tests/test_rms_engine.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/tests/test_s3.py` & `sparksampling-0.4.1/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/tests/test_sms_sampling.py` & `sparksampling-0.4.1/tests/test_sms_sampling.py`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/.gitignore` & `sparksampling-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/LICENSE` & `sparksampling-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/README.md` & `sparksampling-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/pyproject.toml` & `sparksampling-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sparksampling-0.4.0/PKG-INFO` & `sparksampling-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparksampling
-Version: 0.4.0
+Version: 0.4.1
 Summary: pyspark-sampling
 Project-URL: Source, https://github.com/Wh1isper/pyspark-sampling
 Author-email: Wh1isper <9573586@qq.com>
 License: Apache License 2.0
 License-File: LICENSE
 Keywords: pyspark-sampling,sparksampling
 Classifier: Development Status :: 2 - Pre-Alpha
```

