# Comparing `tmp/onnx-tool-0.7.3.tar.gz` & `tmp/onnx-tool-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnx-tool-0.7.3.tar", last modified: Wed Jun 28 15:55:12 2023, max compression
+gzip compressed data, was "onnx-tool-0.7.4.tar", last modified: Tue Aug  1 11:53:40 2023, max compression
```

## Comparing `onnx-tool-0.7.3.tar` & `onnx-tool-0.7.4.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 15:55:11.997973 onnx-tool-0.7.3/
--rw-rw-rw-   0        0        0     1092 2022-12-15 10:33:04.000000 onnx-tool-0.7.3/LICENSE
--rw-rw-rw-   0        0        0    10735 2023-06-28 15:55:11.996448 onnx-tool-0.7.3/PKG-INFO
--rw-rw-rw-   0        0        0    10276 2023-06-18 06:46:34.000000 onnx-tool-0.7.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-28 15:55:11.981558 onnx-tool-0.7.3/onnx_tool/
--rw-rw-rw-   0        0        0     7846 2023-06-19 15:21:47.000000 onnx-tool-0.7.3/onnx_tool/__init__.py
--rw-rw-rw-   0        0        0     3051 2023-06-18 06:46:34.000000 onnx-tool-0.7.3/onnx_tool/__main__.py
--rw-rw-rw-   0        0        0    16079 2023-06-19 15:20:56.000000 onnx-tool-0.7.3/onnx_tool/fusion.py
--rw-rw-rw-   0        0        0    55538 2023-06-28 09:56:20.000000 onnx-tool-0.7.3/onnx_tool/graph.py
--rw-rw-rw-   0        0        0      876 2023-06-19 15:20:56.000000 onnx-tool-0.7.3/onnx_tool/model.py
--rw-rw-rw-   0        0        0    73518 2023-06-28 09:53:51.000000 onnx-tool-0.7.3/onnx_tool/node.py
--rw-rw-rw-   0        0        0     6433 2023-06-18 06:46:34.000000 onnx-tool-0.7.3/onnx_tool/serialization.py
--rw-rw-rw-   0        0        0    15758 2023-06-18 06:46:34.000000 onnx-tool-0.7.3/onnx_tool/tensor.py
--rw-rw-rw-   0        0        0     3685 2023-06-28 15:54:38.000000 onnx-tool-0.7.3/onnx_tool/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-28 15:55:11.994489 onnx-tool-0.7.3/onnx_tool.egg-info/
--rw-rw-rw-   0        0        0    10735 2023-06-28 15:55:11.000000 onnx-tool-0.7.3/onnx_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      404 2023-06-28 15:55:11.000000 onnx-tool-0.7.3/onnx_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 15:55:11.000000 onnx-tool-0.7.3/onnx_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-06-28 15:55:11.000000 onnx-tool-0.7.3/onnx_tool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-28 15:55:11.000000 onnx-tool-0.7.3/onnx_tool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-06-20 15:43:33.000000 onnx-tool-0.7.3/onnx_tool.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-06-28 15:55:11.997973 onnx-tool-0.7.3/setup.cfg
--rw-rw-rw-   0        0        0      988 2023-06-28 15:54:38.000000 onnx-tool-0.7.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:53:40.951804 onnx-tool-0.7.4/
+-rw-rw-rw-   0        0        0     1092 2023-03-28 05:33:56.000000 onnx-tool-0.7.4/LICENSE
+-rw-rw-rw-   0        0        0    11848 2023-08-01 11:53:40.951804 onnx-tool-0.7.4/PKG-INFO
+-rw-rw-rw-   0        0        0    11389 2023-07-31 12:12:52.000000 onnx-tool-0.7.4/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 11:53:40.947799 onnx-tool-0.7.4/onnx_tool/
+-rw-rw-rw-   0        0        0     7844 2023-07-31 11:29:02.000000 onnx-tool-0.7.4/onnx_tool/__init__.py
+-rw-rw-rw-   0        0        0     3051 2023-05-27 08:27:49.000000 onnx-tool-0.7.4/onnx_tool/__main__.py
+-rw-rw-rw-   0        0        0    16079 2023-07-09 04:59:58.000000 onnx-tool-0.7.4/onnx_tool/fusion.py
+-rw-rw-rw-   0        0        0    55875 2023-07-31 11:57:22.000000 onnx-tool-0.7.4/onnx_tool/graph.py
+-rw-rw-rw-   0        0        0      876 2023-07-09 04:59:58.000000 onnx-tool-0.7.4/onnx_tool/model.py
+-rw-rw-rw-   0        0        0    74081 2023-08-01 11:43:45.000000 onnx-tool-0.7.4/onnx_tool/node.py
+-rw-rw-rw-   0        0        0     6266 2023-07-17 16:54:41.000000 onnx-tool-0.7.4/onnx_tool/quantization.py
+-rw-rw-rw-   0        0        0     6433 2023-05-12 10:26:08.000000 onnx-tool-0.7.4/onnx_tool/serialization.py
+-rw-rw-rw-   0        0        0    15757 2023-07-31 11:57:17.000000 onnx-tool-0.7.4/onnx_tool/tensor.py
+-rw-rw-rw-   0        0        0     3685 2023-08-01 11:48:19.000000 onnx-tool-0.7.4/onnx_tool/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-01 11:53:40.950803 onnx-tool-0.7.4/onnx_tool.egg-info/
+-rw-rw-rw-   0        0        0    11848 2023-08-01 11:53:40.000000 onnx-tool-0.7.4/onnx_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      430 2023-08-01 11:53:40.000000 onnx-tool-0.7.4/onnx_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 11:53:40.000000 onnx-tool-0.7.4/onnx_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-08-01 11:53:40.000000 onnx-tool-0.7.4/onnx_tool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-01 11:53:40.000000 onnx-tool-0.7.4/onnx_tool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-08-01 11:53:40.000000 onnx-tool-0.7.4/onnx_tool.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-08-01 11:53:40.951804 onnx-tool-0.7.4/setup.cfg
+-rw-rw-rw-   0        0        0      988 2023-08-01 11:48:14.000000 onnx-tool-0.7.4/setup.py
```

### Comparing `onnx-tool-0.7.3/LICENSE` & `onnx-tool-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `onnx-tool-0.7.3/PKG-INFO` & `onnx-tool-0.7.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,50 @@
-Metadata-Version: 2.1
-Name: onnx-tool
-Version: 0.7.3
-Summary: A tool for ONNX model:Rapid shape inference; Profile model; Compute Graph and Shape Engine; OPs fusion;Quantized models and sparse models are supported.
-Home-page: https://github.com/ThanatosShinji/onnx-tool
-Author: Luo Yu
-Author-email: luoyu888888@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a href="README_CN.md">简体中文</a>
 # onnx-tool
 
 **A tool for ONNX model:**
 
-* *Rapid shape inference.*
-* *Profile model.*
-* *<a href="data/ConstantFolding.md">Constant Folding.</a>*
+* *Parse and edit: <a href="data/ConstantFolding.md">Constant Folding</a>; OPs fusion.*
+* *Model profiling: Rapid shape inference; MACs statistics*
 * *Compute Graph and Shape Engine.*
-* *OPs fusion.*
-* *Activation memory compression.*
+* *Model memory compression: activation compression and weight compression.*
 * *Quantized models and sparse models are supported.*
 
 Supported Models:
 
 * NLP: BERT, T5, GPT, LLaMa, MPT(<a href="benchmark/transfomer_models.py">TransformerModel</a>)
 * Diffusion: Stable Diffusion(TextEncoder, VAE, UNET)
 * CV: <a href="benchmark/compression.py">BEVFormer</a>, MobileNet, YOLO, ...
 * Audio: sovits, LPCNet
 
 ---
 
-## Shape inference
+## Parse and edit
+You can load any onnx file by onnx_tool.Model:  
+Change graph structure with onnx_tool.Graph;  
+Change op attributes and IO tensors with onnx_tool.Node;  
+Change tensor data or type with onnx_tool.Tensor.  
+To apply your changes, just call save_model method of onnx_tool.Model or onnx_tool.Graph.
+
+Please refer [benchmark/samples.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py).
+
+---
 
+## Shape inference
+All profiling data must be built on shape inference result.
 <p align="center">  
   <img src="https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/shape_inference.jpg">
 </p>  
 
 how to use: [data/Profile.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/Profile.md).  
 pytorch usage: [data/PytorchUsage.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/PytorchUsage.md).  
 tensorflow
 usage: [data/TensorflowUsage.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/TensorflowUsage.md).  
 samples: [benchmark/samples.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py).
 
----
 
 ## Profile Model
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/macs_counting.png">
 </p>
 Float MultipleAdd Count(1 MAC=2 FLOPs), Memory Usage(in bytes), Parameters(elements number)<br><br>
@@ -71,15 +67,15 @@
 <p id="compute_graph" align="center">
   <img src="https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/compute_graph.png">
 </p>  
 
 Remove shape calculation layers(created by ONNX export) to get a *Compute Graph*. Use *Shape Engine* to update tensor
 shapes at runtime.  
 Samples: [benchmark/shape_regress.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/shape_regress.py).
-[benchmark/samples.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py#L123).  
+[benchmark/samples.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py#L151).  
 Integrate *Compute Graph* and *Shape Engine* into a cpp inference
 engine: [data/inference_engine.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/inference_engine.md)
 
 ---
 
 ## Inplace op fusion
 
@@ -92,15 +88,15 @@
 </p>
 Resnet18 fusion
 <p align="center">
   <img src="https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/resnet18_fused.png">
 </p>
 
 how to use: [data/Subgraph.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/Subgraph.md).  
-BERT samples: [benchmark/samples.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py#L100).  
+BERT samples: [benchmark/samples.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py#L113).  
 Pattern fusion: [benchmark/do_fusion.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/do_fusion.py).
 
 ---
 
 ## Extract subgraph from ONNX model
 Help implement model parallelism.
 <p align="center">
@@ -109,14 +105,19 @@
 
 how to use: [data/Subgraph.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/Subgraph.md).
 
 ---
 
 ## Memory Compression
 
+### Activation compression
+Activation memory also called temporary memory is created by each OP's output. Only the last activation marked as the
+model's output will be kept. So you don't have to prepare memory space for each activation tensor. They better reuse 
+an optimized memory size.
+
 For large language models and high-resolution CV models, the activation memory compression is a key to save memory.  
 The compression method achieves 5% memory compression on most models.   
 For example:
 
  model                         | Native Memory Size(MB) | Compressed Memory Size(MB) | Compression Ratio(%) 
 -------------------------------|------------------------|----------------------------|----------------------
  StableDiffusion(VAE_encoder)  | 14,245                 | 540                        | 3.7                  
@@ -124,23 +125,26 @@
  StableDiffusion(Text_encoder) | 215                    | 5                          | 2.5                  
  StableDiffusion(UNet)         | 36,135                 | 2,232                      | 6.2                  
  GPT2                          | 40                     | 2                          | 6.9                  
  BERT                          | 2,170                  | 27                         | 1.25                 
 
 code sample: [benchmark/compression.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/compression.py)
 
----
+### Weight compression
+A fp32 model with 7B parameters will take 28GB disk space and memory space. You can not even run the model if your device
+ doesn't have that much memory space. So weight compression is critical to run large language models. As a reference, 7B 
+model with int4 symmetric per block(32) quantization(llama.cpp's q4_0 quantization method) only has ~0.156x model size compared with fp32 model. 
+
+Current support:   
+* [fp16]
+* [int8]x[symmetric/asymmetric]x[per tensor/per channel/per block]  
+* [int4]x[symmetric/asymmetric]x[per tensor/per channel/per block]  
 
-## Tensor operations
+code samples:[benchmark/samples.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py#L36).  
 
-* *Export weight tensors to files*
-* *Simplify tensor and node names, convert name from a long string to a short string*
-* *Remove unused tensors, models like vgg19-7.onnx set its static weight tensors as its input tensors*
-* *Set custom input and output tensors' name and dimension, change model from fixed input to dynamic input*  
-  how to use: [data/Tensors.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/Tensors.md).
 
 ---
 
 ## How to install
     
 `pip install onnx-tool`
 
@@ -154,15 +158,15 @@
 Then `pip install onnx-tool` again.
 
 
 ---
 
 ## Known Issues
 * Loop op is not supported
-* Activation Compression is not optimum
+* Tensor types created by onnx_tool are not correct
   
 ---
 
 ## Results of [ONNX Model Zoo](https://github.com/onnx/models) and SOTA models
 Some models have dynamic input shapes. The MACs varies from input shapes. The input shapes used in these results are writen to [data/public/config.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/public/config.py).
 These onnx models with all tensors' shape can be downloaded: [baidu drive](https://pan.baidu.com/s/1eebBP-n-wXvOhSmIH-NUZQ 
 )(code: p91k) [google drive](https://drive.google.com/drive/folders/1H-ya1wTvjIMg2pMcMITWDIfWNSnjYxTn?usp=sharing)
@@ -211,8 +215,8 @@
 [Faster R-CNN](https://github.com/onnx/models/blob/main/vision/object_detection_segmentation/faster-rcnn) | 44.10     | 46,018
 [FCN ResNet-50](https://github.com/onnx/models/tree/main/vision/object_detection_segmentation/fcn) | 35.29     | 37,056
 [ResNet50](https://github.com/onnx/models/tree/main/vision/classification/resnet) | 25        | 3,868
 
 </td>
 </tr>
 </table>
-</p>
+</p>
```

