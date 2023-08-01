# Comparing `tmp/bentoml-1.1.0.tar.gz` & `tmp/bentoml-1.1.1.tar.gz`

## Comparing `bentoml-1.1.0.tar` & `bentoml-1.1.1.tar`

### file list

```diff
@@ -1,290 +1,290 @@
--rw-r--r--   0        0        0     7343 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/__init__.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/__main__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_version.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/batch.py
--rw-r--r--   0        0        0    20111 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/bentos.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/catboost.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/client.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/cloud.py
--rw-r--r--   0        0        0    16750 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/container.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/detectron.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/diffusers.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/easyocr.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/evalml.py
--rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/exceptions.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/fastai.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/fasttext.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/flax.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/gluon.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/h2o.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/io.py
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/keras.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/lightgbm.py
--rw-r--r--   0        0        0    15368 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/metrics.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/metrics.pyi
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/mlflow.py
--rw-r--r--   0        0        0    11309 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/models.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/monitoring.py
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/onnx.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/onnxmlir.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/paddle.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/picklable_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/py.typed
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/pycaret.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/pyspark.py
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/pytorch.py
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/pytorch_lightning.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/ray.py
--rw-r--r--   0        0        0    30679 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/serve.py
--rw-r--r--   0        0        0    15414 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/server.py
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/sklearn.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/spacy.py
--rw-r--r--   0        0        0    14382 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/start.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/statsmodels.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/tensorflow.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/tensorflow_v1.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/torchscript.py
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/transformers.py
--rw-r--r--   0        0        0     8328 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/triton.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/types.py
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/xgboost.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/__init__.py
--rw-r--r--   0        0        0     7037 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/context.py
--rw-r--r--   0        0        0    13916 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/exportable.py
--rw-r--r--   0        0        0     4822 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/log.py
--rw-r--r--   0        0        0     9725 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/resource.py
--rw-r--r--   0        0        0     6625 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/store.py
--rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/tag.py
--rw-r--r--   0        0        0    10982 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/batch/__init__.py
--rw-r--r--   0        0        0     5625 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/batch/spark.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/bento/__init__.py
--rw-r--r--   0        0        0    20522 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/bento/bento.py
--rw-r--r--   0        0        0    36144 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/bento/build_config.py
--rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/bento/build_dev_bentoml_whl.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/bento/gen.py
--rw-r--r--   0        0        0     4805 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/client/__init__.py
--rw-r--r--   0        0        0    14454 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/client/grpc.py
--rw-r--r--   0        0        0     7113 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/client/http.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/cloud/__init__.py
--rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/cloud/base.py
--rw-r--r--   0        0        0    43056 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/cloud/bentocloud.py
--rw-r--r--   0        0        0    19538 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/cloud/client.py
--rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/cloud/config.py
--rw-r--r--   0        0        0    21890 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/cloud/deployment.py
--rw-r--r--   0        0        0    19150 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/cloud/schemas.py
--rw-r--r--   0        0        0    41949 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/cloud/yatai.py
--rw-r--r--   0        0        0     6224 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/configuration/__init__.py
--rw-r--r--   0        0        0    18788 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/configuration/containers.py
--rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/configuration/helpers.py
--rw-r--r--   0        0        0    11251 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/configuration/v1/__init__.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/configuration/v1/default_configuration.yaml
--rw-r--r--   0        0        0    11401 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/container/__init__.py
--rw-r--r--   0        0        0     7877 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/container/base.py
--rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/container/buildah.py
--rw-r--r--   0        0        0     5425 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/container/buildctl.py
--rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/container/buildx.py
--rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/container/docker.py
--rw-r--r--   0        0        0     6881 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/container/generate.py
--rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/container/nerdctl.py
--rw-r--r--   0        0        0     4831 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/container/podman.py
--rw-r--r--   0        0        0     5606 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/container/frontend/dockerfile/__init__.py
--rwxr-xr-x   0        0        0     2522 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/container/frontend/dockerfile/entrypoint.sh
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/container/frontend/dockerfile/templates/_macros.j2
--rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/container/frontend/dockerfile/templates/base.j2
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/container/frontend/dockerfile/templates/base_alpine.j2
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/container/frontend/dockerfile/templates/base_amazonlinux.j2
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/container/frontend/dockerfile/templates/base_debian.j2
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/container/frontend/dockerfile/templates/base_ubi8.j2
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/container/frontend/dockerfile/templates/cuda_debian.j2
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/container/frontend/dockerfile/templates/cuda_ubi8.j2
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/container/frontend/dockerfile/templates/miniconda_alpine.j2
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/container/frontend/dockerfile/templates/miniconda_debian.j2
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/container/frontend/dockerfile/templates/python_alpine.j2
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/container/frontend/dockerfile/templates/python_amazonlinux.j2
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/container/frontend/dockerfile/templates/python_debian.j2
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/container/frontend/dockerfile/templates/python_ubi8.j2
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/env_manager/__init__.py
--rw-r--r--   0        0        0     4565 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/env_manager/envs.py
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/env_manager/manager.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/external_typing/__init__.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/external_typing/starlette.py
--rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/external_typing/tensorflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/frameworks/__init__.py
--rw-r--r--   0        0        0     9919 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/frameworks/catboost.py
--rw-r--r--   0        0        0    12024 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/frameworks/detectron.py
--rw-r--r--   0        0        0    24613 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/frameworks/diffusers.py
--rw-r--r--   0        0        0     6837 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/frameworks/easyocr.py
--rw-r--r--   0        0        0    11302 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/frameworks/fastai.py
--rw-r--r--   0        0        0    12449 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/frameworks/flax.py
--rw-r--r--   0        0        0    12576 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/frameworks/keras.py
--rw-r--r--   0        0        0    10014 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/frameworks/lightgbm.py
--rw-r--r--   0        0        0     9362 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/frameworks/mlflow.py
--rw-r--r--   0        0        0    16612 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/frameworks/onnx.py
--rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/frameworks/picklable.py
--rw-r--r--   0        0        0     7527 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/frameworks/pytorch.py
--rw-r--r--   0        0        0     7345 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/frameworks/pytorch_lightning.py
--rw-r--r--   0        0        0     6750 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/frameworks/sklearn.py
--rw-r--r--   0        0        0    15375 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/frameworks/tensorflow_v2.py
--rw-r--r--   0        0        0     6828 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/frameworks/torchscript.py
--rw-r--r--   0        0        0    36119 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/frameworks/transformers.py
--rw-r--r--   0        0        0    11073 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/frameworks/xgboost.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/frameworks/common/__init__.py
--rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/frameworks/common/jax.py
--rw-r--r--   0        0        0     6745 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/frameworks/common/pytorch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/frameworks/utils/__init__.py
--rw-r--r--   0        0        0     5192 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/frameworks/utils/onnx.py
--rw-r--r--   0        0        0    17082 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/frameworks/utils/tensorflow.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/frameworks/utils/transformers.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/io_descriptors/__init__.py
--rw-r--r--   0        0        0     5700 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/io_descriptors/base.py
--rw-r--r--   0        0        0    13705 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/io_descriptors/file.py
--rw-r--r--   0        0        0    19126 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/io_descriptors/image.py
--rw-r--r--   0        0        0    18392 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/io_descriptors/json.py
--rw-r--r--   0        0        0    13651 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/io_descriptors/multipart.py
--rw-r--r--   0        0        0    24632 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/io_descriptors/numpy.py
--rw-r--r--   0        0        0    49329 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/io_descriptors/pandas.py
--rw-r--r--   0        0        0     5791 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/io_descriptors/text.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/marshal/__init__.py
--rw-r--r--   0        0        0    14813 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/marshal/dispatcher.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/models/__init__.py
--rw-r--r--   0        0        0    25400 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/models/model.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/monitoring/__init__.py
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/monitoring/api.py
--rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/monitoring/base.py
--rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/monitoring/default.py
--rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/monitoring/otlp.py
--rw-r--r--   0        0        0     7634 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/ray/__init__.py
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/ray/runner_handle.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/runner/__init__.py
--rw-r--r--   0        0        0    24051 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/runner/container.py
--rw-r--r--   0        0        0     4829 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/runner/runnable.py
--rw-r--r--   0        0        0    12809 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/runner/runner.py
--rw-r--r--   0        0        0     6778 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/runner/strategy.py
--rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/runner/utils.py
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/runner/runner_handle/__init__.py
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/runner/runner_handle/local.py
--rw-r--r--   0        0        0    19059 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/runner/runner_handle/remote.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/server/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/server/__init__.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/server/base_app.py
--rw-r--r--   0        0        0    13583 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/server/grpc_app.py
--rw-r--r--   0        0        0    16822 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/server/http_app.py
--rw-r--r--   0        0        0    12258 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/server/runner_app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/server/grpc/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/server/grpc/servicer/__init__.py
--rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/server/grpc/servicer/v1/__init__.py
--rw-r--r--   0        0        0     5289 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/server/grpc/servicer/v1alpha1/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/server/http/__init__.py
--rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/server/http/access.py
--rw-r--r--   0        0        0     9114 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/server/http/instruments.py
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/server/http/traffic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/server/metrics/__init__.py
--rw-r--r--   0        0        0     6192 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/server/metrics/prometheus.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/server/static_content/favicon-dark-32x32.png
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/server/static_content/favicon-light-32x32.png
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/server/static_content/index.css
--rw-r--r--   0        0        0    36011 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/server/static_content/marked.min.js
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/server/static_content/swagger-initializer.js
--rw-r--r--   0        0        0  1096221 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/server/static_content/swagger-ui-bundle.js
--rw-r--r--   0        0        0   339540 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/server/static_content/swagger-ui-standalone-preset.js
--rw-r--r--   0        0        0   143980 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/server/static_content/swagger-ui.css
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/service/__init__.py
--rw-r--r--   0        0        0     7109 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/service/inference_api.py
--rw-r--r--   0        0        0    14652 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/service/loader.py
--rw-r--r--   0        0        0    16459 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/service/service.py
--rw-r--r--   0        0        0     6387 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/service/openapi/__init__.py
--rw-r--r--   0        0        0     9879 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/service/openapi/specification.py
--rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/service/openapi/utils.py
--rw-r--r--   0        0        0    15903 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/utils/__init__.py
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/utils/alg.py
--rw-r--r--   0        0        0    13986 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/utils/benchmark.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/utils/buildx.py
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/utils/cattr.py
--rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/utils/dotenv.py
--rw-r--r--   0        0        0    14318 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/utils/formparser.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/utils/http.py
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/utils/lazy_loader.py
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/utils/metrics.py
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/utils/pickle.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/utils/pkg.py
--rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/utils/telemetry.py
--rw-r--r--   0        0        0     7614 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/utils/unflatten.py
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/utils/uri.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/utils/analytics/__init__.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/utils/analytics/cli_events.py
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/utils/analytics/schemas.py
--rw-r--r--   0        0        0    10371 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/utils/analytics/usage_stats.py
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/utils/circus/__init__.py
--rw-r--r--   0        0        0     4628 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/_internal/utils/circus/watchfilesplugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/grpc/__init__.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/grpc/buf.yaml
--rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/grpc/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/grpc/interceptors/__init__.py
--rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/grpc/interceptors/access.py
--rw-r--r--   0        0        0    10292 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/grpc/interceptors/opentelemetry.py
--rw-r--r--   0        0        0     5522 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/grpc/interceptors/prometheus.py
--rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/grpc/utils/__init__.py
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/grpc/utils/_import_hook.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/grpc/v1/__init__.py
--rw-r--r--   0        0        0     9391 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/grpc/v1/service.proto
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/grpc/v1/service_pb2.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/grpc/v1/service_pb2.pyi
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/grpc/v1/service_pb2_grpc.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/grpc/v1/service_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/grpc/v1/_generated_pb3/__init__.py
--rw-r--r--   0        0        0    14406 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/grpc/v1/_generated_pb3/service_pb2.py
--rw-r--r--   0        0        0    28650 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/grpc/v1/_generated_pb3/service_pb2.pyi
--rw-r--r--   0        0        0     4274 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/grpc/v1/_generated_pb3/service_pb2_grpc.py
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/grpc/v1/_generated_pb3/service_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/grpc/v1/_generated_pb4/__init__.py
--rw-r--r--   0        0        0     9598 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/grpc/v1/_generated_pb4/service_pb2.py
--rw-r--r--   0        0        0    28987 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/grpc/v1/_generated_pb4/service_pb2.pyi
--rw-r--r--   0        0        0     4274 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/grpc/v1/_generated_pb4/service_pb2_grpc.py
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/grpc/v1/_generated_pb4/service_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/grpc/v1alpha1/__init__.py
--rw-r--r--   0        0        0     8488 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/grpc/v1alpha1/service.proto
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/grpc/v1alpha1/service_pb2.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/grpc/v1alpha1/service_pb2.pyi
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/grpc/v1alpha1/service_pb2_grpc.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/grpc/v1alpha1/service_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/grpc/v1alpha1/_generated_pb3/__init__.py
--rw-r--r--   0        0        0    12103 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/grpc/v1alpha1/_generated_pb3/service_pb2.py
--rw-r--r--   0        0        0    24953 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/grpc/v1alpha1/_generated_pb3/service_pb2.pyi
--rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/grpc/v1alpha1/_generated_pb3/service_pb2_grpc.py
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/grpc/v1alpha1/_generated_pb3/service_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/grpc/v1alpha1/_generated_pb4/__init__.py
--rw-r--r--   0        0        0     8916 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/grpc/v1alpha1/_generated_pb4/service_pb2.py
--rw-r--r--   0        0        0    25182 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/grpc/v1alpha1/_generated_pb4/service_pb2.pyi
--rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/grpc/v1alpha1/_generated_pb4/service_pb2_grpc.py
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/grpc/v1alpha1/_generated_pb4/service_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/testing/__init__.py
--rw-r--r--   0        0        0    18696 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/testing/server.py
--rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/testing/utils.py
--rw-r--r--   0        0        0     8397 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/testing/grpc/__init__.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/testing/pytest/__init__.py
--rw-r--r--   0        0        0    10433 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml/testing/pytest/plugin.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml_cli/__init__.py
--rw-r--r--   0        0        0    15555 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml_cli/bentos.py
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml_cli/cli.py
--rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml_cli/cloud.py
--rw-r--r--   0        0        0    23294 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml_cli/containerize.py
--rw-r--r--   0        0        0     9066 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml_cli/deployment.py
--rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml_cli/env.py
--rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml_cli/env_manager.py
--rw-r--r--   0        0        0    11745 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml_cli/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml_cli/py.typed
--rw-r--r--   0        0        0    16572 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml_cli/serve.py
--rw-r--r--   0        0        0    13280 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml_cli/start.py
--rw-r--r--   0        0        0    16723 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml_cli/utils.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml_cli/worker/README.md
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml_cli/worker/__init__.py
--rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml_cli/worker/grpc_api_server.py
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml_cli/worker/grpc_prometheus_server.py
--rw-r--r--   0        0        0     5465 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml_cli/worker/http_api_server.py
--rw-r--r--   0        0        0     5187 2020-02-02 00:00:00.000000 bentoml-1.1.0/src/bentoml_cli/worker/runner.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 bentoml-1.1.0/.gitignore
--rw-r--r--   0        0        0    11347 2020-02-02 00:00:00.000000 bentoml-1.1.0/LICENSE
--rw-r--r--   0        0        0     9857 2020-02-02 00:00:00.000000 bentoml-1.1.0/README.md
--rw-r--r--   0        0        0    12776 2020-02-02 00:00:00.000000 bentoml-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    14331 2020-02-02 00:00:00.000000 bentoml-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     7343 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/__init__.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/__main__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_version.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/batch.py
+-rw-r--r--   0        0        0    20111 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/bentos.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/catboost.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/client.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/cloud.py
+-rw-r--r--   0        0        0    16750 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/container.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/detectron.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/diffusers.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/easyocr.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/evalml.py
+-rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/exceptions.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/fastai.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/fasttext.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/flax.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/gluon.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/h2o.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/io.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/keras.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/lightgbm.py
+-rw-r--r--   0        0        0    15368 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/metrics.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/metrics.pyi
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/mlflow.py
+-rw-r--r--   0        0        0    11309 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/models.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/monitoring.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/onnx.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/onnxmlir.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/paddle.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/picklable_model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/py.typed
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/pycaret.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/pyspark.py
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/pytorch.py
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/pytorch_lightning.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/ray.py
+-rw-r--r--   0        0        0    30679 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/serve.py
+-rw-r--r--   0        0        0    15414 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/server.py
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/sklearn.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/spacy.py
+-rw-r--r--   0        0        0    14382 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/start.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/statsmodels.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/tensorflow.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/tensorflow_v1.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/torchscript.py
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/transformers.py
+-rw-r--r--   0        0        0     8328 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/triton.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/types.py
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/xgboost.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/__init__.py
+-rw-r--r--   0        0        0     7037 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/context.py
+-rw-r--r--   0        0        0    13916 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/exportable.py
+-rw-r--r--   0        0        0     4822 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/log.py
+-rw-r--r--   0        0        0     9725 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/resource.py
+-rw-r--r--   0        0        0     6625 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/store.py
+-rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/tag.py
+-rw-r--r--   0        0        0    10982 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/batch/__init__.py
+-rw-r--r--   0        0        0     5625 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/batch/spark.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/bento/__init__.py
+-rw-r--r--   0        0        0    20529 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/bento/bento.py
+-rw-r--r--   0        0        0    36144 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/bento/build_config.py
+-rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/bento/build_dev_bentoml_whl.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/bento/gen.py
+-rw-r--r--   0        0        0     4819 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/client/__init__.py
+-rw-r--r--   0        0        0    14468 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/client/grpc.py
+-rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/client/http.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/cloud/__init__.py
+-rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/cloud/base.py
+-rw-r--r--   0        0        0    43056 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/cloud/bentocloud.py
+-rw-r--r--   0        0        0    19538 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/cloud/client.py
+-rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/cloud/config.py
+-rw-r--r--   0        0        0    21890 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/cloud/deployment.py
+-rw-r--r--   0        0        0    19150 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/cloud/schemas.py
+-rw-r--r--   0        0        0    41949 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/cloud/yatai.py
+-rw-r--r--   0        0        0     6224 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/configuration/__init__.py
+-rw-r--r--   0        0        0    18788 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/configuration/containers.py
+-rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/configuration/helpers.py
+-rw-r--r--   0        0        0    11251 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/configuration/v1/__init__.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/configuration/v1/default_configuration.yaml
+-rw-r--r--   0        0        0    11401 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/container/__init__.py
+-rw-r--r--   0        0        0     7877 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/container/base.py
+-rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/container/buildah.py
+-rw-r--r--   0        0        0     5425 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/container/buildctl.py
+-rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/container/buildx.py
+-rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/container/docker.py
+-rw-r--r--   0        0        0     6881 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/container/generate.py
+-rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/container/nerdctl.py
+-rw-r--r--   0        0        0     4831 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/container/podman.py
+-rw-r--r--   0        0        0     5606 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/container/frontend/dockerfile/__init__.py
+-rwxr-xr-x   0        0        0     2522 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/container/frontend/dockerfile/entrypoint.sh
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/container/frontend/dockerfile/templates/_macros.j2
+-rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/container/frontend/dockerfile/templates/base.j2
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/container/frontend/dockerfile/templates/base_alpine.j2
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/container/frontend/dockerfile/templates/base_amazonlinux.j2
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/container/frontend/dockerfile/templates/base_debian.j2
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/container/frontend/dockerfile/templates/base_ubi8.j2
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/container/frontend/dockerfile/templates/cuda_debian.j2
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/container/frontend/dockerfile/templates/cuda_ubi8.j2
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/container/frontend/dockerfile/templates/miniconda_alpine.j2
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/container/frontend/dockerfile/templates/miniconda_debian.j2
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/container/frontend/dockerfile/templates/python_alpine.j2
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/container/frontend/dockerfile/templates/python_amazonlinux.j2
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/container/frontend/dockerfile/templates/python_debian.j2
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/container/frontend/dockerfile/templates/python_ubi8.j2
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/env_manager/__init__.py
+-rw-r--r--   0        0        0     4565 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/env_manager/envs.py
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/env_manager/manager.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/external_typing/__init__.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/external_typing/starlette.py
+-rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/external_typing/tensorflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/frameworks/__init__.py
+-rw-r--r--   0        0        0     9919 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/frameworks/catboost.py
+-rw-r--r--   0        0        0    12024 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/frameworks/detectron.py
+-rw-r--r--   0        0        0    24613 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/frameworks/diffusers.py
+-rw-r--r--   0        0        0     6837 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/frameworks/easyocr.py
+-rw-r--r--   0        0        0    11302 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/frameworks/fastai.py
+-rw-r--r--   0        0        0    12449 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/frameworks/flax.py
+-rw-r--r--   0        0        0    12576 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/frameworks/keras.py
+-rw-r--r--   0        0        0    10014 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/frameworks/lightgbm.py
+-rw-r--r--   0        0        0     9362 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/frameworks/mlflow.py
+-rw-r--r--   0        0        0    16612 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/frameworks/onnx.py
+-rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/frameworks/picklable.py
+-rw-r--r--   0        0        0     7527 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/frameworks/pytorch.py
+-rw-r--r--   0        0        0     7345 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/frameworks/pytorch_lightning.py
+-rw-r--r--   0        0        0     6750 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/frameworks/sklearn.py
+-rw-r--r--   0        0        0    15375 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/frameworks/tensorflow_v2.py
+-rw-r--r--   0        0        0     6828 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/frameworks/torchscript.py
+-rw-r--r--   0        0        0    36119 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/frameworks/transformers.py
+-rw-r--r--   0        0        0    11073 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/frameworks/xgboost.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/frameworks/common/__init__.py
+-rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/frameworks/common/jax.py
+-rw-r--r--   0        0        0     6745 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/frameworks/common/pytorch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/frameworks/utils/__init__.py
+-rw-r--r--   0        0        0     5192 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/frameworks/utils/onnx.py
+-rw-r--r--   0        0        0    17082 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/frameworks/utils/tensorflow.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/frameworks/utils/transformers.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/io_descriptors/__init__.py
+-rw-r--r--   0        0        0     5834 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/io_descriptors/base.py
+-rw-r--r--   0        0        0    13705 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/io_descriptors/file.py
+-rw-r--r--   0        0        0    19126 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/io_descriptors/image.py
+-rw-r--r--   0        0        0    18392 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/io_descriptors/json.py
+-rw-r--r--   0        0        0    13651 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/io_descriptors/multipart.py
+-rw-r--r--   0        0        0    24632 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/io_descriptors/numpy.py
+-rw-r--r--   0        0        0    49329 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/io_descriptors/pandas.py
+-rw-r--r--   0        0        0     5791 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/io_descriptors/text.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/marshal/__init__.py
+-rw-r--r--   0        0        0    14813 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/marshal/dispatcher.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/models/__init__.py
+-rw-r--r--   0        0        0    25400 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/models/model.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/monitoring/__init__.py
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/monitoring/api.py
+-rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/monitoring/base.py
+-rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/monitoring/default.py
+-rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/monitoring/otlp.py
+-rw-r--r--   0        0        0     7634 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/ray/__init__.py
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/ray/runner_handle.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/runner/__init__.py
+-rw-r--r--   0        0        0    24051 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/runner/container.py
+-rw-r--r--   0        0        0     4829 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/runner/runnable.py
+-rw-r--r--   0        0        0    12809 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/runner/runner.py
+-rw-r--r--   0        0        0     6778 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/runner/strategy.py
+-rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/runner/utils.py
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/runner/runner_handle/__init__.py
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/runner/runner_handle/local.py
+-rw-r--r--   0        0        0    19059 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/runner/runner_handle/remote.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/server/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/server/__init__.py
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/server/base_app.py
+-rw-r--r--   0        0        0    13583 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/server/grpc_app.py
+-rw-r--r--   0        0        0    16829 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/server/http_app.py
+-rw-r--r--   0        0        0    12258 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/server/runner_app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/server/grpc/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/server/grpc/servicer/__init__.py
+-rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/server/grpc/servicer/v1/__init__.py
+-rw-r--r--   0        0        0     5289 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/server/grpc/servicer/v1alpha1/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/server/http/__init__.py
+-rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/server/http/access.py
+-rw-r--r--   0        0        0     9114 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/server/http/instruments.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/server/http/traffic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/server/metrics/__init__.py
+-rw-r--r--   0        0        0     6192 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/server/metrics/prometheus.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/server/static_content/favicon-dark-32x32.png
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/server/static_content/favicon-light-32x32.png
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/server/static_content/index.css
+-rw-r--r--   0        0        0    36011 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/server/static_content/marked.min.js
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/server/static_content/swagger-initializer.js
+-rw-r--r--   0        0        0  1096221 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/server/static_content/swagger-ui-bundle.js
+-rw-r--r--   0        0        0   339540 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/server/static_content/swagger-ui-standalone-preset.js
+-rw-r--r--   0        0        0   143980 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/server/static_content/swagger-ui.css
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/service/__init__.py
+-rw-r--r--   0        0        0     7141 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/service/inference_api.py
+-rw-r--r--   0        0        0    14652 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/service/loader.py
+-rw-r--r--   0        0        0    17745 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/service/service.py
+-rw-r--r--   0        0        0     6394 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/service/openapi/__init__.py
+-rw-r--r--   0        0        0     9879 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/service/openapi/specification.py
+-rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/service/openapi/utils.py
+-rw-r--r--   0        0        0    15903 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/utils/__init__.py
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/utils/alg.py
+-rw-r--r--   0        0        0    13986 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/utils/benchmark.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/utils/buildx.py
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/utils/cattr.py
+-rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/utils/dotenv.py
+-rw-r--r--   0        0        0    14318 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/utils/formparser.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/utils/http.py
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/utils/lazy_loader.py
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/utils/metrics.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/utils/pickle.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/utils/pkg.py
+-rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/utils/telemetry.py
+-rw-r--r--   0        0        0     7614 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/utils/unflatten.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/utils/uri.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/utils/analytics/__init__.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/utils/analytics/cli_events.py
+-rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/utils/analytics/schemas.py
+-rw-r--r--   0        0        0    10371 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/utils/analytics/usage_stats.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/utils/circus/__init__.py
+-rw-r--r--   0        0        0     4628 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/_internal/utils/circus/watchfilesplugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/grpc/__init__.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/grpc/buf.yaml
+-rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/grpc/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/grpc/interceptors/__init__.py
+-rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/grpc/interceptors/access.py
+-rw-r--r--   0        0        0    10292 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/grpc/interceptors/opentelemetry.py
+-rw-r--r--   0        0        0     5522 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/grpc/interceptors/prometheus.py
+-rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/grpc/utils/__init__.py
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/grpc/utils/_import_hook.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/grpc/v1/__init__.py
+-rw-r--r--   0        0        0     9391 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/grpc/v1/service.proto
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/grpc/v1/service_pb2.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/grpc/v1/service_pb2.pyi
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/grpc/v1/service_pb2_grpc.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/grpc/v1/service_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/grpc/v1/_generated_pb3/__init__.py
+-rw-r--r--   0        0        0    14406 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/grpc/v1/_generated_pb3/service_pb2.py
+-rw-r--r--   0        0        0    28650 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/grpc/v1/_generated_pb3/service_pb2.pyi
+-rw-r--r--   0        0        0     4274 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/grpc/v1/_generated_pb3/service_pb2_grpc.py
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/grpc/v1/_generated_pb3/service_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/grpc/v1/_generated_pb4/__init__.py
+-rw-r--r--   0        0        0     9598 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/grpc/v1/_generated_pb4/service_pb2.py
+-rw-r--r--   0        0        0    29161 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/grpc/v1/_generated_pb4/service_pb2.pyi
+-rw-r--r--   0        0        0     4274 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/grpc/v1/_generated_pb4/service_pb2_grpc.py
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/grpc/v1/_generated_pb4/service_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/grpc/v1alpha1/__init__.py
+-rw-r--r--   0        0        0     8488 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/grpc/v1alpha1/service.proto
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/grpc/v1alpha1/service_pb2.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/grpc/v1alpha1/service_pb2.pyi
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/grpc/v1alpha1/service_pb2_grpc.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/grpc/v1alpha1/service_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/grpc/v1alpha1/_generated_pb3/__init__.py
+-rw-r--r--   0        0        0    12103 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/grpc/v1alpha1/_generated_pb3/service_pb2.py
+-rw-r--r--   0        0        0    24953 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/grpc/v1alpha1/_generated_pb3/service_pb2.pyi
+-rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/grpc/v1alpha1/_generated_pb3/service_pb2_grpc.py
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/grpc/v1alpha1/_generated_pb3/service_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/grpc/v1alpha1/_generated_pb4/__init__.py
+-rw-r--r--   0        0        0     8916 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/grpc/v1alpha1/_generated_pb4/service_pb2.py
+-rw-r--r--   0        0        0    25248 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/grpc/v1alpha1/_generated_pb4/service_pb2.pyi
+-rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/grpc/v1alpha1/_generated_pb4/service_pb2_grpc.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/grpc/v1alpha1/_generated_pb4/service_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/testing/__init__.py
+-rw-r--r--   0        0        0    18696 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/testing/server.py
+-rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/testing/utils.py
+-rw-r--r--   0        0        0     8397 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/testing/grpc/__init__.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/testing/pytest/__init__.py
+-rw-r--r--   0        0        0    10433 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml/testing/pytest/plugin.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml_cli/__init__.py
+-rw-r--r--   0        0        0    15555 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml_cli/bentos.py
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml_cli/cli.py
+-rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml_cli/cloud.py
+-rw-r--r--   0        0        0    23294 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml_cli/containerize.py
+-rw-r--r--   0        0        0    10703 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml_cli/deployment.py
+-rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml_cli/env.py
+-rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml_cli/env_manager.py
+-rw-r--r--   0        0        0    11745 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml_cli/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml_cli/py.typed
+-rw-r--r--   0        0        0    16572 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml_cli/serve.py
+-rw-r--r--   0        0        0    13280 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml_cli/start.py
+-rw-r--r--   0        0        0    16723 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml_cli/utils.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml_cli/worker/README.md
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml_cli/worker/__init__.py
+-rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml_cli/worker/grpc_api_server.py
+-rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml_cli/worker/grpc_prometheus_server.py
+-rw-r--r--   0        0        0     5465 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml_cli/worker/http_api_server.py
+-rw-r--r--   0        0        0     5187 2020-02-02 00:00:00.000000 bentoml-1.1.1/src/bentoml_cli/worker/runner.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 bentoml-1.1.1/.gitignore
+-rw-r--r--   0        0        0    11347 2020-02-02 00:00:00.000000 bentoml-1.1.1/LICENSE
+-rw-r--r--   0        0        0     9857 2020-02-02 00:00:00.000000 bentoml-1.1.1/README.md
+-rw-r--r--   0        0        0    12751 2020-02-02 00:00:00.000000 bentoml-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0    14331 2020-02-02 00:00:00.000000 bentoml-1.1.1/PKG-INFO
```

