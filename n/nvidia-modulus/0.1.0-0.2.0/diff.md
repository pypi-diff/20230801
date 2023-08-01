# Comparing `tmp/nvidia_modulus-0.1.0-py3-none-any.whl.zip` & `tmp/nvidia_modulus-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,94 +1,132 @@
-Zip file size: 167408 bytes, number of entries: 92
--rw-r--r--  2.0 unx      847 b- defN 23-Apr-19 05:45 modulus/__init__.py
--rw-r--r--  2.0 unx     1307 b- defN 23-Apr-19 05:45 modulus/constants.py
--rw-r--r--  2.0 unx      622 b- defN 23-Apr-19 05:45 modulus/datapipes/__init__.py
--rw-r--r--  2.0 unx     2094 b- defN 23-Apr-19 05:45 modulus/datapipes/datapipe.py
--rw-r--r--  2.0 unx      961 b- defN 23-Apr-19 05:45 modulus/datapipes/meta.py
--rw-r--r--  2.0 unx      622 b- defN 23-Apr-19 05:45 modulus/datapipes/benchmarks/__init__.py
--rw-r--r--  2.0 unx    11694 b- defN 23-Apr-19 05:45 modulus/datapipes/benchmarks/darcy.py
--rw-r--r--  2.0 unx    16751 b- defN 23-Apr-19 05:45 modulus/datapipes/benchmarks/kelvin_helmholtz.py
--rw-r--r--  2.0 unx      622 b- defN 23-Apr-19 05:45 modulus/datapipes/benchmarks/kernels/__init__.py
--rw-r--r--  2.0 unx     4330 b- defN 23-Apr-19 05:45 modulus/datapipes/benchmarks/kernels/finite_difference.py
--rw-r--r--  2.0 unx    20542 b- defN 23-Apr-19 05:45 modulus/datapipes/benchmarks/kernels/finite_volume.py
--rw-r--r--  2.0 unx     3657 b- defN 23-Apr-19 05:45 modulus/datapipes/benchmarks/kernels/indexing.py
--rw-r--r--  2.0 unx     2054 b- defN 23-Apr-19 05:45 modulus/datapipes/benchmarks/kernels/initialization.py
--rw-r--r--  2.0 unx     4246 b- defN 23-Apr-19 05:45 modulus/datapipes/benchmarks/kernels/utils.py
--rw-r--r--  2.0 unx      663 b- defN 23-Apr-19 05:45 modulus/datapipes/climate/__init__.py
--rw-r--r--  2.0 unx    14986 b- defN 23-Apr-19 05:45 modulus/datapipes/climate/era5_hdf5.py
--rw-r--r--  2.0 unx      622 b- defN 23-Apr-19 05:45 modulus/datapipes/climate/era5_netcdf.py
--rw-r--r--  2.0 unx    15725 b- defN 23-Apr-19 05:45 modulus/datapipes/gnn/mgn_dataset.py
--rw-r--r--  2.0 unx      684 b- defN 23-Apr-19 05:45 modulus/deploy/onnx/__init__.py
--rw-r--r--  2.0 unx     4662 b- defN 23-Apr-19 05:45 modulus/deploy/onnx/utils.py
--rw-r--r--  2.0 unx      622 b- defN 23-Apr-19 05:45 modulus/deploy/triton/__init__.py
--rw-r--r--  2.0 unx      622 b- defN 23-Apr-19 05:45 modulus/deploy/trt/__init__.py
--rw-r--r--  2.0 unx      695 b- defN 23-Apr-19 05:45 modulus/distributed/__init__.py
--rw-r--r--  2.0 unx    13520 b- defN 23-Apr-19 05:45 modulus/distributed/manager.py
--rw-r--r--  2.0 unx     7075 b- defN 23-Apr-19 05:45 modulus/distributed/utils.py
--rw-r--r--  2.0 unx      622 b- defN 23-Apr-19 05:45 modulus/metrics/__init__.py
--rw-r--r--  2.0 unx      622 b- defN 23-Apr-19 05:45 modulus/metrics/climate/__init__.py
--rw-r--r--  2.0 unx     2716 b- defN 23-Apr-19 05:45 modulus/metrics/climate/acc.py
--rw-r--r--  2.0 unx     3294 b- defN 23-Apr-19 05:45 modulus/metrics/climate/efi.py
--rw-r--r--  2.0 unx     5464 b- defN 23-Apr-19 05:45 modulus/metrics/climate/reduction.py
--rw-r--r--  2.0 unx      622 b- defN 23-Apr-19 05:45 modulus/metrics/general/__init__.py
--rw-r--r--  2.0 unx     4832 b- defN 23-Apr-19 05:45 modulus/metrics/general/calibration.py
--rw-r--r--  2.0 unx     7740 b- defN 23-Apr-19 05:45 modulus/metrics/general/crps.py
--rw-r--r--  2.0 unx    12394 b- defN 23-Apr-19 05:45 modulus/metrics/general/ensemble_metrics.py
--rw-r--r--  2.0 unx     4615 b- defN 23-Apr-19 05:45 modulus/metrics/general/entropy.py
--rw-r--r--  2.0 unx    27154 b- defN 23-Apr-19 05:45 modulus/metrics/general/histogram.py
--rw-r--r--  2.0 unx     1856 b- defN 23-Apr-19 05:45 modulus/metrics/general/mse.py
--rw-r--r--  2.0 unx     4180 b- defN 23-Apr-19 05:45 modulus/metrics/general/reduction.py
--rw-r--r--  2.0 unx     1782 b- defN 23-Apr-19 05:45 modulus/metrics/general/wasserstein.py
--rw-r--r--  2.0 unx      650 b- defN 23-Apr-19 05:45 modulus/models/__init__.py
--rw-r--r--  2.0 unx     1575 b- defN 23-Apr-19 05:45 modulus/models/meta.py
--rw-r--r--  2.0 unx     4347 b- defN 23-Apr-19 05:45 modulus/models/module.py
--rw-r--r--  2.0 unx      646 b- defN 23-Apr-19 05:45 modulus/models/afno/__init__.py
--rw-r--r--  2.0 unx    17591 b- defN 23-Apr-19 05:45 modulus/models/afno/afno.py
--rw-r--r--  2.0 unx      683 b- defN 23-Apr-19 05:45 modulus/models/afno/distributed/__init__.py
--rw-r--r--  2.0 unx    11892 b- defN 23-Apr-19 05:45 modulus/models/afno/distributed/afno.py
--rw-r--r--  2.0 unx    14740 b- defN 23-Apr-19 05:45 modulus/models/afno/distributed/layers.py
--rw-r--r--  2.0 unx     4836 b- defN 23-Apr-19 05:45 modulus/models/afno/distributed/mappings.py
--rw-r--r--  2.0 unx      644 b- defN 23-Apr-19 05:45 modulus/models/fno/__init__.py
--rw-r--r--  2.0 unx    21685 b- defN 23-Apr-19 05:45 modulus/models/fno/fno.py
--rw-r--r--  2.0 unx      622 b- defN 23-Apr-19 05:45 modulus/models/graphcast/__init__.py
--rw-r--r--  2.0 unx    11312 b- defN 23-Apr-19 05:45 modulus/models/graphcast/decoder.py
--rw-r--r--  2.0 unx     8172 b- defN 23-Apr-19 05:45 modulus/models/graphcast/edge_block.py
--rw-r--r--  2.0 unx     5993 b- defN 23-Apr-19 05:45 modulus/models/graphcast/embedder.py
--rw-r--r--  2.0 unx    12765 b- defN 23-Apr-19 05:45 modulus/models/graphcast/encoder.py
--rw-r--r--  2.0 unx    23341 b- defN 23-Apr-19 05:45 modulus/models/graphcast/graph_cast_net.py
--rw-r--r--  2.0 unx    14887 b- defN 23-Apr-19 05:45 modulus/models/graphcast/mlp.py
--rw-r--r--  2.0 unx     4267 b- defN 23-Apr-19 05:45 modulus/models/graphcast/node_block.py
--rw-r--r--  2.0 unx     7048 b- defN 23-Apr-19 05:45 modulus/models/graphcast/processor.py
--rw-r--r--  2.0 unx    12076 b- defN 23-Apr-19 05:45 modulus/models/graphcast/utils.py
--rw-r--r--  2.0 unx      882 b- defN 23-Apr-19 05:45 modulus/models/layers/__init__.py
--rw-r--r--  2.0 unx     2773 b- defN 23-Apr-19 05:45 modulus/models/layers/activations.py
--rw-r--r--  2.0 unx    17497 b- defN 23-Apr-19 05:45 modulus/models/layers/fft.py
--rw-r--r--  2.0 unx     7621 b- defN 23-Apr-19 05:45 modulus/models/layers/fully_connected_layers.py
--rw-r--r--  2.0 unx     7692 b- defN 23-Apr-19 05:45 modulus/models/layers/fused_silu.py
--rw-r--r--  2.0 unx    10000 b- defN 23-Apr-19 05:45 modulus/models/layers/spectral_layers.py
--rw-r--r--  2.0 unx     2461 b- defN 23-Apr-19 05:45 modulus/models/layers/weight_norm.py
--rw-r--r--  2.0 unx      662 b- defN 23-Apr-19 05:45 modulus/models/meshgraphnet/__init__.py
--rw-r--r--  2.0 unx    12254 b- defN 23-Apr-19 05:45 modulus/models/meshgraphnet/meshgraphnet.py
--rw-r--r--  2.0 unx      667 b- defN 23-Apr-19 05:45 modulus/models/mlp/__init__.py
--rw-r--r--  2.0 unx     4220 b- defN 23-Apr-19 05:45 modulus/models/mlp/fully_connected.py
--rw-r--r--  2.0 unx      652 b- defN 23-Apr-19 05:45 modulus/models/pix2pix/__init__.py
--rw-r--r--  2.0 unx    11904 b- defN 23-Apr-19 05:45 modulus/models/pix2pix/pix2pix.py
--rw-r--r--  2.0 unx      697 b- defN 23-Apr-19 05:45 modulus/models/rnn/__init__.py
--rw-r--r--  2.0 unx    16096 b- defN 23-Apr-19 05:45 modulus/models/rnn/layers.py
--rw-r--r--  2.0 unx     8241 b- defN 23-Apr-19 05:45 modulus/models/rnn/rnn_one2many.py
--rw-r--r--  2.0 unx     8556 b- defN 23-Apr-19 05:45 modulus/models/rnn/rnn_seq2seq.py
--rw-r--r--  2.0 unx      659 b- defN 23-Apr-19 05:45 modulus/models/srrn/__init__.py
--rw-r--r--  2.0 unx    11964 b- defN 23-Apr-19 05:45 modulus/models/srrn/super_res_net.py
--rw-r--r--  2.0 unx      695 b- defN 23-Apr-19 05:45 modulus/utils/__init__.py
--rw-r--r--  2.0 unx    14380 b- defN 23-Apr-19 05:45 modulus/utils/capture.py
--rw-r--r--  2.0 unx      622 b- defN 23-Apr-19 05:45 modulus/utils/graphcast/__init__.py
--rw-r--r--  2.0 unx     4015 b- defN 23-Apr-19 05:45 modulus/utils/graphcast/data_utils.py
--rw-r--r--  2.0 unx     8857 b- defN 23-Apr-19 05:45 modulus/utils/graphcast/graph.py
--rw-r--r--  2.0 unx    11234 b- defN 23-Apr-19 05:45 modulus/utils/graphcast/graph_utils.py
--rw-r--r--  2.0 unx     1996 b- defN 23-Apr-19 05:45 modulus/utils/graphcast/icospheres.py
--rw-r--r--  2.0 unx     3427 b- defN 23-Apr-19 05:45 modulus/utils/graphcast/loss.py
--rw-r--r--  2.0 unx    11314 b- defN 23-Apr-19 18:12 nvidia_modulus-0.1.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     2724 b- defN 23-Apr-19 18:12 nvidia_modulus-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-19 18:12 nvidia_modulus-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-19 18:12 nvidia_modulus-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     8409 b- defN 23-Apr-19 18:12 nvidia_modulus-0.1.0.dist-info/RECORD
-92 files, 581161 bytes uncompressed, 153944 bytes compressed:  73.5%
+Zip file size: 266065 bytes, number of entries: 130
+-rw-r--r--  2.0 unx      847 b- defN 23-Aug-01 00:17 modulus/__init__.py
+-rw-r--r--  2.0 unx     1307 b- defN 23-Jul-27 23:18 modulus/constants.py
+-rw-r--r--  2.0 unx      622 b- defN 23-Jul-27 23:18 modulus/datapipes/__init__.py
+-rw-r--r--  2.0 unx     2094 b- defN 23-Jul-27 23:18 modulus/datapipes/datapipe.py
+-rw-r--r--  2.0 unx      961 b- defN 23-Jul-27 23:18 modulus/datapipes/meta.py
+-rw-r--r--  2.0 unx      622 b- defN 23-Jul-27 23:18 modulus/datapipes/benchmarks/__init__.py
+-rw-r--r--  2.0 unx    11694 b- defN 23-Jul-27 23:18 modulus/datapipes/benchmarks/darcy.py
+-rw-r--r--  2.0 unx    16751 b- defN 23-Jul-27 23:18 modulus/datapipes/benchmarks/kelvin_helmholtz.py
+-rw-r--r--  2.0 unx      622 b- defN 23-Jul-27 23:18 modulus/datapipes/benchmarks/kernels/__init__.py
+-rw-r--r--  2.0 unx     4330 b- defN 23-Jul-27 23:18 modulus/datapipes/benchmarks/kernels/finite_difference.py
+-rw-r--r--  2.0 unx    20542 b- defN 23-Jul-27 23:18 modulus/datapipes/benchmarks/kernels/finite_volume.py
+-rw-r--r--  2.0 unx     3657 b- defN 23-Jul-27 23:18 modulus/datapipes/benchmarks/kernels/indexing.py
+-rw-r--r--  2.0 unx     2054 b- defN 23-Jul-27 23:18 modulus/datapipes/benchmarks/kernels/initialization.py
+-rw-r--r--  2.0 unx     4246 b- defN 23-Jul-27 23:18 modulus/datapipes/benchmarks/kernels/utils.py
+-rw-r--r--  2.0 unx      663 b- defN 23-Jul-27 23:18 modulus/datapipes/climate/__init__.py
+-rw-r--r--  2.0 unx    14986 b- defN 23-Jul-27 23:18 modulus/datapipes/climate/era5_hdf5.py
+-rw-r--r--  2.0 unx      622 b- defN 23-Jul-27 23:18 modulus/datapipes/climate/era5_netcdf.py
+-rw-r--r--  2.0 unx     5960 b- defN 23-Jul-28 16:26 modulus/datapipes/climate/sfno/dataloader.py
+-rw-r--r--  2.0 unx    23148 b- defN 23-Aug-01 00:17 modulus/datapipes/climate/sfno/dataloaders/dali_es_helper_2d.py
+-rw-r--r--  2.0 unx    16186 b- defN 23-Aug-01 00:17 modulus/datapipes/climate/sfno/dataloaders/data_loader_dali_2d.py
+-rw-r--r--  2.0 unx     8648 b- defN 23-Jul-28 16:26 modulus/datapipes/climate/sfno/dataloaders/data_loader_dummy.py
+-rw-r--r--  2.0 unx     5338 b- defN 23-Jul-28 16:26 modulus/datapipes/climate/sfno/dataloaders/data_loader_multifiles.py
+-rw-r--r--  2.0 unx     5712 b- defN 23-Jul-27 23:18 modulus/datapipes/climate/sfno/dataloaders/zarr_helper.py
+-rw-r--r--  2.0 unx      622 b- defN 23-Aug-01 00:17 modulus/datapipes/gnn/__init__.py
+-rw-r--r--  2.0 unx    26225 b- defN 23-Jul-27 23:18 modulus/datapipes/gnn/ahmed_body_dataset.py
+-rw-r--r--  2.0 unx     2554 b- defN 23-Jul-27 23:18 modulus/datapipes/gnn/utils.py
+-rw-r--r--  2.0 unx    15363 b- defN 23-Aug-01 00:17 modulus/datapipes/gnn/vortex_shedding_dataset.py
+-rw-r--r--  2.0 unx      622 b- defN 23-Jul-27 23:18 modulus/deploy/__init__.py
+-rw-r--r--  2.0 unx      684 b- defN 23-Jul-27 23:18 modulus/deploy/onnx/__init__.py
+-rw-r--r--  2.0 unx     4662 b- defN 23-Jul-27 23:18 modulus/deploy/onnx/utils.py
+-rw-r--r--  2.0 unx      622 b- defN 23-Jul-27 23:18 modulus/deploy/triton/__init__.py
+-rw-r--r--  2.0 unx      622 b- defN 23-Jul-27 23:18 modulus/deploy/trt/__init__.py
+-rw-r--r--  2.0 unx      695 b- defN 23-Jul-27 23:18 modulus/distributed/__init__.py
+-rw-r--r--  2.0 unx    13549 b- defN 23-Jul-27 23:18 modulus/distributed/manager.py
+-rw-r--r--  2.0 unx     7075 b- defN 23-Jul-27 23:18 modulus/distributed/utils.py
+-rw-r--r--  2.0 unx      622 b- defN 23-Jul-27 23:18 modulus/metrics/__init__.py
+-rw-r--r--  2.0 unx      622 b- defN 23-Jul-27 23:18 modulus/metrics/climate/__init__.py
+-rw-r--r--  2.0 unx     2716 b- defN 23-Jul-27 23:18 modulus/metrics/climate/acc.py
+-rw-r--r--  2.0 unx     3294 b- defN 23-Jul-27 23:18 modulus/metrics/climate/efi.py
+-rw-r--r--  2.0 unx     5464 b- defN 23-Jul-27 23:18 modulus/metrics/climate/reduction.py
+-rw-r--r--  2.0 unx      622 b- defN 23-Jul-27 23:18 modulus/metrics/general/__init__.py
+-rw-r--r--  2.0 unx     4832 b- defN 23-Jul-27 23:18 modulus/metrics/general/calibration.py
+-rw-r--r--  2.0 unx     7892 b- defN 23-Jul-27 23:18 modulus/metrics/general/crps.py
+-rw-r--r--  2.0 unx    13435 b- defN 23-Jul-27 23:18 modulus/metrics/general/ensemble_metrics.py
+-rw-r--r--  2.0 unx     4615 b- defN 23-Jul-27 23:18 modulus/metrics/general/entropy.py
+-rw-r--r--  2.0 unx    27154 b- defN 23-Jul-27 23:18 modulus/metrics/general/histogram.py
+-rw-r--r--  2.0 unx     1856 b- defN 23-Jul-27 23:18 modulus/metrics/general/mse.py
+-rw-r--r--  2.0 unx     4180 b- defN 23-Jul-27 23:18 modulus/metrics/general/reduction.py
+-rw-r--r--  2.0 unx     1782 b- defN 23-Jul-27 23:18 modulus/metrics/general/wasserstein.py
+-rw-r--r--  2.0 unx      650 b- defN 23-Jul-27 23:18 modulus/models/__init__.py
+-rw-r--r--  2.0 unx     9704 b- defN 23-Jul-27 23:18 modulus/models/fcn_mip_plugin.py
+-rw-r--r--  2.0 unx     1574 b- defN 23-Jul-27 23:18 modulus/models/meta.py
+-rw-r--r--  2.0 unx     4347 b- defN 23-Jul-27 23:18 modulus/models/module.py
+-rw-r--r--  2.0 unx      646 b- defN 23-Jul-27 23:18 modulus/models/afno/__init__.py
+-rw-r--r--  2.0 unx    17591 b- defN 23-Jul-27 23:18 modulus/models/afno/afno.py
+-rw-r--r--  2.0 unx      683 b- defN 23-Jul-27 23:18 modulus/models/afno/distributed/__init__.py
+-rw-r--r--  2.0 unx    11892 b- defN 23-Jul-27 23:18 modulus/models/afno/distributed/afno.py
+-rw-r--r--  2.0 unx    14740 b- defN 23-Jul-27 23:18 modulus/models/afno/distributed/layers.py
+-rw-r--r--  2.0 unx     4836 b- defN 23-Jul-27 23:18 modulus/models/afno/distributed/mappings.py
+-rw-r--r--  2.0 unx      646 b- defN 23-Jul-27 23:18 modulus/models/dlwp/__init__.py
+-rw-r--r--  2.0 unx    13279 b- defN 23-Jul-27 23:18 modulus/models/dlwp/dlwp.py
+-rw-r--r--  2.0 unx      644 b- defN 23-Jul-27 23:18 modulus/models/fno/__init__.py
+-rw-r--r--  2.0 unx    28001 b- defN 23-Jul-27 23:18 modulus/models/fno/fno.py
+-rw-r--r--  2.0 unx      622 b- defN 23-Jul-27 23:18 modulus/models/gnn_layers/__init__.py
+-rw-r--r--  2.0 unx     6076 b- defN 23-Jul-27 23:18 modulus/models/gnn_layers/embedder.py
+-rw-r--r--  2.0 unx     3097 b- defN 23-Jul-27 23:18 modulus/models/gnn_layers/mesh_edge_block.py
+-rw-r--r--  2.0 unx     4495 b- defN 23-Jul-27 23:18 modulus/models/gnn_layers/mesh_graph_decoder.py
+-rw-r--r--  2.0 unx     5264 b- defN 23-Jul-27 23:18 modulus/models/gnn_layers/mesh_graph_encoder.py
+-rw-r--r--  2.0 unx    14522 b- defN 23-Jul-27 23:18 modulus/models/gnn_layers/mesh_graph_mlp.py
+-rw-r--r--  2.0 unx     3154 b- defN 23-Jul-27 23:18 modulus/models/gnn_layers/mesh_node_block.py
+-rw-r--r--  2.0 unx    16058 b- defN 23-Jul-27 23:18 modulus/models/gnn_layers/utils.py
+-rw-r--r--  2.0 unx      622 b- defN 23-Jul-27 23:18 modulus/models/graphcast/__init__.py
+-rw-r--r--  2.0 unx    23208 b- defN 23-Jul-27 23:18 modulus/models/graphcast/graph_cast_net.py
+-rw-r--r--  2.0 unx     6032 b- defN 23-Jul-27 23:18 modulus/models/graphcast/graph_cast_processor.py
+-rw-r--r--  2.0 unx      983 b- defN 23-Jul-27 23:18 modulus/models/layers/__init__.py
+-rw-r--r--  2.0 unx     2773 b- defN 23-Jul-27 23:18 modulus/models/layers/activations.py
+-rw-r--r--  2.0 unx    17495 b- defN 23-Jul-27 23:18 modulus/models/layers/fft.py
+-rw-r--r--  2.0 unx     9987 b- defN 23-Jul-27 23:18 modulus/models/layers/fully_connected_layers.py
+-rw-r--r--  2.0 unx     7685 b- defN 23-Jul-27 23:18 modulus/models/layers/fused_silu.py
+-rw-r--r--  2.0 unx    17575 b- defN 23-Jul-27 23:18 modulus/models/layers/spectral_layers.py
+-rw-r--r--  2.0 unx     2461 b- defN 23-Jul-27 23:18 modulus/models/layers/weight_norm.py
+-rw-r--r--  2.0 unx      662 b- defN 23-Jul-27 23:18 modulus/models/meshgraphnet/__init__.py
+-rw-r--r--  2.0 unx    11221 b- defN 23-Jul-27 23:18 modulus/models/meshgraphnet/meshgraphnet.py
+-rw-r--r--  2.0 unx      667 b- defN 23-Jul-27 23:18 modulus/models/mlp/__init__.py
+-rw-r--r--  2.0 unx     4220 b- defN 23-Jul-27 23:18 modulus/models/mlp/fully_connected.py
+-rw-r--r--  2.0 unx      652 b- defN 23-Jul-27 23:18 modulus/models/pix2pix/__init__.py
+-rw-r--r--  2.0 unx    11904 b- defN 23-Jul-27 23:18 modulus/models/pix2pix/pix2pix.py
+-rw-r--r--  2.0 unx      697 b- defN 23-Jul-27 23:18 modulus/models/rnn/__init__.py
+-rw-r--r--  2.0 unx    16096 b- defN 23-Jul-27 23:18 modulus/models/rnn/layers.py
+-rw-r--r--  2.0 unx     8239 b- defN 23-Jul-27 23:18 modulus/models/rnn/rnn_one2many.py
+-rw-r--r--  2.0 unx     8554 b- defN 23-Jul-27 23:18 modulus/models/rnn/rnn_seq2seq.py
+-rw-r--r--  2.0 unx     4310 b- defN 23-Jul-28 16:26 modulus/models/sfno/activations.py
+-rw-r--r--  2.0 unx     7735 b- defN 23-Jul-28 16:26 modulus/models/sfno/contractions.py
+-rw-r--r--  2.0 unx     8862 b- defN 23-Aug-01 00:17 modulus/models/sfno/factorizations.py
+-rw-r--r--  2.0 unx     2869 b- defN 23-Jul-28 16:26 modulus/models/sfno/initialization.py
+-rw-r--r--  2.0 unx    17464 b- defN 23-Jul-28 16:26 modulus/models/sfno/layers.py
+-rw-r--r--  2.0 unx    19226 b- defN 23-Jul-28 16:26 modulus/models/sfno/preprocessor.py
+-rw-r--r--  2.0 unx    12499 b- defN 23-Jul-28 16:26 modulus/models/sfno/s2convolutions.py
+-rw-r--r--  2.0 unx    35279 b- defN 23-Jul-28 16:26 modulus/models/sfno/sfnonet.py
+-rw-r--r--  2.0 unx      659 b- defN 23-Jul-27 23:18 modulus/models/srrn/__init__.py
+-rw-r--r--  2.0 unx    11962 b- defN 23-Jul-27 23:18 modulus/models/srrn/super_res_net.py
+-rw-r--r--  2.0 unx      708 b- defN 23-Jul-27 23:18 modulus/utils/__init__.py
+-rw-r--r--  2.0 unx    17338 b- defN 23-Aug-01 00:17 modulus/utils/capture.py
+-rw-r--r--  2.0 unx     3080 b- defN 23-Jul-27 23:18 modulus/utils/filesystem.py
+-rw-r--r--  2.0 unx      622 b- defN 23-Jul-27 23:18 modulus/utils/graphcast/__init__.py
+-rw-r--r--  2.0 unx     4015 b- defN 23-Jul-27 23:18 modulus/utils/graphcast/data_utils.py
+-rw-r--r--  2.0 unx     9607 b- defN 23-Jul-27 23:18 modulus/utils/graphcast/graph.py
+-rw-r--r--  2.0 unx    11234 b- defN 23-Jul-27 23:18 modulus/utils/graphcast/graph_utils.py
+-rw-r--r--  2.0 unx     2086 b- defN 23-Jul-27 23:18 modulus/utils/graphcast/icospheres.py
+-rw-r--r--  2.0 unx     3427 b- defN 23-Jul-27 23:18 modulus/utils/graphcast/loss.py
+-rw-r--r--  2.0 unx     3387 b- defN 23-Jul-27 23:18 modulus/utils/sfno/YParams.py
+-rw-r--r--  2.0 unx     4383 b- defN 23-Jul-27 23:18 modulus/utils/sfno/img_utils.py
+-rw-r--r--  2.0 unx     2343 b- defN 23-Jul-28 16:26 modulus/utils/sfno/logging_utils.py
+-rw-r--r--  2.0 unx    15733 b- defN 23-Jul-28 16:26 modulus/utils/sfno/loss.py
+-rw-r--r--  2.0 unx    14659 b- defN 23-Jul-28 16:26 modulus/utils/sfno/metric.py
+-rw-r--r--  2.0 unx     3508 b- defN 23-Jul-28 16:26 modulus/utils/sfno/warmup_scheduler.py
+-rw-r--r--  2.0 unx     8751 b- defN 23-Jul-28 16:26 modulus/utils/sfno/zenith_angle.py
+-rw-r--r--  2.0 unx      622 b- defN 23-Jul-27 23:18 modulus/utils/sfno/distributed/__init__.py
+-rw-r--r--  2.0 unx    12297 b- defN 23-Jul-28 16:26 modulus/utils/sfno/distributed/comm.py
+-rw-r--r--  2.0 unx     8524 b- defN 23-Jul-28 16:26 modulus/utils/sfno/distributed/helpers.py
+-rw-r--r--  2.0 unx     5135 b- defN 23-Jul-28 16:26 modulus/utils/sfno/distributed/layer_norm.py
+-rw-r--r--  2.0 unx    23004 b- defN 23-Jul-28 16:26 modulus/utils/sfno/distributed/layers.py
+-rw-r--r--  2.0 unx     9338 b- defN 23-Jul-28 16:26 modulus/utils/sfno/distributed/mappings.py
+-rw-r--r--  2.0 unx     9653 b- defN 23-Jul-28 16:26 modulus/utils/sfno/metrics/weighted_acc_rmse.py
+-rw-r--r--  2.0 unx     8932 b- defN 23-Jul-27 23:18 modulus/utils/sfno/metrics/weighted_acc_rmse_inf.py
+-rw-r--r--  2.0 unx    11314 b- defN 23-Aug-01 00:19 nvidia_modulus-0.2.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     5582 b- defN 23-Aug-01 00:19 nvidia_modulus-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-01 00:19 nvidia_modulus-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Aug-01 00:19 nvidia_modulus-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    12139 b- defN 23-Aug-01 00:19 nvidia_modulus-0.2.0.dist-info/RECORD
+130 files, 950633 bytes uncompressed, 246595 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -45,15 +45,45 @@
 
 Filename: modulus/datapipes/climate/era5_hdf5.py
 Comment: 
 
 Filename: modulus/datapipes/climate/era5_netcdf.py
 Comment: 
 
