# Comparing `tmp/sparseml_nightly-1.6.0.20230723-py3-none-any.whl.zip` & `tmp/sparseml_nightly-1.6.0.20230801-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,378 +1,378 @@
-Zip file size: 969880 bytes, number of entries: 376
--rw-rw-r--  2.0 unx     1413 b- defN 23-Jul-23 01:31 sparseml/__init__.py
--rw-rw-r--  2.0 unx      898 b- defN 23-Jul-23 01:31 sparseml/analytics.py
--rw-rw-r--  2.0 unx    10284 b- defN 23-Jul-23 01:31 sparseml/base.py
--rw-rw-r--  2.0 unx     2483 b- defN 23-Jul-23 01:31 sparseml/log.py
--rw-rw-r--  2.0 unx     1511 b- defN 23-Jul-23 01:31 sparseml/version.py
--rw-rw-r--  2.0 unx      758 b- defN 23-Jul-23 01:31 sparseml/benchmark/__init__.py
--rw-rw-r--  2.0 unx    17763 b- defN 23-Jul-23 01:31 sparseml/benchmark/info.py
--rw-rw-r--  2.0 unx    10778 b- defN 23-Jul-23 01:31 sparseml/benchmark/serialization.py
--rw-rw-r--  2.0 unx      863 b- defN 23-Jul-23 01:31 sparseml/deepsparse/__init__.py
--rw-rw-r--  2.0 unx     3516 b- defN 23-Jul-23 01:31 sparseml/deepsparse/base.py
--rw-rw-r--  2.0 unx      801 b- defN 23-Jul-23 01:31 sparseml/deepsparse/framework/__init__.py
--rw-rw-r--  2.0 unx     6032 b- defN 23-Jul-23 01:31 sparseml/deepsparse/framework/info.py
--rw-rw-r--  2.0 unx      813 b- defN 23-Jul-23 01:31 sparseml/deepsparse/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1348 b- defN 23-Jul-23 01:31 sparseml/deepsparse/sparsification/info.py
--rw-rw-r--  2.0 unx      617 b- defN 23-Jul-23 01:31 sparseml/exporters/__init__.py
--rw-rw-r--  2.0 unx     1477 b- defN 23-Jul-23 01:31 sparseml/exporters/base_exporter.py
--rw-rw-r--  2.0 unx     6325 b- defN 23-Jul-23 01:31 sparseml/exporters/kv_cache_injector.py
--rw-rw-r--  2.0 unx     4847 b- defN 23-Jul-23 01:31 sparseml/exporters/onnx_to_deepsparse.py
--rw-rw-r--  2.0 unx     2350 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/__init__.py
--rw-rw-r--  2.0 unx     2333 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/base_transform.py
--rw-rw-r--  2.0 unx     1388 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/constants_to_initializers.py
--rw-rw-r--  2.0 unx     4630 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/conv_to_convinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     5838 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/conv_to_qlinearconv.py
--rw-rw-r--  2.0 unx     2440 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/delete_repeated_qdq.py
--rw-rw-r--  2.0 unx     1842 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/delete_trivial_onnx_adds.py
--rw-rw-r--  2.0 unx     2181 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/flatten_qparams.py
--rw-rw-r--  2.0 unx     3553 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/fold_conv_div_bn.py
--rw-rw-r--  2.0 unx     1669 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/fold_identity_initializers.py
--rw-rw-r--  2.0 unx     2070 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/fold_relu_quants.py
--rw-rw-r--  2.0 unx     4418 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/gemm_to_matmulinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     7629 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/gemm_to_qlinearmatmul.py
--rw-rw-r--  2.0 unx     1645 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/initializers_to_uint8.py
--rw-rw-r--  2.0 unx     6297 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/matmul_add_to_matmulinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     4681 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/matmul_to_matmulinteger_cast_mul.py
--rw-rw-r--  2.0 unx     4156 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/matmul_to_qlinearmatmul.py
--rw-rw-r--  2.0 unx     3724 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/onnx_transform.py
--rw-rw-r--  2.0 unx     3433 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/propagate_dequant_through_split.py
--rw-rw-r--  2.0 unx     4801 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/propagate_embedding_quantization.py
--rw-rw-r--  2.0 unx     4464 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/quantize_qat_embedding.py
--rw-rw-r--  2.0 unx     3869 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/quantize_residuals.py
--rw-rw-r--  2.0 unx     3331 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/remove_duplicate_qconv_weights.py
--rw-rw-r--  2.0 unx     2545 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/remove_duplicate_quantize_ops.py
--rw-rw-r--  2.0 unx     3210 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/skip_input_quantize.py
--rw-rw-r--  2.0 unx     1373 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/unwrap_batchnorms.py
--rw-rw-r--  2.0 unx      909 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/kv_cache/__init__.py
--rw-rw-r--  2.0 unx    30558 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/kv_cache/cache_keys_and_values.py
--rw-rw-r--  2.0 unx     6523 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/kv_cache/configs.py
--rw-rw-r--  2.0 unx     1660 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/kv_cache/positions_adjustment_base.py
--rw-rw-r--  2.0 unx     3377 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/kv_cache/positions_adjustment_codegen.py
--rw-rw-r--  2.0 unx     4951 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/kv_cache/positions_adjustment_opt.py
--rw-rw-r--  2.0 unx      730 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/utils/__init__.py
--rw-rw-r--  2.0 unx    10570 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py
--rw-rw-r--  2.0 unx     6457 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/utils/helpers.py
--rw-rw-r--  2.0 unx    14429 b- defN 23-Jul-23 01:31 sparseml/exporters/transforms/utils/matching.py
--rw-rw-r--  2.0 unx      790 b- defN 23-Jul-23 01:31 sparseml/framework/__init__.py
--rw-rw-r--  2.0 unx     9479 b- defN 23-Jul-23 01:31 sparseml/framework/info.py
--rw-rw-r--  2.0 unx     1144 b- defN 23-Jul-23 01:31 sparseml/keras/__init__.py
--rw-rw-r--  2.0 unx     8054 b- defN 23-Jul-23 01:31 sparseml/keras/base.py
--rw-rw-r--  2.0 unx      943 b- defN 23-Jul-23 01:31 sparseml/keras/datasets/__init__.py
--rw-rw-r--  2.0 unx     3297 b- defN 23-Jul-23 01:31 sparseml/keras/datasets/dataset.py
--rw-rw-r--  2.0 unx     2423 b- defN 23-Jul-23 01:31 sparseml/keras/datasets/helpers.py
--rw-rw-r--  2.0 unx     2761 b- defN 23-Jul-23 01:31 sparseml/keras/datasets/registry.py
--rw-rw-r--  2.0 unx      786 b- defN 23-Jul-23 01:31 sparseml/keras/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx     8369 b- defN 23-Jul-23 01:31 sparseml/keras/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     4301 b- defN 23-Jul-23 01:31 sparseml/keras/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     2727 b- defN 23-Jul-23 01:31 sparseml/keras/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx      793 b- defN 23-Jul-23 01:31 sparseml/keras/framework/__init__.py
--rw-rw-r--  2.0 unx     5906 b- defN 23-Jul-23 01:31 sparseml/keras/framework/info.py
--rw-rw-r--  2.0 unx      921 b- defN 23-Jul-23 01:31 sparseml/keras/models/__init__.py
--rw-rw-r--  2.0 unx    11814 b- defN 23-Jul-23 01:31 sparseml/keras/models/registry.py
--rw-rw-r--  2.0 unx      656 b- defN 23-Jul-23 01:31 sparseml/keras/models/classification/__init__.py
--rw-rw-r--  2.0 unx    17932 b- defN 23-Jul-23 01:31 sparseml/keras/models/classification/resnet.py
--rw-rw-r--  2.0 unx      768 b- defN 23-Jul-23 01:31 sparseml/keras/models/external/__init__.py
--rw-rw-r--  2.0 unx     4402 b- defN 23-Jul-23 01:31 sparseml/keras/models/external/keras_applications.py
--rw-rw-r--  2.0 unx     1166 b- defN 23-Jul-23 01:31 sparseml/keras/optim/__init__.py
--rw-rw-r--  2.0 unx     5677 b- defN 23-Jul-23 01:31 sparseml/keras/optim/manager.py
--rw-rw-r--  2.0 unx    14777 b- defN 23-Jul-23 01:31 sparseml/keras/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    19740 b- defN 23-Jul-23 01:31 sparseml/keras/optim/mask_pruning_creator.py
--rw-rw-r--  2.0 unx     9183 b- defN 23-Jul-23 01:31 sparseml/keras/optim/modifier.py
--rw-rw-r--  2.0 unx     1676 b- defN 23-Jul-23 01:31 sparseml/keras/optim/modifier_epoch.py
--rw-rw-r--  2.0 unx    14736 b- defN 23-Jul-23 01:31 sparseml/keras/optim/modifier_lr.py
--rw-rw-r--  2.0 unx     5477 b- defN 23-Jul-23 01:31 sparseml/keras/optim/modifier_params.py
--rw-rw-r--  2.0 unx    24031 b- defN 23-Jul-23 01:31 sparseml/keras/optim/modifier_pruning.py
--rw-rw-r--  2.0 unx     1133 b- defN 23-Jul-23 01:31 sparseml/keras/optim/utils.py
--rw-rw-r--  2.0 unx      808 b- defN 23-Jul-23 01:31 sparseml/keras/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1356 b- defN 23-Jul-23 01:31 sparseml/keras/sparsification/info.py
--rw-rw-r--  2.0 unx      962 b- defN 23-Jul-23 01:31 sparseml/keras/utils/__init__.py
--rw-rw-r--  2.0 unx     8202 b- defN 23-Jul-23 01:31 sparseml/keras/utils/callbacks.py
--rw-rw-r--  2.0 unx     1022 b- defN 23-Jul-23 01:31 sparseml/keras/utils/compat.py
--rw-rw-r--  2.0 unx     5737 b- defN 23-Jul-23 01:31 sparseml/keras/utils/exporter.py
--rw-rw-r--  2.0 unx     6087 b- defN 23-Jul-23 01:31 sparseml/keras/utils/logger.py
--rw-rw-r--  2.0 unx     1738 b- defN 23-Jul-23 01:31 sparseml/keras/utils/model.py
--rw-rw-r--  2.0 unx     1036 b- defN 23-Jul-23 01:31 sparseml/onnx/__init__.py
--rw-rw-r--  2.0 unx     6202 b- defN 23-Jul-23 01:31 sparseml/onnx/base.py
--rw-rw-r--  2.0 unx      743 b- defN 23-Jul-23 01:31 sparseml/onnx/benchmark/__init__.py
--rw-rw-r--  2.0 unx    15366 b- defN 23-Jul-23 01:31 sparseml/onnx/benchmark/info.py
--rw-rw-r--  2.0 unx      823 b- defN 23-Jul-23 01:31 sparseml/onnx/framework/__init__.py
--rw-rw-r--  2.0 unx     6116 b- defN 23-Jul-23 01:31 sparseml/onnx/framework/info.py
--rw-rw-r--  2.0 unx      820 b- defN 23-Jul-23 01:31 sparseml/onnx/optim/__init__.py
--rw-rw-r--  2.0 unx    13285 b- defN 23-Jul-23 01:31 sparseml/onnx/optim/analyzer_model.py
--rw-rw-r--  2.0 unx    19639 b- defN 23-Jul-23 01:31 sparseml/onnx/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx     6470 b- defN 23-Jul-23 01:31 sparseml/onnx/optim/structured_pruning.py
--rw-rw-r--  2.0 unx      815 b- defN 23-Jul-23 01:31 sparseml/onnx/optim/quantization/__init__.py
--rw-rw-r--  2.0 unx    14753 b- defN 23-Jul-23 01:31 sparseml/onnx/optim/quantization/calibration.py
--rw-rw-r--  2.0 unx    73551 b- defN 23-Jul-23 01:31 sparseml/onnx/optim/quantization/quantize.py
--rw-rw-r--  2.0 unx     4552 b- defN 23-Jul-23 01:31 sparseml/onnx/optim/quantization/quantize_model_post_training.py
--rw-rw-r--  2.0 unx      869 b- defN 23-Jul-23 01:31 sparseml/onnx/sparsification/__init__.py
--rw-rw-r--  2.0 unx    10209 b- defN 23-Jul-23 01:31 sparseml/onnx/sparsification/analyzer.py
--rw-rw-r--  2.0 unx     1363 b- defN 23-Jul-23 01:31 sparseml/onnx/sparsification/info.py
--rw-rw-r--  2.0 unx     8009 b- defN 23-Jul-23 01:31 sparseml/onnx/sparsification/model_info.py
--rw-rw-r--  2.0 unx      867 b- defN 23-Jul-23 01:31 sparseml/onnx/utils/__init__.py
--rw-rw-r--  2.0 unx    13013 b- defN 23-Jul-23 01:31 sparseml/onnx/utils/data.py
--rw-rw-r--  2.0 unx    18825 b- defN 23-Jul-23 01:31 sparseml/onnx/utils/graph_editor.py
--rw-rw-r--  2.0 unx     8133 b- defN 23-Jul-23 01:31 sparseml/onnx/utils/graph_optimizer.py
--rw-rw-r--  2.0 unx    40230 b- defN 23-Jul-23 01:31 sparseml/onnx/utils/helpers.py
--rw-rw-r--  2.0 unx     1958 b- defN 23-Jul-23 01:31 sparseml/onnx/utils/loss.py
--rw-rw-r--  2.0 unx    31591 b- defN 23-Jul-23 01:31 sparseml/onnx/utils/model.py
--rw-rw-r--  2.0 unx     5437 b- defN 23-Jul-23 01:31 sparseml/onnx/utils/sparse_tensor.py
--rw-rw-r--  2.0 unx      931 b- defN 23-Jul-23 01:31 sparseml/openpifpaf/__init__.py
--rw-rw-r--  2.0 unx     3713 b- defN 23-Jul-23 01:31 sparseml/openpifpaf/export.py
--rw-rw-r--  2.0 unx    10950 b- defN 23-Jul-23 01:31 sparseml/openpifpaf/train.py
--rw-rw-r--  2.0 unx     4211 b- defN 23-Jul-23 01:31 sparseml/openpifpaf/trainer.py
--rw-rw-r--  2.0 unx      882 b- defN 23-Jul-23 01:31 sparseml/optim/__init__.py
--rw-rw-r--  2.0 unx     6302 b- defN 23-Jul-23 01:31 sparseml/optim/analyzer.py
--rw-rw-r--  2.0 unx    25563 b- defN 23-Jul-23 01:31 sparseml/optim/helpers.py
--rw-rw-r--  2.0 unx    25984 b- defN 23-Jul-23 01:31 sparseml/optim/manager.py
--rw-rw-r--  2.0 unx    30708 b- defN 23-Jul-23 01:31 sparseml/optim/modifier.py
--rw-rw-r--  2.0 unx    26315 b- defN 23-Jul-23 01:31 sparseml/optim/sensitivity.py
--rw-rw-r--  2.0 unx     2190 b- defN 23-Jul-23 01:31 sparseml/pytorch/__init__.py
--rw-rw-r--  2.0 unx     6155 b- defN 23-Jul-23 01:31 sparseml/pytorch/base.py
--rw-rw-r--  2.0 unx      933 b- defN 23-Jul-23 01:31 sparseml/pytorch/opset.py
--rw-rw-r--  2.0 unx    11013 b- defN 23-Jul-23 01:31 sparseml/pytorch/torch_to_onnx_exporter.py
--rw-rw-r--  2.0 unx      998 b- defN 23-Jul-23 01:31 sparseml/pytorch/datasets/__init__.py
--rw-rw-r--  2.0 unx     4193 b- defN 23-Jul-23 01:31 sparseml/pytorch/datasets/generic.py
--rw-rw-r--  2.0 unx     3014 b- defN 23-Jul-23 01:31 sparseml/pytorch/datasets/registry.py
--rw-rw-r--  2.0 unx      828 b- defN 23-Jul-23 01:31 sparseml/pytorch/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx     4457 b- defN 23-Jul-23 01:31 sparseml/pytorch/datasets/classification/cifar.py
--rw-rw-r--  2.0 unx     3669 b- defN 23-Jul-23 01:31 sparseml/pytorch/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     4000 b- defN 23-Jul-23 01:31 sparseml/pytorch/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     6491 b- defN 23-Jul-23 01:31 sparseml/pytorch/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx     2434 b- defN 23-Jul-23 01:31 sparseml/pytorch/datasets/classification/mnist.py
--rw-rw-r--  2.0 unx      767 b- defN 23-Jul-23 01:31 sparseml/pytorch/datasets/detection/__init__.py
--rw-rw-r--  2.0 unx    16159 b- defN 23-Jul-23 01:31 sparseml/pytorch/datasets/detection/coco.py
--rw-rw-r--  2.0 unx     5705 b- defN 23-Jul-23 01:31 sparseml/pytorch/datasets/detection/helpers.py
--rw-rw-r--  2.0 unx    10759 b- defN 23-Jul-23 01:31 sparseml/pytorch/datasets/detection/voc.py
--rw-rw-r--  2.0 unx      617 b- defN 23-Jul-23 01:31 sparseml/pytorch/datasets/image_classification/__init__.py
--rw-rw-r--  2.0 unx     9512 b- defN 23-Jul-23 01:31 sparseml/pytorch/datasets/image_classification/ffcv_dataset.py
--rw-rw-r--  2.0 unx      684 b- defN 23-Jul-23 01:31 sparseml/pytorch/datasets/recommendation/__init__.py
--rw-rw-r--  2.0 unx      693 b- defN 23-Jul-23 01:31 sparseml/pytorch/datasets/video/__init__.py
--rw-rw-r--  2.0 unx      814 b- defN 23-Jul-23 01:31 sparseml/pytorch/framework/__init__.py
--rw-rw-r--  2.0 unx     5580 b- defN 23-Jul-23 01:31 sparseml/pytorch/framework/info.py
--rw-rw-r--  2.0 unx      753 b- defN 23-Jul-23 01:31 sparseml/pytorch/image_classification/__init__.py
--rw-rw-r--  2.0 unx    18265 b- defN 23-Jul-23 01:31 sparseml/pytorch/image_classification/export.py
--rw-rw-r--  2.0 unx    15494 b- defN 23-Jul-23 01:31 sparseml/pytorch/image_classification/lr_analysis.py
--rw-rw-r--  2.0 unx    14444 b- defN 23-Jul-23 01:31 sparseml/pytorch/image_classification/pr_sensitivity.py
--rw-rw-r--  2.0 unx    29287 b- defN 23-Jul-23 01:31 sparseml/pytorch/image_classification/train.py
--rw-rw-r--  2.0 unx      682 b- defN 23-Jul-23 01:31 sparseml/pytorch/image_classification/utils/__init__.py
--rw-rw-r--  2.0 unx     4278 b- defN 23-Jul-23 01:31 sparseml/pytorch/image_classification/utils/cli_helpers.py
--rw-rw-r--  2.0 unx     1257 b- defN 23-Jul-23 01:31 sparseml/pytorch/image_classification/utils/constants.py
--rw-rw-r--  2.0 unx    21742 b- defN 23-Jul-23 01:31 sparseml/pytorch/image_classification/utils/helpers.py
--rw-rw-r--  2.0 unx    12056 b- defN 23-Jul-23 01:31 sparseml/pytorch/image_classification/utils/trainer.py
--rw-rw-r--  2.0 unx      976 b- defN 23-Jul-23 01:31 sparseml/pytorch/models/__init__.py
--rw-rw-r--  2.0 unx    14753 b- defN 23-Jul-23 01:31 sparseml/pytorch/models/registry.py
--rw-rw-r--  2.0 unx      901 b- defN 23-Jul-23 01:31 sparseml/pytorch/models/classification/__init__.py
--rw-rw-r--  2.0 unx    11658 b- defN 23-Jul-23 01:31 sparseml/pytorch/models/classification/darknet.py
--rw-rw-r--  2.0 unx    40293 b- defN 23-Jul-23 01:31 sparseml/pytorch/models/classification/efficientnet.py
--rw-rw-r--  2.0 unx    16512 b- defN 23-Jul-23 01:31 sparseml/pytorch/models/classification/inception_v3.py
--rw-rw-r--  2.0 unx     4164 b- defN 23-Jul-23 01:31 sparseml/pytorch/models/classification/mnist.py
--rw-rw-r--  2.0 unx     9546 b- defN 23-Jul-23 01:31 sparseml/pytorch/models/classification/mobilenet.py
--rw-rw-r--  2.0 unx    13014 b- defN 23-Jul-23 01:31 sparseml/pytorch/models/classification/mobilenet_v2.py
--rw-rw-r--  2.0 unx    40800 b- defN 23-Jul-23 01:31 sparseml/pytorch/models/classification/resnet.py
--rw-rw-r--  2.0 unx    16649 b- defN 23-Jul-23 01:31 sparseml/pytorch/models/classification/vgg.py
--rw-rw-r--  2.0 unx      824 b- defN 23-Jul-23 01:31 sparseml/pytorch/models/detection/__init__.py
--rw-rw-r--  2.0 unx     6820 b- defN 23-Jul-23 01:31 sparseml/pytorch/models/detection/ssd.py
--rw-rw-r--  2.0 unx     8116 b- defN 23-Jul-23 01:31 sparseml/pytorch/models/detection/ssd_lite.py
--rw-rw-r--  2.0 unx     4046 b- defN 23-Jul-23 01:31 sparseml/pytorch/models/detection/ssd_mobilenet.py
--rw-rw-r--  2.0 unx     9069 b- defN 23-Jul-23 01:31 sparseml/pytorch/models/detection/ssd_resnet.py
--rw-rw-r--  2.0 unx    10188 b- defN 23-Jul-23 01:31 sparseml/pytorch/models/detection/yolo_v3.py
--rw-rw-r--  2.0 unx      763 b- defN 23-Jul-23 01:31 sparseml/pytorch/models/external/__init__.py
--rw-rw-r--  2.0 unx     6759 b- defN 23-Jul-23 01:31 sparseml/pytorch/models/external/torchvision.py
--rw-rw-r--  2.0 unx      676 b- defN 23-Jul-23 01:31 sparseml/pytorch/models/recommendation/__init__.py
--rw-rw-r--  2.0 unx      925 b- defN 23-Jul-23 01:31 sparseml/pytorch/nn/__init__.py
--rw-rw-r--  2.0 unx     8673 b- defN 23-Jul-23 01:31 sparseml/pytorch/nn/activations.py
--rw-rw-r--  2.0 unx    11854 b- defN 23-Jul-23 01:31 sparseml/pytorch/nn/fatrelu.py
--rw-rw-r--  2.0 unx     1690 b- defN 23-Jul-23 01:31 sparseml/pytorch/nn/identity.py
--rw-rw-r--  2.0 unx     2828 b- defN 23-Jul-23 01:31 sparseml/pytorch/nn/se.py
--rw-rw-r--  2.0 unx     1243 b- defN 23-Jul-23 01:31 sparseml/pytorch/optim/__init__.py
--rw-rw-r--  2.0 unx    13638 b- defN 23-Jul-23 01:31 sparseml/pytorch/optim/analyzer_as.py
--rw-rw-r--  2.0 unx    17069 b- defN 23-Jul-23 01:31 sparseml/pytorch/optim/analyzer_module.py
--rw-rw-r--  2.0 unx     3955 b- defN 23-Jul-23 01:31 sparseml/pytorch/optim/analyzer_pruning.py
--rw-rw-r--  2.0 unx    26838 b- defN 23-Jul-23 01:31 sparseml/pytorch/optim/manager.py
--rw-rw-r--  2.0 unx    36844 b- defN 23-Jul-23 01:31 sparseml/pytorch/optim/mask_creator_pruning.py
--rw-rw-r--  2.0 unx    23085 b- defN 23-Jul-23 01:31 sparseml/pytorch/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    10449 b- defN 23-Jul-23 01:31 sparseml/pytorch/optim/mask_pruning_scorer.py
--rw-rw-r--  2.0 unx     6605 b- defN 23-Jul-23 01:31 sparseml/pytorch/optim/optimizer.py
--rw-rw-r--  2.0 unx    14879 b- defN 23-Jul-23 01:31 sparseml/pytorch/optim/sensitivity_as.py
--rw-rw-r--  2.0 unx     6101 b- defN 23-Jul-23 01:31 sparseml/pytorch/optim/sensitivity_lr.py
--rw-rw-r--  2.0 unx     9324 b- defN 23-Jul-23 01:31 sparseml/pytorch/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx      633 b- defN 23-Jul-23 01:31 sparseml/pytorch/recipe_template/__init__.py
--rw-rw-r--  2.0 unx     4534 b- defN 23-Jul-23 01:31 sparseml/pytorch/recipe_template/cli.py
--rw-rw-r--  2.0 unx     1559 b- defN 23-Jul-23 01:31 sparseml/pytorch/recipe_template/description.py
--rw-rw-r--  2.0 unx    15943 b- defN 23-Jul-23 01:31 sparseml/pytorch/recipe_template/main.py
--rw-rw-r--  2.0 unx      992 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1366 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/info.py
--rw-rw-r--  2.0 unx    32014 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/modifier.py
--rw-rw-r--  2.0 unx    18952 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/modifier_thinning.py
--rw-rw-r--  2.0 unx      705 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/distillation/__init__.py
--rw-rw-r--  2.0 unx     4741 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/distillation/modifier_distillation.py
--rw-rw-r--  2.0 unx    14742 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/distillation/modifier_distillation_base.py
--rw-rw-r--  2.0 unx    19177 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/distillation/modifier_per_layer.py
--rw-rw-r--  2.0 unx     1158 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/pruning/__init__.py
--rw-rw-r--  2.0 unx    29250 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/pruning/mask_creator.py
--rw-rw-r--  2.0 unx    22391 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/pruning/mask_params.py
--rw-rw-r--  2.0 unx    13389 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/pruning/modifier_as.py
--rw-rw-r--  2.0 unx    10455 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_acdc.py
--rw-rw-r--  2.0 unx    33219 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_base.py
--rw-rw-r--  2.0 unx     5757 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_constant.py
--rw-rw-r--  2.0 unx     8860 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_layer.py
--rw-rw-r--  2.0 unx    15595 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_magnitude.py
--rw-rw-r--  2.0 unx    63519 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_mfac.py
--rw-rw-r--  2.0 unx     8774 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_movement.py
--rw-rw-r--  2.0 unx    24121 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_obs.py
--rw-rw-r--  2.0 unx    18245 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/pruning/modifier_pruning_structured.py
--rw-rw-r--  2.0 unx     4644 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/pruning/scorer.py
--rw-rw-r--  2.0 unx      813 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/quantization/__init__.py
--rw-rw-r--  2.0 unx     2220 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/quantization/constants.py
--rw-rw-r--  2.0 unx    32271 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/quantization/helpers.py
--rw-rw-r--  2.0 unx    33626 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/quantization/legacy_modifier_quantization.py
--rw-rw-r--  2.0 unx    26778 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/quantization/modifier_quantization.py
--rw-rw-r--  2.0 unx    12558 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/quantization/quantization_scheme.py
--rw-rw-r--  2.0 unx    17905 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/quantization/quantize.py
--rw-rw-r--  2.0 unx    76796 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/quantization/quantize_qat_export.py
--rw-rw-r--  2.0 unx      790 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/training/__init__.py
--rw-rw-r--  2.0 unx     1778 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/training/modifier_epoch.py
--rw-rw-r--  2.0 unx     2883 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/training/modifier_logging.py
--rw-rw-r--  2.0 unx    24287 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/training/modifier_lr.py
--rw-rw-r--  2.0 unx    21497 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/training/modifier_params.py
--rw-rw-r--  2.0 unx     6690 b- defN 23-Jul-23 01:31 sparseml/pytorch/sparsification/training/modifier_regularizer.py
--rw-rw-r--  2.0 unx      943 b- defN 23-Jul-23 01:31 sparseml/pytorch/torchvision/__init__.py
--rw-rw-r--  2.0 unx     6490 b- defN 23-Jul-23 01:31 sparseml/pytorch/torchvision/export_onnx.py
--rw-rw-r--  2.0 unx     2870 b- defN 23-Jul-23 01:31 sparseml/pytorch/torchvision/presets.py
--rw-rw-r--  2.0 unx     2530 b- defN 23-Jul-23 01:31 sparseml/pytorch/torchvision/sampler.py
--rw-rw-r--  2.0 unx    41409 b- defN 23-Jul-23 01:31 sparseml/pytorch/torchvision/train.py
--rw-rw-r--  2.0 unx     7128 b- defN 23-Jul-23 01:31 sparseml/pytorch/torchvision/transforms.py
--rw-rw-r--  2.0 unx    16675 b- defN 23-Jul-23 01:31 sparseml/pytorch/torchvision/utils.py
--rw-rw-r--  2.0 unx     1160 b- defN 23-Jul-23 01:31 sparseml/pytorch/utils/__init__.py
--rw-rw-r--  2.0 unx     9706 b- defN 23-Jul-23 01:31 sparseml/pytorch/utils/benchmarker.py
--rw-rw-r--  2.0 unx     2846 b- defN 23-Jul-23 01:31 sparseml/pytorch/utils/callbacks.py
--rw-rw-r--  2.0 unx     1061 b- defN 23-Jul-23 01:31 sparseml/pytorch/utils/distributed.py
--rw-rw-r--  2.0 unx    31241 b- defN 23-Jul-23 01:31 sparseml/pytorch/utils/exporter.py
--rw-rw-r--  2.0 unx    41226 b- defN 23-Jul-23 01:31 sparseml/pytorch/utils/helpers.py
--rw-rw-r--  2.0 unx     1663 b- defN 23-Jul-23 01:31 sparseml/pytorch/utils/log_sparsification_info.py
--rw-rw-r--  2.0 unx    31374 b- defN 23-Jul-23 01:31 sparseml/pytorch/utils/logger.py
--rw-rw-r--  2.0 unx    27048 b- defN 23-Jul-23 01:31 sparseml/pytorch/utils/loss.py
--rw-rw-r--  2.0 unx    11754 b- defN 23-Jul-23 01:31 sparseml/pytorch/utils/model.py
--rw-rw-r--  2.0 unx    39117 b- defN 23-Jul-23 01:31 sparseml/pytorch/utils/module.py
--rw-rw-r--  2.0 unx     8809 b- defN 23-Jul-23 01:31 sparseml/pytorch/utils/sparsification.py
--rw-rw-r--  2.0 unx    30059 b- defN 23-Jul-23 01:31 sparseml/pytorch/utils/ssd_helpers.py
--rw-rw-r--  2.0 unx    12337 b- defN 23-Jul-23 01:31 sparseml/pytorch/utils/yolo_helpers.py
--rw-rw-r--  2.0 unx      617 b- defN 23-Jul-23 01:31 sparseml/pytorch/utils/sparsification_info/__init__.py
--rw-rw-r--  2.0 unx    10457 b- defN 23-Jul-23 01:31 sparseml/pytorch/utils/sparsification_info/configs.py
--rw-rw-r--  2.0 unx     4309 b- defN 23-Jul-23 01:31 sparseml/pytorch/utils/sparsification_info/helpers.py
--rw-rw-r--  2.0 unx     2946 b- defN 23-Jul-23 01:31 sparseml/pytorch/utils/sparsification_info/module_sparsification_info.py
--rw-rw-r--  2.0 unx      655 b- defN 23-Jul-23 01:31 sparseml/recipe_template/__init__.py
--rw-rw-r--  2.0 unx     4788 b- defN 23-Jul-23 01:31 sparseml/recipe_template/utils.py
--rw-rw-r--  2.0 unx     1058 b- defN 23-Jul-23 01:31 sparseml/sparsification/__init__.py
--rw-rw-r--  2.0 unx     9387 b- defN 23-Jul-23 01:31 sparseml/sparsification/analyzer.py
--rw-rw-r--  2.0 unx     9065 b- defN 23-Jul-23 01:31 sparseml/sparsification/info.py
--rw-rw-r--  2.0 unx    15565 b- defN 23-Jul-23 01:31 sparseml/sparsification/model_info.py
--rw-rw-r--  2.0 unx     2002 b- defN 23-Jul-23 01:31 sparseml/sparsification/modifier_epoch.py
--rw-rw-r--  2.0 unx    10117 b- defN 23-Jul-23 01:31 sparseml/sparsification/modifier_lr.py
--rw-rw-r--  2.0 unx     5505 b- defN 23-Jul-23 01:31 sparseml/sparsification/modifier_params.py
--rw-rw-r--  2.0 unx    12845 b- defN 23-Jul-23 01:31 sparseml/sparsification/modifier_pruning.py
--rw-rw-r--  2.0 unx     3700 b- defN 23-Jul-23 01:31 sparseml/sparsification/oracle.py
--rw-rw-r--  2.0 unx    18570 b- defN 23-Jul-23 01:31 sparseml/sparsification/recipe_builder.py
--rw-rw-r--  2.0 unx    14413 b- defN 23-Jul-23 01:31 sparseml/sparsification/recipe_editor.py
--rw-rw-r--  2.0 unx     1250 b- defN 23-Jul-23 01:31 sparseml/sparsification/types.py
--rw-rw-r--  2.0 unx     1169 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/__init__.py
--rw-rw-r--  2.0 unx     7272 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/base.py
--rw-rw-r--  2.0 unx      925 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/datasets/__init__.py
--rw-rw-r--  2.0 unx     8121 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/datasets/dataset.py
--rw-rw-r--  2.0 unx     5600 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/datasets/helpers.py
--rw-rw-r--  2.0 unx     2768 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/datasets/registry.py
--rw-rw-r--  2.0 unx      807 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx    12686 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/datasets/classification/cifar.py
--rw-rw-r--  2.0 unx     8690 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     2032 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     4695 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx      805 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/framework/__init__.py
--rw-rw-r--  2.0 unx     5859 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/framework/info.py
--rw-rw-r--  2.0 unx      925 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/models/__init__.py
--rw-rw-r--  2.0 unx    19752 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/models/estimator.py
--rw-rw-r--  2.0 unx    14774 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/models/registry.py
--rw-rw-r--  2.0 unx      822 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/models/classification/__init__.py
--rw-rw-r--  2.0 unx     3540 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/models/classification/mnist.py
--rw-rw-r--  2.0 unx    11161 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/models/classification/mobilenet.py
--rw-rw-r--  2.0 unx    18359 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/models/classification/mobilenet_v2.py
--rw-rw-r--  2.0 unx    28103 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/models/classification/resnet.py
--rw-rw-r--  2.0 unx    26886 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/models/classification/vgg.py
--rw-rw-r--  2.0 unx      865 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/nn/__init__.py
--rw-rw-r--  2.0 unx    18670 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/nn/layers.py
--rw-rw-r--  2.0 unx     1238 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/optim/__init__.py
--rw-rw-r--  2.0 unx     8607 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/optim/analyzer_module.py
--rw-rw-r--  2.0 unx     9591 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/optim/manager.py
--rw-rw-r--  2.0 unx    19683 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/optim/mask_creator_pruning.py
--rw-rw-r--  2.0 unx    33919 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    15955 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/optim/modifier.py
--rw-rw-r--  2.0 unx     1715 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/optim/modifier_epoch.py
--rw-rw-r--  2.0 unx    10685 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/optim/modifier_lr.py
--rw-rw-r--  2.0 unx     7092 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/optim/modifier_params.py
--rw-rw-r--  2.0 unx    15702 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/optim/modifier_pruning.py
--rw-rw-r--  2.0 unx     5682 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/optim/schedule_lr.py
--rw-rw-r--  2.0 unx     9232 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx      801 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1385 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/sparsification/info.py
--rw-rw-r--  2.0 unx      967 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/utils/__init__.py
--rw-rw-r--  2.0 unx    10913 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/utils/exporter.py
--rw-rw-r--  2.0 unx      996 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/utils/helpers.py
--rw-rw-r--  2.0 unx     1974 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/utils/loss.py
--rw-rw-r--  2.0 unx     8119 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/utils/nets_utils.py
--rw-rw-r--  2.0 unx     1327 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/utils/summary.py
--rw-rw-r--  2.0 unx    12536 b- defN 23-Jul-23 01:31 sparseml/tensorflow_v1/utils/variable.py
--rw-rw-r--  2.0 unx     1511 b- defN 23-Jul-23 01:31 sparseml/transformers/__init__.py
--rw-rw-r--  2.0 unx    22048 b- defN 23-Jul-23 01:31 sparseml/transformers/export.py
--rw-rw-r--  2.0 unx    30756 b- defN 23-Jul-23 01:31 sparseml/transformers/masked_language_modeling.py
--rw-rw-r--  2.0 unx    36976 b- defN 23-Jul-23 01:31 sparseml/transformers/question_answering.py
--rw-rw-r--  2.0 unx    40299 b- defN 23-Jul-23 01:31 sparseml/transformers/text_classification.py
--rw-rw-r--  2.0 unx    34350 b- defN 23-Jul-23 01:31 sparseml/transformers/token_classification.py
--rw-rw-r--  2.0 unx      833 b- defN 23-Jul-23 01:31 sparseml/transformers/sparsification/__init__.py
--rw-rw-r--  2.0 unx    19529 b- defN 23-Jul-23 01:31 sparseml/transformers/sparsification/question_answering.py
--rw-rw-r--  2.0 unx    44413 b- defN 23-Jul-23 01:31 sparseml/transformers/sparsification/trainer.py
--rw-rw-r--  2.0 unx     1890 b- defN 23-Jul-23 01:31 sparseml/transformers/sparsification/training_args.py
--rw-rw-r--  2.0 unx      794 b- defN 23-Jul-23 01:31 sparseml/transformers/utils/__init__.py
--rw-rw-r--  2.0 unx     3090 b- defN 23-Jul-23 01:31 sparseml/transformers/utils/helpers.py
--rw-rw-r--  2.0 unx     2536 b- defN 23-Jul-23 01:31 sparseml/transformers/utils/metrics.py
--rw-rw-r--  2.0 unx    17074 b- defN 23-Jul-23 01:31 sparseml/transformers/utils/model.py
--rw-rw-r--  2.0 unx      844 b- defN 23-Jul-23 01:31 sparseml/utils/__init__.py
--rw-rw-r--  2.0 unx      886 b- defN 23-Jul-23 01:31 sparseml/utils/frameworks.py
--rw-rw-r--  2.0 unx    26562 b- defN 23-Jul-23 01:31 sparseml/utils/helpers.py
--rw-rw-r--  2.0 unx     3983 b- defN 23-Jul-23 01:31 sparseml/utils/restricted_eval.py
--rw-rw-r--  2.0 unx     1083 b- defN 23-Jul-23 01:31 sparseml/utils/singleton.py
--rw-rw-r--  2.0 unx     6312 b- defN 23-Jul-23 01:31 sparseml/utils/worker.py
--rw-rw-r--  2.0 unx     2952 b- defN 23-Jul-23 01:31 sparseml/utils/wrapper.py
--rw-rw-r--  2.0 unx      819 b- defN 23-Jul-23 01:31 sparseml/utils/datasets/__init__.py
--rw-rw-r--  2.0 unx      833 b- defN 23-Jul-23 01:31 sparseml/utils/datasets/cifar.py
--rw-rw-r--  2.0 unx     3750 b- defN 23-Jul-23 01:31 sparseml/utils/datasets/coco.py
--rw-rw-r--  2.0 unx     1217 b- defN 23-Jul-23 01:31 sparseml/utils/datasets/helpers.py
--rw-rw-r--  2.0 unx    23366 b- defN 23-Jul-23 01:31 sparseml/utils/datasets/imagenet.py
--rw-rw-r--  2.0 unx     8967 b- defN 23-Jul-23 01:31 sparseml/utils/datasets/imagenette.py
--rw-rw-r--  2.0 unx     1009 b- defN 23-Jul-23 01:31 sparseml/utils/datasets/voc.py
--rw-rw-r--  2.0 unx     1875 b- defN 23-Jul-23 01:31 sparseml/yolact/COCO.sh
--rw-rw-r--  2.0 unx     1418 b- defN 23-Jul-23 01:31 sparseml/yolact/COCO_test.sh
--rw-rw-r--  2.0 unx     4020 b- defN 23-Jul-23 01:31 sparseml/yolact/__init__.py
--rw-rw-r--  2.0 unx     1784 b- defN 23-Jul-23 01:31 sparseml/yolact/scripts.py
--rw-rw-r--  2.0 unx     1440 b- defN 23-Jul-23 01:31 sparseml/yolov5/__init__.py
--rw-rw-r--  2.0 unx     4505 b- defN 23-Jul-23 01:31 sparseml/yolov5/helpers.py
--rw-rw-r--  2.0 unx     1609 b- defN 23-Jul-23 01:31 sparseml/yolov5/scripts.py
--rw-rw-r--  2.0 unx     1220 b- defN 23-Jul-23 01:31 sparseml/yolov5/yolov5.status.yaml
--rw-rw-r--  2.0 unx     1115 b- defN 23-Jul-23 01:31 sparseml/yolov8/__init__.py
--rw-rw-r--  2.0 unx     5781 b- defN 23-Jul-23 01:31 sparseml/yolov8/default.yaml
--rw-rw-r--  2.0 unx     2502 b- defN 23-Jul-23 01:31 sparseml/yolov8/export.py
--rw-rw-r--  2.0 unx     2259 b- defN 23-Jul-23 01:31 sparseml/yolov8/modules.py
--rw-rw-r--  2.0 unx     7194 b- defN 23-Jul-23 01:31 sparseml/yolov8/train.py
--rw-rw-r--  2.0 unx    35999 b- defN 23-Jul-23 01:31 sparseml/yolov8/trainers.py
--rw-rw-r--  2.0 unx     2748 b- defN 23-Jul-23 01:31 sparseml/yolov8/val.py
--rw-rw-r--  2.0 unx     8196 b- defN 23-Jul-23 01:31 sparseml/yolov8/validators.py
--rw-rw-r--  2.0 unx      685 b- defN 23-Jul-23 01:31 sparseml/yolov8/utils/__init__.py
--rw-rw-r--  2.0 unx     6247 b- defN 23-Jul-23 01:31 sparseml/yolov8/utils/export_samples.py
--rw-rw-r--  2.0 unx     4041 b- defN 23-Jul-23 01:31 sparseml/yolov8/utils/helpers.py
--rw-rw-r--  2.0 unx    11357 b- defN 23-Jul-23 01:33 sparseml_nightly-1.6.0.20230723.dist-info/LICENSE
--rw-rw-r--  2.0 unx    21837 b- defN 23-Jul-23 01:33 sparseml_nightly-1.6.0.20230723.dist-info/METADATA
--rw-rw-r--  2.0 unx     2158 b- defN 23-Jul-23 01:33 sparseml_nightly-1.6.0.20230723.dist-info/NOTICE
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-23 01:33 sparseml_nightly-1.6.0.20230723.dist-info/WHEEL
--rw-rw-r--  2.0 unx     2326 b- defN 23-Jul-23 01:33 sparseml_nightly-1.6.0.20230723.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 23-Jul-23 01:33 sparseml_nightly-1.6.0.20230723.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    37503 b- defN 23-Jul-23 01:33 sparseml_nightly-1.6.0.20230723.dist-info/RECORD
-376 files, 3509348 bytes uncompressed, 909128 bytes compressed:  74.1%
+Zip file size: 973141 bytes, number of entries: 376
+-rw-rw-r--  2.0 unx     1413 b- defN 23-Aug-01 13:43 sparseml/__init__.py
+-rw-rw-r--  2.0 unx      898 b- defN 23-Aug-01 13:43 sparseml/analytics.py
+-rw-rw-r--  2.0 unx    10284 b- defN 23-Aug-01 13:43 sparseml/base.py
+-rw-rw-r--  2.0 unx     2483 b- defN 23-Aug-01 13:43 sparseml/log.py
+-rw-rw-r--  2.0 unx     1511 b- defN 23-Aug-01 13:43 sparseml/version.py
+-rw-rw-r--  2.0 unx      758 b- defN 23-Aug-01 13:43 sparseml/benchmark/__init__.py
+-rw-rw-r--  2.0 unx    17763 b- defN 23-Aug-01 13:43 sparseml/benchmark/info.py
+-rw-rw-r--  2.0 unx    10778 b- defN 23-Aug-01 13:43 sparseml/benchmark/serialization.py
+-rw-rw-r--  2.0 unx      863 b- defN 23-Aug-01 13:43 sparseml/deepsparse/__init__.py
+-rw-rw-r--  2.0 unx     3516 b- defN 23-Aug-01 13:43 sparseml/deepsparse/base.py
+-rw-rw-r--  2.0 unx      801 b- defN 23-Aug-01 13:43 sparseml/deepsparse/framework/__init__.py
+-rw-rw-r--  2.0 unx     6032 b- defN 23-Aug-01 13:43 sparseml/deepsparse/framework/info.py
+-rw-rw-r--  2.0 unx      813 b- defN 23-Aug-01 13:43 sparseml/deepsparse/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1348 b- defN 23-Aug-01 13:43 sparseml/deepsparse/sparsification/info.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-Aug-01 13:43 sparseml/exporters/__init__.py
+-rw-rw-r--  2.0 unx     1477 b- defN 23-Aug-01 13:43 sparseml/exporters/base_exporter.py
+-rw-rw-r--  2.0 unx     6576 b- defN 23-Aug-01 13:43 sparseml/exporters/kv_cache_injector.py
+-rw-rw-r--  2.0 unx     5010 b- defN 23-Aug-01 13:43 sparseml/exporters/onnx_to_deepsparse.py
+-rw-rw-r--  2.0 unx     2350 b- defN 23-Aug-01 13:43 sparseml/exporters/transforms/__init__.py
+-rw-rw-r--  2.0 unx     2333 b- defN 23-Aug-01 13:43 sparseml/exporters/transforms/base_transform.py
+-rw-rw-r--  2.0 unx     1388 b- defN 23-Aug-01 13:43 sparseml/exporters/transforms/constants_to_initializers.py
+-rw-rw-r--  2.0 unx     4630 b- defN 23-Aug-01 13:43 sparseml/exporters/transforms/conv_to_convinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     5973 b- defN 23-Aug-01 13:43 sparseml/exporters/transforms/conv_to_qlinearconv.py
+-rw-rw-r--  2.0 unx     2440 b- defN 23-Aug-01 13:43 sparseml/exporters/transforms/delete_repeated_qdq.py
+-rw-rw-r--  2.0 unx     1842 b- defN 23-Aug-01 13:43 sparseml/exporters/transforms/delete_trivial_onnx_adds.py
+-rw-rw-r--  2.0 unx     2181 b- defN 23-Aug-01 13:43 sparseml/exporters/transforms/flatten_qparams.py
+-rw-rw-r--  2.0 unx     3553 b- defN 23-Aug-01 13:43 sparseml/exporters/transforms/fold_conv_div_bn.py
+-rw-rw-r--  2.0 unx     1669 b- defN 23-Aug-01 13:43 sparseml/exporters/transforms/fold_identity_initializers.py
+-rw-rw-r--  2.0 unx     2070 b- defN 23-Aug-01 13:43 sparseml/exporters/transforms/fold_relu_quants.py
+-rw-rw-r--  2.0 unx     4418 b- defN 23-Aug-01 13:43 sparseml/exporters/transforms/gemm_to_matmulinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     7629 b- defN 23-Aug-01 13:43 sparseml/exporters/transforms/gemm_to_qlinearmatmul.py
+-rw-rw-r--  2.0 unx     1645 b- defN 23-Aug-01 13:43 sparseml/exporters/transforms/initializers_to_uint8.py
+-rw-rw-r--  2.0 unx     6297 b- defN 23-Aug-01 13:43 sparseml/exporters/transforms/matmul_add_to_matmulinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     4681 b- defN 23-Aug-01 13:43 sparseml/exporters/transforms/matmul_to_matmulinteger_cast_mul.py
+-rw-rw-r--  2.0 unx     4156 b- defN 23-Aug-01 13:43 sparseml/exporters/transforms/matmul_to_qlinearmatmul.py
+-rw-rw-r--  2.0 unx     3724 b- defN 23-Aug-01 13:43 sparseml/exporters/transforms/onnx_transform.py
+-rw-rw-r--  2.0 unx     3433 b- defN 23-Aug-01 13:43 sparseml/exporters/transforms/propagate_dequant_through_split.py
+-rw-rw-r--  2.0 unx     4801 b- defN 23-Aug-01 13:43 sparseml/exporters/transforms/propagate_embedding_quantization.py
+-rw-rw-r--  2.0 unx     4464 b- defN 23-Aug-01 13:43 sparseml/exporters/transforms/quantize_qat_embedding.py
+-rw-rw-r--  2.0 unx     3869 b- defN 23-Aug-01 13:43 sparseml/exporters/transforms/quantize_residuals.py
+-rw-rw-r--  2.0 unx     3331 b- defN 23-Aug-01 13:43 sparseml/exporters/transforms/remove_duplicate_qconv_weights.py
+-rw-rw-r--  2.0 unx     2545 b- defN 23-Aug-01 13:43 sparseml/exporters/transforms/remove_duplicate_quantize_ops.py
+-rw-rw-r--  2.0 unx     3210 b- defN 23-Aug-01 13:43 sparseml/exporters/transforms/skip_input_quantize.py
+-rw-rw-r--  2.0 unx     1373 b- defN 23-Aug-01 13:43 sparseml/exporters/transforms/unwrap_batchnorms.py
+-rw-rw-r--  2.0 unx      879 b- defN 23-Aug-01 13:43 sparseml/exporters/transforms/kv_cache/__init__.py
+-rw-rw-r--  2.0 unx    30558 b- defN 23-Aug-01 13:43 sparseml/exporters/transforms/kv_cache/cache_keys_and_values.py
+-rw-rw-r--  2.0 unx     6427 b- defN 23-Aug-01 13:43 sparseml/exporters/transforms/kv_cache/configs.py
+-rw-rw-r--  2.0 unx     7027 b- defN 23-Aug-01 13:43 sparseml/exporters/transforms/kv_cache/transforms_base.py
+-rw-rw-r--  2.0 unx     4974 b- defN 23-Aug-01 13:43 sparseml/exporters/transforms/kv_cache/transforms_codegen.py
+-rw-rw-r--  2.0 unx     6066 b- defN 23-Aug-01 13:43 sparseml/exporters/transforms/kv_cache/transforms_opt.py
+-rw-rw-r--  2.0 unx      730 b- defN 23-Aug-01 13:43 sparseml/exporters/transforms/utils/__init__.py
+-rw-rw-r--  2.0 unx    11112 b- defN 23-Aug-01 13:43 sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py
+-rw-rw-r--  2.0 unx     6809 b- defN 23-Aug-01 13:43 sparseml/exporters/transforms/utils/helpers.py
+-rw-rw-r--  2.0 unx    14429 b- defN 23-Aug-01 13:43 sparseml/exporters/transforms/utils/matching.py
+-rw-rw-r--  2.0 unx      790 b- defN 23-Aug-01 13:43 sparseml/framework/__init__.py
+-rw-rw-r--  2.0 unx     9479 b- defN 23-Aug-01 13:43 sparseml/framework/info.py
+-rw-rw-r--  2.0 unx     1144 b- defN 23-Aug-01 13:43 sparseml/keras/__init__.py
+-rw-rw-r--  2.0 unx     8054 b- defN 23-Aug-01 13:43 sparseml/keras/base.py
+-rw-rw-r--  2.0 unx      943 b- defN 23-Aug-01 13:43 sparseml/keras/datasets/__init__.py
+-rw-rw-r--  2.0 unx     3297 b- defN 23-Aug-01 13:43 sparseml/keras/datasets/dataset.py
+-rw-rw-r--  2.0 unx     2423 b- defN 23-Aug-01 13:43 sparseml/keras/datasets/helpers.py
+-rw-rw-r--  2.0 unx     2761 b- defN 23-Aug-01 13:43 sparseml/keras/datasets/registry.py
+-rw-rw-r--  2.0 unx      786 b- defN 23-Aug-01 13:43 sparseml/keras/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx     8369 b- defN 23-Aug-01 13:43 sparseml/keras/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     4301 b- defN 23-Aug-01 13:43 sparseml/keras/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     2727 b- defN 23-Aug-01 13:43 sparseml/keras/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx      793 b- defN 23-Aug-01 13:43 sparseml/keras/framework/__init__.py
+-rw-rw-r--  2.0 unx     5906 b- defN 23-Aug-01 13:43 sparseml/keras/framework/info.py
+-rw-rw-r--  2.0 unx      921 b- defN 23-Aug-01 13:43 sparseml/keras/models/__init__.py
+-rw-rw-r--  2.0 unx    11814 b- defN 23-Aug-01 13:43 sparseml/keras/models/registry.py
+-rw-rw-r--  2.0 unx      656 b- defN 23-Aug-01 13:43 sparseml/keras/models/classification/__init__.py
+-rw-rw-r--  2.0 unx    17932 b- defN 23-Aug-01 13:43 sparseml/keras/models/classification/resnet.py
+-rw-rw-r--  2.0 unx      768 b- defN 23-Aug-01 13:43 sparseml/keras/models/external/__init__.py
+-rw-rw-r--  2.0 unx     4402 b- defN 23-Aug-01 13:43 sparseml/keras/models/external/keras_applications.py
+-rw-rw-r--  2.0 unx     1166 b- defN 23-Aug-01 13:43 sparseml/keras/optim/__init__.py
+-rw-rw-r--  2.0 unx     5677 b- defN 23-Aug-01 13:43 sparseml/keras/optim/manager.py
+-rw-rw-r--  2.0 unx    14777 b- defN 23-Aug-01 13:43 sparseml/keras/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    19740 b- defN 23-Aug-01 13:43 sparseml/keras/optim/mask_pruning_creator.py
+-rw-rw-r--  2.0 unx     9183 b- defN 23-Aug-01 13:43 sparseml/keras/optim/modifier.py
+-rw-rw-r--  2.0 unx     1676 b- defN 23-Aug-01 13:43 sparseml/keras/optim/modifier_epoch.py
+-rw-rw-r--  2.0 unx    14736 b- defN 23-Aug-01 13:43 sparseml/keras/optim/modifier_lr.py
+-rw-rw-r--  2.0 unx     5477 b- defN 23-Aug-01 13:43 sparseml/keras/optim/modifier_params.py
+-rw-rw-r--  2.0 unx    24031 b- defN 23-Aug-01 13:43 sparseml/keras/optim/modifier_pruning.py
+-rw-rw-r--  2.0 unx     1133 b- defN 23-Aug-01 13:43 sparseml/keras/optim/utils.py
+-rw-rw-r--  2.0 unx      808 b- defN 23-Aug-01 13:43 sparseml/keras/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1356 b- defN 23-Aug-01 13:43 sparseml/keras/sparsification/info.py
+-rw-rw-r--  2.0 unx      962 b- defN 23-Aug-01 13:43 sparseml/keras/utils/__init__.py
+-rw-rw-r--  2.0 unx     8202 b- defN 23-Aug-01 13:43 sparseml/keras/utils/callbacks.py
+-rw-rw-r--  2.0 unx     1022 b- defN 23-Aug-01 13:43 sparseml/keras/utils/compat.py
+-rw-rw-r--  2.0 unx     5737 b- defN 23-Aug-01 13:43 sparseml/keras/utils/exporter.py
+-rw-rw-r--  2.0 unx     6087 b- defN 23-Aug-01 13:43 sparseml/keras/utils/logger.py
+-rw-rw-r--  2.0 unx     1738 b- defN 23-Aug-01 13:43 sparseml/keras/utils/model.py
+-rw-rw-r--  2.0 unx     1036 b- defN 23-Aug-01 13:43 sparseml/onnx/__init__.py
+-rw-rw-r--  2.0 unx     6202 b- defN 23-Aug-01 13:43 sparseml/onnx/base.py
+-rw-rw-r--  2.0 unx      743 b- defN 23-Aug-01 13:43 sparseml/onnx/benchmark/__init__.py
+-rw-rw-r--  2.0 unx    15366 b- defN 23-Aug-01 13:43 sparseml/onnx/benchmark/info.py
+-rw-rw-r--  2.0 unx      823 b- defN 23-Aug-01 13:43 sparseml/onnx/framework/__init__.py
+-rw-rw-r--  2.0 unx     6116 b- defN 23-Aug-01 13:43 sparseml/onnx/framework/info.py
+-rw-rw-r--  2.0 unx      820 b- defN 23-Aug-01 13:43 sparseml/onnx/optim/__init__.py
+-rw-rw-r--  2.0 unx    13285 b- defN 23-Aug-01 13:43 sparseml/onnx/optim/analyzer_model.py
+-rw-rw-r--  2.0 unx    19639 b- defN 23-Aug-01 13:43 sparseml/onnx/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx     6470 b- defN 23-Aug-01 13:43 sparseml/onnx/optim/structured_pruning.py
+-rw-rw-r--  2.0 unx      815 b- defN 23-Aug-01 13:43 sparseml/onnx/optim/quantization/__init__.py
+-rw-rw-r--  2.0 unx    14753 b- defN 23-Aug-01 13:43 sparseml/onnx/optim/quantization/calibration.py
+-rw-rw-r--  2.0 unx    73551 b- defN 23-Aug-01 13:43 sparseml/onnx/optim/quantization/quantize.py
+-rw-rw-r--  2.0 unx     4552 b- defN 23-Aug-01 13:43 sparseml/onnx/optim/quantization/quantize_model_post_training.py
+-rw-rw-r--  2.0 unx      869 b- defN 23-Aug-01 13:43 sparseml/onnx/sparsification/__init__.py
+-rw-rw-r--  2.0 unx    10209 b- defN 23-Aug-01 13:43 sparseml/onnx/sparsification/analyzer.py
+-rw-rw-r--  2.0 unx     1363 b- defN 23-Aug-01 13:43 sparseml/onnx/sparsification/info.py
+-rw-rw-r--  2.0 unx     8009 b- defN 23-Aug-01 13:43 sparseml/onnx/sparsification/model_info.py
+-rw-rw-r--  2.0 unx      867 b- defN 23-Aug-01 13:43 sparseml/onnx/utils/__init__.py
+-rw-rw-r--  2.0 unx    13013 b- defN 23-Aug-01 13:43 sparseml/onnx/utils/data.py
+-rw-rw-r--  2.0 unx    20691 b- defN 23-Aug-01 13:43 sparseml/onnx/utils/graph_editor.py
+-rw-rw-r--  2.0 unx     8133 b- defN 23-Aug-01 13:43 sparseml/onnx/utils/graph_optimizer.py
+-rw-rw-r--  2.0 unx    40230 b- defN 23-Aug-01 13:43 sparseml/onnx/utils/helpers.py
+-rw-rw-r--  2.0 unx     1958 b- defN 23-Aug-01 13:43 sparseml/onnx/utils/loss.py
+-rw-rw-r--  2.0 unx    31591 b- defN 23-Aug-01 13:43 sparseml/onnx/utils/model.py
+-rw-rw-r--  2.0 unx     5437 b- defN 23-Aug-01 13:43 sparseml/onnx/utils/sparse_tensor.py
+-rw-rw-r--  2.0 unx      931 b- defN 23-Aug-01 13:43 sparseml/openpifpaf/__init__.py
+-rw-rw-r--  2.0 unx     3713 b- defN 23-Aug-01 13:43 sparseml/openpifpaf/export.py
+-rw-rw-r--  2.0 unx    10950 b- defN 23-Aug-01 13:43 sparseml/openpifpaf/train.py
+-rw-rw-r--  2.0 unx     4211 b- defN 23-Aug-01 13:43 sparseml/openpifpaf/trainer.py
+-rw-rw-r--  2.0 unx      882 b- defN 23-Aug-01 13:43 sparseml/optim/__init__.py
+-rw-rw-r--  2.0 unx     6302 b- defN 23-Aug-01 13:43 sparseml/optim/analyzer.py
+-rw-rw-r--  2.0 unx    25563 b- defN 23-Aug-01 13:43 sparseml/optim/helpers.py
+-rw-rw-r--  2.0 unx    25984 b- defN 23-Aug-01 13:43 sparseml/optim/manager.py
+-rw-rw-r--  2.0 unx    30708 b- defN 23-Aug-01 13:43 sparseml/optim/modifier.py
+-rw-rw-r--  2.0 unx    26315 b- defN 23-Aug-01 13:43 sparseml/optim/sensitivity.py
+-rw-rw-r--  2.0 unx     2190 b- defN 23-Aug-01 13:43 sparseml/pytorch/__init__.py
+-rw-rw-r--  2.0 unx     6155 b- defN 23-Aug-01 13:43 sparseml/pytorch/base.py
+-rw-rw-r--  2.0 unx      933 b- defN 23-Aug-01 13:43 sparseml/pytorch/opset.py
+-rw-rw-r--  2.0 unx    11013 b- defN 23-Aug-01 13:43 sparseml/pytorch/torch_to_onnx_exporter.py
+-rw-rw-r--  2.0 unx      998 b- defN 23-Aug-01 13:43 sparseml/pytorch/datasets/__init__.py
+-rw-rw-r--  2.0 unx     4193 b- defN 23-Aug-01 13:43 sparseml/pytorch/datasets/generic.py
+-rw-rw-r--  2.0 unx     3014 b- defN 23-Aug-01 13:43 sparseml/pytorch/datasets/registry.py
+-rw-rw-r--  2.0 unx      828 b- defN 23-Aug-01 13:43 sparseml/pytorch/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx     4457 b- defN 23-Aug-01 13:43 sparseml/pytorch/datasets/classification/cifar.py
+-rw-rw-r--  2.0 unx     3669 b- defN 23-Aug-01 13:43 sparseml/pytorch/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     4000 b- defN 23-Aug-01 13:43 sparseml/pytorch/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     6491 b- defN 23-Aug-01 13:43 sparseml/pytorch/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx     2434 b- defN 23-Aug-01 13:43 sparseml/pytorch/datasets/classification/mnist.py
+-rw-rw-r--  2.0 unx      767 b- defN 23-Aug-01 13:43 sparseml/pytorch/datasets/detection/__init__.py
+-rw-rw-r--  2.0 unx    16159 b- defN 23-Aug-01 13:43 sparseml/pytorch/datasets/detection/coco.py
+-rw-rw-r--  2.0 unx     5705 b- defN 23-Aug-01 13:43 sparseml/pytorch/datasets/detection/helpers.py
+-rw-rw-r--  2.0 unx    10759 b- defN 23-Aug-01 13:43 sparseml/pytorch/datasets/detection/voc.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-Aug-01 13:43 sparseml/pytorch/datasets/image_classification/__init__.py
+-rw-rw-r--  2.0 unx     9512 b- defN 23-Aug-01 13:43 sparseml/pytorch/datasets/image_classification/ffcv_dataset.py
+-rw-rw-r--  2.0 unx      684 b- defN 23-Aug-01 13:43 sparseml/pytorch/datasets/recommendation/__init__.py
+-rw-rw-r--  2.0 unx      693 b- defN 23-Aug-01 13:43 sparseml/pytorch/datasets/video/__init__.py
+-rw-rw-r--  2.0 unx      814 b- defN 23-Aug-01 13:43 sparseml/pytorch/framework/__init__.py
+-rw-rw-r--  2.0 unx     5580 b- defN 23-Aug-01 13:43 sparseml/pytorch/framework/info.py
+-rw-rw-r--  2.0 unx      753 b- defN 23-Aug-01 13:43 sparseml/pytorch/image_classification/__init__.py
+-rw-rw-r--  2.0 unx    18265 b- defN 23-Aug-01 13:43 sparseml/pytorch/image_classification/export.py
+-rw-rw-r--  2.0 unx    15494 b- defN 23-Aug-01 13:43 sparseml/pytorch/image_classification/lr_analysis.py
+-rw-rw-r--  2.0 unx    14444 b- defN 23-Aug-01 13:43 sparseml/pytorch/image_classification/pr_sensitivity.py
+-rw-rw-r--  2.0 unx    29287 b- defN 23-Aug-01 13:43 sparseml/pytorch/image_classification/train.py
+-rw-rw-r--  2.0 unx      682 b- defN 23-Aug-01 13:43 sparseml/pytorch/image_classification/utils/__init__.py
+-rw-rw-r--  2.0 unx     4278 b- defN 23-Aug-01 13:43 sparseml/pytorch/image_classification/utils/cli_helpers.py
+-rw-rw-r--  2.0 unx     1257 b- defN 23-Aug-01 13:43 sparseml/pytorch/image_classification/utils/constants.py
+-rw-rw-r--  2.0 unx    21742 b- defN 23-Aug-01 13:43 sparseml/pytorch/image_classification/utils/helpers.py
+-rw-rw-r--  2.0 unx    12056 b- defN 23-Aug-01 13:43 sparseml/pytorch/image_classification/utils/trainer.py
+-rw-rw-r--  2.0 unx      976 b- defN 23-Aug-01 13:43 sparseml/pytorch/models/__init__.py
+-rw-rw-r--  2.0 unx    14753 b- defN 23-Aug-01 13:43 sparseml/pytorch/models/registry.py
+-rw-rw-r--  2.0 unx      901 b- defN 23-Aug-01 13:43 sparseml/pytorch/models/classification/__init__.py
+-rw-rw-r--  2.0 unx    11658 b- defN 23-Aug-01 13:43 sparseml/pytorch/models/classification/darknet.py
+-rw-rw-r--  2.0 unx    40293 b- defN 23-Aug-01 13:43 sparseml/pytorch/models/classification/efficientnet.py
+-rw-rw-r--  2.0 unx    16512 b- defN 23-Aug-01 13:43 sparseml/pytorch/models/classification/inception_v3.py
+-rw-rw-r--  2.0 unx     4164 b- defN 23-Aug-01 13:43 sparseml/pytorch/models/classification/mnist.py
+-rw-rw-r--  2.0 unx     9546 b- defN 23-Aug-01 13:43 sparseml/pytorch/models/classification/mobilenet.py
+-rw-rw-r--  2.0 unx    13014 b- defN 23-Aug-01 13:43 sparseml/pytorch/models/classification/mobilenet_v2.py
+-rw-rw-r--  2.0 unx    40800 b- defN 23-Aug-01 13:43 sparseml/pytorch/models/classification/resnet.py
+-rw-rw-r--  2.0 unx    16649 b- defN 23-Aug-01 13:43 sparseml/pytorch/models/classification/vgg.py
+-rw-rw-r--  2.0 unx      824 b- defN 23-Aug-01 13:43 sparseml/pytorch/models/detection/__init__.py
+-rw-rw-r--  2.0 unx     6820 b- defN 23-Aug-01 13:43 sparseml/pytorch/models/detection/ssd.py
+-rw-rw-r--  2.0 unx     8116 b- defN 23-Aug-01 13:43 sparseml/pytorch/models/detection/ssd_lite.py
+-rw-rw-r--  2.0 unx     4046 b- defN 23-Aug-01 13:43 sparseml/pytorch/models/detection/ssd_mobilenet.py
+-rw-rw-r--  2.0 unx     9069 b- defN 23-Aug-01 13:43 sparseml/pytorch/models/detection/ssd_resnet.py
+-rw-rw-r--  2.0 unx    10188 b- defN 23-Aug-01 13:43 sparseml/pytorch/models/detection/yolo_v3.py
+-rw-rw-r--  2.0 unx      763 b- defN 23-Aug-01 13:43 sparseml/pytorch/models/external/__init__.py
+-rw-rw-r--  2.0 unx     6759 b- defN 23-Aug-01 13:43 sparseml/pytorch/models/external/torchvision.py
+-rw-rw-r--  2.0 unx      676 b- defN 23-Aug-01 13:43 sparseml/pytorch/models/recommendation/__init__.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Aug-01 13:43 sparseml/pytorch/nn/__init__.py
+-rw-rw-r--  2.0 unx     8673 b- defN 23-Aug-01 13:43 sparseml/pytorch/nn/activations.py
+-rw-rw-r--  2.0 unx    11854 b- defN 23-Aug-01 13:43 sparseml/pytorch/nn/fatrelu.py
+-rw-rw-r--  2.0 unx     1690 b- defN 23-Aug-01 13:43 sparseml/pytorch/nn/identity.py
+-rw-rw-r--  2.0 unx     2828 b- defN 23-Aug-01 13:43 sparseml/pytorch/nn/se.py
+-rw-rw-r--  2.0 unx     1243 b- defN 23-Aug-01 13:43 sparseml/pytorch/optim/__init__.py
+-rw-rw-r--  2.0 unx    13638 b- defN 23-Aug-01 13:43 sparseml/pytorch/optim/analyzer_as.py
+-rw-rw-r--  2.0 unx    17069 b- defN 23-Aug-01 13:43 sparseml/pytorch/optim/analyzer_module.py
+-rw-rw-r--  2.0 unx     3955 b- defN 23-Aug-01 13:43 sparseml/pytorch/optim/analyzer_pruning.py
+-rw-rw-r--  2.0 unx    26838 b- defN 23-Aug-01 13:43 sparseml/pytorch/optim/manager.py
+-rw-rw-r--  2.0 unx    36844 b- defN 23-Aug-01 13:43 sparseml/pytorch/optim/mask_creator_pruning.py
+-rw-rw-r--  2.0 unx    23085 b- defN 23-Aug-01 13:43 sparseml/pytorch/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    10449 b- defN 23-Aug-01 13:43 sparseml/pytorch/optim/mask_pruning_scorer.py
+-rw-rw-r--  2.0 unx     6605 b- defN 23-Aug-01 13:43 sparseml/pytorch/optim/optimizer.py
+-rw-rw-r--  2.0 unx    14879 b- defN 23-Aug-01 13:43 sparseml/pytorch/optim/sensitivity_as.py
+-rw-rw-r--  2.0 unx     6101 b- defN 23-Aug-01 13:43 sparseml/pytorch/optim/sensitivity_lr.py
+-rw-rw-r--  2.0 unx     9324 b- defN 23-Aug-01 13:43 sparseml/pytorch/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx      633 b- defN 23-Aug-01 13:43 sparseml/pytorch/recipe_template/__init__.py
+-rw-rw-r--  2.0 unx     4534 b- defN 23-Aug-01 13:43 sparseml/pytorch/recipe_template/cli.py
+-rw-rw-r--  2.0 unx     1559 b- defN 23-Aug-01 13:43 sparseml/pytorch/recipe_template/description.py
+-rw-rw-r--  2.0 unx    15943 b- defN 23-Aug-01 13:43 sparseml/pytorch/recipe_template/main.py
+-rw-rw-r--  2.0 unx      992 b- defN 23-Aug-01 13:43 sparseml/pytorch/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1366 b- defN 23-Aug-01 13:43 sparseml/pytorch/sparsification/info.py
+-rw-rw-r--  2.0 unx    32014 b- defN 23-Aug-01 13:43 sparseml/pytorch/sparsification/modifier.py
+-rw-rw-r--  2.0 unx    18952 b- defN 23-Aug-01 13:43 sparseml/pytorch/sparsification/modifier_thinning.py
+-rw-rw-r--  2.0 unx      705 b- defN 23-Aug-01 13:43 sparseml/pytorch/sparsification/distillation/__init__.py
+-rw-rw-r--  2.0 unx     4741 b- defN 23-Aug-01 13:43 sparseml/pytorch/sparsification/distillation/modifier_distillation.py
+-rw-rw-r--  2.0 unx    14742 b- defN 23-Aug-01 13:43 sparseml/pytorch/sparsification/distillation/modifier_distillation_base.py
+-rw-rw-r--  2.0 unx    19177 b- defN 23-Aug-01 13:43 sparseml/pytorch/sparsification/distillation/modifier_per_layer.py
+-rw-rw-r--  2.0 unx     1158 b- defN 23-Aug-01 13:43 sparseml/pytorch/sparsification/pruning/__init__.py
+-rw-rw-r--  2.0 unx    29250 b- defN 23-Aug-01 13:43 sparseml/pytorch/sparsification/pruning/mask_creator.py
+-rw-rw-r--  2.0 unx    22391 b- defN 23-Aug-01 13:43 sparseml/pytorch/sparsification/pruning/mask_params.py
+-rw-rw-r--  2.0 unx    13389 b- defN 23-Aug-01 13:43 sparseml/pytorch/sparsification/pruning/modifier_as.py
+-rw-rw-r--  2.0 unx    10455 b- defN 23-Aug-01 13:43 sparseml/pytorch/sparsification/pruning/modifier_pruning_acdc.py
+-rw-rw-r--  2.0 unx    33219 b- defN 23-Aug-01 13:43 sparseml/pytorch/sparsification/pruning/modifier_pruning_base.py
+-rw-rw-r--  2.0 unx     5757 b- defN 23-Aug-01 13:43 sparseml/pytorch/sparsification/pruning/modifier_pruning_constant.py
+-rw-rw-r--  2.0 unx     8860 b- defN 23-Aug-01 13:43 sparseml/pytorch/sparsification/pruning/modifier_pruning_layer.py
+-rw-rw-r--  2.0 unx    15595 b- defN 23-Aug-01 13:43 sparseml/pytorch/sparsification/pruning/modifier_pruning_magnitude.py
+-rw-rw-r--  2.0 unx    63519 b- defN 23-Aug-01 13:43 sparseml/pytorch/sparsification/pruning/modifier_pruning_mfac.py
+-rw-rw-r--  2.0 unx     8774 b- defN 23-Aug-01 13:43 sparseml/pytorch/sparsification/pruning/modifier_pruning_movement.py
+-rw-rw-r--  2.0 unx    24121 b- defN 23-Aug-01 13:43 sparseml/pytorch/sparsification/pruning/modifier_pruning_obs.py
+-rw-rw-r--  2.0 unx    18245 b- defN 23-Aug-01 13:43 sparseml/pytorch/sparsification/pruning/modifier_pruning_structured.py
+-rw-rw-r--  2.0 unx     4644 b- defN 23-Aug-01 13:43 sparseml/pytorch/sparsification/pruning/scorer.py
+-rw-rw-r--  2.0 unx      813 b- defN 23-Aug-01 13:43 sparseml/pytorch/sparsification/quantization/__init__.py
+-rw-rw-r--  2.0 unx     2220 b- defN 23-Aug-01 13:43 sparseml/pytorch/sparsification/quantization/constants.py
+-rw-rw-r--  2.0 unx    32723 b- defN 23-Aug-01 13:43 sparseml/pytorch/sparsification/quantization/helpers.py
+-rw-rw-r--  2.0 unx    33626 b- defN 23-Aug-01 13:43 sparseml/pytorch/sparsification/quantization/legacy_modifier_quantization.py
+-rw-rw-r--  2.0 unx    26778 b- defN 23-Aug-01 13:43 sparseml/pytorch/sparsification/quantization/modifier_quantization.py
+-rw-rw-r--  2.0 unx    13482 b- defN 23-Aug-01 13:43 sparseml/pytorch/sparsification/quantization/quantization_scheme.py
+-rw-rw-r--  2.0 unx    17905 b- defN 23-Aug-01 13:43 sparseml/pytorch/sparsification/quantization/quantize.py
+-rw-rw-r--  2.0 unx    76796 b- defN 23-Aug-01 13:43 sparseml/pytorch/sparsification/quantization/quantize_qat_export.py
+-rw-rw-r--  2.0 unx      790 b- defN 23-Aug-01 13:43 sparseml/pytorch/sparsification/training/__init__.py
+-rw-rw-r--  2.0 unx     1778 b- defN 23-Aug-01 13:43 sparseml/pytorch/sparsification/training/modifier_epoch.py
+-rw-rw-r--  2.0 unx     2883 b- defN 23-Aug-01 13:43 sparseml/pytorch/sparsification/training/modifier_logging.py
+-rw-rw-r--  2.0 unx    24287 b- defN 23-Aug-01 13:43 sparseml/pytorch/sparsification/training/modifier_lr.py
+-rw-rw-r--  2.0 unx    21497 b- defN 23-Aug-01 13:43 sparseml/pytorch/sparsification/training/modifier_params.py
+-rw-rw-r--  2.0 unx     6690 b- defN 23-Aug-01 13:43 sparseml/pytorch/sparsification/training/modifier_regularizer.py
+-rw-rw-r--  2.0 unx      943 b- defN 23-Aug-01 13:43 sparseml/pytorch/torchvision/__init__.py
+-rw-rw-r--  2.0 unx     6490 b- defN 23-Aug-01 13:43 sparseml/pytorch/torchvision/export_onnx.py
+-rw-rw-r--  2.0 unx     2870 b- defN 23-Aug-01 13:43 sparseml/pytorch/torchvision/presets.py
+-rw-rw-r--  2.0 unx     2530 b- defN 23-Aug-01 13:43 sparseml/pytorch/torchvision/sampler.py
+-rw-rw-r--  2.0 unx    41409 b- defN 23-Aug-01 13:43 sparseml/pytorch/torchvision/train.py
+-rw-rw-r--  2.0 unx     7128 b- defN 23-Aug-01 13:43 sparseml/pytorch/torchvision/transforms.py
+-rw-rw-r--  2.0 unx    16675 b- defN 23-Aug-01 13:43 sparseml/pytorch/torchvision/utils.py
+-rw-rw-r--  2.0 unx     1160 b- defN 23-Aug-01 13:43 sparseml/pytorch/utils/__init__.py
+-rw-rw-r--  2.0 unx     9706 b- defN 23-Aug-01 13:43 sparseml/pytorch/utils/benchmarker.py
+-rw-rw-r--  2.0 unx     2846 b- defN 23-Aug-01 13:43 sparseml/pytorch/utils/callbacks.py
+-rw-rw-r--  2.0 unx     1061 b- defN 23-Aug-01 13:43 sparseml/pytorch/utils/distributed.py
+-rw-rw-r--  2.0 unx    30694 b- defN 23-Aug-01 13:43 sparseml/pytorch/utils/exporter.py
+-rw-rw-r--  2.0 unx    41226 b- defN 23-Aug-01 13:43 sparseml/pytorch/utils/helpers.py
+-rw-rw-r--  2.0 unx     1663 b- defN 23-Aug-01 13:43 sparseml/pytorch/utils/log_sparsification_info.py
+-rw-rw-r--  2.0 unx    31374 b- defN 23-Aug-01 13:43 sparseml/pytorch/utils/logger.py
+-rw-rw-r--  2.0 unx    27048 b- defN 23-Aug-01 13:43 sparseml/pytorch/utils/loss.py
+-rw-rw-r--  2.0 unx    11754 b- defN 23-Aug-01 13:43 sparseml/pytorch/utils/model.py
+-rw-rw-r--  2.0 unx    39117 b- defN 23-Aug-01 13:43 sparseml/pytorch/utils/module.py
+-rw-rw-r--  2.0 unx     8809 b- defN 23-Aug-01 13:43 sparseml/pytorch/utils/sparsification.py
+-rw-rw-r--  2.0 unx    30059 b- defN 23-Aug-01 13:43 sparseml/pytorch/utils/ssd_helpers.py
+-rw-rw-r--  2.0 unx    12337 b- defN 23-Aug-01 13:43 sparseml/pytorch/utils/yolo_helpers.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-Aug-01 13:43 sparseml/pytorch/utils/sparsification_info/__init__.py
+-rw-rw-r--  2.0 unx    10457 b- defN 23-Aug-01 13:43 sparseml/pytorch/utils/sparsification_info/configs.py
+-rw-rw-r--  2.0 unx     4309 b- defN 23-Aug-01 13:43 sparseml/pytorch/utils/sparsification_info/helpers.py
+-rw-rw-r--  2.0 unx     2946 b- defN 23-Aug-01 13:43 sparseml/pytorch/utils/sparsification_info/module_sparsification_info.py
+-rw-rw-r--  2.0 unx      655 b- defN 23-Aug-01 13:43 sparseml/recipe_template/__init__.py
+-rw-rw-r--  2.0 unx     4788 b- defN 23-Aug-01 13:43 sparseml/recipe_template/utils.py
+-rw-rw-r--  2.0 unx     1058 b- defN 23-Aug-01 13:43 sparseml/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     9387 b- defN 23-Aug-01 13:43 sparseml/sparsification/analyzer.py
+-rw-rw-r--  2.0 unx     9065 b- defN 23-Aug-01 13:43 sparseml/sparsification/info.py
+-rw-rw-r--  2.0 unx    15565 b- defN 23-Aug-01 13:43 sparseml/sparsification/model_info.py
+-rw-rw-r--  2.0 unx     2002 b- defN 23-Aug-01 13:43 sparseml/sparsification/modifier_epoch.py
+-rw-rw-r--  2.0 unx    10117 b- defN 23-Aug-01 13:43 sparseml/sparsification/modifier_lr.py
+-rw-rw-r--  2.0 unx     5505 b- defN 23-Aug-01 13:43 sparseml/sparsification/modifier_params.py
+-rw-rw-r--  2.0 unx    12845 b- defN 23-Aug-01 13:43 sparseml/sparsification/modifier_pruning.py
+-rw-rw-r--  2.0 unx     3700 b- defN 23-Aug-01 13:43 sparseml/sparsification/oracle.py
+-rw-rw-r--  2.0 unx    18570 b- defN 23-Aug-01 13:43 sparseml/sparsification/recipe_builder.py
+-rw-rw-r--  2.0 unx    14413 b- defN 23-Aug-01 13:43 sparseml/sparsification/recipe_editor.py
+-rw-rw-r--  2.0 unx     1250 b- defN 23-Aug-01 13:43 sparseml/sparsification/types.py
+-rw-rw-r--  2.0 unx     1169 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/__init__.py
+-rw-rw-r--  2.0 unx     7272 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/base.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/datasets/__init__.py
+-rw-rw-r--  2.0 unx     8121 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/datasets/dataset.py
+-rw-rw-r--  2.0 unx     5600 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/datasets/helpers.py
+-rw-rw-r--  2.0 unx     2768 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/datasets/registry.py
+-rw-rw-r--  2.0 unx      807 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx    12686 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/datasets/classification/cifar.py
+-rw-rw-r--  2.0 unx     8690 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     2032 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     4695 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx      805 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/framework/__init__.py
+-rw-rw-r--  2.0 unx     5859 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/framework/info.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/models/__init__.py
+-rw-rw-r--  2.0 unx    19752 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/models/estimator.py
+-rw-rw-r--  2.0 unx    14774 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/models/registry.py
+-rw-rw-r--  2.0 unx      822 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/models/classification/__init__.py
+-rw-rw-r--  2.0 unx     3540 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/models/classification/mnist.py
+-rw-rw-r--  2.0 unx    11161 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/models/classification/mobilenet.py
+-rw-rw-r--  2.0 unx    18359 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/models/classification/mobilenet_v2.py
+-rw-rw-r--  2.0 unx    28103 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/models/classification/resnet.py
+-rw-rw-r--  2.0 unx    26886 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/models/classification/vgg.py
+-rw-rw-r--  2.0 unx      865 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/nn/__init__.py
+-rw-rw-r--  2.0 unx    18670 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/nn/layers.py
+-rw-rw-r--  2.0 unx     1238 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/optim/__init__.py
+-rw-rw-r--  2.0 unx     8607 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/optim/analyzer_module.py
+-rw-rw-r--  2.0 unx     9591 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/optim/manager.py
+-rw-rw-r--  2.0 unx    19683 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/optim/mask_creator_pruning.py
+-rw-rw-r--  2.0 unx    33919 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    15955 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/optim/modifier.py
+-rw-rw-r--  2.0 unx     1715 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/optim/modifier_epoch.py
+-rw-rw-r--  2.0 unx    10685 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/optim/modifier_lr.py
+-rw-rw-r--  2.0 unx     7092 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/optim/modifier_params.py
+-rw-rw-r--  2.0 unx    15702 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/optim/modifier_pruning.py
+-rw-rw-r--  2.0 unx     5682 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/optim/schedule_lr.py
+-rw-rw-r--  2.0 unx     9232 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx      801 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1385 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/sparsification/info.py
+-rw-rw-r--  2.0 unx      967 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/utils/__init__.py
+-rw-rw-r--  2.0 unx    10913 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/utils/exporter.py
+-rw-rw-r--  2.0 unx      996 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/utils/helpers.py
+-rw-rw-r--  2.0 unx     1974 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/utils/loss.py
+-rw-rw-r--  2.0 unx     8119 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/utils/nets_utils.py
+-rw-rw-r--  2.0 unx     1327 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/utils/summary.py
+-rw-rw-r--  2.0 unx    12536 b- defN 23-Aug-01 13:43 sparseml/tensorflow_v1/utils/variable.py
+-rw-rw-r--  2.0 unx     1511 b- defN 23-Aug-01 13:43 sparseml/transformers/__init__.py
+-rw-rw-r--  2.0 unx    22048 b- defN 23-Aug-01 13:43 sparseml/transformers/export.py
+-rw-rw-r--  2.0 unx    30756 b- defN 23-Aug-01 13:43 sparseml/transformers/masked_language_modeling.py
+-rw-rw-r--  2.0 unx    36976 b- defN 23-Aug-01 13:43 sparseml/transformers/question_answering.py
+-rw-rw-r--  2.0 unx    40299 b- defN 23-Aug-01 13:43 sparseml/transformers/text_classification.py
+-rw-rw-r--  2.0 unx    34350 b- defN 23-Aug-01 13:43 sparseml/transformers/token_classification.py
+-rw-rw-r--  2.0 unx      833 b- defN 23-Aug-01 13:43 sparseml/transformers/sparsification/__init__.py
+-rw-rw-r--  2.0 unx    19529 b- defN 23-Aug-01 13:43 sparseml/transformers/sparsification/question_answering.py
+-rw-rw-r--  2.0 unx    44413 b- defN 23-Aug-01 13:43 sparseml/transformers/sparsification/trainer.py
+-rw-rw-r--  2.0 unx     1890 b- defN 23-Aug-01 13:43 sparseml/transformers/sparsification/training_args.py
+-rw-rw-r--  2.0 unx      794 b- defN 23-Aug-01 13:43 sparseml/transformers/utils/__init__.py
+-rw-rw-r--  2.0 unx     3090 b- defN 23-Aug-01 13:43 sparseml/transformers/utils/helpers.py
+-rw-rw-r--  2.0 unx     2536 b- defN 23-Aug-01 13:43 sparseml/transformers/utils/metrics.py
+-rw-rw-r--  2.0 unx    17074 b- defN 23-Aug-01 13:43 sparseml/transformers/utils/model.py
+-rw-rw-r--  2.0 unx      844 b- defN 23-Aug-01 13:43 sparseml/utils/__init__.py
+-rw-rw-r--  2.0 unx      886 b- defN 23-Aug-01 13:43 sparseml/utils/frameworks.py
+-rw-rw-r--  2.0 unx    26562 b- defN 23-Aug-01 13:43 sparseml/utils/helpers.py
+-rw-rw-r--  2.0 unx     3983 b- defN 23-Aug-01 13:43 sparseml/utils/restricted_eval.py
+-rw-rw-r--  2.0 unx     1083 b- defN 23-Aug-01 13:43 sparseml/utils/singleton.py
+-rw-rw-r--  2.0 unx     6312 b- defN 23-Aug-01 13:43 sparseml/utils/worker.py
+-rw-rw-r--  2.0 unx     2952 b- defN 23-Aug-01 13:43 sparseml/utils/wrapper.py
+-rw-rw-r--  2.0 unx      819 b- defN 23-Aug-01 13:43 sparseml/utils/datasets/__init__.py
+-rw-rw-r--  2.0 unx      833 b- defN 23-Aug-01 13:43 sparseml/utils/datasets/cifar.py
+-rw-rw-r--  2.0 unx     3750 b- defN 23-Aug-01 13:43 sparseml/utils/datasets/coco.py
+-rw-rw-r--  2.0 unx     1217 b- defN 23-Aug-01 13:43 sparseml/utils/datasets/helpers.py
+-rw-rw-r--  2.0 unx    23366 b- defN 23-Aug-01 13:43 sparseml/utils/datasets/imagenet.py
+-rw-rw-r--  2.0 unx     8967 b- defN 23-Aug-01 13:43 sparseml/utils/datasets/imagenette.py
+-rw-rw-r--  2.0 unx     1009 b- defN 23-Aug-01 13:43 sparseml/utils/datasets/voc.py
+-rw-rw-r--  2.0 unx     1875 b- defN 23-Aug-01 13:43 sparseml/yolact/COCO.sh
+-rw-rw-r--  2.0 unx     1418 b- defN 23-Aug-01 13:43 sparseml/yolact/COCO_test.sh
+-rw-rw-r--  2.0 unx     4020 b- defN 23-Aug-01 13:43 sparseml/yolact/__init__.py
+-rw-rw-r--  2.0 unx     1784 b- defN 23-Aug-01 13:43 sparseml/yolact/scripts.py
+-rw-rw-r--  2.0 unx     1440 b- defN 23-Aug-01 13:43 sparseml/yolov5/__init__.py
+-rw-rw-r--  2.0 unx     4505 b- defN 23-Aug-01 13:43 sparseml/yolov5/helpers.py
+-rw-rw-r--  2.0 unx     1609 b- defN 23-Aug-01 13:43 sparseml/yolov5/scripts.py
+-rw-rw-r--  2.0 unx     1220 b- defN 23-Aug-01 13:43 sparseml/yolov5/yolov5.status.yaml
+-rw-rw-r--  2.0 unx     1117 b- defN 23-Aug-01 13:43 sparseml/yolov8/__init__.py
+-rw-rw-r--  2.0 unx     6061 b- defN 23-Aug-01 13:43 sparseml/yolov8/default.yaml
+-rw-rw-r--  2.0 unx     2502 b- defN 23-Aug-01 13:43 sparseml/yolov8/export.py
+-rw-rw-r--  2.0 unx     2259 b- defN 23-Aug-01 13:43 sparseml/yolov8/modules.py
+-rw-rw-r--  2.0 unx     7394 b- defN 23-Aug-01 13:43 sparseml/yolov8/train.py
+-rw-rw-r--  2.0 unx    37330 b- defN 23-Aug-01 13:43 sparseml/yolov8/trainers.py
+-rw-rw-r--  2.0 unx     2748 b- defN 23-Aug-01 13:43 sparseml/yolov8/val.py
+-rw-rw-r--  2.0 unx     8459 b- defN 23-Aug-01 13:43 sparseml/yolov8/validators.py
+-rw-rw-r--  2.0 unx      685 b- defN 23-Aug-01 13:43 sparseml/yolov8/utils/__init__.py
+-rw-rw-r--  2.0 unx     6683 b- defN 23-Aug-01 13:43 sparseml/yolov8/utils/export_samples.py
+-rw-rw-r--  2.0 unx     4041 b- defN 23-Aug-01 13:43 sparseml/yolov8/utils/helpers.py
+-rw-rw-r--  2.0 unx    11357 b- defN 23-Aug-01 13:46 sparseml_nightly-1.6.0.20230801.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    21838 b- defN 23-Aug-01 13:46 sparseml_nightly-1.6.0.20230801.dist-info/METADATA
+-rw-rw-r--  2.0 unx     2158 b- defN 23-Aug-01 13:46 sparseml_nightly-1.6.0.20230801.dist-info/NOTICE
+-rw-rw-r--  2.0 unx       92 b- defN 23-Aug-01 13:46 sparseml_nightly-1.6.0.20230801.dist-info/WHEEL
+-rw-rw-r--  2.0 unx     2326 b- defN 23-Aug-01 13:46 sparseml_nightly-1.6.0.20230801.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 23-Aug-01 13:46 sparseml_nightly-1.6.0.20230801.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    37473 b- defN 23-Aug-01 13:46 sparseml_nightly-1.6.0.20230801.dist-info/RECORD
+376 files, 3523922 bytes uncompressed, 912449 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -135,21 +135,21 @@
 
 Filename: sparseml/exporters/transforms/kv_cache/cache_keys_and_values.py
 Comment: 
 
 Filename: sparseml/exporters/transforms/kv_cache/configs.py
 Comment: 
 