### Comparing `bentoml-1.1.0/src/bentoml/__init__.py` & `bentoml-1.1.1/src/bentoml/__init__.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/bentos.py` & `bentoml-1.1.1/src/bentoml/bentos.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/container.py` & `bentoml-1.1.1/src/bentoml/container.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/exceptions.py` & `bentoml-1.1.1/src/bentoml/exceptions.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/io.py` & `bentoml-1.1.1/src/bentoml/io.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/keras.py` & `bentoml-1.1.1/src/bentoml/keras.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/lightgbm.py` & `bentoml-1.1.1/src/bentoml/lightgbm.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/metrics.py` & `bentoml-1.1.1/src/bentoml/metrics.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/metrics.pyi` & `bentoml-1.1.1/src/bentoml/metrics.pyi`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/models.py` & `bentoml-1.1.1/src/bentoml/models.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/onnx.py` & `bentoml-1.1.1/src/bentoml/onnx.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/pytorch.py` & `bentoml-1.1.1/src/bentoml/pytorch.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/pytorch_lightning.py` & `bentoml-1.1.1/src/bentoml/pytorch_lightning.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/serve.py` & `bentoml-1.1.1/src/bentoml/serve.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/server.py` & `bentoml-1.1.1/src/bentoml/server.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/sklearn.py` & `bentoml-1.1.1/src/bentoml/sklearn.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/start.py` & `bentoml-1.1.1/src/bentoml/start.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/tensorflow.py` & `bentoml-1.1.1/src/bentoml/tensorflow.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/torchscript.py` & `bentoml-1.1.1/src/bentoml/torchscript.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/transformers.py` & `bentoml-1.1.1/src/bentoml/transformers.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/triton.py` & `bentoml-1.1.1/src/bentoml/triton.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/xgboost.py` & `bentoml-1.1.1/src/bentoml/xgboost.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/context.py` & `bentoml-1.1.1/src/bentoml/_internal/context.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/exportable.py` & `bentoml-1.1.1/src/bentoml/_internal/exportable.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/log.py` & `bentoml-1.1.1/src/bentoml/_internal/log.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/resource.py` & `bentoml-1.1.1/src/bentoml/_internal/resource.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/store.py` & `bentoml-1.1.1/src/bentoml/_internal/store.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/tag.py` & `bentoml-1.1.1/src/bentoml/_internal/tag.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/types.py` & `bentoml-1.1.1/src/bentoml/_internal/types.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/batch/spark.py` & `bentoml-1.1.1/src/bentoml/_internal/batch/spark.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/bento/bento.py` & `bentoml-1.1.1/src/bentoml/_internal/bento/bento.py`

 * *Files 0% similar despite different names*