-Filename: modulus/datapipes/gnn/mgn_dataset.py
+Filename: modulus/datapipes/climate/sfno/dataloader.py
+Comment: 
+
+Filename: modulus/datapipes/climate/sfno/dataloaders/dali_es_helper_2d.py
+Comment: 
+
+Filename: modulus/datapipes/climate/sfno/dataloaders/data_loader_dali_2d.py
+Comment: 
+
+Filename: modulus/datapipes/climate/sfno/dataloaders/data_loader_dummy.py
+Comment: 
+
+Filename: modulus/datapipes/climate/sfno/dataloaders/data_loader_multifiles.py
+Comment: 
+
+Filename: modulus/datapipes/climate/sfno/dataloaders/zarr_helper.py
+Comment: 
+
+Filename: modulus/datapipes/gnn/__init__.py
+Comment: 
+
+Filename: modulus/datapipes/gnn/ahmed_body_dataset.py
+Comment: 
+
+Filename: modulus/datapipes/gnn/utils.py
+Comment: 
+
+Filename: modulus/datapipes/gnn/vortex_shedding_dataset.py
+Comment: 
+
+Filename: modulus/deploy/__init__.py
 Comment: 
 
 Filename: modulus/deploy/onnx/__init__.py
 Comment: 
 
 Filename: modulus/deploy/onnx/utils.py
 Comment: 
@@ -114,14 +144,17 @@
 
 Filename: modulus/metrics/general/wasserstein.py
 Comment: 
 
 Filename: modulus/models/__init__.py
 Comment: 
 
+Filename: modulus/models/fcn_mip_plugin.py
+Comment: 
+
 Filename: modulus/models/meta.py
 Comment: 
 
 Filename: modulus/models/module.py
 Comment: 
 
 Filename: modulus/models/afno/__init__.py
@@ -138,48 +171,57 @@
 
 Filename: modulus/models/afno/distributed/layers.py
 Comment: 
 
 Filename: modulus/models/afno/distributed/mappings.py
 Comment: 
 
+Filename: modulus/models/dlwp/__init__.py
+Comment: 
+
+Filename: modulus/models/dlwp/dlwp.py
+Comment: 
+
 Filename: modulus/models/fno/__init__.py
 Comment: 
 
 Filename: modulus/models/fno/fno.py
 Comment: 
 
-Filename: modulus/models/graphcast/__init__.py
+Filename: modulus/models/gnn_layers/__init__.py
 Comment: 
 
-Filename: modulus/models/graphcast/decoder.py
+Filename: modulus/models/gnn_layers/embedder.py
 Comment: 
 
-Filename: modulus/models/graphcast/edge_block.py
+Filename: modulus/models/gnn_layers/mesh_edge_block.py
 Comment: 
 
-Filename: modulus/models/graphcast/embedder.py
+Filename: modulus/models/gnn_layers/mesh_graph_decoder.py
 Comment: 
 
-Filename: modulus/models/graphcast/encoder.py
+Filename: modulus/models/gnn_layers/mesh_graph_encoder.py
 Comment: 
 
-Filename: modulus/models/graphcast/graph_cast_net.py
+Filename: modulus/models/gnn_layers/mesh_graph_mlp.py
+Comment: 
+
+Filename: modulus/models/gnn_layers/mesh_node_block.py
 Comment: 
 
-Filename: modulus/models/graphcast/mlp.py
+Filename: modulus/models/gnn_layers/utils.py
 Comment: 
 
-Filename: modulus/models/graphcast/node_block.py
+Filename: modulus/models/graphcast/__init__.py
 Comment: 
 
-Filename: modulus/models/graphcast/processor.py
+Filename: modulus/models/graphcast/graph_cast_net.py
 Comment: 
 
-Filename: modulus/models/graphcast/utils.py
+Filename: modulus/models/graphcast/graph_cast_processor.py
 Comment: 
 
 Filename: modulus/models/layers/__init__.py
 Comment: 
 
 Filename: modulus/models/layers/activations.py
 Comment: 
@@ -225,26 +267,53 @@
 
 Filename: modulus/models/rnn/rnn_one2many.py
 Comment: 
 
 Filename: modulus/models/rnn/rnn_seq2seq.py
 Comment: 
 
+Filename: modulus/models/sfno/activations.py
+Comment: 
+
+Filename: modulus/models/sfno/contractions.py
+Comment: 
+
+Filename: modulus/models/sfno/factorizations.py
+Comment: 
+
+Filename: modulus/models/sfno/initialization.py
+Comment: 
+
+Filename: modulus/models/sfno/layers.py
+Comment: 
+
+Filename: modulus/models/sfno/preprocessor.py
+Comment: 
+
+Filename: modulus/models/sfno/s2convolutions.py
+Comment: 
+
+Filename: modulus/models/sfno/sfnonet.py
+Comment: 
+
 Filename: modulus/models/srrn/__init__.py
 Comment: 
 
 Filename: modulus/models/srrn/super_res_net.py
 Comment: 
 
 Filename: modulus/utils/__init__.py
 Comment: 
 
 Filename: modulus/utils/capture.py
 Comment: 
 
+Filename: modulus/utils/filesystem.py
+Comment: 
+
 Filename: modulus/utils/graphcast/__init__.py
 Comment: 
 
 Filename: modulus/utils/graphcast/data_utils.py
 Comment: 
 
 Filename: modulus/utils/graphcast/graph.py
@@ -255,23 +324,68 @@
 
 Filename: modulus/utils/graphcast/icospheres.py
 Comment: 
 
 Filename: modulus/utils/graphcast/loss.py
 Comment: 
 
-Filename: nvidia_modulus-0.1.0.dist-info/LICENSE.txt
+Filename: modulus/utils/sfno/YParams.py
+Comment: 
+
+Filename: modulus/utils/sfno/img_utils.py
+Comment: 
+
+Filename: modulus/utils/sfno/logging_utils.py
+Comment: 
+
+Filename: modulus/utils/sfno/loss.py
+Comment: 
+
+Filename: modulus/utils/sfno/metric.py
+Comment: 
+
+Filename: modulus/utils/sfno/warmup_scheduler.py
+Comment: 
+
+Filename: modulus/utils/sfno/zenith_angle.py
+Comment: 
+
+Filename: modulus/utils/sfno/distributed/__init__.py
+Comment: 
+
+Filename: modulus/utils/sfno/distributed/comm.py
+Comment: 
+
+Filename: modulus/utils/sfno/distributed/helpers.py
+Comment: 
+
+Filename: modulus/utils/sfno/distributed/layer_norm.py
+Comment: 
+
+Filename: modulus/utils/sfno/distributed/layers.py
+Comment: 
+
+Filename: modulus/utils/sfno/distributed/mappings.py
+Comment: 
+
+Filename: modulus/utils/sfno/metrics/weighted_acc_rmse.py
+Comment: 
+
+Filename: modulus/utils/sfno/metrics/weighted_acc_rmse_inf.py
+Comment: 
+
+Filename: nvidia_modulus-0.2.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: nvidia_modulus-0.1.0.dist-info/METADATA
+Filename: nvidia_modulus-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: nvidia_modulus-0.1.0.dist-info/WHEEL
+Filename: nvidia_modulus-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: nvidia_modulus-0.1.0.dist-info/top_level.txt
+Filename: nvidia_modulus-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: nvidia_modulus-0.1.0.dist-info/RECORD
+Filename: nvidia_modulus-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## modulus/__init__.py

```diff
@@ -15,8 +15,8 @@
 from .models.module import Module
 from .models.meta import ModelMetaData
 from .datapipes.datapipe import Datapipe
 from .datapipes.meta import DatapipeMetaData
 
 from .datapipes.datapipe import Datapipe
 
-__version__ = "0.1.0"
+__version__ = "0.2.0"
```

## modulus/distributed/manager.py

```diff
@@ -197,14 +197,15 @@
         """Setup method using generic initialization"""
         rank = int(os.environ.get("RANK"))
         world_size = int(os.environ.get("WORLD_SIZE"))
         if "LOCAL_RANK" in os.environ:
             local_rank = int(os.environ.get("LOCAL_RANK"))
         else:
             local_rank = rank % torch.cuda.device_count()
+        # Read env variables
         addr = os.environ.get("MASTER_ADDR")
         port = os.environ.get("MASTER_PORT")
 
         DistributedManager.setup(
             rank=rank,
             world_size=world_size,
             local_rank=local_rank,
```

## modulus/metrics/general/crps.py

```diff
@@ -24,17 +24,19 @@
     """Computes the local Continuous Ranked Probability Score (CRPS)
     using assuming that the forecast distribution is normal.
 
     Creates a map of CRPS and does not accumulate over lat/lon regions.
     Computes:
 
     .. math:
-        CRPS(mean, std, y) = std * [ \\frac{1}{\\pi} - 2 \\phi ( \\frac{x-mean}{std} ) -
+        CRPS(mean, std, y) = std * [ \\frac{1}{\\sqrt{\\pi}}} - 2 \\phi ( \\frac{x-mean}{std} ) -
                 ( \\frac{x-mean}{std} ) * (2 \\Phi(\\frac{x-mean}{std}) - 1) ]
 
+        where \\phi and \\Phi are the normal gaussian pdf/cdf respectively.
+
     Parameters
     ----------
     mean : Tensor
         Tensor of mean of forecast distribution.
     std : Tensor
         Tensor of standard deviation of forecast distribution.
     obs : Union[Tensor, np.ndarray]
@@ -65,17 +67,19 @@
         + " and "
         + str(obs.shape)
         + "."
     )
 
     d = (obs - mean) / std
     phi = torch.exp(-0.5 * d**2) / torch.sqrt(torch.as_tensor(2 * torch.pi))
+
+    # Note, simplified expression below is not exactly Gaussian CDF
     Phi = torch.erf(d / torch.sqrt(torch.as_tensor(2.0)))
 
-    return 2 * phi + (obs - mean) * Phi - std / torch.sqrt(torch.as_tensor(torch.pi))
+    return std * (2 * phi + d * Phi - 1.0 / torch.sqrt(torch.as_tensor(torch.pi)))
 
 
 def _crps_from_cdf(
     bin_edges: Tensor, cdf: Tensor, obs: Union[Tensor, np.ndarray]
 ) -> Tensor:
     """Computes the local Continuous Ranked Probability Score (CRPS)
     using a cumulative distribution function.
```

## modulus/metrics/general/ensemble_metrics.py

```diff
@@ -36,36 +36,36 @@
     dtype : torch.dtype, optional
         Standard dtype to initialize any tensor with
     """
 
     def __init__(
         self,
         input_shape: Union[Tuple[int, ...], List[int]],
-        device: torch.device = "cpu",
+        device: Union[str, torch.device] = "cpu",
         dtype: torch.dtype = torch.float32,
     ):
         super().__init__()
         self.input_shape = list(input_shape)
-        self.device = device
+        self.device = torch.device(device)
         self.dtype = dtype
 
         if DistributedManager.is_initialized() and not (dist.is_initialized()):
             warn(
                 "DistributedManager is detected and initialized but torch distributed \
     process group is not initialized. In order to use this class, please initialize \
     torch process group, see https://pytorch.org/docs/stable/distributed.html"
             )
 
-    def _check_shape(self, input: Tensor) -> None:
+    def _check_shape(self, inputs: Tensor) -> None:
         """
         Check input shapes for non-batched dimension.
         """
-        assert [i == s for (i, s) in zip(input.shape[1:], self.input_shape)], (
+        assert [i == s for (i, s) in zip(inputs.shape[1:], self.input_shape)], (
             "Expected new input to have compatible shape with existing shapes but got"
-            + str(input.shape)
+            + str(inputs.shape)
             + "and"
             + str(self.input_shape)
             + "."
         )
 
     def __call__(self, *args):
         """
@@ -85,15 +85,15 @@
         """
         raise NotImplementedError("Class member must implement a finalize method.")
 
 
 def _update_mean(
     old_sum: Tensor,
     old_n: Union[int, Tensor],
-    input: Tensor,
+    inputs: Tensor,
     batch_dim: Union[int, None] = 0,
 ) -> Tuple[Tensor, Union[int, Tensor]]:
     """Updated mean sufficient statistics given new data
 
     This method updates a running sum and number of samples with new (possibly batched)
     inputs
 
@@ -112,19 +112,19 @@
 
     Returns
     -------
     Tuple[Tensor, Union[int, Tensor]]
         Updated (rolling sum, number of samples)
     """
     if batch_dim is None:
-        input = torch.unsqueeze(input, 0)
+        inputs = torch.unsqueeze(inputs, 0)
         batch_dim = 0
 
-    new_sum = old_sum + torch.sum(input, dim=batch_dim)
-    new_n = old_n + input.shape[batch_dim]
+    new_sum = old_sum + torch.sum(inputs, dim=batch_dim)
+    new_n = old_n + inputs.shape[batch_dim]
 
     return new_sum, new_n
 
 
 class Mean(EnsembleMetrics):
     """Utility class that computes the mean over a batched or ensemble dimension
 
@@ -135,62 +135,79 @@
     input_shape : Union[Tuple, List]
         Shape of broadcasted dimensions
     """
 
     def __init__(self, input_shape: Union[Tuple, List], **kwargs):
         super().__init__(input_shape, **kwargs)
         self.sum = torch.zeros(self.input_shape, dtype=self.dtype, device=self.device)
-        self.n = torch.zeros(1, dtype=torch.int32, device=self.device)
+        self.n = torch.zeros([1], dtype=torch.int32, device=self.device)
 
-    def __call__(self, input: Tensor) -> Tensor:
+    def __call__(self, inputs: Tensor, dim: int = 0) -> Tensor:
         """Calculate an initial mean
 
         Parameters
         ----------
-        input : Tensor
+        inputs : Tensor
             Input data
+        dim : Int
+            Dimension of batched data
 
         Returns
         -------
         Tensor
             Mean value
         """
-        self.sum = torch.sum(input, dim=0)
-        self.n = torch.as_tensor(input.shape[0])
+        assert (
+            inputs.device == self.device
+        ), f"Input device, {inputs.device}, and Module device, {self.device}, must be the same."
+        self.sum = torch.sum(inputs, dim=dim)
+        self.n = torch.as_tensor([inputs.shape[dim]], device=self.device)
         # TODO(Dallas) Move distributed calls into finalize.
 
         if DistributedManager.is_initialized() and dist.is_initialized():
             dist.all_reduce(self.sum, op=dist.ReduceOp.SUM)
             dist.all_reduce(self.n, op=dist.ReduceOp.SUM)
 
         return self.sum / self.n
 
-    def update(self, input: Tensor) -> Tensor:
+    def update(self, inputs: Tensor, dim: int = 0) -> Tensor:
         """Update current mean and essential statistics with new data
 
         Parameters
         ----------
-        input : Tensor
-            Input tensor
+        inputs : Tensor
+            Inputs tensor
+        dim : int
+            Dimension of batched data
 
         Returns
         -------
         Tensor
             Current mean value
         """
-        self._check_shape(input)
+        self._check_shape(inputs)
+        assert (
+            inputs.device == self.device
+        ), f"Inputs device, {inputs.device}, and Module device, {self.device}, must be the same."
+
         # TODO(Dallas) Move distributed calls into finalize.
         if DistributedManager.is_initialized() and dist.is_initialized():
-            sums, n = _update_mean(self.sum, self.n, input, batch_dim=0)
+            # Collect local sums, n
+            sums = torch.sum(inputs, batch_dim=dim)
+            n = torch.as_tensor([inputs.shape[dim]], device=self.device)
+
+            # Reduce
             dist.all_reduce(sums, op=dist.ReduceOp.SUM)
             dist.all_reduce(n, op=dist.ReduceOp.SUM)
+
+            # Update
             self.sum += sums
             self.n += n
         else:
-            self.sum, self.n = _update_mean(self.sum, self.n, input, batch_dim=0)
+            self.sum, self.n = _update_mean(self.sum, self.n, inputs, batch_dim=dim)
         return self.sum / self.n
 
     def finalize(
         self,
     ) -> Tensor:
         """Compute and store final mean
 
@@ -204,15 +221,15 @@
         return self.mean
 
 
 def _update_var(
     old_sum: Tensor,
     old_sum2: Tensor,
     old_n: Union[int, Tensor],
-    input: Tensor,
+    inputs: Tensor,
     batch_dim: Union[int, None] = 0,
 ) -> Tuple[Tensor, Tensor, Union[int, Tensor]]:
     """Updated variance sufficient statistics given new data
 
     This method updates a running running sum, squared sum, and number of samples with
     new (possibly batched) inputs
 
@@ -220,15 +237,15 @@
     ----------
     old_sum : Tensor
         Current, or old, running sum
     old_sum2 : Tensor
         Current, or old, running squared sum
     old_n : Union[int, Tensor]
         Current, or old, number of samples
-    input : Tensor
+    inputs : Tensor
         New input to add to current/old sum. May be batched, in which case the batched
         dimension must be flagged by passing an int to batch_dim.
     batch_dim : Union[int, None], optional
         Whether the new inputs contain a batch of new inputs and what dimension they are
         stored along. Will reduce all elements if None, by default 0.
 
     Returns
@@ -241,20 +258,20 @@
     See "Updating Formulae and a Pairwise Algorithm for Computing Sample Variances"
     by Chan et al.
     http://i.stanford.edu/pub/cstr/reports/cs/tr/79/773/CS-TR-79-773.pdf
     for details.
     """
 
     if batch_dim is None:
-        input = torch.unsqueeze(input, 0)
+        inputs = torch.unsqueeze(inputs, 0)
         batch_dim = 0
 
-    temp_n = input.shape[batch_dim]
-    temp_sum = torch.sum(input, dim=batch_dim)
-    temp_sum2 = torch.sum((input - temp_sum / temp_n) ** 2, dim=batch_dim)
+    temp_n = inputs.shape[batch_dim]
+    temp_sum = torch.sum(inputs, dim=batch_dim)
+    temp_sum2 = torch.sum((inputs - temp_sum / temp_n) ** 2, dim=batch_dim)
 
     delta = old_sum * temp_n / old_n - temp_sum
 
     new_sum = old_sum + temp_sum
     new_sum2 = old_sum2 + temp_sum2
     new_sum2 += old_n / temp_n / (old_n + temp_n) * delta**2
     new_n = old_n + temp_n
@@ -278,64 +295,75 @@
     by Chan et al.
     http://i.stanford.edu/pub/cstr/reports/cs/tr/79/773/CS-TR-79-773.pdf
     for details.
     """
 
     def __init__(self, input_shape: Union[Tuple, List], **kwargs):
         super().__init__(input_shape, **kwargs)
-        self.n = torch.zeros(1, dtype=torch.int32, device=self.device)
+        self.n = torch.zeros([1], dtype=torch.int32, device=self.device)
         self.sum = torch.zeros(self.input_shape, dtype=self.dtype, device=self.device)
         self.sum2 = torch.zeros(self.input_shape, dtype=self.dtype, device=self.device)
 
-    def __call__(self, inputs: Tensor) -> Tensor:
+    def __call__(self, inputs: Tensor, dim: int = 0) -> Tensor:
         """Calculate an initial variance
 
         Parameters
         ----------
-        input : Tensor
+        inputs : Tensor
             Input data
+        dim : Int
+            Dimension of batched data
 
         Returns
         -------
         Tensor
             Unbiased variance values
         """
-        self.sum = torch.sum(inputs, dim=0)
-        self.n = torch.as_tensor(inputs.shape[0])
-        # TODO(Dallas) Move distributed calls into finalize.
+
+        assert (
+            inputs.device == self.device
+        ), f"Input device, {inputs.device}, and Module device, {self.device}, must be the same."
+        self.sum = torch.sum(inputs, dim=dim)
+        self.n = torch.as_tensor([inputs.shape[0]], device=self.device)
+
         if DistributedManager.is_initialized() and dist.is_initialized():
             # Compute mean and send around.
             dist.all_reduce(self.sum, op=dist.ReduceOp.SUM)
             dist.all_reduce(self.n, op=dist.ReduceOp.SUM)
 
-            self.sum2 = torch.sum((inputs - self.sum / self.n) ** 2, dim=0)
+            self.sum2 = torch.sum((inputs - self.sum / self.n) ** 2, dim=dim)
             dist.all_reduce(self.sum2, op=dist.ReduceOp.SUM)
         else:
-            self.sum2 = torch.sum((inputs - self.sum / self.n) ** 2, dim=0)
+            self.sum2 = torch.sum((inputs - self.sum / self.n) ** 2, dim=dim)
 
         if self.n < 2.0:
             return self.sum2
         else:
             return self.sum2 / (self.n - 1.0)
 
     def update(self, inputs: Tensor) -> Tensor:
         """Update current variance value and essential statistics with new data
 
         Parameters
         ----------
-        input : Tensor
+        inputs : Tensor
             Input data
 
         Returns
         -------
         Tensor
             Unbiased variance tensor
         """
+
         self._check_shape(inputs)
-        new_n = torch.as_tensor(inputs.shape[0])
+        assert (
+            inputs.device == self.device
+        ), f"Input device, {inputs.device}, and Module device, {self.device}, must be the same."
+
+        new_n = torch.as_tensor([inputs.shape[0]], device=self.device)
         new_sum = torch.sum(inputs, dim=0)
         # TODO(Dallas) Move distributed calls into finalize.
         if DistributedManager.is_initialized() and dist.is_initialized():
             dist.all_reduce(new_n, op=dist.ReduceOp.SUM)
             dist.all_reduce(new_sum, op=dist.ReduceOp.SUM)
             new_sum2 = torch.sum((inputs - new_sum / new_n) ** 2, dim=0)
             dist.all_reduce(new_sum2, op=dist.ReduceOp.SUM)
```