-Filename: sparseml/exporters/transforms/kv_cache/positions_adjustment_base.py
+Filename: sparseml/exporters/transforms/kv_cache/transforms_base.py
 Comment: 
 
-Filename: sparseml/exporters/transforms/kv_cache/positions_adjustment_codegen.py
+Filename: sparseml/exporters/transforms/kv_cache/transforms_codegen.py
 Comment: 
 
-Filename: sparseml/exporters/transforms/kv_cache/positions_adjustment_opt.py
+Filename: sparseml/exporters/transforms/kv_cache/transforms_opt.py
 Comment: 
 
 Filename: sparseml/exporters/transforms/utils/__init__.py
 Comment: 
 
 Filename: sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py
 Comment: 
@@ -1101,29 +1101,29 @@
 
 Filename: sparseml/yolov8/utils/export_samples.py
 Comment: 
 
 Filename: sparseml/yolov8/utils/helpers.py
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230723.dist-info/LICENSE
+Filename: sparseml_nightly-1.6.0.20230801.dist-info/LICENSE
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230723.dist-info/METADATA
+Filename: sparseml_nightly-1.6.0.20230801.dist-info/METADATA
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230723.dist-info/NOTICE
+Filename: sparseml_nightly-1.6.0.20230801.dist-info/NOTICE
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230723.dist-info/WHEEL
+Filename: sparseml_nightly-1.6.0.20230801.dist-info/WHEEL
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230723.dist-info/entry_points.txt
+Filename: sparseml_nightly-1.6.0.20230801.dist-info/entry_points.txt
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230723.dist-info/top_level.txt
+Filename: sparseml_nightly-1.6.0.20230801.dist-info/top_level.txt
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230723.dist-info/RECORD
+Filename: sparseml_nightly-1.6.0.20230801.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sparseml/exporters/kv_cache_injector.py