```diff
@@ -445,15 +445,15 @@
 @attr.frozen
 class BentoApiInfo:
     name: str
     input_type: str
     output_type: str
 
     @classmethod
-    def from_inference_api(cls, api: InferenceAPI) -> BentoApiInfo:
+    def from_inference_api(cls, api: InferenceAPI[t.Any]) -> BentoApiInfo:
         return cls(
             name=api.name,
             input_type=api.input.__class__.__name__,
             output_type=api.output.__class__.__name__,
         )
```

### Comparing `bentoml-1.1.0/src/bentoml/_internal/bento/build_config.py` & `bentoml-1.1.1/src/bentoml/_internal/bento/build_config.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/bento/build_dev_bentoml_whl.py` & `bentoml-1.1.1/src/bentoml/_internal/bento/build_dev_bentoml_whl.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/bento/gen.py` & `bentoml-1.1.1/src/bentoml/_internal/bento/gen.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/client/__init__.py` & `bentoml-1.1.1/src/bentoml/_internal/client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,21 +124,21 @@
             return GrpcClient.from_url(server_url, **kwargs)
         else:
             raise BentoMLException(
                 f"Invalid client kind '{kind}'. Must be one of 'http', 'grpc', or 'auto'."
             )
 
     def _sync_call(
-        self, inp: t.Any = None, *, _bentoml_api: InferenceAPI, **kwargs: t.Any
+        self, inp: t.Any = None, *, _bentoml_api: InferenceAPI[t.Any], **kwargs: t.Any
     ):
         return asyncio.run(self._call(inp, _bentoml_api=_bentoml_api, **kwargs))
 
     @abstractmethod
     async def _call(
-        self, inp: t.Any = None, *, _bentoml_api: InferenceAPI, **kwargs: t.Any
+        self, inp: t.Any = None, *, _bentoml_api: InferenceAPI[t.Any], **kwargs: t.Any
     ) -> t.Any:
         raise NotImplementedError
 
     def __enter__(self):
         return self
 
     def __exit__(
```

### Comparing `bentoml-1.1.0/src/bentoml/_internal/client/grpc.py` & `bentoml-1.1.1/src/bentoml/_internal/client/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -257,15 +257,15 @@
             rpc(metadata["input_type"](**attrs), **channel_kwargs),
         )
 
     async def _call(
         self,
         inp: t.Any = None,
         *,
-        _bentoml_api: InferenceAPI,
+        _bentoml_api: InferenceAPI[t.Any],
         **attrs: t.Any,
     ) -> t.Any:
         state = self.channel.get_state(try_to_connect=True)
         if state != grpc.ChannelConnectivity.READY:
             # create a blocking call to wait til channel is ready.
             await self.channel.channel_ready()
 