## modulus/models/meta.py

```diff
@@ -36,12 +36,11 @@
     trt: bool = False
     # Physics informed
     var_dim: int = -1
     func_torch: bool = False
     auto_grad: bool = False
 
     def __post_init__(self):
-
         self.amp_cpu = self.amp if self.amp_cpu is None else self.amp_cpu
         self.amp_gpu = self.amp if self.amp_gpu is None else self.amp_gpu
         self.onnx_cpu = self.onnx if self.onnx_cpu is None else self.onnx_cpu
         self.onnx_gpu = self.onnx if self.onnx_gpu is None else self.onnx_gpu
```

## modulus/models/fno/fno.py

```diff
@@ -183,15 +183,14 @@
         fno_layer_size: int = 32,
         num_fno_modes: Union[int, List[int]] = 16,
         padding: Union[int, List[int]] = 8,
         padding_type: str = "constant",
         activation_fn: nn.Module = nn.GELU(),
         coord_features: bool = True,
     ) -> None:
-
         super().__init__()
         self.in_channels = in_channels
         self.num_fno_layers = num_fno_layers
         self.fno_width = fno_layer_size
         self.coord_features = coord_features
         # Spectral modes to have weights
         if isinstance(num_fno_modes, int):
@@ -238,25 +237,25 @@
 
         if self.coord_features:
             coord_feat = self.meshgrid(list(x.shape), x.device)
             x = torch.cat((x, coord_feat), dim=1)
 
         x = self.lift_network(x)
         # (left, right, top, bottom)
-        x = F.pad(x, (0, self.pad[0], 0, self.pad[1]), mode=self.padding_type)
+        x = F.pad(x, (0, self.pad[1], 0, self.pad[0]), mode=self.padding_type)
         # Spectral layers
         for k, conv_w in enumerate(zip(self.conv_layers, self.spconv_layers)):
             conv, w = conv_w
             if k < len(self.conv_layers) - 1:
                 x = self.activation_fn(conv(x) + w(x))
             else:
                 x = conv(x) + w(x)
 
         # remove padding
-        x = x[..., : self.ipad[1], : self.ipad[0]]
+        x = x[..., : self.ipad[0], : self.ipad[1]]
 
         return x
 
     def meshgrid(self, shape: List[int], device: torch.device) -> Tensor:
         """Creates 2D meshgrid feature
 
         Parameters
@@ -374,26 +373,26 @@
             coord_feat = self.meshgrid(list(x.shape), x.device)
             x = torch.cat((x, coord_feat), dim=1)
 
         x = self.lift_network(x)
         # (left, right, top, bottom, front, back)
         x = F.pad(
             x,
-            (0, self.pad[0], 0, self.pad[1], 0, self.pad[2]),
+            (0, self.pad[2], 0, self.pad[1], 0, self.pad[0]),
             mode=self.padding_type,
         )
         # Spectral layers
         for k, conv_w in enumerate(zip(self.conv_layers, self.spconv_layers)):
             conv, w = conv_w
             if k < len(self.conv_layers) - 1:
                 x = self.activation_fn(conv(x) + w(x))
             else:
                 x = conv(x) + w(x)
 
-        x = x[..., : self.ipad[2], : self.ipad[1], : self.ipad[0]]
+        x = x[..., : self.ipad[0], : self.ipad[1], : self.ipad[2]]
         return x
 
     def meshgrid(self, shape: List[int], device: torch.device) -> Tensor:
         """Creates 3D meshgrid feature
 
         Parameters
         ----------
@@ -414,14 +413,165 @@
         grid_x, grid_y, grid_z = torch.meshgrid(grid_x, grid_y, grid_z, indexing="ij")
         grid_x = grid_x.unsqueeze(0).unsqueeze(0).repeat(bsize, 1, 1, 1, 1)
         grid_y = grid_y.unsqueeze(0).unsqueeze(0).repeat(bsize, 1, 1, 1, 1)
         grid_z = grid_z.unsqueeze(0).unsqueeze(0).repeat(bsize, 1, 1, 1, 1)
         return torch.cat((grid_x, grid_y, grid_z), dim=1)
 
 
+# ===================================================================
+# ===================================================================
+# 4D FNO
+# ===================================================================
+# ===================================================================
+
+
+class FNO4DEncoder(nn.Module):
+    """4D Spectral encoder for FNO
+
+    Parameters
+    ----------
+    in_channels : int, optional
+        Number of input channels, by default 1
+    num_fno_layers : int, optional
+        Number of spectral convolutional layers, by default 4
+    fno_layer_size : int, optional
+        Latent features size in spectral convolutions, by default 32
+    num_fno_modes : Union[int, List[int]], optional
+        Number of Fourier modes kept in spectral convolutions, by default 16
+    padding :  Union[int, List[int]], optional
+        Domain padding for spectral convolutions, by default 8
+    padding_type : str, optional
+        Type of padding for spectral convolutions, by default "constant"
+    activation_fn : nn.Module, optional
+        Activation function, by default nn.GELU
+    coord_features : bool, optional
+        Use coordinate grid as additional feature map, by default True
+    """
+
+    def __init__(
+        self,
+        in_channels: int = 1,
+        num_fno_layers: int = 4,
+        fno_layer_size: int = 32,
+        num_fno_modes: Union[int, List[int]] = 16,
+        padding: Union[int, List[int]] = 8,
+        padding_type: str = "constant",
+        activation_fn: nn.Module = nn.GELU(),
+        coord_features: bool = True,
+    ) -> None:
+        super().__init__()
+
+        self.in_channels = in_channels
+        self.num_fno_layers = num_fno_layers
+        self.fno_width = fno_layer_size
+        self.coord_features = coord_features
+        # Spectral modes to have weights
+        if isinstance(num_fno_modes, int):
+            num_fno_modes = [num_fno_modes, num_fno_modes, num_fno_modes, num_fno_modes]
+        # Add relative coordinate feature
+        if self.coord_features:
+            self.in_channels = self.in_channels + 4
+        self.activation_fn = activation_fn
+
+        self.spconv_layers = nn.ModuleList()
+        self.conv_layers = nn.ModuleList()
+
+        # Initial lift network
+        self.lift_network = torch.nn.Sequential()
+        self.lift_network.append(
+            layers.ConvNdFCLayer(self.in_channels, int(self.fno_width / 2))
+        )
+        self.lift_network.append(self.activation_fn)
+        self.lift_network.append(
+            layers.ConvNdFCLayer(int(self.fno_width / 2), self.fno_width)
+        )
+
+        # Build Neural Fourier Operators
+        for _ in range(self.num_fno_layers):
+            self.spconv_layers.append(
+                layers.SpectralConv4d(
+                    self.fno_width,
+                    self.fno_width,
+                    num_fno_modes[0],
+                    num_fno_modes[1],
+                    num_fno_modes[2],
+                    num_fno_modes[3],
+                )
+            )
+            self.conv_layers.append(
+                layers.ConvNdKernel1Layer(self.fno_width, self.fno_width)
+            )
+
+        # Padding values for spectral conv
+        if isinstance(padding, int):
+            padding = [padding, padding, padding, padding]
+        padding = padding + [0, 0, 0, 0]  # Pad with zeros for smaller lists
+        self.pad = padding[:4]
+        self.ipad = [-pad if pad > 0 else None for pad in self.pad]
+        self.padding_type = padding_type
+
+    def forward(self, x: Tensor) -> Tensor:
+        if self.coord_features:
+            coord_feat = self.meshgrid(list(x.shape), x.device)
+            x = torch.cat((x, coord_feat), dim=1)
+
+        x = self.lift_network(x)
+        # (left, right, top, bottom, front, back, past, future)
+        x = F.pad(
+            x,
+            (0, self.pad[3], 0, self.pad[2], 0, self.pad[1], 0, self.pad[0]),
+            mode=self.padding_type,
+        )
+        # Spectral layers
+        for k, conv_w in enumerate(zip(self.conv_layers, self.spconv_layers)):
+            conv, w = conv_w
+            if k < len(self.conv_layers) - 1:
+                x = self.activation_fn(conv(x) + w(x))
+            else:
+                x = conv(x) + w(x)
+
+        x = x[..., : self.ipad[0], : self.ipad[1], : self.ipad[2], : self.ipad[3]]
+        return x
+
+    def meshgrid(self, shape: List[int], device: torch.device) -> Tensor:
+        """Creates 4D meshgrid feature
+
+        Parameters
+        ----------
+        shape : List[int]
+            Tensor shape
+        device : torch.device
+            Device model is on
+
+        Returns
+        -------
+        Tensor
+            Meshgrid tensor
+        """
+        bsize, size_x, size_y, size_z, size_t = (
+            shape[0],
+            shape[2],
+            shape[3],
+            shape[4],
+            shape[5],
+        )
+        grid_x = torch.linspace(0, 1, size_x, dtype=torch.float32, device=device)
+        grid_y = torch.linspace(0, 1, size_y, dtype=torch.float32, device=device)
+        grid_z = torch.linspace(0, 1, size_z, dtype=torch.float32, device=device)
+        grid_t = torch.linspace(0, 1, size_t, dtype=torch.float32, device=device)
+        grid_x, grid_y, grid_z, grid_t = torch.meshgrid(
+            grid_x, grid_y, grid_z, grid_t, indexing="ij"
+        )
+        grid_x = grid_x.unsqueeze(0).unsqueeze(0).repeat(bsize, 1, 1, 1, 1, 1)
+        grid_y = grid_y.unsqueeze(0).unsqueeze(0).repeat(bsize, 1, 1, 1, 1, 1)
+        grid_z = grid_z.unsqueeze(0).unsqueeze(0).repeat(bsize, 1, 1, 1, 1, 1)
+        grid_t = grid_t.unsqueeze(0).unsqueeze(0).repeat(bsize, 1, 1, 1, 1, 1)
+        return torch.cat((grid_x, grid_y, grid_z, grid_t), dim=1)
+
+
 # Functions for converting between point based and grid (image) representations
 def _grid_to_points1d(value: Tensor) -> Tuple[Tensor, List[int]]:
     y_shape = list(value.size())
     output = torch.permute(value, (0, 2, 1))
     return output.reshape(-1, output.size(-1)), y_shape
 
 
@@ -448,14 +598,27 @@
 
 
 def _points_to_grid3d(value: Tensor, shape: List[int]) -> Tensor:
     output = value.reshape(shape[0], shape[2], shape[3], shape[4], value.size(-1))
     return torch.permute(output, (0, 4, 1, 2, 3))
 
 
+def _grid_to_points4d(value: Tensor) -> Tuple[Tensor, List[int]]:
+    y_shape = list(value.size())
+    output = torch.permute(value, (0, 2, 3, 4, 5, 1))
+    return output.reshape(-1, output.size(-1)), y_shape
+
+
+def _points_to_grid4d(value: Tensor, shape: List[int]) -> Tensor:
+    output = value.reshape(
+        shape[0], shape[2], shape[3], shape[4], shape[5], value.size(-1)
+    )
+    return torch.permute(output, (0, 5, 1, 2, 3, 4))
+
+
 # ===================================================================
 # ===================================================================
 # General FNO Model
 # ===================================================================
 # ===================================================================
 
 
@@ -477,15 +640,15 @@
 
 
 class FNO(Module):
     """Fourier neural operator (FNO) model.
 
     Note
     ----
-    The FNO architecture supports options for 1D, 2D and 3D fields which can
+    The FNO architecture supports options for 1D, 2D, 3D and 4D fields which can
     be controlled using the `dimension` parameter.
 
     Parameters
     ----------
     decoder_net : modulus.Module
         Pointwise decoder network, input feature size should match `latent_channels`
     in_channels : int
@@ -569,17 +732,21 @@
             FNOModel = FNO2DEncoder
             self.grid_to_points = _grid_to_points2d  # For JIT
             self.points_to_grid = _points_to_grid2d  # For JIT
         elif dimension == 3:
             FNOModel = FNO3DEncoder
             self.grid_to_points = _grid_to_points3d  # For JIT
             self.points_to_grid = _points_to_grid3d  # For JIT
+        elif dimension == 4:
+            FNOModel = FNO4DEncoder
+            self.grid_to_points = _grid_to_points4d  # For JIT
+            self.points_to_grid = _points_to_grid4d  # For JIT
         else:
             raise NotImplementedError(
-                "Invalid dimensionality. Only 1D, 2D and 3D FNO implemented"
+                "Invalid dimensionality. Only 1D, 2D, 3D and 4D FNO implemented"
             )
 
         self.spec_encoder = FNOModel(
             in_channels,
             num_fno_layers=self.num_fno_layers,
             fno_layer_size=latent_channels,
             num_fno_modes=self.num_fno_modes,
```

## modulus/models/graphcast/graph_cast_net.py

```diff
@@ -15,27 +15,29 @@
 import torch
 import torch.nn as nn
 from torch import Tensor
 
 from typing import Any
 from dataclasses import dataclass
 
-from .utils import set_checkpoint_fn, CuGraphCSC
-from .mlp import MLP
-from .processor import Processor
-from .utils import set_checkpoint_fn
-from .embedder import EncoderEmbedder, DecoderEmbedder
-from .encoder import EncoderSum, EncoderConcat
-from .decoder import DecoderSum, DecoderConcat
-
+from modulus.models.gnn_layers.utils import set_checkpoint_fn, CuGraphCSC
+from modulus.models.gnn_layers.embedder import (
+    GraphCastEncoderEmbedder,
+    GraphCastDecoderEmbedder,
+)
+from modulus.models.gnn_layers.mesh_graph_encoder import MeshGraphEncoder
+from modulus.models.gnn_layers.mesh_graph_decoder import MeshGraphDecoder
+from modulus.models.gnn_layers.mesh_graph_mlp import MeshGraphMLP
 from modulus.models.module import Module
 from modulus.models.meta import ModelMetaData
 from modulus.utils.graphcast.graph import Graph
 from modulus.utils.graphcast.data_utils import StaticData
 
+from .graph_cast_processor import GraphCastProcessor
+
 
 @dataclass
 class MetaData(ModelMetaData):
     name: str = "GraphCastNet"
     # Optimization
     jit: bool = False
     cuda_graphs: bool = False
@@ -125,20 +127,14 @@
         use_cugraphops_processor: bool = False,
         use_cugraphops_decoder: bool = False,
         do_concat_trick: bool = False,
         recompute_activation: bool = False,
     ):
         super().__init__(meta=MetaData())
 
-        # check the input resolution
-        if input_res != (721, 1440):
-            raise NotImplementedError(
-                "Currently only native ERA5 input resolution (721, 1440) is supported"
-            )
-
         # create the lat_lon_grid
         self.latitudes = torch.linspace(-90, 90, steps=input_res[0])
         self.longitudes = torch.linspace(-180, 180, steps=input_res[1] + 1)[1:]
         self.lat_lon_grid = torch.stack(
             torch.meshgrid(self.latitudes, self.longitudes, indexing="ij"), dim=-1
         )
         self.has_static_data = static_dataset_path is not None
@@ -170,149 +166,144 @@
 
         self.g2m_edata = self.g2m_graph.edata["x"]
         self.m2g_edata = self.m2g_graph.edata["x"]
         self.mesh_edata = self.mesh_graph.edata["x"]
         self.mesh_ndata = self.mesh_graph.ndata["x"]
 
         if use_cugraphops_encoder:
-            offsets, indices, edge_ids = self.g2m_graph.adj_sparse("csc")
+            offsets, indices, edge_ids = self.g2m_graph.adj_tensors("csc")
             n_in_nodes, n_out_nodes = (
                 self.g2m_graph.num_src_nodes(),
                 self.g2m_graph.num_dst_nodes(),
             )
             self.g2m_graph = CuGraphCSC(
                 offsets, indices, n_in_nodes, n_out_nodes, edge_ids
             )
 
         if use_cugraphops_decoder:
-            offsets, indices, edge_ids = self.m2g_graph.adj_sparse("csc")
+            offsets, indices, edge_ids = self.m2g_graph.adj_tensors("csc")
             n_in_nodes, n_out_nodes = (
                 self.m2g_graph.num_src_nodes(),
                 self.m2g_graph.num_dst_nodes(),
             )
             self.m2g_graph = CuGraphCSC(
                 offsets, indices, n_in_nodes, n_out_nodes, edge_ids
             )
 
         if use_cugraphops_processor:
-            offsets, indices, edge_ids = self.mesh_graph.adj_sparse("csc")
+            offsets, indices, edge_ids = self.mesh_graph.adj_tensors("csc")
             n_in_nodes, n_out_nodes = (
                 self.mesh_graph.num_src_nodes(),
                 self.mesh_graph.num_dst_nodes(),
             )
             self.mesh_graph = CuGraphCSC(
                 offsets, indices, n_in_nodes, n_out_nodes, edge_ids
             )
 
         # by default: don't checkpoint at all
         self.model_checkpoint_fn = set_checkpoint_fn(False)
         self.encoder_checkpoint_fn = set_checkpoint_fn(False)
         self.decoder_checkpoint_fn = set_checkpoint_fn(False)
 
         # initial feature embedder
-        self.encoder_embedder = EncoderEmbedder(
+        self.encoder_embedder = GraphCastEncoderEmbedder(
             input_dim_grid_nodes=input_dim_grid_nodes,
             input_dim_mesh_nodes=input_dim_mesh_nodes,
             input_dim_edges=input_dim_edges,
             output_dim=hidden_dim,
             hidden_dim=hidden_dim,
             hidden_layers=hidden_layers,
             activation_fn=activation_fn,
             norm_type=norm_type,
             recompute_activation=recompute_activation,
         )
-        self.decoder_embedder = DecoderEmbedder(
+        self.decoder_embedder = GraphCastDecoderEmbedder(
             input_dim_edges=input_dim_edges,
             output_dim=hidden_dim,
             hidden_dim=hidden_dim,
             hidden_layers=hidden_layers,
             activation_fn=activation_fn,
             norm_type=norm_type,
             recompute_activation=recompute_activation,
         )
 
         # grid2mesh encoder
-        Encoder = EncoderSum if do_concat_trick else EncoderConcat
-        self.encoder = Encoder(
-            graph=self.g2m_graph,
+        self.encoder = MeshGraphEncoder(
             aggregation=aggregation,
             input_dim_src_nodes=hidden_dim,
             input_dim_dst_nodes=hidden_dim,
             input_dim_edges=hidden_dim,
             output_dim_src_nodes=hidden_dim,
             output_dim_dst_nodes=hidden_dim,
             output_dim_edges=hidden_dim,
             hidden_dim=hidden_dim,
             hidden_layers=hidden_layers,
             activation_fn=activation_fn,
             norm_type=norm_type,
+            do_concat_trick=do_concat_trick,
             recompute_activation=recompute_activation,
         )
 
         # icosahedron processor
         assert processor_layers > 2, "Expected at least 3 processor layers"
-        self.processor_encoder = Processor(
-            graph=self.mesh_graph,
+        self.processor_encoder = GraphCastProcessor(
             aggregation=aggregation,
             processor_layers=1,
             input_dim_nodes=hidden_dim,
             input_dim_edges=hidden_dim,
             hidden_dim=hidden_dim,
             hidden_layers=hidden_layers,
             activation_fn=activation_fn,
             norm_type=norm_type,
             do_concat_trick=do_concat_trick,
             recompute_activation=recompute_activation,
         )
-        self.processor = Processor(
-            graph=self.mesh_graph,
+        self.processor = GraphCastProcessor(
             aggregation=aggregation,
             processor_layers=processor_layers - 2,
             input_dim_nodes=hidden_dim,
             input_dim_edges=hidden_dim,
             hidden_dim=hidden_dim,
             hidden_layers=hidden_layers,
             activation_fn=activation_fn,
             norm_type=norm_type,
             do_concat_trick=do_concat_trick,
             recompute_activation=recompute_activation,
         )
-        self.processor_decoder = Processor(
-            graph=self.mesh_graph,
+        self.processor_decoder = GraphCastProcessor(
             aggregation=aggregation,
             processor_layers=1,
             input_dim_nodes=hidden_dim,
             input_dim_edges=hidden_dim,
             hidden_dim=hidden_dim,
             hidden_layers=hidden_layers,
             activation_fn=activation_fn,
             norm_type=norm_type,
             do_concat_trick=do_concat_trick,
             recompute_activation=recompute_activation,
         )
 
         # mesh2grid decoder
-        Decoder = DecoderSum if do_concat_trick else DecoderConcat
-        self.decoder = Decoder(
-            graph=self.m2g_graph,
+        self.decoder = MeshGraphDecoder(
             aggregation=aggregation,
             input_dim_src_nodes=hidden_dim,
             input_dim_dst_nodes=hidden_dim,
             input_dim_edges=hidden_dim,
             output_dim_dst_nodes=hidden_dim,
             output_dim_edges=hidden_dim,
             hidden_dim=hidden_dim,
             hidden_layers=hidden_layers,
             activation_fn=activation_fn,
             norm_type=norm_type,
+            do_concat_trick=do_concat_trick,
             recompute_activation=recompute_activation,
         )
 
         # final MLP
-        self.finale = MLP(
+        self.finale = MeshGraphMLP(
             input_dim=hidden_dim,
             output_dim=output_dim_grid_nodes,
             hidden_dim=hidden_dim,
             hidden_layers=hidden_layers,
             activation_fn=activation_fn,
             norm_type=None,
             recompute_activation=recompute_activation,
@@ -455,19 +446,22 @@
         )
 
         # encode lat/lon to multimesh
         grid_nfeat_encoded, mesh_nfeat_encoded = self.encoder(
             g2m_efeat_embedded,
             grid_nfeat_embedded,
             mesh_nfeat_embedded,
+            self.g2m_graph,
         )
 
         # process multimesh graph
         mesh_efeat_processed, mesh_nfeat_processed = self.processor_encoder(
-            mesh_efeat_embedded, mesh_nfeat_encoded
+            mesh_efeat_embedded,
+            mesh_nfeat_encoded,
+            self.mesh_graph,
         )
 
         return mesh_efeat_processed, mesh_nfeat_processed, grid_nfeat_encoded
 
     def decoder_forward(
         self,
         mesh_efeat_processed: Tensor,
@@ -492,21 +486,22 @@
             The final node features for the latitude-longitude grid.
         """
 
         # process multimesh graph
         _, mesh_nfeat_processed = self.processor_decoder(
             mesh_efeat_processed,
             mesh_nfeat_processed,
+            self.mesh_graph,
         )
 
         m2g_efeat_embedded = self.decoder_embedder(self.m2g_edata)
 
         # decode multimesh to lat/lon
         grid_nfeat_decoded = self.decoder(
-            m2g_efeat_embedded, grid_nfeat_encoded, mesh_nfeat_processed
+            m2g_efeat_embedded, grid_nfeat_encoded, mesh_nfeat_processed, self.m2g_graph
         )
 
         # map to the target output dimension
         grid_nfeat_finale = self.finale(
             grid_nfeat_decoded,
         )
 
@@ -536,14 +531,15 @@
             preserve_rng_state=False,
         )
 
         # checkpoint of processor done in processor itself
         mesh_efeat_processed, mesh_nfeat_processed = self.processor(
             mesh_efeat_processed,
             mesh_nfeat_processed,
+            self.mesh_graph,
         )
 
         grid_nfeat_finale = self.decoder_checkpoint_fn(
             self.decoder_forward,
             mesh_efeat_processed,
             mesh_nfeat_processed,
             grid_nfeat_encoded,
@@ -617,21 +613,22 @@
             Keyword arguments to be passed to the `torch._C._nn._parse_to` function.
 
         Returns
         -------
         GraphCastNet
             The updated object after moving to the specified device, dtype, or format.
         """
-        self = super().to(*args, **kwargs)
+        self = super(GraphCastNet, self).to(*args, **kwargs)
+
         self.g2m_edata = self.g2m_edata.to(*args, **kwargs)
         self.m2g_edata = self.m2g_edata.to(*args, **kwargs)
         self.mesh_ndata = self.mesh_ndata.to(*args, **kwargs)
         self.mesh_edata = self.mesh_edata.to(*args, **kwargs)
         if self.has_static_data:
             self.static_data = self.static_data.to(*args, **kwargs)
 
-        self.encoder = self.encoder.to(*args, **kwargs)
-        self.decoder = self.decoder.to(*args, **kwargs)
-        self.processor = self.processor.to(*args, **kwargs)
-        self.processor_encoder = self.processor_encoder.to(*args, **kwargs)
-        self.processor_decoder = self.processor_decoder.to(*args, **kwargs)
+        device, _, _, _ = torch._C._nn._parse_to(*args, **kwargs)
+        self.g2m_graph = self.g2m_graph.to(device)
+        self.mesh_graph = self.mesh_graph.to(device)
+        self.m2g_graph = self.m2g_graph.to(device)
+
         return self
```