#### html2text {}

```diff
@@ -1,28 +1,30 @@
-Metadata-Version: 2.1 Name: onnx-tool Version: 0.7.3 Summary: A tool for ONNX
-model:Rapid shape inference; Profile model; Compute Graph and Shape Engine; OPs
-fusion;Quantized models and sparse models are supported. Home-page: https://
-github.com/ThanatosShinji/onnx-tool Author: Luo Yu Author-email:
-luoyu888888@gmail.com License: MIT Classifier: Programming Language :: Python
-:: 3 Description-Content-Type: text/markdown License-File: LICENSE ç®ä½ä¸­æ
-# onnx-tool **A tool for ONNX model:** * *Rapid shape inference.* * *Profile
-model.* * *Constant_Folding.* * *Compute Graph and Shape Engine.* * *OPs
-fusion.* * *Activation memory compression.* * *Quantized models and sparse
+ç®ä½ä¸­æ # onnx-tool **A tool for ONNX model:** * *Parse and edit: Constant
+Folding; OPs fusion.* * *Model profiling: Rapid shape inference; MACs
+statistics* * *Compute Graph and Shape Engine.* * *Model memory compression:
+activation compression and weight compression.* * *Quantized models and sparse
 models are supported.* Supported Models: * NLP: BERT, T5, GPT, LLaMa, MPT
 (TransformerModel) * Diffusion: Stable Diffusion(TextEncoder, VAE, UNET) * CV:
-BEVFormer, MobileNet, YOLO, ... * Audio: sovits, LPCNet --- ## Shape inference
+BEVFormer, MobileNet, YOLO, ... * Audio: sovits, LPCNet --- ## Parse and edit
+You can load any onnx file by onnx_tool.Model: Change graph structure with
+onnx_tool.Graph; Change op attributes and IO tensors with onnx_tool.Node;
+Change tensor data or type with onnx_tool.Tensor. To apply your changes, just
+call save_model method of onnx_tool.Model or onnx_tool.Graph. Please refer
+[benchmark/samples.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/
+benchmark/samples.py). --- ## Shape inference All profiling data must be built
+on shape inference result.
     [https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/
                              shape_inference.jpg]
 how to use: [data/Profile.md](https://github.com/ThanatosShinji/onnx-tool/blob/
 main/data/Profile.md). pytorch usage: [data/PytorchUsage.md](https://
 github.com/ThanatosShinji/onnx-tool/blob/main/data/PytorchUsage.md). tensorflow
 usage: [data/TensorflowUsage.md](https://github.com/ThanatosShinji/onnx-tool/
 blob/main/data/TensorflowUsage.md). samples: [benchmark/samples.py](https://
-github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py). --- ##
-Profile Model
+github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py). ## Profile
+Model
     [https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/
                               macs_counting.png]
 Float MultipleAdd Count(1 MAC=2 FLOPs), Memory Usage(in bytes), Parameters
 (elements number)
 
     [https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/
                                sparse_model.png]
@@ -37,59 +39,66 @@
 Compute Graph with Shape Engine
     [https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/
                               compute_graph.png]
 Remove shape calculation layers(created by ONNX export) to get a *Compute
 Graph*. Use *Shape Engine* to update tensor shapes at runtime. Samples:
 [benchmark/shape_regress.py](https://github.com/ThanatosShinji/onnx-tool/blob/
 main/benchmark/shape_regress.py). [benchmark/samples.py](https://github.com/
-ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py#L123). Integrate
+ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py#L151). Integrate
 *Compute Graph* and *Shape Engine* into a cpp inference engine: [data/
 inference_engine.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/
 data/inference_engine.md) --- ## Inplace op fusion MHA and Layernorm Fusion for
 Transformers
     [https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/
                                 mha_fusion.png]
     [https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/
                              layernorm_fusion.png]
 Resnet18 fusion
     [https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/
                               resnet18_fused.png]
 how to use: [data/Subgraph.md](https://github.com/ThanatosShinji/onnx-tool/
 blob/main/data/Subgraph.md). BERT samples: [benchmark/samples.py](https://
-github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py#L100).
+github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py#L113).
 Pattern fusion: [benchmark/do_fusion.py](https://github.com/ThanatosShinji/
 onnx-tool/blob/main/benchmark/do_fusion.py). --- ## Extract subgraph from ONNX
 model Help implement model parallelism.
     [https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/
                             resnet18_subgraph.png]
 how to use: [data/Subgraph.md](https://github.com/ThanatosShinji/onnx-tool/
-blob/main/data/Subgraph.md). --- ## Memory Compression For large language
-models and high-resolution CV models, the activation memory compression is a
-key to save memory. The compression method achieves 5% memory compression on
-most models. For example: model | Native Memory Size(MB) | Compressed Memory
-Size(MB) | Compression Ratio(%) -------------------------------|---------------
----------|----------------------------|---------------------- StableDiffusion
-(VAE_encoder) | 14,245 | 540 | 3.7 StableDiffusion(VAE_decoder) | 25,417 |
-1,140 | 4.48 StableDiffusion(Text_encoder) | 215 | 5 | 2.5 StableDiffusion
-(UNet) | 36,135 | 2,232 | 6.2 GPT2 | 40 | 2 | 6.9 BERT | 2,170 | 27 | 1.25 code
-sample: [benchmark/compression.py](https://github.com/ThanatosShinji/onnx-tool/
-blob/main/benchmark/compression.py) --- ## Tensor operations * *Export weight
-tensors to files* * *Simplify tensor and node names, convert name from a long
-string to a short string* * *Remove unused tensors, models like vgg19-7.onnx
-set its static weight tensors as its input tensors* * *Set custom input and
-output tensors' name and dimension, change model from fixed input to dynamic
-input* how to use: [data/Tensors.md](https://github.com/ThanatosShinji/onnx-
-tool/blob/main/data/Tensors.md). --- ## How to install `pip install onnx-tool`
-OR `pip install --upgrade git+https://github.com/ThanatosShinji/onnx-tool.git`
+blob/main/data/Subgraph.md). --- ## Memory Compression ### Activation
+compression Activation memory also called temporary memory is created by each
+OP's output. Only the last activation marked as the model's output will be
+kept. So you don't have to prepare memory space for each activation tensor.
+They better reuse an optimized memory size. For large language models and high-
+resolution CV models, the activation memory compression is a key to save
+memory. The compression method achieves 5% memory compression on most models.
+For example: model | Native Memory Size(MB) | Compressed Memory Size(MB) |
+Compression Ratio(%) -------------------------------|------------------------|-
+---------------------------|---------------------- StableDiffusion(VAE_encoder)
+| 14,245 | 540 | 3.7 StableDiffusion(VAE_decoder) | 25,417 | 1,140 | 4.48
+StableDiffusion(Text_encoder) | 215 | 5 | 2.5 StableDiffusion(UNet) | 36,135 |
+2,232 | 6.2 GPT2 | 40 | 2 | 6.9 BERT | 2,170 | 27 | 1.25 code sample:
+[benchmark/compression.py](https://github.com/ThanatosShinji/onnx-tool/blob/
+main/benchmark/compression.py) ### Weight compression A fp32 model with 7B
+parameters will take 28GB disk space and memory space. You can not even run the
+model if your device doesn't have that much memory space. So weight compression
+is critical to run large language models. As a reference, 7B model with int4
+symmetric per block(32) quantization(llama.cpp's q4_0 quantization method) only
+has ~0.156x model size compared with fp32 model. Current support: * [fp16] *
+[int8]x[symmetric/asymmetric]x[per tensor/per channel/per block] * [int4]x
+[symmetric/asymmetric]x[per tensor/per channel/per block] code samples:
+[benchmark/samples.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/
+benchmark/samples.py#L36). --- ## How to install `pip install onnx-tool` OR
+`pip install --upgrade git+https://github.com/ThanatosShinji/onnx-tool.git`
 python>=3.6 If `pip install onnx-tool` failed by onnx's installation, you may
 try `pip install onnx==1.8.1` (a lower version like this) first. Then `pip
 install onnx-tool` again. --- ## Known Issues * Loop op is not supported *
-Activation Compression is not optimum --- ## Results of [ONNX Model Zoo](https:
-//github.com/onnx/models) and SOTA models Some models have dynamic input
-shapes. The MACs varies from input shapes. The input shapes used in these
+Tensor types created by onnx_tool are not correct --- ## Results of [ONNX Model
+Zoo](https://github.com/onnx/models) and SOTA models Some models have dynamic
+input shapes. The MACs varies from input shapes. The input shapes used in these
 results are writen to [data/public/config.py](https://github.com/
 ThanatosShinji/onnx-tool/blob/main/data/public/config.py). These onnx models
 with all tensors' shape can be downloaded: [baidu drive](https://pan.baidu.com/
 s/1eebBP-n-wXvOhSmIH-NUZQ )(code: p91k) [google drive](https://
 drive.google.com/drive/folders/1H-ya1wTvjIMg2pMcMITWDIfWNSnjYxTn?usp=sharing)
 Model | Params(M) | MACs(M) ---|---|--
 - GPT-J_1_layer | 464 | 173,398 MPT_1   Model | Params(M) | MACs(M) ---|-------
```

### Comparing `onnx-tool-0.7.3/README.md` & `onnx-tool-0.7.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,62 @@
+Metadata-Version: 2.1
+Name: onnx-tool
+Version: 0.7.4
+Summary: A tool for ONNX model:Rapid shape inference; Profile model; Compute Graph and Shape Engine; OPs fusion;Quantized models and sparse models are supported.
+Home-page: https://github.com/ThanatosShinji/onnx-tool
+Author: Luo Yu
+Author-email: luoyu888888@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a href="README_CN.md">简体中文</a>
 # onnx-tool
 
 **A tool for ONNX model:**
 
-* *Rapid shape inference.*
-* *Profile model.*
-* *<a href="data/ConstantFolding.md">Constant Folding.</a>*
+* *Parse and edit: <a href="data/ConstantFolding.md">Constant Folding</a>; OPs fusion.*
+* *Model profiling: Rapid shape inference; MACs statistics*
 * *Compute Graph and Shape Engine.*
-* *OPs fusion.*
-* *Activation memory compression.*
+* *Model memory compression: activation compression and weight compression.*
 * *Quantized models and sparse models are supported.*
 
 Supported Models:
 
 * NLP: BERT, T5, GPT, LLaMa, MPT(<a href="benchmark/transfomer_models.py">TransformerModel</a>)
 * Diffusion: Stable Diffusion(TextEncoder, VAE, UNET)
 * CV: <a href="benchmark/compression.py">BEVFormer</a>, MobileNet, YOLO, ...
 * Audio: sovits, LPCNet
 
 ---
 
-## Shape inference
+## Parse and edit
+You can load any onnx file by onnx_tool.Model:  
+Change graph structure with onnx_tool.Graph;  
+Change op attributes and IO tensors with onnx_tool.Node;  
+Change tensor data or type with onnx_tool.Tensor.  
+To apply your changes, just call save_model method of onnx_tool.Model or onnx_tool.Graph.
+
+Please refer [benchmark/samples.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py).
+
+---
 
+## Shape inference
+All profiling data must be built on shape inference result.
 <p align="center">  
   <img src="https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/shape_inference.jpg">
 </p>  
 
 how to use: [data/Profile.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/Profile.md).  
 pytorch usage: [data/PytorchUsage.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/PytorchUsage.md).  
 tensorflow
 usage: [data/TensorflowUsage.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/TensorflowUsage.md).  
 samples: [benchmark/samples.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py).
 
----
 
 ## Profile Model
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/macs_counting.png">
 </p>
 Float MultipleAdd Count(1 MAC=2 FLOPs), Memory Usage(in bytes), Parameters(elements number)<br><br>
@@ -59,15 +79,15 @@
 <p id="compute_graph" align="center">
   <img src="https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/compute_graph.png">
 </p>  
 
 Remove shape calculation layers(created by ONNX export) to get a *Compute Graph*. Use *Shape Engine* to update tensor
 shapes at runtime.  
 Samples: [benchmark/shape_regress.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/shape_regress.py).
-[benchmark/samples.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py#L123).  
+[benchmark/samples.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py#L151).  
 Integrate *Compute Graph* and *Shape Engine* into a cpp inference
 engine: [data/inference_engine.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/inference_engine.md)
 
 ---
 
 ## Inplace op fusion
 
@@ -80,15 +100,15 @@
 </p>
 Resnet18 fusion
 <p align="center">
   <img src="https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/resnet18_fused.png">
 </p>
 
 how to use: [data/Subgraph.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/Subgraph.md).  
-BERT samples: [benchmark/samples.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py#L100).  
+BERT samples: [benchmark/samples.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py#L113).  
 Pattern fusion: [benchmark/do_fusion.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/do_fusion.py).
 
 ---
 
 ## Extract subgraph from ONNX model
 Help implement model parallelism.
 <p align="center">
@@ -97,14 +117,19 @@
 
 how to use: [data/Subgraph.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/Subgraph.md).
 
 ---
 
 ## Memory Compression
 
+### Activation compression
+Activation memory also called temporary memory is created by each OP's output. Only the last activation marked as the
+model's output will be kept. So you don't have to prepare memory space for each activation tensor. They better reuse 
+an optimized memory size.
+
 For large language models and high-resolution CV models, the activation memory compression is a key to save memory.  
 The compression method achieves 5% memory compression on most models.   
 For example:
 
  model                         | Native Memory Size(MB) | Compressed Memory Size(MB) | Compression Ratio(%) 
 -------------------------------|------------------------|----------------------------|----------------------
  StableDiffusion(VAE_encoder)  | 14,245                 | 540                        | 3.7                  
@@ -112,23 +137,26 @@
  StableDiffusion(Text_encoder) | 215                    | 5                          | 2.5                  
  StableDiffusion(UNet)         | 36,135                 | 2,232                      | 6.2                  
  GPT2                          | 40                     | 2                          | 6.9                  
  BERT                          | 2,170                  | 27                         | 1.25                 
 
 code sample: [benchmark/compression.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/compression.py)
 
----
+### Weight compression
+A fp32 model with 7B parameters will take 28GB disk space and memory space. You can not even run the model if your device
+ doesn't have that much memory space. So weight compression is critical to run large language models. As a reference, 7B 
+model with int4 symmetric per block(32) quantization(llama.cpp's q4_0 quantization method) only has ~0.156x model size compared with fp32 model. 
+
+Current support:   
+* [fp16]
+* [int8]x[symmetric/asymmetric]x[per tensor/per channel/per block]  
+* [int4]x[symmetric/asymmetric]x[per tensor/per channel/per block]  
 
-## Tensor operations
+code samples:[benchmark/samples.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py#L36).  
 
-* *Export weight tensors to files*
-* *Simplify tensor and node names, convert name from a long string to a short string*
-* *Remove unused tensors, models like vgg19-7.onnx set its static weight tensors as its input tensors*
-* *Set custom input and output tensors' name and dimension, change model from fixed input to dynamic input*  
-  how to use: [data/Tensors.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/Tensors.md).
 
 ---
 
 ## How to install
     
 `pip install onnx-tool`
 
@@ -142,15 +170,15 @@
 Then `pip install onnx-tool` again.
 
 
 ---
 
 ## Known Issues
 * Loop op is not supported
-* Activation Compression is not optimum
+* Tensor types created by onnx_tool are not correct
   
 ---
 
 ## Results of [ONNX Model Zoo](https://github.com/onnx/models) and SOTA models
 Some models have dynamic input shapes. The MACs varies from input shapes. The input shapes used in these results are writen to [data/public/config.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/public/config.py).
 These onnx models with all tensors' shape can be downloaded: [baidu drive](https://pan.baidu.com/s/1eebBP-n-wXvOhSmIH-NUZQ 
 )(code: p91k) [google drive](https://drive.google.com/drive/folders/1H-ya1wTvjIMg2pMcMITWDIfWNSnjYxTn?usp=sharing)
@@ -199,8 +227,8 @@
 [Faster R-CNN](https://github.com/onnx/models/blob/main/vision/object_detection_segmentation/faster-rcnn) | 44.10     | 46,018
 [FCN ResNet-50](https://github.com/onnx/models/tree/main/vision/object_detection_segmentation/fcn) | 35.29     | 37,056
 [ResNet50](https://github.com/onnx/models/tree/main/vision/classification/resnet) | 25        | 3,868
 
 </td>
 </tr>
 </table>
-</p>
+</p>
```

#### html2text {}

```diff
@@ -1,22 +1,35 @@
-ç®ä½ä¸­æ # onnx-tool **A tool for ONNX model:** * *Rapid shape inference.*
-* *Profile model.* * *Constant_Folding.* * *Compute Graph and Shape Engine.* *
-*OPs fusion.* * *Activation memory compression.* * *Quantized models and sparse
-models are supported.* Supported Models: * NLP: BERT, T5, GPT, LLaMa, MPT
-(TransformerModel) * Diffusion: Stable Diffusion(TextEncoder, VAE, UNET) * CV:
-BEVFormer, MobileNet, YOLO, ... * Audio: sovits, LPCNet --- ## Shape inference
+Metadata-Version: 2.1 Name: onnx-tool Version: 0.7.4 Summary: A tool for ONNX
+model:Rapid shape inference; Profile model; Compute Graph and Shape Engine; OPs
+fusion;Quantized models and sparse models are supported. Home-page: https://
+github.com/ThanatosShinji/onnx-tool Author: Luo Yu Author-email:
+luoyu888888@gmail.com License: MIT Classifier: Programming Language :: Python
+:: 3 Description-Content-Type: text/markdown License-File: LICENSE ç®ä½ä¸­æ
+# onnx-tool **A tool for ONNX model:** * *Parse and edit: Constant_Folding; OPs
+fusion.* * *Model profiling: Rapid shape inference; MACs statistics* * *Compute
+Graph and Shape Engine.* * *Model memory compression: activation compression
+and weight compression.* * *Quantized models and sparse models are supported.*
+Supported Models: * NLP: BERT, T5, GPT, LLaMa, MPT(TransformerModel) *
+Diffusion: Stable Diffusion(TextEncoder, VAE, UNET) * CV: BEVFormer, MobileNet,
+YOLO, ... * Audio: sovits, LPCNet --- ## Parse and edit You can load any onnx
+file by onnx_tool.Model: Change graph structure with onnx_tool.Graph; Change op
+attributes and IO tensors with onnx_tool.Node; Change tensor data or type with
+onnx_tool.Tensor. To apply your changes, just call save_model method of
+onnx_tool.Model or onnx_tool.Graph. Please refer [benchmark/samples.py](https:/
+/github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py). --- ##
+Shape inference All profiling data must be built on shape inference result.
     [https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/
                              shape_inference.jpg]
 how to use: [data/Profile.md](https://github.com/ThanatosShinji/onnx-tool/blob/
 main/data/Profile.md). pytorch usage: [data/PytorchUsage.md](https://
 github.com/ThanatosShinji/onnx-tool/blob/main/data/PytorchUsage.md). tensorflow
 usage: [data/TensorflowUsage.md](https://github.com/ThanatosShinji/onnx-tool/
 blob/main/data/TensorflowUsage.md). samples: [benchmark/samples.py](https://
-github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py). --- ##
-Profile Model
+github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py). ## Profile
+Model
     [https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/
                               macs_counting.png]
 Float MultipleAdd Count(1 MAC=2 FLOPs), Memory Usage(in bytes), Parameters
 (elements number)
 
     [https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/
                                sparse_model.png]
@@ -31,59 +44,66 @@
 Compute Graph with Shape Engine
     [https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/
                               compute_graph.png]
 Remove shape calculation layers(created by ONNX export) to get a *Compute
 Graph*. Use *Shape Engine* to update tensor shapes at runtime. Samples:
 [benchmark/shape_regress.py](https://github.com/ThanatosShinji/onnx-tool/blob/
 main/benchmark/shape_regress.py). [benchmark/samples.py](https://github.com/
-ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py#L123). Integrate
+ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py#L151). Integrate
 *Compute Graph* and *Shape Engine* into a cpp inference engine: [data/
 inference_engine.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/
 data/inference_engine.md) --- ## Inplace op fusion MHA and Layernorm Fusion for
 Transformers
     [https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/
                                 mha_fusion.png]
     [https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/
                              layernorm_fusion.png]
 Resnet18 fusion
     [https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/
                               resnet18_fused.png]
 how to use: [data/Subgraph.md](https://github.com/ThanatosShinji/onnx-tool/
 blob/main/data/Subgraph.md). BERT samples: [benchmark/samples.py](https://
-github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py#L100).
+github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py#L113).
 Pattern fusion: [benchmark/do_fusion.py](https://github.com/ThanatosShinji/
 onnx-tool/blob/main/benchmark/do_fusion.py). --- ## Extract subgraph from ONNX
 model Help implement model parallelism.
     [https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/
                             resnet18_subgraph.png]
 how to use: [data/Subgraph.md](https://github.com/ThanatosShinji/onnx-tool/
-blob/main/data/Subgraph.md). --- ## Memory Compression For large language
-models and high-resolution CV models, the activation memory compression is a
-key to save memory. The compression method achieves 5% memory compression on
-most models. For example: model | Native Memory Size(MB) | Compressed Memory
-Size(MB) | Compression Ratio(%) -------------------------------|---------------
----------|----------------------------|---------------------- StableDiffusion
-(VAE_encoder) | 14,245 | 540 | 3.7 StableDiffusion(VAE_decoder) | 25,417 |
-1,140 | 4.48 StableDiffusion(Text_encoder) | 215 | 5 | 2.5 StableDiffusion
-(UNet) | 36,135 | 2,232 | 6.2 GPT2 | 40 | 2 | 6.9 BERT | 2,170 | 27 | 1.25 code
-sample: [benchmark/compression.py](https://github.com/ThanatosShinji/onnx-tool/
-blob/main/benchmark/compression.py) --- ## Tensor operations * *Export weight
-tensors to files* * *Simplify tensor and node names, convert name from a long
-string to a short string* * *Remove unused tensors, models like vgg19-7.onnx
-set its static weight tensors as its input tensors* * *Set custom input and
-output tensors' name and dimension, change model from fixed input to dynamic
-input* how to use: [data/Tensors.md](https://github.com/ThanatosShinji/onnx-
-tool/blob/main/data/Tensors.md). --- ## How to install `pip install onnx-tool`
-OR `pip install --upgrade git+https://github.com/ThanatosShinji/onnx-tool.git`
+blob/main/data/Subgraph.md). --- ## Memory Compression ### Activation
+compression Activation memory also called temporary memory is created by each
+OP's output. Only the last activation marked as the model's output will be
+kept. So you don't have to prepare memory space for each activation tensor.
+They better reuse an optimized memory size. For large language models and high-
+resolution CV models, the activation memory compression is a key to save
+memory. The compression method achieves 5% memory compression on most models.
+For example: model | Native Memory Size(MB) | Compressed Memory Size(MB) |
+Compression Ratio(%) -------------------------------|------------------------|-
+---------------------------|---------------------- StableDiffusion(VAE_encoder)
+| 14,245 | 540 | 3.7 StableDiffusion(VAE_decoder) | 25,417 | 1,140 | 4.48
+StableDiffusion(Text_encoder) | 215 | 5 | 2.5 StableDiffusion(UNet) | 36,135 |
+2,232 | 6.2 GPT2 | 40 | 2 | 6.9 BERT | 2,170 | 27 | 1.25 code sample:
+[benchmark/compression.py](https://github.com/ThanatosShinji/onnx-tool/blob/
+main/benchmark/compression.py) ### Weight compression A fp32 model with 7B
+parameters will take 28GB disk space and memory space. You can not even run the
+model if your device doesn't have that much memory space. So weight compression
+is critical to run large language models. As a reference, 7B model with int4
+symmetric per block(32) quantization(llama.cpp's q4_0 quantization method) only
+has ~0.156x model size compared with fp32 model. Current support: * [fp16] *
+[int8]x[symmetric/asymmetric]x[per tensor/per channel/per block] * [int4]x
+[symmetric/asymmetric]x[per tensor/per channel/per block] code samples:
+[benchmark/samples.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/
+benchmark/samples.py#L36). --- ## How to install `pip install onnx-tool` OR
+`pip install --upgrade git+https://github.com/ThanatosShinji/onnx-tool.git`
 python>=3.6 If `pip install onnx-tool` failed by onnx's installation, you may
 try `pip install onnx==1.8.1` (a lower version like this) first. Then `pip
 install onnx-tool` again. --- ## Known Issues * Loop op is not supported *
-Activation Compression is not optimum --- ## Results of [ONNX Model Zoo](https:
-//github.com/onnx/models) and SOTA models Some models have dynamic input
-shapes. The MACs varies from input shapes. The input shapes used in these
+Tensor types created by onnx_tool are not correct --- ## Results of [ONNX Model
+Zoo](https://github.com/onnx/models) and SOTA models Some models have dynamic
+input shapes. The MACs varies from input shapes. The input shapes used in these
 results are writen to [data/public/config.py](https://github.com/
 ThanatosShinji/onnx-tool/blob/main/data/public/config.py). These onnx models
 with all tensors' shape can be downloaded: [baidu drive](https://pan.baidu.com/
 s/1eebBP-n-wXvOhSmIH-NUZQ )(code: p91k) [google drive](https://
 drive.google.com/drive/folders/1H-ya1wTvjIMg2pMcMITWDIfWNSnjYxTn?usp=sharing)
 Model | Params(M) | MACs(M) ---|---|--
 - GPT-J_1_layer | 464 | 173,398 MPT_1   Model | Params(M) | MACs(M) ---|-------
```

### Comparing `onnx-tool-0.7.3/onnx_tool/__init__.py` & `onnx-tool-0.7.4/onnx_tool/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     g.graph_reorder_nodes()
     gtmr.start()
     g.shape_infer(dynamic_shapes)
     g.log(f'infered all tensor shapes, time cost {gtmr.stop():.3f} s')
     gtmr.start()
     g.profile()
     g.log(f'profile all nodes, time cost {gtmr.stop():.3f} s')
-    g.print_node_map(savenode, exclude_nodes=hidden_ops)
+    g.print_node_map(savenode, exclude_ops=hidden_ops)
     if saveshapesmodel is not None:
         model.save_model(saveshapesmodel, shape_only=shapesonly)
 
 
 def model_shape_regress(m, input_desc: {}, input_range: {}):
     model = loadmodel(m)
     graph = model.graph
```

### Comparing `onnx-tool-0.7.3/onnx_tool/__main__.py` & `onnx-tool-0.7.4/onnx_tool/__main__.py`

 * *Files identical despite different names*

### Comparing `onnx-tool-0.7.3/onnx_tool/fusion.py` & `onnx-tool-0.7.4/onnx_tool/fusion.py`

 * *Files identical despite different names*

### Comparing `onnx-tool-0.7.3/onnx_tool/graph.py` & `onnx-tool-0.7.4/onnx_tool/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -530,14 +530,15 @@
                             self.consumedby[indtensor].append(con)
                             break
             else:
                 for pro in self.producedby[indtensor]:
                     pro_node = self.nodemap[pro]
                     assert (len(pro_node.output) == 1)
                     pro_node.output[0] = node.output[0]
+        self.nodemap.pop(nodename)
 
     def fuse_subgraph_node_names(self, nodes: [str], nodeop: str, nodename: str, keep_attr=True):
         _inputs, _outputs = self.get_iotensors(nodes, remove_initials=False)
         newnode = onnx.helper.make_node(nodeop, _inputs, _outputs, name=nodename)
         count = 0
         if keep_attr:
             for node in nodes:
@@ -675,14 +676,21 @@
                 if key in self.input or key in self.output:
                     continue
                 tensor = self.tensormap[key]
                 vinfo = tensor.make_value_proto()
                 if vinfo is None:
                     continue
                 value_infos.append(vinfo)
+            if not with_initializer:
+                 for key in self.initials:
+                    tensor = self.tensormap[key]
+                    vinfo = tensor.make_value_proto()
+                    if vinfo is None:
+                        continue
+                    value_infos.append(vinfo)
         graph = onnx.helper.make_graph(nodes=nodes, name=gname, inputs=inputs, outputs=outputs, initializer=initializer,
                                        value_info=value_infos)
         return graph
 
     def topsort_nodes(self, node_names, input_names):
         # update
         produced_by = {}
@@ -1219,15 +1227,15 @@
             node.sparsity = block_sparsity
             self.macs += macs
             self.params += _params
             self.memory += _memory
 
         self.valid_profile = True
 
-    def print_node_map(self, f: str = None, metric='MACs', exclude_nodes=None):
+    def print_node_map(self, f: str = None, metric='MACs', exclude_ops=None):
         if not self.valid_profile:
             warnings.warn('Please perform a valid profile() before print_node_map().')
             return
         from tabulate import tabulate
         assert (metric in ['MACs', 'FLOPs'])
         print_sparse_table = self.sparse_model
         saveformat = 'txt'
@@ -1276,15 +1284,15 @@
             else:
                 return '{:,}'.format(num)
 
         params += 1e-18
         macs += 1e-18
         for key in self.nodemap.keys():
             node = self.nodemap[key]
-            if exclude_nodes is not None and node.op_type in exclude_nodes:
+            if exclude_ops is not None and node.op_type in exclude_ops:
                 continue
             row = [key, self.nodemap[key].op_type]
             if print_sparse_table:
                 sparsity = node.sparsity
                 row.append(tuple2str(sparsity['blocksize'], splitch))
                 row.append('{:.2%}'.format(sparsity['blockratio']))
                 row.append('{:.2%}'.format(sparsity['ratio']))
```

### Comparing `onnx-tool-0.7.3/onnx_tool/model.py` & `onnx-tool-0.7.4/onnx_tool/model.py`

 * *Files identical despite different names*

### Comparing `onnx-tool-0.7.3/onnx_tool/node.py` & `onnx-tool-0.7.4/onnx_tool/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,14 +135,18 @@
         for att in n.attribute:
             self.attr[att.name] = onnx.helper.get_attribute_value(att)
             self.__setattr__(att.name, get_attribute_data(att))
             if att.name == 'axes':
                 if isinstance(self.axes, list):
                     self.axes = tuple(self.axes)
 
+    def set_attr(self,key,val):
+        self.attr[key]=val
+        self.__setattr__(key,val)
+
     def add_default_value(self, attname, defaultvalue):
         if not hasattr(self, attname):
             setattr(self, attname, defaultvalue)
 
     def make_nodeproto(self):
         return onnx.helper.make_node(self.op_type, self.input, self.output, self.name, **self.attr)
 
@@ -417,15 +421,15 @@
         return [y]
 
 
 @NODE_REGISTRY.register()
 class TanhNode(PWNode):
     def __init__(self, n):
         super().__init__(n)
-        self.op_mac = EXP_MACS
+        self.op_mac = TANH_MACS
         self.ratio = 2
 
     def value_infer(self, intensors: []):
         return [numpy.tanh(intensors[0])]
 
 
 @NODE_REGISTRY.register()
@@ -455,14 +459,27 @@
         self.op_mac = MUL_MACS + ADD_MACS + CMP_MACS * 2
         self.add_default_value('alpha',0.2)
         self.add_default_value('beta',0.5)
 
     def value_infer(self, intensors: []):
         y = max(0, min(1, self.alpha * intensors[0] + self.beta))
         return [y]
+    
+
+@NODE_REGISTRY.register()
+class HardSwishNode(PWNode):
+    def __init__(self, node_proto):
+        super().__init__(node_proto)
+        self.op_mac = MUL_MACS * 2 + ADD_MACS + CMP_MACS * 2
+        self.add_default_value('alpha',1/6)
+        self.add_default_value('beta',0.5)
+
+    def value_infer(self, intensors: []):
+        y = intensors[0] * max(0, min(1, self.alpha * intensors[0] + self.beta))
+        return [y]
 
 
 @NODE_REGISTRY.register()
 class ReluNode(PWNode):
     def __init__(self, n):
         super().__init__(n)
         self.op_mac = CMP_MACS
@@ -1183,14 +1200,20 @@
             sqrt_var=math.sqrt(var[cn]+self.epsilon)
             sm=scale[cn]/sqrt_var
             sv=b[cn]
             m=mean[cn]
             y[i]=(x[i]-m)*sm+sv
         return [y]
 
+    # Fusion of batchnorm is determined by inference engine, here just gives the MACs.
+    def profile(self, intensors: [], outtensors: []):
+        base = volume(_get_shape(outtensors[0]))
+        base *= ADD_MACS + SQRT_MACS + DIV_MACS + ADD_MACS + MUL_MACS
+        return base
+
 @NODE_REGISTRY.register()
 class FlattenNode(Node):
     def __init__(self, node):
         super().__init__(node)
         self.add_default_value('axis', None)
 
     def value_infer(self, intensors: []):
@@ -1616,19 +1639,19 @@
 
     def profile(self, intensors: [], outtensors: []):
         macs = 0
         if len(outtensors) == 1:
             if len(intensors) == 3 or len(intensors) == 2:
                 kernel_shape = _get_shape(intensors[1])
                 outvol = volume(_get_shape(outtensors[0]))
-                if len(kernel_shape) > 3:
-                    macs += outvol * kernel_shape[1] * kernel_shape[2] * kernel_shape[3]
-                elif len(kernel_shape) == 3:
-                    macs += outvol * kernel_shape[1] * kernel_shape[2]
-                macs += (outvol * ADD_MACS)
+                reduce_shape=kernel_shape[1:]
+                reduce_vol=volume(reduce_shape)
+                macs+=outvol*reduce_vol * MUL_MACS
+                if len(intensors)>2:
+                    macs += (outvol * ADD_MACS)
         return macs
 
 
 @NODE_REGISTRY.register()
 class ReduceL2Node(Node):
     def __init__(self, nodeproto):
         super().__init__(nodeproto)
@@ -2017,21 +2040,19 @@
         return [shape, ]
 
     def profile(self, intensors: [], outtensors: []):
         macs = 0
         if len(outtensors) == 1:
             if len(intensors) == 3 or len(intensors) == 2:
                 kernel_shape = _get_shape(intensors[1])
-                if len(kernel_shape) > 3:
-                    outvol = volume(_get_shape(outtensors[0]))
-                    macs += outvol * kernel_shape[1] * kernel_shape[2] * kernel_shape[3]
-                    macs += outvol * ADD_MACS  # treat bias add as 0.5 MACs
-                elif len(kernel_shape) == 3:
-                    outvol = volume(_get_shape(outtensors[0]))
-                    macs += outvol * kernel_shape[1] * kernel_shape[2]
+                outvol = volume(_get_shape(outtensors[0]))
+                reduce_shape = kernel_shape[1:]
+                reduce_vol = volume(reduce_shape)
+                macs += outvol * reduce_vol * MUL_MACS
+                if len(intensors) > 2:
                     macs += (outvol * ADD_MACS)
         return macs
 
 
 @NODE_REGISTRY.register()
 class ReshapeNode(Node):
     def shape_infer(self, intensors: []):
```

### Comparing `onnx-tool-0.7.3/onnx_tool/serialization.py` & `onnx-tool-0.7.4/onnx_tool/serialization.py`

 * *Files identical despite different names*

### Comparing `onnx-tool-0.7.3/onnx_tool/tensor.py` & `onnx-tool-0.7.4/onnx_tool/tensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,14 +106,15 @@
             arr = numpy.array(initial.string_data, dtype=ndtype)
     else:
         arr = numpy.frombuffer(initial.raw_data, dtype=ndtype)
     # if len(shape):
     arr = arr.reshape(shape)
     return arr
 
+
 def get_attribute_data(att):
     if att.type == att.INTS:
         val = []
         for ints in att.ints:
             val.append(ints)
         return val
     elif att.type == att.INT:
@@ -429,21 +430,17 @@
         if (volume(shape) > thres_size) and self.numpy is not None:
             ratio = narray_calc_sparsity(self.numpy)
             if ratio is not None and ratio > thres_ratio:
                 blocksize, blockratio = search_sparse_blocksize(self.numpy, ratio, deltar_thres=0.1)
         self.sparsity = {'blocksize': blocksize, 'blockratio': blockratio, 'ratio': ratio}
 
     def make_value_proto(self, make_dummy=False):
+        shape = self.get_shape()
         if len(self.shape) == 0:
-            if self.proto is None and make_dummy:
-                warnings.warn('Creating a dummpy tensor proto:' + self.name)
-                return onnx.helper.make_tensor_value_info(self.name, 1, None)
-            return self.proto
-        else:
-            shape = self.get_shape()
+            shape = None
         if self.numpy is None:
             if self.proto is not None:
                 dtype = self.proto.type.tensor_type.elem_type
             else:
                 dtype = onnx.TensorProto.FLOAT
         else:
             dtype = npdtype2onnxdtype(self.numpy.dtype)
@@ -454,16 +451,22 @@
     def make_tensor_proto(self):
         if self.numpy is None:
             return None
         if len(self.numpy.shape) == 0:
             tproto = onnx.helper.make_tensor(self.name, npdtype2onnxdtype(self.numpy.dtype)
                                              , [], [self.numpy.item()])
         else:
+            if self.numpy.dtype not in [numpy.float32, numpy.int32]:
+                raw = True
+                data = self.numpy.tobytes()
+            else:
+                raw = False
+                data = self.numpy.flatten()
             tproto = onnx.helper.make_tensor(self.name, npdtype2onnxdtype(self.numpy.dtype)
-                                             , self.numpy.shape, self.numpy.flatten())
+                                             , self.numpy.shape, data, raw=raw)
         return tproto
 
 
 def create_initial_Tensor(name: str, ndarray: numpy.ndarray):
     t = Tensor(name)
     t.type = STATIC_TENSOR
     t.numpy = ndarray
```

### Comparing `onnx-tool-0.7.3/onnx_tool/utils.py` & `onnx-tool-0.7.4/onnx_tool/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import time
 import warnings
 
-VERSION = "0.7.3"
+VERSION = "0.7.4"
 
 
 class timer():
     def __init__(self):
         self._startt = time.time()
 
     def start(self):
```

### Comparing `onnx-tool-0.7.3/onnx_tool.egg-info/PKG-INFO` & `onnx-tool-0.7.4/onnx_tool.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,62 @@
 Metadata-Version: 2.1
 Name: onnx-tool
-Version: 0.7.3
+Version: 0.7.4
 Summary: A tool for ONNX model:Rapid shape inference; Profile model; Compute Graph and Shape Engine; OPs fusion;Quantized models and sparse models are supported.
 Home-page: https://github.com/ThanatosShinji/onnx-tool
 Author: Luo Yu
 Author-email: luoyu888888@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a href="README_CN.md">简体中文</a>
 # onnx-tool
 
 **A tool for ONNX model:**
 
-* *Rapid shape inference.*
-* *Profile model.*
-* *<a href="data/ConstantFolding.md">Constant Folding.</a>*
+* *Parse and edit: <a href="data/ConstantFolding.md">Constant Folding</a>; OPs fusion.*
+* *Model profiling: Rapid shape inference; MACs statistics*
 * *Compute Graph and Shape Engine.*
-* *OPs fusion.*
-* *Activation memory compression.*
+* *Model memory compression: activation compression and weight compression.*
 * *Quantized models and sparse models are supported.*
 
 Supported Models:
 
 * NLP: BERT, T5, GPT, LLaMa, MPT(<a href="benchmark/transfomer_models.py">TransformerModel</a>)
 * Diffusion: Stable Diffusion(TextEncoder, VAE, UNET)
 * CV: <a href="benchmark/compression.py">BEVFormer</a>, MobileNet, YOLO, ...
 * Audio: sovits, LPCNet
 
 ---
 
-## Shape inference
+## Parse and edit
+You can load any onnx file by onnx_tool.Model:  
+Change graph structure with onnx_tool.Graph;  
+Change op attributes and IO tensors with onnx_tool.Node;  
+Change tensor data or type with onnx_tool.Tensor.  
+To apply your changes, just call save_model method of onnx_tool.Model or onnx_tool.Graph.
+
+Please refer [benchmark/samples.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py).
+
+---
 
+## Shape inference
+All profiling data must be built on shape inference result.
 <p align="center">  
   <img src="https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/shape_inference.jpg">
 </p>  
 
 how to use: [data/Profile.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/Profile.md).  
 pytorch usage: [data/PytorchUsage.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/PytorchUsage.md).  
 tensorflow
 usage: [data/TensorflowUsage.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/TensorflowUsage.md).  
 samples: [benchmark/samples.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py).
 
----
 
 ## Profile Model
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/macs_counting.png">
 </p>
 Float MultipleAdd Count(1 MAC=2 FLOPs), Memory Usage(in bytes), Parameters(elements number)<br><br>
@@ -71,15 +79,15 @@
 <p id="compute_graph" align="center">
   <img src="https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/compute_graph.png">
 </p>  
 
 Remove shape calculation layers(created by ONNX export) to get a *Compute Graph*. Use *Shape Engine* to update tensor
 shapes at runtime.  
 Samples: [benchmark/shape_regress.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/shape_regress.py).
-[benchmark/samples.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py#L123).  
+[benchmark/samples.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py#L151).  
 Integrate *Compute Graph* and *Shape Engine* into a cpp inference
 engine: [data/inference_engine.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/inference_engine.md)
 
 ---
 
 ## Inplace op fusion
 
@@ -92,15 +100,15 @@
 </p>
 Resnet18 fusion
 <p align="center">
   <img src="https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/resnet18_fused.png">
 </p>
 
 how to use: [data/Subgraph.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/Subgraph.md).  
-BERT samples: [benchmark/samples.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py#L100).  
+BERT samples: [benchmark/samples.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py#L113).  
 Pattern fusion: [benchmark/do_fusion.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/do_fusion.py).
 
 ---
 
 ## Extract subgraph from ONNX model
 Help implement model parallelism.
 <p align="center">
@@ -109,14 +117,19 @@
 
 how to use: [data/Subgraph.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/Subgraph.md).
 
 ---
 
 ## Memory Compression
 
+### Activation compression
+Activation memory also called temporary memory is created by each OP's output. Only the last activation marked as the
+model's output will be kept. So you don't have to prepare memory space for each activation tensor. They better reuse 
+an optimized memory size.
+
 For large language models and high-resolution CV models, the activation memory compression is a key to save memory.  
 The compression method achieves 5% memory compression on most models.   
 For example:
 
  model                         | Native Memory Size(MB) | Compressed Memory Size(MB) | Compression Ratio(%) 
 -------------------------------|------------------------|----------------------------|----------------------
  StableDiffusion(VAE_encoder)  | 14,245                 | 540                        | 3.7                  
@@ -124,23 +137,26 @@
  StableDiffusion(Text_encoder) | 215                    | 5                          | 2.5                  
  StableDiffusion(UNet)         | 36,135                 | 2,232                      | 6.2                  
  GPT2                          | 40                     | 2                          | 6.9                  
  BERT                          | 2,170                  | 27                         | 1.25                 
 
 code sample: [benchmark/compression.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/compression.py)
 
----
+### Weight compression
+A fp32 model with 7B parameters will take 28GB disk space and memory space. You can not even run the model if your device
+ doesn't have that much memory space. So weight compression is critical to run large language models. As a reference, 7B 
+model with int4 symmetric per block(32) quantization(llama.cpp's q4_0 quantization method) only has ~0.156x model size compared with fp32 model. 
+
+Current support:   
+* [fp16]
+* [int8]x[symmetric/asymmetric]x[per tensor/per channel/per block]  
+* [int4]x[symmetric/asymmetric]x[per tensor/per channel/per block]  
 
-## Tensor operations
+code samples:[benchmark/samples.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py#L36).  
 
-* *Export weight tensors to files*
-* *Simplify tensor and node names, convert name from a long string to a short string*
-* *Remove unused tensors, models like vgg19-7.onnx set its static weight tensors as its input tensors*
-* *Set custom input and output tensors' name and dimension, change model from fixed input to dynamic input*  
-  how to use: [data/Tensors.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/Tensors.md).
 
 ---
 
 ## How to install
     
 `pip install onnx-tool`
 
@@ -154,15 +170,15 @@
 Then `pip install onnx-tool` again.
 
 
 ---
 
 ## Known Issues
 * Loop op is not supported
-* Activation Compression is not optimum
+* Tensor types created by onnx_tool are not correct
   
 ---
 
 ## Results of [ONNX Model Zoo](https://github.com/onnx/models) and SOTA models
 Some models have dynamic input shapes. The MACs varies from input shapes. The input shapes used in these results are writen to [data/public/config.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/data/public/config.py).
 These onnx models with all tensors' shape can be downloaded: [baidu drive](https://pan.baidu.com/s/1eebBP-n-wXvOhSmIH-NUZQ 
 )(code: p91k) [google drive](https://drive.google.com/drive/folders/1H-ya1wTvjIMg2pMcMITWDIfWNSnjYxTn?usp=sharing)
```

#### html2text {}

```diff
@@ -1,28 +1,35 @@
-Metadata-Version: 2.1 Name: onnx-tool Version: 0.7.3 Summary: A tool for ONNX
+Metadata-Version: 2.1 Name: onnx-tool Version: 0.7.4 Summary: A tool for ONNX
 model:Rapid shape inference; Profile model; Compute Graph and Shape Engine; OPs
 fusion;Quantized models and sparse models are supported. Home-page: https://
 github.com/ThanatosShinji/onnx-tool Author: Luo Yu Author-email:
 luoyu888888@gmail.com License: MIT Classifier: Programming Language :: Python
 :: 3 Description-Content-Type: text/markdown License-File: LICENSE ç®ä½ä¸­æ
-# onnx-tool **A tool for ONNX model:** * *Rapid shape inference.* * *Profile
-model.* * *Constant_Folding.* * *Compute Graph and Shape Engine.* * *OPs
-fusion.* * *Activation memory compression.* * *Quantized models and sparse
-models are supported.* Supported Models: * NLP: BERT, T5, GPT, LLaMa, MPT
-(TransformerModel) * Diffusion: Stable Diffusion(TextEncoder, VAE, UNET) * CV:
-BEVFormer, MobileNet, YOLO, ... * Audio: sovits, LPCNet --- ## Shape inference
+# onnx-tool **A tool for ONNX model:** * *Parse and edit: Constant_Folding; OPs
+fusion.* * *Model profiling: Rapid shape inference; MACs statistics* * *Compute
+Graph and Shape Engine.* * *Model memory compression: activation compression
+and weight compression.* * *Quantized models and sparse models are supported.*
+Supported Models: * NLP: BERT, T5, GPT, LLaMa, MPT(TransformerModel) *
+Diffusion: Stable Diffusion(TextEncoder, VAE, UNET) * CV: BEVFormer, MobileNet,
+YOLO, ... * Audio: sovits, LPCNet --- ## Parse and edit You can load any onnx
+file by onnx_tool.Model: Change graph structure with onnx_tool.Graph; Change op
+attributes and IO tensors with onnx_tool.Node; Change tensor data or type with
+onnx_tool.Tensor. To apply your changes, just call save_model method of
+onnx_tool.Model or onnx_tool.Graph. Please refer [benchmark/samples.py](https:/
+/github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py). --- ##
+Shape inference All profiling data must be built on shape inference result.
     [https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/
                              shape_inference.jpg]
 how to use: [data/Profile.md](https://github.com/ThanatosShinji/onnx-tool/blob/
 main/data/Profile.md). pytorch usage: [data/PytorchUsage.md](https://
 github.com/ThanatosShinji/onnx-tool/blob/main/data/PytorchUsage.md). tensorflow
 usage: [data/TensorflowUsage.md](https://github.com/ThanatosShinji/onnx-tool/
 blob/main/data/TensorflowUsage.md). samples: [benchmark/samples.py](https://
-github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py). --- ##
-Profile Model
+github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py). ## Profile
+Model
     [https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/
                               macs_counting.png]
 Float MultipleAdd Count(1 MAC=2 FLOPs), Memory Usage(in bytes), Parameters
 (elements number)
 
     [https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/
                                sparse_model.png]
@@ -37,59 +44,66 @@
 Compute Graph with Shape Engine
     [https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/
                               compute_graph.png]
 Remove shape calculation layers(created by ONNX export) to get a *Compute
 Graph*. Use *Shape Engine* to update tensor shapes at runtime. Samples:
 [benchmark/shape_regress.py](https://github.com/ThanatosShinji/onnx-tool/blob/
 main/benchmark/shape_regress.py). [benchmark/samples.py](https://github.com/
-ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py#L123). Integrate
+ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py#L151). Integrate
 *Compute Graph* and *Shape Engine* into a cpp inference engine: [data/
 inference_engine.md](https://github.com/ThanatosShinji/onnx-tool/blob/main/
 data/inference_engine.md) --- ## Inplace op fusion MHA and Layernorm Fusion for
 Transformers
     [https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/
                                 mha_fusion.png]
     [https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/
                              layernorm_fusion.png]
 Resnet18 fusion
     [https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/
                               resnet18_fused.png]
 how to use: [data/Subgraph.md](https://github.com/ThanatosShinji/onnx-tool/
 blob/main/data/Subgraph.md). BERT samples: [benchmark/samples.py](https://
-github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py#L100).
+github.com/ThanatosShinji/onnx-tool/blob/main/benchmark/samples.py#L113).
 Pattern fusion: [benchmark/do_fusion.py](https://github.com/ThanatosShinji/
 onnx-tool/blob/main/benchmark/do_fusion.py). --- ## Extract subgraph from ONNX
 model Help implement model parallelism.
     [https://raw.githubusercontent.com/ThanatosShinji/onnx-tool/main/data/
                             resnet18_subgraph.png]
 how to use: [data/Subgraph.md](https://github.com/ThanatosShinji/onnx-tool/
-blob/main/data/Subgraph.md). --- ## Memory Compression For large language
-models and high-resolution CV models, the activation memory compression is a
-key to save memory. The compression method achieves 5% memory compression on
-most models. For example: model | Native Memory Size(MB) | Compressed Memory
-Size(MB) | Compression Ratio(%) -------------------------------|---------------
----------|----------------------------|---------------------- StableDiffusion
-(VAE_encoder) | 14,245 | 540 | 3.7 StableDiffusion(VAE_decoder) | 25,417 |
-1,140 | 4.48 StableDiffusion(Text_encoder) | 215 | 5 | 2.5 StableDiffusion
-(UNet) | 36,135 | 2,232 | 6.2 GPT2 | 40 | 2 | 6.9 BERT | 2,170 | 27 | 1.25 code
-sample: [benchmark/compression.py](https://github.com/ThanatosShinji/onnx-tool/
-blob/main/benchmark/compression.py) --- ## Tensor operations * *Export weight
-tensors to files* * *Simplify tensor and node names, convert name from a long
-string to a short string* * *Remove unused tensors, models like vgg19-7.onnx
-set its static weight tensors as its input tensors* * *Set custom input and
-output tensors' name and dimension, change model from fixed input to dynamic
-input* how to use: [data/Tensors.md](https://github.com/ThanatosShinji/onnx-
-tool/blob/main/data/Tensors.md). --- ## How to install `pip install onnx-tool`
-OR `pip install --upgrade git+https://github.com/ThanatosShinji/onnx-tool.git`
+blob/main/data/Subgraph.md). --- ## Memory Compression ### Activation
+compression Activation memory also called temporary memory is created by each
+OP's output. Only the last activation marked as the model's output will be
+kept. So you don't have to prepare memory space for each activation tensor.
+They better reuse an optimized memory size. For large language models and high-
+resolution CV models, the activation memory compression is a key to save
+memory. The compression method achieves 5% memory compression on most models.
+For example: model | Native Memory Size(MB) | Compressed Memory Size(MB) |
+Compression Ratio(%) -------------------------------|------------------------|-
+---------------------------|---------------------- StableDiffusion(VAE_encoder)
+| 14,245 | 540 | 3.7 StableDiffusion(VAE_decoder) | 25,417 | 1,140 | 4.48
+StableDiffusion(Text_encoder) | 215 | 5 | 2.5 StableDiffusion(UNet) | 36,135 |
+2,232 | 6.2 GPT2 | 40 | 2 | 6.9 BERT | 2,170 | 27 | 1.25 code sample:
+[benchmark/compression.py](https://github.com/ThanatosShinji/onnx-tool/blob/
+main/benchmark/compression.py) ### Weight compression A fp32 model with 7B
+parameters will take 28GB disk space and memory space. You can not even run the
+model if your device doesn't have that much memory space. So weight compression
+is critical to run large language models. As a reference, 7B model with int4
+symmetric per block(32) quantization(llama.cpp's q4_0 quantization method) only
+has ~0.156x model size compared with fp32 model. Current support: * [fp16] *
+[int8]x[symmetric/asymmetric]x[per tensor/per channel/per block] * [int4]x
+[symmetric/asymmetric]x[per tensor/per channel/per block] code samples:
+[benchmark/samples.py](https://github.com/ThanatosShinji/onnx-tool/blob/main/
+benchmark/samples.py#L36). --- ## How to install `pip install onnx-tool` OR
+`pip install --upgrade git+https://github.com/ThanatosShinji/onnx-tool.git`
 python>=3.6 If `pip install onnx-tool` failed by onnx's installation, you may
 try `pip install onnx==1.8.1` (a lower version like this) first. Then `pip
 install onnx-tool` again. --- ## Known Issues * Loop op is not supported *
-Activation Compression is not optimum --- ## Results of [ONNX Model Zoo](https:
-//github.com/onnx/models) and SOTA models Some models have dynamic input
-shapes. The MACs varies from input shapes. The input shapes used in these
+Tensor types created by onnx_tool are not correct --- ## Results of [ONNX Model
+Zoo](https://github.com/onnx/models) and SOTA models Some models have dynamic
+input shapes. The MACs varies from input shapes. The input shapes used in these
 results are writen to [data/public/config.py](https://github.com/
 ThanatosShinji/onnx-tool/blob/main/data/public/config.py). These onnx models
 with all tensors' shape can be downloaded: [baidu drive](https://pan.baidu.com/
 s/1eebBP-n-wXvOhSmIH-NUZQ )(code: p91k) [google drive](https://
 drive.google.com/drive/folders/1H-ya1wTvjIMg2pMcMITWDIfWNSnjYxTn?usp=sharing)
 Model | Params(M) | MACs(M) ---|---|--
 - GPT-J_1_layer | 464 | 173,398 MPT_1   Model | Params(M) | MACs(M) ---|-------
```

### Comparing `onnx-tool-0.7.3/setup.py` & `onnx-tool-0.7.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 readme = open("README.md", encoding="utf-8").read()
-VERSION = "0.7.3"
+VERSION = "0.7.4"
 
 requirements = [
     "onnx",
     "numpy",
     'tabulate'
 ]
```