@@ -358,15 +358,15 @@
                     response_deserializer=pb.ServiceMetadataResponse.FromString,
                 )(pb.ServiceMetadataRequest()),
             )
         dummy_service = Service(metadata.name)
 
         for api in metadata.apis:
             try:
-                dummy_service.apis[api.name] = InferenceAPI(
+                dummy_service.apis[api.name] = InferenceAPI[t.Any](
                     None,
                     io_descriptors.from_spec(
                         {
                             "id": api.input.descriptor_id,
                             "args": _json_format.MessageToDict(
                                 api.input.attributes
                             ).get("args", None),
```

### Comparing `bentoml-1.1.0/src/bentoml/_internal/client/http.py` & `bentoml-1.1.1/src/bentoml/_internal/client/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
                             f"Malformed BentoML spec received from BentoML server {server_url}"
                         )
                     if "x-bentoml-name" not in meth_spec:
                         raise BentoMLException(
                             f"Malformed BentoML spec received from BentoML server {server_url}"
                         )
                     try:
-                        api = InferenceAPI(
+                        api = InferenceAPI[t.Any](
                             None,
                             io.from_spec(
                                 meth_spec["requestBody"]["x-bentoml-io-descriptor"]
                             ),
                             io.from_spec(
                                 meth_spec["responses"]["200"]["x-bentoml-io-descriptor"]
                             ),
@@ -141,15 +141,15 @@
                             meth_spec["x-bentoml-name"],
                             e,
                         )
 
         return cls(dummy_service, server_url)
 
     async def _call(
-        self, inp: t.Any = None, *, _bentoml_api: InferenceAPI, **kwargs: t.Any
+        self, inp: t.Any = None, *, _bentoml_api: InferenceAPI[t.Any], **kwargs: t.Any
     ) -> t.Any:
         # All gRPC kwargs should be poped out.
         kwargs = {k: v for k, v in kwargs.items() if not k.startswith("_grpc_")}
         api = _bentoml_api
 
         if api.multi_input:
             if inp is not None:
```

### Comparing `bentoml-1.1.0/src/bentoml/_internal/cloud/base.py` & `bentoml-1.1.1/src/bentoml/_internal/cloud/base.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/cloud/bentocloud.py` & `bentoml-1.1.1/src/bentoml/_internal/cloud/bentocloud.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/cloud/client.py` & `bentoml-1.1.1/src/bentoml/_internal/cloud/client.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/cloud/config.py` & `bentoml-1.1.1/src/bentoml/_internal/cloud/config.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/cloud/deployment.py` & `bentoml-1.1.1/src/bentoml/_internal/cloud/deployment.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/cloud/schemas.py` & `bentoml-1.1.1/src/bentoml/_internal/cloud/schemas.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/cloud/yatai.py` & `bentoml-1.1.1/src/bentoml/_internal/cloud/yatai.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/configuration/__init__.py` & `bentoml-1.1.1/src/bentoml/_internal/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/configuration/containers.py` & `bentoml-1.1.1/src/bentoml/_internal/configuration/containers.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/configuration/helpers.py` & `bentoml-1.1.1/src/bentoml/_internal/configuration/helpers.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/configuration/v1/__init__.py` & `bentoml-1.1.1/src/bentoml/_internal/configuration/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/configuration/v1/default_configuration.yaml` & `bentoml-1.1.1/src/bentoml/_internal/configuration/v1/default_configuration.yaml`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/container/__init__.py` & `bentoml-1.1.1/src/bentoml/_internal/container/__init__.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/container/base.py` & `bentoml-1.1.1/src/bentoml/_internal/container/base.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/container/buildah.py` & `bentoml-1.1.1/src/bentoml/_internal/container/buildah.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/container/buildctl.py` & `bentoml-1.1.1/src/bentoml/_internal/container/buildctl.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/container/buildx.py` & `bentoml-1.1.1/src/bentoml/_internal/container/buildx.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/container/docker.py` & `bentoml-1.1.1/src/bentoml/_internal/container/docker.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/container/generate.py` & `bentoml-1.1.1/src/bentoml/_internal/container/generate.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/container/nerdctl.py` & `bentoml-1.1.1/src/bentoml/_internal/container/nerdctl.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/container/podman.py` & `bentoml-1.1.1/src/bentoml/_internal/container/podman.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/container/frontend/dockerfile/__init__.py` & `bentoml-1.1.1/src/bentoml/_internal/container/frontend/dockerfile/__init__.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/container/frontend/dockerfile/entrypoint.sh` & `bentoml-1.1.1/src/bentoml/_internal/container/frontend/dockerfile/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/container/frontend/dockerfile/templates/_macros.j2` & `bentoml-1.1.1/src/bentoml/_internal/container/frontend/dockerfile/templates/_macros.j2`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/container/frontend/dockerfile/templates/base.j2` & `bentoml-1.1.1/src/bentoml/_internal/container/frontend/dockerfile/templates/base.j2`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/container/frontend/dockerfile/templates/base_alpine.j2` & `bentoml-1.1.1/src/bentoml/_internal/container/frontend/dockerfile/templates/base_alpine.j2`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/container/frontend/dockerfile/templates/base_amazonlinux.j2` & `bentoml-1.1.1/src/bentoml/_internal/container/frontend/dockerfile/templates/base_amazonlinux.j2`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/container/frontend/dockerfile/templates/base_debian.j2` & `bentoml-1.1.1/src/bentoml/_internal/container/frontend/dockerfile/templates/base_debian.j2`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/container/frontend/dockerfile/templates/base_ubi8.j2` & `bentoml-1.1.1/src/bentoml/_internal/container/frontend/dockerfile/templates/base_ubi8.j2`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/container/frontend/dockerfile/templates/cuda_debian.j2` & `bentoml-1.1.1/src/bentoml/_internal/container/frontend/dockerfile/templates/cuda_debian.j2`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/container/frontend/dockerfile/templates/cuda_ubi8.j2` & `bentoml-1.1.1/src/bentoml/_internal/container/frontend/dockerfile/templates/cuda_ubi8.j2`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/env_manager/envs.py` & `bentoml-1.1.1/src/bentoml/_internal/env_manager/envs.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/env_manager/manager.py` & `bentoml-1.1.1/src/bentoml/_internal/env_manager/manager.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/external_typing/__init__.py` & `bentoml-1.1.1/src/bentoml/_internal/external_typing/__init__.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/external_typing/starlette.py` & `bentoml-1.1.1/src/bentoml/_internal/external_typing/starlette.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/external_typing/tensorflow.py` & `bentoml-1.1.1/src/bentoml/_internal/external_typing/tensorflow.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/frameworks/catboost.py` & `bentoml-1.1.1/src/bentoml/_internal/frameworks/catboost.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/frameworks/detectron.py` & `bentoml-1.1.1/src/bentoml/_internal/frameworks/detectron.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/frameworks/diffusers.py` & `bentoml-1.1.1/src/bentoml/_internal/frameworks/diffusers.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/frameworks/easyocr.py` & `bentoml-1.1.1/src/bentoml/_internal/frameworks/easyocr.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/frameworks/fastai.py` & `bentoml-1.1.1/src/bentoml/_internal/frameworks/fastai.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/frameworks/flax.py` & `bentoml-1.1.1/src/bentoml/_internal/frameworks/flax.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/frameworks/keras.py` & `bentoml-1.1.1/src/bentoml/_internal/frameworks/keras.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/frameworks/lightgbm.py` & `bentoml-1.1.1/src/bentoml/_internal/frameworks/lightgbm.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/frameworks/mlflow.py` & `bentoml-1.1.1/src/bentoml/_internal/frameworks/mlflow.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/frameworks/onnx.py` & `bentoml-1.1.1/src/bentoml/_internal/frameworks/onnx.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/frameworks/picklable.py` & `bentoml-1.1.1/src/bentoml/_internal/frameworks/picklable.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/frameworks/pytorch.py` & `bentoml-1.1.1/src/bentoml/_internal/frameworks/pytorch.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/frameworks/pytorch_lightning.py` & `bentoml-1.1.1/src/bentoml/_internal/frameworks/pytorch_lightning.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/frameworks/sklearn.py` & `bentoml-1.1.1/src/bentoml/_internal/frameworks/sklearn.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/frameworks/tensorflow_v2.py` & `bentoml-1.1.1/src/bentoml/_internal/frameworks/tensorflow_v2.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/frameworks/torchscript.py` & `bentoml-1.1.1/src/bentoml/_internal/frameworks/torchscript.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/frameworks/transformers.py` & `bentoml-1.1.1/src/bentoml/_internal/frameworks/transformers.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/frameworks/xgboost.py` & `bentoml-1.1.1/src/bentoml/_internal/frameworks/xgboost.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/frameworks/common/jax.py` & `bentoml-1.1.1/src/bentoml/_internal/frameworks/common/jax.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/frameworks/common/pytorch.py` & `bentoml-1.1.1/src/bentoml/_internal/frameworks/common/pytorch.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/frameworks/utils/onnx.py` & `bentoml-1.1.1/src/bentoml/_internal/frameworks/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/frameworks/utils/tensorflow.py` & `bentoml-1.1.1/src/bentoml/_internal/frameworks/utils/tensorflow.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/frameworks/utils/transformers.py` & `bentoml-1.1.1/src/bentoml/_internal/frameworks/utils/transformers.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/io_descriptors/__init__.py` & `bentoml-1.1.1/src/bentoml/_internal/io_descriptors/__init__.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/io_descriptors/base.py` & `bentoml-1.1.1/src/bentoml/_internal/io_descriptors/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -132,14 +132,20 @@
     def sample(self) -> IOType | None:
         return self._sample
 
     @sample.setter
     def sample(self, value: IOType) -> None:
         self._sample = value
 
+    if t.TYPE_CHECKING:
+
+        @classmethod
+        def from_sample(cls, sample: t.Any, **attrs: t.Any) -> t.Self:
+            ...
+
     @abstractmethod
     def _from_sample(self, sample: t.Any) -> IOType:
         """
         Creates a new instance of the IO Descriptor from given sample.
 
         Args:
             sample: The sample to create the instance from.
```

### Comparing `bentoml-1.1.0/src/bentoml/_internal/io_descriptors/file.py` & `bentoml-1.1.1/src/bentoml/_internal/io_descriptors/file.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/io_descriptors/image.py` & `bentoml-1.1.1/src/bentoml/_internal/io_descriptors/image.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/io_descriptors/json.py` & `bentoml-1.1.1/src/bentoml/_internal/io_descriptors/json.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/io_descriptors/multipart.py` & `bentoml-1.1.1/src/bentoml/_internal/io_descriptors/multipart.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/io_descriptors/numpy.py` & `bentoml-1.1.1/src/bentoml/_internal/io_descriptors/numpy.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/io_descriptors/pandas.py` & `bentoml-1.1.1/src/bentoml/_internal/io_descriptors/pandas.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/io_descriptors/text.py` & `bentoml-1.1.1/src/bentoml/_internal/io_descriptors/text.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/marshal/dispatcher.py` & `bentoml-1.1.1/src/bentoml/_internal/marshal/dispatcher.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/models/__init__.py` & `bentoml-1.1.1/src/bentoml/_internal/models/__init__.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/models/model.py` & `bentoml-1.1.1/src/bentoml/_internal/models/model.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/monitoring/__init__.py` & `bentoml-1.1.1/src/bentoml/_internal/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/monitoring/api.py` & `bentoml-1.1.1/src/bentoml/_internal/monitoring/api.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/monitoring/base.py` & `bentoml-1.1.1/src/bentoml/_internal/monitoring/base.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/monitoring/default.py` & `bentoml-1.1.1/src/bentoml/_internal/monitoring/default.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/monitoring/otlp.py` & `bentoml-1.1.1/src/bentoml/_internal/monitoring/otlp.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/ray/__init__.py` & `bentoml-1.1.1/src/bentoml/_internal/ray/__init__.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/ray/runner_handle.py` & `bentoml-1.1.1/src/bentoml/_internal/ray/runner_handle.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/runner/container.py` & `bentoml-1.1.1/src/bentoml/_internal/runner/container.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/runner/runnable.py` & `bentoml-1.1.1/src/bentoml/_internal/runner/runnable.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/runner/runner.py` & `bentoml-1.1.1/src/bentoml/_internal/runner/runner.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/runner/strategy.py` & `bentoml-1.1.1/src/bentoml/_internal/runner/strategy.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/runner/utils.py` & `bentoml-1.1.1/src/bentoml/_internal/runner/utils.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/runner/runner_handle/__init__.py` & `bentoml-1.1.1/src/bentoml/_internal/runner/runner_handle/__init__.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/runner/runner_handle/local.py` & `bentoml-1.1.1/src/bentoml/_internal/runner/runner_handle/local.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/runner/runner_handle/remote.py` & `bentoml-1.1.1/src/bentoml/_internal/runner/runner_handle/remote.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/server/README.md` & `bentoml-1.1.1/src/bentoml/_internal/server/README.md`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/server/base_app.py` & `bentoml-1.1.1/src/bentoml/_internal/server/base_app.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/server/grpc_app.py` & `bentoml-1.1.1/src/bentoml/_internal/server/grpc_app.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/server/http_app.py` & `bentoml-1.1.1/src/bentoml/_internal/server/http_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,15 +305,15 @@
         app = super().__call__()
         for mount_app, path, name in self.bento_service.mount_apps:
             app.mount(app=mount_app, path=path, name=name)
         return app
 
     def _create_api_endpoint(
         self,
-        api: InferenceAPI,
+        api: InferenceAPI[t.Any],
     ) -> t.Callable[[Request], t.Coroutine[t.Any, t.Any, Response]]:
         """
         Create api function for starlette route, it wraps around user defined API
         callback and adapter class, and adds request logging and instrument metrics
         """
         from starlette.concurrency import run_in_threadpool  # type: ignore
         from starlette.responses import JSONResponse
```

### Comparing `bentoml-1.1.0/src/bentoml/_internal/server/runner_app.py` & `bentoml-1.1.1/src/bentoml/_internal/server/runner_app.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/server/grpc/servicer/v1/__init__.py` & `bentoml-1.1.1/src/bentoml/_internal/server/grpc/servicer/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/server/grpc/servicer/v1alpha1/__init__.py` & `bentoml-1.1.1/src/bentoml/_internal/server/grpc/servicer/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/server/http/access.py` & `bentoml-1.1.1/src/bentoml/_internal/server/http/access.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/server/http/instruments.py` & `bentoml-1.1.1/src/bentoml/_internal/server/http/instruments.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/server/http/traffic.py` & `bentoml-1.1.1/src/bentoml/_internal/server/http/traffic.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/server/metrics/prometheus.py` & `bentoml-1.1.1/src/bentoml/_internal/server/metrics/prometheus.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/server/static_content/favicon-dark-32x32.png` & `bentoml-1.1.1/src/bentoml/_internal/server/static_content/favicon-dark-32x32.png`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/server/static_content/favicon-light-32x32.png` & `bentoml-1.1.1/src/bentoml/_internal/server/static_content/favicon-light-32x32.png`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/server/static_content/index.css` & `bentoml-1.1.1/src/bentoml/_internal/server/static_content/index.css`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/server/static_content/marked.min.js` & `bentoml-1.1.1/src/bentoml/_internal/server/static_content/marked.min.js`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/server/static_content/swagger-ui-bundle.js` & `bentoml-1.1.1/src/bentoml/_internal/server/static_content/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/server/static_content/swagger-ui-standalone-preset.js` & `bentoml-1.1.1/src/bentoml/_internal/server/static_content/swagger-ui-standalone-preset.js`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/server/static_content/swagger-ui.css` & `bentoml-1.1.1/src/bentoml/_internal/server/static_content/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/service/inference_api.py` & `bentoml-1.1.1/src/bentoml/_internal/service/inference_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 from __future__ import annotations
 
 import inspect
 import re
 import typing as t
-from typing import Optional
 
 import yaml
 
 from ...exceptions import InvalidArgument
 from ..context import ServiceContext as Context
 from ..io_descriptors import IODescriptor
+from ..io_descriptors.base import IOType
 from ..types import is_compatible_type
 
 RESERVED_API_NAMES = [
     "index",
     "swagger",
     "docs",
     "metrics",
     "healthz",
     "livez",
     "readyz",
 ]
 
 
-class InferenceAPI:
+class InferenceAPI(t.Generic[IOType]):
     def __init__(
         self,
         user_defined_callback: t.Callable[..., t.Any] | None,
-        input_descriptor: IODescriptor[t.Any],
-        output_descriptor: IODescriptor[t.Any],
-        name: Optional[str],
-        doc: Optional[str] = None,
-        route: Optional[str] = None,
+        input_descriptor: IODescriptor[IOType],
+        output_descriptor: IODescriptor[IOType],
+        name: str | None,
+        doc: str | None = None,
+        route: str | None = None,
     ):
         if user_defined_callback is not None:
             # Use user_defined_callback function variable if name not specified
             name = user_defined_callback.__name__ if name is None else name
             # Use user_defined_callback function docstring `__doc__` if doc not specified
             doc = user_defined_callback.__doc__ if doc is None else doc
         else:
@@ -173,15 +173,15 @@
             )
         if route in RESERVED_API_NAMES:
             raise InvalidArgument(
                 "Reserved API route: '{}' is reserved for infra endpoints".format(route)
             )
 
 
-def _InferenceAPI_dumper(dumper: yaml.Dumper, api: InferenceAPI) -> yaml.Node:
+def _InferenceAPI_dumper(dumper: yaml.Dumper, api: InferenceAPI[t.Any]) -> yaml.Node:
     return dumper.represent_dict(
         {
             "route": api.route,
             "doc": api.doc,
             "input": api.input.__class__.__name__,
             "output": api.output.__class__.__name__,
         }
```

### Comparing `bentoml-1.1.0/src/bentoml/_internal/service/loader.py` & `bentoml-1.1.1/src/bentoml/_internal/service/loader.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/service/service.py` & `bentoml-1.1.1/src/bentoml/_internal/service/service.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,77 +3,68 @@
 import importlib
 import inspect
 import logging
 import os
 import sys
 import typing as t
 from functools import partial
-from typing import TYPE_CHECKING
 
 import attr
 
 from bentoml.exceptions import BentoMLException
 
 from ...exceptions import NotFound
 from ...grpc.utils import LATEST_PROTOCOL_VERSION
 from ...grpc.utils import import_grpc
 from ..bento.bento import get_default_svc_readme
 from ..context import ServiceContext as Context
 from ..io_descriptors import IODescriptor
+from ..io_descriptors.base import IOType
 from ..models import Model
 from ..runner.runner import AbstractRunner
 from ..runner.runner import Runner
 from ..tag import Tag
+from ..utils import first_not_none
 from .inference_api import InferenceAPI
 
-if TYPE_CHECKING:
+if t.TYPE_CHECKING:
     import grpc
 
+    import bentoml
     from bentoml.grpc.types import AddServicerFn
     from bentoml.grpc.types import ServicerClass
 
     from ...grpc.v1 import service_pb2_grpc as services
     from .. import external_typing as ext
     from ..bento import Bento
     from ..types import LifecycleHook
     from .openapi.specification import OpenAPISpecification
 
     ContextFunc = t.Callable[[Context], None | t.Coroutine[t.Any, t.Any, None]]
     HookF = t.TypeVar("HookF", bound=LifecycleHook)
     HookF_ctx = t.TypeVar("HookF_ctx", bound=ContextFunc)
-else:
-    grpc, _ = import_grpc()
 
-logger = logging.getLogger(__name__)
+    class _inference_api_wrapper(t.Generic[IOType]):
+        __name__: str
 
+        # fmt: off
+        @t.overload
+        def __call__(self, func: t.Callable[[IOType], IOType]) -> t.Callable[[IOType], IOType]: ...  # type: ignore (this is considered as stub)
+        @t.overload
+        def __call__(self, func: t.Callable[[IOType], t.Coroutine[IOType, t.Any, t.Any]]) -> t.Callable[[IOType], t.Coroutine[IOType, t.Any, t.Any]]: ...
+        @t.overload
+        def __call__(self, func: t.Callable[[IOType, bentoml.Context], IOType]) -> t.Callable[[IOType, bentoml.Context], IOType]: ...
+        @t.overload
+        def __call__(self, func: t.Callable[[IOType, bentoml.Context], t.Coroutine[IOType, t.Any, t.Any]]) -> t.Callable[[IOType, bentoml.Context], t.Coroutine[IOType, t.Any, t.Any]]: ...
+        # fmt: on
 
-def add_inference_api(
-    svc: Service,
-    func: t.Callable[..., t.Any],
-    input: IODescriptor[t.Any],  # pylint: disable=redefined-builtin
-    output: IODescriptor[t.Any],
-    name: t.Optional[str],
-    doc: t.Optional[str],
-    route: t.Optional[str],
-) -> None:
-    api = InferenceAPI(
-        name=name if name is not None else func.__name__,
-        user_defined_callback=func,
-        input_descriptor=input,
-        output_descriptor=output,
-        doc=doc,
-        route=route,
-    )
-
-    if api.name in svc.apis:
-        raise BentoMLException(
-            f"API {api.name} is already defined in Service {svc.name}"
-        )
+else:
+    grpc, _ = import_grpc()
 
-    svc.apis[api.name] = api
+logger = logging.getLogger(__name__)
 
 
 def get_valid_service_name(user_provided_svc_name: str) -> str:
     lower_name = user_provided_svc_name.lower()
 
     if user_provided_svc_name != lower_name:
         logger.warning(
@@ -81,15 +72,15 @@
         )
 
     # Service name must be a valid Tag name; create a dummy tag to use its validation
     Tag(lower_name)
     return lower_name
 
 
-@attr.define(frozen=True)
+@attr.define(frozen=False, init=False)
 class Service:
     """The service definition is the manifestation of the Service Oriented Architecture
     and the core building block in BentoML where users define the service runtime
     architecture and model serving logic.
 
     A BentoML service is defined via instantiate this Service class. When creating a
     Service instance, user must provide a Service name and list of runners that are
@@ -115,15 +106,15 @@
     )
     interceptors: list[partial[grpc.aio.ServerInterceptor]] = attr.field(
         init=False, factory=list
     )
     grpc_handlers: list[grpc.GenericRpcHandler] = attr.field(init=False, factory=list)
 
     # list of APIs from @svc.api
-    apis: t.Dict[str, InferenceAPI] = attr.field(init=False, factory=dict)
+    apis: t.Dict[str, InferenceAPI[t.Any]] = attr.field(init=False, factory=dict)
 
     # Tag/Bento are only set when the service was loaded from a bento
     tag: Tag | None = attr.field(init=False, default=None)
     bento: Bento | None = attr.field(init=False, default=None)
 
     # Working dir and Import path of the service, set when the service was imported
     _working_dir: str | None = attr.field(init=False, default=None)
@@ -205,20 +196,20 @@
     def __init__(
         self,
         name: str,
         *,
         runners: list[AbstractRunner] | None = None,
         models: list[Model] | None = None,
     ):
-        """
+        """Service definition itself. Runners and models can be optionally pass into a ``bentoml.Service``.
 
         Args:
-            name:
-            runners:
-            models:
+            name: name of the service
+            runners: Optional list of runners to be used with this service.
+            models: Optional list of ``bentoml.Model`` to be used with this service.
         """
         name = get_valid_service_name(name)
 
         # validate runners list contains Runner instances and runner names are unique
         if runners is not None:
             runner_names: t.Set[str] = set()
             for r in runners:
@@ -246,16 +237,16 @@
         )
 
         # Set import origin info - import_str can not be determined at this stage yet as
         # the variable name is only available in module vars after __init__ is returned
         # get_service_import_origin below will use the _caller_module for retriving the
         # correct import_str for this service
         caller_module = inspect.currentframe().f_back.f_globals["__name__"]
-        object.__setattr__(self, "_caller_module", caller_module)
-        object.__setattr__(self, "_working_dir", os.getcwd())
+        self._caller_module = caller_module
+        self._working_dir = os.getcwd()
 
     def get_service_import_origin(self) -> tuple[str, str]:
         """
         Returns the module name and working directory of the service
         """
         if not self._import_str:
             import_module = self._caller_module
@@ -289,31 +280,52 @@
     def is_service_importable(self) -> bool:
         if self._caller_module == "__main__":
             if not hasattr(sys.modules["__main__"], "__file__"):
                 return False
 
         return True
 
+    # fmt: off
+    # case 1: function is not defined, but input and output are
+    @t.overload
+    def api(self, input: IODescriptor[IOType], output: IODescriptor[IOType]) ->  _inference_api_wrapper[IOType]: ...
+    # case 2: the decorator itself with custom routes
+    @t.overload
+    def api(self, input: IODescriptor[IOType], output: IODescriptor[IOType], *, route: str = ...) ->  _inference_api_wrapper[IOType]: ...
+    # fmt: on
     def api(
         self,
-        input: IODescriptor[t.Any],  # pylint: disable=redefined-builtin
-        output: IODescriptor[t.Any],
-        name: t.Optional[str] = None,
-        doc: t.Optional[str] = None,
-        route: t.Optional[str] = None,
-    ) -> t.Callable[[t.Callable[..., t.Any]], t.Callable[..., t.Any]]:
+        input: IODescriptor[IOType],
+        output: IODescriptor[IOType],
+        *,
+        name: str | None = None,
+        doc: str | None = None,
+        route: str | None = None,
+    ) -> _inference_api_wrapper[IOType]:
         """Decorator for adding InferenceAPI to this service"""
 
-        D = t.TypeVar("D", bound=t.Callable[..., t.Any])
-
-        def decorator(func: D) -> D:
-            add_inference_api(self, func, input, output, name, doc, route)
-            return func
+        def decorator(
+            fn: _inference_api_wrapper[IOType],
+        ) -> _inference_api_wrapper[IOType]:
+            _api = InferenceAPI[IOType](
+                name=first_not_none(name, default=fn.__name__),
+                user_defined_callback=fn,
+                input_descriptor=input,
+                output_descriptor=output,
+                doc=doc,
+                route=route,
+            )
+            if _api.name in self.apis:
+                raise BentoMLException(
+                    f"API {_api.name} is already defined in Service {self.name}"
+                )
+            self.apis[_api.name] = _api
+            return fn
 
-        return decorator
+        return t.cast("_inference_api_wrapper[IOType]", decorator)
 
     def __str__(self):
         if self.bento:
             return f'bentoml.Service(tag="{self.tag}", ' f'path="{self.bento.path}")'
 
         try:
             import_str, working_dir = self.get_service_import_origin()
```

### Comparing `bentoml-1.1.0/src/bentoml/_internal/service/openapi/__init__.py` & `bentoml-1.1.1/src/bentoml/_internal/service/openapi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     # override all other types
     ["override"],
     # override conflicting types
     ["override"],
 )
 
 
-def make_api_path(api: InferenceAPI) -> str:
+def make_api_path(api: InferenceAPI[t.Any]) -> str:
     return api.route if api.route.startswith("/") else f"/{api.route}"
 
 
 @lru_cache(maxsize=1)
 def make_infra_endpoints() -> dict[str, PathItem]:
     return {
         endpoint: PathItem(
```

### Comparing `bentoml-1.1.0/src/bentoml/_internal/service/openapi/specification.py` & `bentoml-1.1.1/src/bentoml/_internal/service/openapi/specification.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/service/openapi/utils.py` & `bentoml-1.1.1/src/bentoml/_internal/service/openapi/utils.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/utils/__init__.py` & `bentoml-1.1.1/src/bentoml/_internal/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/utils/alg.py` & `bentoml-1.1.1/src/bentoml/_internal/utils/alg.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/utils/benchmark.py` & `bentoml-1.1.1/src/bentoml/_internal/utils/benchmark.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/utils/buildx.py` & `bentoml-1.1.1/src/bentoml/_internal/utils/buildx.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/utils/cattr.py` & `bentoml-1.1.1/src/bentoml/_internal/utils/cattr.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/utils/dotenv.py` & `bentoml-1.1.1/src/bentoml/_internal/utils/dotenv.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/utils/formparser.py` & `bentoml-1.1.1/src/bentoml/_internal/utils/formparser.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/utils/http.py` & `bentoml-1.1.1/src/bentoml/_internal/utils/http.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/utils/lazy_loader.py` & `bentoml-1.1.1/src/bentoml/_internal/utils/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/utils/metrics.py` & `bentoml-1.1.1/src/bentoml/_internal/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/utils/pickle.py` & `bentoml-1.1.1/src/bentoml/_internal/utils/pickle.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/utils/pkg.py` & `bentoml-1.1.1/src/bentoml/_internal/utils/pkg.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/utils/telemetry.py` & `bentoml-1.1.1/src/bentoml/_internal/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/utils/unflatten.py` & `bentoml-1.1.1/src/bentoml/_internal/utils/unflatten.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/utils/uri.py` & `bentoml-1.1.1/src/bentoml/_internal/utils/uri.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/utils/analytics/__init__.py` & `bentoml-1.1.1/src/bentoml/_internal/utils/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/utils/analytics/cli_events.py` & `bentoml-1.1.1/src/bentoml/_internal/utils/analytics/cli_events.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/utils/analytics/schemas.py` & `bentoml-1.1.1/src/bentoml/_internal/utils/analytics/schemas.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/utils/analytics/usage_stats.py` & `bentoml-1.1.1/src/bentoml/_internal/utils/analytics/usage_stats.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/_internal/utils/circus/__init__.py` & `bentoml-1.1.1/src/bentoml/_internal/utils/circus/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -49,9 +49,12 @@
 
     with reserve_free_port() as endpoint_port:
         with reserve_free_port() as pubsub_port:
             return Arbiter(
                 watchers,
                 endpoint=f"tcp://127.0.0.1:{endpoint_port}",
                 pubsub_endpoint=f"tcp://127.0.0.1:{pubsub_port}",
+                # XXX: Currently ,the default check_delay will always raise ConflictError. This probably has to do with
+                # the runners server is not ready in time when the controller run healthcheck.
+                check_delay=kwargs.pop("check_delay", 10),
                 **kwargs,
             )
```

### Comparing `bentoml-1.1.0/src/bentoml/_internal/utils/circus/watchfilesplugin.py` & `bentoml-1.1.1/src/bentoml/_internal/utils/circus/watchfilesplugin.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/grpc/types.py` & `bentoml-1.1.1/src/bentoml/grpc/types.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/grpc/interceptors/access.py` & `bentoml-1.1.1/src/bentoml/grpc/interceptors/access.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/grpc/interceptors/opentelemetry.py` & `bentoml-1.1.1/src/bentoml/grpc/interceptors/opentelemetry.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/grpc/interceptors/prometheus.py` & `bentoml-1.1.1/src/bentoml/grpc/interceptors/prometheus.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/grpc/utils/__init__.py` & `bentoml-1.1.1/src/bentoml/grpc/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/grpc/utils/_import_hook.py` & `bentoml-1.1.1/src/bentoml/grpc/utils/_import_hook.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/grpc/v1/service.proto` & `bentoml-1.1.1/src/bentoml/grpc/v1/service.proto`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/grpc/v1/_generated_pb3/service_pb2.py` & `bentoml-1.1.1/src/bentoml/grpc/v1/_generated_pb3/service_pb2.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/grpc/v1/_generated_pb3/service_pb2.pyi` & `bentoml-1.1.1/src/bentoml/grpc/v1/_generated_pb3/service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/grpc/v1/_generated_pb3/service_pb2_grpc.py` & `bentoml-1.1.1/src/bentoml/grpc/v1/_generated_pb3/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/grpc/v1/_generated_pb3/service_pb2_grpc.pyi` & `bentoml-1.1.1/src/bentoml/grpc/v1/_generated_pb3/service_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/grpc/v1/_generated_pb4/service_pb2.py` & `bentoml-1.1.1/src/bentoml/grpc/v1/_generated_pb4/service_pb2.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/grpc/v1/_generated_pb4/service_pb2.pyi` & `bentoml-1.1.1/src/bentoml/grpc/v1/_generated_pb4/service_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -478,15 +478,15 @@
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _DType:
         ValueType = typing.NewType("ValueType", builtins.int)
         V: typing_extensions.TypeAlias = ValueType
 
-    class _DTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[NDArray._DType.ValueType], builtins.type):  # noqa: F821
+    class _DTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[NDArray._DType.ValueType], builtins.type):
         DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
         DTYPE_UNSPECIFIED: NDArray._DType.ValueType  # 0
         """Represents a None type."""
         DTYPE_FLOAT: NDArray._DType.ValueType  # 1
         """Represents an float type."""
         DTYPE_DOUBLE: NDArray._DType.ValueType  # 2
         """Represents an double type."""
@@ -584,41 +584,41 @@
 
 class BentoService(google.protobuf.service.Service, metaclass=abc.ABCMeta):
     """a gRPC BentoServer."""
 
     DESCRIPTOR: google.protobuf.descriptor.ServiceDescriptor
     @abc.abstractmethod
     def Call(
-        inst: BentoService,
+        inst: BentoService,  # pyright: ignore[reportSelfClsParameterName]
         rpc_controller: google.protobuf.service.RpcController,
         request: global___Request,
         callback: collections.abc.Callable[[global___Response], None] | None,
     ) -> concurrent.futures.Future[global___Response]:
         """Call handles methodcaller of given API entrypoint."""
     @abc.abstractmethod
     def ServiceMetadata(
-        inst: BentoService,
+        inst: BentoService,  # pyright: ignore[reportSelfClsParameterName]
         rpc_controller: google.protobuf.service.RpcController,
         request: global___ServiceMetadataRequest,
         callback: collections.abc.Callable[[global___ServiceMetadataResponse], None] | None,
     ) -> concurrent.futures.Future[global___ServiceMetadataResponse]:
         """ServiceMetadata returns metadata of bentoml.Service."""
 
 class BentoService_Stub(BentoService):
     """a gRPC BentoServer."""
 
     def __init__(self, rpc_channel: google.protobuf.service.RpcChannel) -> None: ...
     DESCRIPTOR: google.protobuf.descriptor.ServiceDescriptor
     def Call(
-        inst: BentoService_Stub,
+        inst: BentoService_Stub,  # pyright: ignore[reportSelfClsParameterName]
         rpc_controller: google.protobuf.service.RpcController,
         request: global___Request,
         callback: collections.abc.Callable[[global___Response], None] | None = ...,
     ) -> concurrent.futures.Future[global___Response]:
         """Call handles methodcaller of given API entrypoint."""
     def ServiceMetadata(
-        inst: BentoService_Stub,
+        inst: BentoService_Stub,  # pyright: ignore[reportSelfClsParameterName]
         rpc_controller: google.protobuf.service.RpcController,
         request: global___ServiceMetadataRequest,
         callback: collections.abc.Callable[[global___ServiceMetadataResponse], None] | None = ...,
     ) -> concurrent.futures.Future[global___ServiceMetadataResponse]:
         """ServiceMetadata returns metadata of bentoml.Service."""
```

### Comparing `bentoml-1.1.0/src/bentoml/grpc/v1/_generated_pb4/service_pb2_grpc.py` & `bentoml-1.1.1/src/bentoml/grpc/v1/_generated_pb4/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/grpc/v1/_generated_pb4/service_pb2_grpc.pyi` & `bentoml-1.1.1/src/bentoml/grpc/v1alpha1/_generated_pb3/service_pb2_grpc.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,30 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import abc
-import bentoml.grpc.v1.service_pb2
+import bentoml.grpc.v1alpha1.service_pb2
 import grpc
 
 class BentoServiceStub:
     """a gRPC BentoServer."""
 
     def __init__(self, channel: grpc.Channel) -> None: ...
     Call: grpc.UnaryUnaryMultiCallable[
-        bentoml.grpc.v1.service_pb2.Request,
-        bentoml.grpc.v1.service_pb2.Response,
+        bentoml.grpc.v1alpha1.service_pb2.Request,
+        bentoml.grpc.v1alpha1.service_pb2.Response,
     ]
     """Call handles methodcaller of given API entrypoint."""
-    ServiceMetadata: grpc.UnaryUnaryMultiCallable[
-        bentoml.grpc.v1.service_pb2.ServiceMetadataRequest,
-        bentoml.grpc.v1.service_pb2.ServiceMetadataResponse,
-    ]
-    """ServiceMetadata returns metadata of bentoml.Service."""
 
 class BentoServiceServicer(metaclass=abc.ABCMeta):
     """a gRPC BentoServer."""
 
     @abc.abstractmethod
     def Call(
         self,
-        request: bentoml.grpc.v1.service_pb2.Request,
+        request: bentoml.grpc.v1alpha1.service_pb2.Request,
         context: grpc.ServicerContext,
-    ) -> bentoml.grpc.v1.service_pb2.Response:
+    ) -> bentoml.grpc.v1alpha1.service_pb2.Response:
         """Call handles methodcaller of given API entrypoint."""
-    @abc.abstractmethod
-    def ServiceMetadata(
-        self,
-        request: bentoml.grpc.v1.service_pb2.ServiceMetadataRequest,
-        context: grpc.ServicerContext,
-    ) -> bentoml.grpc.v1.service_pb2.ServiceMetadataResponse:
-        """ServiceMetadata returns metadata of bentoml.Service."""
 
 def add_BentoServiceServicer_to_server(servicer: BentoServiceServicer, server: grpc.Server) -> None: ...
```

### Comparing `bentoml-1.1.0/src/bentoml/grpc/v1alpha1/service.proto` & `bentoml-1.1.1/src/bentoml/grpc/v1alpha1/service.proto`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/grpc/v1alpha1/_generated_pb3/service_pb2.py` & `bentoml-1.1.1/src/bentoml/grpc/v1alpha1/_generated_pb3/service_pb2.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/grpc/v1alpha1/_generated_pb3/service_pb2.pyi` & `bentoml-1.1.1/src/bentoml/grpc/v1alpha1/_generated_pb3/service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/grpc/v1alpha1/_generated_pb3/service_pb2_grpc.py` & `bentoml-1.1.1/src/bentoml/grpc/v1alpha1/_generated_pb3/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/grpc/v1alpha1/_generated_pb3/service_pb2_grpc.pyi` & `bentoml-1.1.1/src/bentoml/grpc/v1alpha1/_generated_pb4/service_pb2_grpc.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,50 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import abc
 import bentoml.grpc.v1alpha1.service_pb2
+import collections.abc
 import grpc
+import grpc.aio
+import typing
+
+_T = typing.TypeVar('_T')
+
+class _MaybeAsyncIterator(collections.abc.AsyncIterator[_T], collections.abc.Iterator[_T], metaclass=abc.ABCMeta):
+    ...
+
+class _ServicerContext(grpc.ServicerContext, grpc.aio.ServicerContext):  # type: ignore
+    ...
 
 class BentoServiceStub:
     """a gRPC BentoServer."""
 
-    def __init__(self, channel: grpc.Channel) -> None: ...
+    def __init__(self, channel: typing.Union[grpc.Channel, grpc.aio.Channel]) -> None: ...
     Call: grpc.UnaryUnaryMultiCallable[
         bentoml.grpc.v1alpha1.service_pb2.Request,
         bentoml.grpc.v1alpha1.service_pb2.Response,
     ]
     """Call handles methodcaller of given API entrypoint."""
 
+class BentoServiceAsyncStub:
+    """a gRPC BentoServer."""
+
+    Call: grpc.aio.UnaryUnaryMultiCallable[
+        bentoml.grpc.v1alpha1.service_pb2.Request,
+        bentoml.grpc.v1alpha1.service_pb2.Response,
+    ]
+    """Call handles methodcaller of given API entrypoint."""
+
 class BentoServiceServicer(metaclass=abc.ABCMeta):
     """a gRPC BentoServer."""
 
     @abc.abstractmethod
     def Call(
         self,
         request: bentoml.grpc.v1alpha1.service_pb2.Request,
-        context: grpc.ServicerContext,
-    ) -> bentoml.grpc.v1alpha1.service_pb2.Response:
+        context: _ServicerContext,
+    ) -> typing.Union[bentoml.grpc.v1alpha1.service_pb2.Response, collections.abc.Awaitable[bentoml.grpc.v1alpha1.service_pb2.Response]]:
         """Call handles methodcaller of given API entrypoint."""
 
-def add_BentoServiceServicer_to_server(servicer: BentoServiceServicer, server: grpc.Server) -> None: ...
+def add_BentoServiceServicer_to_server(servicer: BentoServiceServicer, server: typing.Union[grpc.Server, grpc.aio.Server]) -> None: ...
```

### Comparing `bentoml-1.1.0/src/bentoml/grpc/v1alpha1/_generated_pb4/service_pb2.py` & `bentoml-1.1.1/src/bentoml/grpc/v1alpha1/_generated_pb4/service_pb2.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/grpc/v1alpha1/_generated_pb4/service_pb2.pyi` & `bentoml-1.1.1/src/bentoml/grpc/v1alpha1/_generated_pb4/service_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -272,15 +272,15 @@
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _FileType:
         ValueType = typing.NewType("ValueType", builtins.int)
         V: typing_extensions.TypeAlias = ValueType
 
-    class _FileTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[File._FileType.ValueType], builtins.type):  # noqa: F821
+    class _FileTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[File._FileType.ValueType], builtins.type):
         DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
         FILE_TYPE_UNSPECIFIED: File._FileType.ValueType  # 0
         FILE_TYPE_CSV: File._FileType.ValueType  # 1
         """file types"""
         FILE_TYPE_PLAINTEXT: File._FileType.ValueType  # 2
         FILE_TYPE_JSON: File._FileType.ValueType  # 3
         FILE_TYPE_BYTES: File._FileType.ValueType  # 4