## modulus/models/layers/__init__.py

```diff
@@ -10,9 +10,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .activations import Identity, Stan, SquarePlus
 from .weight_norm import WeightNormLinear
-from .spectral_layers import SpectralConv1d, SpectralConv2d, SpectralConv3d
-from .fully_connected_layers import FCLayer, Conv1dFCLayer, Conv2dFCLayer, Conv3dFCLayer
+from .spectral_layers import (
+    SpectralConv1d,
+    SpectralConv2d,
+    SpectralConv3d,
+    SpectralConv4d,
+)
+from .fully_connected_layers import (
+    FCLayer,
+    Conv1dFCLayer,
+    Conv2dFCLayer,
+    Conv3dFCLayer,
+    ConvNdFCLayer,
+    ConvNdKernel1Layer,
+)
```

## modulus/models/layers/fft.py

```diff
@@ -240,15 +240,14 @@
     assert input.size(-1) == 2
     return input[..., 1]
 
 
 def _rfft_onnx(
     input: Tensor, s: Optional[Tuple[Optional[int]]], dim: Tuple[int], norm: str
 ) -> Tensor:
-
     if s is not None:
         _check_padding_rfft(s, dim, input.size())
 
     ndim = len(dim)
     assert ndim in [1, 2], ndim
 
     perm = not _is_last_dims(dim, input.ndim)
@@ -270,15 +269,14 @@
 
     return output
 
 
 def _irfft_onnx(
     input: Tensor, s: Optional[Tuple[Optional[int]]], dim: Tuple[int], norm: str
 ) -> Tensor:
-
     if s is not None:
         _check_padding_irfft(s, dim, input.size())
 
     ndim = len(dim)
     assert ndim in [1, 2], ndim
 
     # Whether to permute axes when DFT axis is not the last.
```

## modulus/models/layers/fully_connected_layers.py

```diff
@@ -232,7 +232,81 @@
         nn.init.constant_(self.conv.bias, 0)
         nn.init.xavier_uniform_(self.conv.weight)
 
     def forward(self, x: Tensor) -> Tensor:
         x = self.conv(x)
         x = self.apply_activation(x)
         return x
+
+
+class ConvNdFCLayer(ConvFCLayer):
+    """Channel-wise FC like layer with convolutions of arbitrary dimensions
+    CAUTION: if n_dims <= 3, use specific version for that n_dims instead
+
+    Parameters
+    ----------
+    in_features : int
+        Size of input features
+    out_features : int
+        Size of output features
+    activation_fn : Union[nn.Module, None], optional
+        Activation function to use. Can be None for no activation, by default None
+    activation_par : Union[nn.Parameter, None], optional
+        Additional parameters for the activation function, by default None
+    """
+
+    def __init__(
+        self,
+        in_channels: int,
+        out_channels: int,
+        activation_fn: Union[nn.Module, None] = None,
+        activation_par: Union[nn.Parameter, None] = None,
+    ) -> None:
+        super().__init__(activation_fn, activation_par)
+        self.in_channels = in_channels
+        self.out_channels = out_channels
+        self.conv = ConvNdKernel1Layer(in_channels, out_channels)
+        self.reset_parameters()
+
+    def reset_parameters(self):
+        self.conv.apply(self.initialise_parameters)  # recursively apply initialisations
+
+    def initialise_parameters(self, model):
+        """Reset layer weights"""
+        if hasattr(model, "bias"):
+            nn.init.constant_(model.bias, 0)
+        if hasattr(model, "weight"):
+            nn.init.xavier_uniform_(model.weight)
+
+    def forward(self, x: Tensor) -> Tensor:
+        x = self.conv(x)
+        x = self.apply_activation(x)
+        return x
+
+
+class ConvNdKernel1Layer(nn.Module):
+    """Channel-wise FC like layer for convolutions of arbitrary dimensions
+    CAUTION: if n_dims <= 3, use specific version for that n_dims instead
+
+    Parameters
+    ----------
+    in_features : int
+        Size of input features
+    out_features : int
+        Size of output features
+    """
+
+    def __init__(
+        self,
+        in_channels: int,
+        out_channels: int,
+    ) -> None:
+        super().__init__()
+        self.in_channels = in_channels
+        self.out_channels = out_channels
+        self.conv = nn.Conv1d(in_channels, out_channels, kernel_size=1, bias=True)
+
+    def forward(self, x: Tensor) -> Tensor:
+        dims = list(x.size())
+        dims[1] = self.out_channels
+        x = self.conv(x.view(dims[0], self.in_channels, -1)).view(dims)
+        return x
```

## modulus/models/layers/fused_silu.py

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import functools
 import torch
 from torch.autograd import Function
-from torch._C._nvfuser import Fusion, FusionDefinition, DataType
+from nvfuser._C import Fusion, FusionDefinition, DataType
 
 
 _torch_dtype_to_nvfuser = {
     torch.double: DataType.Double,
     torch.float: DataType.Float,
     torch.half: DataType.Half,
     torch.int: DataType.Int,
```

## modulus/models/layers/spectral_layers.py

```diff
@@ -296,7 +296,243 @@
 
     def reset_parameters(self):
         """Reset spectral weights with distribution scale*U(0,1)"""
         self.weights1.data = self.scale * torch.rand(self.weights1.data.shape)
         self.weights2.data = self.scale * torch.rand(self.weights2.data.shape)
         self.weights3.data = self.scale * torch.rand(self.weights3.data.shape)
         self.weights4.data = self.scale * torch.rand(self.weights4.data.shape)
+
+
+class SpectralConv4d(nn.Module):
+    """4D Fourier layer. It does FFT, linear transform, and Inverse FFT.
+
+    Parameters
+    ----------
+    in_channels : int
+        Number of input channels
+    out_channels : int
+        Number of output channels
+    modes1 : int
+        Number of Fourier modes to multiply in first dimension, at most floor(N/2) + 1
+    modes2 : int
+        Number of Fourier modes to multiply in second dimension, at most floor(N/2) + 1
+    modes3 : int
+        Number of Fourier modes to multiply in third dimension, at most floor(N/2) + 1
+    """
+
+    def __init__(
+        self,
+        in_channels: int,
+        out_channels: int,
+        modes1: int,
+        modes2: int,
+        modes3: int,
+        modes4: int,
+    ):
+        super().__init__()
+
+        self.in_channels = in_channels
+        self.out_channels = out_channels
+
+        # Number of Fourier modes to multiply, at most floor(N/2) + 1
+        self.modes1 = modes1
+        self.modes2 = modes2
+        self.modes3 = modes3
+        self.modes4 = modes4
+
+        self.scale = 1 / (in_channels * out_channels)
+        self.weights1 = nn.Parameter(
+            torch.empty(
+                in_channels,
+                out_channels,
+                self.modes1,
+                self.modes2,
+                self.modes3,
+                self.modes4,
+                2,
+            )
+        )
+        self.weights2 = nn.Parameter(
+            torch.empty(
+                in_channels,
+                out_channels,
+                self.modes1,
+                self.modes2,
+                self.modes3,
+                self.modes4,
+                2,
+            )
+        )
+        self.weights3 = nn.Parameter(
+            torch.empty(
+                in_channels,
+                out_channels,
+                self.modes1,
+                self.modes2,
+                self.modes3,
+                self.modes4,
+                2,
+            )
+        )
+        self.weights4 = nn.Parameter(
+            torch.empty(
+                in_channels,
+                out_channels,
+                self.modes1,
+                self.modes2,
+                self.modes3,
+                self.modes4,
+                2,
+            )
+        )
+        self.weights5 = nn.Parameter(
+            torch.empty(
+                in_channels,
+                out_channels,
+                self.modes1,
+                self.modes2,
+                self.modes3,
+                self.modes4,
+                2,
+            )
+        )
+        self.weights6 = nn.Parameter(
+            torch.empty(
+                in_channels,
+                out_channels,
+                self.modes1,
+                self.modes2,
+                self.modes3,
+                self.modes4,
+                2,
+            )
+        )
+        self.weights7 = nn.Parameter(
+            torch.empty(
+                in_channels,
+                out_channels,
+                self.modes1,
+                self.modes2,
+                self.modes3,
+                self.modes4,
+                2,
+            )
+        )
+        self.weights8 = nn.Parameter(
+            torch.empty(
+                in_channels,
+                out_channels,
+                self.modes1,
+                self.modes2,
+                self.modes3,
+                self.modes4,
+                2,
+            )
+        )
+        self.reset_parameters()
+
+    def compl_mul4d(
+        self,
+        input: Tensor,
+        weights: Tensor,
+    ) -> Tensor:
+        """Complex multiplication
+
+        Parameters
+        ----------
+        input : Tensor
+            Input tensor
+        weights : Tensor
+            Weights tensor
+
+        Returns
+        -------
+        Tensor
+            Product of complex multiplication
+        """
+        # (batch, in_channel, x, y, z), (in_channel, out_channel, x, y, z) -> (batch, out_channel, x, y, z)
+        cweights = torch.view_as_complex(weights)
+        return torch.einsum("bixyzt,ioxyzt->boxyzt", input, cweights)
+
+    def forward(self, x: Tensor) -> Tensor:
+        batchsize = x.shape[0]
+        # Compute Fourier coeffcients up to factor of e^(- something constant)
+        x_ft = torch.fft.rfftn(x, dim=[-4, -3, -2, -1])
+
+        # Multiply relevant Fourier modes
+        out_ft = torch.zeros(
+            batchsize,
+            self.out_channels,
+            x.size(-4),
+            x.size(-3),
+            x.size(-2),
+            x.size(-1) // 2 + 1,
+            dtype=torch.cfloat,
+            device=x.device,
+        )
+
+        # print(f'mod: size x: {x_ft.size()}, out: {out_ft.size()}')
+        # print(f'mod: x_ft[weight4]: {x_ft[:, :, self.modes1 :, self.modes2 :, : -self.modes3, :self.modes4].size()} weight4: {self.weights4.size()}')
+
+        out_ft[
+            :, :, : self.modes1, : self.modes2, : self.modes3, : self.modes4
+        ] = self.compl_mul4d(
+            x_ft[:, :, : self.modes1, : self.modes2, : self.modes3, : self.modes4],
+            self.weights1,
+        )
+        out_ft[
+            :, :, -self.modes1 :, : self.modes2, : self.modes3, : self.modes4
+        ] = self.compl_mul4d(
+            x_ft[:, :, -self.modes1 :, : self.modes2, : self.modes3, : self.modes4],
+            self.weights2,
+        )
+        out_ft[
+            :, :, : self.modes1, -self.modes2 :, : self.modes3, : self.modes4
+        ] = self.compl_mul4d(
+            x_ft[:, :, : self.modes1, -self.modes2 :, : self.modes3, : self.modes4],
+            self.weights3,
+        )
+        out_ft[
+            :, :, : self.modes1, : self.modes2, -self.modes3 :, : self.modes4
+        ] = self.compl_mul4d(
+            x_ft[:, :, : self.modes1, : self.modes2, -self.modes3 :, : self.modes4],
+            self.weights4,
+        )
+        out_ft[
+            :, :, -self.modes1 :, -self.modes2 :, : self.modes3, : self.modes4
+        ] = self.compl_mul4d(
+            x_ft[:, :, -self.modes1 :, -self.modes2 :, : self.modes3, : self.modes4],
+            self.weights5,
+        )
+        out_ft[
+            :, :, -self.modes1 :, : self.modes2, -self.modes3 :, : self.modes4
+        ] = self.compl_mul4d(
+            x_ft[:, :, -self.modes1 :, : self.modes2, -self.modes3 :, : self.modes4],
+            self.weights6,
+        )
+        out_ft[
+            :, :, : self.modes1, -self.modes2 :, -self.modes3 :, : self.modes4
+        ] = self.compl_mul4d(
+            x_ft[:, :, : self.modes1, -self.modes2 :, -self.modes3 :, : self.modes4],
+            self.weights7,
+        )
+        out_ft[
+            :, :, -self.modes1 :, -self.modes2 :, -self.modes3 :, : self.modes4
+        ] = self.compl_mul4d(
+            x_ft[:, :, -self.modes1 :, -self.modes2 :, -self.modes3 :, : self.modes4],
+            self.weights8,
+        )
+
+        # Return to physical space
+        x = torch.fft.irfftn(out_ft, s=(x.size(-4), x.size(-3), x.size(-2), x.size(-1)))
+        return x
+
+    def reset_parameters(self):
+        """Reset spectral weights with distribution scale*U(0,1)"""
+        self.weights1.data = self.scale * torch.rand(self.weights1.data.shape)
+        self.weights2.data = self.scale * torch.rand(self.weights2.data.shape)
+        self.weights3.data = self.scale * torch.rand(self.weights3.data.shape)
+        self.weights4.data = self.scale * torch.rand(self.weights4.data.shape)
+        self.weights5.data = self.scale * torch.rand(self.weights5.data.shape)
+        self.weights6.data = self.scale * torch.rand(self.weights6.data.shape)
+        self.weights7.data = self.scale * torch.rand(self.weights7.data.shape)
+        self.weights8.data = self.scale * torch.rand(self.weights8.data.shape)
```

## modulus/models/meshgraphnet/meshgraphnet.py

```diff
@@ -11,38 +11,41 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import torch
 from torch import Tensor
 import torch.nn as nn
-import modulus
+import dgl
 
 try:
-    import dgl
-    import dgl.function as fn
     from dgl import DGLGraph
 except:
     raise ImportError(
         "Mesh Graph Net requires the DGL library. Install the "
         + "desired CUDA version at: \n https://www.dgl.ai/pages/start.html"
     )
-from torch.nn import Sequential, ModuleList, Linear, ReLU, LayerNorm
-from typing import Union, List
+from typing import Callable, Tuple, List, Union
 from dataclasses import dataclass
 
-from ..meta import ModelMetaData
-from ..module import Module
+import modulus
+from modulus.models.meta import ModelMetaData
+from modulus.models.module import Module
+
+from modulus.models.gnn_layers.utils import set_checkpoint_fn, CuGraphCSC
+from modulus.models.gnn_layers.mesh_graph_mlp import MeshGraphMLP
+from modulus.models.gnn_layers.mesh_edge_block import MeshEdgeBlock
+from modulus.models.gnn_layers.mesh_node_block import MeshNodeBlock
 
 
 @dataclass
 class MetaData(ModelMetaData):
     name: str = "MeshGraphNet"
-    # Optimization
-    jit: bool = True
+    # Optimization, no JIT as DGLGraph causes trouble
+    jit: bool = False
     cuda_graphs: bool = False
     amp_cpu: bool = False
     amp_gpu: bool = True
     torch_fx: bool = False
     # Inference
     onnx: bool = False
     # Physics informed
@@ -75,26 +78,32 @@
         Hidden layer size for the edge feature encoder, by default 128
     num_layers_edge_encoder : int, optional
         Number of MLP layers for the edge feature encoder, by default 2
     hidden_dim_node_decoder : int, optional
         Hidden layer size for the node feature decoder, by default 128
     num_layers_node_decoder : int, optional
         Number of MLP layers for the node feature decoder, by default 2
+    aggregation: str, optional
+        Message aggregation type, by default "sum"
+    do_conat_trick: : bool, default=False
+        Whether to replace concat+MLP with MLP+idx+sum
+    num_processor_checkpoint_segments: int, optional
+        Number of processor segments for gradient checkpointing, by default 0 (checkpointing disabled)
 
     Example
     -------
     >>> model = modulus.models.meshgraphnet.MeshGraphNet(
     ...         input_dim_nodes=4,
     ...         input_dim_edges=3,
     ...         output_dim=2,
     ...     )
     >>> graph = dgl.rand_graph(10, 5)
     >>> node_features = torch.randn(10, 4)
     >>> edge_features = torch.randn(5, 3)
-    >>> output = model(graph, node_features, edge_features)
+    >>> output = model(node_features, edge_features, graph)
     >>> output.size()
     torch.Size([10, 2])
 
     Note
     ----
     Reference: Pfaff, Tobias, et al. "Learning mesh-based simulation with graph networks."
     arXiv preprint arXiv:2010.03409 (2020).
@@ -110,256 +119,209 @@
         num_layers_edge_processor: int = 2,
         hidden_dim_node_encoder: int = 128,
         num_layers_node_encoder: int = 2,
         hidden_dim_edge_encoder: int = 128,
         num_layers_edge_encoder: int = 2,
         hidden_dim_node_decoder: int = 128,
         num_layers_node_decoder: int = 2,
+        aggregation: str = "sum",
+        do_concat_trick: bool = False,
+        num_processor_checkpoint_segments: int = 0,
     ):
         super().__init__(meta=MetaData())
 