```diff
@@ -56,31 +56,29 @@
         The exporter will look for a `config.json` file in the `model_path`
         directory to determine the parameters for KV cache injection.
         If `model_path` is not provided, the requested parameters can be
         provided in the `kwargs`.
 
         This transformation not only solely injects the kv cache
         inputs/outputs, but also adjusts the original ONNX graph to
-        account for the necessary changes. This involves e.g. adding
-        the 'position' input to the model, so that the positional
-        embeddings of the new model are compatible with the past kv
-        cache information.
+        account for the necessary changes. This is done by the
+        optional `additional_transforms` variable.
 
         Usage:
         ```python
         onnx_model: onnx.ModelProto = ...
         exporter = KeyValueCacheInjector(model_path="path/to/model")
         exporter.export(onnx_model, "model.onnx")
         ```
 
         Alternatively:
         ```python
         onnx_model: onnx.ModelProto = ...
-        exporter = KeyValueCacheInjector(model_path="path/to/model")
-        exporter = KeyValueCacheInjector(num_attention_heads = 16,
+        exporter = KeyValueCacheInjector(model_path="path/to/model",
+                                         num_attention_heads = 16,
                                          hidden_size_dim = 64)
         exporter.export(onnx_model, "model.onnx")
         ```
 
         You can also just optimize the model directly without saving to disk:
         ```python
         onnx_model: onnx.ModelProto = ...
@@ -102,16 +100,18 @@
             transforms = self._get_transforms_from_config(config)
 
         elif kwargs:
             transforms = self._get_transforms_from_kwargs(kwargs)
 
         else:
             raise ValueError(
-                "Either `model_path` or kwargs must be provided to "
-                "KeyValueCacheInjector"
+                f"Unable to find KeyValueCacheConfig for model_path='{model_path}'. "
+                "Either kwargs must be provided to KeyValueCacheInjector to construct "
+                "OnnxTransform, or a new config should be registered in "
+                "`sparseml/src/sparseml/exporters/transforms/kv_cache/configs.py`"
             )
 
         super().__init__(transforms)
 
     def pre_validate(self, model: Union[onnx.ModelProto, str, Path]) -> onnx.ModelProto:
         if isinstance(model, (str, Path)):
             model = onnx.load(str(model))
@@ -127,27 +127,29 @@
 
     def export(self, pre_transforms_model: onnx.ModelProto, file_path: str):
         post_transforms_model: onnx.ModelProto = self.apply(pre_transforms_model)
         save_onnx(post_transforms_model, file_path)
 
     @staticmethod
     def _get_transforms_from_config(config: KeyValueCacheConfig) -> List[OnnxTransform]:
-        positions_adjustment = config.positions_adjustment_transform
+        additional_transforms = config.additional_transforms
 
         transforms = [
             CacheKeysAndValues(
                 num_attention_heads=config.num_attention_heads,
                 hidden_size_kv_cache=config.hidden_size_kv_cache,
                 multiply_batch_by_num_att_heads=config.multiply_batch_by_num_att_heads,
                 transpose_value_input=config.transpose_value_input,
                 transpose_key_input=config.transpose_key_input,
             )
         ]
-        if positions_adjustment is not None:
-            transforms += [positions_adjustment()]
+        if additional_transforms is not None:
+            if not isinstance(additional_transforms, list):
+                additional_transforms = [additional_transforms]
+            transforms += [transform() for transform in additional_transforms]
 
         return transforms
 
     @staticmethod
     def _get_transforms_from_kwargs(kwargs: Dict[str, Any]) -> List[OnnxTransform]:
         transforms = [
             CacheKeysAndValues(
```

## sparseml/exporters/onnx_to_deepsparse.py

```diff
@@ -14,14 +14,15 @@
 
 import os
 from copy import deepcopy
 from pathlib import Path
 from typing import Union
 
 import onnx
+from onnx import ModelProto
 
 from sparseml.exporters import transforms as sparseml_transforms
 from sparseml.exporters.base_exporter import BaseExporter
 from sparsezoo import save_onnx
 
 
 class ONNXToDeepsparse(BaseExporter):
@@ -105,13 +106,15 @@
 
     def post_validate(self, model: onnx.ModelProto) -> onnx.ModelProto:
         # sanity check
         if not isinstance(model, onnx.ModelProto):
             raise TypeError(f"Expected onnx.ModelProto, found {type(model)}")
         return model
 
-    def export(self, pre_transforms_model: onnx.ModelProto, file_path: str):
+    def export(self, pre_transforms_model: Union[ModelProto, str], file_path: str):
+        if not isinstance(pre_transforms_model, ModelProto):
+            pre_transforms_model = onnx.load(pre_transforms_model)
         if self.export_input_model or os.getenv("SAVE_PREQAT_ONNX", False):
             save_onnx(pre_transforms_model, file_path.replace(".onnx", ".preqat.onnx"))
 
         post_transforms_model: onnx.ModelProto = self.apply(pre_transforms_model)
         save_onnx(post_transforms_model, file_path)
```

## sparseml/exporters/transforms/conv_to_qlinearconv.py

```diff
@@ -120,15 +120,18 @@
             if bias is not None:
                 # quantize bias and add it to the qconv inputs
                 bias = numpy_helper.to_array(bias)
                 input_quantize_params = get_quantization_params(
                     model, input_quant, include_target=False
                 )
                 bias_scale = input_quantize_params.scale * weight_quantize_params.scale
-                quantized_bias = quantize_array(bias, bias_scale, 0, numpy.int32)
+                bias_zero_point = numpy.zeros(bias_scale.shape, dtype=numpy.int32)
+                quantized_bias = quantize_array(
+                    bias, bias_scale, bias_zero_point, numpy.int32
+                )
                 quantized_bias_name = f"{conv_node.name}.bias_quantized"
                 quantized_bias_initializer = numpy_helper.from_array(
                     quantized_bias, name=quantized_bias_name
                 )
                 model.graph.initializer.append(quantized_bias_initializer)
                 qconv_inputs.append(quantized_bias_name)
             else:
```

## sparseml/exporters/transforms/kv_cache/__init__.py

```diff
@@ -15,11 +15,11 @@
 Transforms for adding KV caching mechanism into language models
 """
 
 # flake8: noqa
 # isort:skip_file
 
 from .cache_keys_and_values import *
-from .positions_adjustment_base import *
-from .positions_adjustment_opt import *
-from .positions_adjustment_codegen import *
+from .transforms_base import *
+from .transforms_opt import *
+from .transforms_codegen import *
 from .configs import *
```

## sparseml/exporters/transforms/kv_cache/configs.py

```diff
@@ -11,42 +11,42 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
 import logging
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import Any, Dict, List, Optional, Tuple, Type, Union
 
 from pydantic import BaseModel, Field
 
-from sparseml.exporters.transforms.kv_cache.positions_adjustment_codegen import (
-    PositionsAdjustmentCodeGen,
+from sparseml.exporters.transforms import OnnxTransform
+from sparseml.exporters.transforms.kv_cache.transforms_codegen import (
+    AdditionalTransformsCodeGen,
 )
-from sparseml.exporters.transforms.kv_cache.positions_adjustment_opt import (
-    PositionsAdjustmentOPT,
+from sparseml.exporters.transforms.kv_cache.transforms_opt import (
+    AdditionalTransformsOPT,
 )
 
 
 _LOGGER = logging.getLogger(__name__)
 
 __all__ = ["get_kv_cache_config", "KeyValueCacheConfig"]
 
 
 class KeyValueCacheConfig(BaseModel):
     model_name: str = Field(
         description="The name of the model type. This should correspond to "
         "the `model_type` field in the transformer's `config.json` file."
     )
-    positions_adjustment_transform: Any = Field(
-        description="The class to use to transform the positional embeddings. "
-        "This should be a subclass of `PositionsAdjustmentBase`. Note: In the "
-        "future, when we encounter models that are more complex than just "
-        "editing the positions in the model, we can make this transformation more "
-        "general."
+    additional_transforms: Union[
+        List[Type[OnnxTransform]], Type[OnnxTransform], None
+    ] = Field(
+        description="A transform class (or list thereof) to use for additional "
+        "transforms to the model required for finalizing the kv cache injection."
     )
     key_num_attention_heads: str = Field(
         description="The key to use to get the number of attention heads from the "
         "transformer's `config.json` file."
     )
     key_num_embedding_hidden_size: str = Field(
         description="The key to use to get the hidden size "
@@ -80,35 +80,35 @@
 
     class Config:
         arbitrary_types_allowed = True
 
 
 OPT_CONFIG = KeyValueCacheConfig(
     model_name="opt",
-    positions_adjustment_transform=PositionsAdjustmentOPT,
+    additional_transforms=AdditionalTransformsOPT,
     key_num_attention_heads="num_attention_heads",
     key_num_embedding_hidden_size="hidden_size",
     transpose_value_input=None,
     transpose_key_input=None,
     multiply_batch_by_num_att_heads=True,
 )
 
 CODEGEN_CONFIG = KeyValueCacheConfig(
     model_name="codegen",
-    positions_adjustment_transform=PositionsAdjustmentCodeGen,
+    additional_transforms=AdditionalTransformsCodeGen,
     key_num_attention_heads="n_head",
     key_num_embedding_hidden_size="n_embd",
     transpose_value_input=(0, 2, 1, 3),
     transpose_key_input=None,
     multiply_batch_by_num_att_heads=False,
 )
 
 BLOOM_CONFIG = KeyValueCacheConfig(
     model_name="bloom",
-    positional_embedding_transform=None,
+    additional_transforms=None,
     key_num_attention_heads="num_attention_heads",
     key_num_embedding_hidden_size="n_embed",
     transpose_value_input=None,
     transpose_key_input=(0, 1, 3, 2),
     multiply_batch_by_num_att_heads=True,
 )
```

## sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py

```diff
@@ -93,18 +93,25 @@
         qadd_node = _create_qadd_node(
             node,
             integer_op_output="{}_quant".format(node.output[0]),
             quantized_bias_name=quantized_bias_initializer.name,
             output_quantize_node=output_quantize_node,
         )
         model.graph.node.append(qadd_node)
-
-        # bias has same scale as future rescale op
-        rescale_scale = quantized_bias_scale
         mul_input_node_name = qadd_node.name
+
+        # bias has same scale as future rescale op, unless doing channel-wise Conv
+        if weight_quantize_params.scale.size > 1 and node.op_type == "Conv":
+            # channel-wise Conv
+            rescale_scale = _create_rescale_init(
+                node, input_quantize_params, weight_quantize_params, reshape=True
+            )
+            model.graph.initializer.append(rescale_scale)
+        else:
+            rescale_scale = quantized_bias_scale
     else:
         rescale_scale = _create_rescale_init(
             node, input_quantize_params, weight_quantize_params
         )
         model.graph.initializer.append(rescale_scale)
         # cast node should come directly after quantize op output instead of add
         output_quantize_node = output_quantize_node or integer_op_node
@@ -257,15 +264,15 @@
 
 
 def _quantize_bias(
     node, bias_initializer, input_quantize_params, weight_quantize_params, bias_add_name
 ) -> Tuple[TensorProto, TensorProto, TensorProto]:
     bias_initializer = numpy_helper.to_array(bias_initializer)
     bias_scale = input_quantize_params.scale * weight_quantize_params.scale
-    bias_zero_point = 0
+    bias_zero_point = numpy.zeros(bias_scale.shape, dtype=numpy.int32)
     quantized_bias = quantize_array(
         bias_initializer, bias_scale, bias_zero_point, dtype=numpy.int32
     )
     if node.op_type == "Conv" and len(quantized_bias.shape) == 1:
         # reshape for bias add broadcasting
         quantized_bias = quantized_bias.reshape(1, quantized_bias.shape[0], 1, 1)
 
@@ -286,17 +293,19 @@
             numpy.asarray(bias_zero_point, dtype=numpy.uint8),
             name=quantized_bias_zero_point_name,
         ),
     )
 
 
 def _create_rescale_init(
-    node, input_quantize_params, weight_quantize_params
+    node, input_quantize_params, weight_quantize_params, reshape=False
 ) -> TensorProto:
     output_scale = input_quantize_params.scale * weight_quantize_params.scale
+    if reshape:  # for channel-wise Conv
+        output_scale = output_scale.reshape(1, output_scale.shape[0], 1, 1)
     return numpy_helper.from_array(
         numpy.asarray(output_scale), name=f"{node.name}_quant.rescale.scale"
     )
 
 
 def _quantize_weight_initializer(
     node: NodeProto,
```

## sparseml/exporters/transforms/utils/helpers.py

```diff
@@ -122,35 +122,44 @@
     if isinstance(op, str):
         return node.op_type == op
     else:
         return node.op_type in op
 
 
 def quantize_array(
-    array: numpy.ndarray, scale: float, zero_point: int, dtype: Any = numpy.uint8
+    array: numpy.ndarray,
+    scale: numpy.ndarray,
+    zero_point: numpy.ndarray,
+    dtype: Any = numpy.uint8,
 ) -> numpy.ndarray:
     try:
         import torch  # noqa: F401
 
         if dtype == numpy.uint8:
             tensor_dtype = torch.quint8
         elif dtype == numpy.int8:
             tensor_dtype = torch.qint8
         elif dtype == numpy.int32:
             tensor_dtype = torch.qint32
 
         tensor = torch.Tensor(array.copy()).to(torch.float32)
-        if isinstance(scale, numpy.ndarray):
-            scale = scale.item()
-        if isinstance(zero_point, numpy.ndarray):
-            zero_point = zero_point.item()
-
-        quant_tensor = torch.quantize_per_tensor(
-            tensor, scale, zero_point, tensor_dtype
-        )
+        if scale.size > 1 and zero_point.size > 1:  # per-channel quantization
+            scale = torch.Tensor(scale.copy()).to(torch.float32)
+            zero_point = torch.Tensor(zero_point.copy()).to(torch.int32)
+            quant_tensor = torch.quantize_per_channel(
+                tensor,
+                scale,
+                zero_point,
+                0,  # channel axis
+                tensor_dtype,
+            )
+        else:  # per-tensor quantization
+            quant_tensor = torch.quantize_per_tensor(
+                tensor, scale.item(), zero_point.item(), tensor_dtype
+            )
         return quant_tensor.int_repr().numpy()
     except ModuleNotFoundError as err:
         _LOGGER.debug(f"Error: {err}. Defaulting to numpy implementation.")
         dmin = numpy.iinfo(dtype).min
         dmax = numpy.iinfo(dtype).max
         return ((array / scale).round() + zero_point).clip(dmin, dmax).astype(dtype)
```

## sparseml/onnx/utils/graph_editor.py

```diff
@@ -324,14 +324,56 @@
             seen_ids.update(node.output)
 
         # update model node list with topo sorted list
         assert len(updated_node_list) == len(self._model.graph.node)
         self._model.graph.ClearField("node")
         self._model.graph.node.extend(updated_node_list)
 
+    def get_orphaned_nodes(
+        self,
+        graph_output_ids: Optional[Iterable[str]] = None,
+    ) -> List[NodeProto]:
+        """
+        :param graph_output_ids: iterable of output ids in graph. if not supplied,
+            will be read from the model
+        :return: list of all nodes in the graph that are not inputs to
+            other nodes or outputs of the graph
+        """
+        if graph_output_ids is None:
+            graph_output_ids = {output.name for output in self._model.graph.output}
+
+        orphaned_nodes = []
+        for node in self.nodes:
+            node_is_orphaned = True
+            # iterate over possible output ids, in practice, there is almost
+            # always only 1
+            for out_id in node.output:
+                if out_id in self._input_id_to_nodes or out_id in graph_output_ids:
+                    node_is_orphaned = False
+            if node_is_orphaned:
+                orphaned_nodes.append(node)
+        return orphaned_nodes
+
+    def delete_orphaned_node_branches(self):
+        """
+        Deletes all nodes in the graph that are not inputs to other nodes or outputs of
+        the graph. Additionally deletes all nodes that would become orphaned
+        after the node deletion until the graph contains no orphaned nodes
+        """
+        graph_output_ids = {output.name for output in self._model.graph.output}
+        orphaned_nodes = self.get_orphaned_nodes(graph_output_ids=graph_output_ids)
+
+        while orphaned_nodes:
+            # no need to refresh self, delete nodes should update internal graph edges
+            self.delete_nodes(orphaned_nodes)
+            self.update()
+            self.delete_unused_initializers()
+            # update now orphaned nodes, can only run up to len(nodes) times
+            orphaned_nodes = self.get_orphaned_nodes(graph_output_ids=graph_output_ids)
+
     def _store_node_edges(self, node: NodeProto):
         for output_id in node.output:
             self._output_id_to_node[output_id] = node
         for input_id in node.input:
             self._input_id_to_nodes[input_id].append(node)
 
     def _delete_node_edges(self, node: NodeProto):
```

## sparseml/pytorch/sparsification/quantization/helpers.py

```diff
@@ -135,25 +135,31 @@
         weights.
     :param activation_dtype: quantized activation data type.
         Default is torch.quint8.
     :param weight_dtype: quantized weights data type.
         Default is torch.qint8.
     :param activation_bits: number of bits for activations. Default is 8.
     :param weight_bits: number of bits for weights. Default is 8.
+    :param activation_strategy: "tensor" to quantize over the whole activation tensor,
+        or "channel" to quantize per channel. Default is "tensor"
+    :param weight_strategy: "tensor" to quantize over the whole weight tensor, or
+        "channel" to quantize per channel. Default is "tensor"
     :param tensorrt: if True sets quantization configuration for compatibility with
        explict quantization as supported by TensorRT 8.2.
     """
 
     _symmetric_activations: bool = False
     _symmetric_weights: bool = True
     reduce_range: bool = False
     activation_dtype: torch.dtype = torch.quint8
     weight_dtype: torch.dtype = torch.qint8
     activation_bits: int = 8
     weight_bits: int = 8
+    activation_strategy: str = "tensor"
+    weight_strategy: str = "tensor"
     activation_qconfig_kwargs: Dict[str, Any] = field(default_factory=dict)
     weight_qconfig_kwargs: Dict[str, Any] = field(default_factory=dict)
     tensorrt: bool = False
 
     @property
     def symmetric_activations(self) -> bool:
         # always use symmetric activations in tensorrt mode
@@ -548,22 +554,24 @@
 
 def get_qat_qconfig(qproperties: QConfigProperties) -> "torch.quantization.QConfig":
     """
     :param qproperties: properties used to define QConfig.
     """
     activation_observer = get_observer(
         qproperties.symmetric_activations,
+        qproperties.activation_strategy,
         qproperties.activation_dtype,
         qproperties.activation_bits,
         qproperties.reduce_range,
         qproperties.activation_qconfig_kwargs,
     )
 
     weight_observer = get_observer(
         qproperties.symmetric_weights,
+        qproperties.weight_strategy,
         qproperties.weight_dtype,
         qproperties.weight_bits,
         False,
         qproperties.weight_qconfig_kwargs,
     )
 
     return torch_quantization.QConfig(
```

## sparseml/pytorch/sparsification/quantization/quantization_scheme.py

```diff
@@ -17,15 +17,15 @@
 """
 from copy import deepcopy
 from functools import partial
 from typing import Any, Dict, Optional, Union
 
 import torch
 from packaging import version
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, Field, validator
 from torch.nn import Identity
 
 
 try:
     from torch import quantization as torch_quantization
 except Exception:
     torch_quantization = None
@@ -74,14 +74,20 @@
     num_bits: int = Field(
         default=8, description="number of bits to target for quantization"
     )
     symmetric: bool = Field(
         default=False,
         description="set True to use symmetric quantization. Default False",
     )
+    strategy: str = Field(
+        default="tensor",
+        description=(
+            "scope of the quantization to be applied. can be 'tensor' or 'channel'"
+        ),
+    )
     kwargs: Dict[str, Any] = Field(
         default_factory=dict,
         description=(
             "optional dict of kwargs to be passed directly to torch quantization "
             "Observers constructor excluding quantization range or symmetry"
         ),
     )
@@ -102,20 +108,28 @@
 
     def get_observer(self) -> "torch.quantization.FakeQuantize":
         """
         :return: torch quantization FakeQuantize built based on these QuantizationArgs
         """
         return get_observer(
             symmetric=self.symmetric,
+            strategy=self.strategy,
             dtype=torch.qint8,
             bits=self.num_bits,
             reduce_range=self.kwargs.get("reduce_range", False),
             qconfig_kwargs=self.kwargs,
         )
 
+    @validator("strategy")
+    def validate_strategy(cls, value):
+        valid_scopes = ["tensor", "channel"]
+        if value not in valid_scopes:
+            raise ValueError(f"`strategy` must be one of {valid_scopes}, got {value}")
+        return value
+
 
 class QuantizationScheme(BaseModel):
     """
     Class composed of QuantizationArgs to build QConfig and QuantWrapper objects for
     quantizing models. Provides a simple user interface for defining how inputs,
     weights, and outputs should be quantized
     """
@@ -272,29 +286,39 @@
         quant_max = (2**bits) - 1
 
     return quant_min, quant_max, is_custom
 
 
 def get_observer(
     symmetric: bool,
+    strategy: str,
     dtype: torch.dtype,
     bits: int,
     reduce_range: bool,
     qconfig_kwargs: Dict[str, Any],
 ):
-    qscheme = torch.per_tensor_symmetric if symmetric else torch.per_tensor_affine
     quant_min, quant_max, is_custom_qrange = compute_range(dtype, bits)
 
-    observer_cls = torch_quantization.MovingAverageMinMaxObserver
-    observer_kwargs = dict(
-        dtype=dtype,
-        qscheme=qscheme,
-        reduce_range=reduce_range,
-    )
-
+    if strategy == "channel":
+        qscheme = torch.per_channel_symmetric if symmetric else torch.per_channel_affine
+        observer_cls = torch_quantization.MovingAveragePerChannelMinMaxObserver
+        observer_kwargs = dict(
+            ch_axis=0,
+            dtype=dtype,
+            qscheme=qscheme,
+            reduce_range=reduce_range,
+        )
+    else:  # default to tensor strategy
+        qscheme = torch.per_tensor_symmetric if symmetric else torch.per_tensor_affine
+        observer_cls = torch_quantization.MovingAverageMinMaxObserver
+        observer_kwargs = dict(
+            dtype=dtype,
+            qscheme=qscheme,
+            reduce_range=reduce_range,
+        )
     """
     in torch 1.9.1, quant_min and quant_max are not passed to observer:
     https://github.com/pytorch/pytorch/blob/v1.9.1/torch/quantization/fake_quantize.py#L109
     however in 1.12.0, this is fixed so both are passed to observer:
     https://github.com/pytorch/pytorch/blob/v1.12.1/torch/ao/quantization/fake_quantize.py#L132
 
     Passing quant_min/quant_max to observer means the observer will have
```

## sparseml/pytorch/utils/exporter.py

```diff
@@ -30,14 +30,15 @@
 from onnx import numpy_helper
 from packaging import version
 from torch import Tensor
 from torch.nn import Module
 from torch.optim.optimizer import Optimizer
 from torch.utils.data import DataLoader
 
+from sparseml.exporters.onnx_to_deepsparse import ONNXToDeepsparse
 from sparseml.onnx.utils import ONNXGraph
 from sparseml.pytorch.opset import TORCH_DEFAULT_ONNX_OPSET
 from sparseml.pytorch.utils.helpers import (
     adjust_quantization_for_onnx_export,
     tensors_export,
     tensors_module_forward,
     tensors_to_device,
@@ -196,15 +197,15 @@
             fusing during torch export. Default and suggested setting is True. Batch
             norm fusing will change the exported parameter names as well as affect
             sensitivity analyses of the exported graph.  Additionally, the DeepSparse
             inference engine, and other engines, perform batch norm fusing at model
             compilation.
         :param convert_qat: if True and quantization aware training is detected in
             the module being exported, the resulting QAT ONNX model will be converted
-            to a fully quantized ONNX model using `quantize_torch_qat_export`. Default
+            to a fully quantized ONNX model using `ONNXToDeepsparse`. Default
             is False.
         :param export_kwargs: kwargs to be passed as is to the torch.onnx.export api
             call. Useful to pass in dyanmic_axes, input_names, output_names, etc.
             See more on the torch.onnx.export api spec in the PyTorch docs:
             https://pytorch.org/docs/stable/onnx.html
         """
         if not export_kwargs:
@@ -440,15 +441,15 @@
         fusing during torch export. Default and suggested setting is True. Batch
         norm fusing will change the exported parameter names as well as affect
         sensitivity analyses of the exported graph.  Additionally, the DeepSparse
         inference engine, and other engines, perform batch norm fusing at model
         compilation.
     :param convert_qat: if True and quantization aware training is detected in
         the module being exported, the resulting QAT ONNX model will be converted
-        to a fully quantized ONNX model using `quantize_torch_qat_export`. Default
+        to a fully quantized ONNX model using `ONNXToDeepsparse`. Default
         is False.
     :param dynamic_axes: dictionary of input or output names to list of dimensions
         of those tensors that should be exported as dynamic. May input 'batch'
         to set the first dimension of all inputs and outputs to dynamic. Default
         is an empty dict
     :param skip_input_quantize: if True, the export flow will attempt to delete
         the first Quantize Linear Nodes(s) immediately after model input and set
@@ -575,42 +576,24 @@
         _unwrap_batchnorms(onnx_model)
 
         # clean up graph from any injected / wrapped operations
         _delete_trivial_onnx_adds(onnx_model)
     save_onnx(onnx_model, file_path)
 
     if convert_qat and is_quant_module:
-        # overwrite exported model with fully quantized version
-        # import here to avoid cyclic dependency
-        from sparseml.pytorch.sparsification.quantization import (
-            quantize_torch_qat_export,
-        )
 
-        use_qlinearconv = hasattr(module, "export_with_qlinearconv") and (
+        use_qlinear_conv = hasattr(module, "export_with_qlinearconv") and (
             module.export_with_qlinearconv
         )
 
-        quantize_torch_qat_export(
-            model=file_path,
-            output_file_path=file_path,
-            use_qlinearconv=use_qlinearconv,
+        exporter = ONNXToDeepsparse(
+            use_qlinear_conv=use_qlinear_conv,
+            skip_input_quantize=skip_input_quantize,
         )
-
-    if skip_input_quantize:
-        try:
-            # import here to avoid cyclic dependency
-            from sparseml.pytorch.sparsification.quantization import (
-                skip_onnx_input_quantize,
-            )
-
-            skip_onnx_input_quantize(file_path, file_path)
-        except Exception as e:
-            _LOGGER.warning(
-                f"Unable to skip input QuantizeLinear op with exception {e}"
-            )
+        exporter.export(pre_transforms_model=file_path, file_path=file_path)
 
 
 def _copy_file(src: str, target: str):
     if not os.path.exists(src):
         raise ValueError(
             f"Attempting to copy file from {src}, but the file does not exist."
         )
```

## sparseml/yolov8/__init__.py

```diff
@@ -20,12 +20,12 @@
     import ultralytics as _ultralytics  # noqa: F401
 except ImportError:
     raise ImportError("Please install sparseml[yolov8] to use this pathway")
 
 
 _analytics.send_event("python__yolov8__init")
 
-if "8.0.30" not in ultralytics.__version__:
+if "8.0.124" not in ultralytics.__version__:
     raise ValueError(
-        f"ultralytics==8.0.30 is required, found {ultralytics.__version__}. "
+        f"ultralytics==8.0.124 is required, found {ultralytics.__version__}. "
         "To fix run `pip install sparseml[ultralytics]`."
     )
```

## sparseml/yolov8/default.yaml

```diff
@@ -29,14 +29,17 @@
 deterministic: True # whether to enable deterministic mode
 single_cls: False # train multi-class data as single-class
 image_weights: False # use weighted image selection for training
 rect: False # support rectangular training
 cos_lr: False # use cosine learning rate scheduler
 close_mosaic: 10 # disable mosaic augmentation for final 10 epochs
 resume: False # resume training from last checkpoint
+amp: True # (bool) Automatic Mixed Precision (AMP) training, choices=[True, False], True runs AMP check
+fraction: 1.0  # (float) dataset fraction to train on (default is 1.0, all images in train set)
+profile: False # (bool) profile ONNX and TensorRT speeds during training for loggers
 min_memory: False  # minimize memory footprint loss function, choices=[False, True, <roll_out_thr>]
 
 # Segmentation
 overlap_mask: True # masks should overlap during training
 mask_ratio: 4 # mask downsample ratio
 # Classification
 dropout: 0.0  # use dropout regularization
@@ -46,27 +49,27 @@
 split: val  # dataset split to use for validation, i.e. 'val', 'test' or 'train'
 save_json: False # save results to JSON file
 save_hybrid: False # save hybrid version of labels (labels + additional predictions)
 conf: null # object confidence threshold for detection (default 0.25 predict, 0.001 val)
 iou: 0.7 # intersection over union (IoU) threshold for NMS
 max_det: 300 # maximum number of detections per image
 half: False # use half precision (FP16)
-dnn: False # use OpenCV DNN for ONNX inference
+dnn: False # use OpenCV DNN for ONNX inferences
 plots: True # show plots during training
 
 # Prediction settings --------------------------------------------------------------------------------------------------
 source: null # source directory for images or videos
 show: False # show results if possible
 save_txt: False # save results as .txt file
 save_conf: False # save results with confidence scores
 save_crop: False # save cropped images with results
-hide_labels: False # hide labels
-hide_conf: False # hide confidence scores
+show_labels: True # hide labels
+show_conf: True # hide confidence scores
 vid_stride: 1 # video frame-rate stride
-line_thickness: 3 # bounding box thickness (pixels)
+line_width: 3 # bounding box thickness (pixels)
 visualize: False # visualize results
 augment: False # apply data augmentation to images
 agnostic_nms: False # class-agnostiic NMS
 classes:  # filter results by class, i.e. class=0, or class=[0,2,3]
 retina_masks: False # use retina masks for object detection
 boxes: True # Show boxes in segmentation predictions
```

## sparseml/yolov8/train.py

```diff
@@ -46,21 +46,21 @@
     type=click.Choice(["detect", "segment", "classify"]),
     help="Specify task to run.",
 )
 @click.option(
     "--model",
     default="yolov8n.yaml",
     type=str,
-    help="i.e. yolov8n.pt, yolov8n.yaml. Path to model file",
+    help="i.e. yolov8n.pt, yolov8n.yaml, yolov8n-seg.yaml. Path to model file",
 )
 @click.option(
     "--data",
     default="coco128.yaml",
     type=str,
-    help="i.e. coco128.yaml. Path to data file",
+    help="i.e. coco128.yaml, coco128-seg.yaml. Path to data file",
 )
 @click.option("--epochs", default=100, type=int, help="number of epochs to train for")
 @click.option(
     "--patience",
     default=50,
     type=int,
     help="epochs to wait for no observable improvement for early stopping of training",
@@ -217,13 +217,15 @@
     help="Path to override default dataset path.",
 )
 def main(**kwargs):
     if kwargs["dataset_path"] is not None:
         kwargs["data"] = data_from_dataset_path(kwargs["data"], kwargs["dataset_path"])
     del kwargs["dataset_path"]
 
-    model = SparseYOLO(kwargs["model"])
+    # NOTE: the task, model, and data kwargs will override the values in default.yaml
+    # They should be provided or default values will be used.
+    model = SparseYOLO(kwargs["model"], kwargs["task"])
     model.train(**kwargs)
 
 
 if __name__ == "__main__":
     main()
```

## sparseml/yolov8/trainers.py

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
+import re
 import shutil
 import subprocess
 import sys
 import tempfile
 import warnings
 from copy import copy, deepcopy
 from datetime import datetime, timedelta
@@ -47,25 +48,29 @@
 from sparsezoo import Model
 from sparsezoo.utils import validate_onnx
 from ultralytics import __version__
 from ultralytics.nn.modules import Detect, Segment
 from ultralytics.nn.tasks import SegmentationModel, attempt_load_one_weight
 from ultralytics.yolo.cfg import get_cfg
 from ultralytics.yolo.data.dataloaders.v5loader import create_dataloader
-from ultralytics.yolo.engine.model import YOLO
+from ultralytics.yolo.engine.model import TASK_MAP, YOLO
 from ultralytics.yolo.engine.trainer import BaseTrainer
 from ultralytics.yolo.utils import LOGGER, IterableSimpleNamespace, yaml_load
 from ultralytics.yolo.utils.checks import check_file, check_imgsz, check_yaml
 from ultralytics.yolo.utils.dist import (
     USER_CONFIG_DIR,
     ddp_cleanup,
     find_free_network_port,
 )
 from ultralytics.yolo.utils.files import get_latest_run
-from ultralytics.yolo.utils.torch_utils import de_parallel, smart_inference_mode
+from ultralytics.yolo.utils.torch_utils import (
+    TORCH_1_9,
+    de_parallel,
+    smart_inference_mode,
+)
 from ultralytics.yolo.v8.classify import ClassificationTrainer, ClassificationValidator
 from ultralytics.yolo.v8.detect import DetectionTrainer, DetectionValidator
 from ultralytics.yolo.v8.segment import SegmentationTrainer, SegmentationValidator
 
 
 class _NullLRScheduler:
     def step(self):
@@ -151,23 +156,31 @@
                 ) from e
         self.resume = resume
 
     def train(self):
         # NOTE: overriden to use our version of `generate_ddp_command`
         world_size = torch.cuda.device_count()
         if world_size > 1 and "LOCAL_RANK" not in os.environ:
-            command = generate_ddp_command(world_size, self)
+            if self.args.rect:
+                LOGGER.warning(
+                    "WARNING ⚠️ 'rect=True' is incompatible with Multi-GPU training, "
+                    "setting rect=False"
+                )
+                self.args.rect = False
+
+            command, file = generate_ddp_command(world_size, self)
             try:
-                subprocess.run(command)
+                LOGGER.info(f"DDP command: {command}")
+                subprocess.run(command, check=True)
             except Exception as e:
-                self.console(e)
+                raise e
             finally:
-                ddp_cleanup(command, self)
+                ddp_cleanup(command, str(file))
         else:
-            self._do_train(int(os.getenv("RANK", -1)), world_size)
+            self._do_train(world_size)
 
     def setup_model(self):
         # NOTE: override to handle pickled checkpoints and our own checkpoints
         if isinstance(self.model, torch.nn.Module):
             LOGGER.info("Received torch.nn.Module, not loading from checkpoint")
             self._build_managers(ckpt=None)
             return
@@ -229,27 +242,27 @@
         if ckpt["epoch"] == -1:
             LOGGER.info(
                 "Applying structure from completed recipe in checkpoint "
                 f"at epoch {ckpt['epoch']}"
             )
             self.checkpoint_manager = ScheduledModifierManager.from_yaml(ckpt["recipe"])
             if self.checkpoint_manager.quantization_modifiers:
-                self._modify_arch_for_quantization()
+                _modify_arch_for_quantization(self.model)
             self.checkpoint_manager.apply_structure(self.model, epoch=float("inf"))
 
         else:
             # resuming
             # yolo will populate this when the --resume flag
             assert self.args.recipe is not None
             LOGGER.info(
                 "Applying structure from un-finished recipe in checkpoint "
                 f"at epoch {ckpt['epoch']}"
             )
             if self.manager.quantization_modifiers:
-                self._modify_arch_for_quantization()
+                _modify_arch_for_quantization(self.model)
             self.manager.apply_structure(self.model, epoch=ckpt["epoch"])
 
     def resume_training(self, ckpt):
         # NOTE: this method is called at the end of super()._setup_train()
 
         # set self.ema to None so super().resume_training() doesn't load from checkpoint
         cached_ema = self.ema
@@ -272,16 +285,18 @@
             try:
                 self.ema.ema.load_state_dict(ema_state_dict)
             except RuntimeError:
                 LOGGER.warning("Unable to load EMA weights - disabling EMA.")
                 self.ema.enabled = False
             self.ema.updates = ckpt["updates"]
 
-    def _setup_train(self, rank, world_size):
-        super()._setup_train(rank, world_size)
+    def _setup_train(self, world_size):
+        rank = int(os.getenv("RANK", -1))
+
+        super()._setup_train(world_size)
         # NOTE: self.resume_training() was called in ^
 
         if rank in {0, -1}:
             self.test_loader = self.get_dataloader(
                 self.testset,
                 batch_size=max(1, self.train_loader.batch_size // 4),
                 rank=-1,
@@ -336,26 +351,27 @@
                 self.optimizer,
                 steps_per_epoch=self.steps_per_epoch,
                 epoch=self.start_epoch,
                 wrap_optim=self.scaler,
                 loggers=self.logger_manager,
                 grad_sampler={
                     "data_loader_builder": self._get_data_loader_builder(),
-                    "loss_function": lambda preds, batch: self.criterion(preds, batch)[
-                        0
-                    ]
+                    "loss_function": lambda preds, batch: self.model.loss(
+                        batch=batch, preds=preds
+                    )[0]
                     / self.train_loader.batch_size,
                 },
             )
         else:
             # initialize steps_per_epoch for logging when there's no recipe
             self.steps_per_epoch = len(self.train_loader)
 
-    def _setup_ddp(self, rank, world_size):
+    def _setup_ddp(self, world_size):
         # increases the timeout for DDP processes
+        rank = int(os.getenv("RANK", -1))
         torch.cuda.set_device(rank)
         self.device = torch.device("cuda", rank)
         LOGGER.info(
             f"DDP settings: RANK {rank}, WORLD_SIZE {world_size}, DEVICE {self.device}"
         )
         torch.distributed.init_process_group(
             "nccl" if torch.distributed.is_nccl_available() else "gloo",
@@ -515,40 +531,36 @@
 
 class SparseDetectionTrainer(SparseTrainer, DetectionTrainer):
     def get_validator(self):
         self.loss_names = "box_loss", "cls_loss", "dfl_loss"
         return SparseDetectionValidator(
             self.test_loader,
             save_dir=self.save_dir,
-            logger=self.console,
             args=copy(self.args),
         )
 
 
 class SparseClassificationTrainer(SparseTrainer, ClassificationTrainer):
     def get_validator(self):
         self.loss_names = ["loss"]
-        return SparseClassificationValidator(
-            self.test_loader, self.save_dir, logger=self.console
-        )
+        return SparseClassificationValidator(self.test_loader, self.save_dir)
 
 
 class SparseSegmentationTrainer(SparseTrainer, SegmentationTrainer):
     def get_validator(self):
         self.loss_names = "box_loss", "seg_loss", "cls_loss", "dfl_loss"
         return SparseSegmentationValidator(
             self.test_loader,
             save_dir=self.save_dir,
-            logger=self.console,
             args=copy(self.args),
         )
 
 
 class SparseYOLO(YOLO):
-    def __init__(self, model="yolov8n.yaml", type="v8") -> None:
+    def __init__(self, model="yolov8n.yaml", task="detect") -> None:
         model_str = str(model)
 
         if model_str.startswith("zoo:"):
             model = download_framework_model_by_recipe_type(
                 Model(model_str), model_suffix="pt"
             )
             model_str = str(model)
@@ -561,15 +573,20 @@
                     "source" in ckpt and ckpt["source"] == "sparseml"
                 )
             else:
                 self.is_sparseml_checkpoint = False
         else:
             self.is_sparseml_checkpoint = False
 
-        super().__init__(model, type)
+        super().__init__(model, task)
+
+        self.ModelClass = TASK_MAP[self.task][0]
+        self.TrainerClass = TASK_MAP[self.task][1]
+        self.ValidatorClass = TASK_MAP[self.task][2]
+        self.PredictorClass = TASK_MAP[self.task][3]
 
         if self.TrainerClass == DetectionTrainer:
             self.TrainerClass = SparseDetectionTrainer
         elif self.TrainerClass == ClassificationTrainer:
             self.TrainerClass = SparseClassificationTrainer
         elif self.TrainerClass == SegmentationTrainer:
             self.TrainerClass = SparseSegmentationTrainer
@@ -577,15 +594,15 @@
         if self.ValidatorClass == DetectionValidator:
             self.ValidatorClass = SparseDetectionValidator
         elif self.ValidatorClass == ClassificationValidator:
             self.ValidatorClass = SparseClassificationValidator
         elif self.ValidatorClass == SegmentationValidator:
             self.ValidatorClass = SparseSegmentationValidator
 
-    def _load(self, weights: str):
+    def _load(self, weights: str, task=None):
         if self.is_sparseml_checkpoint:
             """
             NOTE: the model is given to the trainer class with this snippet
             from YOLO base class:
             ```python
             self.trainer = self.TrainerClass(overrides=overrides)
             if not overrides.get("resume"):  # manually set model only if not resuming
@@ -599,20 +616,15 @@
             self.ckpt = torch.load(weights, map_location="cpu")
             config = dict(self.ckpt["train_args"])
             config.pop("save_dir", None)
             self.ckpt_path = weights
             self.task = config["task"]
             self.overrides = deepcopy(config)
             self._reset_ckpt_args(self.overrides)
-            (
-                self.ModelClass,
-                self.TrainerClass,
-                self.ValidatorClass,
-                self.PredictorClass,
-            ) = self._assign_ops_from_task(self.task)
+            self.ModelClass = TASK_MAP[self.task][0]
 
             if "yaml" in self.ckpt:
                 self.model = self.ModelClass(dict(self.ckpt["yaml"]))
             elif "model_yaml" in self.ckpt:
                 self.model = self.ModelClass(dict(self.ckpt["model_yaml"]))
             else:
                 self.model = self.ModelClass(dict(self.ckpt["model"].yaml))
@@ -634,16 +646,20 @@
 
             if self.ckpt["ema"]:
                 self.model.load_state_dict(self.ckpt["ema"])
             else:
                 self.model.load_state_dict(self.ckpt["model"])
             LOGGER.info("Loaded previous weights from checkpoint")
             assert self.model.yaml == self.ckpt["model_yaml"]
+
+            self.overrides["model"] = weights
+            self.overrides["task"] = self.task
+
         else:
-            return super()._load(weights)
+            super()._load(weights, task)
 
     def export(self, **kwargs):
         """
         Export model.
         Args:
             **kwargs : Any other args accepted by the exporter.
         """
@@ -707,21 +723,31 @@
             )
             recipe = (
                 ScheduledModifierManager.compose_staged(recipe, manager)
                 if recipe
                 else manager
             )
 
-        name = args.get("name", f"{type(self.model).__name__}.onnx")
+        if args.get("name") and args["name"]:
+            name = args["name"]
+        else:
+            name = f"{type(self.model).__name__}.onnx"
+
         save_dir = args["save_dir"]
+        if not os.path.exists(save_dir):
+            os.mkdir(save_dir)
 
         for _, m in self.model.named_modules():
             if isinstance(m, (Detect, Segment)):
                 m.export = True
 
+        # format attribute seems to not exist within this ultralytics update
+        # This is a workaround. Should be one of
+        # ('saved_model', 'pb', 'tflite', 'edgetpu', 'tfjs')
+        self.model.model[-1].format = "saved_model"
         exporter = ModuleExporter(self.model, save_dir)
         if save_one_shot_torch:
             if not one_shot:
                 warnings.warn(
                     "No one-shot recipe detected; "
                     "skipping one-shot model torch export..."
                 )
@@ -818,28 +844,31 @@
             raise AttributeError(
                 "dataset not provided! Please define `data` "
                 "in config.yaml or pass as an argument."
             )
         if overrides.get("resume"):
             overrides["resume"] = self.ckpt_path
 
+        overrides["nbs"] = int(overrides["nbs"])
         self.trainer = self.TrainerClass(overrides=overrides)
         if not overrides.get("resume"):  # manually set model only if not resuming
             self.trainer.model = self.trainer.get_model(
                 weights=self.model if self.ckpt else None, cfg=self.model.yaml
             )
             self.model = self.trainer.model
         self.trainer.train()
 
     @smart_inference_mode()
     def val(self, data=None, **kwargs):
         overrides = self.overrides.copy()
         overrides["rect"] = True  # rect batches as default
         overrides.update(kwargs)
         overrides["mode"] = "val"
+        if overrides.get("nbs"):
+            overrides["nbs"] = int(overrides["nbs"])
         overrides["data"] = data or overrides["data"]
         args = get_cfg(cfg=DEFAULT_CFG, overrides=overrides)
         args.data = data or args.data
         args.task = self.task
         if args.imgsz == DEFAULT_CFG.imgsz:
             # use trained imgsz unless custom value is passed
             args.imgsz = self.ckpt["train_args"]["imgsz"]
@@ -853,38 +882,45 @@
             trainer=self.TrainerClass(overrides=overrides),
             training=False,
         )
 
 
 def generate_ddp_command(world_size, trainer):
     # NOTE: copied from ultralytics.yolo.utils.dist.generate_ddp_command
+    """Generates and returns command for distributed training."""
     import __main__  # noqa local import to avoid https://github.com/Lightning-AI/lightning/issues/15218
 
-    file_name = os.path.abspath(sys.argv[0])
-    using_cli = not file_name.endswith(".py")
-    if using_cli:
-        file_name = generate_ddp_file(trainer)
-    return [
+    if not trainer.resume:
+        shutil.rmtree(trainer.save_dir)  # remove the save_dir
+    file = str(Path(sys.argv[0]).resolve())
+    safe_pattern = re.compile(
+        r"^[a-zA-Z0-9_. /\\-]{1,128}$"
+    )  # allowed characters and maximum of 100 characters
+    if not (
+        safe_pattern.match(file) and Path(file).exists() and file.endswith(".py")
+    ):  # using CLI
+        file = generate_ddp_file(trainer)
+    dist_cmd = "torch.distributed.run" if TORCH_1_9 else "torch.distributed.launch"
+    port = find_free_network_port()
+    cmd = [
         sys.executable,
         "-m",
-        "torch.distributed.run",
+        dist_cmd,
         "--nproc_per_node",
         f"{world_size}",
         "--master_port",
-        f"{find_free_network_port()}",
-        file_name,
-    ] + sys.argv[1:]
+        f"{port}",
+        file,
+    ]
+    return cmd, file
 
 
 def generate_ddp_file(trainer):
     # NOTE: adapted from ultralytics.yolo.utils.dist.generate_ddp_file
 
-    if not trainer.resume:
-        shutil.rmtree(trainer.save_dir)  # remove the save_dir
-
     content = f"""if __name__ == "__main__":
     from sparseml.yolov8.trainers import {trainer.__class__.__name__}
     trainer = {trainer.__class__.__name__}(config={dict(trainer.args)})
     trainer.train()
 """
     (USER_CONFIG_DIR / "DDP").mkdir(exist_ok=True)
     with tempfile.NamedTemporaryFile(
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## sparseml/yolov8/validators.py

```diff
@@ -19,15 +19,15 @@
 import torch
 from tqdm import tqdm
 
 from sparseml.pytorch.utils import detach
 from ultralytics.nn.autobackend import AutoBackend
 from ultralytics.yolo.data.utils import check_cls_dataset, check_det_dataset
 from ultralytics.yolo.engine.validator import BaseValidator
-from ultralytics.yolo.utils import TQDM_BAR_FORMAT, callbacks, emojis
+from ultralytics.yolo.utils import LOGGER, TQDM_BAR_FORMAT, callbacks, emojis
 from ultralytics.yolo.utils.checks import check_imgsz
 from ultralytics.yolo.utils.ops import Profile
 from ultralytics.yolo.utils.torch_utils import de_parallel, select_device
 from ultralytics.yolo.v8.classify.val import ClassificationValidator
 from ultralytics.yolo.v8.detect.val import DetectionValidator
 from ultralytics.yolo.v8.segment.val import SegmentationValidator
 
@@ -45,64 +45,66 @@
             else:
                 model = trainer.ema.ema or trainer.model
 
             # self.args.half = self.device.type != "cpu"
             model = model.half() if self.args.half else model.float()
             self.model = model
             self.loss = torch.zeros_like(trainer.loss_items, device=trainer.device)
+
             self.args.plots = (
-                trainer.epoch == trainer.epochs - 1
+                trainer.stopper.possible_stop or trainer.epoch == trainer.epochs - 1
             )  # always plot final epoch
+
             model.eval()
         else:
             callbacks.add_integration_callbacks(self)
             self.run_callbacks("on_val_start")
             assert model is not None, "Either trainer or model is needed for validation"
             self.device = select_device(self.args.device, self.args.batch)
             # self.args.half &= self.device.type != "cpu"
             model = AutoBackend(
                 model,
                 device=self.device,
                 dnn=self.args.dnn,
+                data=self.args.data,
                 fp16=self.args.half,
-                fuse=False,
             )
             self.model = model
             stride, pt, jit, engine = model.stride, model.pt, model.jit, model.engine
             imgsz = check_imgsz(self.args.imgsz, stride=stride)
             if engine:
                 self.args.batch = model.batch_size
             else:
                 self.device = model.device
                 if not pt and not jit:
                     self.args.batch = 1  # export.py models default to batch-size 1
-                    self.logger.info(
+                    LOGGER.info(
                         "Forcing --batch-size 1 square inference (1,3,"
                         f"{imgsz},{imgsz}) for non-PyTorch models"
                     )
 
             if isinstance(self.args.data, str) and self.args.data.endswith(".yaml"):
                 self.data = check_det_dataset(self.args.data)
             elif self.args.task == "classify":
-                self.data = check_cls_dataset(self.args.data)
+                self.data = check_cls_dataset(self.args.data, split=self.args.split)
             else:
                 raise FileNotFoundError(
                     emojis(f"Dataset '{self.args.data}' not found ❌")
                 )
             if isinstance(self.data["path"], str):
                 self.data["path"] = Path(self.data["path"])
 
             if self.device.type == "cpu":
                 self.args.workers = (
                     0  # faster CPU val as time dominated by inference, not dataloading
                 )
             if not pt:
                 self.args.rect = False
             self.dataloader = self.dataloader or self.get_dataloader(
-                self.data.get("val") or self.data.set("test"), self.args.batch
+                self.data.get(self.args.split), self.args.batch
             )
 
             model.eval()
             model.warmup(
                 imgsz=(1 if pt else self.args.batch, 3, imgsz, imgsz)
             )  # warmup
             trainer.model = model.model
@@ -125,26 +127,25 @@
             self.batch_i = batch_i
             # pre-process
             with dt[0]:
                 batch = self.preprocess(batch)
 
             # inference
             with dt[1]:
-                preds = model(batch["img"])
+                preds = model(batch["img"], augment=self.args.augment)
 
             # loss
             with dt[2]:
-                if not hasattr(self, "loss"):
-                    self.loss = trainer.criterion(
-                        preds if self.training else preds[1], batch
-                    )[1]
+                if self.training:
+                    self.loss += model.loss(batch=batch, preds=preds)[1]
                 else:
-                    self.loss += trainer.criterion(
-                        preds if self.training else preds[1], batch
-                    )[1]
+                    if hasattr(self, "loss"):
+                        self.loss += model.model.loss(batch=batch, preds=preds[1])[1]
+                    else:
+                        self.loss = model.model.loss(batch=batch, preds=preds[1])[1]
 
             # pre-process predictions
             with dt[3]:
                 preds = self.postprocess(preds)
 
             # During QAT the resulting preds are grad required, breaking
             # the update metrics function.
@@ -154,44 +155,47 @@
             if self.args.plots and batch_i < 3:
                 self.plot_val_samples(batch, batch_i)
                 self.plot_predictions(batch, detached_preds, batch_i)
 
             self.run_callbacks("on_val_batch_end")
         stats = self.get_stats()
         self.check_stats(stats)
-        self.print_results()
-        self.speed = tuple(
-            x.t / len(self.dataloader.dataset) * 1e3 for x in dt
-        )  # speeds per image
+        self.speed = dict(
+            zip(
+                self.speed.keys(),
+                (x.t / len(self.dataloader.dataset) * 1e3 for x in dt),
+            )
+        )
+        self.finalize_metrics()
         self.run_callbacks("on_val_end")
         model.float()
-        stats = {
+        results = {
             **stats,
             **trainer.label_loss_items(
                 self.loss.cpu() / len(self.dataloader), prefix="val"
             ),
         }
         if self.training:
             return {
-                k: round(float(v), 5) for k, v in stats.items()
+                k: round(float(v), 5) for k, v in results.items()
             }  # return results as 5 decimal place floats
         else:
-            self.logger.info(
-                (
-                    "Speed: %.1fms pre-process, %.1fms inference, %.1fms loss, %.1fms "
-                    "post-process per image"
-                ),
-                *self.speed,
+            LOGGER.info(
+                "Speed: %.1fms preprocess, %.1fms inference, %.1fms loss, %.1fms "
+                "postprocess per image" % tuple(self.speed.values())
             )
-            self.logger.info(f"Validation loss: {stats['val/Loss']}")
+            LOGGER.info(f"Validation loss: {results['val/Loss']}")
+            LOGGER.info(f"Metrics: {results}")
             if self.args.save_json and self.jdict:
                 with open(str(self.save_dir / "predictions.json"), "w") as f:
-                    self.logger.info(f"Saving {f.name}...")
+                    LOGGER.info(f"Saving {f.name}...")
                     json.dump(self.jdict, f)  # flatten and save
                 stats = self.eval_json(stats)  # update stats
+            if self.args.plots or self.args.save_json:
+                LOGGER.info(f"Results saved to {self.save_dir}")
             return stats
 
 
 class SparseDetectionValidator(SparseValidator, DetectionValidator):
     ...
```

## sparseml/yolov8/utils/export_samples.py

```diff
@@ -141,37 +141,51 @@
 def _export_torch_outputs(
     image: torch.Tensor, model: torch.nn.Module, sample_out_dir: str, file_idx: str
 ):
 
     # Run model to get torch outputs
     model_out = model(image)
     preds = model_out
+    sample_output_filename = os.path.join(sample_out_dir, f"out-{file_idx}.npz")
+    seg_prediction = None
 
     # Move to cpu for exporting
-    preds = preds.detach().to("cpu")
+    # Segmentation currently supports two outputs
+    if isinstance(preds, tuple):
+        preds_out = preds[0].detach().to("cpu")
+        seg_prediction = preds[1].detach().to("cpu")
+    else:
+        preds_out = preds.detach().to("cpu")
 
-    sample_output_filename = os.path.join(sample_out_dir, f"out-{file_idx}.npz")
-    numpy.savez(sample_output_filename, preds)
+    numpy.savez(sample_output_filename, preds_out, seg_prediction=seg_prediction)
 
 
 def _export_ort_outputs(
     image: numpy.ndarray,
     session: "onnxruntime.InferenceSession",  # noqa: F821
     sample_out_dir: str,
     file_idx: str,
 ):
 
     # Run model to get onnxruntime outputs
     ort_inputs = {session.get_inputs()[0].name: image}
     ort_outs = session.run(None, ort_inputs)
-    preds = numpy.squeeze(ort_outs, axis=0)
-    preds = numpy.squeeze(preds, axis=0)
+    preds = ort_outs
+    seg_prediction = None
+
+    if len(preds) > 1:
+        preds_out = preds[0]
+        seg_prediction = preds[1]
+    else:
+        preds_out = preds[0]
+
+    preds_out = numpy.squeeze(preds_out, axis=0)
 
     sample_output_filename = os.path.join(sample_out_dir, f"out-{file_idx}.npz")
-    numpy.savez(sample_output_filename, preds)
+    numpy.savez(sample_output_filename, preds_out, seg_prediction=seg_prediction)
 
 
 def _export_inputs(image: torch.Tensor, sample_in_dir: str, file_idx: str):
 
     sample_in = image.detach().to("cpu").squeeze(0)
 
     sample_input_filename = os.path.join(sample_in_dir, f"inp-{file_idx}.npz")
```

## Comparing `sparseml_nightly-1.6.0.20230723.dist-info/LICENSE` & `sparseml_nightly-1.6.0.20230801.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sparseml_nightly-1.6.0.20230723.dist-info/METADATA` & `sparseml_nightly-1.6.0.20230801.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparseml-nightly
-Version: 1.6.0.20230723
+Version: 1.6.0.20230801
 Summary: Libraries for applying sparsification recipes to neural networks with a few lines of code, enabling faster and smaller models
 Home-page: https://github.com/neuralmagic/sparseml
 Author: Neuralmagic, Inc.
 Author-email: support@neuralmagic.com
 License: Apache
 Keywords: inference,machine learning,neural network,computer vision,nlp,cv,deep learning,torch,pytorch,tensorflow,keras,sparsity,pruning,deep learning libraries,onnx,quantization,automl
 Platform: UNKNOWN
@@ -111,15 +111,15 @@
 Requires-Dist: nm-transformers-nightly (~=1.6.0) ; extra == 'transformers'
 Requires-Dist: datasets (<=2.11) ; extra == 'transformers'
 Requires-Dist: scikit-learn ; extra == 'transformers'
 Requires-Dist: seqeval ; extra == 'transformers'
 Requires-Dist: einops ; extra == 'transformers'
 Requires-Dist: accelerate (>=0.20.3) ; extra == 'transformers'
 Provides-Extra: ultralytics
-Requires-Dist: ultralytics (==8.0.30) ; extra == 'ultralytics'
+Requires-Dist: ultralytics (==8.0.124) ; extra == 'ultralytics'
 Requires-Dist: torch (<=2.0,>=1.7.0) ; extra == 'ultralytics'
 Provides-Extra: yolov5
 Requires-Dist: torch (<=2.0,>=1.7.0) ; extra == 'yolov5'
 Requires-Dist: gputils ; extra == 'yolov5'
 Requires-Dist: torchvision (<=0.15.1,>=0.3.0) ; extra == 'yolov5'
 Requires-Dist: opencv-python (<=4.6.0.66) ; extra == 'yolov5'
 Requires-Dist: nm-yolov5-nightly (~=1.6.0) ; extra == 'yolov5'
```

## Comparing `sparseml_nightly-1.6.0.20230723.dist-info/NOTICE` & `sparseml_nightly-1.6.0.20230801.dist-info/NOTICE`

 * *Files identical despite different names*

## Comparing `sparseml_nightly-1.6.0.20230723.dist-info/entry_points.txt` & `sparseml_nightly-1.6.0.20230801.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `sparseml_nightly-1.6.0.20230723.dist-info/RECORD` & `sparseml_nightly-1.6.0.20230801.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 sparseml/deepsparse/base.py,sha256=nRjU6TSao0J2iWXcdHwj62X6dVT9vl6TQ2y4Bdn3KN0,3516
 sparseml/deepsparse/framework/__init__.py,sha256=ZHrXXM3AMH78zKcF8Y40IBuy38UFy4fLrvytozw_bNY,801
 sparseml/deepsparse/framework/info.py,sha256=HVDPHFXggFeDqbpM20PkByf1nBccwKnjpTWh0EfrVas,6032
 sparseml/deepsparse/sparsification/__init__.py,sha256=re_2FtHWvO-iQQwRRJZDKz3l_pFZuwe266-4ZFxQqbY,813
 sparseml/deepsparse/sparsification/info.py,sha256=O5FJg5KMJvj-HcJn9W9iiKGZ6Z7_1SavOX-TstXRr6Q,1348
 sparseml/exporters/__init__.py,sha256=fH6rjBYAxuwrTzBTlTjTgCYNyh6TCvCqajCz4Im4YrA,617
 sparseml/exporters/base_exporter.py,sha256=M1HEe9GNf51uYx1z-qxWjIYo5iGZ_Ish8uZ3mj6OZR8,1477
-sparseml/exporters/kv_cache_injector.py,sha256=P14Ma0IRvLUJ7bdKmxWTHwHmTIxJaPYn2z0E8P2aa4U,6325
-sparseml/exporters/onnx_to_deepsparse.py,sha256=XBCXBuJKzxZnQBegZuPU4ZC23VTI8MEXDJI3mWXzfXo,4847
+sparseml/exporters/kv_cache_injector.py,sha256=2fKoRPBE7yrR6h3KXxeU7EbsU5ufyZUIbSnRP2FTjwc,6576
+sparseml/exporters/onnx_to_deepsparse.py,sha256=2FZAI91WryFHGtnNpoHzKO9sPqpKCYRTOGw1irDhzZo,5010
 sparseml/exporters/transforms/__init__.py,sha256=0SMdBqAFpcoDTWDklE2nSk9G4sZOAUyUfeWUJSlRAD0,2350
 sparseml/exporters/transforms/base_transform.py,sha256=IpvdUdEADl2SfqHawcp6-lcNgz-R3L0zpS05WaWF5h8,2333
 sparseml/exporters/transforms/constants_to_initializers.py,sha256=_PX3y16OC-q85d-6DeOOVpKAAMNIU1m5BdYTZlFV_tk,1388
 sparseml/exporters/transforms/conv_to_convinteger_add_cast_mul.py,sha256=x_Y8i9izPyIxX59P3i6rd324yA-o__FWdmwMIuU0_Ng,4630
-sparseml/exporters/transforms/conv_to_qlinearconv.py,sha256=CwCXtIBCOQ1qX5Z2JZhsdXSDk683wRCIBILF_1vd0GI,5838
+sparseml/exporters/transforms/conv_to_qlinearconv.py,sha256=qFxrA8rbk4FmtzUf4TMTXNRe_0GLA_7K78eeIH2PF0g,5973
 sparseml/exporters/transforms/delete_repeated_qdq.py,sha256=YiIOrvKqrxYboOA4A8YTbQIQ4s4MDdmqeLNYHPP4kjs,2440
 sparseml/exporters/transforms/delete_trivial_onnx_adds.py,sha256=St3-PQP8tPXYoyQTFn8fvJi7JF3LoX9Vb9nc-Zbx4Wg,1842
 sparseml/exporters/transforms/flatten_qparams.py,sha256=u0POagPJ_sqaS-DMe2x1Fd40RdlS9nYlLFZqHdsXx4Y,2181
 sparseml/exporters/transforms/fold_conv_div_bn.py,sha256=ckYdMKO2Z31NKRxQk4C4EbMWlVrsuhUDtyeMTMTErE4,3553
 sparseml/exporters/transforms/fold_identity_initializers.py,sha256=Yfv46MvL_vMxNGmUYSvlbucbrWIIDnjWnifmFCzyILA,1669
 sparseml/exporters/transforms/fold_relu_quants.py,sha256=qDGl-6aGmaQ8lAii3v0NvqkjbqtZB1UgHEkd3RzvjXQ,2070
 sparseml/exporters/transforms/gemm_to_matmulinteger_add_cast_mul.py,sha256=r1oVnnu-U0mISkqBJrebXO1o-cmbkSMbo1X4xA0l-t4,4418
@@ -38,23 +38,23 @@
 sparseml/exporters/transforms/propagate_embedding_quantization.py,sha256=MlTJOOM7yDvqy-UTa3y5aFTCjCFmEloDkTA-5Xc_xak,4801
 sparseml/exporters/transforms/quantize_qat_embedding.py,sha256=_v1dEEt5vCSaMF6dJkg9fVGof145-_Lmo0DMjpXsnUE,4464
 sparseml/exporters/transforms/quantize_residuals.py,sha256=f3kNF930ymHI5CmCA0OmYW7vDKvEm9sYhN0UX0UC1EQ,3869
 sparseml/exporters/transforms/remove_duplicate_qconv_weights.py,sha256=mod-7bnlkg20LjerZ7tKKmp_7XyO3FKo13BtIZkDsmM,3331
 sparseml/exporters/transforms/remove_duplicate_quantize_ops.py,sha256=2FSXzaY3jdxOgj3xBaUOUqtk-hzg4kwhheELhoOKpS8,2545
 sparseml/exporters/transforms/skip_input_quantize.py,sha256=ANiYDwSos9gPW4960fMwmGubTDgpAcqFVSIHKf_ffYw,3210
 sparseml/exporters/transforms/unwrap_batchnorms.py,sha256=ly7GHCXN_2r8Gnk8PABWCqcoS-NL3GMfquEK0hRlFCs,1373
-sparseml/exporters/transforms/kv_cache/__init__.py,sha256=6wiIglqacQ56SO_4i5zemLL3VcUfTfJA-AMc5gOHmOE,909
+sparseml/exporters/transforms/kv_cache/__init__.py,sha256=ba_ow-fpv6JUXZ6eCaSS0eRx9_GDlgzY8jksSvqc29E,879
 sparseml/exporters/transforms/kv_cache/cache_keys_and_values.py,sha256=BcJ0s1n3fc28g7IBtPpAB_Az0cJn-3AaIRw9VbxQ3NA,30558
-sparseml/exporters/transforms/kv_cache/configs.py,sha256=kxNTtjPW66S3rG6WkUvZ4NdneT2eTt0gvHX64pWVO1w,6523
-sparseml/exporters/transforms/kv_cache/positions_adjustment_base.py,sha256=bSiZF-U4LRoBxJfnSGXLlaG1pL5MzNPXlzmbDvAXtFw,1660
-sparseml/exporters/transforms/kv_cache/positions_adjustment_codegen.py,sha256=1FSG9npk_R0UK56fap-yRvSjNs5RWRejXJI4fYFD3lk,3377
-sparseml/exporters/transforms/kv_cache/positions_adjustment_opt.py,sha256=d3xqHqbxdRbLIEi5ebXaRwPauvsMjdLPLuRpYyx_DsM,4951
+sparseml/exporters/transforms/kv_cache/configs.py,sha256=qHLliDjLzuNaEnpn_4GvUB3h8S0TaL5RgggxfpclNKE,6427
+sparseml/exporters/transforms/kv_cache/transforms_base.py,sha256=AVqMSwWhCD2F5Hjysqn6CJcNL4khrw8CJmRr9Sa4Ymc,7027
+sparseml/exporters/transforms/kv_cache/transforms_codegen.py,sha256=6uFGzuLUoCXCsplN2QKDcfua3dl8-OtczDh3KGAeEeQ,4974
+sparseml/exporters/transforms/kv_cache/transforms_opt.py,sha256=JHgNKL6e4YSIXuBEEEADMcc_C0xqyd57y7ZT8zRHqsQ,6066
 sparseml/exporters/transforms/utils/__init__.py,sha256=tXSSUnzdyIc_H73xQ5dYhHb1Gj4Nb7GLLDVwJds8c_s,730
-sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py,sha256=I6kugQ0J9yHxCz7Yx3TlxQTUxcaAko4XkBDsQD7v5eo,10570
-sparseml/exporters/transforms/utils/helpers.py,sha256=vkEYL2Bdp_YNXlPg_TGd82Q2ef1EYEr11LVgmORQDiY,6457
+sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py,sha256=u7pD8zO2qtcCQkxN5SDYiujYvnhjfNAVn_3bcHqacWs,11112
+sparseml/exporters/transforms/utils/helpers.py,sha256=0KP47hMugJBKAhgRRj97LjOml8L7rRV8OYOTne9z58Y,6809
 sparseml/exporters/transforms/utils/matching.py,sha256=CnVJLbJARBJwvFjoKh9vwYt6dLP4WXG3p7nCY5VUFaE,14429
 sparseml/framework/__init__.py,sha256=EcIX435yx552d7BkbxmAbQ_X3KAISInHVbD9X-AT1Uk,790
 sparseml/framework/info.py,sha256=TaZAMYdhBHcjl9Xyk3PWjJkDB6g3_f4vD3B6KmhgOl8,9479
 sparseml/keras/__init__.py,sha256=9D-eU-wi0UGuq55i2BTYDgS0mD6UJB10Gi8LQwh9KSk,1144
 sparseml/keras/base.py,sha256=yt1EO6KIeCkdg8rF37U5Y3FNGeAqOQLVGyxRANsyBy0,8054
 sparseml/keras/datasets/__init__.py,sha256=USLH-kFbXiubqgMW8IMkZfycVByQAOdAtzuPHzTok9I,943
 sparseml/keras/datasets/dataset.py,sha256=W6wdx4WXtyy4r1JVbc8fO0Xt5SM03zm8Vq306uNFkaw,3297
@@ -106,15 +106,15 @@
 sparseml/onnx/optim/quantization/quantize_model_post_training.py,sha256=aoz5ixUpQB_6XkowhozqRp8_njthBeqVuwvV2ctM1q0,4552
 sparseml/onnx/sparsification/__init__.py,sha256=hFZDQQXFcXqSqiXlRBRUX7e7GavLphgRd8c21peq8fg,869
 sparseml/onnx/sparsification/analyzer.py,sha256=DCKc8nYo0i3NDu73GVjvBYjuflXUZhkhB14FoFRlTBE,10209
 sparseml/onnx/sparsification/info.py,sha256=UnrwVgOuj-HErwTMc-19h-QOrs1yG_mM45O9VL8oiXU,1363
 sparseml/onnx/sparsification/model_info.py,sha256=Y0tpY9fWN3gr4KlkAdXv2QYJrrrjMvVZOCA-ujPJFPM,8009
 sparseml/onnx/utils/__init__.py,sha256=fGZED95Xmko70ZmTWlZWX3-C4dajmbZcKgaap3HXmVw,867
 sparseml/onnx/utils/data.py,sha256=eh1URN6lmPpVUTg_iHK1R6lLKi4jJh3XGg5OPkgGD_Y,13013
-sparseml/onnx/utils/graph_editor.py,sha256=WLRf0LN__Ou99BIb8Y5Y0ErovGEOuu3J_4PAdFFlxDQ,18825
+sparseml/onnx/utils/graph_editor.py,sha256=ixd2351Q3kfGrwwBQZG_tB_5WcPqO68B-OzkkF6Y80o,20691
 sparseml/onnx/utils/graph_optimizer.py,sha256=AfS2zdxW1tJ6xYAe-2n3KdAdDenxiqslOFUIVAzD-cY,8133
 sparseml/onnx/utils/helpers.py,sha256=I1CJ8loycHBNR35ZaBKxnoFA9TwPHwTEjKlsH1jIgQc,40230
 sparseml/onnx/utils/loss.py,sha256=2njnY0qY2n6DS9HHB0kqLz7N8wgPaDTkAi6Z2DLYPLc,1958
 sparseml/onnx/utils/model.py,sha256=jpuomHDXg4pMngluDRGvGPTO1qhTmyRLTMoHasAC8Co,31591
 sparseml/onnx/utils/sparse_tensor.py,sha256=6Bu9fVJqLCtve3qpg9ScYGqcv4X7ZcRKhVrp8pCLBRI,5437
 sparseml/openpifpaf/__init__.py,sha256=aGr1xneMg-zE7LNhYNjjmEznKB6-xHbpZCT91uv4j3c,931
 sparseml/openpifpaf/export.py,sha256=XkAKuXcCJ64RPZ1YwqzyJKfr9pnn3b0GcROKRXnAWeg,3713
@@ -220,18 +220,18 @@
 sparseml/pytorch/sparsification/pruning/modifier_pruning_mfac.py,sha256=GFJy-obm0cvr2c1vNgCWaUXAhFplvHDxUfmun98rWmY,63519
 sparseml/pytorch/sparsification/pruning/modifier_pruning_movement.py,sha256=gmRbalMpVEJ-U5xdL5Vh-XcTOhkfr8z_cWlKw_m1c9k,8774
 sparseml/pytorch/sparsification/pruning/modifier_pruning_obs.py,sha256=bKZojNIl4aWvU0xXxfAvTZztFcS2Q5QCljt43icIux0,24121
 sparseml/pytorch/sparsification/pruning/modifier_pruning_structured.py,sha256=h7ASPoik7zrBXE_lbdfBO3UkbrTeXG5gGE1Flg75h8s,18245
 sparseml/pytorch/sparsification/pruning/scorer.py,sha256=8gyYSv611GOJwmpQeD7FsWVrLxF8jeM_f59zhQlC6f8,4644
 sparseml/pytorch/sparsification/quantization/__init__.py,sha256=OjbeCzzhoeFJEJQvLmXZc89pghO83sLRhmvNF7_q_oQ,813
 sparseml/pytorch/sparsification/quantization/constants.py,sha256=sla-j0QwLFq92AbDZkHkNLxugpGrNEQJIuLWoWqV3Ks,2220
-sparseml/pytorch/sparsification/quantization/helpers.py,sha256=MmY5iOMlBUBEMrotPyj3H5drzpXhf13v4FJjb1N2aaw,32271
+sparseml/pytorch/sparsification/quantization/helpers.py,sha256=8EjWDeBhgZ-zCO025D0dVbRXPu6EJ9dvBuxNE0j6zS0,32723
 sparseml/pytorch/sparsification/quantization/legacy_modifier_quantization.py,sha256=TToI4dGYZZEzB1q61m1YVg0THlvH7Ew1CZ2y-ajpTts,33626
 sparseml/pytorch/sparsification/quantization/modifier_quantization.py,sha256=LkHNB1IsiFlZugUecB4-LZMjWuoboFYf_PXPx6uPl1g,26778
-sparseml/pytorch/sparsification/quantization/quantization_scheme.py,sha256=10KNttNCHqUTNq706kPB6k7u6mvvfV0WTvx5D5Uqd-Y,12558
+sparseml/pytorch/sparsification/quantization/quantization_scheme.py,sha256=-Ceik2aGOCuxxe0lijUJvCLR25HPEbRUT6ZPzUa0RsQ,13482
 sparseml/pytorch/sparsification/quantization/quantize.py,sha256=bqqH2qBEWYHfea5jzAHmz52uPddfRdmP3TFaCKgQqjM,17905
 sparseml/pytorch/sparsification/quantization/quantize_qat_export.py,sha256=6JLbd3NUy9J0_pygSypJZsPtfxLlY8ZFJfK7kJSRrSY,76796
 sparseml/pytorch/sparsification/training/__init__.py,sha256=4GGhQf6KVSOYwtr_WL9Xcvx4mR-k8yKMVI_zuTBHGO4,790
 sparseml/pytorch/sparsification/training/modifier_epoch.py,sha256=_5p1EZk2qbwTnWsMXbVan3vRj1IRyIM4wYYZdLGA5GE,1778
 sparseml/pytorch/sparsification/training/modifier_logging.py,sha256=K1NMqhea5EBPko6yim8CThShbiSJKN5P_ca_TCyZXto,2883
 sparseml/pytorch/sparsification/training/modifier_lr.py,sha256=m_tCydo_BHiXCHMUKZu6iqKLAP24acAT8-NLjH9RIlE,24287
 sparseml/pytorch/sparsification/training/modifier_params.py,sha256=G_0eVqu0Cup8WNLFhkfPmYnKtJlNrxcJt0FcOOdq9tA,21497
@@ -243,15 +243,15 @@
 sparseml/pytorch/torchvision/train.py,sha256=14gq2sO3_8hKdCm3S5MPA3er7ImeLcbmi1gg3ns6sBs,41409
 sparseml/pytorch/torchvision/transforms.py,sha256=_WfLKV2G9ZLt2zdpKvaHA1ricPGufVIF-lzgKaOL2Ec,7128
 sparseml/pytorch/torchvision/utils.py,sha256=weRmF78Qf9_Kgd-L7aAHERmXKoCVqUP4J8pbSZmav58,16675
 sparseml/pytorch/utils/__init__.py,sha256=WWPrEPVj8YsCZN0JemnAF5z7hOf0nL203uixlqWoAeo,1160
 sparseml/pytorch/utils/benchmarker.py,sha256=Zw1pEj7wDe4ZU_-G0JOCymdLXydN19K1QZKzPJvBp9E,9706
 sparseml/pytorch/utils/callbacks.py,sha256=1z10T8xE0IY5mcL2ARSsHDt6sDWRVF-Nq6zVf9OvD0s,2846
 sparseml/pytorch/utils/distributed.py,sha256=lJtEvgMg6LvH9iUwhveCaWNrx_t7pjn-sOW9rfYViwI,1061
-sparseml/pytorch/utils/exporter.py,sha256=m0Gnj7z4dRuQPCRr_qP6KP0W8hniQgL6gOEwFN2dPxs,31241
+sparseml/pytorch/utils/exporter.py,sha256=AfpsOlo7iIajFzX34Mpl97h6Yv_WwjpApA3klXq77K4,30694
 sparseml/pytorch/utils/helpers.py,sha256=QOFhMhROOBmiJeReZtXfCY9g5jBSK0Tkz5AFqCfYTRM,41226
 sparseml/pytorch/utils/log_sparsification_info.py,sha256=o9WdrrDU8W1J09NHLnW2cja5PXNq442UFzgpXf8po8M,1663
 sparseml/pytorch/utils/logger.py,sha256=KOhmFXNj46gmy5XovwQOZigBuHidVmNqDnVWMUXD7PE,31374
 sparseml/pytorch/utils/loss.py,sha256=RWFyThMBaB-7jAVuS3_CU5bmsWOVFG1jqzPciSpVsj8,27048
 sparseml/pytorch/utils/model.py,sha256=KCEZ6cNkIzLKd6N8KqJe7GX3GD-PoWErZk05nEbQuJc,11754
 sparseml/pytorch/utils/module.py,sha256=gWKNLqn8bI_q97u_QC95WkxBPAclMCwz3HmrZEHEYtU,39117
 sparseml/pytorch/utils/sparsification.py,sha256=BbH3ePC74YWGddSoLcSenLd0D_0nz-Xk5vx4Ui_KkzY,8809
@@ -352,25 +352,25 @@
 sparseml/yolact/COCO_test.sh,sha256=ZoA_h_68zM8EWF510o24_5xBaQtbJLMHenNjSzldYYc,1418
 sparseml/yolact/__init__.py,sha256=5t9V0aePHnzJBik6z1r4W_3DsSn0lKpYjl3pIuZQft0,4020
 sparseml/yolact/scripts.py,sha256=7GE3xp_B8JJpa2H-Vum6rmiOJHcChyffuno4-yteUUw,1784
 sparseml/yolov5/__init__.py,sha256=LiVvIlHR1FF63Ixm2MabdDH1Ul8sFEUEIb3Sbs4awLI,1440
 sparseml/yolov5/helpers.py,sha256=jxzJrgKjsb0PHTeGevKICaL8iBOUzxwZXvPAyGyVE-c,4505
 sparseml/yolov5/scripts.py,sha256=rbVgQ3yNsBCk57BMVh5mKomDHql0S-PkHNGCy_qUfEg,1609
 sparseml/yolov5/yolov5.status.yaml,sha256=4GF6DClV65Qw_1b0J5Ul-B4YFHYQUj34vvqALX8sZFY,1220
-sparseml/yolov8/__init__.py,sha256=l6f1TkolWl2ejQQ63jN3VFft7mMpQDURpWDIeflVKGQ,1115
-sparseml/yolov8/default.yaml,sha256=lWJc8dKEKS0PWG28pAntMe-kHym5PEXX21h9G-9zZhA,5781
+sparseml/yolov8/__init__.py,sha256=eeK3RbfsXhhjbAlqWgXwmxPFbnBxhOmbYBjKLwChpNE,1117
+sparseml/yolov8/default.yaml,sha256=Mi__Ox_lxhsftLyIJfNtDz7t_ncHYxjMXQd0hxHId78,6061
 sparseml/yolov8/export.py,sha256=BN4KFsrYYEfpU8e7icW4rQr4uR4lioNXlY3MII9ecKw,2502
 sparseml/yolov8/modules.py,sha256=j-8TGWMY5-pnEDt-uj1akERLt5zcjK11aN6Bnh1Clrg,2259
-sparseml/yolov8/train.py,sha256=DeZMrZ_moAc3fIojJloq3IvQqiPC_cgPgTjYFSOoG7E,7194
-sparseml/yolov8/trainers.py,sha256=6jr1v056lTlZy8DmPstQosAAIq6-Wj39gdHUoQABzQk,35999
+sparseml/yolov8/train.py,sha256=eetdfCbRQJdBWc7XHb9GYPqMQxZzbKG7FG-4xQeTutk,7394
+sparseml/yolov8/trainers.py,sha256=642diAMZol8Bu_Sgu5I6ehXtSxnRNzx7U_HRqwHk0Lg,37330
 sparseml/yolov8/val.py,sha256=hlFImvknSpV1nONOxA3ivYgvzm64EmK0_Lh-JHLbOsw,2748
-sparseml/yolov8/validators.py,sha256=ytG7g_LOXvKFmxLPmQloT-wNf78convSoRRXVTYCR0Y,8196
+sparseml/yolov8/validators.py,sha256=fkEnjRp1day-KY0n7DZ_VI-zmNqKbalh-g6U-lwHmfQ,8459
 sparseml/yolov8/utils/__init__.py,sha256=6JekgnibQP-8p8Dm1dGiIEGCGdBOAkSOnEds0BMSYhQ,685
-sparseml/yolov8/utils/export_samples.py,sha256=Zy26etoYraN7k6IInS_i0j3RfoIzeeoK6JD-xFjkRk4,6247
+sparseml/yolov8/utils/export_samples.py,sha256=qus5AKOZHxVaSJ2wtawcWZTuZnfHHxEf5KOPNs05AjU,6683
 sparseml/yolov8/utils/helpers.py,sha256=8JZNaTT1zPKiZaOccmMtQu5mXCSMGkq8BDEgUqaPVIs,4041
-sparseml_nightly-1.6.0.20230723.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-sparseml_nightly-1.6.0.20230723.dist-info/METADATA,sha256=L4xP3fNPXhroNhydDPuhlEZ04jXsplVnHnfCFl9wB2E,21837
-sparseml_nightly-1.6.0.20230723.dist-info/NOTICE,sha256=4XaU0pCaSBt7sTZ5qA0WEn0jzOHUEL4FR52UEea4G3w,2158
-sparseml_nightly-1.6.0.20230723.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-sparseml_nightly-1.6.0.20230723.dist-info/entry_points.txt,sha256=UzbZv_wFWQuS0zGUhVxcLWzT_T2Ef9_brFWIy9POI-0,2326
-sparseml_nightly-1.6.0.20230723.dist-info/top_level.txt,sha256=JOOlWKgkyuJBScnty7pC1SQ58fOo1ONbslvMdxB6L2M,9
-sparseml_nightly-1.6.0.20230723.dist-info/RECORD,,
+sparseml_nightly-1.6.0.20230801.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+sparseml_nightly-1.6.0.20230801.dist-info/METADATA,sha256=UMyO879of1AWtaQkVOC4r7F8Q6sGpHxC6FGNNnwY4ME,21838
+sparseml_nightly-1.6.0.20230801.dist-info/NOTICE,sha256=4XaU0pCaSBt7sTZ5qA0WEn0jzOHUEL4FR52UEea4G3w,2158
+sparseml_nightly-1.6.0.20230801.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+sparseml_nightly-1.6.0.20230801.dist-info/entry_points.txt,sha256=UzbZv_wFWQuS0zGUhVxcLWzT_T2Ef9_brFWIy9POI-0,2326
+sparseml_nightly-1.6.0.20230801.dist-info/top_level.txt,sha256=JOOlWKgkyuJBScnty7pC1SQ58fOo1ONbslvMdxB6L2M,9
+sparseml_nightly-1.6.0.20230801.dist-info/RECORD,,
```