@@ -416,15 +416,15 @@
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _DType:
         ValueType = typing.NewType("ValueType", builtins.int)
         V: typing_extensions.TypeAlias = ValueType
 
-    class _DTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[NDArray._DType.ValueType], builtins.type):  # noqa: F821
+    class _DTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[NDArray._DType.ValueType], builtins.type):
         DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
         DTYPE_UNSPECIFIED: NDArray._DType.ValueType  # 0
         """Represents a None type."""
         DTYPE_FLOAT: NDArray._DType.ValueType  # 1
         """Represents an float type."""
         DTYPE_DOUBLE: NDArray._DType.ValueType  # 2
         """Represents an double type."""
@@ -522,26 +522,26 @@
 
 class BentoService(google.protobuf.service.Service, metaclass=abc.ABCMeta):
     """a gRPC BentoServer."""
 
     DESCRIPTOR: google.protobuf.descriptor.ServiceDescriptor
     @abc.abstractmethod
     def Call(
-        inst: BentoService,
+        inst: BentoService,  # pyright: ignore[reportSelfClsParameterName]
         rpc_controller: google.protobuf.service.RpcController,
         request: global___Request,
         callback: collections.abc.Callable[[global___Response], None] | None,
     ) -> concurrent.futures.Future[global___Response]:
         """Call handles methodcaller of given API entrypoint."""
 
 class BentoService_Stub(BentoService):
     """a gRPC BentoServer."""
 
     def __init__(self, rpc_channel: google.protobuf.service.RpcChannel) -> None: ...
     DESCRIPTOR: google.protobuf.descriptor.ServiceDescriptor
     def Call(
-        inst: BentoService_Stub,
+        inst: BentoService_Stub,  # pyright: ignore[reportSelfClsParameterName]
         rpc_controller: google.protobuf.service.RpcController,
         request: global___Request,
         callback: collections.abc.Callable[[global___Response], None] | None = ...,
     ) -> concurrent.futures.Future[global___Response]:
         """Call handles methodcaller of given API entrypoint."""