-        self.edge_encoder = _Encoder(
+        self.edge_encoder = MeshGraphMLP(
             input_dim_edges,
-            hidden_dim_edge_encoder,
-            num_layers_edge_encoder,
+            output_dim=hidden_dim_edge_encoder,
+            hidden_dim=hidden_dim_edge_encoder,
+            hidden_layers=num_layers_edge_encoder,
+            activation_fn=nn.ReLU(),
+            norm_type="LayerNorm",
+            recompute_activation=False,
         )
-        self.node_encoder = _Encoder(
+        self.node_encoder = MeshGraphMLP(
             input_dim_nodes,
-            hidden_dim_node_encoder,
-            num_layers_node_encoder,
+            output_dim=hidden_dim_node_encoder,
+            hidden_dim=hidden_dim_node_encoder,
+            hidden_layers=num_layers_node_encoder,
+            activation_fn=nn.ReLU(),
+            norm_type="LayerNorm",
+            recompute_activation=False,
         )
-        self.node_decoder = _Decoder(
-            output_dim, hidden_dim_node_decoder, num_layers_node_decoder
+        self.node_decoder = MeshGraphMLP(
+            hidden_dim_node_encoder,
+            output_dim=output_dim,
+            hidden_dim=hidden_dim_node_decoder,
+            hidden_layers=num_layers_node_decoder,
+            activation_fn=nn.ReLU(),
+            norm_type=None,
+            recompute_activation=False,
         )
-        self.processor = _GraphProcessor(
+        self.processor = MeshGraphNetProcessor(
             processor_size=processor_size,
             input_dim_node=hidden_dim_node_encoder,
-            num_layers_node=num_layers_node_processor,
             input_dim_edge=hidden_dim_edge_encoder,
+            num_layers_node=num_layers_node_processor,
             num_layers_edge=num_layers_edge_processor,
+            aggregation=aggregation,
+            norm_type="LayerNorm",
+            activation_fn=nn.ReLU(),
+            do_concat_trick=do_concat_trick,
+            num_processor_checkpoint_segments=num_processor_checkpoint_segments,
         )
 
-    @torch.jit.unused
     def forward(
         self,
-        graph: Union[DGLGraph, List[DGLGraph]],
         node_features: Tensor,
         edge_features: Tensor,
+        graph: Union[DGLGraph, List[DGLGraph]],
     ) -> Tensor:
         edge_features = self.edge_encoder(edge_features)
         node_features = self.node_encoder(node_features)
-        x = self.processor(graph, node_features, edge_features)
+        x = self.processor(node_features, edge_features, graph)
         x = self.node_decoder(x)
         return x
 
 
-class _Encoder(nn.Module):
-    """MeshGraphNet encoder
-
-    Parameters
-    ----------
-    input_dim : int
-        Number of input features
-    hidden_dim : int, optional
-        Number of neurons in each hidden layer, by default 128
-    num_layers : int, optional
-        Number of hidden layers, by default 2
-    layer_norm : bool, optional
-        Use layer norm in the last layer, by default True
-    """
-
-    def __init__(
-        self,
-        input_dim: int,
-        hidden_dim: int = 128,
-        num_layers: int = 2,
-        layer_norm: bool = True,
-    ):
-        super().__init__()
-        self.mlp = [Linear(input_dim, hidden_dim), ReLU()]
-        for _ in range(num_layers - 1):
-            self.mlp += [Linear(hidden_dim, hidden_dim), ReLU()]
-        self.mlp.append(Linear(hidden_dim, hidden_dim))
-        if layer_norm:
-            self.mlp.append(LayerNorm(hidden_dim))
-        self.mlp = Sequential(*self.mlp)
-
-    def forward(self, x: Tensor) -> Tensor:
-        return self.mlp(x)
-
-
-class _Decoder(nn.Module):
-    """MeshGraphNet encoder
-
-    Parameters
-    ----------
-    output_dim : int
-        Number of output features
-    hidden_dim : int, optional
-        Number of neurons in each hidden layer, by default 128
-    num_layers : int, optional
-        Number of hidden layers, by default 2
-    layer_norm : bool, optional
-        Use layer norm in the last layer, by default False
-    """
+class MeshGraphNetProcessor(nn.Module):
+    """MeshGraphNet processor block"""
 
     def __init__(
         self,
-        output_dim: int,
-        hidden_dim: int = 128,
-        num_layers: int = 2,
-        layer_norm: bool = False,
-    ):
-        super().__init__()
-        self.mlp = [Linear(hidden_dim, hidden_dim), ReLU()]
-        for _ in range(num_layers - 1):
-            self.mlp += [Linear(hidden_dim, hidden_dim), ReLU()]
-        self.mlp.append(Linear(hidden_dim, output_dim))
-        if layer_norm:
-            self.mlp.append(LayerNorm(output_dim))
-        self.mlp = Sequential(*self.mlp)
-
-    def forward(self, x: Tensor) -> Tensor:
-        return self.mlp(x)
-
-
-class _EdgeBlock(nn.Module):
-    def __init__(
-        self,
+        processor_size: int = 15,
         input_dim_node: int = 128,
         input_dim_edge: int = 128,
-        num_layers: int = 2,
-        layer_norm: bool = True,
+        num_layers_node: int = 2,
+        num_layers_edge: int = 2,
+        aggregation: str = "sum",
+        norm_type: str = "LayerNorm",
+        activation_fn: nn.Module = nn.ReLU(),
+        do_concat_trick: bool = False,
+        num_processor_checkpoint_segments: int = 0,
     ):
         super().__init__()
-        self.edge_mlp = [
-            Linear(2 * input_dim_node + input_dim_edge, input_dim_edge),
-            ReLU(),
-        ]
-        for _ in range(num_layers - 1):
-            self.edge_mlp += [Linear(input_dim_edge, input_dim_edge), ReLU()]
-        self.edge_mlp.append(Linear(input_dim_edge, input_dim_edge))
-        if layer_norm:
-            self.edge_mlp.append(LayerNorm(input_dim_edge))
-        self.edge_mlp = Sequential(*self.edge_mlp)
+        self.processor_size = processor_size
+        self.num_processor_checkpoint_segments = num_processor_checkpoint_segments
 
-    @torch.jit.unused
-    def forward(
-        self, graph: DGLGraph, node_features: Tensor, edge_features: Tensor
-    ) -> Tensor:
-        with graph.local_scope():
-            if isinstance(node_features, tuple):
-                node_features_src, node_features_dst = node_features
-            else:
-                node_features_src = node_features_dst = node_features
-            graph.srcdata["x"] = node_features_src
-            graph.dstdata["x"] = node_features_dst
-            graph.edata["x"] = edge_features
-            graph.apply_edges(self.concat_message_function)
-            return (
-                self.edge_mlp(graph.edata["cat_feat"]) + edge_features
-            )  # residual connection
-
-    @staticmethod
-    def concat_message_function(
-        edges,
-    ):  # TODO feature concat on edges is not efficient, consider optimizing this
-        return {
-            "cat_feat": torch.cat(
-                (edges.src["x"], edges.dst["x"], edges.data["x"]), dim=1
-            )
-        }
+        edge_block_invars = (
+            input_dim_node,
+            input_dim_edge,
+            input_dim_edge,
+            input_dim_edge,
+            num_layers_edge,
+            activation_fn,
+            norm_type,
+            do_concat_trick,
+            False,
+        )
+        node_block_invars = (
+            aggregation,
+            input_dim_node,
+            input_dim_edge,
+            input_dim_edge,
+            input_dim_edge,
+            num_layers_node,
+            activation_fn,
+            norm_type,
+            False,
+        )
 
+        edge_blocks = []
+        node_blocks = []
+        layers = []
 
-class _NodeBlock(nn.Module):
-    def __init__(
-        self,
-        input_dim_node: int = 128,
-        input_dim_edge: int = 128,
-        num_layers: int = 2,
-        layer_norm: bool = True,
-    ):
-        super().__init__()
-        self.node_mlp = [
-            Linear(input_dim_node + input_dim_edge, input_dim_node),
-            ReLU(),
-        ]
-        for _ in range(num_layers - 1):
-            self.node_mlp += [Linear(input_dim_node, input_dim_node), ReLU()]
-        self.node_mlp.append(Linear(input_dim_node, input_dim_node))
-        if layer_norm:
-            self.node_mlp.append(LayerNorm(input_dim_node))
-        self.node_mlp = Sequential(*self.node_mlp)
+        for _ in range(self.processor_size):
+            edge_blocks.append(MeshEdgeBlock(*edge_block_invars))
 
-    @torch.jit.unused
-    def forward(
-        self, graph: DGLGraph, node_features: Tensor, edge_features: Tensor
-    ) -> Tensor:
-        with graph.local_scope():
-            if isinstance(node_features, tuple):
-                node_features_src, node_features_dst = node_features
-            else:
-                node_features_src = node_features_dst = node_features
-            graph.srcdata["x"] = node_features_src
-            graph.dstdata["x"] = node_features_dst
-            graph.edata["x"] = edge_features
-            graph.update_all(
-                fn.copy_e("x", "m"), fn.sum("m", "h_dest")
-            )  # aggregate edge message by target
-            graph.dstdata["h_dest"] = torch.cat(
-                (graph.dstdata["h_dest"], node_features_dst), -1
-            )
-            return (
-                self.node_mlp(graph.dstdata["h_dest"]) + node_features_dst
-            )  # residual connection
+        for _ in range(self.processor_size):
+            node_blocks.append(MeshNodeBlock(*node_block_invars))
 
+        for i in range(self.processor_size):
+            layers.append(edge_blocks[i])
+            layers.append(node_blocks[i])
 
-class _GraphProcessor(nn.Module):
-    def __init__(
-        self,
-        processor_size: int = 15,
-        input_dim_node: int = 128,
-        num_layers_node: int = 2,
-        input_dim_edge: int = 128,
-        num_layers_edge: int = 2,
-    ):
-        super().__init__()
-        self.processor_size = processor_size
-        self.edge_blocks = ModuleList(
-            [
-                _EdgeBlock(
-                    input_dim_node,
-                    input_dim_edge,
-                    num_layers_edge,
+        self.processor_layers = nn.ModuleList(layers)
+        self.num_processor_layers = len(self.processor_layers)
+        self.set_checkpoint_segments(self.num_processor_checkpoint_segments)
+
+    def set_checkpoint_segments(self, checkpoint_segments: int):
+        """
+        Set the number of checkpoint segments
+
+        Parameters
+        ----------
+        checkpoint_segments : int
+            number of checkpoint segments
+
+        Raises
+        ------
+        ValueError
+            if the number of processor layers is not a multiple of the number of
+            checkpoint segments
+        """
+        if checkpoint_segments > 0:
+            if self.num_processor_layers % checkpoint_segments != 0:
+                raise ValueError(
+                    "Processor layers must be a multiple of checkpoint_segments"
                 )
-                for _ in range(self.processor_size)
-            ]
-        )
-        self.node_blocks = ModuleList(
-            [
-                _NodeBlock(input_dim_node, input_dim_edge, num_layers_node)
-                for _ in range(self.processor_size)
-            ]
-        )
+            segment_size = self.num_processor_layers // checkpoint_segments
+            self.checkpoint_segments = []
+            for i in range(0, self.num_processor_layers, segment_size):
+                self.checkpoint_segments.append((i, i + segment_size))
+            self.checkpoint_fn = set_checkpoint_fn(True)
+        else:
+            self.checkpoint_fn = set_checkpoint_fn(False)
+            self.checkpoint_segments = [(0, self.num_processor_layers)]
+
+    def run_function(
+        self, segment_start: int, segment_end: int
+    ) -> Callable[
+        [Tensor, Tensor, Union[DGLGraph, List[DGLGraph]]], Tuple[Tensor, Tensor]
+    ]:
+        """Custom forward for gradient checkpointing
+
+        Parameters
+        ----------
+        segment_start : int
+            Layer index as start of the segment
+        segment_end : int
+            Layer index as end of the segment
+
+        Returns
+        -------
+        Callable
+            Custom forward function
+        """
+        segment = self.processor_layers[segment_start:segment_end]
+
+        def custom_forward(
+            node_features: Tensor,
+            edge_features: Tensor,
+            graph: Union[DGLGraph, List[DGLGraph]],
+        ) -> Tuple[Tensor, Tensor]:
+            """Custom forward function"""
+            for module in segment:
+                edge_features, node_features = module(
+                    edge_features, node_features, graph
+                )
+            return edge_features, node_features
+
+        return custom_forward
 
     @torch.jit.unused
     def forward(
         self,
-        graph: Union[DGLGraph, List[DGLGraph]],
         node_features: Tensor,
         edge_features: Tensor,
+        graph: Union[DGLGraph, List[DGLGraph], CuGraphCSC],
     ) -> Tensor:
-        for i in range(self.processor_size):
-            if isinstance(graph, List):  # in case of neighbor sampling
-                edge_features = edge_features[: graph[i].num_edges(), :]  # TODO check
-                node_features_src = node_features
-                node_features_dst = node_features_src[: graph[i].num_dst_nodes()]
-                edge_features = self.edge_blocks[i](
-                    graph[i], (node_features_src, node_features_dst), edge_features
-                )
-                node_features = self.node_blocks[i](
-                    graph[i], (node_features_src, node_features_dst), edge_features
-                )
-            else:
-                edge_features = self.edge_blocks[i](graph, node_features, edge_features)
-                node_features = self.node_blocks[i](graph, node_features, edge_features)
+        for segment_start, segment_end in self.checkpoint_segments:
+            edge_features, node_features = self.checkpoint_fn(
+                self.run_function(segment_start, segment_end),
+                node_features,
+                edge_features,
+                graph,
+                use_reentrant=False,
+                preserve_rng_state=False,
+            )
+
         return node_features
```

## modulus/models/rnn/rnn_one2many.py

```diff
@@ -218,15 +218,15 @@
             rnn_output.append(h)
 
         decoded_output = []
         for t in range(self.nr_tsteps):
             x_out = rnn_output[t]
             # Decoding step
             latent_context_grid = []
-            for (conv_layer, decoder) in zip(self.conv_layers, self.decoder_layers):
+            for conv_layer, decoder in zip(self.conv_layers, self.decoder_layers):
                 latent_context_grid.append(conv_layer(x_out))
                 upsampling_layers = decoder
                 for upsampling_layer in upsampling_layers:
                     x_out = upsampling_layer(x_out)
 
             # Add a convolution here to make the channel dimensions same as output
             # Only last latent context grid is used, but mult-resolution is available
```

## modulus/models/rnn/rnn_seq2seq.py

```diff
@@ -226,15 +226,15 @@
             rnn_output.append(h)
 
         decoded_output = []
         for t in range(self.nr_tsteps):
             x_out = rnn_output[t]
             # Decoding step
             latent_context_grid = []
-            for (conv_layer, decoder) in zip(self.conv_layers, self.decoder_layers):
+            for conv_layer, decoder in zip(self.conv_layers, self.decoder_layers):
                 latent_context_grid.append(conv_layer(x_out))
                 upsampling_layers = decoder
                 for upsampling_layer in upsampling_layers:
                     x_out = upsampling_layer(x_out)
 
             # Add a convolution here to make the channel dimensions same as output
             # Only last latent context grid is used, but mult-resolution is available
```

## modulus/models/srrn/super_res_net.py

```diff
@@ -171,15 +171,14 @@
             in_channels=conv_layer_size,
             out_channels=out_channels,
             kernel_size=large_kernel_size,
             batch_norm=False,
         )
 
     def forward(self, in_vars: Tensor) -> Tensor:
-
         output = self.conv_block1(in_vars)  # (N, 3, w, h)
         residual = output  # (N, n_channels, w, h)
         output = self.residual_blocks(output)  # (N, n_channels, w, h)
         output = self.conv_block2(output)  # (N, n_channels, w, h)
         output = output + residual  # (N, n_channels, w, h)
         output = self.subpixel_convolutional_blocks(
             output
@@ -316,15 +315,14 @@
         )
         # These additional channels are shuffled to form additional pixels,
         #  upscaling each dimension by the scaling factor
         self.pixel_shuffle = PixelShuffle3d(scaling_factor)
         self.prelu = nn.PReLU()
 
     def forward(self, input: Tensor) -> Tensor:
-
         output = self.conv(input)  # (N, n_channels * scaling factor^2, w, h)
         output = self.pixel_shuffle(
             output
         )  # (N, n_channels, w * scaling factor, h * scaling factor)
         output = self.prelu(
             output
         )  # (N, n_channels, w * scaling factor, h * scaling factor)
```

## modulus/utils/__init__.py

```diff
@@ -8,8 +8,11 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .capture import StaticCaptureTraining, StaticCaptureEvaluateNoGrad
+from .capture import (
+    StaticCaptureTraining,
+    StaticCaptureEvaluateNoGrad,
+)
```

## modulus/utils/capture.py

```diff
@@ -13,119 +13,131 @@
 # limitations under the License.
 
 import functools
 import modulus
 import torch
 import logging
 from logging import Logger
-from typing import Union, Any, Callable, NewType
+from typing import Union, Any, Callable, NewType, Dict, Optional
 from contextlib import nullcontext
 
 float16 = NewType("float16", torch.float16)
 bfloat16 = NewType("bfloat16", torch.bfloat16)
 optim = NewType("optim", torch.optim)
 
 
 class _StaticCapture(object):
     """Base class for StaticCapture decorator.
 
     This class should not be used, rather StaticCaptureTraining and StaticCaptureEvaluate
     should be used instead for training and evaluation functions.
     """
 
-    # Grad scalar singleton use for checkpointing
-    # This limits the number of staticcapture AMP training instances to just one per program
-    scaler_dict = None
-    scaler_singleton = None
+    # Grad scaler and checkpoint class variables use for checkpoint saving and loading
+    # Since an instance of Static capture does not exist for checkpoint functions
+    # one must use class functions to access state dicts
+    _amp_scalers = {}
+    _amp_scaler_checkpoints = {}
+    _logger = logging.getLogger("capture")
+
+    def __new__(cls, *args, **kwargs):
+        obj = super(_StaticCapture, cls).__new__(cls)
+        obj.amp_scalers = cls._amp_scalers
+        obj.amp_scaler_checkpoints = cls._amp_scaler_checkpoints
+        obj.logger = cls._logger
+        return obj
 
     def __init__(
         self,
-        model: modulus.Module,
+        model: modulus.models.Module,
         optim: Union[optim, None] = None,
         logger: Union[Logger, None] = None,
         use_graphs: bool = True,
-        use_amp: bool = True,
+        use_autocast: bool = True,
+        use_gradscaler: bool = True,
         cuda_graph_warmup: int = 11,
         amp_type: Union[float16, bfloat16] = torch.float16,
+        label: Optional[str] = None,
     ):
-        self.logger = logger
-        if self.logger is None:
-            self.logger = logging.getLogger("capture")
+        self.logger = logger if logger else self.logger
+        # Checkpoint label (used for gradscaler)
+        self.label = label if label else f"scaler_{len(self.amp_scalers.keys())}"
 
         # DDP fix
-        if not isinstance(model, modulus.Module) and hasattr(model, "module"):
+        if not isinstance(model, modulus.models.Module) and hasattr(model, "module"):
             model = model.module
 
-        if not isinstance(model, modulus.Module):
+        if not isinstance(model, modulus.models.Module):
             self.logger.error("Model not a Modulus Module!")
             raise ValueError("Model not a Modulus Module!")
         self.model = model
 
         self.optim = optim
         self.eval = False
         self.no_grad = False
 
         # Set up toggles for optimizations
         assert (
             amp_type == torch.float16 or amp_type == torch.bfloat16
         ), "AMP type must be torch.float16 or torch.bfloat16"
+        # CUDA device
         if "cuda" in str(self.model.device):
             # CUDA graphs
             if use_graphs and not self.model.meta.cuda_graphs:
                 self.logger.warning(
                     f"Model {model.meta.name} does not support CUDA graphs, turning off"
                 )
                 use_graphs = False
             self.cuda_graphs_enabled = use_graphs
 
             # AMP GPU
-            if use_amp and not self.model.meta.amp_gpu:
+            if not self.model.meta.amp_gpu:
                 self.logger.warning(
                     f"Model {model.meta.name} does not support AMP on GPUs, turning off"
                 )
-                use_amp = False
-            self.amp_enabled = use_amp
+                use_autocast = False
+                use_gradscaler = False
+            self.use_gradscaler = use_gradscaler
+            self.use_autocast = use_autocast
 
             self.amp_device = "cuda"
             # Check if bfloat16 is suppored on the GPU
             if amp_type == torch.bfloat16 and not torch.cuda.is_bf16_supported():
                 self.logger.warning(
                     f"Current CUDA device does not support bfloat16, falling back to float16"
                 )
                 amp_type = torch.float16
             self.amp_dtype = amp_type
             # Gradient Scaler
-            scalar_enabled = self.amp_enabled and amp_type == torch.float16
-            self.scaler = torch.cuda.amp.GradScaler(enabled=scalar_enabled)
-            _StaticCapture._register_scaler(self.scaler, self.logger)
+            scaler_enabled = self.use_gradscaler and amp_type == torch.float16
+            self.scaler = self._init_amp_scaler(scaler_enabled, self.logger)
 
             self.replay_stream = torch.cuda.current_stream(self.model.device)
+        # CPU device
         else:
             self.cuda_graphs_enabled = False
             # AMP CPU
-            if use_amp and not self.model.meta.amp_cpu:
+            if use_autocast and not self.model.meta.amp_cpu:
                 self.logger.warning(
                     f"Model {model.meta.name} does not support AMP on CPUs, turning off"
                 )
-                use_amp = False
-            self.amp_enabled = use_amp
+                use_autocast = False
+
+            self.use_autocast = use_autocast
             self.amp_device = "cpu"
             # Only float16 is supported on CPUs
             # https://pytorch.org/docs/stable/amp.html#cpu-op-specific-behavior
-            if amp_type == torch.float16 and use_amp:
+            if amp_type == torch.float16 and use_autocast:
                 self.logger.warning(
                     f"torch.float16 not supported for CPU AMP, switching to torch.bfloat16"
                 )
                 amp_type = torch.bfloat16
             self.amp_dtype = torch.bfloat16
-            # Gradient Scaler
-            self.scaler = torch.cuda.amp.GradScaler(
-                enabled=False
-            )  # Always false on CPU
-            _StaticCapture._register_scaler(self.scaler, self.logger)
+            # Gradient Scaler (not enabled)
+            self.scaler = self._init_amp_scaler(False, self.logger)
             self.replay_stream = None
 
         if self.cuda_graphs_enabled:
             self.graph = torch.cuda.CUDAGraph()
 
         self.output = None
         self.iteration = 0
@@ -216,79 +228,126 @@
 
         Returns
         -------
         Any
             Output of neural network forward
         """
         with torch.autocast(
-            self.amp_device, enabled=self.amp_enabled, dtype=self.amp_dtype
+            self.amp_device, enabled=self.use_autocast, dtype=self.amp_dtype
         ):
             output = self.function(*args, **kwargs)
 
         if not self.eval:
             # In training mode output should be the loss
             self.scaler.scale(output).backward()
         return output
 
-    @classmethod
-    def _register_scaler(
-        cls, scaler: torch.cuda.amp.GradScaler, logger: Logger
-    ) -> None:
-        """Class method for saving/loading the grad scaler state dictionary singleton
-
-        Parameters
-        ----------
-        scaler : torch.cuda.amp.GradScaler
-            AMP grad scaler
-        logger : Logger
-            Python console logger
-        """
-        if cls.scaler_dict:
+    def _init_amp_scaler(
+        self, scaler_enabled: bool, logger: Logger
+    ) -> torch.cuda.amp.GradScaler:
+        # Create gradient scaler
+        scaler = torch.cuda.amp.GradScaler(enabled=scaler_enabled)
+        # Store scaler in class variable
+        self.amp_scalers[self.label] = scaler
+        logging.debug(f"Created gradient scaler {self.label}")
+
+        # If our checkpoint dictionary has weights for this scaler lets load
+        if self.label in self.amp_scaler_checkpoints:
             try:
-                scaler.load_state_dict(cls.scaler_dict)
-                logger.success("Loaded grad scaler state dictionary")
-            except:
-                logger.error(
-                    "Failed to load grad scalar state dict from saved singleton. "
-                    + "This could be from loading a invalid checkpoint or using multiple "
-                    + "static captures that have AMP active. Be careful."
+                scaler.load_state_dict(self.amp_scaler_checkpoints[self.label])
+                del self.amp_scaler_checkpoints[self.label]
+                self.logger.info(f"Loaded grad scaler state dictionary {self.label}.")
+            except Exception as e:
+                self.logger.error(
+                    f"Failed to load grad scaler {self.label} state dict from saved "
+                    + "checkpoints. Did you switch the ordering of declared static captures?"
                 )
+                raise ValueError(e)
+        return scaler
 
-        cls.scaler_singleton = scaler
+    @classmethod
+    def state_dict(cls) -> Dict[str, Any]:
+        """Class method for accsessing the StaticCapture state dictionary.
+        Use this in a training checkpoint function.
+
+        Returns
+        -------
+        Dict[str, Any]
+            Dictionary of states to save for file
+        """
+        scaler_states = {}
+        for key, value in cls._amp_scalers.items():
+            scaler_states[key] = value.state_dict()
+
+        return scaler_states
+
+    @classmethod
+    def load_state_dict(cls, state_dict: Dict[str, Any]) -> None:
+        """Class method for loading a StaticCapture state dictionary.
+        Use this in a training checkpoint function.
+
+        Returns
+        -------
+        Dict[str, Any]
+            Dictionary of states to save for file
+        """
+        scaler_states = {}
+        for key, value in state_dict.items():
+            # If scaler has been created already load the weights
+            if key in cls._amp_scalers:
+                try:
+                    cls._amp_scalers[key].load_state_dict(value)
+                    cls._logger.info(f"Loaded grad scaler state dictionary {key}.")
+                except Exception as e:
+                    cls._logger.error(
+                        f"Failed to load grad scaler state dict with id {key}."
+                        + " Something went wrong!"
+                    )
+                    raise ValueError(e)
+            # Otherwise store in checkpoints for later use
+            else:
+                cls._amp_scaler_checkpoints[key] = value
+
+    @classmethod
+    def reset_state(cls):
+        cls._amp_scalers = {}
+        cls._amp_scaler_checkpoints = {}
 
 
 class StaticCaptureTraining(_StaticCapture):
     """A performance optimization decorator for PyTorch training functions.
 
     This class should be initialized as a decorator on a function that computes the
     forward pass of the neural network and loss function. The user should only call the
     defind training step function. This will apply optimizations including: AMP and
     Cuda Graphs.
 
     Parameters
     ----------
-    model : modulus.Module
+    model : modulus.models.Module
         Modulus Model
     optim : torch.optim
         Optimizer
     logger : Union[Logger, None], optional
         Modulus Launch Logger, by default None
     use_graphs : bool, optional
         Toggle CUDA graphs if supported by model, by default True
     use_amp : bool, optional
         Toggle AMP if supported by mode, by default True
     cuda_graph_warmup : int, optional
         Number of warmup steps for cuda graphs, by default 11
     amp_type : Union[float16, bfloat16], optional
         Auto casting type for AMP, by default torch.float16
+    label : Optional[str, None], optional
+        Static capture checkpoint label, by default None
 
     Raises
     ------
     ValueError
-        If the model provided is not a modulus.Module. I.e. has no meta data.
+        If the model provided is not a modulus.models.Module. I.e. has no meta data.
 
     Example
     -------
     >>> # Create model
     >>> model = modulus.models.mlp.FullyConnected(2, 64, 2)
     >>> input = torch.rand(8, 2)
     >>> output = torch.rand(8, 2)
@@ -304,72 +363,79 @@
     >>> # Sample training loop
     >>> for i in range(3):
     ...     loss = training_step(model, input, output)
     ...
 
     Note
     ----
-    Presently only a single instance of training static capture with AMP can be
-    used due to a grad scalar singleton.
+    Static captures must be checkpointed when training using the `state_dict()` if AMP
+    is being used with gradient scaler. By default, this requires static captures to be
+    instantiated in the same order as when they were checkpointed. The label parameter
+    can be used to relax/circumvent this ordering requirement.
 
     Note
     ----
     Capturing multiple cuda graphs in a single program can lead to potential invalid CUDA
     memory access errors on some systems. Prioritize capturing training graphs when this
     occurs.
     """
 
     def __init__(
         self,
-        model: modulus.Module,
+        model: modulus.models.Module,
         optim: torch.optim,
         logger: Union[Logger, None] = None,
         use_graphs: bool = True,
         use_amp: bool = True,
         cuda_graph_warmup: int = 11,
         amp_type: Union[float16, bfloat16] = torch.float16,
+        label: Optional[str] = None,
     ):
         super().__init__(
             model,
             optim,
             logger,
             use_graphs,
             use_amp,
+            use_amp,
             cuda_graph_warmup,
             amp_type,
+            label,
         )
 
 
 class StaticCaptureEvaluateNoGrad(_StaticCapture):
 
     """An performance optimization decorator for PyTorch no grad evaluation.
 
     This class should be initialized as a decorator on a function that computes run the
     forward pass of the model that does not require gradient calculations. This is the
     recommended method to use for inference and validation methods.
 
     Parameters
     ----------
-    model : modulus.Module
+    model : modulus.models.Module
         Modulus Model
     logger : Union[Logger, None], optional
         Modulus Launch Logger, by default None
     use_graphs : bool, optional
         Toggle CUDA graphs if supported by model, by default True
     use_amp : bool, optional
         Toggle AMP if supported by mode, by default True
     cuda_graph_warmup : int, optional
         Number of warmup steps for cuda graphs, by default 11
     amp_type : Union[float16, bfloat16], optional
         Auto casting type for AMP, by default torch.float16
+    label : Optional[str, None], optional
+        Static capture checkpoint label, by default None
 
     Raises
     ------
     ValueError
-        If the model provided is not a modulus.Module. I.e. has no meta data.
+        If the model provided is not a modulus.models.Module. I.e. has no meta data.
 
     Example
     -------
     >>> # Create model
     >>> model = modulus.models.mlp.FullyConnected(2, 64, 2)
     >>> input = torch.rand(8, 2)
     >>> # Create evaluate function with optimization wrapper
@@ -387,25 +453,28 @@
     Capturing multiple cuda graphs in a single program can lead to potential invalid CUDA
     memory access errors on some systems. Prioritize capturing training graphs when this
     occurs.
     """
 
     def __init__(
         self,
-        model: modulus.Module,
+        model: modulus.models.Module,
         logger: Union[Logger, None] = None,
         use_graphs: bool = True,
         use_amp: bool = True,
         cuda_graph_warmup: int = 11,
         amp_type: Union[float16, bfloat16] = torch.float16,
+        label: Optional[str] = None,
     ):
         super().__init__(
             model,
             None,
             logger,
             use_graphs,
             use_amp,
+            False,
             cuda_graph_warmup,
             amp_type,
+            label,
         )
         self.eval = True  # No optimizer/scaler calls
         self.no_grad = True  # No grad context and no grad zeroing
```

## modulus/utils/graphcast/graph.py

```diff
@@ -15,25 +15,28 @@
 import os
 import torch
 import json
 import numpy as np
 
 from torch import Tensor
 from sklearn.neighbors import NearestNeighbors
+import logging
 
 from .graph_utils import (
     cell_to_adj,
     create_graph,
     create_heterograph,
     add_edge_features,
     add_node_features,
     latlon2xyz,
     get_edge_len,
 )
 
+logger = logging.getLogger(__name__)
+
 
 class Graph:
     """Graph class for creating the graph2mesh, multimesh, and mesh2graph graphs.
 
     Parameters
     ----------
     icospheres_path : str
@@ -54,22 +57,29 @@
         try:
             with open(icospheres_path, "r") as f:
                 loaded_dict = json.load(f)
                 icospheres = {
                     key: (np.array(value) if isinstance(value, list) else value)
                     for key, value in loaded_dict.items()
                 }
+                logger.info(f"Opened pre-computed graph at {icospheres_path}.")
         except:
             from modulus.utils.graphcast.icospheres import (
                 generate_and_save_icospheres,
             )  # requires PyMesh
 
+            logger.info(
+                f"Could not open {icospheres_path}...generating mesh from scratch."
+            )
             generate_and_save_icospheres()
 
         self.icospheres = icospheres
+        self.max_order = (
+            len([key for key in self.icospheres.keys() if "faces" in key]) - 2
+        )
 
         # flatten lat/lon gird
         self.lat_lon_grid_flat = lat_lon_grid.permute(2, 0, 1).view(2, -1).permute(1, 0)
 
     def create_mesh_graph(self, verbose: bool = True) -> Tensor:
         """Create the multimesh graph.
 
@@ -80,31 +90,27 @@
 
         Returns
         -------
         DGLGraph
             Multimesh graph.
         """
         # create the bi-directional mesh graph
-        multimesh_faces = np.concatenate(
-            (
-                self.icospheres["order_0_faces"],
-                self.icospheres["order_1_faces"],
-                self.icospheres["order_2_faces"],
-                self.icospheres["order_3_faces"],
-                self.icospheres["order_4_faces"],
-                self.icospheres["order_5_faces"],
-                self.icospheres["order_6_faces"],
+        multimesh_faces = self.icospheres["order_0_faces"]
+        for i in range(1, self.max_order + 1):
+            multimesh_faces = np.concatenate(
+                (multimesh_faces, self.icospheres["order_" + str(i) + "_faces"])
             )
-        )
+
         src, dst = cell_to_adj(multimesh_faces)
         mesh_graph = create_graph(
             src, dst, to_bidirected=True, add_self_loop=False, dtype=torch.int32
         )
         mesh_pos = torch.tensor(
-            self.icospheres["order_6_vertices"], dtype=torch.float32
+            self.icospheres["order_" + str(self.max_order) + "_vertices"],
+            dtype=torch.float32,
         )
         mesh_graph = add_edge_features(mesh_graph, mesh_pos)
         mesh_graph = add_node_features(mesh_graph, mesh_pos)
         # ensure fields set to dtype to avoid later conversions
         mesh_graph.ndata["x"] = mesh_graph.ndata["x"].to(dtype=self.dtype)
         mesh_graph.edata["x"] = mesh_graph.edata["x"].to(dtype=self.dtype)
         if verbose:
@@ -120,43 +126,43 @@
             verbosity, by default True
 
         Returns
         -------
         DGLGraph
             Graph2mesh graph.
         """
-        # get the max edge length of icosphere order 6
-        edge_src = self.icospheres["order_6_vertices"][
-            self.icospheres["order_6_faces"][:, 0]
+        # get the max edge length of icosphere with max order
+        edge_src = self.icospheres["order_" + str(self.max_order) + "_vertices"][
+            self.icospheres["order_" + str(self.max_order) + "_faces"][:, 0]
         ]
-        edge_dst = self.icospheres["order_6_vertices"][
-            self.icospheres["order_6_faces"][:, 1]
+        edge_dst = self.icospheres["order_" + str(self.max_order) + "_vertices"][
+            self.icospheres["order_" + str(self.max_order) + "_faces"][:, 1]
         ]
         edge_len_1 = np.max(get_edge_len(edge_src, edge_dst))
-        edge_src = self.icospheres["order_6_vertices"][
-            self.icospheres["order_6_faces"][:, 0]
+        edge_src = self.icospheres["order_" + str(self.max_order) + "_vertices"][
+            self.icospheres["order_" + str(self.max_order) + "_faces"][:, 0]
         ]
-        edge_dst = self.icospheres["order_6_vertices"][
-            self.icospheres["order_6_faces"][:, 2]
+        edge_dst = self.icospheres["order_" + str(self.max_order) + "_vertices"][
+            self.icospheres["order_" + str(self.max_order) + "_faces"][:, 2]
         ]
         edge_len_2 = np.max(get_edge_len(edge_src, edge_dst))
-        edge_src = self.icospheres["order_6_vertices"][
-            self.icospheres["order_6_faces"][:, 1]
+        edge_src = self.icospheres["order_" + str(self.max_order) + "_vertices"][
+            self.icospheres["order_" + str(self.max_order) + "_faces"][:, 1]
         ]
-        edge_dst = self.icospheres["order_6_vertices"][
-            self.icospheres["order_6_faces"][:, 2]
+        edge_dst = self.icospheres["order_" + str(self.max_order) + "_vertices"][
+            self.icospheres["order_" + str(self.max_order) + "_faces"][:, 2]
         ]
         edge_len_3 = np.max(get_edge_len(edge_src, edge_dst))
         edge_len = max([edge_len_1, edge_len_2, edge_len_3])
 
         # create the grid2mesh bipartite graph
         cartesian_grid = latlon2xyz(self.lat_lon_grid_flat)
         n_nbrs = 4
         neighbors = NearestNeighbors(n_neighbors=n_nbrs).fit(
-            self.icospheres["order_6_vertices"]
+            self.icospheres["order_" + str(self.max_order) + "_vertices"]
         )
         distances, indices = neighbors.kneighbors(cartesian_grid)
 
         src, dst = [], []
         for i in range(len(cartesian_grid)):
             for j in range(n_nbrs):
                 if distances[i][j] <= 0.6 * edge_len:
@@ -167,15 +173,16 @@
                     # in the paper what they use.
 
         g2m_graph = create_heterograph(
             src, dst, ("grid", "g2m", "mesh"), dtype=torch.int32
         )  # number of edges is 3,114,720, exactly matches with the paper
         g2m_graph.srcdata["pos"] = cartesian_grid.to(torch.float32)
         g2m_graph.dstdata["pos"] = torch.tensor(
-            self.icospheres["order_6_vertices"], dtype=torch.float32
+            self.icospheres["order_" + str(self.max_order) + "_vertices"],
+            dtype=torch.float32,
         )
         g2m_graph = add_edge_features(
             g2m_graph, (g2m_graph.srcdata["pos"], g2m_graph.dstdata["pos"])
         )
         # avoid potential conversions at later points
         g2m_graph.srcdata["pos"] = g2m_graph.srcdata["pos"].to(dtype=self.dtype)
         g2m_graph.dstdata["pos"] = g2m_graph.dstdata["pos"].to(dtype=self.dtype)
@@ -203,26 +210,31 @@
         DGLGraph
             Mesh2grid graph.
         """
         # create the mesh2grid bipartite graph
         cartesian_grid = latlon2xyz(self.lat_lon_grid_flat)
         n_nbrs = 1
         neighbors = NearestNeighbors(n_neighbors=n_nbrs).fit(
-            self.icospheres["order_6_face_centroid"]
+            self.icospheres["order_" + str(self.max_order) + "_face_centroid"]
         )
         _, indices = neighbors.kneighbors(cartesian_grid)
         indices = indices.flatten()
 
-        src = [p for i in indices for p in self.icospheres["order_6_faces"][i]]
+        src = [
+            p
+            for i in indices
+            for p in self.icospheres["order_" + str(self.max_order) + "_faces"][i]
+        ]
         dst = [i for i in range(len(cartesian_grid)) for _ in range(3)]
         m2g_graph = create_heterograph(
             src, dst, ("mesh", "m2g", "grid"), dtype=torch.int32
         )  # number of edges is 3,114,720, exactly matches with the paper
         m2g_graph.srcdata["pos"] = torch.tensor(
-            self.icospheres["order_6_vertices"], dtype=torch.float32
+            self.icospheres["order_" + str(self.max_order) + "_vertices"],
+            dtype=torch.float32,
         )
         m2g_graph.dstdata["pos"] = cartesian_grid.to(dtype=torch.float32)
         m2g_graph = add_edge_features(
             m2g_graph, (m2g_graph.srcdata["pos"], m2g_graph.dstdata["pos"])
         )
         # avoid potential conversions at later points
         m2g_graph.srcdata["pos"] = m2g_graph.srcdata["pos"].to(dtype=self.dtype)
```

## modulus/utils/graphcast/icospheres.py

```diff
@@ -20,29 +20,29 @@
 except ImportError:
     Warning("pymesh is not installed. Please install it to use icosphere.")
 
 # TODO apply a transformation to make faces parallel to ploes
 
 
 def generate_and_save_icospheres(
-    save_path: str = "icospheres.json",
+    save_path: str = "icospheres.json", level: int = 6
 ) -> None:  # pragma: no cover
     """enerate icospheres from level 0 to 6 (inclusive) and save them to a json file.
 
     Parameters
     ----------
     path : str
         Path to save the json file.
     """
     radius = 1
     center = np.array((0, 0, 0))
     icospheres = {"vertices": [], "faces": []}
 
     # Generate icospheres from level 0 to 6 (inclusive)
-    for order in range(6 + 1):
+    for order in range(level + 1):
         icosphere = pymesh.generate_icosphere(radius, center, refinement_order=order)
         icospheres["order_" + str(order) + "_vertices"] = icosphere.vertices
         icospheres["order_" + str(order) + "_faces"] = icosphere.faces
         icosphere.add_attribute("face_centroid")
         icospheres[
             "order_" + str(order) + "_face_centroid"
         ] = icosphere.get_face_attribute("face_centroid")
@@ -50,7 +50,11 @@
     # save icosphere vertices and faces to a json file
     icospheres_dict = {
         key: (value.tolist() if isinstance(value, np.ndarray) else value)
         for key, value in icospheres.items()
     }
     with open(save_path, "w") as f:
         json.dump(icospheres_dict, f)
+
+
+if __name__ == "__main__":
+    generate_and_save_icospheres(level=6)
```

## Comparing `modulus/datapipes/gnn/mgn_dataset.py` & `modulus/datapipes/gnn/vortex_shedding_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,19 +29,21 @@
 except:
     raise ImportError(
         "Mesh Graph Net Datapipe requires the DGL library. Install the "
         + "desired CUDA version at: https://www.dgl.ai/pages/start.html"
     )
 from torch.nn import functional as F
 
+from .utils import read_vtp_file, save_json, load_json
+
 # Hide GPU from visible devices for TF
 tf.config.set_visible_devices([], "GPU")
 
 
-class MGNDataset(DGLDataset):
+class VortexSheddingDataset(DGLDataset):
     """In-memory MeshGraphNet Dataset for stationary mesh
     Notes:
         - This dataset prepares and processes the data available in MeshGraphNet's repo:
             https://github.com/deepmind/deepmind-research/tree/master/meshgraphnets
         - A single adj matrix is used for each transient simulation.
             Do not use with adaptive mesh or remeshing
 
@@ -111,15 +113,15 @@
                 self.cells.append(data_np["cells"][0])
                 self.rollout_mask.append(self._get_rollout_mask(node_type))
 
         # compute or load edge data stats
         if self.split == "train":
             self.edge_stats = self._get_edge_stats()
         else:
-            self.edge_stats = self._load_json("edge_stats.json")
+            self.edge_stats = load_json("edge_stats.json")
 
         # normalize edge features
         for i in range(num_samples):
             self.graphs[i].edata["x"] = self.normalize_edge(
                 self.graphs[i],
                 self.edge_stats["edge_mean"],
                 self.edge_stats["edge_std"],
@@ -147,15 +149,15 @@
             self.node_features.append(features)
             self.node_targets.append(targets)
 
         # compute or load node data stats
         if self.split == "train":
             self.node_stats = self._get_node_stats()
         else:
-            self.node_stats = self._load_json("node_stats.json")
+            self.node_stats = load_json("node_stats.json")
 
         # normalize node features
         for i in range(num_samples):
             self.node_features[i]["velocity"] = self.normalize_node(
                 self.node_features[i]["velocity"],
                 self.node_stats["velocity_mean"],
                 self.node_stats["velocity_std"],
@@ -213,15 +215,15 @@
             )
         stats["edge_std"] = torch.sqrt(
             stats["edge_meansqr"] - torch.square(stats["edge_mean"])
         )
         stats.pop("edge_meansqr")
 
         # save to file
-        self._save_json(stats, "edge_stats.json")
+        save_json(stats, "edge_stats.json")
         return stats
 
     def _get_node_stats(self):
         stats = {
             "velocity_mean": 0,
             "velocity_meansqr": 0,
             "velocity_diff_mean": 0,
@@ -270,15 +272,15 @@
             stats["velocity_diff_meansqr"] - torch.square(stats["velocity_diff_mean"])
         )
         stats.pop("velocity_meansqr")
         stats.pop("pressure_meansqr")
         stats.pop("velocity_diff_meansqr")
 
         # save to file
-        self._save_json(stats, "node_stats.json")
+        save_json(stats, "node_stats.json")
         return stats
 
     def _load_tf_data(self, path, split):
         """
         Utility for loading the .tfrecord dataset in DeepMind's MeshGraphNet repo:
         https://github.com/deepmind/deepmind-research/tree/master/meshgraphnets
         Follow the instructions provided in that repo to download the .tfrecord files.
@@ -365,27 +367,14 @@
         return torch.tensor(invar[1:], dtype=torch.float)
 
     @staticmethod
     def _push_forward_diff(invar):
         return torch.tensor(invar[1:] - invar[0:-1], dtype=torch.float)
 
     @staticmethod
-    def _save_json(var, file):
-        var_list = {k: v.numpy().tolist() for k, v in var.items()}
-        with open(file, "w") as f:
-            json.dump(var_list, f)
-
-    @staticmethod
-    def _load_json(file):
-        with open(file, "r") as f:
-            var_list = json.load(f)
-        var = {k: torch.tensor(v, dtype=torch.float) for k, v in var_list.items()}
-        return var
-
-    @staticmethod
     def _get_rollout_mask(node_type):
         mask = torch.logical_or(
             torch.eq(node_type, torch.zeros_like(node_type)),
             torch.eq(
                 node_type,
                 torch.zeros_like(node_type) + 5,
             ),
```

## Comparing `modulus/models/graphcast/edge_block.py` & `modulus/models/graphcast/graph_cast_processor.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,226 +11,167 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import torch
 import torch.nn as nn
 
-from typing import Any, Union
+from typing import Union
 from torch import Tensor
 from dgl import DGLGraph
-from .mlp import MLP, TruncatedMLP, TruncatedMLPCuGraph
-from .utils import concat_efeat_dgl_mesh, CuGraphCSC
 
-try:
-    from pylibcugraphops.pytorch.operators import update_efeat_static_e2e
-except ModuleNotFoundError:
-    update_efeat_static_e2e = None
+from modulus.models.gnn_layers.utils import set_checkpoint_fn, CuGraphCSC
+from modulus.models.gnn_layers.mesh_node_block import MeshNodeBlock
+from modulus.models.gnn_layers.mesh_edge_block import MeshEdgeBlock
 
 
-class EdgeBlockConcat(nn.Module):
-    """Edge block with an explicit concatenation of features.
+class GraphCastProcessor(nn.Module):
+    """Processor block used in GraphCast operating on a latent space
+    represented by hierarchy of icosahedral meshes.
 
     Parameters
     ----------
-    graph : DGLGraph | CuGraphCSC
-        Graph.
+    aggregation : str, optional
+        message passing aggregation method ("sum", "mean"), by default "sum"
+    processor_layers : int, optional
+        number of processor layers, by default 16
     input_dim_nodes : int, optional
-        Input dimensionality of the node features, by default 512
+        input dimensionality of the node features, by default 512
     input_dim_edges : int, optional
-        Input dimensionality of the edge features, by default 512
-    output_dim : int, optional
-        Output dimensionality of the edge features, by default 512
+        input dimensionality of the edge features, by default 512
     hidden_dim : int, optional
-        _description_, by default 512
+        number of neurons in each hidden layer, by default 512
     hidden_layers : int, optional
-        Number of neurons in each hidden layer, by default 1
+        number of hiddel layers, by default 1
     activation_fn : nn.Module, optional
-        Type of activation function, by default nn.SiLU()
+        type of activation function, by default nn.SiLU()
     norm_type : str, optional
         normalization type, by default "LayerNorm"
+    do_conat_trick: : bool, default=False
+        whether to replace concat+MLP with MLP+idx+sum
     recompute_activation : bool, optional
         Flag for recomputing activation in backward to save memory, by default False.
         Currently, only SiLU is supported.
     """
 
     def __init__(
         self,
-        graph: Union[DGLGraph, CuGraphCSC],
+        aggregation: str = "sum",
+        processor_layers: int = 16,
         input_dim_nodes: int = 512,
         input_dim_edges: int = 512,
-        output_dim: int = 512,
         hidden_dim: int = 512,
         hidden_layers: int = 1,
         activation_fn: nn.Module = nn.SiLU(),
         norm_type: str = "LayerNorm",
+        do_concat_trick: bool = False,
         recompute_activation: bool = False,
     ):
         super().__init__()
-        self.graph = graph
-        self.use_cugraphops = isinstance(graph, CuGraphCSC)
 
-        dim_concat = 2 * input_dim_nodes + input_dim_edges
-        self.edge_MLP = MLP(
-            input_dim=dim_concat,
-            output_dim=output_dim,
-            hidden_dim=hidden_dim,
-            hidden_layers=hidden_layers,
-            activation_fn=activation_fn,
-            norm_type=norm_type,
-            recompute_activation=recompute_activation,
+        edge_block_invars = (
+            input_dim_nodes,
+            input_dim_edges,
+            input_dim_edges,
+            hidden_dim,
+            hidden_layers,
+            activation_fn,
+            norm_type,
+            do_concat_trick,
+            recompute_activation,
+        )
+        node_block_invars = (
+            aggregation,
+            input_dim_nodes,
+            input_dim_edges,
+            input_dim_nodes,
+            hidden_dim,
+            hidden_layers,
+            activation_fn,
+            norm_type,
+            recompute_activation,
         )
 
-    def forward(
-        self,
-        efeat: Tensor,
-        nfeat: Tensor,
-    ) -> Tensor:
-        if self.use_cugraphops:
-            static_graph = self.graph.to_static_csc()
-            cat_feat = update_efeat_static_e2e(
-                efeat,
-                nfeat,
-                static_graph,
-                mode="concat",
-                use_source_emb=True,
-                use_target_emb=True,
-            )
-
-        else:
-            cat_feat = concat_efeat_dgl_mesh(efeat, nfeat, self.graph)
-
-        efeat_new = self.edge_MLP(cat_feat) + efeat
-        return efeat_new, nfeat
+        layers = []
+        for _ in range(processor_layers):
+            layers.append(MeshEdgeBlock(*edge_block_invars))
+            layers.append(MeshNodeBlock(*node_block_invars))
+
+        self.processor_layers = nn.ModuleList(layers)
+        self.num_processor_layers = len(self.processor_layers)
+        # per default, no checkpointing
+        # one segment for compatability
+        self.checkpoint_segments = [(0, self.num_processor_layers)]
+        self.checkpoint_fn = set_checkpoint_fn(False)
 
-    def to(self, *args: Any, **kwargs: Any) -> "EdgeBlockConcat":
-        """Moves the object to the specified device, dtype, or format.
-        This method moves the object and its underlying graph to the specified
-        device, dtype, or format, and returns the updated object.
+    def set_checkpoint_segments(self, checkpoint_segments: int):
+        """
+        Set the number of checkpoint segments
 
         Parameters
         ----------
-        *args : Any
-            Positional arguments to be passed to the `torch._C._nn._parse_to` function.
-        **kwargs : Any
-            Keyword arguments to be passed to the `torch._C._nn._parse_to` function.
+        checkpoint_segments : int
+            number of checkpoint segments
 
-        Returns
-        -------
-        EdgeBlockDGLConcat
-            The updated object after moving to the specified device, dtype, or format.
+        Raises
+        ------
+        ValueError
+            if the number of processor layers is not a multiple of the number of
+            checkpoint segments
         """
-        self = super().to(*args, **kwargs)
-        device, _, _, _ = torch._C._nn._parse_to(*args, **kwargs)
-        self.graph = self.graph.to(device=device)
-        return self
-
+        if checkpoint_segments > 0:
+            if self.num_processor_layers % checkpoint_segments != 0:
+                raise ValueError(
+                    "Processor layers must be a multiple of checkpoint_segments"
+                )
+            segment_size = self.num_processor_layers // checkpoint_segments
+            self.checkpoint_segments = []
+            for i in range(0, self.num_processor_layers, segment_size):
+                self.checkpoint_segments.append((i, i + segment_size))
 
-class EdgeBlockSum(nn.Module):
-    """Edge block with truncated MLPs.
+            self.checkpoint_fn = set_checkpoint_fn(True)
+        else:
+            self.checkpoint_fn = set_checkpoint_fn(False)
+            self.checkpoint_segments = [(0, self.num_processor_layers)]
 
-    Parameters
-    ----------
-    graph : DGLGraph
-        Graph.
-    input_dim_nodes : int, optional
-        Input dimensionality of the node features, by default 512
-    input_dim_edges : int, optional
-        Input dimensionality of the edge features, by default 512
-    output_dim : int, optional
-        Output dimensionality of the edge features, by default 512
-    hidden_dim : int, optional
-        _description_, by default 512
-    hidden_layers : int, optional
-        Number of neurons in each hidden layer, by default 1
-    activation_fn : nn.Module, optional
-        Type of activation function, by default nn.SiLU()
-    norm_type : str, optional
-        normalization type, by default "LayerNorm"
-    recompute_activation : bool, optional
-        Flag for recomputing activation in backward to save memory, by default False.
-        Currently, only SiLU is supported.
-    """
+    def run_function(self, segment_start: int, segment_end: int):
+        """Custom forward for gradient checkpointing
 
-    def __init__(
-        self,
-        graph: Union[DGLGraph, CuGraphCSC],
-        input_dim_nodes: int = 512,
-        input_dim_edges: int = 512,
-        output_dim: int = 512,
-        hidden_dim: int = 512,
-        hidden_layers: int = 1,
-        activation_fn: nn.Module = nn.SiLU(),
-        norm_type: str = "LayerNorm",
-        recompute_activation: bool = False,
-    ):
-        super().__init__()
-        self.graph = graph
-        self.use_cugraphops = isinstance(graph, CuGraphCSC)
+        Parameters
+        ----------
+        segment_start : int
+            Layer index as start of the segment
+        segment_end : int
+            Layer index as end of the segment
 
-        if self.use_cugraphops:
-            self.edge_trunc_mlp = TruncatedMLPCuGraph(
-                efeat_dim=input_dim_edges,
-                src_dim=input_dim_nodes,
-                dst_dim=input_dim_nodes,
-                output_dim=output_dim,
-                hidden_dim=hidden_dim,
-                hidden_layers=hidden_layers,
-                activation_fn=activation_fn,
-                norm_type=norm_type,
-                recompute_activation=recompute_activation,
-            )
+        Returns
+        -------
+        function
+            Custom forward function
+        """
+        segment = self.processor_layers[segment_start:segment_end]
 
-        else:
-            self.src, self.dst = (item.long() for item in self.graph.edges())
+        def custom_forward(efeat, nfeat, graph):
+            """Custom forward function"""
+            for module in segment:
+                efeat, nfeat = module(efeat, nfeat, graph)
+            return efeat, nfeat
 
-            self.edge_trunc_mlp = TruncatedMLP(
-                efeat_dim=input_dim_edges,
-                src_dim=input_dim_nodes,
-                dst_dim=input_dim_nodes,
-                output_dim=output_dim,
-                hidden_dim=hidden_dim,
-                hidden_layers=hidden_layers,
-                activation_fn=activation_fn,
-                norm_type=norm_type,
-                recompute_activation=recompute_activation,
-            )
+        return custom_forward
 
     def forward(
         self,
         efeat: Tensor,
         nfeat: Tensor,
+        graph: Union[DGLGraph, CuGraphCSC],
     ) -> Tensor:
-        if self.use_cugraphops:
-            bipartite_graph = self.graph.to_bipartite_csc()
-            efeat_new = (
-                self.edge_trunc_mlp(efeat, nfeat, nfeat, bipartite_graph) + efeat
-            )
-
-        else:
-            efeat_new = (
-                self.edge_trunc_mlp(efeat, nfeat, nfeat, self.src, self.dst) + efeat
+        for segment_start, segment_end in self.checkpoint_segments:
+            efeat, nfeat = self.checkpoint_fn(
+                self.run_function(segment_start, segment_end),
+                efeat,
+                nfeat,
+                graph,
+                use_reentrant=False,
+                preserve_rng_state=False,
             )
 
-        return efeat_new, nfeat
-
-    def to(self, *args: Any, **kwargs: Any) -> "EdgeBlockSum":
-        """Moves the object to the specified device, dtype, or format.
-        This method moves the object and its underlying graph to the specified
-        device, dtype, or format, and returns the updated object.
-
-        Parameters
-        ----------
-        *args : Any
-            Positional arguments to be passed to the `torch._C._nn._parse_to` function.
-        **kwargs : Any
-            Keyword arguments to be passed to the `torch._C._nn._parse_to` function.
-
-        Returns
-        -------
-        EdgeBlockDGLSum
-            The updated object after moving to the specified device, dtype, or format.
-        """
-        self = super().to(*args, **kwargs)
-        device, _, _, _ = torch._C._nn._parse_to(*args, **kwargs)
-        self.graph = self.graph.to(device=device)
-        return self
+        return efeat, nfeat
```

## Comparing `modulus/models/graphcast/embedder.py` & `modulus/models/gnn_layers/embedder.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import torch.nn as nn
 from typing import Tuple
 from torch import Tensor
 
-from .mlp import MLP
+from .mesh_graph_mlp import MeshGraphMLP
 
 
-class EncoderEmbedder(nn.Module):
+class GraphCastEncoderEmbedder(nn.Module):
     """GraphCast feature embedder for gird node features, multimesh node features,
     grid2mesh edge features, and multimesh edge features.
 
     Parameters
     ----------
     input_dim_grid_nodes : int, optional
         Input dimensionality of the grid node features, by default 474
@@ -57,48 +57,48 @@
         activation_fn: nn.Module = nn.SiLU(),
         norm_type: str = "LayerNorm",
         recompute_activation: bool = False,
     ):
         super().__init__()
 
         # MLP for grid node embedding
-        self.grid_node_mlp = MLP(
+        self.grid_node_mlp = MeshGraphMLP(
             input_dim=input_dim_grid_nodes,
             output_dim=output_dim,
             hidden_dim=hidden_dim,
             hidden_layers=hidden_layers,
             activation_fn=activation_fn,
             norm_type=norm_type,
             recompute_activation=recompute_activation,
         )
 
         # MLP for mesh node embedding
-        self.mesh_node_mlp = MLP(
+        self.mesh_node_mlp = MeshGraphMLP(
             input_dim=input_dim_mesh_nodes,
             output_dim=output_dim,
             hidden_dim=hidden_dim,
             hidden_layers=hidden_layers,
             activation_fn=activation_fn,
             norm_type=norm_type,
             recompute_activation=recompute_activation,
         )
 
         # MLP for mesh edge embedding
-        self.mesh_edge_mlp = MLP(
+        self.mesh_edge_mlp = MeshGraphMLP(
             input_dim=input_dim_edges,
             output_dim=output_dim,
             hidden_dim=hidden_dim,
             hidden_layers=hidden_layers,
             activation_fn=activation_fn,
             norm_type=norm_type,
             recompute_activation=recompute_activation,
         )
 
         # MLP for grid2mesh edge embedding
-        self.grid2mesh_edge_mlp = MLP(
+        self.grid2mesh_edge_mlp = MeshGraphMLP(
             input_dim=input_dim_edges,
             output_dim=output_dim,
             hidden_dim=hidden_dim,
             hidden_layers=hidden_layers,
             activation_fn=activation_fn,
             norm_type=norm_type,
             recompute_activation=recompute_activation,
@@ -116,15 +116,15 @@
         mesh_nfeat = self.mesh_node_mlp(mesh_nfeat)
         # Input edge feature embedding
         g2m_efeat = self.grid2mesh_edge_mlp(g2m_efeat)
         mesh_efeat = self.mesh_edge_mlp(mesh_efeat)
         return grid_nfeat, mesh_nfeat, g2m_efeat, mesh_efeat
 
 
-class DecoderEmbedder(nn.Module):
+class GraphCastDecoderEmbedder(nn.Module):
     """GraphCast feature embedder for mesh2grid edge features
 
     Parameters
     ----------
     input_dim_edges : int, optional
         Input dimensionality of the edge features, by default 4
     output_dim : int, optional
@@ -151,15 +151,15 @@
         activation_fn: nn.Module = nn.SiLU(),
         norm_type: str = "LayerNorm",
         recompute_activation: bool = False,
     ):
         super().__init__()
 
         # MLP for mesh2grid edge embedding
-        self.mesh2grid_edge_mlp = MLP(
+        self.mesh2grid_edge_mlp = MeshGraphMLP(
             input_dim=input_dim_edges,
             output_dim=output_dim,
             hidden_dim=hidden_dim,
             hidden_layers=hidden_layers,
             activation_fn=activation_fn,
             norm_type=norm_type,
             recompute_activation=recompute_activation,
```

## Comparing `modulus/models/graphcast/encoder.py` & `modulus/models/gnn_layers/mesh_graph_mlp.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,324 +8,411 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from typing import Tuple, Optional, Union
+
 import torch
 import torch.nn as nn
-
-from torch import Tensor
+import torch.nn.functional as F
 from dgl import DGLGraph
-from typing import Any, Tuple, Union
-from .mlp import MLP, TruncatedMLP, TruncatedMLPCuGraph
-from .utils import agg_concat_dgl, concat_efeat_dgl_m2g_g2m, CuGraphCSC
+from torch import Tensor
+from torch.autograd.function import once_differentiable
+
+from .utils import concat_efeat, sum_efeat, CuGraphCSC
+from modulus.models.layers.fused_silu import silu_backward_for
 
 try:
-    from pylibcugraphops.pytorch.operators import (
-        agg_concat_e2n,
-        update_efeat_bipartite_e2e,
-    )
+    from apex.normalization import FusedLayerNorm
+
+    apex_imported = True
 except:
-    agg_concat_e2n = None
-    update_efeat_bipartite_e2e = None
-    BipartiteCSC = None
+    apex_imported = False
+
 
+class CustomSiLuLinearAutogradFunction(torch.autograd.Function):
+    """Custom SiLU + Linear autograd function"""
 
-class EncoderConcat(nn.Module):
-    """GraphCast Grid2Mesh encoder
+    @staticmethod
+    def forward(
+        ctx,
+        features: torch.Tensor,
+        weight: torch.Tensor,
+        bias: torch.Tensor,
+    ) -> torch.Tensor:
+        # by combining SiLU and a Linear transformation
+        # we can avoid storing the activation
+        # at the cost of recomputing it during the backward
+        out = F.silu(features)
+        out = F.linear(out, weight, bias)
+        ctx.save_for_backward(features, weight)
+        return out
+
+    @staticmethod
+    @once_differentiable
+    def backward(
+        ctx, grad_output: torch.Tensor
+    ) -> Tuple[Optional[torch.Tensor], Optional[torch.Tensor], Optional[torch.Tensor],]:
+        """backward pass of the SiLU + Linear function"""
+        (
+            need_dgrad,
+            need_wgrad,
+            need_bgrad,
+        ) = ctx.needs_input_grad
+        features, weight = ctx.saved_tensors
+
+        grad_features = None
+        grad_weight = None
+        grad_bias = None
+
+        if need_bgrad:
+            grad_bias = grad_output.sum(dim=0)
+
+        if need_wgrad:
+            out = F.silu(features)
+            grad_weight = grad_output.T @ out
+
+        if need_dgrad:
+            grad_features = grad_output @ weight
+            silu_backward = silu_backward_for(features.dtype, features.dim())
+            grad_silu = silu_backward.execute([features])[0]
+            grad_features = grad_features * grad_silu
+
+        return grad_features, grad_weight, grad_bias
+
+
+class MeshGraphMLP(nn.Module):
+    """MLP layer which is commonly used in building blocks
+    of models operating on the union of grids and meshes. It
+    consists of a number of linear layers followed by an activation
+    and a norm layer following the last linear layer.
 
     Parameters
     ----------
-    graph : DGLGraph | CuGraphCSC
-        Graph structure representing the edges between mesh and grid
-    aggregation : str, optional
-        Message passing aggregation method ("sum", "mean"), by default "sum"
-    input_dim_src_nodes : int, optional
-        Input dimensionality of the source node features, by default 512
-    input_dim_dst_nodes : int, optional
-        Input dimensionality of the destination node features, by default 512
-    input_dim_edges : int, optional
-        Input dimensionality of the edge features, by default 512
-    output_dim_src_nodes : int, optional
-        Output dimensionality of the source node features, by default 512
-    output_dim_dst_nodes : int, optional
-        Output dimensionality of the destination node features, by default 512
-    output_dim_edges : int, optional
-        Output dimensionality of the edge features, by default 512
+    input_dim : int
+        dimensionality of the input features
+    output_dim : int, optional
+        dimensionality of the output features, by default 512
     hidden_dim : int, optional
-        Number of neurons in each hidden layer, by default 512
+        number of neurons in each hidden layer, by default 512
     hidden_layers : int, optional
-        Number of hiddel layers, by default 1
+        number of hidden layers, by default 1
     activation_fn : nn.Module, optional
-        Type of activation function, by default nn.SiLU()
+        , by default nn.SiLU()
     norm_type : str, optional
-        Normalization type, by default "LayerNorm"
+        normalization type, by default "LayerNorm"
     recompute_activation : bool, optional
-        Flag for recomputing activation in backward to save memory, by default False.
+        Flag for recomputing recompute_activation in backward to save memory, by default False.
         Currently, only SiLU is supported.
     """
 
     def __init__(
         self,
-        graph: Union[DGLGraph, CuGraphCSC],
-        aggregation: str = "sum",
-        input_dim_src_nodes: int = 512,
-        input_dim_dst_nodes: int = 512,
-        input_dim_edges: int = 512,
-        output_dim_src_nodes: int = 512,
-        output_dim_dst_nodes: int = 512,
-        output_dim_edges: int = 512,
+        input_dim: int,
+        output_dim: int = 512,
         hidden_dim: int = 512,
         hidden_layers: int = 1,
-        activation_fn: int = nn.SiLU(),
+        activation_fn: nn.Module = nn.SiLU(),
         norm_type: str = "LayerNorm",
         recompute_activation: bool = False,
     ):
         super().__init__()
-        self.graph = graph
-        self.aggregation = aggregation
-        self.use_cugraphops = isinstance(graph, CuGraphCSC)
-
-        # edge MLP
-        self.edge_mlp = MLP(
-            input_dim=input_dim_src_nodes + input_dim_dst_nodes + input_dim_edges,
-            output_dim=output_dim_edges,
-            hidden_dim=hidden_dim,
-            hidden_layers=hidden_layers,
-            activation_fn=activation_fn,
-            norm_type=norm_type,
-            recompute_activation=recompute_activation,
-        )
-
-        # src node MLP
-        self.src_node_mlp = MLP(
-            input_dim=input_dim_src_nodes,
-            output_dim=output_dim_src_nodes,
-            hidden_dim=hidden_dim,
-            hidden_layers=hidden_layers,
-            activation_fn=activation_fn,
-            norm_type=norm_type,
-            recompute_activation=recompute_activation,
-        )
 
-        # dst node MLP
-        self.dst_node_mlp = MLP(
-            input_dim=input_dim_dst_nodes + output_dim_edges,
-            output_dim=output_dim_dst_nodes,
-            hidden_dim=hidden_dim,
-            hidden_layers=hidden_layers,
-            activation_fn=activation_fn,
-            norm_type=norm_type,
-            recompute_activation=recompute_activation,
-        )
-
-    def forward(
-        self, g2m_efeat: Tensor, grid_nfeat: Tensor, mesh_nfeat: Tensor
-    ) -> Tuple[Tensor, Tensor]:
-        # update edge features by concatenating node features (both mesh and grid) and existing edger featues
-        # torch.int64 to avoid indexing overflows due tu current behavior of cugraph-ops
-        if self.use_cugraphops:
-            bipartite_graph = self.graph.to_bipartite_csc(dtype=torch.int64)
-            efeat = update_efeat_bipartite_e2e(
-                g2m_efeat, grid_nfeat, mesh_nfeat, bipartite_graph, mode="concat"
-            )
+        layers = [nn.Linear(input_dim, hidden_dim), activation_fn]
+        self.hidden_layers = hidden_layers
+        for _ in range(hidden_layers - 1):
+            layers += [nn.Linear(hidden_dim, hidden_dim), activation_fn]
+        layers.append(nn.Linear(hidden_dim, output_dim))
+
+        self.norm_type = norm_type
+        if norm_type is not None:
+            assert norm_type in [
+                "LayerNorm",
+                "GraphNorm",
+                "InstanceNorm",
+                "BatchNorm",
+                "MessageNorm",
+            ]
+            if norm_type == "LayerNorm" and apex_imported:
+                norm_layer = FusedLayerNorm
+            else:
+                norm_layer = getattr(nn, norm_type)
+            layers.append(norm_layer(output_dim))
+
+        self.model = nn.Sequential(*layers)
+
+        if recompute_activation:
+            assert isinstance(activation_fn, nn.SiLU)
+            self.recompute_activation = True
         else:
-            efeat = concat_efeat_dgl_m2g_g2m(
-                g2m_efeat, grid_nfeat, mesh_nfeat, self.graph
-            )
+            self.recompute_activation = False
 
-        # transform edge features
-        efeat = self.edge_mlp(efeat)
+    def default_forward(self, x: Tensor) -> Tensor:
+        """default forward pass of the MLP"""
+        return self.model(x)
+
+    @torch.jit.ignore()
+    def custom_silu_linear_forward(self, x: Tensor) -> Tensor:
+        """forward pass of the MLP where SiLU is recomputed in backward"""
+        lin = self.model[0]
+        hidden = lin(x)
+        for i in range(1, self.hidden_layers + 1):
+            lin = self.model[2 * i]
+            hidden = CustomSiLuLinearAutogradFunction.apply(
+                hidden, lin.weight, lin.bias
+            )
 
-        # aggregate messages (edge features) to obtain updated node features
-        if self.use_cugraphops:
-            static_graph = self.graph.to_static_csc()
-            cat_feat = agg_concat_e2n(mesh_nfeat, efeat, static_graph, self.aggregation)
-        else:
-            cat_feat = agg_concat_dgl(efeat, mesh_nfeat, self.graph, self.aggregation)
+        if self.norm_type is not None:
+            norm = self.model[2 * self.hidden_layers + 1]
+            hidden = norm(hidden)
+        return hidden
+
+    def forward(self, x: Tensor) -> Tensor:
+        if self.recompute_activation:
+            return self.custom_silu_linear_forward(x)
+        return self.default_forward(x)
+
+
+class MeshGraphEdgeMLPConcat(MeshGraphMLP):
+    """MLP layer which is commonly used in building blocks
+    of models operating on the union of grids and meshes. It
+    consists of a number of linear layers followed by an activation
+    and a norm layer following the last linear layer. It first
+    concatenates the input edge features and the node features of the
+    corresponding source and destination nodes of the corresponding edge
+    to create new edge features. These then are transformed through the
+    transformations mentioned above.
 
-        # update src, dst node features + residual connections
-        mesh_nfeat = mesh_nfeat + self.dst_node_mlp(cat_feat)
-        grid_nfeat = grid_nfeat + self.src_node_mlp(grid_nfeat)
-        return grid_nfeat, mesh_nfeat
-
-    def to(self, *args: Any, **kwargs: Any) -> "EncoderConcat":
-        """Moves the object to the specified device, dtype, or format.
-        This method moves the object and its underlying graph and graph features to
-        the specified device, dtype, or format, and returns the updated object.
-
-        Parameters
-        ----------
-        *args : Any
-            Positional arguments to be passed to the `torch._C._nn._parse_to` function.
-        **kwargs : Any
-            Keyword arguments to be passed to the `torch._C._nn._parse_to` function.
-
-        Returns
-        -------
-        EncoderDGLConcat
-            The updated object after moving to the specified device, dtype, or format.
-        """
-        self = super().to(*args, **kwargs)
-        device, _, _, _ = torch._C._nn._parse_to(*args, **kwargs)
-        self.graph = self.graph.to(device=device)
-        return self
+    Parameters
+    ----------
+    efeat_dim: int
+        dimension of the input edge features
+    src_dim: int
+        dimension of the input src-node features
+    dst_dim: int
+        dimension of the input dst-node features
+    output_dim : int, optional
+        dimensionality of the output features, by default 512
+    hidden_dim : int, optional
+        number of neurons in each hidden layer, by default 512
+    hidden_layers : int, optional
+        number of hidden layers, by default 1
+    activation_fn : nn.Module, optional
+        type of activation function, by default nn.SiLU()
+    norm_type : str, optional
+        normalization type, by default "LayerNorm"
+    bias : bool, optional
+        whether to use bias in the MLP, by default True
+    recompute_activation : bool, optional
+        Flag for recomputing activation in backward to save memory, by default False.
+        Currently, only SiLU is supported.
+    """
 
+    def __init__(
+        self,
+        efeat_dim: int = 512,
+        src_dim: int = 512,
+        dst_dim: int = 512,
+        output_dim: int = 512,
+        hidden_dim: int = 512,
+        hidden_layers: int = 2,
+        activation_fn: nn.Module = nn.SiLU(),
+        norm_type: str = "LayerNorm",
+        bias: bool = True,
+        recompute_activation: bool = False,
+    ):
+        cat_dim = efeat_dim + src_dim + dst_dim
+        super(MeshGraphEdgeMLPConcat, self).__init__(
+            cat_dim,
+            output_dim,
+            hidden_dim,
+            hidden_layers,
+            activation_fn,
+            norm_type,
+            recompute_activation,
+        )
 
-class EncoderSum(nn.Module):
-    """GraphCast Grid2Mesh encoder
+    def forward(
+        self,
+        efeat: Tensor,
+        nfeat: Union[Tensor, Tuple[Tensor]],
+        graph: Union[DGLGraph, CuGraphCSC],
+    ) -> Tensor:
+        efeat = concat_efeat(efeat, nfeat, graph)
+        efeat = self.model(efeat)
+        return efeat
+
+
+class MeshGraphEdgeMLPSum(nn.Module):
+    """MLP layer which is commonly used in building blocks
+    of models operating on the union of grids and meshes. It
+    consists of a number of linear layers followed by an activation
+    and a norm layer following the last linear layer. It transform
+    edge features - which originally are intended to be a concatenation
+    of previous edge features, and the node features of the corresponding
+    source and destinationn nodes - by transorming these three features
+    individually through separate linear transformations and then sums
+    them for each edge accordingly. The result of this is transformed
+    through the remaining linear layers and activation or norm functions.
 
     Parameters
     ----------
-    graph : DGLGraph | CuGraphCSC
-        graph structure representing the edges between mesh and grid
-    aggregation : str, optional
-        message passing aggregation method ("sum", "mean"), by default "sum"
-    input_dim_src_nodes : int, optional
-        input dimensionality of the source node features, by default 512
-    input_dim_dst_nodes : int, optional
-        input dimensionality of the destination node features, by default 512
-    input_dim_edges : int, optional
-        input dimensionality of the edge features, by default 512
-    output_dim_src_nodes : int, optional
-        output dimensionality of the source node features, by default 512
-    output_dim_dst_nodes : int, optional
-        output dimensionality of the destination node features, by default 512
-    output_dim_edges : int, optional
-        output dimensionality of the edge features, by default 512
+    efeat_dim: int
+        dimension of the input edge features
+    src_dim: int
+        dimension of the input src-node features
+    dst_dim: int
+        dimension of the input dst-node features
+    output_dim : int, optional
+        dimensionality of the output features, by default 512
     hidden_dim : int, optional
         number of neurons in each hidden layer, by default 512
     hidden_layers : int, optional
-        number of hiddel layers, by default 1
+        number of hidden layers, by default 1
     activation_fn : nn.Module, optional
         type of activation function, by default nn.SiLU()
     norm_type : str, optional
         normalization type, by default "LayerNorm"
+    bias : bool, optional
+        whether to use bias in the MLP, by default True
     recompute_activation : bool, optional
         Flag for recomputing activation in backward to save memory, by default False.
         Currently, only SiLU is supported.
     """
 
     def __init__(
         self,
-        graph: Union[DGLGraph, CuGraphCSC],
-        aggregation: str = "sum",
-        input_dim_src_nodes: int = 512,
-        input_dim_dst_nodes: int = 512,
-        input_dim_edges: int = 512,
-        output_dim_src_nodes: int = 512,
-        output_dim_dst_nodes: int = 512,
-        output_dim_edges: int = 512,
+        efeat_dim: int,
+        src_dim: int,
+        dst_dim: int,
+        output_dim: int = 512,
         hidden_dim: int = 512,
         hidden_layers: int = 1,
-        activation_fn: int = nn.SiLU(),
+        activation_fn: nn.Module = nn.SiLU(),
         norm_type: str = "LayerNorm",
+        bias: bool = True,
         recompute_activation: bool = False,
     ):
         super().__init__()
-        self.graph = graph
-        self.aggregation = aggregation
-        self.use_cugraphops = isinstance(graph, CuGraphCSC)
-
-        if self.use_cugraphops:
-            # edge MLP
-            self.edge_trunc_mlp = TruncatedMLPCuGraph(
-                efeat_dim=input_dim_edges,
-                src_dim=input_dim_src_nodes,
-                dst_dim=input_dim_dst_nodes,
-                output_dim=output_dim_edges,
-                hidden_dim=hidden_dim,
-                hidden_layers=hidden_layers,
-                activation_fn=activation_fn,
-                norm_type=norm_type,
-                recompute_activation=recompute_activation,
-            )
 
+        self.efeat_dim = efeat_dim
+        self.src_dim = src_dim
+        self.dst_dim = dst_dim
+
+        # this should ensure the same sequence of initializations
+        # as the original MLP-Layer in combination with a concat operation
+        tmp_lin = nn.Linear(efeat_dim + src_dim + dst_dim, hidden_dim, bias=bias)
+        # orig_weight has shape (hidden_dim, efeat_dim + src_dim + dst_dim)
+        orig_weight = tmp_lin.weight
+        w_efeat, w_src, w_dst = torch.split(
+            orig_weight, [efeat_dim, src_dim, dst_dim], dim=1
+        )
+        self.lin_efeat = nn.Parameter(w_efeat)
+        self.lin_src = nn.Parameter(w_src)
+        self.lin_dst = nn.Parameter(w_dst)
+
+        if bias:
+            self.bias = tmp_lin.bias
         else:
-            self.src, self.dst = (item.long() for item in graph.edges())
+            self.bias = None
 
-            # edge MLP
-            self.edge_trunc_mlp = TruncatedMLP(
-                efeat_dim=input_dim_edges,
-                src_dim=input_dim_src_nodes,
-                dst_dim=input_dim_dst_nodes,
-                output_dim=output_dim_edges,
-                hidden_dim=hidden_dim,
-                hidden_layers=hidden_layers,
-                activation_fn=activation_fn,
-                norm_type=norm_type,
-                recompute_activation=recompute_activation,
-            )
+        layers = [activation_fn]
+        self.hidden_layers = hidden_layers
+        for _ in range(hidden_layers - 1):
+            layers += [nn.Linear(hidden_dim, hidden_dim), activation_fn]
+        layers.append(nn.Linear(hidden_dim, output_dim))
+
+        self.norm_type = norm_type
+        if norm_type is not None:
+            assert norm_type in [
+                "LayerNorm",
+                "GraphNorm",
+                "InstanceNorm",
+                "BatchNorm",
+                "MessageNorm",
+            ]
+            if norm_type == "LayerNorm" and apex_imported:
+                norm_layer = FusedLayerNorm
+            else:
+                norm_layer = getattr(nn, norm_type)
+            layers.append(norm_layer(output_dim))
+
+        self.model = nn.Sequential(*layers)
+
+        if recompute_activation:
+            assert isinstance(activation_fn, nn.SiLU)
+            self.recompute_activation = True
+        else:
+            self.recompute_activation = False
 
-        # src node MLP
-        self.src_node_mlp = MLP(
-            input_dim=input_dim_src_nodes,
-            output_dim=output_dim_src_nodes,
-            hidden_dim=hidden_dim,
-            hidden_layers=hidden_layers,
-            activation_fn=activation_fn,
-            norm_type=norm_type,
-            recompute_activation=recompute_activation,
-        )
+    def forward_truncated_sum(
+        self,
+        efeat: Tensor,
+        nfeat: Union[Tensor, Tuple[Tensor]],
+        graph: Union[DGLGraph, CuGraphCSC],
+    ) -> Tensor:
+        """forward pass of the truncated MLP. This uses separate linear layers without
+        bias. Bias is added to one MLP, as we sum afterwards. This adds the bias to the
+         total sum, too. Having it in one F.linear should allow a fusion of the bias
+         addition while avoiding adding the bias to the "edge-level" result.
+        """
+        if isinstance(nfeat, Tensor):
+            src_feat, dst_feat = nfeat, nfeat
+        else:
+            src_feat, dst_feat = nfeat
+        mlp_efeat = F.linear(efeat, self.lin_efeat, None)
+        mlp_src = F.linear(src_feat, self.lin_src, None)
+        mlp_dst = F.linear(dst_feat, self.lin_dst, self.bias)
+        mlp_sum = sum_efeat(mlp_efeat, (mlp_src, mlp_dst), graph)
+        return mlp_sum
 
-        # dst node MLP
-        self.dst_node_mlp = MLP(
-            input_dim=input_dim_dst_nodes + output_dim_edges,
-            output_dim=output_dim_dst_nodes,
-            hidden_dim=hidden_dim,
-            hidden_layers=hidden_layers,
-            activation_fn=activation_fn,
-            norm_type=norm_type,
-            recompute_activation=recompute_activation,
+    def default_forward(
+        self,
+        efeat: Tensor,
+        nfeat: Union[Tensor, Tuple[Tensor]],
+        graph: Union[DGLGraph, CuGraphCSC],
+    ) -> Tensor:
+        """Default forward pass of the truncated MLP."""
+        mlp_sum = self.forward_truncated_sum(
+            efeat,
+            nfeat,
+            graph,
         )
+        return self.model(mlp_sum)
 
-    def forward(
-        self, g2m_efeat: Tensor, grid_nfeat: Tensor, mesh_nfeat: Tensor
-    ) -> Tuple[Tensor, Tensor]:
-        if self.use_cugraphops:
-            bipartite_graph = self.graph.to_bipartite_csc()
-            static_graph = self.graph.to_static_csc()
-
-            mlp_efeat = self.edge_trunc_mlp(
-                g2m_efeat, grid_nfeat, mesh_nfeat, bipartite_graph
-            )
-            cat_feat = agg_concat_e2n(
-                mesh_nfeat, mlp_efeat, static_graph, self.aggregation
-            )
-        else:
-            # update edge features with Truncated MLP
-            mlp_efeat = self.edge_trunc_mlp(
-                g2m_efeat, grid_nfeat, mesh_nfeat, self.src, self.dst
-            )
-            # aggregate messages (edge features) to obtain updated node features
-            cat_feat = agg_concat_dgl(
-                mlp_efeat, mesh_nfeat, self.graph, self.aggregation
+    def custom_silu_linear_forward(
+        self,
+        efeat: Tensor,
+        nfeat: Union[Tensor, Tuple[Tensor]],
+        graph: Union[DGLGraph, CuGraphCSC],
+    ) -> Tensor:
+        """Forward pass of the truncated MLP with custom SiLU function."""
+        mlp_sum = self.forward_truncated_sum(
+            efeat,
+            nfeat,
+            graph,
+        )
+        lin = self.model[1]
+        hidden = CustomSiLuLinearAutogradFunction.apply(mlp_sum, lin.weight, lin.bias)
+        for i in range(2, self.hidden_layers + 1):
+            lin = self.model[2 * i - 1]
+            hidden = CustomSiLuLinearAutogradFunction.apply(
+                hidden, lin.weight, lin.bias
             )
 
-        # update src-feat, dst-feat and apply residual connections
-        mesh_nfeat = mesh_nfeat + self.dst_node_mlp(cat_feat)
-        grid_nfeat = grid_nfeat + self.src_node_mlp(grid_nfeat)
-        return grid_nfeat, mesh_nfeat
-
-    def to(self, *args: Any, **kwargs: Any) -> "EncoderSum":
-        """Moves the object to the specified device, dtype, or format.
-        This method moves the object and its underlying graph and graph features to
-        the specified device, dtype, or format, and returns the updated object.
-
-        Parameters
-        ----------
-        *args : Any
-            Positional arguments to be passed to the `torch._C._nn._parse_to` function.
-        **kwargs : Any
-            Keyword arguments to be passed to the `torch._C._nn._parse_to` function.
-
-        Returns
-        -------
-        EncoderDGLSum
-            The updated object after moving to the specified device, dtype, or format.
-        """
-        self = super().to(*args, **kwargs)
-        device, _, _, _ = torch._C._nn._parse_to(*args, **kwargs)
-        self.graph = self.graph.to(device=device)
-        return self
+        if self.norm_type is not None:
+            norm = self.model[2 * self.hidden_layers]
+            hidden = norm(hidden)
+        return hidden
+
+    def forward(
+        self,
+        efeat: Tensor,
+        nfeat: Union[Tensor, Tuple[Tensor]],
+        graph: Union[DGLGraph, CuGraphCSC],
+    ) -> Tensor:
+        if self.recompute_activation:
+            return self.custom_silu_linear_forward(efeat, nfeat, graph)
+        return self.default_forward(efeat, nfeat, graph)
```

## Comparing `modulus/models/graphcast/node_block.py` & `modulus/models/gnn_layers/mesh_node_block.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,32 +12,26 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import torch
 import torch.nn as nn
 from torch import Tensor
 from dgl import DGLGraph
-from typing import Any, Tuple, Union
+from typing import Tuple, Union
 
-from .mlp import MLP
-from .utils import agg_concat_dgl, CuGraphCSC
+from .mesh_graph_mlp import MeshGraphMLP
+from .utils import aggregate_and_concat, CuGraphCSC
 
-try:
-    from pylibcugraphops.pytorch.operators import agg_concat_e2n
-except:
-    agg_concat_e2n = None
 
-
-class NodeBlock(nn.Module):
-    """Node block for DGLGraph
+class MeshNodeBlock(nn.Module):
+    """Node block used e.g. in GraphCast or MeshGraphNet
+    operating on a latent space represented by a mesh.
 
     Parameters
     ----------
-    graph : DGLGraph | CuGraphCSC
-        Graph.
     aggregation : str, optional
         Aggregation method (sum, mean) , by default "sum"
     input_dim_nodes : int, optional
         Input dimensionality of the node features, by default 512
     input_dim_edges : int, optional
         Input dimensionality of the edge features, by default 512
     output_dim : int, optional
@@ -53,67 +47,42 @@
     recompute_activation : bool, optional
         Flag for recomputing activation in backward to save memory, by default False.
         Currently, only SiLU is supported.
     """
 
     def __init__(
         self,
-        graph: Union[DGLGraph, CuGraphCSC],
         aggregation: str = "sum",
         input_dim_nodes: int = 512,
         input_dim_edges: int = 512,
         output_dim: int = 512,
         hidden_dim: int = 512,
         hidden_layers: int = 1,
         activation_fn: nn.Module = nn.SiLU(),
         norm_type: str = "LayerNorm",
         recompute_activation: bool = False,
     ):
         super().__init__()
-        self.graph = graph
         self.aggregation = aggregation
 
-        self.use_cugraphops = isinstance(graph, CuGraphCSC)
-
-        self.node_mlp = MLP(
+        self.node_mlp = MeshGraphMLP(
             input_dim=input_dim_nodes + input_dim_edges,
             output_dim=output_dim,
             hidden_dim=hidden_dim,
             hidden_layers=hidden_layers,
             activation_fn=activation_fn,
             norm_type=norm_type,
             recompute_activation=recompute_activation,
         )
 
-    def forward(self, efeat: Tensor, nfeat: Tensor) -> Tuple[Tensor, Tensor]:
-        if self.use_cugraphops:
-            static_graph = self.graph.to_static_csc()
-            cat_feat = agg_concat_e2n(nfeat, efeat, static_graph, self.aggregation)
-
-        else:
-            cat_feat = agg_concat_dgl(efeat, nfeat, self.graph, self.aggregation)
-
+    @torch.jit.ignore()
+    def forward(
+        self,
+        efeat: Tensor,
+        nfeat: Tensor,
+        graph: Union[DGLGraph, CuGraphCSC],
+    ) -> Tuple[Tensor, Tensor]:
+        # update edge features
+        cat_feat = aggregate_and_concat(efeat, nfeat, graph, self.aggregation)
         # update node features + residual connection
         nfeat_new = self.node_mlp(cat_feat) + nfeat
         return efeat, nfeat_new
-
-    def to(self, *args: Any, **kwargs: Any) -> "NodeBlock":
-        """Moves the object to the specified device, dtype, or format.
-        This method moves the object and its underlying graph and graph features to
-        the specified device, dtype, or format, and returns the updated object.
-
-        Parameters
-        ----------
-        *args : Any
-            Positional arguments to be passed to the `torch._C._nn._parse_to` function.
-        **kwargs : Any
-            Keyword arguments to be passed to the `torch._C._nn._parse_to` function.
-
-        Returns
-        -------
-        NodeBlockDGL
-            The updated object after moving to the specified device, dtype, or format.
-        """
-        self = super().to(*args, **kwargs)
-        device, _, _, _ = torch._C._nn._parse_to(*args, **kwargs)
-        self.graph = self.graph.to(device=device)
-        return self
```

## Comparing `modulus/models/graphcast/utils.py` & `modulus/models/gnn_layers/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,23 +12,29 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import torch
 from torch import Tensor
 from dgl import DGLGraph
 import dgl.function as fn
-from typing import Any, Callable, Dict, Optional
+from typing import Any, Callable, Dict, Optional, Union, Tuple
 from torch.utils.checkpoint import checkpoint
 
 
 try:
     from pylibcugraphops.pytorch import StaticCSC, BipartiteCSC
+    from pylibcugraphops.pytorch.operators import (
+        update_efeat_bipartite_e2e,
+        update_efeat_static_e2e,
+        agg_concat_e2n,
+    )
 except:
-    StaticCSC = None
-    BipartiteCSC = None
+    update_efeat_bipartite_e2e = None
+    update_efeat_static_e2e = None
+    agg_concat_e2n = None
 
 
 class CuGraphCSC:
     """Constructs a CuGraphCSC object.
 
     Parameters
     ----------
@@ -40,32 +46,37 @@
         The number of source nodes.
     num_dst_nodes : int
         The number of destination nodes.
     ef_indices : Optional[Tensor], optional
         The edge feature indices tensor, by default None
     reverse_graph_bwd : bool, optional
         Whether to reverse the graph for the backward pass, by default True
+    cache_graph : bool, optional
+        Whether to cache graph structures when wrapping offsets and indices
+        to the corresponding cugraph-ops graph types. If graph change in each
+        iteration, set to False, by default True.
     """
 
     def __init__(
         self,
         offsets: Tensor,
         indices: Tensor,
         num_src_nodes: int,
         num_dst_nodes: int,
         ef_indices: Optional[Tensor] = None,
         reverse_graph_bwd: bool = True,
+        cache_graph: bool = True,
     ) -> None:
-
         self.offsets = offsets
         self.indices = indices
         self.num_src_nodes = num_src_nodes
         self.num_dst_nodes = num_dst_nodes
         self.ef_indices = ef_indices
         self.reverse_graph_bwd = reverse_graph_bwd
+        self.cache_graph = cache_graph
 
         self.bipartite_csc = None
         self.static_csc = None
 
     def to(self, *args: Any, **kwargs: Any) -> "CuGraphCSC":
         """Moves the object to the specified device, dtype, or format and returns the
         updated object.
@@ -91,32 +102,30 @@
         self.offsets = self.offsets.to(device=device, dtype=dtype)
         self.indices = self.indices.to(device=device, dtype=dtype)
         if self.ef_indices is not None:
             self.ef_indices = self.ef_indices.to(device=device, dtype=dtype)
 
         return self
 
-    def to_bipartite_csc(self, dtype=None, cache_graph: bool = True):
+    def to_bipartite_csc(self, dtype=None):
         """Converts the graph to a bipartite CSC graph.
 
         Parameters
         ----------
         dtype : torch.dtype, optional
             The dtype of the graph, by default None
-        cache_graph : bool, optional
-            Whether to cache the graph, by default True
 
         Returns
         -------
         BipartiteCSC
             The bipartite CSC graph.
         """
 
         assert self.offsets.is_cuda, "Expected the graph structures to reside on GPU."
-        if self.bipartite_csc is None or not cache_graph:
+        if self.bipartite_csc is None or not self.cache_graph:
             # Occassionally, we have to watch out for the IdxT type
             # of offsets and indices. Technically, they are only relevant
             # for storing node and edge indices. However, they are also used
             # to index pointers in the underlying kernels (for now). This means
             # that depending on the data dimension, one has to rely on int64
             # for the indices despite int32 technically being enough to store the
             # graph. This will be improved in cugraph-ops-23.06. Until then, allow
@@ -138,31 +147,29 @@
                 graph_ef_indices,
                 reverse_graph_bwd=self.reverse_graph_bwd,
             )
             self.bipartite_csc = graph
 
         return self.bipartite_csc
 
-    def to_static_csc(self, dtype=None, cache_graph: bool = True):
+    def to_static_csc(self, dtype=None):
         """Converts the graph to a static CSC graph.
 
         Parameters
         ----------
         dtype : torch.dtype, optional
             The dtype of the graph, by default None
-        cache_graph : bool, optional
-            Whether to cache the graph, by default True
 
         Returns
         -------
         StaticCSC
             The static CSC graph.
         """
 
-        if self.static_csc is None or not cache_graph:
+        if self.static_csc is None or not self.cache_graph:
             # Occassionally, we have to watch out for the IdxT type
             # of offsets and indices. Technically, they are only relevant
             # for storing node and edge indices. However, they are also used
             # to index pointers in the underlying kernels (for now). This means
             # that depending on the data dimension, one has to rely on int64
             # for the indices despite int32 technically being enough to store the
             # graph. This will be improved in cugraph-ops-23.06. Until then, allow
@@ -252,69 +259,103 @@
         Concatenated source node, destination node, and edge features.
     """
     # concats src node , dst node, and edge features
     cat_feat = torch.cat((edges.data["x"], edges.src["x"], edges.dst["x"]), dim=1)
     return {"cat_feat": cat_feat}
 
 
-def concat_efeat_dgl_mesh(efeat: Tensor, nfeat: Tensor, graph: DGLGraph) -> Tensor:
+@torch.jit.ignore()
+def concat_efeat_dgl(
+    efeat: Tensor,
+    nfeat: Union[Tensor, Tuple[torch.Tensor, torch.Tensor]],
+    graph: DGLGraph,
+) -> Tensor:
     """Concatenates edge features with source and destination node features.
     Use for homogeneous graphs.
 
     Parameters
     ----------
     efeat : Tensor
         Edge features.
-    nfeat : Tensor
+    nfeat : Tensor | Tuple[Tensor, Tensor]
         Node features.
     graph : DGLGraph
         Graph.
 
     Returns
     -------
     Tensor
         Concatenated edge features with source and destination node features.
     """
+    if isinstance(nfeat, Tuple):
+        src_feat, dst_feat = nfeat
+        with graph.local_scope():
+            graph.srcdata["x"] = src_feat
+            graph.dstdata["x"] = dst_feat
+            graph.edata["x"] = efeat
+            graph.apply_edges(concat_message_function)
+            return graph.edata["cat_feat"]
+
     with graph.local_scope():
         graph.ndata["x"] = nfeat
         graph.edata["x"] = efeat
-
         graph.apply_edges(concat_message_function)
         return graph.edata["cat_feat"]
 
 
-def concat_efeat_dgl_m2g_g2m(
-    efeat: Tensor, src_feat: Tensor, dst_feat: Tensor, graph: DGLGraph
+def concat_efeat(
+    efeat: Tensor,
+    nfeat: Union[Tensor, Tuple[Tensor]],
+    graph: Union[DGLGraph, CuGraphCSC],
 ) -> Tensor:
     """Concatenates edge features with source and destination node features.
-    Use for heterogeneous graphs.
+    Use for homogeneous graphs.
 
     Parameters
     ----------
     efeat : Tensor
         Edge features.
-    src_feat : Tensor
-        Source node features.
-    dst_feat : Tensor
-        Destination node features.
-    graph : DGLGraph
+    nfeat : Tensor | Tuple[Tensor]
+        Node features.
+    graph : DGLGraph | CuGraphCSC
         Graph.
 
     Returns
     -------
     Tensor
         Concatenated edge features with source and destination node features.
     """
-    with graph.local_scope():
-        graph.srcdata["x"] = src_feat
-        graph.dstdata["x"] = dst_feat
-        graph.edata["x"] = efeat
+    if isinstance(nfeat, Tensor):
+        if isinstance(graph, CuGraphCSC):
+            static_graph = graph.to_static_csc()
+            efeat = update_efeat_static_e2e(
+                efeat,
+                nfeat,
+                static_graph,
+                mode="concat",
+                use_source_emb=True,
+                use_target_emb=True,
+            )
 
-        graph.apply_edges(concat_message_function)
-        return graph.edata["cat_feat"]
+        else:
+            efeat = concat_efeat_dgl(efeat, nfeat, graph)
+
+    else:
+        src_feat, dst_feat = nfeat
+        # update edge features through concatenating edge and node features
+        if isinstance(graph, CuGraphCSC):
+            # torch.int64 to avoid indexing overflows due tu current behavior of cugraph-ops
+            bipartite_graph = graph.to_bipartite_csc(dtype=torch.int64)
+            efeat = update_efeat_bipartite_e2e(
+                efeat, src_feat, dst_feat, bipartite_graph, "concat"
+            )
+        else:
+            efeat = concat_efeat_dgl(efeat, (src_feat, dst_feat), graph)
+
+    return efeat
 
 
 @torch.jit.script
 def sum_efeat_dgl(
     efeat: Tensor, src_feat: Tensor, dst_feat: Tensor, src_idx: Tensor, dst_idx: Tensor
 ) -> Tensor:
     """Sums edge features with source and destination node features.
@@ -333,37 +374,87 @@
         Destination node indices.
 
     Returns
     -------
     Tensor
         Sum of edge features with source and destination node features.
     """
+
     return efeat + src_feat[src_idx] + dst_feat[dst_idx]
 
 
+def sum_efeat(
+    efeat: Tensor,
+    nfeat: Union[Tensor, Tuple[Tensor]],
+    graph: Union[DGLGraph, CuGraphCSC],
+):
+    """Sums edge features with source and destination node features.
+
+    Parameters
+    ----------
+    efeat : Tensor
+        Edge features.
+    nfeat : Tensor | Tuple[Tensor]
+        Node features (static setting) or tuple of node features of
+        source and destination nodes (bipartite setting).
+    graph : DGLGraph | CuGraphCSC
+        The underlying graph.
+
+    Returns
+    -------
+    Tensor
+        Sum of edge features with source and destination node features.
+    """
+    if isinstance(nfeat, Tensor):
+        if isinstance(graph, CuGraphCSC):
+            static_graph = graph.to_static_csc()
+            sum_efeat = update_efeat_bipartite_e2e(
+                efeat, nfeat, static_graph, mode="sum"
+            )
+
+        else:
+            src_feat, dst_feat = nfeat, nfeat
+            src, dst = (item.long() for item in graph.edges())
+            sum_efeat = sum_efeat_dgl(efeat, src_feat, dst_feat, src, dst)
+
+    else:
+        src_feat, dst_feat = nfeat
+        if isinstance(graph, CuGraphCSC):
+            bipartite_graph = graph.to_bipartite_csc()
+            sum_efeat = update_efeat_bipartite_e2e(
+                efeat, src_feat, dst_feat, bipartite_graph, mode="sum"
+            )
+        else:
+            src, dst = (item.long() for item in graph.edges())
+            sum_efeat = sum_efeat_dgl(efeat, src_feat, dst_feat, src, dst)
+
+    return sum_efeat
+
+
+@torch.jit.ignore()
 def agg_concat_dgl(
-    efeat: Tensor, nfeat: Tensor, graph: DGLGraph, aggregation: str
+    efeat: Tensor, dst_nfeat: Tensor, graph: DGLGraph, aggregation: str
 ) -> Tensor:
-    """Aggregates edge features and concatenates with node features.
+    """Aggregates edge features and concatenates result with destination node features.
 
     Parameters
     ----------
     efeat : Tensor
         Edge features.
     nfeat : Tensor
-        Node features.
+        Node features (destination nodes).
     graph : DGLGraph
         Graph.
     aggregation : str
         Aggregation method (sum or mean).
 
     Returns
     -------
     Tensor
-        Aggregated edge features concatenated with node features.
+        Aggregated edge features concatenated with destination node features.
 
     Raises
     ------
     RuntimeError
         If aggregation method is not sum or mean.
     """
     with graph.local_scope():
@@ -374,10 +465,50 @@
         if aggregation == "sum":
             graph.update_all(fn.copy_e("x", "m"), fn.sum("m", "h_dest"))
         elif aggregation == "mean":
             graph.update_all(fn.copy_e("x", "m"), fn.mean("m", "h_dest"))
         else:
             raise RuntimeError("Not a valid aggregation!")
 
-        # concat node & edge features
-        cat_feat = torch.cat((graph.dstdata["h_dest"], nfeat), -1)
+        # concat dst-node & edge features
+        cat_feat = torch.cat((graph.dstdata["h_dest"], dst_nfeat), -1)
         return cat_feat
+
+
+def aggregate_and_concat(
+    efeat: Tensor,
+    nfeat: Tensor,
+    graph: Union[DGLGraph, CuGraphCSC],
+    aggregation: str,
+):
+    """
+    Aggregates edge features and concatenates result with destination node features.
+
+    Parameters
+    ----------
+    efeat : Tensor
+        Edge features.
+    nfeat : Tensor
+        Node features (destination nodes).
+    graph : DGLGraph
+        Graph.
+    aggregation : str
+        Aggregation method (sum or mean).
+
+    Returns
+    -------
+    Tensor
+        Aggregated edge features concatenated with destination node features.
+
+    Raises
+    ------
+    RuntimeError
+        If aggregation method is not sum or mean.
+    """
+
+    if isinstance(graph, CuGraphCSC):
+        static_graph = graph.to_static_csc()
+        cat_feat = agg_concat_e2n(nfeat, efeat, static_graph, aggregation)
+    else:
+        cat_feat = agg_concat_dgl(efeat, nfeat, graph, aggregation)
+
+    return cat_feat
```

## Comparing `nvidia_modulus-0.1.0.dist-info/LICENSE.txt` & `nvidia_modulus-0.2.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