```

### Comparing `bentoml-1.1.0/src/bentoml/grpc/v1alpha1/_generated_pb4/service_pb2_grpc.py` & `bentoml-1.1.1/src/bentoml/grpc/v1alpha1/_generated_pb4/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/testing/server.py` & `bentoml-1.1.1/src/bentoml/testing/server.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/testing/utils.py` & `bentoml-1.1.1/src/bentoml/testing/utils.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/testing/grpc/__init__.py` & `bentoml-1.1.1/src/bentoml/testing/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml/testing/pytest/plugin.py` & `bentoml-1.1.1/src/bentoml/testing/pytest/plugin.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml_cli/bentos.py` & `bentoml-1.1.1/src/bentoml_cli/bentos.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml_cli/cli.py` & `bentoml-1.1.1/src/bentoml_cli/cli.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml_cli/cloud.py` & `bentoml-1.1.1/src/bentoml_cli/cloud.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml_cli/containerize.py` & `bentoml-1.1.1/src/bentoml_cli/containerize.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml_cli/deployment.py` & `bentoml-1.1.1/src/bentoml_cli/deployment.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 else:
     TupleStrAny = tuple
 
 
 def add_deployment_command(cli: click.Group) -> None:
     import json
 
+    import click_option_group as cog
     from rich.table import Table
 
     from bentoml._internal.configuration.containers import BentoMLContainer
     from bentoml._internal.utils import bentoml_cattr
     from bentoml._internal.utils import rich_console as console
     from bentoml_cli.utils import BentoMLCommandGroup
 
@@ -29,38 +30,51 @@
         "-o",
         "--output",
         type=click.Choice(["json", "default"]),
         default="default",
         help="Display the output of this command.",
     )
 
-    def shared_decorator(f: t.Callable[..., t.Any]):
-        options = [
-            click.argument(
-                "deployment-name",
-                type=click.STRING,
-                required=True,
-            ),
-            click.option(
-                "--cluster-name",
-                type=click.STRING,
-                default=None,
-                help="Name of the cluster.",
-            ),
-            click.option(
-                "--kube-namespace",
-                type=click.STRING,
-                default=None,
-                help="Kubernetes namespace.",
-            ),
-            output_option,
-        ]
-        for opt in reversed(options):
-            f = opt(f)
-        return f
+    def shared_decorator(
+        f: t.Callable[..., t.Any] | None = None,
+        *,
+        required_deployment_name: bool = True,
+    ) -> t.Callable[..., t.Any]:
+        def decorate(f: t.Callable[..., t.Any]) -> t.Callable[..., t.Any]:
+            options = [
+                click.argument(
+                    "deployment-name",
+                    type=click.STRING,
+                    required=required_deployment_name,
+                ),
+                cog.optgroup.group(
+                    cls=cog.AllOptionGroup, name="cluster and kube namespace options"
+                ),
+                cog.optgroup.option(
+                    "--cluster-name",
+                    type=click.STRING,
+                    default=None,
+                    help="Name of the cluster.",
+                ),
+                cog.optgroup.option(
+                    "--kube-namespace",
+                    type=click.STRING,
+                    default=None,
+                    help="Kubernetes namespace.",
+                ),
+                output_option,
+            ]
+            for opt in reversed(options):
+                f = opt(f)
+            return f
+
+        if f:
+            return decorate(f)
+        else:
+            return decorate
 
     @cli.group(name="deployment", cls=BentoMLCommandGroup)
     def deployment_cli():
         """Deployment Subcommands Groups"""
 
     @deployment_cli.command()
     @click.option(
@@ -88,69 +102,93 @@
         if output == "default":
             console.print(res)
         elif output == "json":
             click.echo(json.dumps(bentoml_cattr.unstructure(res), indent=2))
         return res
 
     @deployment_cli.command()
+    @shared_decorator(required_deployment_name=False)
     @click.option(
         "-f",
         "--file",
         type=click.File(),
         help="JSON file path for the deployment configuration",
     )
-    @click.option("-n", "--name", type=click.STRING, help="Deployment name")
+    @click.option(
+        "-n", "--name", type=click.STRING, help="Deployment name (deprecated)"
+    )
     @click.option("--bento", type=click.STRING, help="Bento tag")
-    @output_option
     @click.pass_obj
     def update(  # type: ignore
         shared_options: SharedOptions,
+        deployment_name: str | None,
         file: str | None,
         name: str | None,
         bento: str | None,
+        cluster_name: str | None,
+        kube_namespace: str | None,
         output: t.Literal["json", "default"],
     ) -> DeploymentSchema:
         """Update a deployment on BentoCloud.
 
         \b
         A deployment can be updated using a json file with needed configurations.
         The json file has the exact format as the one on BentoCloud Deployment UI.
         """
+        if name is not None:
+            click.echo(
+                "--name is deprecated, pass DEPLOYMENT_NAME as an argument instead, e.g., bentoml update deploy-name"
+            )
         if file is not None:
             if name is not None:
                 click.echo("Reading from file, ignoring --name", err=True)
+            elif deployment_name is not None:
+                click.echo(
+                    "Reading from file, ignoring argument DEPLOYMENT_NAME", err=True
+                )
             res = client.deployment.update_from_file(
                 path_or_stream=file, context=shared_options.cloud_context
             )
         elif name is not None:
             res = client.deployment.update(
                 name,
                 bento=bento,
                 context=shared_options.cloud_context,
                 latest_bento=True,
+                cluster_name=cluster_name,
+                kube_namespace=kube_namespace,
+            )
+        elif deployment_name is not None:
+            res = client.deployment.update(
+                deployment_name,
+                bento=bento,
+                context=shared_options.cloud_context,
+                latest_bento=True,
+                cluster_name=cluster_name,
+                kube_namespace=kube_namespace,
             )
         else:
             raise click.BadArgumentUsage(
-                "Either --file or --name is required for update command"
+                "Either --file or argument DEPLOYMENT_NAME is required for update command"
             )
         if output == "default":
             console.print(res)
         elif output == "json":
             unstructured = bentoml_cattr.unstructure(res)
             click.echo(json.dumps(unstructured, indent=2))
         return res
 
     @deployment_cli.command()
     @shared_decorator
     @click.pass_obj
     def get(  # type: ignore
         shared_options: SharedOptions,
         deployment_name: str,
-        cluster_name: str,
-        kube_namespace: str,
+        cluster_name: str | None,
+        kube_namespace: str | None,
         output: t.Literal["json", "default"],
     ) -> DeploymentSchema:
         """Get a deployment on BentoCloud."""
         res = client.deployment.get(
             deployment_name=deployment_name,
             context=shared_options.cloud_context,
             cluster_name=cluster_name,
@@ -165,16 +203,16 @@
 
     @deployment_cli.command()
     @shared_decorator
     @click.pass_obj
     def terminate(  # type: ignore
         shared_options: SharedOptions,
         deployment_name: str,
-        cluster_name: str,
-        kube_namespace: str,
+        cluster_name: str | None,
+        kube_namespace: str | None,
         output: t.Literal["json", "default"],
     ) -> DeploymentSchema:
         """Terminate a deployment on BentoCloud."""
         res = client.deployment.terminate(
             deployment_name=deployment_name,
             context=shared_options.cloud_context,
             cluster_name=cluster_name,
@@ -189,16 +227,16 @@
 
     @deployment_cli.command()
     @shared_decorator
     @click.pass_obj
     def delete(  # type: ignore
         shared_options: SharedOptions,
         deployment_name: str,
-        cluster_name: str,
-        kube_namespace: str,
+        cluster_name: str | None,
+        kube_namespace: str | None,
         output: t.Literal["json", "default"],
     ) -> DeploymentSchema:
         """Delete a deployment on BentoCloud."""
         res = client.deployment.delete(
             deployment_name=deployment_name,
             context=shared_options.cloud_context,
             cluster_name=cluster_name,
@@ -233,19 +271,19 @@
         help="Display the output of this command.",
         type=click.Choice(["json", "default", "table"]),
         default="table",
     )
     @click.pass_obj
     def list(  # type: ignore
         shared_options: SharedOptions,
-        cluster_name: str,
-        query: str,
-        search: str,
-        count: int,
-        start: int,
+        cluster_name: str | None,
+        query: str | None,
+        search: str | None,
+        count: int | None,
+        start: int | None,
         output: t.Literal["json", "default", "table"],
     ) -> DeploymentListSchema:
         """List existing deployments on BentoCloud."""
         res = client.deployment.list(
             context=shared_options.cloud_context,
             cluster_name=cluster_name,
             query=query,
```

### Comparing `bentoml-1.1.0/src/bentoml_cli/env.py` & `bentoml-1.1.1/src/bentoml_cli/env.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml_cli/env_manager.py` & `bentoml-1.1.1/src/bentoml_cli/env_manager.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml_cli/models.py` & `bentoml-1.1.1/src/bentoml_cli/models.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml_cli/serve.py` & `bentoml-1.1.1/src/bentoml_cli/serve.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml_cli/start.py` & `bentoml-1.1.1/src/bentoml_cli/start.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml_cli/utils.py` & `bentoml-1.1.1/src/bentoml_cli/utils.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml_cli/worker/grpc_api_server.py` & `bentoml-1.1.1/src/bentoml_cli/worker/grpc_api_server.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml_cli/worker/grpc_prometheus_server.py` & `bentoml-1.1.1/src/bentoml_cli/worker/grpc_prometheus_server.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml_cli/worker/http_api_server.py` & `bentoml-1.1.1/src/bentoml_cli/worker/http_api_server.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/src/bentoml_cli/worker/runner.py` & `bentoml-1.1.1/src/bentoml_cli/worker/runner.py`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/.gitignore` & `bentoml-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/LICENSE` & `bentoml-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/README.md` & `bentoml-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `bentoml-1.1.0/pyproject.toml` & `bentoml-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -132,19 +132,22 @@
 only-include = ["src/bentoml", "src/bentoml_cli"]
 [tool.hatch.build.targets.wheel]
 packages = ["src/bentoml", "src/bentoml_cli"]
 
 [[tool.pdm.source]]
 url = "https://download.pytorch.org/whl/cpu"
 name = "torch"
+
 [tool.pdm.resolution]
 respect-source-order = true
 [tool.pdm.resolution.overrides]
 fastapi = "==0.93.0"
 tensorflow = ">=2.3.0"
+tensorflow-io-gcs-filesystem = "==0.31.0"
+
 [tool.pdm.dev-dependencies]
 docs = [
     "sphinx>=5",
     "myst-parser",
     "sphinx-click>=3.0.2",
     "furo",
     "sphinx-inline-tabs",
@@ -172,15 +175,14 @@
     "datasets",
     # ONNX dependencies
     "onnx",
     "onnxruntime",
     "skl2onnx",
     # tensorflow dependencies
     "tensorflow",
-    "tensorflow-io-gcs-filesystem!=0.32.0; python_version < '3.12'",
     # torch-related dependencies
     "torch",
     "lightning",
     # huggingface dependencies
     "transformers",
     "tokenizer",
     "diffusers",
```

### Comparing `bentoml-1.1.0/PKG-INFO` & `bentoml-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bentoml
-Version: 1.1.0
+Version: 1.1.1
 Summary: BentoML: Build Production-Grade AI Applications
 Project-URL: Homepage, https://bentoml.com
 Project-URL: Documentation, https://docs.bentoml.com
 Project-URL: GitHub, https://github.com/bentoml/bentoml
 Project-URL: Twitter, https://twitter.com/bentomlai
 Project-URL: Tracker, https://github.com/bentoml/BentoML/issues
 Project-URL: Slack, https://l.bentoml.com/join-slack
```

